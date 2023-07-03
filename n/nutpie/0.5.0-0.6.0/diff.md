# Comparing `tmp/nutpie-0.5.0.tar.gz` & `tmp/nutpie-0.6.0.tar.gz`

## Comparing `nutpie-0.5.0.tar` & `nutpie-0.6.0.tar`

### file list

```diff
@@ -1,30 +1,23 @@
--rw-r--r--   0        0        0      849 1970-01-01 00:00:00.000000 nutpie-0.5.0/Cargo.toml
--rw-r--r--   0      501       20     2204 2023-01-01 06:15:56.000000 nutpie-0.5.0/.github/workflows/ci.yml
--rw-r--r--   0      501       20      143 2022-12-31 07:46:26.000000 nutpie-0.5.0/.gitignore
--rw-r--r--   0      501       20     1072 2022-12-31 07:46:26.000000 nutpie-0.5.0/LICENSE
--rw-r--r--   0      501       20     3492 2023-01-02 04:15:03.000000 nutpie-0.5.0/README.md
--rw-r--r--   0      501       20     3554 2023-01-01 07:52:14.000000 nutpie-0.5.0/README.md-e
--rw-r--r--   0      501       20     5212 2022-06-17 08:42:58.000000 nutpie-0.5.0/benches/run_tvm_leapfrog.rs_old
--rw-r--r--   0      501       20   251122 2023-01-01 06:23:14.000000 nutpie-0.5.0/notebooks/aesara_logp.ipynb-e
--rw-r--r--   0      501       20     7329 2023-01-01 06:23:14.000000 nutpie-0.5.0/notebooks/aesara_logp.md-e
--rw-r--r--   0      501       20   251122 2023-01-02 04:15:03.000000 nutpie-0.5.0/notebooks/pytensor_logp.ipynb
--rw-r--r--   0      501       20   251122 2023-01-01 07:52:13.000000 nutpie-0.5.0/notebooks/pytensor_logp.ipynb-e
--rw-r--r--   0      501       20     7329 2023-01-02 04:15:03.000000 nutpie-0.5.0/notebooks/pytensor_logp.md
--rw-r--r--   0      501       20     7329 2023-01-01 07:52:14.000000 nutpie-0.5.0/notebooks/pytensor_logp.md-e
--rw-r--r--   0      501       20      501 2023-01-01 07:52:14.000000 nutpie-0.5.0/nutpie/__init__.py
--rw-r--r--   0      501       20      501 2023-01-01 07:52:14.000000 nutpie-0.5.0/nutpie/__init__.py-e
--rw-r--r--   0      501       20    12079 2023-01-02 04:15:03.000000 nutpie-0.5.0/nutpie/compile_pymc.py
--rw-r--r--   0      501       20    12079 2023-01-01 07:52:14.000000 nutpie-0.5.0/nutpie/compile_pymc.py-e
--rw-r--r--   0      501       20     2757 2023-01-01 07:52:14.000000 nutpie-0.5.0/nutpie/compile_stan.py
--rw-r--r--   0      501       20     2757 2023-01-01 07:52:14.000000 nutpie-0.5.0/nutpie/compile_stan.py-e
--rw-r--r--   0      501       20     7839 2023-01-01 07:52:14.000000 nutpie-0.5.0/nutpie/sample.py
--rw-r--r--   0      501       20     7839 2023-01-01 07:52:14.000000 nutpie-0.5.0/nutpie/sample.py-e
--rw-r--r--   0      501       20      110 2022-12-31 07:46:26.000000 nutpie-0.5.0/pyproject.toml
--rw-r--r--   0      501       20      830 2023-01-01 07:52:11.000000 nutpie-0.5.0/replace3.sh
--rw-r--r--   0      501       20    17686 2022-12-31 07:46:26.000000 nutpie-0.5.0/src/lib.rs
--rw-r--r--   0      501       20     1591 2023-01-01 07:52:14.000000 nutpie-0.5.0/tests/test_pymc.py
--rw-r--r--   0      501       20     1591 2023-01-01 07:52:14.000000 nutpie-0.5.0/tests/test_pymc.py-e
--rw-r--r--   0      501       20      378 2023-01-01 07:52:14.000000 nutpie-0.5.0/tests/test_stan.py
--rw-r--r--   0      501       20      378 2023-01-01 07:52:14.000000 nutpie-0.5.0/tests/test_stan.py-e
--rw-r--r--   0      501       20    26449 2023-01-03 05:11:04.000000 nutpie-0.5.0/Cargo.lock
--rw-r--r--   0        0        0     3895 1970-01-01 00:00:00.000000 nutpie-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      988 1970-01-01 00:00:00.000000 nutpie-0.6.0/Cargo.toml
+-rw-r--r--   0     1001      123     4882 2023-07-03 17:49:22.000000 nutpie-0.6.0/.github/workflows/ci.yml
+-rw-r--r--   0     1001      123      143 2023-07-03 17:49:22.000000 nutpie-0.6.0/.gitignore
+-rw-r--r--   0     1001      123     1072 2023-07-03 17:49:22.000000 nutpie-0.6.0/LICENSE
+-rw-r--r--   0     1001      123     3583 2023-07-03 17:49:22.000000 nutpie-0.6.0/README.md
+-rw-r--r--   0     1001      123     5212 2023-07-03 17:49:22.000000 nutpie-0.6.0/benches/run_tvm_leapfrog.rs_old
+-rw-r--r--   0     1001      123       10 2023-07-03 17:49:33.000000 nutpie-0.6.0/dist/nutpie-0.6.0.tar.gz
+-rw-r--r--   0     1001      123   251122 2023-07-03 17:49:22.000000 nutpie-0.6.0/notebooks/pytensor_logp.ipynb
+-rw-r--r--   0     1001      123     7329 2023-07-03 17:49:22.000000 nutpie-0.6.0/notebooks/pytensor_logp.md
+-rw-r--r--   0     1001      123      467 2023-07-03 17:49:22.000000 nutpie-0.6.0/nutpie/__init__.py
+-rw-r--r--   0     1001      123    15805 2023-07-03 17:49:22.000000 nutpie-0.6.0/nutpie/compile_pymc.py
+-rw-r--r--   0     1001      123     4395 2023-07-03 17:49:22.000000 nutpie-0.6.0/nutpie/compile_stan.py
+-rw-r--r--   0     1001      123     8231 2023-07-03 17:49:22.000000 nutpie-0.6.0/nutpie/sample.py
+-rw-r--r--   0     1001      123      861 2023-07-03 17:49:22.000000 nutpie-0.6.0/pyproject.toml
+-rw-r--r--   0     1001      123       72 2023-07-03 17:49:22.000000 nutpie-0.6.0/src/lib.rs
+-rw-r--r--   0     1001      123     7955 2023-07-03 17:49:22.000000 nutpie-0.6.0/src/pymc.rs
+-rw-r--r--   0     1001      123     6783 2023-07-03 17:49:22.000000 nutpie-0.6.0/src/sampler.rs
+-rw-r--r--   0     1001      123     9041 2023-07-03 17:49:22.000000 nutpie-0.6.0/src/stan.rs
+-rw-r--r--   0     1001      123     8472 2023-07-03 17:49:22.000000 nutpie-0.6.0/src/wrapper.rs
+-rw-r--r--   0     1001      123     1534 2023-07-03 17:49:22.000000 nutpie-0.6.0/tests/test_pymc.py
+-rw-r--r--   0     1001      123      721 2023-07-03 17:49:22.000000 nutpie-0.6.0/tests/test_stan.py
+-rw-r--r--   0     1001      123    34350 2023-07-03 17:49:22.000000 nutpie-0.6.0/Cargo.lock
+-rw-r--r--   0        0        0     4721 1970-01-01 00:00:00.000000 nutpie-0.6.0/PKG-INFO
```

