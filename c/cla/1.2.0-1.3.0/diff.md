# Comparing `tmp/cla-1.2.0.tar.gz` & `tmp/cla-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cla-1.2.0.tar", last modified: Sat Jul  1 13:55:28 2023, max compression
+gzip compressed data, was "cla-1.3.0.tar", last modified: Mon Jul  3 03:16:29 2023, max compression
```

## Comparing `cla-1.2.0.tar` & `cla-1.3.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 13:55:28.127403 cla-1.2.0/
--rw-rw-rw-   0        0        0      234 2022-01-07 07:11:13.000000 cla-1.2.0/LICENCE
--rw-rw-rw-   0        0        0      145 2022-11-03 12:37:32.000000 cla-1.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4563 2023-07-01 13:55:28.126402 cla-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     4267 2022-11-13 04:14:25.000000 cla-1.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-01 13:55:27.652528 cla-1.2.0/cla/
--rw-rw-rw-   0        0        0       76 2022-12-27 01:47:03.000000 cla-1.2.0/cla/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-01 13:55:27.888924 cla-1.2.0/cla/gui/
--rw-rw-rw-   0        0        0      971 2023-03-30 15:07:52.000000 cla-1.2.0/cla/gui/9555d1e5-ccaf-45ba-910e-ceb0d7d31234.csv
--rw-rw-rw-   0        0        0        0 2022-01-07 02:28:31.000000 cla-1.2.0/cla/gui/__init__.py
--rw-rw-rw-   0        0        0     3624 2023-03-30 15:03:49.000000 cla-1.2.0/cla/gui/run.py
--rw-rw-rw-   0        0        0     1274 2023-03-30 15:06:16.000000 cla-1.2.0/cla/gui/sample.csv
-drwxrwxrwx   0        0        0        0 2023-07-01 13:55:28.079404 cla-1.2.0/cla/gui/static/
--rw-rw-rw-   0        0        0        0 2022-01-07 02:28:31.000000 cla-1.2.0/cla/gui/static/__init__.py
--rw-rw-rw-   0        0        0   192352 2020-09-09 05:39:36.000000 cla-1.2.0/cla/gui/static/bootstrap.css
--rw-rw-rw-   0        0        0   131637 2020-02-15 01:34:39.000000 cla-1.2.0/cla/gui/static/bootstrap.js
--rw-rw-rw-   0        0        0    86927 2020-02-15 01:36:15.000000 cla-1.2.0/cla/gui/static/jquery-3.3.1.min.js
--rw-rw-rw-   0        0        0    24228 2020-02-15 04:11:19.000000 cla-1.2.0/cla/gui/static/jquery.blockUI.js
--rw-rw-rw-   0        0        0    17108 2020-02-15 04:11:19.000000 cla-1.2.0/cla/gui/static/jquery.form.min.js
--rw-rw-rw-   0        0        0      971 2021-04-27 11:05:37.000000 cla-1.2.0/cla/gui/static/sample.csv
-drwxrwxrwx   0        0        0        0 2023-07-01 13:55:28.106402 cla-1.2.0/cla/gui/templates/
--rw-rw-rw-   0        0        0        0 2022-11-03 12:58:21.000000 cla-1.2.0/cla/gui/templates/__init__.py
--rw-rw-rw-   0        0        0    12788 2022-11-10 06:20:55.000000 cla-1.2.0/cla/gui/templates/home.html
--rw-rw-rw-   0        0        0    79954 2023-07-01 02:23:52.000000 cla-1.2.0/cla/metrics.py
--rw-rw-rw-   0        0        0    15933 2023-02-16 05:23:58.000000 cla-1.2.0/cla/unify.py
-drwxrwxrwx   0        0        0        0 2023-07-01 13:55:28.121405 cla-1.2.0/cla/vis/
--rw-rw-rw-   0        0        0      124 2022-10-23 07:38:04.000000 cla-1.2.0/cla/vis/__init__.py
--rw-rw-rw-   0        0        0     6471 2023-06-28 15:04:04.000000 cla-1.2.0/cla/vis/confusion_matrix.py
--rw-rw-rw-   0        0        0     2429 2023-03-15 01:19:58.000000 cla-1.2.0/cla/vis/feature_importance.py
--rw-rw-rw-   0        0        0     1342 2022-12-27 01:48:57.000000 cla-1.2.0/cla/vis/plotComponents1D.py
--rw-rw-rw-   0        0        0     1848 2022-12-27 01:49:48.000000 cla-1.2.0/cla/vis/plotComponents2D.py
--rw-rw-rw-   0        0        0     1103 2022-12-27 01:49:57.000000 cla-1.2.0/cla/vis/plotComponents3D.py
--rw-rw-rw-   0        0        0      387 2022-12-27 01:51:06.000000 cla-1.2.0/cla/vis/plt2base64.py
--rw-rw-rw-   0        0        0     4953 2023-06-28 11:18:59.000000 cla-1.2.0/cla/vis/unsupervised_dimension_reductions.py
-drwxrwxrwx   0        0        0        0 2023-07-01 13:55:27.868901 cla-1.2.0/cla.egg-info/
--rw-rw-rw-   0        0        0     4563 2023-07-01 13:55:27.000000 cla-1.2.0/cla.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      849 2023-07-01 13:55:27.000000 cla-1.2.0/cla.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 13:55:27.000000 cla-1.2.0/cla.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       91 2023-07-01 13:55:27.000000 cla-1.2.0/cla.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-01 13:55:27.000000 cla-1.2.0/cla.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-01 13:55:28.125401 cla-1.2.0/data/
--rw-rw-rw-   0        0        0      971 2022-01-07 07:13:50.000000 cla-1.2.0/data/sample.csv
--rw-rw-rw-   0        0        0      108 2022-01-07 07:21:30.000000 cla-1.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-01 13:55:28.128403 cla-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1290 2023-06-30 14:07:35.000000 cla-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 03:16:29.112553 cla-1.3.0/
+-rw-rw-rw-   0        0        0      234 2022-01-07 07:11:13.000000 cla-1.3.0/LICENCE
+-rw-rw-rw-   0        0        0      145 2022-11-03 12:37:32.000000 cla-1.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4563 2023-07-03 03:16:29.110554 cla-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4267 2022-11-13 04:14:25.000000 cla-1.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-03 03:16:29.025015 cla-1.3.0/cla/
+-rw-rw-rw-   0        0        0       76 2022-12-27 01:47:03.000000 cla-1.3.0/cla/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 03:16:29.063548 cla-1.3.0/cla/gui/
+-rw-rw-rw-   0        0        0      971 2023-03-30 15:07:52.000000 cla-1.3.0/cla/gui/9555d1e5-ccaf-45ba-910e-ceb0d7d31234.csv
+-rw-rw-rw-   0        0        0        0 2022-01-07 02:28:31.000000 cla-1.3.0/cla/gui/__init__.py
+-rw-rw-rw-   0        0        0     3624 2023-03-30 15:03:49.000000 cla-1.3.0/cla/gui/run.py
+-rw-rw-rw-   0        0        0     1274 2023-03-30 15:06:16.000000 cla-1.3.0/cla/gui/sample.csv
+drwxrwxrwx   0        0        0        0 2023-07-03 03:16:29.081553 cla-1.3.0/cla/gui/static/
+-rw-rw-rw-   0        0        0        0 2022-01-07 02:28:31.000000 cla-1.3.0/cla/gui/static/__init__.py
+-rw-rw-rw-   0        0        0   192352 2020-09-09 05:39:36.000000 cla-1.3.0/cla/gui/static/bootstrap.css
+-rw-rw-rw-   0        0        0   131637 2020-02-15 01:34:39.000000 cla-1.3.0/cla/gui/static/bootstrap.js
+-rw-rw-rw-   0        0        0    86927 2020-02-15 01:36:15.000000 cla-1.3.0/cla/gui/static/jquery-3.3.1.min.js
+-rw-rw-rw-   0        0        0    24228 2020-02-15 04:11:19.000000 cla-1.3.0/cla/gui/static/jquery.blockUI.js
+-rw-rw-rw-   0        0        0    17108 2020-02-15 04:11:19.000000 cla-1.3.0/cla/gui/static/jquery.form.min.js
+-rw-rw-rw-   0        0        0      971 2021-04-27 11:05:37.000000 cla-1.3.0/cla/gui/static/sample.csv
+drwxrwxrwx   0        0        0        0 2023-07-03 03:16:29.087550 cla-1.3.0/cla/gui/templates/
+-rw-rw-rw-   0        0        0        0 2022-11-03 12:58:21.000000 cla-1.3.0/cla/gui/templates/__init__.py
+-rw-rw-rw-   0        0        0    12788 2022-11-10 06:20:55.000000 cla-1.3.0/cla/gui/templates/home.html
+-rw-rw-rw-   0        0        0    80432 2023-07-02 04:01:20.000000 cla-1.3.0/cla/metrics.py
+-rw-rw-rw-   0        0        0    15933 2023-02-16 05:23:58.000000 cla-1.3.0/cla/unify.py
+drwxrwxrwx   0        0        0        0 2023-07-03 03:16:29.106547 cla-1.3.0/cla/vis/
+-rw-rw-rw-   0        0        0      124 2022-10-23 07:38:04.000000 cla-1.3.0/cla/vis/__init__.py
+-rw-rw-rw-   0        0        0     6471 2023-06-28 15:04:04.000000 cla-1.3.0/cla/vis/confusion_matrix.py
+-rw-rw-rw-   0        0        0     2429 2023-03-15 01:19:58.000000 cla-1.3.0/cla/vis/feature_importance.py
+-rw-rw-rw-   0        0        0     1342 2022-12-27 01:48:57.000000 cla-1.3.0/cla/vis/plotComponents1D.py
+-rw-rw-rw-   0        0        0     1848 2022-12-27 01:49:48.000000 cla-1.3.0/cla/vis/plotComponents2D.py
+-rw-rw-rw-   0        0        0     1103 2022-12-27 01:49:57.000000 cla-1.3.0/cla/vis/plotComponents3D.py
+-rw-rw-rw-   0        0        0      387 2022-12-27 01:51:06.000000 cla-1.3.0/cla/vis/plt2base64.py
+-rw-rw-rw-   0        0        0     4953 2023-06-28 11:18:59.000000 cla-1.3.0/cla/vis/unsupervised_dimension_reductions.py
+drwxrwxrwx   0        0        0        0 2023-07-03 03:16:29.053547 cla-1.3.0/cla.egg-info/
+-rw-rw-rw-   0        0        0     4563 2023-07-03 03:16:28.000000 cla-1.3.0/cla.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      849 2023-07-03 03:16:28.000000 cla-1.3.0/cla.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 03:16:28.000000 cla-1.3.0/cla.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       91 2023-07-03 03:16:28.000000 cla-1.3.0/cla.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-03 03:16:28.000000 cla-1.3.0/cla.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 03:16:29.108548 cla-1.3.0/data/
+-rw-rw-rw-   0        0        0      971 2022-01-07 07:13:50.000000 cla-1.3.0/data/sample.csv
+-rw-rw-rw-   0        0        0      108 2022-01-07 07:21:30.000000 cla-1.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-03 03:16:29.113549 cla-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1290 2023-07-03 03:15:54.000000 cla-1.3.0/setup.py
```

### Comparing `cla-1.2.0/PKG-INFO` & `cla-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cla
-Version: 1.2.0
+Version: 1.3.0
 Summary: An integrated Python toolkit for classifiability analysis.
 Home-page: http://pypi.python.org/pypi/cla/
 Author: Zhang
 Author-email: oo@zju.edu.cn
 License: LICENSE.txt
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cla Version: 1.2.0 Summary: An integrated Python
+Metadata-Version: 2.1 Name: cla Version: 1.3.0 Summary: An integrated Python
 toolkit for classifiability analysis. Home-page: http://pypi.python.org/pypi/
 cla/ Author: Zhang Author-email: oo@zju.edu.cn License: LICENSE.txt
 Description-Content-Type: text/markdown License-File: LICENCE # cla
 (classifiability analysis) A unified classifiability analysis framework based
 on meta-learner and its application in spectroscopic profiling data [J].
 Applied Intelligence, 2021, doi: 10.1007/s10489-021-02810-8 pyCLAMs: An
 integrated Python toolkit for classifiability analysis [J]. SoftwareX, Volume
