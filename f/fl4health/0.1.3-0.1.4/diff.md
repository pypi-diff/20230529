# Comparing `tmp/fl4health-0.1.3.tar.gz` & `tmp/fl4health-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fl4health-0.1.3.tar", max compression
+gzip compressed data, was "fl4health-0.1.4.tar", max compression
```

## Comparing `fl4health-0.1.3.tar` & `fl4health-0.1.4.tar`

### file list

```diff
@@ -1,33 +1,42 @@
--rw-r--r--   0        0        0     1073 2023-03-31 16:51:03.427659 fl4health-0.1.3/LICENSE
--rw-r--r--   0        0        0      439 2023-03-31 16:51:03.427659 fl4health-0.1.3/README.md
--rw-r--r--   0        0        0        0 2023-03-31 16:51:03.871692 fl4health-0.1.3/fl4health/__init__.py
--rw-r--r--   0        0        0        0 2023-03-31 16:51:03.871692 fl4health-0.1.3/fl4health/client_managers/__init__.py
--rw-r--r--   0        0        0     1646 2023-03-31 16:51:03.871692 fl4health-0.1.3/fl4health/client_managers/base_sampling_manager.py
--rw-r--r--   0        0        0     1355 2023-03-31 16:51:03.871692 fl4health-0.1.3/fl4health/client_managers/fixed_without_replacement_manager.py
--rw-r--r--   0        0        0     1724 2023-03-31 16:51:03.871692 fl4health-0.1.3/fl4health/client_managers/poisson_sampling_manager.py
--rw-r--r--   0        0        0        0 2023-03-31 16:51:03.871692 fl4health-0.1.3/fl4health/clients/__init__.py
--rw-r--r--   0        0        0     7501 2023-03-31 16:51:03.871692 fl4health-0.1.3/fl4health/clients/apfl_client.py
--rw-r--r--   0        0        0     5209 2023-03-31 16:51:03.871692 fl4health-0.1.3/fl4health/clients/clipping_client.py
--rw-r--r--   0        0        0     2184 2023-03-31 16:51:03.871692 fl4health-0.1.3/fl4health/clients/numpy_fl_client.py
--rw-r--r--   0        0        0        0 2023-03-31 16:51:03.871692 fl4health-0.1.3/fl4health/model_bases/__init__.py
--rw-r--r--   0        0        0     2488 2023-03-31 16:51:03.871692 fl4health-0.1.3/fl4health/model_bases/apfl_base.py
--rw-r--r--   0        0        0     2355 2023-03-31 16:51:03.871692 fl4health-0.1.3/fl4health/model_bases/fenda_base.py
--rw-r--r--   0        0        0        0 2023-03-31 16:51:03.871692 fl4health-0.1.3/fl4health/parameter_exchange/__init__.py
--rw-r--r--   0        0        0     1067 2023-03-31 16:51:03.871692 fl4health-0.1.3/fl4health/parameter_exchange/full_exchanger.py
--rw-r--r--   0        0        0     1291 2023-03-31 16:51:03.871692 fl4health-0.1.3/fl4health/parameter_exchange/layer_exchanger.py
--rw-r--r--   0        0        0      483 2023-03-31 16:51:03.871692 fl4health-0.1.3/fl4health/parameter_exchange/parameter_exchanger_base.py
--rw-r--r--   0        0        0        0 2023-03-31 16:51:03.871692 fl4health-0.1.3/fl4health/privacy/__init__.py
--rw-r--r--   0        0        0     8119 2023-03-31 16:51:03.871692 fl4health-0.1.3/fl4health/privacy/fl_accountants.py
--rw-r--r--   0        0        0    10562 2023-03-31 16:51:03.871692 fl4health-0.1.3/fl4health/privacy/moments_accountant.py
--rw-r--r--   0        0        0        0 2023-03-31 16:51:03.871692 fl4health-0.1.3/fl4health/strategies/__init__.py
--rw-r--r--   0        0        0    17102 2023-03-31 16:51:03.871692 fl4health-0.1.3/fl4health/strategies/client_dp_fedavgm.py
--rw-r--r--   0        0        0     5542 2023-03-31 16:51:03.871692 fl4health-0.1.3/fl4health/strategies/fedavg_sampling.py
--rw-r--r--   0        0        0     4448 2023-03-31 16:51:03.871692 fl4health-0.1.3/fl4health/strategies/noisy_aggregate.py
--rw-r--r--   0        0        0      659 2023-03-31 16:51:03.871692 fl4health-0.1.3/fl4health/test_script.py
--rw-r--r--   0        0        0     1181 2023-03-31 16:51:03.871692 fl4health-0.1.3/fl4health/utils/config.py
--rw-r--r--   0        0        0     1271 2023-03-31 16:51:03.871692 fl4health-0.1.3/fl4health/utils/dataset.py
--rw-r--r--   0        0        0     1251 2023-03-31 16:51:03.871692 fl4health-0.1.3/fl4health/utils/load_data.py
--rw-r--r--   0        0        0     2768 2023-03-31 16:51:03.871692 fl4health-0.1.3/fl4health/utils/metrics.py
--rw-r--r--   0        0        0     4997 2023-03-31 16:51:03.871692 fl4health-0.1.3/fl4health/utils/sampler.py
--rw-r--r--   0        0        0     1006 2023-03-31 16:51:03.875692 fl4health-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1151 1970-01-01 00:00:00.000000 fl4health-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-29 16:54:53.358327 fl4health-0.1.4/LICENSE
+-rw-r--r--   0        0        0      439 2023-05-29 16:54:53.358327 fl4health-0.1.4/README.md
+-rw-r--r--   0        0        0        0 2023-05-29 16:54:53.826327 fl4health-0.1.4/fl4health/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:54:53.826327 fl4health-0.1.4/fl4health/checkpointing/__init__.py
+-rw-r--r--   0        0        0     2652 2023-05-29 16:54:53.826327 fl4health-0.1.4/fl4health/checkpointing/checkpointer.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:54:53.826327 fl4health-0.1.4/fl4health/client_managers/__init__.py
+-rw-r--r--   0        0        0     1645 2023-05-29 16:54:53.826327 fl4health-0.1.4/fl4health/client_managers/base_sampling_manager.py
+-rw-r--r--   0        0        0     1355 2023-05-29 16:54:53.826327 fl4health-0.1.4/fl4health/client_managers/fixed_without_replacement_manager.py
+-rw-r--r--   0        0        0     1724 2023-05-29 16:54:53.826327 fl4health-0.1.4/fl4health/client_managers/poisson_sampling_manager.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:54:53.826327 fl4health-0.1.4/fl4health/clients/__init__.py
+-rw-r--r--   0        0        0     7832 2023-05-29 16:54:53.826327 fl4health-0.1.4/fl4health/clients/apfl_client.py
+-rw-r--r--   0        0        0     3824 2023-05-29 16:54:53.826327 fl4health-0.1.4/fl4health/clients/clipping_client.py
+-rw-r--r--   0        0        0     8540 2023-05-29 16:54:53.826327 fl4health-0.1.4/fl4health/clients/fed_prox_client.py
+-rw-r--r--   0        0        0     2953 2023-05-29 16:54:53.826327 fl4health-0.1.4/fl4health/clients/numpy_fl_client.py
+-rw-r--r--   0        0        0     9998 2023-05-29 16:54:53.826327 fl4health-0.1.4/fl4health/clients/scaffold_client.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:54:53.826327 fl4health-0.1.4/fl4health/model_bases/__init__.py
+-rw-r--r--   0        0        0     2487 2023-05-29 16:54:53.826327 fl4health-0.1.4/fl4health/model_bases/apfl_base.py
+-rw-r--r--   0        0        0     2355 2023-05-29 16:54:53.826327 fl4health-0.1.4/fl4health/model_bases/fenda_base.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:54:53.826327 fl4health-0.1.4/fl4health/parameter_exchange/__init__.py
+-rw-r--r--   0        0        0     1067 2023-05-29 16:54:53.826327 fl4health-0.1.4/fl4health/parameter_exchange/full_exchanger.py
+-rw-r--r--   0        0        0     1291 2023-05-29 16:54:53.826327 fl4health-0.1.4/fl4health/parameter_exchange/layer_exchanger.py
+-rw-r--r--   0        0        0     1509 2023-05-29 16:54:53.826327 fl4health-0.1.4/fl4health/parameter_exchange/packing_exchanger.py
+-rw-r--r--   0        0        0      483 2023-05-29 16:54:53.826327 fl4health-0.1.4/fl4health/parameter_exchange/parameter_exchanger_base.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:54:53.826327 fl4health-0.1.4/fl4health/privacy/__init__.py
+-rw-r--r--   0        0        0     8119 2023-05-29 16:54:53.826327 fl4health-0.1.4/fl4health/privacy/fl_accountants.py
+-rw-r--r--   0        0        0    10562 2023-05-29 16:54:53.826327 fl4health-0.1.4/fl4health/privacy/moments_accountant.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:54:53.826327 fl4health-0.1.4/fl4health/reporting/__init__.py
+-rw-r--r--   0        0        0     6717 2023-05-29 16:54:53.826327 fl4health-0.1.4/fl4health/reporting/fl_wanb.py
+-rw-r--r--   0        0        0     2402 2023-05-29 16:54:53.826327 fl4health-0.1.4/fl4health/server/polling.py
+-rw-r--r--   0        0        0     2706 2023-05-29 16:54:53.826327 fl4health-0.1.4/fl4health/server/server.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:54:53.826327 fl4health-0.1.4/fl4health/strategies/__init__.py
+-rw-r--r--   0        0        0    16868 2023-05-29 16:54:53.826327 fl4health-0.1.4/fl4health/strategies/client_dp_fedavgm.py
+-rw-r--r--   0        0        0     5542 2023-05-29 16:54:53.830327 fl4health-0.1.4/fl4health/strategies/fedavg_sampling.py
+-rw-r--r--   0        0        0     4448 2023-05-29 16:54:53.830327 fl4health-0.1.4/fl4health/strategies/noisy_aggregate.py
+-rw-r--r--   0        0        0     7704 2023-05-29 16:54:53.830327 fl4health-0.1.4/fl4health/strategies/scaffold.py
+-rw-r--r--   0        0        0     1154 2023-05-29 16:54:53.830327 fl4health-0.1.4/fl4health/utils/config.py
+-rw-r--r--   0        0        0     1271 2023-05-29 16:54:53.830327 fl4health-0.1.4/fl4health/utils/dataset.py
+-rw-r--r--   0        0        0     1251 2023-05-29 16:54:53.830327 fl4health-0.1.4/fl4health/utils/load_data.py
+-rw-r--r--   0        0        0     2768 2023-05-29 16:54:53.830327 fl4health-0.1.4/fl4health/utils/metrics.py
+-rw-r--r--   0        0        0     5399 2023-05-29 16:54:53.830327 fl4health-0.1.4/fl4health/utils/sampler.py
+-rw-r--r--   0        0        0     1035 2023-05-29 16:54:53.830327 fl4health-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1096 1970-01-01 00:00:00.000000 fl4health-0.1.4/PKG-INFO
```

### Comparing `fl4health-0.1.3/LICENSE` & `fl4health-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.3/fl4health/client_managers/base_sampling_manager.py` & `fl4health-0.1.4/fl4health/client_managers/base_sampling_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,11 +35,10 @@
             available_cids = [cid for cid in available_cids if criterion.select(self.clients[cid])]
 
         return available_cids
 
     def sample_all(
         self, min_num_clients: Optional[int] = None, criterion: Optional[Criterion] = None
     ) -> List[ClientProxy]:
