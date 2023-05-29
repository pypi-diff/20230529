# Comparing `tmp/perming-1.0.0-py3-none-any.whl.zip` & `tmp/perming-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 12362 bytes, number of entries: 10
--rw-rw-rw-  2.0 fat      849 b- defN 23-May-25 11:55 perming/__init__.py
--rw-rw-rw-  2.0 fat      176 b- defN 23-May-25 11:55 perming/_typing.py
--rw-rw-rw-  2.0 fat    18786 b- defN 23-May-25 12:49 perming/_utils.py
--rw-rw-rw-  2.0 fat      606 b- defN 23-May-25 11:57 perming/_version.py
--rw-rw-rw-  2.0 fat    10392 b- defN 23-May-25 11:57 perming/common.py
--rw-rw-rw-  2.0 fat     5455 b- defN 23-May-25 11:57 perming/general.py
--rw-rw-rw-  2.0 fat     7644 b- defN 23-May-25 13:09 perming-1.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-25 13:09 perming-1.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-May-25 13:09 perming-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      746 b- defN 23-May-25 13:09 perming-1.0.0.dist-info/RECORD
-10 files, 44754 bytes uncompressed, 11108 bytes compressed:  75.2%
+Zip file size: 12483 bytes, number of entries: 10
+-rw-rw-rw-  2.0 fat      849 b- defN 23-May-29 16:13 perming/__init__.py
+-rw-rw-rw-  2.0 fat      176 b- defN 23-May-29 15:03 perming/_typing.py
+-rw-rw-rw-  2.0 fat    19350 b- defN 23-May-29 16:18 perming/_utils.py
+-rw-rw-rw-  2.0 fat      568 b- defN 23-May-29 14:50 perming/_version.py
+-rw-rw-rw-  2.0 fat    10419 b- defN 23-May-29 16:22 perming/common.py
+-rw-rw-rw-  2.0 fat     5523 b- defN 23-May-29 15:25 perming/general.py
+-rw-rw-rw-  2.0 fat     7672 b- defN 23-May-29 16:25 perming-1.0.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-29 16:25 perming-1.0.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-May-29 16:25 perming-1.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      746 b- defN 23-May-29 16:25 perming-1.0.1.dist-info/RECORD
+10 files, 45403 bytes uncompressed, 11229 bytes compressed:  75.3%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: perming/common.py
 Comment: 
 
 Filename: perming/general.py
 Comment: 
 
-Filename: perming-1.0.0.dist-info/METADATA
+Filename: perming-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: perming-1.0.0.dist-info/WHEEL
+Filename: perming-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: perming-1.0.0.dist-info/top_level.txt
+Filename: perming-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: perming-1.0.0.dist-info/RECORD
+Filename: perming-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## perming/__init__.py

```diff
@@ -22,8 +22,8 @@
 
 COMMON_MODELS = {
     'Regression': Regressier,
     'Binary-classification': Binarier,
     'Multi-classification': Mutipler
 }
 
-__version__ = '1.0.0'
+__version__ = '1.0.1'
```

## perming/_utils.py

