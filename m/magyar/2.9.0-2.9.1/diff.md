# Comparing `tmp/magyar-2.9.0.tar.gz` & `tmp/magyar-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magyar-2.9.0.tar", last modified: Fri Apr 14 20:33:37 2023, max compression
+gzip compressed data, was "magyar-2.9.1.tar", last modified: Sat Apr 15 22:09:16 2023, max compression
```

## Comparing `magyar-2.9.0.tar` & `magyar-2.9.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-04-14 20:33:37.108044 magyar-2.9.0/
--rw-rw-r--   0 bela      (1000) bela      (1000)     1798 2023-04-14 20:33:37.108044 magyar-2.9.0/PKG-INFO
--rw-rw-r--   0 bela      (1000) bela      (1000)     1427 2023-04-14 20:32:03.000000 magyar-2.9.0/README.md
-drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-04-14 20:33:37.108044 magyar-2.9.0/magyar.egg-info/
--rw-rw-r--   0 bela      (1000) bela      (1000)     1798 2023-04-14 20:33:37.000000 magyar-2.9.0/magyar.egg-info/PKG-INFO
--rw-rw-r--   0 bela      (1000) bela      (1000)      148 2023-04-14 20:33:37.000000 magyar-2.9.0/magyar.egg-info/SOURCES.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)        1 2023-04-14 20:33:37.000000 magyar-2.9.0/magyar.egg-info/dependency_links.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)        7 2023-04-14 20:33:37.000000 magyar-2.9.0/magyar.egg-info/top_level.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)    10941 2023-04-14 20:21:52.000000 magyar-2.9.0/magyar.py
--rw-rw-r--   0 bela      (1000) bela      (1000)       38 2023-04-14 20:33:37.108044 magyar-2.9.0/setup.cfg
--rw-rw-r--   0 bela      (1000) bela      (1000)      588 2023-04-14 20:33:32.000000 magyar-2.9.0/setup.py
+drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-04-15 22:09:16.544612 magyar-2.9.1/
+-rw-rw-r--   0 bela      (1000) bela      (1000)     1927 2023-04-15 22:09:16.544612 magyar-2.9.1/PKG-INFO
+-rw-rw-r--   0 bela      (1000) bela      (1000)     1556 2023-04-15 21:55:43.000000 magyar-2.9.1/README.md
+drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-04-15 22:09:16.544612 magyar-2.9.1/magyar.egg-info/
+-rw-rw-r--   0 bela      (1000) bela      (1000)     1927 2023-04-15 22:09:16.000000 magyar-2.9.1/magyar.egg-info/PKG-INFO
+-rw-rw-r--   0 bela      (1000) bela      (1000)      148 2023-04-15 22:09:16.000000 magyar-2.9.1/magyar.egg-info/SOURCES.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)        1 2023-04-15 22:09:16.000000 magyar-2.9.1/magyar.egg-info/dependency_links.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)        7 2023-04-15 22:09:16.000000 magyar-2.9.1/magyar.egg-info/top_level.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)    11866 2023-04-15 22:04:09.000000 magyar-2.9.1/magyar.py
+-rw-rw-r--   0 bela      (1000) bela      (1000)       38 2023-04-15 22:09:16.544612 magyar-2.9.1/setup.cfg
+-rw-rw-r--   0 bela      (1000) bela      (1000)      588 2023-04-15 21:55:43.000000 magyar-2.9.1/setup.py
```

### Comparing `magyar-2.9.0/PKG-INFO` & `magyar-2.9.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: magyar
-Version: 2.9.0
-Summary: Hungarian names...
-Home-page: https://github.com/kobanya/nevek
-Author: Nagy Béla
-Author-email: nagy.belabudapest@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-
 # magyar
 
 
 ## Leírás
 
 Magyar listák gyűjteménye - Collection of Hungarian lists.
 
@@ -23,28 +11,32 @@
 3. férfi keresztnevek = magyar.keresztnev_f
 4. utcanevek = magyar.utca
 5. telelpülésnevek= magyar.telepules
 6. vármegyék nevei = magyar.megye
 7. folyók nevei = magyar.folyo
 8. a hét napjai = magyar.nap
 9. az év hónapjai = magyar.honap
+10. gyümölcsok = magyar.gyumolcs
+11. zöldségek = magyar.zoldseg
 
 Szótárak  (dictionary): 
 1. Királyok és uralkodásuk ideje  = magyar.kiraly
 
 ## Description
 1. last names =  magyar.vezeteknev
 2. female first names = magyar.keresztnev_n
 3. male first names  = magyar.keresztnev_f
 4. street names = magyar.utca
 5. city names = magyar.telepules
 6. names of counties = magyar.megye
 7. names of rivers = magyar.folyo
 8. he days of the week = magyar.nap
 9. the months of the year = magyar.honap
+10. fruits = magyar.gyumolcs
+11. vegetables = magyar.zoldseg
 
 Dictionary:
 1. Hungarian Kings and Reigns = magyar.kiraly
 
 ## Listák használat:
 
  Főként véletlengenerátorok kiegészítőjeként ajánlom a listákat
@@ -65,8 +57,8 @@
 ## Szerző
 
 * Név: Nagy BÉLa
 * E-mail:nagy.bela.budapest@gmail.com
 
 ## Licenc
 
