# Comparing `tmp/perming-1.2.1-py3-none-any.whl.zip` & `tmp/perming-1.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 12742 bytes, number of entries: 10
--rw-rw-rw-  2.0 fat      850 b- defN 23-Jun-29 11:51 perming/__init__.py
+Zip file size: 13155 bytes, number of entries: 10
+-rw-rw-rw-  2.0 fat      887 b- defN 23-Jul-03 08:11 perming/__init__.py
 -rw-rw-rw-  2.0 fat      176 b- defN 23-May-29 15:03 perming/_typing.py
--rw-rw-rw-  2.0 fat    20070 b- defN 23-Jun-29 11:56 perming/_utils.py
+-rw-rw-rw-  2.0 fat    20745 b- defN 23-Jul-03 08:32 perming/_utils.py
 -rw-rw-rw-  2.0 fat      568 b- defN 23-May-29 16:53 perming/_version.py
--rw-rw-rw-  2.0 fat    10505 b- defN 23-Jun-29 11:52 perming/common.py
--rw-rw-rw-  2.0 fat     5490 b- defN 23-Jun-29 11:38 perming/general.py
--rw-rw-rw-  2.0 fat     7523 b- defN 23-Jun-29 11:57 perming-1.2.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-29 11:57 perming-1.2.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Jun-29 11:57 perming-1.2.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      746 b- defN 23-Jun-29 11:57 perming-1.2.1.dist-info/RECORD
-10 files, 46028 bytes uncompressed, 11488 bytes compressed:  75.0%
+-rw-rw-rw-  2.0 fat    14049 b- defN 23-Jul-03 08:59 perming/common.py
+-rw-rw-rw-  2.0 fat     5605 b- defN 23-Jul-03 09:34 perming/general.py
+-rw-rw-rw-  2.0 fat     8772 b- defN 23-Jul-03 09:36 perming-1.3.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-03 09:36 perming-1.3.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jul-03 09:36 perming-1.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      746 b- defN 23-Jul-03 09:36 perming-1.3.0.dist-info/RECORD
+10 files, 51648 bytes uncompressed, 11901 bytes compressed:  77.0%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: perming/common.py
 Comment: 
 
 Filename: perming/general.py
 Comment: 
 
-Filename: perming-1.2.1.dist-info/METADATA
+Filename: perming-1.3.0.dist-info/METADATA
 Comment: 
 
-Filename: perming-1.2.1.dist-info/WHEEL
+Filename: perming-1.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: perming-1.2.1.dist-info/top_level.txt
+Filename: perming-1.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: perming-1.2.1.dist-info/RECORD
+Filename: perming-1.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## perming/__init__.py

```diff
@@ -12,18 +12,19 @@
         CUDA_VERSION, DEVICE_COUNT = torch.version.cuda, torch.cuda.device_count()
     else:
         raise OSError(f'Your PyTorch version must support cuda acceleration. Please refer to https://pytorch.org/get-started/locally/ for PyTorch compatible with your windows computer.')
 except ModuleNotFoundError:
     pass
 
 from .general import Box
-from .common import Regressier, Binarier, Mutipler
+from .common import Regressier, Binarier, Mutipler, Ranker
 
 GENERAL_BOX = Box
 
 COMMON_MODELS = {
     'Regression': Regressier,
     'Binary-classification': Binarier,
     'Multi-classification': Mutipler,
+    'Multi-outputs': Ranker
 }
 
-__version__ = '1.2.1'
+__version__ = '1.3.0'
```

## perming/_utils.py

