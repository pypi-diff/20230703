# Comparing `tmp/returnn-1.20230703.180607.tar.gz` & `tmp/returnn-1.20230703.193930.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/returnn-1.20230703.180607.tar", last modified: Mon Jul  3 16:23:34 2023, max compression
+gzip compressed data, was "dist/returnn-1.20230703.193930.tar", last modified: Mon Jul  3 17:47:15 2023, max compression
```

## Comparing `returnn-1.20230703.180607.tar` & `returnn-1.20230703.193930.tar`

### file list

```diff
@@ -1,450 +1,450 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:23:34.000000 returnn-1.20230703.180607/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/.kateconfig
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-07-03 16:23:34.000000 returnn-1.20230703.180607/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-03 16:23:33.000000 returnn-1.20230703.180607/_setup_info_generated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:23:34.000000 returnn-1.20230703.180607/demos/
--rw-r--r--   0 runner    (1001) docker     (123)    36006 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/demos/12AX.cluster_map
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/demos/_setup_returnn_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/demos/demo-fwd.config
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/demos/demo-horovod-mpi.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/demos/demo-horovod-mpi.py.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/demos/demo-horovod-mpi.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/demos/demo-hyper-param-tuning.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     2396 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/demos/demo-iter-dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3635 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/demos/demo-list-devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/demos/demo-lua-torch-layer.config
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/demos/demo-pretrain.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     2331 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/demos/demo-record-and-push-to-webserver.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1950 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/demos/demo-returnn-as-framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/demos/demo-rf.config
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/demos/demo-rhn-enwik8.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/demos/demo-sprint-interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/demos/demo-tf-att-copy.config
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/demos/demo-tf-attention.config
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/demos/demo-tf-chunking-blstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/demos/demo-tf-contribrnn-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/demos/demo-tf-enc-dec.config
--rwxr-xr-x   0 runner    (1001) docker     (123)    11615 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/demos/demo-tf-hard-att-copy.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     7287 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/demos/demo-tf-lstm-benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/demos/demo-tf-maxgradnorm-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/demos/demo-tf-native-lstm-lowmem.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/demos/demo-tf-native-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/demos/demo-tf-native-lstm2.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/demos/demo-tf-native-lstm2.12ax.tuned.config
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/demos/demo-tf-neural-transducer.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/demos/demo-tf-rec-explicit-lstm.config
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/demos/demo-tf-rec-explicit-rnn.config
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/demos/demo-tf-rec-self-att.config
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/demos/demo-tf-search-compiled-graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/demos/demo-tf-vanilla-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/demos/demo-timit-lstm-ctc.config
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/demos/demo-torch.config
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/demos/demo-upd-mult-model.lstm.12ax.config
--rwxr-xr-x   0 runner    (1001) docker     (123)      651 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/demos/demo.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:23:34.000000 returnn-1.20230703.180607/demos/mdlstm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:23:34.000000 returnn-1.20230703.180607/demos/mdlstm/IAM/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:23:34.000000 returnn-1.20230703.180607/demos/mdlstm/IAM/IAM_lines/
--rwxr-xr-x   0 runner    (1001) docker     (123)    43239 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    43552 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/demos/mdlstm/IAM/IAM_lines/a01-007-04.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    45111 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/demos/mdlstm/IAM/IAM_lines/a01-007-06.png
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/demos/mdlstm/IAM/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/demos/mdlstm/IAM/chars.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/demos/mdlstm/IAM/config_demo
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/demos/mdlstm/IAM/config_fwd
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/demos/mdlstm/IAM/config_real
--rwxr-xr-x   0 runner    (1001) docker     (123)    10194 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/demos/mdlstm/IAM/create_IAM_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      749 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/demos/mdlstm/IAM/decode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:23:34.000000 returnn-1.20230703.180607/demos/mdlstm/IAM/features/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:23:34.000000 returnn-1.20230703.180607/demos/mdlstm/IAM/features/raw/
--rw-r--r--   0 runner    (1001) docker     (123)   248580 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/demos/mdlstm/IAM/features/raw/demo.h5
--rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/demos/mdlstm/IAM/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/demos/mdlstm/IAM/lines.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:23:34.000000 returnn-1.20230703.180607/demos/mdlstm/IAM/split/
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/demos/mdlstm/IAM/split/eval.txt
--rw-r--r--   0 runner    (1001) docker     (123)    69536 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/demos/mdlstm/IAM/split/train.txt
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/demos/mdlstm/IAM/split/valid.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/demos/mdlstm/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:23:34.000000 returnn-1.20230703.180607/demos/mdlstm/artificial/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2804 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/demos/mdlstm/artificial/create_test_h5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/demos/mdlstm/artificial/forwardconfig
--rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/demos/mdlstm/artificial/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/demos/mdlstm/artificial/trainconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:23:34.000000 returnn-1.20230703.180607/demos/mdlstm/artificial_rgb/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2966 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/demos/mdlstm/artificial_rgb/create_test_h5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/demos/mdlstm/artificial_rgb/forwardconfig
--rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/demos/mdlstm/artificial_rgb/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/demos/mdlstm/artificial_rgb/trainconfig
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:23:34.000000 returnn-1.20230703.180607/returnn/
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25926 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/__old_mod_loader__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/__setup__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24267 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:23:34.000000 returnn-1.20230703.180607/returnn/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/datasets/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)    63188 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/datasets/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/datasets/bundle_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    24892 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/datasets/cached.py
--rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/datasets/cached2.py
--rw-r--r--   0 runner    (1001) docker     (123)    94213 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/datasets/generating.py
--rw-r--r--   0 runner    (1001) docker     (123)    65113 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/datasets/hdf.py
--rw-r--r--   0 runner    (1001) docker     (123)    85120 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/datasets/lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/datasets/map.py
--rw-r--r--   0 runner    (1001) docker     (123)    76099 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/datasets/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    11167 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/datasets/multi_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14596 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/datasets/normalization_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/datasets/numpy_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/datasets/raw_wav.py
--rw-r--r--   0 runner    (1001) docker     (123)    56015 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/datasets/sprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/datasets/stereo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:23:34.000000 returnn-1.20230703.180607/returnn/datasets/util/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/datasets/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23915 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/datasets/util/feature_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)    20445 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/datasets/util/vocabulary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:23:34.000000 returnn-1.20230703.180607/returnn/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9920 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/engine/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/engine/batch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:23:34.000000 returnn-1.20230703.180607/returnn/extern/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:23:34.000000 returnn-1.20230703.180607/returnn/extern/WarpRna/
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/extern/WarpRna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/extern/WarpRna/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:23:34.000000 returnn-1.20230703.180607/returnn/extern/WarpRna/warp-rna/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-03 16:23:09.000000 returnn-1.20230703.180607/returnn/extern/WarpRna/warp-rna/.git
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-03 16:23:13.000000 returnn-1.20230703.180607/returnn/extern/WarpRna/warp-rna/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-03 16:23:13.000000 returnn-1.20230703.180607/returnn/extern/WarpRna/warp-rna/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-03 16:23:13.000000 returnn-1.20230703.180607/returnn/extern/WarpRna/warp-rna/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    13770 2023-07-03 16:23:13.000000 returnn-1.20230703.180607/returnn/extern/WarpRna/warp-rna/aligner.gif
--rw-r--r--   0 runner    (1001) docker     (123)    51077 2023-07-03 16:23:13.000000 returnn-1.20230703.180607/returnn/extern/WarpRna/warp-rna/check.png
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-07-03 16:23:13.000000 returnn-1.20230703.180607/returnn/extern/WarpRna/warp-rna/core.cu
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-03 16:23:13.000000 returnn-1.20230703.180607/returnn/extern/WarpRna/warp-rna/core.h
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-07-03 16:23:13.000000 returnn-1.20230703.180607/returnn/extern/WarpRna/warp-rna/core_cpu.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:23:34.000000 returnn-1.20230703.180607/returnn/extern/WarpRna/warp-rna/pytorch_binding/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-03 16:23:13.000000 returnn-1.20230703.180607/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-03 16:23:13.000000 returnn-1.20230703.180607/returnn/extern/WarpRna/warp-rna/pytorch_binding/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-07-03 16:23:13.000000 returnn-1.20230703.180607/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-07-03 16:23:13.000000 returnn-1.20230703.180607/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-07-03 16:23:13.000000 returnn-1.20230703.180607/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-03 16:23:13.000000 returnn-1.20230703.180607/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-03 16:23:13.000000 returnn-1.20230703.180607/returnn/extern/WarpRna/warp-rna/pytorch_binding/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-03 16:23:13.000000 returnn-1.20230703.180607/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:23:34.000000 returnn-1.20230703.180607/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-07-03 16:23:13.000000 returnn-1.20230703.180607/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-07-03 16:23:13.000000 returnn-1.20230703.180607/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-07-03 16:23:13.000000 returnn-1.20230703.180607/returnn/extern/WarpRna/warp-rna/ref_rna.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:23:34.000000 returnn-1.20230703.180607/returnn/extern/WarpRna/warp-rna/tensorflow_binding/
--rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-07-03 16:23:13.000000 returnn-1.20230703.180607/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:23:34.000000 returnn-1.20230703.180607/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-07-03 16:23:13.000000 returnn-1.20230703.180607/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-07-03 16:23:13.000000 returnn-1.20230703.180607/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:23:34.000000 returnn-1.20230703.180607/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-03 16:23:13.000000 returnn-1.20230703.180607/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-07-03 16:23:13.000000 returnn-1.20230703.180607/returnn/extern/WarpRna/warp-rna/test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/extern/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:23:34.000000 returnn-1.20230703.180607/returnn/extern/graph_editor/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/extern/graph_editor/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/extern/graph_editor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/extern/graph_editor/edit.py
--rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/extern/graph_editor/reroute.py
--rw-r--r--   0 runner    (1001) docker     (123)    29772 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/extern/graph_editor/select.py
--rw-r--r--   0 runner    (1001) docker     (123)    26578 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/extern/graph_editor/subgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)    30380 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/extern/graph_editor/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/extern/graph_editor/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/forward_iface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:23:34.000000 returnn-1.20230703.180607/returnn/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40460 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/frontend/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/frontend/_numpy_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/frontend/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    21015 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/frontend/array_.py
--rw-r--r--   0 runner    (1001) docker     (123)    20878 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/frontend/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/frontend/cond.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/frontend/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/frontend/container.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/frontend/control_flow_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)    22357 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/frontend/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/frontend/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/frontend/dims.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/frontend/dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/frontend/dtype.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:23:34.000000 returnn-1.20230703.180607/returnn/frontend/encoder/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/frontend/encoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/frontend/encoder/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15428 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/frontend/encoder/conformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/frontend/gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/frontend/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/frontend/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)    15485 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/frontend/loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/frontend/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    13738 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/frontend/math_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/frontend/matmul.py
--rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/frontend/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/frontend/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/frontend/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11035 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/frontend/rand.py
--rw-r--r--   0 runner    (1001) docker     (123)     7528 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/frontend/rec.py
--rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/frontend/reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)    17654 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/frontend/run_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/frontend/signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/frontend/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/frontend/tensor_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/frontend/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:23:34.000000 returnn-1.20230703.180607/returnn/import_/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/import_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/import_/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/import_/git.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/import_/import_.py
--rw-r--r--   0 runner    (1001) docker     (123)    33063 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/learning_rate_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    12235 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    35760 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/native_op.cpp
--rw-r--r--   0 runner    (1001) docker     (123)   244393 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/native_op.py
--rw-r--r--   0 runner    (1001) docker     (123)    23542 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/pretrain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:23:34.000000 returnn-1.20230703.180607/returnn/sprint/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/sprint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31545 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/sprint/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    31137 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/sprint/control.py
--rw-r--r--   0 runner    (1001) docker     (123)    23313 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/sprint/error_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/sprint/extern_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    36475 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/sprint/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:23:34.000000 returnn-1.20230703.180607/returnn/tensor/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/tensor/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/tensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   100183 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/tensor/_dim_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)   158177 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/tensor/_tensor_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/tensor/_tensor_mixin_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/tensor/_tensor_op_overloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/tensor/control_flow_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/tensor/dim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/tensor/marked_dim.py
--rw-r--r--   0 runner    (1001) docker     (123)     7680 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/tensor/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/tensor/tensor_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/tensor/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:23:34.000000 returnn-1.20230703.180607/returnn/tf/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/tf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/tf/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    36646 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/tf/data_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/tf/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)   152240 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/tf/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:23:34.000000 returnn-1.20230703.180607/returnn/tf/frontend_layers/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/tf/frontend_layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40440 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/tf/frontend_layers/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/tf/frontend_layers/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14297 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/tf/frontend_layers/cond.py
--rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/tf/frontend_layers/config_entry_points.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/tf/frontend_layers/debug_eager_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/tf/frontend_layers/dims.py
--rw-r--r--   0 runner    (1001) docker     (123)    71987 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/tf/frontend_layers/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15829 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/tf/frontend_layers/make_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/tf/frontend_layers/parameter_assign.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/tf/frontend_layers/prev_tensor_ref.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:23:34.000000 returnn-1.20230703.180607/returnn/tf/frontend_low_level/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/tf/frontend_low_level/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20261 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/tf/frontend_low_level/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/tf/horovod.py
--rw-r--r--   0 runner    (1001) docker     (123)    31611 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/tf/hyper_param_tuning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:23:34.000000 returnn-1.20230703.180607/returnn/tf/layers/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/tf/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   151302 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/tf/layers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)   586746 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/tf/layers/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)   544125 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/tf/layers/rec.py
--rw-r--r--   0 runner    (1001) docker     (123)    21515 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/tf/layers/segmental_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    52409 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/tf/layers/signal_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/tf/layers/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)    79733 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/tf/native_op.py
--rw-r--r--   0 runner    (1001) docker     (123)   224089 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/tf/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/tf/sprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    71539 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/tf/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:23:34.000000 returnn-1.20230703.180607/returnn/tf/util/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/tf/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   302020 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/tf/util/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    28839 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/tf/util/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/tf/util/gradient_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/tf/util/ken_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/tf/util/open_fst.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:23:34.000000 returnn-1.20230703.180607/returnn/torch/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/torch/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:23:34.000000 returnn-1.20230703.180607/returnn/torch/data/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/torch/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11981 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/torch/data/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/torch/data/returnn_dataset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/torch/data/tensor_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6338 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/torch/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)    35646 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/torch/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:23:34.000000 returnn-1.20230703.180607/returnn/torch/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/torch/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    72979 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/torch/frontend/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/torch/frontend/_rand.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/torch/frontend/bridge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:23:34.000000 returnn-1.20230703.180607/returnn/torch/functional/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/torch/functional/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/torch/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11633 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/torch/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:23:34.000000 returnn-1.20230703.180607/returnn/util/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   145021 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/util/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    59572 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/util/better_exchook.py
--rw-r--r--   0 runner    (1001) docker     (123)    17977 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/util/bpe.py
--rw-r--r--   0 runner    (1001) docker     (123)    15987 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/util/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/util/debug_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    59177 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/util/fsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/util/literal_py_to_pickle.py
--rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/util/pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/util/py-to-pickle.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/util/py_compat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7273 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/util/sig_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)    27230 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/returnn/util/task_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:23:34.000000 returnn-1.20230703.180607/returnn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-07-03 16:23:33.000000 returnn-1.20230703.180607/returnn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12544 2023-07-03 16:23:33.000000 returnn-1.20230703.180607/returnn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 16:23:33.000000 returnn-1.20230703.180607/returnn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-03 16:23:33.000000 returnn-1.20230703.180607/returnn.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      461 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 16:23:34.000000 returnn-1.20230703.180607/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:23:34.000000 returnn-1.20230703.180607/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3392 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/DummySprintExec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/PyCharm-inspection-profile.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:23:34.000000 returnn-1.20230703.180607/tests/PyCharm.idea/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/PyCharm.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/PyCharm.idea/.name
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/PyCharm.idea/codeStyleSettings.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:23:34.000000 returnn-1.20230703.180607/tests/PyCharm.idea/codeStyles/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/PyCharm.idea/codeStyles/Project.xml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/PyCharm.idea/codeStyles/codeStyleConfig.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:23:34.000000 returnn-1.20230703.180607/tests/PyCharm.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/PyCharm.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/PyCharm.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/PyCharm.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/PyCharm.idea/returnn.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:23:34.000000 returnn-1.20230703.180607/tests/PyCharm.idea/scopes/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/PyCharm.idea/scopes/scope_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/_set_num_threads1.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/_setup_returnn_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/_setup_test_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/bpe-unicode-demo.codes
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/bpe-unicode-demo.vocab
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/lexicon_opt.fst
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/lexicon_opt.isyms
--rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/lexicon_opt.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/lexicon_opt.osyms
--rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/lint_common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29203 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/pycharm-inspect.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2960 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/pylint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/returnn-as-framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     9228 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/rf_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/spelling.dic
--rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/test_Config.py
--rw-r--r--   0 runner    (1001) docker     (123)    18921 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/test_Dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13634 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/test_Fsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/test_GeneratingDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    32796 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/test_HDFDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10326 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/test_LearningRateControl.py
--rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/test_Log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/test_MultiProcDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/test_PTDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/test_Pretrain.py
--rw-r--r--   0 runner    (1001) docker     (123)    21403 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/test_ResNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/test_SprintDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/test_SprintInterface.py
--rw-r--r--   0 runner    (1001) docker     (123)   238033 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/test_TFEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)   135453 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/test_TFNativeOp.py
--rw-r--r--   0 runner    (1001) docker     (123)   555550 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/test_TFNetworkLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)   567625 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/test_TFNetworkRecLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/test_TFNetworkSigProcLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    20312 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/test_TFUpdater.py
--rw-r--r--   0 runner    (1001) docker     (123)   188146 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/test_TFUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/test_TF_determinism.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/test_TaskSystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/test_TaskSystem_SharedMem.py
--rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/test_TranslationDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/test_Util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11304 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/test_demos.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/test_fork_exec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/test_hdf_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/test_rf_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/test_rf_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/test_rf_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/test_rf_cond.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/test_rf_const.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/test_rf_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    11673 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/test_rf_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/test_rf_encoder_conformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/test_rf_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/test_rf_math.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/test_rf_normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)    15470 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/test_rf_rec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/test_rf_reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/test_rf_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/test_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/test_torch_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    15594 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/test_torch_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tests/test_torch_internal_frontend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:23:34.000000 returnn-1.20230703.180607/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tools/_setup_returnn_env.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9650 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tools/analyze-dataset-batches.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3943 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tools/bliss-collect-seq-lens.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      780 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tools/bliss-dump-text.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6608 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tools/bliss-get-segment-names.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18221 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tools/bliss-to-ogg-zip.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5644 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tools/bpe-create-lexicon.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10532 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tools/calculate-word-error-rate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1759 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tools/cleanup-old-models.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10783 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tools/collect-orth-symbols.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6801 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tools/collect-words.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4395 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tools/compile_native_op.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    81620 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tools/compile_tf_graph.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8500 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tools/debug-dump-search-scores.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    47001 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tools/debug-plot-search-scores.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6048 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tools/dump-dataset-raw-strings.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12524 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tools/dump-dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5770 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tools/dump-forward-stats.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2576 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tools/dump-forward.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tools/dump-network-json.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      719 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tools/dump-pickle.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16425 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tools/extract_state_tying_from_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14986 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tools/get-attention-weights.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2936 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tools/get-best-model-epoch.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3900 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tools/hdf_dump.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19622 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tools/hdf_dump_translation_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    49563 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tools/import-blocks-mt-model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    31498 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tools/import-t2t-mt-model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:23:34.000000 returnn-1.20230703.180607/tools/lattice_rescorer/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tools/lattice_rescorer/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tools/lattice_rescorer/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tools/lattice_rescorer/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:23:34.000000 returnn-1.20230703.180607/tools/lattice_rescorer/example/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tools/lattice_rescorer/example/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tools/lattice_rescorer/example/libs_list
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:23:34.000000 returnn-1.20230703.180607/tools/lattice_rescorer/example/network.040/
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config
--rwxr-xr-x   0 runner    (1001) docker     (123)      800 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tools/lattice_rescorer/example/rescore_lattice.sh
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tools/lattice_rescorer/example/state_vars_list
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tools/lattice_rescorer/example/tensor_names_list
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tools/lattice_rescorer/file.h
--rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tools/lattice_rescorer/htklatticerescorer.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tools/lattice_rescorer/htklatticerescorer.h
--rw-r--r--   0 runner    (1001) docker     (123)    12488 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tools/lattice_rescorer/main.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tools/lattice_rescorer/rescorer.h
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tools/lattice_rescorer/vocabulary.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tools/lattice_rescorer/vocabulary.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     5438 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tools/tf_avg_checkpoints.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6269 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tools/tf_inspect_checkpoint.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1288 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tools/tf_inspect_summary_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-07-03 16:23:07.000000 returnn-1.20230703.180607/tools/torch_export_to_onnx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/.kateconfig
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/_setup_info_generated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/demos/
+-rw-r--r--   0 runner    (1001) docker     (123)    36006 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/12AX.cluster_map
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/_setup_returnn_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-fwd.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-horovod-mpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-horovod-mpi.py.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-horovod-mpi.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-hyper-param-tuning.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2396 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-iter-dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3635 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-list-devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-lua-torch-layer.config
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-pretrain.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2331 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-record-and-push-to-webserver.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1950 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-returnn-as-framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-rf.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-rhn-enwik8.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-sprint-interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-tf-att-copy.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-tf-attention.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-tf-chunking-blstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-tf-contribrnn-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-tf-enc-dec.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11615 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-tf-hard-att-copy.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7287 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-tf-lstm-benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-tf-maxgradnorm-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-tf-native-lstm-lowmem.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-tf-native-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-tf-native-lstm2.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-tf-native-lstm2.12ax.tuned.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-tf-neural-transducer.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-tf-rec-explicit-lstm.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-tf-rec-explicit-rnn.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-tf-rec-self-att.config
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-tf-search-compiled-graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-tf-vanilla-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-timit-lstm-ctc.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-torch.config
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo-upd-mult-model.lstm.12ax.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)      651 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/demo.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/demos/mdlstm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/demos/mdlstm/IAM/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/demos/mdlstm/IAM/IAM_lines/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43239 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43552 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/mdlstm/IAM/IAM_lines/a01-007-04.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    45111 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/mdlstm/IAM/IAM_lines/a01-007-06.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/mdlstm/IAM/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/mdlstm/IAM/chars.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/mdlstm/IAM/config_demo
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/mdlstm/IAM/config_fwd
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/mdlstm/IAM/config_real
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10194 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/mdlstm/IAM/create_IAM_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      749 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/mdlstm/IAM/decode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/demos/mdlstm/IAM/features/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/demos/mdlstm/IAM/features/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)   248580 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/mdlstm/IAM/features/raw/demo.h5
+-rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/mdlstm/IAM/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/mdlstm/IAM/lines.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/demos/mdlstm/IAM/split/
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/mdlstm/IAM/split/eval.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    69536 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/mdlstm/IAM/split/train.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/mdlstm/IAM/split/valid.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/mdlstm/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/demos/mdlstm/artificial/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2804 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/mdlstm/artificial/create_test_h5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/mdlstm/artificial/forwardconfig
+-rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/mdlstm/artificial/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/mdlstm/artificial/trainconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/demos/mdlstm/artificial_rgb/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2966 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/mdlstm/artificial_rgb/create_test_h5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/mdlstm/artificial_rgb/forwardconfig
+-rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/mdlstm/artificial_rgb/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/demos/mdlstm/artificial_rgb/trainconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25926 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/__old_mod_loader__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/__setup__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24267 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/datasets/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63188 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/datasets/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/datasets/bundle_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24892 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/datasets/cached.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/datasets/cached2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94213 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/datasets/generating.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65113 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/datasets/hdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85120 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/datasets/lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/datasets/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76099 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/datasets/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11167 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/datasets/multi_proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14596 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/datasets/normalization_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/datasets/numpy_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/datasets/raw_wav.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56015 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/datasets/sprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/datasets/stereo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn/datasets/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/datasets/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23915 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/datasets/util/feature_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20445 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/datasets/util/vocabulary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9920 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/engine/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/engine/batch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn/extern/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/.git
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-03 17:47:00.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-03 17:47:00.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-03 17:47:00.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13770 2023-07-03 17:47:00.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/aligner.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    51077 2023-07-03 17:47:00.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/check.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-07-03 17:47:00.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/core.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-03 17:47:00.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/core.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-07-03 17:47:00.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/core_cpu.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/pytorch_binding/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-03 17:47:00.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-03 17:47:00.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/pytorch_binding/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-07-03 17:47:00.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-07-03 17:47:00.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-07-03 17:47:00.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-03 17:47:00.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-03 17:47:00.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/pytorch_binding/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-03 17:47:00.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-07-03 17:47:00.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-07-03 17:47:00.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-07-03 17:47:00.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/ref_rna.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/tensorflow_binding/
+-rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-07-03 17:47:00.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-07-03 17:47:00.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-07-03 17:47:00.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-03 17:47:00.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-07-03 17:47:00.000000 returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/extern/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn/extern/graph_editor/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/extern/graph_editor/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/extern/graph_editor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/extern/graph_editor/edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/extern/graph_editor/reroute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29772 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/extern/graph_editor/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26578 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/extern/graph_editor/subgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30380 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/extern/graph_editor/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/extern/graph_editor/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/forward_iface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40460 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/_numpy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21015 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/array_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20878 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/cond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/control_flow_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22357 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/dims.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/dtype.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn/frontend/encoder/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/encoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/encoder/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15428 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/encoder/conformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15485 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13738 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/math_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/matmul.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11035 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7528 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/rec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17654 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/run_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/tensor_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/frontend/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn/import_/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/import_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/import_/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/import_/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/import_/import_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33063 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/learning_rate_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12235 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35760 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/native_op.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)   244393 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/native_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23542 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/pretrain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn/sprint/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/sprint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31545 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/sprint/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31137 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/sprint/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23313 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/sprint/error_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/sprint/extern_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36475 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/sprint/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn/tensor/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tensor/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100183 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tensor/_dim_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)   158177 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tensor/_tensor_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tensor/_tensor_mixin_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tensor/_tensor_op_overloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tensor/control_flow_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tensor/dim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tensor/marked_dim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7680 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tensor/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tensor/tensor_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tensor/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn/tf/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36646 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/data_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)   152240 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn/tf/frontend_layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/frontend_layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40440 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/frontend_layers/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/frontend_layers/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14297 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/frontend_layers/cond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/frontend_layers/config_entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/frontend_layers/debug_eager_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/frontend_layers/dims.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71987 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/frontend_layers/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15829 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/frontend_layers/make_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/frontend_layers/parameter_assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/frontend_layers/prev_tensor_ref.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn/tf/frontend_low_level/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/frontend_low_level/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20261 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/frontend_low_level/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/horovod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31611 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/hyper_param_tuning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn/tf/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   151302 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/layers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)   586746 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/layers/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)   544225 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/layers/rec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21515 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/layers/segmental_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52409 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/layers/signal_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/layers/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79733 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/native_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)   224089 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/sprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71539 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn/tf/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   302020 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/util/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28839 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/util/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/util/gradient_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/util/ken_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/tf/util/open_fst.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/torch/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn/torch/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/torch/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11981 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/torch/data/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/torch/data/returnn_dataset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/torch/data/tensor_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6338 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/torch/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35646 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/torch/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn/torch/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/torch/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72979 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/torch/frontend/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/torch/frontend/_rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/torch/frontend/bridge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn/torch/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/torch/functional/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/torch/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11633 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/torch/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   144901 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/util/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59572 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/util/better_exchook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17977 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/util/bpe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15987 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/util/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/util/debug_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    59177 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/util/fsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/util/literal_py_to_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/util/pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/util/py-to-pickle.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/util/py_compat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7273 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/util/sig_proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27230 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/returnn/util/task_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12544 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/returnn.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      461 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3392 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/DummySprintExec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/PyCharm-inspection-profile.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/tests/PyCharm.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/PyCharm.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/PyCharm.idea/.name
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/PyCharm.idea/codeStyleSettings.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/tests/PyCharm.idea/codeStyles/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/PyCharm.idea/codeStyles/Project.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/PyCharm.idea/codeStyles/codeStyleConfig.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/tests/PyCharm.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/PyCharm.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/PyCharm.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/PyCharm.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/PyCharm.idea/returnn.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/tests/PyCharm.idea/scopes/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/PyCharm.idea/scopes/scope_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/_set_num_threads1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/_setup_returnn_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/_setup_test_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/bpe-unicode-demo.codes
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/bpe-unicode-demo.vocab
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/lexicon_opt.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/lexicon_opt.isyms
+-rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/lexicon_opt.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/lexicon_opt.osyms
+-rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/lint_common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29203 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/pycharm-inspect.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2960 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/pylint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/returnn-as-framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9228 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/rf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/spelling.dic
+-rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18921 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_Dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13634 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_Fsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_GeneratingDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32796 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_HDFDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10326 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_LearningRateControl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_Log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_MultiProcDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_PTDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_Pretrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21403 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_ResNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_SprintDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_SprintInterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)   238033 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_TFEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)   135453 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_TFNativeOp.py
+-rw-r--r--   0 runner    (1001) docker     (123)   555550 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_TFNetworkLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)   568467 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_TFNetworkRecLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_TFNetworkSigProcLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20312 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_TFUpdater.py
+-rw-r--r--   0 runner    (1001) docker     (123)   188146 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_TFUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_TF_determinism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_TaskSystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_TaskSystem_SharedMem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_TranslationDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_Util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11304 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_demos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_fork_exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_hdf_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_rf_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_rf_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_rf_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_rf_cond.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_rf_const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_rf_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11673 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_rf_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_rf_encoder_conformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_rf_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_rf_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_rf_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15470 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_rf_rec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_rf_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_rf_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_torch_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15594 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_torch_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tests/test_torch_internal_frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/_setup_returnn_env.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9650 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/analyze-dataset-batches.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3943 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/bliss-collect-seq-lens.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      780 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/bliss-dump-text.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6608 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/bliss-get-segment-names.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18221 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/bliss-to-ogg-zip.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5644 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/bpe-create-lexicon.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10532 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/calculate-word-error-rate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1759 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/cleanup-old-models.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10783 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/collect-orth-symbols.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6801 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/collect-words.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4395 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/compile_native_op.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    81620 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/compile_tf_graph.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8500 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/debug-dump-search-scores.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    47001 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/debug-plot-search-scores.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6048 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/dump-dataset-raw-strings.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12524 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/dump-dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5770 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/dump-forward-stats.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2576 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/dump-forward.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/dump-network-json.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      719 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/dump-pickle.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16425 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/extract_state_tying_from_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14986 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/get-attention-weights.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2936 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/get-best-model-epoch.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3900 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/hdf_dump.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19622 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/hdf_dump_translation_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    49563 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/import-blocks-mt-model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31498 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/import-t2t-mt-model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/tools/lattice_rescorer/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/lattice_rescorer/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/lattice_rescorer/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/lattice_rescorer/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/tools/lattice_rescorer/example/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/lattice_rescorer/example/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/lattice_rescorer/example/libs_list
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 17:47:15.000000 returnn-1.20230703.193930/tools/lattice_rescorer/example/network.040/
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)      800 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/lattice_rescorer/example/rescore_lattice.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/lattice_rescorer/example/state_vars_list
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/lattice_rescorer/example/tensor_names_list
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/lattice_rescorer/file.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/lattice_rescorer/htklatticerescorer.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/lattice_rescorer/htklatticerescorer.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12488 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/lattice_rescorer/main.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/lattice_rescorer/rescorer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/lattice_rescorer/vocabulary.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/lattice_rescorer/vocabulary.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5438 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/tf_avg_checkpoints.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6269 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/tf_inspect_checkpoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1288 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/tf_inspect_summary_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-07-03 17:46:57.000000 returnn-1.20230703.193930/tools/torch_export_to_onnx.py
```

### Comparing `returnn-1.20230703.180607/.gitignore` & `returnn-1.20230703.193930/.gitignore`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/.gitmodules` & `returnn-1.20230703.193930/.gitmodules`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/CHANGELOG.md` & `returnn-1.20230703.193930/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/CODEOWNERS` & `returnn-1.20230703.193930/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/CONTRIBUTING.md` & `returnn-1.20230703.193930/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/LICENSE` & `returnn-1.20230703.193930/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/MANIFEST.in` & `returnn-1.20230703.193930/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/PKG-INFO` & `returnn-1.20230703.193930/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: returnn
-Version: 1.20230703.180607
+Version: 1.20230703.193930
 Summary: The RWTH extensible training framework for universal recurrent neural networks
 Home-page: https://github.com/rwth-i6/returnn/
 Author: Albert Zeyer
 Author-email: albzey@gmail.com
 License: RETURNN license
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `returnn-1.20230703.180607/README.rst` & `returnn-1.20230703.193930/README.rst`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/__init__.py` & `returnn-1.20230703.193930/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/demos/12AX.cluster_map` & `returnn-1.20230703.193930/demos/12AX.cluster_map`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/demos/demo-fwd.config` & `returnn-1.20230703.193930/demos/demo-fwd.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/demos/demo-horovod-mpi.py` & `returnn-1.20230703.193930/demos/demo-horovod-mpi.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/demos/demo-horovod-mpi.py.sh` & `returnn-1.20230703.193930/demos/demo-horovod-mpi.py.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/demos/demo-hyper-param-tuning.config` & `returnn-1.20230703.193930/demos/demo-hyper-param-tuning.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/demos/demo-iter-dataset.py` & `returnn-1.20230703.193930/demos/demo-iter-dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/demos/demo-list-devices.py` & `returnn-1.20230703.193930/demos/demo-list-devices.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/demos/demo-lua-torch-layer.config` & `returnn-1.20230703.193930/demos/demo-lua-torch-layer.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/demos/demo-record-and-push-to-webserver.py` & `returnn-1.20230703.193930/demos/demo-record-and-push-to-webserver.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/demos/demo-returnn-as-framework.py` & `returnn-1.20230703.193930/demos/demo-returnn-as-framework.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/demos/demo-rf.config` & `returnn-1.20230703.193930/demos/demo-rf.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/demos/demo-rhn-enwik8.config` & `returnn-1.20230703.193930/demos/demo-rhn-enwik8.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/demos/demo-sprint-interface.py` & `returnn-1.20230703.193930/demos/demo-sprint-interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/demos/demo-tf-att-copy.config` & `returnn-1.20230703.193930/demos/demo-tf-att-copy.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/demos/demo-tf-attention.config` & `returnn-1.20230703.193930/demos/demo-tf-attention.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/demos/demo-tf-chunking-blstm.12ax.config` & `returnn-1.20230703.193930/demos/demo-tf-chunking-blstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/demos/demo-tf-contribrnn-lstm.12ax.config` & `returnn-1.20230703.193930/demos/demo-tf-contribrnn-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/demos/demo-tf-enc-dec.config` & `returnn-1.20230703.193930/demos/demo-tf-enc-dec.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/demos/demo-tf-hard-att-copy.config` & `returnn-1.20230703.193930/demos/demo-tf-hard-att-copy.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/demos/demo-tf-lstm-benchmark.py` & `returnn-1.20230703.193930/demos/demo-tf-lstm-benchmark.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/demos/demo-tf-maxgradnorm-lstm.12ax.config` & `returnn-1.20230703.193930/demos/demo-tf-maxgradnorm-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/demos/demo-tf-native-lstm-lowmem.12ax.config` & `returnn-1.20230703.193930/demos/demo-tf-native-lstm-lowmem.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/demos/demo-tf-native-lstm.12ax.config` & `returnn-1.20230703.193930/demos/demo-tf-native-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/demos/demo-tf-native-lstm2.12ax.config` & `returnn-1.20230703.193930/demos/demo-tf-native-lstm2.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/demos/demo-tf-native-lstm2.12ax.tuned.config` & `returnn-1.20230703.193930/demos/demo-tf-native-lstm2.12ax.tuned.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/demos/demo-tf-neural-transducer.12ax.config` & `returnn-1.20230703.193930/demos/demo-tf-neural-transducer.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/demos/demo-tf-rec-explicit-lstm.config` & `returnn-1.20230703.193930/demos/demo-tf-rec-explicit-lstm.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/demos/demo-tf-rec-explicit-rnn.config` & `returnn-1.20230703.193930/demos/demo-tf-rec-explicit-rnn.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/demos/demo-tf-rec-self-att.config` & `returnn-1.20230703.193930/demos/demo-tf-rec-self-att.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/demos/demo-tf-search-compiled-graph.py` & `returnn-1.20230703.193930/demos/demo-tf-search-compiled-graph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/demos/demo-tf-vanilla-lstm.12ax.config` & `returnn-1.20230703.193930/demos/demo-tf-vanilla-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/demos/demo-timit-lstm-ctc.config` & `returnn-1.20230703.193930/demos/demo-timit-lstm-ctc.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/demos/demo-torch.config` & `returnn-1.20230703.193930/demos/demo-torch.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/demos/demo-upd-mult-model.lstm.12ax.config` & `returnn-1.20230703.193930/demos/demo-upd-mult-model.lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/demos/demo.sh` & `returnn-1.20230703.193930/demos/demo.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png` & `returnn-1.20230703.193930/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/demos/mdlstm/IAM/IAM_lines/a01-007-04.png` & `returnn-1.20230703.193930/demos/mdlstm/IAM/IAM_lines/a01-007-04.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/demos/mdlstm/IAM/IAM_lines/a01-007-06.png` & `returnn-1.20230703.193930/demos/mdlstm/IAM/IAM_lines/a01-007-06.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/demos/mdlstm/IAM/README.txt` & `returnn-1.20230703.193930/demos/mdlstm/IAM/README.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/demos/mdlstm/IAM/config_demo` & `returnn-1.20230703.193930/demos/mdlstm/IAM/config_demo`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/demos/mdlstm/IAM/config_fwd` & `returnn-1.20230703.193930/demos/mdlstm/IAM/config_fwd`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/demos/mdlstm/IAM/config_real` & `returnn-1.20230703.193930/demos/mdlstm/IAM/config_real`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/demos/mdlstm/IAM/create_IAM_dataset.py` & `returnn-1.20230703.193930/demos/mdlstm/IAM/create_IAM_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/demos/mdlstm/IAM/decode.py` & `returnn-1.20230703.193930/demos/mdlstm/IAM/decode.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/demos/mdlstm/IAM/features/raw/demo.h5` & `returnn-1.20230703.193930/demos/mdlstm/IAM/features/raw/demo.h5`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/demos/mdlstm/IAM/split/eval.txt` & `returnn-1.20230703.193930/demos/mdlstm/IAM/split/eval.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/demos/mdlstm/IAM/split/train.txt` & `returnn-1.20230703.193930/demos/mdlstm/IAM/split/train.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/demos/mdlstm/IAM/split/valid.txt` & `returnn-1.20230703.193930/demos/mdlstm/IAM/split/valid.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/demos/mdlstm/artificial/create_test_h5.py` & `returnn-1.20230703.193930/demos/mdlstm/artificial/create_test_h5.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/demos/mdlstm/artificial/forwardconfig` & `returnn-1.20230703.193930/demos/mdlstm/artificial/forwardconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/demos/mdlstm/artificial/trainconfig` & `returnn-1.20230703.193930/demos/mdlstm/artificial/trainconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/demos/mdlstm/artificial_rgb/create_test_h5.py` & `returnn-1.20230703.193930/demos/mdlstm/artificial_rgb/create_test_h5.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/demos/mdlstm/artificial_rgb/forwardconfig` & `returnn-1.20230703.193930/demos/mdlstm/artificial_rgb/forwardconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/demos/mdlstm/artificial_rgb/trainconfig` & `returnn-1.20230703.193930/demos/mdlstm/artificial_rgb/trainconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/__init__.py` & `returnn-1.20230703.193930/returnn/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/__main__.py` & `returnn-1.20230703.193930/returnn/__main__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/__old_mod_loader__.py` & `returnn-1.20230703.193930/returnn/__old_mod_loader__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/__setup__.py` & `returnn-1.20230703.193930/returnn/__setup__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/config.py` & `returnn-1.20230703.193930/returnn/config.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/datasets/audio.py` & `returnn-1.20230703.193930/returnn/datasets/audio.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/datasets/basic.py` & `returnn-1.20230703.193930/returnn/datasets/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/datasets/bundle_file.py` & `returnn-1.20230703.193930/returnn/datasets/bundle_file.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/datasets/cached.py` & `returnn-1.20230703.193930/returnn/datasets/cached.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/datasets/cached2.py` & `returnn-1.20230703.193930/returnn/datasets/cached2.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/datasets/generating.py` & `returnn-1.20230703.193930/returnn/datasets/generating.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/datasets/hdf.py` & `returnn-1.20230703.193930/returnn/datasets/hdf.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/datasets/lm.py` & `returnn-1.20230703.193930/returnn/datasets/lm.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/datasets/map.py` & `returnn-1.20230703.193930/returnn/datasets/map.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/datasets/meta.py` & `returnn-1.20230703.193930/returnn/datasets/meta.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/datasets/multi_proc.py` & `returnn-1.20230703.193930/returnn/datasets/multi_proc.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/datasets/normalization_data.py` & `returnn-1.20230703.193930/returnn/datasets/normalization_data.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/datasets/numpy_dump.py` & `returnn-1.20230703.193930/returnn/datasets/numpy_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/datasets/raw_wav.py` & `returnn-1.20230703.193930/returnn/datasets/raw_wav.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/datasets/sprint.py` & `returnn-1.20230703.193930/returnn/datasets/sprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/datasets/stereo.py` & `returnn-1.20230703.193930/returnn/datasets/stereo.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/datasets/util/feature_extraction.py` & `returnn-1.20230703.193930/returnn/datasets/util/feature_extraction.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/datasets/util/vocabulary.py` & `returnn-1.20230703.193930/returnn/datasets/util/vocabulary.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/engine/base.py` & `returnn-1.20230703.193930/returnn/engine/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/engine/batch.py` & `returnn-1.20230703.193930/returnn/engine/batch.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/extern/WarpRna/__init__.py` & `returnn-1.20230703.193930/returnn/extern/WarpRna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/extern/WarpRna/__main__.py` & `returnn-1.20230703.193930/returnn/extern/WarpRna/__main__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/extern/WarpRna/warp-rna/LICENSE` & `returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/extern/WarpRna/warp-rna/README.md` & `returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/extern/WarpRna/warp-rna/aligner.gif` & `returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/aligner.gif`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/extern/WarpRna/warp-rna/check.png` & `returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/check.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/extern/WarpRna/warp-rna/core.cu` & `returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/core.cu`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/extern/WarpRna/warp-rna/core.h` & `returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/core.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/extern/WarpRna/warp-rna/core_cpu.cpp` & `returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/core_cpu.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE` & `returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md` & `returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp` & `returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu` & `returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h` & `returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py` & `returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py` & `returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py` & `returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/extern/WarpRna/warp-rna/ref_rna.py` & `returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/ref_rna.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py` & `returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc` & `returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h` & `returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py` & `returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/extern/WarpRna/warp-rna/test.cpp` & `returnn-1.20230703.193930/returnn/extern/WarpRna/warp-rna/test.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/extern/graph_editor/__init__.py` & `returnn-1.20230703.193930/returnn/extern/graph_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/extern/graph_editor/edit.py` & `returnn-1.20230703.193930/returnn/extern/graph_editor/edit.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/extern/graph_editor/reroute.py` & `returnn-1.20230703.193930/returnn/extern/graph_editor/reroute.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/extern/graph_editor/select.py` & `returnn-1.20230703.193930/returnn/extern/graph_editor/select.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/extern/graph_editor/subgraph.py` & `returnn-1.20230703.193930/returnn/extern/graph_editor/subgraph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/extern/graph_editor/transform.py` & `returnn-1.20230703.193930/returnn/extern/graph_editor/transform.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/extern/graph_editor/util.py` & `returnn-1.20230703.193930/returnn/extern/graph_editor/util.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/forward_iface.py` & `returnn-1.20230703.193930/returnn/forward_iface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/frontend/__init__.py` & `returnn-1.20230703.193930/returnn/frontend/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/frontend/_backend.py` & `returnn-1.20230703.193930/returnn/frontend/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/frontend/_numpy_backend.py` & `returnn-1.20230703.193930/returnn/frontend/_numpy_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/frontend/_utils.py` & `returnn-1.20230703.193930/returnn/frontend/_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/frontend/array_.py` & `returnn-1.20230703.193930/returnn/frontend/array_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/frontend/attention.py` & `returnn-1.20230703.193930/returnn/frontend/attention.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/frontend/cond.py` & `returnn-1.20230703.193930/returnn/frontend/cond.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/frontend/const.py` & `returnn-1.20230703.193930/returnn/frontend/const.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/frontend/container.py` & `returnn-1.20230703.193930/returnn/frontend/container.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/frontend/conv.py` & `returnn-1.20230703.193930/returnn/frontend/conv.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/frontend/device.py` & `returnn-1.20230703.193930/returnn/frontend/device.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/frontend/dims.py` & `returnn-1.20230703.193930/returnn/frontend/dims.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/frontend/dropout.py` & `returnn-1.20230703.193930/returnn/frontend/dropout.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/frontend/dtype.py` & `returnn-1.20230703.193930/returnn/frontend/dtype.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/frontend/encoder/base.py` & `returnn-1.20230703.193930/returnn/frontend/encoder/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/frontend/encoder/conformer.py` & `returnn-1.20230703.193930/returnn/frontend/encoder/conformer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/frontend/init.py` & `returnn-1.20230703.193930/returnn/frontend/init.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/frontend/linear.py` & `returnn-1.20230703.193930/returnn/frontend/linear.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/frontend/loop.py` & `returnn-1.20230703.193930/returnn/frontend/loop.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/frontend/loss.py` & `returnn-1.20230703.193930/returnn/frontend/loss.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/frontend/math_.py` & `returnn-1.20230703.193930/returnn/frontend/math_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/frontend/matmul.py` & `returnn-1.20230703.193930/returnn/frontend/matmul.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/frontend/module.py` & `returnn-1.20230703.193930/returnn/frontend/module.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/frontend/normalization.py` & `returnn-1.20230703.193930/returnn/frontend/normalization.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/frontend/parameter.py` & `returnn-1.20230703.193930/returnn/frontend/parameter.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/frontend/rand.py` & `returnn-1.20230703.193930/returnn/frontend/rand.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/frontend/rec.py` & `returnn-1.20230703.193930/returnn/frontend/rec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/frontend/reduce.py` & `returnn-1.20230703.193930/returnn/frontend/reduce.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/frontend/run_ctx.py` & `returnn-1.20230703.193930/returnn/frontend/run_ctx.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/frontend/signal.py` & `returnn-1.20230703.193930/returnn/frontend/signal.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/frontend/state.py` & `returnn-1.20230703.193930/returnn/frontend/state.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/frontend/tensor_array.py` & `returnn-1.20230703.193930/returnn/frontend/tensor_array.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/frontend/types.py` & `returnn-1.20230703.193930/returnn/frontend/types.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/import_/common.py` & `returnn-1.20230703.193930/returnn/import_/common.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/import_/git.py` & `returnn-1.20230703.193930/returnn/import_/git.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/import_/import_.py` & `returnn-1.20230703.193930/returnn/import_/import_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/learning_rate_control.py` & `returnn-1.20230703.193930/returnn/learning_rate_control.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/log.py` & `returnn-1.20230703.193930/returnn/log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/native_op.cpp` & `returnn-1.20230703.193930/returnn/native_op.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/native_op.py` & `returnn-1.20230703.193930/returnn/native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/pretrain.py` & `returnn-1.20230703.193930/returnn/pretrain.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/sprint/cache.py` & `returnn-1.20230703.193930/returnn/sprint/cache.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/sprint/control.py` & `returnn-1.20230703.193930/returnn/sprint/control.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/sprint/error_signals.py` & `returnn-1.20230703.193930/returnn/sprint/error_signals.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/sprint/extern_interface.py` & `returnn-1.20230703.193930/returnn/sprint/extern_interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/sprint/interface.py` & `returnn-1.20230703.193930/returnn/sprint/interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/tensor/_dim_extra.py` & `returnn-1.20230703.193930/returnn/tensor/_dim_extra.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/tensor/_tensor_extra.py` & `returnn-1.20230703.193930/returnn/tensor/_tensor_extra.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/tensor/_tensor_mixin_base.py` & `returnn-1.20230703.193930/returnn/tensor/_tensor_mixin_base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/tensor/_tensor_op_overloads.py` & `returnn-1.20230703.193930/returnn/tensor/_tensor_op_overloads.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/tensor/control_flow_ctx.py` & `returnn-1.20230703.193930/returnn/tensor/control_flow_ctx.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/tensor/dim.py` & `returnn-1.20230703.193930/returnn/tensor/dim.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/tensor/marked_dim.py` & `returnn-1.20230703.193930/returnn/tensor/marked_dim.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/tensor/tensor.py` & `returnn-1.20230703.193930/returnn/tensor/tensor.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/tensor/tensor_dict.py` & `returnn-1.20230703.193930/returnn/tensor/tensor_dict.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/tensor/utils.py` & `returnn-1.20230703.193930/returnn/tensor/utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/tf/compat.py` & `returnn-1.20230703.193930/returnn/tf/compat.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/tf/data_pipeline.py` & `returnn-1.20230703.193930/returnn/tf/data_pipeline.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/tf/distributed.py` & `returnn-1.20230703.193930/returnn/tf/distributed.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/tf/engine.py` & `returnn-1.20230703.193930/returnn/tf/engine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/tf/frontend_layers/_backend.py` & `returnn-1.20230703.193930/returnn/tf/frontend_layers/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/tf/frontend_layers/_utils.py` & `returnn-1.20230703.193930/returnn/tf/frontend_layers/_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/tf/frontend_layers/cond.py` & `returnn-1.20230703.193930/returnn/tf/frontend_layers/cond.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/tf/frontend_layers/config_entry_points.py` & `returnn-1.20230703.193930/returnn/tf/frontend_layers/config_entry_points.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/tf/frontend_layers/debug_eager_mode.py` & `returnn-1.20230703.193930/returnn/tf/frontend_layers/debug_eager_mode.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/tf/frontend_layers/dims.py` & `returnn-1.20230703.193930/returnn/tf/frontend_layers/dims.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/tf/frontend_layers/layer.py` & `returnn-1.20230703.193930/returnn/tf/frontend_layers/layer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/tf/frontend_layers/make_layer.py` & `returnn-1.20230703.193930/returnn/tf/frontend_layers/make_layer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/tf/frontend_layers/parameter_assign.py` & `returnn-1.20230703.193930/returnn/tf/frontend_layers/parameter_assign.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/tf/frontend_layers/prev_tensor_ref.py` & `returnn-1.20230703.193930/returnn/tf/frontend_layers/prev_tensor_ref.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/tf/frontend_low_level/_backend.py` & `returnn-1.20230703.193930/returnn/tf/frontend_low_level/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/tf/horovod.py` & `returnn-1.20230703.193930/returnn/tf/horovod.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/tf/hyper_param_tuning.py` & `returnn-1.20230703.193930/returnn/tf/hyper_param_tuning.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/tf/layers/base.py` & `returnn-1.20230703.193930/returnn/tf/layers/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/tf/layers/basic.py` & `returnn-1.20230703.193930/returnn/tf/layers/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/tf/layers/rec.py` & `returnn-1.20230703.193930/returnn/tf/layers/rec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Defines multiple recurrent layers, most importantly :class:`RecLayer`.
 """
 
 from __future__ import annotations
 
+import contextlib
 import typing
 import tensorflow as tf
 import returnn.tf.compat as tf_compat
 
 try:
     from tensorflow.python.ops.nn import rnn_cell
 except ImportError:
@@ -5446,54 +5447,55 @@
                     rec_layer=rec_layer,
                 )
             else:
                 raise Exception("Did not expect hidden_state_size %r." % dim)
 
     @classmethod
     def get_rec_initial_state_inner(
-        cls, initial_shape, name, state_key="state", key=None, initial_state=None, shape_invariant=None, rec_layer=None
+        cls, initial_shape, name, state_key=None, key=None, initial_state=None, shape_invariant=None, rec_layer=None
     ):
         """
         Generate initial hidden state. Primarily used as a inner function for RnnCellLayer.get_rec_initial_state.
 
         :param tuple initial_shape: shape of the initial state.
         :param str name: layer name.
-        :param str state_key: key to be used to get the state from final_rec_vars.
-        :param str|None key: key/attribute of the state if state is a dictionary/namedtuple
+        :param str|None state_key: key to be used to get the state from final_rec_vars.
+            "state" by default.
+        :param str|int|None key: key/attribute of the state if state is a dictionary/namedtuple
             (like 'c' and 'h' for LSTM states).
         :param LayerBase|str|int|float|None|list|tuple|namedtuple initial_state: see code
         :param tuple shape_invariant: If provided, directly used.
             Otherwise, guessed from initial_shape (see code below).
         :param RecLayer|LayerBase|None rec_layer: For the scope.
         :rtype: tf.Tensor
         """
 
         def _get_last_state() -> tf.Tensor:
             # Note: The rec_layer is always the outer rec layer.
             # `name` refers to the inner rec layer.
             # https://github.com/rwth-i6/returnn/pull/1248#issuecomment-1618125397
             if isinstance(rec_layer, RecLayer) and isinstance(rec_layer.cell, _SubnetworkRecCell):
                 final_rec_vars = rec_layer.cell.get_final_rec_vars(name)
-                last_state = cls.get_state_by_key(final_rec_vars[state_key], key=key, shape=initial_shape)
+                last_state = cls.get_state_by_key(final_rec_vars[state_key or "state"], key=key, shape=initial_shape)
             else:
-                last_state = rec_layer.get_last_hidden_state(key=key)
+                assert key is None or not state_key
+                last_state = rec_layer.get_last_hidden_state(key=key if key is not None else state_key)
             last_state.set_shape(shape_invariant)
             return last_state
 
-        if state_key == "state":
+        if not state_key:
             if key is None:
                 key_name = "var"
             else:
                 key_name = str(key)
         else:
             if key is None:
                 key_name = state_key
             else:
                 key_name = f"{state_key}_{key}"
-        from returnn.util.basic import dummy_noop_ctx
 
         if shape_invariant is None:
             shape_invariant = tuple([d if isinstance(d, int) and d != 0 else None for d in initial_shape])
         if isinstance(initial_state, LayerBase):
             h = initial_state.get_last_hidden_state(key="*")
             if h is not None:
                 h.set_shape(shape_invariant)
@@ -5506,15 +5508,15 @@
         elif initial_state == "zeros" or not initial_state:
             return tf.zeros(initial_shape)
         elif initial_state == "ones" or initial_state == 1:
             return tf.ones(initial_shape)
         elif initial_state == "var":  # Initial state is a trainable variable.
             # Assume the first dimension to be batch_dim.
             assert shape_invariant[0] is None and all([d is not None for d in shape_invariant[1:]])
-            with rec_layer.var_creation_scope() if rec_layer else dummy_noop_ctx():
+            with rec_layer.var_creation_scope() if rec_layer else contextlib.nullcontext():
                 var = tf_compat.v1.get_variable(
                     "initial_%s" % key_name, shape=initial_shape[1:], initializer=tf.zeros_initializer()
                 )
             from returnn.tf.util.basic import expand_dims_unbroadcast
 
             var = expand_dims_unbroadcast(var, axis=0, dim=initial_shape[0])  # (batch,dim)
             return var
```

