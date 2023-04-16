# Comparing `tmp/edamame-0.47.tar.gz` & `tmp/edamame-0.48.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edamame-0.47.tar", last modified: Sat Apr 15 12:36:12 2023, max compression
+gzip compressed data, was "edamame-0.48.tar", last modified: Sun Apr 16 11:18:01 2023, max compression
```

## Comparing `edamame-0.47.tar` & `edamame-0.48.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-15 12:36:12.813456 edamame-0.47/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1073 2022-11-30 14:22:32.000000 edamame-0.47/LICENSE
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     9635 2023-04-15 12:36:12.813107 edamame-0.47/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     7881 2023-04-15 12:20:06.000000 edamame-0.47/README.md
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-15 12:36:12.806535 edamame-0.47/edamame/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       21 2023-04-15 12:30:37.000000 edamame-0.47/edamame/__init__.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-15 12:36:12.809297 edamame-0.47/edamame/classifier/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       81 2023-04-06 20:59:47.000000 edamame-0.47/edamame/classifier/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    20589 2023-04-15 12:18:35.000000 edamame-0.47/edamame/classifier/classification.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-15 12:36:12.811287 edamame-0.47/edamame/eda/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      860 2023-04-06 20:58:22.000000 edamame-0.47/edamame/eda/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    32458 2023-03-25 15:28:28.000000 edamame-0.47/edamame/eda/eda.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     3814 2023-03-25 15:57:39.000000 edamame-0.47/edamame/eda/tools.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-15 12:36:12.812599 edamame-0.47/edamame/regressor/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      189 2023-04-06 20:53:01.000000 edamame-0.47/edamame/regressor/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     8324 2023-04-02 09:56:35.000000 edamame-0.47/edamame/regressor/diagnose.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    21388 2023-04-04 20:19:13.000000 edamame-0.47/edamame/regressor/regression.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-15 12:36:12.808361 edamame-0.47/edamame.egg-info/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     9635 2023-04-15 12:36:12.000000 edamame-0.47/edamame.egg-info/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      430 2023-04-15 12:36:12.000000 edamame-0.47/edamame.egg-info/SOURCES.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-04-15 12:36:12.000000 edamame-0.47/edamame.egg-info/dependency_links.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       83 2023-04-15 12:36:12.000000 edamame-0.47/edamame.egg-info/requires.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        8 2023-04-15 12:36:12.000000 edamame-0.47/edamame.egg-info/top_level.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      803 2023-04-15 12:30:43.000000 edamame-0.47/pyproject.toml
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-04-15 12:36:12.813556 edamame-0.47/setup.cfg
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-16 11:18:01.680333 edamame-0.48/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1073 2022-11-30 14:22:32.000000 edamame-0.48/LICENSE
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     9914 2023-04-16 11:18:01.679942 edamame-0.48/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     8160 2023-04-16 11:15:56.000000 edamame-0.48/README.md
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-16 11:18:01.674570 edamame-0.48/edamame/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       21 2023-04-16 10:34:05.000000 edamame-0.48/edamame/__init__.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-16 11:18:01.676720 edamame-0.48/edamame/classifier/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      127 2023-04-16 11:13:18.000000 edamame-0.48/edamame/classifier/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    21608 2023-04-16 11:09:39.000000 edamame-0.48/edamame/classifier/classification.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-16 11:18:01.678010 edamame-0.48/edamame/eda/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      860 2023-04-06 20:58:22.000000 edamame-0.48/edamame/eda/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    32458 2023-03-25 15:28:28.000000 edamame-0.48/edamame/eda/eda.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     3814 2023-03-25 15:57:39.000000 edamame-0.48/edamame/eda/tools.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-16 11:18:01.679391 edamame-0.48/edamame/regressor/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      189 2023-04-06 20:53:01.000000 edamame-0.48/edamame/regressor/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     8324 2023-04-02 09:56:35.000000 edamame-0.48/edamame/regressor/diagnose.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)    21388 2023-04-04 20:19:13.000000 edamame-0.48/edamame/regressor/regression.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-16 11:18:01.676041 edamame-0.48/edamame.egg-info/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     9914 2023-04-16 11:18:01.000000 edamame-0.48/edamame.egg-info/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      430 2023-04-16 11:18:01.000000 edamame-0.48/edamame.egg-info/SOURCES.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-04-16 11:18:01.000000 edamame-0.48/edamame.egg-info/dependency_links.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       83 2023-04-16 11:18:01.000000 edamame-0.48/edamame.egg-info/requires.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        8 2023-04-16 11:18:01.000000 edamame-0.48/edamame.egg-info/top_level.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      803 2023-04-16 10:34:00.000000 edamame-0.48/pyproject.toml
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-04-16 11:18:01.680423 edamame-0.48/setup.cfg
```

### Comparing `edamame-0.47/LICENSE` & `edamame-0.48/LICENSE`

 * *Files identical despite different names*

### Comparing `edamame-0.47/PKG-INFO` & `edamame-0.48/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edamame
-Version: 0.47
+Version: 0.48
 Summary: Exploratory data analysis tools
 Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -155,14 +155,20 @@
 * **random_forest**: Fits a random forest classification model to the training data.
 * **xgboost**: Fits an XGBoost classification model to the training data.
 * * **svm**: Fits an Support Vector classification model to the training data.
 * **auto_ml**: Uses AutoML to select the best model based on performance metrics.
 * **model_metrics**: Computes and prints the performance metrics for each trained model.
 * **save_model**: Saves the trained model to a file.
 