-
         available_cids = self.wait_and_filter(min_num_clients, criterion)
 
         return [self.clients[cid] for cid in available_cids]
```

### Comparing `fl4health-0.1.3/fl4health/client_managers/fixed_without_replacement_manager.py` & `fl4health-0.1.4/fl4health/client_managers/fixed_without_replacement_manager.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.3/fl4health/client_managers/poisson_sampling_manager.py` & `fl4health-0.1.4/fl4health/client_managers/poisson_sampling_manager.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.3/fl4health/clients/apfl_client.py` & `fl4health-0.1.4/fl4health/clients/apfl_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,50 +45,54 @@
         return (
             self.get_parameters(config),
             self.num_examples["train_set"],
             metric_values,
         )
 
     def evaluate(self, parameters: NDArrays, config: Config) -> Tuple[float, int, Dict[str, Scalar]]:
+        if not self.initialized:
+            self.setup_client(config)
+
         self.set_parameters(parameters, config)
         loss, metric_values = self.validate()
         # EvaluateRes should return the loss, number of examples on client, and a dictionary holding metrics
         # calculation results.
         return (
             loss,
             self.num_examples["validation_set"],
             metric_values,
         )
 
     def train(
         self,
         epochs: int,
     ) -> Dict[str, Scalar]:
-
+        self.model.train()
         for epoch in range(epochs):
             loss_dict = {"personal": 0.0, "local": 0.0, "global": 0.0}
 
             global_meter = AverageMeter(self.metrics, "global")
             local_meter = AverageMeter(self.metrics, "local")
             personal_meter = AverageMeter(self.metrics, "personal")
             for step, (input, target) in enumerate(self.train_loader):