### Comparing `returnn-1.20230703.180607/returnn/tf/layers/segmental_model.py` & `returnn-1.20230703.193930/returnn/tf/layers/segmental_model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/tf/layers/signal_processing.py` & `returnn-1.20230703.193930/returnn/tf/layers/signal_processing.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/tf/layers/variable.py` & `returnn-1.20230703.193930/returnn/tf/layers/variable.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/tf/native_op.py` & `returnn-1.20230703.193930/returnn/tf/native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/tf/network.py` & `returnn-1.20230703.193930/returnn/tf/network.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/tf/sprint.py` & `returnn-1.20230703.193930/returnn/tf/sprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/tf/updater.py` & `returnn-1.20230703.193930/returnn/tf/updater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/tf/util/basic.py` & `returnn-1.20230703.193930/returnn/tf/util/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/tf/util/data.py` & `returnn-1.20230703.193930/returnn/tf/util/data.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/tf/util/gradient_checkpoint.py` & `returnn-1.20230703.193930/returnn/tf/util/gradient_checkpoint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/tf/util/ken_lm.py` & `returnn-1.20230703.193930/returnn/tf/util/ken_lm.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/tf/util/open_fst.py` & `returnn-1.20230703.193930/returnn/tf/util/open_fst.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/torch/data/pipeline.py` & `returnn-1.20230703.193930/returnn/torch/data/pipeline.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/torch/data/returnn_dataset_wrapper.py` & `returnn-1.20230703.193930/returnn/torch/data/returnn_dataset_wrapper.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/torch/data/tensor_utils.py` & `returnn-1.20230703.193930/returnn/torch/data/tensor_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/torch/distributed.py` & `returnn-1.20230703.193930/returnn/torch/distributed.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/torch/engine.py` & `returnn-1.20230703.193930/returnn/torch/engine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/torch/frontend/_backend.py` & `returnn-1.20230703.193930/returnn/torch/frontend/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/torch/frontend/_rand.py` & `returnn-1.20230703.193930/returnn/torch/frontend/_rand.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/torch/frontend/bridge.py` & `returnn-1.20230703.193930/returnn/torch/frontend/bridge.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/torch/updater.py` & `returnn-1.20230703.193930/returnn/torch/updater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/util/basic.py` & `returnn-1.20230703.193930/returnn/util/basic.py`

 * *Files 0% similar despite different names*

