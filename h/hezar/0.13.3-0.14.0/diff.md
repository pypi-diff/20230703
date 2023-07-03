# Comparing `tmp/hezar-0.13.3.tar.gz` & `tmp/hezar-0.14.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hezar-0.13.3.tar", max compression
+gzip compressed data, was "hezar-0.14.0.tar", max compression
```

## Comparing `hezar-0.13.3.tar` & `hezar-0.14.0.tar`

### file list

```diff
@@ -1,73 +1,77 @@
--rw-r--r--   0        0        0     1065 2023-06-30 06:57:28.300613 hezar-0.13.3/LICENSE
--rw-r--r--   0        0        0     4227 2023-06-30 06:57:28.300613 hezar-0.13.3/README.md
--rw-r--r--   0        0        0      238 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/__init__.py
--rw-r--r--   0        0        0     6271 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/builders.py
--rw-r--r--   0        0        0    10248 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/configs.py
--rw-r--r--   0        0        0      740 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/constants.py
--rw-r--r--   0        0        0       75 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/data/__init__.py
--rw-r--r--   0        0        0     3708 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/data/data_collators.py
--rw-r--r--   0        0        0      129 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/data/datasets/__init__.py
--rw-r--r--   0        0        0      339 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/data/datasets/dataset.py
--rw-r--r--   0        0        0     3177 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/data/datasets/text_classification_dataset.py
--rw-r--r--   0        0        0       26 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/data/utils/__init__.py
--rw-r--r--   0        0        0     1547 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/data/utils/data_utils.py
--rw-r--r--   0        0        0      127 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/embeddings/__init__.py
--rw-r--r--   0        0        0     4146 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/embeddings/embedding.py
--rw-r--r--   0        0        0     3122 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/embeddings/fasttext.py
--rw-r--r--   0        0        0     3081 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/embeddings/word2vec.py
--rw-r--r--   0        0        0      282 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/audio_classification/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/image2text/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/image2text/crnn/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/image2text/trocr/__init__.py
--rw-r--r--   0        0        0      144 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/language_modeling/__init__.py
--rw-r--r--   0        0        0       69 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/language_modeling/bert/__init__.py
--rw-r--r--   0        0        0     1136 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/language_modeling/bert/bert_lm.py
--rw-r--r--   0        0        0      720 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/language_modeling/bert/bert_lm_config.py
--rw-r--r--   0        0        0       93 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/language_modeling/distilbert/__init__.py
--rw-r--r--   0        0        0     1208 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/language_modeling/distilbert/distilbert_lm.py
--rw-r--r--   0        0        0      586 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/language_modeling/distilbert/distilbert_lm_config.py
--rw-r--r--   0        0        0       81 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/language_modeling/roberta/__init__.py
--rw-r--r--   0        0        0     1172 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/language_modeling/roberta/roberta_lm.py
--rw-r--r--   0        0        0      780 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/language_modeling/roberta/roberta_lm_config.py
--rw-r--r--   0        0        0     9544 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/model.py
--rw-r--r--   0        0        0        0 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/sequence_labeling/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/speech_recognition/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/speech_recognition/wav2vec/__init__.py
--rw-r--r--   0        0        0      240 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/text_classification/__init__.py
--rw-r--r--   0        0        0      135 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/text_classification/bert/__init__.py
--rw-r--r--   0        0        0     2679 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/text_classification/bert/bert_text_classification.py
--rw-r--r--   0        0        0      808 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/text_classification/bert/bert_text_classification_config.py
--rw-r--r--   0        0        0      159 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/text_classification/distilbert/__init__.py
--rw-r--r--   0        0        0     2813 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/text_classification/distilbert/distilbert_text_classification.py
--rw-r--r--   0        0        0      711 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py
--rw-r--r--   0        0        0      147 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/text_classification/roberta/__init__.py
--rw-r--r--   0        0        0     2943 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/text_classification/roberta/roberta_text_classification.py
--rw-r--r--   0        0        0      905 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/text_classification/roberta/roberta_text_classification_config.py
--rw-r--r--   0        0        0        0 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/text_detection/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/text_detection/ctpn/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/text_detection/dbnet/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/models/text_summarization/__init__.py
--rw-r--r--   0        0        0      104 2023-06-30 06:57:28.300613 hezar-0.13.3/hezar/preprocessors/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 06:57:28.304613 hezar-0.13.3/hezar/preprocessors/normalizers/__init__.py
--rw-r--r--   0        0        0        0 2023-06-30 06:57:28.304613 hezar-0.13.3/hezar/preprocessors/normalizers/nfkc.py
--rw-r--r--   0        0        0        0 2023-06-30 06:57:28.304613 hezar-0.13.3/hezar/preprocessors/normalizers/nfkd.py
--rw-r--r--   0        0        0        0 2023-06-30 06:57:28.304613 hezar-0.13.3/hezar/preprocessors/normalizers/normalizer.py
--rw-r--r--   0        0        0     2218 2023-06-30 06:57:28.304613 hezar-0.13.3/hezar/preprocessors/preprocessor.py
--rw-r--r--   0        0        0      298 2023-06-30 06:57:28.304613 hezar-0.13.3/hezar/preprocessors/tokenizers/__init__.py
--rw-r--r--   0        0        0     4623 2023-06-30 06:57:28.304613 hezar-0.13.3/hezar/preprocessors/tokenizers/bpe.py
--rw-r--r--   0        0        0     5181 2023-06-30 06:57:28.304613 hezar-0.13.3/hezar/preprocessors/tokenizers/sentencepiece_bpe.py
--rw-r--r--   0        0        0    15394 2023-06-30 06:57:28.304613 hezar-0.13.3/hezar/preprocessors/tokenizers/tokenizer.py
--rw-r--r--   0        0        0     4215 2023-06-30 06:57:28.304613 hezar-0.13.3/hezar/preprocessors/tokenizers/wordpiece.py
--rw-r--r--   0        0        0     7443 2023-06-30 06:57:28.304613 hezar-0.13.3/hezar/registry.py
--rw-r--r--   0        0        0       29 2023-06-30 06:57:28.304613 hezar-0.13.3/hezar/trainers/__init__.py
--rw-r--r--   0        0        0    13853 2023-06-30 06:57:28.304613 hezar-0.13.3/hezar/trainers/trainer.py
--rw-r--r--   0        0        0     1773 2023-06-30 06:57:28.304613 hezar-0.13.3/hezar/trainers/trainer_utils.py
--rw-r--r--   0        0        0      135 2023-06-30 06:57:28.304613 hezar-0.13.3/hezar/utils/__init__.py
--rw-r--r--   0        0        0     2435 2023-06-30 06:57:28.304613 hezar-0.13.3/hezar/utils/config_utils.py
--rw-r--r--   0        0        0      482 2023-06-30 06:57:28.304613 hezar-0.13.3/hezar/utils/context_managers.py
--rw-r--r--   0        0        0     2773 2023-06-30 06:57:28.304613 hezar-0.13.3/hezar/utils/hub_utils.py
--rw-r--r--   0        0        0      374 2023-06-30 06:57:28.304613 hezar-0.13.3/hezar/utils/logging.py
--rw-r--r--   0        0        0        0 2023-06-30 06:57:28.304613 hezar-0.13.3/hezar/utils/model_utils.py
--rw-r--r--   0        0        0     1579 2023-06-30 06:57:28.304613 hezar-0.13.3/pyproject.toml
--rw-r--r--   0        0        0     6604 1970-01-01 00:00:00.000000 hezar-0.13.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-03 15:56:20.320494 hezar-0.14.0/LICENSE
+-rw-r--r--   0        0        0     4406 2023-07-03 15:56:20.320494 hezar-0.14.0/README.md
+-rw-r--r--   0        0        0      238 2023-07-03 15:56:20.320494 hezar-0.14.0/hezar/__init__.py
+-rw-r--r--   0        0        0     6481 2023-07-03 15:56:20.320494 hezar-0.14.0/hezar/builders.py
+-rw-r--r--   0        0        0    10446 2023-07-03 15:56:20.320494 hezar-0.14.0/hezar/configs.py
+-rw-r--r--   0        0        0     1110 2023-07-03 15:56:20.320494 hezar-0.14.0/hezar/constants.py
+-rw-r--r--   0        0        0       75 2023-07-03 15:56:20.320494 hezar-0.14.0/hezar/data/__init__.py
+-rw-r--r--   0        0        0     6333 2023-07-03 15:56:20.320494 hezar-0.14.0/hezar/data/data_collators.py
+-rw-r--r--   0        0        0      223 2023-07-03 15:56:20.320494 hezar-0.14.0/hezar/data/datasets/__init__.py
+-rw-r--r--   0        0        0     1608 2023-07-03 15:56:20.320494 hezar-0.14.0/hezar/data/datasets/dataset.py
+-rw-r--r--   0        0        0     4576 2023-07-03 15:56:20.320494 hezar-0.14.0/hezar/data/datasets/sequence_labeling_dataset.py
+-rw-r--r--   0        0        0     3701 2023-07-03 15:56:20.320494 hezar-0.14.0/hezar/data/datasets/text_classification_dataset.py
+-rw-r--r--   0        0        0       26 2023-07-03 15:56:20.320494 hezar-0.14.0/hezar/data/utils/__init__.py
+-rw-r--r--   0        0        0     1856 2023-07-03 15:56:20.320494 hezar-0.14.0/hezar/data/utils/data_utils.py
+-rw-r--r--   0        0        0      127 2023-07-03 15:56:20.320494 hezar-0.14.0/hezar/embeddings/__init__.py
+-rw-r--r--   0        0        0     4124 2023-07-03 15:56:20.320494 hezar-0.14.0/hezar/embeddings/embedding.py
+-rw-r--r--   0        0        0     3122 2023-07-03 15:56:20.320494 hezar-0.14.0/hezar/embeddings/fasttext.py
+-rw-r--r--   0        0        0     3081 2023-07-03 15:56:20.320494 hezar-0.14.0/hezar/embeddings/word2vec.py
+-rw-r--r--   0        0        0      282 2023-07-03 15:56:20.320494 hezar-0.14.0/hezar/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 15:56:20.320494 hezar-0.14.0/hezar/models/audio_classification/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 15:56:20.320494 hezar-0.14.0/hezar/models/image2text/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 15:56:20.320494 hezar-0.14.0/hezar/models/image2text/crnn/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 15:56:20.320494 hezar-0.14.0/hezar/models/image2text/trocr/__init__.py
+-rw-r--r--   0        0        0      144 2023-07-03 15:56:20.320494 hezar-0.14.0/hezar/models/language_modeling/__init__.py
+-rw-r--r--   0        0        0       69 2023-07-03 15:56:20.320494 hezar-0.14.0/hezar/models/language_modeling/bert/__init__.py
+-rw-r--r--   0        0        0     1136 2023-07-03 15:56:20.320494 hezar-0.14.0/hezar/models/language_modeling/bert/bert_lm.py
+-rw-r--r--   0        0        0      762 2023-07-03 15:56:20.320494 hezar-0.14.0/hezar/models/language_modeling/bert/bert_lm_config.py
+-rw-r--r--   0        0        0       93 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/models/language_modeling/distilbert/__init__.py
+-rw-r--r--   0        0        0     1208 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/models/language_modeling/distilbert/distilbert_lm.py
+-rw-r--r--   0        0        0      628 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/models/language_modeling/distilbert/distilbert_lm_config.py
+-rw-r--r--   0        0        0       81 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/models/language_modeling/roberta/__init__.py
+-rw-r--r--   0        0        0     1172 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/models/language_modeling/roberta/roberta_lm.py
+-rw-r--r--   0        0        0      822 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/models/language_modeling/roberta/roberta_lm_config.py
+-rw-r--r--   0        0        0     9544 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/models/model.py
+-rw-r--r--   0        0        0       67 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/models/sequence_labeling/__init__.py
+-rw-r--r--   0        0        0      127 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/models/sequence_labeling/bert/__init__.py
+-rw-r--r--   0        0        0     2853 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py
+-rw-r--r--   0        0        0      936 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py
+-rw-r--r--   0        0        0        0 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/models/speech_recognition/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/models/speech_recognition/wav2vec/__init__.py
+-rw-r--r--   0        0        0      240 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/models/text_classification/__init__.py
+-rw-r--r--   0        0        0      135 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/models/text_classification/bert/__init__.py
+-rw-r--r--   0        0        0     2679 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/models/text_classification/bert/bert_text_classification.py
+-rw-r--r--   0        0        0      850 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/models/text_classification/bert/bert_text_classification_config.py
+-rw-r--r--   0        0        0      159 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/models/text_classification/distilbert/__init__.py
+-rw-r--r--   0        0        0     2813 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/models/text_classification/distilbert/distilbert_text_classification.py
+-rw-r--r--   0        0        0      753 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py
+-rw-r--r--   0        0        0      147 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/models/text_classification/roberta/__init__.py
+-rw-r--r--   0        0        0     2943 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/models/text_classification/roberta/roberta_text_classification.py
+-rw-r--r--   0        0        0      947 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/models/text_classification/roberta/roberta_text_classification_config.py
+-rw-r--r--   0        0        0        0 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/models/text_detection/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/models/text_detection/ctpn/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/models/text_detection/dbnet/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/models/text_summarization/__init__.py
+-rw-r--r--   0        0        0      104 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/preprocessors/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/preprocessors/normalizers/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/preprocessors/normalizers/nfkc.py
+-rw-r--r--   0        0        0        0 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/preprocessors/normalizers/nfkd.py
+-rw-r--r--   0        0        0        0 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/preprocessors/normalizers/normalizer.py
+-rw-r--r--   0        0        0     2218 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/preprocessors/preprocessor.py
+-rw-r--r--   0        0        0      298 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/preprocessors/tokenizers/__init__.py
+-rw-r--r--   0        0        0     4623 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/preprocessors/tokenizers/bpe.py
+-rw-r--r--   0        0        0     5181 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/preprocessors/tokenizers/sentencepiece_bpe.py
+-rw-r--r--   0        0        0    18892 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/preprocessors/tokenizers/tokenizer.py
+-rw-r--r--   0        0        0     4215 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/preprocessors/tokenizers/wordpiece.py
+-rw-r--r--   0        0        0     8244 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/registry.py
+-rw-r--r--   0        0        0       29 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/trainers/__init__.py
+-rw-r--r--   0        0        0    13853 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/trainers/trainer.py
+-rw-r--r--   0        0        0     1773 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/trainers/trainer_utils.py
+-rw-r--r--   0        0        0      135 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/utils/__init__.py
+-rw-r--r--   0        0        0     3468 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/utils/config_utils.py
+-rw-r--r--   0        0        0      482 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/utils/context_managers.py
+-rw-r--r--   0        0        0     2773 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/utils/hub_utils.py
+-rw-r--r--   0        0        0      374 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/utils/logging.py
+-rw-r--r--   0        0        0        0 2023-07-03 15:56:20.324494 hezar-0.14.0/hezar/utils/model_utils.py
+-rw-r--r--   0        0        0     1579 2023-07-03 15:56:20.324494 hezar-0.14.0/pyproject.toml
+-rw-r--r--   0        0        0     6783 1970-01-01 00:00:00.000000 hezar-0.14.0/PKG-INFO
```

### Comparing `hezar-0.13.3/LICENSE` & `hezar-0.14.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hezar-0.13.3/README.md` & `hezar-0.14.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,20 @@
 - has a highly developer-friendly interface
 - has a task-based model interface which is more convenient for general users.
 - is packed with additional tools like word embeddings, tokenizers, feature extractors, etc.
 - comes with a lot of supplementary ML tools for deployment, benchmarking, optimization, etc.
 - and more!
 
 ## Installation
