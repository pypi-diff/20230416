# Comparing `tmp/makerlabs-0.31.tar.gz` & `tmp/makerlabs-0.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "makerlabs-0.31.tar", last modified: Sat Apr 15 09:32:39 2023, max compression
+gzip compressed data, was "makerlabs-0.32.tar", last modified: Sun Apr 16 15:13:15 2023, max compression
```

## Comparing `makerlabs-0.31.tar` & `makerlabs-0.32.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 massimo    (501) staff       (20)        0 2023-04-15 09:32:39.453284 makerlabs-0.31/
--rw-r--r--   0 massimo    (501) staff       (20)     7633 2021-02-28 19:17:44.000000 makerlabs-0.31/LICENSE.md
--rw-r--r--   0 massimo    (501) staff       (20)     2177 2023-04-15 09:32:39.453616 makerlabs-0.31/PKG-INFO
--rw-r--r--   0 massimo    (501) staff       (20)     1395 2023-02-20 10:19:56.000000 makerlabs-0.31/README.md
-drwxr-xr-x   0 massimo    (501) staff       (20)        0 2023-04-15 09:32:39.440235 makerlabs-0.31/makerlabs/
--rw-r--r--   0 massimo    (501) staff       (20)        0 2022-04-16 18:00:11.000000 makerlabs-0.31/makerlabs/__init__.py
--rw-r--r--   0 massimo    (501) staff       (20)     1817 2022-09-08 18:39:43.000000 makerlabs-0.31/makerlabs/classes.py
--rw-r--r--   0 massimo    (501) staff       (20)     5582 2023-02-19 22:33:12.000000 makerlabs-0.31/makerlabs/diybio_org.py
--rw-r--r--   0 massimo    (501) staff       (20)     3280 2023-04-14 23:44:23.000000 makerlabs-0.31/makerlabs/fablabs_io.py
--rw-r--r--   0 massimo    (501) staff       (20)     3528 2023-02-19 22:45:09.000000 makerlabs-0.31/makerlabs/hackaday_io.py
--rw-r--r--   0 massimo    (501) staff       (20)     8657 2023-02-19 22:35:18.000000 makerlabs-0.31/makerlabs/hackerspaces_org.py
--rw-r--r--   0 massimo    (501) staff       (20)     3062 2023-02-19 22:45:46.000000 makerlabs-0.31/makerlabs/makerfaire_com.py
--rw-r--r--   0 massimo    (501) staff       (20)     2630 2023-02-19 22:35:34.000000 makerlabs-0.31/makerlabs/makerspaces_make_co.py
--rw-r--r--   0 massimo    (501) staff       (20)     2705 2023-02-19 22:35:42.000000 makerlabs-0.31/makerlabs/makery_info.py
--rw-r--r--   0 massimo    (501) staff       (20)     7925 2023-02-19 22:35:49.000000 makerlabs-0.31/makerlabs/repaircafe_org.py
--rw-r--r--   0 massimo    (501) staff       (20)     3739 2023-02-19 22:46:55.000000 makerlabs-0.31/makerlabs/timeline.py
--rw-r--r--   0 massimo    (501) staff       (20)     4447 2022-09-12 10:56:14.000000 makerlabs-0.31/makerlabs/utils.py
-drwxr-xr-x   0 massimo    (501) staff       (20)        0 2023-04-15 09:32:39.452346 makerlabs-0.31/makerlabs.egg-info/
--rw-r--r--   0 massimo    (501) staff       (20)     2177 2023-04-15 09:32:39.000000 makerlabs-0.31/makerlabs.egg-info/PKG-INFO
--rw-r--r--   0 massimo    (501) staff       (20)      504 2023-04-15 09:32:39.000000 makerlabs-0.31/makerlabs.egg-info/SOURCES.txt
--rw-r--r--   0 massimo    (501) staff       (20)        1 2023-04-15 09:32:39.000000 makerlabs-0.31/makerlabs.egg-info/dependency_links.txt
--rw-r--r--   0 massimo    (501) staff       (20)      165 2023-04-15 09:32:39.000000 makerlabs-0.31/makerlabs.egg-info/requires.txt
--rw-r--r--   0 massimo    (501) staff       (20)       10 2023-04-15 09:32:39.000000 makerlabs-0.31/makerlabs.egg-info/top_level.txt
--rw-r--r--   0 massimo    (501) staff       (20)      495 2023-04-15 09:32:39.455092 makerlabs-0.31/setup.cfg
--rw-r--r--   0 massimo    (501) staff       (20)     1552 2023-04-15 09:29:41.000000 makerlabs-0.31/setup.py
+drwxr-xr-x   0 massimo    (501) staff       (20)        0 2023-04-16 15:13:15.223894 makerlabs-0.32/
+-rw-r--r--   0 massimo    (501) staff       (20)     7633 2021-02-28 19:17:44.000000 makerlabs-0.32/LICENSE.md
+-rw-r--r--   0 massimo    (501) staff       (20)     2261 2023-04-16 15:13:15.224362 makerlabs-0.32/PKG-INFO
+-rw-r--r--   0 massimo    (501) staff       (20)     1479 2023-04-16 15:05:59.000000 makerlabs-0.32/README.md
+drwxr-xr-x   0 massimo    (501) staff       (20)        0 2023-04-16 15:13:15.184309 makerlabs-0.32/makerlabs/
+-rw-r--r--   0 massimo    (501) staff       (20)        0 2022-04-16 18:00:11.000000 makerlabs-0.32/makerlabs/__init__.py
+-rw-r--r--   0 massimo    (501) staff       (20)     1817 2022-09-08 18:39:43.000000 makerlabs-0.32/makerlabs/classes.py
+-rw-r--r--   0 massimo    (501) staff       (20)     5737 2023-04-15 10:14:17.000000 makerlabs-0.32/makerlabs/diybio_org.py
+-rw-r--r--   0 massimo    (501) staff       (20)     3726 2023-04-15 11:39:15.000000 makerlabs-0.32/makerlabs/fablabs_io.py
+-rw-r--r--   0 massimo    (501) staff       (20)     3528 2023-02-19 22:45:09.000000 makerlabs-0.32/makerlabs/hackaday_io.py
+-rw-r--r--   0 massimo    (501) staff       (20)     8946 2023-04-15 15:15:18.000000 makerlabs-0.32/makerlabs/hackerspaces_org.py
+-rw-r--r--   0 massimo    (501) staff       (20)     3062 2023-02-19 22:45:46.000000 makerlabs-0.32/makerlabs/makerfaire_com.py
+-rw-r--r--   0 massimo    (501) staff       (20)     2630 2023-02-19 22:35:34.000000 makerlabs-0.32/makerlabs/makerspaces_make_co.py
+-rw-r--r--   0 massimo    (501) staff       (20)     2705 2023-02-19 22:35:42.000000 makerlabs-0.32/makerlabs/makery_info.py
+-rw-r--r--   0 massimo    (501) staff       (20)     7925 2023-02-19 22:35:49.000000 makerlabs-0.32/makerlabs/repaircafe_org.py
+-rw-r--r--   0 massimo    (501) staff       (20)     3739 2023-02-19 22:46:55.000000 makerlabs-0.32/makerlabs/timeline.py
+-rw-r--r--   0 massimo    (501) staff       (20)     4447 2022-09-12 10:56:14.000000 makerlabs-0.32/makerlabs/utils.py
+drwxr-xr-x   0 massimo    (501) staff       (20)        0 2023-04-16 15:13:15.218553 makerlabs-0.32/makerlabs.egg-info/
+-rw-r--r--   0 massimo    (501) staff       (20)     2261 2023-04-16 15:13:14.000000 makerlabs-0.32/makerlabs.egg-info/PKG-INFO
+-rw-r--r--   0 massimo    (501) staff       (20)      504 2023-04-16 15:13:14.000000 makerlabs-0.32/makerlabs.egg-info/SOURCES.txt
+-rw-r--r--   0 massimo    (501) staff       (20)        1 2023-04-16 15:13:14.000000 makerlabs-0.32/makerlabs.egg-info/dependency_links.txt
+-rw-r--r--   0 massimo    (501) staff       (20)      165 2023-04-16 15:13:14.000000 makerlabs-0.32/makerlabs.egg-info/requires.txt
+-rw-r--r--   0 massimo    (501) staff       (20)       10 2023-04-16 15:13:14.000000 makerlabs-0.32/makerlabs.egg-info/top_level.txt
+-rw-r--r--   0 massimo    (501) staff       (20)      495 2023-04-16 15:13:15.226844 makerlabs-0.32/setup.cfg
+-rw-r--r--   0 massimo    (501) staff       (20)     1552 2023-04-16 15:03:57.000000 makerlabs-0.32/setup.py
```

### Comparing `makerlabs-0.31/LICENSE.md` & `makerlabs-0.32/LICENSE.md`

 * *Files identical despite different names*

### Comparing `makerlabs-0.31/PKG-INFO` & `makerlabs-0.32/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: makerlabs
-Version: 0.31
+Version: 0.32
 Home-page: https://github.com/openp2pdesign/makerlabs