```diff
@@ -1,14 +1,10 @@
 # Copyright (c) 2023 linjing-lab
 
-import torch
-import random
-import numpy
-import gc
-import sortingx
+import torch, random, numpy, gc, sortingx
 from joblib import parallel_backend
 from collections import OrderedDict
 from ._typing import TabularData, Tuple, Dict, Optional, Any
 from ._version import parse_torch_version
 
 class TabularDataset(torch.utils.data.Dataset):
     '''
@@ -35,18 +31,20 @@
     :param hidden_layer_sizes: Tuple[int], configure the size of each hidden layer. default: (100,).
     :param activation:, activation configured by Classfier. default: torch.nn.ReLU().
     '''
     def __init__(self, input_: int, num_classes: int, hidden_layer_sizes: Tuple[int], activation) -> None:
         super(MLP, self).__init__()
         self.squeeze = False if num_classes > 1 else True
         if hidden_layer_sizes:
+            assert hidden_layer_sizes[0] > 0, "Please ensure any layer of hidden_layer_sizes > 0"
             model_layers, hidden_length = OrderedDict(), len(hidden_layer_sizes)
             model_layers['Linear0'] = torch.nn.Linear(input_, hidden_layer_sizes[0])
             model_layers['Activation0'] = activation
             for index in range(1, hidden_length):
+                assert hidden_layer_sizes[index] > 0, "Please ensure any layer of hidden_layer_sizes > 0"
                 linear_, activation_ = "Linear" + str(index), "Activation" + str(index)
                 model_layers[linear_] = torch.nn.Linear(hidden_layer_sizes[index - 1], hidden_layer_sizes[index])
                 model_layers[activation_] = activation
             model_layers["Linear" + str(hidden_length)] = torch.nn.Linear(hidden_layer_sizes[hidden_length - 1], num_classes)
             self.mlp = torch.nn.Sequential(model_layers)
         else:
             self.mlp = torch.nn.Linear(input_, num_classes)
@@ -60,16 +58,16 @@
     Basic Model for Configuring Common Models and General Box.
     :param input_: int, features' dimension of tabular data is input_.
     :param num_classes: int, total number of correct label categories.
     :param hidden_layer_sizes: Tuple[int], configure the size of each hidden layer.
     :param device: Any, device configured by common models and general box.
     :param activation: Any, activated function configured by common models and general box.
     :param criterion: Any, loss function determined by common models and general box.
-    :param solver: str, optimization function coordinated with `torch.optim.lr_scheduler`. default: adam. (modified more params in `_solver`.)
-    :param batch_size: int, batch size of dataset in one training process. default: 32.
+    :param solver: str, optimization coordinated with `torch.optim.lr_scheduler`. default: adam. (modified more params in `_solver`.)
+    :param batch_size: int, batch size of tabular dataset in one training process. default: 32.
     :param learning_rate_init: float, initialize the learning rate of the optimizer. default: 1e-3.
     :param lr_scheduler: str | None, set the learning rate scheduler integrated with the optimizer. default: None. (modifier more params in `_scheduler`.)
     '''
     def __init__(self,
                  input_: int,
                  num_classes: int,
                  hidden_layer_sizes: Tuple[int],
@@ -79,14 +77,16 @@
                  solver: str, 
                  batch_size: int, 
                  learning_rate_init: float,
                  lr_scheduler: Optional[str]=None) -> None:
 
         assert input_ > 0
         assert num_classes > 0
+        assert batch_size > 0
+        assert learning_rate_init > 0
         self.input: int = input_
         self.num_classes: int = num_classes
         self.activation = activation
         self.device = device # device configuration
         self.criterion = criterion
         self.batch_size: int = batch_size
         self.lr: float = learning_rate_init
@@ -146,15 +146,15 @@
     def data_loader(self, 
                     features: TabularData, 
                     target: TabularData, 
                     ratio_set: Dict[str, int]={'train': 8, 'test': 1, 'val': 1}, 
                     worker_set: Dict[str, int]={'train': 8, 'test': 2, 'val': 1},
                     random_seed: Optional[int]=None) -> None:
         '''
-        Encapsulate Dataset to DataLoader from Scratch.
+        Encapsulate Dataset to DataLoader from Tabular Dataset.
         :param features: TabularData, composed of n-row samples and m-column features.
         :param target: TabularData, consists of correct labels or values with size at n.
         :param ratio_set: Dict[str, int], stores the proportion of train-set, test-set and val-set. default: {'train': 7, 'test': 2, 'val': 1}.
         :param worker_set: Dict[str, int], load the configuration of DataLoader with multi-threaded. default: {'train': 8, 'test': 2, 'val': 1}.
         :param random_seed: int | None, random.seed(random_seed) used for fixed random datasets. default: None.
         '''
         assert ratio_set['train'] > 0 and ratio_set['test'] > 0 and ratio_set['val'] > 0
@@ -162,42 +162,44 @@
         assert ratio_set['train'] + ratio_set['test'] + ratio_set['val'] == 10, "The sum of 3 datasets' ratio needs to be 10."
         assert features.shape[1] == self.input, "Please ensure `input_` is equal to `features.shape[1]`."
         if self.num_classes >= 2:
             self.unique = numpy.unique(target)
             assert len(self.unique) == self.num_classes, "Please ensure `num_classes` is equal to `len(numpy.unique(labels))`."
             self.indices = dict(zip(self.unique, range(self.num_classes)))
             target = numpy.array([self.indices[value] for value in target], dtype=numpy.int8)
+        assert str(target.dtype).startswith("float"), "Please ensure target.dtype in any float type of numpy.dtype"
         train_, test_, val_ = train_test_val_split(features, target, ratio_set, random_seed)
         self.train_loader = torch.utils.data.DataLoader(TabularDataset(train_['features'], train_['target'], self.model.squeeze), batch_size=self.batch_size, shuffle=True, num_workers=worker_set['train'], )
         self.test_loader = torch.utils.data.DataLoader(TabularDataset(test_['features'], test_['target'], self.model.squeeze), batch_size=self.batch_size, shuffle=True, num_workers=worker_set['test'])
         self.val_loader = torch.utils.data.DataLoader(TabularDataset(val_['features'], val_['target'], self.model.squeeze), batch_size=self.batch_size, shuffle=False, num_workers=worker_set['val'])
 
     def train_val(self, 
                   num_epochs: int=2, 
                   interval: int=100, 
                   backend: str="threading", 
                   n_jobs: int=-1) -> None:
         '''
         Training and Validation with `train_loader` and `val_container`.
-        :param num_epochs: int, training epochs for `self.model`. default: 5.
+        :param num_epochs: int, training epochs for `self.model`. default: 2.
         :param interval: int, console output interval. default: 100.
         :param backend: str, "threading", "multiprocessing, 'locky'. default: "threading".
         :param n_jobs: int, accelerate processing of validation. default: -1.
         '''
+        assert num_epochs > 0 and interval > 0
         assert n_jobs == -1 or n_jobs > 0
         total_step = len(self.train_loader)
         self._set_container(backend, n_jobs)
         for epoch in range(num_epochs):
             gc.collect()
             torch.cuda.empty_cache()
             for i, (features, target) in enumerate(self.train_loader):
                 features = features.to(self.device)
                 target = target.to(self.device)
 
-                # froward pass
+                # forward pass
                 outputs = self.model(features)
                 self.train_loss = self.criterion(outputs, target)
 
                 # backward and optimize
                 self.solver.zero_grad()
                 self.train_loss.backward()
                 _ = self.solver.step() if self.lr_scheduler == None else self.lr_scheduler.step()
@@ -231,48 +233,48 @@
             for features, target in self.test_loader:
                 features = features.to(self.device)
                 target = target.to(self.device)            
                 outputs = self.model(features)
                 if self.num_classes >= 2:
                     _, predicted = torch.max(outputs.data, 1)
                     for index, value in enumerate(predicted):
-                        self.correct_class[self.unique[value]][1] += 1
-                        self.correct_class[self.unique[value]][0] += (value == target[index]).item()
+                        self.correct_class[self.unique[value]][1] += 1 # record total numbers of each class
+                        self.correct_class[self.unique[value]][0] += (value == target[index]).item() # record total true numbers of each class
                     correct += (predicted == target).sum().item()
                 self.test_loss += self.criterion(outputs, target)
             self.test_loss /= test_loader_step
             print('loss of {0} on the {1} test dataset: {2}. accuracy: {3:.4f} %'.format(self.__class__.__name__, test_total, self.test_loss.item(), 100 * correct / test_total))
         return OrderedDict(self._packing(sort_by, sort_kernel, sort_state))
     
     def save(self, show: bool=True, dir: str='./model') -> None:
         '''
-        Save Model Checkpoint with Classifier.
+        Save Model Checkpoint with Classifier and Regressier.
         :param show: bool, whether to show `model.state_dict()`. default: True.
-        :param dir: str, model save to. default: './model'.
+        :param dir: str, model save to dir. default: './model'.
         '''
         if show:
             print(self.model.state_dict())
         torch.save(self.model.state_dict(), dir)
 
     def load(self, show: bool=True, dir: str='./model') -> None:
         '''
-        Load Model Checkpoint to Classifier.
+        Save Model Checkpoint with Classifier and Regressier.
         :param show: bool, whether to show `model.state_dict()`. default: True.
-        :param dir: str, model load from. default: './model'.
+        :param dir: str, model load from dir. default: './model'.
         '''
         params = torch.load(dir)
         self.model.load_state_dict(params)
         if show:
             print(self.model.state_dict())
 
     def _packing(self, by: str, kernel: str, state: bool) -> Dict[str, Any]:
         '''
         Pack Test Returned Data including `correct_class` and returned result of `sortingx.[method]()`.
         :param by: str, choose which way to sort the order of 'correct_class'.
-        :param kernel: str, choose which kernel used for sorting.
+        :param kernel: str, choose which kernel used for sorting `correct_class.items()`.
         :param state: bool, choose the state when `correct_class` is sorting.
         '''
         assert kernel in sortingx.__all__, "Please ensure kernel is sortingx.__all__."
         kernel = eval('sortingx.' + kernel)
         loss_, classify, regress = {
             'loss': {'train': self.train_loss.item(), 
                      'val': self.val_loss.item(),
@@ -297,16 +299,16 @@
         else:
             regress.update(loss_)
             return regress
 
     def _set_container(self, backend: str, n_jobs: int) -> None:
         '''
         Acquire Validation Container with `parallel_backend` at `n_jobs`.
-        :param backend: str, "threading", "multiprocessing, 'locky'. default: "threading".
-        :param n_jobs: int, set jobs for backend.
+        :param backend: str, "threading", "multiprocessing, 'locky'.
+        :param n_jobs: int, set jobs with backend to accelerate process.
         '''
         with parallel_backend(backend, n_jobs=n_jobs):
             val_iter, self.val_container = iter(self.val_loader), []
             while 1:
                 try:
                     self.val_container.append(next(val_iter))
                 except StopIteration:
```

