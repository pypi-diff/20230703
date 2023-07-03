# Comparing `tmp/rannet-0.1.0.tar.gz` & `tmp/rannet-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rannet-0.1.0.tar", last modified: Thu Jun 22 12:38:33 2023, max compression
+gzip compressed data, was "rannet-0.2.0.tar", last modified: Mon Jul  3 12:47:49 2023, max compression
```

## Comparing `rannet-0.1.0.tar` & `rannet-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 seanlee    (501) staff       (20)        0 2023-06-22 12:38:33.651818 rannet-0.1.0/
--rw-r--r--   0 seanlee    (501) staff       (20)     1060 2023-06-21 14:32:33.000000 rannet-0.1.0/LICENSE
--rw-r--r--   0 seanlee    (501) staff       (20)     4782 2023-06-22 12:38:33.652073 rannet-0.1.0/PKG-INFO
--rw-r--r--   0 seanlee    (501) staff       (20)     4074 2023-06-22 12:31:29.000000 rannet-0.1.0/README.md
-drwxr-xr-x   0 seanlee    (501) staff       (20)        0 2023-06-22 12:38:33.647228 rannet-0.1.0/rannet/
--rw-r--r--   0 seanlee    (501) staff       (20)      323 2023-06-22 12:31:51.000000 rannet-0.1.0/rannet/__init__.py
--rw-r--r--   0 seanlee    (501) staff       (20)     9124 2023-06-22 12:31:29.000000 rannet-0.1.0/rannet/dataloader.py
--rw-r--r--   0 seanlee    (501) staff       (20)    24517 2023-06-22 12:31:29.000000 rannet-0.1.0/rannet/layers.py
--rw-r--r--   0 seanlee    (501) staff       (20)    17145 2023-06-22 12:31:29.000000 rannet-0.1.0/rannet/optimizer.py
--rw-r--r--   0 seanlee    (501) staff       (20)    14505 2023-06-22 12:31:29.000000 rannet-0.1.0/rannet/pretrain.py
--rw-r--r--   0 seanlee    (501) staff       (20)    29124 2023-06-22 12:31:29.000000 rannet-0.1.0/rannet/ran.py
--rw-r--r--   0 seanlee    (501) staff       (20)    24379 2023-06-22 12:31:29.000000 rannet-0.1.0/rannet/rannet.py
--rw-r--r--   0 seanlee    (501) staff       (20)     6394 2023-06-22 12:31:29.000000 rannet-0.1.0/rannet/tokenizer.py
--rw-r--r--   0 seanlee    (501) staff       (20)     1808 2023-06-22 12:31:29.000000 rannet-0.1.0/rannet/utils.py
-drwxr-xr-x   0 seanlee    (501) staff       (20)        0 2023-06-22 12:38:33.651192 rannet-0.1.0/rannet.egg-info/
--rw-r--r--   0 seanlee    (501) staff       (20)     4782 2023-06-22 12:38:33.000000 rannet-0.1.0/rannet.egg-info/PKG-INFO
--rw-r--r--   0 seanlee    (501) staff       (20)      377 2023-06-22 12:38:33.000000 rannet-0.1.0/rannet.egg-info/SOURCES.txt
--rw-r--r--   0 seanlee    (501) staff       (20)        1 2023-06-22 12:38:33.000000 rannet-0.1.0/rannet.egg-info/dependency_links.txt
--rw-r--r--   0 seanlee    (501) staff       (20)        1 2023-06-22 12:32:36.000000 rannet-0.1.0/rannet.egg-info/not-zip-safe
--rw-r--r--   0 seanlee    (501) staff       (20)       31 2023-06-22 12:38:33.000000 rannet-0.1.0/rannet.egg-info/requires.txt
--rw-r--r--   0 seanlee    (501) staff       (20)        7 2023-06-22 12:38:33.000000 rannet-0.1.0/rannet.egg-info/top_level.txt
--rw-r--r--   0 seanlee    (501) staff       (20)      163 2023-06-22 12:38:33.652899 rannet-0.1.0/setup.cfg
--rw-r--r--   0 seanlee    (501) staff       (20)     1395 2023-06-22 12:38:27.000000 rannet-0.1.0/setup.py
+drwxr-xr-x   0 seanlee    (501) staff       (20)        0 2023-07-03 12:47:49.317198 rannet-0.2.0/
+-rw-r--r--   0 seanlee    (501) staff       (20)     1060 2023-07-03 12:41:23.000000 rannet-0.2.0/LICENSE
+-rw-r--r--   0 seanlee    (501) staff       (20)     5559 2023-07-03 12:47:49.317706 rannet-0.2.0/PKG-INFO
+-rw-r--r--   0 seanlee    (501) staff       (20)     4851 2023-07-03 12:43:34.000000 rannet-0.2.0/README.md
+drwxr-xr-x   0 seanlee    (501) staff       (20)        0 2023-07-03 12:47:49.310972 rannet-0.2.0/rannet/
+-rw-r--r--   0 seanlee    (501) staff       (20)      323 2023-07-03 12:47:22.000000 rannet-0.2.0/rannet/__init__.py
+-rw-r--r--   0 seanlee    (501) staff       (20)     9124 2023-07-03 12:41:23.000000 rannet-0.2.0/rannet/dataloader.py
+-rw-r--r--   0 seanlee    (501) staff       (20)    24517 2023-07-03 12:41:23.000000 rannet-0.2.0/rannet/layers.py
+-rw-r--r--   0 seanlee    (501) staff       (20)    17145 2023-07-03 12:41:23.000000 rannet-0.2.0/rannet/optimizer.py
+-rw-r--r--   0 seanlee    (501) staff       (20)    14505 2023-07-03 12:41:23.000000 rannet-0.2.0/rannet/pretrain.py
+-rw-r--r--   0 seanlee    (501) staff       (20)    29604 2023-07-03 12:41:23.000000 rannet-0.2.0/rannet/ran.py
+-rw-r--r--   0 seanlee    (501) staff       (20)    25454 2023-07-03 12:44:13.000000 rannet-0.2.0/rannet/rannet.py
+-rw-r--r--   0 seanlee    (501) staff       (20)     6394 2023-07-03 12:41:23.000000 rannet-0.2.0/rannet/tokenizer.py
+-rw-r--r--   0 seanlee    (501) staff       (20)     1808 2023-07-03 12:41:23.000000 rannet-0.2.0/rannet/utils.py
+drwxr-xr-x   0 seanlee    (501) staff       (20)        0 2023-07-03 12:47:49.316002 rannet-0.2.0/rannet.egg-info/
+-rw-r--r--   0 seanlee    (501) staff       (20)     5559 2023-07-03 12:47:49.000000 rannet-0.2.0/rannet.egg-info/PKG-INFO
+-rw-r--r--   0 seanlee    (501) staff       (20)      377 2023-07-03 12:47:49.000000 rannet-0.2.0/rannet.egg-info/SOURCES.txt
+-rw-r--r--   0 seanlee    (501) staff       (20)        1 2023-07-03 12:47:49.000000 rannet-0.2.0/rannet.egg-info/dependency_links.txt
+-rw-r--r--   0 seanlee    (501) staff       (20)        1 2023-07-03 12:47:49.000000 rannet-0.2.0/rannet.egg-info/not-zip-safe
+-rw-r--r--   0 seanlee    (501) staff       (20)       31 2023-07-03 12:47:49.000000 rannet-0.2.0/rannet.egg-info/requires.txt
+-rw-r--r--   0 seanlee    (501) staff       (20)        7 2023-07-03 12:47:49.000000 rannet-0.2.0/rannet.egg-info/top_level.txt
+-rw-r--r--   0 seanlee    (501) staff       (20)      163 2023-07-03 12:47:49.319594 rannet-0.2.0/setup.cfg
+-rw-r--r--   0 seanlee    (501) staff       (20)     1395 2023-07-03 12:47:22.000000 rannet-0.2.0/setup.py
```

### Comparing `rannet-0.1.0/LICENSE` & `rannet-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rannet-0.1.0/PKG-INFO` & `rannet-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rannet
-Version: 0.1.0
+Version: 0.2.0
 Summary: Recurrent Attention Networks
 Author: sean lee
 Author-email: xmlee97@gmail.com
 Keywords: rannet
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -23,15 +23,18 @@
 <h4 align='center'> 📢 This project is still in the works in order to make long document modeling easier.</h4>
 
 <h4 align="center">
    <a href="https://github.com/4AI/RAN/blob/main/LICENSE">
       <img src="https://img.shields.io/badge/License-MIT-blue.svg?style=flat-square" alt="RAN is released under the MIT license." />
    </a>
    <a href="https://pypi.org/project/rannet/">
