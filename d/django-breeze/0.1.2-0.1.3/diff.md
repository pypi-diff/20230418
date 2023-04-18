# Comparing `tmp/django_breeze-0.1.2.tar.gz` & `tmp/django_breeze-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_breeze-0.1.2.tar", max compression
+gzip compressed data, was "django_breeze-0.1.3.tar", max compression
```

## Comparing `django_breeze-0.1.2.tar` & `django_breeze-0.1.3.tar`

### file list

```diff
@@ -1,36 +1,38 @@
--rwxr-xr-x   0        0        0        0 2023-04-16 21:20:58.715528 django_breeze-0.1.2/LICENSE.md
--rwxr-xr-x   0        0        0     1467 2023-04-17 15:21:07.115933 django_breeze-0.1.2/README.md
--rwxr-xr-x   0        0        0     2509 2023-04-18 11:41:12.477541 django_breeze-0.1.2/django_breeze/__init__.py
--rwxr-xr-x   0        0        0      222 2023-04-18 11:37:34.673551 django_breeze-0.1.2/django_breeze/__main__.py
--rwxr-xr-x   0        0        0        0 2023-04-17 12:29:24.898719 django_breeze-0.1.2/django_breeze/core/__init__.py
--rwxr-xr-x   0        0        0     5859 2023-04-18 11:24:40.928705 django_breeze-0.1.2/django_breeze/core/management/__init__.py
--rwxr-xr-x   0        0        0      719 2023-04-17 12:34:24.726621 django_breeze-0.1.2/django_breeze/middleware.py
--rwxr-xr-x   0        0        0      208 2023-04-18 11:00:29.928394 django_breeze-0.1.2/django_breeze/scripts/django-breeze.py
--rwxr-xr-x   0        0        0      322 2023-04-17 16:02:16.221609 django_breeze-0.1.2/django_breeze/templates/react/.gitignore
--rwxr-xr-x   0        0        0      561 2023-04-17 15:38:34.137680 django_breeze-0.1.2/django_breeze/templates/react/package.json
--rwxr-xr-x   0        0        0       80 2023-04-11 16:36:16.193044 django_breeze-0.1.2/django_breeze/templates/react/postcss.config.js
--rwxr-xr-x   0        0        0      115 2023-04-17 15:55:52.679212 django_breeze-0.1.2/django_breeze/templates/react/src/Layout/SiteLayout.jsx
--rwxr-xr-x   0        0        0     4126 2023-04-11 12:18:56.391967 django_breeze-0.1.2/django_breeze/templates/react/src/assets/react.svg
--rwxr-xr-x   0        0        0       58 2023-04-17 15:26:59.812312 django_breeze-0.1.2/django_breeze/templates/react/src/index.css
--rwxr-xr-x   0        0        0      416 2023-04-17 15:48:56.251208 django_breeze-0.1.2/django_breeze/templates/react/src/index.html
--rwxr-xr-x   0        0        0      544 2023-04-17 15:28:13.267633 django_breeze-0.1.2/django_breeze/templates/react/src/main.jsx
--rwxr-xr-x   0        0        0      143 2023-04-17 15:42:26.503686 django_breeze-0.1.2/django_breeze/templates/react/src/pages/index.jsx
--rwxr-xr-x   0        0        0      174 2023-04-11 16:37:38.133133 django_breeze-0.1.2/django_breeze/templates/react/tailwind.config.js
--rwxr-xr-x   0        0        0      814 2023-04-16 23:40:08.446285 django_breeze-0.1.2/django_breeze/templates/react/vite.config.js
--rwxr-xr-x   0        0        0      322 2023-04-17 16:02:19.154142 django_breeze-0.1.2/django_breeze/templates/react_typescript/.gitignore
--rwxr-xr-x   0        0        0      577 2023-04-17 15:47:44.921698 django_breeze-0.1.2/django_breeze/templates/react_typescript/package.json
--rwxr-xr-x   0        0        0       80 2023-04-11 16:36:16.193044 django_breeze-0.1.2/django_breeze/templates/react_typescript/postcss.config.js
--rwxr-xr-x   0        0        0     1497 2023-04-17 15:44:03.080989 django_breeze-0.1.2/django_breeze/templates/react_typescript/public/vite.svg
--rwxr-xr-x   0        0        0      115 2023-04-17 15:55:31.215573 django_breeze-0.1.2/django_breeze/templates/react_typescript/src/Layout/SiteLayout.tsx
--rwxr-xr-x   0        0        0     4126 2023-04-17 15:44:03.128485 django_breeze-0.1.2/django_breeze/templates/react_typescript/src/assets/react.svg
--rwxr-xr-x   0        0        0       59 2023-04-17 15:51:58.938773 django_breeze-0.1.2/django_breeze/templates/react_typescript/src/index.css
--rwxr-xr-x   0        0        0      417 2023-04-17 15:49:05.983645 django_breeze-0.1.2/django_breeze/templates/react_typescript/src/index.html
--rwxr-xr-x   0        0        0      544 2023-04-17 15:56:37.832534 django_breeze-0.1.2/django_breeze/templates/react_typescript/src/main.tsx
--rwxr-xr-x   0        0        0      143 2023-04-17 15:53:30.284520 django_breeze-0.1.2/django_breeze/templates/react_typescript/src/pages/index.tsx
--rwxr-xr-x   0        0        0       38 2023-04-17 15:44:03.129843 django_breeze-0.1.2/django_breeze/templates/react_typescript/src/vite-env.d.ts
--rwxr-xr-x   0        0        0      174 2023-04-11 16:37:38.133133 django_breeze-0.1.2/django_breeze/templates/react_typescript/tailwind.config.js
--rwxr-xr-x   0        0        0      559 2023-04-17 15:44:03.150638 django_breeze-0.1.2/django_breeze/templates/react_typescript/tsconfig.json
--rwxr-xr-x   0        0        0      184 2023-04-17 15:44:03.151143 django_breeze-0.1.2/django_breeze/templates/react_typescript/tsconfig.node.json
--rwxr-xr-x   0        0        0      814 2023-04-17 15:57:23.467510 django_breeze-0.1.2/django_breeze/templates/react_typescript/vite.config.ts
--rwxr-xr-x   0        0        0      759 2023-04-18 11:52:39.535165 django_breeze-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2260 1970-01-01 00:00:00.000000 django_breeze-0.1.2/PKG-INFO
+-rwxr-xr-x   0        0        0        0 2023-04-16 21:20:58.715528 django_breeze-0.1.3/LICENSE.md
+-rwxr-xr-x   0        0        0     1467 2023-04-17 15:21:07.115933 django_breeze-0.1.3/README.md
+-rwxr-xr-x   0        0        0       61 2023-04-18 13:00:06.368911 django_breeze-0.1.3/django_breeze/__init__.py
+-rwxr-xr-x   0        0        0      222 2023-04-18 11:37:34.673551 django_breeze-0.1.3/django_breeze/__main__.py
+-rwxr-xr-x   0        0        0      246 2023-04-18 13:00:26.296628 django_breeze-0.1.3/django_breeze/apps.py
+-rwxr-xr-x   0        0        0        0 2023-04-17 12:29:24.898719 django_breeze-0.1.3/django_breeze/core/__init__.py
+-rwxr-xr-x   0        0        0     5859 2023-04-18 11:24:40.928705 django_breeze-0.1.3/django_breeze/core/management/__init__.py
+-rwxr-xr-x   0        0        0      719 2023-04-17 12:34:24.726621 django_breeze-0.1.3/django_breeze/middleware.py
+-rwxr-xr-x   0        0        0      232 2023-04-18 12:59:14.307894 django_breeze-0.1.3/django_breeze/scripts/django-breeze.py
+-rwxr-xr-x   0        0        0     2942 2023-04-18 12:55:52.287809 django_breeze-0.1.3/django_breeze/settings.py
+-rwxr-xr-x   0        0        0      322 2023-04-17 16:02:16.221609 django_breeze-0.1.3/django_breeze/templates/react/.gitignore
+-rwxr-xr-x   0        0        0      561 2023-04-17 15:38:34.137680 django_breeze-0.1.3/django_breeze/templates/react/package.json
+-rwxr-xr-x   0        0        0       80 2023-04-11 16:36:16.193044 django_breeze-0.1.3/django_breeze/templates/react/postcss.config.js
+-rwxr-xr-x   0        0        0      115 2023-04-17 15:55:52.679212 django_breeze-0.1.3/django_breeze/templates/react/src/Layout/SiteLayout.jsx
+-rwxr-xr-x   0        0        0     4126 2023-04-11 12:18:56.391967 django_breeze-0.1.3/django_breeze/templates/react/src/assets/react.svg
+-rwxr-xr-x   0        0        0       58 2023-04-17 15:26:59.812312 django_breeze-0.1.3/django_breeze/templates/react/src/index.css
+-rwxr-xr-x   0        0        0      416 2023-04-17 15:48:56.251208 django_breeze-0.1.3/django_breeze/templates/react/src/index.html
+-rwxr-xr-x   0        0        0      544 2023-04-17 15:28:13.267633 django_breeze-0.1.3/django_breeze/templates/react/src/main.jsx
+-rwxr-xr-x   0        0        0      143 2023-04-17 15:42:26.503686 django_breeze-0.1.3/django_breeze/templates/react/src/pages/index.jsx
+-rwxr-xr-x   0        0        0      174 2023-04-11 16:37:38.133133 django_breeze-0.1.3/django_breeze/templates/react/tailwind.config.js
+-rwxr-xr-x   0        0        0      814 2023-04-16 23:40:08.446285 django_breeze-0.1.3/django_breeze/templates/react/vite.config.js
+-rwxr-xr-x   0        0        0      322 2023-04-17 16:02:19.154142 django_breeze-0.1.3/django_breeze/templates/react_typescript/.gitignore
+-rwxr-xr-x   0        0        0      577 2023-04-17 15:47:44.921698 django_breeze-0.1.3/django_breeze/templates/react_typescript/package.json
+-rwxr-xr-x   0        0        0       80 2023-04-11 16:36:16.193044 django_breeze-0.1.3/django_breeze/templates/react_typescript/postcss.config.js
+-rwxr-xr-x   0        0        0     1497 2023-04-17 15:44:03.080989 django_breeze-0.1.3/django_breeze/templates/react_typescript/public/vite.svg
+-rwxr-xr-x   0        0        0      115 2023-04-17 15:55:31.215573 django_breeze-0.1.3/django_breeze/templates/react_typescript/src/Layout/SiteLayout.tsx
+-rwxr-xr-x   0        0        0     4126 2023-04-17 15:44:03.128485 django_breeze-0.1.3/django_breeze/templates/react_typescript/src/assets/react.svg
+-rwxr-xr-x   0        0        0       59 2023-04-17 15:51:58.938773 django_breeze-0.1.3/django_breeze/templates/react_typescript/src/index.css
+-rwxr-xr-x   0        0        0      417 2023-04-17 15:49:05.983645 django_breeze-0.1.3/django_breeze/templates/react_typescript/src/index.html
+-rwxr-xr-x   0        0        0      544 2023-04-17 15:56:37.832534 django_breeze-0.1.3/django_breeze/templates/react_typescript/src/main.tsx
+-rwxr-xr-x   0        0        0      143 2023-04-17 15:53:30.284520 django_breeze-0.1.3/django_breeze/templates/react_typescript/src/pages/index.tsx
+-rwxr-xr-x   0        0        0       38 2023-04-17 15:44:03.129843 django_breeze-0.1.3/django_breeze/templates/react_typescript/src/vite-env.d.ts
+-rwxr-xr-x   0        0        0      174 2023-04-11 16:37:38.133133 django_breeze-0.1.3/django_breeze/templates/react_typescript/tailwind.config.js
+-rwxr-xr-x   0        0        0      559 2023-04-17 15:44:03.150638 django_breeze-0.1.3/django_breeze/templates/react_typescript/tsconfig.json
+-rwxr-xr-x   0        0        0      184 2023-04-17 15:44:03.151143 django_breeze-0.1.3/django_breeze/templates/react_typescript/tsconfig.node.json
+-rwxr-xr-x   0        0        0      814 2023-04-17 15:57:23.467510 django_breeze-0.1.3/django_breeze/templates/react_typescript/vite.config.ts
+-rwxr-xr-x   0        0        0      763 2023-04-18 13:02:24.902686 django_breeze-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2260 1970-01-01 00:00:00.000000 django_breeze-0.1.3/PKG-INFO
```

### Comparing `django_breeze-0.1.2/README.md` & `django_breeze-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `django_breeze-0.1.2/django_breeze/__init__.py` & `django_breeze-0.1.3/django_breeze/settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,88 +1,92 @@
 from django.conf import settings as django_settings
 from inertia.settings import settings as inertia_settings
 from pathlib import Path
+import django
 
-BASE_DIR = getattr(django_settings, "BASE_DIR")
 
-MIDDLEWARES = [
-    "inertia.middleware.InertiaMiddleware",
-    # "django-breeze.django_breeze.middleware.inertia_share",
-]
-
-INSTALLED_APPS = [
-    "inertia",
-    "django_vite",
-]
-
-# Django Breeze Default Settings
-DJANGO_BREEZE: dict = {
-    "INERTIA": {
-        "LAYOUT": "index.html",
-        "SSR_URL": inertia_settings.INERTIA_SSR_URL,
-        "SSR_ENABLED": inertia_settings.INERTIA_SSR_ENABLED,
-        "JSON_ENCODER": inertia_settings.INERTIA_JSON_ENCODER,
-    },
-    "DJANGO_VITE": {
-        "DEV_MODE": getattr(django_settings, "DEBUG", True),
-        "SERVER_PROTOCOL": "http",
-        "DEV_SERVER_HOST": "localhost",
-        "DEV_SERVER_PORT": 5173,
-        "WS_CLIENT_URL": "@vite/client",
-        "ASSETS_PATH": Path(getattr(django_settings, "STATIC_PATH", "static")) / "dist",
-        "STATIC_URL_PREFIX": "",
-        "LEGACY_POLYFILLS_MOTIF": "legacy-polyfills",
-    },
-    "STATIC_ROOT": "static",
-    "CSRF_HEADER_NAME": "HTTP_X_XSRF_TOKEN",
-    "CSRF_COOKIE_NAME": "XSRF-TOKEN",
-}
-
-
-# Merge DJANGO_BREEZE and user-defined settings
-user_settings = getattr(django_settings, "DJANGO_BREEZE", {})
-
-
-def merge_dicts(*dicts):
-    """
-    Recursively merges dictionaries.
-    """
-    result = {}
-    for d in dicts:
-        for k, v in d.items():
-            if isinstance(v, dict):
-                result[k] = merge_dicts(result.get(k, {}), v)
-            else:
-                result[k] = v
-    return result
-
-
-merged_settings = merge_dicts(DJANGO_BREEZE, user_settings)
-
-
-def key_exist(key) -> bool:
-    return hasattr(django_settings, key) and getattr(django_settings, key) is not None
-
-
-settings = {}
-
-for key, value in merged_settings.items():
-    if isinstance(value, dict):
-        for sub_key, sub_value in value.items():
-            sub_key = f"{key}_{sub_key}"
-            if not key_exist(sub_key):
-                settings[sub_key] = sub_value
-    else:
-        if not key_exist(key):
-            settings[key] = value
-
-for key, value in settings.items():
-    setattr(django_settings, key, value)
-
-django_settings.TEMPLATES[0]["DIRS"].append(Path(BASE_DIR) / "src/")
-
-for app in INSTALLED_APPS:
-    django_settings.INSTALLED_APPS.append(app)
-
-for middleware in MIDDLEWARES:
-    django_settings.MIDDLEWARE.append(middleware)
-# django_settings.STATICFILES_DIRS.append(settings.DJANGO_VITE_ASSETS_PATH)
+def initialize() -> None:
+    """Initialize all neccessary django, inertia and django-vite settings"""
+    BASE_DIR = getattr(django_settings, "BASE_DIR")
+
+    MIDDLEWARES = [
+        "inertia.middleware.InertiaMiddleware",
+        # "django-breeze.django_breeze.middleware.inertia_share",
+    ]
+
+    INSTALLED_APPS = [
+        "inertia",
+        "django_vite",
+    ]
+
+    # Django Breeze Default Settings
+    DJANGO_BREEZE: dict = {
+        "INERTIA": {
+            "LAYOUT": "index.html",
+            "SSR_URL": inertia_settings.INERTIA_SSR_URL,
+            "SSR_ENABLED": inertia_settings.INERTIA_SSR_ENABLED,
+            "JSON_ENCODER": inertia_settings.INERTIA_JSON_ENCODER,
+        },
+        "DJANGO_VITE": {
+            "DEV_MODE": getattr(django_settings, "DEBUG", True),
+            "SERVER_PROTOCOL": "http",
+            "DEV_SERVER_HOST": "localhost",
+            "DEV_SERVER_PORT": 5173,
+            "WS_CLIENT_URL": "@vite/client",
+            "ASSETS_PATH": Path(getattr(django_settings, "STATIC_PATH", "static"))
+            / "dist",
+            "STATIC_URL_PREFIX": "",
+            "LEGACY_POLYFILLS_MOTIF": "legacy-polyfills",
+        },
+        "STATIC_ROOT": "static",
+        "CSRF_HEADER_NAME": "HTTP_X_XSRF_TOKEN",
+        "CSRF_COOKIE_NAME": "XSRF-TOKEN",
+    }
+
+    # Merge DJANGO_BREEZE and user-defined settings
+    user_settings = getattr(django_settings, "DJANGO_BREEZE", {})
+
+    def merge_dicts(*dicts):
+        """
+        Recursively merges dictionaries.
+        """
+        result = {}
+        for d in dicts:
+            for k, v in d.items():
+                if isinstance(v, dict):
+                    result[k] = merge_dicts(result.get(k, {}), v)
+                else:
+                    result[k] = v
+        return result
+
+    merged_settings = merge_dicts(DJANGO_BREEZE, user_settings)
+
+    def key_exist(key) -> bool:
+        return (
+            hasattr(django_settings, key) and getattr(django_settings, key) is not None
+        )
+
+    settings = {}
+
+    for key, value in merged_settings.items():
+        if isinstance(value, dict):
+            for sub_key, sub_value in value.items():
+                sub_key = f"{key}_{sub_key}"
+                if not key_exist(sub_key):
+                    settings[sub_key] = sub_value
+        else:
+            if not key_exist(key):
+                settings[key] = value
+
+    for key, value in settings.items():
+        setattr(django_settings, key, value)
+
+    django_settings.TEMPLATES[0]["DIRS"].append(Path(BASE_DIR) / "src/")
+
+    for app in INSTALLED_APPS:
+        django_settings.INSTALLED_APPS.append(app)
+
+    for middleware in MIDDLEWARES:
+        django_settings.MIDDLEWARE.append(middleware)
+    # django_settings.STATICFILES_DIRS.append(settings.DJANGO_VITE_ASSETS_PATH)
+
+    django.setup()
```