## perming/_version.py

```diff
@@ -4,12 +4,11 @@
     '''
     :param version_info: str, version information of PyTorch with `__version__`.
 
     :return tuple value about `version` & `cu_info`.
     '''
     if version_info.find('cu') != -1:
         version_cu = version_info.split('+')
-        version = tuple(version_cu[0].split('.'))
-        cuda_info = version_cu[1]
-        return version, cuda_info
+        version = version_cu[0].split('.')
+        return version, version_cu[1]
     else:
         raise Exception('Please refer to https://pytorch.org/get-started/locally/ for PyTorch with cuda version compatible with your windows computer.')
```

## perming/common.py

```diff
@@ -19,15 +19,15 @@
                  input_: int, 
                  hidden_layer_sizes: Tuple[int]=(100,),
                  *,
                  activation: str='relu', 
                  criterion: str='MSELoss',
                  solver: str='adam', 
                  batch_size: int=32, 
-                 learning_rate_init: float=1e-3,
+                 learning_rate_init: float=1e-2,
                  lr_scheduler: Optional[str]=None) -> None:
 
         super(Regressier, self).__init__(input_, 
                                          1, 
                                          hidden_layer_sizes, 
                                          torch.device("cuda" if torch.cuda.is_available() else "cpu"), 
                                          self._activate(activation), 
@@ -87,27 +87,27 @@
                  input_: int, 
                  hidden_layer_sizes: Tuple[int]=(100,),
                  *,
                  activation: str='relu', 
                  criterion: str='BCELoss',
                  solver: str='adam', 
                  batch_size: int=32, 
-                 learning_rate_init: float=1e-3,
+                 learning_rate_init: float=1e-2,
                  lr_scheduler: Optional[str]=None) -> None:
 
         super(Binarier, self).__init__(input_, 
-                                     2, 
-                                     hidden_layer_sizes, 
-                                     torch.device("cuda" if torch.cuda.is_available() else "cpu"), 
-                                     self._activate(activation), 
-                                     self._criterion(criterion), 
-                                     solver, 
-                                     batch_size, 
-                                     learning_rate_init, 
-                                     lr_scheduler)
+                                       2, 
+                                       hidden_layer_sizes, 
+                                       torch.device("cuda" if torch.cuda.is_available() else "cpu"), 
+                                       self._activate(activation), 
+                                       self._criterion(criterion), 
+                                       solver, 
+                                       batch_size, 
+                                       learning_rate_init, 
+                                       lr_scheduler)
 
     def _activate(self, activation: str):
         '''
         Configure Activation with `activation` and `inplace_on`.
         :param activation: str, "relu", "tanh", "sigmoid", "rrelu", "leaky_relu", "elu", "celu".
         '''
         if activation == 'relu':
@@ -158,27 +158,27 @@
                  num_classes: int,
                  hidden_layer_sizes: Tuple[int]=(100,),
                  *,
                  activation: str='relu', 
                  criterion: str='CrossEntropyLoss',
                  solver: str='adam', 
                  batch_size: int=32, 
-                 learning_rate_init: float=1e-3,
+                 learning_rate_init: float=1e-2,
                  lr_scheduler: Optional[str]=None) -> None:
         
         super(Mutipler, self).__init__(input_, 
-                                      num_classes, 
-                                      hidden_layer_sizes, 
-                                      torch.device("cuda" if torch.cuda.is_available() else "cpu"), 
-                                      self._activate(activation), 
-                                      self._criterion(criterion), 
-                                      solver, 
-                                      batch_size, 
-                                      learning_rate_init, 
-                                      lr_scheduler)
+                                       num_classes, 
+                                       hidden_layer_sizes, 
+                                       torch.device("cuda" if torch.cuda.is_available() else "cpu"), 
+                                       self._activate(activation), 
+                                       self._criterion(criterion), 
+                                       solver, 
+                                       batch_size, 
+                                       learning_rate_init, 
+                                       lr_scheduler)
         assert num_classes >= 2
 
     def _activate(self, activation: str):
         '''
         Configure Activation with `activation` and `inplace_on`.
         :param activation: str, "relu", "rrelu", "leaky_relu", "elu", "celu".
         '''
```

