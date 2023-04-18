# Comparing `tmp/django_prose-1.2.0.tar.gz` & `tmp/django_prose-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_prose-1.2.0.tar", max compression
+gzip compressed data, was "django_prose-1.2.2.tar", max compression
```

## Comparing `django_prose-1.2.0.tar` & `django_prose-1.2.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0     1098 2023-01-27 13:53:42.221301 django_prose-1.2.0/LICENSE
--rw-r--r--   0        0        0     6132 2023-01-27 13:53:42.221301 django_prose-1.2.0/README.md
--rw-r--r--   0        0        0        0 2023-01-27 13:53:42.225301 django_prose-1.2.0/prose/__init__.py
--rw-r--r--   0        0        0      100 2023-01-27 13:53:42.225301 django_prose-1.2.0/prose/admin.py
--rw-r--r--   0        0        0      105 2023-01-27 13:53:42.225301 django_prose-1.2.0/prose/apps.py
--rw-r--r--   0        0        0      986 2023-01-27 13:53:42.225301 django_prose-1.2.0/prose/fields.py
--rw-r--r--   0        0        0      687 2023-01-27 13:53:42.225301 django_prose-1.2.0/prose/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-01-27 13:53:42.225301 django_prose-1.2.0/prose/migrations/__init__.py
--rw-r--r--   0        0        0      538 2023-01-27 13:53:42.225301 django_prose-1.2.0/prose/models.py
--rw-r--r--   0        0        0      426 2023-01-27 13:53:42.225301 django_prose-1.2.0/prose/static/prose/editor.css
--rw-r--r--   0        0        0     1814 2023-01-27 13:53:42.225301 django_prose-1.2.0/prose/static/prose/editor.js
--rw-r--r--   0        0        0      369 2023-01-27 13:53:42.225301 django_prose-1.2.0/prose/templates/prose/forms/widgets/editor.html
--rw-r--r--   0        0        0       60 2023-01-27 13:53:42.225301 django_prose-1.2.0/prose/tests.py
--rw-r--r--   0        0        0      156 2023-01-27 13:53:42.225301 django_prose-1.2.0/prose/urls.py
--rw-r--r--   0        0        0      437 2023-01-27 13:53:42.225301 django_prose-1.2.0/prose/views.py
--rw-r--r--   0        0        0      453 2023-01-27 13:53:42.229301 django_prose-1.2.0/prose/widgets.py
--rw-r--r--   0        0        0      495 2023-01-27 13:53:42.229301 django_prose-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     7049 1970-01-01 00:00:00.000000 django_prose-1.2.0/setup.py
--rw-r--r--   0        0        0     6844 1970-01-01 00:00:00.000000 django_prose-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1098 2023-04-18 10:43:50.399865 django_prose-1.2.2/LICENSE
+-rw-r--r--   0        0        0     6886 2023-04-18 10:43:50.399865 django_prose-1.2.2/README.md
+-rw-r--r--   0        0        0        0 2023-04-18 10:43:50.399865 django_prose-1.2.2/prose/__init__.py
+-rw-r--r--   0        0        0      100 2023-04-18 10:43:50.399865 django_prose-1.2.2/prose/admin.py
+-rw-r--r--   0        0        0      162 2023-04-18 10:43:50.399865 django_prose-1.2.2/prose/apps.py
+-rw-r--r--   0        0        0     1051 2023-04-18 10:43:50.399865 django_prose-1.2.2/prose/fields.py
+-rw-r--r--   0        0        0      686 2023-04-18 10:43:50.399865 django_prose-1.2.2/prose/migrations/0001_initial.py
+-rw-r--r--   0        0        0      459 2023-04-18 10:43:50.399865 django_prose-1.2.2/prose/migrations/0002_alter_document_id.py
+-rw-r--r--   0        0        0        0 2023-04-18 10:43:50.399865 django_prose-1.2.2/prose/migrations/__init__.py
+-rw-r--r--   0        0        0      538 2023-04-18 10:43:50.399865 django_prose-1.2.2/prose/models.py
+-rw-r--r--   0        0        0      519 2023-04-18 10:43:50.399865 django_prose-1.2.2/prose/static/prose/editor.css
+-rw-r--r--   0        0        0     1814 2023-04-18 10:43:50.399865 django_prose-1.2.2/prose/static/prose/editor.js
+-rw-r--r--   0        0        0      369 2023-04-18 10:43:50.399865 django_prose-1.2.2/prose/templates/prose/forms/widgets/editor.html
+-rw-r--r--   0        0        0       60 2023-04-18 10:43:50.399865 django_prose-1.2.2/prose/tests.py
+-rw-r--r--   0        0        0      156 2023-04-18 10:43:50.399865 django_prose-1.2.2/prose/urls.py
+-rw-r--r--   0        0        0      437 2023-04-18 10:43:50.399865 django_prose-1.2.2/prose/views.py
+-rw-r--r--   0        0        0      453 2023-04-18 10:43:50.399865 django_prose-1.2.2/prose/widgets.py
+-rw-r--r--   0        0        0      495 2023-04-18 10:43:50.399865 django_prose-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     7831 1970-01-01 00:00:00.000000 django_prose-1.2.2/setup.py
+-rw-r--r--   0        0        0     7598 1970-01-01 00:00:00.000000 django_prose-1.2.2/PKG-INFO
```

### Comparing `django_prose-1.2.0/LICENSE` & `django_prose-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_prose-1.2.0/README.md` & `django_prose-1.2.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -8,37 +8,57 @@
 
 - Python 3.8 or later
 - Django 3.2 or later
 - Bleach 4.0 or later
 
 ## Getting started
 