```diff
@@ -7,19 +7,19 @@
 from ._version import parse_torch_version
 
 class TabularDataset(torch.utils.data.Dataset):
     '''
     Tabular Data Constructed with `numpy.array` noted as `TabularData`.
     :param features: TabularData, composed of n-row samples and m-column features.
     :param target: TabularData, consists of correct labels or values with size at n.
-    :param squeeze: bool, regression or classification. it represents a regression problem when `squeeze=True`.
+    :param roc: bool, regression or classification. it represents a regression problem when `roc=True`.
     '''
-    def __init__(self, features: TabularData, target: TabularData, squeeze: bool) -> None:
+    def __init__(self, features: TabularData, target: TabularData, roc: bool) -> None:
         self.features = torch.as_tensor(features, dtype=torch.float)
-        self.target = torch.as_tensor(target, dtype=torch.float) if squeeze else torch.as_tensor(target, dtype=torch.long)
+        self.target = torch.as_tensor(target, dtype=torch.float) if roc else torch.as_tensor(target, dtype=torch.long)
 
     def __getitem__(self, index):
         return self.features[index], self.target[index]
 
     def __len__(self) -> int:
         return len(self.features)
 
@@ -159,28 +159,34 @@
         '''
         assert ratio_set['train'] > 0 and ratio_set['test'] > 0 and ratio_set['val'] > 0
         assert ratio_set['train'] > 4 * ratio_set['test'], "The training set needs to be larger than the test set."
         assert ratio_set['train'] + ratio_set['test'] + ratio_set['val'] == 10, "The sum of 3 datasets' ratio needs to be 10."
         assert isinstance(features, TabularData) and features.ndim == 2, 'Please ensure features with dimension at (n_samples, n_features).'
         assert features.shape[1] == self.input, "Please ensure `input_` is equal to `features.shape[1]`."
         assert isinstance(target, TabularData), "Please ensure target format at numpy.ndarray noted as TabularData."
-        if isinstance(target[0], TabularData): # (n_samples, n_outputs)
-            raise RuntimeError("data_loader not support target with (n_samples, n_ouputs) yet.")
+        target_dtype = str(target.dtype) # __str__
+        is_int_type, is_float_type = "int" in target_dtype, "float" in target_dtype
+        self.is_target_2d = isinstance(target[0], TabularData) # judge target is 2d matrix.
+        if self.is_target_2d: # (n_samples, n_outputs)
+            assert target.shape[1] == self.num_classes, "Please ensure target with (n_samples, n_outputs=num_classes)."
+            assert is_int_type or is_float_type, "Please ensure target.dtype in any int or float type of numpy.dtype."
+            roc = not is_int_type and is_float_type
         else: # (n_samples,)
             if self.num_classes >= 2:
                 self.unique = numpy.unique(target) # int indexes -> any class with single value noted
                 assert len(self.unique) == self.num_classes, "Please ensure `num_classes` is equal to `len(numpy.unique(labels))`."
                 self.indices = dict(zip(self.unique, range(self.num_classes))) # original classes -> int indexes
                 target = numpy.array([self.indices[value] for value in target], dtype=numpy.int8) # adjust int8 -> any int dtype
             else:
-                assert str(target.dtype).startswith("float"), "Please ensure target.dtype in any float type of numpy.dtype"
+                assert is_float_type, "Please ensure target.dtype in any float type of numpy.dtype." # continuous
+            roc: bool = self.model.squeeze
         train_, test_, val_ = train_test_val_split(features, target, ratio_set, random_seed)
-        self.train_loader = torch.utils.data.DataLoader(TabularDataset(train_['features'], train_['target'], self.model.squeeze), batch_size=self.batch_size, shuffle=True, num_workers=worker_set['train'], )
-        self.test_loader = torch.utils.data.DataLoader(TabularDataset(test_['features'], test_['target'], self.model.squeeze), batch_size=self.batch_size, shuffle=True, num_workers=worker_set['test'])
-        self.val_loader = torch.utils.data.DataLoader(TabularDataset(val_['features'], val_['target'], self.model.squeeze), batch_size=self.batch_size, shuffle=False, num_workers=worker_set['val'])
+        self.train_loader = torch.utils.data.DataLoader(TabularDataset(train_['features'], train_['target'], roc), batch_size=self.batch_size, shuffle=True, num_workers=worker_set['train'], )
+        self.test_loader = torch.utils.data.DataLoader(TabularDataset(test_['features'], test_['target'], roc), batch_size=self.batch_size, shuffle=True, num_workers=worker_set['test'])
+        self.val_loader = torch.utils.data.DataLoader(TabularDataset(val_['features'], val_['target'], roc), batch_size=self.batch_size, shuffle=False, num_workers=worker_set['val'])
 
     def train_val(self, 
                   num_epochs: int=2, 
                   interval: int=100, 
                   backend: str="threading", 
                   n_jobs: int=-1) -> None:
         '''
@@ -213,15 +219,14 @@
 
                 # validation with val_container
                 self.val_loss = 0
                 with parallel_backend(backend, n_jobs=n_jobs):
                     for val_set in self.val_container:
                         outputs_val = self.model(val_set[0].to(self.device))
                         self.val_loss += self.criterion(outputs_val, val_set[1].to(self.device))
-
                 self.val_loss /= val_length
 
                 # console print
                 if (i + 1) % interval == 0:
                     print ('Epoch [{}/{}], Step [{}/{}], Training Loss: {:.4f}, Validation Loss: {:.4f}'.format(epoch+1, num_epochs, i+1, total_step, self.train_loss.item(), self.val_loss.item()))
 
     def test(self, 
@@ -229,82 +234,87 @@
              sort_state: bool=True):
         '''
         Test with Initialized Configuration. `accuracy > 0`, 'correct_class != None' and keywords only appears when `num_classes >= 2`.
         :param sort_by: str, 'accuracy', 'numbers', 'num-total'. default: 'accuracy'.
         :param sort_state: bool, whether to use descending order when sorting. default: True.
         '''
         with torch.no_grad():
-            self.test_loss, correct, self.correct_class, test_loader_step = 0, 0, dict.fromkeys(self.unique, [0, 0]) if self.num_classes >= 2 else None, len(self.test_loader)
+            self.test_loss, test_loader_step, correct = 0, len(self.test_loader), 0
             test_total = test_loader_step * self.batch_size
+            self.correct_class = dict.fromkeys(self.unique, [0, 0]) if not self.is_target_2d and self.num_classes >= 2 else None
             for features, target in self.test_loader:
                 features = features.to(self.device)
                 target = target.to(self.device)            
                 outputs = self.model(features)
-                if self.num_classes >= 2:
+                if not self.is_target_2d and self.num_classes >= 2:
                     _, predicted = torch.max(outputs.data, 1)
                     for index, value in enumerate(predicted):
                         self.correct_class[self.unique[value]][1] += 1 # record total numbers of each class
                         self.correct_class[self.unique[value]][0] += (value == target[index]).item() # record total true numbers of each class
                     correct += (predicted == target).sum().item()
                 self.test_loss += self.criterion(outputs, target)
             self.test_loss /= test_loader_step
             print('loss of {0} on the {1} test dataset: {2}. accuracy: {3:.4f} %'.format(self.__class__.__name__, test_total, self.test_loss.item(), 100 * correct / test_total))
         return OrderedDict(self._packing(sort_by, sort_state))
     
     def save(self, show: bool=True, dir: str='./model') -> None:
         '''
-        Save Model Checkpoint with Box, Regressier, Binarier, and Multipler.
+        Save Model Checkpoint with Box, Regressier, Binarier, Multipler, and Ranker.
         :param show: bool, whether to show `model.state_dict()`. default: True.
         :param dir: str, model save to dir. default: './model'.
         '''
         if show:
             print(self.model.state_dict())
         torch.save(self.model.state_dict(), dir)
 
     def load(self, show: bool=True, dir: str='./model') -> None:
         '''
-        Load Model Checkpoint with Box, Regressier, Binarier, and Multipler.
+        Load Model Checkpoint with Box, Regressier, Binarier, Multipler, and Ranker.
         :param show: bool, whether to show `model.state_dict()`. default: True.
         :param dir: str, model load from dir. default: './model'.
         '''
         params = torch.load(dir)
         self.model.load_state_dict(params)
         if show:
             print(self.model.state_dict())
 
     def _packing(self, by: str, state: bool) -> Dict[str, Any]:
         '''
         Pack Test Returned Data including `correct_class` and returned result of `sorted`.
         :param by: str, choose which way to sort the order of 'correct_class'.
         :param state: bool, choose the state when `correct_class` is sorting.
         '''
-        loss_, classify, regress = {
+        loss_, classify, regress, outputs = {
             'loss': {'train': self.train_loss.item(), 
                      'val': self.val_loss.item(),
                      'test': self.test_loss.item()}
         }, {'problem': 'classification',
             'num_classes': self.num_classes,
             'column': ('label name', ('true numbers', 'total numbers')),
-            'labels': self.correct_class}, {'problem': 'regression'}
-        if self.num_classes >= 2:
+            'labels': self.correct_class}, {'problem': 'regression'}, {'problem': 'multi-outputs'}
+        if not self.is_target_2d and self.num_classes >= 2:
             classify.update(loss_)
             if by == 'numbers':
                 classify.update({'sorted': sorted(self.correct_class.items(), key=lambda d: d[1][0], reverse=state)})
                 return classify
             elif by == 'accuracy':
                 classify.update({'sorted': sorted(self.correct_class.items(), key=lambda d: d[1][0]/d[1][1], reverse=state)})
                 return classify
             elif by == 'num-total':
                 classify.update({'sorted': sorted(self.correct_class.items(), key=lambda d: (d[1][0], d[1][1]), reverse=state)})
                 return classify
             else:
                 raise ValueError("`lambda` Caused with `by` Configuration Supports: numbers, accuracy, num-total.")
         else:
-            regress.update(loss_)
-            return regress
+            if self.is_target_2d:
+                outputs.update(loss_)
+                return outputs # Multi-outputs
+            else:
+                regress.update(loss_)
+                return regress
 
     def _set_container(self, backend: str, n_jobs: int) -> None:
         '''
         Acquire Validation Container with `parallel_backend` at `n_jobs`.
         :param backend: str, "threading", "multiprocessing, 'locky'.
         :param n_jobs: int, set jobs with backend to accelerate process.
         '''
```

