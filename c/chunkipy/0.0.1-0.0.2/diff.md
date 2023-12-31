# Comparing `tmp/chunkipy-0.0.1-py3-none-any.whl.zip` & `tmp/chunkipy-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,11 @@
-Zip file size: 7901 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat      105 b- defN 23-Feb-23 23:01 chunkipy/__init__.py
--rw-rw-rw-  2.0 fat     3686 b- defN 23-Feb-24 15:33 chunkipy/text_chunkizer.py
--rw-rw-rw-  2.0 fat      987 b- defN 23-Feb-24 17:52 chunkipy/text_splitter.py
--rw-rw-rw-  2.0 fat     1089 b- defN 23-Feb-24 17:54 chunkipy-0.0.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    13567 b- defN 23-Feb-24 17:54 chunkipy-0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Feb-24 17:54 chunkipy-0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Feb-24 17:54 chunkipy-0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      631 b- defN 23-Feb-24 17:54 chunkipy-0.0.1.dist-info/RECORD
-8 files, 20166 bytes uncompressed, 6801 bytes compressed:  66.3%
+Zip file size: 8440 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat       86 b- defN 23-Jul-03 17:21 chunkipy/__init__.py
+-rw-rw-rw-  2.0 fat     4198 b- defN 23-Jul-03 17:11 chunkipy/text_chunker.py
+-rw-rw-rw-  2.0 fat      897 b- defN 23-Jul-03 17:17 chunkipy/text_splitter.py
+-rw-rw-rw-  2.0 fat      434 b- defN 23-Jul-03 17:09 chunkipy/tokens_estimators.py
+-rw-rw-rw-  2.0 fat     1069 b- defN 23-Jul-03 21:25 chunkipy-0.0.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    13965 b- defN 23-Jul-03 21:25 chunkipy-0.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-03 21:25 chunkipy-0.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Jul-03 21:25 chunkipy-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      713 b- defN 23-Jul-03 21:25 chunkipy-0.0.2.dist-info/RECORD
+9 files, 21463 bytes uncompressed, 7210 bytes compressed:  66.4%
```

## zipnote {}

```diff
@@ -1,25 +1,28 @@
 Filename: chunkipy/__init__.py
 Comment: 
 
-Filename: chunkipy/text_chunkizer.py
+Filename: chunkipy/text_chunker.py
 Comment: 
 
 Filename: chunkipy/text_splitter.py
 Comment: 
 
-Filename: chunkipy-0.0.1.dist-info/LICENSE
+Filename: chunkipy/tokens_estimators.py
 Comment: 
 
-Filename: chunkipy-0.0.1.dist-info/METADATA
+Filename: chunkipy-0.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: chunkipy-0.0.1.dist-info/WHEEL
+Filename: chunkipy-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: chunkipy-0.0.1.dist-info/top_level.txt
+Filename: chunkipy-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: chunkipy-0.0.1.dist-info/RECORD
+Filename: chunkipy-0.0.2.dist-info/top_level.txt
+Comment: 
+
+Filename: chunkipy-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## chunkipy/__init__.py

```diff
@@ -1,2 +1,2 @@
-from chunkipy.text_chunkizer import TextChunkizer
-from chunkipy.text_splitter import default_tokenizer
+from chunkipy.text_chunker import TextChunker
+from chunkipy.tokens_estimators import *
```

## chunkipy/text_splitter.py

```diff
@@ -3,18 +3,14 @@
 import langdetect
 import logging
 
 
 logging.getLogger('stanza').disabled = True
 
 
-def default_tokenizer(text):
-    return [t for t in text.split(" ") if t != '' and ' ']
-
-
 def split_by_sentences(text):
     lang = langdetect.detect(text)
     sentence_tokenizer = stanza.Pipeline(lang=lang, processors='tokenize', download_method=DownloadMethod.REUSE_RESOURCES)
     return [s.text + " " for s in sentence_tokenizer(text).sentences]
 
 
 def split_by_separator(text: str, sep: str):
```