-To get started with Django Prose, first make sure to install it. We use and suggest using Poetry, although Pipenv and pip will work seamlessly as well
+To get started with Django Prose, all you need to do is follow **just four steps**.
 
-```console
-poetry add django-prose
-```
-
-Then, add `prose` in Django's installed apps (example: [`example/example/settings.py`](https://github.com/withlogicco/django-prose/blob/9e24cc794eae6db48818dd15a483d106d6a99da0/example/example/settings.py#L46)):
-
-```python
-INSTALLED_APPS = [
-    # Django stock apps (e.g. 'django.contrib.admin')
-
-    'prose',
-
-    # your application's apps
-]
-```
+1. **Install `django-prose`**
+    
+    We use and suggest using Poetry, although Pipenv and plain pip will work seamlessly as well
+    
+    ```console
+    poetry add django-prose
+    ```
+
+2. **Add to `INSTALLED_APPS`**
+    
+    Add `prose` in your Django project's installed apps (example: [`example/example/settings.py`](https://github.com/withlogicco/django-prose/blob/9e24cc794eae6db48818dd15a483d106d6a99da0/example/example/settings.py#L46)):
+    
+    ```python
+    INSTALLED_APPS = [
+        # Django stock apps (e.g. 'django.contrib.admin')
+    
+        'prose',
+    
+        # your application's apps
+    ]
+    ```
 
-Last, run migrations so you can use Django Prose's Document model:
+3. **Run migrations**
 
-```
-python manage.py migrate prose
-```
+    This is required so you can use Django Prose's built-in Document model:
+  
+    ```console
+    python manage.py migrate prose
+    ```
+
+4. **Include URLs**
+
+    You need to edit the main `urls.py` file of your Django project and include `prose.urls`:
+    
+    ```python
+    urlpatterns = [
+        path('admin/', admin.site.urls),
+        # other urls ...
+        path("prose/", include("prose.urls")),
+    ]
+    ```
 
 Now, you are ready to go 🚀.
 
 ## Usage
 
 There are different ways to use Django prose according to your needs. We will examine all of them here.
 
@@ -131,14 +151,20 @@
 
 ## Screenshots
 
 ### Django Prose Documents in Django Admin
 
 ![Django Prose Document in Django Admin](./docs/django-admin-prose-document.png)
 
