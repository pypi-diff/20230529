# Comparing `tmp/asociita-0.1.6.8.tar.gz` & `tmp/asociita-0.1.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asociita-0.1.6.8.tar", max compression
+gzip compressed data, was "asociita-0.1.6.9.tar", max compression
```

## Comparing `asociita-0.1.6.8.tar` & `asociita-0.1.6.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0        0 2023-04-07 16:31:28.755226 asociita-0.1.6.8/asociita/__init__.py
--rw-r--r--   0        0        0     3959 2023-05-20 16:17:12.712011 asociita-0.1.6.8/asociita/components/archiver/archive_manager.py
--rw-r--r--   0        0        0     4768 2023-05-18 12:35:56.518494 asociita-0.1.6.8/asociita/components/evaluator/evaluation_manager.py
--rw-r--r--   0        0        0    13585 2023-05-04 12:29:03.864051 asociita-0.1.6.8/asociita/components/evaluator/mr_evaluator.py
--rw-r--r--   0        0        0    10175 2023-05-03 13:58:58.211507 asociita-0.1.6.8/asociita/components/evaluator/or_evaluator.py
--rw-r--r--   0        0        0     4497 2023-04-17 14:01:29.838168 asociita-0.1.6.8/asociita/components/nodes/federated_node.py
--rw-r--r--   0        0        0     7400 2023-05-20 16:22:57.462290 asociita-0.1.6.8/asociita/components/orchestrator/evaluator_orchestrator.py
--rw-r--r--   0        0        0     6202 2023-05-20 16:45:47.898655 asociita-0.1.6.8/asociita/components/orchestrator/fedopt_orchestrator.py
--rw-r--r--   0        0        0    10794 2023-05-27 14:26:30.132336 asociita-0.1.6.8/asociita/components/orchestrator/generic_orchestrator.py
--rw-r--r--   0        0        0     2190 2023-05-22 09:43:29.422557 asociita-0.1.6.8/asociita/datasets/fetch_data.py
--rw-r--r--   0        0        0     2699 2023-05-22 14:23:05.141330 asociita-0.1.6.8/asociita/datasets/load_cifar.py
--rw-r--r--   0        0        0     2654 2023-05-22 14:12:53.922859 asociita-0.1.6.8/asociita/datasets/load_mnist.py
--rw-r--r--   0        0        0     6874 2023-05-22 14:12:25.240855 asociita-0.1.6.8/asociita/datasets/shard_splits.py
--rw-r--r--   0        0        0     4661 2023-05-22 14:08:01.227174 asociita-0.1.6.8/asociita/datasets/shard_transformation.py
--rw-r--r--   0        0        0      329 2023-05-19 09:42:13.494113 asociita-0.1.6.8/asociita/exceptions/settingexception.py
--rw-r--r--   0        0        0      701 2023-05-20 18:16:28.662467 asociita-0.1.6.8/asociita/models/pytorch/cifar10.py
--rw-r--r--   0        0        0    15295 2023-05-27 14:39:07.401208 asociita-0.1.6.8/asociita/models/pytorch/federated_model.py
--rw-r--r--   0        0        0      966 2023-05-12 12:18:20.228520 asociita-0.1.6.8/asociita/models/pytorch/mnist.py
--rw-r--r--   0        0        0     6068 2023-04-26 13:48:40.502010 asociita-0.1.6.8/asociita/utils/computations.py
--rw-r--r--   0        0        0      633 2023-05-12 12:12:31.672198 asociita-0.1.6.8/asociita/utils/custom_transformations.py
--rw-r--r--   0        0        0     4756 2023-05-17 12:51:14.070551 asociita-0.1.6.8/asociita/utils/handlers.py
--rw-r--r--   0        0        0      585 2023-05-22 14:29:57.943413 asociita-0.1.6.8/asociita/utils/helpers.py
--rw-r--r--   0        0        0     1843 2023-04-14 15:47:01.523825 asociita-0.1.6.8/asociita/utils/loggers.py
--rw-r--r--   0        0        0     3816 2023-05-27 15:04:45.199918 asociita-0.1.6.8/asociita/utils/optimizers.py
--rw-r--r--   0        0        0     4176 2023-04-19 13:27:23.001147 asociita-0.1.6.8/asociita/utils/orchestrations.py
--rw-r--r--   0        0        0     1059 2023-05-03 14:04:40.497199 asociita-0.1.6.8/asociita/utils/showcase.py
--rw-r--r--   0        0        0     1084 2023-04-07 16:30:34.501923 asociita-0.1.6.8/LICENSE
--rw-r--r--   0        0        0      671 2023-05-27 15:05:09.526085 asociita-0.1.6.8/pyproject.toml
--rw-r--r--   0        0        0     2862 2023-04-18 20:10:20.511705 asociita-0.1.6.8/README.md
--rw-r--r--   0        0        0     3998 1970-01-01 00:00:00.000000 asociita-0.1.6.8/setup.py
--rw-r--r--   0        0        0     3713 1970-01-01 00:00:00.000000 asociita-0.1.6.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-07 16:31:28.755226 asociita-0.1.6.9/asociita/__init__.py
+-rw-r--r--   0        0        0     3959 2023-05-20 16:17:12.712011 asociita-0.1.6.9/asociita/components/archiver/archive_manager.py
+-rw-r--r--   0        0        0     4768 2023-05-18 12:35:56.518494 asociita-0.1.6.9/asociita/components/evaluator/evaluation_manager.py
+-rw-r--r--   0        0        0    13585 2023-05-04 12:29:03.864051 asociita-0.1.6.9/asociita/components/evaluator/mr_evaluator.py
+-rw-r--r--   0        0        0    10175 2023-05-03 13:58:58.211507 asociita-0.1.6.9/asociita/components/evaluator/or_evaluator.py
+-rw-r--r--   0        0        0     4497 2023-04-17 14:01:29.838168 asociita-0.1.6.9/asociita/components/nodes/federated_node.py
+-rw-r--r--   0        0        0     7400 2023-05-20 16:22:57.462290 asociita-0.1.6.9/asociita/components/orchestrator/evaluator_orchestrator.py
+-rw-r--r--   0        0        0     6202 2023-05-20 16:45:47.898655 asociita-0.1.6.9/asociita/components/orchestrator/fedopt_orchestrator.py
+-rw-r--r--   0        0        0    11300 2023-05-29 14:02:15.655724 asociita-0.1.6.9/asociita/components/orchestrator/generic_orchestrator.py
+-rw-r--r--   0        0        0     2190 2023-05-22 09:43:29.422557 asociita-0.1.6.9/asociita/datasets/fetch_data.py
+-rw-r--r--   0        0        0     2699 2023-05-22 14:23:05.141330 asociita-0.1.6.9/asociita/datasets/load_cifar.py
+-rw-r--r--   0        0        0     2654 2023-05-22 14:12:53.922859 asociita-0.1.6.9/asociita/datasets/load_mnist.py
+-rw-r--r--   0        0        0     6874 2023-05-22 14:12:25.240855 asociita-0.1.6.9/asociita/datasets/shard_splits.py
+-rw-r--r--   0        0        0     4661 2023-05-22 14:08:01.227174 asociita-0.1.6.9/asociita/datasets/shard_transformation.py
+-rw-r--r--   0        0        0      329 2023-05-19 09:42:13.494113 asociita-0.1.6.9/asociita/exceptions/settingexception.py
+-rw-r--r--   0        0        0      701 2023-05-20 18:16:28.662467 asociita-0.1.6.9/asociita/models/pytorch/cifar10.py
+-rw-r--r--   0        0        0    15195 2023-05-29 14:02:15.656751 asociita-0.1.6.9/asociita/models/pytorch/federated_model.py
+-rw-r--r--   0        0        0      966 2023-05-12 12:18:20.228520 asociita-0.1.6.9/asociita/models/pytorch/mnist.py
+-rw-r--r--   0        0        0     6068 2023-04-26 13:48:40.502010 asociita-0.1.6.9/asociita/utils/computations.py
+-rw-r--r--   0        0        0      633 2023-05-12 12:12:31.672198 asociita-0.1.6.9/asociita/utils/custom_transformations.py
+-rw-r--r--   0        0        0     4756 2023-05-17 12:51:14.070551 asociita-0.1.6.9/asociita/utils/handlers.py
+-rw-r--r--   0        0        0      585 2023-05-22 14:29:57.943413 asociita-0.1.6.9/asociita/utils/helpers.py
+-rw-r--r--   0        0        0     1843 2023-04-14 15:47:01.523825 asociita-0.1.6.9/asociita/utils/loggers.py
+-rw-r--r--   0        0        0     4192 2023-05-29 14:02:15.657751 asociita-0.1.6.9/asociita/utils/optimizers.py
+-rw-r--r--   0        0        0     4176 2023-04-19 13:27:23.001147 asociita-0.1.6.9/asociita/utils/orchestrations.py
+-rw-r--r--   0        0        0     1059 2023-05-03 14:04:40.497199 asociita-0.1.6.9/asociita/utils/showcase.py
+-rw-r--r--   0        0        0     1084 2023-04-07 16:30:34.501923 asociita-0.1.6.9/LICENSE
+-rw-r--r--   0        0        0      705 2023-05-29 14:05:01.254994 asociita-0.1.6.9/pyproject.toml
+-rw-r--r--   0        0        0     2862 2023-04-18 20:10:20.511705 asociita-0.1.6.9/README.md
+-rw-r--r--   0        0        0     4024 1970-01-01 00:00:00.000000 asociita-0.1.6.9/setup.py
+-rw-r--r--   0        0        0     3767 1970-01-01 00:00:00.000000 asociita-0.1.6.9/PKG-INFO
```

### Comparing `asociita-0.1.6.8/asociita/components/archiver/archive_manager.py` & `asociita-0.1.6.9/asociita/components/archiver/archive_manager.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6.8/asociita/components/evaluator/evaluation_manager.py` & `asociita-0.1.6.9/asociita/components/evaluator/evaluation_manager.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6.8/asociita/components/evaluator/mr_evaluator.py` & `asociita-0.1.6.9/asociita/components/evaluator/mr_evaluator.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6.8/asociita/components/evaluator/or_evaluator.py` & `asociita-0.1.6.9/asociita/components/evaluator/or_evaluator.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6.8/asociita/components/nodes/federated_node.py` & `asociita-0.1.6.9/asociita/components/nodes/federated_node.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6.8/asociita/components/orchestrator/evaluator_orchestrator.py` & `asociita-0.1.6.9/asociita/components/orchestrator/evaluator_orchestrator.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6.8/asociita/components/orchestrator/fedopt_orchestrator.py` & `asociita-0.1.6.9/asociita/components/orchestrator/fedopt_orchestrator.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6.8/asociita/components/orchestrator/generic_orchestrator.py` & `asociita-0.1.6.9/asociita/components/orchestrator/generic_orchestrator.py`

 * *Files 3% similar despite different names*

```diff
@@ -118,38 +118,50 @@
             data_list (list[..., ....]): list containing train set and test set
                 wrapped in a hugging facr arrow_dataset.Dataset containers.
             nodes_number (int): Number of nodes that will participate in the training.
         -------------
         Returns:
             list[FederatedNode]"""
         
-        # create the manager
-        with Manager() as manager:
-            # create the shared queue
-            queue = manager.Queue()
-            # create a pool of workers
-            with Pool(nodes_number) as pool:
-                # asynchronously apply the function
-                results = [
-                    pool.apply_async(prepare_nodes, (node, model, dataset, queue))
-                    for node, model, dataset in zip(nodes_list, model_list, data_list)
-                ]
-                # consume the results
-                # Define a list of healthy nodes
-                nodes_green = []
-                for result in results:
-                    # query for results
-                    _ = result.get()
-                    updated_node = queue.get()
-                    # Adds to list only if the node is healthy
-                    if check_health(updated_node,
-                                    orchestrator_logger=orchestrator_logger):
-                        nodes_green.append(updated_node)
+        results = []
+        for node, model, dataset in zip(nodes_list, model_list, data_list):
+            node.prepare_node(model, dataset)
+            results.append(node)
+        nodes_green = []
+        for result in results:
+            if check_health(result,
+                            orchestrator_logger=orchestrator_logger):
+                nodes_green.append(result)
         return nodes_green # Returning initialized nodes
 
+        
+        # # create the manager
+        # with Manager() as manager:
+        #     # create the shared queue
+        #     queue = manager.Queue()
+        #     # create a pool of workers
+        #     with Pool(nodes_number) as pool:
+        #         # asynchronously apply the function
+        #         results = [
+        #             pool.apply_async(prepare_nodes, (node, model, dataset, queue))
+        #             for node, model, dataset in zip(nodes_list, model_list, data_list)
+        #         ]
+        #         # consume the results
+        #         # Define a list of healthy nodes
+        #         nodes_green = []
+        #         for result in results:
+        #             # query for results
+        #             _ = result.get()
+        #             updated_node = queue.get()
+        #             # Adds to list only if the node is healthy
+        #             if check_health(updated_node,
+        #                             orchestrator_logger=orchestrator_logger):
+        #                 nodes_green.append(updated_node)
+        # return nodes_green # Returning initialized nodes
+
     def train_protocol(self,
                 nodes_data: list[datasets.arrow_dataset.Dataset, 
                 datasets.arrow_dataset.Dataset]) -> None:
         """Performs a full federated training according to the initialized
         settings. The train_protocol of the generic_orchestrator.Orchestrator
         follows a classic FedAvg algorithm - it averages the local weights
         and aggregates them taking a weighted average.
