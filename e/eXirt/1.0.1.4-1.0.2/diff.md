# Comparing `tmp/eXirt-1.0.1.4.tar.gz` & `tmp/eXirt-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eXirt-1.0.1.4.tar", last modified: Fri Mar  3 16:31:25 2023, max compression
+gzip compressed data, was "eXirt-1.0.2.tar", last modified: Mon May 29 20:29:54 2023, max compression
```

## Comparing `eXirt-1.0.1.4.tar` & `eXirt-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-03-03 16:31:25.684810 eXirt-1.0.1.4/
--rw-rw-rw-   0        0        0      215 2023-03-03 16:31:25.684810 eXirt-1.0.1.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-03-03 16:31:25.680808 eXirt-1.0.1.4/eXirt.egg-info/
--rw-rw-rw-   0        0        0      215 2023-03-03 16:31:25.000000 eXirt-1.0.1.4/eXirt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      197 2023-03-03 16:31:25.000000 eXirt-1.0.1.4/eXirt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-03 16:31:25.000000 eXirt-1.0.1.4/eXirt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-03-03 16:31:25.000000 eXirt-1.0.1.4/eXirt.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-03 16:31:25.683810 eXirt-1.0.1.4/pyexirt/
--rw-rw-rw-   0        0        0     7453 2023-01-23 16:20:18.000000 eXirt-1.0.1.4/pyexirt/decodIRT_MLtIRT.py
--rw-rw-rw-   0        0        0    34100 2023-01-23 16:20:18.000000 eXirt-1.0.1.4/pyexirt/decodIRT_analysis.py
--rw-rw-rw-   0        0        0    55080 2023-03-03 16:29:50.000000 eXirt-1.0.1.4/pyexirt/eXirt.py
--rw-rw-rw-   0        0        0       42 2023-03-03 16:31:25.685811 eXirt-1.0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      309 2023-03-03 16:30:29.000000 eXirt-1.0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 20:29:54.981755 eXirt-1.0.2/
+-rw-rw-rw-   0        0        0      213 2023-05-29 20:29:54.980754 eXirt-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-29 20:29:54.976754 eXirt-1.0.2/eXirt.egg-info/
+-rw-rw-rw-   0        0        0      213 2023-05-29 20:29:54.000000 eXirt-1.0.2/eXirt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2023-05-29 20:29:54.000000 eXirt-1.0.2/eXirt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 20:29:54.000000 eXirt-1.0.2/eXirt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-29 20:29:54.000000 eXirt-1.0.2/eXirt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-29 20:29:54.979754 eXirt-1.0.2/pyexirt/
+-rw-rw-rw-   0        0        0     7453 2023-01-23 16:20:18.000000 eXirt-1.0.2/pyexirt/decodIRT_MLtIRT.py
+-rw-rw-rw-   0        0        0    34100 2023-01-23 16:20:18.000000 eXirt-1.0.2/pyexirt/decodIRT_analysis.py
+-rw-rw-rw-   0        0        0    55313 2023-05-29 20:25:05.000000 eXirt-1.0.2/pyexirt/eXirt.py
+-rw-rw-rw-   0        0        0       42 2023-05-29 20:29:54.981755 eXirt-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      307 2023-05-29 20:28:27.000000 eXirt-1.0.2/setup.py
```

### Comparing `eXirt-1.0.1.4/pyexirt/decodIRT_MLtIRT.py` & `eXirt-1.0.2/pyexirt/decodIRT_MLtIRT.py`

 * *Files identical despite different names*

### Comparing `eXirt-1.0.1.4/pyexirt/decodIRT_analysis.py` & `eXirt-1.0.2/pyexirt/decodIRT_analysis.py`

 * *Files identical despite different names*

### Comparing `eXirt-1.0.1.4/pyexirt/eXirt.py` & `eXirt-1.0.2/pyexirt/eXirt.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,15 +146,15 @@
     # Properties of IRT
     self.irt_discriminate = True #False remove the property by IRTs calc.
     self.irt_difficulty = True #False remove the property by IRTs calc.
     self.irt_divine = True #False remove the property by IRTs calc.
 
     ################################## PROPOSAL 1 POOL #########################
     self.include_original_clf_data_pool = True
-    self.number_of_features_deletion = 2 # values 1 to ++
+    self.number_of_features_deletion = 1 # values 1 to ++
 
     self.list_clf_pool = [] #empity
 
     ################################## PROPOSAL 2 LOOP #########################
 
     self.include_original_clf_data_loop = True
     self.number_of_features_variation = 1 # values 1 to 4
@@ -213,14 +213,22 @@
 
   def run_prepare(self, model,data_exec_x, data_exec_y, X_train, X_test, y_train, y_test):
     if os.path.isfile(self.path_content+self.path_irt+self.bar+'tabela_base_para_executar_irt.csv'):
         os.remove(self.path_content+self.path_irt+self.bar+'tabela_base_para_executar_irt.csv')
     if os.path.isfile(self.path_content+self.path_irt+self.bar+'tabela_base_para_executar_irt_accuracy.csv'):
         os.remove(self.path_content+self.path_irt+self.bar+'tabela_base_para_executar_irt_accuracy.csv')
 
