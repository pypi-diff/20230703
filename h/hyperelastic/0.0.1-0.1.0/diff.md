# Comparing `tmp/hyperelastic-0.0.1.tar.gz` & `tmp/hyperelastic-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperelastic-0.0.1.tar", last modified: Sun Jul  2 22:06:59 2023, max compression
+gzip compressed data, was "hyperelastic-0.1.0.tar", last modified: Sun Jul  2 22:18:54 2023, max compression
```

## Comparing `hyperelastic-0.0.1.tar` & `hyperelastic-0.1.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:06:59.617007 hyperelastic-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-02 22:06:44.000000 hyperelastic-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    48636 2023-07-02 22:06:59.617007 hyperelastic-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6752 2023-07-02 22:06:44.000000 hyperelastic-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-02 22:06:44.000000 hyperelastic-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 22:06:59.617007 hyperelastic-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:06:59.609006 hyperelastic-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:06:59.613006 hyperelastic-0.0.1/src/hyperelastic/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-02 22:06:44.000000 hyperelastic-0.0.1/src/hyperelastic/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-02 22:06:44.000000 hyperelastic-0.0.1/src/hyperelastic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:06:59.613006 hyperelastic-0.0.1/src/hyperelastic/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-02 22:06:44.000000 hyperelastic-0.0.1/src/hyperelastic/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-07-02 22:06:44.000000 hyperelastic-0.0.1/src/hyperelastic/frameworks/_invariants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6360 2023-07-02 22:06:44.000000 hyperelastic-0.0.1/src/hyperelastic/frameworks/_stretches.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:06:59.613006 hyperelastic-0.0.1/src/hyperelastic/math/
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-02 22:06:44.000000 hyperelastic-0.0.1/src/hyperelastic/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6090 2023-07-02 22:06:44.000000 hyperelastic-0.0.1/src/hyperelastic/math/_voigt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:06:59.613006 hyperelastic-0.0.1/src/hyperelastic/models/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-02 22:06:44.000000 hyperelastic-0.0.1/src/hyperelastic/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:06:59.613006 hyperelastic-0.0.1/src/hyperelastic/models/invariants/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-02 22:06:44.000000 hyperelastic-0.0.1/src/hyperelastic/models/invariants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-07-02 22:06:44.000000 hyperelastic-0.0.1/src/hyperelastic/models/invariants/_third_order_deformation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:06:59.613006 hyperelastic-0.0.1/src/hyperelastic/models/stretches/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-02 22:06:44.000000 hyperelastic-0.0.1/src/hyperelastic/models/stretches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-02 22:06:44.000000 hyperelastic-0.0.1/src/hyperelastic/models/stretches/_ogden.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:06:59.613006 hyperelastic-0.0.1/src/hyperelastic/spaces/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-02 22:06:44.000000 hyperelastic-0.0.1/src/hyperelastic/spaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-07-02 22:06:44.000000 hyperelastic-0.0.1/src/hyperelastic/spaces/_deformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-07-02 22:06:44.000000 hyperelastic-0.0.1/src/hyperelastic/spaces/_dilatational.py
--rw-r--r--   0 runner    (1001) docker     (123)     7967 2023-07-02 22:06:44.000000 hyperelastic-0.0.1/src/hyperelastic/spaces/_distortional.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:06:59.613006 hyperelastic-0.0.1/src/hyperelastic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    48636 2023-07-02 22:06:59.000000 hyperelastic-0.0.1/src/hyperelastic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-02 22:06:59.000000 hyperelastic-0.0.1/src/hyperelastic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 22:06:59.000000 hyperelastic-0.0.1/src/hyperelastic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-02 22:06:59.000000 hyperelastic-0.0.1/src/hyperelastic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-02 22:06:59.000000 hyperelastic-0.0.1/src/hyperelastic.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:06:59.613006 hyperelastic-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-02 22:06:44.000000 hyperelastic-0.0.1/tests/test_space.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-07-02 22:06:44.000000 hyperelastic-0.0.1/tests/test_sympy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:18:54.827358 hyperelastic-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-02 22:18:44.000000 hyperelastic-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    48636 2023-07-02 22:18:54.827358 hyperelastic-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6752 2023-07-02 22:18:44.000000 hyperelastic-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-02 22:18:44.000000 hyperelastic-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-02 22:18:54.827358 hyperelastic-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:18:54.819358 hyperelastic-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:18:54.823358 hyperelastic-0.1.0/src/hyperelastic/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-02 22:18:44.000000 hyperelastic-0.1.0/src/hyperelastic/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-02 22:18:44.000000 hyperelastic-0.1.0/src/hyperelastic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:18:54.823358 hyperelastic-0.1.0/src/hyperelastic/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-02 22:18:44.000000 hyperelastic-0.1.0/src/hyperelastic/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-07-02 22:18:44.000000 hyperelastic-0.1.0/src/hyperelastic/frameworks/_invariants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6360 2023-07-02 22:18:44.000000 hyperelastic-0.1.0/src/hyperelastic/frameworks/_stretches.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:18:54.823358 hyperelastic-0.1.0/src/hyperelastic/math/
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-02 22:18:44.000000 hyperelastic-0.1.0/src/hyperelastic/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6090 2023-07-02 22:18:44.000000 hyperelastic-0.1.0/src/hyperelastic/math/_voigt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:18:54.823358 hyperelastic-0.1.0/src/hyperelastic/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-02 22:18:44.000000 hyperelastic-0.1.0/src/hyperelastic/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:18:54.827358 hyperelastic-0.1.0/src/hyperelastic/models/invariants/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-02 22:18:44.000000 hyperelastic-0.1.0/src/hyperelastic/models/invariants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-07-02 22:18:44.000000 hyperelastic-0.1.0/src/hyperelastic/models/invariants/_third_order_deformation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:18:54.827358 hyperelastic-0.1.0/src/hyperelastic/models/stretches/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-02 22:18:44.000000 hyperelastic-0.1.0/src/hyperelastic/models/stretches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-02 22:18:44.000000 hyperelastic-0.1.0/src/hyperelastic/models/stretches/_ogden.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:18:54.827358 hyperelastic-0.1.0/src/hyperelastic/spaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-02 22:18:44.000000 hyperelastic-0.1.0/src/hyperelastic/spaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2669 2023-07-02 22:18:44.000000 hyperelastic-0.1.0/src/hyperelastic/spaces/_deformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-07-02 22:18:44.000000 hyperelastic-0.1.0/src/hyperelastic/spaces/_dilatational.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7998 2023-07-02 22:18:44.000000 hyperelastic-0.1.0/src/hyperelastic/spaces/_distortional.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:18:54.823358 hyperelastic-0.1.0/src/hyperelastic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    48636 2023-07-02 22:18:54.000000 hyperelastic-0.1.0/src/hyperelastic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-02 22:18:54.000000 hyperelastic-0.1.0/src/hyperelastic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-02 22:18:54.000000 hyperelastic-0.1.0/src/hyperelastic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-02 22:18:54.000000 hyperelastic-0.1.0/src/hyperelastic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-02 22:18:54.000000 hyperelastic-0.1.0/src/hyperelastic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-02 22:18:54.827358 hyperelastic-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-02 22:18:44.000000 hyperelastic-0.1.0/tests/test_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-07-02 22:18:44.000000 hyperelastic-0.1.0/tests/test_sympy.py
```

### Comparing `hyperelastic-0.0.1/LICENSE` & `hyperelastic-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.0.1/PKG-INFO` & `hyperelastic-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperelastic
-Version: 0.0.1
+Version: 0.1.0
 Summary: Constitutive hyperelastic material formulations for FElupe
 Author: Andreas Dutzler
 Author-email: a.dutzler@gmail.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `hyperelastic-0.0.1/README.md` & `hyperelastic-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.0.1/pyproject.toml` & `hyperelastic-0.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -39,19 +39,19 @@
   "Topic :: Scientific/Engineering :: Mathematics",
   "Topic :: Utilities"
 ]
 dynamic = ["version"]
 requires-python = ">=3.7"
 dependencies = [
   "numpy",
-  "felupe",
 ]
 
 [project.optional-dependencies]
 test = [
+    "felupe",
     "sympy",
 ]
 
 [tool.setuptools.dynamic]
 version = {attr = "hyperelastic.__about__.__version__"}
 
 [project.urls]
```