```

### Comparing `asociita-0.1.6.8/asociita/datasets/fetch_data.py` & `asociita-0.1.6.9/asociita/datasets/fetch_data.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6.8/asociita/datasets/load_cifar.py` & `asociita-0.1.6.9/asociita/datasets/load_cifar.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6.8/asociita/datasets/load_mnist.py` & `asociita-0.1.6.9/asociita/datasets/load_mnist.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6.8/asociita/datasets/shard_splits.py` & `asociita-0.1.6.9/asociita/datasets/shard_splits.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6.8/asociita/datasets/shard_transformation.py` & `asociita-0.1.6.9/asociita/datasets/shard_transformation.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6.8/asociita/models/pytorch/cifar10.py` & `asociita-0.1.6.9/asociita/models/pytorch/cifar10.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6.8/asociita/models/pytorch/federated_model.py` & `asociita-0.1.6.9/asociita/models/pytorch/federated_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,32 +49,28 @@
         self.optimizer: optim.Optimizer = None
         
         # Checks for all the necessary elements:
         assert settings, "Could not find settings, please ensure that a valid dictionary containing settings was passed in a function call."
         assert net, "Could not find net object, please ensure that a valid nn.Module was passed in a function call."
         assert local_dataset, "Could not find local dataset that should be used with that model. Pleasure ensure that local dataset was passed in a function call."
         