-
                 # Mechanics of training loop follow from original implementation
                 # https://github.com/MLOPTPSU/FedTorch/blob/main/fedtorch/comms/trainings/federated/apfl.py
                 input, target = input.to(self.device), target.to(self.device)
 
                 # Forward pass on global model and update global parameters
                 self.global_optimizer.zero_grad()
                 global_pred = self.model(input, personal=False)["global"]
                 global_loss = self.criterion(global_pred, target)
                 global_loss.backward()
                 self.global_optimizer.step()
 
                 # Make sure gradients are zero prior to foward passes of global and local model
                 # to generate personalized predictions
+                # NOTE: We zero the global optimizer grads because they are used (after the backward calculation below)
+                # to update the scalar alpha (see update_alpha() where .grad is called.)
                 self.global_optimizer.zero_grad()
                 self.local_optimizer.zero_grad()
 
                 # Personal predictions are generated as a convex combination of the output
                 # of local and global models
                 pred_dict = self.model(input, personal=True)
                 personal_pred, local_pred = pred_dict["personal"], pred_dict["local"]
@@ -128,15 +132,15 @@
             f"Client Training Losses: {train_loss_string} \n"
             f"Client Training Metrics: {train_metric_string}",
         )
 
         return metrics
 
     def validate(self) -> Tuple[float, Dict[str, Scalar]]:
-
+        self.model.eval()
         global_meter = AverageMeter(self.metrics, "global")
         local_meter = AverageMeter(self.metrics, "local")
         personal_meter = AverageMeter(self.metrics, "personal")
         loss_dict = {"global": 0.0, "personal": 0.0, "local": 0.0}
 
         with torch.no_grad():
             for input, target in self.val_loader:
```

### Comparing `fl4health-0.1.3/fl4health/clients/clipping_client.py` & `fl4health-0.1.4/fl4health/clients/clipping_client.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,40 +1,27 @@
 from logging import INFO
 from pathlib import Path
-from typing import Any, Callable, Dict, List, Optional, Tuple
+from typing import Optional, Tuple
 
-import numpy as np
 import torch
 from flwr.common import Config, NDArrays
 from flwr.common.logger import log
 from numpy import linalg
 
 from fl4health.clients.numpy_fl_client import NumpyFlClient
+from fl4health.parameter_exchange.packing_exchanger import ParameterExchangerWithClippingBit
 
 
 class NumpyClippingClient(NumpyFlClient):
     def __init__(self, data_path: Path, device: torch.device) -> None:
         super().__init__(data_path, device)
+        self.parameter_exchanger: ParameterExchangerWithClippingBit
         self.clipping_bound: Optional[float] = None
-        self.initial_weights: Optional[NDArrays] = None
         self.adaptive_clipping: Optional[bool] = None
 
-    def clip_and_pack_parameters(self, parameters: NDArrays) -> NDArrays:
-        clipped_weight_update, clipping_bit = self.compute_weight_update_and_clip(parameters)
-        return clipped_weight_update + [np.array([clipping_bit])]
-
-    def unpack_parameters_with_clipping_bound(self, packed_parameters: NDArrays) -> NDArrays:
-        # The last entry in the parameters list is assumed to be a clipping bound (even if we're evaluating)
-        server_model_parameters = packed_parameters[:-1]
-        # Store the starting parameters without clipping bound before client optimization steps
-        self.initial_weights = server_model_parameters
-        clipping_bound = packed_parameters[-1]
-        self.clipping_bound = float(clipping_bound)
-        return server_model_parameters
-
     def calculate_parameters_norm(self, parameters: NDArrays) -> float:
         layer_inner_products = [pow(linalg.norm(layer_weights), 2) for layer_weights in parameters]
         # network froebenius norm
         return pow(sum(layer_inner_products), 0.5)
 
     def clip_parameters(self, parameters: NDArrays) -> Tuple[NDArrays, float]:
         assert self.clipping_bound is not None
@@ -61,54 +48,25 @@
         return self.clip_parameters(weight_update)
 
     def get_parameters(self, config: Config) -> NDArrays:
         """
         This function performs clipping through compute_weight_update_and_clip and stores the clipping bit
         as the last entry in the NDArrays
         """
+        assert self.model is not None and self.parameter_exchanger is not None
         model_weights = self.parameter_exchanger.push_parameters(self.model, config)
-        return self.clip_and_pack_parameters(model_weights)
+        clipped_weight_update, clipping_bit = self.compute_weight_update_and_clip(model_weights)
+        return self.parameter_exchanger.pack_parameters(clipped_weight_update, clipping_bit)
 
     def set_parameters(self, parameters: NDArrays, config: Config) -> None:
         """
         This function assumes that the parameters being passed contain model parameters followed by the last entry
         of the list being the new clipping bound.
         """