-Clone the repo and run:
+Hezar is available on PyPI and can be installed with pip:
+```commandline
+pip install hezar
+```
+You can also install the latest version from the source.
+Clone the repo and execute the following commands:
 ```commandline
 git clone https://github.com/hezarai/hezar.git
 pip install ./hezar
 ```
 
 ## Quick Tour
 ### Ready-to-use models from Hub
```

### Comparing `hezar-0.13.3/hezar/builders.py` & `hezar-0.14.0/hezar/builders.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,37 +6,45 @@
 Examples:
 
     >>> from hezar.builders import build_model
     >>> model = build_model('distilbert_text_classification', id2label={0: 'negative', 1: 'positive'})
     >>> print(model)
 
 """
+from typing import Optional
 
+from .configs import (
+    DatasetConfig,
+    EmbeddingConfig,
+    ModelConfig,
+    PreprocessorConfig,
+)
 from .registry import (  # noqa
-    models_registry,  # noqa
-    preprocessors_registry,  # noqa
-    datasets_registry,  # noqa
-    embeddings_registry, # noqa
     criterions_registry,  # noqa
-    optimizers_registry,  # noqa
+    datasets_registry,  # noqa
+    embeddings_registry,  # noqa
     lr_schedulers_registry,  # noqa
+    models_registry,  # noqa
+    optimizers_registry,  # noqa
+    preprocessors_registry,  # noqa
 )
 
+
 __all__ = [
     "build_model",
     "build_dataset",
     "build_preprocessor",
     "build_embedding",
     "build_optimizer",
     "build_criterion",
     "build_scheduler",
 ]
 
 
-def build_model(name: str, config=None, **kwargs):
+def build_model(name: str, config: Optional[ModelConfig] = None, **kwargs):
     """
     Build the model using its registry name. If config is None then the model is built using the default config. Notice
     that this function only builds the model and does not perform any weights loading/initialization unless these
     actions are done in the model's :func:`__init__` .
 
     Args:
         name (str): name of the model in the models' registry
