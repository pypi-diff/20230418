# Comparing `tmp/rest_framework_redesign-0.1.2.tar.gz` & `tmp/rest_framework_redesign-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rest_framework_redesign-0.1.2.tar", max compression
+gzip compressed data, was "rest_framework_redesign-0.1.3.tar", max compression
```

## Comparing `rest_framework_redesign-0.1.2.tar` & `rest_framework_redesign-0.1.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1095 2023-04-17 08:21:25.010142 rest_framework_redesign-0.1.2/LICENSE
--rw-r--r--   0        0        0      570 2023-04-18 06:19:41.988888 rest_framework_redesign-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      874 2023-04-17 10:54:06.143589 rest_framework_redesign-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-04-17 08:27:28.035216 rest_framework_redesign-0.1.2/rest_framework_redesign/__init__.py
--rw-r--r--   0        0        0      111 2023-04-17 08:32:42.129922 rest_framework_redesign-0.1.2/rest_framework_redesign/admin.py
--rw-r--r--   0        0        0      248 2023-04-17 08:33:14.492981 rest_framework_redesign-0.1.2/rest_framework_redesign/apps.py
--rw-r--r--   0        0        0        0 2023-04-17 08:27:28.038933 rest_framework_redesign-0.1.2/rest_framework_redesign/migrations/__init__.py
--rw-r--r--   0        0        0       84 2023-04-17 08:33:33.145101 rest_framework_redesign-0.1.2/rest_framework_redesign/models.py
--rw-r--r--   0        0        0    20019 2023-04-18 06:15:07.863341 rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/api.html
--rw-r--r--   0        0        0      707 2023-04-15 12:47:58.113148 rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/filters/base.html
--rw-r--r--   0        0        0      714 2023-04-15 12:46:54.902747 rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/filters/ordering.html
--rw-r--r--   0        0        0      521 2023-04-16 12:17:54.556801 rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/filters/search.html
--rw-r--r--   0        0        0      835 2023-04-17 06:09:51.030141 rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/horizontal/checkbox.html
--rw-r--r--   0        0        0     1536 2023-04-17 06:10:08.352256 rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/horizontal/checkbox_multiple.html
--rw-r--r--   0        0        0      269 2023-04-16 10:47:42.246290 rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/horizontal/dict_field.html
--rw-r--r--   0        0        0      427 2023-04-16 10:49:02.575135 rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/horizontal/fieldset.html
--rw-r--r--   0        0        0      150 2023-04-16 10:49:14.840634 rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/horizontal/form.html
--rw-r--r--   0        0        0     1096 2023-04-17 06:10:16.889823 rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/horizontal/input.html
--rw-r--r--   0        0        0      262 2023-04-16 10:53:49.067743 rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/horizontal/list_field.html
--rw-r--r--   0        0        0      330 2023-04-16 10:54:36.132965 rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/horizontal/list_fieldset.html
--rw-r--r--   0        0        0     1448 2023-04-17 06:10:38.062218 rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/horizontal/radio.html
--rw-r--r--   0        0        0     1205 2023-04-17 06:11:00.824317 rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/horizontal/select.html
--rw-r--r--   0        0        0     1239 2023-04-17 06:12:33.906413 rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/horizontal/select_multiple.html
--rw-r--r--   0        0        0      813 2023-04-17 06:12:09.013201 rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/horizontal/textarea.html
--rw-r--r--   0        0        0     4358 2023-04-17 06:11:41.318982 rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/login.html
--rw-r--r--   0        0        0     1715 2023-04-16 10:26:12.389947 rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/pagination/numbers.html
--rw-r--r--   0        0        0      692 2023-04-16 10:31:24.701736 rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/pagination/previous_and_next.html
--rw-r--r--   0        0        0      307 2023-04-18 06:07:45.314176 rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/raw_data_form.html
--rw-r--r--   0        0        0       86 2023-04-17 08:33:49.776642 rest_framework_redesign-0.1.2/rest_framework_redesign/tests.py
--rw-r--r--   0        0        0       89 2023-04-17 08:34:08.004477 rest_framework_redesign-0.1.2/rest_framework_redesign/views.py
--rw-r--r--   0        0        0     1505 1970-01-01 00:00:00.000000 rest_framework_redesign-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1095 2023-04-17 08:21:25.010142 rest_framework_redesign-0.1.3/LICENSE
+-rw-r--r--   0        0        0      570 2023-04-18 06:25:21.766020 rest_framework_redesign-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      874 2023-04-17 10:54:06.143589 rest_framework_redesign-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-04-17 08:27:28.035216 rest_framework_redesign-0.1.3/rest_framework_redesign/__init__.py
+-rw-r--r--   0        0        0      111 2023-04-17 08:32:42.129922 rest_framework_redesign-0.1.3/rest_framework_redesign/admin.py
+-rw-r--r--   0        0        0      248 2023-04-17 08:33:14.492981 rest_framework_redesign-0.1.3/rest_framework_redesign/apps.py
+-rw-r--r--   0        0        0        0 2023-04-17 08:27:28.038933 rest_framework_redesign-0.1.3/rest_framework_redesign/migrations/__init__.py
+-rw-r--r--   0        0        0       84 2023-04-17 08:33:33.145101 rest_framework_redesign-0.1.3/rest_framework_redesign/models.py
+-rw-r--r--   0        0        0    22124 2023-04-18 07:53:29.559157 rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/api.html
+-rw-r--r--   0        0        0      707 2023-04-15 12:47:58.113148 rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/filters/base.html
+-rw-r--r--   0        0        0      714 2023-04-15 12:46:54.902747 rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/filters/ordering.html
+-rw-r--r--   0        0        0      521 2023-04-16 12:17:54.556801 rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/filters/search.html
+-rw-r--r--   0        0        0      835 2023-04-17 06:09:51.030141 rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/horizontal/checkbox.html
+-rw-r--r--   0        0        0     1536 2023-04-17 06:10:08.352256 rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/horizontal/checkbox_multiple.html
+-rw-r--r--   0        0        0      269 2023-04-16 10:47:42.246290 rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/horizontal/dict_field.html
+-rw-r--r--   0        0        0      427 2023-04-16 10:49:02.575135 rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/horizontal/fieldset.html
+-rw-r--r--   0        0        0      150 2023-04-16 10:49:14.840634 rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/horizontal/form.html
+-rw-r--r--   0        0        0     1096 2023-04-17 06:10:16.889823 rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/horizontal/input.html
+-rw-r--r--   0        0        0      262 2023-04-16 10:53:49.067743 rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/horizontal/list_field.html
+-rw-r--r--   0        0        0      330 2023-04-16 10:54:36.132965 rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/horizontal/list_fieldset.html
+-rw-r--r--   0        0        0     1448 2023-04-17 06:10:38.062218 rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/horizontal/radio.html
+-rw-r--r--   0        0        0     1205 2023-04-17 06:11:00.824317 rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/horizontal/select.html
+-rw-r--r--   0        0        0     1239 2023-04-17 06:12:33.906413 rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/horizontal/select_multiple.html
+-rw-r--r--   0        0        0      813 2023-04-17 06:12:09.013201 rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/horizontal/textarea.html
+-rw-r--r--   0        0        0     4252 2023-04-18 07:52:49.755306 rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/login.html
+-rw-r--r--   0        0        0     1715 2023-04-16 10:26:12.389947 rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/pagination/numbers.html
+-rw-r--r--   0        0        0      692 2023-04-16 10:31:24.701736 rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/pagination/previous_and_next.html
+-rw-r--r--   0        0        0      307 2023-04-18 06:07:45.314176 rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/raw_data_form.html
+-rw-r--r--   0        0        0       86 2023-04-17 08:33:49.776642 rest_framework_redesign-0.1.3/rest_framework_redesign/tests.py
+-rw-r--r--   0        0        0       89 2023-04-17 08:34:08.004477 rest_framework_redesign-0.1.3/rest_framework_redesign/views.py
+-rw-r--r--   0        0        0     1505 1970-01-01 00:00:00.000000 rest_framework_redesign-0.1.3/PKG-INFO
```

### Comparing `rest_framework_redesign-0.1.2/LICENSE` & `rest_framework_redesign-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.2/pyproject.toml` & `rest_framework_redesign-0.1.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rest-framework-redesign"
-version = "0.1.2"
+version = "0.1.3"
 description = "Redesign of the browsable api of Django REST Framework"
 authors = ["Yousef Abu Shanab <josephyousef249@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "rest_framework_redesign"}]
 homepage = "https://github.com/youzarsiph/rest-framework-redesign/"
 repository = "https://github.com/youzarsiph/rest-framework-redesign/"
```

### Comparing `rest_framework_redesign-0.1.2/README.md` & `rest_framework_redesign-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/api.html` & `rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/api.html`

 * *Files 18% similar despite different names*

```diff
@@ -7,14 +7,16 @@
   <meta name="viewport" content="width=device-width, initial-scale=1.0">
 {% endblock %}
 
 {% block style %}
   {% block bootstrap_theme %}
     <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha3/dist/css/bootstrap.min.css" rel="stylesheet"
       integrity="sha384-KK94CHFLLe+nY2dmCWGMq91rCGa5gtU4mk92HdvYe+M/SXH301p5ILy+dN9+nJOZ" crossorigin="anonymous">
+    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.10.4/font/bootstrap-icons.css">
+    <link rel="stylesheet" href="//cdn.jsdelivr.net/gh/highlightjs/cdn-release@11.7.0/build/styles/default.min.css">
   {% endblock %}
 
   {% if code_style %}<style>{{ code_style }}</style>{% endif %}
 {% endblock %}
 
 
 {% block navbar %}
@@ -35,50 +37,60 @@
             <span class="navbar-toggler-icon"></span>
           </button>
 
           <div class="collapse navbar-collapse" id="navbar">
             <ul class="navbar-nav me-auto">
               <li class="nav-item">
                 <a href="https://www.django-rest-framework.org/" class="nav-link">
-                  <strong>
+                  <strong class="d-flex align-items-center gap-3">
+                    <i class="bi house-fill"></i>
                     {% translate "Home" %}
                   </strong>
                 </a>
               </li>
               <li class="nav-item">
                 <a href="https://www.django-rest-framework.org/tutorial/quickstart/" class="nav-link">
-                  <strong>
+                  <strong class="d-flex align-items-center gap-3">
+                    <i class="bi bi-journal-code"></i>
                     {% translate "Tutorial" %}
                   </strong>
                 </a>
               </li>
               <li class="nav-item">
                 <a href="https://github.com/encode/django-rest-framework/" class="nav-link">
-                  <strong>
+                  <strong class="d-flex align-items-center gap-3">
+                    <i class="bi bi-github"></i>
                     {% translate "Github" %}
                   </strong>
                 </a>
               </li>
             </ul>
             <ul class="navbar-nav">
               <li class="nav-item dropdown">
                 <a href="#" class="nav-link" data-bs-toggle="dropdown">
-                  <strong>
+                  <strong class="d-flex align-items-center gap-3">
+                    <i class="bi bi-person-fill"></i>
                     {{ request.user|capfirst }}
                   </strong>
                 </a>
                 <ul class="dropdown-menu dropdown-menu-dark dropdown-menu-end rounded-3 shadow">
                   <li>
                     {% if user.is_authenticated %}
                       <a class="dropdown-item" href="{% url 'rest_framework:logout' %}">
-                        {% translate 'Logout' %}
+                        <strong class="d-flex align-items-center gap-3">
+                          <i class="bi bi-box-arrow-right"></i>
+                          {% translate 'Logout' %}
+                        </strong>
                       </a>
                     {% else %}
                       <a class="dropdown-item" href="{% url 'rest_framework:login' %}">
-                        {% translate 'Login' %}
+                        <strong class="d-flex align-items-center gap-3">
+                          <i class="bi bi-box-arrow-in-right"></i>
+                          {% translate 'Login' %}
+                        </strong>
                       </a>
                     {% endif %}
                   </li>
                 </ul>
               </li>
             </ul>
           </div>
@@ -175,25 +187,27 @@
             </fieldset>
           </form>
         {% endif %}
 
         {% if options_form %}
           <form class="button-form" action="{{ request.get_full_path }}" data-method="OPTIONS">
             <button type="submit" class="btn btn-lg btn-secondary w-100" title="Make an OPTIONS request on the {{ name }} resource">
-              <strong>
+              <strong class="d-flex align-items-center gap-3">
+                <i class="bi bi-info-square"></i>
                 {% translate "OPTIONS" %}
               </strong>
             </button>
           </form>
         {% endif %}
 
         {% if delete_form %}
           <button type="button" class="btn btn-lg btn-danger w-100" data-bs-toggle="modal" data-bs-target="#deleteModal"
             title="Make a DELETE request on the {{ name }} resource">
-            <strong>
+            <strong class="d-flex align-items-center gap-3">
+              <i class="bi bi-trash"></i>
               {% translate "DELETE" %}
             </strong>
           </button>
 
           <div class="modal fade" id="deleteModal" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
             <div class="modal-dialog">
               <div class="modal-content p-3 rounded-3 shadow">
@@ -227,18 +241,18 @@
           </div>
         {% endif %}
 
         {% if extra_actions %}
           <div class="dropdown" style="float: right; margin-right: 10px">
             <button class="btn btn-lg btn-info w-100" id="extra-actions-menu" data-bs-toggle="dropdown" aria-haspopup="true"
               aria-expanded="true">
-              <strong>
+              <strong class="d-flex align-items-center gap-3">
+                <i class="bi bi-three-dots"></i>
                 {% translate "Extra Actions" %}
               </strong>
-              <span class="caret"></span>
             </button>
             <ul class="dropdown-menu" aria-labelledby="extra-actions-menu">
               {% for action_name, url in extra_actions|items %}
                 <li>
                   <a class="dropdown-item" href="{{ url }}">
                     {{ action_name }}
                   </a>
@@ -246,54 +260,57 @@
               {% endfor %}
             </ul>
           </div>
         {% endif %}
 
         {% if filter_form %}
           <button data-bs-toggle="modal" data-bs-target="#filtersModal" class="btn btn-lg btn-success">
-            <strong>
+            <strong class="d-flex align-items-center gap-3">
+              <i class="bi bi-filter"></i>
               {% translate "Filters" %}
             </strong>
           </button>
         {% endif %}
       </section>
     {% endblock %}
 
     <div class="row g-4 mb-4" aria-label="{% translate "Main content" %}">
-      <section class="col-12 col-lg-8" role="main" aria-label="{% translate 'main content' %}">
+      <section class="col-12 col-lg-8" role="main" aria-label="{% translate 'Main content' %}">
         <div class="card card-body rounded-3">
-          <div class="request-info" style="clear: both" aria-label="{% translate 'request info' %}">
+          <div class="request-info" aria-label="{% translate 'Request info' %}">
             <pre class="prettyprint"><b>{{ request.method }}</b> {{ request.get_full_path }}</pre>
           </div>
 
           <div class="response-info" aria-label="{% translate 'response info' %}">
-            <pre class="prettyprint"><div class="language-http bg-white"><strong>HTTP {{ response.status_code }} {{ response.status_text }}</strong><br>{% for key, val in response_headers|items %}<br><strong>{{ key }}:</strong> <span class="lit">{{ val|break_long_headers|urlize }}</span>{% endfor %}</div><code class="language-json bg-light rounded-4">{{ content|urlize }}</code></pre>
+            <pre class="prettyprint"><div class="language-http bg-light rounded-4 mb-4"><div><strong>HTTP {{ response.status_code }} {{ response.status_text }}</strong></div>{% for key, val in response_headers|items %}<div><strong>{{ key }}:</strong> <span class="lit">{{ val|break_long_headers|urlize }}</span></div>{% endfor %}</div><code class="language-json bg-light rounded-4">{{ content|urlize }}</code></pre>
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
-                      <strong>
+                      <strong class="d-flex align-items-center gap-3">
+                        <i class="bi bi-filetype-html"></i>
                         {% translate 'HTML form' %}
                       </strong>
                     </button>
                   </li>
                   <li class="nav-item" role="presentation">
                     <button class="nav-link rounded-5" id="raw-tab" data-bs-toggle="tab" data-bs-target="#raw"
                       type="button" role="tab" aria-controls="raw" aria-selected="false">
-                      <strong>
+                      <strong class="d-flex align-items-center gap-3">
+                        <i class="bi bi-filetype-json"></i>
                         {% translate 'Raw data' %}
                       </strong>
                     </button>
                   </li>
                 </ul>
               {% endif %}
 
@@ -304,15 +321,16 @@
                       <form action="{{ request.get_full_path }}" method="POST" enctype="multipart/form-data"
                         class="form-horizontal" novalidate>
                         <fieldset>
                           {% csrf_token %}
                           {{ post_form }}
                           <div class="form-actions">
                             <button class="btn btn-lg btn-primary w-100" title="Make a POST request on the {{ name }} resource">
-                              <strong>
+                              <strong class="d-flex align-items-center gap-3">
+                                <i class="bi bi-send-fill"></i>
                                 {% translate "POST" %}
                               </strong>
                             </button>
                           </div>
                         </fieldset>
                       </form>
                     {% endwith %}
@@ -322,15 +340,16 @@
                 <div class="tab-pane" id="raw" role="tabpanel" aria-labelledby="raw-tab" tabindex="0">
                   {% with form=raw_data_post_form %}
                     <form action="{{ request.get_full_path }}" method="POST" class="form-horizontal">
                       <fieldset>
                         {% include "rest_framework/raw_data_form.html" %}
                         <div class="form-actions">
                           <button class="btn btn-lg btn-primary w-100" title="Make a POST request on the {{ name }} resource">
-                            <strong>
+                            <strong class="d-flex align-items-center gap-3">
+                              <i class="bi bi-send-fill"></i>
                               {% translate "POST" %}
                             </strong>
                           </button>
                         </div>
                       </fieldset>
                     </form>
                   {% endwith %}
@@ -343,23 +362,25 @@
             <div {% if put_form %}class="card card-body rounded-3"{% endif %}>
               {% if put_form %}
                 <ul class="nav nav-pills nav-fill gap-2 p-1 small bg-dark rounded-5 shadow mb-4" role="tablist"
                   style="--bs-nav-link-color: var(--bs-danger); --bs-nav-pills-link-active-color: var(--bs-white); --bs-nav-pills-link-active-bg: var(--bs-danger);">
                   <li class="nav-item" role="presentation">
                     <button class="nav-link active rounded-5" id="form-tab" data-bs-toggle="tab" data-bs-target="#put-object-form"
                       type="button" role="tab" aria-controls="form" aria-selected="true">
-                      <strong>
+                      <strong class="d-flex align-items-center gap-3">
+                        <i class="bi bi-filetype-html"></i>
                         {% translate 'HTML form' %}
                       </strong>
                     </button>
                   </li>
                   <li class="nav-item" role="presentation">
                     <button class="nav-link rounded-5" id="raw-tab" data-bs-toggle="tab" data-bs-target="#put-generic-content-form"
                       type="button" role="tab" aria-controls="raw" aria-selected="false">
-                      <strong>
+                      <strong class="d-flex align-items-center gap-3">
+                        <i class="bi bi-filetype-json"></i>
                         {% translate 'Raw data' %}
                       </strong>
                     </button>
                   </li>
                 </ul>
               {% endif %}
 
@@ -368,15 +389,16 @@
                   <div class="tab-pane active" id="put-object-form">
                     <form action="{{ request.get_full_path }}" data-method="PUT" enctype="multipart/form-data"
                       class="form-horizontal" novalidate>
                       <fieldset>
                         {{ put_form }}
                         <div class="form-actions">
                           <button class="btn btn-lg btn-primary w-100" title="Make a PUT request on the {{ name }} resource">
-                            <strong>
+                            <strong class="d-flex align-items-center gap-3">
+                              <i class="bi bi-send-fill"></i>
                               {% translate "PUT" %}
                             </strong>
                           </button>
                         </div>
                       </fieldset>
                     </form>
                   </div>
@@ -385,28 +407,30 @@
                 <div {% if put_form %}class="tab-pane"{% endif %} id="put-generic-content-form">
                   {% with form=raw_data_put_or_patch_form %}
                     <form action="{{ request.get_full_path }}" data-method="PUT" class="form-horizontal">
                       <fieldset>
                         {% include "rest_framework/raw_data_form.html" %}
                         <div class="form-actions">
                           {% if raw_data_put_form %}
-                          <button class="btn btn-lg btn-primary w-100"
-                            title="Make a PUT request on the {{ name }} resource">
-                            <strong>
-                              {% translate "PUT" %}
-                            </strong>
-                          </button>
+                            <button class="btn btn-lg btn-primary w-100"
+                              title="Make a PUT request on the {{ name }} resource">
+                              <strong class="d-flex align-items-center gap-3">
+                                <i class="bi bi-send-fill"></i>
+                                {% translate "PUT" %}
+                              </strong>
+                            </button>
                           {% endif %}
                           {% if raw_data_patch_form %}
-                          <button data-method="PATCH" class="btn btn-lg btn-primary"
-                            title="Make a PATCH request on the {{ name }} resource">
-                            <strong>
-                              {% translate "PATCH" %}
-                            </strong>
-                          </button>
+                            <button data-method="PATCH" class="btn btn-lg btn-primary"
+                              title="Make a PATCH request on the {{ name }} resource">
+                              <strong class="d-flex align-items-center gap-3">
+                                <i class="bi bi-send-fill"></i>
+                                {% translate "PATCH" %}
+                              </strong>
+                            </button>
                           {% endif %}
                         </div>
                       </fieldset>
                     </form>
                   {% endwith %}
                 </div>
               </div>
@@ -437,11 +461,10 @@
     $(document).ready(function() {
       $('form').ajaxForm();
     });
   </script>
   <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha3/dist/js/bootstrap.bundle.min.js"
     integrity="sha384-ENjdO4Dr2bkBIFxQpeoTz1HIcje39Wm4jDKdf19U8gI4ddQ3GYNS7NTKfAdVQSZe"
     crossorigin="anonymous"></script>
-  <link rel="stylesheet" href="//cdn.jsdelivr.net/gh/highlightjs/cdn-release@11.7.0/build/styles/default.min.css">
   <script src="//cdn.jsdelivr.net/gh/highlightjs/cdn-release@11.7.0/build/highlight.min.js"></script>
   <script>hljs.highlightAll()</script>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,19 +1,24 @@
 {% extends "rest_framework/base.html" %} {% load i18n static rest_framework %}
 {% block meta %} {{ block.super }}
  {% endblock %} {% block style %} {% block bootstrap_theme %}
+
+
  {% endblock %} {% if code_style %}
 {% endif %} {% endblock %} {% block navbar %}
 {% block branding %} {%_translate_'Django_REST_Framework'_%} {% endblock %}
-    * {%_translate_"Home"_%}
-    * {%_translate_"Tutorial"_%}
-    * {%_translate_"Github"_%}
-    * {{_request.user|capfirst_}}
-          o {% if user.is_authenticated %} {%_translate_'Logout'_%} {% else %}
-            {%_translate_'Login'_%} {% endif %}
+    *  {%_translate_"Home"_%}
+    *  {%_translate_"Tutorial"_%}
+    *  {%_translate_"Github"_%}
+    *  {{_request.user|capfirst_}}
+          o {% if user.is_authenticated %}
+             {%_translate_'Logout'_%}
+             {% else %}
+             {%_translate_'Login'_%}
+             {% endif %}
  {% endblock %} {% block breadcrumbs %}
    1. {% for breadcrumb_name, breadcrumb_url in breadcrumblist %} {% if
       forloop.last %}
    2. {{ breadcrumb_name }}
    3. {% else %}
    4. {{_breadcrumb_name_}}
    5. {% endif %} {% empty %} {% block breadcrumbs_empty %} {% endblock
@@ -28,67 +33,91 @@
 {%_translate_"GET"_%}
     * * {% translate 'Select a format' %} *
     * {% for format in available_formats %}
     * {{_format_}}
     * {% endfor %}
 {% else %} {%_translate_"GET"_%} {% endif %}
 {% endif %} {% if options_form %}
+
  {% translate "OPTIONS" %}
-{% endif %} {% if delete_form %}  {% translate "DELETE" %}
+
+{% endif %} {% if delete_form %}
+ {% translate "DELETE" %}
+
 ** {% translate 'Delete' %} {{ name }} **
 {% translate "Are you sure you want to delete this" %} {{ name }}?
  {% translate "Cancel" %}
  {% translate "Delete" %}
 {% endif %} {% if extra_actions %}
+
  {% translate "Extra Actions" %}
+
     * {% for action_name, url in extra_actions|items %}
     * {{_action_name_}}
     * {% endfor %}
-{% endif %} {% if filter_form %}  {% translate "Filters" %}  {% endif %}  {%
-endblock %}
+{% endif %} {% if filter_form %}
+ {% translate "Filters" %}
+  {% endif %}  {% endblock %}
  %}">
 {{ request.method }} {{ request.get_full_path }}
 HTTP {{ response.status_code }} {{ response.status_text }}
 {% for key, val in response_headers|items %}
-{{ key }}: {{ val|break_long_headers|urlize }}{% endfor %}
+{{ key }}: {{ val|break_long_headers|urlize }}
+{% endfor %}
 {{ content|urlize }}
   {% if display_edit_forms %} {% if post_form or raw_data_post_form %}
 % if post_form %}class="card card-body rounded-3" {% endif %}> {% if post_form
 %}