-        self.net = net
+        self.net = copy.deepcopy(net)
         self.settings = settings
         self.node_name = node_name
 
-        #device = torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
-        # device = torch.device("cpu")
-        # self.net.to(device)
-        # model_logger.info(f"Node {node_name} will use {device} as a device.")
+        self.device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
+        self.net.to(self.device)
+        model_logger.info(f"Node {node_name} will use {self.device} as a device.")
 
         # If both, train and test data were provided
         if len(local_dataset) == 2:
             self.trainloader, self.testloader = self.prepare_data(local_dataset)
-            #self.trainloader.to(device)
-            #self.testloader.to(device)
         # If only a test dataset was provided.
         elif len(local_dataset) == 1:
             self.testloader = self.prepare_data(local_dataset, only_test=True)
-            #self.testloader.to(device)
         else:
             raise "The provided dataset object seem to be wrong. Please provide list[train_set, test_set] or list[test_set]"
 
         # List containing all the parameters to update
         params_to_update = []
         for _, param in self.net.named_parameters():
             if param.requires_grad is True:
@@ -179,28 +175,28 @@
         Raises
         -------------
             Exception: if the model is not initialized it raises an exception
         Returns
         -------------
             _type_: weights of the network
         """
-        return self.net.state_dict()
+        return copy.deepcopy(self.net.state_dict())
     
 
     def get_gradients(self):
         
         assert self.initial_model != None, "Computing gradients require saving initial model first!"
         weights_t1 = self.net.state_dict()
         weights_t2 = self.initial_model.state_dict()
         
         self.gradients = OrderedDict.fromkeys(weights_t1.keys(), 0)
         for key in weights_t1:
             self.gradients[key] = weights_t2[key] - weights_t1[key]
         
-        return self.gradients
+        return copy.deepcopy(self.gradients)
 
 
     def update_weights(self, avg_tensors) -> None:
         """This function updates the weights of the network.
         Raises
         ------
             Exception: _description_
