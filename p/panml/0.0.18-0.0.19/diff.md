# Comparing `tmp/panml-0.0.18.tar.gz` & `tmp/panml-0.0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panml-0.0.18.tar", last modified: Thu May 25 13:23:39 2023, max compression
+gzip compressed data, was "panml-0.0.19.tar", last modified: Sun May 28 12:47:54 2023, max compression
```

## Comparing `panml-0.0.18.tar` & `panml-0.0.19.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-25 13:23:39.393388 panml-0.0.18/
--rw-r--r--   0 williamzheng   (501) staff       (20)     1063 2023-05-11 06:11:04.000000 panml-0.0.18/LICENSE
--rw-r--r--   0 williamzheng   (501) staff       (20)    10152 2023-05-25 13:23:39.393746 panml-0.0.18/PKG-INFO
--rw-r--r--   0 williamzheng   (501) staff       (20)     8973 2023-05-25 13:23:02.000000 panml-0.0.18/README.md
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-25 13:23:39.383383 panml-0.0.18/panml/
--rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-19 12:08:24.000000 panml-0.0.18/panml/__init__.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-25 13:23:39.386941 panml-0.0.18/panml/core/
--rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-21 05:11:31.000000 panml-0.0.18/panml/core/__init__.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-25 13:23:39.387976 panml-0.0.18/panml/core/clustering/
--rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-21 05:11:31.000000 panml-0.0.18/panml/core/clustering/__init__.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     9033 2023-05-24 12:19:14.000000 panml-0.0.18/panml/core/clustering/faiss.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-25 13:23:39.390745 panml-0.0.18/panml/core/llm/
--rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-21 05:11:31.000000 panml-0.0.18/panml/core/llm/__init__.py
--rw-r--r--   0 williamzheng   (501) staff       (20)    19715 2023-05-25 13:23:02.000000 panml-0.0.18/panml/core/llm/huggingface.py
--rw-r--r--   0 williamzheng   (501) staff       (20)    13050 2023-05-25 13:23:02.000000 panml-0.0.18/panml/core/llm/openai.py
--rw-r--r--   0 williamzheng   (501) staff       (20)      537 2023-05-24 12:19:14.000000 panml-0.0.18/panml/core/llm/prompt_template.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     4764 2023-05-24 12:19:14.000000 panml-0.0.18/panml/models.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     3343 2023-05-24 12:19:14.000000 panml-0.0.18/panml/search.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-25 13:23:39.386227 panml-0.0.18/panml.egg-info/
--rw-r--r--   0 williamzheng   (501) staff       (20)    10152 2023-05-25 13:23:39.000000 panml-0.0.18/panml.egg-info/PKG-INFO
--rw-r--r--   0 williamzheng   (501) staff       (20)      483 2023-05-25 13:23:39.000000 panml-0.0.18/panml.egg-info/SOURCES.txt
--rw-r--r--   0 williamzheng   (501) staff       (20)        1 2023-05-25 13:23:39.000000 panml-0.0.18/panml.egg-info/dependency_links.txt
--rw-r--r--   0 williamzheng   (501) staff       (20)      215 2023-05-25 13:23:39.000000 panml-0.0.18/panml.egg-info/requires.txt
--rw-r--r--   0 williamzheng   (501) staff       (20)        6 2023-05-25 13:23:39.000000 panml-0.0.18/panml.egg-info/top_level.txt
--rw-r--r--   0 williamzheng   (501) staff       (20)       79 2023-05-25 13:23:39.394930 panml-0.0.18/setup.cfg
--rw-r--r--   0 williamzheng   (501) staff       (20)     2368 2023-05-25 13:23:02.000000 panml-0.0.18/setup.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-25 13:23:39.392275 panml-0.0.18/test/
--rw-r--r--   0 williamzheng   (501) staff       (20)     4383 2023-05-25 13:23:02.000000 panml-0.0.18/test/test_ModelPack.py
--rw-r--r--   0 williamzheng   (501) staff       (20)    11162 2023-05-22 09:48:53.000000 panml-0.0.18/test/test_VectorEngine.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-28 12:47:54.801039 panml-0.0.19/
+-rw-r--r--   0 williamzheng   (501) staff       (20)     1063 2023-05-11 06:11:04.000000 panml-0.0.19/LICENSE
+-rw-r--r--   0 williamzheng   (501) staff       (20)    10152 2023-05-28 12:47:54.801367 panml-0.0.19/PKG-INFO
+-rw-r--r--   0 williamzheng   (501) staff       (20)     8973 2023-05-25 13:23:02.000000 panml-0.0.19/README.md
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-28 12:47:54.794964 panml-0.0.19/panml/
+-rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-19 12:08:24.000000 panml-0.0.19/panml/__init__.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     3485 2023-05-28 12:46:27.000000 panml-0.0.19/panml/constants.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-28 12:47:54.797237 panml-0.0.19/panml/core/
+-rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-21 05:11:31.000000 panml-0.0.19/panml/core/__init__.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-28 12:47:54.797989 panml-0.0.19/panml/core/clustering/
+-rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-21 05:11:31.000000 panml-0.0.19/panml/core/clustering/__init__.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     9033 2023-05-24 12:19:14.000000 panml-0.0.19/panml/core/clustering/faiss.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-28 12:47:54.799497 panml-0.0.19/panml/core/llm/
+-rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-21 05:11:31.000000 panml-0.0.19/panml/core/llm/__init__.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)    20241 2023-05-28 12:46:27.000000 panml-0.0.19/panml/core/llm/huggingface.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)    13708 2023-05-28 12:46:27.000000 panml-0.0.19/panml/core/llm/openai.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     3085 2023-05-28 12:46:27.000000 panml-0.0.19/panml/models.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     2608 2023-05-28 12:46:27.000000 panml-0.0.19/panml/search.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-28 12:47:54.796881 panml-0.0.19/panml.egg-info/
+-rw-r--r--   0 williamzheng   (501) staff       (20)    10152 2023-05-28 12:47:54.000000 panml-0.0.19/panml.egg-info/PKG-INFO
+-rw-r--r--   0 williamzheng   (501) staff       (20)      468 2023-05-28 12:47:54.000000 panml-0.0.19/panml.egg-info/SOURCES.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)        1 2023-05-28 12:47:54.000000 panml-0.0.19/panml.egg-info/dependency_links.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)      215 2023-05-28 12:47:54.000000 panml-0.0.19/panml.egg-info/requires.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)        6 2023-05-28 12:47:54.000000 panml-0.0.19/panml.egg-info/top_level.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)       79 2023-05-28 12:47:54.803700 panml-0.0.19/setup.cfg
+-rw-r--r--   0 williamzheng   (501) staff       (20)     2384 2023-05-28 12:46:27.000000 panml-0.0.19/setup.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-28 12:47:54.800532 panml-0.0.19/test/
+-rw-r--r--   0 williamzheng   (501) staff       (20)     4383 2023-05-25 13:23:02.000000 panml-0.0.19/test/test_ModelPack.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)    11162 2023-05-22 09:48:53.000000 panml-0.0.19/test/test_VectorEngine.py
```

### Comparing `panml-0.0.18/LICENSE` & `panml-0.0.19/LICENSE`

 * *Files identical despite different names*

### Comparing `panml-0.0.18/PKG-INFO` & `panml-0.0.19/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panml
-Version: 0.0.18
+Version: 0.0.19
 Summary: PanML is a high level generative AI/ML development library designed for ease of use and fast experimentation.
 Home-page: https://github.com/Pan-ML/panml
 Author: PanML team
 Author-email: teampanml@gmail.com
 License: MIT
 Keywords: generative AI,generative model,machine learning,large language model,LLM,prompt engineering,fine tuning,prompt tuning,retrieval augmentation,AI safety,AI alignment
 Platform: UNKNOWN
