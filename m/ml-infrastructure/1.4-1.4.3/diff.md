# Comparing `tmp/ml_infrastructure-1.4.tar.gz` & `tmp/ml_infrastructure-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml_infrastructure-1.4.tar", last modified: Sat Feb 25 18:16:26 2023, max compression
+gzip compressed data, was "ml_infrastructure-1.4.3.tar", last modified: Sun Apr 16 14:43:18 2023, max compression
```

## Comparing `ml_infrastructure-1.4.tar` & `ml_infrastructure-1.4.3.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxrwxr-x   0 maple     (1000) maple     (1000)        0 2023-02-25 18:16:26.205523 ml_infrastructure-1.4/
--rw-rw-r--   0 maple     (1000) maple     (1000)     1069 2023-02-25 18:08:38.000000 ml_infrastructure-1.4/LICENSE.rst
--rw-rw-r--   0 maple     (1000) maple     (1000)      579 2023-02-25 18:16:26.205523 ml_infrastructure-1.4/PKG-INFO
--rw-rw-r--   0 maple     (1000) maple     (1000)        0 2023-02-25 18:05:38.000000 ml_infrastructure-1.4/README.rst
-drwxrwxr-x   0 maple     (1000) maple     (1000)        0 2023-02-25 18:16:26.205523 ml_infrastructure-1.4/ml_infrastructure/
--rw-rw-r--   0 maple     (1000) maple     (1000)      168 2023-02-25 17:41:53.000000 ml_infrastructure-1.4/ml_infrastructure/__init__.py
--rw-rw-r--   0 maple     (1000) maple     (1000)     8150 2023-02-25 16:28:06.000000 ml_infrastructure-1.4/ml_infrastructure/app.py
--rw-rw-r--   0 maple     (1000) maple     (1000)      180 2022-11-28 03:17:28.000000 ml_infrastructure-1.4/ml_infrastructure/data_manager.py
--rw-rw-r--   0 maple     (1000) maple     (1000)     4162 2022-12-13 03:39:09.000000 ml_infrastructure-1.4/ml_infrastructure/evaluator.py
--rw-rw-r--   0 maple     (1000) maple     (1000)     3532 2022-11-28 03:17:28.000000 ml_infrastructure-1.4/ml_infrastructure/example.py
--rw-rw-r--   0 maple     (1000) maple     (1000)     2554 2023-01-03 08:24:04.000000 ml_infrastructure-1.4/ml_infrastructure/manager.py
--rw-rw-r--   0 maple     (1000) maple     (1000)     2831 2022-12-13 05:07:39.000000 ml_infrastructure-1.4/ml_infrastructure/model.py
-drwxrwxr-x   0 maple     (1000) maple     (1000)        0 2023-02-25 18:16:26.205523 ml_infrastructure-1.4/ml_infrastructure/templates/
--rw-rw-r--   0 maple     (1000) maple     (1000)      508 2022-11-28 03:17:28.000000 ml_infrastructure-1.4/ml_infrastructure/templates/control.html
--rw-rw-r--   0 maple     (1000) maple     (1000)      316 2022-11-28 03:17:28.000000 ml_infrastructure-1.4/ml_infrastructure/templates/eval.html
--rw-rw-r--   0 maple     (1000) maple     (1000)     1456 2023-02-25 17:49:40.000000 ml_infrastructure-1.4/ml_infrastructure/templates/header.html
--rw-rw-r--   0 maple     (1000) maple     (1000)      850 2022-11-28 03:17:28.000000 ml_infrastructure-1.4/ml_infrastructure/templates/index.html
--rw-rw-r--   0 maple     (1000) maple     (1000)      309 2023-02-25 16:35:50.000000 ml_infrastructure-1.4/ml_infrastructure/templates/loss.html
--rw-rw-r--   0 maple     (1000) maple     (1000)      181 2022-11-28 03:17:28.000000 ml_infrastructure-1.4/ml_infrastructure/templates/trainingEval.html
--rw-rw-r--   0 maple     (1000) maple     (1000)      452 2023-02-25 17:15:04.000000 ml_infrastructure-1.4/ml_infrastructure/templates/trainingLoss.html
--rw-rw-r--   0 maple     (1000) maple     (1000)      189 2022-11-28 03:17:28.000000 ml_infrastructure-1.4/ml_infrastructure/templates/validationEval.html
--rw-rw-r--   0 maple     (1000) maple     (1000)      446 2023-02-25 16:35:50.000000 ml_infrastructure-1.4/ml_infrastructure/templates/validationLoss.html
--rw-rw-r--   0 maple     (1000) maple     (1000)     1899 2022-12-13 04:56:19.000000 ml_infrastructure-1.4/ml_infrastructure/trainer.py
-drwxrwxr-x   0 maple     (1000) maple     (1000)        0 2023-02-25 18:16:26.205523 ml_infrastructure-1.4/ml_infrastructure.egg-info/
--rw-rw-r--   0 maple     (1000) maple     (1000)      579 2023-02-25 18:16:26.000000 ml_infrastructure-1.4/ml_infrastructure.egg-info/PKG-INFO
--rw-rw-r--   0 maple     (1000) maple     (1000)      863 2023-02-25 18:16:26.000000 ml_infrastructure-1.4/ml_infrastructure.egg-info/SOURCES.txt
--rw-rw-r--   0 maple     (1000) maple     (1000)        1 2023-02-25 18:16:26.000000 ml_infrastructure-1.4/ml_infrastructure.egg-info/dependency_links.txt
--rw-rw-r--   0 maple     (1000) maple     (1000)       46 2023-02-25 18:16:26.000000 ml_infrastructure-1.4/ml_infrastructure.egg-info/requires.txt
--rw-rw-r--   0 maple     (1000) maple     (1000)       18 2023-02-25 18:16:26.000000 ml_infrastructure-1.4/ml_infrastructure.egg-info/top_level.txt
--rw-rw-r--   0 maple     (1000) maple     (1000)      107 2023-02-25 18:16:26.205523 ml_infrastructure-1.4/setup.cfg
--rw-rw-r--   0 maple     (1000) maple     (1000)      985 2023-02-25 15:41:58.000000 ml_infrastructure-1.4/setup.py
+drwxrwxr-x   0 maple     (1000) maple     (1000)        0 2023-04-16 14:43:18.622128 ml_infrastructure-1.4.3/
+-rw-rw-r--   0 maple     (1000) maple     (1000)     1067 2023-04-16 13:21:50.000000 ml_infrastructure-1.4.3/LICENSE.rst
+-rw-rw-r--   0 maple     (1000) maple     (1000)      581 2023-04-16 14:43:18.622128 ml_infrastructure-1.4.3/PKG-INFO
+-rw-rw-r--   0 maple     (1000) maple     (1000)        0 2023-02-25 18:05:38.000000 ml_infrastructure-1.4.3/README.rst
+drwxrwxr-x   0 maple     (1000) maple     (1000)        0 2023-04-16 14:43:18.622128 ml_infrastructure-1.4.3/ml_infrastructure/
+-rw-rw-r--   0 maple     (1000) maple     (1000)      168 2023-02-25 17:41:53.000000 ml_infrastructure-1.4.3/ml_infrastructure/__init__.py
+-rw-rw-r--   0 maple     (1000) maple     (1000)     9224 2023-04-15 23:10:23.000000 ml_infrastructure-1.4.3/ml_infrastructure/app.py
+-rw-rw-r--   0 maple     (1000) maple     (1000)      180 2022-11-28 03:17:28.000000 ml_infrastructure-1.4.3/ml_infrastructure/data_manager.py
+-rw-rw-r--   0 maple     (1000) maple     (1000)     4402 2023-04-16 13:23:13.000000 ml_infrastructure-1.4.3/ml_infrastructure/evaluator.py
+-rw-rw-r--   0 maple     (1000) maple     (1000)     3532 2022-11-28 03:17:28.000000 ml_infrastructure-1.4.3/ml_infrastructure/example.py
+-rw-rw-r--   0 maple     (1000) maple     (1000)     3924 2023-04-16 14:21:11.000000 ml_infrastructure-1.4.3/ml_infrastructure/manager.py
+-rw-rw-r--   0 maple     (1000) maple     (1000)     3300 2023-04-16 13:27:14.000000 ml_infrastructure-1.4.3/ml_infrastructure/model.py
+drwxrwxr-x   0 maple     (1000) maple     (1000)        0 2023-04-16 14:43:18.622128 ml_infrastructure-1.4.3/ml_infrastructure/templates/
+-rw-rw-r--   0 maple     (1000) maple     (1000)      508 2022-11-28 03:17:28.000000 ml_infrastructure-1.4.3/ml_infrastructure/templates/control.html
+-rw-rw-r--   0 maple     (1000) maple     (1000)      316 2023-04-15 15:08:42.000000 ml_infrastructure-1.4.3/ml_infrastructure/templates/eval.html
+-rw-rw-r--   0 maple     (1000) maple     (1000)     1530 2023-04-16 14:31:42.000000 ml_infrastructure-1.4.3/ml_infrastructure/templates/header.html
+-rw-rw-r--   0 maple     (1000) maple     (1000)      138 2023-04-15 15:08:42.000000 ml_infrastructure-1.4.3/ml_infrastructure/templates/index.html
+-rw-rw-r--   0 maple     (1000) maple     (1000)      309 2023-04-15 15:08:42.000000 ml_infrastructure-1.4.3/ml_infrastructure/templates/loss.html
+-rw-rw-r--   0 maple     (1000) maple     (1000)     1706 2023-04-16 14:31:42.000000 ml_infrastructure-1.4.3/ml_infrastructure/templates/stopForm.html
+-rw-rw-r--   0 maple     (1000) maple     (1000)      181 2022-11-28 03:17:28.000000 ml_infrastructure-1.4.3/ml_infrastructure/templates/trainingEval.html
+-rw-rw-r--   0 maple     (1000) maple     (1000)      452 2023-02-25 17:15:04.000000 ml_infrastructure-1.4.3/ml_infrastructure/templates/trainingLoss.html
+-rw-rw-r--   0 maple     (1000) maple     (1000)      189 2022-11-28 03:17:28.000000 ml_infrastructure-1.4.3/ml_infrastructure/templates/validationEval.html
+-rw-rw-r--   0 maple     (1000) maple     (1000)      446 2023-02-25 16:35:50.000000 ml_infrastructure-1.4.3/ml_infrastructure/templates/validationLoss.html
+-rw-rw-r--   0 maple     (1000) maple     (1000)     1899 2022-12-13 04:56:19.000000 ml_infrastructure-1.4.3/ml_infrastructure/trainer.py
+drwxrwxr-x   0 maple     (1000) maple     (1000)        0 2023-04-16 14:43:18.622128 ml_infrastructure-1.4.3/ml_infrastructure.egg-info/
+-rw-rw-r--   0 maple     (1000) maple     (1000)      581 2023-04-16 14:43:18.000000 ml_infrastructure-1.4.3/ml_infrastructure.egg-info/PKG-INFO
+-rw-rw-r--   0 maple     (1000) maple     (1000)      905 2023-04-16 14:43:18.000000 ml_infrastructure-1.4.3/ml_infrastructure.egg-info/SOURCES.txt
+-rw-rw-r--   0 maple     (1000) maple     (1000)        1 2023-04-16 14:43:18.000000 ml_infrastructure-1.4.3/ml_infrastructure.egg-info/dependency_links.txt
+-rw-rw-r--   0 maple     (1000) maple     (1000)       46 2023-04-16 14:43:18.000000 ml_infrastructure-1.4.3/ml_infrastructure.egg-info/requires.txt
+-rw-rw-r--   0 maple     (1000) maple     (1000)       18 2023-04-16 14:43:18.000000 ml_infrastructure-1.4.3/ml_infrastructure.egg-info/top_level.txt
+-rw-rw-r--   0 maple     (1000) maple     (1000)      107 2023-04-16 14:43:18.626129 ml_infrastructure-1.4.3/setup.cfg
+-rw-rw-r--   0 maple     (1000) maple     (1000)      987 2023-04-15 23:10:44.000000 ml_infrastructure-1.4.3/setup.py
```

### Comparing `ml_infrastructure-1.4/LICENSE.rst` & `ml_infrastructure-1.4.3/LICENSE.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) [year] [fullname]
+Copyright (c) 2022 Ada Lazuli
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `ml_infrastructure-1.4/PKG-INFO` & `ml_infrastructure-1.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml_infrastructure
-Version: 1.4
+Version: 1.4.3
 Summary: Software infrastructure to for machine learning
 Author: Ada L
 Author-email: the.nostra.tymus@gmail.com
 License: MIT
 Keywords: machine learning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `ml_infrastructure-1.4/ml_infrastructure/app.py` & `ml_infrastructure-1.4.3/ml_infrastructure/app.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,37 +8,86 @@
 import numpy as np
 import os
 
 app = Flask(__name__)
 turbo = Turbo(app)
 
 performance = dict()