@@ -268,16 +264,16 @@
             data = dic['image']
             target = dic['label']
 
             self.optimizer.zero_grad()
 
             if isinstance(data, list):
                 data = data[0]
-
-            #data, target = data.to(self.device), target.to(self.device)
+            
+            data, target = data.to(self.device), target.to(self.device)
             # forward pass, backward pass and optimization
             outputs = self.net(data)
             _, predicted = torch.max(outputs.data, 1)
             correct = (predicted == target).float().sum()
 
             loss = criterion(outputs, target)
             running_loss += loss.item()
```

### Comparing `asociita-0.1.6.8/asociita/models/pytorch/mnist.py` & `asociita-0.1.6.9/asociita/models/pytorch/mnist.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6.8/asociita/utils/computations.py` & `asociita-0.1.6.9/asociita/utils/computations.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6.8/asociita/utils/custom_transformations.py` & `asociita-0.1.6.9/asociita/utils/custom_transformations.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6.8/asociita/utils/handlers.py` & `asociita-0.1.6.9/asociita/utils/handlers.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6.8/asociita/utils/helpers.py` & `asociita-0.1.6.9/asociita/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6.8/asociita/utils/loggers.py` & `asociita-0.1.6.9/asociita/utils/loggers.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6.8/asociita/utils/optimizers.py` & `asociita-0.1.6.9/asociita/utils/optimizers.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 from collections import OrderedDict
 import numpy as np
