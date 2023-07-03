# Comparing `tmp/pfc_geometry-0.1.2.tar.gz` & `tmp/pfc_geometry-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pfc_geometry-0.1.2.tar", last modified: Wed Jun 14 09:35:33 2023, max compression
+gzip compressed data, was "pfc_geometry-0.1.3.tar", last modified: Mon Jul  3 07:12:05 2023, max compression
```

## Comparing `pfc_geometry-0.1.2.tar` & `pfc_geometry-0.1.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 09:35:33.032517 pfc_geometry-0.1.2/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     7632 2023-03-28 15:54:20.000000 pfc_geometry-0.1.2/LICENSE
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1488 2023-06-14 09:35:33.032517 pfc_geometry-0.1.2/PKG-INFO
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1191 2023-03-28 15:54:20.000000 pfc_geometry-0.1.2/README.md
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 09:35:33.028517 pfc_geometry-0.1.2/geometry/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1207 2023-05-29 08:21:19.000000 pfc_geometry-0.1.2/geometry/__init__.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     8875 2023-03-30 11:31:01.000000 pfc_geometry-0.1.2/geometry/base.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     2956 2023-03-28 15:54:20.000000 pfc_geometry-0.1.2/geometry/coordinate_frame.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     3573 2023-03-28 15:54:20.000000 pfc_geometry-0.1.2/geometry/gps.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1271 2023-03-28 15:54:20.000000 pfc_geometry-0.1.2/geometry/mass.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     5150 2023-03-28 15:54:20.000000 pfc_geometry-0.1.2/geometry/point.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     8238 2023-03-28 15:54:20.000000 pfc_geometry-0.1.2/geometry/quaternion.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      375 2023-03-28 15:54:20.000000 pfc_geometry-0.1.2/geometry/testing.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     3870 2023-03-28 15:54:20.000000 pfc_geometry-0.1.2/geometry/transformation.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 09:35:33.028517 pfc_geometry-0.1.2/pfc_geometry.egg-info/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1488 2023-06-14 09:35:32.000000 pfc_geometry-0.1.2/pfc_geometry.egg-info/PKG-INFO
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      548 2023-06-14 09:35:33.000000 pfc_geometry-0.1.2/pfc_geometry.egg-info/SOURCES.txt
--rw-rw-r--   0 td6834    (1001) td6834    (1001)        1 2023-06-14 09:35:32.000000 pfc_geometry-0.1.2/pfc_geometry.egg-info/dependency_links.txt
--rw-rw-r--   0 td6834    (1001) td6834    (1001)       24 2023-06-14 09:35:32.000000 pfc_geometry-0.1.2/pfc_geometry.egg-info/requires.txt
--rw-rw-r--   0 td6834    (1001) td6834    (1001)        9 2023-06-14 09:35:32.000000 pfc_geometry-0.1.2/pfc_geometry.egg-info/top_level.txt
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      404 2023-06-14 09:35:33.032517 pfc_geometry-0.1.2/setup.cfg
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      699 2023-03-28 15:54:20.000000 pfc_geometry-0.1.2/setup.py
-drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-06-14 09:35:33.032517 pfc_geometry-0.1.2/tests/
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     5379 2023-03-28 15:54:20.000000 pfc_geometry-0.1.2/tests/test_base.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)      875 2023-03-28 15:54:20.000000 pfc_geometry-0.1.2/tests/test_coord.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1248 2023-03-28 15:54:20.000000 pfc_geometry-0.1.2/tests/test_gps.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1163 2023-03-28 15:54:20.000000 pfc_geometry-0.1.2/tests/test_mass.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     2578 2023-03-28 15:54:20.000000 pfc_geometry-0.1.2/tests/test_point.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     5642 2023-06-14 09:30:36.000000 pfc_geometry-0.1.2/tests/test_quaternion.py
--rw-rw-r--   0 td6834    (1001) td6834    (1001)     1650 2023-03-28 15:54:20.000000 pfc_geometry-0.1.2/tests/test_transform.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-07-03 07:12:05.082486 pfc_geometry-0.1.3/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     7632 2023-03-28 15:54:20.000000 pfc_geometry-0.1.3/LICENSE
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1488 2023-07-03 07:12:05.086485 pfc_geometry-0.1.3/PKG-INFO
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1191 2023-03-28 15:54:20.000000 pfc_geometry-0.1.3/README.md
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-07-03 07:12:05.082486 pfc_geometry-0.1.3/geometry/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1207 2023-05-29 08:21:19.000000 pfc_geometry-0.1.3/geometry/__init__.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     8875 2023-03-30 11:31:01.000000 pfc_geometry-0.1.3/geometry/base.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     2956 2023-03-28 15:54:20.000000 pfc_geometry-0.1.3/geometry/coordinate_frame.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     3573 2023-03-28 15:54:20.000000 pfc_geometry-0.1.3/geometry/gps.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1271 2023-03-28 15:54:20.000000 pfc_geometry-0.1.3/geometry/mass.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     4915 2023-06-30 05:30:43.000000 pfc_geometry-0.1.3/geometry/point.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     8830 2023-06-30 13:19:15.000000 pfc_geometry-0.1.3/geometry/quaternion.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      375 2023-03-28 15:54:20.000000 pfc_geometry-0.1.3/geometry/testing.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     3870 2023-03-28 15:54:20.000000 pfc_geometry-0.1.3/geometry/transformation.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-07-03 07:12:05.082486 pfc_geometry-0.1.3/pfc_geometry.egg-info/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1488 2023-07-03 07:12:05.000000 pfc_geometry-0.1.3/pfc_geometry.egg-info/PKG-INFO
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      548 2023-07-03 07:12:05.000000 pfc_geometry-0.1.3/pfc_geometry.egg-info/SOURCES.txt
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)        1 2023-07-03 07:12:05.000000 pfc_geometry-0.1.3/pfc_geometry.egg-info/dependency_links.txt
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)       24 2023-07-03 07:12:05.000000 pfc_geometry-0.1.3/pfc_geometry.egg-info/requires.txt
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)        9 2023-07-03 07:12:05.000000 pfc_geometry-0.1.3/pfc_geometry.egg-info/top_level.txt
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      404 2023-07-03 07:12:05.086485 pfc_geometry-0.1.3/setup.cfg
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      699 2023-03-28 15:54:20.000000 pfc_geometry-0.1.3/setup.py
+drwxrwxr-x   0 td6834    (1001) td6834    (1001)        0 2023-07-03 07:12:05.082486 pfc_geometry-0.1.3/tests/
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     5379 2023-03-28 15:54:20.000000 pfc_geometry-0.1.3/tests/test_base.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)      875 2023-03-28 15:54:20.000000 pfc_geometry-0.1.3/tests/test_coord.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1248 2023-03-28 15:54:20.000000 pfc_geometry-0.1.3/tests/test_gps.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1163 2023-03-28 15:54:20.000000 pfc_geometry-0.1.3/tests/test_mass.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     2639 2023-06-30 05:31:54.000000 pfc_geometry-0.1.3/tests/test_point.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     5668 2023-06-30 05:34:46.000000 pfc_geometry-0.1.3/tests/test_quaternion.py
+-rw-rw-r--   0 td6834    (1001) td6834    (1001)     1650 2023-03-28 15:54:20.000000 pfc_geometry-0.1.3/tests/test_transform.py
```

### Comparing `pfc_geometry-0.1.2/LICENSE` & `pfc_geometry-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.1.2/PKG-INFO` & `pfc_geometry-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pfc_geometry
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package for handling 3D geometry with a nice interface
 Home-page: https://github.com/PyFlightCoach/geometry
 Author: Thomas David
 Author-email: thomasdavid0@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pfc_geometry-0.1.2/README.md` & `pfc_geometry-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.1.2/geometry/__init__.py` & `pfc_geometry-0.1.3/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.1.2/geometry/base.py` & `pfc_geometry-0.1.3/geometry/base.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.1.2/geometry/coordinate_frame.py` & `pfc_geometry-0.1.3/geometry/coordinate_frame.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.1.2/geometry/gps.py` & `pfc_geometry-0.1.3/geometry/gps.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.1.2/geometry/mass.py` & `pfc_geometry-0.1.3/geometry/mass.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.1.2/geometry/point.py` & `pfc_geometry-0.1.3/geometry/point.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,37 +5,36 @@
 version.
 This program is distributed in the hope that it will be useful, but WITHOUT
 ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 You should have received a copy of the GNU General Public License along with
 this program. If not, see <http://www.gnu.org/licenses/>.
 """
+from __future__ import annotations
 from .base import Base
 import numpy as np
 import pandas as pd
 from typing import List 
 from warnings import warn
 
 
 class Point(Base):
     cols=["x", "y", "z"]
     from_np = [
         "sin","cos","tan",
         "arcsin","arccos","arctan",
     ]
 
-    def scale(self, value):
-        a, b=value, abs(self)
-        res = a/b
-        res[b==0] = 0
-        res = self * res
+    def scale(self, value) -> Point:
+        with np.errstate(divide="ignore"):
+            res = value/abs(self)
+        res[res==np.inf] = 0
+        return self * res
         
-        return res
-        
-    def unit(self):
+    def unit(self) -> Point:
         return self.scale(1)
 
     def remove_outliers(self, nstds = 2):
         ab = abs(self)
         std = np.nanstd(ab)
         mean = np.nanmean(ab)
 
@@ -137,39 +136,30 @@
 @ppmeth
 def cross(a, b) -> Point:
     return Point(np.cross(a.data, b.data))
  
 
 @ppmeth
 def cos_angle_between(a: Point, b: Point) -> np.ndarray:
-    if a == 0 or b == 0:
-        raise ValueError("cannot measure the angle to a zero length vector")
     return a.unit().dot(b.unit())
 
-
 @ppmeth
 def angle_between(a: Point, b: Point) -> np.ndarray:
     return np.arccos(a.cos_angle_between(b))
 
 @ppmeth
 def scalar_projection(a: Point, b: Point) -> Point:
-    if a==0 or b==0:
-        return 0
     return a.cos_angle_between(b) * abs(a)
 
 @ppmeth
 def vector_projection(a: Point, b: Point) -> Point:
-    if abs(a) == 0:
-        return Point.zeros()
     return b.scale(a.scalar_projection(b))
 
 @ppmeth
 def is_parallel(a: Point, b: Point, tolerance=1e-6):
-    if a.unit() == b.unit():
-        return True
     return abs(a.cos_angle_between(b) - 1) < tolerance
 
 @ppmeth
 def is_perpendicular(a: Point, b: Point, tolerance=1e-6):
     return abs(a.dot(b)) < tolerance
 
 @ppmeth
@@ -178,16 +168,14 @@
     return min(angle, np.pi - angle)
 
 @ppmeth
 def angle_between(a: Point, b: Point) -> float: 
     return np.arccos(cos_angle_between(a, b))
 
 def arbitrary_perpendicular(v: Point) -> Point:
-    if v.x == 0 and v.y == 0:
-        return Point(0, 1, 0)
-    return Point(-v.y, v.x, 0).unit
+    return Point(-v.y, v.x, 0).unit()
 
 def vector_norm(point: Point):
     return abs(point)
 
 def normalize_vector(point: Point):
     return point / abs(point)
```

### Comparing `pfc_geometry-0.1.2/geometry/quaternion.py` & `pfc_geometry-0.1.3/geometry/quaternion.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,43 +5,44 @@
 version.
 This program is distributed in the hope that it will be useful, but WITHOUT
 ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 You should have received a copy of the GNU General Public License along with
 this program. If not, see <http://www.gnu.org/licenses/>.
 """
