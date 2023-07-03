# Comparing `tmp/pyswcloader-1.0.1-py2.py3-none-any.whl.zip` & `tmp/pyswcloader-1.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,19 @@
-Zip file size: 10906 bytes, number of entries: 13
--rw-rw-r--  2.0 unx      334 b- defN 22-Dec-08 05:04 pyswcloader/__init__.py
+Zip file size: 59133 bytes, number of entries: 17
+-rw-rw-r--  2.0 unx      366 b- defN 23-Jul-01 08:37 pyswcloader/__init__.py
 -rw-rw-r--  2.0 unx     2385 b- defN 23-Mar-06 01:56 pyswcloader/brain.py
 -rw-rw-r--  2.0 unx     2657 b- defN 23-Jan-31 03:26 pyswcloader/cluster.py
--rw-rw-r--  2.0 unx     2890 b- defN 22-Dec-14 04:27 pyswcloader/distance.py
--rw-rw-r--  2.0 unx     8294 b- defN 23-Jan-28 03:41 pyswcloader/projection.py
--rw-rw-r--  2.0 unx     3500 b- defN 23-Mar-14 02:44 pyswcloader/projection_batch.py
--rw-rw-r--  2.0 unx     6771 b- defN 23-Feb-10 08:53 pyswcloader/swc.py
+-rw-rw-r--  2.0 unx     2890 b- defN 23-Jun-30 07:10 pyswcloader/distance.py
+-rw-rw-r--  2.0 unx      605 b- defN 23-Jul-03 04:46 pyswcloader/io.py
+-rw-rw-r--  2.0 unx     8946 b- defN 23-Jun-30 04:41 pyswcloader/projection.py
+-rw-rw-r--  2.0 unx     3477 b- defN 23-Jun-30 04:46 pyswcloader/projection_batch.py
+-rw-rw-r--  2.0 unx     7419 b- defN 23-Jul-01 08:37 pyswcloader/swc.py
 -rw-rw-r--  2.0 unx     3432 b- defN 23-Jan-31 08:00 pyswcloader/visualization.py
--rw-rw-r--  2.0 unx     1062 b- defN 23-Mar-14 02:46 pyswcloader-1.0.1.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx      563 b- defN 23-Mar-14 02:46 pyswcloader-1.0.1.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-Mar-14 02:46 pyswcloader-1.0.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       81 b- defN 23-Mar-14 02:46 pyswcloader-1.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1055 b- defN 23-Mar-14 02:46 pyswcloader-1.0.1.dist-info/RECORD
-13 files, 33134 bytes uncompressed, 9150 bytes compressed:  72.4%
+-rw-rw-r--  2.0 unx    13691 b- defN 23-Jan-28 06:56 pyswcloader/database/acro_stl_dict.pkl
+-rw-rw-r--  2.0 unx   146754 b- defN 23-Feb-14 05:50 pyswcloader/database/allen_brain_tree.pkl
+-rwxr-xr-x  2.0 unx    13691 b- defN 23-Jan-28 06:54 pyswcloader/database/stl_acro_dict.pkl
+-rw-rw-r--  2.0 unx     1062 b- defN 23-Jul-03 04:46 pyswcloader-1.1.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx      750 b- defN 23-Jul-03 04:46 pyswcloader-1.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-Jul-03 04:46 pyswcloader-1.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       81 b- defN 23-Jul-03 04:46 pyswcloader-1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1410 b- defN 23-Jul-03 04:46 pyswcloader-1.1.dist-info/RECORD
+17 files, 209726 bytes uncompressed, 56825 bytes compressed:  72.9%
```

## zipnote {}

```diff
@@ -6,35 +6,47 @@
 
 Filename: pyswcloader/cluster.py
 Comment: 
 
 Filename: pyswcloader/distance.py
 Comment: 
 
+Filename: pyswcloader/io.py
+Comment: 
+
 Filename: pyswcloader/projection.py
 Comment: 
 
 Filename: pyswcloader/projection_batch.py
 Comment: 
 
 Filename: pyswcloader/swc.py
 Comment: 
 
 Filename: pyswcloader/visualization.py
 Comment: 
 
