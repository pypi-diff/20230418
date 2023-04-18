# Comparing `tmp/iocextract-1.8.0.tar.gz` & `tmp/iocextract-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/iocextract-1.8.0.tar", last modified: Wed Sep  5 20:15:53 2018, max compression
+gzip compressed data, was "dist/iocextract-1.9.0.tar", last modified: Thu Sep 20 21:10:52 2018, max compression
```

## Comparing `iocextract-1.8.0.tar` & `iocextract-1.9.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 trunk     (1000) trunk     (1001)        0 2018-09-05 20:15:53.000000 iocextract-1.8.0/
--rw-r--r--   0 trunk     (1000) trunk     (1001)    12750 2018-09-05 20:07:31.000000 iocextract-1.8.0/README.rst
--rw-r--r--   0 trunk     (1000) trunk     (1001)       35 2018-04-17 18:29:34.000000 iocextract-1.8.0/MANIFEST.in
--rw-r--r--   0 trunk     (1000) trunk     (1001)    15765 2018-09-05 20:15:53.000000 iocextract-1.8.0/PKG-INFO
--rw-r--r--   0 trunk     (1000) trunk     (1001)     1507 2018-04-17 18:03:06.000000 iocextract-1.8.0/LICENSE
--rw-r--r--   0 trunk     (1000) trunk     (1001)     1295 2018-09-05 20:09:20.000000 iocextract-1.8.0/setup.py
-drwxr-xr-x   0 trunk     (1000) trunk     (1001)        0 2018-09-05 20:15:53.000000 iocextract-1.8.0/iocextract.egg-info/
--rw-r--r--   0 trunk     (1000) trunk     (1001)    15765 2018-09-05 20:15:53.000000 iocextract-1.8.0/iocextract.egg-info/PKG-INFO
--rw-r--r--   0 trunk     (1000) trunk     (1001)        1 2018-09-05 20:15:53.000000 iocextract-1.8.0/iocextract.egg-info/dependency_links.txt
--rw-r--r--   0 trunk     (1000) trunk     (1001)       11 2018-09-05 20:15:53.000000 iocextract-1.8.0/iocextract.egg-info/top_level.txt
--rw-r--r--   0 trunk     (1000) trunk     (1001)       48 2018-09-05 20:15:53.000000 iocextract-1.8.0/iocextract.egg-info/entry_points.txt
--rw-r--r--   0 trunk     (1000) trunk     (1001)      259 2018-09-05 20:15:53.000000 iocextract-1.8.0/iocextract.egg-info/SOURCES.txt
--rw-r--r--   0 trunk     (1000) trunk     (1001)       44 2018-09-05 20:15:53.000000 iocextract-1.8.0/iocextract.egg-info/requires.txt
--rw-r--r--   0 trunk     (1000) trunk     (1001)    18763 2018-09-05 20:08:53.000000 iocextract-1.8.0/iocextract.py
--rw-r--r--   0 trunk     (1000) trunk     (1001)       38 2018-09-05 20:15:53.000000 iocextract-1.8.0/setup.cfg
+drwxr-xr-x   0 trunk     (1000) trunk     (1001)        0 2018-09-20 21:10:52.000000 iocextract-1.9.0/
+-rw-r--r--   0 trunk     (1000) trunk     (1001)    13967 2018-09-20 21:06:07.000000 iocextract-1.9.0/README.rst
+-rw-r--r--   0 trunk     (1000) trunk     (1001)       35 2018-04-17 18:29:34.000000 iocextract-1.9.0/MANIFEST.in
+-rw-r--r--   0 trunk     (1000) trunk     (1001)    17318 2018-09-20 21:10:52.000000 iocextract-1.9.0/PKG-INFO
+-rw-r--r--   0 trunk     (1000) trunk     (1001)     1507 2018-04-17 18:03:06.000000 iocextract-1.9.0/LICENSE
+-rw-r--r--   0 trunk     (1000) trunk     (1001)     1295 2018-09-20 21:00:25.000000 iocextract-1.9.0/setup.py
+drwxr-xr-x   0 trunk     (1000) trunk     (1001)        0 2018-09-20 21:10:52.000000 iocextract-1.9.0/iocextract.egg-info/
+-rw-r--r--   0 trunk     (1000) trunk     (1001)    17318 2018-09-20 21:10:52.000000 iocextract-1.9.0/iocextract.egg-info/PKG-INFO
+-rw-r--r--   0 trunk     (1000) trunk     (1001)        1 2018-09-20 21:10:52.000000 iocextract-1.9.0/iocextract.egg-info/dependency_links.txt
+-rw-r--r--   0 trunk     (1000) trunk     (1001)       11 2018-09-20 21:10:52.000000 iocextract-1.9.0/iocextract.egg-info/top_level.txt
+-rw-r--r--   0 trunk     (1000) trunk     (1001)       48 2018-09-20 21:10:52.000000 iocextract-1.9.0/iocextract.egg-info/entry_points.txt
+-rw-r--r--   0 trunk     (1000) trunk     (1001)      259 2018-09-20 21:10:52.000000 iocextract-1.9.0/iocextract.egg-info/SOURCES.txt
+-rw-r--r--   0 trunk     (1000) trunk     (1001)       44 2018-09-20 21:10:52.000000 iocextract-1.9.0/iocextract.egg-info/requires.txt
+-rw-r--r--   0 trunk     (1000) trunk     (1001)    20860 2018-09-20 20:46:15.000000 iocextract-1.9.0/iocextract.py
+-rw-r--r--   0 trunk     (1000) trunk     (1001)       38 2018-09-20 21:10:52.000000 iocextract-1.9.0/setup.cfg
```

### Comparing `iocextract-1.8.0/README.rst` & `iocextract-1.9.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -155,14 +155,18 @@
       -h, --help            show this help message and exit
       --input INPUT         default: stdin
       --output OUTPUT       default: stdout
       --extract-ips
       --extract-urls
       --extract-yara-rules
       --extract-hashes
