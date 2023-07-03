# Comparing `tmp/pwasopt-0.0.5.tar.gz` & `tmp/pwasopt-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwasopt-0.0.5.tar", last modified: Sat Jul  1 21:32:37 2023, max compression
+gzip compressed data, was "pwasopt-0.0.6.tar", last modified: Mon Jul  3 15:16:01 2023, max compression
```

## Comparing `pwasopt-0.0.5.tar` & `pwasopt-0.0.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-07-01 21:32:37.884184 pwasopt-0.0.5/
--rw-rw-rw-   0        0        0    11527 2023-06-30 12:07:33.000000 pwasopt-0.0.5/LICENSE
--rw-rw-rw-   0        0        0    17149 2023-07-01 21:32:37.883185 pwasopt-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0    16420 2023-07-01 21:20:12.000000 pwasopt-0.0.5/README.md
--rw-rw-rw-   0        0        0      932 2023-07-01 21:22:06.000000 pwasopt-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-01 21:32:37.885185 pwasopt-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-01 21:32:37.817160 pwasopt-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-07-01 21:32:37.861154 pwasopt-0.0.5/src/pwasopt/
--rw-rw-rw-   0        0        0        0 2023-06-30 09:41:30.000000 pwasopt-0.0.5/src/pwasopt/__init__.py
--rw-rw-rw-   0        0        0    70455 2023-02-08 22:16:04.000000 pwasopt-0.0.5/src/pwasopt/acquisition.py
--rw-rw-rw-   0        0        0     2928 2023-02-08 22:16:44.000000 pwasopt-0.0.5/src/pwasopt/categorical_encoder.py
--rw-rw-rw-   0        0        0    14361 2023-07-01 21:17:48.000000 pwasopt-0.0.5/src/pwasopt/fit_surrogate_pwasp.py
--rw-rw-rw-   0        0        0     3273 2023-02-08 22:16:44.000000 pwasopt-0.0.5/src/pwasopt/integ_encoder.py
--rw-rw-rw-   0        0        0    21999 2023-07-01 12:54:13.000000 pwasopt-0.0.5/src/pwasopt/main_pwas.py
--rw-rw-rw-   0        0        0    22340 2023-07-01 12:53:59.000000 pwasopt-0.0.5/src/pwasopt/main_pwasp.py
--rw-rw-rw-   0        0        0     2773 2022-10-12 17:09:17.000000 pwasopt-0.0.5/src/pwasopt/pref_fun.py
--rw-rw-rw-   0        0        0     4205 2022-10-12 17:09:22.000000 pwasopt-0.0.5/src/pwasopt/pref_fun1.py
--rw-rw-rw-   0        0        0    12417 2023-06-30 12:36:24.000000 pwasopt-0.0.5/src/pwasopt/prob_setup.py
--rw-rw-rw-   0        0        0    30948 2023-06-30 12:36:24.000000 pwasopt-0.0.5/src/pwasopt/sample.py
-drwxrwxrwx   0        0        0        0 2023-07-01 21:32:37.879407 pwasopt-0.0.5/src/pwasopt.egg-info/
--rw-rw-rw-   0        0        0    17149 2023-07-01 21:32:37.000000 pwasopt-0.0.5/src/pwasopt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      504 2023-07-01 21:32:37.000000 pwasopt-0.0.5/src/pwasopt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-01 21:32:37.000000 pwasopt-0.0.5/src/pwasopt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-07-01 21:32:37.000000 pwasopt-0.0.5/src/pwasopt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-01 21:32:37.000000 pwasopt-0.0.5/src/pwasopt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-03 15:16:01.220931 pwasopt-0.0.6/
+-rw-rw-rw-   0        0        0    11527 2023-06-30 12:07:33.000000 pwasopt-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0    17840 2023-07-03 15:16:01.218196 pwasopt-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0    17111 2023-07-03 15:12:57.000000 pwasopt-0.0.6/README.md
+-rw-rw-rw-   0        0        0      932 2023-07-03 15:14:32.000000 pwasopt-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-03 15:16:01.220931 pwasopt-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-03 15:16:01.102627 pwasopt-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-07-03 15:16:01.184053 pwasopt-0.0.6/src/pwasopt/
+-rw-rw-rw-   0        0        0        0 2023-06-30 09:41:30.000000 pwasopt-0.0.6/src/pwasopt/__init__.py
+-rw-rw-rw-   0        0        0    70455 2023-02-08 22:16:04.000000 pwasopt-0.0.6/src/pwasopt/acquisition.py
+-rw-rw-rw-   0        0        0     2928 2023-02-08 22:16:44.000000 pwasopt-0.0.6/src/pwasopt/categorical_encoder.py
+-rw-rw-rw-   0        0        0    14361 2023-07-01 21:17:48.000000 pwasopt-0.0.6/src/pwasopt/fit_surrogate_pwasp.py
+-rw-rw-rw-   0        0        0     3273 2023-02-08 22:16:44.000000 pwasopt-0.0.6/src/pwasopt/integ_encoder.py
+-rw-rw-rw-   0        0        0    21959 2023-07-03 15:10:09.000000 pwasopt-0.0.6/src/pwasopt/main_pwas.py
+-rw-rw-rw-   0        0        0    22300 2023-07-03 15:10:09.000000 pwasopt-0.0.6/src/pwasopt/main_pwasp.py
+-rw-rw-rw-   0        0        0     2773 2022-10-12 17:09:17.000000 pwasopt-0.0.6/src/pwasopt/pref_fun.py
+-rw-rw-rw-   0        0        0     4205 2022-10-12 17:09:22.000000 pwasopt-0.0.6/src/pwasopt/pref_fun1.py
+-rw-rw-rw-   0        0        0    12417 2023-06-30 12:36:24.000000 pwasopt-0.0.6/src/pwasopt/prob_setup.py
+-rw-rw-rw-   0        0        0    30948 2023-06-30 12:36:24.000000 pwasopt-0.0.6/src/pwasopt/sample.py
+drwxrwxrwx   0        0        0        0 2023-07-03 15:16:01.211094 pwasopt-0.0.6/src/pwasopt.egg-info/
+-rw-rw-rw-   0        0        0    17840 2023-07-03 15:16:01.000000 pwasopt-0.0.6/src/pwasopt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      504 2023-07-03 15:16:01.000000 pwasopt-0.0.6/src/pwasopt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 15:16:01.000000 pwasopt-0.0.6/src/pwasopt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-07-03 15:16:01.000000 pwasopt-0.0.6/src/pwasopt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-03 15:16:01.000000 pwasopt-0.0.6/src/pwasopt.egg-info/top_level.txt
```

### Comparing `pwasopt-0.0.5/LICENSE` & `pwasopt-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.5/PKG-INFO` & `pwasopt-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwasopt
-Version: 0.0.5
+Version: 0.0.6
 Summary: PWAS/PWASp - Global and Preference-based Optimization with Mixed Variables using (P)iece(w)ise (A)ffine (S)urrogates
 Author-email: Mengjia Zhu <mengjia.zhu@imtlucca.it>, Alberto Bemporad <alberto.bemporad@imtlucca.it>
 Project-URL: Homepage, https://github.com/mjzhu-p/PWAS
 Keywords: Mixed-variable optimization,Mixed-integer optimization,global optimization,preference-based optimization,black-box optimization
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -52,17 +52,24 @@
 * scipy
 * pulp
 * sklearn
 * [pyparc](https://pypi.org/project/pyparc/)
 * [pyDOE](https://pythonhosted.org/pyDOE/)
 * [pycddlib](https://pypi.org/project/pycddlib/)
 
-**Note**: PWAS/PWASp use `GUROBI` as the default solver to solve the MILP problem of acquisition optimization, 
+### External dependencies:
+MILP solver:
+- PWAS/PWASp use `GUROBI` as the default solver to solve the MILP problem of acquisition optimization, 
 which is found to be the most robust during benchmark testing. Alternatively, we also include `GLPK`, which may introduce
-errors occasionally depending on the test problem and initial samples.
+errors occasionally depending on the test problem and initial samples. User can also switch to another MILP solver by editing the
+relevant codes in `acquisition.py` and `sample.py`. Check the compatability of the MILP solver with `pulp` (the LP modeler) 
+at the [project webpage](https://pypi.org/project/PuLP/).
+- `GUROBI`: [academic licenses](https://www.gurobi.com/academia/academic-program-and-licenses/)
+- `GLPK`: [project webpage](https://www.gnu.org/software/glpk/)
+  - [step-by-step explanation for the installation on Stack Overflow](https://stackoverflow.com/questions/17513666/installing-glpk-gnu-linear-programming-kit-on-windows)
 
 
 <a name="basic-usage"></a>
 ## Basic usage
 
 ### Examples
 Examples of benchmark testing using PWAS/PWASp can be found in the `examples` folder:
@@ -238,15 +245,15 @@
 X2 = np.array(optimizer2.X)
 fbest_seq2 = optimizer2.fbest_seq
 
 ~~~
 Below we show the best values `fbest_seq1` found by PWAS. 
 
 <p align = "center">
-<img src="./figures/PWAS_XG-MNIST.png" alt="drawing" width=60%/>
+<img src="https://github.com/mjzhu-p/PWAS/blob/main/figures/PWAS_XG-MNIST.png" alt="drawing" width=60%/>
 </p>
 
 
 ### Solve use PWASp
 When solve with PWASp, instead of using the function evaluations, we solve a preference-based optimization problem 
 with preference function $\pi(x_1,x_2)$, $x_1,x_2\in\mathbb{R}^n$
 within the finite bounds `lb` $\leq x\leq$ `ub` (see Section 4 of [[1]](#ref1)).
@@ -313,15 +320,15 @@
 fbest_seq2 = list(map(fun, X2[optimizer2.ibest_seq]))
 fbest2 = min(fbest_seq2)
 
 ~~~
 Below we show the best values `fbest_seq1` found by PWASp. Note that function evaluations here are shown solely for demonstration purposes, which are unknown to PWASp during the solution process.
 
 <p align = "center">
-<img src="./figures/PWASp_XG-MNIST.png" alt="drawing" width=60%/>
+<img src="https://github.com/mjzhu-p/PWAS/blob/main/figures/PWASp_XG-MNIST.png" alt="drawing" width=60%/>
 </p>
 
 
 ### Include constraints
 
 We note below how to include constraints if present.
```

### Comparing `pwasopt-0.0.5/README.md` & `pwasopt-0.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -38,17 +38,24 @@
 * scipy
 * pulp
 * sklearn
 * [pyparc](https://pypi.org/project/pyparc/)
 * [pyDOE](https://pythonhosted.org/pyDOE/)
 * [pycddlib](https://pypi.org/project/pycddlib/)
 
-**Note**: PWAS/PWASp use `GUROBI` as the default solver to solve the MILP problem of acquisition optimization, 
+### External dependencies:
+MILP solver:
+- PWAS/PWASp use `GUROBI` as the default solver to solve the MILP problem of acquisition optimization, 
 which is found to be the most robust during benchmark testing. Alternatively, we also include `GLPK`, which may introduce
-errors occasionally depending on the test problem and initial samples.
+errors occasionally depending on the test problem and initial samples. User can also switch to another MILP solver by editing the
+relevant codes in `acquisition.py` and `sample.py`. Check the compatability of the MILP solver with `pulp` (the LP modeler) 
+at the [project webpage](https://pypi.org/project/PuLP/).
+- `GUROBI`: [academic licenses](https://www.gurobi.com/academia/academic-program-and-licenses/)
+- `GLPK`: [project webpage](https://www.gnu.org/software/glpk/)
+  - [step-by-step explanation for the installation on Stack Overflow](https://stackoverflow.com/questions/17513666/installing-glpk-gnu-linear-programming-kit-on-windows)
 
 
 <a name="basic-usage"></a>
 ## Basic usage
 
 ### Examples
 Examples of benchmark testing using PWAS/PWASp can be found in the `examples` folder:
@@ -224,15 +231,15 @@
 X2 = np.array(optimizer2.X)
 fbest_seq2 = optimizer2.fbest_seq
 
 ~~~
 Below we show the best values `fbest_seq1` found by PWAS. 
 
 <p align = "center">
-<img src="./figures/PWAS_XG-MNIST.png" alt="drawing" width=60%/>
+<img src="https://github.com/mjzhu-p/PWAS/blob/main/figures/PWAS_XG-MNIST.png" alt="drawing" width=60%/>
 </p>
 
 
 ### Solve use PWASp
 When solve with PWASp, instead of using the function evaluations, we solve a preference-based optimization problem 
 with preference function $\pi(x_1,x_2)$, $x_1,x_2\in\mathbb{R}^n$
 within the finite bounds `lb` $\leq x\leq$ `ub` (see Section 4 of [[1]](#ref1)).
@@ -299,15 +306,15 @@
 fbest_seq2 = list(map(fun, X2[optimizer2.ibest_seq]))
 fbest2 = min(fbest_seq2)
 
 ~~~
 Below we show the best values `fbest_seq1` found by PWASp. Note that function evaluations here are shown solely for demonstration purposes, which are unknown to PWASp during the solution process.
 
 <p align = "center">
-<img src="./figures/PWASp_XG-MNIST.png" alt="drawing" width=60%/>
+<img src="https://github.com/mjzhu-p/PWAS/blob/main/figures/PWASp_XG-MNIST.png" alt="drawing" width=60%/>
 </p>
 
 
 ### Include constraints
 
 We note below how to include constraints if present.
```

### Comparing `pwasopt-0.0.5/pyproject.toml` & `pwasopt-0.0.6/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pwasopt"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Mengjia Zhu", email="mengjia.zhu@imtlucca.it" },
   { name="Alberto Bemporad", email="alberto.bemporad@imtlucca.it" },
 ]
 description = "PWAS/PWASp - Global and Preference-based Optimization with Mixed Variables using (P)iece(w)ise (A)ffine (S)urrogates"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `pwasopt-0.0.5/src/pwasopt/acquisition.py` & `pwasopt-0.0.6/src/pwasopt/acquisition.py`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.5/src/pwasopt/categorical_encoder.py` & `pwasopt-0.0.6/src/pwasopt/categorical_encoder.py`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.5/src/pwasopt/fit_surrogate_pwasp.py` & `pwasopt-0.0.6/src/pwasopt/fit_surrogate_pwasp.py`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.5/src/pwasopt/integ_encoder.py` & `pwasopt-0.0.6/src/pwasopt/integ_encoder.py`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.5/src/pwasopt/main_pwas.py` & `pwasopt-0.0.6/src/pwasopt/main_pwas.py`

 * *Files 0% similar despite different names*

```diff
@@ -307,15 +307,15 @@
             skip_z = False
             if acq_stage == 'multi-stage':
                 if nd >0:
                     z1 = self.AL.discrete_explore(X_curr[:, nci_encoded:], self.xsbest[:nci_encoded].reshape(nci_encoded, 1), a, b,
                                              N, omega, gamma, Kf, dF_)
                     if np.isnan(z1).any():
                         print(
-                            'The optimal solution is not reached within the timeLimit in GUROBI, solution is sampled using \'acq_surrogate\' function in acquisition.py.')
+                            'The optimal solution is not reached within the timeLimit, solution is sampled using \'acq_surrogate\' function in acquisition.py.')
                         if int_encoded:
                             z = self.AL.acq_surrogate_intEncoded(a, b, omega, gamma, Kf, dF_)
                         else:
                             z = self.AL.acq_surrogate(a, b, omega, gamma, Kf, dF_)
                         skip_z = True
                 else:
                     z1 = np.array([])
@@ -327,15 +327,15 @@
                         if int_encoded:
                             z2 = self.AL.integ_explore_intEncoded(X_curr[:, nc:nci_encoded], self.xsbest[:nc].reshape(nc, 1), z1.reshape(sum_X_d, 1), a,
                                                   b, N, omega, gamma, Kf, dF_)
                         else:
                             z2 = self.AL.integ_explore(X_curr[:, nc:nci_encoded], self.xsbest[:nc].reshape(nc, 1),z1.reshape(sum_X_d, 1), a, b, N, omega, gamma, Kf, dF_)
                             if np.isnan(z2).any():
                                 print(
-                                    'The optimal solution is not reached within the timeLimit in GUROBI, solution is sampled using \'acq_surrogate\' function in acquisition.py.')
+                                    'The optimal solution is not reached within the timeLimit, solution is sampled using \'acq_surrogate\' function in acquisition.py.')
                                 if int_encoded:
                                     z = self.AL.acq_surrogate_intEncoded(a, b, omega, gamma, Kf, dF_)
                                 else:
                                     z = self.AL.acq_surrogate(a, b, omega, gamma, Kf, dF_)
                                 skip_z = True
                 else:
                     z2 = np.array([])
@@ -344,15 +344,15 @@
 
                 if nc>0:
                     if not skip_z:
                         z3 = self.AL.cont_explore(X_curr[:, :nc], z2.reshape(nint_encoded, 1), z1.reshape(sum_X_d, 1), a, b,
                                              N, omega, gamma, Kf, dF_)
                         if np.isnan(z3).any():
                             print(
-                                'The optimal solution is not reached within the timeLimit in GUROBI, solution is sampled using \'acq_surrogate\' function in acquisition.py.')
+                                'The optimal solution is not reached within the timeLimit, solution is sampled using \'acq_surrogate\' function in acquisition.py.')
                             if int_encoded:
                                 z = self.AL.acq_surrogate_intEncoded(a, b, omega, gamma, Kf, dF_)
                             else:
                                 z = self.AL.acq_surrogate(a, b, omega, gamma, Kf, dF_)
                             skip_z = True
                 else:
                     z3 = np.array([])
@@ -363,15 +363,15 @@
                 # Solve the acquisition step in one stage
                 if int_encoded:
                     z = self.AL.acq_explore_intEncoded(X_curr, a, b, N, omega, gamma, Kf, dF_)
                 else:
                     z = self.AL.acq_explore(X_curr, a, b, N, omega, gamma, Kf, dF_)
                 if np.isnan(z).any():
                     print(
-                        'The optimal solution is not reached within the timeLimit in GUROBI, solution is sampled using \'acq_surrogate\' function in acquisition.py.')
+                        'The optimal solution is not reached within the timeLimit, solution is sampled using \'acq_surrogate\' function in acquisition.py.')
                     z = self.AL.acq_surrogate(a, b, omega, gamma, Kf, dF_)
 
             else:
                 errstr_acq_stage = "acq_stage can only be 'one-stage' or 'multi-stage', please check the string assigned"
                 print(errstr_acq_stage)
                 sys.exit(1)
             self.time_opt_acquisition.append(time.time() - t0)
```

### Comparing `pwasopt-0.0.5/src/pwasopt/main_pwasp.py` & `pwasopt-0.0.6/src/pwasopt/main_pwasp.py`

 * *Files 2% similar despite different names*

```diff
@@ -304,15 +304,15 @@
             skip_z = False
             if acq_stage == 'multi-stage':
                 if nd > 0:
                     z1 = self.AL.discrete_explore(X_curr[:, nci_encoded:], self.xsbest[:nci_encoded].reshape(nci_encoded, 1), a, b,
                                              N, omega, gamma, Kf, dF)
                     if np.isnan(z1).any():
                         print(
-                            'The optimal solution is not reached within the timeLimit in GUROBI, solution is sampled using \'acq_surrogate\' function in acquisition.py.')
+                            'The optimal solution is not reached within the timeLimit, solution is sampled using \'acq_surrogate\' function in acquisition.py.')
                         if int_encoded:
                             z = self.AL.acq_surrogate_intEncoded(a, b, omega, gamma, Kf, dF)
                         else:
                             z = self.AL.acq_surrogate(a, b, omega, gamma, Kf, dF)
                         skip_z = True
                 else:
                     z1 = np.array([])
@@ -326,15 +326,15 @@
                                                              z1.reshape(sum_X_d, 1), a,
                                                              b, N, omega, gamma, Kf, dF)
                         else:
                             z2 = self.AL.integ_explore(X_curr[:, nc:nci_encoded], self.xsbest[:nc].reshape(nc, 1),
                                                   z1.reshape(sum_X_d, 1), a, b, N, omega, gamma, Kf, dF)
                             if np.isnan(z2).any():
                                 print(
-                                    'The optimal solution is not reached within the timeLimit in GUROBI, solution is sampled using \'acq_surrogate\' function in acquisition.py.')
+                                    'The optimal solution is not reached within the timeLimit, solution is sampled using \'acq_surrogate\' function in acquisition.py.')
                                 if int_encoded:
                                     z = self.AL.acq_surrogate_intEncoded(a, b, omega, gamma, Kf, dF)
                                 else:
                                     z = self.AL.acq_surrogate(a, b, omega, gamma, Kf, dF)
                                 skip_z = True
                 else:
                     z2 = np.array([])
@@ -343,15 +343,15 @@
 
                 if nc > 0:
                     if not skip_z:
                         z3 = self.AL.cont_explore(X_curr[:, :nc], z2.reshape(nint_encoded, 1), z1.reshape(sum_X_d, 1), a, b,
                                              N, omega, gamma, Kf, dF)
                         if np.isnan(z3).any():
                             print(
-                                'The optimal solution is not reached within the timeLimit in GUROBI, solution is sampled using \'acq_surrogate\' function in acquisition.py.')
+                                'The optimal solution is not reached within the timeLimit, solution is sampled using \'acq_surrogate\' function in acquisition.py.')
                             if int_encoded:
                                 z = self.AL.acq_surrogate_intEncoded(a, b, omega, gamma, Kf, dF)
                             else:
                                 z = self.AL.acq_surrogate(a, b, omega, gamma, Kf, dF)
                             skip_z = True
                 else:
                     z3 = np.array([])
@@ -362,15 +362,15 @@
                 # Solve the acquisition step in one stage
                 if int_encoded:
                     z = self.AL.acq_explore_intEncoded(X_curr, a, b, N, omega, gamma, Kf, dF)
                 else:
                     z = self.AL.acq_explore(X_curr, a, b, N, omega, gamma, Kf, dF)
                 if np.isnan(z).any():
                     print(
-                        'The optimal solution is not reached within the timeLimit in GUROBI, solution is sampled using \'acq_surrogate\' function in acquisition.py.')
+                        'The optimal solution is not reached within the timeLimit, solution is sampled using \'acq_surrogate\' function in acquisition.py.')
                     z = self.AL.acq_surrogate(a, b, omega, gamma, Kf, dF)
 
             else:
                 errstr_acq_stage = "acq_stage can only be 'one-stage' or 'multi-stage', please check the string assigned"
                 print(errstr_acq_stage)
                 sys.exit(1)
             self.time_opt_acquisition.append(time.time() - t0)
```

### Comparing `pwasopt-0.0.5/src/pwasopt/pref_fun.py` & `pwasopt-0.0.6/src/pwasopt/pref_fun.py`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.5/src/pwasopt/pref_fun1.py` & `pwasopt-0.0.6/src/pwasopt/pref_fun1.py`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.5/src/pwasopt/prob_setup.py` & `pwasopt-0.0.6/src/pwasopt/prob_setup.py`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.5/src/pwasopt/sample.py` & `pwasopt-0.0.6/src/pwasopt/sample.py`

 * *Files identical despite different names*

### Comparing `pwasopt-0.0.5/src/pwasopt.egg-info/PKG-INFO` & `pwasopt-0.0.6/src/pwasopt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwasopt
-Version: 0.0.5
+Version: 0.0.6
 Summary: PWAS/PWASp - Global and Preference-based Optimization with Mixed Variables using (P)iece(w)ise (A)ffine (S)urrogates
 Author-email: Mengjia Zhu <mengjia.zhu@imtlucca.it>, Alberto Bemporad <alberto.bemporad@imtlucca.it>
 Project-URL: Homepage, https://github.com/mjzhu-p/PWAS
 Keywords: Mixed-variable optimization,Mixed-integer optimization,global optimization,preference-based optimization,black-box optimization
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -52,17 +52,24 @@
 * scipy
 * pulp
 * sklearn
 * [pyparc](https://pypi.org/project/pyparc/)
 * [pyDOE](https://pythonhosted.org/pyDOE/)
 * [pycddlib](https://pypi.org/project/pycddlib/)
 
-**Note**: PWAS/PWASp use `GUROBI` as the default solver to solve the MILP problem of acquisition optimization, 
+### External dependencies:
+MILP solver:
+- PWAS/PWASp use `GUROBI` as the default solver to solve the MILP problem of acquisition optimization, 
 which is found to be the most robust during benchmark testing. Alternatively, we also include `GLPK`, which may introduce
-errors occasionally depending on the test problem and initial samples.
+errors occasionally depending on the test problem and initial samples. User can also switch to another MILP solver by editing the
+relevant codes in `acquisition.py` and `sample.py`. Check the compatability of the MILP solver with `pulp` (the LP modeler) 
+at the [project webpage](https://pypi.org/project/PuLP/).
+- `GUROBI`: [academic licenses](https://www.gurobi.com/academia/academic-program-and-licenses/)
+- `GLPK`: [project webpage](https://www.gnu.org/software/glpk/)
+  - [step-by-step explanation for the installation on Stack Overflow](https://stackoverflow.com/questions/17513666/installing-glpk-gnu-linear-programming-kit-on-windows)
 
 
 <a name="basic-usage"></a>
 ## Basic usage
 
 ### Examples
 Examples of benchmark testing using PWAS/PWASp can be found in the `examples` folder:
@@ -238,15 +245,15 @@
 X2 = np.array(optimizer2.X)
 fbest_seq2 = optimizer2.fbest_seq
 
 ~~~
 Below we show the best values `fbest_seq1` found by PWAS. 
 
 <p align = "center">
-<img src="./figures/PWAS_XG-MNIST.png" alt="drawing" width=60%/>
+<img src="https://github.com/mjzhu-p/PWAS/blob/main/figures/PWAS_XG-MNIST.png" alt="drawing" width=60%/>
 </p>
 
 
 ### Solve use PWASp
 When solve with PWASp, instead of using the function evaluations, we solve a preference-based optimization problem 
 with preference function $\pi(x_1,x_2)$, $x_1,x_2\in\mathbb{R}^n$
 within the finite bounds `lb` $\leq x\leq$ `ub` (see Section 4 of [[1]](#ref1)).
@@ -313,15 +320,15 @@
 fbest_seq2 = list(map(fun, X2[optimizer2.ibest_seq]))
 fbest2 = min(fbest_seq2)
 
 ~~~
 Below we show the best values `fbest_seq1` found by PWASp. Note that function evaluations here are shown solely for demonstration purposes, which are unknown to PWASp during the solution process.
 
 <p align = "center">
-<img src="./figures/PWASp_XG-MNIST.png" alt="drawing" width=60%/>
+<img src="https://github.com/mjzhu-p/PWAS/blob/main/figures/PWASp_XG-MNIST.png" alt="drawing" width=60%/>
 </p>
 
 
 ### Include constraints
 
 We note below how to include constraints if present.
```