-Filename: pyswcloader-1.0.1.dist-info/LICENSE.txt
+Filename: pyswcloader/database/acro_stl_dict.pkl
+Comment: 
+
+Filename: pyswcloader/database/allen_brain_tree.pkl
+Comment: 
+
+Filename: pyswcloader/database/stl_acro_dict.pkl
+Comment: 
+
+Filename: pyswcloader-1.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: pyswcloader-1.0.1.dist-info/METADATA
+Filename: pyswcloader-1.1.dist-info/METADATA
 Comment: 
 
-Filename: pyswcloader-1.0.1.dist-info/WHEEL
+Filename: pyswcloader-1.1.dist-info/WHEEL
 Comment: 
 
-Filename: pyswcloader-1.0.1.dist-info/top_level.txt
+Filename: pyswcloader-1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: pyswcloader-1.0.1.dist-info/RECORD
+Filename: pyswcloader-1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyswcloader/__init__.py

```diff
@@ -1,16 +1,18 @@
 import pyswcloader.swc
 import pyswcloader.brain
 import pyswcloader.projection
 import pyswcloader.projection_batch
 import pyswcloader.distance
 import pyswcloader.cluster
 import pyswcloader.visualization
+import pyswcloader.io
 
 __all__ = [
+    'io',
     'swc',
     'brain',
     'projection',
     'projection_batch',
     'distance',
     'cluster',
     'visualization',
```

## pyswcloader/projection.py

