# Comparing `tmp/langful-0.23-py2.py3-none-any.whl.zip` & `tmp/langful-0.24-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 7310 bytes, number of entries: 9
+Zip file size: 7703 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat     1507 b- defN 23-Apr-15 03:44 langful/__init__.py
--rw-rw-rw-  2.0 fat      340 b- defN 23-Apr-15 04:33 langful/define.py
+-rw-rw-rw-  2.0 fat      478 b- defN 23-Apr-16 03:28 langful/define.py
 -rw-rw-rw-  2.0 fat     1590 b- defN 23-Apr-15 03:46 langful/function.py
--rw-rw-rw-  2.0 fat    11341 b- defN 23-Apr-15 05:31 langful/lang.py
--rw-rw-rw-  2.0 fat     1064 b- defN 23-Apr-15 05:32 langful-0.23.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2603 b- defN 23-Apr-15 05:32 langful-0.23.dist-info/METADATA
--rw-rw-rw-  2.0 fat      110 b- defN 23-Apr-15 05:32 langful-0.23.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-15 05:32 langful-0.23.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      679 b- defN 23-Apr-15 05:32 langful-0.23.dist-info/RECORD
-9 files, 19242 bytes uncompressed, 6156 bytes compressed:  68.0%
+-rw-rw-rw-  2.0 fat    13440 b- defN 23-Apr-16 05:05 langful/lang.py
+-rw-rw-rw-  2.0 fat     1064 b- defN 23-Apr-16 05:06 langful-0.24.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2603 b- defN 23-Apr-16 05:06 langful-0.24.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      110 b- defN 23-Apr-16 05:06 langful-0.24.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Apr-16 05:06 langful-0.24.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      679 b- defN 23-Apr-16 05:06 langful-0.24.dist-info/RECORD
+9 files, 21479 bytes uncompressed, 6549 bytes compressed:  69.5%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: langful/function.py
 Comment: 
 
 Filename: langful/lang.py
 Comment: 
 
-Filename: langful-0.23.dist-info/LICENSE
+Filename: langful-0.24.dist-info/LICENSE
 Comment: 
 
-Filename: langful-0.23.dist-info/METADATA
+Filename: langful-0.24.dist-info/METADATA
 Comment: 
 
-Filename: langful-0.23.dist-info/WHEEL
+Filename: langful-0.24.dist-info/WHEEL
 Comment: 
 
-Filename: langful-0.23.dist-info/top_level.txt
+Filename: langful-0.24.dist-info/top_level.txt
 Comment: 
 
-Filename: langful-0.23.dist-info/RECORD
+Filename: langful-0.24.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## langful/define.py

```diff
@@ -7,14 +7,20 @@
 LANG = "lang"
 
 FILE = "file"
 DICT = "dict"
 # encode/decode
 UTF8 = "utf-8"
 
+def join( args : list ) -> str :
+    return "".join( args )
+
+def range_len( obj ) -> list :
+    return list( range( len( obj ) ) )
+
 def get_type( obj ) -> str :
     if isinstance( obj , str ) :
         return FILE
     elif isinstance( obj , dict ) :
         return DICT
     else :
         raise TypeError(f"can't use type { type( obj ) }")
```

## langful/lang.py

