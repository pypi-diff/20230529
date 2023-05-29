# Comparing `tmp/protloc_mex1-0.0.5.tar.gz` & `tmp/protloc_mex1-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protloc_mex1-0.0.5.tar", last modified: Mon May 15 11:12:08 2023, max compression
+gzip compressed data, was "protloc_mex1-0.0.6.tar", last modified: Mon May 29 12:50:26 2023, max compression
```

## Comparing `protloc_mex1-0.0.5.tar` & `protloc_mex1-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 11:12:08.679195 protloc_mex1-0.0.5/
--rw-rw-rw-   0        0        0     1091 2023-04-25 08:38:35.000000 protloc_mex1-0.0.5/LICENSE.txt
--rw-rw-rw-   0        0        0     7733 2023-05-15 11:12:08.678632 protloc_mex1-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     6953 2023-05-15 09:50:59.000000 protloc_mex1-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 11:12:08.610279 protloc_mex1-0.0.5/protloc_mex1/
--rw-rw-rw-   0        0        0    14498 2023-05-15 08:52:22.000000 protloc_mex1-0.0.5/protloc_mex1/AA_count.py
--rw-rw-rw-   0        0        0     8014 2023-04-29 12:40:52.000000 protloc_mex1-0.0.5/protloc_mex1/GO_count.py
--rw-rw-rw-   0        0        0    10510 2023-04-28 13:10:04.000000 protloc_mex1-0.0.5/protloc_mex1/SHAP_conduct.py
--rw-rw-rw-   0        0        0    31630 2023-05-11 12:52:32.000000 protloc_mex1-0.0.5/protloc_mex1/SHAP_plus.py
--rw-rw-rw-   0        0        0       39 2023-04-29 12:25:34.000000 protloc_mex1-0.0.5/protloc_mex1/__init__.py
--rw-rw-rw-   0        0        0    10886 2023-05-09 03:16:02.000000 protloc_mex1-0.0.5/protloc_mex1/classifier_evalute.py
-drwxrwxrwx   0        0        0        0 2023-05-15 11:12:08.675013 protloc_mex1-0.0.5/protloc_mex1.egg-info/
--rw-rw-rw-   0        0        0     7733 2023-05-15 11:12:08.000000 protloc_mex1-0.0.5/protloc_mex1.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      380 2023-05-15 11:12:08.000000 protloc_mex1-0.0.5/protloc_mex1.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 11:12:08.000000 protloc_mex1-0.0.5/protloc_mex1.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       91 2023-05-15 11:12:08.000000 protloc_mex1-0.0.5/protloc_mex1.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-15 11:12:08.000000 protloc_mex1-0.0.5/protloc_mex1.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      859 2023-05-15 11:01:00.000000 protloc_mex1-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-15 11:12:08.679195 protloc_mex1-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-29 12:50:26.504173 protloc_mex1-0.0.6/
+-rw-rw-rw-   0        0        0     1091 2023-04-25 08:38:35.000000 protloc_mex1-0.0.6/LICENSE.txt
+-rw-rw-rw-   0        0        0     7733 2023-05-29 12:50:26.502142 protloc_mex1-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     6953 2023-05-15 09:50:59.000000 protloc_mex1-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-29 12:50:26.454728 protloc_mex1-0.0.6/protloc_mex1/
+-rw-rw-rw-   0        0        0    14498 2023-05-15 08:52:22.000000 protloc_mex1-0.0.6/protloc_mex1/AA_count.py
+-rw-rw-rw-   0        0        0     8014 2023-04-29 12:40:52.000000 protloc_mex1-0.0.6/protloc_mex1/GO_count.py
+-rw-rw-rw-   0        0        0    10510 2023-04-28 13:10:04.000000 protloc_mex1-0.0.6/protloc_mex1/SHAP_conduct.py
+-rw-rw-rw-   0        0        0    31630 2023-05-11 12:52:32.000000 protloc_mex1-0.0.6/protloc_mex1/SHAP_plus.py
+-rw-rw-rw-   0        0        0       39 2023-04-29 12:25:34.000000 protloc_mex1-0.0.6/protloc_mex1/__init__.py
+-rw-rw-rw-   0        0        0    11881 2023-05-29 07:53:14.000000 protloc_mex1-0.0.6/protloc_mex1/classifier_evalute.py
+drwxrwxrwx   0        0        0        0 2023-05-29 12:50:26.501136 protloc_mex1-0.0.6/protloc_mex1.egg-info/
+-rw-rw-rw-   0        0        0     7733 2023-05-29 12:50:26.000000 protloc_mex1-0.0.6/protloc_mex1.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      380 2023-05-29 12:50:26.000000 protloc_mex1-0.0.6/protloc_mex1.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 12:50:26.000000 protloc_mex1-0.0.6/protloc_mex1.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       91 2023-05-29 12:50:26.000000 protloc_mex1-0.0.6/protloc_mex1.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-29 12:50:26.000000 protloc_mex1-0.0.6/protloc_mex1.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      859 2023-05-29 12:48:21.000000 protloc_mex1-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-29 12:50:26.504173 protloc_mex1-0.0.6/setup.cfg
```

### Comparing `protloc_mex1-0.0.5/LICENSE.txt` & `protloc_mex1-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `protloc_mex1-0.0.5/PKG-INFO` & `protloc_mex1-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protloc_mex1
-Version: 0.0.5
+Version: 0.0.6
 Summary: ...
 Author-email: Ze Yu Luo <1024226968@qq.com>
 Project-URL: Homepage, https://github.com/yujuan-zhang/ProtLoc-mexl
 Project-URL: Bug Tracker, https://github.com/yujuan-zhang/ProtLoc-mexl/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `protloc_mex1-0.0.5/README.md` & `protloc_mex1-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `protloc_mex1-0.0.5/protloc_mex1/AA_count.py` & `protloc_mex1-0.0.6/protloc_mex1/AA_count.py`

 * *Files identical despite different names*