## Comparing `chunkipy-0.0.1.dist-info/LICENSE` & `chunkipy-0.0.2.dist-info/LICENSE`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2018 Gioele Crispo
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2018 Gioele Crispo
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

## Comparing `chunkipy-0.0.1.dist-info/METADATA` & `chunkipy-0.0.2.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,166 +1,175 @@
-Metadata-Version: 2.1
-Name: chunkipy
-Version: 0.0.1
-Summary: Chunkipy is an easy-to-use library for chunking text based on the tokenizer function you provide.
-Home-page: https://github.com/gioelecrispo/chunkipy.git
-Author: Gioele Crispo
-Author-email: crispogioele@gmail.com
-License: MIT
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=2.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: stanza (==1.4.2)
-Requires-Dist: langdetect (==1.0.9)
-
-# Chunkipy
-
-![Python 3.5, 3.6, 3.7, 3.8, 3.9, 3.10, 3.11](https://img.shields.io/badge/python-3.5%2C%203.6%2C%203.7%2C%203.8%2C%203.9%2C%203.10%2C%203.11-blue.svg)
-[![PyPI version](https://badge.fury.io/py/chunkipy.svg)](https://badge.fury.io/py/chunkipy)
-
-
-`chunkipy` is an extremely useful tool for segmenting long texts into smaller chunks, 
- based on either a character or token count. With customizable chunk sizes and splitting strategies, `chunkipy` provides flexibility and control 
- for various text processing tasks.
-
-## Motivation and Features
-`chunkipy` was created to address the need within the field of natural language processing (NLP) 
-to chunk text so that it does not exceed the input size of **neural networks** such as BERT, 
-but it could be used for several other use cases.
-
-The library offers some useful features:
- - **Tokenizer function**: unlike other text chunking libraries, `chunkipy` offers the possibility of
-providing a tokenizer function, in order to build the chunks taking into account the tokenizer 
-that will use those chunks.
- - **Split text into meaningful sentences**: in its default configuration, `chunkipy`, 
-in creating the chunks, avoids cutting sentences, and always tries to have a complete and syntactically correct sentence. 
-This is achieved through the use of the `stanza` library, which utilizes semantic models to cut text 
-into meaningful sentences.
- - **Flexibility in choosing split strategies**: Additionally, `chunkipy` offers complete flexibility 
-in choosing how to split, allowing users to define their own text splitting function or choose from a list 
-of pre-defined splitting strategies.
- 
-By default, `chunkipy` uses `stanza` are main text splitting method; however, if `stanza` produces 
-sentences with a number of tokens greater than the chunk size, other split strategy are used. 
-Here the list of predefined strategies, sorted by priority (the first one is executed first, 
-if the chunk of text is larger than the chunk size, it is further split using a lower priority 
-strategy).
-
-| Priority | Name | Effect                                                              |
-|:--------:| :--- |:--------------------------------------------------------------------|
-|    0     | `split_by_sentences` | It uses `stanza` to split the text into meaningful sentences.       |
-|    1     | `split_by_semicolon` | It splits the text using the semicolon and space `; ` as separator. |
-|    2     | `split_by_colon` | It splits the text using the colon and space `: ` as separator.     |
-|    3     | `split_by_comma` | It splits the text using the comma and space `, ` as separator.     |
-|    4     | `split_by_word` | It splits the text using the space ` ` as separator.                |
-
-
-
-## Installation
-You can install `chunkipy` using pip:
-
-```bash
-pip install chunkipy
-```
-
-## Usage
-The main class in `chunkipy` is `TextChunkizer`, which takes a text and splits it into chunks of a given size. 
-You can use the default settings or specify custom parameters for the **chunk size**, 
-whether to split by **characters or tokens**, the **tokenizer function** to use (if `tokens` is set to True`), and the list of **split strategies** to apply. 
-
-Here's an example of using it to chunk text that has a number of tokens 
-greater than the input size of BERT:
-
-```python
-from chunkipy import TextChunkizer
-from transformers import AutoTokenizer  
-
-text = """Napoleon Bonaparte (born Napoleone Buonaparte; 15 August 1769 â€“ 5 May 1821), later known by his regnal name Napoleon I, was a French military commander and political leader who rose to prominence during the French Revolution and led successful campaigns during the Revolutionary Wars. He was the de facto leader of the French Republic as First Consul from 1799 to 1804, then Emperor of the French from 1804 until 1814 and again in 1815. Napoleon's political and cultural legacy endures to this day, as a highly celebrated and controversial leader. He initiated many liberal reforms that have persisted in society, and is considered one of the greatest military commanders in history. His wars and campaigns are studied by militaries all over the world. Between three and six million civilians and soldiers perished in what became known as the Napoleonic Wars.
-Napoleon was born on the island of Corsica, not long after its annexation by France, to a native family descending from minor Italian nobility. He supported the French Revolution in 1789 while serving in the French army, and tried to spread its ideals to his native Corsica. He rose rapidly in the Army after he saved the governing French Directory by firing on royalist insurgents. In 1796, he began a military campaign against the Austrians and their Italian allies, scoring decisive victories and becoming a national hero. Two years later, he led a military expedition to Egypt that served as a springboard to political power. He engineered a coup in November 1799 and became First Consul of the Republic.
-Differences with the United Kingdom meant France faced the War of the Third Coalition by 1805. Napoleon shattered this coalition with victories in the Ulm campaign, and at the Battle of Austerlitz, which led to the dissolution of the Holy Roman Empire. In 1806, the Fourth Coalition took up arms against him. Napoleon defeated Prussia at the battles of Jena and Auerstedt, marched the Grande ArmÃ©e into Eastern Europe, and defeated the Russians in June 1807 at Friedland, forcing the defeated nations of the Fourth Coalition to accept the Treaties of Tilsit. Two years later, the Austrians challenged the French again during the War of the Fifth Coalition, but Napoleon solidified his grip over Europe after triumphing at the Battle of Wagram.
-Hoping to extend the Continental System, his embargo against Britain, Napoleon invaded the Iberian Peninsula and declared his brother Joseph the King of Spain in 1808. The Spanish and the Portuguese revolted in the Peninsular War aided by a British army, culminating in defeat for Napoleon's marshals. Napoleon launched an invasion of Russia in the summer of 1812. The resulting campaign witnessed the catastrophic retreat of Napoleon's Grande ArmÃ©e. In 1813, Prussia and Austria joined Russian forces in a Sixth Coalition against France, resulting in a large coalition army defeating Napoleon at the Battle of Leipzig. The coalition invaded France and captured Paris, forcing Napoleon to abdicate in April 1814. He was exiled to the island of Elba, between Corsica and Italy. In France, the Bourbons were restored to power."""
-
-bert_tokenizer = AutoTokenizer.from_pretrained("bert-base-uncased")
-
-print(f"Num of chars: {len(text)}") # --> Num of chars: 3149
-print(f"Num of tokens (using BertTokenizer): {len(bert_tokenizer.encode(text))}") # --> Num of tokens (using BertTokenizer): 603
-
-# This creates an instance of the TextChunkizer class with a chunk size of 512, 
-# using token-based segmentation and a custom tokenizer function bert_tokenizer.encode to count tokens.
-chunkizer = TextChunkizer(512, tokens=True, tokenizer_func=bert_tokenizer.encode)
-chunks = chunkizer.chunkize(text)
-for i, chunk in enumerate(chunks):
-    print(f"Chunk {i+1}, num of tokens: {len(bert_tokenizer.encode(chunk))} -> {chunk}")
-```
-This code returns: 
-```
-Chunk 1, num of tokens 476: -> Napoleon Bonaparte (born Napoleone Buonaparte; 15 August 1769 â€“ 5 May 1821), later known by his regnal name Napoleon I, was a French military commander and political leader who rose to prominence during the French Revolution and led successful campaigns during the Revolutionary Wars. He was the de facto leader of the French Republic as First Consul from 1799 to 1804, then Emperor of the French from 1804 until 1814 and again in 1815. Napoleon's political and cultural legacy endures to this day, as a highly celebrated and controversial leader. He initiated many liberal reforms that have persisted in society, and is considered one of the greatest military commanders in history. His wars and campaigns are studied by militaries all over the world. Between three and six million civilians and soldiers perished in what became known as the Napoleonic Wars. Napoleon was born on the island of Corsica, not long after its annexation by France, to a native family descending from minor Italian nobility. He supported the French Revolution in 1789 while serving in the French army, and tried to spread its ideals to his native Corsica. He rose rapidly in the Army after he saved the governing French Directory by firing on royalist insurgents. In 1796, he began a military campaign against the Austrians and their Italian allies, scoring decisive victories and becoming a national hero. Two years later, he led a military expedition to Egypt that served as a springboard to political power. He engineered a coup in November 1799 and became First Consul of the Republic. Differences with the United Kingdom meant France faced the War of the Third Coalition by 1805. Napoleon shattered this coalition with victories in the Ulm campaign, and at the Battle of Austerlitz, which led to the dissolution of the Holy Roman Empire. In 1806, the Fourth Coalition took up arms against him. Napoleon defeated Prussia at the battles of Jena and Auerstedt, marched the Grande ArmÃ©e into Eastern Europe, and defeated the Russians in June 1807 at Friedland, forcing the defeated nations of the Fourth Coalition to accept the Treaties of Tilsit. Two years later, the Austrians challenged the French again during the War of the Fifth Coalition, but Napoleon solidified his grip over Europe after triumphing at the Battle of Wagram. Hoping to extend the Continental System, his embargo against Britain, Napoleon invaded the Iberian Peninsula and declared his brother Joseph the King of Spain in 1808.
-Chunk 2, num of tokens 129: -> The Spanish and the Portuguese revolted in the Peninsular War aided by a British army, culminating in defeat for Napoleon's marshals. Napoleon launched an invasion of Russia in the summer of 1812. The resulting campaign witnessed the catastrophic retreat of Napoleon's Grande ArmÃ©e. In 1813, Prussia and Austria joined Russian forces in a Sixth Coalition against France, resulting in a large coalition army defeating Napoleon at the Battle of Leipzig. The coalition invaded France and captured Paris, forcing Napoleon to abdicate in April 1814. He was exiled to the island of Elba, between Corsica and Italy. In France, the Bourbons were restored to power.
-```
-
-As you can see, `chunkipy` created chunks smaller than the given input size, 
-`512`, counted the tokens using BERT's tokenizer, and didn't cut sentences in half, 
-producing syntactically correct chunks of text.
-
-You can also use `TextChunkizer`'s `segment()` method to split a text into smaller parts 
-without actually creating the chunks. 
-This can be useful, for example, when you want to apply further processing to 
-the text parts before creating the final chunks.
-
-
-### Provide a custom text split strategy
-If you don't want to use `stanza` or you need to use your custom text splitting logic, 
-you can provide it in the constructor, as shown in this example:
-
-```python
-from chunkipy import TextChunkizer
-
-
-def split_by_arrow(text):
-    return [t for t in text.split("->") if t != '' and ' ']
-
-
-text = "This is a tokenized text -> with custom split strategy."
-
-
-# Create a TextChunkizer object with custom split strategy
-chunkizer = TextChunkizer(chunk_size=8, tokens=True,
-                          split_strategies=[split_by_arrow])
-chunks = chunkizer.chunkize(text)
-
-# Print the resulting chunks
-for i, chunk in enumerate(chunks):
-    print(f"Chunk {i+1}: {chunk}")
-```
-
-This would output:
-
-```
-Chunk 1: This is a tokenized text
-Chunk 2: with custom split strategy.
-```
-
-## Contributing
-If you find a bug or have a feature request, please open an issue on [GitHub](https://github.com/gioelecrispo/chunkipy/issues).
-Contributions are welcome! Just fork the repository, create a new branch with your changes, and submit a pull request. Please make sure to write tests for your changes and to follow the [code style](https://www.python.org/dev/peps/pep-0008/).
-
-## License
-TextChunkizer is licensed under the [MIT License](https://opensource.org/licenses/MIT).
-
-
+Metadata-Version: 2.1
+Name: chunkipy
+Version: 0.0.2
+Summary: Chunkipy is an easy-to-use library for chunking text based on the tokenizer function you provide.
+Home-page: https://github.com/gioelecrispo/chunkipy.git
+Author: Gioele Crispo
+Author-email: crispogioele@gmail.com
+License: MIT
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=2.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: stanza (==1.4.2)
+Requires-Dist: langdetect (==1.0.9)
+
+# Chunkipy
+
+![Python 3.5, 3.6, 3.7, 3.8, 3.9, 3.10, 3.11](https://img.shields.io/badge/python-3.5%2C%203.6%2C%203.7%2C%203.8%2C%203.9%2C%203.10%2C%203.11-blue.svg)
+[![PyPI version](https://badge.fury.io/py/chunkipy.svg)](https://badge.fury.io/py/chunkipy)
+
+
+`chunkipy` is an extremely useful tool for segmenting long texts into smaller chunks,
+based on either a character or token count. With customizable chunk sizes and splitting strategies, `chunkipy` provides flexibility and control
+for various text processing tasks.
+
+## Motivation and Features
+`chunkipy` was created to address the need within the field of natural language processing (NLP)
+to chunk text so that it does not exceed the input size of **neural networks** such as BERT,
+but it could be used for several other use cases.
+
+The library offers some useful features:
+- **Tokenizer function**: unlike other text chunking libraries, `chunkipy` offers the possibility of
+  providing a tokenizer function, in order to build the chunks taking into account the tokenizer
+  that will use those chunks.
+- **Split text into meaningful sentences**: in its default configuration, `chunkipy`,
+  in creating the chunks, avoids cutting sentences, and always tries to have a complete and syntactically correct sentence.
+  This is achieved through the use of the `stanza` library, which utilizes semantic models to cut text
+  into meaningful sentences.
+- **Flexibility in choosing split strategies**: Additionally, `chunkipy` offers complete flexibility
+  in choosing how to split, allowing users to define their own text splitting function or choose from a list
+  of pre-defined splitting strategies.
+
+By default, `chunkipy` uses `stanza` are main text splitting method; however, if `stanza` produces
+sentences with a number of tokens greater than the chunk size, other split strategy are used.
+Here the list of predefined strategies, sorted by priority (the first one is executed first,
+if the chunk of text is larger than the chunk size, it is further split using a lower priority
+strategy).
+
+| Priority | Name | Effect                                                               |
+|:--------:| :--- |:---------------------------------------------------------------------|
+|    0     | `split_by_sentences` | It uses `stanza` to split the text into meaningful sentences.        |
+|    1     | `split_by_semicolon` | It splits the text using the semicolon and space `; `  as separator. |
+|    2     | `split_by_colon` | It splits the text using the colon and space `: ` as separator.      |
+|    3     | `split_by_comma` | It splits the text using the comma and space `, ` as separator.      |
+|    4     | `split_by_word` | It splits the text using the space ` ` as separator.                 |
+
+
+
+## Installation
+You can install `chunkipy` using pip:
+
+```bash
+pip install chunkipy
+```
+
+## Usage
+The main class in `chunkipy` is `TextChunker`, which takes a text and splits it into chunks of a given size.
+You can use the default settings or specify custom parameters for the **chunk size**,
+whether to split by **characters or tokens**, the **tokenizer function** to use (if `tokens` is set to True`), and the list of **split strategies** to apply.
+
+Here's an example of using it to chunk text that has a number of tokens
+greater than the input size of BERT:
+
+```python
+from chunkipy import TextChunker, TokenEstimator
+from transformers import AutoTokenizer
+
+text = """Napoleon Bonaparte (born Napoleone Buonaparte; 15 August 1769 â€“ 5 May 1821), later known by his regnal name Napoleon I, was a French military commander and political leader who rose to prominence during the French Revolution and led successful campaigns during the Revolutionary Wars. He was the de facto leader of the French Republic as First Consul from 1799 to 1804, then Emperor of the French from 1804 until 1814 and again in 1815. Napoleon's political and cultural legacy endures to this day, as a highly celebrated and controversial leader. He initiated many liberal reforms that have persisted in society, and is considered one of the greatest military commanders in history. His wars and campaigns are studied by militaries all over the world. Between three and six million civilians and soldiers perished in what became known as the Napoleonic Wars.
+Napoleon was born on the island of Corsica, not long after its annexation by France, to a native family descending from minor Italian nobility. He supported the French Revolution in 1789 while serving in the French army, and tried to spread its ideals to his native Corsica. He rose rapidly in the Army after he saved the governing French Directory by firing on royalist insurgents. In 1796, he began a military campaign against the Austrians and their Italian allies, scoring decisive victories and becoming a national hero. Two years later, he led a military expedition to Egypt that served as a springboard to political power. He engineered a coup in November 1799 and became First Consul of the Republic.
+Differences with the United Kingdom meant France faced the War of the Third Coalition by 1805. Napoleon shattered this coalition with victories in the Ulm campaign, and at the Battle of Austerlitz, which led to the dissolution of the Holy Roman Empire. In 1806, the Fourth Coalition took up arms against him. Napoleon defeated Prussia at the battles of Jena and Auerstedt, marched the Grande ArmÃ©e into Eastern Europe, and defeated the Russians in June 1807 at Friedland, forcing the defeated nations of the Fourth Coalition to accept the Treaties of Tilsit. Two years later, the Austrians challenged the French again during the War of the Fifth Coalition, but Napoleon solidified his grip over Europe after triumphing at the Battle of Wagram.
+Hoping to extend the Continental System, his embargo against Britain, Napoleon invaded the Iberian Peninsula and declared his brother Joseph the King of Spain in 1808. The Spanish and the Portuguese revolted in the Peninsular War aided by a British army, culminating in defeat for Napoleon's marshals. Napoleon launched an invasion of Russia in the summer of 1812. The resulting campaign witnessed the catastrophic retreat of Napoleon's Grande ArmÃ©e. In 1813, Prussia and Austria joined Russian forces in a Sixth Coalition against France, resulting in a large coalition army defeating Napoleon at the Battle of Leipzig. The coalition invaded France and captured Paris, forcing Napoleon to abdicate in April 1814. He was exiled to the island of Elba, between Corsica and Italy. In France, the Bourbons were restored to power."""
+
+class BertTokenEstimator(TokenEstimator):
+    def __init__(self):
+        self.bert_tokenizer = AutoTokenizer.from_pretrained("bert-base-uncased")
+
+    def estimate_tokens(self, text):
+        return len(self.bert_tokenizer.encode(text))
+
+
+bert_token_estimator = BertTokenEstimator()
+
+print(f"Num of chars: {len(text)}")
+# --> Num of chars: 3149
+print(f"Num of tokens (using BertTokenEstimator): {bert_token_estimator.estimate_tokens(text)}")
+# --> Num of tokens (using BertTokenEstimator): 603
+
+# This creates an instance of the TextChunker class with a chunk size of 512, 
+# using token-based segmentation and a custom tokenizer function bert_tokenizer.encode to count tokens.
+
+
+text_chunker = TextChunker(512, tokens=True, token_estimator=BertTokenEstimator())
+chunks = text_chunker.chunk(text)
+for i, chunk in enumerate(chunks):
+    print(f"Chunk {i + 1}, num of tokens: {bert_token_estimator.estimate_tokens(chunk)} -> {chunk}")
+```
+This code returns:
+```
+Chunk 1, num of tokens 476: -> Napoleon Bonaparte (born Napoleone Buonaparte; 15 August 1769 â€“ 5 May 1821), later known by his regnal name Napoleon I, was a French military commander and political leader who rose to prominence during the French Revolution and led successful campaigns during the Revolutionary Wars. He was the de facto leader of the French Republic as First Consul from 1799 to 1804, then Emperor of the French from 1804 until 1814 and again in 1815. Napoleon's political and cultural legacy endures to this day, as a highly celebrated and controversial leader. He initiated many liberal reforms that have persisted in society, and is considered one of the greatest military commanders in history. His wars and campaigns are studied by militaries all over the world. Between three and six million civilians and soldiers perished in what became known as the Napoleonic Wars. Napoleon was born on the island of Corsica, not long after its annexation by France, to a native family descending from minor Italian nobility. He supported the French Revolution in 1789 while serving in the French army, and tried to spread its ideals to his native Corsica. He rose rapidly in the Army after he saved the governing French Directory by firing on royalist insurgents. In 1796, he began a military campaign against the Austrians and their Italian allies, scoring decisive victories and becoming a national hero. Two years later, he led a military expedition to Egypt that served as a springboard to political power. He engineered a coup in November 1799 and became First Consul of the Republic. Differences with the United Kingdom meant France faced the War of the Third Coalition by 1805. Napoleon shattered this coalition with victories in the Ulm campaign, and at the Battle of Austerlitz, which led to the dissolution of the Holy Roman Empire. In 1806, the Fourth Coalition took up arms against him. Napoleon defeated Prussia at the battles of Jena and Auerstedt, marched the Grande ArmÃ©e into Eastern Europe, and defeated the Russians in June 1807 at Friedland, forcing the defeated nations of the Fourth Coalition to accept the Treaties of Tilsit. Two years later, the Austrians challenged the French again during the War of the Fifth Coalition, but Napoleon solidified his grip over Europe after triumphing at the Battle of Wagram. Hoping to extend the Continental System, his embargo against Britain, Napoleon invaded the Iberian Peninsula and declared his brother Joseph the King of Spain in 1808.
+Chunk 2, num of tokens 129: -> The Spanish and the Portuguese revolted in the Peninsular War aided by a British army, culminating in defeat for Napoleon's marshals. Napoleon launched an invasion of Russia in the summer of 1812. The resulting campaign witnessed the catastrophic retreat of Napoleon's Grande ArmÃ©e. In 1813, Prussia and Austria joined Russian forces in a Sixth Coalition against France, resulting in a large coalition army defeating Napoleon at the Battle of Leipzig. The coalition invaded France and captured Paris, forcing Napoleon to abdicate in April 1814. He was exiled to the island of Elba, between Corsica and Italy. In France, the Bourbons were restored to power.
+```
+
+As you can see, `chunkipy` created chunks smaller than the given input size,
+`512`, counted the tokens using BERT's tokenizer, and didn't cut sentences in half,
+producing syntactically correct chunks of text.
+
+You can also use `TextChunker`'s `segment()` method to split a text into smaller parts
+without actually creating the chunks.
+This can be useful, for example, when you want to apply further processing to
+the text parts before creating the final chunks.
+
+
+### Provide a custom text split strategy
+If you don't want to use `stanza` or you need to use your custom text splitting logic,
+you can provide it in the constructor, as shown in this example:
+
+```python
+from chunkipy import TextChunker
+
+
+def split_by_arrow(text):
+    return [t for t in text.split("->") if t != '' and ' ']
+
+
+text = "This is a tokenized text -> with custom split strategy."
+
+
+# Create a TextChunker object with custom split strategy
+text_chunker = TextChunker(chunk_size=8, tokens=True,
+                           split_strategies=[split_by_arrow])
+chunks = text_chunker.chunk(text)
+
+# Print the resulting chunks
+for i, chunk in enumerate(chunks):
+    print(f"Chunk {i+1}: {chunk}")
+```
+
+This would output:
+
+```
+Chunk 1: This is a tokenized text
+Chunk 2: with custom split strategy.
+```
+
+## Contributing
+If you find a bug or have a feature request, please open an issue on [GitHub](https://github.com/gioelecrispo/chunkipy/issues).
+Contributions are welcome! Just fork the repository, create a new branch with your changes, and submit a pull request. Please make sure to write tests for your changes and to follow the [code style](https://www.python.org/dev/peps/pep-0008/).
+
+## License
+TextChunker is licensed under the [MIT License](https://opensource.org/licenses/MIT).
```

