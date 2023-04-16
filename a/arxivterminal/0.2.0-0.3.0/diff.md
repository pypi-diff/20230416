# Comparing `tmp/arxivterminal-0.2.0.tar.gz` & `tmp/arxivterminal-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arxivterminal-0.2.0.tar", max compression
+gzip compressed data, was "arxivterminal-0.3.0.tar", max compression
```

## Comparing `arxivterminal-0.2.0.tar` & `arxivterminal-0.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    35149 2023-04-15 01:36:31.930555 arxivterminal-0.2.0/LICENSE
--rw-r--r--   0        0        0     3229 2023-04-15 07:14:41.405271 arxivterminal-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-04-15 06:44:50.310227 arxivterminal-0.2.0/arxivterminal/__init__.py
--rw-r--r--   0        0        0     3864 2023-04-15 07:14:41.405840 arxivterminal-0.2.0/arxivterminal/cli.py
--rw-r--r--   0        0        0      349 2023-04-15 07:14:41.406231 arxivterminal-0.2.0/arxivterminal/constants.py
--rw-r--r--   0        0        0     9486 2023-04-15 07:14:41.406551 arxivterminal-0.2.0/arxivterminal/db.py
--rw-r--r--   0        0        0     2171 2023-04-15 06:44:47.860863 arxivterminal-0.2.0/arxivterminal/fetch.py
--rw-r--r--   0        0        0     5222 2023-04-15 07:14:41.406823 arxivterminal-0.2.0/arxivterminal/ml.py
--rw-r--r--   0        0        0      322 2023-04-15 01:16:03.622287 arxivterminal-0.2.0/arxivterminal/models.py
--rw-r--r--   0        0        0     3269 2023-04-15 07:14:41.407077 arxivterminal-0.2.0/arxivterminal/output.py
--rw-r--r--   0        0        0      772 2023-04-15 07:14:41.408183 arxivterminal-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4346 1970-01-01 00:00:00.000000 arxivterminal-0.2.0/setup.py
--rw-r--r--   0        0        0     4213 1970-01-01 00:00:00.000000 arxivterminal-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-15 01:36:31.930555 arxivterminal-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3528 2023-04-16 05:33:02.049937 arxivterminal-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-15 06:44:50.310227 arxivterminal-0.3.0/arxivterminal/__init__.py
+-rw-r--r--   0        0        0     3255 2023-04-16 05:33:02.050319 arxivterminal-0.3.0/arxivterminal/cli.py
+-rw-r--r--   0        0        0      349 2023-04-15 07:14:41.406231 arxivterminal-0.3.0/arxivterminal/constants.py
+-rw-r--r--   0        0        0    10279 2023-04-16 05:33:02.050586 arxivterminal-0.3.0/arxivterminal/db.py
+-rw-r--r--   0        0        0     1049 2023-04-16 05:33:02.050891 arxivterminal-0.3.0/arxivterminal/download.py
+-rw-r--r--   0        0        0     2197 2023-04-16 05:33:02.051247 arxivterminal-0.3.0/arxivterminal/fetch.py
+-rw-r--r--   0        0        0     5222 2023-04-15 07:14:41.406823 arxivterminal-0.3.0/arxivterminal/ml.py
+-rw-r--r--   0        0        0      339 2023-04-16 05:33:02.051527 arxivterminal-0.3.0/arxivterminal/models.py
+-rw-r--r--   0        0        0     4656 2023-04-16 05:33:02.051793 arxivterminal-0.3.0/arxivterminal/output.py
+-rw-r--r--   0        0        0      772 2023-04-16 05:33:02.052023 arxivterminal-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4512 1970-01-01 00:00:00.000000 arxivterminal-0.3.0/PKG-INFO
```

### Comparing `arxivterminal-0.2.0/LICENSE` & `arxivterminal-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arxivterminal-0.2.0/README.md` & `arxivterminal-0.3.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # Arxiv Terminal
 ![Tests](https://github.com/jbencina/arxivterminal/actions/workflows/main.yaml/badge.svg)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/arxivterminal)](https://pypi.org/project/arxivterminal)
 
 Arxiv Terminal is a command-line interface (CLI) tool for fetching, searching, and displaying papers from the [arXiv](https://arxiv.org/) preprint repository. The tool allows you to fetch papers from specified categories, search the fetched papers, and display their statistics.
 
 ## Features
 
 - Fetch paper abstracts from specified categories and save them in a local sqllite database.
 - Show fetched papers and interatively open for more detailed abstracts
 - Search fetched papers based on a query (Currently supports pattern + LSA semantic search)
+- Download papers locally as PDF
 
 ![Demo](static/demo.gif)
 
 ## Contributors
 A special call out to ChatGPT (v4) which helped write and modify various code and documentation in this repository.
 
 ## Installation
@@ -55,14 +57,18 @@
 arxiv delete_all
 ```
 
 Show papers fetched in the last 7 days
 
 ```bash
 arxiv show --days-ago 7
+
+# On this screen the user can select a paper for more
+# details by typing a line number. Additional options
+# allow for searching & downloading
 ```
 
 Display statistics of the papers stored in the database:
 
 ```bash
 arxiv stats
 ```
```

### Comparing `arxivterminal-0.2.0/arxivterminal/cli.py` & `arxivterminal-0.3.0/arxivterminal/cli.py`

 * *Files 23% similar despite different names*

```diff
@@ -22,27 +22,20 @@
     logging.getLogger().addHandler(logging.StreamHandler(sys.stdout))
 
 
 @click.command()
 @click.option("--num-days", default=7, help="Number of days to fetch papers.")
 @click.option(
     "--categories",
-    default="cs.AI",
+    default="cs.AI,cs.LG",  # AI and Machine Learning categories
     help="Comma-separated list of categories to fetch papers.",
 )
 def fetch(num_days, categories):
     """
     Fetch papers from the specified categories and store them in the database.
-
-    Parameters
-    ----------
-    num_days : int
-        Number of days to fetch papers.
-    categories : str
-        Comma-separated list of categories to fetch papers.
     """
     categories = categories.split(",")
     db = ArxivDatabase(DATABASE_PATH)
     for category in categories:
         papers = download_papers(category, num_days=num_days)
         db.save_papers(papers)
         logging.info(f"Fetched papers from {category}")
@@ -59,19 +52,14 @@
 
 
 @click.command()
 @click.option("--days-ago", default=7, help="Number of days ago to fetch papers.")
 def show(days_ago):
     """
     Show papers fetched from the specified number of days ago.
-
-    Parameters
-    ----------
-    days_ago : int
-        Number of days ago to fetch papers.
     """
     published_after = datetime.now() - timedelta(days=days_ago)
     db = ArxivDatabase(DATABASE_PATH)
     papers = db.get_papers(published_after)
 
     try:
         print_papers(papers)
@@ -101,25 +89,14 @@
 )
 @click.option(
     "-l", "--limit", default=10, help="The maximum number of results to return"
 )
 def search(query, experimental, limit, force):
     """
     Search papers in the database based on a query.
-
-    Parameters
-    ----------
-    query : str
-        Search query for the papers.
-    experimental: bool
-        If toggled, then documents will be matched using an LSA model rather than a simple string pattern
-    limit: int
-        The maximum number of results to display.
-    force: bool
-        If toggled, then forces a refresh of the underlying model before performing a search.
     """
     db = ArxivDatabase(DATABASE_PATH)
 
     if experimental:
         # TODO: Try better approaches :)
         lsa = LsaDocumentSearch(MODEL_PATH)
         search_results = lsa.search(db, query, limit=limit, force_refresh=force)
```

### Comparing `arxivterminal-0.2.0/arxivterminal/db.py` & `arxivterminal-0.3.0/arxivterminal/db.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,16 @@
                 CREATE TABLE IF NOT EXISTS papers (
                     entry_id TEXT PRIMARY KEY,
                     updated TIMESTAMP,
                     published TIMESTAMP,
                     title TEXT,
                     summary TEXT,
                     authors TEXT,
-                    categories TEXT
+                    categories TEXT,
+                    viewed BOOLEAN DEFAULT 0
                 )
             """
             )
             conn.commit()
 
     @staticmethod
     def convert_to_paper(row: Tuple) -> ArxivPaper:
@@ -59,14 +60,15 @@
             entry_id=row[0],
             updated=datetime.fromisoformat(row[1]),
             published=datetime.fromisoformat(row[2]),
             title=row[3],
             summary=row[4],
             authors=row[5].split(","),
             categories=row[6].split(","),
+            viewed=(row[7] == 1),
         )
 
     def save_papers(self, papers: List[ArxivPaper]):
         """
         Save a list of ArxivPaper objects to the database.
 
         Parameters
@@ -117,25 +119,27 @@
                         INSERT INTO papers (
                             entry_id,
                             updated,
                             published,
                             title,
                             summary,
                             authors,
-                            categories
-                        ) VALUES (?, ?, ?, ?, ?, ?, ?)
+                            categories,
+                            viewed
+                        ) VALUES (?, ?, ?, ?, ?, ?, ?, ?)
                     """,
                         (
                             paper.entry_id,
                             paper.updated.isoformat(),
                             paper.published.isoformat(),
                             paper.title,
                             paper.summary,
                             ",".join(paper.authors),
                             ",".join(paper.categories),
+                            0,
                         ),
                     )
                     num_inserted += 1
 
             # Commit the changes to the database and close the connection
             conn.commit()
 
@@ -164,26 +168,26 @@
         with sqlite3.connect(self.database_path) as conn:
             cursor = conn.cursor()
 
             if published_after is not None:
                 # Query the database for papers published after the specified date
                 cursor.execute(
                     """
-                    SELECT entry_id, updated, published, title, summary, authors, categories
+                    SELECT entry_id, updated, published, title, summary, authors, categories, viewed
                     FROM papers
                     WHERE published >= ?
                     ORDER BY published ASC
                 """,
                     (published_after.isoformat(),),
                 )
             else:
                 # Query the database for papers published after the specified date
                 cursor.execute(
                     """
-                    SELECT entry_id, updated, published, title, summary, authors, categories
+                    SELECT entry_id, updated, published, title, summary, authors, categories, viewed
                     FROM papers
                     ORDER BY published ASC
                 """
                 )
 
             # Parse the results into ArxivPaper objects
             papers = []
@@ -227,15 +231,15 @@
         # Connect to the database
         with sqlite3.connect(self.database_path) as conn:
             cursor = conn.cursor()
 
             # Query the database for papers with the search phrase in the title or summary
             cursor.execute(
                 """
-                SELECT entry_id, updated, published, title, summary, authors, categories
+                SELECT entry_id, updated, published, title, summary, authors, categories, viewed
                 FROM papers
                 WHERE title LIKE ? OR summary LIKE ?
                 ORDER BY published ASC
             """,
                 (f"%{query}%", f"%{query}%"),
             )
 
@@ -243,14 +247,37 @@
             papers = []
             for row in cursor.fetchall():
                 paper = self.convert_to_paper(row)
                 papers.append(paper)
 
         return papers
 
+    def mark_paper_viewed(self, paper: ArxivPaper):
+        """
+        Marks a paper as viewed
+
+        Parameters
+        ----------
+        paper: ArxivPaper
+            The ArxivPaper to be marked as viewed
+        """
+        with sqlite3.connect(self.database_path) as conn:
+            cursor = conn.cursor()
+
+            # Update the 'viewed' column for the specified paper
+            cursor.execute(
+                """
+                UPDATE papers
+                SET viewed = 1
+                WHERE entry_id = ?
+            """,
+                (paper.entry_id,),
+            )
+            conn.commit()
+
     def get_stats(self) -> List[ArxivStats]:
         """
         Retrieve the count of papers by publication date from the database.
 
         Returns
         -------
         List[ArxivStats]
```

### Comparing `arxivterminal-0.2.0/arxivterminal/fetch.py` & `arxivterminal-0.3.0/arxivterminal/fetch.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,14 +54,15 @@
             entry_id=result.entry_id,
             updated=result.updated,
             published=result.published,
             title=result.title,
             summary=result.summary,
             authors=[a.name for a in result.authors],
             categories=result.categories,
+            viewed=False,
         )
         if paper.published >= start_date and paper.published <= end_date:
             papers.append(paper)
         elif paper.published < start_date:
             logging.info(f"Reached start date {start_date}")
             break
