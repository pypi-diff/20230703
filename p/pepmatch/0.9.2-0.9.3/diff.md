# Comparing `tmp/pepmatch-0.9.2.tar.gz` & `tmp/pepmatch-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pepmatch-0.9.2.tar", last modified: Fri Jun 23 07:36:29 2023, max compression
+gzip compressed data, was "pepmatch-0.9.3.tar", last modified: Mon Jul  3 06:43:04 2023, max compression
```

## Comparing `pepmatch-0.9.2.tar` & `pepmatch-0.9.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)        0 2023-06-23 07:36:29.343149 pepmatch-0.9.2/
--rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)    11757 2023-03-01 21:01:30.000000 pepmatch-0.9.2/LICENSE
--rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)     4839 2023-06-23 07:36:29.342603 pepmatch-0.9.2/PKG-INFO
--rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)     4508 2023-05-30 05:21:03.000000 pepmatch-0.9.2/README.md
-drwxr-xr-x   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)        0 2023-06-23 07:36:29.334154 pepmatch-0.9.2/pepmatch/
--rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)      207 2023-05-30 05:21:03.000000 pepmatch-0.9.2/pepmatch/__init__.py
--rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)     2096 2023-05-30 05:21:03.000000 pepmatch-0.9.2/pepmatch/benchmarker.py
--rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)     2015 2023-05-30 05:21:03.000000 pepmatch-0.9.2/pepmatch/helpers.py
--rwxr-xr-x   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)    31802 2023-05-30 05:21:03.000000 pepmatch-0.9.2/pepmatch/matcher.py
--rwxr-xr-x   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)    10818 2023-05-30 05:21:03.000000 pepmatch-0.9.2/pepmatch/preprocessor.py
--rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)       22 2023-05-30 05:21:03.000000 pepmatch-0.9.2/pepmatch/version.py
-drwxr-xr-x   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)        0 2023-06-23 07:36:29.338614 pepmatch-0.9.2/pepmatch.egg-info/
--rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)     4839 2023-06-23 07:36:28.000000 pepmatch-0.9.2/pepmatch.egg-info/PKG-INFO
--rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)      486 2023-06-23 07:36:28.000000 pepmatch-0.9.2/pepmatch.egg-info/SOURCES.txt
--rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)        1 2023-06-23 07:36:28.000000 pepmatch-0.9.2/pepmatch.egg-info/dependency_links.txt
--rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)      104 2023-06-23 07:36:28.000000 pepmatch-0.9.2/pepmatch.egg-info/entry_points.txt
--rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)        1 2023-03-03 04:38:29.000000 pepmatch-0.9.2/pepmatch.egg-info/not-zip-safe
--rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)       80 2023-06-23 07:36:28.000000 pepmatch-0.9.2/pepmatch.egg-info/requires.txt
--rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)        9 2023-06-23 07:36:28.000000 pepmatch-0.9.2/pepmatch.egg-info/top_level.txt
--rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)       38 2023-06-23 07:36:29.343323 pepmatch-0.9.2/setup.cfg
--rwxr-xr-x   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)      999 2023-05-30 05:21:03.000000 pepmatch-0.9.2/setup.py
-drwxr-xr-x   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)        0 2023-06-23 07:36:29.341243 pepmatch-0.9.2/test/
--rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)     1769 2023-05-30 05:21:03.000000 pepmatch-0.9.2/test/test_best_match.py
--rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)      569 2023-05-30 05:21:03.000000 pepmatch-0.9.2/test/test_discontinuous_search.py
--rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)     1743 2023-05-30 05:21:03.000000 pepmatch-0.9.2/test/test_exact_match.py
--rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)     1785 2023-05-30 05:21:03.000000 pepmatch-0.9.2/test/test_mismatch.py
+drwxr-xr-x   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)        0 2023-07-03 06:43:04.270998 pepmatch-0.9.3/
+-rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)    11757 2023-03-01 21:01:30.000000 pepmatch-0.9.3/LICENSE
+-rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)     4839 2023-07-03 06:43:04.270619 pepmatch-0.9.3/PKG-INFO
+-rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)     4508 2023-05-30 05:21:03.000000 pepmatch-0.9.3/README.md
+drwxr-xr-x   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)        0 2023-07-03 06:43:04.264990 pepmatch-0.9.3/pepmatch/
+-rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)      207 2023-05-30 05:21:03.000000 pepmatch-0.9.3/pepmatch/__init__.py
+-rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)     2096 2023-05-30 05:21:03.000000 pepmatch-0.9.3/pepmatch/benchmarker.py
+-rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)     2015 2023-05-30 05:21:03.000000 pepmatch-0.9.3/pepmatch/helpers.py
+-rwxr-xr-x   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)    32023 2023-07-03 06:41:59.000000 pepmatch-0.9.3/pepmatch/matcher.py
+-rwxr-xr-x   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)    10818 2023-05-30 05:21:03.000000 pepmatch-0.9.3/pepmatch/preprocessor.py
+-rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)       22 2023-07-03 06:42:22.000000 pepmatch-0.9.3/pepmatch/version.py
+drwxr-xr-x   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)        0 2023-07-03 06:43:04.267766 pepmatch-0.9.3/pepmatch.egg-info/
+-rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)     4839 2023-07-03 06:43:02.000000 pepmatch-0.9.3/pepmatch.egg-info/PKG-INFO
+-rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)      486 2023-07-03 06:43:03.000000 pepmatch-0.9.3/pepmatch.egg-info/SOURCES.txt
+-rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)        1 2023-07-03 06:43:02.000000 pepmatch-0.9.3/pepmatch.egg-info/dependency_links.txt
+-rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)      104 2023-07-03 06:43:02.000000 pepmatch-0.9.3/pepmatch.egg-info/entry_points.txt
+-rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)        1 2023-03-03 04:38:29.000000 pepmatch-0.9.3/pepmatch.egg-info/not-zip-safe
+-rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)       80 2023-07-03 06:43:02.000000 pepmatch-0.9.3/pepmatch.egg-info/requires.txt
+-rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)        9 2023-07-03 06:43:02.000000 pepmatch-0.9.3/pepmatch.egg-info/top_level.txt
+-rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)       38 2023-07-03 06:43:04.271113 pepmatch-0.9.3/setup.cfg
+-rwxr-xr-x   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)      999 2023-05-30 05:21:03.000000 pepmatch-0.9.3/setup.py
+drwxr-xr-x   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)        0 2023-07-03 06:43:04.269865 pepmatch-0.9.3/test/
+-rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)     1769 2023-05-30 05:21:03.000000 pepmatch-0.9.3/test/test_best_match.py
+-rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)      569 2023-05-30 05:21:03.000000 pepmatch-0.9.3/test/test_discontinuous_search.py
+-rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)     1743 2023-05-30 05:21:03.000000 pepmatch-0.9.3/test/test_exact_match.py
+-rw-r--r--   0 dmarrama (2118653919) LIAI_AD\Domain Users (1127120232)     1785 2023-05-30 05:21:03.000000 pepmatch-0.9.3/test/test_mismatch.py
```

### Comparing `pepmatch-0.9.2/LICENSE` & `pepmatch-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pepmatch-0.9.2/PKG-INFO` & `pepmatch-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pepmatch
-Version: 0.9.2
+Version: 0.9.3
 Summary: Search tool for peptides and epitopes within a proteome, while considering potential residue substitutions.
 Home-page: https://github.com/IEDB/PEPMatch
 Author: Daniel Marrama
 Author-email: dmarrama@lji.org
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pepmatch-0.9.2/README.md` & `pepmatch-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `pepmatch-0.9.2/pepmatch/benchmarker.py` & `pepmatch-0.9.3/pepmatch/benchmarker.py`

 * *Files identical despite different names*

