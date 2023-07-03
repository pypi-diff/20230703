# Comparing `tmp/turbo_docs-1.0.1.tar.gz` & `tmp/turbo_docs-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turbo_docs-1.0.1.tar", last modified: Fri Jun 23 11:25:09 2023, max compression
+gzip compressed data, was "turbo_docs-1.0.2.tar", last modified: Mon Jul  3 17:56:36 2023, max compression
```

## Comparing `turbo_docs-1.0.1.tar` & `turbo_docs-1.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 11:25:09.307973 turbo_docs-1.0.1/
--rw-rw-rw-   0        0        0     2864 2023-06-23 11:25:09.306974 turbo_docs-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2367 2023-06-22 23:34:54.000000 turbo_docs-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-23 11:25:09.309291 turbo_docs-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      927 2023-06-23 11:24:56.000000 turbo_docs-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-23 11:25:09.244677 turbo_docs-1.0.1/turbo_docs/
--rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-1.0.1/turbo_docs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-23 11:25:09.294469 turbo_docs-1.0.1/turbo_docs/commands/
--rw-rw-rw-   0        0        0        0 2023-04-29 00:25:31.000000 turbo_docs-1.0.1/turbo_docs/commands/__init__.py
--rw-rw-rw-   0        0        0     1508 2023-06-23 11:18:24.000000 turbo_docs-1.0.1/turbo_docs/commands/docs.py
--rw-rw-rw-   0        0        0     1189 2023-06-22 23:34:54.000000 turbo_docs-1.0.1/turbo_docs/commands/readme.py
--rw-rw-rw-   0        0        0     1495 2023-06-23 11:19:54.000000 turbo_docs-1.0.1/turbo_docs/generate.py
-drwxrwxrwx   0        0        0        0 2023-06-23 11:25:09.303973 turbo_docs-1.0.1/turbo_docs/utils/
--rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-1.0.1/turbo_docs/utils/__init__.py
--rw-rw-rw-   0        0        0      826 2023-06-23 00:08:30.000000 turbo_docs-1.0.1/turbo_docs/utils/cli_options.py
--rw-rw-rw-   0        0        0     2114 2023-06-22 23:34:54.000000 turbo_docs-1.0.1/turbo_docs/utils/directory.py
--rw-rw-rw-   0        0        0      992 2023-06-23 11:09:55.000000 turbo_docs-1.0.1/turbo_docs/utils/openai_api.py
-drwxrwxrwx   0        0        0        0 2023-06-23 11:25:09.286466 turbo_docs-1.0.1/turbo_docs.egg-info/
--rw-rw-rw-   0        0        0     2864 2023-06-23 11:25:09.000000 turbo_docs-1.0.1/turbo_docs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      482 2023-06-23 11:25:09.000000 turbo_docs-1.0.1/turbo_docs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 11:25:09.000000 turbo_docs-1.0.1/turbo_docs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-06-23 11:25:09.000000 turbo_docs-1.0.1/turbo_docs.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       76 2023-06-23 11:25:09.000000 turbo_docs-1.0.1/turbo_docs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-23 11:25:09.000000 turbo_docs-1.0.1/turbo_docs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 17:56:36.511887 turbo_docs-1.0.2/
+-rw-rw-rw-   0        0        0     2833 2023-07-03 17:56:36.511887 turbo_docs-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2336 2023-07-03 17:25:01.000000 turbo_docs-1.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-03 17:56:36.512884 turbo_docs-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      927 2023-07-03 17:56:00.000000 turbo_docs-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 17:56:36.499167 turbo_docs-1.0.2/turbo_docs/
+-rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-1.0.2/turbo_docs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-03 17:56:36.505878 turbo_docs-1.0.2/turbo_docs/commands/
+-rw-rw-rw-   0        0        0        0 2023-04-29 00:25:31.000000 turbo_docs-1.0.2/turbo_docs/commands/__init__.py
+-rw-rw-rw-   0        0        0     2144 2023-07-03 17:25:01.000000 turbo_docs-1.0.2/turbo_docs/commands/docs.py
+-rw-rw-rw-   0        0        0     1038 2023-07-03 17:25:01.000000 turbo_docs-1.0.2/turbo_docs/commands/readme.py
+-rw-rw-rw-   0        0        0     2347 2023-07-03 17:55:45.000000 turbo_docs-1.0.2/turbo_docs/generate.py
+drwxrwxrwx   0        0        0        0 2023-07-03 17:56:36.510885 turbo_docs-1.0.2/turbo_docs/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-1.0.2/turbo_docs/utils/__init__.py
+-rw-rw-rw-   0        0        0      826 2023-07-03 17:25:01.000000 turbo_docs-1.0.2/turbo_docs/utils/cli_options.py
+-rw-rw-rw-   0        0        0     1760 2023-07-03 17:25:01.000000 turbo_docs-1.0.2/turbo_docs/utils/directory.py
+-rw-rw-rw-   0        0        0      799 2023-07-03 17:25:01.000000 turbo_docs-1.0.2/turbo_docs/utils/openai_api.py
+drwxrwxrwx   0        0        0        0 2023-07-03 17:56:36.503166 turbo_docs-1.0.2/turbo_docs.egg-info/
+-rw-rw-rw-   0        0        0     2833 2023-07-03 17:56:36.000000 turbo_docs-1.0.2/turbo_docs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      482 2023-07-03 17:56:36.000000 turbo_docs-1.0.2/turbo_docs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 17:56:36.000000 turbo_docs-1.0.2/turbo_docs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-07-03 17:56:36.000000 turbo_docs-1.0.2/turbo_docs.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       76 2023-07-03 17:56:36.000000 turbo_docs-1.0.2/turbo_docs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-03 17:56:36.000000 turbo_docs-1.0.2/turbo_docs.egg-info/top_level.txt
```

### Comparing `turbo_docs-1.0.1/PKG-INFO` & `turbo_docs-1.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,105 +1,92 @@
 Metadata-Version: 2.1
 Name: turbo_docs