### Comparing `django_breeze-0.1.2/django_breeze/core/management/__init__.py` & `django_breeze-0.1.3/django_breeze/core/management/__init__.py`

 * *Files identical despite different names*

### Comparing `django_breeze-0.1.2/django_breeze/middleware.py` & `django_breeze-0.1.3/django_breeze/middleware.py`

 * *Files identical despite different names*

### Comparing `django_breeze-0.1.2/django_breeze/templates/react/package.json` & `django_breeze-0.1.3/django_breeze/templates/react/package.json`

 * *Files identical despite different names*

### Comparing `django_breeze-0.1.2/django_breeze/templates/react/src/assets/react.svg` & `django_breeze-0.1.3/django_breeze/templates/react/src/assets/react.svg`

 * *Files identical despite different names*

### Comparing `django_breeze-0.1.2/django_breeze/templates/react/src/main.jsx` & `django_breeze-0.1.3/django_breeze/templates/react/src/main.jsx`

 * *Files identical despite different names*

### Comparing `django_breeze-0.1.2/django_breeze/templates/react/vite.config.js` & `django_breeze-0.1.3/django_breeze/templates/react/vite.config.js`

 * *Files identical despite different names*

### Comparing `django_breeze-0.1.2/django_breeze/templates/react_typescript/package.json` & `django_breeze-0.1.3/django_breeze/templates/react_typescript/package.json`

 * *Files identical despite different names*

