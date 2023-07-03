# Comparing `tmp/mathkit-2.11.2.tar.gz` & `tmp/mathkit-2.15.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathkit-2.11.2.tar", last modified: Mon Jul  3 06:45:58 2023, max compression
+gzip compressed data, was "mathkit-2.15.2.tar", last modified: Mon Jul  3 06:57:50 2023, max compression
```

## Comparing `mathkit-2.11.2.tar` & `mathkit-2.15.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 06:45:58.636412 mathkit-2.11.2/
--rw-rw-rw-   0        0        0     3467 2023-07-03 06:45:58.631393 mathkit-2.11.2/PKG-INFO
--rw-rw-rw-   0        0        0     3021 2023-07-02 02:47:56.000000 mathkit-2.11.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-03 06:45:58.558189 mathkit-2.11.2/mathkit/
--rw-rw-rw-   0        0        0      527 2023-07-03 06:17:43.000000 mathkit-2.11.2/mathkit/__init__.py
--rw-rw-rw-   0        0        0    10019 2023-07-03 06:42:27.000000 mathkit-2.11.2/mathkit/main.py
-drwxrwxrwx   0        0        0        0 2023-07-03 06:45:58.623925 mathkit-2.11.2/mathkit.egg-info/
--rw-rw-rw-   0        0        0     3467 2023-07-03 06:45:58.000000 mathkit-2.11.2/mathkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-07-03 06:45:58.000000 mathkit-2.11.2/mathkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 06:45:58.000000 mathkit-2.11.2/mathkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-03 06:45:58.000000 mathkit-2.11.2/mathkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-03 06:45:58.639954 mathkit-2.11.2/setup.cfg
--rw-rw-rw-   0        0        0      713 2023-07-03 06:45:45.000000 mathkit-2.11.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:57:50.048018 mathkit-2.15.2/
+-rw-rw-rw-   0        0        0     3467 2023-07-03 06:57:50.046967 mathkit-2.15.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3021 2023-07-02 02:47:56.000000 mathkit-2.15.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-03 06:57:50.022351 mathkit-2.15.2/mathkit/
+-rw-rw-rw-   0        0        0      527 2023-07-03 06:17:43.000000 mathkit-2.15.2/mathkit/__init__.py
+-rw-rw-rw-   0        0        0    10036 2023-07-03 06:56:14.000000 mathkit-2.15.2/mathkit/main.py
+drwxrwxrwx   0        0        0        0 2023-07-03 06:57:50.045044 mathkit-2.15.2/mathkit.egg-info/
+-rw-rw-rw-   0        0        0     3467 2023-07-03 06:57:49.000000 mathkit-2.15.2/mathkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-07-03 06:57:49.000000 mathkit-2.15.2/mathkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-03 06:57:49.000000 mathkit-2.15.2/mathkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-03 06:57:49.000000 mathkit-2.15.2/mathkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-03 06:57:50.048018 mathkit-2.15.2/setup.cfg
+-rw-rw-rw-   0        0        0      713 2023-07-03 06:57:44.000000 mathkit-2.15.2/setup.py
```

### Comparing `mathkit-2.11.2/PKG-INFO` & `mathkit-2.15.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathkit
-Version: 2.11.2
+Version: 2.15.2
 Summary: Python library for mathematical functions
 Home-page: https://github.com/theunkownhacker/mathkit
 Author: TheUnkownHacker
 Author-email: theunkownhacker@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mathkit-2.11.2/README.md` & `mathkit-2.15.2/README.md`

 * *Files identical despite different names*

### Comparing `mathkit-2.11.2/mathkit/__init__.py` & `mathkit-2.15.2/mathkit/__init__.py`

 * *Files identical despite different names*

### Comparing `mathkit-2.11.2/mathkit/main.py` & `mathkit-2.15.2/mathkit/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -226,51 +226,56 @@
 
 def percentage(num=None, perc=None):
     """
     Perform percentage calculations and print the result.
 
     Args:
         num (float): The number for percentage calculation (default: None).
-        percentage (float): The percentage value (default: None).
+        perc (float): The percentage value (default: None).
 
     Returns:
         None
 
     """
     print("1. Percentage of a number")
     print("2. Percentage increase")
     print("3. Percentage decrease")
     print("4. Exit")
     choice = int(input("Enter your choice: "))
+
     if choice == 1:
         if num is None:
             num = float(input("Enter the number: "))
-        elif perc is None:
+        if perc is None:
             perc = float(input("Enter the percentage: "))
         if perc is not None and num is not None:
-            print(str(int(perc)) + "% of " + str(int(num)) + " is " + str(int((perc / 100) * num)))
+            result = (perc / 100) * num
+            print(str(perc) + "% of " + str(num) + " is " + str(result))
     elif choice == 2:
         if num is None:
             num = float(input("Enter the number: "))
-        elif perc is None:
+        if perc is None:
             perc = float(input("Enter the percentage: "))
         if perc is not None and num is not None:
-            print(str(int(num)) + " increased by " + str(int(perc)) + "% is " + str(int(num + ((perc / 100) * num))))
+            result = num + (perc / 100) * num
+            print(str(num) + " increased by " + str(perc) + "% is " + str(result))
     elif choice == 3:
         if num is None:
             num = float(input("Enter the number: "))
-        elif perc is None:
+        if perc is None:
             perc = float(input("Enter the percentage: "))
         if perc is not None and num is not None:
-            print(str(int(num)) + " decreased by " + str(int(perc)) + "% is " + str(int(num - ((perc / 100) * num))))
+            result = num - (perc / 100) * num
+            print(str(num) + " decreased by " + str(perc) + "% is " + str(result))
     elif choice == 4:
         sys.exit()
     else:
         print("Invalid choice!")
-        percentage(num, perc)
+
+    percentage()
 
 def power(num=None):
     """
     Calculate the power of a number and print the result.
 
     Args:
         num (int or float): The number (default: None).
```

### Comparing `mathkit-2.11.2/mathkit.egg-info/PKG-INFO` & `mathkit-2.15.2/mathkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathkit
-Version: 2.11.2
+Version: 2.15.2
 Summary: Python library for mathematical functions
 Home-page: https://github.com/theunkownhacker/mathkit
 Author: TheUnkownHacker
 Author-email: theunkownhacker@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mathkit-2.11.2/setup.py` & `mathkit-2.15.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="mathkit",
-    version="2.11.2",
+    version="2.15.2",
     author="TheUnkownHacker",
     author_email="theunkownhacker@gmail.com",
     description="Python library for mathematical functions",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/theunkownhacker/mathkit",
     packages=find_packages(),
```