### Comparing `hyperelastic-0.0.1/src/hyperelastic/frameworks/_invariants.py` & `hyperelastic-0.1.0/src/hyperelastic/frameworks/_invariants.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.0.1/src/hyperelastic/frameworks/_stretches.py` & `hyperelastic-0.1.0/src/hyperelastic/frameworks/_stretches.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.0.1/src/hyperelastic/math/_voigt.py` & `hyperelastic-0.1.0/src/hyperelastic/math/_voigt.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.0.1/src/hyperelastic/models/invariants/_third_order_deformation.py` & `hyperelastic-0.1.0/src/hyperelastic/models/invariants/_third_order_deformation.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.0.1/src/hyperelastic/spaces/_deformation.py` & `hyperelastic-0.1.0/src/hyperelastic/spaces/_deformation.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import felupe.math as fm
 import numpy as np
 
 from ..math import astensor, asvoigt, cdya_ik, eye
 
 
 class DeformationSpace:
     r"""The deformation space.
@@ -39,29 +38,37 @@
 
     """
 
     def __init__(self, material, parallel=False):
         self.parallel = parallel
         self.material = material
 
+        if self.parallel:
+            from einsumt import einsumt
+
+            self.einsum = einsumt
+        else:
+            self.einsum = np.einsum
+
         # initial variables for calling
         # ``self.gradient(self.x)`` and ``self.hessian(self.x)``
         self.x = [material.x[0], material.x[-1]]
 
     def gradient(self, x):
         """The gradient as the partial derivative of the strain energy function w.r.t.
         the deformation gradient."""
 
         F, statevars = x[0], x[-1]