## perming/common.py

```diff
@@ -35,15 +35,15 @@
                                          solver, 
                                          batch_size, 
                                          learning_rate_init, 
                                          lr_scheduler)
 
     def _activate(self, activation: str):
         '''
-        Configure Activation with `activation` and `inplace_on`.
+        Configure Activation with `activation` and `inplace=True`.
         :param activation: str, "relu", "rrelu", "leaky_relu", "elu", "celu". default: 'relu'.
         '''
         if activation == 'relu':
             return torch.nn.ReLU(inplace=True)
         elif activation == 'rrelu':
             return torch.nn.RReLU(inplace=True)
         elif activation == 'leaky_relu':
@@ -103,15 +103,15 @@
                                        solver, 
                                        batch_size, 
                                        learning_rate_init, 
                                        lr_scheduler)
 
     def _activate(self, activation: str):
         '''
-        Configure Activation with `activation` and `inplace_on`.
+        Configure Activation with `activation` and `inplace=True`.
         :param activation: str, "relu", "tanh", "sigmoid", "rrelu", "leaky_relu", "elu", "celu".
         '''
         if activation == 'relu':
             return torch.nn.ReLU(inplace=True)
         elif activation == 'tanh':
             return torch.nn.Tanh()
         elif activation == 'sigmoid':
@@ -171,19 +171,19 @@
                                        torch.device("cuda" if torch.cuda.is_available() else "cpu"), 
                                        self._activate(activation), 
                                        self._criterion(criterion), 
                                        solver, 
                                        batch_size, 
                                        learning_rate_init, 
                                        lr_scheduler)
-        assert num_classes >= 2, "The predefined options of Multipler are more suitable for Multi-classification problems."
+        assert num_classes >= 2, "The predefined options of Multipler are more suitable for Multi-classification."
 
     def _activate(self, activation: str):
         '''
-        Configure Activation with `activation` and `inplace_on`.
+        Configure Activation with `activation` and `inplace=True`.
         :param activation: str, "relu", "rrelu", "leaky_relu", "elu", "celu".
         '''
         if activation == 'relu':
             return torch.nn.ReLU(inplace=True)
         elif activation == 'rrelu':
             return torch.nn.RReLU(inplace=True)
         elif activation == 'leaky_relu':
@@ -194,15 +194,84 @@
             return torch.nn.CELU(inplace=True)
         else:
             raise ValueError("Activation Function Supports Options: relu, rrelu, leaky_relu, elu, celu.")
 
     def _criterion(self, criterion: str):
         '''
         Configure Loss Criterion with `criterion`.
-        :param criterion: str, "CrossEntropyLoss", "NLLLoss", "BCELoss", "BCEWithLogitsLoss", "MultiLabelMarginLoss", "MSELoss", "L1Loss", "SmoothL1Loss", "KLDivLoss". default: CrossEntropyLoss.
+        :param criterion: str, "CrossEntropyLoss", "NLLLoss".
         '''
         if criterion == 'CrossEntropyLoss':
             return torch.nn.CrossEntropyLoss()
         elif criterion == 'NLLLoss':
             return torch.nn.NLLLoss()
         else:
-            raise ValueError("Criterion Configuration Supports Options: CrossEntropyLoss, NLLLoss.")
+            raise ValueError("Criterion Configuration Supports Options: CrossEntropyLoss, NLLLoss.")
+        
+class Ranker(BaseModel):
+    '''
+    Supervised Learning Outputs Ranker for Tabular Data.
+    :param input_: int, features' dimension of tabular data is input_.
+    :param num_outputs: int, total number of correct label outputs.
+    :param hidden_layer_sizes: Tuple[int], configure the size of each hidden layer. default: (100,).
+    :param activation: str, configure function that activates the hidden layer. default: relu.
+    :param inplace_on: bool, whether to use `inplace=True` on activation. default: False.
+    :param criterion: str, loss function determined by different learning problem. default: MultiLabelSoftMarginLoss.
+    :param solver: str, optimization function coordinated with `torch.optim.lr_scheduler`. default: adam.
+    :param batch_size: int, batch size of dataset in one training process. default: 32.
+    :param learning_rate_init: float, initialize the learning rate of the optimizer. default: 1e-2.
+    :param lr_scheduler: str | None, set the learning rate scheduler integrated with the optimizer. default: None.
+    '''
+    def __init__(self, 
+                 input_: int, 
+                 num_outputs: int,
+                 hidden_layer_sizes: Tuple[int]=(100,),
+                 *,
+                 activation: str='relu', 
+                 criterion: str='MultiLabelSoftMarginLoss',
+                 solver: str='adam', 
+                 batch_size: int=32, 
+                 learning_rate_init: float=1e-2,
+                 lr_scheduler: Optional[str]=None) -> None:
+
+        super(Ranker, self).__init__(input_, 
+                                     num_outputs, 
+                                     hidden_layer_sizes, 
+                                     torch.device("cuda" if torch.cuda.is_available() else "cpu"), 
+                                     self._activate(activation), 
+                                     self._criterion(criterion),
+                                     solver, 
+                                     batch_size, 
+                                     learning_rate_init, 
+                                     lr_scheduler)
+
+    def _activate(self, activation: str):
+        '''
+        Configure Activation with `activation` and `inplace=True`.
+        :param activation: str, "relu", "rrelu", "leaky_relu", "elu", "celu".
+        '''
+        if activation == 'relu':
+            return torch.nn.ReLU(inplace=True)
+        elif activation == 'rrelu':
+            return torch.nn.RReLU(inplace=True)
+        elif activation == 'leaky_relu':
+            return torch.nn.LeakyReLU(inplace=True)
+        elif activation == 'elu':
+            return torch.nn.ELU(inplace=True)
+        elif activation == 'celu':
+            return torch.nn.CELU(inplace=True)
+        else:
+            raise ValueError("Activation Function Supports Options: relu, rrelu, leaky_relu, elu, celu.")
+
+    def _criterion(self, criterion: str):
+        '''
+        Configure Loss Criterion with `criterion`.
+        :param criterion: str, "MultiLabelMarginLoss", "BCEWithLogitsLoss", "MSELoss". default: MultiLabelMarginLoss
+        '''
+        if criterion == 'MultiLabelSoftMarginLoss': # np.array([[0, 1], [1, 1]])
+            return torch.nn.MultiLabelSoftMarginLoss()
+        elif criterion == 'BCEWithLogitsLoss': # np.array([[0.0, 1.0], [1.0, 1.0]])
+            return torch.nn.BCEWithLogitsLoss()
+        elif criterion == 'MSELoss': # np.array([[1.5, 2.0],[3.0, 1.6]])
+            return torch.nn.MSELoss()
+        else:
+            raise ValueError("Criterion Configuration Supports Options: MultiLabelSoftMarginLoss, BCEWithLogitsLoss, MSELoss.")
```