-from .point import Point
+from __future__ import annotations
+from .point import Point, P0
 from .base import Base
 from geometry import PZ
 from typing import Union, Tuple
 import numpy as np
 from warnings import warn
 from numbers import Number
 
 
 
 class Quaternion(Base):
     cols=["w", "x", "y", "z"]
 
     @staticmethod
-    def zero(count=1):
+    def zero(count=1) -> Quaternion:
         return Quaternion(np.tile([1,0,0,0], (count,1)))
 
     @property
     def xyzw(self):
         return np.array([self.x, self.y, self.z, self.w]).T
 
     @property
-    def axis(self):
+    def axis(self) -> Point:
         return Point(self.data[:,1:])
 
-    def norm(self):
+    def norm(self) -> Quaternion:
         return self / abs(self)
 
-    def conjugate(self):
+    def conjugate(self) -> Quaternion:
         return Quaternion(self.w, -self.x, -self.y, -self.z)
 
     def inverse(self):
         return self.conjugate().norm()
 
     def __mul__(self, other):
         if isinstance(other, Quaternion):
@@ -49,32 +50,32 @@
             w = a.w * b.w - a.axis.dot(b.axis)
             xyz = a.w * b.axis + b.w * a.axis + a.axis.cross(b.axis)
             return Quaternion(np.column_stack([w, xyz.data]))
 
         elif isinstance(other, Number):
             return Quaternion(self.data * other)
         elif isinstance(other, np.ndarray):