+    def compResponses(a,b):
+      c = []
+      for i,_ in enumerate(a):
+        if a[i] == b[i]:
+          c.append(1)
+        else:
+          c.append(0)
+      return c    
 
     #Prediction
     original_outputs = model.predict(data_exec_x)
 
 
     #XAI-IRT
     # train, test, model and outputs
@@ -253,16 +261,17 @@
         str_tmp = 'Clf original data'
         if self.exec_performance == self.exec_accuracy:
           result_accuracy = accuracy_score(y_true = original_outputs, y_pred = original_outputs, normalize=self.normalize_performance) #accuracy
         else:
           if self.exec_performance == self.exec_auc:
             result_accuracy = self.auc_score(original_outputs, original_outputs) #AUC
 
-        result_pred = (original_outputs == data_exec_y.values) #binarization
-        df_loop_of_models.loc[len(df_loop_of_models)] = result_pred.astype(int)[:].tolist().insert(0,str_tmp) #boolean to int
+        result_bin = compResponses(list(original_outputs), list(original_outputs))
+        result_bin.insert(0,str_tmp)
+        df_loop_of_models.loc[len(df_loop_of_models)] = result_bin
         df_loop_of_models_performance.loc[len(df_loop_of_models_performance)] = [str_tmp, result_accuracy] 
       
       #inset variation of ONE attribute in loop of models
       if self.number_of_features_variation >= 1:
         for _, variation in enumerate(self.exec_variation_method):
           for id,c in enumerate(data_exec_x.columns):
             #criando cópia do dado inicial
@@ -352,18 +361,20 @@
 
             if self.exec_performance == self.exec_accuracy:
               result_accuracy = accuracy_score(y_true = original_outputs, y_pred = result_pred, normalize=self.normalize_performance) #accuracy
             else:
               if self.exec_performance == self.exec_auc:
                 result_accuracy = self.auc_score(original_outputs, result_pred) #AUC
 
-            result_pred = (result_pred == original_outputs) #binarization
+            
             str_model_name = 'Clf '+method+' "'+str(c)+'"'
             self.list_clf_loop.append(str_model_name)
-            df_loop_of_models.loc[len(df_loop_of_models)] = result_pred.astype(int)[:].tolist().insert(0,str_model_name) #boolean to int
+            result_bin = compResponses(list(original_outputs), list(result_pred))
+            result_bin.insert(0,str_model_name)
+            df_loop_of_models.loc[len(df_loop_of_models)] = result_bin
             df_loop_of_models_performance.loc[len(df_loop_of_models_performance)] = [str_model_name, result_accuracy]
 
       #inset invertion of TWO attributes in loop of models
       if self.number_of_features_variation >= 2:
         for _,variation in enumerate(self.exec_variation_method):
           for id1,c1 in enumerate(data_exec_x.columns):
             for id2,c2 in enumerate(data_exec_x.columns):
@@ -478,18 +489,20 @@
 
                 if self.exec_performance == self.exec_accuracy:
                   result_accuracy = accuracy_score(y_true = original_outputs, y_pred = result_pred, normalize=self.normalize_performance) #accuracy
                 else:
                   if self.exec_performance == self.exec_auc:
                     result_accuracy = self.auc_score(original_outputs, result_pred) #AUC
 
-                result_pred = (result_pred == original_outputs) #binarization
+               
                 str_model_name = 'Clf '+method+' "'+str(c1)+'" and "'+str(c2)+'"'
                 self.list_clf_loop.append(str_model_name)
-                df_loop_of_models.loc[len(df_loop_of_models)] = result_pred.astype(int)[:].tolist().insert(0,str_model_name) #boolean to int
+                result_bin = compResponses(list(original_outputs), list(result_pred))
+                result_bin.insert(0,str_model_name)
+                df_loop_of_models.loc[len(df_loop_of_models)] = result_bin
                 df_loop_of_models_performance.loc[len(df_loop_of_models_performance)] = [str_model_name, result_accuracy]
               else:
                 pass
 
       #inset invertion of Three attributes in loop of models
       if self.number_of_features_variation >= 3:
         for _, variation in enumerate(self.exec_variation_method):
@@ -626,17 +639,19 @@
 
                   if self.exec_performance == self.exec_accuracy:
                     result_accuracy = accuracy_score(y_true = original_outputs, y_pred = result_pred, normalize=self.normalize_performance) #accuracy
                   else:
                     if self.exec_performance == self.exec_auc:
                       result_accuracy = self.auc_score(original_outputs, result_pred) #AUC
 
-                  result_pred = (result_pred == original_outputs) #binarization
+                  
                   self.list_clf_loop.append(str_model_name)
