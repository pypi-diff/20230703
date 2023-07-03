# Comparing `tmp/aiida-wannier90-2.0.1.tar.gz` & `tmp/aiida_wannier90-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aiida-wannier90-2.0.1.tar", last modified: Wed Mar 18 15:33:58 2020, max compression
+gzip compressed data, was "aiida_wannier90-2.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aiida-wannier90-2.0.1.tar` & `aiida_wannier90-2.1.0.tar`

### file list

```diff
@@ -1,28 +1,18 @@
-drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2020-03-18 15:33:58.000000 aiida-wannier90-2.0.1/
--rw-r--r--   0 pizzi      (501) staff       (20)     2226 2020-03-18 15:33:58.000000 aiida-wannier90-2.0.1/PKG-INFO
--rw-r--r--   0 pizzi      (501) staff       (20)     1804 2020-03-18 15:31:57.000000 aiida-wannier90-2.0.1/setup.json
--rw-r--r--   0 pizzi      (501) staff       (20)       39 2020-03-06 12:38:52.000000 aiida-wannier90-2.0.1/MANIFEST.in
--rw-r--r--   0 pizzi      (501) staff       (20)     1027 2020-03-06 12:38:52.000000 aiida-wannier90-2.0.1/README.md
--rw-r--r--   0 pizzi      (501) staff       (20)     1316 2020-03-06 12:38:52.000000 aiida-wannier90-2.0.1/setup.py
-drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2020-03-18 15:33:58.000000 aiida-wannier90-2.0.1/aiida_wannier90.egg-info/
--rw-r--r--   0 pizzi      (501) staff       (20)     2226 2020-03-18 15:33:57.000000 aiida-wannier90-2.0.1/aiida_wannier90.egg-info/PKG-INFO
--rw-r--r--   0 pizzi      (501) staff       (20)      602 2020-03-18 15:33:58.000000 aiida-wannier90-2.0.1/aiida_wannier90.egg-info/SOURCES.txt
--rw-r--r--   0 pizzi      (501) staff       (20)      281 2020-03-18 15:33:57.000000 aiida-wannier90-2.0.1/aiida_wannier90.egg-info/entry_points.txt
--rw-r--r--   0 pizzi      (501) staff       (20)      363 2020-03-18 15:33:57.000000 aiida-wannier90-2.0.1/aiida_wannier90.egg-info/requires.txt
--rw-r--r--   0 pizzi      (501) staff       (20)       16 2020-03-18 15:33:57.000000 aiida-wannier90-2.0.1/aiida_wannier90.egg-info/top_level.txt
--rw-r--r--   0 pizzi      (501) staff       (20)        1 2020-03-18 15:33:57.000000 aiida-wannier90-2.0.1/aiida_wannier90.egg-info/dependency_links.txt
--rw-r--r--   0 pizzi      (501) staff       (20)       38 2020-03-18 15:33:58.000000 aiida-wannier90-2.0.1/setup.cfg
--rwxr-xr-x   0 pizzi      (501) staff       (20)     1303 2020-03-06 12:38:52.000000 aiida-wannier90-2.0.1/LICENSE.txt
-drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2020-03-18 15:33:58.000000 aiida-wannier90-2.0.1/aiida_wannier90/
--rw-r--r--   0 pizzi      (501) staff       (20)    13745 2020-03-06 12:38:52.000000 aiida-wannier90-2.0.1/aiida_wannier90/orbitals.py
-drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2020-03-18 15:33:58.000000 aiida-wannier90-2.0.1/aiida_wannier90/io/
--rw-r--r--   0 pizzi      (501) staff       (20)    13282 2020-03-06 12:38:52.000000 aiida-wannier90-2.0.1/aiida_wannier90/io/_write_win.py
--rw-r--r--   0 pizzi      (501) staff       (20)      869 2020-03-06 12:38:52.000000 aiida-wannier90-2.0.1/aiida_wannier90/io/__init__.py
--rw-r--r--   0 pizzi      (501) staff       (20)     1577 2020-03-06 12:38:52.000000 aiida-wannier90-2.0.1/aiida_wannier90/io/_group_list.py
-drwxr-xr-x   0 pizzi      (501) staff       (20)        0 2020-03-18 15:33:58.000000 aiida-wannier90-2.0.1/aiida_wannier90/workflows/
--rw-r--r--   0 pizzi      (501) staff       (20)      672 2020-03-06 12:38:52.000000 aiida-wannier90-2.0.1/aiida_wannier90/workflows/__init__.py
--rw-r--r--   0 pizzi      (501) staff       (20)    12312 2020-03-18 15:31:57.000000 aiida-wannier90-2.0.1/aiida_wannier90/workflows/minimal.py
--rw-r--r--   0 pizzi      (501) staff       (20)     2248 2020-03-18 15:31:57.000000 aiida-wannier90-2.0.1/aiida_wannier90/__init__.py
--rw-r--r--   0 pizzi      (501) staff       (20)    19640 2020-03-06 12:38:52.000000 aiida-wannier90-2.0.1/aiida_wannier90/parsers.py
--rw-r--r--   0 pizzi      (501) staff       (20)    20975 2020-03-06 12:38:52.000000 aiida-wannier90-2.0.1/aiida_wannier90/calculations.py
--rw-r--r--   0 pizzi      (501) staff       (20)     3380 2020-03-06 12:38:52.000000 aiida-wannier90-2.0.1/aiida_wannier90/utils.py
+-rw-r--r--   0        0        0     1301 2023-07-03 18:09:05.977599 aiida_wannier90-2.1.0/LICENSE.txt
+-rw-r--r--   0        0        0     2118 2023-07-03 18:09:06.101597 aiida_wannier90-2.1.0/README.md
+-rw-r--r--   0        0        0     4929 2023-07-03 18:09:06.189596 aiida_wannier90-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1973 2023-07-03 18:09:06.189596 aiida_wannier90-2.1.0/src/aiida_wannier90/__init__.py
+-rw-r--r--   0        0        0      200 2023-07-03 18:09:06.197595 aiida_wannier90-2.1.0/src/aiida_wannier90/calculations/__init__.py
+-rw-r--r--   0        0        0    19794 2023-07-03 18:09:06.293594 aiida_wannier90-2.1.0/src/aiida_wannier90/calculations/postw90.py
+-rw-r--r--   0        0        0    23668 2023-07-03 18:09:06.297594 aiida_wannier90-2.1.0/src/aiida_wannier90/calculations/wannier90.py
+-rw-r--r--   0        0        0      802 2023-07-03 18:09:06.389593 aiida_wannier90-2.1.0/src/aiida_wannier90/io/__init__.py
+-rw-r--r--   0        0        0     1814 2023-07-03 18:09:06.393593 aiida_wannier90-2.1.0/src/aiida_wannier90/io/_group_list.py
+-rw-r--r--   0        0        0    14969 2023-07-03 18:09:06.393593 aiida_wannier90-2.1.0/src/aiida_wannier90/io/_write_win.py
+-rw-r--r--   0        0        0    13286 2023-07-03 18:09:06.401593 aiida_wannier90-2.1.0/src/aiida_wannier90/orbitals.py
+-rw-r--r--   0        0        0      162 2023-07-03 18:09:06.401593 aiida_wannier90-2.1.0/src/aiida_wannier90/parsers/__init__.py
+-rw-r--r--   0        0        0    20688 2023-07-03 18:09:06.421592 aiida_wannier90-2.1.0/src/aiida_wannier90/parsers/postw90.py
+-rw-r--r--   0        0        0    23479 2023-07-03 18:09:06.433592 aiida_wannier90-2.1.0/src/aiida_wannier90/parsers/wannier90.py
+-rw-r--r--   0        0        0     3092 2023-07-03 18:09:06.445592 aiida_wannier90-2.1.0/src/aiida_wannier90/utils.py
+-rw-r--r--   0        0        0      648 2023-07-03 18:09:06.465592 aiida_wannier90-2.1.0/src/aiida_wannier90/workflows/__init__.py
+-rw-r--r--   0        0        0    11532 2023-07-03 18:09:06.465592 aiida_wannier90-2.1.0/src/aiida_wannier90/workflows/minimal.py
+-rw-r--r--   0        0        0     4108 1970-01-01 00:00:00.000000 aiida_wannier90-2.1.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `aiida-wannier90-2.0.1/LICENSE.txt` & `aiida_wannier90-2.1.0/LICENSE.txt`

 * *Files 11% similar despite different names*

```diff
@@ -18,9 +18,7 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE.
-
-
```

### Comparing `aiida-wannier90-2.0.1/aiida_wannier90/orbitals.py` & `aiida_wannier90-2.1.0/src/aiida_wannier90/orbitals.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,181 +1,159 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
 ################################################################################
 # Copyright (c), AiiDA team and individual contributors.                       #
 #  All rights reserved.                                                        #
 # This file is part of the AiiDA-wannier90 code.                               #
 #                                                                              #
 # The code is hosted on GitHub at https://github.com/aiidateam/aiida-wannier90 #
 # For further information on the license, see the LICENSE.txt file             #
 ################################################################################
-"""
-Creating OrbitalData instances
-==============================
-"""
-from __future__ import absolute_import
-import six
-from six.moves import range
+"""Create OrbitalData instances."""
 