-        self.C = asvoigt(fm.dot(fm.transpose(F), F))
+
+        self.C = asvoigt(self.einsum("kI...,kJ...->IJ...", F, F))
         dWdC, statevars_new = self.material.gradient(self.C, statevars)
 
         self.S = 2 * dWdC
 
-        return [fm.dot(F, astensor(self.S)), statevars_new]
+        return [self.einsum("iK...,KJ...->iJ...", F, astensor(self.S)), statevars_new]
 
     def hessian(self, x):
         """The hessian as the second partial derivative of the strain energy function
         w.r.t. the deformation gradient."""
 
         F, statevars = x[0], x[-1]
```

### Comparing `hyperelastic-0.0.1/src/hyperelastic/spaces/_dilatational.py` & `hyperelastic-0.1.0/src/hyperelastic/spaces/_dilatational.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,42 @@
-import felupe.math as fm
 import numpy as np
 
 from ..math import astensor, asvoigt, cdya, cdya_ik, ddot, det, dya, eye, inv, trace
 
 
 class DilatationalSpace:
     def __init__(self, material, parallel=False):
         self.parallel = parallel
         self.material = material
 
+        if self.parallel:
+            from einsumt import einsumt
+
+            self.einsum = einsumt
+        else:
+            self.einsum = np.einsum
+
         # initial variables for calling
         # ``self.gradient(self.x)`` and ``self.hessian(self.x)``
         self.x = [material.x[0], material.x[-1]]
 
     def gradient(self, x):
         F, statevars = x[0], x[-1]
-        self.C = asvoigt(fm.dot(fm.transpose(F), F))
+
+        self.C = asvoigt(self.einsum("kI...,kJ...->IJ...", F, F))
         self.I3 = det(self.C)
         self.Co = self.I3 ** (1 / 3) * self.C
         dWodCo, statevars_new = self.material.gradient(self.Co, statevars)
 
         self.Sb = 2 * self.I3 ** (1 / 3) * dWodCo
         self.tr_Sb = trace(self.Sb)
         self.invC = inv(self.C, determinant=self.I3)
 
         self.S = self.tr_Sb / 3 * self.invC
-        return [fm.dot(F, astensor(self.S)), statevars_new]
+        return [self.einsum("iK...,KJ...->iJ...", F, astensor(self.S)), statevars_new]
 
     def hessian(self, x):
         F, statevars = x[0], x[-1]
 
         dWodF, statevars_new = self.gradient(x)
 
         d2WodCodCo = self.material.hessian(self.Co, statevars)
@@ -39,17 +46,10 @@
         tr_C4b = ddot(ddot(I, C4b, mode=(2, 4)), I)
         I4 = cdya(self.invC, self.invC)
 
         C4 = (2 * self.tr_Sb + tr_C4b) * dya(
             self.invC, self.invC
         ) / 9 - 2 / 3 * self.tr_Sb * I4
 
