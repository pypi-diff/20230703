# Comparing `tmp/TimeMurmur-0.1.1-py3-none-any.whl.zip` & `tmp/TimeMurmur-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 27524 bytes, number of entries: 26
--rw-rw-rw-  2.0 fat     3191 b- defN 23-Apr-20 15:15 TimeMurmur/Model.py
--rw-rw-rw-  2.0 fat    21726 b- defN 23-Jun-21 21:38 TimeMurmur/Murmur.py
+Zip file size: 27625 bytes, number of entries: 26
+-rw-rw-rw-  2.0 fat     3192 b- defN 23-Jul-03 14:39 TimeMurmur/Model.py
+-rw-rw-rw-  2.0 fat    21728 b- defN 23-Jul-03 14:41 TimeMurmur/Murmur.py
 -rw-rw-rw-  2.0 fat     3311 b- defN 22-Nov-26 15:26 TimeMurmur/Optimizer.py
 -rw-rw-rw-  2.0 fat       27 b- defN 22-Oct-05 13:30 TimeMurmur/__init__.py
 -rw-rw-rw-  2.0 fat     1785 b- defN 22-Dec-11 16:37 TimeMurmur/basis_functions/FourierBasisFunction.py
 -rw-rw-rw-  2.0 fat     2958 b- defN 23-Apr-13 17:23 TimeMurmur/basis_functions/LinearBasisFunction.py
 -rw-rw-rw-  2.0 fat       27 b- defN 22-Oct-05 13:30 TimeMurmur/basis_functions/__init__.py
 -rw-rw-rw-  2.0 fat     3295 b- defN 22-Oct-22 15:46 TimeMurmur/builder/BuildArAxis.py
 -rw-rw-rw-  2.0 fat      425 b- defN 22-Oct-05 13:30 TimeMurmur/builder/BuildHierarchy.py
@@ -16,13 +16,13 @@
 -rw-rw-rw-  2.0 fat     4057 b- defN 23-Apr-06 18:57 TimeMurmur/builder/PreProcess.py
 -rw-rw-rw-  2.0 fat     8422 b- defN 23-Apr-19 15:54 TimeMurmur/builder/Transformer.py
 -rw-rw-rw-  2.0 fat       27 b- defN 22-Oct-05 13:30 TimeMurmur/builder/__init__.py
 -rw-rw-rw-  2.0 fat     9607 b- defN 22-Oct-30 14:45 TimeMurmur/utils/FeatureExtraction.py
 -rw-rw-rw-  2.0 fat       27 b- defN 22-Oct-05 13:30 TimeMurmur/utils/__init__.py
 -rw-rw-rw-  2.0 fat     1184 b- defN 22-Oct-05 13:30 TimeMurmur/utils/series_utils.py
 -rw-rw-rw-  2.0 fat     3110 b- defN 23-Apr-06 18:18 TimeMurmur/utils/utility_functions.py
--rw-rw-rw-  2.0 fat     1088 b- defN 23-Jun-21 21:41 TimeMurmur-0.1.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     4715 b- defN 23-Jun-21 21:41 TimeMurmur-0.1.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-21 21:41 TimeMurmur-0.1.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-Jun-21 21:41 TimeMurmur-0.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     2279 b- defN 23-Jun-21 21:41 TimeMurmur-0.1.1.dist-info/RECORD
-26 files, 103697 bytes uncompressed, 23800 bytes compressed:  77.0%
+-rw-rw-rw-  2.0 fat     1088 b- defN 23-Jul-03 14:44 TimeMurmur-0.1.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     5090 b- defN 23-Jul-03 14:44 TimeMurmur-0.1.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-03 14:44 TimeMurmur-0.1.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Jul-03 14:44 TimeMurmur-0.1.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     2279 b- defN 23-Jul-03 14:44 TimeMurmur-0.1.2.dist-info/RECORD
+26 files, 104075 bytes uncompressed, 23901 bytes compressed:  77.0%
```

## zipnote {}

```diff
@@ -57,23 +57,23 @@
 
 Filename: TimeMurmur/utils/series_utils.py
 Comment: 
 
 Filename: TimeMurmur/utils/utility_functions.py
 Comment: 
 
-Filename: TimeMurmur-0.1.1.dist-info/LICENSE
+Filename: TimeMurmur-0.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: TimeMurmur-0.1.1.dist-info/METADATA
+Filename: TimeMurmur-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: TimeMurmur-0.1.1.dist-info/WHEEL
+Filename: TimeMurmur-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: TimeMurmur-0.1.1.dist-info/top_level.txt
+Filename: TimeMurmur-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: TimeMurmur-0.1.1.dist-info/RECORD
+Filename: TimeMurmur-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## TimeMurmur/Model.py

```diff
@@ -39,15 +39,15 @@
                                     'num_iterations': num_iterations,
                                     'alpha': alpha,
                                     'scale_pos_weights': scale_pos_weights,
                                     'is_unbalance': is_unbalance,
                                     'num_threads': num_threads
                                 }
         else:
-            self.boosted_params = boosting_params
+            self.boosting_params = boosting_params
             
     def build_model(self):
         if self.objective == 'regression' or self.objective == 'quantile' or self.objective == 'mape':
             model_obj = gbm.LGBMRegressor(**self.boosting_params)
         if self.objective == 'binary':
             model_obj = gbm.LGBMClassifier(**self.boosting_params)
         return model_obj
```

## TimeMurmur/Murmur.py

```diff
@@ -448,7 +448,8 @@
         plt.show()
 
     def plot_importance(self, **kwargs):
         import lightgbm as gbm
         gbm.plot_importance(self.model_obj, **kwargs)
 
 
+
```

