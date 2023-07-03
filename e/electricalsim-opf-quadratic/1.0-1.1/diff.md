# Comparing `tmp/electricalsim_opf_quadratic-1.0.tar.gz` & `tmp/electricalsim_opf_quadratic-1.1.tar.gz`

## Comparing `electricalsim_opf_quadratic-1.0.tar` & `electricalsim_opf_quadratic-1.1.tar`

### file list

```diff
@@ -1,14 +1,21 @@
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.0/README.md
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.0/src/electricalsim_opf_quadratic/__init__.py
--rw-r--r--   0        0        0    15434 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.0/src/electricalsim_opf_quadratic/extension.py
--rw-r--r--   0        0        0    43294 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.0/src/electricalsim_opf_quadratic/input.ui
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.0/src/electricalsim_opf_quadratic/.idea/electricalsim_opf_quadratic.iml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.0/src/electricalsim_opf_quadratic/.idea/misc.xml
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.0/src/electricalsim_opf_quadratic/.idea/modules.xml
--rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.0/src/electricalsim_opf_quadratic/.idea/workspace.xml
--rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.0/src/electricalsim_opf_quadratic/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.0/src/electricalsim_opf_quadratic/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.0/LICENSE
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.0/README_PyPI.md
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.0/pyproject.toml
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.0/PKG-INFO
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.1/README.md
+-rw-r--r--   0        0        0    10969 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.1/img/EGS_extension_manager.png
+-rw-r--r--   0        0        0   129135 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.1/img/opf_with_EGS.png
+-rw-r--r--   0        0        0   197876 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.1/img/results.png
+-rw-r--r--   0        0        0    64393 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.1/img/tab1.png
+-rw-r--r--   0        0        0    55999 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.1/img/tab2.png
+-rw-r--r--   0        0        0    65976 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.1/img/tab3.png
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.1/src/electricalsim_opf_quadratic/__init__.py
+-rw-r--r--   0        0        0    15434 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.1/src/electricalsim_opf_quadratic/extension.py
+-rw-r--r--   0        0        0    43291 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.1/src/electricalsim_opf_quadratic/input.ui
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.1/src/electricalsim_opf_quadratic/.idea/electricalsim_opf_quadratic.iml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.1/src/electricalsim_opf_quadratic/.idea/misc.xml
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.1/src/electricalsim_opf_quadratic/.idea/modules.xml
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.1/src/electricalsim_opf_quadratic/.idea/workspace.xml
+-rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.1/src/electricalsim_opf_quadratic/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.1/src/electricalsim_opf_quadratic/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.1/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.1/LICENSE
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.1/README_PyPI.md
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.1/pyproject.toml
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 electricalsim_opf_quadratic-1.1/PKG-INFO
```

### Comparing `electricalsim_opf_quadratic-1.0/src/electricalsim_opf_quadratic/extension.py` & `electricalsim_opf_quadratic-1.1/src/electricalsim_opf_quadratic/extension.py`

 * *Files identical despite different names*

### Comparing `electricalsim_opf_quadratic-1.0/src/electricalsim_opf_quadratic/input.ui` & `electricalsim_opf_quadratic-1.1/src/electricalsim_opf_quadratic/input.ui`

 * *Files 0% similar despite different names*

#### Comparing `electricalsim_opf_quadratic-1.0/src/electricalsim_opf_quadratic/input.ui` & `electricalsim_opf_quadratic-1.1/src/electricalsim_opf_quadratic/input.ui`

```diff
@@ -8,21 +8,21 @@
         <y>0</y>
         <width>527</width>
         <height>673</height>
       </rect>
     </property>
     <property name="minimumSize">
       <size>
-        <width>0</width>
+        <width>527</width>
         <height>673</height>
       </size>
     </property>
     <property name="maximumSize">
       <size>
-        <width>16777215</width>
+        <width>527</width>
         <height>673</height>
       </size>
     </property>
     <property name="windowTitle">
       <string>OPF calculation (quadratic costs)</string>
     </property>
     <layout class="QVBoxLayout" name="verticalLayout">
```

### Comparing `electricalsim_opf_quadratic-1.0/src/electricalsim_opf_quadratic/.idea/workspace.xml` & `electricalsim_opf_quadratic-1.1/src/electricalsim_opf_quadratic/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `electricalsim_opf_quadratic-1.0/src/electricalsim_opf_quadratic/.idea/inspectionProfiles/Project_Default.xml` & `electricalsim_opf_quadratic-1.1/src/electricalsim_opf_quadratic/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `electricalsim_opf_quadratic-1.0/LICENSE` & `electricalsim_opf_quadratic-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `electricalsim_opf_quadratic-1.0/pyproject.toml` & `electricalsim_opf_quadratic-1.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "electricalsim_opf_quadratic"
-version = "1.0"
-author = "PhD Ariel S. Loyarte"
+version = "1.1"
+author = "Dr. Ing. Ariel S. Loyarte"
 authors = [
-  { name="PhD Ariel S. Loyarte", email="aloyarte@frsf.utn.edu.ar" },
+  { name="Dr. Ing. Ariel S. Loyarte", email="aloyarte@frsf.utn.edu.ar" },
 ]
-description = "Optimal power flow calculation with quadratic costs for the Electrical Grid Simulator"
+description = "Optimal Power Flow calculation with quadratic costs for the Electrical Grid Simulator (EGS)"
 readme = "README_PyPI.md"
 requires-python = ">=3.8"
 dependencies = [
   "electricalsim>=0.0.7.0",
 ]
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
   "Operating System :: OS Independent",
 ]
 keywords = ["electrical networks", "simulation", "energy", "power systems", "optimal power flow", "Electrical Grid Simulator", "pandapower"]
 license = {text = "MIT"}
 
+[project.urls]
+"Homepage" = "https://github.com/aloytag/electricalsim-opf-quadratic"
+"Bug Tracker" = "https://github.com/aloytag/electricalsim-opf-quadratic/issues"
+"Repository" = "https://github.com/aloytag/electricalsim-opf-quadratic"
 
 [project.entry-points.'electricalsim.extensions']
 opf_quadratic = 'electricalsim_opf_quadratic'
```