-      <img src="https://badge.fury.io/py/RAN.svg?style=flat-square" alt="PyPI version" />
+      <img src="https://img.shields.io/pypi/v/rannet?style=flat-square" alt="PyPI version" />
+   </a>
+   <a href="https://pypi.org/project/rannet/">
+      <img src="https://img.shields.io/pypi/dm/rannet?style=flat-square" alt="PyPI Downloads" />
    </a>
    <a href="http://makeapullrequest.com">
       <img src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square" alt="http://makeapullrequest.com" />
    </a>
    <a href="https://arxiv.org/abs/2306.06843">
       <img src="https://img.shields.io/badge/Arxiv-2306.06843-yellow.svg?style=flat-square" alt="https://arxiv.org/abs/2306.06843" />
    </a>
@@ -65,14 +68,39 @@
 | CN   |   [base](https://drive.google.com/file/d/1_gmrulSU-ln_jElc2hktPTTQDzaeG1wU/view?usp=sharing)  \| [small](https://drive.google.com/file/d/1D-FCxY_UMwZCkvcwl6hkRcl6VnCzRGIj/view?usp=sharing)         |        [base](https://pan.baidu.com/s/1WIcePgmqb7Ox0w1qigWQ_w)\[code: e47w\]  \| [small](https://pan.baidu.com/s/17DAboL9w0mArcBBuiy3tGg)\[code: mdmg\]        |
 
 
 # 🚀 Quick Tour
 
 ## 🈶 w/ pretrained models
 
+*Extract semantic feature*
+
+set `apply_cell_transform=False` to extract semantic feature.
+
+```python
+import numpy as np
+from rannet import RanNet, RanNetWordPieceTokenizer
+
+
+vocab_path = 'pretrained/vocab.txt'
+ckpt_path = 'pretrained/model.ckpt'
+config_path = 'pretrained/config.json'
+tokenizer = RanNetWordPieceTokenizer(vocab_path, lowercase=True)
+
+rannet, rannet_model = RanNet.load_rannet(
+    config_path=config_path,
+    checkpoint_path=ckpt_path,
+    return_sequences=False,
+    apply_cell_transform=False
+)
+text = 'input text'
+tok = tokenizer.encode(text)
+vec = rannet_model.predict(np.array([tok.ids]))
+```
+
 *For the classification task*
 
 ```python
 from rannet import RanNet, RanNetWordPieceTokenizer
 
 
 vocab_path = 'pretrained/vocab.txt'
@@ -97,15 +125,15 @@
 
 vocab_path = 'pretrained/vocab.txt'
 ckpt_path = 'pretrained/model.ckpt'
 config_path = 'pretrained/config.json'
 tokenizer = RanNetWordPieceTokenizer(vocab_path, lowercase=True)
 
 rannet, rannet_model = RanNet.load_rannet(
-    config_path=config_path, checkpoint_path=ckpt_path, return_cell=False)
+    config_path=config_path, checkpoint_path=ckpt_path, return_gpc=False)
 output = rannet_model.output  # (B, L, D)
 rannet_model.summary()
 ```
 
 ## 🈚 w/o pretrained models
 
 Embed the `RAN` (a Keras layer) into your network.
@@ -137,10 +165,10 @@
     author = "Li, Xianming and Li, Zongxi and Luo, Xiaotian and Xie, Haoran and Lee, Xing and Zhao, Yingbin and Wang, Fu Lee and Li, Qing",
     booktitle = "Findings of the Association for Computational Linguistics: ACL 2023",
     year = "2023",
     publisher = "Association for Computational Linguistics"
 }
 ```
 
-# Contact
+# 📬 Contact
 
 Please contact us at 1) for code problems, create a GitHub issue; 2) for paper problems, email xmlee97@gmail.com
```

#### html2text {}