+After saving a model with the **save_model** method, we can upload the model using the **load_model** function of the eda module and evaluate its performance on new data using the **classifier_metrics** function.
+
+```python
+from edamame.classifier import classifier_metrics
+```
+
 <hr>
 
 ## Todos
 
 * Add the ClassifierDiagnose class to the classifier module.
 * Add the notebook for EDA in a classification problem to the edamame-notebook repository.
 * Add the notebook for training/diagnosing classification models to the edamame-notebook repository.
```

### Comparing `edamame-0.47/README.md` & `edamame-0.48/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -122,14 +122,20 @@
 * **random_forest**: Fits a random forest classification model to the training data.
 * **xgboost**: Fits an XGBoost classification model to the training data.
 * * **svm**: Fits an Support Vector classification model to the training data.
 * **auto_ml**: Uses AutoML to select the best model based on performance metrics.
 * **model_metrics**: Computes and prints the performance metrics for each trained model.
 * **save_model**: Saves the trained model to a file.
 
+After saving a model with the **save_model** method, we can upload the model using the **load_model** function of the eda module and evaluate its performance on new data using the **classifier_metrics** function.
+
+```python
+from edamame.classifier import classifier_metrics
+```
+
 <hr>
 
 ## Todos
 
 * Add the ClassifierDiagnose class to the classifier module.
 * Add the notebook for EDA in a classification problem to the edamame-notebook repository.
 * Add the notebook for training/diagnosing classification models to the edamame-notebook repository.
```

### Comparing `edamame-0.47/edamame/classifier/classification.py` & `edamame-0.48/edamame/classifier/classification.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#TODO - add SVM method
+#TODO - add classifier metrics function 
 
 import numpy as np
 import pandas as pd
 from  edamame.eda.tools import dataframe_review, dummy_control
 from sklearn.linear_model import LogisticRegression
 from sklearn.preprocessing import StandardScaler
 from sklearn.naive_bayes import GaussianNB
@@ -12,15 +12,15 @@
 from xgboost import XGBClassifier
 from sklearn.model_selection import GridSearchCV, KFold, cross_val_score
 from sklearn.metrics import confusion_matrix, classification_report
 import seaborn as sns
 import pickle
 from IPython.display import display, Markdown
 import matplotlib.pyplot as plt 
-from typing import Tuple, Literal, List
+from typing import Tuple, Literal, List, Union
 from sklearn.svm import SVC
 # pandas options
 pd.set_option('display.max_columns', None)
 pd.set_option('display.width', None)
 pd.set_option('display.max_colwidth', None)
 
 
@@ -84,15 +84,14 @@
             >>> classifier = TrainClassifier(X_train=X_train, y_train=y_train, X_test=X_test, y_test=y_test)
             >>> logistic = classifier.logistic()
         """
         logistic = LogisticRegression()
         logistic.fit(self.X_train, self.y_train.squeeze())
         # save the model in the instance attributes
         self.__logistic_fit = logistic
-        # return step 
         return self.__logistic_fit
 
 
     def gaussian_nb(self) -> GaussianNB:
         """
         Trains a Gaussian Naive Bayes classifier using the training data and returns the fitted model.
 
