# Comparing `tmp/algovision-0.1.1.tar.gz` & `tmp/algovision-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "algovision-0.1.1.tar", last modified: Sun Dec  5 18:24:35 2021, max compression
+gzip compressed data, was "algovision-0.1.2.tar", last modified: Mon Jul  3 19:29:21 2023, max compression
```

## Comparing `algovision-0.1.1.tar` & `algovision-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 felixpetersen   (501) staff       (20)        0 2021-12-05 18:24:35.982008 algovision-0.1.1/
--rw-r--r--   0 felixpetersen   (501) staff       (20)     1071 2021-12-05 18:17:26.000000 algovision-0.1.1/LICENSE
--rw-r--r--   0 felixpetersen   (501) staff       (20)     9452 2021-12-05 18:24:35.981706 algovision-0.1.1/PKG-INFO
--rw-r--r--   0 felixpetersen   (501) staff       (20)     8570 2021-12-05 18:18:29.000000 algovision-0.1.1/README.md
-drwxr-xr-x   0 felixpetersen   (501) staff       (20)        0 2021-12-05 18:24:35.975897 algovision-0.1.1/algovision/
--rw-r--r--   0 felixpetersen   (501) staff       (20)      315 2021-12-05 18:17:26.000000 algovision-0.1.1/algovision/__init__.py
--rw-r--r--   0 felixpetersen   (501) staff       (20)     3061 2021-12-05 18:17:26.000000 algovision-0.1.1/algovision/conditions.py
--rw-r--r--   0 felixpetersen   (501) staff       (20)     6792 2021-12-05 18:17:26.000000 algovision-0.1.1/algovision/control_structures.py
--rw-r--r--   0 felixpetersen   (501) staff       (20)    22378 2021-12-05 18:17:26.000000 algovision-0.1.1/algovision/core.py
--rw-r--r--   0 felixpetersen   (501) staff       (20)     1386 2021-12-05 18:17:26.000000 algovision-0.1.1/algovision/functions.py
--rw-r--r--   0 felixpetersen   (501) staff       (20)    16603 2021-12-05 18:17:26.000000 algovision-0.1.1/algovision/instructions.py
-drwxr-xr-x   0 felixpetersen   (501) staff       (20)        0 2021-12-05 18:24:35.981365 algovision-0.1.1/algovision.egg-info/
--rw-r--r--   0 felixpetersen   (501) staff       (20)     9452 2021-12-05 18:24:35.000000 algovision-0.1.1/algovision.egg-info/PKG-INFO
--rw-r--r--   0 felixpetersen   (501) staff       (20)      346 2021-12-05 18:24:35.000000 algovision-0.1.1/algovision.egg-info/SOURCES.txt
--rw-r--r--   0 felixpetersen   (501) staff       (20)        1 2021-12-05 18:24:35.000000 algovision-0.1.1/algovision.egg-info/dependency_links.txt
--rw-r--r--   0 felixpetersen   (501) staff       (20)       19 2021-12-05 18:24:35.000000 algovision-0.1.1/algovision.egg-info/requires.txt
--rw-r--r--   0 felixpetersen   (501) staff       (20)       11 2021-12-05 18:24:35.000000 algovision-0.1.1/algovision.egg-info/top_level.txt
--rw-r--r--   0 felixpetersen   (501) staff       (20)       38 2021-12-05 18:24:35.982074 algovision-0.1.1/setup.cfg
--rw-r--r--   0 felixpetersen   (501) staff       (20)     1474 2021-12-05 18:17:26.000000 algovision-0.1.1/setup.py
+drwxr-xr-x   0 felixpetersen   (501) staff       (20)        0 2023-07-03 19:29:21.517352 algovision-0.1.2/
+-rw-r--r--   0 felixpetersen   (501) staff       (20)     1071 2021-12-05 14:34:11.000000 algovision-0.1.2/LICENSE
+-rw-r--r--   0 felixpetersen   (501) staff       (20)    11513 2023-07-03 19:29:21.517186 algovision-0.1.2/PKG-INFO
+-rw-r--r--   0 felixpetersen   (501) staff       (20)    10651 2021-12-06 14:18:52.000000 algovision-0.1.2/README.md
+drwxr-xr-x   0 felixpetersen   (501) staff       (20)        0 2023-07-03 19:29:21.516199 algovision-0.1.2/algovision/
+-rw-r--r--   0 felixpetersen   (501) staff       (20)      315 2021-12-05 17:43:46.000000 algovision-0.1.2/algovision/__init__.py
+-rw-r--r--   0 felixpetersen   (501) staff       (20)     3061 2021-12-05 17:43:46.000000 algovision-0.1.2/algovision/conditions.py
+-rw-r--r--   0 felixpetersen   (501) staff       (20)     6792 2021-12-05 17:43:46.000000 algovision-0.1.2/algovision/control_structures.py
+-rw-r--r--   0 felixpetersen   (501) staff       (20)    22455 2023-07-03 19:27:39.000000 algovision-0.1.2/algovision/core.py
+-rw-r--r--   0 felixpetersen   (501) staff       (20)     2882 2021-12-06 14:13:10.000000 algovision-0.1.2/algovision/functions.py
+-rw-r--r--   0 felixpetersen   (501) staff       (20)    18238 2021-12-06 14:13:10.000000 algovision-0.1.2/algovision/instructions.py
+drwxr-xr-x   0 felixpetersen   (501) staff       (20)        0 2023-07-03 19:29:21.516963 algovision-0.1.2/algovision.egg-info/
+-rw-r--r--   0 felixpetersen   (501) staff       (20)    11513 2023-07-03 19:29:21.000000 algovision-0.1.2/algovision.egg-info/PKG-INFO
+-rw-r--r--   0 felixpetersen   (501) staff       (20)      346 2023-07-03 19:29:21.000000 algovision-0.1.2/algovision.egg-info/SOURCES.txt
+-rw-r--r--   0 felixpetersen   (501) staff       (20)        1 2023-07-03 19:29:21.000000 algovision-0.1.2/algovision.egg-info/dependency_links.txt
+-rw-r--r--   0 felixpetersen   (501) staff       (20)       19 2023-07-03 19:29:21.000000 algovision-0.1.2/algovision.egg-info/requires.txt
+-rw-r--r--   0 felixpetersen   (501) staff       (20)       11 2023-07-03 19:29:21.000000 algovision-0.1.2/algovision.egg-info/top_level.txt
+-rw-r--r--   0 felixpetersen   (501) staff       (20)       38 2023-07-03 19:29:21.517399 algovision-0.1.2/setup.cfg
+-rw-r--r--   0 felixpetersen   (501) staff       (20)     1474 2023-07-03 19:26:24.000000 algovision-0.1.2/setup.py
```

### Comparing `algovision-0.1.1/LICENSE` & `algovision-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `algovision-0.1.1/PKG-INFO` & `algovision-0.1.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: algovision
-Version: 0.1.1
+Version: 0.1.2
 Summary: AlgoVision - A Framework for Differentiable Algorithms and Algorithmic Supervision
 Home-page: https://github.com/Felix-Petersen/algovision
 Author: Felix Petersen
 Author-email: ads0399@felix-petersen.de
 License: MIT License
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
@@ -29,26 +28,26 @@
 Video @ [Youtube](https://www.youtube.com/watch?v=01ENzpkjOCE)).
 
 `algovision` is a Python 3.6+ and PyTorch 1.9.0+ based library for making algorithms differentiable. It can be installed via:
 ```shell
 pip install algovision
 ```
 Applications include smoothly integrating algorithms into neural networks for algorithmic supervision, problem-specific optimization within an algorithm, and whatever your imagination allows.
+As `algovision` relies on PyTorch it also supports CUDA, etc. 
 
 ### [Check out the Documentation!](https://felix-petersen.github.io/algovision-docs/)
 
 ## 🌱 Intro
 
 Deriving a loss from a smooth algorithm can be as easy as
 
 ```python
 from examples import get_bubble_sort
 import torch
 
