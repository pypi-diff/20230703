# Comparing `tmp/tensorqtl-1.0.7.tar.gz` & `tmp/tensorqtl-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorqtl-1.0.7.tar", last modified: Thu Jul  7 03:45:50 2022, max compression
+gzip compressed data, was "tensorqtl-1.0.8.tar", last modified: Mon Jul  3 02:48:16 2023, max compression
```

## Comparing `tensorqtl-1.0.7.tar` & `tensorqtl-1.0.8.tar`

### file list

```diff
@@ -1,32 +1,28 @@
-drwxrwxr-x   0 francois  (1001) francois  (1002)        0 2022-07-07 03:45:50.400670 tensorqtl-1.0.7/
--rw-rw-r--   0 francois  (1001) francois  (1002)     1568 2019-12-01 02:13:14.000000 tensorqtl-1.0.7/LICENSE
--rw-rw-r--   0 francois  (1001) francois  (1002)     9150 2022-07-07 03:45:50.400670 tensorqtl-1.0.7/PKG-INFO
--rw-rw-r--   0 francois  (1001) francois  (1002)     8754 2022-03-18 22:24:08.000000 tensorqtl-1.0.7/README.md
--rw-rw-r--   0 francois  (1001) francois  (1002)       38 2022-07-07 03:45:50.400670 tensorqtl-1.0.7/setup.cfg
--rw-rw-r--   0 francois  (1001) francois  (1002)     1148 2022-05-01 03:15:45.000000 tensorqtl-1.0.7/setup.py
-drwxrwxr-x   0 francois  (1001) francois  (1002)        0 2022-07-07 03:45:50.400670 tensorqtl-1.0.7/tensorqtl/
--rw-rw-r--   0 francois  (1001) francois  (1002)       47 2022-07-07 03:41:07.000000 tensorqtl-1.0.7/tensorqtl/__init__.py
--rw-rw-r--   0 francois  (1001) francois  (1002)       34 2018-11-14 05:39:18.000000 tensorqtl-1.0.7/tensorqtl/__main__.py
--rw-rw-r--   0 francois  (1001) francois  (1002)    49348 2022-03-21 02:00:54.000000 tensorqtl-1.0.7/tensorqtl/cis.py
--rw-rw-r--   0 francois  (1001) francois  (1002)    42646 2021-01-31 03:21:18.000000 tensorqtl-1.0.7/tensorqtl/cis_MAF_filter.py
--rw-rw-r--   0 francois  (1001) francois  (1002)     8525 2022-01-26 06:41:44.000000 tensorqtl-1.0.7/tensorqtl/coloc.py
--rw-rw-r--   0 francois  (1001) francois  (1002)    15391 2022-05-01 00:15:01.000000 tensorqtl-1.0.7/tensorqtl/core.py
--rw-rw-r--   0 francois  (1001) francois  (1002)     7606 2022-03-20 07:25:37.000000 tensorqtl-1.0.7/tensorqtl/eigenmt.py
--rw-rw-r--   0 francois  (1001) francois  (1002)    24290 2022-07-06 23:48:57.000000 tensorqtl-1.0.7/tensorqtl/genotypeio.py
--rw-rw-r--   0 francois  (1001) francois  (1002)     6402 2022-05-01 00:51:59.000000 tensorqtl-1.0.7/tensorqtl/mixqtl.py
--rw-rw-r--   0 francois  (1001) francois  (1002)    35109 2020-04-14 04:03:29.000000 tensorqtl-1.0.7/tensorqtl/mixqtl_bak.py
--rw-rw-r--   0 francois  (1001) francois  (1002)    37629 2020-05-23 21:15:29.000000 tensorqtl-1.0.7/tensorqtl/mixqtl_perm.py
--rw-rw-r--   0 francois  (1001) francois  (1002)    23721 2022-01-23 01:54:27.000000 tensorqtl-1.0.7/tensorqtl/mixqtl_protoype.py
--rw-rw-r--   0 francois  (1001) francois  (1002)     4962 2022-07-06 23:25:17.000000 tensorqtl-1.0.7/tensorqtl/pgen.py
--rw-rw-r--   0 francois  (1001) francois  (1002)    18245 2022-07-07 00:45:45.000000 tensorqtl-1.0.7/tensorqtl/post.py
--rw-rw-r--   0 francois  (1001) francois  (1002)     1974 2022-07-07 00:44:56.000000 tensorqtl-1.0.7/tensorqtl/rfunc.py
--rw-rw-r--   0 francois  (1001) francois  (1002)    25316 2021-07-20 02:49:26.000000 tensorqtl-1.0.7/tensorqtl/susie.py
--rwxrwxr-x   0 francois  (1001) francois  (1002)    12871 2022-07-07 00:33:03.000000 tensorqtl-1.0.7/tensorqtl/tensorqtl.py
--rw-rw-r--   0 francois  (1001) francois  (1002)    21644 2022-01-18 00:41:42.000000 tensorqtl-1.0.7/tensorqtl/trans.py
-drwxrwxr-x   0 francois  (1001) francois  (1002)        0 2022-07-07 03:45:50.400670 tensorqtl-1.0.7/tensorqtl.egg-info/
--rw-rw-r--   0 francois  (1001) francois  (1002)     9150 2022-07-07 03:45:49.000000 tensorqtl-1.0.7/tensorqtl.egg-info/PKG-INFO
--rw-rw-r--   0 francois  (1001) francois  (1002)      611 2022-07-07 03:45:50.000000 tensorqtl-1.0.7/tensorqtl.egg-info/SOURCES.txt
--rw-rw-r--   0 francois  (1001) francois  (1002)        1 2022-07-07 03:45:49.000000 tensorqtl-1.0.7/tensorqtl.egg-info/dependency_links.txt
--rw-rw-r--   0 francois  (1001) francois  (1002)       49 2022-07-07 03:45:50.000000 tensorqtl-1.0.7/tensorqtl.egg-info/entry_points.txt
--rw-rw-r--   0 francois  (1001) francois  (1002)       50 2022-07-07 03:45:50.000000 tensorqtl-1.0.7/tensorqtl.egg-info/requires.txt
--rw-rw-r--   0 francois  (1001) francois  (1002)       10 2022-07-07 03:45:50.000000 tensorqtl-1.0.7/tensorqtl.egg-info/top_level.txt
+drwxrwxr-x   0 francois  (1001) francois  (1002)        0 2023-07-03 02:48:16.060299 tensorqtl-1.0.8/
+-rw-rw-r--   0 francois  (1001) francois  (1002)     1568 2019-12-01 02:13:14.000000 tensorqtl-1.0.8/LICENSE
+-rw-rw-r--   0 francois  (1001) francois  (1002)     9442 2023-07-03 02:48:16.060299 tensorqtl-1.0.8/PKG-INFO
+-rw-rw-r--   0 francois  (1001) francois  (1002)     9046 2022-11-01 06:43:49.000000 tensorqtl-1.0.8/README.md
+-rw-rw-r--   0 francois  (1001) francois  (1002)       38 2023-07-03 02:48:16.060299 tensorqtl-1.0.8/setup.cfg
+-rw-rw-r--   0 francois  (1001) francois  (1002)     1175 2023-07-02 07:31:12.000000 tensorqtl-1.0.8/setup.py
+drwxrwxr-x   0 francois  (1001) francois  (1002)        0 2023-07-03 02:48:16.056299 tensorqtl-1.0.8/tensorqtl/
+-rw-rw-r--   0 francois  (1001) francois  (1002)       47 2023-05-25 08:21:56.000000 tensorqtl-1.0.8/tensorqtl/__init__.py
+-rw-rw-r--   0 francois  (1001) francois  (1002)       34 2018-11-14 05:39:18.000000 tensorqtl-1.0.8/tensorqtl/__main__.py
+-rw-rw-r--   0 francois  (1001) francois  (1002)    55492 2023-07-02 17:54:50.000000 tensorqtl-1.0.8/tensorqtl/cis.py
+-rw-rw-r--   0 francois  (1001) francois  (1002)     8501 2023-06-25 01:46:31.000000 tensorqtl-1.0.8/tensorqtl/coloc.py
+-rw-rw-r--   0 francois  (1001) francois  (1002)    15579 2023-05-25 06:48:46.000000 tensorqtl-1.0.8/tensorqtl/core.py
+-rw-rw-r--   0 francois  (1001) francois  (1002)     7626 2023-05-25 08:28:29.000000 tensorqtl-1.0.8/tensorqtl/eigenmt.py
+-rw-rw-r--   0 francois  (1001) francois  (1002)    24364 2023-07-02 07:26:36.000000 tensorqtl-1.0.8/tensorqtl/genotypeio.py
+-rw-rw-r--   0 francois  (1001) francois  (1002)     2552 2023-07-03 02:40:35.000000 tensorqtl-1.0.8/tensorqtl/mixqtl.py
+-rw-rw-r--   0 francois  (1001) francois  (1002)    20083 2023-07-02 19:56:02.000000 tensorqtl-1.0.8/tensorqtl/pgen.py
+-rw-rw-r--   0 francois  (1001) francois  (1002)    16520 2023-07-03 01:08:40.000000 tensorqtl-1.0.8/tensorqtl/post.py
+-rw-rw-r--   0 francois  (1001) francois  (1002)     1978 2023-02-26 01:09:48.000000 tensorqtl-1.0.8/tensorqtl/rfunc.py
+-rw-rw-r--   0 francois  (1001) francois  (1002)    26512 2022-12-07 16:17:46.000000 tensorqtl-1.0.8/tensorqtl/susie.py
+-rwxrwxr-x   0 francois  (1001) francois  (1002)    19714 2023-07-02 23:22:32.000000 tensorqtl-1.0.8/tensorqtl/tensorqtl.py
+-rw-rw-r--   0 francois  (1001) francois  (1002)    22017 2023-05-29 00:32:15.000000 tensorqtl-1.0.8/tensorqtl/trans.py
+drwxrwxr-x   0 francois  (1001) francois  (1002)        0 2023-07-03 02:48:16.060299 tensorqtl-1.0.8/tensorqtl.egg-info/
+-rw-rw-r--   0 francois  (1001) francois  (1002)     9442 2023-07-03 02:48:16.000000 tensorqtl-1.0.8/tensorqtl.egg-info/PKG-INFO
+-rw-rw-r--   0 francois  (1001) francois  (1002)      505 2023-07-03 02:48:16.000000 tensorqtl-1.0.8/tensorqtl.egg-info/SOURCES.txt
+-rw-rw-r--   0 francois  (1001) francois  (1002)        1 2023-07-03 02:48:16.000000 tensorqtl-1.0.8/tensorqtl.egg-info/dependency_links.txt
+-rw-rw-r--   0 francois  (1001) francois  (1002)       49 2023-07-03 02:48:16.000000 tensorqtl-1.0.8/tensorqtl.egg-info/entry_points.txt
+-rw-rw-r--   0 francois  (1001) francois  (1002)       66 2023-07-03 02:48:16.000000 tensorqtl-1.0.8/tensorqtl.egg-info/requires.txt
+-rw-rw-r--   0 francois  (1001) francois  (1002)       10 2023-07-03 02:48:16.000000 tensorqtl-1.0.8/tensorqtl.egg-info/top_level.txt
```

### Comparing `tensorqtl-1.0.7/LICENSE` & `tensorqtl-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorqtl-1.0.7/PKG-INFO` & `tensorqtl-1.0.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: tensorqtl
-Version: 1.0.7
+Version: 1.0.8
 Summary: GPU-accelerated QTL mapper
 Author: Francois Aguet (Broad Institute)
 Author-email: francois@broadinstitute.org
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## tensorQTL
 
 tensorQTL is a GPU-enabled QTL mapper, achieving ~200-300 fold faster *cis*- and *trans*-QTL mapping compared to CPU-based implementations.
 
 If you use tensorQTL in your research, please cite the following paper:
-[Taylor-Weiner, Aguet, et al., *Genome Biol.* 20:228, 2019](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-019-1836-7).
+[Taylor-Weiner, Aguet, et al., *Genome Biol.*, 2019](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-019-1836-7).
 