```diff
@@ -13,19 +13,22 @@
     length = length.fillna(0)
     data = swc.swc_preprocess(data_path)
     data['region'] = data.apply(lambda x: brain.find_region(x[['x','y','z']], annotation, resolution), axis=1)
     for idx in data.index[1:]:
         reg = data.loc[idx, 'region']
         parent_idx = data.loc[idx, 'parent']
         parent_reg = data.loc[parent_idx, 'region']
-        if reg==parent_reg:
-            length.loc[neuron_name, reg] += math.dist(data.loc[idx, 'x':'z'], data.loc[parent_idx, 'x':'z'])
-        else:
-            length.loc[neuron_name, reg] += math.dist(data.loc[idx, 'x':'z'], data.loc[parent_idx, 'x':'z'])/2
-            length.loc[neuron_name, parent_reg] += math.dist(data.loc[idx, 'x':'z'], data.loc[parent_idx, 'x':'z'])/2
+        _is_axon = data.loc[idx, 'type']
+        _parent_is_axon = data.loc[parent_idx, 'type']
+        if _is_axon not in [3, 4] and _parent_is_axon not in [3, 4]:
+            if reg==parent_reg:
+                length.loc[neuron_name, reg] += math.dist(data.loc[idx, 'x':'z'], data.loc[parent_idx, 'x':'z'])
+            else:
+                length.loc[neuron_name, reg] += math.dist(data.loc[idx, 'x':'z'], data.loc[parent_idx, 'x':'z'])/2
+                length.loc[neuron_name, parent_reg] += math.dist(data.loc[idx, 'x':'z'], data.loc[parent_idx, 'x':'z'])/2
     if 0 in length.columns:
         length = length.drop(columns=0)
     if save == True:
         length.to_csv(os.path.join(save_path, neuron_name+'_projection_length.csv'))
     return length
 
 def projection_length_ipsi(data_path, annotation, resolution, save=False, save_path=os.getcwd()):
@@ -40,26 +43,29 @@
     data['ipsi'] = [(item<mid)==mark for item in data.z]
     for idx in data.index[1:]:
         reg = data.loc[idx, 'region']
         ipsi = data.loc[idx, 'ipsi']
         parent_idx = data.loc[idx, 'parent']
         parent_reg = data.loc[parent_idx, 'region']
         parent_ipsi = data.loc[parent_idx, 'ipsi']
-        if ipsi==parent_ipsi and ipsi==True:
-            if reg==parent_reg:
-                length.loc[neuron_name, reg] += math.dist(data.loc[idx, 'x':'z'], data.loc[parent_idx, 'x':'z'])
-            else:
-                length.loc[neuron_name, reg] += math.dist(data.loc[idx, 'x':'z'], data.loc[parent_idx, 'x':'z'])/2
-                length.loc[neuron_name, parent_reg] += math.dist(data.loc[idx, 'x':'z'], data.loc[parent_idx, 'x':'z'])/2
-        elif ipsi != parent_ipsi:
-            if reg==parent_reg:
-                length.loc[neuron_name, reg] += math.dist(data.loc[idx, 'x':'z'], data.loc[parent_idx, 'x':'z'])/2
-            else:
-                length.loc[neuron_name, reg] += math.dist(data.loc[idx, 'x':'z'], data.loc[parent_idx, 'x':'z'])/4
-                length.loc[neuron_name, parent_reg] += math.dist(data.loc[idx, 'x':'z'], data.loc[parent_idx, 'x':'z'])/4
+        _is_axon = data.loc[idx, 'type']
+        _parent_is_axon = data.loc[parent_idx, 'type']
+        if _is_axon not in [3, 4] and _parent_is_axon not in [3, 4]:
+            if ipsi==parent_ipsi and ipsi==True:
+                if reg==parent_reg:
+                    length.loc[neuron_name, reg] += math.dist(data.loc[idx, 'x':'z'], data.loc[parent_idx, 'x':'z'])
+                else:
+                    length.loc[neuron_name, reg] += math.dist(data.loc[idx, 'x':'z'], data.loc[parent_idx, 'x':'z'])/2
+                    length.loc[neuron_name, parent_reg] += math.dist(data.loc[idx, 'x':'z'], data.loc[parent_idx, 'x':'z'])/2
+            elif ipsi != parent_ipsi:
+                if reg==parent_reg:
+                    length.loc[neuron_name, reg] += math.dist(data.loc[idx, 'x':'z'], data.loc[parent_idx, 'x':'z'])/2
+                else:
+                    length.loc[neuron_name, reg] += math.dist(data.loc[idx, 'x':'z'], data.loc[parent_idx, 'x':'z'])/4
+                    length.loc[neuron_name, parent_reg] += math.dist(data.loc[idx, 'x':'z'], data.loc[parent_idx, 'x':'z'])/4
     if 0 in length.columns:
         length = length.drop(columns=0)
     if save == True:
         length.to_csv(os.path.join(save_path, neuron_name+'_projection_length_ipsi.csv'))
     return length
 
 def projection_length_contra(data_path, annotation, resolution, save=False, save_path=os.getcwd()):
@@ -74,40 +80,44 @@
     data['ipsi'] = [(item<mid)==mark for item in data.z]
     for idx in data.index[1:]:
         reg = data.loc[idx, 'region']
         ipsi = data.loc[idx, 'ipsi']
         parent_idx = data.loc[idx, 'parent']
         parent_reg = data.loc[parent_idx, 'region']
         parent_ipsi = data.loc[parent_idx, 'ipsi']
-        if ipsi==parent_ipsi and ipsi==False:
-            if reg==parent_reg:
-                length.loc[neuron_name, reg] += math.dist(data.loc[idx, 'x':'z'], data.loc[parent_idx, 'x':'z'])
-            else:
-                length.loc[neuron_name, reg] += math.dist(data.loc[idx, 'x':'z'], data.loc[parent_idx, 'x':'z'])/2
-                length.loc[neuron_name, parent_reg] += math.dist(data.loc[idx, 'x':'z'], data.loc[parent_idx, 'x':'z'])/2
-        elif ipsi != parent_ipsi:
-            if reg==parent_reg:
-                length.loc[neuron_name, reg] += math.dist(data.loc[idx, 'x':'z'], data.loc[parent_idx, 'x':'z'])/2
-            else:
-                length.loc[neuron_name, reg] += math.dist(data.loc[idx, 'x':'z'], data.loc[parent_idx, 'x':'z'])/4
-                length.loc[neuron_name, parent_reg] += math.dist(data.loc[idx, 'x':'z'], data.loc[parent_idx, 'x':'z'])/4
+        _is_axon = data.loc[idx, 'type']
+        _parent_is_axon = data.loc[parent_idx, 'type']
+        if _is_axon not in [3, 4] and _parent_is_axon not in [3, 4]:
+            if ipsi==parent_ipsi and ipsi==False:
+                if reg==parent_reg:
+                    length.loc[neuron_name, reg] += math.dist(data.loc[idx, 'x':'z'], data.loc[parent_idx, 'x':'z'])
+                else:
+                    length.loc[neuron_name, reg] += math.dist(data.loc[idx, 'x':'z'], data.loc[parent_idx, 'x':'z'])/2
+                    length.loc[neuron_name, parent_reg] += math.dist(data.loc[idx, 'x':'z'], data.loc[parent_idx, 'x':'z'])/2
+            elif ipsi != parent_ipsi:
+                if reg==parent_reg:
+                    length.loc[neuron_name, reg] += math.dist(data.loc[idx, 'x':'z'], data.loc[parent_idx, 'x':'z'])/2
+                else:
+                    length.loc[neuron_name, reg] += math.dist(data.loc[idx, 'x':'z'], data.loc[parent_idx, 'x':'z'])/4
+                    length.loc[neuron_name, parent_reg] += math.dist(data.loc[idx, 'x':'z'], data.loc[parent_idx, 'x':'z'])/4
     if 0 in length.columns:
         length = length.drop(columns=0)
     if save == True:
         length.to_csv(os.path.join(save_path, neuron_name+'_projection_length_contra.csv'))
     return length
 
 def terminal_info(data_path, save=False, save_path=os.getcwd()):
     neuron_name = data_path.split('/')[-1].split('.')[0]
     data = swc.swc_preprocess(data_path)
     tree = swc.swc_tree(data_path)
     terminal_list = []
     for item in tree.filter_nodes(lambda x: x.is_leaf()):
         terminal_list.append(item.identifier)
     info = data.loc[data.id.isin(terminal_list)]
+    info = info[~info.type.isin([3, 4])]
     if save == True:
         info.to_csv(os.path.join(save_path, neuron_name+'_terminal_info.csv'))
     return info
 
 def terminal_count(data_path, annotation, resolution, save=False, save_path=os.getcwd()):
     neuron_name = data_path.split('/')[-1].split('.')[0]
     info = terminal_info(data_path)
```

