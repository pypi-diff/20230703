# Comparing `tmp/codeassist-0.1.0.tar.gz` & `tmp/codeassist-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codeassist-0.1.0.tar", last modified: Mon Jun 26 06:01:45 2023, max compression
+gzip compressed data, was "codeassist-1.0.0.tar", last modified: Mon Jul  3 12:22:44 2023, max compression
```

## Comparing `codeassist-0.1.0.tar` & `codeassist-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-06-26 06:01:45.579583 codeassist-0.1.0/
--rw-r--r--   0 xuming     (501) staff       (20)    11357 2023-06-26 05:33:48.000000 codeassist-0.1.0/LICENSE
--rw-r--r--   0 xuming     (501) staff       (20)    12066 2023-06-26 06:01:45.580093 codeassist-0.1.0/PKG-INFO
--rw-r--r--   0 xuming     (501) staff       (20)     8840 2023-06-26 05:42:30.000000 codeassist-0.1.0/README.md
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-06-26 06:01:45.573187 codeassist-0.1.0/autocoder/
--rw-r--r--   0 xuming     (501) staff       (20)      147 2023-06-26 05:38:03.000000 codeassist-0.1.0/autocoder/__init__.py
--rwxr-xr-x   0 xuming     (501) staff       (20)     6623 2023-06-26 05:33:48.000000 codeassist-0.1.0/autocoder/create_dataset.py
--rwxr-xr-x   0 xuming     (501) staff       (20)    19355 2023-06-26 05:33:48.000000 codeassist-0.1.0/autocoder/gpt2_coder.py
-drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-06-26 06:01:45.578895 codeassist-0.1.0/codeassist.egg-info/
--rw-r--r--   0 xuming     (501) staff       (20)    12066 2023-06-26 06:01:45.000000 codeassist-0.1.0/codeassist.egg-info/PKG-INFO
--rw-r--r--   0 xuming     (501) staff       (20)      312 2023-06-26 06:01:45.000000 codeassist-0.1.0/codeassist.egg-info/SOURCES.txt
--rw-r--r--   0 xuming     (501) staff       (20)        1 2023-06-26 06:01:45.000000 codeassist-0.1.0/codeassist.egg-info/dependency_links.txt
--rw-r--r--   0 xuming     (501) staff       (20)        1 2023-06-26 06:01:45.000000 codeassist-0.1.0/codeassist.egg-info/not-zip-safe
--rw-r--r--   0 xuming     (501) staff       (20)       27 2023-06-26 06:01:45.000000 codeassist-0.1.0/codeassist.egg-info/requires.txt
--rw-r--r--   0 xuming     (501) staff       (20)       10 2023-06-26 06:01:45.000000 codeassist-0.1.0/codeassist.egg-info/top_level.txt
--rw-r--r--   0 xuming     (501) staff       (20)      309 2023-06-26 06:01:45.581029 codeassist-0.1.0/setup.cfg
--rw-r--r--   0 xuming     (501) staff       (20)     1253 2023-06-26 06:01:31.000000 codeassist-0.1.0/setup.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-07-03 12:22:44.604294 codeassist-1.0.0/
+-rw-r--r--   0 xuming     (501) staff       (20)    11357 2023-06-26 05:33:48.000000 codeassist-1.0.0/LICENSE
+-rw-r--r--   0 xuming     (501) staff       (20)    13051 2023-07-03 12:22:44.604569 codeassist-1.0.0/PKG-INFO
+-rw-r--r--   0 xuming     (501) staff       (20)     9873 2023-07-03 12:20:59.000000 codeassist-1.0.0/README.md
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-07-03 12:22:44.600391 codeassist-1.0.0/codeassist/
+-rw-r--r--   0 xuming     (501) staff       (20)      196 2023-06-30 11:51:24.000000 codeassist-1.0.0/codeassist/__init__.py
+-rwxr-xr-x   0 xuming     (501) staff       (20)     6623 2023-06-26 05:33:48.000000 codeassist-1.0.0/codeassist/create_dataset.py
+-rwxr-xr-x   0 xuming     (501) staff       (20)    19389 2023-06-30 13:22:13.000000 codeassist-1.0.0/codeassist/gpt2_coder.py
+-rwxr-xr-x   0 xuming     (501) staff       (20)    23862 2023-07-01 07:19:27.000000 codeassist-1.0.0/codeassist/wizard_coder.py
+drwxr-xr-x   0 xuming     (501) staff       (20)        0 2023-07-03 12:22:44.603910 codeassist-1.0.0/codeassist.egg-info/
+-rw-r--r--   0 xuming     (501) staff       (20)    13051 2023-07-03 12:22:44.000000 codeassist-1.0.0/codeassist.egg-info/PKG-INFO
+-rw-r--r--   0 xuming     (501) staff       (20)      342 2023-07-03 12:22:44.000000 codeassist-1.0.0/codeassist.egg-info/SOURCES.txt
+-rw-r--r--   0 xuming     (501) staff       (20)        1 2023-07-03 12:22:44.000000 codeassist-1.0.0/codeassist.egg-info/dependency_links.txt
+-rw-r--r--   0 xuming     (501) staff       (20)        1 2023-07-03 12:21:53.000000 codeassist-1.0.0/codeassist.egg-info/not-zip-safe
+-rw-r--r--   0 xuming     (501) staff       (20)       41 2023-07-03 12:22:44.000000 codeassist-1.0.0/codeassist.egg-info/requires.txt
+-rw-r--r--   0 xuming     (501) staff       (20)       11 2023-07-03 12:22:44.000000 codeassist-1.0.0/codeassist.egg-info/top_level.txt
+-rw-r--r--   0 xuming     (501) staff       (20)      309 2023-07-03 12:22:44.605139 codeassist-1.0.0/setup.cfg
+-rw-r--r--   0 xuming     (501) staff       (20)     1289 2023-06-30 10:19:57.000000 codeassist-1.0.0/setup.py
```

### Comparing `codeassist-0.1.0/LICENSE` & `codeassist-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `codeassist-0.1.0/PKG-INFO` & `codeassist-1.0.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,172 +1,193 @@
 Metadata-Version: 2.1
 Name: codeassist
-Version: 0.1.0
+Version: 1.0.0
 Summary: Code AutoComplete
 Home-page: https://github.com/shibing624/autocoder
 Author: XuMing
 Author-email: xuming624@qq.com
 License: Apache License 2.0
-Description: [![PyPI version](https://badge.fury.io/py/autocoder.svg)](https://badge.fury.io/py/autocoder)
+Description: [**🇨🇳中文**](https://github.com/shibing624/codeassist/blob/main/README.md) | [**🌐English**](https://github.com/shibing624/codeassist/blob/main/README_EN.md) | [**📖文档/Docs**](https://github.com/shibing624/codeassist/wiki) | [**🤖模型/Models**](https://huggingface.co/shibing624) 
+        
+        <div align="center">
+          <a href="https://github.com/shibing624/codeassist">
+            <img src="https://github.com/shibing624/codeassist/blob/main/docs/codeassist.png" height="130" alt="Logo">
+          </a>
+        </div>
+        
+        -----------------
+        
+        # CodeAssist: Advanced Code Completion Tool
+        [![PyPI version](https://badge.fury.io/py/codeassist.svg)](https://badge.fury.io/py/codeassist)
         [![Contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)](CONTRIBUTING.md)
-        [![GitHub contributors](https://img.shields.io/github/contributors/shibing624/autocoder.svg)](https://github.com/shibing624/autocoder/graphs/contributors)
+        [![GitHub contributors](https://img.shields.io/github/contributors/shibing624/codeassist.svg)](https://github.com/shibing624/codeassist/graphs/contributors)
         [![License Apache 2.0](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](LICENSE)
         [![python_vesion](https://img.shields.io/badge/Python-3.5%2B-green.svg)](requirements.txt)
-        [![GitHub issues](https://img.shields.io/github/issues/shibing624/autocoder.svg)](https://github.com/shibing624/autocoder/issues)
+        [![GitHub issues](https://img.shields.io/github/issues/shibing624/codeassist.svg)](https://github.com/shibing624/codeassist/issues)
         [![Wechat Group](http://vlog.sfyc.ltd/wechat_everyday/wxgroup_logo.png?imageView2/0/w/60/h/20)](#Contact)
         
-        # AutoCoder
-        
-        **AutoCoder** is an advanced code completion tool that intelligently provides high-quality code completions for Python, Java, and C++ and so on. 
+        ## Introduction
         
-        AutoCoder 是一个高级代码补全工具，能智能地为 Python、Java 和 C++ 等编程语言高质量补全代码
+        **CodeAssist** is an advanced code completion tool that intelligently provides high-quality code completions for Python, Java, and C++ and so on. 
         
+        CodeAssist 是一个高级代码补全工具，高质量为 Python、Java 和 C++ 等编程语言补全代码
         
-        **Guide**
         
-        - [Feature](#Feature)
-        - [Install](#install)
-        - [Usage](#usage)
-        - [Contact](#Contact)
-        - [Citation](#Citation)
-        - [Reference](#reference)
+        ## Features
         
-        # Feature
-        
-        - GPT2-based code completion
-        - Code completion for Python, other language is coming soon
+        - GPT based code completion
+        - Code completion for `Python`, `Java`, `C++`, `javascript` and so on
         - Line and block code completion
-        - Train(Fine-tune GPT2) and predict model with your own data
+        - Train(Fine-tuning) and predict model with your own data
+        
+        ### Release Models
         
+        | Arch   | BaseModel         | Model                                                                                                                   | Model Size | 
+        |:-------|:------------------|:------------------------------------------------------------------------------------------------------------------------|:----------:|
+        | GPT   | gpt2              | [shibing624/code-autocomplete-gpt2-base](https://huggingface.co/shibing624/code-autocomplete-gpt2-base)                 |   487MB    |
+        | GPT   | distilgpt2        | [shibing624/code-autocomplete-distilgpt2-python](https://huggingface.co/shibing624/code-autocomplete-distilgpt2-python) |   319MB    |
+        | GPT   | bigcode/starcoder | [WizardLM/WizardCoder-15B-V1.0](https://huggingface.co/WizardLM/WizardCoder-15B-V1.0)                                   |    29GB    |
         
-        # Demo
         
+        ### Demo
         
         HuggingFace Demo: https://huggingface.co/spaces/shibing624/code-autocomplete
         
-        # Install
+        backend model: `shibing624/code-autocomplete-gpt2-base`
         
-        ```
+        ## Install
+        
+        ```shell
         pip install torch # conda install pytorch
-        pip install -U autocoder
+        pip install -U codeassist
         ```
         
         or
         