### Comparing `nutpie-0.5.0/LICENSE` & `nutpie-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nutpie-0.5.0/README.md` & `nutpie-0.6.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -4,31 +4,44 @@
 
 nutpie can be installed using conda or mamba from conda-forge with
 
 ```
 mamba install -c conda-forge nutpie pymc
 ```
 
-To install it from source, install a rust compiler (eg using rustup) and run
+Or using pip:
+
+```
+pip install nutpie
+```
+
+To install it from source, install a rust compiler and maturin and then
 
 ```
 maturin develop --release
 ```
 
 If you want to use the nightly simd implementation for some of the math functions,
-switch to rust nightly and then install with the `simd_support` feature in the nutpie dir:
+switch to rust nightly and then install with the `simd_support` feature in then
+nutpie directory:
 
 ```
 rustup override set nightly
 maturin develop --release --features=simd_support
 ```
 
-## Usage
+## Usage with PyMC
+
+First, PyMC and numba need to be installed, for example using
+
+```
+mamba install pymc numba
+```
 
-First, we need to create a model, for example using pymc:
+We need to create a model:
 
 ```python
 import pymc as pm
 import numpy as np
 import nutpie
 import pandas as pd
 import seaborn as sns
@@ -71,34 +84,61 @@
     )
 ```
 
 We then compile this model and sample form the posterior:
 
 ```python
 compiled_model = nutpie.compile_pymc_model(pymc_model)
-trace_pymc = nutpie.sample(compiled_model, chains=10)
+trace_pymc = nutpie.sample(compiled_model)
 ```
 
 `trace_pymc` now contains an arviz `InferenceData` object, including sampling
 statistics and the posterior of the variables defined above.
 
-For more details, see the example notebook `pytensor_logp`
+## Usage with Stan
+
+In order to sample from stan model, `bridgestan` needs to be installed.
+A pip package is available, but right now this can not be installed using conda.
+
+```
+pip install bridgestan
+```
+
+When we install nutpie with pip, we can also specify that we want optional
+dependencies for Stan models using
+
+```
+pip install 'bridgestan[stan]'
+```
+
+In addition, a C++ compiler needs to be available. For details see
+[the stan docs](https://mc-stan.org/docs/cmdstan-guide/cmdstan-installation.html#cpp-toolchain).
+
+We can then compile a Stan model, and sample using nutpie:
 
-nutpie can also sample from stan models, it currently needs a patched version of httpstan do so so however.
-The required version can be found [here](https://github.com/stan-dev/httpstan/pull/600).
-Make sure to follow the development
-[installation instructions for httpstan](https://httpstan.readthedocs.io/en/latest/installation.html#installation-from-source).
+```
+import nutpie
+
+code = """
+data {
+    real mu;
+}
+parameters {
+    real x;
+}
+model {
+    x ~ normal(mu, 1);
+}
+"""
+
+compiled = nutpie.compile_stan_model(code=code)
+# Provide data
+compiled = compiled.with_data(mu=3.)
+trace = nutpie.sample(compiled)
+```
 
 ## Advantages
 
 nutpie uses `nuts-rs`, a library written in rust, that implements NUTS as in
 pymc and stan, but with a slightly different mass matrix tuning method as
 those. It often produces a higher effective sample size per gradient
 evaluation, and tends to converge faster and with fewer gradient evaluation.
-
-From the benchmarks I did, it seems to be the fastest CPU based sampler I could
-find, outperforming cmdstan and numpyro.
-
-Unfortunately performance on pymc models is currently somewhat limited by an
-[issue in numba](https://github.com/numba/numba/issues/8156), which hopefully
-will be fixed soon. Without the patch mentioned in the issue the model above
-samples in about 2s on my machine, with the patch it finished is about 700ms.
```

### Comparing `nutpie-0.5.0/benches/run_tvm_leapfrog.rs_old` & `nutpie-0.6.0/benches/run_tvm_leapfrog.rs_old`

 * *Files identical despite different names*

### Comparing `nutpie-0.5.0/notebooks/aesara_logp.ipynb-e` & `nutpie-0.6.0/notebooks/pytensor_logp.ipynb`

 * *Files identical despite different names*

### Comparing `nutpie-0.5.0/notebooks/aesara_logp.md-e` & `nutpie-0.6.0/notebooks/pytensor_logp.md`

 * *Files identical despite different names*

### Comparing `nutpie-0.5.0/nutpie/compile_pymc.py` & `nutpie-0.6.0/nutpie/compile_pymc.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,47 +1,68 @@
-from dataclasses import dataclass
 import dataclasses
 import functools
+import itertools
+from dataclasses import dataclass
 from math import prod
-from typing import Dict, List
+from typing import Any, Dict, Optional, Tuple
 
-import pytensor
-import pytensor.tensor as pt
-from numpy.typing import NDArray
-import pymc as pm
-import numpy as np
 import numba
-from pytensor.raise_op import CheckAndRaise
+import numba.core.ccallback
+import numpy as np
+import pandas as pd
+import pymc as pm
+import pytensor
 import pytensor.link.numba.dispatch
+import pytensor.tensor as pt
 from numba import literal_unroll
 from numba.cpython.unsafe.tuple import alloca_once, tuple_setitem
-import numba.core.ccallback
+from numpy.typing import NDArray
 
-from .sample import CompiledModel
 from . import lib
+from .sample import CompiledModel
 
 
 @numba.extending.intrinsic
 def address_as_void_pointer(typingctx, src):
     """returns a void pointer from a given memory address"""
-    from numba.core import types, cgutils
+    from numba.core import cgutils, types
 
     sig = types.voidptr(src)
 
     def codegen(cgctx, builder, sig, args):
         return builder.inttoptr(args[0], cgutils.voidptr_t)
 
     return sig, codegen
 
 
 @dataclass(frozen=True)
 class CompiledPyMCModel(CompiledModel):
     compiled_logp_func: numba.core.ccallback.CFunc
+    compiled_expand_func: numba.core.ccallback.CFunc
     shared_data: Dict[str, NDArray]
     user_data: NDArray
+    n_expanded: int
+    shape_info: Any
+    logp_func: Any
+    expand_func: Any
+    _n_dim: int
+    _shapes: Dict[str, Tuple[int, ...]]
+    _coords: Optional[Dict[str, Any]]
+
+    @property
+    def n_dim(self):
+        return self._n_dim
+
+    @property
+    def shapes(self):
+        return self._shapes
+
+    @property
+    def coords(self):
+        return self._coords
 
     def with_data(self, **updates):
         shared_data = self.shared_data.copy()
         user_data = self.user_data.copy()
         for name, new_val in updates.items():
             if name not in shared_data:
                 raise KeyError(f"Unknown shared variable: {name}")
@@ -51,24 +72,48 @@
             if old_val.ndim != new_val.ndim:
                 raise ValueError(
                     f"Shared variable {name} must have rank {old_val.ndim}"
                 )
             shared_data[name] = new_val
         user_data = update_user_data(user_data, shared_data)
 
-        logp_func_maker = self.logp_func_maker.with_arg(user_data.ctypes.data)
-        expand_draw_fn = functools.partial(
-            self.expand_draw_fn.func, shared_data=shared_data
-        )
         return dataclasses.replace(
             self,
             shared_data=shared_data,
             user_data=user_data,
-            logp_func_maker=logp_func_maker,
-            expand_draw_fn=expand_draw_fn,
+        )
+
+    def _make_sampler(self, settings, init_mean, chains, cores, seed):
+        model = self._make_model(init_mean)
+        return lib.PySampler.from_pymc(settings, chains, cores, model, seed)
+
+    def _make_model(self, init_mean):
+        expand_fn = lib.ExpandFunc(
+            self.n_dim,
+            self.n_expanded,
+            self.compiled_expand_func.address,
+            self.user_data.ctypes.data,
+            self,
+        )
+        logp_fn = lib.LogpFunc(
+            self.n_dim,
+            self.compiled_logp_func.address,
+            self.user_data.ctypes.data,
+            self,
+        )
+
+        var_sizes = [prod(shape) for shape in self.shape_info[2]]
+
+        return lib.PyMcModel(
+            self.n_dim,
+            logp_fn,
+            expand_fn,
+            var_sizes,
+            self.shape_info[0],
+            init_mean,
         )
 
 
 def update_user_data(user_data, user_data_storage):
     user_data = user_data[()]
     for name, val in user_data_storage.items():
         user_data["shared"]["data"][name] = val.ctypes.data
@@ -89,66 +134,92 @@
                     (
                         "shape",
                         [(var.name, np.uint, (var.ndim,)) for var in shared_vars],
                     ),
                 ],
             )
         ],
-        align=True,
     )
     user_data = np.zeros((), dtype=record_dtype)
     update_user_data(user_data, shared_data)
     return user_data
 
 
