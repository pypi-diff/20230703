# Comparing `tmp/pyzview-1.49.tar.gz` & `tmp/pyzview-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyzview-1.49.tar", last modified: Wed Oct 28 12:57:51 2020, max compression
+gzip compressed data, was "pyzview-1.5.0.tar", last modified: Sun Jul  2 22:43:49 2023, max compression
```

## Comparing `pyzview-1.49.tar` & `pyzview-1.5.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxr-x   0 ohad      (1000) ohad      (1000)        0 2020-10-28 12:57:51.000000 pyzview-1.49/
--rw-r--r--   0 ohad      (1000) ohad      (1000)      623 2020-10-16 09:23:38.000000 pyzview-1.49/README.md
--rw-rw-r--   0 ohad      (1000) ohad      (1000)     1320 2020-10-28 12:57:51.000000 pyzview-1.49/PKG-INFO
--rw-r--r--   0 ohad      (1000) ohad      (1000)      811 2020-10-28 12:57:41.000000 pyzview-1.49/setup.py
-drwxrwxr-x   0 ohad      (1000) ohad      (1000)        0 2020-10-28 12:57:51.000000 pyzview-1.49/test/
--rw-rw-r--   0 ohad      (1000) ohad      (1000)     1403 2020-10-25 15:50:32.000000 pyzview-1.49/test/test_pyzview.py
-drwxrwxr-x   0 ohad      (1000) ohad      (1000)        0 2020-10-28 12:57:51.000000 pyzview-1.49/pyzview.egg-info/
--rw-r--r--   0 ohad      (1000) ohad      (1000)        1 2020-10-28 12:57:51.000000 pyzview-1.49/pyzview.egg-info/dependency_links.txt
--rw-r--r--   0 ohad      (1000) ohad      (1000)     1320 2020-10-28 12:57:51.000000 pyzview-1.49/pyzview.egg-info/PKG-INFO
--rw-r--r--   0 ohad      (1000) ohad      (1000)      224 2020-10-28 12:57:51.000000 pyzview-1.49/pyzview.egg-info/SOURCES.txt
--rw-r--r--   0 ohad      (1000) ohad      (1000)       15 2020-10-28 12:57:51.000000 pyzview-1.49/pyzview.egg-info/top_level.txt
-drwxrwxr-x   0 ohad      (1000) ohad      (1000)        0 2020-10-28 12:57:51.000000 pyzview-1.49/pyzview/
--rw-r--r--   0 ohad      (1000) ohad      (1000)     4765 2020-10-18 22:18:11.000000 pyzview-1.49/pyzview/zview_inf.cpp
--rw-rw-r--   0 ohad      (1000) ohad      (1000)       22 2020-10-06 19:28:04.000000 pyzview-1.49/pyzview/__init__.py
--rw-r--r--   0 ohad      (1000) ohad      (1000)    12469 2020-10-26 21:56:56.000000 pyzview-1.49/pyzview/pyzview.py
--rw-rw-r--   0 ohad      (1000) ohad      (1000)       38 2020-10-28 12:57:51.000000 pyzview-1.49/setup.cfg
+drwxrwxr-x   0 ohad      (1000) ohad      (1000)        0 2023-07-02 22:43:49.430028 pyzview-1.5.0/
+-rw-rw-r--   0 ohad      (1000) ohad      (1000)     1401 2023-07-02 22:43:49.430028 pyzview-1.5.0/PKG-INFO
+-rw-rw-r--   0 ohad      (1000) ohad      (1000)      647 2023-07-02 22:15:47.000000 pyzview-1.5.0/README.md
+drwxrwxr-x   0 ohad      (1000) ohad      (1000)        0 2023-07-02 22:43:49.430028 pyzview-1.5.0/pyzview/
+-rw-rw-r--   0 ohad      (1000) ohad      (1000)       22 2020-10-06 19:28:04.000000 pyzview-1.5.0/pyzview/__init__.py
+-rw-rw-r--   0 ohad      (1000) ohad      (1000)    12606 2023-07-02 22:16:19.000000 pyzview-1.5.0/pyzview/pyzview.py
+-rw-rw-r--   0 ohad      (1000) ohad      (1000)     5534 2023-07-02 22:29:39.000000 pyzview-1.5.0/pyzview/zview_inf.cpp
+drwxrwxr-x   0 ohad      (1000) ohad      (1000)        0 2023-07-02 22:43:49.430028 pyzview-1.5.0/pyzview.egg-info/
+-rw-r--r--   0 ohad      (1000) ohad      (1000)     1401 2023-07-02 22:43:49.000000 pyzview-1.5.0/pyzview.egg-info/PKG-INFO
+-rw-r--r--   0 ohad      (1000) ohad      (1000)      254 2023-07-02 22:43:49.000000 pyzview-1.5.0/pyzview.egg-info/SOURCES.txt
+-rw-r--r--   0 ohad      (1000) ohad      (1000)        1 2023-07-02 22:43:49.000000 pyzview-1.5.0/pyzview.egg-info/dependency_links.txt
+-rw-rw-r--   0 ohad      (1000) ohad      (1000)       14 2023-07-02 22:43:49.000000 pyzview-1.5.0/pyzview.egg-info/requires.txt
+-rw-r--r--   0 ohad      (1000) ohad      (1000)       15 2023-07-02 22:43:49.000000 pyzview-1.5.0/pyzview.egg-info/top_level.txt
+-rw-rw-r--   0 ohad      (1000) ohad      (1000)       38 2023-07-02 22:43:49.430028 pyzview-1.5.0/setup.cfg
+-rw-rw-r--   0 ohad      (1000) ohad      (1000)      992 2023-07-02 22:43:25.000000 pyzview-1.5.0/setup.py
+drwxrwxr-x   0 ohad      (1000) ohad      (1000)        0 2023-07-02 22:43:49.430028 pyzview-1.5.0/test/
+-rw-rw-r--   0 ohad      (1000) ohad      (1000)     1403 2023-07-02 22:09:49.000000 pyzview-1.5.0/test/test_pyzview.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyzview-1.49/README.md` & `pyzview-1.5.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-===========
+
 Pyzview
 ===========
 
 Requirements
 ------------
 
 You'll need to install ziew stanalon app, You can grab it from:
 
 
 ``https://github.com/ohadmen/zview/releases/latest``
 
 Installation
 ------------
     pip install pyzview