## pyswcloader/projection_batch.py

```diff
@@ -8,72 +8,72 @@
 from . import projection
 from . import swc
 
 def projection_length(data_path, annotation, resolution, cores=int(cpu_count()/2), save_state=False, save_path=os.getcwd()):
     path_list = swc.read_neuron_path(data_path)
     length = pd.DataFrame()
     pool = Pool(cores)
-    length = length.append(pool.map(partial(projection.projection_length, annotation=annotation, resolution=resolution, save=save_state, save_path=save_path), tqdm(path_list)))
+    length = pd.concat(pool.map(partial(projection.projection_length, annotation=annotation, resolution=resolution, save=save_state, save_path=save_path), tqdm(path_list)))
     pool.close()
     pool.join()
     return length
 
 def projection_length_ipsi(data_path, annotation, resolution, cores=int(cpu_count()/2), save_state=False, save_path=os.getcwd()):
     path_list = swc.read_neuron_path(data_path)
     length = pd.DataFrame()
     pool = Pool(cores)
-    length = length.append(pool.map(partial(projection.projection_length_ipsi, annotation=annotation, resolution=resolution, save=save_state, save_path=save_path), tqdm(path_list)))
+    length = pd.concat(pool.map(partial(projection.projection_length_ipsi, annotation=annotation, resolution=resolution, save=save_state, save_path=save_path), tqdm(path_list)))
     pool.close()
     pool.join()
     return length
 
 def projection_length_contra(data_path, annotation, resolution, cores=int(cpu_count()/2), save_state=False, save_path=os.getcwd()):
     path_list = swc.read_neuron_path(data_path)
     length = pd.DataFrame()
     pool = Pool(cores)
-    length = length.append(pool.map(partial(projection.projection_length_contra, annotation=annotation, resolution=resolution, save=save_state, save_path=save_path), tqdm(path_list)))
+    length = pd.concat(pool.map(partial(projection.projection_length_contra, annotation=annotation, resolution=resolution, save=save_state, save_path=save_path), tqdm(path_list)))
     pool.close()
     pool.join()
     return length
 
 def _terminal_info(path, save_state, save_path):
     info = projection.terminal_info(path, save=save_state, save_path=save_path)
     info['neuron'] = os.path.basename(path).split('.')[0]
     return info
 
 def terminal_info(data_path, cores=int(cpu_count()/2), save_state=False, save_path=os.getcwd()):
     path_list = swc.read_neuron_path(data_path)
     info = pd.DataFrame()
     pool = Pool(cores)
-    info = info.append(pool.map(partial(_terminal_info, save_state=save_state, save_path=save_path), tqdm(path_list)))
+    info = pd.concat(pool.map(partial(_terminal_info, save_state=save_state, save_path=save_path), tqdm(path_list)))
     pool.close()
     pool.join()
     return info
 
 def terminal_count(data_path, annotation, resolution, cores=int(cpu_count()/2), save_state=False, save_path=os.getcwd()):
     path_list = swc.read_neuron_path(data_path)
     count = pd.DataFrame()
     pool = Pool(cores)
-    count = count.append(pool.map(partial(projection.terminal_count, annotation=annotation, resolution=resolution, save=save_state, save_path=save_path), tqdm(path_list)))
+    count = pd.concat(pool.map(partial(projection.terminal_count, annotation=annotation, resolution=resolution, save=save_state, save_path=save_path), tqdm(path_list)))
     pool.close()
     pool.join()
     return count
 
 def terminal_count_ipsi(data_path, annotation, resolution, cores=int(cpu_count()/2), save_state=False, save_path=os.getcwd()):
     path_list = swc.read_neuron_path(data_path)
     count = pd.DataFrame()
     pool = Pool(cores)
-    count = count.append(pool.map(partial(projection.terminal_count_ipsi, annotation=annotation, resolution=resolution, save=save_state, save_path=save_path), tqdm(path_list)))
+    count = pd.concat(pool.map(partial(projection.terminal_count_ipsi, annotation=annotation, resolution=resolution, save=save_state, save_path=save_path), tqdm(path_list)))
     pool.close()
     pool.join()
     return count
 
 def terminal_count_contra(data_path, annotation, resolution, cores=int(cpu_count()/2), save_state=False, save_path=os.getcwd()):
     path_list = swc.read_neuron_path(data_path)
     count = pd.DataFrame()
     pool = Pool(cores)
-    count = count.append(pool.map(partial(projection.terminal_count_contra, annotation=annotation, resolution=resolution, save=save_state, save_path=save_path), tqdm(path_list)))
+    count = pd.concat(pool.map(partial(projection.terminal_count_contra, annotation=annotation, resolution=resolution, save=save_state, save_path=save_path), tqdm(path_list)))
     pool.close()
     pool.join()
     return count
```