-def compile_pymc_model(model, **kwargs):
-    """Compile necessary functions for sampling a pymc model."""
+def compile_pymc_model(model: pm.Model, **kwargs) -> CompiledPyMCModel:
+    """Compile necessary functions for sampling a pymc model.
 
-    n_dim, logp_fn_pt, logp_fn, expand_fn, shared_expand, shape_info = _make_functions(
-        model
-    )
+    Parameters
+    ----------
+    model : pymc.Model
+        The model to compile.
+
+    Returns
+    -------
+    compiled_model : CompiledPyMCModel
+        A compiled model object.
+
+    """
+
+    (
+        n_dim,
+        n_expanded,
+        logp_fn_pt,
+        logp_fn,
+        expand_fn_pt,
+        expand_fn,
+        shared_expand,
+        shape_info,
+    ) = _make_functions(model)
 
     shared_data = {val.name: val.get_value().copy() for val in logp_fn_pt.get_shared()}
     for val in shared_data.values():
         val.flags.writeable = False
 
     shared_logp = [var.name for var in logp_fn_pt.get_shared()]
 
     user_data = make_user_data(logp_fn_pt, shared_data)
 
     logp_numba_raw, c_sig = _make_c_logp_func(
         n_dim, logp_fn, user_data, shared_logp, shared_data
     )
     logp_numba = numba.cfunc(c_sig, **kwargs)(logp_numba_raw)
 