@@ -45,20 +53,20 @@
 
     Returns:
         A Model instance
     """
     if name not in models_registry:
         raise ValueError(f"Unknown model name: `{name}`!\n"
                          f"Available model names: {list(models_registry.keys())}")
-    config = config or models_registry[name]["config_class"]()
-    model = models_registry[name]["model_class"](config, **kwargs)
+    config = config or models_registry[name].config_class()
+    model = models_registry[name].module_class(config, **kwargs)
     return model
 
 
-def build_preprocessor(name: str, config=None, **kwargs):
+def build_preprocessor(name: str, config: Optional[PreprocessorConfig] = None, **kwargs):
     """
     Build the preprocessor using its registry name. If config is None then the preprocessor is built using the
     default config.
 
     Args:
         name (str): name of the preprocessor in the preprocessors' registry
         config (PreprocessorConfig): a PreprocessorConfig instance
@@ -66,20 +74,20 @@
 
     Returns:
         A Preprocessor instance
     """
     if name not in preprocessors_registry:
         raise ValueError(f"Unknown preprocessor name: `{name}`!\n"
                          f"Available preprocessor names: {list(preprocessors_registry.keys())}")
-    config = config or preprocessors_registry[name]["config_class"]()
-    preprocessor = preprocessors_registry[name]["preprocessor_class"](config, **kwargs)
+    config = config or preprocessors_registry[name].config_class()
+    preprocessor = preprocessors_registry[name].module_class(config, **kwargs)
     return preprocessor
 
 
-def build_dataset(name: str, config=None, split=None, **kwargs):
+def build_dataset(name: str, config: Optional[DatasetConfig] = None, split=None, **kwargs):
     """
     Build the dataset using its registry name. If config is None then the dataset is built using the
     default config.
 
     Args:
         name (str): name of the dataset in the datasets' registry
         config (DatasetConfig): a DatasetConfig instance
@@ -88,20 +96,20 @@
 
     Returns:
         A Dataset instance
     """
     if name not in datasets_registry:
         raise ValueError(f"Unknown dataset name: `{name}`!\n"
                          f"Available dataset names: {list(datasets_registry.keys())}")
-    config = config or datasets_registry[name]["config_class"]()
-    dataset = datasets_registry[name]["dataset_class"](config, split=split, **kwargs)
+    config = config or datasets_registry[name].config_class()
+    dataset = datasets_registry[name].module_class(config, split, **kwargs)
     return dataset
 
 
-def build_embedding(name: str, config=None, **kwargs):
+def build_embedding(name: str, config: Optional[EmbeddingConfig] = None, **kwargs):
     """
     Build the embedding using its registry name. If config is None then the embedding is built using the
     default config.
 
     Args:
         name (str): Name of the embedding in the embeddings' registry
         config (EmbeddingConfig): An EmbeddingConfig instance
@@ -109,16 +117,16 @@
 
     Returns:
         A Dataset instance
     """
     if name not in embeddings_registry:
         raise ValueError(f"Unknown embedding name: `{name}`!\n"
                          f"Available embedding names: {list(embeddings_registry.keys())}")
-    config = config or embeddings_registry[name]["config_class"]()
-    embedding = embeddings_registry[name]["embedding_class"](config, **kwargs)
+    config = config or embeddings_registry[name].config_class()
+    embedding = embeddings_registry[name].module_class(config, **kwargs)
     return embedding
 
 
 def build_criterion(name: str, **kwargs):
     """
     Build the loss function using its registry name.
```

### Comparing `hezar-0.13.3/hezar/configs.py` & `hezar-0.14.0/hezar/configs.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from dataclasses import asdict, dataclass, field
 from typing import Any, Dict, List, Optional, Union
 
 import torch
 from huggingface_hub import create_repo, hf_hub_download, upload_file
 from omegaconf import DictConfig, OmegaConf
 