## pyswcloader/swc.py

```diff
@@ -16,28 +16,40 @@
     data = pd.read_csv(path, sep=' ', header=None, comment='#')
     data.columns = ['id', 'type', 'x', 'y', 'z', 'radius', 'parent']
     data.index = np.arange(1, len(data)+1)
     return data
 
 def swc_preprocess(path, save_path=None, save=False, check_validity=True, flip=True, dimension=[13200, 8000, 11400]):
     data = read_swc(path)
+
     if flip==True and float(data.loc[1, 'z'])>(11400/2):
         data.z = dimension[2] - data.z
+
     if check_validity==True:
-        if len(data.loc[data.parent==-1])>1 or len(data.loc[data.type==1])>1:
-            raise Exception('More than one soma detected.')
+        if len(data.loc[data.parent==-1])>1:
+            print(path + ': more than one soma detected -> parent=-1.')
+            child_list = list(data.loc[data.parent==-1].index[1:])
+            while len(child_list)>0:
+                data = data.loc[~data.index.isin(child_list), :]
+                child_list = list(data[data.parent.isin(child_list)].index)
+
+        elif len(data.loc[data.type==1])>1:
+            print(path + ': more than one soma detected -> type=1.')
+            data.loc[data[data.type==1].index[1:],'type'] = 0
+
     if data.x.max()>dimension[0]:
         data.x = [item if item<dimension[0] else dimension[0]-1 for item in data.x]
         print('X axis exceeds boundary.')
     if data.y.max()>dimension[1]:
         data.y = [item if item<dimension[1] else dimension[1]-1 for item in data.y]
         print('Y axis exceeds boundary.')
     if data.z.max()>dimension[2]:
         data.z = [item if item<dimension[2] else dimension[2]-1 for item in data.z]
         print('Z axis exceeds boundary.')    
+
     if save==True:
         data.to_csv(save_path, sep=" ", header=None, index=None)
     return data
 
 def swc_tree(path):
     tree = Tree()
     data = read_swc(path)
@@ -51,15 +63,18 @@
     return tree
 
 def total_length(path):
     length = 0
     data = read_swc(path)
     for idx in data.index[1:]:
         parent_idx = data.loc[idx, 'parent']
-        length += math.dist(data.loc[idx, 'x':'z'], data.loc[parent_idx, 'x':'z'])
+        _is_axon = data.loc[idx, 'type']
+        _parent_is_axon = data.loc[parent_idx, 'type']
+        if _is_axon not in [3, 4] and _parent_is_axon not in [3, 4]:
+            length += math.dist(data.loc[idx, 'x':'z'], data.loc[parent_idx, 'x':'z'])
     return length
 
 def find_longest_stem(path):
     tree = swc_tree(path)
     weight_dict = {}
     for node in list(tree.nodes.keys())[1:]:
         weight_dict[node] = math.dist(tree.nodes[node].data.values(), tree.parent(node).data.values())
@@ -162,15 +177,16 @@
     return path_list
 
 def plot_soma_distribution(data_path, **kwargs):
     path_list = read_neuron_path(data_path)
     soma_info = pd.DataFrame()
     for path in tqdm(path_list):
         data = read_swc(path)
-        soma_info = soma_info.append(data.loc[1, 'x':'z'])
+        # soma_info = soma_info.append(data.loc[1, 'x':'z'])
+        soma_info = pd.concat([soma_info, data.loc[1, 'x':'z']], axis=0)
     fig, _ = plt.subplots(nrows=3, sharex=False, sharey=False)
     cnt = 1
     for axis in ['x', 'y', 'z']:
         plt.subplot(310+cnt)
         sns.kdeplot(list(soma_info[axis]), **kwargs)
         plt.ylabel('')
         ax = plt.gca()
```