+      --custom-regex REGEX_FILE
+                            file with custom regex strings, one per line, with one
+                            capture group each
+
       --refang              default: no
       --strip-urls          remove possible garbage from the end of urls. default:
                             no
       --wide                preprocess input to allow wide-encoded character
                             matches. default: no
 
 
@@ -187,14 +191,15 @@
     * Partially supported, anchoring on ``@``
 * YARA rules
 * Hashes
     * MD5
     * SHA1
     * SHA256
     * SHA512
+* Custom regex
 
 For IPv4 addresses, the following defang techniques are supported:
 
 .. container:: responsive-table
 
    +-----------------+---------------+-----------+
    | Technique       | Defanged      | Refanged  |
@@ -262,14 +267,50 @@
 
 Note that the table above is not exhaustive, and other URL/defang patterns may
 also be extracted correctly. If you notice something missing or not working
 correctly, feel free to let us know via the GitHub Issues_.
 
 The base64 regex was generated with `@deadpixi`_'s `base64 regex tool`_.
 
+Custom Regex
+------------
+
+If you'd like to use the CLI to extract IOCs using your own custom regex, create
+a plain text file with one regex string per line, and pass it in with the
+``--custom-regex`` flag. Be sure each regex string includes exactly one
+`capture group`_. For example:
+
+.. code-block:: text
+
+    http://(example\.com)/
+    (?:https|ftp)://(example\.com)/
+
+This custom regex file will exctract the domain ``example.com`` from matching
+URLs. The ``(?: )`` noncapture group won't be included in matches.
+
+If you would like to extract the entire match, just put parentheses around your
+entire regex string, like this:
+
+.. code-block:: text
+
+    (https?://.*?.com)
+
+If your regex is invalid, you'll see an error message like this:
+
+.. code-block:: text
+
+    Error in custom regex: missing ) at position 5
+
+If your regex does not include a capture group, you'll see an error message
+like this:
+
+.. code-block:: text
+
+    Error in custom regex: no such group
+
 Changelog
 ---------
 
 New features, improvements, and bugfixes for each release can be found in the
 `GitHub releases`_.
 
 Contributing
@@ -282,7 +323,8 @@
 .. _Issues: https://github.com/inquest/python-iocextract/issues
 .. _this tweet from @InQuest: https://twitter.com/InQuest/status/969469856931287041
 .. _Cisco ESA: https://www.cisco.com/c/en/us/support/docs/security/email-security-appliance/118775-technote-esa-00.html
 .. _GitHub releases: https://github.com/InQuest/python-iocextract/releases
 .. _appropriate wheel from PyPI: https://pypi.org/project/regex/#files
 .. _@deadpixi: https://github.com/deadpixi
 .. _base64 regex tool: http://www.erlang-factory.com/upload/presentations/225/ErlangFactorySFBay2010-RobKing.pdf