+   * pybind 2.2 is required!  
+   
 
 
 Usage example
 -------------
     from pyzview import Pyzview
 
     import numpy as np
```

### Comparing `pyzview-1.49/PKG-INFO` & `pyzview-1.5.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,32 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pyzview
-Version: 1.49
+Version: 1.5.0
 Summary: zview python inferface
 Home-page: https://github.com/ohadmen/pyzview
 Author: Ohad Menashe
 Author-email: ohad.men@gmail.com
 License: UNKNOWN
-Description: ===========
+Description: 
         Pyzview
         ===========
         
         Requirements
         ------------
         
         You'll need to install ziew stanalon app, You can grab it from:
         
         
         ``https://github.com/ohadmen/zview/releases/latest``
         
         Installation
         ------------
             pip install pyzview
+           * pybind 2.2 is required!  
+           
         
         
         Usage example
         -------------
             from pyzview import Pyzview
         
             import numpy as np
@@ -47,7 +49,8 @@
                 
                 k = zv.add_points("demo", pts) if 'k' not in locals() else zv.update_points(k, pts)
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
```

### Comparing `pyzview-1.49/test/test_pyzview.py` & `pyzview-1.5.0/test/test_pyzview.py`

 * *Files identical despite different names*

### Comparing `pyzview-1.49/pyzview.egg-info/PKG-INFO` & `pyzview-1.5.0/pyzview.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,32 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pyzview
-Version: 1.49
+Version: 1.5.0
 Summary: zview python inferface
 Home-page: https://github.com/ohadmen/pyzview
 Author: Ohad Menashe
 Author-email: ohad.men@gmail.com
 License: UNKNOWN
