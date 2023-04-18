# Comparing `tmp/rest_framework_redesign-0.1.1.tar.gz` & `tmp/rest_framework_redesign-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rest_framework_redesign-0.1.1.tar", max compression
+gzip compressed data, was "rest_framework_redesign-0.1.2.tar", max compression
```

## Comparing `rest_framework_redesign-0.1.1.tar` & `rest_framework_redesign-0.1.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1095 2023-04-17 08:21:25.010142 rest_framework_redesign-0.1.1/LICENSE
--rw-r--r--   0        0        0      620 2023-04-17 10:46:17.091546 rest_framework_redesign-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      874 2023-04-17 10:54:06.143589 rest_framework_redesign-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-04-17 08:27:28.035216 rest_framework_redesign-0.1.1/rest_framework_redesign/__init__.py
--rw-r--r--   0        0        0      111 2023-04-17 08:32:42.129922 rest_framework_redesign-0.1.1/rest_framework_redesign/admin.py
--rw-r--r--   0        0        0      248 2023-04-17 08:33:14.492981 rest_framework_redesign-0.1.1/rest_framework_redesign/apps.py
--rw-r--r--   0        0        0        0 2023-04-17 08:27:28.038933 rest_framework_redesign-0.1.1/rest_framework_redesign/migrations/__init__.py
--rw-r--r--   0        0        0       84 2023-04-17 08:33:33.145101 rest_framework_redesign-0.1.1/rest_framework_redesign/models.py
--rw-r--r--   0        0        0    20074 2023-04-17 10:42:53.173824 rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/api.html
--rw-r--r--   0        0        0      707 2023-04-15 12:47:58.113148 rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/filters/base.html
--rw-r--r--   0        0        0      714 2023-04-15 12:46:54.902747 rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/filters/ordering.html
--rw-r--r--   0        0        0      521 2023-04-16 12:17:54.556801 rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/filters/search.html
--rw-r--r--   0        0        0      835 2023-04-17 06:09:51.030141 rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/horizontal/checkbox.html
--rw-r--r--   0        0        0     1536 2023-04-17 06:10:08.352256 rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/horizontal/checkbox_multiple.html
--rw-r--r--   0        0        0      269 2023-04-16 10:47:42.246290 rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/horizontal/dict_field.html
--rw-r--r--   0        0        0      427 2023-04-16 10:49:02.575135 rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/horizontal/fieldset.html
--rw-r--r--   0        0        0      150 2023-04-16 10:49:14.840634 rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/horizontal/form.html
--rw-r--r--   0        0        0     1096 2023-04-17 06:10:16.889823 rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/horizontal/input.html
--rw-r--r--   0        0        0      262 2023-04-16 10:53:49.067743 rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/horizontal/list_field.html
--rw-r--r--   0        0        0      330 2023-04-16 10:54:36.132965 rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/horizontal/list_fieldset.html
--rw-r--r--   0        0        0     1448 2023-04-17 06:10:38.062218 rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/horizontal/radio.html
--rw-r--r--   0        0        0     1205 2023-04-17 06:11:00.824317 rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/horizontal/select.html
--rw-r--r--   0        0        0     1239 2023-04-17 06:12:33.906413 rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/horizontal/select_multiple.html
--rw-r--r--   0        0        0      813 2023-04-17 06:12:09.013201 rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/horizontal/textarea.html
--rw-r--r--   0        0        0     4358 2023-04-17 06:11:41.318982 rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/login.html
--rw-r--r--   0        0        0     1715 2023-04-16 10:26:12.389947 rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/pagination/numbers.html
--rw-r--r--   0        0        0      692 2023-04-16 10:31:24.701736 rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/pagination/previous_and_next.html
--rw-r--r--   0        0        0      302 2023-04-17 10:44:35.187066 rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/raw_data_form.html
--rw-r--r--   0        0        0       86 2023-04-17 08:33:49.776642 rest_framework_redesign-0.1.1/rest_framework_redesign/tests.py
--rw-r--r--   0        0        0       89 2023-04-17 08:34:08.004477 rest_framework_redesign-0.1.1/rest_framework_redesign/views.py
--rw-r--r--   0        0        0     1593 1970-01-01 00:00:00.000000 rest_framework_redesign-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1095 2023-04-17 08:21:25.010142 rest_framework_redesign-0.1.2/LICENSE
+-rw-r--r--   0        0        0      570 2023-04-18 06:19:41.988888 rest_framework_redesign-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      874 2023-04-17 10:54:06.143589 rest_framework_redesign-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-04-17 08:27:28.035216 rest_framework_redesign-0.1.2/rest_framework_redesign/__init__.py
+-rw-r--r--   0        0        0      111 2023-04-17 08:32:42.129922 rest_framework_redesign-0.1.2/rest_framework_redesign/admin.py
+-rw-r--r--   0        0        0      248 2023-04-17 08:33:14.492981 rest_framework_redesign-0.1.2/rest_framework_redesign/apps.py
+-rw-r--r--   0        0        0        0 2023-04-17 08:27:28.038933 rest_framework_redesign-0.1.2/rest_framework_redesign/migrations/__init__.py
+-rw-r--r--   0        0        0       84 2023-04-17 08:33:33.145101 rest_framework_redesign-0.1.2/rest_framework_redesign/models.py
+-rw-r--r--   0        0        0    20019 2023-04-18 06:15:07.863341 rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/api.html
+-rw-r--r--   0        0        0      707 2023-04-15 12:47:58.113148 rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/filters/base.html
+-rw-r--r--   0        0        0      714 2023-04-15 12:46:54.902747 rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/filters/ordering.html
+-rw-r--r--   0        0        0      521 2023-04-16 12:17:54.556801 rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/filters/search.html
+-rw-r--r--   0        0        0      835 2023-04-17 06:09:51.030141 rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/horizontal/checkbox.html
+-rw-r--r--   0        0        0     1536 2023-04-17 06:10:08.352256 rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/horizontal/checkbox_multiple.html
+-rw-r--r--   0        0        0      269 2023-04-16 10:47:42.246290 rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/horizontal/dict_field.html
+-rw-r--r--   0        0        0      427 2023-04-16 10:49:02.575135 rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/horizontal/fieldset.html
+-rw-r--r--   0        0        0      150 2023-04-16 10:49:14.840634 rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/horizontal/form.html
+-rw-r--r--   0        0        0     1096 2023-04-17 06:10:16.889823 rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/horizontal/input.html
+-rw-r--r--   0        0        0      262 2023-04-16 10:53:49.067743 rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/horizontal/list_field.html
+-rw-r--r--   0        0        0      330 2023-04-16 10:54:36.132965 rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/horizontal/list_fieldset.html
+-rw-r--r--   0        0        0     1448 2023-04-17 06:10:38.062218 rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/horizontal/radio.html
+-rw-r--r--   0        0        0     1205 2023-04-17 06:11:00.824317 rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/horizontal/select.html
+-rw-r--r--   0        0        0     1239 2023-04-17 06:12:33.906413 rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/horizontal/select_multiple.html
+-rw-r--r--   0        0        0      813 2023-04-17 06:12:09.013201 rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/horizontal/textarea.html
+-rw-r--r--   0        0        0     4358 2023-04-17 06:11:41.318982 rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/login.html
+-rw-r--r--   0        0        0     1715 2023-04-16 10:26:12.389947 rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/pagination/numbers.html
+-rw-r--r--   0        0        0      692 2023-04-16 10:31:24.701736 rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/pagination/previous_and_next.html
+-rw-r--r--   0        0        0      307 2023-04-18 06:07:45.314176 rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/raw_data_form.html
+-rw-r--r--   0        0        0       86 2023-04-17 08:33:49.776642 rest_framework_redesign-0.1.2/rest_framework_redesign/tests.py
+-rw-r--r--   0        0        0       89 2023-04-17 08:34:08.004477 rest_framework_redesign-0.1.2/rest_framework_redesign/views.py
+-rw-r--r--   0        0        0     1505 1970-01-01 00:00:00.000000 rest_framework_redesign-0.1.2/PKG-INFO
```

### Comparing `rest_framework_redesign-0.1.1/LICENSE` & `rest_framework_redesign-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.1/pyproject.toml` & `rest_framework_redesign-0.1.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 [tool.poetry]
 name = "rest-framework-redesign"