## perming/general.py

```diff
@@ -81,27 +81,29 @@
             return torch.nn.CELU(inplace=inplace_on)
         else:
             raise ValueError("Activation Function Supports Options: relu, tanh, sigmoid, rrelu, leaky_relu, softplus, elu, celu.")
 
     def _criterion(self, criterion: str):
         '''
         Configure Loss Criterion with `criterion`.
-        :param criterion: str, "CrossEntropyLoss", "NLLLoss", "BCELoss", "BCEWithLogitsLoss", "MultiLabelMarginLoss", "MSELoss", "L1Loss", "SmoothL1Loss", "KLDivLoss". default: CrossEntropyLoss.
+        :param criterion: str, "CrossEntropyLoss", "NLLLoss", "MultiLabelMarginLoss", "BCELoss", "BCEWithLogitsLoss", "MSELoss", "L1Loss", "SmoothL1Loss", "KLDivLoss". default: CrossEntropyLoss.
         '''
         if criterion == 'CrossEntropyLoss': # classification with num_classes > 2.
             return torch.nn.CrossEntropyLoss()
         elif criterion == 'NLLLoss':
             return torch.nn.NLLLoss()
+        elif criterion == 'MultiLabelSoftMarginLoss':
+            return torch.nn.MultiLabelSoftMarginLoss()
         elif criterion == 'BCELoss': # classification with num_classes = 2
             return torch.nn.BCELoss()
         elif criterion == 'BCEWithLogitsLoss':
             return torch.nn.BCEWithLogitsLoss()
         elif criterion == 'MSELoss': # regression
             return torch.nn.MSELoss()
         elif criterion == 'L1Loss':
             return torch.nn.L1Loss()
         elif criterion == 'SmoothL1Loss':
             return torch.nn.SmoothL1Loss()
         elif criterion == 'KLDivLoss':
             return torch.nn.KLDivLoss()
         else:
-            raise ValueError("Criterion Configuration Supports Options: CrossEntropyLoss, NLLLoss, BCELoss, BCEWithLogitsLoss, MultiLabelMarginLoss, MSELoss, L1Loss, SmoothL1Loss, KLDivLoss.") 
+            raise ValueError("Criterion Configuration Supports Options: CrossEntropyLoss, NLLLoss, MultiLabelSoftMarginLoss, BCELoss, BCEWithLogitsLoss, MSELoss, L1Loss, SmoothL1Loss, KLDivLoss.")
```