-from .constants import DEFAULT_MODEL_CONFIG_FILE, HEZAR_CACHE_DIR
+from .constants import DEFAULT_MODEL_CONFIG_FILE, HEZAR_CACHE_DIR, TaskType
 from .utils import get_logger, get_module_config_class
 
 
 __all__ = [
     "Config",
     "ModelConfig",
     "PreprocessorConfig",
@@ -104,23 +104,25 @@
 
     @classmethod
     def load(
         cls,
         hub_or_local_path: Union[str, os.PathLike],
         filename: Optional[str] = None,
         subfolder: Optional[str] = None,
+        repo_type=None,
         **kwargs,
     ):
         """
         Load config from Hub or locally if it already exists on disk (handled by HfApi)
 
         Args:
             hub_or_local_path: Local or Hub path for the config
             filename: Configuration filename
             subfolder: Optional subfolder path where the config is in
+            repo_type: Repo type e.g, model, dataset, etc
             **kwargs: Manual config parameters to override
 
         Returns:
             A Config instance
         """
         filename = filename or DEFAULT_MODEL_CONFIG_FILE
         subfolder = subfolder or ""
@@ -134,14 +136,15 @@
         # if the file or repo_id does not exist locally, load from the Hub
         if not is_local:
             config_path = hf_hub_download(
                 hub_or_local_path,
                 filename=filename,
                 subfolder=subfolder,
                 cache_dir=HEZAR_CACHE_DIR,
+                repo_type=repo_type,
             )
 
         dict_config = OmegaConf.load(config_path)
         config = OmegaConf.to_container(dict_config)
         config_cls = get_module_config_class(config["name"], config_type=config["config_type"])
         config = config_cls.from_dict(config, strict=False, **kwargs)
         return config
@@ -208,14 +211,15 @@
         # push to hub
         if commit_message is None:
             commit_message = f"Hezar: Upload {filename}"
         upload_file(
             path_or_fileobj=config_path,
             path_in_repo=path_in_repo,
             repo_id=repo_id,
+            repo_type=repo_type,
             commit_message=commit_message,
         )
         logger.info(
             f"Uploaded:`{self.__class__.__name__}(name={self.name})` --> `{os.path.join(repo_id, subfolder, filename)}`"
         )
 
 
@@ -240,15 +244,15 @@
 @dataclass
 class DatasetConfig(Config):
     """
     Base dataclass for all dataset configs
     """
     name: str = field(default=None, metadata={"help": "The dataset's key in the datasets_registry"})
     config_type: str = "dataset"
-    task: Union[str, List[str]] = field(
+    task: Union[TaskType, List[TaskType]] = field(
         default=None, metadata={"help": "Name of the task(s) this dataset is built for"}
     )
 
 
 @dataclass
 class EmbeddingConfig(Config):
     """
@@ -295,14 +299,15 @@
 @dataclass
 class TrainConfig(Config):
     """
     Base dataclass for all trainer configs
     """
     name: str = field(default=None, metadata={"help": "The trainer's key in the trainers_registry"})
     config_type: str = "train"
+    task: TaskType = None
     device: str = "cuda"
     init_weights_from: str = None
     seed: int = 42
     optimizer: Union[Dict[str, Any], OptimizerConfig] = None
     batch_size: int = None
     use_amp: bool = False
     metrics: Dict[str, Dict] = field(default_factory=dict)
```

### Comparing `hezar-0.13.3/hezar/data/datasets/text_classification_dataset.py` & `hezar-0.14.0/hezar/data/datasets/text_classification_dataset.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 from dataclasses import dataclass
 from typing import Dict, List, Tuple
 
 import torch
 from datasets import load_dataset
 
 from ...configs import DatasetConfig
+from ...constants import TaskType
 from ...preprocessors import Sequential, Tokenizer
 from ...registry import register_dataset
+from ...utils import get_logger
 from ..data_collators import TextPaddingDataCollator
 from .dataset import Dataset
 
 
+logger = get_logger(__name__)
+
+
 @dataclass
 class TextClassificationDatasetConfig(DatasetConfig):
     name: str = "text_classification"
-    task: str = "text_classification"
+    task: str = TaskType.TEXT_CLASSIFICATION
     path: str = None
     normalizers: List[Tuple[str, Dict]] = None
     tokenizer_path: str = None
     label_field: str = None
     text_field: str = None
     max_length: int = None
 
@@ -35,15 +40,15 @@
         **kwargs: Extra config parameters to assign to the original config
     """
 
     def __init__(self, config: TextClassificationDatasetConfig, split=None, **kwargs):
         super().__init__(config, **kwargs)
         self.dataset = self._load(split)
         self._extract_labels()
-        self.tokenizer = Tokenizer.load(self.config.tokenizer_path)
+        self.tokenizer = self._build_tokenizer()
         self.normalizer = Sequential(self.config.normalizers)
         self.data_collator = TextPaddingDataCollator(
             tokenizer=self.tokenizer,
             max_length=self.config.max_length,
         )
 
     def _load(self, split):
@@ -56,14 +61,23 @@
         Returns:
             The whole dataset
         """
         # TODO: In case we want to make this class work on other types like csv, json, etc. we have to do it here.
         dataset = load_dataset(self.config.path, split=split)
         return dataset
 
+    def _build_tokenizer(self):
+        if self.config.tokenizer_path:
+            tokenizer = Tokenizer.load(self.config.tokenizer_path)
+        else:
+            logger.warning("This dataset requires a tokenizer to work. Provide it in config as `tokenizer_path` "
+                           "or set it manually as `dataset.tokenizer = your_tokenizer` after building the dataset.")
+            tokenizer = None
+        return tokenizer
+
     def _extract_labels(self):
         """
         Extract label names, ids and build dictionaries
         """
         labels_list = self.dataset.features[self.config.label_field].names
         self.id2label = self.config.id2label = {k: str(v) for k, v in dict(list(enumerate(labels_list))).items()}
         self.label2id = self.config.label2id = {v: k for k, v in self.id2label.items()}
```

### Comparing `hezar-0.13.3/hezar/data/utils/data_utils.py` & `hezar-0.14.0/hezar/data/utils/data_utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,59 +1,70 @@
 from typing import Any, Dict
 
 
 __all__ = [
     "convert_batch_dict_dtype",
-    "get_str_keys",
+    "get_non_numeric_keys",
 ]
 
 
-def convert_batch_dict_dtype(batch_dict: Dict[str, Any], dtype: str = "list", skip: list = None):
+def convert_batch_dict_dtype(batch_dict: Dict[str, Any], dtype: str = None, skip_keys: list = None):
     """
     Convert data dtypes of the values in a batch dict
 
     Args:
         batch_dict: The batched dictionary
         dtype: Target data type to convert to
-        skip: A list of key names to skip conversion
+        skip_keys: A list of key names to skip conversion
 
     Returns:
         The same dict with cast values
     """
     import numpy as np
     import torch
 
-    skip = skip or []
-    skip += get_str_keys(batch_dict)
+    dtype = dtype or "list"
+    skip_keys = skip_keys or []
+
     if dtype == "list":
         for k, v in batch_dict.items():
             if isinstance(v, np.ndarray):
                 batch_dict[k] = v.tolist()
             elif isinstance(v, torch.Tensor):
                 batch_dict[k] = v.numpy().tolist()
         return batch_dict
-    caster = np.ndarray if dtype in ["np", "numpy"] else torch.tensor
+
+    if dtype in ["np", "numpy"]:
+        caster = np.ndarray
+    elif dtype in ["pt", "torch", "pytorch"]:
+        caster = torch.tensor
+    else:
+        raise ValueError(f"Invalid `dtype`: {dtype}")
+
     for k, v in batch_dict.items():
-        if k not in skip:
-            batch_dict[k] = caster(v)
+        if k not in skip_keys:
+            try:
+                batch_dict[k] = caster(v)
+            except Exception as e:  # noqa
+                continue
     return batch_dict
 
 
-def get_str_keys(d: Dict, batched=True):
+def get_non_numeric_keys(d: Dict, batched=True):
     """
     Get keys that have string values in a dictionary
 
     Args:
         d: The dict
         batched: Are the input dict values batched or not
 
     Returns:
         A list of string-valued keys
     """
     keys = []
     for k, v in d.items():
         if len(v) and isinstance(v[0], list):
-            if batched and isinstance(v[0][0], str):
+            if batched and not isinstance(v[0][0], (int, float, complex)) and not isinstance(v[0][0], bool):
                 keys.append(k)
             elif isinstance(v[0], str):
                 keys.append(k)
     return keys
```

### Comparing `hezar-0.13.3/hezar/embeddings/embedding.py` & `hezar-0.14.0/hezar/embeddings/embedding.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from ..builders import build_embedding
 from ..configs import EmbeddingConfig
 from ..constants import (
     DEFAULT_EMBEDDING_CONFIG_FILE,
     DEFAULT_EMBEDDING_FILE,
     DEFAULT_EMBEDDING_SUBFOLDER,
 )
-from ..utils import get_local_cache_path, get_logger
+from ..utils import get_logger
 
 
 logger = get_logger(__name__)
 
 
 class Embedding:
     """
```

### Comparing `hezar-0.13.3/hezar/embeddings/fasttext.py` & `hezar-0.14.0/hezar/embeddings/fasttext.py`

 * *Files identical despite different names*

### Comparing `hezar-0.13.3/hezar/embeddings/word2vec.py` & `hezar-0.14.0/hezar/embeddings/word2vec.py`

 * *Files identical despite different names*

### Comparing `hezar-0.13.3/hezar/models/language_modeling/bert/bert_lm.py` & `hezar-0.14.0/hezar/models/language_modeling/bert/bert_lm.py`

 * *Files identical despite different names*

### Comparing `hezar-0.13.3/hezar/models/language_modeling/bert/bert_lm_config.py` & `hezar-0.14.0/hezar/models/text_classification/roberta/roberta_text_classification_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 from dataclasses import dataclass
 
 from ....configs import ModelConfig
+from ....constants import TaskType
 
 
 @dataclass
-class BertLMConfig(ModelConfig):
-    name: str = "bert_lm"
-    task: str = "language_modeling"
-    vocab_size: int = 42000
-    hidden_size: int = 768
-    num_hidden_layers: int = 12
-    num_attention_heads: int = 12
-    intermediate_size: int = 3072
+class RobertaTextClassificationConfig(ModelConfig):
+    name: str = "roberta_text_classification"
+    task: str = TaskType.TEXT_CLASSIFICATION
+    num_labels: int = None
+    id2label: dict = None
+    attention_probs_dropout_prob: float = 0.1
+    bos_token_id: int = 0
+    eos_token_id: int = 2
+    gradient_checkpointing: bool = False
     hidden_act: str = "gelu"
     hidden_dropout_prob: float = 0.1
-    attention_probs_dropout_prob: float = 0.1
-    max_position_embeddings: int = 512
-    type_vocab_size: int = 2
-    initializer_range: float = 0.02
+    hidden_size: int = 768
+    classifier_dropout: float = None
+    initializer_range: int = 0.02
+    intermediate_size: int = 3072
     layer_norm_eps: float = 1e-12
-    pad_token_id: int = 0
+    max_position_embeddings: int = 514
+    num_attention_heads: int = 12
+    num_hidden_layers: int = 12
+    pad_token_id: int = 1
     position_embedding_type: str = "absolute"
+    type_vocab_size: int = 1
     use_cache: bool = True
-    classifier_dropout: float = None
+    vocab_size: int = 42000
```

### Comparing `hezar-0.13.3/hezar/models/language_modeling/distilbert/distilbert_lm.py` & `hezar-0.14.0/hezar/models/language_modeling/distilbert/distilbert_lm.py`

 * *Files identical despite different names*

### Comparing `hezar-0.13.3/hezar/models/language_modeling/distilbert/distilbert_lm_config.py` & `hezar-0.14.0/hezar/models/language_modeling/distilbert/distilbert_lm_config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from dataclasses import dataclass
 
 from ....configs import ModelConfig
+from ....constants import TaskType
 
 
 @dataclass
 class DistilBertLMConfig(ModelConfig):
     name: str = "distilbert_lm"
-    task: str = "language_modeling"
+    task: str = TaskType.LANGUAGE_MODELING
     activation: str = "gelu"
     attention_dropout: float = 0.1
     dim: int = 768
     dropout: float = 0.1
     hidden_dim: int = 3072
     initializer_range: float = 0.02
     max_position_embeddings: int = 512
```

### Comparing `hezar-0.13.3/hezar/models/language_modeling/roberta/roberta_lm.py` & `hezar-0.14.0/hezar/models/language_modeling/roberta/roberta_lm.py`

 * *Files identical despite different names*

### Comparing `hezar-0.13.3/hezar/models/language_modeling/roberta/roberta_lm_config.py` & `hezar-0.14.0/hezar/models/language_modeling/bert/bert_lm_config.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 from dataclasses import dataclass
 
 from ....configs import ModelConfig
+from ....constants import TaskType
 
 
 @dataclass
-class RobertaLMConfig(ModelConfig):
-    name: str = "roberta_lm"
-    task: str = "language_modeling"
-    attention_probs_dropout_prob: float = 0.1
-    bos_token_id: int = 0
-    eos_token_id: int = 2
-    gradient_checkpointing: bool = False
-    hidden_act: str = "gelu"
-    hidden_dropout_prob: float = 0.1
+class BertLMConfig(ModelConfig):
+    name: str = "bert_lm"
+    task: str = TaskType.LANGUAGE_MODELING
+    vocab_size: int = 42000
     hidden_size: int = 768
-    initializer_range: int = 0.02
+    num_hidden_layers: int = 12
+    num_attention_heads: int = 12
     intermediate_size: int = 3072
+    hidden_act: str = "gelu"
+    hidden_dropout_prob: float = 0.1
+    attention_probs_dropout_prob: float = 0.1
+    max_position_embeddings: int = 512
+    type_vocab_size: int = 2
+    initializer_range: float = 0.02
     layer_norm_eps: float = 1e-12
-    max_position_embeddings: int = 514
-    num_attention_heads: int = 12
-    num_hidden_layers: int = 12
-    pad_token_id: int = 1
+    pad_token_id: int = 0
     position_embedding_type: str = "absolute"
-    type_vocab_size: int = 1
     use_cache: bool = True
-    vocab_size: int = 42000
+    classifier_dropout: float = None
```

### Comparing `hezar-0.13.3/hezar/models/model.py` & `hezar-0.14.0/hezar/models/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     >>> from hezar import Model
     >>> model = Model.load("hezarai/bert-base-fa")
 """
 import os
 import tempfile
 from abc import abstractmethod
 from collections import OrderedDict
-from typing import Dict, Union, Mapping, Any, Optional
+from typing import Any, Dict, Mapping, Optional, Union
 
 import torch
 from huggingface_hub import create_repo, hf_hub_download, upload_file
 from torch import nn
 
 from ..builders import build_model
 from ..configs import ModelConfig
```

### Comparing `hezar-0.13.3/hezar/models/text_classification/bert/bert_text_classification.py` & `hezar-0.14.0/hezar/models/text_classification/bert/bert_text_classification.py`

 * *Files identical despite different names*

### Comparing `hezar-0.13.3/hezar/models/text_classification/bert/bert_text_classification_config.py` & `hezar-0.14.0/hezar/models/text_classification/bert/bert_text_classification_config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from dataclasses import dataclass
 
 from ....configs import ModelConfig
+from ....constants import TaskType
 
 
 @dataclass
 class BertTextClassificationConfig(ModelConfig):
     name: str = "bert_text_classification"
-    task: str = "text_classification"
+    task: str = TaskType.TEXT_CLASSIFICATION
     num_labels: int = None
     id2label: dict = None
     vocab_size: int = 42000
     hidden_size: int = 768
     num_hidden_layers: int = 12
     num_attention_heads: int = 12
     intermediate_size: int = 3072
```

### Comparing `hezar-0.13.3/hezar/models/text_classification/distilbert/distilbert_text_classification.py` & `hezar-0.14.0/hezar/models/text_classification/distilbert/distilbert_text_classification.py`

 * *Files identical despite different names*

### Comparing `hezar-0.13.3/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py` & `hezar-0.14.0/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from dataclasses import dataclass
 
 from ....configs import ModelConfig
+from ....constants import TaskType
 
 
 @dataclass
 class DistilBertTextClassificationConfig(ModelConfig):
     name: str = "distilbert_text_classification"
-    task: str = "text_classification"
+    task: str = TaskType.TEXT_CLASSIFICATION
     num_labels: int = None
     id2label: dict = None
     activation: str = "gelu"
     attention_dropout: float = 0.1
     dim: int = 768
     dropout: float = 0.1
     hidden_dim: int = 3072
```

### Comparing `hezar-0.13.3/hezar/models/text_classification/roberta/roberta_text_classification.py` & `hezar-0.14.0/hezar/models/text_classification/roberta/roberta_text_classification.py`

 * *Files identical despite different names*

### Comparing `hezar-0.13.3/hezar/models/text_classification/roberta/roberta_text_classification_config.py` & `hezar-0.14.0/hezar/models/language_modeling/roberta/roberta_lm_config.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 from dataclasses import dataclass
 
 from ....configs import ModelConfig
+from ....constants import TaskType
 
 
 @dataclass
-class RobertaTextClassificationConfig(ModelConfig):
-    name: str = "roberta_text_classification"
-    task: str = "text_classification"
-    num_labels: int = None
-    id2label: dict = None
+class RobertaLMConfig(ModelConfig):
+    name: str = "roberta_lm"
+    task: str = TaskType.LANGUAGE_MODELING
     attention_probs_dropout_prob: float = 0.1
     bos_token_id: int = 0
     eos_token_id: int = 2
     gradient_checkpointing: bool = False
     hidden_act: str = "gelu"
     hidden_dropout_prob: float = 0.1
     hidden_size: int = 768
-    classifier_dropout: float = None
     initializer_range: int = 0.02
     intermediate_size: int = 3072
     layer_norm_eps: float = 1e-12
     max_position_embeddings: int = 514
     num_attention_heads: int = 12
     num_hidden_layers: int = 12
     pad_token_id: int = 1
```

### Comparing `hezar-0.13.3/hezar/preprocessors/preprocessor.py` & `hezar-0.14.0/hezar/preprocessors/preprocessor.py`

 * *Files identical despite different names*

### Comparing `hezar-0.13.3/hezar/preprocessors/tokenizers/bpe.py` & `hezar-0.14.0/hezar/preprocessors/tokenizers/bpe.py`

 * *Files identical despite different names*

### Comparing `hezar-0.13.3/hezar/preprocessors/tokenizers/sentencepiece_bpe.py` & `hezar-0.14.0/hezar/preprocessors/tokenizers/sentencepiece_bpe.py`

 * *Files identical despite different names*

### Comparing `hezar-0.13.3/hezar/preprocessors/tokenizers/tokenizer.py` & `hezar-0.14.0/hezar/preprocessors/tokenizers/tokenizer.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import tempfile
 from collections import defaultdict
 from dataclasses import dataclass
-from typing import Dict, List, Union
+from typing import Dict, List, Mapping, Optional, Union
 
 import torch
 from huggingface_hub import create_repo, upload_file
 from tokenizers import Tokenizer as HFTokenizer
 from tokenizers.decoders import Decoder
 from tokenizers.models import Model
 
@@ -62,21 +62,88 @@
 
     def build(self) -> HFTokenizer:
         raise NotImplementedError
 
     def encode(self, inputs, is_pretokenized: bool = False, add_special_tokens: bool = True):
         if isinstance(inputs, str):
             inputs = [inputs]
+        elif isinstance(inputs, list) and is_pretokenized:
+            if isinstance(inputs[0], str):
+                inputs = [inputs]
         return self._tokenizer.encode_batch(inputs, is_pretokenized, add_special_tokens)
 
     def decode(self, ids: List[int], skip_special_tokens: bool = True) -> str:
         if isinstance(ids[0], list):
             return self._tokenizer.decode_batch(ids, skip_special_tokens=skip_special_tokens)
         return self._tokenizer.decode(ids, skip_special_tokens=skip_special_tokens)
 
+    def pad_encoded_batch(
+        self,
+        inputs,
+        padding: Union[bool, str] = None,
+        max_length: Optional[int] = None,
+        return_tensors: Optional[str] = None,
+        skip_keys: list = None,
+    ):
+
+        if isinstance(inputs, (list, tuple)) and isinstance(inputs[0], Mapping):
+            inputs = {key: [example[key] for example in inputs] for key in inputs[0].keys()}
+
+        inputs_max_length = max([len(x) for x in inputs[self.token_ids_name]])
+        # resolve padding and max_length parameters
+        padding = padding or self.config.padding_strategy
+
+        if padding is None:
+            if max_length is not None:
+                padding = "max_length"
+            elif max_length is None:
+                logger.warning("Both padding and max_length are None so the inputs cannot be padded!")
+                return inputs
+
+        if padding == "longest":
+            if max_length is not None:
+                logger.warning("Setting padding='longest' and max_length is not valid. You must set one of them"
+                               "and leave the other as None. Falling back to padding='longest'")
+
+            inputs_length = inputs_max_length
+
+        elif padding == "max_length":
+            if max_length is None:
+                logger.warning("Setting padding='max_length' but no max_length value is provided in the function "
+                               "parameters nor the tokenizer config! Falling back to padding='longest'")
+                inputs_length = inputs_max_length
+            else:
+                # TODO implement truncation if possible and remove this condition
+                if max_length <= inputs_max_length:
+                    logger.warning(f"Setting max_length to {max_length} while max input length is {inputs_max_length}!"
+                                   f"Falling back to padding='longest' "
+                                   f"since truncation is not available yet in Hezar :(")
+                    inputs_length = inputs_max_length
+                else:
+                    inputs_length = max_length
+
+        inputs = convert_batch_dict_dtype(inputs, dtype="list", skip_keys=skip_keys)
+
+        skip_keys = skip_keys or []
+        for field, batch in inputs.items():
+            if field in skip_keys:
+                continue
+            padding_id = 0 if field == "attention_mask" else self.config.pad_token_id
+            padded_batch = []
+            for x in batch:
+                difference = inputs_length - len(x)
+                paddings = [padding_id] * difference
+                padded_x = x + paddings if self.config.padding_direction == "right" else paddings + x
+                padded_batch.append(padded_x)
+            inputs[field] = padded_batch
+
+        inputs = convert_batch_dict_dtype(inputs, dtype=return_tensors)
+
+        return inputs
+
     def __call__(
         self,
         inputs: List[str],
         device: Union[str, torch.device] = None,
         add_special_tokens: bool = True,
         padding_strategy=None,
         truncation_strategy=None,
@@ -88,14 +155,15 @@
         return_tokens: bool = None,
         return_token_type_ids: bool = None,
         return_attention_mask: bool = True,
         return_overflowing_tokens: bool = False,
         return_special_tokens_mask: bool = True,
         return_offsets_mapping: bool = False,
         return_length: bool = False,
+        return_word_ids: bool = False,
         verbose: bool = True,
         **kwargs,
     ):
         """
         Tokenize a batch of string inputs and return the relevant properties e.g, token ids, attention mask, etc.
 
         Args:
@@ -149,14 +217,15 @@
                 return_tokens=return_tokens,
                 return_token_type_ids=return_token_type_ids,
                 return_attention_mask=return_attention_mask,
                 return_overflowing_tokens=return_overflowing_tokens,
                 return_special_tokens_mask=return_special_tokens_mask,
                 return_offsets_mapping=return_offsets_mapping,
                 return_length=return_length,
+                return_word_ids=return_word_ids,
             )
             for encoding in encodings
         ]
         # Permute output dict from [batch_0: Dict[key, value], ...] to Dict[key, [batch_0, batch_1, ...], ...]
         sanitized_outputs = {}
         for key in encodings_dict[0].keys():
             stack = [e for item in encodings_dict for e in item[key]]
