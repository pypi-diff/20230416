# Comparing `tmp/rsrch-0.1.2.tar.gz` & `tmp/rsrch-0.1.4.tar.gz`

## Comparing `rsrch-0.1.2.tar` & `rsrch-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 rsrch-0.1.2/.DS_Store
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 rsrch-0.1.2/requirements.txt
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 rsrch-0.1.2/examples/yitay.md
--rw-r--r--   0        0        0  2231016 2020-02-02 00:00:00.000000 rsrch-0.1.2/papers/Birdwatch:_Crowd_Wisdom_and_Bridging_Algorithms_can_Inform
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 rsrch-0.1.4/.DS_Store
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 rsrch-0.1.4/requirements.txt
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 rsrch-0.1.4/examples/yitay.md
+-rw-r--r--   0        0        0  2231016 2020-02-02 00:00:00.000000 rsrch-0.1.4/papers/Birdwatch:_Crowd_Wisdom_and_Bridging_Algorithms_can_Inform
 Understanding_and_Reduce_the_Spread_of_Misinformation.pdf
--rw-r--r--   0        0        0   704784 2020-02-02 00:00:00.000000 rsrch-0.1.2/papers/Decision_Transformer:_Reinforcement
+-rw-r--r--   0        0        0   704784 2020-02-02 00:00:00.000000 rsrch-0.1.4/papers/Decision_Transformer:_Reinforcement
 Learning_via_Sequence_Modeling.pdf
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 rsrch-0.1.2/rsrch/__about__.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 rsrch-0.1.2/rsrch/__init__.py
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 rsrch-0.1.2/rsrch/_src/cli.py
--rw-r--r--   0        0        0     4327 2020-02-02 00:00:00.000000 rsrch-0.1.2/rsrch/_src/rsrch.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 rsrch-0.1.2/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 rsrch-0.1.2/LICENSE
--rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 rsrch-0.1.2/README.md
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 rsrch-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     4231 2020-02-02 00:00:00.000000 rsrch-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 rsrch-0.1.4/rsrch/__about__.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 rsrch-0.1.4/rsrch/__init__.py
+-rw-r--r--   0        0        0     4312 2020-02-02 00:00:00.000000 rsrch-0.1.4/rsrch/_src/rsrch.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 rsrch-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 rsrch-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 rsrch-0.1.4/README.md
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 rsrch-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3247 2020-02-02 00:00:00.000000 rsrch-0.1.4/PKG-INFO
```

### Comparing `rsrch-0.1.2/.DS_Store` & `rsrch-0.1.4/.DS_Store`

 * *Files identical despite different names*

### Comparing `rsrch-0.1.2/requirements.txt` & `rsrch-0.1.4/requirements.txt`

 * *Files identical despite different names*

### Comparing `rsrch-0.1.2/papers/Birdwatch:_Crowd_Wisdom_and_Bridging_Algorithms_can_Inform
Understanding_and_Reduce_the_Spread_of_Misinformation.pdf` & `rsrch-0.1.4/papers/Birdwatch:_Crowd_Wisdom_and_Bridging_Algorithms_can_Inform
Understanding_and_Reduce_the_Spread_of_Misinformation.pdf`

 * *Files identical despite different names*

### Comparing `rsrch-0.1.2/papers/Decision_Transformer:_Reinforcement
Learning_via_Sequence_Modeling.pdf` & `rsrch-0.1.4/papers/Decision_Transformer:_Reinforcement
Learning_via_Sequence_Modeling.pdf`

 * *Files identical despite different names*

### Comparing `rsrch-0.1.2/rsrch/_src/rsrch.py` & `rsrch-0.1.4/rsrch/_src/rsrch.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,25 +22,25 @@
             authors = paper["properties"]["Authors"]["rich_text"][0]["plain_text"]
             if not url == None and url.startswith("http"):
                 papers.append((title, url, date, authors))
 
     return papers
 
 
-def download_papers():
+def download():
     print("Downloading papers from Notion...")
     urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
     load_dotenv()
     papers = fetch_table()
 
-    if not os.path.exists("../papers"):
-        os.mkdir("../papers")
+    if not os.path.exists("papers"):
+        os.mkdir("papers")
 
     for title, url, _, _ in papers:
-        path = f"../papers/{title.replace(' ', '_')}.pdf"
+        path = f"papers/{title.replace(' ', '_')}.pdf"
         if not os.path.exists(path):
             print(f'\nDownloading "{title}"')
             try:
                 r = requests.get(url, stream=True, verify=True)
             except requests.exceptions.SSLError:
                 r = requests.get(url, stream=True, verify=False)
 
@@ -88,15 +88,15 @@
             },
         },
     )
 
     print(f"- {title}")
 
 
-def push_papers(arxiv_urls):
+def upload(arxiv_urls):
     load_dotenv()
     notion = Client(auth=os.getenv("NOTION_TOKEN"))
 
     # Extract arXiv IDs from valid URLs
     ids = []
     for url in arxiv_urls:
         if url.startswith("https://arxiv.org/abs/"):
@@ -109,15 +109,15 @@
             print(f"ERROR: {url} is not a valid arXiv abstract URL, PDF URL, or ID.")
 
     # Fetch titles of papers already in Notion
     papers = fetch_table()
     titles = [title for title, _, _, _ in papers]
 
     # Fetch paper data from arXiv
-    print("Pushing papers to Notion...")
+    print("Uploading papers to Notion...\n")
     results = arxiv.Search(id_list=ids)
     for paper in results.results():
         # Date is in ISO 8601 format, e.g. 2020-01-01
         date = paper.published.isoformat().split("T")[0]
 
         # Paper title
         title = paper.title