-        ```
-        git clone https://github.com/shibing624/autocoder.git
-        cd AutoCoder
+        ```shell
+        git clone https://github.com/shibing624/codeassist.git
+        cd CodeAssist
         python setup.py install
         ```
         
-        # Usage
+        ## Usage
+        
+        ### WizardCoder model
         
-        ## Code Completion
+        WizardCoder-15b is fine-tuned `bigcode/starcoder` with alpaca code data, you can use the following code to generate code:
         
-        Model upload to HF's model hub:
+        example: [examples/wizardcoder_demo.py](https://github.com/shibing624/CodeAssist/blob/main/examples/wizardcoder_demo.py)
         
-        - DistilGPT2-python: [shibing624/code-autocomplete-distilgpt2-python](https://huggingface.co/shibing624/code-autocomplete-distilgpt2-python) (fine-tuned distilgpt2, model size: 319MB)
-        - GPT2-python: [shibing624/code-autocomplete-gpt2-base](https://huggingface.co/shibing624/code-autocomplete-gpt2-base) (fine-tuned gpt2, model size: 487MB)
+        ```python
+        import sys
+        
+        sys.path.append('..')
+        from codeassist import WizardCoder
         
-        ![hf](docs/hf_model.png)
+        m = WizardCoder("WizardLM/WizardCoder-15B-V1.0")
+        print(m.generate('def load_csv_file(file_path):')[0])
+        ```
         
-        ### Use with autocoder
+        output:
         
-        example: [base_demo.py](./examples/base_demo.py)
         
         ```python
-        from autocoder import GPT2Coder
+        import csv
         
-        m = GPT2Coder("shibing624/code-autocomplete-gpt2-base")
-        print(m.generate('import torch.nn as')[0])
+        def load_csv_file(file_path):
+            """
+            Load data from a CSV file and return a list of dictionaries.
+            """
+            # Open the file in read mode
+            with open(file_path, 'r') as file:
+                # Create a CSV reader object
+                csv_reader = csv.DictReader(file)
+                # Initialize an empty list to store the data
+                data = []
+                # Iterate over each row of data
+                for row in csv_reader:
+                    # Append the row of data to the list
+                    data.append(row)
+            # Return the list of data
+            return data
         ```
         
+        model output is impressively effective, it currently supports English and Chinese input, you can enter instructions or code prefixes as required.
+        
+        ### distilgpt2 model
+        
+        
         distilgpt2 fine-tuned code autocomplete model, you can use the following code:
         
-        example: [distilgpt2_demo.py](./examples/distilgpt2_demo.py)
+        example: [examples/distilgpt2_demo.py](https://github.com/shibing624/CodeAssist/blob/main/examples/distilgpt2_demo.py)
         
         ```python
         import sys
         
         sys.path.append('..')
-        from autocoder import GPT2Coder
+        from codeassist import GPT2Coder
         
         m = GPT2Coder("shibing624/code-autocomplete-distilgpt2-python")
         print(m.generate('import torch.nn as')[0])
         ```
         
         output:
         
         ```shell
         import torch.nn as nn
         import torch.nn.functional as F
         ```
         
         ### Use with huggingface/transformers：
         
-        example: [use_transformers_gpt2.py](./examples/use_transformers_gpt2.py)
+        example: [examples/use_transformers_gpt2.py](https://github.com/shibing624/CodeAssist/blob/main/examples/use_transformers_gpt2.py)
         
-        *Please use 'GPT2' related functions to load this model!*
+        ### Train Model
+        #### Train WizardCoder model
+        example: [examples/training_wizardcoder_mydata.py](https://github.com/shibing624/CodeAssist/blob/main/examples/training_wizardcoder_mydata.py)
         
-        ```python
+        ```shell
+        cd examples
+        CUDA_VISIBLE_DEVICES=0,1 python training_wizardcoder_mydata.py --do_train --do_predict --num_epochs 1 --output_dir outputs-wizard --model_name WizardLM/WizardCoder-15B-V1.0
+        ```
         
-        import os
-        from transformers import GPT2Tokenizer, GPT2LMHeadModel
+        - GPU memory: 31GB
+        - finetune need 2*V100(32GB)
+        - inference need 1*V100(32GB)
         