+idx = 0
+stop_criteria = {
+    "threshold": -1,
+    "epoch": -1
+}
 
 
 @app.route('/')
 @app.route('/loss')
 def loss():
     return render_template('loss.html')
 
 
 @app.route('/evaluation')
 def evaluation():
+    global idx
+    idx = int(request.args['index'])
+    print(idx)
     return render_template('eval.html')
 
 
 @app.route('/controller')
 def control():
     return render_template('control.html')
 
 
 @app.route('/console')
 def console():
     return render_template('console.html')
 
 
+@app.route('/stop')
+def stopForm():
+    return render_template('stopForm.html')
+
+
+@app.route('/stopCriteria')
+def getStopCriteria():
+    global stop_criteria
+
+    return Response(json.dumps(stop_criteria), status=200, mimetype='application/json')
+
+
+@app.route('/updateCriteria')
+def updateCriteria():
+    global stop_criteria
+
+    if request.args['index'] == "":
+        index = 0
+    else:
+        index = request.args['index']
+
+    if request.args['threshold'] == "":
+        threshold = -1
+    else:
+        threshold = request.args['threshold']
+
+    if request.args['epoch'] == "":
+        epoch = -1
+    else:
+        epoch = request.args['epoch']
+
+    stop_criteria = {
+        'metric': request.args['metric'],
+        'threshold': threshold,
+        'index': index,
+        'epoch': epoch
+    }
+
+    return Response("Okay", status=200, mimetype='application/json')
+
+
 @app.route('/updateLoss', methods=["POST"])
 def updateLoss():
     global performance
     name = request.json['data']['name']
     mode = request.json['data']['mode']
     if name not in performance.keys():
         performance = add_model(performance, name)