## Comparing `pyswcloader-1.0.1.dist-info/LICENSE.txt` & `pyswcloader-1.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `pyswcloader-1.0.1.dist-info/METADATA` & `pyswcloader-1.1.dist-info/METADATA`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyswcloader
-Version: 1.0.1
+Version: 1.1
 Summary: analysis tool for neuron swc files
 Home-page: https://github.com/txgxxx/pyswcloader/
 Author: tsgao
 Author-email: gaots@ion.ac.cn
 License: MIT
 Keywords: swc
 License-File: LICENSE.txt
@@ -19,7 +19,10 @@
 Requires-Dist: kaleido
 Requires-Dist: glob2
 Requires-Dist: scikit-learn
 Requires-Dist: statistics
 Requires-Dist: scipy
 Requires-Dist: rdp
 
+This library is built for single-cell clustering based on neuron morphology and projection analysis.
+
+For source code and tutorials, please refer to: https://github.com/txgxxx/pyswcloader.
```

## Comparing `pyswcloader-1.0.1.dist-info/RECORD` & `pyswcloader-1.1.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,17 @@
-pyswcloader/__init__.py,sha256=jVe6ECQ7hZjM413wllQx2qllkAdifqY7UbLNV5r5I74,334
+pyswcloader/__init__.py,sha256=Nz1BR_F2HPd3IFEDljR7hpJaaX6TaZC1QTa0g8YeBB8,366
 pyswcloader/brain.py,sha256=8dMkpBVJ5niYRbPMKQi31pprX9K2igLMY9dCaZMjzhE,2385
 pyswcloader/cluster.py,sha256=rtkrQfufpk2BaVohQ20-rmiZdd_I3WKLtQ7f4vpsJlo,2657
 pyswcloader/distance.py,sha256=-UFgLcB81xtY2ADVq72L6Ilgfid-kDGl1GCM9-JNoAw,2890