-        if self.parallel:
-            from einsumt import einsumt
-
-            einsum = einsumt
-        else:
-            einsum = np.einsum
-
-        A4 = einsum("iI...,kK...,IJKL...->iJkL...", F, F, astensor(C4, 4))
+        A4 = self.einsum("iI...,kK...,IJKL...->iJkL...", F, F, astensor(C4, 4))
 
         return [A4 + cdya_ik(I, self.S)]
```

### Comparing `hyperelastic-0.0.1/src/hyperelastic/spaces/_distortional.py` & `hyperelastic-0.1.0/src/hyperelastic/spaces/_distortional.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import felupe.math as fm
 import numpy as np
 
 from ..math import astensor, asvoigt, cdya, cdya_ik, ddot, det, dya, eye, inv, transpose
 
 
 class DistortionalSpace:
     r"""The distortional (part of the deformation) space is a partial deformation with
@@ -141,35 +140,43 @@
 
     """
 
     def __init__(self, material, parallel=False):
         self.parallel = parallel
         self.material = material
 
+        if self.parallel:
+            from einsumt import einsumt
+
+            self.einsum = einsumt
+        else:
+            self.einsum = np.einsum
+
         # initial variables for calling
         # ``self.gradient(self.x)`` and ``self.hessian(self.x)``
         self.x = [material.x[0], material.x[-1]]
 
     def gradient(self, x):
         """The gradient as the partial derivative of the strain energy function w.r.t.
         the deformation gradient."""
 
         F, statevars = x[0], x[-1]
-        self.C = C = asvoigt(fm.dot(fm.transpose(F), F))
+
+        self.C = C = asvoigt(self.einsum("kI...,kJ...->IJ...", F, F))
         self.I3 = I3 = det(C)
         self.Cu = I3 ** (-1 / 3) * C
         dWudCu, statevars_new = self.material.gradient(self.Cu, statevars)
 
         self.Sb = Sb = 2 * I3 ** (-1 / 3) * dWudCu
         self.SbC = SbC = ddot(Sb, C)
         self.invC = invC = inv(C, determinant=I3)
 
         self.S = Sb - SbC / 3 * invC
 
-        return [fm.dot(F, astensor(self.S)), statevars_new]
+        return [self.einsum("iK...,KJ...->iJ...", F, astensor(self.S)), statevars_new]
 
     def hessian(self, x):
         """The hessian as the second partial derivative of the strain energy function
         w.r.t. the deformation gradient."""
 
         F, statevars = x[0], x[-1]
 
@@ -187,17 +194,10 @@
         invCinvC = dya(self.invC, self.invC)
 
         C4 = 2 / 3 * (self.SbC * I4 - SbinvC - invCSb + self.SbC / 3 * invCinvC)
 
         if not np.allclose(C4b, 0):
             C4 += ddot(ddot(P4, C4b, mode=(4, 4)), transpose(P4), mode=(4, 4))
 
-        if self.parallel:
-            from einsumt import einsumt
-
-            einsum = einsumt
-        else:
-            einsum = np.einsum
-
-        A4 = einsum("iI...,kK...,IJKL...->iJkL...", F, F, astensor(C4, 4))
+        A4 = self.einsum("iI...,kK...,IJKL...->iJkL...", F, F, astensor(C4, 4))
 
         return [A4 + cdya_ik(I, self.S)]
```

### Comparing `hyperelastic-0.0.1/src/hyperelastic.egg-info/PKG-INFO` & `hyperelastic-0.1.0/src/hyperelastic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperelastic
-Version: 0.0.1
+Version: 0.1.0
 Summary: Constitutive hyperelastic material formulations for FElupe
 Author: Andreas Dutzler
 Author-email: a.dutzler@gmail.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `hyperelastic-0.0.1/src/hyperelastic.egg-info/SOURCES.txt` & `hyperelastic-0.1.0/src/hyperelastic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.0.1/tests/test_space.py` & `hyperelastic-0.1.0/tests/test_space.py`

 * *Files identical despite different names*

### Comparing `hyperelastic-0.0.1/tests/test_sympy.py` & `hyperelastic-0.1.0/tests/test_sympy.py`

 * *Files identical despite different names*

