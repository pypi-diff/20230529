# Comparing `tmp/so_vits_svc_fork-3.9.5.tar.gz` & `tmp/so_vits_svc_fork-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "so_vits_svc_fork-3.9.5.tar", max compression
+gzip compressed data, was "so_vits_svc_fork-4.0.0.tar", max compression
```

## Comparing `so_vits_svc_fork-3.9.5.tar` & `so_vits_svc_fork-4.0.0.tar`

### file list

```diff
@@ -1,51 +1,52 @@
--rw-r--r--   0        0        0    12463 2023-04-18 10:19:48.034368 so_vits_svc_fork-3.9.5/LICENSE
--rw-r--r--   0        0        0    18160 2023-04-18 10:19:48.034368 so_vits_svc_fork-3.9.5/README.md
--rw-r--r--   0        0        0     3092 2023-04-18 10:19:49.082357 so_vits_svc_fork-3.9.5/pyproject.toml
--rw-r--r--   0        0        0       70 2023-04-18 10:19:49.034358 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/__init__.py
--rw-r--r--   0        0        0    22747 2023-04-18 10:19:48.034368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/__main__.py
--rw-r--r--   0        0        0     1393 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/cluster/__init__.py
--rw-r--r--   0        0        0     2844 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/cluster/train_cluster.py
--rw-r--r--   0        0        0     2868 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/dataset.py
--rw-r--r--   0        0        0     2454 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/default_gui_presets.json
--rw-r--r--   0        0        0     7267 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/f0.py
--rw-r--r--   0        0        0    25933 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/gui.py
--rw-r--r--   0        0        0      864 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/hparams.py
--rw-r--r--   0        0        0        0 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/inference/__init__.py
--rw-r--r--   0        0        0    24054 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/inference/core.py
--rw-r--r--   0        0        0     7485 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/inference/main.py
--rw-r--r--   0        0        0     1213 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/logger.py
--rw-r--r--   0        0        0        0 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/__init__.py
--rw-r--r--   0        0        0    16683 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/attentions.py
--rw-r--r--   0        0        0     4620 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/commons.py
--rw-r--r--   0        0        0        0 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/decoders/__init__.py
--rw-r--r--   0        0        0     1419 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/decoders/f0.py
--rw-r--r--   0        0        0       76 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/decoders/hifigan/__init__.py
--rw-r--r--   0        0        0    11618 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py
--rw-r--r--   0        0        0      340 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/decoders/hifigan/_utils.py
--rw-r--r--   0        0        0      318 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/decoders/mb_istft/__init__.py
--rw-r--r--   0        0        0    12477 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py
--rw-r--r--   0        0        0      419 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/decoders/mb_istft/_loss.py
--rw-r--r--   0        0        0     4725 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py
--rw-r--r--   0        0        0     8954 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py
--rw-r--r--   0        0        0     4879 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py
--rw-r--r--   0        0        0     5604 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/descriminators.py
--rw-r--r--   0        0        0     4400 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/encoders.py
--rw-r--r--   0        0        0     1390 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/flows.py
--rw-r--r--   0        0        0     1405 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/losses.py
--rw-r--r--   0        0        0     5753 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/mel_processing.py
--rw-r--r--   0        0        0    14435 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/modules.py
--rw-r--r--   0        0        0     8178 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/synthesizers.py
--rw-r--r--   0        0        0        0 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/preprocessing/__init__.py
--rw-r--r--   0        0        0     1737 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json
--rw-r--r--   0        0        0     1487 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json
--rw-r--r--   0        0        0     1548 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json
--rw-r--r--   0        0        0     2793 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py
--rw-r--r--   0        0        0     4646 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py
--rw-r--r--   0        0        0     4382 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/preprocessing/preprocess_resample.py
--rw-r--r--   0        0        0     2948 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py
--rw-r--r--   0        0        0     1878 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/preprocessing/preprocess_split.py
--rw-r--r--   0        0        0      126 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/preprocessing/preprocess_utils.py
--rw-r--r--   0        0        0        0 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/py.typed
--rw-r--r--   0        0        0    20240 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/train.py
--rw-r--r--   0        0        0    13442 2023-04-18 10:19:48.038368 so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/utils.py
--rw-r--r--   0        0        0    20087 1970-01-01 00:00:00.000000 so_vits_svc_fork-3.9.5/PKG-INFO
+-rw-r--r--   0        0        0    12463 2023-05-29 12:04:20.100162 so_vits_svc_fork-4.0.0/LICENSE
+-rw-r--r--   0        0        0    27605 2023-05-29 12:04:20.100162 so_vits_svc_fork-4.0.0/README.md
+-rw-r--r--   0        0        0     3091 2023-05-29 12:04:21.044174 so_vits_svc_fork-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0       70 2023-05-29 12:04:20.996173 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/__init__.py
+-rw-r--r--   0        0        0    24434 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/__main__.py
+-rw-r--r--   0        0        0     1393 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/cluster/__init__.py
+-rw-r--r--   0        0        0     2844 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/cluster/train_cluster.py
+-rw-r--r--   0        0        0     2875 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/dataset.py
+-rw-r--r--   0        0        0     2599 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/default_gui_presets.json
+-rw-r--r--   0        0        0     7267 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/f0.py
+-rw-r--r--   0        0        0    29784 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/gui.py
+-rw-r--r--   0        0        0      864 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/hparams.py
+-rw-r--r--   0        0        0        0 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/inference/__init__.py
+-rw-r--r--   0        0        0    24604 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/inference/core.py
+-rw-r--r--   0        0        0     9408 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/inference/main.py
+-rw-r--r--   0        0        0     1169 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/logger.py
+-rw-r--r--   0        0        0        0 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/__init__.py
+-rw-r--r--   0        0        0    16683 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/attentions.py
+-rw-r--r--   0        0        0     4620 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/commons.py
+-rw-r--r--   0        0        0        0 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/decoders/__init__.py
+-rw-r--r--   0        0        0     1463 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/decoders/f0.py
+-rw-r--r--   0        0        0       76 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/decoders/hifigan/__init__.py
+-rw-r--r--   0        0        0    11618 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py
+-rw-r--r--   0        0        0      340 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/decoders/hifigan/_utils.py
+-rw-r--r--   0        0        0      318 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/decoders/mb_istft/__init__.py
+-rw-r--r--   0        0        0    12477 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py
+-rw-r--r--   0        0        0      419 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_loss.py
+-rw-r--r--   0        0        0     4725 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py
+-rw-r--r--   0        0        0     8954 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py
+-rw-r--r--   0        0        0     4879 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py
+-rw-r--r--   0        0        0     5604 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/descriminators.py
+-rw-r--r--   0        0        0     4400 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/encoders.py
+-rw-r--r--   0        0        0     1390 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/flows.py
+-rw-r--r--   0        0        0     1405 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/losses.py
+-rw-r--r--   0        0        0     5753 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/mel_processing.py
+-rw-r--r--   0        0        0    14435 2023-05-29 12:04:20.104162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/modules.py
+-rw-r--r--   0        0        0     8178 2023-05-29 12:04:20.108162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/synthesizers.py
+-rw-r--r--   0        0        0        0 2023-05-29 12:04:20.108162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/preprocessing/__init__.py
+-rw-r--r--   0        0        0     2051 2023-05-29 12:04:20.108162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json
+-rw-r--r--   0        0        0     1705 2023-05-29 12:04:20.108162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json
+-rw-r--r--   0        0        0     1862 2023-05-29 12:04:20.108162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json
+-rw-r--r--   0        0        0     2975 2023-05-29 12:04:20.108162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/preprocessing/preprocess_classify.py
+-rw-r--r--   0        0        0     2710 2023-05-29 12:04:20.108162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py
+-rw-r--r--   0        0        0     4667 2023-05-29 12:04:20.108162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py
+-rw-r--r--   0        0        0     4447 2023-05-29 12:04:20.108162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/preprocessing/preprocess_resample.py
+-rw-r--r--   0        0        0     2948 2023-05-29 12:04:20.108162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py
+-rw-r--r--   0        0        0     1878 2023-05-29 12:04:20.108162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/preprocessing/preprocess_split.py
+-rw-r--r--   0        0        0      126 2023-05-29 12:04:20.108162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/preprocessing/preprocess_utils.py
+-rw-r--r--   0        0        0        0 2023-05-29 12:04:20.108162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/py.typed
+-rw-r--r--   0        0        0    21359 2023-05-29 12:04:20.108162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/train.py
+-rw-r--r--   0        0        0    14797 2023-05-29 12:04:20.108162 so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/utils.py
+-rw-r--r--   0        0        0    29411 1970-01-01 00:00:00.000000 so_vits_svc_fork-4.0.0/PKG-INFO
```

### Comparing `so_vits_svc_fork-3.9.5/LICENSE` & `so_vits_svc_fork-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.5/pyproject.toml` & `so_vits_svc_fork-4.0.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "so-vits-svc-fork"
-version = "3.9.5"
+version = "4.0.0"
 description = "A fork of so-vits-svc."
 authors = ["34j <34j.95a2p@simplelogin.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/34j/so-vits-svc-fork"
 documentation = "https://so-vits-svc-fork.readthedocs.io"
 classifiers = [
@@ -29,50 +29,48 @@
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/34j/so-vits-svc-fork/issues"
 "Changelog" = "https://github.com/34j/so-vits-svc-fork/blob/main/CHANGELOG.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
 librosa = "*"
-fairseq = "*"
-flask = "*"
-flask_cors = "*"
-gradio = "*"
 numpy = "^1.23"
-pydub = "*"
 pyworld = "*"
 requests = "*"
 scipy = "*"
 sounddevice = "*"
 SoundFile = "*"
-starlette = "*"
 tqdm = "*"
-scikit-maad = "*"
 praat-parselmouth = "*"
 onnx = "*"
 onnxsim = "*"
 onnxoptimizer = "*"
-torch = ">=1.12"
-torchaudio = ">=0.12"
+torch = "*"
+torchaudio = "*"
 tensorboard = "*"
 rich = "*"
 tqdm-joblib = "*"
 tensorboardx = "*"
-pyinputplus = "*"
 cm-time = ">=0.1.2"
 pysimplegui = ">=4.6"
 pebble = ">=5.0"
 torchcrepe = ">=0.0.17"
 lightning = "^2.0.1"
 fastapi = "==0.88"
+transformers = "^4.28.1"
+matplotlib = "^3.7.1"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = ">=3"
 pytest = "^7.0"
 pytest-cov = "^4.0.0"
+poetry = "^1.4.2"
+pipdeptree = "^2.7.0"
+pip-licenses = "^4.3.1"
+black = "^23.3.0"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 myst-parser = ">=0.16"
 sphinx = ">=4.0"
```

### Comparing `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/__main__.py` & `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import os
 from logging import getLogger
 from multiprocessing import freeze_support
 from pathlib import Path
 from typing import Literal
 
 import click
-import pyinputplus as pyip
 import torch
 
 from so_vits_svc_fork import __version__
 from so_vits_svc_fork.utils import get_optimal_device
 
 LOG = getLogger(__name__)
 
@@ -128,14 +127,23 @@
 
     train(
         config_path=config_path, model_path=model_path, reset_optimizer=reset_optimizer
     )
 
 
 @cli.command()
+def gui():
+    """Opens GUI
+    for conversion and realtime inference"""
+    from .gui import main
+
+    main()
+
+
+@cli.command()
 @click.argument(
     "input-path",
     type=click.Path(exists=True),
 )
 @click.option(
     "-o",
     "--output-path",
@@ -160,14 +168,22 @@
 @click.option(
     "-k",
     "--cluster-model-path",
     type=click.Path(exists=True),
     default=None,
     help="path to cluster model",
 )
+@click.option(
+    "-re",
+    "--recursive",
+    type=bool,
+    default=False,
+    help="Search recursively",
+    is_flag=True,
+)
 @click.option("-t", "--transpose", type=int, default=0, help="transpose")
 @click.option(
     "-db", "--db-thresh", type=int, default=-20, help="threshold (DB) (RELATIVE)"
 )
 @click.option(
     "-fm",
     "--f0-method",
@@ -198,33 +214,42 @@
 @click.option(
     "-ab/-nab",
     "--absolute-thresh/--no-absolute-thresh",
     type=bool,
     default=False,
     help="absolute thresh",
 )
+@click.option(
+    "-mc",
+    "--max-chunk-seconds",
+    type=float,
+    default=40,
+    help="maximum allowed single chunk length, set lower if you get out of memory (0 to disable)",
+)
 def infer(
     # paths
     input_path: Path,
     output_path: Path,
     model_path: Path,
     config_path: Path,
+    recursive: bool,
     # svc config
     speaker: str,
     cluster_model_path: Path | None = None,
     transpose: int = 0,
     auto_predict_f0: bool = False,
     cluster_infer_ratio: float = 0,
     noise_scale: float = 0.4,
     f0_method: Literal["crepe", "crepe-tiny", "parselmouth", "dio", "harvest"] = "dio",
     # slice config
     db_thresh: int = -40,
     pad_seconds: float = 0.5,
     chunk_seconds: float = 0.5,
     absolute_thresh: bool = False,
+    max_chunk_seconds: float = 40,
     device: str | torch.device = get_optimal_device(),
 ):
     """Inference"""
     from so_vits_svc_fork.inference.main import infer
 
     if not auto_predict_f0:
         LOG.warning(
@@ -232,14 +257,18 @@
             "Generally transpose = 0 does not work because your voice pitch and target voice pitch are different."
         )
 
     input_path = Path(input_path)
     if output_path is None:
         output_path = input_path.parent / f"{input_path.stem}.out{input_path.suffix}"
     output_path = Path(output_path)
+    if input_path.is_dir() and not recursive:
+        raise ValueError(
+            "input_path is a directory. Use 0re or --recursive to infer recursively."
+        )
     model_path = Path(model_path)
     if model_path.is_dir():
         model_path = list(
             sorted(model_path.glob("G_*.pth"), key=lambda x: x.stat().st_mtime)
         )[-1]
         LOG.info(f"Since model_path is a directory, use {model_path}")
     config_path = Path(config_path)
@@ -247,27 +276,29 @@
         cluster_model_path = Path(cluster_model_path)
     infer(
         # paths
         input_path=input_path,
         output_path=output_path,
         model_path=model_path,
         config_path=config_path,
+        recursive=recursive,
         # svc config
         speaker=speaker,
         cluster_model_path=cluster_model_path,
         transpose=transpose,
         auto_predict_f0=auto_predict_f0,
         cluster_infer_ratio=cluster_infer_ratio,
         noise_scale=noise_scale,
         f0_method=f0_method,
         # slice config
         db_thresh=db_thresh,
         pad_seconds=pad_seconds,
         chunk_seconds=chunk_seconds,
         absolute_thresh=absolute_thresh,
+        max_chunk_seconds=max_chunk_seconds,
         device=device,
     )
 
 
 @cli.command()
 @click.option(
     "-m",
@@ -511,15 +542,15 @@
     default=Path("./configs/44k/config.json"),
     help="path to config",
 )
 @click.option(
     "-t",
     "--config-type",
     type=click.Choice([x.stem for x in CONFIG_TEMPLATE_DIR.rglob("*.json")]),
-    default="so-vits-svc-4.0v1-legacy",
+    default="so-vits-svc-4.0v1",
     help="config type",
 )
 def pre_config(
     input_dir: Path,
     filelist_path: Path,
     config_path: Path,
     config_type: str,
@@ -712,21 +743,61 @@
         frame_seconds=frame_seconds,
         hop_seconds=hop_seconds,
         n_jobs=n_jobs,
         sr=sr,
     )
 
 
+@cli.command()
+@click.option(
+    "-i",
+    "--input-dir",
+    type=click.Path(exists=True),
+    required=True,
+    help="path to source dir",
+)
+@click.option(
+    "-o",
+    "--output-dir",
+    type=click.Path(),
+    default=None,
+    help="path to output dir",
+)
+@click.option(
+    "-c/-nc",
+    "--create-new/--no-create-new",
+    type=bool,
+    default=True,
+    help="create a new folder for the speaker if not exist",
+)
+def pre_classify(
+    input_dir: Path | str,
+    output_dir: Path | str | None,
+    create_new: bool,
+) -> None:
+    """Classify multiple audio files into multiple files"""
+    from so_vits_svc_fork.preprocessing.preprocess_classify import preprocess_classify
+
+    if output_dir is None:
+        output_dir = input_dir
+    preprocess_classify(
+        input_dir=input_dir,
+        output_dir=output_dir,
+        create_new=create_new,
+    )
+
+
 @cli.command
 def clean():
     """Clean up files, only useful if you are using the default file structure"""
     import shutil
 
     folders = ["dataset", "filelists", "logs"]
-    if pyip.inputYesNo(f"Are you sure you want to delete files in {folders}?") == "yes":
+    # if pyip.inputYesNo(f"Are you sure you want to delete files in {folders}?") == "yes":
+    if input("Are you sure you want to delete files in {folders}?") in ["yes", "y"]:
         for folder in folders:
             if Path(folder).exists():
                 shutil.rmtree(folder)
         LOG.info("Cleaned up files")
     else:
         LOG.info("Aborted")
 
@@ -759,16 +830,16 @@
     type=str,
     default="cpu",
     help="device to use",
 )
 def onnx(
     input_path: Path, output_path: Path, config_path: Path, device: torch.device | str
 ) -> None:
+    """Export model to onnx (currently not working)"""
     raise NotImplementedError("ONNX export is not yet supported")
-    """Export model to onnx"""
     input_path = Path(input_path)
     if input_path.is_dir():
         input_path = list(input_path.glob("*.pth"))[0]
     if output_path is None:
         output_path = input_path.with_suffix(".onnx")
     output_path = Path(output_path)
     if output_path.is_dir():
```

### Comparing `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/cluster/__init__.py` & `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/cluster/train_cluster.py` & `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/cluster/train_cluster.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/dataset.py` & `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 class TextAudioDataset(Dataset):
     def __init__(self, hps: HParams, is_validation: bool = False):
         self.datapaths = [
             Path(x).parent / (Path(x).name + ".data.pt")
             for x in Path(
                 hps.data.validation_files if is_validation else hps.data.training_files
             )
-            .read_text()
+            .read_text("utf-8")
             .splitlines()
         ]
         self.hps = hps
         self.random = Random(hps.train.seed)
         self.random.shuffle(self.datapaths)
         self.max_spec_len = 800
```

### Comparing `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/default_gui_presets.json` & `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/default_gui_presets.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9681372549019608%*

 * *Differences: {"'Default File'": "{'max_chunk_seconds': 40}",*

 * * "'Default VC (CPU)'": "{'max_chunk_seconds': 40}",*

 * * "'Default VC (Crooning)'": "{'max_chunk_seconds': 40}",*

 * * "'Default VC (GPU, GTX 1060)'": "{'max_chunk_seconds': 40}",*

 * * "'Default VC (Mobile CPU)'": "{'max_chunk_seconds': 40}"}*

```diff
@@ -2,14 +2,15 @@
     "Default File": {
         "absolute_thresh": true,
         "auto_play": true,
         "auto_predict_f0": true,
         "chunk_seconds": 0.5,
         "cluster_infer_ratio": 0.0,
         "f0_method": "crepe",
+        "max_chunk_seconds": 40,
         "noise_scale": 0.4,
         "pad_seconds": 0.1,
         "passthrough_original": false,
         "silence_threshold": -35.0,
         "transpose": 0.0
     },
     "Default VC (CPU)": {
@@ -18,14 +19,15 @@
         "additional_infer_before_seconds": 0.01,
         "auto_predict_f0": false,
         "block_seconds": 1.5,
         "chunk_seconds": 0.5,
         "cluster_infer_ratio": 0.0,
         "crossfade_seconds": 0.05,
         "f0_method": "dio",
+        "max_chunk_seconds": 40,
         "noise_scale": 0.4,
         "pad_seconds": 0.1,
         "passthrough_original": false,
         "realtime_algorithm": "1 (Divide constantly)",
         "silence_threshold": -35.0,
         "transpose": 12.0,
         "use_gpu": false
@@ -36,14 +38,15 @@
         "additional_infer_before_seconds": 0.05,
         "auto_predict_f0": false,
         "block_seconds": 0.15,
         "chunk_seconds": 0.5,
         "cluster_infer_ratio": 0.0,
         "crossfade_seconds": 0.04,
         "f0_method": "dio",
+        "max_chunk_seconds": 40,
         "noise_scale": 0.4,
         "pad_seconds": 0.1,
         "passthrough_original": false,
         "realtime_algorithm": "1 (Divide constantly)",
         "silence_threshold": -35.0,
         "transpose": 12.0,
         "use_gpu": true
@@ -54,14 +57,15 @@
         "additional_infer_before_seconds": 0.15,
         "auto_predict_f0": false,
         "block_seconds": 0.35,
         "chunk_seconds": 0.5,
         "cluster_infer_ratio": 0.0,
         "crossfade_seconds": 0.05,
         "f0_method": "dio",
+        "max_chunk_seconds": 40,
         "noise_scale": 0.4,
         "pad_seconds": 0.1,
         "passthrough_original": false,
         "realtime_algorithm": "1 (Divide constantly)",
         "silence_threshold": -35.0,
         "transpose": 12.0,
         "use_gpu": true
@@ -72,14 +76,15 @@
         "additional_infer_before_seconds": 0.01,
         "auto_predict_f0": false,
         "block_seconds": 2.5,
         "chunk_seconds": 0.5,
         "cluster_infer_ratio": 0.0,
         "crossfade_seconds": 0.05,
         "f0_method": "dio",
+        "max_chunk_seconds": 40,
         "noise_scale": 0.4,
         "pad_seconds": 0.1,
         "passthrough_original": false,
         "realtime_algorithm": "1 (Divide constantly)",
         "silence_threshold": -35.0,
         "transpose": 12.0,
         "use_gpu": false
```

### Comparing `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/f0.py` & `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/f0.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/gui.py` & `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/gui.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,18 +7,17 @@
 from pathlib import Path
 
 import PySimpleGUI as sg
 import sounddevice as sd
 import soundfile as sf
 import torch
 from pebble import ProcessFuture, ProcessPool
-from tqdm.tk import tqdm_tk
 
 from . import __version__
-from .utils import ensure_pretrained_model, get_optimal_device
+from .utils import get_optimal_device
 
 GUI_DEFAULT_PRESETS_PATH = Path(__file__).parent / "default_gui_presets.json"
 GUI_PRESETS_PATH = Path("./user_gui_presets.json").absolute()
 
 LOG = getLogger(__name__)
 
 
@@ -26,17 +25,19 @@
     if isinstance(path, Path):
         path = path.as_posix()
     data, sr = sf.read(path)
     sd.play(data, sr)
 
 
 def load_presets() -> dict:
-    defaults = json.loads(GUI_DEFAULT_PRESETS_PATH.read_text())
+    defaults = json.loads(GUI_DEFAULT_PRESETS_PATH.read_text("utf-8"))
     users = (
-        json.loads(GUI_PRESETS_PATH.read_text()) if GUI_PRESETS_PATH.exists() else {}
+        json.loads(GUI_PRESETS_PATH.read_text("utf-8"))
+        if GUI_PRESETS_PATH.exists()
+        else {}
     )
     # prioriy: defaults > users
     # order: defaults -> users
     return {**defaults, **users, **defaults}
 
 
 def add_preset(name: str, preset: dict) -> dict:
@@ -54,14 +55,72 @@
     else:
         LOG.warning(f"Cannot delete preset {name} because it does not exist.")
     with GUI_PRESETS_PATH.open("w") as f:
         json.dump(presets, f, indent=2)
     return load_presets()
 
 
+def get_output_path(input_path: Path) -> Path:
+    # Default output path
+    output_path = input_path.parent / f"{input_path.stem}.out{input_path.suffix}"
+
+    # Increment file number in path if output file already exists
+    file_num = 1
+    while output_path.exists():
+        output_path = (
+            input_path.parent / f"{input_path.stem}.out_{file_num}{input_path.suffix}"
+        )
+        file_num += 1
+    return output_path
+
+
+def get_supported_file_types() -> tuple[tuple[str, str], ...]:
+    res = tuple(
+        [
+            (extension, f".{extension.lower()}")
+            for extension in sf.available_formats().keys()
+        ]
+    )
+
+    # Sort by popularity
+    common_file_types = ["WAV", "MP3", "FLAC", "OGG", "M4A", "WMA"]
+    res = sorted(
+        res,
+        key=lambda x: common_file_types.index(x[0])
+        if x[0] in common_file_types
+        else len(common_file_types),
+    )
+    return res
+
+
+def get_supported_file_types_concat() -> tuple[tuple[str, str], ...]:
+    return (("Audio", " ".join(sf.available_formats().keys())),)
+
+
+def validate_output_file_type(output_path: Path) -> bool:
+    supported_file_types = sorted(
+        [f".{extension.lower()}" for extension in sf.available_formats().keys()]
+    )
+    if not output_path.suffix:
+        sg.popup_ok(
+            "Error: Output path missing file type extension, enter "
+            + "one of the following manually:\n\n"
+            + "\n".join(supported_file_types)
+        )
+        return False
+    if output_path.suffix.lower() not in supported_file_types:
+        sg.popup_ok(
+            f"Error: {output_path.suffix.lower()} is not a supported "
+            + "extension; use one of the following:\n\n"
+            + "\n".join(supported_file_types)
+        )
+        return False
+    return True
+
+
 def get_devices(
     update: bool = True,
 ) -> tuple[list[str], list[str], list[int], list[int]]:
     if update:
         sd._terminate()
         sd._initialize()
     devices = sd.query_devices()
@@ -95,33 +154,33 @@
             play_audio(output_path)
     except Exception as e:
         LOG.exception(e)
 
 
 def main():
     LOG.info(f"version: {__version__}")
-    try:
-        ensure_pretrained_model(".", "contentvec", tqdm_cls=tqdm_tk)
-    except Exception as e:
-        LOG.exception(e)
-        LOG.info("Trying tqdm.std...")
-        try:
-            ensure_pretrained_model(".", "contentvec")
-        except Exception as e:
-            LOG.exception(e)
-            try:
-                ensure_pretrained_model(".", "contentvec", disabled=True)
-            except Exception as e:
-                LOG.exception(e)
-                LOG.error(
-                    "Failed to download Hubert model. Please download it manually."
-                )
-                return
 
-    sg.theme("Dark")
+    # sg.theme("Dark")
+    sg.theme_add_new(
+        "Very Dark",
+        {
+            "BACKGROUND": "#111111",
+            "TEXT": "#FFFFFF",
+            "INPUT": "#444444",
+            "TEXT_INPUT": "#FFFFFF",
+            "SCROLL": "#333333",
+            "BUTTON": ("white", "#112233"),
+            "PROGRESS": ("#111111", "#333333"),
+            "BORDER": 2,
+            "SLIDER_DEPTH": 2,
+            "PROGRESS_DEPTH": 2,
+        },
+    )
+    sg.theme("Very Dark")
+
     model_candidates = list(sorted(Path("./logs/44k/").glob("G_*.pth")))
 
     frame_contents = {
         "Paths": [
             [
                 sg.Text("Model path"),
                 sg.Push(),
@@ -133,15 +192,18 @@
                     enable_events=True,
                 ),
                 sg.FileBrowse(
                     initial_folder=Path("./logs/44k/").absolute
                     if Path("./logs/44k/").exists()
                     else Path(".").absolute().as_posix(),
                     key="model_path_browse",
-                    file_types=(("PyTorch", "*.pth"),),
+                    file_types=(
+                        ("PyTorch", "G_*.pth G_*.pt"),
+                        ("Pytorch", "*.pth *.pt"),
+                    ),
                 ),
             ],
             [
                 sg.Text("Config path"),
                 sg.Push(),
                 sg.InputText(
                     key="config_path",
@@ -169,15 +231,15 @@
                     enable_events=True,
                 ),
                 sg.FileBrowse(
                     initial_folder="./logs/44k/"
                     if Path("./logs/44k/").exists()
                     else ".",
                     key="cluster_model_path_browse",
-                    file_types=(("PyTorch", "*.pt"),),
+                    file_types=(("PyTorch", "*.pt"), ("Pickle", "*.pt *.pth *.pkl")),
                 ),
             ],
         ],
         "Common": [
             [
                 sg.Text("Speaker"),
                 sg.Push(),
@@ -259,28 +321,58 @@
                     range=(0.0, 3.0),
                     orientation="h",
                     key="chunk_seconds",
                     resolution=0.01,
                 ),
             ],
             [
+                sg.Text("Max chunk seconds (set lower if Out Of Memory, 0 to disable)"),
+                sg.Push(),
+                sg.Slider(
+                    range=(0.0, 240.0),
+                    orientation="h",
+                    key="max_chunk_seconds",
+                    resolution=1.0,
+                ),
+            ],
+            [
                 sg.Checkbox(
                     key="absolute_thresh",
                     text="Absolute threshold (ignored (True) in realtime inference)",
                 )
             ],
         ],
         "File": [
             [
                 sg.Text("Input audio path"),
                 sg.Push(),
-                sg.InputText(key="input_path"),
-                sg.FileBrowse(initial_folder=".", key="input_path_browse"),
+                sg.InputText(key="input_path", enable_events=True),
+                sg.FileBrowse(
+                    initial_folder=".",
+                    key="input_path_browse",
+                    file_types=get_supported_file_types_concat(),
+                ),
+                sg.FolderBrowse(
+                    button_text="Browse(Folder)",
+                    initial_folder=".",
+                    key="input_path_folder_browse",
+                    target="input_path",
+                ),
                 sg.Button("Play", key="play_input"),
             ],
+            [
+                sg.Text("Output audio path"),
+                sg.Push(),
+                sg.InputText(key="output_path"),
+                sg.FileSaveAs(
+                    initial_folder=".",
+                    key="output_path_browse",
+                    file_types=get_supported_file_types(),
+                ),
+            ],
             [sg.Checkbox(key="auto_play", text="Auto play", default=True)],
         ],
         "Realtime": [
             [
                 sg.Text("Crossfade seconds"),
                 sg.Push(),
                 sg.Slider(
@@ -386,23 +478,23 @@
         "Presets": [
             [
                 sg.Text("Presets"),
                 sg.Push(),
                 sg.Combo(
                     key="presets",
                     values=list(load_presets().keys()),
-                    size=(20, 1),
+                    size=(40, 1),
                     enable_events=True,
                 ),
                 sg.Button("Delete preset", key="delete_preset"),
             ],
             [
                 sg.Text("Preset name"),
                 sg.Stretch(),
-                sg.InputText(key="preset_name", size=(20, 1)),
+                sg.InputText(key="preset_name", size=(26, 1)),
                 sg.Button("Add current settings as a preset", key="add_preset"),
             ],
         ],
     }
 
     # frames
     frames = {}
@@ -446,16 +538,23 @@
         ]
     )
 
     # columns
     layout = [[column1, column2]]
     # layout = [[sg.Column(layout, vertical_alignment="top", scrollable=True, expand_x=True, expand_y=True)]]
     window = sg.Window(
-        f"{__name__.split('.')[0]}", layout, grab_anywhere=True, finalize=True
-    )  # , use_custom_titlebar=True)
+        f"{__name__.split('.')[0].replace('_', '-')} v{__version__}",
+        layout,
+        grab_anywhere=True,
+        finalize=True,
+        # Below disables taskbar, which may be not useful for some users
+        # use_custom_titlebar=True, no_titlebar=False
+        # Keep on top
+        # keep_on_top=True
+    )
     # for n in ["input_device", "output_device"]:
     #     window[n].Widget.configure(justify="right")
     event, values = window.read(timeout=0.01)
 
     def update_speaker() -> None:
         from . import utils
 
@@ -542,14 +641,18 @@
                             browser.update()
                         else:
                             LOG.warning(f"Browser {browser} is not a FileBrowse")
             window["transpose"].update(
                 disabled=values["auto_predict_f0"],
                 visible=not values["auto_predict_f0"],
             )
+
+            input_path = Path(values["input_path"])
+            output_path = Path(values["output_path"])
+
             if event == "add_preset":
                 presets = add_preset(
                     values["preset_name"], {key: values[key] for key in PRESET_KEYS}
                 )
                 window["presets"].update(values=list(presets.keys()))
             elif event == "delete_preset":
                 presets = delete_preset(values["presets"])
@@ -557,36 +660,49 @@
             elif event == "presets":
                 apply_preset(values["presets"])
                 update_speaker()
             elif event == "refresh_devices":
                 update_devices()
             elif event == "config_path":
                 update_speaker()
+            elif event == "input_path":
+                # Don't change the output path if it's already set
+                # if values["output_path"]:
+                #     continue
+                # Set a sensible default output path
+                window.Element("output_path").Update(str(get_output_path(input_path)))
             elif event == "infer":
-                input_path = Path(values["input_path"])
-                output_path = (
-                    input_path.parent / f"{input_path.stem}.out{input_path.suffix}"
-                )
-                if not input_path.exists() or not input_path.is_file():
+                if "Default VC" in values["presets"]:
+                    window["presets"].update(
+                        set_to_index=list(load_presets().keys()).index("Default File")
+                    )
+                    apply_preset("Default File")
+                if values["input_path"] == "":
+                    LOG.warning("Input path is empty.")
+                    continue
+                if not input_path.exists():
                     LOG.warning(f"Input path {input_path} does not exist.")
                     continue
+                # if not validate_output_file_type(output_path):
+                #     continue
 
                 try:
                     from so_vits_svc_fork.inference.main import infer
 
                     LOG.info("Starting inference...")
                     window["infer"].update(disabled=True)
                     infer_future = pool.schedule(
                         infer,
                         kwargs=dict(
                             # paths
                             model_path=Path(values["model_path"]),
                             output_path=output_path,
                             input_path=input_path,
                             config_path=Path(values["config_path"]),
+                            recursive=True,
                             # svc config
                             speaker=values["speaker"],
                             cluster_model_path=Path(values["cluster_model_path"])
                             if values["cluster_model_path"]
                             else None,
                             transpose=values["transpose"],
                             auto_predict_f0=values["auto_predict_f0"],
@@ -594,14 +710,15 @@
                             noise_scale=values["noise_scale"],
                             f0_method=values["f0_method"],
                             # slice config
                             db_thresh=values["silence_threshold"],
                             pad_seconds=values["pad_seconds"],
                             chunk_seconds=values["chunk_seconds"],
                             absolute_thresh=values["absolute_thresh"],
+                            max_chunk_seconds=values["max_chunk_seconds"],
                             device="cpu"
                             if not values["use_gpu"]
                             else get_optimal_device(),
                         ),
                     )
                     infer_future.add_done_callback(
                         lambda _future: after_inference(
```

### Comparing `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/hparams.py` & `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/hparams.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/inference/core.py` & `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/inference/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 def split_silence(
     audio: ndarray[Any, dtype[float32]],
     top_db: int = 40,
     ref: float | Callable[[ndarray[Any, dtype[float32]]], float] = 1,
     frame_length: int = 2048,
     hop_length: int = 512,
     aggregate: Callable[[ndarray[Any, dtype[float32]]], float] = np.mean,
+    max_chunk_length: int = 0,
 ) -> Iterable[Chunk]:
     non_silence_indices = librosa.effects.split(
         audio,
         top_db=top_db,
         ref=ref,
         frame_length=frame_length,
         hop_length=hop_length,
@@ -75,15 +76,24 @@
     )
     last_end = 0
     for start, end in non_silence_indices:
         if start != last_end:
             yield Chunk(
                 is_speech=False, audio=audio[last_end:start], start=last_end, end=start
             )
-        yield Chunk(is_speech=True, audio=audio[start:end], start=start, end=end)
+        while max_chunk_length > 0 and end - start > max_chunk_length:
+            yield Chunk(
+                is_speech=True,
+                audio=audio[start : start + max_chunk_length],
+                start=start,
+                end=start + max_chunk_length,
+            )
+            start += max_chunk_length
+        if end - start > 0:
+            yield Chunk(is_speech=True, audio=audio[start:end], start=start, end=end)
         last_end = end
     if last_end != len(audio):
         yield Chunk(
             is_speech=False, audio=audio[last_end:], start=last_end, end=len(audio)
         )
 
 
@@ -102,15 +112,17 @@
             self.device = (get_optimal_device(),)
         else:
             self.device = torch.device(device)
         self.hps = utils.get_hparams(config_path)
         self.target_sample = self.hps.data.sampling_rate
         self.hop_size = self.hps.data.hop_length
         self.spk2id = self.hps.spk
-        self.hubert_model = utils.get_hubert_model(self.device)
+        self.hubert_model = utils.get_hubert_model(
+            self.device, self.hps.data.get("contentvec_final_proj", True)
+        )
         self.dtype = torch.float16 if half else torch.float32
         self.contentvec_final_proj = self.hps.data.__dict__.get(
             "contentvec_final_proj", True
         )
         self.load_model()
         if cluster_model_path is not None and Path(cluster_model_path).exists():
             self.cluster_model = cluster.get_cluster_model(cluster_model_path)
@@ -242,14 +254,15 @@
             "crepe", "crepe-tiny", "parselmouth", "dio", "harvest"
         ] = "dio",
         # slice config
         db_thresh: int = -40,
         pad_seconds: float = 0.5,
         chunk_seconds: float = 0.5,
         absolute_thresh: bool = False,
+        max_chunk_seconds: float = 40,
         # fade_seconds: float = 0.0,
     ) -> np.ndarray[Any, np.dtype[np.float32]]:
         sr = self.target_sample
         result_audio = np.array([], dtype=np.float32)
         chunk_length_min = chunk_length_min = (
             int(
                 min(
@@ -261,14 +274,15 @@
         )
         for chunk in split_silence(
             audio,
             top_db=-db_thresh,
             frame_length=chunk_length_min * 2,
             hop_length=chunk_length_min,
             ref=1 if absolute_thresh else np.max,
+            max_chunk_length=int(max_chunk_seconds * sr),
         ):
             LOG.info(f"Chunk: {chunk}")
             if not chunk.is_speech:
                 audio_chunk_infer = np.zeros_like(chunk.audio)
             else:
                 # pad
                 pad_len = int(sr * pad_seconds)
```

### Comparing `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/inference/main.py` & `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/inference/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,77 +1,119 @@
 from __future__ import annotations
 
 from logging import getLogger
 from pathlib import Path
-from typing import Literal
+from typing import Literal, Sequence
 
 import librosa
 import numpy as np
 import soundfile
 import torch
 from cm_time import timer
+from tqdm import tqdm
 
 from so_vits_svc_fork.inference.core import RealtimeVC, RealtimeVC2, Svc
 from so_vits_svc_fork.utils import get_optimal_device
 
 LOG = getLogger(__name__)
 
 
 def infer(
     *,
     # paths
-    input_path: Path | str,
-    output_path: Path | str,
+    input_path: Path | str | Sequence[Path | str],
+    output_path: Path | str | Sequence[Path | str],
     model_path: Path | str,
     config_path: Path | str,
+    recursive: bool = False,
     # svc config
     speaker: int | str,
     cluster_model_path: Path | str | None = None,
     transpose: int = 0,
     auto_predict_f0: bool = False,
     cluster_infer_ratio: float = 0,
     noise_scale: float = 0.4,
     f0_method: Literal["crepe", "crepe-tiny", "parselmouth", "dio", "harvest"] = "dio",
     # slice config
     db_thresh: int = -40,
     pad_seconds: float = 0.5,
     chunk_seconds: float = 0.5,
     absolute_thresh: bool = False,
+    max_chunk_seconds: float = 40,
     device: str | torch.device = get_optimal_device(),
 ):
+    if isinstance(input_path, (str, Path)):
+        input_path = [input_path]
+    if isinstance(output_path, (str, Path)):
+        output_path = [output_path]
+    if len(input_path) != len(output_path):
+        raise ValueError(
+            f"input_path and output_path must have same length, but got {len(input_path)} and {len(output_path)}"
+        )
+
     model_path = Path(model_path)
-    output_path = Path(output_path)
-    input_path = Path(input_path)
     config_path = Path(config_path)
+    output_path = [Path(p) for p in output_path]
+    input_path = [Path(p) for p in input_path]
+    output_paths = []
+    input_paths = []
+
+    for input_path, output_path in zip(input_path, output_path):
+        if input_path.is_dir():
+            if not recursive:
+                raise ValueError(
+                    f"input_path is a directory, but recursive is False: {input_path}"
+                )
+            input_paths.extend(list(input_path.rglob("*.*")))
+            output_paths.extend(
+                [output_path / p.relative_to(input_path) for p in input_paths]
+            )
+            continue
+        input_paths.append(input_path)
+        output_paths.append(output_path)
+
     cluster_model_path = Path(cluster_model_path) if cluster_model_path else None
     svc_model = Svc(
         net_g_path=model_path.as_posix(),
         config_path=config_path.as_posix(),
         cluster_model_path=cluster_model_path.as_posix()
         if cluster_model_path
         else None,
         device=device,
     )
 
-    audio, _ = librosa.load(input_path, sr=svc_model.target_sample)
-    audio = svc_model.infer_silence(
-        audio.astype(np.float32),
-        speaker=speaker,
-        transpose=transpose,
-        auto_predict_f0=auto_predict_f0,
-        cluster_infer_ratio=cluster_infer_ratio,
-        noise_scale=noise_scale,
-        f0_method=f0_method,
-        db_thresh=db_thresh,
-        pad_seconds=pad_seconds,
-        chunk_seconds=chunk_seconds,
-        absolute_thresh=absolute_thresh,
-    )
-
-    soundfile.write(output_path, audio, svc_model.target_sample)
+    try:
+        pbar = tqdm(list(zip(input_paths, output_paths)), disable=len(input_paths) == 1)
+        for input_path, output_path in pbar:
+            pbar.set_description(f"{input_path}")
+            try:
+                audio, _ = librosa.load(input_path, sr=svc_model.target_sample)
+            except Exception as e:
+                LOG.error(f"Failed to load {input_path}")
+                LOG.exception(e)
+                continue
+            output_path.parent.mkdir(parents=True, exist_ok=True)
+            audio = svc_model.infer_silence(
+                audio.astype(np.float32),
+                speaker=speaker,
+                transpose=transpose,
+                auto_predict_f0=auto_predict_f0,
+                cluster_infer_ratio=cluster_infer_ratio,
+                noise_scale=noise_scale,
+                f0_method=f0_method,
+                db_thresh=db_thresh,
+                pad_seconds=pad_seconds,
+                chunk_seconds=chunk_seconds,
+                absolute_thresh=absolute_thresh,
+                max_chunk_seconds=max_chunk_seconds,
+            )
+            soundfile.write(output_path, audio, svc_model.target_sample)
+    finally:
+        del svc_model
+        torch.cuda.empty_cache()
 
 
 def realtime(
     *,
     # paths
     model_path: Path | str,
     config_path: Path | str,
@@ -209,18 +251,22 @@
         else:
             outdata[:] = inference
         rtf = t.elapsed / block_seconds
         LOG.info(f"Realtime inference time: {t.elapsed:.3f}s, RTF: {rtf:.3f}")
         if rtf > 1:
             LOG.warning("RTF is too high, consider increasing block_seconds")
 
-    with sd.Stream(
-        device=(input_device, output_device),
-        channels=1,
-        callback=callback,
-        samplerate=svc_model.target_sample,
-        blocksize=int(block_seconds * svc_model.target_sample),
-        latency="low",
-    ) as stream:
-        LOG.info(f"Latency: {stream.latency}")
-        while True:
-            sd.sleep(1000)
+    try:
+        with sd.Stream(
+            device=(input_device, output_device),
+            channels=1,
+            callback=callback,
+            samplerate=svc_model.target_sample,
+            blocksize=int(block_seconds * svc_model.target_sample),
+            latency="low",
+        ) as stream:
+            LOG.info(f"Latency: {stream.latency}")
+            while True:
+                sd.sleep(1000)
+    finally:
+        # del model, svc_model
+        torch.cuda.empty_cache()
```

### Comparing `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/logger.py` & `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/logger.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,10 @@
 import os
 import sys
-from logging import (
-    DEBUG,
-    INFO,
-    FileHandler,
-    StreamHandler,
-    basicConfig,
-    captureWarnings,
-    getLogger,
-)
+from logging import DEBUG, INFO, StreamHandler, basicConfig, captureWarnings, getLogger
 from pathlib import Path
 
 from rich.logging import RichHandler
 
 LOGGER_INIT = False
 
 
@@ -25,15 +17,15 @@
     package_name = sys.modules[__name__].__package__
     basicConfig(
         level=INFO,
         format="%(asctime)s %(message)s",
         datefmt="[%X]",
         handlers=[
             StreamHandler() if is_notebook() else RichHandler(),
-            FileHandler(f"{package_name}.log"),
+            # FileHandler(f"{package_name}.log"),
         ],
     )
     if IS_TEST:
         getLogger(package_name).setLevel(DEBUG)
     captureWarnings(True)
     LOGGER_INIT = True
```

### Comparing `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/attentions.py` & `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/attentions.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/commons.py` & `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/commons.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/decoders/f0.py` & `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/decoders/f0.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,13 +33,14 @@
         self.proj = nn.Conv1d(hidden_channels, out_channels, 1)
         self.f0_prenet = nn.Conv1d(1, hidden_channels, 3, padding=1)
         self.cond = nn.Conv1d(spk_channels, hidden_channels, 1)
 
     def forward(self, x, norm_f0, x_mask, spk_emb=None):
         x = torch.detach(x)
         if spk_emb is not None:
+            spk_emb = torch.detach(spk_emb)
             x = x + self.cond(spk_emb)
         x += self.f0_prenet(norm_f0)
         x = self.prenet(x) * x_mask
         x = self.decoder(x * x_mask, x_mask)
         x = self.proj(x) * x_mask
         return x
```

### Comparing `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py` & `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/decoders/hifigan/_models.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py` & `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_generators.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py` & `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_pqmf.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py` & `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py` & `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/decoders/mb_istft/_stft_loss.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/descriminators.py` & `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/descriminators.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/encoders.py` & `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/encoders.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/flows.py` & `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/flows.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/losses.py` & `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/losses.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/mel_processing.py` & `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/mel_processing.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/modules.py` & `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/modules.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/modules/synthesizers.py` & `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/modules/synthesizers.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json` & `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9318946452098626%*

 * *Differences: {"'data'": "{delete: ['contentvec_final_proj']}",*

 * * "'model'": "{'upsample_rates': {insert: [(1, 8), (2, 2), (3, 2), (4, 2)], delete: [1]}, "*

 * *            "'upsample_kernel_sizes': {insert: [(0, 16), (2, 4), (3, 4), (4, 4)], delete: [0]}, "*

 * *            "'ssl_dim': 256, 'pretrained': OrderedDict([('D_0.pth', "*

 * *            "'https://huggingface.co/therealvul/so-vits-svc-4.0-init/resolve/main/D_0.pth'), "*

 * *            "('G_0.pth', "*

 * *            "'https://huggingface.co/therealvul/so-vits-svc-4.0-init/resolve/main […]*

```diff
@@ -1,34 +1,35 @@
 {
     "data": {
-        "contentvec_final_proj": false,
         "filter_length": 2048,
         "hop_length": 512,
         "max_wav_value": 32768.0,
         "mel_fmax": 22050,
         "mel_fmin": 0.0,
         "n_mel_channels": 80,
         "sampling_rate": 44100,
         "training_files": "filelists/44k/train.txt",
         "validation_files": "filelists/44k/val.txt",
         "win_length": 2048
     },
     "model": {
         "filter_channels": 768,
-        "gen_istft_hop_size": 4,
-        "gen_istft_n_fft": 16,
         "gin_channels": 256,
         "hidden_channels": 192,
         "inter_channels": 192,
         "kernel_size": 3,
         "n_heads": 2,
         "n_layers": 6,
         "n_layers_q": 3,
         "n_speakers": 200,
         "p_dropout": 0.1,
+        "pretrained": {
+            "D_0.pth": "https://huggingface.co/therealvul/so-vits-svc-4.0-init/resolve/main/D_0.pth",
+            "G_0.pth": "https://huggingface.co/therealvul/so-vits-svc-4.0-init/resolve/main/G_0.pth"
+        },
         "resblock": "1",
         "resblock_dilation_sizes": [
             [
                 1,
                 3,
                 5
             ],
@@ -44,25 +45,29 @@
             ]
         ],
         "resblock_kernel_sizes": [
             3,
             7,
             11
         ],
-        "ssl_dim": 768,
-        "subbands": 4,
-        "type_": "ms-istft",
+        "ssl_dim": 256,
         "upsample_initial_channel": 512,
         "upsample_kernel_sizes": [
-            32,
-            16
+            16,
+            16,
+            4,
+            4,
+            4
         ],
         "upsample_rates": [
             8,
-            4
+            8,
+            2,
+            2,
+            2
         ],
         "use_spectral_norm": false
     },
     "spk": {},
     "train": {
         "accumulate_grad_batches": 1,
         "batch_size": 16,
@@ -72,40 +77,24 @@
         ],
         "bf16_run": false,
         "c_kl": 1.0,
         "c_mel": 45,
         "ckpt_name_by_step": false,
         "epochs": 10000,
         "eps": 1e-09,
-        "eval_interval": 200,
-        "fft_sizes": [
-            768,
-            1366,
-            342
-        ],
+        "eval_interval": 800,
         "fp16_run": false,
-        "hop_sizes": [
-            60,
-            120,
-            20
-        ],
         "init_lr_ratio": 1,
         "keep_ckpts": 3,
         "learning_rate": 0.0001,
-        "log_interval": 100,
+        "log_interval": 200,
         "log_version": 0,
         "lr_decay": 0.999875,
         "max_speclen": 512,
         "num_workers": 4,
         "port": "8001",
         "seed": 1234,
         "segment_size": 10240,
         "use_sr": true,
-        "warmup_epochs": 0,
-        "win_lengths": [
-            300,
-            600,
-            120
-        ],
-        "window": "hann_window"
+        "warmup_epochs": 0
     }
 }
```

### Comparing `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1-legacy.json` & `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9678030303030303%*

 * *Differences: {"'data'": "{'contentvec_final_proj': False}",*

 * * "'model'": "{'ssl_dim': 768, 'type_': 'hifi-gan', 'pretrained': OrderedDict([('D_0.pth', "*

 * *            "'https://huggingface.co/datasets/ms903/sovits4.0-768vec-layer12/resolve/main/sovits_768l12_pre_large_320k/clean_D_320000.pth'), "*

 * *            "('G_0.pth', "*

 * *            "'https://huggingface.co/datasets/ms903/sovits4.0-768vec-layer12/resolve/main/sovits_768l12_pre_large_320k/clean_G_320000.pth')])}",*

 * * "'train'": "{'log_interval': 100, 'eval_interval': 200}"}*

```diff
@@ -1,9 +1,10 @@
 {
     "data": {
+        "contentvec_final_proj": false,
         "filter_length": 2048,
         "hop_length": 512,
         "max_wav_value": 32768.0,
         "mel_fmax": 22050,
         "mel_fmin": 0.0,
         "n_mel_channels": 80,
         "sampling_rate": 44100,
@@ -18,14 +19,18 @@
         "inter_channels": 192,
         "kernel_size": 3,
         "n_heads": 2,
         "n_layers": 6,
         "n_layers_q": 3,
         "n_speakers": 200,
         "p_dropout": 0.1,
+        "pretrained": {
+            "D_0.pth": "https://huggingface.co/datasets/ms903/sovits4.0-768vec-layer12/resolve/main/sovits_768l12_pre_large_320k/clean_D_320000.pth",
+            "G_0.pth": "https://huggingface.co/datasets/ms903/sovits4.0-768vec-layer12/resolve/main/sovits_768l12_pre_large_320k/clean_G_320000.pth"
+        },
         "resblock": "1",
         "resblock_dilation_sizes": [
             [
                 1,
                 3,
                 5
             ],
@@ -41,15 +46,16 @@
             ]
         ],
         "resblock_kernel_sizes": [
             3,
             7,
             11
         ],
-        "ssl_dim": 256,
+        "ssl_dim": 768,
+        "type_": "hifi-gan",
         "upsample_initial_channel": 512,
         "upsample_kernel_sizes": [
             16,
             16,
             4,
             4,
             4
@@ -73,20 +79,20 @@
         ],
         "bf16_run": false,
         "c_kl": 1.0,
         "c_mel": 45,
         "ckpt_name_by_step": false,
         "epochs": 10000,
         "eps": 1e-09,
-        "eval_interval": 800,
+        "eval_interval": 200,
         "fp16_run": false,
         "init_lr_ratio": 1,
         "keep_ckpts": 3,
         "learning_rate": 0.0001,
-        "log_interval": 200,
+        "log_interval": 100,
         "log_version": 0,
         "lr_decay": 0.999875,
         "max_speclen": 512,
         "num_workers": 4,
         "port": "8001",
         "seed": 1234,
         "segment_size": 10240,
```

### Comparing `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/preprocessing/config_templates/so-vits-svc-4.0v1.json` & `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/preprocessing/config_templates/quickvc.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9531573498964804%*

 * *Differences: {"'model'": "{'upsample_rates': {insert: [(1, 4)], delete: [4, 3, 2, 0]}, 'upsample_kernel_sizes': "*

 * *            "{insert: [(0, 32)], delete: [4, 3, 2, 0]}, 'type_': 'ms-istft', 'gen_istft_n_fft': "*

 * *            "16, 'gen_istft_hop_size': 4, 'subbands': 4, 'pretrained': OrderedDict([('D_0.pth', "*

 * *            "'https://huggingface.co/datasets/ms903/sovits4.0-768vec-layer12/resolve/main/sovits_768l12_pre_large_320k/clean_D_320000.pth'), "*

 * *            "('G_0.pth', "*

 * *            "'https://huggingface.co/datasets […]*

```diff
@@ -10,23 +10,29 @@
         "sampling_rate": 44100,
         "training_files": "filelists/44k/train.txt",
         "validation_files": "filelists/44k/val.txt",
         "win_length": 2048
     },
     "model": {
         "filter_channels": 768,
+        "gen_istft_hop_size": 4,
+        "gen_istft_n_fft": 16,
         "gin_channels": 256,
         "hidden_channels": 192,
         "inter_channels": 192,
         "kernel_size": 3,
         "n_heads": 2,
         "n_layers": 6,
         "n_layers_q": 3,
         "n_speakers": 200,
         "p_dropout": 0.1,
+        "pretrained": {
+            "D_0.pth": "https://huggingface.co/datasets/ms903/sovits4.0-768vec-layer12/resolve/main/sovits_768l12_pre_large_320k/clean_D_320000.pth",
+            "G_0.pth": "https://huggingface.co/datasets/ms903/sovits4.0-768vec-layer12/resolve/main/sovits_768l12_pre_large_320k/clean_G_320000.pth"
+        },
         "resblock": "1",
         "resblock_dilation_sizes": [
             [
                 1,
                 3,
                 5
             ],
@@ -43,29 +49,24 @@
         ],
         "resblock_kernel_sizes": [
             3,
             7,
             11
         ],
         "ssl_dim": 768,
-        "type_": "hifi-gan",
+        "subbands": 4,
+        "type_": "ms-istft",
         "upsample_initial_channel": 512,
         "upsample_kernel_sizes": [
-            16,
-            16,
-            4,
-            4,
-            4
+            32,
+            16
         ],
         "upsample_rates": [
             8,
-            8,
-            2,
-            2,
-            2
+            4
         ],
         "use_spectral_norm": false
     },
     "spk": {},
     "train": {
         "accumulate_grad_batches": 1,
         "batch_size": 16,
@@ -76,23 +77,39 @@
         "bf16_run": false,
         "c_kl": 1.0,
         "c_mel": 45,
         "ckpt_name_by_step": false,
         "epochs": 10000,
         "eps": 1e-09,
         "eval_interval": 200,
+        "fft_sizes": [
+            768,
+            1366,
+            342
+        ],
         "fp16_run": false,
+        "hop_sizes": [
+            60,
+            120,
+            20
+        ],
         "init_lr_ratio": 1,
         "keep_ckpts": 3,
         "learning_rate": 0.0001,
         "log_interval": 100,
         "log_version": 0,
         "lr_decay": 0.999875,
         "max_speclen": 512,
         "num_workers": 4,
         "port": "8001",
         "seed": 1234,
         "segment_size": 10240,
         "use_sr": true,
-        "warmup_epochs": 0
+        "warmup_epochs": 0,
+        "win_lengths": [
+            300,
+            600,
+            120
+        ],
+        "window": "hann_window"
     }
 }
```

### Comparing `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py` & `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/preprocessing/preprocess_flist_config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from __future__ import annotations
 
 import json
 import os
 from copy import deepcopy
 from logging import getLogger
 from pathlib import Path
-from random import shuffle
 
+import numpy as np
 from librosa import get_duration
 from tqdm import tqdm
 
 LOG = getLogger(__name__)
 CONFIG_TEMPLATE_DIR = Path(__file__).parent / "config_templates"
 
 
@@ -28,60 +28,57 @@
     test_list_path = Path(test_list_path)
     config_path = Path(config_path)
     train = []
     val = []
     test = []
     spk_dict = {}
     spk_id = 0
+    random = np.random.RandomState(1234)
     for speaker in os.listdir(input_dir):
         spk_dict[speaker] = spk_id
         spk_id += 1
         paths = []
         for path in tqdm(list((input_dir / speaker).rglob("*.wav"))):
             if get_duration(filename=path) < 0.3:
                 LOG.warning(f"skip {path} because it is too short.")
                 continue
             paths.append(path)
-        shuffle(paths)
+        random.shuffle(paths)
         if len(paths) <= 4:
             raise ValueError(
                 f"too few files in {input_dir / speaker} (expected at least 5)."
             )
         train += paths[2:-2]
         val += paths[:2]
         test += paths[-2:]
 
     LOG.info(f"Writing {train_list_path}")
     train_list_path.parent.mkdir(parents=True, exist_ok=True)
-    with train_list_path.open("w", encoding="utf-8") as f:
-        for fname in train:
-            wavpath = fname.as_posix()
-            f.write(wavpath + "\n")
+    train_list_path.write_text(
+        "\n".join([x.as_posix() for x in train]), encoding="utf-8"
+    )
 
     LOG.info(f"Writing {val_list_path}")
     val_list_path.parent.mkdir(parents=True, exist_ok=True)
-    with val_list_path.open("w", encoding="utf-8") as f:
-        for fname in val:
-            wavpath = fname.as_posix()
-            f.write(wavpath + "\n")
+    val_list_path.write_text("\n".join([x.as_posix() for x in val]), encoding="utf-8")
 
     LOG.info(f"Writing {test_list_path}")
     test_list_path.parent.mkdir(parents=True, exist_ok=True)
-    with test_list_path.open("w", encoding="utf-8") as f:
-        for fname in test:
-            wavpath = fname.as_posix()
-            f.write(wavpath + "\n")
+    test_list_path.write_text("\n".join([x.as_posix() for x in test]), encoding="utf-8")
 
     config = deepcopy(
         json.loads(
             (
-                CONFIG_TEMPLATE_DIR / f"{config_name}.json"
-                if not config_name.endswith(".json")
-                else config_name
-            ).read_text()
+                CONFIG_TEMPLATE_DIR
+                / (
+                    config_name
+                    if config_name.endswith(".json")
+                    else config_name + ".json"
+                )
+            ).read_text(encoding="utf-8")
         )
     )
     config["spk"] = spk_dict
     config["data"]["training_files"] = train_list_path.as_posix()
     config["data"]["validation_files"] = val_list_path.as_posix()
     LOG.info(f"Writing {config_path}")
     config_path.parent.mkdir(parents=True, exist_ok=True)
```

### Comparing `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py` & `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/preprocessing/preprocess_hubert_f0.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 from random import shuffle
 from typing import Iterable, Literal
 
 import librosa
 import numpy as np
 import torch
 import torchaudio
-from fairseq.models.hubert import HubertModel
 from joblib import Parallel, cpu_count, delayed
 from tqdm import tqdm
+from transformers import HubertModel
 
 import so_vits_svc_fork.f0
 from so_vits_svc_fork import utils
 
 from ..hparams import HParams
 from ..modules.mel_processing import spec_to_mel_torch, spectrogram_torch
 from ..utils import get_optimal_device, get_total_gpu_memory
@@ -99,15 +99,18 @@
     }
     data = {k: v.cpu() for k, v in data.items()}
     with data_path.open("wb") as f:
         torch.save(data, f)
 
 
 def _process_batch(filepaths: Iterable[Path], pbar_position: int, **kwargs):
-    content_model = utils.get_hubert_model(get_optimal_device())
+    hps = kwargs["hps"]
+    content_model = utils.get_hubert_model(
+        get_optimal_device(), hps.data.get("contentvec_final_proj", True)
+    )
 
     for filepath in tqdm(filepaths, position=pbar_position):
         _process_one(
             content_model=content_model,
             filepath=filepath,
             **kwargs,
         )
@@ -118,15 +121,14 @@
     config_path: Path | str,
     n_jobs: int | None = None,
     f0_method: Literal["crepe", "crepe-tiny", "parselmouth", "dio", "harvest"] = "dio",
     force_rebuild: bool = False,
 ):
     input_dir = Path(input_dir)
     config_path = Path(config_path)
-    utils.ensure_pretrained_model(".", "contentvec")
     hps = utils.get_hparams(config_path)
     if n_jobs is None:
         # add cpu_count() to avoid SIGKILL
         memory = get_total_gpu_memory("total")
         n_jobs = min(
             max(
                 memory
```

### Comparing `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/preprocessing/preprocess_resample.py` & `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/preprocessing/preprocess_resample.py`

 * *Files 3% similar despite different names*

```diff
@@ -99,17 +99,19 @@
     frame_seconds: float = 0.1,
     hop_seconds: float = 0.05,
 ) -> None:
     input_dir = Path(input_dir)
     output_dir = Path(output_dir)
     """Preprocess audio files in input_dir and save them to output_dir."""
 
-    in_paths = []
     out_paths = []
-    for in_path in input_dir.rglob("*.*"):
+    in_paths = list(input_dir.rglob("*.*"))
+    if not in_paths:
+        raise ValueError(f"No audio files found in {input_dir}")
+    for in_path in in_paths:
         in_path_relative = in_path.relative_to(input_dir)
         if not in_path.is_absolute() and is_relative_to(
             in_path, Path("dataset_raw") / "44k"
         ):
             new_in_path_relative = in_path_relative.relative_to("44k")
             warnings.warn(
                 f"Recommended folder structure has changed since v1.0.0. "
@@ -121,15 +123,14 @@
         if len(in_path_relative.parts) < 2:
             continue
         speaker_name = in_path_relative.parts[0]
         file_name = in_path_relative.with_suffix(".wav").name
         out_path = output_dir / speaker_name / file_name
         out_path = _get_unique_filename(out_path, out_paths)
         out_path.parent.mkdir(parents=True, exist_ok=True)
-        in_paths.append(in_path)
         out_paths.append(out_path)
 
     in_and_out_paths = list(zip(in_paths, out_paths))
 
     with tqdm_joblib(desc="Preprocessing", total=len(in_and_out_paths)):
         Parallel(n_jobs=n_jobs)(
             delayed(_preprocess_one)(
```

### Comparing `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py` & `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/preprocessing/preprocess_speaker_diarization.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/preprocessing/preprocess_split.py` & `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/preprocessing/preprocess_split.py`

 * *Files identical despite different names*

### Comparing `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/train.py` & `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/train.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 from __future__ import annotations
 
+import os
 import warnings
 from logging import getLogger
 from multiprocessing import cpu_count
 from pathlib import Path
 from typing import Any
 
 import lightning.pytorch as pl
 import torch
 from lightning.pytorch.accelerators import MPSAccelerator, TPUAccelerator
+from lightning.pytorch.callbacks import DeviceStatsMonitor
 from lightning.pytorch.loggers import TensorBoardLogger
+from lightning.pytorch.strategies.ddp import DDPStrategy
 from lightning.pytorch.tuner import Tuner
 from torch.cuda.amp import autocast
 from torch.nn import functional as F
 from torch.utils.data import DataLoader
 from torch.utils.tensorboard.writer import SummaryWriter
 
 import so_vits_svc_fork.f0
@@ -67,19 +70,34 @@
 def train(
     config_path: Path | str, model_path: Path | str, reset_optimizer: bool = False
 ):
     config_path = Path(config_path)
     model_path = Path(model_path)
 
     hparams = utils.get_backup_hparams(config_path, model_path)
-    utils.ensure_pretrained_model(model_path, hparams.model.get("type_", "hifi-gan"))
+    utils.ensure_pretrained_model(
+        model_path,
+        hparams.model.get(
+            "pretrained",
+            {
+                "D_0.pth": "https://huggingface.co/therealvul/so-vits-svc-4.0-init/resolve/main/D_0.pth",
+                "G_0.pth": "https://huggingface.co/therealvul/so-vits-svc-4.0-init/resolve/main/G_0.pth",
+            },
+        ),
+    )
 
     datamodule = VCDataModule(hparams)
     strategy = (
-        "ddp_find_unused_parameters_true" if torch.cuda.device_count() > 1 else "auto"
+        (
+            "ddp_find_unused_parameters_true"
+            if os.name != "nt"
+            else DDPStrategy(find_unused_parameters=True, process_group_backend="gloo")
+        )
+        if torch.cuda.device_count() > 1
+        else "auto"
     )
     LOG.info(f"Using strategy: {strategy}")
     trainer = pl.Trainer(
         logger=TensorBoardLogger(
             model_path, "lightning_logs", hparams.train.get("log_version", 0)
         ),
         # profiler="simple",
@@ -88,15 +106,16 @@
         check_val_every_n_epoch=None,
         precision="16-mixed"
         if hparams.train.fp16_run
         else "bf16-mixed"
         if hparams.train.get("bf16_run", False)
         else 32,
         strategy=strategy,
-        callbacks=[pl.callbacks.RichProgressBar()] if not is_notebook() else None,
+        callbacks=([pl.callbacks.RichProgressBar()] if not is_notebook() else [])
+        + [DeviceStatsMonitor()],
         benchmark=True,
         enable_checkpointing=False,
     )
     tuner = Tuner(trainer)
     model = VitsLightning(reset_optimizer=reset_optimizer, **hparams)
 
     # automatic batch size scaling
@@ -241,17 +260,61 @@
                     normalized,
                     onesided,
                     return_complex,
                 ).to(dtype)
 
             torch.stft = stft
 
+    def on_train_end(self) -> None:
+        self.save_checkpoints(adjust=0)
+
+    def save_checkpoints(self, adjust=1):
+        if self.tuning or self.trainer.sanity_checking:
+            return
+
+        # only save checkpoints if we are on the main device
+        if (
+            hasattr(self.device, "index")
+            and self.device.index != None
+            and self.device.index != 0
+        ):
+            return
+
+        # `on_train_end` will be the actual epoch, not a -1, so we have to call it with `adjust = 0`
+        current_epoch = self.current_epoch + adjust
+        total_batch_idx = self.total_batch_idx - 1 + adjust
+
+        utils.save_checkpoint(
+            self.net_g,
+            self.optim_g,
+            self.learning_rate,
+            current_epoch,
+            Path(self.hparams.model_dir)
+            / f"G_{total_batch_idx if self.hparams.train.get('ckpt_name_by_step', False) else current_epoch}.pth",
+        )
+        utils.save_checkpoint(
+            self.net_d,
+            self.optim_d,
+            self.learning_rate,
+            current_epoch,
+            Path(self.hparams.model_dir)
+            / f"D_{total_batch_idx if self.hparams.train.get('ckpt_name_by_step', False) else current_epoch}.pth",
+        )
+        keep_ckpts = self.hparams.train.get("keep_ckpts", 0)
+        if keep_ckpts > 0:
+            utils.clean_checkpoints(
+                path_to_models=self.hparams.model_dir,
+                n_ckpts_to_keep=keep_ckpts,
+                sort_by_time=True,
+            )
+
     def set_current_epoch(self, epoch: int):
         LOG.info(f"Setting current epoch to {epoch}")
         self.trainer.fit_loop.epoch_progress.current.completed = epoch
+        self.trainer.fit_loop.epoch_progress.current.processed = epoch
         assert self.current_epoch == epoch, f"{self.current_epoch} != {epoch}"
 
     def set_global_step(self, global_step: int):
         LOG.info(f"Setting global step to {global_step}")
         self.trainer.fit_loop.epoch_loop.manual_optimization.optim_step_progress.total.completed = (
             global_step
         )
@@ -499,32 +562,10 @@
                         y_hat_mel[0].cpu().float().numpy()
                     ),
                     "gt/mel": utils.plot_spectrogram_to_numpy(
                         mel[0].cpu().float().numpy()
                     ),
                 }
             )
-            if self.current_epoch == 0 or batch_idx != 0:
-                return
-            utils.save_checkpoint(
-                self.net_g,
-                self.optim_g,
-                self.learning_rate,
-                self.current_epoch + 1,  # prioritize prevention of undervaluation
-                Path(self.hparams.model_dir)
-                / f"G_{self.total_batch_idx if self.hparams.train.get('ckpt_name_by_step', False) else self.current_epoch + 1}.pth",
-            )
-            utils.save_checkpoint(
-                self.net_d,
-                self.optim_d,
-                self.learning_rate,
-                self.current_epoch + 1,
-                Path(self.hparams.model_dir)
-                / f"D_{self.total_batch_idx if self.hparams.train.get('ckpt_name_by_step', False) else self.current_epoch + 1}.pth",
-            )
-            keep_ckpts = self.hparams.train.get("keep_ckpts", 0)
-            if keep_ckpts > 0:
-                utils.clean_checkpoints(
-                    path_to_models=self.hparams.model_dir,
-                    n_ckpts_to_keep=keep_ckpts,
-                    sort_by_time=True,
-                )
+
+    def on_validation_end(self) -> None:
+        self.save_checkpoints()
```

### Comparing `so_vits_svc_fork-3.9.5/src/so_vits_svc_fork/utils.py` & `so_vits_svc_fork-4.0.0/src/so_vits_svc_fork/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 from __future__ import annotations
 
 import json
+import os
 import re
 import subprocess
+import warnings
 from itertools import groupby
 from logging import getLogger
 from pathlib import Path
 from typing import Any, Literal, Sequence
 
 import matplotlib
 import matplotlib.pylab as plt
 import numpy as np
 import requests
 import torch
 import torch.backends.mps
+import torch.nn as nn
+import torchaudio
 from cm_time import timer
-from fairseq import checkpoint_utils
-from fairseq.models.hubert.hubert import HubertModel
 from numpy import ndarray
 from tqdm import tqdm
+from transformers import HubertModel
 
 from so_vits_svc_fork.hparams import HParams
 
 LOG = getLogger(__name__)
 HUBERT_SAMPLING_RATE = 16000
+IS_COLAB = os.getenv("COLAB_RELEASE_TAG", False)
 
 
 def get_optimal_device(index: int = 0) -> torch.device:
     if torch.cuda.is_available():
         return torch.device(f"cuda:{index % torch.cuda.device_count()}")
     elif torch.backends.mps.is_available():
         return torch.device("mps")
@@ -105,17 +109,39 @@
         ],
     ],
 }
 from joblib import Parallel, delayed
 
 
 def ensure_pretrained_model(
-    folder_path: Path | str, type_: str, **tqdm_kwargs: Any
+    folder_path: Path | str, type_: str | dict[str, str], **tqdm_kwargs: Any
 ) -> tuple[Path, ...] | None:
     folder_path = Path(folder_path)
