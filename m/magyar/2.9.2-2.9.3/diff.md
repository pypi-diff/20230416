# Comparing `tmp/magyar-2.9.2.tar.gz` & `tmp/magyar-2.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magyar-2.9.2.tar", last modified: Sun Apr 16 08:55:30 2023, max compression
+gzip compressed data, was "magyar-2.9.3.tar", last modified: Sun Apr 16 15:54:19 2023, max compression
```

## Comparing `magyar-2.9.2.tar` & `magyar-2.9.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-04-16 08:55:30.413411 magyar-2.9.2/
--rw-rw-r--   0 bela      (1000) bela      (1000)     2726 2023-04-16 08:55:30.413411 magyar-2.9.2/PKG-INFO
--rw-rw-r--   0 bela      (1000) bela      (1000)     2355 2023-04-16 08:47:46.000000 magyar-2.9.2/README.md
-drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-04-16 08:55:30.413411 magyar-2.9.2/magyar.egg-info/
--rw-rw-r--   0 bela      (1000) bela      (1000)     2726 2023-04-16 08:55:30.000000 magyar-2.9.2/magyar.egg-info/PKG-INFO
--rw-rw-r--   0 bela      (1000) bela      (1000)      148 2023-04-16 08:55:30.000000 magyar-2.9.2/magyar.egg-info/SOURCES.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)        1 2023-04-16 08:55:30.000000 magyar-2.9.2/magyar.egg-info/dependency_links.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)        7 2023-04-16 08:55:30.000000 magyar-2.9.2/magyar.egg-info/top_level.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)    23049 2023-04-16 08:51:33.000000 magyar-2.9.2/magyar.py
--rw-rw-r--   0 bela      (1000) bela      (1000)       38 2023-04-16 08:55:30.413411 magyar-2.9.2/setup.cfg
--rw-rw-r--   0 bela      (1000) bela      (1000)      588 2023-04-16 08:55:24.000000 magyar-2.9.2/setup.py
+drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-04-16 15:54:19.770351 magyar-2.9.3/
+-rw-rw-r--   0 bela      (1000) bela      (1000)     2925 2023-04-16 15:54:19.770351 magyar-2.9.3/PKG-INFO
+-rw-rw-r--   0 bela      (1000) bela      (1000)     2554 2023-04-16 15:50:54.000000 magyar-2.9.3/README.md
+drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-04-16 15:54:19.770351 magyar-2.9.3/magyar.egg-info/
+-rw-rw-r--   0 bela      (1000) bela      (1000)     2925 2023-04-16 15:54:19.000000 magyar-2.9.3/magyar.egg-info/PKG-INFO
+-rw-rw-r--   0 bela      (1000) bela      (1000)      148 2023-04-16 15:54:19.000000 magyar-2.9.3/magyar.egg-info/SOURCES.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)        1 2023-04-16 15:54:19.000000 magyar-2.9.3/magyar.egg-info/dependency_links.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)        7 2023-04-16 15:54:19.000000 magyar-2.9.3/magyar.egg-info/top_level.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)    28123 2023-04-16 15:46:17.000000 magyar-2.9.3/magyar.py
+-rw-rw-r--   0 bela      (1000) bela      (1000)       38 2023-04-16 15:54:19.770351 magyar-2.9.3/setup.cfg
+-rw-rw-r--   0 bela      (1000) bela      (1000)      588 2023-04-16 15:54:10.000000 magyar-2.9.3/setup.py
```

### Comparing `magyar-2.9.2/PKG-INFO` & `magyar-2.9.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magyar
-Version: 2.9.2
+Version: 2.9.3
 Summary: Hungarian names...
 Home-page: https://github.com/kobanya/nevek
 Author: Nagy Béla
 Author-email: nagy.belabudapest@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -32,14 +32,15 @@
 14. Magyarország halai = magyar.hal
 15. Magyarország madarai = magyar.madar
 
 ## Szótárak  (dictionary): 
 1. Királyok és uralkodásuk ideje  = magyar.kiraly
 2. Vármegyék és azok székhelyei = magyar.megye_szekhely
 3. Járások, székhelyük , megye = magyar.jaras