```diff
@@ -1,55 +1,64 @@
-Metadata-Version: 2.1 Name: rannet Version: 0.1.0 Summary: Recurrent Attention
+Metadata-Version: 2.1 Name: rannet Version: 0.2.0 Summary: Recurrent Attention
 Networks Author: sean lee Author-email: xmlee97@gmail.com Keywords: rannet
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Description-Content-Type: text/markdown
 License-File: LICENSE
                 ****** RAN: Recurrent Attention Network ******
   *** ð¢ This project is still in the works in order to make long document
                              modeling easier. ***
-     *** [RAN_is_released_under_the_MIT_license.] [PyPI_version] [http://
-         makeapullrequest.com] [https://arxiv.org/abs/2306.06843] ***
+ *** [RAN_is_released_under_the_MIT_license.] [PyPI_version] [PyPI_Downloads]
+     [http://makeapullrequest.com] [https://arxiv.org/abs/2306.06843] ***
 # â¬ï¸ Installation *stable* ```bash python -m pip install -U rannet ```
 *latest* ```bash python -m pip install git+https://github.com/4AI/RAN.git ```
 *environment* - â­ tensorflow>2.0,<=2.10 ð¤ `export TF_KERAS=1` -
 tensorflow>=1.14,<2.0 ð¤ Keras==2.3.1 ## ðï¸ Pretrained Models | Lang |
 Google Drive | Baidu NetDrive | |------|--------------|----------------| | EN |
 [base](https://drive.google.com/file/d/1mRabw0Hy9T5_EWbZshD6Uk-bvauNzG9R/
 view?usp=sharing) | [base](https://pan.baidu.com/s/18uhAkY46aIcy4ncwzXp5mA)\
 [code: djkj\] | | CN | [base](https://drive.google.com/file/d/1_gmrulSU-
 ln_jElc2hktPTTQDzaeG1wU/view?usp=sharing) \| [small](https://drive.google.com/
 file/d/1D-FCxY_UMwZCkvcwl6hkRcl6VnCzRGIj/view?usp=sharing) | [base](https://
 pan.baidu.com/s/1WIcePgmqb7Ox0w1qigWQ_w)\[code: e47w\] \| [small](https://
 pan.baidu.com/s/17DAboL9w0mArcBBuiy3tGg)\[code: mdmg\] | # ð Quick Tour ##
-ð¶ w/ pretrained models *For the classification task* ```python from rannet
-import RanNet, RanNetWordPieceTokenizer vocab_path = 'pretrained/vocab.txt'
-ckpt_path = 'pretrained/model.ckpt' config_path = 'pretrained/config.json'
-tokenizer = RanNetWordPieceTokenizer(vocab_path, lowercase=True) rannet,
-rannet_model = RanNet.load_rannet( config_path=config_path,
-checkpoint_path=ckpt_path, return_sequences=False) output = rannet_model.output
-# (B, D) output = L.Dropout(0.1)(output) output = L.Dense(2,
-activation='softmax')(output) model = keras.models.Model(rannet_model.input,
-output) model.summary() ``` *For the sequence task* ```python from rannet
-import RanNet, RanNetWordPieceTokenizer vocab_path = 'pretrained/vocab.txt'
-ckpt_path = 'pretrained/model.ckpt' config_path = 'pretrained/config.json'
-tokenizer = RanNetWordPieceTokenizer(vocab_path, lowercase=True) rannet,
-rannet_model = RanNet.load_rannet( config_path=config_path,
-checkpoint_path=ckpt_path, return_cell=False) output = rannet_model.output #
-(B, L, D) rannet_model.summary() ``` ## ð w/o pretrained models Embed the
-`RAN` (a Keras layer) into your network. ```python from rannet import RAN ran =
-RAN(head_num=8, head_size=256, window_size=256, min_window_size=16,
-activation='swish', kernel_initializer='glorot_normal', apply_lm_mask=False,
+ð¶ w/ pretrained models *Extract semantic feature* set
+`apply_cell_transform=False` to extract semantic feature. ```python import
+numpy as np from rannet import RanNet, RanNetWordPieceTokenizer vocab_path =
+'pretrained/vocab.txt' ckpt_path = 'pretrained/model.ckpt' config_path =
+'pretrained/config.json' tokenizer = RanNetWordPieceTokenizer(vocab_path,
+lowercase=True) rannet, rannet_model = RanNet.load_rannet
+( config_path=config_path, checkpoint_path=ckpt_path, return_sequences=False,
+apply_cell_transform=False ) text = 'input text' tok = tokenizer.encode(text)
+vec = rannet_model.predict(np.array([tok.ids])) ``` *For the classification
+task* ```python from rannet import RanNet, RanNetWordPieceTokenizer vocab_path
+= 'pretrained/vocab.txt' ckpt_path = 'pretrained/model.ckpt' config_path =
+'pretrained/config.json' tokenizer = RanNetWordPieceTokenizer(vocab_path,
+lowercase=True) rannet, rannet_model = RanNet.load_rannet
+( config_path=config_path, checkpoint_path=ckpt_path, return_sequences=False)
+output = rannet_model.output # (B, D) output = L.Dropout(0.1)(output) output =
+L.Dense(2, activation='softmax')(output) model = keras.models.Model
+(rannet_model.input, output) model.summary() ``` *For the sequence task*
+```python from rannet import RanNet, RanNetWordPieceTokenizer vocab_path =
+'pretrained/vocab.txt' ckpt_path = 'pretrained/model.ckpt' config_path =
+'pretrained/config.json' tokenizer = RanNetWordPieceTokenizer(vocab_path,
+lowercase=True) rannet, rannet_model = RanNet.load_rannet
+( config_path=config_path, checkpoint_path=ckpt_path, return_gpc=False) output
+= rannet_model.output # (B, L, D) rannet_model.summary() ``` ## ð w/
+o pretrained models Embed the `RAN` (a Keras layer) into your network.
+```python from rannet import RAN ran = RAN(head_num=8, head_size=256,
+window_size=256, min_window_size=16, activation='swish',
+kernel_initializer='glorot_normal', apply_lm_mask=False,
 apply_seq2seq_mask=False, apply_memory_review=True, dropout_rate=0.0,
 cell_initializer_type='zero') output, cell = ran(X) ``` # ð Citation If you
 use our code in your research, please cite our work: ``` @inproceedings{li-
 etal-2023-ran, title = "Recurrent Attention Networks for Long-text Modeling",
 author = "Li, Xianming and Li, Zongxi and Luo, Xiaotian and Xie, Haoran and
 Lee, Xing and Zhao, Yingbin and Wang, Fu Lee and Li, Qing", booktitle =
 "Findings of the Association for Computational Linguistics: ACL 2023", year =
-"2023", publisher = "Association for Computational Linguistics" } ``` # Contact
-Please contact us at 1) for code problems, create a GitHub issue; 2) for paper
-problems, email xmlee97@gmail.com
+"2023", publisher = "Association for Computational Linguistics" } ``` # ð¬
+Contact Please contact us at 1) for code problems, create a GitHub issue; 2)
+for paper problems, email xmlee97@gmail.com
```

### Comparing `rannet-0.1.0/README.md` & `rannet-0.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,18 @@
 <h4 align='center'> 📢 This project is still in the works in order to make long document modeling easier.</h4>
 
 <h4 align="center">
    <a href="https://github.com/4AI/RAN/blob/main/LICENSE">
       <img src="https://img.shields.io/badge/License-MIT-blue.svg?style=flat-square" alt="RAN is released under the MIT license." />
    </a>
    <a href="https://pypi.org/project/rannet/">
-      <img src="https://badge.fury.io/py/RAN.svg?style=flat-square" alt="PyPI version" />
+      <img src="https://img.shields.io/pypi/v/rannet?style=flat-square" alt="PyPI version" />
+   </a>
+   <a href="https://pypi.org/project/rannet/">
+      <img src="https://img.shields.io/pypi/dm/rannet?style=flat-square" alt="PyPI Downloads" />
    </a>
    <a href="http://makeapullrequest.com">
       <img src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square" alt="http://makeapullrequest.com" />
    </a>
    <a href="https://arxiv.org/abs/2306.06843">
       <img src="https://img.shields.io/badge/Arxiv-2306.06843-yellow.svg?style=flat-square" alt="https://arxiv.org/abs/2306.06843" />
    </a>
@@ -45,14 +48,39 @@
 | CN   |   [base](https://drive.google.com/file/d/1_gmrulSU-ln_jElc2hktPTTQDzaeG1wU/view?usp=sharing)  \| [small](https://drive.google.com/file/d/1D-FCxY_UMwZCkvcwl6hkRcl6VnCzRGIj/view?usp=sharing)         |        [base](https://pan.baidu.com/s/1WIcePgmqb7Ox0w1qigWQ_w)\[code: e47w\]  \| [small](https://pan.baidu.com/s/17DAboL9w0mArcBBuiy3tGg)\[code: mdmg\]        |
 
 
 # 🚀 Quick Tour
 
 ## 🈶 w/ pretrained models
 
+*Extract semantic feature*
+
+set `apply_cell_transform=False` to extract semantic feature.
+
+```python
+import numpy as np
+from rannet import RanNet, RanNetWordPieceTokenizer
+
+
+vocab_path = 'pretrained/vocab.txt'
+ckpt_path = 'pretrained/model.ckpt'
+config_path = 'pretrained/config.json'
+tokenizer = RanNetWordPieceTokenizer(vocab_path, lowercase=True)
+
+rannet, rannet_model = RanNet.load_rannet(
+    config_path=config_path,
+    checkpoint_path=ckpt_path,
+    return_sequences=False,
+    apply_cell_transform=False
+)
+text = 'input text'
+tok = tokenizer.encode(text)
+vec = rannet_model.predict(np.array([tok.ids]))
+```
+
 *For the classification task*
 
 ```python
 from rannet import RanNet, RanNetWordPieceTokenizer
 
 
 vocab_path = 'pretrained/vocab.txt'
@@ -77,15 +105,15 @@
 
 vocab_path = 'pretrained/vocab.txt'
 ckpt_path = 'pretrained/model.ckpt'
 config_path = 'pretrained/config.json'
 tokenizer = RanNetWordPieceTokenizer(vocab_path, lowercase=True)
 
 rannet, rannet_model = RanNet.load_rannet(
-    config_path=config_path, checkpoint_path=ckpt_path, return_cell=False)
+    config_path=config_path, checkpoint_path=ckpt_path, return_gpc=False)
 output = rannet_model.output  # (B, L, D)
 rannet_model.summary()
 ```
 
 ## 🈚 w/o pretrained models
 
 Embed the `RAN` (a Keras layer) into your network.
@@ -117,10 +145,10 @@
     author = "Li, Xianming and Li, Zongxi and Luo, Xiaotian and Xie, Haoran and Lee, Xing and Zhao, Yingbin and Wang, Fu Lee and Li, Qing",
     booktitle = "Findings of the Association for Computational Linguistics: ACL 2023",
     year = "2023",
     publisher = "Association for Computational Linguistics"
 }
 ```
 
-# Contact
+# 📬 Contact
 
 Please contact us at 1) for code problems, create a GitHub issue; 2) for paper problems, email xmlee97@gmail.com
```

