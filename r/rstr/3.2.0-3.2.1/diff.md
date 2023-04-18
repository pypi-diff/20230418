# Comparing `tmp/rstr-3.2.0.tar.gz` & `tmp/rstr-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rstr-3.2.0.tar", last modified: Wed May 25 21:23:39 2022, max compression
+gzip compressed data, was "rstr-3.2.1.tar", last modified: Tue Apr 18 19:34:43 2023, max compression
```

## Comparing `rstr-3.2.0.tar` & `rstr-3.2.1.tar`

### file list

```diff
@@ -1,22 +1,28 @@
-drwxrwxr-x   0 bjmc      (1000) bjmc      (1000)        0 2022-05-25 21:23:39.827694 rstr-3.2.0/
--rw-r--r--   0 bjmc      (1000) bjmc      (1000)     1636 2020-07-04 14:13:44.000000 rstr-3.2.0/LICENSE.txt
--rw-rw-r--   0 bjmc      (1000) bjmc      (1000)       42 2022-05-24 06:43:18.000000 rstr-3.2.0/MANIFEST.in
--rw-rw-r--   0 bjmc      (1000) bjmc      (1000)     8833 2022-05-25 21:23:39.827694 rstr-3.2.0/PKG-INFO
--rw-rw-r--   0 bjmc      (1000) bjmc      (1000)     6168 2021-11-27 16:44:44.000000 rstr-3.2.0/README.rst
--rw-rw-r--   0 bjmc      (1000) bjmc      (1000)      104 2021-08-01 19:17:07.000000 rstr-3.2.0/pyproject.toml
-drwxrwxr-x   0 bjmc      (1000) bjmc      (1000)        0 2022-05-25 21:23:39.827694 rstr-3.2.0/rstr/
--rw-rw-r--   0 bjmc      (1000) bjmc      (1000)     1016 2021-11-27 16:44:55.000000 rstr-3.2.0/rstr/__init__.py
--rw-rw-r--   0 bjmc      (1000) bjmc      (1000)        0 2022-05-24 06:43:18.000000 rstr-3.2.0/rstr/py.typed
--rw-rw-r--   0 bjmc      (1000) bjmc      (1000)     7883 2021-11-27 16:44:55.000000 rstr-3.2.0/rstr/rstr_base.py
-drwxrwxr-x   0 bjmc      (1000) bjmc      (1000)        0 2022-05-25 21:23:39.827694 rstr-3.2.0/rstr/tests/
--rw-rw-r--   0 bjmc      (1000) bjmc      (1000)        0 2021-11-27 16:17:19.000000 rstr-3.2.0/rstr/tests/__init__.py
--rw-rw-r--   0 bjmc      (1000) bjmc      (1000)      400 2021-11-27 16:44:55.000000 rstr-3.2.0/rstr/tests/test_package_level_access.py
--rw-rw-r--   0 bjmc      (1000) bjmc      (1000)     4516 2021-11-27 16:44:55.000000 rstr-3.2.0/rstr/tests/test_rstr.py
--rw-rw-r--   0 bjmc      (1000) bjmc      (1000)     2965 2021-11-27 16:44:55.000000 rstr-3.2.0/rstr/tests/test_xeger.py
--rw-rw-r--   0 bjmc      (1000) bjmc      (1000)     4128 2022-05-24 06:43:18.000000 rstr-3.2.0/rstr/xeger.py
-drwxrwxr-x   0 bjmc      (1000) bjmc      (1000)        0 2022-05-25 21:23:39.827694 rstr-3.2.0/rstr.egg-info/
--rw-r--r--   0 bjmc      (1000) bjmc      (1000)     8833 2022-05-25 21:23:39.000000 rstr-3.2.0/rstr.egg-info/PKG-INFO
--rw-r--r--   0 bjmc      (1000) bjmc      (1000)      346 2022-05-25 21:23:39.000000 rstr-3.2.0/rstr.egg-info/SOURCES.txt
--rw-r--r--   0 bjmc      (1000) bjmc      (1000)        1 2022-05-25 21:23:39.000000 rstr-3.2.0/rstr.egg-info/dependency_links.txt
--rw-r--r--   0 bjmc      (1000) bjmc      (1000)        5 2022-05-25 21:23:39.000000 rstr-3.2.0/rstr.egg-info/top_level.txt
--rw-rw-r--   0 bjmc      (1000) bjmc      (1000)     1008 2022-05-25 21:23:39.831694 rstr-3.2.0/setup.cfg
+drwxrwxr-x   0 bjmc      (1000) bjmc      (1000)        0 2023-04-18 19:34:43.484581 rstr-3.2.1/
+drwxrwxr-x   0 bjmc      (1000) bjmc      (1000)        0 2023-04-18 19:34:43.480581 rstr-3.2.1/.circleci/
+-rw-rw-r--   0 bjmc      (1000) bjmc      (1000)      249 2023-04-18 18:20:47.000000 rstr-3.2.1/.circleci/config.yml
+-rw-rw-r--   0 bjmc      (1000) bjmc      (1000)       67 2021-08-01 21:25:20.000000 rstr-3.2.1/.gitignore
+-rw-rw-r--   0 bjmc      (1000) bjmc      (1000)      133 2023-04-18 17:45:26.000000 rstr-3.2.1/AUTHORS
+-rw-r--r--   0 bjmc      (1000) bjmc      (1000)     1636 2020-07-04 14:13:44.000000 rstr-3.2.1/LICENSE.txt
+-rw-rw-r--   0 bjmc      (1000) bjmc      (1000)       42 2022-05-24 06:43:18.000000 rstr-3.2.1/MANIFEST.in
+-rw-rw-r--   0 bjmc      (1000) bjmc      (1000)     7144 2023-04-18 19:34:43.484581 rstr-3.2.1/PKG-INFO
+-rw-rw-r--   0 bjmc      (1000) bjmc      (1000)     6168 2021-11-27 16:44:44.000000 rstr-3.2.1/README.rst
+-rw-rw-r--   0 bjmc      (1000) bjmc      (1000)      589 2023-04-18 19:29:04.000000 rstr-3.2.1/RELEASE_NOTES
+-rw-rw-r--   0 bjmc      (1000) bjmc      (1000)     1240 2023-04-18 19:27:02.000000 rstr-3.2.1/pyproject.toml
+drwxrwxr-x   0 bjmc      (1000) bjmc      (1000)        0 2023-04-18 19:34:43.480581 rstr-3.2.1/rstr/
+-rw-rw-r--   0 bjmc      (1000) bjmc      (1000)      994 2023-04-18 17:45:26.000000 rstr-3.2.1/rstr/__init__.py
+-rw-rw-r--   0 bjmc      (1000) bjmc      (1000)        0 2022-05-24 06:43:18.000000 rstr-3.2.1/rstr/py.typed
+-rw-rw-r--   0 bjmc      (1000) bjmc      (1000)     7832 2023-04-18 17:45:26.000000 rstr-3.2.1/rstr/rstr_base.py
+-rw-rw-r--   0 bjmc      (1000) bjmc      (1000)     4245 2023-04-18 18:20:47.000000 rstr-3.2.1/rstr/xeger.py
+drwxrwxr-x   0 bjmc      (1000) bjmc      (1000)        0 2023-04-18 19:34:43.480581 rstr-3.2.1/rstr.egg-info/
+-rw-r--r--   0 bjmc      (1000) bjmc      (1000)     7144 2023-04-18 19:34:43.000000 rstr-3.2.1/rstr.egg-info/PKG-INFO
+-rw-r--r--   0 bjmc      (1000) bjmc      (1000)      378 2023-04-18 19:34:43.000000 rstr-3.2.1/rstr.egg-info/SOURCES.txt
+-rw-r--r--   0 bjmc      (1000) bjmc      (1000)        1 2023-04-18 19:34:43.000000 rstr-3.2.1/rstr.egg-info/dependency_links.txt
+-rw-r--r--   0 bjmc      (1000) bjmc      (1000)        5 2023-04-18 19:34:43.000000 rstr-3.2.1/rstr.egg-info/top_level.txt
+-rw-rw-r--   0 bjmc      (1000) bjmc      (1000)       38 2023-04-18 19:34:43.484581 rstr-3.2.1/setup.cfg
+drwxrwxr-x   0 bjmc      (1000) bjmc      (1000)        0 2023-04-18 19:34:43.484581 rstr-3.2.1/tests/
+-rw-rw-r--   0 bjmc      (1000) bjmc      (1000)        0 2023-04-18 17:45:26.000000 rstr-3.2.1/tests/__init__.py
+-rw-rw-r--   0 bjmc      (1000) bjmc      (1000)      401 2023-04-18 17:45:26.000000 rstr-3.2.1/tests/test_package_level_access.py
+-rw-rw-r--   0 bjmc      (1000) bjmc      (1000)     4506 2023-04-18 17:45:26.000000 rstr-3.2.1/tests/test_rstr.py
+-rw-rw-r--   0 bjmc      (1000) bjmc      (1000)     2964 2023-04-18 17:45:26.000000 rstr-3.2.1/tests/test_xeger.py
+-rw-rw-r--   0 bjmc      (1000) bjmc      (1000)      216 2023-04-18 18:20:47.000000 rstr-3.2.1/tox.ini
```

### Comparing `rstr-3.2.0/LICENSE.txt` & `rstr-3.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rstr-3.2.0/PKG-INFO` & `rstr-3.2.1/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,241 +1,217 @@
-Metadata-Version: 2.1
-Name: rstr
-Version: 3.2.0
-Summary: Generate random strings in Python
-Home-page: https://github.com/leapfrogonline/rstr
-Author: Leapfrog Direct Response LLC
-Author-email: oss@leapfrogdevelopment.com
-Maintainer: Brendan McCollam
-Maintainer-email: rstr@mccoll.am
-License: UNKNOWN
-Description: ===============================
-        rstr = Random Strings in Python
-        ===============================
-        
-        .. image:: https://circleci.com/gh/leapfrogonline/rstr.svg?style=svg
-            :target: https://circleci.com/gh/leapfrogonline/rstr
-        
-        rstr is a helper module for easily generating random strings of various types.
-        It could be useful for fuzz testing, generating dummy data, or other
-        applications.
-        
-        It has no dependencies outside the standard library.
-        
-        A Word of Caution
-        -----------------
-        
-        By default, rstr uses the Python ``random`` module to generate pseudorandom text. This module is based on the Mersenne Twister and is *not* cryptographically secure.
-        
-        **If you wish to use rstr for password-generation or other cryptographic
-        applications, you must create an instance that uses** SystemRandom_.
-        
-        For example:
-        
-        ::
-        
-            >> from rstr import Rstr
-            >> from random import SystemRandom
-            >> rs = Rstr(SystemRandom())
-        
-        
-        Use
-        ---
-        
-        The basic method of rstr is ``rstr()``. At a minimum, it requires one argument,
-        an alphabet of characters from which to create a string.
-        
-        ::
-        
-            >>> import rstr
-            >>> rstr.rstr('ABC')
-            'AACAACCB'
-        
-        By default, it will return a string between 1 and 10 characters in length. You
-        may specify an exact length by including it as a second argument:
-        
-        ::
-        
-            >>> rstr.rstr('ABC', 4)
-            'ACBC'
-        
-        You can also generate a range of lengths by adding two arguments. In the following
-        case, rstr will return a string with a randomly selected length between 5 and 10
-        characters.
-        
-        ::
-        
-            >>> rstr.rstr('ABC', 5, 10)
-            'CBCCCABAA'
-        
-        It's also possible to include particular characters in your string. This is useful
-        when testing a validator to make sure that certain characters are rejected.
-        Characters listed in the 'include' argument will *always* be present somewhere
-        in the resulting string.
-        
-        ::
-        
-            >>> rstr.rstr('ABC', include='&')
-            'CA&A'
-        
-        Conversely, you can exclude particular characters from the generated string. This is
-        helpful when starting with a pre-defined population of characters.
-        
-        ::
-        
-            >>> import string
-            >>> rstr.rstr(string.digits, exclude='5')
-            '8661442'
-        
-        Note that any of the arguments that accept strings can also
-        accept lists or tuples of strings:
-        
-        ::
-        
-            >>> rstr.rstr(['A', 'B', 'C'], include = ['@'], exclude=('C',))
-            'BAAABBA@BAA'
-        
-        Other methods
-        -------------
-        
-        The other methods provided by rstr, besides ``rstr()`` and ``xeger()``, are convenience
-        methods that can be called without arguments, and provide a pre-defined alphabet.
-        They accept the same arguments as ``rstr()`` for purposes of
-        specifying lengths and including or excluding particular characters.
-        
-        letters()
-            The characters provided by string.letters in the standard library.
-        
-        uppercase()
-            The characters provided by string.uppercase in the standard library.
-        
-        lowercase()
-            The characters provided by string.lowercase in the standard library.
-        
-        printable()
-            The characters provided by string.printable in the standard library.
-        
-        punctuation()
-            The characters provided by string.punctuation in the standard library.
-        
-        nonwhitespace()
-            The characters provided by string.printable in the standard library, except
-            for those representing whitespace: tab, space, etc.
-        
-        digits()
-            The characters provided by string.digits in the standard library.
-        
-        nondigits()
-            The characters provided by the concatenation of string.letters and
-            string.punctuation in the standard library.
-        
-        nonletters()
-            The characters provided by the concatenation of string.digits and
-            string.punctuation in the standard library.
-        
-        normal()
-            Characters commonly accepted in text input, equivalent to string.digits +
-            string.letters + ' ' (the space character).
-        
-        unambiguous()
-            The characters provided by the concatenation of string.digits and
-            string.letters except characters which are similar: 1, l and I, etc.
-        
-        postalsafe()
-            Characters that are safe for use in postal addresses in the United States:
-            upper- and lower-case letters, digits, spaces, and the punctuation marks period,
-            hash (#), hyphen, and forward-slash.
-        
-        urlsafe()
-            Characters safe (unreserved) for use in URLs: letters, digits, hyphen, period, underscore,
-            and tilde.
-        
-        domainsafe()
-            Characters that are allowed for use in hostnames, and consequently, in internet domains: letters,
-            digits, and the hyphen.
-        
-        Xeger
-        -----
-        
-        Inspired by the Java library of the same name, the ``xeger()`` method allows users to
-        create a random string from a regular expression.
-        
-        For example to generate a postal code that fits the Canadian format:
-        
-            >>> import rstr
-            >>> rstr.xeger(r'[A-Z]\d[A-Z] \d[A-Z]\d')
-            u'R6M 1W5'
-        
-        xeger works fine with most simple regular expressions, but it doesn't support all
-        Python regular expression features.
-        
-        Custom Alphabets
-        ----------------
-        
-        If you have custom alphabets of characters that you would like to use with a method
-        shortcut, you can specify them by keyword when instantiating an Rstr object:
-        
-            >>> from rstr import Rstr
-            >>> rs = Rstr(vowels='AEIOU')
-            >>> rs.vowels()
-            'AEEUU'
-        
-        You can also add an alphabet to an existing instance with the add_alphabet() method:
-        
-            >>> rs.add_alphabet('odds', '13579')
-            >>> rs.odds()
-            '339599519'
-        
-        Examples
-        --------
-        
-        You can combine rstr with Python's built-in string formatting to produce strings
-        that fit a variety of templates.
-        
-        An email address:
-        
-        ::
-        
-            '{0}@{1}.{2}'.format(rstr.nonwhitespace(exclude='@'),
-                                 rstr.domainsafe(),
-                                 rstr.letters(3))
-        
-        A URL:
-        
-        ::
-        
-            'http://{0}.{1}/{2}/?{3}'.format(rstr.domainsafe(),
-                                            rstr.letters(3),
-                                            rstr.urlsafe(),
-                                            rstr.urlsafe())
-        
-        A postal address:
-        
-        ::
-        
-            """{0} {1}
-            {2} {3}
-            {4}, {5} {6}
-            """.format(rstr.letters(4, 8).title(),
-                       rstr.letters(4, 8).title(),
-                       rstr.digits(3, 5),
-                       rstr.letters(4, 10).title(),
-                       rstr.letters(4, 15).title(),
-                       rstr.uppercase(2),
-                       rstr.digits(5),
-                       )
-        
-        .. _SystemRandom: https://docs.python.org/3/library/random.html#random.SystemRandom
-        
-Keywords: random string,reverse regex,reverse regular expression,testing,fuzz testing
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development :: Testing
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
+===============================
+rstr = Random Strings in Python
+===============================
+
+.. image:: https://circleci.com/gh/leapfrogonline/rstr.svg?style=svg
+    :target: https://circleci.com/gh/leapfrogonline/rstr
+
+rstr is a helper module for easily generating random strings of various types.
+It could be useful for fuzz testing, generating dummy data, or other
+applications.
+
+It has no dependencies outside the standard library.
+
+A Word of Caution
+-----------------
+
+By default, rstr uses the Python ``random`` module to generate pseudorandom text. This module is based on the Mersenne Twister and is *not* cryptographically secure.
+
+**If you wish to use rstr for password-generation or other cryptographic
+applications, you must create an instance that uses** SystemRandom_.
+
+For example:
+
+::
+
+    >> from rstr import Rstr
+    >> from random import SystemRandom
+    >> rs = Rstr(SystemRandom())
+
+
+Use
+---
+
+The basic method of rstr is ``rstr()``. At a minimum, it requires one argument,
+an alphabet of characters from which to create a string.
+
+::
+
+    >>> import rstr
+    >>> rstr.rstr('ABC')
+    'AACAACCB'
+
+By default, it will return a string between 1 and 10 characters in length. You
+may specify an exact length by including it as a second argument:
+
+::
+
+    >>> rstr.rstr('ABC', 4)
+    'ACBC'
+
+You can also generate a range of lengths by adding two arguments. In the following
+case, rstr will return a string with a randomly selected length between 5 and 10
+characters.
+
+::
+
+    >>> rstr.rstr('ABC', 5, 10)
+    'CBCCCABAA'
+
+It's also possible to include particular characters in your string. This is useful
+when testing a validator to make sure that certain characters are rejected.
+Characters listed in the 'include' argument will *always* be present somewhere
+in the resulting string.
+
+::
+
+    >>> rstr.rstr('ABC', include='&')
+    'CA&A'
+
+Conversely, you can exclude particular characters from the generated string. This is
+helpful when starting with a pre-defined population of characters.
+
+::
+
+    >>> import string
+    >>> rstr.rstr(string.digits, exclude='5')
+    '8661442'
+
+Note that any of the arguments that accept strings can also
+accept lists or tuples of strings:
+
+::
+
+    >>> rstr.rstr(['A', 'B', 'C'], include = ['@'], exclude=('C',))
+    'BAAABBA@BAA'
+
+Other methods
+-------------
+
+The other methods provided by rstr, besides ``rstr()`` and ``xeger()``, are convenience
+methods that can be called without arguments, and provide a pre-defined alphabet.
+They accept the same arguments as ``rstr()`` for purposes of
+specifying lengths and including or excluding particular characters.
+
+letters()
+    The characters provided by string.letters in the standard library.
+
+uppercase()
+    The characters provided by string.uppercase in the standard library.
+
+lowercase()
+    The characters provided by string.lowercase in the standard library.
+
+printable()
+    The characters provided by string.printable in the standard library.
+
+punctuation()
+    The characters provided by string.punctuation in the standard library.
+
+nonwhitespace()
+    The characters provided by string.printable in the standard library, except
+    for those representing whitespace: tab, space, etc.
+
+digits()
+    The characters provided by string.digits in the standard library.
+
+nondigits()
+    The characters provided by the concatenation of string.letters and
+    string.punctuation in the standard library.
+
+nonletters()
+    The characters provided by the concatenation of string.digits and
+    string.punctuation in the standard library.
+
+normal()
+    Characters commonly accepted in text input, equivalent to string.digits +
+    string.letters + ' ' (the space character).
+
+unambiguous()
+    The characters provided by the concatenation of string.digits and
+    string.letters except characters which are similar: 1, l and I, etc.
+
+postalsafe()
+    Characters that are safe for use in postal addresses in the United States:
+    upper- and lower-case letters, digits, spaces, and the punctuation marks period,
+    hash (#), hyphen, and forward-slash.
+
+urlsafe()
+    Characters safe (unreserved) for use in URLs: letters, digits, hyphen, period, underscore,
+    and tilde.
+
+domainsafe()
+    Characters that are allowed for use in hostnames, and consequently, in internet domains: letters,
+    digits, and the hyphen.
+
+Xeger
+-----
+
+Inspired by the Java library of the same name, the ``xeger()`` method allows users to
+create a random string from a regular expression.
+
+For example to generate a postal code that fits the Canadian format:
+
+    >>> import rstr
+    >>> rstr.xeger(r'[A-Z]\d[A-Z] \d[A-Z]\d')
+    u'R6M 1W5'
+
+xeger works fine with most simple regular expressions, but it doesn't support all
+Python regular expression features.
+
+Custom Alphabets
+----------------
+
+If you have custom alphabets of characters that you would like to use with a method
+shortcut, you can specify them by keyword when instantiating an Rstr object:
+
+    >>> from rstr import Rstr
+    >>> rs = Rstr(vowels='AEIOU')
+    >>> rs.vowels()
+    'AEEUU'
+
+You can also add an alphabet to an existing instance with the add_alphabet() method:
+
+    >>> rs.add_alphabet('odds', '13579')
+    >>> rs.odds()
+    '339599519'
+
+Examples
+--------
+
+You can combine rstr with Python's built-in string formatting to produce strings
+that fit a variety of templates.
+
+An email address:
+
+::
+
+    '{0}@{1}.{2}'.format(rstr.nonwhitespace(exclude='@'),
+                         rstr.domainsafe(),
+                         rstr.letters(3))
+
+A URL:
+
+::
+
+    'http://{0}.{1}/{2}/?{3}'.format(rstr.domainsafe(),
+                                    rstr.letters(3),
+                                    rstr.urlsafe(),
+                                    rstr.urlsafe())
+
+A postal address:
+
+::
+
+    """{0} {1}
+    {2} {3}
+    {4}, {5} {6}
+    """.format(rstr.letters(4, 8).title(),
+               rstr.letters(4, 8).title(),
+               rstr.digits(3, 5),
+               rstr.letters(4, 10).title(),
+               rstr.letters(4, 15).title(),
+               rstr.uppercase(2),
+               rstr.digits(5),
+               )
+
+.. _SystemRandom: https://docs.python.org/3/library/random.html#random.SystemRandom
```

### Comparing `rstr-3.2.0/rstr/__init__.py` & `rstr-3.2.1/rstr/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from rstr.xeger import Xeger
-from rstr.rstr_base import SameCharacterError as SameCharacterError
+from rstr.rstr_base import SameCharacterError
 
 Rstr = Xeger
 _default_instance = Rstr()
 
 rstr = _default_instance.rstr
 xeger = _default_instance.xeger
```

### Comparing `rstr-3.2.0/rstr/rstr_base.py` & `rstr-3.2.1/rstr/rstr_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     'unambiguous': ''.join(set(string.ascii_letters + string.digits).difference('0O1lI')),
     'postalsafe': string.ascii_letters + string.digits + ' .-#/',
     'urlsafe': string.ascii_letters + string.digits + '-._~',
     'domainsafe': string.ascii_letters + string.digits + '-',
 }
 
 
-class RstrBase(object):
+class RstrBase():
     '''Create random strings from a variety of alphabets.
 
     The alphabets for printable(), uppercase(), lowercase(), digits(), and
     punctuation() are equivalent to the constants by those same names in the
     standard library string module.
 
     nondigits() uses an alphabet of string.letters + string.punctuation
@@ -121,15 +121,15 @@
 
     domainsafe() uses an alphabet of characters allowed in hostnames, and
     consequently, in internet domains: letters, digits, and the hyphen.
 
     '''
 
     def __init__(self, _random: '_Random', **custom_alphabets: str) -> None:
-        super(RstrBase, self).__init__()
+        super().__init__()
         self._random = _random
         self._alphabets = dict(ALPHABETS)
         for alpha_name, alphabet in custom_alphabets.items():
             self.add_alphabet(alpha_name, alphabet)
 
     def add_alphabet(self, alpha_name: str, characters: str) -> None:
         '''Add an additional alphabet to an Rstr instance and make it available
@@ -137,17 +137,16 @@
 
         '''
         self._alphabets[alpha_name] = characters
 
     def __getattr__(self, attr: str) -> '_PartialRstrFunc':
         if attr in self._alphabets:
             return partial(self.rstr, self._alphabets[attr])
-        else:
-            message = 'Rstr instance has no attribute: {0}'.format(attr)
-            raise AttributeError(message)
+        message = f'Rstr instance has no attribute: {attr}'
+        raise AttributeError(message)
 
     def sample_wr(self, population: Sequence[str], k: int) -> List[str]:
         '''Samples k random elements (with replacement) from a population'''
         return [self._random.choice(population) for i in itertools.repeat(None, k)]
 
     def rstr(
         self,
```

### Comparing `rstr-3.2.0/rstr/tests/test_rstr.py` & `rstr-3.2.1/tests/test_rstr.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import unittest
 import random
 
 from rstr import Rstr, SameCharacterError
 
 
 def assert_matches(pattern: str, value: str) -> None:
-    errmsg = '{} does not match {}'.format(value, pattern)
+    errmsg = f'{value} does not match {pattern}'
     assert re.match(pattern, value), errmsg
 
 
 class TestRstr(unittest.TestCase):
     def setUp(self) -> None:
         self.rs = Rstr()
```

### Comparing `rstr-3.2.0/rstr/tests/test_xeger.py` & `rstr-3.2.1/tests/test_xeger.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
     def test_dot(self) -> None:
         '''
         Verify that the dot character doesn't produce newlines.
         See: https://bitbucket.org/leapfrogdevelopment/rstr/issue/1/
         '''
         pattern = r'.+'
-        for i in range(100):
+        for _ in range(100):
             assert re.match(pattern, self.rs.xeger(pattern))
 
     def test_digit(self) -> None:
         pattern = r'\d'
         assert re.match(pattern, self.rs.xeger(pattern))
 
     def test_nondigits(self) -> None:
@@ -30,15 +30,15 @@
         assert re.match(pattern, self.rs.xeger(pattern))
 
     def test_literal_with_repeat(self) -> None:
         pattern = r'A{3}'
         assert re.match(pattern, self.rs.xeger(pattern))
 
     def test_literal_with_range_repeat(self) -> None:
-        pattern = r'A{2, 5}'
+        pattern = r'A{2,5}'
         assert re.match(pattern, self.rs.xeger(pattern))
 
     def test_word(self) -> None:
         pattern = r'\w'
         assert re.match(pattern, self.rs.xeger(pattern))
 
     def test_nonword(self) -> None:
```

### Comparing `rstr-3.2.0/rstr/xeger.py` & `rstr-3.2.1/rstr/xeger.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 import random
-import sre_parse
 import string
 from itertools import chain
 import typing
 from typing import Any, Callable, Dict, Mapping, Pattern, Sequence, Union
 
 from rstr.rstr_base import RstrBase
 
 if typing.TYPE_CHECKING:
     from rstr.rstr_base import _Random
 
+try:
+    import re._parser as sre_parse  # type: ignore[import]
+except ImportError:  # Python < 3.11
+    import sre_parse  # type: ignore[no-redef]
+
 
 # The * and + characters in a regular expression
 # match up to any number of repeats in theory,
 # (and actually 65535 repeats in python) but you
 # probably don't want that many repeats in your
 # generated strings. This sets an upper-bound on
 # repeats generated from + and * characters.
@@ -24,16 +28,16 @@
     '''Inspired by the Java library Xeger: http://code.google.com/p/xeger/
     This class adds functionality to Rstr allowing users to generate a
     semi-random string from a regular expression.'''
 
     def __init__(
         self, _random: '_Random' = typing.cast('_Random', random), **custom_alphabets: str,
     ) -> None:
-        super(Xeger, self).__init__(_random, **custom_alphabets)
-        self._cache: Dict[str, str] = dict()
+        super().__init__(_random, **custom_alphabets)
+        self._cache: Dict[str, str] = {}
         self._categories: Mapping[str, Callable[[], str]] = {
             'category_digit': lambda: self._alphabets['digits'],
             'category_not_digit': lambda: self._alphabets['nondigits'],
             'category_space': lambda: self._alphabets['whitespace'],
             'category_not_space': lambda: self._alphabets['nonwhitespace'],
             'category_word': lambda: self._alphabets['word'],
             'category_not_word': lambda: self._alphabets['nonword'],
```

