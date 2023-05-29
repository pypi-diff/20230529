# Comparing `tmp/genda_lens-0.0.1.tar.gz` & `tmp/genda_lens-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genda_lens-0.0.1.tar", max compression
+gzip compressed data, was "genda_lens-0.0.2.tar", max compression
```

## Comparing `genda_lens-0.0.1.tar` & `genda_lens-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1065 2023-05-16 07:25:58.546949 genda_lens-0.0.1/LICENSE
--rw-r--r--   0        0        0     4094 2023-05-27 22:01:31.208109 genda_lens-0.0.1/README.md
--rw-r--r--   0        0        0       48 2023-05-16 07:31:44.932265 genda_lens-0.0.1/genda_lens/__init__.py
--rw-r--r--   0        0        0     8236 2023-05-27 21:28:14.357211 genda_lens-0.0.1/genda_lens/coref_tasks/abc_utils.py
--rw-r--r--   0        0        0    12485 2023-05-18 12:02:26.903295 genda_lens-0.0.1/genda_lens/coref_tasks/wino_utils.py
--rw-r--r--   0        0        0    57119 2023-03-21 08:24:08.746101 genda_lens-0.0.1/genda_lens/data/DaWinoBias_anti_stereotyped_evalda.txt
--rw-r--r--   0        0        0    57118 2023-03-09 16:12:47.834912 genda_lens-0.0.1/genda_lens/data/DaWinoBias_pro_stereotyped_evalda.txt
--rw-r--r--   0        0        0   336571 2023-04-26 15:47:17.498741 genda_lens-0.0.1/genda_lens/data/abc_fem_sents.txt
--rw-r--r--   0        0        0   324943 2023-04-26 15:47:29.017834 genda_lens-0.0.1/genda_lens/data/abc_male_sents.txt
--rw-r--r--   0        0        0   706895 2023-05-03 17:07:48.000948 genda_lens-0.0.1/genda_lens/data/name_aug_csv_files/first_names_2023_men.csv
--rw-r--r--   0        0        0   891168 2023-05-03 17:07:48.029137 genda_lens-0.0.1/genda_lens/data/name_aug_csv_files/first_names_2023_women.csv
--rw-r--r--   0        0        0  4094899 2023-05-03 17:07:48.124266 genda_lens-0.0.1/genda_lens/data/name_aug_csv_files/last_names_2023.csv
--rw-r--r--   0        0        0     1114 2023-05-03 17:07:48.132607 genda_lens-0.0.1/genda_lens/data/name_aug_csv_files/overlapping_names.csv
--rw-r--r--   0        0        0    11901 2023-05-03 17:07:48.133913 genda_lens-0.0.1/genda_lens/data/name_aug_csv_files/unisex_names.csv
--rw-r--r--   0        0        0    18426 2023-05-27 21:37:44.237834 genda_lens-0.0.1/genda_lens/genda_lens.py
--rw-r--r--   0        0        0    10287 2023-05-27 21:13:32.580660 genda_lens-0.0.1/genda_lens/lm_tasks/abc_utils.py
--rw-r--r--   0        0        0      256 2023-05-18 12:02:26.951826 genda_lens-0.0.1/genda_lens/lm_tasks/load_model.py
--rw-r--r--   0        0        0     6957 2023-05-18 12:02:26.953592 genda_lens-0.0.1/genda_lens/lm_tasks/wino_utils.py
--rw-r--r--   0        0        0     1550 2023-05-18 12:02:26.954488 genda_lens-0.0.1/genda_lens/ner_tasks/augmentation.py
--rw-r--r--   0        0        0     5755 2023-05-18 12:02:26.955388 genda_lens-0.0.1/genda_lens/ner_tasks/performance.py
--rw-r--r--   0        0        0     2687 2023-05-18 12:02:26.956243 genda_lens-0.0.1/genda_lens/ner_tasks/process_names.py
--rw-r--r--   0        0        0      793 2023-05-27 21:21:16.489577 genda_lens-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     5185 1970-01-01 00:00:00.000000 genda_lens-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-16 07:25:58.546949 genda_lens-0.0.2/LICENSE
+-rw-r--r--   0        0        0     4094 2023-05-27 22:01:31.208109 genda_lens-0.0.2/README.md
+-rw-r--r--   0        0        0       48 2023-05-29 19:40:52.621288 genda_lens-0.0.2/genda_lens/__init__.py
+-rw-r--r--   0        0        0     8236 2023-05-27 21:28:14.357211 genda_lens-0.0.2/genda_lens/coref_tasks/abc_utils.py
+-rw-r--r--   0        0        0    12485 2023-05-18 12:02:26.903295 genda_lens-0.0.2/genda_lens/coref_tasks/wino_utils.py
+-rw-r--r--   0        0        0    57119 2023-03-21 08:24:08.746101 genda_lens-0.0.2/genda_lens/data/DaWinoBias_anti_stereotyped_evalda.txt
+-rw-r--r--   0        0        0    57118 2023-03-09 16:12:47.834912 genda_lens-0.0.2/genda_lens/data/DaWinoBias_pro_stereotyped_evalda.txt
+-rw-r--r--   0        0        0   336571 2023-04-26 15:47:17.498741 genda_lens-0.0.2/genda_lens/data/abc_fem_sents.txt
+-rw-r--r--   0        0        0   324943 2023-04-26 15:47:29.017834 genda_lens-0.0.2/genda_lens/data/abc_male_sents.txt
+-rw-r--r--   0        0        0   706895 2023-05-03 17:07:48.000948 genda_lens-0.0.2/genda_lens/data/name_aug_csv_files/first_names_2023_men.csv
+-rw-r--r--   0        0        0   891168 2023-05-03 17:07:48.029137 genda_lens-0.0.2/genda_lens/data/name_aug_csv_files/first_names_2023_women.csv
+-rw-r--r--   0        0        0  4094899 2023-05-03 17:07:48.124266 genda_lens-0.0.2/genda_lens/data/name_aug_csv_files/last_names_2023.csv
+-rw-r--r--   0        0        0     1114 2023-05-03 17:07:48.132607 genda_lens-0.0.2/genda_lens/data/name_aug_csv_files/overlapping_names.csv
+-rw-r--r--   0        0        0    11901 2023-05-03 17:07:48.133913 genda_lens-0.0.2/genda_lens/data/name_aug_csv_files/unisex_names.csv
+-rw-r--r--   0        0        0    18439 2023-05-29 19:40:07.994862 genda_lens-0.0.2/genda_lens/genda_lens.py
+-rw-r--r--   0        0        0    10287 2023-05-27 21:13:32.580660 genda_lens-0.0.2/genda_lens/lm_tasks/abc_utils.py
+-rw-r--r--   0        0        0      256 2023-05-18 12:02:26.951826 genda_lens-0.0.2/genda_lens/lm_tasks/load_model.py
+-rw-r--r--   0        0        0     6957 2023-05-18 12:02:26.953592 genda_lens-0.0.2/genda_lens/lm_tasks/wino_utils.py
+-rw-r--r--   0        0        0     1550 2023-05-18 12:02:26.954488 genda_lens-0.0.2/genda_lens/ner_tasks/augmentation.py
+-rw-r--r--   0        0        0     5755 2023-05-18 12:02:26.955388 genda_lens-0.0.2/genda_lens/ner_tasks/performance.py
+-rw-r--r--   0        0        0     2687 2023-05-18 12:02:26.956243 genda_lens-0.0.2/genda_lens/ner_tasks/process_names.py
+-rw-r--r--   0        0        0      764 2023-05-29 19:41:00.042448 genda_lens-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5201 1970-01-01 00:00:00.000000 genda_lens-0.0.2/PKG-INFO
```

### Comparing `genda_lens-0.0.1/LICENSE` & `genda_lens-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `genda_lens-0.0.1/README.md` & `genda_lens-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `genda_lens-0.0.1/genda_lens/coref_tasks/abc_utils.py` & `genda_lens-0.0.2/genda_lens/coref_tasks/abc_utils.py`

 * *Files identical despite different names*

### Comparing `genda_lens-0.0.1/genda_lens/coref_tasks/wino_utils.py` & `genda_lens-0.0.2/genda_lens/coref_tasks/wino_utils.py`

 * *Files identical despite different names*

### Comparing `genda_lens-0.0.1/genda_lens/data/DaWinoBias_anti_stereotyped_evalda.txt` & `genda_lens-0.0.2/genda_lens/data/DaWinoBias_anti_stereotyped_evalda.txt`

 * *Files identical despite different names*

### Comparing `genda_lens-0.0.1/genda_lens/data/DaWinoBias_pro_stereotyped_evalda.txt` & `genda_lens-0.0.2/genda_lens/data/DaWinoBias_pro_stereotyped_evalda.txt`

 * *Files identical despite different names*

### Comparing `genda_lens-0.0.1/genda_lens/data/abc_fem_sents.txt` & `genda_lens-0.0.2/genda_lens/data/abc_fem_sents.txt`

 * *Files identical despite different names*

### Comparing `genda_lens-0.0.1/genda_lens/data/abc_male_sents.txt` & `genda_lens-0.0.2/genda_lens/data/abc_male_sents.txt`

 * *Files identical despite different names*

### Comparing `genda_lens-0.0.1/genda_lens/data/name_aug_csv_files/first_names_2023_men.csv` & `genda_lens-0.0.2/genda_lens/data/name_aug_csv_files/first_names_2023_men.csv`

 * *Files identical despite different names*

### Comparing `genda_lens-0.0.1/genda_lens/data/name_aug_csv_files/first_names_2023_women.csv` & `genda_lens-0.0.2/genda_lens/data/name_aug_csv_files/first_names_2023_women.csv`

 * *Files identical despite different names*

### Comparing `genda_lens-0.0.1/genda_lens/data/name_aug_csv_files/last_names_2023.csv` & `genda_lens-0.0.2/genda_lens/data/name_aug_csv_files/last_names_2023.csv`

 * *Files identical despite different names*

### Comparing `genda_lens-0.0.1/genda_lens/data/name_aug_csv_files/overlapping_names.csv` & `genda_lens-0.0.2/genda_lens/data/name_aug_csv_files/overlapping_names.csv`

 * *Files identical despite different names*

### Comparing `genda_lens-0.0.1/genda_lens/data/name_aug_csv_files/unisex_names.csv` & `genda_lens-0.0.2/genda_lens/data/name_aug_csv_files/unisex_names.csv`

 * *Files identical despite different names*

### Comparing `genda_lens-0.0.1/genda_lens/genda_lens.py` & `genda_lens-0.0.2/genda_lens/genda_lens.py`

 * *Files 1% similar despite different names*

```diff
@@ -301,15 +301,15 @@
     def visualize_results(self, data, framework, model_name, task=None):
         """Visualize output from any of the genderbias tests that can be run in this package.
 
         Args:
             data (df): detailed output from any of the tests.
             framework (str): choose between "ner", "dawinobias" or "abc".
             model_name (str): model name
-            task (str, optional): choose between "lm", "ner" or "coref" depending on which task the output is from.
+            task (str, optional): choose between "lm" or "coref" if the output is either from the dawinobias or abc framework.
         Returns:
             plot (plot): seaborn plot visualization.
 
         *EXAMPLE*
 
            ```python
            from genda_lens import Visualizer
@@ -391,15 +391,15 @@
                         float(data.iloc[2, 1].split(" ")[0]),
                         float(data.iloc[4, 3].split(" ")[0]),
                         float(data.iloc[4, 4].split(" ")[0]),
                         float(data.iloc[2, 3].split(" ")[0]),
                     ]
                 except:
                     points = [
-                        float(df.iloc[4, 0].split(" ")[0]),
+                        float(data.iloc[4, 0].split(" ")[0]),
                         float(data.iloc[4, 1].split(" ")[0]),
                         float(data.iloc[2, 0].split(" ")[0]),
                         float(data.iloc[4, 2].split(" ")[0]),
                         float(data.iloc[4, 3].split(" ")[0]),
                         float(data.iloc[2, 2].split(" ")[0]),
                     ]
                 df["Median Perplexity"] = points
```

### Comparing `genda_lens-0.0.1/genda_lens/lm_tasks/abc_utils.py` & `genda_lens-0.0.2/genda_lens/lm_tasks/abc_utils.py`

 * *Files identical despite different names*

### Comparing `genda_lens-0.0.1/genda_lens/lm_tasks/wino_utils.py` & `genda_lens-0.0.2/genda_lens/lm_tasks/wino_utils.py`

 * *Files identical despite different names*

### Comparing `genda_lens-0.0.1/genda_lens/ner_tasks/augmentation.py` & `genda_lens-0.0.2/genda_lens/ner_tasks/augmentation.py`

 * *Files identical despite different names*

### Comparing `genda_lens-0.0.1/genda_lens/ner_tasks/performance.py` & `genda_lens-0.0.2/genda_lens/ner_tasks/performance.py`

 * *Files identical despite different names*

### Comparing `genda_lens-0.0.1/genda_lens/ner_tasks/process_names.py` & `genda_lens-0.0.2/genda_lens/ner_tasks/process_names.py`

 * *Files identical despite different names*

### Comparing `genda_lens-0.0.1/pyproject.toml` & `genda_lens-0.0.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "genda-lens"
-version = "0.0.1"
+version = "0.0.2"
 description = "A package for quantifying bias in Danish language models."
-authors = ["Astrid Rybner <astrid.rybner@hotmail.com>", "Thea Rolskov <thearollesloth@hotmail.com>"]
+authors = ["Rybner, Astrid. Rolskov, Thea <astrid.rybner@hotmail.com>"]
 packages = [{include = "genda_lens"}]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/DaDebias/genda-lens"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `genda_lens-0.0.1/PKG-INFO` & `genda_lens-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: genda-lens
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package for quantifying bias in Danish language models.
 Home-page: https://github.com/DaDebias/genda-lens
 License: MIT
-Author: Astrid Rybner
+Author: Rybner, Astrid. Rolskov, Thea
 Author-email: astrid.rybner@hotmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: genda-lens Version: 0.0.1 Summary: A package for
+Metadata-Version: 2.1 Name: genda-lens Version: 0.0.2 Summary: A package for
 quantifying bias in Danish language models. Home-page: https://github.com/
-DaDebias/genda-lens License: MIT Author: Astrid Rybner Author-email:
-astrid.rybner@hotmail.com Requires-Python: >=3.9,<4.0 Classifier: License ::
-OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: augmenty (>=1.3.7,<1.4) Requires-Dist: dacy (>=2.7.1,<2.8)
-Requires-Dist: fairlearn (>=0.8.0,<0.9.0) Requires-Dist: matplotlib
-(>=3.7,<3.8) Requires-Dist: numpy (>=1.24,<1.25) Requires-Dist: pandas
-(>=1.5,<1.6) Requires-Dist: scikit-learn (>=1.2,<1.3) Requires-Dist: seaborn
-(>=0.12,<0.13) Requires-Dist: spacy (>=3.5,<3.6) Requires-Dist: spacy-wrap
-(>=1.4.2,<1.5) Requires-Dist: tqdm (>=4.65.0,<4.66) Requires-Dist: transformers
-(>=4.28,<4.29) Project-URL: Repository, https://github.com/DaDebias/genda-lens
-Description-Content-Type: text/markdown
+DaDebias/genda-lens License: MIT Author: Rybner, Astrid. Rolskov, Thea Author-
+email: astrid.rybner@hotmail.com Requires-Python: >=3.9,<4.0 Classifier:
+License :: OSI Approved :: MIT License Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
+Programming Language :: Python :: 3.10 Classifier: Programming Language ::
+Python :: 3.11 Requires-Dist: augmenty (>=1.3.7,<1.4) Requires-Dist: dacy
+(>=2.7.1,<2.8) Requires-Dist: fairlearn (>=0.8.0,<0.9.0) Requires-Dist:
+matplotlib (>=3.7,<3.8) Requires-Dist: numpy (>=1.24,<1.25) Requires-Dist:
+pandas (>=1.5,<1.6) Requires-Dist: scikit-learn (>=1.2,<1.3) Requires-Dist:
+seaborn (>=0.12,<0.13) Requires-Dist: spacy (>=3.5,<3.6) Requires-Dist: spacy-
+wrap (>=1.4.2,<1.5) Requires-Dist: tqdm (>=4.65.0,<4.66) Requires-Dist:
+transformers (>=4.28,<4.29) Project-URL: Repository, https://github.com/
+DaDebias/genda-lens Description-Content-Type: text/markdown
                                     [Logo]
                          ****** The GenDa Lens: ******
           **** Quantifying Gender Bias in Danish language models ****
                   Thea Rolskov Sloth & Astrid Sletten Rybner
 
 A python package for investigating gender bias in Danish language models within
 the following domains: * **Language Modeling** (for pre-trained models) *
```

