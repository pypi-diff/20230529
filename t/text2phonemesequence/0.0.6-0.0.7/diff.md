# Comparing `tmp/text2phonemesequence-0.0.6.tar.gz` & `tmp/text2phonemesequence-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/text2phonemesequence-0.0.6.tar", last modified: Sun May 21 16:58:08 2023, max compression
+gzip compressed data, was "dist/text2phonemesequence-0.0.7.tar", last modified: Mon May 29 10:28:43 2023, max compression
```

## Comparing `text2phonemesequence-0.0.6.tar` & `text2phonemesequence-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 vinai     (1000) vinai     (1000)        0 2023-05-21 16:58:08.000000 text2phonemesequence-0.0.6/
--rw-rw-r--   0 vinai     (1000) vinai     (1000)     2640 2023-05-21 16:58:08.000000 text2phonemesequence-0.0.6/PKG-INFO
--rw-rw-r--   0 vinai     (1000) vinai     (1000)     1777 2023-05-20 04:58:56.000000 text2phonemesequence-0.0.6/README.md
--rw-rw-r--   0 vinai     (1000) vinai     (1000)       38 2023-05-21 16:58:08.000000 text2phonemesequence-0.0.6/setup.cfg
--rw-rw-r--   0 vinai     (1000) vinai     (1000)     1291 2023-05-19 08:19:14.000000 text2phonemesequence-0.0.6/setup.py
-drwxrwxr-x   0 vinai     (1000) vinai     (1000)        0 2023-05-21 16:58:08.000000 text2phonemesequence-0.0.6/text2phonemesequence/
--rw-rw-r--   0 vinai     (1000) vinai     (1000)      162 2023-05-21 16:57:44.000000 text2phonemesequence-0.0.6/text2phonemesequence/__init__.py
--rw-rw-r--   0 vinai     (1000) vinai     (1000)     7251 2023-05-21 16:52:00.000000 text2phonemesequence-0.0.6/text2phonemesequence/text2phonemesequence.py
-drwxrwxr-x   0 vinai     (1000) vinai     (1000)        0 2023-05-21 16:58:08.000000 text2phonemesequence-0.0.6/text2phonemesequence.egg-info/
--rw-rw-r--   0 vinai     (1000) vinai     (1000)     2640 2023-05-21 16:58:08.000000 text2phonemesequence-0.0.6/text2phonemesequence.egg-info/PKG-INFO
--rw-rw-r--   0 vinai     (1000) vinai     (1000)      315 2023-05-21 16:58:08.000000 text2phonemesequence-0.0.6/text2phonemesequence.egg-info/SOURCES.txt
--rw-rw-r--   0 vinai     (1000) vinai     (1000)        1 2023-05-21 16:58:08.000000 text2phonemesequence-0.0.6/text2phonemesequence.egg-info/dependency_links.txt
--rw-rw-r--   0 vinai     (1000) vinai     (1000)       27 2023-05-21 16:58:08.000000 text2phonemesequence-0.0.6/text2phonemesequence.egg-info/requires.txt
--rw-rw-r--   0 vinai     (1000) vinai     (1000)       21 2023-05-21 16:58:08.000000 text2phonemesequence-0.0.6/text2phonemesequence.egg-info/top_level.txt
+drwxrwxr-x   0 vinai     (1000) vinai     (1000)        0 2023-05-29 10:28:43.000000 text2phonemesequence-0.0.7/
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)     1291 2023-05-19 08:19:14.000000 text2phonemesequence-0.0.7/setup.py
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)     1777 2023-05-20 04:58:56.000000 text2phonemesequence-0.0.7/README.md
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)     2405 2023-05-29 10:28:43.000000 text2phonemesequence-0.0.7/PKG-INFO
+drwxrwxr-x   0 vinai     (1000) vinai     (1000)        0 2023-05-29 10:28:43.000000 text2phonemesequence-0.0.7/text2phonemesequence.egg-info/
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)     2405 2023-05-29 10:28:43.000000 text2phonemesequence-0.0.7/text2phonemesequence.egg-info/PKG-INFO
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)       21 2023-05-29 10:28:43.000000 text2phonemesequence-0.0.7/text2phonemesequence.egg-info/top_level.txt
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)        1 2023-05-29 10:28:43.000000 text2phonemesequence-0.0.7/text2phonemesequence.egg-info/dependency_links.txt
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)      315 2023-05-29 10:28:43.000000 text2phonemesequence-0.0.7/text2phonemesequence.egg-info/SOURCES.txt
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)       27 2023-05-29 10:28:43.000000 text2phonemesequence-0.0.7/text2phonemesequence.egg-info/requires.txt
+drwxrwxr-x   0 vinai     (1000) vinai     (1000)        0 2023-05-29 10:28:43.000000 text2phonemesequence-0.0.7/text2phonemesequence/
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)     7256 2023-05-29 10:27:51.000000 text2phonemesequence-0.0.7/text2phonemesequence/text2phonemesequence.py
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)      162 2023-05-29 10:27:40.000000 text2phonemesequence-0.0.7/text2phonemesequence/__init__.py
+-rw-rw-r--   0 vinai     (1000) vinai     (1000)       38 2023-05-29 10:28:43.000000 text2phonemesequence-0.0.7/setup.cfg
```

### Comparing `text2phonemesequence-0.0.6/PKG-INFO` & `text2phonemesequence-0.0.7/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,48 @@
 Metadata-Version: 2.1
 Name: text2phonemesequence
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Python Library to convert text to phoneme sequence used for XPhoneBERT
 Home-page: https://github.com/thelinhbkhn2014/Text2PhonemeSequence
 Author: Linh The Nguyen
 Author-email: toank45sphn@gmail.com
 Maintainer: linhthenguyen
 Maintainer-email: toank45sphn@gmail.com
 License: UNKNOWN