-version = "0.1.1"
+version = "0.1.2"
 description = "Redesign of the browsable api of Django REST Framework"
 authors = ["Yousef Abu Shanab <josephyousef249@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "rest_framework_redesign"}]
 homepage = "https://github.com/youzarsiph/rest-framework-redesign/"
 repository = "https://github.com/youzarsiph/rest-framework-redesign/"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-Django = "^4.2"
-djangorestframework = "^3.14.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `rest_framework_redesign-0.1.1/README.md` & `rest_framework_redesign-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/api.html` & `rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/api.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 {% extends "rest_framework/base.html" %}
 
 {% load i18n static rest_framework %}
 
 {% block meta %}
-  <meta name="robots" content="NONE,NOARCHIVE" />
-  <meta http-equiv="Content-Type" content="text/html; charset=utf-8"/>
+  {{ block.super }}
   <meta name="viewport" content="width=device-width, initial-scale=1.0">
 {% endblock %}
 
 {% block style %}
   {% block bootstrap_theme %}
     <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha3/dist/css/bootstrap.min.css" rel="stylesheet"
       integrity="sha384-KK94CHFLLe+nY2dmCWGMq91rCGa5gtU4mk92HdvYe+M/SXH301p5ILy+dN9+nJOZ" crossorigin="anonymous">
@@ -133,25 +132,25 @@
 
     {% block request_forms %}
       <section class="d-grid d-md-flex align-items-lg-center justify-content-lg-end gap-4 mb-4" aria-label="{% translate 'Request form' %}">
         {% if 'GET' in allowed_methods %}
           <form id="get-form">
             <fieldset>
               {% if api_settings.URL_FORMAT_OVERRIDE %}
-                <div class="btn-group" role="group">
-                  <a class="btn btn-lg btn-primary" href="{{ request.get_full_path }}" rel="nofollow"
+                <div class="btn-group w-100" role="group">
+                  <a class="btn btn-lg btn-primary w-100" href="{{ request.get_full_path }}" rel="nofollow"
                     title="Make a GET request on the {{ name }} resource">
                     <strong>
                       {% translate "GET" %}
                     </strong>
                   </a>
-                  <button class="btn btn-lg btn-outline-primary dropdown-toggle" type="button" id="dropdownMenuButtonSM"
+                  <button class="btn btn-lg btn-outline-primary w-25 dropdown-toggle" type="button" id="dropdownMenuButtonSM"
                     data-bs-toggle="dropdown" aria-expanded="false"></button>
                   <div class="dropdown">
-                    <ul class="dropdown-menu rounded-3 shadow" aria-labelledby="dropdownMenuButtonSM">
+                    <ul class="dropdown-menu dropdown-menu-end rounded-3 shadow" aria-labelledby="dropdownMenuButtonSM">
                       <li>
                         <h6 class="dropdown-header">
                           {% translate 'Select a format' %}
                         </h6>
                       </li>
                       {% for format in available_formats %}
                       <li>
@@ -263,19 +262,15 @@
       <section class="col-12 col-lg-8" role="main" aria-label="{% translate 'main content' %}">
         <div class="card card-body rounded-3">
           <div class="request-info" style="clear: both" aria-label="{% translate 'request info' %}">
             <pre class="prettyprint"><b>{{ request.method }}</b> {{ request.get_full_path }}</pre>
           </div>
 
           <div class="response-info" aria-label="{% translate 'response info' %}">
-            <pre class="prettyprint">
-<div class="language-http bg-white"><strong>HTTP {{ response.status_code }} {{ response.status_text }}</strong>
-{% for key, val in response_headers|items %}<strong>{{ key }}:</strong> <span class="lit">{{ val|break_long_headers|urlize }}</span>
-{% endfor %}</div>
-<code class="language-json bg-light rounded-4">{{ content|urlize }}</code></pre>
+            <pre class="prettyprint"><div class="language-http bg-white"><strong>HTTP {{ response.status_code }} {{ response.status_text }}</strong><br>{% for key, val in response_headers|items %}<br><strong>{{ key }}:</strong> <span class="lit">{{ val|break_long_headers|urlize }}</span>{% endfor %}</div><code class="language-json bg-light rounded-4">{{ content|urlize }}</code></pre>
           </div>
         </div>
       </section>
 
       <section class="col-12 col-lg-4">
         {% if display_edit_forms %}
           {% if post_form or raw_data_post_form %}
@@ -326,15 +321,15 @@
 
                 <div class="tab-pane" id="raw" role="tabpanel" aria-labelledby="raw-tab" tabindex="0">
                   {% with form=raw_data_post_form %}
                     <form action="{{ request.get_full_path }}" method="POST" class="form-horizontal">
                       <fieldset>
                         {% include "rest_framework/raw_data_form.html" %}
                         <div class="form-actions">
-                          <button class="btn btn-lg btn-primary" title="Make a POST request on the {{ name }} resource">
+                          <button class="btn btn-lg btn-primary w-100" title="Make a POST request on the {{ name }} resource">
                             <strong>
                               {% translate "POST" %}
                             </strong>
                           </button>
                         </div>
                       </fieldset>
                     </form>
@@ -390,15 +385,15 @@
                 <div {% if put_form %}class="tab-pane"{% endif %} id="put-generic-content-form">
                   {% with form=raw_data_put_or_patch_form %}
                     <form action="{{ request.get_full_path }}" data-method="PUT" class="form-horizontal">
                       <fieldset>
                         {% include "rest_framework/raw_data_form.html" %}
                         <div class="form-actions">
                           {% if raw_data_put_form %}
-                          <button class="btn btn-lg btn-primary"
+                          <button class="btn btn-lg btn-primary w-100"
                             title="Make a PUT request on the {{ name }} resource">
                             <strong>
                               {% translate "PUT" %}
                             </strong>
                           </button>
                           {% endif %}
                           {% if raw_data_patch_form %}
```

#### html2text {}

```diff
@@ -1,11 +1,9 @@
 {% extends "rest_framework/base.html" %} {% load i18n static rest_framework %}
-{% block meta %}
-
-
+{% block meta %} {{ block.super }}
  {% endblock %} {% block style %} {% block bootstrap_theme %}
  {% endblock %} {% if code_style %}
 {% endif %} {% endblock %} {% block navbar %}
 {% block branding %} {%_translate_'Django_REST_Framework'_%} {% endblock %}
     * {%_translate_"Home"_%}
     * {%_translate_"Tutorial"_%}
     * {%_translate_"Github"_%}
@@ -46,18 +44,16 @@
     * {{_action_name_}}
     * {% endfor %}
 {% endif %} {% if filter_form %}  {% translate "Filters" %}  {% endif %}  {%
 endblock %}
  %}">
 {{ request.method }} {{ request.get_full_path }}
 HTTP {{ response.status_code }} {{ response.status_text }}
