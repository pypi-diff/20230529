# Comparing `tmp/easymms-0.1.1.tar.gz` & `tmp/easymms-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easymms-0.1.1.tar", last modified: Sun May 28 04:22:42 2023, max compression
+gzip compressed data, was "easymms-0.1.2.tar", last modified: Mon May 29 04:24:23 2023, max compression
```

## Comparing `easymms-0.1.1.tar` & `easymms-0.1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 04:22:42.409532 easymms-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    17529 2023-05-28 04:22:31.000000 easymms-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-05-28 04:22:42.409532 easymms-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-05-28 04:22:31.000000 easymms-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 04:22:42.409532 easymms-0.1.1/easymms/
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-28 04:22:31.000000 easymms-0.1.1/easymms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-28 04:22:31.000000 easymms-0.1.1/easymms/_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-05-28 04:22:31.000000 easymms-0.1.1/easymms/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 04:22:42.409532 easymms-0.1.1/easymms/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 04:22:31.000000 easymms-0.1.1/easymms/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-05-28 04:22:31.000000 easymms-0.1.1/easymms/models/alignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-05-28 04:22:31.000000 easymms-0.1.1/easymms/models/asr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-05-28 04:22:31.000000 easymms-0.1.1/easymms/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 04:22:42.409532 easymms-0.1.1/easymms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-05-28 04:22:42.000000 easymms-0.1.1/easymms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-28 04:22:42.000000 easymms-0.1.1/easymms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 04:22:42.000000 easymms-0.1.1/easymms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 04:22:42.000000 easymms-0.1.1/easymms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-28 04:22:42.000000 easymms-0.1.1/easymms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-28 04:22:42.000000 easymms-0.1.1/easymms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 04:22:42.409532 easymms-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-28 04:22:31.000000 easymms-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 04:22:42.409532 easymms-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 04:22:31.000000 easymms-0.1.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-28 04:22:31.000000 easymms-0.1.1/tests/test_asr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 04:24:23.548463 easymms-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    17529 2023-05-29 04:24:12.000000 easymms-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-05-29 04:24:23.548463 easymms-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-05-29 04:24:12.000000 easymms-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 04:24:23.548463 easymms-0.1.2/easymms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-29 04:24:12.000000 easymms-0.1.2/easymms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-29 04:24:12.000000 easymms-0.1.2/easymms/_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5535 2023-05-29 04:24:12.000000 easymms-0.1.2/easymms/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 04:24:23.548463 easymms-0.1.2/easymms/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 04:24:12.000000 easymms-0.1.2/easymms/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7865 2023-05-29 04:24:12.000000 easymms-0.1.2/easymms/models/alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7907 2023-05-29 04:24:12.000000 easymms-0.1.2/easymms/models/asr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-05-29 04:24:12.000000 easymms-0.1.2/easymms/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 04:24:23.548463 easymms-0.1.2/easymms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-05-29 04:24:23.000000 easymms-0.1.2/easymms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-29 04:24:23.000000 easymms-0.1.2/easymms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 04:24:23.000000 easymms-0.1.2/easymms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 04:24:23.000000 easymms-0.1.2/easymms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-29 04:24:23.000000 easymms-0.1.2/easymms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-29 04:24:23.000000 easymms-0.1.2/easymms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 04:24:23.548463 easymms-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-29 04:24:12.000000 easymms-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 04:24:23.548463 easymms-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 04:24:12.000000 easymms-0.1.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-29 04:24:12.000000 easymms-0.1.2/tests/test_asr.py
```

### Comparing `easymms-0.1.1/LICENSE` & `easymms-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `easymms-0.1.1/PKG-INFO` & `easymms-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easymms
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple Python package to easily use Meta's Massively Multilingual Speech (MMS) project
 Author: Abdeladim Sadiki
 License: MIT
 Project-URL: Documentation, https://abdeladim-s.github.io/easymms/
 Project-URL: Source, https://abdeladim-s.github.io/easymms/
 Project-URL: Tracker, https://abdeladim-s.github.io/easymms/issues
 Requires-Python: >=3.8
@@ -33,15 +33,15 @@
 1. You will need [ffmpeg](https://ffmpeg.org/download.html) for audio processing
 
 2. Also, if you want to use the [`Alignment` model](https://github.com/facebookresearch/fairseq/tree/main/examples/mms/data_prep):
 * you will need `perl` to use [uroman](https://github.com/isi-nlp/uroman).
 Check the [perl website]([perl](https://www.perl.org/get.html)) for installation instructions on different platforms.
 * You will need a nightly version of `torchaudio`:
 ```shell
