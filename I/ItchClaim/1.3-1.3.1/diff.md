# Comparing `tmp/ItchClaim-1.3.tar.gz` & `tmp/ItchClaim-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ItchClaim-1.3.tar", last modified: Sat Apr  1 08:37:50 2023, max compression
+gzip compressed data, was "ItchClaim-1.3.1.tar", last modified: Sun Apr 16 16:18:16 2023, max compression
```

## Comparing `ItchClaim-1.3.tar` & `ItchClaim-1.3.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 08:37:50.985150 ItchClaim-1.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 08:37:50.985150 ItchClaim-1.3/ItchClaim/
--rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-04-01 08:37:32.000000 ItchClaim-1.3/ItchClaim/DiskManager.py
--rw-r--r--   0 runner    (1001) docker     (123)    10204 2023-04-01 08:37:32.000000 ItchClaim-1.3/ItchClaim/ItchGame.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-04-01 08:37:32.000000 ItchClaim-1.3/ItchClaim/ItchSale.py
--rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-04-01 08:37:32.000000 ItchClaim-1.3/ItchClaim/ItchUser.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-01 08:37:32.000000 ItchClaim-1.3/ItchClaim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-04-01 08:37:32.000000 ItchClaim-1.3/ItchClaim/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-04-01 08:37:32.000000 ItchClaim-1.3/ItchClaim/index.template.html
--rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-04-01 08:37:32.000000 ItchClaim-1.3/ItchClaim/web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 08:37:50.985150 ItchClaim-1.3/ItchClaim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-04-01 08:37:50.000000 ItchClaim-1.3/ItchClaim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-01 08:37:50.000000 ItchClaim-1.3/ItchClaim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-01 08:37:50.000000 ItchClaim-1.3/ItchClaim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-01 08:37:50.000000 ItchClaim-1.3/ItchClaim.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-01 08:37:50.000000 ItchClaim-1.3/ItchClaim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-01 08:37:50.000000 ItchClaim-1.3/ItchClaim.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-01 08:37:32.000000 ItchClaim-1.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-04-01 08:37:50.985150 ItchClaim-1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-04-01 08:37:32.000000 ItchClaim-1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-01 08:37:32.000000 ItchClaim-1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-01 08:37:32.000000 ItchClaim-1.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-01 08:37:50.985150 ItchClaim-1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:18:16.838622 ItchClaim-1.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:18:16.838622 ItchClaim-1.3.1/ItchClaim/
+-rw-r--r--   0 runner    (1001) docker     (123)     8406 2023-04-16 16:18:00.000000 ItchClaim-1.3.1/ItchClaim/DiskManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10820 2023-04-16 16:18:00.000000 ItchClaim-1.3.1/ItchClaim/ItchGame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-04-16 16:18:00.000000 ItchClaim-1.3.1/ItchClaim/ItchSale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8252 2023-04-16 16:18:00.000000 ItchClaim-1.3.1/ItchClaim/ItchUser.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-16 16:18:00.000000 ItchClaim-1.3.1/ItchClaim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6091 2023-04-16 16:18:00.000000 ItchClaim-1.3.1/ItchClaim/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-04-16 16:18:00.000000 ItchClaim-1.3.1/ItchClaim/index.template.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-04-16 16:18:00.000000 ItchClaim-1.3.1/ItchClaim/web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:18:16.838622 ItchClaim-1.3.1/ItchClaim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-04-16 16:18:16.000000 ItchClaim-1.3.1/ItchClaim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-16 16:18:16.000000 ItchClaim-1.3.1/ItchClaim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 16:18:16.000000 ItchClaim-1.3.1/ItchClaim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-16 16:18:16.000000 ItchClaim-1.3.1/ItchClaim.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-16 16:18:16.000000 ItchClaim-1.3.1/ItchClaim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-16 16:18:16.000000 ItchClaim-1.3.1/ItchClaim.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-16 16:18:00.000000 ItchClaim-1.3.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-04-16 16:18:16.838622 ItchClaim-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-04-16 16:18:00.000000 ItchClaim-1.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-16 16:18:00.000000 ItchClaim-1.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-16 16:18:00.000000 ItchClaim-1.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 16:18:16.838622 ItchClaim-1.3.1/setup.cfg
```

### Comparing `ItchClaim-1.3/ItchClaim/DiskManager.py` & `ItchClaim-1.3.1/ItchClaim/DiskManager.py`

 * *Files 25% similar despite different names*

```diff
@@ -16,16 +16,19 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-import os, requests, json
 from typing import List