```

### Comparing `panml-0.0.18/README.md` & `panml-0.0.19/README.md`

 * *Files identical despite different names*

### Comparing `panml-0.0.18/panml/core/clustering/faiss.py` & `panml-0.0.19/panml/core/clustering/faiss.py`

 * *Files identical despite different names*

### Comparing `panml-0.0.18/panml/core/llm/huggingface.py` & `panml-0.0.19/panml/core/llm/huggingface.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 import pandas as pd
 import torch
-from typing import Union
+from typing import Union, Callable
 from transformers import AutoModelForCausalLM, AutoModelForSeq2SeqLM, AutoModelForMaskedLM, AutoTokenizer
 from transformers import TrainingArguments, Trainer, Seq2SeqTrainingArguments, Seq2SeqTrainer, DataCollatorForLanguageModeling, DataCollatorForSeq2Seq
 from datasets import Dataset
 
 # HuggingFace model class
 class HuggingFaceModelPack:
     '''
@@ -60,14 +60,18 @@
         if self.model_hf.config.tokenizer_class:
             self.tokenizer = AutoTokenizer.from_pretrained(self.model_hf.config.tokenizer_class.lower().replace('tokenizer', ''), mirror='https://huggingface.co')
         else:
             self.tokenizer = AutoTokenizer.from_pretrained(self.model_name, mirror='https://huggingface.co')
 
         # Set model on GPU if available and specified
         self.model_hf.to(torch.device(self.device))
+        
+    # Set initial prompt
+    def _init_prompt(self) -> list[dict[str, Union[str, Callable]]]:
+        return [{'prepend': '', 'append': '', 'transform': None}]
 
     # Embed text
     def embedding(self, text: str) -> torch.Tensor:
         '''
         Gets the embedding of the text using open source collections of models from HuggingFace Hub
 
         Args:
@@ -143,15 +147,15 @@
 
         return output_context
     
     # Generate text
     def predict(self, text: Union[str, list[str], pd.Series], max_length: int=50, skip_special_tokens: bool=True, 
                 display_probability: bool=False, num_return_sequences: int=1, temperature: float=0.8, 
                 top_p: float=0.8, top_k: int=0, no_repeat_ngram_size: int=3, 
-                prompt_modifier: list[dict[str, str]]=[{'prepend': '', 'append': ''}], keep_history: bool=False) -> dict[str, str]:
+                prompt_modifier: list[dict[str, Union[str, Callable]]]=None, keep_history: bool=False) -> Union[dict[str, str], list[str]]:
         '''
         Generates output by prompting a language model from HuggingFace Hub
 
         Args:
         text: text of the prompt, can be a string, list, or pandas.series
         max_length: parameter from HuggingFace Hub, specifies the max length of tokens generated
         skip_special_tokens: parameter from HuggingFace Hub, specifies whether or not to remove special tokens in the decoding
@@ -161,31 +165,35 @@
         top_p: parameter from HuggingFace Hub, if set to float < 1, only the smallest set of most probable tokens with probabilities that add up to top_p or higher are kept for generation
         no_repeat_ngram_size: parameter from HuggingFace Hub, ff set to int > 0, all ngrams of that size can only occur once
 
         Returns: 
         prediction: list, or list of dict containing generated text with probabilities and perplexity if specified and available
         '''
         input_context = None
-        
+        self.prediction_history = []
+
         # Catch input exceptions
         if not isinstance(text, str) and not isinstance(text, list) and not isinstance(text, pd.Series):
             raise TypeError('Input text needs to be of type: string, list or pandas.series')
         if isinstance(text, pd.Series): # convert to list from pandas series if available
             input_context = text.tolist()
             if len(input_context) == 0:
                 raise ValueError('Input text list cannot be empty')
         if isinstance(text, str): # wrap input text into list if available
             if len(text) == 0:
                 raise ValueError('Input text cannot be empty')
             input_context = [text]
         if isinstance(text, list):
             if len(text) == 0:
                 raise ValueError('Input text list cannot be empty')
-        if not isinstance(prompt_modifier, list):
-            raise TypeError('Input prompt modifier needs to be of type: list')
+        if prompt_modifier is None:
+            prompt_modifier = self._init_prompt()
+        else:
+            if not isinstance(prompt_modifier, list):
+                raise TypeError('Input prompt modifier needs to be of type: list')
         
         # Run prediction on text samples
         prediction = []
         for context in input_context:
             # Create loop for text prediction
             history = []
             for count, mod in enumerate(prompt_modifier):