-            return Quaternions(self.data * self._dprep(other))
+            return Quaternion(self.data * self._dprep(other))
                         
         raise TypeError(f"cant multiply a quaternion by a {other.__class__.__name__}")
 
     def __rmul__(self, other):
         #either it should have been picked up by the left hand object or it should commute
         return self * other   
 
-    def transform_point(self, point: Point):
+    def transform_point(self, point: Point) -> Point:
         '''Transform a point by the rotation described by self'''
         a, b = Base.length_check(self, point)
         
         qdata = np.column_stack((np.zeros(len(a)), b.data))
 
         return (a * Quaternion(qdata) * a.inverse()).axis
   
     @staticmethod
-    def from_euler(eul: Point):
+    def from_euler(eul: Point) -> Quaternion:
         eul = Point.type_check(eul)
         # xyz-fixed Euler angle convention: matches ArduPilot AP_Math/Quaternion::from_euler
         half = eul * 0.5
         c = half.cos
         s = half.sin
 
         return Quaternion(
@@ -82,15 +83,15 @@
                 c.y * c.z * c.x + s.y * s.z * s.x,
                 c.y * c.z * s.x - s.y * s.z * c.x,
                 s.y * c.z * c.x + c.y * s.z * s.x,
                 c.y * s.z * c.x - s.y * c.z * s.x
             ]).T
         )
 