#### html2text {}

```diff
@@ -1,45 +1,54 @@
                 ****** RAN: Recurrent Attention Network ******
   *** ð¢ This project is still in the works in order to make long document
                              modeling easier. ***
-     *** [RAN_is_released_under_the_MIT_license.] [PyPI_version] [http://
-         makeapullrequest.com] [https://arxiv.org/abs/2306.06843] ***
+ *** [RAN_is_released_under_the_MIT_license.] [PyPI_version] [PyPI_Downloads]
+     [http://makeapullrequest.com] [https://arxiv.org/abs/2306.06843] ***
 # â¬ï¸ Installation *stable* ```bash python -m pip install -U rannet ```
 *latest* ```bash python -m pip install git+https://github.com/4AI/RAN.git ```
 *environment* - â­ tensorflow>2.0,<=2.10 ð¤ `export TF_KERAS=1` -
 tensorflow>=1.14,<2.0 ð¤ Keras==2.3.1 ## ðï¸ Pretrained Models | Lang |
 Google Drive | Baidu NetDrive | |------|--------------|----------------| | EN |
 [base](https://drive.google.com/file/d/1mRabw0Hy9T5_EWbZshD6Uk-bvauNzG9R/
 view?usp=sharing) | [base](https://pan.baidu.com/s/18uhAkY46aIcy4ncwzXp5mA)\
 [code: djkj\] | | CN | [base](https://drive.google.com/file/d/1_gmrulSU-
 ln_jElc2hktPTTQDzaeG1wU/view?usp=sharing) \| [small](https://drive.google.com/
 file/d/1D-FCxY_UMwZCkvcwl6hkRcl6VnCzRGIj/view?usp=sharing) | [base](https://
 pan.baidu.com/s/1WIcePgmqb7Ox0w1qigWQ_w)\[code: e47w\] \| [small](https://
 pan.baidu.com/s/17DAboL9w0mArcBBuiy3tGg)\[code: mdmg\] | # ð Quick Tour ##
-ð¶ w/ pretrained models *For the classification task* ```python from rannet
-import RanNet, RanNetWordPieceTokenizer vocab_path = 'pretrained/vocab.txt'
-ckpt_path = 'pretrained/model.ckpt' config_path = 'pretrained/config.json'
-tokenizer = RanNetWordPieceTokenizer(vocab_path, lowercase=True) rannet,
-rannet_model = RanNet.load_rannet( config_path=config_path,
-checkpoint_path=ckpt_path, return_sequences=False) output = rannet_model.output
-# (B, D) output = L.Dropout(0.1)(output) output = L.Dense(2,
-activation='softmax')(output) model = keras.models.Model(rannet_model.input,
-output) model.summary() ``` *For the sequence task* ```python from rannet
-import RanNet, RanNetWordPieceTokenizer vocab_path = 'pretrained/vocab.txt'
-ckpt_path = 'pretrained/model.ckpt' config_path = 'pretrained/config.json'
-tokenizer = RanNetWordPieceTokenizer(vocab_path, lowercase=True) rannet,
-rannet_model = RanNet.load_rannet( config_path=config_path,
-checkpoint_path=ckpt_path, return_cell=False) output = rannet_model.output #
-(B, L, D) rannet_model.summary() ``` ## ð w/o pretrained models Embed the
-`RAN` (a Keras layer) into your network. ```python from rannet import RAN ran =
-RAN(head_num=8, head_size=256, window_size=256, min_window_size=16,
-activation='swish', kernel_initializer='glorot_normal', apply_lm_mask=False,
+ð¶ w/ pretrained models *Extract semantic feature* set
+`apply_cell_transform=False` to extract semantic feature. ```python import
+numpy as np from rannet import RanNet, RanNetWordPieceTokenizer vocab_path =
+'pretrained/vocab.txt' ckpt_path = 'pretrained/model.ckpt' config_path =
+'pretrained/config.json' tokenizer = RanNetWordPieceTokenizer(vocab_path,
+lowercase=True) rannet, rannet_model = RanNet.load_rannet
+( config_path=config_path, checkpoint_path=ckpt_path, return_sequences=False,
+apply_cell_transform=False ) text = 'input text' tok = tokenizer.encode(text)
+vec = rannet_model.predict(np.array([tok.ids])) ``` *For the classification
+task* ```python from rannet import RanNet, RanNetWordPieceTokenizer vocab_path
+= 'pretrained/vocab.txt' ckpt_path = 'pretrained/model.ckpt' config_path =
+'pretrained/config.json' tokenizer = RanNetWordPieceTokenizer(vocab_path,
+lowercase=True) rannet, rannet_model = RanNet.load_rannet
+( config_path=config_path, checkpoint_path=ckpt_path, return_sequences=False)
+output = rannet_model.output # (B, D) output = L.Dropout(0.1)(output) output =
+L.Dense(2, activation='softmax')(output) model = keras.models.Model
+(rannet_model.input, output) model.summary() ``` *For the sequence task*
+```python from rannet import RanNet, RanNetWordPieceTokenizer vocab_path =
+'pretrained/vocab.txt' ckpt_path = 'pretrained/model.ckpt' config_path =
+'pretrained/config.json' tokenizer = RanNetWordPieceTokenizer(vocab_path,
+lowercase=True) rannet, rannet_model = RanNet.load_rannet
+( config_path=config_path, checkpoint_path=ckpt_path, return_gpc=False) output
+= rannet_model.output # (B, L, D) rannet_model.summary() ``` ## ð w/
+o pretrained models Embed the `RAN` (a Keras layer) into your network.
+```python from rannet import RAN ran = RAN(head_num=8, head_size=256,
+window_size=256, min_window_size=16, activation='swish',
+kernel_initializer='glorot_normal', apply_lm_mask=False,
 apply_seq2seq_mask=False, apply_memory_review=True, dropout_rate=0.0,
 cell_initializer_type='zero') output, cell = ran(X) ``` # ð Citation If you
 use our code in your research, please cite our work: ``` @inproceedings{li-
 etal-2023-ran, title = "Recurrent Attention Networks for Long-text Modeling",
 author = "Li, Xianming and Li, Zongxi and Luo, Xiaotian and Xie, Haoran and
 Lee, Xing and Zhao, Yingbin and Wang, Fu Lee and Li, Qing", booktitle =
 "Findings of the Association for Computational Linguistics: ACL 2023", year =
-"2023", publisher = "Association for Computational Linguistics" } ``` # Contact
-Please contact us at 1) for code problems, create a GitHub issue; 2) for paper
-problems, email xmlee97@gmail.com
+"2023", publisher = "Association for Computational Linguistics" } ``` # ð¬
+Contact Please contact us at 1) for code problems, create a GitHub issue; 2)
+for paper problems, email xmlee97@gmail.com
```

### Comparing `rannet-0.1.0/rannet/dataloader.py` & `rannet-0.2.0/rannet/dataloader.py`

 * *Files identical despite different names*

### Comparing `rannet-0.1.0/rannet/layers.py` & `rannet-0.2.0/rannet/layers.py`

 * *Files identical despite different names*

### Comparing `rannet-0.1.0/rannet/optimizer.py` & `rannet-0.2.0/rannet/optimizer.py`

 * *Files identical despite different names*

