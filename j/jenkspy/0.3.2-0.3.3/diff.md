# Comparing `tmp/jenkspy-0.3.2.tar.gz` & `tmp/jenkspy-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jenkspy-0.3.2.tar", last modified: Thu Nov 10 10:03:13 2022, max compression
+gzip compressed data, was "jenkspy-0.3.3.tar", last modified: Mon Jul  3 10:23:17 2023, max compression
```

## Comparing `jenkspy-0.3.2.tar` & `jenkspy-0.3.3.tar`

### file list

```diff
@@ -1,25 +1,17 @@
-drwxrwxr-x   0 mthh      (1000) mthh      (1000)        0 2022-11-10 10:03:13.283964 jenkspy-0.3.2/
--rwxrwxr-x   0 mthh      (1000) mthh      (1000)     1075 2022-08-11 15:40:53.000000 jenkspy-0.3.2/LICENSE
--rwxrwxr-x   0 mthh      (1000) mthh      (1000)      125 2022-08-23 20:01:39.000000 jenkspy-0.3.2/MANIFEST.in
--rw-rw-r--   0 mthh      (1000) mthh      (1000)     5930 2022-11-10 10:03:13.283964 jenkspy-0.3.2/PKG-INFO
--rw-rw-r--   0 mthh      (1000) mthh      (1000)     5150 2022-08-23 09:28:38.000000 jenkspy-0.3.2/README.rst
-drwxrwxr-x   0 mthh      (1000) mthh      (1000)        0 2022-11-10 10:03:13.279964 jenkspy-0.3.2/jenkspy/
--rw-rw-r--   0 mthh      (1000) mthh      (1000)      241 2022-11-10 09:59:39.000000 jenkspy-0.3.2/jenkspy/__init__.py
--rw-rw-r--   0 mthh      (1000) mthh      (1000)     7819 2022-11-10 09:57:19.000000 jenkspy-0.3.2/jenkspy/core.py
-drwxrwxr-x   0 mthh      (1000) mthh      (1000)        0 2022-11-10 10:03:13.283964 jenkspy-0.3.2/jenkspy/src/
--rw-rw-r--   0 mthh      (1000) mthh      (1000)     5730 2022-08-23 08:32:02.000000 jenkspy-0.3.2/jenkspy/src/_jenks.c
--rw-rw-r--   0 mthh      (1000) mthh      (1000)   837386 2022-09-01 12:08:38.000000 jenkspy-0.3.2/jenkspy/src/jenks.c
--rwxrwxr-x   0 mthh      (1000) mthh      (1000)     4150 2022-08-23 08:34:02.000000 jenkspy-0.3.2/jenkspy/src/jenks.pyx
-drwxrwxr-x   0 mthh      (1000) mthh      (1000)        0 2022-11-10 10:03:13.283964 jenkspy-0.3.2/jenkspy.egg-info/
--rw-rw-r--   0 mthh      (1000) mthh      (1000)     5930 2022-11-10 10:03:13.000000 jenkspy-0.3.2/jenkspy.egg-info/PKG-INFO
--rw-rw-r--   0 mthh      (1000) mthh      (1000)      363 2022-11-10 10:03:13.000000 jenkspy-0.3.2/jenkspy.egg-info/SOURCES.txt
--rw-rw-r--   0 mthh      (1000) mthh      (1000)        1 2022-11-10 10:03:13.000000 jenkspy-0.3.2/jenkspy.egg-info/dependency_links.txt
--rw-rw-r--   0 mthh      (1000) mthh      (1000)        6 2022-11-10 10:03:13.000000 jenkspy-0.3.2/jenkspy.egg-info/requires.txt
--rw-rw-r--   0 mthh      (1000) mthh      (1000)        8 2022-11-10 10:03:13.000000 jenkspy-0.3.2/jenkspy.egg-info/top_level.txt
--rw-rw-r--   0 mthh      (1000) mthh      (1000)        5 2022-08-22 11:32:28.000000 jenkspy-0.3.2/requirements.txt
--rw-rw-r--   0 mthh      (1000) mthh      (1000)       38 2022-11-10 10:03:13.283964 jenkspy-0.3.2/setup.cfg
--rw-rw-r--   0 mthh      (1000) mthh      (1000)     1836 2022-08-22 21:59:52.000000 jenkspy-0.3.2/setup.py
-drwxrwxr-x   0 mthh      (1000) mthh      (1000)        0 2022-11-10 10:03:13.283964 jenkspy-0.3.2/tests/
--rwxrwxr-x   0 mthh      (1000) mthh      (1000)        0 2022-08-11 09:50:36.000000 jenkspy-0.3.2/tests/__init__.py
--rw-rw-r--   0 mthh      (1000) mthh      (1000)    36567 2022-08-11 11:20:32.000000 jenkspy-0.3.2/tests/test.json
--rwxrwxr-x   0 mthh      (1000) mthh      (1000)    48248 2022-11-10 09:57:19.000000 jenkspy-0.3.2/tests/test_jenks.py
+drwxrwxr-x   0 mthh      (1000) mthh      (1000)        0 2023-07-03 10:23:17.716018 jenkspy-0.3.3/
+-rwxrwxr-x   0 mthh      (1000) mthh      (1000)     1075 2023-07-03 10:04:21.116016 jenkspy-0.3.3/LICENSE
+-rw-rw-r--   0 mthh      (1000) mthh      (1000)     6972 2023-07-03 10:23:17.716018 jenkspy-0.3.3/PKG-INFO
+-rw-rw-r--   0 mthh      (1000) mthh      (1000)     5163 2023-07-03 10:04:21.116016 jenkspy-0.3.3/README.rst
+drwxrwxr-x   0 mthh      (1000) mthh      (1000)        0 2023-07-03 10:23:17.716018 jenkspy-0.3.3/jenkspy/
+-rw-rw-r--   0 mthh      (1000) mthh      (1000)      241 2023-07-03 10:18:44.676017 jenkspy-0.3.3/jenkspy/__init__.py
+-rw-rw-r--   0 mthh      (1000) mthh      (1000)     8440 2023-07-03 10:15:47.820017 jenkspy-0.3.3/jenkspy/core.py
+drwxrwxr-x   0 mthh      (1000) mthh      (1000)        0 2023-07-03 10:23:17.716018 jenkspy-0.3.3/jenkspy/src/
+-rw-rw-r--   0 mthh      (1000) mthh      (1000)     5730 2023-07-03 10:04:21.116016 jenkspy-0.3.3/jenkspy/src/_jenks.c
+-rw-rw-r--   0 mthh      (1000) mthh      (1000)   837386 2023-07-03 10:04:21.120016 jenkspy-0.3.3/jenkspy/src/jenks.c
+-rwxrwxr-x   0 mthh      (1000) mthh      (1000)     4150 2023-07-03 10:04:21.120016 jenkspy-0.3.3/jenkspy/src/jenks.pyx
+-rw-rw-r--   0 mthh      (1000) mthh      (1000)        5 2023-07-03 10:04:21.120016 jenkspy-0.3.3/requirements.txt
+-rw-rw-r--   0 mthh      (1000) mthh      (1000)     1927 2023-07-03 10:04:21.120016 jenkspy-0.3.3/setup.py
+drwxrwxr-x   0 mthh      (1000) mthh      (1000)        0 2023-07-03 10:23:17.716018 jenkspy-0.3.3/tests/
+-rwxrwxr-x   0 mthh      (1000) mthh      (1000)        0 2023-07-03 10:04:21.120016 jenkspy-0.3.3/tests/__init__.py
+-rw-rw-r--   0 mthh      (1000) mthh      (1000)    36567 2023-07-03 10:04:21.124016 jenkspy-0.3.3/tests/test.json
+-rwxrwxr-x   0 mthh      (1000) mthh      (1000)    48973 2023-07-03 10:16:43.168017 jenkspy-0.3.3/tests/test_jenks.py
```

### Comparing `jenkspy-0.3.2/LICENSE` & `jenkspy-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jenkspy-0.3.2/PKG-INFO` & `jenkspy-0.3.3/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: jenkspy
-Version: 0.3.2
-Summary: Compute Natural Breaks (Fisher-Jenks algorithm)
-Home-page: http://github.com/mthh/jenkspy
-Author: Matthieu Viry
-Author-email: matthieu.viry@cnrs.fr
-License: MIT
-Platform: UNKNOWN
-Classifier: Programming Language :: Python
-Classifier: Development Status :: 4 - Beta
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
 Fast Fisher-Jenks breaks for Python
 ===================================
 
 Compute "natural breaks" (*Fisher-Jenks algorithm*) on list / tuple / array / numpy.ndarray of integers/floats.
 
 The algorithm implemented by this library is also sometimes referred to as *Fisher-Jenks algorithm*, *Jenks Optimisation Method* or *Fisher exact optimization method*. This is a deterministic method to calculate the optimal class boundaries.
 
