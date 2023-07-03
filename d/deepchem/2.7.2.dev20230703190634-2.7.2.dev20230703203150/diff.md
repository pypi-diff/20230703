# Comparing `tmp/deepchem-2.7.2.dev20230703190634.tar.gz` & `tmp/deepchem-2.7.2.dev20230703203150.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepchem-2.7.2.dev20230703190634.tar", last modified: Mon Jul  3 19:06:34 2023, max compression
+gzip compressed data, was "deepchem-2.7.2.dev20230703203150.tar", last modified: Mon Jul  3 20:31:50 2023, max compression
```

## Comparing `deepchem-2.7.2.dev20230703190634.tar` & `deepchem-2.7.2.dev20230703203150.tar`

### file list

```diff
@@ -1,297 +1,297 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:06:34.739825 deepchem-2.7.2.dev20230703190634/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1047 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-03 19:06:34.739825 deepchem-2.7.2.dev20230703190634/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:06:34.715825 deepchem-2.7.2.dev20230703190634/deepchem/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:06:34.715825 deepchem-2.7.2.dev20230703190634/deepchem/data/
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    67894 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/data/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)   118009 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/data/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/data/pytorch_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    12606 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/data/supports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:06:34.715825 deepchem-2.7.2.dev20230703190634/deepchem/dock/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/dock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/dock/binding_pocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/dock/docking.py
--rw-r--r--   0 runner    (1001) docker     (123)    19576 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/dock/pose_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/dock/pose_scoring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:06:34.719825 deepchem-2.7.2.dev20230703190634/deepchem/feat/
--rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/feat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/feat/atomic_conformation.py
--rw-r--r--   0 runner    (1001) docker     (123)    19458 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/feat/base_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/feat/bert_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/feat/binding_pocket_features.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:06:34.719825 deepchem-2.7.2.dev20230703190634/deepchem/feat/complex_featurizers/
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/feat/complex_featurizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/feat/complex_featurizers/complex_atomic_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)    10769 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/feat/complex_featurizers/contact_fingerprints.py
--rw-r--r--   0 runner    (1001) docker     (123)    27676 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/feat/complex_featurizers/grid_featurizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    20248 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/feat/complex_featurizers/rdkit_grid_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11465 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/feat/complex_featurizers/splif_fingerprints.py
--rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/feat/dft_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    22111 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/feat/graph_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    38890 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/feat/graph_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/feat/huggingface_featurizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:06:34.719825 deepchem-2.7.2.dev20230703190634/deepchem/feat/material_featurizers/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/feat/material_featurizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7539 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/feat/material_featurizers/cgcnn_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/feat/material_featurizers/element_property_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/feat/material_featurizers/elemnet_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    28058 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/feat/material_featurizers/lcnn_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/feat/material_featurizers/sine_coulomb_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    14808 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/feat/mol_graphs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:06:34.719825 deepchem-2.7.2.dev20230703190634/deepchem/feat/molecule_featurizers/
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/feat/molecule_featurizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/feat/molecule_featurizers/atomic_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/feat/molecule_featurizers/bp_symmetry_function_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/feat/molecule_featurizers/circular_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     9448 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/feat/molecule_featurizers/conformer_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10925 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/feat/molecule_featurizers/coulomb_matrices.py
--rw-r--r--   0 runner    (1001) docker     (123)    19123 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/feat/molecule_featurizers/dmpnn_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/feat/molecule_featurizers/grover_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/feat/molecule_featurizers/maccs_keys_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/feat/molecule_featurizers/mat_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7587 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/feat/molecule_featurizers/mol2vec_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    20381 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/feat/molecule_featurizers/mol_graph_conv_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9346 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/feat/molecule_featurizers/molgan_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/feat/molecule_featurizers/mordred_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/feat/molecule_featurizers/one_hot_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/feat/molecule_featurizers/pubchem_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/feat/molecule_featurizers/raw_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/feat/molecule_featurizers/rdkit_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/feat/molecule_featurizers/smiles_to_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/feat/molecule_featurizers/smiles_to_seq.py
--rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/feat/molecule_featurizers/snap_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/feat/molecule_featurizers/sparse_matrix_one_hot_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/feat/reaction_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/feat/roberta_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:06:34.719825 deepchem-2.7.2.dev20230703190634/deepchem/feat/sequence_featurizers/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/feat/sequence_featurizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/feat/sequence_featurizers/position_frequency_matrix_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/feat/smiles_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:06:34.723825 deepchem-2.7.2.dev20230703190634/deepchem/feat/vocabulary_builders/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/feat/vocabulary_builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17686 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/feat/vocabulary_builders/grover_vocab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/feat/vocabulary_builders/hf_vocab.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/feat/vocabulary_builders/vocabulary_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:06:34.723825 deepchem-2.7.2.dev20230703190634/deepchem/hyper/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/hyper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/hyper/base_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)    17151 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/hyper/gaussian_process.py
--rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/hyper/grid_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    12427 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/hyper/random_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:06:34.723825 deepchem-2.7.2.dev20230703190634/deepchem/metalearning/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/metalearning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10539 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/metalearning/maml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:06:34.723825 deepchem-2.7.2.dev20230703190634/deepchem/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/metrics/genomic_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    31620 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/metrics/score_function.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:06:34.723825 deepchem-2.7.2.dev20230703190634/deepchem/models/
--rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/IRV.py
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13833 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/atomic_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    17354 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/chemnet_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    15504 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/chemnet_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:06:34.723825 deepchem-2.7.2.dev20230703190634/deepchem/models/dft/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/dft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9553 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/dft/dftxc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14020 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/dft/nnxc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/dft/scf.py
--rw-r--r--   0 runner    (1001) docker     (123)    23457 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/fcnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    24548 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/gan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:06:34.727825 deepchem-2.7.2.dev20230703190634/deepchem/models/gbdt_models/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/gbdt_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/gbdt_models/gbdt_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    57408 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/graph_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:06:34.727825 deepchem-2.7.2.dev20230703190634/deepchem/models/jax_models/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/jax_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28179 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/jax_models/jax_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/jax_models/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    17070 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/jax_models/pinns_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    56522 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/keras_model.py
--rw-r--r--   0 runner    (1001) docker     (123)   144759 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:06:34.727825 deepchem-2.7.2.dev20230703190634/deepchem/models/lightning/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/lightning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/lightning/dc_lightning_dataset_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/lightning/dc_lightning_module.py
--rw-r--r--   0 runner    (1001) docker     (123)    61903 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    14135 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/molgan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/multitask.py
--rw-r--r--   0 runner    (1001) docker     (123)    10975 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/normalizing_flows.py
--rw-r--r--   0 runner    (1001) docker     (123)    26871 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13095 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/progressive_multitask.py
--rw-r--r--   0 runner    (1001) docker     (123)    17830 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/robust_multitask.py
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/scscore.py
--rw-r--r--   0 runner    (1001) docker     (123)    25969 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/seqtoseq.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:06:34.727825 deepchem-2.7.2.dev20230703190634/deepchem/models/sklearn_models/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/sklearn_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/sklearn_models/sklearn_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10552 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/text_cnn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:06:34.727825 deepchem-2.7.2.dev20230703190634/deepchem/models/torch_models/
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/torch_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/torch_models/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    12226 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/torch_models/attentivefp.py
--rw-r--r--   0 runner    (1001) docker     (123)    14455 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/torch_models/cgcnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/torch_models/chemberta.py
--rw-r--r--   0 runner    (1001) docker     (123)     9543 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/torch_models/cnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    31166 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/torch_models/dmpnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/torch_models/ferminet.py
--rw-r--r--   0 runner    (1001) docker     (123)    15845 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/torch_models/gat.py
--rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/torch_models/gcn.py
--rw-r--r--   0 runner    (1001) docker     (123)    51159 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/torch_models/gnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    25005 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/torch_models/gnn3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    38126 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/torch_models/grover.py
--rw-r--r--   0 runner    (1001) docker     (123)    38432 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/torch_models/grover_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    22942 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/torch_models/hf_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    30077 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/torch_models/infograph.py
--rw-r--r--   0 runner    (1001) docker     (123)    19215 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/torch_models/kfac_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)   140973 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/torch_models/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18575 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/torch_models/lcnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    17126 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/torch_models/mat.py
--rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/torch_models/megnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    18122 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/torch_models/modular.py
--rw-r--r--   0 runner    (1001) docker     (123)    12074 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/torch_models/mpnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/torch_models/normalizing_flows_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/torch_models/pagtn.py
--rw-r--r--   0 runner    (1001) docker     (123)    23019 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/torch_models/pna_gnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/torch_models/readout.py
--rw-r--r--   0 runner    (1001) docker     (123)    52726 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/torch_models/torch_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/models/wandblogger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:06:34.731825 deepchem-2.7.2.dev20230703190634/deepchem/molnet/
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/molnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11668 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/molnet/check_availability.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/molnet/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    14702 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/molnet/dnasim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:06:34.731825 deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/bace_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    14202 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/bace_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/bbbc_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/bbbp_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/cell_counting_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/chembl25_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/chembl_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    10252 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/chembl_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/clearance_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/clintox_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/delaney_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/factors_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/freesolv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/hiv_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/hopv_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/hppb_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/kaggle_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)   165414 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/kaggle_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/kinase_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/lipo_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     9165 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/load_dataset_template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:06:34.735825 deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/material_datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/material_datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/material_datasets/load_Pt_NO_surface_adsorbate_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/material_datasets/load_bandgap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/material_datasets/load_mp_formation_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/material_datasets/load_mp_metallicity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/material_datasets/load_perovskite.py
--rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/molnet_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/muv_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/nci_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/pcba_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     8586 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/pdbbind_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/ppb_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/qm7_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/qm8_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/qm9_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/sampl_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/sider_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/sweetlead_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/thermosol_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/tox21_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    18900 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/toxcast_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/uspto_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/uv_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/uv_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/zinc15_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/molnet/preset_hyper_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    13549 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/molnet/run_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/molnet/run_benchmark_low_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    36564 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/molnet/run_benchmark_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:06:34.735825 deepchem-2.7.2.dev20230703190634/deepchem/rl/
--rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23102 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/rl/a2c.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:06:34.735825 deepchem-2.7.2.dev20230703190634/deepchem/rl/envs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/rl/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/rl/envs/test_tictactoe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/rl/envs/tictactoe.py
--rw-r--r--   0 runner    (1001) docker     (123)    25262 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/rl/ppo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:06:34.735825 deepchem-2.7.2.dev20230703190634/deepchem/splits/
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/splits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63895 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/splits/splitters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/splits/task_splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:06:34.735825 deepchem-2.7.2.dev20230703190634/deepchem/trans/
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/trans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/trans/duplicate.py
--rw-r--r--   0 runner    (1001) docker     (123)    91191 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/trans/transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:06:34.739825 deepchem-2.7.2.dev20230703190634/deepchem/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/utils/conformers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13294 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/utils/coordinate_box_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20923 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/utils/debug_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/utils/dftutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10476 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/utils/docking_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13528 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/utils/electron_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    19454 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/utils/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/utils/fake_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/utils/fragment_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/utils/genomics_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/utils/geometry_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/utils/graph_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/utils/grover.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/utils/hash_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    19262 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/utils/molecule_feature_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17713 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/utils/noncovalent_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11749 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/utils/pdbqt_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/utils/pytorch_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    65672 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/utils/rdkit_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/utils/save.py
--rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/utils/sequence_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:06:34.739825 deepchem-2.7.2.dev20230703190634/deepchem/utils/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/utils/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/utils/test/test_coordinate_box_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/utils/test/test_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/utils/test/test_dftutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/utils/test/test_docking_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/utils/test/test_electron_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12977 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/utils/test/test_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/utils/test/test_fake_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/utils/test/test_fragment_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/utils/test/test_generator_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/utils/test/test_genomics_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/utils/test/test_geometry_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/utils/test/test_graph_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/utils/test/test_grover.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/utils/test/test_hash_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/utils/test/test_molecule_feature_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/utils/test/test_noncovalent_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/utils/test/test_pdbqt_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/utils/test/test_pytorch_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/utils/test/test_rdkit_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/utils/test/test_sequence_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/utils/test/test_updated_scipy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/utils/test/test_voxel_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/utils/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/utils/vina_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/deepchem/utils/voxel_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 19:06:34.715825 deepchem-2.7.2.dev20230703190634/deepchem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-03 19:06:34.000000 deepchem-2.7.2.dev20230703190634/deepchem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10711 2023-07-03 19:06:34.000000 deepchem-2.7.2.dev20230703190634/deepchem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 19:06:34.000000 deepchem-2.7.2.dev20230703190634/deepchem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-03 19:06:34.000000 deepchem-2.7.2.dev20230703190634/deepchem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-03 19:06:34.000000 deepchem-2.7.2.dev20230703190634/deepchem.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-03 19:06:34.739825 deepchem-2.7.2.dev20230703190634/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-07-03 19:06:24.000000 deepchem-2.7.2.dev20230703190634/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:31:50.619017 deepchem-2.7.2.dev20230703203150/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1047 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-03 20:31:50.619017 deepchem-2.7.2.dev20230703203150/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:31:50.579017 deepchem-2.7.2.dev20230703203150/deepchem/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:31:50.583017 deepchem-2.7.2.dev20230703203150/deepchem/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67894 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/data/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118009 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/data/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/data/pytorch_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12606 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/data/supports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:31:50.583017 deepchem-2.7.2.dev20230703203150/deepchem/dock/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/dock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/dock/binding_pocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/dock/docking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19576 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/dock/pose_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/dock/pose_scoring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:31:50.583017 deepchem-2.7.2.dev20230703203150/deepchem/feat/
+-rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/feat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/feat/atomic_conformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19458 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/feat/base_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/feat/bert_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/feat/binding_pocket_features.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:31:50.587017 deepchem-2.7.2.dev20230703203150/deepchem/feat/complex_featurizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/feat/complex_featurizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/feat/complex_featurizers/complex_atomic_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10769 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/feat/complex_featurizers/contact_fingerprints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27676 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/feat/complex_featurizers/grid_featurizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20248 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/feat/complex_featurizers/rdkit_grid_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11465 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/feat/complex_featurizers/splif_fingerprints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/feat/dft_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22111 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/feat/graph_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38890 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/feat/graph_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/feat/huggingface_featurizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:31:50.587017 deepchem-2.7.2.dev20230703203150/deepchem/feat/material_featurizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/feat/material_featurizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7539 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/feat/material_featurizers/cgcnn_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/feat/material_featurizers/element_property_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/feat/material_featurizers/elemnet_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28058 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/feat/material_featurizers/lcnn_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/feat/material_featurizers/sine_coulomb_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14808 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/feat/mol_graphs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:31:50.591017 deepchem-2.7.2.dev20230703203150/deepchem/feat/molecule_featurizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/feat/molecule_featurizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/feat/molecule_featurizers/atomic_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/feat/molecule_featurizers/bp_symmetry_function_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/feat/molecule_featurizers/circular_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9448 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/feat/molecule_featurizers/conformer_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10925 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/feat/molecule_featurizers/coulomb_matrices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19123 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/feat/molecule_featurizers/dmpnn_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/feat/molecule_featurizers/grover_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/feat/molecule_featurizers/maccs_keys_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/feat/molecule_featurizers/mat_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7587 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/feat/molecule_featurizers/mol2vec_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20381 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/feat/molecule_featurizers/mol_graph_conv_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9346 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/feat/molecule_featurizers/molgan_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/feat/molecule_featurizers/mordred_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/feat/molecule_featurizers/one_hot_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/feat/molecule_featurizers/pubchem_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/feat/molecule_featurizers/raw_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/feat/molecule_featurizers/rdkit_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/feat/molecule_featurizers/smiles_to_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/feat/molecule_featurizers/smiles_to_seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/feat/molecule_featurizers/snap_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/feat/molecule_featurizers/sparse_matrix_one_hot_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/feat/reaction_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/feat/roberta_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:31:50.591017 deepchem-2.7.2.dev20230703203150/deepchem/feat/sequence_featurizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/feat/sequence_featurizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/feat/sequence_featurizers/position_frequency_matrix_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/feat/smiles_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:31:50.591017 deepchem-2.7.2.dev20230703203150/deepchem/feat/vocabulary_builders/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/feat/vocabulary_builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17686 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/feat/vocabulary_builders/grover_vocab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/feat/vocabulary_builders/hf_vocab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/feat/vocabulary_builders/vocabulary_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:31:50.591017 deepchem-2.7.2.dev20230703203150/deepchem/hyper/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/hyper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/hyper/base_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17151 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/hyper/gaussian_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/hyper/grid_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12427 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/hyper/random_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:31:50.591017 deepchem-2.7.2.dev20230703203150/deepchem/metalearning/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/metalearning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10539 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/metalearning/maml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:31:50.591017 deepchem-2.7.2.dev20230703203150/deepchem/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/metrics/genomic_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31620 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/metrics/score_function.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:31:50.595017 deepchem-2.7.2.dev20230703203150/deepchem/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/IRV.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13833 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/atomic_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17354 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/chemnet_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15504 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/chemnet_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:31:50.595017 deepchem-2.7.2.dev20230703203150/deepchem/models/dft/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/dft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9553 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/dft/dftxc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14020 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/dft/nnxc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/dft/scf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23457 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/fcnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24548 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/gan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:31:50.595017 deepchem-2.7.2.dev20230703203150/deepchem/models/gbdt_models/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/gbdt_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/gbdt_models/gbdt_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57408 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/graph_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:31:50.595017 deepchem-2.7.2.dev20230703203150/deepchem/models/jax_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/jax_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28179 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/jax_models/jax_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/jax_models/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17070 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/jax_models/pinns_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56522 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/keras_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)   144759 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:31:50.595017 deepchem-2.7.2.dev20230703203150/deepchem/models/lightning/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/lightning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/lightning/dc_lightning_dataset_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/lightning/dc_lightning_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61903 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14135 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/molgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/multitask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10975 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/normalizing_flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26871 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13095 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/progressive_multitask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17830 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/robust_multitask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/scscore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25969 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/seqtoseq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:31:50.595017 deepchem-2.7.2.dev20230703203150/deepchem/models/sklearn_models/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/sklearn_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/sklearn_models/sklearn_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10552 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/text_cnn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:31:50.603017 deepchem-2.7.2.dev20230703203150/deepchem/models/torch_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/torch_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/torch_models/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12226 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/torch_models/attentivefp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14455 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/torch_models/cgcnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/torch_models/chemberta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9543 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/torch_models/cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31166 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/torch_models/dmpnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/torch_models/ferminet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15845 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/torch_models/gat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/torch_models/gcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51159 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/torch_models/gnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25005 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/torch_models/gnn3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38126 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/torch_models/grover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38432 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/torch_models/grover_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22942 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/torch_models/hf_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30077 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/torch_models/infograph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19215 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/torch_models/kfac_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)   145745 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/torch_models/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18575 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/torch_models/lcnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17126 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/torch_models/mat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/torch_models/megnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18122 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/torch_models/modular.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12074 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/torch_models/mpnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/torch_models/normalizing_flows_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/torch_models/pagtn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23019 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/torch_models/pna_gnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/torch_models/readout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52726 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/torch_models/torch_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/models/wandblogger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:31:50.603017 deepchem-2.7.2.dev20230703203150/deepchem/molnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/molnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11668 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/molnet/check_availability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/molnet/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14702 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/molnet/dnasim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:31:50.607017 deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/bace_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14202 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/bace_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/bbbc_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/bbbp_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/cell_counting_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/chembl25_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/chembl_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10252 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/chembl_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/clearance_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/clintox_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/delaney_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/factors_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/freesolv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/hiv_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/hopv_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/hppb_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/kaggle_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)   165414 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/kaggle_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/kinase_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/lipo_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9165 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/load_dataset_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:31:50.611017 deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/material_datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/material_datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/material_datasets/load_Pt_NO_surface_adsorbate_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/material_datasets/load_bandgap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/material_datasets/load_mp_formation_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/material_datasets/load_mp_metallicity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/material_datasets/load_perovskite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/molnet_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/muv_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/nci_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/pcba_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8586 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/pdbbind_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/ppb_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/qm7_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/qm8_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/qm9_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/sampl_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/sider_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/sweetlead_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/thermosol_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/tox21_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18900 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/toxcast_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/uspto_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/uv_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/uv_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/zinc15_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/molnet/preset_hyper_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13549 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/molnet/run_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/molnet/run_benchmark_low_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36564 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/molnet/run_benchmark_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:31:50.611017 deepchem-2.7.2.dev20230703203150/deepchem/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23102 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/rl/a2c.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:31:50.611017 deepchem-2.7.2.dev20230703203150/deepchem/rl/envs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/rl/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/rl/envs/test_tictactoe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/rl/envs/tictactoe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25262 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/rl/ppo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:31:50.611017 deepchem-2.7.2.dev20230703203150/deepchem/splits/
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/splits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63895 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/splits/splitters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/splits/task_splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:31:50.611017 deepchem-2.7.2.dev20230703203150/deepchem/trans/
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/trans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/trans/duplicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91191 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/trans/transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:31:50.615017 deepchem-2.7.2.dev20230703203150/deepchem/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/utils/conformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13294 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/utils/coordinate_box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20923 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/utils/debug_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/utils/dftutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10476 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/utils/docking_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13528 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/utils/electron_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19454 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/utils/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/utils/fake_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/utils/fragment_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/utils/genomics_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/utils/geometry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/utils/graph_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/utils/grover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/utils/hash_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19262 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/utils/molecule_feature_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17713 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/utils/noncovalent_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11749 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/utils/pdbqt_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/utils/pytorch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65672 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/utils/rdkit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/utils/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/utils/sequence_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:31:50.619017 deepchem-2.7.2.dev20230703203150/deepchem/utils/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/utils/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/utils/test/test_coordinate_box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/utils/test/test_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/utils/test/test_dftutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/utils/test/test_docking_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/utils/test/test_electron_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12977 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/utils/test/test_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/utils/test/test_fake_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/utils/test/test_fragment_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/utils/test/test_generator_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/utils/test/test_genomics_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/utils/test/test_geometry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/utils/test/test_graph_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/utils/test/test_grover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/utils/test/test_hash_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/utils/test/test_molecule_feature_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/utils/test/test_noncovalent_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/utils/test/test_pdbqt_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/utils/test/test_pytorch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/utils/test/test_rdkit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/utils/test/test_sequence_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/utils/test/test_updated_scipy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/utils/test/test_voxel_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/utils/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/utils/vina_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-07-03 20:31:34.000000 deepchem-2.7.2.dev20230703203150/deepchem/utils/voxel_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 20:31:50.583017 deepchem-2.7.2.dev20230703203150/deepchem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-03 20:31:50.000000 deepchem-2.7.2.dev20230703203150/deepchem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10711 2023-07-03 20:31:50.000000 deepchem-2.7.2.dev20230703203150/deepchem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 20:31:50.000000 deepchem-2.7.2.dev20230703203150/deepchem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-03 20:31:50.000000 deepchem-2.7.2.dev20230703203150/deepchem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-03 20:31:50.000000 deepchem-2.7.2.dev20230703203150/deepchem.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-03 20:31:50.619017 deepchem-2.7.2.dev20230703203150/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-07-03 20:31:35.000000 deepchem-2.7.2.dev20230703203150/setup.py
```

### Comparing `deepchem-2.7.2.dev20230703190634/LICENSE` & `deepchem-2.7.2.dev20230703203150/LICENSE`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/PKG-INFO` & `deepchem-2.7.2.dev20230703203150/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepchem
-Version: 2.7.2.dev20230703190634
+Version: 2.7.2.dev20230703203150
 Summary: Deep learning models for drug discovery,         quantum chemistry, and the life sciences.
 Home-page: https://github.com/deepchem/deepchem
 Maintainer: DeepChem contributors
 License: MIT
 Project-URL: Documentation, https://deepchem.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/deepchem/deepchem
 Keywords: deepchem,chemistry,biology,materials-science,life-science,drug-discovery
```

### Comparing `deepchem-2.7.2.dev20230703190634/README.md` & `deepchem-2.7.2.dev20230703203150/README.md`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/data/__init__.py` & `deepchem-2.7.2.dev20230703203150/deepchem/data/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/data/data_loader.py` & `deepchem-2.7.2.dev20230703203150/deepchem/data/data_loader.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/data/datasets.py` & `deepchem-2.7.2.dev20230703203150/deepchem/data/datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/data/pytorch_datasets.py` & `deepchem-2.7.2.dev20230703203150/deepchem/data/pytorch_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/data/supports.py` & `deepchem-2.7.2.dev20230703203150/deepchem/data/supports.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/dock/binding_pocket.py` & `deepchem-2.7.2.dev20230703203150/deepchem/dock/binding_pocket.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/dock/docking.py` & `deepchem-2.7.2.dev20230703203150/deepchem/dock/docking.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/dock/pose_generation.py` & `deepchem-2.7.2.dev20230703203150/deepchem/dock/pose_generation.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/dock/pose_scoring.py` & `deepchem-2.7.2.dev20230703203150/deepchem/dock/pose_scoring.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/feat/__init__.py` & `deepchem-2.7.2.dev20230703203150/deepchem/feat/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/feat/atomic_conformation.py` & `deepchem-2.7.2.dev20230703203150/deepchem/feat/atomic_conformation.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/feat/base_classes.py` & `deepchem-2.7.2.dev20230703203150/deepchem/feat/base_classes.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/feat/bert_tokenizer.py` & `deepchem-2.7.2.dev20230703203150/deepchem/feat/bert_tokenizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/feat/binding_pocket_features.py` & `deepchem-2.7.2.dev20230703203150/deepchem/feat/binding_pocket_features.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/feat/complex_featurizers/__init__.py` & `deepchem-2.7.2.dev20230703203150/deepchem/feat/complex_featurizers/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/feat/complex_featurizers/complex_atomic_coordinates.py` & `deepchem-2.7.2.dev20230703203150/deepchem/feat/complex_featurizers/complex_atomic_coordinates.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/feat/complex_featurizers/contact_fingerprints.py` & `deepchem-2.7.2.dev20230703203150/deepchem/feat/complex_featurizers/contact_fingerprints.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/feat/complex_featurizers/grid_featurizers.py` & `deepchem-2.7.2.dev20230703203150/deepchem/feat/complex_featurizers/grid_featurizers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/feat/complex_featurizers/rdkit_grid_featurizer.py` & `deepchem-2.7.2.dev20230703203150/deepchem/feat/complex_featurizers/rdkit_grid_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/feat/complex_featurizers/splif_fingerprints.py` & `deepchem-2.7.2.dev20230703203150/deepchem/feat/complex_featurizers/splif_fingerprints.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/feat/dft_data.py` & `deepchem-2.7.2.dev20230703203150/deepchem/feat/dft_data.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/feat/graph_data.py` & `deepchem-2.7.2.dev20230703203150/deepchem/feat/graph_data.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/feat/graph_features.py` & `deepchem-2.7.2.dev20230703203150/deepchem/feat/graph_features.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/feat/huggingface_featurizer.py` & `deepchem-2.7.2.dev20230703203150/deepchem/feat/huggingface_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/feat/material_featurizers/cgcnn_featurizer.py` & `deepchem-2.7.2.dev20230703203150/deepchem/feat/material_featurizers/cgcnn_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/feat/material_featurizers/element_property_fingerprint.py` & `deepchem-2.7.2.dev20230703203150/deepchem/feat/material_featurizers/element_property_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/feat/material_featurizers/elemnet_featurizer.py` & `deepchem-2.7.2.dev20230703203150/deepchem/feat/material_featurizers/elemnet_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/feat/material_featurizers/lcnn_featurizer.py` & `deepchem-2.7.2.dev20230703203150/deepchem/feat/material_featurizers/lcnn_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/feat/material_featurizers/sine_coulomb_matrix.py` & `deepchem-2.7.2.dev20230703203150/deepchem/feat/material_featurizers/sine_coulomb_matrix.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/feat/mol_graphs.py` & `deepchem-2.7.2.dev20230703203150/deepchem/feat/mol_graphs.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/feat/molecule_featurizers/__init__.py` & `deepchem-2.7.2.dev20230703203150/deepchem/feat/molecule_featurizers/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/feat/molecule_featurizers/atomic_coordinates.py` & `deepchem-2.7.2.dev20230703203150/deepchem/feat/molecule_featurizers/atomic_coordinates.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/feat/molecule_featurizers/bp_symmetry_function_input.py` & `deepchem-2.7.2.dev20230703203150/deepchem/feat/molecule_featurizers/bp_symmetry_function_input.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/feat/molecule_featurizers/circular_fingerprint.py` & `deepchem-2.7.2.dev20230703203150/deepchem/feat/molecule_featurizers/circular_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/feat/molecule_featurizers/conformer_featurizer.py` & `deepchem-2.7.2.dev20230703203150/deepchem/feat/molecule_featurizers/conformer_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/feat/molecule_featurizers/coulomb_matrices.py` & `deepchem-2.7.2.dev20230703203150/deepchem/feat/molecule_featurizers/coulomb_matrices.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/feat/molecule_featurizers/dmpnn_featurizer.py` & `deepchem-2.7.2.dev20230703203150/deepchem/feat/molecule_featurizers/dmpnn_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/feat/molecule_featurizers/grover_featurizer.py` & `deepchem-2.7.2.dev20230703203150/deepchem/feat/molecule_featurizers/grover_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/feat/molecule_featurizers/maccs_keys_fingerprint.py` & `deepchem-2.7.2.dev20230703203150/deepchem/feat/molecule_featurizers/maccs_keys_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/feat/molecule_featurizers/mat_featurizer.py` & `deepchem-2.7.2.dev20230703203150/deepchem/feat/molecule_featurizers/mat_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/feat/molecule_featurizers/mol2vec_fingerprint.py` & `deepchem-2.7.2.dev20230703203150/deepchem/feat/molecule_featurizers/mol2vec_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/feat/molecule_featurizers/mol_graph_conv_featurizer.py` & `deepchem-2.7.2.dev20230703203150/deepchem/feat/molecule_featurizers/mol_graph_conv_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/feat/molecule_featurizers/molgan_featurizer.py` & `deepchem-2.7.2.dev20230703203150/deepchem/feat/molecule_featurizers/molgan_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/feat/molecule_featurizers/mordred_descriptors.py` & `deepchem-2.7.2.dev20230703203150/deepchem/feat/molecule_featurizers/mordred_descriptors.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/feat/molecule_featurizers/one_hot_featurizer.py` & `deepchem-2.7.2.dev20230703203150/deepchem/feat/molecule_featurizers/one_hot_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/feat/molecule_featurizers/pubchem_fingerprint.py` & `deepchem-2.7.2.dev20230703203150/deepchem/feat/molecule_featurizers/pubchem_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/feat/molecule_featurizers/raw_featurizer.py` & `deepchem-2.7.2.dev20230703203150/deepchem/feat/molecule_featurizers/raw_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/feat/molecule_featurizers/rdkit_descriptors.py` & `deepchem-2.7.2.dev20230703203150/deepchem/feat/molecule_featurizers/rdkit_descriptors.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/feat/molecule_featurizers/smiles_to_image.py` & `deepchem-2.7.2.dev20230703203150/deepchem/feat/molecule_featurizers/smiles_to_image.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/feat/molecule_featurizers/smiles_to_seq.py` & `deepchem-2.7.2.dev20230703203150/deepchem/feat/molecule_featurizers/smiles_to_seq.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/feat/molecule_featurizers/snap_featurizer.py` & `deepchem-2.7.2.dev20230703203150/deepchem/feat/molecule_featurizers/snap_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/feat/molecule_featurizers/sparse_matrix_one_hot_featurizer.py` & `deepchem-2.7.2.dev20230703203150/deepchem/feat/molecule_featurizers/sparse_matrix_one_hot_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/feat/reaction_featurizer.py` & `deepchem-2.7.2.dev20230703203150/deepchem/feat/reaction_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/feat/roberta_tokenizer.py` & `deepchem-2.7.2.dev20230703203150/deepchem/feat/roberta_tokenizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/feat/sequence_featurizers/position_frequency_matrix_featurizer.py` & `deepchem-2.7.2.dev20230703203150/deepchem/feat/sequence_featurizers/position_frequency_matrix_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/feat/smiles_tokenizer.py` & `deepchem-2.7.2.dev20230703203150/deepchem/feat/smiles_tokenizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/feat/vocabulary_builders/grover_vocab.py` & `deepchem-2.7.2.dev20230703203150/deepchem/feat/vocabulary_builders/grover_vocab.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/feat/vocabulary_builders/hf_vocab.py` & `deepchem-2.7.2.dev20230703203150/deepchem/feat/vocabulary_builders/hf_vocab.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/feat/vocabulary_builders/vocabulary_builder.py` & `deepchem-2.7.2.dev20230703203150/deepchem/feat/vocabulary_builders/vocabulary_builder.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/hyper/base_classes.py` & `deepchem-2.7.2.dev20230703203150/deepchem/hyper/base_classes.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/hyper/gaussian_process.py` & `deepchem-2.7.2.dev20230703203150/deepchem/hyper/gaussian_process.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/hyper/grid_search.py` & `deepchem-2.7.2.dev20230703203150/deepchem/hyper/grid_search.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/hyper/random_search.py` & `deepchem-2.7.2.dev20230703203150/deepchem/hyper/random_search.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/metalearning/maml.py` & `deepchem-2.7.2.dev20230703203150/deepchem/metalearning/maml.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/metrics/__init__.py` & `deepchem-2.7.2.dev20230703203150/deepchem/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/metrics/genomic_metrics.py` & `deepchem-2.7.2.dev20230703203150/deepchem/metrics/genomic_metrics.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/metrics/metric.py` & `deepchem-2.7.2.dev20230703203150/deepchem/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/metrics/score_function.py` & `deepchem-2.7.2.dev20230703203150/deepchem/metrics/score_function.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/models/IRV.py` & `deepchem-2.7.2.dev20230703203150/deepchem/models/IRV.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/models/__init__.py` & `deepchem-2.7.2.dev20230703203150/deepchem/models/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/models/atomic_conv.py` & `deepchem-2.7.2.dev20230703203150/deepchem/models/atomic_conv.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/models/callbacks.py` & `deepchem-2.7.2.dev20230703203150/deepchem/models/callbacks.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/models/chemnet_layers.py` & `deepchem-2.7.2.dev20230703203150/deepchem/models/chemnet_layers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/models/chemnet_models.py` & `deepchem-2.7.2.dev20230703203150/deepchem/models/chemnet_models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/models/dft/dftxc.py` & `deepchem-2.7.2.dev20230703203150/deepchem/models/dft/dftxc.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/models/dft/nnxc.py` & `deepchem-2.7.2.dev20230703203150/deepchem/models/dft/nnxc.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/models/dft/scf.py` & `deepchem-2.7.2.dev20230703203150/deepchem/models/dft/scf.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/models/fcnet.py` & `deepchem-2.7.2.dev20230703203150/deepchem/models/fcnet.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/models/gan.py` & `deepchem-2.7.2.dev20230703203150/deepchem/models/gan.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/models/gbdt_models/gbdt_model.py` & `deepchem-2.7.2.dev20230703203150/deepchem/models/gbdt_models/gbdt_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/models/graph_models.py` & `deepchem-2.7.2.dev20230703203150/deepchem/models/graph_models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/models/jax_models/jax_model.py` & `deepchem-2.7.2.dev20230703203150/deepchem/models/jax_models/jax_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/models/jax_models/layers.py` & `deepchem-2.7.2.dev20230703203150/deepchem/models/jax_models/layers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/models/jax_models/pinns_model.py` & `deepchem-2.7.2.dev20230703203150/deepchem/models/jax_models/pinns_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/models/keras_model.py` & `deepchem-2.7.2.dev20230703203150/deepchem/models/keras_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/models/layers.py` & `deepchem-2.7.2.dev20230703203150/deepchem/models/layers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/models/lightning/dc_lightning_dataset_module.py` & `deepchem-2.7.2.dev20230703203150/deepchem/models/lightning/dc_lightning_dataset_module.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/models/lightning/dc_lightning_module.py` & `deepchem-2.7.2.dev20230703203150/deepchem/models/lightning/dc_lightning_module.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/models/losses.py` & `deepchem-2.7.2.dev20230703203150/deepchem/models/losses.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/models/models.py` & `deepchem-2.7.2.dev20230703203150/deepchem/models/models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/models/molgan.py` & `deepchem-2.7.2.dev20230703203150/deepchem/models/molgan.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/models/multitask.py` & `deepchem-2.7.2.dev20230703203150/deepchem/models/multitask.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/models/normalizing_flows.py` & `deepchem-2.7.2.dev20230703203150/deepchem/models/normalizing_flows.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/models/optimizers.py` & `deepchem-2.7.2.dev20230703203150/deepchem/models/optimizers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/models/progressive_multitask.py` & `deepchem-2.7.2.dev20230703203150/deepchem/models/progressive_multitask.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/models/robust_multitask.py` & `deepchem-2.7.2.dev20230703203150/deepchem/models/robust_multitask.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/models/scscore.py` & `deepchem-2.7.2.dev20230703203150/deepchem/models/scscore.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/models/seqtoseq.py` & `deepchem-2.7.2.dev20230703203150/deepchem/models/seqtoseq.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/models/sklearn_models/sklearn_model.py` & `deepchem-2.7.2.dev20230703203150/deepchem/models/sklearn_models/sklearn_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/models/text_cnn.py` & `deepchem-2.7.2.dev20230703203150/deepchem/models/text_cnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/models/torch_models/__init__.py` & `deepchem-2.7.2.dev20230703203150/deepchem/models/torch_models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from deepchem.models.torch_models.infograph import InfoGraphStar, InfoGraphStarModel, InfoGraphEncoder, GINEncoder, InfoGraph, InfoGraphModel, InfoGraphEncoder
 from deepchem.models.torch_models.mpnn import MPNN, MPNNModel
 from deepchem.models.torch_models.lcnn import LCNN, LCNNModel
 from deepchem.models.torch_models.pagtn import Pagtn, PagtnModel
 from deepchem.models.torch_models.mat import MAT, MATModel
 from deepchem.models.torch_models.megnet import MEGNetModel
 from deepchem.models.torch_models.normalizing_flows_pytorch import NormalizingFlow
-from deepchem.models.torch_models.layers import MultilayerPerceptron, CNNModule, CombineMeanStd, WeightedLinearCombo, AtomicConvolution, NeighborList, SetGather, EdgeNetwork, WeaveLayer
+from deepchem.models.torch_models.layers import MultilayerPerceptron, CNNModule, CombineMeanStd, WeightedLinearCombo, AtomicConvolution, NeighborList, SetGather, EdgeNetwork, WeaveLayer, MolGANConvolutionLayer
 from deepchem.models.torch_models.cnn import CNN
 from deepchem.models.torch_models.attention import ScaledDotProductAttention, SelfAttention
 from deepchem.models.torch_models.grover import GroverModel, GroverPretrain, GroverFinetune
 from deepchem.models.torch_models.readout import GroverReadout
 try:
     from deepchem.models.torch_models.dmpnn import DMPNN, DMPNNModel
     from deepchem.models.torch_models.gnn import GNN, GNNHead, GNNModular
```

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/models/torch_models/attention.py` & `deepchem-2.7.2.dev20230703203150/deepchem/models/torch_models/attention.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/models/torch_models/attentivefp.py` & `deepchem-2.7.2.dev20230703203150/deepchem/models/torch_models/attentivefp.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/models/torch_models/cgcnn.py` & `deepchem-2.7.2.dev20230703203150/deepchem/models/torch_models/cgcnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/models/torch_models/chemberta.py` & `deepchem-2.7.2.dev20230703203150/deepchem/models/torch_models/chemberta.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/models/torch_models/cnn.py` & `deepchem-2.7.2.dev20230703203150/deepchem/models/torch_models/cnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/models/torch_models/dmpnn.py` & `deepchem-2.7.2.dev20230703203150/deepchem/models/torch_models/dmpnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/models/torch_models/ferminet.py` & `deepchem-2.7.2.dev20230703203150/deepchem/models/torch_models/ferminet.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/models/torch_models/gat.py` & `deepchem-2.7.2.dev20230703203150/deepchem/models/torch_models/gat.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/models/torch_models/gcn.py` & `deepchem-2.7.2.dev20230703203150/deepchem/models/torch_models/gcn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/models/torch_models/gnn.py` & `deepchem-2.7.2.dev20230703203150/deepchem/models/torch_models/gnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/models/torch_models/gnn3d.py` & `deepchem-2.7.2.dev20230703203150/deepchem/models/torch_models/gnn3d.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/models/torch_models/grover.py` & `deepchem-2.7.2.dev20230703203150/deepchem/models/torch_models/grover.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/models/torch_models/grover_layers.py` & `deepchem-2.7.2.dev20230703203150/deepchem/models/torch_models/grover_layers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/models/torch_models/hf_models.py` & `deepchem-2.7.2.dev20230703203150/deepchem/models/torch_models/hf_models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/models/torch_models/infograph.py` & `deepchem-2.7.2.dev20230703203150/deepchem/models/torch_models/infograph.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/models/torch_models/kfac_optimizer.py` & `deepchem-2.7.2.dev20230703203150/deepchem/models/torch_models/kfac_optimizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/models/torch_models/layers.py` & `deepchem-2.7.2.dev20230703203150/deepchem/models/torch_models/layers.py`

 * *Files 1% similar despite different names*

```diff
@@ -7407,1405 +7407,1704 @@
 0001cee0: 6572 2c0a 2020 2020 2020 2020 2020 2020  er,.            
 0001cef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001cf00: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001cf10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
 0001cf20: 2e65 6d62 6564 6469 6e67 5f6c 6973 7429  .embedding_list)
 0001cf30: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
 0001cf40: 6174 6f6d 5f65 6e62 6564 6469 6e67 730a  atom_enbeddings.
-0001cf50: 0a0a 636c 6173 7320 4454 4e4e 5374 6570  ..class DTNNStep
-0001cf60: 286e 6e2e 4d6f 6475 6c65 293a 0a20 2020  (nn.Module):.   
-0001cf70: 2022 2222 4454 4e4e 5374 6570 204c 6179   """DTNNStep Lay
-0001cf80: 6572 2066 6f72 2044 544e 4e20 6d6f 6465  er for DTNN mode
-0001cf90: 6c2e 0a0a 2020 2020 456e 636f 6465 7320  l...    Encodes 
-0001cfa0: 7468 6520 6174 6f6d 2773 2069 6e74 6572  the atom's inter
-0001cfb0: 6163 7469 6f6e 2077 6974 6820 6f74 6865  action with othe
-0001cfc0: 7220 6174 6f6d 7320 6163 636f 7264 696e  r atoms accordin
-0001cfd0: 6720 746f 2064 6973 7461 6e63 6520 7265  g to distance re
-0001cfe0: 6c61 7469 6f6e 7368 6970 732e 205b 315d  lationships. [1]
-0001cff0: 5f0a 0a20 2020 2054 6869 7320 4c61 7965  _..    This Laye
-0001d000: 7220 696d 706c 656d 656e 7473 2074 6865  r implements the
-0001d010: 2045 7120 2837 2920 6672 6f6d 2044 544e   Eq (7) from DTN
-0001d020: 4e20 5061 7065 722e 2054 6865 6e20 7375  N Paper. Then su
-0001d030: 6d73 2074 6865 6d20 7570 2074 6f20 6765  ms them up to ge
-0001d040: 7420 7468 6520 6669 6e61 6c20 6f75 7470  t the final outp
-0001d050: 7574 2075 7369 6e67 2045 7120 2836 2920  ut using Eq (6) 
-0001d060: 6672 6f6d 2044 544e 4e20 5061 7065 722e  from DTNN Paper.
-0001d070: 0a0a 2020 2020 4571 2028 3729 3a20 565f  ..    Eq (7): V_
-0001d080: 696a 203d 2074 616e 685b 575f 6663 202e  ij = tanh[W_fc .
-0001d090: 2028 2857 5f63 6620 2e20 435f 6a20 2b20   ((W_cf . C_j + 
-0001d0a0: 625f 6366 2920 2a20 2857 5f64 6620 2e20  b_cf) * (W_df . 
-0001d0b0: 645f 696a 202b 2062 5f64 6629 295d 0a0a  d_ij + b_df))]..
-0001d0c0: 2020 2020 4571 2028 3629 3a20 435f 6920      Eq (6): C_i 
-0001d0d0: 3d20 435f 6920 2b20 7375 6d28 565f 696a  = C_i + sum(V_ij
-0001d0e0: 290a 0a20 2020 2048 6572 6520 3a20 272e  )..    Here : '.
-0001d0f0: 273d 4d61 7472 6978 204d 756c 7469 706c  '=Matrix Multipl
-0001d100: 6963 6174 696f 6e20 2c20 272a 273d 4d75  ication , '*'=Mu
-0001d110: 6c74 6970 6c69 6361 7469 6f6e 0a0a 2020  ltiplication..  
-0001d120: 2020 5265 6665 7265 6e63 6573 0a20 2020    References.   
-0001d130: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-0001d140: 5b31 5d20 5363 68c3 bc74 742c 204b 7269  [1] Sch..tt, Kri
-0001d150: 7374 6f66 2054 2e2c 2065 7420 616c 2e20  stof T., et al. 
-0001d160: 2251 7561 6e74 756d 2d63 6865 6d69 6361  "Quantum-chemica
-0001d170: 6c20 696e 7369 6768 7473 2066 726f 6d20  l insights from 
-0001d180: 6465 6570 0a20 2020 2020 2020 2074 656e  deep.        ten
-0001d190: 736f 7220 6e65 7572 616c 206e 6574 776f  sor neural netwo
-0001d1a0: 726b 732e 2220 4e61 7475 7265 2063 6f6d  rks." Nature com
-0001d1b0: 6d75 6e69 6361 7469 6f6e 7320 382e 3120  munications 8.1 
-0001d1c0: 2832 3031 3729 3a20 312d 382e 0a0a 2020  (2017): 1-8...  
-0001d1d0: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
-0001d1e0: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-0001d1f0: 6e5f 656d 6265 6464 696e 673a 2069 6e74  n_embedding: int
-0001d200: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
-0001d210: 2020 204e 756d 6265 7220 6f66 2066 6561     Number of fea
-0001d220: 7475 7265 7320 666f 7220 6561 6368 2061  tures for each a
-0001d230: 746f 6d0a 2020 2020 6e5f 6469 7374 616e  tom.    n_distan
-0001d240: 6365 3a20 696e 742c 206f 7074 696f 6e61  ce: int, optiona
-0001d250: 6c0a 2020 2020 2020 2020 6772 616e 756c  l.        granul
-0001d260: 6172 6974 7920 6f66 2064 6973 7461 6e63  arity of distanc
-0001d270: 6520 6d61 7472 6978 0a20 2020 206e 5f68  e matrix.    n_h
-0001d280: 6964 6465 6e3a 2069 6e74 2c20 6f70 7469  idden: int, opti
-0001d290: 6f6e 616c 0a20 2020 2020 2020 204e 756d  onal.        Num
-0001d2a0: 6265 7220 6f66 206e 6f64 6573 2069 6e20  ber of nodes in 
-0001d2b0: 6869 6464 656e 206c 6179 6572 0a20 2020  hidden layer.   
-0001d2c0: 2069 6e69 7469 616c 697a 6572 3a20 7374   initializer: st
-0001d2d0: 722c 206f 7074 696f 6e61 6c0a 2020 2020  r, optional.    
-0001d2e0: 2020 2020 5765 6967 6874 2069 6e69 7469      Weight initi
-0001d2f0: 616c 697a 6174 696f 6e20 666f 7220 6669  alization for fi
-0001d300: 6c74 6572 732e 0a20 2020 2020 2020 204f  lters..        O
-0001d310: 7074 696f 6e73 3a20 7b78 6176 6965 725f  ptions: {xavier_
-0001d320: 756e 6966 6f72 6d5f 2c20 7861 7669 6572  uniform_, xavier
-0001d330: 5f6e 6f72 6d61 6c5f 2c20 6b61 696d 696e  _normal_, kaimin
-0001d340: 675f 756e 6966 6f72 6d5f 2c20 6b61 696d  g_uniform_, kaim
-0001d350: 696e 675f 6e6f 726d 616c 5f2c 2074 7275  ing_normal_, tru
-0001d360: 6e63 5f6e 6f72 6d61 6c5f 7d0a 2020 2020  nc_normal_}.    
-0001d370: 6163 7469 7661 7469 6f6e 3a20 7374 722c  activation: str,
-0001d380: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
-0001d390: 2020 4163 7469 7661 7469 6f6e 2066 756e    Activation fun
-0001d3a0: 6374 696f 6e20 6170 706c 6965 640a 0a20  ction applied.. 
-0001d3b0: 2020 2045 7861 6d70 6c65 730a 2020 2020     Examples.    
-0001d3c0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 203e 3e3e  --------.    >>>
-0001d3d0: 2066 726f 6d20 6465 6570 6368 656d 2e6d   from deepchem.m
-0001d3e0: 6f64 656c 732e 746f 7263 685f 6d6f 6465  odels.torch_mode
-0001d3f0: 6c73 2069 6d70 6f72 7420 6c61 7965 7273  ls import layers
-0001d400: 0a20 2020 203e 3e3e 2069 6d70 6f72 7420  .    >>> import 
-0001d410: 746f 7263 680a 2020 2020 3e3e 3e20 656d  torch.    >>> em
-0001d420: 6265 6464 696e 675f 6c61 7965 7220 3d20  bedding_layer = 
-0001d430: 6c61 7965 7273 2e44 544e 4e45 6d62 6564  layers.DTNNEmbed
-0001d440: 6469 6e67 2834 2c20 3429 0a20 2020 203e  ding(4, 4).    >
-0001d450: 3e3e 2065 6d62 203d 2065 6d62 6564 6469  >> emb = embeddi
-0001d460: 6e67 5f6c 6179 6572 2874 6f72 6368 2e54  ng_layer(torch.T
-0001d470: 656e 736f 7228 5b30 2c31 2c32 2c33 5d29  ensor([0,1,2,3])
-0001d480: 2e74 6f28 746f 7263 682e 696e 7436 3429  .to(torch.int64)
-0001d490: 290a 2020 2020 3e3e 3e20 7374 6570 5f6c  ).    >>> step_l
-0001d4a0: 6179 6572 203d 206c 6179 6572 732e 4454  ayer = layers.DT
-0001d4b0: 4e4e 5374 6570 2834 2c20 362c 2038 290a  NNStep(4, 6, 8).
-0001d4c0: 2020 2020 3e3e 3e20 6f75 7470 7574 5f74      >>> output_t
-0001d4d0: 6f72 6368 203d 2073 7465 705f 6c61 7965  orch = step_laye
-0001d4e0: 7228 5b0a 2020 2020 2e2e 2e20 2020 2020  r([.    ...     
-0001d4f0: 746f 7263 682e 5465 6e73 6f72 2865 6d62  torch.Tensor(emb
-0001d500: 292c 0a20 2020 202e 2e2e 2020 2020 2074  ),.    ...     t
-0001d510: 6f72 6368 2e54 656e 736f 7228 5b30 2c20  orch.Tensor([0, 
-0001d520: 312c 2032 2c20 332c 2034 2c20 355d 292e  1, 2, 3, 4, 5]).
-0001d530: 746f 2874 6f72 6368 2e66 6c6f 6174 3332  to(torch.float32
-0001d540: 292c 0a20 2020 202e 2e2e 2020 2020 2074  ),.    ...     t
-0001d550: 6f72 6368 2e54 656e 736f 7228 5b31 5d29  orch.Tensor([1])
-0001d560: 2e74 6f28 746f 7263 682e 696e 7436 3429  .to(torch.int64)
-0001d570: 2c0a 2020 2020 2e2e 2e20 2020 2020 746f  ,.    ...     to
-0001d580: 7263 682e 5465 6e73 6f72 285b 5b31 5d5d  rch.Tensor([[1]]
-0001d590: 292e 746f 2874 6f72 6368 2e69 6e74 3634  ).to(torch.int64
-0001d5a0: 290a 2020 2020 2e2e 2e20 5d29 0a20 2020  ).    ... ]).   
-0001d5b0: 203e 3e3e 206f 7574 7075 745f 746f 7263   >>> output_torc
-0001d5c0: 682e 7368 6170 650a 2020 2020 746f 7263  h.shape.    torc
-0001d5d0: 682e 5369 7a65 285b 322c 2034 2c20 345d  h.Size([2, 4, 4]
-0001d5e0: 290a 0a20 2020 2022 2222 0a0a 2020 2020  )..    """..    
-0001d5f0: 6465 6620 5f5f 696e 6974 5f5f 2873 656c  def __init__(sel
-0001d600: 662c 0a20 2020 2020 2020 2020 2020 2020  f,.             
-0001d610: 2020 2020 6e5f 656d 6265 6464 696e 673a      n_embedding:
-0001d620: 2069 6e74 203d 2033 302c 0a20 2020 2020   int = 30,.     
-0001d630: 2020 2020 2020 2020 2020 2020 6e5f 6469              n_di
-0001d640: 7374 616e 6365 3a20 696e 7420 3d20 3130  stance: int = 10
-0001d650: 302c 0a20 2020 2020 2020 2020 2020 2020  0,.             
-0001d660: 2020 2020 6e5f 6869 6464 656e 3a20 696e      n_hidden: in
-0001d670: 7420 3d20 3630 2c0a 2020 2020 2020 2020  t = 60,.        
-0001d680: 2020 2020 2020 2020 2069 6e69 7469 616c           initial
-0001d690: 697a 6572 3a20 7374 7220 3d20 2778 6176  izer: str = 'xav
-0001d6a0: 6965 725f 756e 6966 6f72 6d5f 272c 0a20  ier_uniform_',. 
-0001d6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d6c0: 6163 7469 7661 7469 6f6e 3d27 7461 6e68  activation='tanh
-0001d6d0: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
-0001d6e0: 2020 2020 2a2a 6b77 6172 6773 293a 0a0a      **kwargs):..
-0001d6f0: 2020 2020 2020 2020 7375 7065 7228 4454          super(DT
-0001d700: 4e4e 5374 6570 2c20 7365 6c66 292e 5f5f  NNStep, self).__
-0001d710: 696e 6974 5f5f 282a 2a6b 7761 7267 7329  init__(**kwargs)
-0001d720: 0a20 2020 2020 2020 2073 656c 662e 6e5f  .        self.n_
-0001d730: 656d 6265 6464 696e 6720 3d20 6e5f 656d  embedding = n_em
-0001d740: 6265 6464 696e 670a 2020 2020 2020 2020  bedding.        
-0001d750: 7365 6c66 2e6e 5f64 6973 7461 6e63 6520  self.n_distance 
-0001d760: 3d20 6e5f 6469 7374 616e 6365 0a20 2020  = n_distance.   
-0001d770: 2020 2020 2073 656c 662e 6e5f 6869 6464       self.n_hidd
-0001d780: 656e 203d 206e 5f68 6964 6465 6e0a 2020  en = n_hidden.  
-0001d790: 2020 2020 2020 7365 6c66 2e69 6e69 7469        self.initi
-0001d7a0: 616c 697a 6572 203d 2069 6e69 7469 616c  alizer = initial
-0001d7b0: 697a 6572 2020 2320 5365 7420 7765 6967  izer  # Set weig
-0001d7c0: 6874 2069 6e69 7469 616c 697a 6174 696f  ht initializatio
-0001d7d0: 6e0a 2020 2020 2020 2020 7365 6c66 2e61  n.        self.a
-0001d7e0: 6374 6976 6174 696f 6e20 3d20 6163 7469  ctivation = acti
-0001d7f0: 7661 7469 6f6e 2020 2320 4765 7420 6163  vation  # Get ac
-0001d800: 7469 7661 7469 6f6e 730a 2020 2020 2020  tivations.      
-0001d810: 2020 7365 6c66 2e61 6374 6976 6174 696f    self.activatio
-0001d820: 6e5f 666e 203d 2067 6574 5f61 6374 6976  n_fn = get_activ
-0001d830: 6174 696f 6e28 7365 6c66 2e61 6374 6976  ation(self.activ
-0001d840: 6174 696f 6e29 0a0a 2020 2020 2020 2020  ation)..        
-0001d850: 696e 6974 5f66 756e 633a 2043 616c 6c61  init_func: Calla
-0001d860: 626c 6520 3d20 6765 7461 7474 7228 696e  ble = getattr(in
-0001d870: 6974 6961 6c69 7a65 7273 2c20 7365 6c66  itializers, self
-0001d880: 2e69 6e69 7469 616c 697a 6572 290a 0a20  .initializer).. 
-0001d890: 2020 2020 2020 2073 656c 662e 575f 6366         self.W_cf
-0001d8a0: 203d 2069 6e69 745f 6675 6e63 2874 6f72   = init_func(tor
-0001d8b0: 6368 2e65 6d70 7479 285b 7365 6c66 2e6e  ch.empty([self.n
-0001d8c0: 5f65 6d62 6564 6469 6e67 2c20 7365 6c66  _embedding, self
-0001d8d0: 2e6e 5f68 6964 6465 6e5d 2929 0a20 2020  .n_hidden])).   
-0001d8e0: 2020 2020 2073 656c 662e 575f 6466 203d       self.W_df =
-0001d8f0: 2069 6e69 745f 6675 6e63 2874 6f72 6368   init_func(torch
-0001d900: 2e65 6d70 7479 285b 7365 6c66 2e6e 5f64  .empty([self.n_d
-0001d910: 6973 7461 6e63 652c 2073 656c 662e 6e5f  istance, self.n_
-0001d920: 6869 6464 656e 5d29 290a 2020 2020 2020  hidden])).      
-0001d930: 2020 7365 6c66 2e57 5f66 6320 3d20 696e    self.W_fc = in
-0001d940: 6974 5f66 756e 6328 746f 7263 682e 656d  it_func(torch.em
-0001d950: 7074 7928 5b73 656c 662e 6e5f 6869 6464  pty([self.n_hidd
-0001d960: 656e 2c20 7365 6c66 2e6e 5f65 6d62 6564  en, self.n_embed
-0001d970: 6469 6e67 5d29 290a 2020 2020 2020 2020  ding])).        
-0001d980: 7365 6c66 2e62 5f63 6620 3d20 746f 7263  self.b_cf = torc
-0001d990: 682e 7a65 726f 7328 7369 7a65 3d5b 0a20  h.zeros(size=[. 
-0001d9a0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0001d9b0: 6e5f 6869 6464 656e 2c0a 2020 2020 2020  n_hidden,.      
-0001d9c0: 2020 5d29 0a20 2020 2020 2020 2073 656c    ]).        sel
-0001d9d0: 662e 625f 6466 203d 2074 6f72 6368 2e7a  f.b_df = torch.z
-0001d9e0: 6572 6f73 2873 697a 653d 5b0a 2020 2020  eros(size=[.    
-0001d9f0: 2020 2020 2020 2020 7365 6c66 2e6e 5f68          self.n_h
-0001da00: 6964 6465 6e2c 0a20 2020 2020 2020 205d  idden,.        ]
-0001da10: 290a 0a20 2020 2064 6566 205f 5f72 6570  )..    def __rep
-0001da20: 725f 5f28 7365 6c66 293a 0a20 2020 2020  r__(self):.     
-0001da30: 2020 2022 2222 5265 7475 726e 7320 6120     """Returns a 
-0001da40: 7374 7269 6e67 2072 6570 7265 7365 6e74  string represent
-0001da50: 696e 6720 7468 6520 636f 6e66 6967 7572  ing the configur
-0001da60: 6174 696f 6e20 6f66 2074 6865 206c 6179  ation of the lay
-0001da70: 6572 2e0a 0a20 2020 2020 2020 2052 6574  er...        Ret
-0001da80: 7572 6e73 0a20 2020 2020 2020 202d 2d2d  urns.        ---
-0001da90: 2d2d 2d2d 0a20 2020 2020 2020 206e 5f65  ----.        n_e
-0001daa0: 6d62 6564 6469 6e67 3a20 696e 742c 206f  mbedding: int, o
-0001dab0: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
-0001dac0: 2020 2020 4e75 6d62 6572 206f 6620 6665      Number of fe
-0001dad0: 6174 7572 6573 2066 6f72 2065 6163 6820  atures for each 
-0001dae0: 6174 6f6d 0a20 2020 2020 2020 206e 5f64  atom.        n_d
-0001daf0: 6973 7461 6e63 653a 2069 6e74 2c20 6f70  istance: int, op
-0001db00: 7469 6f6e 616c 0a20 2020 2020 2020 2020  tional.         
-0001db10: 2020 2067 7261 6e75 6c61 7269 7479 206f     granularity o
-0001db20: 6620 6469 7374 616e 6365 206d 6174 7269  f distance matri
-0001db30: 780a 2020 2020 2020 2020 6e5f 6869 6464  x.        n_hidd
-0001db40: 656e 3a20 696e 742c 206f 7074 696f 6e61  en: int, optiona
-0001db50: 6c0a 2020 2020 2020 2020 2020 2020 4e75  l.            Nu
-0001db60: 6d62 6572 206f 6620 6e6f 6465 7320 696e  mber of nodes in
-0001db70: 2068 6964 6465 6e20 6c61 7965 720a 2020   hidden layer.  
-0001db80: 2020 2020 2020 696e 6974 6961 6c69 7a65        initialize
-0001db90: 723a 2073 7472 2c20 6f70 7469 6f6e 616c  r: str, optional
-0001dba0: 0a20 2020 2020 2020 2020 2020 2057 6569  .            Wei
-0001dbb0: 6768 7420 696e 6974 6961 6c69 7a61 7469  ght initializati
-0001dbc0: 6f6e 2066 6f72 2066 696c 7465 7273 2e0a  on for filters..
-0001dbd0: 2020 2020 2020 2020 2020 2020 4f70 7469              Opti
-0001dbe0: 6f6e 733a 207b 7861 7669 6572 5f75 6e69  ons: {xavier_uni
-0001dbf0: 666f 726d 5f2c 2078 6176 6965 725f 6e6f  form_, xavier_no
-0001dc00: 726d 616c 5f2c 206b 6169 6d69 6e67 5f75  rmal_, kaiming_u
-0001dc10: 6e69 666f 726d 5f2c 206b 6169 6d69 6e67  niform_, kaiming
-0001dc20: 5f6e 6f72 6d61 6c5f 2c20 7472 756e 635f  _normal_, trunc_
-0001dc30: 6e6f 726d 616c 5f7d 0a20 2020 2020 2020  normal_}.       
-0001dc40: 2061 6374 6976 6174 696f 6e3a 2073 7472   activation: str
-0001dc50: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
-0001dc60: 2020 2020 2020 2041 6374 6976 6174 696f         Activatio
-0001dc70: 6e20 6675 6e63 7469 6f6e 2061 7070 6c69  n function appli
-0001dc80: 6564 0a0a 2020 2020 2020 2020 2222 220a  ed..        """.
-0001dc90: 2020 2020 2020 2020 7265 7475 726e 2066          return f
-0001dca0: 277b 7365 6c66 2e5f 5f63 6c61 7373 5f5f  '{self.__class__
-0001dcb0: 2e5f 5f6e 616d 655f 5f7d 286e 5f65 6d62  .__name__}(n_emb
-0001dcc0: 6564 6469 6e67 3d7b 7365 6c66 2e6e 5f65  edding={self.n_e
-0001dcd0: 6d62 6564 6469 6e67 7d2c 206e 5f64 6973  mbedding}, n_dis
-0001dce0: 7461 6e63 653d 7b73 656c 662e 6e5f 6469  tance={self.n_di
-0001dcf0: 7374 616e 6365 7d2c 206e 5f68 6964 6465  stance}, n_hidde
-0001dd00: 6e3d 7b73 656c 662e 6e5f 6869 6464 656e  n={self.n_hidden
-0001dd10: 7d2c 2069 6e69 7469 616c 697a 6572 3d7b  }, initializer={
-0001dd20: 7365 6c66 2e69 6e69 7469 616c 697a 6572  self.initializer
-0001dd30: 7d2c 2061 6374 6976 6174 696f 6e3d 7b73  }, activation={s
-0001dd40: 656c 662e 6163 7469 7661 7469 6f6e 7d29  elf.activation})
-0001dd50: 270a 0a20 2020 2064 6566 2066 6f72 7761  '..    def forwa
-0001dd60: 7264 2873 656c 662c 2069 6e70 7574 7329  rd(self, inputs)
-0001dd70: 3a0a 2020 2020 2020 2020 2222 2245 7865  :.        """Exe
-0001dd80: 6375 7465 7320 7468 6520 6571 7561 7469  cutes the equati
-0001dd90: 6f6e 7320 616e 6420 5265 7475 726e 7320  ons and Returns 
-0001dda0: 7468 6520 696e 7472 6163 7469 6f6e 2076  the intraction v
-0001ddb0: 6563 746f 7220 6f66 2074 6865 2061 746f  ector of the ato
-0001ddc0: 6d20 7769 7468 206f 7468 6572 2061 746f  m with other ato
-0001ddd0: 6d73 2e0a 0a20 2020 2020 2020 2050 6172  ms...        Par
-0001dde0: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
-0001ddf0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
-0001de00: 2020 2069 6e70 7574 733a 2074 6f72 6368     inputs: torch
-0001de10: 2e54 656e 736f 720a 2020 2020 2020 2020  .Tensor.        
-0001de20: 2020 2020 4c69 7374 206f 6620 5465 6e73      List of Tens
-0001de30: 6f72 7320 6861 7669 6e67 2061 746f 6d5f  ors having atom_
-0001de40: 6665 6174 7572 6573 2c20 6469 7374 616e  features, distan
-0001de50: 6365 2c20 6469 7374 616e 6365 5f6d 656d  ce, distance_mem
-0001de60: 6265 7273 6869 705f 692c 2064 6973 7461  bership_i, dista
-0001de70: 6e63 655f 6d65 6d62 6572 7368 6970 5f6a  nce_membership_j
-0001de80: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-0001de90: 6e73 0a20 2020 2020 2020 202d 2d2d 2d2d  ns.        -----
-0001dea0: 2d2d 0a20 2020 2020 2020 2069 6e74 6572  --.        inter
-0001deb0: 6163 7469 6f6e 5f76 6563 746f 723a 2074  action_vector: t
-0001dec0: 6f72 6368 2e54 656e 736f 720a 2020 2020  orch.Tensor.    
-0001ded0: 2020 2020 2020 2020 696e 7465 7261 6374          interact
-0001dee0: 696f 6e20 6f66 2074 6865 2061 746f 6d20  ion of the atom 
-0001def0: 7769 7468 206f 7468 6572 2061 746f 6d73  with other atoms
-0001df00: 2062 6173 6564 206f 6e20 6469 7374 616e   based on distan
-0001df10: 6365 2061 6e64 2064 6973 7461 6e63 655f  ce and distance_
-0001df20: 6d65 6d62 6572 7368 6970 2e0a 0a20 2020  membership...   
-0001df30: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0001df40: 2061 746f 6d5f 6665 6174 7572 6573 203d   atom_features =
-0001df50: 2069 6e70 7574 735b 305d 0a20 2020 2020   inputs[0].     
-0001df60: 2020 2064 6973 7461 6e63 6520 3d20 696e     distance = in
-0001df70: 7075 7473 5b31 5d0a 2020 2020 2020 2020  puts[1].        
-0001df80: 6469 7374 616e 6365 5f6d 656d 6265 7273  distance_members
-0001df90: 6869 705f 6920 3d20 696e 7075 7473 5b32  hip_i = inputs[2
-0001dfa0: 5d0a 2020 2020 2020 2020 6469 7374 616e  ].        distan
-0001dfb0: 6365 5f6d 656d 6265 7273 6869 705f 6a20  ce_membership_j 
-0001dfc0: 3d20 696e 7075 7473 5b33 5d0a 2020 2020  = inputs[3].    
-0001dfd0: 2020 2020 6469 7374 616e 6365 5f68 6964      distance_hid
-0001dfe0: 6465 6e20 3d20 746f 7263 682e 6d61 746d  den = torch.matm
-0001dff0: 756c 2864 6973 7461 6e63 652c 2073 656c  ul(distance, sel
-0001e000: 662e 575f 6466 2920 2b20 7365 6c66 2e62  f.W_df) + self.b
-0001e010: 5f64 660a 2020 2020 2020 2020 6174 6f6d  _df.        atom
-0001e020: 5f66 6561 7475 7265 735f 6869 6464 656e  _features_hidden
-0001e030: 203d 2074 6f72 6368 2e6d 6174 6d75 6c28   = torch.matmul(
-0001e040: 6174 6f6d 5f66 6561 7475 7265 732c 0a20  atom_features,. 
-0001e050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e070: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0001e080: 575f 6366 2920 2b20 7365 6c66 2e62 5f63  W_cf) + self.b_c
-0001e090: 660a 2020 2020 2020 2020 6f75 7470 7574  f.        output
-0001e0a0: 7320 3d20 746f 7263 682e 6d75 6c28 0a20  s = torch.mul(. 
-0001e0b0: 2020 2020 2020 2020 2020 2064 6973 7461             dista
-0001e0c0: 6e63 655f 6869 6464 656e 2c0a 2020 2020  nce_hidden,.    
-0001e0d0: 2020 2020 2020 2020 746f 7263 682e 656d          torch.em
-0001e0e0: 6265 6464 696e 6728 6174 6f6d 5f66 6561  bedding(atom_fea
-0001e0f0: 7475 7265 735f 6869 6464 656e 2c20 6469  tures_hidden, di
-0001e100: 7374 616e 6365 5f6d 656d 6265 7273 6869  stance_membershi
-0001e110: 705f 6a29 290a 0a20 2020 2020 2020 2023  p_j))..        #
-0001e120: 2066 6f72 2061 746f 6d20 6920 696e 2061   for atom i in a
-0001e130: 206d 6f6c 6563 756c 6520 6d2c 2074 6869   molecule m, thi
-0001e140: 7320 7374 6570 206d 756c 7469 706c 6965  s step multiplie
-0001e150: 7320 746f 6765 7468 6572 2064 6973 7461  s together dista
-0001e160: 6e63 6520 696e 666f 206f 6620 6174 6f6d  nce info of atom
-0001e170: 2070 6169 7228 692c 6a29 0a20 2020 2020   pair(i,j).     
-0001e180: 2020 2023 2061 6e64 2065 6d62 6564 6469     # and embeddi
-0001e190: 6e67 7320 6f66 2061 746f 6d20 6a28 626f  ngs of atom j(bo
-0001e1a0: 7468 2067 6f6e 6520 7468 726f 7567 6820  th gone through 
-0001e1b0: 6120 6869 6464 656e 206c 6179 6572 290a  a hidden layer).
-0001e1c0: 2020 2020 2020 2020 6f75 7470 7574 7320          outputs 
-0001e1d0: 3d20 746f 7263 682e 6d61 746d 756c 286f  = torch.matmul(o
-0001e1e0: 7574 7075 7473 2c20 7365 6c66 2e57 5f66  utputs, self.W_f
-0001e1f0: 6329 0a20 2020 2020 2020 206f 7574 7075  c).        outpu
-0001e200: 7473 203d 2073 656c 662e 6163 7469 7661  ts = self.activa
-0001e210: 7469 6f6e 5f66 6e28 6f75 7470 7574 7329  tion_fn(outputs)
-0001e220: 0a0a 2020 2020 2020 2020 6f75 7470 7574  ..        output
-0001e230: 5f69 6920 3d20 746f 7263 682e 6d75 6c28  _ii = torch.mul(
-0001e240: 7365 6c66 2e62 5f64 662c 2061 746f 6d5f  self.b_df, atom_
-0001e250: 6665 6174 7572 6573 5f68 6964 6465 6e29  features_hidden)
-0001e260: 0a20 2020 2020 2020 206f 7574 7075 745f  .        output_
-0001e270: 6969 203d 2074 6f72 6368 2e6d 6174 6d75  ii = torch.matmu
-0001e280: 6c28 6f75 7470 7574 5f69 692c 2073 656c  l(output_ii, sel
-0001e290: 662e 575f 6663 290a 2020 2020 2020 2020  f.W_fc).        
-0001e2a0: 6f75 7470 7574 5f69 6920 3d20 7365 6c66  output_ii = self
-0001e2b0: 2e61 6374 6976 6174 696f 6e5f 666e 286f  .activation_fn(o
-0001e2c0: 7574 7075 745f 6969 290a 0a20 2020 2020  utput_ii)..     
-0001e2d0: 2020 2023 2066 6f72 2061 746f 6d20 692c     # for atom i,
-0001e2e0: 2073 756d 2074 6865 2069 6e66 6c75 656e   sum the influen
-0001e2f0: 6365 2066 726f 6d20 616c 6c20 6f74 6865  ce from all othe
-0001e300: 7220 6174 6f6d 206a 2069 6e20 7468 6520  r atom j in the 
-0001e310: 6d6f 6c65 6375 6c65 0a20 2020 2020 2020  molecule.       
-0001e320: 2069 6e74 7261 6374 696f 6e5f 7665 6374   intraction_vect
-0001e330: 6f72 203d 2073 6361 7474 6572 286f 7574  or = scatter(out
-0001e340: 7075 7473 2c20 6469 7374 616e 6365 5f6d  puts, distance_m
-0001e350: 656d 6265 7273 6869 705f 692c 0a20 2020  embership_i,.   
-0001e360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e380: 2064 696d 3d30 2920 2d20 6f75 7470 7574   dim=0) - output
-0001e390: 5f69 6920 2b20 6174 6f6d 5f66 6561 7475  _ii + atom_featu
-0001e3a0: 7265 730a 2020 2020 2020 2020 7265 7475  res.        retu
-0001e3b0: 726e 2069 6e74 7261 6374 696f 6e5f 7665  rn intraction_ve
-0001e3c0: 6374 6f72 0a0a 0a63 6c61 7373 2045 6467  ctor...class Edg
-0001e3d0: 654e 6574 776f 726b 286e 6e2e 4d6f 6475  eNetwork(nn.Modu
-0001e3e0: 6c65 293a 0a20 2020 2022 2222 5468 6520  le):.    """The 
-0001e3f0: 4564 6765 4e65 7477 6f72 6b20 6d6f 6475  EdgeNetwork modu
-0001e400: 6c65 2069 7320 6120 5079 546f 7263 6820  le is a PyTorch 
-0001e410: 7375 626d 6f64 756c 6520 6465 7369 676e  submodule design
-0001e420: 6564 2066 6f72 206d 6573 7361 6765 2070  ed for message p
-0001e430: 6173 7369 6e67 2069 6e20 6772 6170 6820  assing in graph 
-0001e440: 6e65 7572 616c 206e 6574 776f 726b 732e  neural networks.
-0001e450: 0a0a 2020 2020 4578 616d 706c 6573 0a20  ..    Examples. 
-0001e460: 2020 202d 2d2d 2d2d 2d2d 2d0a 2020 2020     --------.    
-0001e470: 3e3e 3e20 7061 6972 5f66 6561 7475 7265  >>> pair_feature
-0001e480: 7320 3d20 746f 7263 682e 7261 6e64 2828  s = torch.rand((
-0001e490: 342c 2032 292c 2064 7479 7065 3d74 6f72  4, 2), dtype=tor
-0001e4a0: 6368 2e66 6c6f 6174 3332 290a 2020 2020  ch.float32).    
-0001e4b0: 3e3e 3e20 6174 6f6d 5f66 6561 7475 7265  >>> atom_feature
-0001e4c0: 7320 3d20 746f 7263 682e 7261 6e64 2828  s = torch.rand((
-0001e4d0: 352c 2032 292c 2064 7479 7065 3d74 6f72  5, 2), dtype=tor
-0001e4e0: 6368 2e66 6c6f 6174 3332 290a 2020 2020  ch.float32).    
-0001e4f0: 3e3e 3e20 6174 6f6d 5f74 6f5f 7061 6972  >>> atom_to_pair
-0001e500: 203d 205b 5d0a 2020 2020 3e3e 3e20 6e5f   = [].    >>> n_
-0001e510: 6174 6f6d 7320 3d20 320a 2020 2020 3e3e  atoms = 2.    >>
-0001e520: 3e20 7374 6172 7420 3d20 300a 2020 2020  > start = 0.    
-0001e530: 3e3e 3e20 4330 2c20 4331 203d 206e 702e  >>> C0, C1 = np.
-0001e540: 6d65 7368 6772 6964 286e 702e 6172 616e  meshgrid(np.aran
-0001e550: 6765 286e 5f61 746f 6d73 292c 206e 702e  ge(n_atoms), np.
-0001e560: 6172 616e 6765 286e 5f61 746f 6d73 2929  arange(n_atoms))
-0001e570: 0a20 2020 203e 3e3e 2061 746f 6d5f 746f  .    >>> atom_to
-0001e580: 5f70 6169 722e 6170 7065 6e64 286e 702e  _pair.append(np.
-0001e590: 7472 616e 7370 6f73 6528 6e70 2e61 7272  transpose(np.arr
-0001e5a0: 6179 285b 4331 2e66 6c61 7474 656e 2829  ay([C1.flatten()
-0001e5b0: 202b 2073 7461 7274 2c20 4330 2e66 6c61   + start, C0.fla
-0001e5c0: 7474 656e 2829 202b 2073 7461 7274 5d29  tten() + start])
-0001e5d0: 2929 0a20 2020 203e 3e3e 2061 746f 6d5f  )).    >>> atom_
-0001e5e0: 746f 5f70 6169 7220 3d20 746f 7263 682e  to_pair = torch.
-0001e5f0: 5465 6e73 6f72 2861 746f 6d5f 746f 5f70  Tensor(atom_to_p
-0001e600: 6169 7229 0a20 2020 203e 3e3e 2061 746f  air).    >>> ato
-0001e610: 6d5f 746f 5f70 6169 7220 3d20 746f 7263  m_to_pair = torc
-0001e620: 682e 7371 7565 657a 6528 6174 6f6d 5f74  h.squeeze(atom_t
-0001e630: 6f5f 7061 6972 2e74 6f28 746f 7263 682e  o_pair.to(torch.
-0001e640: 696e 7436 3429 2c20 6469 6d3d 3029 0a20  int64), dim=0). 
-0001e650: 2020 203e 3e3e 2069 6e70 7574 7320 3d20     >>> inputs = 
-0001e660: 5b70 6169 725f 6665 6174 7572 6573 2c20  [pair_features, 
-0001e670: 6174 6f6d 5f66 6561 7475 7265 732c 2061  atom_features, a
-0001e680: 746f 6d5f 746f 5f70 6169 725d 0a20 2020  tom_to_pair].   
-0001e690: 203e 3e3e 206e 5f70 6169 725f 6665 6174   >>> n_pair_feat
-0001e6a0: 7572 6573 203d 2032 0a20 2020 203e 3e3e  ures = 2.    >>>
-0001e6b0: 206e 5f68 6964 6465 6e20 3d20 320a 2020   n_hidden = 2.  
-0001e6c0: 2020 3e3e 3e20 696e 6974 203d 2027 7861    >>> init = 'xa
-0001e6d0: 7669 6572 5f75 6e69 666f 726d 5f27 0a20  vier_uniform_'. 
-0001e6e0: 2020 203e 3e3e 206c 6179 6572 203d 2045     >>> layer = E
-0001e6f0: 6467 654e 6574 776f 726b 286e 5f70 6169  dgeNetwork(n_pai
-0001e700: 725f 6665 6174 7572 6573 2c20 6e5f 6869  r_features, n_hi
-0001e710: 6464 656e 2c20 696e 6974 290a 2020 2020  dden, init).    
-0001e720: 3e3e 3e20 7265 7375 6c74 203d 206c 6179  >>> result = lay
-0001e730: 6572 2869 6e70 7574 7329 0a20 2020 203e  er(inputs).    >
-0001e740: 3e3e 2072 6573 756c 742e 7368 6170 655b  >> result.shape[
-0001e750: 315d 0a20 2020 2032 0a20 2020 2022 2222  1].    2.    """
-0001e760: 0a0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
-0001e770: 5f5f 2873 656c 662c 0a20 2020 2020 2020  __(self,.       
-0001e780: 2020 2020 2020 2020 2020 6e5f 7061 6972            n_pair
-0001e790: 5f66 6561 7475 7265 733a 2069 6e74 203d  _features: int =
-0001e7a0: 2038 2c0a 2020 2020 2020 2020 2020 2020   8,.            
-0001e7b0: 2020 2020 206e 5f68 6964 6465 6e3a 2069       n_hidden: i
-0001e7c0: 6e74 203d 2031 3030 2c0a 2020 2020 2020  nt = 100,.      
-0001e7d0: 2020 2020 2020 2020 2020 2069 6e69 743a             init:
-0001e7e0: 2073 7472 203d 2027 7861 7669 6572 5f75   str = 'xavier_u
-0001e7f0: 6e69 666f 726d 5f27 2c0a 2020 2020 2020  niform_',.      
-0001e800: 2020 2020 2020 2020 2020 202a 2a6b 7761             **kwa
-0001e810: 7267 7329 3a0a 2020 2020 2020 2020 2222  rgs):.        ""
-0001e820: 2249 6e69 7461 6c69 7365 7320 6120 4564  "Initalises a Ed
-0001e830: 6765 4e65 7477 6f72 6b20 4c61 7965 720a  geNetwork Layer.
-0001e840: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
-0001e850: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
-0001e860: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 206e  ------.        n
-0001e870: 5f70 6169 725f 6665 6174 7572 6573 3a20  _pair_features: 
-0001e880: 696e 742c 206f 7074 696f 6e61 6c0a 2020  int, optional.  
-0001e890: 2020 2020 2020 2020 2020 5468 6520 6c65            The le
-0001e8a0: 6e67 7468 206f 6620 7468 6520 7061 6972  ngth of the pair
-0001e8b0: 2066 6561 7475 7265 7320 7665 6374 6f72   features vector
-0001e8c0: 2e0a 2020 2020 2020 2020 6e5f 6869 6464  ..        n_hidd
-0001e8d0: 656e 3a20 696e 742c 206f 7074 696f 6e61  en: int, optiona
-0001e8e0: 6c0a 2020 2020 2020 2020 2020 2020 6e75  l.            nu
-0001e8f0: 6d62 6572 206f 6620 6869 6464 656e 2075  mber of hidden u
-0001e900: 6e69 7473 2069 6e20 7468 6520 7061 7373  nits in the pass
-0001e910: 696e 6720 7068 6173 650a 2020 2020 2020  ing phase.      
-0001e920: 2020 696e 6974 3a20 7374 722c 206f 7074    init: str, opt
-0001e930: 696f 6e61 6c0a 2020 2020 2020 2020 2020  ional.          
-0001e940: 2020 496e 6974 6961 6c69 7a61 7469 6f6e    Initialization
-0001e950: 2066 756e 6374 696f 6e20 746f 2062 6520   function to be 
-0001e960: 7573 6564 2069 6e20 7468 6520 6d65 7373  used in the mess
-0001e970: 6167 6520 7061 7373 696e 6720 6c61 7965  age passing laye
-0001e980: 722e 0a20 2020 2020 2020 2022 2222 0a0a  r..        """..
-0001e990: 2020 2020 2020 2020 7375 7065 7228 4564          super(Ed
-0001e9a0: 6765 4e65 7477 6f72 6b2c 2073 656c 6629  geNetwork, self)
-0001e9b0: 2e5f 5f69 6e69 745f 5f28 2a2a 6b77 6172  .__init__(**kwar
-0001e9c0: 6773 290a 2020 2020 2020 2020 7365 6c66  gs).        self
-0001e9d0: 2e6e 5f70 6169 725f 6665 6174 7572 6573  .n_pair_features
-0001e9e0: 3a20 696e 7420 3d20 6e5f 7061 6972 5f66  : int = n_pair_f
-0001e9f0: 6561 7475 7265 730a 2020 2020 2020 2020  eatures.        
-0001ea00: 7365 6c66 2e6e 5f68 6964 6465 6e3a 2069  self.n_hidden: i
-0001ea10: 6e74 203d 206e 5f68 6964 6465 6e0a 2020  nt = n_hidden.  
-0001ea20: 2020 2020 2020 7365 6c66 2e69 6e69 743a        self.init:
-0001ea30: 2073 7472 203d 2069 6e69 740a 0a20 2020   str = init..   
-0001ea40: 2020 2020 2069 6e69 745f 6675 6e63 3a20       init_func: 
-0001ea50: 4361 6c6c 6162 6c65 203d 2067 6574 6174  Callable = getat
-0001ea60: 7472 2869 6e69 7469 616c 697a 6572 732c  tr(initializers,
-0001ea70: 2073 656c 662e 696e 6974 290a 2020 2020   self.init).    
-0001ea80: 2020 2020 7365 6c66 2e57 3a20 746f 7263      self.W: torc
-0001ea90: 682e 5465 6e73 6f72 203d 2069 6e69 745f  h.Tensor = init_
-0001eaa0: 6675 6e63 280a 2020 2020 2020 2020 2020  func(.          
-0001eab0: 2020 746f 7263 682e 656d 7074 7928 5b73    torch.empty([s
-0001eac0: 656c 662e 6e5f 7061 6972 5f66 6561 7475  elf.n_pair_featu
-0001ead0: 7265 732c 2073 656c 662e 6e5f 6869 6464  res, self.n_hidd
-0001eae0: 656e 202a 2073 656c 662e 6e5f 6869 6464  en * self.n_hidd
-0001eaf0: 656e 5d29 290a 2020 2020 2020 2020 7365  en])).        se
-0001eb00: 6c66 2e62 3a20 746f 7263 682e 5465 6e73  lf.b: torch.Tens
-0001eb10: 6f72 203d 2074 6f72 6368 2e7a 6572 6f73  or = torch.zeros
-0001eb20: 2828 7365 6c66 2e6e 5f68 6964 6465 6e20  ((self.n_hidden 
-0001eb30: 2a20 7365 6c66 2e6e 5f68 6964 6465 6e2c  * self.n_hidden,
-0001eb40: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-0001eb50: 6275 696c 743a 2062 6f6f 6c20 3d20 5472  built: bool = Tr
-0001eb60: 7565 0a0a 2020 2020 6465 6620 5f5f 7265  ue..    def __re
-0001eb70: 7072 5f5f 2873 656c 6629 202d 3e20 7374  pr__(self) -> st
-0001eb80: 723a 0a20 2020 2020 2020 2072 6574 7572  r:.        retur
-0001eb90: 6e20 280a 2020 2020 2020 2020 2020 2020  n (.            
-0001eba0: 6627 7b73 656c 662e 5f5f 636c 6173 735f  f'{self.__class_
-0001ebb0: 5f2e 5f5f 6e61 6d65 5f5f 7d28 6e5f 7061  _.__name__}(n_pa
-0001ebc0: 6972 5f66 6561 7475 7265 733a 7b73 656c  ir_features:{sel
-0001ebd0: 662e 6e5f 7061 6972 5f66 6561 7475 7265  f.n_pair_feature
-0001ebe0: 737d 2c6e 5f68 6964 6465 6e3a 7b73 656c  s},n_hidden:{sel
-0001ebf0: 662e 6e5f 6869 6464 656e 7d2c 696e 6974  f.n_hidden},init
-0001ec00: 3a7b 7365 6c66 2e69 6e69 747d 2927 0a20  :{self.init})'. 
-0001ec10: 2020 2020 2020 2029 0a0a 2020 2020 6465         )..    de
-0001ec20: 6620 666f 7277 6172 6428 7365 6c66 2c20  f forward(self, 
-0001ec30: 696e 7075 7473 3a20 4c69 7374 5b74 6f72  inputs: List[tor
-0001ec40: 6368 2e54 656e 736f 725d 2920 2d3e 2074  ch.Tensor]) -> t
-0001ec50: 6f72 6368 2e54 656e 736f 723a 0a20 2020  orch.Tensor:.   
-0001ec60: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0001ec70: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
-0001ec80: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-0001ec90: 2020 2020 2020 2069 6e70 7574 733a 204c         inputs: L
-0001eca0: 6973 745b 746f 7263 682e 5465 6e73 6f72  ist[torch.Tensor
-0001ecb0: 5d0a 2020 2020 2020 2020 2020 2020 5468  ].            Th
-0001ecc0: 6520 6c65 6e67 7468 206f 6620 6174 6f6d  e length of atom
-0001ecd0: 5f74 6f5f 7061 6972 2073 686f 756c 6420  _to_pair should 
-0001ece0: 6265 2073 616d 6520 6173 206e 5f70 6169  be same as n_pai
-0001ecf0: 725f 6665 6174 7572 6573 2e0a 2020 2020  r_features..    
-0001ed00: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
-0001ed10: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
-0001ed20: 2020 2020 7265 7375 6c74 3a20 746f 7263      result: torc
-0001ed30: 682e 5465 6e73 6f72 0a20 2020 2020 2020  h.Tensor.       
-0001ed40: 2020 2020 2054 656e 736f 7220 636f 6e74       Tensor cont
-0001ed50: 6169 6e69 6e67 2074 6865 206d 6170 7069  aining the mappi
-0001ed60: 6e67 206f 6620 7468 6520 6564 6765 2076  ng of the edge v
-0001ed70: 6563 746f 7220 746f 2061 2064 20c3 9720  ector to a d .. 
-0001ed80: 6420 6d61 7472 6978 2c20 7768 6572 6520  d matrix, where 
-0001ed90: 6420 6465 6e6f 7465 7320 7468 6520 6469  d denotes the di
-0001eda0: 6d65 6e73 696f 6e20 6f66 2074 6865 2069  mension of the i
-0001edb0: 6e74 6572 6e61 6c20 6869 6464 656e 2072  nternal hidden r
-0001edc0: 6570 7265 7365 6e74 6174 696f 6e20 6f66  epresentation of
-0001edd0: 2065 6163 6820 6e6f 6465 2069 6e20 7468   each node in th
-0001ede0: 6520 6772 6170 682e 0a20 2020 2020 2020  e graph..       
-0001edf0: 2022 2222 0a20 2020 2020 2020 2070 6169   """.        pai
-0001ee00: 725f 6665 6174 7572 6573 3a20 746f 7263  r_features: torc
-0001ee10: 682e 5465 6e73 6f72 0a20 2020 2020 2020  h.Tensor.       
-0001ee20: 2061 746f 6d5f 6665 6174 7572 6573 3a20   atom_features: 
-0001ee30: 746f 7263 682e 5465 6e73 6f72 0a20 2020  torch.Tensor.   
-0001ee40: 2020 2020 2061 746f 6d5f 746f 5f70 6169       atom_to_pai
-0001ee50: 723a 2074 6f72 6368 2e54 656e 736f 720a  r: torch.Tensor.
-0001ee60: 2020 2020 2020 2020 7061 6972 5f66 6561          pair_fea
-0001ee70: 7475 7265 732c 2061 746f 6d5f 6665 6174  tures, atom_feat
-0001ee80: 7572 6573 2c20 6174 6f6d 5f74 6f5f 7061  ures, atom_to_pa
-0001ee90: 6972 203d 2069 6e70 7574 730a 0a20 2020  ir = inputs..   
-0001eea0: 2020 2020 2041 3a20 746f 7263 682e 5465       A: torch.Te
-0001eeb0: 6e73 6f72 203d 2074 6f72 6368 2e61 6464  nsor = torch.add
-0001eec0: 2874 6f72 6368 2e6d 6174 6d75 6c28 7061  (torch.matmul(pa
-0001eed0: 6972 5f66 6561 7475 7265 732c 2073 656c  ir_features, sel
-0001eee0: 662e 5729 2c20 7365 6c66 2e62 290a 2020  f.W), self.b).  
-0001eef0: 2020 2020 2020 4120 3d20 746f 7263 682e        A = torch.
-0001ef00: 7265 7368 6170 6528 412c 2028 2d31 2c20  reshape(A, (-1, 
-0001ef10: 7365 6c66 2e6e 5f68 6964 6465 6e2c 2073  self.n_hidden, s
-0001ef20: 656c 662e 6e5f 6869 6464 656e 2929 0a20  elf.n_hidden)). 
-0001ef30: 2020 2020 2020 206f 7574 3a20 746f 7263         out: torc
-0001ef40: 682e 5465 6e73 6f72 203d 2074 6f72 6368  h.Tensor = torch
-0001ef50: 2e75 6e73 7175 6565 7a65 2861 746f 6d5f  .unsqueeze(atom_
-0001ef60: 6665 6174 7572 6573 5b61 746f 6d5f 746f  features[atom_to
-0001ef70: 5f70 6169 725b 3a2c 2031 5d5d 2c0a 2020  _pair[:, 1]],.  
-0001ef80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ef90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001efa0: 2020 2020 2020 2020 2020 6469 6d3d 3229            dim=2)
-0001efb0: 0a20 2020 2020 2020 206f 7574 5f73 7175  .        out_squ
-0001efc0: 6565 7a65 3a20 746f 7263 682e 5465 6e73  eeze: torch.Tens
-0001efd0: 6f72 203d 2074 6f72 6368 2e73 7175 6565  or = torch.squee
-0001efe0: 7a65 2874 6f72 6368 2e6d 6174 6d75 6c28  ze(torch.matmul(
-0001eff0: 412c 206f 7574 292c 2064 696d 3d32 290a  A, out), dim=2).
-0001f000: 2020 2020 2020 2020 696e 643a 2074 6f72          ind: tor
-0001f010: 6368 2e54 656e 736f 7220 3d20 6174 6f6d  ch.Tensor = atom
-0001f020: 5f74 6f5f 7061 6972 5b3a 2c20 305d 0a0a  _to_pair[:, 0]..
-0001f030: 2020 2020 2020 2020 7265 7375 6c74 3a20          result: 
-0001f040: 746f 7263 682e 5465 6e73 6f72 203d 2073  torch.Tensor = s
-0001f050: 6567 6d65 6e74 5f73 756d 286f 7574 5f73  egment_sum(out_s
-0001f060: 7175 6565 7a65 2c20 696e 6429 0a0a 2020  queeze, ind)..  
-0001f070: 2020 2020 2020 7265 7475 726e 2072 6573        return res
-0001f080: 756c 740a 0a0a 636c 6173 7320 5765 6176  ult...class Weav
-0001f090: 654c 6179 6572 286e 6e2e 4d6f 6475 6c65  eLayer(nn.Module
-0001f0a0: 293a 0a20 2020 2022 2222 5468 6973 2063  ):.    """This c
-0001f0b0: 6c61 7373 2069 6d70 6c65 6d65 6e74 7320  lass implements 
-0001f0c0: 7468 6520 636f 7265 2057 6561 7665 2063  the core Weave c
-0001f0d0: 6f6e 766f 6c75 7469 6f6e 2066 726f 6d20  onvolution from 
-0001f0e0: 7468 6520 476f 6f67 6c65 2067 7261 7068  the Google graph
-0001f0f0: 2063 6f6e 766f 6c75 7469 6f6e 2070 6170   convolution pap
-0001f100: 6572 205b 315d 5f0a 2020 5468 6973 2069  er [1]_.  This i
-0001f110: 7320 7468 6520 546f 7263 6820 6571 7569  s the Torch equi
-0001f120: 7661 6c65 6e74 206f 6620 7468 6520 6f72  valent of the or
-0001f130: 6967 696e 616c 2069 6d70 6c65 6d65 6e74  iginal implement
-0001f140: 6174 696f 6e20 7573 696e 6720 4b65 7261  ation using Kera
-0001f150: 732e 0a0a 2020 5468 6973 206d 6f64 656c  s...  This model
-0001f160: 2063 6f6e 7461 696e 7320 6174 6f6d 2066   contains atom f
-0001f170: 6561 7475 7265 7320 616e 6420 626f 6e64  eatures and bond
-0001f180: 2066 6561 7475 7265 730a 2020 7365 7061   features.  sepa
-0001f190: 7261 7465 6c79 2e48 6572 652c 2062 6f6e  rately.Here, bon
-0001f1a0: 6420 6665 6174 7572 6573 2061 7265 2061  d features are a
-0001f1b0: 6c73 6f20 6361 6c6c 6564 2070 6169 7220  lso called pair 
-0001f1c0: 6665 6174 7572 6573 2e0a 2020 5468 6572  features..  Ther
-0001f1d0: 6520 6172 6520 3220 7479 7065 7320 6f66  e are 2 types of
-0001f1e0: 2074 7261 6e73 666f 726d 6174 696f 6e2c   transformation,
-0001f1f0: 2061 746f 6d2d 3e61 746f 6d2c 2061 746f   atom->atom, ato
-0001f200: 6d2d 3e70 6169 722c 2070 6169 722d 3e61  m->pair, pair->a
-0001f210: 746f 6d2c 2070 6169 722d 3e70 6169 7220  tom, pair->pair 
-0001f220: 7468 6174 2074 6869 7320 6d6f 6465 6c20  that this model 
-0001f230: 696d 706c 656d 656e 7473 2e0a 0a20 2045  implements...  E
-0001f240: 7861 6d70 6c65 730a 2020 2d2d 2d2d 2d2d  xamples.  ------
-0001f250: 2d2d 0a20 2054 6869 7320 6c61 7965 7220  --.  This layer 
-0001f260: 6578 7065 6374 7320 3420 696e 7075 7473  expects 4 inputs
-0001f270: 2069 6e20 6120 6c69 7374 206f 6620 7468   in a list of th
-0001f280: 6520 666f 726d 2060 5b61 746f 6d5f 6665  e form `[atom_fe
-0001f290: 6174 7572 6573 2c0a 2020 7061 6972 5f66  atures,.  pair_f
-0001f2a0: 6561 7475 7265 732c 2070 6169 725f 7370  eatures, pair_sp
-0001f2b0: 6c69 742c 2061 746f 6d5f 746f 5f70 6169  lit, atom_to_pai
-0001f2c0: 725d 602e 2057 6527 6c6c 2077 616c 6b20  r]`. We'll walk 
-0001f2d0: 7468 726f 7567 6820 7468 6520 7374 7275  through the stru
-0001f2e0: 6374 7572 6520 6f66 2074 6865 7365 2069  cture of these i
-0001f2f0: 6e70 7574 732e 204c 6574 2773 2073 7461  nputs. Let's sta
-0001f300: 7274 2077 6974 6820 736f 6d65 2062 6173  rt with some bas
-0001f310: 6963 2064 6566 696e 6974 696f 6e73 2e0a  ic definitions..
-0001f320: 2020 3e3e 3e20 696d 706f 7274 2064 6565    >>> import dee
-0001f330: 7063 6865 6d20 6173 2064 630a 2020 3e3e  pchem as dc.  >>
-0001f340: 3e20 696d 706f 7274 206e 756d 7079 2061  > import numpy a
-0001f350: 7320 6e70 0a20 203e 3e3e 2073 6d69 6c65  s np.  >>> smile
-0001f360: 7320 3d20 5b22 4343 4322 2c20 2243 225d  s = ["CCC", "C"]
-0001f370: 0a0a 2020 4e6f 7465 2074 6861 7420 7468  ..  Note that th
-0001f380: 6572 6520 6172 6520 3420 6174 6f6d 7320  ere are 4 atoms 
-0001f390: 696e 2074 6f74 616c 2069 6e20 7468 6973  in total in this
-0001f3a0: 2073 7973 7465 6d2e 2054 6869 7320 6c61   system. This la
-0001f3b0: 7965 7220 6578 7065 6374 7320 6974 7320  yer expects its 
-0001f3c0: 696e 7075 7420 6d6f 6c65 6375 6c65 7320  input molecules 
-0001f3d0: 746f 2062 6520 6261 7463 6865 6420 746f  to be batched to
-0001f3e0: 6765 7468 6572 2e0a 0a20 203e 3e3e 2074  gether...  >>> t
-0001f3f0: 6f74 616c 5f6e 5f61 746f 6d73 203d 2034  otal_n_atoms = 4
-0001f400: 0a0a 2020 4c65 7427 7320 7375 7070 6f73  ..  Let's suppos
-0001f410: 6520 7468 6174 2077 6520 6861 7665 2061  e that we have a
-0001f420: 2066 6561 7475 7269 7a65 7220 7468 6174   featurizer that
-0001f430: 2063 6f6d 7075 7465 7320 606e 5f61 746f   computes `n_ato
-0001f440: 6d5f 6665 6174 6020 6665 6174 7572 6573  m_feat` features
-0001f450: 2070 6572 2061 746f 6d2e 0a0a 2020 3e3e   per atom...  >>
-0001f460: 3e20 6e5f 6174 6f6d 5f66 6561 7420 3d20  > n_atom_feat = 
-0001f470: 3735 0a0a 2020 5468 656e 2063 6f6e 6365  75..  Then conce
-0001f480: 7074 7561 6c6c 792c 2060 6174 6f6d 5f66  ptually, `atom_f
-0001f490: 6561 7460 2069 7320 7468 6520 6172 7261  eat` is the arra
-0001f4a0: 7920 6f66 2073 6861 7065 2060 2874 6f74  y of shape `(tot
-0001f4b0: 616c 5f6e 5f61 746f 6d73 2c0a 2020 6e5f  al_n_atoms,.  n_
-0001f4c0: 6174 6f6d 5f66 6561 7429 6020 6f66 2061  atom_feat)` of a
-0001f4d0: 746f 6d69 6320 6665 6174 7572 6573 2e20  tomic features. 
-0001f4e0: 466f 7220 7369 6d70 6c69 6369 7479 2c20  For simplicity, 
-0001f4f0: 6c65 7427 7320 6a75 7374 2067 6f20 7769  let's just go wi
-0001f500: 7468 2061 0a20 2072 616e 646f 6d20 7375  th a.  random su
-0001f510: 6368 206d 6174 7269 782e 0a0a 2020 3e3e  ch matrix...  >>
-0001f520: 3e20 6174 6f6d 5f66 6561 7420 3d20 6e70  > atom_feat = np
-0001f530: 2e72 616e 646f 6d2e 7261 6e64 2874 6f74  .random.rand(tot
-0001f540: 616c 5f6e 5f61 746f 6d73 2c20 6e5f 6174  al_n_atoms, n_at
-0001f550: 6f6d 5f66 6561 7429 0a0a 2020 4c65 7427  om_feat)..  Let'
-0001f560: 7320 7375 7070 6f73 6520 7765 2068 6176  s suppose we hav
-0001f570: 6520 606e 5f70 6169 725f 6665 6174 6020  e `n_pair_feat` 
-0001f580: 7061 6972 7769 7365 2066 6561 7475 7265  pairwise feature
-0001f590: 730a 0a20 203e 3e3e 206e 5f70 6169 725f  s..  >>> n_pair_
-0001f5a0: 6665 6174 203d 2031 340a 0a20 2046 6f72  feat = 14..  For
-0001f5b0: 2065 6163 6820 6d6f 6c65 6375 6c65 2c20   each molecule, 
-0001f5c0: 7765 2063 6f6d 7075 7465 2061 206d 6174  we compute a mat
-0001f5d0: 7269 7820 6f66 2073 6861 7065 2060 286e  rix of shape `(n
-0001f5e0: 5f61 746f 6d73 2a6e 5f61 746f 6d73 2c0a  _atoms*n_atoms,.
-0001f5f0: 2020 6e5f 7061 6972 5f66 6561 7429 6020    n_pair_feat)` 
-0001f600: 6f66 2070 6169 7277 6973 6520 6665 6174  of pairwise feat
-0001f610: 7572 6573 2066 6f72 2065 6163 6820 7061  ures for each pa
-0001f620: 6972 206f 6620 6174 6f6d 7320 696e 2074  ir of atoms in t
-0001f630: 6865 206d 6f6c 6563 756c 652e 0a20 204c  he molecule..  L
-0001f640: 6574 2773 2063 6f6e 7374 7275 6374 2074  et's construct t
-0001f650: 6869 7320 636f 6e63 6570 7475 616c 6c79  his conceptually
-0001f660: 2066 6f72 206f 7572 2065 7861 6d70 6c65   for our example
-0001f670: 2e0a 0a20 203e 3e3e 2070 6169 725f 6665  ...  >>> pair_fe
-0001f680: 6174 203d 205b 6e70 2e72 616e 646f 6d2e  at = [np.random.
-0001f690: 7261 6e64 2833 2a33 2c20 6e5f 7061 6972  rand(3*3, n_pair
-0001f6a0: 5f66 6561 7429 2c20 6e70 2e72 616e 646f  _feat), np.rando
-0001f6b0: 6d2e 7261 6e64 2831 2a31 2c6e 5f70 6169  m.rand(1*1,n_pai
-0001f6c0: 725f 6665 6174 295d 0a20 203e 3e3e 2070  r_feat)].  >>> p
-0001f6d0: 6169 725f 6665 6174 203d 206e 702e 636f  air_feat = np.co
-0001f6e0: 6e63 6174 656e 6174 6528 7061 6972 5f66  ncatenate(pair_f
-0001f6f0: 6561 742c 2061 7869 733d 3029 0a20 203e  eat, axis=0).  >
-0001f700: 3e3e 2070 6169 725f 6665 6174 2e73 6861  >> pair_feat.sha
-0001f710: 7065 0a20 2028 3130 2c20 3134 290a 0a20  pe.  (10, 14).. 
-0001f720: 2060 7061 6972 5f73 706c 6974 6020 6973   `pair_split` is
-0001f730: 2061 6e20 696e 6465 7820 696e 746f 2060   an index into `
-0001f740: 7061 6972 5f66 6561 7460 2077 6869 6368  pair_feat` which
-0001f750: 2074 656c 6c73 2075 7320 7768 6963 6820   tells us which 
-0001f760: 6174 6f6d 2065 6163 6820 726f 7720 6265  atom each row be
-0001f770: 6c6f 6e67 7320 746f 2e20 496e 206f 7572  longs to. In our
-0001f780: 2063 6173 652c 2077 6520 6876 650a 0a20   case, we hve.. 
-0001f790: 203e 3e3e 2070 6169 725f 7370 6c69 7420   >>> pair_split 
-0001f7a0: 3d20 6e70 2e61 7272 6179 285b 302c 2030  = np.array([0, 0
-0001f7b0: 2c20 302c 2031 2c20 312c 2031 2c20 322c  , 0, 1, 1, 1, 2,
-0001f7c0: 2032 2c20 322c 2033 5d29 0a0a 2020 5468   2, 2, 3])..  Th
-0001f7d0: 6174 2069 732c 2074 6865 2066 6972 7374  at is, the first
-0001f7e0: 2039 2065 6e74 7269 6573 2062 656c 6f6e   9 entries belon
-0001f7f0: 6720 746f 2022 4343 4322 2061 6e64 2074  g to "CCC" and t
-0001f800: 6865 206c 6173 7420 656e 7472 7920 746f  he last entry to
-0001f810: 2022 4322 2e20 5468 650a 2020 6669 6e61   "C". The.  fina
-0001f820: 6c20 656e 7472 7920 6061 746f 6d5f 746f  l entry `atom_to
-0001f830: 5f70 6169 7260 2067 6f65 7320 696e 2061  _pair` goes in a
-0001f840: 206c 6974 746c 6520 6d6f 7265 2069 6e2d   little more in-
-0001f850: 6465 7074 6820 7468 616e 2060 7061 6972  depth than `pair
-0001f860: 5f73 706c 6974 600a 2020 616e 6420 7465  _split`.  and te
-0001f870: 6c6c 7320 7573 2074 6865 2070 7265 6369  lls us the preci
-0001f880: 7365 2070 6169 7220 6561 6368 2070 6169  se pair each pai
-0001f890: 7220 6665 6174 7572 6520 6265 6c6f 6e67  r feature belong
-0001f8a0: 7320 746f 2e20 496e 206f 7572 2063 6173  s to. In our cas
-0001f8b0: 650a 0a20 203e 3e3e 2061 746f 6d5f 746f  e..  >>> atom_to
-0001f8c0: 5f70 6169 7220 3d20 6e70 2e61 7272 6179  _pair = np.array
-0001f8d0: 285b 5b30 2c20 305d 2c0a 2020 2e2e 2e20  ([[0, 0],.  ... 
-0001f8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f8f0: 2020 2020 2020 2020 205b 302c 2031 5d2c           [0, 1],
-0001f900: 0a20 202e 2e2e 2020 2020 2020 2020 2020  .  ...          
-0001f910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f920: 5b30 2c20 325d 2c0a 2020 2e2e 2e20 2020  [0, 2],.  ...   
-0001f930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f940: 2020 2020 2020 205b 312c 2030 5d2c 0a20         [1, 0],. 
-0001f950: 202e 2e2e 2020 2020 2020 2020 2020 2020   ...            
-0001f960: 2020 2020 2020 2020 2020 2020 2020 5b31                [1
-0001f970: 2c20 315d 2c0a 2020 2e2e 2e20 2020 2020  , 1],.  ...     
-0001f980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f990: 2020 2020 205b 312c 2032 5d2c 0a20 202e       [1, 2],.  .
-0001f9a0: 2e2e 2020 2020 2020 2020 2020 2020 2020  ..              
-0001f9b0: 2020 2020 2020 2020 2020 2020 5b32 2c20              [2, 
-0001f9c0: 305d 2c0a 2020 2e2e 2e20 2020 2020 2020  0],.  ...       
-0001f9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f9e0: 2020 205b 322c 2031 5d2c 0a20 202e 2e2e     [2, 1],.  ...
-0001f9f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fa00: 2020 2020 2020 2020 2020 5b32 2c20 325d            [2, 2]
-0001fa10: 2c0a 2020 2e2e 2e20 2020 2020 2020 2020  ,.  ...         
-0001fa20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001fa30: 205b 332c 2033 5d5d 290a 0a20 204c 6574   [3, 3]])..  Let
-0001fa40: 2773 206e 6f77 2064 6566 696e 6520 7468  's now define th
-0001fa50: 6520 6163 7475 616c 206c 6179 6572 0a0a  e actual layer..
-0001fa60: 2020 3e3e 3e20 6c61 7965 7220 3d20 5765    >>> layer = We
-0001fa70: 6176 654c 6179 6572 2829 0a0a 2020 416e  aveLayer()..  An
-0001fa80: 6420 696e 766f 6b65 2069 740a 0a20 203e  d invoke it..  >
-0001fa90: 3e3e 205b 412c 2050 5d20 3d20 6c61 7965  >> [A, P] = laye
-0001faa0: 7228 5b61 746f 6d5f 6665 6174 2c20 7061  r([atom_feat, pa
-0001fab0: 6972 5f66 6561 742c 2070 6169 725f 7370  ir_feat, pair_sp
-0001fac0: 6c69 742c 2061 746f 6d5f 746f 5f70 6169  lit, atom_to_pai
-0001fad0: 725d 290a 0a20 2054 6865 2077 6561 7665  r])..  The weave
-0001fae0: 206c 6179 6572 2070 726f 6475 6365 7320   layer produces 
-0001faf0: 6e65 7720 6174 6f6d 2f70 6169 7220 6665  new atom/pair fe
-0001fb00: 6174 7572 6573 2e20 4c65 7427 7320 6368  atures. Let's ch
-0001fb10: 6563 6b20 7468 6569 7220 7368 6170 6573  eck their shapes
-0001fb20: 0a0a 2020 3e3e 3e20 4120 3d20 412e 6465  ..  >>> A = A.de
-0001fb30: 7461 6368 2829 2e6e 756d 7079 2829 0a20  tach().numpy(). 
-0001fb40: 203e 3e3e 2041 2e73 6861 7065 0a20 2028   >>> A.shape.  (
-0001fb50: 342c 2035 3029 0a20 203e 3e3e 2050 203d  4, 50).  >>> P =
-0001fb60: 2050 2e64 6574 6163 6828 292e 6e75 6d70   P.detach().nump
-0001fb70: 7928 290a 2020 3e3e 3e20 502e 7368 6170  y().  >>> P.shap
-0001fb80: 650a 2020 2831 302c 2035 3029 0a0a 2020  e.  (10, 50)..  
-0001fb90: 5468 6520 3420 6973 2060 746f 7461 6c5f  The 4 is `total_
-0001fba0: 6e75 6d5f 6174 6f6d 7360 2061 6e64 2074  num_atoms` and t
-0001fbb0: 6865 2031 3020 6973 2074 6865 2074 6f74  he 10 is the tot
-0001fbc0: 616c 206e 756d 6265 7220 6f66 2070 6169  al number of pai
-0001fbd0: 7273 2e20 5768 6572 650a 2020 646f 6573  rs. Where.  does
-0001fbe0: 2060 3530 6020 636f 6d65 2066 726f 6d3f   `50` come from?
-0001fbf0: 2049 7427 7320 6672 6f6d 2074 6865 2064   It's from the d
-0001fc00: 6566 6175 6c74 2061 7267 756d 656e 7473  efault arguments
-0001fc10: 2060 6e5f 6174 6f6d 5f69 6e70 7574 5f66   `n_atom_input_f
-0001fc20: 6561 7460 2061 6e64 0a20 2060 6e5f 7061  eat` and.  `n_pa
-0001fc30: 6972 5f69 6e70 7574 5f66 6561 7460 2e0a  ir_input_feat`..
-0001fc40: 0a20 2052 6566 6572 656e 6365 730a 2020  .  References.  
-0001fc50: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 202e 2e20  ----------.  .. 
-0001fc60: 5b31 5d20 4b65 6172 6e65 732c 2053 7465  [1] Kearnes, Ste
-0001fc70: 7665 6e2c 2065 7420 616c 2e20 224d 6f6c  ven, et al. "Mol
-0001fc80: 6563 756c 6172 2067 7261 7068 2063 6f6e  ecular graph con
-0001fc90: 766f 6c75 7469 6f6e 733a 206d 6f76 696e  volutions: movin
-0001fca0: 6720 6265 796f 6e64 0a20 2020 2020 2020  g beyond.       
-0001fcb0: 2066 696e 6765 7270 7269 6e74 732e 2220   fingerprints." 
-0001fcc0: 4a6f 7572 6e61 6c20 6f66 2063 6f6d 7075  Journal of compu
-0001fcd0: 7465 722d 6169 6465 6420 6d6f 6c65 6375  ter-aided molecu
-0001fce0: 6c61 7220 6465 7369 676e 2033 302e 3820  lar design 30.8 
-0001fcf0: 2832 3031 3629 3a0a 2020 2020 2020 2020  (2016):.        
-0001fd00: 3539 352d 3630 382e 0a20 2022 2222 0a0a  595-608..  """..
-0001fd10: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
-0001fd20: 2873 656c 662c 0a20 2020 2020 2020 2020  (self,.         
-0001fd30: 2020 2020 2020 2020 6e5f 6174 6f6d 5f69          n_atom_i
-0001fd40: 6e70 7574 5f66 6561 743a 2069 6e74 203d  nput_feat: int =
-0001fd50: 2037 352c 0a20 2020 2020 2020 2020 2020   75,.           
-0001fd60: 2020 2020 2020 6e5f 7061 6972 5f69 6e70        n_pair_inp
-0001fd70: 7574 5f66 6561 743a 2069 6e74 203d 2031  ut_feat: int = 1
-0001fd80: 342c 0a20 2020 2020 2020 2020 2020 2020  4,.             
-0001fd90: 2020 2020 6e5f 6174 6f6d 5f6f 7574 7075      n_atom_outpu
-0001fda0: 745f 6665 6174 3a20 696e 7420 3d20 3530  t_feat: int = 50
-0001fdb0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0001fdc0: 2020 206e 5f70 6169 725f 6f75 7470 7574     n_pair_output
-0001fdd0: 5f66 6561 743a 2069 6e74 203d 2035 302c  _feat: int = 50,
-0001fde0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001fdf0: 2020 6e5f 6869 6464 656e 5f41 413a 2069    n_hidden_AA: i
-0001fe00: 6e74 203d 2035 302c 0a20 2020 2020 2020  nt = 50,.       
-0001fe10: 2020 2020 2020 2020 2020 6e5f 6869 6464            n_hidd
-0001fe20: 656e 5f50 413a 2069 6e74 203d 2035 302c  en_PA: int = 50,
-0001fe30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001fe40: 2020 6e5f 6869 6464 656e 5f41 503a 2069    n_hidden_AP: i
-0001fe50: 6e74 203d 2035 302c 0a20 2020 2020 2020  nt = 50,.       
-0001fe60: 2020 2020 2020 2020 2020 6e5f 6869 6464            n_hidd
-0001fe70: 656e 5f50 503a 2069 6e74 203d 2035 302c  en_PP: int = 50,
-0001fe80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001fe90: 2020 7570 6461 7465 5f70 6169 723a 2062    update_pair: b
-0001fea0: 6f6f 6c20 3d20 5472 7565 2c0a 2020 2020  ool = True,.    
-0001feb0: 2020 2020 2020 2020 2020 2020 2069 6e69               ini
-0001fec0: 745f 3a20 7374 7220 3d20 2778 6176 6965  t_: str = 'xavie
-0001fed0: 725f 756e 6966 6f72 6d5f 272c 0a20 2020  r_uniform_',.   
-0001fee0: 2020 2020 2020 2020 2020 2020 2020 6163                ac
-0001fef0: 7469 7661 7469 6f6e 3a20 7374 7220 3d20  tivation: str = 
-0001ff00: 2772 656c 7527 2c0a 2020 2020 2020 2020  'relu',.        
-0001ff10: 2020 2020 2020 2020 2062 6174 6368 5f6e           batch_n
-0001ff20: 6f72 6d61 6c69 7a65 3a20 626f 6f6c 203d  ormalize: bool =
-0001ff30: 2054 7275 652c 0a20 2020 2020 2020 2020   True,.         
-0001ff40: 2020 2020 2020 2020 2a2a 6b77 6172 6773          **kwargs
-0001ff50: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-0001ff60: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
-0001ff70: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-0001ff80: 206e 5f61 746f 6d5f 696e 7075 745f 6665   n_atom_input_fe
-0001ff90: 6174 3a20 696e 742c 206f 7074 696f 6e61  at: int, optiona
-0001ffa0: 6c20 2864 6566 6175 6c74 2037 3529 0a20  l (default 75). 
-0001ffb0: 2020 2020 204e 756d 6265 7220 6f66 2066       Number of f
-0001ffc0: 6561 7475 7265 7320 666f 7220 6561 6368  eatures for each
-0001ffd0: 2061 746f 6d20 696e 2069 6e70 7574 2e0a   atom in input..
-0001ffe0: 2020 2020 6e5f 7061 6972 5f69 6e70 7574      n_pair_input
-0001fff0: 5f66 6561 743a 2069 6e74 2c20 6f70 7469  _feat: int, opti
-00020000: 6f6e 616c 2028 6465 6661 756c 7420 3134  onal (default 14
-00020010: 290a 2020 2020 2020 4e75 6d62 6572 206f  ).      Number o
-00020020: 6620 6665 6174 7572 6573 2066 6f72 2065  f features for e
-00020030: 6163 6820 7061 6972 206f 6620 6174 6f6d  ach pair of atom
-00020040: 7320 696e 2069 6e70 7574 2e0a 2020 2020  s in input..    
-00020050: 6e5f 6174 6f6d 5f6f 7574 7075 745f 6665  n_atom_output_fe
-00020060: 6174 3a20 696e 742c 206f 7074 696f 6e61  at: int, optiona
-00020070: 6c20 2864 6566 6175 6c74 2035 3029 0a20  l (default 50). 
-00020080: 2020 2020 204e 756d 6265 7220 6f66 2066       Number of f
-00020090: 6561 7475 7265 7320 666f 7220 6561 6368  eatures for each
-000200a0: 2061 746f 6d20 696e 206f 7574 7075 742e   atom in output.
-000200b0: 0a20 2020 206e 5f70 6169 725f 6f75 7470  .    n_pair_outp
-000200c0: 7574 5f66 6561 743a 2069 6e74 2c20 6f70  ut_feat: int, op
-000200d0: 7469 6f6e 616c 2028 6465 6661 756c 7420  tional (default 
-000200e0: 3530 290a 2020 2020 2020 4e75 6d62 6572  50).      Number
-000200f0: 206f 6620 6665 6174 7572 6573 2066 6f72   of features for
-00020100: 2065 6163 6820 7061 6972 206f 6620 6174   each pair of at
-00020110: 6f6d 7320 696e 206f 7574 7075 742e 0a20  oms in output.. 
-00020120: 2020 206e 5f68 6964 6465 6e5f 4141 3a20     n_hidden_AA: 
-00020130: 696e 742c 206f 7074 696f 6e61 6c20 2864  int, optional (d
-00020140: 6566 6175 6c74 2035 3029 0a20 2020 2020  efault 50).     
-00020150: 204e 756d 6265 7220 6f66 2075 6e69 7473   Number of units
-00020160: 2863 6f6e 766f 6c75 7469 6f6e 2064 6570  (convolution dep
-00020170: 7468 7329 2069 6e20 636f 7272 6573 706f  ths) in correspo
-00020180: 6e64 696e 6720 6869 6464 656e 206c 6179  nding hidden lay
-00020190: 6572 0a20 2020 206e 5f68 6964 6465 6e5f  er.    n_hidden_
-000201a0: 5041 3a20 696e 742c 206f 7074 696f 6e61  PA: int, optiona
-000201b0: 6c20 2864 6566 6175 6c74 2035 3029 0a20  l (default 50). 
-000201c0: 2020 2020 204e 756d 6265 7220 6f66 2075       Number of u
-000201d0: 6e69 7473 2863 6f6e 766f 6c75 7469 6f6e  nits(convolution
-000201e0: 2064 6570 7468 7329 2069 6e20 636f 7272   depths) in corr
-000201f0: 6573 706f 6e64 696e 6720 6869 6464 656e  esponding hidden
-00020200: 206c 6179 6572 0a20 2020 206e 5f68 6964   layer.    n_hid
-00020210: 6465 6e5f 4150 3a20 696e 742c 206f 7074  den_AP: int, opt
-00020220: 696f 6e61 6c20 2864 6566 6175 6c74 2035  ional (default 5
-00020230: 3029 0a20 2020 2020 204e 756d 6265 7220  0).      Number 
-00020240: 6f66 2075 6e69 7473 2863 6f6e 766f 6c75  of units(convolu
-00020250: 7469 6f6e 2064 6570 7468 7329 2069 6e20  tion depths) in 
-00020260: 636f 7272 6573 706f 6e64 696e 6720 6869  corresponding hi
-00020270: 6464 656e 206c 6179 6572 0a20 2020 206e  dden layer.    n
-00020280: 5f68 6964 6465 6e5f 5050 3a20 696e 742c  _hidden_PP: int,
-00020290: 206f 7074 696f 6e61 6c20 2864 6566 6175   optional (defau
-000202a0: 6c74 2035 3029 0a20 2020 2020 204e 756d  lt 50).      Num
-000202b0: 6265 7220 6f66 2075 6e69 7473 2863 6f6e  ber of units(con
-000202c0: 766f 6c75 7469 6f6e 2064 6570 7468 7329  volution depths)
-000202d0: 2069 6e20 636f 7272 6573 706f 6e64 696e   in correspondin
-000202e0: 6720 6869 6464 656e 206c 6179 6572 0a20  g hidden layer. 
-000202f0: 2020 2075 7064 6174 655f 7061 6972 3a20     update_pair: 
-00020300: 626f 6f6c 2c20 6f70 7469 6f6e 616c 2028  bool, optional (
-00020310: 6465 6661 756c 7420 5472 7565 290a 2020  default True).  
-00020320: 2020 2020 5768 6574 6865 7220 746f 2063      Whether to c
-00020330: 616c 6375 6c61 7465 2066 6f72 2070 6169  alculate for pai
-00020340: 7220 6665 6174 7572 6573 2c0a 2020 2020  r features,.    
-00020350: 2020 636f 756c 6420 6265 2074 7572 6e65    could be turne
-00020360: 6420 6f66 6620 666f 7220 6c61 7374 206c  d off for last l
-00020370: 6179 6572 0a20 2020 2069 6e69 743a 2073  ayer.    init: s
-00020380: 7472 2c20 6f70 7469 6f6e 616c 2028 6465  tr, optional (de
-00020390: 6661 756c 7420 2778 6176 6965 725f 756e  fault 'xavier_un
-000203a0: 6966 6f72 6d5f 2729 0a20 2020 2020 2057  iform_').      W
-000203b0: 6569 6768 7420 696e 6974 6961 6c69 7a61  eight initializa
-000203c0: 7469 6f6e 2066 6f72 2066 696c 7465 7273  tion for filters
-000203d0: 2e0a 2020 2020 6163 7469 7661 7469 6f6e  ..    activation
-000203e0: 3a20 7374 722c 206f 7074 696f 6e61 6c20  : str, optional 
-000203f0: 2864 6566 6175 6c74 2027 7265 6c75 2729  (default 'relu')
-00020400: 0a20 2020 2020 2041 6374 6976 6174 696f  .      Activatio
-00020410: 6e20 6675 6e63 7469 6f6e 2061 7070 6c69  n function appli
-00020420: 6564 0a20 2020 2062 6174 6368 5f6e 6f72  ed.    batch_nor
-00020430: 6d61 6c69 7a65 3a20 626f 6f6c 2c20 6f70  malize: bool, op
-00020440: 7469 6f6e 616c 2028 6465 6661 756c 7420  tional (default 
-00020450: 5472 7565 290a 2020 2020 2020 4966 2074  True).      If t
-00020460: 6869 7320 6973 2074 7572 6e65 6420 6f6e  his is turned on
-00020470: 2c20 6170 706c 7920 6261 7463 6820 6e6f  , apply batch no
-00020480: 726d 616c 697a 6174 696f 6e20 6265 666f  rmalization befo
-00020490: 7265 2061 7070 6c79 696e 670a 2020 2020  re applying.    
-000204a0: 2020 6163 7469 7661 7469 6f6e 2066 756e    activation fun
-000204b0: 6374 696f 6e73 206f 6e20 636f 6e76 6f6c  ctions on convol
-000204c0: 7574 696f 6e61 6c20 6c61 7965 7273 2e0a  utional layers..
-000204d0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-000204e0: 7375 7065 7228 5765 6176 654c 6179 6572  super(WeaveLayer
-000204f0: 2c20 7365 6c66 292e 5f5f 696e 6974 5f5f  , self).__init__
-00020500: 282a 2a6b 7761 7267 7329 0a20 2020 2020  (**kwargs).     
-00020510: 2020 2073 656c 662e 696e 6974 3a20 7374     self.init: st
-00020520: 7220 3d20 696e 6974 5f20 2023 2053 6574  r = init_  # Set
-00020530: 2077 6569 6768 7420 696e 6974 6961 6c69   weight initiali
-00020540: 7a61 7469 6f6e 0a20 2020 2020 2020 2073  zation.        s
-00020550: 656c 662e 6163 7469 7661 7469 6f6e 3a20  elf.activation: 
-00020560: 7374 7220 3d20 6163 7469 7661 7469 6f6e  str = activation
-00020570: 2020 2320 4765 7420 6163 7469 7661 7469    # Get activati
-00020580: 6f6e 730a 2020 2020 2020 2020 7365 6c66  ons.        self
-00020590: 2e61 6374 6976 6174 696f 6e5f 666e 3a20  .activation_fn: 
-000205a0: 746f 7263 682e 6e6e 2e4d 6f64 756c 6520  torch.nn.Module 
-000205b0: 3d20 6765 745f 6163 7469 7661 7469 6f6e  = get_activation
-000205c0: 2861 6374 6976 6174 696f 6e29 0a20 2020  (activation).   
-000205d0: 2020 2020 2073 656c 662e 7570 6461 7465       self.update
-000205e0: 5f70 6169 723a 2062 6f6f 6c20 3d20 7570  _pair: bool = up
-000205f0: 6461 7465 5f70 6169 7220 2023 206c 6173  date_pair  # las
-00020600: 7420 7765 6176 6520 6c61 7965 7220 646f  t weave layer do
-00020610: 6573 206e 6f74 206e 6565 6420 746f 2075  es not need to u
-00020620: 7064 6174 650a 2020 2020 2020 2020 7365  pdate.        se
-00020630: 6c66 2e6e 5f68 6964 6465 6e5f 4141 3a20  lf.n_hidden_AA: 
-00020640: 696e 7420 3d20 6e5f 6869 6464 656e 5f41  int = n_hidden_A
-00020650: 410a 2020 2020 2020 2020 7365 6c66 2e6e  A.        self.n
-00020660: 5f68 6964 6465 6e5f 5041 3a20 696e 7420  _hidden_PA: int 
-00020670: 3d20 6e5f 6869 6464 656e 5f50 410a 2020  = n_hidden_PA.  
-00020680: 2020 2020 2020 7365 6c66 2e6e 5f68 6964        self.n_hid
-00020690: 6465 6e5f 4150 3a20 696e 7420 3d20 6e5f  den_AP: int = n_
-000206a0: 6869 6464 656e 5f41 500a 2020 2020 2020  hidden_AP.      
-000206b0: 2020 7365 6c66 2e6e 5f68 6964 6465 6e5f    self.n_hidden_
-000206c0: 5050 3a20 696e 7420 3d20 6e5f 6869 6464  PP: int = n_hidd
-000206d0: 656e 5f50 500a 2020 2020 2020 2020 7365  en_PP.        se
-000206e0: 6c66 2e6e 5f68 6964 6465 6e5f 413a 2069  lf.n_hidden_A: i
-000206f0: 6e74 203d 206e 5f68 6964 6465 6e5f 4141  nt = n_hidden_AA
-00020700: 202b 206e 5f68 6964 6465 6e5f 5041 0a20   + n_hidden_PA. 
-00020710: 2020 2020 2020 2073 656c 662e 6e5f 6869         self.n_hi
-00020720: 6464 656e 5f50 3a20 696e 7420 3d20 6e5f  dden_P: int = n_
-00020730: 6869 6464 656e 5f41 5020 2b20 6e5f 6869  hidden_AP + n_hi
-00020740: 6464 656e 5f50 500a 2020 2020 2020 2020  dden_PP.        
-00020750: 7365 6c66 2e62 6174 6368 5f6e 6f72 6d61  self.batch_norma
-00020760: 6c69 7a65 3a20 626f 6f6c 203d 2062 6174  lize: bool = bat
-00020770: 6368 5f6e 6f72 6d61 6c69 7a65 0a0a 2020  ch_normalize..  
-00020780: 2020 2020 2020 7365 6c66 2e6e 5f61 746f        self.n_ato
-00020790: 6d5f 696e 7075 745f 6665 6174 3a20 696e  m_input_feat: in
-000207a0: 7420 3d20 6e5f 6174 6f6d 5f69 6e70 7574  t = n_atom_input
-000207b0: 5f66 6561 740a 2020 2020 2020 2020 7365  _feat.        se
-000207c0: 6c66 2e6e 5f70 6169 725f 696e 7075 745f  lf.n_pair_input_
-000207d0: 6665 6174 3a20 696e 7420 3d20 6e5f 7061  feat: int = n_pa
-000207e0: 6972 5f69 6e70 7574 5f66 6561 740a 2020  ir_input_feat.  
-000207f0: 2020 2020 2020 7365 6c66 2e6e 5f61 746f        self.n_ato
-00020800: 6d5f 6f75 7470 7574 5f66 6561 743a 2069  m_output_feat: i
-00020810: 6e74 203d 206e 5f61 746f 6d5f 6f75 7470  nt = n_atom_outp
-00020820: 7574 5f66 6561 740a 2020 2020 2020 2020  ut_feat.        
-00020830: 7365 6c66 2e6e 5f70 6169 725f 6f75 7470  self.n_pair_outp
-00020840: 7574 5f66 6561 743a 2069 6e74 203d 206e  ut_feat: int = n
-00020850: 5f70 6169 725f 6f75 7470 7574 5f66 6561  _pair_output_fea
-00020860: 740a 0a20 2020 2020 2020 2023 2043 6f6e  t..        # Con
-00020870: 7374 7275 6374 2069 6e74 6572 6e61 6c20  struct internal 
-00020880: 7472 6169 6e61 626c 6520 7765 6967 6874  trainable weight
-00020890: 730a 2020 2020 2020 2020 696e 6974 203d  s.        init =
-000208a0: 2067 6574 6174 7472 2869 6e69 7469 616c   getattr(initial
-000208b0: 697a 6572 732c 2073 656c 662e 696e 6974  izers, self.init
-000208c0: 290a 2020 2020 2020 2020 2320 5765 6967  ).        # Weig
-000208d0: 6874 206d 6174 7269 7820 616e 6420 6269  ht matrix and bi
-000208e0: 6173 206d 6174 7269 7820 7265 7175 6972  as matrix requir
-000208f0: 6564 2074 6f20 636f 6d70 7574 6520 6e65  ed to compute ne
-00020900: 7720 6174 6f6d 206c 6179 6572 2066 726f  w atom layer fro
-00020910: 6d20 7468 6520 7072 6576 696f 7573 2061  m the previous a
-00020920: 746f 6d20 6c61 7965 720a 2020 2020 2020  tom layer.      
-00020930: 2020 7365 6c66 2e57 5f41 413a 2074 6f72    self.W_AA: tor
-00020940: 6368 2e54 656e 736f 7220 3d20 696e 6974  ch.Tensor = init
-00020950: 280a 2020 2020 2020 2020 2020 2020 746f  (.            to
-00020960: 7263 682e 656d 7074 7928 7365 6c66 2e6e  rch.empty(self.n
-00020970: 5f61 746f 6d5f 696e 7075 745f 6665 6174  _atom_input_feat
-00020980: 2c20 7365 6c66 2e6e 5f68 6964 6465 6e5f  , self.n_hidden_
-00020990: 4141 2929 0a20 2020 2020 2020 2073 656c  AA)).        sel
-000209a0: 662e 625f 4141 3a20 746f 7263 682e 5465  f.b_AA: torch.Te
-000209b0: 6e73 6f72 203d 2074 6f72 6368 2e7a 6572  nsor = torch.zer
-000209c0: 6f73 2828 7365 6c66 2e6e 5f68 6964 6465  os((self.n_hidde
-000209d0: 6e5f 4141 2c29 290a 2020 2020 2020 2020  n_AA,)).        
-000209e0: 7365 6c66 2e41 415f 626e 3a20 6e6e 2e42  self.AA_bn: nn.B
-000209f0: 6174 6368 4e6f 726d 3164 203d 206e 6e2e  atchNorm1d = nn.
-00020a00: 4261 7463 684e 6f72 6d31 6428 0a20 2020  BatchNorm1d(.   
-00020a10: 2020 2020 2020 2020 206e 756d 5f66 6561           num_fea
-00020a20: 7475 7265 733d 7365 6c66 2e6e 5f68 6964  tures=self.n_hid
-00020a30: 6465 6e5f 4141 2c0a 2020 2020 2020 2020  den_AA,.        
-00020a40: 2020 2020 6570 733d 3165 2d33 2c0a 2020      eps=1e-3,.  
-00020a50: 2020 2020 2020 2020 2020 6d6f 6d65 6e74            moment
-00020a60: 756d 3d30 2e39 392c 0a20 2020 2020 2020  um=0.99,.       
-00020a70: 2020 2020 2061 6666 696e 653d 5472 7565       affine=True
-00020a80: 2c0a 2020 2020 2020 2020 2020 2020 7472  ,.            tr
-00020a90: 6163 6b5f 7275 6e6e 696e 675f 7374 6174  ack_running_stat
-00020aa0: 733d 5472 7565 290a 0a20 2020 2020 2020  s=True)..       
-00020ab0: 2023 2057 6569 6768 7420 6d61 7472 6978   # Weight matrix
-00020ac0: 2061 6e64 2062 6961 7320 6d61 7472 6978   and bias matrix
-00020ad0: 2072 6571 7569 7265 6420 746f 2063 6f6d   required to com
-00020ae0: 7075 7465 206e 6577 2061 746f 6d20 6c61  pute new atom la
-00020af0: 7965 7220 6672 6f6d 2074 6865 2070 7265  yer from the pre
-00020b00: 7669 6f75 7320 7061 6972 206c 6179 6572  vious pair layer
-00020b10: 0a20 2020 2020 2020 2073 656c 662e 575f  .        self.W_
-00020b20: 5041 3a20 746f 7263 682e 5465 6e73 6f72  PA: torch.Tensor
-00020b30: 203d 2069 6e69 7428 0a20 2020 2020 2020   = init(.       
-00020b40: 2020 2020 2074 6f72 6368 2e65 6d70 7479       torch.empty
-00020b50: 2873 656c 662e 6e5f 7061 6972 5f69 6e70  (self.n_pair_inp
-00020b60: 7574 5f66 6561 742c 2073 656c 662e 6e5f  ut_feat, self.n_
-00020b70: 6869 6464 656e 5f50 4129 290a 2020 2020  hidden_PA)).    
-00020b80: 2020 2020 7365 6c66 2e62 5f50 413a 2074      self.b_PA: t
-00020b90: 6f72 6368 2e54 656e 736f 7220 3d20 746f  orch.Tensor = to
-00020ba0: 7263 682e 7a65 726f 7328 2873 656c 662e  rch.zeros((self.
-00020bb0: 6e5f 6869 6464 656e 5f50 412c 2929 0a20  n_hidden_PA,)). 
-00020bc0: 2020 2020 2020 2073 656c 662e 5041 5f62         self.PA_b
-00020bd0: 6e3a 206e 6e2e 4261 7463 684e 6f72 6d31  n: nn.BatchNorm1
-00020be0: 6420 3d20 6e6e 2e42 6174 6368 4e6f 726d  d = nn.BatchNorm
-00020bf0: 3164 280a 2020 2020 2020 2020 2020 2020  1d(.            
-00020c00: 6e75 6d5f 6665 6174 7572 6573 3d73 656c  num_features=sel
-00020c10: 662e 6e5f 6869 6464 656e 5f50 412c 0a20  f.n_hidden_PA,. 
-00020c20: 2020 2020 2020 2020 2020 2065 7073 3d31             eps=1
-00020c30: 652d 332c 0a20 2020 2020 2020 2020 2020  e-3,.           
-00020c40: 206d 6f6d 656e 7475 6d3d 302e 3939 2c0a   momentum=0.99,.
-00020c50: 2020 2020 2020 2020 2020 2020 6166 6669              affi
-00020c60: 6e65 3d54 7275 652c 0a20 2020 2020 2020  ne=True,.       
-00020c70: 2020 2020 2074 7261 636b 5f72 756e 6e69       track_runni
-00020c80: 6e67 5f73 7461 7473 3d54 7275 6529 0a0a  ng_stats=True)..
-00020c90: 2020 2020 2020 2020 7365 6c66 2e57 5f41          self.W_A
-00020ca0: 3a20 746f 7263 682e 5465 6e73 6f72 203d  : torch.Tensor =
-00020cb0: 2069 6e69 7428 0a20 2020 2020 2020 2020   init(.         
-00020cc0: 2020 2074 6f72 6368 2e65 6d70 7479 2873     torch.empty(s
-00020cd0: 656c 662e 6e5f 6869 6464 656e 5f41 2c20  elf.n_hidden_A, 
-00020ce0: 7365 6c66 2e6e 5f61 746f 6d5f 6f75 7470  self.n_atom_outp
-00020cf0: 7574 5f66 6561 7429 290a 2020 2020 2020  ut_feat)).      
-00020d00: 2020 7365 6c66 2e62 5f41 3a20 746f 7263    self.b_A: torc
-00020d10: 682e 5465 6e73 6f72 203d 2074 6f72 6368  h.Tensor = torch
-00020d20: 2e7a 6572 6f73 2828 7365 6c66 2e6e 5f61  .zeros((self.n_a
-00020d30: 746f 6d5f 6f75 7470 7574 5f66 6561 742c  tom_output_feat,
-00020d40: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
-00020d50: 415f 626e 3a20 6e6e 2e42 6174 6368 4e6f  A_bn: nn.BatchNo
-00020d60: 726d 3164 203d 206e 6e2e 4261 7463 684e  rm1d = nn.BatchN
-00020d70: 6f72 6d31 6428 0a20 2020 2020 2020 2020  orm1d(.         
-00020d80: 2020 206e 756d 5f66 6561 7475 7265 733d     num_features=
-00020d90: 7365 6c66 2e6e 5f61 746f 6d5f 6f75 7470  self.n_atom_outp
-00020da0: 7574 5f66 6561 742c 0a20 2020 2020 2020  ut_feat,.       
-00020db0: 2020 2020 2065 7073 3d31 652d 332c 0a20       eps=1e-3,. 
-00020dc0: 2020 2020 2020 2020 2020 206d 6f6d 656e             momen
-00020dd0: 7475 6d3d 302e 3939 2c0a 2020 2020 2020  tum=0.99,.      
-00020de0: 2020 2020 2020 6166 6669 6e65 3d54 7275        affine=Tru
-00020df0: 652c 0a20 2020 2020 2020 2020 2020 2074  e,.            t
-00020e00: 7261 636b 5f72 756e 6e69 6e67 5f73 7461  rack_running_sta
-00020e10: 7473 3d54 7275 6529 0a0a 2020 2020 2020  ts=True)..      
-00020e20: 2020 6966 2073 656c 662e 7570 6461 7465    if self.update
-00020e30: 5f70 6169 723a 0a20 2020 2020 2020 2020  _pair:.         
-00020e40: 2020 2023 2057 6569 6768 7420 6d61 7472     # Weight matr
-00020e50: 6978 2061 6e64 2062 6961 7320 6d61 7472  ix and bias matr
-00020e60: 6978 2072 6571 7569 7265 6420 746f 2063  ix required to c
-00020e70: 6f6d 7075 7465 206e 6577 2070 6169 7220  ompute new pair 
-00020e80: 6c61 7965 7220 6672 6f6d 2074 6865 2070  layer from the p
-00020e90: 7265 7669 6f75 7320 6174 6f6d 206c 6179  revious atom lay
-00020ea0: 6572 0a20 2020 2020 2020 2020 2020 2073  er.            s
-00020eb0: 656c 662e 575f 4150 3a20 746f 7263 682e  elf.W_AP: torch.
-00020ec0: 5465 6e73 6f72 203d 2069 6e69 7428 0a20  Tensor = init(. 
-00020ed0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00020ee0: 6f72 6368 2e65 6d70 7479 2873 656c 662e  orch.empty(self.
-00020ef0: 6e5f 6174 6f6d 5f69 6e70 7574 5f66 6561  n_atom_input_fea
-00020f00: 7420 2a20 322c 2073 656c 662e 6e5f 6869  t * 2, self.n_hi
-00020f10: 6464 656e 5f41 5029 290a 2020 2020 2020  dden_AP)).      
-00020f20: 2020 2020 2020 7365 6c66 2e62 5f41 503a        self.b_AP:
-00020f30: 2074 6f72 6368 2e54 656e 736f 7220 3d20   torch.Tensor = 
-00020f40: 746f 7263 682e 7a65 726f 7328 2873 656c  torch.zeros((sel
-00020f50: 662e 6e5f 6869 6464 656e 5f41 502c 2929  f.n_hidden_AP,))
-00020f60: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00020f70: 662e 4150 5f62 6e3a 206e 6e2e 4261 7463  f.AP_bn: nn.Batc
-00020f80: 684e 6f72 6d31 6420 3d20 6e6e 2e42 6174  hNorm1d = nn.Bat
-00020f90: 6368 4e6f 726d 3164 280a 2020 2020 2020  chNorm1d(.      
-00020fa0: 2020 2020 2020 2020 2020 6e75 6d5f 6665            num_fe
-00020fb0: 6174 7572 6573 3d73 656c 662e 6e5f 6869  atures=self.n_hi
-00020fc0: 6464 656e 5f41 502c 0a20 2020 2020 2020  dden_AP,.       
-00020fd0: 2020 2020 2020 2020 2065 7073 3d31 652d           eps=1e-
-00020fe0: 332c 0a20 2020 2020 2020 2020 2020 2020  3,.             
-00020ff0: 2020 206d 6f6d 656e 7475 6d3d 302e 3939     momentum=0.99
-00021000: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00021010: 2020 6166 6669 6e65 3d54 7275 652c 0a20    affine=True,. 
-00021020: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00021030: 7261 636b 5f72 756e 6e69 6e67 5f73 7461  rack_running_sta
-00021040: 7473 3d54 7275 6529 0a20 2020 2020 2020  ts=True).       
-00021050: 2020 2020 2023 2057 6569 6768 7420 6d61       # Weight ma
-00021060: 7472 6978 2061 6e64 2062 6961 7320 6d61  trix and bias ma
-00021070: 7472 6978 2072 6571 7569 7265 6420 746f  trix required to
-00021080: 2063 6f6d 7075 7465 206e 6577 2070 6169   compute new pai
-00021090: 7220 6c61 7965 7220 6672 6f6d 2074 6865  r layer from the
-000210a0: 2070 7265 7669 6f75 7320 7061 6972 206c   previous pair l
-000210b0: 6179 6572 0a20 2020 2020 2020 2020 2020  ayer.           
-000210c0: 2073 656c 662e 575f 5050 3a20 746f 7263   self.W_PP: torc
-000210d0: 682e 5465 6e73 6f72 203d 2069 6e69 7428  h.Tensor = init(
-000210e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000210f0: 2074 6f72 6368 2e65 6d70 7479 2873 656c   torch.empty(sel
-00021100: 662e 6e5f 7061 6972 5f69 6e70 7574 5f66  f.n_pair_input_f
-00021110: 6561 742c 2073 656c 662e 6e5f 6869 6464  eat, self.n_hidd
-00021120: 656e 5f50 5029 290a 2020 2020 2020 2020  en_PP)).        
-00021130: 2020 2020 7365 6c66 2e62 5f50 503a 2074      self.b_PP: t
-00021140: 6f72 6368 2e54 656e 736f 7220 3d20 746f  orch.Tensor = to
-00021150: 7263 682e 7a65 726f 7328 2873 656c 662e  rch.zeros((self.
-00021160: 6e5f 6869 6464 656e 5f50 502c 2929 0a20  n_hidden_PP,)). 
-00021170: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00021180: 5050 5f62 6e3a 206e 6e2e 4261 7463 684e  PP_bn: nn.BatchN
-00021190: 6f72 6d31 6420 3d20 6e6e 2e42 6174 6368  orm1d = nn.Batch
-000211a0: 4e6f 726d 3164 280a 2020 2020 2020 2020  Norm1d(.        
-000211b0: 2020 2020 2020 2020 6e75 6d5f 6665 6174          num_feat
-000211c0: 7572 6573 3d73 656c 662e 6e5f 6869 6464  ures=self.n_hidd
-000211d0: 656e 5f50 502c 0a20 2020 2020 2020 2020  en_PP,.         
-000211e0: 2020 2020 2020 2065 7073 3d31 652d 332c         eps=1e-3,
-000211f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00021200: 206d 6f6d 656e 7475 6d3d 302e 3939 2c0a   momentum=0.99,.
-00021210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021220: 6166 6669 6e65 3d54 7275 652c 0a20 2020  affine=True,.   
-00021230: 2020 2020 2020 2020 2020 2020 2074 7261               tra
-00021240: 636b 5f72 756e 6e69 6e67 5f73 7461 7473  ck_running_stats
-00021250: 3d54 7275 6529 0a0a 2020 2020 2020 2020  =True)..        
-00021260: 2020 2020 7365 6c66 2e57 5f50 3a20 746f      self.W_P: to
-00021270: 7263 682e 5465 6e73 6f72 203d 2069 6e69  rch.Tensor = ini
-00021280: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
-00021290: 2020 2074 6f72 6368 2e65 6d70 7479 2873     torch.empty(s
-000212a0: 656c 662e 6e5f 6869 6464 656e 5f50 2c20  elf.n_hidden_P, 
-000212b0: 7365 6c66 2e6e 5f70 6169 725f 6f75 7470  self.n_pair_outp
-000212c0: 7574 5f66 6561 7429 290a 2020 2020 2020  ut_feat)).      
-000212d0: 2020 2020 2020 7365 6c66 2e62 5f50 3a20        self.b_P: 
-000212e0: 746f 7263 682e 5465 6e73 6f72 203d 2074  torch.Tensor = t
-000212f0: 6f72 6368 2e7a 6572 6f73 2828 7365 6c66  orch.zeros((self
-00021300: 2e6e 5f70 6169 725f 6f75 7470 7574 5f66  .n_pair_output_f
-00021310: 6561 742c 2929 0a20 2020 2020 2020 2020  eat,)).         
-00021320: 2020 2073 656c 662e 505f 626e 3a20 6e6e     self.P_bn: nn
-00021330: 2e42 6174 6368 4e6f 726d 3164 203d 206e  .BatchNorm1d = n
-00021340: 6e2e 4261 7463 684e 6f72 6d31 6428 0a20  n.BatchNorm1d(. 
-00021350: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00021360: 756d 5f66 6561 7475 7265 733d 7365 6c66  um_features=self
-00021370: 2e6e 5f70 6169 725f 6f75 7470 7574 5f66  .n_pair_output_f
-00021380: 6561 742c 0a20 2020 2020 2020 2020 2020  eat,.           
-00021390: 2020 2020 2065 7073 3d31 652d 332c 0a20       eps=1e-3,. 
-000213a0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-000213b0: 6f6d 656e 7475 6d3d 302e 3939 2c0a 2020  omentum=0.99,.  
-000213c0: 2020 2020 2020 2020 2020 2020 2020 6166                af
-000213d0: 6669 6e65 3d54 7275 652c 0a20 2020 2020  fine=True,.     
-000213e0: 2020 2020 2020 2020 2020 2074 7261 636b             track
-000213f0: 5f72 756e 6e69 6e67 5f73 7461 7473 3d54  _running_stats=T
-00021400: 7275 6529 0a20 2020 2020 2020 2073 656c  rue).        sel
-00021410: 662e 6275 696c 7420 3d20 5472 7565 0a0a  f.built = True..
-00021420: 2020 2020 6465 6620 5f5f 7265 7072 5f5f      def __repr__
-00021430: 2873 656c 6629 202d 3e20 7374 723a 0a20  (self) -> str:. 
-00021440: 2020 2020 2020 2022 2222 0a20 2020 2052         """.    R
-00021450: 6574 7572 6e73 2061 2073 7472 696e 6720  eturns a string 
-00021460: 7265 7072 6573 656e 7461 7469 6f6e 206f  representation o
-00021470: 6620 7468 6520 6f62 6a65 6374 2e0a 0a20  f the object... 
-00021480: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-00021490: 2d2d 2d2d 2d2d 2d0a 2020 2020 7374 723a  -------.    str:
-000214a0: 2041 2073 7472 696e 6720 7468 6174 2063   A string that c
-000214b0: 6f6e 7461 696e 7320 7468 6520 636c 6173  ontains the clas
-000214c0: 7320 6e61 6d65 2066 6f6c 6c6f 7765 6420  s name followed 
-000214d0: 6279 2074 6865 2076 616c 7565 7320 6f66  by the values of
-000214e0: 2069 7473 2069 6e73 7461 6e63 6520 7661   its instance va
-000214f0: 7269 6162 6c65 2e0a 2020 2020 2222 220a  riable..    """.
-00021500: 2020 2020 2020 2020 2320 666c 616b 6538          # flake8
-00021510: 3a20 6e6f 7161 0a20 2020 2020 2020 2072  : noqa.        r
-00021520: 6574 7572 6e20 280a 2020 2020 2020 2020  eturn (.        
-00021530: 2020 2020 6627 7b73 656c 662e 5f5f 636c      f'{self.__cl
-00021540: 6173 735f 5f2e 5f5f 6e61 6d65 5f5f 7d28  ass__.__name__}(
-00021550: 6e5f 6174 6f6d 5f69 6e70 7574 5f66 6561  n_atom_input_fea
-00021560: 743a 7b73 656c 662e 6e5f 6174 6f6d 5f69  t:{self.n_atom_i
-00021570: 6e70 7574 5f66 6561 747d 2c6e 5f70 6169  nput_feat},n_pai
-00021580: 725f 696e 7075 745f 6665 6174 3a7b 7365  r_input_feat:{se
-00021590: 6c66 2e6e 5f70 6169 725f 696e 7075 745f  lf.n_pair_input_
-000215a0: 6665 6174 7d2c 6e5f 6174 6f6d 5f6f 7574  feat},n_atom_out
-000215b0: 7075 745f 6665 6174 3a7b 7365 6c66 2e6e  put_feat:{self.n
-000215c0: 5f61 746f 6d5f 6f75 7470 7574 5f66 6561  _atom_output_fea
-000215d0: 747d 2c6e 5f70 6169 725f 6f75 7470 7574  t},n_pair_output
-000215e0: 5f66 6561 743a 7b73 656c 662e 6e5f 7061  _feat:{self.n_pa
-000215f0: 6972 5f6f 7574 7075 745f 6665 6174 7d2c  ir_output_feat},
-00021600: 6e5f 6869 6464 656e 5f41 413a 7b73 656c  n_hidden_AA:{sel
-00021610: 662e 6e5f 6869 6464 656e 5f41 417d 2c6e  f.n_hidden_AA},n
-00021620: 5f68 6964 6465 6e5f 5041 3a7b 7365 6c66  _hidden_PA:{self
-00021630: 2e6e 5f68 6964 6465 6e5f 5041 7d2c 6e5f  .n_hidden_PA},n_
-00021640: 6869 6464 656e 5f41 503a 7b73 656c 662e  hidden_AP:{self.
-00021650: 6e5f 6869 6464 656e 5f41 507d 2c6e 5f68  n_hidden_AP},n_h
-00021660: 6964 6465 6e5f 5050 3a7b 7365 6c66 2e6e  idden_PP:{self.n
-00021670: 5f68 6964 6465 6e5f 5050 7d2c 6261 7463  _hidden_PP},batc
-00021680: 685f 6e6f 726d 616c 697a 653a 7b73 656c  h_normalize:{sel
-00021690: 662e 6261 7463 685f 6e6f 726d 616c 697a  f.batch_normaliz
-000216a0: 657d 2c75 7064 6174 655f 7061 6972 3a7b  e},update_pair:{
-000216b0: 7365 6c66 2e75 7064 6174 655f 7061 6972  self.update_pair
-000216c0: 7d2c 696e 6974 3a7b 7365 6c66 2e69 6e69  },init:{self.ini
-000216d0: 747d 2c61 6374 6976 6174 696f 6e3a 7b73  t},activation:{s
-000216e0: 656c 662e 6163 7469 7661 7469 6f6e 7d29  elf.activation})
-000216f0: 270a 2020 2020 2020 2020 290a 0a20 2020  '.        )..   
-00021700: 2064 6566 2066 6f72 7761 7264 280a 2020   def forward(.  
-00021710: 2020 2020 2020 7365 6c66 2c20 696e 7075        self, inpu
-00021720: 7473 3a20 4c69 7374 5b55 6e69 6f6e 5b6e  ts: List[Union[n
-00021730: 702e 6e64 6172 7261 792c 206e 702e 6e64  p.ndarray, np.nd
-00021740: 6172 7261 792c 206e 702e 6e64 6172 7261  array, np.ndarra
-00021750: 792c 0a20 2020 2020 2020 2020 2020 2020  y,.             
-00021760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021770: 2020 2020 6e70 2e6e 6461 7272 6179 5d5d      np.ndarray]]
-00021780: 0a20 2020 2029 202d 3e20 4c69 7374 5b55  .    ) -> List[U
-00021790: 6e69 6f6e 5b74 6f72 6368 2e54 656e 736f  nion[torch.Tenso
-000217a0: 722c 2074 6f72 6368 2e54 656e 736f 725d  r, torch.Tensor]
-000217b0: 5d3a 0a20 2020 2020 2020 2022 2222 0a20  ]:.        """. 
-000217c0: 2020 2043 7265 6174 6573 2077 6561 7665     Creates weave
-000217d0: 2074 656e 736f 7273 2e0a 0a20 2020 2050   tensors...    P
-000217e0: 6172 616d 6574 6572 730a 2020 2020 2d2d  arameters.    --
-000217f0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2069 6e70  --------.    inp
-00021800: 7574 733a 204c 6973 745b 556e 696f 6e5b  uts: List[Union[
-00021810: 6e70 2e6e 6461 7272 6179 2c20 6e70 2e6e  np.ndarray, np.n
-00021820: 6461 7272 6179 2c20 6e70 2e6e 6461 7272  darray, np.ndarr
-00021830: 6179 2c20 6e70 2e6e 6461 7272 6179 5d5d  ay, np.ndarray]]
-00021840: 0a20 2020 2053 686f 756c 6420 636f 6e74  .    Should cont
-00021850: 6169 6e20 3420 7465 6e73 6f72 7320 5b61  ain 4 tensors [a
-00021860: 746f 6d5f 6665 6174 7572 6573 2c20 7061  tom_features, pa
-00021870: 6972 5f66 6561 7475 7265 732c 2070 6169  ir_features, pai
-00021880: 725f 7370 6c69 742c 0a20 2020 2061 746f  r_split,.    ato
-00021890: 6d5f 746f 5f70 6169 725d 0a0a 2020 2020  m_to_pair]..    
-000218a0: 5265 7475 726e 733a 0a20 2020 202d 2d2d  Returns:.    ---
-000218b0: 2d2d 2d2d 0a20 2020 204c 6973 745b 556e  ----.    List[Un
-000218c0: 696f 6e5b 746f 7263 682e 5465 6e73 6f72  ion[torch.Tensor
-000218d0: 2c20 746f 7263 682e 5465 6e73 6f72 5d5d  , torch.Tensor]]
-000218e0: 0a20 2020 2020 2041 3a20 4174 6f6d 2066  .      A: Atom f
-000218f0: 6561 7475 7265 7320 7465 6e73 6f72 2077  eatures tensor w
-00021900: 6974 6820 7368 6170 655b 746f 7461 6c5f  ith shape[total_
-00021910: 6e75 6d5f 6174 6f6d 732c 6174 6f6d 2066  num_atoms,atom f
-00021920: 6561 7475 7265 2073 697a 655d 0a20 2020  eature size].   
-00021930: 2020 2050 3a20 5061 6972 2066 6561 7475     P: Pair featu
-00021940: 7265 7320 7465 6e73 6f72 2077 6974 6820  res tensor with 
-00021950: 7368 6170 655b 746f 7461 6c20 6e75 6d20  shape[total num 
-00021960: 6f66 2070 6169 7273 2c62 6f6e 6420 6665  of pairs,bond fe
-00021970: 6174 7572 6520 7369 7a65 5d0a 2020 2020  ature size].    
-00021980: 2222 220a 2020 2020 2020 2020 2320 436f  """.        # Co
-00021990: 6e76 6572 7469 6e67 2074 6865 2069 6e70  nverting the inp
-000219a0: 7574 2074 6f20 746f 7263 6820 7465 6e73  ut to torch tens
-000219b0: 6f72 730a 2020 2020 2020 2020 6174 6f6d  ors.        atom
-000219c0: 5f66 6561 7475 7265 733a 2074 6f72 6368  _features: torch
-000219d0: 2e54 656e 736f 7220 3d20 746f 7263 682e  .Tensor = torch.
-000219e0: 7465 6e73 6f72 2869 6e70 7574 735b 305d  tensor(inputs[0]
-000219f0: 290a 2020 2020 2020 2020 7061 6972 5f66  ).        pair_f
-00021a00: 6561 7475 7265 733a 2074 6f72 6368 2e54  eatures: torch.T
-00021a10: 656e 736f 7220 3d20 746f 7263 682e 7465  ensor = torch.te
-00021a20: 6e73 6f72 2869 6e70 7574 735b 315d 290a  nsor(inputs[1]).
-00021a30: 0a20 2020 2020 2020 2070 6169 725f 7370  .        pair_sp
-00021a40: 6c69 743a 2074 6f72 6368 2e54 656e 736f  lit: torch.Tenso
-00021a50: 7220 3d20 746f 7263 682e 7465 6e73 6f72  r = torch.tensor
-00021a60: 2869 6e70 7574 735b 325d 290a 2020 2020  (inputs[2]).    
-00021a70: 2020 2020 6174 6f6d 5f74 6f5f 7061 6972      atom_to_pair
-00021a80: 3a20 746f 7263 682e 5465 6e73 6f72 203d  : torch.Tensor =
-00021a90: 2074 6f72 6368 2e74 656e 736f 7228 696e   torch.tensor(in
-00021aa0: 7075 7473 5b33 5d29 0a0a 2020 2020 2020  puts[3])..      
-00021ab0: 2020 6163 7469 7661 7469 6f6e 203d 2073    activation = s
-00021ac0: 656c 662e 6163 7469 7661 7469 6f6e 5f66  elf.activation_f
-00021ad0: 6e0a 0a20 2020 2020 2020 2023 2041 4120  n..        # AA 
-00021ae0: 6973 2061 2074 656e 736f 7220 7769 7468  is a tensor with
-00021af0: 2073 6861 7065 5b74 6f74 616c 5f6e 756d   shape[total_num
-00021b00: 5f61 746f 6d73 2c6e 5f68 6964 6465 6e5f  _atoms,n_hidden_
-00021b10: 4141 5d0a 2020 2020 2020 2020 4141 3a20  AA].        AA: 
-00021b20: 746f 7263 682e 5465 6e73 6f72 203d 2074  torch.Tensor = t
-00021b30: 6f72 6368 2e6d 6174 6d75 6c28 6174 6f6d  orch.matmul(atom
-00021b40: 5f66 6561 7475 7265 732e 7479 7065 2874  _features.type(t
-00021b50: 6f72 6368 2e66 6c6f 6174 3332 292c 0a20  orch.float32),. 
-00021b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021b80: 2020 2020 2020 2073 656c 662e 575f 4141         self.W_AA
-00021b90: 2920 2b20 7365 6c66 2e62 5f41 410a 2020  ) + self.b_AA.  
-00021ba0: 2020 2020 2020 6966 2073 656c 662e 6261        if self.ba
-00021bb0: 7463 685f 6e6f 726d 616c 697a 653a 0a20  tch_normalize:. 
-00021bc0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00021bd0: 4141 5f62 6e2e 6576 616c 2829 0a20 2020  AA_bn.eval().   
-00021be0: 2020 2020 2020 2020 2041 4120 3d20 7365           AA = se
-00021bf0: 6c66 2e41 415f 626e 2841 4129 0a20 2020  lf.AA_bn(AA).   
-00021c00: 2020 2020 2041 4120 3d20 6163 7469 7661       AA = activa
-00021c10: 7469 6f6e 2841 4129 0a20 2020 2020 2020  tion(AA).       
-00021c20: 2023 2050 4120 6973 2061 2074 656e 736f   # PA is a tenso
-00021c30: 7220 7769 7468 2073 6861 7065 5b74 6f74  r with shape[tot
-00021c40: 616c 206e 756d 6265 7220 6f66 2070 6169  al number of pai
-00021c50: 7273 2c6e 5f68 6964 6465 6e5f 5041 5d0a  rs,n_hidden_PA].
-00021c60: 2020 2020 2020 2020 5041 3a20 746f 7263          PA: torc
-00021c70: 682e 5465 6e73 6f72 203d 2074 6f72 6368  h.Tensor = torch
-00021c80: 2e6d 6174 6d75 6c28 7061 6972 5f66 6561  .matmul(pair_fea
-00021c90: 7475 7265 732e 7479 7065 2874 6f72 6368  tures.type(torch
-00021ca0: 2e66 6c6f 6174 3332 292c 0a20 2020 2020  .float32),.     
-00021cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021cd0: 2020 2073 656c 662e 575f 5041 2920 2b20     self.W_PA) + 
-00021ce0: 7365 6c66 2e62 5f50 410a 2020 2020 2020  self.b_PA.      
-00021cf0: 2020 6966 2073 656c 662e 6261 7463 685f    if self.batch_
-00021d00: 6e6f 726d 616c 697a 653a 0a20 2020 2020  normalize:.     
-00021d10: 2020 2020 2020 2073 656c 662e 5041 5f62         self.PA_b
-00021d20: 6e2e 6576 616c 2829 0a20 2020 2020 2020  n.eval().       
-00021d30: 2020 2020 2050 4120 3d20 7365 6c66 2e50       PA = self.P
-00021d40: 415f 626e 2850 4129 0a20 2020 2020 2020  A_bn(PA).       
-00021d50: 2050 4120 3d20 6163 7469 7661 7469 6f6e   PA = activation
-00021d60: 2850 4129 0a0a 2020 2020 2020 2020 2320  (PA)..        # 
-00021d70: 5370 6c69 7420 7468 6520 5041 2074 656e  Split the PA ten
-00021d80: 736f 7220 6163 636f 7264 696e 6720 746f  sor according to
-00021d90: 2074 6865 2027 7061 6972 5f73 706c 6974   the 'pair_split
-00021da0: 2720 7465 6e73 6f72 0a20 2020 2020 2020  ' tensor.       
-00021db0: 2074 5f67 7270 3a20 4469 6374 5b54 656e   t_grp: Dict[Ten
-00021dc0: 736f 722c 2054 656e 736f 725d 203d 207b  sor, Tensor] = {
-00021dd0: 7d0a 2020 2020 2020 2020 6964 783a 2069  }.        idx: i
-00021de0: 6e74 203d 2030 0a20 2020 2020 2020 2066  nt = 0.        f
-00021df0: 6f72 2069 2c20 735f 6964 2069 6e20 656e  or i, s_id in en
-00021e00: 756d 6572 6174 6528 7061 6972 5f73 706c  umerate(pair_spl
-00021e10: 6974 293a 0a20 2020 2020 2020 2020 2020  it):.           
-00021e20: 2073 5f69 6420 3d20 735f 6964 2e69 7465   s_id = s_id.ite
-00021e30: 6d28 290a 2020 2020 2020 2020 2020 2020  m().            
-00021e40: 6966 2073 5f69 6420 696e 2074 5f67 7270  if s_id in t_grp
-00021e50: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00021e60: 2020 745f 6772 705b 735f 6964 5d20 3d20    t_grp[s_id] = 
-00021e70: 745f 6772 705b 735f 6964 5d20 2b20 5041  t_grp[s_id] + PA
-00021e80: 5b69 6478 5d0a 2020 2020 2020 2020 2020  [idx].          
-00021e90: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00021ea0: 2020 2020 2020 2020 745f 6772 705b 735f          t_grp[s_
-00021eb0: 6964 5d20 3d20 5041 5b69 6478 5d0a 2020  id] = PA[idx].  
-00021ec0: 2020 2020 2020 2020 2020 6964 7820 3d20            idx = 
-00021ed0: 6920 2b20 310a 0a20 2020 2020 2020 2020  i + 1..         
-00021ee0: 2020 206c 7374 203d 206c 6973 7428 745f     lst = list(t_
-00021ef0: 6772 702e 7661 6c75 6573 2829 290a 2020  grp.values()).  
-00021f00: 2020 2020 2020 2020 2020 7465 6e73 6f72            tensor
-00021f10: 203d 2074 6f72 6368 2e73 7461 636b 286c   = torch.stack(l
-00021f20: 7374 290a 2020 2020 2020 2020 5041 203d  st).        PA =
-00021f30: 2074 656e 736f 720a 0a20 2020 2020 2020   tensor..       
-00021f40: 2041 3a20 746f 7263 682e 5465 6e73 6f72   A: torch.Tensor
-00021f50: 203d 2074 6f72 6368 2e6d 6174 6d75 6c28   = torch.matmul(
-00021f60: 746f 7263 682e 636f 6e63 6174 285b 4141  torch.concat([AA
-00021f70: 2c20 5041 5d2c 2031 292c 0a20 2020 2020  , PA], 1),.     
-00021f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00021fa0: 2020 7365 6c66 2e57 5f41 2920 2b20 7365    self.W_A) + se
-00021fb0: 6c66 2e62 5f41 0a20 2020 2020 2020 2069  lf.b_A.        i
-00021fc0: 6620 7365 6c66 2e62 6174 6368 5f6e 6f72  f self.batch_nor
-00021fd0: 6d61 6c69 7a65 3a0a 2020 2020 2020 2020  malize:.        
-00021fe0: 2020 2020 7365 6c66 2e41 5f62 6e2e 6576      self.A_bn.ev
-00021ff0: 616c 2829 0a20 2020 2020 2020 2020 2020  al().           
-00022000: 2041 203d 2073 656c 662e 415f 626e 2841   A = self.A_bn(A
-00022010: 290a 2020 2020 2020 2020 4120 3d20 6163  ).        A = ac
-00022020: 7469 7661 7469 6f6e 2841 290a 0a20 2020  tivation(A)..   
-00022030: 2020 2020 2069 6620 7365 6c66 2e75 7064       if self.upd
-00022040: 6174 655f 7061 6972 3a0a 2020 2020 2020  ate_pair:.      
-00022050: 2020 2020 2020 2320 4e6f 7465 2074 6861        # Note tha
-00022060: 7420 4150 5f69 6a20 616e 6420 4150 5f6a  t AP_ij and AP_j
-00022070: 6920 7368 6172 6520 7468 6520 7361 6d65  i share the same
-00022080: 2073 656c 662e 4150 5f62 6e20 6261 7463   self.AP_bn batc
-00022090: 680a 2020 2020 2020 2020 2020 2020 2320  h.            # 
-000220a0: 6e6f 726d 616c 697a 6174 696f 6e0a 2020  normalization.  
-000220b0: 2020 2020 2020 2020 2020 4150 5f69 6a3a            AP_ij:
-000220c0: 2074 6f72 6368 2e54 656e 736f 7220 3d20   torch.Tensor = 
-000220d0: 746f 7263 682e 6d61 746d 756c 280a 2020  torch.matmul(.  
-000220e0: 2020 2020 2020 2020 2020 2020 2020 746f                to
-000220f0: 7263 682e 7265 7368 6170 6528 6174 6f6d  rch.reshape(atom
-00022100: 5f66 6561 7475 7265 735b 6174 6f6d 5f74  _features[atom_t
-00022110: 6f5f 7061 6972 5d2c 0a20 2020 2020 2020  o_pair],.       
-00022120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022130: 2020 2020 2020 205b 2d31 2c20 3220 2a20         [-1, 2 * 
-00022140: 7365 6c66 2e6e 5f61 746f 6d5f 696e 7075  self.n_atom_inpu
-00022150: 745f 6665 6174 5d29 2e74 7970 6528 0a20  t_feat]).type(. 
-00022160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022180: 2074 6f72 6368 2e66 6c6f 6174 3332 292c   torch.float32),
-00022190: 2073 656c 662e 575f 4150 2920 2b20 7365   self.W_AP) + se
-000221a0: 6c66 2e62 5f41 500a 2020 2020 2020 2020  lf.b_AP.        
-000221b0: 2020 2020 6966 2073 656c 662e 6261 7463      if self.batc
-000221c0: 685f 6e6f 726d 616c 697a 653a 0a20 2020  h_normalize:.   
-000221d0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000221e0: 662e 4150 5f62 6e2e 6576 616c 2829 0a20  f.AP_bn.eval(). 
-000221f0: 2020 2020 2020 2020 2020 2020 2020 2041                 A
-00022200: 505f 696a 203d 2073 656c 662e 4150 5f62  P_ij = self.AP_b
-00022210: 6e28 4150 5f69 6a29 0a20 2020 2020 2020  n(AP_ij).       
-00022220: 2020 2020 2041 505f 696a 203d 2061 6374       AP_ij = act
-00022230: 6976 6174 696f 6e28 4150 5f69 6a29 0a20  ivation(AP_ij). 
-00022240: 2020 2020 2020 2020 2020 2041 505f 6a69             AP_ji
-00022250: 3a20 746f 7263 682e 5465 6e73 6f72 203d  : torch.Tensor =
-00022260: 2074 6f72 6368 2e6d 6174 6d75 6c28 0a20   torch.matmul(. 
-00022270: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00022280: 6f72 6368 2e72 6573 6861 7065 2861 746f  orch.reshape(ato
-00022290: 6d5f 6665 6174 7572 6573 5b74 6f72 6368  m_features[torch
-000222a0: 2e66 6c69 7028 6174 6f6d 5f74 6f5f 7061  .flip(atom_to_pa
-000222b0: 6972 2c20 5b31 5d29 5d2c 0a20 2020 2020  ir, [1])],.     
-000222c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000222d0: 2020 2020 2020 2020 205b 2d31 2c20 3220           [-1, 2 
-000222e0: 2a20 7365 6c66 2e6e 5f61 746f 6d5f 696e  * self.n_atom_in
-000222f0: 7075 745f 6665 6174 5d29 2e74 7970 6528  put_feat]).type(
-00022300: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00022310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022320: 2020 2074 6f72 6368 2e66 6c6f 6174 3332     torch.float32
-00022330: 292c 2073 656c 662e 575f 4150 2920 2b20  ), self.W_AP) + 
-00022340: 7365 6c66 2e62 5f41 500a 2020 2020 2020  self.b_AP.      
-00022350: 2020 2020 2020 6966 2073 656c 662e 6261        if self.ba
-00022360: 7463 685f 6e6f 726d 616c 697a 653a 0a20  tch_normalize:. 
-00022370: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00022380: 656c 662e 4150 5f62 6e2e 6576 616c 2829  elf.AP_bn.eval()
-00022390: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000223a0: 2041 505f 6a69 203d 2073 656c 662e 4150   AP_ji = self.AP
-000223b0: 5f62 6e28 4150 5f6a 6929 0a20 2020 2020  _bn(AP_ji).     
-000223c0: 2020 2020 2020 2041 505f 6a69 203d 2061         AP_ji = a
-000223d0: 6374 6976 6174 696f 6e28 4150 5f6a 6929  ctivation(AP_ji)
-000223e0: 0a20 2020 2020 2020 2020 2020 2023 2050  .            # P
-000223f0: 5020 6973 2061 2074 656e 736f 7220 7769  P is a tensor wi
-00022400: 7468 2073 6861 7065 205b 746f 7461 6c20  th shape [total 
-00022410: 6e75 6d62 6572 206f 6620 7061 6972 732c  number of pairs,
-00022420: 6e5f 6869 6464 656e 5f50 505d 0a20 2020  n_hidden_PP].   
-00022430: 2020 2020 2020 2020 2050 503a 2074 6f72           PP: tor
-00022440: 6368 2e54 656e 736f 7220 3d20 746f 7263  ch.Tensor = torc
-00022450: 682e 6d61 746d 756c 2870 6169 725f 6665  h.matmul(pair_fe
-00022460: 6174 7572 6573 2e74 7970 6528 746f 7263  atures.type(torc
-00022470: 682e 666c 6f61 7433 3229 2c0a 2020 2020  h.float32),.    
-00022480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00022490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000224a0: 2020 2020 2020 2020 7365 6c66 2e57 5f50          self.W_P
-000224b0: 5029 202b 2073 656c 662e 625f 5050 0a20  P) + self.b_PP. 
-000224c0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-000224d0: 6c66 2e62 6174 6368 5f6e 6f72 6d61 6c69  lf.batch_normali
-000224e0: 7a65 3a0a 2020 2020 2020 2020 2020 2020  ze:.            
-000224f0: 2020 2020 7365 6c66 2e50 505f 626e 2e65      self.PP_bn.e
-00022500: 7661 6c28 290a 2020 2020 2020 2020 2020  val().          
-00022510: 2020 2020 2020 5050 203d 2073 656c 662e        PP = self.
-00022520: 5050 5f62 6e28 5050 290a 2020 2020 2020  PP_bn(PP).      
-00022530: 2020 2020 2020 5050 203d 2061 6374 6976        PP = activ
-00022540: 6174 696f 6e28 5050 290a 2020 2020 2020  ation(PP).      
-00022550: 2020 2020 2020 503a 2074 6f72 6368 2e54        P: torch.T
-00022560: 656e 736f 7220 3d20 746f 7263 682e 6d61  ensor = torch.ma
-00022570: 746d 756c 280a 2020 2020 2020 2020 2020  tmul(.          
-00022580: 2020 2020 2020 746f 7263 682e 636f 6e63        torch.conc
-00022590: 6174 285b 4150 5f69 6a20 2b20 4150 5f6a  at([AP_ij + AP_j
-000225a0: 692c 2050 505d 2c20 3129 2e74 7970 6528  i, PP], 1).type(
-000225b0: 746f 7263 682e 666c 6f61 7433 3229 2c0a  torch.float32),.
-000225c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000225d0: 7365 6c66 2e57 5f50 2920 2b20 7365 6c66  self.W_P) + self
-000225e0: 2e62 5f50 0a20 2020 2020 2020 2020 2020  .b_P.           
-000225f0: 2069 6620 7365 6c66 2e62 6174 6368 5f6e   if self.batch_n
-00022600: 6f72 6d61 6c69 7a65 3a0a 2020 2020 2020  ormalize:.      
-00022610: 2020 2020 2020 2020 2020 7365 6c66 2e50            self.P
-00022620: 5f62 6e2e 6576 616c 2829 0a20 2020 2020  _bn.eval().     
-00022630: 2020 2020 2020 2020 2020 2050 203d 2073             P = s
-00022640: 656c 662e 505f 626e 2850 290a 2020 2020  elf.P_bn(P).    
-00022650: 2020 2020 2020 2020 5020 3d20 6163 7469          P = acti
-00022660: 7661 7469 6f6e 2850 290a 2020 2020 2020  vation(P).      
-00022670: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00022680: 2020 2020 5020 3d20 7061 6972 5f66 6561      P = pair_fea
-00022690: 7475 7265 730a 0a20 2020 2020 2020 2072  tures..        r
-000226a0: 6574 7572 6e20 5b41 2c20 505d 0a         eturn [A, P].
+0001cf50: 0a0a 636c 6173 7320 4d6f 6c47 414e 436f  ..class MolGANCo
+0001cf60: 6e76 6f6c 7574 696f 6e4c 6179 6572 286e  nvolutionLayer(n
+0001cf70: 6e2e 4d6f 6475 6c65 293a 0a20 2020 2022  n.Module):.    "
+0001cf80: 2222 0a20 2020 2047 7261 7068 2063 6f6e  "".    Graph con
+0001cf90: 766f 6c75 7469 6f6e 206c 6179 6572 2075  volution layer u
+0001cfa0: 7365 6420 696e 204d 6f6c 4741 4e20 6d6f  sed in MolGAN mo
+0001cfb0: 6465 6c2e 0a20 2020 204d 6f6c 4741 4e20  del..    MolGAN 
+0001cfc0: 6973 2061 2057 4741 4e20 7479 7065 206d  is a WGAN type m
+0001cfd0: 6f64 656c 2066 6f72 2067 656e 6572 6174  odel for generat
+0001cfe0: 696f 6e20 6f66 2073 6d61 6c6c 206d 6f6c  ion of small mol
+0001cff0: 6563 756c 6573 2e0a 2020 2020 4e6f 7420  ecules..    Not 
+0001d000: 7573 6564 2064 6972 6563 746c 792c 2068  used directly, h
+0001d010: 6967 6865 7220 6c65 7665 6c20 6c61 7965  igher level laye
+0001d020: 7273 206c 696b 6520 4d6f 6c47 414e 4d75  rs like MolGANMu
+0001d030: 6c74 6943 6f6e 766f 6c75 7469 6f6e 4c61  ltiConvolutionLa
+0001d040: 7965 7220 7573 6520 6974 2e0a 2020 2020  yer use it..    
+0001d050: 5468 6973 206c 6179 6572 2070 6572 666f  This layer perfo
+0001d060: 726d 7320 6261 7369 6320 636f 6e76 6f6c  rms basic convol
+0001d070: 7574 696f 6e20 6f6e 206f 6e65 2d68 6f74  ution on one-hot
+0001d080: 2065 6e63 6f64 6564 206d 6174 7269 6365   encoded matrice
+0001d090: 7320 636f 6e74 6169 6e69 6e67 0a20 2020  s containing.   
+0001d0a0: 2061 746f 6d20 616e 6420 626f 6e64 2069   atom and bond i
+0001d0b0: 6e66 6f72 6d61 7469 6f6e 2e20 5468 6973  nformation. This
+0001d0c0: 206c 6179 6572 2061 6c73 6f20 6163 6365   layer also acce
+0001d0d0: 7074 7320 7468 7265 6520 696e 7075 7473  pts three inputs
+0001d0e0: 2066 6f72 2074 6865 2063 6173 650a 2020   for the case.  
+0001d0f0: 2020 7768 656e 2063 6f6e 766f 6c75 7469    when convoluti
+0001d100: 6f6e 2069 7320 7065 7266 6f72 6d65 6420  on is performed 
+0001d110: 6d6f 7265 2074 6861 6e20 6f6e 6365 2061  more than once a
+0001d120: 6e64 2072 6573 756c 7473 206f 6620 7072  nd results of pr
+0001d130: 6576 696f 7573 2063 6f6e 766f 6c75 7469  evious convoluti
+0001d140: 6f6e 0a20 2020 206e 6565 6420 746f 2075  on.    need to u
+0001d150: 7365 642e 2049 7420 7761 7320 646f 6e65  sed. It was done
+0001d160: 2069 6e20 7375 6368 2061 2077 6179 2074   in such a way t
+0001d170: 6f20 6176 6f69 6420 6372 6561 7469 6e67  o avoid creating
+0001d180: 2061 6e6f 7468 6572 206c 6179 6572 2074   another layer t
+0001d190: 6861 740a 2020 2020 6163 6365 7074 7320  hat.    accepts 
+0001d1a0: 7468 7265 6520 696e 7075 7473 2072 6174  three inputs rat
+0001d1b0: 6865 7220 7468 616e 2074 776f 2e20 5468  her than two. Th
+0001d1c0: 6520 6c61 7374 2069 6e70 7574 206c 6179  e last input lay
+0001d1d0: 6572 2069 7320 736f 2d63 616c 6c65 640a  er is so-called.
+0001d1e0: 2020 2020 6869 6464 656e 5f6c 6179 6572      hidden_layer
+0001d1f0: 2061 6e64 2069 7420 686f 6c64 2072 6573   and it hold res
+0001d200: 756c 7473 206f 6620 7468 6520 636f 6e76  ults of the conv
+0001d210: 6f6c 7574 696f 6e20 7768 696c 6520 6669  olution while fi
+0001d220: 7273 7420 7477 6f20 6172 6520 756e 6368  rst two are unch
+0001d230: 616e 6765 640a 2020 2020 696e 7075 7420  anged.    input 
+0001d240: 7465 6e73 6f72 732e 0a0a 2020 2020 4578  tensors...    Ex
+0001d250: 616d 706c 650a 2020 2020 2d2d 2d2d 2d2d  ample.    ------
+0001d260: 2d0a 2020 2020 5365 653a 204d 6f6c 4741  -.    See: MolGA
+0001d270: 4e4d 756c 7469 436f 6e76 6f6c 7574 696f  NMultiConvolutio
+0001d280: 6e4c 6179 6572 2066 6f72 2075 7369 6e67  nLayer for using
+0001d290: 2069 6e20 6c61 7965 7273 2e0a 0a20 2020   in layers...   
+0001d2a0: 203e 3e3e 2069 6d70 6f72 7420 746f 7263   >>> import torc
+0001d2b0: 680a 2020 2020 3e3e 3e20 696d 706f 7274  h.    >>> import
+0001d2c0: 2074 6f72 6368 2e6e 6e20 6173 206e 6e0a   torch.nn as nn.
+0001d2d0: 2020 2020 3e3e 3e20 696d 706f 7274 2074      >>> import t
+0001d2e0: 6f72 6368 2e6e 6e2e 6675 6e63 7469 6f6e  orch.nn.function
+0001d2f0: 616c 2061 7320 460a 2020 2020 3e3e 3e20  al as F.    >>> 
+0001d300: 7665 7274 6963 6573 203d 2039 0a20 2020  vertices = 9.   
+0001d310: 203e 3e3e 206e 6f64 6573 203d 2035 0a20   >>> nodes = 5. 
+0001d320: 2020 203e 3e3e 2065 6467 6573 203d 2035     >>> edges = 5
+0001d330: 0a20 2020 203e 3e3e 2075 6e69 7473 203d  .    >>> units =
+0001d340: 2031 3238 0a0a 2020 2020 3e3e 3e20 6c61   128..    >>> la
+0001d350: 7965 7231 203d 204d 6f6c 4741 4e43 6f6e  yer1 = MolGANCon
+0001d360: 766f 6c75 7469 6f6e 4c61 7965 7228 756e  volutionLayer(un
+0001d370: 6974 733d 756e 6974 732c 2065 6467 6573  its=units, edges
+0001d380: 3d65 6467 6573 2c20 6e6f 6465 733d 6e6f  =edges, nodes=no
+0001d390: 6465 732c 206e 616d 653d 276c 6179 6572  des, name='layer
+0001d3a0: 3127 290a 2020 2020 3e3e 3e20 6164 6a61  1').    >>> adja
+0001d3b0: 6365 6e63 795f 7465 6e73 6f72 203d 2074  cency_tensor = t
+0001d3c0: 6f72 6368 2e72 616e 646e 2828 312c 2076  orch.randn((1, v
+0001d3d0: 6572 7469 6365 732c 2076 6572 7469 6365  ertices, vertice
+0001d3e0: 732c 2065 6467 6573 2929 0a20 2020 203e  s, edges)).    >
+0001d3f0: 3e3e 206e 6f64 655f 7465 6e73 6f72 203d  >> node_tensor =
+0001d400: 2074 6f72 6368 2e72 616e 646e 2828 312c   torch.randn((1,
+0001d410: 2076 6572 7469 6365 732c 206e 6f64 6573   vertices, nodes
+0001d420: 2929 0a20 2020 203e 3e3e 206f 7574 7075  )).    >>> outpu
+0001d430: 7420 3d20 6c61 7965 7231 285b 6164 6a61  t = layer1([adja
+0001d440: 6365 6e63 795f 7465 6e73 6f72 2c20 6e6f  cency_tensor, no
+0001d450: 6465 5f74 656e 736f 725d 290a 0a20 2020  de_tensor])..   
+0001d460: 2052 6566 6572 656e 6365 730a 2020 2020   References.    
+0001d470: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 202e  ----------.    .
+0001d480: 2e20 5b31 5d20 4e69 636f 6c61 2044 6520  . [1] Nicola De 
+0001d490: 4361 6f20 6574 2061 6c2e 2022 4d6f 6c47  Cao et al. "MolG
+0001d4a0: 414e 3a20 416e 2069 6d70 6c69 6369 7420  AN: An implicit 
+0001d4b0: 6765 6e65 7261 7469 7665 206d 6f64 656c  generative model
+0001d4c0: 0a20 2020 2020 2020 2066 6f72 2073 6d61  .        for sma
+0001d4d0: 6c6c 206d 6f6c 6563 756c 6172 2067 7261  ll molecular gra
+0001d4e0: 7068 7322 2c20 6874 7470 733a 2f2f 6172  phs", https://ar
+0001d4f0: 7869 762e 6f72 672f 6162 732f 3138 3035  xiv.org/abs/1805
+0001d500: 2e31 3139 3733 0a20 2020 2022 2222 0a0a  .11973.    """..
+0001d510: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+0001d520: 2873 656c 662c 0a20 2020 2020 2020 2020  (self,.         
+0001d530: 2020 2020 2020 2020 756e 6974 733a 2069          units: i
+0001d540: 6e74 2c0a 2020 2020 2020 2020 2020 2020  nt,.            
+0001d550: 2020 2020 206e 6f64 6573 3a20 696e 742c       nodes: int,
+0001d560: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001d570: 2020 6163 7469 7661 7469 6f6e 3d46 2e74    activation=F.t
+0001d580: 616e 682c 0a20 2020 2020 2020 2020 2020  anh,.           
+0001d590: 2020 2020 2020 6472 6f70 6f75 745f 7261        dropout_ra
+0001d5a0: 7465 3a20 666c 6f61 7420 3d20 302e 302c  te: float = 0.0,
+0001d5b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001d5c0: 2020 6564 6765 733a 2069 6e74 203d 2035    edges: int = 5
+0001d5d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0001d5e0: 2020 206e 616d 653a 2073 7472 203d 2022     name: str = "
+0001d5f0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+0001d600: 2020 2020 2a2a 6b77 6172 6773 293a 0a20      **kwargs):. 
+0001d610: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0001d620: 2020 2049 6e69 7469 616c 697a 6520 7468     Initialize th
+0001d630: 6973 206c 6179 6572 2e0a 0a20 2020 2020  is layer...     
+0001d640: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+0001d650: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d0a        ---------.
+0001d660: 2020 2020 2020 2020 756e 6974 733a 2069          units: i
+0001d670: 6e74 0a20 2020 2020 2020 2020 2020 2044  nt.            D
+0001d680: 696d 6573 696f 6e20 6f66 2064 656e 7365  imesion of dense
+0001d690: 206c 6179 6572 7320 7573 6564 2066 6f72   layers used for
+0001d6a0: 2063 6f6e 766f 6c75 7469 6f6e 0a20 2020   convolution.   
+0001d6b0: 2020 2020 206e 6f64 6573 3a20 696e 740a       nodes: int.
+0001d6c0: 2020 2020 2020 2020 2020 2020 4e75 6d62              Numb
+0001d6d0: 6572 206f 6620 6665 6174 7572 6573 2069  er of features i
+0001d6e0: 6e20 6e6f 6465 2074 656e 736f 720a 2020  n node tensor.  
+0001d6f0: 2020 2020 2020 6163 7469 7661 7469 6f6e        activation
+0001d700: 3a20 6675 6e63 7469 6f6e 2c20 6f70 7469  : function, opti
+0001d710: 6f6e 616c 2028 6465 6661 756c 743d 5461  onal (default=Ta
+0001d720: 6e68 290a 2020 2020 2020 2020 2020 2020  nh).            
+0001d730: 6163 7469 7661 7469 6f6e 2066 756e 6374  activation funct
+0001d740: 696f 6e20 7573 6564 2061 6372 6f73 7320  ion used across 
+0001d750: 6d6f 6465 6c2c 2064 6566 6175 6c74 2069  model, default i
+0001d760: 7320 5461 6e68 0a20 2020 2020 2020 2064  s Tanh.        d
+0001d770: 726f 706f 7574 5f72 6174 653a 2066 6c6f  ropout_rate: flo
+0001d780: 6174 2c20 6f70 7469 6f6e 616c 2028 6465  at, optional (de
+0001d790: 6661 756c 743d 302e 3029 0a20 2020 2020  fault=0.0).     
+0001d7a0: 2020 2020 2020 2044 726f 706f 7574 2072         Dropout r
+0001d7b0: 6174 6520 7573 6564 2062 7920 6472 6f70  ate used by drop
+0001d7c0: 6f75 7420 6c61 7965 720a 2020 2020 2020  out layer.      
+0001d7d0: 2020 6564 6765 733a 2069 6e74 2c20 6f70    edges: int, op
+0001d7e0: 7469 6f6e 616c 2028 6465 6661 756c 743d  tional (default=
+0001d7f0: 3529 0a20 2020 2020 2020 2020 2020 2048  5).            H
+0001d800: 6f77 206d 616e 7920 6465 6e73 6520 6c61  ow many dense la
+0001d810: 7965 7273 2074 6f20 7573 6520 696e 2063  yers to use in c
+0001d820: 6f6e 766f 6c75 7469 6f6e 2e0a 2020 2020  onvolution..    
+0001d830: 2020 2020 2020 2020 5479 7069 6361 6c6c          Typicall
+0001d840: 7920 6571 7561 6c20 746f 206e 756d 6265  y equal to numbe
+0001d850: 7220 6f66 2062 6f6e 6420 7479 7065 7320  r of bond types 
+0001d860: 7573 6564 2069 6e20 7468 6520 6d6f 6465  used in the mode
+0001d870: 6c2e 0a20 2020 2020 2020 206e 616d 653a  l..        name:
+0001d880: 2073 7472 696e 672c 206f 7074 696f 6e61   string, optiona
+0001d890: 6c20 2864 6566 6175 6c74 3d22 2229 0a20  l (default=""). 
+0001d8a0: 2020 2020 2020 2020 2020 204e 616d 6520             Name 
+0001d8b0: 6f66 2074 6865 206c 6179 6572 0a20 2020  of the layer.   
+0001d8c0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0001d8d0: 2073 7570 6572 284d 6f6c 4741 4e43 6f6e   super(MolGANCon
+0001d8e0: 766f 6c75 7469 6f6e 4c61 7965 722c 2073  volutionLayer, s
+0001d8f0: 656c 6629 2e5f 5f69 6e69 745f 5f28 290a  elf).__init__().
+0001d900: 0a20 2020 2020 2020 2073 656c 662e 6163  .        self.ac
+0001d910: 7469 7661 7469 6f6e 203d 2061 6374 6976  tivation = activ
+0001d920: 6174 696f 6e0a 2020 2020 2020 2020 7365  ation.        se
+0001d930: 6c66 2e64 726f 706f 7574 5f72 6174 653a  lf.dropout_rate:
+0001d940: 2066 6c6f 6174 203d 2064 726f 706f 7574   float = dropout
+0001d950: 5f72 6174 650a 2020 2020 2020 2020 7365  _rate.        se
+0001d960: 6c66 2e75 6e69 7473 3a20 696e 7420 3d20  lf.units: int = 
+0001d970: 756e 6974 730a 2020 2020 2020 2020 7365  units.        se
+0001d980: 6c66 2e65 6467 6573 3a20 696e 7420 3d20  lf.edges: int = 
+0001d990: 6564 6765 730a 2020 2020 2020 2020 7365  edges.        se
+0001d9a0: 6c66 2e6e 616d 653a 2073 7472 203d 206e  lf.name: str = n
+0001d9b0: 616d 650a 2020 2020 2020 2020 7365 6c66  ame.        self
+0001d9c0: 2e6e 6f64 6573 3a20 696e 7420 3d20 6e6f  .nodes: int = no
+0001d9d0: 6465 730a 0a20 2020 2020 2020 2073 656c  des..        sel
+0001d9e0: 662e 6465 6e73 6531 3a20 6e6e 2e4d 6f64  f.dense1: nn.Mod
+0001d9f0: 756c 654c 6973 7420 3d20 6e6e 2e4d 6f64  uleList = nn.Mod
+0001da00: 756c 654c 6973 7428 0a20 2020 2020 2020  uleList(.       
+0001da10: 2020 2020 205b 6e6e 2e4c 696e 6561 7228       [nn.Linear(
+0001da20: 6e6f 6465 732c 2073 656c 662e 756e 6974  nodes, self.unit
+0001da30: 7329 2066 6f72 205f 2069 6e20 7261 6e67  s) for _ in rang
+0001da40: 6528 6564 6765 7320 2d20 3129 5d29 0a20  e(edges - 1)]). 
+0001da50: 2020 2020 2020 2073 656c 662e 6465 6e73         self.dens
+0001da60: 6532 3a20 6e6e 2e4c 696e 6561 7220 3d20  e2: nn.Linear = 
+0001da70: 6e6e 2e4c 696e 6561 7228 6e6f 6465 732c  nn.Linear(nodes,
+0001da80: 2073 656c 662e 756e 6974 7329 0a20 2020   self.units).   
+0001da90: 2020 2020 2073 656c 662e 6472 6f70 6f75       self.dropou
+0001daa0: 743a 206e 6e2e 4472 6f70 6f75 7420 3d20  t: nn.Dropout = 
+0001dab0: 6e6e 2e44 726f 706f 7574 2873 656c 662e  nn.Dropout(self.
+0001dac0: 6472 6f70 6f75 745f 7261 7465 290a 0a20  dropout_rate).. 
+0001dad0: 2020 2064 6566 205f 5f72 6570 725f 5f28     def __repr__(
+0001dae0: 7365 6c66 2920 2d3e 2073 7472 3a0a 2020  self) -> str:.  
+0001daf0: 2020 2020 2020 7265 7475 726e 2028 0a20        return (. 
+0001db00: 2020 2020 2020 2020 2020 2066 277b 7365             f'{se
+0001db10: 6c66 2e5f 5f63 6c61 7373 5f5f 2e5f 5f6e  lf.__class__.__n
+0001db20: 616d 655f 5f7d 2855 6e69 7473 3d7b 7365  ame__}(Units={se
+0001db30: 6c66 2e75 6e69 7473 7d2c 204e 6f64 6573  lf.units}, Nodes
+0001db40: 3d7b 7365 6c66 2e6e 6f64 6573 7d2c 2041  ={self.nodes}, A
+0001db50: 6374 6976 6174 696f 6e3d 7b73 656c 662e  ctivation={self.
+0001db60: 6163 7469 7661 7469 6f6e 7d2c 2044 726f  activation}, Dro
+0001db70: 706f 7574 5f72 6174 653d 7b73 656c 662e  pout_rate={self.
+0001db80: 6472 6f70 7574 5f72 6174 657d 2c20 4564  droput_rate}, Ed
+0001db90: 6765 733d 7b73 656c 662e 6564 6765 737d  ges={self.edges}
+0001dba0: 2c20 4e61 6d65 3d7b 7365 6c66 2e6e 616d  , Name={self.nam
+0001dbb0: 657d 2927 0a20 2020 2020 2020 2029 0a0a  e})'.        )..
+0001dbc0: 2020 2020 6465 6620 666f 7277 6172 6428      def forward(
+0001dbd0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0001dbe0: 662c 0a20 2020 2020 2020 2020 2020 2069  f,.            i
+0001dbf0: 6e70 7574 733a 204c 6973 7429 202d 3e20  nputs: List) -> 
+0001dc00: 5475 706c 655b 746f 7263 682e 5465 6e73  Tuple[torch.Tens
+0001dc10: 6f72 2c20 746f 7263 682e 5465 6e73 6f72  or, torch.Tensor
+0001dc20: 2c20 746f 7263 682e 5465 6e73 6f72 5d3a  , torch.Tensor]:
+0001dc30: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0001dc40: 2020 2020 2049 6e76 6f6b 6520 7468 6973       Invoke this
+0001dc50: 206c 6179 6572 0a0a 2020 2020 2020 2020   layer..        
+0001dc60: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
+0001dc70: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+0001dc80: 2020 2020 2020 696e 7075 7473 3a20 6c69        inputs: li
+0001dc90: 7374 0a20 2020 2020 2020 2020 2020 204c  st.            L
+0001dca0: 6973 7420 6f66 2074 776f 2069 6e70 7574  ist of two input
+0001dcb0: 206d 6174 7269 6365 732c 2061 646a 6163   matrices, adjac
+0001dcc0: 656e 6379 2074 656e 736f 7220 616e 6420  ency tensor and 
+0001dcd0: 6e6f 6465 2066 6561 7475 7265 7320 7465  node features te
+0001dce0: 6e73 6f72 730a 2020 2020 2020 2020 2020  nsors.          
+0001dcf0: 2020 696e 206f 6e65 2d68 6f74 2065 6e63    in one-hot enc
+0001dd00: 6f64 696e 6720 666f 726d 6174 2e0a 0a20  oding format... 
+0001dd10: 2020 2020 2020 2052 6574 7572 6e73 0a20         Returns. 
+0001dd20: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d0a         --------.
+0001dd30: 2020 2020 2020 2020 7475 706c 6528 746f          tuple(to
+0001dd40: 7263 682e 5465 6e73 6f72 2c74 6f72 6368  rch.Tensor,torch
+0001dd50: 2e54 656e 736f 722c 746f 7263 682e 5465  .Tensor,torch.Te
+0001dd60: 6e73 6f72 290a 2020 2020 2020 2020 2020  nsor).          
+0001dd70: 2020 4669 7273 7420 616e 6420 7365 636f    First and seco
+0001dd80: 6e64 2061 7265 206f 7269 6769 6e61 6c20  nd are original 
+0001dd90: 696e 7075 7420 7465 6e73 6f72 730a 2020  input tensors.  
+0001dda0: 2020 2020 2020 2020 2020 5468 6972 6420            Third 
+0001ddb0: 6973 2074 6865 2072 6573 756c 7420 6f66  is the result of
+0001ddc0: 2063 6f6e 766f 6c75 7469 6f6e 0a20 2020   convolution.   
+0001ddd0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0001dde0: 2069 633a 2069 6e74 203d 206c 656e 2869   ic: int = len(i
+0001ddf0: 6e70 7574 7329 0a20 2020 2020 2020 2069  nputs).        i
+0001de00: 6620 6963 203c 2032 3a0a 2020 2020 2020  f ic < 2:.      
+0001de10: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
+0001de20: 6545 7272 6f72 280a 2020 2020 2020 2020  eError(.        
+0001de30: 2020 2020 2020 2020 224d 6f6c 4741 4e43          "MolGANC
+0001de40: 6f6e 766f 6c75 7469 6f6e 4c61 7965 7220  onvolutionLayer 
+0001de50: 7265 7175 6972 6573 2061 7420 6c65 6173  requires at leas
+0001de60: 7420 7477 6f20 696e 7075 7473 3a20 5b61  t two inputs: [a
+0001de70: 646a 6163 656e 6379 5f74 656e 736f 722c  djacency_tensor,
+0001de80: 206e 6f64 655f 6665 6174 7572 6573 5f74   node_features_t
+0001de90: 656e 736f 725d 220a 2020 2020 2020 2020  ensor]".        
+0001dea0: 2020 2020 290a 0a20 2020 2020 2020 2061      )..        a
+0001deb0: 646a 6163 656e 6379 5f74 656e 736f 723a  djacency_tensor:
+0001dec0: 2074 6f72 6368 2e54 656e 736f 7220 3d20   torch.Tensor = 
+0001ded0: 696e 7075 7473 5b30 5d0a 2020 2020 2020  inputs[0].      
+0001dee0: 2020 6e6f 6465 5f74 656e 736f 723a 2074    node_tensor: t
+0001def0: 6f72 6368 2e54 656e 736f 7220 3d20 696e  orch.Tensor = in
+0001df00: 7075 7473 5b31 5d0a 0a20 2020 2020 2020  puts[1]..       
+0001df10: 2069 6620 6963 203e 2032 3a0a 2020 2020   if ic > 2:.    
+0001df20: 2020 2020 2020 2020 6869 6464 656e 5f74          hidden_t
+0001df30: 656e 736f 723a 2074 6f72 6368 2e54 656e  ensor: torch.Ten
+0001df40: 736f 7220 3d20 696e 7075 7473 5b32 5d0a  sor = inputs[2].
+0001df50: 2020 2020 2020 2020 2020 2020 616e 6e6f              anno
+0001df60: 7461 7469 6f6e 7320 3d20 746f 7263 682e  tations = torch.
+0001df70: 6361 7428 2868 6964 6465 6e5f 7465 6e73  cat((hidden_tens
+0001df80: 6f72 2c20 6e6f 6465 5f74 656e 736f 7229  or, node_tensor)
+0001df90: 2c20 2d31 290a 2020 2020 2020 2020 656c  , -1).        el
+0001dfa0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0001dfb0: 616e 6e6f 7461 7469 6f6e 7320 3d20 6e6f  annotations = no
+0001dfc0: 6465 5f74 656e 736f 720a 0a20 2020 2020  de_tensor..     
+0001dfd0: 2020 206f 7574 7075 745f 6465 6e73 653a     output_dense:
+0001dfe0: 2074 6f72 6368 2e54 656e 736f 7220 3d20   torch.Tensor = 
+0001dff0: 746f 7263 682e 7374 6163 6b28 0a20 2020  torch.stack(.   
+0001e000: 2020 2020 2020 2020 205b 6465 6e73 6528           [dense(
+0001e010: 616e 6e6f 7461 7469 6f6e 7329 2066 6f72  annotations) for
+0001e020: 2064 656e 7365 2069 6e20 7365 6c66 2e64   dense in self.d
+0001e030: 656e 7365 315d 2c20 3129 0a0a 2020 2020  ense1], 1)..    
+0001e040: 2020 2020 6164 6a3a 2074 6f72 6368 2e54      adj: torch.T
+0001e050: 656e 736f 7220 3d20 6164 6a61 6365 6e63  ensor = adjacenc
+0001e060: 795f 7465 6e73 6f72 2e70 6572 6d75 7465  y_tensor.permute
+0001e070: 2830 2c20 332c 2031 2c20 3229 5b3a 2c20  (0, 3, 1, 2)[:, 
+0001e080: 313a 2c20 3a2c 203a 5d0a 0a20 2020 2020  1:, :, :]..     
+0001e090: 2020 206f 7574 7075 745f 6d75 6c3a 2074     output_mul: t
+0001e0a0: 6f72 6368 2e54 656e 736f 7220 3d20 746f  orch.Tensor = to
+0001e0b0: 7263 682e 6d61 746d 756c 2861 646a 2c20  rch.matmul(adj, 
+0001e0c0: 6f75 7470 7574 5f64 656e 7365 290a 2020  output_dense).  
+0001e0d0: 2020 2020 2020 6f75 7470 7574 5f73 756d        output_sum
+0001e0e0: 3a20 746f 7263 682e 5465 6e73 6f72 203d  : torch.Tensor =
+0001e0f0: 2074 6f72 6368 2e73 756d 286f 7574 7075   torch.sum(outpu
+0001e100: 745f 6d75 6c2c 0a20 2020 2020 2020 2020  t_mul,.         
+0001e110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e130: 2020 2020 6469 6d3d 3129 202b 2073 656c      dim=1) + sel
+0001e140: 662e 6465 6e73 6532 286e 6f64 655f 7465  f.dense2(node_te
+0001e150: 6e73 6f72 290a 2020 2020 2020 2020 6f75  nsor).        ou
+0001e160: 7470 7574 5f61 6374 3a20 746f 7263 682e  tput_act: torch.
+0001e170: 5465 6e73 6f72 203d 2073 656c 662e 6163  Tensor = self.ac
+0001e180: 7469 7661 7469 6f6e 286f 7574 7075 745f  tivation(output_
+0001e190: 7375 6d29 0a20 2020 2020 2020 206f 7574  sum).        out
+0001e1a0: 7075 7420 3d20 7365 6c66 2e64 726f 706f  put = self.dropo
+0001e1b0: 7574 286f 7574 7075 745f 6163 7429 0a20  ut(output_act). 
+0001e1c0: 2020 2020 2020 2072 6574 7572 6e20 6164         return ad
+0001e1d0: 6a61 6365 6e63 795f 7465 6e73 6f72 2c20  jacency_tensor, 
+0001e1e0: 6e6f 6465 5f74 656e 736f 722c 206f 7574  node_tensor, out
+0001e1f0: 7075 740a 0a0a 636c 6173 7320 4454 4e4e  put...class DTNN
+0001e200: 5374 6570 286e 6e2e 4d6f 6475 6c65 293a  Step(nn.Module):
+0001e210: 0a20 2020 2022 2222 4454 4e4e 5374 6570  .    """DTNNStep
+0001e220: 204c 6179 6572 2066 6f72 2044 544e 4e20   Layer for DTNN 
+0001e230: 6d6f 6465 6c2e 0a0a 2020 2020 456e 636f  model...    Enco
+0001e240: 6465 7320 7468 6520 6174 6f6d 2773 2069  des the atom's i
+0001e250: 6e74 6572 6163 7469 6f6e 2077 6974 6820  nteraction with 
+0001e260: 6f74 6865 7220 6174 6f6d 7320 6163 636f  other atoms acco
+0001e270: 7264 696e 6720 746f 2064 6973 7461 6e63  rding to distanc
+0001e280: 6520 7265 6c61 7469 6f6e 7368 6970 732e  e relationships.
+0001e290: 205b 315d 5f0a 0a20 2020 2054 6869 7320   [1]_..    This 
+0001e2a0: 4c61 7965 7220 696d 706c 656d 656e 7473  Layer implements
+0001e2b0: 2074 6865 2045 7120 2837 2920 6672 6f6d   the Eq (7) from
+0001e2c0: 2044 544e 4e20 5061 7065 722e 2054 6865   DTNN Paper. The
+0001e2d0: 6e20 7375 6d73 2074 6865 6d20 7570 2074  n sums them up t
+0001e2e0: 6f20 6765 7420 7468 6520 6669 6e61 6c20  o get the final 
+0001e2f0: 6f75 7470 7574 2075 7369 6e67 2045 7120  output using Eq 
+0001e300: 2836 2920 6672 6f6d 2044 544e 4e20 5061  (6) from DTNN Pa
+0001e310: 7065 722e 0a0a 2020 2020 4571 2028 3729  per...    Eq (7)
+0001e320: 3a20 565f 696a 203d 2074 616e 685b 575f  : V_ij = tanh[W_
+0001e330: 6663 202e 2028 2857 5f63 6620 2e20 435f  fc . ((W_cf . C_
+0001e340: 6a20 2b20 625f 6366 2920 2a20 2857 5f64  j + b_cf) * (W_d
+0001e350: 6620 2e20 645f 696a 202b 2062 5f64 6629  f . d_ij + b_df)
+0001e360: 295d 0a0a 2020 2020 4571 2028 3629 3a20  )]..    Eq (6): 
+0001e370: 435f 6920 3d20 435f 6920 2b20 7375 6d28  C_i = C_i + sum(
+0001e380: 565f 696a 290a 0a20 2020 2048 6572 6520  V_ij)..    Here 
+0001e390: 3a20 272e 273d 4d61 7472 6978 204d 756c  : '.'=Matrix Mul
+0001e3a0: 7469 706c 6963 6174 696f 6e20 2c20 272a  tiplication , '*
+0001e3b0: 273d 4d75 6c74 6970 6c69 6361 7469 6f6e  '=Multiplication
+0001e3c0: 0a0a 2020 2020 5265 6665 7265 6e63 6573  ..    References
+0001e3d0: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
+0001e3e0: 2020 2020 5b31 5d20 5363 68c3 bc74 742c      [1] Sch..tt,
+0001e3f0: 204b 7269 7374 6f66 2054 2e2c 2065 7420   Kristof T., et 
+0001e400: 616c 2e20 2251 7561 6e74 756d 2d63 6865  al. "Quantum-che
+0001e410: 6d69 6361 6c20 696e 7369 6768 7473 2066  mical insights f
+0001e420: 726f 6d20 6465 6570 0a20 2020 2020 2020  rom deep.       
+0001e430: 2074 656e 736f 7220 6e65 7572 616c 206e   tensor neural n
+0001e440: 6574 776f 726b 732e 2220 4e61 7475 7265  etworks." Nature
+0001e450: 2063 6f6d 6d75 6e69 6361 7469 6f6e 7320   communications 
+0001e460: 382e 3120 2832 3031 3729 3a20 312d 382e  8.1 (2017): 1-8.
+0001e470: 0a0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
+0001e480: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
+0001e490: 2020 2020 6e5f 656d 6265 6464 696e 673a      n_embedding:
+0001e4a0: 2069 6e74 2c20 6f70 7469 6f6e 616c 0a20   int, optional. 
+0001e4b0: 2020 2020 2020 204e 756d 6265 7220 6f66         Number of
+0001e4c0: 2066 6561 7475 7265 7320 666f 7220 6561   features for ea
+0001e4d0: 6368 2061 746f 6d0a 2020 2020 6e5f 6469  ch atom.    n_di
+0001e4e0: 7374 616e 6365 3a20 696e 742c 206f 7074  stance: int, opt
+0001e4f0: 696f 6e61 6c0a 2020 2020 2020 2020 6772  ional.        gr
+0001e500: 616e 756c 6172 6974 7920 6f66 2064 6973  anularity of dis
+0001e510: 7461 6e63 6520 6d61 7472 6978 0a20 2020  tance matrix.   
+0001e520: 206e 5f68 6964 6465 6e3a 2069 6e74 2c20   n_hidden: int, 
+0001e530: 6f70 7469 6f6e 616c 0a20 2020 2020 2020  optional.       
+0001e540: 204e 756d 6265 7220 6f66 206e 6f64 6573   Number of nodes
+0001e550: 2069 6e20 6869 6464 656e 206c 6179 6572   in hidden layer
+0001e560: 0a20 2020 2069 6e69 7469 616c 697a 6572  .    initializer
+0001e570: 3a20 7374 722c 206f 7074 696f 6e61 6c0a  : str, optional.
+0001e580: 2020 2020 2020 2020 5765 6967 6874 2069          Weight i
+0001e590: 6e69 7469 616c 697a 6174 696f 6e20 666f  nitialization fo
+0001e5a0: 7220 6669 6c74 6572 732e 0a20 2020 2020  r filters..     
+0001e5b0: 2020 204f 7074 696f 6e73 3a20 7b78 6176     Options: {xav
+0001e5c0: 6965 725f 756e 6966 6f72 6d5f 2c20 7861  ier_uniform_, xa
+0001e5d0: 7669 6572 5f6e 6f72 6d61 6c5f 2c20 6b61  vier_normal_, ka
+0001e5e0: 696d 696e 675f 756e 6966 6f72 6d5f 2c20  iming_uniform_, 
+0001e5f0: 6b61 696d 696e 675f 6e6f 726d 616c 5f2c  kaiming_normal_,
+0001e600: 2074 7275 6e63 5f6e 6f72 6d61 6c5f 7d0a   trunc_normal_}.
+0001e610: 2020 2020 6163 7469 7661 7469 6f6e 3a20      activation: 
+0001e620: 7374 722c 206f 7074 696f 6e61 6c0a 2020  str, optional.  
+0001e630: 2020 2020 2020 4163 7469 7661 7469 6f6e        Activation
+0001e640: 2066 756e 6374 696f 6e20 6170 706c 6965   function applie
+0001e650: 640a 0a20 2020 2045 7861 6d70 6c65 730a  d..    Examples.
+0001e660: 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020      --------.   
+0001e670: 203e 3e3e 2066 726f 6d20 6465 6570 6368   >>> from deepch
+0001e680: 656d 2e6d 6f64 656c 732e 746f 7263 685f  em.models.torch_
+0001e690: 6d6f 6465 6c73 2069 6d70 6f72 7420 6c61  models import la
+0001e6a0: 7965 7273 0a20 2020 203e 3e3e 2069 6d70  yers.    >>> imp
+0001e6b0: 6f72 7420 746f 7263 680a 2020 2020 3e3e  ort torch.    >>
+0001e6c0: 3e20 656d 6265 6464 696e 675f 6c61 7965  > embedding_laye
+0001e6d0: 7220 3d20 6c61 7965 7273 2e44 544e 4e45  r = layers.DTNNE
+0001e6e0: 6d62 6564 6469 6e67 2834 2c20 3429 0a20  mbedding(4, 4). 
+0001e6f0: 2020 203e 3e3e 2065 6d62 203d 2065 6d62     >>> emb = emb
+0001e700: 6564 6469 6e67 5f6c 6179 6572 2874 6f72  edding_layer(tor
+0001e710: 6368 2e54 656e 736f 7228 5b30 2c31 2c32  ch.Tensor([0,1,2
+0001e720: 2c33 5d29 2e74 6f28 746f 7263 682e 696e  ,3]).to(torch.in
+0001e730: 7436 3429 290a 2020 2020 3e3e 3e20 7374  t64)).    >>> st
+0001e740: 6570 5f6c 6179 6572 203d 206c 6179 6572  ep_layer = layer
+0001e750: 732e 4454 4e4e 5374 6570 2834 2c20 362c  s.DTNNStep(4, 6,
+0001e760: 2038 290a 2020 2020 3e3e 3e20 6f75 7470   8).    >>> outp
+0001e770: 7574 5f74 6f72 6368 203d 2073 7465 705f  ut_torch = step_
+0001e780: 6c61 7965 7228 5b0a 2020 2020 2e2e 2e20  layer([.    ... 
+0001e790: 2020 2020 746f 7263 682e 5465 6e73 6f72      torch.Tensor
+0001e7a0: 2865 6d62 292c 0a20 2020 202e 2e2e 2020  (emb),.    ...  
+0001e7b0: 2020 2074 6f72 6368 2e54 656e 736f 7228     torch.Tensor(
+0001e7c0: 5b30 2c20 312c 2032 2c20 332c 2034 2c20  [0, 1, 2, 3, 4, 
+0001e7d0: 355d 292e 746f 2874 6f72 6368 2e66 6c6f  5]).to(torch.flo
+0001e7e0: 6174 3332 292c 0a20 2020 202e 2e2e 2020  at32),.    ...  
+0001e7f0: 2020 2074 6f72 6368 2e54 656e 736f 7228     torch.Tensor(
+0001e800: 5b31 5d29 2e74 6f28 746f 7263 682e 696e  [1]).to(torch.in
+0001e810: 7436 3429 2c0a 2020 2020 2e2e 2e20 2020  t64),.    ...   
+0001e820: 2020 746f 7263 682e 5465 6e73 6f72 285b    torch.Tensor([
+0001e830: 5b31 5d5d 292e 746f 2874 6f72 6368 2e69  [1]]).to(torch.i
+0001e840: 6e74 3634 290a 2020 2020 2e2e 2e20 5d29  nt64).    ... ])
+0001e850: 0a20 2020 203e 3e3e 206f 7574 7075 745f  .    >>> output_
+0001e860: 746f 7263 682e 7368 6170 650a 2020 2020  torch.shape.    
+0001e870: 746f 7263 682e 5369 7a65 285b 322c 2034  torch.Size([2, 4
+0001e880: 2c20 345d 290a 0a20 2020 2022 2222 0a0a  , 4])..    """..
+0001e890: 2020 2020 6465 6620 5f5f 696e 6974 5f5f      def __init__
+0001e8a0: 2873 656c 662c 0a20 2020 2020 2020 2020  (self,.         
+0001e8b0: 2020 2020 2020 2020 6e5f 656d 6265 6464          n_embedd
+0001e8c0: 696e 673a 2069 6e74 203d 2033 302c 0a20  ing: int = 30,. 
+0001e8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e8e0: 6e5f 6469 7374 616e 6365 3a20 696e 7420  n_distance: int 
+0001e8f0: 3d20 3130 302c 0a20 2020 2020 2020 2020  = 100,.         
+0001e900: 2020 2020 2020 2020 6e5f 6869 6464 656e          n_hidden
+0001e910: 3a20 696e 7420 3d20 3630 2c0a 2020 2020  : int = 60,.    
+0001e920: 2020 2020 2020 2020 2020 2020 2069 6e69               ini
+0001e930: 7469 616c 697a 6572 3a20 7374 7220 3d20  tializer: str = 
+0001e940: 2778 6176 6965 725f 756e 6966 6f72 6d5f  'xavier_uniform_
+0001e950: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
+0001e960: 2020 2020 6163 7469 7661 7469 6f6e 3d27      activation='
+0001e970: 7461 6e68 272c 0a20 2020 2020 2020 2020  tanh',.         
+0001e980: 2020 2020 2020 2020 2a2a 6b77 6172 6773          **kwargs
+0001e990: 293a 0a0a 2020 2020 2020 2020 7375 7065  ):..        supe
+0001e9a0: 7228 4454 4e4e 5374 6570 2c20 7365 6c66  r(DTNNStep, self
+0001e9b0: 292e 5f5f 696e 6974 5f5f 282a 2a6b 7761  ).__init__(**kwa
+0001e9c0: 7267 7329 0a20 2020 2020 2020 2073 656c  rgs).        sel
+0001e9d0: 662e 6e5f 656d 6265 6464 696e 6720 3d20  f.n_embedding = 
+0001e9e0: 6e5f 656d 6265 6464 696e 670a 2020 2020  n_embedding.    
+0001e9f0: 2020 2020 7365 6c66 2e6e 5f64 6973 7461      self.n_dista
+0001ea00: 6e63 6520 3d20 6e5f 6469 7374 616e 6365  nce = n_distance
+0001ea10: 0a20 2020 2020 2020 2073 656c 662e 6e5f  .        self.n_
+0001ea20: 6869 6464 656e 203d 206e 5f68 6964 6465  hidden = n_hidde
+0001ea30: 6e0a 2020 2020 2020 2020 7365 6c66 2e69  n.        self.i
+0001ea40: 6e69 7469 616c 697a 6572 203d 2069 6e69  nitializer = ini
+0001ea50: 7469 616c 697a 6572 2020 2320 5365 7420  tializer  # Set 
+0001ea60: 7765 6967 6874 2069 6e69 7469 616c 697a  weight initializ
+0001ea70: 6174 696f 6e0a 2020 2020 2020 2020 7365  ation.        se
+0001ea80: 6c66 2e61 6374 6976 6174 696f 6e20 3d20  lf.activation = 
+0001ea90: 6163 7469 7661 7469 6f6e 2020 2320 4765  activation  # Ge
+0001eaa0: 7420 6163 7469 7661 7469 6f6e 730a 2020  t activations.  
+0001eab0: 2020 2020 2020 7365 6c66 2e61 6374 6976        self.activ
+0001eac0: 6174 696f 6e5f 666e 203d 2067 6574 5f61  ation_fn = get_a
+0001ead0: 6374 6976 6174 696f 6e28 7365 6c66 2e61  ctivation(self.a
+0001eae0: 6374 6976 6174 696f 6e29 0a0a 2020 2020  ctivation)..    
+0001eaf0: 2020 2020 696e 6974 5f66 756e 633a 2043      init_func: C
+0001eb00: 616c 6c61 626c 6520 3d20 6765 7461 7474  allable = getatt
+0001eb10: 7228 696e 6974 6961 6c69 7a65 7273 2c20  r(initializers, 
+0001eb20: 7365 6c66 2e69 6e69 7469 616c 697a 6572  self.initializer
+0001eb30: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+0001eb40: 575f 6366 203d 2069 6e69 745f 6675 6e63  W_cf = init_func
+0001eb50: 2874 6f72 6368 2e65 6d70 7479 285b 7365  (torch.empty([se
+0001eb60: 6c66 2e6e 5f65 6d62 6564 6469 6e67 2c20  lf.n_embedding, 
+0001eb70: 7365 6c66 2e6e 5f68 6964 6465 6e5d 2929  self.n_hidden]))
+0001eb80: 0a20 2020 2020 2020 2073 656c 662e 575f  .        self.W_
+0001eb90: 6466 203d 2069 6e69 745f 6675 6e63 2874  df = init_func(t
+0001eba0: 6f72 6368 2e65 6d70 7479 285b 7365 6c66  orch.empty([self
+0001ebb0: 2e6e 5f64 6973 7461 6e63 652c 2073 656c  .n_distance, sel
+0001ebc0: 662e 6e5f 6869 6464 656e 5d29 290a 2020  f.n_hidden])).  
+0001ebd0: 2020 2020 2020 7365 6c66 2e57 5f66 6320        self.W_fc 
+0001ebe0: 3d20 696e 6974 5f66 756e 6328 746f 7263  = init_func(torc
+0001ebf0: 682e 656d 7074 7928 5b73 656c 662e 6e5f  h.empty([self.n_
+0001ec00: 6869 6464 656e 2c20 7365 6c66 2e6e 5f65  hidden, self.n_e
+0001ec10: 6d62 6564 6469 6e67 5d29 290a 2020 2020  mbedding])).    
+0001ec20: 2020 2020 7365 6c66 2e62 5f63 6620 3d20      self.b_cf = 
+0001ec30: 746f 7263 682e 7a65 726f 7328 7369 7a65  torch.zeros(size
+0001ec40: 3d5b 0a20 2020 2020 2020 2020 2020 2073  =[.            s
+0001ec50: 656c 662e 6e5f 6869 6464 656e 2c0a 2020  elf.n_hidden,.  
+0001ec60: 2020 2020 2020 5d29 0a20 2020 2020 2020        ]).       
+0001ec70: 2073 656c 662e 625f 6466 203d 2074 6f72   self.b_df = tor
+0001ec80: 6368 2e7a 6572 6f73 2873 697a 653d 5b0a  ch.zeros(size=[.
+0001ec90: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0001eca0: 2e6e 5f68 6964 6465 6e2c 0a20 2020 2020  .n_hidden,.     
+0001ecb0: 2020 205d 290a 0a20 2020 2064 6566 205f     ])..    def _
+0001ecc0: 5f72 6570 725f 5f28 7365 6c66 293a 0a20  _repr__(self):. 
+0001ecd0: 2020 2020 2020 2022 2222 5265 7475 726e         """Return
+0001ece0: 7320 6120 7374 7269 6e67 2072 6570 7265  s a string repre
+0001ecf0: 7365 6e74 696e 6720 7468 6520 636f 6e66  senting the conf
+0001ed00: 6967 7572 6174 696f 6e20 6f66 2074 6865  iguration of the
+0001ed10: 206c 6179 6572 2e0a 0a20 2020 2020 2020   layer...       
+0001ed20: 2052 6574 7572 6e73 0a20 2020 2020 2020   Returns.       
+0001ed30: 202d 2d2d 2d2d 2d2d 0a20 2020 2020 2020   -------.       
+0001ed40: 206e 5f65 6d62 6564 6469 6e67 3a20 696e   n_embedding: in
+0001ed50: 742c 206f 7074 696f 6e61 6c0a 2020 2020  t, optional.    
+0001ed60: 2020 2020 2020 2020 4e75 6d62 6572 206f          Number o
+0001ed70: 6620 6665 6174 7572 6573 2066 6f72 2065  f features for e
+0001ed80: 6163 6820 6174 6f6d 0a20 2020 2020 2020  ach atom.       
+0001ed90: 206e 5f64 6973 7461 6e63 653a 2069 6e74   n_distance: int
+0001eda0: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
+0001edb0: 2020 2020 2020 2067 7261 6e75 6c61 7269         granulari
+0001edc0: 7479 206f 6620 6469 7374 616e 6365 206d  ty of distance m
+0001edd0: 6174 7269 780a 2020 2020 2020 2020 6e5f  atrix.        n_
+0001ede0: 6869 6464 656e 3a20 696e 742c 206f 7074  hidden: int, opt
+0001edf0: 696f 6e61 6c0a 2020 2020 2020 2020 2020  ional.          
+0001ee00: 2020 4e75 6d62 6572 206f 6620 6e6f 6465    Number of node
+0001ee10: 7320 696e 2068 6964 6465 6e20 6c61 7965  s in hidden laye
+0001ee20: 720a 2020 2020 2020 2020 696e 6974 6961  r.        initia
+0001ee30: 6c69 7a65 723a 2073 7472 2c20 6f70 7469  lizer: str, opti
+0001ee40: 6f6e 616c 0a20 2020 2020 2020 2020 2020  onal.           
+0001ee50: 2057 6569 6768 7420 696e 6974 6961 6c69   Weight initiali
+0001ee60: 7a61 7469 6f6e 2066 6f72 2066 696c 7465  zation for filte
+0001ee70: 7273 2e0a 2020 2020 2020 2020 2020 2020  rs..            
+0001ee80: 4f70 7469 6f6e 733a 207b 7861 7669 6572  Options: {xavier
+0001ee90: 5f75 6e69 666f 726d 5f2c 2078 6176 6965  _uniform_, xavie
+0001eea0: 725f 6e6f 726d 616c 5f2c 206b 6169 6d69  r_normal_, kaimi
+0001eeb0: 6e67 5f75 6e69 666f 726d 5f2c 206b 6169  ng_uniform_, kai
+0001eec0: 6d69 6e67 5f6e 6f72 6d61 6c5f 2c20 7472  ming_normal_, tr
+0001eed0: 756e 635f 6e6f 726d 616c 5f7d 0a20 2020  unc_normal_}.   
+0001eee0: 2020 2020 2061 6374 6976 6174 696f 6e3a       activation:
+0001eef0: 2073 7472 2c20 6f70 7469 6f6e 616c 0a20   str, optional. 
+0001ef00: 2020 2020 2020 2020 2020 2041 6374 6976             Activ
+0001ef10: 6174 696f 6e20 6675 6e63 7469 6f6e 2061  ation function a
+0001ef20: 7070 6c69 6564 0a0a 2020 2020 2020 2020  pplied..        
+0001ef30: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
+0001ef40: 726e 2066 277b 7365 6c66 2e5f 5f63 6c61  rn f'{self.__cla
+0001ef50: 7373 5f5f 2e5f 5f6e 616d 655f 5f7d 286e  ss__.__name__}(n
+0001ef60: 5f65 6d62 6564 6469 6e67 3d7b 7365 6c66  _embedding={self
+0001ef70: 2e6e 5f65 6d62 6564 6469 6e67 7d2c 206e  .n_embedding}, n
+0001ef80: 5f64 6973 7461 6e63 653d 7b73 656c 662e  _distance={self.
+0001ef90: 6e5f 6469 7374 616e 6365 7d2c 206e 5f68  n_distance}, n_h
+0001efa0: 6964 6465 6e3d 7b73 656c 662e 6e5f 6869  idden={self.n_hi
+0001efb0: 6464 656e 7d2c 2069 6e69 7469 616c 697a  dden}, initializ
+0001efc0: 6572 3d7b 7365 6c66 2e69 6e69 7469 616c  er={self.initial
+0001efd0: 697a 6572 7d2c 2061 6374 6976 6174 696f  izer}, activatio
+0001efe0: 6e3d 7b73 656c 662e 6163 7469 7661 7469  n={self.activati
+0001eff0: 6f6e 7d29 270a 0a20 2020 2064 6566 2066  on})'..    def f
+0001f000: 6f72 7761 7264 2873 656c 662c 2069 6e70  orward(self, inp
+0001f010: 7574 7329 3a0a 2020 2020 2020 2020 2222  uts):.        ""
+0001f020: 2245 7865 6375 7465 7320 7468 6520 6571  "Executes the eq
+0001f030: 7561 7469 6f6e 7320 616e 6420 5265 7475  uations and Retu
+0001f040: 726e 7320 7468 6520 696e 7472 6163 7469  rns the intracti
+0001f050: 6f6e 2076 6563 746f 7220 6f66 2074 6865  on vector of the
+0001f060: 2061 746f 6d20 7769 7468 206f 7468 6572   atom with other
+0001f070: 2061 746f 6d73 2e0a 0a20 2020 2020 2020   atoms...       
+0001f080: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
+0001f090: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+0001f0a0: 2020 2020 2020 2069 6e70 7574 733a 2074         inputs: t
+0001f0b0: 6f72 6368 2e54 656e 736f 720a 2020 2020  orch.Tensor.    
+0001f0c0: 2020 2020 2020 2020 4c69 7374 206f 6620          List of 
+0001f0d0: 5465 6e73 6f72 7320 6861 7669 6e67 2061  Tensors having a
+0001f0e0: 746f 6d5f 6665 6174 7572 6573 2c20 6469  tom_features, di
+0001f0f0: 7374 616e 6365 2c20 6469 7374 616e 6365  stance, distance
+0001f100: 5f6d 656d 6265 7273 6869 705f 692c 2064  _membership_i, d
+0001f110: 6973 7461 6e63 655f 6d65 6d62 6572 7368  istance_membersh
+0001f120: 6970 5f6a 2e0a 0a20 2020 2020 2020 2052  ip_j...        R
+0001f130: 6574 7572 6e73 0a20 2020 2020 2020 202d  eturns.        -
+0001f140: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2069  ------.        i
+0001f150: 6e74 6572 6163 7469 6f6e 5f76 6563 746f  nteraction_vecto
+0001f160: 723a 2074 6f72 6368 2e54 656e 736f 720a  r: torch.Tensor.
+0001f170: 2020 2020 2020 2020 2020 2020 696e 7465              inte
+0001f180: 7261 6374 696f 6e20 6f66 2074 6865 2061  raction of the a
+0001f190: 746f 6d20 7769 7468 206f 7468 6572 2061  tom with other a
+0001f1a0: 746f 6d73 2062 6173 6564 206f 6e20 6469  toms based on di
+0001f1b0: 7374 616e 6365 2061 6e64 2064 6973 7461  stance and dista
+0001f1c0: 6e63 655f 6d65 6d62 6572 7368 6970 2e0a  nce_membership..
+0001f1d0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0001f1e0: 2020 2020 2061 746f 6d5f 6665 6174 7572       atom_featur
+0001f1f0: 6573 203d 2069 6e70 7574 735b 305d 0a20  es = inputs[0]. 
+0001f200: 2020 2020 2020 2064 6973 7461 6e63 6520         distance 
+0001f210: 3d20 696e 7075 7473 5b31 5d0a 2020 2020  = inputs[1].    
+0001f220: 2020 2020 6469 7374 616e 6365 5f6d 656d      distance_mem
+0001f230: 6265 7273 6869 705f 6920 3d20 696e 7075  bership_i = inpu
+0001f240: 7473 5b32 5d0a 2020 2020 2020 2020 6469  ts[2].        di
+0001f250: 7374 616e 6365 5f6d 656d 6265 7273 6869  stance_membershi
+0001f260: 705f 6a20 3d20 696e 7075 7473 5b33 5d0a  p_j = inputs[3].
+0001f270: 2020 2020 2020 2020 6469 7374 616e 6365          distance
+0001f280: 5f68 6964 6465 6e20 3d20 746f 7263 682e  _hidden = torch.
+0001f290: 6d61 746d 756c 2864 6973 7461 6e63 652c  matmul(distance,
+0001f2a0: 2073 656c 662e 575f 6466 2920 2b20 7365   self.W_df) + se
+0001f2b0: 6c66 2e62 5f64 660a 2020 2020 2020 2020  lf.b_df.        
+0001f2c0: 6174 6f6d 5f66 6561 7475 7265 735f 6869  atom_features_hi
+0001f2d0: 6464 656e 203d 2074 6f72 6368 2e6d 6174  dden = torch.mat
+0001f2e0: 6d75 6c28 6174 6f6d 5f66 6561 7475 7265  mul(atom_feature
+0001f2f0: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
+0001f300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f310: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0001f320: 656c 662e 575f 6366 2920 2b20 7365 6c66  elf.W_cf) + self
+0001f330: 2e62 5f63 660a 2020 2020 2020 2020 6f75  .b_cf.        ou
+0001f340: 7470 7574 7320 3d20 746f 7263 682e 6d75  tputs = torch.mu
+0001f350: 6c28 0a20 2020 2020 2020 2020 2020 2064  l(.            d
+0001f360: 6973 7461 6e63 655f 6869 6464 656e 2c0a  istance_hidden,.
+0001f370: 2020 2020 2020 2020 2020 2020 746f 7263              torc
+0001f380: 682e 656d 6265 6464 696e 6728 6174 6f6d  h.embedding(atom
+0001f390: 5f66 6561 7475 7265 735f 6869 6464 656e  _features_hidden
+0001f3a0: 2c20 6469 7374 616e 6365 5f6d 656d 6265  , distance_membe
+0001f3b0: 7273 6869 705f 6a29 290a 0a20 2020 2020  rship_j))..     
+0001f3c0: 2020 2023 2066 6f72 2061 746f 6d20 6920     # for atom i 
+0001f3d0: 696e 2061 206d 6f6c 6563 756c 6520 6d2c  in a molecule m,
+0001f3e0: 2074 6869 7320 7374 6570 206d 756c 7469   this step multi
+0001f3f0: 706c 6965 7320 746f 6765 7468 6572 2064  plies together d
+0001f400: 6973 7461 6e63 6520 696e 666f 206f 6620  istance info of 
+0001f410: 6174 6f6d 2070 6169 7228 692c 6a29 0a20  atom pair(i,j). 
+0001f420: 2020 2020 2020 2023 2061 6e64 2065 6d62         # and emb
+0001f430: 6564 6469 6e67 7320 6f66 2061 746f 6d20  eddings of atom 
+0001f440: 6a28 626f 7468 2067 6f6e 6520 7468 726f  j(both gone thro
+0001f450: 7567 6820 6120 6869 6464 656e 206c 6179  ugh a hidden lay
+0001f460: 6572 290a 2020 2020 2020 2020 6f75 7470  er).        outp
+0001f470: 7574 7320 3d20 746f 7263 682e 6d61 746d  uts = torch.matm
+0001f480: 756c 286f 7574 7075 7473 2c20 7365 6c66  ul(outputs, self
+0001f490: 2e57 5f66 6329 0a20 2020 2020 2020 206f  .W_fc).        o
+0001f4a0: 7574 7075 7473 203d 2073 656c 662e 6163  utputs = self.ac
+0001f4b0: 7469 7661 7469 6f6e 5f66 6e28 6f75 7470  tivation_fn(outp
+0001f4c0: 7574 7329 0a0a 2020 2020 2020 2020 6f75  uts)..        ou
+0001f4d0: 7470 7574 5f69 6920 3d20 746f 7263 682e  tput_ii = torch.
+0001f4e0: 6d75 6c28 7365 6c66 2e62 5f64 662c 2061  mul(self.b_df, a
+0001f4f0: 746f 6d5f 6665 6174 7572 6573 5f68 6964  tom_features_hid
+0001f500: 6465 6e29 0a20 2020 2020 2020 206f 7574  den).        out
+0001f510: 7075 745f 6969 203d 2074 6f72 6368 2e6d  put_ii = torch.m
+0001f520: 6174 6d75 6c28 6f75 7470 7574 5f69 692c  atmul(output_ii,
+0001f530: 2073 656c 662e 575f 6663 290a 2020 2020   self.W_fc).    
+0001f540: 2020 2020 6f75 7470 7574 5f69 6920 3d20      output_ii = 
+0001f550: 7365 6c66 2e61 6374 6976 6174 696f 6e5f  self.activation_
+0001f560: 666e 286f 7574 7075 745f 6969 290a 0a20  fn(output_ii).. 
+0001f570: 2020 2020 2020 2023 2066 6f72 2061 746f         # for ato
+0001f580: 6d20 692c 2073 756d 2074 6865 2069 6e66  m i, sum the inf
+0001f590: 6c75 656e 6365 2066 726f 6d20 616c 6c20  luence from all 
+0001f5a0: 6f74 6865 7220 6174 6f6d 206a 2069 6e20  other atom j in 
+0001f5b0: 7468 6520 6d6f 6c65 6375 6c65 0a20 2020  the molecule.   
+0001f5c0: 2020 2020 2069 6e74 7261 6374 696f 6e5f       intraction_
+0001f5d0: 7665 6374 6f72 203d 2073 6361 7474 6572  vector = scatter
+0001f5e0: 286f 7574 7075 7473 2c20 6469 7374 616e  (outputs, distan
+0001f5f0: 6365 5f6d 656d 6265 7273 6869 705f 692c  ce_membership_i,
+0001f600: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001f610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f620: 2020 2020 2064 696d 3d30 2920 2d20 6f75       dim=0) - ou
+0001f630: 7470 7574 5f69 6920 2b20 6174 6f6d 5f66  tput_ii + atom_f
+0001f640: 6561 7475 7265 730a 2020 2020 2020 2020  eatures.        
+0001f650: 7265 7475 726e 2069 6e74 7261 6374 696f  return intractio
+0001f660: 6e5f 7665 6374 6f72 0a0a 0a63 6c61 7373  n_vector...class
+0001f670: 2045 6467 654e 6574 776f 726b 286e 6e2e   EdgeNetwork(nn.
+0001f680: 4d6f 6475 6c65 293a 0a20 2020 2022 2222  Module):.    """
+0001f690: 5468 6520 4564 6765 4e65 7477 6f72 6b20  The EdgeNetwork 
+0001f6a0: 6d6f 6475 6c65 2069 7320 6120 5079 546f  module is a PyTo
+0001f6b0: 7263 6820 7375 626d 6f64 756c 6520 6465  rch submodule de
+0001f6c0: 7369 676e 6564 2066 6f72 206d 6573 7361  signed for messa
+0001f6d0: 6765 2070 6173 7369 6e67 2069 6e20 6772  ge passing in gr
+0001f6e0: 6170 6820 6e65 7572 616c 206e 6574 776f  aph neural netwo
+0001f6f0: 726b 732e 0a0a 2020 2020 4578 616d 706c  rks...    Exampl
+0001f700: 6573 0a20 2020 202d 2d2d 2d2d 2d2d 2d0a  es.    --------.
+0001f710: 2020 2020 3e3e 3e20 7061 6972 5f66 6561      >>> pair_fea
+0001f720: 7475 7265 7320 3d20 746f 7263 682e 7261  tures = torch.ra
+0001f730: 6e64 2828 342c 2032 292c 2064 7479 7065  nd((4, 2), dtype
+0001f740: 3d74 6f72 6368 2e66 6c6f 6174 3332 290a  =torch.float32).
+0001f750: 2020 2020 3e3e 3e20 6174 6f6d 5f66 6561      >>> atom_fea
+0001f760: 7475 7265 7320 3d20 746f 7263 682e 7261  tures = torch.ra
+0001f770: 6e64 2828 352c 2032 292c 2064 7479 7065  nd((5, 2), dtype
+0001f780: 3d74 6f72 6368 2e66 6c6f 6174 3332 290a  =torch.float32).
+0001f790: 2020 2020 3e3e 3e20 6174 6f6d 5f74 6f5f      >>> atom_to_
+0001f7a0: 7061 6972 203d 205b 5d0a 2020 2020 3e3e  pair = [].    >>
+0001f7b0: 3e20 6e5f 6174 6f6d 7320 3d20 320a 2020  > n_atoms = 2.  
+0001f7c0: 2020 3e3e 3e20 7374 6172 7420 3d20 300a    >>> start = 0.
+0001f7d0: 2020 2020 3e3e 3e20 4330 2c20 4331 203d      >>> C0, C1 =
+0001f7e0: 206e 702e 6d65 7368 6772 6964 286e 702e   np.meshgrid(np.
+0001f7f0: 6172 616e 6765 286e 5f61 746f 6d73 292c  arange(n_atoms),
+0001f800: 206e 702e 6172 616e 6765 286e 5f61 746f   np.arange(n_ato
+0001f810: 6d73 2929 0a20 2020 203e 3e3e 2061 746f  ms)).    >>> ato
+0001f820: 6d5f 746f 5f70 6169 722e 6170 7065 6e64  m_to_pair.append
+0001f830: 286e 702e 7472 616e 7370 6f73 6528 6e70  (np.transpose(np
+0001f840: 2e61 7272 6179 285b 4331 2e66 6c61 7474  .array([C1.flatt
+0001f850: 656e 2829 202b 2073 7461 7274 2c20 4330  en() + start, C0
+0001f860: 2e66 6c61 7474 656e 2829 202b 2073 7461  .flatten() + sta
+0001f870: 7274 5d29 2929 0a20 2020 203e 3e3e 2061  rt]))).    >>> a
+0001f880: 746f 6d5f 746f 5f70 6169 7220 3d20 746f  tom_to_pair = to
+0001f890: 7263 682e 5465 6e73 6f72 2861 746f 6d5f  rch.Tensor(atom_
+0001f8a0: 746f 5f70 6169 7229 0a20 2020 203e 3e3e  to_pair).    >>>
+0001f8b0: 2061 746f 6d5f 746f 5f70 6169 7220 3d20   atom_to_pair = 
+0001f8c0: 746f 7263 682e 7371 7565 657a 6528 6174  torch.squeeze(at
+0001f8d0: 6f6d 5f74 6f5f 7061 6972 2e74 6f28 746f  om_to_pair.to(to
+0001f8e0: 7263 682e 696e 7436 3429 2c20 6469 6d3d  rch.int64), dim=
+0001f8f0: 3029 0a20 2020 203e 3e3e 2069 6e70 7574  0).    >>> input
+0001f900: 7320 3d20 5b70 6169 725f 6665 6174 7572  s = [pair_featur
+0001f910: 6573 2c20 6174 6f6d 5f66 6561 7475 7265  es, atom_feature
+0001f920: 732c 2061 746f 6d5f 746f 5f70 6169 725d  s, atom_to_pair]
+0001f930: 0a20 2020 203e 3e3e 206e 5f70 6169 725f  .    >>> n_pair_
+0001f940: 6665 6174 7572 6573 203d 2032 0a20 2020  features = 2.   
+0001f950: 203e 3e3e 206e 5f68 6964 6465 6e20 3d20   >>> n_hidden = 
+0001f960: 320a 2020 2020 3e3e 3e20 696e 6974 203d  2.    >>> init =
+0001f970: 2027 7861 7669 6572 5f75 6e69 666f 726d   'xavier_uniform
+0001f980: 5f27 0a20 2020 203e 3e3e 206c 6179 6572  _'.    >>> layer
+0001f990: 203d 2045 6467 654e 6574 776f 726b 286e   = EdgeNetwork(n
+0001f9a0: 5f70 6169 725f 6665 6174 7572 6573 2c20  _pair_features, 
+0001f9b0: 6e5f 6869 6464 656e 2c20 696e 6974 290a  n_hidden, init).
+0001f9c0: 2020 2020 3e3e 3e20 7265 7375 6c74 203d      >>> result =
+0001f9d0: 206c 6179 6572 2869 6e70 7574 7329 0a20   layer(inputs). 
+0001f9e0: 2020 203e 3e3e 2072 6573 756c 742e 7368     >>> result.sh
+0001f9f0: 6170 655b 315d 0a20 2020 2032 0a20 2020  ape[1].    2.   
+0001fa00: 2022 2222 0a0a 2020 2020 6465 6620 5f5f   """..    def __
+0001fa10: 696e 6974 5f5f 2873 656c 662c 0a20 2020  init__(self,.   
+0001fa20: 2020 2020 2020 2020 2020 2020 2020 6e5f                n_
+0001fa30: 7061 6972 5f66 6561 7475 7265 733a 2069  pair_features: i
+0001fa40: 6e74 203d 2038 2c0a 2020 2020 2020 2020  nt = 8,.        
+0001fa50: 2020 2020 2020 2020 206e 5f68 6964 6465           n_hidde
+0001fa60: 6e3a 2069 6e74 203d 2031 3030 2c0a 2020  n: int = 100,.  
+0001fa70: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0001fa80: 6e69 743a 2073 7472 203d 2027 7861 7669  nit: str = 'xavi
+0001fa90: 6572 5f75 6e69 666f 726d 5f27 2c0a 2020  er_uniform_',.  
+0001faa0: 2020 2020 2020 2020 2020 2020 2020 202a                 *
+0001fab0: 2a6b 7761 7267 7329 3a0a 2020 2020 2020  *kwargs):.      
+0001fac0: 2020 2222 2249 6e69 7461 6c69 7365 7320    """Initalises 
+0001fad0: 6120 4564 6765 4e65 7477 6f72 6b20 4c61  a EdgeNetwork La
+0001fae0: 7965 720a 0a20 2020 2020 2020 2050 6172  yer..        Par
+0001faf0: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
+0001fb00: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
+0001fb10: 2020 206e 5f70 6169 725f 6665 6174 7572     n_pair_featur
+0001fb20: 6573 3a20 696e 742c 206f 7074 696f 6e61  es: int, optiona
+0001fb30: 6c0a 2020 2020 2020 2020 2020 2020 5468  l.            Th
+0001fb40: 6520 6c65 6e67 7468 206f 6620 7468 6520  e length of the 
+0001fb50: 7061 6972 2066 6561 7475 7265 7320 7665  pair features ve
+0001fb60: 6374 6f72 2e0a 2020 2020 2020 2020 6e5f  ctor..        n_
+0001fb70: 6869 6464 656e 3a20 696e 742c 206f 7074  hidden: int, opt
+0001fb80: 696f 6e61 6c0a 2020 2020 2020 2020 2020  ional.          
+0001fb90: 2020 6e75 6d62 6572 206f 6620 6869 6464    number of hidd
+0001fba0: 656e 2075 6e69 7473 2069 6e20 7468 6520  en units in the 
+0001fbb0: 7061 7373 696e 6720 7068 6173 650a 2020  passing phase.  
+0001fbc0: 2020 2020 2020 696e 6974 3a20 7374 722c        init: str,
+0001fbd0: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
+0001fbe0: 2020 2020 2020 496e 6974 6961 6c69 7a61        Initializa
+0001fbf0: 7469 6f6e 2066 756e 6374 696f 6e20 746f  tion function to
+0001fc00: 2062 6520 7573 6564 2069 6e20 7468 6520   be used in the 
+0001fc10: 6d65 7373 6167 6520 7061 7373 696e 6720  message passing 
+0001fc20: 6c61 7965 722e 0a20 2020 2020 2020 2022  layer..        "
+0001fc30: 2222 0a0a 2020 2020 2020 2020 7375 7065  ""..        supe
+0001fc40: 7228 4564 6765 4e65 7477 6f72 6b2c 2073  r(EdgeNetwork, s
+0001fc50: 656c 6629 2e5f 5f69 6e69 745f 5f28 2a2a  elf).__init__(**
+0001fc60: 6b77 6172 6773 290a 2020 2020 2020 2020  kwargs).        
+0001fc70: 7365 6c66 2e6e 5f70 6169 725f 6665 6174  self.n_pair_feat
+0001fc80: 7572 6573 3a20 696e 7420 3d20 6e5f 7061  ures: int = n_pa
+0001fc90: 6972 5f66 6561 7475 7265 730a 2020 2020  ir_features.    
+0001fca0: 2020 2020 7365 6c66 2e6e 5f68 6964 6465      self.n_hidde
+0001fcb0: 6e3a 2069 6e74 203d 206e 5f68 6964 6465  n: int = n_hidde
+0001fcc0: 6e0a 2020 2020 2020 2020 7365 6c66 2e69  n.        self.i
+0001fcd0: 6e69 743a 2073 7472 203d 2069 6e69 740a  nit: str = init.
+0001fce0: 0a20 2020 2020 2020 2069 6e69 745f 6675  .        init_fu
+0001fcf0: 6e63 3a20 4361 6c6c 6162 6c65 203d 2067  nc: Callable = g
+0001fd00: 6574 6174 7472 2869 6e69 7469 616c 697a  etattr(initializ
+0001fd10: 6572 732c 2073 656c 662e 696e 6974 290a  ers, self.init).
+0001fd20: 2020 2020 2020 2020 7365 6c66 2e57 3a20          self.W: 
+0001fd30: 746f 7263 682e 5465 6e73 6f72 203d 2069  torch.Tensor = i
+0001fd40: 6e69 745f 6675 6e63 280a 2020 2020 2020  nit_func(.      
+0001fd50: 2020 2020 2020 746f 7263 682e 656d 7074        torch.empt
+0001fd60: 7928 5b73 656c 662e 6e5f 7061 6972 5f66  y([self.n_pair_f
+0001fd70: 6561 7475 7265 732c 2073 656c 662e 6e5f  eatures, self.n_
+0001fd80: 6869 6464 656e 202a 2073 656c 662e 6e5f  hidden * self.n_
+0001fd90: 6869 6464 656e 5d29 290a 2020 2020 2020  hidden])).      
+0001fda0: 2020 7365 6c66 2e62 3a20 746f 7263 682e    self.b: torch.
+0001fdb0: 5465 6e73 6f72 203d 2074 6f72 6368 2e7a  Tensor = torch.z
+0001fdc0: 6572 6f73 2828 7365 6c66 2e6e 5f68 6964  eros((self.n_hid
+0001fdd0: 6465 6e20 2a20 7365 6c66 2e6e 5f68 6964  den * self.n_hid
+0001fde0: 6465 6e2c 2929 0a20 2020 2020 2020 2073  den,)).        s
+0001fdf0: 656c 662e 6275 696c 743a 2062 6f6f 6c20  elf.built: bool 
+0001fe00: 3d20 5472 7565 0a0a 2020 2020 6465 6620  = True..    def 
+0001fe10: 5f5f 7265 7072 5f5f 2873 656c 6629 202d  __repr__(self) -
+0001fe20: 3e20 7374 723a 0a20 2020 2020 2020 2072  > str:.        r
+0001fe30: 6574 7572 6e20 280a 2020 2020 2020 2020  eturn (.        
+0001fe40: 2020 2020 6627 7b73 656c 662e 5f5f 636c      f'{self.__cl
+0001fe50: 6173 735f 5f2e 5f5f 6e61 6d65 5f5f 7d28  ass__.__name__}(
+0001fe60: 6e5f 7061 6972 5f66 6561 7475 7265 733a  n_pair_features:
+0001fe70: 7b73 656c 662e 6e5f 7061 6972 5f66 6561  {self.n_pair_fea
+0001fe80: 7475 7265 737d 2c6e 5f68 6964 6465 6e3a  tures},n_hidden:
+0001fe90: 7b73 656c 662e 6e5f 6869 6464 656e 7d2c  {self.n_hidden},
+0001fea0: 696e 6974 3a7b 7365 6c66 2e69 6e69 747d  init:{self.init}
+0001feb0: 2927 0a20 2020 2020 2020 2029 0a0a 2020  )'.        )..  
+0001fec0: 2020 6465 6620 666f 7277 6172 6428 7365    def forward(se
+0001fed0: 6c66 2c20 696e 7075 7473 3a20 4c69 7374  lf, inputs: List
+0001fee0: 5b74 6f72 6368 2e54 656e 736f 725d 2920  [torch.Tensor]) 
+0001fef0: 2d3e 2074 6f72 6368 2e54 656e 736f 723a  -> torch.Tensor:
+0001ff00: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0001ff10: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
+0001ff20: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
+0001ff30: 2d2d 0a20 2020 2020 2020 2069 6e70 7574  --.        input
+0001ff40: 733a 204c 6973 745b 746f 7263 682e 5465  s: List[torch.Te
+0001ff50: 6e73 6f72 5d0a 2020 2020 2020 2020 2020  nsor].          
+0001ff60: 2020 5468 6520 6c65 6e67 7468 206f 6620    The length of 
+0001ff70: 6174 6f6d 5f74 6f5f 7061 6972 2073 686f  atom_to_pair sho
+0001ff80: 756c 6420 6265 2073 616d 6520 6173 206e  uld be same as n
+0001ff90: 5f70 6169 725f 6665 6174 7572 6573 2e0a  _pair_features..
+0001ffa0: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
+0001ffb0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
+0001ffc0: 2020 2020 2020 2020 7265 7375 6c74 3a20          result: 
+0001ffd0: 746f 7263 682e 5465 6e73 6f72 0a20 2020  torch.Tensor.   
+0001ffe0: 2020 2020 2020 2020 2054 656e 736f 7220           Tensor 
+0001fff0: 636f 6e74 6169 6e69 6e67 2074 6865 206d  containing the m
+00020000: 6170 7069 6e67 206f 6620 7468 6520 6564  apping of the ed
+00020010: 6765 2076 6563 746f 7220 746f 2061 2064  ge vector to a d
+00020020: 20c3 9720 6420 6d61 7472 6978 2c20 7768   .. d matrix, wh
+00020030: 6572 6520 6420 6465 6e6f 7465 7320 7468  ere d denotes th
+00020040: 6520 6469 6d65 6e73 696f 6e20 6f66 2074  e dimension of t
+00020050: 6865 2069 6e74 6572 6e61 6c20 6869 6464  he internal hidd
+00020060: 656e 2072 6570 7265 7365 6e74 6174 696f  en representatio
+00020070: 6e20 6f66 2065 6163 6820 6e6f 6465 2069  n of each node i
+00020080: 6e20 7468 6520 6772 6170 682e 0a20 2020  n the graph..   
+00020090: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000200a0: 2070 6169 725f 6665 6174 7572 6573 3a20   pair_features: 
+000200b0: 746f 7263 682e 5465 6e73 6f72 0a20 2020  torch.Tensor.   
+000200c0: 2020 2020 2061 746f 6d5f 6665 6174 7572       atom_featur
+000200d0: 6573 3a20 746f 7263 682e 5465 6e73 6f72  es: torch.Tensor
+000200e0: 0a20 2020 2020 2020 2061 746f 6d5f 746f  .        atom_to
+000200f0: 5f70 6169 723a 2074 6f72 6368 2e54 656e  _pair: torch.Ten
+00020100: 736f 720a 2020 2020 2020 2020 7061 6972  sor.        pair
+00020110: 5f66 6561 7475 7265 732c 2061 746f 6d5f  _features, atom_
+00020120: 6665 6174 7572 6573 2c20 6174 6f6d 5f74  features, atom_t
+00020130: 6f5f 7061 6972 203d 2069 6e70 7574 730a  o_pair = inputs.
+00020140: 0a20 2020 2020 2020 2041 3a20 746f 7263  .        A: torc
+00020150: 682e 5465 6e73 6f72 203d 2074 6f72 6368  h.Tensor = torch
+00020160: 2e61 6464 2874 6f72 6368 2e6d 6174 6d75  .add(torch.matmu
+00020170: 6c28 7061 6972 5f66 6561 7475 7265 732c  l(pair_features,
+00020180: 2073 656c 662e 5729 2c20 7365 6c66 2e62   self.W), self.b
+00020190: 290a 2020 2020 2020 2020 4120 3d20 746f  ).        A = to
+000201a0: 7263 682e 7265 7368 6170 6528 412c 2028  rch.reshape(A, (
+000201b0: 2d31 2c20 7365 6c66 2e6e 5f68 6964 6465  -1, self.n_hidde
+000201c0: 6e2c 2073 656c 662e 6e5f 6869 6464 656e  n, self.n_hidden
+000201d0: 2929 0a20 2020 2020 2020 206f 7574 3a20  )).        out: 
+000201e0: 746f 7263 682e 5465 6e73 6f72 203d 2074  torch.Tensor = t
+000201f0: 6f72 6368 2e75 6e73 7175 6565 7a65 2861  orch.unsqueeze(a
+00020200: 746f 6d5f 6665 6174 7572 6573 5b61 746f  tom_features[ato
+00020210: 6d5f 746f 5f70 6169 725b 3a2c 2031 5d5d  m_to_pair[:, 1]]
+00020220: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00020230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020240: 2020 2020 2020 2020 2020 2020 2020 6469                di
+00020250: 6d3d 3229 0a20 2020 2020 2020 206f 7574  m=2).        out
+00020260: 5f73 7175 6565 7a65 3a20 746f 7263 682e  _squeeze: torch.
+00020270: 5465 6e73 6f72 203d 2074 6f72 6368 2e73  Tensor = torch.s
+00020280: 7175 6565 7a65 2874 6f72 6368 2e6d 6174  queeze(torch.mat
+00020290: 6d75 6c28 412c 206f 7574 292c 2064 696d  mul(A, out), dim
+000202a0: 3d32 290a 2020 2020 2020 2020 696e 643a  =2).        ind:
+000202b0: 2074 6f72 6368 2e54 656e 736f 7220 3d20   torch.Tensor = 
+000202c0: 6174 6f6d 5f74 6f5f 7061 6972 5b3a 2c20  atom_to_pair[:, 
+000202d0: 305d 0a0a 2020 2020 2020 2020 7265 7375  0]..        resu
+000202e0: 6c74 3a20 746f 7263 682e 5465 6e73 6f72  lt: torch.Tensor
+000202f0: 203d 2073 6567 6d65 6e74 5f73 756d 286f   = segment_sum(o
+00020300: 7574 5f73 7175 6565 7a65 2c20 696e 6429  ut_squeeze, ind)
+00020310: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00020320: 2072 6573 756c 740a 0a0a 636c 6173 7320   result...class 
+00020330: 5765 6176 654c 6179 6572 286e 6e2e 4d6f  WeaveLayer(nn.Mo
+00020340: 6475 6c65 293a 0a20 2020 2022 2222 5468  dule):.    """Th
+00020350: 6973 2063 6c61 7373 2069 6d70 6c65 6d65  is class impleme
+00020360: 6e74 7320 7468 6520 636f 7265 2057 6561  nts the core Wea
+00020370: 7665 2063 6f6e 766f 6c75 7469 6f6e 2066  ve convolution f
+00020380: 726f 6d20 7468 6520 476f 6f67 6c65 2067  rom the Google g
+00020390: 7261 7068 2063 6f6e 766f 6c75 7469 6f6e  raph convolution
+000203a0: 2070 6170 6572 205b 315d 5f0a 2020 5468   paper [1]_.  Th
+000203b0: 6973 2069 7320 7468 6520 546f 7263 6820  is is the Torch 
+000203c0: 6571 7569 7661 6c65 6e74 206f 6620 7468  equivalent of th
+000203d0: 6520 6f72 6967 696e 616c 2069 6d70 6c65  e original imple
+000203e0: 6d65 6e74 6174 696f 6e20 7573 696e 6720  mentation using 
+000203f0: 4b65 7261 732e 0a0a 2020 5468 6973 206d  Keras...  This m
+00020400: 6f64 656c 2063 6f6e 7461 696e 7320 6174  odel contains at
+00020410: 6f6d 2066 6561 7475 7265 7320 616e 6420  om features and 
+00020420: 626f 6e64 2066 6561 7475 7265 730a 2020  bond features.  
+00020430: 7365 7061 7261 7465 6c79 2e48 6572 652c  separately.Here,
+00020440: 2062 6f6e 6420 6665 6174 7572 6573 2061   bond features a
+00020450: 7265 2061 6c73 6f20 6361 6c6c 6564 2070  re also called p
+00020460: 6169 7220 6665 6174 7572 6573 2e0a 2020  air features..  
+00020470: 5468 6572 6520 6172 6520 3220 7479 7065  There are 2 type
+00020480: 7320 6f66 2074 7261 6e73 666f 726d 6174  s of transformat
+00020490: 696f 6e2c 2061 746f 6d2d 3e61 746f 6d2c  ion, atom->atom,
+000204a0: 2061 746f 6d2d 3e70 6169 722c 2070 6169   atom->pair, pai
+000204b0: 722d 3e61 746f 6d2c 2070 6169 722d 3e70  r->atom, pair->p
+000204c0: 6169 7220 7468 6174 2074 6869 7320 6d6f  air that this mo
+000204d0: 6465 6c20 696d 706c 656d 656e 7473 2e0a  del implements..
+000204e0: 0a20 2045 7861 6d70 6c65 730a 2020 2d2d  .  Examples.  --
+000204f0: 2d2d 2d2d 2d2d 0a20 2054 6869 7320 6c61  ------.  This la
+00020500: 7965 7220 6578 7065 6374 7320 3420 696e  yer expects 4 in
+00020510: 7075 7473 2069 6e20 6120 6c69 7374 206f  puts in a list o
+00020520: 6620 7468 6520 666f 726d 2060 5b61 746f  f the form `[ato
+00020530: 6d5f 6665 6174 7572 6573 2c0a 2020 7061  m_features,.  pa
+00020540: 6972 5f66 6561 7475 7265 732c 2070 6169  ir_features, pai
+00020550: 725f 7370 6c69 742c 2061 746f 6d5f 746f  r_split, atom_to
+00020560: 5f70 6169 725d 602e 2057 6527 6c6c 2077  _pair]`. We'll w
+00020570: 616c 6b20 7468 726f 7567 6820 7468 6520  alk through the 
+00020580: 7374 7275 6374 7572 6520 6f66 2074 6865  structure of the
+00020590: 7365 2069 6e70 7574 732e 204c 6574 2773  se inputs. Let's
+000205a0: 2073 7461 7274 2077 6974 6820 736f 6d65   start with some
+000205b0: 2062 6173 6963 2064 6566 696e 6974 696f   basic definitio
+000205c0: 6e73 2e0a 2020 3e3e 3e20 696d 706f 7274  ns..  >>> import
+000205d0: 2064 6565 7063 6865 6d20 6173 2064 630a   deepchem as dc.
+000205e0: 2020 3e3e 3e20 696d 706f 7274 206e 756d    >>> import num
+000205f0: 7079 2061 7320 6e70 0a20 203e 3e3e 2073  py as np.  >>> s
+00020600: 6d69 6c65 7320 3d20 5b22 4343 4322 2c20  miles = ["CCC", 
+00020610: 2243 225d 0a0a 2020 4e6f 7465 2074 6861  "C"]..  Note tha
+00020620: 7420 7468 6572 6520 6172 6520 3420 6174  t there are 4 at
+00020630: 6f6d 7320 696e 2074 6f74 616c 2069 6e20  oms in total in 
+00020640: 7468 6973 2073 7973 7465 6d2e 2054 6869  this system. Thi
+00020650: 7320 6c61 7965 7220 6578 7065 6374 7320  s layer expects 
+00020660: 6974 7320 696e 7075 7420 6d6f 6c65 6375  its input molecu
+00020670: 6c65 7320 746f 2062 6520 6261 7463 6865  les to be batche
+00020680: 6420 746f 6765 7468 6572 2e0a 0a20 203e  d together...  >
+00020690: 3e3e 2074 6f74 616c 5f6e 5f61 746f 6d73  >> total_n_atoms
+000206a0: 203d 2034 0a0a 2020 4c65 7427 7320 7375   = 4..  Let's su
+000206b0: 7070 6f73 6520 7468 6174 2077 6520 6861  ppose that we ha
+000206c0: 7665 2061 2066 6561 7475 7269 7a65 7220  ve a featurizer 
+000206d0: 7468 6174 2063 6f6d 7075 7465 7320 606e  that computes `n
+000206e0: 5f61 746f 6d5f 6665 6174 6020 6665 6174  _atom_feat` feat
+000206f0: 7572 6573 2070 6572 2061 746f 6d2e 0a0a  ures per atom...
+00020700: 2020 3e3e 3e20 6e5f 6174 6f6d 5f66 6561    >>> n_atom_fea
+00020710: 7420 3d20 3735 0a0a 2020 5468 656e 2063  t = 75..  Then c
+00020720: 6f6e 6365 7074 7561 6c6c 792c 2060 6174  onceptually, `at
+00020730: 6f6d 5f66 6561 7460 2069 7320 7468 6520  om_feat` is the 
+00020740: 6172 7261 7920 6f66 2073 6861 7065 2060  array of shape `
+00020750: 2874 6f74 616c 5f6e 5f61 746f 6d73 2c0a  (total_n_atoms,.
+00020760: 2020 6e5f 6174 6f6d 5f66 6561 7429 6020    n_atom_feat)` 
+00020770: 6f66 2061 746f 6d69 6320 6665 6174 7572  of atomic featur
+00020780: 6573 2e20 466f 7220 7369 6d70 6c69 6369  es. For simplici
+00020790: 7479 2c20 6c65 7427 7320 6a75 7374 2067  ty, let's just g
+000207a0: 6f20 7769 7468 2061 0a20 2072 616e 646f  o with a.  rando
+000207b0: 6d20 7375 6368 206d 6174 7269 782e 0a0a  m such matrix...
+000207c0: 2020 3e3e 3e20 6174 6f6d 5f66 6561 7420    >>> atom_feat 
+000207d0: 3d20 6e70 2e72 616e 646f 6d2e 7261 6e64  = np.random.rand
+000207e0: 2874 6f74 616c 5f6e 5f61 746f 6d73 2c20  (total_n_atoms, 
+000207f0: 6e5f 6174 6f6d 5f66 6561 7429 0a0a 2020  n_atom_feat)..  
+00020800: 4c65 7427 7320 7375 7070 6f73 6520 7765  Let's suppose we
+00020810: 2068 6176 6520 606e 5f70 6169 725f 6665   have `n_pair_fe
+00020820: 6174 6020 7061 6972 7769 7365 2066 6561  at` pairwise fea
+00020830: 7475 7265 730a 0a20 203e 3e3e 206e 5f70  tures..  >>> n_p
+00020840: 6169 725f 6665 6174 203d 2031 340a 0a20  air_feat = 14.. 
+00020850: 2046 6f72 2065 6163 6820 6d6f 6c65 6375   For each molecu
+00020860: 6c65 2c20 7765 2063 6f6d 7075 7465 2061  le, we compute a
+00020870: 206d 6174 7269 7820 6f66 2073 6861 7065   matrix of shape
+00020880: 2060 286e 5f61 746f 6d73 2a6e 5f61 746f   `(n_atoms*n_ato
+00020890: 6d73 2c0a 2020 6e5f 7061 6972 5f66 6561  ms,.  n_pair_fea
+000208a0: 7429 6020 6f66 2070 6169 7277 6973 6520  t)` of pairwise 
+000208b0: 6665 6174 7572 6573 2066 6f72 2065 6163  features for eac
+000208c0: 6820 7061 6972 206f 6620 6174 6f6d 7320  h pair of atoms 
+000208d0: 696e 2074 6865 206d 6f6c 6563 756c 652e  in the molecule.
+000208e0: 0a20 204c 6574 2773 2063 6f6e 7374 7275  .  Let's constru
+000208f0: 6374 2074 6869 7320 636f 6e63 6570 7475  ct this conceptu
+00020900: 616c 6c79 2066 6f72 206f 7572 2065 7861  ally for our exa
+00020910: 6d70 6c65 2e0a 0a20 203e 3e3e 2070 6169  mple...  >>> pai
+00020920: 725f 6665 6174 203d 205b 6e70 2e72 616e  r_feat = [np.ran
+00020930: 646f 6d2e 7261 6e64 2833 2a33 2c20 6e5f  dom.rand(3*3, n_
+00020940: 7061 6972 5f66 6561 7429 2c20 6e70 2e72  pair_feat), np.r
+00020950: 616e 646f 6d2e 7261 6e64 2831 2a31 2c6e  andom.rand(1*1,n
+00020960: 5f70 6169 725f 6665 6174 295d 0a20 203e  _pair_feat)].  >
+00020970: 3e3e 2070 6169 725f 6665 6174 203d 206e  >> pair_feat = n
+00020980: 702e 636f 6e63 6174 656e 6174 6528 7061  p.concatenate(pa
+00020990: 6972 5f66 6561 742c 2061 7869 733d 3029  ir_feat, axis=0)
+000209a0: 0a20 203e 3e3e 2070 6169 725f 6665 6174  .  >>> pair_feat
+000209b0: 2e73 6861 7065 0a20 2028 3130 2c20 3134  .shape.  (10, 14
+000209c0: 290a 0a20 2060 7061 6972 5f73 706c 6974  )..  `pair_split
+000209d0: 6020 6973 2061 6e20 696e 6465 7820 696e  ` is an index in
+000209e0: 746f 2060 7061 6972 5f66 6561 7460 2077  to `pair_feat` w
+000209f0: 6869 6368 2074 656c 6c73 2075 7320 7768  hich tells us wh
+00020a00: 6963 6820 6174 6f6d 2065 6163 6820 726f  ich atom each ro
+00020a10: 7720 6265 6c6f 6e67 7320 746f 2e20 496e  w belongs to. In
+00020a20: 206f 7572 2063 6173 652c 2077 6520 6876   our case, we hv
+00020a30: 650a 0a20 203e 3e3e 2070 6169 725f 7370  e..  >>> pair_sp
+00020a40: 6c69 7420 3d20 6e70 2e61 7272 6179 285b  lit = np.array([
+00020a50: 302c 2030 2c20 302c 2031 2c20 312c 2031  0, 0, 0, 1, 1, 1
+00020a60: 2c20 322c 2032 2c20 322c 2033 5d29 0a0a  , 2, 2, 2, 3])..
+00020a70: 2020 5468 6174 2069 732c 2074 6865 2066    That is, the f
+00020a80: 6972 7374 2039 2065 6e74 7269 6573 2062  irst 9 entries b
+00020a90: 656c 6f6e 6720 746f 2022 4343 4322 2061  elong to "CCC" a
+00020aa0: 6e64 2074 6865 206c 6173 7420 656e 7472  nd the last entr
+00020ab0: 7920 746f 2022 4322 2e20 5468 650a 2020  y to "C". The.  
+00020ac0: 6669 6e61 6c20 656e 7472 7920 6061 746f  final entry `ato
+00020ad0: 6d5f 746f 5f70 6169 7260 2067 6f65 7320  m_to_pair` goes 
+00020ae0: 696e 2061 206c 6974 746c 6520 6d6f 7265  in a little more
+00020af0: 2069 6e2d 6465 7074 6820 7468 616e 2060   in-depth than `
+00020b00: 7061 6972 5f73 706c 6974 600a 2020 616e  pair_split`.  an
+00020b10: 6420 7465 6c6c 7320 7573 2074 6865 2070  d tells us the p
+00020b20: 7265 6369 7365 2070 6169 7220 6561 6368  recise pair each
+00020b30: 2070 6169 7220 6665 6174 7572 6520 6265   pair feature be
+00020b40: 6c6f 6e67 7320 746f 2e20 496e 206f 7572  longs to. In our
+00020b50: 2063 6173 650a 0a20 203e 3e3e 2061 746f   case..  >>> ato
+00020b60: 6d5f 746f 5f70 6169 7220 3d20 6e70 2e61  m_to_pair = np.a
+00020b70: 7272 6179 285b 5b30 2c20 305d 2c0a 2020  rray([[0, 0],.  
+00020b80: 2e2e 2e20 2020 2020 2020 2020 2020 2020  ...             
+00020b90: 2020 2020 2020 2020 2020 2020 205b 302c               [0,
+00020ba0: 2031 5d2c 0a20 202e 2e2e 2020 2020 2020   1],.  ...      
+00020bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020bc0: 2020 2020 5b30 2c20 325d 2c0a 2020 2e2e      [0, 2],.  ..
+00020bd0: 2e20 2020 2020 2020 2020 2020 2020 2020  .               
+00020be0: 2020 2020 2020 2020 2020 205b 312c 2030             [1, 0
+00020bf0: 5d2c 0a20 202e 2e2e 2020 2020 2020 2020  ],.  ...        
+00020c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020c10: 2020 5b31 2c20 315d 2c0a 2020 2e2e 2e20    [1, 1],.  ... 
+00020c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020c30: 2020 2020 2020 2020 205b 312c 2032 5d2c           [1, 2],
+00020c40: 0a20 202e 2e2e 2020 2020 2020 2020 2020  .  ...          
+00020c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020c60: 5b32 2c20 305d 2c0a 2020 2e2e 2e20 2020  [2, 0],.  ...   
+00020c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020c80: 2020 2020 2020 205b 322c 2031 5d2c 0a20         [2, 1],. 
+00020c90: 202e 2e2e 2020 2020 2020 2020 2020 2020   ...            
+00020ca0: 2020 2020 2020 2020 2020 2020 2020 5b32                [2
+00020cb0: 2c20 325d 2c0a 2020 2e2e 2e20 2020 2020  , 2],.  ...     
+00020cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020cd0: 2020 2020 205b 332c 2033 5d5d 290a 0a20       [3, 3]]).. 
+00020ce0: 204c 6574 2773 206e 6f77 2064 6566 696e   Let's now defin
+00020cf0: 6520 7468 6520 6163 7475 616c 206c 6179  e the actual lay
+00020d00: 6572 0a0a 2020 3e3e 3e20 6c61 7965 7220  er..  >>> layer 
+00020d10: 3d20 5765 6176 654c 6179 6572 2829 0a0a  = WeaveLayer()..
+00020d20: 2020 416e 6420 696e 766f 6b65 2069 740a    And invoke it.
+00020d30: 0a20 203e 3e3e 205b 412c 2050 5d20 3d20  .  >>> [A, P] = 
+00020d40: 6c61 7965 7228 5b61 746f 6d5f 6665 6174  layer([atom_feat
+00020d50: 2c20 7061 6972 5f66 6561 742c 2070 6169  , pair_feat, pai
+00020d60: 725f 7370 6c69 742c 2061 746f 6d5f 746f  r_split, atom_to
+00020d70: 5f70 6169 725d 290a 0a20 2054 6865 2077  _pair])..  The w
+00020d80: 6561 7665 206c 6179 6572 2070 726f 6475  eave layer produ
+00020d90: 6365 7320 6e65 7720 6174 6f6d 2f70 6169  ces new atom/pai
+00020da0: 7220 6665 6174 7572 6573 2e20 4c65 7427  r features. Let'
+00020db0: 7320 6368 6563 6b20 7468 6569 7220 7368  s check their sh
+00020dc0: 6170 6573 0a0a 2020 3e3e 3e20 4120 3d20  apes..  >>> A = 
+00020dd0: 412e 6465 7461 6368 2829 2e6e 756d 7079  A.detach().numpy
+00020de0: 2829 0a20 203e 3e3e 2041 2e73 6861 7065  ().  >>> A.shape
+00020df0: 0a20 2028 342c 2035 3029 0a20 203e 3e3e  .  (4, 50).  >>>
+00020e00: 2050 203d 2050 2e64 6574 6163 6828 292e   P = P.detach().
+00020e10: 6e75 6d70 7928 290a 2020 3e3e 3e20 502e  numpy().  >>> P.
+00020e20: 7368 6170 650a 2020 2831 302c 2035 3029  shape.  (10, 50)
+00020e30: 0a0a 2020 5468 6520 3420 6973 2060 746f  ..  The 4 is `to
+00020e40: 7461 6c5f 6e75 6d5f 6174 6f6d 7360 2061  tal_num_atoms` a
+00020e50: 6e64 2074 6865 2031 3020 6973 2074 6865  nd the 10 is the
+00020e60: 2074 6f74 616c 206e 756d 6265 7220 6f66   total number of
+00020e70: 2070 6169 7273 2e20 5768 6572 650a 2020   pairs. Where.  
+00020e80: 646f 6573 2060 3530 6020 636f 6d65 2066  does `50` come f
+00020e90: 726f 6d3f 2049 7427 7320 6672 6f6d 2074  rom? It's from t
+00020ea0: 6865 2064 6566 6175 6c74 2061 7267 756d  he default argum
+00020eb0: 656e 7473 2060 6e5f 6174 6f6d 5f69 6e70  ents `n_atom_inp
+00020ec0: 7574 5f66 6561 7460 2061 6e64 0a20 2060  ut_feat` and.  `
+00020ed0: 6e5f 7061 6972 5f69 6e70 7574 5f66 6561  n_pair_input_fea
+00020ee0: 7460 2e0a 0a20 2052 6566 6572 656e 6365  t`...  Reference
+00020ef0: 730a 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20  s.  ----------. 
+00020f00: 202e 2e20 5b31 5d20 4b65 6172 6e65 732c   .. [1] Kearnes,
+00020f10: 2053 7465 7665 6e2c 2065 7420 616c 2e20   Steven, et al. 
+00020f20: 224d 6f6c 6563 756c 6172 2067 7261 7068  "Molecular graph
+00020f30: 2063 6f6e 766f 6c75 7469 6f6e 733a 206d   convolutions: m
+00020f40: 6f76 696e 6720 6265 796f 6e64 0a20 2020  oving beyond.   
+00020f50: 2020 2020 2066 696e 6765 7270 7269 6e74       fingerprint
+00020f60: 732e 2220 4a6f 7572 6e61 6c20 6f66 2063  s." Journal of c
+00020f70: 6f6d 7075 7465 722d 6169 6465 6420 6d6f  omputer-aided mo
+00020f80: 6c65 6375 6c61 7220 6465 7369 676e 2033  lecular design 3
+00020f90: 302e 3820 2832 3031 3629 3a0a 2020 2020  0.8 (2016):.    
+00020fa0: 2020 2020 3539 352d 3630 382e 0a20 2022      595-608..  "
+00020fb0: 2222 0a0a 2020 2020 6465 6620 5f5f 696e  ""..    def __in
+00020fc0: 6974 5f5f 2873 656c 662c 0a20 2020 2020  it__(self,.     
+00020fd0: 2020 2020 2020 2020 2020 2020 6e5f 6174              n_at
+00020fe0: 6f6d 5f69 6e70 7574 5f66 6561 743a 2069  om_input_feat: i
+00020ff0: 6e74 203d 2037 352c 0a20 2020 2020 2020  nt = 75,.       
+00021000: 2020 2020 2020 2020 2020 6e5f 7061 6972            n_pair
+00021010: 5f69 6e70 7574 5f66 6561 743a 2069 6e74  _input_feat: int
+00021020: 203d 2031 342c 0a20 2020 2020 2020 2020   = 14,.         
+00021030: 2020 2020 2020 2020 6e5f 6174 6f6d 5f6f          n_atom_o
+00021040: 7574 7075 745f 6665 6174 3a20 696e 7420  utput_feat: int 
+00021050: 3d20 3530 2c0a 2020 2020 2020 2020 2020  = 50,.          
+00021060: 2020 2020 2020 206e 5f70 6169 725f 6f75         n_pair_ou
+00021070: 7470 7574 5f66 6561 743a 2069 6e74 203d  tput_feat: int =
+00021080: 2035 302c 0a20 2020 2020 2020 2020 2020   50,.           
+00021090: 2020 2020 2020 6e5f 6869 6464 656e 5f41        n_hidden_A
+000210a0: 413a 2069 6e74 203d 2035 302c 0a20 2020  A: int = 50,.   
+000210b0: 2020 2020 2020 2020 2020 2020 2020 6e5f                n_
+000210c0: 6869 6464 656e 5f50 413a 2069 6e74 203d  hidden_PA: int =
+000210d0: 2035 302c 0a20 2020 2020 2020 2020 2020   50,.           
+000210e0: 2020 2020 2020 6e5f 6869 6464 656e 5f41        n_hidden_A
+000210f0: 503a 2069 6e74 203d 2035 302c 0a20 2020  P: int = 50,.   
+00021100: 2020 2020 2020 2020 2020 2020 2020 6e5f                n_
+00021110: 6869 6464 656e 5f50 503a 2069 6e74 203d  hidden_PP: int =
+00021120: 2035 302c 0a20 2020 2020 2020 2020 2020   50,.           
+00021130: 2020 2020 2020 7570 6461 7465 5f70 6169        update_pai
+00021140: 723a 2062 6f6f 6c20 3d20 5472 7565 2c0a  r: bool = True,.
+00021150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00021160: 2069 6e69 745f 3a20 7374 7220 3d20 2778   init_: str = 'x
+00021170: 6176 6965 725f 756e 6966 6f72 6d5f 272c  avier_uniform_',
+00021180: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00021190: 2020 6163 7469 7661 7469 6f6e 3a20 7374    activation: st
+000211a0: 7220 3d20 2772 656c 7527 2c0a 2020 2020  r = 'relu',.    
+000211b0: 2020 2020 2020 2020 2020 2020 2062 6174               bat
+000211c0: 6368 5f6e 6f72 6d61 6c69 7a65 3a20 626f  ch_normalize: bo
+000211d0: 6f6c 203d 2054 7275 652c 0a20 2020 2020  ol = True,.     
+000211e0: 2020 2020 2020 2020 2020 2020 2a2a 6b77              **kw
+000211f0: 6172 6773 293a 0a20 2020 2020 2020 2022  args):.        "
+00021200: 2222 0a20 2020 2050 6172 616d 6574 6572  "".    Parameter
+00021210: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  s.    ----------
+00021220: 0a20 2020 206e 5f61 746f 6d5f 696e 7075  .    n_atom_inpu
+00021230: 745f 6665 6174 3a20 696e 742c 206f 7074  t_feat: int, opt
+00021240: 696f 6e61 6c20 2864 6566 6175 6c74 2037  ional (default 7
+00021250: 3529 0a20 2020 2020 204e 756d 6265 7220  5).      Number 
+00021260: 6f66 2066 6561 7475 7265 7320 666f 7220  of features for 
+00021270: 6561 6368 2061 746f 6d20 696e 2069 6e70  each atom in inp
+00021280: 7574 2e0a 2020 2020 6e5f 7061 6972 5f69  ut..    n_pair_i
+00021290: 6e70 7574 5f66 6561 743a 2069 6e74 2c20  nput_feat: int, 
+000212a0: 6f70 7469 6f6e 616c 2028 6465 6661 756c  optional (defaul
+000212b0: 7420 3134 290a 2020 2020 2020 4e75 6d62  t 14).      Numb
+000212c0: 6572 206f 6620 6665 6174 7572 6573 2066  er of features f
+000212d0: 6f72 2065 6163 6820 7061 6972 206f 6620  or each pair of 
+000212e0: 6174 6f6d 7320 696e 2069 6e70 7574 2e0a  atoms in input..
+000212f0: 2020 2020 6e5f 6174 6f6d 5f6f 7574 7075      n_atom_outpu
+00021300: 745f 6665 6174 3a20 696e 742c 206f 7074  t_feat: int, opt
+00021310: 696f 6e61 6c20 2864 6566 6175 6c74 2035  ional (default 5
+00021320: 3029 0a20 2020 2020 204e 756d 6265 7220  0).      Number 
+00021330: 6f66 2066 6561 7475 7265 7320 666f 7220  of features for 
+00021340: 6561 6368 2061 746f 6d20 696e 206f 7574  each atom in out
+00021350: 7075 742e 0a20 2020 206e 5f70 6169 725f  put..    n_pair_
+00021360: 6f75 7470 7574 5f66 6561 743a 2069 6e74  output_feat: int
+00021370: 2c20 6f70 7469 6f6e 616c 2028 6465 6661  , optional (defa
+00021380: 756c 7420 3530 290a 2020 2020 2020 4e75  ult 50).      Nu
+00021390: 6d62 6572 206f 6620 6665 6174 7572 6573  mber of features
+000213a0: 2066 6f72 2065 6163 6820 7061 6972 206f   for each pair o
+000213b0: 6620 6174 6f6d 7320 696e 206f 7574 7075  f atoms in outpu
+000213c0: 742e 0a20 2020 206e 5f68 6964 6465 6e5f  t..    n_hidden_
+000213d0: 4141 3a20 696e 742c 206f 7074 696f 6e61  AA: int, optiona
+000213e0: 6c20 2864 6566 6175 6c74 2035 3029 0a20  l (default 50). 
+000213f0: 2020 2020 204e 756d 6265 7220 6f66 2075       Number of u
+00021400: 6e69 7473 2863 6f6e 766f 6c75 7469 6f6e  nits(convolution
+00021410: 2064 6570 7468 7329 2069 6e20 636f 7272   depths) in corr
+00021420: 6573 706f 6e64 696e 6720 6869 6464 656e  esponding hidden
+00021430: 206c 6179 6572 0a20 2020 206e 5f68 6964   layer.    n_hid
+00021440: 6465 6e5f 5041 3a20 696e 742c 206f 7074  den_PA: int, opt
+00021450: 696f 6e61 6c20 2864 6566 6175 6c74 2035  ional (default 5
+00021460: 3029 0a20 2020 2020 204e 756d 6265 7220  0).      Number 
+00021470: 6f66 2075 6e69 7473 2863 6f6e 766f 6c75  of units(convolu
+00021480: 7469 6f6e 2064 6570 7468 7329 2069 6e20  tion depths) in 
+00021490: 636f 7272 6573 706f 6e64 696e 6720 6869  corresponding hi
+000214a0: 6464 656e 206c 6179 6572 0a20 2020 206e  dden layer.    n
+000214b0: 5f68 6964 6465 6e5f 4150 3a20 696e 742c  _hidden_AP: int,
+000214c0: 206f 7074 696f 6e61 6c20 2864 6566 6175   optional (defau
+000214d0: 6c74 2035 3029 0a20 2020 2020 204e 756d  lt 50).      Num
+000214e0: 6265 7220 6f66 2075 6e69 7473 2863 6f6e  ber of units(con
+000214f0: 766f 6c75 7469 6f6e 2064 6570 7468 7329  volution depths)
+00021500: 2069 6e20 636f 7272 6573 706f 6e64 696e   in correspondin
+00021510: 6720 6869 6464 656e 206c 6179 6572 0a20  g hidden layer. 
+00021520: 2020 206e 5f68 6964 6465 6e5f 5050 3a20     n_hidden_PP: 
+00021530: 696e 742c 206f 7074 696f 6e61 6c20 2864  int, optional (d
+00021540: 6566 6175 6c74 2035 3029 0a20 2020 2020  efault 50).     
+00021550: 204e 756d 6265 7220 6f66 2075 6e69 7473   Number of units
+00021560: 2863 6f6e 766f 6c75 7469 6f6e 2064 6570  (convolution dep
+00021570: 7468 7329 2069 6e20 636f 7272 6573 706f  ths) in correspo
+00021580: 6e64 696e 6720 6869 6464 656e 206c 6179  nding hidden lay
+00021590: 6572 0a20 2020 2075 7064 6174 655f 7061  er.    update_pa
+000215a0: 6972 3a20 626f 6f6c 2c20 6f70 7469 6f6e  ir: bool, option
+000215b0: 616c 2028 6465 6661 756c 7420 5472 7565  al (default True
+000215c0: 290a 2020 2020 2020 5768 6574 6865 7220  ).      Whether 
+000215d0: 746f 2063 616c 6375 6c61 7465 2066 6f72  to calculate for
+000215e0: 2070 6169 7220 6665 6174 7572 6573 2c0a   pair features,.
+000215f0: 2020 2020 2020 636f 756c 6420 6265 2074        could be t
+00021600: 7572 6e65 6420 6f66 6620 666f 7220 6c61  urned off for la
+00021610: 7374 206c 6179 6572 0a20 2020 2069 6e69  st layer.    ini
+00021620: 743a 2073 7472 2c20 6f70 7469 6f6e 616c  t: str, optional
+00021630: 2028 6465 6661 756c 7420 2778 6176 6965   (default 'xavie
+00021640: 725f 756e 6966 6f72 6d5f 2729 0a20 2020  r_uniform_').   
+00021650: 2020 2057 6569 6768 7420 696e 6974 6961     Weight initia
+00021660: 6c69 7a61 7469 6f6e 2066 6f72 2066 696c  lization for fil
+00021670: 7465 7273 2e0a 2020 2020 6163 7469 7661  ters..    activa
+00021680: 7469 6f6e 3a20 7374 722c 206f 7074 696f  tion: str, optio
+00021690: 6e61 6c20 2864 6566 6175 6c74 2027 7265  nal (default 're
+000216a0: 6c75 2729 0a20 2020 2020 2041 6374 6976  lu').      Activ
+000216b0: 6174 696f 6e20 6675 6e63 7469 6f6e 2061  ation function a
+000216c0: 7070 6c69 6564 0a20 2020 2062 6174 6368  pplied.    batch
+000216d0: 5f6e 6f72 6d61 6c69 7a65 3a20 626f 6f6c  _normalize: bool
+000216e0: 2c20 6f70 7469 6f6e 616c 2028 6465 6661  , optional (defa
+000216f0: 756c 7420 5472 7565 290a 2020 2020 2020  ult True).      
+00021700: 4966 2074 6869 7320 6973 2074 7572 6e65  If this is turne
+00021710: 6420 6f6e 2c20 6170 706c 7920 6261 7463  d on, apply batc
+00021720: 6820 6e6f 726d 616c 697a 6174 696f 6e20  h normalization 
+00021730: 6265 666f 7265 2061 7070 6c79 696e 670a  before applying.
+00021740: 2020 2020 2020 6163 7469 7661 7469 6f6e        activation
+00021750: 2066 756e 6374 696f 6e73 206f 6e20 636f   functions on co
+00021760: 6e76 6f6c 7574 696f 6e61 6c20 6c61 7965  nvolutional laye
+00021770: 7273 2e0a 2020 2020 2222 220a 2020 2020  rs..    """.    
+00021780: 2020 2020 7375 7065 7228 5765 6176 654c      super(WeaveL
+00021790: 6179 6572 2c20 7365 6c66 292e 5f5f 696e  ayer, self).__in
+000217a0: 6974 5f5f 282a 2a6b 7761 7267 7329 0a20  it__(**kwargs). 
+000217b0: 2020 2020 2020 2073 656c 662e 696e 6974         self.init
+000217c0: 3a20 7374 7220 3d20 696e 6974 5f20 2023  : str = init_  #
+000217d0: 2053 6574 2077 6569 6768 7420 696e 6974   Set weight init
+000217e0: 6961 6c69 7a61 7469 6f6e 0a20 2020 2020  ialization.     
+000217f0: 2020 2073 656c 662e 6163 7469 7661 7469     self.activati
+00021800: 6f6e 3a20 7374 7220 3d20 6163 7469 7661  on: str = activa
+00021810: 7469 6f6e 2020 2320 4765 7420 6163 7469  tion  # Get acti
+00021820: 7661 7469 6f6e 730a 2020 2020 2020 2020  vations.        
+00021830: 7365 6c66 2e61 6374 6976 6174 696f 6e5f  self.activation_
+00021840: 666e 3a20 746f 7263 682e 6e6e 2e4d 6f64  fn: torch.nn.Mod
+00021850: 756c 6520 3d20 6765 745f 6163 7469 7661  ule = get_activa
+00021860: 7469 6f6e 2861 6374 6976 6174 696f 6e29  tion(activation)
+00021870: 0a20 2020 2020 2020 2073 656c 662e 7570  .        self.up
+00021880: 6461 7465 5f70 6169 723a 2062 6f6f 6c20  date_pair: bool 
+00021890: 3d20 7570 6461 7465 5f70 6169 7220 2023  = update_pair  #
+000218a0: 206c 6173 7420 7765 6176 6520 6c61 7965   last weave laye
+000218b0: 7220 646f 6573 206e 6f74 206e 6565 6420  r does not need 
+000218c0: 746f 2075 7064 6174 650a 2020 2020 2020  to update.      
+000218d0: 2020 7365 6c66 2e6e 5f68 6964 6465 6e5f    self.n_hidden_
+000218e0: 4141 3a20 696e 7420 3d20 6e5f 6869 6464  AA: int = n_hidd
+000218f0: 656e 5f41 410a 2020 2020 2020 2020 7365  en_AA.        se
+00021900: 6c66 2e6e 5f68 6964 6465 6e5f 5041 3a20  lf.n_hidden_PA: 
+00021910: 696e 7420 3d20 6e5f 6869 6464 656e 5f50  int = n_hidden_P
+00021920: 410a 2020 2020 2020 2020 7365 6c66 2e6e  A.        self.n
+00021930: 5f68 6964 6465 6e5f 4150 3a20 696e 7420  _hidden_AP: int 
+00021940: 3d20 6e5f 6869 6464 656e 5f41 500a 2020  = n_hidden_AP.  
+00021950: 2020 2020 2020 7365 6c66 2e6e 5f68 6964        self.n_hid
+00021960: 6465 6e5f 5050 3a20 696e 7420 3d20 6e5f  den_PP: int = n_
+00021970: 6869 6464 656e 5f50 500a 2020 2020 2020  hidden_PP.      
+00021980: 2020 7365 6c66 2e6e 5f68 6964 6465 6e5f    self.n_hidden_
+00021990: 413a 2069 6e74 203d 206e 5f68 6964 6465  A: int = n_hidde
+000219a0: 6e5f 4141 202b 206e 5f68 6964 6465 6e5f  n_AA + n_hidden_
+000219b0: 5041 0a20 2020 2020 2020 2073 656c 662e  PA.        self.
+000219c0: 6e5f 6869 6464 656e 5f50 3a20 696e 7420  n_hidden_P: int 
+000219d0: 3d20 6e5f 6869 6464 656e 5f41 5020 2b20  = n_hidden_AP + 
+000219e0: 6e5f 6869 6464 656e 5f50 500a 2020 2020  n_hidden_PP.    
+000219f0: 2020 2020 7365 6c66 2e62 6174 6368 5f6e      self.batch_n
+00021a00: 6f72 6d61 6c69 7a65 3a20 626f 6f6c 203d  ormalize: bool =
+00021a10: 2062 6174 6368 5f6e 6f72 6d61 6c69 7a65   batch_normalize
+00021a20: 0a0a 2020 2020 2020 2020 7365 6c66 2e6e  ..        self.n
+00021a30: 5f61 746f 6d5f 696e 7075 745f 6665 6174  _atom_input_feat
+00021a40: 3a20 696e 7420 3d20 6e5f 6174 6f6d 5f69  : int = n_atom_i
+00021a50: 6e70 7574 5f66 6561 740a 2020 2020 2020  nput_feat.      
+00021a60: 2020 7365 6c66 2e6e 5f70 6169 725f 696e    self.n_pair_in
+00021a70: 7075 745f 6665 6174 3a20 696e 7420 3d20  put_feat: int = 
+00021a80: 6e5f 7061 6972 5f69 6e70 7574 5f66 6561  n_pair_input_fea
+00021a90: 740a 2020 2020 2020 2020 7365 6c66 2e6e  t.        self.n
+00021aa0: 5f61 746f 6d5f 6f75 7470 7574 5f66 6561  _atom_output_fea
+00021ab0: 743a 2069 6e74 203d 206e 5f61 746f 6d5f  t: int = n_atom_
+00021ac0: 6f75 7470 7574 5f66 6561 740a 2020 2020  output_feat.    
+00021ad0: 2020 2020 7365 6c66 2e6e 5f70 6169 725f      self.n_pair_
+00021ae0: 6f75 7470 7574 5f66 6561 743a 2069 6e74  output_feat: int
+00021af0: 203d 206e 5f70 6169 725f 6f75 7470 7574   = n_pair_output
+00021b00: 5f66 6561 740a 0a20 2020 2020 2020 2023  _feat..        #
+00021b10: 2043 6f6e 7374 7275 6374 2069 6e74 6572   Construct inter
+00021b20: 6e61 6c20 7472 6169 6e61 626c 6520 7765  nal trainable we
+00021b30: 6967 6874 730a 2020 2020 2020 2020 696e  ights.        in
+00021b40: 6974 203d 2067 6574 6174 7472 2869 6e69  it = getattr(ini
+00021b50: 7469 616c 697a 6572 732c 2073 656c 662e  tializers, self.
+00021b60: 696e 6974 290a 2020 2020 2020 2020 2320  init).        # 
+00021b70: 5765 6967 6874 206d 6174 7269 7820 616e  Weight matrix an
+00021b80: 6420 6269 6173 206d 6174 7269 7820 7265  d bias matrix re
+00021b90: 7175 6972 6564 2074 6f20 636f 6d70 7574  quired to comput
+00021ba0: 6520 6e65 7720 6174 6f6d 206c 6179 6572  e new atom layer
+00021bb0: 2066 726f 6d20 7468 6520 7072 6576 696f   from the previo
+00021bc0: 7573 2061 746f 6d20 6c61 7965 720a 2020  us atom layer.  
+00021bd0: 2020 2020 2020 7365 6c66 2e57 5f41 413a        self.W_AA:
+00021be0: 2074 6f72 6368 2e54 656e 736f 7220 3d20   torch.Tensor = 
+00021bf0: 696e 6974 280a 2020 2020 2020 2020 2020  init(.          
+00021c00: 2020 746f 7263 682e 656d 7074 7928 7365    torch.empty(se
+00021c10: 6c66 2e6e 5f61 746f 6d5f 696e 7075 745f  lf.n_atom_input_
+00021c20: 6665 6174 2c20 7365 6c66 2e6e 5f68 6964  feat, self.n_hid
+00021c30: 6465 6e5f 4141 2929 0a20 2020 2020 2020  den_AA)).       
+00021c40: 2073 656c 662e 625f 4141 3a20 746f 7263   self.b_AA: torc
+00021c50: 682e 5465 6e73 6f72 203d 2074 6f72 6368  h.Tensor = torch
+00021c60: 2e7a 6572 6f73 2828 7365 6c66 2e6e 5f68  .zeros((self.n_h
+00021c70: 6964 6465 6e5f 4141 2c29 290a 2020 2020  idden_AA,)).    
+00021c80: 2020 2020 7365 6c66 2e41 415f 626e 3a20      self.AA_bn: 
+00021c90: 6e6e 2e42 6174 6368 4e6f 726d 3164 203d  nn.BatchNorm1d =
+00021ca0: 206e 6e2e 4261 7463 684e 6f72 6d31 6428   nn.BatchNorm1d(
+00021cb0: 0a20 2020 2020 2020 2020 2020 206e 756d  .            num
+00021cc0: 5f66 6561 7475 7265 733d 7365 6c66 2e6e  _features=self.n
+00021cd0: 5f68 6964 6465 6e5f 4141 2c0a 2020 2020  _hidden_AA,.    
+00021ce0: 2020 2020 2020 2020 6570 733d 3165 2d33          eps=1e-3
+00021cf0: 2c0a 2020 2020 2020 2020 2020 2020 6d6f  ,.            mo
+00021d00: 6d65 6e74 756d 3d30 2e39 392c 0a20 2020  mentum=0.99,.   
+00021d10: 2020 2020 2020 2020 2061 6666 696e 653d           affine=
+00021d20: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
+00021d30: 2020 7472 6163 6b5f 7275 6e6e 696e 675f    track_running_
+00021d40: 7374 6174 733d 5472 7565 290a 0a20 2020  stats=True)..   
+00021d50: 2020 2020 2023 2057 6569 6768 7420 6d61       # Weight ma
+00021d60: 7472 6978 2061 6e64 2062 6961 7320 6d61  trix and bias ma
+00021d70: 7472 6978 2072 6571 7569 7265 6420 746f  trix required to
+00021d80: 2063 6f6d 7075 7465 206e 6577 2061 746f   compute new ato
+00021d90: 6d20 6c61 7965 7220 6672 6f6d 2074 6865  m layer from the
+00021da0: 2070 7265 7669 6f75 7320 7061 6972 206c   previous pair l
+00021db0: 6179 6572 0a20 2020 2020 2020 2073 656c  ayer.        sel
+00021dc0: 662e 575f 5041 3a20 746f 7263 682e 5465  f.W_PA: torch.Te
+00021dd0: 6e73 6f72 203d 2069 6e69 7428 0a20 2020  nsor = init(.   
+00021de0: 2020 2020 2020 2020 2074 6f72 6368 2e65           torch.e
+00021df0: 6d70 7479 2873 656c 662e 6e5f 7061 6972  mpty(self.n_pair
+00021e00: 5f69 6e70 7574 5f66 6561 742c 2073 656c  _input_feat, sel
+00021e10: 662e 6e5f 6869 6464 656e 5f50 4129 290a  f.n_hidden_PA)).
+00021e20: 2020 2020 2020 2020 7365 6c66 2e62 5f50          self.b_P
+00021e30: 413a 2074 6f72 6368 2e54 656e 736f 7220  A: torch.Tensor 
+00021e40: 3d20 746f 7263 682e 7a65 726f 7328 2873  = torch.zeros((s
+00021e50: 656c 662e 6e5f 6869 6464 656e 5f50 412c  elf.n_hidden_PA,
+00021e60: 2929 0a20 2020 2020 2020 2073 656c 662e  )).        self.
+00021e70: 5041 5f62 6e3a 206e 6e2e 4261 7463 684e  PA_bn: nn.BatchN
+00021e80: 6f72 6d31 6420 3d20 6e6e 2e42 6174 6368  orm1d = nn.Batch
+00021e90: 4e6f 726d 3164 280a 2020 2020 2020 2020  Norm1d(.        
+00021ea0: 2020 2020 6e75 6d5f 6665 6174 7572 6573      num_features
+00021eb0: 3d73 656c 662e 6e5f 6869 6464 656e 5f50  =self.n_hidden_P
+00021ec0: 412c 0a20 2020 2020 2020 2020 2020 2065  A,.            e
+00021ed0: 7073 3d31 652d 332c 0a20 2020 2020 2020  ps=1e-3,.       
+00021ee0: 2020 2020 206d 6f6d 656e 7475 6d3d 302e       momentum=0.
+00021ef0: 3939 2c0a 2020 2020 2020 2020 2020 2020  99,.            
+00021f00: 6166 6669 6e65 3d54 7275 652c 0a20 2020  affine=True,.   
+00021f10: 2020 2020 2020 2020 2074 7261 636b 5f72           track_r
+00021f20: 756e 6e69 6e67 5f73 7461 7473 3d54 7275  unning_stats=Tru
+00021f30: 6529 0a0a 2020 2020 2020 2020 7365 6c66  e)..        self
+00021f40: 2e57 5f41 3a20 746f 7263 682e 5465 6e73  .W_A: torch.Tens
+00021f50: 6f72 203d 2069 6e69 7428 0a20 2020 2020  or = init(.     
+00021f60: 2020 2020 2020 2074 6f72 6368 2e65 6d70         torch.emp
+00021f70: 7479 2873 656c 662e 6e5f 6869 6464 656e  ty(self.n_hidden
+00021f80: 5f41 2c20 7365 6c66 2e6e 5f61 746f 6d5f  _A, self.n_atom_
+00021f90: 6f75 7470 7574 5f66 6561 7429 290a 2020  output_feat)).  
+00021fa0: 2020 2020 2020 7365 6c66 2e62 5f41 3a20        self.b_A: 
+00021fb0: 746f 7263 682e 5465 6e73 6f72 203d 2074  torch.Tensor = t
+00021fc0: 6f72 6368 2e7a 6572 6f73 2828 7365 6c66  orch.zeros((self
+00021fd0: 2e6e 5f61 746f 6d5f 6f75 7470 7574 5f66  .n_atom_output_f
+00021fe0: 6561 742c 2929 0a20 2020 2020 2020 2073  eat,)).        s
+00021ff0: 656c 662e 415f 626e 3a20 6e6e 2e42 6174  elf.A_bn: nn.Bat
+00022000: 6368 4e6f 726d 3164 203d 206e 6e2e 4261  chNorm1d = nn.Ba
+00022010: 7463 684e 6f72 6d31 6428 0a20 2020 2020  tchNorm1d(.     
+00022020: 2020 2020 2020 206e 756d 5f66 6561 7475         num_featu
+00022030: 7265 733d 7365 6c66 2e6e 5f61 746f 6d5f  res=self.n_atom_
+00022040: 6f75 7470 7574 5f66 6561 742c 0a20 2020  output_feat,.   
+00022050: 2020 2020 2020 2020 2065 7073 3d31 652d           eps=1e-
+00022060: 332c 0a20 2020 2020 2020 2020 2020 206d  3,.            m
+00022070: 6f6d 656e 7475 6d3d 302e 3939 2c0a 2020  omentum=0.99,.  
+00022080: 2020 2020 2020 2020 2020 6166 6669 6e65            affine
+00022090: 3d54 7275 652c 0a20 2020 2020 2020 2020  =True,.         
+000220a0: 2020 2074 7261 636b 5f72 756e 6e69 6e67     track_running
+000220b0: 5f73 7461 7473 3d54 7275 6529 0a0a 2020  _stats=True)..  
+000220c0: 2020 2020 2020 6966 2073 656c 662e 7570        if self.up
+000220d0: 6461 7465 5f70 6169 723a 0a20 2020 2020  date_pair:.     
+000220e0: 2020 2020 2020 2023 2057 6569 6768 7420         # Weight 
+000220f0: 6d61 7472 6978 2061 6e64 2062 6961 7320  matrix and bias 
+00022100: 6d61 7472 6978 2072 6571 7569 7265 6420  matrix required 
+00022110: 746f 2063 6f6d 7075 7465 206e 6577 2070  to compute new p
+00022120: 6169 7220 6c61 7965 7220 6672 6f6d 2074  air layer from t
+00022130: 6865 2070 7265 7669 6f75 7320 6174 6f6d  he previous atom
+00022140: 206c 6179 6572 0a20 2020 2020 2020 2020   layer.         
+00022150: 2020 2073 656c 662e 575f 4150 3a20 746f     self.W_AP: to
+00022160: 7263 682e 5465 6e73 6f72 203d 2069 6e69  rch.Tensor = ini
+00022170: 7428 0a20 2020 2020 2020 2020 2020 2020  t(.             
+00022180: 2020 2074 6f72 6368 2e65 6d70 7479 2873     torch.empty(s
+00022190: 656c 662e 6e5f 6174 6f6d 5f69 6e70 7574  elf.n_atom_input
+000221a0: 5f66 6561 7420 2a20 322c 2073 656c 662e  _feat * 2, self.
+000221b0: 6e5f 6869 6464 656e 5f41 5029 290a 2020  n_hidden_AP)).  
+000221c0: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
+000221d0: 5f41 503a 2074 6f72 6368 2e54 656e 736f  _AP: torch.Tenso
+000221e0: 7220 3d20 746f 7263 682e 7a65 726f 7328  r = torch.zeros(
+000221f0: 2873 656c 662e 6e5f 6869 6464 656e 5f41  (self.n_hidden_A
+00022200: 502c 2929 0a20 2020 2020 2020 2020 2020  P,)).           
+00022210: 2073 656c 662e 4150 5f62 6e3a 206e 6e2e   self.AP_bn: nn.
+00022220: 4261 7463 684e 6f72 6d31 6420 3d20 6e6e  BatchNorm1d = nn
+00022230: 2e42 6174 6368 4e6f 726d 3164 280a 2020  .BatchNorm1d(.  
+00022240: 2020 2020 2020 2020 2020 2020 2020 6e75                nu
+00022250: 6d5f 6665 6174 7572 6573 3d73 656c 662e  m_features=self.
+00022260: 6e5f 6869 6464 656e 5f41 502c 0a20 2020  n_hidden_AP,.   
+00022270: 2020 2020 2020 2020 2020 2020 2065 7073               eps
+00022280: 3d31 652d 332c 0a20 2020 2020 2020 2020  =1e-3,.         
+00022290: 2020 2020 2020 206d 6f6d 656e 7475 6d3d         momentum=
+000222a0: 302e 3939 2c0a 2020 2020 2020 2020 2020  0.99,.          
+000222b0: 2020 2020 2020 6166 6669 6e65 3d54 7275        affine=Tru
+000222c0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+000222d0: 2020 2074 7261 636b 5f72 756e 6e69 6e67     track_running
+000222e0: 5f73 7461 7473 3d54 7275 6529 0a20 2020  _stats=True).   
+000222f0: 2020 2020 2020 2020 2023 2057 6569 6768           # Weigh
+00022300: 7420 6d61 7472 6978 2061 6e64 2062 6961  t matrix and bia
+00022310: 7320 6d61 7472 6978 2072 6571 7569 7265  s matrix require
+00022320: 6420 746f 2063 6f6d 7075 7465 206e 6577  d to compute new
+00022330: 2070 6169 7220 6c61 7965 7220 6672 6f6d   pair layer from
+00022340: 2074 6865 2070 7265 7669 6f75 7320 7061   the previous pa
+00022350: 6972 206c 6179 6572 0a20 2020 2020 2020  ir layer.       
+00022360: 2020 2020 2073 656c 662e 575f 5050 3a20       self.W_PP: 
+00022370: 746f 7263 682e 5465 6e73 6f72 203d 2069  torch.Tensor = i
+00022380: 6e69 7428 0a20 2020 2020 2020 2020 2020  nit(.           
+00022390: 2020 2020 2074 6f72 6368 2e65 6d70 7479       torch.empty
+000223a0: 2873 656c 662e 6e5f 7061 6972 5f69 6e70  (self.n_pair_inp
+000223b0: 7574 5f66 6561 742c 2073 656c 662e 6e5f  ut_feat, self.n_
+000223c0: 6869 6464 656e 5f50 5029 290a 2020 2020  hidden_PP)).    
+000223d0: 2020 2020 2020 2020 7365 6c66 2e62 5f50          self.b_P
+000223e0: 503a 2074 6f72 6368 2e54 656e 736f 7220  P: torch.Tensor 
+000223f0: 3d20 746f 7263 682e 7a65 726f 7328 2873  = torch.zeros((s
+00022400: 656c 662e 6e5f 6869 6464 656e 5f50 502c  elf.n_hidden_PP,
+00022410: 2929 0a20 2020 2020 2020 2020 2020 2073  )).            s
+00022420: 656c 662e 5050 5f62 6e3a 206e 6e2e 4261  elf.PP_bn: nn.Ba
+00022430: 7463 684e 6f72 6d31 6420 3d20 6e6e 2e42  tchNorm1d = nn.B
+00022440: 6174 6368 4e6f 726d 3164 280a 2020 2020  atchNorm1d(.    
+00022450: 2020 2020 2020 2020 2020 2020 6e75 6d5f              num_
+00022460: 6665 6174 7572 6573 3d73 656c 662e 6e5f  features=self.n_
+00022470: 6869 6464 656e 5f50 502c 0a20 2020 2020  hidden_PP,.     
+00022480: 2020 2020 2020 2020 2020 2065 7073 3d31             eps=1
+00022490: 652d 332c 0a20 2020 2020 2020 2020 2020  e-3,.           
+000224a0: 2020 2020 206d 6f6d 656e 7475 6d3d 302e       momentum=0.
+000224b0: 3939 2c0a 2020 2020 2020 2020 2020 2020  99,.            
+000224c0: 2020 2020 6166 6669 6e65 3d54 7275 652c      affine=True,
+000224d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000224e0: 2074 7261 636b 5f72 756e 6e69 6e67 5f73   track_running_s
+000224f0: 7461 7473 3d54 7275 6529 0a0a 2020 2020  tats=True)..    
+00022500: 2020 2020 2020 2020 7365 6c66 2e57 5f50          self.W_P
+00022510: 3a20 746f 7263 682e 5465 6e73 6f72 203d  : torch.Tensor =
+00022520: 2069 6e69 7428 0a20 2020 2020 2020 2020   init(.         
+00022530: 2020 2020 2020 2074 6f72 6368 2e65 6d70         torch.emp
+00022540: 7479 2873 656c 662e 6e5f 6869 6464 656e  ty(self.n_hidden
+00022550: 5f50 2c20 7365 6c66 2e6e 5f70 6169 725f  _P, self.n_pair_
+00022560: 6f75 7470 7574 5f66 6561 7429 290a 2020  output_feat)).  
+00022570: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
+00022580: 5f50 3a20 746f 7263 682e 5465 6e73 6f72  _P: torch.Tensor
+00022590: 203d 2074 6f72 6368 2e7a 6572 6f73 2828   = torch.zeros((
+000225a0: 7365 6c66 2e6e 5f70 6169 725f 6f75 7470  self.n_pair_outp
+000225b0: 7574 5f66 6561 742c 2929 0a20 2020 2020  ut_feat,)).     
+000225c0: 2020 2020 2020 2073 656c 662e 505f 626e         self.P_bn
+000225d0: 3a20 6e6e 2e42 6174 6368 4e6f 726d 3164  : nn.BatchNorm1d
+000225e0: 203d 206e 6e2e 4261 7463 684e 6f72 6d31   = nn.BatchNorm1
+000225f0: 6428 0a20 2020 2020 2020 2020 2020 2020  d(.             
+00022600: 2020 206e 756d 5f66 6561 7475 7265 733d     num_features=
+00022610: 7365 6c66 2e6e 5f70 6169 725f 6f75 7470  self.n_pair_outp
+00022620: 7574 5f66 6561 742c 0a20 2020 2020 2020  ut_feat,.       
+00022630: 2020 2020 2020 2020 2065 7073 3d31 652d           eps=1e-
+00022640: 332c 0a20 2020 2020 2020 2020 2020 2020  3,.             
+00022650: 2020 206d 6f6d 656e 7475 6d3d 302e 3939     momentum=0.99
+00022660: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00022670: 2020 6166 6669 6e65 3d54 7275 652c 0a20    affine=True,. 
+00022680: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00022690: 7261 636b 5f72 756e 6e69 6e67 5f73 7461  rack_running_sta
+000226a0: 7473 3d54 7275 6529 0a20 2020 2020 2020  ts=True).       
+000226b0: 2073 656c 662e 6275 696c 7420 3d20 5472   self.built = Tr
+000226c0: 7565 0a0a 2020 2020 6465 6620 5f5f 7265  ue..    def __re
+000226d0: 7072 5f5f 2873 656c 6629 202d 3e20 7374  pr__(self) -> st
+000226e0: 723a 0a20 2020 2020 2020 2022 2222 0a20  r:.        """. 
+000226f0: 2020 2052 6574 7572 6e73 2061 2073 7472     Returns a str
+00022700: 696e 6720 7265 7072 6573 656e 7461 7469  ing representati
+00022710: 6f6e 206f 6620 7468 6520 6f62 6a65 6374  on of the object
+00022720: 2e0a 0a20 2020 2052 6574 7572 6e73 3a0a  ...    Returns:.
+00022730: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
+00022740: 7374 723a 2041 2073 7472 696e 6720 7468  str: A string th
+00022750: 6174 2063 6f6e 7461 696e 7320 7468 6520  at contains the 
+00022760: 636c 6173 7320 6e61 6d65 2066 6f6c 6c6f  class name follo
+00022770: 7765 6420 6279 2074 6865 2076 616c 7565  wed by the value
+00022780: 7320 6f66 2069 7473 2069 6e73 7461 6e63  s of its instanc
+00022790: 6520 7661 7269 6162 6c65 2e0a 2020 2020  e variable..    
+000227a0: 2222 220a 2020 2020 2020 2020 2320 666c  """.        # fl
+000227b0: 616b 6538 3a20 6e6f 7161 0a20 2020 2020  ake8: noqa.     
+000227c0: 2020 2072 6574 7572 6e20 280a 2020 2020     return (.    
+000227d0: 2020 2020 2020 2020 6627 7b73 656c 662e          f'{self.
+000227e0: 5f5f 636c 6173 735f 5f2e 5f5f 6e61 6d65  __class__.__name
+000227f0: 5f5f 7d28 6e5f 6174 6f6d 5f69 6e70 7574  __}(n_atom_input
+00022800: 5f66 6561 743a 7b73 656c 662e 6e5f 6174  _feat:{self.n_at
+00022810: 6f6d 5f69 6e70 7574 5f66 6561 747d 2c6e  om_input_feat},n
+00022820: 5f70 6169 725f 696e 7075 745f 6665 6174  _pair_input_feat
+00022830: 3a7b 7365 6c66 2e6e 5f70 6169 725f 696e  :{self.n_pair_in
+00022840: 7075 745f 6665 6174 7d2c 6e5f 6174 6f6d  put_feat},n_atom
+00022850: 5f6f 7574 7075 745f 6665 6174 3a7b 7365  _output_feat:{se
+00022860: 6c66 2e6e 5f61 746f 6d5f 6f75 7470 7574  lf.n_atom_output
+00022870: 5f66 6561 747d 2c6e 5f70 6169 725f 6f75  _feat},n_pair_ou
+00022880: 7470 7574 5f66 6561 743a 7b73 656c 662e  tput_feat:{self.
+00022890: 6e5f 7061 6972 5f6f 7574 7075 745f 6665  n_pair_output_fe
+000228a0: 6174 7d2c 6e5f 6869 6464 656e 5f41 413a  at},n_hidden_AA:
+000228b0: 7b73 656c 662e 6e5f 6869 6464 656e 5f41  {self.n_hidden_A
+000228c0: 417d 2c6e 5f68 6964 6465 6e5f 5041 3a7b  A},n_hidden_PA:{
+000228d0: 7365 6c66 2e6e 5f68 6964 6465 6e5f 5041  self.n_hidden_PA
+000228e0: 7d2c 6e5f 6869 6464 656e 5f41 503a 7b73  },n_hidden_AP:{s
+000228f0: 656c 662e 6e5f 6869 6464 656e 5f41 507d  elf.n_hidden_AP}
+00022900: 2c6e 5f68 6964 6465 6e5f 5050 3a7b 7365  ,n_hidden_PP:{se
+00022910: 6c66 2e6e 5f68 6964 6465 6e5f 5050 7d2c  lf.n_hidden_PP},
+00022920: 6261 7463 685f 6e6f 726d 616c 697a 653a  batch_normalize:
+00022930: 7b73 656c 662e 6261 7463 685f 6e6f 726d  {self.batch_norm
+00022940: 616c 697a 657d 2c75 7064 6174 655f 7061  alize},update_pa
+00022950: 6972 3a7b 7365 6c66 2e75 7064 6174 655f  ir:{self.update_
+00022960: 7061 6972 7d2c 696e 6974 3a7b 7365 6c66  pair},init:{self
+00022970: 2e69 6e69 747d 2c61 6374 6976 6174 696f  .init},activatio
+00022980: 6e3a 7b73 656c 662e 6163 7469 7661 7469  n:{self.activati
+00022990: 6f6e 7d29 270a 2020 2020 2020 2020 290a  on})'.        ).
+000229a0: 0a20 2020 2064 6566 2066 6f72 7761 7264  .    def forward
+000229b0: 280a 2020 2020 2020 2020 7365 6c66 2c20  (.        self, 
+000229c0: 696e 7075 7473 3a20 4c69 7374 5b55 6e69  inputs: List[Uni
+000229d0: 6f6e 5b6e 702e 6e64 6172 7261 792c 206e  on[np.ndarray, n
+000229e0: 702e 6e64 6172 7261 792c 206e 702e 6e64  p.ndarray, np.nd
+000229f0: 6172 7261 792c 0a20 2020 2020 2020 2020  array,.         
+00022a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022a10: 2020 2020 2020 2020 6e70 2e6e 6461 7272          np.ndarr
+00022a20: 6179 5d5d 0a20 2020 2029 202d 3e20 4c69  ay]].    ) -> Li
+00022a30: 7374 5b55 6e69 6f6e 5b74 6f72 6368 2e54  st[Union[torch.T
+00022a40: 656e 736f 722c 2074 6f72 6368 2e54 656e  ensor, torch.Ten
+00022a50: 736f 725d 5d3a 0a20 2020 2020 2020 2022  sor]]:.        "
+00022a60: 2222 0a20 2020 2043 7265 6174 6573 2077  "".    Creates w
+00022a70: 6561 7665 2074 656e 736f 7273 2e0a 0a20  eave tensors... 
+00022a80: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
+00022a90: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+00022aa0: 2069 6e70 7574 733a 204c 6973 745b 556e   inputs: List[Un
+00022ab0: 696f 6e5b 6e70 2e6e 6461 7272 6179 2c20  ion[np.ndarray, 
+00022ac0: 6e70 2e6e 6461 7272 6179 2c20 6e70 2e6e  np.ndarray, np.n
+00022ad0: 6461 7272 6179 2c20 6e70 2e6e 6461 7272  darray, np.ndarr
+00022ae0: 6179 5d5d 0a20 2020 2053 686f 756c 6420  ay]].    Should 
+00022af0: 636f 6e74 6169 6e20 3420 7465 6e73 6f72  contain 4 tensor
+00022b00: 7320 5b61 746f 6d5f 6665 6174 7572 6573  s [atom_features
+00022b10: 2c20 7061 6972 5f66 6561 7475 7265 732c  , pair_features,
+00022b20: 2070 6169 725f 7370 6c69 742c 0a20 2020   pair_split,.   
+00022b30: 2061 746f 6d5f 746f 5f70 6169 725d 0a0a   atom_to_pair]..
+00022b40: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
+00022b50: 202d 2d2d 2d2d 2d2d 0a20 2020 204c 6973   -------.    Lis
+00022b60: 745b 556e 696f 6e5b 746f 7263 682e 5465  t[Union[torch.Te
+00022b70: 6e73 6f72 2c20 746f 7263 682e 5465 6e73  nsor, torch.Tens
+00022b80: 6f72 5d5d 0a20 2020 2020 2041 3a20 4174  or]].      A: At
+00022b90: 6f6d 2066 6561 7475 7265 7320 7465 6e73  om features tens
+00022ba0: 6f72 2077 6974 6820 7368 6170 655b 746f  or with shape[to
+00022bb0: 7461 6c5f 6e75 6d5f 6174 6f6d 732c 6174  tal_num_atoms,at
+00022bc0: 6f6d 2066 6561 7475 7265 2073 697a 655d  om feature size]
+00022bd0: 0a20 2020 2020 2050 3a20 5061 6972 2066  .      P: Pair f
+00022be0: 6561 7475 7265 7320 7465 6e73 6f72 2077  eatures tensor w
+00022bf0: 6974 6820 7368 6170 655b 746f 7461 6c20  ith shape[total 
+00022c00: 6e75 6d20 6f66 2070 6169 7273 2c62 6f6e  num of pairs,bon
+00022c10: 6420 6665 6174 7572 6520 7369 7a65 5d0a  d feature size].
+00022c20: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00022c30: 2320 436f 6e76 6572 7469 6e67 2074 6865  # Converting the
+00022c40: 2069 6e70 7574 2074 6f20 746f 7263 6820   input to torch 
+00022c50: 7465 6e73 6f72 730a 2020 2020 2020 2020  tensors.        
+00022c60: 6174 6f6d 5f66 6561 7475 7265 733a 2074  atom_features: t
+00022c70: 6f72 6368 2e54 656e 736f 7220 3d20 746f  orch.Tensor = to
+00022c80: 7263 682e 7465 6e73 6f72 2869 6e70 7574  rch.tensor(input
+00022c90: 735b 305d 290a 2020 2020 2020 2020 7061  s[0]).        pa
+00022ca0: 6972 5f66 6561 7475 7265 733a 2074 6f72  ir_features: tor
+00022cb0: 6368 2e54 656e 736f 7220 3d20 746f 7263  ch.Tensor = torc
+00022cc0: 682e 7465 6e73 6f72 2869 6e70 7574 735b  h.tensor(inputs[
+00022cd0: 315d 290a 0a20 2020 2020 2020 2070 6169  1])..        pai
+00022ce0: 725f 7370 6c69 743a 2074 6f72 6368 2e54  r_split: torch.T
+00022cf0: 656e 736f 7220 3d20 746f 7263 682e 7465  ensor = torch.te
+00022d00: 6e73 6f72 2869 6e70 7574 735b 325d 290a  nsor(inputs[2]).
+00022d10: 2020 2020 2020 2020 6174 6f6d 5f74 6f5f          atom_to_
+00022d20: 7061 6972 3a20 746f 7263 682e 5465 6e73  pair: torch.Tens
+00022d30: 6f72 203d 2074 6f72 6368 2e74 656e 736f  or = torch.tenso
+00022d40: 7228 696e 7075 7473 5b33 5d29 0a0a 2020  r(inputs[3])..  
+00022d50: 2020 2020 2020 6163 7469 7661 7469 6f6e        activation
+00022d60: 203d 2073 656c 662e 6163 7469 7661 7469   = self.activati
+00022d70: 6f6e 5f66 6e0a 0a20 2020 2020 2020 2023  on_fn..        #
+00022d80: 2041 4120 6973 2061 2074 656e 736f 7220   AA is a tensor 
+00022d90: 7769 7468 2073 6861 7065 5b74 6f74 616c  with shape[total
+00022da0: 5f6e 756d 5f61 746f 6d73 2c6e 5f68 6964  _num_atoms,n_hid
+00022db0: 6465 6e5f 4141 5d0a 2020 2020 2020 2020  den_AA].        
+00022dc0: 4141 3a20 746f 7263 682e 5465 6e73 6f72  AA: torch.Tensor
+00022dd0: 203d 2074 6f72 6368 2e6d 6174 6d75 6c28   = torch.matmul(
+00022de0: 6174 6f6d 5f66 6561 7475 7265 732e 7479  atom_features.ty
+00022df0: 7065 2874 6f72 6368 2e66 6c6f 6174 3332  pe(torch.float32
+00022e00: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+00022e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022e20: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00022e30: 575f 4141 2920 2b20 7365 6c66 2e62 5f41  W_AA) + self.b_A
+00022e40: 410a 2020 2020 2020 2020 6966 2073 656c  A.        if sel
+00022e50: 662e 6261 7463 685f 6e6f 726d 616c 697a  f.batch_normaliz
+00022e60: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
+00022e70: 656c 662e 4141 5f62 6e2e 6576 616c 2829  elf.AA_bn.eval()
+00022e80: 0a20 2020 2020 2020 2020 2020 2041 4120  .            AA 
+00022e90: 3d20 7365 6c66 2e41 415f 626e 2841 4129  = self.AA_bn(AA)
+00022ea0: 0a20 2020 2020 2020 2041 4120 3d20 6163  .        AA = ac
+00022eb0: 7469 7661 7469 6f6e 2841 4129 0a20 2020  tivation(AA).   
+00022ec0: 2020 2020 2023 2050 4120 6973 2061 2074       # PA is a t
+00022ed0: 656e 736f 7220 7769 7468 2073 6861 7065  ensor with shape
+00022ee0: 5b74 6f74 616c 206e 756d 6265 7220 6f66  [total number of
+00022ef0: 2070 6169 7273 2c6e 5f68 6964 6465 6e5f   pairs,n_hidden_
+00022f00: 5041 5d0a 2020 2020 2020 2020 5041 3a20  PA].        PA: 
+00022f10: 746f 7263 682e 5465 6e73 6f72 203d 2074  torch.Tensor = t
+00022f20: 6f72 6368 2e6d 6174 6d75 6c28 7061 6972  orch.matmul(pair
+00022f30: 5f66 6561 7475 7265 732e 7479 7065 2874  _features.type(t
+00022f40: 6f72 6368 2e66 6c6f 6174 3332 292c 0a20  orch.float32),. 
+00022f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022f70: 2020 2020 2020 2073 656c 662e 575f 5041         self.W_PA
+00022f80: 2920 2b20 7365 6c66 2e62 5f50 410a 2020  ) + self.b_PA.  
+00022f90: 2020 2020 2020 6966 2073 656c 662e 6261        if self.ba
+00022fa0: 7463 685f 6e6f 726d 616c 697a 653a 0a20  tch_normalize:. 
+00022fb0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00022fc0: 5041 5f62 6e2e 6576 616c 2829 0a20 2020  PA_bn.eval().   
+00022fd0: 2020 2020 2020 2020 2050 4120 3d20 7365           PA = se
+00022fe0: 6c66 2e50 415f 626e 2850 4129 0a20 2020  lf.PA_bn(PA).   
+00022ff0: 2020 2020 2050 4120 3d20 6163 7469 7661       PA = activa
+00023000: 7469 6f6e 2850 4129 0a0a 2020 2020 2020  tion(PA)..      
+00023010: 2020 2320 5370 6c69 7420 7468 6520 5041    # Split the PA
+00023020: 2074 656e 736f 7220 6163 636f 7264 696e   tensor accordin
+00023030: 6720 746f 2074 6865 2027 7061 6972 5f73  g to the 'pair_s
+00023040: 706c 6974 2720 7465 6e73 6f72 0a20 2020  plit' tensor.   
+00023050: 2020 2020 2074 5f67 7270 3a20 4469 6374       t_grp: Dict
+00023060: 5b54 656e 736f 722c 2054 656e 736f 725d  [Tensor, Tensor]
+00023070: 203d 207b 7d0a 2020 2020 2020 2020 6964   = {}.        id
+00023080: 783a 2069 6e74 203d 2030 0a20 2020 2020  x: int = 0.     
+00023090: 2020 2066 6f72 2069 2c20 735f 6964 2069     for i, s_id i
+000230a0: 6e20 656e 756d 6572 6174 6528 7061 6972  n enumerate(pair
+000230b0: 5f73 706c 6974 293a 0a20 2020 2020 2020  _split):.       
+000230c0: 2020 2020 2073 5f69 6420 3d20 735f 6964       s_id = s_id
+000230d0: 2e69 7465 6d28 290a 2020 2020 2020 2020  .item().        
+000230e0: 2020 2020 6966 2073 5f69 6420 696e 2074      if s_id in t
+000230f0: 5f67 7270 3a0a 2020 2020 2020 2020 2020  _grp:.          
+00023100: 2020 2020 2020 745f 6772 705b 735f 6964        t_grp[s_id
+00023110: 5d20 3d20 745f 6772 705b 735f 6964 5d20  ] = t_grp[s_id] 
+00023120: 2b20 5041 5b69 6478 5d0a 2020 2020 2020  + PA[idx].      
+00023130: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00023140: 2020 2020 2020 2020 2020 2020 745f 6772              t_gr
+00023150: 705b 735f 6964 5d20 3d20 5041 5b69 6478  p[s_id] = PA[idx
+00023160: 5d0a 2020 2020 2020 2020 2020 2020 6964  ].            id
+00023170: 7820 3d20 6920 2b20 310a 0a20 2020 2020  x = i + 1..     
+00023180: 2020 2020 2020 206c 7374 203d 206c 6973         lst = lis
+00023190: 7428 745f 6772 702e 7661 6c75 6573 2829  t(t_grp.values()
+000231a0: 290a 2020 2020 2020 2020 2020 2020 7465  ).            te
+000231b0: 6e73 6f72 203d 2074 6f72 6368 2e73 7461  nsor = torch.sta
+000231c0: 636b 286c 7374 290a 2020 2020 2020 2020  ck(lst).        
+000231d0: 5041 203d 2074 656e 736f 720a 0a20 2020  PA = tensor..   
+000231e0: 2020 2020 2041 3a20 746f 7263 682e 5465       A: torch.Te
+000231f0: 6e73 6f72 203d 2074 6f72 6368 2e6d 6174  nsor = torch.mat
+00023200: 6d75 6c28 746f 7263 682e 636f 6e63 6174  mul(torch.concat
+00023210: 285b 4141 2c20 5041 5d2c 2031 292c 0a20  ([AA, PA], 1),. 
+00023220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023240: 2020 2020 2020 7365 6c66 2e57 5f41 2920        self.W_A) 
+00023250: 2b20 7365 6c66 2e62 5f41 0a20 2020 2020  + self.b_A.     
+00023260: 2020 2069 6620 7365 6c66 2e62 6174 6368     if self.batch
+00023270: 5f6e 6f72 6d61 6c69 7a65 3a0a 2020 2020  _normalize:.    
+00023280: 2020 2020 2020 2020 7365 6c66 2e41 5f62          self.A_b
+00023290: 6e2e 6576 616c 2829 0a20 2020 2020 2020  n.eval().       
+000232a0: 2020 2020 2041 203d 2073 656c 662e 415f       A = self.A_
+000232b0: 626e 2841 290a 2020 2020 2020 2020 4120  bn(A).        A 
+000232c0: 3d20 6163 7469 7661 7469 6f6e 2841 290a  = activation(A).
+000232d0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+000232e0: 2e75 7064 6174 655f 7061 6972 3a0a 2020  .update_pair:.  
+000232f0: 2020 2020 2020 2020 2020 2320 4e6f 7465            # Note
+00023300: 2074 6861 7420 4150 5f69 6a20 616e 6420   that AP_ij and 
+00023310: 4150 5f6a 6920 7368 6172 6520 7468 6520  AP_ji share the 
+00023320: 7361 6d65 2073 656c 662e 4150 5f62 6e20  same self.AP_bn 
+00023330: 6261 7463 680a 2020 2020 2020 2020 2020  batch.          
+00023340: 2020 2320 6e6f 726d 616c 697a 6174 696f    # normalizatio
+00023350: 6e0a 2020 2020 2020 2020 2020 2020 4150  n.            AP
+00023360: 5f69 6a3a 2074 6f72 6368 2e54 656e 736f  _ij: torch.Tenso
+00023370: 7220 3d20 746f 7263 682e 6d61 746d 756c  r = torch.matmul
+00023380: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00023390: 2020 746f 7263 682e 7265 7368 6170 6528    torch.reshape(
+000233a0: 6174 6f6d 5f66 6561 7475 7265 735b 6174  atom_features[at
+000233b0: 6f6d 5f74 6f5f 7061 6972 5d2c 0a20 2020  om_to_pair],.   
+000233c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000233d0: 2020 2020 2020 2020 2020 205b 2d31 2c20             [-1, 
+000233e0: 3220 2a20 7365 6c66 2e6e 5f61 746f 6d5f  2 * self.n_atom_
+000233f0: 696e 7075 745f 6665 6174 5d29 2e74 7970  input_feat]).typ
+00023400: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
+00023410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023420: 2020 2020 2074 6f72 6368 2e66 6c6f 6174       torch.float
+00023430: 3332 292c 2073 656c 662e 575f 4150 2920  32), self.W_AP) 
+00023440: 2b20 7365 6c66 2e62 5f41 500a 2020 2020  + self.b_AP.    
+00023450: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00023460: 6261 7463 685f 6e6f 726d 616c 697a 653a  batch_normalize:
+00023470: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00023480: 2073 656c 662e 4150 5f62 6e2e 6576 616c   self.AP_bn.eval
+00023490: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+000234a0: 2020 2041 505f 696a 203d 2073 656c 662e     AP_ij = self.
+000234b0: 4150 5f62 6e28 4150 5f69 6a29 0a20 2020  AP_bn(AP_ij).   
+000234c0: 2020 2020 2020 2020 2041 505f 696a 203d           AP_ij =
+000234d0: 2061 6374 6976 6174 696f 6e28 4150 5f69   activation(AP_i
+000234e0: 6a29 0a20 2020 2020 2020 2020 2020 2041  j).            A
+000234f0: 505f 6a69 3a20 746f 7263 682e 5465 6e73  P_ji: torch.Tens
+00023500: 6f72 203d 2074 6f72 6368 2e6d 6174 6d75  or = torch.matmu
+00023510: 6c28 0a20 2020 2020 2020 2020 2020 2020  l(.             
+00023520: 2020 2074 6f72 6368 2e72 6573 6861 7065     torch.reshape
+00023530: 2861 746f 6d5f 6665 6174 7572 6573 5b74  (atom_features[t
+00023540: 6f72 6368 2e66 6c69 7028 6174 6f6d 5f74  orch.flip(atom_t
+00023550: 6f5f 7061 6972 2c20 5b31 5d29 5d2c 0a20  o_pair, [1])],. 
+00023560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023570: 2020 2020 2020 2020 2020 2020 205b 2d31               [-1
+00023580: 2c20 3220 2a20 7365 6c66 2e6e 5f61 746f  , 2 * self.n_ato
+00023590: 6d5f 696e 7075 745f 6665 6174 5d29 2e74  m_input_feat]).t
+000235a0: 7970 6528 0a20 2020 2020 2020 2020 2020  ype(.           
+000235b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000235c0: 2020 2020 2020 2074 6f72 6368 2e66 6c6f         torch.flo
+000235d0: 6174 3332 292c 2073 656c 662e 575f 4150  at32), self.W_AP
+000235e0: 2920 2b20 7365 6c66 2e62 5f41 500a 2020  ) + self.b_AP.  
+000235f0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00023600: 662e 6261 7463 685f 6e6f 726d 616c 697a  f.batch_normaliz
+00023610: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00023620: 2020 2073 656c 662e 4150 5f62 6e2e 6576     self.AP_bn.ev
+00023630: 616c 2829 0a20 2020 2020 2020 2020 2020  al().           
+00023640: 2020 2020 2041 505f 6a69 203d 2073 656c       AP_ji = sel
+00023650: 662e 4150 5f62 6e28 4150 5f6a 6929 0a20  f.AP_bn(AP_ji). 
+00023660: 2020 2020 2020 2020 2020 2041 505f 6a69             AP_ji
+00023670: 203d 2061 6374 6976 6174 696f 6e28 4150   = activation(AP
+00023680: 5f6a 6929 0a20 2020 2020 2020 2020 2020  _ji).           
+00023690: 2023 2050 5020 6973 2061 2074 656e 736f   # PP is a tenso
+000236a0: 7220 7769 7468 2073 6861 7065 205b 746f  r with shape [to
+000236b0: 7461 6c20 6e75 6d62 6572 206f 6620 7061  tal number of pa
+000236c0: 6972 732c 6e5f 6869 6464 656e 5f50 505d  irs,n_hidden_PP]
+000236d0: 0a20 2020 2020 2020 2020 2020 2050 503a  .            PP:
+000236e0: 2074 6f72 6368 2e54 656e 736f 7220 3d20   torch.Tensor = 
+000236f0: 746f 7263 682e 6d61 746d 756c 2870 6169  torch.matmul(pai
+00023700: 725f 6665 6174 7572 6573 2e74 7970 6528  r_features.type(
+00023710: 746f 7263 682e 666c 6f61 7433 3229 2c0a  torch.float32),.
+00023720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00023740: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00023750: 2e57 5f50 5029 202b 2073 656c 662e 625f  .W_PP) + self.b_
+00023760: 5050 0a20 2020 2020 2020 2020 2020 2069  PP.            i
+00023770: 6620 7365 6c66 2e62 6174 6368 5f6e 6f72  f self.batch_nor
+00023780: 6d61 6c69 7a65 3a0a 2020 2020 2020 2020  malize:.        
+00023790: 2020 2020 2020 2020 7365 6c66 2e50 505f          self.PP_
+000237a0: 626e 2e65 7661 6c28 290a 2020 2020 2020  bn.eval().      
+000237b0: 2020 2020 2020 2020 2020 5050 203d 2073            PP = s
+000237c0: 656c 662e 5050 5f62 6e28 5050 290a 2020  elf.PP_bn(PP).  
+000237d0: 2020 2020 2020 2020 2020 5050 203d 2061            PP = a
+000237e0: 6374 6976 6174 696f 6e28 5050 290a 2020  ctivation(PP).  
+000237f0: 2020 2020 2020 2020 2020 503a 2074 6f72            P: tor
+00023800: 6368 2e54 656e 736f 7220 3d20 746f 7263  ch.Tensor = torc
+00023810: 682e 6d61 746d 756c 280a 2020 2020 2020  h.matmul(.      
+00023820: 2020 2020 2020 2020 2020 746f 7263 682e            torch.
+00023830: 636f 6e63 6174 285b 4150 5f69 6a20 2b20  concat([AP_ij + 
+00023840: 4150 5f6a 692c 2050 505d 2c20 3129 2e74  AP_ji, PP], 1).t
+00023850: 7970 6528 746f 7263 682e 666c 6f61 7433  ype(torch.float3
+00023860: 3229 2c0a 2020 2020 2020 2020 2020 2020  2),.            
+00023870: 2020 2020 7365 6c66 2e57 5f50 2920 2b20      self.W_P) + 
+00023880: 7365 6c66 2e62 5f50 0a20 2020 2020 2020  self.b_P.       
+00023890: 2020 2020 2069 6620 7365 6c66 2e62 6174       if self.bat
+000238a0: 6368 5f6e 6f72 6d61 6c69 7a65 3a0a 2020  ch_normalize:.  
+000238b0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000238c0: 6c66 2e50 5f62 6e2e 6576 616c 2829 0a20  lf.P_bn.eval(). 
+000238d0: 2020 2020 2020 2020 2020 2020 2020 2050                 P
+000238e0: 203d 2073 656c 662e 505f 626e 2850 290a   = self.P_bn(P).
+000238f0: 2020 2020 2020 2020 2020 2020 5020 3d20              P = 
+00023900: 6163 7469 7661 7469 6f6e 2850 290a 2020  activation(P).  
+00023910: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00023920: 2020 2020 2020 2020 5020 3d20 7061 6972          P = pair
+00023930: 5f66 6561 7475 7265 730a 0a20 2020 2020  _features..     
+00023940: 2020 2072 6574 7572 6e20 5b41 2c20 505d     return [A, P]
+00023950: 0a                                       .
```

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/models/torch_models/lcnn.py` & `deepchem-2.7.2.dev20230703203150/deepchem/models/torch_models/lcnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/models/torch_models/mat.py` & `deepchem-2.7.2.dev20230703203150/deepchem/models/torch_models/mat.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/models/torch_models/megnet.py` & `deepchem-2.7.2.dev20230703203150/deepchem/models/torch_models/megnet.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/models/torch_models/modular.py` & `deepchem-2.7.2.dev20230703203150/deepchem/models/torch_models/modular.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/models/torch_models/mpnn.py` & `deepchem-2.7.2.dev20230703203150/deepchem/models/torch_models/mpnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/models/torch_models/normalizing_flows_pytorch.py` & `deepchem-2.7.2.dev20230703203150/deepchem/models/torch_models/normalizing_flows_pytorch.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/models/torch_models/pagtn.py` & `deepchem-2.7.2.dev20230703203150/deepchem/models/torch_models/pagtn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/models/torch_models/pna_gnn.py` & `deepchem-2.7.2.dev20230703203150/deepchem/models/torch_models/pna_gnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/models/torch_models/readout.py` & `deepchem-2.7.2.dev20230703203150/deepchem/models/torch_models/readout.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/models/torch_models/torch_model.py` & `deepchem-2.7.2.dev20230703203150/deepchem/models/torch_models/torch_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/models/wandblogger.py` & `deepchem-2.7.2.dev20230703203150/deepchem/models/wandblogger.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/molnet/__init__.py` & `deepchem-2.7.2.dev20230703203150/deepchem/molnet/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/molnet/check_availability.py` & `deepchem-2.7.2.dev20230703203150/deepchem/molnet/check_availability.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/molnet/defaults.py` & `deepchem-2.7.2.dev20230703203150/deepchem/molnet/defaults.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/molnet/dnasim.py` & `deepchem-2.7.2.dev20230703203150/deepchem/molnet/dnasim.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/bace_datasets.py` & `deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/bace_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/bace_features.py` & `deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/bace_features.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/bbbc_datasets.py` & `deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/bbbc_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/bbbp_datasets.py` & `deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/bbbp_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/cell_counting_datasets.py` & `deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/cell_counting_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/chembl25_datasets.py` & `deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/chembl25_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/chembl_datasets.py` & `deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/chembl_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/chembl_tasks.py` & `deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/chembl_tasks.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/clearance_datasets.py` & `deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/clearance_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/clintox_datasets.py` & `deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/clintox_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/delaney_datasets.py` & `deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/delaney_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/factors_datasets.py` & `deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/factors_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/freesolv_dataset.py` & `deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/freesolv_dataset.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/hiv_datasets.py` & `deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/hiv_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/hopv_datasets.py` & `deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/hopv_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/hppb_datasets.py` & `deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/hppb_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/kaggle_datasets.py` & `deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/kaggle_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/kaggle_features.py` & `deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/kaggle_features.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/kinase_datasets.py` & `deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/kinase_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/lipo_datasets.py` & `deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/lipo_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/load_dataset_template.py` & `deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/load_dataset_template.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/material_datasets/load_Pt_NO_surface_adsorbate_energy.py` & `deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/material_datasets/load_Pt_NO_surface_adsorbate_energy.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/material_datasets/load_bandgap.py` & `deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/material_datasets/load_bandgap.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/material_datasets/load_mp_formation_energy.py` & `deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/material_datasets/load_mp_formation_energy.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/material_datasets/load_mp_metallicity.py` & `deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/material_datasets/load_mp_metallicity.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/material_datasets/load_perovskite.py` & `deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/material_datasets/load_perovskite.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/molnet_loader.py` & `deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/molnet_loader.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/muv_datasets.py` & `deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/muv_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/nci_datasets.py` & `deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/nci_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/pcba_datasets.py` & `deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/pcba_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/pdbbind_datasets.py` & `deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/pdbbind_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/ppb_datasets.py` & `deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/ppb_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/qm7_datasets.py` & `deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/qm7_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/qm8_datasets.py` & `deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/qm8_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/qm9_datasets.py` & `deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/qm9_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/sampl_datasets.py` & `deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/sampl_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/sider_datasets.py` & `deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/sider_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/sweetlead_datasets.py` & `deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/sweetlead_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/thermosol_datasets.py` & `deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/thermosol_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/tox21_datasets.py` & `deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/tox21_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/toxcast_datasets.py` & `deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/toxcast_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/uspto_datasets.py` & `deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/uspto_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/uv_datasets.py` & `deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/uv_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/uv_tasks.py` & `deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/uv_tasks.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/molnet/load_function/zinc15_datasets.py` & `deepchem-2.7.2.dev20230703203150/deepchem/molnet/load_function/zinc15_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/molnet/preset_hyper_parameters.py` & `deepchem-2.7.2.dev20230703203150/deepchem/molnet/preset_hyper_parameters.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/molnet/run_benchmark.py` & `deepchem-2.7.2.dev20230703203150/deepchem/molnet/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/molnet/run_benchmark_low_data.py` & `deepchem-2.7.2.dev20230703203150/deepchem/molnet/run_benchmark_low_data.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/molnet/run_benchmark_models.py` & `deepchem-2.7.2.dev20230703203150/deepchem/molnet/run_benchmark_models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/rl/__init__.py` & `deepchem-2.7.2.dev20230703203150/deepchem/rl/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/rl/a2c.py` & `deepchem-2.7.2.dev20230703203150/deepchem/rl/a2c.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/rl/envs/test_tictactoe.py` & `deepchem-2.7.2.dev20230703203150/deepchem/rl/envs/test_tictactoe.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/rl/envs/tictactoe.py` & `deepchem-2.7.2.dev20230703203150/deepchem/rl/envs/tictactoe.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/rl/ppo.py` & `deepchem-2.7.2.dev20230703203150/deepchem/rl/ppo.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/splits/__init__.py` & `deepchem-2.7.2.dev20230703203150/deepchem/splits/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/splits/splitters.py` & `deepchem-2.7.2.dev20230703203150/deepchem/splits/splitters.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/splits/task_splitter.py` & `deepchem-2.7.2.dev20230703203150/deepchem/splits/task_splitter.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/trans/__init__.py` & `deepchem-2.7.2.dev20230703203150/deepchem/trans/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/trans/duplicate.py` & `deepchem-2.7.2.dev20230703203150/deepchem/trans/duplicate.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/trans/transformers.py` & `deepchem-2.7.2.dev20230703203150/deepchem/trans/transformers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/utils/__init__.py` & `deepchem-2.7.2.dev20230703203150/deepchem/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/utils/conformers.py` & `deepchem-2.7.2.dev20230703203150/deepchem/utils/conformers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/utils/coordinate_box_utils.py` & `deepchem-2.7.2.dev20230703203150/deepchem/utils/coordinate_box_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/utils/data_utils.py` & `deepchem-2.7.2.dev20230703203150/deepchem/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/utils/debug_utils.py` & `deepchem-2.7.2.dev20230703203150/deepchem/utils/debug_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/utils/dftutils.py` & `deepchem-2.7.2.dev20230703203150/deepchem/utils/dftutils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/utils/docking_utils.py` & `deepchem-2.7.2.dev20230703203150/deepchem/utils/docking_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/utils/electron_sampler.py` & `deepchem-2.7.2.dev20230703203150/deepchem/utils/electron_sampler.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/utils/evaluate.py` & `deepchem-2.7.2.dev20230703203150/deepchem/utils/evaluate.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/utils/fake_data_generator.py` & `deepchem-2.7.2.dev20230703203150/deepchem/utils/fake_data_generator.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/utils/fragment_utils.py` & `deepchem-2.7.2.dev20230703203150/deepchem/utils/fragment_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/utils/genomics_utils.py` & `deepchem-2.7.2.dev20230703203150/deepchem/utils/genomics_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/utils/geometry_utils.py` & `deepchem-2.7.2.dev20230703203150/deepchem/utils/geometry_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/utils/graph_utils.py` & `deepchem-2.7.2.dev20230703203150/deepchem/utils/graph_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/utils/grover.py` & `deepchem-2.7.2.dev20230703203150/deepchem/utils/grover.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/utils/hash_utils.py` & `deepchem-2.7.2.dev20230703203150/deepchem/utils/hash_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/utils/molecule_feature_utils.py` & `deepchem-2.7.2.dev20230703203150/deepchem/utils/molecule_feature_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/utils/noncovalent_utils.py` & `deepchem-2.7.2.dev20230703203150/deepchem/utils/noncovalent_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/utils/pdbqt_utils.py` & `deepchem-2.7.2.dev20230703203150/deepchem/utils/pdbqt_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/utils/pytorch_utils.py` & `deepchem-2.7.2.dev20230703203150/deepchem/utils/pytorch_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/utils/rdkit_utils.py` & `deepchem-2.7.2.dev20230703203150/deepchem/utils/rdkit_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/utils/save.py` & `deepchem-2.7.2.dev20230703203150/deepchem/utils/save.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/utils/sequence_utils.py` & `deepchem-2.7.2.dev20230703203150/deepchem/utils/sequence_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/utils/test/test_coordinate_box_utils.py` & `deepchem-2.7.2.dev20230703203150/deepchem/utils/test/test_coordinate_box_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/utils/test/test_data_utils.py` & `deepchem-2.7.2.dev20230703203150/deepchem/utils/test/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/utils/test/test_dftutils.py` & `deepchem-2.7.2.dev20230703203150/deepchem/utils/test/test_dftutils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/utils/test/test_docking_utils.py` & `deepchem-2.7.2.dev20230703203150/deepchem/utils/test/test_docking_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/utils/test/test_electron_sampler.py` & `deepchem-2.7.2.dev20230703203150/deepchem/utils/test/test_electron_sampler.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/utils/test/test_evaluate.py` & `deepchem-2.7.2.dev20230703203150/deepchem/utils/test/test_evaluate.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/utils/test/test_fake_data_generator.py` & `deepchem-2.7.2.dev20230703203150/deepchem/utils/test/test_fake_data_generator.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/utils/test/test_fragment_utils.py` & `deepchem-2.7.2.dev20230703203150/deepchem/utils/test/test_fragment_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/utils/test/test_generator_evaluator.py` & `deepchem-2.7.2.dev20230703203150/deepchem/utils/test/test_generator_evaluator.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/utils/test/test_genomics_utils.py` & `deepchem-2.7.2.dev20230703203150/deepchem/utils/test/test_genomics_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/utils/test/test_geometry_utils.py` & `deepchem-2.7.2.dev20230703203150/deepchem/utils/test/test_geometry_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/utils/test/test_graph_utils.py` & `deepchem-2.7.2.dev20230703203150/deepchem/utils/test/test_graph_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/utils/test/test_grover.py` & `deepchem-2.7.2.dev20230703203150/deepchem/utils/test/test_grover.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/utils/test/test_hash_utils.py` & `deepchem-2.7.2.dev20230703203150/deepchem/utils/test/test_hash_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/utils/test/test_molecule_feature_utils.py` & `deepchem-2.7.2.dev20230703203150/deepchem/utils/test/test_molecule_feature_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/utils/test/test_noncovalent_utils.py` & `deepchem-2.7.2.dev20230703203150/deepchem/utils/test/test_noncovalent_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/utils/test/test_pdbqt_utils.py` & `deepchem-2.7.2.dev20230703203150/deepchem/utils/test/test_pdbqt_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/utils/test/test_pytorch_utils.py` & `deepchem-2.7.2.dev20230703203150/deepchem/utils/test/test_pytorch_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/utils/test/test_rdkit_utils.py` & `deepchem-2.7.2.dev20230703203150/deepchem/utils/test/test_rdkit_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/utils/test/test_sequence_utils.py` & `deepchem-2.7.2.dev20230703203150/deepchem/utils/test/test_sequence_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/utils/test/test_voxel_utils.py` & `deepchem-2.7.2.dev20230703203150/deepchem/utils/test/test_voxel_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/utils/typing.py` & `deepchem-2.7.2.dev20230703203150/deepchem/utils/typing.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/utils/vina_utils.py` & `deepchem-2.7.2.dev20230703203150/deepchem/utils/vina_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem/utils/voxel_utils.py` & `deepchem-2.7.2.dev20230703203150/deepchem/utils/voxel_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem.egg-info/PKG-INFO` & `deepchem-2.7.2.dev20230703203150/deepchem.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepchem
-Version: 2.7.2.dev20230703190634
+Version: 2.7.2.dev20230703203150
 Summary: Deep learning models for drug discovery,         quantum chemistry, and the life sciences.
 Home-page: https://github.com/deepchem/deepchem
 Maintainer: DeepChem contributors
 License: MIT
 Project-URL: Documentation, https://deepchem.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/deepchem/deepchem
 Keywords: deepchem,chemistry,biology,materials-science,life-science,drug-discovery
```

### Comparing `deepchem-2.7.2.dev20230703190634/deepchem.egg-info/SOURCES.txt` & `deepchem-2.7.2.dev20230703203150/deepchem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/setup.cfg` & `deepchem-2.7.2.dev20230703203150/setup.cfg`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230703190634/setup.py` & `deepchem-2.7.2.dev20230703203150/setup.py`

 * *Files identical despite different names*