### Comparing `rannet-0.1.0/rannet/pretrain.py` & `rannet-0.2.0/rannet/pretrain.py`

 * *Files identical despite different names*

### Comparing `rannet-0.1.0/rannet/ran.py` & `rannet-0.2.0/rannet/ran.py`

 * *Files 2% similar despite different names*

```diff
@@ -428,15 +428,16 @@
         mask: Optional[Tensors] = None,
         apply_lm_mask: bool = False,
         apply_seq2seq_mask: bool = False,
         window_size: int = 128,
         concat_layernorm=None,
         memory_review=None,
         dropout_rate: float = 0.0,
-        min_window_size: int = 16):
+        min_window_size: int = 16,
+        cell_pooling: str = 'last'):
     """ Core implementation
     """
 
     def do_step(cell, current_input, mask=None, segment=None):
         current_input = K.concatenate((cell, current_input), axis=1)  # (B, 1 + W, D)
         # avoid gradient explosion
         # x' = \gamma * \frac{x - \mu}{\sigma} + \beta
@@ -605,15 +606,22 @@
         name='final-step'
     )
 
     if isinstance(memory_review, SelfAttention):
         outputs = memory_review([outputs, cells, cells], mask=mask)
     else:
         outputs = memory_review(outputs)
-    cell = K.squeeze(cell, axis=1)  # (B, D)
+    if cell_pooling == 'last':
+        cell = K.squeeze(cell, axis=1)  # (B, D)
+    elif cell_pooling == 'mean':
+        cell = K.mean(cells, axis=1)
+    elif cell_pooling == 'max':
+        cell = K.max(cells, axis=1)
+    else:
+        raise ValueError('Please specify `cell_pooling` from [`last`, `mean`, `max`]')
     return outputs, cell
 
 
 class RAN(L.Layer):
     def __init__(self,
                  head_num: int,
                  head_size: int = 256,
@@ -622,29 +630,30 @@
                  activation: Activation = 'swish',
                  kernel_initializer: Initializer = 'glorot_normal',
                  apply_lm_mask: bool = False,
                  apply_seq2seq_mask: bool = False,
                  apply_memory_review: bool = True,
                  dropout_rate: float = 0.0,
                  cell_initializer_type: str = 'zero',
+                 cell_pooling: str = 'last',
                  **kwargs):
         super(RAN, self).__init__(**kwargs)
         assert window_size > min_window_size, "window_size must be greater than min_window_size"
         self.head_num = head_num
         self.head_size = head_size
         self.window_size = window_size
         self.min_window_size = min_window_size
         self.activation = keras.activations.get(activation)
         self.kernel_initializer = kernel_initializer
         self.apply_lm_mask = apply_lm_mask
         self.apply_seq2seq_mask = apply_seq2seq_mask
         self.apply_memory_review = apply_memory_review
         self.dropout_rate = dropout_rate
         self.cell_initializer_type = cell_initializer_type
-
+        self.cell_pooling = cell_pooling
         self.supports_masking = True
 
     def get_config(self):
         config = {
             "head_num": self.head_num,
             "head_size": self.head_size,
             "window_size": self.window_size,
@@ -652,14 +661,15 @@
             "activation": keras.activations.serialize(self.activation),
             "kernel_initializer": keras.initializers.serialize(self.kernel_initializer),
             "apply_lm_mask": self.apply_lm_mask,
             "apply_seq2seq_mask": self.apply_seq2seq_mask,
             "apply_memory_review": self.apply_memory_review,
             "dropout_rate": self.dropout_rate,
             "cell_initializer_type": self.cell_initializer_type,
+            "cell_pooling": self.cell_pooling
         }
         base_config = super(RAN, self).get_config()
         return dict(base_config, **config)
 
     def build(self, input_shape: Union[Tensors, List[Tensors]]):
         super(RAN, self).build(input_shape)
         if not isinstance(input_shape, list):
@@ -734,14 +744,15 @@
             apply_lm_mask=self.apply_lm_mask,
             apply_seq2seq_mask=self.apply_seq2seq_mask,
             window_size=self.window_size,
             concat_layernorm=self.concat_layernorm,
             memory_review=self.memory_review,
             dropout_rate=self.dropout_rate,
             min_window_size=self.min_window_size,
+            cell_pooling=self.cell_pooling
         )
         return [outputs, cell]
 
     def compute_output_shape(self,
                              input_shape: Union[Tensors, List[Tensors]]) -> Union[Tensors, Tuple[Tensors, Tensors]]:
         if not isinstance(input_shape, list):
             input_shape = [input_shape]
```

### Comparing `rannet-0.1.0/rannet/rannet.py` & `rannet-0.2.0/rannet/rannet.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 
 """ lastest version
 """
 
 import json
 import itertools
-from typing import Dict, Union, Optional, Callable, Tuple, List
+from typing import Dict, Union, Optional, Callable, Tuple, List, Any
 
 import tensorflow as tf
 from langml import keras, L, K, TF_KERAS
 from langml.layers import LayerNorm
 from langml.plm import TokenEmbedding, EmbeddingMatching
 from langml.tensor_typing import Models, Tensors
 from langml.utils import load_variables
@@ -30,15 +30,16 @@
         self.embedding_size = config.get('embedding_size', 512)
         self.dropout_rate = config.get('dropout_rate', 0.1)
         self.ran_layers = config.get('ran_layers', 2)
         self.head_size = config.get('head_size', 128)
         self.head_num = config.get('head_num', 8)
         self.window_size = config.get('window_size', 256)
         self.min_window_size = config.get('min_window_size', 16)
-        self.cell_initializer_type = config.get('cell_initializer_type', 'zero')
+        self.cell_initializer_type = config.get('cell_initializer_type', 'zero')  # zero | mean
+        self.cell_pooling = config.get('cell_pooling', 'last')  # last | mean | max
         self.embedding_initializer = config.get('embedding_initializer', 'truncated_normal')
         self.kernel_initializer = config.get('kernel_initializer', 'truncated_normal')
         self.kernel_initializer_range = config.get('kernel_initializer_range', 0.02)
 
     @staticmethod
     def from_file(config_path: str):
         with open(config_path, 'r') as reader:
@@ -49,27 +50,38 @@
         return ','.join([f'{k}={v}' for k, v in self.__dict__.items()])
 
 
 class RanNet:
     def __init__(self,
                  params: RanNetParams,
                  return_sequences: bool = True,
-                 return_cell: bool = True,
+                 return_gpc: bool = True,
+                 return_history: bool = True,
                  mlm_softmax: bool = False,
-                 apply_final_cell_transform: bool = True,
+                 apply_cell_transform: bool = True,
                  apply_lm_mask: bool = False,
                  apply_seq2seq_mask: bool = False,
                  apply_memory_review: bool = True,
+                 cell_initializer_type: str = 'zero',
+                 cell_pooling: str = 'last',
+                 min_window_size: Optional[int] = None,
+                 window_size: Optional[int] = None,
                  prefix: str = ''):
         self.params = params
         self.return_sequences = return_sequences
-        self.return_cell = return_cell
-        self.apply_final_cell_transform = apply_final_cell_transform
+        self.return_gpc = return_gpc
+        self.return_history = return_history
+        self.apply_cell_transform = apply_cell_transform
+        self.cell_initializer_type = cell_initializer_type
+        self.cell_pooling = cell_pooling
+        self.min_window_size = min_window_size
+        self.window_size = window_size
         self.prefix = prefix
         self.inputs = None
+        self.__var_status = {}
 
         if self.params.kernel_initializer == 'truncated_normal':
             self.initializer = keras.initializers.TruncatedNormal(
                 stddev=self.params.kernel_initializer_range)
         else:
             self.initializer = self.params.kernel_initializer
         if self.params.embedding_initializer == 'truncated_normal':