```diff
@@ -8277,788 +8277,781 @@
 00020540: 6973 7375 652f 5059 2d35 3038 3238 292e  issue/PY-50828).
 00020550: 0a20 2020 203a 7274 7970 653a 206c 6973  .    :rtype: lis
 00020560: 745b 545d 0a20 2020 2022 2222 0a20 2020  t[T].    """.   
 00020570: 2061 7373 6572 7420 616c 6c28 6973 696e   assert all(isin
 00020580: 7374 616e 6365 2865 6c65 6d2c 2074 7970  stance(elem, typ
 00020590: 655f 2920 666f 7220 656c 656d 2069 6e20  e_) for elem in 
 000205a0: 6c73 290a 2020 2020 7265 7475 726e 206c  ls).    return l
-000205b0: 730a 0a0a 4063 6f6e 7465 7874 6c69 622e  s...@contextlib.
-000205c0: 636f 6e74 6578 746d 616e 6167 6572 0a64  contextmanager.d
-000205d0: 6566 2064 756d 6d79 5f6e 6f6f 705f 6374  ef dummy_noop_ct
-000205e0: 7828 293a 0a20 2020 2022 2222 0a20 2020  x():.    """.   
-000205f0: 2050 726f 7669 6465 7320 6120 6e6f 2d6f   Provides a no-o
-00020600: 7020 636f 6e74 6578 7420 6d61 6e61 6765  p context manage
-00020610: 722e 0a20 2020 2022 2222 0a20 2020 2079  r..    """.    y
-00020620: 6965 6c64 204e 6f6e 650a 0a0a 6465 6620  ield None...def 
-00020630: 5f67 6574 5f6e 6772 616d 7328 7365 676d  _get_ngrams(segm
-00020640: 656e 742c 206d 6178 5f6f 7264 6572 293a  ent, max_order):
-00020650: 0a20 2020 2022 2222 4578 7472 6163 7473  .    """Extracts
-00020660: 2061 6c6c 206e 2d67 7261 6d73 2075 7074   all n-grams upt
-00020670: 6f20 6120 6769 7665 6e20 6d61 7869 6d75  o a given maximu
-00020680: 6d20 6f72 6465 7220 6672 6f6d 2061 6e20  m order from an 
-00020690: 696e 7075 7420 7365 676d 656e 742e 0a20  input segment.. 
-000206a0: 2020 2043 6f64 6520 6164 6170 7465 6420     Code adapted 
-000206b0: 6672 6f6d 2047 6f6f 676c 6520 5465 6e73  from Google Tens
-000206c0: 6f72 3254 656e 736f 722e 0a0a 2020 2020  or2Tensor...    
-000206d0: 4172 6773 3a0a 2020 2020 2020 7365 676d  Args:.      segm
-000206e0: 656e 7420 286c 6973 745b 696e 745d 7c6c  ent (list[int]|l
-000206f0: 6973 745b 7374 725d 293a 2074 6578 7420  ist[str]): text 
-00020700: 7365 676d 656e 7420 6672 6f6d 2077 6869  segment from whi
-00020710: 6368 206e 2d67 7261 6d73 2077 696c 6c20  ch n-grams will 
-00020720: 6265 2065 7874 7261 6374 6564 2e0a 2020  be extracted..  
-00020730: 2020 2020 6d61 785f 6f72 6465 7220 2869      max_order (i
-00020740: 6e74 293a 206d 6178 696d 756d 206c 656e  nt): maximum len
-00020750: 6774 6820 696e 2074 6f6b 656e 7320 6f66  gth in tokens of
-00020760: 2074 6865 206e 2d67 7261 6d73 2072 6574   the n-grams ret
-00020770: 7572 6e65 6420 6279 2074 6869 730a 2020  urned by this.  
-00020780: 2020 2020 2020 2020 6d65 7468 6f64 732e          methods.
-00020790: 0a0a 2020 2020 5265 7475 726e 733a 0a20  ..    Returns:. 
-000207a0: 2020 2020 2054 6865 2043 6f75 6e74 6572       The Counter
-000207b0: 2063 6f6e 7461 696e 696e 6720 616c 6c20   containing all 
-000207c0: 6e2d 6772 616d 7320 7570 746f 206d 6178  n-grams upto max
-000207d0: 5f6f 7264 6572 2069 6e20 7365 676d 656e  _order in segmen
-000207e0: 740a 2020 2020 2020 7769 7468 2061 2063  t.      with a c
-000207f0: 6f75 6e74 206f 6620 686f 7720 6d61 6e79  ount of how many
-00020800: 2074 696d 6573 2065 6163 6820 6e2d 6772   times each n-gr
-00020810: 616d 206f 6363 7572 7265 642e 0a20 2020  am occurred..   
-00020820: 2022 2222 0a20 2020 2069 6d70 6f72 7420   """.    import 
-00020830: 636f 6c6c 6563 7469 6f6e 730a 0a20 2020  collections..   
-00020840: 206e 6772 616d 5f63 6f75 6e74 7320 3d20   ngram_counts = 
-00020850: 636f 6c6c 6563 7469 6f6e 732e 436f 756e  collections.Coun
-00020860: 7465 7228 290a 2020 2020 666f 7220 6f72  ter().    for or
-00020870: 6465 7220 696e 2072 616e 6765 2831 2c20  der in range(1, 
-00020880: 6d61 785f 6f72 6465 7220 2b20 3129 3a0a  max_order + 1):.
-00020890: 2020 2020 2020 2020 666f 7220 6920 696e          for i in
-000208a0: 2072 616e 6765 2830 2c20 6c65 6e28 7365   range(0, len(se
-000208b0: 676d 656e 7429 202d 206f 7264 6572 202b  gment) - order +
-000208c0: 2031 293a 0a20 2020 2020 2020 2020 2020   1):.           
-000208d0: 206e 6772 616d 203d 2074 7570 6c65 2873   ngram = tuple(s
-000208e0: 6567 6d65 6e74 5b69 203a 2069 202b 206f  egment[i : i + o
-000208f0: 7264 6572 5d29 0a20 2020 2020 2020 2020  rder]).         
-00020900: 2020 206e 6772 616d 5f63 6f75 6e74 735b     ngram_counts[
-00020910: 6e67 7261 6d5d 202b 3d20 310a 2020 2020  ngram] += 1.    
-00020920: 7265 7475 726e 206e 6772 616d 5f63 6f75  return ngram_cou
-00020930: 6e74 730a 0a0a 6465 6620 636f 6d70 7574  nts...def comput
-00020940: 655f 626c 6575 2872 6566 6572 656e 6365  e_bleu(reference
-00020950: 5f63 6f72 7075 732c 2074 7261 6e73 6c61  _corpus, transla
-00020960: 7469 6f6e 5f63 6f72 7075 732c 206d 6178  tion_corpus, max
-00020970: 5f6f 7264 6572 3d34 2c20 7573 655f 6270  _order=4, use_bp
-00020980: 3d54 7275 6529 3a0a 2020 2020 2222 2243  =True):.    """C
-00020990: 6f6d 7075 7465 7320 424c 4555 2073 636f  omputes BLEU sco
-000209a0: 7265 206f 6620 7472 616e 736c 6174 6564  re of translated
-000209b0: 2073 6567 6d65 6e74 7320 6167 6169 6e73   segments agains
-000209c0: 7420 6f6e 6520 6f72 206d 6f72 6520 7265  t one or more re
-000209d0: 6665 7265 6e63 6573 2e0a 2020 2020 436f  ferences..    Co
-000209e0: 6465 2061 6461 7074 6564 2066 726f 6d20  de adapted from 
-000209f0: 476f 6f67 6c65 2054 656e 736f 7232 5465  Google Tensor2Te
-00020a00: 6e73 6f72 2e0a 0a20 2020 2041 7267 733a  nsor...    Args:
-00020a10: 0a20 2020 2020 2072 6566 6572 656e 6365  .      reference
-00020a20: 5f63 6f72 7075 7320 286c 6973 745b 6c69  _corpus (list[li
-00020a30: 7374 5b69 6e74 5d7c 6c69 7374 5b73 7472  st[int]|list[str
-00020a40: 5d5d 293a 206c 6973 7420 6f66 2072 6566  ]]): list of ref
-00020a50: 6572 656e 6365 7320 666f 7220 6561 6368  erences for each
-00020a60: 2074 7261 6e73 6c61 7469 6f6e 2e20 4561   translation. Ea
-00020a70: 6368 0a20 2020 2020 2020 2020 2072 6566  ch.          ref
-00020a80: 6572 656e 6365 2073 686f 756c 6420 6265  erence should be
-00020a90: 2074 6f6b 656e 697a 6564 2069 6e74 6f20   tokenized into 
-00020aa0: 6120 6c69 7374 206f 6620 746f 6b65 6e73  a list of tokens
-00020ab0: 2e0a 2020 2020 2020 7472 616e 736c 6174  ..      translat
-00020ac0: 696f 6e5f 636f 7270 7573 2028 6c69 7374  ion_corpus (list
-00020ad0: 5b6c 6973 745b 696e 745d 7c6c 6973 745b  [list[int]|list[
-00020ae0: 7374 725d 5d29 3a20 6c69 7374 206f 6620  str]]): list of 
-00020af0: 7472 616e 736c 6174 696f 6e73 2074 6f20  translations to 
-00020b00: 7363 6f72 652e 2045 6163 6820 7472 616e  score. Each tran
-00020b10: 736c 6174 696f 6e0a 2020 2020 2020 2020  slation.        
-00020b20: 2020 7368 6f75 6c64 2062 6520 746f 6b65    should be toke
-00020b30: 6e69 7a65 6420 696e 746f 2061 206c 6973  nized into a lis
-00020b40: 7420 6f66 2074 6f6b 656e 732e 0a20 2020  t of tokens..   
-00020b50: 2020 206d 6178 5f6f 7264 6572 2028 696e     max_order (in
-00020b60: 7429 3a20 4d61 7869 6d75 6d20 6e2d 6772  t): Maximum n-gr
-00020b70: 616d 206f 7264 6572 2074 6f20 7573 6520  am order to use 
-00020b80: 7768 656e 2063 6f6d 7075 7469 6e67 2042  when computing B
-00020b90: 4c45 5520 7363 6f72 652e 0a20 2020 2020  LEU score..     
-00020ba0: 2075 7365 5f62 7020 2862 6f6f 6c29 3a20   use_bp (bool): 
-00020bb0: 626f 6f6c 6561 6e2c 2077 6865 7468 6572  boolean, whether
-00020bc0: 2074 6f20 6170 706c 7920 6272 6576 6974   to apply brevit
-00020bd0: 7920 7065 6e61 6c74 792e 0a0a 2020 2020  y penalty...    
-00020be0: 5265 7475 726e 733a 0a20 2020 2020 2042  Returns:.      B
-00020bf0: 4c45 5520 7363 6f72 652e 0a20 2020 2022  LEU score..    "
-00020c00: 2222 0a20 2020 2069 6d70 6f72 7420 6d61  "".    import ma
-00020c10: 7468 0a0a 2020 2020 7265 6665 7265 6e63  th..    referenc
-00020c20: 655f 6c65 6e67 7468 203d 2030 0a20 2020  e_length = 0.   
-00020c30: 2074 7261 6e73 6c61 7469 6f6e 5f6c 656e   translation_len
-00020c40: 6774 6820 3d20 300a 2020 2020 6270 203d  gth = 0.    bp =
-00020c50: 2031 2e30 0a20 2020 2067 656f 5f6d 6561   1.0.    geo_mea
-00020c60: 6e20 3d20 300a 0a20 2020 206d 6174 6368  n = 0..    match
-00020c70: 6573 5f62 795f 6f72 6465 7220 3d20 5b30  es_by_order = [0
-00020c80: 5d20 2a20 6d61 785f 6f72 6465 720a 2020  ] * max_order.  
-00020c90: 2020 706f 7373 6962 6c65 5f6d 6174 6368    possible_match
-00020ca0: 6573 5f62 795f 6f72 6465 7220 3d20 5b30  es_by_order = [0
-00020cb0: 5d20 2a20 6d61 785f 6f72 6465 720a 0a20  ] * max_order.. 
-00020cc0: 2020 2066 6f72 2028 7265 6665 7265 6e63     for (referenc
-00020cd0: 6573 2c20 7472 616e 736c 6174 696f 6e73  es, translations
-00020ce0: 2920 696e 207a 6970 2872 6566 6572 656e  ) in zip(referen
-00020cf0: 6365 5f63 6f72 7075 732c 2074 7261 6e73  ce_corpus, trans
-00020d00: 6c61 7469 6f6e 5f63 6f72 7075 7329 3a0a  lation_corpus):.
-00020d10: 2020 2020 2020 2020 7265 6665 7265 6e63          referenc
-00020d20: 655f 6c65 6e67 7468 202b 3d20 6c65 6e28  e_length += len(
-00020d30: 7265 6665 7265 6e63 6573 290a 2020 2020  references).    
-00020d40: 2020 2020 7472 616e 736c 6174 696f 6e5f      translation_
-00020d50: 6c65 6e67 7468 202b 3d20 6c65 6e28 7472  length += len(tr
-00020d60: 616e 736c 6174 696f 6e73 290a 2020 2020  anslations).    
-00020d70: 2020 2020 7265 665f 6e67 7261 6d5f 636f      ref_ngram_co
-00020d80: 756e 7473 203d 205f 6765 745f 6e67 7261  unts = _get_ngra
-00020d90: 6d73 2872 6566 6572 656e 6365 732c 206d  ms(references, m
-00020da0: 6178 5f6f 7264 6572 290a 2020 2020 2020  ax_order).      
-00020db0: 2020 7472 616e 736c 6174 696f 6e5f 6e67    translation_ng
-00020dc0: 7261 6d5f 636f 756e 7473 203d 205f 6765  ram_counts = _ge
-00020dd0: 745f 6e67 7261 6d73 2874 7261 6e73 6c61  t_ngrams(transla
-00020de0: 7469 6f6e 732c 206d 6178 5f6f 7264 6572  tions, max_order
-00020df0: 290a 0a20 2020 2020 2020 206f 7665 726c  )..        overl
-00020e00: 6170 203d 207b 6e67 7261 6d3a 206d 696e  ap = {ngram: min
-00020e10: 2863 6f75 6e74 2c20 7472 616e 736c 6174  (count, translat
-00020e20: 696f 6e5f 6e67 7261 6d5f 636f 756e 7473  ion_ngram_counts
-00020e30: 5b6e 6772 616d 5d29 2066 6f72 206e 6772  [ngram]) for ngr
-00020e40: 616d 2c20 636f 756e 7420 696e 2072 6566  am, count in ref
-00020e50: 5f6e 6772 616d 5f63 6f75 6e74 732e 6974  _ngram_counts.it
-00020e60: 656d 7328 297d 0a0a 2020 2020 2020 2020  ems()}..        
-00020e70: 666f 7220 6e67 7261 6d20 696e 206f 7665  for ngram in ove
-00020e80: 726c 6170 3a0a 2020 2020 2020 2020 2020  rlap:.          
-00020e90: 2020 6d61 7463 6865 735f 6279 5f6f 7264    matches_by_ord
-00020ea0: 6572 5b6c 656e 286e 6772 616d 2920 2d20  er[len(ngram) - 
-00020eb0: 315d 202b 3d20 6f76 6572 6c61 705b 6e67  1] += overlap[ng
-00020ec0: 7261 6d5d 0a20 2020 2020 2020 2066 6f72  ram].        for
-00020ed0: 206e 6772 616d 2069 6e20 7472 616e 736c   ngram in transl
-00020ee0: 6174 696f 6e5f 6e67 7261 6d5f 636f 756e  ation_ngram_coun
-00020ef0: 7473 3a0a 2020 2020 2020 2020 2020 2020  ts:.            
-00020f00: 706f 7373 6962 6c65 5f6d 6174 6368 6573  possible_matches
-00020f10: 5f62 795f 6f72 6465 725b 6c65 6e28 6e67  _by_order[len(ng
-00020f20: 7261 6d29 202d 2031 5d20 2b3d 2074 7261  ram) - 1] += tra
-00020f30: 6e73 6c61 7469 6f6e 5f6e 6772 616d 5f63  nslation_ngram_c
-00020f40: 6f75 6e74 735b 6e67 7261 6d5d 0a0a 2020  ounts[ngram]..  
-00020f50: 2020 7072 6563 6973 696f 6e73 203d 205b    precisions = [
-00020f60: 302e 305d 202a 206d 6178 5f6f 7264 6572  0.0] * max_order
-00020f70: 0a20 2020 2073 6d6f 6f74 6820 3d20 312e  .    smooth = 1.
-00020f80: 300a 2020 2020 666f 7220 6920 696e 2072  0.    for i in r
-00020f90: 616e 6765 2830 2c20 6d61 785f 6f72 6465  ange(0, max_orde
-00020fa0: 7229 3a0a 2020 2020 2020 2020 6966 2070  r):.        if p
-00020fb0: 6f73 7369 626c 655f 6d61 7463 6865 735f  ossible_matches_
-00020fc0: 6279 5f6f 7264 6572 5b69 5d20 3e20 303a  by_order[i] > 0:
-00020fd0: 0a20 2020 2020 2020 2020 2020 2070 7265  .            pre
-00020fe0: 6369 7369 6f6e 735b 695d 203d 206d 6174  cisions[i] = mat
-00020ff0: 6368 6573 5f62 795f 6f72 6465 725b 695d  ches_by_order[i]
-00021000: 202f 2070 6f73 7369 626c 655f 6d61 7463   / possible_matc
-00021010: 6865 735f 6279 5f6f 7264 6572 5b69 5d0a  hes_by_order[i].
-00021020: 2020 2020 2020 2020 2020 2020 6966 206d              if m
-00021030: 6174 6368 6573 5f62 795f 6f72 6465 725b  atches_by_order[
-00021040: 695d 203e 2030 3a0a 2020 2020 2020 2020  i] > 0:.        
-00021050: 2020 2020 2020 2020 7072 6563 6973 696f          precisio
-00021060: 6e73 5b69 5d20 3d20 6d61 7463 6865 735f  ns[i] = matches_
-00021070: 6279 5f6f 7264 6572 5b69 5d20 2f20 706f  by_order[i] / po
-00021080: 7373 6962 6c65 5f6d 6174 6368 6573 5f62  ssible_matches_b
-00021090: 795f 6f72 6465 725b 695d 0a20 2020 2020  y_order[i].     
+000205b0: 730a 0a0a 6465 6620 5f67 6574 5f6e 6772  s...def _get_ngr
+000205c0: 616d 7328 7365 676d 656e 742c 206d 6178  ams(segment, max
+000205d0: 5f6f 7264 6572 293a 0a20 2020 2022 2222  _order):.    """
+000205e0: 4578 7472 6163 7473 2061 6c6c 206e 2d67  Extracts all n-g
+000205f0: 7261 6d73 2075 7074 6f20 6120 6769 7665  rams upto a give
+00020600: 6e20 6d61 7869 6d75 6d20 6f72 6465 7220  n maximum order 
+00020610: 6672 6f6d 2061 6e20 696e 7075 7420 7365  from an input se
+00020620: 676d 656e 742e 0a20 2020 2043 6f64 6520  gment..    Code 
+00020630: 6164 6170 7465 6420 6672 6f6d 2047 6f6f  adapted from Goo
+00020640: 676c 6520 5465 6e73 6f72 3254 656e 736f  gle Tensor2Tenso
+00020650: 722e 0a0a 2020 2020 4172 6773 3a0a 2020  r...    Args:.  
+00020660: 2020 2020 7365 676d 656e 7420 286c 6973      segment (lis
+00020670: 745b 696e 745d 7c6c 6973 745b 7374 725d  t[int]|list[str]
+00020680: 293a 2074 6578 7420 7365 676d 656e 7420  ): text segment 
+00020690: 6672 6f6d 2077 6869 6368 206e 2d67 7261  from which n-gra
+000206a0: 6d73 2077 696c 6c20 6265 2065 7874 7261  ms will be extra
+000206b0: 6374 6564 2e0a 2020 2020 2020 6d61 785f  cted..      max_
+000206c0: 6f72 6465 7220 2869 6e74 293a 206d 6178  order (int): max
+000206d0: 696d 756d 206c 656e 6774 6820 696e 2074  imum length in t
+000206e0: 6f6b 656e 7320 6f66 2074 6865 206e 2d67  okens of the n-g
+000206f0: 7261 6d73 2072 6574 7572 6e65 6420 6279  rams returned by
+00020700: 2074 6869 730a 2020 2020 2020 2020 2020   this.          
+00020710: 6d65 7468 6f64 732e 0a0a 2020 2020 5265  methods...    Re
+00020720: 7475 726e 733a 0a20 2020 2020 2054 6865  turns:.      The
+00020730: 2043 6f75 6e74 6572 2063 6f6e 7461 696e   Counter contain
+00020740: 696e 6720 616c 6c20 6e2d 6772 616d 7320  ing all n-grams 
+00020750: 7570 746f 206d 6178 5f6f 7264 6572 2069  upto max_order i
+00020760: 6e20 7365 676d 656e 740a 2020 2020 2020  n segment.      
+00020770: 7769 7468 2061 2063 6f75 6e74 206f 6620  with a count of 
+00020780: 686f 7720 6d61 6e79 2074 696d 6573 2065  how many times e
+00020790: 6163 6820 6e2d 6772 616d 206f 6363 7572  ach n-gram occur
+000207a0: 7265 642e 0a20 2020 2022 2222 0a20 2020  red..    """.   
+000207b0: 2069 6d70 6f72 7420 636f 6c6c 6563 7469   import collecti
+000207c0: 6f6e 730a 0a20 2020 206e 6772 616d 5f63  ons..    ngram_c
+000207d0: 6f75 6e74 7320 3d20 636f 6c6c 6563 7469  ounts = collecti
+000207e0: 6f6e 732e 436f 756e 7465 7228 290a 2020  ons.Counter().  
+000207f0: 2020 666f 7220 6f72 6465 7220 696e 2072    for order in r
+00020800: 616e 6765 2831 2c20 6d61 785f 6f72 6465  ange(1, max_orde
+00020810: 7220 2b20 3129 3a0a 2020 2020 2020 2020  r + 1):.        
+00020820: 666f 7220 6920 696e 2072 616e 6765 2830  for i in range(0
+00020830: 2c20 6c65 6e28 7365 676d 656e 7429 202d  , len(segment) -
+00020840: 206f 7264 6572 202b 2031 293a 0a20 2020   order + 1):.   
+00020850: 2020 2020 2020 2020 206e 6772 616d 203d           ngram =
+00020860: 2074 7570 6c65 2873 6567 6d65 6e74 5b69   tuple(segment[i
+00020870: 203a 2069 202b 206f 7264 6572 5d29 0a20   : i + order]). 
+00020880: 2020 2020 2020 2020 2020 206e 6772 616d             ngram
+00020890: 5f63 6f75 6e74 735b 6e67 7261 6d5d 202b  _counts[ngram] +
+000208a0: 3d20 310a 2020 2020 7265 7475 726e 206e  = 1.    return n
+000208b0: 6772 616d 5f63 6f75 6e74 730a 0a0a 6465  gram_counts...de
+000208c0: 6620 636f 6d70 7574 655f 626c 6575 2872  f compute_bleu(r
+000208d0: 6566 6572 656e 6365 5f63 6f72 7075 732c  eference_corpus,
+000208e0: 2074 7261 6e73 6c61 7469 6f6e 5f63 6f72   translation_cor
+000208f0: 7075 732c 206d 6178 5f6f 7264 6572 3d34  pus, max_order=4
+00020900: 2c20 7573 655f 6270 3d54 7275 6529 3a0a  , use_bp=True):.
+00020910: 2020 2020 2222 2243 6f6d 7075 7465 7320      """Computes 
+00020920: 424c 4555 2073 636f 7265 206f 6620 7472  BLEU score of tr
+00020930: 616e 736c 6174 6564 2073 6567 6d65 6e74  anslated segment
+00020940: 7320 6167 6169 6e73 7420 6f6e 6520 6f72  s against one or
+00020950: 206d 6f72 6520 7265 6665 7265 6e63 6573   more references
+00020960: 2e0a 2020 2020 436f 6465 2061 6461 7074  ..    Code adapt
+00020970: 6564 2066 726f 6d20 476f 6f67 6c65 2054  ed from Google T
+00020980: 656e 736f 7232 5465 6e73 6f72 2e0a 0a20  ensor2Tensor... 
+00020990: 2020 2041 7267 733a 0a20 2020 2020 2072     Args:.      r
+000209a0: 6566 6572 656e 6365 5f63 6f72 7075 7320  eference_corpus 
+000209b0: 286c 6973 745b 6c69 7374 5b69 6e74 5d7c  (list[list[int]|
+000209c0: 6c69 7374 5b73 7472 5d5d 293a 206c 6973  list[str]]): lis
+000209d0: 7420 6f66 2072 6566 6572 656e 6365 7320  t of references 
+000209e0: 666f 7220 6561 6368 2074 7261 6e73 6c61  for each transla
+000209f0: 7469 6f6e 2e20 4561 6368 0a20 2020 2020  tion. Each.     
+00020a00: 2020 2020 2072 6566 6572 656e 6365 2073       reference s
+00020a10: 686f 756c 6420 6265 2074 6f6b 656e 697a  hould be tokeniz
+00020a20: 6564 2069 6e74 6f20 6120 6c69 7374 206f  ed into a list o
+00020a30: 6620 746f 6b65 6e73 2e0a 2020 2020 2020  f tokens..      
+00020a40: 7472 616e 736c 6174 696f 6e5f 636f 7270  translation_corp
+00020a50: 7573 2028 6c69 7374 5b6c 6973 745b 696e  us (list[list[in
+00020a60: 745d 7c6c 6973 745b 7374 725d 5d29 3a20  t]|list[str]]): 
+00020a70: 6c69 7374 206f 6620 7472 616e 736c 6174  list of translat
+00020a80: 696f 6e73 2074 6f20 7363 6f72 652e 2045  ions to score. E
+00020a90: 6163 6820 7472 616e 736c 6174 696f 6e0a  ach translation.
+00020aa0: 2020 2020 2020 2020 2020 7368 6f75 6c64            should
+00020ab0: 2062 6520 746f 6b65 6e69 7a65 6420 696e   be tokenized in
+00020ac0: 746f 2061 206c 6973 7420 6f66 2074 6f6b  to a list of tok
+00020ad0: 656e 732e 0a20 2020 2020 206d 6178 5f6f  ens..      max_o
+00020ae0: 7264 6572 2028 696e 7429 3a20 4d61 7869  rder (int): Maxi
+00020af0: 6d75 6d20 6e2d 6772 616d 206f 7264 6572  mum n-gram order
+00020b00: 2074 6f20 7573 6520 7768 656e 2063 6f6d   to use when com
+00020b10: 7075 7469 6e67 2042 4c45 5520 7363 6f72  puting BLEU scor
+00020b20: 652e 0a20 2020 2020 2075 7365 5f62 7020  e..      use_bp 
+00020b30: 2862 6f6f 6c29 3a20 626f 6f6c 6561 6e2c  (bool): boolean,
+00020b40: 2077 6865 7468 6572 2074 6f20 6170 706c   whether to appl
+00020b50: 7920 6272 6576 6974 7920 7065 6e61 6c74  y brevity penalt
+00020b60: 792e 0a0a 2020 2020 5265 7475 726e 733a  y...    Returns:
+00020b70: 0a20 2020 2020 2042 4c45 5520 7363 6f72  .      BLEU scor
+00020b80: 652e 0a20 2020 2022 2222 0a20 2020 2069  e..    """.    i
+00020b90: 6d70 6f72 7420 6d61 7468 0a0a 2020 2020  mport math..    
+00020ba0: 7265 6665 7265 6e63 655f 6c65 6e67 7468  reference_length
+00020bb0: 203d 2030 0a20 2020 2074 7261 6e73 6c61   = 0.    transla
+00020bc0: 7469 6f6e 5f6c 656e 6774 6820 3d20 300a  tion_length = 0.
+00020bd0: 2020 2020 6270 203d 2031 2e30 0a20 2020      bp = 1.0.   
+00020be0: 2067 656f 5f6d 6561 6e20 3d20 300a 0a20   geo_mean = 0.. 
+00020bf0: 2020 206d 6174 6368 6573 5f62 795f 6f72     matches_by_or
+00020c00: 6465 7220 3d20 5b30 5d20 2a20 6d61 785f  der = [0] * max_
+00020c10: 6f72 6465 720a 2020 2020 706f 7373 6962  order.    possib
+00020c20: 6c65 5f6d 6174 6368 6573 5f62 795f 6f72  le_matches_by_or
+00020c30: 6465 7220 3d20 5b30 5d20 2a20 6d61 785f  der = [0] * max_
+00020c40: 6f72 6465 720a 0a20 2020 2066 6f72 2028  order..    for (
+00020c50: 7265 6665 7265 6e63 6573 2c20 7472 616e  references, tran
+00020c60: 736c 6174 696f 6e73 2920 696e 207a 6970  slations) in zip
+00020c70: 2872 6566 6572 656e 6365 5f63 6f72 7075  (reference_corpu
+00020c80: 732c 2074 7261 6e73 6c61 7469 6f6e 5f63  s, translation_c
+00020c90: 6f72 7075 7329 3a0a 2020 2020 2020 2020  orpus):.        
+00020ca0: 7265 6665 7265 6e63 655f 6c65 6e67 7468  reference_length
+00020cb0: 202b 3d20 6c65 6e28 7265 6665 7265 6e63   += len(referenc
+00020cc0: 6573 290a 2020 2020 2020 2020 7472 616e  es).        tran
+00020cd0: 736c 6174 696f 6e5f 6c65 6e67 7468 202b  slation_length +
+00020ce0: 3d20 6c65 6e28 7472 616e 736c 6174 696f  = len(translatio
+00020cf0: 6e73 290a 2020 2020 2020 2020 7265 665f  ns).        ref_
+00020d00: 6e67 7261 6d5f 636f 756e 7473 203d 205f  ngram_counts = _
+00020d10: 6765 745f 6e67 7261 6d73 2872 6566 6572  get_ngrams(refer
+00020d20: 656e 6365 732c 206d 6178 5f6f 7264 6572  ences, max_order
+00020d30: 290a 2020 2020 2020 2020 7472 616e 736c  ).        transl
+00020d40: 6174 696f 6e5f 6e67 7261 6d5f 636f 756e  ation_ngram_coun
+00020d50: 7473 203d 205f 6765 745f 6e67 7261 6d73  ts = _get_ngrams
+00020d60: 2874 7261 6e73 6c61 7469 6f6e 732c 206d  (translations, m
+00020d70: 6178 5f6f 7264 6572 290a 0a20 2020 2020  ax_order)..     
+00020d80: 2020 206f 7665 726c 6170 203d 207b 6e67     overlap = {ng
+00020d90: 7261 6d3a 206d 696e 2863 6f75 6e74 2c20  ram: min(count, 
+00020da0: 7472 616e 736c 6174 696f 6e5f 6e67 7261  translation_ngra
+00020db0: 6d5f 636f 756e 7473 5b6e 6772 616d 5d29  m_counts[ngram])
+00020dc0: 2066 6f72 206e 6772 616d 2c20 636f 756e   for ngram, coun
+00020dd0: 7420 696e 2072 6566 5f6e 6772 616d 5f63  t in ref_ngram_c
+00020de0: 6f75 6e74 732e 6974 656d 7328 297d 0a0a  ounts.items()}..
+00020df0: 2020 2020 2020 2020 666f 7220 6e67 7261          for ngra
+00020e00: 6d20 696e 206f 7665 726c 6170 3a0a 2020  m in overlap:.  
+00020e10: 2020 2020 2020 2020 2020 6d61 7463 6865            matche
+00020e20: 735f 6279 5f6f 7264 6572 5b6c 656e 286e  s_by_order[len(n
+00020e30: 6772 616d 2920 2d20 315d 202b 3d20 6f76  gram) - 1] += ov
+00020e40: 6572 6c61 705b 6e67 7261 6d5d 0a20 2020  erlap[ngram].   
+00020e50: 2020 2020 2066 6f72 206e 6772 616d 2069       for ngram i
+00020e60: 6e20 7472 616e 736c 6174 696f 6e5f 6e67  n translation_ng
+00020e70: 7261 6d5f 636f 756e 7473 3a0a 2020 2020  ram_counts:.    
+00020e80: 2020 2020 2020 2020 706f 7373 6962 6c65          possible
+00020e90: 5f6d 6174 6368 6573 5f62 795f 6f72 6465  _matches_by_orde
+00020ea0: 725b 6c65 6e28 6e67 7261 6d29 202d 2031  r[len(ngram) - 1
+00020eb0: 5d20 2b3d 2074 7261 6e73 6c61 7469 6f6e  ] += translation
+00020ec0: 5f6e 6772 616d 5f63 6f75 6e74 735b 6e67  _ngram_counts[ng
+00020ed0: 7261 6d5d 0a0a 2020 2020 7072 6563 6973  ram]..    precis
+00020ee0: 696f 6e73 203d 205b 302e 305d 202a 206d  ions = [0.0] * m
+00020ef0: 6178 5f6f 7264 6572 0a20 2020 2073 6d6f  ax_order.    smo
+00020f00: 6f74 6820 3d20 312e 300a 2020 2020 666f  oth = 1.0.    fo
+00020f10: 7220 6920 696e 2072 616e 6765 2830 2c20  r i in range(0, 
+00020f20: 6d61 785f 6f72 6465 7229 3a0a 2020 2020  max_order):.    
+00020f30: 2020 2020 6966 2070 6f73 7369 626c 655f      if possible_
+00020f40: 6d61 7463 6865 735f 6279 5f6f 7264 6572  matches_by_order
+00020f50: 5b69 5d20 3e20 303a 0a20 2020 2020 2020  [i] > 0:.       
+00020f60: 2020 2020 2070 7265 6369 7369 6f6e 735b       precisions[
+00020f70: 695d 203d 206d 6174 6368 6573 5f62 795f  i] = matches_by_
+00020f80: 6f72 6465 725b 695d 202f 2070 6f73 7369  order[i] / possi
+00020f90: 626c 655f 6d61 7463 6865 735f 6279 5f6f  ble_matches_by_o
+00020fa0: 7264 6572 5b69 5d0a 2020 2020 2020 2020  rder[i].        
+00020fb0: 2020 2020 6966 206d 6174 6368 6573 5f62      if matches_b
+00020fc0: 795f 6f72 6465 725b 695d 203e 2030 3a0a  y_order[i] > 0:.
+00020fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00020fe0: 7072 6563 6973 696f 6e73 5b69 5d20 3d20  precisions[i] = 
+00020ff0: 6d61 7463 6865 735f 6279 5f6f 7264 6572  matches_by_order
+00021000: 5b69 5d20 2f20 706f 7373 6962 6c65 5f6d  [i] / possible_m
+00021010: 6174 6368 6573 5f62 795f 6f72 6465 725b  atches_by_order[
+00021020: 695d 0a20 2020 2020 2020 2020 2020 2065  i].            e
+00021030: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00021040: 2020 2020 2073 6d6f 6f74 6820 2a3d 2032       smooth *= 2
+00021050: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00021060: 2070 7265 6369 7369 6f6e 735b 695d 203d   precisions[i] =
+00021070: 2031 2e30 202f 2028 736d 6f6f 7468 202a   1.0 / (smooth *
+00021080: 2070 6f73 7369 626c 655f 6d61 7463 6865   possible_matche
+00021090: 735f 6279 5f6f 7264 6572 5b69 5d29 0a20  s_by_order[i]). 
 000210a0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-000210b0: 2020 2020 2020 2020 2020 2020 2073 6d6f               smo
-000210c0: 6f74 6820 2a3d 2032 0a20 2020 2020 2020  oth *= 2.       
-000210d0: 2020 2020 2020 2020 2070 7265 6369 7369           precisi
-000210e0: 6f6e 735b 695d 203d 2031 2e30 202f 2028  ons[i] = 1.0 / (
-000210f0: 736d 6f6f 7468 202a 2070 6f73 7369 626c  smooth * possibl
-00021100: 655f 6d61 7463 6865 735f 6279 5f6f 7264  e_matches_by_ord
-00021110: 6572 5b69 5d29 0a20 2020 2020 2020 2065  er[i]).        e
-00021120: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00021130: 2070 7265 6369 7369 6f6e 735b 695d 203d   precisions[i] =
-00021140: 2030 2e30 0a0a 2020 2020 6966 206d 6178   0.0..    if max
-00021150: 2870 7265 6369 7369 6f6e 7329 203e 2030  (precisions) > 0
-00021160: 3a0a 2020 2020 2020 2020 705f 6c6f 675f  :.        p_log_
-00021170: 7375 6d20 3d20 7375 6d28 6d61 7468 2e6c  sum = sum(math.l
-00021180: 6f67 2870 2920 666f 7220 7020 696e 2070  og(p) for p in p
-00021190: 7265 6369 7369 6f6e 7320 6966 2070 290a  recisions if p).
-000211a0: 2020 2020 2020 2020 6765 6f5f 6d65 616e          geo_mean
-000211b0: 203d 206d 6174 682e 6578 7028 705f 6c6f   = math.exp(p_lo
-000211c0: 675f 7375 6d20 2f20 6d61 785f 6f72 6465  g_sum / max_orde
-000211d0: 7229 0a0a 2020 2020 6966 2075 7365 5f62  r)..    if use_b
-000211e0: 703a 0a20 2020 2020 2020 2072 6174 696f  p:.        ratio
-000211f0: 203d 2074 7261 6e73 6c61 7469 6f6e 5f6c   = translation_l
-00021200: 656e 6774 6820 2f20 7265 6665 7265 6e63  ength / referenc
-00021210: 655f 6c65 6e67 7468 0a20 2020 2020 2020  e_length.       
-00021220: 2069 6620 7261 7469 6f20 3c20 3165 2d33   if ratio < 1e-3
-00021230: 303a 0a20 2020 2020 2020 2020 2020 2062  0:.            b
-00021240: 7020 3d20 302e 300a 2020 2020 2020 2020  p = 0.0.        
-00021250: 656c 6966 2072 6174 696f 203c 2031 2e30  elif ratio < 1.0
-00021260: 3a0a 2020 2020 2020 2020 2020 2020 6270  :.            bp
-00021270: 203d 206d 6174 682e 6578 7028 3120 2d20   = math.exp(1 - 
-00021280: 312e 3020 2f20 7261 7469 6f29 0a20 2020  1.0 / ratio).   
-00021290: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-000212a0: 2020 2020 2020 2062 7020 3d20 312e 300a         bp = 1.0.
-000212b0: 2020 2020 626c 6575 203d 2067 656f 5f6d      bleu = geo_m
-000212c0: 6561 6e20 2a20 6270 0a20 2020 2072 6574  ean * bp.    ret
-000212d0: 7572 6e20 6e70 2e66 6c6f 6174 3332 2862  urn np.float32(b
-000212e0: 6c65 7529 0a0a 0a23 206e 6f69 6e73 7065  leu)...# noinspe
-000212f0: 6374 696f 6e20 5079 5061 636b 6167 6552  ction PyPackageR
-00021300: 6571 7569 7265 6d65 6e74 730a 6465 6620  equirements.def 
-00021310: 6d6f 6e6b 6579 6669 785f 676c 6962 2829  monkeyfix_glib()
-00021320: 3a0a 2020 2020 2222 220a 2020 2020 4669  :.    """.    Fi
-00021330: 7865 7320 736f 6d65 2073 7475 7069 6420  xes some stupid 
-00021340: 6275 6773 2073 7563 6820 7468 6174 2053  bugs such that S
-00021350: 4947 494e 5420 6973 206e 6f74 2077 6f72  IGINT is not wor
-00021360: 6b69 6e67 2e0a 2020 2020 5468 6973 2069  king..    This i
-00021370: 7320 7573 6564 2062 7920 6175 6469 6f72  s used by audior
-00021380: 6561 642c 2061 6e64 2069 6e64 6972 6563  ead, and indirec
-00021390: 746c 7920 6279 206c 6962 726f 7361 2066  tly by librosa f
-000213a0: 6f72 206c 6f61 6469 6e67 2061 7564 696f  or loading audio
-000213b0: 2e0a 2020 2020 6874 7470 733a 2f2f 7374  ..    https://st
-000213c0: 6163 6b6f 7665 7266 6c6f 772e 636f 6d2f  ackoverflow.com/
-000213d0: 7175 6573 7469 6f6e 732f 3136 3431 3038  questions/164108
-000213e0: 3532 2f0a 2020 2020 5365 6520 616c 736f  52/.    See also
-000213f0: 203a 6675 6e63 3a60 6d6f 6e6b 6579 7061   :func:`monkeypa
-00021400: 7463 685f 6175 6469 6f72 6561 6460 2e0a  tch_audioread`..
-00021410: 2020 2020 2222 220a 2020 2020 7472 793a      """.    try:
-00021420: 0a20 2020 2020 2020 2069 6d70 6f72 7420  .        import 
-00021430: 6769 0a20 2020 2065 7863 6570 7420 496d  gi.    except Im
-00021440: 706f 7274 4572 726f 723a 0a20 2020 2020  portError:.     
-00021450: 2020 2072 6574 7572 6e0a 2020 2020 7472     return.    tr
-00021460: 793a 0a20 2020 2020 2020 2066 726f 6d20  y:.        from 
-00021470: 6769 2e72 6570 6f73 6974 6f72 7920 696d  gi.repository im
-00021480: 706f 7274 2047 4c69 620a 2020 2020 6578  port GLib.    ex
-00021490: 6365 7074 2049 6d70 6f72 7445 7272 6f72  cept ImportError
-000214a0: 3a0a 2020 2020 2020 2020 2320 6e6f 696e  :.        # noin
-000214b0: 7370 6563 7469 6f6e 2050 7955 6e72 6573  spection PyUnres
-000214c0: 6f6c 7665 6452 6566 6572 656e 6365 730a  olvedReferences.
-000214d0: 2020 2020 2020 2020 6672 6f6d 2067 692e          from gi.
-000214e0: 6f76 6572 7269 6465 7320 696d 706f 7274  overrides import
-000214f0: 2047 4c69 620a 2020 2020 2320 446f 206e   GLib.    # Do n
-00021500: 6f74 6869 6e67 2e0a 2020 2020 2320 5468  othing..    # Th
-00021510: 6520 6f72 6967 696e 616c 2062 6568 6176  e original behav
-00021520: 696f 7220 776f 756c 6420 696e 7374 616c  ior would instal
-00021530: 6c20 6120 5349 4749 4e54 2068 616e 646c  l a SIGINT handl
-00021540: 6572 2077 6869 6368 2063 616c 6c73 2047  er which calls G
-00021550: 4c69 622e 4d61 696e 4c6f 6f70 2e71 7569  Lib.MainLoop.qui
-00021560: 7428 292c 0a20 2020 2023 2061 6e64 2074  t(),.    # and t
-00021570: 6865 6e20 7265 7261 6973 6520 6120 4b65  hen reraise a Ke
-00021580: 7962 6f61 7264 496e 7465 7272 7570 7420  yboardInterrupt 
-00021590: 696e 2074 6861 7420 7468 7265 6164 2e0a  in that thread..
-000215a0: 2020 2020 2320 486f 7765 7665 722c 2077      # However, w
-000215b0: 6520 7761 6e74 2061 6e64 2065 7870 6563  e want and expec
-000215c0: 7420 746f 2067 6574 2074 6865 204b 6579  t to get the Key
-000215d0: 626f 6172 6449 6e74 6572 7275 7074 2069  boardInterrupt i
-000215e0: 6e20 7468 6520 6d61 696e 2074 6872 6561  n the main threa
-000215f0: 642e 0a20 2020 2047 4c69 622e 4d61 696e  d..    GLib.Main
-00021600: 4c6f 6f70 2e5f 5f69 6e69 745f 5f20 3d20  Loop.__init__ = 
-00021610: 6c61 6d62 6461 202a 6172 6773 2c20 2a2a  lambda *args, **
-00021620: 6b77 6172 6773 3a20 4e6f 6e65 0a0a 0a64  kwargs: None...d
-00021630: 6566 206d 6f6e 6b65 7970 6174 6368 5f61  ef monkeypatch_a
-00021640: 7564 696f 7265 6164 2829 3a0a 2020 2020  udioread():.    
-00021650: 2222 220a 2020 2020 6175 6469 6f72 6561  """.    audiorea
-00021660: 6420 646f 6573 206e 6f74 2062 6568 6176  d does not behav
-00021670: 6520 6f70 7469 6d61 6c20 696e 2073 6f6d  e optimal in som
-00021680: 6520 6361 7365 732e 0a20 2020 2045 2e67  e cases..    E.g
-00021690: 2e20 6561 6368 2063 616c 6c20 746f 205f  . each call to _
-000216a0: 6361 5f61 7661 696c 6162 6c65 2829 2074  ca_available() t
-000216b0: 616b 6573 2071 7569 7465 206c 6f6e 6720  akes quite long 
-000216c0: 6265 6361 7573 6520 6f66 2074 6865 2063  because of the c
-000216d0: 7479 7065 732e 7574 696c 2e66 696e 645f  types.util.find_
-000216e0: 6c69 6272 6172 7920 7573 6167 652e 0a20  library usage.. 
-000216f0: 2020 2057 6520 7769 6c6c 2070 6174 6368     We will patch
-00021700: 2074 6869 732e 0a0a 2020 2020 486f 7765   this...    Howe
-00021710: 7665 722c 2074 6865 2072 6563 6f6d 6d65  ver, the recomme
-00021720: 6e64 6174 696f 6e20 776f 756c 6420 6265  ndation would be
-00021730: 2074 6f20 6e6f 7420 7573 6520 6175 6469   to not use audi
-00021740: 6f72 6561 6420 286c 6962 726f 7361 2e6c  oread (librosa.l
-00021750: 6f61 6429 2e0a 2020 2020 6175 6469 6f72  oad)..    audior
-00021760: 6561 6420 7573 6573 2047 7374 7265 616d  ead uses Gstream
-00021770: 6572 2061 7320 6120 6261 636b 656e 6420  er as a backend 
-00021780: 6279 2064 6566 6175 6c74 2063 7572 7265  by default curre
-00021790: 6e74 6c79 2028 6f6e 204c 696e 7578 292e  ntly (on Linux).
-000217a0: 0a20 2020 2047 7374 7265 616d 6572 2068  .    Gstreamer h
-000217b0: 6173 206d 756c 7469 706c 6520 6973 7375  as multiple issu
-000217c0: 6573 2e20 5365 6520 616c 736f 203a 6675  es. See also :fu
-000217d0: 6e63 3a60 6d6f 6e6b 6579 6669 785f 676c  nc:`monkeyfix_gl
-000217e0: 6962 602c 2061 6e64 2068 6572 6520 666f  ib`, and here fo
-000217f0: 7220 6469 7363 7573 7369 6f6e 3a0a 2020  r discussion:.  
-00021800: 2020 6874 7470 733a 2f2f 6769 7468 7562    https://github
-00021810: 2e63 6f6d 2f62 6565 7462 6f78 2f61 7564  .com/beetbox/aud
-00021820: 696f 7265 6164 2f69 7373 7565 732f 3632  ioread/issues/62
-00021830: 0a20 2020 2068 7474 7073 3a2f 2f67 6974  .    https://git
-00021840: 6875 622e 636f 6d2f 6265 6574 626f 782f  hub.com/beetbox/
-00021850: 6175 6469 6f72 6561 642f 6973 7375 6573  audioread/issues
-00021860: 2f36 330a 0a20 2020 2049 6e73 7465 6164  /63..    Instead
-00021870: 2c20 7573 6520 5079 536f 756e 6446 696c  , use PySoundFil
-00021880: 652c 2077 6869 6368 2069 7320 616c 736f  e, which is also
-00021890: 2066 6173 7465 722e 2053 6565 2068 6572   faster. See her
-000218a0: 6520 666f 7220 6469 7363 7573 7369 6f6e  e for discussion
-000218b0: 733a 0a20 2020 2068 7474 7073 3a2f 2f67  s:.    https://g
-000218c0: 6974 6875 622e 636f 6d2f 6265 6574 626f  ithub.com/beetbo
-000218d0: 782f 6175 6469 6f72 6561 642f 6973 7375  x/audioread/issu
-000218e0: 6573 2f36 340a 2020 2020 6874 7470 733a  es/64.    https:
-000218f0: 2f2f 6769 7468 7562 2e63 6f6d 2f6c 6962  //github.com/lib
-00021900: 726f 7361 2f6c 6962 726f 7361 2f69 7373  rosa/librosa/iss
-00021910: 7565 732f 3638 310a 2020 2020 2222 220a  ues/681.    """.
-00021920: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-00021930: 2023 206e 6f69 6e73 7065 6374 696f 6e20   # noinspection 
-00021940: 5079 5061 636b 6167 6552 6571 7569 7265  PyPackageRequire
-00021950: 6d65 6e74 730a 2020 2020 2020 2020 696d  ments.        im
-00021960: 706f 7274 2061 7564 696f 7265 6164 0a20  port audioread. 
-00021970: 2020 2065 7863 6570 7420 496d 706f 7274     except Import
-00021980: 4572 726f 723a 0a20 2020 2020 2020 2072  Error:.        r
-00021990: 6574 7572 6e0a 2020 2020 2320 6e6f 696e  eturn.    # noin
-000219a0: 7370 6563 7469 6f6e 2050 7950 726f 7465  spection PyProte
-000219b0: 6374 6564 4d65 6d62 6572 0a20 2020 2072  ctedMember.    r
-000219c0: 6573 203d 2061 7564 696f 7265 6164 2e5f  es = audioread._
-000219d0: 6361 5f61 7661 696c 6162 6c65 2829 0a20  ca_available(). 
-000219e0: 2020 2061 7564 696f 7265 6164 2e5f 6361     audioread._ca
-000219f0: 5f61 7661 696c 6162 6c65 203d 206c 616d  _available = lam
-00021a00: 6264 613a 2072 6573 0a0a 0a5f 6366 5f63  bda: res..._cf_c
-00021a10: 6163 6865 203d 207b 7d0a 5f63 665f 6d73  ache = {}._cf_ms
-00021a20: 675f 7072 696e 7465 6420 3d20 4661 6c73  g_printed = Fals
-00021a30: 650a 0a0a 6465 6620 6366 2866 696c 656e  e...def cf(filen
-00021a40: 616d 6529 3a0a 2020 2020 2222 220a 2020  ame):.    """.  
-00021a50: 2020 4361 6368 6520 6d61 6e61 6765 722e    Cache manager.
-00021a60: 2069 3620 7370 6563 6966 6963 2e0a 0a20   i6 specific... 
-00021a70: 2020 203a 7265 7475 726e 3a20 6669 6c65     :return: file
-00021a80: 6e61 6d65 0a20 2020 203a 7274 7970 653a  name.    :rtype:
-00021a90: 2073 7472 0a20 2020 2022 2222 0a20 2020   str.    """.   
-00021aa0: 2067 6c6f 6261 6c20 5f63 665f 6d73 675f   global _cf_msg_
-00021ab0: 7072 696e 7465 640a 2020 2020 696d 706f  printed.    impo
-00021ac0: 7274 206f 730a 2020 2020 6672 6f6d 2073  rt os.    from s
-00021ad0: 7562 7072 6f63 6573 7320 696d 706f 7274  ubprocess import
-00021ae0: 2063 6865 636b 5f6f 7574 7075 740a 0a20   check_output.. 
-00021af0: 2020 2069 6620 6669 6c65 6e61 6d65 2069     if filename i
-00021b00: 6e20 5f63 665f 6361 6368 653a 0a20 2020  n _cf_cache:.   
-00021b10: 2020 2020 2072 6574 7572 6e20 5f63 665f       return _cf_
-00021b20: 6361 6368 655b 6669 6c65 6e61 6d65 5d0a  cache[filename].
-00021b30: 2020 2020 6465 6275 675f 6d6f 6465 203d      debug_mode =
-00021b40: 2069 6e74 286f 732e 656e 7669 726f 6e2e   int(os.environ.
-00021b50: 6765 7428 2244 4542 5547 222c 2030 2929  get("DEBUG", 0))
-00021b60: 0a20 2020 2069 6620 6465 6275 675f 6d6f  .    if debug_mo
-00021b70: 6465 206f 7220 6765 745f 686f 7374 6e61  de or get_hostna
-00021b80: 6d65 2829 203d 3d20 2263 6c75 7374 6572  me() == "cluster
-00021b90: 2d63 6e2d 3231 3122 206f 7220 6e6f 7420  -cn-211" or not 
-00021ba0: 6973 5f72 756e 6e69 6e67 5f6f 6e5f 636c  is_running_on_cl
-00021bb0: 7573 7465 7228 293a 0a20 2020 2020 2020  uster():.       
-00021bc0: 2069 6620 6e6f 7420 5f63 665f 6d73 675f   if not _cf_msg_
-00021bd0: 7072 696e 7465 643a 0a20 2020 2020 2020  printed:.       
-00021be0: 2020 2020 2070 7269 6e74 2822 4361 6368       print("Cach
-00021bf0: 6520 6d61 6e61 6765 723a 206e 6f74 2075  e manager: not u
-00021c00: 7365 642c 2075 7365 206c 6f63 616c 2066  sed, use local f
-00021c10: 696c 653a 2025 7320 2864 6973 6361 7264  ile: %s (discard
-00021c20: 2066 7572 7468 6572 206d 6573 7361 6765   further message
-00021c30: 7329 2220 2520 6669 6c65 6e61 6d65 290a  s)" % filename).
-00021c40: 2020 2020 2020 2020 2020 2020 5f63 665f              _cf_
-00021c50: 6d73 675f 7072 696e 7465 6420 3d20 5472  msg_printed = Tr
-00021c60: 7565 0a20 2020 2020 2020 2072 6574 7572  ue.        retur
-00021c70: 6e20 6669 6c65 6e61 6d65 2020 2320 666f  n filename  # fo
-00021c80: 7220 6465 6275 6767 696e 670a 2020 2020  r debugging.    
-00021c90: 7472 793a 0a20 2020 2020 2020 2063 6163  try:.        cac
-00021ca0: 6865 645f 666e 203d 2063 6865 636b 5f6f  hed_fn = check_o
-00021cb0: 7574 7075 7428 5b22 6366 222c 2066 696c  utput(["cf", fil
-00021cc0: 656e 616d 655d 292e 7374 7269 7028 292e  ename]).strip().
-00021cd0: 6465 636f 6465 2822 7574 6638 2229 0a20  decode("utf8"). 
-00021ce0: 2020 2065 7863 6570 7420 4361 6c6c 6564     except Called
-00021cf0: 5072 6f63 6573 7345 7272 6f72 3a0a 2020  ProcessError:.  
-00021d00: 2020 2020 2020 6966 206e 6f74 205f 6366        if not _cf
-00021d10: 5f6d 7367 5f70 7269 6e74 6564 3a0a 2020  _msg_printed:.  
-00021d20: 2020 2020 2020 2020 2020 7072 696e 7428            print(
-00021d30: 2243 6163 6865 206d 616e 6167 6572 3a20  "Cache manager: 
-00021d40: 4572 726f 7220 6f63 6375 7272 6564 2c20  Error occurred, 
-00021d50: 7573 696e 6720 6c6f 6361 6c20 6669 6c65  using local file
-00021d60: 2229 0a20 2020 2020 2020 2020 2020 205f  ").            _
-00021d70: 6366 5f6d 7367 5f70 7269 6e74 6564 203d  cf_msg_printed =
-00021d80: 2054 7275 650a 2020 2020 2020 2020 7265   True.        re
-00021d90: 7475 726e 2066 696c 656e 616d 650a 2020  turn filename.  
-00021da0: 2020 6173 7365 7274 206f 732e 7061 7468    assert os.path
-00021db0: 2e65 7869 7374 7328 6361 6368 6564 5f66  .exists(cached_f
-00021dc0: 6e29 0a20 2020 205f 6366 5f63 6163 6865  n).    _cf_cache
-00021dd0: 5b66 696c 656e 616d 655d 203d 2063 6163  [filename] = cac
-00021de0: 6865 645f 666e 0a20 2020 2072 6574 7572  hed_fn.    retur
-00021df0: 6e20 6361 6368 6564 5f66 6e0a 0a0a 6465  n cached_fn...de
-00021e00: 6620 6269 6e61 7279 5f73 6561 7263 685f  f binary_search_
-00021e10: 616e 7928 636d 702c 206c 6f77 2c20 6869  any(cmp, low, hi
-00021e20: 6768 293a 0a20 2020 2022 2222 0a20 2020  gh):.    """.   
-00021e30: 2042 696e 6172 7920 7365 6172 6368 2066   Binary search f
-00021e40: 6f72 2061 2063 7573 746f 6d20 636f 6d70  or a custom comp
-00021e50: 6172 6520 6675 6e63 7469 6f6e 2e0a 0a20  are function... 
-00021e60: 2020 203a 7061 7261 6d20 2869 6e74 292d     :param (int)-
-00021e70: 3e69 6e74 2063 6d70 3a20 652e 672e 2063  >int cmp: e.g. c
-00021e80: 6d70 2869 6478 2920 3d3d 2063 6f6d 7061  mp(idx) == compa
-00021e90: 7265 2861 7272 6179 5b69 6478 5d2c 206b  re(array[idx], k
-00021ea0: 6579 290a 2020 2020 3a70 6172 616d 2069  ey).    :param i
-00021eb0: 6e74 206c 6f77 3a20 696e 636c 7573 6976  nt low: inclusiv
-00021ec0: 650a 2020 2020 3a70 6172 616d 2069 6e74  e.    :param int
-00021ed0: 2068 6967 683a 2065 7863 6c75 7369 7665   high: exclusive
-00021ee0: 0a20 2020 203a 7274 7970 653a 2069 6e74  .    :rtype: int
-00021ef0: 7c4e 6f6e 650a 2020 2020 2222 220a 2020  |None.    """.  
-00021f00: 2020 7768 696c 6520 6c6f 7720 3c20 6869    while low < hi
-00021f10: 6768 3a0a 2020 2020 2020 2020 6d69 6420  gh:.        mid 
-00021f20: 3d20 286c 6f77 202b 2068 6967 6829 202f  = (low + high) /
-00021f30: 2f20 320a 2020 2020 2020 2020 7220 3d20  / 2.        r = 
-00021f40: 636d 7028 6d69 6429 0a20 2020 2020 2020  cmp(mid).       
-00021f50: 2069 6620 7220 3c20 303a 0a20 2020 2020   if r < 0:.     
-00021f60: 2020 2020 2020 206c 6f77 203d 206d 6964         low = mid
-00021f70: 202b 2031 0a20 2020 2020 2020 2065 6c69   + 1.        eli
-00021f80: 6620 7220 3e20 303a 0a20 2020 2020 2020  f r > 0:.       
-00021f90: 2020 2020 2068 6967 6820 3d20 6d69 640a       high = mid.
-00021fa0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00021fb0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00021fc0: 206d 6964 0a20 2020 2072 6574 7572 6e20   mid.    return 
-00021fd0: 6c6f 770a 0a0a 6465 6620 6765 6e65 7269  low...def generi
-00021fe0: 635f 696d 706f 7274 5f6d 6f64 756c 6528  c_import_module(
-00021ff0: 6669 6c65 6e61 6d65 293a 0a20 2020 2022  filename):.    "
-00022000: 2222 0a20 2020 203a 7061 7261 6d20 7374  "".    :param st
-00022010: 7220 6669 6c65 6e61 6d65 3a0a 2020 2020  r filename:.    
-00022020: 2020 5765 2074 7279 2074 6f20 6265 2063    We try to be c
-00022030: 6c65 7665 7220 6162 6f75 7420 6669 6c65  lever about file
-00022040: 6e61 6d65 2e0a 2020 2020 2020 4966 2069  name..      If i
-00022050: 7420 6c6f 6f6b 7320 6c69 6b65 2061 206d  t looks like a m
-00022060: 6f64 756c 6520 6e61 6d65 2c20 6a75 7374  odule name, just
-00022070: 2064 6f20 696d 706f 7274 6c69 622e 696d   do importlib.im
-00022080: 706f 7274 5f6d 6f64 756c 652e 0a20 2020  port_module..   
-00022090: 2020 2049 6620 6974 206c 6f6f 6b73 206c     If it looks l
-000220a0: 696b 6520 6120 6669 6c65 6e61 6d65 2c20  ike a filename, 
-000220b0: 7365 6172 6368 2066 6f72 2061 2062 6173  search for a bas
-000220c0: 6520 7061 7468 2028 7768 6963 6820 646f  e path (which do
-000220d0: 6573 206e 6f74 2068 6176 6520 5f5f 696e  es not have __in
-000220e0: 6974 5f5f 2e70 7929 2c0a 2020 2020 2020  it__.py),.      
-000220f0: 6164 6420 7468 6174 2070 6174 6820 746f  add that path to
-00022100: 2073 7973 2e70 6174 6820 6966 206e 6565   sys.path if nee
-00022110: 6465 642c 2061 6e64 2069 6d70 6f72 7420  ded, and import 
-00022120: 7468 6520 7265 6d61 696e 696e 6720 7768  the remaining wh
-00022130: 6572 6520 222f 2220 6973 2072 6570 6c61  ere "/" is repla
-00022140: 6365 6420 6279 2022 2e22 0a20 2020 2020  ced by ".".     
-00022150: 2061 6e64 2074 6865 2066 696c 6520 6578   and the file ex
-00022160: 7465 6e73 696f 6e20 6973 2072 656d 6f76  tension is remov
-00022170: 6564 2e0a 2020 2020 3a72 6574 7572 6e3a  ed..    :return:
-00022180: 2074 6865 206d 6f64 756c 650a 2020 2020   the module.    
-00022190: 3a72 7479 7065 3a20 7479 7065 732e 4d6f  :rtype: types.Mo
-000221a0: 6475 6c65 5479 7065 0a20 2020 2022 2222  duleType.    """
-000221b0: 0a20 2020 2061 7373 6572 7420 6669 6c65  .    assert file
-000221c0: 6e61 6d65 0a20 2020 2069 6d70 6f72 7420  name.    import 
-000221d0: 696d 706f 7274 6c69 620a 0a20 2020 2069  importlib..    i
-000221e0: 6620 222f 2220 6e6f 7420 696e 2066 696c  f "/" not in fil
-000221f0: 656e 616d 653a 0a20 2020 2020 2020 2072  ename:.        r
-00022200: 6574 7572 6e20 696d 706f 7274 6c69 622e  eturn importlib.
-00022210: 696d 706f 7274 5f6d 6f64 756c 6528 6669  import_module(fi
-00022220: 6c65 6e61 6d65 290a 2020 2020 7072 6566  lename).    pref
-00022230: 6978 5f64 6972 203d 2022 220a 2020 2020  ix_dir = "".    
-00022240: 6966 206e 6f74 206f 732e 7061 7468 2e65  if not os.path.e
-00022250: 7869 7374 7328 6669 6c65 6e61 6d65 293a  xists(filename):
-00022260: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-00022270: 6669 6c65 6e61 6d65 5b30 5d20 213d 2022  filename[0] != "
-00022280: 2f22 0a20 2020 2020 2020 2023 204d 6179  /".        # May
-00022290: 6265 2072 656c 6174 6976 6520 746f 2052  be relative to R
-000222a0: 6574 7572 6e6e 3f0a 2020 2020 2020 2020  eturnn?.        
-000222b0: 7072 6566 6978 5f64 6972 203d 2022 2573  prefix_dir = "%s
-000222c0: 2f22 2025 2072 6574 7572 6e6e 5f72 6f6f  /" % returnn_roo
-000222d0: 745f 6469 720a 2020 2020 6173 7365 7274  t_dir.    assert
-000222e0: 206f 732e 7061 7468 2e65 7869 7374 7328   os.path.exists(
-000222f0: 7072 6566 6978 5f64 6972 202b 2066 696c  prefix_dir + fil
-00022300: 656e 616d 6529 0a20 2020 2061 7373 6572  ename).    asser
-00022310: 7420 6669 6c65 6e61 6d65 2e65 6e64 7377  t filename.endsw
-00022320: 6974 6828 222e 7079 2229 206f 7220 6f73  ith(".py") or os
-00022330: 2e70 6174 682e 6973 6469 7228 7072 6566  .path.isdir(pref
-00022340: 6978 5f64 6972 202b 2066 696c 656e 616d  ix_dir + filenam
-00022350: 6529 0a20 2020 2064 6972 7320 3d20 6669  e).    dirs = fi
-00022360: 6c65 6e61 6d65 2e73 706c 6974 2822 2f22  lename.split("/"
-00022370: 290a 2020 2020 6469 7273 2c20 6261 7365  ).    dirs, base
-00022380: 5f66 6e20 3d20 6469 7273 5b3a 2d31 5d2c  _fn = dirs[:-1],
-00022390: 2064 6972 735b 2d31 5d0a 2020 2020 6173   dirs[-1].    as
-000223a0: 7365 7274 206c 656e 2864 6972 7329 203e  sert len(dirs) >
-000223b0: 3d20 310a 2020 2020 666f 7220 6920 696e  = 1.    for i in
-000223c0: 2072 6576 6572 7365 6428 7261 6e67 6528   reversed(range(
-000223d0: 6c65 6e28 6469 7273 2929 293a 0a20 2020  len(dirs))):.   
-000223e0: 2020 2020 2064 203d 2070 7265 6669 785f       d = prefix_
-000223f0: 6469 7220 2b20 222f 222e 6a6f 696e 2864  dir + "/".join(d
-00022400: 6972 735b 3a20 6920 2b20 315d 290a 2020  irs[: i + 1]).  
-00022410: 2020 2020 2020 6173 7365 7274 206f 732e        assert os.
-00022420: 7061 7468 2e69 7364 6972 2864 290a 2020  path.isdir(d).  
-00022430: 2020 2020 2020 6966 206f 732e 7061 7468        if os.path
-00022440: 2e65 7869 7374 7328 2225 732f 5f5f 696e  .exists("%s/__in
-00022450: 6974 5f5f 2e70 7922 2025 2064 293a 0a20  it__.py" % d):. 
-00022460: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
-00022470: 6e75 650a 2020 2020 2020 2020 6966 2064  nue.        if d
-00022480: 206e 6f74 2069 6e20 7379 732e 7061 7468   not in sys.path
-00022490: 3a0a 2020 2020 2020 2020 2020 2020 7379  :.            sy
-000224a0: 732e 7061 7468 2e61 7070 656e 6428 6429  s.path.append(d)
-000224b0: 0a20 2020 2020 2020 206d 203d 2022 2e22  .        m = "."
-000224c0: 2e6a 6f69 6e28 6469 7273 5b69 202b 2031  .join(dirs[i + 1
-000224d0: 203a 5d20 2b20 5b62 6173 655f 666e 5d29   :] + [base_fn])
-000224e0: 0a20 2020 2020 2020 2069 6620 6261 7365  .        if base
-000224f0: 5f66 6e2e 656e 6473 7769 7468 2822 2e70  _fn.endswith(".p
-00022500: 7922 293a 0a20 2020 2020 2020 2020 2020  y"):.           
-00022510: 206d 203d 206d 5b3a 2d33 5d0a 2020 2020   m = m[:-3].    
-00022520: 2020 2020 7265 7475 726e 2069 6d70 6f72      return impor
-00022530: 746c 6962 2e69 6d70 6f72 745f 6d6f 6475  tlib.import_modu
-00022540: 6c65 286d 290a 2020 2020 7261 6973 6520  le(m).    raise 
-00022550: 5661 6c75 6545 7272 6f72 2822 6361 6e6e  ValueError("cann
-00022560: 6f74 2066 6967 7572 6520 6f75 7420 6261  ot figure out ba
-00022570: 7365 206d 6f64 756c 6520 7061 7468 2066  se module path f
-00022580: 726f 6d20 2572 2220 2520 6669 6c65 6e61  rom %r" % filena
-00022590: 6d65 290a 0a0a 6465 6620 736f 6674 6d61  me)...def softma
-000225a0: 7828 782c 2061 7869 733d 4e6f 6e65 293a  x(x, axis=None):
-000225b0: 0a20 2020 2022 2222 0a20 2020 203a 7061  .    """.    :pa
-000225c0: 7261 6d20 6e75 6d70 792e 6e64 6172 7261  ram numpy.ndarra
-000225d0: 7920 783a 0a20 2020 203a 7061 7261 6d20  y x:.    :param 
-000225e0: 696e 747c 4e6f 6e65 2061 7869 733a 0a20  int|None axis:. 
-000225f0: 2020 203a 7274 7970 653a 206e 756d 7079     :rtype: numpy
-00022600: 2e6e 6461 7272 6179 0a20 2020 2022 2222  .ndarray.    """
-00022610: 0a20 2020 2069 6d70 6f72 7420 6e75 6d70  .    import nump
-00022620: 790a 0a20 2020 2065 5f78 203d 206e 756d  y..    e_x = num
-00022630: 7079 2e65 7870 2878 202d 206e 756d 7079  py.exp(x - numpy
-00022640: 2e6d 6178 2878 2c20 6178 6973 3d61 7869  .max(x, axis=axi
-00022650: 732c 206b 6565 7064 696d 733d 5472 7565  s, keepdims=True
-00022660: 2929 0a20 2020 2072 6574 7572 6e20 655f  )).    return e_
-00022670: 7820 2f20 6e75 6d70 792e 7375 6d28 655f  x / numpy.sum(e_
-00022680: 782c 2061 7869 733d 6178 6973 2c20 6b65  x, axis=axis, ke
-00022690: 6570 6469 6d73 3d54 7275 6529 0a0a 0a64  epdims=True)...d
-000226a0: 6566 2063 6f6c 6c65 6374 5f70 726f 635f  ef collect_proc_
-000226b0: 6d61 7073 5f65 7865 635f 6669 6c65 7328  maps_exec_files(
-000226c0: 293a 0a20 2020 2022 2222 0a20 2020 2043  ):.    """.    C
-000226d0: 7572 7265 6e74 6c79 206f 6e6c 7920 776f  urrently only wo
-000226e0: 726b 7320 6f6e 204c 696e 7578 2e2e 2e0a  rks on Linux....
-000226f0: 0a20 2020 203a 7265 7475 726e 3a20 6c69  .    :return: li
-00022700: 7374 206f 6620 6d61 7070 6564 2065 7865  st of mapped exe
-00022710: 6375 7461 626c 6573 2028 6c69 6273 290a  cutables (libs).
-00022720: 2020 2020 3a72 7479 7065 3a20 6c69 7374      :rtype: list
-00022730: 5b73 7472 5d0a 2020 2020 2222 220a 2020  [str].    """.  
-00022740: 2020 696d 706f 7274 2072 650a 0a20 2020    import re..   
-00022750: 2070 6964 203d 206f 732e 6765 7470 6964   pid = os.getpid
-00022760: 2829 0a20 2020 2066 6e73 203d 205b 5d0a  ().    fns = [].
-00022770: 2020 2020 666f 7220 6c69 6e65 2069 6e20      for line in 
-00022780: 6f70 656e 2822 2f70 726f 632f 2569 2f6d  open("/proc/%i/m
-00022790: 6170 7322 2025 2070 6964 2c20 2272 2229  aps" % pid, "r")
-000227a0: 2e72 6561 6428 292e 7370 6c69 746c 696e  .read().splitlin
-000227b0: 6573 2829 3a20 2023 2066 6f72 2065 6163  es():  # for eac
-000227c0: 6820 6d61 7070 6564 2072 6567 696f 6e0a  h mapped region.
-000227d0: 2020 2020 2020 2020 2320 6874 7470 733a          # https:
-000227e0: 2f2f 7374 6163 6b6f 7665 7266 6c6f 772e  //stackoverflow.
-000227f0: 636f 6d2f 7175 6573 7469 6f6e 732f 3134  com/questions/14
-00022800: 3031 3335 392f 756e 6465 7273 7461 6e64  01359/understand
-00022810: 696e 672d 6c69 6e75 782d 7072 6f63 2d69  ing-linux-proc-i
-00022820: 642d 6d61 7073 0a20 2020 2020 2020 2023  d-maps.        #
-00022830: 2061 6464 7265 7373 2020 2020 2020 2020   address        
-00022840: 2020 2070 6572 6d73 206f 6666 7365 7420     perms offset 
-00022850: 2064 6576 2020 2069 6e6f 6465 2020 2070   dev   inode   p
-00022860: 6174 686e 616d 650a 2020 2020 2020 2020  athname.        
-00022870: 2320 452e 672e 3a0a 2020 2020 2020 2020  # E.g.:.        
-00022880: 2320 3766 6632 6465 3931 6330 3030 2d37  # 7ff2de91c000-7
-00022890: 6666 3264 6539 3165 3030 3020 7277 2d70  ff2de91e000 rw-p
-000228a0: 2030 3031 3763 3030 3020 3038 3a30 3220   0017c000 08:02 
-000228b0: 3739 3438 3434 2020 2020 2020 2020 2020  794844          
-000228c0: 2020 2020 2020 2020 2020 202f 7573 722f             /usr/
-000228d0: 6c69 622f 7838 365f 3634 2d6c 696e 7578  lib/x86_64-linux
-000228e0: 2d67 6e75 2f6c 6962 7374 6463 2b2e 2e2e  -gnu/libstdc+...
-000228f0: 0a20 2020 2020 2020 206d 203d 2072 652e  .        m = re.
-00022900: 6d61 7463 6828 0a20 2020 2020 2020 2020  match(.         
-00022910: 2020 2072 225e 285b 302d 3941 2d46 612d     r"^([0-9A-Fa-
-00022920: 665d 2b29 2d28 5b30 2d39 412d 4661 2d66  f]+)-([0-9A-Fa-f
-00022930: 5d2b 295c 732b 285b 7277 7870 735c 2d5d  ]+)\s+([rwxps\-]
-00022940: 2b29 5c73 2b28 5b30 2d39 412d 4661 2d66  +)\s+([0-9A-Fa-f
-00022950: 5d2b 295c 732b 285b 302d 3941 2d46 612d  ]+)\s+([0-9A-Fa-
-00022960: 663a 5d2b 295c 732b 285b 302d 395d 2b29  f:]+)\s+([0-9]+)
-00022970: 5c73 2a28 2e2a 2924 222c 206c 696e 650a  \s*(.*)$", line.
-00022980: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00022990: 2020 6173 7365 7274 206d 2c20 226e 6f20    assert m, "no 
-000229a0: 6d61 7463 6820 666f 7220 2572 2220 2520  match for %r" % 
-000229b0: 6c69 6e65 0a20 2020 2020 2020 2061 6464  line.        add
-000229c0: 7265 7373 5f73 7461 7274 2c20 6164 6472  ress_start, addr
-000229d0: 6573 735f 656e 642c 2070 6572 6d73 2c20  ess_end, perms, 
-000229e0: 6f66 6673 6574 2c20 6465 762c 2069 5f6e  offset, dev, i_n
-000229f0: 6f64 652c 2070 6174 685f 6e61 6d65 203d  ode, path_name =
-00022a00: 206d 2e67 726f 7570 7328 290a 2020 2020   m.groups().    
-00022a10: 2020 2020 6966 2022 7822 206e 6f74 2069      if "x" not i
-00022a20: 6e20 7065 726d 733a 0a20 2020 2020 2020  n perms:.       
-00022a30: 2020 2020 2063 6f6e 7469 6e75 650a 2020       continue.  
-00022a40: 2020 2020 2020 6966 206e 6f74 2070 6174        if not pat
-00022a50: 685f 6e61 6d65 206f 7220 7061 7468 5f6e  h_name or path_n
-00022a60: 616d 652e 7374 6172 7473 7769 7468 2822  ame.startswith("
-00022a70: 5b22 2920 6f72 2022 2864 656c 6574 6564  [") or "(deleted
-00022a80: 2922 2069 6e20 7061 7468 5f6e 616d 653a  )" in path_name:
-00022a90: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
-00022aa0: 7469 6e75 650a 2020 2020 2020 2020 6966  tinue.        if
-00022ab0: 2070 6174 685f 6e61 6d65 206e 6f74 2069   path_name not i
-00022ac0: 6e20 666e 733a 0a20 2020 2020 2020 2020  n fns:.         
-00022ad0: 2020 2066 6e73 2e61 7070 656e 6428 7061     fns.append(pa
-00022ae0: 7468 5f6e 616d 6529 0a20 2020 2072 6574  th_name).    ret
-00022af0: 7572 6e20 666e 730a 0a0a 6465 6620 6669  urn fns...def fi
-00022b00: 6e64 5f73 796d 5f69 6e5f 6578 6563 2866  nd_sym_in_exec(f
-00022b10: 6e2c 2073 796d 293a 0a20 2020 2022 2222  n, sym):.    """
-00022b20: 0a20 2020 2055 7365 7320 6060 6f62 6a64  .    Uses ``objd
-00022b30: 756d 7060 6020 746f 206c 6973 7420 6176  ump`` to list av
-00022b40: 6169 6c61 626c 6520 7379 6d62 6f6c 732c  ailable symbols,
-00022b50: 2061 6e64 2066 696c 7465 7273 2074 6865   and filters the
-00022b60: 6d20 6279 2074 6865 2067 6976 656e 2060  m by the given `
-00022b70: 6073 796d 6060 2e0a 0a20 2020 203a 7061  `sym``...    :pa
-00022b80: 7261 6d20 7374 7220 666e 3a20 7061 7468  ram str fn: path
-00022b90: 0a20 2020 203a 7061 7261 6d20 7374 7220  .    :param str 
-00022ba0: 7379 6d3a 0a20 2020 203a 7265 7475 726e  sym:.    :return
-00022bb0: 3a20 6d61 7463 6865 6420 6f75 742c 206f  : matched out, o
-00022bc0: 7220 4e6f 6e65 0a20 2020 203a 7274 7970  r None.    :rtyp
-00022bd0: 653a 2073 7472 7c4e 6f6e 650a 2020 2020  e: str|None.    
-00022be0: 2222 220a 2020 2020 6672 6f6d 2073 7562  """.    from sub
-00022bf0: 7072 6f63 6573 7320 696d 706f 7274 2043  process import C
-00022c00: 616c 6c65 6450 726f 6365 7373 4572 726f  alledProcessErro
-00022c10: 720a 0a20 2020 206f 626a 6475 6d70 203d  r..    objdump =
-00022c20: 2022 6f62 6a64 756d 7020 2d54 220a 2020   "objdump -T".  
-00022c30: 2020 6966 2073 7973 2e70 6c61 7466 6f72    if sys.platfor
-00022c40: 6d20 3d3d 2022 6461 7277 696e 223a 0a20  m == "darwin":. 
-00022c50: 2020 2020 2020 206f 626a 6475 6d70 203d         objdump =
-00022c60: 2022 6f74 6f6f 6c20 2d49 4847 7622 0a20   "otool -IHGv". 
-00022c70: 2020 2073 6865 6c6c 5f63 6d64 203d 2022     shell_cmd = "
-00022c80: 2573 2025 7320 7c20 6772 6570 2025 7322  %s %s | grep %s"
-00022c90: 2025 2028 6f62 6a64 756d 702c 2066 6e2c   % (objdump, fn,
-00022ca0: 2073 796d 290a 2020 2020 7472 793a 0a20   sym).    try:. 
-00022cb0: 2020 2020 2020 206f 7574 203d 2073 7973         out = sys
-00022cc0: 5f65 7865 635f 6f75 7428 7368 656c 6c5f  _exec_out(shell_
-00022cd0: 636d 642c 2073 6865 6c6c 3d54 7275 6529  cmd, shell=True)
-00022ce0: 0a20 2020 2065 7863 6570 7420 4361 6c6c  .    except Call
-00022cf0: 6564 5072 6f63 6573 7345 7272 6f72 3a20  edProcessError: 
-00022d00: 2023 206e 6f6e 6520 666f 756e 640a 2020   # none found.  
-00022d10: 2020 2020 2020 7265 7475 726e 204e 6f6e        return Non
-00022d20: 650a 2020 2020 6173 7365 7274 2069 7369  e.    assert isi
-00022d30: 6e73 7461 6e63 6528 6f75 742c 2028 7374  nstance(out, (st
-00022d40: 722c 2075 6e69 636f 6465 2929 0a20 2020  r, unicode)).   
-00022d50: 206f 7574 5f6c 6e73 203d 206f 7574 2e73   out_lns = out.s
-00022d60: 706c 6974 6c69 6e65 7328 290a 2020 2020  plitlines().    
-00022d70: 6f75 745f 6c6e 7320 3d20 5b6c 6e20 666f  out_lns = [ln fo
-00022d80: 7220 6c6e 2069 6e20 6f75 745f 6c6e 7320  r ln in out_lns 
-00022d90: 6966 2022 2e74 6578 7422 2069 6e20 6c6e  if ".text" in ln
-00022da0: 5d20 2023 2073 6565 206f 626a 6475 6d70  ]  # see objdump
-00022db0: 0a20 2020 206f 7574 5f6c 6e73 203d 205b  .    out_lns = [
-00022dc0: 6c6e 2066 6f72 206c 6e20 696e 206f 7574  ln for ln in out
-00022dd0: 5f6c 6e73 2069 6620 7379 6d20 696e 206c  _lns if sym in l
-00022de0: 6e2e 7370 6c69 7428 295d 0a20 2020 2069  n.split()].    i
-00022df0: 6620 6e6f 7420 6f75 745f 6c6e 733a 0a20  f not out_lns:. 
-00022e00: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
-00022e10: 6e65 0a20 2020 2072 6574 7572 6e20 2246  ne.    return "F
-00022e20: 6f75 6e64 2025 7220 696e 2025 723a 5c6e  ound %r in %r:\n
-00022e30: 2573 2220 2520 2873 796d 2c20 666e 2c20  %s" % (sym, fn, 
-00022e40: 225c 6e22 2e6a 6f69 6e28 6f75 745f 6c6e  "\n".join(out_ln
-00022e50: 7329 290a 0a0a 6465 6620 6475 6d6d 795f  s))...def dummy_
-00022e60: 6e75 6d70 795f 6765 6d6d 5f63 616c 6c28  numpy_gemm_call(
-00022e70: 293a 0a20 2020 2022 2222 0a20 2020 204a  ):.    """.    J
-00022e80: 7573 7420 7065 7266 6f72 6d73 2073 6f6d  ust performs som
-00022e90: 6520 4745 4d4d 2063 616c 6c20 7669 6120  e GEMM call via 
-00022ea0: 4e75 6d70 792e 0a20 2020 2054 6869 7320  Numpy..    This 
-00022eb0: 6d61 6b65 7320 7375 7265 2074 6861 7420  makes sure that 
-00022ec0: 7468 6520 424c 4153 206c 6962 7261 7279  the BLAS library
-00022ed0: 2069 7320 6c6f 6164 6564 2e0a 2020 2020   is loaded..    
-00022ee0: 2222 220a 2020 2020 696d 706f 7274 206e  """.    import n
-00022ef0: 756d 7079 0a0a 2020 2020 6120 3d20 6e75  umpy..    a = nu
-00022f00: 6d70 792e 7261 6e64 6f6d 2e72 616e 646e  mpy.random.randn
-00022f10: 2835 2c20 3329 2e61 7374 7970 6528 6e75  (5, 3).astype(nu
-00022f20: 6d70 792e 666c 6f61 7433 3229 0a20 2020  mpy.float32).   
-00022f30: 2062 203d 206e 756d 7079 2e72 616e 646f   b = numpy.rando
-00022f40: 6d2e 7261 6e64 6e28 332c 2037 292e 6173  m.randn(3, 7).as
-00022f50: 7479 7065 286e 756d 7079 2e66 6c6f 6174  type(numpy.float
-00022f60: 3332 290a 2020 2020 6320 3d20 6e75 6d70  32).    c = nump
-00022f70: 792e 646f 7428 612c 2062 290a 2020 2020  y.dot(a, b).    
-00022f80: 6173 7365 7274 206e 756d 7079 2e69 7366  assert numpy.isf
-00022f90: 696e 6974 6528 6329 2e61 6c6c 2829 0a0a  inite(c).all()..
-00022fa0: 0a5f 6669 6e64 5f73 6765 6d6d 5f6c 6962  ._find_sgemm_lib
-00022fb0: 5f66 726f 6d5f 7275 6e74 696d 655f 6361  _from_runtime_ca
-00022fc0: 6368 6564 203d 204e 6f6e 650a 0a0a 6465  ched = None...de
-00022fd0: 6620 6669 6e64 5f73 6765 6d6d 5f6c 6962  f find_sgemm_lib
-00022fe0: 735f 6672 6f6d 5f72 756e 7469 6d65 2829  s_from_runtime()
-00022ff0: 3a0a 2020 2020 2222 220a 2020 2020 4c6f  :.    """.    Lo
-00023000: 6f6b 7320 7468 726f 7567 6820 616c 6c20  oks through all 
-00023010: 6c69 6273 2076 6961 203a 6675 6e63 3a60  libs via :func:`
-00023020: 636f 6c6c 6563 745f 7072 6f63 5f6d 6170  collect_proc_map
-00023030: 735f 6578 6563 5f66 696c 6573 602c 0a20  s_exec_files`,. 
-00023040: 2020 2061 6e64 2073 6561 7263 6865 7320     and searches 
-00023050: 666f 7220 616c 6c20 7768 6963 6820 6861  for all which ha
-00023060: 7665 2074 6865 2060 6073 6765 6d6d 6060  ve the ``sgemm``
-00023070: 2073 796d 626f 6c2e 0a20 2020 2043 7572   symbol..    Cur
-00023080: 7265 6e74 6c79 206f 6e6c 7920 776f 726b  rently only work
-00023090: 7320 6f6e 204c 696e 7578 2028 6265 6361  s on Linux (beca
-000230a0: 7573 6520 636f 6c6c 6563 745f 7072 6f63  use collect_proc
-000230b0: 5f6d 6170 735f 6578 6563 5f66 696c 6573  _maps_exec_files
-000230c0: 292e 0a0a 2020 2020 3a72 6574 7572 6e3a  )...    :return:
-000230d0: 206c 6973 7420 6f66 206c 6962 7320 2874   list of libs (t
-000230e0: 6865 6972 2070 6174 6829 0a20 2020 203a  heir path).    :
-000230f0: 7274 7970 653a 206c 6973 745b 7374 725d  rtype: list[str]
-00023100: 0a20 2020 2022 2222 0a20 2020 2069 6620  .    """.    if 
-00023110: 6e6f 7420 6f73 2e70 6174 682e 6578 6973  not os.path.exis
-00023120: 7473 2822 2f70 726f 6322 293a 0a20 2020  ts("/proc"):.   
-00023130: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
-00023140: 0a20 2020 2067 6c6f 6261 6c20 5f66 696e  .    global _fin
-00023150: 645f 7367 656d 6d5f 6c69 625f 6672 6f6d  d_sgemm_lib_from
-00023160: 5f72 756e 7469 6d65 5f63 6163 6865 640a  _runtime_cached.
-00023170: 2020 2020 6966 205f 6669 6e64 5f73 6765      if _find_sge
-00023180: 6d6d 5f6c 6962 5f66 726f 6d5f 7275 6e74  mm_lib_from_runt
-00023190: 696d 655f 6361 6368 6564 2069 7320 6e6f  ime_cached is no
-000231a0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-000231b0: 7265 7475 726e 205f 6669 6e64 5f73 6765  return _find_sge
-000231c0: 6d6d 5f6c 6962 5f66 726f 6d5f 7275 6e74  mm_lib_from_runt
-000231d0: 696d 655f 6361 6368 6564 0a20 2020 2064  ime_cached.    d
-000231e0: 756d 6d79 5f6e 756d 7079 5f67 656d 6d5f  ummy_numpy_gemm_
-000231f0: 6361 6c6c 2829 2020 2320 6d61 6b65 2073  call()  # make s
-00023200: 7572 6520 7468 6174 204e 756d 7079 2069  ure that Numpy i
-00023210: 7320 6c6f 6164 6564 2061 6e64 204e 756d  s loaded and Num
-00023220: 7079 2073 6765 6d6d 2069 7320 6176 6169  py sgemm is avai
-00023230: 6c61 626c 650a 2020 2020 666e 7320 3d20  lable.    fns = 
-00023240: 636f 6c6c 6563 745f 7072 6f63 5f6d 6170  collect_proc_map
-00023250: 735f 6578 6563 5f66 696c 6573 2829 0a20  s_exec_files(). 
-00023260: 2020 2066 6e73 5f77 6974 685f 7367 656d     fns_with_sgem
-00023270: 6d20 3d20 5b5d 0a20 2020 2066 6f72 2066  m = [].    for f
-00023280: 6e20 696e 2066 6e73 3a0a 2020 2020 2020  n in fns:.      
-00023290: 2020 6f75 7420 3d20 6669 6e64 5f73 796d    out = find_sym
-000232a0: 5f69 6e5f 6578 6563 2866 6e2c 2022 7367  _in_exec(fn, "sg
-000232b0: 656d 6d5f 2229 0a20 2020 2020 2020 2069  emm_").        i
-000232c0: 6620 6f75 743a 0a20 2020 2020 2020 2020  f out:.         
-000232d0: 2020 2066 6e73 5f77 6974 685f 7367 656d     fns_with_sgem
-000232e0: 6d2e 6170 7065 6e64 2866 6e29 0a20 2020  m.append(fn).   
-000232f0: 205f 6669 6e64 5f73 6765 6d6d 5f6c 6962   _find_sgemm_lib
-00023300: 5f66 726f 6d5f 7275 6e74 696d 655f 6361  _from_runtime_ca
-00023310: 6368 6564 203d 2066 6e73 5f77 6974 685f  ched = fns_with_
-00023320: 7367 656d 6d0a 2020 2020 7265 7475 726e  sgemm.    return
-00023330: 2066 6e73 5f77 6974 685f 7367 656d 6d0a   fns_with_sgemm.
-00023340: 0a0a 5f66 696e 645f 6c69 6263 7564 6172  .._find_libcudar
-00023350: 745f 6672 6f6d 5f72 756e 7469 6d65 5f63  t_from_runtime_c
-00023360: 6163 6865 6420 3d20 4e6f 6e65 0a0a 0a64  ached = None...d
-00023370: 6566 2066 696e 645f 6c69 6263 7564 6172  ef find_libcudar
-00023380: 745f 6672 6f6d 5f72 756e 7469 6d65 2829  t_from_runtime()
-00023390: 3a0a 2020 2020 2222 220a 2020 2020 4c6f  :.    """.    Lo
-000233a0: 6f6b 7320 7468 726f 7567 6820 616c 6c20  oks through all 
-000233b0: 6c69 6273 2076 6961 203a 6675 6e63 3a60  libs via :func:`
-000233c0: 636f 6c6c 6563 745f 7072 6f63 5f6d 6170  collect_proc_map
-000233d0: 735f 6578 6563 5f66 696c 6573 602c 0a20  s_exec_files`,. 
-000233e0: 2020 2061 6e64 2073 6561 7263 6865 7320     and searches 
-000233f0: 666f 7220 616c 6c20 7768 6963 6820 6861  for all which ha
-00023400: 7665 2074 6865 2060 6073 6765 6d6d 6060  ve the ``sgemm``
-00023410: 2073 796d 626f 6c2e 0a20 2020 2043 7572   symbol..    Cur
-00023420: 7265 6e74 6c79 206f 6e6c 7920 776f 726b  rently only work
-00023430: 7320 6f6e 204c 696e 7578 2028 6265 6361  s on Linux (beca
-00023440: 7573 6520 636f 6c6c 6563 745f 7072 6f63  use collect_proc
-00023450: 5f6d 6170 735f 6578 6563 5f66 696c 6573  _maps_exec_files
-00023460: 292e 0a0a 2020 2020 3a72 6574 7572 6e3a  )...    :return:
-00023470: 206c 6973 7420 6f66 206c 6962 7320 2874   list of libs (t
-00023480: 6865 6972 2070 6174 6829 0a20 2020 203a  heir path).    :
-00023490: 7274 7970 653a 2073 7472 7c4e 6f6e 650a  rtype: str|None.
-000234a0: 2020 2020 2222 220a 2020 2020 6966 206e      """.    if n
-000234b0: 6f74 206f 732e 7061 7468 2e65 7869 7374  ot os.path.exist
-000234c0: 7328 222f 7072 6f63 2229 3a0a 2020 2020  s("/proc"):.    
-000234d0: 2020 2020 7265 7475 726e 204e 6f6e 650a      return None.
-000234e0: 2020 2020 676c 6f62 616c 205f 6669 6e64      global _find
-000234f0: 5f6c 6962 6375 6461 7274 5f66 726f 6d5f  _libcudart_from_
-00023500: 7275 6e74 696d 655f 6361 6368 6564 0a20  runtime_cached. 
-00023510: 2020 2069 6620 5f66 696e 645f 6c69 6263     if _find_libc
-00023520: 7564 6172 745f 6672 6f6d 5f72 756e 7469  udart_from_runti
-00023530: 6d65 5f63 6163 6865 6420 6973 206e 6f74  me_cached is not
-00023540: 204e 6f6e 653a 0a20 2020 2020 2020 2072   None:.        r
-00023550: 6574 7572 6e20 5f66 696e 645f 6c69 6263  eturn _find_libc
-00023560: 7564 6172 745f 6672 6f6d 5f72 756e 7469  udart_from_runti
-00023570: 6d65 5f63 6163 6865 645b 305d 0a20 2020  me_cached[0].   
-00023580: 2066 6e73 203d 2063 6f6c 6c65 6374 5f70   fns = collect_p
-00023590: 726f 635f 6d61 7073 5f65 7865 635f 6669  roc_maps_exec_fi
-000235a0: 6c65 7328 290a 2020 2020 666f 7220 666e  les().    for fn
-000235b0: 2069 6e20 666e 733a 0a20 2020 2020 2020   in fns:.       
-000235c0: 2069 6620 7265 2e6d 6174 6368 2822 2e2a   if re.match(".*
-000235d0: 2f6c 6962 6375 6461 7274 5c5c 2e73 6f28  /libcudart\\.so(
-000235e0: 5c5c 2e2e 2a29 3f22 2c20 666e 293a 0a20  \\..*)?", fn):. 
-000235f0: 2020 2020 2020 2020 2020 205f 6669 6e64             _find
-00023600: 5f6c 6962 6375 6461 7274 5f66 726f 6d5f  _libcudart_from_
-00023610: 7275 6e74 696d 655f 6361 6368 6564 203d  runtime_cached =
-00023620: 205b 666e 5d0a 2020 2020 2020 2020 2020   [fn].          
-00023630: 2020 7265 7475 726e 2066 6e0a 2020 2020    return fn.    
-00023640: 5f66 696e 645f 6c69 6263 7564 6172 745f  _find_libcudart_
-00023650: 6672 6f6d 5f72 756e 7469 6d65 5f63 6163  from_runtime_cac
-00023660: 6865 6420 3d20 5b4e 6f6e 655d 0a20 2020  hed = [None].   
-00023670: 2072 6574 7572 6e20 4e6f 6e65 0a          return None.
+000210b0: 2020 2020 2020 2020 2070 7265 6369 7369           precisi
+000210c0: 6f6e 735b 695d 203d 2030 2e30 0a0a 2020  ons[i] = 0.0..  
+000210d0: 2020 6966 206d 6178 2870 7265 6369 7369    if max(precisi
+000210e0: 6f6e 7329 203e 2030 3a0a 2020 2020 2020  ons) > 0:.      
+000210f0: 2020 705f 6c6f 675f 7375 6d20 3d20 7375    p_log_sum = su
+00021100: 6d28 6d61 7468 2e6c 6f67 2870 2920 666f  m(math.log(p) fo
+00021110: 7220 7020 696e 2070 7265 6369 7369 6f6e  r p in precision
+00021120: 7320 6966 2070 290a 2020 2020 2020 2020  s if p).        
+00021130: 6765 6f5f 6d65 616e 203d 206d 6174 682e  geo_mean = math.
+00021140: 6578 7028 705f 6c6f 675f 7375 6d20 2f20  exp(p_log_sum / 
+00021150: 6d61 785f 6f72 6465 7229 0a0a 2020 2020  max_order)..    
+00021160: 6966 2075 7365 5f62 703a 0a20 2020 2020  if use_bp:.     
+00021170: 2020 2072 6174 696f 203d 2074 7261 6e73     ratio = trans
+00021180: 6c61 7469 6f6e 5f6c 656e 6774 6820 2f20  lation_length / 
+00021190: 7265 6665 7265 6e63 655f 6c65 6e67 7468  reference_length
+000211a0: 0a20 2020 2020 2020 2069 6620 7261 7469  .        if rati
+000211b0: 6f20 3c20 3165 2d33 303a 0a20 2020 2020  o < 1e-30:.     
+000211c0: 2020 2020 2020 2062 7020 3d20 302e 300a         bp = 0.0.
+000211d0: 2020 2020 2020 2020 656c 6966 2072 6174          elif rat
+000211e0: 696f 203c 2031 2e30 3a0a 2020 2020 2020  io < 1.0:.      
+000211f0: 2020 2020 2020 6270 203d 206d 6174 682e        bp = math.
+00021200: 6578 7028 3120 2d20 312e 3020 2f20 7261  exp(1 - 1.0 / ra
+00021210: 7469 6f29 0a20 2020 2020 2020 2065 6c73  tio).        els
+00021220: 653a 0a20 2020 2020 2020 2020 2020 2062  e:.            b
+00021230: 7020 3d20 312e 300a 2020 2020 626c 6575  p = 1.0.    bleu
+00021240: 203d 2067 656f 5f6d 6561 6e20 2a20 6270   = geo_mean * bp
+00021250: 0a20 2020 2072 6574 7572 6e20 6e70 2e66  .    return np.f
+00021260: 6c6f 6174 3332 2862 6c65 7529 0a0a 0a23  loat32(bleu)...#
+00021270: 206e 6f69 6e73 7065 6374 696f 6e20 5079   noinspection Py
+00021280: 5061 636b 6167 6552 6571 7569 7265 6d65  PackageRequireme
+00021290: 6e74 730a 6465 6620 6d6f 6e6b 6579 6669  nts.def monkeyfi
+000212a0: 785f 676c 6962 2829 3a0a 2020 2020 2222  x_glib():.    ""
+000212b0: 220a 2020 2020 4669 7865 7320 736f 6d65  ".    Fixes some
+000212c0: 2073 7475 7069 6420 6275 6773 2073 7563   stupid bugs suc
+000212d0: 6820 7468 6174 2053 4947 494e 5420 6973  h that SIGINT is
+000212e0: 206e 6f74 2077 6f72 6b69 6e67 2e0a 2020   not working..  
+000212f0: 2020 5468 6973 2069 7320 7573 6564 2062    This is used b
+00021300: 7920 6175 6469 6f72 6561 642c 2061 6e64  y audioread, and
+00021310: 2069 6e64 6972 6563 746c 7920 6279 206c   indirectly by l
+00021320: 6962 726f 7361 2066 6f72 206c 6f61 6469  ibrosa for loadi
+00021330: 6e67 2061 7564 696f 2e0a 2020 2020 6874  ng audio..    ht
+00021340: 7470 733a 2f2f 7374 6163 6b6f 7665 7266  tps://stackoverf
+00021350: 6c6f 772e 636f 6d2f 7175 6573 7469 6f6e  low.com/question
+00021360: 732f 3136 3431 3038 3532 2f0a 2020 2020  s/16410852/.    
+00021370: 5365 6520 616c 736f 203a 6675 6e63 3a60  See also :func:`
+00021380: 6d6f 6e6b 6579 7061 7463 685f 6175 6469  monkeypatch_audi
+00021390: 6f72 6561 6460 2e0a 2020 2020 2222 220a  oread`..    """.
+000213a0: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
+000213b0: 2069 6d70 6f72 7420 6769 0a20 2020 2065   import gi.    e
+000213c0: 7863 6570 7420 496d 706f 7274 4572 726f  xcept ImportErro
+000213d0: 723a 0a20 2020 2020 2020 2072 6574 7572  r:.        retur
+000213e0: 6e0a 2020 2020 7472 793a 0a20 2020 2020  n.    try:.     
+000213f0: 2020 2066 726f 6d20 6769 2e72 6570 6f73     from gi.repos
+00021400: 6974 6f72 7920 696d 706f 7274 2047 4c69  itory import GLi
+00021410: 620a 2020 2020 6578 6365 7074 2049 6d70  b.    except Imp
+00021420: 6f72 7445 7272 6f72 3a0a 2020 2020 2020  ortError:.      
+00021430: 2020 2320 6e6f 696e 7370 6563 7469 6f6e    # noinspection
+00021440: 2050 7955 6e72 6573 6f6c 7665 6452 6566   PyUnresolvedRef
+00021450: 6572 656e 6365 730a 2020 2020 2020 2020  erences.        
+00021460: 6672 6f6d 2067 692e 6f76 6572 7269 6465  from gi.override
+00021470: 7320 696d 706f 7274 2047 4c69 620a 2020  s import GLib.  
+00021480: 2020 2320 446f 206e 6f74 6869 6e67 2e0a    # Do nothing..
+00021490: 2020 2020 2320 5468 6520 6f72 6967 696e      # The origin
+000214a0: 616c 2062 6568 6176 696f 7220 776f 756c  al behavior woul
+000214b0: 6420 696e 7374 616c 6c20 6120 5349 4749  d install a SIGI
+000214c0: 4e54 2068 616e 646c 6572 2077 6869 6368  NT handler which
+000214d0: 2063 616c 6c73 2047 4c69 622e 4d61 696e   calls GLib.Main
+000214e0: 4c6f 6f70 2e71 7569 7428 292c 0a20 2020  Loop.quit(),.   
+000214f0: 2023 2061 6e64 2074 6865 6e20 7265 7261   # and then rera
+00021500: 6973 6520 6120 4b65 7962 6f61 7264 496e  ise a KeyboardIn
+00021510: 7465 7272 7570 7420 696e 2074 6861 7420  terrupt in that 
+00021520: 7468 7265 6164 2e0a 2020 2020 2320 486f  thread..    # Ho
+00021530: 7765 7665 722c 2077 6520 7761 6e74 2061  wever, we want a
+00021540: 6e64 2065 7870 6563 7420 746f 2067 6574  nd expect to get
+00021550: 2074 6865 204b 6579 626f 6172 6449 6e74   the KeyboardInt
+00021560: 6572 7275 7074 2069 6e20 7468 6520 6d61  errupt in the ma
+00021570: 696e 2074 6872 6561 642e 0a20 2020 2047  in thread..    G
+00021580: 4c69 622e 4d61 696e 4c6f 6f70 2e5f 5f69  Lib.MainLoop.__i
+00021590: 6e69 745f 5f20 3d20 6c61 6d62 6461 202a  nit__ = lambda *
+000215a0: 6172 6773 2c20 2a2a 6b77 6172 6773 3a20  args, **kwargs: 
+000215b0: 4e6f 6e65 0a0a 0a64 6566 206d 6f6e 6b65  None...def monke
+000215c0: 7970 6174 6368 5f61 7564 696f 7265 6164  ypatch_audioread
+000215d0: 2829 3a0a 2020 2020 2222 220a 2020 2020  ():.    """.    
+000215e0: 6175 6469 6f72 6561 6420 646f 6573 206e  audioread does n
+000215f0: 6f74 2062 6568 6176 6520 6f70 7469 6d61  ot behave optima
+00021600: 6c20 696e 2073 6f6d 6520 6361 7365 732e  l in some cases.
+00021610: 0a20 2020 2045 2e67 2e20 6561 6368 2063  .    E.g. each c
+00021620: 616c 6c20 746f 205f 6361 5f61 7661 696c  all to _ca_avail
+00021630: 6162 6c65 2829 2074 616b 6573 2071 7569  able() takes qui
+00021640: 7465 206c 6f6e 6720 6265 6361 7573 6520  te long because 
+00021650: 6f66 2074 6865 2063 7479 7065 732e 7574  of the ctypes.ut
+00021660: 696c 2e66 696e 645f 6c69 6272 6172 7920  il.find_library 
+00021670: 7573 6167 652e 0a20 2020 2057 6520 7769  usage..    We wi
+00021680: 6c6c 2070 6174 6368 2074 6869 732e 0a0a  ll patch this...
+00021690: 2020 2020 486f 7765 7665 722c 2074 6865      However, the
+000216a0: 2072 6563 6f6d 6d65 6e64 6174 696f 6e20   recommendation 
+000216b0: 776f 756c 6420 6265 2074 6f20 6e6f 7420  would be to not 
+000216c0: 7573 6520 6175 6469 6f72 6561 6420 286c  use audioread (l
+000216d0: 6962 726f 7361 2e6c 6f61 6429 2e0a 2020  ibrosa.load)..  
+000216e0: 2020 6175 6469 6f72 6561 6420 7573 6573    audioread uses
+000216f0: 2047 7374 7265 616d 6572 2061 7320 6120   Gstreamer as a 
+00021700: 6261 636b 656e 6420 6279 2064 6566 6175  backend by defau
+00021710: 6c74 2063 7572 7265 6e74 6c79 2028 6f6e  lt currently (on
+00021720: 204c 696e 7578 292e 0a20 2020 2047 7374   Linux)..    Gst
+00021730: 7265 616d 6572 2068 6173 206d 756c 7469  reamer has multi
+00021740: 706c 6520 6973 7375 6573 2e20 5365 6520  ple issues. See 
+00021750: 616c 736f 203a 6675 6e63 3a60 6d6f 6e6b  also :func:`monk
+00021760: 6579 6669 785f 676c 6962 602c 2061 6e64  eyfix_glib`, and
+00021770: 2068 6572 6520 666f 7220 6469 7363 7573   here for discus
+00021780: 7369 6f6e 3a0a 2020 2020 6874 7470 733a  sion:.    https:
+00021790: 2f2f 6769 7468 7562 2e63 6f6d 2f62 6565  //github.com/bee
+000217a0: 7462 6f78 2f61 7564 696f 7265 6164 2f69  tbox/audioread/i
+000217b0: 7373 7565 732f 3632 0a20 2020 2068 7474  ssues/62.    htt
+000217c0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000217d0: 6265 6574 626f 782f 6175 6469 6f72 6561  beetbox/audiorea
+000217e0: 642f 6973 7375 6573 2f36 330a 0a20 2020  d/issues/63..   
+000217f0: 2049 6e73 7465 6164 2c20 7573 6520 5079   Instead, use Py
+00021800: 536f 756e 6446 696c 652c 2077 6869 6368  SoundFile, which
+00021810: 2069 7320 616c 736f 2066 6173 7465 722e   is also faster.
+00021820: 2053 6565 2068 6572 6520 666f 7220 6469   See here for di
+00021830: 7363 7573 7369 6f6e 733a 0a20 2020 2068  scussions:.    h
+00021840: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00021850: 6d2f 6265 6574 626f 782f 6175 6469 6f72  m/beetbox/audior
+00021860: 6561 642f 6973 7375 6573 2f36 340a 2020  ead/issues/64.  
+00021870: 2020 6874 7470 733a 2f2f 6769 7468 7562    https://github
+00021880: 2e63 6f6d 2f6c 6962 726f 7361 2f6c 6962  .com/librosa/lib
+00021890: 726f 7361 2f69 7373 7565 732f 3638 310a  rosa/issues/681.
+000218a0: 2020 2020 2222 220a 2020 2020 7472 793a      """.    try:
+000218b0: 0a20 2020 2020 2020 2023 206e 6f69 6e73  .        # noins
+000218c0: 7065 6374 696f 6e20 5079 5061 636b 6167  pection PyPackag
+000218d0: 6552 6571 7569 7265 6d65 6e74 730a 2020  eRequirements.  
+000218e0: 2020 2020 2020 696d 706f 7274 2061 7564        import aud
+000218f0: 696f 7265 6164 0a20 2020 2065 7863 6570  ioread.    excep
+00021900: 7420 496d 706f 7274 4572 726f 723a 0a20  t ImportError:. 
+00021910: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
+00021920: 2020 2320 6e6f 696e 7370 6563 7469 6f6e    # noinspection
+00021930: 2050 7950 726f 7465 6374 6564 4d65 6d62   PyProtectedMemb
+00021940: 6572 0a20 2020 2072 6573 203d 2061 7564  er.    res = aud
+00021950: 696f 7265 6164 2e5f 6361 5f61 7661 696c  ioread._ca_avail
+00021960: 6162 6c65 2829 0a20 2020 2061 7564 696f  able().    audio
+00021970: 7265 6164 2e5f 6361 5f61 7661 696c 6162  read._ca_availab
+00021980: 6c65 203d 206c 616d 6264 613a 2072 6573  le = lambda: res
+00021990: 0a0a 0a5f 6366 5f63 6163 6865 203d 207b  ..._cf_cache = {
+000219a0: 7d0a 5f63 665f 6d73 675f 7072 696e 7465  }._cf_msg_printe
+000219b0: 6420 3d20 4661 6c73 650a 0a0a 6465 6620  d = False...def 
+000219c0: 6366 2866 696c 656e 616d 6529 3a0a 2020  cf(filename):.  
+000219d0: 2020 2222 220a 2020 2020 4361 6368 6520    """.    Cache 
+000219e0: 6d61 6e61 6765 722e 2069 3620 7370 6563  manager. i6 spec
+000219f0: 6966 6963 2e0a 0a20 2020 203a 7265 7475  ific...    :retu
+00021a00: 726e 3a20 6669 6c65 6e61 6d65 0a20 2020  rn: filename.   
+00021a10: 203a 7274 7970 653a 2073 7472 0a20 2020   :rtype: str.   
+00021a20: 2022 2222 0a20 2020 2067 6c6f 6261 6c20   """.    global 
+00021a30: 5f63 665f 6d73 675f 7072 696e 7465 640a  _cf_msg_printed.
+00021a40: 2020 2020 696d 706f 7274 206f 730a 2020      import os.  
+00021a50: 2020 6672 6f6d 2073 7562 7072 6f63 6573    from subproces
+00021a60: 7320 696d 706f 7274 2063 6865 636b 5f6f  s import check_o
+00021a70: 7574 7075 740a 0a20 2020 2069 6620 6669  utput..    if fi
+00021a80: 6c65 6e61 6d65 2069 6e20 5f63 665f 6361  lename in _cf_ca
+00021a90: 6368 653a 0a20 2020 2020 2020 2072 6574  che:.        ret
+00021aa0: 7572 6e20 5f63 665f 6361 6368 655b 6669  urn _cf_cache[fi
+00021ab0: 6c65 6e61 6d65 5d0a 2020 2020 6465 6275  lename].    debu
+00021ac0: 675f 6d6f 6465 203d 2069 6e74 286f 732e  g_mode = int(os.
+00021ad0: 656e 7669 726f 6e2e 6765 7428 2244 4542  environ.get("DEB
+00021ae0: 5547 222c 2030 2929 0a20 2020 2069 6620  UG", 0)).    if 
+00021af0: 6465 6275 675f 6d6f 6465 206f 7220 6765  debug_mode or ge
+00021b00: 745f 686f 7374 6e61 6d65 2829 203d 3d20  t_hostname() == 
+00021b10: 2263 6c75 7374 6572 2d63 6e2d 3231 3122  "cluster-cn-211"
+00021b20: 206f 7220 6e6f 7420 6973 5f72 756e 6e69   or not is_runni
+00021b30: 6e67 5f6f 6e5f 636c 7573 7465 7228 293a  ng_on_cluster():
+00021b40: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+00021b50: 5f63 665f 6d73 675f 7072 696e 7465 643a  _cf_msg_printed:
+00021b60: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+00021b70: 6e74 2822 4361 6368 6520 6d61 6e61 6765  nt("Cache manage
+00021b80: 723a 206e 6f74 2075 7365 642c 2075 7365  r: not used, use
+00021b90: 206c 6f63 616c 2066 696c 653a 2025 7320   local file: %s 
+00021ba0: 2864 6973 6361 7264 2066 7572 7468 6572  (discard further
+00021bb0: 206d 6573 7361 6765 7329 2220 2520 6669   messages)" % fi
+00021bc0: 6c65 6e61 6d65 290a 2020 2020 2020 2020  lename).        
+00021bd0: 2020 2020 5f63 665f 6d73 675f 7072 696e      _cf_msg_prin
+00021be0: 7465 6420 3d20 5472 7565 0a20 2020 2020  ted = True.     
+00021bf0: 2020 2072 6574 7572 6e20 6669 6c65 6e61     return filena
+00021c00: 6d65 2020 2320 666f 7220 6465 6275 6767  me  # for debugg
+00021c10: 696e 670a 2020 2020 7472 793a 0a20 2020  ing.    try:.   
+00021c20: 2020 2020 2063 6163 6865 645f 666e 203d       cached_fn =
+00021c30: 2063 6865 636b 5f6f 7574 7075 7428 5b22   check_output(["
+00021c40: 6366 222c 2066 696c 656e 616d 655d 292e  cf", filename]).
+00021c50: 7374 7269 7028 292e 6465 636f 6465 2822  strip().decode("
+00021c60: 7574 6638 2229 0a20 2020 2065 7863 6570  utf8").    excep
+00021c70: 7420 4361 6c6c 6564 5072 6f63 6573 7345  t CalledProcessE
+00021c80: 7272 6f72 3a0a 2020 2020 2020 2020 6966  rror:.        if
+00021c90: 206e 6f74 205f 6366 5f6d 7367 5f70 7269   not _cf_msg_pri
+00021ca0: 6e74 6564 3a0a 2020 2020 2020 2020 2020  nted:.          
+00021cb0: 2020 7072 696e 7428 2243 6163 6865 206d    print("Cache m
+00021cc0: 616e 6167 6572 3a20 4572 726f 7220 6f63  anager: Error oc
+00021cd0: 6375 7272 6564 2c20 7573 696e 6720 6c6f  curred, using lo
+00021ce0: 6361 6c20 6669 6c65 2229 0a20 2020 2020  cal file").     
+00021cf0: 2020 2020 2020 205f 6366 5f6d 7367 5f70         _cf_msg_p
+00021d00: 7269 6e74 6564 203d 2054 7275 650a 2020  rinted = True.  
+00021d10: 2020 2020 2020 7265 7475 726e 2066 696c        return fil
+00021d20: 656e 616d 650a 2020 2020 6173 7365 7274  ename.    assert
+00021d30: 206f 732e 7061 7468 2e65 7869 7374 7328   os.path.exists(
+00021d40: 6361 6368 6564 5f66 6e29 0a20 2020 205f  cached_fn).    _
+00021d50: 6366 5f63 6163 6865 5b66 696c 656e 616d  cf_cache[filenam
+00021d60: 655d 203d 2063 6163 6865 645f 666e 0a20  e] = cached_fn. 
+00021d70: 2020 2072 6574 7572 6e20 6361 6368 6564     return cached
+00021d80: 5f66 6e0a 0a0a 6465 6620 6269 6e61 7279  _fn...def binary
+00021d90: 5f73 6561 7263 685f 616e 7928 636d 702c  _search_any(cmp,
+00021da0: 206c 6f77 2c20 6869 6768 293a 0a20 2020   low, high):.   
+00021db0: 2022 2222 0a20 2020 2042 696e 6172 7920   """.    Binary 
+00021dc0: 7365 6172 6368 2066 6f72 2061 2063 7573  search for a cus
+00021dd0: 746f 6d20 636f 6d70 6172 6520 6675 6e63  tom compare func
+00021de0: 7469 6f6e 2e0a 0a20 2020 203a 7061 7261  tion...    :para
+00021df0: 6d20 2869 6e74 292d 3e69 6e74 2063 6d70  m (int)->int cmp
+00021e00: 3a20 652e 672e 2063 6d70 2869 6478 2920  : e.g. cmp(idx) 
+00021e10: 3d3d 2063 6f6d 7061 7265 2861 7272 6179  == compare(array
+00021e20: 5b69 6478 5d2c 206b 6579 290a 2020 2020  [idx], key).    
+00021e30: 3a70 6172 616d 2069 6e74 206c 6f77 3a20  :param int low: 
+00021e40: 696e 636c 7573 6976 650a 2020 2020 3a70  inclusive.    :p
+00021e50: 6172 616d 2069 6e74 2068 6967 683a 2065  aram int high: e
+00021e60: 7863 6c75 7369 7665 0a20 2020 203a 7274  xclusive.    :rt
+00021e70: 7970 653a 2069 6e74 7c4e 6f6e 650a 2020  ype: int|None.  
+00021e80: 2020 2222 220a 2020 2020 7768 696c 6520    """.    while 
+00021e90: 6c6f 7720 3c20 6869 6768 3a0a 2020 2020  low < high:.    
+00021ea0: 2020 2020 6d69 6420 3d20 286c 6f77 202b      mid = (low +
+00021eb0: 2068 6967 6829 202f 2f20 320a 2020 2020   high) // 2.    
+00021ec0: 2020 2020 7220 3d20 636d 7028 6d69 6429      r = cmp(mid)
+00021ed0: 0a20 2020 2020 2020 2069 6620 7220 3c20  .        if r < 
+00021ee0: 303a 0a20 2020 2020 2020 2020 2020 206c  0:.            l
+00021ef0: 6f77 203d 206d 6964 202b 2031 0a20 2020  ow = mid + 1.   
+00021f00: 2020 2020 2065 6c69 6620 7220 3e20 303a       elif r > 0:
+00021f10: 0a20 2020 2020 2020 2020 2020 2068 6967  .            hig
+00021f20: 6820 3d20 6d69 640a 2020 2020 2020 2020  h = mid.        
+00021f30: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00021f40: 2020 7265 7475 726e 206d 6964 0a20 2020    return mid.   
+00021f50: 2072 6574 7572 6e20 6c6f 770a 0a0a 6465   return low...de
+00021f60: 6620 6765 6e65 7269 635f 696d 706f 7274  f generic_import
+00021f70: 5f6d 6f64 756c 6528 6669 6c65 6e61 6d65  _module(filename
+00021f80: 293a 0a20 2020 2022 2222 0a20 2020 203a  ):.    """.    :
+00021f90: 7061 7261 6d20 7374 7220 6669 6c65 6e61  param str filena
+00021fa0: 6d65 3a0a 2020 2020 2020 5765 2074 7279  me:.      We try
+00021fb0: 2074 6f20 6265 2063 6c65 7665 7220 6162   to be clever ab
+00021fc0: 6f75 7420 6669 6c65 6e61 6d65 2e0a 2020  out filename..  
+00021fd0: 2020 2020 4966 2069 7420 6c6f 6f6b 7320      If it looks 
+00021fe0: 6c69 6b65 2061 206d 6f64 756c 6520 6e61  like a module na
+00021ff0: 6d65 2c20 6a75 7374 2064 6f20 696d 706f  me, just do impo
+00022000: 7274 6c69 622e 696d 706f 7274 5f6d 6f64  rtlib.import_mod
+00022010: 756c 652e 0a20 2020 2020 2049 6620 6974  ule..      If it
+00022020: 206c 6f6f 6b73 206c 696b 6520 6120 6669   looks like a fi
+00022030: 6c65 6e61 6d65 2c20 7365 6172 6368 2066  lename, search f
+00022040: 6f72 2061 2062 6173 6520 7061 7468 2028  or a base path (
+00022050: 7768 6963 6820 646f 6573 206e 6f74 2068  which does not h
+00022060: 6176 6520 5f5f 696e 6974 5f5f 2e70 7929  ave __init__.py)
+00022070: 2c0a 2020 2020 2020 6164 6420 7468 6174  ,.      add that
+00022080: 2070 6174 6820 746f 2073 7973 2e70 6174   path to sys.pat
+00022090: 6820 6966 206e 6565 6465 642c 2061 6e64  h if needed, and
+000220a0: 2069 6d70 6f72 7420 7468 6520 7265 6d61   import the rema
+000220b0: 696e 696e 6720 7768 6572 6520 222f 2220  ining where "/" 
+000220c0: 6973 2072 6570 6c61 6365 6420 6279 2022  is replaced by "
+000220d0: 2e22 0a20 2020 2020 2061 6e64 2074 6865  .".      and the
+000220e0: 2066 696c 6520 6578 7465 6e73 696f 6e20   file extension 
+000220f0: 6973 2072 656d 6f76 6564 2e0a 2020 2020  is removed..    
+00022100: 3a72 6574 7572 6e3a 2074 6865 206d 6f64  :return: the mod
+00022110: 756c 650a 2020 2020 3a72 7479 7065 3a20  ule.    :rtype: 
+00022120: 7479 7065 732e 4d6f 6475 6c65 5479 7065  types.ModuleType
+00022130: 0a20 2020 2022 2222 0a20 2020 2061 7373  .    """.    ass
+00022140: 6572 7420 6669 6c65 6e61 6d65 0a20 2020  ert filename.   
+00022150: 2069 6d70 6f72 7420 696d 706f 7274 6c69   import importli
+00022160: 620a 0a20 2020 2069 6620 222f 2220 6e6f  b..    if "/" no
+00022170: 7420 696e 2066 696c 656e 616d 653a 0a20  t in filename:. 
+00022180: 2020 2020 2020 2072 6574 7572 6e20 696d         return im
+00022190: 706f 7274 6c69 622e 696d 706f 7274 5f6d  portlib.import_m
+000221a0: 6f64 756c 6528 6669 6c65 6e61 6d65 290a  odule(filename).
+000221b0: 2020 2020 7072 6566 6978 5f64 6972 203d      prefix_dir =
+000221c0: 2022 220a 2020 2020 6966 206e 6f74 206f   "".    if not o
+000221d0: 732e 7061 7468 2e65 7869 7374 7328 6669  s.path.exists(fi
+000221e0: 6c65 6e61 6d65 293a 0a20 2020 2020 2020  lename):.       
+000221f0: 2061 7373 6572 7420 6669 6c65 6e61 6d65   assert filename
+00022200: 5b30 5d20 213d 2022 2f22 0a20 2020 2020  [0] != "/".     
+00022210: 2020 2023 204d 6179 6265 2072 656c 6174     # Maybe relat
+00022220: 6976 6520 746f 2052 6574 7572 6e6e 3f0a  ive to Returnn?.
+00022230: 2020 2020 2020 2020 7072 6566 6978 5f64          prefix_d
+00022240: 6972 203d 2022 2573 2f22 2025 2072 6574  ir = "%s/" % ret
+00022250: 7572 6e6e 5f72 6f6f 745f 6469 720a 2020  urnn_root_dir.  
+00022260: 2020 6173 7365 7274 206f 732e 7061 7468    assert os.path
+00022270: 2e65 7869 7374 7328 7072 6566 6978 5f64  .exists(prefix_d
+00022280: 6972 202b 2066 696c 656e 616d 6529 0a20  ir + filename). 
+00022290: 2020 2061 7373 6572 7420 6669 6c65 6e61     assert filena
+000222a0: 6d65 2e65 6e64 7377 6974 6828 222e 7079  me.endswith(".py
+000222b0: 2229 206f 7220 6f73 2e70 6174 682e 6973  ") or os.path.is
+000222c0: 6469 7228 7072 6566 6978 5f64 6972 202b  dir(prefix_dir +
+000222d0: 2066 696c 656e 616d 6529 0a20 2020 2064   filename).    d
+000222e0: 6972 7320 3d20 6669 6c65 6e61 6d65 2e73  irs = filename.s
+000222f0: 706c 6974 2822 2f22 290a 2020 2020 6469  plit("/").    di
+00022300: 7273 2c20 6261 7365 5f66 6e20 3d20 6469  rs, base_fn = di
+00022310: 7273 5b3a 2d31 5d2c 2064 6972 735b 2d31  rs[:-1], dirs[-1
+00022320: 5d0a 2020 2020 6173 7365 7274 206c 656e  ].    assert len
+00022330: 2864 6972 7329 203e 3d20 310a 2020 2020  (dirs) >= 1.    
+00022340: 666f 7220 6920 696e 2072 6576 6572 7365  for i in reverse
+00022350: 6428 7261 6e67 6528 6c65 6e28 6469 7273  d(range(len(dirs
+00022360: 2929 293a 0a20 2020 2020 2020 2064 203d  ))):.        d =
+00022370: 2070 7265 6669 785f 6469 7220 2b20 222f   prefix_dir + "/
+00022380: 222e 6a6f 696e 2864 6972 735b 3a20 6920  ".join(dirs[: i 
+00022390: 2b20 315d 290a 2020 2020 2020 2020 6173  + 1]).        as
+000223a0: 7365 7274 206f 732e 7061 7468 2e69 7364  sert os.path.isd
+000223b0: 6972 2864 290a 2020 2020 2020 2020 6966  ir(d).        if
+000223c0: 206f 732e 7061 7468 2e65 7869 7374 7328   os.path.exists(
+000223d0: 2225 732f 5f5f 696e 6974 5f5f 2e70 7922  "%s/__init__.py"
+000223e0: 2025 2064 293a 0a20 2020 2020 2020 2020   % d):.         
+000223f0: 2020 2063 6f6e 7469 6e75 650a 2020 2020     continue.    
+00022400: 2020 2020 6966 2064 206e 6f74 2069 6e20      if d not in 
+00022410: 7379 732e 7061 7468 3a0a 2020 2020 2020  sys.path:.      
+00022420: 2020 2020 2020 7379 732e 7061 7468 2e61        sys.path.a
+00022430: 7070 656e 6428 6429 0a20 2020 2020 2020  ppend(d).       
+00022440: 206d 203d 2022 2e22 2e6a 6f69 6e28 6469   m = ".".join(di
+00022450: 7273 5b69 202b 2031 203a 5d20 2b20 5b62  rs[i + 1 :] + [b
+00022460: 6173 655f 666e 5d29 0a20 2020 2020 2020  ase_fn]).       
+00022470: 2069 6620 6261 7365 5f66 6e2e 656e 6473   if base_fn.ends
+00022480: 7769 7468 2822 2e70 7922 293a 0a20 2020  with(".py"):.   
+00022490: 2020 2020 2020 2020 206d 203d 206d 5b3a           m = m[:
+000224a0: 2d33 5d0a 2020 2020 2020 2020 7265 7475  -3].        retu
+000224b0: 726e 2069 6d70 6f72 746c 6962 2e69 6d70  rn importlib.imp
+000224c0: 6f72 745f 6d6f 6475 6c65 286d 290a 2020  ort_module(m).  
+000224d0: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
+000224e0: 6f72 2822 6361 6e6e 6f74 2066 6967 7572  or("cannot figur
+000224f0: 6520 6f75 7420 6261 7365 206d 6f64 756c  e out base modul
+00022500: 6520 7061 7468 2066 726f 6d20 2572 2220  e path from %r" 
+00022510: 2520 6669 6c65 6e61 6d65 290a 0a0a 6465  % filename)...de
+00022520: 6620 736f 6674 6d61 7828 782c 2061 7869  f softmax(x, axi
+00022530: 733d 4e6f 6e65 293a 0a20 2020 2022 2222  s=None):.    """
+00022540: 0a20 2020 203a 7061 7261 6d20 6e75 6d70  .    :param nump
+00022550: 792e 6e64 6172 7261 7920 783a 0a20 2020  y.ndarray x:.   
+00022560: 203a 7061 7261 6d20 696e 747c 4e6f 6e65   :param int|None
+00022570: 2061 7869 733a 0a20 2020 203a 7274 7970   axis:.    :rtyp
+00022580: 653a 206e 756d 7079 2e6e 6461 7272 6179  e: numpy.ndarray
+00022590: 0a20 2020 2022 2222 0a20 2020 2069 6d70  .    """.    imp
+000225a0: 6f72 7420 6e75 6d70 790a 0a20 2020 2065  ort numpy..    e
+000225b0: 5f78 203d 206e 756d 7079 2e65 7870 2878  _x = numpy.exp(x
+000225c0: 202d 206e 756d 7079 2e6d 6178 2878 2c20   - numpy.max(x, 
+000225d0: 6178 6973 3d61 7869 732c 206b 6565 7064  axis=axis, keepd
+000225e0: 696d 733d 5472 7565 2929 0a20 2020 2072  ims=True)).    r
+000225f0: 6574 7572 6e20 655f 7820 2f20 6e75 6d70  eturn e_x / nump
+00022600: 792e 7375 6d28 655f 782c 2061 7869 733d  y.sum(e_x, axis=
+00022610: 6178 6973 2c20 6b65 6570 6469 6d73 3d54  axis, keepdims=T
+00022620: 7275 6529 0a0a 0a64 6566 2063 6f6c 6c65  rue)...def colle
+00022630: 6374 5f70 726f 635f 6d61 7073 5f65 7865  ct_proc_maps_exe
+00022640: 635f 6669 6c65 7328 293a 0a20 2020 2022  c_files():.    "
+00022650: 2222 0a20 2020 2043 7572 7265 6e74 6c79  "".    Currently
+00022660: 206f 6e6c 7920 776f 726b 7320 6f6e 204c   only works on L
+00022670: 696e 7578 2e2e 2e0a 0a20 2020 203a 7265  inux.....    :re
+00022680: 7475 726e 3a20 6c69 7374 206f 6620 6d61  turn: list of ma
+00022690: 7070 6564 2065 7865 6375 7461 626c 6573  pped executables
+000226a0: 2028 6c69 6273 290a 2020 2020 3a72 7479   (libs).    :rty
+000226b0: 7065 3a20 6c69 7374 5b73 7472 5d0a 2020  pe: list[str].  
+000226c0: 2020 2222 220a 2020 2020 696d 706f 7274    """.    import
+000226d0: 2072 650a 0a20 2020 2070 6964 203d 206f   re..    pid = o
+000226e0: 732e 6765 7470 6964 2829 0a20 2020 2066  s.getpid().    f
+000226f0: 6e73 203d 205b 5d0a 2020 2020 666f 7220  ns = [].    for 
+00022700: 6c69 6e65 2069 6e20 6f70 656e 2822 2f70  line in open("/p
+00022710: 726f 632f 2569 2f6d 6170 7322 2025 2070  roc/%i/maps" % p
+00022720: 6964 2c20 2272 2229 2e72 6561 6428 292e  id, "r").read().
+00022730: 7370 6c69 746c 696e 6573 2829 3a20 2023  splitlines():  #
+00022740: 2066 6f72 2065 6163 6820 6d61 7070 6564   for each mapped
+00022750: 2072 6567 696f 6e0a 2020 2020 2020 2020   region.        
+00022760: 2320 6874 7470 733a 2f2f 7374 6163 6b6f  # https://stacko
+00022770: 7665 7266 6c6f 772e 636f 6d2f 7175 6573  verflow.com/ques
+00022780: 7469 6f6e 732f 3134 3031 3335 392f 756e  tions/1401359/un
+00022790: 6465 7273 7461 6e64 696e 672d 6c69 6e75  derstanding-linu
+000227a0: 782d 7072 6f63 2d69 642d 6d61 7073 0a20  x-proc-id-maps. 
+000227b0: 2020 2020 2020 2023 2061 6464 7265 7373         # address
+000227c0: 2020 2020 2020 2020 2020 2070 6572 6d73             perms
+000227d0: 206f 6666 7365 7420 2064 6576 2020 2069   offset  dev   i
+000227e0: 6e6f 6465 2020 2070 6174 686e 616d 650a  node   pathname.
+000227f0: 2020 2020 2020 2020 2320 452e 672e 3a0a          # E.g.:.
+00022800: 2020 2020 2020 2020 2320 3766 6632 6465          # 7ff2de
+00022810: 3931 6330 3030 2d37 6666 3264 6539 3165  91c000-7ff2de91e
+00022820: 3030 3020 7277 2d70 2030 3031 3763 3030  000 rw-p 0017c00
+00022830: 3020 3038 3a30 3220 3739 3438 3434 2020  0 08:02 794844  
+00022840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00022850: 2020 202f 7573 722f 6c69 622f 7838 365f     /usr/lib/x86_
+00022860: 3634 2d6c 696e 7578 2d67 6e75 2f6c 6962  64-linux-gnu/lib
+00022870: 7374 6463 2b2e 2e2e 0a20 2020 2020 2020  stdc+....       
+00022880: 206d 203d 2072 652e 6d61 7463 6828 0a20   m = re.match(. 
+00022890: 2020 2020 2020 2020 2020 2072 225e 285b             r"^([
+000228a0: 302d 3941 2d46 612d 665d 2b29 2d28 5b30  0-9A-Fa-f]+)-([0
+000228b0: 2d39 412d 4661 2d66 5d2b 295c 732b 285b  -9A-Fa-f]+)\s+([
+000228c0: 7277 7870 735c 2d5d 2b29 5c73 2b28 5b30  rwxps\-]+)\s+([0
+000228d0: 2d39 412d 4661 2d66 5d2b 295c 732b 285b  -9A-Fa-f]+)\s+([
+000228e0: 302d 3941 2d46 612d 663a 5d2b 295c 732b  0-9A-Fa-f:]+)\s+
+000228f0: 285b 302d 395d 2b29 5c73 2a28 2e2a 2924  ([0-9]+)\s*(.*)$
+00022900: 222c 206c 696e 650a 2020 2020 2020 2020  ", line.        
+00022910: 290a 2020 2020 2020 2020 6173 7365 7274  ).        assert
+00022920: 206d 2c20 226e 6f20 6d61 7463 6820 666f   m, "no match fo
+00022930: 7220 2572 2220 2520 6c69 6e65 0a20 2020  r %r" % line.   
+00022940: 2020 2020 2061 6464 7265 7373 5f73 7461       address_sta
+00022950: 7274 2c20 6164 6472 6573 735f 656e 642c  rt, address_end,
+00022960: 2070 6572 6d73 2c20 6f66 6673 6574 2c20   perms, offset, 
+00022970: 6465 762c 2069 5f6e 6f64 652c 2070 6174  dev, i_node, pat
+00022980: 685f 6e61 6d65 203d 206d 2e67 726f 7570  h_name = m.group
+00022990: 7328 290a 2020 2020 2020 2020 6966 2022  s().        if "
+000229a0: 7822 206e 6f74 2069 6e20 7065 726d 733a  x" not in perms:
+000229b0: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
+000229c0: 7469 6e75 650a 2020 2020 2020 2020 6966  tinue.        if
+000229d0: 206e 6f74 2070 6174 685f 6e61 6d65 206f   not path_name o
+000229e0: 7220 7061 7468 5f6e 616d 652e 7374 6172  r path_name.star
+000229f0: 7473 7769 7468 2822 5b22 2920 6f72 2022  tswith("[") or "
+00022a00: 2864 656c 6574 6564 2922 2069 6e20 7061  (deleted)" in pa
+00022a10: 7468 5f6e 616d 653a 0a20 2020 2020 2020  th_name:.       
+00022a20: 2020 2020 2063 6f6e 7469 6e75 650a 2020       continue.  
+00022a30: 2020 2020 2020 6966 2070 6174 685f 6e61        if path_na
+00022a40: 6d65 206e 6f74 2069 6e20 666e 733a 0a20  me not in fns:. 
+00022a50: 2020 2020 2020 2020 2020 2066 6e73 2e61             fns.a
+00022a60: 7070 656e 6428 7061 7468 5f6e 616d 6529  ppend(path_name)
+00022a70: 0a20 2020 2072 6574 7572 6e20 666e 730a  .    return fns.
+00022a80: 0a0a 6465 6620 6669 6e64 5f73 796d 5f69  ..def find_sym_i
+00022a90: 6e5f 6578 6563 2866 6e2c 2073 796d 293a  n_exec(fn, sym):
+00022aa0: 0a20 2020 2022 2222 0a20 2020 2055 7365  .    """.    Use
+00022ab0: 7320 6060 6f62 6a64 756d 7060 6020 746f  s ``objdump`` to
+00022ac0: 206c 6973 7420 6176 6169 6c61 626c 6520   list available 
+00022ad0: 7379 6d62 6f6c 732c 2061 6e64 2066 696c  symbols, and fil
+00022ae0: 7465 7273 2074 6865 6d20 6279 2074 6865  ters them by the
+00022af0: 2067 6976 656e 2060 6073 796d 6060 2e0a   given ``sym``..
+00022b00: 0a20 2020 203a 7061 7261 6d20 7374 7220  .    :param str 
+00022b10: 666e 3a20 7061 7468 0a20 2020 203a 7061  fn: path.    :pa
+00022b20: 7261 6d20 7374 7220 7379 6d3a 0a20 2020  ram str sym:.   
+00022b30: 203a 7265 7475 726e 3a20 6d61 7463 6865   :return: matche
+00022b40: 6420 6f75 742c 206f 7220 4e6f 6e65 0a20  d out, or None. 
+00022b50: 2020 203a 7274 7970 653a 2073 7472 7c4e     :rtype: str|N
+00022b60: 6f6e 650a 2020 2020 2222 220a 2020 2020  one.    """.    
+00022b70: 6672 6f6d 2073 7562 7072 6f63 6573 7320  from subprocess 
+00022b80: 696d 706f 7274 2043 616c 6c65 6450 726f  import CalledPro
+00022b90: 6365 7373 4572 726f 720a 0a20 2020 206f  cessError..    o
+00022ba0: 626a 6475 6d70 203d 2022 6f62 6a64 756d  bjdump = "objdum
+00022bb0: 7020 2d54 220a 2020 2020 6966 2073 7973  p -T".    if sys
+00022bc0: 2e70 6c61 7466 6f72 6d20 3d3d 2022 6461  .platform == "da
+00022bd0: 7277 696e 223a 0a20 2020 2020 2020 206f  rwin":.        o
+00022be0: 626a 6475 6d70 203d 2022 6f74 6f6f 6c20  bjdump = "otool 
+00022bf0: 2d49 4847 7622 0a20 2020 2073 6865 6c6c  -IHGv".    shell
+00022c00: 5f63 6d64 203d 2022 2573 2025 7320 7c20  _cmd = "%s %s | 
+00022c10: 6772 6570 2025 7322 2025 2028 6f62 6a64  grep %s" % (objd
+00022c20: 756d 702c 2066 6e2c 2073 796d 290a 2020  ump, fn, sym).  
+00022c30: 2020 7472 793a 0a20 2020 2020 2020 206f    try:.        o
+00022c40: 7574 203d 2073 7973 5f65 7865 635f 6f75  ut = sys_exec_ou
+00022c50: 7428 7368 656c 6c5f 636d 642c 2073 6865  t(shell_cmd, she
+00022c60: 6c6c 3d54 7275 6529 0a20 2020 2065 7863  ll=True).    exc
+00022c70: 6570 7420 4361 6c6c 6564 5072 6f63 6573  ept CalledProces
+00022c80: 7345 7272 6f72 3a20 2023 206e 6f6e 6520  sError:  # none 
+00022c90: 666f 756e 640a 2020 2020 2020 2020 7265  found.        re
+00022ca0: 7475 726e 204e 6f6e 650a 2020 2020 6173  turn None.    as
+00022cb0: 7365 7274 2069 7369 6e73 7461 6e63 6528  sert isinstance(
+00022cc0: 6f75 742c 2028 7374 722c 2075 6e69 636f  out, (str, unico
+00022cd0: 6465 2929 0a20 2020 206f 7574 5f6c 6e73  de)).    out_lns
+00022ce0: 203d 206f 7574 2e73 706c 6974 6c69 6e65   = out.splitline
+00022cf0: 7328 290a 2020 2020 6f75 745f 6c6e 7320  s().    out_lns 
+00022d00: 3d20 5b6c 6e20 666f 7220 6c6e 2069 6e20  = [ln for ln in 
+00022d10: 6f75 745f 6c6e 7320 6966 2022 2e74 6578  out_lns if ".tex
+00022d20: 7422 2069 6e20 6c6e 5d20 2023 2073 6565  t" in ln]  # see
+00022d30: 206f 626a 6475 6d70 0a20 2020 206f 7574   objdump.    out
+00022d40: 5f6c 6e73 203d 205b 6c6e 2066 6f72 206c  _lns = [ln for l
+00022d50: 6e20 696e 206f 7574 5f6c 6e73 2069 6620  n in out_lns if 
+00022d60: 7379 6d20 696e 206c 6e2e 7370 6c69 7428  sym in ln.split(
+00022d70: 295d 0a20 2020 2069 6620 6e6f 7420 6f75  )].    if not ou
+00022d80: 745f 6c6e 733a 0a20 2020 2020 2020 2072  t_lns:.        r
+00022d90: 6574 7572 6e20 4e6f 6e65 0a20 2020 2072  eturn None.    r
+00022da0: 6574 7572 6e20 2246 6f75 6e64 2025 7220  eturn "Found %r 
+00022db0: 696e 2025 723a 5c6e 2573 2220 2520 2873  in %r:\n%s" % (s
+00022dc0: 796d 2c20 666e 2c20 225c 6e22 2e6a 6f69  ym, fn, "\n".joi
+00022dd0: 6e28 6f75 745f 6c6e 7329 290a 0a0a 6465  n(out_lns))...de
+00022de0: 6620 6475 6d6d 795f 6e75 6d70 795f 6765  f dummy_numpy_ge
+00022df0: 6d6d 5f63 616c 6c28 293a 0a20 2020 2022  mm_call():.    "
+00022e00: 2222 0a20 2020 204a 7573 7420 7065 7266  "".    Just perf
+00022e10: 6f72 6d73 2073 6f6d 6520 4745 4d4d 2063  orms some GEMM c
+00022e20: 616c 6c20 7669 6120 4e75 6d70 792e 0a20  all via Numpy.. 
+00022e30: 2020 2054 6869 7320 6d61 6b65 7320 7375     This makes su
+00022e40: 7265 2074 6861 7420 7468 6520 424c 4153  re that the BLAS
+00022e50: 206c 6962 7261 7279 2069 7320 6c6f 6164   library is load
+00022e60: 6564 2e0a 2020 2020 2222 220a 2020 2020  ed..    """.    
+00022e70: 696d 706f 7274 206e 756d 7079 0a0a 2020  import numpy..  
+00022e80: 2020 6120 3d20 6e75 6d70 792e 7261 6e64    a = numpy.rand
+00022e90: 6f6d 2e72 616e 646e 2835 2c20 3329 2e61  om.randn(5, 3).a
+00022ea0: 7374 7970 6528 6e75 6d70 792e 666c 6f61  stype(numpy.floa
+00022eb0: 7433 3229 0a20 2020 2062 203d 206e 756d  t32).    b = num
+00022ec0: 7079 2e72 616e 646f 6d2e 7261 6e64 6e28  py.random.randn(
+00022ed0: 332c 2037 292e 6173 7479 7065 286e 756d  3, 7).astype(num
+00022ee0: 7079 2e66 6c6f 6174 3332 290a 2020 2020  py.float32).    
+00022ef0: 6320 3d20 6e75 6d70 792e 646f 7428 612c  c = numpy.dot(a,
+00022f00: 2062 290a 2020 2020 6173 7365 7274 206e   b).    assert n
+00022f10: 756d 7079 2e69 7366 696e 6974 6528 6329  umpy.isfinite(c)
+00022f20: 2e61 6c6c 2829 0a0a 0a5f 6669 6e64 5f73  .all()..._find_s
+00022f30: 6765 6d6d 5f6c 6962 5f66 726f 6d5f 7275  gemm_lib_from_ru
+00022f40: 6e74 696d 655f 6361 6368 6564 203d 204e  ntime_cached = N
+00022f50: 6f6e 650a 0a0a 6465 6620 6669 6e64 5f73  one...def find_s
+00022f60: 6765 6d6d 5f6c 6962 735f 6672 6f6d 5f72  gemm_libs_from_r
+00022f70: 756e 7469 6d65 2829 3a0a 2020 2020 2222  untime():.    ""
+00022f80: 220a 2020 2020 4c6f 6f6b 7320 7468 726f  ".    Looks thro
+00022f90: 7567 6820 616c 6c20 6c69 6273 2076 6961  ugh all libs via
+00022fa0: 203a 6675 6e63 3a60 636f 6c6c 6563 745f   :func:`collect_
+00022fb0: 7072 6f63 5f6d 6170 735f 6578 6563 5f66  proc_maps_exec_f
+00022fc0: 696c 6573 602c 0a20 2020 2061 6e64 2073  iles`,.    and s
+00022fd0: 6561 7263 6865 7320 666f 7220 616c 6c20  earches for all 
+00022fe0: 7768 6963 6820 6861 7665 2074 6865 2060  which have the `
+00022ff0: 6073 6765 6d6d 6060 2073 796d 626f 6c2e  `sgemm`` symbol.
+00023000: 0a20 2020 2043 7572 7265 6e74 6c79 206f  .    Currently o
+00023010: 6e6c 7920 776f 726b 7320 6f6e 204c 696e  nly works on Lin
+00023020: 7578 2028 6265 6361 7573 6520 636f 6c6c  ux (because coll
+00023030: 6563 745f 7072 6f63 5f6d 6170 735f 6578  ect_proc_maps_ex
+00023040: 6563 5f66 696c 6573 292e 0a0a 2020 2020  ec_files)...    
+00023050: 3a72 6574 7572 6e3a 206c 6973 7420 6f66  :return: list of
+00023060: 206c 6962 7320 2874 6865 6972 2070 6174   libs (their pat
+00023070: 6829 0a20 2020 203a 7274 7970 653a 206c  h).    :rtype: l
+00023080: 6973 745b 7374 725d 0a20 2020 2022 2222  ist[str].    """
+00023090: 0a20 2020 2069 6620 6e6f 7420 6f73 2e70  .    if not os.p
+000230a0: 6174 682e 6578 6973 7473 2822 2f70 726f  ath.exists("/pro
+000230b0: 6322 293a 0a20 2020 2020 2020 2072 6574  c"):.        ret
+000230c0: 7572 6e20 4e6f 6e65 0a20 2020 2067 6c6f  urn None.    glo
+000230d0: 6261 6c20 5f66 696e 645f 7367 656d 6d5f  bal _find_sgemm_
+000230e0: 6c69 625f 6672 6f6d 5f72 756e 7469 6d65  lib_from_runtime
+000230f0: 5f63 6163 6865 640a 2020 2020 6966 205f  _cached.    if _
+00023100: 6669 6e64 5f73 6765 6d6d 5f6c 6962 5f66  find_sgemm_lib_f
+00023110: 726f 6d5f 7275 6e74 696d 655f 6361 6368  rom_runtime_cach
+00023120: 6564 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ed is not None:.
+00023130: 2020 2020 2020 2020 7265 7475 726e 205f          return _
+00023140: 6669 6e64 5f73 6765 6d6d 5f6c 6962 5f66  find_sgemm_lib_f
+00023150: 726f 6d5f 7275 6e74 696d 655f 6361 6368  rom_runtime_cach
+00023160: 6564 0a20 2020 2064 756d 6d79 5f6e 756d  ed.    dummy_num
+00023170: 7079 5f67 656d 6d5f 6361 6c6c 2829 2020  py_gemm_call()  
+00023180: 2320 6d61 6b65 2073 7572 6520 7468 6174  # make sure that
+00023190: 204e 756d 7079 2069 7320 6c6f 6164 6564   Numpy is loaded
+000231a0: 2061 6e64 204e 756d 7079 2073 6765 6d6d   and Numpy sgemm
+000231b0: 2069 7320 6176 6169 6c61 626c 650a 2020   is available.  
+000231c0: 2020 666e 7320 3d20 636f 6c6c 6563 745f    fns = collect_
+000231d0: 7072 6f63 5f6d 6170 735f 6578 6563 5f66  proc_maps_exec_f
+000231e0: 696c 6573 2829 0a20 2020 2066 6e73 5f77  iles().    fns_w
+000231f0: 6974 685f 7367 656d 6d20 3d20 5b5d 0a20  ith_sgemm = []. 
+00023200: 2020 2066 6f72 2066 6e20 696e 2066 6e73     for fn in fns
+00023210: 3a0a 2020 2020 2020 2020 6f75 7420 3d20  :.        out = 
+00023220: 6669 6e64 5f73 796d 5f69 6e5f 6578 6563  find_sym_in_exec
+00023230: 2866 6e2c 2022 7367 656d 6d5f 2229 0a20  (fn, "sgemm_"). 
+00023240: 2020 2020 2020 2069 6620 6f75 743a 0a20         if out:. 
+00023250: 2020 2020 2020 2020 2020 2066 6e73 5f77             fns_w
+00023260: 6974 685f 7367 656d 6d2e 6170 7065 6e64  ith_sgemm.append
+00023270: 2866 6e29 0a20 2020 205f 6669 6e64 5f73  (fn).    _find_s
+00023280: 6765 6d6d 5f6c 6962 5f66 726f 6d5f 7275  gemm_lib_from_ru
+00023290: 6e74 696d 655f 6361 6368 6564 203d 2066  ntime_cached = f
+000232a0: 6e73 5f77 6974 685f 7367 656d 6d0a 2020  ns_with_sgemm.  
+000232b0: 2020 7265 7475 726e 2066 6e73 5f77 6974    return fns_wit
+000232c0: 685f 7367 656d 6d0a 0a0a 5f66 696e 645f  h_sgemm..._find_
+000232d0: 6c69 6263 7564 6172 745f 6672 6f6d 5f72  libcudart_from_r
+000232e0: 756e 7469 6d65 5f63 6163 6865 6420 3d20  untime_cached = 
+000232f0: 4e6f 6e65 0a0a 0a64 6566 2066 696e 645f  None...def find_
+00023300: 6c69 6263 7564 6172 745f 6672 6f6d 5f72  libcudart_from_r
+00023310: 756e 7469 6d65 2829 3a0a 2020 2020 2222  untime():.    ""
+00023320: 220a 2020 2020 4c6f 6f6b 7320 7468 726f  ".    Looks thro
+00023330: 7567 6820 616c 6c20 6c69 6273 2076 6961  ugh all libs via
+00023340: 203a 6675 6e63 3a60 636f 6c6c 6563 745f   :func:`collect_
+00023350: 7072 6f63 5f6d 6170 735f 6578 6563 5f66  proc_maps_exec_f
+00023360: 696c 6573 602c 0a20 2020 2061 6e64 2073  iles`,.    and s
+00023370: 6561 7263 6865 7320 666f 7220 616c 6c20  earches for all 
+00023380: 7768 6963 6820 6861 7665 2074 6865 2060  which have the `
+00023390: 6073 6765 6d6d 6060 2073 796d 626f 6c2e  `sgemm`` symbol.
+000233a0: 0a20 2020 2043 7572 7265 6e74 6c79 206f  .    Currently o
+000233b0: 6e6c 7920 776f 726b 7320 6f6e 204c 696e  nly works on Lin
+000233c0: 7578 2028 6265 6361 7573 6520 636f 6c6c  ux (because coll
+000233d0: 6563 745f 7072 6f63 5f6d 6170 735f 6578  ect_proc_maps_ex
+000233e0: 6563 5f66 696c 6573 292e 0a0a 2020 2020  ec_files)...    
+000233f0: 3a72 6574 7572 6e3a 206c 6973 7420 6f66  :return: list of
+00023400: 206c 6962 7320 2874 6865 6972 2070 6174   libs (their pat
+00023410: 6829 0a20 2020 203a 7274 7970 653a 2073  h).    :rtype: s
+00023420: 7472 7c4e 6f6e 650a 2020 2020 2222 220a  tr|None.    """.
+00023430: 2020 2020 6966 206e 6f74 206f 732e 7061      if not os.pa
+00023440: 7468 2e65 7869 7374 7328 222f 7072 6f63  th.exists("/proc
+00023450: 2229 3a0a 2020 2020 2020 2020 7265 7475  "):.        retu
+00023460: 726e 204e 6f6e 650a 2020 2020 676c 6f62  rn None.    glob
+00023470: 616c 205f 6669 6e64 5f6c 6962 6375 6461  al _find_libcuda
+00023480: 7274 5f66 726f 6d5f 7275 6e74 696d 655f  rt_from_runtime_
+00023490: 6361 6368 6564 0a20 2020 2069 6620 5f66  cached.    if _f
+000234a0: 696e 645f 6c69 6263 7564 6172 745f 6672  ind_libcudart_fr
+000234b0: 6f6d 5f72 756e 7469 6d65 5f63 6163 6865  om_runtime_cache
+000234c0: 6420 6973 206e 6f74 204e 6f6e 653a 0a20  d is not None:. 
+000234d0: 2020 2020 2020 2072 6574 7572 6e20 5f66         return _f
+000234e0: 696e 645f 6c69 6263 7564 6172 745f 6672  ind_libcudart_fr
+000234f0: 6f6d 5f72 756e 7469 6d65 5f63 6163 6865  om_runtime_cache
+00023500: 645b 305d 0a20 2020 2066 6e73 203d 2063  d[0].    fns = c
+00023510: 6f6c 6c65 6374 5f70 726f 635f 6d61 7073  ollect_proc_maps
+00023520: 5f65 7865 635f 6669 6c65 7328 290a 2020  _exec_files().  
+00023530: 2020 666f 7220 666e 2069 6e20 666e 733a    for fn in fns:
+00023540: 0a20 2020 2020 2020 2069 6620 7265 2e6d  .        if re.m
+00023550: 6174 6368 2822 2e2a 2f6c 6962 6375 6461  atch(".*/libcuda
+00023560: 7274 5c5c 2e73 6f28 5c5c 2e2e 2a29 3f22  rt\\.so(\\..*)?"
+00023570: 2c20 666e 293a 0a20 2020 2020 2020 2020  , fn):.         
+00023580: 2020 205f 6669 6e64 5f6c 6962 6375 6461     _find_libcuda
+00023590: 7274 5f66 726f 6d5f 7275 6e74 696d 655f  rt_from_runtime_
+000235a0: 6361 6368 6564 203d 205b 666e 5d0a 2020  cached = [fn].  
+000235b0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+000235c0: 2066 6e0a 2020 2020 5f66 696e 645f 6c69   fn.    _find_li
+000235d0: 6263 7564 6172 745f 6672 6f6d 5f72 756e  bcudart_from_run
+000235e0: 7469 6d65 5f63 6163 6865 6420 3d20 5b4e  time_cached = [N
+000235f0: 6f6e 655d 0a20 2020 2072 6574 7572 6e20  one].    return 
+00023600: 4e6f 6e65 0a                             None.
```