-Version: 1.0.1
+Version: 1.0.2
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 
 # Turbo Docs 🚀
 
-[![PyPI version](https://badge.fury.io/py/turbo_docs.svg)](https://badge.fury.io/py/turbo_docs)
-[![GitHub stars](https://img.shields.io/github/stars/voynow/turbo-docs.svg)](https://github.com/voynow/turbo-docs/stargazers)
+![GitHub stars](https://img.shields.io/github/stars/voynow/turbo-docs?style=social)
+![PyPI](https://img.shields.io/pypi/v/turbo_docs)
 
-Turbo Docs is a powerful Python tool that helps developers automatically generate high-quality README.md files for their repositories. It leverages the power of OpenAI's GPT-3.5 Turbo and GPT-4 models to create well-structured, informative, and engaging documentation.
+Turbo Docs is a powerful Python package that automates the generation of documentation for your Python projects. It utilizes OpenAI's GPT models to create concise and informative documentation, making it easier for you and your users to understand your code.
 
-## Why Turbo Docs? 🤔
-
-Writing good documentation is essential for any software project, but it can be time-consuming and tedious. Turbo Docs simplifies this process by generating a README.md file that meets all your requirements, allowing you to focus on writing great code.
-
-## Table of Contents 📚
+## 📚 Table of Contents
 
+- [Why Use Turbo Docs?](#why-use-turbo-docs)
+- [Repo Structure](#repo-structure)
 - [Installation](#installation)
 - [Usage](#usage)
-- [Repo Structure](#repo-structure)
-- [Example Usage](#example-usage)
-- [Badges](#badges)
+- [Examples](#examples)
+- [Contributing](#contributing)
+- [License](#license)
+
+## 🎯 Why Use Turbo Docs?
+
+- **Save time**: Turbo Docs automatically generates documentation for your Python functions, so you can focus on writing code.
+- **Stay up-to-date**: Turbo Docs can be easily integrated into your development workflow, ensuring your documentation is always current.
+- **High-quality documentation**: Turbo Docs leverages the power of OpenAI's GPT models to generate concise and informative documentation.
+- **Customizable**: You can choose between GPT-3.5 Turbo and GPT-4 models, and even provide your own templates for generating documentation.
+
+## 🌳 Repo Structure
+
+```
+turbo_docs/
+├── commands/
+│   ├── docs.py
+│   ├── readme.py
+│   └── __init__.py
+├── utils/
+│   ├── cli_options.py
+│   ├── directory.py
+│   ├── openai_api.py
+│   └── __init__.py
+├── generate.py
+├── __init__.py
+├── setup.py
+├── requirements.txt
+└── turbo_docs.toml
+```
 
-## Installation 💻
+## 📦 Installation
 
 To install Turbo Docs, simply run:
 
 ```bash
 pip install turbo_docs
 ```
 
-## Usage 🛠️
+## 🛠 Usage
 
-To use Turbo Docs, navigate to your project's root directory and run:
+To generate documentation for your Python project, navigate to your project's root directory and run:
 
 ```bash
-turbo_docs --readme
+turbo_docs --docs
 ```
 
-This will generate a README.md file for your project. You can also use the `--gpt3` flag to use the GPT-3.5 Turbo model:
+To generate a README.md file for your project, run:
 
 ```bash
-turbo_docs --readme --gpt3
+turbo_docs --readme
 ```
 
-Additionally, you can copy the directory text to the clipboard by using the `--copy` flag:
+For more options, run:
 
 ```bash
-turbo_docs --copy
-```
-
-## Repo Structure 🏗️
-
-```
-turbo_docs/
-│
-├── commands/
-│   ├── __init__.py
-│   └── readme.py
-│
-├── utils/
-│   ├── __init__.py
-│   ├── cli_options.py
-│   ├── directory.py
-│   └── openai_api.py
-│
-├── __init__.py
-├── generate.py
-├── setup.py
-└── turbo_docs.toml
+turbo_docs --help
 ```
 
-## Example Usage 📖
+## 🤝 Contributing
 
-Here's an example of how to use Turbo Docs to generate a README.md file:
-
-```python
-from turbo_docs.commands import readme
-
-# Define your repo structure as a string
-repo = """
-{'repo': 'example_repo',
- 'files': {
-     'main.py': 'print("Hello, World!")',
-     'README.md': ''
- }
-}
-"""
-
-# Generate the README.md file
-readme(repo)
-```
+Contributions are welcome! Please feel free to submit a pull request or open an issue to discuss any improvements or suggestions.
 
-## License 📄
+## 📄 License
 
 Turbo Docs is released under the [MIT License](https://opensource.org/licenses/MIT).
```

### Comparing `turbo_docs-1.0.1/README.md` & `turbo_docs-1.0.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,92 +1,79 @@
 # Turbo Docs 🚀
 
-[![PyPI version](https://badge.fury.io/py/turbo_docs.svg)](https://badge.fury.io/py/turbo_docs)
-[![GitHub stars](https://img.shields.io/github/stars/voynow/turbo-docs.svg)](https://github.com/voynow/turbo-docs/stargazers)
+![GitHub stars](https://img.shields.io/github/stars/voynow/turbo-docs?style=social)
+![PyPI](https://img.shields.io/pypi/v/turbo_docs)
 
-Turbo Docs is a powerful Python tool that helps developers automatically generate high-quality README.md files for their repositories. It leverages the power of OpenAI's GPT-3.5 Turbo and GPT-4 models to create well-structured, informative, and engaging documentation.
+Turbo Docs is a powerful Python package that automates the generation of documentation for your Python projects. It utilizes OpenAI's GPT models to create concise and informative documentation, making it easier for you and your users to understand your code.
 
-## Why Turbo Docs? 🤔
-
-Writing good documentation is essential for any software project, but it can be time-consuming and tedious. Turbo Docs simplifies this process by generating a README.md file that meets all your requirements, allowing you to focus on writing great code.
-
-## Table of Contents 📚
+## 📚 Table of Contents
 
+- [Why Use Turbo Docs?](#why-use-turbo-docs)
+- [Repo Structure](#repo-structure)
 - [Installation](#installation)
 - [Usage](#usage)
-- [Repo Structure](#repo-structure)
-- [Example Usage](#example-usage)
-- [Badges](#badges)
+- [Examples](#examples)
+- [Contributing](#contributing)
+- [License](#license)
+
+## 🎯 Why Use Turbo Docs?
+
+- **Save time**: Turbo Docs automatically generates documentation for your Python functions, so you can focus on writing code.
+- **Stay up-to-date**: Turbo Docs can be easily integrated into your development workflow, ensuring your documentation is always current.
+- **High-quality documentation**: Turbo Docs leverages the power of OpenAI's GPT models to generate concise and informative documentation.
+- **Customizable**: You can choose between GPT-3.5 Turbo and GPT-4 models, and even provide your own templates for generating documentation.
+
+## 🌳 Repo Structure
+
+```
+turbo_docs/
+├── commands/
+│   ├── docs.py
+│   ├── readme.py
+│   └── __init__.py
+├── utils/
+│   ├── cli_options.py
+│   ├── directory.py
+│   ├── openai_api.py
+│   └── __init__.py
+├── generate.py
+├── __init__.py
+├── setup.py
+├── requirements.txt
+└── turbo_docs.toml
+```
 
-## Installation 💻
+## 📦 Installation
 
 To install Turbo Docs, simply run:
 
 ```bash
 pip install turbo_docs
 ```
 
-## Usage 🛠️
+## 🛠 Usage
 
-To use Turbo Docs, navigate to your project's root directory and run:
+To generate documentation for your Python project, navigate to your project's root directory and run:
 
 ```bash
-turbo_docs --readme
+turbo_docs --docs
 ```
 
-This will generate a README.md file for your project. You can also use the `--gpt3` flag to use the GPT-3.5 Turbo model:
+To generate a README.md file for your project, run:
 
 ```bash
-turbo_docs --readme --gpt3
+turbo_docs --readme
 ```
 
-Additionally, you can copy the directory text to the clipboard by using the `--copy` flag:
+For more options, run:
 
 ```bash
-turbo_docs --copy
-```
-
-## Repo Structure 🏗️
-
-```
-turbo_docs/
-│
-├── commands/
-│   ├── __init__.py
-│   └── readme.py
-│
-├── utils/
-│   ├── __init__.py
-│   ├── cli_options.py
-│   ├── directory.py
-│   └── openai_api.py
-│
-├── __init__.py
-├── generate.py
-├── setup.py
-└── turbo_docs.toml
+turbo_docs --help
 ```
 
-## Example Usage 📖
+## 🤝 Contributing
 
-Here's an example of how to use Turbo Docs to generate a README.md file:
-
-```python
-from turbo_docs.commands import readme
-
-# Define your repo structure as a string
-repo = """
-{'repo': 'example_repo',
- 'files': {
-     'main.py': 'print("Hello, World!")',
-     'README.md': ''
- }
-}
-"""
-
-# Generate the README.md file
-readme(repo)
-```
+Contributions are welcome! Please feel free to submit a pull request or open an issue to discuss any improvements or suggestions.
 
-## License 📄
+## 📄 License
 
 Turbo Docs is released under the [MIT License](https://opensource.org/licenses/MIT).
```

### Comparing `turbo_docs-1.0.1/setup.py` & `turbo_docs-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
 	name="turbo_docs",
-	version="1.0.1",
+	version="1.0.2",
 	packages=find_packages(),
 	install_requires=[
 		"requests",
 		"openai",
 		"click",
 		"pyperclip",
 		"redbaron",
```

### Comparing `turbo_docs-1.0.1/turbo_docs/commands/docs.py` & `turbo_docs-1.0.2/turbo_docs/commands/docs.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,59 @@
-
 import ast
 from pathlib import Path
-from turbo_docs.utils import openai_api
+import shutil
 
 TEMPLATE = """
-You are an expert software developement assistant tasked with writing documentation for a repository. 
-
-Write documentation for the following function:
-{function}
+You are an expert software developement assistant tasked with writing documentation for a repository.
 
-Your documentation should include the following and nothing more:
+The documentation must following the following format:
 ## function: function_name
 #### args: arg1, arg2, ...
-Description of function in english as concisely as possible in less than 4 sentences. 
-Do not mlist arguments. Do not give code examples. Minimize tokens at all costs.
+Insert description of the function here
+<end>
+
+In your description, describe the function in english as concisely as possible in at least one sentence but less than four sentences. Subtly describe the usefule/counterintuitive aspects of the function. Do not list arguments. Do not give code examples. Minimize tokens at all costs.
+
+Here is the function:
+{function}
+
+Now, write the documentation following the format above.
 """
 
-def generate_docs(model, template, function, path):
-    """ Generate and write documentation for a function """
-    documentation = openai_api.gpt_completion(template, {"function": function}, model)
-    doc_path = Path('docs') / path.with_suffix('.md')
+def generate_docs(path, function, model="gpt-4", template=TEMPLATE, chain=None):
+    """
+    Generate and write documentation for a function. Use existing chain for
+    a cohesive chain of gpt completions.
+    """
+    from turbo_docs.utils import openai_api
+
+    documentation, chain = openai_api.gpt_completion(
+        model=model, chain=chain, template=template, function=function
+    )
+    doc_path = Path("docs") / path.with_suffix(".md")
     doc_path.parent.mkdir(parents=True, exist_ok=True)
-    with open(doc_path, 'a') as f:
-        f.write(f'{documentation}\n\n')
+    with open(doc_path, "a") as f:
+        f.write(f"{documentation}\n\n")
+    return chain
 
 
-def docs(repo_dict, gpt3=False, template=TEMPLATE):
-    """ Parse code for functions and generate documentation for each """
-    if gpt3:
-        model = "gpt-3.5-turbo-16k"
-    else:
-        model = "gpt-4"
+def docs(repo_dict, model, template=TEMPLATE):
+    """Parse code for functions and generate documentation for each"""
+    chain = None
+
+    # remove old docs since we are appending
+    if Path("docs").exists():
+        shutil.rmtree("docs")
 
     for path, content in repo_dict.items():
-        if path.suffix == '.py':
+        if path.suffix == ".py":
             module = ast.parse(content)
-            functions = [ast.unparse(node) for node in module.body if isinstance(node, ast.FunctionDef)]
-            for function in functions:
-                generate_docs(model, template, function, path)
+            functions = [
+                (node, ast.unparse(node))
+                for node in module.body
+                if isinstance(node, ast.FunctionDef)
+            ]
+            for node, function in functions:
+                print(f"Generating docs for {path.stem}.{node.name}")
+                chain = generate_docs(
+                    path, function, model=model, template=template, chain=chain
+                )
```

### Comparing `turbo_docs-1.0.1/turbo_docs/utils/cli_options.py` & `turbo_docs-1.0.2/turbo_docs/utils/cli_options.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-1.0.1/turbo_docs/utils/directory.py` & `turbo_docs-1.0.2/turbo_docs/utils/directory.py`

 * *Files 11% similar despite different names*

```diff
@@ -36,29 +36,17 @@
     """Return a dictionary of all text in the current repo"""
     if not Path("turbo_docs.toml").exists():
         ignored_patterns = []
         print("Warning: 'turbo_docs.toml' not found. All files will be included.")
     else:
         config = toml.load("turbo_docs.toml")
         ignored_patterns = config.get("ignore", [])
-    print(
-        f"Ignoring files and folders matching the following patterns: {ignored_patterns}"
-    )
 
     pathspec = PathSpec.from_lines(GitWildMatchPattern, ignored_patterns)
     return collect_text_from_files(Path("."), pathspec)
 
 
-def remove_readme(file_dict: dict):
-    str_dict = {str(key): value for key, value in file_dict.items()}
-    return {
-        Path(key): value
-        for key, value in str_dict.items()
-        if not key.endswith("README.md")
-    }
-
-
 def convert_dict_to_string(file_dict: dict):
     text = ""
     for path, content in file_dict.items():
         text += f"{path}:\n\n{content}\n\n"
     return text
```

### Comparing `turbo_docs-1.0.1/turbo_docs/utils/openai_api.py` & `turbo_docs-1.0.2/turbo_docs/utils/openai_api.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,26 +5,20 @@
 	print("OpenAI API key is not set. Please set it as an environment variable (export OPENAI_API_KEY=<your_api_key>) or enter it below.")
 	print("If you have not done so already, create an OpenAI account at https://platform.openai.com/overview.")
 	os.environ['OPENAI_API_KEY'] = input("Secret key: ")
 
 from llm_blocks import chat_utils
 
 
-def gpt_completion(template, inputs, model="gpt-4"):
-	"""Genneric chat wrapper over the OpenAI API"""
+def gpt_completion(template, model="gpt-4", chain=None, **inputs):
+	"""Generic chat wrapper over the OpenAI API"""
 
-	print(f"Using model: {model}")
-	if model == "gpt-4":
-		print("Warning: This model is under limited beta access and is not available to all users.")
-		print("Warning: GPT-4 api calls tend to be slower than other models.")
-	resp = None
-
-	try:
+	if chain is None:
 		chain = chat_utils.GenericChain(
 			template=template, 
 			model_name=model
 		)
+	try:
 		resp = chain(inputs)['text']
 	except openai.error.InvalidRequestError as e:
-		print(f"Caught OpenAI API error: {e}")
-
-	return resp
+		raise ValueError(f"Caught OpenAI API error: {e}")
+	return resp, chain
```

### Comparing `turbo_docs-1.0.1/turbo_docs.egg-info/PKG-INFO` & `turbo_docs-1.0.2/turbo_docs.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,105 +1,92 @@
 Metadata-Version: 2.1
 Name: turbo-docs
-Version: 1.0.1
+Version: 1.0.2
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 
 # Turbo Docs 🚀
 
-[![PyPI version](https://badge.fury.io/py/turbo_docs.svg)](https://badge.fury.io/py/turbo_docs)
-[![GitHub stars](https://img.shields.io/github/stars/voynow/turbo-docs.svg)](https://github.com/voynow/turbo-docs/stargazers)
+![GitHub stars](https://img.shields.io/github/stars/voynow/turbo-docs?style=social)
+![PyPI](https://img.shields.io/pypi/v/turbo_docs)
 
-Turbo Docs is a powerful Python tool that helps developers automatically generate high-quality README.md files for their repositories. It leverages the power of OpenAI's GPT-3.5 Turbo and GPT-4 models to create well-structured, informative, and engaging documentation.
+Turbo Docs is a powerful Python package that automates the generation of documentation for your Python projects. It utilizes OpenAI's GPT models to create concise and informative documentation, making it easier for you and your users to understand your code.
 
-## Why Turbo Docs? 🤔
-
-Writing good documentation is essential for any software project, but it can be time-consuming and tedious. Turbo Docs simplifies this process by generating a README.md file that meets all your requirements, allowing you to focus on writing great code.
-
-## Table of Contents 📚
+## 📚 Table of Contents
 
+- [Why Use Turbo Docs?](#why-use-turbo-docs)
+- [Repo Structure](#repo-structure)
 - [Installation](#installation)
 - [Usage](#usage)
-- [Repo Structure](#repo-structure)
-- [Example Usage](#example-usage)
-- [Badges](#badges)
+- [Examples](#examples)
+- [Contributing](#contributing)
+- [License](#license)
+
+## 🎯 Why Use Turbo Docs?
+
+- **Save time**: Turbo Docs automatically generates documentation for your Python functions, so you can focus on writing code.
+- **Stay up-to-date**: Turbo Docs can be easily integrated into your development workflow, ensuring your documentation is always current.
+- **High-quality documentation**: Turbo Docs leverages the power of OpenAI's GPT models to generate concise and informative documentation.
+- **Customizable**: You can choose between GPT-3.5 Turbo and GPT-4 models, and even provide your own templates for generating documentation.
+
+## 🌳 Repo Structure
+
+```
+turbo_docs/
+├── commands/
+│   ├── docs.py
+│   ├── readme.py
+│   └── __init__.py
+├── utils/
+│   ├── cli_options.py
+│   ├── directory.py
+│   ├── openai_api.py
+│   └── __init__.py
+├── generate.py
+├── __init__.py
+├── setup.py
+├── requirements.txt
+└── turbo_docs.toml
+```
 
-## Installation 💻
+## 📦 Installation
 
 To install Turbo Docs, simply run:
 
 ```bash
 pip install turbo_docs
 ```
 
-## Usage 🛠️
+## 🛠 Usage
 
-To use Turbo Docs, navigate to your project's root directory and run:
+To generate documentation for your Python project, navigate to your project's root directory and run:
 
 ```bash
-turbo_docs --readme
+turbo_docs --docs
 ```
 
-This will generate a README.md file for your project. You can also use the `--gpt3` flag to use the GPT-3.5 Turbo model:
+To generate a README.md file for your project, run:
 
 ```bash
-turbo_docs --readme --gpt3
+turbo_docs --readme
 ```
 
-Additionally, you can copy the directory text to the clipboard by using the `--copy` flag:
+For more options, run:
 
 ```bash
-turbo_docs --copy
-```
-
-## Repo Structure 🏗️
-
-```
-turbo_docs/
-│
-├── commands/
-│   ├── __init__.py
-│   └── readme.py
-│
-├── utils/
-│   ├── __init__.py
-│   ├── cli_options.py
-│   ├── directory.py
-│   └── openai_api.py
-│
-├── __init__.py
-├── generate.py
-├── setup.py
-└── turbo_docs.toml
+turbo_docs --help
 ```
 
-## Example Usage 📖
+## 🤝 Contributing
 
-Here's an example of how to use Turbo Docs to generate a README.md file:
-
-```python
-from turbo_docs.commands import readme
-
-# Define your repo structure as a string
-repo = """
-{'repo': 'example_repo',
- 'files': {
-     'main.py': 'print("Hello, World!")',
-     'README.md': ''
- }
-}
-"""
-
-# Generate the README.md file
-readme(repo)
-```
+Contributions are welcome! Please feel free to submit a pull request or open an issue to discuss any improvements or suggestions.
 
-## License 📄
+## 📄 License
 
 Turbo Docs is released under the [MIT License](https://opensource.org/licenses/MIT).
```