-Description: ===========
+Description: 
         Pyzview
         ===========
         
         Requirements
         ------------
         
         You'll need to install ziew stanalon app, You can grab it from:
         
         
         ``https://github.com/ohadmen/zview/releases/latest``
         
         Installation
         ------------
             pip install pyzview
+           * pybind 2.2 is required!  
+           
         
         
         Usage example
         -------------
             from pyzview import Pyzview
         
             import numpy as np
@@ -47,7 +49,8 @@
                 
                 k = zv.add_points("demo", pts) if 'k' not in locals() else zv.update_points(k, pts)
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
```

### Comparing `pyzview-1.49/pyzview/zview_inf.cpp` & `pyzview-1.5.0/pyzview/zview_inf.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,25 @@
     static T* arr2ptr(const py::array_t<T>& arr)
     {
         py::buffer_info buff = arr.request();
         return static_cast<T*>(buff.ptr);
     }
 
     template<class T>
+    void setZero(const py::array_t<T>& arr)
+    {
+        T* p = arr2ptr(arr);
+        for(ssize_t i{0};i<arr.size();++i)
+        {
+            p[i]=T{0};
+        }
+    }
+
+
+    template<class T>
     size_t getrows(const py::array_t<T>& arr)
     {
         py::buffer_info buff = arr.request();
         return buff.shape[0];
     }
     template<class T>
     size_t getcols(const py::array_t<T>& arr)
@@ -85,15 +96,35 @@
         float* up = arr2ptr(u);
         return m_zvi->setCameraLookAt(ep[0],ep[1],ep[2],cp[0],cp[1],cp[2],up[0],up[1],up[2]);
     }
     int getHandleNumFromString(const char *name)
     {
         return m_zvi->getHandleNumFromString(name);
     }
+    py::array_t<float> getTargetXYZ()
+    {
+        py::array_t<float> xyz(3);
 
+        bool ok = m_zvi->getClickedTarget(arr2ptr(xyz));
+        if(!ok)
+        {
+            setZero(xyz);
+        }
+        return xyz;
+    }
+    py::array_t<std::uint8_t,3> getVersion()
+    {
+        py::array_t<std::uint8_t> ver(3);
+        bool ok = m_zvi->getVersion(arr2ptr(ver));
+        if(!ok)
+        {
+            setZero(ver);
+        }
+        return ver;
+    }
 };
 
 
 
 PYBIND11_MODULE(zview_module, m)
 {
     py::class_<ZviewInfWrapper>(m, "interface")
@@ -107,11 +138,12 @@
         .def("addColoredPoints", &ZviewInfWrapper::addColoredPoints)
         .def("addMesh", &ZviewInfWrapper::addMesh)
         .def("addColoredMesh", &ZviewInfWrapper::addColoredMesh)
         .def("addEdges", &ZviewInfWrapper::addEdges)
         .def("addColoredEdges", &ZviewInfWrapper::addColoredEdges)
         .def("loadFile", &ZviewInfWrapper::loadFile)
         .def("removeShape", &ZviewInfWrapper::removeShape)
-        .def("getHandleNumFromString", &ZviewInfWrapper::getHandleNumFromString);
-
+        .def("getHandleNumFromString", &ZviewInfWrapper::getHandleNumFromString)
+        .def("getTargetXYZ", &ZviewInfWrapper::getTargetXYZ)
+        .def("getVersion", &ZviewInfWrapper::getVersion);
         
-}
+}
```

### Comparing `pyzview-1.49/pyzview/pyzview.py` & `pyzview-1.5.0/pyzview/pyzview.py`

 * *Files 2% similar despite different names*

```diff
@@ -313,7 +313,13 @@
             return namehandle
 
     KEY_ESC = 16777216
     KEY_ENTER = 16777220
 
     def get_last_keystroke(self):
         return self.zv.getLastKeyStroke()
+    
+    def get_target_xyz(self):
+        return self.zv.getTargetXYZ()
+
+    def get_version(self):
+        return self.zv.getVersion()
```

