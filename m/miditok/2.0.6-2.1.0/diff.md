# Comparing `tmp/miditok-2.0.6.tar.gz` & `tmp/miditok-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miditok-2.0.6.tar", last modified: Tue May 16 18:41:54 2023, max compression
+gzip compressed data, was "miditok-2.1.0.tar", last modified: Mon Jul  3 14:48:10 2023, max compression
```

## Comparing `miditok-2.0.6.tar` & `miditok-2.1.0.tar`

### file list

```diff
@@ -1,44 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:41:54.109077 miditok-2.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-16 18:41:43.000000 miditok-2.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-05-16 18:41:54.109077 miditok-2.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-05-16 18:41:43.000000 miditok-2.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:41:54.105077 miditok-2.0.6/miditok/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-16 18:41:43.000000 miditok-2.0.6/miditok/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-05-16 18:41:43.000000 miditok-2.0.6/miditok/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)    15179 2023-05-16 18:41:43.000000 miditok-2.0.6/miditok/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:41:54.105077 miditok-2.0.6/miditok/data_augmentation/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-16 18:41:43.000000 miditok-2.0.6/miditok/data_augmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23080 2023-05-16 18:41:43.000000 miditok-2.0.6/miditok/data_augmentation/data_augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)    86231 2023-05-16 18:41:43.000000 miditok-2.0.6/miditok/midi_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:41:54.109077 miditok-2.0.6/miditok/tokenizations/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-16 18:41:43.000000 miditok-2.0.6/miditok/tokenizations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24237 2023-05-16 18:41:43.000000 miditok-2.0.6/miditok/tokenizations/cp_word.py
--rw-r--r--   0 runner    (1001) docker     (123)    19574 2023-05-16 18:41:43.000000 miditok-2.0.6/miditok/tokenizations/midi_like.py
--rw-r--r--   0 runner    (1001) docker     (123)    23891 2023-05-16 18:41:43.000000 miditok-2.0.6/miditok/tokenizations/mmm.py
--rw-r--r--   0 runner    (1001) docker     (123)    25451 2023-05-16 18:41:43.000000 miditok-2.0.6/miditok/tokenizations/mumidi.py
--rw-r--r--   0 runner    (1001) docker     (123)    23212 2023-05-16 18:41:43.000000 miditok-2.0.6/miditok/tokenizations/octuple.py
--rw-r--r--   0 runner    (1001) docker     (123)    14265 2023-05-16 18:41:43.000000 miditok-2.0.6/miditok/tokenizations/octuple_mono.py
--rw-r--r--   0 runner    (1001) docker     (123)    17968 2023-05-16 18:41:43.000000 miditok-2.0.6/miditok/tokenizations/remi.py
--rw-r--r--   0 runner    (1001) docker     (123)    28157 2023-05-16 18:41:43.000000 miditok-2.0.6/miditok/tokenizations/remi_plus.py
--rw-r--r--   0 runner    (1001) docker     (123)    11310 2023-05-16 18:41:43.000000 miditok-2.0.6/miditok/tokenizations/structured.py
--rw-r--r--   0 runner    (1001) docker     (123)    16594 2023-05-16 18:41:43.000000 miditok-2.0.6/miditok/tokenizations/tsd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:41:54.109077 miditok-2.0.6/miditok/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-16 18:41:43.000000 miditok-2.0.6/miditok/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15698 2023-05-16 18:41:43.000000 miditok-2.0.6/miditok/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:41:54.105077 miditok-2.0.6/miditok.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-05-16 18:41:54.000000 miditok-2.0.6/miditok.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-16 18:41:54.000000 miditok-2.0.6/miditok.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 18:41:54.000000 miditok-2.0.6/miditok.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-16 18:41:54.000000 miditok-2.0.6/miditok.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 18:41:54.000000 miditok-2.0.6/miditok.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 18:41:54.109077 miditok-2.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-16 18:41:43.000000 miditok-2.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 18:41:54.109077 miditok-2.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7041 2023-05-16 18:41:43.000000 miditok-2.0.6/tests/test_bpe.py
--rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-05-16 18:41:43.000000 miditok-2.0.6/tests/test_bpe_slow.py
--rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-05-16 18:41:43.000000 miditok-2.0.6/tests/test_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-05-16 18:41:43.000000 miditok-2.0.6/tests/test_multitrack.py
--rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-05-16 18:41:43.000000 miditok-2.0.6/tests/test_one_track.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-16 18:41:43.000000 miditok-2.0.6/tests/test_saving_loading_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-05-16 18:41:43.000000 miditok-2.0.6/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-05-16 18:41:43.000000 miditok-2.0.6/tests/tests_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:48:10.472050 miditok-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-03 14:48:00.000000 miditok-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-07-03 14:48:10.472050 miditok-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-07-03 14:48:00.000000 miditok-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:48:10.468050 miditok-2.1.0/miditok/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-03 14:48:00.000000 miditok-2.1.0/miditok/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16493 2023-07-03 14:48:00.000000 miditok-2.1.0/miditok/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14950 2023-07-03 14:48:00.000000 miditok-2.1.0/miditok/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:48:10.468050 miditok-2.1.0/miditok/data_augmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-03 14:48:00.000000 miditok-2.1.0/miditok/data_augmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23102 2023-07-03 14:48:00.000000 miditok-2.1.0/miditok/data_augmentation/data_augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73357 2023-07-03 14:48:00.000000 miditok-2.1.0/miditok/midi_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:48:10.472050 miditok-2.1.0/miditok/tokenizations/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-03 14:48:00.000000 miditok-2.1.0/miditok/tokenizations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22589 2023-07-03 14:48:00.000000 miditok-2.1.0/miditok/tokenizations/cp_word.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17831 2023-07-03 14:48:00.000000 miditok-2.1.0/miditok/tokenizations/midi_like.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22309 2023-07-03 14:48:00.000000 miditok-2.1.0/miditok/tokenizations/mmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23063 2023-07-03 14:48:00.000000 miditok-2.1.0/miditok/tokenizations/mumidi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20737 2023-07-03 14:48:00.000000 miditok-2.1.0/miditok/tokenizations/octuple.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11982 2023-07-03 14:48:00.000000 miditok-2.1.0/miditok/tokenizations/octuple_mono.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16140 2023-07-03 14:48:00.000000 miditok-2.1.0/miditok/tokenizations/remi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26784 2023-07-03 14:48:00.000000 miditok-2.1.0/miditok/tokenizations/remi_plus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9612 2023-07-03 14:48:00.000000 miditok-2.1.0/miditok/tokenizations/structured.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20990 2023-07-03 14:48:00.000000 miditok-2.1.0/miditok/tokenizations/tsd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:48:10.472050 miditok-2.1.0/miditok/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-03 14:48:00.000000 miditok-2.1.0/miditok/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15771 2023-07-03 14:48:00.000000 miditok-2.1.0/miditok/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:48:10.468050 miditok-2.1.0/miditok.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-07-03 14:48:10.000000 miditok-2.1.0/miditok.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-03 14:48:10.000000 miditok-2.1.0/miditok.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 14:48:10.000000 miditok-2.1.0/miditok.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-03 14:48:10.000000 miditok-2.1.0/miditok.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-03 14:48:10.000000 miditok-2.1.0/miditok.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 14:48:10.472050 miditok-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-07-03 14:48:00.000000 miditok-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:48:10.472050 miditok-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-07-03 14:48:00.000000 miditok-2.1.0/tests/test_bpe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10880 2023-07-03 14:48:00.000000 miditok-2.1.0/tests/test_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8316 2023-07-03 14:48:00.000000 miditok-2.1.0/tests/test_multitrack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-07-03 14:48:00.000000 miditok-2.1.0/tests/test_one_track.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-07-03 14:48:00.000000 miditok-2.1.0/tests/test_saving_loading_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-07-03 14:48:00.000000 miditok-2.1.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-07-03 14:48:00.000000 miditok-2.1.0/tests/tests_utils.py
```

### Comparing `miditok-2.0.6/LICENSE` & `miditok-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `miditok-2.0.6/PKG-INFO` & `miditok-2.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miditok
-Version: 2.0.6
+Version: 2.1.0
 Summary: A convenient MIDI tokenizer for Deep Learning networks, with multiple encoding strategies
 Home-page: https://github.com/Natooz/MidiTok
 Author: Nathan Fradet
 License: MIT
 Keywords: artificial intelligence,deep learning,transformer,midi,tokenization,music,mir
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -45,21 +45,24 @@
 MidiTok uses [MIDIToolkit](https://github.com/YatingMusic/miditoolkit), which itself uses [Mido](https://github.com/mido/mido) to read and write MIDI files, and BPE is backed by [Hugging Face 🤗tokenizers](https://github.com/huggingface/tokenizers) for super-fast encoding.
 
 ## Usage example
 
 The most basic and useful methods are summarized here. And [here](colab-notebooks/Full_Example_HuggingFace_GPT2_Transformer.ipynb) is a simple notebook example showing how to use Hugging Face models to generate music, with MidiTok taking care of tokenizing MIDIs.
 
 ```python
-from miditok import REMI
+from miditok import REMI, TokenizerConfig
 from miditok.utils import get_midi_programs
 from miditoolkit import MidiFile
 from pathlib import Path
 
+# Creating the tokenizer's configuration, read the doc to explore other parameters
+config = TokenizerConfig(nb_velocities=16, use_chords=True)
+
 # Creates the tokenizer and loads a MIDI
-tokenizer = REMI()  # using the default parameters, read the documentation to customize your tokenizer
+tokenizer = REMI(config)
 midi = MidiFile('path/to/your_midi.mid')
 
 # Converts MIDI to tokens, and back to a MIDI
 tokens = tokenizer(midi)  # calling it will automatically detect MIDIs, paths and tokens before the conversion
 converted_back_midi = tokenizer(tokens, get_midi_programs(midi))  # PyTorch / Tensorflow / Numpy tensors supported
 
 # Converts MIDI files to tokens saved as JSON files
@@ -72,15 +75,15 @@
 tokenizer.learn_bpe(
     vocab_size=500,
     tokens_paths=list(Path("path", "to", "tokens_noBPE").glob("**/*.json")),
     start_from_empty_voc=False,
 )
 
 # Saving our tokenizer, to retrieve it back later with the load_params method
-tokenizer.save_params(Path("path", "to", "save", "tokenizer"))
+tokenizer.save_params(Path("path", "to", "save", "tokenizer.json"))
 
 # Converts the tokenized musics into tokens with BPE
 tokenizer.apply_bpe_to_dataset(Path('path', 'to', 'tokens_noBPE'), Path('path', 'to', 'tokens_BPE'))
 ```
 
 ## Tokenizations
 
@@ -104,19 +107,20 @@
 
 ## Contributions
 
 Contributions are gratefully welcomed, feel free to open an issue or send a PR if you want to add a tokenization or speed up the code. You can read the [contribution guide](CONTRIBUTING.md) for details.
 
 ### Todos
 
-* Extend Time Signature to all tokenizations
-* Control Change messages
-* Option to represent pitch values as pitch intervals, as [it seems to improve performances](https://ismir2022program.ismir.net/lbd_369.html).
-* Speeding up MIDI read / load (Rust / C++ binding)
-* Data augmentation on duration values at the MIDI level
+* Option to place `Program` tokens before note tokens for *TSD*, "vanilla" *REMI*, *MIDI-Like* and *Structured*;
+* Extend Time Signature to all tokenizations;
+* Control Change messages;
+* Option to represent pitch values as pitch intervals, as [it seems to improve performances](https://ismir2022program.ismir.net/lbd_369.html);
+* Speeding up MIDI read / load (using a Rust / C++ io library + Python binding ?);
+* Data augmentation on duration values at the MIDI level.
 
 ## Citation
 
 If you use MidiTok for your research, a citation in your manuscript would be gladly appreciated. ❤️
 
 [**MidiTok paper**](https://archives.ismir.net/ismir2021/latebreaking/000005.pdf)
 ```bibtex
