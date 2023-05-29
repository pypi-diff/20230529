# Comparing `tmp/dreamai_pdf-0.1.0.tar.gz` & `tmp/dreamai_pdf-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dreamai_pdf-0.1.0.tar", last modified: Sun May 21 06:51:20 2023, max compression
+gzip compressed data, was "dreamai_pdf-0.1.2.tar", last modified: Mon May 29 15:16:01 2023, max compression
```

## Comparing `dreamai_pdf-0.1.0.tar` & `dreamai_pdf-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-21 06:51:20.677612 dreamai_pdf-0.1.0/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)    11337 2023-04-27 10:12:58.000000 dreamai_pdf-0.1.0/LICENSE
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      111 2023-04-27 10:12:58.000000 dreamai_pdf-0.1.0/MANIFEST.in
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     1005 2023-05-21 06:51:20.677612 dreamai_pdf-0.1.0/PKG-INFO
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      215 2023-05-21 06:46:56.000000 dreamai_pdf-0.1.0/README.md
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-21 06:51:20.677612 dreamai_pdf-0.1.0/dreamai_pdf/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       22 2023-05-21 06:50:52.000000 dreamai_pdf-0.1.0/dreamai_pdf/__init__.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     1359 2023-05-21 06:50:52.000000 dreamai_pdf-0.1.0/dreamai_pdf/_modidx.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     2200 2023-05-21 06:50:52.000000 dreamai_pdf-0.1.0/dreamai_pdf/core.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      173 2023-05-21 06:44:43.000000 dreamai_pdf-0.1.0/dreamai_pdf/imports.py
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     2667 2023-05-21 06:50:52.000000 dreamai_pdf-0.1.0/dreamai_pdf/segment.py
-drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-21 06:51:20.677612 dreamai_pdf-0.1.0/dreamai_pdf.egg-info/
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     1005 2023-05-21 06:51:20.000000 dreamai_pdf-0.1.0/dreamai_pdf.egg-info/PKG-INFO
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      410 2023-05-21 06:51:20.000000 dreamai_pdf-0.1.0/dreamai_pdf.egg-info/SOURCES.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-05-21 06:51:20.000000 dreamai_pdf-0.1.0/dreamai_pdf.egg-info/dependency_links.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       44 2023-05-21 06:51:20.000000 dreamai_pdf-0.1.0/dreamai_pdf.egg-info/entry_points.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-05-21 06:51:00.000000 dreamai_pdf-0.1.0/dreamai_pdf.egg-info/not-zip-safe
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       72 2023-05-21 06:51:20.000000 dreamai_pdf-0.1.0/dreamai_pdf.egg-info/requires.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       12 2023-05-21 06:51:20.000000 dreamai_pdf-0.1.0/dreamai_pdf.egg-info/top_level.txt
--rw-rw-r--   0 hamza     (1000) hamza     (1000)      758 2023-05-21 06:50:13.000000 dreamai_pdf-0.1.0/settings.ini
--rw-rw-r--   0 hamza     (1000) hamza     (1000)       38 2023-05-21 06:51:20.677612 dreamai_pdf-0.1.0/setup.cfg
--rw-rw-r--   0 hamza     (1000) hamza     (1000)     2596 2023-04-27 10:12:58.000000 dreamai_pdf-0.1.0/setup.py
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-29 15:16:01.484638 dreamai_pdf-0.1.2/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)    11337 2023-04-27 10:12:58.000000 dreamai_pdf-0.1.2/LICENSE
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      111 2023-04-27 10:12:58.000000 dreamai_pdf-0.1.2/MANIFEST.in
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     1005 2023-05-29 15:16:01.484638 dreamai_pdf-0.1.2/PKG-INFO
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      215 2023-05-21 06:46:56.000000 dreamai_pdf-0.1.2/README.md
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-29 15:16:01.484638 dreamai_pdf-0.1.2/dreamai_pdf/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       22 2023-05-29 15:15:52.000000 dreamai_pdf-0.1.2/dreamai_pdf/__init__.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     2760 2023-05-29 15:15:52.000000 dreamai_pdf-0.1.2/dreamai_pdf/_modidx.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     6006 2023-05-29 15:15:52.000000 dreamai_pdf-0.1.2/dreamai_pdf/core.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     4590 2023-05-29 15:15:52.000000 dreamai_pdf-0.1.2/dreamai_pdf/extract.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      328 2023-05-27 03:27:42.000000 dreamai_pdf-0.1.2/dreamai_pdf/imports.py
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     3680 2023-05-29 15:15:52.000000 dreamai_pdf-0.1.2/dreamai_pdf/ner.py
+drwxrwxr-x   0 hamza     (1000) hamza     (1000)        0 2023-05-29 15:16:01.484638 dreamai_pdf-0.1.2/dreamai_pdf.egg-info/
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     1005 2023-05-29 15:16:01.000000 dreamai_pdf-0.1.2/dreamai_pdf.egg-info/PKG-INFO
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      429 2023-05-29 15:16:01.000000 dreamai_pdf-0.1.2/dreamai_pdf.egg-info/SOURCES.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-05-29 15:16:01.000000 dreamai_pdf-0.1.2/dreamai_pdf.egg-info/dependency_links.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       44 2023-05-29 15:16:01.000000 dreamai_pdf-0.1.2/dreamai_pdf.egg-info/entry_points.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)        1 2023-05-21 06:51:00.000000 dreamai_pdf-0.1.2/dreamai_pdf.egg-info/not-zip-safe
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       72 2023-05-29 15:16:01.000000 dreamai_pdf-0.1.2/dreamai_pdf.egg-info/requires.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       12 2023-05-29 15:16:01.000000 dreamai_pdf-0.1.2/dreamai_pdf.egg-info/top_level.txt
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)      758 2023-05-29 15:15:44.000000 dreamai_pdf-0.1.2/settings.ini
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)       38 2023-05-29 15:16:01.484638 dreamai_pdf-0.1.2/setup.cfg
+-rw-rw-r--   0 hamza     (1000) hamza     (1000)     2596 2023-04-27 10:12:58.000000 dreamai_pdf-0.1.2/setup.py
```

### Comparing `dreamai_pdf-0.1.0/LICENSE` & `dreamai_pdf-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dreamai_pdf-0.1.0/PKG-INFO` & `dreamai_pdf-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dreamai_pdf
-Version: 0.1.0
+Version: 0.1.2
 Summary: Library based on DreamAI for parsing PDFs
 Home-page: https://github.com/HamzaFarhan/dreamai_pdf
 Author: Hamza Farhan
 Author-email: thehamza96@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dreamai_pdf-0.1.0/dreamai_pdf/segment.py` & `dreamai_pdf-0.1.2/dreamai_pdf/extract.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,67 +1,127 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/01_segment.ipynb.
+# AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/01_extract.ipynb.
 
 # %% auto 0
-__all__ = ['text_to_segments', 'print_segments', 'load_segs_model', 'load_ems_model', 'write_segments']
+__all__ = ['print_segments', 'text_to_segments', 'load_segs_model', 'load_ems_model', 'write_segments', 'write_embeddings']
 
-# %% ../nbs/01_segment.ipynb 2
+# %% ../nbs/01_extract.ipynb 2
 from .imports import *
 from .core import *
 
-# %% ../nbs/01_segment.ipynb 3
-def text_to_segments(text: Union[str, List[str]], segs_model: SetFitModel,
-                     thresh: float=0.6, classes: List=['Work Experience', 'Education', 'Certifications', 'Other']):
+
+# %% ../nbs/01_extract.ipynb 3
+def print_segments(segments: dict, limit: int = 10, width: int = 100):
+    for k, v in segments.items():
+        print(f"{k}: {len(v)}")
+        for s in v[:limit]:
+            print("\t", end="")
+            pprint(s, width=width)
+            print()
+        print("-" * width + 4)
+
+
+def text_to_segments(
+    text: Union[str, List[str]],
+    segs_model: SetFitModel,
+    thresh: float = 0.6,
+    classes: List = ["Work Experience", "Education", "Certifications", "Other"],
+):
     preds = segs_model.predict(text).detach().cpu().numpy()
     probs = segs_model.predict_proba(text).detach().cpu().numpy().max(1)
     preds[probs < thresh] = 3
     pred_classes = [classes[p] for p in preds]
-    segments = {pc:[] for pc in classes}
-    for i,pc in enumerate(pred_classes):
-        txt = text[i]
+    segments = {pc: [] for pc in classes}
+    for pc, txt in zip(pred_classes, text):
         if txt not in segments[pc]:
-            segments[pc].append(text[i])
+            segments[pc].append(txt)
     return segments, pred_classes, probs
 
-def print_segments(segments: dict, limit: int=10):
-    for k,v in segments.items():
-        print(f'{k}: {len(v)}')
-        for s in v[:limit]:
-            print('\t', end='')
-            pprint(s, width=100)
-            print()
-        print('-'*100)
-        
-def load_segs_model(model_name: str='HamzaFarhan/PDFSegs', device: Union[str, torch.device]='cpu'):
+
+def load_segs_model(
+    model_name: str = "HamzaFarhan/PDFSegs", device: Union[str, torch.device] = "cpu"
+):
     return SetFitModel.from_pretrained(model_name).to(device)
 
-def load_ems_model(model_name: str='HamzaFarhan/PDFSegs', device: Union[str, torch.device]='cpu'):
+
+def load_ems_model(
+    model_name: str = "HamzaFarhan/PDFSegs", device: Union[str, torch.device] = "cpu"
+):
     return SentenceTransformer(model_name, device=device)
 