```

### Comparing `cla-1.2.0/README.md` & `cla-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `cla-1.2.0/cla/gui/9555d1e5-ccaf-45ba-910e-ceb0d7d31234.csv` & `cla-1.3.0/cla/gui/9555d1e5-ccaf-45ba-910e-ceb0d7d31234.csv`

 * *Files identical despite different names*

### Comparing `cla-1.2.0/cla/gui/run.py` & `cla-1.3.0/cla/gui/run.py`

 * *Files identical despite different names*

### Comparing `cla-1.2.0/cla/gui/sample.csv` & `cla-1.3.0/cla/gui/sample.csv`

 * *Files identical despite different names*

### Comparing `cla-1.2.0/cla/gui/static/bootstrap.css` & `cla-1.3.0/cla/gui/static/bootstrap.css`

 * *Files identical despite different names*

### Comparing `cla-1.2.0/cla/gui/static/bootstrap.js` & `cla-1.3.0/cla/gui/static/bootstrap.js`

 * *Files identical despite different names*

### Comparing `cla-1.2.0/cla/gui/static/jquery-3.3.1.min.js` & `cla-1.3.0/cla/gui/static/jquery-3.3.1.min.js`

 * *Files identical despite different names*

### Comparing `cla-1.2.0/cla/gui/static/jquery.blockUI.js` & `cla-1.3.0/cla/gui/static/jquery.blockUI.js`

 * *Files identical despite different names*

