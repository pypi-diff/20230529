# Comparing `tmp/Hefesto-0.4.1.tar.gz` & `tmp/Hefesto-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Hefesto-0.4.1.tar", last modified: Wed May 17 07:46:09 2023, max compression
+gzip compressed data, was "Hefesto-0.4.2.tar", last modified: Mon May 29 11:02:09 2023, max compression
```

## Comparing `Hefesto-0.4.1.tar` & `Hefesto-0.4.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2023-05-17 07:46:09.189123 Hefesto-0.4.1/
-drwxrwxr-x   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2023-05-17 07:46:09.189123 Hefesto-0.4.1/Hefesto/
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2022-10-25 10:40:14.000000 Hefesto-0.4.1/Hefesto/__init__.py
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)    11950 2023-05-17 07:22:54.000000 Hefesto-0.4.1/Hefesto/main.py
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)     8594 2023-04-21 09:41:24.000000 Hefesto-0.4.1/Hefesto/template.py
-drwxrwxr-x   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2023-05-17 07:46:09.189123 Hefesto-0.4.1/Hefesto.egg-info/
--rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      287 2023-05-17 07:46:09.000000 Hefesto-0.4.1/Hefesto.egg-info/PKG-INFO
--rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      227 2023-05-17 07:46:09.000000 Hefesto-0.4.1/Hefesto.egg-info/SOURCES.txt
--rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)        1 2023-05-17 07:46:09.000000 Hefesto-0.4.1/Hefesto.egg-info/dependency_links.txt
--rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)        8 2023-05-17 07:46:09.000000 Hefesto-0.4.1/Hefesto.egg-info/top_level.txt
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      147 2022-10-25 10:40:14.000000 Hefesto-0.4.1/MANIFEST.in
--rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      287 2023-05-17 07:46:09.189123 Hefesto-0.4.1/PKG-INFO
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      719 2023-02-08 11:49:59.000000 Hefesto-0.4.1/README.md
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)       31 2023-02-10 09:50:43.000000 Hefesto-0.4.1/requirements.txt
--rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)       38 2023-05-17 07:46:09.189123 Hefesto-0.4.1/setup.cfg
--rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      520 2023-05-17 07:44:20.000000 Hefesto-0.4.1/setup.py
+drwxrwxr-x   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2023-05-29 11:02:09.147207 Hefesto-0.4.2/
+drwxrwxr-x   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2023-05-29 11:02:09.143207 Hefesto-0.4.2/Hefesto/
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2022-10-25 10:40:14.000000 Hefesto-0.4.2/Hefesto/__init__.py
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)    10220 2023-05-29 11:01:36.000000 Hefesto-0.4.2/Hefesto/main.py
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)     7518 2023-05-29 09:20:38.000000 Hefesto-0.4.2/Hefesto/template.py
+drwxrwxr-x   0 pabloalarconm  (1000) pabloalarconm  (1000)        0 2023-05-29 11:02:09.147207 Hefesto-0.4.2/Hefesto.egg-info/
+-rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      287 2023-05-29 11:02:09.000000 Hefesto-0.4.2/Hefesto.egg-info/PKG-INFO
+-rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      227 2023-05-29 11:02:09.000000 Hefesto-0.4.2/Hefesto.egg-info/SOURCES.txt
+-rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)        1 2023-05-29 11:02:09.000000 Hefesto-0.4.2/Hefesto.egg-info/dependency_links.txt
+-rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)        8 2023-05-29 11:02:09.000000 Hefesto-0.4.2/Hefesto.egg-info/top_level.txt
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      147 2022-10-25 10:40:14.000000 Hefesto-0.4.2/MANIFEST.in
+-rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      287 2023-05-29 11:02:09.147207 Hefesto-0.4.2/PKG-INFO
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      719 2023-02-08 11:49:59.000000 Hefesto-0.4.2/README.md
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)       31 2023-02-10 09:50:43.000000 Hefesto-0.4.2/requirements.txt
+-rw-rw-r--   0 pabloalarconm  (1000) pabloalarconm  (1000)       38 2023-05-29 11:02:09.147207 Hefesto-0.4.2/setup.cfg
+-rw-r--r--   0 pabloalarconm  (1000) pabloalarconm  (1000)      520 2023-05-29 11:01:40.000000 Hefesto-0.4.2/setup.py
```

### Comparing `Hefesto-0.4.1/Hefesto/main.py` & `Hefesto-0.4.2/Hefesto/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,35 +2,44 @@
 from perseo.main import milisec
 # from template import Template
 from Hefesto.template import Template
 import sys
 import yaml
 import math
 import requests
