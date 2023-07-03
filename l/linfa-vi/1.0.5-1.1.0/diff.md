# Comparing `tmp/linfa_vi-1.0.5.tar.gz` & `tmp/linfa_vi-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linfa_vi-1.0.5.tar", last modified: Sat Jul  1 20:32:28 2023, max compression
+gzip compressed data, was "linfa_vi-1.1.0.tar", last modified: Mon Jul  3 16:17:20 2023, max compression
```

## Comparing `linfa_vi-1.0.5.tar` & `linfa_vi-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:32:28.572410 linfa_vi-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-01 20:32:14.000000 linfa_vi-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-07-01 20:32:28.572410 linfa_vi-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-07-01 20:32:14.000000 linfa_vi-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:32:28.568410 linfa_vi-1.0.5/linfa/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-01 20:32:14.000000 linfa_vi-1.0.5/linfa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13040 2023-07-01 20:32:14.000000 linfa_vi-1.0.5/linfa/maf.py
--rw-r--r--   0 runner    (1001) docker     (123)    13517 2023-07-01 20:32:14.000000 linfa_vi-1.0.5/linfa/nofas.py
--rw-r--r--   0 runner    (1001) docker     (123)    13555 2023-07-01 20:32:14.000000 linfa_vi-1.0.5/linfa/run_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-07-01 20:32:14.000000 linfa_vi-1.0.5/linfa/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:32:28.568410 linfa_vi-1.0.5/linfa_vi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-07-01 20:32:28.000000 linfa_vi-1.0.5/linfa_vi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-01 20:32:28.000000 linfa_vi-1.0.5/linfa_vi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 20:32:28.000000 linfa_vi-1.0.5/linfa_vi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-01 20:32:28.000000 linfa_vi-1.0.5/linfa_vi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-01 20:32:28.000000 linfa_vi-1.0.5/linfa_vi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-01 20:32:14.000000 linfa_vi-1.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 20:32:28.572410 linfa_vi-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 20:32:14.000000 linfa_vi-1.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 20:32:28.572410 linfa_vi-1.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    30715 2023-07-01 20:32:14.000000 linfa_vi-1.0.5/tests/test_linfa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:17:20.894684 linfa_vi-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-03 16:17:06.000000 linfa_vi-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-07-03 16:17:20.890684 linfa_vi-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-07-03 16:17:06.000000 linfa_vi-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:17:20.890684 linfa_vi-1.1.0/linfa/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 16:17:06.000000 linfa_vi-1.1.0/linfa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13040 2023-07-03 16:17:06.000000 linfa_vi-1.1.0/linfa/maf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13731 2023-07-03 16:17:06.000000 linfa_vi-1.1.0/linfa/nofas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-07-03 16:17:06.000000 linfa_vi-1.1.0/linfa/plot_res.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14014 2023-07-03 16:17:06.000000 linfa_vi-1.1.0/linfa/run_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-07-03 16:17:06.000000 linfa_vi-1.1.0/linfa/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:17:20.890684 linfa_vi-1.1.0/linfa_vi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6505 2023-07-03 16:17:20.000000 linfa_vi-1.1.0/linfa_vi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-03 16:17:20.000000 linfa_vi-1.1.0/linfa_vi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 16:17:20.000000 linfa_vi-1.1.0/linfa_vi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-03 16:17:20.000000 linfa_vi-1.1.0/linfa_vi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-03 16:17:20.000000 linfa_vi-1.1.0/linfa_vi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-03 16:17:06.000000 linfa_vi-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 16:17:20.894684 linfa_vi-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 16:17:06.000000 linfa_vi-1.1.0/setup.py
```

### Comparing `linfa_vi-1.0.5/LICENSE` & `linfa_vi-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.0.5/PKG-INFO` & `linfa_vi-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linfa_vi
-Version: 1.0.5
+Version: 1.1.0
 Summary: A Python library for inference with normalizing flow and annealing
 Author-email: resDesLab  <daniele.schiavazzi@gmail.com>
 License: Copyright © 2023 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `linfa_vi-1.0.5/README.md` & `linfa_vi-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.0.5/linfa/maf.py` & `linfa_vi-1.1.0/linfa/maf.py`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.0.5/linfa/nofas.py` & `linfa_vi-1.1.0/linfa/nofas.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,19 +44,20 @@
             input_size (int): input dimension of true model.
             output_size (int): output dimension of true model.
             limits (list or lists): bounds for all inputs, in format of [[low_0, high_0], [low_1, high_1], ... ]
             memory_len (int): the maximal number of batches stored in buffer. Default: 20
             surrogate (None or torch.nn.Module): the implementation of surrogate model used. Default: FNN
 
     """
-    def __init__(self, model_name, model_func, input_size, output_size, limits=None, memory_len=20, surrogate=None, device='cpu'):
+    def __init__(self, model_name, model_func, input_size, output_size, model_folder='./', limits=None, memory_len=20, surrogate=None, device='cpu'):
         self.device = device
         self.input_size = input_size
         self.output_size = output_size
         self.model_name = model_name
+        self.model_folder = model_folder
         self.mf = model_func
         self.pre_out = None
         self.m = None
         self.sd = None
         self.tm = None
         self.tsd = None
         self.limits = limits
@@ -112,21 +113,21 @@
             pre_grid (None or torch.Tensor): Specifies a matrix of model inputs with size [data_num, feature_dim]. If None, will try to search for *npz* containing this info.
 
         Returns:
             None
 
         """
         if pre_grid is None:
