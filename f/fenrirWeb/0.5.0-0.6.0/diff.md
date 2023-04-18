# Comparing `tmp/fenrirWeb-0.5.0.tar.gz` & `tmp/fenrirWeb-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fenrirWeb-0.5.0.tar", last modified: Sun Apr 16 18:36:43 2023, max compression
+gzip compressed data, was "fenrirWeb-0.6.0.tar", last modified: Tue Apr 18 21:08:02 2023, max compression
```

## Comparing `fenrirWeb-0.5.0.tar` & `fenrirWeb-0.6.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 hannes    (1000) users      (100)        0 2023-04-16 18:36:43.928919 fenrirWeb-0.5.0/
--rw-r--r--   0 hannes    (1000) users      (100)    18092 2023-04-10 10:56:55.000000 fenrirWeb-0.5.0/LICENSE
--rw-r--r--   0 hannes    (1000) users      (100)       80 2023-04-10 10:56:55.000000 fenrirWeb-0.5.0/MANIFEST.in
--rw-r--r--   0 hannes    (1000) users      (100)      340 2023-04-16 18:36:43.928919 fenrirWeb-0.5.0/PKG-INFO
--rw-r--r--   0 hannes    (1000) users      (100)      765 2023-04-10 10:59:05.000000 fenrirWeb-0.5.0/README.md
-drwxr-xr-x   0 hannes    (1000) users      (100)        0 2023-04-16 18:36:43.924919 fenrirWeb-0.5.0/fenrirWeb/
--rw-r--r--   0 hannes    (1000) users      (100)       22 2023-04-16 18:34:53.000000 fenrirWeb-0.5.0/fenrirWeb/__init__.py
--rw-r--r--   0 hannes    (1000) users      (100)    16875 2023-04-11 21:45:56.000000 fenrirWeb-0.5.0/fenrirWeb/lib.py
--rw-r--r--   0 hannes    (1000) users      (100)     1052 2023-04-10 10:56:55.000000 fenrirWeb-0.5.0/fenrirWeb/main.py
-drwxr-xr-x   0 hannes    (1000) users      (100)        0 2023-04-16 18:36:43.928919 fenrirWeb-0.5.0/fenrirWeb/static/
--rw-r--r--   0 hannes    (1000) users      (100)    80420 2023-04-10 10:56:55.000000 fenrirWeb-0.5.0/fenrirWeb/static/bootstrap.bundle.min.js
--rw-r--r--   0 hannes    (1000) users      (100)   194901 2023-04-10 10:56:55.000000 fenrirWeb-0.5.0/fenrirWeb/static/bootstrap.min.css
--rw-r--r--   0 hannes    (1000) users      (100)    60404 2023-04-10 10:56:55.000000 fenrirWeb-0.5.0/fenrirWeb/static/bootstrap.min.js
--rw-r--r--   0 hannes    (1000) users      (100)     9369 2023-04-10 10:56:55.000000 fenrirWeb-0.5.0/fenrirWeb/static/disabled.png
--rw-r--r--   0 hannes    (1000) users      (100)    20270 2023-04-10 10:56:55.000000 fenrirWeb-0.5.0/fenrirWeb/static/disabled.svg
--rw-r--r--   0 hannes    (1000) users      (100)     8004 2023-04-10 10:56:55.000000 fenrirWeb-0.5.0/fenrirWeb/static/enabled.png
--rw-r--r--   0 hannes    (1000) users      (100)    28344 2023-04-10 10:56:55.000000 fenrirWeb-0.5.0/fenrirWeb/static/enabled.svg
--rw-r--r--   0 hannes    (1000) users      (100)    93062 2023-04-10 10:56:55.000000 fenrirWeb-0.5.0/fenrirWeb/static/favicon.ico
--rw-r--r--   0 hannes    (1000) users      (100)    15194 2023-04-16 18:30:17.000000 fenrirWeb-0.5.0/fenrirWeb/static/fenrir.js
--rw-r--r--   0 hannes    (1000) users      (100)     2104 2023-04-10 10:56:55.000000 fenrirWeb-0.5.0/fenrirWeb/static/settings.png
--rw-r--r--   0 hannes    (1000) users      (100)     9046 2023-04-10 10:56:55.000000 fenrirWeb-0.5.0/fenrirWeb/view_config.py
--rw-r--r--   0 hannes    (1000) users      (100)     3152 2023-04-10 10:56:55.000000 fenrirWeb-0.5.0/fenrirWeb/view_main.py
-drwxr-xr-x   0 hannes    (1000) users      (100)        0 2023-04-16 18:36:43.928919 fenrirWeb-0.5.0/fenrirWeb/views/
--rw-r--r--   0 hannes    (1000) users      (100)     3143 2023-04-16 16:41:07.000000 fenrirWeb-0.5.0/fenrirWeb/views/changepassword.tpl
--rw-r--r--   0 hannes    (1000) users      (100)     2736 2023-04-16 16:31:13.000000 fenrirWeb-0.5.0/fenrirWeb/views/createpassword.tpl
--rw-r--r--   0 hannes    (1000) users      (100)     3064 2023-04-10 10:56:55.000000 fenrirWeb-0.5.0/fenrirWeb/views/index.tpl
--rw-r--r--   0 hannes    (1000) users      (100)     1697 2023-04-10 10:56:55.000000 fenrirWeb-0.5.0/fenrirWeb/views/mappinginput.tpl
--rw-r--r--   0 hannes    (1000) users      (100)      939 2023-04-10 10:56:55.000000 fenrirWeb-0.5.0/fenrirWeb/views/navbar.tpl
--rw-r--r--   0 hannes    (1000) users      (100)     8286 2023-04-10 10:56:55.000000 fenrirWeb-0.5.0/fenrirWeb/views/settings.tpl
--rw-r--r--   0 hannes    (1000) users      (100)     2501 2023-04-10 10:56:55.000000 fenrirWeb-0.5.0/fenrirWeb/views/vpninput.tpl
-drwxr-xr-x   0 hannes    (1000) users      (100)        0 2023-04-16 18:36:43.928919 fenrirWeb-0.5.0/fenrirWeb.egg-info/
--rw-r--r--   0 hannes    (1000) users      (100)      340 2023-04-16 18:36:43.000000 fenrirWeb-0.5.0/fenrirWeb.egg-info/PKG-INFO
--rw-r--r--   0 hannes    (1000) users      (100)      903 2023-04-16 18:36:43.000000 fenrirWeb-0.5.0/fenrirWeb.egg-info/SOURCES.txt
--rw-r--r--   0 hannes    (1000) users      (100)        1 2023-04-16 18:36:43.000000 fenrirWeb-0.5.0/fenrirWeb.egg-info/dependency_links.txt
--rw-r--r--   0 hannes    (1000) users      (100)       50 2023-04-16 18:36:43.000000 fenrirWeb-0.5.0/fenrirWeb.egg-info/entry_points.txt
--rw-r--r--   0 hannes    (1000) users      (100)        1 2023-04-10 10:16:52.000000 fenrirWeb-0.5.0/fenrirWeb.egg-info/not-zip-safe
--rw-r--r--   0 hannes    (1000) users      (100)       32 2023-04-16 18:36:43.000000 fenrirWeb-0.5.0/fenrirWeb.egg-info/requires.txt
--rw-r--r--   0 hannes    (1000) users      (100)       10 2023-04-16 18:36:43.000000 fenrirWeb-0.5.0/fenrirWeb.egg-info/top_level.txt
--rw-r--r--   0 hannes    (1000) users      (100)       38 2023-04-16 18:36:43.928919 fenrirWeb-0.5.0/setup.cfg
--rw-r--r--   0 hannes    (1000) users      (100)      693 2023-04-10 10:56:55.000000 fenrirWeb-0.5.0/setup.py
+drwxr-xr-x   0 hannes    (1000) users      (100)        0 2023-04-18 21:08:02.069570 fenrirWeb-0.6.0/
+-rw-r--r--   0 hannes    (1000) users      (100)    18092 2023-04-10 10:56:55.000000 fenrirWeb-0.6.0/LICENSE
+-rw-r--r--   0 hannes    (1000) users      (100)       80 2023-04-10 10:56:55.000000 fenrirWeb-0.6.0/MANIFEST.in
+-rw-r--r--   0 hannes    (1000) users      (100)      340 2023-04-18 21:08:02.069570 fenrirWeb-0.6.0/PKG-INFO
+-rw-r--r--   0 hannes    (1000) users      (100)      765 2023-04-10 10:59:05.000000 fenrirWeb-0.6.0/README.md
+drwxr-xr-x   0 hannes    (1000) users      (100)        0 2023-04-18 21:08:02.069570 fenrirWeb-0.6.0/fenrirWeb/
+-rw-r--r--   0 hannes    (1000) users      (100)       22 2023-04-18 21:06:58.000000 fenrirWeb-0.6.0/fenrirWeb/__init__.py
+-rw-r--r--   0 hannes    (1000) users      (100)    16875 2023-04-11 21:45:56.000000 fenrirWeb-0.6.0/fenrirWeb/lib.py
+-rw-r--r--   0 hannes    (1000) users      (100)     1052 2023-04-10 10:56:55.000000 fenrirWeb-0.6.0/fenrirWeb/main.py
+drwxr-xr-x   0 hannes    (1000) users      (100)        0 2023-04-18 21:08:02.069570 fenrirWeb-0.6.0/fenrirWeb/static/
+-rw-r--r--   0 hannes    (1000) users      (100)    80420 2023-04-10 10:56:55.000000 fenrirWeb-0.6.0/fenrirWeb/static/bootstrap.bundle.min.js
+-rw-r--r--   0 hannes    (1000) users      (100)   194901 2023-04-10 10:56:55.000000 fenrirWeb-0.6.0/fenrirWeb/static/bootstrap.min.css
+-rw-r--r--   0 hannes    (1000) users      (100)    60404 2023-04-10 10:56:55.000000 fenrirWeb-0.6.0/fenrirWeb/static/bootstrap.min.js
+-rw-r--r--   0 hannes    (1000) users      (100)     9369 2023-04-10 10:56:55.000000 fenrirWeb-0.6.0/fenrirWeb/static/disabled.png
+-rw-r--r--   0 hannes    (1000) users      (100)    20270 2023-04-10 10:56:55.000000 fenrirWeb-0.6.0/fenrirWeb/static/disabled.svg
+-rw-r--r--   0 hannes    (1000) users      (100)     8004 2023-04-10 10:56:55.000000 fenrirWeb-0.6.0/fenrirWeb/static/enabled.png
+-rw-r--r--   0 hannes    (1000) users      (100)    28344 2023-04-10 10:56:55.000000 fenrirWeb-0.6.0/fenrirWeb/static/enabled.svg
+-rw-r--r--   0 hannes    (1000) users      (100)    93062 2023-04-10 10:56:55.000000 fenrirWeb-0.6.0/fenrirWeb/static/favicon.ico
+-rw-r--r--   0 hannes    (1000) users      (100)    15986 2023-04-18 21:03:38.000000 fenrirWeb-0.6.0/fenrirWeb/static/fenrir.js
+-rw-r--r--   0 hannes    (1000) users      (100)     2104 2023-04-10 10:56:55.000000 fenrirWeb-0.6.0/fenrirWeb/static/settings.png
+-rw-r--r--   0 hannes    (1000) users      (100)     9046 2023-04-10 10:56:55.000000 fenrirWeb-0.6.0/fenrirWeb/view_config.py
+-rw-r--r--   0 hannes    (1000) users      (100)     3152 2023-04-10 10:56:55.000000 fenrirWeb-0.6.0/fenrirWeb/view_main.py
+drwxr-xr-x   0 hannes    (1000) users      (100)        0 2023-04-18 21:08:02.069570 fenrirWeb-0.6.0/fenrirWeb/views/
+-rw-r--r--   0 hannes    (1000) users      (100)     3143 2023-04-16 16:41:07.000000 fenrirWeb-0.6.0/fenrirWeb/views/changepassword.tpl
+-rw-r--r--   0 hannes    (1000) users      (100)     2736 2023-04-16 16:31:13.000000 fenrirWeb-0.6.0/fenrirWeb/views/createpassword.tpl
+-rw-r--r--   0 hannes    (1000) users      (100)     3064 2023-04-10 10:56:55.000000 fenrirWeb-0.6.0/fenrirWeb/views/index.tpl
+-rw-r--r--   0 hannes    (1000) users      (100)     1697 2023-04-10 10:56:55.000000 fenrirWeb-0.6.0/fenrirWeb/views/mappinginput.tpl
+-rw-r--r--   0 hannes    (1000) users      (100)      939 2023-04-10 10:56:55.000000 fenrirWeb-0.6.0/fenrirWeb/views/navbar.tpl
+-rw-r--r--   0 hannes    (1000) users      (100)     8286 2023-04-10 10:56:55.000000 fenrirWeb-0.6.0/fenrirWeb/views/settings.tpl
+-rw-r--r--   0 hannes    (1000) users      (100)     2768 2023-04-18 20:40:56.000000 fenrirWeb-0.6.0/fenrirWeb/views/vpninput.tpl
+drwxr-xr-x   0 hannes    (1000) users      (100)        0 2023-04-18 21:08:02.069570 fenrirWeb-0.6.0/fenrirWeb.egg-info/
+-rw-r--r--   0 hannes    (1000) users      (100)      340 2023-04-18 21:08:02.000000 fenrirWeb-0.6.0/fenrirWeb.egg-info/PKG-INFO
+-rw-r--r--   0 hannes    (1000) users      (100)      903 2023-04-18 21:08:02.000000 fenrirWeb-0.6.0/fenrirWeb.egg-info/SOURCES.txt
+-rw-r--r--   0 hannes    (1000) users      (100)        1 2023-04-18 21:08:02.000000 fenrirWeb-0.6.0/fenrirWeb.egg-info/dependency_links.txt
+-rw-r--r--   0 hannes    (1000) users      (100)       50 2023-04-18 21:08:02.000000 fenrirWeb-0.6.0/fenrirWeb.egg-info/entry_points.txt
+-rw-r--r--   0 hannes    (1000) users      (100)        1 2023-04-10 10:16:52.000000 fenrirWeb-0.6.0/fenrirWeb.egg-info/not-zip-safe
+-rw-r--r--   0 hannes    (1000) users      (100)       32 2023-04-18 21:08:02.000000 fenrirWeb-0.6.0/fenrirWeb.egg-info/requires.txt
+-rw-r--r--   0 hannes    (1000) users      (100)       10 2023-04-18 21:08:02.000000 fenrirWeb-0.6.0/fenrirWeb.egg-info/top_level.txt
+-rw-r--r--   0 hannes    (1000) users      (100)       38 2023-04-18 21:08:02.069570 fenrirWeb-0.6.0/setup.cfg
+-rw-r--r--   0 hannes    (1000) users      (100)      693 2023-04-10 10:56:55.000000 fenrirWeb-0.6.0/setup.py
```

### Comparing `fenrirWeb-0.5.0/LICENSE` & `fenrirWeb-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.5.0/README.md` & `fenrirWeb-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.5.0/fenrirWeb/lib.py` & `fenrirWeb-0.6.0/fenrirWeb/lib.py`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.5.0/fenrirWeb/main.py` & `fenrirWeb-0.6.0/fenrirWeb/main.py`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.5.0/fenrirWeb/static/bootstrap.bundle.min.js` & `fenrirWeb-0.6.0/fenrirWeb/static/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.5.0/fenrirWeb/static/bootstrap.min.css` & `fenrirWeb-0.6.0/fenrirWeb/static/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.5.0/fenrirWeb/static/bootstrap.min.js` & `fenrirWeb-0.6.0/fenrirWeb/static/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.5.0/fenrirWeb/static/disabled.png` & `fenrirWeb-0.6.0/fenrirWeb/static/disabled.png`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.5.0/fenrirWeb/static/disabled.svg` & `fenrirWeb-0.6.0/fenrirWeb/static/disabled.svg`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.5.0/fenrirWeb/static/enabled.png` & `fenrirWeb-0.6.0/fenrirWeb/static/enabled.png`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.5.0/fenrirWeb/static/enabled.svg` & `fenrirWeb-0.6.0/fenrirWeb/static/enabled.svg`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.5.0/fenrirWeb/static/favicon.ico` & `fenrirWeb-0.6.0/fenrirWeb/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.5.0/fenrirWeb/static/fenrir.js` & `fenrirWeb-0.6.0/fenrirWeb/static/fenrir.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -265,14 +265,15 @@
         }
         var el = document.getElementById("vpnconfigismodification");
         if (el)
             el.outerHTML = "";
         return;
     }
 