## Comparing `perming-1.2.1.dist-info/METADATA` & `perming-1.3.0.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perming
-Version: 1.2.1
+Version: 1.3.0
 Summary: The supervised learning framework based on perceptron for tabular data.
 Home-page: https://github.com/linjing-lab/easy-pytorch/tree/main/released_box
 Download-URL: https://github.com/linjing-lab/easy-pytorch/tags
 Author: 林景
 Author-email: linjing010729@163.com
 License: MPL 2.0
 Project-URL: Source, https://github.com/linjing-lab/easy-pytorch/tree/main/released_box/perming
@@ -87,14 +87,25 @@
 |`__init__`|input_: int<br />num_classes: int<br />hidden_layer_sizes: Tuple[int]=(100,)*<br /><br />activation: str="relu"<br />criterion: str="CrossEntropyLoss"<br />solver: str="adam"<br />batch_size: int=32<br />learning_rate_init: float=1e-2<br />lr_scheduler: Optional[str]=None|Initialize Classifier Based on Basic Information of the Classification Dataset Obtained through Data Preprocessing and Feature Engineering with `num_classes>2`.|
 |print_config|/|Return Initialized Parameters of Multi-layer Perceptron and Graph.|
 |train_val|num_epochs: int=2<br />interval: int=100<br />backend: str="threading"<br />n_jobs: int=-1|Using `ratio_set` and `worker_set` to Load the Regression Dataset with Numpy format into `torch.utils.data.DataLoader`.|
 |test|sort_by: str="accuracy"<br />sort_state: bool=True|Sort Returned Test Result about Correct Classes with `sort_by` and `sort_state` Which Only Appears in Classification.|
 |save|show: bool=True<br />dir: str='./model'|Save Trained Model Parameters with Model `state_dict` Control by `show`.|
 |load|show: bool=True<br />dir: str='./model'|Load Trained Model Parameters with Model `state_dict` Control by `show`.|
 