### Comparing `protloc_mex1-0.0.5/protloc_mex1/GO_count.py` & `protloc_mex1-0.0.6/protloc_mex1/GO_count.py`

 * *Files identical despite different names*

### Comparing `protloc_mex1-0.0.5/protloc_mex1/SHAP_conduct.py` & `protloc_mex1-0.0.6/protloc_mex1/SHAP_conduct.py`

 * *Files identical despite different names*

### Comparing `protloc_mex1-0.0.5/protloc_mex1/SHAP_plus.py` & `protloc_mex1-0.0.6/protloc_mex1/SHAP_plus.py`

 * *Files identical despite different names*

### Comparing `protloc_mex1-0.0.5/protloc_mex1/classifier_evalute.py` & `protloc_mex1-0.0.6/protloc_mex1/classifier_evalute.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 try:
     import sklearn
     if version.parse(sklearn.__version__) < version.parse('1.0.2'):
         warnings.warn("Your sklearn version is older than 1.0.2 and may not operate correctly.")
     from sklearn.metrics import roc_curve, auc, confusion_matrix
     from sklearn.metrics import classification_report, accuracy_score, roc_auc_score
+    from sklearn.metrics import matthews_corrcoef
 except ImportError:
     warnings.warn("Sklearn not found. Some functions will not be available.")
 
 try:
     import mglearn
 except ImportError:
     warnings.warn("Mglearn not found. Some functions will not be available.")
@@ -86,25 +87,43 @@
             y_true=pd.Series(self.self_obj.y_data).map(type_mapping)  #Sample actual values
             y_pred=self.self_obj.X_hat_data["predict"].map(type_mapping) #Model Predicted Values
             auc=roc_auc_score(y_true,y_pred)
             auc_save_data=pd.DataFrame({protein_class:["{:.5f}".format(auc)]},columns=[protein_class]
                                             ,index=['auc'])
             return(auc_save_data)
         
+        def mcc_calculate(self, protein_class):
+            type_mapping = {}
+            for value in self.self_obj.type_class:
+                if value != protein_class:
+                    type_mapping[value] = 0
+                else:
+                    type_mapping[value] = 1
+            y_true = pd.Series(self.self_obj.y_data).map(type_mapping)  # Sample actual values
+            y_pred = self.self_obj.X_hat_data["predict"].map(type_mapping) # Model Predicted Values
+            mcc = matthews_corrcoef(y_true, y_pred)
+            mcc_save_data = pd.DataFrame({protein_class: ["{:.5f}".format(mcc)]}, columns=[protein_class], index=['mcc'])
+            return mcc_save_data
+    
+        
         def plot(self,save_path,file_name):
             
             ##accuracy
             accuracy_save_list=list(map(lambda x:self.accuracy_calculate(x),self.self_obj.type_class))
             accuracy_save_data=reduce(lambda x,y:pd.concat([x,y],axis=1),accuracy_save_list)
             ##auc
             auc_save_list=list(map(lambda x:self.auc_calculate(x),self.self_obj.type_class))
             auc_save_data=reduce(lambda x,y:pd.concat([x,y],axis=1),auc_save_list)
+            ##mcc
+            mcc_save_list = list(map(lambda x: self.mcc_calculate(x), self.self_obj.type_class))
+            mcc_save_data = reduce(lambda x, y: pd.concat([x, y], axis=1), mcc_save_list)
+
             ## Merging and save accuracy and auc
-            accuracy_auc_outcome=pd.concat([accuracy_save_data,auc_save_data],axis=0)
-            accuracy_auc_outcome.to_csv(save_path+file_name+'_classification_report2.csv',index_label='index')
+            accuracy_auc_mcc_outcome=pd.concat([accuracy_save_data,auc_save_data,mcc_save_data],axis=0)
+            accuracy_auc_mcc_outcome.to_csv(save_path+file_name+'_classification_report2.csv',index_label='index')
             ## Save f1, recall, precision
             test_class_report=classification_report(self.self_obj.y_data, 
                                                     self.self_obj.X_hat_data["predict"].to_numpy(),
                                                     output_dict=True)
             ## Save test set results
             test_class_report_save=dict()
             for i in self.self_obj.type_class.tolist():
```

### Comparing `protloc_mex1-0.0.5/protloc_mex1.egg-info/PKG-INFO` & `protloc_mex1-0.0.6/protloc_mex1.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protloc-mex1
-Version: 0.0.5
+Version: 0.0.6
 Summary: ...
 Author-email: Ze Yu Luo <1024226968@qq.com>
 Project-URL: Homepage, https://github.com/yujuan-zhang/ProtLoc-mexl
 Project-URL: Bug Tracker, https://github.com/yujuan-zhang/ProtLoc-mexl/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `protloc_mex1-0.0.5/pyproject.toml` & `protloc_mex1-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "protloc_mex1"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Ze Yu Luo", email="1024226968@qq.com" },
 ]
 description = "..."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