-def write_segments(segs_model: SetFitModel, data_path: Union[str, Path, List[Union[str, Path]]], output_path: Union[str, Path]='pdf_segments'):
+
+def write_segments(segs_model, data_path, output_path="pdf_segments", n_lines=2):
     """
     Extracts text from PDFs and writes segments to JSON files.
-    
+
     Parameters
     ----------
     segs_model : SetFitModel
         SetFit model for segment classification.
     data_path : Union[str, Path, List[Union[str, Path]]]
         Path to PDFs. Can be a single file, a directory, or a list of files/directories.
     output_path : Union[str, Path]
         Folder to write JSON files. Defaults to 'pdf_segments'.
-    
+    n_lines : int
+        Number of lines to group together when extracting text from PDFs.
     Returns
     -------
     None
     """
     output_path = Path(output_path)
     os.makedirs(output_path, exist_ok=True)
     pdfs = resolve_data_path(data_path)
+    text_dict = extract_text_dict(pdfs, n_lines=n_lines)
     for file in pdfs:
         try:
-            pdf_text = extract_text(file)[str(file)]
-            segments, _, _ = text_to_segments(pdf_text, segs_model, thresh=0.6)
-            fn = (output_path/Path(file).stem).with_suffix('.json')
-            with open(fn, 'w') as f:
+            pdf_text = text_dict[str(file)]
+            (segments,) = text_to_segments(pdf_text, segs_model, thresh=0.6)[0]
+            fn = (output_path / Path(file).stem).with_suffix(".json")
+            with open(fn, "w") as f:
                 json.dump(segments, f, indent=4)
         except Exception as e:
-            print(f'\nCould not write segments for file: {str(file)}\n{e}')
+            msg.fail(f"\nCould not write segments for file: {str(file)}", e)
+            # print(f"\nCould not write segments for file: {str(file)}\n{e}")
+
+
+def write_embeddings(
+    segs_model, ems_model, data_path, output_path="pdf_ems", n_lines=3
+):
+    """
+    Extracts text from PDFs and writes embeddings to JSON files.
+
+    Parameters
+    ----------
+    segs_model : SetFitModel
+        SetFit model for segment classification.
+    ems_model : SentenceTransformer
+        SentenceTransformer model for embedding generation.
+    data_path : Union[str, Path, List[Union[str, Path]]]
+        Path to PDFs. Can be a single file, a directory, or a list of files/directories.
+    output_path : Union[str, Path]
+        Folder to write JSON files. Defaults to 'pdf_ems'.
+    n_lines : int
+        Number of lines to group together when extracting text from PDFs.
+    Returns
+    -------
+    None
+    """
+    os.makedirs(output_path, exist_ok=True)
+    seg_ids = {"Work Experience": 1, "Education": 2, "Certifications": 3, "Other": 4}
+    pdfs = resolve_data_path(data_path)
+    text_dict = extract_text_dict(pdfs, n_lines=n_lines)
+    for file in pdfs:
+        try:
+            fn = Path(file).stem
+            pdf_text = text_dict[str(file)]
+            ems = ems_model.encode(pdf_text)
+            pred_classes = text_to_segments(pdf_text, segs_model)[1]
+            for i, data in enumerate(zip(pred_classes, ems)):
+                pc, em = data
+                seg_id = seg_ids[pc]
+                jf = Path(output_path) / f"{fn}_{seg_id}_{i+1}.json"
+                em_dict = {"id": fn, "embedding": em.tolist()}
+                with open(jf, "w") as f:
+                    json.dump(em_dict, f)
+        except Exception as e:
+            msg.fail(f"\nCould not write embeddings for {str(file)}", e)
+            # print(f"\nCould not write embeddings for {str(file)}\n{e}")
+
```

### Comparing `dreamai_pdf-0.1.0/dreamai_pdf.egg-info/PKG-INFO` & `dreamai_pdf-0.1.2/dreamai_pdf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dreamai-pdf
-Version: 0.1.0
+Version: 0.1.2
 Summary: Library based on DreamAI for parsing PDFs
 Home-page: https://github.com/HamzaFarhan/dreamai_pdf
 Author: Hamza Farhan
 Author-email: thehamza96@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dreamai_pdf-0.1.0/settings.ini` & `dreamai_pdf-0.1.2/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = dreamai_pdf
 lib_name = %(repo)s
-version = 0.1.0
+version = 0.1.2
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = dreamai_pdf
 nbs_path = nbs
 recursive = True
```

### Comparing `dreamai_pdf-0.1.0/setup.py` & `dreamai_pdf-0.1.2/setup.py`

 * *Files identical despite different names*