-    *  {% translate 'HTML form' %}
-    *  {% translate 'Raw data' %}
+    *
+       {% translate 'HTML form' %}
+
+    *
+       {% translate 'Raw data' %}
+
 {% endif %}
 {% if post_form %}
 {% with form=post_form %}
  {% csrf_token %} {{ post_form }}
+
  {% translate "POST" %}
+
 {% endwith %}
 {% endif %}
 {% with form=raw_data_post_form %}
  {% include "rest_framework/raw_data_form.html" %}
+
  {% translate "POST" %}
+
 {% endwith %}
 {% endif %} {% if put_form or raw_data_put_form or raw_data_patch_form %}
 % if put_form %}class="card card-body rounded-3"{% endif %}> {% if put_form %}
-    *  {% translate 'HTML form' %}
-    *  {% translate 'Raw data' %}
+    *
+       {% translate 'HTML form' %}
+
+    *
+       {% translate 'Raw data' %}
+
 {% endif %}
 {% if put_form %}
  {{ put_form }}
+
  {% translate "PUT" %}
+
 {% endif %}
 % if put_form %}class="tab-pane"{% endif %} id="put-generic-content-form"> {%
 with form=raw_data_put_or_patch_form %}
  {% include "rest_framework/raw_data_form.html" %}
-{% if raw_data_put_form %}  {% translate "PUT" %}  {% endif %} {% if
-raw_data_patch_form %}  {% translate "PATCH" %}  {% endif %}
+{% if raw_data_put_form %}
+ {% translate "PUT" %}
+  {% endif %} {% if raw_data_patch_form %}
+ {% translate "PATCH" %}
+  {% endif %}
 {% endwith %}
 {% endif %} {% endif %}   {% endblock %} {% if filter_form %} {{ filter_form }}
 {% endif %} {% block script %}
 
 s/jquery-3.5.1.min.js" %}">
 s/ajax-form.js" %}">
 s/csrf.js" %}">
 s/prettify-min.js" %}">
 s/default.js" %}">
