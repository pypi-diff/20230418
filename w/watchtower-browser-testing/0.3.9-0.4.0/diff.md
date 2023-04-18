# Comparing `tmp/watchtower_browser_testing-0.3.9.tar.gz` & `tmp/watchtower_browser_testing-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchtower_browser_testing-0.3.9.tar", last modified: Thu Apr 13 19:32:15 2023, max compression
+gzip compressed data, was "watchtower_browser_testing-0.4.0.tar", last modified: Tue Apr 18 07:09:16 2023, max compression
```

## Comparing `watchtower_browser_testing-0.3.9.tar` & `watchtower_browser_testing-0.4.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 19:32:15.220158 watchtower_browser_testing-0.3.9/
--rw-rw-rw-   0        0        0      310 2023-04-13 19:32:15.220158 watchtower_browser_testing-0.3.9/PKG-INFO
--rw-rw-rw-   0        0        0       28 2023-04-01 10:03:10.000000 watchtower_browser_testing-0.3.9/README.md
--rw-rw-rw-   0        0        0       42 2023-04-13 19:32:15.220158 watchtower_browser_testing-0.3.9/setup.cfg
--rw-rw-rw-   0        0        0     1106 2023-04-13 18:41:33.000000 watchtower_browser_testing-0.3.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:32:15.220158 watchtower_browser_testing-0.3.9/watchtower_browser_testing/
--rw-rw-rw-   0        0        0      148 2023-04-12 13:29:47.000000 watchtower_browser_testing-0.3.9/watchtower_browser_testing/__init__.py
--rw-rw-rw-   0        0        0      810 2023-04-13 18:26:41.000000 watchtower_browser_testing-0.3.9/watchtower_browser_testing/config.py
--rw-rw-rw-   0        0        0      116 2023-04-12 07:57:54.000000 watchtower_browser_testing-0.3.9/watchtower_browser_testing/exceptions.py
--rw-rw-rw-   0        0        0     1509 2023-04-13 18:16:09.000000 watchtower_browser_testing-0.3.9/watchtower_browser_testing/helpers.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:32:15.220158 watchtower_browser_testing-0.3.9/watchtower_browser_testing/templates/
--rw-rw-rw-   0        0        0     3255 2023-04-13 19:32:04.000000 watchtower_browser_testing-0.3.9/watchtower_browser_testing/templates/measurement_plan.html
--rw-rw-rw-   0        0        0    14236 2023-04-13 19:16:36.000000 watchtower_browser_testing-0.3.9/watchtower_browser_testing/testsuite.py
--rw-rw-rw-   0        0        0     7743 2023-04-12 06:31:40.000000 watchtower_browser_testing-0.3.9/watchtower_browser_testing/tracking_validation.py
--rw-rw-rw-   0        0        0       21 2023-04-13 19:32:04.000000 watchtower_browser_testing-0.3.9/watchtower_browser_testing/version.py
-drwxrwxrwx   0        0        0        0 2023-04-13 19:32:15.220158 watchtower_browser_testing-0.3.9/watchtower_browser_testing.egg-info/
--rw-rw-rw-   0        0        0      310 2023-04-13 19:32:15.000000 watchtower_browser_testing-0.3.9/watchtower_browser_testing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      609 2023-04-13 19:32:15.000000 watchtower_browser_testing-0.3.9/watchtower_browser_testing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 19:32:15.000000 watchtower_browser_testing-0.3.9/watchtower_browser_testing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-04-13 19:32:15.000000 watchtower_browser_testing-0.3.9/watchtower_browser_testing.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2023-04-13 19:32:15.000000 watchtower_browser_testing-0.3.9/watchtower_browser_testing.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 07:09:16.649080 watchtower_browser_testing-0.4.0/
+-rw-rw-rw-   0        0        0      310 2023-04-18 07:09:16.649080 watchtower_browser_testing-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0       28 2023-04-01 10:03:10.000000 watchtower_browser_testing-0.4.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-18 07:09:16.649080 watchtower_browser_testing-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1135 2023-04-17 17:34:58.000000 watchtower_browser_testing-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 07:09:16.631347 watchtower_browser_testing-0.4.0/watchtower_browser_testing/
+-rw-rw-rw-   0        0        0      148 2023-04-12 13:29:47.000000 watchtower_browser_testing-0.4.0/watchtower_browser_testing/__init__.py
+-rw-rw-rw-   0        0        0      945 2023-04-18 07:07:32.000000 watchtower_browser_testing-0.4.0/watchtower_browser_testing/config.py
+-rw-rw-rw-   0        0        0      116 2023-04-12 07:57:54.000000 watchtower_browser_testing-0.4.0/watchtower_browser_testing/exceptions.py
+-rw-rw-rw-   0        0        0     1509 2023-04-13 18:16:09.000000 watchtower_browser_testing-0.4.0/watchtower_browser_testing/helpers.py
+drwxrwxrwx   0        0        0        0 2023-04-18 07:09:16.649080 watchtower_browser_testing-0.4.0/watchtower_browser_testing/templates/
+-rw-rw-rw-   0        0        0     6148 2023-04-18 07:09:05.000000 watchtower_browser_testing-0.4.0/watchtower_browser_testing/templates/measurement_plan.html
+-rw-rw-rw-   0        0        0    16875 2023-04-17 17:56:52.000000 watchtower_browser_testing-0.4.0/watchtower_browser_testing/testsuite.py
+-rw-rw-rw-   0        0        0     7743 2023-04-17 17:27:01.000000 watchtower_browser_testing-0.4.0/watchtower_browser_testing/tracking_validation.py
+-rw-rw-rw-   0        0        0       21 2023-04-18 07:08:06.000000 watchtower_browser_testing-0.4.0/watchtower_browser_testing/version.py
+drwxrwxrwx   0        0        0        0 2023-04-18 07:09:16.649080 watchtower_browser_testing-0.4.0/watchtower_browser_testing.egg-info/
+-rw-rw-rw-   0        0        0      310 2023-04-18 07:09:16.000000 watchtower_browser_testing-0.4.0/watchtower_browser_testing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      609 2023-04-18 07:09:16.000000 watchtower_browser_testing-0.4.0/watchtower_browser_testing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 07:09:16.000000 watchtower_browser_testing-0.4.0/watchtower_browser_testing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-04-18 07:09:16.000000 watchtower_browser_testing-0.4.0/watchtower_browser_testing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-04-18 07:09:16.000000 watchtower_browser_testing-0.4.0/watchtower_browser_testing.egg-info/top_level.txt
```

### Comparing `watchtower_browser_testing-0.3.9/setup.py` & `watchtower_browser_testing-0.4.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -29,12 +29,14 @@
     package_data={'watchtower_browser_testing': ['templates/*.html']}
 )
 
 install_requires = [
     'playwright==1.32.1',
     'Cerberus',
     'marko',
-    'Jinja2'
+    'Jinja2',
+    'pytz',
+    'tzlocal'
 ]
 
 if __name__ == '__main__':
     setup(**setup_args, install_requires=install_requires)
