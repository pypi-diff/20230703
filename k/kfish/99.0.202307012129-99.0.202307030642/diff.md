# Comparing `tmp/kfish-99.0.202307012129-py3-none-any.whl.zip` & `tmp/kfish-99.0.202307030642-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 7255 bytes, number of entries: 6
--rw-r--r--  2.0 unx     8477 b- defN 23-Jul-01 21:25 kfish/__init__.py
--rw-r--r--  2.0 unx    11358 b- defN 23-Jul-01 21:29 kfish-99.0.202307012129.dist-info/LICENSE
--rw-r--r--  2.0 unx      302 b- defN 23-Jul-01 21:29 kfish-99.0.202307012129.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-01 21:29 kfish-99.0.202307012129.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-Jul-01 21:29 kfish-99.0.202307012129.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      509 b- defN 23-Jul-01 21:29 kfish-99.0.202307012129.dist-info/RECORD
-6 files, 20744 bytes uncompressed, 6325 bytes compressed:  69.5%
+Zip file size: 7263 bytes, number of entries: 6
+-rw-r--r--  2.0 unx     8542 b- defN 23-Jul-03 06:35 kfish/__init__.py
+-rw-r--r--  2.0 unx    11358 b- defN 23-Jul-03 06:42 kfish-99.0.202307030642.dist-info/LICENSE
+-rw-r--r--  2.0 unx      302 b- defN 23-Jul-03 06:42 kfish-99.0.202307030642.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-03 06:42 kfish-99.0.202307030642.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-Jul-03 06:42 kfish-99.0.202307030642.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      509 b- defN 23-Jul-03 06:42 kfish-99.0.202307030642.dist-info/RECORD
+6 files, 20809 bytes uncompressed, 6333 bytes compressed:  69.6%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: kfish/__init__.py
 Comment: 
 
-Filename: kfish-99.0.202307012129.dist-info/LICENSE
+Filename: kfish-99.0.202307030642.dist-info/LICENSE
 Comment: 
 
-Filename: kfish-99.0.202307012129.dist-info/METADATA
+Filename: kfish-99.0.202307030642.dist-info/METADATA
 Comment: 
 
-Filename: kfish-99.0.202307012129.dist-info/WHEEL
+Filename: kfish-99.0.202307030642.dist-info/WHEEL
 Comment: 
 
-Filename: kfish-99.0.202307012129.dist-info/top_level.txt
+Filename: kfish-99.0.202307030642.dist-info/top_level.txt
 Comment: 
 
-Filename: kfish-99.0.202307012129.dist-info/RECORD
+Filename: kfish-99.0.202307030642.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kfish/__init__.py

```diff
@@ -186,9 +186,12 @@
 
     def set_iso(self, iso_url):
         try:
             self.eject_iso()
         except:
             pass
         self.insert_iso(iso_url)
-        self.set_iso_once()
+        try:
+            self.set_iso_once()
+        except:
+            self.set_iso_once()
         self.restart()
```

## Comparing `kfish-99.0.202307012129.dist-info/LICENSE` & `kfish-99.0.202307030642.dist-info/LICENSE`

 * *Files identical despite different names*

