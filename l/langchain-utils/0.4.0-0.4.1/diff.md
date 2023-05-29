# Comparing `tmp/langchain_utils-0.4.0.tar.gz` & `tmp/langchain_utils-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_utils-0.4.0.tar", max compression
+gzip compressed data, was "langchain_utils-0.4.1.tar", max compression
```

## Comparing `langchain_utils-0.4.0.tar` & `langchain_utils-0.4.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    12824 2023-05-03 03:03:42.597279 langchain_utils-0.4.0/README.md
--rw-r--r--   0        0        0       22 2023-05-29 09:24:45.089914 langchain_utils-0.4.0/langchain_utils/__init__.py
--rw-r--r--   0        0        0     2163 2023-05-29 09:12:58.926326 langchain_utils-0.4.0/langchain_utils/config.py
--rw-r--r--   0        0        0     4476 2023-05-29 09:15:45.189121 langchain_utils-0.4.0/langchain_utils/document_loaders.py
--rwxr-xr-x   0        0        0     3130 2023-04-17 03:23:31.837819 langchain_utils-0.4.0/langchain_utils/get_html_prompt.py
--rwxr-xr-x   0        0        0     4844 2023-05-29 09:18:35.763289 langchain_utils-0.4.0/langchain_utils/get_pdf_prompt.py
--rwxr-xr-x   0        0        0     3721 2023-04-17 03:23:31.791685 langchain_utils-0.4.0/langchain_utils/get_text_prompt.py
--rwxr-xr-x   0        0        0     4101 2023-05-03 03:00:37.545180 langchain_utils-0.4.0/langchain_utils/get_url_prompt.py
--rwxr-xr-x   0        0        0     3476 2023-04-17 03:23:31.837872 langchain_utils-0.4.0/langchain_utils/get_word_prompt.py
--rwxr-xr-x   0        0        0     2874 2023-05-23 10:30:00.649134 langchain_utils-0.4.0/langchain_utils/get_youtube_transcript_prompt.py
--rw-r--r--   0        0        0     3505 2023-05-29 09:16:10.506138 langchain_utils-0.4.0/langchain_utils/loaders.py
--rw-r--r--   0        0        0      509 2023-04-16 15:20:17.709721 langchain_utils-0.4.0/langchain_utils/prompts.py
--rw-r--r--   0        0        0    10484 2023-05-03 02:59:26.472452 langchain_utils-0.4.0/langchain_utils/utils.py
--rw-r--r--   0        0        0     2154 2023-04-16 15:19:45.633897 langchain_utils-0.4.0/langchain_utils/utils_argparse.py
--rw-r--r--   0        0        0     3314 2023-05-29 08:59:46.652209 langchain_utils-0.4.0/langchain_utils/utils_doc_loaders.py
--rw-r--r--   0        0        0     1891 2023-05-29 09:24:45.087373 langchain_utils-0.4.0/pyproject.toml
--rw-r--r--   0        0        0    13900 1970-01-01 00:00:00.000000 langchain_utils-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    13101 2023-05-29 13:16:54.761092 langchain_utils-0.4.1/README.md
+-rw-r--r--   0        0        0       22 2023-05-29 13:17:03.820392 langchain_utils-0.4.1/langchain_utils/__init__.py
+-rw-r--r--   0        0        0     2163 2023-05-29 09:12:58.926326 langchain_utils-0.4.1/langchain_utils/config.py
+-rw-r--r--   0        0        0     4476 2023-05-29 09:15:45.189121 langchain_utils-0.4.1/langchain_utils/document_loaders.py
+-rwxr-xr-x   0        0        0     3130 2023-04-17 03:23:31.837819 langchain_utils-0.4.1/langchain_utils/get_html_prompt.py
+-rwxr-xr-x   0        0        0     4844 2023-05-29 09:18:35.763289 langchain_utils-0.4.1/langchain_utils/get_pdf_prompt.py
+-rwxr-xr-x   0        0        0     3721 2023-04-17 03:23:31.791685 langchain_utils-0.4.1/langchain_utils/get_text_prompt.py
+-rwxr-xr-x   0        0        0     4101 2023-05-03 03:00:37.545180 langchain_utils-0.4.1/langchain_utils/get_url_prompt.py
+-rwxr-xr-x   0        0        0     3476 2023-04-17 03:23:31.837872 langchain_utils-0.4.1/langchain_utils/get_word_prompt.py
+-rwxr-xr-x   0        0        0     2874 2023-05-23 10:30:00.649134 langchain_utils-0.4.1/langchain_utils/get_youtube_transcript_prompt.py
+-rw-r--r--   0        0        0     3505 2023-05-29 09:16:10.506138 langchain_utils-0.4.1/langchain_utils/loaders.py
+-rw-r--r--   0        0        0      509 2023-04-16 15:20:17.709721 langchain_utils-0.4.1/langchain_utils/prompts.py
+-rw-r--r--   0        0        0    10484 2023-05-03 02:59:26.472452 langchain_utils-0.4.1/langchain_utils/utils.py
+-rw-r--r--   0        0        0     2154 2023-04-16 15:19:45.633897 langchain_utils-0.4.1/langchain_utils/utils_argparse.py
+-rw-r--r--   0        0        0     3314 2023-05-29 08:59:46.652209 langchain_utils-0.4.1/langchain_utils/utils_doc_loaders.py
+-rw-r--r--   0        0        0     1933 2023-05-29 13:17:03.819858 langchain_utils-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0    14219 1970-01-01 00:00:00.000000 langchain_utils-0.4.1/PKG-INFO
```

### Comparing `langchain_utils-0.4.0/README.md` & `langchain_utils-0.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -109,14 +109,15 @@
 
 ```
 $ pdfprompt --help
 
 usage: pdfprompt [-h] [-V] [-c] [-e] [-m model] [-S] [-s chunk_size]
                  [-P PARTS [PARTS ...]] [-r] [--print-percentage-non-ascii]
                  [-n] [-p PAGES [PAGES ...]] [-l PAGE_SLICE] [-M] [-w WHAT]
+                 [-o] [-L OCR_LANGUAGE]
                  PDF Path
 
 Get a prompt consisting the text content of a PDF file
 
 positional arguments:
   PDF Path              Path to the PDF file
 
@@ -149,14 +150,18 @@
                         Use Python slice syntax to select page numbers (e.g.
                         1:3, 1:10:2, etc.) (default: None)
   -M, --merge           Merge contents of all pages before processing
                         (default: False)
   -w WHAT, --what WHAT  Initial knowledge you want to insert before the PDF
                         content in the prompt (default: the content of a PDF
                         file)
+  -o, --fallback-ocr    Use OCR as fallback if no text detected on page
+                        (default: False)
+  -L OCR_LANGUAGE, --ocr-language OCR_LANGUAGE
+                        Language to use for Tesseract OCR (default: chi_sim)
 
 ```
 ### `ytprompt`
 
 ```
 $ ytprompt --help
```