### Comparing `cla-1.2.0/cla/gui/static/jquery.form.min.js` & `cla-1.3.0/cla/gui/static/jquery.form.min.js`

 * *Files identical despite different names*

### Comparing `cla-1.2.0/cla/gui/static/sample.csv` & `cla-1.3.0/cla/gui/static/sample.csv`

 * *Files identical despite different names*

### Comparing `cla-1.2.0/cla/gui/templates/home.html` & `cla-1.3.0/cla/gui/templates/home.html`

 * *Files identical despite different names*

### Comparing `cla-1.2.0/cla/metrics.py` & `cla-1.3.0/cla/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -2269,63 +2269,74 @@
     plt.xticks(rotation=90)
     plt.show()
 
     print("1st PC: ", PCs[:, 0])
 
     return pca
 
-def run_multiclass_clfs(X, y, split = .3, show = True):
+def run_multiclass_clfs(X, y, clfs = 'all', split = .3, show = True):
     '''
+    Use grid search to train and evaluate various multi-class classifiers.
 
     原生支持多分类的模型：
 
     naive_bayes.BernoulliNB (only for binary features)
     tree.DecisionTreeClassifier
     ensemble.ExtraTreesClassifier (only in ensembles)
     naive_bayes.GaussianNB
     neighbors.KNeighborsClassifier
     discriminant_analysis.LinearDiscriminantAnalysis
     svm.LinearSVC (multi_class=”crammer_singer”)
     linear_model.LogisticRegression(CV) (multi_class=”multinomial”)
     neural_network.MLPClassifier
-    neighbors.NearestCentroid
     ensemble.RandomForestClassifier
     '''
 
     matplotlib.rcParams.update({'font.size': 17})
 
     n_classes = len(np.unique(y))
     X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=split, random_state = 2, stratify=y)
     dic_test_accs = {}
 
     html_str = ''
