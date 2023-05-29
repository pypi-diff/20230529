# Comparing `tmp/tree-of-thoughts-0.2.6.tar.gz` & `tmp/tree-of-thoughts-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tree-of-thoughts-0.2.6.tar", last modified: Sun May 28 03:58:43 2023, max compression
+gzip compressed data, was "tree-of-thoughts-0.2.7.tar", last modified: Mon May 29 14:50:24 2023, max compression
```

## Comparing `tree-of-thoughts-0.2.6.tar` & `tree-of-thoughts-0.2.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 03:58:42.998712 tree-of-thoughts-0.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-28 03:58:32.000000 tree-of-thoughts-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-28 03:58:42.998712 tree-of-thoughts-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15204 2023-05-28 03:58:32.000000 tree-of-thoughts-0.2.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 03:58:42.998712 tree-of-thoughts-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-28 03:58:32.000000 tree-of-thoughts-0.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 03:58:42.994712 tree-of-thoughts-0.2.6/tree_of_thoughts/
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-28 03:58:32.000000 tree-of-thoughts-0.2.6/tree_of_thoughts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-28 03:58:32.000000 tree-of-thoughts-0.2.6/tree_of_thoughts/abstractLanguageModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-05-28 03:58:32.000000 tree-of-thoughts-0.2.6/tree_of_thoughts/guidanceModels.py
--rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-05-28 03:58:32.000000 tree-of-thoughts-0.2.6/tree_of_thoughts/huggingModels.py
--rw-r--r--   0 runner    (1001) docker     (123)     9181 2023-05-28 03:58:32.000000 tree-of-thoughts-0.2.6/tree_of_thoughts/openaiModels.py
--rw-r--r--   0 runner    (1001) docker     (123)    11105 2023-05-28 03:58:32.000000 tree-of-thoughts-0.2.6/tree_of_thoughts/treeofthoughts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 03:58:42.998712 tree-of-thoughts-0.2.6/tree_of_thoughts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-28 03:58:42.000000 tree-of-thoughts-0.2.6/tree_of_thoughts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-28 03:58:42.000000 tree-of-thoughts-0.2.6/tree_of_thoughts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 03:58:42.000000 tree-of-thoughts-0.2.6/tree_of_thoughts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-28 03:58:42.000000 tree-of-thoughts-0.2.6/tree_of_thoughts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-28 03:58:42.000000 tree-of-thoughts-0.2.6/tree_of_thoughts.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:50:24.092428 tree-of-thoughts-0.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-29 14:50:08.000000 tree-of-thoughts-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-29 14:50:24.092428 tree-of-thoughts-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13962 2023-05-29 14:50:08.000000 tree-of-thoughts-0.2.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 14:50:24.092428 tree-of-thoughts-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-29 14:50:08.000000 tree-of-thoughts-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:50:24.092428 tree-of-thoughts-0.2.7/tree_of_thoughts/
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-29 14:50:08.000000 tree-of-thoughts-0.2.7/tree_of_thoughts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-29 14:50:08.000000 tree-of-thoughts-0.2.7/tree_of_thoughts/abstractLanguageModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6974 2023-05-29 14:50:08.000000 tree-of-thoughts-0.2.7/tree_of_thoughts/guidanceModels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-05-29 14:50:08.000000 tree-of-thoughts-0.2.7/tree_of_thoughts/huggingModels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-05-29 14:50:08.000000 tree-of-thoughts-0.2.7/tree_of_thoughts/openaiModels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10133 2023-05-29 14:50:08.000000 tree-of-thoughts-0.2.7/tree_of_thoughts/treeofthoughts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:50:24.092428 tree-of-thoughts-0.2.7/tree_of_thoughts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-29 14:50:24.000000 tree-of-thoughts-0.2.7/tree_of_thoughts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-29 14:50:24.000000 tree-of-thoughts-0.2.7/tree_of_thoughts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 14:50:24.000000 tree-of-thoughts-0.2.7/tree_of_thoughts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-29 14:50:24.000000 tree-of-thoughts-0.2.7/tree_of_thoughts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-29 14:50:24.000000 tree-of-thoughts-0.2.7/tree_of_thoughts.egg-info/top_level.txt
```

### Comparing `tree-of-thoughts-0.2.6/LICENSE` & `tree-of-thoughts-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tree-of-thoughts-0.2.6/PKG-INFO` & `tree-of-thoughts-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tree-of-thoughts
-Version: 0.2.6
+Version: 0.2.7
 Summary: Tree of Thoughts - Pytorch
 Home-page: https://github.com/kyegomez/tree-of-thoughts
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `tree-of-thoughts-0.2.6/README.md` & `tree-of-thoughts-0.2.7/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -9,91 +9,91 @@
 
 Share this repository by clicking on the following buttons 😊 
 
 [![Twitter](https://img.shields.io/twitter/url?style=social&url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Ftree-of-thoughts)](https://twitter.com/intent/tweet?text=Check%20out%20this%20amazing%20project%20on%20improving%20AI%20reasoning%20-%20Tree%20of%20Thoughts!%20https://github.com/kyegomez/tree-of-thoughts)
 [![LinkedIn](https://img.shields.io/badge/Share-LinkedIn-blue?style=social&logo=linkedin)](https://www.linkedin.com/sharing/share-offsite/?url=https%3A%2F%2Fgithub.com%2Fkyegomez%2Ftree-of-thoughts)
 
 # Join Agora, Creators United
-This implementation of Tree of Thoughts is brought to you by Agora, Agora advances Humanity with open source SOTA Multi-Modality AI research! We plan on combating Humanity's grandest root problems like food insecurity, planetary insecurity, and disease, and hopefully death itself.
+This implementation of Tree of Thoughts is brought to you by Agora, Agora advances Humanity with open source SOTA Multi-Modality AI research!
+
 
 [Join our Discord and contribute to this project](https://discord.gg/qUtxnK2NMf)
 
+
+# Basic Prompts:
+No complex implementations, just pass in one of these prompts to your model: head over to `prompts.txt`
+
+'Three experts with exceptional logical thinking skills are collaboratively answering a question using a tree of thoughts method. Each expert will share their thought process in detail, taking into account the previous thoughts of others and admitting any errors. They will iteratively refine and expand upon each other's ideas, giving credit where it's due. The process continues until a conclusive answer is found. Organize the entire response in a markdown table format. The question is...'
+
 ## Getting started
 Set Openai key in your environment file `.env.` as `OPENAI_API_KEY='SK'`
 
 
 ## Method1
 Clone this repository with 
 
 ```git clone https://github.com/kyegomez/tree-of-thoughts```
 
 ``` 
 cd tree-of-thoughts
+python3 -m pip install -r requirements.txt
 cd tree_of_thoughts
 python3 treeofthoughts.py --problem "design an new transportation system for an all-new city" --search_algorithm="BFS"
 ```
 Add ` OPENAI_API_KEY='API KEY'` in the .env!
 