### Comparing `langchain_utils-0.4.0/langchain_utils/config.py` & `langchain_utils-0.4.1/langchain_utils/config.py`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.4.0/langchain_utils/document_loaders.py` & `langchain_utils-0.4.1/langchain_utils/document_loaders.py`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.4.0/langchain_utils/get_html_prompt.py` & `langchain_utils-0.4.1/langchain_utils/get_html_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.4.0/langchain_utils/get_pdf_prompt.py` & `langchain_utils-0.4.1/langchain_utils/get_pdf_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.4.0/langchain_utils/get_text_prompt.py` & `langchain_utils-0.4.1/langchain_utils/get_text_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.4.0/langchain_utils/get_url_prompt.py` & `langchain_utils-0.4.1/langchain_utils/get_url_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.4.0/langchain_utils/get_word_prompt.py` & `langchain_utils-0.4.1/langchain_utils/get_word_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.4.0/langchain_utils/get_youtube_transcript_prompt.py` & `langchain_utils-0.4.1/langchain_utils/get_youtube_transcript_prompt.py`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.4.0/langchain_utils/loaders.py` & `langchain_utils-0.4.1/langchain_utils/loaders.py`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.4.0/langchain_utils/utils.py` & `langchain_utils-0.4.1/langchain_utils/utils.py`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.4.0/langchain_utils/utils_argparse.py` & `langchain_utils-0.4.1/langchain_utils/utils_argparse.py`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.4.0/langchain_utils/utils_doc_loaders.py` & `langchain_utils-0.4.1/langchain_utils/utils_doc_loaders.py`

 * *Files identical despite different names*

### Comparing `langchain_utils-0.4.0/pyproject.toml` & `langchain_utils-0.4.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "langchain-utils"
-version = "0.4.0"
-description = ""
+version = "0.4.1"
+description = "Utilities built upon the langchain library"
 authors = ["Teddy Xinyuan Chen <45612704+tddschn@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{ include = "langchain_utils" }]
 license = "MIT"
 homepage = "https://github.com/tddschn/langchain-utils"
 repository = "https://github.com/tddschn/langchain-utils"
 classifiers = ["Topic :: Utilities"]
```

### Comparing `langchain_utils-0.4.0/PKG-INFO` & `langchain_utils-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: langchain-utils
-Version: 0.4.0
-Summary: 
+Version: 0.4.1
+Summary: Utilities built upon the langchain library
 Home-page: https://github.com/tddschn/langchain-utils
 License: MIT
 Keywords: langchain,utils,LLM,prompts,CLI
 Author: Teddy Xinyuan Chen
 Author-email: 45612704+tddschn@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -137,14 +137,15 @@
 
 ```
 $ pdfprompt --help
 
 usage: pdfprompt [-h] [-V] [-c] [-e] [-m model] [-S] [-s chunk_size]
                  [-P PARTS [PARTS ...]] [-r] [--print-percentage-non-ascii]
                  [-n] [-p PAGES [PAGES ...]] [-l PAGE_SLICE] [-M] [-w WHAT]
+                 [-o] [-L OCR_LANGUAGE]
                  PDF Path
 
 Get a prompt consisting the text content of a PDF file
 
 positional arguments:
   PDF Path              Path to the PDF file
 
@@ -177,14 +178,18 @@
                         Use Python slice syntax to select page numbers (e.g.
                         1:3, 1:10:2, etc.) (default: None)
   -M, --merge           Merge contents of all pages before processing
                         (default: False)
   -w WHAT, --what WHAT  Initial knowledge you want to insert before the PDF
                         content in the prompt (default: the content of a PDF
                         file)
+  -o, --fallback-ocr    Use OCR as fallback if no text detected on page
+                        (default: False)
+  -L OCR_LANGUAGE, --ocr-language OCR_LANGUAGE
+                        Language to use for Tesseract OCR (default: chi_sim)
 
 ```
 ### `ytprompt`
 
 ```
 $ ytprompt --help
```