-    def to_euler(self):
+    def to_euler(self) -> Point:
         
         # roll (x-axis rotation)
         sinr_cosp = 2 * (self.w * self.x + self.y * self.z)
         cosr_cosp = 1 - 2 * (self.x * self.x + self.y * self.y)
         roll = np.arctan2(sinr_cosp, cosr_cosp)
 
         # pitch (y-axis rotation)
@@ -107,15 +108,15 @@
             pitch[test] = np.copysign(np.pi / 2, sinp[test])
             yaw[test] = np.zeros(len(sinp[test]))
 
             roll[test] = 2* np.arctan2(self.x[test],self.w[test])
         return Point(roll, pitch, yaw)
 
     @staticmethod
-    def from_axis_angle(axangles: Point):
+    def from_axis_angle(axangles: Point) -> Quaternion:
         small = 1e-6
         angles = abs(axangles)
 
         qdat = np.tile(np.array([1.0, 0.0, 0.0, 0.0]), (len(angles), 1))
 
         if angles.any() >= small:
             baxangles = Point(axangles.data[angles >= small])
@@ -129,35 +130,47 @@
                 c, axis.x * s, axis.y * s, axis.z * s
             ]).T
 
         #qdat[abs(Quaternions(qdat)) < .001] = np.array([[1, 0, 0, 0]])
         return Quaternion(qdat)
 
     def to_axis_angle(self):
+        a = (-self)._to_axis_angle()
+        b = self._to_axis_angle()
+
+        res = a.data
+        res[abs(a)>abs(b), :] = -b.data[abs(a)>abs(b), :]
+
+        return Point(res)
+
+    def _to_axis_angle(self) -> Point:
         """to a point of axis angles. must be normalized first."""
         angle = 2 * np.arccos(self.w)
         s = np.sqrt(1 - self.w**2)
         np.array(s)[np.array(s) < 1e-6] = 1.0