-
+And in the `examples` folder we have other examples for huggingface transformers + hugginggface pipelines
 
 ## Method2
 or:
 
 ```pip install tree-of-thoughts ```
 
 
-Navigate to the repository folder: ```cd tree-of-thoughts```
-
-```pip install openai```
-
 Create a Python script (e.g., example.py) and import the necessary classes:
 
 ``` python
 import os
 from tree_of_thoughts.openaiModels import OpenAILanguageModel
 from tree_of_thoughts.treeofthoughts import TreeofThoughts
 from tree_of_thoughts.huggingModel import HuggingLanguageModel
 
-use_v2 = False
-
 
 model = OptimizedOpenAILanguageModel(api_key='') # api_model="gpt4" # for higher performance base model is not smart
 
 
 #choose search algorithm('BFS' or 'DFS')
 search_algorithm = "BFS"
 
 #cot or propose
 strategy="cot"
 
 # value or vote
 evaluation_strategy = "value"
 
-
+#initialize the class
 tree_of_thoughts = TreeofThoughts(model, search_algorithm)
 
-
+#enter an problem if you want!
 input_problem = "use 4 numbers and basic arithmetic operations (+-*/) to obtain 24" #note for superior intelligent responses you'll have to be more explicit in your prompt and select a better model
     
 
-input_problem = "What are the best reasoning methods to advance Large Language Models"
-k = 5 #number of thoughts to generate
-T = 3 # maximum depth of the search tree
-b = 5 # branching factor -< number of child nodes for each branch
-vth = 0.5 # pruning state -> any evaluated thought below this is eliminated
-timeout = 10 #10 seconds timeout before stop
-confidence = 0.8 #cmodel is confident on performance
-max_iterations = 40 #tree branh nodes 
-convergence_threshold = 0.01 #determining when the search process has converged
-convergence_count = 5 # number of searchers to be considered converged
-#read documentation for more
+num_thoughts = 2
+max_steps= 3
+max_states = 5
+value_threshold= 0.5
 
 #call the solve emthod with the input problem and other params
-solution = tree_of_thoughts.solve(input_problem, k, T, b, vth, timeout, confidence, max_iterations, convergence_threshold, convergence_count)
 
+solution = tree_of_thoughts.solve(input_problem, 
+    num_thoughts=num_thoughts,
+    max_steps=max_states,
+    max_states=5,
+    value_threshold=value_threshold,
+    )
 
 ```
 
 Or Integrate your own custom language model:
 
 ```python
 
@@ -303,47 +303,31 @@
 5. Optimize the algorithm for performance and resource usage, ensuring it scales well with large multi-modal datasets.
 6. Publish the results and gather feedback from the community to further improve the multi-modal Tree of Thoughts algorithm.
 
 Join us on this exciting journey to advance the Tree of Thoughts algorithm to multi-modality superintelligence! 🚀
 
 # Documentation:
 
-## x (str): 
+## input_problem (str): 
 The initial problem statement or prompt for which the Tree of Thoughts algorithm will generate a solution.
 
-## k (int, default=5): 
+## num_thoughts (int, default=5): 
 The number of thoughts to generate at each state. 
 A higher value of k will result in more thoughts being generated, potentially leading to a more diverse set of solutions. However, increasing k may also increase the computational complexity and time required to find a solution.
 
-## T (int, default=3): 
+## max_steps (int, default=3): 
 The maximum depth of the search tree. 
 A higher value of T allows the algorithm to explore deeper states, potentially leading to better solutions. However, increasing T may also increase the computational complexity and time required to find a solution.
 
-## b (int, default=5): 
+## max_states (int, default=5): 
 The branching factor of the search tree, which determines the maximum number of child nodes for each parent node.
 A higher value of b allows the algorithm to explore more states, potentially leading to better solutions. However, increasing b may also increase the computational complexity and time required to find a solution.
 
-## vth (float, default=0.5): 
+## value_threshold (float, default=0.5): 
 The value threshold for pruning states. 
 States with a value below this threshold will be discarded, reducing the search space. A higher value of vth will result in a more aggressive pruning strategy, potentially speeding up the search process. However, setting vth too high may cause the algorithm to discard promising states, leading to suboptimal solutions.
 
-## timeout (int, default=10): 
-The maximum time (in seconds) allowed for the search process. If the search process exceeds this time limit, the algorithm will return the best solution found so far.
-
-## confidence_threshold (float, default=0.8): 
-The confidence threshold for determining when a solution is satisfactory. If the algorithm finds a solution with a confidence value above this threshold, it will return the solution immediately.
-
-## max_iterations (int, default=40): 
-The maximum number of iterations allowed for the search process. If the search process exceeds this number of iterations, the algorithm will return the best solution found so far.
-
-## convergence_threshold (float, default=0.01): 
-The convergence threshold for determining when the search process has converged. If the difference in confidence values between consecutive iterations is below this threshold for a specified number of iterations (convergence_count), the algorithm will return the best solution found so far.
-
-## convergence_count (int, default=5): 
-The number of consecutive iterations required for the search process to be considered converged. If the difference in confidence values between consecutive iterations is below the convergence_threshold for this number of iterations, the algorithm will return the best solution found so far.
-
-
 # Acknowledgements
 
 Thanks to: Shunyu Yao Princeton University, Dian Yu Google DeepMind, Jeffrey Zhao, Google DeepMind, Izhak Shafran Google DeepMind, Thomas L. Griffiths, Princeton University, Yuan Cao Google DeepMind, Karthik Narasimha, Princeton University for sharing this amazing work with the world!
 
 And, thanks to Phil Wang or Lucidrains for inspiring me to devote myself to open source AI Research
```