### Comparing `pepmatch-0.9.2/pepmatch/helpers.py` & `pepmatch-0.9.3/pepmatch/helpers.py`

 * *Files identical despite different names*

### Comparing `pepmatch-0.9.2/pepmatch/matcher.py` & `pepmatch-0.9.3/pepmatch/matcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,16 @@
                query,
                proteome_file,
                max_mismatches=-1,
                k=0,
                preprocessed_files_path='.',
                best_match=False,
                output_format='csv',
-               output_name=''):
+               output_name='',
+               sequence_version=True):
 
     if k < 0 or k == 1:
       raise ValueError('Invalid k value given. k cannot be negative or 1.')
 
     if output_format not in VALID_OUTPUT_FORMATS:
       raise ValueError(
         'Invalid output format, please choose `dataframe`, '
@@ -65,14 +66,15 @@
     assert self.query or self.discontinuous_epitopes, 'Query is empty.'
     
     self.lengths = sorted(set(len(peptide) for peptide in self.query))
     self.max_mismatches = max_mismatches
     self.preprocessed_files_path = preprocessed_files_path
     self.best_match = best_match
     self.output_format = output_format
+    self.sequence_version = sequence_version
 
     # select format based on # of mismatches to pass to Preprocessor
     # SQLite for exact matching - pickle for mismatching
     self.preprocess_format = 'sql' if not max_mismatches else 'pickle'
     
     # initialize k and k_specified
     if self.query:
@@ -623,29 +625,32 @@
 
         mutated_positions = [
           i+1 for i in range(len(peptide)) if peptide[i] != match[0][i]
         ]
         index_start = int((match[2] % 1000000) + 1)
         index_end = int((match[2] % 1000000) + len(peptide))
 
+        taxon_id = int(metadata[3]) if metadata[3] else np.nan
+        pe_level = int(metadata[5]) if metadata[5] else np.nan
+
         match_data = (
-            peptide,                      # query peptide
-            match[0],                     # matched peptide
-            metadata[0],                  # protein ID
-            metadata[1],                  # protein name
-            metadata[2],                  # species
-            int(metadata[3]),             # taxon ID
-            metadata[4],                  # gene symbol
-            int(match[1]),                # mismatches count
-            mutated_positions,            # mutated positions
-            index_start,                  # index start
-            index_end,                    # index end
-            int(metadata[5]),             # protein existence level
-            metadata[6],                  # sequence version
-            metadata[7]                   # gene priority flag
+          peptide,                      # query peptide
+          match[0],                     # matched peptide
+          metadata[0],                  # protein ID
+          metadata[1],                  # protein name
+          metadata[2],                  # species
+          taxon_id,                     # taxon ID
+          metadata[4],                  # gene symbol
+          int(match[1]),                # mismatches count
+          mutated_positions,            # mutated positions
+          index_start,                  # index start
+          index_end,                    # index end
+          pe_level,                     # protein existence level
+          metadata[6],                  # sequence version
+          metadata[7]                   # gene priority flag
         )
         all_matches.append(match_data)
 
     return all_matches
 
   def best_match_search(self) -> list:
     """After calculating the splits we would need (starting with lowest peptide
@@ -789,19 +794,20 @@
         'Query Sequence', group_keys=False
       ).apply(filter_fragments).reset_index(drop=True)
 
       # sort values by protein ID and drop duplicates, guaranteeing same results 
       df.sort_values(by=['Query Sequence', 'Protein ID', 'Index start'], inplace=True)
       df.drop_duplicates(['Query Sequence'], inplace=True)
 
-    # combine protein ID and sequence version
-    df['Sequence Version'] = df[
-       'Sequence Version'
-    ].apply(lambda x: f'.{int(x)}' if not pd.isna(x) else '')   
-    df['Protein ID'] = df['Protein ID'] + df['Sequence Version']
+    if self.sequence_version:
+      # combine protein ID and sequence version
+      df['Sequence Version'] = df['Sequence Version'].apply(
+        lambda x: f'.{int(x)}' if not pd.isna(x) else ''
+      )   
+      df['Protein ID'] = df['Protein ID'] + df['Sequence Version']
     
     # drop "Sequence Version" and "Gene Priority" columns
     df.drop(columns=['Sequence Version'], inplace=True)
     df.drop(columns=['Gene Priority'], inplace=True)
 
     # force integers on some columns
     int_cols = [
```

### Comparing `pepmatch-0.9.2/pepmatch/preprocessor.py` & `pepmatch-0.9.3/pepmatch/preprocessor.py`

 * *Files identical despite different names*

### Comparing `pepmatch-0.9.2/pepmatch.egg-info/PKG-INFO` & `pepmatch-0.9.3/pepmatch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pepmatch
-Version: 0.9.2
+Version: 0.9.3
 Summary: Search tool for peptides and epitopes within a proteome, while considering potential residue substitutions.
 Home-page: https://github.com/IEDB/PEPMatch
 Author: Daniel Marrama
 Author-email: dmarrama@lji.org
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pepmatch-0.9.2/setup.py` & `pepmatch-0.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `pepmatch-0.9.2/test/test_best_match.py` & `pepmatch-0.9.3/test/test_best_match.py`

 * *Files identical despite different names*

### Comparing `pepmatch-0.9.2/test/test_discontinuous_search.py` & `pepmatch-0.9.3/test/test_discontinuous_search.py`

 * *Files identical despite different names*

### Comparing `pepmatch-0.9.2/test/test_exact_match.py` & `pepmatch-0.9.3/test/test_exact_match.py`

 * *Files identical despite different names*

### Comparing `pepmatch-0.9.2/test/test_mismatch.py` & `pepmatch-0.9.3/test/test_mismatch.py`

 * *Files identical despite different names*