@@ -104,15 +103,14 @@
             >>> classifier = TrainClassifier(X_train=X_train, y_train=y_train, X_test=X_test, y_test=y_test)
             >>> nb = classifier.gaussian_nb()
         """
         gauss_nb = GaussianNB()
         gauss_nb.fit(self.X_train, self.y_train.squeeze())
         # save the model in the instance attributes
         self.__gaussian_nb_fit = gauss_nb
-        # return step 
         return self.__gaussian_nb_fit
 
 
     # ------------ #
     # KNN
     # ------------ #
     def knn(self, n_neighbors: Tuple[int, int, int] = (1, 50, 50), n_folds: int = 5) -> KNeighborsClassifier:
@@ -134,19 +132,18 @@
             >>> from edamame.classifier import TrainClassifier
             >>> classifier = TrainClassifier(X_train=X_train, y_train=y_train, X_test=X_test, y_test=y_test)
             >>> knn = classifier.knn(n_neighbors=(1,50,50), n_folds=3) 
         """
         n_n = np.linspace(n_neighbors[0], n_neighbors[1], n_neighbors[2]).astype(np.int32)
         knn = KNeighborsClassifier()
         tuned_parameters = [{"n_neighbors": n_n}]
-        reg_knn = GridSearchCV(knn, tuned_parameters, cv=n_folds, refit=True, verbose=0, scoring='accuracy')
-        reg_knn.fit(self.X_train, self.y_train.squeeze())
+        grid_knn = GridSearchCV(knn, tuned_parameters, cv=n_folds, refit=True, verbose=0, scoring='accuracy')
+        grid_knn.fit(self.X_train, self.y_train.squeeze())
         # save the model in the instance attributes
-        self.__knn_fit = reg_knn.best_estimator_
-        # return step 
+        self.__knn_fit = grid_knn.best_estimator_
         return self.__knn_fit
 
 
     def tree(self, alpha: Tuple[float, float, int] = (0., 0.001, 5), impurity: Tuple[float, float, int] = (0., 0.00001, 5), n_folds: int = 5) -> DecisionTreeClassifier:
         """
         Trains a decision tree classifier using the training data and returns the fitted model.
     
@@ -163,19 +160,18 @@
             >>> classifier = TrainClassifier(X_train=X_train, y_train=y_train, X_test=X_test, y_test=y_test)
             >>> tree = classifier.tree(alpha=(0., 0.001, 5), impurity=(0., 0.00001, 5), n_folds=3) 
         """
         alphas = np.linspace(alpha[0], alpha[1], alpha[2])
         impurities = np.linspace(impurity[0], impurity[1], impurity[2])
         tuned_parameters = [{"ccp_alpha": alphas, 'min_impurity_decrease': impurities}]
         tree = DecisionTreeClassifier() 
-        reg_tree = GridSearchCV(tree, tuned_parameters, cv=n_folds, refit=True, verbose=0, scoring='accuracy')
-        reg_tree.fit(self.X_train, self.y_train.squeeze())
+        grid_tree = GridSearchCV(tree, tuned_parameters, cv=n_folds, refit=True, verbose=0, scoring='accuracy')
+        grid_tree.fit(self.X_train, self.y_train.squeeze())
         # save the model in the instance attributes
-        self.__tree_fit = reg_tree.best_estimator_
-        # return step 
+        self.__tree_fit = grid_tree.best_estimator_
         return self.__tree_fit
 
 
     def random_forest(self, n_estimators: Tuple[int, int, int] = (50, 1000, 5), n_folds: int = 2) -> RandomForestClassifier:
         """
         Train a Random Forest classifier using the training data and return the fitted model.
 
@@ -190,19 +186,18 @@
             >>> from edamame.classifier import TrainClassifier
             >>> classifier = TrainClassifier(X_train=X_train, y_train=y_train, X_test=X_test, y_test=y_test)
             >>> rf = classifier.random_forest(n_estimators=(50, 1000, 5), n_folds=2) 
         """
         n_estimators = np.linspace(n_estimators[0], n_estimators[1], n_estimators[2]).astype(np.int16)
         tuned_parameters = [{"n_estimators": n_estimators}]
         random_forest = RandomForestClassifier(warm_start=True, n_jobs=-1)
-        reg_random_forest = GridSearchCV(random_forest, tuned_parameters, cv=n_folds, refit=True, verbose=0, scoring='accuracy')
-        reg_random_forest.fit(self.X_train, self.y_train.squeeze())
+        grid_random_forest = GridSearchCV(random_forest, tuned_parameters, cv=n_folds, refit=True, verbose=0, scoring='accuracy')
+        grid_random_forest.fit(self.X_train, self.y_train.squeeze())
         # save the model in the instance attributes