+import logging
 
 class Hefesto():
 
     def __init__(self, datainput, reset = False):
-        # Create an object as dictonary to reduce duplicate calls:
-        self.reg = dict()
-
         # Import data input:
         if not reset:
-            self.df_data = pd.read_csv(datainput)
-            self.df_data = self.df_data.where(pd.notnull(self.df_data), None)
-
+            try:
+                self.df_data = pd.read_csv(datainput)
+            except FileNotFoundError:
+                raise FileNotFoundError(f"File '{datainput}' does not exist.")
+            finally:
+                self.df_data = self.df_data.where(pd.notnull(self.df_data), None)
         else:
             self.df_data = datainput
             return self.df_data
+        
+        # Create an object as dictonary to reduce duplicate calls:
+        self.reg = dict()
+
 
-    def transform_Fiab(self):
+    def transformFiab(self):
 
     # Import static template for all CDE terms:
         temp = Template.template_model
 
+    # Check the status of the dataframe used:
+        if not "model" and "pid" and "value" in self.df_data.columns:
+            sys.exit(" The quality of the data used in not correct, please check CSV used to perform the transformation.")
+
     # Empty objects:
         resulting_df = pd.DataFrame()
         row_df = {}
 
 
         for row in self.df_data.iterrows():
             milisec_point = milisec()
@@ -55,61 +64,29 @@
             resulting_df = pd.concat([resulting_df, final_row_df])
 
         # Reset Index:    
         resulting_df = resulting_df.reset_index(drop=True)
         # Turn any nan to None:
         resulting_df = resulting_df.where(pd.notnull(resulting_df), None)
 
-        # Delete columns without values:
-        # for row_final in resulting_df.iterrows():
-        #     if row_final[1]["value"] == None and row_final[1]["valueIRI"] == None:
-        #         resulting_df = resulting_df.drop(row_final[0])
-
-        # Datatype:
-        datatype_relationship = {
-            "xsd:string":"value_string",
-            "xsd:date" : "value_date",
-            "xsd:float": "value_float",
-            "xsd:integer":"value_integer"
-        }
-
         # Value edition:
-        for index, row in resulting_df.iterrows():
-            for k,v in datatype_relationship.items():
-
-                # value ---> value_DATATYPE:
-                if row["value_datatype"] == k:
-                    resulting_df.at[index, v] = resulting_df["value"][index]
-
-                # # valueIRI ---> process_type for Disability
-                # if row["model"] == "Disability" and row["valueIRI"] != None:
-                #     resulting_df.at[index, "process_type"] = resulting_df["valueIRI"][index]
-                #     resulting_df["valueIRI"][index] = None
-
-                # enddate correction:
-                if row["startdate"] != None and row["enddate"] == None:
-                    resulting_df["enddate"][index] = resulting_df["startdate"][index]
-
-        del resulting_df["value"]
-
-
-        # # valueIRI ---> valueAttributeIRI:
-        # del resulting_df["valueAttributeIRI"]
-        # resulting_df.rename(columns={'valueIRI':'valueAttributeIRI'}, inplace=True)
+        resulting_df = self.valueEdition(resulting_df)
+        # Clean blanks:
+        resulting_df = self.cleanBlanks(resulting_df)
 
         # uniqid generation:
         resulting_df['uniqid'] = ""
         for i in resulting_df.index:
             resulting_df.at[i, "uniqid"] = milisec()
 
         print("Structural transformation: Done")
         new = Hefesto.__init__(self, datainput= resulting_df, reset = True)
         return new
 