-        os.environ["KMP_DUPLICATE_LIB_OK"] = "TRUE"
+        #### Train distilgpt2 model
+        example: [examples/training_gpt2_mydata.py](https://github.com/shibing624/CodeAssist/blob/main/examples/training_gpt2_mydata.py)
         
-        tokenizer = GPT2Tokenizer.from_pretrained("shibing624/autocoder-gpt2-base")
-        model = GPT2LMHeadModel.from_pretrained("shibing624/autocoder-gpt2-base")
-        prompts = [
-            "import numpy as np",
-            "import torch.nn as",
-            'parser.add_argument("--num_train_epochs",',
-            "def set_seed(",
-            "def factorial",
-        ]
-        for prompt in prompts:
-            input_ids = tokenizer(prompt, return_tensors='pt').input_ids
-            outputs = model.generate(input_ids=input_ids,
-                                     max_length=64 + len(input_ids[0]),
-                                     temperature=1.0,
-                                     top_k=50,
-                                     top_p=0.95,
-                                     repetition_penalty=1.0,
-                                     do_sample=True,
-                                     num_return_sequences=1,
-                                     length_penalty=2.0,
-                                     early_stopping=True,
-                                     pad_token_id=tokenizer.eos_token_id,
-                                     eos_token_id=tokenizer.eos_token_id,
-                                     )
-            decoded = tokenizer.decode(outputs[0], skip_special_tokens=True)
-            print("Input :", prompt)
-            print("Output:", decoded)
-            print("=" * 20)
+        ```shell
+        cd examples
+        python training_gpt2_mydata.py --do_train --do_predict --num_epochs 15 --output_dir outputs-gpt2 --model_name gpt2
         ```
         
-        output:
+        PS: fine-tuned result model is GPT2-python: [shibing624/code-autocomplete-gpt2-base](https://huggingface.co/shibing624/code-autocomplete-gpt2-base), 
+        I spent about 24 hours with V100 to fine-tune it. 
+        
+        
+        ### Server
+        
+        start FastAPI server:
+        
+        example: [examples/server.py](https://github.com/shibing624/CodeAssist/blob/main/examples/server.py)
         
         ```shell
-        import numpy as np
-        ====================
-        import torch.nn as nn
-        import torchvision.transforms as transforms
-        ====================
-        parser.add_argument("--num_train_epochs", type=int, default=50, help="Number of training epochs.")
-        parser.add_argument("--batch_size", type=int, default=32, help="Batch size of validation/test data.")
-        ====================
-        def set_seed(self):
-        ====================
-        def factorial(n: int) -> int:
+        cd examples
+        python server.py
         ```
         
-        ## Train your own model with Dataset
+        open url: http://0.0.0.0:8001/docs
+        
+        ![api](https://github.com/shibing624/CodeAssist/blob/main/docs/api.png)
+        
         
-        ### Build dataset
+        
+        ## Dataset
         
         This allows to customize dataset building. Below is an example of the building process.
         
         Let's use Python codes from [Awesome-pytorch-list](https://github.com/bharathgs/Awesome-pytorch-list)
         
         1. We want the model to help auto-complete codes at a general level. The codes of The Algorithms suits the need.
         2. This code from this project is well written (high-quality codes).
@@ -180,18 +201,14 @@
         └── test.txt
         ```
         
         There are three ways to build dataset:
         1. Use the huggingface/datasets library load the dataset
         huggingface datasets [https://huggingface.co/datasets/shibing624/source_code](https://huggingface.co/datasets/shibing624/source_code)
         
-        ```shell
-        pip install datasets
-        ```
-        
         ```python
         from datasets import load_dataset
         dataset = load_dataset("shibing624/source_code", "python") # python or java or cpp
         print(dataset)
         print(dataset['test'][0:10])
         ```
         
@@ -223,99 +240,76 @@
         ]}
         ```
         
         2. Download dataset from Cloud
         
         | Name | Source | Download | Size |
         | :------- | :--------- | :---------: | :---------: |
-        | Python+Java+CPP source code | Awesome-pytorch-list(5.22 Million lines) | [github_source_code.zip](https://github.com/shibing624/autocoder/releases/download/0.0.4/source_code.zip) | 105M |
+        | Python+Java+CPP source code | Awesome-pytorch-list(5.22 Million lines) | [github_source_code.zip](https://github.com/shibing624/codeassist/releases/download/0.0.4/source_code.zip) | 105M |
         
         download dataset and unzip it, put to `examples/`.
         
         3. Get source code from scratch and build dataset
         
-        [prepare_data.py](./examples/prepare_data.py)
+        [prepare_code_data.py](https://github.com/shibing624/CodeAssist/blob/main/examples/prepare_code_data.py)
         
         ```shell
         cd examples
-        python prepare_data.py --num_repos 260
+        python prepare_code_data.py --num_repos 260
         ```
         
-        ### Train and predict model
         
-        example: [train_gpt2.py](./examples/train_gpt2.py)
-        
-        ```shell
-        cd examples
-        python training_gpt2_mydata.py --do_train --do_predict --num_epochs 15 --model_dir outputs-fine-tuned --model_name gpt2
-        ```
-        
-        PS: fine-tuned result model is GPT2-python: [shibing624/autocoder-gpt2-base](https://huggingface.co/shibing624/autocoder-gpt2-base), 
-        i spent about 24 hours with V100 to fine-tune it. 
-        
-        ## Server
-        
-        start FastAPI server:
-        
-        example: [server.py](./examples/server.py)
-        
-        ```shell
-        cd examples
-        python server.py
-        ```
-        
-        open url: http://0.0.0.0:8001/docs
-        
-        ![api](./docs/api.png)
-        
-        # Contact
+        ## Contact
         
         - Issue(建议)
-          ：[![GitHub issues](https://img.shields.io/github/issues/shibing624/autocoder.svg)](https://github.com/shibing624/autocoder/issues)
+          ：[![GitHub issues](https://img.shields.io/github/issues/shibing624/codeassist.svg)](https://github.com/shibing624/codeassist/issues)
         - 邮件我：xuming: xuming624@qq.com
         - 微信我： 加我*微信号：xuming624, 备注：个人名称-公司-NLP* 进NLP交流群。
         
         <img src="docs/wechat.jpeg" width="200" />
         
-        # Citation
+        ## Citation
         
-        如果你在研究中使用了autocoder，请按如下格式引用：
+        如果你在研究中使用了codeassist，请按如下格式引用：
         
         APA:
         ```latex
-        Xu, M. AutoCoder: Code AutoComplete with GPT2 model (Version 0.0.4) [Computer software]. https://github.com/shibing624/autocoder
+        Xu, M. codeassist: Code AutoComplete with GPT model (Version 1.0.0) [Computer software]. https://github.com/shibing624/codeassist
         ```
         
         BibTeX:
         ```latex
-        @software{Xu_autocoder_Code_AutoComplete,
-        author = {Xu, Ming},
-        title = {autocoder: Code AutoComplete with Code model},
-        url = {https://github.com/shibing624/autocoder},
-        version = {0.1.0}
+        @software{Xu_codeassist,
+        author = {Ming Xu},
+        title = {CodeAssist: Code AutoComplete with Generation model},
+        url = {https://github.com/shibing624/codeassist},
+        version = {1.0.0}
         }
         ```
         
-        # License
+        ## License
+        This repository is licensed under the [The Apache License 2.0](LICENSE).
+        
+        Please follow the [Attribution-NonCommercial 4.0 International](https://github.com/nlpxucan/WizardLM/blob/main/WizardCoder/MODEL_WEIGHTS_LICENSE) to use the WizardCoder model.
         
-        授权协议为 [The Apache License 2.0](/LICENSE)，可免费用做商业用途。请在产品说明中附加autocoder的链接和授权协议。
         
-        # Contribute
+        ## Contribute
         
         项目代码还很粗糙，如果大家对代码有所改进，欢迎提交回本项目，在提交之前，注意以下两点：
         
         - 在`tests`添加相应的单元测试
         - 使用`python setup.py test`来运行所有单元测试，确保所有单测都是通过的
         
         之后即可提交PR。
         
-        # Reference
+        ## Reference
         
         - [gpt-2-simple](https://github.com/minimaxir/gpt-2-simple)
         - [galois-autocompleter](https://github.com/galois-autocompleter/galois-autocompleter)
+        - [WizardLM/WizardCoder-15B-V1.0](https://huggingface.co/WizardLM/WizardCoder-15B-V1.0)
         
 Keywords: CodeGenie,autocomplete,code-autocomplete
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Natural Language :: Chinese (Traditional)
```

### Comparing `codeassist-0.1.0/README.md` & `codeassist-1.0.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,164 +1,185 @@
-[![PyPI version](https://badge.fury.io/py/autocoder.svg)](https://badge.fury.io/py/autocoder)
+[**🇨🇳中文**](https://github.com/shibing624/codeassist/blob/main/README.md) | [**🌐English**](https://github.com/shibing624/codeassist/blob/main/README_EN.md) | [**📖文档/Docs**](https://github.com/shibing624/codeassist/wiki) | [**🤖模型/Models**](https://huggingface.co/shibing624) 
+
+<div align="center">
+  <a href="https://github.com/shibing624/codeassist">
+    <img src="https://github.com/shibing624/codeassist/blob/main/docs/codeassist.png" height="130" alt="Logo">
+  </a>
+</div>
+
+-----------------
+
+# CodeAssist: Advanced Code Completion Tool
+[![PyPI version](https://badge.fury.io/py/codeassist.svg)](https://badge.fury.io/py/codeassist)
 [![Contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)](CONTRIBUTING.md)
-[![GitHub contributors](https://img.shields.io/github/contributors/shibing624/autocoder.svg)](https://github.com/shibing624/autocoder/graphs/contributors)
+[![GitHub contributors](https://img.shields.io/github/contributors/shibing624/codeassist.svg)](https://github.com/shibing624/codeassist/graphs/contributors)
 [![License Apache 2.0](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](LICENSE)
 [![python_vesion](https://img.shields.io/badge/Python-3.5%2B-green.svg)](requirements.txt)
-[![GitHub issues](https://img.shields.io/github/issues/shibing624/autocoder.svg)](https://github.com/shibing624/autocoder/issues)
+[![GitHub issues](https://img.shields.io/github/issues/shibing624/codeassist.svg)](https://github.com/shibing624/codeassist/issues)
 [![Wechat Group](http://vlog.sfyc.ltd/wechat_everyday/wxgroup_logo.png?imageView2/0/w/60/h/20)](#Contact)
 
-# AutoCoder
-
-**AutoCoder** is an advanced code completion tool that intelligently provides high-quality code completions for Python, Java, and C++ and so on. 
+## Introduction
 
-AutoCoder 是一个高级代码补全工具，能智能地为 Python、Java 和 C++ 等编程语言高质量补全代码
+**CodeAssist** is an advanced code completion tool that intelligently provides high-quality code completions for Python, Java, and C++ and so on. 
 
+CodeAssist 是一个高级代码补全工具，高质量为 Python、Java 和 C++ 等编程语言补全代码
 
-**Guide**
 
-- [Feature](#Feature)
-- [Install](#install)
-- [Usage](#usage)
-- [Contact](#Contact)
-- [Citation](#Citation)
-- [Reference](#reference)
+## Features
 
-# Feature
-
-- GPT2-based code completion
-- Code completion for Python, other language is coming soon
+- GPT based code completion
+- Code completion for `Python`, `Java`, `C++`, `javascript` and so on
 - Line and block code completion
-- Train(Fine-tune GPT2) and predict model with your own data
+- Train(Fine-tuning) and predict model with your own data
+
+### Release Models
 
+| Arch   | BaseModel         | Model                                                                                                                   | Model Size | 
+|:-------|:------------------|:------------------------------------------------------------------------------------------------------------------------|:----------:|
+| GPT   | gpt2              | [shibing624/code-autocomplete-gpt2-base](https://huggingface.co/shibing624/code-autocomplete-gpt2-base)                 |   487MB    |
+| GPT   | distilgpt2        | [shibing624/code-autocomplete-distilgpt2-python](https://huggingface.co/shibing624/code-autocomplete-distilgpt2-python) |   319MB    |
+| GPT   | bigcode/starcoder | [WizardLM/WizardCoder-15B-V1.0](https://huggingface.co/WizardLM/WizardCoder-15B-V1.0)                                   |    29GB    |
 
-# Demo
 
+### Demo
 
 HuggingFace Demo: https://huggingface.co/spaces/shibing624/code-autocomplete
 
-# Install
+backend model: `shibing624/code-autocomplete-gpt2-base`
 
-```
+## Install
+
+```shell
 pip install torch # conda install pytorch
-pip install -U autocoder
+pip install -U codeassist
 ```
 
 or
 
-```
-git clone https://github.com/shibing624/autocoder.git
-cd AutoCoder
+```shell
+git clone https://github.com/shibing624/codeassist.git
+cd CodeAssist
 python setup.py install
 ```
 
-# Usage
+## Usage
+
+### WizardCoder model
 
-## Code Completion
+WizardCoder-15b is fine-tuned `bigcode/starcoder` with alpaca code data, you can use the following code to generate code:
 
-Model upload to HF's model hub:
+example: [examples/wizardcoder_demo.py](https://github.com/shibing624/CodeAssist/blob/main/examples/wizardcoder_demo.py)
 
-- DistilGPT2-python: [shibing624/code-autocomplete-distilgpt2-python](https://huggingface.co/shibing624/code-autocomplete-distilgpt2-python) (fine-tuned distilgpt2, model size: 319MB)
-- GPT2-python: [shibing624/code-autocomplete-gpt2-base](https://huggingface.co/shibing624/code-autocomplete-gpt2-base) (fine-tuned gpt2, model size: 487MB)
+```python
+import sys
+
+sys.path.append('..')
+from codeassist import WizardCoder
 
-![hf](docs/hf_model.png)
+m = WizardCoder("WizardLM/WizardCoder-15B-V1.0")
+print(m.generate('def load_csv_file(file_path):')[0])
+```
 
-### Use with autocoder
+output:
 
-example: [base_demo.py](./examples/base_demo.py)
 
 ```python
-from autocoder import GPT2Coder
+import csv
 
-m = GPT2Coder("shibing624/code-autocomplete-gpt2-base")
-print(m.generate('import torch.nn as')[0])
+def load_csv_file(file_path):
+    """
+    Load data from a CSV file and return a list of dictionaries.
+    """
+    # Open the file in read mode
+    with open(file_path, 'r') as file:
+        # Create a CSV reader object
+        csv_reader = csv.DictReader(file)
+        # Initialize an empty list to store the data
+        data = []
+        # Iterate over each row of data
+        for row in csv_reader:
+            # Append the row of data to the list
+            data.append(row)
+    # Return the list of data
+    return data
 ```
 
+model output is impressively effective, it currently supports English and Chinese input, you can enter instructions or code prefixes as required.
+
+### distilgpt2 model
+
+
 distilgpt2 fine-tuned code autocomplete model, you can use the following code:
 
-example: [distilgpt2_demo.py](./examples/distilgpt2_demo.py)
+example: [examples/distilgpt2_demo.py](https://github.com/shibing624/CodeAssist/blob/main/examples/distilgpt2_demo.py)
 
 ```python
 import sys
 
 sys.path.append('..')
-from autocoder import GPT2Coder
+from codeassist import GPT2Coder
 
 m = GPT2Coder("shibing624/code-autocomplete-distilgpt2-python")
 print(m.generate('import torch.nn as')[0])
 ```
 
 output:
 
 ```shell
 import torch.nn as nn
 import torch.nn.functional as F
 ```
 
 ### Use with huggingface/transformers：
 
-example: [use_transformers_gpt2.py](./examples/use_transformers_gpt2.py)
+example: [examples/use_transformers_gpt2.py](https://github.com/shibing624/CodeAssist/blob/main/examples/use_transformers_gpt2.py)
 
-*Please use 'GPT2' related functions to load this model!*
+### Train Model
+#### Train WizardCoder model
+example: [examples/training_wizardcoder_mydata.py](https://github.com/shibing624/CodeAssist/blob/main/examples/training_wizardcoder_mydata.py)
 
-```python
+```shell
+cd examples
+CUDA_VISIBLE_DEVICES=0,1 python training_wizardcoder_mydata.py --do_train --do_predict --num_epochs 1 --output_dir outputs-wizard --model_name WizardLM/WizardCoder-15B-V1.0
+```
 
-import os
-from transformers import GPT2Tokenizer, GPT2LMHeadModel
+- GPU memory: 31GB
+- finetune need 2*V100(32GB)
+- inference need 1*V100(32GB)
 
-os.environ["KMP_DUPLICATE_LIB_OK"] = "TRUE"
+#### Train distilgpt2 model
+example: [examples/training_gpt2_mydata.py](https://github.com/shibing624/CodeAssist/blob/main/examples/training_gpt2_mydata.py)
 
-tokenizer = GPT2Tokenizer.from_pretrained("shibing624/autocoder-gpt2-base")
-model = GPT2LMHeadModel.from_pretrained("shibing624/autocoder-gpt2-base")
-prompts = [
-    "import numpy as np",
-    "import torch.nn as",
-    'parser.add_argument("--num_train_epochs",',
-    "def set_seed(",
-    "def factorial",
-]
-for prompt in prompts:
-    input_ids = tokenizer(prompt, return_tensors='pt').input_ids
-    outputs = model.generate(input_ids=input_ids,
-                             max_length=64 + len(input_ids[0]),
-                             temperature=1.0,
-                             top_k=50,
-                             top_p=0.95,
-                             repetition_penalty=1.0,
-                             do_sample=True,
-                             num_return_sequences=1,
-                             length_penalty=2.0,
-                             early_stopping=True,
-                             pad_token_id=tokenizer.eos_token_id,
-                             eos_token_id=tokenizer.eos_token_id,
-                             )
-    decoded = tokenizer.decode(outputs[0], skip_special_tokens=True)
-    print("Input :", prompt)
-    print("Output:", decoded)
-    print("=" * 20)
+```shell
+cd examples
+python training_gpt2_mydata.py --do_train --do_predict --num_epochs 15 --output_dir outputs-gpt2 --model_name gpt2
 ```
 
-output:
+PS: fine-tuned result model is GPT2-python: [shibing624/code-autocomplete-gpt2-base](https://huggingface.co/shibing624/code-autocomplete-gpt2-base), 
+I spent about 24 hours with V100 to fine-tune it. 
+
+
+### Server
+
+start FastAPI server:
+
+example: [examples/server.py](https://github.com/shibing624/CodeAssist/blob/main/examples/server.py)
 
 ```shell
-import numpy as np
-====================
-import torch.nn as nn
-import torchvision.transforms as transforms
-====================
-parser.add_argument("--num_train_epochs", type=int, default=50, help="Number of training epochs.")
-parser.add_argument("--batch_size", type=int, default=32, help="Batch size of validation/test data.")
-====================
-def set_seed(self):
-====================
-def factorial(n: int) -> int:
+cd examples
+python server.py
 ```
 
-## Train your own model with Dataset
+open url: http://0.0.0.0:8001/docs
+
+![api](https://github.com/shibing624/CodeAssist/blob/main/docs/api.png)
+
 
-### Build dataset
+
+## Dataset
 
 This allows to customize dataset building. Below is an example of the building process.
 
 Let's use Python codes from [Awesome-pytorch-list](https://github.com/bharathgs/Awesome-pytorch-list)
 
 1. We want the model to help auto-complete codes at a general level. The codes of The Algorithms suits the need.
 2. This code from this project is well written (high-quality codes).
@@ -172,18 +193,14 @@
 └── test.txt
 ```
 
 There are three ways to build dataset:
 1. Use the huggingface/datasets library load the dataset
 huggingface datasets [https://huggingface.co/datasets/shibing624/source_code](https://huggingface.co/datasets/shibing624/source_code)
 
-```shell
-pip install datasets
-```
-
 ```python
 from datasets import load_dataset
 dataset = load_dataset("shibing624/source_code", "python") # python or java or cpp
 print(dataset)
 print(dataset['test'][0:10])
 ```
 
@@ -215,92 +232,69 @@
 ]}
 ```
 
 2. Download dataset from Cloud
 
 | Name | Source | Download | Size |
 | :------- | :--------- | :---------: | :---------: |
-| Python+Java+CPP source code | Awesome-pytorch-list(5.22 Million lines) | [github_source_code.zip](https://github.com/shibing624/autocoder/releases/download/0.0.4/source_code.zip) | 105M |
+| Python+Java+CPP source code | Awesome-pytorch-list(5.22 Million lines) | [github_source_code.zip](https://github.com/shibing624/codeassist/releases/download/0.0.4/source_code.zip) | 105M |
 
 download dataset and unzip it, put to `examples/`.
 
 3. Get source code from scratch and build dataset
 
-[prepare_data.py](./examples/prepare_data.py)
+[prepare_code_data.py](https://github.com/shibing624/CodeAssist/blob/main/examples/prepare_code_data.py)
 
 ```shell
 cd examples
-python prepare_data.py --num_repos 260
+python prepare_code_data.py --num_repos 260
 ```
 
-### Train and predict model
 
-example: [train_gpt2.py](./examples/train_gpt2.py)
-
-```shell
-cd examples
-python training_gpt2_mydata.py --do_train --do_predict --num_epochs 15 --model_dir outputs-fine-tuned --model_name gpt2
-```
-
-PS: fine-tuned result model is GPT2-python: [shibing624/autocoder-gpt2-base](https://huggingface.co/shibing624/autocoder-gpt2-base), 
-i spent about 24 hours with V100 to fine-tune it. 
-
-## Server
-
-start FastAPI server:
-
-example: [server.py](./examples/server.py)
-
-```shell
-cd examples
-python server.py
-```
-
-open url: http://0.0.0.0:8001/docs
-
-![api](./docs/api.png)
-
-# Contact
+## Contact
 
 - Issue(建议)
-  ：[![GitHub issues](https://img.shields.io/github/issues/shibing624/autocoder.svg)](https://github.com/shibing624/autocoder/issues)
+  ：[![GitHub issues](https://img.shields.io/github/issues/shibing624/codeassist.svg)](https://github.com/shibing624/codeassist/issues)
 - 邮件我：xuming: xuming624@qq.com
 - 微信我： 加我*微信号：xuming624, 备注：个人名称-公司-NLP* 进NLP交流群。
 
 <img src="docs/wechat.jpeg" width="200" />
 
-# Citation
+## Citation
 
-如果你在研究中使用了autocoder，请按如下格式引用：
+如果你在研究中使用了codeassist，请按如下格式引用：
 
 APA:
 ```latex
-Xu, M. AutoCoder: Code AutoComplete with GPT2 model (Version 0.0.4) [Computer software]. https://github.com/shibing624/autocoder
+Xu, M. codeassist: Code AutoComplete with GPT model (Version 1.0.0) [Computer software]. https://github.com/shibing624/codeassist
 ```
 
 BibTeX:
 ```latex
-@software{Xu_autocoder_Code_AutoComplete,
-author = {Xu, Ming},
-title = {autocoder: Code AutoComplete with Code model},
-url = {https://github.com/shibing624/autocoder},
-version = {0.1.0}
+@software{Xu_codeassist,
+author = {Ming Xu},
+title = {CodeAssist: Code AutoComplete with Generation model},
+url = {https://github.com/shibing624/codeassist},
+version = {1.0.0}
 }
 ```
 
-# License
+## License
+This repository is licensed under the [The Apache License 2.0](LICENSE).
+
+Please follow the [Attribution-NonCommercial 4.0 International](https://github.com/nlpxucan/WizardLM/blob/main/WizardCoder/MODEL_WEIGHTS_LICENSE) to use the WizardCoder model.
 
-授权协议为 [The Apache License 2.0](/LICENSE)，可免费用做商业用途。请在产品说明中附加autocoder的链接和授权协议。
 
-# Contribute
+## Contribute
 
 项目代码还很粗糙，如果大家对代码有所改进，欢迎提交回本项目，在提交之前，注意以下两点：
 
 - 在`tests`添加相应的单元测试
 - 使用`python setup.py test`来运行所有单元测试，确保所有单测都是通过的
 
 之后即可提交PR。
 
-# Reference
+## Reference
 
 - [gpt-2-simple](https://github.com/minimaxir/gpt-2-simple)
 - [galois-autocompleter](https://github.com/galois-autocompleter/galois-autocompleter)
+- [WizardLM/WizardCoder-15B-V1.0](https://huggingface.co/WizardLM/WizardCoder-15B-V1.0)
```

### Comparing `codeassist-0.1.0/autocoder/create_dataset.py` & `codeassist-1.0.0/codeassist/create_dataset.py`

 * *Files identical despite different names*

### Comparing `codeassist-0.1.0/autocoder/gpt2_coder.py` & `codeassist-1.0.0/codeassist/gpt2_coder.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,50 +12,49 @@
 import numpy as np
 import pandas as pd
 import torch
 from loguru import logger
 from torch.nn.utils.rnn import pad_sequence
 from torch.utils.data import DataLoader, Dataset, RandomSampler, SequentialSampler
 from torch.utils.data.distributed import DistributedSampler
-from tqdm.auto import tqdm, trange
+from tqdm import tqdm, trange
 from transformers import GPT2LMHeadModel, GPT2Tokenizer
 from transformers.data.datasets.language_modeling import TextDataset
 from transformers.optimization import AdamW, get_linear_schedule_with_warmup
 
 os.environ["KMP_DUPLICATE_LIB_OK"] = "TRUE"
 device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
 
 
 class GPT2Coder:
     def __init__(
             self,
-            model_name_or_path: str,
-            max_seq_length: int = 128,
+            model_name_or_path: str = "shibing624/code-autocomplete-gpt2-base",
+            max_length: int = 128,
             do_lower_case: bool = False,
             special_words_dict: Dict = None
     ):
         """
         Initializes a GPT2 LanguageModelingModel.
     
         Args:
             model_name_or_path: Default Transformer model name or path to a directory containing Transformer model file (pytorch_nodel.bin).
-            max_seq_length: The maximum total input sequence length after tokenization.
+            max_length: The maximum total input sequence length after tokenization.
             do_lower_case: Set this flag if you are using an uncased model.
             special_words_dict: A dictionary of special words and their token ids.
         """
         self.model_name_or_path = model_name_or_path
         self.do_lower_case = do_lower_case
-        if max_seq_length > 1024:
-            logger.warning("GPT only allows a max_seq_length of 1024. Value will be set to 1024")
-            max_seq_length = 1024
-        self.max_seq_length = max_seq_length
+        if max_length > 1024:
+            logger.warning("GPT only allows a max_length of 1024. Value will be set to 1024")
+            max_length = 1024
+        self.max_length = max_length
         self.model = GPT2LMHeadModel.from_pretrained(model_name_or_path)
         self.model.to(device)
         self.tokenizer = GPT2Tokenizer.from_pretrained(model_name_or_path, do_lower_case=do_lower_case)
-        # When download from transformers, cache dir: ~/.cache/huggingface/transformers/
         if special_words_dict is not None:
             self.add_special_words(special_words_dict)
         self.results = {}
 
     def set_seed(self, seed):
         logger.debug(f"Set seed for random, numpy and torch: {seed}")
         random.seed(seed)
@@ -107,15 +106,15 @@
             max_steps (optional): If > 0: set total number of training steps to perform. Override num_epochs.
         Returns:
             global_step: Number of global steps trained
             training_details: Average training loss if evaluate_during_training is False or full training progress scores if evaluate_during_training is True
         """
         os.makedirs(output_dir, exist_ok=True)
         self.model.to(device)
-        train_dataset = TextDataset(self.tokenizer, train_file, self.max_seq_length, overwrite_cache=True,
+        train_dataset = TextDataset(self.tokenizer, train_file, self.max_length, overwrite_cache=True,
                                     cache_dir=output_dir)
 
         global_step, training_details = self.train(
             train_dataset,
             output_dir,
             eval_file=eval_file,
             verbose=verbose,
@@ -284,15 +283,15 @@
 
     def eval_model(self, eval_file: str, output_dir: str = None, verbose: bool = True, batch_size: int = 16):
         """
         Evaluates the model on eval_df. Saves results to args.output_dir
             result: Dictionary containing evaluation results.
         """
         self.model.to(device)
-        eval_dataset = TextDataset(self.tokenizer, eval_file, self.max_seq_length, overwrite_cache=True)
+        eval_dataset = TextDataset(self.tokenizer, eval_file, self.max_length, overwrite_cache=True)
         result = self.evaluate(eval_dataset, output_dir, batch_size=batch_size)
         self.results.update(result)
 
         if verbose:
             logger.info(self.results)
 
         return result
@@ -359,32 +358,34 @@
                 for key in sorted(results.keys()):
                     writer.write("{} = {}\n".format(key, str(results[key])))
 
     def generate(
             self,
             prompt: str,
             is_add_prompt: bool = True,
+            max_length: int = 128,
             temperature: int = 1.0,
             top_k: int = 50,
             top_p: float = 0.95,
             repetition_penalty: float = 1.0,
             do_sample: bool = True,
             num_return_sequences: int = 1,
             length_penalty: float = 2.0,
             early_stopping: bool = True,
             stop_word: str = "\n\n",
             bad_words: list = None,
-            **kwargs
+            **kwargs,
     ):
         """
         Generate text using a GPT2 LanguageGenerationModel
 
         Args:
             prompt: A prompt text for the model.
             is_add_prompt: Whether to add the prompt to the returned text.
+            max_length: The maximum length of the sequence to be generated.
             temperature: The sampling temperature.
             top_k: The number of top k tokens to be considered by sampling.
             top_p: The sampling probability for top p tokens.
             repetition_penalty: The repetition penalty parameter.
             do_sample: Boolean value indicating whether to sample or greedy generate.
             num_return_sequences: The number of samples to return.
             length_penalty: The length penalty parameter.
@@ -397,15 +398,15 @@
         encoded_prompt = self.tokenizer(prompt, return_tensors="pt").to(device)
         encoded_prompt_ids = encoded_prompt.input_ids
         # Get tokens of words that should not be generated
         bad_words_ids = [self.tokenizer(bad_word, add_prefix_space=True).input_ids for bad_word in
                          bad_words] if bad_words else None
         output_sequences = self.model.generate(
             input_ids=encoded_prompt_ids,
-            max_length=self.max_seq_length + len(encoded_prompt_ids[0]),
+            max_length=max_length if max_length is not None else self.max_length,
             temperature=temperature,
             top_k=top_k,
             top_p=top_p,
             repetition_penalty=repetition_penalty,
             do_sample=do_sample,
             num_return_sequences=num_return_sequences,
             length_penalty=length_penalty,
```

### Comparing `codeassist-0.1.0/codeassist.egg-info/PKG-INFO` & `codeassist-1.0.0/codeassist.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,172 +1,193 @@
 Metadata-Version: 2.1
 Name: codeassist
-Version: 0.1.0
+Version: 1.0.0
 Summary: Code AutoComplete
 Home-page: https://github.com/shibing624/autocoder
 Author: XuMing
 Author-email: xuming624@qq.com
 License: Apache License 2.0
-Description: [![PyPI version](https://badge.fury.io/py/autocoder.svg)](https://badge.fury.io/py/autocoder)
+Description: [**🇨🇳中文**](https://github.com/shibing624/codeassist/blob/main/README.md) | [**🌐English**](https://github.com/shibing624/codeassist/blob/main/README_EN.md) | [**📖文档/Docs**](https://github.com/shibing624/codeassist/wiki) | [**🤖模型/Models**](https://huggingface.co/shibing624) 
+        
+        <div align="center">
+          <a href="https://github.com/shibing624/codeassist">
+            <img src="https://github.com/shibing624/codeassist/blob/main/docs/codeassist.png" height="130" alt="Logo">
+          </a>
+        </div>
+        
+        -----------------
+        
+        # CodeAssist: Advanced Code Completion Tool
+        [![PyPI version](https://badge.fury.io/py/codeassist.svg)](https://badge.fury.io/py/codeassist)
         [![Contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg)](CONTRIBUTING.md)
-        [![GitHub contributors](https://img.shields.io/github/contributors/shibing624/autocoder.svg)](https://github.com/shibing624/autocoder/graphs/contributors)
+        [![GitHub contributors](https://img.shields.io/github/contributors/shibing624/codeassist.svg)](https://github.com/shibing624/codeassist/graphs/contributors)
         [![License Apache 2.0](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](LICENSE)
         [![python_vesion](https://img.shields.io/badge/Python-3.5%2B-green.svg)](requirements.txt)
-        [![GitHub issues](https://img.shields.io/github/issues/shibing624/autocoder.svg)](https://github.com/shibing624/autocoder/issues)
+        [![GitHub issues](https://img.shields.io/github/issues/shibing624/codeassist.svg)](https://github.com/shibing624/codeassist/issues)
         [![Wechat Group](http://vlog.sfyc.ltd/wechat_everyday/wxgroup_logo.png?imageView2/0/w/60/h/20)](#Contact)
         
-        # AutoCoder
-        
-        **AutoCoder** is an advanced code completion tool that intelligently provides high-quality code completions for Python, Java, and C++ and so on. 
+        ## Introduction
         
-        AutoCoder 是一个高级代码补全工具，能智能地为 Python、Java 和 C++ 等编程语言高质量补全代码
+        **CodeAssist** is an advanced code completion tool that intelligently provides high-quality code completions for Python, Java, and C++ and so on. 
         
+        CodeAssist 是一个高级代码补全工具，高质量为 Python、Java 和 C++ 等编程语言补全代码
         
-        **Guide**
         
-        - [Feature](#Feature)
-        - [Install](#install)
-        - [Usage](#usage)
-        - [Contact](#Contact)
-        - [Citation](#Citation)
-        - [Reference](#reference)
+        ## Features
         
-        # Feature
-        
-        - GPT2-based code completion
-        - Code completion for Python, other language is coming soon
+        - GPT based code completion
+        - Code completion for `Python`, `Java`, `C++`, `javascript` and so on
         - Line and block code completion
-        - Train(Fine-tune GPT2) and predict model with your own data
+        - Train(Fine-tuning) and predict model with your own data
+        
+        ### Release Models
         
+        | Arch   | BaseModel         | Model                                                                                                                   | Model Size | 
+        |:-------|:------------------|:------------------------------------------------------------------------------------------------------------------------|:----------:|
+        | GPT   | gpt2              | [shibing624/code-autocomplete-gpt2-base](https://huggingface.co/shibing624/code-autocomplete-gpt2-base)                 |   487MB    |
+        | GPT   | distilgpt2        | [shibing624/code-autocomplete-distilgpt2-python](https://huggingface.co/shibing624/code-autocomplete-distilgpt2-python) |   319MB    |
+        | GPT   | bigcode/starcoder | [WizardLM/WizardCoder-15B-V1.0](https://huggingface.co/WizardLM/WizardCoder-15B-V1.0)                                   |    29GB    |
         
-        # Demo
         
+        ### Demo
         
         HuggingFace Demo: https://huggingface.co/spaces/shibing624/code-autocomplete
         
-        # Install
+        backend model: `shibing624/code-autocomplete-gpt2-base`
         
-        ```
+        ## Install
+        
+        ```shell
         pip install torch # conda install pytorch
-        pip install -U autocoder
+        pip install -U codeassist
         ```
         
         or
         
-        ```
-        git clone https://github.com/shibing624/autocoder.git
-        cd AutoCoder
+        ```shell
+        git clone https://github.com/shibing624/codeassist.git
+        cd CodeAssist
         python setup.py install
         ```
         
-        # Usage
+        ## Usage
+        
+        ### WizardCoder model
         
-        ## Code Completion
+        WizardCoder-15b is fine-tuned `bigcode/starcoder` with alpaca code data, you can use the following code to generate code:
         
-        Model upload to HF's model hub:
+        example: [examples/wizardcoder_demo.py](https://github.com/shibing624/CodeAssist/blob/main/examples/wizardcoder_demo.py)
         
-        - DistilGPT2-python: [shibing624/code-autocomplete-distilgpt2-python](https://huggingface.co/shibing624/code-autocomplete-distilgpt2-python) (fine-tuned distilgpt2, model size: 319MB)
-        - GPT2-python: [shibing624/code-autocomplete-gpt2-base](https://huggingface.co/shibing624/code-autocomplete-gpt2-base) (fine-tuned gpt2, model size: 487MB)
+        ```python
+        import sys
+        
+        sys.path.append('..')
+        from codeassist import WizardCoder
         
-        ![hf](docs/hf_model.png)
+        m = WizardCoder("WizardLM/WizardCoder-15B-V1.0")
+        print(m.generate('def load_csv_file(file_path):')[0])
+        ```
         
-        ### Use with autocoder
+        output:
         
-        example: [base_demo.py](./examples/base_demo.py)
         
         ```python
-        from autocoder import GPT2Coder
+        import csv
         
-        m = GPT2Coder("shibing624/code-autocomplete-gpt2-base")
-        print(m.generate('import torch.nn as')[0])
+        def load_csv_file(file_path):
+            """
+            Load data from a CSV file and return a list of dictionaries.
+            """
+            # Open the file in read mode
+            with open(file_path, 'r') as file:
+                # Create a CSV reader object
+                csv_reader = csv.DictReader(file)
+                # Initialize an empty list to store the data
+                data = []
+                # Iterate over each row of data
+                for row in csv_reader:
+                    # Append the row of data to the list
+                    data.append(row)
+            # Return the list of data
+            return data
         ```
         
+        model output is impressively effective, it currently supports English and Chinese input, you can enter instructions or code prefixes as required.
+        
+        ### distilgpt2 model
+        
+        
         distilgpt2 fine-tuned code autocomplete model, you can use the following code:
         
-        example: [distilgpt2_demo.py](./examples/distilgpt2_demo.py)
+        example: [examples/distilgpt2_demo.py](https://github.com/shibing624/CodeAssist/blob/main/examples/distilgpt2_demo.py)
         
         ```python
         import sys
         
         sys.path.append('..')
-        from autocoder import GPT2Coder
+        from codeassist import GPT2Coder
         
         m = GPT2Coder("shibing624/code-autocomplete-distilgpt2-python")
         print(m.generate('import torch.nn as')[0])
         ```
         
         output:
         
         ```shell
         import torch.nn as nn
         import torch.nn.functional as F
         ```
         
         ### Use with huggingface/transformers：
         
-        example: [use_transformers_gpt2.py](./examples/use_transformers_gpt2.py)
+        example: [examples/use_transformers_gpt2.py](https://github.com/shibing624/CodeAssist/blob/main/examples/use_transformers_gpt2.py)
         
-        *Please use 'GPT2' related functions to load this model!*
+        ### Train Model
+        #### Train WizardCoder model
+        example: [examples/training_wizardcoder_mydata.py](https://github.com/shibing624/CodeAssist/blob/main/examples/training_wizardcoder_mydata.py)
         
-        ```python
+        ```shell
+        cd examples
+        CUDA_VISIBLE_DEVICES=0,1 python training_wizardcoder_mydata.py --do_train --do_predict --num_epochs 1 --output_dir outputs-wizard --model_name WizardLM/WizardCoder-15B-V1.0
+        ```
         
-        import os
-        from transformers import GPT2Tokenizer, GPT2LMHeadModel
+        - GPU memory: 31GB
+        - finetune need 2*V100(32GB)
+        - inference need 1*V100(32GB)
         
-        os.environ["KMP_DUPLICATE_LIB_OK"] = "TRUE"
+        #### Train distilgpt2 model
+        example: [examples/training_gpt2_mydata.py](https://github.com/shibing624/CodeAssist/blob/main/examples/training_gpt2_mydata.py)
         
-        tokenizer = GPT2Tokenizer.from_pretrained("shibing624/autocoder-gpt2-base")
-        model = GPT2LMHeadModel.from_pretrained("shibing624/autocoder-gpt2-base")
-        prompts = [
-            "import numpy as np",
-            "import torch.nn as",
-            'parser.add_argument("--num_train_epochs",',
-            "def set_seed(",
-            "def factorial",
-        ]
-        for prompt in prompts:
-            input_ids = tokenizer(prompt, return_tensors='pt').input_ids
-            outputs = model.generate(input_ids=input_ids,
-                                     max_length=64 + len(input_ids[0]),
-                                     temperature=1.0,
-                                     top_k=50,
-                                     top_p=0.95,
-                                     repetition_penalty=1.0,
-                                     do_sample=True,
-                                     num_return_sequences=1,
-                                     length_penalty=2.0,
-                                     early_stopping=True,
-                                     pad_token_id=tokenizer.eos_token_id,
-                                     eos_token_id=tokenizer.eos_token_id,
-                                     )
-            decoded = tokenizer.decode(outputs[0], skip_special_tokens=True)
-            print("Input :", prompt)
-            print("Output:", decoded)
-            print("=" * 20)
+        ```shell
+        cd examples
+        python training_gpt2_mydata.py --do_train --do_predict --num_epochs 15 --output_dir outputs-gpt2 --model_name gpt2
         ```
         
-        output:
+        PS: fine-tuned result model is GPT2-python: [shibing624/code-autocomplete-gpt2-base](https://huggingface.co/shibing624/code-autocomplete-gpt2-base), 
+        I spent about 24 hours with V100 to fine-tune it. 
+        
+        
+        ### Server
+        
+        start FastAPI server:
+        
+        example: [examples/server.py](https://github.com/shibing624/CodeAssist/blob/main/examples/server.py)
         
         ```shell
-        import numpy as np
-        ====================
-        import torch.nn as nn
-        import torchvision.transforms as transforms
-        ====================
-        parser.add_argument("--num_train_epochs", type=int, default=50, help="Number of training epochs.")
-        parser.add_argument("--batch_size", type=int, default=32, help="Batch size of validation/test data.")
-        ====================
-        def set_seed(self):
-        ====================
-        def factorial(n: int) -> int:
+        cd examples
+        python server.py
         ```
         
-        ## Train your own model with Dataset
+        open url: http://0.0.0.0:8001/docs
+        
+        ![api](https://github.com/shibing624/CodeAssist/blob/main/docs/api.png)
+        
         
-        ### Build dataset
+        
+        ## Dataset
         
         This allows to customize dataset building. Below is an example of the building process.
         
         Let's use Python codes from [Awesome-pytorch-list](https://github.com/bharathgs/Awesome-pytorch-list)
         
         1. We want the model to help auto-complete codes at a general level. The codes of The Algorithms suits the need.
         2. This code from this project is well written (high-quality codes).
@@ -180,18 +201,14 @@
         └── test.txt
         ```
         
         There are three ways to build dataset:
         1. Use the huggingface/datasets library load the dataset
         huggingface datasets [https://huggingface.co/datasets/shibing624/source_code](https://huggingface.co/datasets/shibing624/source_code)
         
-        ```shell
-        pip install datasets
-        ```
-        
         ```python
         from datasets import load_dataset
         dataset = load_dataset("shibing624/source_code", "python") # python or java or cpp
         print(dataset)
         print(dataset['test'][0:10])
         ```
         
@@ -223,99 +240,76 @@
         ]}
         ```
         
         2. Download dataset from Cloud
         
         | Name | Source | Download | Size |
         | :------- | :--------- | :---------: | :---------: |
-        | Python+Java+CPP source code | Awesome-pytorch-list(5.22 Million lines) | [github_source_code.zip](https://github.com/shibing624/autocoder/releases/download/0.0.4/source_code.zip) | 105M |
+        | Python+Java+CPP source code | Awesome-pytorch-list(5.22 Million lines) | [github_source_code.zip](https://github.com/shibing624/codeassist/releases/download/0.0.4/source_code.zip) | 105M |
         
         download dataset and unzip it, put to `examples/`.
         
         3. Get source code from scratch and build dataset
         
-        [prepare_data.py](./examples/prepare_data.py)
+        [prepare_code_data.py](https://github.com/shibing624/CodeAssist/blob/main/examples/prepare_code_data.py)
         
         ```shell
         cd examples
-        python prepare_data.py --num_repos 260
+        python prepare_code_data.py --num_repos 260
         ```
         
-        ### Train and predict model
         
-        example: [train_gpt2.py](./examples/train_gpt2.py)
-        
-        ```shell
-        cd examples
-        python training_gpt2_mydata.py --do_train --do_predict --num_epochs 15 --model_dir outputs-fine-tuned --model_name gpt2
-        ```
-        
-        PS: fine-tuned result model is GPT2-python: [shibing624/autocoder-gpt2-base](https://huggingface.co/shibing624/autocoder-gpt2-base), 
-        i spent about 24 hours with V100 to fine-tune it. 
-        
-        ## Server
-        
-        start FastAPI server:
-        
-        example: [server.py](./examples/server.py)
-        
-        ```shell
-        cd examples
-        python server.py
-        ```
-        
-        open url: http://0.0.0.0:8001/docs
-        
-        ![api](./docs/api.png)
-        
-        # Contact
+        ## Contact
         
         - Issue(建议)
-          ：[![GitHub issues](https://img.shields.io/github/issues/shibing624/autocoder.svg)](https://github.com/shibing624/autocoder/issues)
+          ：[![GitHub issues](https://img.shields.io/github/issues/shibing624/codeassist.svg)](https://github.com/shibing624/codeassist/issues)
         - 邮件我：xuming: xuming624@qq.com
         - 微信我： 加我*微信号：xuming624, 备注：个人名称-公司-NLP* 进NLP交流群。
         
         <img src="docs/wechat.jpeg" width="200" />
         
-        # Citation
+        ## Citation
         
-        如果你在研究中使用了autocoder，请按如下格式引用：
+        如果你在研究中使用了codeassist，请按如下格式引用：
         
         APA:
         ```latex
-        Xu, M. AutoCoder: Code AutoComplete with GPT2 model (Version 0.0.4) [Computer software]. https://github.com/shibing624/autocoder
+        Xu, M. codeassist: Code AutoComplete with GPT model (Version 1.0.0) [Computer software]. https://github.com/shibing624/codeassist
         ```
         
         BibTeX:
         ```latex
-        @software{Xu_autocoder_Code_AutoComplete,
-        author = {Xu, Ming},
-        title = {autocoder: Code AutoComplete with Code model},
-        url = {https://github.com/shibing624/autocoder},
-        version = {0.1.0}
+        @software{Xu_codeassist,
+        author = {Ming Xu},
+        title = {CodeAssist: Code AutoComplete with Generation model},
+        url = {https://github.com/shibing624/codeassist},
+        version = {1.0.0}
         }
         ```
         
-        # License
+        ## License
+        This repository is licensed under the [The Apache License 2.0](LICENSE).
+        
+        Please follow the [Attribution-NonCommercial 4.0 International](https://github.com/nlpxucan/WizardLM/blob/main/WizardCoder/MODEL_WEIGHTS_LICENSE) to use the WizardCoder model.
         
-        授权协议为 [The Apache License 2.0](/LICENSE)，可免费用做商业用途。请在产品说明中附加autocoder的链接和授权协议。
         
-        # Contribute
+        ## Contribute
         
         项目代码还很粗糙，如果大家对代码有所改进，欢迎提交回本项目，在提交之前，注意以下两点：
         
         - 在`tests`添加相应的单元测试
         - 使用`python setup.py test`来运行所有单元测试，确保所有单测都是通过的
         
         之后即可提交PR。
         
-        # Reference
+        ## Reference
         
         - [gpt-2-simple](https://github.com/minimaxir/gpt-2-simple)
         - [galois-autocompleter](https://github.com/galois-autocompleter/galois-autocompleter)
+        - [WizardLM/WizardCoder-15B-V1.0](https://huggingface.co/WizardLM/WizardCoder-15B-V1.0)
         
 Keywords: CodeGenie,autocomplete,code-autocomplete
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Natural Language :: Chinese (Traditional)
```

### Comparing `codeassist-0.1.0/setup.py` & `codeassist-1.0.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup, find_packages
 
-__version__ = "0.1.0"
+__version__ = "1.0.0"
 
 with open('README.md', 'r', encoding='utf-8') as f:
     readme = f.read()
 
 setup(
     name='codeassist',
     version=__version__,
@@ -30,12 +30,14 @@
         'Topic :: Text Processing :: Linguistic',
     ],
     keywords='CodeGenie,autocomplete,code-autocomplete',
     install_requires=[
         "loguru",
         "transformers",
         "pandas",
+        "datasets",
+        "tqdm",
     ],
     packages=find_packages(exclude=['tests']),
     package_dir={'autocoder': 'autocoder'},
     package_data={'autocoder': ['*.*']}
 )
```

