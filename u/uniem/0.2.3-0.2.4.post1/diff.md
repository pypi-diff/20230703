# Comparing `tmp/uniem-0.2.3.tar.gz` & `tmp/uniem-0.2.4.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uniem-0.2.3.tar", max compression
+gzip compressed data, was "uniem-0.2.4.post1.tar", max compression
```

## Comparing `uniem-0.2.3.tar` & `uniem-0.2.4.post1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2023-06-21 03:51:44.156512 uniem-0.2.3/LICENSE
--rw-r--r--   0        0        0     5876 2023-06-21 03:51:44.156512 uniem-0.2.3/README.md
--rw-r--r--   0        0        0      793 2023-06-21 03:51:44.168511 uniem-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      104 2023-06-21 03:51:44.264500 uniem-0.2.3/uniem/__init__.py
--rw-r--r--   0        0        0     7166 2023-06-21 03:51:44.264500 uniem-0.2.3/uniem/criteria.py
--rw-r--r--   0        0        0    10992 2023-06-21 03:51:44.264500 uniem-0.2.3/uniem/data.py
--rw-r--r--   0        0        0     1109 2023-06-21 03:51:44.264500 uniem-0.2.3/uniem/data_structures.py
--rw-r--r--   0        0        0    14138 2023-06-21 03:51:44.264500 uniem-0.2.3/uniem/finetuner.py
--rw-r--r--   0        0        0    13796 2023-06-21 03:51:44.264500 uniem-0.2.3/uniem/model.py
--rw-r--r--   0        0        0     6025 2023-06-21 03:51:44.264500 uniem-0.2.3/uniem/trainer.py
--rw-r--r--   0        0        0      658 2023-06-21 03:51:44.264500 uniem-0.2.3/uniem/types.py
--rw-r--r--   0        0        0     1663 2023-06-21 03:51:44.264500 uniem-0.2.3/uniem/utils.py
--rw-r--r--   0        0        0       22 2023-06-21 03:51:44.264500 uniem-0.2.3/uniem/version.py
--rw-r--r--   0        0        0     6511 1970-01-01 00:00:00.000000 uniem-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-03 08:22:19.445050 uniem-0.2.4.post1/LICENSE
+-rw-r--r--   0        0        0     5876 2023-07-03 08:22:19.445050 uniem-0.2.4.post1/README.md
+-rw-r--r--   0        0        0      799 2023-07-03 08:22:19.457049 uniem-0.2.4.post1/pyproject.toml
+-rw-r--r--   0        0        0      104 2023-07-03 08:22:19.553048 uniem-0.2.4.post1/uniem/__init__.py
+-rw-r--r--   0        0        0     7166 2023-07-03 08:22:19.553048 uniem-0.2.4.post1/uniem/criteria.py
+-rw-r--r--   0        0        0    10992 2023-07-03 08:22:19.553048 uniem-0.2.4.post1/uniem/data.py
+-rw-r--r--   0        0        0     1109 2023-07-03 08:22:19.553048 uniem-0.2.4.post1/uniem/data_structures.py
+-rw-r--r--   0        0        0    14799 2023-07-03 08:22:19.553048 uniem-0.2.4.post1/uniem/finetuner.py
+-rw-r--r--   0        0        0    14611 2023-07-03 08:22:19.553048 uniem-0.2.4.post1/uniem/model.py
+-rw-r--r--   0        0        0     6025 2023-07-03 08:22:19.553048 uniem-0.2.4.post1/uniem/trainer.py
+-rw-r--r--   0        0        0      658 2023-07-03 08:22:19.553048 uniem-0.2.4.post1/uniem/types.py
+-rw-r--r--   0        0        0     4675 2023-07-03 08:22:19.553048 uniem-0.2.4.post1/uniem/utils.py
+-rw-r--r--   0        0        0       22 2023-07-03 08:22:19.553048 uniem-0.2.4.post1/uniem/version.py
+-rw-r--r--   0        0        0     6517 1970-01-01 00:00:00.000000 uniem-0.2.4.post1/PKG-INFO
```

### Comparing `uniem-0.2.3/LICENSE` & `uniem-0.2.4.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `uniem-0.2.3/README.md` & `uniem-0.2.4.post1/README.md`

 * *Files identical despite different names*