+import os
+import json
+import requests
+from bs4 import BeautifulSoup
 from .ItchGame import ItchGame
 from .ItchSale import ItchSale
 from . import __version__
 
 def get_all_sales(start: int) -> List[ItchGame]:
     """Download details about every sale posted on itch.io
 
@@ -76,27 +79,27 @@
     games_raw = current_sale.soup.find_all('div', class_="game_cell")
 
     if len(games_raw) == 0:
         print(f'Sale page #{page}: empty page')
         return 0
 
     for div in games_raw:
-        game: ItchGame = ItchGame.from_div(div)
+        game: ItchGame = ItchGame.from_div(div, price_needed=True)
 
         if game.price != 0:
             print(f'Sale page #{page}: games are not discounted by 100%')
             break
 
         # If the sale is not active, we can't check if it's claimable
         if not current_sale.is_active:
             game.claimable = None
 
         # load previously saved sales
         if os.path.exists(game.get_default_game_filename()):
-            disk_game: ItchGame = ItchGame.load_from_disk(game.get_default_game_filename())
+            disk_game: ItchGame = ItchGame.load_from_disk(game.get_default_game_filename(), refresh_claimable=True)
             game.sales = disk_game.sales
             if game.sales[-1].id == page and not force:
                 print(f'Sale {page} has been already saved for game {game.name} (wrong resume index?)')
                 continue
         
         if not force:
             game.sales.append(current_sale)
@@ -112,18 +115,92 @@
                 game.sales.append(current_sale)
                 game.sales.sort(key=lambda a: a.id)
 
         games_num += 1
         game.save_to_disk()
 
     if game.price == 0:
-        expired_str = '(inactive)' if current_sale.is_active else ''
+        expired_str = '(inactive)' if not current_sale.is_active else ''
         print(f'Sale page #{page}: added {len(games_raw)} games', expired_str)
     return games_num
 
+def get_all_sale_pages(category: str = 'games') -> List[ItchGame]:
+    """Gets all the pages of the sales feed from itch.io, and saves the missing games
+
+    Args:
+        category (str): the category of the items
+            Possible values: games, tools, game-assets, comics, books, physical-games,
+            soundtracks, game-mods, misc"""
+    page = -1
+    games_num = 0
+    while True:
+        page += 1
+        try:
+            games_added = get_online_sale_page(page, category=category)
+            if games_added == -1:
+                break
+            else:
+                games_num += games_added
+        #pylint: disable=broad-exception-caught
+        except Exception as ex:
+            print(f'Failed to parse {category} sale page {page}. Reason: {ex}')
+
+    print(f'Collecting sales from category {category} finished.',
+          f'Added a total of {games_num} {category}')
+
+def get_online_sale_page(page: int, category: str = 'games') -> int:
+    """Get a page of the sales feed from itch.io, and save the missing ones to the disk.
+    Supposed to be ran after get_all_sales() to catch updated sales.
+    
+    Args:
+        page (int): the id of the page to load
+        category (str): the category of the items
+            Possible values: games, tools, game-assets, comics, books, physical-games,
+            soundtracks, game-mods, misc
+
+    Returns:
+        int: The number of games updated
+    """
+    print(f'Processing {category} sale page #{page}')
+    r = requests.get(f"https://itch.io/{category}/newest/on-sale?page={page}&format=json",
+                    headers={'User-Agent': f'ItchClaim {__version__}'},
+                    timeout=8,)
+    html = json.loads(r.text)['content']
+    soup = BeautifulSoup(html, 'html.parser')
+    games_raw = soup.find_all('div', class_="game_cell")
+    games = []
+    games_added = 0
+    for div in games_raw:
+        game = ItchGame.from_div(div, price_needed=True)
+        if game.price == 0:
+            # Save game if it's new to us
+            if not os.path.exists(game.get_default_game_filename()):
+                # Call API to get active sale
+                ItchGame.from_api(game.url).save_to_disk()
+                print(f'Saved new {category} {game.name} ({game.url})')
+                games_added += 1
+                continue
+
+            # load previously saved sales
+            game = ItchGame.load_from_disk(game.get_default_game_filename(), refresh_claimable=True)
+            if game.active_sale:
+                print(f'Skipping {category} {game.name} ({game.url}): already active sale found on disk')
+                continue
+
+            # Call API to get active sale
+            sale = ItchGame.from_api(game.url).active_sale
+            game.sales.append(sale)
+            game.sales.sort(key=lambda a: a.id)
+            game.save_to_disk()
+            print(f'Updated values for {category} {game.name} ({game.url})')
+            games_added += 1
+    if len(games) == 0 and json.loads(r.text)["num_items"] == 0:
+        return -1
+    return games_added
+
 def load_all_games():
     """Load all games cached on the disk"""
     l: List[ItchGame] = []
     for file in os.listdir(ItchGame.games_dir):
         if not file.endswith('.json'):
             continue
         path = os.path.join(ItchGame.games_dir, file)
```

### Comparing `ItchClaim-1.3/ItchClaim/ItchGame.py` & `ItchClaim-1.3.1/ItchClaim/ItchGame.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,16 +37,22 @@
         self.name: str = None
         self.url: str = None
         self.price: float = None
         self.sales: List[ItchSale] = []
         self.cover_image: str = None
 
     @classmethod
-    def from_div(cls, div: Tag):
-        """Create an ItchGame Instance from a div that's found in the sale page or the my purchases page"""
+    def from_div(cls, div: Tag, price_needed: bool = False):
+        """Create an ItchGame Instance from a div that's found in tables on itch.io.
+        These can usually be found on the sale or the my purchases page.
+        
+        Args
+            div (Tag): A bs4 div element, containing the data of a game
+            price_needed (bool): wether to send another request to the API if the div has no
+                information about the price"""
         id = int(div.attrs['data-game_id'])
         self = ItchGame(id)
         a = div.find('a', class_='title game_link')
         self.name = a.text
         self.url = a.attrs['href']
 
         try:
@@ -55,15 +61,15 @@
             self.cover_image = None
 
         price_element = div.find('div', attrs={'class': 'price_value'})
         # Some elements don't have a price defined
         if price_element != None:
             price_str = re.findall(r"[-+]?(?:\d*\.\d+|\d+)", price_element.text)[0]
             self.price = float(price_str)
-        else:
+        elif price_needed:
             # some obscure games have no price (they are always free) and are also
             # discounted by 100% and are claimable, for example:
             # https://web.archive.org/web/20230308004149/https://itch.io/s/88108/100-discount
             api_data = ItchGame.from_api(self.url)
 
             # only 100% sales are collected by the from_api() method
             # this filters free games in bundles, for example:
@@ -85,25 +91,31 @@
             'sales': ItchSale.serialize_list(self.sales),
             'cover_image': self.cover_image,
         }
         with open(self.get_default_game_filename(), 'w', encoding='utf-8') as f:
             f.write(json.dumps(data))
 
     @classmethod
-    def load_from_disk(cls, path: str):
-        """Load cached details about game from the disk"""
+    def load_from_disk(cls, path: str, refresh_claimable: bool = False):
+        """Load cached details about game from the disk
+        
+        Args:
+            path (str): The location of the JSON file that contains the data about the game
+            refresh_claimable (bool): Check claimability online again
+                Defaults to False
+            """
         with open(path, 'r', encoding='utf-8') as f:
             data = json.loads(f.read())
         id = data['id']
         self = ItchGame(id)
         self.name = data['name']
         self.url = data['url']
         self.price = data['price']
         self.sales = [ ItchSale.from_dict(sale) for sale in data['sales'] ]