### Comparing `django_breeze-0.1.2/django_breeze/templates/react_typescript/public/vite.svg` & `django_breeze-0.1.3/django_breeze/templates/react_typescript/public/vite.svg`

 * *Files identical despite different names*

### Comparing `django_breeze-0.1.2/django_breeze/templates/react_typescript/src/assets/react.svg` & `django_breeze-0.1.3/django_breeze/templates/react_typescript/src/assets/react.svg`

 * *Files identical despite different names*

### Comparing `django_breeze-0.1.2/django_breeze/templates/react_typescript/src/main.tsx` & `django_breeze-0.1.3/django_breeze/templates/react_typescript/src/main.tsx`

 * *Files identical despite different names*

### Comparing `django_breeze-0.1.2/django_breeze/templates/react_typescript/tsconfig.json` & `django_breeze-0.1.3/django_breeze/templates/react_typescript/tsconfig.json`

 * *Files identical despite different names*

### Comparing `django_breeze-0.1.2/django_breeze/templates/react_typescript/vite.config.ts` & `django_breeze-0.1.3/django_breeze/templates/react_typescript/vite.config.ts`

 * *Files identical despite different names*

### Comparing `django_breeze-0.1.2/pyproject.toml` & `django_breeze-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-breeze"
-version = "0.1.2"
+version = "0.1.3"
 description = "Django Breeze provides a minimal and simple starting point for building a Django application with Inertia.js Styled with Tailwind CSS."
 keywords = ["react", "django", "vue", "inertia", "vite"]
 authors = ["louxsdon <louisayivi.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/Louxsdon/django-breeze"
 packages = [{include = "django_breeze"}]
@@ -15,12 +15,12 @@
 inertia-django = "^0.5.2"
 
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.2.0"
 
 [tool.poetry.scripts]
-django-breeze = 'django_breeze.scripts.django-breeze'
+django-breeze = 'django_breeze.scripts.django-breeze:run'
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `django_breeze-0.1.2/PKG-INFO` & `django_breeze-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-breeze
-Version: 0.1.2
+Version: 0.1.3
 Summary: Django Breeze provides a minimal and simple starting point for building a Django application with Inertia.js Styled with Tailwind CSS.
 Home-page: https://github.com/Louxsdon/django-breeze
 License: MIT
 Keywords: react,django,vue,inertia,vite
 Author: louxsdon
 Author-email: louisayivi.dev@gmail.com
 Requires-Python: >=3.10,<4.0
```