+## Video tutorial
+
+If you are more of a video person, you can watch our video showcasing how to **Create a blog using Django Prose** on YouTube
+
+[![Watch the video](https://img.youtube.com/vi/uICZjUpAbhQ/hqdefault.jpg)](https://youtu.be/uICZjUpAbhQ)
+
 ## Real world use cases
 - **Remote Work Café**: Used to edit location pagess, like [Amsterdam | Remote Work Café](https://remotework.cafe/locations/amsterdam/)
 - In production by multiple clients of [LOGIC](https://withlogic.co), from small companies to the public sector.
 
 If you are using Django Prose in your application too, feek free to open a [Pull Request](https://github.com/withlogicco/django-prose/pulls) to include it here. We would love to have it.
 
 ## Development for Django Prose
```

### Comparing `django_prose-1.2.0/prose/fields.py` & `django_prose-1.2.2/prose/fields.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     "h3",
     "h4",
     "h5",
     "h6",
     "picture",
     "source",
     "img",
+    "del",
 ]
 ALLOWED_ATTRIBUTES = [
     "alt",
     "class",
     "id",
     "src",
     "srcset",
@@ -45,14 +46,17 @@
 class RichTextField(models.TextField):
     def formfield(self, **kwargs):
         kwargs["widget"] = RichTextEditor
         return super().formfield(**kwargs)
 
     def pre_save(self, model_instance, add):
         raw_html = getattr(model_instance, self.attname)
+        if not raw_html:
+            return raw_html
+
         sanitized_html = bleach.clean(
             raw_html, tags=ALLOWED_TAGS, attributes=ALLOWED_ATTRIBUTES
         )
         return sanitized_html
 
 
 class DocumentContentField(RichTextField):
```

### Comparing `django_prose-1.2.0/prose/migrations/0001_initial.py` & `django_prose-1.2.2/prose/migrations/0001_initial.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Generated by Django 2.1.4 on 2019-01-05 16:09
 
 from django.db import migrations, models
 import prose.fields
 
 
 class Migration(migrations.Migration):
-
     initial = True
 
     dependencies = []
 
     operations = [
         migrations.CreateModel(
             name="Document",
```

### Comparing `django_prose-1.2.0/prose/models.py` & `django_prose-1.2.2/prose/models.py`

 * *Files identical despite different names*

### Comparing `django_prose-1.2.0/prose/static/prose/editor.js` & `django_prose-1.2.2/prose/static/prose/editor.js`

 * *Files identical despite different names*

### Comparing `django_prose-1.2.0/setup.py` & `django_prose-1.2.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*'], 'prose': ['static/prose/*', 'templates/prose/forms/widgets/*']}
 
 install_requires = \
 ['bleach>=4.0', 'django>=3.2']
 
 setup_kwargs = {
     'name': 'django-prose',
-    'version': '1.2.0',
+    'version': '1.2.2',
     'description': 'Wonderful rich text for Django',
-    'long_description': '# Django Prose\n\n![PyPI - Downloads](https://img.shields.io/pypi/dw/django-prose?color=purple) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/django-prose)\n\nDjango Prose provides your Django applications with wonderful rich-text editing capabilities.\n\n## Requirements\n\n- Python 3.8 or later\n- Django 3.2 or later\n- Bleach 4.0 or later\n\n## Getting started\n\nTo get started with Django Prose, first make sure to install it. We use and suggest using Poetry, although Pipenv and pip will work seamlessly as well\n\n```console\npoetry add django-prose\n```\n\nThen, add `prose` in Django\'s installed apps (example: [`example/example/settings.py`](https://github.com/withlogicco/django-prose/blob/9e24cc794eae6db48818dd15a483d106d6a99da0/example/example/settings.py#L46)):\n\n```python\nINSTALLED_APPS = [\n    # Django stock apps (e.g. \'django.contrib.admin\')\n\n    \'prose\',\n\n    # your application\'s apps\n]\n```\n\nLast, run migrations so you can use Django Prose\'s Document model:\n\n```\npython manage.py migrate prose\n```\n\nNow, you are ready to go 🚀.\n\n## Usage\n\nThere are different ways to use Django prose according to your needs. We will examine all of them here.\n\n### Rendering rich-text in templates\n\nRich text content essentially is HTML. For this reason it needs to be manually marked as [`safe`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#safe), when rendered in Django templates. Example:\n\n```django\n{{ document.content | safe}}\n```\n\n### Small rich-text content\n\nYou might want to add rich-text content in a model that is just a few characters (e.g. 140), like an excerpt from an article. In that case we suggest using the `RichTextField`. Example:\n\n```py\nfrom django.db import models\nfrom prose.fields import RichTextField\n\nclass Article(models.Model):\n    excerpt = RichTextField()\n```\n\nAs mentioned above, you need to mark the article excerpt as `safe`, in order to render it:\n\n```django\n<div class="article-excerpt">{{ article.excerpt | safe}}</div>\n```\n\n### Large rich-text content\n\nIn case you want to store large rich-text content, like the body of an article, which can span to quite a few thousand characters, we suggest you use the `AbstractDocument` model. This will save large rich-text content in a separate database table, which is better for performance. Example:\n\n```py\nfrom django.db import models\nfrom prose.fields import RichTextField\nfrom prose.models import AbstractDocument\n\nclass ArticleContent(AbstractDocument):\n    pass\n\nclass Article(models.Model):\n    excerpt = RichTextField()\n    body = models.OneToOneField(ArticleContent, on_delete=models.CASCADE)\n```\n\nSimilarly here as well, you need to mark the article\'s body as `safe`, in order to render it:\n\n```django\n<div class="article-body">{{ article.body.content | safe}}</div>\n```\n\n### Forms with rich-text editing\n\nYou can create forms for your Django Prose models, to provide rich-text editing functionality. In that case, you will also need to render `form.media`, to load Trix with its stylesheets.\n\n```django\n<form  method="POST" >\n  {% csrf_token %}\n  \n  {{ form.as_p }}\n  {{ form.media }}\n  \n  <button type="submit">Submit</button>\n</form>\n```\n\nThe same is true also, if you are rendering the forms field manually.\n\n### Attachments\n\nDjango Prose can also handle uploading attachments with drag and drop. To set this up, first you need to:\n\n- [x] Set up the `MEDIA_ROOT` and `MEDIA_URL` of your Django project (example in [`example/example/settings.py`](https://github.com/withlogicco/django-prose/blob/9e24cc794eae6db48818dd15a483d106d6a99da0/example/example/settings.py#L130-L131)))\n- [x] Include the Django Prose URLs (example in [`example/example/urls.py`](https://github.com/withlogicco/django-prose/blob/9e24cc794eae6db48818dd15a483d106d6a99da0/example/example/urls.py#L13-L14))\n- [x] (Optional) Set up a different Django storage to store your files (e.g. S3)\n\n### Full example\n\nYou can find a full example of a blog, built with Django Prose in the [`example`](./example/) directory.\n\n## 🔒 A note on security\n\nAs you can see in the examples above, what Django Prose does is provide you with a user friendly editor ([Trix](https://trix-editor.org/)) for your rich text content and then store it as HTML in your database. Since you will mark this HTML as safe in order to use it in your templates, it needs to be **sanitised**, before it gets stored in the database.\n\nFor this reason Django Prose is using [Bleach](https://bleach.readthedocs.io/en/latest/) to only allow the following tags and attributes:\n\n- **Allowed tags**: `p`, `ul`, `ol`, `li`, `strong`, `em`, `div`, `span`, `a`, `blockquote`, `pre`, `figure`, `figcaption`, `br`, `code`, `h1`, `h2`, `h3`, `h4`, `h5`, `h6`, `picture`, `source`, `img`\n- **Allowed attributes**: `alt`, `class`, `id`, `src`, `srcset`, `href`, `media`\n\n## Screenshots\n\n### Django Prose Documents in Django Admin\n\n![Django Prose Document in Django Admin](./docs/django-admin-prose-document.png)\n\n## Real world use cases\n- **Remote Work Café**: Used to edit location pagess, like [Amsterdam | Remote Work Café](https://remotework.cafe/locations/amsterdam/)\n- In production by multiple clients of [LOGIC](https://withlogic.co), from small companies to the public sector.\n\nIf you are using Django Prose in your application too, feek free to open a [Pull Request](https://github.com/withlogicco/django-prose/pulls) to include it here. We would love to have it.\n\n## Development for Django Prose\n\nIf you plan to contribute code to Django Prose, this section is for you. All development tooling for Django Prose has been set up with Docker and Development Containers.\n\nTo get started run these commands in the provided order:\n\n```console\ndocker compose run --rm migrate\ndocker compose run --rm createsuperuser\ndocker compose up\n```\n\nIf you are using Visual Studio code, just open this repository in a container using the [`Dev Containers: Open Folder in Container`](https://code.visualstudio.com/docs/devcontainers/containers#_quick-start-open-an-existing-folder-in-a-container).\n\n---\n\n<p align="center">\n  <i>🦄 Built with <a href="https://withlogic.co/">LOGIC</a>. 🦄</i>\n</p>\n',
+    'long_description': '# Django Prose\n\n![PyPI - Downloads](https://img.shields.io/pypi/dw/django-prose?color=purple) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/django-prose)\n\nDjango Prose provides your Django applications with wonderful rich-text editing capabilities.\n\n## Requirements\n\n- Python 3.8 or later\n- Django 3.2 or later\n- Bleach 4.0 or later\n\n## Getting started\n\nTo get started with Django Prose, all you need to do is follow **just four steps**.\n\n1. **Install `django-prose`**\n    \n    We use and suggest using Poetry, although Pipenv and plain pip will work seamlessly as well\n    \n    ```console\n    poetry add django-prose\n    ```\n\n2. **Add to `INSTALLED_APPS`**\n    \n    Add `prose` in your Django project\'s installed apps (example: [`example/example/settings.py`](https://github.com/withlogicco/django-prose/blob/9e24cc794eae6db48818dd15a483d106d6a99da0/example/example/settings.py#L46)):\n    \n    ```python\n    INSTALLED_APPS = [\n        # Django stock apps (e.g. \'django.contrib.admin\')\n    \n        \'prose\',\n    \n        # your application\'s apps\n    ]\n    ```\n\n3. **Run migrations**\n\n    This is required so you can use Django Prose\'s built-in Document model:\n  \n    ```console\n    python manage.py migrate prose\n    ```\n\n4. **Include URLs**\n\n    You need to edit the main `urls.py` file of your Django project and include `prose.urls`:\n    \n    ```python\n    urlpatterns = [\n        path(\'admin/\', admin.site.urls),\n        # other urls ...\n        path("prose/", include("prose.urls")),\n    ]\n    ```\n\nNow, you are ready to go 🚀.\n\n## Usage\n\nThere are different ways to use Django prose according to your needs. We will examine all of them here.\n\n### Rendering rich-text in templates\n\nRich text content essentially is HTML. For this reason it needs to be manually marked as [`safe`](https://docs.djangoproject.com/en/4.2/ref/templates/builtins/#safe), when rendered in Django templates. Example:\n\n```django\n{{ document.content | safe}}\n```\n\n### Small rich-text content\n\nYou might want to add rich-text content in a model that is just a few characters (e.g. 140), like an excerpt from an article. In that case we suggest using the `RichTextField`. Example:\n\n```py\nfrom django.db import models\nfrom prose.fields import RichTextField\n\nclass Article(models.Model):\n    excerpt = RichTextField()\n```\n\nAs mentioned above, you need to mark the article excerpt as `safe`, in order to render it:\n\n```django\n<div class="article-excerpt">{{ article.excerpt | safe}}</div>\n```\n\n### Large rich-text content\n\nIn case you want to store large rich-text content, like the body of an article, which can span to quite a few thousand characters, we suggest you use the `AbstractDocument` model. This will save large rich-text content in a separate database table, which is better for performance. Example:\n\n```py\nfrom django.db import models\nfrom prose.fields import RichTextField\nfrom prose.models import AbstractDocument\n\nclass ArticleContent(AbstractDocument):\n    pass\n\nclass Article(models.Model):\n    excerpt = RichTextField()\n    body = models.OneToOneField(ArticleContent, on_delete=models.CASCADE)\n```\n\nSimilarly here as well, you need to mark the article\'s body as `safe`, in order to render it:\n\n```django\n<div class="article-body">{{ article.body.content | safe}}</div>\n```\n\n### Forms with rich-text editing\n\nYou can create forms for your Django Prose models, to provide rich-text editing functionality. In that case, you will also need to render `form.media`, to load Trix with its stylesheets.\n\n```django\n<form  method="POST" >\n  {% csrf_token %}\n  \n  {{ form.as_p }}\n  {{ form.media }}\n  \n  <button type="submit">Submit</button>\n</form>\n```\n\nThe same is true also, if you are rendering the forms field manually.\n\n### Attachments\n\nDjango Prose can also handle uploading attachments with drag and drop. To set this up, first you need to:\n\n- [x] Set up the `MEDIA_ROOT` and `MEDIA_URL` of your Django project (example in [`example/example/settings.py`](https://github.com/withlogicco/django-prose/blob/9e24cc794eae6db48818dd15a483d106d6a99da0/example/example/settings.py#L130-L131)))\n- [x] Include the Django Prose URLs (example in [`example/example/urls.py`](https://github.com/withlogicco/django-prose/blob/9e24cc794eae6db48818dd15a483d106d6a99da0/example/example/urls.py#L13-L14))\n- [x] (Optional) Set up a different Django storage to store your files (e.g. S3)\n\n### Full example\n\nYou can find a full example of a blog, built with Django Prose in the [`example`](./example/) directory.\n\n## 🔒 A note on security\n\nAs you can see in the examples above, what Django Prose does is provide you with a user friendly editor ([Trix](https://trix-editor.org/)) for your rich text content and then store it as HTML in your database. Since you will mark this HTML as safe in order to use it in your templates, it needs to be **sanitised**, before it gets stored in the database.\n\nFor this reason Django Prose is using [Bleach](https://bleach.readthedocs.io/en/latest/) to only allow the following tags and attributes:\n\n- **Allowed tags**: `p`, `ul`, `ol`, `li`, `strong`, `em`, `div`, `span`, `a`, `blockquote`, `pre`, `figure`, `figcaption`, `br`, `code`, `h1`, `h2`, `h3`, `h4`, `h5`, `h6`, `picture`, `source`, `img`\n- **Allowed attributes**: `alt`, `class`, `id`, `src`, `srcset`, `href`, `media`\n\n## Screenshots\n\n### Django Prose Documents in Django Admin\n\n![Django Prose Document in Django Admin](./docs/django-admin-prose-document.png)\n\n## Video tutorial\n\nIf you are more of a video person, you can watch our video showcasing how to **Create a blog using Django Prose** on YouTube\n\n[![Watch the video](https://img.youtube.com/vi/uICZjUpAbhQ/hqdefault.jpg)](https://youtu.be/uICZjUpAbhQ)\n\n## Real world use cases\n- **Remote Work Café**: Used to edit location pagess, like [Amsterdam | Remote Work Café](https://remotework.cafe/locations/amsterdam/)\n- In production by multiple clients of [LOGIC](https://withlogic.co), from small companies to the public sector.\n\nIf you are using Django Prose in your application too, feek free to open a [Pull Request](https://github.com/withlogicco/django-prose/pulls) to include it here. We would love to have it.\n\n## Development for Django Prose\n\nIf you plan to contribute code to Django Prose, this section is for you. All development tooling for Django Prose has been set up with Docker and Development Containers.\n\nTo get started run these commands in the provided order:\n\n```console\ndocker compose run --rm migrate\ndocker compose run --rm createsuperuser\ndocker compose up\n```\n\nIf you are using Visual Studio code, just open this repository in a container using the [`Dev Containers: Open Folder in Container`](https://code.visualstudio.com/docs/devcontainers/containers#_quick-start-open-an-existing-folder-in-a-container).\n\n---\n\n<p align="center">\n  <i>🦄 Built with <a href="https://withlogic.co/">LOGIC</a>. 🦄</i>\n</p>\n',
     'author': 'Paris Kasidiaris',
     'author_email': 'paris@withlogic.co',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/parisk/django-prose',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `django_prose-1.2.0/PKG-INFO` & `django_prose-1.2.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-prose
-Version: 1.2.0
+Version: 1.2.2
 Summary: Wonderful rich text for Django
 Home-page: https://github.com/parisk/django-prose
 License: MIT
 Author: Paris Kasidiaris
 Author-email: paris@withlogic.co
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -28,37 +28,57 @@
 
 - Python 3.8 or later
 - Django 3.2 or later
 - Bleach 4.0 or later
 
 ## Getting started
 
-To get started with Django Prose, first make sure to install it. We use and suggest using Poetry, although Pipenv and pip will work seamlessly as well
+To get started with Django Prose, all you need to do is follow **just four steps**.
 
-```console
-poetry add django-prose
-```
-
-Then, add `prose` in Django's installed apps (example: [`example/example/settings.py`](https://github.com/withlogicco/django-prose/blob/9e24cc794eae6db48818dd15a483d106d6a99da0/example/example/settings.py#L46)):
-
-```python
-INSTALLED_APPS = [
-    # Django stock apps (e.g. 'django.contrib.admin')
-
-    'prose',
-
-    # your application's apps
-]
-```
+1. **Install `django-prose`**
+    
+    We use and suggest using Poetry, although Pipenv and plain pip will work seamlessly as well
+    
+    ```console
+    poetry add django-prose
+    ```
+
+2. **Add to `INSTALLED_APPS`**
+    
+    Add `prose` in your Django project's installed apps (example: [`example/example/settings.py`](https://github.com/withlogicco/django-prose/blob/9e24cc794eae6db48818dd15a483d106d6a99da0/example/example/settings.py#L46)):
+    
+    ```python
+    INSTALLED_APPS = [
+        # Django stock apps (e.g. 'django.contrib.admin')
+    
+        'prose',
+    
+        # your application's apps
+    ]
+    ```
 
-Last, run migrations so you can use Django Prose's Document model:
+3. **Run migrations**
 
-```
-python manage.py migrate prose
-```
+    This is required so you can use Django Prose's built-in Document model:
+  
+    ```console
+    python manage.py migrate prose
+    ```
+
+4. **Include URLs**
+
+    You need to edit the main `urls.py` file of your Django project and include `prose.urls`:
+    
+    ```python
+    urlpatterns = [
+        path('admin/', admin.site.urls),
+        # other urls ...
+        path("prose/", include("prose.urls")),
+    ]
+    ```
 
 Now, you are ready to go 🚀.
 
 ## Usage
 
 There are different ways to use Django prose according to your needs. We will examine all of them here.
 
@@ -151,14 +171,20 @@
 
 ## Screenshots
 
 ### Django Prose Documents in Django Admin
 
 ![Django Prose Document in Django Admin](./docs/django-admin-prose-document.png)
 
+## Video tutorial
+
+If you are more of a video person, you can watch our video showcasing how to **Create a blog using Django Prose** on YouTube
+
+[![Watch the video](https://img.youtube.com/vi/uICZjUpAbhQ/hqdefault.jpg)](https://youtu.be/uICZjUpAbhQ)
+
 ## Real world use cases
 - **Remote Work Café**: Used to edit location pagess, like [Amsterdam | Remote Work Café](https://remotework.cafe/locations/amsterdam/)
 - In production by multiple clients of [LOGIC](https://withlogic.co), from small companies to the public sector.
 
 If you are using Django Prose in your application too, feek free to open a [Pull Request](https://github.com/withlogicco/django-prose/pulls) to include it here. We would love to have it.
 
 ## Development for Django Prose
```