+.. _capture group: https://www.regular-expressions.info/brackets.html
```

### Comparing `iocextract-1.8.0/PKG-INFO` & `iocextract-1.9.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: iocextract
-Version: 1.8.0
+Version: 1.9.0
 Summary: Advanced Indicator of Compromise (IOC) extractor.
 Home-page: https://github.com/InQuest/python-iocextract
 Author: InQuest Labs
 Author-email: labs@inquest.net
 License: BSD
 Description-Content-Type: UNKNOWN
 Description: iocextract
@@ -164,14 +164,18 @@
               -h, --help            show this help message and exit
               --input INPUT         default: stdin
               --output OUTPUT       default: stdout
               --extract-ips
               --extract-urls
               --extract-yara-rules
               --extract-hashes
+              --custom-regex REGEX_FILE
+                                    file with custom regex strings, one per line, with one
+                                    capture group each
+        
               --refang              default: no
               --strip-urls          remove possible garbage from the end of urls. default:
                                     no
               --wide                preprocess input to allow wide-encoded character
                                     matches. default: no
         
         
@@ -196,14 +200,15 @@
             * Partially supported, anchoring on ``@``
         * YARA rules
         * Hashes
             * MD5
             * SHA1
             * SHA256
             * SHA512
+        * Custom regex
         
         For IPv4 addresses, the following defang techniques are supported:
         
         .. container:: responsive-table
         
            +-----------------+---------------+-----------+
            | Technique       | Defanged      | Refanged  |
@@ -271,14 +276,50 @@
         
         Note that the table above is not exhaustive, and other URL/defang patterns may
         also be extracted correctly. If you notice something missing or not working
         correctly, feel free to let us know via the GitHub Issues_.
         
         The base64 regex was generated with `@deadpixi`_'s `base64 regex tool`_.
         
+        Custom Regex
+        ------------
+        
+        If you'd like to use the CLI to extract IOCs using your own custom regex, create
+        a plain text file with one regex string per line, and pass it in with the
+        ``--custom-regex`` flag. Be sure each regex string includes exactly one
+        `capture group`_. For example:
+        
+        .. code-block:: text
+        
+            http://(example\.com)/
+            (?:https|ftp)://(example\.com)/
+        
+        This custom regex file will exctract the domain ``example.com`` from matching
+        URLs. The ``(?: )`` noncapture group won't be included in matches.
+        
+        If you would like to extract the entire match, just put parentheses around your
+        entire regex string, like this:
+        
+        .. code-block:: text
+        
+            (https?://.*?.com)
+        
+        If your regex is invalid, you'll see an error message like this:
+        
+        .. code-block:: text
+        
+            Error in custom regex: missing ) at position 5
+        
+        If your regex does not include a capture group, you'll see an error message
+        like this:
+        
+        .. code-block:: text
+        
+            Error in custom regex: no such group
+        
         Changelog
         ---------
         
         New features, improvements, and bugfixes for each release can be found in the
         `GitHub releases`_.
         
         Contributing
@@ -291,14 +332,15 @@
         .. _Issues: https://github.com/inquest/python-iocextract/issues
         .. _this tweet from @InQuest: https://twitter.com/InQuest/status/969469856931287041
         .. _Cisco ESA: https://www.cisco.com/c/en/us/support/docs/security/email-security-appliance/118775-technote-esa-00.html
         .. _GitHub releases: https://github.com/InQuest/python-iocextract/releases
         .. _appropriate wheel from PyPI: https://pypi.org/project/regex/#files
         .. _@deadpixi: https://github.com/deadpixi
         .. _base64 regex tool: http://www.erlang-factory.com/upload/presentations/225/ErlangFactorySFBay2010-RobKing.pdf
+        .. _capture group: https://www.regular-expressions.info/brackets.html
         
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `iocextract-1.8.0/LICENSE` & `iocextract-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iocextract-1.8.0/setup.py` & `iocextract-1.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 README = open(os.path.join(os.path.dirname(__file__), 'README.rst')).read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='iocextract',
-    version='1.8.0',
+    version='1.9.0',
     include_package_data=True,
     py_modules=[
         'iocextract',
     ],
     install_requires=[
         'regex',
     ],
```

### Comparing `iocextract-1.8.0/iocextract.egg-info/PKG-INFO` & `iocextract-1.9.0/iocextract.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: iocextract
-Version: 1.8.0
+Version: 1.9.0
 Summary: Advanced Indicator of Compromise (IOC) extractor.
 Home-page: https://github.com/InQuest/python-iocextract
 Author: InQuest Labs
 Author-email: labs@inquest.net
 License: BSD
 Description-Content-Type: UNKNOWN
 Description: iocextract