@@ -194,15 +202,18 @@
                     mod['prepend'] = ''
                 if 'append' not in mod:
                     mod['append'] = ''
 
                 # Set the query text to previous output to carry on the prompt loop
                 if count > 0:
                     context = output_context['text']
-                context = f"{mod['prepend']} \n {context} \n {mod['append']}"
+                if mod['transform'] is not None and callable(mod['transform']):
+                    context = f"{mod['prepend']}\n{mod['transform'](context)}\n{mod['append']}"
+                else:
+                    context = f"{mod['prepend']}\n{context}\n{mod['append']}"
 
                 # Call model for text generation
                 output_context = self._predict(context, max_length=max_length, skip_special_tokens=skip_special_tokens,
                                                display_probability=display_probability, num_return_sequences=num_return_sequences, 
                                                temperature=temperature, top_p=top_p, top_k=top_k, no_repeat_ngram_size=no_repeat_ngram_size)
 
                 # Terminate loop for next prompt when context contains no meaningful words (less than 2)
@@ -213,16 +224,16 @@
                 if len(output_context['text'].replace(' ', '')) < 2:
                     break
 
                 history.append(output_context)
             
             try:
                 if keep_history:
-                    prediction.append(history[-1]) # get last prediction output
-                    self.prediction_history.append(history) # get all historical prediction output
+                    prediction.append(history[-1]) # saves last prediction output
+                    self.prediction_history.append(history) # saves all historical prediction output
                 else:
                     prediction.append(history[-1])
             except:
                 prediction.append({'text': None}) # if there is invalid response from the language model, return None
                 
         # Gather output
         if isinstance(text, str):
```

### Comparing `panml-0.0.18/panml/core/llm/openai.py` & `panml-0.0.19/panml/core/llm/openai.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 from __future__ import annotations
 import pandas as pd
 import torch
-from typing import Union
+from typing import Union, Callable
 import openai
+from panml.constants import SUPPORTED_OAI_CODE_MODELS, SUPPORTED_OAI_COMPLETION_MODELS, SUPPORTED_OAI_CHAT_MODELS
 
 # OpenAI model class
 class OpenAIModelPack:
     '''
     OpenAI model pack class
     '''
     def __init__(self, model: str, api_key: str) -> None:
         self.model_name = model
         self.model_embedding = 'text-embedding-ada-002'
-        self.prediction_history = []
+        self.prediction_history = None
+        self.supported_code_models = SUPPORTED_OAI_CODE_MODELS
+        self.completion_models = SUPPORTED_OAI_COMPLETION_MODELS
+        self.chat_completion_models = SUPPORTED_OAI_CHAT_MODELS
         openai.api_key = api_key
+        
+    def _init_prompt(self) -> list[dict[str, Union[str, Callable]]]:
+        return [{'prepend': '', 'append': '', 'transform': None}]
     
     # Generate text of single model call
     def _predict(self, text: str, temperature: float, max_tokens: int, top_p: float, n: int, 
                  frequency_penalty: float, presence_penalty: float, display_probability: bool, logprobs: int, 
                  chat_role: str) -> dict[str, str]:
         '''
         Base function for text generation using OpenAI models
@@ -31,37 +38,30 @@
         probability: token probabilities if available
         perplexity: perplexity score if available
         Note: probability and peplexity scores are calculated only for some OpenAI models in this package
         '''
         output_context = {
             'text': None
         }
-        completion_models = [
-            'text-davinci-002', 
-            'text-davinci-003',
-        ]
-        chat_completion_models = [
-            'gpt-3.5-turbo',
-            'gpt-3.5-turbo-0301',
-        ]
-        if self.model_name in completion_models:
+        
+        if self.model_name in self.completion_models:
             response = openai.Completion.create(
                 model=self.model_name,
                 prompt=text,
                 temperature=temperature,
                 max_tokens=max_tokens,
                 top_p=top_p,
                 n=n,
                 frequency_penalty=frequency_penalty,
                 presence_penalty=presence_penalty,
                 logprobs=logprobs
             )
             output_context['text'] = response['choices'][0]['text']
             
