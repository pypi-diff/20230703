# Comparing `tmp/langful-0.30-py2.py3-none-any.whl.zip` & `tmp/langful-0.31-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5422 bytes, number of entries: 7
+Zip file size: 5431 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat      224 b- defN 23-Jun-20 12:20 langful/__init__.py
--rw-rw-rw-  2.0 fat     9667 b- defN 23-Jul-02 03:20 langful/lang.py
--rw-rw-rw-  2.0 fat     1066 b- defN 23-Jul-02 03:32 langful-0.30.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3101 b- defN 23-Jul-02 03:32 langful-0.30.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Jul-02 03:32 langful-0.30.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Jul-02 03:32 langful-0.30.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      528 b- defN 23-Jul-02 03:32 langful-0.30.dist-info/RECORD
-7 files, 14704 bytes uncompressed, 4492 bytes compressed:  69.5%
+-rw-rw-rw-  2.0 fat     9748 b- defN 23-Jul-03 10:08 langful/lang.py
+-rw-rw-rw-  2.0 fat     1066 b- defN 23-Jul-03 10:09 langful-0.31.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3130 b- defN 23-Jul-03 10:09 langful-0.31.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-03 10:09 langful-0.31.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jul-03 10:09 langful-0.31.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      527 b- defN 23-Jul-03 10:09 langful-0.31.dist-info/RECORD
+7 files, 14795 bytes uncompressed, 4501 bytes compressed:  69.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: langful/__init__.py
 Comment: 
 
 Filename: langful/lang.py
 Comment: 
 
-Filename: langful-0.30.dist-info/LICENSE
+Filename: langful-0.31.dist-info/LICENSE
 Comment: 
 
-Filename: langful-0.30.dist-info/METADATA
+Filename: langful-0.31.dist-info/METADATA
 Comment: 
 
-Filename: langful-0.30.dist-info/WHEEL
+Filename: langful-0.31.dist-info/WHEEL
 Comment: 
 
-Filename: langful-0.30.dist-info/top_level.txt
+Filename: langful-0.31.dist-info/top_level.txt
 Comment: 
 
-Filename: langful-0.30.dist-info/RECORD
+Filename: langful-0.31.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## langful/lang.py