### Comparing `returnn-1.20230703.180607/returnn/util/better_exchook.py` & `returnn-1.20230703.193930/returnn/util/better_exchook.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/util/bpe.py` & `returnn-1.20230703.193930/returnn/util/bpe.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/util/debug.py` & `returnn-1.20230703.193930/returnn/util/debug.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/util/debug_helpers.py` & `returnn-1.20230703.193930/returnn/util/debug_helpers.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/util/fsa.py` & `returnn-1.20230703.193930/returnn/util/fsa.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/util/literal_py_to_pickle.py` & `returnn-1.20230703.193930/returnn/util/literal_py_to_pickle.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/util/pprint.py` & `returnn-1.20230703.193930/returnn/util/pprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/util/py-to-pickle.cpp` & `returnn-1.20230703.193930/returnn/util/py-to-pickle.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/util/sig_proc.py` & `returnn-1.20230703.193930/returnn/util/sig_proc.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn/util/task_system.py` & `returnn-1.20230703.193930/returnn/util/task_system.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/returnn.egg-info/PKG-INFO` & `returnn-1.20230703.193930/returnn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: returnn
-Version: 1.20230703.180607
+Version: 1.20230703.193930
 Summary: The RWTH extensible training framework for universal recurrent neural networks
 Home-page: https://github.com/rwth-i6/returnn/
 Author: Albert Zeyer
 Author-email: albzey@gmail.com
 License: RETURNN license
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `returnn-1.20230703.180607/returnn.egg-info/SOURCES.txt` & `returnn-1.20230703.193930/returnn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/setup.py` & `returnn-1.20230703.193930/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tests/DummySprintExec.py` & `returnn-1.20230703.193930/tests/DummySprintExec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tests/PyCharm-inspection-profile.xml` & `returnn-1.20230703.193930/tests/PyCharm-inspection-profile.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tests/PyCharm.idea/codeStyleSettings.xml` & `returnn-1.20230703.193930/tests/PyCharm.idea/codeStyleSettings.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml` & `returnn-1.20230703.193930/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tests/_set_num_threads1.py` & `returnn-1.20230703.193930/tests/_set_num_threads1.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tests/_setup_test_env.py` & `returnn-1.20230703.193930/tests/_setup_test_env.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tests/bpe-unicode-demo.codes` & `returnn-1.20230703.193930/tests/bpe-unicode-demo.codes`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tests/bpe-unicode-demo.vocab` & `returnn-1.20230703.193930/tests/bpe-unicode-demo.vocab`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tests/lexicon_opt.isyms` & `returnn-1.20230703.193930/tests/lexicon_opt.isyms`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tests/lexicon_opt.jpg` & `returnn-1.20230703.193930/tests/lexicon_opt.jpg`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tests/lint_common.py` & `returnn-1.20230703.193930/tests/lint_common.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tests/pycharm-inspect.py` & `returnn-1.20230703.193930/tests/pycharm-inspect.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tests/pylint.py` & `returnn-1.20230703.193930/tests/pylint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tests/returnn-as-framework.py` & `returnn-1.20230703.193930/tests/returnn-as-framework.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tests/rf_utils.py` & `returnn-1.20230703.193930/tests/rf_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tests/spelling.dic` & `returnn-1.20230703.193930/tests/spelling.dic`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tests/test_Config.py` & `returnn-1.20230703.193930/tests/test_Config.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tests/test_Dataset.py` & `returnn-1.20230703.193930/tests/test_Dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tests/test_Fsa.py` & `returnn-1.20230703.193930/tests/test_Fsa.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tests/test_GeneratingDataset.py` & `returnn-1.20230703.193930/tests/test_GeneratingDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tests/test_HDFDataset.py` & `returnn-1.20230703.193930/tests/test_HDFDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tests/test_LearningRateControl.py` & `returnn-1.20230703.193930/tests/test_LearningRateControl.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tests/test_Log.py` & `returnn-1.20230703.193930/tests/test_Log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tests/test_MultiProcDataset.py` & `returnn-1.20230703.193930/tests/test_MultiProcDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tests/test_PTDataset.py` & `returnn-1.20230703.193930/tests/test_PTDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tests/test_Pretrain.py` & `returnn-1.20230703.193930/tests/test_Pretrain.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tests/test_ResNet.py` & `returnn-1.20230703.193930/tests/test_ResNet.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tests/test_SprintDataset.py` & `returnn-1.20230703.193930/tests/test_SprintDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tests/test_SprintInterface.py` & `returnn-1.20230703.193930/tests/test_SprintInterface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tests/test_TFEngine.py` & `returnn-1.20230703.193930/tests/test_TFEngine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tests/test_TFNativeOp.py` & `returnn-1.20230703.193930/tests/test_TFNativeOp.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tests/test_TFNetworkLayer.py` & `returnn-1.20230703.193930/tests/test_TFNetworkLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tests/test_TFNetworkRecLayer.py` & `returnn-1.20230703.193930/tests/test_TFNetworkRecLayer.py`

 * *Files 0% similar despite different names*

```diff
@@ -11451,69 +11451,85 @@
         feed_dict[network.get_epoch_step()] = 0
         session.run((out.placeholder, post_control_deps), feed_dict=feed_dict)
         feed_dict[network.get_epoch_step()] = 1
         session.run((out.placeholder, post_control_deps), feed_dict=feed_dict)
 
 
 def test_self_attention_placeholder_state():