-        elif self.model_name in chat_completion_models:
+        elif self.model_name in self.chat_completion_models:
             response = openai.ChatCompletion.create(
                 model=self.model_name,
                 messages = [
                     {'role': chat_role, 'content': text}
                 ],
                 temperature=temperature,
                 max_tokens=max_tokens,
@@ -71,50 +71,51 @@
                 presence_penalty=presence_penalty,
             )
             output_context['text'] = response['choices'][0]['message']['content']
         else:
             raise ValueError(f'{self.model_name} is not currently supported in this package')
 
         # Get probability of output tokens
-        if display_probability and self.model_name in completion_models:
+        if display_probability and self.model_name in self.completion_models:
             tokens = response["choices"][0]['logprobs']['tokens']
             token_logprobs = response["choices"][0]['logprobs']['token_logprobs']
             output_context['probability'] = [{'token': token, 'probability': torch.exp(torch.Tensor([logprob])).item()} for token, logprob in zip(tokens, token_logprobs)]
 
             # Calculate perplexity of output
             output_context['perplexity'] = (1/torch.prod(torch.tensor([torch.exp(torch.Tensor([logprob])).item() for logprob in token_logprobs])).item())**(1/len(tokens))
 
         return output_context
     
     # Generate text in prompt loop
-    def predict(self, text: Union[str, list[str], pd.Series], temperature: float=0, max_tokens: int=100, top_p: float=1, n: int=3, 
+    def predict(self, text: Union[str, list[str], pd.Series], temperature: float=0, max_length: int=100, top_p: float=1, n: int=3, 
                 frequency_penalty: float=0, presence_penalty: float=0, display_probability: bool=False, logprobs: int=1, 
-                prompt_modifier: list[dict[str, str]]=[{'prepend': '', 'append': ''}], keep_history: bool=False, 
-                chat_role: str='user') -> dict[str, str]:
+                prompt_modifier: list[dict[str, str]]=None, keep_history: bool=False, 
+                chat_role: str='user') -> Union[dict[str, str], list[str]]:
         '''
         Generates output by prompting a language model from OpenAI
         
         Args:
         text: text of the prompt, can be a string, list, or pandas.series
         temperature: temperature of the generated text (for further details please refer to this topic covered in language model text generation)
-        max_tokens: max number of tokens to be generated from OpenAI API
+        max_length: max number of tokens to be generated from OpenAI API
         top_p: max number of tokens to be generated from OpenAI API
         n: parameter from OpenAI API (for further details please refer to this topic covered in language model text generation)
         frequency_penalty: parameter from OpenAI API (for further details please refer to this topic covered in language model text generation)
         presence_penalty: parameter from OpenAI API (for further details please refer to this topic covered in language model text generation)
         display_probability: show probability of the generated tokens
         logprobs: parameter from OpenAI API (for further details please refer to this topic covered in language model text generation)
         prompt_modifier: list of prompts to be added in the context of multi-stage prompt chaining
         keep_history: keep or discard the history of responses from the mulit-stage prompt chaining
         chat_role: parameter from OpenAI API, specifies the role of the LLM assistant. Currently this is available for models of gpt-3.5-turbo or above (for further details please refer to this topic covered in language model text generation)
 
         Returns: 
         prediction: list, or list of dict containing generated text with probabilities and perplexity if specified and available
         '''
         input_context = None
+        self.prediction_history = []
 
         # Catch input exceptions
         if not isinstance(text, str) and not isinstance(text, list) and not isinstance(text, pd.Series):
             raise TypeError('Input text needs to be of type: string, list or pandas.series')
         if isinstance(text, pd.Series): # convert to list from pandas series if available
             input_context = text.tolist()
             if len(input_context) == 0:
@@ -122,38 +123,46 @@
         if isinstance(text, str): # wrap input text into list if available
             if len(text) == 0:
                 raise ValueError('Input text cannot be empty')
             input_context = [text]
         if isinstance(text, list):
             if len(text) == 0:
                 raise ValueError('Input text list cannot be empty')