-        return self.axis * angle / s
-
+        with np.errstate(divide="ignore"):
+            sangle = angle / s
+            sangle[sangle==np.inf] = 0
+        res = self.axis * sangle
+        return res
 
     @staticmethod
-    def axis_rates(q, qdot) -> Point:
+    def axis_rates(q: Quaternion, qdot: Quaternion) -> Point:
         wdash = qdot * q.conjugate()
         return wdash.norm().to_axis_angle() 
 
     @staticmethod
-    def body_axis_rates(q, qdot) -> Point:
+    def body_axis_rates(q: Quaternion, qdot: Quaternion) -> Point:
         wdash = q.conjugate() * qdot
         return wdash.norm().to_axis_angle() 
 
-    def rotate(self, rate: Point):
+    def rotate(self, rate: Point) -> Quaternion:
         return (Quaternion.from_axis_angle(rate) * self).norm()
 
-    def body_rotate(self, rate: Point):
+    def body_rotate(self, rate: Point) -> Quaternion:
         return (self * Quaternion.from_axis_angle(rate)).norm()
 
     def diff(self, dt: np.array) -> Point:
         """differentiate in the world frame"""
         assert len(dt) == len(self)
         dt = dt * len(dt) / (len(dt) - 1)
 
@@ -189,15 +202,15 @@
         return np.array([
             [1 - 2 * (y2 + z2), 2 * x * y - 2 * s * z, 2 * s * y + 2 * x * z],
             [2 * x * y + 2 * s * z, 1 - 2 * (x2 + z2), -2 * s * x + 2 * y * z],
             [-2 * s * y + 2 * x * z, 2 * s * x + 2 * y * z, 1 - 2 * (x2 + y2)]
         ]).T
 
     @staticmethod
-    def from_rotation_matrix(matrix: np.ndarray):
+    def from_rotation_matrix(matrix: np.ndarray) -> Quaternion:
         # This method assumes row-vector and postmultiplication of that vector
         m = matrix.conj().transpose()
         if m[2, 2] < 0:
             if m[0, 0] > m[1, 1]:
                 t = 1 + m[0, 0] - m[1, 1] - m[2, 2]
                 q = [m[1, 2] - m[2, 1], t, m[0, 1] + m[1, 0], m[2, 0] + m[0, 2]]
             else:
@@ -216,20 +229,20 @@
         q = np.array(q).astype('float64')
         q *= 0.5 / np.sqrt(t)
         return Quaternion(*q)
 
     def __str__(self):
         return "W:{w:.2f}\nX:{x:.2f}\nY:{y:.2f}\nZ:{z:.2f}".format(w=self.w, x=self.x, y=self.y, z=self.z)
 
-    def closest_principal(self):
+    def closest_principal(self) -> Quaternion:
         eul = self.to_euler()
         rads = eul * (2 / np.pi)
         return Quaternion.from_euler(rads.round(0) * np.pi/2)
 
-    def is_inverted(self):
+    def is_inverted(self) -> bool:
         # does the rotation reverse the Z axis?
         return np.sign(self.transform_point(PZ()).z) > 0
 
 
 
 def Q0(count=1):
     return Quaternion.zero(count)
```

### Comparing `pfc_geometry-0.1.2/geometry/transformation.py` & `pfc_geometry-0.1.3/geometry/transformation.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.1.2/pfc_geometry.egg-info/PKG-INFO` & `pfc_geometry-0.1.3/pfc_geometry.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pfc-geometry
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package for handling 3D geometry with a nice interface
 Home-page: https://github.com/PyFlightCoach/geometry
 Author: Thomas David
 Author-email: thomasdavid0@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pfc_geometry-0.1.2/pfc_geometry.egg-info/SOURCES.txt` & `pfc_geometry-0.1.3/pfc_geometry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.1.2/setup.py` & `pfc_geometry-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.1.2/tests/test_base.py` & `pfc_geometry-0.1.3/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.1.2/tests/test_coord.py` & `pfc_geometry-0.1.3/tests/test_coord.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.1.2/tests/test_gps.py` & `pfc_geometry-0.1.3/tests/test_gps.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.1.2/tests/test_mass.py` & `pfc_geometry-0.1.3/tests/test_mass.py`

 * *Files identical despite different names*

### Comparing `pfc_geometry-0.1.2/tests/test_point.py` & `pfc_geometry-0.1.3/tests/test_point.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,23 +31,25 @@
     np.testing.assert_array_almost_equal(c.data, c_check)
 
 
 def test_scale():
     assert Point(1,0,0).scale(5) == Point(5,0,0)
     assert Point(1,0,0).scale(5).data.shape == Point(5,0,0).data.shape
 
