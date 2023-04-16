# Comparing `tmp/acro-0.0.5.tar.gz` & `tmp/acro-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acro-0.0.5.tar", last modified: Wed Nov  2 11:55:45 2022, max compression
+gzip compressed data, was "acro-0.0.6.tar", last modified: Sun Apr 16 19:05:49 2023, max compression
```

## Comparing `acro-0.0.5.tar` & `acro-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2022-11-02 11:55:45.440933 acro-0.0.5/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1063 2022-09-08 13:00:24.000000 acro-0.0.5/LICENSE
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1960 2022-11-02 11:55:45.436933 acro-0.0.5/PKG-INFO
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1126 2022-11-02 11:52:01.000000 acro-0.0.5/README.md
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2022-11-02 11:55:45.436933 acro-0.0.5/acro/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       32 2022-10-06 14:19:43.000000 acro-0.0.5/acro/__init__.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    26505 2022-10-14 14:38:14.000000 acro-0.0.5/acro/acro.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1006 2022-10-14 14:35:44.000000 acro-0.0.5/acro/default.yaml
--rw-rw-r--   0 unknown   (1000) unknown   (1000)    10123 2022-10-30 13:33:18.000000 acro-0.0.5/acro/utils.py
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2022-11-02 11:55:45.436933 acro-0.0.5/acro.egg-info/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1960 2022-11-02 11:55:45.000000 acro-0.0.5/acro.egg-info/PKG-INFO
--rw-rw-r--   0 unknown   (1000) unknown   (1000)      265 2022-11-02 11:55:45.000000 acro-0.0.5/acro.egg-info/SOURCES.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)        1 2022-11-02 11:55:45.000000 acro-0.0.5/acro.egg-info/dependency_links.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       46 2022-11-02 11:55:45.000000 acro-0.0.5/acro.egg-info/requires.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       10 2022-11-02 11:55:45.000000 acro-0.0.5/acro.egg-info/top_level.txt
--rw-rw-r--   0 unknown   (1000) unknown   (1000)       38 2022-11-02 11:55:45.440933 acro-0.0.5/setup.cfg
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     1369 2022-11-02 11:46:25.000000 acro-0.0.5/setup.py
-drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2022-11-02 11:55:45.436933 acro-0.0.5/test/
--rw-rw-r--   0 unknown   (1000) unknown   (1000)        0 2022-09-26 11:44:01.000000 acro-0.0.5/test/__init__.py
--rw-rw-r--   0 unknown   (1000) unknown   (1000)     5927 2022-10-30 15:03:03.000000 acro-0.0.5/test/test_initial.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-04-16 19:05:49.689686 acro-0.0.6/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1063 2022-09-08 13:00:24.000000 acro-0.0.6/LICENSE
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3149 2023-04-16 19:05:49.689686 acro-0.0.6/PKG-INFO
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     2247 2022-11-17 15:40:19.000000 acro-0.0.6/README.md
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-04-16 19:05:49.689686 acro-0.0.6/acro/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       32 2023-03-13 11:57:55.000000 acro-0.0.6/acro/__init__.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    28833 2023-04-16 18:48:41.000000 acro-0.0.6/acro/acro.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1006 2023-03-13 11:57:55.000000 acro-0.0.6/acro/default.yaml
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)    11264 2023-04-16 18:48:41.000000 acro-0.0.6/acro/utils.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-04-16 19:05:49.689686 acro-0.0.6/acro.egg-info/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     3149 2023-04-16 19:05:49.000000 acro-0.0.6/acro.egg-info/PKG-INFO
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)      265 2023-04-16 19:05:49.000000 acro-0.0.6/acro.egg-info/SOURCES.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)        1 2023-04-16 19:05:49.000000 acro-0.0.6/acro.egg-info/dependency_links.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       46 2023-04-16 19:05:49.000000 acro-0.0.6/acro.egg-info/requires.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       10 2023-04-16 19:05:49.000000 acro-0.0.6/acro.egg-info/top_level.txt
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)       38 2023-04-16 19:05:49.689686 acro-0.0.6/setup.cfg
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     1427 2023-04-16 18:51:12.000000 acro-0.0.6/setup.py
+drwxrwxr-x   0 unknown   (1000) unknown   (1000)        0 2023-04-16 19:05:49.689686 acro-0.0.6/test/
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)        0 2022-09-26 11:44:01.000000 acro-0.0.6/test/__init__.py
+-rw-rw-r--   0 unknown   (1000) unknown   (1000)     9669 2023-04-16 18:48:41.000000 acro-0.0.6/test/test_initial.py
```

### Comparing `acro-0.0.5/LICENSE` & `acro-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `acro-0.0.5/PKG-INFO` & `acro-0.0.6/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: acro
-Version: 0.0.5
+Version: 0.0.6
+Summary: ACRO: Tools for the Automatic Checking of Research Outputs
 Home-page: https://github.com/AI-SDC/ACRO
 Maintainer: Jim Smith
 Maintainer-email: james.smith@uwe.ac.uk
 License: MIT
 Keywords: data-privacy,data-protection,privacy,privacy-tools,statistical-disclosure-control
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -18,14 +19,38 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## ACRO: Tools for the Automatic Checking of Research Outputs
 
+Statistical agencies and other custodians of secure facilities such as Trusted
+Research Environments (TREs) routinely require the checking of research outputs
+for disclosure risk. This can be a time-consuming and costly task, requiring
+skilled staff.
+
+ACRO (Automatic Checking of Research Outputs) is an open source
+tool for automating the statistical disclosure control (SDC) of research
+outputs. ACRO assists researchers and output checkers by distinguishing between
+research output that is safe to publish, output that requires further analysis,
+and output that cannot be published because of substantial disclosure risk.
+
+It does this by providing a light-weight 'skin' that sits over well-known
+analysis tools, in a variety of languages researchers might use. This adds
+functionality to:
+
+*   identify potentially disclosive outputs against a range of commonly used
+    disclosure tests;
+*   suppress outputs where required;
+*   report reasons for suppression;
+*   produce simple summary documents TRE staff can use to streamline their
+    workflow.
+
+![ACRO workflow and architecture schematic](docs/schematic.png)
+
 See the project [wiki](https://github.com/AI-SDC/ACRO/wiki) for details.
 
 *******************************************************************************
 
 [![License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](https://opensource.org/licenses/MIT)
 [![Latest Version](https://img.shields.io/github/v/release/AI-SDC/ACRO?style=flat)](https://github.com/AI-SDC/ACRO/releases)
 [![DOI](https://zenodo.org/badge/534172863.svg)](https://zenodo.org/badge/latestdoi/534172863)
```