-    def transform_shape(self,configuration, uniqid_generation= True, contextid_generation= True, clean_blanks= False):
+    def transformShape(self,configuration, uniqid_generation= True, contextid_generation= True, clean_blanks= False):
 
         if type(configuration) is not dict:
             sys.exit("configuration file must be a dictionary from a Python, YAML or JSON file")
 
         
         # Import static template for all CDE terms:
         temp = Template.template_model
@@ -145,82 +122,63 @@
                 final_row_df = pd.DataFrame(row_df[milisec_point], index=[1])
                 resulting_df = pd.concat([resulting_df, final_row_df])
 
         # Reset Index:    
         resulting_df = resulting_df.reset_index(drop=True)
         # Turn any nan to None:
         resulting_df = resulting_df.where(pd.notnull(resulting_df), None)
+        # Value edition:
+        resulting_df = self.valueEdition(resulting_df)
+        # Clean blanks:
+        resulting_df = self.cleanBlanks(resulting_df)
+        
+        # uniqid generation:
+        resulting_df['uniqid'] = ""
+        for i in resulting_df.index:
+            resulting_df.at[i, "uniqid"] = milisec()
+
+        
+        print("Structural transformation: Done")
+        new = Hefesto.__init__(self, datainput= resulting_df, reset = True)
+        return new
+
+    def cleanBlanks(self, resulting_df):
+
+        for row_final in resulting_df.iterrows():
+            if row_final[1]["value"] == None and row_final[1]["attribute_id"] == None and row_final[1]["comments"] == None and row_final[1]["agent_id"] == None:
+                resulting_df = resulting_df.drop(row_final[0])
+        del resulting_df["value"]
+
+        return resulting_df
+
+    def valueEdition(self, resulting_df):
 
         # Datatype:
         datatype_relationship = {
             "xsd:string":"value_string",
             "xsd:date" : "value_date",
             "xsd:float": "value_float",
             "xsd:integer":"value_integer"
         }
-
+        
         # Value edition:
         for index, row in resulting_df.iterrows():
             for k,v in datatype_relationship.items():
                 
-
                 # value ---> value_DATATYPE:
                 if row["value_datatype"] == k:
                     resulting_df.at[index, v] = resulting_df["value"][index]
                     resulting_df = resulting_df.where(pd.notnull(resulting_df), None)
 
                 # enddate correction:
                 if row["startdate"] != None and row["enddate"] == None:
-                    resulting_df["enddate"][index] = resulting_df["startdate"][index]
+                    resulting_df.at[index,"enddate"] = resulting_df["startdate"][index]
                     resulting_df = resulting_df.where(pd.notnull(resulting_df), None)
 
-
-        # clean blanks
-        for row_final in resulting_df.iterrows():
-            if row_final[1]["value"] == None and row_final[1]["attribute_id"] == None and row_final[1]["comments"] == None and row_final[1]["agent_id"] == None:
-                resulting_df = resulting_df.drop(row_final[0])
-        del resulting_df["value"]
-
-
-        # # valueIRI ---> valueAttributeIRI:
-        # del resulting_df["valueAttributeIRI"]
-        # resulting_df.rename(columns={'valueIRI':'valueAttributeIRI'}, inplace=True)
-
-        # uniqid generation:
-        resulting_df['uniqid'] = ""
-        for i in resulting_df.index:
-            resulting_df.at[i, "uniqid"] = milisec()
-
-
-        # # Empty value row removal
-        # for row_final in resulting_df.iterrows():
-        #     if row_final[1]["valueOutput_date"] == None and row_final[1]["valueOutput_string"] == None and row_final[1]["valueOutput_float"] == None:
-        #         resulting_df = resulting_df.drop(row_final[0])
-
-        #     # Reset Dataframe index again
-        #     resulting_df = resulting_df.reset_index(drop=True)
-                    
-        # # uniqid (re)generation:
-        # resulting_df = resulting_df.reset_index(drop=True)
-
-        # if uniqid_generation:
-        #     resulting_df['uniqid'] = ""
-        #     for i in resulting_df.index:
-        #         resulting_df.at[i, "uniqid"] = milisec()
-
-        # # context_id (re)generation:
-        # if contextid_generation:
-        #     resulting_df['context_id'] = ""
-        #     for i in resulting_df.index:
-        #         resulting_df.at[i, "context_id"] = milisec()
-
-        
-        print("Structural transformation: Done")
-        new = Hefesto.__init__(self, datainput= resulting_df, reset = True)
-        return new
+        return resulting_df
 
     def get_uri(self, col, ont):
 
         
         if not col in list(self.df_data.columns):
             sys.exit("ERROR: selected column doesnt exist")
 