@@ -131,17 +109,15 @@
 -  Getting the break values! (and fast!). No fancy functionality provided,
    but contributions/forks/etc are welcome.
 -  Other python implementations are currently existing but not as fast or not available on PyPi.
 
 .. |Build status GH| image:: https://github.com/mthh/jenkspy/actions/workflows/wheel.yml/badge.svg
    :target: https://github.com/mthh/jenkspy/actions/workflows/wheel.yml
 
-.. |Version| image:: https://img.shields.io/pypi/v/jenkspy.svg
+.. |Version| image:: https://img.shields.io/pypi/v/jenkspy.svg?color=007ec6
    :target: https://pypi.python.org/pypi/jenkspy
 
 .. |Anaconda-Server Badge| image:: https://anaconda.org/conda-forge/jenkspy/badges/version.svg
    :target: https://anaconda.org/conda-forge/jenkspy
 
 .. |PyPI download month| image:: https://img.shields.io/pypi/dm/jenkspy.svg
    :target: https://pypi.python.org/pypi/jenkspy
-
-
```

### Comparing `jenkspy-0.3.2/jenkspy/core.py` & `jenkspy-0.3.3/jenkspy/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,16 +11,28 @@
     """
 
     def __init__(self, n_classes: int = 6) -> None:
         """
         Parameters
         ----------
         n_classes : int