```

### Comparing `watchtower_browser_testing-0.3.9/watchtower_browser_testing/helpers.py` & `watchtower_browser_testing-0.4.0/watchtower_browser_testing/helpers.py`

 * *Files identical despite different names*

### Comparing `watchtower_browser_testing-0.3.9/watchtower_browser_testing/testsuite.py` & `watchtower_browser_testing-0.4.0/watchtower_browser_testing/testsuite.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,18 +3,21 @@
 import glob
 import importlib.util
 import inspect
 import sys
 import types
 import functools
 import json
+import datetime
 
 from playwright.sync_api import sync_playwright
 from marko.ext.gfm import gfm as markdown
 import jinja2
+import pytz
+import tzlocal
 
 from watchtower_browser_testing.tracking_validation import EventQueue, RequestValidator, Validator
 from watchtower_browser_testing import exceptions
 from watchtower_browser_testing import config
 from watchtower_browser_testing import helpers
 
 
@@ -50,40 +53,63 @@
 
 
 class TestResult(object):
 
     def __init__(self,
                  test_name,
                  browser,
+                 measurement_plan=None,
                  scenario=None,
                  event=None,
                  ok=True,
                  errors=None,
                  data=None):
 
         self.test_name = test_name
+        self.measurement_plan = measurement_plan
         self.scenario = scenario
         self.event = event
         self.browser = browser
         self.ok = ok
         self.errors = errors
         self.data = data
 