## perming/general.py

```diff
@@ -9,31 +9,31 @@
     :param input_: int, features' dimension of tabular data is input_.
     :param num_classes: int, total number of correct label categories.
     :param hidden_layer_sizes: Tuple[int], configure the size of each hidden layer. default: (100,).
     :param device: str, configure hardware environment for training. options: "cuda", "cpu". default: cuda.
     :param activation: str, configure function that activates the hidden layer. default: relu.
     :param inplace_on: bool, whether to use `inplace=True` on activation. default: False.
     :param criterion: str, loss function determined by different learning problem. default: CrossEntropyLoss.
-    :param solver: str, optimization function coordinated with `torch.optim.lr_scheduler`. default: adam.
-    :param batch_size: int, batch size of dataset in one training process. default: 32.
+    :param solver: str, optimization coordinated with `torch.optim.lr_scheduler`. default: adam.
+    :param batch_size: int, batch size of tabular dataset in one training process. default: 32.
     :param learning_rate_init: float, initialize the learning rate of the optimizer. default: 1e-3.
     :param lr_scheduler: str | None, set the learning rate scheduler integrated with the optimizer. default: None.
     '''
     def __init__(self, 
                  input_: int, 
                  num_classes: int, # num_classes=1
                  hidden_layer_sizes: Tuple[int]=(100,),
                  device: str="cuda",
                  *,
                  activation: str='relu', 
                  inplace_on: bool=False, 
                  criterion: str='CrossEntropyLoss', # criterion='MSELoss'
                  solver: str='adam', 
                  batch_size: int=32, 
-                 learning_rate_init: float=1e-3,
+                 learning_rate_init: float=1e-2,
                  lr_scheduler: Optional[str]=None) -> None:
         
         super(Box, self).__init__(input_, 
                                   num_classes, 
                                   hidden_layer_sizes, 
                                   self._device(device), 
                                   self._activate(activation, inplace_on), 
@@ -43,34 +43,34 @@
                                   learning_rate_init, 
                                   lr_scheduler)
         assert num_classes >= 1
 
     def _device(self, option: str) -> None:
         '''
         Set Device for Model and Training.
-        :param option: str, "cuda" or "cpu".
+        :param option: device configuration. str, "cuda" or "cpu".
         '''
         if option == "cuda":
             return torch.device(option if torch.cuda.is_available() else "cpu")
         elif option == "cpu":
             return torch.device(option)
         else:
             raise ValueError('Box Only Support 2 Options for Device Configuration: "cuda" or "cpu".')
 
     def _activate(self, activation: str, inplace_on: bool):
         '''
         Configure Activation with `activation` and `inplace_on`.
         :param activation: str, "relu", "tanh", "sigmoid", "rrelu", "leaky_relu", "prelu", "softplus", "elu", "celu".
         :param inplace_on: bool, whether to use `inplace=True` on activations. default: False.
         '''
-        if activation == 'relu':
+        if activation == 'relu': # most use
             return torch.nn.ReLU(inplace=inplace_on)
         elif activation == 'tanh':
             return torch.nn.Tanh()
-        elif activation == 'sigmoid':
+        elif activation == 'sigmoid': # can be used in classification = 2
             return torch.nn.Sigmoid()
         elif activation == 'rrelu':
             return torch.nn.RReLU(inplace=inplace_on)
         elif activation == 'leaky_relu':
             return torch.nn.LeakyReLU(inplace=inplace_on)
         elif activation == 'prelu':
             return torch.nn.PReLU()
```

