# Comparing `tmp/whois-format-0.1.0a6.tar.gz` & `tmp/whois-format-0.1.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whois-format-0.1.0a6.tar", last modified: Wed Mar 29 04:32:51 2023, max compression
+gzip compressed data, was "whois-format-0.1.0a7.tar", last modified: Tue Apr 18 05:55:28 2023, max compression
```

## Comparing `whois-format-0.1.0a6.tar` & `whois-format-0.1.0a7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 dspruell  (1000) dspruell  (1000)        0 2023-03-29 04:32:51.499665 whois-format-0.1.0a6/
--rw-r--r--   0 dspruell  (1000) dspruell  (1000)      729 2023-03-25 10:06:17.000000 whois-format-0.1.0a6/LICENSE
--rw-rw-r--   0 dspruell  (1000) dspruell  (1000)     3482 2023-03-29 04:32:51.499665 whois-format-0.1.0a6/PKG-INFO
--rw-rw-r--   0 dspruell  (1000) dspruell  (1000)     3126 2023-03-29 04:24:46.000000 whois-format-0.1.0a6/README.md
--rw-rw-r--   0 dspruell  (1000) dspruell  (1000)      561 2023-03-29 03:59:38.000000 whois-format-0.1.0a6/pyproject.toml
--rw-rw-r--   0 dspruell  (1000) dspruell  (1000)       38 2023-03-29 04:32:51.499665 whois-format-0.1.0a6/setup.cfg
-drwxrwxr-x   0 dspruell  (1000) dspruell  (1000)        0 2023-03-29 04:32:51.499665 whois-format-0.1.0a6/tests/
--rw-rw-r--   0 dspruell  (1000) dspruell  (1000)       92 2023-03-27 06:34:02.000000 whois-format-0.1.0a6/tests/test_nop.py
-drwxrwxr-x   0 dspruell  (1000) dspruell  (1000)        0 2023-03-29 04:32:51.499665 whois-format-0.1.0a6/whois_format.egg-info/
--rw-rw-r--   0 dspruell  (1000) dspruell  (1000)     3482 2023-03-29 04:32:51.000000 whois-format-0.1.0a6/whois_format.egg-info/PKG-INFO
--rw-rw-r--   0 dspruell  (1000) dspruell  (1000)      284 2023-03-29 04:32:51.000000 whois-format-0.1.0a6/whois_format.egg-info/SOURCES.txt
--rw-rw-r--   0 dspruell  (1000) dspruell  (1000)        1 2023-03-29 04:32:51.000000 whois-format-0.1.0a6/whois_format.egg-info/dependency_links.txt
--rw-rw-r--   0 dspruell  (1000) dspruell  (1000)       50 2023-03-29 04:32:51.000000 whois-format-0.1.0a6/whois_format.egg-info/entry_points.txt
--rw-rw-r--   0 dspruell  (1000) dspruell  (1000)       22 2023-03-29 04:32:51.000000 whois-format-0.1.0a6/whois_format.egg-info/requires.txt
--rw-rw-r--   0 dspruell  (1000) dspruell  (1000)       13 2023-03-29 04:32:51.000000 whois-format-0.1.0a6/whois_format.egg-info/top_level.txt
--rw-rw-r--   0 dspruell  (1000) dspruell  (1000)     2948 2023-03-29 04:01:49.000000 whois-format-0.1.0a6/whois_format.py
+drwxrwxr-x   0 dspruell  (1000) dspruell  (1000)        0 2023-04-18 05:55:28.648684 whois-format-0.1.0a7/
+-rw-r--r--   0 dspruell  (1000) dspruell  (1000)      729 2023-03-25 10:06:17.000000 whois-format-0.1.0a7/LICENSE
+-rw-rw-r--   0 dspruell  (1000) dspruell  (1000)     3482 2023-04-18 05:55:28.648684 whois-format-0.1.0a7/PKG-INFO
+-rw-rw-r--   0 dspruell  (1000) dspruell  (1000)     3126 2023-03-29 04:24:46.000000 whois-format-0.1.0a7/README.md
+-rw-rw-r--   0 dspruell  (1000) dspruell  (1000)      561 2023-04-18 05:55:09.000000 whois-format-0.1.0a7/pyproject.toml
+-rw-rw-r--   0 dspruell  (1000) dspruell  (1000)       38 2023-04-18 05:55:28.648684 whois-format-0.1.0a7/setup.cfg
+drwxrwxr-x   0 dspruell  (1000) dspruell  (1000)        0 2023-04-18 05:55:28.648684 whois-format-0.1.0a7/tests/
+-rw-rw-r--   0 dspruell  (1000) dspruell  (1000)       92 2023-03-27 06:34:02.000000 whois-format-0.1.0a7/tests/test_nop.py
+drwxrwxr-x   0 dspruell  (1000) dspruell  (1000)        0 2023-04-18 05:55:28.648684 whois-format-0.1.0a7/whois_format.egg-info/
+-rw-rw-r--   0 dspruell  (1000) dspruell  (1000)     3482 2023-04-18 05:55:28.000000 whois-format-0.1.0a7/whois_format.egg-info/PKG-INFO
+-rw-rw-r--   0 dspruell  (1000) dspruell  (1000)      284 2023-04-18 05:55:28.000000 whois-format-0.1.0a7/whois_format.egg-info/SOURCES.txt
+-rw-rw-r--   0 dspruell  (1000) dspruell  (1000)        1 2023-04-18 05:55:28.000000 whois-format-0.1.0a7/whois_format.egg-info/dependency_links.txt
+-rw-rw-r--   0 dspruell  (1000) dspruell  (1000)       50 2023-04-18 05:55:28.000000 whois-format-0.1.0a7/whois_format.egg-info/entry_points.txt
+-rw-rw-r--   0 dspruell  (1000) dspruell  (1000)       22 2023-04-18 05:55:28.000000 whois-format-0.1.0a7/whois_format.egg-info/requires.txt
+-rw-rw-r--   0 dspruell  (1000) dspruell  (1000)       13 2023-04-18 05:55:28.000000 whois-format-0.1.0a7/whois_format.egg-info/top_level.txt
+-rw-rw-r--   0 dspruell  (1000) dspruell  (1000)     3640 2023-04-18 05:55:09.000000 whois-format-0.1.0a7/whois_format.py
```

### Comparing `whois-format-0.1.0a6/LICENSE` & `whois-format-0.1.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `whois-format-0.1.0a6/PKG-INFO` & `whois-format-0.1.0a7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whois-format
-Version: 0.1.0a6
+Version: 0.1.0a7
 Summary: Whois client wrapper producing a terse, single-line format.
 Author-email: Darren Spruell <phatbuckett@gmail.com>
 Project-URL: Homepage, https://github.com/dspruell/whois-format/
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `whois-format-0.1.0a6/README.md` & `whois-format-0.1.0a7/README.md`

 * *Files identical despite different names*

### Comparing `whois-format-0.1.0a6/pyproject.toml` & `whois-format-0.1.0a7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "whois-format"
-version = "0.1.0-alpha.6"
+version = "0.1.0-alpha.7"
 authors = [
     { name="Darren Spruell", email="phatbuckett@gmail.com" },
 ]
 description = "Whois client wrapper producing a terse, single-line format."
 readme = "README.md"
 dependencies = [
     "python-whois",
```

### Comparing `whois-format-0.1.0a6/whois_format.egg-info/PKG-INFO` & `whois-format-0.1.0a7/whois_format.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whois-format
-Version: 0.1.0a6
+Version: 0.1.0a7
 Summary: Whois client wrapper producing a terse, single-line format.
 Author-email: Darren Spruell <phatbuckett@gmail.com>
 Project-URL: Homepage, https://github.com/dspruell/whois-format/
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `whois-format-0.1.0a6/whois_format.py` & `whois-format-0.1.0a7/whois_format.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from whois import whois  # type: ignore
 
 
 __application_name__ = "whois-format"
 __version__ = pkg_resources.get_distribution(__application_name__).version
 __full_version__ = f"{__application_name__} {__version__}"
 
-logging.basicConfig(level=logging.DEBUG, format="[%(levelname)s] %(message)s")
+logging.basicConfig(level=logging.INFO, format="[%(levelname)s] %(message)s")
 
 DEFAULT_STR = "-"
 NUM_SLEEP_SECONDS = 15
 
 
 def get_ns_domains(nameservers: list) -> list:
     """Return parent domain(s) for list of DNS server FQDNs."""
@@ -41,38 +41,59 @@
         help=(
             "number of seconds to sleep for a pause between lookups of "
             "multiple domains (default: %(default)s)"
         ),
     )
     group = parser.add_mutually_exclusive_group(required=True)
     group.add_argument(
-        "-d", "--domain", nargs="+", help="domain name(s) to query"
+        "domain", nargs="*", default=[], help="domain name(s) to query"
     )
     group.add_argument(
-        "-f", "--in-file", type=FileType("r"), help="input file of domains"
+        "-f",
+        "--in-file",
+        type=FileType("r"),
+        help="input file of domains (`-` for standard input)",
     )
     group.add_argument(
         "-V",
         "--version",
         action="version",
         version=__full_version__,
         help="print package version",
     )
+    parser.add_argument(
+        "-d", "--debug", action="store_true", help="enable debug output"
+    )
     args = parser.parse_args()
 
+    if args.debug:
+        logging.getLogger().setLevel(logging.DEBUG)
+
     resp_data = []
 
     if args.in_file:
         lookup_domains = args.in_file.readlines()
     else:
         lookup_domains = args.domain
 
+    val = 0
     for domain in lookup_domains:
+        val += 1
         data = []
-        w = whois(domain.strip().lower())
+        domain = domain.strip().lower()
+        logging.debug("about to query for domain: %s", domain)
+        w = whois(domain)
+        logging.debug("completed query for domain: %s; result: %s", domain, w)
+        if w.domain_name is None:
+            logging.error(
+                "%s: received null response to lookup "
+                "(possible WHOIS library issue)",
+                domain,
+            )
+            continue
 
         # Field ordering matters - keep to this format:
         # domain, creation_date, registrar, nameservers, registrant name or
         # organization, registrant email(s)
 
         data.append(w.domain.upper())
         creation = w.get("creation_date")
@@ -90,10 +111,11 @@
         data.append(w.get("name") or w.get("org", DEFAULT_STR))
         emails = w.get("emails", [DEFAULT_STR])
         if not isinstance(emails, list):
             emails = [emails]
         data.append(", ".join(emails))
 
         resp_data.append(data)
-        sleep(args.sleep)
+        if val < len(lookup_domains):
+            sleep(args.sleep)
 
     print(tabulate(resp_data, tablefmt="plain"))
```