-torch.manual_seed(0)
 # Get an array (the first dimension is the batch dimension, which is always required)
 array = torch.randn(1, 8, requires_grad=True)
 
 bubble_sort = get_bubble_sort(beta=5)
 result, loss = bubble_sort(array)
 
 loss.backward()
@@ -58,18 +57,19 @@
 ```
 
 Here, the loss is a sorting loss corresponding to the number of swaps in the bubble sort algorithm.
 But we can also define this algorithm from scratch:
 
 ```python
 from algovision import (
-    Algorithm, Input, Output, Var, VarInt,  # core
-    GT, IsTrue,                       # conditions
-    If, While, For,           # control_structures
-    Let, LetInt,                       # functions
+    Algorithm, Input, Output, Var, VarInt,                                          # core
+    Let, LetInt, Print,                                                     # instructions
+    Eq, NEq, LT, LEq, GT, GEq, CatProbEq, CosineSimilarity, IsTrue, IsFalse,  # conditions
+    If, While, For,                                                   # control_structures
+    Min, ArgMin, Max, ArgMax,                                                  # functions
 )
 import torch
 
 bubble_sort = Algorithm(
     # Define the variables the input corresponds to
     Input('array'),
     # Declare and initialize all differentiable variables 
@@ -123,17 +123,18 @@
   <summary>(<i>click to expand</i>)</summary>
 
 
 The full set of modules is:
 ```python
 from algovision import (
     Algorithm, Input, Output, Var, VarInt,                                          # core
+    Let, LetInt, Print,                                                     # instructions
     Eq, NEq, LT, LEq, GT, GEq, CatProbEq, CosineSimilarity, IsTrue, IsFalse,  # conditions
     If, While, For,                                                   # control_structures
-    Let, LetInt, Print, Min, ArgMin, Max, ArgMax,                              # functions
+    Min, ArgMin, Max, ArgMax,                                                  # functions
 )
 ```
 `Algorithm` is the main class, `Input` and `Output` define arguments and return values, `Var` defines differentiable variables and `VarInt` defines non-differentiable integer variables.
 `Eq`, `LT`, etc. are relaxed conditions for `If` and `While`, which are respective control structures.
 `For` bounded loops of fixed length that are unrolled.
 `Let` sets a differentiable variable, `LetInt` sets a hard integer variable. 
 Note that hard integer variables should only be used if they are independent of the input values, but they may depend on the input shape (e.g., for reducing the number of iterations after each traversal of a For loop).
@@ -150,15 +151,28 @@
 
 `Let('z', lambda x, y: x**2 + y)` corresponds to the regular line of code `z = x**2 + y`.
 This also allows inserting complex external functions including neural networks as part of the lambda expression.
 Assuming `net` is a neural networks, one can write `Let('y', lambda x: net(x))` (corresponding to `y = net(x)`).
 
 ### Let
 
-`Let` is a very flexible instruction.
+`Let` is a very flexible instruction. The following table shows the use cases of it.
+
+| AlgoVision                                    | Python                        | Description                       |
+|-----------------------------------------------|-------------------------------|-----------------------------------|
+| `Let('a', 'x')`                               | `a = x`                       | Variable `a` is set to the value of variable `x`. |
+| `Let('a', lambda x: x**2)`                    | `a = x**2`                    | As soon as we compute anything on the right hand side of the equation, we need to write it as a `lambda` expression. |
+| `Let('a', 'array', ['i'])`                    | `a = array[i]`                | Indexing on the right hand requires an additional list parameter after the second argument. |
+| `Let('a', lambda array, i: array[:, i])`      | `a = array[i]`                | Equivalent to the row above: indexing can also be manually done inside of a `lambda` expression. Note that in this case, the batch dimension has to be written explicitly. |
+| `Let('a', 'array', ['i', lambda j: j+1])`     | `a = array[i, j+1]`           | Multiple indices and `lambda` expressions are also supported. |
+| `Let('a', 'array', [None, slice(0, None, 2)])`| `a = array[:, 0::2]`          | `None` and `slice`s are also supported. |
+| `Let('a', ['i'], 'x')`                        | `a[i] = x`                    | Indexing can also be done on the left hand side of the equation. |
+| `Let('a', ['i'], 'x', ['j'])`                 | `a[i] = x['j']`               | ...or on both sides. |
+| `Let(['a', 'b'], lamba x, y: (x+y, x-y))`     | `a, b = x+y, x-y`             | Multiple return values are supported. |
+
 In its most simple form `Let` obtains two arguments, a string naming the variable where the result is written, and the value that may be expressed via a `lambda` expression.
 
 If the lambda expression returns multiple values, e.g., because a complex function is called and has two return values, the left argument can be a list of strings. 
 That is, `Let(['a', 'b'], lamba x, y: (x+y, x-y))` corresponds to `a, b = x+y, x-y`.
 
 `Let` also supports indexing. This is denoted by an additional list argument after the left and/or the right argument.
 For example, `Let('a', 'array', ['i'])` corresponds to `a = array[i]`, while `Let('array', ['i'], 'b')` corresponds to `array[i] = b`.
@@ -201,9 +215,7 @@
 }
 ```
 
 ## 📜 License
 
 `algovision` is released under the MIT license. See [LICENSE](LICENSE) for additional details.
 
-
-
```