-pip install --pre torchaudio --index-url https://download.pytorch.org/whl/nightly/cu118
+pip install -U --pre torchaudio --index-url https://download.pytorch.org/whl/nightly/cu118
 ```
 * You might need [sox](https://arielvb.readthedocs.io/en/latest/docs/commandline/sox.html) as well.
 
 3. Install `easymms` from Pypi
 ```bash
 pip install easymms
 ```
```

### Comparing `easymms-0.1.1/README.md` & `easymms-0.1.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 1. You will need [ffmpeg](https://ffmpeg.org/download.html) for audio processing
 
 2. Also, if you want to use the [`Alignment` model](https://github.com/facebookresearch/fairseq/tree/main/examples/mms/data_prep):
 * you will need `perl` to use [uroman](https://github.com/isi-nlp/uroman).
 Check the [perl website]([perl](https://www.perl.org/get.html)) for installation instructions on different platforms.
 * You will need a nightly version of `torchaudio`:
 ```shell
-pip install --pre torchaudio --index-url https://download.pytorch.org/whl/nightly/cu118
+pip install -U --pre torchaudio --index-url https://download.pytorch.org/whl/nightly/cu118
 ```
 * You might need [sox](https://arielvb.readthedocs.io/en/latest/docs/commandline/sox.html) as well.
 
 3. Install `easymms` from Pypi
 ```bash
 pip install easymms
 ```
```

### Comparing `easymms-0.1.1/easymms/__init__.py` & `easymms-0.1.2/easymms/__init__.py`

 * *Files identical despite different names*

### Comparing `easymms-0.1.1/easymms/_logger.py` & `easymms-0.1.2/easymms/_logger.py`

 * *Files identical despite different names*

### Comparing `easymms-0.1.1/easymms/constants.py` & `easymms-0.1.2/easymms/constants.py`

 * *Files identical despite different names*

### Comparing `easymms-0.1.1/easymms/models/alignment.py` & `easymms-0.1.2/easymms/models/alignment.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,26 +7,38 @@
 """
 import logging
 import shutil
 import sys
 from pathlib import Path
 from typing import List
 import torch
-import fairseq
+# fix importing from fairseq.examples
+try:
+    from fairseq.examples.mms.data_prep.align_and_segment import get_alignments
+    from fairseq.examples.mms.data_prep.align_utils import get_uroman_tokens, get_spans
+    from fairseq.examples.mms.data_prep.text_normalization import text_normalize
+except ImportError:
+    try:
+        from examples.mms.data_prep.align_and_segment import get_alignments
+        from examples.mms.data_prep.align_utils import get_uroman_tokens, get_spans
+        from examples.mms.data_prep.text_normalization import text_normalize
+    except ImportError:
+        import fairseq
+        sys.path.append(str(Path(fairseq.__file__).parent))
+        from fairseq.examples.mms.data_prep.align_and_segment import get_alignments
+        from fairseq.examples.mms.data_prep.align_utils import get_uroman_tokens, get_spans
+        from fairseq.examples.mms.data_prep.text_normalization import text_normalize
 
 from easymms import utils
 from easymms._logger import set_log_level
 from easymms.constants import PACKAGE_DATA_DIR, ALIGNMENT_MODEL_URL, ALIGNMENT_DICTIONARY_URL, UROMAN_URL, \
     UROMAN_DIR_NAME
 
-sys.path.append(str(Path(fairseq.__file__).parent))  # fix importing from fairseq.examples
 
-from fairseq.examples.mms.data_prep.align_and_segment import get_alignments
-from fairseq.examples.mms.data_prep.align_utils import get_uroman_tokens, get_spans
-from fairseq.examples.mms.data_prep.text_normalization import text_normalize
+
 from torchaudio.models import wav2vec2_model
 
 logger = logging.getLogger(__name__)
 
 
 class AlignmentModel:
     """
```

### Comparing `easymms-0.1.1/easymms/models/asr.py` & `easymms-0.1.2/easymms/models/asr.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,25 +11,32 @@
 import atexit
 import json
 import sys
 import tempfile
 import logging
 from pathlib import Path
 from typing import Union, List
-import fairseq
+
 import torch
 from omegaconf import OmegaConf
 from pydub import AudioSegment
 from pydub.utils import mediainfo
 
-from easymms import utils
-
-sys.path.append(str(Path(fairseq.__file__).parent))  # fix importing from fairseq.examples
+# fix importing from fairseq.examples
+try:
+    from fairseq.examples.speech_recognition.new.infer import hydra_main
+except ImportError:
+    try:
+        from examples.speech_recognition.new.infer import hydra_main
+    except ImportError:
+        import fairseq
+        sys.path.append(str(Path(fairseq.__file__).parent))
+        from fairseq.examples.speech_recognition.new.infer import hydra_main
 
-from fairseq.examples.speech_recognition.new.infer import hydra_main
+from easymms import utils
 from easymms._logger import set_log_level
 from easymms.models.alignment import AlignmentModel
 from easymms.constants import CFG, HYPO_WORDS_FILE, MMS_LANGS_FILE
 
 logger = logging.getLogger(__name__)
 
 
@@ -147,15 +154,15 @@
             self.cfg['dataset']['gen_subset'] = f'{lang}:dev'
             if device is None or device == 'cuda':
                 if torch.cuda.is_available():
                     device = 'cuda'
                     pass  # default
                 else:
                     device = 'cpu'
-            elif device == 'cpu':
+            if device == 'cpu':
                 self.cfg['common']['cpu'] = True
             elif device == 'tpu':
                 self.cfg['common']['tpu'] = True
             else:
                 logging.warning(f'Unknown device option {device}, Use one of (cuda, cpu, tpu)')
             cfg = OmegaConf.structured(self.cfg)
```

### Comparing `easymms-0.1.1/easymms/utils.py` & `easymms-0.1.2/easymms/utils.py`

 * *Files identical despite different names*

### Comparing `easymms-0.1.1/easymms.egg-info/PKG-INFO` & `easymms-0.1.2/easymms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easymms
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple Python package to easily use Meta's Massively Multilingual Speech (MMS) project
 Author: Abdeladim Sadiki
 License: MIT
 Project-URL: Documentation, https://abdeladim-s.github.io/easymms/
 Project-URL: Source, https://abdeladim-s.github.io/easymms/
 Project-URL: Tracker, https://abdeladim-s.github.io/easymms/issues
 Requires-Python: >=3.8
@@ -33,15 +33,15 @@
 1. You will need [ffmpeg](https://ffmpeg.org/download.html) for audio processing
 
 2. Also, if you want to use the [`Alignment` model](https://github.com/facebookresearch/fairseq/tree/main/examples/mms/data_prep):
 * you will need `perl` to use [uroman](https://github.com/isi-nlp/uroman).
 Check the [perl website]([perl](https://www.perl.org/get.html)) for installation instructions on different platforms.
 * You will need a nightly version of `torchaudio`:
 ```shell
-pip install --pre torchaudio --index-url https://download.pytorch.org/whl/nightly/cu118
+pip install -U --pre torchaudio --index-url https://download.pytorch.org/whl/nightly/cu118
 ```
 * You might need [sox](https://arielvb.readthedocs.io/en/latest/docs/commandline/sox.html) as well.
 
 3. Install `easymms` from Pypi
 ```bash
 pip install easymms
 ```
```

### Comparing `easymms-0.1.1/setup.py` & `easymms-0.1.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # read the contents of your README file
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text(encoding='utf-8')
 
 
 setup(
     name="easymms",
-    version="0.1.1",
+    version="0.1.2",
     author="Abdeladim Sadiki",
     description="A simple Python package to easily use Meta's Massively Multilingual Speech (MMS) project",
     long_description=long_description,
     ext_modules=[],
     zip_safe=False,
     python_requires=">=3.8",
     packages=find_packages('.'),
```

### Comparing `easymms-0.1.1/tests/test_asr.py` & `easymms-0.1.2/tests/test_asr.py`

 * *Files identical despite different names*