+- Multi-outputs
+
+|Ranker|Parameters|Meaning|
+|--|--|--|
+|`__init__`|input_: int<br />num_outputs: int<br />hidden_layer_sizes: Tuple[int]=(100,)*<br /><br />activation: str="relu"<br />criterion: str="MultiLabelSoftMarginLoss"<br />solver: str="adam"<br />batch_size: int=32<br />learning_rate_init: float=1e-2<br />lr_scheduler: Optional[str]=None|Initialize Ranker Based on Basic Information of the Classification Dataset Obtained through Data Preprocessing and Feature Engineering with (n_samples, n_outputs).|
+|print_config|/|Return Initialized Parameters of Multi-layer Perceptron and Graph.|
+|train_val|num_epochs: int=2<br />interval: int=100<br />backend: str="threading"<br />n_jobs: int=-1|Using `ratio_set` and `worker_set` to Load the Regression Dataset with Numpy format into `torch.utils.data.DataLoader`.|
+|test|sort_by: str="accuracy"<br />sort_state: bool=True|Sort Returned Test Result about Correct Classes with `sort_by` and `sort_state` Which Only Appears in Classification.|
+|save|show: bool=True<br />dir: str='./model'|Save Trained Model Parameters with Model `state_dict` Control by `show`.|
+|load|show: bool=True<br />dir: str='./model'|Load Trained Model Parameters with Model `state_dict` Control by `show`.|
+
 ## pip install
 
 download latest version:
 ```text
 git clone https://github.com/linjing-lab/easy-pytorch.git
 cd easy-pytorch/released_box
 pip install -e . --verbose
```