-            The number of classes to be generated by the classifier.
+            The number of classes to be generated by the classifier (should be a positive integer).
         """
+        if isinstance(n_classes, float) and int(n_classes) == n_classes:
+            n_classes = int(n_classes)
+        if not isinstance(n_classes, int):
+            raise TypeError(
+                "Number of class have to be a positive integer: "
+                "expected an instance of 'int' but found {}"
+                .format(type(n_classes)))
+        if n_classes < 1:
+            raise ValueError(
+                "Number of class have to be an integer "
+                "greater than or equal to 1"
+            )
         self.n_classes = n_classes
 
     def __repr__(self) -> str:
         return f"JenksNaturalBreaks(n_classes={self.n_classes})"
 
     def __str__(self) -> str:
         return f"JenksNaturalBreaks(n_classes={self.n_classes})"
@@ -69,14 +81,16 @@
             The sequence of numbers (integer/float) to be classified.
 
         Returns
         -------
         list of numpy.array
             The list of groups that contains the values of x.
         """
+        if self.n_classes == 1:
+            return [np.array(x)]
         arr = np.array(x)
         groups_ = [arr[arr <= self.inner_breaks_[0]]]
         for idx in range(len(self.inner_breaks_))[:-1]:
             groups_.append(arr[(arr > self.inner_breaks_[idx])*(arr <= self.inner_breaks_[idx + 1])])
         groups_.append(arr[arr > self.inner_breaks_[-1]])
         return groups_
```

### Comparing `jenkspy-0.3.2/jenkspy/src/_jenks.c` & `jenkspy-0.3.3/jenkspy/src/_jenks.c`

 * *Files identical despite different names*

### Comparing `jenkspy-0.3.2/jenkspy/src/jenks.c` & `jenkspy-0.3.3/jenkspy/src/jenks.c`

 * *Files identical despite different names*

### Comparing `jenkspy-0.3.2/jenkspy/src/jenks.pyx` & `jenkspy-0.3.3/jenkspy/src/jenks.pyx`

 * *Files identical despite different names*

### Comparing `jenkspy-0.3.2/jenkspy.egg-info/PKG-INFO` & `jenkspy-0.3.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,147 +1,145 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: jenkspy
-Version: 0.3.2
+Version: 0.3.3
 Summary: Compute Natural Breaks (Fisher-Jenks algorithm)
-Home-page: http://github.com/mthh/jenkspy
+Home-page: https://github.com/mthh/jenkspy
 Author: Matthieu Viry
 Author-email: matthieu.viry@cnrs.fr
 License: MIT