-        server_model_parameters = self.unpack_parameters_with_clipping_bound(parameters)
+        assert self.model is not None and self.parameter_exchanger is not None
+        # The last entry in the parameters list is assumed to be a clipping bound (even if we're evaluating)
+        server_model_parameters, clipping_bound = self.parameter_exchanger.unpack_parameters(parameters)
+        # Store the starting parameters without clipping bound before client optimization steps
+        self.initial_weights = server_model_parameters
+        self.clipping_bound = clipping_bound
+        # Inject the server model parameters into the client model
         self.parameter_exchanger.pull_parameters(server_model_parameters, self.model, config)
-
-    def _first_round_fit(self, parameters: NDArrays, configs: Config) -> Tuple[List, int, Dict]:
-        # To be called on first round when weighted_averaging and adaptive_clipping are true
-
-        log(
-            INFO,
-            """Solely fetching client sample counts. Parameters not updated.""",
-        )
-
-        return (
-            parameters,
-            self.num_examples["train_set"],
-            {},
-        )
-
-    def __getattribute__(self, name: str) -> Any:
-        # If attribute is not fit, regular __getattribute__ behaviour
-        if name != "fit":
-            return object.__getattribute__(self, name)
-
-        # Wrapper for the fit function only
-        def wrapper(parameters: NDArrays, config: Config) -> Callable:
-            # If client is not initialized, setup client
-            if name == "fit" and self.initialized is False:
-                self.setup_client(config)
-
-                # Check if we should train
-                training = config.get("training", True)
-
-                # If true then call _first_round_fit method
-                if training is False:
-                    return object.__getattribute__(self, "_first_round_fit")(parameters, config)
-
-            # Else call fit method
-            return object.__getattribute__(self, "fit")(parameters, config)
-
-        return wrapper
```

### Comparing `fl4health-0.1.3/fl4health/clients/numpy_fl_client.py` & `fl4health-0.1.4/fl4health/clients/numpy_fl_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,39 @@
+import random
+import string
 from pathlib import Path
-from typing import Type, TypeVar
+from typing import Optional, Type, TypeVar
 
 import torch
 import torch.nn as nn
 from flwr.client import NumPyClient
 from flwr.common import Config, NDArrays
 
+from fl4health.checkpointing.checkpointer import TorchCheckpointer
 from fl4health.parameter_exchange.parameter_exchanger_base import ParameterExchanger
+from fl4health.reporting.fl_wanb import ClientWandBReporter
 
 T = TypeVar("T")
 
 
 class NumpyFlClient(NumPyClient):
     def __init__(self, data_path: Path, device: torch.device) -> None:
+        self.client_name = self.generate_hash()
         self.model: nn.Module
         self.parameter_exchanger: ParameterExchanger
         self.initialized = False
         self.data_path = data_path
         self.device = device