-        if not isinstance(prompt_modifier, list):
-            raise TypeError('Input prompt modifier needs to be of type: list')
+        if prompt_modifier is None:
+            prompt_modifier = self._init_prompt()
+        else:
+            if not isinstance(prompt_modifier, list):
+                raise TypeError('Input prompt modifier needs to be of type: list')
         if not isinstance(chat_role, str):
             raise TypeError('Input chat role needs to be of type: string')
             
         # Run prediction on text samples
         prediction = []
         for context in input_context:
             # Create loop for text prediction
             history = []
             for count, mod in enumerate(prompt_modifier):
                 # Set prepend or append to empty str if there is no input for these
                 if 'prepend' not in mod: 
                     mod['prepend'] = ''
                 if 'append' not in mod:
                     mod['append'] = ''
+                if 'transform' not in mod:
+                    mod['transform'] = None
 
                 # Set the query text to previous output to carry on the prompt loop
                 if count > 0:
                     context = output_context['text']
-                context = f"{mod['prepend']} \n {context} \n {mod['append']}"
+                if mod['transform'] is not None and callable(mod['transform']):
+                    context = f"{mod['prepend']}\n{mod['transform'](context)}\n{mod['append']}"
+                else:
+                    context = f"{mod['prepend']}\n{context}\n{mod['append']}"
 
                 # Call model for text generation