-from torch import zeros, tensor
+from torch import zeros
 from typing import Union
+import torch
 
 
 class Optimizers():
     def __init__(self,
                  weights: OrderedDict) -> None:
-        self.previous_delta = OrderedDict((key, zeros(weights[key].size())) for key in weights.keys())
-        self.previous_momentum = OrderedDict((key, zeros(weights[key].size())) for key in weights.keys())
+        self.device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
+        self.previous_delta = OrderedDict((key, zeros(weights[key].size(), device=self.device)) for key in weights.keys())
+        self.previous_momentum = OrderedDict((key, zeros(weights[key].size(), device=self.device)) for key in weights.keys())
     
 
     def fed_optimize(self,
                      optimizer: str,
                      settings: dict,
                      weights: OrderedDict,
                      delta: OrderedDict) -> OrderedDict:
         if optimizer == "Simple":
-            learning_rate = settings['learning_rate']
+            learning_rate = torch.tensor(settings['learning_rate'])
+            learning_rate = learning_rate.to(self.device)
             updated_weights = self.SimpleFedopt(weights=weights,
                                                 delta = delta,
                                                 learning_rate=learning_rate)
             return updated_weights
         elif optimizer == "FedAdagard":
-            learning_rate = settings['learning_rate']
-            b1 = tensor(settings['b1'])
-            tau = tensor(settings['tau'])
+            learning_rate = torch.tensor(settings['learning_rate'])
+            b1 = torch.tensor(settings['b1'])
+            tau = torch.tensor(settings['tau'])
+            b1, tau, learning_rate = b1.to(self.device), tau.to(self.device), learning_rate.to(self.device)
             updated_weights = self.FedAdagard(weights=weights,
                                               delta=delta,
                                               b1=b1,
                                               tau=tau,
                                               learning_rate=learning_rate)
             return updated_weights
         elif optimizer == "FedYogi":