-            if path.exists(self.model_name + '.npz'):
-                container = np.load(self.model_name + '.npz')
+            if path.exists(self.model_folder + self.model_name + '.npz'):
+                container = np.load(self.model_folder + self.model_name + '.npz')
                 if 'pre_grid' in container:
                     self.pre_grid = container['pre_grid']
                     print("Success: Pre-Grid found.")
             else:
-                print("Warning: " + self.model_name + ".npz does not found, please generate pre-grid.")
+                print("Warning: " + self.model_folder + self.model_name + ".npz does not found, please generate pre-grid.")
                 print("Suggestion: Use Surrogate.gen_grid(input_limits=None, grid_num=5, store=True)")
         else:
             self.__pre_grid = torch.Tensor(pre_grid).to(self.device)
             self.m = torch.mean(self.pre_grid, 0)
             self.sd = torch.std(self.pre_grid, 0)
             # Evaluate model at pre-grid
             self.pre_out = self.mf(self.pre_grid)
@@ -149,15 +150,15 @@
           
             meshpoints = []
             if input_limits is not None:
                 self.limits = input_limits
                 print("Warning: Input limits recorded in surrogate.")
 
             for lim in self.limits: meshpoints.append(torch.linspace(lim[0], lim[1], steps=gridnum))
-            grid = torch.meshgrid(meshpoints)
+            grid = torch.meshgrid(meshpoints,indexing='ij')
             grid = torch.cat([item.reshape(gridnum ** len(self.limits), 1) for item in grid], 1)
 
         elif (grid_type == 'sobol'):
 
             # Generate sobol samples in [0,1]^d
             soboleng = torch.quasirandom.SobolEngine(dimension=len(self.limits))
             grid = soboleng.draw(gridnum)
@@ -181,26 +182,26 @@
     def surrogate_save(self):
         """Save surrogate model to [self.name].sur and [self.name].npz
         
         Returns:
             None
 
         """