-        self.__random_forest_fit = reg_random_forest.best_estimator_
-        # return step 
+        self.__random_forest_fit = grid_random_forest.best_estimator_
         return self.__random_forest_fit
 
 
     def xgboost(self, n_estimators: Tuple[int, int, int] = (10, 100, 5), n_folds: int = 2) -> XGBClassifier:
         """
         Train an XGBoost classifier using the training data and return the fitted model.
 
@@ -217,42 +212,45 @@
             >>> from edamame.classifier import TrainClassifier
             >>> classifier = TrainClassifier(X_train=X_train, y_train=y_train, X_test=X_test, y_test=y_test)
             >>> xgboost = classifier.xgboost(n_estimators=(10, 100, 5), n_folds=2) 
         """
         n_est = np.linspace(n_estimators[0], n_estimators[1], n_estimators[2]).astype(np.int16)
         tuned_parameters = {"n_estimators": n_est}
         xgb_m = XGBClassifier()
-        reg_xgb = GridSearchCV(xgb_m, tuned_parameters, cv=n_folds, refit=True, verbose=0, scoring='accuracy')
-        reg_xgb.fit(self.X_train, self.y_train.squeeze())
+        grid_xgb = GridSearchCV(xgb_m, tuned_parameters, cv=n_folds, refit=True, verbose=0, scoring='accuracy')
+        grid_xgb.fit(self.X_train, self.y_train.squeeze())
         # save the model in the instance attributes
-        self.__xgb_fit = reg_xgb.best_estimator_
-        # return step 
+        self.__xgb_fit = grid_xgb.best_estimator_
         return self.__xgb_fit
     
 
-    def svm(self, kernel: Literal["linear", "poly", "rbf", "sigmoid", "precomputed"] = "rbf", *args, **kwargs) -> SVC:
+    def svm(self, n_folds: int = 2, *args, **kwargs) -> SVC:
         """
         Trains an SVM classifier using the training data and returns the fitted model.
 
         Args:
-            kernel (Literal["linear", "poly", "rbf", "sigmoid", "precomputed"]): The kernel type to be used in the algorithm. Default is "rbf".
+            n_folds (int): The number of folds in cross-validation. Default is 2.
             *args: Variable length argument list to be passed to the `SVC` constructor.
             **kwargs: Arbitrary keyword arguments to be passed to the `SVC` constructor.
         
         Returns:
             SVC: The trained SVM classifier.
         
         Example: 
             >>> from edamame.classifier import TrainClassifier
             >>> classifier = TrainClassifier(X_train=X_train, y_train=y_train, X_test=X_test, y_test=y_test)
             >>> svm = classifier.svm(kernel="linear", C=1.0, gamma="auto")
         """