-Oktatási célra készült, szabadon használható
+Oktatási célra készült, szabadon használható
```

### Comparing `magyar-2.9.0/magyar.egg-info/PKG-INFO` & `magyar-2.9.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magyar
-Version: 2.9.0
+Version: 2.9.1
 Summary: Hungarian names...
 Home-page: https://github.com/kobanya/nevek
 Author: Nagy Béla
 Author-email: nagy.belabudapest@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,28 +23,32 @@
 3. férfi keresztnevek = magyar.keresztnev_f
 4. utcanevek = magyar.utca
 5. telelpülésnevek= magyar.telepules
 6. vármegyék nevei = magyar.megye
 7. folyók nevei = magyar.folyo
 8. a hét napjai = magyar.nap
 9. az év hónapjai = magyar.honap
+10. gyümölcsok = magyar.gyumolcs
+11. zöldségek = magyar.zoldseg
 
 Szótárak  (dictionary): 
 1. Királyok és uralkodásuk ideje  = magyar.kiraly
 
 ## Description
 1. last names =  magyar.vezeteknev
 2. female first names = magyar.keresztnev_n
 3. male first names  = magyar.keresztnev_f
 4. street names = magyar.utca
 5. city names = magyar.telepules
 6. names of counties = magyar.megye
 7. names of rivers = magyar.folyo
 8. he days of the week = magyar.nap
 9. the months of the year = magyar.honap
+10. fruits = magyar.gyumolcs
+11. vegetables = magyar.zoldseg
 
 Dictionary:
 1. Hungarian Kings and Reigns = magyar.kiraly
 
 ## Listák használat:
 
  Főként véletlengenerátorok kiegészítőjeként ajánlom a listákat
```

### Comparing `magyar-2.9.0/magyar.py` & `magyar-2.9.1/magyar.py`

 * *Files 7% similar despite different names*

```diff
@@ -90,14 +90,26 @@
          'Cserna', 'Ivacs-patak', 'Bükkös-patak', 'Pilinka', 'Bodva', 'Hármas-Körös', 'Sajgó']
 
 nap = ['hétfő', 'kedd', 'szerda', 'csütörtök', 'péntek', 'szombat', 'vasárnap']
 
 honap = ['január', 'február', 'március', 'április', 'május', 'június', 'július',
          'augusztus', 'szeptember', 'október', 'november', 'december']
 
+gyumolcs= ['alma', 'ananász',  'banán', 'barack', 'birs', 'cseresznye', 'datolya', 'dinnye', 'eper', 'füge',
+            'gránátalma', 'kajszibarack', 'kivi', 'málna', 'meggy', 'narancs', 'őszibarack', 'ribizli',
+            'sárgabarack', 'szeder', 'szilva', 'egres', 'vörösszőlő', 'szeder', 'körte', 'meggy', 'áfonya',
+           'sárgadinnye', 'erdei szamóca', 'mangó']
+zoldseg = ['articsóka', 'bab', 'borsó', 'brokkoli', 'burgonya', 'cékla', 'csicsóka', 'csiperkegomba', 'fokhagyma',
+           'hagyma', 'karalábé', 'karfiol', 'káposzta', 'kelbimbó', 'kukorica', 'fejes sajáta', 'lilahagyma',
+           'lilakáposzta', 'padlizsán', 'paprika', 'paszternák', 'retek', 'sárgarépa', 'spárga', 'spenót',
+           'sütőtök', 'tök', 'uborka', 'zeller', 'sárgarépa', 'feketeretek','zeller', 'kínai kel', 'retek',
+           'jégcsapretek', 'fokhagyma', 'újhagyma', 'szárzeller']
+
+
+
 kiraly = {'Árpád': (895, 907), 'Zoltán': (907, 947), 'Fajsz': (947, 955), 'Taksony': (955, 972), 'Géza': (972, 997),
     'I.István': (997, 1038),'I. Péter': (1038, 1041), 'Sámuel': (1041, 1044), 'Péter-2': (1044, 1045), 'I.András': (1041, 1060),
     'I. Béla': (1060, 1063), 'Salamon': (1063, 1074), 'I. Géza': (1074, 1077), 'I. László': (1077, 1095),
     'Kálmán': (1095, 1116),'II. István': (1116, 1131), 'II. Béla': (1131, 1141), 'II. Géza': (1141,1162),
     'III. István': (1162, 1172), 'III. Béla': (1172, 1196), 'Imre':(1196, 1204), 'III. László': (1204, 1205),
     'II. András': (1205, 1235),'IV. Béla': (1235, 1270), 'V. István': (1270, 1272), 'IV. László': (1272, 1290),
     'III. András': (1290, 1301), 'Vencel': (1301, 1305), 'Ottó': (1305, 1307), 'I. Károly': (1308, 1342),
```

### Comparing `magyar-2.9.0/setup.py` & `magyar-2.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="magyar",
-    version="2.9.0",
+    version="2.9.1",
     author="Nagy Béla",
     author_email="nagy.belabudapest@gmail.com",
     description="Hungarian names...",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kobanya/nevek",
     py_modules=["magyar"],
```