-Description: # Text2PhonemeSequence: A Python Library to convert text to phoneme sequences used for [XPhoneBERT](https://github.com/VinAIResearch/XPhoneBERT) 
-        
-        - [Installation](#install)
-        - [Usage example](#example)
-        
-        ## Installation <a name="install"></a>
-        
-        - To install **Text2PhonemeSequence**, users have to run the following command:
-        
-            `$ pip install text2phonemesequence` 
-        
-        ## Usage example <a name="example"></a>
-        The library uses CharsiuG2P to convert text to phoneme sequences. Users can find the information on `pretrained_g2p_model` and `language` in the [CharsiuG2P](https://github.com/lingjzhu/CharsiuG2P/tree/main) repository. For languages where words are not separated by spaces such as Vietnamese and Chinese, users need to use an external tokenizer before feeding the dataset or sentences into our **Text2PhonemeSequence** library. 
-        
-        ```python
-        from text2phonemesequence import Text2PhonemeSequence
-        
-        # Load Text2PhonemeSequence
-        model = Text2PhonemeSequence(pretrained_g2p_model='charsiu/g2p_multilingual_byT5_tiny_16_layers_100', language='eng-us', is_cuda=False)
-        
-        
-        # Convert a raw corpus
-        model.infer_dataset(input_file="/absolute/path/to/input/file", output_file="/absolute/path/to/output/file")
-        
-        # Convert a raw sentence
-        model.infer_sentence("The overwhelming majority of people in this country know how to sift the wheat from the chaff in what they hear and what they read .")
-        ##Output: "ˈθ i ▁ ˈo ʊ v ɝ ˌw ɛ ɫ m ɪ ŋ ▁ m ə ˈd ʒ ɔ ɹ ə t i ▁ ˈɑ f ▁ ˈp i p ə ɫ ▁ ˈɪ n ▁ ˈθ ɪ s ▁ ˈk a ʊ n t ɹ i ▁ ˈn o ʊ ▁ ˈh o ʊ ▁ ˈt o ʊ ▁ ˈs ɪ f t ▁ ˈθ i ▁ ˈw i t ▁ ˈf ɹ ɑ m ▁ ˈθ i ▁ ˈt ʃ æ f ▁ ˈɪ n ▁ ˈw æ t ▁ ˈθ e ɪ ▁ ˈh ɪ ɹ ▁ ˈæ n d ▁ ˈw æ t ▁ ˈθ e ɪ ▁ ˈɹ ɛ d ▁ ."
-        ```
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+
+# Text2PhonemeSequence: A Python Library to convert text to phoneme sequences used for [XPhoneBERT](https://github.com/VinAIResearch/XPhoneBERT) 
+
+- [Installation](#install)
+- [Usage example](#example)
+
+## Installation <a name="install"></a>
+
+- To install **Text2PhonemeSequence**, users have to run the following command:
+
+    `$ pip install text2phonemesequence` 
+
+## Usage example <a name="example"></a>
+The library uses CharsiuG2P to convert text to phoneme sequences. Users can find the information on `pretrained_g2p_model` and `language` in the [CharsiuG2P](https://github.com/lingjzhu/CharsiuG2P/tree/main) repository. For languages where words are not separated by spaces such as Vietnamese and Chinese, users need to use an external tokenizer before feeding the dataset or sentences into our **Text2PhonemeSequence** library. 
+
+```python
+from text2phonemesequence import Text2PhonemeSequence
+
+# Load Text2PhonemeSequence
+model = Text2PhonemeSequence(pretrained_g2p_model='charsiu/g2p_multilingual_byT5_tiny_16_layers_100', language='eng-us', is_cuda=False)
+
+
+# Convert a raw corpus
+model.infer_dataset(input_file="/absolute/path/to/input/file", output_file="/absolute/path/to/output/file")
+
+# Convert a raw sentence
+model.infer_sentence("The overwhelming majority of people in this country know how to sift the wheat from the chaff in what they hear and what they read .")
+##Output: "ˈθ i ▁ ˈo ʊ v ɝ ˌw ɛ ɫ m ɪ ŋ ▁ m ə ˈd ʒ ɔ ɹ ə t i ▁ ˈɑ f ▁ ˈp i p ə ɫ ▁ ˈɪ n ▁ ˈθ ɪ s ▁ ˈk a ʊ n t ɹ i ▁ ˈn o ʊ ▁ ˈh o ʊ ▁ ˈt o ʊ ▁ ˈs ɪ f t ▁ ˈθ i ▁ ˈw i t ▁ ˈf ɹ ɑ m ▁ ˈθ i ▁ ˈt ʃ æ f ▁ ˈɪ n ▁ ˈw æ t ▁ ˈθ e ɪ ▁ ˈh ɪ ɹ ▁ ˈæ n d ▁ ˈw æ t ▁ ˈθ e ɪ ▁ ˈɹ ɛ d ▁ ."
+```
+
+
```

### Comparing `text2phonemesequence-0.0.6/README.md` & `text2phonemesequence-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `text2phonemesequence-0.0.6/setup.py` & `text2phonemesequence-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `text2phonemesequence-0.0.6/text2phonemesequence/text2phonemesequence.py` & `text2phonemesequence-0.0.7/text2phonemesequence/text2phonemesequence.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 class Text2PhonemeSequence:
     def __init__(self, pretrained_g2p_model='charsiu/g2p_multilingual_byT5_tiny_16_layers_100', language='vie-c', is_cuda=True):
         self.tokenizer = AutoTokenizer.from_pretrained('google/byt5-small')
         self.model = T5ForConditionalGeneration.from_pretrained(pretrained_g2p_model)
         self.is_cuda = is_cuda
         if self.is_cuda:
-            self.model = model.cuda()
+            self.model = self.model.cuda()
         self.punctuation = list('.?!,:;-()[]{}<>"') + list("'/‘”“/&#~@^|") + ['...', '*']
         self.segment_tool = Tokenizer()
         self.language = language
         self.phoneme_length = {'msa.tsv': 27, 'amh.tsv': 28, 'urd.tsv': 152, 'mri.tsv': 30, 'glg.tsv': 22, 'swa.tsv': 28, 'est.tsv': 47, 'hbs-latn.tsv': 31, 'spa.tsv': 28, 'pol.tsv': 38, 'spa-latin.tsv': 24, 'fra.tsv': 43, 'uig.tsv': 33, 'aze.tsv': 34, 'nob.tsv': 52, 'swe.tsv': 36, 'por-bz.tsv': 28, 'arg.tsv': 30, 'yue.tsv': 227, 'sqi.tsv': 42, 'cat.tsv': 27, 'hbs-cyrl.tsv': 31, 'grc.tsv': 39, 'bak.tsv': 44, 'hun.tsv': 67, 'lat-clas.tsv': 61, 'ita.tsv': 37, 'san.tsv': 38, 'arm-w.tsv': 41, 'afr.tsv': 81, 'ind.tsv': 87, 'sme.tsv': 31, 'egy.tsv': 22, 'rus.tsv': 62, 'ady.tsv': 29, 'epo.tsv': 43, 'srp.tsv': 42, 'zho-t.tsv': 135, 'tha.tsv': 295, 'vie-c.tsv': 184, 'kur.tsv': 37, 'ice.tsv': 37, 'geo.tsv': 75, 'cze.tsv': 43, 'ara.tsv': 370, 'tgl.tsv': 27, 'nan.tsv': 175, 'por-po.tsv': 35, 'bos.tsv': 52, 'enm.tsv': 24, 'ltz.tsv': 55, 'ina.tsv': 26, 'ukr.tsv': 39, 'mac.tsv': 44, 'kaz.tsv': 44, 'slk.tsv': 73, 'ang.tsv': 33, 'khm.tsv': 47, 'syc.tsv': 24, 'eus.tsv': 35, 'spa-me.tsv': 28, 'tts.tsv': 26, 'gle.tsv': 36, 'slv.tsv': 35, 'ido.tsv': 23, 'zho-s.tsv': 135, 'vie-n.tsv': 174, 'gre.tsv': 20, 'eng-us.tsv': 119, 'fin.tsv': 44, 'pap.tsv': 26, 'tuk.tsv': 49, 'jpn.tsv': 174, 'bel.tsv': 58, 'uzb.tsv': 36, 'dan.tsv': 42, 'ori.tsv': 45, 'ron.tsv': 30, 'bul.tsv': 40, 'bur.tsv': 52, 'lit.tsv': 87, 'dut.tsv': 48, 'fra-qu.tsv': 255, 'eng-uk.tsv': 129, 'hin.tsv': 110, 'isl.tsv': 41, 'arm-e.tsv': 38, 'kor.tsv': 175, 'tur.tsv': 54, 'fas.tsv': 70, 'ger.tsv': 56, 'tam.tsv': 38, 'wel-sw.tsv': 44, 'vie-s.tsv': 172, 'mlt.tsv': 47, 'wel-nw.tsv': 49, 'slo.tsv': 27, 'lat-eccl.tsv': 43, 'snd.tsv': 60, 'tat.tsv': 103, 'alb.tsv': 40, 'hau.tsv': 45, 'pus.tsv': 34, 'tib.tsv': 61, 'sga.tsv': 47, 'heb.tsv': 39, 'hrx.tsv': 27, 'fao.tsv': 42, 'dsb.tsv': 29}
         self.phone_dict = {}
         if not os.path.exists('./' + language + ".tsv"):
             os.system("wget https://raw.githubusercontent.com/lingjzhu/CharsiuG2P/main/dicts/" + language + ".tsv")
```

### Comparing `text2phonemesequence-0.0.6/text2phonemesequence.egg-info/PKG-INFO` & `text2phonemesequence-0.0.7/text2phonemesequence.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,48 @@
 Metadata-Version: 2.1
 Name: text2phonemesequence
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Python Library to convert text to phoneme sequence used for XPhoneBERT
 Home-page: https://github.com/thelinhbkhn2014/Text2PhonemeSequence
 Author: Linh The Nguyen
 Author-email: toank45sphn@gmail.com
 Maintainer: linhthenguyen
 Maintainer-email: toank45sphn@gmail.com
 License: UNKNOWN
-Description: # Text2PhonemeSequence: A Python Library to convert text to phoneme sequences used for [XPhoneBERT](https://github.com/VinAIResearch/XPhoneBERT) 
-        
-        - [Installation](#install)
-        - [Usage example](#example)
-        
-        ## Installation <a name="install"></a>
-        
-        - To install **Text2PhonemeSequence**, users have to run the following command:
-        
-            `$ pip install text2phonemesequence` 
-        
-        ## Usage example <a name="example"></a>
-        The library uses CharsiuG2P to convert text to phoneme sequences. Users can find the information on `pretrained_g2p_model` and `language` in the [CharsiuG2P](https://github.com/lingjzhu/CharsiuG2P/tree/main) repository. For languages where words are not separated by spaces such as Vietnamese and Chinese, users need to use an external tokenizer before feeding the dataset or sentences into our **Text2PhonemeSequence** library. 
-        
-        ```python
-        from text2phonemesequence import Text2PhonemeSequence
-        
-        # Load Text2PhonemeSequence
-        model = Text2PhonemeSequence(pretrained_g2p_model='charsiu/g2p_multilingual_byT5_tiny_16_layers_100', language='eng-us', is_cuda=False)
-        
-        
-        # Convert a raw corpus
-        model.infer_dataset(input_file="/absolute/path/to/input/file", output_file="/absolute/path/to/output/file")
-        
-        # Convert a raw sentence
-        model.infer_sentence("The overwhelming majority of people in this country know how to sift the wheat from the chaff in what they hear and what they read .")
-        ##Output: "ˈθ i ▁ ˈo ʊ v ɝ ˌw ɛ ɫ m ɪ ŋ ▁ m ə ˈd ʒ ɔ ɹ ə t i ▁ ˈɑ f ▁ ˈp i p ə ɫ ▁ ˈɪ n ▁ ˈθ ɪ s ▁ ˈk a ʊ n t ɹ i ▁ ˈn o ʊ ▁ ˈh o ʊ ▁ ˈt o ʊ ▁ ˈs ɪ f t ▁ ˈθ i ▁ ˈw i t ▁ ˈf ɹ ɑ m ▁ ˈθ i ▁ ˈt ʃ æ f ▁ ˈɪ n ▁ ˈw æ t ▁ ˈθ e ɪ ▁ ˈh ɪ ɹ ▁ ˈæ n d ▁ ˈw æ t ▁ ˈθ e ɪ ▁ ˈɹ ɛ d ▁ ."
-        ```
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+
+# Text2PhonemeSequence: A Python Library to convert text to phoneme sequences used for [XPhoneBERT](https://github.com/VinAIResearch/XPhoneBERT) 
+
+- [Installation](#install)
+- [Usage example](#example)
+
+## Installation <a name="install"></a>
+
+- To install **Text2PhonemeSequence**, users have to run the following command:
+
+    `$ pip install text2phonemesequence` 
+
+## Usage example <a name="example"></a>
+The library uses CharsiuG2P to convert text to phoneme sequences. Users can find the information on `pretrained_g2p_model` and `language` in the [CharsiuG2P](https://github.com/lingjzhu/CharsiuG2P/tree/main) repository. For languages where words are not separated by spaces such as Vietnamese and Chinese, users need to use an external tokenizer before feeding the dataset or sentences into our **Text2PhonemeSequence** library. 
+
+```python
+from text2phonemesequence import Text2PhonemeSequence
+
+# Load Text2PhonemeSequence
+model = Text2PhonemeSequence(pretrained_g2p_model='charsiu/g2p_multilingual_byT5_tiny_16_layers_100', language='eng-us', is_cuda=False)
+
+
+# Convert a raw corpus
+model.infer_dataset(input_file="/absolute/path/to/input/file", output_file="/absolute/path/to/output/file")
+
+# Convert a raw sentence
+model.infer_sentence("The overwhelming majority of people in this country know how to sift the wheat from the chaff in what they hear and what they read .")
+##Output: "ˈθ i ▁ ˈo ʊ v ɝ ˌw ɛ ɫ m ɪ ŋ ▁ m ə ˈd ʒ ɔ ɹ ə t i ▁ ˈɑ f ▁ ˈp i p ə ɫ ▁ ˈɪ n ▁ ˈθ ɪ s ▁ ˈk a ʊ n t ɹ i ▁ ˈn o ʊ ▁ ˈh o ʊ ▁ ˈt o ʊ ▁ ˈs ɪ f t ▁ ˈθ i ▁ ˈw i t ▁ ˈf ɹ ɑ m ▁ ˈθ i ▁ ˈt ʃ æ f ▁ ˈɪ n ▁ ˈw æ t ▁ ˈθ e ɪ ▁ ˈh ɪ ɹ ▁ ˈæ n d ▁ ˈw æ t ▁ ˈθ e ɪ ▁ ˈɹ ɛ d ▁ ."
+```
+
+
```