### Comparing `algovision-0.1.1/README.md` & `algovision-0.1.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -7,26 +7,26 @@
 Video @ [Youtube](https://www.youtube.com/watch?v=01ENzpkjOCE)).
 
 `algovision` is a Python 3.6+ and PyTorch 1.9.0+ based library for making algorithms differentiable. It can be installed via:
 ```shell
 pip install algovision
 ```
 Applications include smoothly integrating algorithms into neural networks for algorithmic supervision, problem-specific optimization within an algorithm, and whatever your imagination allows.
+As `algovision` relies on PyTorch it also supports CUDA, etc. 
 
 ### [Check out the Documentation!](https://felix-petersen.github.io/algovision-docs/)
 
 ## 🌱 Intro
 
 Deriving a loss from a smooth algorithm can be as easy as
 
 ```python
 from examples import get_bubble_sort
 import torch
 
-torch.manual_seed(0)
 # Get an array (the first dimension is the batch dimension, which is always required)
 array = torch.randn(1, 8, requires_grad=True)
 
 bubble_sort = get_bubble_sort(beta=5)
 result, loss = bubble_sort(array)
 
 loss.backward()
@@ -36,18 +36,19 @@
 ```
 
 Here, the loss is a sorting loss corresponding to the number of swaps in the bubble sort algorithm.
 But we can also define this algorithm from scratch:
 
 ```python
 from algovision import (
-    Algorithm, Input, Output, Var, VarInt,  # core
-    GT, IsTrue,                       # conditions
-    If, While, For,           # control_structures
-    Let, LetInt,                       # functions
+    Algorithm, Input, Output, Var, VarInt,                                          # core
+    Let, LetInt, Print,                                                     # instructions
+    Eq, NEq, LT, LEq, GT, GEq, CatProbEq, CosineSimilarity, IsTrue, IsFalse,  # conditions
+    If, While, For,                                                   # control_structures
+    Min, ArgMin, Max, ArgMax,                                                  # functions
 )
 import torch
 
 bubble_sort = Algorithm(
     # Define the variables the input corresponds to
     Input('array'),
     # Declare and initialize all differentiable variables 
@@ -101,17 +102,18 @@
   <summary>(<i>click to expand</i>)</summary>
 
 
 The full set of modules is:
 ```python
 from algovision import (
     Algorithm, Input, Output, Var, VarInt,                                          # core
+    Let, LetInt, Print,                                                     # instructions
     Eq, NEq, LT, LEq, GT, GEq, CatProbEq, CosineSimilarity, IsTrue, IsFalse,  # conditions
     If, While, For,                                                   # control_structures
-    Let, LetInt, Print, Min, ArgMin, Max, ArgMax,                              # functions
+    Min, ArgMin, Max, ArgMax,                                                  # functions
 )
 ```
 `Algorithm` is the main class, `Input` and `Output` define arguments and return values, `Var` defines differentiable variables and `VarInt` defines non-differentiable integer variables.
 `Eq`, `LT`, etc. are relaxed conditions for `If` and `While`, which are respective control structures.
 `For` bounded loops of fixed length that are unrolled.
 `Let` sets a differentiable variable, `LetInt` sets a hard integer variable. 
 Note that hard integer variables should only be used if they are independent of the input values, but they may depend on the input shape (e.g., for reducing the number of iterations after each traversal of a For loop).
@@ -128,15 +130,28 @@
 
 `Let('z', lambda x, y: x**2 + y)` corresponds to the regular line of code `z = x**2 + y`.
 This also allows inserting complex external functions including neural networks as part of the lambda expression.
 Assuming `net` is a neural networks, one can write `Let('y', lambda x: net(x))` (corresponding to `y = net(x)`).
 
 ### Let
 
-`Let` is a very flexible instruction.
+`Let` is a very flexible instruction. The following table shows the use cases of it.
+
+| AlgoVision                                    | Python                        | Description                       |
+|-----------------------------------------------|-------------------------------|-----------------------------------|
+| `Let('a', 'x')`                               | `a = x`                       | Variable `a` is set to the value of variable `x`. |
+| `Let('a', lambda x: x**2)`                    | `a = x**2`                    | As soon as we compute anything on the right hand side of the equation, we need to write it as a `lambda` expression. |
+| `Let('a', 'array', ['i'])`                    | `a = array[i]`                | Indexing on the right hand requires an additional list parameter after the second argument. |
+| `Let('a', lambda array, i: array[:, i])`      | `a = array[i]`                | Equivalent to the row above: indexing can also be manually done inside of a `lambda` expression. Note that in this case, the batch dimension has to be written explicitly. |
+| `Let('a', 'array', ['i', lambda j: j+1])`     | `a = array[i, j+1]`           | Multiple indices and `lambda` expressions are also supported. |
+| `Let('a', 'array', [None, slice(0, None, 2)])`| `a = array[:, 0::2]`          | `None` and `slice`s are also supported. |
+| `Let('a', ['i'], 'x')`                        | `a[i] = x`                    | Indexing can also be done on the left hand side of the equation. |
+| `Let('a', ['i'], 'x', ['j'])`                 | `a[i] = x['j']`               | ...or on both sides. |
+| `Let(['a', 'b'], lamba x, y: (x+y, x-y))`     | `a, b = x+y, x-y`             | Multiple return values are supported. |
+
 In its most simple form `Let` obtains two arguments, a string naming the variable where the result is written, and the value that may be expressed via a `lambda` expression.
 
 If the lambda expression returns multiple values, e.g., because a complex function is called and has two return values, the left argument can be a list of strings. 
 That is, `Let(['a', 'b'], lamba x, y: (x+y, x-y))` corresponds to `a, b = x+y, x-y`.
 
 `Let` also supports indexing. This is denoted by an additional list argument after the left and/or the right argument.
 For example, `Let('a', 'array', ['i'])` corresponds to `a = array[i]`, while `Let('array', ['i'], 'b')` corresponds to `array[i] = b`.
```

### Comparing `algovision-0.1.1/algovision/conditions.py` & `algovision-0.1.2/algovision/conditions.py`

 * *Files identical despite different names*

### Comparing `algovision-0.1.1/algovision/control_structures.py` & `algovision-0.1.2/algovision/control_structures.py`

 * *Files identical despite different names*

### Comparing `algovision-0.1.1/algovision/core.py` & `algovision-0.1.2/algovision/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -246,16 +246,17 @@
             # print('merge', p_0.shape, self.state[key].shape, value.shape)
             self.state[key] = (self.state[key] * p_0 + value * p_1)
 
     def probabilistic_update(self, key, value, p):
         assert p.shape[0] == self.batch_size, (p.shape, self.batch_size)
         assert len(p.shape) == len(self.state[key].shape), (p.shape, self.state[key].shape)
 
-        while len(value.shape) < len(self.state[key].shape):
-            value = value.unsqueeze(-1)
+        if not (isinstance(value, int) or isinstance(value, float)):
+            while len(value.shape) < len(self.state[key].shape):
+                value = value.unsqueeze(-1)
 
         # print('probabilistic_update', p.shape, self.state[key].shape, value.shape)
         self.state[key] = p * value + (1-p) * self.state[key]
 
     def reset(self):
         """(Internal)  Resets all tensors to zero.
         """
```

### Comparing `algovision-0.1.1/algovision/instructions.py` & `algovision-0.1.2/algovision/instructions.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,53 @@
 # This source code is licensed under the MIT license found in the
 # LICENSE file in the root directory of this source tree.
 
 from algovision.core import *
 
 
 class Let(AlgoModule):
+    """
+
+    .. list-table:: Use cases of :class:`Let`
+       :widths: 38 24 37
+       :header-rows: 1
+       :class: tight-table
+
+       * - AlgoVision
+         - Python
+         - Description
+       * - ``Let('a', 'x')``
+         - ``a = x``
+         - Variable ``a`` is set to the value of variable ``x``.
+       * - ``Let('a', lambda x: x**2)``
+         - ``a = x**2``
+         - As soon as we compute anything on the right hand side of the equation, we need to write it as a ``lambda`` expression.
+       * - ``Let('a', 'array', ['i'])``
+         - ``a = array[i]``
+         - Indexing on the right hand requires an additional list parameter after the second argument.
+       * - ``Let('a', lambda array, i: array[:, i])``
+         - ``a = array[i]``
+         - Equivalent to the row above: indexing can also be manually done inside of a ``lambda`` expression. Note that in this case, the batch dimension has to be written explicitly.
+       * - ``Let('a', 'array', ['i', lambda j: j+1])``
+         - ``a = array[i, j+1]``
+         - Multiple indices and `lambda` expressions are also supported.
+       * - ``Let('a', 'array', [None, slice(0, None, 2)])``
+         - ``a = array[:, 0::2]``
+         - ``None`` and ``slice`` s are also supported.
+       * - ``Let('a', ['i'], 'x')``
+         - ``a[i] = x``
+         - Indexing can also be done on the left hand side of the equation.
+       * - ``Let('a', ['i'], 'x', ['j'])``
+         - ``a[i] = x['j']``
+         - ...or on both sides.
+       * - ``Let(['a', 'b'], lamba x, y: (x+y, x-y))``
+         - ``a, b = x+y, x-y``
+         - Multiple return values are supported.
+
+    """
     def __init__(self, *args):
         """
         The :class:`Let` module executes a lambda or arbitrary other function and writes the return values back to
         the specified variable.
 
         """
         super(Let, self).__init__()
```

### Comparing `algovision-0.1.1/algovision.egg-info/PKG-INFO` & `algovision-0.1.2/algovision.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: algovision
-Version: 0.1.1
+Version: 0.1.2
 Summary: AlgoVision - A Framework for Differentiable Algorithms and Algorithmic Supervision
 Home-page: https://github.com/Felix-Petersen/algovision
 Author: Felix Petersen
 Author-email: ads0399@felix-petersen.de
 License: MIT License
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
@@ -29,26 +28,26 @@
 Video @ [Youtube](https://www.youtube.com/watch?v=01ENzpkjOCE)).
 
 `algovision` is a Python 3.6+ and PyTorch 1.9.0+ based library for making algorithms differentiable. It can be installed via:
 ```shell
 pip install algovision
 ```
 Applications include smoothly integrating algorithms into neural networks for algorithmic supervision, problem-specific optimization within an algorithm, and whatever your imagination allows.
+As `algovision` relies on PyTorch it also supports CUDA, etc. 
 
 ### [Check out the Documentation!](https://felix-petersen.github.io/algovision-docs/)
 
 ## 🌱 Intro
 
 Deriving a loss from a smooth algorithm can be as easy as
 
 ```python
 from examples import get_bubble_sort
 import torch
 
-torch.manual_seed(0)
 # Get an array (the first dimension is the batch dimension, which is always required)
 array = torch.randn(1, 8, requires_grad=True)
 
 bubble_sort = get_bubble_sort(beta=5)
 result, loss = bubble_sort(array)
 
 loss.backward()
@@ -58,18 +57,19 @@
 ```
 
 Here, the loss is a sorting loss corresponding to the number of swaps in the bubble sort algorithm.
 But we can also define this algorithm from scratch:
 
 ```python
 from algovision import (
-    Algorithm, Input, Output, Var, VarInt,  # core
-    GT, IsTrue,                       # conditions
-    If, While, For,           # control_structures
-    Let, LetInt,                       # functions
+    Algorithm, Input, Output, Var, VarInt,                                          # core
+    Let, LetInt, Print,                                                     # instructions
+    Eq, NEq, LT, LEq, GT, GEq, CatProbEq, CosineSimilarity, IsTrue, IsFalse,  # conditions
+    If, While, For,                                                   # control_structures
+    Min, ArgMin, Max, ArgMax,                                                  # functions
 )
 import torch
 
 bubble_sort = Algorithm(
     # Define the variables the input corresponds to
     Input('array'),
     # Declare and initialize all differentiable variables 
@@ -123,17 +123,18 @@
   <summary>(<i>click to expand</i>)</summary>
 
 
 The full set of modules is:
 ```python
 from algovision import (
     Algorithm, Input, Output, Var, VarInt,                                          # core
+    Let, LetInt, Print,                                                     # instructions
     Eq, NEq, LT, LEq, GT, GEq, CatProbEq, CosineSimilarity, IsTrue, IsFalse,  # conditions
     If, While, For,                                                   # control_structures
-    Let, LetInt, Print, Min, ArgMin, Max, ArgMax,                              # functions
+    Min, ArgMin, Max, ArgMax,                                                  # functions
 )
 ```
 `Algorithm` is the main class, `Input` and `Output` define arguments and return values, `Var` defines differentiable variables and `VarInt` defines non-differentiable integer variables.
 `Eq`, `LT`, etc. are relaxed conditions for `If` and `While`, which are respective control structures.
 `For` bounded loops of fixed length that are unrolled.
 `Let` sets a differentiable variable, `LetInt` sets a hard integer variable. 
 Note that hard integer variables should only be used if they are independent of the input values, but they may depend on the input shape (e.g., for reducing the number of iterations after each traversal of a For loop).
@@ -150,15 +151,28 @@
 
 `Let('z', lambda x, y: x**2 + y)` corresponds to the regular line of code `z = x**2 + y`.
 This also allows inserting complex external functions including neural networks as part of the lambda expression.
 Assuming `net` is a neural networks, one can write `Let('y', lambda x: net(x))` (corresponding to `y = net(x)`).
 
 ### Let
 
-`Let` is a very flexible instruction.
+`Let` is a very flexible instruction. The following table shows the use cases of it.
+
+| AlgoVision                                    | Python                        | Description                       |
+|-----------------------------------------------|-------------------------------|-----------------------------------|
+| `Let('a', 'x')`                               | `a = x`                       | Variable `a` is set to the value of variable `x`. |
+| `Let('a', lambda x: x**2)`                    | `a = x**2`                    | As soon as we compute anything on the right hand side of the equation, we need to write it as a `lambda` expression. |
+| `Let('a', 'array', ['i'])`                    | `a = array[i]`                | Indexing on the right hand requires an additional list parameter after the second argument. |
+| `Let('a', lambda array, i: array[:, i])`      | `a = array[i]`                | Equivalent to the row above: indexing can also be manually done inside of a `lambda` expression. Note that in this case, the batch dimension has to be written explicitly. |
+| `Let('a', 'array', ['i', lambda j: j+1])`     | `a = array[i, j+1]`           | Multiple indices and `lambda` expressions are also supported. |
+| `Let('a', 'array', [None, slice(0, None, 2)])`| `a = array[:, 0::2]`          | `None` and `slice`s are also supported. |
+| `Let('a', ['i'], 'x')`                        | `a[i] = x`                    | Indexing can also be done on the left hand side of the equation. |
+| `Let('a', ['i'], 'x', ['j'])`                 | `a[i] = x['j']`               | ...or on both sides. |
+| `Let(['a', 'b'], lamba x, y: (x+y, x-y))`     | `a, b = x+y, x-y`             | Multiple return values are supported. |
+
 In its most simple form `Let` obtains two arguments, a string naming the variable where the result is written, and the value that may be expressed via a `lambda` expression.
 
 If the lambda expression returns multiple values, e.g., because a complex function is called and has two return values, the left argument can be a list of strings. 
 That is, `Let(['a', 'b'], lamba x, y: (x+y, x-y))` corresponds to `a, b = x+y, x-y`.
 
 `Let` also supports indexing. This is denoted by an additional list argument after the left and/or the right argument.
 For example, `Let('a', 'array', ['i'])` corresponds to `a = array[i]`, while `Let('array', ['i'], 'b')` corresponds to `array[i] = b`.
@@ -201,9 +215,7 @@
 }
 ```
 
 ## 📜 License
 
 `algovision` is released under the MIT license. See [LICENSE](LICENSE) for additional details.
 
-
-
```

### Comparing `algovision-0.1.1/setup.py` & `algovision-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='algovision',
-    version='v0.1.1',
+    version='v0.1.2',
     description='AlgoVision - A Framework for Differentiable Algorithms and Algorithmic Supervision',
     author='Felix Petersen',
     author_email=__email__,
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/Felix-Petersen/algovision',
     classifiers=[
```

