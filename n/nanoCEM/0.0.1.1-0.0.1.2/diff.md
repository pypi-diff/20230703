# Comparing `tmp/nanoCEM-0.0.1.1.tar.gz` & `tmp/nanoCEM-0.0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nanoCEM-0.0.1.1.tar", last modified: Mon Jul  3 09:52:00 2023, max compression
+gzip compressed data, was "dist/nanoCEM-0.0.1.2.tar", last modified: Mon Jul  3 10:43:35 2023, max compression
```

## Comparing `nanoCEM-0.0.1.1.tar` & `nanoCEM-0.0.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-03 09:52:00.000064 nanoCEM-0.0.1.1/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2023-05-31 12:16:43.000000 nanoCEM-0.0.1.1/LICENSE
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     8937 2023-07-03 09:52:00.000064 nanoCEM-0.0.1.1/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     8336 2023-07-03 09:49:00.000000 nanoCEM-0.0.1.1/README.md
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-03 09:52:00.000064 nanoCEM-0.0.1.1/nanoCEM/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9323 2023-07-03 09:49:00.000000 nanoCEM-0.0.1.1/nanoCEM/CE_magnifier_test.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       56 2023-06-14 11:15:11.000000 nanoCEM-0.0.1.1/nanoCEM/__init__.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1584 2023-06-06 06:49:54.000000 nanoCEM-0.0.1.1/nanoCEM/cem_utils.py
--rwxrwxrwx   0 zhguo     (1000) zhguo     (1000)     7624 2023-07-03 09:49:00.000000 nanoCEM-0.0.1.1/nanoCEM/current_events_magnifier.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     3954 2023-07-03 09:40:02.000000 nanoCEM-0.0.1.1/nanoCEM/extract_sub_fast5_from_bam.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      893 2023-06-05 13:34:35.000000 nanoCEM-0.0.1.1/nanoCEM/normalization.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     7727 2023-06-26 15:00:04.000000 nanoCEM-0.0.1.1/nanoCEM/plot.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    10594 2023-07-03 09:49:00.000000 nanoCEM-0.0.1.1/nanoCEM/read_f5c_resquiggle.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13844 2023-07-03 09:49:00.000000 nanoCEM-0.0.1.1/nanoCEM/read_tombo_resquiggle.py
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-03 09:52:00.000064 nanoCEM-0.0.1.1/nanoCEM.egg-info/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     8937 2023-07-03 09:51:59.000000 nanoCEM-0.0.1.1/nanoCEM.egg-info/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      429 2023-07-03 09:51:59.000000 nanoCEM-0.0.1.1/nanoCEM.egg-info/SOURCES.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-07-03 09:51:59.000000 nanoCEM-0.0.1.1/nanoCEM.egg-info/dependency_links.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      121 2023-07-03 09:51:59.000000 nanoCEM-0.0.1.1/nanoCEM.egg-info/requires.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        8 2023-07-03 09:51:59.000000 nanoCEM-0.0.1.1/nanoCEM.egg-info/top_level.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2023-07-03 09:52:00.000064 nanoCEM-0.0.1.1/setup.cfg
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1152 2023-07-03 09:51:59.000000 nanoCEM-0.0.1.1/setup.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-03 10:43:35.289410 nanoCEM-0.0.1.2/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2023-05-31 12:16:43.000000 nanoCEM-0.0.1.2/LICENSE
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     8989 2023-07-03 10:43:35.289410 nanoCEM-0.0.1.2/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     8388 2023-07-03 09:59:45.000000 nanoCEM-0.0.1.2/README.md
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-03 10:43:35.289410 nanoCEM-0.0.1.2/nanoCEM/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     9415 2023-07-03 10:42:53.000000 nanoCEM-0.0.1.2/nanoCEM/CE_magnifier_test.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       56 2023-06-14 11:15:11.000000 nanoCEM-0.0.1.2/nanoCEM/__init__.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1584 2023-06-06 06:49:54.000000 nanoCEM-0.0.1.2/nanoCEM/cem_utils.py
+-rwxrwxrwx   0 zhguo     (1000) zhguo     (1000)     7691 2023-07-03 10:42:53.000000 nanoCEM-0.0.1.2/nanoCEM/current_events_magnifier.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     3954 2023-07-03 09:40:02.000000 nanoCEM-0.0.1.2/nanoCEM/extract_sub_fast5_from_bam.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      893 2023-06-05 13:34:35.000000 nanoCEM-0.0.1.2/nanoCEM/normalization.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     7727 2023-06-26 15:00:04.000000 nanoCEM-0.0.1.2/nanoCEM/plot.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    11062 2023-07-03 10:37:41.000000 nanoCEM-0.0.1.2/nanoCEM/read_f5c_resquiggle.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13844 2023-07-03 09:49:00.000000 nanoCEM-0.0.1.2/nanoCEM/read_tombo_resquiggle.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2023-07-03 10:43:35.289410 nanoCEM-0.0.1.2/nanoCEM.egg-info/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     8989 2023-07-03 10:43:35.000000 nanoCEM-0.0.1.2/nanoCEM.egg-info/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      429 2023-07-03 10:43:35.000000 nanoCEM-0.0.1.2/nanoCEM.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2023-07-03 10:43:35.000000 nanoCEM-0.0.1.2/nanoCEM.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      121 2023-07-03 10:43:35.000000 nanoCEM-0.0.1.2/nanoCEM.egg-info/requires.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        8 2023-07-03 10:43:35.000000 nanoCEM-0.0.1.2/nanoCEM.egg-info/top_level.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2023-07-03 10:43:35.289410 nanoCEM-0.0.1.2/setup.cfg
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1152 2023-07-03 10:43:27.000000 nanoCEM-0.0.1.2/setup.py
```

### Comparing `nanoCEM-0.0.1.1/LICENSE` & `nanoCEM-0.0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.1.1/PKG-INFO` & `nanoCEM-0.0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: nanoCEM
-Version: 0.0.1.1
+Version: 0.0.1.2
 Summary: A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports two re-squiggle pipeline(Tombo and f5c).
 Home-page: https://github.com/lrslab/current_events_magnifier
 Author: GUO Zhihao
 Author-email: qhuozhihao@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7,<3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # nanoCEM