+4. Villamosvonalak, végállomások, menetidő = magyar.villamos
 
 ## Description
 1. last names =  magyar.vezeteknev
 2. female first names = magyar.keresztnev_n
 3. male first names  = magyar.keresztnev_f
 4. street names = magyar.utca
 5. city names = magyar.telepules
@@ -54,14 +55,15 @@
 14. Fishes of Hungary = magyar.hal
 15. Birds of Hungary = magyar.madar
 
 Dictionary:
 1. Hungarian Kings and Reigns = magyar.kiraly
 2. Hungarian counties and their administrative centers = magyar.megye_szekhely
 3. Hungarian districts, their seats, county = magyar.jaras
+4. Hungarian tram lines  magyar.villamos
 
 ## Listák használat:
 
  Főként véletlengenerátorok kiegészítőjeként ajánlom a listákat
  
 I recommend it mainly as a supplement to random number generators. 
        
@@ -69,22 +71,23 @@
             utca = random.sample(magyar.utca, k=16) 
             random.choices()
             telepulesek = random.choice(magyar.telepules)
 
 ## Szótárak:
 Több adatot tartalmaznak összekapcsolva.
 
-magyar.kiraly tartalma :   {'király neve' : (uralkodása tól, ig)}
-magyar.megye_szekhely :    {'megye neve' : 'székhelye'}
-magyar.jaras :             {'megye' : (székhely, megye)}
+    magyar.kiraly tartalma :   {'király neve' : (uralkodása tól, ig)}
+    magyar.megye_szekhely :    {'megye neve' : 'székhelye'}
+    magyar.jaras :             {'megye' : (székhely, megye)}
+    magyar.villamos:    kulcs {'viszonylat', indulas, erkezes, menetido, varos}
 
 
 
 
 ## Szerző
 
 * Név: Nagy BÉLa
 * E-mail:nagy.bela.budapest@gmail.com
 
 ## Licenc
 
-Oktatási célra készült, szabadon használható
+Oktatási célra készült, szabadon használható.
```

### Comparing `magyar-2.9.2/README.md` & `magyar-2.9.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 14. Magyarország halai = magyar.hal
 15. Magyarország madarai = magyar.madar
 
 ## Szótárak  (dictionary): 
 1. Királyok és uralkodásuk ideje  = magyar.kiraly
 2. Vármegyék és azok székhelyei = magyar.megye_szekhely
 3. Járások, székhelyük , megye = magyar.jaras
+4. Villamosvonalak, végállomások, menetidő = magyar.villamos
 
 ## Description
 1. last names =  magyar.vezeteknev
 2. female first names = magyar.keresztnev_n
 3. male first names  = magyar.keresztnev_f
 4. street names = magyar.utca
 5. city names = magyar.telepules
@@ -42,14 +43,15 @@
 14. Fishes of Hungary = magyar.hal
 15. Birds of Hungary = magyar.madar
 
 Dictionary:
 1. Hungarian Kings and Reigns = magyar.kiraly
 2. Hungarian counties and their administrative centers = magyar.megye_szekhely
 3. Hungarian districts, their seats, county = magyar.jaras
+4. Hungarian tram lines  magyar.villamos
 
 ## Listák használat:
 
  Főként véletlengenerátorok kiegészítőjeként ajánlom a listákat
  
 I recommend it mainly as a supplement to random number generators. 
        
@@ -57,22 +59,23 @@
             utca = random.sample(magyar.utca, k=16) 
             random.choices()
             telepulesek = random.choice(magyar.telepules)
 
 ## Szótárak:
 Több adatot tartalmaznak összekapcsolva.
 
