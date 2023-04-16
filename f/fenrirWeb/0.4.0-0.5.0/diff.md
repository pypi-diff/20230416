# Comparing `tmp/fenrirWeb-0.4.0.tar.gz` & `tmp/fenrirWeb-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fenrirWeb-0.4.0.tar", last modified: Wed Apr 12 19:51:06 2023, max compression
+gzip compressed data, was "fenrirWeb-0.5.0.tar", last modified: Sun Apr 16 18:36:43 2023, max compression
```

## Comparing `fenrirWeb-0.4.0.tar` & `fenrirWeb-0.5.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 hannes    (1000) users      (100)        0 2023-04-12 19:51:06.145783 fenrirWeb-0.4.0/
--rw-r--r--   0 hannes    (1000) users      (100)    18092 2023-04-10 10:56:55.000000 fenrirWeb-0.4.0/LICENSE
--rw-r--r--   0 hannes    (1000) users      (100)       80 2023-04-10 10:56:55.000000 fenrirWeb-0.4.0/MANIFEST.in
--rw-r--r--   0 hannes    (1000) users      (100)      340 2023-04-12 19:51:06.145783 fenrirWeb-0.4.0/PKG-INFO
--rw-r--r--   0 hannes    (1000) users      (100)      765 2023-04-10 10:59:05.000000 fenrirWeb-0.4.0/README.md
-drwxr-xr-x   0 hannes    (1000) users      (100)        0 2023-04-12 19:51:06.137783 fenrirWeb-0.4.0/fenrirWeb/
--rw-r--r--   0 hannes    (1000) users      (100)       22 2023-04-11 19:55:18.000000 fenrirWeb-0.4.0/fenrirWeb/__init__.py
--rw-r--r--   0 hannes    (1000) users      (100)    16875 2023-04-11 21:45:56.000000 fenrirWeb-0.4.0/fenrirWeb/lib.py
--rw-r--r--   0 hannes    (1000) users      (100)     1052 2023-04-10 10:56:55.000000 fenrirWeb-0.4.0/fenrirWeb/main.py
-drwxr-xr-x   0 hannes    (1000) users      (100)        0 2023-04-12 19:51:06.141783 fenrirWeb-0.4.0/fenrirWeb/static/
--rw-r--r--   0 hannes    (1000) users      (100)    80420 2023-04-10 10:56:55.000000 fenrirWeb-0.4.0/fenrirWeb/static/bootstrap.bundle.min.js
--rw-r--r--   0 hannes    (1000) users      (100)   194901 2023-04-10 10:56:55.000000 fenrirWeb-0.4.0/fenrirWeb/static/bootstrap.min.css
--rw-r--r--   0 hannes    (1000) users      (100)    60404 2023-04-10 10:56:55.000000 fenrirWeb-0.4.0/fenrirWeb/static/bootstrap.min.js
--rw-r--r--   0 hannes    (1000) users      (100)     9369 2023-04-10 10:56:55.000000 fenrirWeb-0.4.0/fenrirWeb/static/disabled.png
--rw-r--r--   0 hannes    (1000) users      (100)    20270 2023-04-10 10:56:55.000000 fenrirWeb-0.4.0/fenrirWeb/static/disabled.svg
--rw-r--r--   0 hannes    (1000) users      (100)     8004 2023-04-10 10:56:55.000000 fenrirWeb-0.4.0/fenrirWeb/static/enabled.png
--rw-r--r--   0 hannes    (1000) users      (100)    28344 2023-04-10 10:56:55.000000 fenrirWeb-0.4.0/fenrirWeb/static/enabled.svg
--rw-r--r--   0 hannes    (1000) users      (100)    93062 2023-04-10 10:56:55.000000 fenrirWeb-0.4.0/fenrirWeb/static/favicon.ico
--rw-r--r--   0 hannes    (1000) users      (100)    13258 2023-04-10 10:56:55.000000 fenrirWeb-0.4.0/fenrirWeb/static/fenrir.js
--rw-r--r--   0 hannes    (1000) users      (100)     2104 2023-04-10 10:56:55.000000 fenrirWeb-0.4.0/fenrirWeb/static/settings.png
--rw-r--r--   0 hannes    (1000) users      (100)     9046 2023-04-10 10:56:55.000000 fenrirWeb-0.4.0/fenrirWeb/view_config.py
--rw-r--r--   0 hannes    (1000) users      (100)     3152 2023-04-10 10:56:55.000000 fenrirWeb-0.4.0/fenrirWeb/view_main.py
-drwxr-xr-x   0 hannes    (1000) users      (100)        0 2023-04-12 19:51:06.145783 fenrirWeb-0.4.0/fenrirWeb/views/
--rw-r--r--   0 hannes    (1000) users      (100)     3046 2023-04-10 10:56:55.000000 fenrirWeb-0.4.0/fenrirWeb/views/changepassword.tpl
--rw-r--r--   0 hannes    (1000) users      (100)     2547 2023-04-10 10:56:55.000000 fenrirWeb-0.4.0/fenrirWeb/views/createpassword.tpl
--rw-r--r--   0 hannes    (1000) users      (100)     3064 2023-04-10 10:56:55.000000 fenrirWeb-0.4.0/fenrirWeb/views/index.tpl
--rw-r--r--   0 hannes    (1000) users      (100)     1697 2023-04-10 10:56:55.000000 fenrirWeb-0.4.0/fenrirWeb/views/mappinginput.tpl
--rw-r--r--   0 hannes    (1000) users      (100)      939 2023-04-10 10:56:55.000000 fenrirWeb-0.4.0/fenrirWeb/views/navbar.tpl
--rw-r--r--   0 hannes    (1000) users      (100)     8286 2023-04-10 10:56:55.000000 fenrirWeb-0.4.0/fenrirWeb/views/settings.tpl
--rw-r--r--   0 hannes    (1000) users      (100)     2501 2023-04-10 10:56:55.000000 fenrirWeb-0.4.0/fenrirWeb/views/vpninput.tpl
-drwxr-xr-x   0 hannes    (1000) users      (100)        0 2023-04-12 19:51:06.137783 fenrirWeb-0.4.0/fenrirWeb.egg-info/
--rw-r--r--   0 hannes    (1000) users      (100)      340 2023-04-12 19:51:06.000000 fenrirWeb-0.4.0/fenrirWeb.egg-info/PKG-INFO
--rw-r--r--   0 hannes    (1000) users      (100)      903 2023-04-12 19:51:06.000000 fenrirWeb-0.4.0/fenrirWeb.egg-info/SOURCES.txt
--rw-r--r--   0 hannes    (1000) users      (100)        1 2023-04-12 19:51:06.000000 fenrirWeb-0.4.0/fenrirWeb.egg-info/dependency_links.txt
--rw-r--r--   0 hannes    (1000) users      (100)       50 2023-04-12 19:51:06.000000 fenrirWeb-0.4.0/fenrirWeb.egg-info/entry_points.txt
--rw-r--r--   0 hannes    (1000) users      (100)        1 2023-04-10 10:16:52.000000 fenrirWeb-0.4.0/fenrirWeb.egg-info/not-zip-safe
--rw-r--r--   0 hannes    (1000) users      (100)       32 2023-04-12 19:51:06.000000 fenrirWeb-0.4.0/fenrirWeb.egg-info/requires.txt
--rw-r--r--   0 hannes    (1000) users      (100)       10 2023-04-12 19:51:06.000000 fenrirWeb-0.4.0/fenrirWeb.egg-info/top_level.txt
--rw-r--r--   0 hannes    (1000) users      (100)       38 2023-04-12 19:51:06.145783 fenrirWeb-0.4.0/setup.cfg
--rw-r--r--   0 hannes    (1000) users      (100)      693 2023-04-10 10:56:55.000000 fenrirWeb-0.4.0/setup.py
+drwxr-xr-x   0 hannes    (1000) users      (100)        0 2023-04-16 18:36:43.928919 fenrirWeb-0.5.0/
+-rw-r--r--   0 hannes    (1000) users      (100)    18092 2023-04-10 10:56:55.000000 fenrirWeb-0.5.0/LICENSE
+-rw-r--r--   0 hannes    (1000) users      (100)       80 2023-04-10 10:56:55.000000 fenrirWeb-0.5.0/MANIFEST.in
+-rw-r--r--   0 hannes    (1000) users      (100)      340 2023-04-16 18:36:43.928919 fenrirWeb-0.5.0/PKG-INFO
+-rw-r--r--   0 hannes    (1000) users      (100)      765 2023-04-10 10:59:05.000000 fenrirWeb-0.5.0/README.md
+drwxr-xr-x   0 hannes    (1000) users      (100)        0 2023-04-16 18:36:43.924919 fenrirWeb-0.5.0/fenrirWeb/
+-rw-r--r--   0 hannes    (1000) users      (100)       22 2023-04-16 18:34:53.000000 fenrirWeb-0.5.0/fenrirWeb/__init__.py
+-rw-r--r--   0 hannes    (1000) users      (100)    16875 2023-04-11 21:45:56.000000 fenrirWeb-0.5.0/fenrirWeb/lib.py
+-rw-r--r--   0 hannes    (1000) users      (100)     1052 2023-04-10 10:56:55.000000 fenrirWeb-0.5.0/fenrirWeb/main.py
+drwxr-xr-x   0 hannes    (1000) users      (100)        0 2023-04-16 18:36:43.928919 fenrirWeb-0.5.0/fenrirWeb/static/
+-rw-r--r--   0 hannes    (1000) users      (100)    80420 2023-04-10 10:56:55.000000 fenrirWeb-0.5.0/fenrirWeb/static/bootstrap.bundle.min.js
+-rw-r--r--   0 hannes    (1000) users      (100)   194901 2023-04-10 10:56:55.000000 fenrirWeb-0.5.0/fenrirWeb/static/bootstrap.min.css
+-rw-r--r--   0 hannes    (1000) users      (100)    60404 2023-04-10 10:56:55.000000 fenrirWeb-0.5.0/fenrirWeb/static/bootstrap.min.js
+-rw-r--r--   0 hannes    (1000) users      (100)     9369 2023-04-10 10:56:55.000000 fenrirWeb-0.5.0/fenrirWeb/static/disabled.png
+-rw-r--r--   0 hannes    (1000) users      (100)    20270 2023-04-10 10:56:55.000000 fenrirWeb-0.5.0/fenrirWeb/static/disabled.svg
+-rw-r--r--   0 hannes    (1000) users      (100)     8004 2023-04-10 10:56:55.000000 fenrirWeb-0.5.0/fenrirWeb/static/enabled.png
+-rw-r--r--   0 hannes    (1000) users      (100)    28344 2023-04-10 10:56:55.000000 fenrirWeb-0.5.0/fenrirWeb/static/enabled.svg
+-rw-r--r--   0 hannes    (1000) users      (100)    93062 2023-04-10 10:56:55.000000 fenrirWeb-0.5.0/fenrirWeb/static/favicon.ico
+-rw-r--r--   0 hannes    (1000) users      (100)    15194 2023-04-16 18:30:17.000000 fenrirWeb-0.5.0/fenrirWeb/static/fenrir.js
+-rw-r--r--   0 hannes    (1000) users      (100)     2104 2023-04-10 10:56:55.000000 fenrirWeb-0.5.0/fenrirWeb/static/settings.png
+-rw-r--r--   0 hannes    (1000) users      (100)     9046 2023-04-10 10:56:55.000000 fenrirWeb-0.5.0/fenrirWeb/view_config.py
+-rw-r--r--   0 hannes    (1000) users      (100)     3152 2023-04-10 10:56:55.000000 fenrirWeb-0.5.0/fenrirWeb/view_main.py
+drwxr-xr-x   0 hannes    (1000) users      (100)        0 2023-04-16 18:36:43.928919 fenrirWeb-0.5.0/fenrirWeb/views/
+-rw-r--r--   0 hannes    (1000) users      (100)     3143 2023-04-16 16:41:07.000000 fenrirWeb-0.5.0/fenrirWeb/views/changepassword.tpl
+-rw-r--r--   0 hannes    (1000) users      (100)     2736 2023-04-16 16:31:13.000000 fenrirWeb-0.5.0/fenrirWeb/views/createpassword.tpl
+-rw-r--r--   0 hannes    (1000) users      (100)     3064 2023-04-10 10:56:55.000000 fenrirWeb-0.5.0/fenrirWeb/views/index.tpl
+-rw-r--r--   0 hannes    (1000) users      (100)     1697 2023-04-10 10:56:55.000000 fenrirWeb-0.5.0/fenrirWeb/views/mappinginput.tpl
+-rw-r--r--   0 hannes    (1000) users      (100)      939 2023-04-10 10:56:55.000000 fenrirWeb-0.5.0/fenrirWeb/views/navbar.tpl
+-rw-r--r--   0 hannes    (1000) users      (100)     8286 2023-04-10 10:56:55.000000 fenrirWeb-0.5.0/fenrirWeb/views/settings.tpl
+-rw-r--r--   0 hannes    (1000) users      (100)     2501 2023-04-10 10:56:55.000000 fenrirWeb-0.5.0/fenrirWeb/views/vpninput.tpl
+drwxr-xr-x   0 hannes    (1000) users      (100)        0 2023-04-16 18:36:43.928919 fenrirWeb-0.5.0/fenrirWeb.egg-info/
+-rw-r--r--   0 hannes    (1000) users      (100)      340 2023-04-16 18:36:43.000000 fenrirWeb-0.5.0/fenrirWeb.egg-info/PKG-INFO
+-rw-r--r--   0 hannes    (1000) users      (100)      903 2023-04-16 18:36:43.000000 fenrirWeb-0.5.0/fenrirWeb.egg-info/SOURCES.txt
+-rw-r--r--   0 hannes    (1000) users      (100)        1 2023-04-16 18:36:43.000000 fenrirWeb-0.5.0/fenrirWeb.egg-info/dependency_links.txt
+-rw-r--r--   0 hannes    (1000) users      (100)       50 2023-04-16 18:36:43.000000 fenrirWeb-0.5.0/fenrirWeb.egg-info/entry_points.txt
+-rw-r--r--   0 hannes    (1000) users      (100)        1 2023-04-10 10:16:52.000000 fenrirWeb-0.5.0/fenrirWeb.egg-info/not-zip-safe
+-rw-r--r--   0 hannes    (1000) users      (100)       32 2023-04-16 18:36:43.000000 fenrirWeb-0.5.0/fenrirWeb.egg-info/requires.txt
+-rw-r--r--   0 hannes    (1000) users      (100)       10 2023-04-16 18:36:43.000000 fenrirWeb-0.5.0/fenrirWeb.egg-info/top_level.txt
+-rw-r--r--   0 hannes    (1000) users      (100)       38 2023-04-16 18:36:43.928919 fenrirWeb-0.5.0/setup.cfg
+-rw-r--r--   0 hannes    (1000) users      (100)      693 2023-04-10 10:56:55.000000 fenrirWeb-0.5.0/setup.py
```

### Comparing `fenrirWeb-0.4.0/LICENSE` & `fenrirWeb-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.4.0/README.md` & `fenrirWeb-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.4.0/fenrirWeb/lib.py` & `fenrirWeb-0.5.0/fenrirWeb/lib.py`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.4.0/fenrirWeb/main.py` & `fenrirWeb-0.5.0/fenrirWeb/main.py`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.4.0/fenrirWeb/static/bootstrap.bundle.min.js` & `fenrirWeb-0.5.0/fenrirWeb/static/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.4.0/fenrirWeb/static/bootstrap.min.css` & `fenrirWeb-0.5.0/fenrirWeb/static/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.4.0/fenrirWeb/static/bootstrap.min.js` & `fenrirWeb-0.5.0/fenrirWeb/static/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.4.0/fenrirWeb/static/disabled.png` & `fenrirWeb-0.5.0/fenrirWeb/static/disabled.png`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.4.0/fenrirWeb/static/disabled.svg` & `fenrirWeb-0.5.0/fenrirWeb/static/disabled.svg`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.4.0/fenrirWeb/static/enabled.png` & `fenrirWeb-0.5.0/fenrirWeb/static/enabled.png`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.4.0/fenrirWeb/static/enabled.svg` & `fenrirWeb-0.5.0/fenrirWeb/static/enabled.svg`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.4.0/fenrirWeb/static/favicon.ico` & `fenrirWeb-0.5.0/fenrirWeb/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.4.0/fenrirWeb/static/fenrir.js` & `fenrirWeb-0.5.0/fenrirWeb/static/fenrir.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -28,26 +28,32 @@
         handleResponseToast('mappingModal', resp);
         refreshMapping();
     })
 
 }
 
 async function handleCreatePasswordSubmit() {
+    document.getElementById('createpasswordsubmit').disabled = true;
+    document.getElementById('createpasswordsubmitspinner').hidden = false;
+
     var data = {
         'password': document.getElementById('vpnpassword').value,
         'passwordrepeat': document.getElementById('repeatvpnpassword').value,
         'passwordusedforencryption': document.getElementById('chisencryptionpassword').checked ? "on" : "off"
     };
 
     getData('/createpassword', data).then(resp => resp.text()).then(resp => {
         handleResponseToast('createpasswordmodal', resp);
     })
 }
 
 async function handleChangePasswordSubmit() {
+    document.getElementById('changepasswordsubmit').disabled = true;
+    document.getElementById('changepasswordsubmitspinner').hidden = false;
+
     var data = {
         'currentpassword': document.getElementById('chcurrentpassword').value,
         'password': document.getElementById('chvpnpassword').value,
         'passwordrepeat': document.getElementById('chrepeatvpnpassword').value,
         'passwordusedforencryption': document.getElementById('chisencryptionpassword').checked ? "on" : "off"
     };
     getData('/changepassword', data).then(resp => resp.text()).then(resp => {
@@ -125,23 +131,21 @@
     })
 }
 
 function sumbitVPNConfig() {
     form = document.getElementById("vpnconfigform")
     if (checkformvalidity(form)) {
         handleVPNConfigSubmit();
-        //form.dispatchEvent(new CustomEvent('submit', {cancelable: true}));
     }
 }
 
 function sumbitMappingConfig() {
     form = document.getElementById("mappingform")
     if (checkformvalidity(form)) {
         handleIPmappingSubmit();
-        //form.dispatchEvent(new CustomEvent('submit', {cancelable: true}));
     }
 }
 
 async function deleteVPNConfigConfirmed() {
     data = {
         profilename: document.getElementById('deletename').innerHTML
     }
@@ -225,14 +229,22 @@
     document.getElementById('vpnconfigsubmitspinner').hidden = true;
     var jsondata = event.relatedTarget.getAttribute('data-id');
     var data = JSON.parse(jsondata);
     var name = data ? data['data'] : null;
     var inputform = document.getElementById('vpnconfigform');
     var defaultisset = profiletablehasdefault(inputform);
     inputform.classList.remove("was-validated");
+
+    document.getElementById('vpnconfigform').addEventListener('keydown', function(event) {
+        if (event.key == "Enter" && event.target.type !== "textarea") {
+            event.preventDefault();
+            sumbitVPNConfig();
+        }
+    });
+
     // adding new configuration
     if (!name) {
         var inputs = inputform.getElementsByTagName('input');
         var textarea = inputform.getElementsByTagName('textarea');
         data = [].concat(Array.from(inputs)).concat(Array.from(textarea));
         for (i = 0; i < data.length; i++) {
             if (data[i].type == 'checkbox') {
@@ -372,25 +384,60 @@
     ipselect.disabled = false
     var jsondata = event.relatedTarget.getAttribute('data-id');
     var data = JSON.parse(jsondata);
     if (data) {
         ipselect.value = data['data']
         nameselect.value = data['profile']
         ipselect.disabled = true
+    } else {
+        var tbody = document.getElementById('vpnsettingstablebody');
+        var rows = tbody.getElementsByTagName('tr');
+        for (var i = nameselect.options.length - 1; i > 0; i--) {
+            nameselect.removeChild(nameselect.options[i]);
+        }
+        for (var i = 0; i < rows.length; i++) {
+            var firstCell = rows[i].querySelector('td:first-child');
+            var value = firstCell.innerText;
+            var option = document.createElement('option');
+            option.value = value;
+            option.text = value;
+            nameselect.appendChild(option);
+        }
     }
 }
 
 function changePasswordModal(event) {
-    document.getElementById('chvpnpasswordform').classList.remove("was-validated")
-    document.getElementById('chcurrentpassword').value = ''
-    document.getElementById('chvpnpassword').value = ''
-    document.getElementById('chrepeatvpnpassword').value = ''
+    document.getElementById('chvpnpasswordform').classList.remove("was-validated");
+    document.getElementById('chvpnpassword').value = '';
+    document.getElementById('chcurrentpassword').value = '';
+    document.getElementById('chrepeatvpnpassword').value = '';
     getData('/ispasswordusedforencryption', {}).then(resp => resp.json()).then(resp => {
         document.getElementById('chisencryptionpassword').checked = resp['checked']
     })
+    document.getElementById('chvpnpasswordform').addEventListener('keydown', function(event) {
+        if (event.key == "Enter") {
+            event.preventDefault();
+            sumbitVPNPassword(true);
+        }
+    });
+}
+
+function createPasswordModal(event) {
+    document.getElementById('vpnpasswordform').addEventListener('keydown', function(event) {
+        if (event.key == "Enter") {
+            event.preventDefault();
+            sumbitVPNPassword(false);
+        }
+    });
+}
+
+function setfocus(focusobject) {
+    focusobject.focus();
+    focusobject.select();
+
 }
 
 function modalData() {
     var configurationDataModal = document.getElementById('configurationDataModal')
     configurationDataModal.addEventListener('show.bs.modal', function(event) {
         configModal(event);
     })
@@ -406,14 +453,28 @@
     })
 
     var changePasswordModalobj = document.getElementById('changepasswordmodal')
     changePasswordModalobj.addEventListener('show.bs.modal', function(event) {
         changePasswordModal(event);
     })
 
+    var createPasswordModalobj = document.getElementById('createpasswordmodal')
+    createPasswordModalobj.addEventListener('show.bs.modal', function(event) {
+        createPasswordModal(event);
+    })
+
+    createPasswordModalobj.addEventListener('shown.bs.modal', function(event) {
+        setfocus(document.getElementById('vpnpassword'));
+    })
+    changePasswordModalobj.addEventListener('shown.bs.modal', function(event) {
+        setfocus(document.getElementById('chcurrentpassword'));
+    })
+    configurationDataModal.addEventListener('shown.bs.modal', function(event) {
+        setfocus(document.getElementById('profilename'));
+    })
 }
 
 function checkformvalidity(from) {
     result = form.checkValidity()
     form.classList.add('was-validated')
     return result
 }
```

### Comparing `fenrirWeb-0.4.0/fenrirWeb/static/settings.png` & `fenrirWeb-0.5.0/fenrirWeb/static/settings.png`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.4.0/fenrirWeb/view_config.py` & `fenrirWeb-0.5.0/fenrirWeb/view_config.py`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.4.0/fenrirWeb/view_main.py` & `fenrirWeb-0.5.0/fenrirWeb/view_main.py`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.4.0/fenrirWeb/views/changepassword.tpl` & `fenrirWeb-0.5.0/fenrirWeb/views/changepassword.tpl`

 * *Files 3% similar despite different names*

```diff
@@ -1,48 +1,51 @@
 <div class="modal fade" id="changepasswordmodal" tabindex="-1" aria-labelledby="changepasswordmodalLabel" aria-hidden="true">
-    <div class="modal-dialog modal-md">
-      <div class="modal-content">
-        <div class="modal-header">
-          <h5 class="modal-title" >Change Password for VPN Profiles</h5>
-          <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
-        </div>
-        <div class="modal-body">
-          <div class="container">
-            <form class="needs-validation" id="chvpnpasswordform" onsubmit="handleChangePasswordSubmit();" novalidate>
-              <div class="col-12 mb-3 form-floating has-validation">
-                <input type="password" class="form-control" id="chcurrentpassword" placeholder="current Password">
-                <label for="currentpassword" class="form-label mx-2">Enter current VPNProfiles password</label>
-                <div class="invalid-feedback">Passwords do not match</div>
-              </div>
+  <div class="modal-dialog modal-md">
+    <div class="modal-content">
+      <div class="modal-header">
+        <h5 class="modal-title" >Change Password for VPN Profiles</h5>
+        <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
+      </div>
+      <div class="modal-body">
+        <div class="container">
+          <form class="needs-validation" id="chvpnpasswordform" onsubmit="handleChangePasswordSubmit();" novalidate>
+            <div class="col-12 mb-3 form-floating has-validation">
+              <input type="password" class="form-control" id="chcurrentpassword" placeholder="current Password">
+              <label for="currentpassword" class="form-label mx-2">Enter current VPNProfiles password</label>
+              <div class="invalid-feedback">Passwords do not match</div>
+            </div>
 
-              <div class="col-12 mb-3 form-floating has-validation">
-                <input type="password" class="form-control" id="chvpnpassword" placeholder="new Password" onkeyup="validatepassword();">
-                <label for="vpnpassword" class="form-label mx-2">Enter new VPNProfiles password</label>
-                <div class="invalid-feedback">Passwords do not match</div>
-              </div>
-              <div class="col-12 mb-3 form-floating has-validation">
-                <input type="password" class="form-control" id="chrepeatvpnpassword" placeholder="new Password" onkeyup="validatepassword();">
-                <label for="repeatvpnpassword" class="form-label mx-2">Repeat new VPNProfiles password</label>
-                <div class="invalid-feedback">Passwords do not match</div>
-              </div>
-              <div class="col-12 mt-3 form-floating">
-                <div class="form-check col-12 m-2 form-switch">
-                    <input class="form-check-input" style="transform: scale(1.3);" type="checkbox" role="switch" id="chisencryptionpassword">
-                    <label class="form-check-label" for="isencryptionpassword">Use password for VPNProfile encryption</label>
-                </div>
+            <div class="col-12 mb-3 form-floating has-validation">
+              <input type="password" class="form-control" id="chvpnpassword" placeholder="new Password" onkeyup="validatepassword();">
+              <label for="vpnpassword" class="form-label mx-2">Enter new VPNProfiles password</label>
+              <div class="invalid-feedback">Passwords do not match</div>
+            </div>
+            <div class="col-12 mb-3 form-floating has-validation">
+              <input type="password" class="form-control" id="chrepeatvpnpassword" placeholder="new Password" onkeyup="validatepassword();">
+              <label for="repeatvpnpassword" class="form-label mx-2">Repeat new VPNProfiles password</label>
+              <div class="invalid-feedback">Passwords do not match</div>
+            </div>
+            <div class="col-12 mt-3 form-floating">
+              <div class="form-check col-12 m-2 form-switch">
+                  <input class="form-check-input" style="transform: scale(1.3);" type="checkbox" role="switch" id="chisencryptionpassword">
+                  <label class="form-check-label" for="isencryptionpassword">Use password for VPNProfile encryption</label>
               </div>
-            </form>
-            <div class="mt-5 mx-2 col-12 fs-6">
-              <p class="fw-bolder ">Note:</p>
-              <p>Password must be enterd in order to modify, delete and add VPNConfigurations.
-                  This is done to ensure that sensitive data is not shown without authentication.<br><br>
-                  When password is used for VPNProfile encryption password must be enterd in order for VPNConnection(s) to work.</p>
             </div>
+          </form>
+          <div class="mt-5 mx-2 col-12 fs-6">
+            <p class="fw-bolder ">Note:</p>
+            <p>Password must be enterd in order to modify, delete and add VPNConfigurations.
+                This is done to ensure that sensitive data is not shown without authentication.<br><br>
+                When password is used for VPNProfile encryption password must be enterd in order for VPNConnection(s) to work.</p>
           </div>
         </div>
-        <div class="modal-footer">
-          <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Cancel</button>
-          <button type="button" class="btn btn-success" onclick="sumbitVPNPassword(true);">Sumbit</button>
-        </div>
+      </div>
+      <div class="modal-footer">
+        <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Cancel</button>
+        <button type="button" class="btn btn-success" id="changepasswordsubmit" onclick="sumbitVPNPassword(true);">
+          <span class="spinner-border spinner-border-sm mr-2" id="changepasswordsubmitspinner" hidden role="status" aria-hidden="true"></span>
+          Sumbit
+        </button>
       </div>
     </div>
-  </div>
+  </div>
+</div>
```

### Comparing `fenrirWeb-0.4.0/fenrirWeb/views/createpassword.tpl` & `fenrirWeb-0.5.0/fenrirWeb/views/createpassword.tpl`

 * *Files 9% similar despite different names*

```diff
@@ -31,12 +31,15 @@
                 This is done to ensure that sensitive data is not shown without authentication.<br><br>
                 When password is used for VPNProfile encryption password must be enterd in order for VPNConnection(s) to work.</p>
           </div>
         </div>
       </div>
       <div class="modal-footer">
         <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Cancel</button>
-        <button type="button" class="btn btn-success" onclick="sumbitVPNPassword();">Sumbit</button>
+        <button type="button" class="btn btn-success" id="createpasswordsubmit" onclick="sumbitVPNPassword();">
+          <span class="spinner-border spinner-border-sm mr-2" id="createpasswordsubmitspinner" hidden role="status" aria-hidden="true"></span>
+          Sumbit
+        </button>
       </div>
     </div>
   </div>
 </div>
```

### Comparing `fenrirWeb-0.4.0/fenrirWeb/views/index.tpl` & `fenrirWeb-0.5.0/fenrirWeb/views/index.tpl`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.4.0/fenrirWeb/views/mappinginput.tpl` & `fenrirWeb-0.5.0/fenrirWeb/views/mappinginput.tpl`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.4.0/fenrirWeb/views/navbar.tpl` & `fenrirWeb-0.5.0/fenrirWeb/views/navbar.tpl`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.4.0/fenrirWeb/views/settings.tpl` & `fenrirWeb-0.5.0/fenrirWeb/views/settings.tpl`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.4.0/fenrirWeb/views/vpninput.tpl` & `fenrirWeb-0.5.0/fenrirWeb/views/vpninput.tpl`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.4.0/fenrirWeb.egg-info/SOURCES.txt` & `fenrirWeb-0.5.0/fenrirWeb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fenrirWeb-0.4.0/setup.py` & `fenrirWeb-0.5.0/setup.py`

 * *Files identical despite different names*