-        svm_c = SVC(kernel=kernel, *args, **kwargs)
-        svm_c.fit(self.X_train, self.y_train.squeeze())
-        self.__svm_fit = svm_c
+        n_kernel = ["linear", "poly", "rbf", "sigmoid"] 
+        tuned_parameters = {"kernel": n_kernel}
+        svm_c = SVC(*args, **kwargs)
+        grid_svm_c = GridSearchCV(svm_c, tuned_parameters, cv=n_folds, refit=True, verbose=0, scoring='accuracy')
+        grid_svm_c.fit(self.X_train, self.y_train.squeeze())
+        # save the model in the instance attributes
+        self.__svm_fit = grid_svm_c.best_estimator_
         return self.__svm_fit
 
 
     def model_metrics(self, model_name: Literal["all", "logistic", "guassian_nb", "knn", "tree", "random_forest", "xgboost", "svm"] = 'all') -> None:
         """
         Display classification metrics (confusion matrix and classification report) for specified or all trained models.
 
@@ -298,15 +296,15 @@
                 display(f'unable to show {model_name} model metrics')
             else:
                 title = f'### {model_name} model metrics:'
                 display(Markdown(title))
                 y_pred_train = model_list[model_dct[model_name]].predict(self.X_train)
                 y_pred_test = model_list[model_dct[model_name]].predict(self.X_test)
                 plt.figure(figsize=(10,4))
-                # plt.subplot(121)
+                plt.subplot(121)
                 sns.heatmap(confusion_matrix(self.y_train, y_pred_train), annot=True, fmt="2.0f")
                 plt.title(f'{model_name} train')
                 plt.subplot(122)
                 sns.heatmap(confusion_matrix(self.y_test, y_pred_test), annot=True, fmt="2.0f")
                 plt.title(f'{model_name} test')
                 plt.show()
                 title = f'#### Train classification report'
@@ -349,20 +347,21 @@
             # find best hyperparameters
             self.logistic()
             self.gaussian_nb()
             self.knn()
             self.tree()
             self.random_forest()
             self.xgboost()
+            self.svm()
             # model list 
             model_list = [LogisticRegression(), GaussianNB(), KNeighborsClassifier(n_neighbors=self.__knn_fit.n_neighbors),
                           DecisionTreeClassifier(ccp_alpha=self.__tree_fit.ccp_alpha, min_impurity_decrease=self.__tree_fit.min_impurity_decrease),
                           RandomForestClassifier(n_estimators = self.__random_forest_fit.n_estimators, warm_start=True, n_jobs=-1),
                           XGBClassifier(n_estimators = self.__xgb_fit.n_estimators),
-                          SVC()]
+                          SVC(kernel=self.__svm_fit.kernel)]
         # cross validation loop 
         for model in model_list:
             if data == 'train':
                 cv_result = cross_val_score(model, self.X_train, self.y_train.squeeze(), cv=kfold, scoring="accuracy")
             elif data == 'test':
                 cv_result = cross_val_score(model, self.X_test, self.y_test.squeeze(), cv=kfold, scoring="accuracy")
             else:
@@ -416,8 +415,32 @@
         else:
             if model_list[model_dct[model_name]].__class__.__name__ == 'dict':
                 display(f'unable to save {model_name} model')
             else:
                 filename = f'{model_name}.pkl'
                 with open(filename, 'wb') as file:
                     pickle.dump(model_list[model_dct[model_name]], file)
+
+
+
+def classifier_metrics(model: Union[LogisticRegression, GaussianNB, KNeighborsClassifier, DecisionTreeClassifier, RandomForestClassifier, XGBClassifier, SVC], X: pd.DataFrame, y: pd.DataFrame) -> None:
+    """
+    Display classification metrics (confusion matrix and classification report) for the model passed as input to the function.
+
+    Args:
+        model (Union[LogisticRegression, GaussianNB, KNeighborsClassifier, DecisionTreeClassifier, RandomForestClassifier, XGBClassifier, SVC]): Classification model.
+        X (pd.DataFrame): Input features.
+        y (pd.DataFrame): Target feature.
+    
+    Returns:
+        None
+    """
+    dataframe_review(X)
+    dummy_control(X)
+    y_pred = model.predict(X)
+    title = f'#### Model metrics:'
+    display(Markdown(title))
+    sns.heatmap(confusion_matrix(y, y_pred), annot=True, fmt="2.0f")
+    plt.show()
+    print(classification_report(y, y_pred))
+
```

### Comparing `edamame-0.47/edamame/eda/__init__.py` & `edamame-0.48/edamame/eda/__init__.py`

 * *Files identical despite different names*

### Comparing `edamame-0.47/edamame/eda/eda.py` & `edamame-0.48/edamame/eda/eda.py`

 * *Files identical despite different names*

### Comparing `edamame-0.47/edamame/eda/tools.py` & `edamame-0.48/edamame/eda/tools.py`

 * *Files identical despite different names*

### Comparing `edamame-0.47/edamame/regressor/diagnose.py` & `edamame-0.48/edamame/regressor/diagnose.py`

 * *Files identical despite different names*

### Comparing `edamame-0.47/edamame/regressor/regression.py` & `edamame-0.48/edamame/regressor/regression.py`

 * *Files identical despite different names*

### Comparing `edamame-0.47/edamame.egg-info/PKG-INFO` & `edamame-0.48/edamame.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edamame
-Version: 0.47
+Version: 0.48
 Summary: Exploratory data analysis tools
 Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -155,14 +155,20 @@
 * **random_forest**: Fits a random forest classification model to the training data.
 * **xgboost**: Fits an XGBoost classification model to the training data.
 * * **svm**: Fits an Support Vector classification model to the training data.
 * **auto_ml**: Uses AutoML to select the best model based on performance metrics.
 * **model_metrics**: Computes and prints the performance metrics for each trained model.
 * **save_model**: Saves the trained model to a file.
 
+After saving a model with the **save_model** method, we can upload the model using the **load_model** function of the eda module and evaluate its performance on new data using the **classifier_metrics** function.
+
+```python
+from edamame.classifier import classifier_metrics
+```
+
 <hr>
 
 ## Todos
 
 * Add the ClassifierDiagnose class to the classifier module.
 * Add the notebook for EDA in a classification problem to the edamame-notebook repository.
 * Add the notebook for training/diagnosing classification models to the edamame-notebook repository.
```

### Comparing `edamame-0.47/pyproject.toml` & `edamame-0.48/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "edamame"
-version = "0.47"
+version = "0.48"
 authors = [
   { name="Marco Salvalaggio", email="mar.salvalaggio@gmail.com" },
 ]
 description = "Exploratory data analysis tools"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