+    @property
+    def css_id(self):
+
+        return 'e_' + '_'.join([str(x) for x in [
+            self.measurement_plan,
+            self.test_name,
+            self.scenario,
+            self.event
+        ]])
+
     def as_dict(self):
 
         return {
+            'measurement_plan': self.measurement_plan,
             'name': self.test_name,
             'scenario': self.scenario,
             'event': self.event,
             'browser': self.browser,
             'ok': self.ok,
             'errors': self.errors,
             'data': self.data
         }
 
+    def test_report_data(self):
+
+        return {
+            'ok': self.ok,
+            'browser': self.browser,
+            'errors': self.errors,
+            'data': self.data,
+            'css_id': self.css_id
+        }
+
 def new_page_from_gtm(self, ta_page, *args, **kwargs):
 
     with ta_page.expect_popup() as page_info:
         ta_page.get_by_role("button", name="Reopen").click()
     return page_info.value
 
 
@@ -152,14 +178,15 @@
         self.page.on('request', self.event_queue.register)
 
     def run(self,
             browser=None,
             headless=False,
             gtm_web_preview_link=None,
             tag_assistant_path=None,
+            measurement_plan=None,
             report_data=None):
 
         if browser is None:
             browsers = self.browsers
         else:
             browsers = [browser]
 
@@ -189,36 +216,40 @@
 
                     for event, setup in validation_setup.items():
 
                         validator = RequestValidator(**setup)
                         validator.select(self.event_queue.requests)
 
                         if validator.is_valid():