-    assert P0().scale(5) == P0()
+    with np.errstate(divide="raise"):
+        assert Point.concatenate([PX(1,10), P0(10)]).scale(5) == Point.concatenate([PX(5,10), P0(10)])
+
 
 def test_unit():
     assert Point(5,0,0).unit() == Point(1,0,0)
     assert Point(5,0,0).unit().data.shape == (1,3)
 
 def test_angle_between():
-    with raises(ValueError):
-        Point(1,2,3).cos_angle_between(Point.zeros())
+    #with raises(ValueError):
+    Point(1,2,3).cos_angle_between(Point.zeros()) == P0()
 
     assert PX().cos_angle_between(PY()) == 0
 
     assert PX().angle_between(PY()) == np.pi / 2
 
     
     assert PX(-1).angle_between(Point(1,1,0)) == 3 * np.pi / 4
@@ -55,20 +57,14 @@
 
 def test_is_parallel():
     assert not Point(1,0, 0).is_parallel(Point(-1,0, 0))
     assert Point(1,0, 0).is_parallel(Point(1,0, 0))
     assert not Point(1,0, 0).is_parallel(Point(0,1, 0))
 
 
-@mark.skip("this is going to be picked up later with coord and Quaternion stuff")
-def test_rotate():
-    assert PX().rotate(np.identity(3)) == PX()
-
-    assert PX().rotate(np.array([[0, -1, 0], [1, 0, 0], [0, 0, 1]])) == Point(0, 1, 0)
-
 def test_scalar_projection():
     assert Point(1, 1, 0).scalar_projection(PX()) == 1
     assert P0().scalar_projection(Point(1, 1, 0)) == 0
     assert Point(1, 1, 0).scalar_projection(P0()) == 0
 
 def test_is_perpendicular():
     assert is_perpendicular(Point(1, 0, 0), Point(0, 1, 0))
@@ -86,7 +82,15 @@
     
 def test_X():
     assert Point.X(1,100) + Point.Y(1,100) + Point.Z(1,100) == Point(np.ones((100,3)))
 
 
 def test_to_rotation_matrix():
     np.testing.assert_array_equal(P0().to_rotation_matrix()[0],np.identity(3))
+
+
+def test_vector_projection():
+    res = Point.vector_projection(PX(1,20), PY(1))
+    assert res == P0()
+
+    res = Point.vector_projection(PZ(20), PZ(20,20))
+    assert res == PZ(20)
```

### Comparing `pfc_geometry-0.1.2/tests/test_quaternion.py` & `pfc_geometry-0.1.3/tests/test_quaternion.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,16 @@
 
     assert qdot.transform_point(Point(0, 1, 0)).z == np.sin(np.radians(5))
 
 def test_body_rotate_zero():
     qinit = Quaternion.from_euler(Point(0, 0, 0))
     qdot = qinit.body_rotate(Point(0, 0, 0))
 
-    np.testing.assert_array_equal(list(qinit), list(qdot))
+    assert qinit == qdot
+#    np.testing.assert_array_equal(list(qinit), list(qdot))
 
 
 def test_to_from_axis_angle():
     points = Point(np.random.random((100, 3)))
     tqs = Quaternion.from_axis_angle(points)
     tps = tqs.to_axis_angle()
```

### Comparing `pfc_geometry-0.1.2/tests/test_transform.py` & `pfc_geometry-0.1.3/tests/test_transform.py`

 * *Files identical despite different names*