-
  {% endblock %}
```

### Comparing `rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/filters/base.html` & `rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/filters/base.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/filters/ordering.html` & `rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/filters/ordering.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/filters/search.html` & `rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/filters/search.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/horizontal/checkbox.html` & `rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/horizontal/checkbox.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/horizontal/checkbox_multiple.html` & `rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/horizontal/checkbox_multiple.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/horizontal/input.html` & `rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/horizontal/input.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/horizontal/radio.html` & `rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/horizontal/radio.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/horizontal/select.html` & `rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/horizontal/select.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/horizontal/select_multiple.html` & `rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/horizontal/select_multiple.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/horizontal/textarea.html` & `rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/horizontal/textarea.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/login.html` & `rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/login.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 {% extends "rest_framework/login_base.html" %}
 
 {% load static i18n rest_framework %}
 
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
+    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.10.4/font/bootstrap-icons.css">
   {% endblock %}
 
   {% if code_style %}<style>{{ code_style }}</style>{% endif %}
 {% endblock %}
 
 {% block body %}
-<body class="container">
+  <body class="container">
   <div style="height: 100vh" class="d-flex align-items-center justify-content-center">
     <div class="col-12 col-md-6 col-lg-4">
       <div class="card rounded-4 shadow">
         <div class="card-header bg-danger rounded-top-4"></div>
         <main class="card-body gap-4 p-5">
           {% block branding %}
             <h3 class="mb-4">