@@ -88,23 +100,24 @@
         )
         self.embedding_layernorm = LayerNorm(name=self.get_weight_name('Embedding-LayerNorm'))
         self.embedding_dropout = L.Dropout(self.params.dropout_rate, name=self.get_weight_name('Embedding-Dropout'))
         self.rans = [
             RAN(
                 self.params.head_num,
                 head_size=self.params.head_size,
-                window_size=self.params.window_size,
-                min_window_size=self.params.min_window_size,
+                window_size=self.window_size or self.params.window_size,
+                min_window_size=self.min_window_size or self.params.min_window_size,
                 activation='swish',
                 kernel_initializer=self.initializer,
                 apply_lm_mask=apply_lm_mask,
                 apply_seq2seq_mask=apply_seq2seq_mask,
                 apply_memory_review=apply_memory_review,
                 dropout_rate=self.params.dropout_rate,
-                cell_initializer_type=self.params.cell_initializer_type,
+                cell_initializer_type=self.cell_initializer_type or self.params.cell_initializer_type,
+                cell_pooling=self.cell_pooling or self.params.cell_pooling,
                 name=self.get_weight_name(f'RAN-{i}')
             )
             for i in range(self.params.ran_layers)
         ]
         self.mlm_hidden = keras.Sequential([
             L.Dropout(self.params.dropout_rate, name='Dropout'),
             L.Dense(
@@ -130,15 +143,15 @@
         return name
 
     def get_inputs(self, with_cell: bool = False, with_segment: bool = False):
         x_in = L.Input(name=self.get_weight_name('Input-Token'), shape=(None, ))
         x = x_in
         self.inputs = [x_in]
         if with_cell:
-            cell_in = L.Input(name=self.get_weight_name('Input-Cell'), shape=(self.params.embedding_size, ))
+            cell_in = L.Input(name=self.get_weight_name('Input-GPC'), shape=(self.params.embedding_size, ))
             self.inputs.append(cell_in)
             cell = cell_in
         else:
             cell = None
         if with_segment:
             segment_in = L.Input(name=self.get_weight_name('Input-Segment'), shape=(None, ))
             self.inputs.append(segment_in)
@@ -151,19 +164,19 @@
                x: Tensors,
                x_mask: Tensors,
                cell: Optional[Tensors] = None,
                segments: Optional[Tensors] = None) -> Union[Tensors, List[Tensors]]:
         x = self.embedding_layernorm(x)
         x = self.embedding_dropout(x)
 
-        outputs, cell = x, None
+        outputs = x
         for kernel in self.rans:
             outputs, cell = kernel([outputs, x_mask], cell=cell, segments=segments)
 
-        if self.return_cell and self.apply_final_cell_transform:
+        if self.return_gpc and self.apply_cell_transform:
             cell = L.Lambda(lambda x: K.expand_dims(x, axis=1))(cell)
             cell = L.Dense(self.params.embedding_size,
                            kernel_initializer=self.initializer,
                            activation='swish',
                            name='Output-Cell-Dense')(cell)
             cell = L.Dropout(self.params.dropout_rate)(cell)
             cell = GatedLinearUnit(
@@ -174,15 +187,15 @@
             max_pooling = L.Dense(self.params.embedding_size,
                                   kernel_initializer=self.initializer,
                                   name='Output-Pooling-Dense')(max_pooling)
             # ct = p + g(c), use maxpooling to enhance semantic feature
             cell = L.Lambda(lambda x: x[0] + x[1], name='Output-Cell-Fuse')([cell, max_pooling])
             cell = L.Lambda(lambda x: K.squeeze(x, axis=1), name='Output-Cell-Squeeze')(cell)
         if self.return_sequences:
-            if self.return_cell:
+            if self.return_gpc:
                 return [outputs, cell]
             return outputs
         return cell
 
     def __call__(self,
                  with_cell: bool = False,
                  with_mlm: bool = False,
@@ -194,14 +207,19 @@
             with_mlm: bool,  if set `True` the mlm outputs will be returned,
                          if set `False`, the finetuning outputs including the sentence representation
                          and the semantic cell will be returned. Defaults to False.
             return_model: bool, whether to return keras model. Defaults to True.
             seq2seq: bool. Set seq2seq model. if seq2seq is True, segment information is required to input.
                 Segment is used to compute prefix causal mask. Defaults to False.
         """
+        self.__var_status['with_cell'] = with_cell
+        self.__var_status['with_mlm'] = with_mlm
+        self.__var_status['return_model'] = return_model
+        self.__var_status['seq2seq'] = seq2seq
+
         if seq2seq:
             assert with_mlm, "seq2seq only works for mlm model, please specify `with_mlm=True`"
         if with_mlm:
             assert self.return_sequences, "please specify `RanNet(..., return_sequences=True)`, when return mlm"
         x, cell, segments = self.get_inputs(with_cell=with_cell, with_segment=seq2seq)
         x_mask = self.text_masking(x)
 
@@ -209,15 +227,15 @@
         outputs = self.encode(x, x_mask, cell, segments=segments)
 
         if not with_mlm:
             if return_model:
                 return keras.Model(self.inputs, outputs)
             return outputs
 
-        output = outputs[0] if self.return_cell else outputs
+        output = outputs[0] if self.return_gpc else outputs
         mlm = self.mlm_hidden(output)
         mlm = self.mlm_matching([mlm, embedding_weights])
 
         if return_model:
             return keras.Model(self.inputs, mlm)
         return mlm
 
@@ -284,14 +302,17 @@
                 f'{prefix}/mlm-hidden/layernorm/beta',
                 f'{prefix}/mlm-hidden/layernorm/gamma',
             ],
             'MLM-Matching': [f'{prefix}/mlm-matching/bias'],
         })
         return mapping
 
+    def check_var_status(self, key: str, val: Any) -> bool:
+        return self.__var_status.get(key) == val
+
     @staticmethod
     def fields_to_check():
         """ define fields to be check in export checkpoint
         """
         return ['bias', 'kernel', 'beta', 'gamma', 'embeddings', 'gau_kernel', 'encode_attn',
                 'output_attn', 'output_layernorm', 'cell_initializer', 'cell_residual_layernorm',
                 'cell_glu']
@@ -366,14 +387,15 @@
 
     @staticmethod
     def load_rannet(config_path: str,
                     checkpoint_path: str,
                     window_size: Optional[int] = None,
                     cell_initializer_type: Optional[str] = None,
                     with_mlm: bool = False,
+                    with_cell: bool = False,
                     **kwargs) -> Tuple[object, Models]:
         """ Load pretrained RanNet model
         Args:
             config_path: str. Path to config
             checkpoint_path: str. Path to checkpoint
             with_mlm: bool. Wether to return mlm output. Defaults to False
             kwargs: Other kwargs of RanNet
@@ -383,15 +405,15 @@
         """
         params = RanNetParams.from_file(config_path)
         if window_size is not None:
             params.window_size = window_size
         if cell_initializer_type is not None:
             params.cell_initializer_type = cell_initializer_type
         rannet = RanNet(params, **kwargs)
-        model = rannet(with_mlm=with_mlm)
+        model = rannet(with_mlm=with_mlm, with_cell=with_cell)
         model = rannet.restore_weights_from_checkpoint(model, checkpoint_path, ran_layers=params.ran_layers)
         return rannet, model
 
     @staticmethod
     def compile(model: Models,
                 learning_rate: float = 1e-3,
                 weight_decay: float = 0.01,
@@ -416,20 +438,20 @@
             **kwargs
         )
 
 
 class RanNetForLM(RanNet):
     def __init__(self,
                  params: RanNetParams,
-                 return_cell: bool = False,
+                 return_gpc: bool = False,
                  prefix: str = ''):
         super().__init__(params,
                          return_sequences=True,
-                         return_cell=return_cell,
-                         apply_final_cell_transform=False,
+                         return_gpc=return_gpc,
+                         apply_cell_transform=False,
                          mlm_softmax=True,
                          apply_lm_mask=True,
                          apply_seq2seq_mask=False,
                          prefix=prefix)
 
     def __call__(self, with_cell: bool = False, return_model: bool = True) -> Union[Models, Tensors]:
         return super().__call__(with_cell=with_cell, with_mlm=True, return_model=return_model, seq2seq=False)
@@ -437,21 +459,21 @@
 
 class RanNetForAdaptiveLM(RanNet):
     def __init__(self,
                  params: RanNetParams,
                  cutoffs: List[int],
                  div_val: int = 1,
                  output_dropout_rate: float = 0.0,
-                 return_cell: bool = False,
+                 return_gpc: bool = False,
                  prefix: str = ''):
         super().__init__(params,
                          return_sequences=True,
-                         return_cell=return_cell,
+                         return_gpc=return_gpc,
                          mlm_softmax=False,
-                         apply_final_cell_transform=False,
+                         apply_cell_transform=False,
                          apply_lm_mask=True,
                          apply_seq2seq_mask=False,
                          prefix=prefix)
         dropout_rate = output_dropout_rate or self.params.dropout_rate
         self.output_dropout = L.Dropout(dropout_rate, name='Output-Dropout')
         self.token_embedding = AdaptiveEmbedding(
             input_dim=self.params.vocab_size,
@@ -502,31 +524,31 @@
 
 class RanNetForSeq2Seq(RanNet):
     def __init__(self,
                  params: RanNetParams,
                  prefix: str = ''):
         super().__init__(params,
                          return_sequences=True,
-                         return_cell=False,
+                         return_gpc=False,
                          mlm_softmax=True,
-                         apply_final_cell_transform=False,
+                         apply_cell_transform=False,
                          apply_lm_mask=False,
                          apply_seq2seq_mask=True,
                          prefix=prefix)
 
     def __call__(self, with_cell: bool = False, return_model: bool = True) -> Union[Models, Tensors]:
         return super().__call__(with_cell=with_cell, with_mlm=True, return_model=return_model, seq2seq=True)
 
 
 class RanNetForMLMPretrain(RanNet):
     def __init__(self, params: RanNetParams, **kwargs):
         super().__init__(params,
-                         return_cell=False,
+                         return_gpc=False,
                          return_sequences=True,
-                         apply_final_cell_transform=False,
+                         apply_cell_transform=False,
                          **kwargs)
 
     def __call__(self) -> Tuple[Models, Models, Dict]:
         mlm_output = super().__call__(with_mlm=True, return_model=False)
         token_ids_in = L.Input(name=self.get_weight_name('token_ids'),
                                shape=(None,), dtype=K.floatx())  # ground-truth token ids
         mlm_mask_in = L.Input(name=self.get_weight_name('mlm_mask'), shape=(None,), dtype=K.floatx())  # mlm mask
```

### Comparing `rannet-0.1.0/rannet/tokenizer.py` & `rannet-0.2.0/rannet/tokenizer.py`

 * *Files identical despite different names*

### Comparing `rannet-0.1.0/rannet/utils.py` & `rannet-0.2.0/rannet/utils.py`

 * *Files identical despite different names*

### Comparing `rannet-0.1.0/rannet.egg-info/PKG-INFO` & `rannet-0.2.0/rannet.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rannet
-Version: 0.1.0
+Version: 0.2.0
 Summary: Recurrent Attention Networks
 Author: sean lee
 Author-email: xmlee97@gmail.com
 Keywords: rannet
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -23,15 +23,18 @@
 <h4 align='center'> 📢 This project is still in the works in order to make long document modeling easier.</h4>
 
 <h4 align="center">
    <a href="https://github.com/4AI/RAN/blob/main/LICENSE">
       <img src="https://img.shields.io/badge/License-MIT-blue.svg?style=flat-square" alt="RAN is released under the MIT license." />
    </a>
    <a href="https://pypi.org/project/rannet/">
-      <img src="https://badge.fury.io/py/RAN.svg?style=flat-square" alt="PyPI version" />
+      <img src="https://img.shields.io/pypi/v/rannet?style=flat-square" alt="PyPI version" />
+   </a>
+   <a href="https://pypi.org/project/rannet/">
+      <img src="https://img.shields.io/pypi/dm/rannet?style=flat-square" alt="PyPI Downloads" />
    </a>
    <a href="http://makeapullrequest.com">
       <img src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square" alt="http://makeapullrequest.com" />
    </a>
    <a href="https://arxiv.org/abs/2306.06843">
       <img src="https://img.shields.io/badge/Arxiv-2306.06843-yellow.svg?style=flat-square" alt="https://arxiv.org/abs/2306.06843" />
    </a>
@@ -65,14 +68,39 @@
 | CN   |   [base](https://drive.google.com/file/d/1_gmrulSU-ln_jElc2hktPTTQDzaeG1wU/view?usp=sharing)  \| [small](https://drive.google.com/file/d/1D-FCxY_UMwZCkvcwl6hkRcl6VnCzRGIj/view?usp=sharing)         |        [base](https://pan.baidu.com/s/1WIcePgmqb7Ox0w1qigWQ_w)\[code: e47w\]  \| [small](https://pan.baidu.com/s/17DAboL9w0mArcBBuiy3tGg)\[code: mdmg\]        |
 
 
 # 🚀 Quick Tour
 
 ## 🈶 w/ pretrained models
 
+*Extract semantic feature*
+
+set `apply_cell_transform=False` to extract semantic feature.
+
+```python
+import numpy as np
+from rannet import RanNet, RanNetWordPieceTokenizer
+
+
+vocab_path = 'pretrained/vocab.txt'
+ckpt_path = 'pretrained/model.ckpt'
+config_path = 'pretrained/config.json'
+tokenizer = RanNetWordPieceTokenizer(vocab_path, lowercase=True)
+
+rannet, rannet_model = RanNet.load_rannet(
+    config_path=config_path,
+    checkpoint_path=ckpt_path,
+    return_sequences=False,
+    apply_cell_transform=False
+)
+text = 'input text'
+tok = tokenizer.encode(text)
+vec = rannet_model.predict(np.array([tok.ids]))
+```
+
 *For the classification task*
 
 ```python
 from rannet import RanNet, RanNetWordPieceTokenizer
 
 
 vocab_path = 'pretrained/vocab.txt'
@@ -97,15 +125,15 @@
 
 vocab_path = 'pretrained/vocab.txt'
 ckpt_path = 'pretrained/model.ckpt'
 config_path = 'pretrained/config.json'
 tokenizer = RanNetWordPieceTokenizer(vocab_path, lowercase=True)
 
 rannet, rannet_model = RanNet.load_rannet(
-    config_path=config_path, checkpoint_path=ckpt_path, return_cell=False)
+    config_path=config_path, checkpoint_path=ckpt_path, return_gpc=False)
 output = rannet_model.output  # (B, L, D)
 rannet_model.summary()
 ```
 
 ## 🈚 w/o pretrained models
 
 Embed the `RAN` (a Keras layer) into your network.
@@ -137,10 +165,10 @@
     author = "Li, Xianming and Li, Zongxi and Luo, Xiaotian and Xie, Haoran and Lee, Xing and Zhao, Yingbin and Wang, Fu Lee and Li, Qing",
     booktitle = "Findings of the Association for Computational Linguistics: ACL 2023",
     year = "2023",
     publisher = "Association for Computational Linguistics"
 }
 ```
 
-# Contact
+# 📬 Contact
 
 Please contact us at 1) for code problems, create a GitHub issue; 2) for paper problems, email xmlee97@gmail.com
```

#### html2text {}

```diff
@@ -1,55 +1,64 @@
-Metadata-Version: 2.1 Name: rannet Version: 0.1.0 Summary: Recurrent Attention
+Metadata-Version: 2.1 Name: rannet Version: 0.2.0 Summary: Recurrent Attention
 Networks Author: sean lee Author-email: xmlee97@gmail.com Keywords: rannet
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Description-Content-Type: text/markdown
 License-File: LICENSE
                 ****** RAN: Recurrent Attention Network ******
   *** ð¢ This project is still in the works in order to make long document
                              modeling easier. ***
-     *** [RAN_is_released_under_the_MIT_license.] [PyPI_version] [http://
-         makeapullrequest.com] [https://arxiv.org/abs/2306.06843] ***
+ *** [RAN_is_released_under_the_MIT_license.] [PyPI_version] [PyPI_Downloads]
+     [http://makeapullrequest.com] [https://arxiv.org/abs/2306.06843] ***
 # â¬ï¸ Installation *stable* ```bash python -m pip install -U rannet ```
 *latest* ```bash python -m pip install git+https://github.com/4AI/RAN.git ```
 *environment* - â­ tensorflow>2.0,<=2.10 ð¤ `export TF_KERAS=1` -
 tensorflow>=1.14,<2.0 ð¤ Keras==2.3.1 ## ðï¸ Pretrained Models | Lang |
 Google Drive | Baidu NetDrive | |------|--------------|----------------| | EN |
 [base](https://drive.google.com/file/d/1mRabw0Hy9T5_EWbZshD6Uk-bvauNzG9R/
 view?usp=sharing) | [base](https://pan.baidu.com/s/18uhAkY46aIcy4ncwzXp5mA)\
 [code: djkj\] | | CN | [base](https://drive.google.com/file/d/1_gmrulSU-
 ln_jElc2hktPTTQDzaeG1wU/view?usp=sharing) \| [small](https://drive.google.com/
 file/d/1D-FCxY_UMwZCkvcwl6hkRcl6VnCzRGIj/view?usp=sharing) | [base](https://
 pan.baidu.com/s/1WIcePgmqb7Ox0w1qigWQ_w)\[code: e47w\] \| [small](https://
 pan.baidu.com/s/17DAboL9w0mArcBBuiy3tGg)\[code: mdmg\] | # ð Quick Tour ##
-ð¶ w/ pretrained models *For the classification task* ```python from rannet
-import RanNet, RanNetWordPieceTokenizer vocab_path = 'pretrained/vocab.txt'
-ckpt_path = 'pretrained/model.ckpt' config_path = 'pretrained/config.json'
-tokenizer = RanNetWordPieceTokenizer(vocab_path, lowercase=True) rannet,
-rannet_model = RanNet.load_rannet( config_path=config_path,
-checkpoint_path=ckpt_path, return_sequences=False) output = rannet_model.output
-# (B, D) output = L.Dropout(0.1)(output) output = L.Dense(2,
-activation='softmax')(output) model = keras.models.Model(rannet_model.input,
-output) model.summary() ``` *For the sequence task* ```python from rannet
-import RanNet, RanNetWordPieceTokenizer vocab_path = 'pretrained/vocab.txt'
-ckpt_path = 'pretrained/model.ckpt' config_path = 'pretrained/config.json'
-tokenizer = RanNetWordPieceTokenizer(vocab_path, lowercase=True) rannet,
-rannet_model = RanNet.load_rannet( config_path=config_path,
-checkpoint_path=ckpt_path, return_cell=False) output = rannet_model.output #
-(B, L, D) rannet_model.summary() ``` ## ð w/o pretrained models Embed the
-`RAN` (a Keras layer) into your network. ```python from rannet import RAN ran =
-RAN(head_num=8, head_size=256, window_size=256, min_window_size=16,
-activation='swish', kernel_initializer='glorot_normal', apply_lm_mask=False,
+ð¶ w/ pretrained models *Extract semantic feature* set
+`apply_cell_transform=False` to extract semantic feature. ```python import
+numpy as np from rannet import RanNet, RanNetWordPieceTokenizer vocab_path =
+'pretrained/vocab.txt' ckpt_path = 'pretrained/model.ckpt' config_path =
+'pretrained/config.json' tokenizer = RanNetWordPieceTokenizer(vocab_path,
+lowercase=True) rannet, rannet_model = RanNet.load_rannet
+( config_path=config_path, checkpoint_path=ckpt_path, return_sequences=False,
+apply_cell_transform=False ) text = 'input text' tok = tokenizer.encode(text)
+vec = rannet_model.predict(np.array([tok.ids])) ``` *For the classification
+task* ```python from rannet import RanNet, RanNetWordPieceTokenizer vocab_path
+= 'pretrained/vocab.txt' ckpt_path = 'pretrained/model.ckpt' config_path =
+'pretrained/config.json' tokenizer = RanNetWordPieceTokenizer(vocab_path,
+lowercase=True) rannet, rannet_model = RanNet.load_rannet
+( config_path=config_path, checkpoint_path=ckpt_path, return_sequences=False)
+output = rannet_model.output # (B, D) output = L.Dropout(0.1)(output) output =
+L.Dense(2, activation='softmax')(output) model = keras.models.Model
+(rannet_model.input, output) model.summary() ``` *For the sequence task*
+```python from rannet import RanNet, RanNetWordPieceTokenizer vocab_path =
+'pretrained/vocab.txt' ckpt_path = 'pretrained/model.ckpt' config_path =
+'pretrained/config.json' tokenizer = RanNetWordPieceTokenizer(vocab_path,
+lowercase=True) rannet, rannet_model = RanNet.load_rannet
+( config_path=config_path, checkpoint_path=ckpt_path, return_gpc=False) output
+= rannet_model.output # (B, L, D) rannet_model.summary() ``` ## ð w/
+o pretrained models Embed the `RAN` (a Keras layer) into your network.
+```python from rannet import RAN ran = RAN(head_num=8, head_size=256,
+window_size=256, min_window_size=16, activation='swish',
+kernel_initializer='glorot_normal', apply_lm_mask=False,
 apply_seq2seq_mask=False, apply_memory_review=True, dropout_rate=0.0,
 cell_initializer_type='zero') output, cell = ran(X) ``` # ð Citation If you
 use our code in your research, please cite our work: ``` @inproceedings{li-
 etal-2023-ran, title = "Recurrent Attention Networks for Long-text Modeling",
 author = "Li, Xianming and Li, Zongxi and Luo, Xiaotian and Xie, Haoran and
 Lee, Xing and Zhao, Yingbin and Wang, Fu Lee and Li, Qing", booktitle =
 "Findings of the Association for Computational Linguistics: ACL 2023", year =
-"2023", publisher = "Association for Computational Linguistics" } ``` # Contact
-Please contact us at 1) for code problems, create a GitHub issue; 2) for paper
-problems, email xmlee97@gmail.com
+"2023", publisher = "Association for Computational Linguistics" } ``` # ð¬
+Contact Please contact us at 1) for code problems, create a GitHub issue; 2)
+for paper problems, email xmlee97@gmail.com
```

### Comparing `rannet-0.1.0/setup.py` & `rannet-0.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     requirements = [l for l in f.read().splitlines() if l]
 
 with open('dev-requirements.txt', encoding='utf-8') as f:
     test_requirements = [l for l in f.read().splitlines() if l][1:]
 
 setup(
     name='rannet',
-    version='0.1.0',
+    version='0.2.0',
     description='Recurrent Attention Networks',
     long_description=readme,
     long_description_content_type="text/markdown",
     author='sean lee',
     author_email='xmlee97@gmail.com',
     packages=find_packages(exclude=("tests", "tests.*", "examples", "examples.*")),
     install_requires=requirements,
```

