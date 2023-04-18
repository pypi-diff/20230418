# Comparing `tmp/rest_framework_redesign-0.1.3.tar.gz` & `tmp/rest_framework_redesign-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rest_framework_redesign-0.1.3.tar", max compression
+gzip compressed data, was "rest_framework_redesign-0.1.4.tar", max compression
```

## Comparing `rest_framework_redesign-0.1.3.tar` & `rest_framework_redesign-0.1.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1095 2023-04-17 08:21:25.010142 rest_framework_redesign-0.1.3/LICENSE
--rw-r--r--   0        0        0      570 2023-04-18 06:25:21.766020 rest_framework_redesign-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      874 2023-04-17 10:54:06.143589 rest_framework_redesign-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-04-17 08:27:28.035216 rest_framework_redesign-0.1.3/rest_framework_redesign/__init__.py
--rw-r--r--   0        0        0      111 2023-04-17 08:32:42.129922 rest_framework_redesign-0.1.3/rest_framework_redesign/admin.py
--rw-r--r--   0        0        0      248 2023-04-17 08:33:14.492981 rest_framework_redesign-0.1.3/rest_framework_redesign/apps.py
--rw-r--r--   0        0        0        0 2023-04-17 08:27:28.038933 rest_framework_redesign-0.1.3/rest_framework_redesign/migrations/__init__.py
--rw-r--r--   0        0        0       84 2023-04-17 08:33:33.145101 rest_framework_redesign-0.1.3/rest_framework_redesign/models.py
--rw-r--r--   0        0        0    22124 2023-04-18 07:53:29.559157 rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/api.html
--rw-r--r--   0        0        0      707 2023-04-15 12:47:58.113148 rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/filters/base.html
--rw-r--r--   0        0        0      714 2023-04-15 12:46:54.902747 rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/filters/ordering.html
--rw-r--r--   0        0        0      521 2023-04-16 12:17:54.556801 rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/filters/search.html
--rw-r--r--   0        0        0      835 2023-04-17 06:09:51.030141 rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/horizontal/checkbox.html
--rw-r--r--   0        0        0     1536 2023-04-17 06:10:08.352256 rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/horizontal/checkbox_multiple.html
--rw-r--r--   0        0        0      269 2023-04-16 10:47:42.246290 rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/horizontal/dict_field.html
--rw-r--r--   0        0        0      427 2023-04-16 10:49:02.575135 rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/horizontal/fieldset.html
--rw-r--r--   0        0        0      150 2023-04-16 10:49:14.840634 rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/horizontal/form.html
--rw-r--r--   0        0        0     1096 2023-04-17 06:10:16.889823 rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/horizontal/input.html
--rw-r--r--   0        0        0      262 2023-04-16 10:53:49.067743 rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/horizontal/list_field.html
--rw-r--r--   0        0        0      330 2023-04-16 10:54:36.132965 rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/horizontal/list_fieldset.html
--rw-r--r--   0        0        0     1448 2023-04-17 06:10:38.062218 rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/horizontal/radio.html
--rw-r--r--   0        0        0     1205 2023-04-17 06:11:00.824317 rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/horizontal/select.html
--rw-r--r--   0        0        0     1239 2023-04-17 06:12:33.906413 rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/horizontal/select_multiple.html
--rw-r--r--   0        0        0      813 2023-04-17 06:12:09.013201 rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/horizontal/textarea.html
--rw-r--r--   0        0        0     4252 2023-04-18 07:52:49.755306 rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/login.html
--rw-r--r--   0        0        0     1715 2023-04-16 10:26:12.389947 rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/pagination/numbers.html
--rw-r--r--   0        0        0      692 2023-04-16 10:31:24.701736 rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/pagination/previous_and_next.html
--rw-r--r--   0        0        0      307 2023-04-18 06:07:45.314176 rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/raw_data_form.html
--rw-r--r--   0        0        0       86 2023-04-17 08:33:49.776642 rest_framework_redesign-0.1.3/rest_framework_redesign/tests.py
--rw-r--r--   0        0        0       89 2023-04-17 08:34:08.004477 rest_framework_redesign-0.1.3/rest_framework_redesign/views.py
--rw-r--r--   0        0        0     1505 1970-01-01 00:00:00.000000 rest_framework_redesign-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1095 2023-04-17 08:21:25.010142 rest_framework_redesign-0.1.4/LICENSE
+-rw-r--r--   0        0        0      570 2023-04-18 08:05:33.167625 rest_framework_redesign-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      792 2023-04-18 08:20:43.087539 rest_framework_redesign-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-04-17 08:27:28.035216 rest_framework_redesign-0.1.4/rest_framework_redesign/__init__.py
+-rw-r--r--   0        0        0      111 2023-04-17 08:32:42.129922 rest_framework_redesign-0.1.4/rest_framework_redesign/admin.py
+-rw-r--r--   0        0        0      248 2023-04-17 08:33:14.492981 rest_framework_redesign-0.1.4/rest_framework_redesign/apps.py
+-rw-r--r--   0        0        0        0 2023-04-17 08:27:28.038933 rest_framework_redesign-0.1.4/rest_framework_redesign/migrations/__init__.py
+-rw-r--r--   0        0        0       84 2023-04-17 08:33:33.145101 rest_framework_redesign-0.1.4/rest_framework_redesign/models.py
+-rw-r--r--   0        0        0    22666 2023-04-18 08:18:28.669065 rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/api.html
+-rw-r--r--   0        0        0      707 2023-04-15 12:47:58.113148 rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/filters/base.html
+-rw-r--r--   0        0        0      714 2023-04-15 12:46:54.902747 rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/filters/ordering.html
+-rw-r--r--   0        0        0      521 2023-04-16 12:17:54.556801 rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/filters/search.html
+-rw-r--r--   0        0        0      835 2023-04-17 06:09:51.030141 rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/horizontal/checkbox.html
+-rw-r--r--   0        0        0     1536 2023-04-17 06:10:08.352256 rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/horizontal/checkbox_multiple.html
+-rw-r--r--   0        0        0      269 2023-04-16 10:47:42.246290 rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/horizontal/dict_field.html
+-rw-r--r--   0        0        0      427 2023-04-16 10:49:02.575135 rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/horizontal/fieldset.html
+-rw-r--r--   0        0        0      150 2023-04-16 10:49:14.840634 rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/horizontal/form.html
+-rw-r--r--   0        0        0     1096 2023-04-17 06:10:16.889823 rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/horizontal/input.html
+-rw-r--r--   0        0        0      262 2023-04-16 10:53:49.067743 rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/horizontal/list_field.html
+-rw-r--r--   0        0        0      330 2023-04-16 10:54:36.132965 rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/horizontal/list_fieldset.html
+-rw-r--r--   0        0        0     1448 2023-04-17 06:10:38.062218 rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/horizontal/radio.html
+-rw-r--r--   0        0        0     1205 2023-04-17 06:11:00.824317 rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/horizontal/select.html
+-rw-r--r--   0        0        0     1239 2023-04-17 06:12:33.906413 rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/horizontal/select_multiple.html
+-rw-r--r--   0        0        0      813 2023-04-17 06:12:09.013201 rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/horizontal/textarea.html
+-rw-r--r--   0        0        0     4375 2023-04-18 08:11:26.812363 rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/login.html
+-rw-r--r--   0        0        0     1715 2023-04-16 10:26:12.389947 rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/pagination/numbers.html
+-rw-r--r--   0        0        0      692 2023-04-16 10:31:24.701736 rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/pagination/previous_and_next.html
+-rw-r--r--   0        0        0      307 2023-04-18 06:07:45.314176 rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/raw_data_form.html
+-rw-r--r--   0        0        0       86 2023-04-17 08:33:49.776642 rest_framework_redesign-0.1.4/rest_framework_redesign/tests.py
+-rw-r--r--   0        0        0       89 2023-04-17 08:34:08.004477 rest_framework_redesign-0.1.4/rest_framework_redesign/views.py
+-rw-r--r--   0        0        0     1420 1970-01-01 00:00:00.000000 rest_framework_redesign-0.1.4/PKG-INFO
```

### Comparing `rest_framework_redesign-0.1.3/LICENSE` & `rest_framework_redesign-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.3/pyproject.toml` & `rest_framework_redesign-0.1.4/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rest-framework-redesign"
-version = "0.1.3"
+version = "0.1.4"
 description = "Redesign of the browsable api of Django REST Framework"
 authors = ["Yousef Abu Shanab <josephyousef249@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "rest_framework_redesign"}]
 homepage = "https://github.com/youzarsiph/rest-framework-redesign/"
 repository = "https://github.com/youzarsiph/rest-framework-redesign/"
```

### Comparing `rest_framework_redesign-0.1.3/README.md` & `rest_framework_redesign-0.1.4/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -2,45 +2,48 @@
 
 Redesign of the browsable api of Django REST Framework
 
 ## Get started
 
 To get started with rest-framework-redesign:
 
-- Install the package:
+Install the package:
 
-  ```bash
-    pip install rest-framework-redesign
-  ```
+```bash
+pip install rest-framework-redesign
+```
 
-- Add `rest_framework_redesign` to `INSTALLED_APPS` setting, make sure that it's before `rest_framework`
+Add `rest_framework_redesign` to `INSTALLED_APPS` setting, make sure that it's before `rest_framework`
 
-  ```python
-    # settings.py
+```python
+# settings.py
 
-    INSTALLED_APPS = [
-        ...
-        'rest_framework_redesign',
-        'rest_framework',
-        ...
-    ]
-  ```
+INSTALLED_APPS = [
+    ...
+    'rest_framework_redesign',
+    'rest_framework',
+    ...
+]
+```
 
-- Include `rest_framework.urls` in your project URLConf
+Include `rest_framework.urls` in your project URLConf
 
-  ```python
-    # urls.py
+```python
+# urls.py
 
+...
+from django.urls import path, include
+
+urlpatterns = [
+    ...
+    path('auth/', include('rest_framework.urls')),
     ...
-    from django.urls import path, include
+]
+```
 
-    urlpatterns = [
-        ...
-        path('admin/', admin.site.urls),
-        path('auth/', include('rest_framework.urls')),
-        ...
-    ]
-  ```
+Run the server
 
-- Run the server
+```bash
+python manage.py runserver
+```
 
 I hope you that you find this useful.
```

### Comparing `rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/api.html` & `rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/api.html`

 * *Files 4% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 
   {% if code_style %}<style>{{ code_style }}</style>{% endif %}
 {% endblock %}
 
 
 {% block navbar %}
   <header class="fixed-top">
-    <div class="bg-danger pt-2">
-      <nav class="navbar navbar-expand-lg navbar-dark bg-dark shadow pb-3 {% block bootstrap_navbar_variant %}{% endblock %}"
+    <div class="bg-danger py-2 shadow">
+      <nav class="navbar navbar-expand-lg navbar-dark bg-dark {% block bootstrap_navbar_variant %}{% endblock %}"
         role="navigation" aria-label="{% translate 'navbar' %}">
         <div class="container">
           {% block branding %}
             <a class="navbar-brand" rel="nofollow" href="https://www.django-rest-framework.org/">
                 <strong>{% translate 'Django REST Framework' %}</strong>
             </a>
           {% endblock %}
@@ -38,15 +38,15 @@
           </button>
 
           <div class="collapse navbar-collapse" id="navbar">
             <ul class="navbar-nav me-auto">
               <li class="nav-item">
                 <a href="https://www.django-rest-framework.org/" class="nav-link">
                   <strong class="d-flex align-items-center gap-3">
-                    <i class="bi house-fill"></i>
+                    <i class="bi bi-house-fill"></i>
                     {% translate "Home" %}
                   </strong>
                 </a>
               </li>
               <li class="nav-item">
                 <a href="https://www.django-rest-framework.org/tutorial/quickstart/" class="nav-link">
                   <strong class="d-flex align-items-center gap-3">
@@ -147,19 +147,20 @@
         {% if 'GET' in allowed_methods %}
           <form id="get-form">
             <fieldset>
               {% if api_settings.URL_FORMAT_OVERRIDE %}
                 <div class="btn-group w-100" role="group">
                   <a class="btn btn-lg btn-primary w-100" href="{{ request.get_full_path }}" rel="nofollow"
                     title="Make a GET request on the {{ name }} resource">
-                    <strong>
+                    <strong class="d-flex align-items-center justify-content-center gap-4">
+                      <i class="bi bi-arrow-clockwise"></i>
                       {% translate "GET" %}
                     </strong>
                   </a>
-                  <button class="btn btn-lg btn-outline-primary w-25 dropdown-toggle" type="button" id="dropdownMenuButtonSM"
+                  <button class="btn btn-lg btn-outline-primary dropdown-toggle" type="button" id="dropdownMenuButtonSM"
                     data-bs-toggle="dropdown" aria-expanded="false"></button>
                   <div class="dropdown">
                     <ul class="dropdown-menu dropdown-menu-end rounded-3 shadow" aria-labelledby="dropdownMenuButtonSM">
                       <li>
                         <h6 class="dropdown-header">
                           {% translate 'Select a format' %}
                         </h6>
@@ -175,38 +176,39 @@
                       {% endfor %}
                     </ul>
                   </div>
                 </div>
               {% else %}
                 <a class="btn btn-lg btn-primary" href="{{ request.get_full_path }}" rel="nofollow"
                   title="Make a GET request on the {{ name }} resource">
-                  <strong>
+                  <strong class="d-flex align-items-center justify-content-center gap-4">
+                    <i class="bi bi-arrow-clockwise"></i>
                     {% translate "GET" %}
                   </strong>
                 </a>
               {% endif %}
             </fieldset>
           </form>
         {% endif %}
 
         {% if options_form %}
           <form class="button-form" action="{{ request.get_full_path }}" data-method="OPTIONS">
             <button type="submit" class="btn btn-lg btn-secondary w-100" title="Make an OPTIONS request on the {{ name }} resource">
-              <strong class="d-flex align-items-center gap-3">
+              <strong class="d-flex align-items-center justify-content-center gap-3">
                 <i class="bi bi-info-square"></i>
                 {% translate "OPTIONS" %}
               </strong>
             </button>
           </form>
         {% endif %}
 
         {% if delete_form %}
           <button type="button" class="btn btn-lg btn-danger w-100" data-bs-toggle="modal" data-bs-target="#deleteModal"
             title="Make a DELETE request on the {{ name }} resource">
-            <strong class="d-flex align-items-center gap-3">
+            <strong class="d-flex align-items-center justify-content-center gap-3">
               <i class="bi bi-trash"></i>
               {% translate "DELETE" %}
             </strong>
           </button>
 
           <div class="modal fade" id="deleteModal" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
             <div class="modal-dialog">
@@ -241,15 +243,15 @@
           </div>
         {% endif %}
 
         {% if extra_actions %}
           <div class="dropdown" style="float: right; margin-right: 10px">
             <button class="btn btn-lg btn-info w-100" id="extra-actions-menu" data-bs-toggle="dropdown" aria-haspopup="true"
               aria-expanded="true">
-              <strong class="d-flex align-items-center gap-3">
+              <strong class="d-flex align-items-center justify-content-center gap-3">
                 <i class="bi bi-three-dots"></i>
                 {% translate "Extra Actions" %}
               </strong>
             </button>
             <ul class="dropdown-menu" aria-labelledby="extra-actions-menu">
               {% for action_name, url in extra_actions|items %}
                 <li>
@@ -260,15 +262,15 @@
               {% endfor %}
             </ul>
           </div>
         {% endif %}
 
         {% if filter_form %}
           <button data-bs-toggle="modal" data-bs-target="#filtersModal" class="btn btn-lg btn-success">
-            <strong class="d-flex align-items-center gap-3">
+            <strong class="d-flex align-items-center justify-content-center gap-3">
               <i class="bi bi-filter"></i>
               {% translate "Filters" %}
             </strong>
           </button>
         {% endif %}
       </section>
     {% endblock %}
@@ -277,39 +279,39 @@
       <section class="col-12 col-lg-8" role="main" aria-label="{% translate 'Main content' %}">
         <div class="card card-body rounded-3">
           <div class="request-info" aria-label="{% translate 'Request info' %}">
             <pre class="prettyprint"><b>{{ request.method }}</b> {{ request.get_full_path }}</pre>
           </div>
 
           <div class="response-info" aria-label="{% translate 'response info' %}">
-            <pre class="prettyprint"><div class="language-http bg-light rounded-4 mb-4"><div><strong>HTTP {{ response.status_code }} {{ response.status_text }}</strong></div>{% for key, val in response_headers|items %}<div><strong>{{ key }}:</strong> <span class="lit">{{ val|break_long_headers|urlize }}</span></div>{% endfor %}</div><code class="language-json bg-light rounded-4">{{ content|urlize }}</code></pre>
+            <pre class="prettyprint"><div class="language-http bg-light rounded-4 mb-4 p-3"><div><strong>HTTP {{ response.status_code }} {{ response.status_text }}</strong></div>{% for key, val in response_headers|items %}<div><strong>{{ key }}:</strong> <span class="lit">{{ val|break_long_headers|urlize }}</span></div>{% endfor %}</div><code class="language-json bg-light rounded-4">{{ content|urlize }}</code></pre>
           </div>
         </div>
       </section>
 
       <section class="col-12 col-lg-4">
         {% if display_edit_forms %}
           {% if post_form or raw_data_post_form %}
             <div {% if post_form %}class="card card-body rounded-3" {% endif %}>
               {% if post_form %}
                 <ul class="nav nav-pills nav-fill gap-2 p-1 small bg-dark rounded-5 shadow mb-4" role="tablist"
                   style="--bs-nav-link-color: var(--bs-danger); --bs-nav-pills-link-active-color: var(--bs-white); --bs-nav-pills-link-active-bg: var(--bs-danger);">
                   <li class="nav-item" role="presentation">
                     <button class="nav-link active rounded-5" id="form-tab" data-bs-toggle="tab" data-bs-target="#form"
                       type="button" role="tab" aria-controls="form" aria-selected="true">
-                      <strong class="d-flex align-items-center gap-3">
+                      <strong class="d-flex align-items-center justify-content-center gap-3">
                         <i class="bi bi-filetype-html"></i>
                         {% translate 'HTML form' %}
                       </strong>
                     </button>
                   </li>
                   <li class="nav-item" role="presentation">
                     <button class="nav-link rounded-5" id="raw-tab" data-bs-toggle="tab" data-bs-target="#raw"
                       type="button" role="tab" aria-controls="raw" aria-selected="false">
-                      <strong class="d-flex align-items-center gap-3">
+                      <strong class="d-flex align-items-center justify-content-center gap-3">
                         <i class="bi bi-filetype-json"></i>
                         {% translate 'Raw data' %}
                       </strong>
                     </button>
                   </li>
                 </ul>
               {% endif %}
@@ -321,15 +323,15 @@
                       <form action="{{ request.get_full_path }}" method="POST" enctype="multipart/form-data"
                         class="form-horizontal" novalidate>
                         <fieldset>
                           {% csrf_token %}
                           {{ post_form }}
                           <div class="form-actions">
                             <button class="btn btn-lg btn-primary w-100" title="Make a POST request on the {{ name }} resource">
-                              <strong class="d-flex align-items-center gap-3">
+                              <strong class="d-flex align-items-center justify-content-center gap-3">
                                 <i class="bi bi-send-fill"></i>
                                 {% translate "POST" %}
                               </strong>
                             </button>
                           </div>
                         </fieldset>
                       </form>
@@ -340,15 +342,15 @@
                 <div class="tab-pane" id="raw" role="tabpanel" aria-labelledby="raw-tab" tabindex="0">
                   {% with form=raw_data_post_form %}
                     <form action="{{ request.get_full_path }}" method="POST" class="form-horizontal">
                       <fieldset>
                         {% include "rest_framework/raw_data_form.html" %}
                         <div class="form-actions">
                           <button class="btn btn-lg btn-primary w-100" title="Make a POST request on the {{ name }} resource">
-                            <strong class="d-flex align-items-center gap-3">
+                            <strong class="d-flex align-items-center justify-content-center gap-3">
                               <i class="bi bi-send-fill"></i>
                               {% translate "POST" %}
                             </strong>
                           </button>
                         </div>
                       </fieldset>
                     </form>
@@ -362,24 +364,24 @@
             <div {% if put_form %}class="card card-body rounded-3"{% endif %}>
               {% if put_form %}
                 <ul class="nav nav-pills nav-fill gap-2 p-1 small bg-dark rounded-5 shadow mb-4" role="tablist"
                   style="--bs-nav-link-color: var(--bs-danger); --bs-nav-pills-link-active-color: var(--bs-white); --bs-nav-pills-link-active-bg: var(--bs-danger);">
                   <li class="nav-item" role="presentation">
                     <button class="nav-link active rounded-5" id="form-tab" data-bs-toggle="tab" data-bs-target="#put-object-form"
                       type="button" role="tab" aria-controls="form" aria-selected="true">
-                      <strong class="d-flex align-items-center gap-3">
+                      <strong class="d-flex align-items-center justify-content-center gap-3">
                         <i class="bi bi-filetype-html"></i>
                         {% translate 'HTML form' %}
                       </strong>
                     </button>
                   </li>
                   <li class="nav-item" role="presentation">
                     <button class="nav-link rounded-5" id="raw-tab" data-bs-toggle="tab" data-bs-target="#put-generic-content-form"
                       type="button" role="tab" aria-controls="raw" aria-selected="false">
-                      <strong class="d-flex align-items-center gap-3">
+                      <strong class="d-flex align-items-center justify-content-center gap-3">
                         <i class="bi bi-filetype-json"></i>
                         {% translate 'Raw data' %}
                       </strong>
                     </button>
                   </li>
                 </ul>
               {% endif %}
@@ -389,15 +391,15 @@
                   <div class="tab-pane active" id="put-object-form">
                     <form action="{{ request.get_full_path }}" data-method="PUT" enctype="multipart/form-data"
                       class="form-horizontal" novalidate>
                       <fieldset>
                         {{ put_form }}
                         <div class="form-actions">
                           <button class="btn btn-lg btn-primary w-100" title="Make a PUT request on the {{ name }} resource">
-                            <strong class="d-flex align-items-center gap-3">
+                            <strong class="d-flex align-items-center justify-content-center gap-3">
                               <i class="bi bi-send-fill"></i>
                               {% translate "PUT" %}
                             </strong>
                           </button>
                         </div>
                       </fieldset>
                     </form>
@@ -409,24 +411,24 @@
                     <form action="{{ request.get_full_path }}" data-method="PUT" class="form-horizontal">
                       <fieldset>
                         {% include "rest_framework/raw_data_form.html" %}
                         <div class="form-actions">
                           {% if raw_data_put_form %}
                             <button class="btn btn-lg btn-primary w-100"
                               title="Make a PUT request on the {{ name }} resource">
-                              <strong class="d-flex align-items-center gap-3">
+                              <strong class="d-flex align-items-center justify-content-center gap-3">
                                 <i class="bi bi-send-fill"></i>
                                 {% translate "PUT" %}
                               </strong>
                             </button>
                           {% endif %}
                           {% if raw_data_patch_form %}
                             <button data-method="PATCH" class="btn btn-lg btn-primary"
                               title="Make a PATCH request on the {{ name }} resource">
-                              <strong class="d-flex align-items-center gap-3">
+                              <strong class="d-flex align-items-center justify-content-center gap-3">
                                 <i class="bi bi-send-fill"></i>
                                 {% translate "PATCH" %}
                               </strong>
                             </button>
                           {% endif %}
                         </div>
                       </fieldset>
```

#### html2text {}

```diff
@@ -26,20 +26,23 @@
 {% endblock %} {% block content %}
  %}">
 ****** {{ name }} ******
 {% block description %} {{ description }} {% endblock %}
 {% if paginator %}  {% get_pagination_html paginator %}  {% endif %}  {% block
 request_forms %}  {% if 'GET' in allowed_methods %}
  {% if api_settings.URL_FORMAT_OVERRIDE %}
-{%_translate_"GET"_%}
+ {%_translate_"GET"_%}
+
     * * {% translate 'Select a format' %} *
     * {% for format in available_formats %}
     * {{_format_}}
     * {% endfor %}
-{% else %} {%_translate_"GET"_%} {% endif %}
+{% else %}
+ {%_translate_"GET"_%}
+ {% endif %}
 {% endif %} {% if options_form %}
 
  {% translate "OPTIONS" %}
 
 {% endif %} {% if delete_form %}
  {% translate "DELETE" %}
```

### Comparing `rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/filters/base.html` & `rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/filters/base.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/filters/ordering.html` & `rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/filters/ordering.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/filters/search.html` & `rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/filters/search.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/horizontal/checkbox.html` & `rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/horizontal/checkbox.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/horizontal/checkbox_multiple.html` & `rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/horizontal/checkbox_multiple.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/horizontal/input.html` & `rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/horizontal/input.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/horizontal/radio.html` & `rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/horizontal/radio.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/horizontal/select.html` & `rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/horizontal/select.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/horizontal/select_multiple.html` & `rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/horizontal/select_multiple.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/horizontal/textarea.html` & `rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/horizontal/textarea.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/login.html` & `rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/login.html`

 * *Files 2% similar despite different names*

```diff
@@ -15,69 +15,69 @@
   {% endblock %}
 
   {% if code_style %}<style>{{ code_style }}</style>{% endif %}
 {% endblock %}
 
 {% block body %}
   <body class="container">
-  <div style="height: 100vh" class="d-flex align-items-center justify-content-center">
-    <div class="col-12 col-md-6 col-lg-4">
-      <div class="card rounded-4 shadow">
-        <div class="card-header bg-danger rounded-top-4"></div>
-        <main class="card-body gap-4 p-5">
-          {% block branding %}
-            <h3 class="mb-4">
-              {% translate "Django REST framework" %}
-            </h3>
-          {% endblock %}
-
-          <form action="{% url 'rest_framework:login' %}" role="form" method="post">
-            {% csrf_token %}
-            <input type="hidden" name="next" value="{{ next }}" />
-
-            <div class="form-floating mb-4">
-              <input type="text" name="username" maxlength="150" class="form-control {% if form.username.errors %}is-invalid{% endif %}"
-                id="id_username" placeholder="Username" required autofocus {% if form.username.value %}value="{{ form.username.value }}"{% endif %}>
-              <label for="id_username">{{ form.username.label }}</label>
-              {% if form.username.errors %}
-                <small class="d-block text-muted" class="invalid-feedback">
-                  {{ form.username.errors|striptags }}
-                </small>
+    <div style="height: 100vh" class="d-flex align-items-center justify-content-center">
+      <div class="col-12 col-md-6 col-lg-4">
+        <div class="card rounded-4 shadow">
+          <div class="card-header bg-danger rounded-top-4"></div>
+          <main class="card-body gap-4 p-5">
+            {% block branding %}
+              <h3 class="mb-4">
+                {% translate "Django REST framework" %}
+              </h3>
+            {% endblock %}
+
+            <form action="{% url 'rest_framework:login' %}" role="form" method="post">
+              {% csrf_token %}
+              <input type="hidden" name="next" value="{{ next }}" />
+
+              <div class="form-floating mb-4">
+                <input type="text" name="username" maxlength="150" class="form-control {% if form.username.errors %}is-invalid{% endif %}"
+                  id="id_username" placeholder="Username" required autofocus {% if form.username.value %}value="{{ form.username.value }}"{% endif %}>
+                <label for="id_username">{{ form.username.label }}</label>
+                {% if form.username.errors %}
+                  <small class="d-block text-muted" class="invalid-feedback">
+                    {{ form.username.errors|striptags }}
+                  </small>
+                {% endif %}
+              </div>
+
+              <div class="form-floating mb-4">
+                <input type="password" name="password" maxlength="128" class="form-control  {% if form.username.errors %}is-invalid{% endif %}"
+                  id="id_password" required placeholder="Password">
+                <label for="id_password">{{ form.password.label }}</label>
+                {% if form.password.errors %}
+                  <small class="d-block text-muted" class="invalid-feedback">
+                    {{ form.password.errors|striptags }}
+                  </small>
+                {% endif %}
+              </div>
+
+              {% if form.non_field_errors %}
+                {% for error in form.non_field_errors %}
+                  <div class="alert alert-warning" role="alert">{{ error }}</div>
+                {% endfor %}
               {% endif %}
-            </div>
 
-            <div class="form-floating mb-4">
-              <input type="password" name="password" maxlength="128" class="form-control  {% if form.username.errors %}is-invalid{% endif %}"
-                id="id_password" required placeholder="Password">
-              <label for="id_password">{{ form.password.label }}</label>
-              {% if form.password.errors %}
-                <small class="d-block text-muted" class="invalid-feedback">
-                  {{ form.password.errors|striptags }}
-                </small>
-              {% endif %}
-            </div>
-
-            {% if form.non_field_errors %}
-              {% for error in form.non_field_errors %}
-                <div class="alert alert-warning" role="alert">{{ error }}</div>
-              {% endfor %}
-            {% endif %}
-
-            <button type="submit" class="btn btn-lg btn-primary w-100">
-              <strong class="d-flex align-items-center gap-3">
-                <i class="bi bi-box-arrow-in-right"></i>
-                {% translate "Login" %}
-              </strong>
-            </button>
-          </form>
-        </main>
-        <div class="card-footer bg-danger rounded-bottom-4"></div>
+              <button type="submit" class="btn btn-lg btn-primary w-100">
+                <strong class="d-flex align-items-center justify-content-center gap-3">
+                  <i class="bi bi-box-arrow-in-right"></i>
+                  {% translate "Login" %}
+                </strong>
+              </button>
+            </form>
+          </main>
+          <div class="card-footer bg-danger rounded-bottom-4"></div>
+        </div>
       </div>
     </div>
-  </div>
   </body>
 {% endblock %}
 
 
 {% block script %}
   <script>
     window.drf = {
```

### Comparing `rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/pagination/numbers.html` & `rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/pagination/numbers.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/pagination/previous_and_next.html` & `rest_framework_redesign-0.1.4/rest_framework_redesign/templates/rest_framework/pagination/previous_and_next.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.3/PKG-INFO` & `rest_framework_redesign-0.1.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rest-framework-redesign
-Version: 0.1.3
+Version: 0.1.4
 Summary: Redesign of the browsable api of Django REST Framework
 Home-page: https://github.com/youzarsiph/rest-framework-redesign/
 License: MIT
 Author: Yousef Abu Shanab
 Author-email: josephyousef249@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -19,46 +19,49 @@
 
 Redesign of the browsable api of Django REST Framework
 
 ## Get started
 
 To get started with rest-framework-redesign:
 
-- Install the package:
+Install the package:
 
-  ```bash
-    pip install rest-framework-redesign
-  ```
+```bash
+pip install rest-framework-redesign
+```
 
-- Add `rest_framework_redesign` to `INSTALLED_APPS` setting, make sure that it's before `rest_framework`
+Add `rest_framework_redesign` to `INSTALLED_APPS` setting, make sure that it's before `rest_framework`
 
-  ```python
-    # settings.py
+```python
+# settings.py
 
-    INSTALLED_APPS = [
-        ...
-        'rest_framework_redesign',
-        'rest_framework',
-        ...
-    ]
-  ```
+INSTALLED_APPS = [
+    ...
+    'rest_framework_redesign',
+    'rest_framework',
+    ...
+]
+```
 
-- Include `rest_framework.urls` in your project URLConf
+Include `rest_framework.urls` in your project URLConf
 
-  ```python
-    # urls.py
+```python
+# urls.py
 
+...
+from django.urls import path, include
+
+urlpatterns = [
+    ...
+    path('auth/', include('rest_framework.urls')),
     ...
-    from django.urls import path, include
+]
+```
 
-    urlpatterns = [
-        ...
-        path('admin/', admin.site.urls),
-        path('auth/', include('rest_framework.urls')),
-        ...
-    ]
-  ```
+Run the server
 
-- Run the server
+```bash
+python manage.py runserver
+```
 
 I hope you that you find this useful.
```

