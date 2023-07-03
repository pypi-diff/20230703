# Comparing `tmp/isotools-0.3.3.tar.gz` & `tmp/isotools-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isotools-0.3.3.tar", last modified: Tue Apr 25 11:57:25 2023, max compression
+gzip compressed data, was "isotools-0.3.4.tar", last modified: Mon Jul  3 10:20:18 2023, max compression
```

## Comparing `isotools-0.3.3.tar` & `isotools-0.3.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-s--x   0 lienhard  (2263) 42grp      (542)        0 2023-04-25 11:57:25.748769 isotools-0.3.3/
--rw-rw----   0 lienhard  (2263) 42grp      (542)     8837 2023-04-20 10:09:55.000000 isotools-0.3.3/CHANGELOG.md
--rw-r--r--   0 lienhard  (2263) 42grp      (542)     1069 2021-07-05 21:13:24.000000 isotools-0.3.3/LICENSE.txt
--rw-r--r--   0 lienhard  (2263) 42grp      (542)       66 2021-07-06 21:43:48.000000 isotools-0.3.3/MANIFEST.in
--rw-r-----   0 lienhard  (2263) 42grp      (542)     3682 2023-04-25 11:57:25.757769 isotools-0.3.3/PKG-INFO
--rw-r--r--   0 lienhard  (2263) 42grp      (542)     3094 2022-07-25 20:40:02.000000 isotools-0.3.3/README.md
--rw-rw----   0 lienhard  (2263) 42grp      (542)        6 2023-04-25 11:54:34.000000 isotools-0.3.3/VERSION.txt
--rw-r--r--   0 lienhard  (2263) 42grp      (542)      499 2021-11-03 16:29:14.000000 isotools-0.3.3/pyproject.toml
--rw-r--r--   0 lienhard  (2263) 42grp      (542)      144 2022-12-20 14:36:28.000000 isotools-0.3.3/requirements.txt
--rw-r--r--   0 lienhard  (2263) 42grp      (542)     1106 2023-04-25 11:57:25.815769 isotools-0.3.3/setup.cfg
--rw-r--r--   0 lienhard  (2263) 42grp      (542)       69 2022-03-15 10:42:16.000000 isotools-0.3.3/setup.py
-drwxr-s--x   0 lienhard  (2263) 42grp      (542)        0 2023-04-25 11:57:23.572777 isotools-0.3.3/src/
-drwxr-s--x   0 lienhard  (2263) 42grp      (542)        0 2023-04-25 11:57:25.345771 isotools-0.3.3/src/isotools/
--rw-r--r--   0 lienhard  (2263) 42grp      (542)     1392 2022-12-20 14:05:25.000000 isotools-0.3.3/src/isotools/__init__.py
--rw-r--r--   0 lienhard  (2263) 42grp      (542)    35998 2022-12-20 14:05:26.000000 isotools-0.3.3/src/isotools/_gene_plots.py
--rw-r--r--   0 lienhard  (2263) 42grp      (542)    16950 2023-04-25 11:54:19.000000 isotools-0.3.3/src/isotools/_transcriptome_filter.py
--rw-rw----   0 lienhard  (2263) 42grp      (542)    92705 2023-04-25 11:55:17.000000 isotools-0.3.3/src/isotools/_transcriptome_io.py
--rw-r--r--   0 lienhard  (2263) 42grp      (542)    45711 2023-04-20 09:20:25.000000 isotools-0.3.3/src/isotools/_transcriptome_stats.py
--rw-rw----   0 lienhard  (2263) 42grp      (542)    18257 2023-02-21 16:14:10.000000 isotools-0.3.3/src/isotools/_utils.py
--rw-r--r--   0 lienhard  (2263) 42grp      (542)     1816 2021-11-08 07:31:42.000000 isotools-0.3.3/src/isotools/decorators.py
--rw-r--r--   0 lienhard  (2263) 42grp      (542)    21716 2023-04-25 11:55:14.000000 isotools-0.3.3/src/isotools/domains.py
--rw-r--r--   0 lienhard  (2263) 42grp      (542)    46312 2023-04-20 09:21:31.000000 isotools-0.3.3/src/isotools/gene.py
--rw-r--r--   0 lienhard  (2263) 42grp      (542)    19493 2023-02-27 10:02:46.000000 isotools-0.3.3/src/isotools/plots.py
--rw-r--r--   0 lienhard  (2263) 42grp      (542)    19824 2022-12-20 14:05:28.000000 isotools-0.3.3/src/isotools/run_isotools.py
--rw-r-----   0 lienhard  (2263) 42grp      (542)     3791 2022-08-30 17:56:01.000000 isotools-0.3.3/src/isotools/short_read.py
--rwxr-xr-x   0 lienhard  (2263) 42grp      (542)    58449 2023-02-21 14:29:36.000000 isotools-0.3.3/src/isotools/splice_graph.py
--rw-rw----   0 lienhard  (2263) 42grp      (542)    11241 2022-10-21 15:40:11.000000 isotools-0.3.3/src/isotools/transcriptome.py
-drwxr-s--x   0 lienhard  (2263) 42grp      (542)        0 2023-04-25 11:57:25.708770 isotools-0.3.3/src/isotools.egg-info/
--rw-r-----   0 lienhard  (2263) 42grp      (542)     3682 2023-04-25 11:57:23.000000 isotools-0.3.3/src/isotools.egg-info/PKG-INFO
--rw-r-----   0 lienhard  (2263) 42grp      (542)      721 2023-04-25 11:57:23.000000 isotools-0.3.3/src/isotools.egg-info/SOURCES.txt
--rw-r-----   0 lienhard  (2263) 42grp      (542)        1 2023-04-25 11:57:23.000000 isotools-0.3.3/src/isotools.egg-info/dependency_links.txt
--rw-r-----   0 lienhard  (2263) 42grp      (542)       60 2023-04-25 11:57:23.000000 isotools-0.3.3/src/isotools.egg-info/entry_points.txt
--rw-r-----   0 lienhard  (2263) 42grp      (542)      198 2023-04-25 11:57:23.000000 isotools-0.3.3/src/isotools.egg-info/requires.txt
--rw-r-----   0 lienhard  (2263) 42grp      (542)        9 2023-04-25 11:57:23.000000 isotools-0.3.3/src/isotools.egg-info/top_level.txt
+drwxr-s--x   0 lienhard  (2263) 42grp      (542)        0 2023-07-03 10:20:18.824497 isotools-0.3.4/
+-rw-r-----   0 lienhard  (2263) 42grp      (542)     9422 2023-07-03 10:18:16.000000 isotools-0.3.4/CHANGELOG.md
+-rw-r--r--   0 lienhard  (2263) 42grp      (542)     1069 2021-07-05 21:13:24.000000 isotools-0.3.4/LICENSE.txt
+-rw-r--r--   0 lienhard  (2263) 42grp      (542)       66 2021-07-06 21:43:48.000000 isotools-0.3.4/MANIFEST.in
+-rw-r-----   0 lienhard  (2263) 42grp      (542)     3755 2023-07-03 10:20:18.832497 isotools-0.3.4/PKG-INFO
+-rw-r-----   0 lienhard  (2263) 42grp      (542)     3167 2023-07-03 10:18:16.000000 isotools-0.3.4/README.md
+-rw-r-----   0 lienhard  (2263) 42grp      (542)        6 2023-07-03 10:18:43.000000 isotools-0.3.4/VERSION.txt
+-rw-r--r--   0 lienhard  (2263) 42grp      (542)      499 2021-11-03 16:29:14.000000 isotools-0.3.4/pyproject.toml
+-rw-r-----   0 lienhard  (2263) 42grp      (542)      148 2023-07-03 10:18:16.000000 isotools-0.3.4/requirements.txt
+-rw-r-----   0 lienhard  (2263) 42grp      (542)     1112 2023-07-03 10:20:18.900497 isotools-0.3.4/setup.cfg
+-rw-r--r--   0 lienhard  (2263) 42grp      (542)       69 2022-03-15 10:42:16.000000 isotools-0.3.4/setup.py
+drwxr-s--x   0 lienhard  (2263) 42grp      (542)        0 2023-07-03 10:20:16.543505 isotools-0.3.4/src/
+drwxr-s--x   0 lienhard  (2263) 42grp      (542)        0 2023-07-03 10:20:18.332499 isotools-0.3.4/src/isotools/
+-rw-r--r--   0 lienhard  (2263) 42grp      (542)     1392 2022-12-20 14:05:25.000000 isotools-0.3.4/src/isotools/__init__.py
+-rw-r-----   0 lienhard  (2263) 42grp      (542)    37925 2023-07-03 10:18:17.000000 isotools-0.3.4/src/isotools/_gene_plots.py
+-rw-r-----   0 lienhard  (2263) 42grp      (542)    18900 2023-07-03 10:18:17.000000 isotools-0.3.4/src/isotools/_transcriptome_filter.py
+-rw-r-----   0 lienhard  (2263) 42grp      (542)    92795 2023-04-26 13:05:31.000000 isotools-0.3.4/src/isotools/_transcriptome_io.py
+-rw-r-----   0 lienhard  (2263) 42grp      (542)    45708 2023-07-03 10:18:17.000000 isotools-0.3.4/src/isotools/_transcriptome_stats.py
+-rw-r-----   0 lienhard  (2263) 42grp      (542)    19990 2023-07-03 10:18:17.000000 isotools-0.3.4/src/isotools/_utils.py
+-rw-r--r--   0 lienhard  (2263) 42grp      (542)     1816 2021-11-08 07:31:42.000000 isotools-0.3.4/src/isotools/decorators.py
+-rw-r-----   0 lienhard  (2263) 42grp      (542)    21716 2023-04-26 13:05:31.000000 isotools-0.3.4/src/isotools/domains.py
+-rw-r-----   0 lienhard  (2263) 42grp      (542)    47045 2023-07-03 10:18:17.000000 isotools-0.3.4/src/isotools/gene.py
+-rw-r-----   0 lienhard  (2263) 42grp      (542)    19493 2023-04-26 13:05:31.000000 isotools-0.3.4/src/isotools/plots.py
+-rw-r--r--   0 lienhard  (2263) 42grp      (542)    19824 2022-12-20 14:05:28.000000 isotools-0.3.4/src/isotools/run_isotools.py
+-rw-r-----   0 lienhard  (2263) 42grp      (542)     3791 2022-08-30 17:56:01.000000 isotools-0.3.4/src/isotools/short_read.py
+-rwxr-x--x   0 lienhard  (2263) 42grp      (542)    58449 2023-04-26 13:05:31.000000 isotools-0.3.4/src/isotools/splice_graph.py
+-rw-r-----   0 lienhard  (2263) 42grp      (542)    11261 2023-07-03 10:18:17.000000 isotools-0.3.4/src/isotools/transcriptome.py
+drwxr-s--x   0 lienhard  (2263) 42grp      (542)        0 2023-07-03 10:20:18.775498 isotools-0.3.4/src/isotools.egg-info/
+-rw-r-----   0 lienhard  (2263) 42grp      (542)     3755 2023-07-03 10:20:16.000000 isotools-0.3.4/src/isotools.egg-info/PKG-INFO
+-rw-r-----   0 lienhard  (2263) 42grp      (542)      721 2023-07-03 10:20:16.000000 isotools-0.3.4/src/isotools.egg-info/SOURCES.txt
+-rw-r-----   0 lienhard  (2263) 42grp      (542)        1 2023-07-03 10:20:16.000000 isotools-0.3.4/src/isotools.egg-info/dependency_links.txt
+-rw-r-----   0 lienhard  (2263) 42grp      (542)       60 2023-07-03 10:20:16.000000 isotools-0.3.4/src/isotools.egg-info/entry_points.txt
+-rw-r-----   0 lienhard  (2263) 42grp      (542)      203 2023-07-03 10:20:16.000000 isotools-0.3.4/src/isotools.egg-info/requires.txt
+-rw-r-----   0 lienhard  (2263) 42grp      (542)        9 2023-07-03 10:20:16.000000 isotools-0.3.4/src/isotools.egg-info/top_level.txt
```

### Comparing `isotools-0.3.3/CHANGELOG.md` & `isotools-0.3.4/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,30 @@
 # Change Log
 
 ## TODO: ideas, issues and planed extensions or changes that are not yet implemented
 * optimize add_qc_metrics for run after new samples have been added - should not recompute everything
 * planned new feature: during import of long reads, (optionally) correct for short exon alignment issues. 
 * separate new read import and classification of isoforms.
 