```diff
@@ -56,28 +56,28 @@
             lang_file_list = []
             language_dict = {}
             use_locale = default_locale
             if not os.path.exists( lang_file ) : # 若默认语言不存在对应的本地化 那么就选用默认语言文件
                 use_locale = default_lang
                 lang_file = default_lang + file_suffix
 
-            for filename in os.listdir(lang_dir): # 尝试加载所有能加载的模块
+            for filename in os.listdir( lang_dir ): # 尝试加载所有能加载的模块
                 if len( filename ) > file_suffix_len and filename[ -file_suffix_len: ] == file_suffix :
                     try :
                         with open( os.path.join( lang_dir , filename ) , encoding = UTF8 ) as file :
                             if file_type == JSON :
                                 l = json.load( file ) # 直接加载JSON文件
                             elif file_type == LANG :
                                 l = {}
                                 for i in file.read().split( "\n" ) : # 去换行
                                     if i :
                                         k , v = i.split( "=" ) # 键 = 值
                                         if v and v[0] == " " : # 去空格
                                             v = v[ 1: ]
-                                        l[ "".join( k.split() ) ] = v
+                                        l[ join( k.split() ) ] = v
                             else :
                                 raise TypeError( f"can't use type '{file_type}'" )
                         language_dict[ filename[ :-file_suffix_len ] ] = l # 加载文件
                         lang_file_list.append( filename )
                     except Exception as e :
                         print( f"{e}\n" )
                         traceback.print_exc()
@@ -145,20 +145,28 @@
             lang_str = self.use_locale
         if lang_str in self.lang_str_list :
             return self.language_dict[ lang_str ]
         else :
             raise KeyError( f"lang '{lang_str}' has not find!" )
 
     def save( self ) -> None :
+        """
+        # save
+        to save all lang file
+
+        ---
+
+        保存所有lang文件
+        """
         if self.type == FILE :
             for k , v in self.language_dict.items() :
                 try :
                     with open( os.path.join( self.lang_dir , k + self.file_suffix ) , "w+" , encoding = UTF8 ) as file :
                         if self.file_type == JSON :
-                            file.write( json.dumps( v , indent=4 , ensure_ascii = False ) )
+                            file.write( json.dumps( v , indent = 4 , separators = ( " ," , ": " ) , ensure_ascii = False ) )
                         elif self.file_type == LANG :
                             for i_k , i_v in v.items() :
                                 s = f"{i_k} = {i_v}\n"
                                 file.write( s )
                 except Exception as e :
                     print( f"{e}\n" )
                     traceback.print_exc()
@@ -285,22 +293,85 @@
             raise RuntimeError( f"can't remove '{lang_str}' " )
         del self.language_dict[ lang_str ]
         del self.lang_str_list[ self.lang_str_list.index( lang_str ) ]
         if self.type == FILE and change_file :
             self.save()
         self._reload()
 
-    def replace( self , * args : str , lang_str : str = None , change : str = None ) -> str : # 替换字符串 使用%号
+    def replace( self , key : str = None , args = None , lang_str : str = None , change : str = None ) -> str :
         """
+        # replace
 
-        Replace string with some one dictionary
+        Replace language dictionary one key with list/string
 
-        用某个字典替换字符串
+        用 列表/字符串 替换语言字典中的某个键
 
-        # replace
+        ---
+
+        key: dictionary's key
+
+        args: list
+
+        lang_str: Such as 'zh_cn' or 'en_us' and more
+
+        change: Specifies what character to use for substitution , default is '%'
+
+        ---
+
+        key: 键值
+
+        args: 列表
+
+        lang_str: 例如 'zh_cn' 或 'en_us' 等等
+
+        change: 选择用什么符号做替换 默认为'%'
+        """
+        if not change :
+            change = self.change
+
+        language = self._lang_str_to_language( lang_str )
+
+        if ( not key ) or ( key not in language ) :
+            raise KeyError( f"can't use key '{key}'" )
+
+        if not ( isinstance( args , str ) or isinstance( args , list ) ) :
+            raise TypeError( f"args can't use '{ type( args ) }' type" )
+
+        text = self.get( key , lang_str ).split( change )
+        if len( text ) == 1 :
+            text = text[0]
+        ret = ""
+
+        for i in range_len( text ) :
+            if isinstance( text , str ) :
+                ret += text[i]
+            else :
+                if isinstance( args , list ) :
+                    if ( len( text ) - 1 ) > i :
+                        if len( args ) > i :
+                            ret += text[i] + args[i]
+                        else :
+                            ret += text[i] + args[-1]
+                    else :
+                        ret += text[i]
+                elif isinstance( args , str ) :
+                    if ( len( text ) - 1 ) > i :
+                        ret += text[i] + args
+                    else :
+                        ret += text[i]
+
+        return ret
+
+    def str_replace( self , * args : str , lang_str : str = None , change : str = None ) -> str : # 替换字符串 使用%号
+        """
+        # str_replace
+
+        Replace string with some one language dictionary
+
+        用某个语言字典替换字符串
 
         ---
 
         key: The dictionary's key
 
         args: Strings
 
@@ -318,24 +389,24 @@
 
         change: 选择用什么符号做替换 默认为'%'
         """
         if not change :
             change = self.change
 
         i = 0
-        Ret = ""
-        text = "".join( args ).split( change )
+        ret = ""
+        text = join( args ).split( change )
         language = self._lang_str_to_language( lang_str )
 
         for I in text :
             if i % 2 :
                 if I in language :
-                    Ret += language[I]
+                    ret += language[I]
                 elif not I :
-                    Ret += change
+                    ret += change
                 else :
                     raise KeyError( f"key '{I}' has not find!" )
             else :
-                Ret += I
+                ret += I
             i += 1
 
-        return Ret
+        return ret
```

## Comparing `langful-0.23.dist-info/LICENSE` & `langful-0.24.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `langful-0.23.dist-info/METADATA` & `langful-0.24.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langful
-Version: 0.23
+Version: 0.24
 Home-page: https://github.com/cueavyqwp/langful
 Author: cueavyqwp
 Author-email: cueavyqwp@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: > 3.6
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: langful Version: 0.23 Home-page: https://
+Metadata-Version: 2.1 Name: langful Version: 0.24 Home-page: https://
 github.com/cueavyqwp/langful Author: cueavyqwp Author-email:
 cueavyqwp@outlook.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Requires-Python: > 3.6 Description-Content-Type: text/
 markdown License-File: LICENSE # langful
    [PyPI_version] [Python_version] [license] [Github_stars] [Github_issues]
 # install Use `pip` to install `pip install langful` or `pip3 install langful`
```