-pyswcloader/projection.py,sha256=sffOEL-cU6_RxHsIHJia7rnunc-BYn2qMwx0r1Wqdh0,8294
-pyswcloader/projection_batch.py,sha256=hYBFmbfTlGe2OsCir846K03IFEU1nkNaJtT769ZUOBk,3500
-pyswcloader/swc.py,sha256=1yYHoG5r9df4sBNeowKFQaWEDl3SvHGja_3mDKqHn5k,6771
+pyswcloader/io.py,sha256=altOMmP1IXyMAbaUz1aINcyx23GzU8UYn_LG_5RlZrA,605
+pyswcloader/projection.py,sha256=gUEH5XYAMk9MEajz0PneYAVNwVjExLi8I5USdvt0CoA,8946
+pyswcloader/projection_batch.py,sha256=juqPKzl_HgcdKreBjzKBLJ9m6cr5LkzdUDRweVeIqs0,3477
+pyswcloader/swc.py,sha256=W71B-JCXnt_YCdvZEiREj-oA31vlFE0DUNEN8X7kHCI,7419
 pyswcloader/visualization.py,sha256=HONADF3oio27vuYfqfPFQqmc_gUkOuc8wExW4SeQ-rs,3432
-pyswcloader-1.0.1.dist-info/LICENSE.txt,sha256=kD2oe1i9Gq8wK3bMbliBamRR_hKEKImWBzZISNov6os,1062
-pyswcloader-1.0.1.dist-info/METADATA,sha256=ggYBpZl_RU8qEJQz-mFOreVPdGo_xjaNLRVyZBR9xpI,563
-pyswcloader-1.0.1.dist-info/WHEEL,sha256=Z-nyYpwrcSqxfdux5Mbn_DQ525iP7J2DG3JgGvOYyTQ,110
-pyswcloader-1.0.1.dist-info/top_level.txt,sha256=E3iDEX_8GHBgmTqDgo7zwYTv2lagnVFAnorZBnOc6yc,81
-pyswcloader-1.0.1.dist-info/RECORD,,
+pyswcloader/database/acro_stl_dict.pkl,sha256=7MMt4HK-IXAM-AGkmv2_gXaWw8DvYJXaoptZrqJk6d0,13691
+pyswcloader/database/allen_brain_tree.pkl,sha256=Hrw7rt-LmvDkvH7i20YXttzozEY12hbPiEvKn1plcnM,146754
+pyswcloader/database/stl_acro_dict.pkl,sha256=A9IJP2lZIO-P-hconjDS2R1WgKjHily9Gd8j9pYircA,13691
+pyswcloader-1.1.dist-info/LICENSE.txt,sha256=kD2oe1i9Gq8wK3bMbliBamRR_hKEKImWBzZISNov6os,1062
+pyswcloader-1.1.dist-info/METADATA,sha256=kqYBOct0bSzqh3hSnSFHt4ZCZDHiXwKtSCwN-GbPtII,750
+pyswcloader-1.1.dist-info/WHEEL,sha256=Z-nyYpwrcSqxfdux5Mbn_DQ525iP7J2DG3JgGvOYyTQ,110
+pyswcloader-1.1.dist-info/top_level.txt,sha256=E3iDEX_8GHBgmTqDgo7zwYTv2lagnVFAnorZBnOc6yc,81
+pyswcloader-1.1.dist-info/RECORD,,
```

