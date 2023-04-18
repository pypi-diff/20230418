# Comparing `tmp/rest_framework_redesign-0.1.4.tar.gz` & `tmp/rest_framework_redesign-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rest_framework_redesign-0.1.4.tar", max compression
+gzip compressed data, was "rest_framework_redesign-0.1.5.tar", max compression
```

## Comparing `rest_framework_redesign-0.1.4.tar` & `rest_framework_redesign-0.1.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1095 2023-04-17 08:21:25.010142 rest_framework_redesign-0.1.4/LICENSE
--rw-r--r--   0        0        0      570 2023-04-18 08:05:33.167625 rest_framework_redesign-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      792 2023-04-18 08:20:43.087539 rest_framework_redesign-0.1.4/README.md
--rw-r--r--   0        0        0        0 2023-04-17 08:27:28.035216 rest_framework_redesign-0.1.4/rest_framework_redesign/__init__.py
--rw-r--r--   0        0        0      111 2023-04-17 08:32:42.129922 rest_framework_redesign-0.1.4/rest_framework_redesign/admin.py
--rw-r--r--   0        0        0      248 2023-04-17 08:33:14.492981 rest_framework_redesign-0.1.4/rest_framework_redesign/apps.py
--rw-r--r--   0        0        0        0 2023-04-17 08:27:28.038933 rest_framework_redesign-0.1.4/rest_framework_redesign/migrations/__init__.py
--rw-r--r--   0        0        0       84 2023-04-17 08:33:33.145101 rest_framework_redesign-0.1.4/rest_framework_redesign/models.py
--rw-r--r--   0        0        0    22666 2023-04-18 08:18:28.669065 rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/api.html
--rw-r--r--   0        0        0      707 2023-04-15 12:47:58.113148 rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/filters/base.html
--rw-r--r--   0        0        0      714 2023-04-15 12:46:54.902747 rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/filters/ordering.html
--rw-r--r--   0        0        0      521 2023-04-16 12:17:54.556801 rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/filters/search.html
--rw-r--r--   0        0        0      835 2023-04-17 06:09:51.030141 rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/horizontal/checkbox.html
--rw-r--r--   0        0        0     1536 2023-04-17 06:10:08.352256 rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/horizontal/checkbox_multiple.html
--rw-r--r--   0        0        0      269 2023-04-16 10:47:42.246290 rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/horizontal/dict_field.html
--rw-r--r--   0        0        0      427 2023-04-16 10:49:02.575135 rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/horizontal/fieldset.html
--rw-r--r--   0        0        0      150 2023-04-16 10:49:14.840634 rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/horizontal/form.html
--rw-r--r--   0        0        0     1096 2023-04-17 06:10:16.889823 rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/horizontal/input.html
--rw-r--r--   0        0        0      262 2023-04-16 10:53:49.067743 rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/horizontal/list_field.html
--rw-r--r--   0        0        0      330 2023-04-16 10:54:36.132965 rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/horizontal/list_fieldset.html
--rw-r--r--   0        0        0     1448 2023-04-17 06:10:38.062218 rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/horizontal/radio.html
--rw-r--r--   0        0        0     1205 2023-04-17 06:11:00.824317 rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/horizontal/select.html
--rw-r--r--   0        0        0     1239 2023-04-17 06:12:33.906413 rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/horizontal/select_multiple.html
--rw-r--r--   0        0        0      813 2023-04-17 06:12:09.013201 rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/horizontal/textarea.html
--rw-r--r--   0        0        0     4375 2023-04-18 08:11:26.812363 rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/login.html
--rw-r--r--   0        0        0     1715 2023-04-16 10:26:12.389947 rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/pagination/numbers.html
--rw-r--r--   0        0        0      692 2023-04-16 10:31:24.701736 rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/pagination/previous_and_next.html
--rw-r--r--   0        0        0      307 2023-04-18 06:07:45.314176 rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/raw_data_form.html
--rw-r--r--   0        0        0       86 2023-04-17 08:33:49.776642 rest_framework_redesign-0.1.4/rest_framework_redesign/tests.py
--rw-r--r--   0        0        0       89 2023-04-17 08:34:08.004477 rest_framework_redesign-0.1.4/rest_framework_redesign/views.py
--rw-r--r--   0        0        0     1420 1970-01-01 00:00:00.000000 rest_framework_redesign-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1095 2023-04-17 08:21:25.010142 rest_framework_redesign-0.1.5/LICENSE
+-rw-r--r--   0        0        0      570 2023-04-18 08:29:22.507759 rest_framework_redesign-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      792 2023-04-18 08:20:43.087539 rest_framework_redesign-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2023-04-17 08:27:28.035216 rest_framework_redesign-0.1.5/rest_framework_redesign/__init__.py
+-rw-r--r--   0        0        0      111 2023-04-17 08:32:42.129922 rest_framework_redesign-0.1.5/rest_framework_redesign/admin.py
+-rw-r--r--   0        0        0      248 2023-04-17 08:33:14.492981 rest_framework_redesign-0.1.5/rest_framework_redesign/apps.py
+-rw-r--r--   0        0        0        0 2023-04-17 08:27:28.038933 rest_framework_redesign-0.1.5/rest_framework_redesign/migrations/__init__.py
+-rw-r--r--   0        0        0       84 2023-04-17 08:33:33.145101 rest_framework_redesign-0.1.5/rest_framework_redesign/models.py
+-rw-r--r--   0        0        0    22948 2023-04-18 08:45:22.244712 rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/api.html
+-rw-r--r--   0        0        0      744 2023-04-18 08:53:35.615309 rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/filters/base.html
+-rw-r--r--   0        0        0      700 2023-04-18 08:50:06.523205 rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/filters/ordering.html
+-rw-r--r--   0        0        0      608 2023-04-18 08:49:46.702650 rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/filters/search.html
+-rw-r--r--   0        0        0      835 2023-04-17 06:09:51.030141 rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/horizontal/checkbox.html
+-rw-r--r--   0        0        0     1536 2023-04-17 06:10:08.352256 rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/horizontal/checkbox_multiple.html
+-rw-r--r--   0        0        0      269 2023-04-16 10:47:42.246290 rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/horizontal/dict_field.html
+-rw-r--r--   0        0        0      427 2023-04-16 10:49:02.575135 rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/horizontal/fieldset.html
+-rw-r--r--   0        0        0      150 2023-04-16 10:49:14.840634 rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/horizontal/form.html
+-rw-r--r--   0        0        0     1096 2023-04-17 06:10:16.889823 rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/horizontal/input.html
+-rw-r--r--   0        0        0      262 2023-04-16 10:53:49.067743 rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/horizontal/list_field.html
+-rw-r--r--   0        0        0      330 2023-04-16 10:54:36.132965 rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/horizontal/list_fieldset.html
+-rw-r--r--   0        0        0     1448 2023-04-17 06:10:38.062218 rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/horizontal/radio.html
+-rw-r--r--   0        0        0     1205 2023-04-17 06:11:00.824317 rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/horizontal/select.html
+-rw-r--r--   0        0        0     1239 2023-04-17 06:12:33.906413 rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/horizontal/select_multiple.html
+-rw-r--r--   0        0        0      813 2023-04-17 06:12:09.013201 rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/horizontal/textarea.html
+-rw-r--r--   0        0        0     4375 2023-04-18 08:11:26.812363 rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/login.html
+-rw-r--r--   0        0        0     1715 2023-04-16 10:26:12.389947 rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/pagination/numbers.html
+-rw-r--r--   0        0        0      692 2023-04-16 10:31:24.701736 rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/pagination/previous_and_next.html
+-rw-r--r--   0        0        0      307 2023-04-18 06:07:45.314176 rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/raw_data_form.html
+-rw-r--r--   0        0        0       86 2023-04-17 08:33:49.776642 rest_framework_redesign-0.1.5/rest_framework_redesign/tests.py
+-rw-r--r--   0        0        0       89 2023-04-17 08:34:08.004477 rest_framework_redesign-0.1.5/rest_framework_redesign/views.py
+-rw-r--r--   0        0        0     1420 1970-01-01 00:00:00.000000 rest_framework_redesign-0.1.5/PKG-INFO
```

### Comparing `rest_framework_redesign-0.1.4/LICENSE` & `rest_framework_redesign-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.4/pyproject.toml` & `rest_framework_redesign-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rest-framework-redesign"
-version = "0.1.4"
+version = "0.1.5"
 description = "Redesign of the browsable api of Django REST Framework"
 authors = ["Yousef Abu Shanab <josephyousef249@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "rest_framework_redesign"}]
 homepage = "https://github.com/youzarsiph/rest-framework-redesign/"
 repository = "https://github.com/youzarsiph/rest-framework-redesign/"
```

### Comparing `rest_framework_redesign-0.1.4/README.md` & `rest_framework_redesign-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/api.html` & `rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/api.html`

 * *Files 0% similar despite different names*

```diff
@@ -147,23 +147,23 @@
         {% if 'GET' in allowed_methods %}
           <form id="get-form">
             <fieldset>
               {% if api_settings.URL_FORMAT_OVERRIDE %}
                 <div class="btn-group w-100" role="group">
                   <a class="btn btn-lg btn-primary w-100" href="{{ request.get_full_path }}" rel="nofollow"
                     title="Make a GET request on the {{ name }} resource">
-                    <strong class="d-flex align-items-center justify-content-center gap-4">
+                    <strong class="d-flex align-items-center justify-content-center gap-3">
                       <i class="bi bi-arrow-clockwise"></i>
                       {% translate "GET" %}
                     </strong>
                   </a>
-                  <button class="btn btn-lg btn-outline-primary dropdown-toggle" type="button" id="dropdownMenuButtonSM"
+                  <button class="btn btn-lg btn-outline-primary dropdown-toggle" type="button" id="dropdownMenuButton"
                     data-bs-toggle="dropdown" aria-expanded="false"></button>
                   <div class="dropdown">
-                    <ul class="dropdown-menu dropdown-menu-end rounded-3 shadow" aria-labelledby="dropdownMenuButtonSM">
+                    <ul class="dropdown-menu dropdown-menu-end rounded-3 shadow" aria-labelledby="dropdownMenuButton">
                       <li>
                         <h6 class="dropdown-header">
                           {% translate 'Select a format' %}
                         </h6>
                       </li>
                       {% for format in available_formats %}
                       <li>
@@ -176,15 +176,15 @@
                       {% endfor %}
                     </ul>
                   </div>
                 </div>
               {% else %}
                 <a class="btn btn-lg btn-primary" href="{{ request.get_full_path }}" rel="nofollow"
                   title="Make a GET request on the {{ name }} resource">
-                  <strong class="d-flex align-items-center justify-content-center gap-4">
+                  <strong class="d-flex align-items-center justify-content-center gap-3">
                     <i class="bi bi-arrow-clockwise"></i>
                     {% translate "GET" %}
                   </strong>
                 </a>
               {% endif %}
             </fieldset>
           </form>
@@ -198,46 +198,50 @@
                 {% translate "OPTIONS" %}
               </strong>
             </button>
           </form>
         {% endif %}
 
         {% if delete_form %}
-          <button type="button" class="btn btn-lg btn-danger w-100" data-bs-toggle="modal" data-bs-target="#deleteModal"
-            title="Make a DELETE request on the {{ name }} resource">
-            <strong class="d-flex align-items-center justify-content-center gap-3">
-              <i class="bi bi-trash"></i>
-              {% translate "DELETE" %}
-            </strong>
-          </button>
+          <div>
+            <button type="button" class="btn btn-lg btn-danger w-100" data-bs-toggle="modal" data-bs-target="#deleteModal"
+              title="Make a DELETE request on the {{ name }} resource">
+              <strong class="d-flex align-items-center justify-content-center gap-3">
+                <i class="bi bi-trash"></i>
+                {% translate "DELETE" %}
+              </strong>
+            </button>
+          </div>
 
           <div class="modal fade" id="deleteModal" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
             <div class="modal-dialog">
-              <div class="modal-content p-3 rounded-3 shadow">
+              <div class="modal-content p-4 rounded-3 shadow">
                 <div class="modal-header border-bottom-0">
-                  <h5 class="modal-title" id="exampleModalLabel">
+                  <h3 class="modal-title" id="exampleModalLabel">
                     {% translate 'Delete' %} {{ name }}
-                  </h5>
+                  </h3>
                   <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                 </div>
                 <div class="modal-body">
-                  <p class="lead">
+                  <p class="lead mb-4">
                     {% translate "Are you sure you want to delete this" %} {{ name }}?
                   </p>
-                  <div class="d-flex align-items-center justify-content-end gap-4">
+                  <div class="d-grid gap-4">
                     <button type="button" class="btn btn-lg btn-outline-secondary" data-bs-dismiss="modal">
-                      <strong>
+                      <strong class="d-flex align-item-center justify-content-center gap-3">
+                        <i class="bi bi-close"></i>
                         {% translate "Cancel" %}
                       </strong>
                     </button>
                     <form class="button-form" action="{{ request.get_full_path }}" data-method="DELETE">
                       <button class="btn btn-lg btn-danger">
-                      <strong>
-                        {% translate "Delete" %}
-                      </strong>
+                        <strong class="d-flex align-item-center justify-content-center gap-3">
+                          <i class="bi bi-trash"></i>
+                          {% translate "Delete" %}
+                        </strong>
                       </button>
                     </form>
                   </div>
                 </div>
               </div>
             </div>
           </div>
@@ -279,15 +283,15 @@
       <section class="col-12 col-lg-8" role="main" aria-label="{% translate 'Main content' %}">
         <div class="card card-body rounded-3">
           <div class="request-info" aria-label="{% translate 'Request info' %}">
             <pre class="prettyprint"><b>{{ request.method }}</b> {{ request.get_full_path }}</pre>
           </div>
 
           <div class="response-info" aria-label="{% translate 'response info' %}">
-            <pre class="prettyprint"><div class="language-http bg-light rounded-4 mb-4 p-3"><div><strong>HTTP {{ response.status_code }} {{ response.status_text }}</strong></div>{% for key, val in response_headers|items %}<div><strong>{{ key }}:</strong> <span class="lit">{{ val|break_long_headers|urlize }}</span></div>{% endfor %}</div><code class="language-json bg-light rounded-4">{{ content|urlize }}</code></pre>
+            <pre class="prettyprint"><div class="language-http bg-light rounded-4 mb-4 p-3 overflow-auto"><div><strong>HTTP {{ response.status_code }} {{ response.status_text }}</strong></div>{% for key, val in response_headers|items %}<div><strong>{{ key }}:</strong> <span class="lit">{{ val|break_long_headers|urlize }}</span></div>{% endfor %}</div><code class="language-json bg-light rounded-4">{{ content|urlize }}</code></pre>
           </div>
         </div>
       </section>
 
       <section class="col-12 col-lg-4">
         {% if display_edit_forms %}
           {% if post_form or raw_data_post_form %}
@@ -418,15 +422,15 @@
                               <strong class="d-flex align-items-center justify-content-center gap-3">
                                 <i class="bi bi-send-fill"></i>
                                 {% translate "PUT" %}
                               </strong>
                             </button>
                           {% endif %}
                           {% if raw_data_patch_form %}
-                            <button data-method="PATCH" class="btn btn-lg btn-primary"
+                            <button data-method="PATCH" class="btn btn-lg btn-outline-primary w-100 mt-4"
                               title="Make a PATCH request on the {{ name }} resource">
                               <strong class="d-flex align-items-center justify-content-center gap-3">
                                 <i class="bi bi-send-fill"></i>
                                 {% translate "PATCH" %}
                               </strong>
                             </button>
                           {% endif %}
```

#### html2text {}

```diff
@@ -40,20 +40,25 @@
  {%_translate_"GET"_%}
  {% endif %}
 {% endif %} {% if options_form %}
 
  {% translate "OPTIONS" %}
 
 {% endif %} {% if delete_form %}
+
  {% translate "DELETE" %}
 
-** {% translate 'Delete' %} {{ name }} **
+**** {% translate 'Delete' %} {{ name }} ****
 {% translate "Are you sure you want to delete this" %} {{ name }}?
+
  {% translate "Cancel" %}
+
+
  {% translate "Delete" %}
+
 {% endif %} {% if extra_actions %}
 
  {% translate "Extra Actions" %}
 
     * {% for action_name, url in extra_actions|items %}
     * {{_action_name_}}
     * {% endfor %}
```

### Comparing `rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/filters/base.html` & `rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/filters/base.html`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+{% load i18n %}
+
 <div class="modal fade" id="filtersModal" tabindex="-1" aria-labelledby="filters" role="dialog" aria-hidden="true">
   <div class="modal-dialog">
-    <div class="modal-content p-3 rounded-3 shadow">
+    <div class="modal-content p-4 rounded-3 shadow">
       <div class="modal-header border-bottom-0">
-        <h1 class="modal-title" id="filters">
-          Filters
-        </h1>
+        <h3 class="modal-title" id="filters">
+          {% translate "Filters" %}
+        </h3>
         <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
       </div>
       <div class="modal-body">
         <div class="d-grid gap-4">
           {% for element in elements %}
             <div>
               {{ element }}
```

### Comparing `rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/filters/ordering.html` & `rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/filters/ordering.html`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-{% load rest_framework %}
-{% load i18n %}
-
-<h2>{% translate "Ordering" %}</h2>
+{% load i18n rest_framework %}
 
+<h5>{% translate "Ordering" %}</h5>
 <ul class="card card-body rounded-3 list-group">
   {% for key, label in options %}
     <li class="list-group-item border-0 px-4">
       <a href="{% add_query_param request param key %}" class="d-flex align-items-center text-decoration-none gap-3">
         <div class="form-check">
           {% if key == current %}
             <input type="radio" id="{{ key }}" checked class="form-check-input" name="order">
```

#### html2text {}

```diff
@@ -1,6 +1,6 @@
-{% load rest_framework %} {% load i18n %}
-***** {% translate "Ordering" %} *****
+{% load i18n rest_framework %}
+** {% translate "Ordering" %} **
     * {% for key, label in options %}
     * {%_if_key_==_current_%}_#_{%_else_%}_o_{%_endif_%}
       {{_label_}}
     * {% endfor %}
```

### Comparing `rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/filters/search.html` & `rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/filters/search.html`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 {% load i18n %}
-<h2>{% translate "Search" %}</h2>
 
+<h5>{% translate "Search" %}</h5>
 <form class="form-inline">
   <div class="form-group">
     <div class="input-group">
       <input
         type="search"
         class="form-control"
         name="{{ param }}"
         value="{{ term }}"
+        placeholder="{% translate "Type here to search..." %}"
       />
       <button class="btn btn-lg btn-outline-primary" type="submit">
-        <span class="glyphicon glyphicon-search" aria-hidden="true"></span>
-        <strong> {% translate "Search" %} </strong>
+        <strong class="d-flex align-items-center gap-3">
+          <i class="bi bi-search"></i>
+          {% translate "Search" %}
+        </strong>
       </button>
     </div>
   </div>
 </form>
```

### Comparing `rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/horizontal/checkbox.html` & `rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/horizontal/checkbox.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/horizontal/checkbox_multiple.html` & `rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/horizontal/checkbox_multiple.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/horizontal/input.html` & `rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/horizontal/input.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/horizontal/radio.html` & `rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/horizontal/radio.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/horizontal/select.html` & `rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/horizontal/select.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/horizontal/select_multiple.html` & `rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/horizontal/select_multiple.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/horizontal/textarea.html` & `rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/horizontal/textarea.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/login.html` & `rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/login.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/pagination/numbers.html` & `rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/pagination/numbers.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/pagination/previous_and_next.html` & `rest_framework_redesign-0.1.5/rest_framework_redesign/templates/rest_framework/pagination/previous_and_next.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.4/PKG-INFO` & `rest_framework_redesign-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rest-framework-redesign
-Version: 0.1.4
+Version: 0.1.5
 Summary: Redesign of the browsable api of Django REST Framework
 Home-page: https://github.com/youzarsiph/rest-framework-redesign/
 License: MIT
 Author: Yousef Abu Shanab
 Author-email: josephyousef249@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