@@ -56,18 +105,19 @@
 
 @app.route('/evalUpdate', methods=["POST"])
 def evalUpdate():
     global performance
     evaluation_results = request.json['data']
     name = evaluation_results['name']
     mode = evaluation_results['mode']
+
     if name not in performance.keys():
         performance = add_model(performance, name)
-
     performance[name]['evaluation'][mode] = evaluation_results
+
     if mode == 'training':
         turbo.push(turbo.replace(render_template('trainingEval.html'), 'trainingEval'))
     else:
         turbo.push(turbo.replace(render_template('validationEval.html'), 'validationEval'))
 
     return Response("Okay", status=200, mimetype='application/json')
 
@@ -116,15 +166,15 @@
 
 @app.route('/download', methods=['GET'])
 def download():
     global performance
     temp = tempfile.NamedTemporaryFile()
     with open(temp.name, 'w') as file_out:
         json.dump(performance, file_out)
-    return send_file(temp.name)
+    return send_file(temp.name, download_name="Evaluation_Metrics.json")
 
 
 @app.route('/shutdown', methods=['GET'])
 def shutdown():
     os._exit(0)
 
 
@@ -172,64 +222,66 @@
         }
     }
     return json.dumps(loss_graph, cls=plotly.utils.PlotlyJSONEncoder)
 
 
 def get_eval_table(mode):
     global performance