## Comparing `perming-1.0.0.dist-info/METADATA` & `perming-1.0.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perming
-Version: 1.0.0
+Version: 1.0.1
 Summary: The supervised learning framework based on perceptron for tabular data.
 Home-page: https://github.com/linjing-lab/easy-pytorch/tree/main/released_box
 Download-URL: https://github.com/linjing-lab/easy-pytorch/tags
 Author: 林景
 Author-email: linjing010729@163.com
 License: MPL 2.0
 Project-URL: Source, https://github.com/linjing-lab/easy-pytorch/tree/main/released_box/perming
@@ -45,51 +45,51 @@
 
 test with: PyTorch 1.7.1+cu101
 
 ## general model
 
 |GENERAL_BOX(Box)|Parameters|Meaning|
 |--|--|--|
-|`__init__`|input_: int<br />num_classes: int<br />hidden_layer_sizes: Tuple[int]=(100,)<br />device: str="cuda"<br />activation: str="relu"<br />inplace_on: bool=True<br />criterion: str="CrossEntropyLoss"<br />solver: str="adam"<br />batch_size: int=32<br />learning_rate_init: float=1e-3<br />lr_scheduler: Optional[str]=None|Initialize Classifier or Regressier Based on Basic Information of the Dataset Obtained through Data Preprocessing and Feature Engineering.|
+|`__init__`|input_: int<br />num_classes: int<br />hidden_layer_sizes: Tuple[int]=(100,)<br />device: str="cuda"<br />*<br />activation: str="relu"<br />inplace_on: bool=True<br />criterion: str="CrossEntropyLoss"<br />solver: str="adam"<br />batch_size: int=32<br />learning_rate_init: float=1e-2<br />lr_scheduler: Optional[str]=None|Initialize Classifier or Regressier Based on Basic Information of the Dataset Obtained through Data Preprocessing and Feature Engineering.|
 |print_config|/|Return Initialized Parameters of Multi-layer Perceptron and Graph.|
 |data_loader|features: TabularData<br />labels: TabularData<br />ratio_set: Dict[str, int]={'train': 8, 'test': 1, 'val': 1}<br />worker_set: Dict[str, int]={'train': 8, 'test': 2, 'val': 1}<br />random_seed: Optional[int]=None|Using `ratio_set` and `worker_set` to Load the Numpy Dataset into `torch.utils.data.DataLoader`.|
 |train_val|num_epochs: int=5<br />interval: int=100<br />backend: str="threading"<br />n_jobs: int=-1|Using `num_epochs` to Control Training Process and `interval` to Adjust Print Interval with Accelerated Validation Combined with `backend` and `n_jobs`.|
 |test|sort_by: str="accuracy"<br />sort_kernel: str="bubble"<br />sort_state: bool=True|Sort Returned Test Result about Correct Classes with `sort_by`, `sort_kernel`, `sort_state` Which Only Appears in Classification.|
 |save|show: bool=True<br />dir: str='./model'|Save Trained Model Parameters with Model `state_dict` Control by `show`.|
 |load|show: bool=True<br />dir: str='./model'|Load Trained Model Parameters with Model `state_dict` Control by `show`.|
 
 ## common models (cuda first)
 
 - Regression
 
 |Regressier|Parameters|Meaning|
 |--|--|--|