+    n_batch = 3
     num_heads = 2
     total_key_dim = 6
     total_value_dim = 14
-    with make_scope() as session:
-        n_in, n_out = 2, 3
-        config = Config(
-            {
-                "extern_data": {"data": {"dim": n_in}, "classes": {"dim": n_out, "sparse": True}},
-            }
-        )
-        net_dict = {
-            "loop": {
-                "class": "rec",
-                "from": "data",
-                "unit": {
-                    "self_att": {
-                        "class": "self_attention",
-                        "from": "data:source",
-                        "attention_left_only": True,
-                        "num_heads": num_heads,
-                        "total_key_dim": total_key_dim,
-                        "n_out": total_value_dim,
-                        "initial_state": "placeholder",
+    rnd = numpy.random.RandomState(42)
+    prev_time = 2
+    k_init_v = rnd.normal(size=(n_batch, num_heads, prev_time, total_key_dim // num_heads)).astype("float32")
+    v_init_v = rnd.normal(size=(n_batch, num_heads, prev_time, total_value_dim // num_heads)).astype("float32")
+    prev_params_serialized = None
+    prev_out_vs = None
+    for opt in [False, True]:
+        with make_scope() as session:
+            n_in, n_out = 2, 3
+            config = Config(
+                {
+                    "extern_data": {"data": {"dim": n_in}, "classes": {"dim": n_out, "sparse": True}},
+                }
+            )
+            net_dict = {
+                "loop": {
+                    "class": "rec",
+                    "from": "data",
+                    "unit": {
+                        "self_att": {
+                            "class": "self_attention",
+                            "from": "data:source",
+                            "attention_left_only": True,
+                            "num_heads": num_heads,
+                            "total_key_dim": total_key_dim,
+                            "n_out": total_value_dim,
+                            "initial_state": "placeholder",
+                        },
+                        "output": {"class": "copy", "from": "self_att"},
                     },
-                    "output": {"class": "copy", "from": "self_att"},
+                    "optimize_move_layers_out": opt,
                 },
-                "optimize_move_layers_out": False,
-            },
-            "output": {"class": "softmax", "loss": "ce", "target": "classes", "from": "loop", "n_out": n_out},
-        }
-        network = TFNetwork(config=config)
-        network.construct_from_dict(net_dict)
-
-        expected_model_params = {"loop/rec/self_att/QKV", "output/W", "output/b"}
-
-        print("All global variables:")
-        params = tf_compat.v1.global_variables()
-        params = {v.op.name: v for v in params}
-        pprint(params)
-        params.pop("global_step", None)
-        assert set(params.keys()) == expected_model_params
-
-        from test_TFNetworkLayer import make_feed_dict
-
-        network.initialize_params(session)
-        out = network.get_default_output_layer().output
-        n_batch = 3
-        feed_dict = make_feed_dict(network.extern_data, n_batch=n_batch)
-        k_init = session.graph.get_tensor_by_name("loop/rec/self_att/initial_state_placeholder_k_left:0")
-        v_init = session.graph.get_tensor_by_name("loop/rec/self_att/initial_state_placeholder_v_left:0")
-        k_last = session.graph.get_tensor_by_name("loop/rec/self_att/last_state_k_left:0")
-        v_last = session.graph.get_tensor_by_name("loop/rec/self_att/last_state_v_left:0")
-        feed_dict[k_init] = numpy.zeros((n_batch, num_heads, 0, total_key_dim // num_heads), dtype="float32")
-        feed_dict[v_init] = numpy.zeros((n_batch, num_heads, 0, total_value_dim // num_heads), dtype="float32")
-        session.run((out.placeholder, k_last, v_last), feed_dict=feed_dict)
+                "output": {"class": "softmax", "loss": "ce", "target": "classes", "from": "loop", "n_out": n_out},
+            }
+            network = TFNetwork(config=config)
+            network.construct_from_dict(net_dict)
+
+            expected_model_params = {"loop/rec/self_att/QKV", "output/W", "output/b"}
+
+            print("All global variables:")
+            params = tf_compat.v1.global_variables()
+            params = {v.op.name: v for v in params}
+            pprint(params)
+            params.pop("global_step", None)
+            assert set(params.keys()) == expected_model_params
+
+            if prev_params_serialized is None:
+                network.initialize_params(session)
+                prev_params_serialized = network.get_params_serialized(session)
+            else:
+                network.set_params_by_serialized(prev_params_serialized, session)
+
+            from test_TFNetworkLayer import make_feed_dict
+
+            out = network.get_default_output_layer().output
+            feed_dict = make_feed_dict(network.extern_data, n_batch=n_batch)
+            k_init = session.graph.get_tensor_by_name("loop/rec/self_att/initial_state_placeholder_k_left:0")
+            v_init = session.graph.get_tensor_by_name("loop/rec/self_att/initial_state_placeholder_v_left:0")
+            k_last = session.graph.get_tensor_by_name("loop/rec/self_att/last_state_k_left:0")
+            v_last = session.graph.get_tensor_by_name("loop/rec/self_att/last_state_v_left:0")
+            feed_dict[k_init] = k_init_v
+            feed_dict[v_init] = v_init_v
+            out_vs = session.run((out.placeholder, k_last, v_last), feed_dict=feed_dict)
+            if prev_out_vs is not None:
+                for v, prev_v in zip(out_vs, prev_out_vs):
+                    assert_allclose(v, prev_v, atol=1e-5, rtol=1e-5)
+            prev_out_vs = out_vs
 
 
 def test_OptimalCompletionsLayer():
     with make_scope() as session:
         from returnn.tf.layers.base import InternalLayer
         from returnn.tf.util.basic import expand_dims_unbroadcast
```

### Comparing `returnn-1.20230703.180607/tests/test_TFNetworkSigProcLayer.py` & `returnn-1.20230703.193930/tests/test_TFNetworkSigProcLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tests/test_TFUpdater.py` & `returnn-1.20230703.193930/tests/test_TFUpdater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tests/test_TFUtil.py` & `returnn-1.20230703.193930/tests/test_TFUtil.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tests/test_TF_determinism.py` & `returnn-1.20230703.193930/tests/test_TF_determinism.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tests/test_TaskSystem.py` & `returnn-1.20230703.193930/tests/test_TaskSystem.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tests/test_TaskSystem_SharedMem.py` & `returnn-1.20230703.193930/tests/test_TaskSystem_SharedMem.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tests/test_TranslationDataset.py` & `returnn-1.20230703.193930/tests/test_TranslationDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tests/test_Util.py` & `returnn-1.20230703.193930/tests/test_Util.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tests/test_demos.py` & `returnn-1.20230703.193930/tests/test_demos.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tests/test_fork_exec.py` & `returnn-1.20230703.193930/tests/test_fork_exec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tests/test_hdf_dump.py` & `returnn-1.20230703.193930/tests/test_hdf_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tests/test_rf_array.py` & `returnn-1.20230703.193930/tests/test_rf_array.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tests/test_rf_attention.py` & `returnn-1.20230703.193930/tests/test_rf_attention.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tests/test_rf_base.py` & `returnn-1.20230703.193930/tests/test_rf_base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tests/test_rf_cond.py` & `returnn-1.20230703.193930/tests/test_rf_cond.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tests/test_rf_const.py` & `returnn-1.20230703.193930/tests/test_rf_const.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tests/test_rf_container.py` & `returnn-1.20230703.193930/tests/test_rf_container.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tests/test_rf_conv.py` & `returnn-1.20230703.193930/tests/test_rf_conv.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tests/test_rf_encoder_conformer.py` & `returnn-1.20230703.193930/tests/test_rf_encoder_conformer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tests/test_rf_loop.py` & `returnn-1.20230703.193930/tests/test_rf_loop.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tests/test_rf_math.py` & `returnn-1.20230703.193930/tests/test_rf_math.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tests/test_rf_normalization.py` & `returnn-1.20230703.193930/tests/test_rf_normalization.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tests/test_rf_rec.py` & `returnn-1.20230703.193930/tests/test_rf_rec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tests/test_rf_reduce.py` & `returnn-1.20230703.193930/tests/test_rf_reduce.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tests/test_rf_signal.py` & `returnn-1.20230703.193930/tests/test_rf_signal.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tests/test_tensor.py` & `returnn-1.20230703.193930/tests/test_tensor.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tests/test_tools.py` & `returnn-1.20230703.193930/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tests/test_torch_engine.py` & `returnn-1.20230703.193930/tests/test_torch_engine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tests/test_torch_frontend.py` & `returnn-1.20230703.193930/tests/test_torch_frontend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tests/test_torch_internal_frontend.py` & `returnn-1.20230703.193930/tests/test_torch_internal_frontend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tools/analyze-dataset-batches.py` & `returnn-1.20230703.193930/tools/analyze-dataset-batches.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tools/bliss-collect-seq-lens.py` & `returnn-1.20230703.193930/tools/bliss-collect-seq-lens.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tools/bliss-dump-text.py` & `returnn-1.20230703.193930/tools/bliss-dump-text.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tools/bliss-get-segment-names.py` & `returnn-1.20230703.193930/tools/bliss-get-segment-names.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tools/bliss-to-ogg-zip.py` & `returnn-1.20230703.193930/tools/bliss-to-ogg-zip.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tools/bpe-create-lexicon.py` & `returnn-1.20230703.193930/tools/bpe-create-lexicon.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tools/calculate-word-error-rate.py` & `returnn-1.20230703.193930/tools/calculate-word-error-rate.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tools/cleanup-old-models.py` & `returnn-1.20230703.193930/tools/cleanup-old-models.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tools/collect-orth-symbols.py` & `returnn-1.20230703.193930/tools/collect-orth-symbols.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tools/collect-words.py` & `returnn-1.20230703.193930/tools/collect-words.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tools/compile_native_op.py` & `returnn-1.20230703.193930/tools/compile_native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tools/compile_tf_graph.py` & `returnn-1.20230703.193930/tools/compile_tf_graph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tools/debug-dump-search-scores.py` & `returnn-1.20230703.193930/tools/debug-dump-search-scores.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tools/debug-plot-search-scores.py` & `returnn-1.20230703.193930/tools/debug-plot-search-scores.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tools/dump-dataset-raw-strings.py` & `returnn-1.20230703.193930/tools/dump-dataset-raw-strings.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tools/dump-dataset.py` & `returnn-1.20230703.193930/tools/dump-dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tools/dump-forward-stats.py` & `returnn-1.20230703.193930/tools/dump-forward-stats.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tools/dump-forward.py` & `returnn-1.20230703.193930/tools/dump-forward.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tools/dump-network-json.py` & `returnn-1.20230703.193930/tools/dump-network-json.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tools/dump-pickle.py` & `returnn-1.20230703.193930/tools/dump-pickle.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tools/extract_state_tying_from_dataset.py` & `returnn-1.20230703.193930/tools/extract_state_tying_from_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tools/get-attention-weights.py` & `returnn-1.20230703.193930/tools/get-attention-weights.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tools/get-best-model-epoch.py` & `returnn-1.20230703.193930/tools/get-best-model-epoch.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tools/hdf_dump.py` & `returnn-1.20230703.193930/tools/hdf_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tools/hdf_dump_translation_dataset.py` & `returnn-1.20230703.193930/tools/hdf_dump_translation_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tools/import-blocks-mt-model.py` & `returnn-1.20230703.193930/tools/import-blocks-mt-model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tools/import-t2t-mt-model.py` & `returnn-1.20230703.193930/tools/import-t2t-mt-model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tools/lattice_rescorer/Makefile` & `returnn-1.20230703.193930/tools/lattice_rescorer/Makefile`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tools/lattice_rescorer/README.md` & `returnn-1.20230703.193930/tools/lattice_rescorer/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tools/lattice_rescorer/example/README.md` & `returnn-1.20230703.193930/tools/lattice_rescorer/example/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config` & `returnn-1.20230703.193930/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config` & `returnn-1.20230703.193930/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tools/lattice_rescorer/example/rescore_lattice.sh` & `returnn-1.20230703.193930/tools/lattice_rescorer/example/rescore_lattice.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tools/lattice_rescorer/file.h` & `returnn-1.20230703.193930/tools/lattice_rescorer/file.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tools/lattice_rescorer/htklatticerescorer.cc` & `returnn-1.20230703.193930/tools/lattice_rescorer/htklatticerescorer.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tools/lattice_rescorer/htklatticerescorer.h` & `returnn-1.20230703.193930/tools/lattice_rescorer/htklatticerescorer.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tools/lattice_rescorer/main.cc` & `returnn-1.20230703.193930/tools/lattice_rescorer/main.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tools/lattice_rescorer/rescorer.h` & `returnn-1.20230703.193930/tools/lattice_rescorer/rescorer.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tools/lattice_rescorer/vocabulary.cc` & `returnn-1.20230703.193930/tools/lattice_rescorer/vocabulary.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tools/lattice_rescorer/vocabulary.h` & `returnn-1.20230703.193930/tools/lattice_rescorer/vocabulary.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tools/tf_avg_checkpoints.py` & `returnn-1.20230703.193930/tools/tf_avg_checkpoints.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tools/tf_inspect_checkpoint.py` & `returnn-1.20230703.193930/tools/tf_inspect_checkpoint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tools/tf_inspect_summary_log.py` & `returnn-1.20230703.193930/tools/tf_inspect_summary_log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230703.180607/tools/torch_export_to_onnx.py` & `returnn-1.20230703.193930/tools/torch_export_to_onnx.py`

 * *Files identical despite different names*