-    for clf in [GaussianNB(), DecisionTreeClassifier(), RandomForestClassifier(n_estimators=max(10, n_classes)), 
+    for base_learner, param_grid in zip( [GaussianNB(), DecisionTreeClassifier(), RandomForestClassifier(), 
                 LinearSVC(multi_class="crammer_singer"), LogisticRegressionCV (multi_class="multinomial", max_iter=1000), 
-                MLPClassifier(hidden_layer_sizes=(max(n_classes, X.shape[1]),)), 
-                KNeighborsClassifier(n_neighbors=max(5, n_classes)), 
-                NearestCentroid(), LinearDiscriminantAnalysis()]:
+                MLPClassifier(), 
+                KNeighborsClassifier(), # NearestCentroid(),
+                LinearDiscriminantAnalysis()], 
+                [{}, {'max_depth': [1,2,3,4,5,10,20]}, {'n_estimators': list(range(2, max(10, n_classes)))},
+                 {'C': [0.01, 0.1, 1, 10]}, {},
+                 {'hidden_layer_sizes': [(x,) for x in range(1, 102, 10)], 'alpha': [0.0001, 0.01, 1] },
+                  {'n_neighbors': list(range(1, max(5, n_classes)))}, 
+                  {}]):
         
+        if clfs != 'all' and str(base_learner) not in clfs:
+            continue
+
+        gs = GridSearchCV(base_learner, param_grid, cv= min(3,len(y_train)), n_jobs=-1, verbose=0)
+        gs.fit(X_train, y_train)
+
+        clf = gs.best_estimator_
         html_str += '<h4>' + str(clf) + '</h4>'
         if show:
             IPython.display.display(IPython.display.HTML('<h3>' + str(clf) + '</h3>'))
-                                
-        clf.fit(X_train, y_train)   
+
         y_pred = clf.predict(X_test) 