@@ -164,14 +164,18 @@
               -h, --help            show this help message and exit
               --input INPUT         default: stdin
               --output OUTPUT       default: stdout
               --extract-ips
               --extract-urls
               --extract-yara-rules
               --extract-hashes
+              --custom-regex REGEX_FILE
+                                    file with custom regex strings, one per line, with one
+                                    capture group each
+        
               --refang              default: no
               --strip-urls          remove possible garbage from the end of urls. default:
                                     no
               --wide                preprocess input to allow wide-encoded character
                                     matches. default: no
         
         
@@ -196,14 +200,15 @@
             * Partially supported, anchoring on ``@``
         * YARA rules
         * Hashes
             * MD5
             * SHA1
             * SHA256
             * SHA512
+        * Custom regex
         
         For IPv4 addresses, the following defang techniques are supported:
         
         .. container:: responsive-table
         
            +-----------------+---------------+-----------+
            | Technique       | Defanged      | Refanged  |
@@ -271,14 +276,50 @@
         
         Note that the table above is not exhaustive, and other URL/defang patterns may
         also be extracted correctly. If you notice something missing or not working
         correctly, feel free to let us know via the GitHub Issues_.
         
         The base64 regex was generated with `@deadpixi`_'s `base64 regex tool`_.
         
+        Custom Regex
+        ------------
+        
+        If you'd like to use the CLI to extract IOCs using your own custom regex, create
+        a plain text file with one regex string per line, and pass it in with the
+        ``--custom-regex`` flag. Be sure each regex string includes exactly one
+        `capture group`_. For example:
+        
+        .. code-block:: text
+        
+            http://(example\.com)/
+            (?:https|ftp)://(example\.com)/
+        
+        This custom regex file will exctract the domain ``example.com`` from matching
+        URLs. The ``(?: )`` noncapture group won't be included in matches.
+        
+        If you would like to extract the entire match, just put parentheses around your
+        entire regex string, like this:
+        
+        .. code-block:: text
+        
+            (https?://.*?.com)
+        
+        If your regex is invalid, you'll see an error message like this:
+        
+        .. code-block:: text
+        
+            Error in custom regex: missing ) at position 5
+        
+        If your regex does not include a capture group, you'll see an error message
+        like this:
+        
+        .. code-block:: text
+        
+            Error in custom regex: no such group
+        
         Changelog
         ---------
         
         New features, improvements, and bugfixes for each release can be found in the
         `GitHub releases`_.
         
         Contributing
@@ -291,14 +332,15 @@
         .. _Issues: https://github.com/inquest/python-iocextract/issues
         .. _this tweet from @InQuest: https://twitter.com/InQuest/status/969469856931287041
         .. _Cisco ESA: https://www.cisco.com/c/en/us/support/docs/security/email-security-appliance/118775-technote-esa-00.html
         .. _GitHub releases: https://github.com/InQuest/python-iocextract/releases
         .. _appropriate wheel from PyPI: https://pypi.org/project/regex/#files
         .. _@deadpixi: https://github.com/deadpixi
         .. _base64 regex tool: http://www.erlang-factory.com/upload/presentations/225/ErlangFactorySFBay2010-RobKing.pdf