@@ -247,16 +205,14 @@
                 self.reg[term] = data_iri
                 self.df_data.at[i,col+"_uri"] = data_iri 
 
         print("URLs from Label calling: Done")
         new = Hefesto.__init__(self, datainput= self.df_data, reset = True)
         return new
 
-
-
     def get_label(self, col):
 
         # Column duplication to work in new column:
         self.df_data[col+"_label"] = self.df_data.loc[:, col]
 
         # Loop throught new column to replace current value with API term:
         for i in self.df_data[col+"_label"].index:
@@ -277,15 +233,14 @@
                 self.reg[term] = data_label
                 self.df_data.at[i,col+"_label"] = data_label 
 
         print("Labels from URL calling: Done")
         new = Hefesto.__init__(self, datainput= self.df_data, reset = True)
         return new
 
-    
     def replacement(self, col, key, value, duplicate = False):
 
         if duplicate == "True":
             # Column duplication to work in new column:
             self.df_data[col+"_dup"] = self.df_data.loc[:, col]
             self.df_data[col+"_dup"] = self.df_data[col+"_dup"].replace([key],value)
         else:
@@ -298,15 +253,15 @@
 
 # # Test 1:
 
 # test = Hefesto(datainput = "../data/INPUT_DATA.csv")
 # transform = test.transform_Fiab()
 # transform.to_csv ("../data/OUTPUT_DATA.csv", index = False, header=True)
 
-# # Test 2
+# # # Test 2
 # with open("../data/CDEconfig.yaml") as file:
 #     configuration = yaml.load(file, Loader=yaml.FullLoader)
 
 # test = Hefesto(datainput = "../data/INPUT_DATA2.csv")
 # transform = test.transform_shape(configuration=configuration, clean_blanks = True) #, clean_blanks=False
 # # label = test.get_label("output_type")
 # # url_from_label= test.get_uri("output_type_label","ncit")