-Download-URL: https://github.com/openp2pdesign/makerlabs/releases/tag/v0.31
+Download-URL: https://github.com/openp2pdesign/makerlabs/releases/tag/v0.32
 Author: Massimo Menichinelli
 Author-email: info@openp2pdesign.org
 Keywords: Fab Lab,Fab Lab,Makerspace,Hackerspace,Repair Cafes,Makers,DIYbio
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: Environment :: Web Environment
 Classifier: Operating System :: OS Independent
@@ -40,11 +40,12 @@
 
 
 ## History
 This package continues the development of the discontinued packages *PyMakerspaces* at [https://pypi.python.org/pypi/PyMakerspaces/](https://pypi.python.org/pypi/PyMakerspaces/).
 
 ## Credits
 v0.14-v0.21.3:
+The research behind this software has taken place during the H2020 MAKE-IT project.
 [![](doc/images/from_30.png)](https://ec.europa.eu/digital-agenda/en/news/22-new-caps-projects-horizon-2020)
 
-v0.30:
+v0.3x:
 The research behind this software has taken place at the Politecnico di Milano during Massimo Menichinelli's stay as Senior Resident Researcher from 01/02/2021 to 08/01/2022.
```

### Comparing `makerlabs-0.31/README.md` & `makerlabs-0.32/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -21,11 +21,12 @@
 
 
 ## History
 This package continues the development of the discontinued packages *PyMakerspaces* at [https://pypi.python.org/pypi/PyMakerspaces/](https://pypi.python.org/pypi/PyMakerspaces/).
 
 ## Credits
 v0.14-v0.21.3:
+The research behind this software has taken place during the H2020 MAKE-IT project.
 [![](doc/images/from_30.png)](https://ec.europa.eu/digital-agenda/en/news/22-new-caps-projects-horizon-2020)
 
-v0.30:
+v0.3x:
 The research behind this software has taken place at the Politecnico di Milano during Massimo Menichinelli's stay as Senior Resident Researcher from 01/02/2021 to 08/01/2022.
```

### Comparing `makerlabs-0.31/makerlabs/classes.py` & `makerlabs-0.32/makerlabs/classes.py`

 * *Files identical despite different names*

### Comparing `makerlabs-0.31/makerlabs/diybio_org.py` & `makerlabs-0.32/makerlabs/diybio_org.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     """Represents a DIYBio Lab as it is described on diybio.org."""
 
     def __init__(self):
         self.source = "diybio.org"
         self.lab_type = "DIYBio Lab"
 
 
-def data_from_diybio_org():
+def data_from_diybio_org(API_endpoint):
     """Scrapes data from diybio.org."""
 
     r = requests.get(API_endpoint)
 
     if r.status_code == 200:
         # Fix a problem in the html source while loading it
         data = BeautifulSoup(r.text.replace('\xa0', ''), "lxml")
@@ -48,15 +48,15 @@
 
     return data
 
 
 def get_labs(format, open_cage_api_key):
     """Gets DIYBio Lab data from diybio.org."""
 
-    diybiolabs_soup = data_from_diybio_org()
+    diybiolabs_soup = data_from_diybio_org(API_endpoint)
     diybiolabs = {}
 
     rows_list = []
     continents_dict = {}
     continents_order = 0
     ranges_starting_points = []
 
@@ -101,15 +101,18 @@
                 if continents_dict[i] == "USA-EAST" or continents_dict[
                         i] == "USA-WEST":
                     current_lab.state = rows_list[j][2].contents[0].replace(
                         " ", "").encode('utf-8')
                 else:
                     current_lab.country_code = rows_list[j][2].contents[
                         0].encode('utf-8')
-                current_lab.url = rows_list[j][3].contents[0].attrs['href']
+                try:
+                    current_lab.url = rows_list[j][3].contents[0].attrs['href']
+                except:
+                    current_lab.url = rows_list[j][3].contents[0]
                 # Each lab is identified by the simplified url
                 slug = current_lab.url
                 if "http://" in slug:
                     slug = slug.replace("http://", "")
                 elif "https://" in slug:
                     slug = slug.replace("https://", "")
                 if "www." in slug:
@@ -119,15 +122,15 @@
 
                 # Data from the USA is not really well formatted
                 if continents_dict[i] == "USA-EAST" or continents_dict[i] == "USA-WEST":
                     current_lab.continent = "North America"
                     current_lab.country_code = "USA"
                     current_lab.country = "United States of America"
                     current_lab.state = us.states.lookup(
-                        current_lab.state).name
+                        current_lab.state.decode('utf-8')).name
 
                 # Get address from city
                 address = get_location(query=current_lab.city, format="direct", api_key=open_cage_api_key)
                 current_lab.continent = address["continent"]
                 current_lab.latitude = address["latitude"]
                 current_lab.longitude = address["longitude"]
                 current_lab.address_1 = address["address_1"]
```

### Comparing `makerlabs-0.31/makerlabs/fablabs_io.py` & `makerlabs-0.32/makerlabs/fablabs_io.py`

 * *Files 21% similar despite different names*

```diff
@@ -36,22 +36,22 @@
     """Gets data from fablabs.io."""
 
     data = requests.get(API_endpoint).json()
 
     return data
 
 
-def get_labs(format):
+def get_labs(format, open_cage_api_key):
     """Gets Fab Lab data from fablabs.io."""
 
     fablabs_json = data_from_fablabs_io(API_endpoint)
     labs = {}
 
     # Load all the FabLabs
-    for i in fablabs_json["labs"]:
+    for i in fablabs_json:
         current_lab = FabLab()
         current_lab.name = i["name"]
         current_lab.address_1 = i["address_1"]
         current_lab.address_2 = i["address_2"]
         current_lab.address_notes = i["address_notes"]
         current_lab.avatar = i["avatar_url"]
         current_lab.blurb = i["blurb"]
@@ -63,42 +63,55 @@
         current_lab.county = i["county"]
         current_lab.description = i["description"]
         current_lab.email = i["email"]
         current_lab.id = i["id"]
         current_lab.phone = i["phone"]
         current_lab.postal_code = i["postal_code"]
         current_lab.slug = i["slug"]
-        current_lab.url = i["url"]
-
-        continent_code = pycountry.country_alpha2_to_continent_code(i["country_code"])
-        current_lab.continent = pycountry.convert_continent_code_to_continent_name(continent_code)
-
-        current_country = pycountry.countries.get(alpha_2=i["country_code"].upper())
-        current_lab.country_code = current_country.alpha_3
-        current_lab.country = current_country.name
 
         # Check coordinates
         if i["longitude"] is not None:
             current_lab.longitude = i["longitude"]
         else:
             current_lab.longitude = 0.0
         if i["latitude"] is not None:
             current_lab.latitude = i["latitude"]
         else:
             current_lab.latitude = 0.0
 
+        # Get address from coordinates
+        # Try, in case there are issues with some coordinates formatting
+        try:
+            location = get_location(query=(
+                current_lab.latitude,
+                current_lab.longitude),
+                format="reverse",
+                api_key=open_cage_api_key)
+
+            current_lab.address_1 = location["address_1"]
+            current_lab.city = location["city"]
+            current_lab.country_code = location["country_code"]
+            current_lab.country = location["country"]
+            current_lab.county = location["county"]
+            current_lab.postal_code = location["postal_code"]
+            current_lab.continent = location["continent"]
+            current_lab.state = location["state"]
+        except:
+            pass
+
         # Find Facebook and Twitter links, add also the other ones
         current_lab.links = {"facebook": "", "twitter": ""}
         for link in i["links"]:
             if "facebook" in link["url"]:
                 current_lab.links["facebook"] = link["url"]
             elif "twitter" in link["url"]:
                 current_lab.links["twitter"] = link["url"]
             else:
                 current_lab.links[link["id"]] = link["url"]
+                current_lab.url = link["url"]
 
         # Add the lab to the list
         labs[i["slug"]] = current_lab
 
     # Return formatted data
     data = format_labs_data(format=format, labs=labs)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `makerlabs-0.31/makerlabs/hackaday_io.py` & `makerlabs-0.32/makerlabs/hackaday_io.py`

 * *Files identical despite different names*

### Comparing `makerlabs-0.31/makerlabs/hackerspaces_org.py` & `makerlabs-0.32/makerlabs/hackerspaces_org.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 from . utils import get_location
 from . utils import format_labs_data
 
 import json
 import requests
 import pandas as pd
 from bs4 import BeautifulSoup
+from requests.adapters import HTTPAdapter
+from requests.packages.urllib3.util.retry import Retry
 
 # Endpoints
 API_endpoint = "https://wiki.hackerspaces.org/w/api.php"
 
 
 class Hackerspace(Lab):
 
@@ -78,14 +80,18 @@
         params = {
             "action": "parse",
             "page": i,
             "prop": "text",
             "formatversion": "2",
             "format": "json"
         }
+        retry_strategy = Retry(total=3,backoff_factor=1)
+        adapter = HTTPAdapter(max_retries=retry_strategy)
+        req.mount("https://", adapter)
+        req.mount("http://", adapter)
         request_data = req.get(url=API_endpoint, params=params).json()
         current_lab.name = request_data['parse']['title']
         current_lab.links = {"facebook": "", "twitter": ""}
         content = BeautifulSoup(request_data['parse']['text'], 'html.parser')
         # Get coordinates from the embedded map
         # If the lab has no locations, we don't consider it
         map_div = content.find("div", {"class": "mapdata"})
```

### Comparing `makerlabs-0.31/makerlabs/makerfaire_com.py` & `makerlabs-0.32/makerlabs/makerfaire_com.py`

 * *Files identical despite different names*

### Comparing `makerlabs-0.31/makerlabs/makerspaces_make_co.py` & `makerlabs-0.32/makerlabs/makerspaces_make_co.py`

 * *Files identical despite different names*

### Comparing `makerlabs-0.31/makerlabs/makery_info.py` & `makerlabs-0.32/makerlabs/makery_info.py`

 * *Files identical despite different names*

### Comparing `makerlabs-0.31/makerlabs/repaircafe_org.py` & `makerlabs-0.32/makerlabs/repaircafe_org.py`

 * *Files identical despite different names*

### Comparing `makerlabs-0.31/makerlabs/timeline.py` & `makerlabs-0.32/makerlabs/timeline.py`

 * *Files identical despite different names*

### Comparing `makerlabs-0.31/makerlabs/utils.py` & `makerlabs-0.32/makerlabs/utils.py`

 * *Files identical despite different names*

### Comparing `makerlabs-0.31/makerlabs.egg-info/PKG-INFO` & `makerlabs-0.32/makerlabs.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: makerlabs
-Version: 0.31
+Version: 0.32
 Home-page: https://github.com/openp2pdesign/makerlabs
-Download-URL: https://github.com/openp2pdesign/makerlabs/releases/tag/v0.31
+Download-URL: https://github.com/openp2pdesign/makerlabs/releases/tag/v0.32
 Author: Massimo Menichinelli
 Author-email: info@openp2pdesign.org
 Keywords: Fab Lab,Fab Lab,Makerspace,Hackerspace,Repair Cafes,Makers,DIYbio
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: Environment :: Web Environment
 Classifier: Operating System :: OS Independent
@@ -40,11 +40,12 @@
 
 
 ## History
 This package continues the development of the discontinued packages *PyMakerspaces* at [https://pypi.python.org/pypi/PyMakerspaces/](https://pypi.python.org/pypi/PyMakerspaces/).
 
 ## Credits
 v0.14-v0.21.3:
+The research behind this software has taken place during the H2020 MAKE-IT project.
 [![](doc/images/from_30.png)](https://ec.europa.eu/digital-agenda/en/news/22-new-caps-projects-horizon-2020)
 
-v0.30:
+v0.3x:
 The research behind this software has taken place at the Politecnico di Milano during Massimo Menichinelli's stay as Senior Resident Researcher from 01/02/2021 to 08/01/2022.
```

### Comparing `makerlabs-0.31/setup.py` & `makerlabs-0.32/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,21 +27,21 @@
         "pytz",
         "requests",
         "six",
         "soupsieve",
         "urllib3",
         "us"
     ],
-    version='0.31',
+    version='0.32',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Massimo Menichinelli',
     author_email='info@openp2pdesign.org',
     url='https://github.com/openp2pdesign/makerlabs',
-    download_url='https://github.com/openp2pdesign/makerlabs/releases/tag/v0.31',
+    download_url='https://github.com/openp2pdesign/makerlabs/releases/tag/v0.32',
     keywords=['Fab Lab', 'Fab Lab', 'Makerspace', 'Hackerspace', 'Repair Cafes',
               'Makers', 'DIYbio'],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Topic :: Utilities",
         "Environment :: Web Environment",
         "Operating System :: OS Independent",
```