@@ -40,39 +44,39 @@
             raise "Wrong optimizer was provided. Available optimizers: FedAdagard, FedYogi, FedAdam."
 
     @staticmethod
     def SimpleFedopt(weights: OrderedDict,
                      delta: OrderedDict,
                      learning_rate: float):
         """Adds gradients to the central weights, concluding one round of Federated Training."""
-        updated_weights = OrderedDict.fromkeys(weights.keys(), tensor(0))
+        updated_weights = OrderedDict.fromkeys(weights.keys(), 0)
         for key in weights:
-            updated_weights[key] = weights[key] - (tensor(learning_rate) * delta[key])
+            updated_weights[key] = weights[key] - (learning_rate * delta[key])
         return updated_weights
     
 
     def FedAdagard(self,
                    weights: OrderedDict,
                    delta: OrderedDict,
                    b1: float, 
                    tau: float,
                    learning_rate: float) -> OrderedDict:
         # Defining the current delta.
-        current_delta = OrderedDict((key, zeros(weights[key].size())) for key in weights.keys())
-        current_momentum = OrderedDict((key, zeros(weights[key].size())) for key in weights.keys())
-        updated_weights = OrderedDict((key, zeros(weights[key].size())) for key in weights.keys())
-        
+        current_delta = OrderedDict((key, zeros(weights[key].size(), device=self.device)) for key in weights.keys())
+        current_momentum = OrderedDict((key, zeros(weights[key].size(), device=self.device)) for key in weights.keys())
+        updated_weights = OrderedDict((key, zeros(weights[key].size(), device=self.device)) for key in weights.keys())
+
         for row_key in current_delta.keys():
             current_delta[row_key] = b1 * self.previous_delta[row_key] - (1 - b1) * delta[row_key]
         
         for row_key in current_momentum.keys():
             current_momentum[row_key] = self.previous_momentum[row_key] + current_delta[row_key] ** 2
 
         for row_key in updated_weights.keys():
-            updated_weights[row_key] = weights[row_key] + learning_rate * (current_delta[row_key] / (np.sqrt(current_momentum[row_key]) + tau ))
+            updated_weights[row_key] = weights[row_key] + learning_rate * (current_delta[row_key] / (torch.sqrt(current_momentum[row_key]) + tau))
         
         self.previous_delta = current_delta
         self.previous_momentum = current_momentum
 
         return updated_weights
```

### Comparing `asociita-0.1.6.8/asociita/utils/orchestrations.py` & `asociita-0.1.6.9/asociita/utils/orchestrations.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6.8/asociita/utils/showcase.py` & `asociita-0.1.6.9/asociita/utils/showcase.py`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6.8/LICENSE` & `asociita-0.1.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6.8/README.md` & `asociita-0.1.6.9/README.md`

 * *Files identical despite different names*