-        report = '<br/><pre>' + str(classification_report(y_test, y_pred)) + '</pre>'
-                
+        # report = '<br/><pre>' + str(classification_report(y_test, y_pred)) + '</pre>'
+        dic_test_accs[str(clf)] = [clf.score(X_test, y_test)]
+        report = '<p>top-1 acc = ' + str(round( clf.score(X_test, y_test), 3 )) + '</p>'        
+        
         if len(np.unique(y)) >= 8:
             # y_score = OneHotEncoder(categories = list( range(len(np.unique(y)))) ).fit_transform(y_pred.reshape(-1, 1))
             y_score = np.eye(n_classes)[y_pred] # one-hot encoding, make sure y is 0-indexed.
             if hasattr(clf, 'predict_proba') and callable(clf.predict_proba):
                 y_score = clf.predict_proba(X_test)
 
-            dic_test_accs[str(clf)] = [top_k_accuracy_score(y_test, y_score, k=1)] 
             dic_test_accs[str(clf)].append(top_k_accuracy_score(y_test, y_score, k=3))
             dic_test_accs[str(clf)].append(top_k_accuracy_score(y_test, y_score, k=5))
-            report += '<p>top-1 acc = ' + str(round( top_k_accuracy_score(y_test, y_score, k=1),3)) + '</p>'        
             report += '<p>top-3 acc = ' + str(round( top_k_accuracy_score(y_test, y_score, k=3),3)) + '</p>'
             report += '<p>top-5 acc = ' + str(round( top_k_accuracy_score(y_test, y_score, k=5),3)) + '</p>'
 
         if show:
             IPython.display.display(IPython.display.HTML(report)) 
         html_str += report
```

### Comparing `cla-1.2.0/cla/unify.py` & `cla-1.3.0/cla/unify.py`

 * *Files identical despite different names*

### Comparing `cla-1.2.0/cla/vis/confusion_matrix.py` & `cla-1.3.0/cla/vis/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `cla-1.2.0/cla/vis/feature_importance.py` & `cla-1.3.0/cla/vis/feature_importance.py`

 * *Files identical despite different names*

### Comparing `cla-1.2.0/cla/vis/plotComponents1D.py` & `cla-1.3.0/cla/vis/plotComponents1D.py`

 * *Files identical despite different names*

### Comparing `cla-1.2.0/cla/vis/plotComponents2D.py` & `cla-1.3.0/cla/vis/plotComponents2D.py`

 * *Files identical despite different names*

### Comparing `cla-1.2.0/cla/vis/plotComponents3D.py` & `cla-1.3.0/cla/vis/plotComponents3D.py`

 * *Files identical despite different names*

### Comparing `cla-1.2.0/cla/vis/unsupervised_dimension_reductions.py` & `cla-1.3.0/cla/vis/unsupervised_dimension_reductions.py`

 * *Files identical despite different names*

### Comparing `cla-1.2.0/cla.egg-info/PKG-INFO` & `cla-1.3.0/cla.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cla
-Version: 1.2.0
+Version: 1.3.0
 Summary: An integrated Python toolkit for classifiability analysis.
 Home-page: http://pypi.python.org/pypi/cla/
 Author: Zhang
 Author-email: oo@zju.edu.cn
 License: LICENSE.txt
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cla Version: 1.2.0 Summary: An integrated Python
+Metadata-Version: 2.1 Name: cla Version: 1.3.0 Summary: An integrated Python
 toolkit for classifiability analysis. Home-page: http://pypi.python.org/pypi/
 cla/ Author: Zhang Author-email: oo@zju.edu.cn License: LICENSE.txt
 Description-Content-Type: text/markdown License-File: LICENCE # cla
 (classifiability analysis) A unified classifiability analysis framework based
 on meta-learner and its application in spectroscopic profiling data [J].
 Applied Intelligence, 2021, doi: 10.1007/s10489-021-02810-8 pyCLAMs: An
 integrated Python toolkit for classifiability analysis [J]. SoftwareX, Volume
```

### Comparing `cla-1.2.0/cla.egg-info/SOURCES.txt` & `cla-1.3.0/cla.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cla-1.2.0/data/sample.csv` & `cla-1.3.0/data/sample.csv`

 * *Files identical despite different names*

### Comparing `cla-1.2.0/setup.py` & `cla-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 setup(
     # Application name:
     name="cla",
     
     # Version number (initial):
-    version="1.2.0",
+    version="1.3.0",
     
     # Application author details:
     author="Zhang",
     author_email="oo@zju.edu.cn",
     
     # Packages
     packages=["cla", "cla.vis", "cla.gui", "cla.gui.templates", "cla.gui.static"],
```