@@ -59,25 +59,26 @@
             {% if form.non_field_errors %}
               {% for error in form.non_field_errors %}
                 <div class="alert alert-warning" role="alert">{{ error }}</div>
               {% endfor %}
             {% endif %}
 
             <button type="submit" class="btn btn-lg btn-primary w-100">
-              <strong>
+              <strong class="d-flex align-items-center gap-3">
+                <i class="bi bi-box-arrow-in-right"></i>
                 {% translate "Login" %}
               </strong>
             </button>
           </form>
         </main>
         <div class="card-footer bg-danger rounded-bottom-4"></div>
       </div>
     </div>
   </div>
-</body>
+  </body>
 {% endblock %}
 
 
 {% block script %}
   <script>
     window.drf = {
       csrfHeaderName: "{{ csrf_header_name|default:'X-CSRFToken' }}",
@@ -93,10 +94,8 @@
     $(document).ready(function() {
       $('form').ajaxForm();
     });
   </script>
   <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha3/dist/js/bootstrap.bundle.min.js"
     integrity="sha384-ENjdO4Dr2bkBIFxQpeoTz1HIcje39Wm4jDKdf19U8gI4ddQ3GYNS7NTKfAdVQSZe"
     crossorigin="anonymous"></script>
-  <link rel="stylesheet" href="//cdn.jsdelivr.net/gh/highlightjs/cdn-release@11.7.0/build/styles/default.min.css">
-  <script src="//cdn.jsdelivr.net/gh/highlightjs/cdn-release@11.7.0/build/highlight.min.js"></script>
 {% endblock %}
```

### Comparing `rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/pagination/numbers.html` & `rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/pagination/numbers.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.2/rest_framework_redesign/templates/rest_framework/pagination/previous_and_next.html` & `rest_framework_redesign-0.1.3/rest_framework_redesign/templates/rest_framework/pagination/previous_and_next.html`

 * *Files identical despite different names*

### Comparing `rest_framework_redesign-0.1.2/PKG-INFO` & `rest_framework_redesign-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rest-framework-redesign
-Version: 0.1.2
+Version: 0.1.3
 Summary: Redesign of the browsable api of Django REST Framework
 Home-page: https://github.com/youzarsiph/rest-framework-redesign/
 License: MIT
 Author: Yousef Abu Shanab
 Author-email: josephyousef249@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