### Comparing `acro-0.0.5/acro/acro.py` & `acro-0.0.6/acro/acro.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """ACRO: Automatic Checking of Research Outputs."""
 
+import datetime
 import logging
 import os
 import pathlib
 import warnings
 from inspect import stack
 
 import pandas as pd
@@ -83,37 +84,50 @@
         elif extension == ".xlsx":
             utils.finalise_excel(filename, self.results)
         else:
             raise ValueError("Invalid file extension. Options: {.json, .xlsx}")
         logger.info("output written to: %s", filename)
         return self.results
 
-    def __add_output(
-        self, command: str, summary: str, outcome: DataFrame, output: list[DataFrame]
+    def __add_output(  # pylint: disable=too-many-arguments
+        self,
+        command: str,
+        summary: str,
+        outcome: DataFrame,
+        output: list[DataFrame],
+        comments: str = "",
     ) -> None:
         """Adds an output to the results dictionary.
 
         Parameters
         ----------
         command : str
             String representation of the operation performed.
         summary : str
             String summarising the ACRO checks.
         outcome : DataFrame
             DataFrame describing the details of ACRO checks.
         output : list[DataFrame]
             List of output DataFrames.
+        comments: str
+            String entered by the user to add comments to the output.
         """
-        name: str = f"output_{self.output_id}"
+
+        now = datetime.datetime.now()
+        timestamp = str(now.strftime("%Y-%m-%d-%H%M%S%f")[:-4])
+
+        name: str = f"output_{self.output_id}_{timestamp}"
         self.output_id += 1
         self.results[name] = {
             "command": command,
             "summary": summary,
             "outcome": outcome,
             "output": output,  # json.loads(output),  # JSON to dict
+            "timestamp": timestamp,
+            "comments": comments,
         }
         logger.info("add_output(): %s", name)
 
     def remove_output(self, key: str) -> None:
         """Removes an output from the results dictionary.
 
         Parameters
@@ -121,25 +135,41 @@
         key : str
             Key specifying which output to remove, e.g., 'output_0'.
         """
         if key in self.results:
             del self.results[key]
             logger.info("remove_output(): %s removed", key)
         else:
-            warnings.warn(f"unable to remove {key}, key not found")
+            warnings.warn(f"unable to remove {key}, key not found", stacklevel=8)
 
     def print_outputs(self) -> None:
         """Prints the current results dictionary."""
         logger.debug("print_outputs()")
         for name, result in self.results.items():
             print(f"{name}:")
             for key, item in result.items():
                 print(f"{key}: {item}")
             print("\n")
 
+    def custom_output(self, filename: str, comment: str = "") -> None:
+        """Adds an unsupported output to the results dictionary.
+
+        Parameters
+        ----------
+        filename : str
+            The name of the file that will be added to the list of the outputs.
+        """
+        self.__add_output(
+            command="custom",
+            summary="review",
+            outcome=DataFrame(),
+            output=os.path.abspath(filename),
+            comments=comment,
+        )
+
     def crosstab(  # pylint: disable=too-many-arguments,too-many-locals
         self,
         index,
         columns,
         values=None,
         rownames=None,
         colnames=None,
@@ -366,15 +396,15 @@
         str
             Summary of the check.
         """
         dof: int = model.df_resid
         threshold: int = self.config["safe_dof_threshold"]
         if dof < threshold:
             summary = f"fail; dof={dof} < {threshold}"
-            warnings.warn(f"Unsafe {name}: {summary}")
+            warnings.warn(f"Unsafe {name}: {summary}", stacklevel=8)
         else:
             summary = f"pass; dof={dof} >= {threshold}"
         logger.info("%s() outcome: %s", name, summary)
         return summary
 
     def ols(  # pylint: disable=too-many-locals
         self, endog, exog=None, missing="none", hasconst=None, **kwargs
@@ -669,14 +699,55 @@
         summary = self.__check_model_dof("probitr", model)
         tables: list[SimpleTable] = results.summary().tables
         self.__add_output(
             command, summary, DataFrame(), utils.get_summary_dataframes(tables)
         )
         return results
 
+    def rename_output(self, old: str, new: str) -> None:
+        """Rename an output and take the timestamp from the old name
+        and suffix it to the new name
+
+        Parameters
+        ----------
+        old : str
+            The old name of the output.
+        new : str
+            The new name of the output.
+        """
+        timestamp = old.split("_")[2]
+        new = new + "_" + timestamp
+        if old in self.results:
+            self.results[new] = self.results[old]
+            del self.results[old]
+            logger.info("rename_output(): %s renamed to %s", old, new)
+        else:
+            warnings.warn(f"unable to rename {old}, key not found", stacklevel=8)
+
+    def add_comments(self, output: str, comment: str) -> None:
+        """Adds comments to outputs
+
+        Parameters
+        ----------
+        output : str
+            The name of the output.
+        comment : str
+            The comment.
+        """
+        if output in self.results:
+            if self.results[output]["comments"] == "":
+                self.results[output]["comments"] = comment
+            else:
+                self.results[output]["comments"] = (
+                    self.results[output]["comments"] + ", " + comment
+                )
+            logger.info("a comment was added to %s", output)
+        else:
+            warnings.warn(f"unable to find {output}, key not found", stacklevel=8)
+
 
 def add_constant(data, prepend: bool = True, has_constant: str = "skip"):
     """Add a column of ones to an array.
 
     Parameters
     ----------
     data : array_like
```

### Comparing `acro-0.0.5/acro/default.yaml` & `acro-0.0.6/acro/default.yaml`

 * *Files identical despite different names*

### Comparing `acro-0.0.5/acro/utils.py` & `acro-0.0.6/acro/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """ACRO: Utility Functions."""
 
 import copy
 import json
 import logging
+import os
 from collections.abc import Callable
 from inspect import getframeinfo
 
 import numpy as np
 import pandas as pd
 from pandas import DataFrame, Series
 from statsmodels.iolib.table import SimpleTable
@@ -23,14 +24,17 @@
 
 # aggregation function parameters
 THRESHOLD: int = 10
 SAFE_PRATIO_P: float = 0.1
 SAFE_NK_N: int = 2
 SAFE_NK_K: float = 0.9
 
+# add output directory
+OUTPUT_DIRECTORY = "outputs/"
+
 
 def get_command(default: str, stack_list: list[tuple]) -> str:
     """Returns the calling source line as a string.
 
     Parameters
     ----------
     default : str
@@ -60,24 +64,56 @@
     Parameters
     ----------
     filename : str
         Name of the output file.
     results : dict
         Outputs to write.
     """
-    # convert dataframes to json
+
     outputs: dict = copy.deepcopy(results)
-    for _, output in outputs.items():
+
+    # check if the outputs directory was already created
+    try:  # pragma: no cover
+        os.makedirs(OUTPUT_DIRECTORY)
+        logger.info("Directory %s created successfully", OUTPUT_DIRECTORY)
+    except FileExistsError:
+        logger.info("Directory %s already exists", OUTPUT_DIRECTORY)
+
+    # convert dataframes to json
+    for output_id, output in outputs.items():
         if output["outcome"] is not None:
             output["outcome"] = output["outcome"].to_json()
-        for i, _ in enumerate(output["output"]):
-            output["output"][i] = output["output"][i].to_json()
+
+        # save each output to a different file
+        if not isinstance(output["output"], str):
+            with open(
+                OUTPUT_DIRECTORY + f"{output_id}.csv",
+                mode="w",
+                newline="",
+                encoding="utf-8",
+            ) as file:
+                for i, _ in enumerate(output["output"]):
+                    file.write(output["output"][i].to_csv())
+            output["output"] = os.path.abspath(f"{OUTPUT_DIRECTORY}{output_id}.csv")
+
     # write to disk
-    with open(filename, "w", encoding="utf-8") as file:
-        json.dump(outputs, file, indent=4, sort_keys=False)
+    if os.path.isfile(OUTPUT_DIRECTORY + filename):
+        with open(
+            OUTPUT_DIRECTORY + filename, "r+", newline="", encoding="utf-8"
+        ) as file:
+            data = json.load(file)
+            data.update(outputs)
+            file.seek(0)
+            json.dump(data, file, indent=4, sort_keys=False)
+
+    else:
+        with open(
+            OUTPUT_DIRECTORY + filename, "w", newline="", encoding="utf-8"
+        ) as file:
+            json.dump(outputs, file, indent=4, sort_keys=False)
 
 
 def finalise_excel(filename: str, results: dict) -> None:
     """Writes outputs to an excel spreadsheet.
 
     Parameters
     ----------
```

### Comparing `acro-0.0.5/acro.egg-info/PKG-INFO` & `acro-0.0.6/acro.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: acro
-Version: 0.0.5
+Version: 0.0.6
+Summary: ACRO: Tools for the Automatic Checking of Research Outputs
 Home-page: https://github.com/AI-SDC/ACRO
 Maintainer: Jim Smith
 Maintainer-email: james.smith@uwe.ac.uk
 License: MIT
 Keywords: data-privacy,data-protection,privacy,privacy-tools,statistical-disclosure-control
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -18,14 +19,38 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## ACRO: Tools for the Automatic Checking of Research Outputs
 
+Statistical agencies and other custodians of secure facilities such as Trusted
+Research Environments (TREs) routinely require the checking of research outputs
+for disclosure risk. This can be a time-consuming and costly task, requiring
+skilled staff.
+
+ACRO (Automatic Checking of Research Outputs) is an open source
+tool for automating the statistical disclosure control (SDC) of research
+outputs. ACRO assists researchers and output checkers by distinguishing between
+research output that is safe to publish, output that requires further analysis,
+and output that cannot be published because of substantial disclosure risk.
+
+It does this by providing a light-weight 'skin' that sits over well-known
+analysis tools, in a variety of languages researchers might use. This adds
+functionality to:
+
+*   identify potentially disclosive outputs against a range of commonly used
+    disclosure tests;
+*   suppress outputs where required;
+*   report reasons for suppression;
+*   produce simple summary documents TRE staff can use to streamline their
+    workflow.
+
+![ACRO workflow and architecture schematic](docs/schematic.png)
+
 See the project [wiki](https://github.com/AI-SDC/ACRO/wiki) for details.
 
 *******************************************************************************
 
 [![License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat)](https://opensource.org/licenses/MIT)
 [![Latest Version](https://img.shields.io/github/v/release/AI-SDC/ACRO?style=flat)](https://github.com/AI-SDC/ACRO/releases)
 [![DOI](https://zenodo.org/badge/534172863.svg)](https://zenodo.org/badge/latestdoi/534172863)
```

### Comparing `acro-0.0.5/setup.py` & `acro-0.0.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 from setuptools import find_packages, setup
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="acro",
-    version="0.0.5",
+    version="0.0.6",
     license="MIT",
     maintainer="Jim Smith",
     maintainer_email="james.smith@uwe.ac.uk",
-    description="",
+    description="ACRO: Tools for the Automatic Checking of Research Outputs",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/AI-SDC/ACRO",
     packages=find_packages(),
     package_data={"acro": ["default.yaml"]},
     python_requires=">=3.10",
     install_requires=["lxml", "numpy", "openpyxl", "pandas", "PyYAML", "statsmodels"],
```