@@ -134,8 +134,8 @@
 
         # Create paper in Notion if it doesn't already exist
         if title not in titles:
             create_paper(notion, title, pdf_url, date, authors)
         else:
             print(f"- {title} (already exists)")
 
-    print("Done!")
+    print("\nDone!")
```

### Comparing `rsrch-0.1.2/LICENSE` & `rsrch-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rsrch-0.1.2/README.md` & `rsrch-0.1.4/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,30 @@
+Metadata-Version: 2.1
+Name: rsrch
+Version: 0.1.4
+Summary: Manage your ever-growing list of research papers
+Project-URL: Homepage, https://github.com/ishan0102/rsrch
+Project-URL: Bug Tracker, https://github.com/ishan0102/rsrch/issues
+Author-email: Ishan Shah <ishan0102@utexas.edu>
+License-File: LICENSE
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Requires-Dist: arxiv==1.4.2
+Requires-Dist: click==8.1.3
+Requires-Dist: notion-client==2.0.0
+Requires-Dist: python-dotenv==0.21.0
+Requires-Dist: requests==2.28.1
+Requires-Dist: tqdm==4.64.1
+Requires-Dist: urllib3==1.26.13
+Description-Content-Type: text/markdown
+
 # rsrch
-Manage your research papers through your CLI. This project lets you update a Notion database with arXiv links and download PDFs of papers to your local machine.
+Manage your research papers from the command line. This project lets you update a Notion database with arXiv links and download PDFs of papers to your local machine.
 
 <p align="center">
     <img width="1095" alt="image" src="https://user-images.githubusercontent.com/47067154/219932040-ab4962f8-b01e-4d94-9eba-77a155b0e933.png">
 </p>
 
 ## Installation
 1. Create an [internal integration](https://www.notion.so/help/create-integrations-with-the-notion-api) in Notion.
@@ -17,90 +38,52 @@
     NOTION_DATABASE_ID=XXXXXXXXXXXXXXXX
     ```
     Your `NOTION_TOKEN` can be found in your [integrations page](https://www.notion.so/my-integrations) and is called the **Internal Integration Token**. The `NOTION_DATABASE_ID` can be found in the [URL of your database](https://www.notion.so/my-integrations) (`https://www.notion.so/{workspace_name}/{database_id}?v={view_id}`).
 
 4. Install local dependencies:
 
     ```bash
-    python3 -m venv venv
-    pip install -r requirements.txt
+    pip install rsrch
     ```
 
 5. **Important**: Your Notion database must have the following columns with the corresponding types:
     - **Title**: `Title`
     - **URL**: `URL`
     - **Date**: `Date`
     - **Authors**: `Text`
 
     You can add more columns, but these are the ones that are required.
 
 ## Usage
-Activate the virtual environment:
-
-```bash
-source venv/bin/activate
-```
-
 ### Download
 This will download all the papers from your Notion database to the `papers/` directory.
 
-```bash
-cd src
-python cli.py download
+```python
+from rsrch import download
+download()
 ```
 
 <p>
-    <img width="1097" alt="image" src="https://user-images.githubusercontent.com/47067154/219932318-54b37a51-850f-4ab2-b916-43361816fa91.png">
+    <img width="1097" alt="image" src="https://user-images.githubusercontent.com/47067154/232264456-4bdef487-36e8-4627-95c3-82f5c3876082.png">
 </p>
 
-### Push
-You can push arXiv abstract links, PDF links, or IDs to your Notion database and have it autofill all of the relevant fields.
+### Upload
+You can upload arXiv abstract links, PDF links, or IDs to your Notion database and have it autofill all of the relevant fields.
 
-```bash
-cd src
-python cli.py push https://arxiv.org/abs/1706.03762
+```python
+from rsrch import upload
+upload()
 ```
 
 <p>
-    <img width="1095" alt="image" src="https://user-images.githubusercontent.com/47067154/219932341-a44ff798-3fd0-46f8-8a43-3a22b5dcdcf8.png">
+    <img width="1095" alt="image" src="https://user-images.githubusercontent.com/47067154/232264615-82b42d8c-ca1c-4f21-899f-439a6c8a7879.png">
 </p>
 
 Alternatively, you can add non-arXiv links manually to Notion.
 
 
 ## Notes
 - Uploading papers to Notion is currently only supported for arXiv links. Papers with titles that already exist in the database will not be uploaded.
-- The script will download the PDFs to the `papers/` directory. If you want to change this, you can change the `path` variable in `main.py`.
 - I plan on adding support for other databases in the future, but for now it only works with Notion databases.
 
-### Bash Functions
-For those of us that use the command line a lot, you can add the following functions to your `.bashrc` file to make it easier to use:
-
-#### Download any new research papers
-```bash
-function get_papers() {
-    # Go to rsrch directory
-    cd ~/Documents/projects/rsrch
-
-    # Download papers
-    source venv/bin/activate
-    python src/cli.py download
-    cd papers
-}
-```
-
-#### Push any new research papers
-```bash
-function add_papers() {
-    # Go to rsrch directory
-    cd ~/Documents/projects/rsrch
-
-    # Push papers
-    source venv/bin/activate
-    python src/cli.py push $*
-}
-```
-
-Now you can just run `get_papers` or `add_papers` with `N` arXiv links to download or push papers to your Notion database!
-
 ### Resources
 - [Notion API](https://developers.notion.com/)
```

### Comparing `rsrch-0.1.2/pyproject.toml` & `rsrch-0.1.4/pyproject.toml`

 * *Files identical despite different names*