@@ -166,14 +235,20 @@
         # from the batch idx to the original sample
         if return_overflowing_tokens:
             overflow_to_sample_mapping = []
             for i, encodings_ in enumerate(encodings_dict):
                 overflow_to_sample_mapping += [i] * len(encodings_["input_ids"])
             sanitized_outputs["overflow_to_sample_mapping"] = overflow_to_sample_mapping
 
+        if return_tensors == "list" or return_tensors is None:
+            sanitized_outputs = {
+                key: value[0] if len(value) > 0 and isinstance(value[0], list) else value
+                for key, value in sanitized_outputs.items()
+            }
+
         outputs = convert_batch_dict_dtype(sanitized_outputs, dtype=return_tensors)
         if device and return_tensors == "pt":
             outputs = {k: v.to(device) for k, v in outputs.items() if isinstance(v, torch.Tensor)}
 
         return outputs
 
     def set_truncation_and_padding(
@@ -227,14 +302,15 @@
         return_tokens: bool = None,
         return_token_type_ids: bool = None,
         return_attention_mask: bool = None,
         return_overflowing_tokens: bool = False,
         return_special_tokens_mask: bool = False,
         return_offsets_mapping: bool = False,
         return_length: bool = False,
+        return_word_ids: bool = False,
     ):
         if return_overflowing_tokens and encoding.overflowing is not None:
             encodings = [encoding] + encoding.overflowing
         else:
             encodings = [encoding]
 
         encoding_dict = defaultdict(list)