-magyar.kiraly tartalma :   {'király neve' : (uralkodása tól, ig)}
-magyar.megye_szekhely :    {'megye neve' : 'székhelye'}
-magyar.jaras :             {'megye' : (székhely, megye)}
+    magyar.kiraly tartalma :   {'király neve' : (uralkodása tól, ig)}
+    magyar.megye_szekhely :    {'megye neve' : 'székhelye'}
+    magyar.jaras :             {'megye' : (székhely, megye)}
+    magyar.villamos:    kulcs {'viszonylat', indulas, erkezes, menetido, varos}
 
 
 
 
 ## Szerző
 
 * Név: Nagy BÉLa
 * E-mail:nagy.bela.budapest@gmail.com
 
 ## Licenc
 
-Oktatási célra készült, szabadon használható
+Oktatási célra készült, szabadon használható.
```

### Comparing `magyar-2.9.2/magyar.egg-info/PKG-INFO` & `magyar-2.9.3/magyar.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magyar
-Version: 2.9.2
+Version: 2.9.3
 Summary: Hungarian names...
 Home-page: https://github.com/kobanya/nevek
 Author: Nagy Béla
 Author-email: nagy.belabudapest@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -32,14 +32,15 @@
 14. Magyarország halai = magyar.hal
 15. Magyarország madarai = magyar.madar
 
 ## Szótárak  (dictionary): 
 1. Királyok és uralkodásuk ideje  = magyar.kiraly
 2. Vármegyék és azok székhelyei = magyar.megye_szekhely
 3. Járások, székhelyük , megye = magyar.jaras
+4. Villamosvonalak, végállomások, menetidő = magyar.villamos
 
 ## Description
 1. last names =  magyar.vezeteknev
 2. female first names = magyar.keresztnev_n
 3. male first names  = magyar.keresztnev_f
 4. street names = magyar.utca
 5. city names = magyar.telepules
@@ -54,14 +55,15 @@
 14. Fishes of Hungary = magyar.hal
 15. Birds of Hungary = magyar.madar
 
 Dictionary:
 1. Hungarian Kings and Reigns = magyar.kiraly
 2. Hungarian counties and their administrative centers = magyar.megye_szekhely
 3. Hungarian districts, their seats, county = magyar.jaras
+4. Hungarian tram lines  magyar.villamos
 
 ## Listák használat:
 
  Főként véletlengenerátorok kiegészítőjeként ajánlom a listákat
  
 I recommend it mainly as a supplement to random number generators. 
        
@@ -69,22 +71,23 @@
             utca = random.sample(magyar.utca, k=16) 
             random.choices()
             telepulesek = random.choice(magyar.telepules)
 
 ## Szótárak:
 Több adatot tartalmaznak összekapcsolva.
 
-magyar.kiraly tartalma :   {'király neve' : (uralkodása tól, ig)}
-magyar.megye_szekhely :    {'megye neve' : 'székhelye'}
-magyar.jaras :             {'megye' : (székhely, megye)}
+    magyar.kiraly tartalma :   {'király neve' : (uralkodása tól, ig)}
+    magyar.megye_szekhely :    {'megye neve' : 'székhelye'}
+    magyar.jaras :             {'megye' : (székhely, megye)}
+    magyar.villamos:    kulcs {'viszonylat', indulas, erkezes, menetido, varos}
 
 
 
 
 ## Szerző
 
 * Név: Nagy BÉLa
 * E-mail:nagy.bela.budapest@gmail.com
 
 ## Licenc
 
-Oktatási célra készült, szabadon használható
+Oktatási célra készült, szabadon használható.
```

### Comparing `magyar-2.9.2/setup.py` & `magyar-2.9.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="magyar",
-    version="2.9.2",
+    version="2.9.3",
     author="Nagy Béla",
     author_email="nagy.belabudapest@gmail.com",
     description="Hungarian names...",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kobanya/nevek",
     py_modules=["magyar"],
```