## Comparing `TimeMurmur-0.1.1.dist-info/LICENSE` & `TimeMurmur-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `TimeMurmur-0.1.1.dist-info/METADATA` & `TimeMurmur-0.1.2.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TimeMurmur
-Version: 0.1.1
+Version: 0.1.2
 Summary: Time series forecasting at scale with LightGBM
 Author: Tyler Blume
 Author-email: tblume@mail.USF.edu
 Keywords: forecasting,time series,lightgbm
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -131,7 +131,20 @@
                     num_iterations=100,
                     learning_rate=.1,
                     num_leaves=31,
                     objective='quantile',
                     alpha=.9)
 predicted = murmur.predict(20)
 ```
+
+## Explanations with Shapley
+
+```
+#get shapley values of predictions
+predicted_shap_vals = murmur.explain_predictions(predicted)
+fitted_shap_vals = murmur.explain_fitted(fitted)
+#plot using shapley values
+murmur.plot_explanations(fitted_shap_vals=fitted_shap_vals,
+                         predicted_shap_vals=predicted_shap_vals,
+                         murmur_id=0)
+```
+
```

## Comparing `TimeMurmur-0.1.1.dist-info/RECORD` & `TimeMurmur-0.1.2.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-TimeMurmur/Model.py,sha256=fYwjBBDjsBsLoQj1XOmjXAVCDl1hLdWuR63pVp0M_VA,3191
-TimeMurmur/Murmur.py,sha256=5vkaunDpm00SIlfO6glhHBVCZFbOpNDWCfJz8BlWzLE,21726
+TimeMurmur/Model.py,sha256=zQ9ZKIsiqhpBiA7VXeJ80gB125rn8FUpAzYOTVhDbrU,3192
+TimeMurmur/Murmur.py,sha256=BfchOHrm6eDkZbmNsNO_3l2f7xyF-A7DKfpsVF9mHew,21728
 TimeMurmur/Optimizer.py,sha256=7sicRO2bVeLUCDX7ba8dhR7aNLcpgOwE1HHm6hRTNlQ,3311
 TimeMurmur/__init__.py,sha256=M9j1NuexsmXRO0O_LLRNrLF7fEfPAHWIxm90hC6gV3I,27
 TimeMurmur/basis_functions/FourierBasisFunction.py,sha256=Z5ONw7IN_HB6MnyEqm6aDLOnfMy4E72GTEr5yM7BAAA,1785
 TimeMurmur/basis_functions/LinearBasisFunction.py,sha256=A5NIV3kcRNm-rUIwcIPCtYPvtkgmHW4tw1xhsGIPmgw,2958
 TimeMurmur/basis_functions/__init__.py,sha256=M9j1NuexsmXRO0O_LLRNrLF7fEfPAHWIxm90hC6gV3I,27
 TimeMurmur/builder/BuildArAxis.py,sha256=2T8G8VqISOnl8sZ5TFqsrIgxqSjv-U1EUWW1WL9Wn2E,3295
 TimeMurmur/builder/BuildHierarchy.py,sha256=hvJfawGP3HsKI1527EMQp70uIkdE8K9FdTFWOxtsNGo,425
@@ -15,12 +15,12 @@
 TimeMurmur/builder/PreProcess.py,sha256=Epx9xiDAvvMYqb7qtrovYUB7f8u9bdsvw4Ve1Xusm3A,4057
 TimeMurmur/builder/Transformer.py,sha256=RRFMBuqVej9g7q5UU20d0lai1hKJV4fob8SUO4FZX2g,8422
 TimeMurmur/builder/__init__.py,sha256=M9j1NuexsmXRO0O_LLRNrLF7fEfPAHWIxm90hC6gV3I,27
 TimeMurmur/utils/FeatureExtraction.py,sha256=Pnre_KgFoQi5VrVyA6SH_JlJ4GCnfHtRNvCrjB-RePY,9607
 TimeMurmur/utils/__init__.py,sha256=M9j1NuexsmXRO0O_LLRNrLF7fEfPAHWIxm90hC6gV3I,27
 TimeMurmur/utils/series_utils.py,sha256=P153Yi_P4DhpjFPnIRJPfu6OYHT3pe7BUnHKHzdzfWk,1184
 TimeMurmur/utils/utility_functions.py,sha256=ie1pRCLwSijQJS_MoY8J7BcgExmh809aVtWNDSkJYWs,3110
-TimeMurmur-0.1.1.dist-info/LICENSE,sha256=PKTFxJnxvWRgz1XsBhnki8iKznsV6TFyR305UdmXoeY,1088
-TimeMurmur-0.1.1.dist-info/METADATA,sha256=BhVLrdUBtviXM72bQNS2IKQlMZctV1ra4oCFItwdOMk,4715
-TimeMurmur-0.1.1.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-TimeMurmur-0.1.1.dist-info/top_level.txt,sha256=P2PDgK20ZHd9EywUDWXFr6a1710Uc0hiGLEtHGdaXhk,11
-TimeMurmur-0.1.1.dist-info/RECORD,,
+TimeMurmur-0.1.2.dist-info/LICENSE,sha256=PKTFxJnxvWRgz1XsBhnki8iKznsV6TFyR305UdmXoeY,1088
+TimeMurmur-0.1.2.dist-info/METADATA,sha256=Hpx5ae1BsVNV1S-z4uIFgkJ7KXlu5U9RerzbcH2s4G8,5090
+TimeMurmur-0.1.2.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+TimeMurmur-0.1.2.dist-info/top_level.txt,sha256=P2PDgK20ZHd9EywUDWXFr6a1710Uc0hiGLEtHGdaXhk,11
+TimeMurmur-0.1.2.dist-info/RECORD,,
```