## Comparing `perming-1.2.1.dist-info/RECORD` & `perming-1.3.0.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-perming/__init__.py,sha256=C0QBZ1-KILgGvlTx7VU7xme7SZxS3Tkj3j-IK0RtLqM,850
+perming/__init__.py,sha256=4aona4mDIp6VRzAJBa7iz4nRP9-yd77_Ypff0KvQNRY,887
 perming/_typing.py,sha256=SGQP3QKfMZr-ciHT6jIrv4NUDmgqkx-RhYxIQloBSC4,176
-perming/_utils.py,sha256=_ma8mQ9ByXhVeKDW-Y65VI1Dq82N7pziYHN20oRgi14,20070
+perming/_utils.py,sha256=HPF94TnQlIiGBw4Tlk8qhwF35W-g7lAGK5tyzww7G_0,20745
 perming/_version.py,sha256=K3CPQxLgHmXPNpNWlhpnrp6Bt8v5rU9wZyVRBsRTI3E,568
-perming/common.py,sha256=wahlru3fczkyPbbiYkxcSyMGbj1_1py50w4LN-CS7qI,10505
-perming/general.py,sha256=I_dljULlKZ1yXy9frZysVxKKaJBx1LIGb3IznFH8c_g,5490
-perming-1.2.1.dist-info/METADATA,sha256=Lbrj4fbSsRFw54pY6NDqTA0cQts45AqcJVril_6rjMk,7523
-perming-1.2.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-perming-1.2.1.dist-info/top_level.txt,sha256=mxFGHPJW81IzoNdyMqNWWZA7gUBzz0RtiAw5cQ0qzX8,8
-perming-1.2.1.dist-info/RECORD,,
+perming/common.py,sha256=pOz6zWTF7cULulskyt3AGnoRj3P9kCLQUrECGwEaomM,14049
+perming/general.py,sha256=V2ZzelsVUeuDvp6zA44kCguSthncCoKmf-Hh5iKyTws,5605
+perming-1.3.0.dist-info/METADATA,sha256=0_jdJOlAZkezFjUyUKegLWg6Y_v13tHqFiVyf8KRNdM,8772
+perming-1.3.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+perming-1.3.0.dist-info/top_level.txt,sha256=mxFGHPJW81IzoNdyMqNWWZA7gUBzz0RtiAw5cQ0qzX8,8
+perming-1.3.0.dist-info/RECORD,,
```