-                output_context = self._predict(context, temperature=temperature, max_tokens=max_tokens, top_p=top_p,
+                output_context = self._predict(context, temperature=temperature, max_tokens=max_length, top_p=top_p,
                                                n=n, frequency_penalty=frequency_penalty, presence_penalty=presence_penalty,
                                                display_probability=display_probability, logprobs=logprobs, chat_role=chat_role)
 
                 # Terminate loop for next prompt when context contains no meaningful words (less than 2)
                 output_context['text'] = output_context['text'].replace('\n', ' ').replace('\xa0', '').replace('  ', ' ')
                 output_context['text'] = output_context['text'].replace(',', ', ')
                 output_context['text'] = output_context['text'].replace('.', '. ')
@@ -161,16 +170,16 @@
                 if len(output_context['text'].replace(' ', '')) < 2:
                     break
 
                 history.append(output_context)
             
             try:
                 if keep_history:
-                    prediction.append(history[-1]) # returns last prediction output
-                    self.prediction_history.append(history) # returns all historical prediction output
+                    prediction.append(history[-1]) # saves last prediction output
+                    self.prediction_history.append(history) # saves all historical prediction output
                 else:
                     prediction.append(history[-1])
             except:
                 prediction.append({'text': None}) # if there is invalid response from the language model, return None
 
         # Gather output
         if isinstance(text, str):
@@ -194,16 +203,16 @@
         langauge: programming language of the code to be generated
         max_tokens: max number of tokens to be generated from OpenAI API
    
         Returns: 
         text of generated code
         '''
         # Catch input exceptions
-        if self.model_name != 'text-davinci-002' and self.model_name != 'text-davinci-003':
-            raise ValueError(f"The specified model is '{self.model_name}'. Only 'text-davinci-002' and 'text-davinci-002' are supported in this package for code generation")
+        if self.model_name not in self.supported_code_models:
+            raise ValueError(f"The specified model is '{self.model_name}'. Only {', '.join(self.supported_code_models)} are supported in this package for code generation")
         if not isinstance(text, str):
             raise TypeError('Input text needs to be of type: string')
         if not isinstance(x, int) and not isinstance(x, float) and \
             not isinstance(x, str) and not isinstance(x, pd.DataFrame):
             raise TypeError('Input x needs to be of type: int, float, str or pandas dataframe')
         if not isinstance(variable_names, dict):
             raise TypeError('Input variable names needs to be of type: dict')
```

### Comparing `panml-0.0.18/panml/search.py` & `panml-0.0.19/panml/search.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,53 +3,28 @@
 # Dependencies for data processing and general machine learning implementations
 import torch
 import torch.nn.functional as F
 from typing import Union
 
 # Dependencies for vector search
 from panml.core.clustering.faiss import FAISSVectorEngine
+from panml.constants import SUPPORTED_VECTOR_SEARCH_SOURCES, SUPPORTED_EMBEDDING_MODELS
 
 # Entry vector engine class           
 class VectorEngine:
     '''
     Main vector engine class
     '''
     def __init__(self, model: str='all-MiniLM-L6-v2', source: str='faiss', api_key: str=None) -> None:
         self.source = source
         self.model = model
         self.api_key = api_key
         self.model_emb_source = None
-
-        # Accepted vectors search from sources
-        self.supported_vector_search = [
-            'faiss', 
-            'pinecone',
-        ]
-        self.supported_embedding_models = {
-            'huggingface': [
-                'all-MiniLM-L6-v2',
-                'all-mpnet-base-v2',
-                'all-distilroberta-v1'
-                'nq-distilbert-base-v1',
-                'paraphrase-albert-small-v2',
-                'paraphrase-MiniLM-L3-v2',
-                'paraphrase-MiniLM-L6-v2',
-                'multi-qa-MiniLM-L6-cos-v1',
-                'multi-qa-distilbert-cos-v1',
-                'msmarco-MiniLM-L6-cos-v5',
-                'distiluse-base-multilingual-cased-v1',
-                'distiluse-base-multilingual-cased-v2',
-                'paraphrase-multilingual-MiniLM-L12-v2',
-                'paraphrase-multilingual-mpnet-base-v2',
-                'distilbert-base-nli-stsb-mean-tokens',
-            ],
-            'openai': [
-                'text-embedding-ada-002', 
-            ],
-        }
+        self.supported_vector_search = SUPPORTED_VECTOR_SEARCH_SOURCES # supported vectors search sources
+        self.supported_embedding_models = SUPPORTED_EMBEDDING_MODELS # supported embedding models
         
         # General exceptions handling on user input
         if self.source not in self.supported_vector_search:
             raise ValueError('The specified vector search implementation is currently not supported in this package. Supported vector search implementations are: ' + ', '.join([f"{m}" for m in self.supported_vector_search]))
         if self.model not in self.supported_embedding_models['huggingface'] and \
             self.model not in self.supported_embedding_models['openai']:
             raise ValueError('The specified embedding model is currently not supported in this package. Supported embedding models for vector search are: ' + '\n' + str(self.supported_embedding_models))
```

### Comparing `panml-0.0.18/panml.egg-info/PKG-INFO` & `panml-0.0.19/panml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panml
-Version: 0.0.18
+Version: 0.0.19
 Summary: PanML is a high level generative AI/ML development library designed for ease of use and fast experimentation.
 Home-page: https://github.com/Pan-ML/panml
 Author: PanML team
 Author-email: teampanml@gmail.com
 License: MIT
 Keywords: generative AI,generative model,machine learning,large language model,LLM,prompt engineering,fine tuning,prompt tuning,retrieval augmentation,AI safety,AI alignment
 Platform: UNKNOWN
```

### Comparing `panml-0.0.18/setup.py` & `panml-0.0.19/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
-long_description = (this_directory / "README.md").read_text()
+long_description = (this_directory / "README.md").read_text(encoding="utf-8")
 
 setup(
   name = 'panml', # package name     
   packages = find_packages(exclude=['test']), # package name
-  version = '0.0.18', # version
+  version = '0.0.19', # version
   license = 'MIT', # license
   description = 'PanML is a high level generative AI/ML development library designed for ease of use and fast experimentation.', # short description about the package
   long_description=long_description,
   long_description_content_type='text/markdown',
   author = 'PanML team', # team name
   author_email = 'teampanml@gmail.com', # contact email
   url = 'https://github.com/Pan-ML/panml', # url link
```

### Comparing `panml-0.0.18/test/test_ModelPack.py` & `panml-0.0.19/test/test_ModelPack.py`

 * *Files identical despite different names*

### Comparing `panml-0.0.18/test/test_VectorEngine.py` & `panml-0.0.19/test/test_VectorEngine.py`

 * *Files identical despite different names*

