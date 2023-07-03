# Comparing `tmp/lmo-0.5.3.tar.gz` & `tmp/lmo-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmo-0.5.3.tar", max compression
+gzip compressed data, was "lmo-0.6.0.tar", max compression
```

## Comparing `lmo-0.5.3.tar` & `lmo-0.6.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
--rw-r--r--   0        0        0     1505 2023-04-29 15:29:38.675734 lmo-0.5.3/LICENSE
--rw-r--r--   0        0        0      792 2023-05-30 00:24:12.512261 lmo-0.5.3/README.md
--rw-r--r--   0        0        0      737 2023-06-04 10:26:56.859497 lmo-0.5.3/lmo/__init__.py
--rw-r--r--   0        0        0    22995 2023-06-05 16:35:54.551340 lmo-0.5.3/lmo/_lm.py
--rw-r--r--   0        0        0    11816 2023-06-04 14:08:29.938996 lmo-0.5.3/lmo/_lm_co.py
--rw-r--r--   0        0        0      158 2023-05-02 20:44:05.723493 lmo-0.5.3/lmo/_meta.py
--rw-r--r--   0        0        0     4802 2023-06-04 14:08:29.950996 lmo-0.5.3/lmo/_pwm.py
--rw-r--r--   0        0        0     1615 2023-06-03 20:03:40.058997 lmo-0.5.3/lmo/_utils.py
--rw-r--r--   0        0        0     2240 2023-06-05 14:45:24.686312 lmo-0.5.3/lmo/diagnostic.py
--rw-r--r--   0        0        0     4467 2023-05-30 20:47:52.462490 lmo-0.5.3/lmo/linalg.py
--rw-r--r--   0        0        0        0 2023-04-29 15:53:33.056174 lmo-0.5.3/lmo/py.typed
--rw-r--r--   0        0        0     5394 2023-06-05 14:17:18.849483 lmo-0.5.3/lmo/stats.py
--rw-r--r--   0        0        0     1609 2023-05-29 19:12:59.718239 lmo-0.5.3/lmo/typing.py
--rw-r--r--   0        0        0     2057 2023-06-05 16:36:45.192453 lmo-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     1950 1970-01-01 00:00:00.000000 lmo-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1505 2023-04-29 15:29:38.675734 lmo-0.6.0/LICENSE
+-rw-r--r--   0        0        0      792 2023-05-30 00:24:12.512261 lmo-0.6.0/README.md
+-rw-r--r--   0        0        0      737 2023-06-04 10:26:56.859497 lmo-0.6.0/lmo/__init__.py
+-rw-r--r--   0        0        0    23927 2023-07-02 23:41:18.697958 lmo-0.6.0/lmo/_lm.py
+-rw-r--r--   0        0        0    12018 2023-07-03 01:24:30.178022 lmo-0.6.0/lmo/_lm_co.py
+-rw-r--r--   0        0        0     2534 2023-07-03 01:16:46.763168 lmo-0.6.0/lmo/_lmm.py
+-rw-r--r--   0        0        0      158 2023-05-02 20:44:05.723493 lmo-0.6.0/lmo/_meta.py
+-rw-r--r--   0        0        0     4802 2023-06-04 14:08:29.950996 lmo-0.6.0/lmo/_pwm.py
+-rw-r--r--   0        0        0     1615 2023-06-03 20:03:40.058997 lmo-0.6.0/lmo/_utils.py
+-rw-r--r--   0        0        0     2240 2023-06-05 14:45:24.686312 lmo-0.6.0/lmo/diagnostic.py
+-rw-r--r--   0        0        0     4467 2023-05-30 20:47:52.462490 lmo-0.6.0/lmo/linalg.py
+-rw-r--r--   0        0        0        0 2023-04-29 15:53:33.056174 lmo-0.6.0/lmo/py.typed
+-rw-r--r--   0        0        0      521 2023-06-26 00:03:03.516628 lmo-0.6.0/lmo/quad.py
+-rw-r--r--   0        0        0     5400 2023-07-03 01:19:59.803689 lmo-0.6.0/lmo/stats.py
+-rw-r--r--   0        0        0     1609 2023-05-29 19:12:59.718239 lmo-0.6.0/lmo/typing.py
+-rw-r--r--   0        0        0     2147 2023-07-03 01:26:03.728214 lmo-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1950 1970-01-01 00:00:00.000000 lmo-0.6.0/PKG-INFO
```

### Comparing `lmo-0.5.3/LICENSE` & `lmo-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lmo-0.5.3/README.md` & `lmo-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `lmo-0.5.3/lmo/__init__.py` & `lmo-0.6.0/lmo/__init__.py`

 * *Files identical despite different names*