-                  df_loop_of_models.loc[len(df_loop_of_models)] = result_pred.astype(int)[:].tolist().insert(0,str_model_name) #boolean to int
+                  result_bin = compResponses(list(original_outputs), list(result_pred))
+                  result_bin.insert(0,str_model_name)
+                  df_loop_of_models.loc[len(df_loop_of_models)] = result_bin
                   df_loop_of_models_performance.loc[len(df_loop_of_models_performance)] = [str_model_name, result_accuracy]
                 else:
                   pass
 
       #inset invertion of Four attributes in loop of models
       if self.number_of_features_variation == 4:
         for _, variation in enumerate(self.exec_variation_method):
@@ -793,17 +808,19 @@
 
                     if self.exec_performance == self.exec_accuracy:
                       result_accuracy = accuracy_score(y_true = original_outputs, y_pred = result_pred, normalize=self.normalize_performance) #accuracy
                     else:
                       if self.exec_performance == self.exec_auc:
                         result_accuracy = self.auc_score(original_outputs, result_pred) #AUC
 
-                    result_pred = (result_pred == original_outputs) #binarization
+                    
                     self.list_clf_loop.append(str_model_name)
-                    df_loop_of_models.loc[len(df_loop_of_models)] = result_pred.astype(int)[:].tolist().insert(0,str_model_name) #boolean to int
+                    result_bin = compResponses(list(original_outputs), list(result_pred))
+                    result_bin.insert(0,str_model_name)
+                    df_loop_of_models.loc[len(df_loop_of_models)] = result_bin
                     df_loop_of_models_performance.loc[len(df_loop_of_models_performance)] = [str_model_name, result_accuracy]
                   else:
                     pass
     else:
       if self.exec_proposal == self.proposal_1_pool:
         
         model_copy = copy.deepcopy(model)
@@ -850,42 +867,44 @@
           result_pred = model_copy.predict(data_test_x_copy)
           if self.exec_performance == self.exec_accuracy:
             result_accuracy = accuracy_score(y_true = original_outputs, y_pred = result_pred, normalize=self.normalize_performance) #accuracy
           else:
             if self.exec_performance == self.exec_auc:
               result_accuracy = self.auc_score(original_outputs, result_pred) #AUC
 
-          result_pred = (result_pred == original_outputs) #binarization
+          
             
           str_model_name = 'Clf feature elimination: '
           for _, i in enumerate(ps_c):
             str_model_name = str_model_name + '"'+str(i)+'" '
           self.list_clf_pool.append(str_model_name)
-          df_loop_of_models.loc[len(df_loop_of_models)] = result_pred.astype(int)[:].tolist().insert(0,str_model_name) #boolean to int
+          result_bin = compResponses(list(original_outputs), list(result_pred))
+          result_bin.insert(0,str_model_name)
+          df_loop_of_models.loc[len(df_loop_of_models)] = result_bin
           df_loop_of_models_performance.loc[len(df_loop_of_models_performance)] = [str_model_name, result_accuracy]
           if self.verbose:
             print('')
             print(str_model_name)
             print(data_test_x_copy)
 
-    df_loop_of_models.set_index('Clf')
+    df_loop_of_models = df_loop_of_models.set_index('Clf')
     if self.verbose:
       print('Resume Loop of model')
       print(df_loop_of_models)
       print()
       print('Resume Loop of model accuracy')
       print(df_loop_of_models_performance)
 
     df = df_loop_of_models
-    df.to_csv(self.path_content+self.path_irt+self.bar+"tabela_base_para_executar_irt.csv")
+    df.to_csv(self.path_content+self.path_irt+self.bar+"tabela_base_para_executar_irt.csv",',')
     #if self.download_files:
     #  files.download(self.path_content+self.path_irt+self.bar+"tabela_base_para_executar_irt.csv") 
 
     df = df_loop_of_models_performance
-    df.to_csv(self.path_content+self.path_irt+self.bar+"tabela_base_para_executar_irt_accuracy.csv",index=False)
+    df.to_csv(self.path_content+self.path_irt+self.bar+"tabela_base_para_executar_irt_accuracy.csv",',',index=False)
     #if self.download_files:
     #  files.download(self.path_content+self.path_irt+self.bar+"tabela_base_para_executar_irt_accuracy.csv")
 
     return  df_loop_of_models, df_loop_of_models_performance
 
   def run_irt(self, datasetName):
 
@@ -1052,15 +1071,15 @@
 
     dataset = openml.datasets.get_dataset(dataset_name)
     X, Y, categorical_indicator, attribute_names = dataset.get_data(
                       dataset_format="dataframe", target=dataset.default_target_attribute)
     
     
     #Preprocess Y and X numerics
-    print(Y)
+    #print(Y)
     
     if (Y.dtype != 'numeric'):
       Y = Y.astype(int)
     
     for i,c in enumerate(X.columns):
       if (X[c].dtype != 'float64'):
         X = X.astype(float)
```