+    global idx
     keys = ['Name', 'Accuracy', 'Classification Error', 'Precision', 'Recall', 'Specificity', 'F1-Score', 'TP', 'FP',
             'TN', 'FN']
     table = Figure([Table(
         header=dict(
             values=keys,
             font=dict(size=12),
             align="left"
         ),
         cells=dict(
-            values=get_evaluation_metrics(performance, mode),
+            values=get_evaluation_metrics(performance, mode, idx),
             align="left")
     )
     ])
     return json.dumps(table, cls=plotly.utils.PlotlyJSONEncoder)
 
 
-def get_evaluation_metrics(performance, mode):
+# TODO Verify this function works
+def get_evaluation_metrics(performance, mode, idx=0):
     return [
 
         [key for key in performance.keys() if
          len(performance[key]['evaluation'][mode].keys()) > 0],
 
-        [np.mean(performance[key]['evaluation'][mode]['Accuracy']) for key in performance.keys() if
+        [performance[key]['evaluation'][mode]['Accuracy'][idx] for key in performance.keys() if
          len(performance[key]['evaluation'][mode].keys()) > 0],
 
-        [np.mean(performance[key]['evaluation'][mode]['Classification Error']) for key in performance.keys() if
+        [performance[key]['evaluation'][mode]['Classification Error'][idx] for key in performance.keys() if
          len(performance[key]['evaluation'][mode].keys()) > 0],
 
-        [np.mean(performance[key]['evaluation'][mode]['Precision']) for key in performance.keys() if
+        [performance[key]['evaluation'][mode]['Precision'][idx] for key in performance.keys() if
          len(performance[key]['evaluation'][mode].keys()) > 0],
 
-        [np.mean(performance[key]['evaluation'][mode]['Recall']) for key in performance.keys() if
+        [performance[key]['evaluation'][mode]['Recall'][idx] for key in performance.keys() if
          len(performance[key]['evaluation'][mode].keys()) > 0],
 
-        [np.mean(performance[key]['evaluation'][mode]['Specificity']) for key in performance.keys() if
+        [performance[key]['evaluation'][mode]['Specificity'][idx] for key in performance.keys() if
          len(performance[key]['evaluation'][mode].keys()) > 0],
 
-        [np.mean(performance[key]['evaluation'][mode]['F1-Score']) for key in performance.keys() if
+        [performance[key]['evaluation'][mode]['F1-Score'][idx] for key in performance.keys() if
          len(performance[key]['evaluation'][mode].keys()) > 0],
 
-        [np.sum(performance[key]['evaluation'][mode]['TP']) for key in performance.keys() if
+        [performance[key]['evaluation'][mode]['TP'][idx] for key in performance.keys() if
          len(performance[key]['evaluation'][mode].keys()) > 0],
 
-        [np.sum(performance[key]['evaluation'][mode]['FP']) for key in performance.keys() if
+        [performance[key]['evaluation'][mode]['FP'][idx] for key in performance.keys() if
          len(performance[key]['evaluation'][mode].keys()) > 0],
 
-        [np.sum(performance[key]['evaluation'][mode]['TN']) for key in performance.keys() if
+        [performance[key]['evaluation'][mode]['TN'][idx] for key in performance.keys() if
          len(performance[key]['evaluation'][mode].keys()) > 0],
 
-        [np.sum(performance[key]['evaluation'][mode]['FN']) for key in performance.keys() if
+        [performance[key]['evaluation'][mode]['FN'][idx] for key in performance.keys() if
          len(performance[key]['evaluation'][mode].keys()) > 0],
     ]
 
 
 def add_model(performance_dict, name):
     performance_dict[name] = {'training': {'values': [], 'index': []},
                               'validation': {'values': [], 'index': []},
```

### Comparing `ml_infrastructure-1.4/ml_infrastructure/evaluator.py` & `ml_infrastructure-1.4.3/ml_infrastructure/evaluator.py`

 * *Files 7% similar despite different names*

```diff
@@ -88,44 +88,47 @@
     if mode == 'training':
         loader = data_manager.train_loader
     else:
         loader = data_manager.validation_loader
 
     confusion_matrix = np.zeros((len(classes), len(classes)), dtype=int)
 
-    with torch.no_grad():
-        for data in loader:
-            inputs, targets = data[0], data[1]
-
-            outputs = model.classify(inputs)
-
-            _, predicted = torch.max(outputs, 1)
-            predicted = predicted.to("cpu")
-
-            for pred, true in zip(predicted, targets):
-                confusion_matrix[int(pred), int(true)] += 1
+    if len(data_manager.classes) == 2:
+        with torch.no_grad():
+            for data in loader:
+                inputs, targets = data[0], data[1]
+
+                outputs = model.classify(inputs)
+                predicted = torch.sigmoid(outputs)
+                predicted = predicted.to("cpu")
+                predicted = [1 if x >= .5 else 0 for x in predicted]
+                for pred, true in zip(predicted, targets):
+                    confusion_matrix[int(pred), int(true)] += 1
 
     return confusion_matrix
 
 
 @dataclass
 class Evaluator:
     model: any = None
     data_manager: any = None
     ip: str = "0.0.0.0"
     port: int = 5000
     best_f1: int = 0
+    save_dir: str = "./results/"
 
     def evaluate(self):
         total_performance = {'training': None, 'validation': None}
         for mode in ['training', 'validation']:
             matrix = evaluate_model(self.model, self.data_manager, mode)
             performance = calc_performance(matrix, self.model, self.data_manager.classes, mode)
             send_performance(performance, self.ip, self.port)
 
             total_performance[mode] = performance
 
         self.model.save(mode="current")
 
         if np.mean(total_performance['validation']['F1-Score']) > self.best_f1:
-            self.model.save(mode='best')
+            self.model.save(mode='best-f1-score', ip=self.ip, port=self.port)
             self.best_f1 = np.mean(total_performance['validation']['F1-Score'])
+
+        return total_performance
```

### Comparing `ml_infrastructure-1.4/ml_infrastructure/example.py` & `ml_infrastructure-1.4.3/ml_infrastructure/example.py`

 * *Files identical despite different names*

### Comparing `ml_infrastructure-1.4/ml_infrastructure/model.py` & `ml_infrastructure-1.4.3/ml_infrastructure/model.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+import json
 import os
 import socket
 from datetime import datetime
 
+import requests
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 import torch.optim as optim
 
 
 class Net(nn.Module):
@@ -61,21 +63,29 @@
         outputs = self.net(inputs)
         loss = self.criterion(outputs, labels)
         return loss.item()
 
     def classify(self, inputs):
         return self.net(inputs.to(self.device))
 
-    def save(self, mode=None):
+    def save(self, mode=None, ip=None, port=None):
         if mode is not None:
             save_name = os.path.join(self.save_dir, f"{self.name}-{mode}.pth")
             torch.save(self.net.state_dict(), save_name)
         else:
             torch.save(self.net.state_dict(), self.save_name)
 
+        if ip is not None and port is not None:
+            res = requests.get(f'http://{ip}:{port}/download')
+            json_dict = json.loads(res.text)
+            if not os.path.isdir(self.save_dir):
+                os.mkdir(self.save_dir)
+            with open(os.path.join(self.save_dir, f"{self.name}-{mode}-performance-metrics.json"), 'w') as file_out:
+                json.dump(json_dict[self.name], file_out)
+
     def load(self):
         self.net.load_state_dict(torch.load(self.save_name))
 
     def verify_save_dir(self, directory):
         if not os.path.exists(directory):
             os.makedirs(directory)
```

### Comparing `ml_infrastructure-1.4/ml_infrastructure/templates/header.html` & `ml_infrastructure-1.4.3/ml_infrastructure/templates/header.html`

 * *Files 14% similar despite different names*

```diff
@@ -20,16 +20,17 @@
     <div class="container">
         <div class="navbar-header">
             <a class="navbar-brand" href="/">M.L.I.</a> |
         </div>
         <div id="navbar" class="collapse navbar-collapse">
             <ul class="nav navbar-nav">
                 <li><a href="/loss">Loss</a></li>
-                <li><a href="/evaluation">Evaluation</a></li>
+                <li><a href="/evaluation?index=0">Evaluation</a></li>
                 <li><a href="/controller">Controller</a></li>
+                <li><a href="/stop">Termination Criteria</a></li>
             </ul>
         </div>
     </div>
 </nav>
 <br />
        {% block content_root %}
        {% endblock %}
```

#### html2text {}

```diff
@@ -2,9 +2,10 @@
 
 
  {{ turbo() }}
 M.L.I. |
     * Loss
     * Evaluation
     * Controller
+    * Termination_Criteria
 
 {% block content_root %} {% endblock %}
```

### Comparing `ml_infrastructure-1.4/ml_infrastructure/trainer.py` & `ml_infrastructure-1.4.3/ml_infrastructure/trainer.py`

 * *Files identical despite different names*

### Comparing `ml_infrastructure-1.4/ml_infrastructure.egg-info/PKG-INFO` & `ml_infrastructure-1.4.3/ml_infrastructure.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-infrastructure
-Version: 1.4
+Version: 1.4.3
 Summary: Software infrastructure to for machine learning
 Author: Ada L
 Author-email: the.nostra.tymus@gmail.com
 License: MIT
 Keywords: machine learning
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `ml_infrastructure-1.4/ml_infrastructure.egg-info/SOURCES.txt` & `ml_infrastructure-1.4.3/ml_infrastructure.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -16,11 +16,12 @@
 ml_infrastructure.egg-info/requires.txt
 ml_infrastructure.egg-info/top_level.txt
 ml_infrastructure/templates/control.html
 ml_infrastructure/templates/eval.html
 ml_infrastructure/templates/header.html
 ml_infrastructure/templates/index.html
 ml_infrastructure/templates/loss.html
+ml_infrastructure/templates/stopForm.html
 ml_infrastructure/templates/trainingEval.html
 ml_infrastructure/templates/trainingLoss.html
 ml_infrastructure/templates/validationEval.html
 ml_infrastructure/templates/validationLoss.html
```

### Comparing `ml_infrastructure-1.4/setup.py` & `ml_infrastructure-1.4.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-VERSION = '1.4'
+VERSION = '1.4.3'
 DESCRIPTION = 'Software infrastructure to for machine learning'
 LONG_DESCRIPTION = 'Software infrastructure for machine learning projects that makes it easier to manage experiments and log progress'
 
 setup(
     name="ml_infrastructure",
     version=VERSION,
     description=DESCRIPTION,
```