-{% for key, val in response_headers|items %}{{ key }}: {
-{ val|break_long_headers|urlize }}
-{% endfor %}
-
+{% for key, val in response_headers|items %}
+{{ key }}: {{ val|break_long_headers|urlize }}{% endfor %}
 {{ content|urlize }}
   {% if display_edit_forms %} {% if post_form or raw_data_post_form %}
 % if post_form %}class="card card-body rounded-3" {% endif %}> {% if post_form
 %}
     *  {% translate 'HTML form' %}
     *  {% translate 'Raw data' %}
 {% endif %}
```

### Comparing `rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/filters/base.html` & `rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/filters/base.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/filters/ordering.html` & `rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/filters/ordering.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/filters/search.html` & `rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/filters/search.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/horizontal/checkbox.html` & `rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/horizontal/checkbox.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/horizontal/checkbox_multiple.html` & `rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/horizontal/checkbox_multiple.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/horizontal/input.html` & `rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/horizontal/input.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/horizontal/radio.html` & `rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/horizontal/radio.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/horizontal/select.html` & `rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/horizontal/select.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/horizontal/select_multiple.html` & `rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/horizontal/select_multiple.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/horizontal/textarea.html` & `rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/horizontal/textarea.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/login.html` & `rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/login.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/pagination/numbers.html` & `rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/pagination/numbers.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.1/rest_framework_redesign/templates/rest_framework/pagination/previous_and_next.html` & `rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/pagination/previous_and_next.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.1/PKG-INFO` & `rest_framework_redesign-0.1.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
 Name: rest-framework-redesign
-Version: 0.1.1
+Version: 0.1.2
 Summary: Redesign of the browsable api of Django REST Framework
 Home-page: https://github.com/youzarsiph/rest-framework-redesign/
 License: MIT
 Author: Yousef Abu Shanab
 Author-email: josephyousef249@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: Django (>=4.2,<5.0)
-Requires-Dist: djangorestframework (>=3.14.0,<4.0.0)
 Project-URL: Repository, https://github.com/youzarsiph/rest-framework-redesign/
 Description-Content-Type: text/markdown
 
 # rest-framework-redesign
 
 Redesign of the browsable api of Django REST Framework
```