-        torch.save(self.surrogate.state_dict(), self.model_name + '.sur')
-        np.savez(self.model_name, limits=self.limits, pre_grid=self.pre_grid.clone().cpu().numpy(),
+        torch.save(self.surrogate.state_dict(), self.model_folder + self.model_name + '.sur')
+        np.savez(self.model_folder + self.model_name, limits=self.limits, pre_grid=self.pre_grid.clone().cpu().numpy(),
                  grid_record=self.grid_record.clone().cpu().numpy())
 
     def surrogate_load(self):
         """Load surrogate model from [self.name].sur and [self.name].npz
         
         Returns:
             None
         """
-        self.surrogate.load_state_dict(torch.load(self.model_name + '.sur'))
-        container = np.load(self.model_name + '.npz')
+        self.surrogate.load_state_dict(torch.load(self.model_folder + self.model_name + '.sur'))
+        container = np.load(self.model_folder + self.model_name + '.npz')
         for key in container:
             try:
                 setattr(self, key, torch.Tensor(container[key]))
                 print("Success: [" + key + "] loaded.")
             except:
                 print("Warning: [" + key + "] is not a surrogate variables.")
```

### Comparing `linfa_vi-1.0.5/linfa/run_experiment.py` & `linfa_vi-1.1.0/linfa/run_experiment.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,16 @@
         self.run_nofas          = True  #:bool:   Activate NoFAS and the use of a surrogate model
         self.log_interval       = 10    #:int:    How often the loss statistics are printed
         self.calibrate_interval = 300   #:int:    How often the surrogate model is updated
         self.true_data_num      = 2     #:double: Number of true model evaluated at each surrogate update
         self.budget             = 216   #:int:    Maximum number of allowed evaluations of the true model
         self.surr_pre_it        = 40000 #:int:    Number of pre-training iterations for surrogate model
         self.surr_upd_it        = 6000  #:int:    Number of iterations for the surrogate model update
+        self.surr_folder        = "./"  #:str:    Folder where the surrogate model is stored
+        self.use_new_surr       = True #:bool:   Start by pre-training a new surrogate and ignore existing surrogates
 
         # OPTIMIZER parameters
         self.optimizer    = 'Adam'   #:str:    Type of optimizer used (either 'Adam' or 'RMSprop')
         self.lr           = 0.003    #:double: Learning rate
         self.lr_decay     = 0.9999   #:double: Learning rate decay
         self.lr_scheduler = 'StepLR' #:str:    type of lr scheduler used (either 'StepLR' or 'ExponentialLR')
         self.lr_step      = 1000     #:int:    Number of steps for StepLR learning rate scheduler 
@@ -55,20 +57,21 @@
         self.T            = 5        #:int:    Number of parameter updates for each temperature for $t<1$
         self.T_1          = 5001     #:int:    Number of parameter updates at $t=1$
         self.M            = 1000     #:int:    Number of Monte Carlo  samples use to compute the denominator of the AdaAnn formula        
         # Linear scheduler
         self.linear_step  = 0.0001   #:double: Fixed step size for the Linear annealing scheduler
 
         # OUTPUT parameters
-        self.output_dir        = './results/' + self.name #:str: Name of the output folder
-        self.log_file          = 'log.txt'                #:str: File name where the log profile stats are written
-        self.seed              = 35435                    #:int: Random seed
-        self.n_sample          = 5000                     #:int: Number of batch samples used to print results at save_interval
-        self.save_interval     = 200                      #:int: Save interval for all results
-        self.store_nf_interval = 1000                     #:int: Save interval for normalizing flow parameters
+        self.output_dir          = './results/' + self.name #:str: Name of the output folder
+        self.log_file            = 'log.txt'                #:str: File name where the log profile stats are written
+        self.seed                = 35435                    #:int: Random seed
+        self.n_sample            = 5000                     #:int: Number of batch samples used to print results at save_interval
+        self.save_interval       = 200                      #:int: Save interval for all results
+        self.store_nf_interval   = 1000                     #:int: Save interval for normalizing flow parameters
+        self.store_surr_interval = None                     #:int: Save interval for surrogate model (None for no save)
 
         # DEVICE parameters
         self.no_cuda = True #:bool: Flag to use CPU
 
         # Set device
         self.device = torch.device('cuda:0' if torch.cuda.is_available() and not self.no_cuda else 'cpu')
 
@@ -167,16 +170,15 @@
         else:
             loglist = []
             for i in range(1, self.n_iter+1):                
                 self.train(nf, optimizer, i, loglist, sampling=True)
                 scheduler.step()
 
         print('')
-        print('--- Simulation completed!')
-        # rt.surrogate.surrogate_save() # Used for saving the resulting surrogate model
+        print('--- Simulation completed!')        
 
     def train(self, nf, optimizer, iteration, log, sampling=True, t=1):
         """Parameter update for normalizing flow and surrogate model
 
         This is the function where the ELBO loss function is evaluated, 
         the results are saved and the surrogate model is updated.
         
@@ -254,7 +256,10 @@
         if iteration % self.log_interval == 0:
             print('VI NF (t=%5.3f): it: %7d | loss: %8.3e' % (t,iteration, loss.item()))
             log.append([t, iteration, loss.item()])
         
         # Save state of normalizing flow layers
         if self.store_nf_interval > 0 and iteration % self.store_nf_interval == 0:
             torch.save(nf.state_dict(), self.output_dir + '/' + self.name + "_" + str(iteration) + ".nf")
+
+        if not(self.store_surr_interval is None) and self.store_surr_interval > 0 and iteration % self.store_surr_interval == 0:
+            self.surrogate.surrogate_save() # Save surrogate model
```

### Comparing `linfa_vi-1.0.5/linfa/transform.py` & `linfa_vi-1.1.0/linfa/transform.py`

 * *Files identical despite different names*

### Comparing `linfa_vi-1.0.5/linfa_vi.egg-info/PKG-INFO` & `linfa_vi-1.1.0/linfa_vi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linfa-vi
-Version: 1.0.5
+Version: 1.1.0
 Summary: A Python library for inference with normalizing flow and annealing
 Author-email: resDesLab  <daniele.schiavazzi@gmail.com>
 License: Copyright © 2023 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `linfa_vi-1.0.5/pyproject.toml` & `linfa_vi-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "linfa_vi"
-version = "1.0.5"
+version = "1.1.0"
 description = "A Python library for inference with normalizing flow and annealing"
 readme = "README.md"
 authors = [{ name = "resDesLab ", email = "daniele.schiavazzi@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