```diff
@@ -34,54 +34,55 @@
     return ret
 
 class lang :
     """
     # lang
     """
 
-    def __getitem__( self , key ) -> str :
-        return self.get( key )
-
     def __setitem__( self , key , value ) -> None :
         self.set( key , value )
 
     def __delitem__( self , key ) -> None :
         self.remove( key )
 
+    def __getitem__( self , key ) -> str :
+        return self.get( key )
+
     def __call__( self ) -> None :
         self.init()
 
     def __len__( self ) -> int :
         return len( self.languages )
 
-    def __init__( self , lang_dir : str  |  bool = "lang" , default_locale : str = "en_us" , json_first : bool = True ) -> None :
+    def __init__( self , lang_dir : str | dict | bool = "lang" , default_locale : str = "en_us" , json_first : bool = True ) -> None :
         """
-        lang_dir: lang files dir, if use dict to set that False
+        lang_dir: lang files dir, if use dict to set that to a dictionary or False
         default_locale: default locale
         json_first: is load json file first
         """
-        system_locale = self.get_system_locale
+        system_locale = self.system_locale_get()
         self.default_locale = default_locale
         self.system_locale = system_locale
         self.json_first = json_first
         self.replace_letter = "%"
         self.lang_dir = lang_dir
         self.is_file = False
         self.languages = {}
-        self.locales = []
         self.types = {}
-        self.init()
+        if isinstance( lang_dir , str ) :
+            self.init()
+        elif isinstance( lang_dir , dict ) :
+            self.init_dict( lang_dir )
 
     def init( self ) -> None :
         """
         init by a directory
         """
         path = self.lang_dir
-        if isinstance( path , str ) :
-            self.is_file = True
+        self.is_file = True
         if not isinstance( self.json_first , bool ) :
             self.json_first = True
         if self.json_first :
             loads = [ ".json" , ".lang" ]
         else :
             loads = [ ".lang" , ".json" ]
         if self.is_file :
@@ -98,38 +99,42 @@
                                 data = json.load( file )
                             except json.decoder.JSONDecodeError :
                                 raise SyntaxError( "can't to load .json file" )
                         elif suffix == ".lang" :
                             data = lang_to_json( file.read() )
                         else :
                             continue
-                    self.locales.append( name )
                     self.languages[ name ] = data
                     self.types[ name ] = suffix
 
     def init_dict( self , language : dict ) -> None :
         """
         init by a dictionary, so cant't to save it to the file
         """
         if self.is_file :
             raise TypeError( "can't init by a dictionary, because it's init by a dir" )
         for value in language.values() :
             if not isinstance( value , dict ) :
                 raise TypeError( f"can't use type '{ type( value ) }'" )
         for key in language.keys() :
             self.types[ key ] = ".json"
-            self.locales.append( key )
         self.languages = language
 
-    @property
-    def get_system_locale( self ) -> str :
+    def system_locale_get( self ) -> str :
         """
         get system locale
         """
-        return getdefaultlocale()[0].lower() # 系统语言
+        return getdefaultlocale()[0].lower()
+
+    @property
+    def locales( self ) -> list :
+        """
+        locales
+        """
+        return list( self.types.keys() )
 
     @property
     def locale( self ) -> str :
         """
         choose locale
         """
         if self.system_locale in self.locales :
@@ -163,42 +168,42 @@
     @property
     def type( self ) -> str :
         """
         get type, ".json" or ".lang"
         """
         return self.types[ self.locale ]
 
-    def get_locale( self , locale : str = None ) -> str :
+    def locale_get( self , locale : str = None ) -> str :
         """
         get locale, usually use in function
         """
         if locale :
             return locale
         else :
             return self.locale
 
-    def get_replace_letter( self , replace_letter : str = None ) -> str :
+    def replace_letter_get( self , replace_letter : str = None ) -> str :
         """
         get replace letter, usually use in function
         """
         if replace_letter :
             return replace_letter
         else :
             return self.replace_letter
 
-    def set_locale( self , locale : str = None  ) -> None :
+    def locale_set( self , locale : str = None  ) -> None :
         """
         if give a locale then set that, else reset it
         """
         if locale != None :
             self.system_locale = locale
         else :
-            self.system_locale = self.get_system_locale
+            self.system_locale = self.system_locale_get()
 
-    def lang_set( self , locale : str , suffix : str , value : dict = {} ) -> None :
+    def lang_set( self , locale : str , value : dict = {} , suffix : str = ".json" ) -> None :
         """
         set a new lang
         """
         self.languages[ locale ] = value
         self.types[ locale ] = suffix
 
     def lang_del( self , locale : str ) -> None :
@@ -208,40 +213,39 @@
         del self.languages[ locale ]
         del self.types[ locale ]
 
     def get( self , key : str | int , locale : str = None ) -> str :
         """
         get the key by a locale dictionary
         """
-        locale = self.get_locale( locale )
+        locale = self.locale_get( locale )
         return self.languages[ locale ][ key ]
 
     def set( self , key : str | int , value : str , locale : str = None ) -> None :
         """
         set a value by a locale dictionary
         """
-        locale = self.get_locale( locale )
+        locale = self.locale_get( locale )
         self.languages[ locale ][ key ] = value
 
     def remove( self , key : str | int , locale : str = None ) -> None :
         """
         remove a value by a locale dictionary
         """
-        locale = self.get_locale( locale )
+        locale = self.locale_get( locale )
         del self.languages[ locale ][ key ]
 
     def save( self ) -> None :
         """
         save file when is_file variable is true, else raise the error
         """
         if self.is_file :
             for key , value in self.languages.items() :
                 suffix = self.types[ key ]
-                print(suffix,value)
-                with open( os.path.join( self.lang_dir , key + suffix ) , "w+" , encoding = "utf-8" ) as file :
+                with open( os.path.join( self.lang_dir , key , suffix ) , "w" , encoding = "utf-8" ) as file :
                     if suffix == ".json" :
                         file.write( json.dumps( value , indent = 4 , separators = ( " ," , ": " ) , ensure_ascii = False ) )
                     elif suffix == ".lang" :
                         file.write( json_to_lang( value ) )
         else :
             raise TypeError( "can't to save, because it's not a file" )
 
@@ -254,16 +258,16 @@
         else :
             raise TypeError( "can't to save, because it's not a dict" )
 
     def replace( self , key : str = None , args : list | str = None , locale : str = None , replace_letter : str = None ) -> str :
         """
         replace
         """
-        replace_letter = self.get_replace_letter( replace_letter )
-        locale = self.get_locale( locale )
+        replace_letter = self.replace_letter_get( replace_letter )
+        locale = self.locale_get( locale )
         text = self.get( key , locale ).split( replace_letter )
         if isinstance( args , str ) :
             args = [ args ]
         ret = ""
         p = 0
         for i in text :
             ret += i
@@ -275,16 +279,16 @@
                 p += 1
         return ret
 
     def replace_str( self , text : str , locale : str = None , replace_letter : str = None ) -> str :
         """
         replace by str
         """
-        locale = self.get_locale( locale )
-        replace_letter = self.get_replace_letter( replace_letter )
+        locale = self.locale_get( locale )
+        replace_letter = self.replace_letter_get( replace_letter )
         text = text.split( replace_letter )
         ret = ""
         p = 0
         for i in text :
             if p % 2 :
                 if i :
                     ret += self.get( i )
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## Comparing `langful-0.30.dist-info/LICENSE` & `langful-0.31.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `langful-0.30.dist-info/METADATA` & `langful-0.31.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: langful
-Version: 0.30
-Home-page: https://github.com/cueavyqwp/langful
+Version: 0.31
+Summary: Help to localization
+Home-page: https://github.com/cueavy/langful
 Author: cueavyqwp
 Author-email: cueavyqwp@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: > 3.6
+Requires-Python: >= 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align = "center" >
     <h1>langful</h1>
     <a href = "https://pypi.org/project/langful" >
         <img alt = "PyPI version" src = "https://img.shields.io/pypi/v/langful?color=blue" >
```