-Empirical beta-approximated p-values are computed as described in [FastQTL](http://fastqtl.sourceforge.net/) ([Ongen et al., 2016](https://academic.oup.com/bioinformatics/article/32/10/1479/1742545)).
+Empirical beta-approximated p-values are computed as described in [Ongen et al., *Bioinformatics*, 2016](https://academic.oup.com/bioinformatics/article/32/10/1479/1742545).
 
 ### Install
 You can install tensorQTL using pip:
 ```
 pip3 install tensorqtl
 ```
 or directly from this repository:
@@ -29,14 +29,21 @@
 $ git clone git@github.com:broadinstitute/tensorqtl.git
 $ cd tensorqtl
 # set up virtual environment and install
 $ virtualenv venv
 $ source venv/bin/activate
 (venv)$ pip install -r install/requirements.txt .
 ```
+To use PLINK 2 binary files ([pgen/pvar/psam](https://www.cog-genomics.org/plink/2.0/input#pgen)), [pgenlib](https://github.com/chrchang/plink-ng/tree/master/2.0/Python) must be installed:
+```
+git clone git@github.com:chrchang/plink-ng.git
+cd plink-ng/2.0/Python/
+python3 setup.py build_ext
+python3 setup.py install
+```
 
 ### Requirements
 
 tensorQTL requires an environment configured with a GPU for optimal performance, but can also be run on a CPU. Instructions for setting up a virtual machine on Google Cloud Platform are provided [here](install/INSTALL.md).
 
 ### Input formats
 Three inputs are required for QTL analyses with tensorQTL: genotypes, phenotypes, and covariates. 
@@ -50,15 +57,15 @@
       --out ${plink_prefix_path}
   ```
   If using PLINK 1.9 or earlier, add the `--keep-allele-order` flag. 
   
   Alternatively, the genotypes can be provided as a dataframe (genotypes x samples). 
 
 
-The [examples notebook](example/tensorqtl_examples.ipynb) below contains examples of all input files. The input formats for phenotypes and covariates are identical to those used by [FastQTL](http://fastqtl.sourceforge.net/).
+The [examples notebook](example/tensorqtl_examples.ipynb) below contains examples of all input files. The input formats for phenotypes and covariates are identical to those used by [FastQTL](https://github.com/francois-a/fastqtl).
 
 ### Examples
 For examples illustrating *cis*- and *trans*-QTL mapping, please see [tensorqtl_examples.ipynb](example/tensorqtl_examples.ipynb).
 
 ### Running tensorQTL
 This section describes how to run the different modes of tensorQTL, both from the command line and within Python.
 For a full list of options, run
```

### Comparing `tensorqtl-1.0.7/README.md` & `tensorqtl-1.0.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ## tensorQTL
 
 tensorQTL is a GPU-enabled QTL mapper, achieving ~200-300 fold faster *cis*- and *trans*-QTL mapping compared to CPU-based implementations.
 
 If you use tensorQTL in your research, please cite the following paper:
-[Taylor-Weiner, Aguet, et al., *Genome Biol.* 20:228, 2019](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-019-1836-7).
+[Taylor-Weiner, Aguet, et al., *Genome Biol.*, 2019](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-019-1836-7).
 
-Empirical beta-approximated p-values are computed as described in [FastQTL](http://fastqtl.sourceforge.net/) ([Ongen et al., 2016](https://academic.oup.com/bioinformatics/article/32/10/1479/1742545)).
+Empirical beta-approximated p-values are computed as described in [Ongen et al., *Bioinformatics*, 2016](https://academic.oup.com/bioinformatics/article/32/10/1479/1742545).
 
 ### Install
 You can install tensorQTL using pip:
 ```
 pip3 install tensorqtl
 ```
 or directly from this repository:
@@ -17,14 +17,21 @@
 $ git clone git@github.com:broadinstitute/tensorqtl.git
 $ cd tensorqtl
 # set up virtual environment and install
 $ virtualenv venv
 $ source venv/bin/activate
 (venv)$ pip install -r install/requirements.txt .
 ```
+To use PLINK 2 binary files ([pgen/pvar/psam](https://www.cog-genomics.org/plink/2.0/input#pgen)), [pgenlib](https://github.com/chrchang/plink-ng/tree/master/2.0/Python) must be installed:
+```
+git clone git@github.com:chrchang/plink-ng.git
+cd plink-ng/2.0/Python/
+python3 setup.py build_ext
+python3 setup.py install
+```
 
 ### Requirements
 
 tensorQTL requires an environment configured with a GPU for optimal performance, but can also be run on a CPU. Instructions for setting up a virtual machine on Google Cloud Platform are provided [here](install/INSTALL.md).
 
 ### Input formats
 Three inputs are required for QTL analyses with tensorQTL: genotypes, phenotypes, and covariates. 
@@ -38,15 +45,15 @@
       --out ${plink_prefix_path}
   ```
   If using PLINK 1.9 or earlier, add the `--keep-allele-order` flag. 
   
   Alternatively, the genotypes can be provided as a dataframe (genotypes x samples). 
 
 
-The [examples notebook](example/tensorqtl_examples.ipynb) below contains examples of all input files. The input formats for phenotypes and covariates are identical to those used by [FastQTL](http://fastqtl.sourceforge.net/).
+The [examples notebook](example/tensorqtl_examples.ipynb) below contains examples of all input files. The input formats for phenotypes and covariates are identical to those used by [FastQTL](https://github.com/francois-a/fastqtl).
 
 ### Examples
 For examples illustrating *cis*- and *trans*-QTL mapping, please see [tensorqtl_examples.ipynb](example/tensorqtl_examples.ipynb).
 
 ### Running tensorQTL
 This section describes how to run the different modes of tensorQTL, both from the command line and within Python.
 For a full list of options, run
```

### Comparing `tensorqtl-1.0.7/setup.py` & `tensorqtl-1.0.8/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -23,19 +23,20 @@
         'console_scripts': [
             'tensorqtl = tensorqtl:__main__'
         ]
     },
     install_requires = [
         'numpy',
         'pandas',
+        'pandas-plink',
+        'Pgenlib>=0.90.1',
         'pyarrow',
+        'qtl',
         'scipy',
-        'pandas-plink',
         'torch',
-        'qtl',
     ],
     classifiers = [
         "Programming Language :: Python :: 3",
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering :: Bio-Informatics",
     ],
 )
```

### Comparing `tensorqtl-1.0.7/tensorqtl/cis.py` & `tensorqtl-1.0.8/tensorqtl/cis.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,19 +7,14 @@
 import time
 from collections import OrderedDict
 
 sys.path.insert(1, os.path.dirname(__file__))
 import genotypeio, eigenmt
 from core import *
 
-import imp
-import core
-imp.reload(core)
-from core import *
-imp.reload(eigenmt)
 
 def calculate_cis_nominal(genotypes_t, phenotype_t, residualizer=None, return_af=True):
     """
     Calculate nominal associations
 
     genotypes_t: genotypes x samples
     phenotype_t: single phenotype
@@ -131,15 +126,15 @@
         }, index=genotype_df.index[mask])
     if df.index.str.startswith('chr').all():  # assume chr_pos_ref_alt_build format
         df['position'] = df.index.map(lambda x: int(x.split('_')[1]))
     return df
 
 
 def map_nominal(genotype_df, variant_df, phenotype_df, phenotype_pos_df, prefix,
-                covariates_df=None, maf_threshold=0, interaction_df=None, maf_threshold_interaction=0.05,
+                covariates_df=None, paired_covariate_df=None, maf_threshold=0, interaction_df=None, maf_threshold_interaction=0.05,
                 group_s=None, window=1000000, run_eigenmt=False,
                 output_dir='.', write_top=True, write_stats=True, logger=None, verbose=True):
     """
     cis-QTL mapping: nominal associations for all variant-phenotype pairs
 
     Association results for each chromosome are written to parquet files
     in the format <output_dir>/<prefix>.cis_qtl_pairs.<chr>.parquet
@@ -155,49 +150,58 @@
     if group_s is not None:
         group_dict = group_s.to_dict()
 
     logger.write('cis-QTL mapping: nominal associations for all variant-phenotype pairs')
     logger.write(f'  * {phenotype_df.shape[1]} samples')
     logger.write(f'  * {phenotype_df.shape[0]} phenotypes')
     if covariates_df is not None:
-        assert np.all(phenotype_df.columns==covariates_df.index)
+        assert np.all(phenotype_df.columns == covariates_df.index)
         logger.write(f'  * {covariates_df.shape[1]} covariates')
         residualizer = Residualizer(torch.tensor(covariates_df.values, dtype=torch.float32).to(device))
         dof = phenotype_df.shape[1] - 2 - covariates_df.shape[1]
     else:
         residualizer = None
         dof = phenotype_df.shape[1] - 2
+    if paired_covariate_df is not None:
+        assert covariates_df is not None
+        assert paired_covariate_df.index.isin(phenotype_df.index).all(), f"Paired covariate phenotypes must be present in phenotype matrix."
+        assert paired_covariate_df.columns.equals(phenotype_df.columns), f"Paired covariate samples must match samples in phenotype matrix."
+        paired_covariate_df = paired_covariate_df.T  # samples x phenotypes
+        logger.write(f'  * including phenotype-specific covariate')
     logger.write(f'  * {variant_df.shape[0]} variants')
     if interaction_df is not None:
         assert interaction_df.index.equals(phenotype_df.columns)
         logger.write(f"  * including {interaction_df.shape[1]} interaction term(s)")
         if maf_threshold_interaction > 0:
             logger.write(f'    * using {maf_threshold_interaction:.2f} MAF threshold')
     elif maf_threshold > 0:
         logger.write(f'  * applying in-sample {maf_threshold} MAF filter')
+    logger.write(f'  * cis-window: ±{window:,}')
 
     genotype_ix = np.array([genotype_df.columns.tolist().index(i) for i in phenotype_df.columns])
     genotype_ix_t = torch.from_numpy(genotype_ix).to(device)
     if interaction_df is not None:
         ni = interaction_df.shape[1]
         dof -= 2 * ni
         interaction_t = torch.tensor(interaction_df.values, dtype=torch.float32).to(device)
         if maf_threshold_interaction > 0 and ni == 1:
             mask_s = pd.Series(True, index=interaction_df.index)
             mask_s[interaction_df[interaction_df.columns[0]].sort_values(kind='mergesort').index[:interaction_df.shape[0]//2]] = False
             interaction_mask_t = torch.BoolTensor(mask_s).to(device)
         else:
             # TODO: implement filtering for multiple interactions?
             interaction_mask_t = None
+        col_order = ['phenotype_id', 'variant_id', 'start_distance']
+        if 'pos' not in phenotype_pos_df:
+            col_order += ['end_distance']
+        col_order += ['af', 'ma_samples', 'ma_count', 'pval_g', 'b_g', 'b_g_se']
         if ni == 1:
-            col_order = ['phenotype_id', 'variant_id', 'tss_distance', 'af', 'ma_samples', 'ma_count', 'pval_g', 'b_g', 'b_g_se',
-                         'pval_i', 'b_i', 'b_i_se', 'pval_gi', 'b_gi', 'b_gi_se']
+            col_order += ['pval_i', 'b_i', 'b_i_se', 'pval_gi', 'b_gi', 'b_gi_se']
         else:
-            col_order = (['phenotype_id', 'variant_id', 'tss_distance', 'af', 'ma_samples', 'ma_count', 'pval_g', 'b_g', 'b_g_se'] +
-                         [k.replace('i', f"i{i+1}") for i in range(0,ni) for k in ['pval_i', 'b_i', 'b_i_se', 'pval_gi', 'b_gi', 'b_gi_se']])
+            col_order += [k.replace('i', f"i{i+1}") for i in range(0,ni) for k in ['pval_i', 'b_i', 'b_i_se', 'pval_gi', 'b_gi', 'b_gi_se']]
 
         # use column names instead of numbered interaction variables in output files
         var_dict = []
         for i,v in enumerate(interaction_df.columns, 1):
             for c in ['pval_i', 'b_i', 'b_i_se']:
                 var_dict.append((c.replace('_i', f'_i{i}'), c.replace('_i', f'_{v}')))
             for c in ['pval_gi', 'b_gi', 'b_gi_se']:
@@ -222,15 +226,17 @@
             for i in igc.group_s[igc.phenotype_pos_df['chr'] == chrom].drop_duplicates().index:
                 j = igc.cis_ranges[i]
                 n += j[1] - j[0] + 1
 
         chr_res = OrderedDict()
         chr_res['phenotype_id'] = []
         chr_res['variant_id'] = []
-        chr_res['tss_distance'] = np.empty(n, dtype=np.int32)
+        chr_res['start_distance'] = np.empty(n, dtype=np.int32)
+        if 'pos' not in phenotype_pos_df:
+            chr_res['end_distance'] = np.empty(n, dtype=np.int32)
         chr_res['af'] =           np.empty(n, dtype=np.float32)
         chr_res['ma_samples'] =   np.empty(n, dtype=np.int32)
         chr_res['ma_count'] =     np.empty(n, dtype=np.int32)
         if interaction_df is None:
             chr_res['pval_nominal'] = np.empty(n, dtype=np.float64)
             chr_res['slope'] =        np.empty(n, dtype=np.float32)
             chr_res['slope_se'] =     np.empty(n, dtype=np.float32)
@@ -251,59 +257,76 @@
                 # copy genotypes to GPU
                 phenotype_t = torch.tensor(phenotype, dtype=torch.float).to(device)
                 genotypes_t = torch.tensor(genotypes, dtype=torch.float).to(device)
                 genotypes_t = genotypes_t[:,genotype_ix_t]
                 impute_mean(genotypes_t)
 
                 variant_ids = variant_df.index[genotype_range[0]:genotype_range[-1]+1]
-                tss_distance = np.int32(variant_df['pos'].values[genotype_range[0]:genotype_range[-1]+1] - igc.phenotype_tss[phenotype_id])
+                start_distance = np.int32(variant_df['pos'].values[genotype_range[0]:genotype_range[-1]+1] - igc.phenotype_start[phenotype_id])
+                if 'pos' not in phenotype_pos_df:
+                    end_distance = np.int32(variant_df['pos'].values[genotype_range[0]:genotype_range[-1]+1] - igc.phenotype_end[phenotype_id])
 
                 if maf_threshold > 0:
                     maf_t = calculate_maf(genotypes_t)
                     mask_t = maf_t >= maf_threshold
                     genotypes_t = genotypes_t[mask_t]
                     mask = mask_t.cpu().numpy().astype(bool)
                     variant_ids = variant_ids[mask]
-                    tss_distance = tss_distance[mask]
+                    start_distance = start_distance[mask]
+                    if 'pos' not in phenotype_pos_df:
+                        end_distance = end_distance[mask]
+
+                if paired_covariate_df is None or phenotype_id not in paired_covariate_df:
+                    iresidualizer = residualizer
+                else:
+                    iresidualizer = Residualizer(torch.tensor(np.c_[covariates_df, paired_covariate_df[phenotype_id]],
+                                                              dtype=torch.float32).to(device))
 
                 if interaction_df is None:
-                    res = calculate_cis_nominal(genotypes_t, phenotype_t, residualizer=residualizer)
+                    res = calculate_cis_nominal(genotypes_t, phenotype_t, residualizer=iresidualizer)
                     tstat, slope, slope_se, af, ma_samples, ma_count = [i.cpu().numpy() for i in res]
                     n = len(variant_ids)
                 else:
                     genotypes_t, mask_t = filter_maf_interaction(genotypes_t, interaction_mask_t=interaction_mask_t,
                                                                  maf_threshold_interaction=maf_threshold_interaction)
                     if genotypes_t.shape[0] > 0:
                         mask = mask_t.cpu().numpy()
                         variant_ids = variant_ids[mask]
                         res = calculate_interaction_nominal(genotypes_t, phenotype_t.unsqueeze(0), interaction_t,
-                                                            residualizer=residualizer, return_sparse=False,
+                                                            residualizer=iresidualizer, return_sparse=False,
                                                             variant_ids=variant_ids)
                         tstat, b, b_se, af, ma_samples, ma_count = [i.cpu().numpy() for i in res]
-                        tss_distance = tss_distance[mask]
+                        start_distance = start_distance[mask]
+                        if 'pos' not in phenotype_pos_df:
+                            end_distance = end_distance[mask]
                         n = len(variant_ids)
 
                         # top association
                         ix = np.nanargmax(np.abs(tstat[:,1+ni:]).max(1))  # top association among all interactions tested
                         # index order: 0, 1, 1+ni, 2, 2+ni, 3, 3+ni, ...
                         order = [0] + [i if j % 2 == 0 else i+ni for i in range(1,ni+1) for j in range(2)]
-                        top_s = [phenotype_id, variant_ids[ix], tss_distance[ix], af[ix], ma_samples[ix], ma_count[ix]]
+                        top_s = [phenotype_id, variant_ids[ix], start_distance[ix]]
+                        if 'pos' not in phenotype_pos_df:
+                            top_s += [end_distance[ix]]
+                        top_s += [af[ix], ma_samples[ix], ma_count[ix]]
                         for i in order:
                             top_s += [tstat[ix,i], b[ix,i], b_se[ix,i]]
                         top_s = pd.Series(top_s, index=col_order)
                         if run_eigenmt:  # compute eigenMT correction
                             top_s['tests_emt'] = eigenmt.compute_tests(genotypes_t, var_thresh=0.99, variant_window=200)
                         best_assoc.append(top_s)
                     else:  # all genotypes in window were filtered out
                         n = 0
 
                 if n > 0:
                     chr_res['phenotype_id'].extend([phenotype_id]*n)
                     chr_res['variant_id'].extend(variant_ids)
-                    chr_res['tss_distance'][start:start+n] = tss_distance
+                    chr_res['start_distance'][start:start+n] = start_distance
+                    if 'pos' not in phenotype_pos_df:
+                        chr_res['end_distance'][start:start+n] = end_distance
                     chr_res['af'][start:start+n] = af
                     chr_res['ma_samples'][start:start+n] = ma_samples
                     chr_res['ma_count'][start:start+n] = ma_count
                     if interaction_df is None:
                         chr_res['pval_nominal'][start:start+n] = tstat
                         chr_res['slope'][start:start+n] = slope
                         chr_res['slope_se'][start:start+n] = slope_se
@@ -326,57 +349,69 @@
                 # copy genotypes to GPU
                 genotypes_t = torch.tensor(genotypes, dtype=torch.float).to(device)
                 genotypes_t = genotypes_t[:,genotype_ix_t]
                 impute_mean(genotypes_t)
 
                 variant_ids = variant_df.index[genotype_range[0]:genotype_range[-1]+1]
                 # assuming that the TSS for all grouped phenotypes is the same
-                tss_distance = np.int32(variant_df['pos'].values[genotype_range[0]:genotype_range[-1]+1] - igc.phenotype_tss[phenotype_ids[0]])
+                start_distance = np.int32(variant_df['pos'].values[genotype_range[0]:genotype_range[-1]+1] - igc.phenotype_start[phenotype_ids[0]])
+                if 'pos' not in phenotype_pos_df:
+                    end_distance = np.int32(variant_df['pos'].values[genotype_range[0]:genotype_range[-1]+1] - igc.phenotype_end[phenotype_ids[0]])
 
                 if maf_threshold > 0:
                     maf_t = calculate_maf(genotypes_t)
                     mask_t = maf_t >= maf_threshold
                     genotypes_t = genotypes_t[mask_t]
                     mask = mask_t.cpu().numpy().astype(bool)
                     variant_ids = variant_ids[mask]
-                    tss_distance = tss_distance[mask]
+                    start_distance = start_distance[mask]
+                    if 'pos' not in phenotype_pos_df:
+                        end_distance = end_distance[mask]
+
+                if paired_covariate_df is None or phenotype_id not in paired_covariate_df:
+                    iresidualizer = residualizer
+                else:
+                    iresidualizer = Residualizer(torch.tensor(np.c_[covariates_df, paired_covariate_df[phenotype_id]],
+                                                              dtype=torch.float32).to(device))
 
                 if interaction_df is not None:
                     genotypes_t, mask_t = filter_maf_interaction(genotypes_t, interaction_mask_t=interaction_mask_t,
                                                                  maf_threshold_interaction=maf_threshold_interaction)
                     mask = mask_t.cpu().numpy()
                     variant_ids = variant_ids[mask]
-                    tss_distance = tss_distance[mask]
+                    start_distance = start_distance[mask]
+                    if 'pos' not in phenotype_pos_df:
+                        end_distance = end_distance[mask]
 
                 n = len(variant_ids)
 
                 if genotypes_t.shape[0] > 0:
                     # process first phenotype in group
                     phenotype_id = phenotype_ids[0]
                     phenotype_t = torch.tensor(phenotypes[0], dtype=torch.float).to(device)
 
                     if interaction_df is None:
-                        res = calculate_cis_nominal(genotypes_t, phenotype_t, residualizer=residualizer)
+                        res = calculate_cis_nominal(genotypes_t, phenotype_t, residualizer=iresidualizer)
                         tstat, slope, slope_se, af, ma_samples, ma_count = [i.cpu().numpy() for i in res]
                     else:
                         res = calculate_interaction_nominal(genotypes_t, phenotype_t.unsqueeze(0), interaction_t,
-                                                            residualizer=residualizer, return_sparse=False,
+                                                            residualizer=iresidualizer, return_sparse=False,
                                                             variant_ids=variant_ids)
                         tstat, b, b_se, af, ma_samples, ma_count = [i.cpu().numpy() for i in res]
                     px = [phenotype_id]*n
 
                     # iterate over remaining phenotypes in group
                     for phenotype, phenotype_id in zip(phenotypes[1:], phenotype_ids[1:]):
                         phenotype_t = torch.tensor(phenotype, dtype=torch.float).to(device)
                         if interaction_df is None:
-                            res = calculate_cis_nominal(genotypes_t, phenotype_t, residualizer=residualizer)
+                            res = calculate_cis_nominal(genotypes_t, phenotype_t, residualizer=iresidualizer)
                             tstat0, slope0, slope_se0, af, ma_samples, ma_count = [i.cpu().numpy() for i in res]
                         else:
                             res = calculate_interaction_nominal(genotypes_t, phenotype_t.unsqueeze(0), interaction_t,
-                                                                residualizer=residualizer, return_sparse=False,
+                                                                residualizer=iresidualizer, return_sparse=False,
                                                                 variant_ids=variant_ids)
                             tstat0, b0, b_se0, af, ma_samples, ma_count = [i.cpu().numpy() for i in res]
 
                         # find associations that are stronger for current phenotype
                         if interaction_df is None:
                             ix = np.where(np.abs(tstat0) > np.abs(tstat))[0]
                         else:
@@ -392,15 +427,17 @@
                         else:
                             tstat[ix] = tstat0[ix]
                             b[ix] = b0[ix]
                             b_se[ix] = b_se0[ix]
 
                     chr_res['phenotype_id'].extend(px)
                     chr_res['variant_id'].extend(variant_ids)
-                    chr_res['tss_distance'][start:start+n] = tss_distance
+                    chr_res['start_distance'][start:start+n] = start_distance
+                    if 'pos' not in phenotype_pos_df:
+                        chr_res['end_distance'][start:start+n] = end_distance
                     chr_res['af'][start:start+n] = af
                     chr_res['ma_samples'][start:start+n] = ma_samples
                     chr_res['ma_count'][start:start+n] = ma_count
                     if interaction_df is None:
                         chr_res['pval_nominal'][start:start+n] = tstat
                         chr_res['slope'][start:start+n] = slope
                         chr_res['slope_se'][start:start+n] = slope_se
@@ -415,17 +452,19 @@
                         chr_res['b_gi'][start:start+n]    = b[:,1+ni:]
                         chr_res['b_gi_se'][start:start+n] = b_se[:,1+ni:]
 
                     # top association for the group
                     if interaction_df is not None:
                         ix = np.nanargmax(np.abs(tstat[:,1+ni:]).max(1))  # top association among all interactions tested
                         # index order: 0, 1, 1+ni, 2, 2+ni, 3, 3+ni, ...
-                        order = [0] + [i if j % 2 == 0 else i+ni for i in range(1,ni+1) for j in range(2)]
-                        top_s = [chr_res['phenotype_id'][start:start+n][ix], variant_ids[ix],
-                                 tss_distance[ix], af[ix], ma_samples[ix], ma_count[ix]]
+                        order = [0] + [i if j % 2 == 0 else i+ni for i in range(1, ni+1) for j in range(2)]
+                        top_s = [chr_res['phenotype_id'][start:start+n][ix], variant_ids[ix], start_distance[ix]]
+                        if 'pos' not in phenotype_pos_df:
+                            top_s += [end_distance[ix]]
+                        top_s += [af[ix], ma_samples[ix], ma_count[ix]]
                         for i in order:
                             top_s += [tstat[ix,i], b[ix,i], b_se[ix,i]]
                         top_s = pd.Series(top_s, index=col_order)
                         top_s['num_phenotypes'] = len(phenotype_ids)
                         if run_eigenmt:  # compute eigenMT correction
                             top_s['tests_emt'] = eigenmt.compute_tests(genotypes_t, var_thresh=0.99, variant_window=200)
                         best_assoc.append(top_s)
@@ -435,60 +474,80 @@
         logger.write(f'    time elapsed: {(time.time()-start_time)/60:.2f} min')
 
         # convert to dataframe, compute p-values and write current chromosome
         if start < len(chr_res['af']):
             for x in chr_res:
                 chr_res[x] = chr_res[x][:start]
 
-        if write_stats:
+        if write_stats:  # write full summary stats for current chromosome
             if interaction_df is not None:
                 cols = ['pval_i', 'b_i', 'b_i_se', 'pval_gi', 'b_gi', 'b_gi_se']
                 if ni == 1:  # squeeze columns
-                    for k in cols:
-                        chr_res[k] = chr_res[k][:,0]
+                    for c in cols:
+                        chr_res[c] = chr_res[c][:,0]
                 else: # split interactions
                     for i in range(0, ni):  # fix order
-                        for k in cols:
-                            chr_res[k.replace('i', f"i{i+1}")] = None
-                    for k in cols:
+                        for c in cols:
+                            chr_res[c.replace('i', f"i{i+1}")] = None
+                    for c in cols:
                         for i in range(0, ni):
-                            chr_res[k.replace('i', f"i{i+1}")] = chr_res[k][:,i]
-                        del chr_res[k]
+                            chr_res[c.replace('i', f"i{i+1}")] = chr_res[c][:,i]
+                        del chr_res[c]
             chr_res_df = pd.DataFrame(chr_res)
+
+            if paired_covariate_df is not None:
+                idof = dof - chr_res_df['phenotype_id'].isin(paired_covariate_df.columns).astype(int).values
+            else:
+                idof = dof
+
             if interaction_df is None:
                 m = chr_res_df['pval_nominal'].notnull()
-                chr_res_df.loc[m, 'pval_nominal'] = 2*stats.t.cdf(-chr_res_df.loc[m, 'pval_nominal'].abs(), dof)
+                m = m[m].index
+                if paired_covariate_df is not None:
+                    idof = idof[m]
+                chr_res_df.loc[m, 'pval_nominal'] = 2*stats.t.cdf(-chr_res_df.loc[m, 'pval_nominal'].abs(), idof)
             else:
                 if ni == 1:
                     m = chr_res_df['pval_gi'].notnull()
-                    chr_res_df.loc[m, 'pval_g'] =  2*stats.t.cdf(-chr_res_df.loc[m, 'pval_g'].abs(), dof)
-                    chr_res_df.loc[m, 'pval_i'] =  2*stats.t.cdf(-chr_res_df.loc[m, 'pval_i'].abs(), dof)
-                    chr_res_df.loc[m, 'pval_gi'] = 2*stats.t.cdf(-chr_res_df.loc[m, 'pval_gi'].abs(), dof)
+                    m = m[m].index
+                    if paired_covariate_df is not None:
+                        idof = idof[m]
+                    chr_res_df.loc[m, 'pval_g'] =  2*stats.t.cdf(-chr_res_df.loc[m, 'pval_g'].abs(), idof)
+                    chr_res_df.loc[m, 'pval_i'] =  2*stats.t.cdf(-chr_res_df.loc[m, 'pval_i'].abs(), idof)
+                    chr_res_df.loc[m, 'pval_gi'] = 2*stats.t.cdf(-chr_res_df.loc[m, 'pval_gi'].abs(), idof)
                 else:
                     m = chr_res_df['pval_gi1'].notnull()
-                    chr_res_df.loc[m, 'pval_g'] =  2*stats.t.cdf(-chr_res_df.loc[m, 'pval_g'].abs(), dof)
+                    m = m[m].index
+                    if paired_covariate_df is not None:
+                        idof = idof[m]
+                    chr_res_df.loc[m, 'pval_g'] =  2*stats.t.cdf(-chr_res_df.loc[m, 'pval_g'].abs(), idof)
                     for i in range(1, ni+1):
-                        chr_res_df.loc[m, f'pval_i{i}'] =  2*stats.t.cdf(-chr_res_df.loc[m, f'pval_i{i}'].abs(), dof)
-                        chr_res_df.loc[m, f'pval_gi{i}'] = 2*stats.t.cdf(-chr_res_df.loc[m, f'pval_gi{i}'].abs(), dof)
+                        chr_res_df.loc[m, f'pval_i{i}'] =  2*stats.t.cdf(-chr_res_df.loc[m, f'pval_i{i}'].abs(), idof)
+                        chr_res_df.loc[m, f'pval_gi{i}'] = 2*stats.t.cdf(-chr_res_df.loc[m, f'pval_gi{i}'].abs(), idof)
                     # substitute column headers
                     chr_res_df.rename(columns=var_dict, inplace=True)
             print('    * writing output')
             chr_res_df.to_parquet(os.path.join(output_dir, f'{prefix}.cis_qtl_pairs.{chrom}.parquet'))
 
     if interaction_df is not None and len(best_assoc) > 0:
         best_assoc = pd.concat(best_assoc, axis=1, sort=False).T.set_index('phenotype_id').infer_objects()
         m = best_assoc['pval_g'].notnull()
-        best_assoc.loc[m, 'pval_g'] =  2*stats.t.cdf(-best_assoc.loc[m, 'pval_g'].abs(), dof)
+        m = m[m].index
+        if paired_covariate_df is not None:
+            idof = dof - best_assoc.index.isin(paired_covariate_df.columns).astype(int).values[m]
+        else:
+            idof = dof
+        best_assoc.loc[m, 'pval_g'] =  2*stats.t.cdf(-best_assoc.loc[m, 'pval_g'].abs(), idof)
         if ni == 1:
-            best_assoc.loc[m, 'pval_i'] =  2*stats.t.cdf(-best_assoc.loc[m, 'pval_i'].abs(), dof)
-            best_assoc.loc[m, 'pval_gi'] = 2*stats.t.cdf(-best_assoc.loc[m, 'pval_gi'].abs(), dof)
+            best_assoc.loc[m, 'pval_i'] =  2*stats.t.cdf(-best_assoc.loc[m, 'pval_i'].abs(), idof)
+            best_assoc.loc[m, 'pval_gi'] = 2*stats.t.cdf(-best_assoc.loc[m, 'pval_gi'].abs(), idof)
         else:
             for i in range(1, ni+1):
-                best_assoc.loc[m, f'pval_i{i}'] =  2*stats.t.cdf(-best_assoc.loc[m, f'pval_i{i}'].abs(), dof)
-                best_assoc.loc[m, f'pval_gi{i}'] = 2*stats.t.cdf(-best_assoc.loc[m, f'pval_gi{i}'].abs(), dof)
+                best_assoc.loc[m, f'pval_i{i}'] =  2*stats.t.cdf(-best_assoc.loc[m, f'pval_i{i}'].abs(), idof)
+                best_assoc.loc[m, f'pval_gi{i}'] = 2*stats.t.cdf(-best_assoc.loc[m, f'pval_gi{i}'].abs(), idof)
         if run_eigenmt and ni == 1:  # leave correction of specific p-values up to user for now (TODO)
             if group_s is None:
                 best_assoc['pval_emt'] = np.minimum(best_assoc['tests_emt']*best_assoc['pval_gi'], 1)
             else:
                 best_assoc['pval_emt'] = np.minimum(best_assoc['num_phenotypes']*best_assoc['tests_emt']*best_assoc['pval_gi'], 1)
             best_assoc['pval_adj_bh'] = eigenmt.padjust_bh(best_assoc['pval_emt'])
         if ni > 1:  # substitute column headers
@@ -497,18 +556,18 @@
             best_assoc.to_csv(os.path.join(output_dir, f'{prefix}.cis_qtl_top_assoc.txt.gz'),
                               sep='\t', float_format='%.6g')
         else:
             return best_assoc
     logger.write('done.')
 
 
-def prepare_cis_output(r_nominal, r2_perm, std_ratio, g, num_var, dof, variant_id, tss_distance, phenotype_id, nperm=10000):
+def prepare_cis_output(r_nominal, r2_perm, std_ratio, g, num_var, dof, variant_id, start_distance, end_distance, phenotype_id, nperm=10000):
     """Return nominal p-value, allele frequencies, etc. as pd.Series"""
     r2_nominal = r_nominal*r_nominal
-    pval_perm = (np.sum(r2_perm>=r2_nominal)+1) / (nperm+1)
+    pval_perm = (np.sum(r2_perm >= r2_nominal)+1) / (nperm+1)
 
     slope = r_nominal * std_ratio
     tstat2 = dof * r2_nominal / (1 - r2_nominal)
     slope_se = np.abs(slope) / np.sqrt(tstat2)
 
     n2 = 2*len(g)
     af = np.sum(g) / n2
@@ -522,52 +581,54 @@
     res_s = pd.Series(OrderedDict([
         ('num_var', num_var),
         ('beta_shape1', np.NaN),
         ('beta_shape2', np.NaN),
         ('true_df', np.NaN),
         ('pval_true_df', np.NaN),
         ('variant_id', variant_id),
-        ('tss_distance', tss_distance),
+        ('start_distance', start_distance),
+        ('end_distance', end_distance),
         ('ma_samples', ma_samples),
         ('ma_count', ma_count),
         ('af', af),
         ('pval_nominal', pval_from_corr(r2_nominal, dof)),
         ('slope', slope),
         ('slope_se', slope_se),
         ('pval_perm', pval_perm),
         ('pval_beta', np.NaN),
     ]), name=phenotype_id)
     return res_s
 
 
-def _process_group_permutations(buf, variant_df, tss, dof, group_id, nperm=10000, beta_approx=True):
+def _process_group_permutations(buf, variant_df, start_pos, end_pos, dof, group_id, nperm=10000, beta_approx=True):
     """
     Merge results for grouped phenotypes
 
     buf: [r_nominal, std_ratio, var_ix, r2_perm, g, num_var, phenotype_id]
     """
     # select phenotype with strongest nominal association
     max_ix = np.argmax(np.abs([b[0] for b in buf]))
     r_nominal, std_ratio, var_ix = buf[max_ix][:3]
     g, num_var, phenotype_id = buf[max_ix][4:]
     # select best phenotype correlation for each permutation
     r2_perm = np.max([b[3] for b in buf], 0)
     # return r_nominal, std_ratio, var_ix, r2_perm, g, num_var, phenotype_id
     variant_id = variant_df.index[var_ix]
-    tss_distance = variant_df['pos'].values[var_ix] - tss
-    res_s = prepare_cis_output(r_nominal, r2_perm, std_ratio, g, num_var, dof, variant_id, tss_distance, phenotype_id, nperm=nperm)
+    start_distance = variant_df['pos'].values[var_ix] - start_pos
+    end_distance = variant_df['pos'].values[var_ix] - end_pos
+    res_s = prepare_cis_output(r_nominal, r2_perm, std_ratio, g, num_var, dof, variant_id, start_distance, end_distance, phenotype_id, nperm=nperm)
     if beta_approx:
         res_s[['pval_beta', 'beta_shape1', 'beta_shape2', 'true_df', 'pval_true_df']] = calculate_beta_approx_pval(r2_perm, r_nominal*r_nominal, dof*0.25)
     res_s['group_id'] = group_id
     res_s['group_size'] = len(buf)
     return res_s
 
 
 def map_cis(genotype_df, variant_df, phenotype_df, phenotype_pos_df, covariates_df=None,
-            group_s=None, maf_threshold=0, beta_approx=True, nperm=10000,
+            group_s=None, paired_covariate_df=None, maf_threshold=0, beta_approx=True, nperm=10000,
             window=1000000, random_tiebreak=False, logger=None, seed=None,
             verbose=True, warn_monomorphic=True):
     """Run cis-QTL mapping"""
 
     device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
 
     if logger is None:
@@ -576,27 +637,34 @@
     logger.write('cis-QTL mapping: empirical p-values for phenotypes')
     logger.write(f'  * {phenotype_df.shape[1]} samples')
     logger.write(f'  * {phenotype_df.shape[0]} phenotypes')
     if group_s is not None:
         logger.write(f'  * {len(group_s.unique())} phenotype groups')
         group_dict = group_s.to_dict()
     if covariates_df is not None:
-        assert np.all(phenotype_df.columns==covariates_df.index), 'Sample names in phenotype matrix columns and covariate matrix rows do not match!'
+        assert covariates_df.index.equals(phenotype_df.columns), 'Sample names in phenotype matrix columns and covariate matrix rows do not match!'
         assert ~(covariates_df.isnull().any().any()), f'Missing or null values in covariates matrix, in columns {",".join(covariates_df.columns[covariates_df.isnull().any(axis=0)].astype(str))}'
         logger.write(f'  * {covariates_df.shape[1]} covariates')
         residualizer = Residualizer(torch.tensor(covariates_df.values, dtype=torch.float32).to(device))
         dof = phenotype_df.shape[1] - 2 - covariates_df.shape[1]
     else:
         residualizer = None
         dof = phenotype_df.shape[1] - 2
+    if paired_covariate_df is not None:
+        assert covariates_df is not None
+        assert paired_covariate_df.index.isin(phenotype_df.index).all(), f"Paired covariate phenotypes must be present in phenotype matrix."
+        assert paired_covariate_df.columns.equals(phenotype_df.columns), f"Paired covariate samples must match samples in phenotype matrix."
+        paired_covariate_df = paired_covariate_df.T  # samples x phenotypes
+        logger.write(f'  * including phenotype-specific covariate')
     logger.write(f'  * {genotype_df.shape[0]} variants')
     if maf_threshold > 0:
         logger.write(f'  * applying in-sample {maf_threshold} MAF filter')
     if random_tiebreak:
         logger.write(f'  * randomly selecting top variant in case of ties')
+    logger.write(f'  * cis-window: ±{window:,}')
 
     genotype_ix = np.array([genotype_df.columns.tolist().index(i) for i in phenotype_df.columns])
     genotype_ix_t = torch.from_numpy(genotype_ix).to(device)
 
     # permutation indices
     n_samples = phenotype_df.shape[1]
     ix = np.arange(n_samples)
@@ -634,24 +702,32 @@
                     logger.write(f'    * WARNING: excluding {mono_t.sum()} monomorphic variants')
 
             if genotypes_t.shape[0] == 0:
                 logger.write(f'WARNING: skipping {phenotype_id} (no valid variants)')
                 continue
 
             phenotype_t = torch.tensor(phenotype, dtype=torch.float).to(device)
-
+            if paired_covariate_df is None or phenotype_id not in paired_covariate_df:
+                iresidualizer = residualizer
+                idof = dof
+            else:
+                iresidualizer = Residualizer(torch.tensor(np.c_[covariates_df, paired_covariate_df[phenotype_id]],
+                                                          dtype=torch.float32).to(device))
+                idof = dof - 1
             res = calculate_cis_permutations(genotypes_t, phenotype_t, permutation_ix_t,
-                                             residualizer=residualizer, random_tiebreak=random_tiebreak)
+                                             residualizer=iresidualizer, random_tiebreak=random_tiebreak)
             r_nominal, std_ratio, var_ix, r2_perm, g = [i.cpu().numpy() for i in res]
             var_ix = genotype_range[var_ix]
             variant_id = variant_df.index[var_ix]
-            tss_distance = variant_df['pos'].values[var_ix] - igc.phenotype_tss[phenotype_id]
-            res_s = prepare_cis_output(r_nominal, r2_perm, std_ratio, g, genotypes_t.shape[0], dof, variant_id, tss_distance, phenotype_id, nperm=nperm)
+            start_distance = variant_df['pos'].values[var_ix] - igc.phenotype_start[phenotype_id]
+            end_distance = variant_df['pos'].values[var_ix] - igc.phenotype_end[phenotype_id]
+            res_s = prepare_cis_output(r_nominal, r2_perm, std_ratio, g, genotypes_t.shape[0], idof, variant_id,
+                                       start_distance, end_distance, phenotype_id, nperm=nperm)
             if beta_approx:
-                res_s[['pval_beta', 'beta_shape1', 'beta_shape2', 'true_df', 'pval_true_df']] = calculate_beta_approx_pval(r2_perm, r_nominal*r_nominal, dof)
+                res_s[['pval_beta', 'beta_shape1', 'beta_shape2', 'true_df', 'pval_true_df']] = calculate_beta_approx_pval(r2_perm, r_nominal*r_nominal, idof)
             res_df.append(res_s)
     else:  # grouped mode
         for k, (phenotypes, genotypes, genotype_range, phenotype_ids, group_id) in enumerate(igc.generate_data(verbose=verbose), 1):
             # copy genotypes to GPU
             genotypes_t = torch.tensor(genotypes, dtype=torch.float).to(device)
             genotypes_t = genotypes_t[:,genotype_ix_t]
             impute_mean(genotypes_t)
@@ -668,27 +744,35 @@
             if mono_t.any():
                 genotypes_t = genotypes_t[~mono_t]
                 genotype_range = genotype_range[~mono_t.cpu()]
                 if warn_monomorphic:
                     logger.write(f'    * WARNING: excluding {mono_t.sum()} monomorphic variants')
 
             if genotypes_t.shape[0] == 0:
-                logger.write(f'WARNING: skipping {phenotype_id} (no valid variants)')
+                logger.write(f'WARNING: skipping {group_id} (no valid variants)')
                 continue
 
             # iterate over phenotypes
             buf = []
             for phenotype, phenotype_id in zip(phenotypes, phenotype_ids):
                 phenotype_t = torch.tensor(phenotype, dtype=torch.float).to(device)
+                if paired_covariate_df is None or phenotype_id not in paired_covariate_df:
+                    iresidualizer = residualizer
+                    idof = dof
+                else:
+                    iresidualizer = Residualizer(torch.tensor(np.c_[covariates_df, paired_covariate_df[phenotype_id]],
+                                                              dtype=torch.float32).to(device))
+                    idof = dof - 1
                 res = calculate_cis_permutations(genotypes_t, phenotype_t, permutation_ix_t,
-                                                 residualizer=residualizer, random_tiebreak=random_tiebreak)
+                                                 residualizer=iresidualizer, random_tiebreak=random_tiebreak)
                 res = [i.cpu().numpy() for i in res]  # r_nominal, std_ratio, var_ix, r2_perm, g
                 res[2] = genotype_range[res[2]]
                 buf.append(res + [genotypes_t.shape[0], phenotype_id])
-            res_s = _process_group_permutations(buf, variant_df, igc.phenotype_tss[phenotype_ids[0]], dof,
+            res_s = _process_group_permutations(buf, variant_df, igc.phenotype_start[phenotype_ids[0]],
+                                                igc.phenotype_end[phenotype_ids[0]], idof,
                                                 group_id, nperm=nperm, beta_approx=beta_approx)
             res_df.append(res_s)
 
     res_df = pd.concat(res_df, axis=1, sort=False).T
     res_df.index.name = 'phenotype_id'
     logger.write(f'  Time elapsed: {(time.time()-start_time)/60:.2f} min')
     logger.write('done.')
@@ -701,25 +785,26 @@
     """
     Run independent cis-QTL mapping (forward-backward regression)
 
     cis_df: output from map_cis, annotated with q-values (calculate_qvalues)
     """
     device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
 
-    assert np.all(phenotype_df.index==phenotype_pos_df.index)
-    assert np.all(covariates_df.index==phenotype_df.columns)
+    assert phenotype_df.index.equals(phenotype_pos_df.index)
+    assert covariates_df.index.equals(phenotype_df.columns)
     if logger is None:
         logger = SimpleLogger()
 
-    signif_df = cis_df[cis_df[fdr_col]<=fdr].copy()
-    cols = [
-        'num_var', 'beta_shape1', 'beta_shape2', 'true_df', 'pval_true_df',
-        'variant_id', 'tss_distance', 'ma_samples', 'ma_count', 'af',
-        'pval_nominal', 'slope', 'slope_se', 'pval_perm', 'pval_beta',
-    ]
+    signif_df = cis_df[cis_df[fdr_col] <= fdr].copy()
+    if len(signif_df) == 0:
+        raise ValueError(f"No significant phenotypes at FDR ≤ {fdr}.")
+
+    cols = ['num_var', 'beta_shape1', 'beta_shape2', 'true_df', 'pval_true_df', 'variant_id',
+            'start_distance', 'end_distance', 'ma_samples', 'ma_count', 'af',
+            'pval_nominal', 'slope', 'slope_se', 'pval_perm', 'pval_beta']
     if group_s is not None:
         cols += ['group_id', 'group_size']
     signif_df = signif_df[cols]
     signif_threshold = signif_df['pval_beta'].max()
     # subset significant phenotypes
     if group_s is None:
         ix = phenotype_df.index[phenotype_df.index.isin(signif_df.index)]
@@ -736,14 +821,15 @@
         group_dict = group_s.to_dict()
     logger.write(f'  * {covariates_df.shape[1]} covariates')
     logger.write(f'  * {genotype_df.shape[0]} variants')
     if maf_threshold > 0:
         logger.write(f'  * applying in-sample {maf_threshold} MAF filter')
     if random_tiebreak:
         logger.write(f'  * randomly selecting top variant in case of ties')
+    logger.write(f'  * cis-window: ±{window:,}')
     phenotype_df = phenotype_df.loc[ix]
     phenotype_pos_df = phenotype_pos_df.loc[ix]
 
     genotype_ix = np.array([genotype_df.columns.tolist().index(i) for i in phenotype_df.columns])
     genotype_ix_t = torch.from_numpy(genotype_ix).to(device)
     dof = phenotype_df.shape[1] - 2 - covariates_df.shape[1]
     ix_dict = {i:k for k,i in enumerate(genotype_df.index)}
@@ -796,16 +882,18 @@
                                                  residualizer=residualizer, random_tiebreak=random_tiebreak)
                 r_nominal, std_ratio, var_ix, r2_perm, g = [i.cpu().numpy() for i in res]
                 x = calculate_beta_approx_pval(r2_perm, r_nominal*r_nominal, dof)
                 # add to list if empirical p-value passes significance threshold
                 if x[0] <= signif_threshold:
                     var_ix = genotype_range[var_ix]
                     variant_id = variant_df.index[var_ix]
-                    tss_distance = variant_df['pos'].values[var_ix] - igc.phenotype_tss[phenotype_id]
-                    res_s = prepare_cis_output(r_nominal, r2_perm, std_ratio, g, genotypes.shape[0], dof, variant_id, tss_distance, phenotype_id, nperm=nperm)
+                    start_distance = variant_df['pos'].values[var_ix] - igc.phenotype_start[phenotype_id]
+                    end_distance = variant_df['pos'].values[var_ix] - igc.phenotype_end[phenotype_id]
+                    res_s = prepare_cis_output(r_nominal, r2_perm, std_ratio, g, genotypes.shape[0], dof, variant_id,
+                                               start_distance, end_distance, phenotype_id, nperm=nperm)
                     res_s[['pval_beta', 'beta_shape1', 'beta_shape2', 'true_df', 'pval_true_df']] = x
                     forward_df.append(res_s)
                 else:
                     break
             forward_df = pd.concat(forward_df, axis=1, sort=False).T
             dosage_df = pd.DataFrame(dosage_dict)
 
@@ -824,16 +912,18 @@
                     res = calculate_cis_permutations(genotypes_t, phenotype_t, permutation_ix_t,
                                                      residualizer=residualizer, random_tiebreak=random_tiebreak)
                     r_nominal, std_ratio, var_ix, r2_perm, g = [i.cpu().numpy() for i in res]
                     var_ix = genotype_range[var_ix]
                     variant_id = variant_df.index[var_ix]
                     x = calculate_beta_approx_pval(r2_perm, r_nominal*r_nominal, dof)
                     if x[0] <= signif_threshold and variant_id not in variant_set:
-                        tss_distance = variant_df['pos'].values[var_ix] - igc.phenotype_tss[phenotype_id]
-                        res_s = prepare_cis_output(r_nominal, r2_perm, std_ratio, g, genotypes.shape[0], dof, variant_id, tss_distance, phenotype_id, nperm=nperm)
+                        start_distance = variant_df['pos'].values[var_ix] - igc.phenotype_start[phenotype_id]
+                        end_distance = variant_df['pos'].values[var_ix] - igc.phenotype_end[phenotype_id]
+                        res_s = prepare_cis_output(r_nominal, r2_perm, std_ratio, g, genotypes.shape[0], dof, variant_id,
+                                                   start_distance, end_distance, phenotype_id, nperm=nperm)
                         res_s[['pval_beta', 'beta_shape1', 'beta_shape2', 'true_df', 'pval_true_df']] = x
                         res_s['rank'] = k
                         back_df.append(res_s)
                         variant_set.add(variant_id)
                 if len(back_df)>0:
                     res_df.append(pd.concat(back_df, axis=1, sort=False).T)
             else:  # single independent variant
@@ -851,15 +941,15 @@
                 maf_t = calculate_maf(genotypes_t)
                 mask_t = maf_t >= maf_threshold
                 genotypes_t = genotypes_t[mask_t]
                 mask = mask_t.cpu().numpy().astype(bool)
                 genotype_range = genotype_range[mask]
 
             # 1) forward pass
-            forward_df = [signif_df[signif_df['group_id']==group_id].iloc[0]]  # initialize results with top variant
+            forward_df = [signif_df[signif_df['group_id'] == group_id].iloc[0]]  # initialize results with top variant
             covariates = covariates_df.values.copy()  # initialize covariates
             dosage_dict = {}
             while True:
                 # add variant to covariates
                 variant_id = forward_df[-1]['variant_id']
                 ig = genotype_df.values[ix_dict[variant_id], genotype_ix].copy()
                 m = ig == -1
@@ -874,15 +964,16 @@
                 for phenotype, phenotype_id in zip(phenotypes, phenotype_ids):
                     phenotype_t = torch.tensor(phenotype, dtype=torch.float).to(device)
                     res = calculate_cis_permutations(genotypes_t, phenotype_t, permutation_ix_t,
                                                      residualizer=residualizer, random_tiebreak=random_tiebreak)
                     res = [i.cpu().numpy() for i in res]  # r_nominal, std_ratio, var_ix, r2_perm, g
                     res[2] = genotype_range[res[2]]
                     buf.append(res + [genotypes.shape[0], phenotype_id])
-                res_s = _process_group_permutations(buf, variant_df, igc.phenotype_tss[phenotype_ids[0]], dof, group_id, nperm=nperm)
+                res_s = _process_group_permutations(buf, variant_df, igc.phenotype_start[phenotype_ids[0]],
+                                                    igc.phenotype_end[phenotype_ids[0]], dof, group_id, nperm=nperm)
 
                 # add to list if significant
                 if res_s['pval_beta'] <= signif_threshold:
                     forward_df.append(res_s)
                 else:
                     break
             forward_df = pd.concat(forward_df, axis=1, sort=False).T
@@ -905,15 +996,16 @@
                     for phenotype, phenotype_id in zip(phenotypes, phenotype_ids):
                         phenotype_t = torch.tensor(phenotype, dtype=torch.float).to(device)
                         res = calculate_cis_permutations(genotypes_t, phenotype_t, permutation_ix_t,
                                                          residualizer=residualizer, random_tiebreak=random_tiebreak)
                         res = [i.cpu().numpy() for i in res]  # r_nominal, std_ratio, var_ix, r2_perm, g
                         res[2] = genotype_range[res[2]]
                         buf.append(res + [genotypes.shape[0], phenotype_id])
-                    res_s = _process_group_permutations(buf, variant_df, igc.phenotype_tss[phenotype_ids[0]], dof, group_id, nperm=nperm)
+                    res_s = _process_group_permutations(buf, variant_df, igc.phenotype_start[phenotype_ids[0]],
+                                                        igc.phenotype_end[phenotype_ids[0]], dof, group_id, nperm=nperm)
 
                     if res_s['pval_beta'] <= signif_threshold and variant_id not in variant_set:
                         res_s['rank'] = k
                         back_df.append(res_s)
                         variant_set.add(variant_id)
                 if len(back_df)>0:
                     res_df.append(pd.concat(back_df, axis=1, sort=False).T)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tensorqtl-1.0.7/tensorqtl/coloc.py` & `tensorqtl-1.0.8/tensorqtl/coloc.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,16 +33,16 @@
     # phenotype 1
     if mode == 'beta':
         r_nominal_t, genotype_var_t, phenotype_var_t = calculate_corr(
             genotypes1_t, phenotype1_t.reshape(1,-1), residualizer1, return_var=True)
         r_nominal_t = r_nominal_t.squeeze()
         var_ratio_t = phenotype_var_t.reshape(1,-1) / genotype_var_t.reshape(-1,1)
     else:
-        r_nominal_t = calculate_corr(genotypes1_t, phenotype1_t.reshape(1,-1),
-                                     residualizer1, return_var=False).squeeze()
+        r_nominal_t = calculate_corr(
+            genotypes1_t, phenotype1_t.reshape(1,-1), residualizer1, return_var=False).squeeze()
     r2_nominal_t = r_nominal_t.double().pow(2)
 
     if residualizer1 is not None:
         dof = residualizer1.dof
     else:
         dof = phenotype1_t.shape[0] - 2
 
@@ -169,21 +169,21 @@
         phenotype1_t = torch.tensor(phenotype1, dtype=torch.float).to(device)
         phenotype2_t = torch.tensor(phenotype2, dtype=torch.float).to(device)
         genotypes_t = torch.tensor(genotypes, dtype=torch.float).to(device)
         genotypes1_t = genotypes_t[:,genotype1_ix_t]
         genotypes2_t = genotypes_t[:,genotype2_ix_t]
         del genotypes_t
 
+        impute_mean(genotypes1_t)
+        impute_mean(genotypes2_t)
         # filter monomorphic sites
         m = ((genotypes1_t==0).all(1) | (genotypes1_t==1).all(1) | (genotypes1_t==2).all(1) |
              (genotypes2_t==0).all(1) | (genotypes2_t==1).all(1) | (genotypes2_t==2).all(1))
         genotypes1_t = genotypes1_t[~m]
         genotypes2_t = genotypes2_t[~m]
-        impute_mean(genotypes1_t)
-        impute_mean(genotypes2_t)
 
         if maf_threshold > 0:
             maf1_t = calculate_maf(genotypes1_t)
             maf2_t = calculate_maf(genotypes2_t)
             mask_t = (maf1_t >= maf_threshold) | (maf2_t >= maf_threshold)
             genotypes1_t = genotypes1_t[mask_t]
             genotypes2_t = genotypes2_t[mask_t]
```

### Comparing `tensorqtl-1.0.7/tensorqtl/core.py` & `tensorqtl-1.0.8/tensorqtl/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 output_dtype_dict = {
     'num_var':np.int32,
     'beta_shape1':np.float32,
     'beta_shape2':np.float32,
     'true_df':np.float32,
     'pval_true_df':np.float64,
     'variant_id':str,
-    'tss_distance':np.int32,
+    'start_distance':np.int32,
+    'end_distance':np.int32,
     'ma_samples':np.int32,
     'ma_count':np.int32,
     'af':np.float32,
     'pval_nominal':np.float64,
     'slope':np.float32,
     'slope_se':np.float32,
     'pval_perm':np.float64,
@@ -362,23 +363,32 @@
     pval_true_dof = pval_from_corr(r2_nominal, true_dof)
     pval_beta = stats.beta.cdf(pval_true_dof, beta_shape1, beta_shape2)
     return pval_beta, beta_shape1, beta_shape2, true_dof, pval_true_dof
 
 #------------------------------------------------------------------------------
 #  i/o functions
 #------------------------------------------------------------------------------
+
 def read_phenotype_bed(phenotype_bed):
-    """Load phenotype BED file as phenotype and TSS DataFrames"""
-    if phenotype_bed.endswith('.bed.gz'):
+    """Load phenotype BED file as phenotype and position DataFrames"""
+    if phenotype_bed.endswith(('.bed.gz', '.bed')):
         phenotype_df = pd.read_csv(phenotype_bed, sep='\t', index_col=3, dtype={'#chr':str, '#Chr':str})
     elif phenotype_bed.endswith('.parquet'):
         phenotype_df = pd.read_parquet(phenotype_bed)
         phenotype_df.set_index(phenotype_df.columns[3], inplace=True)
     else:
         raise ValueError('Unsupported file type.')
     phenotype_df.rename(columns={i:i.lower().replace('#chr','chr') for i in phenotype_df.columns[:3]}, inplace=True)
-    # make sure TSS/cis-window is properly defined
-    if not (phenotype_df['start']+1 == phenotype_df['end']).all():
-        raise ValueError("The BED file must define the TSS/cis-window center, with start+1 == end.")
-    phenotype_pos_df = phenotype_df[['chr', 'end']].rename(columns={'end':'tss'})
+
+    phenotype_df['start'] += 1  # change to 1-based
+    pos_df = phenotype_df[['chr', 'start', 'end']]
     phenotype_df.drop(['chr', 'start', 'end'], axis=1, inplace=True)
-    return phenotype_df, phenotype_pos_df
+
+    # make sure BED file is properly sorted
+    assert pos_df.equals(
+        pos_df.groupby('chr', sort=False, group_keys=False).apply(lambda x: x.sort_values(['start', 'end']))
+    ), "Positions in BED file must be sorted."
+
+    if (pos_df['start'] == pos_df['end']).all():
+        pos_df = pos_df[['chr', 'end']].rename(columns={'end':'pos'})
+
+    return phenotype_df, pos_df
```

### Comparing `tensorqtl-1.0.7/tensorqtl/eigenmt.py` & `tensorqtl-1.0.8/tensorqtl/eigenmt.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,25 +94,25 @@
 
         n_samples, n_features = windows[0].T.shape
         # indices of diagonals
         ix = torch.LongTensor(np.array([np.arange(0, n_features**2, n_features+1)+i*n_features**2 for i in range(shrunk_cov_t.shape[0])])).to(device)
         shrunk_precision_t = torch.zeros(shrunk_cov_t.shape).to(device)
         shrunk_precision_t.view(-1)[ix] = shrunk_cov_t.view(-1)[ix].pow(-0.5)
         shrunk_cor_t = torch.matmul(torch.matmul(shrunk_precision_t, shrunk_cov_t), shrunk_precision_t)
-        eigenvalues_t,_ = torch.symeig(shrunk_cor_t, eigenvectors=False)  # will be deprecated
-        # eigenvalues_t = torch.linalg.eigvalsh(shrunk_cor_t)  # ~2x slower than symeig with 1.10.0+cu102
+        # eigenvalues_t,_ = torch.symeig(shrunk_cor_t, eigenvectors=False)  # will be deprecated
+        eigenvalues_t = torch.linalg.eigvalsh(shrunk_cor_t)  # ~2x slower than symeig with 1.10.0+cu102 and 2.0.1+cu118
 
     # last window
     shrunk_cov0_t, shrinkage0_t = lw_shrink(windows[-1].t())
     shrunk_precision0_t = torch.diag(torch.diag(shrunk_cov0_t).pow(-0.5))
     shrunk_cor0_t = torch.mm(torch.mm(shrunk_precision0_t, shrunk_cov0_t), shrunk_precision0_t)
-    eigenvalues0_t,_ = torch.symeig(shrunk_cor0_t, eigenvectors=False)
-    # eigenvalues0_t = torch.linalg.eigvalsh(shrunk_cor0_t)
+    # eigenvalues0_t,_ = torch.symeig(shrunk_cor0_t, eigenvectors=False)
+    eigenvalues0_t = torch.linalg.eigvalsh(shrunk_cor0_t)
 
-    if len(windows)>1:
+    if len(windows) > 1:
         eigenvalues = list(eigenvalues_t.cpu().numpy())
         eigenvalues.append(eigenvalues0_t.cpu().numpy())
     else:
         eigenvalues = [eigenvalues0_t.cpu().numpy()]
 
     m_eff = 0
     for ev,m in zip(eigenvalues, [i.shape[0] for i in windows]):
@@ -176,8 +176,8 @@
     """Benjamini-Hochberg adjusted p-values"""
     if not np.all(np.isfinite(p)):
         raise ValueError('P values must be finite.')
     n = len(p)
     i = np.arange(n,0,-1)
     o = np.argsort(p)[::-1]
     ro = np.argsort(o)
-    return np.minimum(1, np.minimum.accumulate(np.float(n)/i * np.array(p)[o]))[ro]
+    return np.minimum(1, np.minimum.accumulate(np.float64(n)/i * np.array(p)[o]))[ro]
```

### Comparing `tensorqtl-1.0.7/tensorqtl/genotypeio.py` & `tensorqtl-1.0.8/tensorqtl/genotypeio.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 import pandas as pd
 import tempfile
 import numpy as np
 import subprocess
+import os
 import gzip
 import sys
 import threading
 import queue
+import bisect
 from pandas_plink import read_plink
 
+sys.path.insert(1, os.path.dirname(__file__))
+from core import *
+
 try:
     import pgen
 except ImportError as e:
     pgen = None
 
 
 gt_to_dosage_dict = {'0/0':0, '0/1':1, '1/1':2, './.':np.NaN,
                      '0|0':0, '0|1':1, '1|0':1, '1|1':2, '.|.':np.NaN}
 
 
 def _check_dependency(name):
-    e = subprocess.call('which '+name, shell=True, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
-    if e!=0:
-        raise RuntimeError('External dependency \''+name+'\' not installed')
+    e = subprocess.call(f"which {name}", shell=True, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
+    if e != 0:
+        raise RuntimeError(f"External dependency '{name}' not installed")
 
 
 def print_progress(k, n, entity):
     s = f'\r    processing {entity} {k}/{n}'
     if k == n:
         s += '\n'
     sys.stdout.write(s)
@@ -77,24 +82,24 @@
         return open(vcfpath)
 
 
 def get_sample_ids(vcfpath):
     """Get sample IDs from VCF"""
     with _get_vcf_opener(vcfpath) as vcf:
         for header in vcf:
-            if header[:2]=='##': continue
+            if header[:2] == '##': continue
             break
     return header.strip().split('\t')[9:]
 
 
 def parse_genotypes(x, field='GT'):
     """Convert list of genotypes (str) to np.float32"""
-    if field=='GT':
+    if field == 'GT':
         g = np.float32([gt_to_dosage_dict[i] for i in x])
-    elif field=='DS':
+    elif field == 'DS':
         g = np.float32(x)
     return g
 
 
 def _get_field_ix(line, field):
     """Get position of field ('GT' or 'DS') in FORMAT"""
     fmt = line[8].split(':')
@@ -218,128 +223,48 @@
             return pd.Series(g[0], index=sample_ids, name=variant_id)
 
     def load_genotypes(self):
         """Load all genotypes into memory, as pd.DataFrame"""
         return pd.DataFrame(self.bed.compute(), index=self.bim['snp'], columns=self.fam['iid'])
 
 
-class Plink2Reader(object):
-    def __init__(self, plink_prefix_path, verbose=True, dtype=np.float32):
-        """
-        Class for reading genotypes from PLINK 2 pgen files
-
-        plink_prefix_path: prefix to PLINK pgen,psam,pvar files
-        select_samples: specify a subset of samples
-
-        Notes:
-          Use this command to convert a VCF to PLINK format:
-            plink2 \
-                --output-chr chrM \
-                --vcf ${plink_prefix_path}.vcf.gz \
-                --out ${plink_prefix_path}
-          To use dosages, run:
-            plink2 \
-                --output-chr chrM \
-                --vcf ${plink_prefix_path}.vcf.gz 'dosage=DS' \
-                --out ${plink_prefix_path}
-
-          Requires pgenlib: https://github.com/chrchang/plink-ng/tree/master/2.0/Python
-        """
-
-        self.psam = pgen.read_psam(f"{plink_prefix_path}.psam")
-        self.pvar = pgen.read_pvar(f"{plink_prefix_path}.pvar")
-        self.pgen_file = f"{plink_prefix_path}.pgen"
-        self.sample_ids = self.psam.index.tolist()
-        self.n_samples = self.psam.shape[0]
-        self.chrs = list(self.pvar['chrom'].unique())
-        self.variant_pos = {i:g['pos'] for i,g in self.pvar.set_index('id')[['chrom', 'pos']].groupby('chrom')}
-        self.variant_pos_dict = self.pvar.set_index('id')['pos'].to_dict()
-
-    def get_sample_indexes(self, sample_ids):
-        """Get sorted indexes corresponding to sample IDs"""
-        sample_idxs = [self.sample_ids.index(i) for i in sample_ids]
-        # sort sample IDs by pgen order
-        sidx = np.argsort(sample_idxs)
-        sample_idxs = [sample_idxs[i] for i in sidx]
-        sample_ids_sorted = [sample_ids[i] for i in sidx]
-        return sample_idxs, sample_ids_sorted
-
-    def get_region_index(self, region_str, return_pos=False):
-        s = region_str.split(':')
-        chrom = s[0]
-        c = self.pvar[self.pvar['chrom'] == chrom]
-        if len(s) > 1:
-            start, end = s[1].split('-')
-            c = c[(c['pos'] >= int(start)) & (c['pos'] <= int(end))]
-        if return_pos:
-            return c.index.values, c.set_index('id')['pos']
-        else:
-            return c.index.values
-
-    def get_region(self, region_str, sample_ids=None, impute=False, verbose=False, dtype=np.float32):
-        """Get genotypes for a region defined by 'chr:start-end' or 'chr'"""
-        ix, pos_s = self.get_region_index(region_str, return_pos=True)
-        g = pgen.read_dosages_range(self.pgen_file, ix[0], ix[-1], dtype=dtype)
-        if sample_ids is not None:
-            ix = [self.sample_ids.index(i) for i in sample_ids]
-            g = g[:, ix]
-        if impute:
-            _impute_mean(g, missing=-9, verbose=verbose)
-        return g, pos_s
-
-    def get_genotypes(self, variant_ids, sample_ids=None, impute=False, verbose=False, dtype=np.float32):
-        """Load genotypes for selected variant IDs"""
-        c = self.pvar[self.pvar['id'].isin(variant_ids)]
-        g = pgen.read_dosages_list(self.pgen_file, c.index, dtype=dtype)
-        if sample_ids is not None:
-            ix = [self.sample_ids.index(i) for i in sample_ids]
-            g = g[:, ix]
-        if impute:
-            _impute_mean(g, missing=-9, verbose=verbose)
-        return g, c.set_index('id')['pos']
-
-    def get_genotype(self, variant_id, sample_ids=None, impute=False, verbose=False, dtype=np.float32):
-        """Load genotypes for a single variant ID as pd.Series"""
-        g,_ = self.get_genotypes([variant_id], sample_ids=sample_ids, impute=impute, verbose=verbose, dtype=dtype)
-        if sample_ids is None:
-            return pd.Series(g[0], index=self.sample_ids, name=variant_id)
-        else:
-            return pd.Series(g[0], index=sample_ids, name=variant_id)
-
-    def load_genotypes(self, sample_ids=None):
-        """Load all genotypes into memory, as pd.DataFrame"""
-        if sample_ids is not None:
-            sample_idxs, sample_ids = self.get_sample_indexes(sample_ids)
-        else:
-            sample_idxs = None
-            sample_ids = self.sample_ids
-
-        return pd.DataFrame(pgen.read_dosages_range(self.pgen_file, 0, self.pvar.shape[0]-1, sample_subset=sample_idxs),
-                            index=self.pvar['id'], columns=sample_ids)
-
-
-def load_genotypes(plink_prefix_path, select_samples=None, dtype=np.int8):
+def load_genotypes(genotype_path, select_samples=None, dosages=False):
     """Load all genotypes into a dataframe"""
-
-    print('Loading genotypes ... ', end='', flush=True)
-
-    # identify format
-    if all([os.path.exists(f"{plink_prefix_path}.{ext}" for ext in ['bed', 'bim', 'fam'])]):
-        pr = PlinkReader(plink_prefix_path, select_samples=select_samples, dtype=dtype)
-        df = pr.load_genotypes()
-    elif all([os.path.exists(f"{plink_prefix_path}.{ext}" for ext in ['pgen', 'psam', 'pvar'])]):
+    if all([os.path.exists(f"{genotype_path}.{ext}") for ext in ['pgen', 'psam', 'pvar']]):
         if pgen is None:
-            raise ImportError('The pgenlib package must be installed to use PLINK 2 pgen/psam/pvar files.')
-        pr = Plink2Reader(plink_prefix_path)
-        df = pr.load_genotypes(sample_ids=select_samples)
+            raise ImportError('Pgenlib must be installed to use PLINK 2 pgen/psam/pvar files.')
+        pgr = pgen.PgenReader(genotype_path, select_samples=select_samples)
+        variant_df = pgr.pvar_df.set_index('id')[['chrom', 'pos']]
+        if dosages:
+            genotype_df = pgr.load_dosages()
+        else:
+            genotype_df = pgr.load_genotypes()
+            # temporary workaround
+            genotype_df.values[genotype_df.values == -9] = -1
+    elif all([os.path.exists(f"{genotype_path}.{ext}") for ext in ['bed', 'bim', 'fam']]):
+        pr = PlinkReader(genotype_path, select_samples=select_samples, dtype=np.int8)
+        genotype_df = pr.load_genotypes()
+        variant_df = pr.bim.set_index('snp')[['chrom', 'pos']]
+    elif genotype_path.endswith(('.bed.parquet', '.bed.gz', '.bed')):
+        genotype_df, variant_df = read_phenotype_bed(genotype_path)
+        assert variant_df.columns[1] == 'pos', "The BED file must define a single position for each variant, with start + 1 == end."
+        variant_df.columns = ['chrom', 'pos']
+    elif genotype_path.endswith('.parquet'):
+        genotype_df = pd.read_parquet(genotype_path)
+        variant_df = None
+    elif genotype_path.endswith('.gz'):
+        with gzip.open(genotype_path, 'rt') as f:
+            header = f.readline().strip().split('\t')
+        dtypes = {i:np.float32 for i in header}
+        dtypes[header[0]] = str
+        genotype_df = pd.read_csv(genotype_path, sep='\t', index_col=0, dtype=dtypes)
+        variant_df = None
     else:
-        raise ValueError(f"No compatible PLINK files found for {plink_prefix_path}")
-
-    print('done.', flush=True)
-    return df
+        raise ValueError(f"Failed to load genotypes from {genotype_path}. Supported formats: pgen/psam/pvar, bed/bim/fam, parquet, tsv.gz")
+    return genotype_df, variant_df
 
 
 def get_vcf_region(region_str, vcfpath, field='GT', sample_ids=None, select_samples=None, impute_missing=True):
     """Load VCF region (str: 'chr:start-end') as DataFrame (requires tabix)"""
     s = subprocess.check_output(f'tabix {vcfpath} {region_str}', shell=True)
     s = s.decode().strip().split('\n')
     s = [i.split('\t') for i in s]
@@ -443,88 +368,109 @@
             if verbose:
                 print_progress(k, num_batches, 'batch')
             g = self.genotype_df.values[i[0]:i[1]]
             ix = self.genotype_df.index[i[0]:i[1]]  # variant IDs
             yield g, ix
 
 
+def get_cis_ranges(phenotype_pos_df, chr_variant_dfs, window, verbose=True):
+    """
+
+    start, end indexes (inclusive)
+    """
+    # check phenotypes & calculate genotype ranges
+    # get genotype indexes corresponding to cis-window of each phenotype
+    if 'pos' in phenotype_pos_df:
+        phenotype_pos_df = phenotype_pos_df.rename(columns={'pos':'start'})
+        phenotype_pos_df['end'] = phenotype_pos_df['start']
+    phenotype_pos_dict = phenotype_pos_df.to_dict(orient='index')
+
+    drop_ids = []
+    cis_ranges = {}
+    n = len(phenotype_pos_df)
+    for k, phenotype_id in enumerate(phenotype_pos_df.index, 1):
+        if verbose and (k % 1000 == 0 or k == n):
+            print(f'\r  * checking phenotypes: {k}/{n}',  end='' if k != n else None)
+
+        pos = phenotype_pos_dict[phenotype_id]
+        chrom = pos['chr']
+        m = len(chr_variant_dfs[chrom]['pos'].values)
+        lb = bisect.bisect_left(chr_variant_dfs[chrom]['pos'].values, pos['start'] - window)
+        ub = bisect.bisect_right(chr_variant_dfs[chrom]['pos'].values, pos['end'] + window)
+        if lb != ub:
+            r = chr_variant_dfs[chrom]['index'].values[[lb, ub - 1]]
+        else:
+            r = []
+
+        if len(r) > 0:
+            cis_ranges[phenotype_id] = r
+        else:
+            drop_ids.append(phenotype_id)
+
+    return cis_ranges, drop_ids
+
+
 class InputGeneratorCis(object):
     """
     Input generator for cis-mapping
 
     Inputs:
       genotype_df:      genotype DataFrame (genotypes x samples)
       variant_df:       DataFrame mapping variant_id (index) to chrom, pos
       phenotype_df:     phenotype DataFrame (phenotypes x samples)
-      phenotype_pos_df: DataFrame defining position of each phenotype, with columns 'chr' and 'tss'
-      window:           cis-window (selects variants within +- cis-window from TSS)
+      phenotype_pos_df: DataFrame defining position of each phenotype, with columns ['chr', 'pos'] or ['chr', 'start', 'end']
+      window:           cis-window; selects variants within +- cis-window from 'pos' (e.g., TSS for gene-based features)
+                        or within [start-window, end+window] if 'start' and 'end' are present in phenotype_pos_df
 
     Generates: phenotype array, genotype array (2D), cis-window indices, phenotype ID
     """
     def __init__(self, genotype_df, variant_df, phenotype_df, phenotype_pos_df, group_s=None, window=1000000):
         assert (genotype_df.index == variant_df.index).all()
         assert (phenotype_df.index == phenotype_df.index.unique()).all()
         self.genotype_df = genotype_df
         self.variant_df = variant_df.copy()
         self.variant_df['index'] = np.arange(variant_df.shape[0])
         self.n_samples = phenotype_df.shape[1]
-        self.phenotype_df = phenotype_df
-        self.phenotype_pos_df = phenotype_pos_df
+
+        # drop phenotypes without genotypes on same contig
+        variant_chrs = variant_df['chrom'].unique()
+        phenotype_chrs = phenotype_pos_df['chr'].unique()
+        self.chrs = [i for i in phenotype_chrs if i in variant_chrs]
+        m = phenotype_pos_df['chr'].isin(self.chrs)
+        if any(~m):
+            print(f'    ** dropping {sum(~m)} phenotypes on chrs. without genotypes')
+        self.phenotype_df = phenotype_df[m]
+        self.phenotype_pos_df = phenotype_pos_df[m]
+
         # check for constant phenotypes and drop
-        m = np.all(phenotype_df.values == phenotype_df.values[:,[0]], 1)
+        m = np.all(self.phenotype_df.values == self.phenotype_df.values[:,[0]], 1)
         if m.any():
             print(f'    ** dropping {np.sum(m)} constant phenotypes')
             self.phenotype_df = self.phenotype_df.loc[~m]
             self.phenotype_pos_df = self.phenotype_pos_df.loc[~m]
         self.group_s = None
         self.window = window
 
-        self.phenotype_tss = self.phenotype_pos_df['tss'].to_dict()
-        self.phenotype_chr = self.phenotype_pos_df['chr'].to_dict()
-        variant_chrs = variant_df['chrom'].unique()
-        phenotype_chrs = phenotype_pos_df['chr'].unique()
-        self.chrs = [i for i in phenotype_chrs if i in variant_chrs]
         self.chr_variant_dfs = {c:g[['pos', 'index']] for c,g in self.variant_df.groupby('chrom')}
 
         # check phenotypes & calculate genotype ranges
         # get genotype indexes corresponding to cis-window of each phenotype
-        valid_ix = []
-        self.cis_ranges = {}
-        for k,phenotype_id in enumerate(self.phenotype_df.index,1):
-            if np.mod(k, 1000) == 0 or k == phenotype_df.shape[0]:
-                print(f'\r  * checking phenotypes: {k}/{self.phenotype_df.shape[0]}',
-                      end='' if k != phenotype_df.shape[0] else None)
-
-            tss = self.phenotype_tss[phenotype_id]
-            chrom = self.phenotype_chr[phenotype_id]
-            # r = self.chr_variant_dfs[chrom]['index'].values[
-            #     (self.chr_variant_dfs[chrom]['pos'].values >= tss - self.window) &
-            #     (self.chr_variant_dfs[chrom]['pos'].values <= tss + self.window)
-            # ]
-            # r = [r[0],r[-1]]
-
-            m = len(self.chr_variant_dfs[chrom]['pos'].values)
-            lb = np.searchsorted(self.chr_variant_dfs[chrom]['pos'].values, tss - self.window)
-            ub = np.searchsorted(self.chr_variant_dfs[chrom]['pos'].values, tss + self.window, side='right')
-            if lb != ub:
-                r = self.chr_variant_dfs[chrom]['index'].values[[lb, ub - 1]]
-            else:
-                r = []
-
-            if len(r) > 0:
-                valid_ix.append(phenotype_id)
-                self.cis_ranges[phenotype_id] = r
-        if len(valid_ix) != self.phenotype_df.shape[0]:
-            print('    ** dropping {} phenotypes without variants in cis-window'.format(
-                  self.phenotype_df.shape[0] - len(valid_ix)))
-            self.phenotype_df = self.phenotype_df.loc[valid_ix]
-            self.phenotype_pos_df = self.phenotype_pos_df.loc[valid_ix]
-            self.phenotype_tss = self.phenotype_pos_df['tss'].to_dict()
-            self.phenotype_chr = self.phenotype_pos_df['chr'].to_dict()
+        self.cis_ranges, drop_ids = get_cis_ranges(self.phenotype_pos_df, self.chr_variant_dfs, self.window)
+        if len(drop_ids) > 0:
+            print(f"    ** dropping {len(drop_ids)} phenotypes without variants in cis-window")
+            self.phenotype_df = self.phenotype_df.drop(drop_ids)
+            self.phenotype_pos_df = self.phenotype_pos_df.drop(drop_ids)
+        if 'pos' in self.phenotype_pos_df:
+            self.phenotype_start = self.phenotype_pos_df['pos'].to_dict()
+            self.phenotype_end = self.phenotype_start
+        else:
+            self.phenotype_start = self.phenotype_pos_df['start'].to_dict()
+            self.phenotype_end = self.phenotype_pos_df['end'].to_dict()
         self.n_phenotypes = self.phenotype_df.shape[0]
+
         if group_s is not None:
             self.group_s = group_s.loc[self.phenotype_df.index].copy()
             self.n_groups = self.group_s.unique().shape[0]
 
 
     @background(max_prefetch=6)
     def generate_data(self, chrom=None, verbose=False):
@@ -562,7 +508,64 @@
                 # check that ranges are the same for all phenotypes within group
                 assert np.all([self.cis_ranges[g.index[0]][0] == self.cis_ranges[i][0] and self.cis_ranges[g.index[0]][1] == self.cis_ranges[i][1] for i in g.index[1:]])
                 group_phenotype_ids = g.index.tolist()
                 # p = self.phenotype_df.loc[group_phenotype_ids].values
                 p = self.phenotype_df.values[[index_dict[i] for i in group_phenotype_ids]]
                 r = self.cis_ranges[g.index[0]]
                 yield p, self.genotype_df.values[r[0]:r[-1]+1], np.arange(r[0],r[-1]+1), group_phenotype_ids, group_id
+
+
+def get_chunk_size(memory_gb, samples):
+    """"""
+    return memory_gb * 1024**3 // samples
+
+
+def generate_paired_chunks(pgr, phenotype_df, phenotype_pos_df, chunk_size, window=1000000,
+                           dosages=False, verbose=True):
+    """
+    Generate paired genotype-phenotype chunks for large datasets where only a subset of
+    genotypes can be loaded into memory.
+
+    pgr: pgen.PgenReader
+    phenotype_df:     phenotype DataFrame (phenotypes x samples)
+    phenotype_pos_df: DataFrame defining position of each phenotype, with columns ['chr', 'pos'] or ['chr', 'start', 'end']
+    chunk_size: maximum number of variants to load into CPU memory
+    window: cis-window
+    dosages: load dosages (DS) from genotype files (default: GT)
+    """
+    variant_df = pgr.pvar_df.set_index('id')[['chrom', 'pos']]
+    cis_ranges, _ = get_cis_ranges(phenotype_pos_df, pgr.variant_dfs, window)
+    range_df = pd.DataFrame(cis_ranges, index=['start', 'end']).T
+    range_df = range_df.join(phenotype_pos_df['chr'])
+
+    if chunk_size == 'chr':
+        chrlen_s = range_df['chr'].value_counts(sort=False)
+        start_ixs = [0] + chrlen_s.cumsum().tolist()
+    else:
+        chunk_size = int(chunk_size)
+        # check chunk size
+        max_cis_var = (range_df['end'] - range_df['start'] + 1).max()
+        if not max_cis_var <= chunk_size:
+            raise ValueError(f"Max. chunk size must be at least largest cis-window ({max_cis_var})")
+
+        start_ixs = [0]
+        while start_ixs[-1] < range_df.shape[0]:
+            end_ix = bisect.bisect_left(range_df['end'].values, range_df['start'].values[start_ixs[-1]] + chunk_size)
+            start_ixs.append(end_ix)
+        start_ixs[-1] = range_df.shape[0]
+
+    nchunks = len(start_ixs) - 1
+    for ci in range(nchunks):
+        if verbose:
+            print(f"Processing genotype-phenotype chunk {ci+1}/{nchunks}")
+        ix = slice(start_ixs[ci], start_ixs[ci+1])
+        chunk_df = range_df[ix]
+        if chunk_size == 'chr':
+            assert (chunk_df['chr'] == chrlen_s.index[ci]).all()
+        if dosages:
+            gt_df = pgr.read_dosages_range(chunk_df['start'].values[0], chunk_df['end'].values[-1], dtype=np.float32)
+        else:
+            gt_df = pgr.read_range(chunk_df['start'].values[0], chunk_df['end'].values[-1], impute_mean=False, dtype=np.int8)
+            # temporary workaround
+            gt_df.values[gt_df.values == -9] = -1
+        var_df = variant_df.iloc[chunk_df['start'].values[0]:chunk_df['end'].values[-1]+1]
+        yield gt_df, var_df, phenotype_df[ix], phenotype_pos_df[ix], ci
```

### Comparing `tensorqtl-1.0.7/tensorqtl/post.py` & `tensorqtl-1.0.8/tensorqtl/post.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,154 +11,63 @@
 sys.path.insert(1, os.path.dirname(__file__))
 from core import SimpleLogger, Residualizer, center_normalize, impute_mean, get_allele_stats
 import mixqtl
 import qtl.genotype as gt
 
 
 has_rpy2 = False
-e = subprocess.call('which R', shell=True, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
 try:
+    subprocess.check_call('which R', shell=True, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
+    subprocess.check_call("R -e 'library(qvalue)'", shell=True, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
     import rpy2
     import rfunc
-    if e == 0:
-        has_rpy2 = True
+    has_rpy2 = True
 except:
-    pass
-if not has_rpy2:
-    print("Warning: 'rfunc' cannot be imported. R and the 'rpy2' Python package are needed.")
+    print("Warning: 'rfunc' cannot be imported. R with the 'qvalue' library, and the 'rpy2' Python package are needed.")
 
 
 def calculate_qvalues(res_df, fdr=0.05, qvalue_lambda=None, logger=None):
     """Annotate permutation results with q-values, p-value threshold"""
     if logger is None:
         logger = SimpleLogger()
 
     logger.write('Computing q-values')
     logger.write(f'  * Number of phenotypes tested: {res_df.shape[0]}')
-    r = stats.pearsonr(res_df['pval_perm'], res_df['pval_beta'])[0]
-    logger.write(f'  * Correlation between Beta-approximated and empirical p-values: {r:.4f}')
 
-    # calculate q-values
-    if qvalue_lambda is None:
-        qval, pi0 = rfunc.qvalue(res_df['pval_beta'])
+    if not res_df['pval_beta'].isnull().all():
+        pval_col = 'pval_beta'
+        r = stats.pearsonr(res_df['pval_perm'], res_df['pval_beta'])[0]
+        logger.write(f'  * Correlation between Beta-approximated and empirical p-values: {r:.4f}')
     else:
+        pval_col = 'pval_perm'
+        logger.write(f'  * WARNING: no beta-approximated p-values found, using permutation p-values instead.')
+
+    # calculate q-values
+    if qvalue_lambda is not None:
         logger.write(f'  * Calculating q-values with lambda = {qvalue_lambda:.3f}')
-        qval, pi0 = rfunc.qvalue(res_df['pval_beta'], qvalue_lambda)
+    qval, pi0 = rfunc.qvalue(res_df[pval_col], lambda_qvalue=qvalue_lambda)
+
     res_df['qval'] = qval
     logger.write(f'  * Proportion of significant phenotypes (1-pi0): {1-pi0:.2f}')
     logger.write(f"  * QTL phenotypes @ FDR {fdr:.2f}: {(res_df['qval'] <= fdr).sum()}")
 
     # determine global min(p) significance threshold and calculate nominal p-value threshold for each gene
-    lb = res_df.loc[res_df['qval'] <= fdr, 'pval_beta'].sort_values()
-    ub = res_df.loc[res_df['qval'] > fdr, 'pval_beta'].sort_values()
-
-    if lb.shape[0] > 0:  # significant phenotypes
-        lb = lb[-1]
-        if ub.shape[0] > 0:
-            ub = ub[0]
-            pthreshold = (lb+ub)/2
-        else:
-            pthreshold = lb
-        logger.write(f'  * min p-value threshold @ FDR {fdr}: {pthreshold:.6g}')
-        res_df['pval_nominal_threshold'] = stats.beta.ppf(pthreshold, res_df['beta_shape1'], res_df['beta_shape2'])
-
-
-# ## modified by Yanyu Liang
-# def trc_calc(genotypes_t, log_counts_t, raw_counts_t, covariates0_t,
-#              count_threshold=100, select_covariates=True):
-#     mask_t = raw_counts_t >= count_threshold
-#     mask_cov = raw_counts_t != 0
-#
-#     if select_covariates:
-#         covariates_t = select_covariates(covariates0_t[mask_cov], log_counts_t[mask_cov])
-#         # b_t, b_se_t = linreg_robust(covariates0_t[mask_cov, :], log_counts_t[mask_cov])
-#         # tstat_t = b_t / b_se_t
-#         # m = tstat_t.abs() > 2
-#         # m[0] = True
-#         # covariates_t = covariates0_t[:, m]
-#     else:
-#         covariates_t = covariates0_t
-#
-#     M = torch.unsqueeze(mask_t, 1).float()
-#     M_cov = torch.unsqueeze(mask_cov, 1).float()
-#     Y = log_counts_t.reshape(1,-1).T
-#     Y[M_cov == False] = 0
-#     if covariates_t.shape[1] != 0:
-#         Y[M_cov == True] = regress_out(covariates_t[mask_cov, :], log_counts_t[mask_cov])
-#     res = wrapper_nominal_algo1_matrixLS(Y, genotypes_t.T / 2, M, numpy = False)
-#     dof = M.sum() - 2
-#     return res, int(mask_t.sum()), dof
-#
-#
-#
-#
-#
-# def trc_calc2(genotypes_t, log_counts_t, raw_counts_t, covariates0_t,
-#              count_threshold=100, select_covariates=True):
-#     """
-#     Inputs:
-#       genotypes_t:  genotype dosages (variants x samples)
-#       log_counts_t: log-transformed, normalized counts (e.g., log(counts/size_factors))
-#       # log_counts_t: log(counts/(2*libsize)) --> TODO: use better normalization. CPM/TMM vs size factors?
-#       # log_counts_t: log(counts/(2*libsize)) --> TODO: use size factor normalized counts instead
-#       raw_counts_t: raw RNA-seq counts
-#       covariates0_t: covariates matrix (samples x covariates)
-#                      including genotype PCs, PEER factors, etc.
-#                      ***with intercept in first column***
-#       count_threshold: minimum read count to include a sample
-#     """
-#     # only use samples that pass count threshold
-#
-# ## modified by Yanyu Liang
-#
-#     mask_t = raw_counts_t >= count_threshold
-#     mask_cov = raw_counts_t != 0
-#
-#     if select_covariates:
-#         b_t, b_se_t = linreg_robust(covariates0_t[mask_cov, :], log_counts_t[mask_cov])
-#         tstat_t = b_t / b_se_t
-#         m = tstat_t.abs() > 2
-#         m[0] = True
-#         covariates_t = covariates0_t[:, m]
-#     else:
-#         covariates_t = covariates0_t
-#
-#     M = torch.unsqueeze(mask_t, 1).float()
-#     M_cov = torch.unsqueeze(mask_cov, 1).float()
-#     Y = log_counts_t.reshape(1,-1).T
-#     Y[M_cov == False] = 0
-#     if covariates_t.shape[1] != 0:
-#         Y[M_cov == True] = regress_out(covariates_t[mask_cov, :], log_counts_t[mask_cov])
-#     res = wrapper_nominal_algo1_matrixLS(Y, genotypes_t.T / 2, M, numpy = False)
-#     dof = M.sum() - 2
-#     return res, int(mask_t.sum()), dof
-#
-#     # my version
-#
-#     # mask_t = raw_counts_t >= count_threshold
-#     # if select_covariates:
-#     #     covariates_t = filter_covariates(covariates0_t[mask_t], log_counts_t[mask_t])
-#     # else:
-#     #     covariates_t = covariates0_t[mask_t, 1:]
-#     #
-#     # residualizer = tensorqtl.Residualizer(covariates_t)
-#     # res = cis.calculate_cis_nominal(genotypes_t[:, mask_t] / 2, log_counts_t[mask_t].reshape(1,-1), residualizer)
-#     # # [tstat, beta, beta_se, maf, ma_samples, ma_count], samples, dof
-#     # return res, covariates_t.shape[0], residualizer.dof
-#
-#     if select_covariates:
-#         covariates_t = filter_covariates(covariates0_t, log_counts_t)
-#     else:
-#         covariates_t = covariates0_t[:, 1:]
-#
-#     mask_t = raw_counts_t >= count_threshold
-#     residualizer = tensorqtl.Residualizer(covariates_t[mask_t])
-#     res = cis.calculate_cis_nominal(genotypes_t[:, mask_t] / 2, log_counts_t[mask_t].reshape(1,-1), residualizer, return)
-#     # [tstat, beta, beta_se, maf, ma_samples, ma_count], samples
-#     return res, int(mask_t.sum()), residualizer.dof
+    if pval_col == 'pval_beta':
+        lb = res_df.loc[res_df['qval'] <= fdr, 'pval_beta'].sort_values()
+        ub = res_df.loc[res_df['qval'] > fdr, 'pval_beta'].sort_values()
+
+        if lb.shape[0] > 0:  # significant phenotypes
+            lb = lb[-1]
+            if ub.shape[0] > 0:
+                ub = ub[0]
+                pthreshold = (lb+ub)/2
+            else:
+                pthreshold = lb
+            logger.write(f'  * min p-value threshold @ FDR {fdr}: {pthreshold:.6g}')
+            res_df['pval_nominal_threshold'] = stats.beta.ppf(pthreshold, res_df['beta_shape1'], res_df['beta_shape2'])
 
 
 def calculate_afc(assoc_df, counts_df, genotype_df, variant_df=None, covariates_df=None,
                   select_covariates=True, group='gene_id',
                   imputation='offset', count_threshold=0, verbose=True):
     """
     Calculate allelic fold-change (aFC) for variant-gene pairs
@@ -214,54 +123,90 @@
         except:
             print(f'WARNING: aFC calculation failed for {phenotype_id}')
     afc_df = pd.concat(afc_df)
 
     return afc_df
 
 
-def calculate_replication(res_df, genotype_df, phenotype_df, covariates_df, interaction_s=None,
-                          compute_pi1=False, lambda_qvalue=None):
+def calculate_replication(res_df, genotype_df, phenotype_df, covariates_df=None, paired_covariate_df=None,
+                          interaction_s=None, compute_pi1=False, lambda_qvalue=None):
     """res_df: DataFrame with 'variant_id' column and phenotype IDs as index"""
     device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
 
+    if paired_covariate_df is not None:
+        assert paired_covariate_df.index.equals(covariates_df.index)
+        assert paired_covariate_df.columns.isin(phenotype_df.index).all()
+
     genotypes_t = torch.tensor(genotype_df.loc[res_df['variant_id']].values, dtype=torch.float).to(device)
     genotype_ix = np.array([genotype_df.columns.tolist().index(i) for i in phenotype_df.columns])
     genotype_ix_t = torch.from_numpy(genotype_ix).to(device)
     genotypes_t = genotypes_t[:,genotype_ix_t]
     impute_mean(genotypes_t)
+    af_t, ma_samples_t, ma_count_t = get_allele_stats(genotypes_t)
 
     phenotypes_t = torch.tensor(phenotype_df.loc[res_df.index].values, dtype=torch.float32).to(device)
-    residualizer = Residualizer(torch.tensor(covariates_df.values, dtype=torch.float32).to(device))
-    af_t, ma_samples_t, ma_count_t = get_allele_stats(genotypes_t)
+
+
+    if covariates_df is not None:
+        residualizer = Residualizer(torch.tensor(covariates_df.values, dtype=torch.float32).to(device))
+        # dof -= covariates_df.shape[1]
+    else:
+        residualizer = None
 
     if interaction_s is None:
-        genotype_res_t = residualizer.transform(genotypes_t)  # variants x samples
-        phenotype_res_t = residualizer.transform(phenotypes_t)  # phenotypes x samples
+        if paired_covariate_df is None:
+            if residualizer is not None:
+                genotype_res_t = residualizer.transform(genotypes_t)  # variants x samples
+                phenotype_res_t = residualizer.transform(phenotypes_t)  # phenotypes x samples
+                dof = residualizer.dof
+                dof_t = dof
+            else:
+                genotype_res_t = genotypes_t
+                phenotype_res_t = phenotypes_t
+                dof =  phenotypes_t.shape[1] - 2
+                dof_t = dof
+        else:
+            genotype_res_t = torch.zeros_like(genotypes_t).to(device)
+            phenotype_res_t = torch.zeros_like(phenotypes_t).to(device)
+            dof = []
+            for k,phenotype_id in enumerate(res_df.index):
+                if phenotype_id in paired_covariate_df:
+                    iresidualizer = Residualizer(torch.tensor(np.c_[covariates_df, paired_covariate_df[phenotype_id]],
+                                                              dtype=torch.float32).to(device))
+                else:
+                    iresidualizer = residualizer
+                genotype_res_t[[k]] = iresidualizer.transform(genotypes_t[[k]])
+                phenotype_res_t[[k]] = iresidualizer.transform(phenotypes_t[[k]])
+                dof.append(iresidualizer.dof)
+            dof = np.array(dof)
+            dof_t = torch.Tensor(dof).to(device)
 
         gstd = genotype_res_t.var(1)
         pstd = phenotype_res_t.var(1)
         std_ratio_t = torch.sqrt(pstd / gstd)
 
         # center and normalize
         genotype_res_t = center_normalize(genotype_res_t, dim=1)
         phenotype_res_t = center_normalize(phenotype_res_t, dim=1)
 
         r_nominal_t = (genotype_res_t * phenotype_res_t).sum(1)
         r2_nominal_t = r_nominal_t.double().pow(2)
 
-        dof = residualizer.dof
-        tstat_t = torch.sqrt((dof * r2_nominal_t) / (1 - r2_nominal_t))
+        tstat_t = torch.sqrt((dof_t * r2_nominal_t) / (1 - r2_nominal_t))
         slope_t = r_nominal_t * std_ratio_t
         slope_se_t = (slope_t.abs().double() / tstat_t).float()
         pval = 2*stats.t.cdf(-np.abs(tstat_t.cpu()), dof)
 
         rep_df = pd.DataFrame(np.c_[res_df.index, res_df['variant_id'], ma_samples_t.cpu(), ma_count_t.cpu(), af_t.cpu(), pval, slope_t.cpu(), slope_se_t.cpu()],
                               columns=['phenotype_id', 'variant_id', 'ma_samples', 'ma_count', 'af', 'pval_nominal', 'slope', 'slope_se']).infer_objects()
 
     else:
+        if paired_covariate_df is not None:
+            raise NotImplementedError("Paired covariates are not yet supported for interactions")
+
         interaction_t = torch.tensor(interaction_s.values.reshape(1,-1), dtype=torch.float32).to(device)
         ng, ns = genotypes_t.shape
         nps = phenotypes_t.shape[0]
 
         # centered inputs
         g0_t = genotypes_t - genotypes_t.mean(1, keepdim=True)
         gi_t = genotypes_t * interaction_t
@@ -315,15 +260,15 @@
     """
     gene_dict = {}
     print('['+datetime.now().strftime("%b %d %H:%M:%S")+'] Adding gene and variant annotations', flush=True)
     print('  * parsing GTF', flush=True)
     with open(annotation_gtf) as gtf:
         for row in gtf:
             row = row.strip().split('\t')
-            if row[0][0]=='#' or row[2]!='gene': continue
+            if row[0][0] == '#' or row[2] != 'gene': continue
             # get gene_id and gene_name from attributes
             attr = dict([i.split() for i in row[8].replace('"','').split(';') if i!=''])
             # gene_name, gene_chr, gene_start, gene_end, strand
             gene_dict[attr['gene_id']] = [attr['gene_name'], row[0], row[3], row[4], row[6]]
 
     print('  * annotating genes', flush=True)
     if 'group_id' in gene_df:
@@ -331,18 +276,22 @@
                                  columns=['gene_name', 'gene_chr', 'gene_start', 'gene_end', 'strand'],
                                  index=gene_df.index)
     else:
         gene_info = pd.DataFrame(data=[gene_dict[i] for i in gene_df.index],
                                  columns=['gene_name', 'gene_chr', 'gene_start', 'gene_end', 'strand'],
                                  index=gene_df.index)
     gene_df = pd.concat([gene_info, gene_df], axis=1)
-    assert np.all(gene_df.index==gene_info.index)
+    assert np.all(gene_df.index == gene_info.index)
 
     col_order = ['gene_name', 'gene_chr', 'gene_start', 'gene_end', 'strand',
-        'num_var', 'beta_shape1', 'beta_shape2', 'true_df', 'pval_true_df', 'variant_id', 'tss_distance']
+        'num_var', 'beta_shape1', 'beta_shape2', 'true_df', 'pval_true_df', 'variant_id']
+    if 'tss_distance' in gene_df:
+        col_order += ['tss_distance']
+    else:
+        col_order += ['start_distance', 'end_distance']
     if lookup_df is not None:
         print('  * adding variant annotations from lookup table', flush=True)
         gene_df = gene_df.join(lookup_df, on='variant_id')  # add variant information
         col_order += list(lookup_df.columns)
     col_order += ['ma_samples', 'ma_count', 'af', 'pval_nominal',
                   'slope', 'slope_se', 'pval_perm', 'pval_beta']
     if 'group_id' in gene_df:
@@ -375,14 +324,15 @@
         assert isinstance(nominal_files, dict)
 
     chroms = sorted(nominal_files.keys(), key=lambda x: int(x.replace('chr', '').replace('X', '23')))
     signif_df = []
     for k,c in enumerate(chroms, 1):
         print(f'  * processing chr. {k}/{len(chroms)}', end='\r', flush=True)
         nominal_df = pd.read_parquet(nominal_files[c])
+        # drop pairs that never pass threshold
         nominal_df = nominal_df[nominal_df['pval_nominal'] <= df['pval_nominal_threshold'].max()]
         if group_s is not None:
             nominal_df.insert(1, 'group_id', nominal_df['phenotype_id'].map(group_s))
             nominal_df = nominal_df[nominal_df['group_id'].isin(signif_phenotype_ids)]
             m = nominal_df['pval_nominal'] < nominal_df['group_id'].apply(lambda x: threshold_dict[x])
         else:
             nominal_df = nominal_df[nominal_df['phenotype_id'].isin(signif_phenotype_ids)]
```

### Comparing `tensorqtl-1.0.7/tensorqtl/rfunc.py` & `tensorqtl-1.0.8/tensorqtl/rfunc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Author: Francois Aguet
 import numpy as np
 import rpy2
 from rpy2.robjects.packages import importr
-from collections import Iterable
+from collections.abc import Iterable
 from contextlib import contextmanager
 
 # silence R warnings
 from rpy2.rinterface_lib.callbacks import logger as rpy2_logger
 import logging
 rpy2_logger.setLevel(logging.ERROR)
```

### Comparing `tensorqtl-1.0.7/tensorqtl/susie.py` & `tensorqtl-1.0.8/tensorqtl/susie.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,15 @@
     s = {
         'alpha': torch.full((L,p), 1/p).to(device),
         'mu': torch.zeros((L,p)).to(device),
         'mu2': torch.zeros((L,p)).to(device),
         'Xr': torch.zeros(n).to(device),
         'KL': torch.full([L], np.NaN).to(device),
         'lbf': torch.full([L], np.NaN).to(device),
+        'lbf_variable': torch.full([L, p], np.NaN).to(device),
         'sigma2': residual_variance,
         'V': scaled_prior_variance * varY,
         'pi': prior_weights,
     }
     if null_weight is None:
         s['null_index'] = 0
     else:
@@ -164,15 +165,15 @@
     """"""
     # EM solution
     V = (alpha * post_mean2).sum()
 
     # set V exactly 0 if that beats the numerical value
     # by check_null_threshold in loglik.
     # check_null_threshold = 0.1 is exp(0.1) = 1.1 on likelihood scale;
-    # it means that for parsimony reasons we set estiate of V to zero, if its
+    # it means that for parsimony reasons we set estimate of V to zero, if its
     # numerical estimate is only "negligibly" different from zero. We use a likelihood
     # ratio of exp(check_null_threshold) to define "negligible" in this context.
     # This is fairly modest condition compared to, say, a formal LRT with p-value 0.05.
     # But the idea is to be lenient to non-zeros estimates unless they are indeed small enough
     # to be neglible.
     # See more intuition at https://stephens999.github.io/fiveMinuteStats/LR_and_BF.html
     if loglik(0, betahat, shat2, prior_weights) + check_null_threshold >= loglik(V, betahat, shat2, prior_weights):
@@ -272,14 +273,15 @@
 
         # update the variational estimate of the posterior mean
         s['mu'][l] = res['mu']
         s['alpha'][l] = res['alpha']
         s['mu2'][l] = res['mu2']
         s['V'][l] = res['V']
         s['lbf'][l] = res['lbf_model']
+        s['lbf_variable'][l] = res['lbf']
         s['KL'][l] = -res['loglik'] + SER_posterior_e_loglik(X_t, xattr, R_t, s['sigma2'], res['alpha']*res['mu'], res['alpha']*res['mu2'])
         s['Xr'] = s['Xr'] + compute_Xb(X_t, (s['alpha'][l,:] * s['mu'][l,:]), xattr['scaled_center'], xattr['scaled_scale'])
     return(s)
 
 
 def get_objective(X_t, xattr, Y_t, s):
     """Get objective function from data and susie fit object"""
@@ -484,15 +486,15 @@
         y_t = y_t - mean_y
 
     xattr = get_x_attributes(X_t, center=intercept, scale=standardize)
 
     # initialize susie fit
     s = init_setup(n, p, L, scaled_prior_variance, y_t.var(unbiased=True),
                    residual_variance=residual_variance,
-                   prior_weights=prior_weights, null_weight=null_weight)  # , standardize <-- never used?
+                   prior_weights=prior_weights, null_weight=null_weight)
     s = init_finalize(s)
 
     # initialize elbo to NA
     elbo = torch.full([max_iter + 1], np.NaN).to(device)
     elbo[0] = -np.Inf;
     tracking = []
     for i in range(1, max_iter+1):
@@ -511,15 +513,15 @@
         if estimate_residual_variance:
             s['sigma2'] = estimate_residual_variance_fct(X_t, xattr, y_t, s)
             if s['sigma2'] > residual_variance_upperbound:
                 s['sigma2'] = residual_variance_upperbound
             if verbose:
                 print(f'Objective (iter {i}): {get_objective(X_t, xattr, y_t, s)}')
 
-    s['elbo'] = elbo[1:i+1]  # Remove first (infinite) entry, and trailing NAs.
+    s['elbo'] = elbo[1:i+1].cpu().numpy()  # Remove first (infinite) entry, and trailing NAs.
     s['niter'] = i
 
     if 'converged' not in s:
         print(f"\n    WARNING: IBSS algorithm did not converge in {max_iter} iterations!")
         s['converged'] = False
 
     if intercept:
@@ -529,67 +531,74 @@
         s['intercept'] = 0
         s['fitted'] = s['Xr']
 
     s['fitted'] = s['fitted'].squeeze()
     # if track_fit:
     #     s['trace'] = tracking
 
+    s['lbf_variable'] = s['lbf_variable'].cpu().numpy()
+
     # SuSiE CS and PIP
     if coverage is not None and min_abs_corr is not None:
         s['sets'] = susie_get_cs(s, coverage=coverage, X=X_t, min_abs_corr=min_abs_corr)
         s['pip'] = susie_get_pip(s, prune_by_cs=False, prior_tol=prior_tol).cpu().numpy()
 
     return s
 
 
 def map(genotype_df, variant_df, phenotype_df, phenotype_pos_df, covariates_df,
-        L=10, scaled_prior_variance=0.2, estimate_residual_variance=True,
-        estimate_prior_variance=True, tol=1e-3,
-        coverage=0.95, min_abs_corr=0.5, summary_only=True, maf_threshold=0,
-        max_iter=100, window=1000000, logger=None, verbose=True, warn_monomorphic=False):
+        paired_covariate_df=None, L=10, scaled_prior_variance=0.2, estimate_residual_variance=True,
+        estimate_prior_variance=True, tol=1e-3, coverage=0.95, min_abs_corr=0.5,
+        summary_only=True, maf_threshold=0, max_iter=100, window=1000000,
+        logger=None, verbose=True, warn_monomorphic=False):
     """
     SuSiE fine-mapping: computes SuSiE model for all phenotypes
     """
-    assert np.all(phenotype_df.columns==covariates_df.index)
+    assert phenotype_df.columns.equals(covariates_df.index)
     device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
 
     if logger is None:
         logger = SimpleLogger()
 
     logger.write('SuSiE fine-mapping')
     logger.write(f'  * {phenotype_df.shape[1]} samples')
     logger.write(f'  * {phenotype_df.shape[0]} phenotypes')
     logger.write(f'  * {covariates_df.shape[1]} covariates')
+    if paired_covariate_df is not None:
+        assert covariates_df is not None
+        assert paired_covariate_df.columns.equals(phenotype_df.columns), f"Paired covariate samples must match samples in phenotype matrix."
+        paired_covariate_df = paired_covariate_df.T  # samples x phenotypes
+        logger.write(f'  * including phenotype-specific covariate')
     logger.write(f'  * {variant_df.shape[0]} variants')
+    logger.write(f'  * cis-window: ±{window:,}')
     if maf_threshold > 0:
         logger.write(f'  * applying in-sample MAF >= {maf_threshold} filter')
 
     residualizer = Residualizer(torch.tensor(covariates_df.values, dtype=torch.float32).to(device))
 
     genotype_ix = np.array([genotype_df.columns.tolist().index(i) for i in phenotype_df.columns])
     genotype_ix_t = torch.from_numpy(genotype_ix).to(device)
 
     igc = genotypeio.InputGeneratorCis(genotype_df, variant_df, phenotype_df, phenotype_pos_df, window=window)
     if igc.n_phenotypes == 0:
         raise ValueError('No valid phenotypes found.')
 
     start_time = time.time()
     logger.write('  * fine-mapping')
-    copy_keys = ['pip', 'sets', 'converged', 'niter']
+    copy_keys = ['pip', 'sets', 'converged', 'elbo', 'niter', 'lbf_variable']
+    susie_summary = []
     if not summary_only:
         susie_res = {}
-    else:
-        susie_res = []
     for k, (phenotype, genotypes, genotype_range, phenotype_id) in enumerate(igc.generate_data(verbose=verbose), 1):
         # copy genotypes to GPU
         genotypes_t = torch.tensor(genotypes, dtype=torch.float).to(device)
         genotypes_t = genotypes_t[:,genotype_ix_t]
         impute_mean(genotypes_t)
 
-        variant_ids = variant_df.index[genotype_range[0]:genotype_range[-1]+1]
+        variant_ids = variant_df.index[genotype_range[0]:genotype_range[-1]+1].rename('variant_id')
 
         # filter monomorphic variants
         mask_t = ~(genotypes_t == genotypes_t[:, [0]]).all(1)
         if warn_monomorphic:
             logger.write(f'    * WARNING: excluding {~mask_t.sum()} monomorphic variants')
         if maf_threshold > 0:
             maf_t = calculate_maf(genotypes_t)
@@ -600,47 +609,59 @@
             variant_ids = variant_ids[mask]
             genotype_range = genotype_range[mask]
 
         if genotypes_t.shape[0] == 0:
             logger.write(f'WARNING: skipping {phenotype_id} (no valid variants)')
             continue
 
+        if paired_covariate_df is None or phenotype_id not in paired_covariate_df:
+            iresidualizer = residualizer
+        else:
+            iresidualizer = Residualizer(torch.tensor(np.c_[covariates_df, paired_covariate_df[phenotype_id]],
+                                                      dtype=torch.float32).to(device))
+
         phenotype_t = torch.tensor(phenotype, dtype=torch.float).to(device)
-        genotypes_res_t = residualizer.transform(genotypes_t)  # variants x samples
-        phenotype_res_t = residualizer.transform(phenotype_t.reshape(1,-1))  # phenotypes x samples
+        genotypes_res_t = iresidualizer.transform(genotypes_t)  # variants x samples
+        phenotype_res_t = iresidualizer.transform(phenotype_t.reshape(1,-1))  # phenotypes x samples
 
         res = susie(genotypes_res_t.T, phenotype_res_t.T, L=L,
                     scaled_prior_variance=scaled_prior_variance,
                     coverage=coverage, min_abs_corr=min_abs_corr,
                     estimate_residual_variance=estimate_residual_variance,
                     estimate_prior_variance=estimate_prior_variance,
                     tol=tol, max_iter=max_iter)
 
         af_t = genotypes_t.sum(1) / (2 * genotypes_t.shape[1])
         res['pip'] = pd.DataFrame({'pip':res['pip'], 'af':af_t.cpu().numpy()}, index=variant_ids)
-        if not summary_only:
+        if res['sets']['cs'] is not None:
+            if res['converged'] == True:
+                for c in sorted(res['sets']['cs'], key=lambda x: int(x.replace('L',''))):
+                    cs = res['sets']['cs'][c]  # indexes
+                    p = res['pip'].iloc[cs].copy().reset_index()
+                    p['cs_id'] = c.replace('L','')
+                    p.insert(0, 'phenotype_id', phenotype_id)
+                    susie_summary.append(p)
+                res['lbf_variable'] = res['lbf_variable'][res['sets']['cs_index']]  # drop zero entries
+            else:
+                print(f'    * phenotype ID: {phenotype_id}')
+
+        if not summary_only:  # keep full results
             susie_res[phenotype_id] = {k:res[k] for k in copy_keys}
-        else:
-            if res['sets']['cs'] is not None:
-                # assert res['converged'] == True
-                if res['converged'] == True:
-                    for c in sorted(res['sets']['cs'], key=lambda x: int(x.replace('L',''))):
-                        cs = res['sets']['cs'][c]  # indexes
-                        p = res['pip'].iloc[cs].copy().reset_index()
-                        p['cs_id'] = c.replace('L','')
-                        p.insert(0, 'phenotype_id', phenotype_id)
-                        susie_res.append(p)
-                else:
-                    print(f'    * phenotype ID: {phenotype_id}')
 
     logger.write(f'  Time elapsed: {(time.time()-start_time)/60:.2f} min')
     logger.write('done.')
-    if summary_only and susie_res:
-        susie_res = pd.concat(susie_res, axis=0).rename(columns={'snp':'variant_id'}).reset_index(drop=True)
-    return susie_res
+    if susie_summary:
+        susie_summary = pd.concat(susie_summary, axis=0).rename(columns={'snp': 'variant_id'}).reset_index(drop=True)
+    if summary_only:
+        return susie_summary
+    else:
+        drop_ids = [k for k in susie_res if susie_res[k]['sets']['cs'] is None]
+        for k in drop_ids:
+            del susie_res[k]
+        return susie_summary, susie_res
 
 
 def get_summary(res_dict, verbose=True):
     """
 
       res_dict: gene_id -> SuSiE results
     """
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `tensorqtl-1.0.7/tensorqtl/trans.py` & `tensorqtl-1.0.8/tensorqtl/trans.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,42 +9,47 @@
 import time
 
 sys.path.insert(1, os.path.dirname(__file__))
 import genotypeio
 from core import *
 
 
-def _in_cis(chrom, pos, gene_id, tss_dict, window=1000000):
+def _in_cis(chrom, pos, gene_id, pos_dict, window=1000000):
     """Test if a variant is within +/-window of a gene's TSS."""
-    if chrom == tss_dict[gene_id]['chr']:
-        tss = tss_dict[gene_id]['tss']
-        if pos >= tss - window and pos <= tss + window:
+    if chrom == pos_dict[gene_id]['chr']:
+        gene_dict = pos_dict[gene_id]
+        if 'pos' in gene_dict:
+            start = gene_dict['pos']
+            end = start
+        else:
+            start = gene_dict['start']
+            end = gene_dict['end']
+        if pos >= start - window and pos <= end + window:
             return True
         else:
             return False
     else:
         return False
 
 
-def filter_cis(pairs_df, tss_dict, variant_df, window=5000000):
+def filter_cis(pairs_df, phenotype_pos_df, variant_df, window=5000000):
     """Filter out cis-QTLs
 
     Args:
         pairs_df: sparse output from map_trans()
-        tss_dict: gene_id->tss
-        window: filter variants within +/-window of TSS
+        pos_dict: phenotype_id -> pos
+        window: filter variants within +/-window of feature position (e.g., TSS for genes)
     """
+    pos_dict = phenotype_pos_df.T.to_dict()
     variant_df = variant_df.loc[pairs_df['variant_id'].unique()].copy()
-    variant_dict = {}
-    for variant_id, chrom, pos in zip(variant_df.index, variant_df['chrom'], variant_df['pos']):
-        variant_dict[variant_id] = {'chrom':chrom, 'pos':pos}
+    variant_dict = {v:{'chrom':c, 'pos':p} for v,c,p in zip(variant_df.index, variant_df['chrom'], variant_df['pos'])}
 
     drop_ix = []
     for k,gene_id,variant_id in zip(pairs_df['phenotype_id'].index, pairs_df['phenotype_id'], pairs_df['variant_id']):
-        if _in_cis(variant_dict[variant_id]['chrom'], variant_dict[variant_id]['pos'], gene_id, tss_dict, window=window):
+        if _in_cis(variant_dict[variant_id]['chrom'], variant_dict[variant_id]['pos'], gene_id, pos_dict, window=window):
             drop_ix.append(k)
     return pairs_df.drop(drop_ix)
 
 
 def map_trans(genotype_df, phenotype_df, covariates_df=None, interaction_s=None,
               return_sparse=True, pval_threshold=1e-5, maf_threshold=0.05,
               alleles=2, return_r2=False, batch_size=20000,
@@ -352,16 +357,19 @@
 
         chr_max_r2 = OrderedDict()
         k = 0
         for chrom in ggt.chroms:
             max_r2_t = torch.FloatTensor(nperms).fill_(0).to(device)
             for k, (genotypes, variant_ids) in enumerate(ggt.generate_data(chrom=chrom, verbose=verbose, enum_start=k+1), k+1):
                 genotypes_t = torch.tensor(genotypes, dtype=torch.float).to(device)
-                genotypes_t, _, _ = filter_maf(genotypes_t[:, genotype_ix_t], variant_ids, maf_threshold)
+                genotypes_t = genotypes_t[:, genotype_ix_t]
+                impute_mean(genotypes_t)
+                genotypes_t, _, _ = filter_maf(genotypes_t, variant_ids, maf_threshold)
                 n_variants += genotypes_t.shape[0]
+
                 r2_t = calculate_corr(genotypes_t, permutations_t, residualizer=residualizer).pow(2)
                 del genotypes_t
                 m,_ = r2_t.max(0)
                 max_r2_t = torch.max(m, max_r2_t)
             chr_max_r2[chrom] = max_r2_t.cpu()
         logger.write(f'    time elapsed: {(time.time()-start_time)/60:.2f} min')
         if maf_threshold > 0:
@@ -397,16 +405,19 @@
     else:  # not split_chr
         ggt = genotypeio.GenotypeGeneratorTrans(genotype_df, batch_size=batch_size)
         start_time = time.time()
         max_r2_t = torch.FloatTensor(nperms).fill_(0).to(device)
         n_variants = 0
         for k, (genotypes, variant_ids) in enumerate(ggt.generate_data(verbose=verbose), 1):
             genotypes_t = torch.tensor(genotypes, dtype=torch.float).to(device)
-            genotypes_t, _, _ = filter_maf(genotypes_t[:, genotype_ix_t], variant_ids, maf_threshold)
+            genotypes_t = genotypes_t[:, genotype_ix_t]
+            impute_mean(genotypes_t)
+            genotypes_t, _, _ = filter_maf(genotypes_t, variant_ids, maf_threshold)
             n_variants += genotypes_t.shape[0]
+
             r2_t = calculate_corr(genotypes_t, permutations_t, residualizer=residualizer).pow(2)
             del genotypes_t
             m,_ = r2_t.max(0)
             max_r2_t = torch.max(m, max_r2_t)
         logger.write(f'    time elapsed: {(time.time()-start_time)/60:.2f} min')
         if maf_threshold > 0:
             logger.write(f'  * {n_variants} variants passed MAF >= {maf_threshold:.2f} filtering')
```

### Comparing `tensorqtl-1.0.7/tensorqtl.egg-info/PKG-INFO` & `tensorqtl-1.0.8/tensorqtl.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: tensorqtl
-Version: 1.0.7
+Version: 1.0.8
 Summary: GPU-accelerated QTL mapper
 Author: Francois Aguet (Broad Institute)
 Author-email: francois@broadinstitute.org
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## tensorQTL
 
 tensorQTL is a GPU-enabled QTL mapper, achieving ~200-300 fold faster *cis*- and *trans*-QTL mapping compared to CPU-based implementations.
 
 If you use tensorQTL in your research, please cite the following paper:
-[Taylor-Weiner, Aguet, et al., *Genome Biol.* 20:228, 2019](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-019-1836-7).
+[Taylor-Weiner, Aguet, et al., *Genome Biol.*, 2019](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-019-1836-7).
 
-Empirical beta-approximated p-values are computed as described in [FastQTL](http://fastqtl.sourceforge.net/) ([Ongen et al., 2016](https://academic.oup.com/bioinformatics/article/32/10/1479/1742545)).
+Empirical beta-approximated p-values are computed as described in [Ongen et al., *Bioinformatics*, 2016](https://academic.oup.com/bioinformatics/article/32/10/1479/1742545).
 
 ### Install
 You can install tensorQTL using pip:
 ```
 pip3 install tensorqtl
 ```
 or directly from this repository:
@@ -29,14 +29,21 @@
 $ git clone git@github.com:broadinstitute/tensorqtl.git
 $ cd tensorqtl
 # set up virtual environment and install
 $ virtualenv venv
 $ source venv/bin/activate
 (venv)$ pip install -r install/requirements.txt .
 ```
+To use PLINK 2 binary files ([pgen/pvar/psam](https://www.cog-genomics.org/plink/2.0/input#pgen)), [pgenlib](https://github.com/chrchang/plink-ng/tree/master/2.0/Python) must be installed:
+```
+git clone git@github.com:chrchang/plink-ng.git
+cd plink-ng/2.0/Python/
+python3 setup.py build_ext
+python3 setup.py install
+```
 
 ### Requirements
 
 tensorQTL requires an environment configured with a GPU for optimal performance, but can also be run on a CPU. Instructions for setting up a virtual machine on Google Cloud Platform are provided [here](install/INSTALL.md).
 
 ### Input formats
 Three inputs are required for QTL analyses with tensorQTL: genotypes, phenotypes, and covariates. 
@@ -50,15 +57,15 @@
       --out ${plink_prefix_path}
   ```
   If using PLINK 1.9 or earlier, add the `--keep-allele-order` flag. 
   
   Alternatively, the genotypes can be provided as a dataframe (genotypes x samples). 
 
 
-The [examples notebook](example/tensorqtl_examples.ipynb) below contains examples of all input files. The input formats for phenotypes and covariates are identical to those used by [FastQTL](http://fastqtl.sourceforge.net/).
+The [examples notebook](example/tensorqtl_examples.ipynb) below contains examples of all input files. The input formats for phenotypes and covariates are identical to those used by [FastQTL](https://github.com/francois-a/fastqtl).
 
 ### Examples
 For examples illustrating *cis*- and *trans*-QTL mapping, please see [tensorqtl_examples.ipynb](example/tensorqtl_examples.ipynb).
 
 ### Running tensorQTL
 This section describes how to run the different modes of tensorQTL, both from the command line and within Python.
 For a full list of options, run
```