### Comparing `asociita-0.1.6.8/setup.py` & `asociita-0.1.6.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,20 +16,22 @@
 {'': ['*']}
 
 install_requires = \
 ['datasets>=1.0.1,<2.0.0',
  'matplotlib>=3.7.1,<4.0.0',
  'numpy>=1.24.1,<2.0.0',
  'scikit-learn>=1.2.0,<2.0.0',
- 'torch>=1.13.1,<2.0.0',
- 'torchvision>=0.14.1,<0.15.0']
+ 'timm>=0.9,<0.10',
+ 'torch==2.0.0',
+ 'torchaudio==2.0.1',
+ 'torchvision==0.15.1']
 
 setup_kwargs = {
     'name': 'asociita',
-    'version': '0.1.6.8',
+    'version': '0.1.6.9',
     'description': "An intuitive and modular simulator for assessing the marginal value of a client's contribution in a decentralized setting.",
     'long_description': '### Setting Configuration\n\nIn order to run the simulation, the `Orchestrator` instance must receive a `settings` object that contains all the necessary parameters. It is possible to store those parameters in a `JSON` format and load them as the Python dictionary by using `asociita.utils.helper.load_from_json` function. Below is an exemplary settings object embedded as a `json` file. All the elements are necessary unless stated otherwise.\n\n```\n{\n    "orchestrator":{\n        "iterations": int,\n        "number_of_nodes": int,\n        "local_warm_start": bool,\n        "sample_size": int,\n        "evaluation": "none" | "full"\n        "save_metrics": bool,\n\t"save_models": bool,\n\t"save_path": str\n\t"nodes": [0,\n\t1,\n\t2]\n    },\n    "nodes":{\n    "local_epochs": int,\n    "model_settings": {\n        "optimizer": "RMS",\n        "batch_size": int,\n        "learning_rate": float}\n        }\n}\n```\n\nThe `settings` contains two dictionaries: `orchestrator` and `nodes`.\n\n`orchestrator` contains all the settings necessary details of the training:\n\n* `iterations` is the number of rounds to be performed. Example: `iterations:12`\n* `number_of_nodes` is the number of nodes that will be included in the training. Example: `number_of_nodes: 10`\n* `local_warm_start` allows to distribute various pre-trained weights to different local clients. Not implemeneted yet. Example: `local_warm_start: false`.\n* `sample_size` is the size of the sample that will be taken each round. Example: `sample_size : 4.`\n* `evaluation` allows to control the evaluation procedure across the clients.  Currently, only `none` or `full` are supported. Setting the evaluation to full will perform a full evaluation of every client included in the training. Example: `evaluation: full`\n* `save_metrics` allows to control whether the metrics should be saved in a csv file. Example: `save_metrics: true.`\n* `save_models` allows to control whether the models should be saved. Not implemeneted yet. Example: `save_metrics: false`.\n* `save_path` is the system path that will be used when saving the model. It is possible to define a saving_path in a method call.\n* `nodes` is the list containing the ids of all the nodes participating in the training. Length of `nodes` must be equal `number_of_nodes`.\n\n`nodes` contains all the necessary configuration for nodes.\n\n* `"local_epochs":` the number of local epochs to be performed on the local nodes.\n* `"model_settings"` is a dictionary containing all the parameters for training the model.\n  * `optimizer` is an optimizer that will be used during the training. Example: `optimizer: "RMS"`\n  * `batch_size` is the batch size that will be used during the training. Example: `batch_size: 32`\n  * `learning_rate` is the learning rate that will be used during the training. Example: `learning_rate: 0.001`\n',
     'author': 'Maciej Zuziak',
     'author_email': 'maciejkrzysztof.zuziak@isti.cnr.it',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/Scolpe/Asociita',
```

### Comparing `asociita-0.1.6.8/PKG-INFO` & `asociita-0.1.6.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: asociita
-Version: 0.1.6.8
+Version: 0.1.6.9
 Summary: An intuitive and modular simulator for assessing the marginal value of a client's contribution in a decentralized setting.
 Home-page: https://github.com/Scolpe/Asociita
 License: MIT
 Author: Maciej Zuziak
 Author-email: maciejkrzysztof.zuziak@isti.cnr.it
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: datasets (>=1.0.1,<2.0.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: numpy (>=1.24.1,<2.0.0)
 Requires-Dist: scikit-learn (>=1.2.0,<2.0.0)
-Requires-Dist: torch (>=1.13.1,<2.0.0)
-Requires-Dist: torchvision (>=0.14.1,<0.15.0)
+Requires-Dist: timm (>=0.9,<0.10)
+Requires-Dist: torch (==2.0.0)
+Requires-Dist: torchaudio (==2.0.1)
+Requires-Dist: torchvision (==0.15.1)
 Project-URL: Repository, https://github.com/Scolpe/Asociita
 Description-Content-Type: text/markdown
 
 ### Setting Configuration
 
 In order to run the simulation, the `Orchestrator` instance must receive a `settings` object that contains all the necessary parameters. It is possible to store those parameters in a `JSON` format and load them as the Python dictionary by using `asociita.utils.helper.load_from_json` function. Below is an exemplary settings object embedded as a `json` file. All the elements are necessary unless stated otherwise.
```