+Description: Fast Fisher-Jenks breaks for Python
+        ===================================
+        
+        Compute "natural breaks" (*Fisher-Jenks algorithm*) on list / tuple / array / numpy.ndarray of integers/floats.
+        
+        The algorithm implemented by this library is also sometimes referred to as *Fisher-Jenks algorithm*, *Jenks Optimisation Method* or *Fisher exact optimization method*. This is a deterministic method to calculate the optimal class boundaries.
+        
+        Intended compatibility: CPython 3.6+
+        
+        Wheels are provided via PyPI for Windows / MacOS / Linux users - Also available on conda-forge channel for Anaconda users.
+        
+        |Version| |Anaconda-Server Badge| |Build Status GH| |PyPI download month|
+        
+        Usage
+        -----
+        
+        Two ways of using `jenkspy` are available:
+        
+        - by using the ``jenks_breaks`` function which takes as input a `list <https://docs.python.org/3/library/stdtypes.html#list>`_ / `tuple <https://docs.python.org/3/library/stdtypes.html#tuple>`_ / `array.array <https://docs.python.org/3/library/array.html#array.array>`_ / `numpy.ndarray <https://numpy.org/doc/stable/reference/generated/numpy.ndarray.html>`_ of integers or floats and returns a list of values that correspond to the limits of the classes (starting with the minimum value of the series - the lower bound of the first class - and ending with its maximum value - the upper bound of the last class).
+        
+        .. code:: python
+        
+            >>> import jenkspy
+            >>> import json
+        
+            >>> with open('tests/test.json', 'r') as f:
+            ...     # Read some data from a JSON file
+            ...     data = json.loads(f.read())
+            ...
+            >>> jenkspy.jenks_breaks(data, n_classes=5) # Asking for 5 classes
+            [0.0028109620325267315, 2.0935479691252112, 4.205495140049607, 6.178148351609707, 8.09175917180255, 9.997982932254672]
+            # ^                      ^                    ^                 ^                  ^                 ^
+            # Lower bound            Upper bound          Upper bound       Upper bound        Upper bound       Upper bound
+            # 1st class              1st class            2nd class         3rd class          4th class         5th class
+            # (Minimum value)                                                                                    (Maximum value)
+        
+        
+        - by using the ``JenksNaturalBreaks`` class that is inspired by ``scikit-learn`` classes.
+        
+        The ``.fit`` and ``.group`` behavior is slightly different from ``jenks_breaks``, by accepting value outside the range of the minimum and maximum value of ``breaks_``, retaining the input size. It means that fit and group will use only the ``inner_breaks_``. All value below the min bound will be included in the first group and all value higher than the max bound will be included in the last group.
+        
+        .. code:: python
+        
+            >>> from jenkspy import JenksNaturalBreaks
+        
+            >>> x = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11]
+        
+            >>> jnb = JenksNaturalBreaks(4) # Asking for 4 clusters
+        
+            >>> jnb.fit(x) # Create the clusters according to values in 'x'
+            >>> print(jnb.labels_) # Labels for fitted data
+            ... print(jnb.groups_) # Content of each group
+            ... print(jnb.breaks_) # Break values (including min and max)
+            ... print(jnb.inner_breaks_) # Inner breaks (ie breaks_[1:-1])
+            [0 0 0 1 1 1 2 2 2 3 3 3]
+            [array([0, 1, 2]), array([3, 4, 5]), array([6, 7, 8]), array([ 9, 10, 11])]
+            [0.0, 2.0, 5.0, 8.0, 11.0]
+            [2.0, 5.0, 8.0]
+        
+            >>> print(jnb.predict(15)) # Predict the group of a value
+            3
+        
+            >>> print(jnb.predict([2.5, 3.5, 6.5])) # Predict the group of several values
+            [1 1 2]
+        
+            >>> print(jnb.group([2.5, 3.5, 6.5])) # Group the elements into there groups
+            [array([], dtype=float64), array([2.5, 3.5]), array([6.5]), array([], dtype=float64)]
+        
+        
+        Installation
+        ------------
+        
+        + **From pypi**
+        
+        .. code:: shell
+        
+            pip install jenkspy
+        
+        
+        + **From source**
+        
+        .. code:: shell
+        
+            git clone http://github.com/mthh/jenkspy
+            cd jenkspy/
+            python setup.py install
+        
+        + **For anaconda users**
+        
+        .. code:: shell
+        
+            conda install -c conda-forge jenkspy
+        
+        
+        Requirements :
+        --------------
+        
+        - `Numpy <https://numpy.org>`_
+        
+        -  Only for building from source: C compiler, Python C headers and optionally Cython.
+        
+        
+        Motivation :
+        ------------
+        
+        -  Making a painless installing C extension so it could be used more easily
+           as a dependency in an other package (and so learning how to build wheels
+           using *appveyor* / *travis* at first - now it uses *GitHub Actions*).
+        -  Getting the break values! (and fast!). No fancy functionality provided,
+           but contributions/forks/etc are welcome.
+        -  Other python implementations are currently existing but not as fast or not available on PyPi.
+        
+        .. |Build status GH| image:: https://github.com/mthh/jenkspy/actions/workflows/wheel.yml/badge.svg
+           :target: https://github.com/mthh/jenkspy/actions/workflows/wheel.yml
+        
+        .. |Version| image:: https://img.shields.io/pypi/v/jenkspy.svg?color=007ec6
+           :target: https://pypi.python.org/pypi/jenkspy
+        
+        .. |Anaconda-Server Badge| image:: https://anaconda.org/conda-forge/jenkspy/badges/version.svg
+           :target: https://anaconda.org/conda-forge/jenkspy
+        
+        .. |PyPI download month| image:: https://img.shields.io/pypi/dm/jenkspy.svg
+           :target: https://pypi.python.org/pypi/jenkspy
+        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
-Fast Fisher-Jenks breaks for Python
-===================================
-
-Compute "natural breaks" (*Fisher-Jenks algorithm*) on list / tuple / array / numpy.ndarray of integers/floats.
-
-The algorithm implemented by this library is also sometimes referred to as *Fisher-Jenks algorithm*, *Jenks Optimisation Method* or *Fisher exact optimization method*. This is a deterministic method to calculate the optimal class boundaries.
-
-Intended compatibility: CPython 3.6+
-
-Wheels are provided via PyPI for Windows / MacOS / Linux users - Also available on conda-forge channel for Anaconda users.
-
-|Version| |Anaconda-Server Badge| |Build Status GH| |PyPI download month|
-
-Usage
------
-
-Two ways of using `jenkspy` are available:
-
-- by using the ``jenks_breaks`` function which takes as input a `list <https://docs.python.org/3/library/stdtypes.html#list>`_ / `tuple <https://docs.python.org/3/library/stdtypes.html#tuple>`_ / `array.array <https://docs.python.org/3/library/array.html#array.array>`_ / `numpy.ndarray <https://numpy.org/doc/stable/reference/generated/numpy.ndarray.html>`_ of integers or floats and returns a list of values that correspond to the limits of the classes (starting with the minimum value of the series - the lower bound of the first class - and ending with its maximum value - the upper bound of the last class).
-
-.. code:: python
-
-    >>> import jenkspy
-    >>> import json
-
-    >>> with open('tests/test.json', 'r') as f:
-    ...     # Read some data from a JSON file
-    ...     data = json.loads(f.read())
-    ...
-    >>> jenkspy.jenks_breaks(data, n_classes=5) # Asking for 5 classes
-    [0.0028109620325267315, 2.0935479691252112, 4.205495140049607, 6.178148351609707, 8.09175917180255, 9.997982932254672]
-    # ^                      ^                    ^                 ^                  ^                 ^
-    # Lower bound            Upper bound          Upper bound       Upper bound        Upper bound       Upper bound
-    # 1st class              1st class            2nd class         3rd class          4th class         5th class
-    # (Minimum value)                                                                                    (Maximum value)
-
-
-- by using the ``JenksNaturalBreaks`` class that is inspired by ``scikit-learn`` classes.
-
-The ``.fit`` and ``.group`` behavior is slightly different from ``jenks_breaks``, by accepting value outside the range of the minimum and maximum value of ``breaks_``, retaining the input size. It means that fit and group will use only the ``inner_breaks_``. All value below the min bound will be included in the first group and all value higher than the max bound will be included in the last group.
-
-.. code:: python
-
-    >>> from jenkspy import JenksNaturalBreaks
-
-    >>> x = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11]
-
-    >>> jnb = JenksNaturalBreaks(4) # Asking for 4 clusters
-
-    >>> jnb.fit(x) # Create the clusters according to values in 'x'
-    >>> print(jnb.labels_) # Labels for fitted data
-    ... print(jnb.groups_) # Content of each group
-    ... print(jnb.breaks_) # Break values (including min and max)
-    ... print(jnb.inner_breaks_) # Inner breaks (ie breaks_[1:-1])
-    [0 0 0 1 1 1 2 2 2 3 3 3]
-    [array([0, 1, 2]), array([3, 4, 5]), array([6, 7, 8]), array([ 9, 10, 11])]
-    [0.0, 2.0, 5.0, 8.0, 11.0]
-    [2.0, 5.0, 8.0]
-
-    >>> print(jnb.predict(15)) # Predict the group of a value
-    3
-
-    >>> print(jnb.predict([2.5, 3.5, 6.5])) # Predict the group of several values
-    [1 1 2]
-
-    >>> print(jnb.group([2.5, 3.5, 6.5])) # Group the elements into there groups
-    [array([], dtype=float64), array([2.5, 3.5]), array([6.5]), array([], dtype=float64)]
-
-
-Installation
-------------
-
-+ **From pypi**
-
-.. code:: shell
-
-    pip install jenkspy
-
-
-+ **From source**
-
-.. code:: shell
-
-    git clone http://github.com/mthh/jenkspy
-    cd jenkspy/
-    python setup.py install
-
-+ **For anaconda users**
-
-.. code:: shell
-
-    conda install -c conda-forge jenkspy
-
-
-Requirements :
---------------
-
-- `Numpy <https://numpy.org>`_
-
--  Only for building from source: C compiler, Python C headers and optionally Cython.
-
-
-Motivation :
-------------
-
--  Making a painless installing C extension so it could be used more easily
-   as a dependency in an other package (and so learning how to build wheels
-   using *appveyor* / *travis* at first - now it uses *GitHub Actions*).
--  Getting the break values! (and fast!). No fancy functionality provided,
-   but contributions/forks/etc are welcome.
--  Other python implementations are currently existing but not as fast or not available on PyPi.
-
-.. |Build status GH| image:: https://github.com/mthh/jenkspy/actions/workflows/wheel.yml/badge.svg
-   :target: https://github.com/mthh/jenkspy/actions/workflows/wheel.yml
-
-.. |Version| image:: https://img.shields.io/pypi/v/jenkspy.svg
-   :target: https://pypi.python.org/pypi/jenkspy
-
-.. |Anaconda-Server Badge| image:: https://anaconda.org/conda-forge/jenkspy/badges/version.svg
-   :target: https://anaconda.org/conda-forge/jenkspy
-
-.. |PyPI download month| image:: https://img.shields.io/pypi/dm/jenkspy.svg
-   :target: https://pypi.python.org/pypi/jenkspy
-
-
+Classifier: Typing :: Typed
```

### Comparing `jenkspy-0.3.2/setup.py` & `jenkspy-0.3.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,21 +42,23 @@
     description="Compute Natural Breaks (Fisher-Jenks algorithm)",
     long_description=long_desc,
     long_description_content_type='text/x-rst',
     install_requires=requirements,
     test_suite="tests",
     author="Matthieu Viry",
     author_email="matthieu.viry@cnrs.fr",