+## [0.3.4]
+* fixing #8: AssertationError when unifying TSS/PAS between transcript
+* improved domain plots: ORF start and end do not appear like exon exon boundaries. 
+* API change: separated ORF prediction from QC metrics calculation. 
+* new feature: count number of upstream start codons in Gene.add_orfs() (called by default when adding QC metrics to transcriptome)
+* new feature: calculate Fickett testcode and hexamer score for longest ORFs, to separate coding and noncoding genes. 
+
+
 ## [0.3.3]
 * fixed bug in filter_ref_transcripts with no query
 * export gtf with long read transcripts as well uncovered as reference transcripts
 * fix warning in plot_diff_results
 * changed export to rMATS: events report complete flanking exons of top covered isoform
 * fixed bug with transcript_id_col parameter in add_sample_from_csv
 * fixed handling of interpro protein domains
+* improved documentation: syntax highlighting, code style, additional explanations on filtering
 
 ## [0.3.2]
 * restructured tutorials
 * new feature: add domains to differential splicing result tables.
 * new feature: min_coverage and max_coverage for iter_genes function.
 
 ## [0.3.1]
```

### Comparing `isotools-0.3.3/LICENSE.txt` & `isotools-0.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `isotools-0.3.3/PKG-INFO` & `isotools-0.3.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isotools
-Version: 0.3.3
+Version: 0.3.4
 Summary: Framework for the analysis of long read transcriptome sequencing data
 Home-page: https://github.com/MatthiasLienhard/isotools
 Author: Matthias Lienhard
 Author-email: lienhard@molgen.mpg.de
 Project-URL: Bug Tracker, https://github.com/MatthiasLienhard/isotools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -67,8 +67,8 @@
 isoseq.add_qc_metrics('../tests/data/example.fa')
 isoseq.save('../tests/data/example_1_isotools.pkl')
 ```
 
 ## Citation and feedback:
 * If you run into any issues, please use the [github issues report feature](https://github.com/MatthiasLienhard/isotools/issues).
 * For general feedback, please write me an email to [lienhard@molgen.mpg.de](mailto:lienhard@molgen.mpg.de).
-* If you use isotools in your publication, please cite the following paper: IsoTools: IsoTools: a python toolbox for long-read transcriptome sequencing (in preparation)
+* If you use isotools in your publication, please cite the following [paper](https://doi.org/10.1093/bioinformatics/btad364): Lienhard et al, Bioinformatics, 2023: IsoTools: a flexible workflow for long-read transcriptome sequencing analysis
```

### Comparing `isotools-0.3.3/README.md` & `isotools-0.3.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -51,8 +51,8 @@
 isoseq.add_qc_metrics('../tests/data/example.fa')
 isoseq.save('../tests/data/example_1_isotools.pkl')
 ```
 
 ## Citation and feedback:
 * If you run into any issues, please use the [github issues report feature](https://github.com/MatthiasLienhard/isotools/issues).
 * For general feedback, please write me an email to [lienhard@molgen.mpg.de](mailto:lienhard@molgen.mpg.de).
-* If you use isotools in your publication, please cite the following paper: IsoTools: IsoTools: a python toolbox for long-read transcriptome sequencing (in preparation)
+* If you use isotools in your publication, please cite the following [paper](https://doi.org/10.1093/bioinformatics/btad364): Lienhard et al, Bioinformatics, 2023: IsoTools: a flexible workflow for long-read transcriptome sequencing analysis
```

### Comparing `isotools-0.3.3/setup.cfg` & `isotools-0.3.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 	pysam
 	umap-learn
 	scikit-learn
 	scipy
 	statsmodels
 	pyhmmer
 	requests
+	CPAT
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 console_scripts = 
 	run_isotools = isotools.run_isotools:main
```

### Comparing `isotools-0.3.3/src/isotools/__init__.py` & `isotools-0.3.4/src/isotools/__init__.py`

 * *Files identical despite different names*

### Comparing `isotools-0.3.3/src/isotools/_gene_plots.py` & `isotools-0.3.4/src/isotools/_gene_plots.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import collections.abc
 import matplotlib.colors as plt_col
 import matplotlib.patches as patches
 import matplotlib.pyplot as plt
 from matplotlib.ticker import FuncFormatter
 import numpy as np
 from math import log10
+from itertools import chain
 from ._utils import has_overlap, pairwise
 import logging
 logger = logging.getLogger('isotools')
 
 
 def _label_overlap(pos1, pos2, width, height):
     if abs(pos1[0] - pos2[0]) < width and abs(pos1[1] - pos2[1]) < height:
@@ -511,19 +512,50 @@
                 adj_pos.append(seg)
             else:
                 adj_pos[-1][1] = seg[-1]
     return adj_pos
 
 
 def get_rects(blocks, h=1, w=.1, connect=False,  **kwargs):
-    rects = [patches.Rectangle((b[0], h), b[1]-b[0], w, **kwargs) for b in blocks]
+    rects = [patches.Rectangle((b[0], h-w/2), b[1]-b[0], w, **kwargs) for b in blocks]
+    #  Rectangle(xy=lower left, width, height)
+    if connect:  # draw a line between blocks
+        rects.extend([patches.Polygon(np.array([[b1[1], h], [b2[0], h]]), closed=True, **kwargs) for b1, b2 in pairwise(blocks) if b1[1] < b2[0]])
+    return (rects)
+
 
-    if connect:
-        c = h+w/2
-        rects.extend([patches.Polygon(np.array([[b1[1], c], [b2[0], c]]), closed=True, **kwargs) for b1, b2 in pairwise(blocks)])
+def get_patches(start_blocks, orf_blocks, end_blocks, h, w1=.1, w2=.5, connect=True, **kwargs):
+    rects = [patches.Rectangle((b[0], h-w1/2), b[1]-b[0], w1, **kwargs) for b in start_blocks[:-1]]
+    rects.extend([patches.Rectangle((b[0], h-w1/2), b[1]-b[0], w1, **kwargs) for b in end_blocks[1:]])
+    if not orf_blocks:
+        if start_blocks:
+            rects.append(patches.Rectangle((start_blocks[-1][0], h-w1/2), start_blocks[-1][1]-start_blocks[-1][0], w1, **kwargs))
+        if end_blocks:
+            rects.append(patches.Rectangle((end_blocks[0][0], h-w1/2), end_blocks[0][1]-end_blocks[0][0], w1, **kwargs))
+        return rects
+    rects.extend(patches.Rectangle((b[0], h-w2/2), b[1]-b[0], w2, **kwargs) for b in orf_blocks[1:-1])
+    b1, b4 = start_blocks[-1], end_blocks[0]
+    y1, y2 = h+w1/2, h-w1/2
+    p_start = [[b1[1], y2], [b1[0], y2], [b1[0], y1], [b1[1], y1]]
+    p_end = [[b4[0], y1], [b4[1], y1], [b4[1], y2], [b4[0], y2]]
+    y1, y2 = h+w2/2, h-w2/2
+    b2 = orf_blocks[0]
+    if len(orf_blocks) == 1:
+        xy = np.array(list(chain(p_start, [[b2[0], y1], [b2[1], y1]], p_end, [[b2[1], y2], [b2[0], y2]])))
+        rects.append(patches.Polygon(xy, closed=True, **kwargs))
+    else:
+        xy = np.array(list(chain(p_start, [[b2[0], y1], [b2[1], y1], [b2[1], y2], [b2[0], y2]])))
+        rects.append(patches.Polygon(xy, closed=True, **kwargs))
+        b3 = orf_blocks[-1]
+        xy = np.array(list(chain([[b3[1], y2], [b3[0], y2], [b3[0], y1], [b3[1], y1]], p_end)))
+        rects.append(patches.Polygon(xy, closed=True, **kwargs))
+
+    if connect:  # draw a line between blocks
+        all_blocks = chain(start_blocks, orf_blocks, end_blocks)
+        rects.extend([patches.Polygon(np.array([[b1[1], h], [b2[0], h]]), closed=False, **kwargs) for b1, b2 in pairwise(all_blocks) if b1[1] < b2[0]])
     return (rects)
 
 
 def find_segments(transcripts, orf_only=True, seperate_exons=False):
     '''Find exonic parts of the gene, with respect to trids.'''
     if orf_only:
         exon_list = []
@@ -654,35 +686,35 @@
         highlight_pos = sorted(highlight_pos)
         pos_map = genome_pos_to_gene_segments(highlight_pos, genome_map, False)
         for pos in highlight:
             if isinstance(pos, collections.abc.Sequence):
                 assert len(pos) == 2, 'provide intervals as a sequence of length 2'
                 # draw box
                 box_x = sorted(pos_map[p] for p in pos)
-                patch = patches.Rectangle((box_x[0], -n_tr+.7), box_x[1]-box_x[0], n_tr+.6, edgecolor=highlight_col, facecolor=highlight_col)
+                patch = patches.Rectangle((box_x[0], -n_tr), box_x[1]-box_x[0], n_tr+1, edgecolor=highlight_col, facecolor=highlight_col)
                 ax.add_patch(patch)
             else:  # draw line
-                ax.vlines(pos_map[pos], -n_tr+.7, 0.8, colors=[highlight_col])
+                ax.vlines(pos_map[pos], -n_tr, 1, colors=[highlight_col])
 
     for line, (trid, tr) in enumerate(transcripts):
         seg = segments[line]
         orf_pos = tr.get('CDS', tr.get('ORF'))[:2]
         orf = sorted(self.find_transcript_positions(trid, orf_pos, reference=line < len(ref_trids)))
         if include_utr:
-            for rect in get_rects(find_blocks((0, orf[0]), seg),
-                                  h=-line+.2, w=.1, connect=True, linewidth=1, edgecolor="black", facecolor="white"):
-                ax.add_patch(rect)
-            for rect in get_rects(find_blocks((orf[1], sum(e[1]-e[0] for e in tr['exons'])), seg),
-                                  h=-line+.2, w=.1, connect=True, linewidth=1, edgecolor="black", facecolor="white"):
-                ax.add_patch(rect)
+            start_blocks = find_blocks((0, orf[0]), seg)
+            orf_blocks = find_blocks(orf[:2], seg)
+            end_blocks = find_blocks((orf[1], sum(e[1]-e[0] for e in tr['exons'])), seg)
+            for block_patch in get_patches(start_blocks, orf_blocks, end_blocks,
+                                           h=-line, connect=True,
+                                           linewidth=1, edgecolor="black", facecolor="white"):
+                ax.add_patch(block_patch)
         else:
-            orf = (0, orf[1]-orf[0])
-        orf_block = find_blocks((orf), seg)
-        for rect in get_rects(orf_block, h=-line, w=.5, connect=True, linewidth=1, edgecolor="black", facecolor="white"):
-            ax.add_patch(rect)
+            orf_block = find_blocks((0, orf[1]-orf[0]), seg)
+            for rect in get_patches([], orf_block, [], h=-line, linewidth=1, edgecolor="black", facecolor="white"):
+                ax.add_patch(rect)
 
         domains = [dom for dom in tr.get('domain', {}).get(source, []) if categories is None or dom[2] in categories]
         # sort by length
         domains.sort(key=lambda x: x[3][1]-x[3][0], reverse=True)
         # get positions relative to segments
         dom_blocks = [find_blocks([p+orf[0] for p in dom[3]], seg, True) for dom in domains]
         dom_line = {}
@@ -695,29 +727,29 @@
                     skipped += 1
                     break
             else:
                 dom_line[i].append((idx, block_interval))  # idx in length-sorted domains
 
         w = .4/max(len(dom_line), 1)
         for dom_l in dom_line:
-            h = -line+w*(len(dom_line)//2 + (dom_l+1)//2 * (-1 if dom_l % 2 else 1))+.05
+            h = -line+w*(len(dom_line)//2 + (dom_l+1)//2 * (-1 if dom_l % 2 else 1))
             for idx, bl in dom_line[dom_l]:
                 dom = domains[idx]
                 try:
                     for rect in get_rects(dom_blocks[idx], h=h, w=w, linewidth=1, edgecolor="black", facecolor=domain_cols.get(dom[2].lower(), "white")):
                         ax.add_patch(rect)
                 except IndexError:
                     logger.error(f'cannot add patch for {dom_blocks[idx]}')
                     raise
                 if label is not None:
-                    ax.text((bl[0]+bl[1])/2, h+w/2, dom[label_idx], ha='center', va='center', color='black', clip_on=True)
+                    ax.text((bl[0]+bl[1])/2, h, dom[label_idx], ha='center', va='center', color='black', clip_on=True)
 
     if skipped:
         logger.warning("skipped %s domains, consider increasing max_overlap parameter", skipped)
-    ax.set_ylim(-len(transcripts)+.5, 1)
+    ax.set_ylim(-len(transcripts)+.25, .75)
     ax.set_xlim(-10, max_len+10)
     if x_ticks == 'genome':
         xticks = [0]+list(np.cumsum([abs(seg[1]-seg[0]) for seg in genome_map]))
         xticklabels = [str(genome_map[0][0])]+[f'{seg[0][1]}|{seg[1][0]}' for seg in pairwise(genome_map)] + [str(genome_map[-1][1])]
         ax.set_xticks(ticks=xticks, labels=xticklabels)
-    ax.set_yticks(ticks=[-i+.25 for i in range(len(transcripts))], labels=[tr.get('transcript_name', f'{self.name} {trid}') for trid, tr in transcripts])
+    ax.set_yticks(ticks=[-i for i in range(len(transcripts))], labels=[tr.get('transcript_name', f'{self.name} {trid}') for trid, tr in transcripts])
     return ax, genome_map
```

### Comparing `isotools-0.3.3/src/isotools/_transcriptome_filter.py` & `isotools-0.3.4/src/isotools/_transcriptome_filter.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,28 +34,66 @@
 ANNOTATION_VOCABULARY = ['antisense', 'intergenic', 'genic genomic', 'novel exonic PAS', 'novel intronic PAS', 'readthrough fusion',
                          'novel exon', "novel 3' splice site", 'intron retention', "novel 5' splice site", 'exon skipping', 'novel combination',
                          'novel intronic TSS', 'novel exonic TSS', 'mono-exon', 'novel junction', "5' fragment", "3' fragment", 'intronic']
 
 
 # filtering functions for the transcriptome class
 
+def add_orf_prediction(self, genome_fn, progress_bar=True, fickett_score=True, hexamer_file=None):
+    ''' Performs ORF prediction on the transcripts.
 
-def add_qc_metrics(self, genome_fn, progress_bar=True, downstream_a_len=30, direct_repeat_wd=15, direct_repeat_wobble=2, direct_repeat_mm=2, unify_ends=True):
+    For each transcript the longest open reading frame is determined, and metrics to assess the coding potential
+    (UTR and CDS lenghts, Fickett score, hexamer score and NMD prediction). The hexamer score depends on hexamer frequency table,
+    see CPAT python module for prebuild tables and instructions.
+
+    :param geneome_fn: Path to the genome in fastA format.
+    :param fickett_score: If set to True, the Fickett TESTCODE score is computed for each transcript.
+    :param hexamer_file: Filename of the hexamer table, for the ORF hexamer scores. If set not None, the hexamer score is not computed.'''
+
+    if hexamer_file is None:
+        coding = None
+        noncoding = None
+    else:
+        coding = {}
+        noncoding = {}
+        for line in open(hexamer_file):
+            line = line.strip()
+            fields = line.split()
+            if fields[0] == 'hexamer':
+                continue
+            coding[fields[0]] = float(fields[1])
+            noncoding[fields[0]] = float(fields[2])
+
+    with FastaFile(genome_fn) as genome_fh:
+        missing_chr = set(self.chromosomes) - set(genome_fh.references)
+        if missing_chr:
+            missing_genes = sum(len(self.data[mc]) for mc in missing_chr)
+            logger.warning('%s contigs are not contained in genome, affecting %s genes. \
+                ORFs cannot be computed for these contigs: %s', str(len(missing_chr)), str(missing_genes), str(missing_chr))
+
+        for g in self.iter_genes(progress_bar=progress_bar):
+            if g.chrom in genome_fh.references:
+                g.add_orfs(genome_fh, reference=False, minlen=30, get_fickett=fickett_score, coding_hexamers=coding, noncoding_hexamers=noncoding)
+                g.add_orfs(genome_fh, reference=True, minlen=30, get_fickett=fickett_score, coding_hexamers=coding, noncoding_hexamers=noncoding)
+
+
+def add_qc_metrics(self, genome_fn, progress_bar=True, downstream_a_len=30, direct_repeat_wd=15, direct_repeat_wobble=2, direct_repeat_mm=2,
+                   unify_ends=True):
     ''' Retrieves QC metrics for the transcripts.
 
     Calling this function populates transcript["biases"] information, which can be used do create filters.
-    In particular, the direct repeat length, the downstream adenosine content and information about noncanonical splice sites are fetched.
-    Additionaly genes are scanned for transcripts that are fully contained in other transcripts.
+    In particular, the direct repeat length, the downstream adenosine content and information about non-canonical splice sites are fetched.
+    In addition, genes are scanned for transcripts that are fully contained in other transcripts.
 
     :param geneome_fn: Path to the genome in fastA format.
     :param downstream_a_len: The number of bases downstream the transcript where the adenosine fraction is determined.
     :param direct_repeat_wd: The number of bases around the splice sites scanned for direct repeats.
     :param direct_repeat_wobble: Number of bases the splice site sequences are shifted.
     :param unify_ends: Unify TSS/PAS across transcripts of a gene.
-    :param direct_repeat_mm: Maximum number of missmatches in a direct repeat. '''
+    :param direct_repeat_mm: Maximum number of missmatches in a direct repeat.'''
 
     with FastaFile(genome_fn) as genome_fh:
         missing_chr = set(self.chromosomes) - set(genome_fh.references)
         if missing_chr:
             missing_genes = sum(len(self.data[mc]) for mc in missing_chr)
             logger.warning('%s contigs are not contained in genome, affecting %s genes. \
                 Some metrics cannot be computed: %s', str(len(missing_chr)), str(missing_genes), str(missing_chr))
@@ -66,15 +104,14 @@
                 g.data['segment_graph'] = None
                 # "unify" TSS/PAS (if unify TSS/PAS option selected)
                 g._unify_ends()
             # compute segment graph (if not present)
             _ = g.segment_graph
             g.add_fragments()
             if g.chrom in genome_fh.references:
-                g.add_orfs(genome_fh, reference=False, minlen=30)
                 g.add_direct_repeat_len(genome_fh, delta=direct_repeat_wd, max_mm=direct_repeat_mm, wobble=direct_repeat_wobble)
                 g.add_noncanonical_splicing(genome_fh)
                 g.add_threeprime_a_content(genome_fh, length=downstream_a_len)
 
     self.infos['biases'] = True  # flag to check that the function was called
```

### Comparing `isotools-0.3.3/src/isotools/_transcriptome_io.py` & `isotools-0.3.4/src/isotools/_transcriptome_io.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,34 +130,37 @@
         elif 'gene_id' in cov_tab.columns and 'transcript_nr' in cov_tab.columns:
             cov_tab['transcript_id'] = cov_tab.gene_id+'_'+cov_tab.transcript_nr.astype(str)
         else:
             raise ValueError('"transcript_id_col" not specified, and coverage table does not contain "transcript_id", nor "gene_id" and "transcript_nr"')
         transcript_id_col = 'transcript_id'
     elif isinstance(transcript_id_col, list):
         assert all(c in cov_tab for c in transcript_id_col), 'missing specified transcript_id_col'
-        cov_tab['transcript_id'] = ['_'.join(str(v) for v in row.values()) for _, row in cov_tab[transcript_id_col].iterrows()]
+        cov_tab['transcript_id'] = ['_'.join(str(v) for v in row) for _, row in cov_tab[transcript_id_col].iterrows()]
         transcript_id_col = 'transcript_id'
     else:
         assert transcript_id_col in cov_tab, 'missing specified transcript_id_col'
         cov_tab['transcript_id'] = cov_tab[transcript_id_col]
     known_sa = set(samples).intersection(self.samples)
     assert transcript_id_col == 'transcript_id'  # could be optimized, but code is easier when the id column always is transcript_id
     assert not known_sa, 'Attempt to add known samples: %s' % known_sa
     # cov_tab.set_index('transcript_id')
     # assert cov_tab.index.is_unique, 'ambigous transcript ids in %s' % coverage_csv_file
     # check sample properties
     if sample_properties is None:
-        sample_properties = {sa: {} for sa in samples}
+        sample_properties = {sa: {'group': sa} for sa in samples}
     elif isinstance(sample_properties, pd.DataFrame):
         if 'name' in sample_properties:
             sample_properties = sample_properties.set_index('name')
         sample_properties = {sa: {k: v for k, v in row.items() if k not in {'file', 'nonchimeric_reads', 'chimeric_reads'}}
                              for sa, row in sample_properties.iterrows()}
     assert all(sa in sample_properties for sa in samples), 'missing sample_properties for samples %s' % ', '.join(
         (sa for sa in samples if sa not in sample_properties))
+    for sa in sample_properties:
+        sample_properties[sa].setdefault('group', sa)
+
     logger.info('adding samples "%s" from csv', '", "'.join(samples))
     # consider chromosomes not in the referernce?
     if add_chromosomes:
         chromosomes = None
     else:
         chromosomes = self.chromosomes
```

### Comparing `isotools-0.3.3/src/isotools/_transcriptome_stats.py` & `isotools-0.3.4/src/isotools/_transcriptome_stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -254,16 +254,16 @@
     return df
 
 
 def die_test(self, groups, min_cov=25, n_isoforms=10, padj_method='fdr_bh', progress_bar=True):
     ''' Reimplementation of the DIE test, suggested by Joglekar et al in Nat Commun 12, 463 (2021):
     "A spatially resolved brain region- and cell type-specific isoform atlas of the postnatal mouse brain"
 
-    Syntax and parameters follow the original implementation in
-    https://github.com/noush-joglekar/scisorseqr/blob/master/inst/RScript/IsoformTest.R
+    Syntax and parameters follow the original implementation in https://github.com/noush-joglekar/scisorseqr/blob/master/inst/RScript/IsoformTest.R
+
     :param groups: Dict with group names as keys and lists of sample names as values, defining the two groups for the test.
     :param min_cov: Minimal number of reads per group for each gene.
     :param n_isoforms: Number of isoforms to consider in the test for each gene. All additional least expressed isoforms get summarized.'''
 
     groupnames, groups, grp_idx = _check_groups(self, groups)
     logger.info('testing differential isoform expression (DIE) for %s.', ' vs '.join(f'{groupnames[i]} ({len(groups[i])})' for i in range(2)))
```

### Comparing `isotools-0.3.3/src/isotools/_utils.py` & `isotools-0.3.4/src/isotools/_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -139,36 +139,65 @@
         return False
     for e1, e2 in zip(tr1[1:-1], tr2[1:-1]):  # check other exons
         if e1[0] != e2[0] or e1[1] != e2[1]:
             return False
     return True
 
 
-def find_orfs(seq, start_codons=["ATG"], stop_codons=['TAA', 'TAG', 'TGA'], minlen=100):
+def find_longest_orf(seq, start_codons=["ATG"], stop_codons=['TAA', 'TAG', 'TGA'], coding_hexamers=None, noncoding_hexamers=None):
+    '''Find the longest open reading frames on the forward strand of the sequence.
+    Return a 8-tuple with start and stop position, reading frame (0,1 or 2), start and stop codon sequence,
+    number of upstream start codons, the hexamere score and the Fickett TESTCODE score'''
+    orf = []
+    starts = [[], [], []]
+    stops = [[], [], []]
+    for match in re.finditer("|".join(start_codons), seq):
+        starts[match.start() % 3].append((match.start(), match.group()))  # position and codon
+    for match in re.finditer("|".join(stop_codons), seq):
+        stops[match.start() % 3].append((match.end(), match.group()))
+    for frame in range(3):
+        stop, stop_codon = (0, None)
+        for start, start_codon in starts[frame]:
+            if start < stop:  # inframe start within the previous ORF
+                continue
+            try:
+                stop, stop_codon = next(s for s in sorted(stops[frame]) if s[0] > start)
+            except StopIteration:  # no stop codon - still report as it might be an uAUG
+                stop, stop_codon = start, None
+            orf.append([start, stop, frame, start_codon, stop_codon, 0])
+    if not orf:
+        return
+    uORFs = 0
+    for orf_i in sorted(orf):  # sort by start position
+        orf_i[5] = uORFs
+        uORFs += 1
+    return max(orf, key=lambda x: x[1]-x[0] if x[1] else -1)
+
+
+def find_orfs(seq, start_codons=["ATG"], stop_codons=['TAA', 'TAG', 'TGA']):
     ''' Find all open reading frames on the forward strand of the sequence.
     Return a 5-tuple with start and stop position, reading frame (0,1 or 2) and start and stop codon sequence
     '''
     orf = []
     starts = [[], [], []]
     stops = [[], [], []]
     for match in re.finditer("|".join(start_codons), seq):
-        starts[match.start() % 3].append((match.start(), match.group()))
+        starts[match.start() % 3].append((match.start(), match.group()))  # position and codon
     for match in re.finditer("|".join(stop_codons), seq):
         stops[match.start() % 3].append((match.end(), match.group()))
     for frame in range(3):
-        stop = (0, None)
-        for start in starts[frame]:
-            if start[0] < stop[0]:
+        stop, stop_codon = (0, None)
+        for start, start_codon in starts[frame]:
+            if start < stop:  # inframe start within the previous ORF
                 continue
             try:
-                stop = next(s for s in sorted(stops[frame]) if s[0] > start[0])
-            except StopIteration:
-                continue
-            if stop[0]-start[0] >= minlen:
-                orf.append((start[0], stop[0], frame, start[1], stop[1]))
+                stop, stop_codon = next(s for s in sorted(stops[frame]) if s[0] > start)
+            except StopIteration:  # no stop codon - still report as it might be an uAUG
+                stop, stop_codon = start, None
+            orf.append((start, stop, frame, start_codon, stop_codon))
     return orf
 
 
 def has_overlap(r1, r2):
     "check the overlap of two intervals"
     # assuming start < end
     if r1[1] <= r2[0] or r2[1] <= r1[0]:
@@ -195,15 +224,15 @@
     for i, tr2_exon in enumerate(tr2):
         while tr1_exon[0] < tr2_exon[1]:
             if tr2_exon[0] == tr1_exon[0] and i > 0 and j > 0:  # neglegt TSS and polyA
                 sjintersect += 1
             if tr2_exon[1] == tr1_exon[1] and i < len(tr2)-1 and j < len(tr1)-1:
                 sjintersect += 1
             if has_overlap(tr1_exon, tr2_exon):
-                # region intersect
+                # the regions intersect
                 i_end = min(tr1_exon[1], tr2_exon[1])
                 i_start = max(tr1_exon[0], tr2_exon[0])
                 intersect += (i_end-i_start)
             try:
                 j, tr1_exon = next(tr1_enum)
             except StopIteration:  # tr1 is at end
                 return sjintersect, intersect
@@ -481,7 +510,15 @@
         break
     else:
         for i in range(i, len(tr_pos)):
             mapped_pos.append(offset+intron_len+tr_pos[i])
     if reverse_strand:  # get them back to the original
         tr_pos = [tr_len-p for p in tr_pos]
     return {p: mp for p, mp in zip(tr_pos, mapped_pos)}
+
+
+def cmp_dist(a, b, min_dist=3):
+    if a >= b+min_dist:
+        return 1
+    if b >= a+min_dist:
+        return -1
+    return 0
```

### Comparing `isotools-0.3.3/src/isotools/decorators.py` & `isotools-0.3.4/src/isotools/decorators.py`

 * *Files identical despite different names*

### Comparing `isotools-0.3.3/src/isotools/domains.py` & `isotools-0.3.4/src/isotools/domains.py`

 * *Files identical despite different names*

### Comparing `isotools-0.3.3/src/isotools/gene.py` & `isotools-0.3.4/src/isotools/gene.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from operator import itemgetter
 from intervaltree import Interval
 from collections.abc import Iterable
 from scipy.stats import chi2_contingency
 from scipy.signal import find_peaks
 from Bio.Seq import reverse_complement, translate
 from Bio.Data.CodonTable import TranslationError
-
 from pysam import FastaFile
 import numpy as np
 import copy
 import itertools
+from cpmodule import fickett, FrameKmer  # this is from the CPAT module
 from .splice_graph import SegmentGraph
 from .short_read import Coverage
 from ._transcriptome_filter import SPLICE_CATEGORY
-from ._utils import pairwise, _filter_event, find_orfs, smooth, get_quantiles, _filter_function, \
-    pairwise_event_test, prepare_contingency_table
+from ._utils import pairwise, _filter_event, find_longest_orf, smooth, get_quantiles, _filter_function, \
+    pairwise_event_test, prepare_contingency_table, cmp_dist
 
 import logging
 logger = logging.getLogger('isotools')
 
 
 class Gene(Interval):
     'This class stores all gene information and transcripts. It is derived from intervaltree.Interval.'
@@ -55,16 +55,16 @@
             for i in range(len(self.data['short_reads']), len(srdf)):
                 self.data['short_reads'].append(Coverage.from_bam(srdf.file[i], self))
         return self.data['short_reads'][idx]
 
     def correct_fuzzy_junctions(self, trid, size, modify=True):
         '''Corrects for splicing shifts.
 
-         This function looks for "shifted junctions", e.g. same difference compared to reference annotaiton at both donor and acceptor)
-         presumably caused by ambigous alignments. In these cases the positions are adapted to the reference position (if modify is set).
+         This function looks for "shifted junctions", e.g. same difference compared to reference annotation at both donor and acceptor)
+         presumably caused by ambiguous alignments. In these cases the positions are adapted to the reference position (if modify is set).
 
          :param trid: The index of the transcript to be checked.
          :param size: The maximum shift to be corrected.
          :param modify: If set, the exon positions are corrected according to the reference.
          :returns: A dictionary with the exon id as keys and the shifted bases as values.'''
 
         exons = trid['exons']
@@ -161,18 +161,18 @@
         return []
 
     def add_noncanonical_splicing(self, genome_fh):
         '''Add information on noncanonical splicing.
 
         For all transcripts of the gene, scan for noncanonical (i.e. not GT-AG) splice sites.
         If noncanonical splice sites are present, the corresponding intron index (in genomic orientation) and the sequence
-        i.e. the dinucleotides of donor and aceptor as XX-YY string are stored in the "noncannoncical_splicing" field of the transcript dicts.
-        True noncanonical splicing is rare, thus it might indicate technical artifacts (template switching, missalignment, ...)
+        i.e. the di-nucleotides of donor and acceptor as XX-YY string are stored in the "noncannoncical_splicing" field of the transcript dicts.
+        True noncanonical splicing is rare, thus it might indicate technical artifacts (template switching, misalignment, ...)
 
-        :param genome_fh: A file handle of the genome fasta file.'''
+        :param genome_fh: A file handle of the genome fastA file.'''
         ss_seq = {}
         for tr in self.transcripts:
             pos = [(tr['exons'][i][1], tr['exons'][i + 1][0] - 2) for i in range(len(tr['exons']) - 1)]
             new_ss_seq = {site: genome_fh.fetch(self.chrom, site, site + 2).upper() for intron in pos for site in intron if site not in ss_seq}
             if new_ss_seq:
                 ss_seq.update(new_ss_seq)
 
@@ -184,19 +184,19 @@
             nc = [(i, seq) for i, seq in enumerate(sj_seq) if seq != 'GTAG']
             if nc:
                 tr['noncanonical_splicing'] = nc
 
     def add_direct_repeat_len(self, genome_fh, delta=15, max_mm=2, wobble=2):
         '''Computes direct repeat length.
 
-        This function counts the number of consequtive equal bases at donor and acceptor sites of the splice junctions.
+        This function counts the number of consecutive equal bases at donor and acceptor sites of the splice junctions.
         This information is stored in the "direct_repeat_len" filed of the transcript dictionaries.
         Direct repeats longer than expected by chance indicate template switching.
 
-        :param genome_fh: The file handle to the genome fasta.
+        :param genome_fh: The file handle to the genome fastA.
         :param delta: The maximum length of direct repeats that can be found.
         :param max_mm: The maximum length of direct repeats that can be found.
         :param wobble: The maximum length of direct repeats that can be found.'''
 
         intron_seq = {}
         score = {}
 
@@ -221,15 +221,15 @@
 
     def add_threeprime_a_content(self, genome_fh, length=30):
         '''Adds the information of the genomic A content downstream the transcript.
 
         High values of genomic A content indicate internal priming and hence genomic origin of the LRTS read.
         This function populates the 'downstream_A_content' field of the transcript dictionaries.
 
-        :param geneome_fh: A file handle for the indexed genome fasta file.
+        :param geneome_fh: A file handle for the indexed genome fastA file.
         :param length: The length of the downstream region to be considered.
         '''
         a_content = {}
         for tr in (t for tL in (self.transcripts, self.ref_transcripts) for t in tL):
             if self.strand == '+':
                 pos = tr['exons'][-1][1]
             else:
@@ -241,17 +241,17 @@
                 else:
                     a_content[pos] = seq.upper().count('T') / length
             tr['downstream_A_content'] = a_content[pos]
 
     def get_sequence(self, genome_fh, trids=None, reference=False, protein=False):
         '''Returns the nucleotide sequence of the specified transcripts.
 
-        :param genome_fh: The path to the genome fasta file, or FastaFile handle.
+        :param genome_fh: The path to the genome fastA file, or FastaFile handle.
         :param trids: List of transcript ids for which the sequence are requested.
-        :param reference: Specifiy whether the sequence is fetched for reference transcripts (True)
+        :param reference: Specify whether the sequence is fetched for reference transcripts (True)
             or long read transcripts (False, default).
         :param protein: Return protein sequences instead of transcript sequences.
         :returns: A dictionary of transcript ids and their sequences.
         '''
 
         trL = [(i, tr) for i, tr in enumerate(self.ref_transcripts if reference else self.transcripts) if trids is None or i in trids]
         if not trL:
@@ -282,59 +282,64 @@
             pos = sorted(self.find_transcript_positions(i, orf[:2], reference=reference))
             try:
                 prot_seqs[i] = translate(tr_seqs[i][pos[0]:pos[1]], cds=True)
             except TranslationError:
                 logger.warning(f'CDS sequence of {self.id} {"reference" if reference else ""} transcript {i} cannot be translated.')
         return prot_seqs
 
-    def add_orfs(self, genome_fh, reference=False, minlen=30, start_codons=["ATG"], stop_codons=['TAA', 'TAG', 'TGA']):
-        '''find longest ORF for each transcript and add to the transcript properties tr["ORF"]'''
-        trL = self.ref_transcripts if reference else self.transcripts
-        for (_, orfs), tr in zip(self.get_all_orf(genome_fh, reference, minlen, start_codons, stop_codons), trL):
-            if orfs:
-                tr["ORF"] = max(orfs, key=lambda x: x[2]['length'])
-
-    def get_all_orf(self, genome_fh, reference=False, minlen=30, start_codons=["ATG"], stop_codons=['TAA', 'TAG', 'TGA']):
-        ''' Predicts ORF.
+    def add_orfs(self, genome_fh, reference=False, minlen=30, start_codons=["ATG"], stop_codons=['TAA', 'TAG', 'TGA'],
+                 get_fickett=True, coding_hexamers=None, noncoding_hexamers=None):
+        '''Find longest ORF for each transcript.
+
+        For each transcript, the longest ORF (sequence starting with start_condon, and ending with in frame stop codon) is determined.
+        The genomic and transcript positions of these codons, and the length of the ORF, as well as  the number of upstream start codons
+        is added to the transcript properties tr["ORF"]. Additionally, the Fickett score, and the hexamer score are computed. For the
+        latter, hexamer frequencies in coding and noncoding transcripts are needed. See CPAT python module for prebuilt tables and
+        instructions.
+        :param minlen: the minimum length of a ORF (in bases) to be considered.
+        :param start_codons: List of base triplets that are considered as start codons. By default ['ATG'].
+        :param stop_codons: List of base triplets that are considered as stop codons. By default ['TAA', 'TAG', 'TGA'].
+        :param coding_hexamers: The hexamer frequencies for coding sequences.
+        :param noncoding_hexamers: The hexamer frequencies for coding sequences.'''
 
-        :param genome_fh: The path to the genome fasta file, or FastaFile handle.
-        :param reference: Specifiy whether the sequence is fetched for reference transcripts (True)
-            or long read transcripts (False, default).
-        :param minlen: The minimum length of the ORF.
-        :param start_codons: List of start codons.
-        :param stop_codons: List of stop codons.
-        :returns: A list of (transcript_id, list_of_orfs) tuples. Each orf is a tuple of (genomic_start, genomic_end, orf_properties).
-        The orf_properties is a dictionary with keys 'start', 'length', 'start_codon', 'stop_codon' and 'NMD'.
-        NMD is True if the ORF is predicted to be degraded by nonsense-mediated decay,
-        as defined by the 55 bases rule, e.g. there is at least one splice site upstream the stop codon,
-        and the distance of the stop codon to the last upstrame splice site is less than 55 bases.
-        '''
-        orf_list = []
         trL = self.ref_transcripts if reference else self.transcripts
         for trid, tr_seq in self.get_sequence(genome_fh, reference=reference).items():
+            try:
+                start, stop, frame, seq_start, seq_end, uORFs = find_longest_orf(
+                    tr_seq, start_codons, stop_codons, coding_hexamers, noncoding_hexamers)
+            except TypeError:  # No ORF
+                continue
+            if stop is None or stop - start < minlen:
+                continue
+
             tr = trL[trid]
             tr_start = tr['exons'][0][0]
-            cum_exon_len = np.cumsum([end-start for start, end in tr['exons']])  # cummulative exon length
-            cum_intron_len = np.cumsum([0]+[end-start for (_, start), (end, _) in pairwise(tr['exons'])])  # cummulative intron length
-            orf_list.append((tr_seq, []))
-            for start, stop, frame, seq_start, seq_end in find_orfs(tr_seq, minlen=minlen):
-                if self.strand == '-':
-                    start, stop = cum_exon_len[-1]-stop, cum_exon_len[-1]-start
-                start_exon = next(i for i in range(len(cum_exon_len)) if cum_exon_len[i] >= start)
-                stop_exon = next(i for i in range(start_exon, len(cum_exon_len)) if cum_exon_len[i] >= stop)
-                genome_pos = (tr_start+start+cum_intron_len[start_exon],
-                              tr_start+stop+cum_intron_len[stop_exon])
-                dist_pas = 0  # distance of termination codon to last upstream splice site
-                if self.strand == '+' and stop_exon < len(cum_exon_len)-1:
-                    dist_pas = cum_exon_len[-2]-stop
-                if self.strand == '-' and start_exon > 0:
-                    dist_pas = start-cum_exon_len[0]
-                orf_list[-1][1].append((*genome_pos, {'start': start, 'length': stop-start,
-                                       'start_codon': seq_start, 'stop_codon': seq_end, 'NMD': dist_pas > 55}))
-        return orf_list
+            cum_exon_len = np.cumsum([end-start for start, end in tr['exons']])  # cumulative exon length
+            cum_intron_len = np.cumsum([0]+[end-start for (_, start), (end, _) in pairwise(tr['exons'])])  # cumulative intron length
+            if self.strand == '-':
+                fwd_start, fwd_stop = cum_exon_len[-1]-stop, cum_exon_len[-1]-start
+            else:
+                fwd_start, fwd_stop = start, stop  # start/stop position wrt genomic fwd strand
+            start_exon = next(i for i in range(len(cum_exon_len)) if cum_exon_len[i] >= fwd_start)
+            stop_exon = next(i for i in range(start_exon, len(cum_exon_len)) if cum_exon_len[i] >= fwd_stop)
+            genome_pos = (tr_start+fwd_start+cum_intron_len[start_exon],
+                          tr_start+fwd_stop+cum_intron_len[stop_exon])
+            dist_pas = 0  # distance of termination codon to last upstream splice site
+            if self.strand == '+' and stop_exon < len(cum_exon_len)-1:
+                dist_pas = cum_exon_len[-2]-fwd_stop
+            if self.strand == '-' and start_exon > 0:
+                dist_pas = fwd_start-cum_exon_len[0]
+            orf_dict = {"5'UTR": start, 'CDS': stop-start, "3'UTR": cum_exon_len[-1]-stop,
+                        'start_codon': seq_start, 'stop_codon': seq_end, 'NMD': dist_pas > 55, 'uORFs': uORFs}
+
+            if coding_hexamers is not None and noncoding_hexamers is not None:
+                orf_dict['hexamer'] = FrameKmer.kmer_ratio(tr_seq[start:stop], 6, 3, coding_hexamers, noncoding_hexamers)
+            if get_fickett:
+                orf_dict['fickett'] = fickett.fickett_value(tr_seq[start:stop])
+            tr['ORF'] = (*genome_pos, orf_dict)
 
     def add_fragments(self):
         '''Checks for transcripts that are fully contained in other transcripts.
 
         Transcripts that are fully contained in other transcripts are potential truncations.
         This function populates the 'fragment' filed of the transcript dictionaries with the indices of the containing transcripts,
         and the exon ids that match the first and last exons.'''
@@ -778,14 +783,15 @@
         if not self.transcripts:
             # nothing to do here
             return
         assert 0 <= search_range[0] <= .5 <= search_range[1] <= 1
         # get gene tss/pas profiles
         tss = {}
         pas = {}
+        strand = 1 if self.strand == '+' else -1
         for tr in self.transcripts:
             for sa in tr['TSS']:
                 for pos, c in tr['TSS'][sa].items():
                     tss[pos] = tss.get(pos, 0)+c
             for sa in tr['PAS']:
                 for pos, c in tr['PAS'][sa].items():
                     pas[pos] = pas.get(pos, 0)+c
@@ -794,36 +800,37 @@
         if tss_pos[1]-tss_pos[0] < smooth_window:
             tss_pos[0] -= (smooth_window + tss_pos[0]-tss_pos[1] - 1)
         pas_pos = [min(pas), max(pas)]
         if pas_pos[1]-pas_pos[0] < smooth_window:
             pas_pos[0] -= (smooth_window + pas_pos[0]-pas_pos[1] - 1)
         tss = [tss.get(pos, 0) for pos in range(tss_pos[0], tss_pos[1]+1)]
         pas = [pas.get(pos, 0) for pos in range(pas_pos[0], pas_pos[1]+1)]
-        # smooth profiles and finde maxima
+        # smooth profiles and find maxima
         tss_smooth = smooth(np.array(tss), smooth_window)
         pas_smooth = smooth(np.array(pas), smooth_window)
         # at least half of smooth_window reads required to call a peak
         # minimal distance between peaks is > ~ smooth_window
         # rel_prominence=1 -> smaller peak must have twice the hight of valley to call two peaks
         tss_peaks, _ = find_peaks(np.log2(tss_smooth+1), prominence=(rel_prominence, None))
-        tss_peak_pos = tss_peaks+tss_pos[0]
+        tss_peak_pos = tss_peaks+tss_pos[0]-1
         pas_peaks, _ = find_peaks(np.log2(pas_smooth+1), prominence=(rel_prominence, None))
-        pas_peak_pos = pas_peaks+pas_pos[0]
+        pas_peak_pos = pas_peaks+pas_pos[0]-1
 
         # find transcripts with common first/last splice site
-        starts = {}
-        ends = {}
+        first_junction = {}
+        last_junction = {}
         for trid, tr in enumerate(self.transcripts):
-            starts.setdefault(tr['exons'][0][1], []).append(trid)
-            ends.setdefault(tr['exons'][-1][0], []).append(trid)
+            first_junction.setdefault(tr['exons'][0][1], []).append(trid)
+            last_junction.setdefault(tr['exons'][-1][0], []).append(trid)
+        # first / last junction with respect to direction of transcription
         if self.strand == '-':
-            starts, ends = ends, starts
+            first_junction, last_junction = last_junction, first_junction
         # for each site, find consistant "peaks" TSS/PAS
         # if none found use median of all read starts
-        for pos, tr_ids in starts.items():
+        for junction_pos, tr_ids in first_junction.items():
             profile = {}
             for trid in tr_ids:
                 for sa_tss in self.transcripts[trid]['TSS'].values():
                     for pos, c in sa_tss.items():
                         profile[pos] = profile.get(pos, 0)+c
             quantiles = get_quantiles(sorted(profile.items()), [search_range[0], .5, search_range[1]])
             # one/ several peaks within base range? -> quantify by next read_start
@@ -832,21 +839,21 @@
             if not ol_peaks:
                 ol_peaks = [quantiles[1]]
             for trid in tr_ids:
                 tr = self.transcripts[trid]
                 tr['TSS_unified'] = {}
                 for sa, sa_tss in tr['TSS'].items():
                     tss_unified = {}
-                    for pos, c in sa_tss.items():
-                        next_peak = min((p for p in ol_peaks if p < tr['exons'][0][1]),
+                    for pos, c in sa_tss.items():  # for each read start position, find closest peak
+                        next_peak = min((p for p in ol_peaks if cmp_dist(junction_pos, p, min_dist=3) == strand),
                                         default=pos, key=lambda x: abs(x-pos))
                         tss_unified[next_peak] = tss_unified.get(next_peak, 0)+c
                     tr['TSS_unified'][sa] = tss_unified
         # same for PAS
-        for pos, tr_ids in ends.items():
+        for junction_pos, tr_ids in last_junction.items():
             profile = {}
             for trid in tr_ids:
                 for sa_pas in self.transcripts[trid]['PAS'].values():
                     for pos, c in sa_pas.items():
                         profile[pos] = profile.get(pos, 0)+c
             quantiles = get_quantiles(sorted(profile.items()), [search_range[0], .5, search_range[1]])
             # one/ several peaks within base range? -> quantify by next read_start
@@ -856,15 +863,15 @@
                 ol_peaks = [quantiles[1]]
             for trid in tr_ids:
                 tr = self.transcripts[trid]
                 tr['PAS_unified'] = {}
                 for sa, sa_pas in tr['PAS'].items():
                     pas_unified = {}
                     for pos, c in sa_pas.items():
-                        next_peak = min((p for p in ol_peaks if p > tr['exons'][-1][0]),
+                        next_peak = min((p for p in ol_peaks if cmp_dist(p, junction_pos, min_dist=3) == strand),
                                         default=pos, key=lambda x: abs(x-pos))
                         pas_unified[next_peak] = pas_unified.get(next_peak, 0)+c
                     tr['PAS_unified'][sa] = pas_unified
         for tr in self.transcripts:
             # find the most common tss/pas per transcript, and set the exon boundaries
             sum_tss = {}
             sum_pas = {}
```

### Comparing `isotools-0.3.3/src/isotools/plots.py` & `isotools-0.3.4/src/isotools/plots.py`

 * *Files identical despite different names*

### Comparing `isotools-0.3.3/src/isotools/run_isotools.py` & `isotools-0.3.4/src/isotools/run_isotools.py`

 * *Files identical despite different names*

### Comparing `isotools-0.3.3/src/isotools/short_read.py` & `isotools-0.3.4/src/isotools/short_read.py`

 * *Files identical despite different names*

### Comparing `isotools-0.3.3/src/isotools/splice_graph.py` & `isotools-0.3.4/src/isotools/splice_graph.py`

 * *Files identical despite different names*

### Comparing `isotools-0.3.3/src/isotools/transcriptome.py` & `isotools-0.3.4/src/isotools/transcriptome.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,15 +240,15 @@
     from ._transcriptome_io import add_sample_from_bam, add_sample_from_csv, remove_samples, add_short_read_coverage, \
         remove_short_read_coverage, collapse_immune_genes
 
     # IO: output data as tables or other human readable format
     from ._transcriptome_io import gene_table, transcript_table, chimeric_table, write_gtf, export_alternative_splicing
 
     # filtering functionality and iterators
-    from ._transcriptome_filter import add_qc_metrics, add_filter, remove_filter, iter_genes, iter_transcripts, iter_ref_transcripts
+    from ._transcriptome_filter import add_qc_metrics, add_orf_prediction, add_filter, remove_filter, iter_genes, iter_transcripts, iter_ref_transcripts
 
     # statistic: differential splicing, alternative_splicing_events
     from ._transcriptome_stats import die_test, altsplice_test, coordination_test, alternative_splicing_events, rarefaction
 
     # statistic: summary tables (can be used as input to plot_bar / plot_dist)
     from ._transcriptome_stats import altsplice_stats, filter_stats, transcript_length_hist, transcript_coverage_hist,\
         transcripts_per_gene_hist, exons_per_transcript_hist, downstream_a_hist, direct_repeat_hist
```

### Comparing `isotools-0.3.3/src/isotools.egg-info/PKG-INFO` & `isotools-0.3.4/src/isotools.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isotools
-Version: 0.3.3
+Version: 0.3.4
 Summary: Framework for the analysis of long read transcriptome sequencing data
 Home-page: https://github.com/MatthiasLienhard/isotools
 Author: Matthias Lienhard
 Author-email: lienhard@molgen.mpg.de
 Project-URL: Bug Tracker, https://github.com/MatthiasLienhard/isotools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -67,8 +67,8 @@
 isoseq.add_qc_metrics('../tests/data/example.fa')
 isoseq.save('../tests/data/example_1_isotools.pkl')
 ```
 
 ## Citation and feedback:
 * If you run into any issues, please use the [github issues report feature](https://github.com/MatthiasLienhard/isotools/issues).
 * For general feedback, please write me an email to [lienhard@molgen.mpg.de](mailto:lienhard@molgen.mpg.de).
-* If you use isotools in your publication, please cite the following paper: IsoTools: IsoTools: a python toolbox for long-read transcriptome sequencing (in preparation)
+* If you use isotools in your publication, please cite the following [paper](https://doi.org/10.1093/bioinformatics/btad364): Lienhard et al, Bioinformatics, 2023: IsoTools: a flexible workflow for long-read transcriptome sequencing analysis
```

### Comparing `isotools-0.3.3/src/isotools.egg-info/SOURCES.txt` & `isotools-0.3.4/src/isotools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