@@ -249,14 +325,16 @@
                 encoding_dict["special_tokens_mask"].append(e.special_tokens_mask)
             if return_offsets_mapping:
                 encoding_dict["offset_mapping"].append(e.offsets)
             if return_length:
                 encoding_dict["length"].append(len(e.ids))
             if return_tokens:
                 encoding_dict["tokens"].append(e.tokens)
+            if return_word_ids:
+                encoding_dict["word_ids"].append(e.word_ids)
 
         return encoding_dict
 
     def num_special_tokens_to_add(self, is_pair: bool) -> int:
         return self._tokenizer.num_special_tokens_to_add(is_pair)
 
     def get_vocab(self, with_added_tokens: bool = True) -> Dict[str, int]:
```

### Comparing `hezar-0.13.3/hezar/preprocessors/tokenizers/wordpiece.py` & `hezar-0.14.0/hezar/preprocessors/tokenizers/wordpiece.py`

 * *Files identical despite different names*

### Comparing `hezar-0.13.3/hezar/registry.py` & `hezar-0.14.0/hezar/registry.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,49 +3,62 @@
 specific registry. These registries are simple python dictionaries that map a module's name to its class and its config
 class. These registries are initialized here and filled automatically when you import hezar or a registry itself.
 
 Examples:
     >>> # read models registry
     >>> from hezar.registry import models_registry
     >>> print(models_registry)