```

### Comparing `Hefesto-0.4.1/Hefesto/template.py` & `Hefesto-0.4.2/Hefesto/template.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 
 class Template:
 
   template_model = dict(
 
-    Age = dict(
+    Birthyear = dict(
       process_type = "http://purl.obolibrary.org/obo/NCIT_C142470",
       output_type = "http://purl.obolibrary.org/obo/NCIT_C70856",
-      attribute_type = "http://purl.obolibrary.org/obo/NCIT_C25150",
-      value_datatype = "xsd:date",
+      attribute_id = "http://purl.obolibrary.org/obo/NCIT_C83164",
+      value_datatype = "xsd:integer",
       startdate = None,
       enddate = None,
       pid = None,
       context_id = None
     ),
 
     Birthdate = dict(
       process_type = "http://purl.obolibrary.org/obo/NCIT_C142470",
       output_type = "http://purl.obolibrary.org/obo/NCIT_C70856",
-      attribute_type = "http://purl.obolibrary.org/obo/NCIT_C68615",
+      attribute_id = "http://purl.obolibrary.org/obo/NCIT_C68615",
       value_datatype = "xsd:date",
       startdate = None,
       enddate = None,
       pid = None,
       context_id = None
     ),
 
     Deathdate = dict( 
       process_type= "http://purl.obolibrary.org/obo/NCIT_C142470",
       output_type= "http://purl.obolibrary.org/obo/NCIT_C70856",
-      attribute_type = "http://purl.obolibrary.org/obo/NCIT_C70810",
+      attribute_id = "http://purl.obolibrary.org/obo/NCIT_C70810",
       value_datatype = "xsd:date",
       startdate = None,
       enddate = None,
       pid = None,
       context_id = None
     ),
 
     First_visit = dict(
       process_type = "http://purl.obolibrary.org/obo/NCIT_C142470",
       output_type = "http://purl.obolibrary.org/obo/NCIT_C70856",
-      attribute_type = "http://purl.obolibrary.org/obo/NCIT_C164021",
+      attribute_id = "http://purl.obolibrary.org/obo/NCIT_C164021",
       value_datatype = "xsd:date",
       startdate = None,
       enddate = None,
       pid = None,
       context_id = None
     ),
 
@@ -88,125 +88,86 @@
     #   value_datatype = "xsd:date",
     #   startdate = None,
     #   enddate = None,
     #   pid = None,
     #   context_id = None
     # ),
 
-    Onset_symptoms = dict(
+    Symptoms_onset_date = dict(
       process_type= "http://purl.obolibrary.org/obo/NCIT_C142470",
       output_type = "http://purl.obolibrary.org/obo/NCIT_C70856",
       attribute_type= "http://purl.obolibrary.org/obo/NCIT_C124353",
+      attribute_id= "http://purl.obolibrary.org/obo/NCIT_C119242",
       value_datatype = "xsd:date",
       startdate = None,
       enddate = None,
       pid = None,
       context_id = None
     ),
 
-    # Phenotype = dict(
-    #   process_type= "http://purl.obolibrary.org/obo/NCIT_C25305",
-    #   output_type= "http://purl.obolibrary.org/obo/NCIT_C125204",
-    #   attribute_type= "http://semanticscience.org/resource/SIO_010056",
-    #   attribute_id = None,
-    #   value_string= None,
-    #   value_datatype = None,
-    #   startdate = None,
-    #   enddate = None,
-    #   pid = None,
-    #   context_id = None
-    # ),
+    Symptoms_onset_age = dict(
+      process_type= "http://purl.obolibrary.org/obo/NCIT_C142470",
+      output_type = "http://purl.obolibrary.org/obo/NCIT_C70856",
+      attribute_type= "http://purl.obolibrary.org/obo/NCIT_C124353",
+      attribute_id= "http://purl.obolibrary.org/obo/NCIT_C174273",
+      value_datatype = "xsd:float",
+      startdate = None,
+      enddate = None,
+      pid = None,
+      context_id = None
+    ),
 
     Genetic = dict(
       process_type= "http://purl.obolibrary.org/obo/NCIT_C15709",
       output_type= "http://purl.obolibrary.org/obo/NCIT_C70856",
       attribute_type= "http://purl.obolibrary.org/obo/NCIT_C103223",
       value_datatype = "xsd:string",
       startdate = None,
       enddate = None,
       pid = None,
       context_id = None
     ),
 
-    # Genotype_OMIM = dict(
-    #   process_type= "http://purl.obolibrary.org/obo/NCIT_C15709",
-    #   output_type= "http://purl.obolibrary.org/obo/NCIT_C16612",
-    #   attribute_type= "http://edamontology.org/data_1153",
-    #   attribute_id = None,
-    #   value_string= None,
-    #   value_datatype = None,
-    #   startdate = None,
-    #   enddate = None,
-    #   pid = None,
-    #   context_id = None
-    # ),
-
-    # Genotype_HGNC = dict(
-    #   process_type= "http://purl.obolibrary.org/obo/NCIT_C15709",
-    #   output_type= "http://purl.obolibrary.org/obo/NCIT_C16612",
-    #   attribute_type= "http://edamontology.org/data_2298",
-    #   attribute_id = None,
-    #   value_string= None,
-    #   value_datatype = None,
-    #   startdate = None,
-    #   enddate = None,
-    #   pid = None,
-    #   context_id = None
-    # ),
-
-    # Consent = dict(
-    #   process_type= "http://purl.obolibrary.org/obo/OBI_0000810",
-    #   output_type = None,
-    #   attribute_type= "http://purl.obolibrary.org/obo/NCIT_C25460",
-    #   attribute_id = None,
-    #   value_string= None,
-    #   value_datatype = None,
-    #   startdate = None,
-    #   enddate = None,
-    #   pid = None,
-    #   context_id = None
-    # ),
-
     Consent_contacted = dict(
       process_type= "http://purl.obolibrary.org/obo/OBI_0000810",
       output_type = "http://purl.obolibrary.org/obo/OBIB_0000488",
-      attribute_type= "http://purl.obolibrary.org/obo/NCIT_C25460",
+      attribute_id= "http://purl.obolibrary.org/obo/NCIT_C25460",
       value_datatype = "xsd:string",
       startdate = None,
       enddate = None,
       pid = None,
       context_id = None
     ),
 
     Consent_used = dict(
       process_type= "http://purl.obolibrary.org/obo/OBI_0000810",
       output_type = "http://purl.obolibrary.org/obo/DUO_0000001",
-      attribute_type= "http://purl.obolibrary.org/obo/NCIT_C25460",
+      attribute_id= "http://purl.obolibrary.org/obo/NCIT_C25460",
       value_datatype = "xsd:string",
       startdate = None,
       enddate = None,
       pid = None,
       context_id = None
     ),
 
     Biobank = dict(
       process_type= "http://purl.obolibrary.org/obo/OMIABIS_0000061",
       output_type= "http://purl.obolibrary.org/obo/NCIT_C115570",
-      attribute_type= "http://purl.obolibrary.org/obo/NCIT_C25429",
+      attribute_id= "http://purl.obolibrary.org/obo/NCIT_C25429",
       value_datatype = "xsd:string",
       startdate = None,
       enddate = None,
       pid = None,
       context_id = None
     ),
 
     Disability = dict(
       process_type = None,
       output_type = "http://purl.obolibrary.org/obo/NCIT_C70856",
-      attribute_type = "http://purl.obolibrary.org/obo/NCIT_C21007",
+      attribute_id = "http://purl.obolibrary.org/obo/NCIT_C21007",
       value_datatype = "xsd:float",
       startdate = None,
       enddate = None,
       pid = None,
       context_id = None
     ),
 
@@ -233,24 +194,25 @@
       context_id= None 
     ),
 
 
     Imaging = dict(
       process_type = None ,
       output_type =  "http://purl.obolibrary.org/obo/NCIT_C70856" ,
+      attribute_id = "http://purl.obolibrary.org/obo/NCIT_C176708",
       value_datatype = "xsd:string" ,
       startdate= None ,
       enddate= None ,
       comments= None ,
       pid = None ,
       context_id= None 
     ),
 
 
-    Surgery = dict(
+    Intervention = dict(
       value_datatype = "xsd:string" ,
       startdate= None ,
       enddate= None ,
       comments= None ,
       pid= None ,
       context_id= None 
     ),
```

### Comparing `Hefesto-0.4.1/README.md` & `Hefesto-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `Hefesto-0.4.1/setup.py` & `Hefesto-0.4.2/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #     readme = readme_file.read()
 
 # with open('requirements.txt') as f:
 #     requirements = f.read().splitlines()
 
 setup(
     name="Hefesto",
-    version="0.4.1",
+    version="0.4.2",
     packages=["Hefesto"],
     author="Pablo Alarcón Moreno",
     author_email="pabloalarconmoreno@gmail.com",
     url="https://github.com/pabloalarconm/hefesto",
     description="Preprocessing datatable toolkit",
     license="MIT",
     keywords=["EJP","CDE"]
```