+
+    # new code
+    if not isinstance(type_, str):
+        try:
+            Parallel(n_jobs=len(type_))(
+                [
+                    delayed(download_file)(
+                        url,
+                        folder_path / filename,
+                        position=i,
+                        skip_if_exists=True,
+                        **tqdm_kwargs,
+                    )
+                    for i, (filename, url) in enumerate(type_.items())
+                ]
+            )
+            return tuple(folder_path / filename for filename in type_.values())
+        except Exception as e:
+            LOG.error(f"Failed to download {type_}")
+            LOG.exception(e)
+
+    # old code
     models_candidates = PRETRAINED_MODEL_URLS.get(type_, None)
     if models_candidates is None:
         LOG.warning(f"Unknown pretrained model type: {type_}")
         return
     for model_urls in models_candidates:
         paths = [folder_path / model_url.split("/")[-1] for model_url in model_urls]
         try:
@@ -125,32 +151,37 @@
                         url, path, position=i, skip_if_exists=True, **tqdm_kwargs
                     )
                     for i, (url, path) in enumerate(zip(model_urls, paths))
                 ]
             )
             return tuple(paths)
         except Exception as e:
+            LOG.error(f"Failed to download {model_urls}")
             LOG.exception(e)
-    return
-
-
-def get_hubert_model(device: str | torch.device) -> HubertModel:
-    (path,) = ensure_pretrained_model(Path("."), "contentvec")
-
-    models, saved_cfg, task = checkpoint_utils.load_model_ensemble_and_task(
-        [path.as_posix()],
-        suffix="",
-    )
-    model = models[0]
-    return model.eval().to(device)
 
 
-import warnings
-
-import torchaudio
+class HubertModelWithFinalProj(HubertModel):
+    def __init__(self, config):
+        super().__init__(config)
+
+        # The final projection layer is only used for backward compatibility.
+        # Following https://github.com/auspicious3000/contentvec/issues/6
+        # Remove this layer is necessary to achieve the desired outcome.
+        self.final_proj = nn.Linear(config.hidden_size, config.classifier_proj_size)
+
+
+def get_hubert_model(
+    device: str | torch.device, final_proj: bool = True
+) -> HubertModel:
+    if final_proj:
+        return HubertModelWithFinalProj.from_pretrained(
+            "lengyue233/content-vec-best"
+        ).to(device)
+    else:
+        return HubertModel.from_pretrained("lengyue233/content-vec-best").to(device)
 
 
 def get_content(
     cmodel: HubertModel,
     audio: torch.Tensor | ndarray[Any, Any],
     device: torch.device | str,
     sr: int,
@@ -162,21 +193,22 @@
             torchaudio.transforms.Resample(sr, HUBERT_SAMPLING_RATE)
             .to(audio.device)(audio)
             .to(device)
         )
     if audio.ndim == 1:
         audio = audio.unsqueeze(0)
     with torch.no_grad(), timer() as t:
-        params = {"output_layer": 9} if legacy_final_proj else {}
-        c: torch.Tensor = cmodel.extract_features(audio, **params)[0]
         if legacy_final_proj:
             warnings.warn("legacy_final_proj is deprecated")
-            assert hasattr(cmodel, "final_proj")
-            assert isinstance(cmodel.final_proj, torch.nn.Module)
+            if not hasattr(cmodel, "final_proj"):
+                raise ValueError("HubertModel does not have final_proj")
+            c = cmodel(audio, output_hidden_states=True)["hidden_states"][9]
             c = cmodel.final_proj(c)
+        else:
+            c = cmodel(audio)["last_hidden_state"]
         c = c.transpose(1, 2)
     wav_len = audio.shape[-1] / HUBERT_SAMPLING_RATE
     LOG.info(
         f"HuBERT inference time  : {t.elapsed:.3f}s, RTF: {t.elapsed / wav_len:.3f}"
     )
     return c
 
@@ -244,27 +276,27 @@
         and not skip_optimizer
         and checkpoint_dict["optimizer"] is not None
     ):
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
             safe_load(optimizer, checkpoint_dict["optimizer"])
 
-    LOG.info(f"Loaded checkpoint '{checkpoint_path}' (iteration {iteration})")
+    LOG.info(f"Loaded checkpoint '{checkpoint_path}' (epoch {iteration})")
     return model, optimizer, learning_rate, iteration
 
 
 def save_checkpoint(
     model: torch.nn.Module,
     optimizer: torch.optim.Optimizer,
     learning_rate: float,
     iteration: int,
     checkpoint_path: Path | str,
 ) -> None:
     LOG.info(
-        "Saving model and optimizer state at iteration {} to {}".format(
+        "Saving model and optimizer state at epoch {} to {}".format(
             iteration, checkpoint_path
         )
     )
     if hasattr(model, "module"):
         state_dict = model.module.state_dict()
     else:
         state_dict = model.state_dict()
@@ -314,16 +346,19 @@
 
     models_sorted_grouped = groupby(models_sorted, lambda p: p.stem[0])
 
     for group_name, group_items in models_sorted_grouped:
         to_delete_list = list(group_items)[:-n_ckpts_to_keep]
 
         for to_delete in to_delete_list:
-            LOG.info(f"Removing {to_delete}")
-            to_delete.unlink()
+            if to_delete.exists():
+                LOG.info(f"Removing {to_delete}")
+                if IS_COLAB:
+                    to_delete.write_text("")
+                to_delete.unlink()
 
 
 def latest_checkpoint_path(dir_path: Path | str, regex: str = "G_*.pth") -> Path | None:
     dir_path = Path(dir_path)
     name_key = lambda p: int(re.match(r"._(\d+)\.pth", p.name).group(1))
     paths = list(sorted(dir_path.glob(regex), key=name_key))
     if len(paths) == 0:
@@ -364,15 +399,15 @@
 
     hparams = HParams(**config)
     hparams.model_dir = model_path.as_posix()
     return hparams
 
 
 def get_hparams(config_path: Path | str) -> HParams:
-    config = json.loads(Path(config_path).read_text())
+    config = json.loads(Path(config_path).read_text("utf-8"))
     hparams = HParams(**config)
     return hparams
 
 
 def repeat_expand_2d(content: torch.Tensor, target_len: int) -> torch.Tensor:
     # content : [h, t]
     src_len = content.shape[-1]
```