-    url='http://github.com/mthh/jenkspy',
+    url='https://github.com/mthh/jenkspy',
     classifiers=[
         "Programming Language :: Python",
-        "Development Status :: 4 - Beta",
+        "Development Status :: 5 - Production/Stable",
         "Operating System :: OS Independent",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Scientific/Engineering",
+        "Typing :: Typed",
     ],
 )
```

### Comparing `jenkspy-0.3.2/tests/test.json` & `jenkspy-0.3.3/tests/test.json`

 * *Files identical despite different names*

### Comparing `jenkspy-0.3.2/tests/test_jenks.py` & `jenkspy-0.3.3/tests/test_jenks.py`

 * *Files 0% similar despite different names*

```diff
@@ -274,9 +274,34 @@
         for group_fit, group_true in zip(jnb.group(150), self.res8):
             self.assertEqual((group_fit == group_true).all(), True)
         for group_fit, group_true in zip(jnb.group([150, 700]), self.res9):
             self.assertEqual((group_fit == group_true).all(), True)
         for group_fit, group_true in zip(jnb.group(np.array([150, 700])), self.res9):
             self.assertEqual((group_fit == group_true).all(), True)
 
+    def test_one_class(self):
+        """
+        JenksNaturalBreaks should also work if only one classe is asked.
+        """
+        jnb = JenksNaturalBreaks(n_classes=1)
+        jnb.fit(self.data2)
+        g = jnb.group(1000.)
+        self.assertEqual(g, [np.array(1000.)])
+        l = jnb.get_label_(1000.)
+        self.assertEqual(l, 0)
+
+    def test_zero_class(self):
+        """
+        JenksNaturalBreaks shouldn't work with less than 1 class.
+        """
+        with self.assertRaises(ValueError):
+            jnb = JenksNaturalBreaks(0)
+
+        with self.assertRaises(ValueError):
+            jnb = JenksNaturalBreaks(-12)
+
+        with self.assertRaises(TypeError):
+            jnb = JenksNaturalBreaks("abc")
+
+
 if __name__ == "__main__":
     unittest.main()
```