### Comparing `lmo-0.5.3/lmo/_lm.py` & `lmo-0.6.0/lmo/_lm.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,31 +11,38 @@
     'l_loc',
     'l_scale',
     'l_variation',
     'l_skew',
     'l_kurtosis',
 )
 
-from typing import Any, TypeVar, cast
+from typing import Any, Final, TypeVar, cast
 
 import numpy as np
 import numpy.typing as npt
 
 from ._pwm import b_moment_cov, b_weights
 from ._utils import clean_order, ensure_axis_at
 from .linalg import hosking_jacobi, sandwich, sh_legendre
 from .stats import ordered
 from .typing import AnyInt, IntVector, SortKind
 
 T = TypeVar('T', bound=np.floating[Any])
 
 
-# Low-level methods
+# Low-level weight methods
 
-def l0_weights(
+_L_WEIGHTS_CACHE: Final[
+    dict[
+        tuple[int, int, int],  # (n, t_1, t_2)
+        npt.NDArray[np.floating[Any]]
+    ]
+] = {}
+
+def _l0_weights(
     r: int,
     n: int,
     /,
     dtype: np.dtype[T] | type[T] = np.float_,
     *,
     enforce_symmetry: bool = True,
 ) -> npt.NDArray[T]:
@@ -121,14 +128,16 @@
 
 def l_weights(
     r: int,
     n: int,
     /,
     trim: tuple[int, int] = (0, 0),
     dtype: np.dtype[T] | type[T] = np.float_,
+    *,
+    cache: bool = False
 ) -> npt.NDArray[T]:
     """
     Projection matrix of the first $r$ (T)L-moments for $n$ samples.
 
     The matrix is a linear combination of the Power Weighted Moment
     (PWM) weight matrix (the sample estimator of $beta_{r_1}$), and the
     shifted Legendre polynomials.
@@ -170,37 +179,56 @@
         array([0.25      , 0.66666667, 0.        ])
 
     References:
         - [J.R.M. Hosking (2007) - Some theory and practical uses of trimmed
             L-moments](https://doi.org/10.1016/j.jspi.2006.12.002)
 
     """
+    cache_key = n, *trim
+    if (
+        cache_key in _L_WEIGHTS_CACHE
+        and (P_r := _L_WEIGHTS_CACHE[cache_key]).shape[0] <= r
+    ):
+        if P_r.dtype is not np.dtype(dtype):
+            P_r = P_r.view(dtype)
+        if P_r.shape[0] < r:
+            P_r = P_r[:r]
+
+        assert P_r.shape == (r, n)
+        return cast(npt.NDArray[T], P_r)
+
+
     if sum(trim) == 0:
-        return l0_weights(r, n, dtype)
+        return _l0_weights(r, n, dtype)
 
     P_r = np.empty((r, n), dtype)
 
     if r == 0:
         return P_r
 
     # the k-th TL-(t_1, t_2) weights are a linear combination of L-weights
     # with orders k, ..., k + t_1 + t_2
 
     np.matmul(
         hosking_jacobi(r, trim),
-        l0_weights(r + sum(trim), n),
+        _l0_weights(r + sum(trim), n),
         out=P_r
     )
 
     # remove numerical noise from the trimmings, and correct for potential
     # shifts in means
     t1, t2 = trim
     P_r[:, :t1] = P_r[:, n - t2:] = 0
     P_r[1:, t1:n - t2] -= P_r[1:, t1:n - t2].mean(1, keepdims=True)
 
+    if cache:
+        # memoize, and mark as readonly to avoid corruping the cache
+        P_r.setflags(write=False)
+        _L_WEIGHTS_CACHE[cache_key] = P_r
+
     return P_r
 
 
 # Summary statistics
 
 def l_moment(
     a: npt.ArrayLike,
@@ -209,14 +237,15 @@
     trim: tuple[int, int] = (0, 0),
     axis: int | None = None,
     dtype: np.dtype[T] | type[T] = np.float_,
     *,
     fweights: IntVector | None = None,
     aweights: npt.ArrayLike | None = None,
     sort: SortKind | None = 'stable',
+    cache: bool = False,
 ) -> T | npt.NDArray[T]:
     """
     Estimates the generalized trimmed L-moment $\\lambda^{(t_1, t_2)}_r$ from
     the samples along the specified axis. By default, this will be the regular
     L-moment, $\\lambda_r = \\lambda^{(0, 0)}_r$.
 
     Parameters:
@@ -273,14 +302,19 @@
             All `aweights` must be `>=0`, and the sum must be nonzero.
 
             The algorithm is similar to that for weighted quantiles.
 
         sort ('quick' | 'stable' | 'heap'):
             Sorting algorithm, see [`numpy.sort`][numpy.sort].
 
+        cache:
+            Set to `True` to speed up future L-moment calculations that have
+            the same number of observations in `a`, equal `trim`, and equal or
+            smaller `r`.
+
     Returns:
         l:
             The L-moment(s) of the input This is a scalar iff a is 1-d and
             r is a scalar. Otherwise, this is an array with
             `np.ndim(r) + np.ndim(a) - 1` dimensions and shape like
             `(*np.shape(r), *(d for d in np.shape(a) if d != axis))`.
 
@@ -318,15 +352,15 @@
     r_max: int = clean_order(cast(
         int,
         np.max(np.asarray(r))  # pyright: ignore [reportUnknownMemberType]
     ))
     n = x_k.shape[-1]
 
     # projection matrix
-    P_r = l_weights(r_max, n, trim, dtype=dtype)
+    P_r = l_weights(r_max, n, trim, dtype=dtype, cache=cache)
 
     l_r = np.inner(P_r, x_k)
 
     # we like 0-based indexing; so if P_r starts at r=1, prepend all 1's
     # for r=0 (any zeroth moment is defined to be 1)
     l_r = np.r_[np.ones((1, *l_r.shape[1:]), dtype=l_r.dtype), l_r]
```

### Comparing `lmo-0.5.3/lmo/_lm_co.py` & `lmo-0.6.0/lmo/_lm_co.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     r: AnyInt | IntVector,
     /,
     trim: tuple[int, int] = (0, 0),
     rowvar: bool = True,
     dtype: np.dtype[T] | type[T] = np.float_,
     *,
     sort: SortKind | None = 'stable',
+    cache: bool = False,
 ) -> npt.NDArray[T]:
     """
     Multivariate extension of [`lmo.l_moment`][lmo.l_moment]. Estimates the
     L-comoment matrix:
 
     $$
     \\Lambda_{r}^{(t_1, t_2)} =
@@ -98,14 +99,19 @@
         dtype:
             Floating type to use in computing the L-moments. Default is
             [`numpy.float64`][numpy.float64].
 
         sort ('quick' | 'stable' | 'heap'):
             Sorting algorithm, see [`numpy.sort`][numpy.sort].
 
+        cache:
+            Set to `True` to speed up future L-moment calculations that have
+            the same number of observations in `a`, equal `trim`, and equal or
+            smaller `r`.
+
     Returns:
         L: Array of shape `(*r.shape, m, m)` with r-th L-comoments.
 
     Examples:
         Estimation of the second L-comoment (the L-coscale) from biviariate
         normal samples:
 
@@ -141,27 +147,26 @@
     ))
     m, n = x.shape
 
     if not m:
         return np.empty(np.shape(_r) + (0, 0), dtype=dtype)
 
     # projection matrix of shape (r, n)