-__all__ = ('generate_projections', )
+__all__ = ("generate_projections",)
 
 
-def _generate_wannier_orbitals( # pylint: disable=too-many-arguments,too-many-locals,too-many-statements # noqa:  disable=MC0001
+def _generate_wannier_orbitals(  # pylint: disable=too-many-arguments,too-many-statements # noqa:  disable=MC0001
     position_cart=None,
     structure=None,
     kind_name=None,
     radial=1,
     ang_mtm_name=None,
     ang_mtm_l_list=None,
     ang_mtm_mr_list=None,
     spin=None,
     zona=None,
     zaxis=None,
     xaxis=None,
-    spin_axis=None
+    spin_axis=None,
 ):
-    """
-    Use this method to emulate the input style of Wannier90,
-    when setting the orbitals (see chapter 3 in the user_guide). Position
-    can be provided either in Cartesian coordiantes using ``position_cart``
+    """Emulate the input style of Wannier90, when setting the orbitals.
+
+    See chapter 3 in the user_guide.
+    Position can be provided either in Cartesian coordiantes using ``position_cart``
     or can be assigned based on an input structure and ``kind_name``.
 
     :param position_cart: position in Cartesian coordinates or list of
                           positions in Cartesian coodriantes
     :param structure: input structure for use with kind_names
     :param kind_name: kind_name, for use with the structure
     :param radial: number of radial nodes
     :param ang_mtm_name: orbital name or list of orbital names, cannot
                          be used in conjunction with ang_mtm_l_list or
                          ang_mtm_mr_list
-    :param ang_mtm_l_list: angular momentum (either an integer or a list), if 
+    :param ang_mtm_l_list: angular momentum (either an integer or a list), if
                  ang_mtm_mr_list is not specified will return all orbitals associated with it
     :param ang_mtm_mr_list: magnetic angular momentum number must be specified
                        along with ang_mtm_l_list. Note that if this is specified,
                        ang_mtm_l_list must be an integer and not a list
     :param spin: the spin, spin up can be specified with 1,u or U and
                  spin down can be specified using -1,d,D
     :param zona: as specified in user guide, applied to all orbitals
     :param zaxis: the zaxis, list of three floats
                   as described in wannier user guide
     :param xaxis: the xaxis, list of three floats as described in the
                   wannier user guide
     :param spin_axis: the spin alignment axis, as described in the
                       user guide
     """
-    from aiida.plugins import DataFactory
-    from aiida.plugins import OrbitalFactory
     from aiida.common import InputValidationError
+    from aiida.plugins import DataFactory, OrbitalFactory
 
     def convert_to_list(item):
-        """
-        internal method, checks if the item is already a list or tuple.
-        if not returns a tuple containing only item, otherwise returns
-        tuple(item)
+        """Check if the item is already a list or tuple.
+
+        if not returns a tuple containing only item, otherwise returns ``tuple(item)``.
         """
         if isinstance(item, (list, tuple)):
             return tuple(item)
         return tuple([item])
 
     def combine_dictlists(dict_list1, dict_list2):
-        """
-        Creates a list of every dict in dict_list1 updated with every
-        dict in dict_list2
-        """
+        """Create a list of every dict in dict_list1 updated with every dict in dict_list2."""
         out_list = []
         # excpetion handling for the case of empty dicts
-        dict_list1_empty = not any([bool(x) for x in dict_list1])
-        dict_list2_empty = not any([bool(x) for x in dict_list2])
+        dict_list1_empty = not any(bool(x) for x in dict_list1)
+        dict_list2_empty = not any(bool(x) for x in dict_list2)
         if dict_list1_empty and dict_list2_empty:
-            raise InputValidationError('One dict must not be empty')
+            raise InputValidationError("One dict must not be empty")
         if dict_list1_empty:
             return dict_list2
         if dict_list2_empty:
             return dict_list2
 
         for dict_1 in dict_list1:
             for dict_2 in dict_list2:
                 temp_1 = dict_1.copy()
                 temp_2 = dict_2.copy()
                 temp_1.update(temp_2)
                 out_list.append(temp_1)
         return out_list
 
-    RealhydrogenOrbital = OrbitalFactory('realhydrogen')
+    RealhydrogenOrbital = OrbitalFactory("core.realhydrogen")
 
     #########################################################################
     # Validation of inputs                                                  #
     #########################################################################
     if position_cart is None and kind_name is None:
-        raise InputValidationError('Must supply a kind_name or position')
+        raise InputValidationError("Must supply a kind_name or position")
     if position_cart is not None and kind_name is not None:
-        raise InputValidationError(
-            'Must supply position or kind_name'
-            ' not both'
-        )
+        raise InputValidationError("Must supply position or kind_name not both")
 
-    structure_class = DataFactory('structure')
+    structure_class = DataFactory("core.structure")
     if kind_name is not None:
         if not isinstance(structure, structure_class):
             raise InputValidationError(
-                'Must supply a StructureData as '
-                'structure if using kind_name'
+                "Must supply a StructureData as structure if using kind_name"
             )
-        if not isinstance(kind_name, six.string_types):
-            raise InputValidationError('kind_name must be a string')
+        if not isinstance(kind_name, str):
+            raise InputValidationError("kind_name must be a string")
 
     if ang_mtm_name is None and ang_mtm_l_list is None:
-        raise InputValidationError(
-            "Must supply ang_mtm_name or ang_mtm_l_list"
-        )
+        raise InputValidationError("Must supply ang_mtm_name or ang_mtm_l_list")
     if ang_mtm_name is not None and (
         ang_mtm_l_list is not None or ang_mtm_mr_list is not None
     ):
         raise InputValidationError(
-            "Cannot supply ang_mtm_l_list or ang_mtm_mr_list"
-            " but not both"
+            "Cannot supply ang_mtm_l_list or ang_mtm_mr_list but not both"
         )
     if ang_mtm_l_list is None and ang_mtm_mr_list is not None:
         raise InputValidationError(
-            "Cannot supply ang_mtm_mr_list without "
-            "ang_mtm_l_list"
+            "Cannot supply ang_mtm_mr_list without ang_mtm_l_list"
         )
 
     ####################################################################
-    #Setting up initial basic parameters
+    # Setting up initial basic parameters
     ####################################################################
     projection_dict = {}
     if radial:
-        projection_dict['radial_nodes'] = radial - 1
+        projection_dict["radial_nodes"] = radial - 1
     if xaxis:
-        projection_dict['x_orientation'] = xaxis
+        projection_dict["x_orientation"] = xaxis
     if zaxis:
-        projection_dict['z_orientation'] = zaxis
+        projection_dict["z_orientation"] = zaxis
     if kind_name:
-        projection_dict['kind_name'] = kind_name
+        projection_dict["kind_name"] = kind_name
     if spin_axis:
-        projection_dict['spin_orientation'] = spin_axis
+        projection_dict["spin_orientation"] = spin_axis
     if zona:
-        projection_dict['diffusivity'] = zona
+        projection_dict["diffusivity"] = zona
 
     projection_dicts = [projection_dict]
 
     #####################################################################
     # Setting up Positions                                              #
     #####################################################################
     # finds all the positions to append the orbitals to (if applicable)
     position_list = []
     if kind_name:
         for site in structure.sites:
             if site.kind_name == kind_name:
                 position_list.append(site.position)
         if not position_list:
             raise InputValidationError(
-                "No valid positions found in structure "
-                "using {}".format(kind_name)
+                f"No valid positions found in structure using {kind_name}"
             )
     # otherwise turns position into position_list
     else:
         position_list = [convert_to_list(position_cart)]
     position_dicts = [{"position": v} for v in position_list]
     projection_dicts = combine_dictlists(projection_dicts, position_dicts)
 
@@ -184,77 +162,76 @@
     #######################################################################
     # if ang_mtm_l_list, ang_mtm_mr_list provided, setup dicts
     if ang_mtm_l_list is not None:
         ang_mtm_l_list = convert_to_list(ang_mtm_l_list)
         ang_mtm_dicts = []
         for ang_mtm_l in ang_mtm_l_list:
             if ang_mtm_l >= 0:
-                ang_mtm_dicts += [{
-                    'angular_momentum': ang_mtm_l,
-                    'magnetic_number': i
-                } for i in range(2 * ang_mtm_l + 1)]
+                ang_mtm_dicts += [
+                    {"angular_momentum": ang_mtm_l, "magnetic_number": i}
+                    for i in range(2 * ang_mtm_l + 1)
+                ]
             else:
-                ang_mtm_dicts += [{
-                    'angular_momentum': ang_mtm_l,
-                    'magnetic_number': i
-                } for i in range(-ang_mtm_l + 1)]
+                ang_mtm_dicts += [
+                    {"angular_momentum": ang_mtm_l, "magnetic_number": i}
+                    for i in range(-ang_mtm_l + 1)
+                ]
         if ang_mtm_mr_list is not None:
             if len(ang_mtm_l_list) > 1:
                 raise InputValidationError(
                     "If you are giving specific"
                     " magnetic numbers please do"
                     " not supply more than one"
                     " angular number."
                 )
             ang_mtm_mr_list = convert_to_list(ang_mtm_mr_list)
             ang_mtm_l_num = ang_mtm_l_list[0]
-            ang_mtm_dicts = [{
-                'angular_momentum': ang_mtm_l_num,
-                'magnetic_number': j - 1
-            } for j in ang_mtm_mr_list]
+            ang_mtm_dicts = [
+                {"angular_momentum": ang_mtm_l_num, "magnetic_number": j - 1}
+                for j in ang_mtm_mr_list
+            ]
     if ang_mtm_name is not None:
         ang_mtm_names = convert_to_list(ang_mtm_name)
         ang_mtm_dicts = []
         for name in ang_mtm_names:
             # get_quantum_numbers_from_name (in AiiDA) might not return
             # a consistent order since it creates the list from a dictionary
             # This might be considered a bug in AiiDA, but since AiiDA is going
             # to drop py2 support soon, this might not be fixed, so we work
             # around the issue here.
             ang_mtm_dicts += sorted(
                 RealhydrogenOrbital.get_quantum_numbers_from_name(name),
-                key=lambda qnums:
-                (qnums['angular_momentum'], qnums['magnetic_number'])
+                key=lambda qnums: (qnums["angular_momentum"], qnums["magnetic_number"]),
             )
     projection_dicts = combine_dictlists(projection_dicts, ang_mtm_dicts)
 
     #####################################################################
     # Setting up the spin                                               #
     #####################################################################
     if spin:
-        spin_dict = {'U': 1, 'u': 1, 1: 1, 'D': -1, 'd': -1, -1: -1}
+        spin_dict = {"U": 1, "u": 1, 1: 1, "D": -1, "d": -1, -1: -1}
         if isinstance(spin, (list, tuple)):
             spin = [spin_dict[x] for x in spin]
         else:
             spin = [spin_dict[spin]]
-        spin_dicts = [{'spin': v} for v in spin]
+        spin_dicts = [{"spin": v} for v in spin]
         projection_dicts = combine_dictlists(projection_dicts, spin_dicts)
 
     # generating and returning a list of all corresponding orbitals
     orbital_out = []
     for projection_dict in projection_dicts:
         realh = RealhydrogenOrbital(**projection_dict)
         orbital_out.append(realh)
     return orbital_out
 
 
 def generate_projections(list_of_projection_dicts, structure):
-    """
-    Use this method to emulate the input style of Wannier90,
-    when setting the orbitals (see chapter 3 in the Wannier90 user guide).
+    """Emulate the input style of Wannier90, when setting the orbitals.
+
+    See chapter 3 in the Wannier90 user guide.
     Position can be provided either in Cartesian coordinates using
     ``position_cart`` or can be assigned based on an input structure and
     ``kind_name``. Pass a list of dictionaries, in which the keys of each
     dictionary correspond to those below. Also note that ``radial``
     and ``ang_mtm_mr_list`` both use 0-based indexing as opposed to 1-based
     indexing, effectively meaning that both should be offset by 1.
     E.g., an orbital with two radial nodes would use ``radial=2``
@@ -272,22 +249,22 @@
         positions in Cartesian coordinates (``position``)
     :param kind_name: kind name in the input
         :py:class:`~aiida.orm.StructureData` node (``kind_name``)
     :param radial: number of radial nodes (``radial_nodes + 1``)
     :param ang_mtm_name: orbital name or list of orbital names, cannot
         be used in conjunction with ``ang_mtm_l_list`` or ``ang_mtm_mr_list``
         (see ``ang_mtm_l_list`` and ``ang_mtm_mr_list``).
-    :param ang_mtm_l_list: angular momentum (either an integer or a list), if 
+    :param ang_mtm_l_list: angular momentum (either an integer or a list), if
         ``ang_mtm_mr_list`` is not specified will return all orbitals
         associated with it (``angular_momentum``).
     :param ang_mtm_mr_list: magnetic angular momentum number must be specified
         along with ``ang_mtm_l_list`` (``magnetic_number + 1``). Note that
         if this is specified, ``ang_mtm_l_list`` must be an
         integer and not a list.
-    :param spin: the spin, spin up can be specified with ``1``, ``'u'`` or 
+    :param spin: the spin, spin up can be specified with ``1``, ``'u'`` or
         ``'U'`` and spin down can be specified using ``-1``, ``'d'``
         or ``'D'`` (``spin``)
     :param zona: as specified in user guide, applied to all orbitals
         (``diffusivity``)
     :param zaxis: the z-axis of the orbital, a list of three floats
         as described in wannier user guide (``z_orientation``)
     :param xaxis: the x-axis of the orbital, a list of three floats as
@@ -297,13 +274,13 @@
     """
     from aiida.plugins import DataFactory
 
     if not isinstance(list_of_projection_dicts, (list, tuple)):
         list_of_projection_dicts = [list_of_projection_dicts]
     orbitals = []
     for this_dict in list_of_projection_dicts:
-        if 'kind_name' in this_dict:
-            this_dict.update({'structure': structure})
+        if "kind_name" in this_dict:
+            this_dict.update({"structure": structure})
         orbitals += _generate_wannier_orbitals(**this_dict)
-    orbitaldata = DataFactory('orbital')()
+    orbitaldata = DataFactory("core.orbital")()
     orbitaldata.set_orbitals(orbitals)
     return orbitaldata
```

### Comparing `aiida-wannier90-2.0.1/aiida_wannier90/io/_write_win.py` & `aiida_wannier90-2.1.0/src/aiida_wannier90/io/_write_win.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,39 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
 ################################################################################
 # Copyright (c), AiiDA team and individual contributors.                       #
 #  All rights reserved.                                                        #
 # This file is part of the AiiDA-wannier90 code.                               #
 #                                                                              #
 # The code is hosted on GitHub at https://github.com/aiidateam/aiida-wannier90 #
 # For further information on the license, see the LICENSE.txt file             #
 ################################################################################
-
-from __future__ import unicode_literals
-
-from __future__ import absolute_import
+"""Write input to a ``.win`` file."""
 import copy
+import typing as ty
 
-from aiida_wannier90.utils import conv_to_fortran_withlists
+from aiida import orm
 from aiida.common import InputValidationError
 
+from ..utils import conv_to_fortran_withlists
 from ._group_list import list_to_grouped_string
-import six
 
-__all__ = ('write_win', )
+__all__ = ("write_win",)
 
 
-def write_win( # pylint: disable=too-many-arguments
+def write_win(  # pylint: disable=too-many-arguments
     filename,
     parameters,
     kpoints=None,
     structure=None,
     kpoint_path=None,
+    bands_kpoints=None,
     projections=None,
     random_projections=False,
 ):
-    """
-    Write input to a ``.win`` file.
+    """Write input to a ``.win`` file.
 
     :param filename: Path of the file where the input is written.
     :type filename: str
 
     :param parameters: Additional input parameters, as specified in the Wannier90 user guide.
     :type parameters: dict, aiida.orm.nodes.data.dict.Dict
 
@@ -46,306 +42,342 @@
 
     :param kpoints: Mesh of k-points used for the Wannierization procedure.
     :type kpoints: aiida.orm.nodes.data.array.kpoints.KpointsData
 
     :param kpoint_path: List of k-points used for band interpolation.
     :type kpoint_path: aiida.orm.nodes.data.dict.Dict
 
-    :param projections: Orbitals used for the projections. Can be specified either as AiiDA  class :py:class:`OrbitalData <aiida.orm.OrbitalData>`,
-     or as a list of strings specifying the projections in Wannier90's format.
+    :param bands_kpoints: An explicit list of k-points used for band interpolation.
+    :type bands_kpoints: aiida.orm.KpointsData
+
+    :param projections: Orbitals used for the projections. Can be specified either as AiiDA class
+    :py:class:`OrbitalData <aiida.orm.OrbitalData>`,
+    or as a list of strings specifying the projections in Wannier90's format.
     :type projections: aiida.orm.nodes.data.orbital.OrbitalData, aiida.orm.nodes.data.list.List[str]
 
-    :param random_projections: If  class :py:class:`OrbitalData <aiida.orm.OrbitalData>` is used for projections, enables random projections completion
+    :param random_projections: If  class :py:class:`OrbitalData <aiida.orm.OrbitalData>` is used for projections,
+    enables random projections completion
     :type random_projections: aiida.orm.nodes.data.bool.Bool
     """
-    with open(filename, 'w') as file:  #pylint: disable= redefined-builtin
+    with open(filename, "w", encoding="utf-8") as file:
         file.write(
             _create_win_string(
                 parameters=parameters,
                 structure=structure,
                 kpoints=kpoints,
                 kpoint_path=kpoint_path,
+                bands_kpoints=bands_kpoints,
                 projections=projections,
                 random_projections=random_projections,
             )
         )
 
 
-def _create_win_string( # pylint: disable=too-many-arguments
+def _create_win_string(  # pylint: disable=too-many-arguments
     parameters,
     kpoints,
     structure=None,
     kpoint_path=None,
+    bands_kpoints=None,
     projections=None,
     random_projections=False,
 ):
-    from aiida.plugins import DataFactory
+    """Generate a string with the content of a .win file."""
     from aiida.orm import List
+    from aiida.plugins import DataFactory
 
     # prepare the main input text
     input_file_lines = []
-    if isinstance(parameters, DataFactory('dict')):
+    if isinstance(parameters, DataFactory("core.dict")):
         parameters = parameters.get_dict()
     try:
-        parameters.setdefault('mp_grid', kpoints.get_kpoints_mesh()[0])
+        parameters.setdefault("mp_grid", kpoints.get_kpoints_mesh()[0])
     except AttributeError:
         pass
     input_file_lines += _format_parameters(parameters)
 
     block_inputs = {}
     if projections is None:
         # If no projections are specified, random projections is used (Dangerous!)
         if random_projections:
-            block_inputs['projections'] = ['random']
+            block_inputs["projections"] = ["random"]
         else:
-            block_inputs['projections'] = []
+            block_inputs["projections"] = []
     elif isinstance(projections, (tuple, list)):
         if random_projections:
             raise InputValidationError(
-                'random_projections cannot be True with (tuple,list) projections.'
+                "random_projections cannot be True with (tuple,list) projections."
                 'Instead, use "random" string as first element of the list.'
             )
-        block_inputs['projections'] = projections
+        block_inputs["projections"] = projections
     elif isinstance(projections, List):
         if random_projections:
             raise InputValidationError(
-                'random_projections cannot be True if with List-type projections.'
+                "random_projections cannot be True if with List-type projections."
                 'Instead, use "random" string as first element of the List.'
             )
-        block_inputs['projections'] = projections.get_list()
+        block_inputs["projections"] = projections.get_list()
     else:
-        block_inputs['projections'] = _format_all_projections(
+        block_inputs["projections"] = _format_all_projections(
             projections, random_projections=True
         )
 
     if structure is not None:
-        block_inputs['unit_cell_cart'] = _format_unit_cell(structure)
-        block_inputs['atoms_cart'] = _format_atoms_cart(structure)
+        block_inputs["unit_cell_cart"] = _format_unit_cell(structure)
+        block_inputs["atoms_cart"] = _format_atoms_cart(structure)
     if kpoints is not None:
-        block_inputs['kpoints'] = _format_kpoints(kpoints)
+        block_inputs["kpoints"] = _format_kpoints(kpoints)
     if kpoint_path is not None:
-        block_inputs['kpoint_path'] = _format_kpoint_path(kpoint_path)
+        block_inputs["kpoint_path"] = _format_kpoint_path(kpoint_path)
+    elif bands_kpoints is not None:
+        kpath, labels = _format_explicit_kpoint_path(bands_kpoints)
+        block_inputs["explicit_kpath"] = kpath
+        block_inputs["explicit_kpath_labels"] = labels
     input_file_lines += _format_block_inputs(block_inputs)
 
-    return '\n'.join(input_file_lines) + '\n'
+    return "\n".join(input_file_lines) + "\n"
 
 
 def _format_parameters(parameters_dict):
-    """
-    Join key / value pairs of the parameters dictionary into formatted strings, returning a list of lines for the .win file.
+    """Join key / value pairs of the parameters dictionary into formatted strings.
+
+    Returning a list of lines for the .win file.
     """
     lines = []
-    for key, value in sorted(
-        _format_parameter_values(parameters_dict).items()
-    ):
-        lines.append(key + ' = ' + value)
+    for key, value in sorted(_format_parameter_values(parameters_dict).items()):
+        lines.append(key + " = " + value)
     return lines
 
 
 def _format_parameter_values(parameters_dict):
-    """
-    Turn the values of the parameters dictionary into the appropriate string.
-    """
+    """Turn the values of the parameters dictionary into the appropriate string."""
     result_dict = {}
     for key, value in parameters_dict.items():
         key = key.lower()
-        if key == 'exclude_bands':
+        if key == "exclude_bands":
             if len(set(value)) < len(value):
                 raise InputValidationError(
                     "The 'exclude_bands' input contains duplicate entries."
                 )
+            if any(val <= 0 for val in value):
+                raise InputValidationError(
+                    "The 'exclude_bands' values must be positive."
+                )
             result_dict[key] = list_to_grouped_string(value)
         else:
-            result_dict[key] = conv_to_fortran_withlists(
-                value, quote_strings=False
-            )
+            result_dict[key] = conv_to_fortran_withlists(value, quote_strings=False)
     return result_dict
 
 
 def _format_all_projections(projections, random_projections=False):
-    """
-    Return a list of strings, they are the lines to insert into
-    Wannier90 projections block.
+    """Return a list of strings, they are the lines to insert into Wannier90 projections block.
 
     :param projections: OrbitalData object with projections info
     :param random_projections: if True, add the 'random' keyword on top.
         It asks the code to fill missing projections with random orbitals (see Wannier90 docs)
     """
     projection_list = projections.get_orbitals()
     # TODO: Check if spinor_projections actually needs to be used.
     # spin_use = any([bool(projection.get_orbital_dict()['spin'])
     #                 for projection in projection_list])
     # projector_type = "spinor_projections" if spin_use else "projections"
     projection_lines = [
         _format_single_projection(projection) for projection in projection_list
     ]
     if random_projections:
-        projection_lines = ['random'] + projection_lines
+        projection_lines = ["random"] + projection_lines
     return projection_lines
 
 
-def _format_single_projection(orbital):  #pylint: disable=too-many-locals
-    """
-    Creates an appropriate wannier line from input orbitaldata,
-    will raise an exception if the orbital does not contain enough
-    information, or the information is badly formated
+def _format_single_projection(orbital):  # pylint: disable=too-many-locals
+    """Create an appropriate wannier line from input orbitaldata.
+
+    Will raise an exception if the orbital does not contain enough information,
+    or the information is badly formatted.
     """
     from aiida.plugins import OrbitalFactory
-    RealhydrogenOrbital = OrbitalFactory("realhydrogen")
+
+    RealhydrogenOrbital = OrbitalFactory("core.realhydrogen")
 
     if not isinstance(orbital, RealhydrogenOrbital):
         raise InputValidationError(
             "Only realhydrogen orbitals are currently supported for Wannier90 input."
         )
     orb_dict = copy.deepcopy(orbital.get_orbital_dict())
 
     def _get_attribute(name, required=True):
         res = orb_dict.get(name, None)
         if res is None and required:
-            raise InputValidationError(
-                "Orbital is missing attribute '{}'.".format(name)
-            )
+            raise InputValidationError(f"Orbital is missing attribute '{name}'.")
         return res
 
     def _format_projection_values_float(name, value):
-        """
-        Return a string for a given key-value pair of the projections block, e.g.
+        """Return a string for a given key-value pair of the projections block.
+
+        E.g.
         ``'c=0.132443,1.324823823,0.547423243'``, where we know that values are floats
         that will be formatted with a specific formatting option.
         """
         if value is None:
-            return ''
+            return ""
         if not isinstance(value, (tuple, list)):
             value = [value]
-        return '{}={}'.format(
-            name, ','.join("{:.10f}".format(x) for x in value)
-        )
+        return f'{name}={",".join(f"{x:.10f}" for x in value)}'
 
     def _format_projection_values_generic(name, value):
-        """
-        Return a string for a given key-value pair of the projections block, e.g.
+        """Return a string for a given key-value pair of the projections block.
+
+        E.g.
         ``'l=1'``, where formatting of the values is done without specifying
         a custom format - this is ok for e.g. integers, while for floats it's
         better to use :func:`_format_projection_values_float` function that
         properly formats floats, avoiding differences between python versions.
         """
         if value is None:
-            return ''
+            return ""
         if not isinstance(value, (tuple, list)):
             value = [value]
-        return '{}={}'.format(name, ','.join("{}".format(x) for x in value))
+        return f'{name}={",".join(f"{x}" for x in value)}'
 
     # required arguments
     position = _get_attribute("position")
     angular_momentum = _get_attribute("angular_momentum")
     magnetic_number = _get_attribute("magnetic_number")
     wann_string = (
-        _format_projection_values_float('c', position) + ':' +
-        _format_projection_values_generic('l', angular_momentum) + ',' +
-        _format_projection_values_generic('mr', magnetic_number + 1)
+        _format_projection_values_float("c", position)
+        + ":"
+        + _format_projection_values_generic("l", angular_momentum)
+        + ","
+        + _format_projection_values_generic("mr", magnetic_number + 1)
     )
 
     # optional, colon-separated arguments
     zaxis = _get_attribute("z_orientation", required=False)
     xaxis = _get_attribute("x_orientation", required=False)
     radial = _get_attribute("radial_nodes", required=False)
     zona = _get_attribute("diffusivity", required=False)
     if any(arg is not None for arg in [zaxis, xaxis, radial, zona]):
-        zaxis_string = _format_projection_values_float('z', zaxis)
-        xaxis_string = _format_projection_values_float('x', xaxis)
-        radial_string = _format_projection_values_generic('r', radial + 1)
-        zona_string = _format_projection_values_float('zona', zona)
-        wann_string += ':{}:{}:{}:{}'.format(
-            zaxis_string, xaxis_string, radial_string, zona_string
-        )
+        zaxis_string = _format_projection_values_float("z", zaxis)
+        xaxis_string = _format_projection_values_float("x", xaxis)
+        radial_string = _format_projection_values_generic("r", radial + 1)
+        zona_string = _format_projection_values_float("zona", zona)
+        wann_string += f":{zaxis_string}:{xaxis_string}:{radial_string}:{zona_string}"
 
     # spin, optional
     # Careful with spin, it is insufficient to set the spin the projection
     # line alone. You must, in addition, apply the appropriate settings:
     # either set spinors=.true. or use spinor_projections, see user guide
     spin = _get_attribute("spin", required=False)
     if spin is not None and spin != 0:
         spin_dict = {-1: "d", 1: "u"}
-        wann_string += "({})".format(spin_dict[spin])
+        wann_string += f"({spin_dict[spin]})"
     spin_orient = _get_attribute("spin_orientation", required=False)
     if spin_orient is not None:
-        wann_string += "[" + ",".join([
-            "{:18.10f}".format(x) for x in spin_orient
-        ]) + "]"
+        wann_string += "[" + ",".join([f"{x:18.10f}" for x in spin_orient]) + "]"
 
     return wann_string
 
 
 def _format_unit_cell(structure):
-    return ['ang'] + [
-        "{0:18.10f} {1:18.10f} {2:18.10f}".format(*vector)
+    return ["ang"] + [
+        f"{vector[0]:18.10f} {vector[1]:18.10f} {vector[2]:18.10f}"
         for vector in structure.cell
     ]
 
 
 def _format_atoms_cart(structure):
-    """
-    Generates site locations and cell dimensions
-    in a manner that can be used by the wannier90 input script
-    """
+    """Generate site locations and cell dimensions that can be used by the wannier90 input script."""
+
     def list2str(list_item):
-        '''
-        Converts an input list item into a str
-        '''
+        """Convert an input list item into a str."""
         list_item = copy.deepcopy(list_item)
-        if isinstance(list_item, (str, six.text_type)):
+        if isinstance(list_item, str):
             return list_item
-        return ' ' + ' '.join(["{:18.10f}".format(_) for _ in list_item]) + ' '
+        return " " + " ".join([f"{_:18.10f}" for _ in list_item]) + " "
 
-    return ['ang'] + [
-        '{}  {}'.format(site.kind_name, list2str(site.position))
-        for site in structure.sites
+    return ["ang"] + [
+        f"{site.kind_name}  {list2str(site.position)}" for site in structure.sites
     ]
 
 
 def _format_kpoints(kpoints):
     # KpointsData was set with set_kpoints_mesh
     try:
         all_kpoints = kpoints.get_kpoints_mesh(print_list=True)
     # KpointsData was set with set_kpoints
     except AttributeError:
         all_kpoints = kpoints.get_kpoints()
-    return ["{:18.10f} {:18.10f} {:18.10f}".format(*k) for k in all_kpoints]
+    return [f"{k[0]:18.10f} {k[1]:18.10f} {k[2]:18.10f}" for k in all_kpoints]
 
 
 def _format_kpoint_path(kpoint_path):
-    """
-    Prepare the lines for the Wannier90 input file related to
-    the kpoint_path.
+    """Prepare the lines for the Wannier90 input file related to the kpoint_path.
 
     :param kpoint_path: a ParameterData containing two entries:
         a 'path' list with the labels of the endpoints of each
         path segment, and a dictionary called "point_coords" that gives the
         three (fractional) coordinates for each label.
     :return: a list of strings to be added to the input file, within the
         kpoint_info block
     """
     kinfo = kpoint_path.get_dict()
-    path = kinfo.pop('path')
-    point_coords = kinfo.pop('point_coords')
+    path = kinfo.pop("path")
+    point_coords = kinfo.pop("point_coords")
 
     # In Wannier90 (from the user guide): Values are in
     # fractional coordinates with respect to the primitive
     # reciprocal lattice vectors.
     res = []
-    for (point1, point2) in path:
+    for point1, point2 in path:
         coord1 = point_coords[point1]
         coord2 = point_coords[point2]
-        path_line = '{} {} {} {} '.format(point1, *coord1)
-        path_line += ' {} {} {} {}'.format(point2, *coord2)
+        path_line = f"{point1} {coord1[0]} {coord1[1]} {coord1[2]} "
+        path_line += f" {point2} {coord2[0]} {coord2[1]} {coord2[2]}"
         res.append(path_line)
     return res
 
 
+def _format_explicit_kpoint_path(bands_kpoints: orm.KpointsData) -> ty.Tuple:
+    """Prepare the lines for the Wannier90 input file related to the `explicit_kpath` and `explicit_kpath_labels`.
+
+    :param bands_kpoints: a KpointsData which must contain labels.
+    :return: a tuple of list of strings to be added to the input file, for the `explicit_kpath`
+    and `explicit_kpath_labels` blocks.
+    """
+    if "mesh" in bands_kpoints.base.attributes.all:
+        raise ValueError(
+            "Input should be a list of kpoints along the kpath, but "
+            f"KpointsData<{bands_kpoints.pk}> contains a mesh"
+        )
+
+    if bands_kpoints.labels is None:
+        raise ValueError(
+            f"Input KpointsData<{bands_kpoints.pk}> should contain `labels`"
+        )
+
+    kpoints = bands_kpoints.get_kpoints()
+    labels = bands_kpoints.labels
+
+    # In Wannier90 (from the user guide): Values are in
+    # fractional coordinates with respect to the primitive
+    # reciprocal lattice vectors.
+    explicit_kpath = []
+    for kpt in kpoints:
+        explicit_kpath.append(f"{kpt[0]:18.10f} {kpt[1]:18.10f} {kpt[2]:18.10f}")
+
+    explicit_kpath_labels = []
+    for idx, lab in labels:
+        kpt = kpoints[idx]
+        path_line = f"{lab} {kpt[0]:18.10f} {kpt[1]:18.10f} {kpt[2]:18.10f}"
+        explicit_kpath_labels.append(path_line)
+
+    return explicit_kpath, explicit_kpath_labels
+
+
 def _format_block_inputs(block_inputs):
     res = []
     for name, lines in sorted(block_inputs.items()):
-        res.append('')
-        res.append('begin {}'.format(name))
+        res.append("")
+        res.append(f"begin {name}")
         res.extend(lines)
-        res.append('end {}'.format(name))
+        res.append(f"end {name}")
     return res
```

### Comparing `aiida-wannier90-2.0.1/aiida_wannier90/io/__init__.py` & `aiida_wannier90-2.1.0/src/aiida_wannier90/io/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,16 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
 ################################################################################
 # Copyright (c), AiiDA team and individual contributors.                       #
 #  All rights reserved.                                                        #
 # This file is part of the AiiDA-wannier90 code.                               #
 #                                                                              #
 # The code is hosted on GitHub at https://github.com/aiidateam/aiida-wannier90 #
 # For further information on the license, see the LICENSE.txt file             #
 ################################################################################
-"""
-Writing input files
-===================
+"""Writing input files.
 
 This submodule contains helper functions to create input files.
 """
 
 from ._write_win import write_win
 
-__all__ = ('write_win', )
+__all__ = ("write_win",)
```

### Comparing `aiida-wannier90-2.0.1/aiida_wannier90/io/_group_list.py` & `aiida_wannier90-2.1.0/src/aiida_wannier90/io/_group_list.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,44 +1,47 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
 ################################################################################
 # Copyright (c), AiiDA team and individual contributors.                       #
 #  All rights reserved.                                                        #
 # This file is part of the AiiDA-wannier90 code.                               #
 #                                                                              #
 # The code is hosted on GitHub at https://github.com/aiidateam/aiida-wannier90 #
 # For further information on the license, see the LICENSE.txt file             #
 ################################################################################
+"""Functions for converting list of integers."""
 
-from __future__ import absolute_import
-from six.moves import zip
-
-__all__ = ('group_list', 'groups_to_string', 'list_to_grouped_string')
+__all__ = ("group_list", "groups_to_string", "list_to_grouped_string")
 
 
 def group_list(values):
+    """Group a list of values into a list of groups of consecutive values.
+
+    For W90 input parameters, e.g. exclude_bands.
+    """
     values = sorted(values)
     groups = []
     if not values:
         return groups
+    if len(values) == 1:
+        return [values]
     current_start = values[0]
-    for v1, v2 in zip(values, values[1:]):
+    for val1, val2 in zip(values, values[1:]):
         # contiguous range
-        if v2 - 1 <= v1:
+        if val2 - 1 <= val1:
             continue
         # break in the range
-        else:
-            groups.append(sorted(set([current_start, v1])))
-            current_start = v2
+        groups.append(sorted({current_start, val1}))
+        current_start = val2
         # final group
-    groups.append(sorted(set([current_start, v2])))  # pylint: disable=undefined-loop-variable
+    groups.append(
+        sorted({current_start, val2})  # pylint: disable=undefined-loop-variable
+    )
     return groups
 
 
 def groups_to_string(value_groups):
-    return ','.join(
-        '-'.join([str(g) for g in group]) for group in value_groups
-    )
+    """Convert a list of groups of values to a string."""
+    return ",".join("-".join([str(g) for g in group]) for group in value_groups)
 
 
 def list_to_grouped_string(values):
+    """Convert a list of values to a string, grouping consecutive values."""
     return groups_to_string(group_list(values))
```

### Comparing `aiida-wannier90-2.0.1/aiida_wannier90/workflows/__init__.py` & `aiida_wannier90-2.1.0/src/aiida_wannier90/workflows/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 ################################################################################
 # Copyright (c), AiiDA team and individual contributors.                       #
 #  All rights reserved.                                                        #
 # This file is part of the AiiDA-wannier90 code.                               #
 #                                                                              #
 # The code is hosted on GitHub at https://github.com/aiidateam/aiida-wannier90 #
 # For further information on the license, see the LICENSE.txt file             #
```

### Comparing `aiida-wannier90-2.0.1/aiida_wannier90/workflows/minimal.py` & `aiida_wannier90-2.1.0/src/aiida_wannier90/workflows/minimal.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,349 +1,305 @@
-# -*- coding: utf-8 -*-
 ################################################################################
 # Copyright (c), AiiDA team and individual contributors.                       #
 #  All rights reserved.                                                        #
 # This file is part of the AiiDA-wannier90 code.                               #
 #                                                                              #
 # The code is hosted on GitHub at https://github.com/aiidateam/aiida-wannier90 #
 # For further information on the license, see the LICENSE.txt file             #
 ################################################################################
-from __future__ import absolute_import, print_function, division
+"""A minimal WorkChain to run Wannier90."""
 from aiida import orm
-from aiida.plugins import CalculationFactory
-from aiida.engine import WorkChain, ToContext, calcfunction
-from aiida.orm.nodes.data.upf import get_pseudos_from_structure
+from aiida.engine import ToContext, WorkChain, calcfunction
 from aiida.orm import Dict
+from aiida.orm.nodes.data.upf import get_pseudos_from_structure
+from aiida.plugins import CalculationFactory
 
 
 class MinimalW90WorkChain(WorkChain):
     """Workchain to run a full stack of Quantum ESPRESSO + Wannier90 for GaAs.
 
     Note that this is mostly to be used as an example, as there is no
     error checking and runs directly Quantum ESPRESSO calculations rather
     than the base workflows.
     """
+
     @classmethod
     def define(cls, spec):
         """Define the process specification."""
-        super(MinimalW90WorkChain, cls).define(spec)
+        super().define(spec)
         spec.input(
-            'pw_code',
+            "pw_code",
             valid_type=orm.Code,
-            help='The `pw.x` code to use for the `PwCalculation`s.'
+            help="The `pw.x` code to use for the `PwCalculation`s.",
         )
         spec.input(
-            'pw2wannier90_code',
+            "pw2wannier90_code",
             valid_type=orm.Code,
-            help=
-            'The `pw2wannier90.x` code to use for the `Pw2Wannier90Calculation`s.'
+            help="The `pw2wannier90.x` code to use for the `Pw2Wannier90Calculation`s.",
         )
         spec.input(
-            'wannier_code',
+            "wannier_code",
             valid_type=orm.Code,
-            help='The `wannier90.x` code to use for the `Wannier90Calculation`s.'
+            help="The `wannier90.x` code to use for the `Wannier90Calculation`s.",
         )
         spec.input(
-            'structure',
-            valid_type=orm.StructureData,
-            help='The input structure.'
+            "structure", valid_type=orm.StructureData, help="The input structure."
         )
         spec.input(
-            'pseudo_family',
+            "pseudo_family",
             valid_type=orm.Str,
-            help='The name of a pseudopotential family to use.'
+            help="The name of a pseudopotential family to use.",
         )
         spec.input(
-            'num_machines',
+            "num_machines",
             valid_type=orm.Int,
-            help='The number of machines (nodes) to use',
+            help="The number of machines (nodes) to use",
             required=False,
-            default=lambda: orm.Int(1)
+            default=lambda: orm.Int(1),
         )
         spec.input(
-            'max_wallclock_seconds',
+            "max_wallclock_seconds",
             valid_type=orm.Int,
-            help='Maximum wallclock time in seconds',
+            help="Maximum wallclock time in seconds",
             required=False,
-            default=lambda: orm.Int(30 * 60)
+            default=lambda: orm.Int(30 * 60),
         )
         spec.input(
-            'kpoints_scf',
+            "kpoints_scf",
             valid_type=orm.KpointsData,
-            help='The kpoints for the SCF run.'
+            help="The kpoints for the SCF run.",
         )
         spec.input(
-            'kpoints_nscf',
+            "kpoints_nscf",
             valid_type=orm.KpointsData,
-            help='The kpoints for the NSCF run and Wannierisation.'
+            help="The kpoints for the NSCF run and Wannierisation.",
         )
         spec.input(
-            'kpoint_path',
+            "kpoint_path",
             valid_type=orm.Dict,
-            help='The kpoints path for the NSCF run and Wannierisation.'
+            help="The kpoints path for the NSCF run and Wannierisation.",
         )
         spec.input(
-            'projections',
+            "projections",
             valid_type=orm.OrbitalData,
-            help='The projections for the Wannierisation.'
+            help="The projections for the Wannierisation.",
         )
 
         spec.outline(
             cls.run_pw_scf,
             cls.run_pw_nscf,
             cls.run_w90_pp,
             cls.run_pw2wan,
             cls.run_w90,
             cls.results,
         )
-        spec.output('scf_output', valid_type=orm.Dict)
-        spec.output('nscf_output', valid_type=orm.Dict)
-        spec.output('nnkp_file', valid_type=orm.SinglefileData)
-        spec.output('p2wannier_output', valid_type=orm.Dict)
-        spec.output('matrices_folder', valid_type=orm.FolderData)
-        spec.output('pw2wan_remote_folder', valid_type=orm.RemoteData)
-        spec.output('wannier_bands', valid_type=orm.BandsData)
+        spec.output("scf_output", valid_type=orm.Dict)
+        spec.output("nscf_output", valid_type=orm.Dict)
+        spec.output("nnkp_file", valid_type=orm.SinglefileData)
+        spec.output("p2wannier_output", valid_type=orm.Dict)
+        spec.output("matrices_folder", valid_type=orm.FolderData)
+        spec.output("pw2wan_remote_folder", valid_type=orm.RemoteData)
+        spec.output("wannier_bands", valid_type=orm.BandsData)
 
     def run_pw_scf(self):
         """Run the SCF with pw.x."""
 
         # A fixed value, for testing
-        ecutwfc = 30.
+        ecutwfc = 30.0
 
         self.ctx.scf_parameters = {
-            'CONTROL': {
-                'calculation': 'scf',
+            "CONTROL": {
+                "calculation": "scf",
+            },
+            "SYSTEM": {
+                "ecutwfc": ecutwfc,
+                "ecutrho": ecutwfc * 8.0,
             },
-            'SYSTEM': {
-                'ecutwfc': ecutwfc,
-                'ecutrho': ecutwfc * 8.,
-            }
         }
 
         inputs = {
-            'code':
-            self.inputs.pw_code,
-            'structure':
-            self.inputs.structure,
-            'pseudos':
-            get_pseudos_from_structure(
+            "code": self.inputs.pw_code,
+            "structure": self.inputs.structure,
+            "pseudos": get_pseudos_from_structure(
                 self.inputs.structure, self.inputs.pseudo_family.value
             ),
-            'parameters':
-            orm.Dict(dict=self.ctx.scf_parameters),
-            'kpoints':
-            self.inputs.kpoints_scf,
-            'metadata': {
-                'options': {
+            "parameters": orm.Dict(self.ctx.scf_parameters),
+            "kpoints": self.inputs.kpoints_scf,
+            "metadata": {
+                "options": {
                     # int is used to convert from AiiDA nodes to python ints
-                    'resources': {
-                        'num_machines': int(self.inputs.num_machines)
-                    },
-                    'max_wallclock_seconds':
-                    int(self.inputs.max_wallclock_seconds),
-                    'withmpi': True,
+                    "resources": {"num_machines": int(self.inputs.num_machines)},
+                    "max_wallclock_seconds": int(self.inputs.max_wallclock_seconds),
+                    "withmpi": True,
                 }
-            }
+            },
         }
 
-        running = self.submit(
-            CalculationFactory('quantumespresso.pw'), **inputs
-        )
-        self.report(
-            'launching PwCalculation<{}> (SCF step)'.format(running.pk)
-        )
+        running = self.submit(CalculationFactory("quantumespresso.pw"), **inputs)
+        self.report(f"launching PwCalculation<{running.pk}> (SCF step)")
 
         return ToContext(pw_scf=running)
 
     def run_pw_nscf(self):
-        """Run the NSCF step with pw.x"""
+        """Run the NSCF step with ``pw.x``."""
 
-        self.out('scf_output', self.ctx.pw_scf.outputs.output_parameters)
+        self.out("scf_output", self.ctx.pw_scf.outputs.output_parameters)
 
         try:
             # Check if it's an explicit list of kpoints; this raises AttributeError if it's a mesh
             self.inputs.kpoints_nscf.get_kpoints()
             # If I am here, this an explicit grid, I stop
             raise ValueError(
                 "You should pass an MP grid; we'll take care of converting to an explicit one"
             )
         except AttributeError:
             # Check that the one provided is an unshifted mesh
             assert self.inputs.kpoints_nscf.get_kpoints_mesh()[1] == [
-                0, 0, 0
+                0,
+                0,
+                0,
             ], "You should pass an unshifted mesh"
             self.ctx.kpoints_nscf_explicit = get_explicit_kpoints(
                 self.inputs.kpoints_nscf
             )
 
         nscf_parameters = self.ctx.scf_parameters.copy()
-        nscf_parameters['CONTROL']['calculation'] = 'nscf'
+        nscf_parameters["CONTROL"]["calculation"] = "nscf"
 
         inputs = {
-            'code':
-            self.inputs.pw_code,
-            'structure':
-            self.inputs.structure,
-            'pseudos':
-            get_pseudos_from_structure(
+            "code": self.inputs.pw_code,
+            "structure": self.inputs.structure,
+            "pseudos": get_pseudos_from_structure(
                 self.inputs.structure, self.inputs.pseudo_family.value
             ),
-            'parameters':
-            orm.Dict(dict=nscf_parameters),
-            'kpoints':
-            self.ctx.kpoints_nscf_explicit,
-            'parent_folder':
-            self.ctx.pw_scf.outputs.remote_folder,
-            'metadata': {
-                'options': {
-                    'resources': {
-                        'num_machines': int(self.inputs.num_machines)
-                    },
-                    'max_wallclock_seconds':
-                    int(self.inputs.max_wallclock_seconds),
-                    'withmpi': True,
+            "parameters": orm.Dict(nscf_parameters),
+            "kpoints": self.ctx.kpoints_nscf_explicit,
+            "parent_folder": self.ctx.pw_scf.outputs.remote_folder,
+            "metadata": {
+                "options": {
+                    "resources": {"num_machines": int(self.inputs.num_machines)},
+                    "max_wallclock_seconds": int(self.inputs.max_wallclock_seconds),
+                    "withmpi": True,
                 }
-            }
+            },
         }
 
-        running = self.submit(
-            CalculationFactory('quantumespresso.pw'), **inputs
-        )
-        self.report(
-            'launching PwCalculation<{}> (NSCF step)'.format(running.pk)
-        )
+        running = self.submit(CalculationFactory("quantumespresso.pw"), **inputs)
+        self.report(f"launching PwCalculation<{running.pk}> (NSCF step)")
 
         return ToContext(pw_nscf=running)
 
     def run_w90_pp(self):
         """Run the Wannier90 pre-processing with -pp wannier90.x."""
 
-        self.out('nscf_output', self.ctx.pw_nscf.outputs.output_parameters)
+        self.out("nscf_output", self.ctx.pw_nscf.outputs.output_parameters)
 
         # A fixed value, for testing
         self.ctx.exclude_bands = [1, 2, 3, 4, 5]
 
         self.ctx.w90_pp_parameters = {
-            'mp_grid': self.inputs.kpoints_nscf.get_kpoints_mesh()[0],
-            'write_hr': False,
-            'write_xyz': False,
-            'use_ws_distance': True,
-            'bands_plot': True,
-            'num_iter': 200,
-            'guiding_centres': False,
-            'num_wann': 4,
-            'exclude_bands': self.ctx.exclude_bands,
+            "mp_grid": self.inputs.kpoints_nscf.get_kpoints_mesh()[0],
+            "write_hr": False,
+            "write_xyz": False,
+            "use_ws_distance": True,
+            "bands_plot": True,
+            "num_iter": 200,
+            "guiding_centres": False,
+            "num_wann": 4,
+            "exclude_bands": self.ctx.exclude_bands,
         }
 
         inputs = {
-            'code': self.inputs.wannier_code,
-            'structure': self.inputs.structure,
-            'parameters': orm.Dict(dict=self.ctx.w90_pp_parameters),
-            'kpoints': self.ctx.kpoints_nscf_explicit,
-            'kpoint_path': self.inputs.kpoint_path,
-            'projections': self.inputs.projections,
-            'settings': Dict(dict={'postproc_setup': True}),
-            'metadata': {
-                'options': {
-                    'resources': {
-                        'num_machines': int(self.inputs.num_machines)
-                    },
-                    'max_wallclock_seconds':
-                    int(self.inputs.max_wallclock_seconds),
-                    'withmpi': False,  #serial run
+            "code": self.inputs.wannier_code,
+            "structure": self.inputs.structure,
+            "parameters": orm.Dict(self.ctx.w90_pp_parameters),
+            "kpoints": self.ctx.kpoints_nscf_explicit,
+            "kpoint_path": self.inputs.kpoint_path,
+            "projections": self.inputs.projections,
+            "settings": Dict({"postproc_setup": True}),
+            "metadata": {
+                "options": {
+                    "resources": {"num_machines": int(self.inputs.num_machines)},
+                    "max_wallclock_seconds": int(self.inputs.max_wallclock_seconds),
+                    "withmpi": False,  # serial run
                 }
-            }
+            },
         }
 
-        running = self.submit(
-            CalculationFactory('wannier90.wannier90'), **inputs
-        )
-        self.report('launching Wannier90<{}> (pp step)'.format(running.pk))
+        running = self.submit(CalculationFactory("wannier90.wannier90"), **inputs)
+        self.report(f"launching Wannier90<{running.pk}> (pp step)")
 
         return ToContext(w90_pp=running)
 
     def run_pw2wan(self):
         """Run pw2wannier90.x."""
-        self.out('nnkp_file', self.ctx.w90_pp.outputs.nnkp_file)
+        self.out("nnkp_file", self.ctx.w90_pp.outputs.nnkp_file)
 
         self.ctx.pw2wannier_parameters = {
-            'inputpp': {
-                'write_amn': True,
-                'write_unk': True,
-                'write_mmn': True,
+            "inputpp": {
+                "write_amn": True,
+                "write_unk": True,
+                "write_mmn": True,
             }
         }
-        settings = {'ADDITIONAL_RETRIEVE_LIST': ['*.amn', '*.mmn', '*.eig']}
+        settings = {"ADDITIONAL_RETRIEVE_LIST": ["*.amn", "*.mmn", "*.eig"]}
         inputs = {
-            'code': self.inputs.pw2wannier90_code,
-            'parameters': orm.Dict(dict=self.ctx.pw2wannier_parameters),
-            'parent_folder': self.ctx.pw_nscf.outputs.remote_folder,
-            'nnkp_file': self.ctx.w90_pp.outputs.nnkp_file,
-            'settings': Dict(dict=settings),
-            'metadata': {
-                'options': {
-                    'resources': {
-                        'num_machines': int(self.inputs.num_machines)
-                    },
-                    'max_wallclock_seconds':
-                    int(self.inputs.max_wallclock_seconds),
-                    'withmpi': True,
+            "code": self.inputs.pw2wannier90_code,
+            "parameters": orm.Dict(self.ctx.pw2wannier_parameters),
+            "parent_folder": self.ctx.pw_nscf.outputs.remote_folder,
+            "nnkp_file": self.ctx.w90_pp.outputs.nnkp_file,
+            "settings": Dict(settings),
+            "metadata": {
+                "options": {
+                    "resources": {"num_machines": int(self.inputs.num_machines)},
+                    "max_wallclock_seconds": int(self.inputs.max_wallclock_seconds),
+                    "withmpi": True,
                 }
-            }
+            },
         }
         running = self.submit(
-            CalculationFactory('quantumespresso.pw2wannier90'), **inputs
-        )
-        self.report(
-            'launching pw2wannier90<{}>(pw2wannier90 step)'.format(running.pk)
+            CalculationFactory("quantumespresso.pw2wannier90"), **inputs
         )
+        self.report(f"launching pw2wannier90<{running.pk}>(pw2wannier90 step)")
         return ToContext(pw2wannier=running)
 
     def run_w90(self):
         """Run the Wannier90 main run with wannier90.x."""
-        self.out('matrices_folder', self.ctx.pw2wannier.outputs.retrieved)
-        self.out(
-            'pw2wan_remote_folder', self.ctx.pw2wannier.outputs.remote_folder
-        )
-        self.out(
-            'p2wannier_output', self.ctx.pw2wannier.outputs.output_parameters
-        )
+        self.out("matrices_folder", self.ctx.pw2wannier.outputs.retrieved)
+        self.out("pw2wan_remote_folder", self.ctx.pw2wannier.outputs.remote_folder)
+        self.out("p2wannier_output", self.ctx.pw2wannier.outputs.output_parameters)
 
         inputs = {
-            'code': self.inputs.wannier_code,
-            'structure': self.inputs.structure,
-            'parameters': orm.Dict(dict=self.ctx.w90_pp_parameters),
-            'kpoints': self.ctx.kpoints_nscf_explicit,
-            'kpoint_path': self.inputs.kpoint_path,
-            'remote_input_folder': self.ctx.pw2wannier.outputs.remote_folder,
-            'projections': self.inputs.projections,
-            'metadata': {
-                'options': {
-                    'resources': {
-                        'num_machines': int(self.inputs.num_machines)
-                    },
-                    'max_wallclock_seconds':
-                    int(self.inputs.max_wallclock_seconds),
-                    'withmpi': False,
+            "code": self.inputs.wannier_code,
+            "structure": self.inputs.structure,
+            "parameters": orm.Dict(self.ctx.w90_pp_parameters),
+            "kpoints": self.ctx.kpoints_nscf_explicit,
+            "kpoint_path": self.inputs.kpoint_path,
+            "remote_input_folder": self.ctx.pw2wannier.outputs.remote_folder,
+            "projections": self.inputs.projections,
+            "metadata": {
+                "options": {
+                    "resources": {"num_machines": int(self.inputs.num_machines)},
+                    "max_wallclock_seconds": int(self.inputs.max_wallclock_seconds),
+                    "withmpi": False,
                 }
-            }
+            },
         }
 
-        running = self.submit(
-            CalculationFactory('wannier90.wannier90'), **inputs
-        )
-        self.report('launching Wannier90<{}> (main run)'.format(running.pk))
+        running = self.submit(CalculationFactory("wannier90.wannier90"), **inputs)
+        self.report(f"launching Wannier90<{running.pk}> (main run)")
 
         return ToContext(w90=running)
 
     def results(self):
-        """Output the final results obtained in the previous step"""
-        self.out('wannier_bands', self.ctx.w90.outputs.interpolated_bands)
+        """Output the final results obtained in the previous step."""
+        self.out("wannier_bands", self.ctx.w90.outputs.interpolated_bands)
 
 
 @calcfunction
 def get_explicit_kpoints(kpoints):
-    """Convert from a mesh to an explicit list"""
+    """Convert from a mesh to an explicit list."""
     from aiida.orm import KpointsData
+
     kpt = KpointsData()
     kpt.set_kpoints(kpoints.get_kpoints_mesh(print_list=True))
     return kpt
```

### Comparing `aiida-wannier90-2.0.1/aiida_wannier90/__init__.py` & `aiida_wannier90-2.1.0/src/aiida_wannier90/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,16 @@
-# -*- coding: utf-8 -*-
 ################################################################################
 # Copyright (c), AiiDA team and individual contributors.                       #
 #  All rights reserved.                                                        #
 # This file is part of the AiiDA-wannier90 code.                               #
 #                                                                              #
 # The code is hosted on GitHub at https://github.com/aiidateam/aiida-wannier90 #
 # For further information on the license, see the LICENSE.txt file             #
 ################################################################################
-"""
-AiiDA Wannier90 plugin
-======================
+"""AiiDA Wannier90 plugin.
 
 This is a plugin for running `Wannier90 <http://wannier.org>`_ calculations on the `AiiDA <http://aiida.net>`_ platform.
 
 **Please cite:**
 
 -  **Wannier90 as a community code: new features and applications**
    G. Pizzi, V. Vitale, R. Arita, S. Blügel, F. Freimuth, G. Géranton,
@@ -27,20 +24,14 @@
 -  **AiiDA: automated interactive infrastructure and database for computational science**
    G. Pizzi, A. Cepellotti, R. Sabatini, N. Marzari, and B. Kozinsky,
    *Comp. Mat. Sci.* **111**, 218-230 (2016)
    `[Journal link] <https://doi.org/10.1016/j.commatsci.2015.09.013>`_
    `[arXiv link] <https://arxiv.org/abs/1504.01163>`_
 """
 
-from __future__ import absolute_import
-
-__authors__ = "Dominik Gresch, Antimo Marrazzo, Daniel Marchand, Giovanni Pizzi, Junfeng Qiao, Norma Rivano, and the AiiDA team."
+__authors__ = "The AiiDA team."
 __license__ = "MIT License, see LICENSE.txt file."
-## If upgraded, remember to change it also in setup.json (for pip)
-__version__ = "2.0.1"
+__version__ = "2.1.0"
 
-from . import io
-from . import parsers
-from . import orbitals
-from . import calculations
+from . import calculations, io, orbitals, parsers, utils
 
-__all__ = ('io', 'parsers', 'orbitals', 'calculations')
+__all__ = ("io", "parsers", "orbitals", "calculations", "utils")
```

### Comparing `aiida-wannier90-2.0.1/aiida_wannier90/parsers.py` & `aiida_wannier90-2.1.0/src/aiida_wannier90/parsers/wannier90.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,367 +1,439 @@
-# -*- coding: utf-8 -*-
 ################################################################################
 # Copyright (c), AiiDA team and individual contributors.                       #
 #  All rights reserved.                                                        #
 # This file is part of the AiiDA-wannier90 code.                               #
 #                                                                              #
 # The code is hosted on GitHub at https://github.com/aiidateam/aiida-wannier90 #
 # For further information on the license, see the LICENSE.txt file             #
 ################################################################################
-from __future__ import absolute_import
-import io
+"""Parser for the `Wannier90Calculation`."""
 import os
-import six
-from six.moves import range
-from aiida.parsers import Parser
+
 from aiida.common import exceptions as exc
+from aiida.parsers import Parser
 
 __all__ = (
-    'Wannier90Parser',
-    'band_parser',
-    'raw_wout_parser',
+    "Wannier90Parser",
+    "band_parser",
+    "raw_wout_parser",
 )
 
 
 class Wannier90Parser(Parser):
-    """
-    Wannier90 output parser. Will parse the centres, spreads and, if
-    available, the Imaginary/Real ratio of the Wannier functions.
+    """Wannier90 output parser.
+
+    Will parse the centres, spreads and, if available, the Imaginary/Real ratio of the Wannier functions.
     Will also check if the output converged.
     """
+
     def __init__(self, node):
-        from .calculations import Wannier90Calculation
+        """Construct the parser."""
+        from ..calculations import Wannier90Calculation
 
         # check for valid input
         if not issubclass(node.process_class, Wannier90Calculation):
             raise exc.OutputParsingError(
                 "Input must calc must be a "
-                "Wannier90Calculation, it is instead {}".format(
-                    type(node.process_class)
-                )
+                f"Wannier90Calculation, it is instead {type(node.process_class)}"
             )
-        super(Wannier90Parser, self).__init__(node)
+        super().__init__(node)
 
     @staticmethod
     def _get_seedname_from_input_filename(input_filename):
-        """
-        Return the seedname given the input filename
+        """Return the seedname given the input filename.
 
         Raises a ValueError if the input filename does not end with .win.
         """
-        input_suffix = '.win'
+        input_suffix = ".win"
         if input_filename.endswith(input_suffix):
-            return input_filename[:-len(input_suffix)]
+            return input_filename[: -len(input_suffix)]
 
         raise ValueError(
-            "The input filename '{}' does not end with '{}', so I don't know how to get the seedname"
-            .format(input_filename, input_suffix)
+            f"The input filename '{input_filename}' does not end with '{input_suffix}', "
+            "so I don't know how to get the seedname"
         )
 
-    def parse(self, **kwargs):  # pylint: disable=too-many-locals,inconsistent-return-statements; # noqa: MC0001
-        """
-        Parses the datafolder, stores results.
+    def parse(self, **kwargs):  # pylint: disable=inconsistent-return-statements
+        """Parse the datafolder, stores results.
+
         This parser for this simple code does simply store in the DB a node
-        representing the file of forces in real space
+        representing the file of forces in real space.
         """
+        # pylint: disable=too-many-return-statements,too-many-statements
+        import re
+
         from aiida.orm import Dict, SinglefileData
 
         # None if unset
-        temporary_folder = kwargs.get('retrieved_temporary_folder')
+        temporary_folder = kwargs.get("retrieved_temporary_folder")
 
         seedname = self._get_seedname_from_input_filename(
-            self.node.get_options()['input_filename']
+            self.node.get_options()["input_filename"]
         )
-        output_file_name = "{}.wout".format(seedname)
-        error_file_name = "{}.werr".format(seedname)
-        nnkp_file_name = "{}.nnkp".format(seedname)
+        output_file_name = f"{seedname}.wout"
+        error_file_name = f"{seedname}.werr"
+        nnkp_file_name = f"{seedname}.nnkp"
 
         # select the folder object
         # Check that the retrieved folder is there
         try:
             out_folder = self.retrieved
         except exc.NotExistent:
             return self.exit_codes.ERROR_NO_RETRIEVED_FOLDER
 
-        # Checks for error output files
-        if error_file_name in out_folder.list_object_names():
-            self.logger.error(
-                'Errors were found please check the retrieved '
-                '{} file'.format(error_file_name)
-            )
-            return self.exit_codes.ERROR_WERR_FILE_PRESENT
-
         exiting_in_stdout = False
         try:
-            with out_folder.open(output_file_name) as handle:
+            with out_folder.base.repository.open(output_file_name) as handle:
                 out_file = handle.readlines()
             # Wannier90 doesn't always write the .werr file on error
-            if any('Exiting......' in line for line in out_file):
-                exiting_in_stdout = True
+            for line in out_file:
+                if "Exiting......" in line:
+                    exiting_in_stdout = True
+                if "Unable to satisfy B1" in line:
+                    return self.exit_codes.ERROR_BVECTORS
+                if "kmesh_get_bvector: Not enough bvectors found" in line:
+                    return self.exit_codes.ERROR_BVECTORS
+                if (
+                    "kmesh_get: something wrong, found too many nearest neighbours"
+                    in line
+                ):
+                    return self.exit_codes.ERROR_BVECTORS
+                err_msg = (
+                    "Energy window contains fewer states than number of target WFs, "
+                    "consider reducing dis_proj_min/increasing dis_win_max?"
+                )
+                if err_msg in line:
+                    return self.exit_codes.ERROR_DISENTANGLEMENT_NOT_ENOUGH_STATES
+                if "Error plotting WF cube. Try one of the following:" in line:
+                    return self.exit_codes.ERROR_PLOT_WF_CUBE
+            if len(out_file) == 0:
+                return self.exit_codes.ERROR_OUTPUT_STDOUT_INCOMPLETE
+            if out_file[-1].strip() not in (
+                f"Exiting... {seedname}.nnkp written.",
+                "All done: wannier90 exiting",
+            ):
+                return self.exit_codes.ERROR_OUTPUT_STDOUT_INCOMPLETE
         except OSError:
             self.logger.error("Standard output file could not be found.")
             return self.exit_codes.ERROR_OUTPUT_STDOUT_MISSING
 
+        # Checks for error output files
+        # This is after the check of stdout, since stdout might give more verbose exit code.
+        if error_file_name in out_folder.base.repository.list_object_names():
+            self.logger.error(
+                "Errors were found please check the retrieved "
+                f"{error_file_name} file"
+            )
+            return self.exit_codes.ERROR_WERR_FILE_PRESENT
+
+        # Some times the error files are aiida.node_00001.werr, ...
+        error_file_name = re.compile(seedname + r".+?\.werr")
+        for filename in out_folder.base.repository.list_object_names():
+            if error_file_name.match(filename):
+                self.logger.error(
+                    f"Errors were found please check the retrieved {filename} file"
+                )
+                return self.exit_codes.ERROR_WERR_FILE_PRESENT
+
         if temporary_folder is not None:
             nnkp_temp_path = os.path.join(temporary_folder, nnkp_file_name)
             if os.path.isfile(nnkp_temp_path):
-                with io.open(nnkp_temp_path, 'rb') as handle:
+                with open(nnkp_temp_path, "rb") as handle:
                     node = SinglefileData(file=handle)
-                    self.out('nnkp_file', node)
+                    self.out("nnkp_file", node)
 
         # Tries to parse the bands
         try:
-            with out_folder.open('{}_band.dat'.format(seedname)) as fil:
+            with out_folder.base.repository.open(f"{seedname}_band.dat") as fil:
                 band_dat = fil.readlines()
-            with out_folder.open('{}_band.kpt'.format(seedname)) as fil:
+            with out_folder.base.repository.open(f"{seedname}_band.kpt") as fil:
                 band_kpt = fil.readlines()
-        except IOError:
+        except OSError:
             # IOError: _band.* files not present
             pass
         else:
             structure = self.node.inputs.structure
             ## TODO: should we catch exceptions here?
             try:
-                with out_folder.open(
-                    '{}_band.labelinfo.dat'.format(seedname)
+                with out_folder.base.repository.open(
+                    f"{seedname}_band.labelinfo.dat"
                 ) as fil:
                     band_labelinfo = fil.readlines()
-            except IOError:  # use legacy parser for wannier90 < 3.0
+            except OSError:  # use legacy parser for wannier90 < 3.0
                 try:
                     kpoint_path = self.node.inputs.kpoint_path
                     special_points = kpoint_path.get_dict()
                 except (exc.NotExistent, KeyError):
                     # exc.NotExistent: no input kpoint_path
                     # KeyError: no get_dict()
                     pass
                 else:
                     output_bandsdata, band_warnings = band_parser_legacy(
                         band_dat, band_kpt, special_points, structure
                     )
-                    self.out('interpolated_bands', output_bandsdata)
+                    self.out("interpolated_bands", output_bandsdata)
             else:
                 output_bandsdata, band_warnings = band_parser(
                     band_dat, band_kpt, band_labelinfo, structure
                 )
-                self.out('interpolated_bands', output_bandsdata)
+                self.out("interpolated_bands", output_bandsdata)
 
         # Parse the stdout an return the parsed data
         wout_dictionary = raw_wout_parser(out_file)
         try:
-            wout_dictionary['warnings'].extend(band_warnings)
+            wout_dictionary["warnings"].extend(band_warnings)
         except (KeyError, NameError):
             # KeyError: wout_dictionary does not contain warnings
             # NameError: no band_warnings
             pass
-        output_data = Dict(dict=wout_dictionary)
-        self.out('output_parameters', output_data)
+        output_data = Dict(wout_dictionary)
+        self.out("output_parameters", output_data)
 
         if exiting_in_stdout:
             return self.exit_codes.ERROR_EXITING_MESSAGE_IN_STDOUT
 
 
-def raw_wout_parser(wann_out_file):  # pylint: disable=too-many-locals,too-many-statements # noqa:  disable=MC0001
-    '''
-    This section will parse a .wout file and return certain key
-    parameters such as the centers and spreads of the
+def raw_wout_parser(
+    wann_out_file,
+):  # pylint: disable=too-many-locals,too-many-statements
+    """Parse a .wout file and return certain key parameters.
+
+    E.g., the centers and spreads of the
     wannier90 functions, the Im/Re ratios, certain warnings,
-    and labels indicating output files produced
+    and labels indicating output files produced.
 
     :param out_file: the .wout file, as a list of strings
     :return out: a dictionary of parameters that can be stored as parameter data
-    '''
-    w90_conv = False  #Used to assess convergence of MLWF procedure use conv_tol and conv_window>1
+    """
+    w90_conv = False  # Used to assess convergence of MLWF procedure use conv_tol and conv_window>1
+    w90_restart = False
     out = {}
-    out.update({'warnings': []})
+    out.update({"warnings": []})
     for i, line in enumerate(wann_out_file):
         # checks for any warnings
-        if 'Warning' in line:
+        if "Warning" in line:
             # Certain warnings get a special flag
-            out['warnings'].append(line)
+            out["warnings"].append(line)
 
         # From the 'initial' part of the output, only sections which indicate
         # whether certain files have been written, e.g. 'Write r^2_nm to file'
         # the units used, e.g. 'Length Unit', that will guide the parser
         # e.g. 'Number of Wannier Functions', or which supplament warnings
         # not directly provided, e.g. unconvergerged wannierization needs
         # some logic in AiiDa to determine whether it met the convergence
         # target or not...
 
         # Parses some of the MAIN parameters
-        if 'MAIN' in line:
+        if "MAIN" in line:
             i += 1
             line = wann_out_file[i]
-            while '-----' not in line:
+            while "-----" not in line:
                 line = wann_out_file[i]
-                if 'Number of Wannier Functions' in line:
-                    out.update({'number_wfs': int(line.split()[-2])})
-                if 'Length Unit' in line:
-                    out.update({'length_units': line.split()[-2]})
-                    if (out['length_units'] != 'Ang'):
-                        out['warnings'].append(
-                            'Units not Ang, '
-                            'be sure this is OK!'
+                if "Number of Wannier Functions" in line:
+                    out.update({"number_wfs": int(line.split()[-2])})
+                if "Length Unit" in line:
+                    out.update({"length_units": line.split()[-2]})
+                    if out["length_units"] != "Ang":
+                        out["warnings"].append("Units not Ang, be sure this is OK!")
+
+                if "Output verbosity (1=low, 5=high)" in line:
+                    out.update({"output_verbosity": int(line.split()[-2])})
+                    if out["output_verbosity"] != 1:
+                        out["warnings"].append(
+                            "Parsing is only supported "
+                            "if output verbosity is set to 1"
                         )
-
-                if 'Output verbosity (1=low, 5=high)' in line:
-                    out.update({'output_verbosity': int(line.split()[-2])})
-                    if out['output_verbosity'] != 1:
-                        out['warnings'].append(
-                            'Parsing is only supported '
-                            'if output verbosity is set to 1'
-                        )
-                if 'Post-processing' in line:
-                    out.update({'preprocess_only': line.split()[-2]})
+                if "Post-processing" in line:
+                    out.update({"preprocess_only": line.split()[-2]})
                 i += 1
 
         # Parses some of the WANNIERISE parameters
-        if 'WANNIERISE' in line:
+        if "WANNIERISE" in line:
             i += 1
             line = wann_out_file[i]
-            while '-----' not in line:
+            while "-----" not in line:
                 line = wann_out_file[i]
-                if 'Convergence tolerence' in line:
-                    out.update({
-                        'convergence_tolerance': float(line.split()[-2])
-                    })
-                if 'Write r^2_nm to file' in line:
-                    out.update({'r2mn_writeout': line.split()[-2]})
-                    if out['r2mn_writeout'] != 'F':
-                        out['warnings'].append(
-                            'The r^2_nm file has been selected '
-                            'to be written, but this is not yet supported!'
+                if "Convergence tolerence" in line:
+                    out.update({"convergence_tolerance": float(line.split()[-2])})
+                if "Write r^2_nm to file" in line:
+                    out.update({"r2mn_writeout": line.split()[-2]})
+                    if out["r2mn_writeout"] != "F":
+                        out["warnings"].append(
+                            "The r^2_nm file has been selected "
+                            "to be written, but this is not yet supported!"
                         )
 
-                if 'Write xyz WF centres to file' in line:
-                    out.update({'xyz_writeout': line.split()[-2]})
-                    if out['xyz_writeout'] != 'F':
-                        out['warnings'].append(
-                            'The xyz_WF_center file has '
-                            'been selected to be written, but this is not '
-                            'yet supported!'
+                if "Write xyz WF centres to file" in line:
+                    out.update({"xyz_writeout": line.split()[-2]})
+                    if out["xyz_writeout"] != "F":
+                        out["warnings"].append(
+                            "The xyz_WF_center file has "
+                            "been selected to be written, but this is not "
+                            "yet supported!"
                         )
 
                 i += 1
-        if 'Wannierisation convergence criteria satisfied' in line:
+        if "Wannierisation convergence criteria satisfied" in line:
             w90_conv = True
 
         # Reading the final WF, also checks to see if they converged or not
-        if 'Final State' in line:
+        if "Final State" in line:
             # Originally wanted to implement automatic convergence check
             # but parsing this using the version below fails depending
             # on the convergence settings used in the aiida.win file
             # Final_check_line = wann_out_file[i-2]
             # if  'Wannierisation convergence criteria satisfied' \
             #         not in Final_check_line:
             #     Final_Delta = float(Final_check_line.split()[-3])
             #     if abs(Final_Delta) > out['convergence_tolerance']:
             #         out['Warnings'] += ['Wannierization not converged within '
             #         'specified tolerance!']
-            num_wf = out['number_wfs']
+            num_wf = out["number_wfs"]
             wf_out = []
             end_wf_loop = i + num_wf + 1
-            for i in range(i + 1, end_wf_loop):
+            for i in range(i + 1, end_wf_loop):  # pylint: disable=redefined-outer-name
                 line = wann_out_file[i]
-                wf_out_i = {'wf_ids': '', 'wf_centres': '', 'wf_spreads': ''}
-                #wf_out_i['wf_ids'] = int(line.split()[-7])
-                wf_out_i['wf_ids'] = int(line.split('(')[0].split()[-1])
-                wf_out_i['wf_spreads'] = float(line.split(')')[1].strip())
-                #wf_out_i['wf_spreads'] = float(line.split()[-1])
+                wf_out_i = {"wf_ids": "", "wf_centres": "", "wf_spreads": ""}
+                # wf_out_i['wf_ids'] = int(line.split()[-7])
+                wf_out_i["wf_ids"] = int(line.split("(")[0].split()[-1])
+                wf_out_i["wf_spreads"] = float(line.split(")")[1].strip())
+                # wf_out_i['wf_spreads'] = float(line.split()[-1])
                 try:
-                    x = float(
-                        line.split('(')[1].split(')')[0].split(',')[0].strip()
-                    )
+                    x = float(line.split("(")[1].split(")")[0].split(",")[0].strip())
                 except (ValueError, IndexError):
                     # To avoid that the crasher completely fails, we set None as a fallback
                     x = None
                 try:
-                    y = float(
-                        line.split('(')[1].split(')')[0].split(',')[1].strip()
-                    )
+                    y = float(line.split("(")[1].split(")")[0].split(",")[1].strip())
                 except (ValueError, IndexError):
                     y = None
                 try:
-                    z = float(
-                        line.split('(')[1].split(')')[0].split(',')[2].strip()
-                    )
+                    z = float(line.split("(")[1].split(")")[0].split(",")[2].strip())
                 except (ValueError, IndexError):
                     z = None
                 coord = (x, y, z)
-                wf_out_i['wf_centres'] = coord
+                wf_out_i["wf_centres"] = coord
                 wf_out.append(wf_out_i)
-            out.update({'wannier_functions_output': wf_out})
-            for i in range(i + 2, i + 6):
+            out.update({"wannier_functions_output": wf_out})
+            for i in range(i + 2, i + 6):  # pylint: disable=redefined-outer-name
                 line = wann_out_file[i]
-                if 'Omega I' in line:
-                    out.update({'Omega_I': float(line.split()[-1])})
-                if 'Omega D' in line:
-                    out.update({'Omega_D': float(line.split()[-1])})
-                if 'Omega OD' in line:
-                    out.update({'Omega_OD': float(line.split()[-1])})
-                if 'Omega Total' in line:
-                    out.update({'Omega_total': float(line.split()[-1])})
+                if "Omega I" in line:
+                    out.update({"Omega_I": float(line.split()[-1])})
+                if "Omega D" in line:
+                    out.update({"Omega_D": float(line.split()[-1])})
+                if "Omega OD" in line:
+                    out.update({"Omega_OD": float(line.split()[-1])})
+                if "Omega Total" in line:
+                    out.update({"Omega_total": float(line.split()[-1])})
+
+        # Reading the initial WF
+        if "Initial State" in line:
+            num_wf = out["number_wfs"]
+            wf_out = []
+            end_wf_loop = i + num_wf + 1
+            for j in range(i + 1, end_wf_loop):
+                line = wann_out_file[j]
+                wf_out_i = {"wf_ids": "", "wf_centres": "", "wf_spreads": ""}
+                # wf_out_i['wf_ids'] = int(line.split()[-7])
+                wf_out_i["wf_ids"] = int(line.split("(")[0].split()[-1])
+                wf_out_i["wf_spreads"] = float(line.split(")")[1].strip())
+                # wf_out_i['wf_spreads'] = float(line.split()[-1])
+                try:
+                    x = float(line.split("(")[1].split(")")[0].split(",")[0].strip())
+                except (ValueError, IndexError):
+                    # To avoid that the crasher completely fails, we set None as a fallback
+                    x = None
+                try:
+                    y = float(line.split("(")[1].split(")")[0].split(",")[1].strip())
+                except (ValueError, IndexError):
+                    y = None
+                try:
+                    z = float(line.split("(")[1].split(")")[0].split(",")[2].strip())
+                except (ValueError, IndexError):
+                    z = None
+                coord = (x, y, z)
+                wf_out_i["wf_centres"] = coord
+                wf_out.append(wf_out_i)
+            out.update({"wannier_functions_initial": wf_out})
 
-        if ' Maximum Im/Re Ratio' in line:
-            wann_functions = out['wannier_functions_output']
+        if "Reading restart information from file" in line:
+            w90_restart = True
+            # When restart for plotting WFs, there might be no `out['wannier_functions_output']`
+            wann_functions = []
+
+        if " Maximum Im/Re Ratio" in line:
             wann_id = int(line.split()[3])
-            wann_function = wann_functions[wann_id - 1]
-            wann_function.update({'im_re_ratio': float(line.split()[-1])})
-    if not w90_conv:
-        out['warnings'].append(
-            'Wannierisation finished because num_iter was reached.'
-        )
+            wann_ratio = float(line.split()[-1])
+            if w90_restart:
+                wann_functions.append({"wf_ids": wann_id, "im_re_ratio": wann_ratio})
+            else:
+                wann_functions = out["wannier_functions_output"]
+                wann_function = wann_functions[wann_id - 1]
+                wann_function.update({"im_re_ratio": wann_ratio})
+    if w90_restart:
+        if "wannier_functions_output" not in out and len(wann_functions) > 0:
+            out["wannier_functions_output"] = wann_functions
+        else:
+            for wann_function in wann_functions:
+                wann_id = wann_function["wf_ids"]
+                wann_out = out["wannier_functions_output"][wann_id - 1]
+                if wann_out["wf_ids"] != wann_id:
+                    raise ValueError(
+                        f"Failed to parse `wannier_functions_output` for wf_ids = {wann_id}"
+                    )
+                wann_out.update(wann_functions)
+    if not w90_restart and not w90_conv:
+        out["warnings"].append("Wannierisation finished because num_iter was reached.")
     return out
 
 
-def band_parser(band_dat, band_kpt, band_labelinfo, structure):  # pylint: disable=too-many-locals
-    """
-    Parsers the bands output data to construct a BandsData object which is then
-    returned. Used for wannier90 >= 3.0
+def band_parser(band_dat, band_kpt, band_labelinfo, structure):
+    """Parser the bands output data to construct a BandsData object.
+
+    Used for wannier90 >= 3.0
 
     :param band_dat: list of str with each str stores one line of aiida_band.dat file
     :param band_kpt: list of str with each str stores one line of aiida_band.kpt file
     :param band_labelinfo: list of str with each str stores one line in aiida_band.labelinfo.dat file
     :return: BandsData object constructed from the input params
     """
     import numpy as np
 
-    from aiida.orm import BandsData
-    from aiida.orm import KpointsData
+    from aiida.orm import BandsData, KpointsData
 
     warnings = []
 
     # imports the data
     out_kpt = np.genfromtxt(band_kpt, skip_header=1, usecols=(0, 1, 2))
     out_dat = np.genfromtxt(band_dat, usecols=1)
 
     # reshaps the output bands
-    out_dat = out_dat.reshape(
-        len(out_kpt), (len(out_dat) // len(out_kpt)), order="F"
-    )
+    out_dat = out_dat.reshape(len(out_kpt), (len(out_dat) // len(out_kpt)), order="F")
 
     labels_dict = {}
     for line_idx, line in enumerate(band_labelinfo, start=1):
         if not line.strip():
             continue
         try:
             # label, idx, xval, kx, ky, kz = line.split()
             label, idx, _, _, _, _ = line.split()
         except ValueError:
-            warnings.append((
-                'Wrong number of items in line {} of the labelinfo file - '
-                'I will not assign that label'
-            )).format(line_idx)
+            warnings.append(
+                "Wrong number of items in line {} of the labelinfo file - "
+                "I will not assign that label"
+            ).format(line_idx)
             continue
         try:
             idx = int(idx)
         except ValueError:
-            warnings.append((
-                "Invalid value for the index in line {} of the labelinfo file, "
+            warnings.append(
+                f"Invalid value for the index in line {line_idx} of the labelinfo file, "
                 "it's not an integer - I will not assign that label"
-            )).format(line_idx)
+            )
             continue
 
         # I use a dictionary because there are cases in which there are
         # two lines for the same point (e.g. when I do a zero-length path,
         # from a point to the same point, just to have that value)
         # Note the -1 because in fortran indices are 1-based, in Python are
         # 0-based
@@ -369,72 +441,74 @@
     labels = [(key, labels_dict[key]) for key in sorted(labels_dict)]
 
     bands = BandsData()
     k = KpointsData()
     k.set_cell_from_structure(structure)
     k.set_kpoints(out_kpt, cartesian=False)
     bands.set_kpointsdata(k)
-    bands.set_bands(out_dat, units='eV')
+    bands.set_bands(out_dat, units="eV")
     bands.labels = labels
     return bands, warnings
 
 
-def band_parser_legacy(band_dat, band_kpt, special_points, structure):  # pylint: disable=too-many-locals
-    """
-    Parsers the bands output data, along with the special points retrieved
+def band_parser_legacy(
+    band_dat, band_kpt, special_points, structure
+):  # pylint: disable=too-many-locals
+    """Parse the bands output data.
+
+    Along with the special points retrieved
     from the input kpoints to construct a BandsData object which is then
     returned. Cannot handle discontinuities in the kpath, if two points are
     assigned to same spot only one will be passed. Used for wannier90 < 3.0
     :param band_dat: list of str with each str stores one line of aiida_band.dat file
     :param band_kpt: list of str with each str stores one line of aiida_band.kpt file
     :param special_points: special points to add labels to the bands a dictionary in
         the form expected in the input as described in the wannier90 documentation
     :return: BandsData object constructed from the input params,
         and a list contains warnings.
     """
     import numpy as np
 
-    from aiida.orm import BandsData
-    from aiida.orm import KpointsData
+    from aiida.orm import BandsData, KpointsData
 
     warnings = []
-    warnings.append((
+    warnings.append(
         "Note: no file named SEEDNAME_band.labelinfo.dat found. "
         "You are probably using a version of Wannier90 before 3.0. "
         "There, the labels associated with each k-points were not printed in output "
         "and there were also cases in which points were not calculated "
         "(see issue #195 on the Wannier90 GitHub page). "
         "I will anyway try to do my best to assign labels, "
         "but the assignment might be wrong "
         "(especially if there are path discontinuities)."
-    ))
+    )
 
     # imports the data
     out_kpt = np.genfromtxt(band_kpt, skip_header=1, usecols=(0, 1, 2))
     out_dat = np.genfromtxt(band_dat, usecols=1)
 
     # reshaps the output bands
-    out_dat = out_dat.reshape(
-        len(out_kpt), (len(out_dat) // len(out_kpt)), order="F"
-    )
+    out_dat = out_dat.reshape(len(out_kpt), (len(out_dat) // len(out_kpt)), order="F")
 
     # finds expected points of discontinuity
-    kpath = special_points['path']
-    cont_break = [(i, (kpath[i - 1][1], kpath[i][0]))
-                  for i in range(1, len(kpath))
-                  if kpath[i - 1][1] != kpath[i][0]]
+    kpath = special_points["path"]
+    cont_break = [
+        (i, (kpath[i - 1][1], kpath[i][0]))
+        for i in range(1, len(kpath))
+        if kpath[i - 1][1] != kpath[i][0]
+    ]
 
     # finds the special points
-    special_points_dict = special_points['point_coords']
+    special_points_dict = special_points["point_coords"]
     # We set atol to 1e-5 because in the kpt file the coords are printed with fixed precision
     labels = [
-        (i, k) for k in special_points_dict for i in range(len(out_kpt))
-        if all(
-            np.isclose(special_points_dict[k], out_kpt[i], rtol=0, atol=1.e-5)
-        )
+        (i, k)
+        for k in special_points_dict
+        for i in range(len(out_kpt))
+        if all(np.isclose(special_points_dict[k], out_kpt[i], rtol=0, atol=1.0e-5))
     ]
     labels.sort()
 
     # Checks and appends labels if discontinuity
     appends = []
     for x in cont_break:
         # two cases the break is before or the break is after
@@ -455,16 +529,16 @@
             insert_point = x[0] + 1
             new_label = x[1][1]
             kpoint = labels[x[0]][0] + 1
             appends += [[insert_point, new_label, kpoint]]
     appends.sort()
 
     for i, append in enumerate(appends):
-        labels.insert(append[0] + i, (append[2], six.text_type(append[1])))
+        labels.insert(append[0] + i, (append[2], str(append[1])))
     bands = BandsData()
     k = KpointsData()
     k.set_cell_from_structure(structure)
     k.set_kpoints(out_kpt, cartesian=False)
     bands.set_kpointsdata(k)
-    bands.set_bands(out_dat, units='eV')
+    bands.set_bands(out_dat, units="eV")
     bands.labels = labels
     return bands, warnings
```

### Comparing `aiida-wannier90-2.0.1/aiida_wannier90/calculations.py` & `aiida_wannier90-2.1.0/src/aiida_wannier90/calculations/wannier90.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,239 +1,331 @@
-# -*- coding: utf-8 -*-
 ################################################################################
 # Copyright (c), AiiDA team and individual contributors.                       #
 #  All rights reserved.                                                        #
 # This file is part of the AiiDA-wannier90 code.                               #
 #                                                                              #
 # The code is hosted on GitHub at https://github.com/aiidateam/aiida-wannier90 #
 # For further information on the license, see the LICENSE.txt file             #
 ################################################################################
-from __future__ import absolute_import, print_function, division
-import os
-import six
-import fnmatch
+"""Calculation for the Wannier90 code."""
 from collections import namedtuple
+import fnmatch
+import os
 
 from aiida.common import datastructures
 from aiida.common import exceptions as exc
 from aiida.engine import CalcJob
 from aiida.orm import (
-    BandsData, Dict, FolderData, KpointsData, List, OrbitalData, RemoteData,
-    SinglefileData, StructureData
+    BandsData,
+    Dict,
+    FolderData,
+    KpointsData,
+    List,
+    OrbitalData,
+    RemoteData,
+    SinglefileData,
+    StructureData,
 )
 
-from .io import write_win
+from ..io import write_win
 
-__all__ = ('Wannier90Calculation', )
+__all__ = ("Wannier90Calculation",)
 
 _InputFileLists = namedtuple(
-    '_InputFileLists',
-    ('local_copy_list', 'remote_copy_list', 'remote_symlink_list')
+    "_InputFileLists", ("local_copy_list", "remote_copy_list", "remote_symlink_list")
 )
 # When support for Python <3.7 is dropped, we can set 'default=(False, False)'
 # here, and remove the extra kwargs in the constructor calls -- or use
 # a dataclass to implement the same.
-_InputFileSpec = namedtuple(
-    '_InputFileSpec', ('suffix', 'required', 'always_copy')
-)
+_InputFileSpec = namedtuple("_InputFileSpec", ("suffix", "required", "always_copy"))
+
+
+def validate_inputs_base(  # pylint: disable=unused-argument,inconsistent-return-statements
+    inputs, ctx=None
+):
+    """Validate the inputs of the entire input namespace."""
+
+    # Cannot specify both `kpoint_path` and `bands_kpoints`
+    if all(key in inputs for key in ["kpoint_path", "bands_kpoints"]):
+        return "Cannot specify both `kpoint_path` and `bands_kpoints`."
+
+    # `bands_kpoints` must contain `labels`
+    if "bands_kpoints" in inputs:
+        if inputs["bands_kpoints"].labels is None:
+            return "`bands_kpoints` must contain `labels`."
+
+
+def validate_inputs(inputs, ctx=None):  # pylint: disable=inconsistent-return-statements
+    """Validate the inputs of the entire input namespace."""
+
+    results = validate_inputs_base(inputs, ctx)
+    if results:
+        return results
+
+    # Check bands_plot and kpoint_path, bands_kpoints
+    bands_plot = inputs["parameters"].get_dict().get("bands_plot", False)
+    if bands_plot:
+        kpoint_path = inputs.get("kpoint_path", None)
+        bands_kpoints = inputs.get("bands_kpoints", None)
+        if kpoint_path is None and bands_kpoints is None:
+            return (
+                "`bands_plot` is True but no `kpoint_path` or `bands_kpoints` provided"
+            )
 
 
 class Wannier90Calculation(CalcJob):
+    """Plugin for Wannier90.
+
+    Wannier90 is a code for computing maximally-localized Wannier functions.
+    See http://www.wannier.org/ for more details.
     """
-    Plugin for Wannier90, a code for computing maximally-localized Wannier
-    functions. See http://www.wannier.org/ for more details.
-    """
+
     # The input filename MUST end with .win. This is validated by the prepare_for_submission
     _REQUIRED_INPUT_SUFFIX = ".win"
-    _DEFAULT_INPUT_FILE = 'aiida.win'
-    _DEFAULT_OUTPUT_FILE = 'aiida.wout'
+    _DEFAULT_INPUT_FILE = "aiida.win"
+    _DEFAULT_OUTPUT_FILE = "aiida.wout"
 
     # The following ones CANNOT be set by the user - in this case an exception will be raised
     # IMPORTANT: define them here in lower-case
     _BLOCKED_PARAMETER_KEYS = (
-        'length_unit',
-        'unit_cell_cart',
-        'atoms_cart',
-        'projections',
-        'postproc_setup'  # Pass instead a 'postproc_setup' in the input `settings` node
+        "length_unit",
+        "unit_cell_cart",
+        "atoms_cart",
+        "projections",
+        "postproc_setup",  # Pass instead a 'postproc_setup' in the input `settings` node
     )
 
     # By default, retrieve all produced files except .nnkp (which
     # is handled separately) and .chk (checkpoint files are large,
     # and usually not needed).
     _DEFAULT_RETRIEVE_SUFFIXES = (
-        '.wout', '.werr', '.r2mn', '_band.dat', '_band.dat', '_band.agr',
-        '_band.kpt', '.bxsf', '_w.xsf', '_w.cube', '_centres.xyz', '_hr.dat',
-        '_tb.dat', '_r.dat', '.bvec', '_wsvec.dat', '_qc.dat', '_dos.dat',
-        '_htB.dat', '_u.mat', '_u_dis.mat', '.vdw', '_band_proj.dat',
-        '_band.labelinfo.dat'
+        ".wout",
+        ".werr",
+        ".r2mn",
+        "_band.dat",
+        "_band.dat",
+        "_band.agr",
+        "_band.kpt",
+        ".bxsf",
+        "_w.xsf",
+        "_w.cube",
+        "_centres.xyz",
+        "_hr.dat",
+        "_tb.dat",
+        "_r.dat",
+        ".bvec",
+        "_wsvec.dat",
+        "_qc.dat",
+        "_dos.dat",
+        "_htB.dat",
+        "_u.mat",
+        "_u_dis.mat",
+        ".vdw",
+        "_band_proj.dat",
+        "_band.labelinfo.dat",
+        ".node_00001.werr",
     )
 
     @classmethod
-    def define(cls, spec):  # pylint: disable=no-self-argument
-        super(Wannier90Calculation, cls).define(spec)
+    def define(cls, spec):
+        """Define the specs."""
+        super().define(spec)
         spec.input(
-            "structure",
-            valid_type=StructureData,
-            help="input crystal structure"
+            "structure", valid_type=StructureData, help="input crystal structure"
         )
         spec.input(
             "parameters",
             valid_type=Dict,
-            help="Input parameters for the Wannier90 code"
+            help="Input parameters for the Wannier90 code",
         )
         spec.input(
             "settings",
             valid_type=Dict,
             required=False,
-            help="""Additional settings to manage the Wannier90 calculation."""
+            help="""Additional settings to manage the Wannier90 calculation.""",
         )
         spec.input(
             "projections",
             valid_type=(OrbitalData, Dict, List),
             help="Starting projections for the Wannierisation procedure.",
-            required=False
+            required=False,
         )
         spec.input(
             "local_input_folder",
             valid_type=FolderData,
             required=False,
-            help=
-            "Get input files (``.amn``, ``.mmn``, ...) from a class ``FolderData`` stored in the AiiDA repository."
+            help=(
+                "Get input files (``.amn``, ``.mmn``, ...) from "
+                "a class ``FolderData`` stored in the AiiDA repository."
+            ),
         )
         spec.input(
             "remote_input_folder",
             valid_type=RemoteData,
             required=False,
-            help=
-            "Get input files (``.amn``, ``.mmn``, ...) from a class ``RemoteData`` possibly stored in a remote computer."
+            help=(
+                "Get input files (``.amn``, ``.mmn``, ...) from a class "
+                "``RemoteData`` possibly stored in a remote computer."
+            ),
         )
         spec.input(
             "kpoints",
             valid_type=KpointsData,
-            help="k-point mesh used in the NSCF calculation."
+            help="k-point mesh used in the NSCF calculation.",
         )
         spec.input(
             "kpoint_path",
             valid_type=Dict,
             required=False,
-            help=
-            "Description of the k-points path to be used for bands interpolation; "
-            "it should contain two properties: "
-            "a list ``path`` of length-2 tuples with the labels of the endpoints of the path; and "
-            "a dictionary ``point_coords`` giving the scaled coordinates for each high-symmetry endpoint."
+            help=(
+                "Description of the k-points path to be used for bands interpolation; "
+                "it should contain two properties: "
+                "a list ``path`` of length-2 tuples with the labels of the endpoints of the path; and "
+                "a dictionary ``point_coords`` giving the scaled coordinates for each high-symmetry endpoint."
+            ),
         )
+        spec.input(
+            "bands_kpoints",
+            valid_type=KpointsData,
+            required=False,
+            help=(
+                "A list of k-points along a path to be used for bands interpolation; "
+                "it should contain `labels`. Specify either this or `kpoint_path`."
+            ),
+        )
+        spec.inputs.validator = validate_inputs
 
         spec.output(
-            'output_parameters',
+            "output_parameters",
             valid_type=Dict,
-            help=
-            'The ``output_parameters`` output node of the successful calculation.'
+            help="The ``output_parameters`` output node of the successful calculation.",
         )
         spec.output(
-            'interpolated_bands',
+            "interpolated_bands",
             valid_type=BandsData,
             required=False,
-            help='The interpolated band structure by Wannier90 (if any).'
+            help="The interpolated band structure by Wannier90 (if any).",
         )
         spec.output(
-            'nnkp_file',
+            "nnkp_file",
             valid_type=SinglefileData,
             required=False,
-            help='The ``.nnkp`` file, produced only in -pp (postproc) mode.'
+            help="The ``.nnkp`` file, produced only in -pp (postproc) mode.",
         )
-        spec.default_output_node = 'output_parameters'
+        spec.default_output_node = "output_parameters"
 
         spec.input(
-            'metadata.options.input_filename',
-            valid_type=six.string_types,
-            default=cls._DEFAULT_INPUT_FILE
+            "metadata.options.input_filename",
+            valid_type=str,
+            default=cls._DEFAULT_INPUT_FILE,
         )
         spec.input(
-            'metadata.options.output_filename',
-            valid_type=six.string_types,
-            default=cls._DEFAULT_OUTPUT_FILE
+            "metadata.options.output_filename",
+            valid_type=str,
+            default=cls._DEFAULT_OUTPUT_FILE,
         )
         spec.input(
-            'metadata.options.parser_name',
-            valid_type=six.string_types,
-            default='wannier90.wannier90'
+            "metadata.options.parser_name",
+            valid_type=str,
+            default="wannier90.wannier90",
         )
         # withmpi defaults to "False" in aiida-core 1.0. Below, we override to default to withmpi=True
-        spec.input('metadata.options.withmpi', valid_type=bool, default=True)
+        spec.input("metadata.options.withmpi", valid_type=bool, default=True)
         spec.exit_code(
             200,
-            'ERROR_NO_RETRIEVED_FOLDER',
-            message='The retrieved folder data node could not be accessed.'
+            "ERROR_NO_RETRIEVED_FOLDER",
+            message="The retrieved folder data node could not be accessed.",
+            invalidates_cache=True,
         )
         spec.exit_code(
             210,
-            'ERROR_OUTPUT_STDOUT_MISSING',
-            message=
-            'The retrieved folder did not contain the required stdout output file.'
+            "ERROR_OUTPUT_STDOUT_MISSING",
+            message="The retrieved folder did not contain the required stdout output file.",
+            invalidates_cache=True,
         )
         spec.exit_code(
             300,
-            'ERROR_WERR_FILE_PRESENT',
-            message='A Wannier90 error file (.werr) has been found.'
+            "ERROR_WERR_FILE_PRESENT",
+            message="A Wannier90 error file (.werr) has been found.",
         )
         spec.exit_code(
             400,
-            'ERROR_EXITING_MESSAGE_IN_STDOUT',
-            message=
-            'The string "Exiting..." has been found in the Wannier90 output (some partial output might have been '
-            'parsed).'
+            "ERROR_EXITING_MESSAGE_IN_STDOUT",
+            message=(
+                'The string "Exiting..." has been found in the Wannier90 output '
+                "(some partial output might have been parsed)."
+            ),
+        )
+        spec.exit_code(
+            401,
+            "ERROR_BVECTORS",
+            message="An error related to bvectors has been found in the Wannier90 output.",
+        )
+        spec.exit_code(
+            402,
+            "ERROR_DISENTANGLEMENT_NOT_ENOUGH_STATES",
+            message="Energy window contains fewer states than number of target WFs.",
+        )
+        spec.exit_code(
+            403,
+            "ERROR_PLOT_WF_CUBE",
+            message="Error plotting Wanier functions in cube format.",
+        )
+        spec.exit_code(
+            404,
+            "ERROR_OUTPUT_STDOUT_INCOMPLETE",
+            message="The stdout output file was incomplete probably because the calculation got interrupted.",
         )
 
     @property
     def _SEEDNAME(self):
-        """
-        Return the default seedname, unless a custom one has been set in the
-        calculation settings.
+        """Return the default seedname, unless a custom one has been set in the calculation settings.
 
         :raise ValueError: if the input_filename does not end with ``.win``.
         """
         input_filename = self.inputs.metadata.options.input_filename
 
         if input_filename.endswith(self._REQUIRED_INPUT_SUFFIX):
-            return input_filename[:-len(self._REQUIRED_INPUT_SUFFIX)]
+            return input_filename[: -len(self._REQUIRED_INPUT_SUFFIX)]
 
         # If we are here, it's an invalid input filename.
         raise ValueError(
-            "The input filename '{}' does not end with '{}', so I don't know how to get the seedname. "
+            f"The input filename '{input_filename}' does not end with '{self._REQUIRED_INPUT_SUFFIX}', "
+            "so I don't know how to get the seedname. "
             "You need to change the `metadata.options.input_filename` in the process inputs."
-            .format(input_filename, self._REQUIRED_INPUT_SUFFIX)
         )
 
-    def prepare_for_submission(self, folder):  #pylint: disable=too-many-locals, too-many-statements # noqa:  disable=MC0001
-        """
-        Routine which creates the input file of Wannier90
+    def prepare_for_submission(
+        self, folder
+    ):  # pylint: disable=too-many-locals, too-many-statements # noqa:  disable=MC0001
+        """Create the input file of Wannier90.
+
         :param folder: a aiida.common.folders.Folder subclass where
             the plugin should put all its files.
         """
         self._validate_input_output_names()
 
         param_dict = self.inputs.parameters.get_dict()
         self._validate_lowercase(param_dict)
         self._validate_input_parameters(param_dict)
 
-        if 'settings' in self.inputs:
+        if "settings" in self.inputs:
             settings_dict = self.inputs.settings.get_dict()
         else:
             settings_dict = {}
         self._validate_lowercase(settings_dict)
 
-        pp_setup = settings_dict.pop('postproc_setup', False)
+        pp_setup = settings_dict.pop("postproc_setup", False)
         if pp_setup:
-            param_dict.update({'postproc_setup': True})
+            param_dict.update({"postproc_setup": True})
 
-        has_local_input = 'local_input_folder' in self.inputs
-        has_remote_input = 'remote_input_folder' in self.inputs
+        has_local_input = "local_input_folder" in self.inputs
+        has_remote_input = "remote_input_folder" in self.inputs
         if pp_setup:
-            if has_local_input or has_local_input:
+            if has_local_input or has_remote_input:
                 raise exc.InputValidationError(
                     "Can not set 'local_input_folder' or 'remote_input_folder' "
                     "with the 'postproc_setup' option."
                 )
 
         else:
             if has_local_input and has_remote_input:
@@ -247,250 +339,242 @@
                     "None of the 'local_input_folder' and 'remote_input_folder' "
                     "inputs is set. Exactly one of the two must be given."
                 )
 
         ############################################################
         # End basic check on inputs
         ############################################################
-        random_projections = settings_dict.pop('random_projections', False)
+        random_projections = settings_dict.pop("random_projections", False)
 
         write_win(
-            filename=folder.get_abs_path('{}.win'.format(self._SEEDNAME)),
+            filename=folder.get_abs_path(f"{self._SEEDNAME}.win"),
             parameters=param_dict,
             structure=self.inputs.structure,
             kpoints=self.inputs.kpoints,
-            kpoint_path=getattr(self.inputs, 'kpoint_path', None),
-            projections=getattr(self.inputs, 'projections', None),
+            kpoint_path=getattr(self.inputs, "kpoint_path", None),
+            bands_kpoints=getattr(self.inputs, "bands_kpoints", None),
+            projections=getattr(self.inputs, "projections", None),
             random_projections=random_projections,
         )
 
         input_file_lists = self._get_input_file_lists(pp_setup=pp_setup)
 
         #######################################################################
 
         calcinfo = datastructures.CalcInfo()
         calcinfo.uuid = self.uuid
         calcinfo.local_copy_list = input_file_lists.local_copy_list + settings_dict.pop(
             "additional_local_copy_list", []
         )
-        calcinfo.remote_copy_list = input_file_lists.remote_copy_list + settings_dict.pop(
-            "additional_remote_copy_list", []
-        )
-        calcinfo.remote_symlink_list = input_file_lists.remote_symlink_list + settings_dict.pop(
-            "additional_remote_symlink_list", []
+        calcinfo.remote_copy_list = (
+            input_file_lists.remote_copy_list
+            + settings_dict.pop("additional_remote_copy_list", [])
+        )
+        calcinfo.remote_symlink_list = (
+            input_file_lists.remote_symlink_list
+            + settings_dict.pop("additional_remote_symlink_list", [])
         )
 
         codeinfo = datastructures.CodeInfo()
         codeinfo.code_uuid = self.inputs.code.uuid
         codeinfo.cmdline_params = [self._SEEDNAME]
 
         calcinfo.codes_info = [codeinfo]
         calcinfo.codes_run_mode = datastructures.CodeRunMode.SERIAL
 
         retrieve_list = [
-            self._SEEDNAME + suffix
-            for suffix in self._DEFAULT_RETRIEVE_SUFFIXES
+            self._SEEDNAME + suffix for suffix in self._DEFAULT_RETRIEVE_SUFFIXES
         ]
         exclude_retrieve_list = settings_dict.pop("exclude_retrieve_list", [])
         retrieve_list = [
-            filename for filename in retrieve_list if not any(
-                fnmatch.fnmatch(filename, pattern)
-                for pattern in exclude_retrieve_list
+            filename
+            for filename in retrieve_list
+            if not any(
+                fnmatch.fnmatch(filename, pattern) for pattern in exclude_retrieve_list
             )
         ]
 
         calcinfo.retrieve_list = retrieve_list
         calcinfo.retrieve_temporary_list = []
         if pp_setup:
             # The parser will then put this in a SinglefileData (if present)
-            calcinfo.retrieve_temporary_list.append(
-                '{}.nnkp'.format(self._SEEDNAME)
-            )
+            calcinfo.retrieve_temporary_list.append(f"{self._SEEDNAME}.nnkp")
 
         # Retrieves bands automatically, if they are calculated
 
-        calcinfo.retrieve_list += settings_dict.pop(
-            "additional_retrieve_list", []
-        )
+        calcinfo.retrieve_list += settings_dict.pop("additional_retrieve_list", [])
 
         # pop input keys not used here
-        settings_dict.pop('seedname', None)
+        settings_dict.pop("seedname", None)
         if settings_dict:
             raise exc.InputValidationError(
-                "The following keys in settings are unrecognized: {}".format(
-                    list(settings_dict.keys())
-                )
+                f"The following keys in settings are unrecognized: {list(settings_dict.keys())}"
             )
 
         return calcinfo
 
     def _validate_input_output_names(self):
-        """
-        This function validates the input and output file names given in the
-        settings Dict.
-        """
+        """Validate the input and output file names given in the settings Dict."""
         # Let's check that the user-specified input filename ends with .win
         if not self.inputs.metadata.options.input_filename.endswith(
             self._REQUIRED_INPUT_SUFFIX
         ):
             raise exc.InputValidationError(
                 "The input filename for Wannier90 (specified in the metadata.options.input_filename) "
-                "must end with .win, you specified instead '{}'".format(
-                    self.inputs.metadata.options.input_filename
-                )
+                f"must end with .win, you specified instead '{self.inputs.metadata.options.input_filename}'"
             )
 
         # The output filename is defined by Wannier90 based on the seedname.
         # In AiiDA, the output_filename needs to be specified as a metadata.option to allow for
         # `verdi calcjob outputcat` to work correctly. Here we check that, if the users manually changed
         # the input_filename, they also changed the output_filename accordingly
         expected_output_filename = self._SEEDNAME + ".wout"
         if self.inputs.metadata.options.output_filename != expected_output_filename:
             raise exc.InputValidationError(
                 "The output filename specified is wrong. You probably changed the metadata.options.input_filename "
                 "but you forgot to adapt the metadata.options.output_filename accordingly! Currently, you have: "
-                "input_filename: '{}', output_filename: '{}', while I would expect '{}'"
-                .format(
-                    self.inputs.metadata.options.input_filename,
-                    self.inputs.metadata.options.output_filename,
-                    expected_output_filename
-                )
+                f"input_filename: '{self.inputs.metadata.options.input_filename}', "
+                f"output_filename: '{self.inputs.metadata.options.output_filename}', "
+                f"while I would expect '{expected_output_filename}'"
             )
 
     @staticmethod
     def _validate_lowercase(dictionary):
-        """
-        This function gets a dictionary and checks that all keys are lower-case.
+        """Get a dictionary and checks that all keys are lower-case.
 
         :param dict_node: a dictionary
         :raises InputValidationError: if any of the keys is not lower-case
         :return: ``None`` if validation passes
         """
         non_lowercase = []
         for key in dictionary:
             if key != key.lower():
                 non_lowercase.append(key)
         if non_lowercase:
             raise exc.InputValidationError(
-                "input keys to the Wannier90 plugin must be all lower-case, but the following aren't : {}"
-                .format(", ".join(non_lowercase))
+                "input keys to the Wannier90 plugin must be all lower-case, "
+                f"but the following aren't : {', '.join(non_lowercase)}"
             )
 
     def _validate_input_parameters(self, parameters):
-        """
-        This function gets a dictionary with the content of the parameters Dict passed by the user
-        and performs some validation.
+        """Get a dictionary with the content of the parameters Dict passed by the user and perform some validation.
 
         In particular, it checks that there are no blocked parameters keys passed.
 
         :param dict_node: a dictionary
         :raises InputValidationError: if any of the validation fails
         :return: ``None`` if validation passes
         """
         existing_blocked_keys = []
         for key in self._BLOCKED_PARAMETER_KEYS:
             if key in parameters:
                 existing_blocked_keys.append(key)
         if existing_blocked_keys:
             raise exc.InputValidationError(
-                'The following blocked keys were found in the parameters: {}'.
-                format(", ".join(existing_blocked_keys))
+                f'The following blocked keys were found in the parameters: {", ".join(existing_blocked_keys)}'
             )
 
     def _get_input_file_lists(self, pp_setup):
-        """
-        Generate the lists of files to copy and link from the
-        'local_input_folder' and 'remote_input_folder'.
-        """
+        """Generate the lists of files to copy and link from the 'local_input_folder' and 'remote_input_folder'."""
         if pp_setup:
             return _InputFileLists([], [], [])
 
-        input_file_specs = [
-            _InputFileSpec(suffix=suffix, required=True, always_copy=False)
-            for suffix in ['.mmn', '.amn']
-        ] + [
-            _InputFileSpec(suffix=suffix, required=False, always_copy=False)
-            for suffix in [
-                '.eig', '.spn', '.uHu', '_htB.dat', '_htL.dat', '_htR.dat',
-                '_htC.dat', '_htLC.dat', '_htCR.dat', '.unkg'
+        input_file_specs = (
+            [
+                _InputFileSpec(suffix=suffix, required=True, always_copy=False)
+                for suffix in [".mmn", ".amn"]
+            ]
+            + [
+                _InputFileSpec(suffix=suffix, required=False, always_copy=False)
+                for suffix in [
+                    ".eig",
+                    ".spn",
+                    ".uHu",
+                    "_htB.dat",
+                    "_htL.dat",
+                    "_htR.dat",
+                    "_htC.dat",
+                    "_htLC.dat",
+                    "_htCR.dat",
+                    ".unkg",
+                ]
             ]
-        ] + [_InputFileSpec(suffix='.chk', required=False, always_copy=True)]
+            + [_InputFileSpec(suffix=".chk", required=False, always_copy=True)]
+        )
 
-        optional_file_globs = ['UNK*']
+        # Only symlink UNK* when plotting Wannier functions, to save inodes.
+        if self.inputs["parameters"].get_dict().get("wannier_plot", False):
+            optional_file_globs = ["UNK*"]
+        else:
+            optional_file_globs = []
 
-        if 'remote_input_folder' in self.inputs:
+        if "remote_input_folder" in self.inputs:
             return self._get_remote_input_file_lists(
                 input_file_specs=input_file_specs,
-                optional_file_globs=optional_file_globs
+                optional_file_globs=optional_file_globs,
             )
         return self._get_local_input_file_lists(
-            input_file_specs=input_file_specs,
-            optional_file_globs=optional_file_globs
+            input_file_specs=input_file_specs, optional_file_globs=optional_file_globs
         )
 
-    def _get_remote_input_file_lists(
-        self, input_file_specs, optional_file_globs
-    ):
-        """
-        Generate the lists of input files for the case of a remote input folder.
-        """
+    def _get_remote_input_file_lists(self, input_file_specs, optional_file_globs):
+        """Generate the lists of input files for the case of a remote input folder."""
         remote_input_folder_uuid = self.inputs.remote_input_folder.computer.uuid
-        remote_input_folder_path = self.inputs.remote_input_folder.get_remote_path(
-        )
+        remote_input_folder_path = self.inputs.remote_input_folder.get_remote_path()
 
         remote_copy_list = []
         # We use globbing for optional input files because the 'copy'
         # call in the 'upload' step of the calculation does not fail
         # if a pattern does not match any files. If we were to use the
         # explicit file name, the 'upload' would fail if the file does
         # not exist. See also aiida-core issue #3813.
-        remote_symlink_list = [(
-            remote_input_folder_uuid,
-            os.path.join(remote_input_folder_path, pattern), '.'
-        ) for pattern in optional_file_globs]
+        remote_symlink_list = [
+            (
+                remote_input_folder_uuid,
+                os.path.join(remote_input_folder_path, pattern),
+                ".",
+            )
+            for pattern in optional_file_globs
+        ]
         for file_spec in input_file_specs:
             if file_spec.required:
                 filename = self._SEEDNAME + file_spec.suffix
                 file_info = (
                     remote_input_folder_uuid,
-                    os.path.join(remote_input_folder_path, filename), filename
+                    os.path.join(remote_input_folder_path, filename),
+                    filename,
                 )
             else:
                 # Use globbing for optional files, see comment above.
                 file_info = (
                     remote_input_folder_uuid,
-                    os.path.join(
-                        remote_input_folder_path, '*' + file_spec.suffix
-                    ), '.'
+                    os.path.join(remote_input_folder_path, "*" + file_spec.suffix),
+                    ".",
                 )
             if file_spec.always_copy:
                 remote_copy_list.append(file_info)
             else:
                 remote_symlink_list.append(file_info)
         return _InputFileLists(
             local_copy_list=[],
             remote_copy_list=remote_copy_list,
-            remote_symlink_list=remote_symlink_list
+            remote_symlink_list=remote_symlink_list,
         )
 
-    def _get_local_input_file_lists(
-        self, input_file_specs, optional_file_globs
-    ):
-        """
-        Generate the lists of input files for the case of a local input folder.
-        """
+    def _get_local_input_file_lists(self, input_file_specs, optional_file_globs):
+        """Generate the lists of input files for the case of a local input folder."""
         # It is possible that the same file is matched multiple times,
         # for example if a globbing pattern matches an explicit filename.
         # To avoid copying the same file twice (which could be costly),
         # we keep track of which local folder content is already in the
         # list of files to copy.
         # To avoid false errors, the explicit files (and thus the required
         # ones) are checked first, before doing pattern-matching.
         local_folder_content = set(
-            self.inputs.local_input_folder.list_object_names()
+            self.inputs.local_input_folder.base.repository.list_object_names()
         )
 
         def _get_local_file_info(filename):
             return (self.inputs.local_input_folder.uuid, filename, filename)
 
         local_copy_list = []
         not_found = []
@@ -500,26 +584,23 @@
                 local_copy_list.append(_get_local_file_info(filename))
                 local_folder_content.remove(filename)
             elif file_spec.required:
                 not_found.append(filename)
 
         if not_found:
             raise exc.InputValidationError(
-                "{} necessary input files were not found: {} (NOTE: if you "
+                f"{len(not_found)} necessary input files were not found: "
+                f"{', '.join(str(nf) for nf in not_found)} (NOTE: if you "
                 "wanted to run a preprocess step, remember to pass "
-                "postproc_setup=True in the input settings node)".format(
-                    len(not_found), ', '.join(str(nf) for nf in not_found)
-                )
+                "postproc_setup=True in the input settings node)"
             )
 
         for pattern in optional_file_globs:
             matched_files = fnmatch.filter(local_folder_content, pattern)
             local_folder_content -= set(matched_files)
             local_copy_list.extend(
                 _get_local_file_info(filename) for filename in matched_files
             )
 
         return _InputFileLists(
-            local_copy_list=local_copy_list,
-            remote_copy_list=[],
-            remote_symlink_list=[]
+            local_copy_list=local_copy_list, remote_copy_list=[], remote_symlink_list=[]
         )
```

### Comparing `aiida-wannier90-2.0.1/aiida_wannier90/utils.py` & `aiida_wannier90-2.1.0/src/aiida_wannier90/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,101 +1,89 @@
-# -*- coding: utf-8 -*-
 ################################################################################
 # Copyright (c), AiiDA team and individual contributors.                       #
 #  All rights reserved.                                                        #
 # This file is part of the AiiDA-wannier90 code.                               #
 #                                                                              #
 # The code is hosted on GitHub at https://github.com/aiidateam/aiida-wannier90 #
 # For further information on the license, see the LICENSE.txt file             #
 ################################################################################
-from __future__ import absolute_import
+"""Utilities."""
 import numbers
 
-import six
+__all__ = ("plot_centres_xsf", "conv_to_fortran", "conv_to_fortran_withlists")
 
-__all__ = ('plot_centres_xsf', 'conv_to_fortran', 'conv_to_fortran_withlists')
 
-
-def plot_centres_xsf(structure, w90_calc, filename='./wannier.xsf'):
-    """
-    Plots Wannier function centres in .xsf format
-    """
+def plot_centres_xsf(structure, w90_calc, filename="./wannier.xsf"):
+    """Plot Wannier function centres in .xsf format."""
     # Disabling the import-error since this is an optional requirement
-    import ase  # pylint: disable=import-error
+    import ase  # pylint: disable=import-error,useless-suppression
 
     a = structure.get_ase()
     new_a = a.copy()
-    out = w90_calc.out.output_parameters.get_dict()['wannier_functions_output']
-    coords = [i['wf_centres'] for i in out]
+    out = w90_calc.out.output_parameters.get_dict()["wannier_functions_output"]
+    coords = [i["wf_centres"] for i in out]
     for c in coords:
-        new_a.append(ase.Atom('X', c))
+        new_a.append(ase.Atom("X", c))
     new_a.write(filename)
 
 
 def conv_to_fortran(val, quote_strings=True):
-    """
-    :param val: the value to be read and converted to a Fortran-friendly string.
-    """
+    """Convert the input ``val`` to a Fortran-friendly string."""
     # Note that bool should come before integer, because a boolean matches also
     # isinstance(...,int)
     import numpy
 
     if isinstance(val, (bool, numpy.bool_)):
         if val:
-            val_str = '.true.'
+            val_str = ".true."
         else:
-            val_str = '.false.'
+            val_str = ".false."
     elif isinstance(val, numbers.Integral):
-        val_str = "{:d}".format(val)
+        val_str = f"{val:d}"
     elif isinstance(val, numbers.Real):
-        val_str = ("{:18.10e}".format(val)).replace('e', 'd')
-    elif isinstance(val, six.string_types):
+        val_str = (f"{val:18.10e}").replace("e", "d")
+    elif isinstance(val, str):
         if quote_strings:
-            val_str = "'{!s}'".format(val)
+            val_str = f"'{val!s}'"
         else:
-            val_str = "{!s}".format(val)
+            val_str = f"{val!s}"
     else:
         raise ValueError(
-            "Invalid value '{}' of type '{}' passed, accepts only bools, ints, floats and strings"
-            .format(val, type(val))
+            f"Invalid value '{val}' of type '{type(val)}' passed, accepts only bools, ints, floats and strings"
         )
 
     return val_str
 
 
 def conv_to_fortran_withlists(val, quote_strings=True):
-    """
-    Same as conv_to_fortran but with extra logic to handle lists
-    :param val: the value to be read and converted to a Fortran-friendly string.
-    """
+    """Convert to Fortran, same as conv_to_fortran but with extra logic to handle lists."""
     # pylint: disable=too-many-return-statements
 
     # Note that bool should come before integer, because a boolean matches also
     # isinstance(...,int)
     if isinstance(val, (list, tuple)):
         val_str = ", ".join(
-            conv_to_fortran(thing, quote_strings=quote_strings)
-            for thing in val
+            conv_to_fortran(thing, quote_strings=quote_strings) for thing in val
         )
         return val_str
 
     if isinstance(val, bool):
         if val:
-            return '.true.'
+            return ".true."
 
-        return '.false.'
+        return ".false."
 
-    if isinstance(val, six.integer_types):
-        return "{:d}".format(val)
+    if isinstance(val, int):
+        return f"{val:d}"
 
     if isinstance(val, float):
-        return "{:18.10e}".format(val).replace('e', 'd')
+        return f"{val:18.10e}".replace("e", "d")
 
-    if isinstance(val, six.string_types):
+    if isinstance(val, str):
         if quote_strings:
-            return "'{!s}'".format(val)
+            return f"'{val!s}'"
 
-        return "{!s}".format(val)
+        return f"{val!s}"
 
     raise ValueError(
         "Invalid value passed, accepts only bools, ints, floats and strings"
     )
```