```

### Comparing `miditok-2.0.6/README.md` & `miditok-2.1.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -26,21 +26,24 @@
 MidiTok uses [MIDIToolkit](https://github.com/YatingMusic/miditoolkit), which itself uses [Mido](https://github.com/mido/mido) to read and write MIDI files, and BPE is backed by [Hugging Face 🤗tokenizers](https://github.com/huggingface/tokenizers) for super-fast encoding.
 
 ## Usage example
 
 The most basic and useful methods are summarized here. And [here](colab-notebooks/Full_Example_HuggingFace_GPT2_Transformer.ipynb) is a simple notebook example showing how to use Hugging Face models to generate music, with MidiTok taking care of tokenizing MIDIs.
 
 ```python
-from miditok import REMI
+from miditok import REMI, TokenizerConfig
 from miditok.utils import get_midi_programs
 from miditoolkit import MidiFile
 from pathlib import Path
 
+# Creating the tokenizer's configuration, read the doc to explore other parameters
+config = TokenizerConfig(nb_velocities=16, use_chords=True)
+
 # Creates the tokenizer and loads a MIDI
-tokenizer = REMI()  # using the default parameters, read the documentation to customize your tokenizer
+tokenizer = REMI(config)
 midi = MidiFile('path/to/your_midi.mid')
 
 # Converts MIDI to tokens, and back to a MIDI
 tokens = tokenizer(midi)  # calling it will automatically detect MIDIs, paths and tokens before the conversion
 converted_back_midi = tokenizer(tokens, get_midi_programs(midi))  # PyTorch / Tensorflow / Numpy tensors supported
 
 # Converts MIDI files to tokens saved as JSON files
@@ -53,15 +56,15 @@
 tokenizer.learn_bpe(
     vocab_size=500,
     tokens_paths=list(Path("path", "to", "tokens_noBPE").glob("**/*.json")),
     start_from_empty_voc=False,
 )
 
 # Saving our tokenizer, to retrieve it back later with the load_params method
-tokenizer.save_params(Path("path", "to", "save", "tokenizer"))
+tokenizer.save_params(Path("path", "to", "save", "tokenizer.json"))
 
 # Converts the tokenized musics into tokens with BPE
 tokenizer.apply_bpe_to_dataset(Path('path', 'to', 'tokens_noBPE'), Path('path', 'to', 'tokens_BPE'))
 ```
 
 ## Tokenizations
 
@@ -85,19 +88,20 @@
 
 ## Contributions
 
 Contributions are gratefully welcomed, feel free to open an issue or send a PR if you want to add a tokenization or speed up the code. You can read the [contribution guide](CONTRIBUTING.md) for details.
 
 ### Todos
 
-* Extend Time Signature to all tokenizations
-* Control Change messages
-* Option to represent pitch values as pitch intervals, as [it seems to improve performances](https://ismir2022program.ismir.net/lbd_369.html).
-* Speeding up MIDI read / load (Rust / C++ binding)
-* Data augmentation on duration values at the MIDI level
+* Option to place `Program` tokens before note tokens for *TSD*, "vanilla" *REMI*, *MIDI-Like* and *Structured*;
+* Extend Time Signature to all tokenizations;
+* Control Change messages;
+* Option to represent pitch values as pitch intervals, as [it seems to improve performances](https://ismir2022program.ismir.net/lbd_369.html);
+* Speeding up MIDI read / load (using a Rust / C++ io library + Python binding ?);
+* Data augmentation on duration values at the MIDI level.
 
 ## Citation
 
 If you use MidiTok for your research, a citation in your manuscript would be gladly appreciated. ❤️
 
 [**MidiTok paper**](https://archives.ismir.net/ismir2021/latebreaking/000005.pdf)
 ```bibtex
```

### Comparing `miditok-2.0.6/miditok/constants.py` & `miditok-2.1.0/miditok/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,43 @@
 """Constants for data encoding
 
 """
 
-CURRENT_VERSION_PACKAGE = "2.0.6"  # used when saving the config of a tokenizer
+CURRENT_VERSION_PACKAGE = "2.1.0"  # used when saving the config of a tokenizer
 
 MIDI_FILES_EXTENSIONS = [".mid", ".midi", ".MID", ".MIDI"]
 
 # Starting id of chr() method for BPE, as the 5 (0 to 4 included) firsts are ignored by 🤗tokenize
 # We also skip the 32nd (0x20) (space) as it causes issues when loading a BPE model with spaces in merged
 # Issue for reference: https://github.com/huggingface/tokenizers/issues/566
 # List of unicode characters: https://www.fileformat.info/info/charset/UTF-8/list.htm
 CHR_ID_START = 33
 
+# MIDI encodings default parameters, used when tokenizing a dataset and using tokens
+# These are the parameters from which a MIDI file will be tokenized
+# the recommended pitches for piano in the GM2 specs are from 21 to 108
+PITCH_RANGE = (21, 109)
+BEAT_RES = {(0, 4): 8, (4, 12): 4}  # samples per beat
+# nb of velocity bins, velocities values from 0 to 127 will be quantized
+NB_VELOCITIES = 32
+# default special tokens
+SPECIAL_TOKENS = ["PAD", "BOS", "EOS", "MASK"]
+
+USE_CHORDS = False
+USE_RESTS = False
+USE_TEMPOS = False
+USE_TIME_SIGNATURE = False
+USE_PROGRAMS = False
+
+# rest params, (/min_rest, max_rest_in_BEAT)
+REST_RANGE = (2, 8)
+
+# Chord params
+# "chord_unknown" specifies the range of number of notes that can form "unknown" chords (that do not fit
+# in "chord_maps") to add in tokens
 # Known chord maps, with 0 as root note
 CHORD_MAPS = {
     "min": (0, 3, 7),
     "maj": (0, 4, 7),
     "dim": (0, 3, 6),
     "aug": (0, 4, 8),
     "sus2": (0, 2, 7),
@@ -25,56 +47,36 @@
     "7maj": (0, 4, 7, 11),
     "7halfdim": (0, 3, 6, 10),
     "7dim": (0, 3, 6, 9),
     "7aug": (0, 4, 8, 11),
     "9maj": (0, 4, 7, 10, 14),
     "9min": (0, 4, 7, 10, 13),
 }
-UNKNOWN_CHORD_PREFIX = "ukn"
+# Tokens will look as "Chord_C:maj"
+CHORD_TOKENS_WITH_ROOT_NOTE = False
+# (3, 6) for chords between 3 and 5 notes
+CHORD_UNKNOWN = None
+UNKNOWN_CHORD_PREFIX = "ukn"  # only used in methods
+
+# Tempo params
+# nb of tempo bins for additional tempo tokens, quantized like velocities
+NB_TEMPOS = 32
+TEMPO_RANGE = (40, 250)  # (min_tempo, max_tempo)
+
+# Time signature params
+TIME_SIGNATURE_RANGE = (8, 2)
+
+# Programs
+PROGRAMS = list(range(-1, 128))
 
-# MIDI encodings default parameters, used when tokenizing a dataset and using tokens
-# These are the parameters from which a MIDI file will be tokenized
-PITCH_RANGE = range(
-    21, 109
-)  # the recommended pitches for piano in the GM2 specs are from 21 to 108
-BEAT_RES = {(0, 4): 8, (4, 12): 4}  # samples per beat
-NB_VELOCITIES = (
-    32  # nb of velocity bins, velocities values from 0 to 127 will be quantized
-)
-ADDITIONAL_TOKENS = {
-    "Chord": False,
-    "Rest": False,
-    "Tempo": False,
-    "TimeSignature": False,
-    "Program": False,
-    # rest params
-    "rest_range": (
-        2,
-        8,
-    ),  # (/min_rest, max_rest_in_BEAT), first divides a whole note/rest
-    # Chord params
-    # "chord_unknown" specifies the range of number of notes that can form "unknown" chords (that do not fit
-    # in "chord_maps") to add in tokens
-    "chord_maps": CHORD_MAPS,
-    "chord_tokens_with_root_note": True,  # Tokens will look as "Chord_C:maj"
-    "chord_unknown": False,  # (3, 6) for chords between 3 and 5 notes
-    # Tempo params
-    "nb_tempos": 32,  # nb of tempo bins for additional tempo tokens, quantized like velocities
-    "tempo_range": (40, 250),  # (min_tempo, max_tempo)
-    # Time signature params
-    "time_signature_range": (8, 2),
-    # Programs
-    "programs": list(range(-1, 128)),
-}  # (max_beat_res, max_bar_length_in_NOTE)
-SPECIAL_TOKENS = ["PAD", "BOS", "EOS", "MASK"]  # default special tokens
 
 # Tokenizers specific parameters
 # For MuMIDI, recommended range from the GM2 specs
 # note: we ignore the "Applause" at pitch 88 of the orchestra drum set, increase to 89 if you need it
-DRUM_PITCH_RANGE = range(27, 88)
+DRUM_PITCH_RANGE = (27, 88)
 MMM_DENSITY_BINS_MAX = (10, 20)
 
 # Defaults values when writing new MIDI files
 TIME_DIVISION = 384  # 384 and 480 are convenient as divisible by 4, 8, 12, 16, 24, 32
 TEMPO = 120
 TIME_SIGNATURE = (4, 4)
```

### Comparing `miditok-2.0.6/miditok/data_augmentation/data_augmentation.py` & `miditok-2.1.0/miditok/data_augmentation/data_augmentation.py`

 * *Files 1% similar despite different names*

```diff
@@ -266,18 +266,19 @@
                 max_pitch = tokenizer[
                     pitch_voc_idx, int(np.max(np.concatenate(ids_pitch)))
                 ].split("_")[1]
                 min_pitch = tokenizer[
                     pitch_voc_idx, int(np.min(np.concatenate(ids_pitch)))
                 ].split("_")[1]
         offset_up = min(
-            nb_octave_offset, (tokenizer.pitch_range.stop - 1 - int(max_pitch)) // 12
+            nb_octave_offset,
+            (tokenizer.config.pitch_range[1] - 1 - int(max_pitch)) // 12,
         )
         offset_down = min(
-            nb_octave_offset, (int(min_pitch) - tokenizer.pitch_range.start) // 12
+            nb_octave_offset, (int(min_pitch) - tokenizer.config.pitch_range[0]) // 12
         )
 
         off = []
         if octave_directions[0]:
             off += list(range(12, offset_up * 12 + 1, 12))
         if octave_directions[1]:
             off += list(range(-offset_down * 12, 0, 12))
```

### Comparing `miditok-2.0.6/miditok/midi_tokenizer.py` & `miditok-2.1.0/miditok/midi_tokenizer.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,34 @@
 """
 MIDI encoding base class and methods
 """
 from abc import ABC, abstractmethod
 import math
 from pathlib import Path
 import json
-from random import choices
 from copy import deepcopy
-from typing import List, Tuple, Dict, Union, Callable, Iterable, Optional, Any
+from typing import List, Tuple, Dict, Union, Callable, Iterable, Optional, Any, Sequence
 
 import numpy as np
 from tqdm import tqdm
 from miditoolkit import MidiFile, Instrument, Note, TempoChange, TimeSignature
 from tokenizers import Tokenizer as TokenizerFast
 from tokenizers.models import BPE
 from tokenizers.trainers import BpeTrainer
 
-from .classes import Event, TokSequence
+from .classes import Event, TokSequence, TokenizerConfig
 from .utils import (
     remove_duplicated_notes,
     get_midi_programs,
     convert_ids_tensors_to_list,
 )
 from .data_augmentation import data_augmentation_dataset
 from .constants import (
     TIME_DIVISION,
     CURRENT_VERSION_PACKAGE,
-    PITCH_RANGE,
-    BEAT_RES,
-    NB_VELOCITIES,
-    ADDITIONAL_TOKENS,
-    SPECIAL_TOKENS,
     CHR_ID_START,
     PITCH_CLASSES,
     UNKNOWN_CHORD_PREFIX,
     MIDI_FILES_EXTENSIONS,
 )
 
 
@@ -46,198 +40,179 @@
     :param decode_bpe: will decode BPE, if applicable. This step is performed before completing the sequence.
     """
 
     def decorator(function: Callable = None):
         def wrapper(*args, **kwargs):
             self = args[0]
             seq = args[1]
-            if not isinstance(seq, TokSequence):
-                ids = tokens = events = None
+            if not isinstance(seq, TokSequence) and not all(
+                isinstance(seq_, TokSequence) for seq_ in seq
+            ):
                 try:
-                    ids = convert_ids_tensors_to_list(seq)
+                    arg = ("ids", convert_ids_tensors_to_list(seq))
                 except (AttributeError, ValueError, TypeError, IndexError):
                     if isinstance(seq[0], str) or (
                         isinstance(seq[0], str) and isinstance(seq[0][0], str)
                     ):
-                        tokens = seq
+                        arg = ("tokens", seq)
                     else:  # list of Event, very unlikely
-                        events = seq
+                        arg = ("events", seq)
 
-                seq = TokSequence(
-                    ids=ids,
-                    tokens=tokens,
-                    events=events,
-                    ids_bpe_encoded=self._ids_are_bpe_encoded(ids),
-                )
+                if isinstance(arg[1][0], list):
+                    seq = []
+                    for obj in arg[1]:
+                        kwarg = {arg[0]: obj}
+                        seq.append(TokSequence(**kwarg))
+                        seq[-1].ids_bpe_encoded = self._are_ids_bpe_encoded(seq[-1].ids)
+                else:
+                    kwarg = {arg[0]: arg[1]}
+                    seq = TokSequence(**kwarg)
+                    seq.ids_bpe_encoded = self._are_ids_bpe_encoded(seq.ids)
 
             if self.has_bpe and decode_bpe:
                 self.decode_bpe(seq)
             if complete:
-                self.complete_sequence(seq)
+                if isinstance(seq, TokSequence):
+                    self.complete_sequence(seq)
+                else:
+                    for seq_ in seq:
+                        self.complete_sequence(seq_)
 
             args = list(args)
             args[1] = seq
             return function(*args, **kwargs)
 
         return wrapper
 
     return decorator
 
 
 def _out_as_complete_seq(function: Callable):
-    """Decorator completing a output Sequence object."""
+    """Decorator completing an output Sequence object."""
 
     def wrapper(*args, **kwargs):
         self = args[0]
         res = function(*args, **kwargs)
         self.complete_sequence(res)
         return res
 
     return wrapper
 
 
 class MIDITokenizer(ABC):
     r"""MIDI tokenizer base class, containing common methods and attributes for all tokenizers.
 
-    :param pitch_range: (default: range(21, 109)) range of MIDI pitches to use. Pitches can take
-            values between 0 and 127 (included).
-            The `General MIDI 2 (GM2) specifications <https://www.midi.org/specifications-old/item/general-midi-2>`_
-            indicate the **recommended** ranges of pitches per MIDI program (instrument).
-            These recommended ranges can also be found in ``miditok.constants`` .
-            In all cases, the range from 21 to 108 (included) covers all the recommended values.
-            When processing a MIDI, the notes with pitches under or above this range can be discarded.
-    :param beat_res: (default: `{(0, 4): 8, (4, 12): 4}`) beat resolutions, as a dictionary in the form:
-            ``{(beat_x1, beat_x2): beat_res_1, (beat_x2, beat_x3): beat_res_2, ...}``
-            The keys are tuples indicating a range of beats, ex 0 to 3 for the first bar, and
-            the values are the resolution (in samples per beat) to apply to the ranges, ex 8.
-            This allows to use **Duration** / **TimeShift** tokens of different lengths / resolutions.
-            Note: for tokenization with **Position** tokens, the total number of possible positions will
-            be set at four times the maximum resolution given (``max(beat_res.values)``\).
-    :param nb_velocities: (default: 32) number of velocity bins. In the MIDI norm, velocities can take
-            up to 128 values (0 to 127). This parameter allows to reduce the number of velocity values.
-            The velocities of the MIDIs resolution will be downsampled to ``nb_velocities`` values, equally
-            separated between 0 and 127.
-    :param additional_tokens: (default: None used) specify which additional tokens to use.
-            Compatibilities between tokenization and additional tokens may vary.
-            See :ref:`Additional tokens` for the details and available tokens.
-    :param special_tokens: list of special tokens. This must be given as a list of strings given
-            only the names of the tokens. (default: ``["PAD", "BOS", "EOS", "MASK"]``\)
+    :param tokenizer_config: the tokenizer's configuration, as a :class:`miditok.classes.TokenizerConfig` object.
     :param unique_track: set to True if the tokenizer works only with a unique track.
             Tokens will be saved as a single track. This applies to representations that natively handle
             multiple tracks such as Octuple, resulting in a single "stream" of tokens for all tracks.
             This attribute will be saved in config files of the tokenizer. (default: False)
     :param params: path to a tokenizer config file. This will override other arguments and
             load the tokenizer based on the config file. This is particularly useful if the
             tokenizer learned Byte Pair Encoding. (default: None)
     """
 
     def __init__(
         self,
-        pitch_range: range = PITCH_RANGE,
-        beat_res: Dict[Tuple[int, int], int] = BEAT_RES,
-        nb_velocities: int = NB_VELOCITIES,
-        additional_tokens: Dict[
-            str, Union[bool, int, Dict[str, Tuple], Tuple[int, int]]
-        ] = ADDITIONAL_TOKENS,
-        special_tokens: List[str] = SPECIAL_TOKENS,
+        tokenizer_config: TokenizerConfig = None,
         unique_track: bool = False,
         params: Union[str, Path] = None,
     ):
         # Initialize params
-        self._vocab_base = (
-            {}
-        )  # vocab of prime tokens, can be viewed as unique char / bytes
-        self.__vocab_base_inv = {}  # the other way, to decode id (int) -> token (str)
-        self._vocab_base_id_to_byte = (
-            {}
-        )  # id (int) -> byte (str), as this might not be chr(id) after BPE training
-        self._vocab_base_byte_to_token = (
-            {}
-        )  # byte (str) -> token (str), for basic tokens
-        self._vocab_bpe_bytes_to_tokens = (
-            {}
-        )  # byte(s) -> token(s), for faster BPE decoding
+        self.config = deepcopy(tokenizer_config)
+        # vocab of prime tokens, can be viewed as unique char / bytes
+        self._vocab_base = {}
+        # the other way, to decode id (int) -> token (str)
+        self.__vocab_base_inv = {}
+        # id (int) -> byte (str), as this might not be chr(id) after BPE training
+        self._vocab_base_id_to_byte = {}
+        # byte (str) -> token (str), for basic tokens
+        self._vocab_base_byte_to_token = {}
+        # byte(s) -> token(s), for faster BPE decoding
+        self._vocab_bpe_bytes_to_tokens = {}
         self.has_bpe = False
-
         # Fast BPE tokenizer backed with 🤗tokenizers
         self._bpe_model = None
 
         # Loading params, or initializing them from args
         if params is not None:
-            self.load_params(params)
+            # Will overwrite self.config
+            self._load_params(params)
         else:
+            # If no TokenizerConfig is given, we falls back to the default parameters
+            if self.config is None:
+                self.config = TokenizerConfig()
             assert (
-                pitch_range.start >= 0 and pitch_range.stop <= 128
+                self.config.pitch_range[0] >= 0 and self.config.pitch_range[1] <= 128
             ), "You must specify a pitch_range between 0 and 127 (included, i.e. range.stop at 128)"
             assert (
-                0 < nb_velocities < 128
+                0 < self.config.nb_velocities < 128
             ), "You must specify a nb_velocities between 1 and 127 (included)"
-            self.pitch_range = pitch_range
-            self.beat_res = beat_res
-            self._nb_velocities = nb_velocities
-            self.additional_tokens = additional_tokens
-            self.special_tokens = special_tokens if special_tokens is not None else []
             self.unique_track = unique_track
 
+        # Tweak the tokenizer's configuration and / or attributes before creating the vocabulary
+        # This method is intended to be overridden by inheriting tokenizer classes
+        self._tweak_config_before_creating_voc()
+
         # Init duration and velocity values
         self.durations = self.__create_durations_tuples()
-        self.velocities = np.linspace(0, 127, self._nb_velocities + 1, dtype=np.intc)[
-            1:
-        ]  # remove velocity 0
-        self._first_beat_res = list(self.beat_res.values())[0]
-        for beat_range, res in self.beat_res.items():
+        # [1:] so that there is no velocity_0
+        self.velocities = np.linspace(
+            0, 127, self.config.nb_velocities + 1, dtype=np.intc
+        )[1:]
+        self._first_beat_res = list(self.config.beat_res.values())[0]
+        for beat_range, res in self.config.beat_res.items():
             if 0 in beat_range:
                 self._first_beat_res = res
                 break
 
         # Tempos
         self.tempos = np.zeros(1)
-        if self.additional_tokens["Tempo"]:
+        if self.config.use_tempos:
             self.tempos = np.linspace(
-                *self.additional_tokens["tempo_range"],
-                self.additional_tokens["nb_tempos"],
+                *self.config.tempo_range,
+                self.config.nb_tempos,
                 dtype=np.intc,
             )
 
         # Rests
         self.rests = []
-        if self.additional_tokens["Rest"]:
+        if self.config.use_rests:
             assert (
-                self.additional_tokens["rest_range"][0] // 4 <= self._first_beat_res
+                self.config.rest_range[0] // 4 <= self._first_beat_res
             ), "The minimum rest value must be equal or superior to the initial beat resolution"
             self.rests = self.__create_rests()
 
         # Time Signatures
         self.time_signatures = []
-        if self.additional_tokens["TimeSignature"]:
+        if self.config.use_time_signatures:
             self.time_signatures = self.__create_time_signatures()
 
         # Vocabulary and token types graph
         if (
             len(self.vocab) == 0
         ):  # in case it was not already loaded by load_params, such as with BPE
             self.__create_vocabulary()
         self.tokens_types_graph = self._create_token_types_graph()
         self._add_special_tokens_to_types_graph()
         self._token_types_indexes = {}
         self._update_token_types_indexes()
 
-        # Slow BPE attributes
-        self.__bpe_successions = {}
-        if self.bpe_slow:  # loaded from config file
-            self.__set_bpe_slow_tokens_successions()
-
         # Keep in memory durations in ticks for seen time divisions so these values
         # are not calculated each time a MIDI is processed
         self._durations_ticks = {}
 
         # Holds the tempo changes, time signature, time division and key signature of a
         # MIDI (being parsed) so that methods processing tracks can access them
         self._current_midi_metadata = {}  # needs to be updated each time a MIDI is read
 
+    def _tweak_config_before_creating_voc(self):
+        # called after setting the tokenizer's TokenizerConfig (.config). To be customized by tokenizer classes.
+        pass
+
     @property
     def vocab(
         self,
     ) -> Union[Dict[str, int], List[Dict[str, int]]]:  # token (str) to its id (int)
         """Get the base vocabulary, as a dictionary linking tokens (str) to their ids (int).
         The different (hidden / protected) vocabulary attributes of the class are:
 
@@ -256,28 +231,43 @@
         ``._vocab_base_byte_to_token`` .
 
         :return: the base vocabulary.
         """
         return self._vocab_base
 
     @property
-    def vocab_bpe(self) -> [str, int]:  # byte (str) to its id (int)
+    def vocab_bpe(self) -> Union[None, Dict[str, int]]:  # byte (str) to its id (int)
         r"""Returns the vocabulary learnt with BPE.
         In case the tokenizer has not been trained with BPE, it returns None.
-        In case it was trained with the *slow* BPE method, it returns the base vocabulary.
 
         :return: the BPE model's vocabulary.
         """
         if not self.has_bpe:
             return None
-        elif self.bpe_slow:
-            return self._vocab_base
         else:
             return self._bpe_model.get_vocab()
 
+    @property
+    def special_tokens(self) -> Sequence[str]:
+        r"""Returns the vocabulary learnt with BPE.
+        In case the tokenizer has not been trained with BPE, it returns None.
+
+        :return: special tokens of the tokenizer
+        """
+        return self.config.special_tokens
+
+    @property
+    def special_tokens_ids(self) -> Sequence[int]:
+        r"""Returns the vocabulary learnt with BPE.
+        In case the tokenizer has not been trained with BPE, it returns None.
+
+        :return: special tokens of the tokenizer
+        """
+        return [self[token] for token in self.special_tokens]
+
     def preprocess_midi(self, midi: MidiFile):
         r"""Pre-process (in place) a MIDI file to quantize its time and note attributes
         before tokenizing it. Its notes attribute (times, pitches, velocities) will be
         quantized and sorted, duplicated notes removed, as well as tempos. Empty tracks
         (with no note) will be removed from the MIDI object. Notes with pitches outside
         of self.pitch_range will be deleted.
 
@@ -295,45 +285,46 @@
                 midi.instruments[t].notes
             )  # remove possible duplicated notes
             if len(midi.instruments[t].notes) == 0:
                 del midi.instruments[t]
                 continue
             t += 1
 
-        # Recalculate max_tick is this could have change after notes quantization
+        # Recalculate max_tick is this could have changed after notes quantization
         if len(midi.instruments) > 0:
             midi.max_tick = max(
                 [max([note.end for note in track.notes]) for track in midi.instruments]
             )
 
-        if self.additional_tokens["Tempo"]:
+        if self.config.use_tempos:
             self._quantize_tempos(midi.tempo_changes, midi.ticks_per_beat)
 
         if len(midi.time_signature_changes) == 0:  # can sometimes happen
             midi.time_signature_changes.append(
                 TimeSignature(4, 4, 0)
             )  # 4/4 by default in this case
-        if self.additional_tokens["TimeSignature"]:
+        if self.config.use_time_signatures:
             self._quantize_time_signatures(
                 midi.time_signature_changes, midi.ticks_per_beat
             )
 
     def _quantize_notes(self, notes: List[Note], time_division: int):
         r"""Quantize the notes attributes: their pitch, velocity, start and end values.
         It shifts the notes so that they start at times that match the time resolution
         (e.g. 16 samples per bar).
         Notes with pitches outside of self.pitch_range will be deleted.
 
         :param notes: notes to quantize.
         :param time_division: MIDI time division / resolution, in ticks/beat (of the MIDI being parsed).
         """
-        ticks_per_sample = int(time_division / max(self.beat_res.values()))
+        ticks_per_sample = int(time_division / max(self.config.beat_res.values()))
         i = 0
+        pitches = range(*self.config.pitch_range)
         while i < len(notes):
-            if notes[i].pitch not in self.pitch_range:
+            if notes[i].pitch not in pitches:
                 del notes[i]
                 continue
             start_offset = notes[i].start % ticks_per_sample
             end_offset = notes[i].end % ticks_per_sample
             notes[i].start += (
                 -start_offset
                 if start_offset <= ticks_per_sample / 2
@@ -364,15 +355,15 @@
     def _quantize_tempos(self, tempos: List[TempoChange], time_division: int):
         r"""Quantize the times and tempo values of tempo change events.
         Consecutive identical tempo changes will be removed.
 
         :param tempos: tempo changes to quantize.
         :param time_division: MIDI time division / resolution, in ticks/beat (of the MIDI being parsed).
         """
-        ticks_per_sample = int(time_division / max(self.beat_res.values()))
+        ticks_per_sample = int(time_division / max(self.config.beat_res.values()))
         prev_tempo = -1
         i = 0
         while i < len(tempos):
             # Quantize tempo value
             tempos[i].tempo = self.tempos[
                 np.argmin(np.abs(self.tempos - tempos[i].tempo))
             ]
@@ -427,35 +418,36 @@
 
     def _midi_to_tokens(self, midi: MidiFile, *args, **kwargs) -> List[TokSequence]:
         r"""Converts a preprocessed MIDI object to a sequence of tokens.
         Tokenization treating all tracks as a single token sequence might
         override this method, e.g. Octuple or PopMAG.
 
         :param midi: the MIDI object to convert.
-        :return: sequences of tokens.
+        :return: a list of :class:`miditok.TokSequence` objects.
         """
         # Convert each track to tokens
         tokens = []
         for track in midi.instruments:
             tokens.append(self.track_to_tokens(track))
             self.complete_sequence(tokens[-1])
         return tokens
 
     def midi_to_tokens(
         self, midi: MidiFile, apply_bpe_if_possible: bool = True, *args, **kwargs
-    ) -> List[TokSequence]:
+    ) -> Union[TokSequence, List[TokSequence]]:
         r"""Tokenizes a MIDI file.
         This method returns a list of :class:`miditok.TokSequence`.
 
         If you are implementing your own tokenization by subclassing this class, **override the
         ``_midi_to_tokens`` method**. This method implement necessary MIDI preprocessing.
 
         :param midi: the MIDI object to convert.
         :param apply_bpe_if_possible: will apply BPE if the tokenizer's vocabulary was learned with.
-        :return: sequences of tokens.
+        :return: a :class:`miditok.TokSequence` if `tokenizer.unique_track` is true, else a list of
+                :class:`miditok.TokSequence` objects.
         """
         # Check if the durations values have been calculated before for this time division
         if midi.ticks_per_beat not in self._durations_ticks:
             self._durations_ticks[midi.ticks_per_beat] = np.array(
                 [
                     (beat * res + pos) * midi.ticks_per_beat // res
                     for beat, pos, res in self.durations
@@ -507,27 +499,27 @@
             elif seq.ids is not None:
                 seq.tokens = self._ids_to_tokens(seq.ids)
             elif seq.bytes is not None:
                 seq.tokens = self._bytes_to_tokens(seq.bytes)
         if seq.ids is None:
             seq.ids = self._tokens_to_ids(seq.tokens)
 
-        if self.has_bpe and not self.bpe_slow:
+        if self.has_bpe:
             if seq.bytes is None:
                 seq.bytes = self._ids_to_bytes(seq.ids, as_one_str=True)
 
     def _tokens_to_ids(
-        self, tokens: List[Union[str, List[str]]]
+        self, tokens: Sequence[Union[str, List[str]]]
     ) -> List[Union[int, List[int]]]:
         r"""Converts a list of tokens (str) into their associated ids (int).
 
         :param tokens: list of tokens (str) to convert.
         :return: list of corresponding ids (int).
         """
-        if isinstance(tokens[0], list):
+        if isinstance(tokens[0], (list, tuple)):
             ids = []
             for seq in tokens:
                 ids.append([self[i, token] for i, token in enumerate(seq)])
         else:
             ids = [self[token] for token in tokens]
         return ids
 
@@ -654,15 +646,15 @@
         r"""Converts a sequence of tokens into a track object.
         This method is unimplemented and need to be overridden by inheriting classes.
         This method should be decorated with _in_as_complete_seq to receive any type of input.
 
         :param tokens: tokens to convert. Can be either a :class:`miditok.TokSequence`,
                 a Tensor (PyTorch and Tensorflow are supported), a numpy array or a Python list of ints.
         :param time_division: MIDI time division / resolution, in ticks/beat (of the MIDI to create).
-        :param program: the MIDI program of the produced track and if it drum. (default (0, False), piano)
+        :param program: the MIDI program of the produced track and if it is drums. (default (0, False), piano)
         :return: the miditoolkit instrument object and the possible tempo changes.
         """
         raise NotImplementedError
 
     @abstractmethod
     def _create_base_vocabulary(self, *args, **kwargs) -> List[Union[str, List[str]]]:
         r"""Creates the vocabulary, as a list of string tokens.
@@ -753,19 +745,15 @@
 
         if vocab_idx is not None:
             self._vocab_base[vocab_idx][token_str] = len(self._vocab_base[vocab_idx])
             self.__vocab_base_inv[vocab_idx][
                 len(self.__vocab_base_inv[vocab_idx])
             ] = token_str
         else:
-            id_ = (
-                len(self._bpe_model.get_vocab())
-                if self.has_bpe and not self.bpe_slow
-                else len(self.vocab)
-            )
+            id_ = len(self._bpe_model.get_vocab()) if self.has_bpe else len(self.vocab)
             self._vocab_base[token_str] = id_
             self.__vocab_base_inv[len(self.__vocab_base_inv)] = token_str
 
             # For BPE
             if byte_ is None:
                 byte_ = chr(id_ + CHR_ID_START)
             self._vocab_base_id_to_byte[
@@ -778,39 +766,35 @@
     def _create_chords_tokens(self) -> List[str]:
         """Just create the *Chord* tokens that will populate the base vocabulary.
         This protected method is intended to be used by subclasses when creating their vocabularies.
 
         :return: chord tokens, created from the tokenizer's params
         """
         tokens = []
-        if self.additional_tokens.get("chord_tokens_with_root_note", False):
+        if self.config.chord_tokens_with_root_note:
             tokens += [
                 f"Chord_{root_note}:{chord_quality}"
-                for chord_quality in self.additional_tokens["chord_maps"]
+                for chord_quality in self.config.chord_maps
                 for root_note in PITCH_CLASSES
             ]
         else:
             tokens += [
-                f"Chord_{chord_quality}"
-                for chord_quality in self.additional_tokens["chord_maps"]
+                f"Chord_{chord_quality}" for chord_quality in self.config.chord_maps
             ]
 
         # Unknown chords
-        if self.additional_tokens["chord_unknown"] is not False:
-            if self.additional_tokens["chord_tokens_with_root_note"]:
+        if self.config.chord_unknown is not None:
+            if self.config.chord_tokens_with_root_note:
                 tokens += [
                     f"Chord_{root_note}:{UNKNOWN_CHORD_PREFIX}{i}"
-                    for i in range(*self.additional_tokens["chord_unknown"])
+                    for i in range(*self.config.chord_unknown)
                     for root_note in PITCH_CLASSES
                 ]
             else:
-                tokens += [
-                    f"Chord_{i}"
-                    for i in range(*self.additional_tokens["chord_unknown"])
-                ]
+                tokens += [f"Chord_{i}" for i in range(*self.config.chord_unknown)]
 
         return tokens
 
     def token_id_type(self, id_: int, vocab_id: int = None) -> str:
         r"""Returns the type of the given token id.
 
         :param id_: token id to get the type.
@@ -830,20 +814,20 @@
 
     def _add_special_tokens_to_types_graph(self):
         r"""Adds (inplace) special tokens types to the token types graph dictionary.
         Two exceptions are made for the special BOS (Beginning of Sequence) and EOS (End of Sequence) tokens:
         No token type can precede a BOS token, and EOS token cannot precede any other token.
         """
         original_token_types = list(self.tokens_types_graph.keys())
-        for special_token in self.special_tokens:
+        for special_token in self.config.special_tokens:
             if special_token == "EOS":
                 self.tokens_types_graph["EOS"] = []
             else:
-                self.tokens_types_graph[special_token] = (
-                    original_token_types + self.special_tokens
+                self.tokens_types_graph[special_token] = original_token_types + list(
+                    self.config.special_tokens
                 )
 
             if special_token != "BOS":
                 for token_type in original_token_types:
                     self.tokens_types_graph[token_type].append(special_token)
 
     def __create_durations_tuples(self) -> List[Tuple]:
@@ -854,22 +838,26 @@
         In pure ticks we have: duration = (beat * res + pos) * time_division // res
             Is equivalent to: duration = nb_of_samples * ticks_per_sample
         So in the last example, if time_division is 384: duration = (2 * 8 + 5) * 384 // 8 = 1008 ticks
 
         :return: the duration bins.
         """
         durations = []
-        for beat_range, beat_res in self.beat_res.items():
+        for beat_range, beat_res in self.config.beat_res.items():
             durations += [
                 (beat, pos, beat_res)
                 for beat in range(*beat_range)
                 for pos in range(beat_res)
             ]
         durations += [
-            (max(max(self.beat_res)), 0, self.beat_res[max(self.beat_res)])
+            (
+                max(max(self.config.beat_res)),
+                0,
+                self.config.beat_res[max(self.config.beat_res)],
+            )
         ]  # the last one
         del durations[0]  # removes duration of 0
         return durations
 
     @staticmethod
     def _token_duration_to_ticks(token_duration: str, time_division: int) -> int:
         r"""Converts a *Duration* token value of the form x.x.x, for beat.position.resolution,
@@ -881,47 +869,45 @@
         """
         beat, pos, res = map(int, token_duration.split("."))
         return (beat * res + pos) * time_division // res
 
     def __create_rests(self) -> List[Tuple]:
         r"""Creates the possible rests in beat / position units, as tuple of the form:
         (beat, pos) where beat is the number of beats, pos the number of "samples"
-        The rests are calculated from the value of self.additional_tokens[rest_range],
-        which first value divide a beat to determine the minimum rest represented,
+        The rests are calculated from the value of self.config.rest_range,
+        which first value divides a beat to determine the minimum rest to represent,
         and the second the maximum rest in beats.
         The rests shorter than 1 beat will scale x2, as rests in music theory (semiquaver, quaver, crotchet...)
         Note that the values of the rests in positions will be determined by the beat
         resolution of the first range (self.beat_res)
 
         Example: (4, 6) and a first beat resolution of 8 will give the rests:
             [(0, 2), (0, 4), (1, 0), (2, 0), (3, 0), (4, 0), (5, 0), (6, 0)]
 
         :return: the rests.
         """
-        div, max_beat = self.additional_tokens["rest_range"]
+        div, max_beat = self.config.rest_range
         assert (
             div % 2 == 0 and div <= self._first_beat_res
         ), f"The minimum rest must be divisible by 2 and lower than the first beat resolution ({self._first_beat_res})"
         rests = []
         while div > 1:
             rests.append((0, self._first_beat_res // div))
             div //= 2
         rests += [(i, 0) for i in range(1, max_beat + 1)]
         return rests
 
     def __create_time_signatures(self) -> List[Tuple]:
-        r"""Creates the possible time signatures, as tuple of the form:
+        r"""Creates the possible time signatures, as tuples of the form:
         (nb_beats, beat_res) where nb_beats is the number of beats per bar.
         Example: (3, 4) means one bar is 3 beat long and each beat is a quarter note.
 
         :return: the time signatures.
         """
-        max_beat_res, nb_notes = self.additional_tokens.get(
-            "time_signature_range", (4, 1)
-        )
+        max_beat_res, nb_notes = self.config.time_signature_range
         assert (
             max_beat_res > 0 and math.log2(max_beat_res).is_integer()
         ), "The beat resolution in time signature must be a power of 2"
 
         time_signatures = []
         for i in range(0, int(math.log2(max_beat_res)) + 1):  # 1 ~ max_beat_res
             for j in range(1, ((2**i) * nb_notes) + 1):
@@ -939,15 +925,15 @@
 
         Example: (10, 4), max_beat_res of 8, and nb_notes of 2 will convert the signature into (5, 4).
 
         :param numerator: time signature's numerator (bar length in beats).
         :param denominator: time signature's denominator (beat resolution).
         :return: the numerator and denominator of a reduced and decomposed time signature.
         """
-        max_beat_res, nb_notes = self.additional_tokens["time_signature_range"]
+        max_beat_res, nb_notes = self.config.time_signature_range
 
         # reduction (when denominator exceed max_beat_res)
         while (
             denominator > max_beat_res and denominator % 2 == 0 and numerator % 2 == 0
         ):
             denominator //= 2
             numerator //= 2
@@ -1016,17 +1002,14 @@
         if self.is_multi_voc:
             print(
                 "This tokenizer is based on multiple vocabularies / embedding pooling. It is therefore not compatible"
                 "with Byte Pair Encoding (BPE). Skipping this function call (learn_bpe)."
             )
             return
         assert (
-            not self.bpe_slow
-        ), "This tokenizer has already been trained with slow BPE. You can't retrain it with fast BPE"
-        assert (
             iterator is not None or tokens_paths is not None
         ), "You must give at an iterator or a path to to token "
 
         if vocab_size <= len(self.vocab):
             print(
                 f"vocab_size ({vocab_size}) need to be higher than the size of the current vocabulary "
                 f"({len(self.vocab)}). Skipping BPE training."
@@ -1059,23 +1042,23 @@
             unique_chars = set()
             for seq in iterator:
                 unique_chars.update(*seq)
 
             if len(unique_chars) >= vocab_size:
                 print(
                     f"BPE TRAINING: the provided data comprises {len(unique_chars)} base tokens (character level), "
-                    f"whereas the target BPE vocaulary size is inferior ({vocab_size}). No new token can be learned, "
+                    f"whereas the target BPE vocabulary size is inferior ({vocab_size}). No new token can be learned, "
                     f"skipping BPE training."
                 )
                 return
 
         # Create new tokenizer model
         if self._bpe_model is None or start_from_empty_voc:
             nb_bytes = (
-                len(self.special_tokens)
+                len(self.config.special_tokens)
                 if start_from_empty_voc
                 else len(self._vocab_base)
             )
             voc_start = {chr(i + CHR_ID_START): i for i in range(nb_bytes)}
             self._bpe_model = TokenizerFast(
                 BPE(
                     vocab=voc_start,
@@ -1085,15 +1068,15 @@
                     end_of_word_suffix="",
                     fuse_unk=False,
                 )
             )
 
         # Trains the tokenizer
         special_tokens_bytes = self._ids_to_bytes(
-            self._tokens_to_ids([f"{tok}_None" for tok in self.special_tokens])
+            self._tokens_to_ids([f"{tok}_None" for tok in self.config.special_tokens])
         )
         trainer = BpeTrainer(
             vocab_size=vocab_size,
             special_tokens=special_tokens_bytes,
             show_progress=True,
             **kwargs,
         )
@@ -1144,24 +1127,15 @@
 
     def apply_bpe(self, seq: Union[TokSequence, List[TokSequence]]):
         """Applies Byte Pair Encoding (BPE) to a TokSequence, or list of TokSequences.
         If a list is given, BPE will be applied by batch on all sequences at the time.
 
         :param seq: Sequence(s) to apply BPE.
         """
-        if self.bpe_slow:  # will call slow encoding method, one seq at a time
-            if isinstance(seq, list):
-                for seq_ in seq:
-                    seq_.ids = self.__apply_bpe_slow(seq_.ids)
-                    seq_.ids_bpe_encoded = True
-            else:
-                seq.ids = self.__apply_bpe_slow(seq.ids)
-                seq.ids_bpe_encoded = True
-
-        elif isinstance(seq, list):
+        if isinstance(seq, list):
             for seq_ in seq:
                 self.complete_sequence(seq_)
             encoded_tokens = self._bpe_model.encode_batch(
                 [[t.bytes] for t in seq], is_pretokenized=True
             )
             for seq_, bpe_tokens in zip(seq, encoded_tokens):
                 seq_.ids = bpe_tokens.ids
@@ -1169,267 +1143,14 @@
 
         else:
             self.complete_sequence(seq)
             encoded_tokens = self._bpe_model.encode([seq.bytes], is_pretokenized=True)
             seq.ids = encoded_tokens.ids
             seq.ids_bpe_encoded = True
 
-    def learn_bpe_slow(
-        self,
-        tokens_path: Union[Path, str],
-        vocab_size: int,
-        out_dir: Union[Path, str] = None,
-        files_lim: int = None,
-        save_converted_samples: bool = False,
-        print_seq_len_variation: bool = True,
-    ) -> Tuple[List[float], List[int], List[float]]:
-        r"""**DEPRECIATED - WILL BE REMOVED IN FUTURE UPDATES**
-        Method to construct the vocabulary from BPE, 100% in Python and slower than
-        :py:func:`miditok.MIDITokenizer.learn_bpe`.
-        This method will build (modify) the vocabulary by analyzing an already tokenized dataset to find
-        the most recurrent token successions.
-        **Note that this implementation is in pure Python and will be slow if you use a large amount of
-        tokens files.** It will also not be updated in the future. We advise to use the fast
-        :py:func:`miditok.MIDITokenizer.learn_bpe` method.
-
-        :param tokens_path: path to token files to learn the BPE combinations from.
-        :param vocab_size: the new vocabulary size.
-        :param out_dir: directory to save the tokenizer's parameters and vocabulary after BPE learning is finished.
-        :param files_lim: limit of token files to use. (default: None)
-        :param save_converted_samples: will save in out_path the samples that have been used
-                to create the BPE vocab. Files will keep the same name and relative path. (default: True)
-        :param print_seq_len_variation: prints the mean sequence length before and after BPE,
-                and the variation in %. (default: True)
-        :return: learning metrics, as lists of:
-                - the average number of token combinations covered by the newly created BPE tokens
-                - the maximum number of token combinations
-                - the average sequence length
-                Each index in the list correspond to a learning step.
-        """
-        print(
-            "You are using the slow BPE method, which is depreciated and will be removed in future updates."
-            "We recommend to use the learn_bpe method for much faster (x30-50) learning, encoding and decoding."
-        )
-        assert not self.is_multi_voc, (
-            "You are using a multi-vocabulary tokenizer, "
-            "it is not compatible with byte pair encoding"
-        )
-        assert (
-            not self.has_bpe and not self.bpe_slow
-        ), "This tokenizer has already been trained with fast BPE. You can't retrain it with slow BPE."
-        assert vocab_size > len(self.vocab), (
-            f"vocab_size ({vocab_size}) need to be higher than the size"
-            f"of the current vocabulary ({len(self.vocab)})"
-        )
-        files_paths = list(Path(tokens_path).glob("**/*.json"))
-        assert (
-            len(files_paths) > 0
-        ), "BPE learning: the specified path does not contain tokens files (json)"
-        files_paths_bpe = (
-            choices(files_paths, k=files_lim)
-            if (files_lim is not None and files_lim < len(files_paths))
-            else files_paths
-        )
-        samples, samples_paths = [], []
-        original_lengths = []
-
-        # Loads tokens / samples to analyze
-        for file_path in tqdm(files_paths_bpe, desc="Loading token files"):
-            file = self.load_tokens(file_path)
-            samples.append(file)
-            samples_paths.append(file_path.relative_to(tokens_path))
-            original_lengths += (
-                [len(file["ids"])]
-                if self.unique_track
-                else [len(track) for track in file["ids"]]
-            )
-
-        def replace_token_in_seq(
-            seq: List[int], succession: Tuple[int, int], new_event: str
-        ):
-            j = 0
-            while j < len(seq) - 1:
-                if tuple(seq[j : j + 2]) == succession:
-                    seq[j] = self[f"BPE_{new_event}"]
-                    del seq[j + 1]
-                j += 1
-
-        # Learning Byte Pair Encoding
-        avg_seq_len = [sum(original_lengths) / len(original_lengths)]
-        bpe_comb_nb, bpe_comb_means, bpe_comb_max = [], [], []
-        pbar = tqdm(
-            total=vocab_size - len(self.vocab), desc="Learning byte pair encoding"
-        )
-        while len(self.vocab) < vocab_size:
-            occurrences = {}  # count occurrences of successive tokens
-            for sample in samples:
-                tracks = [sample["ids"]] if self.unique_track else sample["ids"]
-                for track in tracks:
-                    for i in range(len(track) - 1):
-                        try:
-                            occurrences[tuple(track[i : i + 2])] += 1
-                        except KeyError:
-                            occurrences[tuple(track[i : i + 2])] = 1
-
-            # Add new BPE token to vocabulary
-            most_rec_tok_succession = max(
-                occurrences, key=occurrences.get
-            )  # most recurrent succession of two tokens
-            prime_tokens_eq = []  # the equivalent succession with decomposed BPE tokens
-            for token in most_rec_tok_succession:
-                if self[token].split("_")[0] == "BPE":
-                    prime_tokens_eq += map(
-                        int,
-                        self[token].split("_")[1].split(".")[1].split("-"),
-                    )
-                else:
-                    prime_tokens_eq.append(token)
-            final_event_val = (
-                "-".join(map(str, most_rec_tok_succession))
-                + "."
-                + "-".join(map(str, prime_tokens_eq))
-            )
-            self.add_to_vocab(f"BPE_{final_event_val}")
-
-            # Replace newly created token in learning samples
-            for sample in samples:
-                if self.unique_track:
-                    replace_token_in_seq(
-                        sample["ids"], most_rec_tok_succession, final_event_val
-                    )
-                else:
-                    for track in sample["ids"]:
-                        replace_token_in_seq(
-                            track, most_rec_tok_succession, final_event_val
-                        )
-
-            # Compute metrics
-            avg = []
-            for sample in samples:
-                if self.unique_track:
-                    avg.append(len(sample["ids"]))
-                else:
-                    avg += [len(track) for track in sample["ids"]]
-            avg_seq_len.append(np.mean(np.array(avg)).item(0))
-            nb_combs = np.array([len(prime_tokens_eq)])  # bpe-combs.prime-combs
-            bpe_comb_nb = (
-                np.concatenate([bpe_comb_nb, nb_combs])
-                if isinstance(bpe_comb_nb, np.ndarray)
-                else nb_combs
-            )
-            bpe_comb_means.append(np.mean(bpe_comb_nb).item(0))
-            bpe_comb_max.append(np.max(bpe_comb_nb).item(0))
-            pbar.set_postfix(
-                {
-                    "seq_len_variation": f"{(avg_seq_len[-1] - avg_seq_len[0]) / avg_seq_len[0] * 100:.2f}",
-                    "avg_nb_token_combs": f"{bpe_comb_means[-1]:.2f}",
-                    "max_nb_token_combs": f"{bpe_comb_max[-1]}",
-                },
-                refresh=False,
-            )
-            pbar.update(1)
-
-        pbar.close()
-        self.has_bpe = True
-        self.__set_bpe_slow_tokens_successions()
-
-        # Saves dictionary and prints the difference in sequence length
-        if out_dir is not None:
-            if isinstance(out_dir, str):
-                out_dir = Path(out_dir)
-            out_dir.mkdir(parents=True, exist_ok=True)
-
-            if save_converted_samples:
-                for sample, path in zip(samples, samples_paths):
-                    self.save_tokens(
-                        sample["ids"],
-                        Path(out_dir, path).with_suffix(".json"),
-                        sample["programs"],
-                    )
-            self.save_params(
-                out_dir / "config.txt"
-            )  # Saves the parameters with which the MIDIs are converted
-
-        if print_seq_len_variation:
-            print(
-                f"Mean of original lengths: {avg_seq_len[0]}\nMean length after BPE: {avg_seq_len[-1]}"
-            )
-            print(
-                f"Variation from original: {(avg_seq_len[-1] - avg_seq_len[0]) / avg_seq_len[0] * 100:.2f} %"
-            )
-
-        return bpe_comb_means, bpe_comb_max, avg_seq_len
-
-    def __set_bpe_slow_tokens_successions(self):
-        r"""For slow BPE.
-        Creates the bpe_successions attributes, as a dictionary of the form {bpe_token: (tok1, tok2, tok3...)}
-        """
-        self.__bpe_successions = {
-            tok: list(
-                map(
-                    int,
-                    self[tok].split("_")[1].split(".")[0].split("-"),
-                )
-            )
-            for tok, event in enumerate(self.vocab)
-            if event.split("_")[0] == "BPE"
-        }
-
-    def __apply_bpe_slow(self, ids: List[int]) -> List[int]:
-        r"""Converts a sequence of token ids into ids with BPE.
-
-        :param ids: token ids to encode.
-        :return: the ids with BPE applied.
-        """
-        if not self.has_bpe:
-            return ids
-
-        previous_len = len(ids) + 1  # + 1 to fool when entering the loop the first time
-        while previous_len != len(
-            ids
-        ):  # if this is True, it means no more BPE combinations is possible
-            previous_len = len(ids)  # length of the token sequence before applying BPE
-            for (
-                tok,
-                token_succession,
-            ) in (
-                self.__bpe_successions.items()
-            ):  # loops over BPE tokens from the vocabulary
-                occurrences = self.__find_subseq(ids, token_succession)
-                for idx in reversed(occurrences):
-                    ids[idx] = tok
-                    for _ in range(len(token_succession) - 1):
-                        del ids[idx + 1]
-        return ids
-
-    @staticmethod
-    def __find_subseq(in_list: List[int], pattern: List[int]) -> List[int]:
-        """Finds the locations of a pattern within a list.
-        Adapted from: https://stackoverflow.com/questions/10106901/elegant-find-sub-list-in-list
-        Related: https://www.reddit.com/r/learnpython/comments/2xqlwj/using_npwhere_to_find_subarrays/
-        After testing, the numba jit version does not seem to be much faster.
-        The conversion of python lists to numba.typed.List() seems to also take time.
-
-        :param in_list: input list to analyze.
-        :param pattern: pattern to detect.
-        :return: indices of in_list where the pattern has been found.
-        """
-        matches = []
-        next_possible_idx = 0
-        for i in range(len(in_list)):
-            if (
-                in_list[i] == pattern[0]
-                and in_list[i : i + len(pattern)] == pattern
-                and i >= next_possible_idx
-            ):
-                matches.append(i)
-                next_possible_idx = i + len(pattern)
-
-        return matches
-
     def apply_bpe_to_dataset(
         self, dataset_path: Union[Path, str], out_path: Union[Path, str] = None
     ):
         r"""Applies BPE to an already tokenized dataset (with no BPE).
 
         :param dataset_path: path to token files to load.
         :param out_path: output directory to save. If none is given, this method will overwrite original files.
@@ -1451,15 +1172,15 @@
             out_ = (
                 Path(out_path) / path.relative_to(dataset_path)
                 if out_path is not None
                 else path
             )
             self.save_tokens(seq, out_, sample["programs"])
 
-    def _ids_are_bpe_encoded(self, ids: Union[List[int], np.ndarray]) -> bool:
+    def _are_ids_bpe_encoded(self, ids: Union[List[int], np.ndarray]) -> bool:
         r"""A small check telling if a sequence of ids are encoded with BPE.
         This is performed by checking if any id has a value superior or equal to the length
         of the base vocabulary.
 
         :param ids: ids to check
         :return: boolean, True if ids are encoded with BPE, False otherwise.
         """
@@ -1470,55 +1191,29 @@
         This method only modifies the ``.ids`` attribute of the input sequence(s) only and does not complete it.
         This method can also receive a list of sequences, in which case it will decompose BPE on each of them
         recursively.
 
         :param seq: token sequence to decompose.
         """
 
-        if self.bpe_slow:  # will call slow encoding method, one seq at a time
-            if isinstance(seq, list):
-                [self.decode_bpe(seq_) for seq_ in seq]
-            else:
-                seq.ids = self.__decode_bpe_slow(seq.ids)
-                seq.ids_bpe_encoded = False
-
-        elif isinstance(seq, list):
+        if isinstance(seq, list):
             [self.decode_bpe(seq_) for seq_ in seq]
 
         elif isinstance(seq, TokSequence) and seq.ids_bpe_encoded:
             encoded_bytes = [self._bpe_model.id_to_token(id_) for id_ in seq.ids]
             decoded_tokens = [
                 self._vocab_bpe_bytes_to_tokens[byte_] for byte_ in encoded_bytes
             ]
             decoded_tokens = [
                 item for sublist in decoded_tokens for item in sublist
             ]  # flatten
             seq.tokens = decoded_tokens
             seq.ids = self._tokens_to_ids(decoded_tokens)
             seq.ids_bpe_encoded = False
 
-    def __decode_bpe_slow(self, ids: List[int]) -> List[int]:
-        r"""Decodes a sequence of token ids encoded with BPE.
-
-        :param ids: ids sequence to decode.
-        :return: decoded id sequence.
-        """
-        ids = deepcopy(ids)
-        i = 0
-        while i < len(ids):
-            token_type, token_val = self[ids[i]].split("_")
-            if token_type == "BPE":
-                del ids[i]
-                for j, to_insert in enumerate(
-                    map(int, token_val.split(".")[1].split("-"))
-                ):
-                    ids.insert(i + j, to_insert)
-            i += 1
-        return ids
-
     def tokenize_midi_dataset(
         self,
         midi_paths: Union[List[str], List[Path]],
         out_dir: Union[str, Path],
         validation_fn: Callable[[MidiFile], bool] = None,
         data_augment_offsets=None,
         apply_bpe: bool = True,
@@ -1567,15 +1262,15 @@
                 continue
             except (
                 Exception
             ):  # ValueError, OSError, FileNotFoundError, IOError, EOFError, mido.KeySignatureError
                 continue
 
             # Checks the time division is valid
-            if midi.ticks_per_beat < max(self.beat_res.values()) * 4:
+            if midi.ticks_per_beat < max(self.config.beat_res.values()) * 4:
                 continue
             # Passing the MIDI to validation tests if given
             if validation_fn is not None:
                 if not validation_fn(midi):
                     continue
 
             # Converting the MIDI to tokens and saving them as json
@@ -1619,48 +1314,48 @@
         tokens = tokens.tokens
 
         err_type = 0  # i.e. incompatible next type predicted
         err_time = 0  # i.e. goes back or stay in time (does not go forward)
         err_note = 0  # i.e. duplicated
         previous_type = tokens[0].split("_")[0]
         current_pos = -1
-        current_pitches = []
+        current_program = 0
+        current_pitches = {p: [] for p in self.config.programs}
         note_tokens_types = ["Pitch", "NoteOn"]
 
         # Init first note and current pitches if needed
         if previous_type in note_tokens_types:
-            if previous_type in ["Pitch", "NoteOn"]:
-                pitch_val = int(tokens[0].split("_")[1])
-            else:  # PitchVel or PitchVelDur
-                pitch_val = int(tokens[0].split("_")[1].split("-")[0])
-            current_pitches.append(pitch_val)
+            pitch_val = int(tokens[0].split("_")[1])
+            current_pitches[current_program].append(pitch_val)
         elif previous_type == "Position":
             current_pos = int(tokens[0].split("_")[1])
 
         for token in tokens[1:]:
             event_type, event_value = token.split("_")[0], token.split("_")[1]
 
             # Good token type
             if event_type in self.tokens_types_graph[previous_type]:
                 if event_type == "Bar":  # reset
                     current_pos = -1
-                    current_pitches = []
+                    current_pitches = {p: [] for p in self.config.programs}
                 elif event_type in ["TimeShift", "Time-Shift", "Rest"]:
-                    current_pitches = []
+                    current_pitches = {p: [] for p in self.config.programs}
                 elif event_type in note_tokens_types:
                     pitch_val = int(event_value)
-                    if pitch_val in current_pitches:
+                    if pitch_val in current_pitches[current_program]:
                         err_note += 1  # pitch already played at current position
                     else:
-                        current_pitches.append(pitch_val)
+                        current_pitches[current_program].append(pitch_val)
                 elif event_type == "Position":
                     if int(event_value) <= current_pos and previous_type != "Rest":
                         err_time += 1  # token position value <= to the current position
                     current_pos = int(event_value)
-                    current_pitches = []
+                    current_pitches = {p: [] for p in self.config.programs}
+                elif event_type == "Program":  # reset
+                    current_program = int(event_value)
             # Bad token type
             else:
                 err_type += 1
             previous_type = event_type
 
         return (err_type + err_time + err_note) / nb_tok_predicted
 
@@ -1730,98 +1425,111 @@
 
         :param out_path: output path to save the file.
         :param additional_attributes: any additional information to store in the config file.
                 It can be used to override the default attributes saved in the parent method. (default: None)
         """
         if additional_attributes is None:
             additional_attributes = {}
-        if (
-            self.has_bpe and "_vocab_base" not in additional_attributes
-        ):  # saves whole vocab if BPE
+        if self.has_bpe:  # saves whole vocab if BPE
             additional_attributes["_vocab_base"] = self._vocab_base
-            if not self.bpe_slow:
-                additional_attributes["_bpe_model"] = self._bpe_model.to_str()
-                additional_attributes[
-                    "_vocab_base_byte_to_token"
-                ] = self._vocab_base_byte_to_token
-
+            additional_attributes["_bpe_model"] = self._bpe_model.to_str()
+            additional_attributes[
+                "_vocab_base_byte_to_token"
+            ] = self._vocab_base_byte_to_token
+
+        dict_config = self.config.to_dict(serialize=True)
+        dict_config["beat_res"] = {
+            f"{k1}_{k2}": v for (k1, k2), v in dict_config["beat_res"].items()
+        }
         params = {
-            "pitch_range": (self.pitch_range.start, self.pitch_range.stop),
-            "beat_res": {f"{k1}_{k2}": v for (k1, k2), v in self.beat_res.items()},
-            "_nb_velocities": len(self.velocities),
-            "additional_tokens": self.additional_tokens,
-            "special_tokens": self.special_tokens,
+            "config": dict_config,
             "unique_track": self.unique_track,
             "has_bpe": self.has_bpe,
             "tokenization": self.__class__.__name__,
             "miditok_version": CURRENT_VERSION_PACKAGE,
             **additional_attributes,
         }
 
         out_path = Path(out_path)
         out_path.parent.mkdir(parents=True, exist_ok=True)
         with open(out_path, "w") as outfile:
             json.dump(params, outfile, indent=4)
 
-    def load_params(self, config_file_path: Union[str, Path]):
+    def _load_params(self, config_file_path: Union[str, Path]):
         r"""Loads the parameters of the tokenizer from a config file.
+        This method is not intended to be called outside __init__, when creating a tokenizer.
 
         :param config_file_path: path to the tokenizer config file (encoded as json).
         """
         with open(config_file_path) as param_file:
             params = json.load(param_file)
 
-        params["pitch_range"] = range(*params["pitch_range"])
+        # Grab config, or creates one with default parameters (for retro-compatibility with previous version)
+        self.config = TokenizerConfig()
+        config_attributes = list(self.config.to_dict().keys())
+        old_add_tokens_attr = {
+            "Chord": "use_chords",
+            "Rest": "use_rests",
+            "Tempo": "use_tempos",
+            "TimeSignature": "use_time_signatures",
+            "Program": "use_program",
+        }
 
+        # Overwrite config attributes
         for key, value in params.items():
             if key in ["tokenization", "miditok_version"]:
                 continue
-            elif key == "beat_res":
-                value = {
-                    tuple(map(int, beat_range.split("_"))): res
-                    for beat_range, res in value.items()
-                }
-            elif key == "additional_tokens":
-                value["TimeSignature"] = value.get("TimeSignature", False)
             elif key == "_vocab_base":
                 self._vocab_base = value
                 self.__vocab_base_inv = {v: k for k, v in value.items()}
                 continue
             elif key == "_bpe_model":
-                self._bpe_model = TokenizerFast.from_str(
-                    value
-                )  # using 🤗tokenizers builtin method
+                # using 🤗tokenizers builtin method
+                self._bpe_model = TokenizerFast.from_str(value)
                 continue
             elif key == "_vocab_base_byte_to_token":
                 self._vocab_base_byte_to_token = value
                 token_to_byte = {v: k for k, v in value.items()}
                 self._vocab_base_id_to_byte = {
                     i: token_to_byte[tok] for tok, i in self._vocab_base.items()
                 }
                 self._vocab_bpe_bytes_to_tokens = {
                     k: [self._vocab_base_byte_to_token[b] for b in k]
                     for k in self._bpe_model.get_vocab()
                 }
                 continue
+            elif key == "config":
+                value["beat_res"] = {
+                    tuple(map(int, beat_range.split("_"))): res
+                    for beat_range, res in value["beat_res"].items()
+                }
+                value = TokenizerConfig.from_dict(value)
+            elif key in config_attributes:
+                if key == "beat_res":
+                    value = {
+                        tuple(map(int, beat_range.split("_"))): res
+                        for beat_range, res in value.items()
+                    }
+                # Convert old attribute from < v2.1.0 to new for TokenizerConfig
+                elif key in old_add_tokens_attr:
+                    key = old_add_tokens_attr[key]
+                setattr(self.config, key, value)
+                continue
 
             setattr(self, key, value)
 
     @property
     def is_multi_voc(self) -> bool:
         """Returns a bool indicating if the tokenizer uses embedding
         pooling, and so have multiple vocabularies.
 
         :return: True is the tokenizer uses embedding pooling else False.
         """
         return isinstance(self._vocab_base, list)
 
-    @property
-    def bpe_slow(self) -> bool:
-        return self.has_bpe and self._bpe_model is None
-
     def __call__(self, obj: Any, *args, **kwargs):
         r"""Calling a tokenizer allows to directly convert a MIDI to tokens or the other way around.
         The method automatically detects MIDI and token objects, as well as paths and can directly load
         MIDI or token json files before converting them.
         This will call the :py:func:`miditok.MIDITokenizer.midi_to_tokens` if you provide a MIDI object
         or path to a MIDI file, or the :py:func:`miditok.MIDITokenizer.tokens_to_midi` method otherwise.
 
@@ -1846,22 +1554,22 @@
         else:
             return self.tokens_to_midi(obj, *args, **kwargs)
 
     def __len__(self) -> int:
         r"""Returns the length of the vocabulary. If the tokenizer uses embedding
         pooling / have multiple vocabularies, it will return the **sum** of their lengths.
         If the vocabulary was learned with fast BPE, it will return the length of the BPE vocabulary,
-        i.e. the proper number of possible token ids. Otherwise it will return the length of the base vocabulary.
+        i.e. the proper number of possible token ids. Otherwise, it will return the length of the base vocabulary.
         Use the :py:func:`miditok.MIDITokenizer.len` property (``tokenizer.len``) to have the list of lengths.
 
         :return: length of the vocabulary.
         """
         if self.is_multi_voc:
             return sum([len(v) for v in self.vocab])
-        elif self.has_bpe and not self.bpe_slow:
+        elif self.has_bpe:
             return len(self._bpe_model.get_vocab())
         return len(self.vocab)
 
     @property
     def len(self) -> Union[int, List[int]]:
         r"""Returns the length of the vocabulary. If the tokenizer uses embedding
         pooling / have multiple vocabularies, it will return the **list** of their lengths.
@@ -1869,18 +1577,22 @@
         to get the sum of the lengths.
 
         :return: length of the vocabulary.
         """
         return [len(v) for v in self.vocab] if self.is_multi_voc else len(self)
 
     def __repr__(self):
-        return (
-            f'{len(self.len)} tokens {"(multi-voc) " if self.is_multi_voc else ""}'
-            f'{"with BPE" if self.has_bpe else "without BPE"}'
-        )
+        out_str = f"{self.len} tokens"
+        if self.is_multi_voc:
+            out_str += " (multi-voc)"
+        if self.has_bpe:
+            out_str += " with BPE"
+        else:
+            out_str += " without BPE"
+        return out_str
 
     def __getitem__(
         self, item: Union[int, str, Tuple[int, Union[int, str]]]
     ) -> Union[str, int, List[int]]:
         r"""Convert a token (int) to an event (str), or vice-versa.
 
         :param item: a token (int) or an event (str). For tokenizers with embedding pooling / multiple vocabularies
@@ -1921,22 +1633,23 @@
                 if self.is_multi_voc
                 else self.__vocab_base_inv
             )
         return voc[item]
 
     def __eq__(self, other) -> bool:
         r"""Checks if two tokenizers are identical. This is done by comparing their vocabularies,
-        as they are built depending on most of their attributes.
+        and configuration.
 
         :param other: tokenizer to compare.
         :return: True if the vocabulary(ies) are identical, False otherwise.
         """
         if isinstance(other, MIDITokenizer):
             bpe_voc_eq = True
             if self._bpe_model is not None and other._bpe_model is not None:
                 bpe_voc_eq = self._bpe_model.get_vocab() == other._bpe_model.get_vocab()
             return (
                 self._vocab_base == other._vocab_base
                 and bpe_voc_eq
                 and self._vocab_base_byte_to_token == other._vocab_base_byte_to_token
+                and self.config == other.config
             )
         return False
```

### Comparing `miditok-2.0.6/miditok/tokenizations/cp_word.py` & `miditok-2.1.0/miditok/tokenizations/cp_word.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,16 @@
 from typing import List, Tuple, Dict, Optional, Union, Any
-from pathlib import Path
 
 import numpy as np
 from miditoolkit import Instrument, Note, TempoChange
 
 from ..midi_tokenizer import MIDITokenizer, _in_as_seq, _out_as_complete_seq
 from ..classes import TokSequence, Event
 from ..utils import detect_chords
-from ..constants import (
-    PITCH_RANGE,
-    NB_VELOCITIES,
-    BEAT_RES,
-    ADDITIONAL_TOKENS,
-    SPECIAL_TOKENS,
-    TIME_DIVISION,
-    TEMPO,
-    MIDI_INSTRUMENTS,
-)
+from ..constants import TIME_DIVISION, TEMPO, MIDI_INSTRUMENTS
 
 
 class CPWord(MIDITokenizer):
     r"""Introduced with the
     `Compound Word Transformer (Hsiao et al.) <https://ojs.aaai.org/index.php/AAAI/article/view/16091>`_,
     this tokenization is similar to :ref:`REMI` but uses embedding pooling operations to reduce
     the overall sequence length: note tokens (*Pitch*, *Velocity* and *Duration*) are first
@@ -36,78 +26,50 @@
     * (+ Optional) Rest: rest acting as a TimeShift token
     * (+ Optional) Tempo: occurring with position tokens
 
     The output hidden states of the model will then be fed to several output layers
     (one per token type). This means that the training requires to add multiple losses.
     For generation, the decoding implies sample from several distributions, which can be
     very delicate. Hence, we do not recommend this tokenization for generation with small models.
-
-    :param pitch_range: range of MIDI pitches to use
-    :param beat_res: beat resolutions, as a dictionary:
-            {(beat_x1, beat_x2): beat_res_1, (beat_x2, beat_x3): beat_res_2, ...}
-            The keys are tuples indicating a range of beats, ex 0 to 3 for the first bar, and
-            the values are the resolution to apply to the ranges, in samples per beat, ex 8
-    :param nb_velocities: number of velocity bins
-    :param additional_tokens: additional tokens (chords, time signature, rests, tempo...) to use,
-            to be given as a dictionary. (default: None is used)
-    :param special_tokens: list of special tokens. This must be given as a list of strings given
-            only the names of the tokens. (default: ``["PAD", "BOS", "EOS", "MASK"]``)
-    :param params: path to a tokenizer config file. This will override other arguments and
-            load the tokenizer based on the config file. This is particularly useful if the
-            tokenizer learned Byte Pair Encoding. (default: None)
     """
 
-    def __init__(
-        self,
-        pitch_range: range = PITCH_RANGE,
-        beat_res: Dict[Tuple[int, int], int] = BEAT_RES,
-        nb_velocities: int = NB_VELOCITIES,
-        additional_tokens: Dict[str, bool] = ADDITIONAL_TOKENS,
-        special_tokens: List[str] = SPECIAL_TOKENS,
-        params: Union[str, Path] = None,
-    ):
-        # Indexes of additional token types within a compound token
-        additional_tokens["TimeSignature"] = False  # not compatible
+    def _tweak_config_before_creating_voc(self):
+        self.config.use_time_signatures = False
         token_types = ["Family", "Position", "Pitch", "Velocity", "Duration"]
-        add_tokens = ["Program", "Chord", "Rest", "Tempo"]
-        for add_token in add_tokens:
-            if additional_tokens[add_token]:
+        for add_tok_attr, add_token in [
+            ("use_programs", "Program"),
+            ("use_chords", "Chord"),
+            ("use_rests", "Rest"),
+            ("use_tempos", "Tempo"),
+        ]:
+            if getattr(self.config, add_tok_attr):
                 token_types.append(add_token)
         self.vocab_types_idx = {
             type_: idx for idx, type_ in enumerate(token_types)
         }  # used for data augmentation
         self.vocab_types_idx["Bar"] = 1  # same as position
 
-        super().__init__(
-            pitch_range,
-            beat_res,
-            nb_velocities,
-            additional_tokens,
-            special_tokens,
-            params=params,
-        )
-
     @_out_as_complete_seq
     def track_to_tokens(self, track: Instrument) -> TokSequence:
         r"""Converts a track (miditoolkit.Instrument object) into a sequence of tokens (:class:`miditok.TokSequence`).
 
         :param track: MIDI track to convert
         :return: :class:`miditok.TokSequence` of corresponding tokens.
         """
         # Make sure the notes are sorted first by their onset (start) times, second by pitch
         # notes.sort(key=lambda x: (x.start, x.pitch))  # done in midi_to_tokens
         ticks_per_sample = self._current_midi_metadata["time_division"] / max(
-            self.beat_res.values()
+            self.config.beat_res.values()
         )
         ticks_per_bar = self._current_midi_metadata["time_division"] * 4
         dur_bins = self._durations_ticks[self._current_midi_metadata["time_division"]]
         min_rest = (
             self._current_midi_metadata["time_division"] * self.rests[0][0]
             + ticks_per_sample * self.rests[0][1]
-            if self.additional_tokens["Rest"]
+            if self.config.use_rests
             else 0
         )
         tokens: List[List[Union[str, Event]]] = []  # list of lists of tokens
 
         # Creates tokens
         previous_tick = -1
         previous_note_end = (
@@ -119,15 +81,15 @@
             current_tempo_idx
         ].tempo
         for note in track.notes:
             # Bar / Position / (Tempo) / (Rest)
             if note.start != previous_tick:
                 # (Rest)
                 if (
-                    self.additional_tokens["Rest"]
+                    self.config.use_rests
                     and note.start > previous_note_end
                     and note.start - previous_note_end >= min_rest
                 ):
                     previous_tick = previous_note_end
                     rest_beat, rest_pos = divmod(
                         note.start - previous_tick,
                         self._current_midi_metadata["time_division"],
@@ -158,15 +120,15 @@
                         )
                         previous_tick += round(rest_pos_temp * ticks_per_sample)
                         rest_pos -= rest_pos_temp
 
                     current_bar = previous_tick // ticks_per_bar
 
                 # (Tempo)
-                if self.additional_tokens["Tempo"]:
+                if self.config.use_tempos:
                     # If the current tempo is not the last one
                     if current_tempo_idx + 1 < len(
                         self._current_midi_metadata["tempo_changes"]
                     ):
                         # Will loop over incoming tempo changes
                         for tempo_change in self._current_midi_metadata[
                             "tempo_changes"
@@ -192,17 +154,15 @@
 
                 # Position
                 pos_index = int((note.start % ticks_per_bar) / ticks_per_sample)
                 tokens.append(
                     self.__create_cp_token(
                         int(note.start),
                         pos=pos_index,
-                        tempo=current_tempo
-                        if self.additional_tokens["Tempo"]
-                        else None,
+                        tempo=current_tempo if self.config.use_tempos else None,
                         desc="Position",
                     )
                 )
                 previous_tick = note.start
 
             # Note
             duration = note.end - note.start
@@ -218,22 +178,22 @@
                 )
             )
             previous_note_end = max(previous_note_end, note.end)
 
         tokens.sort(key=lambda x: x[0].time)
 
         # Adds chord tokens if specified
-        if self.additional_tokens["Chord"] and not track.is_drum:
+        if self.config.use_chords and not track.is_drum:
             chord_events = detect_chords(
                 track.notes,
                 self._current_midi_metadata["time_division"],
-                chord_maps=self.additional_tokens["chord_maps"],
-                specify_root_note=self.additional_tokens["chord_tokens_with_root_note"],
+                chord_maps=self.config.chord_maps,
+                specify_root_note=self.config.chord_tokens_with_root_note,
                 beat_res=self._first_beat_res,
-                unknown_chords_nb_notes_range=self.additional_tokens["chord_unknown"],
+                unknown_chords_nb_notes_range=self.config.chord_unknown,
             )
             count = 0
             for chord_event in chord_events:
                 for e, cp_token in enumerate(tokens[count:]):
                     if (
                         cp_token[0].time == chord_event.time
                         and cp_token[0].desc == "Position"
@@ -295,16 +255,16 @@
         cp_token_template = [
             Event(type="Family", value="Metric", time=time, desc=desc),
             "Ignore_None",
             "Ignore_None",
             "Ignore_None",
             "Ignore_None",
         ]
-        for add_tok in ["Program", "Chord", "Rest", "Tempo"]:
-            if self.additional_tokens[add_tok]:
+        for add_tok_attr in ["use_programs", "use_chords", "use_rests", "use_tempos"]:
+            if getattr(self.config, add_tok_attr):
                 cp_token_template.append("Ignore_None")
 
         if bar:
             cp_token_template[1] = "Bar_None"
         elif pos is not None:
             cp_token_template[1] = f"Position_{pos}"
             if chord is not None:
@@ -337,18 +297,18 @@
         :param tokens: sequence of tokens to convert. Can be either a Tensor (PyTorch and Tensorflow are supported),
                 a numpy array, a Python list or a TokSequence.
         :param time_division: MIDI time division / resolution, in ticks/beat (of the MIDI to create)
         :param program: the MIDI program of the produced track and if it drum, (default (0, False), piano)
         :return: the miditoolkit instrument object and tempo changes
         """
         assert (
-            time_division % max(self.beat_res.values()) == 0
-        ), f"Invalid time division, please give one divisible by {max(self.beat_res.values())}"
+            time_division % max(self.config.beat_res.values()) == 0
+        ), f"Invalid time division, please give one divisible by {max(self.config.beat_res.values())}"
 
-        ticks_per_sample = time_division // max(self.beat_res.values())
+        ticks_per_sample = time_division // max(self.config.beat_res.values())
         ticks_per_bar = time_division * 4
         name = "Drums" if program[1] else MIDI_INSTRUMENTS[program[0]]["name"]
         instrument = Instrument(program[0], is_drum=program[1], name=name)
         tempo_changes = [
             TempoChange(TEMPO, -1)
         ]  # mock the first tempo change to optimize below
 
@@ -380,20 +340,20 @@
                         current_bar = (
                             0  # as this Position token occurs before any Bar token
                         )
                     current_tick = (
                         current_bar * ticks_per_bar
                         + int(compound_token[1].split("_")[1]) * ticks_per_sample
                     )
-                    if self.additional_tokens["Tempo"]:
+                    if self.config.use_tempos:
                         tempo = int(compound_token[-1].split("_")[1])
                         if tempo != tempo_changes[-1].tempo:
                             tempo_changes.append(TempoChange(tempo, current_tick))
                 elif (
-                    self.additional_tokens["Rest"]
+                    self.config.use_rests
                     and compound_token[self.vocab_types_idx["Rest"]].split("_")[1]
                     != "None"
                 ):
                     if (
                         current_tick < previous_note_end
                     ):  # if in case successive rest happen
                         current_tick = previous_note_end
@@ -424,52 +384,52 @@
 
         vocab = [[] for _ in range(5)]
 
         vocab[0].append("Family_Metric")
         vocab[0].append("Family_Note")
 
         # POSITION
-        nb_positions = max(self.beat_res.values()) * 4  # 4/* time signature
+        nb_positions = max(self.config.beat_res.values()) * 4  # 4/* time signature
         vocab[1].append("Ignore_None")
         vocab[1].append("Bar_None")
         vocab[1] += [f"Position_{i}" for i in range(nb_positions)]
 
         # PITCH
         vocab[2].append("Ignore_None")
-        vocab[2] += [f"Pitch_{i}" for i in self.pitch_range]
+        vocab[2] += [f"Pitch_{i}" for i in range(*self.config.pitch_range)]
 
         # VELOCITY
         vocab[3].append("Ignore_None")
         vocab[3] += [f"Velocity_{i}" for i in self.velocities]
 
         # DURATION
         vocab[4].append("Ignore_None")
         vocab[4] += [
             f'Duration_{".".join(map(str, duration))}' for duration in self.durations
         ]
 
         # PROGRAM
-        if self.additional_tokens["Program"]:
+        if self.config.use_programs:
             vocab += [
                 ["Ignore_None"] + [f"Program_{program}" for program in range(-1, 128)]
             ]
 
         # CHORD
-        if self.additional_tokens["Chord"]:
+        if self.config.use_chords:
             vocab += [["Ignore_None"] + self._create_chords_tokens()]
 
         # REST
-        if self.additional_tokens["Rest"]:
+        if self.config.use_rests:
             vocab += [
                 ["Ignore_None"]
                 + [f'Rest_{".".join(map(str, rest))}' for rest in self.rests]
             ]
 
         # TEMPO
-        if self.additional_tokens["Tempo"]:
+        if self.config.use_tempos:
             vocab += [["Ignore_None"] + [f"Tempo_{i}" for i in self.tempos]]
 
         return vocab
 
     def _create_token_types_graph(self) -> Dict[str, List[str]]:
         r"""Returns a graph (as a dictionary) of the possible token
         types successions.
@@ -485,22 +445,26 @@
         """
         dic = dict()
 
         dic["Bar"] = ["Position", "Bar"]
         dic["Position"] = ["Pitch"]
         dic["Pitch"] = ["Pitch", "Bar", "Position"]
 
-        if self.additional_tokens["Chord"]:
+        if self.config.use_chords:
             dic["Rest"] = ["Rest", "Position"]
             dic["Pitch"] += ["Rest"]
 
-        if self.additional_tokens["Rest"]:
+        if self.config.use_rests:
             dic["Rest"] = ["Rest", "Position", "Bar"]
             dic["Pitch"] += ["Rest"]
 
+        for key in dic:
+            dic[key].append("Ignore")
+        dic["Ignore"] = list(dic.keys())
+
         return dic
 
     @_in_as_seq()
     def tokens_errors(self, tokens: Union[TokSequence, List, np.ndarray, Any]) -> float:
         r"""Checks if a sequence of tokens is made of good token types
         successions and returns the error ratio (lower is better).
         The Pitch and Position values are also analyzed:
```

### Comparing `miditok-2.0.6/miditok/tokenizations/midi_like.py` & `miditok-2.1.0/miditok/tokenizations/midi_like.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,16 @@
 from typing import List, Tuple, Dict, Optional, Union, Any
-from pathlib import Path
 
 import numpy as np
 from miditoolkit import Instrument, Note, TempoChange
 
 from ..midi_tokenizer import MIDITokenizer, _in_as_seq, _out_as_complete_seq
 from ..classes import TokSequence, Event
 from ..utils import detect_chords
 from ..constants import (
-    PITCH_RANGE,
-    NB_VELOCITIES,
-    BEAT_RES,
-    ADDITIONAL_TOKENS,
-    SPECIAL_TOKENS,
     TIME_DIVISION,
     TEMPO,
     MIDI_INSTRUMENTS,
 )
 
 
 class MIDILike(MIDITokenizer):
@@ -24,67 +18,37 @@
     and later used with `Music Transformer (Huang et al.) <https://openreview.net/forum?id=rJe4ShAcF7>`_
     and `MT3 (Gardner et al.) <https://openreview.net/forum?id=iMSjopcOn0p>`_,
     this tokenization simply converts MIDI messages (*NoteOn*, *NoteOff*, *TimeShift*...)
     as tokens, hence the name "MIDI-Like".
     **Note:** as MIDI-Like uses *TimeShifts* events to move the time from note to
     note, it could be unsuited for tracks with long pauses. In such case, the
     maximum *TimeShift* value will be used.
-
-    :param pitch_range: range of MIDI pitches to use
-    :param beat_res: beat resolutions, as a dictionary:
-            {(beat_x1, beat_x2): beat_res_1, (beat_x2, beat_x3): beat_res_2, ...}
-            The keys are tuples indicating a range of beats, ex 0 to 3 for the first bar, and
-            the values are the resolution to apply to the ranges, in samples per beat, ex 8
-    :param nb_velocities: number of velocity bins
-    :param additional_tokens: additional tokens (chords, time signature, rests, tempo...) to use,
-            to be given as a dictionary. (default: None is used)
-    :param special_tokens: list of special tokens. This must be given as a list of strings given
-            only the names of the tokens. (default: ``["PAD", "BOS", "EOS", "MASK"]``)
-    :param params: path to a tokenizer config file. This will override other arguments and
-            load the tokenizer based on the config file. This is particularly useful if the
-            tokenizer learned Byte Pair Encoding. (default: None)
     """
 
-    def __init__(
-        self,
-        pitch_range: range = PITCH_RANGE,
-        beat_res: Dict[Tuple[int, int], int] = BEAT_RES,
-        nb_velocities: int = NB_VELOCITIES,
-        additional_tokens: Dict[str, bool] = ADDITIONAL_TOKENS,
-        special_tokens: List[str] = SPECIAL_TOKENS,
-        params: Union[str, Path] = None,
-    ):
-        additional_tokens["TimeSignature"] = False  # not compatible
-        super().__init__(
-            pitch_range,
-            beat_res,
-            nb_velocities,
-            additional_tokens,
-            special_tokens,
-            params=params,
-        )
+    def _tweak_config_before_creating_voc(self):
+        self.config.use_time_signatures = False
 
     @_out_as_complete_seq
     def track_to_tokens(self, track: Instrument) -> TokSequence:
         r"""Converts a track (miditoolkit.Instrument object) into a sequence of tokens (:class:`miditok.TokSequence`).
         (can probably be achieved faster with Mido objects)
 
         :param track: MIDI track to convert
         :return: :class:`miditok.TokSequence` of corresponding tokens.
         """
         # Make sure the notes are sorted first by their onset (start) times, second by pitch
         # notes.sort(key=lambda x: (x.start, x.pitch))  # done in midi_to_tokens
         ticks_per_sample = self._current_midi_metadata["time_division"] / max(
-            self.beat_res.values()
+            self.config.beat_res.values()
         )
         dur_bins = self._durations_ticks[self._current_midi_metadata["time_division"]]
         min_rest = (
             self._current_midi_metadata["time_division"] * self.rests[0][0]
             + ticks_per_sample * self.rests[0][1]
-            if self.additional_tokens["Rest"]
+            if self.config.use_rests
             else 0
         )
         events = []
 
         # Creates the Note On, Note Off and Velocity events
         for n, note in enumerate(track.notes):
             # Note On
@@ -101,15 +65,15 @@
                 )
             )
             # Note Off
             events.append(
                 Event(type="NoteOff", value=note.pitch, time=note.end, desc=note.end)
             )
         # Adds tempo events if specified
-        if self.additional_tokens["Tempo"]:
+        if self.config.use_tempos:
             for tempo_change in self._current_midi_metadata["tempo_changes"]:
                 events.append(
                     Event(
                         type="Tempo",
                         value=tempo_change.tempo,
                         time=tempo_change.time,
                         desc=tempo_change.tempo,
@@ -125,15 +89,15 @@
         for e, event in enumerate(events.copy()):
             # No time shift
             if event.time == previous_tick:
                 pass
 
             # (Rest)
             elif (
-                self.additional_tokens["Rest"]
+                self.config.use_rests
                 and event.type in ["NoteOn", "Tempo"]
                 and event.time - previous_note_end >= min_rest
             ):
                 rest_beat, rest_pos = divmod(
                     event.time - previous_tick,
                     self._current_midi_metadata["time_division"],
                 )
@@ -196,22 +160,22 @@
                 )
 
             if event.type == "NoteOn":
                 previous_note_end = max(previous_note_end, event.desc)
             previous_tick = event.time
 
         # Adds chord events if specified
-        if self.additional_tokens["Chord"] and not track.is_drum:
+        if self.config.use_chords and not track.is_drum:
             events += detect_chords(
                 track.notes,
                 self._current_midi_metadata["time_division"],
-                chord_maps=self.additional_tokens["chord_maps"],
-                specify_root_note=self.additional_tokens["chord_tokens_with_root_note"],
+                chord_maps=self.config.chord_maps,
+                specify_root_note=self.config.chord_tokens_with_root_note,
                 beat_res=self._first_beat_res,
-                unknown_chords_nb_notes_range=self.additional_tokens["chord_unknown"],
+                unknown_chords_nb_notes_range=self.config.chord_unknown,
             )
 
         events.sort(key=lambda x: (x.time, self._order(x)))
 
         return TokSequence(events=events)
 
     @_in_as_seq()
@@ -228,15 +192,15 @@
                 a numpy array, a Python list or a TokSequence.
         :param time_division: MIDI time division / resolution, in ticks/beat (of the MIDI to create)
         :param program: the MIDI program of the produced track and if it drum, (default (0, False), piano)
         :param default_duration: default duration (in ticks) in case a Note On event occurs without its associated
                                 note off event. Leave None to discard Note On with no Note Off event.
         :return: the miditoolkit instrument object and tempo changes
         """
-        ticks_per_sample = time_division // max(self.beat_res.values())
+        ticks_per_sample = time_division // max(self.config.beat_res.values())
         events = (
             tokens.events
             if tokens.events is not None
             else [Event(*tok.split("_")) for tok in tokens.tokens]
         )
 
         max_duration = self.durations[-1][0] * time_division + self.durations[-1][1] * (
@@ -317,41 +281,41 @@
         will be added to the vocabulary by :class:`miditok.MIDITokenizer`.
 
         :return: the vocabulary as a list of string.
         """
         vocab = []
 
         # NOTE ON
-        vocab += [f"NoteOn_{i}" for i in self.pitch_range]
+        vocab += [f"NoteOn_{i}" for i in range(*self.config.pitch_range)]
 
         # NOTE OFF
-        vocab += [f"NoteOff_{i}" for i in self.pitch_range]
+        vocab += [f"NoteOff_{i}" for i in range(*self.config.pitch_range)]
 
         # VELOCITY
         vocab += [f"Velocity_{i}" for i in self.velocities]
 
         # TIME SHIFTS
         vocab += [
             f'TimeShift_{".".join(map(str, duration))}' for duration in self.durations
         ]
 
         # CHORD
-        if self.additional_tokens["Chord"]:
+        if self.config.use_chords:
             vocab += self._create_chords_tokens()
 
         # REST
-        if self.additional_tokens["Rest"]:
+        if self.config.use_rests:
             vocab += [f'Rest_{".".join(map(str, rest))}' for rest in self.rests]
 
         # TEMPO
-        if self.additional_tokens["Tempo"]:
+        if self.config.use_tempos:
             vocab += [f"Tempo_{i}" for i in self.tempos]
 
         # PROGRAM
-        if self.additional_tokens["Program"]:
+        if self.config.use_programs:
             vocab += [f"Program_{program}" for program in range(-1, 128)]
 
         return vocab
 
     def _create_token_types_graph(self) -> Dict[str, List[str]]:
         r"""Returns a graph (as a dictionary) of the possible token
         types successions.
@@ -363,28 +327,28 @@
         dic = dict()
 
         dic["NoteOn"] = ["Velocity"]
         dic["Velocity"] = ["NoteOn", "TimeShift"]
         dic["TimeShift"] = ["NoteOff", "NoteOn"]
         dic["NoteOff"] = ["NoteOff", "NoteOn", "TimeShift"]
 
-        if self.additional_tokens["Chord"]:
+        if self.config.use_chords:
             dic["Chord"] = ["NoteOn"]
             dic["TimeShift"] += ["Chord"]
             dic["NoteOff"] += ["Chord"]
 
-        if self.additional_tokens["Tempo"]:
+        if self.config.use_tempos:
             dic["TimeShift"] += ["Tempo"]
             dic["Tempo"] = ["NoteOn", "TimeShift"]
-            if self.additional_tokens["Chord"]:
+            if self.config.use_chords:
                 dic["Tempo"] += ["Chord"]
 
-        if self.additional_tokens["Rest"]:
+        if self.config.use_rests:
             dic["Rest"] = ["Rest", "NoteOn", "TimeShift"]
-            if self.additional_tokens["Chord"]:
+            if self.config.use_chords:
                 dic["Rest"] += ["Chord"]
             dic["NoteOff"] += ["Rest"]
 
         return dic
 
     @_in_as_seq(complete=False, decode_bpe=False)
     def tokens_errors(self, tokens: Union[TokSequence, List, np.ndarray, Any]) -> float:
@@ -402,17 +366,17 @@
             self.decode_bpe(tokens)
         self.complete_sequence(tokens)
 
         # Override from here
 
         err = 0
         current_pitches = []
-        max_duration = self.durations[-1][0] * max(self.beat_res.values())
+        max_duration = self.durations[-1][0] * max(self.config.beat_res.values())
         max_duration += self.durations[-1][1] * (
-            max(self.beat_res.values()) // self.durations[-1][2]
+            max(self.config.beat_res.values()) // self.durations[-1][2]
         )
 
         events = (
             tokens.events
             if tokens.events is not None
             else [Event(*tok.split("_")) for tok in tokens.tokens]
         )
@@ -431,15 +395,15 @@
                     for j in range(i + 1, len(events)):
                         if events[j].type == "NoteOff" and int(events[j].value) == int(
                             events[i].value
                         ):
                             break  # all good
                         elif events[j].type == "TimeShift":
                             offset_sample += self._token_duration_to_ticks(
-                                events[j].value, max(self.beat_res.values())
+                                events[j].value, max(self.config.beat_res.values())
                             )
 
                         if (
                             offset_sample > max_duration
                         ):  # will not look for Note Off beyond
                             err += 1
                             break
```

### Comparing `miditok-2.0.6/miditok/tokenizations/mmm.py` & `miditok-2.1.0/miditok/tokenizations/mmm.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Tuple, Union, cast
 
 import numpy as np
 from miditoolkit import Instrument, MidiFile, Note, TempoChange, TimeSignature
 
-from ..classes import Event, TokSequence
+from ..classes import Event, TokSequence, TokenizerConfig
 from ..constants import (
-    ADDITIONAL_TOKENS,
-    BEAT_RES,
     MIDI_INSTRUMENTS,
-    NB_VELOCITIES,
-    PITCH_RANGE,
-    SPECIAL_TOKENS,
     TEMPO,
     TIME_DIVISION,
     TIME_SIGNATURE,
     MMM_DENSITY_BINS_MAX,
 )
 from ..midi_tokenizer import MIDITokenizer, _in_as_seq, _out_as_complete_seq
 from ..utils import detect_chords
@@ -27,92 +22,69 @@
     Tracks are tokenized independently and concatenated into a single token sequence.
     ``Bar_Fill`` tokens are used to specify the bars to fill (or inpaint, or rewrite), the new tokens are then
     autoregressively generated.
     Note that *this implementation represents note durations with ``Duration`` tokens* instead of the ``NoteOff``
     strategy of the [original paper](https://arxiv.org/abs/2008.06048). The reason being that ``NoteOff`` tokens perform
     poorer for generation with causal models.
 
-    :param pitch_range: range of MIDI pitches to use
-    :param beat_res: beat resolutions, as a dictionary:
-            {(beat_x1, beat_x2): beat_res_1, (beat_x2, beat_x3): beat_res_2, ...}
-            The keys are tuples indicating a range of beats, ex 0 to 3 for the first bar, and
-            the values are the resolution to apply to the ranges, in samples per beat, ex 8
-    :param nb_velocities: number of velocity bins
-    :param additional_tokens: additional tokens (chords, time signature, rests, tempo...) to use,
-            to be given as a dictionary. (default: None is used)
-    :param special_tokens: list of special tokens. This must be given as a list of strings given
-            only the names of the tokens. (default: ``["PAD", "BOS", "EOS", "MASK"]``)
+    :param tokenizer_config: the tokenizer's configuration, as a :class:`miditok.classes.TokenizerConfig` object.
     :param density_bins_max: tuple specifying the number of density bins, and the maximum density in
             notes per beat to consider. (default: (10, 20))
     :param params: path to a tokenizer config file. This will override other arguments and
             load the tokenizer based on the config file. This is particularly useful if the
             tokenizer learned Byte Pair Encoding. (default: None)
     """
 
     def __init__(
         self,
-        pitch_range: range = PITCH_RANGE,
-        beat_res: Dict[Tuple[int, int], int] = BEAT_RES,
-        nb_velocities: int = NB_VELOCITIES,
-        additional_tokens: Dict[
-            str, Union[bool, int, Tuple[int, int]]
-        ] = ADDITIONAL_TOKENS,
-        special_tokens: List[str] = SPECIAL_TOKENS,
+        tokenizer_config: TokenizerConfig = None,
         density_bins_max: Tuple[int, int] = MMM_DENSITY_BINS_MAX,
         params: Optional[Union[str, Path]] = None,
     ):
-        additional_tokens["Program"] = True  # required
-        additional_tokens["Rest"] = False
-        self.programs = additional_tokens.get("programs", list(range(-1, 128)))
-        self.density_bins_max = density_bins_max
-        self.note_densities = np.linspace(
-            0, density_bins_max[1], density_bins_max[0] + 1, dtype=np.intc
-        )
-        super().__init__(
-            pitch_range,
-            beat_res,
-            nb_velocities,
-            additional_tokens,
-            special_tokens,
-            unique_track=True,  # handles multi-track sequences in single stream
-            params=params,  # type: ignore
-        )
-
-    def save_params(
-        self, out_path: Union[str, Path], additional_attributes: Optional[Dict] = None
-    ):
-        r"""Saves the config / parameters of the tokenizer in a json encoded file.
-        This can be useful to keep track of how a dataset has been tokenized.
-
-        :param out_path: output path to save the file.
-        :param additional_attributes: any additional information to store in the config file.
-                It can be used to override the default attributes saved in the parent method. (default: None)
-        """
-        if additional_attributes is None:
-            additional_attributes = {}
-        additional_attributes_tmp = {
-            "density_bins_max": self.density_bins_max,
-            **additional_attributes,
-        }
-        super().save_params(out_path, additional_attributes_tmp)
+        if (
+            tokenizer_config is not None
+            and "density_bins_max" not in tokenizer_config.additional_params
+        ):
+            tokenizer_config.additional_params["density_bins_max"] = density_bins_max
+        super().__init__(tokenizer_config, True, params)
+
+    def _tweak_config_before_creating_voc(self):
+        self.config.use_programs = True
+        self.config.use_rests = False
+        # Recreate densities here just in case density_bins_max was loaded from params (list to np array)
+        if "note_densities" in self.config.additional_params:
+            if isinstance(
+                self.config.additional_params["note_densities"], (list, tuple)
+            ):
+                self.config.additional_params["note_densities"] = np.array(
+                    self.config.additional_params["note_densities"]
+                )
+        else:
+            self.config.additional_params["note_densities"] = np.linspace(
+                0,
+                self.config.additional_params["density_bins_max"][1],
+                self.config.additional_params["density_bins_max"][0] + 1,
+                dtype=np.intc,
+            )
 
     def track_to_tokens(self, track: Instrument) -> List[Event]:
         r"""Converts a track (miditoolkit.Instrument object) into a sequence of Event (:class:`miditok.Event`).
 
         :param track: MIDI track to convert
         :return: :class:`miditok.TokSequence` of corresponding tokens.
         """
         # Make sure the notes are sorted first by their onset (start) times, second by pitch
         # notes.sort(key=lambda x: (x.start, x.pitch))  # done in midi_to_tokens
         time_division = self._current_midi_metadata["time_division"]
         dur_bins = self._durations_ticks[self._current_midi_metadata["time_division"]]
+        note_density_bins = self.config.additional_params["note_densities"]
 
         # Creates first events
         note_density = len(track.notes) / self._current_midi_metadata["max_tick"]
-        note_density = int(np.argmin(np.abs(dur_bins - note_density)))
+        note_density = int(np.argmin(np.abs(note_density_bins - note_density)))
         events: List[Event] = [
             Event("Track", "Start", 0),
             Event(
                 type="Program",
                 value=-1 if track.is_drum else track.program,
                 time=0,
             ),
@@ -125,40 +97,40 @@
                 type="Bar",
                 value="Start",
                 time=0,
             ),
         ]
 
         # (Chord)
-        if self.additional_tokens.get("Chord", False) and not track.is_drum:
+        if self.config.use_chords and not track.is_drum:
             chords = detect_chords(
                 track.notes,
                 self._current_midi_metadata["time_division"],
-                chord_maps=self.additional_tokens["chord_maps"],
-                specify_root_note=self.additional_tokens["chord_tokens_with_root_note"],
+                chord_maps=self.config.chord_maps,
+                specify_root_note=self.config.chord_tokens_with_root_note,
                 beat_res=self._first_beat_res,
-                unknown_chords_nb_notes_range=self.additional_tokens["chord_unknown"],
+                unknown_chords_nb_notes_range=self.config.chord_unknown,
             )
             for chord in chords:
                 events.append(chord)
 
         # (Tempo)
-        if self.additional_tokens["Tempo"]:
+        if self.config.use_tempos:
             for tempo_change in self._current_midi_metadata["tempo_changes"]:
                 events.append(
                     Event(
                         type="Tempo",
                         value=tempo_change.tempo,
                         time=tempo_change.time,
                         desc=tempo_change.tempo,
                     )
                 )
 
         # (Time signature)
-        if self.additional_tokens["TimeSignature"]:
+        if self.config.use_time_signatures:
             for time_sig in self._current_midi_metadata["time_sig_changes"]:
                 events.append(
                     Event(
                         type="TimeSig",
                         value=f"{time_sig.numerator}/{time_sig.denominator}",
                         time=time_sig.time,
                         desc=(time_sig.numerator, time_sig.denominator),
@@ -291,32 +263,31 @@
         :param output_path: path to save the file. (default: None)
         :param time_division: MIDI time division / resolution, in ticks/beat (of the MIDI to create).
         :return: the midi object (:class:`miditoolkit.MidiFile`).
         """
         tokens = cast(TokSequence, tokens)
         midi = MidiFile(ticks_per_beat=time_division)
         assert (
-            time_division % max(self.beat_res.values()) == 0
-        ), f"Invalid time division, please give one divisible by {max(self.beat_res.values())}"
+            time_division % max(self.config.beat_res.values()) == 0
+        ), f"Invalid time division, please give one divisible by {max(self.config.beat_res.values())}"
         tokens = cast(List[str], tokens.tokens)  # for reducing type errors
-        ticks_per_sample = time_division // max(self.beat_res.values())
+        ticks_per_sample = time_division // max(self.config.beat_res.values())
 
         # RESULTS
         instruments: List[Instrument] = []
         tempo_changes = [
             TempoChange(TEMPO, -1)
         ]  # mock the first tempo change to optimize below
         time_signature_changes = [
             TimeSignature(*TIME_SIGNATURE, 0)
         ]  # mock the first time signature change to optimize below
         ticks_per_bar = time_division * TIME_SIGNATURE[0]  # init
 
         current_tick = 0
         current_bar = -1
-        current_program = 0
         previous_note_end = 0  # unused (rest)
         for ti, token in enumerate(tokens):
             tok_type, tok_val = token.split("_")
             if tok_type == "Program":
                 current_program = int(tok_val)
                 instruments.append(
                     Instrument(
@@ -412,27 +383,23 @@
         The :class:`miditok.MIDITokenizer` main class will then create the "real" vocabulary as
         a dictionary.
         Special tokens have to be given when creating the tokenizer, and
         will be added to the vocabulary by :class:`miditok.MIDITokenizer`.
 
         :return: the vocabulary as a list of string.
         """
-        # Recreate densities here just in case density_bins_max was loaded from params
-        self.note_densities = np.linspace(
-            0, self.density_bins_max[1], self.density_bins_max[0] + 1, dtype=np.intc
-        )
         vocab = []
 
         # TRACK / BAR / FILL
         vocab += ["Track_Start", "Track_End"]
         vocab += ["Bar_Start", "Bar_End", "Bar_Fill"]
         vocab += ["Fill_Start", "Fill_End"]
 
         # PITCH
-        vocab += [f"Pitch_{i}" for i in self.pitch_range]
+        vocab += [f"Pitch_{i}" for i in range(*self.config.pitch_range)]
 
         # VELOCITY
         vocab += [f"Velocity_{i}" for i in self.velocities]
 
         # DURATION
         vocab += [
             f'Duration_{".".join(map(str, duration))}' for duration in self.durations
@@ -441,31 +408,32 @@
         # TIME SHIFTS
         vocab += [
             f'TimeShift_{".".join(map(str, self.durations[i]))}'
             for i in range(len(self.durations))
         ]
 
         # NOTE DENSITY
-        vocab += [f"NoteDensity_{i}" for i in self.note_densities]
+        vocab += [
+            f"NoteDensity_{i}" for i in self.config.additional_params["note_densities"]
+        ]
 
         # TIME SIGNATURE
-        if self.additional_tokens["TimeSignature"]:
+        if self.config.use_time_signatures:
             vocab += [f"TimeSig_{i[0]}/{i[1]}" for i in self.time_signatures]
 
         # CHORD
-        if self.additional_tokens["Chord"]:
+        if self.config.use_chords:
             vocab += self._create_chords_tokens()
 
         # TEMPO
-        if self.additional_tokens["Tempo"]:
+        if self.config.use_tempos:
             vocab += [f"Tempo_{i}" for i in self.tempos]
 
         # PROGRAM
-        if self.additional_tokens["Program"]:
-            vocab += [f"Program_{program}" for program in self.programs]
+        vocab += [f"Program_{program}" for program in self.config.programs]
 
         return vocab
 
     def _create_token_types_graph(self) -> Dict[str, List[str]]:
         r"""Returns a graph (as a dictionary) of the possible token
         types successions.
 
@@ -478,28 +446,28 @@
         dic["Track"] = ["Program", "Track"]
         dic["Program"] = ["NoteDensity"]
         dic["NoteDensity"] = ["Bar"]
         dic["Pitch"] = ["Velocity"]
         dic["Velocity"] = ["Duration"]
         dic["Duration"] = ["Pitch", "TimeShift", "Bar"]
 
-        if self.additional_tokens["TimeSignature"]:
+        if self.config.use_time_signatures:
             dic["Bar"] += ["TimeSig"]
             dic["TimeSig"] = ["Pitch", "TimeShift"]
 
-        if self.additional_tokens["Chord"]:
+        if self.config.use_chords:
             dic["Chord"] = ["TimeShift", "Pitch"]
             dic["Bar"] += ["Chord"]
             dic["TimeShift"] += ["Chord"]
 
-        if self.additional_tokens["Tempo"]:
+        if self.config.use_tempos:
             dic["Tempo"] = ["TimeShift", "Pitch", "Bar"]
             dic["Bar"] += ["Tempo"]
             dic["TimeShift"] += ["Tempo"]
-            if self.additional_tokens["TimeSignature"]:
+            if self.config.use_time_signatures:
                 dic["TimeSig"] += ["Tempo"]
 
         dic["Fill"] = list(dic.keys())
 
         return dic
 
     @staticmethod
```

### Comparing `miditok-2.0.6/miditok/tokenizations/mumidi.py` & `miditok-2.1.0/miditok/tokenizations/mumidi.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,18 @@
 from math import ceil
-from pathlib import Path, PurePath
+from pathlib import Path
 from typing import List, Tuple, Dict, Optional, Union, Any
 
 import numpy as np
 from miditoolkit import MidiFile, Instrument, Note, TempoChange
 
 from ..midi_tokenizer import MIDITokenizer, _in_as_seq, _out_as_complete_seq
-from ..classes import TokSequence, Event
+from ..classes import TokSequence, Event, TokenizerConfig
 from ..utils import detect_chords
 from ..constants import (
-    PITCH_RANGE,
-    NB_VELOCITIES,
-    BEAT_RES,
-    ADDITIONAL_TOKENS,
-    SPECIAL_TOKENS,
     TIME_DIVISION,
     TEMPO,
     MIDI_INSTRUMENTS,
     DRUM_PITCH_RANGE,
 )
 
 
@@ -42,105 +37,59 @@
     For generation, the decoding implies sample from several distributions, which can be
     very delicate. Hence, we do not recommend this tokenization for generation with small models.
 
     **Notes:**
         * Tokens are first sorted by time, then track, then pitch values.
         * Tracks with the same *Program* will be merged.
 
-    :param pitch_range: range of MIDI pitches to use
-    :param beat_res: beat resolutions, as a dictionary:
-            {(beat_x1, beat_x2): beat_res_1, (beat_x2, beat_x3): beat_res_2, ...}
-            The keys are tuples indicating a range of beats, ex 0 to 3 for the first bar, and
-            the values are the resolution to apply to the ranges, in samples per beat, ex 8
-    :param nb_velocities: number of velocity bins
-    :param additional_tokens: additional tokens (chords, time signature, rests, tempo...) to use,
-            to be given as a dictionary. (default: None is used)
-    :param special_tokens: list of special tokens. This must be given as a list of strings given
-            only the names of the tokens. (default: ``["PAD", "BOS", "EOS", "MASK"]``)
+    :param tokenizer_config: the tokenizer's configuration, as a :class:`miditok.classes.TokenizerConfig` object.
+    :param drum_pitch_range: range of used MIDI pitches for drums exclusively
     :param params: path to a tokenizer config file. This will override other arguments and
             load the tokenizer based on the config file. This is particularly useful if the
             tokenizer learned Byte Pair Encoding. (default: None)
-    :param drum_pitch_range: range of used MIDI pitches for drums exclusively
     """
 
     def __init__(
         self,
-        pitch_range: range = PITCH_RANGE,
-        beat_res: Dict[Tuple[int, int], int] = BEAT_RES,
-        nb_velocities: int = NB_VELOCITIES,
-        additional_tokens: Dict[str, bool] = ADDITIONAL_TOKENS,
-        special_tokens: List[str] = SPECIAL_TOKENS,
+        tokenizer_config: TokenizerConfig = None,
+        drum_pitch_range: Tuple[int, int] = DRUM_PITCH_RANGE,
         params: Union[str, Path] = None,
-        drum_pitch_range: range = DRUM_PITCH_RANGE,
     ):
-        additional_tokens["Rest"] = False
-        additional_tokens["TimeSignature"] = False  # not compatible
-        self.drum_pitch_range = drum_pitch_range
-        self.programs = additional_tokens.get("programs", list(range(-1, 128)))
-        # used in place of positional encoding
-        self.max_bar_embedding = 60  # this attribute might increase during encoding
+        if tokenizer_config is not None:
+            if "drum_pitch_range" not in tokenizer_config.additional_params:
+                tokenizer_config.additional_params[
+                    "drum_pitch_range"
+                ] = drum_pitch_range
+            if "max_bar_embedding" not in tokenizer_config.additional_params:
+                # this attribute might increase over tokenizations, if the tokenizer encounter longer MIDIs
+                tokenizer_config.additional_params["max_bar_embedding"] = 60
+        super().__init__(tokenizer_config, True, params=params)
+
+    def _tweak_config_before_creating_voc(self):
+        self.config.use_rests = False
+        self.config.use_time_signatures = False
+        # self.unique_track = True
+
         self.vocab_types_idx = {
             "Pitch": 0,
             "DrumPitch": 0,
             "Position": 0,
             "Bar": 0,
             "Program": 0,
             "BarPosEnc": 1,
             "PositionPosEnc": 2,
             "Velocity": -2,
             "Duration": -1,
         }
-        if additional_tokens["Chord"]:
+        if self.config.use_chords:
             self.vocab_types_idx["Chord"] = 0
-        if additional_tokens["Rest"]:
+        if self.config.use_rests:
             self.vocab_types_idx["Rest"] = 0
-        if additional_tokens["Tempo"]:
+        if self.config.use_tempos:
             self.vocab_types_idx["Tempo"] = -3
-        super().__init__(
-            pitch_range,
-            beat_res,
-            nb_velocities,
-            additional_tokens,
-            special_tokens,
-            True,
-            params=params,
-        )
-
-    def save_params(
-        self, out_path: Union[str, Path, PurePath], additional_attributes: Dict = None
-    ):
-        r"""Saves the config / parameters of the tokenizer in a json encoded file.
-        This can be useful to keep track of how a dataset has been tokenized.
-        **Note:** if you override this method, you should probably call it (super()) at the end
-            and use the additional_attributes argument.
-
-        :param out_path: output path to save the file.
-        :param additional_attributes: any additional information to store in the config file.
-                It can be used to override the default attributes saved in the parent method. (default: None)
-        """
-        if additional_attributes is None:
-            additional_attributes = {}
-        additional_attributes_tmp = {
-            "max_bar_embedding": self.max_bar_embedding,
-            "programs": self.programs,
-            "drum_pitch_range": (
-                self.drum_pitch_range.start,
-                self.drum_pitch_range.stop,
-            ),
-            **additional_attributes,
-        }
-        super().save_params(out_path, additional_attributes_tmp)
-
-    def load_params(self, config_file_path: Union[str, Path, PurePath]):
-        r"""Load the parameters of the tokenizer from a config file.
-
-        :param config_file_path: path to the tokenizer config file (encoded as json).
-        """
-        super().load_params(config_file_path)
-        self.drum_pitch_range = range(*self.drum_pitch_range)
 
     @_out_as_complete_seq
     def _midi_to_tokens(self, midi: MidiFile, *args, **kwargs) -> TokSequence:
         r"""Tokenize a MIDI file.
         Each pooled token will be a list of the form (index: Token type):
         * 0: Pitch / DrumPitch / Position / Bar / Program / (Chord) / (Rest)
         * 1: BarPosEnc
@@ -171,50 +120,44 @@
             "key_sig_changes": midi.key_signature_changes,
         }
 
         # **************** OVERRIDE FROM HERE, KEEP THE LINES ABOVE IN YOUR METHOD ****************
 
         # Check bar embedding limit, update if needed
         nb_bars = ceil(midi.max_tick / (midi.ticks_per_beat * 4))
-        if self.max_bar_embedding < nb_bars:
-            for i in range(self.max_bar_embedding, nb_bars):
+        if self.config.additional_params["max_bar_embedding"] < nb_bars:
+            for i in range(self.config.additional_params["max_bar_embedding"], nb_bars):
                 self.add_to_vocab(f"BarPosEnc_{i}", 1)
-            self.max_bar_embedding = nb_bars
+            self.config.additional_params["max_bar_embedding"] = nb_bars
 
         # Convert each track to tokens (except first pos to track time)
         note_tokens = []
         for track in midi.instruments:
-            if track.program in self.programs:
+            if track.program in self.config.programs:
                 note_tokens += self.track_to_tokens(track)
 
         note_tokens.sort(
             key=lambda x: (x[0].time, x[0].desc)
         )  # Sort by time then track
 
-        """from copy import deepcopy  # TODO remove
-        toto = deepcopy(note_tokens)
-        for i in range(len(toto)):
-            for j in range(1, len(toto[i])):
-                toto[i][j] = self[j, toto[i][j]]"""
-
-        ticks_per_sample = midi.ticks_per_beat / max(self.beat_res.values())
+        ticks_per_sample = midi.ticks_per_beat / max(self.config.beat_res.values())
         ticks_per_bar = midi.ticks_per_beat * 4
         tokens = []
 
         current_tick = -1
         current_bar = -1
         current_pos = -1
         current_track = -2  # because -2 doesn't exist
         current_tempo_idx = 0
         current_tempo = self.current_midi_metadata["tempo_changes"][
             current_tempo_idx
         ].tempo
         for note_token in note_tokens:
             # (Tempo) update tempo values current_tempo
-            if self.additional_tokens["Tempo"]:
+            if self.config.use_tempos:
                 # If the current tempo is not the last one
                 if current_tempo_idx + 1 < len(
                     self.current_midi_metadata["tempo_changes"]
                 ):
                     # Will loop over incoming tempo changes
                     for tempo_change in self.current_midi_metadata["tempo_changes"][
                         current_tempo_idx + 1 :
@@ -238,44 +181,44 @@
                     nb_new_bars = current_tick // ticks_per_bar - current_bar
                     for i in range(nb_new_bars):
                         bar_token = [
                             "Bar_None",
                             f"BarPosEnc_{current_bar + i + 1}",
                             "PositionPosEnc_None",
                         ]
-                        if self.additional_tokens["Tempo"]:
+                        if self.config.use_tempos:
                             bar_token.append(f"Tempo_{current_tempo}")
                         tokens.append(bar_token)
                     current_bar += nb_new_bars
                 # Position
                 pos_token = [
                     f"Position_{current_pos}",
                     f"BarPosEnc_{current_bar}",
                     f"PositionPosEnc_{current_pos}",
                 ]
-                if self.additional_tokens["Tempo"]:
+                if self.config.use_tempos:
                     pos_token.append(f"Tempo_{current_tempo}")
                 tokens.append(pos_token)
             # Program (track)
             if note_token[0].desc != current_track:
                 current_track = note_token[0].desc
                 track_token = [
                     f"Program_{current_track}",
                     f"BarPosEnc_{current_bar}",
                     f"PositionPosEnc_{current_pos}",
                 ]
-                if self.additional_tokens["Tempo"]:
+                if self.config.use_tempos:
                     track_token.append(f"Tempo_{current_tempo}")
                 tokens.append(track_token)
 
             # Adding bar and position tokens to notes for positional encoding
             note_token[0] = str(note_token[0])
             note_token.insert(1, f"BarPosEnc_{current_bar}")
             note_token.insert(2, f"PositionPosEnc_{current_pos}")
-            if self.additional_tokens["Tempo"]:
+            if self.config.use_tempos:
                 note_token.insert(3, f"Tempo_{current_tempo}")
             tokens.append(note_token)
 
         return TokSequence(tokens=tokens)
 
     def track_to_tokens(self, track: Instrument) -> List[List[Union[Event, str]]]:
         r"""Converts a track (miditoolkit.Instrument object) into a sequence of tokens (:class:`miditok.TokSequence`).
@@ -320,22 +263,22 @@
                         ),
                         f"Velocity_{note.velocity}",
                         f'Duration_{".".join(map(str, self.durations[dur_idx]))}',
                     ]
                 )
 
         # Adds chord tokens if specified
-        if self.additional_tokens["Chord"] and not track.is_drum:
+        if self.config.use_chords and not track.is_drum:
             chords = detect_chords(
                 track.notes,
                 self._current_midi_metadata["time_division"],
-                chord_maps=self.additional_tokens["chord_maps"],
-                specify_root_note=self.additional_tokens["chord_tokens_with_root_note"],
+                chord_maps=self.config.chord_maps,
+                specify_root_note=self.config.chord_tokens_with_root_note,
                 beat_res=self._first_beat_res,
-                unknown_chords_nb_notes_range=self.additional_tokens["chord_unknown"],
+                unknown_chords_nb_notes_range=self.config.chord_unknown,
             )
             unsqueezed = []
             for c in range(len(chords)):
                 chords[c].desc = track.program
                 unsqueezed.append([chords[c]])
             tokens = (
                 unsqueezed + tokens
@@ -369,19 +312,19 @@
         :param _: unused, to match parent method signature
         :param output_path: path to save the file (with its name, e.g. music.mid),
                         leave None to not save the file
         :param time_division: MIDI time division / resolution, in ticks/beat (of the MIDI to create)
         :return: the midi object (miditoolkit.MidiFile)
         """
         assert (
-            time_division % max(self.beat_res.values()) == 0
-        ), f"Invalid time division, please give one divisible by {max(self.beat_res.values())}"
+            time_division % max(self.config.beat_res.values()) == 0
+        ), f"Invalid time division, please give one divisible by {max(self.config.beat_res.values())}"
         midi = MidiFile(ticks_per_beat=time_division)
         midi.tempo_changes.append(TempoChange(TEMPO, 0))
-        ticks_per_sample = time_division // max(self.beat_res.values())
+        ticks_per_sample = time_division // max(self.config.beat_res.values())
 
         tracks = {}
         current_tick = 0
         current_bar = -1
         current_track = 0  # default set to piano
         for time_step in tokens.tokens:
             tok_type, tok_val = time_step[0].split("_")
@@ -466,40 +409,46 @@
         * -1: Duration
 
         :return: the vocabulary as a list of string.
         """
         vocab = [[] for _ in range(3)]
 
         # PITCH & DRUM PITCHES & BAR & POSITIONS & PROGRAM
-        vocab[0] += [f"Pitch_{i}" for i in self.pitch_range]
-        vocab[0] += [f"DrumPitch_{i}" for i in self.drum_pitch_range]
+        vocab[0] += [f"Pitch_{i}" for i in range(*self.config.pitch_range)]
+        vocab[0] += [
+            f"DrumPitch_{i}"
+            for i in range(*self.config.additional_params["drum_pitch_range"])
+        ]
         vocab[0] += ["Bar_None"]  # new bar token
-        nb_positions = max(self.beat_res.values()) * 4  # 4/* time signature
+        nb_positions = max(self.config.beat_res.values()) * 4  # 4/* time signature
         vocab[0] += [f"Position_{i}" for i in range(nb_positions)]
-        vocab[0] += [f"Program_{program}" for program in self.programs]
+        vocab[0] += [f"Program_{program}" for program in self.config.programs]
 
         # BAR POS ENC
-        vocab[1] += [f"BarPosEnc_{i}" for i in range(self.max_bar_embedding)]
+        vocab[1] += [
+            f"BarPosEnc_{i}"
+            for i in range(self.config.additional_params["max_bar_embedding"])
+        ]
 
         # POSITION POS ENC
         vocab[2] += [
             "PositionPosEnc_None"
         ]  # special embedding used with 'Bar_None' tokens
         vocab[2] += [f"PositionPosEnc_{i}" for i in range(nb_positions)]  # pos enc
 
         # CHORD
-        if self.additional_tokens["Chord"]:
+        if self.config.use_chords:
             vocab[0] += self._create_chords_tokens()
 
         # REST
-        if self.additional_tokens["Rest"]:
+        if self.config.use_rests:
             vocab[0] += [f'Rest_{".".join(map(str, rest))}' for rest in self.rests]
 
         # TEMPO
-        if self.additional_tokens["Tempo"]:
+        if self.config.use_tempos:
             vocab.append([f"Tempo_{i}" for i in self.tempos])
 
         # Velocity and Duration in last position
         # VELOCITY
         vocab.append([f"Velocity_{i}" for i in self.velocities])
 
         # DURATION
@@ -521,15 +470,15 @@
 
         dic["Bar"] = ["Bar", "Position"]
         dic["Position"] = ["Program"]
         dic["Program"] = ["Pitch", "DrumPitch"]
         dic["Pitch"] = ["Pitch", "Program", "Bar", "Position"]
         dic["DrumPitch"] = ["DrumPitch", "Program", "Bar", "Position"]
 
-        if self.additional_tokens["Chord"]:
+        if self.config.use_chords:
             dic["Program"] += ["Chord"]
             dic["Chord"] = ["Pitch"]
 
         return dic
 
     @_in_as_seq()
     def tokens_errors(self, tokens: Union[TokSequence, List, np.ndarray, Any]) -> float:
```

### Comparing `miditok-2.0.6/miditok/tokenizations/octuple.py` & `miditok-2.1.0/miditok/tokenizations/octuple.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,17 @@
 from math import ceil
-from pathlib import Path, PurePath
+from pathlib import Path
 from typing import List, Tuple, Dict, Optional, Union, Any
 
 import numpy as np
 from miditoolkit import MidiFile, Instrument, Note, TempoChange, TimeSignature
 
 from ..midi_tokenizer import MIDITokenizer, _in_as_seq, _out_as_complete_seq
 from ..classes import TokSequence, Event
 from ..constants import (
-    PITCH_RANGE,
-    NB_VELOCITIES,
-    BEAT_RES,
-    ADDITIONAL_TOKENS,
-    SPECIAL_TOKENS,
     TIME_DIVISION,
     TIME_SIGNATURE,
     TEMPO,
     MIDI_INSTRUMENTS,
 )
 
 
@@ -40,82 +35,34 @@
     (one per token type). This means that the training requires to add multiple losses.
     For generation, the decoding implies sample from several distributions, which can be
     very delicate. Hence, we do not recommend this tokenization for generation with small models.
 
     **Notes:**
     * Tokens are first sorted by time, then track, then pitch values.
     * Tracks with the same *Program* will be merged.
-
-    :param pitch_range: range of MIDI pitches to use
-    :param beat_res: beat resolutions, as a dictionary:
-            {(beat_x1, beat_x2): beat_res_1, (beat_x2, beat_x3): beat_res_2, ...}
-            The keys are tuples indicating a range of beats, ex 0 to 3 for the first bar, and
-            the values are the resolution to apply to the ranges, in samples per beat, ex 8
-    :param nb_velocities: number of velocity bins
-    :param additional_tokens: additional tokens (chords, time signature, rests, tempo...) to use,
-            to be given as a dictionary. (default: None is used)
-    :param special_tokens: list of special tokens. This must be given as a list of strings given
-            only the names of the tokens. (default: ``["PAD", "BOS", "EOS", "MASK"]``)
-    :param params: path to a tokenizer config file. This will override other arguments and
-            load the tokenizer based on the config file. This is particularly useful if the
-            tokenizer learned Byte Pair Encoding. (default: None)
     """
 
-    def __init__(
-        self,
-        pitch_range: range = PITCH_RANGE,
-        beat_res: Dict[Tuple[int, int], int] = BEAT_RES,
-        nb_velocities: int = NB_VELOCITIES,
-        additional_tokens: Dict[str, bool] = ADDITIONAL_TOKENS,
-        special_tokens: List[str] = SPECIAL_TOKENS,
-        params: Union[str, Path] = None,
-    ):
-        additional_tokens["Chord"] = False  # Incompatible additional token
-        additional_tokens["Rest"] = False
+    def _tweak_config_before_creating_voc(self):
+        self.config.use_chords = False
+        self.config.use_rests = False
+        self.unique_track = True
+
         # used in place of positional encoding
-        self.programs = additional_tokens.get("programs", list(range(-1, 128)))
-        self.max_bar_embedding = 60  # this attribute might increase during encoding
+        # This attribute might increase over tokenizations, if the tokenizer encounter longer MIDIs
+        if "max_bar_embedding" not in self.config.additional_params:
+            self.config.additional_params["max_bar_embedding"] = 60
+
         token_types = ["Pitch", "Velocity", "Duration", "Program", "Position", "Bar"]
-        if additional_tokens["Tempo"]:
+        if self.config.use_tempos:
             token_types.append("Tempo")
-        if additional_tokens["TimeSignature"]:
+        if self.config.use_time_signatures:
             token_types.append("TimeSignature")
         self.vocab_types_idx = {
             type_: idx for idx, type_ in enumerate(token_types)
         }  # used for data augmentation
-        super().__init__(
-            pitch_range,
-            beat_res,
-            nb_velocities,
-            additional_tokens,
-            special_tokens,
-            True,
-            params=params,
-        )
-
-    def save_params(
-        self, out_path: Union[str, Path, PurePath], additional_attributes: Dict = None
-    ):
-        r"""Saves the config / parameters of the tokenizer in a json encoded file.
-        This can be useful to keep track of how a dataset has been tokenized.
-        **Note:** if you override this method, you should probably call it (super()) at the end
-            and use the additional_attributes argument.
-
-        :param out_path: output path to save the file.
-        :param additional_attributes: any additional information to store in the config file.
-                It can be used to override the default attributes saved in the parent method. (default: None)
-        """
-        if additional_attributes is None:
-            additional_attributes = {}
-        additional_attributes_tmp = {
-            "max_bar_embedding": self.max_bar_embedding,
-            "programs": self.programs,
-            **additional_attributes,
-        }
-        super().save_params(out_path, additional_attributes_tmp)
 
     @_out_as_complete_seq
     def _midi_to_tokens(self, midi: MidiFile, *args, **kwargs) -> TokSequence:
         r"""Override the parent class method
         Converts a MIDI file in a token representation, a sequence of "time steps".
         A time step is a list of tokens where:
             (list index: token type)
@@ -151,28 +98,28 @@
             "key_sig_changes": midi.key_signature_changes,
         }
 
         # **************** OVERRIDE FROM HERE, KEEP THE LINES ABOVE IN YOUR METHOD ****************
 
         # Check bar embedding limit, update if needed
         nb_bars = ceil(midi.max_tick / (midi.ticks_per_beat * 4))
-        if self.max_bar_embedding < nb_bars:
-            for i in range(self.max_bar_embedding, nb_bars):
+        if self.config.additional_params["max_bar_embedding"] < nb_bars:
+            for i in range(self.config.additional_params["max_bar_embedding"], nb_bars):
                 self.add_to_vocab(f"Bar_{i}", 5)
-            self.max_bar_embedding = nb_bars
+            self.config.additional_params["max_bar_embedding"] = nb_bars
 
         # Convert each track to tokens
         tokens = []
         for track in midi.instruments:
-            if track.program in self.programs:
+            if track.program in self.config.programs:
                 tokens += self.track_to_tokens(track)
 
         tokens.sort(
             key=lambda x: (x[0].time, x[0].desc, x[0].value)
-        )  # Sort by time then track then pitch
+        )  # Sort by time, then track, then pitch
 
         # Convert pitch events into tokens
         for time_step in tokens:
             time_step[0] = str(time_step[0])
 
         return TokSequence(tokens=tokens)
 
@@ -191,15 +138,15 @@
 
         :param track: track object to convert
         :return: sequence of corresponding tokens
         """
         # Make sure the notes are sorted first by their onset (start) times, second by pitch
         # notes.sort(key=lambda x: (x.start, x.pitch))  # done in midi_to_tokens
         time_division = self.current_midi_metadata["time_division"]
-        ticks_per_sample = time_division / max(self.beat_res.values())
+        ticks_per_sample = time_division / max(self.config.beat_res.values())
         dur_bins = self._durations_ticks[time_division]
 
         tokens = []
         current_tick = -1
         current_bar = -1
         current_pos = -1
         current_tempo_idx = 0
@@ -245,15 +192,15 @@
                 f'Duration_{".".join(map(str, self.durations[dur_index]))}',
                 f"Program_{-1 if track.is_drum else track.program}",
                 f"Position_{current_pos}",
                 f"Bar_{current_bar}",
             ]
 
             # (Tempo)
-            if self.additional_tokens["Tempo"]:
+            if self.config.use_tempos:
                 # If the current tempo is not the last one
                 if current_tempo_idx + 1 < len(
                     self.current_midi_metadata["tempo_changes"]
                 ):
                     # Will loop over incoming tempo changes
                     for tempo_change in self.current_midi_metadata["tempo_changes"][
                         current_tempo_idx + 1 :
@@ -265,15 +212,15 @@
                                 1  # update tempo value (might not change) and index
                             )
                         elif tempo_change.time > note.start:
                             break  # this tempo change is beyond the current time step, we break the loop
                 token.append(f"Tempo_{current_tempo}")
 
             # (TimeSignature)
-            if self.additional_tokens["TimeSignature"]:
+            if self.config.use_time_signatures:
                 # If the current time signature is not the last one
                 if current_time_sig_idx + 1 < len(
                     self.current_midi_metadata["time_sig_changes"]
                 ):
                     # Will loop over incoming time signature changes
                     for time_sig_change in self.current_midi_metadata[
                         "time_sig_changes"
@@ -322,29 +269,29 @@
         :param _: unused, to match parent method signature
         :param output_path: path to save the file (with its name, e.g. music.mid),
                         leave None to not save the file
         :param time_division: MIDI time division / resolution, in ticks/beat (of the MIDI to create)
         :return: the midi object (miditoolkit.MidiFile)
         """
         assert (
-            time_division % max(self.beat_res.values()) == 0
-        ), f"Invalid time division, please give one divisible by {max(self.beat_res.values())}"
+            time_division % max(self.config.beat_res.values()) == 0
+        ), f"Invalid time division, please give one divisible by {max(self.config.beat_res.values())}"
         midi = MidiFile(ticks_per_beat=time_division)
-        ticks_per_sample = time_division // max(self.beat_res.values())
+        ticks_per_sample = time_division // max(self.config.beat_res.values())
         tokens = tokens.tokens
 
         tempo_changes = [TempoChange(TEMPO, 0)]
-        if self.additional_tokens["Tempo"]:
+        if self.config.use_tempos:
             for i in range(len(tokens)):
                 if tokens[i][6].split("_")[1] != "None":
                     tempo_changes = [TempoChange(int(tokens[i][6].split("_")[1]), 0)]
                     break
 
         time_sig = TIME_SIGNATURE
-        if self.additional_tokens["TimeSignature"]:
+        if self.config.use_time_signatures:
             for i in range(len(tokens)):
                 if tokens[i][-1].split("_")[1] != "None":
                     time_sig = self._parse_token_time_signature(
                         tokens[i][-1].split("_")[1]
                     )
                     break
 
@@ -378,22 +325,22 @@
 
             # Append the created note
             tracks[program].append(
                 Note(vel, pitch, current_tick, current_tick + duration)
             )
 
             # Tempo, adds a TempoChange if necessary
-            if self.additional_tokens["Tempo"] and time_step[6].split("_")[1] != "None":
+            if self.config.use_tempos and time_step[6].split("_")[1] != "None":
                 tempo = int(time_step[6].split("_")[1])
                 if tempo != tempo_changes[-1].tempo:
                     tempo_changes.append(TempoChange(tempo, current_tick))
 
             # Time Signature, adds a TimeSignatureChange if necessary
             if (
-                self.additional_tokens["TimeSignature"]
+                self.config.use_time_signatures
                 and time_step[-1].split("_")[1] != "None"
             ):
                 time_sig = self._parse_token_time_signature(time_step[-1].split("_")[1])
                 if time_sig != (
                     time_sig_changes[-1].numerator,
                     time_sig_changes[-1].denominator,
                 ):
@@ -459,42 +406,43 @@
         will be added to the vocabulary by :class:`miditok.MIDITokenizer`.
 
         :return: the vocabulary as a list of string.
         """
         vocab = [[] for _ in range(6)]
 
         # PITCH
-        vocab[0] += [f"Pitch_{i}" for i in self.pitch_range]
+        vocab[0] += [f"Pitch_{i}" for i in range(*self.config.pitch_range)]
 
         # VELOCITY
         vocab[1] += [f"Velocity_{i}" for i in self.velocities]
 
         # DURATION
         vocab[2] += [
             f'Duration_{".".join(map(str, duration))}' for duration in self.durations
         ]
 
         # PROGRAM
-        vocab[3] += [f"Program_{i}" for i in self.programs]
+        vocab[3] += [f"Program_{i}" for i in self.config.programs]
 
         # POSITION
-        nb_positions = max(self.beat_res.values()) * 4  # 4/4 time signature
+        nb_positions = max(self.config.beat_res.values()) * 4  # 4/4 time signature
         vocab[4] += [f"Position_{i}" for i in range(nb_positions)]
 
-        # BAR
+        # BAR (positional encoding)
         vocab[5] += [
-            f"Bar_{i}" for i in range(self.max_bar_embedding)
-        ]  # bar embeddings (positional encoding)
+            f"Bar_{i}"
+            for i in range(self.config.additional_params["max_bar_embedding"])
+        ]
 
         # TEMPO
-        if self.additional_tokens["Tempo"]:
+        if self.config.use_tempos:
             vocab.append([f"Tempo_{i}" for i in self.tempos])
 
         # TIME_SIGNATURE
-        if self.additional_tokens["TimeSignature"]:
+        if self.config.use_time_signatures:
             vocab.append([f"TimeSig_{i[0]}/{i[1]}" for i in self.time_signatures])
 
         return vocab
 
     def _create_token_types_graph(self) -> Dict[str, List[str]]:
         r"""Returns a graph (as a dictionary) of the possible token
         types successions.
@@ -515,15 +463,15 @@
             - a pitch token should not be present if the same pitch is already played at the current position
 
         :param tokens: sequence of tokens to check
         :return: the error ratio (lower is better)
         """
         err = 0
         current_bar = current_pos = -1
-        current_pitches = {p: [] for p in self.programs}
+        current_pitches = {p: [] for p in self.config.programs}
 
         for token in tokens.tokens:
             if any(tok.split("_")[1] == "None" for tok in token):
                 err += 1
                 continue
             has_error = False
             bar_value = int(token[5].split("_")[1])
@@ -533,22 +481,22 @@
 
             # Bar
             if bar_value < current_bar:
                 has_error = True
             elif bar_value > current_bar:
                 current_bar = bar_value
                 current_pos = -1
-                current_pitches = {p: [] for p in self.programs}
+                current_pitches = {p: [] for p in self.config.programs}
 
             # Position
             if pos_value < current_pos:
                 has_error = True
             elif pos_value > current_pos:
                 current_pos = pos_value
-                current_pitches = {p: [] for p in self.programs}
+                current_pitches = {p: [] for p in self.config.programs}
 
             # Pitch
             if pitch_value in current_pitches[program_value]:
                 has_error = True
             else:
                 current_pitches[program_value].append(pitch_value)
```

### Comparing `miditok-2.0.6/miditok/tokenizations/octuple_mono.py` & `miditok-2.1.0/miditok/tokenizations/octuple_mono.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,16 @@
 from math import ceil
-from pathlib import Path, PurePath
 from typing import List, Tuple, Dict, Optional, Union, Any
 
 import numpy as np
 from miditoolkit import Instrument, Note, TempoChange
 
 from ..midi_tokenizer import MIDITokenizer, _in_as_seq, _out_as_complete_seq
 from ..classes import TokSequence
 from ..constants import (
-    PITCH_RANGE,
-    NB_VELOCITIES,
-    BEAT_RES,
-    ADDITIONAL_TOKENS,
-    SPECIAL_TOKENS,
     TIME_DIVISION,
     TEMPO,
     MIDI_INSTRUMENTS,
 )
 
 
 class OctupleMono(MIDITokenizer):
@@ -27,78 +21,34 @@
     * 0: Pitch
     * 1: Velocity
     * 2: Duration
     * 3: Position
     * 4: Bar
     * (+ Optional) Tempo
     * (+ Optional) TimeSignature
-
-    :param pitch_range: range of MIDI pitches to use
-    :param beat_res: beat resolutions, as a dictionary:
-            {(beat_x1, beat_x2): beat_res_1, (beat_x2, beat_x3): beat_res_2, ...}
-            The keys are tuples indicating a range of beats, ex 0 to 3 for the first bar, and
-            the values are the resolution to apply to the ranges, in samples per beat, ex 8
-    :param nb_velocities: number of velocity bins
-    :param additional_tokens: additional tokens (chords, time signature, rests, tempo...) to use,
-            to be given as a dictionary. (default: None is used)
-    :param special_tokens: list of special tokens. This must be given as a list of strings given
-            only the names of the tokens. (default: ``["PAD", "BOS", "EOS", "MASK"]``)
-    :param params: path to a tokenizer config file. This will override other arguments and
-            load the tokenizer based on the config file. This is particularly useful if the
-            tokenizer learned Byte Pair Encoding. (default: None)
     """
 
-    def __init__(
-        self,
-        pitch_range: range = PITCH_RANGE,
-        beat_res: Dict[Tuple[int, int], int] = BEAT_RES,
-        nb_velocities: int = NB_VELOCITIES,
-        additional_tokens: Dict[str, bool] = ADDITIONAL_TOKENS,
-        special_tokens: List[str] = SPECIAL_TOKENS,
-        params: Union[str, Path] = None,
-    ):
-        additional_tokens["Chord"] = False  # Incompatible additional token
-        additional_tokens["Rest"] = False
-        additional_tokens["Program"] = False
+    def _tweak_config_before_creating_voc(self):
+        self.config.use_chords = False
+        self.config.use_rests = False
+        self.config.use_programs = False
+
         # used in place of positional encoding
-        self.max_bar_embedding = 60  # this attribute might increase during encoding
+        # This attribute might increase over tokenizations, if the tokenizer encounter longer MIDIs
+        if "max_bar_embedding" not in self.config.additional_params:
+            self.config.additional_params["max_bar_embedding"] = 60
+
         token_types = ["Pitch", "Velocity", "Duration", "Position", "Bar"]
-        if additional_tokens["Tempo"]:
+        if self.config.use_tempos:
             token_types.append("Tempo")
-        if additional_tokens["TimeSignature"]:
+        if self.config.use_time_signatures:
             token_types.append("TimeSignature")
         self.vocab_types_idx = {
             type_: idx for idx, type_ in enumerate(token_types)
         }  # used for data augmentation
-        super().__init__(
-            pitch_range,
-            beat_res,
-            nb_velocities,
-            additional_tokens,
-            special_tokens,
-            params=params,
-        )
-
-    def save_params(
-        self, out_path: Union[str, Path, PurePath], additional_attributes: Dict = None
-    ):
-        r"""Saves the config / parameters of the tokenizer in a json encoded file.
-        This can be useful to keep track of how a dataset has been tokenized.
-
-        :param out_path: output path to save the file.
-        :param additional_attributes: any additional information to store in the config file.
-                It can be used to override the default attributes saved in the parent method. (default: None)
-        """
-        if additional_attributes is None:
-            additional_attributes = {}
-        additional_attributes_tmp = {
-            "max_bar_embedding": self.max_bar_embedding,
-            **additional_attributes,
-        }
-        super().save_params(out_path, additional_attributes_tmp)
 
     @_out_as_complete_seq
     def track_to_tokens(self, track: Instrument) -> TokSequence:
         r"""Converts a track (miditoolkit.Instrument object) into a sequence of tokens (:class:`miditok.TokSequence`).
         A time step is a list of tokens where:
             (list index: token type)
             0: Pitch
@@ -110,28 +60,28 @@
 
         :param track: MIDI track to convert
         :return: :class:`miditok.TokSequence` of corresponding tokens.
         """
         # Make sure the notes are sorted first by their onset (start) times, second by pitch
         # notes.sort(key=lambda x: (x.start, x.pitch))  # done in midi_to_tokens
         ticks_per_sample = self._current_midi_metadata["time_division"] / max(
-            self.beat_res.values()
+            self.config.beat_res.values()
         )
         ticks_per_bar = self._current_midi_metadata["time_division"] * 4
         dur_bins = self._durations_ticks[self._current_midi_metadata["time_division"]]
 
         # Check bar embedding limit, update if needed
         nb_bars = ceil(
             max(note.end for note in track.notes)
             / (self._current_midi_metadata["time_division"] * 4)
         )
-        if self.max_bar_embedding < nb_bars:
-            for i in range(self.max_bar_embedding, nb_bars):
+        if self.config.additional_params["max_bar_embedding"] < nb_bars:
+            for i in range(self.config.additional_params["max_bar_embedding"], nb_bars):
                 self.add_to_vocab(f"Bar_{i}", 4)
-            self.max_bar_embedding = nb_bars
+            self.config.additional_params["max_bar_embedding"] = nb_bars
 
         tokens = []
         current_tick = -1
         current_bar = -1
         current_pos = -1
         current_tempo_idx = 0
         current_tempo = self._current_midi_metadata["tempo_changes"][
@@ -153,15 +103,15 @@
                 f"Velocity_{note.velocity}",
                 f'Duration_{".".join(map(str, self.durations[dur_index]))}',
                 f"Position_{current_pos}",
                 f"Bar_{current_bar}",
             ]
 
             # (Tempo)
-            if self.additional_tokens["Tempo"]:
+            if self.config.use_tempos:
                 # If the current tempo is not the last one
                 if current_tempo_idx + 1 < len(
                     self._current_midi_metadata["tempo_changes"]
                 ):
                     # Will loop over incoming tempo changes
                     for tempo_change in self._current_midi_metadata["tempo_changes"][
                         current_tempo_idx + 1 :
@@ -201,24 +151,24 @@
         :param tokens: sequence of tokens to convert. Can be either a Tensor (PyTorch and Tensorflow are supported),
                 a numpy array, a Python list or a TokSequence.
         :param time_division: MIDI time division / resolution, in ticks/beat (of the MIDI to create)
         :param program: the MIDI program of the produced track and if it drum, (default (0, False), piano)
         :return: the miditoolkit instrument object and tempo changes
         """
         assert (
-            time_division % max(self.beat_res.values()) == 0
-        ), f"Invalid time division, please give one divisible by {max(self.beat_res.values())}"
+            time_division % max(self.config.beat_res.values()) == 0
+        ), f"Invalid time division, please give one divisible by {max(self.config.beat_res.values())}"
         tokens = tokens.tokens
 
-        ticks_per_sample = time_division // max(self.beat_res.values())
+        ticks_per_sample = time_division // max(self.config.beat_res.values())
         name = "Drums" if program[1] else MIDI_INSTRUMENTS[program[0]]["name"]
         instrument = Instrument(program[0], is_drum=program[1], name=name)
 
         tempo_changes = [TempoChange(TEMPO, 0)]
-        if self.additional_tokens["Tempo"]:
+        if self.config.use_tempos:
             for i in range(len(tokens)):
                 if tokens[i][-1].split("_")[1] != "None":
                     tempo_changes = [TempoChange(int(tokens[i][-1].split("_")[1]), 0)]
                     break
 
         for time_step in tokens:
             if any(tok.split("_")[1] == "None" for tok in time_step[:6]):
@@ -240,18 +190,15 @@
 
             # Append the created note
             instrument.notes.append(
                 Note(vel, pitch, current_tick, current_tick + duration)
             )
 
             # Tempo, adds a TempoChange if necessary
-            if (
-                self.additional_tokens["Tempo"]
-                and time_step[-1].split("_")[1] != "None"
-            ):
+            if self.config.use_tempos and time_step[-1].split("_")[1] != "None":
                 tempo = int(time_step[-1].split("_")[1])
                 if tempo != tempo_changes[-1].tempo:
                     tempo_changes.append(TempoChange(tempo, current_tick))
 
         return instrument, tempo_changes
 
     def _create_base_vocabulary(self, sos_eos_tokens: bool = None) -> List[List[str]]:
@@ -264,35 +211,36 @@
         will be added to the vocabulary by :class:`miditok.MIDITokenizer`.
 
         :return: the vocabulary as a list of string.
         """
         vocab = [[] for _ in range(5)]
 
         # PITCH
-        vocab[0] += [f"Pitch_{i}" for i in self.pitch_range]
+        vocab[0] += [f"Pitch_{i}" for i in range(*self.config.pitch_range)]
 
         # VELOCITY
         vocab[1] += [f"Velocity_{i}" for i in self.velocities]
 
         # DURATION
         vocab[2] += [
             f'Duration_{".".join(map(str, duration))}' for duration in self.durations
         ]
 
         # POSITION
-        nb_positions = max(self.beat_res.values()) * 4  # 4/4 time signature
+        nb_positions = max(self.config.beat_res.values()) * 4  # 4/4 time signature
         vocab[3] += [f"Position_{i}" for i in range(nb_positions)]
 
         # BAR
         vocab[4] += [
-            f"Bar_{i}" for i in range(self.max_bar_embedding)
+            f"Bar_{i}"
+            for i in range(self.config.additional_params["max_bar_embedding"])
         ]  # bar embeddings (positional encoding)
 
         # TEMPO
-        if self.additional_tokens["Tempo"]:
+        if self.config.use_tempos:
             vocab.append([f"Tempo_{i}" for i in self.tempos])
 
         return vocab
 
     def _create_token_types_graph(self) -> Dict[str, List[str]]:
         r"""Returns a graph (as a dictionary) of the possible token
         types successions.
```

### Comparing `miditok-2.0.6/miditok/tokenizations/remi.py` & `miditok-2.1.0/miditok/tokenizations/tsd.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,430 +1,507 @@
 from typing import List, Tuple, Dict, Optional, Union, Any
 from pathlib import Path
 
 import numpy as np
-from miditoolkit import Instrument, Note, TempoChange
+from miditoolkit import MidiFile, Instrument, Note, TempoChange, TimeSignature
 
-from ..midi_tokenizer import MIDITokenizer, _in_as_seq, _out_as_complete_seq
+from ..midi_tokenizer import MIDITokenizer, _in_as_seq
 from ..classes import TokSequence, Event
 from ..utils import detect_chords
 from ..constants import (
-    PITCH_RANGE,
-    NB_VELOCITIES,
-    BEAT_RES,
-    ADDITIONAL_TOKENS,
-    SPECIAL_TOKENS,
     TIME_DIVISION,
     TEMPO,
     MIDI_INSTRUMENTS,
+    TIME_SIGNATURE,
 )
 
 
-class REMI(MIDITokenizer):
-    r"""REMI, standing for Revamped MIDI and introduced with the
-    `Pop Music Transformer (Huang and Yang) <https://dl.acm.org/doi/10.1145/3394171.3413671>`_,
-    is a tokenization that represents notes as successions of *Pitch*, *Velocity* and *Duration*
-    tokens, and time with *Bar* and *Position* tokens. A *Bar* token indicate that a new bar
-    is beginning, and *Position* the current position within the current bar. The number of
-    positions is determined by the ``beat_res`` argument, the maximum value will be used as
-    resolution.
-    **NOTE:** in the original paper, the tempo information is represented as the succession
-    of two token types: a *TempoClass* indicating if the tempo is fast or slow, and a
-    *TempoValue* indicating its value. MidiTok only uses one *Tempo* token for its value
-    (see :ref:`Additional tokens`).
-
-    :param pitch_range: range of MIDI pitches to use
-    :param beat_res: beat resolutions, as a dictionary:
-            {(beat_x1, beat_x2): beat_res_1, (beat_x2, beat_x3): beat_res_2, ...}
-            The keys are tuples indicating a range of beats, ex 0 to 3 for the first bar, and
-            the values are the resolution to apply to the ranges, in samples per beat, ex 8
-    :param nb_velocities: number of velocity bins
-    :param additional_tokens: additional tokens (chords, time signature, rests, tempo...) to use,
-            to be given as a dictionary. (default: None is used)
-    :param special_tokens: list of special tokens. This must be given as a list of strings given
-            only the names of the tokens. (default: ``["PAD", "BOS", "EOS", "MASK"]``)
-    :param params: path to a tokenizer config file. This will override other arguments and
-            load the tokenizer based on the config file. This is particularly useful if the
-            tokenizer learned Byte Pair Encoding. (default: None)
+class TSD(MIDITokenizer):
+    r"""TSD, for Time Shift Duration, is similar to MIDI-Like :ref:`MIDI-Like`
+    but uses explicit *Duration* tokens to represent note durations, which have
+    showed `better results than with NoteOff tokens <https://arxiv.org/abs/2002.00212>`_.
+    **Note:** as TSD uses *TimeShifts* events to move the time from note to
+    note, it could be unsuited for tracks with long pauses. In such case, the
+    maximum *TimeShift* value will be used.
     """
 
-    def __init__(
-        self,
-        pitch_range: range = PITCH_RANGE,
-        beat_res: Dict[Tuple[int, int], int] = BEAT_RES,
-        nb_velocities: int = NB_VELOCITIES,
-        additional_tokens: Dict[str, Union[bool, int]] = ADDITIONAL_TOKENS,
-        special_tokens: List[str] = SPECIAL_TOKENS,
-        params: Union[str, Path] = None,
-    ):
-        self.encoder = []
-        additional_tokens["TimeSignature"] = False  # not compatible
-        super().__init__(
-            pitch_range,
-            beat_res,
-            nb_velocities,
-            additional_tokens,
-            special_tokens,
-            params=params,
-        )
+    def _tweak_config_before_creating_voc(self):
+        self.config.use_time_signatures = False
+        if self.config.use_programs:
+            self.unique_track = True
 
-    @_out_as_complete_seq
-    def track_to_tokens(self, track: Instrument) -> TokSequence:
-        r"""Converts a track (miditoolkit.Instrument object) into a sequence of tokens (:class:`miditok.TokSequence`).
+    def __notes_to_events(self, track: Instrument) -> List[Event]:
+        r"""Converts notes of a track (``miditoolkit.Instrument``) into a sequence of `Event` objects.
 
         :param track: MIDI track to convert
-        :return: :class:`miditok.TokSequence` of corresponding tokens.
+        :return: sequence of corresponding Events
         """
         # Make sure the notes are sorted first by their onset (start) times, second by pitch
         # notes.sort(key=lambda x: (x.start, x.pitch))  # done in midi_to_tokens
+        dur_bins = self._durations_ticks[self._current_midi_metadata["time_division"]]
+        program = track.program if not track.is_drum else -1
+        events = []
+
+        # Add chords
+        if self.config.use_chords and not track.is_drum:
+            chords = detect_chords(
+                track.notes,
+                self._current_midi_metadata["time_division"],
+                chord_maps=self.config.chord_maps,
+                specify_root_note=self.config.chord_tokens_with_root_note,
+                beat_res=self._first_beat_res,
+                unknown_chords_nb_notes_range=self.config.chord_unknown,
+            )
+            for chord in chords:
+                if self.config.use_programs:
+                    events.append(
+                        Event("Program", track.program, chord.time, "ProgramChord")
+                    )
+                events.append(chord)
+
+        # Creates the Note On, Note Off and Velocity events
+        for n, note in enumerate(track.notes):
+            # Note On / Velocity / Duration
+            if self.config.use_programs:
+                events.append(
+                    Event(type="Program", value=program, time=note.start, desc=note.end)
+                )
+            events.append(
+                Event(type="Pitch", value=note.pitch, time=note.start, desc=note.end)
+            )
+            events.append(
+                Event(
+                    type="Velocity",
+                    value=note.velocity,
+                    time=note.start,
+                    desc=f"{note.velocity}",
+                )
+            )
+            duration = note.end - note.start
+            index = np.argmin(np.abs(dur_bins - duration))
+            events.append(
+                Event(
+                    type="Duration",
+                    value=".".join(map(str, self.durations[index])),
+                    time=note.start,
+                    desc=f"{duration} ticks",
+                )
+            )
+
+        return events
+
+    def __add_time_note_events(self, events: List[Event]) -> List[Event]:
+        r"""
+        Takes a sequence of note events (containing optionally Chord, Tempo and TimeSignature tokens),
+        and insert (not inplace) time tokens (TimeShift, Rest) to complete the sequence.
+
+        :param events: note events to complete.
+        :return: the same events, with time events inserted.
+        """
+        dur_bins = self._durations_ticks[self._current_midi_metadata["time_division"]]
         ticks_per_sample = self._current_midi_metadata["time_division"] / max(
-            self.beat_res.values()
+            self.config.beat_res.values()
         )
-        ticks_per_bar = self._current_midi_metadata["time_division"] * 4
-        dur_bins = self._durations_ticks[self._current_midi_metadata["time_division"]]
         min_rest = (
             self._current_midi_metadata["time_division"] * self.rests[0][0]
             + ticks_per_sample * self.rests[0][1]
-            if self.additional_tokens["Rest"]
+            if self.config.use_rests
             else 0
         )
 
-        events = []
-
-        # Creates events
-        previous_tick = -1
-        previous_note_end = (
-            track.notes[0].start + 1
-        )  # so that no rest is created before the first note
-        current_bar = -1
-        current_tempo_idx = 0
-        current_tempo = self._current_midi_metadata["tempo_changes"][
-            current_tempo_idx
-        ].tempo
-        for note in track.notes:
-            if note.start != previous_tick:
+        # Add time events
+        all_events = events.copy()
+        previous_tick = 0
+        previous_note_end = events[0].time + 1
+        for e, event in enumerate(events.copy()):
+            # No time shift
+            if event.time != previous_tick:
                 # (Rest)
                 if (
-                    self.additional_tokens["Rest"]
-                    and note.start > previous_note_end
-                    and note.start - previous_note_end >= min_rest
+                    event.type in ["Pitch", "Tempo", "TimeSig"]
+                    and self.config.use_rests
+                    and event.time - previous_note_end >= min_rest
                 ):
-                    previous_tick = previous_note_end
+                    # untouched tick value to the order is not messed after sorting
+                    # in case of tempo change, we need to take its time as reference
+                    rest_tick = max(previous_note_end, previous_tick)
                     rest_beat, rest_pos = divmod(
-                        note.start - previous_tick,
+                        event.time - rest_tick,
                         self._current_midi_metadata["time_division"],
                     )
                     rest_beat = min(rest_beat, max([r[0] for r in self.rests]))
                     rest_pos = round(rest_pos / ticks_per_sample)
+                    previous_tick = rest_tick
 
                     if rest_beat > 0:
-                        events.append(
+                        all_events.append(
                             Event(
                                 type="Rest",
                                 value=f"{rest_beat}.0",
-                                time=previous_note_end,
+                                time=rest_tick,
                                 desc=f"{rest_beat}.0",
                             )
                         )
                         previous_tick += (
                             rest_beat * self._current_midi_metadata["time_division"]
                         )
 
                     while rest_pos >= self.rests[0][1]:
                         rest_pos_temp = min(
                             [r[1] for r in self.rests], key=lambda x: abs(x - rest_pos)
                         )
-                        events.append(
+                        all_events.append(
                             Event(
                                 type="Rest",
                                 value=f"0.{rest_pos_temp}",
-                                time=previous_note_end,
+                                time=rest_tick,
                                 desc=f"0.{rest_pos_temp}",
                             )
                         )
                         previous_tick += round(rest_pos_temp * ticks_per_sample)
                         rest_pos -= rest_pos_temp
 
-                    current_bar = previous_tick // ticks_per_bar
-
-                # Bar
-                nb_new_bars = note.start // ticks_per_bar - current_bar
-                for i in range(nb_new_bars):
-                    events.append(
-                        Event(
-                            type="Bar",
-                            value="None",
-                            time=(current_bar + i + 1) * ticks_per_bar,
-                            desc=0,
+                    # Adds an additional time shift if needed
+                    if rest_pos > 0:
+                        time_shift = round(rest_pos * ticks_per_sample)
+                        index = np.argmin(np.abs(dur_bins - time_shift))
+                        all_events.append(
+                            Event(
+                                type="TimeShift",
+                                value=".".join(map(str, self.durations[index])),
+                                time=previous_tick,
+                                desc=f"{time_shift} ticks",
+                            )
                         )
-                    )
-                current_bar += nb_new_bars
-
-                # Position
-                pos_index = int((note.start % ticks_per_bar) / ticks_per_sample)
-                events.append(
-                    Event(
-                        type="Position",
-                        value=pos_index,
-                        time=note.start,
-                        desc=note.start,
-                    )
-                )
 
-                # (Tempo)
-                if self.additional_tokens["Tempo"]:
-                    # If the current tempo is not the last one
-                    if current_tempo_idx + 1 < len(
-                        self._current_midi_metadata["tempo_changes"]
-                    ):
-                        # Will loop over incoming tempo changes
-                        for tempo_change in self._current_midi_metadata[
-                            "tempo_changes"
-                        ][current_tempo_idx + 1 :]:
-                            # If this tempo change happened before the current moment
-                            if tempo_change.time <= note.start:
-                                current_tempo = tempo_change.tempo
-                                current_tempo_idx += (
-                                    1  # update tempo value (might not change) and index
-                                )
-                            else:  # <==> elif tempo_change.time > previous_tick:
-                                break  # this tempo change is beyond the current time step, we break the loop
-                    events.append(
+                # Time shift
+                else:
+                    time_shift = event.time - previous_tick
+                    index = np.argmin(np.abs(dur_bins - time_shift))
+                    all_events.append(
                         Event(
-                            type="Tempo",
-                            value=current_tempo,
-                            time=note.start,
-                            desc=note.start,
+                            type="TimeShift",
+                            value=".".join(map(str, self.durations[index])),
+                            time=previous_tick,
+                            desc=f"{time_shift} ticks",
                         )
                     )
+                previous_tick = event.time
 
-                previous_tick = note.start
+            # Update max offset time of the notes encountered
+            if event.type == "Pitch":
+                previous_note_end = max(previous_note_end, event.desc)
+
+        # Sort the tokens so that they come in the good order
+        all_events.sort(key=lambda x: (x.time, self._order(x)))
+        return all_events
+
+    def _midi_to_tokens(
+        self, midi: MidiFile, *args, **kwargs
+    ) -> Union[TokSequence, List[TokSequence]]:
+        r"""Converts a preprocessed MIDI object to a sequence of tokens.
+
+        :param midi: the MIDI objet to convert.
+        :return: a :class:`miditok.TokSequence` if `tokenizer.unique_track` is true, else a list of
+                :class:`miditok.TokSequence` objects.
+        """
+        # Convert each track to tokens
+        all_events = []
 
-            # Pitch / Velocity / Duration
-            events.append(
-                Event(type="Pitch", value=note.pitch, time=note.start, desc=note.pitch)
-            )
-            events.append(
-                Event(
-                    type="Velocity",
-                    value=note.velocity,
-                    time=note.start,
-                    desc=f"{note.velocity}",
-                )
-            )
-            duration = note.end - note.start
-            index = np.argmin(np.abs(dur_bins - duration))
-            events.append(
-                Event(
-                    type="Duration",
-                    value=".".join(map(str, self.durations[index])),
-                    time=note.start,
-                    desc=f"{duration} ticks",
+        # Adds note tokens
+        for track in midi.instruments:
+            note_events = self.__notes_to_events(track)
+            if self.unique_track:
+                all_events += note_events
+            else:
+                all_events.append(note_events)
+        # Adds tempo events if specified
+        if self.config.use_tempos:
+            tempo_events = []
+            for tempo_change in self._current_midi_metadata["tempo_changes"]:
+                tempo_events.append(
+                    Event(
+                        type="Tempo",
+                        value=tempo_change.tempo,
+                        time=tempo_change.time,
+                        desc=tempo_change.tempo,
+                    )
                 )
-            )
-
-            previous_note_end = max(previous_note_end, note.end)
-
-        # Adds chord events if specified
-        if self.additional_tokens["Chord"] and not track.is_drum:
-            events += detect_chords(
-                track.notes,
-                self._current_midi_metadata["time_division"],
-                chord_maps=self.additional_tokens["chord_maps"],
-                specify_root_note=self.additional_tokens["chord_tokens_with_root_note"],
-                beat_res=self._first_beat_res,
-                unknown_chords_nb_notes_range=self.additional_tokens["chord_unknown"],
-            )
+            if self.unique_track:
+                all_events += tempo_events
+            else:
+                for i in range(len(all_events)):
+                    all_events[i] += tempo_events
+
+        # Add time events
+        if self.unique_track:
+            all_events.sort(key=lambda x: x.time)
+            all_events = self.__add_time_note_events(all_events)
+            tok_sequence = TokSequence(events=all_events)
+            self.complete_sequence(tok_sequence)
+        else:
+            tok_sequence = []
+            for i in range(len(all_events)):
+                all_events[i].sort(key=lambda x: x.time)
+                all_events[i] = self.__add_time_note_events(all_events[i])
+                tok_sequence.append(TokSequence(events=all_events[i]))
+                self.complete_sequence(tok_sequence[-1])
 
-        events.sort(key=lambda x: (x.time, self._order(x)))
+        return tok_sequence
 
-        return TokSequence(events=events)
-
-    @_in_as_seq()
     def tokens_to_track(
         self,
         tokens: Union[TokSequence, List, np.ndarray, Any],
         time_division: Optional[int] = TIME_DIVISION,
         program: Optional[Tuple[int, bool]] = (0, False),
     ) -> Tuple[Instrument, List[TempoChange]]:
-        r"""Converts a sequence of tokens into a track object
+        pass
+
+    def track_to_tokens(self, track: Instrument) -> TokSequence:
+        pass
 
-        :param tokens: sequence of tokens to convert. Can be either a Tensor (PyTorch and Tensorflow are supported),
-                a numpy array, a Python list or a TokSequence.
-        :param time_division: MIDI time division / resolution, in ticks/beat (of the MIDI to create)
-        :param program: the MIDI program of the produced track and if it drum, (default (0, False), piano)
-        :return: the miditoolkit instrument object and tempo changes
+    @_in_as_seq()
+    def tokens_to_midi(
+        self,
+        tokens: Union[
+            Union[TokSequence, List, np.ndarray, Any],
+            List[Union[TokSequence, List, np.ndarray, Any]],
+        ],
+        _=None,
+        output_path: Optional[str] = None,
+        time_division: int = TIME_DIVISION,
+    ) -> MidiFile:
+        r"""Converts tokens (:class:`miditok.TokSequence`) into a MIDI and saves it.
+
+        :param tokens: tokens to convert. Can be either a list of :class:`miditok.TokSequence`,
+        :param _: unused, to match parent method signature
+        :param output_path: path to save the file. (default: None)
+        :param time_division: MIDI time division / resolution, in ticks/beat (of the MIDI to create).
+        :return: the midi object (:class:`miditoolkit.MidiFile`).
         """
+        # Unsqueeze tokens in case of unique_track
+        if self.unique_track:  # ie single token seq
+            tokens = [tokens]
+        for i in range(len(tokens)):
+            tokens[i] = tokens[i].tokens
+        midi = MidiFile(ticks_per_beat=time_division)
         assert (
-            time_division % max(self.beat_res.values()) == 0
-        ), f"Invalid time division, please give one divisible by {max(self.beat_res.values())}"
-        tokens = tokens.tokens
-
-        ticks_per_sample = time_division // max(self.beat_res.values())
-        ticks_per_bar = time_division * 4
-        name = "Drums" if program[1] else MIDI_INSTRUMENTS[program[0]]["name"]
-        instrument = Instrument(program[0], is_drum=program[1], name=name)
-        tempo_changes = [
-            TempoChange(TEMPO, -1)
-        ]  # mock the first tempo change to optimize below
+            time_division % max(self.config.beat_res.values()) == 0
+        ), f"Invalid time division, please give one divisible by {max(self.config.beat_res.values())}"
+        ticks_per_sample = time_division // max(self.config.beat_res.values())
+
+        # RESULTS
+        instruments: Dict[int, Instrument] = {}
+        tempo_changes = [TempoChange(TEMPO, -1)]
+        time_signature_changes = [TimeSignature(*TIME_SIGNATURE, 0)]
 
         current_tick = 0
-        current_bar = -1
+        current_program = 0
         previous_note_end = 0
-        for ti, token in enumerate(tokens):
-            if token.split("_")[0] == "Bar":
-                current_bar += 1
-                current_tick = current_bar * ticks_per_bar
-            elif token.split("_")[0] == "Rest":
-                beat, pos = map(int, tokens[ti].split("_")[1].split("."))
-                if (
-                    current_tick < previous_note_end
-                ):  # if in case successive rest happen
-                    current_tick = previous_note_end
-                current_tick += beat * time_division + pos * ticks_per_sample
-                current_bar = current_tick // ticks_per_bar
-            elif token.split("_")[0] == "Position":
-                if current_bar == -1:
-                    current_bar = (
-                        0  # as this Position token occurs before any Bar token
+        for seq in tokens:
+            for ti, token in enumerate(seq):
+                if token.split("_")[0] == "TimeShift":
+                    current_tick += self._token_duration_to_ticks(
+                        token.split("_")[1], time_division
                     )
-                current_tick = (
-                    current_bar * ticks_per_bar
-                    + int(token.split("_")[1]) * ticks_per_sample
-                )
-            elif token.split("_")[0] == "Tempo":
-                # If your encoding include tempo tokens, each Position token should be followed by
-                # a tempo token, but if it is not the case this method will skip this step
-                tempo = int(token.split("_")[1])
-                if tempo != tempo_changes[-1].tempo:
-                    tempo_changes.append(TempoChange(tempo, current_tick))
-            elif token.split("_")[0] == "Pitch":
-                try:
+                elif token.split("_")[0] == "Rest":
+                    beat, pos = map(int, seq[ti].split("_")[1].split("."))
                     if (
-                        tokens[ti + 1].split("_")[0] == "Velocity"
-                        and tokens[ti + 2].split("_")[0] == "Duration"
+                        current_tick < previous_note_end
+                    ):  # if in case successive rest happen
+                        current_tick = previous_note_end
+                    current_tick += beat * time_division + pos * ticks_per_sample
+                elif token.split("_")[0] == "Pitch":
+                    try:
+                        if (
+                            seq[ti + 1].split("_")[0] == "Velocity"
+                            and seq[ti + 2].split("_")[0] == "Duration"
+                        ):
+                            pitch = int(seq[ti].split("_")[1])
+                            vel = int(seq[ti + 1].split("_")[1])
+                            duration = self._token_duration_to_ticks(
+                                seq[ti + 2].split("_")[1], time_division
+                            )
+                            if current_program not in instruments.keys():
+                                instruments[current_program] = Instrument(
+                                    program=0
+                                    if current_program == -1
+                                    else current_program,
+                                    is_drum=current_program == -1,
+                                    name="Drums"
+                                    if current_program == -1
+                                    else MIDI_INSTRUMENTS[current_program]["name"],
+                                )
+                            instruments[current_program].notes.append(
+                                Note(vel, pitch, current_tick, current_tick + duration)
+                            )
+                            previous_note_end = max(
+                                previous_note_end, current_tick + duration
+                            )
+                    except (
+                        IndexError
+                    ):  # A well constituted sequence should not raise an exception
+                        pass  # However with generated sequences this can happen, or if the sequence isn't finished
+                elif token.split("_")[0] == "Program":
+                    current_program = int(token.split("_")[1])
+                elif token.split("_")[0] == "Tempo":
+                    # If your encoding include tempo tokens, each Position token should be followed by
+                    # a tempo token, but if it is not the case this method will skip this step
+                    tempo = int(token.split("_")[1])
+                    if tempo != tempo_changes[-1].tempo:
+                        tempo_changes.append(TempoChange(tempo, current_tick))
+                elif token.split("_")[0] == "TimeSig":
+                    num, den = self._parse_token_time_signature(token.split("_")[1])
+                    current_time_signature = time_signature_changes[-1]
+                    if (
+                        num != current_time_signature.numerator
+                        and den != current_time_signature.denominator
                     ):
-                        pitch = int(tokens[ti].split("_")[1])
-                        vel = int(tokens[ti + 1].split("_")[1])
-                        duration = self._token_duration_to_ticks(
-                            tokens[ti + 2].split("_")[1], time_division
-                        )
-                        instrument.notes.append(
-                            Note(vel, pitch, current_tick, current_tick + duration)
+                        time_signature_changes.append(
+                            TimeSignature(num, den, current_tick)
                         )
-                        previous_note_end = max(
-                            previous_note_end, current_tick + duration
-                        )
-                except (
-                    IndexError
-                ):  # A well constituted sequence should not raise an exception
-                    pass  # However with generated sequences this can happen, or if the sequence isn't finished
-
         if len(tempo_changes) > 1:
             del tempo_changes[0]  # delete mocked tempo change
         tempo_changes[0].time = 0
-        return instrument, tempo_changes
+        if len(time_signature_changes) > 1:
+            del time_signature_changes[0]  # delete mocked time signature change
+        time_signature_changes[0].time = 0
+
+        # create MidiFile
+        midi.instruments = list(instruments.values())
+        midi.tempo_changes = tempo_changes
+        midi.time_signature_changes = time_signature_changes
+        midi.max_tick = max(
+            [
+                max([note.end for note in track.notes]) if len(track.notes) > 0 else 0
+                for track in midi.instruments
+            ]
+        )
+        # Write MIDI file
+        if output_path:
+            Path(output_path).mkdir(parents=True, exist_ok=True)
+            midi.dump(output_path)
+        return midi
 
-    def _create_base_vocabulary(self, sos_eos_tokens: bool = None) -> List[str]:
+    def _create_base_vocabulary(self, sos_eos_tokens: bool = False) -> List[str]:
         r"""Creates the vocabulary, as a list of string tokens.
         Each token as to be given as the form of "Type_Value", separated with an underscore.
         Example: Pitch_58
         The :class:`miditok.MIDITokenizer` main class will then create the "real" vocabulary as
         a dictionary.
         Special tokens have to be given when creating the tokenizer, and
         will be added to the vocabulary by :class:`miditok.MIDITokenizer`.
 
         :return: the vocabulary as a list of string.
         """
-        vocab = ["Bar_None"]
+        vocab = []
 
-        # PITCH
-        vocab += [f"Pitch_{i}" for i in self.pitch_range]
+        # NOTE ON
+        vocab += [f"Pitch_{i}" for i in range(*self.config.pitch_range)]
 
         # VELOCITY
         vocab += [f"Velocity_{i}" for i in self.velocities]
 
         # DURATION
         vocab += [
             f'Duration_{".".join(map(str, duration))}' for duration in self.durations
         ]
 
-        # POSITION
-        nb_positions = max(self.beat_res.values()) * 4  # 4/4 time signature
-        vocab += [f"Position_{i}" for i in range(nb_positions)]
+        # TIME SHIFTS
+        vocab += [
+            f'TimeShift_{".".join(map(str, self.durations[i]))}'
+            for i in range(len(self.durations))
+        ]
 
         # CHORD
-        if self.additional_tokens["Chord"]:
+        if self.config.use_chords:
             vocab += self._create_chords_tokens()
 
         # REST
-        if self.additional_tokens["Rest"]:
+        if self.config.use_rests:
             vocab += [f'Rest_{".".join(map(str, rest))}' for rest in self.rests]
 
         # TEMPO
-        if self.additional_tokens["Tempo"]:
+        if self.config.use_tempos:
             vocab += [f"Tempo_{i}" for i in self.tempos]
 
         # PROGRAM
-        if self.additional_tokens["Program"]:
+        if self.config.use_programs:
             vocab += [f"Program_{program}" for program in range(-1, 128)]
 
+        # TIME SIGNATURE
+        if self.config.use_time_signatures:
+            vocab += [f"TimeSig_{i[0]}/{i[1]}" for i in self.time_signatures]
+
         return vocab
 
     def _create_token_types_graph(self) -> Dict[str, List[str]]:
         r"""Returns a graph (as a dictionary) of the possible token
         types successions.
         NOTE: Program type is not referenced here, you can add it manually by
         modifying the tokens_types_graph class attribute following your strategy.
 
         :return: the token types transitions dictionary
         """
         dic = dict()
 
-        dic["Bar"] = ["Position", "Bar"]
-
-        dic["Position"] = ["Pitch"]
         dic["Pitch"] = ["Velocity"]
         dic["Velocity"] = ["Duration"]
-        dic["Duration"] = ["Pitch", "Position", "Bar"]
-
-        if self.additional_tokens["Program"]:
-            dic["Program"] = ["Bar"]
+        dic["Duration"] = ["Pitch", "TimeShift"]
+        dic["TimeShift"] = ["Pitch"]
 
-        if self.additional_tokens["Chord"]:
+        if self.config.use_chords:
             dic["Chord"] = ["Pitch"]
-            dic["Duration"] += ["Chord"]
-            dic["Position"] += ["Chord"]
+            dic["TimeShift"] += ["Chord"]
 
-        if self.additional_tokens["Tempo"]:
-            dic["Tempo"] = (
-                ["Chord", "Pitch"] if self.additional_tokens["Chord"] else ["Pitch"]
-            )
-            dic["Position"] += ["Tempo"]
+        if self.config.use_tempos:
+            dic["TimeShift"] += ["Tempo"]
+            dic["Tempo"] = ["Pitch", "TimeShift"]
+            if self.config.use_chords:
+                dic["Tempo"] += ["Chord"]
 
-        if self.additional_tokens["Rest"]:
-            dic["Rest"] = ["Rest", "Position", "Bar"]
+        if self.config.use_rests:
+            dic["Rest"] = ["Rest", "Pitch", "TimeShift"]
             dic["Duration"] += ["Rest"]
+            if self.config.use_chords:
+                dic["Rest"] += ["Chord"]
+            if self.config.use_tempos:
+                dic["Rest"] += ["Tempo"]
+                dic["Tempo"] += ["Rest"]
+            if self.config.use_time_signatures:
+                dic["Rest"] += ["TimeSig"]
+                dic["TimeSig"] += ["Rest"]
+
+        if self.config.use_programs:
+            dic["Program"] = ["Pitch"]
+            dic["Duration"] += ["Program"]
+            dic["Duration"].remove("Pitch")
+            dic["TimeShift"] += ["Program"]
+            dic["TimeShift"].remove("Pitch")
+            if self.config.use_chords:
+                dic["Program"] += ["Chord"]
+                dic["Chord"] += ["Program"]
+                dic["Chord"].remove("Pitch")
+            if self.config.use_tempos:
+                dic["Tempo"] += ["Program"]
+                dic["Tempo"].remove("Pitch")
+            if self.config.use_rests:
+                dic["Rest"] += ["Program"]
+                dic["Rest"].remove("Pitch")
 
         return dic
 
     @staticmethod
     def _order(x: Event) -> int:
         r"""Helper function to sort events in the right order
 
         :param x: event to get order index
         :return: an order int
         """
-        if x.type == "Program":
-            return 0
-        elif x.type == "Bar":
+        if x.type == "Tempo":
             return 1
-        elif x.type == "Position":
+        elif x.type == "TimeSig":
             return 2
-        elif (
-            x.type == "Chord" or x.type == "Tempo"
-        ):  # actually object_list will be before chords
-            return 3
-        elif x.type == "Rest":
-            return 5
+        elif x.type == "TimeShift" or x.type == "Rest":
+            return 1000  # always last
         else:  # for other types of events, the order should be handle when inserting the events in the sequence
             return 4
```

### Comparing `miditok-2.0.6/miditok/tokenizations/remi_plus.py` & `miditok-2.1.0/miditok/tokenizations/remi_plus.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,17 @@
 from math import ceil
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Tuple, Union, cast
 
 import numpy as np
 from miditoolkit import Instrument, MidiFile, Note, TempoChange, TimeSignature
 
-from ..classes import Event, TokSequence
+from ..classes import Event, TokSequence, TokenizerConfig
 from ..constants import (
-    ADDITIONAL_TOKENS,
-    BEAT_RES,
     MIDI_INSTRUMENTS,
-    NB_VELOCITIES,
-    PITCH_RANGE,
-    SPECIAL_TOKENS,
     TEMPO,
     TIME_DIVISION,
     TIME_SIGNATURE,
 )
 from ..midi_tokenizer import MIDITokenizer, _in_as_seq, _out_as_complete_seq
 from ..utils import detect_chords
 
@@ -27,77 +22,46 @@
     `FIGARO (Rütte et al.) <https://arxiv.org/abs/2201.10936>`, which
     represents notes as successions of *Program* (originally *Instrument* in the paper),
     *Pitch*, *Velocity* and *Duration* tokens, and time with *Bar* and *Position* tokens.
     A *Bar* token indicate that a new bar is beginning, and *Position* the current
     position within the current bar. The number of positions is determined by
     the ``beat_res`` argument, the maximum value will be used as resolution.
 
-    :param pitch_range: range of MIDI pitches to use
-    :param beat_res: beat resolutions, as a dictionary:
-            {(beat_x1, beat_x2): beat_res_1, (beat_x2, beat_x3): beat_res_2, ...}
-            The keys are tuples indicating a range of beats, ex 0 to 3 for the first bar, and
-            the values are the resolution to apply to the ranges, in samples per beat, ex 8
-    :param nb_velocities: number of velocity bins
-    :param additional_tokens: additional tokens (chords, time signature, rests, tempo...) to use,
-            to be given as a dictionary. (default: None is used)
-    :param special_tokens: list of special tokens. This must be given as a list of strings given
-            only the names of the tokens. (default: ``["PAD", "BOS", "EOS", "MASK"]``)
+    :param tokenizer_config: the tokenizer's configuration, as a :class:`miditok.classes.TokenizerConfig` object.
+    :param max_bar_embedding: Maximum number of bars ("Bar_0", "Bar_1",...,"Bar_{num_bars-1}").
+            If None passed, creates "Bar_None" token only in vocabulary for Bar token.
     :param params: path to a tokenizer config file. This will override other arguments and
             load the tokenizer based on the config file. This is particularly useful if the
             tokenizer learned Byte Pair Encoding. (default: None)
-    :param max_bar_embedding: Maximum number of bars ("Bar_0", "Bar_1",...,"Bar_{num_bars-1}").
-            If None passed, creates "Bar_None" token only in vocabulary for Bar token.
     """
 
     def __init__(
         self,
-        pitch_range: range = PITCH_RANGE,
-        beat_res: Dict[Tuple[int, int], int] = BEAT_RES,
-        nb_velocities: int = NB_VELOCITIES,
-        additional_tokens: Dict[
-            str, Union[bool, int, Tuple[int, int]]
-        ] = ADDITIONAL_TOKENS,
-        special_tokens: List[str] = SPECIAL_TOKENS,
-        params: Optional[Union[str, Path]] = None,
-        max_bar_embedding: Optional[int] = 60,
+        tokenizer_config: TokenizerConfig = None,
+        max_bar_embedding: Optional[int] = None,
+        params: Union[str, Path] = None,
     ):
-        additional_tokens["Program"] = True  # required
-        # code handling rest decoding is writen, but not for detection (encoding)
-        additional_tokens["Rest"] = False
-        self.programs = additional_tokens.get("programs", list(range(-1, 128)))
-        self.max_bar_embedding = (
-            max_bar_embedding  # this attribute might increase during encoding
-        )
-        super().__init__(
-            pitch_range,
-            beat_res,
-            nb_velocities,
-            additional_tokens,
-            special_tokens,
-            unique_track=True,  # handles multi-track sequences in single stream
-            params=params,  # type: ignore
-        )
+        if (
+            tokenizer_config is not None
+            and "max_bar_embedding" not in tokenizer_config.additional_params
+        ):
+            # If used, this attribute might increase over tokenizations, if the tokenizer encounter longer MIDIs
+            tokenizer_config.additional_params["max_bar_embedding"] = max_bar_embedding
+        super().__init__(tokenizer_config, True, params)
 
-    def save_params(
-        self, out_path: Union[str, Path], additional_attributes: Optional[Dict] = None
-    ):
-        r"""Saves the config / parameters of the tokenizer in a json encoded file.
-        This can be useful to keep track of how a dataset has been tokenized.
+    def _tweak_config_before_creating_voc(self):
+        self.config.use_programs = True
+        # code handling rest decoding is writen, but not for detection (encoding)
+        self.config.use_rests = False
+        # self.unique_track = True
 
-        :param out_path: output path to save the file.
-        :param additional_attributes: any additional information to store in the config file.
-                It can be used to override the default attributes saved in the parent method. (default: None)
-        """
-        if additional_attributes is None:
-            additional_attributes = {}
-        additional_attributes_tmp = {
-            "max_bar_embedding": self.max_bar_embedding,
-            **additional_attributes,
-        }
-        super().save_params(out_path, additional_attributes_tmp)
+        # In case the tokenizer has been created without specifying any config or params file path
+        if "max_bar_embedding" not in self.config.additional_params:
+            # If used, this attribute might increase over tokenizations, if the tokenizer encounter longer MIDIs
+            self.config.additional_params["max_bar_embedding"] = None
 
     def __notes_to_events(self, tracks: List[Instrument]) -> List[Event]:
         """Convert multi-track notes into one Token sequence.
 
         :param tracks: list of tracks (`miditoolkit.Instrument`) to convert.
         :return: sequences of Event.
         """
@@ -108,32 +72,36 @@
             for note in track.notes
         ]
         notes_with_program.sort(key=lambda n: (n[0].start, n[0].pitch))
 
         # Make sure the notes are sorted first by their onset (start) times, second by pitch
         # notes.sort(key=lambda x: (x.start, x.pitch))  # done in midi_to_tokens
         time_division = self._current_midi_metadata["time_division"]
-        ticks_per_sample = time_division / max(self.beat_res.values())
+        ticks_per_sample = time_division / max(self.config.beat_res.values())
         dur_bins = self._durations_ticks[self._current_midi_metadata["time_division"]]
         # Creates events
         events: List[Event] = []
         previous_tick = -1
         previous_note_end = (
             notes_with_program[0][0].start + 1
         )  # so that no rest is created before the first note
         # Bar
-        if self.max_bar_embedding:  # Check bar embedding limit, update if needed
+        if self.config.additional_params[
+            "max_bar_embedding"
+        ]:  # Check bar embedding limit, update if needed
             nb_bars = ceil(
                 max(n[0].end for n in notes_with_program)
                 / (self._current_midi_metadata["time_division"] * 4)
             )
-            if self.max_bar_embedding < nb_bars:
-                for i in range(self.max_bar_embedding, nb_bars):
+            if self.config.additional_params["max_bar_embedding"] < nb_bars:
+                for i in range(
+                    self.config.additional_params["max_bar_embedding"], nb_bars
+                ):
                     self.add_to_vocab(f"Bar_{i}")
-                self.max_bar_embedding = nb_bars
+                self.config.additional_params["max_bar_embedding"] = nb_bars
         current_bar = -1
         # Tempo
         current_tempo_idx = 0
         current_tempo = self._current_midi_metadata["tempo_changes"][
             current_tempo_idx
         ].tempo
         # TimeSignature
@@ -144,29 +112,25 @@
             current_time_sig_idx
         ]
         current_time_sig = self._reduce_time_signature(
             time_sig_change.numerator, time_sig_change.denominator
         )
         ticks_per_bar = time_division * current_time_sig[0]
         # (Chord)
-        if self.additional_tokens.get("Chord", False):  # "Chord" in additional tokens
+        if self.config.use_chords:  # "Chord" in additional tokens
             for track in tracks:  # find chords per track
                 if track.is_drum:
                     continue
                 chords = detect_chords(
                     track.notes,
                     self._current_midi_metadata["time_division"],
-                    chord_maps=self.additional_tokens["chord_maps"],
-                    specify_root_note=self.additional_tokens[
-                        "chord_tokens_with_root_note"
-                    ],
+                    chord_maps=self.config.chord_maps,
+                    specify_root_note=self.config.chord_tokens_with_root_note,
                     beat_res=self._first_beat_res,
-                    unknown_chords_nb_notes_range=self.additional_tokens[
-                        "chord_unknown"
-                    ],
+                    unknown_chords_nb_notes_range=self.config.chord_unknown,
                 )
                 for chord in chords:
                     pos_index = int((chord.time % ticks_per_bar) / ticks_per_sample)
                     events.append(
                         Event("Position", pos_index, chord.time, "PositionChord")
                     )
                     events.append(
@@ -180,24 +144,25 @@
                 # Bar
                 nb_new_bars = note.start // ticks_per_bar - current_bar
                 for i in range(nb_new_bars):
                     events.append(
                         Event(
                             type="Bar",
                             value=str(current_bar + i + 1)
-                            if self.max_bar_embedding is not None
+                            if self.config.additional_params["max_bar_embedding"]
+                            is not None
                             else "None",
                             time=(current_bar + i + 1) * ticks_per_bar,
                             desc=0,
                         )
                     )
                 current_bar += nb_new_bars
 
                 # (TimeSignature)
-                if self.additional_tokens["TimeSignature"]:
+                if self.config.use_time_signatures:
                     # If the current time signature is not the last one
                     if current_time_sig_idx + 1 < len(
                         self._current_midi_metadata["time_sig_changes"]
                     ):
                         # Will loop over incoming time signature changes
                         for time_sig_change in self._current_midi_metadata[
                             "time_sig_changes"
@@ -222,15 +187,15 @@
                                 type="TimeSig",
                                 value=f"{current_time_sig[0]}/{current_time_sig[1]}",
                                 time=note.start,
                             )
                         )
 
                 # (Tempo)
-                if self.additional_tokens["Tempo"]:
+                if self.config.use_tempos:
                     is_tempo_changed = False
                     # If the current tempo is not the last one
                     if current_tempo_idx + 1 < len(
                         self._current_midi_metadata["tempo_changes"]
                     ):
                         # Will loop over incoming tempo changes
                         for tempo_change in self._current_midi_metadata[
@@ -369,18 +334,18 @@
         :param output_path: path to save the file. (default: None)
         :param time_division: MIDI time division / resolution, in ticks/beat (of the MIDI to create).
         :return: the midi object (:class:`miditoolkit.MidiFile`).
         """
         tokens = cast(TokSequence, tokens)
         midi = MidiFile(ticks_per_beat=time_division)
         assert (
-            time_division % max(self.beat_res.values()) == 0
-        ), f"Invalid time division, please give one divisible by {max(self.beat_res.values())}"
+            time_division % max(self.config.beat_res.values()) == 0
+        ), f"Invalid time division, please give one divisible by {max(self.config.beat_res.values())}"
         tokens = cast(List[str], tokens.tokens)  # for reducing type errors
-        ticks_per_sample = time_division // max(self.beat_res.values())
+        ticks_per_sample = time_division // max(self.config.beat_res.values())
 
         # RESULTS
         instruments: Dict[int, Instrument] = {}
         tempo_changes = [
             TempoChange(TEMPO, -1)
         ]  # mock the first tempo change to optimize below
         time_signature_changes = [
@@ -491,49 +456,51 @@
         will be added to the vocabulary by :class:`miditok.MIDITokenizer`.
 
         :return: the vocabulary as a list of string.
         """
         vocab = []
 
         # BAR
-        if self.max_bar_embedding:
-            vocab += [f"Bar_{i}" for i in range(self.max_bar_embedding)]
+        if self.config.additional_params["max_bar_embedding"] is not None:
+            vocab += [
+                f"Bar_{i}"
+                for i in range(self.config.additional_params["max_bar_embedding"])
+            ]
         else:
             vocab += ["Bar_None"]
 
         # PITCH
-        vocab += [f"Pitch_{i}" for i in self.pitch_range]
+        vocab += [f"Pitch_{i}" for i in range(*self.config.pitch_range)]
 
         # VELOCITY
         vocab += [f"Velocity_{i}" for i in self.velocities]
 
         # DURATION
         vocab += [
             f'Duration_{".".join(map(str, duration))}' for duration in self.durations
         ]
 
         # POSITION
-        nb_positions = max(self.beat_res.values()) * 4  # 4/4 time signature
+        nb_positions = max(self.config.beat_res.values()) * 4  # 4/4 time signature
         vocab += [f"Position_{i}" for i in range(nb_positions)]
 
         # TIME SIGNATURE
-        if self.additional_tokens["TimeSignature"]:
+        if self.config.use_time_signatures:
             vocab += [f"TimeSig_{i[0]}/{i[1]}" for i in self.time_signatures]
 
         # CHORD
-        if self.additional_tokens["Chord"]:
+        if self.config.use_chords:
             vocab += self._create_chords_tokens()
 
         # TEMPO
-        if self.additional_tokens["Tempo"]:
+        if self.config.use_tempos:
             vocab += [f"Tempo_{i}" for i in self.tempos]
 
         # PROGRAM
-        if self.additional_tokens["Program"]:
-            vocab += [f"Program_{program}" for program in self.programs]
+        vocab += [f"Program_{program}" for program in self.config.programs]
 
         return vocab
 
     def _create_token_types_graph(self) -> Dict[str, List[str]]:
         r"""Returns a graph (as a dictionary) of the possible token
         types successions.
 
@@ -544,23 +511,23 @@
         dic["Bar"] = ["Position", "Bar"]
         dic["Position"] = ["Program"]
         dic["Program"] = ["Pitch", "Chord"]
         dic["Pitch"] = ["Velocity"]
         dic["Velocity"] = ["Duration"]
         dic["Duration"] = ["Program", "Position", "Bar"]
 
-        if self.additional_tokens["TimeSignature"]:
+        if self.config.use_time_signatures:
             dic["Bar"] = ["TimeSig", "Bar"]
             dic["TimeSig"] = ["Position"]
 
-        if self.additional_tokens["Chord"]:
+        if self.config.use_chords:
             dic["Chord"] = ["Position"]
             dic["Position"] += ["Chord"]
 
-        if self.additional_tokens["Tempo"]:
+        if self.config.use_tempos:
             dic["Tempo"] = ["Position"]
             dic["Position"] += ["Tempo"]
 
         return dic
 
     @staticmethod
     def _order(x: Event) -> int:
@@ -597,15 +564,15 @@
 
         err_type = 0  # i.e. incompatible next type predicted
         err_time = 0  # i.e. goes back or stay in time (does not go forward)
         err_note = 0  # i.e. duplicated
         previous_type = tokens[0].split("_")[0]
         current_pos = -1
         current_program = 0
-        current_pitches = {p: [] for p in self.programs}
+        current_pitches = {p: [] for p in self.config.programs}
 
         # Init first note and current pitches if needed
         if previous_type == "Pitch":
             pitch_val = int(tokens[0].split("_")[1])
             current_pitches[current_program].append(pitch_val)
         elif previous_type == "Position":
             current_pos = int(tokens[0].split("_")[1])
@@ -613,27 +580,27 @@
         for token in tokens[1:]:
             event_type, event_value = token.split("_")[0], token.split("_")[1]
 
             # Good token type
             if event_type in self.tokens_types_graph[previous_type]:
                 if event_type == "Bar":  # reset
                     current_pos = -1
-                    current_pitches = {p: [] for p in self.programs}
+                    current_pitches = {p: [] for p in self.config.programs}
                 elif previous_type == "Pitch":
                     pitch_val = int(event_value)
                     if pitch_val in current_pitches[current_program]:
                         err_note += 1  # pitch already played at current position
                     else:
                         current_pitches[current_program].append(pitch_val)
                 elif event_type == "Position":
                     if int(event_value) < current_pos:
                         err_time += 1  # token position value <= to the current position
                     else:
                         current_pos = int(event_value)
-                        current_pitches = {p: [] for p in self.programs}
+                        current_pitches = {p: [] for p in self.config.programs}
                 elif event_type == "Program":  # reset
                     current_program = int(event_value)
             # Bad token type
             else:
                 err_type += 1
             previous_type = event_type
```

### Comparing `miditok-2.0.6/miditok/tokenizations/structured.py` & `miditok-2.1.0/miditok/tokenizations/structured.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,15 @@
 from typing import List, Tuple, Dict, Optional, Union, Any
-from pathlib import Path
 
 import numpy as np
 from miditoolkit import Instrument, Note, TempoChange
 
 from ..midi_tokenizer import MIDITokenizer, _in_as_seq, _out_as_complete_seq
 from ..classes import TokSequence, Event
 from ..constants import (
-    PITCH_RANGE,
-    NB_VELOCITIES,
-    BEAT_RES,
-    ADDITIONAL_TOKENS,
-    SPECIAL_TOKENS,
     TIME_DIVISION,
     TEMPO,
     MIDI_INSTRUMENTS,
 )
 
 
 class Structured(MIDITokenizer):
@@ -24,52 +18,21 @@
     Token types always follow the same pattern: *Pitch* -> *Velocity* -> *Duration* -> *TimeShift*.
     The latter is set to 0 for simultaneous notes.
     To keep this property, no additional token can be inserted in MidiTok's implementation,
     except *Program* that can be added to the vocabulary and are up to you to use.
     **Note:** as Structured uses *TimeShifts* events to move the time from note to
     note, it could be unsuited for tracks with long pauses. In such case, the
     maximum *TimeShift* value will be used.
-
-    :param pitch_range: range of MIDI pitches to use
-    :param beat_res: beat resolutions, as a dictionary:
-            {(beat_x1, beat_x2): beat_res_1, (beat_x2, beat_x3): beat_res_2, ...}
-            The keys are tuples indicating a range of beats, ex 0 to 3 for the first bar, and
-            the values are the resolution to apply to the ranges, in samples per beat, ex 8
-    :param nb_velocities: number of velocity bins
-    :param additional_tokens: additional tokens (chords, time signature, rests, tempo...) to use,
-            to be given as a dictionary. (default: None is used)
-    :param special_tokens: list of special tokens. This must be given as a list of strings given
-            only the names of the tokens. (default: ``["PAD", "BOS", "EOS", "MASK"]``)
-    :param params: path to a tokenizer config file. This will override other arguments and
-            load the tokenizer based on the config file. This is particularly useful if the
-            tokenizer learned Byte Pair Encoding. (default: None)
     """
 
-    def __init__(
-        self,
-        pitch_range: range = PITCH_RANGE,
-        beat_res: Dict[Tuple[int, int], int] = BEAT_RES,
-        nb_velocities: int = NB_VELOCITIES,
-        additional_tokens: Dict[str, Union[bool, int]] = ADDITIONAL_TOKENS,
-        special_tokens: List[str] = SPECIAL_TOKENS,
-        params: Union[str, Path] = None,
-    ):
-        # No additional tokens
-        additional_tokens["Chord"] = False  # Incompatible additional token
-        additional_tokens["Rest"] = False
-        additional_tokens["Tempo"] = False
-        additional_tokens["TimeSignature"] = False
-        super().__init__(
-            pitch_range,
-            beat_res,
-            nb_velocities,
-            additional_tokens,
-            special_tokens,
-            params=params,
-        )
+    def _tweak_config_before_creating_voc(self):
+        self.config.use_chords = False
+        self.config.use_rests = False
+        self.config.use_tempos = False
+        self.config.use_time_signatures = False
 
     @_out_as_complete_seq
     def track_to_tokens(self, track: Instrument) -> TokSequence:
         r"""Converts a track (miditoolkit.Instrument object) into a sequence of tokens (:class:`miditok.TokSequence`).
 
         :param track: MIDI track to convert
         :return: :class:`miditok.TokSequence` of corresponding tokens.
@@ -134,15 +97,15 @@
                     desc=f"{time_shift} ticks",
                     value=".".join(map(str, self.durations[index]))
                     if time_shift != 0
                     else "0.0.1",
                 )
             )
         # Adds the last note
-        if track.notes[-1].pitch not in self.pitch_range:
+        if track.notes[-1].pitch not in range(*self.config.pitch_range):
             if len(events) > 0:
                 del events[-1]
         else:
             events.append(
                 Event(
                     type="Pitch",
                     value=track.notes[-1].pitch,
@@ -237,15 +200,15 @@
             print(
                 "\033[93msos_eos_tokens argument is depreciated and will be removed in a future update, "
                 "_create_vocabulary now uses self._sos_eos attribute set a class init \033[0m"
             )
         vocab = []
 
         # PITCH
-        vocab += [f"Pitch_{i}" for i in self.pitch_range]
+        vocab += [f"Pitch_{i}" for i in range(*self.config.pitch_range)]
 
         # VELOCITY
         vocab += [f"Velocity_{i}" for i in self.velocities]
 
         # DURATION
         vocab += [
             f'Duration_{".".join(map(str, duration))}' for duration in self.durations
@@ -254,15 +217,15 @@
         # TIME SHIFT (same as durations)
         vocab.append("TimeShift_0.0.1")  # for a time shift of 0
         vocab += [
             f'TimeShift_{".".join(map(str, duration))}' for duration in self.durations
         ]
 
         # PROGRAM
-        if self.additional_tokens["Program"]:
+        if self.config.use_programs:
             vocab += [f"Program_{program}" for program in range(-1, 128)]
 
         return vocab
 
     def _create_token_types_graph(self) -> Dict[str, List[str]]:
         r"""Returns a graph (as a dictionary) of the possible token
         types successions.
```

### Comparing `miditok-2.0.6/miditok/tokenizations/tsd.py` & `miditok-2.1.0/miditok/tokenizations/remi.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,97 +1,174 @@
 from typing import List, Tuple, Dict, Optional, Union, Any
-from pathlib import Path
 
 import numpy as np
 from miditoolkit import Instrument, Note, TempoChange
 
 from ..midi_tokenizer import MIDITokenizer, _in_as_seq, _out_as_complete_seq
 from ..classes import TokSequence, Event
 from ..utils import detect_chords
 from ..constants import (
-    PITCH_RANGE,
-    NB_VELOCITIES,
-    BEAT_RES,
-    ADDITIONAL_TOKENS,
-    SPECIAL_TOKENS,
     TIME_DIVISION,
     TEMPO,
     MIDI_INSTRUMENTS,
 )
 
 
-class TSD(MIDITokenizer):
-    r"""TSD, for Time Shift Duration, is similar to MIDI-Like :ref:`MIDI-Like`
-    but uses explicit *Duration* tokens to represent note durations, which have
-    showed `better results than with NoteOff tokens <https://arxiv.org/abs/2002.00212>`_.
-    **Note:** as TSD uses *TimeShifts* events to move the time from note to
-    note, it could be unsuited for tracks with long pauses. In such case, the
-    maximum *TimeShift* value will be used.
-
-    :param pitch_range: range of MIDI pitches to use
-    :param beat_res: beat resolutions, as a dictionary:
-            {(beat_x1, beat_x2): beat_res_1, (beat_x2, beat_x3): beat_res_2, ...}
-            The keys are tuples indicating a range of beats, ex 0 to 3 for the first bar, and
-            the values are the resolution to apply to the ranges, in samples per beat, ex 8
-    :param nb_velocities: number of velocity bins
-    :param additional_tokens: additional tokens (chords, time signature, rests, tempo...) to use,
-            to be given as a dictionary. (default: None is used)
-    :param special_tokens: list of special tokens. This must be given as a list of strings given
-            only the names of the tokens. (default: ``["PAD", "BOS", "EOS", "MASK"]``)
-    :param params: path to a tokenizer config file. This will override other arguments and
-            load the tokenizer based on the config file. This is particularly useful if the
-            tokenizer learned Byte Pair Encoding. (default: None)
+class REMI(MIDITokenizer):
+    r"""REMI, standing for Revamped MIDI and introduced with the
+    `Pop Music Transformer (Huang and Yang) <https://dl.acm.org/doi/10.1145/3394171.3413671>`_,
+    is a tokenization that represents notes as successions of *Pitch*, *Velocity* and *Duration*
+    tokens, and time with *Bar* and *Position* tokens. A *Bar* token indicate that a new bar
+    is beginning, and *Position* the current position within the current bar. The number of
+    positions is determined by the ``beat_res`` argument, the maximum value will be used as
+    resolution.
+    **NOTE:** in the original paper, the tempo information is represented as the succession
+    of two token types: a *TempoClass* indicating if the tempo is fast or slow, and a
+    *TempoValue* indicating its value. MidiTok only uses one *Tempo* token for its value
+    (see :ref:`Additional tokens`).
     """
 
-    def __init__(
-        self,
-        pitch_range: range = PITCH_RANGE,
-        beat_res: Dict[Tuple[int, int], int] = BEAT_RES,
-        nb_velocities: int = NB_VELOCITIES,
-        additional_tokens: Dict[str, bool] = ADDITIONAL_TOKENS,
-        special_tokens: List[str] = SPECIAL_TOKENS,
-        params: Union[str, Path] = None,
-    ):
-        additional_tokens["TimeSignature"] = False  # not compatible
-        super().__init__(
-            pitch_range,
-            beat_res,
-            nb_velocities,
-            additional_tokens,
-            special_tokens,
-            params=params,
-        )
+    def _tweak_config_before_creating_voc(self):
+        self.config.use_time_signatures = False
 
     @_out_as_complete_seq
     def track_to_tokens(self, track: Instrument) -> TokSequence:
         r"""Converts a track (miditoolkit.Instrument object) into a sequence of tokens (:class:`miditok.TokSequence`).
-        (can probably be achieved faster with Mido objects)
 
         :param track: MIDI track to convert
         :return: :class:`miditok.TokSequence` of corresponding tokens.
         """
         # Make sure the notes are sorted first by their onset (start) times, second by pitch
         # notes.sort(key=lambda x: (x.start, x.pitch))  # done in midi_to_tokens
         ticks_per_sample = self._current_midi_metadata["time_division"] / max(
-            self.beat_res.values()
+            self.config.beat_res.values()
         )
+        ticks_per_bar = self._current_midi_metadata["time_division"] * 4
         dur_bins = self._durations_ticks[self._current_midi_metadata["time_division"]]
         min_rest = (
             self._current_midi_metadata["time_division"] * self.rests[0][0]
             + ticks_per_sample * self.rests[0][1]
-            if self.additional_tokens["Rest"]
+            if self.config.use_rests
             else 0
         )
+
         events = []
 
-        # Creates the Note On, Note Off and Velocity events
-        for n, note in enumerate(track.notes):
-            # Note On / Velocity / Duration
+        # Creates events
+        previous_tick = -1
+        previous_note_end = (
+            track.notes[0].start + 1
+        )  # so that no rest is created before the first note
+        current_bar = -1
+        current_tempo_idx = 0
+        current_tempo = self._current_midi_metadata["tempo_changes"][
+            current_tempo_idx
+        ].tempo
+        for note in track.notes:
+            if note.start != previous_tick:
+                # (Rest)
+                if (
+                    self.config.use_rests
+                    and note.start > previous_note_end
+                    and note.start - previous_note_end >= min_rest
+                ):
+                    previous_tick = previous_note_end
+                    rest_beat, rest_pos = divmod(
+                        note.start - previous_tick,
+                        self._current_midi_metadata["time_division"],
+                    )
+                    rest_beat = min(rest_beat, max([r[0] for r in self.rests]))
+                    rest_pos = round(rest_pos / ticks_per_sample)
+
+                    if rest_beat > 0:
+                        events.append(
+                            Event(
+                                type="Rest",
+                                value=f"{rest_beat}.0",
+                                time=previous_note_end,
+                                desc=f"{rest_beat}.0",
+                            )
+                        )
+                        previous_tick += (
+                            rest_beat * self._current_midi_metadata["time_division"]
+                        )
+
+                    while rest_pos >= self.rests[0][1]:
+                        rest_pos_temp = min(
+                            [r[1] for r in self.rests], key=lambda x: abs(x - rest_pos)
+                        )
+                        events.append(
+                            Event(
+                                type="Rest",
+                                value=f"0.{rest_pos_temp}",
+                                time=previous_note_end,
+                                desc=f"0.{rest_pos_temp}",
+                            )
+                        )
+                        previous_tick += round(rest_pos_temp * ticks_per_sample)
+                        rest_pos -= rest_pos_temp
+
+                    current_bar = previous_tick // ticks_per_bar
+
+                # Bar
+                nb_new_bars = note.start // ticks_per_bar - current_bar
+                for i in range(nb_new_bars):
+                    events.append(
+                        Event(
+                            type="Bar",
+                            value="None",
+                            time=(current_bar + i + 1) * ticks_per_bar,
+                            desc=0,
+                        )
+                    )
+                current_bar += nb_new_bars
+
+                # Position
+                pos_index = int((note.start % ticks_per_bar) / ticks_per_sample)
+                events.append(
+                    Event(
+                        type="Position",
+                        value=pos_index,
+                        time=note.start,
+                        desc=note.start,
+                    )
+                )
+
+                # (Tempo)
+                if self.config.use_tempos:
+                    # If the current tempo is not the last one
+                    if current_tempo_idx + 1 < len(
+                        self._current_midi_metadata["tempo_changes"]
+                    ):
+                        # Will loop over incoming tempo changes
+                        for tempo_change in self._current_midi_metadata[
+                            "tempo_changes"
+                        ][current_tempo_idx + 1 :]:
+                            # If this tempo change happened before the current moment
+                            if tempo_change.time <= note.start:
+                                current_tempo = tempo_change.tempo
+                                current_tempo_idx += (
+                                    1  # update tempo value (might not change) and index
+                                )
+                            else:  # <==> elif tempo_change.time > previous_tick:
+                                break  # this tempo change is beyond the current time step, we break the loop
+                    events.append(
+                        Event(
+                            type="Tempo",
+                            value=current_tempo,
+                            time=note.start,
+                            desc=note.start,
+                        )
+                    )
+
+                previous_tick = note.start
+
+            # Pitch / Velocity / Duration
             events.append(
-                Event(type="Pitch", value=note.pitch, time=note.start, desc=note.end)
+                Event(type="Pitch", value=note.pitch, time=note.start, desc=note.pitch)
             )
             events.append(
                 Event(
                     type="Velocity",
                     value=note.velocity,
                     time=note.start,
                     desc=f"{note.velocity}",
@@ -103,118 +180,26 @@
                 Event(
                     type="Duration",
                     value=".".join(map(str, self.durations[index])),
                     time=note.start,
                     desc=f"{duration} ticks",
                 )
             )
-        # Adds tempo events if specified
-        if self.additional_tokens["Tempo"]:
-            for tempo_change in self._current_midi_metadata["tempo_changes"]:
-                events.append(
-                    Event(
-                        type="Tempo",
-                        value=tempo_change.tempo,
-                        time=tempo_change.time,
-                        desc=tempo_change.tempo,
-                    )
-                )
 
-        # Sorts events
-        events.sort(key=lambda x: x.time)
-
-        # Time Shift
-        previous_tick = 0
-        previous_note_end = track.notes[0].start + 1
-        for e, event in enumerate(events.copy()):
-            # No time shift
-            if event.time == previous_tick:
-                pass
-
-            # (Rest)
-            elif (
-                event.type in ["Pitch", "Tempo"]
-                and self.additional_tokens["Rest"]
-                and event.time - previous_note_end >= min_rest
-            ):
-                rest_beat, rest_pos = divmod(
-                    event.time - previous_tick,
-                    self._current_midi_metadata["time_division"],
-                )
-                rest_beat = min(rest_beat, max([r[0] for r in self.rests]))
-                rest_pos = round(rest_pos / ticks_per_sample)
-                rest_tick = previous_tick  # untouched tick value to the order is not messed after sorting
-
-                if rest_beat > 0:
-                    events.append(
-                        Event(
-                            type="Rest",
-                            value=f"{rest_beat}.0",
-                            time=rest_tick,
-                            desc=f"{rest_beat}.0",
-                        )
-                    )
-                    previous_tick += (
-                        rest_beat * self._current_midi_metadata["time_division"]
-                    )
-
-                while rest_pos >= self.rests[0][1]:
-                    rest_pos_temp = min(
-                        [r[1] for r in self.rests], key=lambda x: abs(x - rest_pos)
-                    )
-                    events.append(
-                        Event(
-                            type="Rest",
-                            value=f"0.{rest_pos_temp}",
-                            time=rest_tick,
-                            desc=f"0.{rest_pos_temp}",
-                        )
-                    )
-                    previous_tick += round(rest_pos_temp * ticks_per_sample)
-                    rest_pos -= rest_pos_temp
-
-                # Adds an additional time shift if needed
-                if rest_pos > 0:
-                    time_shift = round(rest_pos * ticks_per_sample)
-                    index = np.argmin(np.abs(dur_bins - time_shift))
-                    events.append(
-                        Event(
-                            type="TimeShift",
-                            value=".".join(map(str, self.durations[index])),
-                            time=previous_tick,
-                            desc=f"{time_shift} ticks",
-                        )
-                    )
-
-            # Time shift
-            else:
-                time_shift = event.time - previous_tick
-                index = np.argmin(np.abs(dur_bins - time_shift))
-                events.append(
-                    Event(
-                        type="TimeShift",
-                        value=".".join(map(str, self.durations[index])),
-                        time=previous_tick,
-                        desc=f"{time_shift} ticks",
-                    )
-                )
-
-            if event.type == "Pitch":
-                previous_note_end = max(previous_note_end, event.desc)
-            previous_tick = event.time
+            previous_note_end = max(previous_note_end, note.end)
 
         # Adds chord events if specified
-        if self.additional_tokens["Chord"] and not track.is_drum:
+        if self.config.use_chords and not track.is_drum:
             events += detect_chords(
                 track.notes,
                 self._current_midi_metadata["time_division"],
-                chord_maps=self.additional_tokens["chord_maps"],
-                specify_root_note=self.additional_tokens["chord_tokens_with_root_note"],
+                chord_maps=self.config.chord_maps,
+                specify_root_note=self.config.chord_tokens_with_root_note,
                 beat_res=self._first_beat_res,
-                unknown_chords_nb_notes_range=self.additional_tokens["chord_unknown"],
+                unknown_chords_nb_notes_range=self.config.chord_unknown,
             )
 
         events.sort(key=lambda x: (x.time, self._order(x)))
 
         return TokSequence(events=events)
 
     @_in_as_seq()
@@ -228,188 +213,179 @@
 
         :param tokens: sequence of tokens to convert. Can be either a Tensor (PyTorch and Tensorflow are supported),
                 a numpy array, a Python list or a TokSequence.
         :param time_division: MIDI time division / resolution, in ticks/beat (of the MIDI to create)
         :param program: the MIDI program of the produced track and if it drum, (default (0, False), piano)
         :return: the miditoolkit instrument object and tempo changes
         """
-        ticks_per_sample = time_division // max(self.beat_res.values())
+        assert (
+            time_division % max(self.config.beat_res.values()) == 0
+        ), f"Invalid time division, please give one divisible by {max(self.config.beat_res.values())}"
         tokens = tokens.tokens
 
+        ticks_per_sample = time_division // max(self.config.beat_res.values())
+        ticks_per_bar = time_division * 4
         name = "Drums" if program[1] else MIDI_INSTRUMENTS[program[0]]["name"]
         instrument = Instrument(program[0], is_drum=program[1], name=name)
         tempo_changes = [
             TempoChange(TEMPO, -1)
         ]  # mock the first tempo change to optimize below
 
         current_tick = 0
-        ei = 0
-        while ei < len(tokens):
-            if tokens[ei].split("_")[0] == "Pitch":
+        current_bar = -1
+        previous_note_end = 0
+        for ti, token in enumerate(tokens):
+            if token.split("_")[0] == "Bar":
+                current_bar += 1
+                current_tick = current_bar * ticks_per_bar
+            elif token.split("_")[0] == "Rest":
+                beat, pos = map(int, tokens[ti].split("_")[1].split("."))
+                if (
+                    current_tick < previous_note_end
+                ):  # if in case successive rest happen
+                    current_tick = previous_note_end
+                current_tick += beat * time_division + pos * ticks_per_sample
+                current_bar = current_tick // ticks_per_bar
+            elif token.split("_")[0] == "Position":
+                if current_bar == -1:
+                    current_bar = (
+                        0  # as this Position token occurs before any Bar token
+                    )
+                current_tick = (
+                    current_bar * ticks_per_bar
+                    + int(token.split("_")[1]) * ticks_per_sample
+                )
+            elif token.split("_")[0] == "Tempo":
+                # If your encoding include tempo tokens, each Position token should be followed by
+                # a tempo token, but if it is not the case this method will skip this step
+                tempo = int(token.split("_")[1])
+                if tempo != tempo_changes[-1].tempo:
+                    tempo_changes.append(TempoChange(tempo, current_tick))
+            elif token.split("_")[0] == "Pitch":
                 try:
                     if (
-                        tokens[ei + 1].split("_")[0] == "Velocity"
-                        and tokens[ei + 2].split("_")[0] == "Duration"
+                        tokens[ti + 1].split("_")[0] == "Velocity"
+                        and tokens[ti + 2].split("_")[0] == "Duration"
                     ):
-                        pitch = int(tokens[ei].split("_")[1])
-                        vel = int(tokens[ei + 1].split("_")[1])
+                        pitch = int(tokens[ti].split("_")[1])
+                        vel = int(tokens[ti + 1].split("_")[1])
                         duration = self._token_duration_to_ticks(
-                            tokens[ei + 2].split("_")[1], time_division
+                            tokens[ti + 2].split("_")[1], time_division
                         )
                         instrument.notes.append(
                             Note(vel, pitch, current_tick, current_tick + duration)
                         )
-                        ei += 1
-                except IndexError:
-                    pass
-            elif tokens[ei].split("_")[0] == "TimeShift":
-                current_tick += self._token_duration_to_ticks(
-                    tokens[ei].split("_")[1], time_division
-                )
-            elif tokens[ei].split("_")[0] == "Rest":
-                beat, pos = map(int, tokens[ei].split("_")[1].split("."))
-                current_tick += beat * time_division + pos * ticks_per_sample
-            elif tokens[ei].split("_")[0] == "Tempo":
-                tempo = int(tokens[ei].split("_")[1])
-                if tempo != tempo_changes[-1].tempo:
-                    tempo_changes.append(TempoChange(tempo, current_tick))
-            ei += 1
+                        previous_note_end = max(
+                            previous_note_end, current_tick + duration
+                        )
+                except (
+                    IndexError
+                ):  # A well constituted sequence should not raise an exception
+                    pass  # However with generated sequences this can happen, or if the sequence isn't finished
+
         if len(tempo_changes) > 1:
             del tempo_changes[0]  # delete mocked tempo change
         tempo_changes[0].time = 0
         return instrument, tempo_changes
 
-    def _create_base_vocabulary(self, sos_eos_tokens: bool = False) -> List[str]:
+    def _create_base_vocabulary(self, sos_eos_tokens: bool = None) -> List[str]:
         r"""Creates the vocabulary, as a list of string tokens.
         Each token as to be given as the form of "Type_Value", separated with an underscore.
         Example: Pitch_58
         The :class:`miditok.MIDITokenizer` main class will then create the "real" vocabulary as
         a dictionary.
         Special tokens have to be given when creating the tokenizer, and
         will be added to the vocabulary by :class:`miditok.MIDITokenizer`.
 
         :return: the vocabulary as a list of string.
         """
-        vocab = []
+        vocab = ["Bar_None"]
 
-        # NOTE ON
-        vocab += [f"Pitch_{i}" for i in self.pitch_range]
+        # PITCH
+        vocab += [f"Pitch_{i}" for i in range(*self.config.pitch_range)]
 
         # VELOCITY
         vocab += [f"Velocity_{i}" for i in self.velocities]
 
         # DURATION
         vocab += [
             f'Duration_{".".join(map(str, duration))}' for duration in self.durations
         ]
 
-        # TIME SHIFTS
-        vocab += [
-            f'TimeShift_{".".join(map(str, self.durations[i]))}'
-            for i in range(len(self.durations))
-        ]
+        # POSITION
+        nb_positions = max(self.config.beat_res.values()) * 4  # 4/4 time signature
+        vocab += [f"Position_{i}" for i in range(nb_positions)]
 
         # CHORD
-        if self.additional_tokens["Chord"]:
+        if self.config.use_chords:
             vocab += self._create_chords_tokens()
 
         # REST
-        if self.additional_tokens["Rest"]:
+        if self.config.use_rests:
             vocab += [f'Rest_{".".join(map(str, rest))}' for rest in self.rests]
 
         # TEMPO
-        if self.additional_tokens["Tempo"]:
+        if self.config.use_tempos:
             vocab += [f"Tempo_{i}" for i in self.tempos]
 
         # PROGRAM
-        if self.additional_tokens["Program"]:
+        if self.config.use_programs:
             vocab += [f"Program_{program}" for program in range(-1, 128)]
 
         return vocab
 
     def _create_token_types_graph(self) -> Dict[str, List[str]]:
         r"""Returns a graph (as a dictionary) of the possible token
         types successions.
         NOTE: Program type is not referenced here, you can add it manually by
         modifying the tokens_types_graph class attribute following your strategy.
 
         :return: the token types transitions dictionary
         """
         dic = dict()
 
+        dic["Bar"] = ["Position", "Bar"]
+
+        dic["Position"] = ["Pitch"]
         dic["Pitch"] = ["Velocity"]
         dic["Velocity"] = ["Duration"]
-        dic["Duration"] = ["Pitch", "TimeShift"]
-        dic["TimeShift"] = ["Pitch"]
+        dic["Duration"] = ["Pitch", "Position", "Bar"]
+
+        if self.config.use_programs:
+            dic["Program"] = ["Bar"]
 
-        if self.additional_tokens["Chord"]:
+        if self.config.use_chords:
             dic["Chord"] = ["Pitch"]
-            dic["TimeShift"] += ["Chord"]
+            dic["Duration"] += ["Chord"]
+            dic["Position"] += ["Chord"]
 
-        if self.additional_tokens["Tempo"]:
-            dic["TimeShift"] += ["Tempo"]
-            dic["Tempo"] = ["Pitch", "TimeShift"]
-            if self.additional_tokens["Chord"]:
-                dic["Tempo"] += ["Chord"]
-
-        if self.additional_tokens["Rest"]:
-            dic["Rest"] = ["Rest", "Pitch", "TimeShift"]
-            if self.additional_tokens["Chord"]:
-                dic["Rest"] += ["Chord"]
+        if self.config.use_tempos:
+            dic["Tempo"] = ["Chord", "Pitch"] if self.config.use_chords else ["Pitch"]
+            dic["Position"] += ["Tempo"]
+
+        if self.config.use_rests:
+            dic["Rest"] = ["Rest", "Position", "Bar"]
             dic["Duration"] += ["Rest"]
 
         return dic
 
-    def token_types_errors_training(
-        self, x_tokens: List[int], y_tokens: List[int]
-    ) -> Tuple[Union[float, Any]]:
-        r"""Checks if a sequence of tokens is constituted of good token types
-        successions and returns the error ratio (lower is better).
-        The Pitch and Position values are also analyzed:
-            - a Pitch token should not be present if the same pitch is already being played
-
-        :param x_tokens: input tokens
-        :param y_tokens: produced token to check according to input
-        :return: the error ratio (lower is better)
-        """
-        err_type = 0
-        err_note = 0
-        current_pitches = []
-
-        for x_tok, y_tok in zip(x_tokens, y_tokens):
-            x_type, x_value = self[x_tok].split("_")
-            y_type, y_value = self[y_tok].split("_")
-            if x_type == "PAD":
-                break
-
-            if x_type == "Pitch":
-                current_pitches.append(int(x_value))
-            elif x_type in ["TimeShift", "Rest"]:
-                current_pitches = []  # moving in time, list reset
-
-            # Good token type
-            if y_type in self.tokens_types_graph[x_type]:
-                if y_type == "Pitch" and int(y_value) in current_pitches:
-                    err_note += 1  # pitch already being played
-            # Bad token type
-            else:
-                err_type += 1
-
-        return tuple(map(lambda err: err / len(x_tokens), (err_type, 0.0, err_note)))
-
     @staticmethod
     def _order(x: Event) -> int:
         r"""Helper function to sort events in the right order
 
         :param x: event to get order index
         :return: an order int
         """
         if x.type == "Program":
             return 0
-        elif x.type == "Tempo":
+        elif x.type == "Bar":
             return 1
-        elif x.type == "Chord":
+        elif x.type == "Position":
             return 2
-        elif x.type == "TimeShift" or x.type == "Rest":
-            return 1000  # always last
+        elif (
+            x.type == "Chord" or x.type == "Tempo"
+        ):  # actually object_list will be before chords
+            return 3
+        elif x.type == "Rest":
+            return 5
         else:  # for other types of events, the order should be handle when inserting the events in the sequence
             return 4
```

### Comparing `miditok-2.0.6/miditok/utils/utils.py` & `miditok-2.1.0/miditok/utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,36 +66,38 @@
 def detect_chords(
     notes: Sequence[Note],
     time_division: int,
     chord_maps: Dict[str, Sequence[int]],
     specify_root_note: bool = True,
     beat_res: int = 4,
     onset_offset: int = 1,
-    unknown_chords_nb_notes_range: Union[bool, Tuple[int]] = False,
+    unknown_chords_nb_notes_range: Tuple[int, int] = None,
     simul_notes_limit: int = 10,
 ) -> List[Event]:
     r"""Chord detection method. Make sure to sort notes by start time then pitch before:
     ``notes.sort(key=lambda x: (x.start, x.pitch))``.
-    **On very large tracks with high note density this method can slow down processes.**
+    **On very large tracks with high note density this method can be slow.**
     If you plan to use it with the Maestro or GiantMIDI datasets, it can take up to
     hundreds of seconds per MIDI depending on your cpu.
     This method works by iterating over each note, find if it played with other notes, and if it
     forms a chord from the chord maps. **It does not consider chord inversion.**
 
     :param notes: notes to analyse (sorted by starting time, them pitch)
     :param time_division: MIDI time division / resolution, in ticks/beat (of the MIDI being parsed)
     :param chord_maps: list of chord maps, to be given as a dictionary where keys are chord qualities
-                    (e.g. "maj") and values pitch maps as tuples of integers (e.g. (0, 4, 7)).
-                    You can use or take as an example ``miditok.constants.CHORD_MAPS``.
-    :param specify_root_note: the root note of each chord will be specified in Events / tokens (default: True).
+            (e.g. "maj") and values pitch maps as tuples of integers (e.g. (0, 4, 7)).
+            You can use ``miditok.constants.CHORD_MAPS`` as an example.
+    :param specify_root_note: the root note of each chord will be specified in Events / tokens.
+            Tokens will look as "Chord_C:maj". (default: True)
     :param beat_res: beat resolution, i.e. nb of samples per beat (default 4).
     :param onset_offset: maximum offset (in samples) ∈ N separating notes starts to consider them
-                    starting at the same time / onset (default is 1).
-    :param unknown_chords_nb_notes_range: will detect only chords recognized in the chord maps. If set to False,
-                    non recognized chords of *n* notes will give a *Chord_n* token (default False).
+            starting at the same time / onset (default is 1).
+    :param unknown_chords_nb_notes_range: range of number of notes to represent unknown chords.
+            If you want to represent chords that does not match any combination in ``chord_maps``, use this argument.
+            Leave ``None`` to not represent unknown chords. (default: None)
     :param simul_notes_limit: nb of simultaneous notes being processed when looking for a chord
             this parameter allows to speed up the chord detection, and must be >= 5 (default 10).
     :return: the detected chords as Event objects.
     """
     assert (
         simul_notes_limit >= 5
     ), "simul_notes_limit must be higher than 5, chords can be made up to 5 notes"
@@ -144,15 +146,15 @@
             for quality, known_chord in chord_maps.items():
                 if known_chord == chord_map:
                     chord_quality = quality
                     is_unknown_chord = False
                     break
 
             # We found a chord quality, or we specify unknown chords
-            if not (unknown_chords_nb_notes_range is False and is_unknown_chord):
+            if not (unknown_chords_nb_notes_range is not None and is_unknown_chord):
                 if specify_root_note:
                     chord_quality = (
                         f"{PITCH_CLASSES[notes[count, 0] % 12]}:{chord_quality}"
                     )
                 chords.append(
                     Event(
                         type="Chord",
@@ -298,15 +300,15 @@
         tracks_[0].pedals = sum((t.pedals for t in tracks_), [])
         tracks_[0].pedals.sort(key=lambda pedal: pedal.start)
         # Control changes
         tracks_[0].control_changes = sum((t.control_changes for t in tracks_), [])
         tracks_[0].control_changes.sort(key=lambda control_change: control_change.time)
         # Pitch bends
         tracks_[0].pitch_bends = sum((t.pitch_bends for t in tracks_), [])
-        tracks_[0].pitch_bends.sort(key=lambda pitch_bend: pitch_bend.start)
+        tracks_[0].pitch_bends.sort(key=lambda pitch_bend: pitch_bend.time)
 
     # Keeps only one track
     if isinstance(tracks, MidiFile):
         tracks.instruments = [tracks_[0]]
     else:
         for _ in range(1, len(tracks)):
             del tracks[1]
```

### Comparing `miditok-2.0.6/miditok.egg-info/PKG-INFO` & `miditok-2.1.0/miditok.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miditok
-Version: 2.0.6
+Version: 2.1.0
 Summary: A convenient MIDI tokenizer for Deep Learning networks, with multiple encoding strategies
 Home-page: https://github.com/Natooz/MidiTok
 Author: Nathan Fradet
 License: MIT
 Keywords: artificial intelligence,deep learning,transformer,midi,tokenization,music,mir
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -45,21 +45,24 @@
 MidiTok uses [MIDIToolkit](https://github.com/YatingMusic/miditoolkit), which itself uses [Mido](https://github.com/mido/mido) to read and write MIDI files, and BPE is backed by [Hugging Face 🤗tokenizers](https://github.com/huggingface/tokenizers) for super-fast encoding.
 
 ## Usage example
 
 The most basic and useful methods are summarized here. And [here](colab-notebooks/Full_Example_HuggingFace_GPT2_Transformer.ipynb) is a simple notebook example showing how to use Hugging Face models to generate music, with MidiTok taking care of tokenizing MIDIs.
 
 ```python
-from miditok import REMI
+from miditok import REMI, TokenizerConfig
 from miditok.utils import get_midi_programs
 from miditoolkit import MidiFile
 from pathlib import Path
 
+# Creating the tokenizer's configuration, read the doc to explore other parameters
+config = TokenizerConfig(nb_velocities=16, use_chords=True)
+
 # Creates the tokenizer and loads a MIDI
-tokenizer = REMI()  # using the default parameters, read the documentation to customize your tokenizer
+tokenizer = REMI(config)
 midi = MidiFile('path/to/your_midi.mid')
 
 # Converts MIDI to tokens, and back to a MIDI
 tokens = tokenizer(midi)  # calling it will automatically detect MIDIs, paths and tokens before the conversion
 converted_back_midi = tokenizer(tokens, get_midi_programs(midi))  # PyTorch / Tensorflow / Numpy tensors supported
 
 # Converts MIDI files to tokens saved as JSON files
@@ -72,15 +75,15 @@
 tokenizer.learn_bpe(
     vocab_size=500,
     tokens_paths=list(Path("path", "to", "tokens_noBPE").glob("**/*.json")),
     start_from_empty_voc=False,
 )
 
 # Saving our tokenizer, to retrieve it back later with the load_params method
-tokenizer.save_params(Path("path", "to", "save", "tokenizer"))
+tokenizer.save_params(Path("path", "to", "save", "tokenizer.json"))
 
 # Converts the tokenized musics into tokens with BPE
 tokenizer.apply_bpe_to_dataset(Path('path', 'to', 'tokens_noBPE'), Path('path', 'to', 'tokens_BPE'))
 ```
 
 ## Tokenizations
 
@@ -104,19 +107,20 @@
 
 ## Contributions
 
 Contributions are gratefully welcomed, feel free to open an issue or send a PR if you want to add a tokenization or speed up the code. You can read the [contribution guide](CONTRIBUTING.md) for details.
 
 ### Todos
 
-* Extend Time Signature to all tokenizations
-* Control Change messages
-* Option to represent pitch values as pitch intervals, as [it seems to improve performances](https://ismir2022program.ismir.net/lbd_369.html).
-* Speeding up MIDI read / load (Rust / C++ binding)
-* Data augmentation on duration values at the MIDI level
+* Option to place `Program` tokens before note tokens for *TSD*, "vanilla" *REMI*, *MIDI-Like* and *Structured*;
+* Extend Time Signature to all tokenizations;
+* Control Change messages;
+* Option to represent pitch values as pitch intervals, as [it seems to improve performances](https://ismir2022program.ismir.net/lbd_369.html);
+* Speeding up MIDI read / load (using a Rust / C++ io library + Python binding ?);
+* Data augmentation on duration values at the MIDI level.
 
 ## Citation
 
 If you use MidiTok for your research, a citation in your manuscript would be gladly appreciated. ❤️
 
 [**MidiTok paper**](https://archives.ismir.net/ismir2021/latebreaking/000005.pdf)
 ```bibtex
```

### Comparing `miditok-2.0.6/miditok.egg-info/SOURCES.txt` & `miditok-2.1.0/miditok.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -22,14 +22,13 @@
 miditok/tokenizations/remi.py
 miditok/tokenizations/remi_plus.py
 miditok/tokenizations/structured.py
 miditok/tokenizations/tsd.py
 miditok/utils/__init__.py
 miditok/utils/utils.py
 tests/test_bpe.py
-tests/test_bpe_slow.py
 tests/test_methods.py
 tests/test_multitrack.py
 tests/test_one_track.py
 tests/test_saving_loading_config.py
 tests/test_utils.py
 tests/tests_utils.py
```

### Comparing `miditok-2.0.6/setup.py` & `miditok-2.1.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
-    name='miditok',
-    author='Nathan Fradet',
-    url='https://github.com/Natooz/MidiTok',
+    name="miditok",
+    author="Nathan Fradet",
+    url="https://github.com/Natooz/MidiTok",
     packages=find_packages(exclude=("tests",)),
-    version='2.0.6',
-    license='MIT',
-    description='A convenient MIDI tokenizer for Deep Learning networks, with multiple encoding strategies',
+    version="2.1.0",
+    license="MIT",
+    description="A convenient MIDI tokenizer for Deep Learning networks, with multiple encoding strategies",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords=[
-        'artificial intelligence',
-        'deep learning',
-        'transformer',
-        'midi',
-        'tokenization',
-        'music',
-        'mir'
+        "artificial intelligence",
+        "deep learning",
+        "transformer",
+        "midi",
+        "tokenization",
+        "music",
+        "mir",
     ],
     install_requires=[
-        'numpy>=1.19,<1.24',
-        'miditoolkit>=0.1.16',
-        'tqdm'
+        "numpy>=1.19,<1.24",
+        "miditoolkit>=0.1.16",
+        "tqdm",
+        "tokenizers>=0.13.0",
+        "scipy",  # needed for miditoolkit
+        "matplotlib",  # needed for miditoolkit
     ],
     classifiers=[
-        'Intended Audience :: Developers',
-        'Intended Audience :: Science/Research',
-        'Topic :: Scientific/Engineering :: Artificial Intelligence',
-        'Topic :: Multimedia :: Sound/Audio :: MIDI',
-        'License :: OSI Approved :: MIT License',
+        "Intended Audience :: Developers",
+        "Intended Audience :: Science/Research",
+        "Topic :: Scientific/Engineering :: Artificial Intelligence",
+        "Topic :: Multimedia :: Sound/Audio :: MIDI",
+        "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
-        "Operating System :: OS Independent"
+        "Operating System :: OS Independent",
     ],
 )
```

### Comparing `miditok-2.0.6/tests/test_bpe.py` & `miditok-2.1.0/tests/test_bpe.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,20 +12,21 @@
 import miditok
 from miditoolkit import MidiFile
 from tqdm import tqdm
 
 # Special beat res for test, up to 64 beats so the duration and time-shift values are
 # long enough for MIDI-Like and Structured encodings, and with a single beat resolution
 BEAT_RES_TEST = {(0, 4): 8, (4, 12): 4}
-ADDITIONAL_TOKENS_TEST = {
-    "Chord": False,  # set false to speed up tests as it takes some time on maestro MIDIs
-    "Rest": True,
-    "Tempo": True,
-    "TimeSignature": True,
-    "Program": False,
+TOKENIZER_PARAMS = {
+    "beat_res": BEAT_RES_TEST,
+    "use_chords": False,  # set false to speed up tests as it takes some time on maestro MIDIs
+    "use_rests": True,
+    "use_tempos": True,
+    "use_time_signatures": True,
+    "use_programs": False,
     "rest_range": (4, 16),
     "nb_tempos": 32,
     "tempo_range": (40, 250),
     "time_signature_range": (16, 2),
 }
 
 
@@ -43,17 +44,17 @@
     data_path = Path(data_path)
     files = list(data_path.glob("**/*.mid"))
 
     # Creates tokenizers and computes BPE (build voc)
     first_tokenizers = []
     first_samples_bpe = {tok: [] for tok in tokenizations}
     for tokenization in tokenizations:
-        add_tokens = deepcopy(ADDITIONAL_TOKENS_TEST)
+        tokenizer_config = miditok.TokenizerConfig(**TOKENIZER_PARAMS)
         tokenizer: miditok.MIDITokenizer = getattr(miditok, tokenization)(
-            beat_res=BEAT_RES_TEST, additional_tokens=add_tokens
+            tokenizer_config=tokenizer_config
         )
         tokenizer.tokenize_midi_dataset(
             files, Path("tests", "test_results", tokenization)
         )
         tokenizer.learn_bpe(
             vocab_size=len(tokenizer) + 400,
             tokens_paths=list(
```

### Comparing `miditok-2.0.6/tests/test_methods.py` & `miditok-2.1.0/tests/test_methods.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 )
 from tensorflow import Tensor as tfTensor, convert_to_tensor
 
 import miditok
 
 
 def test_convert_tensors():
-    original = [[2, 6, 87, 89, 25, 15]]
+    original = [[2, 6, 95, 130, 25, 15]]
     types = [ptTensor, ptIntTensor, ptFloatTensor, tfTensor]
 
     tokenizer = miditok.TSD()
     for type_ in types:
         if type_ == tfTensor:
             tensor = convert_to_tensor(original)
         else:
```

### Comparing `miditok-2.0.6/tests/test_multitrack.py` & `miditok-2.1.0/tests/test_multitrack.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,26 +30,27 @@
     adapt_tempo_changes_times,
     time_signature_changes_equals,
 )
 
 # Special beat res for test, up to 16 beats so the duration and time-shift values are
 # long enough for MIDI-Like and Structured encodings, and with a single beat resolution
 BEAT_RES_TEST = {(0, 16): 8}
-ADDITIONAL_TOKENS_TEST = {
-    "Chord": True,
-    "Rest": True,
-    "Tempo": True,
-    "TimeSignature": True,
-    "Program": True,
+TOKENIZER_PARAMS = {
+    "beat_res": BEAT_RES_TEST,
+    "use_chords": True,
+    "use_rests": True,
+    "use_tempos": True,
+    "use_time_signatures": True,
+    "use_programs": True,
     "chord_maps": miditok.constants.CHORD_MAPS,
     "chord_tokens_with_root_note": True,  # Tokens will look as "Chord_C:maj"
     "chord_unknown": (3, 6),
     "rest_range": (
         4,
-        1024,
+        512,
     ),  # very high value to cover every possible rest in the test files
     "nb_tempos": 32,
     "tempo_range": (40, 250),
     "time_signature_range": (16, 2),
 }
 
 
@@ -59,14 +60,15 @@
 ):
     r"""Reads a few MIDI files, convert them into token sequences, convert them back to MIDI files.
     The converted back MIDI files should identical to original one, expect with note starting and ending
     times quantized, and maybe a some duplicated notes removed
 
     """
     tokenizations = [
+        "TSD",
         "REMI",
         "REMIPlus",
         "CPWord",
         "Octuple",
         "OctupleMono",
         "MuMIDI",
         "MMM",
@@ -83,32 +85,32 @@
         ):  # ValueError, OSError, FileNotFoundError, IOError, EOFError, mido.KeySignatureError
             continue
         if midi.ticks_per_beat % max(BEAT_RES_TEST.values()) != 0:
             continue
         has_errors = False
 
         for tokenization in tokenizations:
-            tokenizer = getattr(miditok, tokenization)(
-                beat_res=BEAT_RES_TEST,
-                additional_tokens=deepcopy(ADDITIONAL_TOKENS_TEST),
+            tokenizer_config = miditok.TokenizerConfig(**TOKENIZER_PARAMS)
+            tokenizer: miditok.MIDITokenizer = getattr(miditok, tokenization)(
+                tokenizer_config=tokenizer_config
             )
 
             # Process the MIDI
             midi_to_compare = deepcopy(
                 midi
             )  # midi notes / tempos / time signature quantized with the line above
             for track in midi_to_compare.instruments:
                 if track.is_drum:
                     track.program = (
                         0  # need to be done before sorting tracks per program
                     )
 
             # Sort and merge tracks if needed
             # MIDI produced with Octuple contains tracks ordered by program
-            if tokenization in ["Octuple", "MuMIDI", "REMIPlus"]:
+            if tokenizer.unique_track:
                 miditok.utils.merge_same_program_tracks(
                     midi_to_compare.instruments
                 )  # merge tracks
             for (
                 track
             ) in midi_to_compare.instruments:  # reduce the duration of notes to long
                 reduce_note_durations(
@@ -155,28 +157,28 @@
                     f"MIDI {i} - {file_path} failed to encode/decode NOTES with "
                     f"{tokenization} ({sum(len(t[2]) for t in errors)} errors)"
                 )
                 # return False
 
             # Checks tempos
             if (
-                tokenizer.additional_tokens["Tempo"] and tokenization != "MuMIDI"
+                tokenizer.config.use_tempos and tokenization != "MuMIDI"
             ):  # MuMIDI doesn't decode tempos
                 tempo_errors = tempo_changes_equals(
                     midi_to_compare.tempo_changes, new_midi.tempo_changes
                 )
                 if len(tempo_errors) > 0:
                     has_errors = True
                     print(
                         f"MIDI {i} - {file_path} failed to encode/decode TEMPO changes with "
                         f"{tokenization} ({len(tempo_errors)} errors)"
                     )
 
             # Checks time signatures
-            if tokenizer.additional_tokens["TimeSignature"] and tokenization in [
+            if tokenizer.config.use_time_signatures and tokenization in [
                 "Octuple",
                 "REMIPlus",
             ]:
                 time_sig_errors = time_signature_changes_equals(
                     midi_to_compare.time_signature_changes,
                     new_midi.time_signature_changes,
                 )
```

### Comparing `miditok-2.0.6/tests/test_one_track.py` & `miditok-2.1.0/tests/test_one_track.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,20 +23,21 @@
     tempo_changes_equals,
     time_signature_changes_equals,
 )
 
 # Special beat res for test, up to 64 beats so the duration and time-shift values are
 # long enough for MIDI-Like and Structured encodings, and with a single beat resolution
 BEAT_RES_TEST = {(0, 64): 8}
-ADDITIONAL_TOKENS_TEST = {
-    "Chord": False,  # set false to speed up tests as it takes some time on maestro MIDIs
-    "Rest": True,
-    "Tempo": True,
-    "TimeSignature": True,
-    "Program": False,
+TOKENIZER_PARAMS = {
+    "beat_res": BEAT_RES_TEST,
+    "use_chords": False,  # set false to speed up tests as it takes some time on maestro MIDIs
+    "use_rests": True,
+    "use_tempos": True,
+    "use_time_signatures": True,
+    "use_programs": False,
     "rest_range": (4, 16),
     "nb_tempos": 32,
     "tempo_range": (40, 250),
     "time_signature_range": (16, 2),
     "chord_maps": miditok.constants.CHORD_MAPS,
     "chord_tokens_with_root_note": True,  # Tokens will look as "Chord_C:maj"
     "chord_unknown": False,
@@ -72,42 +73,48 @@
     for i, file_path in enumerate(tqdm(files, desc="Testing One Track")):
         # Reads the midi
         midi = MidiFile(file_path)
         tracks = [deepcopy(midi.instruments[0])]
         has_errors = False
 
         for tokenization in tokenizations:
-            add_tokens = deepcopy(ADDITIONAL_TOKENS_TEST)
+            tokenizer_config = miditok.TokenizerConfig(**TOKENIZER_PARAMS)
             # Increase the number of rest just to cover very long pauses / rests in test examples
             if tokenization in ["MIDILike", "TSD"]:
-                add_tokens["rest_range"] = (
-                    add_tokens["rest_range"][0],
+                tokenizer_config.rest_range = (
+                    tokenizer_config.rest_range[0],
                     max(t[1] for t in BEAT_RES_TEST),
                 )
-            tokenizer = getattr(miditok, tokenization)(
-                beat_res=BEAT_RES_TEST,
-                additional_tokens=add_tokens,
+            tokenizer: miditok.MIDITokenizer = getattr(miditok, tokenization)(
+                tokenizer_config=tokenizer_config
             )
 
+            # printing the tokenizer shouldn't fail
+            _ = str(tokenizer)
+
             # Convert the track in tokens
             tokens = tokenizer(midi)
-            if not tokenizer.unique_track:  # or isinstance list
+            if (
+                not tokenizer.unique_track or tokenization == "TSD"
+            ):  # or isinstance list
                 tokens = tokens[0]
 
             # Checks types and values conformity following the rules
             tokens_types = tokenizer.tokens_errors(tokens)
             if tokens_types != 0.0:
                 print(
                     f"Validation of tokens types / values successions failed with {tokenization}: {tokens_types:.2f}"
                 )
 
             # Convert back tokens into a track object
             tempo_changes = None
             time_sig_changes = None
-            if tokenizer.unique_track:
+            if tokenizer.unique_track or tokenization == "TSD":
+                if tokenization == "TSD":
+                    tokens = [tokens]
                 new_midi = tokenizer.tokens_to_midi(
                     tokens, time_division=midi.ticks_per_beat
                 )
                 track = new_midi.instruments[0]
                 if tokenization == "Octuple":
                     tempo_changes = new_midi.tempo_changes
                     time_sig_changes = new_midi.time_signature_changes
@@ -132,28 +139,25 @@
                     f"MIDI {i} - {file_path} failed to encode/decode NOTES with {tokenization} ({len(errors)} errors)"
                 )
                 # return False
             track.name = f"encoded with {tokenization}"
             tracks.append(track)
 
             # Checks tempos
-            if tempo_changes is not None and tokenizer.additional_tokens["Tempo"]:
+            if tempo_changes is not None and tokenizer.config.use_tempos:
                 tempo_errors = tempo_changes_equals(midi.tempo_changes, tempo_changes)
                 if len(tempo_errors) > 0:
                     has_errors = True
                     print(
                         f"MIDI {i} - {file_path} failed to encode/decode TEMPO changes with "
                         f"{tokenization} ({len(tempo_errors)} errors)"
                     )
 
             # Checks time signatures
-            if (
-                time_sig_changes is not None
-                and tokenizer.additional_tokens["TimeSignature"]
-            ):
+            if time_sig_changes is not None and tokenizer.config.use_time_signatures:
                 time_sig_errors = time_signature_changes_equals(
                     midi.time_signature_changes, time_sig_changes
                 )
                 if len(time_sig_errors) > 0:
                     has_errors = True
                     print(
                         f"MIDI {i} - {file_path} failed to encode/decode TIME SIGNATURE changes with "
```

### Comparing `miditok-2.0.6/tests/test_saving_loading_config.py` & `miditok-2.1.0/tests/test_saving_loading_config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,59 +1,72 @@
 #!/usr/bin/python3 python
 
 """Tests to create tokenizers, save their config, and load it back.
 If all went well the tokenizer should be identical.
 
 """
 
-from copy import deepcopy
-
 import miditok
 
 
 ADDITIONAL_TOKENS_TEST = {
-    "Chord": False,  # set False to speed up tests as it takes some time on maestro MIDIs
-    "Rest": True,
-    "Tempo": True,
-    "TimeSignature": True,
-    "Program": False,
+    "use_chords": False,  # set False to speed up tests as it takes some time on maestro MIDIs
+    "use_rests": True,
+    "use_tempos": True,
+    "use_time_signatures": True,
+    "use_programs": False,
     "rest_range": (4, 16),
     "nb_tempos": 32,
     "tempo_range": (40, 250),
     "time_signature_range": (16, 2),
 }
+tokenizations = [
+    "MIDILike",
+    "TSD",
+    "Structured",
+    "REMI",
+    "REMIPlus",
+    "CPWord",
+    "Octuple",
+    "OctupleMono",
+    "MuMIDI",
+]
+
+
+def test_saving_loading_tokenizer_config():
+    for tokenization in tokenizations:
+        config1 = miditok.TokenizerConfig()
+        config1.save_to_json(f"./tests/configs/tok_conf_{tokenization}.json")
+
+        config2 = miditok.TokenizerConfig.load_from_json(
+            f"./tests/configs/tok_conf_{tokenization}.json"
+        )
+
+        assert config1 == config2
+        config1.pitch_range = (0, 777)
+        assert config1 != config2
 
 
 def test_saving_loading_tokenizer():
     r"""Tests to create tokenizers, save their config, and load it back.
     If all went well the tokenizer should be identical.
     """
-    tokenizations = [
-        "MIDILike",
-        "TSD",
-        "Structured",
-        "REMI",
-        "REMIPlus",
-        "CPWord",
-        "Octuple",
-        "OctupleMono",
-        "MuMIDI",
-    ]
 
     for tokenization in tokenizations:
-        add_tokens = deepcopy(ADDITIONAL_TOKENS_TEST)
+        tokenizer_config = miditok.TokenizerConfig(**ADDITIONAL_TOKENS_TEST)
         tokenizer: miditok.MIDITokenizer = getattr(miditok, tokenization)(
-            additional_tokens=add_tokens
+            tokenizer_config=tokenizer_config
         )
         tokenizer.save_params(f"./tests/configs/{tokenization}.txt")
 
         tokenizer2: miditok.MIDITokenizer = getattr(miditok, tokenization)(
             params=f"./tests/configs/{tokenization}.txt"
         )
         assert tokenizer == tokenizer2
         if tokenization == "Octuple":
             tokenizer.vocab[0]["PAD_None"] = 8
             assert tokenizer != tokenizer2
 
 
 if __name__ == "__main__":
+    test_saving_loading_tokenizer_config()
     test_saving_loading_tokenizer()
```

### Comparing `miditok-2.0.6/tests/test_utils.py` & `miditok-2.1.0/tests/test_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,14 +22,24 @@
 def test_merge_tracks():
     midi = MidiFile(Path("tests", "Maestro_MIDIs", "Maestro_1.mid"))
     original_track = deepcopy(midi.instruments[0])
     midi.instruments.append(deepcopy(midi.instruments[0]))
     merge_tracks(midi.instruments)
     assert len(midi.instruments[0].notes) == 2 * len(original_track.notes)
 
+    # Test merge with effects
+    midi.instruments.append(deepcopy(midi.instruments[0]))
+    merge_tracks(midi, effects=True)
+    assert len(midi.instruments[0].notes) == 4 * len(original_track.notes)
+    assert len(midi.instruments[0].pedals) == 2 * len(original_track.pedals)
+    assert len(midi.instruments[0].control_changes) == 2 * len(
+        original_track.control_changes
+    )
+    assert len(midi.instruments[0].pitch_bends) == 2 * len(original_track.pitch_bends)
+
 
 def test_merge_same_program_tracks_and_by_class():
     multitrack_midi_paths = list(Path("tests", "Multitrack_MIDIs").glob("**/*.mid"))
     for midi_path in multitrack_midi_paths:
         midi = MidiFile(midi_path)
         for track in midi.instruments:
             if track.is_drum:
```

### Comparing `miditok-2.0.6/tests/tests_utils.py` & `miditok-2.1.0/tests/tests_utils.py`

 * *Files identical despite different names*