```

### Comparing `arxivterminal-0.2.0/arxivterminal/ml.py` & `arxivterminal-0.3.0/arxivterminal/ml.py`

 * *Files identical despite different names*

### Comparing `arxivterminal-0.2.0/arxivterminal/output.py` & `arxivterminal-0.3.0/arxivterminal/output.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import List
 
 from termcolor import colored
 
 from arxivterminal.constants import DATABASE_PATH, MODEL_PATH
 from arxivterminal.db import ArxivDatabase, ArxivStats
+from arxivterminal.download import download_paper
 from arxivterminal.fetch import ArxivPaper
 from arxivterminal.ml import LsaDocumentSearch
 
 
 class ExitAppException(Exception):
     pass
 
@@ -23,54 +24,87 @@
     show_dates: bool
         If true, then the publish date of the paper is shown. Otherwise, date headers are
         omitted.
     """
     current_date = None
     total_papers = len(papers)
 
+    def _format_categories(categories: List[str]) -> str:
+        joined = ",".join(categories)
+        return f"[{joined}]"
+
+    def _format_authors(authors: List[str], max_len: int):
+        author_list = ", ".join(authors[:max_len])
+
+        if len(authors) > max_len:
+            author_list += ", et al."
+
+        return author_list
+
     while True:
         for i, paper in enumerate(papers):
             paper_date = paper.published.date()
             if (paper_date != current_date) and show_dates:
                 print(colored(f"\n{paper_date}", "cyan"))
                 print(colored("".join(["-"] * 10), "cyan"))
                 current_date = paper_date
             inverted_line_number = total_papers - i
-            print(f"{colored(inverted_line_number, 'yellow')}. {paper.title}")
+
+            if paper.viewed:
+                print(
+                    f"{colored(inverted_line_number, 'green')}. {colored(paper.title, 'green')}"
+                )
+            else:
+                print(f"{colored(inverted_line_number, 'yellow')}. {paper.title}")
 
         # Get the line number from the user
         user_input = input(
             "\nEnter the line number to show the full abstract, 'b' to go back, or 'q' to quit: "
         )
 
         while user_input.lower() != "b":
             try:
                 line_number = int(user_input)
                 if 1 <= line_number <= total_papers:
-                    selected_paper = papers[total_papers - line_number]
+                    selected_index = total_papers - line_number
+                    selected_paper = papers[selected_index]
                     print(f"\n{colored(selected_paper.title, 'yellow')}")
-                    print(f"{colored(selected_paper.entry_id, 'blue')}")
+                    print(f"{_format_authors(selected_paper.authors, 3)}")
+                    print(f"\n{colored(selected_paper.entry_id, 'blue')}")
+                    print(f"\n{colored('Abstract:', 'cyan')} {selected_paper.summary}")
                     print(
-                        f"\n{colored('Abstract:', 'cyan')} {selected_paper.summary}\n"
+                        f"\nCategories: {_format_categories(selected_paper.categories)}\n"
                     )
+                    db = ArxivDatabase(str(DATABASE_PATH))
+                    db.mark_paper_viewed(selected_paper)
+                    papers[selected_index].viewed = True
                 else:
                     print("Invalid line number. Please try again.")
             except ValueError:
                 if user_input.lower() == "q":
                     raise ExitAppException
+                elif user_input.lower() == "d":
+                    try:
+                        download_paper(selected_paper)
+                    except FileExistsError:
+                        pass
+                    user_input = input(
+                        "Enter 'b' to go back, 'd' to download, 's' to search similar, or 'q' to quit: "
+                    )
+                    continue
                 elif user_input.lower() == "s":
                     db = ArxivDatabase(str(DATABASE_PATH))
                     lsa = LsaDocumentSearch(str(MODEL_PATH))
                     search_results = lsa.search(db, selected_paper.summary)
                     print_papers(search_results, show_dates=False)
 
                 print("Invalid input. Please try again.")
 
             user_input = input(
-                "Enter the line number to show the full abstract, 'b' to go back, 's' to search similar, or 'q' to quit: "  # noqa: E501
+                "Enter the line number to show the full abstract, 'b' to go back, 'd' to download, 's' to search similar, or 'q' to quit: "  # noqa: E501
             )
 
 
 def print_stats(stats: List[ArxivStats]):
     """
     Print the count of Arxiv papers by their publication date in a formatted manner.