-    {'distilbert_lm': {'model_class': <class 'hezar.models.language_modeling.distilbert.distilbert_lm.DistilBertLM'>,
-    'config_class': <class 'hezar.models.language_modeling.distilbert.distilbert_lm_config.DistilBertLMConfig'>}}
+    {'distilbert_lm': {'module_class': <class 'hezar.models.language_modeling.distilbert.distilbert_lm.DistilBertLM'>,
+    'config_class': <class 'hezar.models.language_modeling.distilbert.distilbert_lm_config.DistilBertLMConfig'>},
+    'doc': ''}
 
     >>> # add a model class to models_registry
     >>> from hezar import Model, register_model
     >>> @register_model(name="my_awesome_model", config_class=MyAwesomeModelConfig)
     >>> class MyAwesomeModel(Model):
     ...    def __init__(config: MyAwesomeModelConfig):
     ...        ...
 
 Keep in mind that registries usually don't need to be used directly. There is a bunch of functions to build modules
 using a module's registry name in `hezar.builders` module. See the file `builders.py` for more info.
 
 Note: In case of adding a new registry container, make sure to add to `__all__` below!
 """
 
+from dataclasses import dataclass
+from typing import Dict, Type
+
 from torch import nn, optim
 
+from .configs import DatasetConfig, EmbeddingConfig, ModelConfig, PreprocessorConfig, TrainConfig
 from .utils import get_logger
 
 
 __all__ = [
     "register_model",
     "register_preprocessor",
     "register_dataset",
     "register_embedding",
 ]
 
 logger = get_logger(__name__)
 
-models_registry = {}
-preprocessors_registry = {}
-datasets_registry = {}
-embeddings_registry = {}
-trainers_registry = {}
+
+@dataclass
+class Registry:
+    module_class: type
+    config_class: type
+    doc: str
+
+
+models_registry: Dict[str, Registry] = {}
+preprocessors_registry: Dict[str, Registry] = {}
+datasets_registry: Dict[str, Registry] = {}
+embeddings_registry: Dict[str, Registry] = {}
+trainers_registry: Dict[str, Registry] = {}
 
 criterions_registry = {
     "bce": nn.BCELoss,
     "bce_with_logits": nn.BCEWithLogitsLoss,
     "nll": nn.NLLLoss,
     "cross_entropy": nn.CrossEntropyLoss,
     "mse": nn.MSELoss,
@@ -58,15 +71,15 @@
 }
 lr_schedulers_registry = {
     "reduce_on_plateau": optim.lr_scheduler.ReduceLROnPlateau,
     "cosine_lr": optim.lr_scheduler.CosineAnnealingLR,
 }
 
 
-def register_model(model_name: str, config_class):
+def register_model(model_name: str, config_class: Type[ModelConfig]):
     """
     A class decorator that adds the model class and the config class to the `models_registry`
 
     Args:
         model_name: Model's registry name e.g, `bert_sequence_labeling`
         config_class: Model's config class e.g, `BertSequenceLabelingConfig`. This parameter must be the config class
             itself not a config instance!
@@ -78,22 +91,27 @@
         if model_name in models_registry:
             logger.warning(f"Model `{model_name}` is already registered. Overwriting...")
 
         if config_class.name != model_name:
             raise ValueError(f"`model_name` and `config.name` are not compatible for `{cls.__name__}`\n"
                              f"model_name: {model_name}\n"
                              f"{config_class.__name__}.name: {config_class.name}")
-        models_registry[model_name] = {"model_class": cls, "config_class": config_class}
+
+        models_registry[model_name] = Registry(
+            module_class=cls,
+            config_class=config_class,
+            doc=cls.__doc__
+        )
 
         return cls
 
     return register
 
 
-def register_dataset(dataset_name: str, config_class):
+def register_dataset(dataset_name: str, config_class: Type[DatasetConfig]):
     """
     A class decorator that adds the dataset class and the config class to the `datasets_registry`
 
     Args:
         dataset_name: Dataset's registry name e.g, `text_classification`.
         config_class: Dataset's config class e.g, `TextClassificationDatasetConfig`. This parameter must be the config
             class itself not a config instance!
@@ -105,22 +123,27 @@
         if dataset_name in datasets_registry:
             logger.warning(f"Dataset `{dataset_name}` is already registered. Overwriting...")
 
         if config_class.name != dataset_name:
             raise ValueError(f"`dataset_name` and `config.name` are not compatible for `{cls.__name__}`\n"
                              f"dataset_name: {dataset_name}\n"
                              f"{config_class.__name__}.name: {config_class.name}")
-        datasets_registry[dataset_name] = {"dataset_class": cls, "config_class": config_class}
+
+        datasets_registry[dataset_name] = Registry(
+            module_class=cls,
+            config_class=config_class,
+            doc=cls.__doc__
+        )
 
         return cls
 
     return register
 
 
-def register_preprocessor(preprocessor_name: str, config_class):
+def register_preprocessor(preprocessor_name: str, config_class: Type[PreprocessorConfig]):
     """
     A class decorator that adds the preprocessor class and the config class to the `preprocessors_registry`
 
     Args:
         preprocessor_name: Preprocessor's registry name e.g, `bpe_tokenizer`.
         config_class: Preprocessor's config class e.g, BPEConfig. This parameter must be the config
             class itself not a config instance!