-    P_r = l_weights(r_max, n, trim, dtype=dtype)
+    P_r = l_weights(r_max, n, trim, dtype=dtype, cache=cache)
 
     # L-comoment matrices for r = 0, ..., r_max
     L_ij = np.empty((r_max + 1, m, m), dtype=dtype)
 
     # the zeroth L-comoment is the delta function, so the L-comoment
     # matrix is the identity matrix
     L_ij[0] = np.eye(m, dtype=dtype)
 
-    kwargs = {'axis': -1, 'dtype': dtype, 'sort': sort}
     for j in range(m):
         # concomitants of x[i] w.r.t. x[j] for all i
-        x_k_ij = ordered(x, x[j], **kwargs)
+        x_k_ij = ordered(x, x[j], axis=-1, dtype=dtype, sort=sort)
 
         L_ij[1:, :, j] = np.inner(P_r, x_k_ij)
 
     return L_ij.take(_r, 0)  # pyright: ignore [reportUnknownMemberType]
 
 
 def l_coratio(
```

### Comparing `lmo-0.5.3/lmo/_pwm.py` & `lmo-0.6.0/lmo/_pwm.py`

 * *Files identical despite different names*

### Comparing `lmo-0.5.3/lmo/_utils.py` & `lmo-0.6.0/lmo/_utils.py`

 * *Files identical despite different names*

### Comparing `lmo-0.5.3/lmo/diagnostic.py` & `lmo-0.6.0/lmo/diagnostic.py`

 * *Files identical despite different names*

### Comparing `lmo-0.5.3/lmo/linalg.py` & `lmo-0.6.0/lmo/linalg.py`

 * *Files identical despite different names*

### Comparing `lmo-0.5.3/lmo/stats.py` & `lmo-0.6.0/lmo/stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,25 +107,24 @@
         return x_k
 
     w_k = _sort_like(_clean_array(aweights))
     return _apply_aweights(x_k, w_k, axis=axis or 0)
 
 
 
-R = TypeVar('R', bound=float | npt.NDArray[np.float_])
+R = TypeVar('R', bound=float | npt.NDArray[np.floating[Any]])
 
 
 def ostat_from_ppf(
     ppf: Callable[[float], R],
     /,
     *,
     p_min: float = 0.0,
     p_max: float = 1.0,
     cache: bool = True,
-
     **quad_options: Any,
 ) -> Callable[[int, int], R]:
     # TODO: docstring, example, tests
 
     ppf_cached = functools.cache(ppf) if cache else ppf
 
     def u_ppf(
```

### Comparing `lmo-0.5.3/lmo/typing.py` & `lmo-0.6.0/lmo/typing.py`

 * *Files identical despite different names*

### Comparing `lmo-0.5.3/pyproject.toml` & `lmo-0.6.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core", "oldest-supported-numpy"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "lmo"
-version = "0.5.3"
+version = "0.6.0"
 description = "L-Moments for robust statistics."
 authors = ["Joren Hammudoglu <jhammudoglu@gmail.com>"]
 readme = "README.md"
 license = "BSD-3-Clause"
 homepage = "https://jorenham.github.io/lmo/"
 repository = "https://github.com/jorenham/lmo/"
 classifiers = [
@@ -26,16 +26,16 @@
 
 [tool.poetry.urls]
 Documentation = "https://jorenham.github.io/lmo/"
 "Bug Tracker" = "https://github.com/jorenham/lmo/issues"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-numpy = "^1.21"
-scipy = { version = "^1.8", python = "<3.12" }
+numpy = "^1.22"
+scipy = { version = "^1.9", python = "<3.12" }
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3"
 hypothesis = {extras = ["numpy"], version = "^6.75"}
 pyright = "^1.1"
 ruff = ">=0.0.263,<1.0"
@@ -65,26 +65,30 @@
 
 
 [tool.pyright]
 include = ["lmo"]
 exclude = [
     "**/__pycache__",
     "**/.pytest_cache",
+    "**/.hypothesis",
+    "**./.pytest_cache",
+    "**/.ruff_cache",
     ".git",
     ".github",
-    ".hypothesis",
-    ".pytest_cache",
-    ".ruff_cache",
     "dist",
     "docs",
+    "site",
+    "tests",
 ]
-venvPath = ".venv"
+venv = ".venv"
 pythonVersion = "3.10"
 pythonPlatform = "Linux"
 typeCheckingMode = "strict"
+reportMissingImports = true
+reportMissingTypeStubs = false
 
 
 [tool.ruff]
 line-length = 80
 target-version = "py310"
 
 [tool.ruff.pydocstyle]
```

### Comparing `lmo-0.5.3/PKG-INFO` & `lmo-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmo
-Version: 0.5.3
+Version: 0.6.0
 Summary: L-Moments for robust statistics.
 Home-page: https://jorenham.github.io/lmo/
 License: BSD-3-Clause
 Author: Joren Hammudoglu
 Author-email: jhammudoglu@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -16,16 +16,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
-Requires-Dist: numpy (>=1.21,<2.0)
-Requires-Dist: scipy (>=1.8,<2.0) ; python_version < "3.12"
+Requires-Dist: numpy (>=1.22,<2.0)
+Requires-Dist: scipy (>=1.9,<2.0) ; python_version < "3.12"
 Project-URL: Bug Tracker, https://github.com/jorenham/lmo/issues
 Project-URL: Documentation, https://jorenham.github.io/lmo/
 Project-URL: Repository, https://github.com/jorenham/lmo/
 Description-Content-Type: text/markdown
 
 <!--head-start-->
```