-|`__init__`|input_: int<br />hidden_layer_sizes: Tuple[int]=(100,)<br />activation: str="relu"<br />criterion: str="MSELoss"<br />solver: str="adam"<br />batch_size: int=32<br />learning_rate_init: float=1e-3<br />lr_scheduler: Optional[str]=None|Initialize Regressier Based on Basic Information of the Regression Dataset Obtained through Data Preprocessing and Feature Engineering with `num_classes=1`.|
+|`__init__`|input_: int<br />hidden_layer_sizes: Tuple[int]=(100,)*<br /><br />activation: str="relu"<br />criterion: str="MSELoss"<br />solver: str="adam"<br />batch_size: int=32<br />learning_rate_init: float=1e-2<br />lr_scheduler: Optional[str]=None|Initialize Regressier Based on Basic Information of the Regression Dataset Obtained through Data Preprocessing and Feature Engineering with `num_classes=1`.|
 |print_config|/|Return Initialized Parameters of Multi-layer Perceptron and Graph.|
 |train_val|num_epochs: int=5<br />interval: int=100<br />backend: str="threading"<br />n_jobs: int=-1|Using `ratio_set` and `worker_set` to Load the Regression Dataset with Numpy format into `torch.utils.data.DataLoader`.|
 |test|/|Test Module Only Show with Loss at 3 Stages: Train, Test, Val|
 |save|show: bool=True<br />dir: str='./model'|Save Trained Model Parameters with Model `state_dict` Control by `show`.|
 |load|show: bool=True<br />dir: str='./model'|Load Trained Model Parameters with Model `state_dict` Control by `show`.|
 
 - Binary-classification
 
 |Binarier|Parameters|Meaning|
 |--|--|--|