+        .. _capture group: https://www.regular-expressions.info/brackets.html
         
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `iocextract-1.8.0/iocextract.py` & `iocextract-1.9.0/iocextract.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,28 +3,29 @@
 All methods return iterator objects, not lists. If for some reason you need
 a list, do e.g.: ``list(extract_iocs(my_data))``.
 
 Otherwise, you can iterate over the objects (e.g. in a ``for`` loop) normally.
 Each object yielded from the generators will by of type :class:`str`.
 """
 import io
-import regex as re
+import sys
 import itertools
 import argparse
 import binascii
 import base64
 try:
     # python3
     from urllib.parse import urlparse, unquote
     unicode = str
 except ImportError:
     from urlparse import urlparse
     from urllib import unquote
 
 import ipaddress
+import regex as re
 
 # Get basic url format, including a few obfuscation techniques, main anchor is the uri scheme.
 GENERIC_URL_RE = re.compile(r"""
         (
             [fhstu]\w\w?[px]s?
             (?::\/\/|__)
             [\x20\(\[]*
@@ -381,14 +382,58 @@
     :rtype: Iterator[:class:`str`]
     """
     yara_rules = re.sub(YARA_SPLIT_STR, "}\r\n\\1", data,
                         re.MULTILINE | re.DOTALL | re.VERBOSE)
     for yara_rule in YARA_PARSE_RE.finditer(yara_rules):
         yield yara_rule.group(1)
 
+def extract_custom_iocs(data, regex_list):
+    """Extract using custom regex strings.
+
+    Will always yield only the first *group* match from each regex.
+
+    Always use a single capture group! Do this::
+
+        [
+            r'(my regex)',  # This yields 'my regex' if the pattern matches.
+            r'my (re)gex',  # This yields 're' if the pattern matches.
+        ]
+
+    NOT this::
+
+        [
+            r'my regex',  # BAD! This doesn't yield anything.
+            r'(my) (re)gex',  # BAD! This yields 'my' if the pattern matches.
+        ]
+
+    For complicated regexes, you can combine capture and non-capture groups,
+    like this::
+
+        [
+            r'(?:my|your) (re)gex',  # This yields 're' if the pattern matches.
+        ]
+
+    Note the (?: ) syntax for noncapture groups vs the ( ) syntax for the capture
+    group.
+
+    :param data: Input text
+    :param regex_list: List of strings to treat as regex and match against data.
+    :rtype: Iterator[:class:`str`]
+    """
+
+    # Compile all the regex strings first, so we can error out quickly.
+    regex_objects = []
+    for regex_string in regex_list:
+        regex_objects.append(re.compile(regex_string))
+
+    # Iterate over regex objects, running each against input data.
+    for regex_object in regex_objects:
+        for ioc in regex_object.finditer(data):
+            yield ioc.group(1)
+
 def _is_ipv6_url(url):
     """URL network location is an IPv6 address, not a domain.
 
     :param url: String URL
     :rtype: bool
     """
     # fix urlparse exception
@@ -551,28 +596,32 @@
                         default=io.open(0, 'r', encoding='utf-8', errors='ignore'), help="default: stdin")
     parser.add_argument('--output', type=lambda x: io.open(x, 'w', encoding='utf-8', errors='ignore'),
                         default=io.open(1, 'w', encoding='utf-8', errors='ignore'), help="default: stdout")
     parser.add_argument('--extract-ips', action='store_true')
     parser.add_argument('--extract-urls', action='store_true')
     parser.add_argument('--extract-yara-rules', action='store_true')
     parser.add_argument('--extract-hashes', action='store_true')
+    parser.add_argument('--custom-regex', type=lambda x: io.open(x, 'r', encoding='utf-8', errors='ignore'),
+                        metavar='REGEX_FILE',
+                        help="file with custom regex strings, one per line, with one capture group each")
     parser.add_argument('--refang', action='store_true', help="default: no")
     parser.add_argument('--strip-urls', action='store_true',
                         help="remove possible garbage from the end of urls. default: no")
     parser.add_argument('--wide', action='store_true',
                         help="preprocess input to allow wide-encoded character matches. default: no")
     args = parser.parse_args()
 
     # Read input.
     data = args.input.read()
     if args.wide:
         data = data.replace('\x00', '')
 
     # By default, extract all.
-    if not (args.extract_ips or args.extract_urls or args.extract_yara_rules or args.extract_hashes):
+    if not (args.extract_ips or args.extract_urls or args.extract_yara_rules or args.extract_hashes or
+            args.custom_regex):
         for ioc in extract_iocs(data, refang=args.refang, strip=args.strip_urls):
             args.output.write(u"{ioc}\n".format(ioc=ioc))
     else:
         if args.extract_ips:
             for ioc in extract_ips(data, refang=args.refang):
                 args.output.write(u"{ioc}\n".format(ioc=ioc))
         if args.extract_urls:
@@ -581,9 +630,19 @@
         if args.extract_yara_rules:
             for ioc in extract_yara_rules(data):
                 args.output.write(u"{ioc}\n".format(ioc=ioc))
         if args.extract_hashes:
             for ioc in extract_hashes(data):
                 args.output.write(u"{ioc}\n".format(ioc=ioc))
 
+        # Custom regex file, one per line.
+        if args.custom_regex:
+            regex_list = [l.strip() for l in args.custom_regex.readlines()]
+
+            try:
+                for ioc in extract_custom_iocs(data, regex_list):
+                    args.output.write(u"{ioc}\n".format(ioc=ioc))
+            except (IndexError, re.error) as e:
+                sys.stderr.write('Error in custom regex: {e}\n'.format(e=e))
+
 if __name__ == "__main__":
     main()
```