### Comparing `tree-of-thoughts-0.2.6/setup.py` & `tree-of-thoughts-0.2.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'tree-of-thoughts',
   packages = find_packages(exclude=[]),
-  version = '0.2.6',
+  version = '0.2.7',
   license='MIT',
   description = 'Tree of Thoughts - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/tree-of-thoughts',
   keywords = [
@@ -15,15 +15,17 @@
     'deep learning',
     'optimizers',
     "Prompt Engineering"
   ],
   install_requires=[
     'guidance',
     'openai',
-    'transformers'
+    'transformers',
+    'dotenv',
+    ''
   ],
   classifiers=[
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'Topic :: Scientific/Engineering :: Artificial Intelligence',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3.6',
```

### Comparing `tree-of-thoughts-0.2.6/tree_of_thoughts/guidanceModels.py` & `tree-of-thoughts-0.2.7/tree_of_thoughts/guidanceModels.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import guidance
-from .abstractLanguageModel import AbstractLanguageModel
+from tree_of_thoughts.abstractLanguageModel import AbstractLanguageModel
 import time
 import os
 import openai
 from dotenv import load_dotenv
 load_dotenv()
 class GuidanceLanguageModel(AbstractLanguageModel):
     def __init__(self, model, strategy="cot", evaluation_strategy="value", enable_ReAct_prompting=False):
```

### Comparing `tree-of-thoughts-0.2.6/tree_of_thoughts/huggingModels.py` & `tree-of-thoughts-0.2.7/tree_of_thoughts/huggingModels.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from transformers import AutoModelForCausalLM, AutoTokenizer
 from transformers import pipeline
-from .abstractLanguageModel import AbstractLanguageModel
+from tree_of_thoughts.abstractLanguageModel import AbstractLanguageModel
 
 
 class HuggingLanguageModel(AbstractLanguageModel):
     def __init__(self, model_name, model_tokenizer=None, verbose=False):
         self.model = AutoModelForCausalLM.from_pretrained(model_name)
         self.tokenizer = AutoTokenizer.from_pretrained(model_tokenizer or model_name)
         self.verbose = verbose
```

### Comparing `tree-of-thoughts-0.2.6/tree_of_thoughts/openaiModels.py` & `tree-of-thoughts-0.2.7/tree_of_thoughts/openaiModels.py`

 * *Files 11% similar despite different names*

```diff
@@ -96,23 +96,19 @@
 
 
     def generate_thoughts(self, state, k, inital_prompt):
         if (type(state) == str):
             state_text = state
         else:
             state_text = '\n'.join(state)
-        print("We receive a state of type", type(state), "For state: ", state, "\n\n")
-        
-        # prompt = f"Given the current state of reasoning: \n\n\n'{state_text}'\n\n\nGenerate the next best coherent thought to achieve the reasoning process and get the solution: "
-        # prompt = f"Based on the current state of reasoning: \n\n\n'{state_text} Provide the next coherent thought that will help progress the reasoning process and reach an soluton "
-        # prompt = f"These are the thoughts you've had: \n\n\n{state_text}, provide the next coherent thought that will help advance the reasoning process and reach an solution for this problem {inital_prompt}. Think sharply, think out of the box, predict failure. Do not leave any open questions. Unleash your mind."
+        print("New state genering thought", state, "\n\n")
         prompt = f"Considering the thoughts you've had until now:\n\n{state_text}\n\nDevise the next coherent thought that will aid in advancing the reasoning process and achieving a solution to {inital_prompt}. Assess various scenarios, think unconventionally, anticipate potential challenges, and resolve any outstanding queries. Tap into your mind's full potential and make certain no open questions remain."
 
         prompt += self.ReAct_prompt
-        print(prompt)
+        # print(prompt)
         thoughts = self.generate_text(prompt, k)
         # print(thoughts)
         print(f"Generated thoughts: {thoughts}")
         return thoughts
 
         
     def generate_solution(self, initial_prompt, state):
@@ -124,25 +120,30 @@
         prompt = f"Considering the reasoning provided:\n\n'{state_text}'\n\nDevise the best possible solution for the task: {initial_prompt}"
         answer = self.generate_text(prompt, 1)
         # print(thoughts)
         print(f"General solution : {answer}")
         return answer
 
     def evaluate_states(self, states, inital_prompt):
+
+
         if self.evaluation_strategy == 'value':
             state_values = {}
             for state in states:
-                state_text = ' '.join(state)
+                if (type(state) == str):
+                    state_text = state
+                else:
+                    state_text = '\n'.join(state)
                 print("We receive a state of type", type(state), "For state: ", state, "\n\n")
                 prompt = f"Given the current state of reasoning: '{state_text}', evaluate its value as a float between 0 and 1, become very pessimistic think of potential adverse risks on the probability of this state of reasoning achieveing {inital_prompt} and DO NOT RESPOND WITH ANYTHING ELSE: OTHER THAN AN FLOAT"
                 
                 response = self.openai_api_call_handler(prompt, 10, 1)
                 try:
                     value_text = self.openai_choice2text_handler(response.choices[0])
-                    print(f'state: {value_text}')
+                    # print(f'state: {value_text}')
                     value = float(value_text)
                     print(f"value: {value}")
                 except ValueError:
                     value = 0  # Assign a default value if the conversion fails
                 state_values[state] = value
             return state_values
```

### Comparing `tree-of-thoughts-0.2.6/tree_of_thoughts/treeofthoughts.py` & `tree-of-thoughts-0.2.7/tree_of_thoughts/treeofthoughts.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,187 +5,151 @@
 import json
 from tree_of_thoughts.openaiModels import OptimizedOpenAILanguageModel
 DATA_PATH = './data'
 import logging 
 import argparse
 logging.basicConfig(level=logging.INFO, format='%(asctime)s - %(levelname)s - %(message)s')
 logger = logging.getLogger(__name__)
+from typing import Any, Dict, List, Optional, Set, Tuple, Union
 
-DATA_PATH = './data'
 
 
 class TreeofThoughts:
-    """
-    1. Thought Decomposition --> based on problem properties
-
-    2. Thought Generator -> create a thought generator function G(p0, s, k) with 2 strategies a sample iid thoughts from a cot prompt b. propose thoughts
-    sequentially using a propose prompt
-
-    3. create a state evaluator function V(p0, S) with 2 strategies a value each state independently b. vote across states
-
-    4. Choose a search algo based on tree structure [BFS or DFS]
-
-    Implement chosen search algorithm for bfs (algo1):
-        init S0 with the input x
-        for t = 1 to T (step limit):
-            generate candidate thoughts for each state in St-1
-            eveluate the candiate states using the state evaluator V
-            select the b most promising states for St
-
-        return the final output by genertaing the thought for the best state in St for DFS(algo2)
-
-        defien a recurseive DFS function with the current state s, step t, and other required params
-
-        if t > T record the output by generating the thought for current state S
-
-        for each candidate state s in the sorted list of generated thoughts for s:
-            
-            if the evaluated value of s is greater the the threshold of vth call the dfs function recursively
-            with s and t + 1
-
-    execute the chosen search algo with the input problem, thought generator, and state evaluator, and other required params
-    """
-
     def __init__(self, model, search_algorithm):
         self.model = model
         self.search_algorithm = search_algorithm
-        self.tree = {
+        self.tree: Dict[str, Dict[str, float]] = {
             "nodes": {}
         }
 
-    def solve(self, x, k=None, T=None, b=None, vth=None, timeout=None, confidence_threshold=None, max_iterations=None, convergence_threshold=None, convergence_count=None):
+    def solve(self, initial_prompt: str, 
+              num_thoughts: Optional[int] = None, 
+              max_steps: Optional[int] = None, 
+              max_states: Optional[int] = None, 
+              value_threshold: Optional[float] = None, 
+              pruning_threshold: Optional[float] = 0.5,
+              timeout: Optional[float] = None, 
+              confidence_threshold: Optional[float] = None, 
+              max_iterations: Optional[int] = None, 
+              convergence_threshold: Optional[float] = None, 
+              convergence_count: Optional[int] = None) -> str:
         start_time = time.time()
         self.file_name = f"logs/tree_of_thoughts_output_{self.search_algorithm}.json"
         try:
             best_thoughts = ""
             if self.search_algorithm == 'BFS':
-                while timeout is None or time.time() - start_time < timeout:
-                    result = self.tot_bfs(x, k, T, b, vth)
-                    if result:
-                        self.save_tree_to_json(self.file_name )
-                        best_thoughts = result
+                result = self.tot_bfs(initial_prompt, num_thoughts, max_steps, max_states, value_threshold, pruning_threshold)
+                if result:
+                    self.save_tree_to_json(self.file_name)
+                    best_thoughts = result
             elif self.search_algorithm == 'DFS':
-                while timeout is None or time.time() - start_time < timeout:
-                    result = self.tot_dfs(x, k, T, vth)
-                    if result:
-                        self.save_tree_to_json(self.file_name)
-                        best_thoughts = result
-            if(best_thoughts):
-                solution = self.model.generate_solution(x, best_thoughts)
+                result = self.tot_dfs(initial_prompt, num_thoughts, max_steps, value_threshold, 
+                                          confidence_threshold=confidence_threshold, max_iterations=max_iterations, convergence_threshold=convergence_threshold, 
+                                          convergence_count=convergence_count)
+                if result:
+                    self.save_tree_to_json(self.file_name)
+                    best_thoughts = result
+            if best_thoughts:
+                solution = self.model.generate_solution(initial_prompt, best_thoughts)
                 if solution:
                     return solution
             else:
                 raise ValueError("Invalid search algorithm. Choose 'BFS' or 'DFS'.")
         except KeyboardInterrupt:
             logger.error("Keyboard interrupt detected.")
         except ValueError as e:
             logger.error(f"Error: {e}")
         finally:
             logger.info("Saving the current tree and metrics.")
             self.save_tree_to_json(self.file_name)
 
-    def tot_bfs(self, x, k, T, b, pruning_threshold):
-        S0 = {x}
-        for t in range(1, T + 1):
-            S0_t = set()
-            for s in S0:
-                for z in self.model.generate_thoughts(s, k, x):
-                    if (type(s) == str):
-                        S0_t.add((s, z))
-                    else:
-                        S0_t.add((*s, z))
-            Vt = self.model.evaluate_states(S0_t, x)
-
-            for s, v in Vt.items():
-                if not (type(s) == str):
-                    s = " | ".join(s)
-                self.tree["nodes"][s] = v
-            print("Saving tree")
-            self.save_tree_to_json(self.file_name)
-            pruned_S0_t = {s: v for s, v in Vt.items() if v >= pruning_threshold}
-
-            St = sorted(pruned_S0_t.keys(), key=lambda s: pruned_S0_t[s], reverse=True)[:b]
-            S0 = set(St)
-            
-            logger.info(f'Step: {t}, S0_t: {S0_t}, Vt: {Vt}, St: {St}, S0: {S0}')
-
-        best_state = max(St, key=lambda s: Vt[s])
-
-        return best_state
-
-
-
-    def tot_dfs(self, x, k, T, vth, pruning_threshold=0.5, confidence_threshold=None, max_iterations=None, convergence_threshold=None, convergence_count=None):
-        #vote across across states
+    def logNewState(self, state, evaluation):
+        if not (type(state) == str):
+            state = " | ".join(state)
+        self.tree["nodes"][state] = evaluation
+        self.save_tree_to_json(self.file_name)    
+        
+    def tot_bfs(self, initial_prompt, num_thoughts, max_steps, max_states, pruning_threshold):
+        current_states = [initial_prompt]
+        state_values = {}
+        try:
+            for step in range(1, max_steps + 1):
+                selected_states = []
+                for state in current_states:
+                    thoughts = self.model.generate_thoughts(state, num_thoughts, initial_prompt)
+                    evaluated_thoughts = self.model.evaluate_states({thought: 0 for thought in thoughts}, initial_prompt)
+                    for thought, value in evaluated_thoughts.items():
+                        if value >= pruning_threshold:
+                            flattened_state = (state, thought) if isinstance(state, str) else (*state, thought)
+                            selected_states.append(flattened_state)
+                            state_values[flattened_state] = value
+                            self.logNewState(flattened_state, value)
+                if len(selected_states) > 1:
+                    current_states = selected_states[:max_states]
+
+            if len(current_states) == 1:
+                return initial_prompt
+
+            if current_states:
+                best_state = max(current_states, key=lambda state: state_values[state])
+                return best_state
+        except Exception as e:
+            logger.error(f"Error in tot_bfs: {e}")
+            return None
+
+    def tot_dfs(self,
+                inital_prompt: str,
+                num_thoughts: str,
+                max_steps: int,
+                value_threshold,
+                pruning_threshold=0.5):
         output = []
-        iteration_count = 0
-        consecutive_convergence_count = 0
-        prev_best_value = None
         file_name = f"logs/tree_of_thoughts_output_{self.search_algorithm}.json"
 
-
-        def dfs(s, t):
-            nonlocal consecutive_convergence_count, prev_best_value, iteration_count, output
-            if t > T:
-                thought = self.model.generate_thoughts(s, 1, x)
-                print(f'thoughts inside dfs {thought}')
-                
-                value = self.model.evaluate_states({s}, x)[s]
-                print(f'values inside dfs {value}')
-
+        def dfs(state, step):
+            nonlocal output
+            if step > max_steps:
+                thought = self.model.generate_thoughts(state, 1, inital_prompt)
+                value = self.model.evaluate_states({state}, inital_prompt)[state]
                 output.append((thought, value))
-                print(f'output {output}')
-
-                if confidence_threshold is not None and value >= confidence_threshold:
-                    return True
-
-                if prev_best_value is not None and convergence_threshold is not None:
-                    if abs(value - prev_best_value) < convergence_threshold:
-                        consecutive_convergence_count += 1
-                    else:
-                        consecutive_convergence_count = 0
-
-                prev_best_value = value
-                iteration_count += 1
-
-                if (max_iterations is not None and iteration_count >= max_iterations) or (convergence_count is not None and consecutive_convergence_count >= convergence_count):
-                    return True
-
-                return False
+                return 
+            
+            for next_state in sorted(self.model.generated_thoughts(state, num_thoughts, inital_prompt)):
+                state_value = self.model.evaluate_states({next_state}, inital_prompt)[next_state]
+                logger.ingo(f"state: {next_state}, value: {state_value}")
 
-            for s_prime in sorted(self.model.generate_thoughts(s, k, x)):
-                state_value = self.model.evaluate_states({s_prime}, x)[s_prime]
-                logger.info(f"State: {s_prime}, Value: {state_value}")
 
-                if state_value > vth and (pruning_threshold is None or state_value >= pruning_threshold):
-                    if (type(s) == str):
-                        child = (s, s_prime)
+                if state_value > value_threshold and (pruning_threshold is None or state_value >= pruning_threshold):
+                    if isinstance(state, str):
+                        child = (state, next_state)
                     else:
-                        child = (*s, s_prime)
+                        child = (*state, next_state)
 
-                    if dfs(child, t + 1):
-                        return True
+                    dfs(child, step + 1)
 
             self.save_tree_to_json(file_name)
-            return False
         
-            
-        dfs(x, 1)
-        print(f'output  {output}')
-        best_state = max(output, key=lambda x: x[1])
-        return best_state[0]
+        try:
+            dfs(inital_prompt, 1)
+            best_state = max(output, key=lambda x: x[1])
+            return best_state[0]
+        except Exception as e:
+            logger.error(f"Error in tot_dfs: {e}")
+            return None
 
 
     def save_tree_to_json(self, file_name):
         os.makedirs(os.path.dirname(file_name), exist_ok=True)
 
         with open(file_name, 'w') as json_file:
             json.dump(self.tree, json_file, indent=4)
 
-    def print_tree(self, node, depth=0):
+    def print_tree(self, 
+                   node: str, 
+                   depth=0):
         thought = self.tree["metrics"]["thoughts"].get(node, "")
         evaluation = self.tree["metrics"]["evaluations"].get(node, "")
 
         tree_info = f"{'  ' * depth}Node: {node}, Thought: {thought}, Evaluation: {evaluation}\n"
 
         for child, parent in self.tree["nodes"].items():
             if parent == node:
@@ -236,26 +200,26 @@
     parser.add_argument("--timeout", type=int, default=10, help="Timeout in seconds before stopping")
     parser.add_argument("--confidence", type=float, default=0.8, help="Model confidence threshold")
     parser.add_argument("--max_iterations", type=int, default=40, help="Maximum number of tree branch nodes")
     parser.add_argument("--convergence_threshold", type=float, default=0.01, help="Convergence threshold for the search process")
     parser.add_argument("--convergence_count", type=int, default=5, help="Number of searches to be considered converged")
 
 
-    #args from original implementation
 
-    args = parser.parse_args()
-    print(args)
+
+    # args = parser.parse_args()
+    # print(args)
     
-    model = OptimizedOpenAILanguageModel()
-    #solve the problem using the tree of thoughts class
-    optimized_tree_of_thoughts = TreeofThoughts(model, search_algorithm=args.search_algorithm)
+    # model = OptimizedOpenAILanguageModel(api_key='')
+    # #solve the problem using the tree of thoughts class
+    # optimized_tree_of_thoughts = TreeofThoughts(model, search_algorithm=args.search_algorithm)
 
-    #solve the porblem using tree of thoughts problem helper
-    best_state = optimized_tree_of_thoughts.solve(args.problem, k=args.k, T=args.T, b=args.b, vth=args.vth)
+    # #solve the porblem using tree of thoughts problem helper
+    # best_state = optimized_tree_of_thoughts.solve(args.problem, k=args.k, T=args.T, b=args.b, vth=args.vth)
 
 
-    #generate the final silution
-    final_solution = optimized_tree_of_thoughts.model.generate_solution(best_state, args.problem)
+    # #generate the final silution
+    # final_solution = optimized_tree_of_thoughts.model.generate_solution(best_state, args.problem)
 
 
-    #print the final solutions
-    print(f"Final solution: {final_solution}")
+    # #print the final solutions
+    # print(f"Final solution: {final_solution}")
```

### Comparing `tree-of-thoughts-0.2.6/tree_of_thoughts.egg-info/PKG-INFO` & `tree-of-thoughts-0.2.7/tree_of_thoughts.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tree-of-thoughts
-Version: 0.2.6
+Version: 0.2.7
 Summary: Tree of Thoughts - Pytorch
 Home-page: https://github.com/kyegomez/tree-of-thoughts
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