-        if data['claimable'] is not None:
+        if data['claimable'] is not None and not refresh_claimable:
             self.claimable = data['claimable']
         self.cover_image = data['cover_image']
         return self
 
     @classmethod
     def from_api(cls, url: str):
         """Get details about a game from the itch.io API
```

### Comparing `ItchClaim-1.3/ItchClaim/ItchSale.py` & `ItchClaim-1.3.1/ItchClaim/ItchSale.py`

 * *Files identical despite different names*

### Comparing `ItchClaim-1.3/ItchClaim/ItchUser.py` & `ItchClaim-1.3.1/ItchClaim/ItchUser.py`

 * *Files identical despite different names*

### Comparing `ItchClaim-1.3/ItchClaim/__main__.py` & `ItchClaim-1.3.1/ItchClaim/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,17 +63,24 @@
                 resume = int(f.read())
                 print(f'Resuming sale downloads from {resume}')
         except FileNotFoundError:
             print('Resume index not found. Downloading sales from beginning')
 
         DiskManager.get_all_sales(resume)
 
+        print('Updating games from sale lists, to catch updates of already known sales.')
+
+        for category in ['games', 'tools', 'game-assets', 'comics', 'books', 'physical-games',
+                'soundtracks', 'game-mods', 'misc']:
+            print(f'Collecting sales from {category} list')
+            DiskManager.get_all_sale_pages(category=category)
+
     def refresh_library(self):
-        """Refresh the list of owned games of an account. This is used to skip claiming already owned games. Requires login.
-        """
+        """Refresh the list of owned games of an account. This is used to skip claiming already
+        owned games. Requires login."""
         if self.user is None:
             print('You must be logged in')
             return
         self.user.reload_owned_games()
         self.user.save_session()
 
     def claim(self, url: str = 'https://itchclaim.tmbpeter.com/api/active.json'):
```

### Comparing `ItchClaim-1.3/ItchClaim/index.template.html` & `ItchClaim-1.3.1/ItchClaim/index.template.html`

 * *Files 10% similar despite different names*

```diff
@@ -58,14 +58,15 @@
                     </tr>
                     $upcoming_sales_rows
                 </table>
             </div>
             <div class="descriptions">
                 <h2>Last update</h2>
                 <p>$last_update (UTC)</p>
+                <p>Last checked sale: <a href="https://itch.io/s/$last_sale">$last_sale</a></p>
 
                 <h2>Legend</h2>
                 <p>&#x1F310;: Game URL on itch.io</p>
                 <p>&#x1F4DC;: Details about the game in JSON format</p>
                 <p>&#x2714;: Claimable game</p>
                 <p>&#x274C;: Download only game</p>
                 <p>&#x1F551;: Claimability unknown</p>
@@ -81,13 +82,14 @@
 
                 <h2>Legal</h2>
                 <p>Copyright (c) 2022-2023 P&#xE9;ter Tombor.<br>
                 Released under The MIT License (MIT)<br>
                 Please read the <a href="https://github.com/Smart123s/ItchClaim/blob/master/LICENSE.txt">full license</a>.</p>
                 <p>Game and sales data are collected from <a href="https://itch.io">itch.io</a>.<br>
                 The data shown on this site may be inaccurate.<br>
-                Please read the license for legal disclaimers.
+                Please read the license for legal disclaimers.<br>
+                This site is not affiliated with Itch Corp.
                 </p>
             </div>
         </main>
     </body>
 </html>
```

#### html2text {}

```diff
@@ -2,14 +2,15 @@
 ****** Itch.io Free Games ******
 ***** Active sales *****
 Name Sale end (UTC)
 ***** Upcoming sales *****
 Name Sale start (UTC)
 ***** Last update *****
 $last_update (UTC)
+Last checked sale: $last_sale
 ***** Legend *****
 &#x1F310;: Game URL on itch.io
 &#x1F4DC;: Details about the game in JSON format
 &#x2714;: Claimable game
 &#x274C;: Download only game
 &#x1F551;: Claimability unknown
 &#x1F947;: First time on sale
@@ -22,7 +23,8 @@
 ***** Legal *****
 Copyright (c) 2022-2023 P&#xE9;ter Tombor.
 Released under The MIT License (MIT)
 Please read the full_license.
 Game and sales data are collected from itch.io.
 The data shown on this site may be inaccurate.
 Please read the license for legal disclaimers.
+This site is not affiliated with Itch Corp.
```

### Comparing `ItchClaim-1.3/ItchClaim/web.py` & `ItchClaim-1.3.1/ItchClaim/web.py`

 * *Files 8% similar despite different names*

```diff
@@ -117,156 +117,172 @@
 00000740: 706b 675f 7265 736f 7572 6365 732e 7265  pkg_resources.re
 00000750: 6164 5f74 6578 7428 5f5f 7061 636b 6167  ad_text(__packag
 00000760: 655f 5f2c 2027 696e 6465 782e 7465 6d70  e__, 'index.temp
 00000770: 6c61 7465 2e68 746d 6c27 2929 0a20 2020  late.html')).   
 00000780: 2067 616d 6573 2e73 6f72 7428 6b65 793d   games.sort(key=
 00000790: 6c61 6d62 6461 2061 3a20 282d 312a 612e  lambda a: (-1*a.
 000007a0: 7361 6c65 735b 2d31 5d2e 6964 2c20 612e  sales[-1].id, a.
-000007b0: 6e61 6d65 2929 0a0a 2020 2020 2320 3d3d  name))..    # ==
-000007c0: 3d3d 3d3d 3d20 4854 4d4c 203d 3d3d 3d3d  ===== HTML =====
-000007d0: 3d3d 0a0a 2020 2020 6163 7469 7665 5f73  ==..    active_s
-000007e0: 616c 6573 203d 206c 6973 7428 6669 6c74  ales = list(filt
-000007f0: 6572 286c 616d 6264 6120 6761 6d65 3a20  er(lambda game: 
-00000800: 6761 6d65 2e61 6374 6976 655f 7361 6c65  game.active_sale
-00000810: 2c20 6761 6d65 7329 290a 2020 2020 6163  , games)).    ac
-00000820: 7469 7665 5f73 616c 6573 5f72 6f77 7320  tive_sales_rows 
-00000830: 3d20 6765 6e65 7261 7465 5f72 6f77 7328  = generate_rows(
-00000840: 6163 7469 7665 5f73 616c 6573 2c20 2761  active_sales, 'a
-00000850: 6374 6976 6527 290a 0a20 2020 2075 7063  ctive')..    upc
-00000860: 6f6d 696e 675f 7361 6c65 7320 3d20 6c69  oming_sales = li
-00000870: 7374 2866 696c 7465 7228 6c61 6d62 6461  st(filter(lambda
-00000880: 2067 616d 653a 2067 616d 652e 6c61 7374   game: game.last
-00000890: 5f75 7063 6f6d 696e 675f 7361 6c65 2c20  _upcoming_sale, 
-000008a0: 6761 6d65 7329 290a 2020 2020 7570 636f  games)).    upco
-000008b0: 6d69 6e67 5f73 616c 6573 5f72 6f77 7320  ming_sales_rows 
-000008c0: 3d20 6765 6e65 7261 7465 5f72 6f77 7328  = generate_rows(
-000008d0: 7570 636f 6d69 6e67 5f73 616c 6573 2c20  upcoming_sales, 
-000008e0: 2775 7063 6f6d 696e 6727 290a 0a20 2020  'upcoming')..   
-000008f0: 2068 746d 6c20 3d20 7465 6d70 6c61 7465   html = template
-00000900: 2e73 7562 7374 6974 7574 6528 0a20 2020  .substitute(.   
-00000910: 2020 2020 2020 2020 2061 6374 6976 655f           active_
-00000920: 7361 6c65 735f 726f 7773 203d 2027 5c6e  sales_rows = '\n
-00000930: 272e 6a6f 696e 2861 6374 6976 655f 7361  '.join(active_sa
-00000940: 6c65 735f 726f 7773 292c 0a20 2020 2020  les_rows),.     
-00000950: 2020 2020 2020 2075 7063 6f6d 696e 675f         upcoming_
-00000960: 7361 6c65 735f 726f 7773 203d 2027 5c6e  sales_rows = '\n
-00000970: 272e 6a6f 696e 2875 7063 6f6d 696e 675f  '.join(upcoming_
-00000980: 7361 6c65 735f 726f 7773 292c 0a20 2020  sales_rows),.   
-00000990: 2020 2020 2020 2020 206c 6173 745f 7570           last_up
-000009a0: 6461 7465 203d 2064 6174 6574 696d 652e  date = datetime.
-000009b0: 6e6f 7728 292e 7374 7266 7469 6d65 2844  now().strftime(D
-000009c0: 4154 455f 464f 524d 4154 292c 0a20 2020  ATE_FORMAT),.   
-000009d0: 2020 2020 2029 0a0a 2020 2020 7769 7468       )..    with
-000009e0: 206f 7065 6e28 6f73 2e70 6174 682e 6a6f   open(os.path.jo
-000009f0: 696e 2877 6562 5f64 6972 2c20 2769 6e64  in(web_dir, 'ind
-00000a00: 6578 2e68 746d 6c27 292c 2027 7727 2c20  ex.html'), 'w', 
-00000a10: 656e 636f 6469 6e67 3d22 7574 662d 3822  encoding="utf-8"
-00000a20: 2920 6173 2066 3a0a 2020 2020 2020 2020  ) as f:.        
-00000a30: 662e 7772 6974 6528 6874 6d6c 290a 0a20  f.write(html).. 
-00000a40: 2020 2023 203d 3d3d 3d3d 3d3d 204a 534f     # ======= JSO
-00000a50: 4e20 2861 6374 6976 6520 7361 6c65 7329  N (active sales)
-00000a60: 203d 3d3d 3d3d 3d3d 0a20 2020 2061 6374   =======.    act
-00000a70: 6976 655f 7361 6c65 735f 6d69 6e20 3d20  ive_sales_min = 
-00000a80: 5b20 6761 6d65 2e73 6572 6961 6c69 7a65  [ game.serialize
-00000a90: 5f6d 696e 2829 2066 6f72 2067 616d 6520  _min() for game 
-00000aa0: 696e 2061 6374 6976 655f 7361 6c65 7320  in active_sales 
-00000ab0: 5d0a 2020 2020 7769 7468 206f 7065 6e28  ].    with open(
-00000ac0: 6f73 2e70 6174 682e 6a6f 696e 2877 6562  os.path.join(web
-00000ad0: 5f64 6972 2c20 2761 7069 272c 2027 6163  _dir, 'api', 'ac
-00000ae0: 7469 7665 2e6a 736f 6e27 292c 2027 7727  tive.json'), 'w'
-00000af0: 2c20 656e 636f 6469 6e67 3d22 7574 662d  , encoding="utf-
-00000b00: 3822 2920 6173 2066 3a0a 2020 2020 2020  8") as f:.      
-00000b10: 2020 662e 7772 6974 6528 6a73 6f6e 2e64    f.write(json.d
-00000b20: 756d 7073 2861 6374 6976 655f 7361 6c65  umps(active_sale
-00000b30: 735f 6d69 6e29 290a 0a20 2020 2023 203d  s_min))..    # =
-00000b40: 3d3d 3d3d 3d3d 204a 534f 4e20 2875 7063  ====== JSON (upc
-00000b50: 6f6d 696e 6720 7361 6c65 7329 203d 3d3d  oming sales) ===
-00000b60: 3d3d 3d3d 0a20 2020 2075 7063 6f6d 696e  ====.    upcomin
-00000b70: 675f 7361 6c65 735f 6d69 6e20 3d20 5b20  g_sales_min = [ 
-00000b80: 6761 6d65 2e73 6572 6961 6c69 7a65 5f6d  game.serialize_m
-00000b90: 696e 2829 2066 6f72 2067 616d 6520 696e  in() for game in
-00000ba0: 2075 7063 6f6d 696e 675f 7361 6c65 7320   upcoming_sales 
-00000bb0: 5d0a 2020 2020 7769 7468 206f 7065 6e28  ].    with open(
-00000bc0: 6f73 2e70 6174 682e 6a6f 696e 2877 6562  os.path.join(web
-00000bd0: 5f64 6972 2c20 2761 7069 272c 2027 7570  _dir, 'api', 'up
-00000be0: 636f 6d69 6e67 2e6a 736f 6e27 292c 2027  coming.json'), '
-00000bf0: 7727 2c20 656e 636f 6469 6e67 3d22 7574  w', encoding="ut
-00000c00: 662d 3822 2920 6173 2066 3a0a 2020 2020  f-8") as f:.    
-00000c10: 2020 2020 662e 7772 6974 6528 6a73 6f6e      f.write(json
-00000c20: 2e64 756d 7073 2875 7063 6f6d 696e 675f  .dumps(upcoming_
-00000c30: 7361 6c65 735f 6d69 6e29 290a 0a20 2020  sales_min))..   
-00000c40: 2023 203d 3d3d 3d3d 3d3d 204a 534f 4e20   # ======= JSON 
-00000c50: 2861 6c6c 2073 616c 6573 2920 3d3d 3d3d  (all sales) ====
-00000c60: 3d3d 3d0a 2020 2020 616c 6c5f 6d69 6e20  ===.    all_min 
-00000c70: 3d20 5b20 6761 6d65 2e73 6572 6961 6c69  = [ game.seriali
-00000c80: 7a65 5f6d 696e 2829 2066 6f72 2067 616d  ze_min() for gam
-00000c90: 6520 696e 2067 616d 6573 205d 0a20 2020  e in games ].   
-00000ca0: 2077 6974 6820 6f70 656e 286f 732e 7061   with open(os.pa
-00000cb0: 7468 2e6a 6f69 6e28 7765 625f 6469 722c  th.join(web_dir,
-00000cc0: 2027 6170 6927 2c20 2761 6c6c 2e6a 736f   'api', 'all.jso
-00000cd0: 6e27 292c 2027 7727 2c20 656e 636f 6469  n'), 'w', encodi
-00000ce0: 6e67 3d22 7574 662d 3822 2920 6173 2066  ng="utf-8") as f
-00000cf0: 3a0a 2020 2020 2020 2020 662e 7772 6974  :.        f.writ
-00000d00: 6528 6a73 6f6e 2e64 756d 7073 2861 6c6c  e(json.dumps(all
-00000d10: 5f6d 696e 2929 0a0a 6465 6620 6765 6e65  _min))..def gene
-00000d20: 7261 7465 5f72 6f77 7328 6761 6d65 733a  rate_rows(games:
-00000d30: 204c 6973 745b 4974 6368 4761 6d65 5d2c   List[ItchGame],
-00000d40: 2074 7970 653a 2073 7472 2920 2d3e 204c   type: str) -> L
-00000d50: 6973 745b 7374 725d 3a0a 2020 2020 726f  ist[str]:.    ro
-00000d60: 7773 3a20 4c69 7374 5b73 7472 5d20 3d20  ws: List[str] = 
-00000d70: 5b5d 0a20 2020 2066 6f72 2067 616d 6520  [].    for game 
-00000d80: 696e 2067 616d 6573 3a0a 2020 2020 2020  in games:.      
-00000d90: 2020 6966 2067 616d 652e 636c 6169 6d61    if game.claima
-00000da0: 626c 6520 3d3d 2046 616c 7365 3a0a 2020  ble == False:.  
-00000db0: 2020 2020 2020 2020 2020 636c 6169 6d61            claima
-00000dc0: 626c 655f 7465 7874 203d 2027 4e6f 7420  ble_text = 'Not 
-00000dd0: 636c 6169 6d61 626c 6527 0a20 2020 2020  claimable'.     
-00000de0: 2020 2020 2020 2063 6c61 696d 6162 6c65         claimable
-00000df0: 5f69 636f 6e20 3d20 2726 2378 3237 3443  _icon = '&#x274C
-00000e00: 3b27 0a20 2020 2020 2020 2065 6c69 6620  ;'.        elif 
-00000e10: 6761 6d65 2e63 6c61 696d 6162 6c65 203d  game.claimable =
-00000e20: 3d20 5472 7565 3a0a 2020 2020 2020 2020  = True:.        
-00000e30: 2020 2020 636c 6169 6d61 626c 655f 7465      claimable_te
-00000e40: 7874 203d 2027 636c 6169 6d61 626c 6527  xt = 'claimable'
-00000e50: 0a20 2020 2020 2020 2020 2020 2063 6c61  .            cla
-00000e60: 696d 6162 6c65 5f69 636f 6e20 3d20 2726  imable_icon = '&
-00000e70: 2378 3237 3134 3b27 0a20 2020 2020 2020  #x2714;'.       
-00000e80: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00000e90: 2020 2063 6c61 696d 6162 6c65 5f74 6578     claimable_tex
-00000ea0: 7420 3d20 2755 6e6b 6e6f 776e 270a 2020  t = 'Unknown'.  
-00000eb0: 2020 2020 2020 2020 2020 636c 6169 6d61            claima
-00000ec0: 626c 655f 6963 6f6e 203d 2027 2623 7831  ble_icon = '&#x1
-00000ed0: 4635 3531 3b27 0a20 2020 2020 2020 200a  F551;'.        .
-00000ee0: 2020 2020 2020 2020 6966 2074 7970 6520          if type 
-00000ef0: 3d3d 2027 6163 7469 7665 273a 0a20 2020  == 'active':.   
-00000f00: 2020 2020 2020 2020 2073 616c 655f 6461           sale_da
-00000f10: 7465 203d 2067 616d 652e 6163 7469 7665  te = game.active
-00000f20: 5f73 616c 652e 656e 640a 2020 2020 2020  _sale.end.      
-00000f30: 2020 656c 6966 2074 7970 6520 3d3d 2027    elif type == '
-00000f40: 7570 636f 6d69 6e67 273a 0a20 2020 2020  upcoming':.     
-00000f50: 2020 2020 2020 2073 616c 655f 6461 7465         sale_date
-00000f60: 203d 2067 616d 652e 6c61 7374 5f75 7063   = game.last_upc
-00000f70: 6f6d 696e 675f 7361 6c65 2e73 7461 7274  oming_sale.start
-00000f80: 0a0a 2020 2020 2020 2020 726f 7773 2e61  ..        rows.a
-00000f90: 7070 656e 6428 524f 575f 5445 4d50 4c41  ppend(ROW_TEMPLA
-00000fa0: 5445 2e73 7562 7374 6974 7574 6528 0a20  TE.substitute(. 
-00000fb0: 2020 2020 2020 2020 2020 206e 616d 6520             name 
-00000fc0: 3d20 6761 6d65 2e6e 616d 652c 0a20 2020  = game.name,.   
-00000fd0: 2020 2020 2020 2020 2073 616c 655f 6461           sale_da
-00000fe0: 7465 203d 2073 616c 655f 6461 7465 2e73  te = sale_date.s
-00000ff0: 7472 6674 696d 6528 4441 5445 5f46 4f52  trftime(DATE_FOR
-00001000: 4d41 5429 2c0a 2020 2020 2020 2020 2020  MAT),.          
-00001010: 2020 6669 7273 745f 7361 6c65 203d 2027    first_sale = '
-00001020: 2623 7831 4639 3437 3b27 2069 6620 6761  &#x1F947;' if ga
-00001030: 6d65 2e69 735f 6669 7273 745f 7361 6c65  me.is_first_sale
-00001040: 2065 6c73 6520 2727 2c0a 2020 2020 2020   else '',.      
-00001050: 2020 2020 2020 636c 6169 6d61 626c 655f        claimable_
-00001060: 7465 7874 203d 2063 6c61 696d 6162 6c65  text = claimable
-00001070: 5f74 6578 742c 0a20 2020 2020 2020 2020  _text,.         
-00001080: 2020 2063 6c61 696d 6162 6c65 5f69 636f     claimable_ico
-00001090: 6e20 3d20 636c 6169 6d61 626c 655f 6963  n = claimable_ic
-000010a0: 6f6e 2c0a 2020 2020 2020 2020 2020 2020  on,.            
-000010b0: 7572 6c20 3d20 6761 6d65 2e75 726c 2c0a  url = game.url,.
-000010c0: 2020 2020 2020 2020 2020 2020 6964 203d              id =
-000010d0: 2067 616d 652e 6964 2c0a 2020 2020 2020   game.id,.      
-000010e0: 2020 2929 0a20 2020 2072 6574 7572 6e20    )).    return 
-000010f0: 726f 7773 0a                             rows.
+000007b0: 6e61 6d65 2929 0a0a 2020 2020 2320 4c6f  name))..    # Lo
+000007c0: 6164 2072 6573 756d 6520 696e 6465 780a  ad resume index.
+000007d0: 0a20 2020 2074 7279 3a0a 2020 2020 2020  .    try:.      
+000007e0: 2020 7769 7468 206f 7065 6e28 6f73 2e70    with open(os.p
+000007f0: 6174 682e 6a6f 696e 2877 6562 5f64 6972  ath.join(web_dir
+00000800: 2c20 2764 6174 6127 2c20 2772 6573 756d  , 'data', 'resum
+00000810: 655f 696e 6465 782e 7478 7427 292c 2027  e_index.txt'), '
+00000820: 7227 2c20 656e 636f 6469 6e67 3d27 7574  r', encoding='ut
+00000830: 662d 3827 2920 6173 2066 3a0a 2020 2020  f-8') as f:.    
+00000840: 2020 2020 2020 2020 7265 7375 6d65 5f69          resume_i
+00000850: 6e64 6578 203d 2069 6e74 2866 2e72 6561  ndex = int(f.rea
+00000860: 6428 2929 0a20 2020 2065 7863 6570 7420  d()).    except 
+00000870: 4669 6c65 4e6f 7446 6f75 6e64 4572 726f  FileNotFoundErro
+00000880: 723a 0a20 2020 2020 2020 2072 6573 756d  r:.        resum
+00000890: 655f 696e 6465 7820 3d20 300a 0a20 2020  e_index = 0..   
+000008a0: 2023 203d 3d3d 3d3d 3d3d 2048 544d 4c20   # ======= HTML 
+000008b0: 3d3d 3d3d 3d3d 3d0a 0a20 2020 2061 6374  =======..    act
+000008c0: 6976 655f 7361 6c65 7320 3d20 6c69 7374  ive_sales = list
+000008d0: 2866 696c 7465 7228 6c61 6d62 6461 2067  (filter(lambda g
+000008e0: 616d 653a 2067 616d 652e 6163 7469 7665  ame: game.active
+000008f0: 5f73 616c 652c 2067 616d 6573 2929 0a20  _sale, games)). 
+00000900: 2020 2061 6374 6976 655f 7361 6c65 735f     active_sales_
+00000910: 726f 7773 203d 2067 656e 6572 6174 655f  rows = generate_
+00000920: 726f 7773 2861 6374 6976 655f 7361 6c65  rows(active_sale
+00000930: 732c 2027 6163 7469 7665 2729 0a0a 2020  s, 'active')..  
+00000940: 2020 7570 636f 6d69 6e67 5f73 616c 6573    upcoming_sales
+00000950: 203d 206c 6973 7428 6669 6c74 6572 286c   = list(filter(l
+00000960: 616d 6264 6120 6761 6d65 3a20 6761 6d65  ambda game: game
+00000970: 2e6c 6173 745f 7570 636f 6d69 6e67 5f73  .last_upcoming_s
+00000980: 616c 652c 2067 616d 6573 2929 0a20 2020  ale, games)).   
+00000990: 2075 7063 6f6d 696e 675f 7361 6c65 735f   upcoming_sales_
+000009a0: 726f 7773 203d 2067 656e 6572 6174 655f  rows = generate_
+000009b0: 726f 7773 2875 7063 6f6d 696e 675f 7361  rows(upcoming_sa
+000009c0: 6c65 732c 2027 7570 636f 6d69 6e67 2729  les, 'upcoming')
+000009d0: 0a0a 2020 2020 6874 6d6c 203d 2074 656d  ..    html = tem
+000009e0: 706c 6174 652e 7375 6273 7469 7475 7465  plate.substitute
+000009f0: 280a 2020 2020 2020 2020 2020 2020 6163  (.            ac
+00000a00: 7469 7665 5f73 616c 6573 5f72 6f77 7320  tive_sales_rows 
+00000a10: 3d20 275c 6e27 2e6a 6f69 6e28 6163 7469  = '\n'.join(acti
+00000a20: 7665 5f73 616c 6573 5f72 6f77 7329 2c0a  ve_sales_rows),.
+00000a30: 2020 2020 2020 2020 2020 2020 7570 636f              upco
+00000a40: 6d69 6e67 5f73 616c 6573 5f72 6f77 7320  ming_sales_rows 
+00000a50: 3d20 275c 6e27 2e6a 6f69 6e28 7570 636f  = '\n'.join(upco
+00000a60: 6d69 6e67 5f73 616c 6573 5f72 6f77 7329  ming_sales_rows)
+00000a70: 2c0a 2020 2020 2020 2020 2020 2020 6c61  ,.            la
+00000a80: 7374 5f75 7064 6174 6520 3d20 6461 7465  st_update = date
+00000a90: 7469 6d65 2e6e 6f77 2829 2e73 7472 6674  time.now().strft
+00000aa0: 696d 6528 4441 5445 5f46 4f52 4d41 5429  ime(DATE_FORMAT)
+00000ab0: 2c0a 2020 2020 2020 2020 2020 2020 6c61  ,.            la
+00000ac0: 7374 5f73 616c 6520 3d20 7265 7375 6d65  st_sale = resume
+00000ad0: 5f69 6e64 6578 2c0a 2020 2020 2020 2020  _index,.        
+00000ae0: 290a 0a20 2020 2077 6974 6820 6f70 656e  )..    with open
+00000af0: 286f 732e 7061 7468 2e6a 6f69 6e28 7765  (os.path.join(we
+00000b00: 625f 6469 722c 2027 696e 6465 782e 6874  b_dir, 'index.ht
+00000b10: 6d6c 2729 2c20 2777 272c 2065 6e63 6f64  ml'), 'w', encod
+00000b20: 696e 673d 2275 7466 2d38 2229 2061 7320  ing="utf-8") as 
+00000b30: 663a 0a20 2020 2020 2020 2066 2e77 7269  f:.        f.wri
+00000b40: 7465 2868 746d 6c29 0a0a 2020 2020 2320  te(html)..    # 
+00000b50: 3d3d 3d3d 3d3d 3d20 4a53 4f4e 2028 6163  ======= JSON (ac
+00000b60: 7469 7665 2073 616c 6573 2920 3d3d 3d3d  tive sales) ====
+00000b70: 3d3d 3d0a 2020 2020 6163 7469 7665 5f73  ===.    active_s
+00000b80: 616c 6573 5f6d 696e 203d 205b 2067 616d  ales_min = [ gam
+00000b90: 652e 7365 7269 616c 697a 655f 6d69 6e28  e.serialize_min(
+00000ba0: 2920 666f 7220 6761 6d65 2069 6e20 6163  ) for game in ac
+00000bb0: 7469 7665 5f73 616c 6573 205d 0a20 2020  tive_sales ].   
+00000bc0: 2077 6974 6820 6f70 656e 286f 732e 7061   with open(os.pa
+00000bd0: 7468 2e6a 6f69 6e28 7765 625f 6469 722c  th.join(web_dir,
+00000be0: 2027 6170 6927 2c20 2761 6374 6976 652e   'api', 'active.
+00000bf0: 6a73 6f6e 2729 2c20 2777 272c 2065 6e63  json'), 'w', enc
+00000c00: 6f64 696e 673d 2275 7466 2d38 2229 2061  oding="utf-8") a
+00000c10: 7320 663a 0a20 2020 2020 2020 2066 2e77  s f:.        f.w
+00000c20: 7269 7465 286a 736f 6e2e 6475 6d70 7328  rite(json.dumps(
+00000c30: 6163 7469 7665 5f73 616c 6573 5f6d 696e  active_sales_min
+00000c40: 2929 0a0a 2020 2020 2320 3d3d 3d3d 3d3d  ))..    # ======
+00000c50: 3d20 4a53 4f4e 2028 7570 636f 6d69 6e67  = JSON (upcoming
+00000c60: 2073 616c 6573 2920 3d3d 3d3d 3d3d 3d0a   sales) =======.
+00000c70: 2020 2020 7570 636f 6d69 6e67 5f73 616c      upcoming_sal
+00000c80: 6573 5f6d 696e 203d 205b 2067 616d 652e  es_min = [ game.
+00000c90: 7365 7269 616c 697a 655f 6d69 6e28 2920  serialize_min() 
+00000ca0: 666f 7220 6761 6d65 2069 6e20 7570 636f  for game in upco
+00000cb0: 6d69 6e67 5f73 616c 6573 205d 0a20 2020  ming_sales ].   
+00000cc0: 2077 6974 6820 6f70 656e 286f 732e 7061   with open(os.pa
+00000cd0: 7468 2e6a 6f69 6e28 7765 625f 6469 722c  th.join(web_dir,
+00000ce0: 2027 6170 6927 2c20 2775 7063 6f6d 696e   'api', 'upcomin
+00000cf0: 672e 6a73 6f6e 2729 2c20 2777 272c 2065  g.json'), 'w', e
+00000d00: 6e63 6f64 696e 673d 2275 7466 2d38 2229  ncoding="utf-8")
+00000d10: 2061 7320 663a 0a20 2020 2020 2020 2066   as f:.        f
+00000d20: 2e77 7269 7465 286a 736f 6e2e 6475 6d70  .write(json.dump
+00000d30: 7328 7570 636f 6d69 6e67 5f73 616c 6573  s(upcoming_sales
+00000d40: 5f6d 696e 2929 0a0a 2020 2020 2320 3d3d  _min))..    # ==
+00000d50: 3d3d 3d3d 3d20 4a53 4f4e 2028 616c 6c20  ===== JSON (all 
+00000d60: 7361 6c65 7329 203d 3d3d 3d3d 3d3d 0a20  sales) =======. 
+00000d70: 2020 2061 6c6c 5f6d 696e 203d 205b 2067     all_min = [ g
+00000d80: 616d 652e 7365 7269 616c 697a 655f 6d69  ame.serialize_mi
+00000d90: 6e28 2920 666f 7220 6761 6d65 2069 6e20  n() for game in 
+00000da0: 6761 6d65 7320 5d0a 2020 2020 7769 7468  games ].    with
+00000db0: 206f 7065 6e28 6f73 2e70 6174 682e 6a6f   open(os.path.jo
+00000dc0: 696e 2877 6562 5f64 6972 2c20 2761 7069  in(web_dir, 'api
+00000dd0: 272c 2027 616c 6c2e 6a73 6f6e 2729 2c20  ', 'all.json'), 
+00000de0: 2777 272c 2065 6e63 6f64 696e 673d 2275  'w', encoding="u
+00000df0: 7466 2d38 2229 2061 7320 663a 0a20 2020  tf-8") as f:.   
+00000e00: 2020 2020 2066 2e77 7269 7465 286a 736f       f.write(jso
+00000e10: 6e2e 6475 6d70 7328 616c 6c5f 6d69 6e29  n.dumps(all_min)
+00000e20: 290a 0a64 6566 2067 656e 6572 6174 655f  )..def generate_
+00000e30: 726f 7773 2867 616d 6573 3a20 4c69 7374  rows(games: List
+00000e40: 5b49 7463 6847 616d 655d 2c20 7479 7065  [ItchGame], type
+00000e50: 3a20 7374 7229 202d 3e20 4c69 7374 5b73  : str) -> List[s
+00000e60: 7472 5d3a 0a20 2020 2072 6f77 733a 204c  tr]:.    rows: L
+00000e70: 6973 745b 7374 725d 203d 205b 5d0a 2020  ist[str] = [].  
+00000e80: 2020 666f 7220 6761 6d65 2069 6e20 6761    for game in ga
+00000e90: 6d65 733a 0a20 2020 2020 2020 2069 6620  mes:.        if 
+00000ea0: 6761 6d65 2e63 6c61 696d 6162 6c65 203d  game.claimable =
+00000eb0: 3d20 4661 6c73 653a 0a20 2020 2020 2020  = False:.       
+00000ec0: 2020 2020 2063 6c61 696d 6162 6c65 5f74       claimable_t
+00000ed0: 6578 7420 3d20 274e 6f74 2063 6c61 696d  ext = 'Not claim
+00000ee0: 6162 6c65 270a 2020 2020 2020 2020 2020  able'.          
+00000ef0: 2020 636c 6169 6d61 626c 655f 6963 6f6e    claimable_icon
+00000f00: 203d 2027 2623 7832 3734 433b 270a 2020   = '&#x274C;'.  
+00000f10: 2020 2020 2020 656c 6966 2067 616d 652e        elif game.
+00000f20: 636c 6169 6d61 626c 6520 3d3d 2054 7275  claimable == Tru
+00000f30: 653a 0a20 2020 2020 2020 2020 2020 2063  e:.            c
+00000f40: 6c61 696d 6162 6c65 5f74 6578 7420 3d20  laimable_text = 
+00000f50: 2763 6c61 696d 6162 6c65 270a 2020 2020  'claimable'.    
+00000f60: 2020 2020 2020 2020 636c 6169 6d61 626c          claimabl
+00000f70: 655f 6963 6f6e 203d 2027 2623 7832 3731  e_icon = '&#x271
+00000f80: 343b 270a 2020 2020 2020 2020 656c 7365  4;'.        else
+00000f90: 3a0a 2020 2020 2020 2020 2020 2020 636c  :.            cl
+00000fa0: 6169 6d61 626c 655f 7465 7874 203d 2027  aimable_text = '
+00000fb0: 556e 6b6e 6f77 6e27 0a20 2020 2020 2020  Unknown'.       
+00000fc0: 2020 2020 2063 6c61 696d 6162 6c65 5f69       claimable_i
+00000fd0: 636f 6e20 3d20 2726 2378 3146 3535 313b  con = '&#x1F551;
+00000fe0: 270a 2020 2020 2020 2020 0a20 2020 2020  '.        .     
+00000ff0: 2020 2069 6620 7479 7065 203d 3d20 2761     if type == 'a
+00001000: 6374 6976 6527 3a0a 2020 2020 2020 2020  ctive':.        
+00001010: 2020 2020 7361 6c65 5f64 6174 6520 3d20      sale_date = 
+00001020: 6761 6d65 2e61 6374 6976 655f 7361 6c65  game.active_sale
+00001030: 2e65 6e64 0a20 2020 2020 2020 2065 6c69  .end.        eli
+00001040: 6620 7479 7065 203d 3d20 2775 7063 6f6d  f type == 'upcom
+00001050: 696e 6727 3a0a 2020 2020 2020 2020 2020  ing':.          
+00001060: 2020 7361 6c65 5f64 6174 6520 3d20 6761    sale_date = ga
+00001070: 6d65 2e6c 6173 745f 7570 636f 6d69 6e67  me.last_upcoming
+00001080: 5f73 616c 652e 7374 6172 740a 0a20 2020  _sale.start..   
+00001090: 2020 2020 2072 6f77 732e 6170 7065 6e64       rows.append
+000010a0: 2852 4f57 5f54 454d 504c 4154 452e 7375  (ROW_TEMPLATE.su
+000010b0: 6273 7469 7475 7465 280a 2020 2020 2020  bstitute(.      
+000010c0: 2020 2020 2020 6e61 6d65 203d 2067 616d        name = gam
+000010d0: 652e 6e61 6d65 2c0a 2020 2020 2020 2020  e.name,.        
+000010e0: 2020 2020 7361 6c65 5f64 6174 6520 3d20      sale_date = 
+000010f0: 7361 6c65 5f64 6174 652e 7374 7266 7469  sale_date.strfti
+00001100: 6d65 2844 4154 455f 464f 524d 4154 292c  me(DATE_FORMAT),
+00001110: 0a20 2020 2020 2020 2020 2020 2066 6972  .            fir
+00001120: 7374 5f73 616c 6520 3d20 2726 2378 3146  st_sale = '&#x1F
+00001130: 3934 373b 2720 6966 2067 616d 652e 6973  947;' if game.is
+00001140: 5f66 6972 7374 5f73 616c 6520 656c 7365  _first_sale else
+00001150: 2027 272c 0a20 2020 2020 2020 2020 2020   '',.           
+00001160: 2063 6c61 696d 6162 6c65 5f74 6578 7420   claimable_text 
+00001170: 3d20 636c 6169 6d61 626c 655f 7465 7874  = claimable_text
+00001180: 2c0a 2020 2020 2020 2020 2020 2020 636c  ,.            cl
+00001190: 6169 6d61 626c 655f 6963 6f6e 203d 2063  aimable_icon = c
+000011a0: 6c61 696d 6162 6c65 5f69 636f 6e2c 0a20  laimable_icon,. 
+000011b0: 2020 2020 2020 2020 2020 2075 726c 203d             url =
+000011c0: 2067 616d 652e 7572 6c2c 0a20 2020 2020   game.url,.     
+000011d0: 2020 2020 2020 2069 6420 3d20 6761 6d65         id = game
+000011e0: 2e69 642c 0a20 2020 2020 2020 2029 290a  .id,.        )).
+000011f0: 2020 2020 7265 7475 726e 2072 6f77 730a      return rows.
```

### Comparing `ItchClaim-1.3/ItchClaim.egg-info/PKG-INFO` & `ItchClaim-1.3.1/ItchClaim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ItchClaim
-Version: 1.3
+Version: 1.3.1
 Summary: Automatically claim free games from itch.io
 Author: Smart123s
 Project-URL: Homepage, https://github.com/Smart123s/ItchClaim
 Project-URL: Bug Tracker, https://github.com/Smart123s/ItchClaim/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `ItchClaim-1.3/LICENSE.txt` & `ItchClaim-1.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ItchClaim-1.3/PKG-INFO` & `ItchClaim-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ItchClaim
-Version: 1.3
+Version: 1.3.1
 Summary: Automatically claim free games from itch.io
 Author: Smart123s
 Project-URL: Homepage, https://github.com/Smart123s/ItchClaim
 Project-URL: Bug Tracker, https://github.com/Smart123s/ItchClaim/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `ItchClaim-1.3/README.md` & `ItchClaim-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `ItchClaim-1.3/pyproject.toml` & `ItchClaim-1.3.1/pyproject.toml`

 * *Files identical despite different names*

