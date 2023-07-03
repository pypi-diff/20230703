# Comparing `tmp/parcoords-0.1.2.tar.gz` & `tmp/parcoords-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parcoords-0.1.2.tar", last modified: Sat Jul  1 15:35:55 2023, max compression
+gzip compressed data, was "parcoords-0.1.3.tar", last modified: Mon Jul  3 16:39:09 2023, max compression
```

## Comparing `parcoords-0.1.2.tar` & `parcoords-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 15:35:55.377490 parcoords-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-01 15:35:46.000000 parcoords-0.1.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-07-01 15:35:55.377490 parcoords-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-01 15:35:46.000000 parcoords-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 15:35:55.377490 parcoords-0.1.2/parcoords/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-01 15:35:46.000000 parcoords-0.1.2/parcoords/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-07-01 15:35:46.000000 parcoords-0.1.2/parcoords/parcoords.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-01 15:35:55.377490 parcoords-0.1.2/parcoords.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-07-01 15:35:55.000000 parcoords-0.1.2/parcoords.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-01 15:35:55.000000 parcoords-0.1.2/parcoords.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-01 15:35:55.000000 parcoords-0.1.2/parcoords.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-01 15:35:55.000000 parcoords-0.1.2/parcoords.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-01 15:35:55.000000 parcoords-0.1.2/parcoords.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-01 15:35:55.377490 parcoords-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-01 15:35:46.000000 parcoords-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:39:09.469583 parcoords-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-03 16:38:59.000000 parcoords-0.1.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-03 16:39:09.469583 parcoords-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-07-03 16:38:59.000000 parcoords-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:39:09.465583 parcoords-0.1.3/parcoords/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-03 16:38:59.000000 parcoords-0.1.3/parcoords/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-07-03 16:38:59.000000 parcoords-0.1.3/parcoords/parcoords.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 16:39:09.469583 parcoords-0.1.3/parcoords.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-07-03 16:39:09.000000 parcoords-0.1.3/parcoords.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-03 16:39:09.000000 parcoords-0.1.3/parcoords.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 16:39:09.000000 parcoords-0.1.3/parcoords.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-03 16:39:09.000000 parcoords-0.1.3/parcoords.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-03 16:39:09.000000 parcoords-0.1.3/parcoords.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 16:39:09.469583 parcoords-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-03 16:38:59.000000 parcoords-0.1.3/setup.py
```

### Comparing `parcoords-0.1.2/LICENSE.txt` & `parcoords-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `parcoords-0.1.2/parcoords/parcoords.py` & `parcoords-0.1.3/parcoords/parcoords.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import Union, Sequence
+from __future__ import annotations
+from typing import Union, Sequence, Tuple
 
 import numpy as np
 
 import matplotlib.colors
 import matplotlib.pyplot as plt
 from matplotlib.scale import ScaleBase
 
@@ -10,45 +11,46 @@
 def plot_parcoords(
     values: Union[Sequence, np.ndarray],
     labels: Union[Sequence[str], np.ndarray[str]] = None,
     title: str = None,
     color_field: Union[str, int] = None,
     color="grey",
     scale: Union[
-        Sequence[tuple[Union[str, int], Union[str, ScaleBase]]],
+        Sequence[Tuple[Union[str, int], Union[str, ScaleBase]]],
         Sequence[Union[str, ScaleBase]],
         str,
     ] = None,
-    figsize: tuple[int, int] = None,
+    figsize: Tuple[int, int] = None,
     cmap=plt.cm.viridis,
     y_limits: Union[Sequence, np.ndarray] = None,
     axs: np.ndarray[plt.Axes] = None,
-) -> tuple[plt.Figure, np.ndarray[plt.Axes]]:
+) -> Tuple[plt.Figure, np.ndarray[plt.Axes]]:
     """Plotting function for parallel coordinate plots.
+
     :param values: 2-dimensional sequence or numpy-array containing
-                   row-vectors of the data to display. (required)
+        row-vectors of the data to display. (required)
     :param labels: Sequence containing the column labels. (optional)
     :param title: Title of the figure. (optional)
     :param color_field: Either the label of the column (`labels` must be provided)
-                        or the column index used as basis for the coloring. If not
-                        provided, the `color` attribute will be used. (optional)
+        or the column index used as basis for the coloring. If not
+        provided, the `color` attribute will be used. (optional)
     :param color: Color of the edges when `color_field` attribute is not provided.
-                  (default: grey)
+        (default: grey)
     :param scale: Sequence of scale types. Must be in one of the forms:
-                  [({field label/index}, {"linear", "log", ...}), ...] or
-                  [{"linear", "log", ...}, ...] or
-                  {"linear", "log", ...}.
-                  (optional, default: linear)
+        [({field label/index}, {"linear", "log", ...}), ...] or
+        [{"linear", "log", ...}, ...] or
+        {"linear", "log", ...}.
+        (optional, default: linear)
     :param figsize: Size of the figure. (optional)
     :param cmap: The colormap for the edge-colors (to be used together with
-                 `color_field`). (default: viridis)
+        `color_field`). (default: viridis)
     :param y_limits: The min- & max-limits for the axes. Must be in the form of:
-                     [(`min`, `max`), ...] for all axes. (optional)
+        [(`min`, `max`), ...] for all axes. (optional)
     :param axs: An existing axes array, to be used when adding more datapoints.
-                (optional)
+        (optional)
     :return: The figure object and the axes (as ndarray).
     """
     # transpose row-vector to column-vector
     if not isinstance(values, np.ndarray):
         values = np.array(values, dtype="object")
     values = values.T
 
@@ -73,14 +75,23 @@
             if y_limits is None:
                 smallest = column.min(axis=0)
                 largest = column.max(axis=0)
                 ylims.append([smallest, largest])
         if y_limits is None:
             y_limits = ylims
     else:
+        for i, (column, ax) in enumerate(zip(values, axs)):
+            if not all(isinstance(item, (int, float)) for item in column):
+                for x, value in enumerate(column):
+                    if isinstance(value, str):
+                        column[x] = {
+                            text.get_text(): i
+                            for i, text in enumerate(ax.get_yticklabels())
+                        }[value]
+                values[i] = column
         if y_limits is not None:
             print(
                 "Warning: setting `y_limits` when using existing axes has no effect."
             )
             y_limits = None
         if scale is not None:
             print(
@@ -184,10 +195,11 @@
                 c=l_color,
                 transform=axs[i].transAxes,
             )
 
     if fig:
         fig.subplots_adjust(wspace=0)
         fig.subplots_adjust(top=0.85)
-        fig.suptitle(title)
+        if title is not None:
+            fig.suptitle(title)
 
     return fig, axs
```