```

### Comparing `arxivterminal-0.2.0/pyproject.toml` & `arxivterminal-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "arxivterminal"
-version = "0.2.0"
+version = "0.3.0"
 description = "An application for summarizing Arxiv results within the terminal"
 authors = ["John Bencina <jbencina@users.noreply.github.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `arxivterminal-0.2.0/PKG-INFO` & `arxivterminal-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arxivterminal
-Version: 0.2.0
+Version: 0.3.0
 Summary: An application for summarizing Arxiv results within the terminal
 License: GPL-3.0-or-later
 Author: John Bencina
 Author-email: jbencina@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
@@ -21,22 +21,24 @@
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
 Requires-Dist: termcolor (>=2.2.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Arxiv Terminal
 ![Tests](https://github.com/jbencina/arxivterminal/actions/workflows/main.yaml/badge.svg)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/arxivterminal)](https://pypi.org/project/arxivterminal)
 
 Arxiv Terminal is a command-line interface (CLI) tool for fetching, searching, and displaying papers from the [arXiv](https://arxiv.org/) preprint repository. The tool allows you to fetch papers from specified categories, search the fetched papers, and display their statistics.
 
 ## Features
 
 - Fetch paper abstracts from specified categories and save them in a local sqllite database.
 - Show fetched papers and interatively open for more detailed abstracts
 - Search fetched papers based on a query (Currently supports pattern + LSA semantic search)
+- Download papers locally as PDF
 
 ![Demo](static/demo.gif)
 
 ## Contributors
 A special call out to ChatGPT (v4) which helped write and modify various code and documentation in this repository.
 
 ## Installation
@@ -80,14 +82,18 @@
 arxiv delete_all
 ```
 
 Show papers fetched in the last 7 days
 
 ```bash
 arxiv show --days-ago 7
+
+# On this screen the user can select a paper for more
+# details by typing a line number. Additional options
+# allow for searching & downloading
 ```
 
 Display statistics of the papers stored in the database:
 
 ```bash
 arxiv stats
 ```
```