-|`__init__`|input_: int<br />hidden_layer_sizes: Tuple[int]=(100,)<br />activation: str="relu"<br />criterion: str="BCELoss"<br />solver: str="adam"<br />batch_size: int=32<br />learning_rate_init: float=1e-3<br />lr_scheduler: Optional[str]=None|Initialize Classifier Based on Basic Information of the Classification Dataset Obtained through Data Preprocessing and Feature Engineering with `num_classes=2`.|
+|`__init__`|input_: int<br />hidden_layer_sizes: Tuple[int]=(100,)*<br /><br />activation: str="relu"<br />criterion: str="BCELoss"<br />solver: str="adam"<br />batch_size: int=32<br />learning_rate_init: float=1e-2<br />lr_scheduler: Optional[str]=None|Initialize Classifier Based on Basic Information of the Classification Dataset Obtained through Data Preprocessing and Feature Engineering with `num_classes=2`.|
 |print_config|/|Return Initialized Parameters of Multi-layer Perceptron and Graph.|
 |train_val|num_epochs: int=2<br />interval: int=100<br />backend: str="threading"<br />n_jobs: int=-1|Using `ratio_set` and `worker_set` to Load the Regression Dataset with Numpy format into `torch.utils.data.DataLoader`.|
 |test|sort_by: str="accuracy"<br />sort_kernel: str="bubble"<br />sort_state: bool=True|Test Module Show with Correct Class and Loss at 3 Stages: Train, Test, Val|
 |save|show: bool=True<br />dir: str='./model'|Save Trained Model Parameters with Model `state_dict` Control by `show`.|
 |load|show: bool=True<br />dir: str='./model'|Load Trained Model Parameters with Model `state_dict` Control by `show`.|
 
 - Multi-classification
 
 |Multipler|Parameters|Meaning|
 |--|--|--|
-|`__init__`|input_: int<br />num_classes: int<br />hidden_layer_sizes: Tuple[int]=(100,)<br />activation: str="relu"<br />criterion: str="CrossEntropyLoss"<br />solver: str="adam"<br />batch_size: int=32<br />learning_rate_init: float=1e-3<br />lr_scheduler: Optional[str]=None|Initialize Classifier Based on Basic Information of the Classification Dataset Obtained through Data Preprocessing and Feature Engineering with `num_classes>2`.|
+|`__init__`|input_: int<br />num_classes: int<br />hidden_layer_sizes: Tuple[int]=(100,)*<br /><br />activation: str="relu"<br />criterion: str="CrossEntropyLoss"<br />solver: str="adam"<br />batch_size: int=32<br />learning_rate_init: float=1e-2<br />lr_scheduler: Optional[str]=None|Initialize Classifier Based on Basic Information of the Classification Dataset Obtained through Data Preprocessing and Feature Engineering with `num_classes>2`.|
 |print_config|/|Return Initialized Parameters of Multi-layer Perceptron and Graph.|
 |train_val|num_epochs: int=2<br />interval: int=100<br />backend: str="threading"<br />n_jobs: int=-1|Using `ratio_set` and `worker_set` to Load the Regression Dataset with Numpy format into `torch.utils.data.DataLoader`.|
 |test|sort_by: str="accuracy"<br />sort_kernel: str="bubble"<br />sort_state: bool=True|Sort Returned Test Result about Correct Classes with `sort_by`, `sort_kernel`, `sort_state` Which Only Appears in Classification.|
 |save|show: bool=True<br />dir: str='./model'|Save Trained Model Parameters with Model `state_dict` Control by `show`.|
 |load|show: bool=True<br />dir: str='./model'|Load Trained Model Parameters with Model `state_dict` Control by `show`.|
 
 ## pip install
```