+    disableVPNInput();
     // modifying existing configuration
     data = {
         profilename: name,
         completeData: true
     }
     getData('/getvpnconfigurations', data).then(resp => resp.json()).then(resp => {
         for (const [key, value] of Object.entries(resp['profile0'])) {
@@ -293,14 +294,15 @@
         var el = document.getElementById("vpnconfigismodification");
         if (!el) {
             var input = document.createElement('input');
             input.setAttribute('type', 'hidden');
             input.setAttribute('id', 'vpnconfigismodification');
             document.getElementById("vpnconfigform").appendChild(input);
         }
+        enableVPNInput();
     })
 }
 
 function refreshMapping() {
     tablebody = document.getElementById('vpnmappingtablebody')
     tablebody.innerHTML = `<tr id="vpntableloader">
 							<td></td><td></td><td>
@@ -401,14 +403,34 @@
             option.value = value;
             option.text = value;
             nameselect.appendChild(option);
         }
     }
 }
 
+function disableVPNInput() {
+    var configForm = document.getElementById("vpnconfigform");
+    document.getElementById("loading").removeAttribute("hidden");
+    document.getElementById("vpnconfigsubmit").disabled = true;
+    var inputElements = configForm.querySelectorAll("input, textarea");
+    for (var i = 0; i < inputElements.length; i++) {
+        inputElements[i].disabled = true;
+    }
+}
+
+function enableVPNInput() {
+    var configForm = document.getElementById("vpnconfigform");
+    document.getElementById("loading").setAttribute("hidden", true);
+    document.getElementById("vpnconfigsubmit").disabled = false;
+    var inputElements = configForm.querySelectorAll("input, textarea");
+    for (var i = 0; i < inputElements.length; i++) {
+        inputElements[i].disabled = false;
+    }
+}
+
 function changePasswordModal(event) {
     document.getElementById('chvpnpasswordform').classList.remove("was-validated");
     document.getElementById('chvpnpassword').value = '';
     document.getElementById('chcurrentpassword').value = '';
     document.getElementById('chrepeatvpnpassword').value = '';
     getData('/ispasswordusedforencryption', {}).then(resp => resp.json()).then(resp => {
         document.getElementById('chisencryptionpassword').checked = resp['checked']
```

### Comparing `fenrirWeb-0.5.0/fenrirWeb/static/settings.png` & `fenrirWeb-0.6.0/fenrirWeb/static/settings.png`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.5.0/fenrirWeb/view_config.py` & `fenrirWeb-0.6.0/fenrirWeb/view_config.py`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.5.0/fenrirWeb/view_main.py` & `fenrirWeb-0.6.0/fenrirWeb/view_main.py`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.5.0/fenrirWeb/views/changepassword.tpl` & `fenrirWeb-0.6.0/fenrirWeb/views/changepassword.tpl`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.5.0/fenrirWeb/views/createpassword.tpl` & `fenrirWeb-0.6.0/fenrirWeb/views/createpassword.tpl`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.5.0/fenrirWeb/views/index.tpl` & `fenrirWeb-0.6.0/fenrirWeb/views/index.tpl`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.5.0/fenrirWeb/views/mappinginput.tpl` & `fenrirWeb-0.6.0/fenrirWeb/views/mappinginput.tpl`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.5.0/fenrirWeb/views/navbar.tpl` & `fenrirWeb-0.6.0/fenrirWeb/views/navbar.tpl`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.5.0/fenrirWeb/views/settings.tpl` & `fenrirWeb-0.6.0/fenrirWeb/views/settings.tpl`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.5.0/fenrirWeb/views/vpninput.tpl` & `fenrirWeb-0.6.0/fenrirWeb/views/vpninput.tpl`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 <div class="container">
     <form class="needs-validation" id="vpnconfigform" onsubmit="handleVPNConfigSubmit();" novalidate>
+        <div class="overlay" id="loading" hidden>
+            <div class="d-flex justify-content-center">
+              <div class="spinner-border" role="status" >
+                <span class="sr-only"></span>
+              </div>
+            </div>
+          </div>
         <div class="row">
             <div class="col-12 mb-3 form-floating has-validation">
                 <input type="text" class="form-control" id="profilename" placeholder="Profile Name" required>
                 <label for="profileName" class="form-label mx-2">Profilename</label>
                 <div class="invalid-feedback">Please choose a Profilename.</div>
             </div>
             <div class="col-12 mb-3 form-floating">
```

### Comparing `fenrirWeb-0.5.0/fenrirWeb.egg-info/SOURCES.txt` & `fenrirWeb-0.6.0/fenrirWeb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.5.0/setup.py` & `fenrirWeb-0.6.0/setup.py`

 * *Files identical despite different names*