@@ -132,22 +155,27 @@
         if preprocessor_name in preprocessors_registry:
             logger.warning(f"Preprocessor `{preprocessor_name}` is already registered. Overwriting...")
 
         if config_class.name != preprocessor_name:
             raise ValueError(f"`preprocessor_name` and `config.name` are not compatible for `{cls.__name__}`\n"
                              f"preprocessor_name: {preprocessor_name}\n"
                              f"{config_class.__name__}.name: {config_class.name}")
-        preprocessors_registry[preprocessor_name] = {"preprocessor_class": cls, "config_class": config_class}
+
+        preprocessors_registry[preprocessor_name] = Registry(
+            module_class=cls,
+            config_class=config_class,
+            doc=cls.__doc__
+        )
 
         return cls
 
     return register
 
 
-def register_embedding(embedding_name: str, config_class):
+def register_embedding(embedding_name: str, config_class: Type[EmbeddingConfig]):
     """
     A class decorator that adds the embedding class and the config class to the `embeddings_registry`
 
     Args:
         embedding_name: Embedding's registry name e.g, `word2vec_cbow`.
         config_class: Embedding's config class e.g, Word2VecCBOWConfig. This parameter must be the config
             class itself not a config instance!
@@ -159,22 +187,27 @@
         if embedding_name in embeddings_registry:
             logger.warning(f"Embedding `{embedding_name}` is already registered. Overwriting...")
 
         if config_class.name != embedding_name:
             raise ValueError(f"`embedding_name` and `config.name` are not compatible for `{cls.__name__}`\n"
                              f"embedding_name: {embedding_name}\n"
                              f"{config_class.__name__}.name: {config_class.name}")
-        embeddings_registry[embedding_name] = {"embedding_class": cls, "config_class": config_class}
+
+        embeddings_registry[embedding_name] = Registry(
+            module_class=cls,
+            config_class=config_class,
+            doc=cls.__doc__
+        )
 
         return cls
 
     return register
 
 
-def register_trainer(trainer_name: str, config_class):
+def register_trainer(trainer_name: str, config_class: Type[TrainConfig]):
     """
     A class decorator that adds the Trainer class and the config class to the `trainers_registry`
 
     Args:
         trainer_name: Trainer's registry name e.g, `text_classification_trainer`
         config_class: Trainer's config class e.g, `TextClassificationTrainerConfig`.
             This parameter must be the config class itself not a config instance!
@@ -186,12 +219,17 @@
         if trainer_name in trainers_registry:
             logger.warning(f"Trainer `{trainer_name}` is already registered. Overwriting...")
 
         if config_class.name != trainer_name:
             raise ValueError(f"`trainer_name` and `config.name` are not compatible for `{cls.__name__}`\n"
                              f"trainer_name: {trainer_name}\n"
                              f"{config_class.__name__}.name: {config_class.name}")
-        trainers_registry[trainer_name] = {"trainer_class": cls, "config_class": config_class}
+
+        trainers_registry[trainer_name] = Registry(
+            module_class=cls,
+            config_class=config_class,
+            doc=cls.__doc__
+        )
 
         return cls
 
     return register
```

### Comparing `hezar-0.13.3/hezar/trainers/trainer.py` & `hezar-0.14.0/hezar/trainers/trainer.py`

 * *Files identical despite different names*

### Comparing `hezar-0.13.3/hezar/trainers/trainer_utils.py` & `hezar-0.14.0/hezar/trainers/trainer_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.13.3/hezar/utils/config_utils.py` & `hezar-0.14.0/hezar/utils/config_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 
 __all__ = [
     "flatten_dict",
     "load_yaml_config",
     "load_json_config",
     "hezar_config_to_hf_config",
     "get_module_config_class",
+    "get_module_class",
 ]
 
 logger = get_logger(__name__)
 
 
 def flatten_dict(dict_config: Union[Dict, DictConfig]) -> DictConfig:
     """
@@ -90,15 +91,49 @@
 
         registry = preprocessors_registry
     elif config_type == "dataset":
         from ..registry import datasets_registry  # noqa
 
         registry = datasets_registry
     elif config_type == "embedding":
-        from ..registry import embeddings_registry
+        from ..registry import embeddings_registry  # noqa
         registry = embeddings_registry
 
     else:
         raise ValueError(f"Invalid `config_type`: {config_type}!")
 
-    config_cls = registry[name]["config_class"]
+    config_cls = registry[name].config_class
     return config_cls
+
+
+def get_module_class(name: str, module_type: str):
+    """
+    Get module class based on registry name
+
+    Args:
+        name: Module's key name in its registry
+        module_type: Type of the module e.g, model, dataset, preprocessor, embedding, etc
+
+    Returns:
+        A class corresponding to the given module
+    """
+    if module_type == "model":
+        from ..registry import models_registry  # noqa
+
+        registry = models_registry
+    elif module_type == "preprocessor":
+        from ..registry import preprocessors_registry  # noqa
+
+        registry = preprocessors_registry
+    elif module_type == "dataset":
+        from ..registry import datasets_registry  # noqa
+
+        registry = datasets_registry
+    elif module_type == "embedding":
+        from ..registry import embeddings_registry  # noqa
+        registry = embeddings_registry
+
+    else:
+        raise ValueError(f"Invalid `config_type`: {module_type}!")
+
+    module_cls = registry[name].module_class
+    return module_cls
```

### Comparing `hezar-0.13.3/hezar/utils/hub_utils.py` & `hezar-0.14.0/hezar/utils/hub_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.13.3/pyproject.toml` & `hezar-0.14.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "hezar"
-version = "0.13.3"
+version = "0.14.0"
 packages = [{ include = "hezar" }]
 description = "Hezar: A seamless AI framework & library for Persian"
 license = "MIT"
 authors = ["Aryan Shekarlaban <arxyzan@gmail.com>"]
 maintainers = ["Aryan Shekarlaban <arxyzan@gmail.com>"]
 repository = "https://github.com/hezarai/hezar"
 homepage = "https://github.com/hezarai"
```

### Comparing `hezar-0.13.3/PKG-INFO` & `hezar-0.14.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hezar
-Version: 0.13.3
+Version: 0.14.0
 Summary: Hezar: A seamless AI framework & library for Persian
 Home-page: https://github.com/hezarai
 License: MIT
 Keywords: packaging,poetry
 Author: Aryan Shekarlaban
 Author-email: arxyzan@gmail.com
 Maintainer: Aryan Shekarlaban
@@ -47,15 +47,20 @@
 - has a highly developer-friendly interface
 - has a task-based model interface which is more convenient for general users.
 - is packed with additional tools like word embeddings, tokenizers, feature extractors, etc.
 - comes with a lot of supplementary ML tools for deployment, benchmarking, optimization, etc.
 - and more!
 
 ## Installation
-Clone the repo and run:
+Hezar is available on PyPI and can be installed with pip:
+```commandline
+pip install hezar
+```
+You can also install the latest version from the source.
+Clone the repo and execute the following commands:
 ```commandline
 git clone https://github.com/hezarai/hezar.git
 pip install ./hezar
 ```
 
 ## Quick Tour
 ### Ready-to-use models from Hub
```