### Comparing `uniem-0.2.3/pyproject.toml` & `uniem-0.2.4.post1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "uniem"
-version = "0.2.3"
+version = "0.2.4.post1"
 description = "unified embedding model"
 authors = ["wangyuxin <wangyuxin@mokahr.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `uniem-0.2.3/uniem/criteria.py` & `uniem-0.2.4.post1/uniem/criteria.py`

 * *Files identical despite different names*

### Comparing `uniem-0.2.3/uniem/data.py` & `uniem-0.2.4.post1/uniem/data.py`

 * *Files identical despite different names*

### Comparing `uniem-0.2.3/uniem/data_structures.py` & `uniem-0.2.4.post1/uniem/data_structures.py`

 * *Files identical despite different names*

### Comparing `uniem-0.2.3/uniem/finetuner.py` & `uniem-0.2.4.post1/uniem/finetuner.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 import logging
 import os
 from pathlib import Path
 from typing import Sequence, cast
 
 import torch
 from accelerate import Accelerator
-from accelerate.utils import ProjectConfiguration, set_seed
+from accelerate.tracking import GeneralTracker
+from accelerate.utils import LoggerType, ProjectConfiguration, set_seed
 from datasets import Dataset as HFDataset
 from datasets import DatasetDict as HFDatasetDict
 from torch.utils.data import DataLoader
 from transformers import AutoTokenizer, get_cosine_schedule_with_warmup  # type: ignore
 
 from uniem.data import (
     FinetuneDataset,
@@ -26,20 +27,34 @@
     EmbedderForTrain,
     EmbedderForTripletInBatchNegTrain,
     InBatchNegLossType,
     PoolingStrategy,
 )
 from uniem.trainer import Trainer
 from uniem.types import MixedPrecisionType
-from uniem.utils import create_adamw_optimizer, split_dataset_dict
+from uniem.utils import create_adamw_optimizer, find_executable_batch_size, split_dataset_dict
 
 logger = logging.getLogger(__name__)
 RawDataset = Sequence[dict] | dict[str, Sequence[dict]] | HFDatasetDict | HFDataset
 
 
+def suggest_lr(model_name: str) -> float:
+    default_lr = 3e-5
+    if 'm3e-small' in model_name:
+        lr = 1e-4
+    elif 'm3e-base' in model_name:
+        lr = 5e-5
+    elif 'm3e-large' in model_name:
+        lr = 8e-6
+    else:
+        lr = default_lr
+    logger.info(f'Suggested learning rate: {lr}')
+    return lr
+
+
 class FineTuner:
     def __init__(
         self,
         model_name_or_path: str,
         dataset: RawDataset,
         record_type: RecordType | str | None = None,
     ):
@@ -133,53 +148,56 @@
                 model = EmbedderForScoredPairTrain(
                     model_name_or_path=self.model_name_or_path,
                     temperature=temperature,
                     embedding_strategy=embedding_strategy,
                 )
         return model
 
+    @find_executable_batch_size(starting_batch_size=256)
     def run(
         self,
         temperature: float | None = None,
         embedding_strategy: PoolingStrategy = PoolingStrategy.last_mean,
-        batch_size: int = 32,
+        lr: float | None = None,
         drop_last: bool = True,
         max_length: int = 512,
-        lr: float = 3e-5,
         weight_decay: float = 1e-3,
         num_warmup_steps: float = 0.05,
+        batch_size: int = 256,
         epochs: int = 3,
         mixed_precision: MixedPrecisionType = MixedPrecisionType.no,
         gradient_accumulation_steps: int = 1,
         save_on_epoch_end: bool = False,
         num_max_checkpoints: int = 1,
-        use_tensorboard: bool = False,
+        log_with: str | LoggerType | GeneralTracker | list[str | LoggerType | GeneralTracker] | None = None,
         num_workers: int = 0,
         seed: int = 42,
         output_dir: Path | str | None = None,
     ):
+
         os.environ.setdefault('TRANSFORMERS_NO_ADVISORY_WARNINGS', '1')
         if num_workers >= 1:
             os.environ.setdefault('TOKENIZERS_PARALLELISM', 'false')
 
         output_dir = Path(output_dir) if output_dir is not None else Path('finetuned-model')
         project_config = ProjectConfiguration(
             project_dir=str(output_dir),
             automatic_checkpoint_naming=True,
             total_limit=num_max_checkpoints,
         )
         accelerator = Accelerator(
             mixed_precision=mixed_precision.value,
             gradient_accumulation_steps=gradient_accumulation_steps,
             project_config=project_config,
-            log_with=['tensorboard'] if use_tensorboard else None,
+            log_with=log_with,
         )
         accelerator.init_trackers('uniem')
 
         set_seed(seed)
+        accelerator.print(batch_size)
         accelerator.print(f'Start with seed: {seed}')
         accelerator.print(f'Output dir: {output_dir}')
 
         train_dataloader, validation_dataloader = self.create_dataloaders(
             batch_size=batch_size,
             drop_last=drop_last,
             max_length=max_length,
@@ -189,14 +207,15 @@
         validation_dataloader = accelerator.prepare(validation_dataloader) if validation_dataloader is not None else None
 
         model = self.create_finetune_model(temperature=temperature, embedding_strategy=embedding_strategy)
         model.embedder.encoder.config.pad_token_id = self.tokenizer.pad_token_id
         model = accelerator.prepare(model)
 
         # Optimizer & LRScheduler
+        lr = lr or suggest_lr(self.model_name_or_path)
         optimizer = create_adamw_optimizer(model, lr=lr, weight_decay=weight_decay)
         total_steps = len(train_dataloader) * epochs
         if num_warmup_steps < 1:
             num_warmup_steps = int(num_warmup_steps * total_steps)
         lr_scheduler = get_cosine_schedule_with_warmup(
             optimizer=optimizer,
             num_warmup_steps=int(num_warmup_steps),
@@ -279,19 +298,20 @@
                 param.requires_grad = False
             embedding_layer_weight = model.embedder.encoder.get_input_embeddings().weight
             embedding_layer_weight = cast(torch.nn.Parameter, embedding_layer_weight)
             embedding_layer_weight.requires_grad = True
             embedding_layer_weight.register_hook(hook)
         return model
 
+    @find_executable_batch_size(starting_batch_size=256)
     def run(
         self,
         temperature: float | None = None,
         embedding_strategy: PoolingStrategy = PoolingStrategy.last_mean,
-        batch_size: int = 32,
+        batch_size: int = 256,
         drop_last: bool = True,
         max_length: int = 512,
         lr: float = 1e-2,
         epochs: int = 5,
         mixed_precision: MixedPrecisionType = MixedPrecisionType.no,
         gradient_accumulation_steps: int = 1,
         save_on_epoch_end: bool = False,
```

### Comparing `uniem-0.2.3/uniem/model.py` & `uniem-0.2.4.post1/uniem/model.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+import importlib
 from enum import Enum
 from pathlib import Path
 from typing import ClassVar, Literal, Type, TypeVar, cast
 
 import numpy as np
 import torch
 import tqdm
-from transformers import AutoConfig, AutoModel, AutoTokenizer, PreTrainedModel  # type: ignore
+from transformers import AutoModel, AutoTokenizer, PreTrainedModel  # type: ignore
 
 from uniem.criteria import (
     CoSentLoss,
     PairInBatchNegCoSentLoss,
     PairInBatchNegSigmoidContrastLoss,
     PairInBatchNegSoftmaxContrastLoss,
     TripletInBatchNegCoSentLoss,
@@ -32,34 +33,37 @@
 
 class InBatchNegLossType(str, Enum):
     sigmoid = 'sigmoid'
     softmax = 'softmax'
     cosent = 'cosent'
 
 
-def creat_mask_from_input_ids(input_ids: torch.Tensor, pad_token_id: int) -> torch.Tensor:
+def creat_attention_mask_from_input_ids(input_ids: torch.Tensor, pad_token_id: int) -> torch.Tensor:
     return input_ids != pad_token_id
 
 
-def mean_pooling(hidden_state: torch.Tensor, mask: torch.Tensor | None = None) -> torch.Tensor:
-    if mask is None:
+def mean_pooling(hidden_state: torch.Tensor, attention_mask: torch.Tensor | None = None) -> torch.Tensor:
+    if attention_mask is None:
         return torch.mean(hidden_state, dim=1)
-    mask = mask.float()
-    return torch.sum(hidden_state * mask.unsqueeze(-1), dim=1) / torch.sum(mask, dim=-1, keepdim=True)
+    attention_mask = attention_mask.float()
+    return torch.sum(hidden_state * attention_mask.unsqueeze(-1), dim=1) / torch.sum(attention_mask, dim=-1, keepdim=True)
 
 
-def load_hf_pretrained_model(model_name_or_path: str) -> PreTrainedModel:
-    config = AutoConfig.from_pretrained(model_name_or_path)
-    if config.model_type == 't5':
-        from transformers import T5EncoderModel  # type: ignore
-
-        pretrained_model = T5EncoderModel.from_pretrained(model_name_or_path)
-    else:
-        pretrained_model = AutoModel.from_pretrained(model_name_or_path)
-    return pretrained_model  # type: ignore
+def load_hf_pretrained_model(
+    model_name_or_path: str, model_class: str | None | Type[PreTrainedModel] | Type[AutoModel] = None
+) -> PreTrainedModel:
+    if model_class is None:
+        model_class = AutoModel
+    elif isinstance(model_class, str):
+        transformers_module = importlib.import_module('transformers')
+        model_class = getattr(transformers_module, model_class)
+
+    model = model_class.from_pretrained(model_name_or_path)  # type: ignore
+    model = cast(PreTrainedModel, model)
+    return model
 
 
 StrategyEmbedderClsMap: dict[PoolingStrategy, Type['Embedder']] = {}
 
 
 class Embedder(torch.nn.Module):
     pooling_strategy: ClassVar[PoolingStrategy]
@@ -95,73 +99,77 @@
     def max_length(self):
         return self.encoder.config.max_position_embeddings
 
 
 class LastMeanEmbedder(Embedder):
     pooling_strategy: ClassVar[PoolingStrategy] = PoolingStrategy.last_mean
 
-    def forward(self, input_ids: torch.Tensor, mask: torch.Tensor | None = None) -> torch.Tensor:
-        if mask is None:
-            mask = creat_mask_from_input_ids(input_ids, self.pad_token_id)
-        embeddings = self.encoder(input_ids).last_hidden_state
-        embeddings = mean_pooling(embeddings, mask)
+    def forward(self, input_ids: torch.Tensor, attention_mask: torch.Tensor | None = None) -> torch.Tensor:
+        if attention_mask is None:
+            attention_mask = creat_attention_mask_from_input_ids(input_ids, self.pad_token_id)
+        embeddings = self.encoder(input_ids, attention_mask=attention_mask).last_hidden_state
+        embeddings = mean_pooling(embeddings, attention_mask)
         return embeddings
 
 
 class ClsEmbedder(Embedder):
     pooling_strategy: ClassVar[PoolingStrategy] = PoolingStrategy.cls
 
-    def forward(self, input_ids: torch.Tensor, mask: torch.Tensor | None = None) -> torch.Tensor:
-        embeddings = self.encoder(input_ids).last_hidden_state[:, 0]
+    def forward(self, input_ids: torch.Tensor, attention_mask: torch.Tensor | None = None) -> torch.Tensor:
+        if attention_mask is None:
+            attention_mask = creat_attention_mask_from_input_ids(input_ids, self.pad_token_id)
+        embeddings = self.encoder(input_ids, attention_mask=attention_mask).last_hidden_state[:, 0]
         return embeddings
 
 
 class FirstLastEmbedder(Embedder):
     pooling_strategy: ClassVar[PoolingStrategy] = PoolingStrategy.first_last_mean
 
-    def forward(self, input_ids: torch.Tensor, mask: torch.Tensor | None = None) -> torch.Tensor:
-        if mask is None:
-            mask = creat_mask_from_input_ids(input_ids, self.pad_token_id)
-        embeddings = self.encoder(input_ids, output_hidden_states=True).hidden_states
-        first_embeddings = mean_pooling(embeddings[0], mask)
-        last_embeddings = mean_pooling(embeddings[-1], mask)
+    def forward(self, input_ids: torch.Tensor, attention_mask: torch.Tensor | None = None) -> torch.Tensor:
+        if attention_mask is None:
+            attention_mask = creat_attention_mask_from_input_ids(input_ids, self.pad_token_id)
+        embeddings = self.encoder(input_ids, attention_mask=attention_mask, output_hidden_states=True).hidden_states
+        first_embeddings = mean_pooling(embeddings[0], attention_mask)
+        last_embeddings = mean_pooling(embeddings[-1], attention_mask)
         embeddings = (first_embeddings + last_embeddings) / 2
         return embeddings
 
 
 class EmbeddingLastEmbedder(Embedder):
     pooling_strategy: ClassVar[PoolingStrategy] = PoolingStrategy.embedding_last_mean
 
     def __init__(self, encoder: PreTrainedModel, pad_token_id: int | None = None):
         super().__init__(encoder, pad_token_id)
         self.embedding_layer = self.encoder.get_input_embeddings()
 
-    def forward(self, input_ids: torch.Tensor, mask: torch.Tensor | None = None) -> torch.Tensor:
-        if mask is None:
-            mask = creat_mask_from_input_ids(input_ids, self.pad_token_id)
+    def forward(self, input_ids: torch.Tensor, attention_mask: torch.Tensor | None = None) -> torch.Tensor:
+        if attention_mask is None:
+            attention_mask = creat_attention_mask_from_input_ids(input_ids, self.pad_token_id)
         static_embeddings = self.embedding_layer(input_ids)
-        mean_last_embeddings = mean_pooling(self.encoder(input_ids).last_hidden_state, mask)
-        mean_static_embeddings = mean_pooling(static_embeddings, mask)
+        mean_last_embeddings = mean_pooling(
+            self.encoder(input_ids, attention_mask=attention_mask).last_hidden_state, attention_mask
+        )
+        mean_static_embeddings = mean_pooling(static_embeddings, attention_mask)
         return (mean_last_embeddings + mean_static_embeddings) / 2
 
 
 class LastWeightedEmbedder(Embedder):
     pooling_strategy: ClassVar[PoolingStrategy] = PoolingStrategy.last_weighted
 
     def __init__(self, encoder: PreTrainedModel, pad_token_id: int | None = None):
         super().__init__(encoder, pad_token_id)
         self.embedding_layer = self.encoder.get_input_embeddings()
 
-    def forward(self, input_ids: torch.Tensor, mask: torch.Tensor | None = None) -> torch.Tensor:
-        if mask is None:
-            mask = creat_mask_from_input_ids(input_ids, self.pad_token_id)
+    def forward(self, input_ids: torch.Tensor, attention_mask: torch.Tensor | None = None) -> torch.Tensor:
+        if attention_mask is None:
+            attention_mask = creat_attention_mask_from_input_ids(input_ids, self.pad_token_id)
         weights = (torch.arange(input_ids.shape[1], device=input_ids.device) + 1).float()
         embeddings = self.encoder(input_ids).last_hidden_state
-        embeddings = embeddings * mask.unsqueeze(-1).float() * weights.unsqueeze(0).unsqueeze(-1)
-        embeddings = torch.sum(embeddings, dim=1) / torch.sum(weights * mask, dim=-1, keepdim=True)
+        embeddings = embeddings * attention_mask.unsqueeze(-1).float() * weights.unsqueeze(0).unsqueeze(-1)
+        embeddings = torch.sum(embeddings, dim=1) / torch.sum(weights * attention_mask, dim=-1, keepdim=True)
         return embeddings
 
 
 class AutoEmbedder:
     @classmethod
     def from_pretrained(cls, model_name_or_path: str | Path):
         encoder = load_hf_pretrained_model(str(model_name_or_path))
@@ -183,19 +191,20 @@
         self.embedder = embedder
 
 
 class EmbedderForPairInBatchNegTrain(EmbedderForTrain):
     def __init__(
         self,
         model_name_or_path: str,
+        model_class: str | None = None,
         temperature: float | None = None,
         loss_type: InBatchNegLossType | str = InBatchNegLossType.softmax,
         embedding_strategy: PoolingStrategy | str = PoolingStrategy.last_mean,
     ):
-        pretrained_model = load_hf_pretrained_model(model_name_or_path)
+        pretrained_model = load_hf_pretrained_model(model_name_or_path, model_class=model_class)
         embedder = StrategyEmbedderClsMap[PoolingStrategy(embedding_strategy)](pretrained_model)
         super().__init__(embedder)
         temperature = temperature or 0.05
         self.loss_type = InBatchNegLossType(loss_type)
         match self.loss_type:
             case InBatchNegLossType.sigmoid:
                 self.criterion = PairInBatchNegSigmoidContrastLoss(temperature)
@@ -211,20 +220,21 @@
         return {'loss': loss}
 
 
 class EmbedderForTripletInBatchNegTrain(EmbedderForTrain):
     def __init__(
         self,
         model_name_or_path: str,
+        model_class: str | None = None,
         temperature: float | None = None,
         loss_type: InBatchNegLossType | str = InBatchNegLossType.softmax,
         embedding_strategy: PoolingStrategy | str = PoolingStrategy.last_mean,
         add_swap_loss: bool = False,
     ):
-        pretrained_model = load_hf_pretrained_model(model_name_or_path)
+        pretrained_model = load_hf_pretrained_model(model_name_or_path, model_class=model_class)
         embedder = StrategyEmbedderClsMap[PoolingStrategy(embedding_strategy)](pretrained_model)
         super().__init__(embedder)
         temperature = temperature or 0.05
         self.loss_type = InBatchNegLossType(loss_type)
         match self.loss_type:
             case InBatchNegLossType.sigmoid:
                 self.criterion = TripletInBatchNegSigmoidContrastLoss(temperature, add_swap_loss)
@@ -328,15 +338,15 @@
             input_ids = input_ids.to(self.embedder.encoder.device)
 
             attention_mask = encodes['attention_mask']
             attention_mask = cast(torch.Tensor, attention_mask)
             attention_mask = attention_mask.to(self.embedder.encoder.device)
 
             with torch.inference_mode():
-                batch_embeddings = self.embedder(input_ids, mask=attention_mask)
+                batch_embeddings = self.embedder(input_ids, attention_mask=attention_mask)
                 if self.normalize:
                     batch_embeddings = torch.nn.functional.normalize(batch_embeddings, dim=-1)
                 batch_embeddings = cast(torch.Tensor, batch_embeddings)
             embeddings.extend([i.cpu().numpy() for i in batch_embeddings])
         return embeddings
 
     def encode_single(self, sentence: str):
```

### Comparing `uniem-0.2.3/uniem/trainer.py` & `uniem-0.2.4.post1/uniem/trainer.py`

 * *Files identical despite different names*

### Comparing `uniem-0.2.3/uniem/types.py` & `uniem-0.2.4.post1/uniem/types.py`

 * *Files identical despite different names*

### Comparing `uniem-0.2.3/PKG-INFO` & `uniem-0.2.4.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uniem
-Version: 0.2.3
+Version: 0.2.4.post1
 Summary: unified embedding model
 License: MIT
 Author: wangyuxin
 Author-email: wangyuxin@mokahr.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