+        # Optional variable to store the weights that the client was initialized with during each round of training
+        self.initial_weights: Optional[NDArrays] = None
+        self.wandb_reporter: Optional[ClientWandBReporter] = None
+        self.checkpointer: Optional[TorchCheckpointer] = None
+
+    def generate_hash(self, length: int = 8) -> str:
+        return "".join(random.choice(string.ascii_lowercase) for i in range(length))
 
     def setup_client(self, config: Config) -> None:
         """
         This method should be used to set up all of the required components for the client through the config passed
         by the server and need only be done once. The quintessential example is data loaders with a batch size set by
         the server in the config. The parameter initialized should be set to true when this function is finished.
         Overriding this class and calling super is the preferred flow.
@@ -42,7 +54,11 @@
 
     def narrow_config_type(self, config: Config, config_key: str, narrow_type_to: Type[T]) -> T:
         config_value = config[config_key]
         if isinstance(config_value, narrow_type_to):
             return config_value
         else:
             raise ValueError(f"Provided configuration key ({config_key}) value does not have correct type")
+
+    def shutdown(self) -> None:
+        if self.wandb_reporter:
+            self.wandb_reporter.shutdown_reporter()
```

### Comparing `fl4health-0.1.3/fl4health/model_bases/apfl_base.py` & `fl4health-0.1.4/fl4health/model_bases/apfl_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,14 @@
         self.global_model: nn.Module = copy.deepcopy(model)
 
         self.adaptive_alpha = adaptive_alpha
         self.alpha = alpha
         self.alpha_lr = alpha_lr
 
     def forward(self, input: torch.Tensor, personal: bool) -> Dict[str, torch.Tensor]:
-
         if not personal:
             global_logits = self.global_model(input)
             return {"global": global_logits}
 
         global_logits = self.global_model(input)
         local_logits = self.local_model(input)
         personal_logits = self.alpha * local_logits + (1.0 - self.alpha) * global_logits
```

### Comparing `fl4health-0.1.3/fl4health/model_bases/fenda_base.py` & `fl4health-0.1.4/fl4health/model_bases/fenda_base.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.3/fl4health/parameter_exchange/full_exchanger.py` & `fl4health-0.1.4/fl4health/parameter_exchange/full_exchanger.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.3/fl4health/parameter_exchange/layer_exchanger.py` & `fl4health-0.1.4/fl4health/parameter_exchange/layer_exchanger.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.3/fl4health/privacy/fl_accountants.py` & `fl4health-0.1.4/fl4health/privacy/fl_accountants.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.3/fl4health/privacy/moments_accountant.py` & `fl4health-0.1.4/fl4health/privacy/moments_accountant.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.3/fl4health/strategies/client_dp_fedavgm.py` & `fl4health-0.1.4/fl4health/strategies/client_dp_fedavgm.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     Parameters,
     Scalar,
     ndarray_to_bytes,
     ndarrays_to_parameters,
     parameters_to_ndarrays,
 )
 from flwr.common.logger import log
+from flwr.common.typing import GetPropertiesIns
 from flwr.server.client_manager import ClientManager
 from flwr.server.client_proxy import ClientProxy
 
 from fl4health.client_managers.base_sampling_manager import BaseSamplingManager
 from fl4health.strategies.fedavg_sampling import FedAvgSampling
 from fl4health.strategies.noisy_aggregate import (
     gaussian_noisy_aggregate_clipping_bits,
@@ -157,14 +158,17 @@
         self.clipping_learning_rate = clipping_learning_rate
         self.clipping_quantile = clipping_quantile
         self.clipping_bound = initial_clipping_bound
         self.weight_noise_multiplier = weight_noise_multiplier
         self.clipping_noise_mutliplier = clipping_noise_mutliplier
         self.beta = beta
 
+        # Weighted averaging requires list of sample counts
+        # to compute client weights. Set by server after polling clients.
+        self.sample_counts: Optional[List[int]] = None
         self.m_t: Optional[NDArrays] = None
 
     def __repr__(self) -> str:
         rep = f"ClientLevelDPFedAvgM(accept_failures={self.accept_failures})"
         return rep
 
     def modify_noise_multiplier(self) -> float:
@@ -207,15 +211,14 @@
             for current_layer_weight, layer_mt in zip(self.current_weights, self.m_t)
         ]
 
     def _update_clipping_bound_with_noised_bits(
         self,
         noised_clipping_bits: float,
     ) -> None:
-
         self.clipping_bound = self.clipping_bound * math.exp(
             -self.clipping_learning_rate * (noised_clipping_bits - self.clipping_quantile)
         )
 
     def update_clipping_bound(self, clipping_bits: NDArrays) -> None:
         noised_clipping_bits_sum = gaussian_noisy_aggregate_clipping_bits(
             clipping_bits, self.clipping_noise_mutliplier
@@ -238,45 +241,28 @@
 
         if not results:
             return None, {}
         # Do not aggregate if there are failures and failures are not accepted
         if not self.accept_failures and failures:
             return None, {}
 
-        # If first round compute total expected client weight and return empty update
+        # If first round compute total expected client weight
         if self.weighted_averaging and server_round == 1:
-            successful_client_example_counts = [fit_res.num_examples for _, fit_res in results]
-            valid_failures = [fail for fail in failures if not isinstance(fail, BaseException)]
-            failed_client_example_counts = [fit_res.num_examples for _, fit_res in valid_failures]
-            client_example_counts = successful_client_example_counts + failed_client_example_counts
-            total_successful_samples = sum(client_example_counts)
-            avg_samples = total_successful_samples / len(client_example_counts)
-
-            # Total number of clients is length of successes plus length of failures
-            n_clients = len(client_example_counts)
+            assert self.sample_counts is not None
 
-            # To estimate total_samples we scale avg_samples by the n_total_clients by average samples
-            total_samples = avg_samples * n_clients
+            total_samples = sum(self.sample_counts)
 
             self.per_client_example_cap = (
                 total_samples if self.per_client_example_cap is None else self.per_client_example_cap
             )
 
-            self.total_client_weight = sum(
-                [num_examples / self.per_client_example_cap for num_examples in client_example_counts]
-            )
-
-            log(
-                INFO,
-                """First round reserved for solely fetching client sample counts when weighted_averaging is True.
-                No updates to aggregate.""",
+            self.total_client_weight: float = sum(
+                [sample_count / self.per_client_example_cap for sample_count in self.sample_counts]
             )
 
-            return None, {}
-
         # Convert results
         weights_updates = [
             (parameters_to_ndarrays(fit_res.parameters), fit_res.num_examples) for _, fit_res in results
         ]
 
         weights_updates, clipping_bits = self.split_model_weights_and_clipping_bits(weights_updates)
 
@@ -313,50 +299,64 @@
         metrics_aggregated = {}
         if self.fit_metrics_aggregation_fn:
             fit_metrics = [(res.num_examples, res.metrics) for _, res in results]
             metrics_aggregated = self.fit_metrics_aggregation_fn(fit_metrics)
         elif server_round == 1:  # Only log this warning once
             log(WARNING, "No fit_metrics_aggregation_fn provided")
 
+        # Weights plus the clipping bound to be used by the clients
         return ndarrays_to_parameters(self.current_weights + [np.array([self.clipping_bound])]), metrics_aggregated
 
     def configure_fit(
         self, server_round: int, parameters: Parameters, client_manager: ClientManager
     ) -> List[Tuple[ClientProxy, FitIns]]:
-
         # This strategy requires the client manager to be of type at least BaseSamplingManager
         assert isinstance(client_manager, BaseSamplingManager)
         """Configure the next round of training."""
         config = {}
         if self.on_fit_config_fn is not None:
             # Custom fit config function provided
             config = self.on_fit_config_fn(server_round)
 
-        config["training"] = (self.weighted_averaging and server_round == 1) is False
         fit_ins = FitIns(parameters, config)
 
-        # Sample clients
-        if self.weighted_averaging and server_round == 1:
-            clients = client_manager.sample_all(self.min_available_clients)
-        else:
-            clients = client_manager.sample_fraction(self.fraction_fit, self.min_available_clients)
+        clients = client_manager.sample_fraction(self.fraction_fit, self.min_available_clients)
 
         # Return client/config pairs
         return [(client, fit_ins) for client in clients]
 
+    def configure_poll(
+        self, server_round: int, client_manager: ClientManager
+    ) -> List[Tuple[ClientProxy, GetPropertiesIns]]:
+        """Configure server for polling of clients."""
+
+        # This strategy requires the client manager to be of type at least BaseSamplingManager
+        assert isinstance(client_manager, BaseSamplingManager)
+        config = {}
+        if self.on_fit_config_fn is not None:
+            # Custom fit config function provided
+            config = self.on_fit_config_fn(server_round)
+
+        property_ins = GetPropertiesIns(config)
+
+        clients = client_manager.sample_all(min_num_clients=self.min_available_clients)
+
+        # Return client/config pairs
+        return [(client, property_ins) for client in clients]
+
     def configure_evaluate(
         self, server_round: int, parameters: Parameters, client_manager: ClientManager
     ) -> List[Tuple[ClientProxy, EvaluateIns]]:
         """Configure the next round of evaluation."""
 
         # This strategy requires the client manager to be of type at least BaseSamplingManager
         assert isinstance(client_manager, BaseSamplingManager)
 
         # Do not configure federated evaluation if fraction eval is 0 or server is not initialized
-        if self.fraction_evaluate == 0.0 or (self.weighted_averaging and server_round == 1):
+        if self.fraction_evaluate == 0.0:
             return []
 
         # Parameters and config
         config = {}
         if self.on_evaluate_config_fn is not None:
             # Custom evaluation config function provided
             config = self.on_evaluate_config_fn(server_round)
```

### Comparing `fl4health-0.1.3/fl4health/strategies/fedavg_sampling.py` & `fl4health-0.1.4/fl4health/strategies/fedavg_sampling.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.3/fl4health/strategies/noisy_aggregate.py` & `fl4health-0.1.4/fl4health/strategies/noisy_aggregate.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.3/fl4health/utils/config.py` & `fl4health-0.1.4/fl4health/utils/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from typing import Any, Dict
 
 import yaml
 
 REQUIRED_CONFIG = {
     "n_server_rounds": int,
     "n_clients": int,
-    "local_epochs": int,
     "batch_size": int,
 }
 
 
 class InvalidConfigError(ValueError):
     pass
 
@@ -35,10 +34,10 @@
 
     # Check for invalid parameter value types
     for req_key, val in REQUIRED_CONFIG.items():
         if not isinstance(config[req_key], val):
             raise InvalidConfigError(f"{req_key} must be of type {str(val)}")
 
     # Check for invalid integer parameter values
-    for key in ["n_server_rounds", "n_clients", "local_epochs"]:
+    for key in ["n_server_rounds", "n_clients", "batch_size"]:
         if config[key] <= 0:
             raise InvalidConfigError(f"{key} must be greater than 0")
```

### Comparing `fl4health-0.1.3/fl4health/utils/dataset.py` & `fl4health-0.1.4/fl4health/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.3/fl4health/utils/load_data.py` & `fl4health-0.1.4/fl4health/utils/load_data.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.3/fl4health/utils/metrics.py` & `fl4health-0.1.4/fl4health/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `fl4health-0.1.3/fl4health/utils/sampler.py` & `fl4health-0.1.4/fl4health/utils/sampler.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,15 +41,14 @@
 
     def subsample(self, dataset: BaseDataset) -> BaseDataset:
         """
         Returns a new dataset where samples part of minority_labels are downsampled
         """
         selected_indices_list: List[torch.Tensor] = []
         for label in self.unique_labels:
-
             # Get indices of samples equal to the current label
             indices_of_label = (dataset.targets == label).nonzero()
             if label in self.minority_labels:
                 subsample_size = int(indices_of_label.shape[0] * self.downsampling_ratio)
                 subsampled_indices = self._get_random_subsample(indices_of_label, subsample_size)
                 selected_indices_list.append(subsampled_indices.squeeze())
             else:
@@ -73,14 +72,20 @@
     """
     class used to subsample a dataset so the classes of samples are distributed in a non-IID way.
     In particular, the DirichletLabelBasedSampler uses a dirichlet distribution to determine the number
     of samples from each class. The sampler is constructed by passing a beta parameter that determines
     the level of heterogeneity and a sample_percentage that determines the relative size of the modified
     dataset. Subsampling a dataset is accomplished by calling the subsample method and passing a BaseDataset object.
     This will return the resulting subsampled dataset.