-    def expand_draw(x, seed, chain, draw, *, shared_data):
-        return expand_fn(x, **{name: shared_data[name] for name in shared_expand})[0]
-
-    def make_logp_pyfn(data_ptr):
-        return logp_numba.address, data_ptr, None
-
-    logp_func_maker = lib.PtrLogpFuncMaker(
-        make_logp_pyfn,
-        user_data.ctypes.data,
-        n_dim,
-        logp_numba,
+    expand_numba_raw, c_sig_expand = _make_c_expand_func(
+        n_dim, n_expanded, expand_fn, user_data, shared_expand, shared_data
     )
+    expand_numba = numba.cfunc(c_sig_expand, **kwargs)(expand_numba_raw)
 
-    expand_draw_fn = functools.partial(expand_draw, shared_data=shared_data)
+    coords = {name: pd.Index(vals) for name, vals in model.coords.items()}
+    if "unconstrained_parameter" in coords:
+        raise ValueError("Model contains invalid name 'unconstrained_parameter'.")
+
+    names = []
+    for base, _, shape in zip(*shape_info):
+        if base not in [var.name for var in model.value_vars]:
+            continue
+        for idx in itertools.product(*[range(length) for length in shape]):
+            if len(idx) == 0:
+                names.append(base)
+            else:
+                names.append(f"{base}_{'_'.join(str(i) for i in idx)}")
+    coords["unconstrained_parameter"] = pd.Index(names)
 
     return CompiledPyMCModel(
-        n_dim=n_dim,
-        dims=model.RV_dims,
-        coords=model.coords,
-        shape_info=shape_info,
-        logp_func_maker=logp_func_maker,
-        expand_draw_fn=expand_draw_fn,
+        _n_dim=n_dim,
+        dims=model.named_vars_to_dims,
+        _coords=model.coords,
+        _shapes={name: tuple(shape) for name, _, shape in zip(*shape_info)},
         compiled_logp_func=logp_numba,
+        compiled_expand_func=expand_numba,
         shared_data=shared_data,
         user_data=user_data,
+        n_expanded=n_expanded,
+        shape_info=shape_info,
+        logp_func=logp_fn_pt,
+        expand_func=expand_fn_pt,
     )
 
 
 def _compute_shapes(model):
     point = pm.model.make_initial_point_fn(model=model, return_transformed=True)(0)
 
     trace_vars = {
@@ -179,40 +250,73 @@
 
     # Make logp_dlogp_function
     joined = pt.dvector("__joined_variables")
 
     value_vars = [model.rvs_to_values[var] for var in model.free_RVs]
 
     logp = model.logp()
+
+    rewrites = ["canonicalize", "stabilize"]
+    if not model.check_bounds:
+        rewrites.append("local_remove_check_parameter")
+
+    logp = pytensor.graph.rewrite_graph(logp, include=rewrites)
     grads = pytensor.gradient.grad(logp, value_vars)
     grad = pt.concatenate([grad.ravel() for grad in grads])
 
     count = 0
     joined_slices = []
     joined_shapes = []
     joined_names = []
 
-    symbolic_sliced = []
+    splits = []
+
     for var in model.free_RVs:
         value_var = model.rvs_to_values[var]
-
         joined_names.append(value_var.name)
         shape = shapes[value_var.name]
         joined_shapes.append(shape)
         length = prod(shape)
         slice_val = slice(count, count + length)
         joined_slices.append(slice_val)
-        symbolic_sliced.append((value_var, joined[slice_val].reshape(shape)))
         count += length
 
+        splits.append(length)
+
     num_free_vars = count
 
+    joined = pt.TensorType("float64", shape=(num_free_vars,))(
+        name="_unconstrained_point"
+    )
+
+    use_split = False
+    if use_split:
+        variables = pt.split(joined, splits, len(splits))
+    else:
+        variables = [
+            joined[slice_val].reshape(shape)
+            for slice_val, shape in zip(joined_slices, joined_shapes)
+        ]
+
+    replacements = {
+        model.rvs_to_values[var]: value.reshape(shape) if len(shape) != 1 else value
+        for var, shape, value in zip(
+            model.free_RVs,
+            joined_shapes,
+            variables,
+        )
+    }
+
+    (logp, grad) = pytensor.graph_replace([logp, grad], replacements)
+    # (logp, grad) = pytensor.graph.rewrite_graph(logp, include=["canonicalize", "stabilize"])
+    # grad = pytensor.gradient.grad(logp, joined)
+
     # We should avoid compiling the function, and optimize only
     logp_fn_pt = pytensor.compile.function.function(
-        (joined,), (logp, grad), givens=symbolic_sliced, mode=pytensor.compile.NUMBA
+        (joined,), (logp, grad), mode=pytensor.compile.NUMBA
     )
 
     logp_fn = logp_fn_pt.vm.jit_fn
 
     # Make function that computes remaining variables for the trace
     trace_vars = {
         name: var
@@ -234,27 +338,34 @@
         all_names.append(var.name)
         shape = shapes[var.name]
         all_shapes.append(shape)
         length = prod(shape)
         all_slices.append(slice(count, count + length))
         count += length
 
+    num_expanded = count
+
     allvars = pt.concatenate([joined, *[var.ravel() for var in remaining_rvs]])
     expand_fn_pt = pytensor.compile.function.function(
-        (joined,), (allvars,), givens=symbolic_sliced, mode=pytensor.compile.NUMBA
+        (joined,),
+        (allvars,),
+        givens=list(replacements.items()),
+        mode=pytensor.compile.NUMBA,
     )
     expand_fn = expand_fn_pt.vm.jit_fn
     # expand_fn = numba.njit(expand_fn, fastmath=True, error_model="numpy")
     # Trigger a compile
-    expand_fn(np.zeros(num_free_vars), *[var.get_value() for var in expand_fn_pt.get_shared()])
+    # expand_fn(np.zeros(num_free_vars), *[var.get_value() for var in expand_fn_pt.get_shared()])
 
     return (
         num_free_vars,
+        num_expanded,
         logp_fn_pt,
         logp_fn,
+        expand_fn_pt,
         expand_fn,
         [var.name for var in expand_fn_pt.get_shared()],
         (all_names, all_slices, all_shapes),
     )
 
 
 def make_extraction_fn(inner, shared_data, shared_vars, record_dtype):
@@ -278,16 +389,15 @@
 
     names = shared_vars
     indices = tuple(range(len(names)))
     shared_tuple = tuple(shared_data[name] for name in shared_vars)
 
     @numba.extending.intrinsic
     def tuple_setitem_literal(typingctx, tup, idx, val):
-        """Return a copy of the tuple with item at *idx* replaced with *val*.
-        """
+        """Return a copy of the tuple with item at *idx* replaced with *val*."""
         if not isinstance(idx, numba.types.IntegerLiteral):
             return
 
         idx_val = idx.literal_value
         assert idx_val >= 0
         assert idx_val < len(tup)
 
@@ -350,15 +460,14 @@
 
         return inner(x, *_shared_tuple)
 
     return extract_shared
 
 
 def _make_c_logp_func(n_dim, logp_fn, user_data, shared_logp, shared_data):
-
     extract = make_extraction_fn(logp_fn, shared_data, shared_logp, user_data.dtype)
 
     c_sig = numba.types.int64(
         numba.types.uint64,
         numba.types.CPointer(numba.types.double),
         numba.types.CPointer(numba.types.double),
         numba.types.CPointer(numba.types.double),
@@ -385,7 +494,40 @@
             # if np.any(out == 0):
             #    return 4
         except Exception:
             return 1
         return 0
 
     return logp_numba, c_sig
+
+
+def _make_c_expand_func(
+    n_dim, n_expanded, expand_fn, user_data, shared_vars, shared_data
+):
+    extract = make_extraction_fn(expand_fn, shared_data, shared_vars, user_data.dtype)
+
+    c_sig = numba.types.int64(
+        numba.types.uint64,
+        numba.types.uint64,
+        numba.types.CPointer(numba.types.double),
+        numba.types.CPointer(numba.types.double),
+        numba.types.voidptr,
+    )
+
+    def expand_numba(dim, expanded, x_, out_, user_data_):
+        if dim != n_dim:
+            return -1
+        if expanded != n_expanded:
+            return -1
+
+        try:
+            x = numba.carray(x_, (n_dim,))
+            out = numba.carray(out_, (n_expanded,))
+
+            (values,) = extract(x, user_data_)
+            out[...] = values
+
+        except Exception:
+            return -2
+        return 0
+
+    return expand_numba, c_sig
```

### Comparing `nutpie-0.5.0/Cargo.lock` & `nutpie-0.6.0/Cargo.lock`

 * *Files 18% similar despite different names*

```diff
@@ -1,132 +1,260 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
 name = "ahash"
-version = "0.7.6"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fcb51a0695d8f838b1ee009b3fbf66bda078cd64590202a864a8f3e8c4315c47"
+checksum = "2c99f64d1e06488f620f932677e24bc6e2897582980441ae90a671415bd7ec2f"
 dependencies = [
+ "cfg-if",
  "getrandom",
  "once_cell",
  "version_check",
 ]
 
 [[package]]
+name = "android-tzdata"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e999941b234f3131b00bc13c22d06e8c5ff726d1b6318ac7eb276997bbb4fef0"
+
+[[package]]
 name = "anes"
 version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4b46cbb362ab8752921c97e041f5e366ee6297bd428a31275b9fcf1e380f7299"
 
 [[package]]
-name = "atty"
-version = "0.2.14"
+name = "anstyle"
+version = "1.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3a30da5c5f2d5e72842e00bcb57657162cdabef0931f40e2deb9b4140440cecd"
+
+[[package]]
+name = "anyhow"
+version = "1.0.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d9b39be18770d11421cdb1b9947a45dd3f37e93092cbf377614828a319d5fee8"
+checksum = "9c7d0618f0e0b7e8ff11427422b64564d5fb0be1940354bfe2e0529b18a9d9b8"
+
+[[package]]
+name = "arrow2"
+version = "0.17.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "15ae0428d69ab31d7b2adad22a752d6f11fef2e901d2262d0cad4f5cb08b7093"
 dependencies = [
- "hermit-abi 0.1.19",
- "libc",
- "winapi",
+ "ahash",
+ "bytemuck",
+ "chrono",
+ "dyn-clone",
+ "either",
+ "ethnum",
+ "foreign_vec",
+ "getrandom",
+ "hash_hasher",
+ "num-traits",
+ "rustc_version",
+ "simdutf8",
 ]
 
 [[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
+name = "bindgen"
+version = "0.66.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f2b84e06fc203107bfbad243f4aba2af864eb7db3b1cf46ea0a023b0b433d2a7"
+dependencies = [
+ "bitflags 2.3.3",
+ "cexpr",
+ "clang-sys",
+ "lazy_static",
+ "lazycell",
+ "log",
+ "peeking_take_while",
+ "prettyplease",
+ "proc-macro2",
+ "quote",
+ "regex",
+ "rustc-hash",
+ "shlex",
+ "syn 2.0.23",
+ "which",
+]
+
+[[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
+name = "bitflags"
+version = "2.3.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "630be753d4e58660abd17930c71b647fe46c27ea6b63cc59e1e3851406972e42"
+
+[[package]]
+name = "bridgestan"
+version = "2.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "40be108ab686fe2710a841b5e9473de9d5823c436200b9eb0b25e5a3a36afe90"
+dependencies = [
+ "bindgen",
+ "libloading 0.8.0",
+ "thiserror",
+]
+
+[[package]]
 name = "bumpalo"
-version = "3.11.1"
+version = "3.13.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a3e2c3daef883ecc1b5d58c15adae93470a91d425f3532ba1695849656af3fc1"
+
+[[package]]
+name = "bytemuck"
+version = "1.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "572f695136211188308f16ad2ca5c851a712c464060ae6974944458eb83880ba"
+checksum = "17febce684fd15d89027105661fec94afb475cb995fbc59d2865198446ba2eea"
+dependencies = [
+ "bytemuck_derive",
+]
+
+[[package]]
+name = "bytemuck_derive"
+version = "1.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fdde5c9cd29ebd706ce1b35600920a33550e402fc998a2e53ad3b42c3c47a192"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.23",
+]
 
 [[package]]
 name = "cast"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "37b2a672a2cb129a2e41c10b1224bb368f9f37a2b16b612598138befd7b37eb5"
 
 [[package]]
+name = "cc"
+version = "1.0.79"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "50d30906286121d95be3d479533b458f87493b30a4b5f79a607db8f5d11aa91f"
+
+[[package]]
+name = "cexpr"
+version = "0.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6fac387a98bb7c37292057cffc56d62ecb629900026402633ae9160df93a8766"
+dependencies = [
+ "nom",
+]
+
+[[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
+name = "chrono"
+version = "0.4.26"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ec837a71355b28f6556dbd569b37b3f363091c0bd4b2e735674521b4c5fd9bc5"
+dependencies = [
+ "android-tzdata",
+ "num-traits",
+]
+
+[[package]]
 name = "ciborium"
-version = "0.2.0"
+version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b0c137568cc60b904a7724001b35ce2630fd00d5d84805fbb608ab89509d788f"
+checksum = "effd91f6c78e5a4ace8a5d3c0b6bfaec9e2baaef55f3efc00e45fb2e477ee926"
 dependencies = [
  "ciborium-io",
  "ciborium-ll",
  "serde",
 ]
 
 [[package]]
 name = "ciborium-io"
-version = "0.2.0"
+version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "346de753af073cc87b52b2083a506b38ac176a44cfb05497b622e27be899b369"
+checksum = "cdf919175532b369853f5d5e20b26b43112613fd6fe7aee757e35f7a44642656"
 
 [[package]]
 name = "ciborium-ll"
-version = "0.2.0"
+version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "213030a2b5a4e0c0892b6652260cf6ccac84827b83a85a534e178e3906c4cf1b"
+checksum = "defaa24ecc093c77630e6c15e17c51f5e187bf35ee514f4e2d67baaa96dae22b"
 dependencies = [
  "ciborium-io",
  "half",
 ]
 
 [[package]]
+name = "clang-sys"
+version = "1.6.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c688fc74432808e3eb684cae8830a86be1d66a2bd58e1f248ed0960a590baf6f"
+dependencies = [
+ "glob",
+ "libc",
+ "libloading 0.7.4",
+]
+
+[[package]]
 name = "clap"
-version = "3.2.23"
+version = "4.3.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "71655c45cb9845d3270c9d6df84ebe72b4dad3c2ba3f7023ad47c144e4e473a5"
+checksum = "384e169cc618c613d5e3ca6404dda77a8685a63e08660dcc64abaf7da7cb0c7a"
 dependencies = [
- "bitflags",
- "clap_lex",
- "indexmap",
- "textwrap",
+ "clap_builder",
 ]
 
 [[package]]
-name = "clap_lex"
-version = "0.2.4"
+name = "clap_builder"
+version = "4.3.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2850f2f5a82cbf437dd5af4d49848fbdfc27c157c3d010345776f952765261c5"
+checksum = "ef137bbe35aab78bdb468ccfba75a5f4d8321ae011d34063770780545176af2d"
 dependencies = [
- "os_str_bytes",
+ "anstyle",
+ "clap_lex",
 ]
 
 [[package]]
+name = "clap_lex"
+version = "0.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2da6da31387c7e4ef160ffab6d5e7f00c42626fe39aea70a7b0f1773f7dd6c1b"
+
+[[package]]
 name = "criterion"
-version = "0.4.0"
+version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e7c76e09c1aae2bc52b3d2f29e13c6572553b30c4aa1b8a49fd70de6412654cb"
+checksum = "f2b12d017a929603d80db1831cd3a24082f8137ce19c69e6447f54f5fc8d692f"
 dependencies = [
  "anes",
- "atty",
  "cast",
  "ciborium",
  "clap",
  "criterion-plot",
- "itertools",
- "lazy_static",
+ "is-terminal",
+ "itertools 0.10.5",
  "num-traits",
+ "once_cell",
  "oorandom",
  "plotters",
  "rayon",
  "regex",
  "serde",
  "serde_derive",
  "serde_json",
@@ -137,15 +265,15 @@
 [[package]]
 name = "criterion-plot"
 version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6b50826342786a51a89e2da3a28f1c32b06e387201bc2d19791f622c673706b1"
 dependencies = [
  "cast",
- "itertools",
+ "itertools 0.10.5",
 ]
 
 [[package]]
 name = "crossbeam"
 version = "0.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2801af0d36612ae591caa9568261fddce32ce6e08a7275ea334a06a4ad021a2c"
@@ -156,43 +284,43 @@
  "crossbeam-epoch",
  "crossbeam-queue",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-channel"
-version = "0.5.6"
+version = "0.5.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c2dd04ddaf88237dc3b8d8f9a3c1004b506b54b3313403944054d23c0870c521"
+checksum = "a33c2bf77f2df06183c3aa30d1e96c0695a313d4f9c453cc3762a6db39f99200"
 dependencies = [
  "cfg-if",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-deque"
-version = "0.8.2"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "715e8152b692bba2d374b53d4875445368fdf21a94751410af607a5ac677d1fc"
+checksum = "ce6fd6f855243022dcecf8702fef0c297d4338e226845fe067f6341ad9fa0cef"
 dependencies = [
  "cfg-if",
  "crossbeam-epoch",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-epoch"
-version = "0.9.13"
+version = "0.9.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "01a9af1f4c2ef74bb8aa1f7e19706bc72d03598c8a570bb5de72243c7a9d9d5a"
+checksum = "ae211234986c545741a7dc064309f67ee1e5ad243d0e48335adc0484d960bcc7"
 dependencies = [
  "autocfg",
  "cfg-if",
  "crossbeam-utils",
- "memoffset 0.7.1",
+ "memoffset",
  "scopeguard",
 ]
 
 [[package]]
 name = "crossbeam-queue"
 version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -200,191 +328,269 @@
 dependencies = [
  "cfg-if",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-utils"
-version = "0.8.14"
+version = "0.8.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4fb766fa798726286dbbb842f174001dab8abc7b627a1dd86e0b7222a95d929f"
+checksum = "5a22b2d63d4d1dc0b7f1b6b2747dd0088008a9be28b6ddf0b1e7d335e3037294"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
+name = "dyn-clone"
+version = "1.0.11"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "68b0cf012f1230e43cd00ebb729c6bb58707ecfa8ad08b52ef3a4ccd2697fc30"
+
+[[package]]
 name = "either"
-version = "1.8.0"
+version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "90e5c1c8368803113bf0c9584fc495a58b86dc8a29edbf8fe877d21d9507e797"
+checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
+
+[[package]]
+name = "errno"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4bcfec3a70f97c962c307b2d2c56e358cf1d00b558d74262b5f929ee8cc7e73a"
+dependencies = [
+ "errno-dragonfly",
+ "libc",
+ "windows-sys",
+]
+
+[[package]]
+name = "errno-dragonfly"
+version = "0.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "aa68f1b12764fab894d2755d2518754e71b4fd80ecfb822714a1206c2aab39bf"
+dependencies = [
+ "cc",
+ "libc",
+]
+
+[[package]]
+name = "ethnum"
+version = "1.3.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "0198b9d0078e0f30dedc7acbb21c974e838fc8fae3ee170128658a98cb2c1c04"
+
+[[package]]
+name = "foreign_vec"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ee1b05cbd864bcaecbd3455d6d967862d446e4ebfc3c2e5e5b9841e53cba6673"
 
 [[package]]
 name = "getrandom"
-version = "0.2.8"
+version = "0.2.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c05aeb6a22b8f62540c194aac980f2115af067bfe15a0734d7277a768d396b31"
+checksum = "be4136b2a15dd319360be1c07d9933517ccf0be8f16bf62a3bee4f0d618df427"
 dependencies = [
  "cfg-if",
+ "js-sys",
  "libc",
  "wasi",
+ "wasm-bindgen",
 ]
 
 [[package]]
+name = "glob"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d2fabcfbdc87f4758337ca535fb41a6d701b65693ce38287d856d1674551ec9b"
+
+[[package]]
 name = "half"
 version = "1.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "eabb4a44450da02c90444cf74558da904edde8fb4e9035a9a6a4e15445af0bd7"
 
 [[package]]
-name = "hashbrown"
-version = "0.12.3"
+name = "hash_hasher"
+version = "2.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
+checksum = "74721d007512d0cb3338cd20f0654ac913920061a4c4d0d8708edb3f2a698c0c"
 
 [[package]]
 name = "hermit-abi"
-version = "0.1.19"
+version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "62b467343b94ba476dcb2500d242dadbb39557df889310ac77c5d99100aaac33"
-dependencies = [
- "libc",
-]
+checksum = "fed44880c466736ef9a5c5b5facefb5ed0785676d0c02d612db14e54f0d84286"
 
 [[package]]
-name = "hermit-abi"
-version = "0.2.6"
+name = "indoc"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ee512640fe35acbfb4bb779db6f0d80704c2cacfa2e39b601ef3e3f47d1ae4c7"
-dependencies = [
- "libc",
-]
+checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
-name = "indexmap"
-version = "1.9.2"
+name = "is-terminal"
+version = "0.4.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1885e79c1fc4b10f0e172c475f458b7f7b93061064d98c3293e98c5ba0c8b399"
+checksum = "24fddda5af7e54bf7da53067d6e802dbcc381d0a8eef629df528e3ebf68755cb"
 dependencies = [
- "autocfg",
- "hashbrown",
+ "hermit-abi",
+ "rustix",
+ "windows-sys",
 ]
 
 [[package]]
-name = "indoc"
-version = "1.0.8"
+name = "itertools"
+version = "0.10.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da2d6f23ffea9d7e76c53eee25dfb67bcd8fde7f1198b0855350698c9f07c780"
+checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
+dependencies = [
+ "either",
+]
 
 [[package]]
 name = "itertools"
-version = "0.10.5"
+version = "0.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
+checksum = "b1c173a5686ce8bfa551b3563d0c2170bf24ca44da99c7ca4bfdab5418c3fe57"
 dependencies = [
  "either",
 ]
 
 [[package]]
 name = "itoa"
-version = "1.0.5"
+version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fad582f4b9e86b6caa621cabeb0963332d92eea04729ab12892c2533951e6440"
+checksum = "c0aa48fab2893d8a49caa94082ae8488f4e1050d73b367881dcd2198f4199fd8"
 
 [[package]]
 name = "js-sys"
-version = "0.3.60"
+version = "0.3.64"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "49409df3e3bf0856b916e2ceaca09ee28e6871cf7d9ce97a692cacfdb2a25a47"
+checksum = "c5f195fe497f702db0f318b07fdd68edb16955aed830df8363d837542f8f935a"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
+name = "lazycell"
+version = "1.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "830d08ce1d1d941e6b30645f1a0eb5643013d835ce3779a5fc208261dbe10f55"
+
+[[package]]
 name = "libc"
-version = "0.2.139"
+version = "0.2.147"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b4668fb0ea861c1df094127ac5f1da3409a82116a4ba74fca2e58ef927159bb3"
+
+[[package]]
+name = "libloading"
+version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "201de327520df007757c1f0adce6e827fe8562fbc28bfd9c15571c66ca1f5f79"
+checksum = "b67380fd3b2fbe7527a606e18729d21c6f3951633d0500574c4dc22d2d638b9f"
+dependencies = [
+ "cfg-if",
+ "winapi",
+]
+
+[[package]]
+name = "libloading"
+version = "0.8.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d580318f95776505201b28cf98eb1fa5e4be3b689633ba6a3e6cd880ff22d8cb"
+dependencies = [
+ "cfg-if",
+ "windows-sys",
+]
 
 [[package]]
 name = "libm"
-version = "0.2.6"
+version = "0.2.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f7012b1bbb0719e1097c47611d3898568c546d597c2e74d66f6087edd5233ff4"
+
+[[package]]
+name = "linux-raw-sys"
+version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "348108ab3fba42ec82ff6e9564fc4ca0247bdccdc68dd8af9764bbc79c3c8ffb"
+checksum = "09fc20d2ca12cb9f044c93e3bd6d32d523e6e2ec3db4f7b2939cd99026ecd3f0"
 
 [[package]]
 name = "lock_api"
-version = "0.4.9"
+version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
+checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.17"
+version = "0.4.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "abb12e687cfb44aa40f41fc3978ef76448f9b6038cad6aef4259d3c095a2382e"
-dependencies = [
- "cfg-if",
-]
+checksum = "b06a4cde4c0f271a446782e3eff8de789548ce57dbc8eca9292c27f4a42004b4"
 
 [[package]]
 name = "matrixmultiply"
-version = "0.3.2"
+version = "0.3.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "add85d4dd35074e6fedc608f8c8f513a3548619a9024b751949ef0e8e45a4d84"
+checksum = "090126dc04f95dc0d1c1c91f61bdd474b3930ca064c1edc8a849da2c6cbe1e77"
 dependencies = [
+ "autocfg",
  "rawpointer",
 ]
 
 [[package]]
-name = "memoffset"
-version = "0.6.5"
+name = "memchr"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5aa361d4faea93603064a027415f07bd8e1d5c88c9fbf68bf56a285428fd79ce"
-dependencies = [
- "autocfg",
-]
+checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
 
 [[package]]
 name = "memoffset"
-version = "0.7.1"
+version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5de893c32cde5f383baa4c04c5d6dbdd735cfd4a794b0debdb2bb1b421da5ff4"
+checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
+name = "minimal-lexical"
+version = "0.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "68354c5c6bd36d73ff3feceb05efa59b6acb7626617f4962be322a825e61f79a"
+
+[[package]]
 name = "multiversion"
-version = "0.7.1"
+version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e6a87eede2251ca235e5573086d01d2ab6b59dfaea54c2be10f9320980f7e8f7"
+checksum = "8cda45dade5144c2c929bf2ed6c24bebbba784e9198df049ec87d722b9462bd1"
 dependencies = [
  "multiversion-macros",
  "target-features",
 ]
 
 [[package]]
 name = "multiversion-macros"
-version = "0.7.1"
+version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1af1abf82261d780d114014eff4b555e47d823f3b84f893c4388572b40e089fb"
+checksum = "04bffdccbd4798b61dce08c97ce8c66a68976f95541aaf284a6e90c1d1c306e1"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
  "target-features",
 ]
 
 [[package]]
 name = "ndarray"
 version = "0.15.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -394,18 +600,28 @@
  "num-complex",
  "num-integer",
  "num-traits",
  "rawpointer",
 ]
 
 [[package]]
+name = "nom"
+version = "7.1.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d273983c5a657a70a3e8f2a01329822f3b8c8172b73826411a55751e404a0a4a"
+dependencies = [
+ "memchr",
+ "minimal-lexical",
+]
+
+[[package]]
 name = "num-complex"
-version = "0.4.2"
+version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ae39348c8bc5fbd7f40c727a9925f03517afd2ab27d46702108b6a7e5414c19"
+checksum = "02e0d21255c828d6f128a1e41534206671e8c3ea0c62f32291e808dc82cff17d"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "num-integer"
 version = "0.1.45"
@@ -424,216 +640,234 @@
 dependencies = [
  "autocfg",
  "libm",
 ]
 
 [[package]]
 name = "num_cpus"
-version = "1.15.0"
+version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0fac9e2da13b5eb447a6ce3d392f23a29d8694bff781bf03a16cd9ac8697593b"
+checksum = "4161fcb6d602d4d2081af7c3a45852d875a03dd337a6bfdd6e06407b61342a43"
 dependencies = [
- "hermit-abi 0.2.6",
+ "hermit-abi",
  "libc",
 ]
 
 [[package]]
 name = "numpy"
-version = "0.17.2"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a462c1af5ba1fddec1488c4646993a23ae7931f9e170ccba23e9c7c834277797"
+checksum = "437213adf41bbccf4aeae535fbfcdad0f6fed241e1ae182ebe97fa1f3ce19389"
 dependencies = [
- "ahash",
  "libc",
  "ndarray",
  "num-complex",
  "num-integer",
  "num-traits",
  "pyo3",
+ "rustc-hash",
 ]
 
 [[package]]
 name = "nutpie"
-version = "0.5.0"
+version = "0.6.0"
 dependencies = [
+ "anyhow",
+ "arrow2",
+ "bridgestan",
  "criterion",
- "crossbeam",
+ "itertools 0.11.0",
  "ndarray",
  "numpy",
  "nuts-rs",
  "pyo3",
  "rand",
+ "rand_chacha",
+ "rayon",
  "thiserror",
 ]
 
 [[package]]
 name = "nuts-rs"
-version = "0.4.1"
+version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a70c6c986a8b0641690cdc3a15e522482b3a8930340ed775acb511735208fbea"
+checksum = "aa23fb9109210d6afebc5b9f4c06827c2d6985838a911b8ff75cd4f75aa7c79f"
 dependencies = [
+ "anyhow",
+ "arrow2",
  "crossbeam",
- "itertools",
+ "itertools 0.11.0",
  "multiversion",
- "ndarray",
  "rand",
+ "rand_chacha",
  "rand_distr",
  "rayon",
  "thiserror",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.17.0"
+version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6f61fba1741ea2b3d6a1e3178721804bb716a68a6aeba1149b5d52e3d464ea66"
+checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
 name = "oorandom"
 version = "11.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ab1bc2a289d34bd04a330323ac98a1b4bc82c9d9fcb1e66b63caa84da26b575"
 
 [[package]]
-name = "os_str_bytes"
-version = "6.4.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9b7820b9daea5457c9f21c69448905d723fbd21136ccf521748f23fd49e723ee"
-
-[[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.5"
+version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ff9f3fef3968a3ec5945535ed654cb38ff72d7495a25619e2247fb15a2ed9ba"
+checksum = "93f00c865fe7cabf650081affecd3871070f26767e7b2070a3ffae14c654b447"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-sys",
+ "windows-targets",
 ]
 
 [[package]]
+name = "peeking_take_while"
+version = "0.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "19b17cddbe7ec3f8bc800887bab5e717348c95ea2ca0b1bf0837fb964dc67099"
+
+[[package]]
 name = "plotters"
-version = "0.3.4"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2538b639e642295546c50fcd545198c9d64ee2a38620a628724a3b266d5fbf97"
+checksum = "d2c224ba00d7cadd4d5c660deaf2098e5e80e07846537c51f9cfa4be50c1fd45"
 dependencies = [
  "num-traits",
  "plotters-backend",
  "plotters-svg",
  "wasm-bindgen",
  "web-sys",
 ]
 
 [[package]]
 name = "plotters-backend"
-version = "0.3.4"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "193228616381fecdc1224c62e96946dfbc73ff4384fba576e052ff8c1bea8142"
+checksum = "9e76628b4d3a7581389a35d5b6e2139607ad7c75b17aed325f210aa91f4a9609"
 
 [[package]]
 name = "plotters-svg"
-version = "0.3.3"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f9a81d2759aae1dae668f783c308bc5c8ebd191ff4184aaa1b37f65a6ae5a56f"
+checksum = "38f6d39893cca0701371e3c27294f09797214b86f1fb951b89ade8ec04e2abab"
 dependencies = [
  "plotters-backend",
 ]
 
 [[package]]
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
+name = "prettyplease"
+version = "0.2.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9825a04601d60621feed79c4e6b56d65db77cdca55cef43b46b0de1096d1c282"
+dependencies = [
+ "proc-macro2",
+ "syn 2.0.23",
+]
+
+[[package]]
 name = "proc-macro2"
-version = "1.0.49"
+version = "1.0.63"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "57a8eca9f9c4ffde41714334dee777596264c7825420f521abc92b5b5deb63a5"
+checksum = "7b368fba921b0dce7e60f5e04ec15e565b3303972b42bcfde1d0713b881959eb"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.17.3"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "268be0c73583c183f2b14052337465768c07726936a260f480f0857cb95ba543"
+checksum = "ffb88ae05f306b4bfcde40ac4a51dc0b05936a9207a4b75b798c7729c4258a59"
 dependencies = [
+ "anyhow",
  "cfg-if",
  "indoc",
  "libc",
- "memoffset 0.6.5",
+ "memoffset",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.17.3"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "28fcd1e73f06ec85bf3280c48c67e731d8290ad3d730f8be9dc07946923005c8"
+checksum = "554db24f0b3c180a9c0b1268f91287ab3f17c162e15b54caaae5a6b3773396b0"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.17.3"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0f6cb136e222e49115b3c51c32792886defbfb0adead26a688142b346a0b9ffc"
+checksum = "922ede8759e8600ad4da3195ae41259654b9c55da4f7eec84a0ccc7d067a70a4"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.17.3"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "94144a1266e236b1c932682136dc35a9dee8d3589728f68130c7c3861ef96b28"
+checksum = "8a5caec6a1dd355964a841fcbeeb1b89fe4146c87295573f94228911af3cc5a2"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.17.3"
+version = "0.19.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c8df9be978a2d2f0cdebabb03206ed73b11314701a5bfe71b0d753b81997777f"
+checksum = "e0b78ccbb160db1556cdb6fd96c50334c5d4ec44dc5e0a968d0a1208fa0efa8b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.23"
+version = "1.0.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8856d8364d252a14d474036ea1358d63c9e6965c8e5c1885c18f73d70bff9c7b"
+checksum = "573015e8ab27661678357f27dc26460738fd2b6c86e46f386fde94cb5d913105"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -678,63 +912,91 @@
 name = "rawpointer"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "60a357793950651c4ed0f3f52338f53b2f809f32d83a07f72909fa13e4c6c1e3"
 
 [[package]]
 name = "rayon"
-version = "1.6.1"
+version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6db3a213adf02b3bcfd2d3846bb41cb22857d131789e01df434fb7e7bc0759b7"
+checksum = "1d2df5196e37bcc87abebc0053e20787d73847bb33134a69841207dd0a47f03b"
 dependencies = [
  "either",
  "rayon-core",
 ]
 
 [[package]]
 name = "rayon-core"
-version = "1.10.1"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cac410af5d00ab6884528b4ab69d1e8e146e8d471201800fa1b4524126de6ad3"
+checksum = "4b8f95bd6966f5c87776639160a66bd8ab9895d9d4ab01ddba9fc60661aebe8d"
 dependencies = [
  "crossbeam-channel",
  "crossbeam-deque",
  "crossbeam-utils",
  "num_cpus",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.2.16"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
+checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
- "bitflags",
+ "bitflags 1.3.2",
 ]
 
 [[package]]
 name = "regex"
-version = "1.7.0"
+version = "1.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e076559ef8e241f2ae3479e36f97bd5741c0330689e217ad51ce2c76808b868a"
+checksum = "d0ab3ca65655bb1e41f2a8c8cd662eb4fb035e67c3f78da1d61dffe89d07300f"
 dependencies = [
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.6.28"
+version = "0.7.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "436b050e76ed2903236f032a59761c1eb99e1b0aead2c257922771dab1fc8c78"
+
+[[package]]
+name = "rustc-hash"
+version = "1.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
+
+[[package]]
+name = "rustc_version"
+version = "0.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
+dependencies = [
+ "semver",
+]
+
+[[package]]
+name = "rustix"
+version = "0.38.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "456c603be3e8d448b072f410900c09faf164fbce2d480456f50eea6e25f9c848"
+checksum = "aabcb0461ebd01d6b79945797c27f8529082226cb630a9865a71870ff63532a4"
+dependencies = [
+ "bitflags 2.3.3",
+ "errno",
+ "libc",
+ "linux-raw-sys",
+ "windows-sys",
+]
 
 [[package]]
 name = "ryu"
-version = "1.0.12"
+version = "1.0.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b4b9743ed687d4b4bcedf9ff5eaa7398495ae14e61cba0a295704edbc7decde"
+checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
 
 [[package]]
 name = "same-file"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "93fc1dc3aaa9bfed95e02e6eadabb4baf7e3078b0bd1b4d7b6b0b68378900502"
 dependencies = [
@@ -744,114 +1006,137 @@
 [[package]]
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
+name = "semver"
+version = "1.0.17"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bebd363326d05ec3e2f532ab7660680f3b02130d780c299bca73469d521bc0ed"
+
+[[package]]
 name = "serde"
-version = "1.0.152"
+version = "1.0.165"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bb7d1f0d3021d347a83e556fc4683dea2ea09d87bccdf88ff5c12545d89d5efb"
+checksum = "c939f902bb7d0ccc5bce4f03297e161543c2dcb30914faf032c2bd0b7a0d48fc"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.152"
+version = "1.0.165"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "af487d118eecd09402d70a5d72551860e788df87b464af30e5ea6a38c75c541e"
+checksum = "6eaae920e25fffe4019b75ff65e7660e72091e59dd204cb5849bbd6a3fd343d7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.91"
+version = "1.0.99"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "877c235533714907a8c2464236f5c4b2a17262ef1bd71f38f35ea592c8da6883"
+checksum = "46266871c240a00b8f503b877622fe33430b3c7d963bdc0f2adc511e54a1eae3"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
+name = "shlex"
+version = "1.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "43b2853a4d09f215c24cc5489c992ce46052d359b5109343cbafbf26bc62f8a3"
+
+[[package]]
+name = "simdutf8"
+version = "0.1.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f27f6278552951f1f2b8cf9da965d10969b2efdea95a6ec47987ab46edfe263a"
+
+[[package]]
 name = "smallvec"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
 
 [[package]]
 name = "syn"
-version = "1.0.107"
+version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1f4064b5b16e03ae50984a5a8ed5d4f8803e6bc1fd170a3cda91a1be4b18e3f5"
+checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
-name = "target-features"
-version = "0.1.1"
+name = "syn"
+version = "2.0.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3a50a4fd5a723c3f94b5db8561fcf72a4bf3a1a3b40c35bc4ff5c5e6efeb35e4"
+checksum = "59fb7d6d8281a51045d62b8eb3a7d1ce347b76f312af50cd3dc0af39c87c1737"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "unicode-ident",
+]
 
 [[package]]
-name = "target-lexicon"
-version = "0.12.5"
+name = "target-features"
+version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9410d0f6853b1d94f0e519fb95df60f29d2c1eff2d921ffdf01a4c8a3b54f12d"
+checksum = "06f6b473c37f9add4cf1df5b4d66a8ef58ab6c895f1a3b3f949cf3e21230140e"
 
 [[package]]
-name = "textwrap"
-version = "0.16.0"
+name = "target-lexicon"
+version = "0.12.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "222a222a5bfe1bba4a77b45ec488a741b3cb8872e5e499451fd7d0129c9c7c3d"
+checksum = "1b1c7f239eb94671427157bd93b3694320f3668d4e1eff08c7285366fd777fac"
 
 [[package]]
 name = "thiserror"
-version = "1.0.38"
+version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6a9cd18aa97d5c45c6603caea1da6628790b37f7a34b6ca89522331c5180fed0"
+checksum = "978c9a314bd8dc99be594bc3c175faaa9794be04a5a5e153caba6915336cebac"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.38"
+version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1fb327af4685e4d03fa8cbcf1716380da910eeb2bb8be417e7f9fd3fb164f36f"
+checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.23",
 ]
 
 [[package]]
 name = "tinytemplate"
 version = "1.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "be4d6b5f19ff7664e8c98d03e2139cb510db9b0a60b55f8e8709b689d939b6bc"
 dependencies = [
  "serde",
  "serde_json",
 ]
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.6"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "84a22b9f218b40614adcb3f4ff08b703773ad44fa9423e4e0d346d5db86e4ebc"
+checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
 
 [[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
@@ -859,94 +1144,104 @@
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
 [[package]]
 name = "walkdir"
-version = "2.3.2"
+version = "2.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "808cf2735cd4b6866113f648b791c6adc5714537bc222d9347bb203386ffda56"
+checksum = "36df944cda56c7d8d8b7496af378e6b16de9284591917d307c9b4d313c44e698"
 dependencies = [
  "same-file",
- "winapi",
  "winapi-util",
 ]
 
 [[package]]
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.83"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eaf9f5aceeec8be17c128b2e93e031fb8a4d469bb9c4ae2d7dc1888b26887268"
+checksum = "7706a72ab36d8cb1f80ffbf0e071533974a60d0a308d01a5d0375bf60499a342"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.83"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c8ffb332579b0557b52d268b91feab8df3615f265d5270fec2a8c95b17c1142"
+checksum = "5ef2b6d3c510e9625e5fe6f509ab07d66a760f0885d858736483c32ed7809abd"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.23",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.83"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "052be0f94026e6cbc75cdefc9bae13fd6052cdcaf532fa6c45e7ae33a1e6c810"
+checksum = "dee495e55982a3bd48105a7b947fd2a9b4a8ae3010041b9e0faab3f9cd028f1d"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.83"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "07bc0c051dc5f23e307b13285f9d75df86bfdf816c5721e573dec1f9b8aa193c"
+checksum = "54681b18a46765f095758388f2d0cf16eb8d4169b639ab575a8f5693af210c7b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.23",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.83"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1c38c045535d93ec4f0b4defec448e4291638ee608530863b1e2ba115d4fff7f"
+checksum = "ca6ad05a4870b2bf5fe995117d3728437bd27d7cd5f06f13c17443ef369775a1"
 
 [[package]]
 name = "web-sys"
-version = "0.3.60"
+version = "0.3.64"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bcda906d8be16e728fd5adc5b729afad4e444e106ab28cd1c7256e54fa61510f"
+checksum = "9b85cbef8c220a6abc02aefd892dfc0fc23afb1c6a426316ec33253a3877249b"
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
+name = "which"
+version = "4.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2441c784c52b289a054b7201fc93253e288f094e2f4be9058343127c4226a269"
+dependencies = [
+ "either",
+ "libc",
+ "once_cell",
+]
+
+[[package]]
 name = "winapi"
 version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
 dependencies = [
  "winapi-i686-pc-windows-gnu",
  "winapi-x86_64-pc-windows-gnu",
@@ -971,61 +1266,70 @@
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
 name = "windows-sys"
-version = "0.42.0"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
+dependencies = [
+ "windows-targets",
+]
+
+[[package]]
+name = "windows-targets"
+version = "0.48.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a3e1820f08b8513f676f7ab6c1f99ff312fb97b553d30ff4dd86f9f15728aa7"
+checksum = "05d4b17490f70499f20b9e791dcf6a299785ce8af4d709018206dc5b4953e95f"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
  "windows_i686_gnu",
  "windows_i686_msvc",
  "windows_x86_64_gnu",
  "windows_x86_64_gnullvm",
  "windows_x86_64_msvc",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "41d2aa71f6f0cbe00ae5167d90ef3cfe66527d6f613ca78ac8024c3ccab9a19e"
+checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dd0f252f5a35cac83d6311b2e795981f5ee6e67eb1f9a7f64eb4500fbc4dcdb4"
+checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fbeae19f6716841636c28d695375df17562ca208b2b7d0dc47635a50ae6c5de7"
+checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "84c12f65daa39dd2babe6e442988fc329d6243fdce47d7d2d155b8d874862246"
+checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf7b1b21b5362cbc318f686150e5bcea75ecedc74dd157d874d754a2ca44b0ed"
+checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "09d525d2ba30eeb3297665bd434a54297e4170c7f1a44cad4ef58095b4cd2028"
+checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f40009d85759725a34da6d89a94e63d7bdc50a862acf0dbc7c8e488f1edcb6f5"
+checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
```