-The nanopore_current_events_magnifier(`nanoCEM`) is a python command line to facilitate the analysis of DNA/RNA modification sites by visualizing statistical features of current events. 
+The nanopore current events magnifier (`nanoCEM`) is a python command line to facilitate the analysis of DNA/RNA modification sites by visualizing statistical features of current events. 
 CEM can be used to showcase high confidence sites and observe the difference based on the modification sample and the low or no modification sample.
 
 It supports two re-squiggle pipeline(`Tombo` and `f5c`) and support `R9` and `R10`.
 If you want to view single read signal or raw signal, [Squigualiser](https://github.com/hiruna72/squigualiser) is recommended.
 
 ## Example
 Here is an example that show the difference of A2030 on 23S rRNA.
@@ -49,15 +49,15 @@
 pip install nanoCEM==0.0.4.4
 pip install ont-fast5-api
 conda install -c bioconda f5c slow5tools
 ```
 ## Options
 ### read_tombo_resquiggle
 ```sh
-nanoCEM.py tombo -h
+current_events_magnifier.py tombo -h
 optional arguments:
   -h, --help            show this help message and exit
   --basecall_group BASECALL_GROUP
                         The attribute group to extract the training data from. e.g. RawGenomeCorrected_000
   --basecall_subgroup BASECALL_SUBGROUP
                         Basecall subgroup Nanoraw resquiggle into. Default is BaseCalled_template
   -i FAST5, --fast5 FAST5
@@ -74,15 +74,15 @@
   --ref REF             fasta file
   --overplot-number OVERPLOT_NUMBER (default:500)
                         Number of read will be used to plot
   --rna                 Turn on the RNA mode 
 ```
 ### read_f5c_resquiggle
 ```sh
-nanoCEM.py f5c -h
+current_events_magnifier.py f5c -h
 optional arguments:
   -h, --help            show this help message and exit
   -i INPUT, --input INPUT
                         path and suffix of blow5, bam file and paf files
   -c CONTROL, --control CONTROL
                         control path and suffix of blow5, bam file and paf files
   -o OUTPUT, --output OUTPUT
@@ -163,15 +163,15 @@
 Use ```--rna``` to turn to the rna mode and ```--pore r10``` to re-squiggle reads from R10
 ```sh
 f5c resquiggle -c all.fastq file.blow5 -o file.paf --rna --pore r9
 ```
 3. Run nanoCEM to plot
 ```sh
 # run the pipeline below for your two sample respective and keep the suffix of bam/paf/blow5 is the same
-nanoCEM.py f5c -i sample1/file -c sample2/file -o f5c_result \
+current_events_magnifier.py f5c -i sample1/file -c sample2/file -o f5c_result \
 --chrom NR_103073.1 --strand + \
 --pos 3929 --len 10 \
 --ref reference.fasta --base_shift 2 --rna
 ```
```

### Comparing `nanoCEM-0.0.1.1/README.md` & `nanoCEM-0.0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # nanoCEM
-The nanopore_current_events_magnifier(`nanoCEM`) is a python command line to facilitate the analysis of DNA/RNA modification sites by visualizing statistical features of current events. 
+The nanopore current events magnifier (`nanoCEM`) is a python command line to facilitate the analysis of DNA/RNA modification sites by visualizing statistical features of current events. 
 CEM can be used to showcase high confidence sites and observe the difference based on the modification sample and the low or no modification sample.
 
 It supports two re-squiggle pipeline(`Tombo` and `f5c`) and support `R9` and `R10`.
 If you want to view single read signal or raw signal, [Squigualiser](https://github.com/hiruna72/squigualiser) is recommended.
 
 ## Example
 Here is an example that show the difference of A2030 on 23S rRNA.
@@ -35,15 +35,15 @@
 pip install nanoCEM==0.0.4.4
 pip install ont-fast5-api
 conda install -c bioconda f5c slow5tools
 ```
 ## Options
 ### read_tombo_resquiggle
 ```sh
-nanoCEM.py tombo -h
+current_events_magnifier.py tombo -h
 optional arguments:
   -h, --help            show this help message and exit
   --basecall_group BASECALL_GROUP
                         The attribute group to extract the training data from. e.g. RawGenomeCorrected_000
   --basecall_subgroup BASECALL_SUBGROUP
                         Basecall subgroup Nanoraw resquiggle into. Default is BaseCalled_template
   -i FAST5, --fast5 FAST5
@@ -60,15 +60,15 @@
   --ref REF             fasta file
   --overplot-number OVERPLOT_NUMBER (default:500)
                         Number of read will be used to plot
   --rna                 Turn on the RNA mode 
 ```
 ### read_f5c_resquiggle
 ```sh
-nanoCEM.py f5c -h
+current_events_magnifier.py f5c -h
 optional arguments:
   -h, --help            show this help message and exit
   -i INPUT, --input INPUT
                         path and suffix of blow5, bam file and paf files
   -c CONTROL, --control CONTROL
                         control path and suffix of blow5, bam file and paf files
   -o OUTPUT, --output OUTPUT
@@ -149,15 +149,15 @@
 Use ```--rna``` to turn to the rna mode and ```--pore r10``` to re-squiggle reads from R10
 ```sh
 f5c resquiggle -c all.fastq file.blow5 -o file.paf --rna --pore r9
 ```
 3. Run nanoCEM to plot
 ```sh
 # run the pipeline below for your two sample respective and keep the suffix of bam/paf/blow5 is the same
-nanoCEM.py f5c -i sample1/file -c sample2/file -o f5c_result \
+current_events_magnifier.py f5c -i sample1/file -c sample2/file -o f5c_result \
 --chrom NR_103073.1 --strand + \
 --pos 3929 --len 10 \
 --ref reference.fasta --base_shift 2 --rna
 ```
```

### Comparing `nanoCEM-0.0.1.1/nanoCEM/CE_magnifier_test.py` & `nanoCEM-0.0.1.2/nanoCEM/CE_magnifier_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,26 +52,27 @@
     #                     basecall_group="RawGenomeCorrected_000", basecall_subgroup="BaseCalled_template",rna=False)
     # parser.set_defaults(function='tombo', chrom="NR_103073.1", pos=2030, len=10, strand='+', cpu=8,input_fast5='/data/Ecoli_23s/data/L_rep2/single/',\
     #                     control_fast5='/data/Ecoli_23s/data/IVT_negative/single/',output='tombo_result_rna',overplot_number=500,\
     #                     ref="/data/Ecoli_23s/23S_rRNA.fasta",\
     #                      basecall_group="RawGenomeCorrected_000", basecall_subgroup="BaseCalled_template",rna=True)
     parser.set_defaults(function='f5c', chrom="NR_103073.1", pos=2030, len=10, strand='+', cpu=4,input='/data/Ecoli_23s/data/L_rep2/file',\
                         control='/data/Ecoli_23s/data/IVT_negative/file',\
-                        output='f5c_result_rna',overplot_number=1000,ref="/data/Ecoli_23s/23S_rRNA.fasta",rna=True,base_shift=2)
+                        output='f5c_result_rna_new',overplot_number=1000,ref="/data/Ecoli_23s/23S_rRNA.fasta",rna=True,base_shift=2)
     # parser.set_defaults(function='f5c', chrom="1", pos=150280972, len=10, strand='+', cpu=4,input='/data/current_test_data/samp/cem_test_dna/WGS/file',\
     #                     control='/data/current_test_data/samp/cem_test_dna/WGA/file',\
-    #                     output='f5c_result_dna',overplot_number=1000,ref="/data/current_test_data/samp/cem_test_dna/hg.fa",rna=False,base_shift=2)
+    #                     output='f5c_result_dna_new',overplot_number=1000,ref="/data/current_test_data/samp/cem_test_dna/hg.fa",rna=False,base_shift=2)
 
     return parser
 
 if __name__ == '__main__':
     # Parse the arguments
     parser = init_parser()
     args = parser.parse_args()
-
+    aligned_num_wt = 0
+    aligned_num_ivt = 0
     # read reference
     subsample_num = args.overplot_number
     fasta = read_fasta_to_dic(args.ref)
     # length filter
     args.pos = args.pos - 1
     length_gene = len(fasta[args.chrom])
     if args.pos + args.len + 1 >= length_gene or args.pos - args.len <= 0:
@@ -120,19 +121,19 @@
             df = df_wt
             df_wt['type'] = 'Single'
             title = title + '   Sample:' + str(aligned_num_wt)
     elif args.function == 'f5c':
         from nanoCEM.read_f5c_resquiggle import read_blow5
         if args.base_shift < 0:
             raise RuntimeError("base_shift should not less than 0")
-        if (args.rna and args.strand=='+') or (not args.rna and args.strand=='-'):
-            args.pos = args.pos + args.base_shift
-        else:
-            args.pos = args.pos - args.base_shift
-        df_wt, aligned_num_wt,nucleotide_type = read_blow5(args.input, args.pos, args.len, args.chrom, args.strand,subsample_num)
+        # if (args.rna and args.strand=='+') or (not args.rna and args.strand=='-'):
+        #     args.pos = args.pos + args.base_shift
+        # else:
+        #     args.pos = args.pos - args.base_shift
+        df_wt, aligned_num_wt,nucleotide_type = read_blow5(args.input, args.pos, args.len, args.chrom, args.strand,subsample_num,args.base_shift)
         df_wt['type'] = 'Sample'
         if nucleotide_type=='RNA' and not args.rna:
             raise RuntimeError("You need to add --rna to turn on the rna mode")
         try:
             df_ivt, aligned_num_ivt,_ = read_blow5(args.control, args.pos, args.len, args.chrom, args.strand,
                                                  subsample_num)
             df_ivt['type'] = 'Control'
@@ -154,20 +155,20 @@
     category = pd.api.types.CategoricalDtype(categories=category_data, ordered=True)
     df['position'] = df['position'].astype(category)
 
 
     # draw_volin(df,results_path,args.pos,base_list,title)
     # draw_boxplot(df,results_path,args.pos,base_list,title)
     print("Start to generate plots and save  in "+ results_path)
-    if args.function == 'f5c':
-        if (args.rna and args.strand == '+') or (not args.rna and args.strand == '-'):
-            args.pos = args.pos - args.base_shift
-        else:
-            args.pos = args.pos + args.base_shift
+    # if args.function == 'f5c':
+    #     if (args.rna and args.strand == '+') or (not args.rna and args.strand == '-'):
+    #         args.pos = args.pos - args.base_shift
+    #     else:
+    #         args.pos = args.pos + args.base_shift
     percentile_filter=False
-    if aligned_num_wt>50 and aligned_num_ivt>50:
+    if aligned_num_wt > 50 and aligned_num_ivt > 50:
         percentile_filter=True
 
     signal_plot(df, results_path, args.pos, base_list, title, 'merged',percentile_filter)
     signal_plot(df, results_path, args.pos, base_list, title, 'boxplot')
     signal_plot(df, results_path, args.pos, base_list, title, 'violin_plot')
     print('finished')
```

### Comparing `nanoCEM-0.0.1.1/nanoCEM/cem_utils.py` & `nanoCEM-0.0.1.2/nanoCEM/cem_utils.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.1.1/nanoCEM/current_events_magnifier.py` & `nanoCEM-0.0.1.2/nanoCEM/current_events_magnifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 import argparse
 import os
-from nanoCEM.cem_utils import read_fasta_to_dic,reverse_fasta
+from cem_utils import read_fasta_to_dic,reverse_fasta
 import pandas as pd
-from nanoCEM.plot import signal_plot
+from plot import signal_plot
 from plotnine.exceptions import PlotnineWarning
 import warnings
 import time
 warnings.filterwarnings("ignore", category=PlotnineWarning)
 import numpy as np
 def init_parser():
     def add_public_argument(parser_input):
@@ -42,22 +42,22 @@
     parser_f5c.add_argument("-i", "--input", required=True,
                         help="blow5_path")
     parser_f5c.add_argument('-c', "--control",
                         help="control_blow5_path")
     parser_f5c.add_argument('-o', "--output", default="f5c_result", help="output_file")
     parser_f5c.add_argument('--base_shift',type=int, default=0, help="output_file")
     add_public_argument(parser_f5c)
-
     return parser
 
 if __name__ == '__main__':
     # Parse the arguments
     parser = init_parser()
     args = parser.parse_args()
-
+    aligned_num_wt = 0
+    aligned_num_ivt = 0
     # read reference
     subsample_num = args.overplot_number
     fasta = read_fasta_to_dic(args.ref)
     # length filter
     args.pos = args.pos - 1
     length_gene = len(fasta[args.chrom])
     if args.pos + args.len + 1 >= length_gene or args.pos - args.len <= 0:
@@ -106,19 +106,19 @@
             df = df_wt
             df_wt['type'] = 'Single'
             title = title + '   Sample:' + str(aligned_num_wt)
     elif args.function == 'f5c':
         from nanoCEM.read_f5c_resquiggle import read_blow5
         if args.base_shift < 0:
             raise RuntimeError("base_shift should not less than 0")
-        if (args.rna and args.strand=='+') or (not args.rna and args.strand=='-'):
-            args.pos = args.pos + args.base_shift
-        else:
-            args.pos = args.pos - args.base_shift
-        df_wt, aligned_num_wt,nucleotide_type = read_blow5(args.input, args.pos, args.len, args.chrom, args.strand,subsample_num)
+        # if (args.rna and args.strand=='+') or (not args.rna and args.strand=='-'):
+        #     args.pos = args.pos + args.base_shift
+        # else:
+        #     args.pos = args.pos - args.base_shift
+        df_wt, aligned_num_wt,nucleotide_type = read_blow5(args.input, args.pos, args.len, args.chrom, args.strand,subsample_num,args.base_shift)
         df_wt['type'] = 'Sample'
         if nucleotide_type=='RNA' and not args.rna:
             raise RuntimeError("You need to add --rna to turn on the rna mode")
         try:
             df_ivt, aligned_num_ivt,_ = read_blow5(args.control, args.pos, args.len, args.chrom, args.strand,
                                                  subsample_num)
             df_ivt['type'] = 'Control'
@@ -140,20 +140,20 @@
     category = pd.api.types.CategoricalDtype(categories=category_data, ordered=True)
     df['position'] = df['position'].astype(category)
 
 
     # draw_volin(df,results_path,args.pos,base_list,title)
     # draw_boxplot(df,results_path,args.pos,base_list,title)
     print("Start to generate plots and save  in "+ results_path)
-    if args.function == 'f5c':
-        if (args.rna and args.strand == '+') or (not args.rna and args.strand == '-'):
-            args.pos = args.pos - args.base_shift
-        else:
-            args.pos = args.pos + args.base_shift
+    # if args.function == 'f5c':
+    #     if (args.rna and args.strand == '+') or (not args.rna and args.strand == '-'):
+    #         args.pos = args.pos - args.base_shift
+    #     else:
+    #         args.pos = args.pos + args.base_shift
     percentile_filter=False
-    if aligned_num_wt>50 and aligned_num_ivt>50:
+    if aligned_num_wt > 50 and aligned_num_ivt > 50:
         percentile_filter=True
 
     signal_plot(df, results_path, args.pos, base_list, title, 'merged',percentile_filter)
     signal_plot(df, results_path, args.pos, base_list, title, 'boxplot')
     signal_plot(df, results_path, args.pos, base_list, title, 'violin_plot')
     print('finished')
```

### Comparing `nanoCEM-0.0.1.1/nanoCEM/extract_sub_fast5_from_bam.py` & `nanoCEM-0.0.1.2/nanoCEM/extract_sub_fast5_from_bam.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.1.1/nanoCEM/normalization.py` & `nanoCEM-0.0.1.2/nanoCEM/normalization.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.1.1/nanoCEM/plot.py` & `nanoCEM-0.0.1.2/nanoCEM/plot.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.1.1/nanoCEM/read_f5c_resquiggle.py` & `nanoCEM-0.0.1.2/nanoCEM/read_f5c_resquiggle.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import pysam
 from tqdm import tqdm
 from nanoCEM.normalization import normalize_signal,normalize_signal_with_lim
 import os
 import argparse
 score_dict={}
 nucleotide_type=None
-def extract_feature(line,strand):
+def extract_feature(line,strand,base_shift=2):
     global nucleotide_type
     pbar.update(1)
     read_id = line[0]
     # if read_id !='562eeb47-2b86-4fc7-abfc-5dce62f511ed':
     #     return None
     if read_id not in info_dict:
         return None
@@ -87,27 +87,33 @@
 
     # normalized signal
     signal = normalize_signal_with_lim(signal)
 
     # index query and reference
     aligned_pair=info_dict[read_id]['pairs']
     qlen = info_dict[read_id]['query_length']
-
+    # correct index about DNA and RNA
     if nucleotide_type == 'RNA':
         if strand == '+':
             gap = qlen - event_length.shape[0]
             aligned_pair[0] = aligned_pair[0] - gap
             aligned_pair = aligned_pair[aligned_pair[0] >= 0]
         elif strand == '-':
             aligned_pair[0] = event_length.shape[0]-aligned_pair[0]-1
     else:
         if strand == '-':
             aligned_pair[0] = qlen - aligned_pair[0] - 1
-        aligned_pair=aligned_pair[aligned_pair[0] <= event_length.shape[0]]
-
+        aligned_pair=aligned_pair[aligned_pair[0] < event_length.shape[0]]
+    # base shift
+    if (strand == '+' and nucleotide_type == 'RNA') or (strand == '-' and nucleotide_type == 'DNA'):
+        aligned_pair[0]=aligned_pair[0].values + base_shift
+        aligned_pair = aligned_pair[aligned_pair[0] < event_length.shape[0]]
+    else:
+        aligned_pair[0] = aligned_pair[0].values - base_shift
+        aligned_pair = aligned_pair[aligned_pair[0] >= 0]
 
     if aligned_pair.shape[0]==0:
         return None
     read_pos = aligned_pair[0].values
     ref_pos = aligned_pair[1].values
 
     # extract raw signal by event length and event start
@@ -153,15 +159,15 @@
         temp['pairs']=aligned_pair
         temp['query_length'] = read.query_length
         result_dict[read.qname] = temp
     return result_dict
 
 
 
-def read_blow5(path,position,length,chromo,strand,subsapmle_num=500):
+def read_blow5(path,position,length,chromo,strand,subsapmle_num=500,base_shift=2):
     global info_dict,s5,pbar
     bam_file=path+".bam"
     bam_file=pysam.AlignmentFile(bam_file,'rb')
     # if rna_mode:
     #     if strand =='+':
     #         position=position+ (kmer_model-1)
     #     else:
@@ -176,15 +182,15 @@
     df=pd.read_csv(path+".paf",sep='\t',header=None)
     df=pd.merge(df,info_df,how='inner',on=0)
     if df.shape[0] == 0:
         raise RuntimeError("cannot found the record from bam in your paf file. Please check your f5c command ... ")
     if df.shape[0] / info_df.shape[0] < 0.8:
         print('There are '+str(info_df.shape[0]-df.shape[0])+" reads not found in your paf file ...")
     pbar = tqdm(total=df.shape[0], position=0, leave=True)
-    df["feature"] = df.apply(extract_feature,strand=strand,axis=1)
+    df["feature"] = df.apply(extract_feature,strand=strand,base_shift=base_shift,axis=1)
     pbar.close()
     df.dropna(inplace=True)
     num_aligned = df.shape[0]
     if subsapmle_num < df.shape[0]:
         df=df.sample(n=subsapmle_num)
     final_feature=[]
     for item in df["feature"]:
```

### Comparing `nanoCEM-0.0.1.1/nanoCEM/read_tombo_resquiggle.py` & `nanoCEM-0.0.1.2/nanoCEM/read_tombo_resquiggle.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.1.1/nanoCEM.egg-info/PKG-INFO` & `nanoCEM-0.0.1.2/nanoCEM.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: nanoCEM
-Version: 0.0.1.1
+Version: 0.0.1.2
 Summary: A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports two re-squiggle pipeline(Tombo and f5c).
 Home-page: https://github.com/lrslab/current_events_magnifier
 Author: GUO Zhihao
 Author-email: qhuozhihao@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7,<3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # nanoCEM
-The nanopore_current_events_magnifier(`nanoCEM`) is a python command line to facilitate the analysis of DNA/RNA modification sites by visualizing statistical features of current events. 
+The nanopore current events magnifier (`nanoCEM`) is a python command line to facilitate the analysis of DNA/RNA modification sites by visualizing statistical features of current events. 
 CEM can be used to showcase high confidence sites and observe the difference based on the modification sample and the low or no modification sample.
 
 It supports two re-squiggle pipeline(`Tombo` and `f5c`) and support `R9` and `R10`.
 If you want to view single read signal or raw signal, [Squigualiser](https://github.com/hiruna72/squigualiser) is recommended.
 
 ## Example
 Here is an example that show the difference of A2030 on 23S rRNA.
@@ -49,15 +49,15 @@
 pip install nanoCEM==0.0.4.4
 pip install ont-fast5-api
 conda install -c bioconda f5c slow5tools
 ```
 ## Options
 ### read_tombo_resquiggle
 ```sh
-nanoCEM.py tombo -h
+current_events_magnifier.py tombo -h
 optional arguments:
   -h, --help            show this help message and exit
   --basecall_group BASECALL_GROUP
                         The attribute group to extract the training data from. e.g. RawGenomeCorrected_000
   --basecall_subgroup BASECALL_SUBGROUP
                         Basecall subgroup Nanoraw resquiggle into. Default is BaseCalled_template
   -i FAST5, --fast5 FAST5
@@ -74,15 +74,15 @@
   --ref REF             fasta file
   --overplot-number OVERPLOT_NUMBER (default:500)
                         Number of read will be used to plot
   --rna                 Turn on the RNA mode 
 ```
 ### read_f5c_resquiggle
 ```sh
-nanoCEM.py f5c -h
+current_events_magnifier.py f5c -h
 optional arguments:
   -h, --help            show this help message and exit
   -i INPUT, --input INPUT
                         path and suffix of blow5, bam file and paf files
   -c CONTROL, --control CONTROL
                         control path and suffix of blow5, bam file and paf files
   -o OUTPUT, --output OUTPUT
@@ -163,15 +163,15 @@
 Use ```--rna``` to turn to the rna mode and ```--pore r10``` to re-squiggle reads from R10
 ```sh
 f5c resquiggle -c all.fastq file.blow5 -o file.paf --rna --pore r9
 ```
 3. Run nanoCEM to plot
 ```sh
 # run the pipeline below for your two sample respective and keep the suffix of bam/paf/blow5 is the same
-nanoCEM.py f5c -i sample1/file -c sample2/file -o f5c_result \
+current_events_magnifier.py f5c -i sample1/file -c sample2/file -o f5c_result \
 --chrom NR_103073.1 --strand + \
 --pos 3929 --len 10 \
 --ref reference.fasta --base_shift 2 --rna
 ```
```

### Comparing `nanoCEM-0.0.1.1/setup.py` & `nanoCEM-0.0.1.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="nanoCEM",
-    version="0.0.1.1",
+    version="0.0.1.2",
     author="GUO Zhihao",
     author_email="qhuozhihao@icloud.com",
     description='A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level.\
                 It supports two re-squiggle pipeline(Tombo and f5c).',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lrslab/current_events_magnifier",
```