+
+    NOTE: The range for beta is (0, infinity). The larger the value of beta, the more evenly the multinomial
+    probability of the labels will be. The smaller beta is the more heterogeneous it is.
+
+    np.random.dirichlet([1]*5): array([0.23645891, 0.08857052, 0.29519184, 0.2999956 , 0.07978313])
+    np.random.dirichlet([1000]*5): array([0.2066252 , 0.19644968, 0.20080513, 0.19992536, 0.19619462])
     """
 
     def __init__(self, unique_labels: List[Any], sample_percentage: float = 0.5, beta: float = 100) -> None:
         super().__init__(unique_labels)
         self.probabilities = np.random.dirichlet(np.repeat(beta, self.num_classes))
         self.sample_percentage = sample_percentage
```

### Comparing `fl4health-0.1.3/pyproject.toml` & `fl4health-0.1.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "fl4health"
-version = "0.1.3"
+version = "0.1.4"
 description = "Federated Learning for Health"
 authors = ["Vector AI Engineering <fl4health@vectorinstitute.ai>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.8.1,<3.11"
-flwr = "^1.2.0"
+python = ">=3.9.0,<3.11"
+flwr = "1.4.0"
 opacus = "^1.3.0"
 tensorflow-privacy = "^0.8.7"
 torch = "^1.12.1"
 
 [tool.poetry.group.dev.dependencies]
 nltk = "^3.8.1"
 torchvision = "^0.14.1"
@@ -41,7 +41,8 @@
 [tool.black]
 line-length = 119
 
 [tool.isort]
 line_length = 119
 profile = "black"
 skip_gitignore = true
+known_third_party = ["wandb"]
```

### Comparing `fl4health-0.1.3/PKG-INFO` & `fl4health-0.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: fl4health
-Version: 0.1.3
+Version: 0.1.4
 Summary: Federated Learning for Health
 License: MIT
 Author: Vector AI Engineering
 Author-email: fl4health@vectorinstitute.ai
-Requires-Python: >=3.8.1,<3.11
+Requires-Python: >=3.9.0,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3
-Requires-Dist: flwr (>=1.2.0,<2.0.0)
+Requires-Dist: flwr (==1.4.0)
 Requires-Dist: opacus (>=1.3.0,<2.0.0)
 Requires-Dist: tensorflow-privacy (>=0.8.7,<0.9.0)
 Requires-Dist: torch (>=1.12.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 # FL4Health
-Repository containing a federated learning engine aimed at health experimentation with an ultimate target of integration into the DHDP, the static code checker runs on python3.8
+Repository containing a federated learning engine aimed at health experimentation with an ultimate target of integration into the DHDP, the static code checker runs on python3.9
 
 # Installing dependencies
 ```
 pip install --upgrade pip
 pip install -r requirements.txt
 ```
```