-                            self.result(browser=browser, scenario=scenario, event=event, ok=True,
+                            self.result(browser=browser, measurement_plan=measurement_plan, scenario=scenario,
+                                        event=event, ok=True,
                                         data={'n_matched_requests': validator.n_matched_requests, **report_data})
                         else:
-                            self.result(browser=browser, scenario=scenario, event=event, ok=False,
+                            self.result(browser=browser, measurement_plan=measurement_plan, scenario=scenario,
+                                        event=event, ok=False,
                                         errors=validator.errors,
                                         data={'n_matched_requests': validator.n_matched_requests, **report_data})
 
                     self.afterEach()
 
                 self.tearDownInstance()
 
     def result(self,
                browser,
+               measurement_plan,
                scenario,
                event,
                ok,
                errors=None,
                data=None):
 
         self.results.append(
             TestResult(
                 test_name=self.name,
+                measurement_plan=measurement_plan,
                 scenario=scenario,
                 event=event,
                 browser=browser,
                 ok=ok,
                 errors=errors,
                 data=data)
         )
@@ -260,16 +291,29 @@
 
             for event_name, obj in val.items():
 
                 event_id = scenario_id + '_' + event_name
                 body_validator = obj['validators'].get('body')
                 if body_validator and isinstance(body_validator, Validator):
                     body_validator = body_validator.schema
-                json_string = json.dumps(dict(body_validator), indent=4, cls=helpers.ExtendedEncoder)
-                mdstring = config.VALIDATION_MD_STRING.format(event_name=event_name, json_string=json_string)
+                json_string_body = json.dumps(dict(body_validator or {}), indent=4, cls=helpers.ExtendedEncoder)
+
+                query_validator = obj['validators'].get('query_string')
+                if query_validator and isinstance(query_validator, Validator):
+                    query_validator = query_validator.schema
+                json_string_query = json.dumps(dict(query_validator or {}), indent=4, cls=helpers.ExtendedEncoder)
+
+                check_user_id = not 'check_user_id' in obj['validators'] or obj['validators']['check_user_id']
+                allow_multiple = obj.get('allow_multiple', False)
+
+                mdstring = config.VALIDATION_MD_STRING.format(event_name=event_name,
+                                                              allow_multiple=allow_multiple,
+                                                              check_user_id=check_user_id,
+                                                              json_string_query=json_string_query,
+                                                              json_string_body=json_string_body)
                 event_struct = {'name': event_name,
                                 'id': 'e_' + event_id,
                                 'type': 'event',
                                 'description': markdown.convert(mdstring)}
 
                 scenario_struct['children'].append(event_struct)
 
@@ -285,14 +329,15 @@
 
     def __init__(self,
                  test_modules=None,
                  test_directory=None):
 
         self.test_modules = self.test_modules or test_modules
         self.test_directory = self.test_directory or test_directory
+        self.test_results = None
 
     def get_tests(self):
 
         directory = self.test_directory or os.getcwd()
 
         mods = glob.glob(os.path.join(directory, '*.py'))
         test_modules = [os.path.basename(f)[:-3] for f in mods
@@ -362,18 +407,40 @@
 
             test_instance = test['class']()
             report_data = {'module': test['module']}
             test_instance.run(headless=headless,
                               browser=browser,
                               gtm_web_preview_link=gtm_web_preview_link,
                               tag_assistant_path=tag_assistant_path,
+                              measurement_plan=self.__class__.__name__,
                               report_data=report_data)
             results.extend(test_instance.results)
 
-        return results
+        self.test_results = results
+
+    def test_report_data(self,
+                         timezone=None):
+
+        if self.test_results is None:
+            raise exceptions.TestError('Run tests firsts')
+
+        if timezone is None:
+            timezone = tzlocal.get_localzone()
+        elif isinstance(timezone, str):
+            timezone = pytz.timezone(timezone)
+
+        time = pytz.utc.localize(datetime.datetime.utcnow()).astimezone(timezone)
+
+        n_errors = len([r for r in self.test_results if not r.ok])
+
+        return {
+            'time': time.strftime('%Y-%m-%d %H:%M:%S'),
+            'n_errors': n_errors,
+            'results': [result.test_report_data() for result in self.test_results]
+        }
 
     def md_description(self):
 
         tests = self.get_tests()
 
         name = self.__class__.__name__
         structure = {'name': name,
```

### Comparing `watchtower_browser_testing-0.3.9/watchtower_browser_testing/tracking_validation.py` & `watchtower_browser_testing-0.4.0/watchtower_browser_testing/tracking_validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,22 +185,22 @@
         self.errors = None
 
     def is_valid(self):
 
         self.errors = []
 
         if self.n_matched_requests == 0:
-            self.errors.append({'general': 'No matched requests found'})
+            self.errors.append({'details': 'No matched requests found'})
 
         for request in self.matched_requests:
             if not request.is_valid(validators=self.validators):
                 self.errors.append(request.errors)
 
         if not self.allow_multiple and self.n_matched_requests > 1:
-            self.errors.append({'general': 'multiple matching requests are not allowed'})
+            self.errors.append({'details': 'multiple matching requests are not allowed'})
 
         return len(self.errors) == 0
 
     @property
     def n_matched_requests(self):
         return len(self.matched_requests)
```

### Comparing `watchtower_browser_testing-0.3.9/watchtower_browser_testing.egg-info/SOURCES.txt` & `watchtower_browser_testing-0.4.0/watchtower_browser_testing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

