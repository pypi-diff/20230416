# Comparing `tmp/dover-lap-1.1.0.tar.gz` & `tmp/dover-lap-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dover-lap-1.1.0.tar", last modified: Sat Mar  6 15:00:26 2021, max compression
+gzip compressed data, was "/Users/desh/Work/dover-lap/dist/.tmp-3g3xh83o/dover-lap-1.2.0.tar", last modified: Sun Apr 16 15:40:47 2023, max compression
```

## Comparing `dover-lap-1.1.0.tar` & `dover-lap-1.2.0.tar`

### file list

```diff
@@ -1,34 +1,37 @@
-drwxr-xr-x   0 desh       (501) staff       (20)        0 2021-03-06 15:00:26.040775 dover-lap-1.1.0/
--rw-r--r--   0 desh       (501) staff       (20)       24 2020-11-30 03:18:26.000000 dover-lap-1.1.0/MANIFEST.in
--rw-r--r--   0 desh       (501) staff       (20)     6026 2021-03-06 15:00:26.040347 dover-lap-1.1.0/PKG-INFO
--rw-r--r--   0 desh       (501) staff       (20)     4540 2021-03-06 14:56:26.000000 dover-lap-1.1.0/README.md
-drwxr-xr-x   0 desh       (501) staff       (20)        0 2021-03-06 15:00:26.032198 dover-lap-1.1.0/dover_lap/
--rw-r--r--   0 desh       (501) staff       (20)       39 2021-01-16 15:09:22.000000 dover-lap-1.1.0/dover_lap/__init__.py
--rwxr-xr-x   0 desh       (501) staff       (20)     5074 2021-03-06 14:56:26.000000 dover-lap-1.1.0/dover_lap/dover_lap.py
-drwxr-xr-x   0 desh       (501) staff       (20)        0 2021-03-06 15:00:26.036571 dover-lap-1.1.0/dover_lap/libs/
--rw-r--r--   0 desh       (501) staff       (20)       80 2021-03-06 14:52:05.000000 dover-lap-1.1.0/dover_lap/libs/__init__.py
--rw-r--r--   0 desh       (501) staff       (20)     2230 2021-02-26 02:25:16.000000 dover-lap-1.1.0/dover_lap/libs/metrics.py
--rw-r--r--   0 desh       (501) staff       (20)     4198 2021-01-16 15:09:22.000000 dover-lap-1.1.0/dover_lap/libs/rttm.py
--rw-r--r--   0 desh       (501) staff       (20)     8884 2021-01-16 15:09:22.000000 dover-lap-1.1.0/dover_lap/libs/turn.py
--rw-r--r--   0 desh       (501) staff       (20)     3949 2021-01-16 15:09:22.000000 dover-lap-1.1.0/dover_lap/libs/uem.py
--rw-r--r--   0 desh       (501) staff       (20)     2439 2021-01-16 15:09:22.000000 dover-lap-1.1.0/dover_lap/libs/utils.py
-drwxr-xr-x   0 desh       (501) staff       (20)        0 2021-03-06 15:00:26.038105 dover-lap-1.1.0/dover_lap/src/
--rw-r--r--   0 desh       (501) staff       (20)      132 2021-03-06 14:56:26.000000 dover-lap-1.1.0/dover_lap/src/__init__.py
--rw-r--r--   0 desh       (501) staff       (20)     1645 2021-03-06 14:56:26.000000 dover-lap-1.1.0/dover_lap/src/doverlap.py
--rw-r--r--   0 desh       (501) staff       (20)     2361 2021-03-06 14:56:26.000000 dover-lap-1.1.0/dover_lap/src/label_mapping.py
--rw-r--r--   0 desh       (501) staff       (20)     5382 2021-01-16 15:09:22.000000 dover-lap-1.1.0/dover_lap/src/label_voting.py
-drwxr-xr-x   0 desh       (501) staff       (20)        0 2021-03-06 15:00:26.039811 dover-lap-1.1.0/dover_lap/src/mapping/
--rw-r--r--   0 desh       (501) staff       (20)       66 2021-03-06 14:56:26.000000 dover-lap-1.1.0/dover_lap/src/mapping/__init__.py
--rw-r--r--   0 desh       (501) staff       (20)     7810 2021-03-06 14:56:26.000000 dover-lap-1.1.0/dover_lap/src/mapping/greedy.py
--rw-r--r--   0 desh       (501) staff       (20)     5933 2021-03-06 14:56:26.000000 dover-lap-1.1.0/dover_lap/src/mapping/hungarian.py
--rw-r--r--   0 desh       (501) staff       (20)     1646 2021-03-06 14:56:26.000000 dover-lap-1.1.0/dover_lap/src/mapping/map_utils.py
-drwxr-xr-x   0 desh       (501) staff       (20)        0 2021-03-06 15:00:26.033982 dover-lap-1.1.0/dover_lap.egg-info/
--rw-r--r--   0 desh       (501) staff       (20)     6026 2021-03-06 15:00:25.000000 dover-lap-1.1.0/dover_lap.egg-info/PKG-INFO
--rw-r--r--   0 desh       (501) staff       (20)      686 2021-03-06 15:00:25.000000 dover-lap-1.1.0/dover_lap.egg-info/SOURCES.txt
--rw-r--r--   0 desh       (501) staff       (20)        1 2021-03-06 15:00:25.000000 dover-lap-1.1.0/dover_lap.egg-info/dependency_links.txt
--rw-r--r--   0 desh       (501) staff       (20)       56 2021-03-06 15:00:25.000000 dover-lap-1.1.0/dover_lap.egg-info/entry_points.txt
--rw-r--r--   0 desh       (501) staff       (20)       75 2021-03-06 15:00:25.000000 dover-lap-1.1.0/dover_lap.egg-info/requires.txt
--rw-r--r--   0 desh       (501) staff       (20)       10 2021-03-06 15:00:25.000000 dover-lap-1.1.0/dover_lap.egg-info/top_level.txt
--rw-r--r--   0 desh       (501) staff       (20)       74 2021-03-06 14:56:26.000000 dover-lap-1.1.0/requirements.txt
--rw-r--r--   0 desh       (501) staff       (20)       38 2021-03-06 15:00:26.040909 dover-lap-1.1.0/setup.cfg
--rw-r--r--   0 desh       (501) staff       (20)      907 2021-03-06 14:56:26.000000 dover-lap-1.1.0/setup.py
+drwxr-xr-x   0 desh       (501) staff       (20)        0 2023-04-16 15:40:47.202525 dover-lap-1.2.0/
+-rw-r--r--   0 desh       (501) staff       (20)     1065 2020-09-03 00:18:50.000000 dover-lap-1.2.0/LICENSE
+-rw-r--r--   0 desh       (501) staff       (20)       24 2020-11-30 03:18:26.000000 dover-lap-1.2.0/MANIFEST.in
+-rw-r--r--   0 desh       (501) staff       (20)     4931 2023-04-16 15:40:47.202322 dover-lap-1.2.0/PKG-INFO
+-rw-r--r--   0 desh       (501) staff       (20)     4478 2023-04-16 15:34:23.000000 dover-lap-1.2.0/README.md
+drwxr-xr-x   0 desh       (501) staff       (20)        0 2023-04-16 15:40:47.196703 dover-lap-1.2.0/dover_lap/
+-rw-r--r--   0 desh       (501) staff       (20)       39 2021-01-16 15:09:22.000000 dover-lap-1.2.0/dover_lap/__init__.py
+-rwxr-xr-x   0 desh       (501) staff       (20)     4870 2023-04-16 15:31:18.000000 dover-lap-1.2.0/dover_lap/dover_lap.py
+drwxr-xr-x   0 desh       (501) staff       (20)        0 2023-04-16 15:40:47.199341 dover-lap-1.2.0/dover_lap/libs/
+-rw-r--r--   0 desh       (501) staff       (20)       80 2023-03-27 18:35:28.000000 dover-lap-1.2.0/dover_lap/libs/__init__.py
+-rw-r--r--   0 desh       (501) staff       (20)     4198 2021-01-16 15:09:22.000000 dover-lap-1.2.0/dover_lap/libs/rttm.py
+-rw-r--r--   0 desh       (501) staff       (20)     8884 2021-01-16 15:09:22.000000 dover-lap-1.2.0/dover_lap/libs/turn.py
+-rw-r--r--   0 desh       (501) staff       (20)     3899 2023-04-15 19:23:06.000000 dover-lap-1.2.0/dover_lap/libs/uem.py
+-rw-r--r--   0 desh       (501) staff       (20)     2556 2023-04-15 19:32:10.000000 dover-lap-1.2.0/dover_lap/libs/utils.py
+drwxr-xr-x   0 desh       (501) staff       (20)        0 2023-04-16 15:40:47.200435 dover-lap-1.2.0/dover_lap/src/
+-rw-r--r--   0 desh       (501) staff       (20)      132 2021-03-06 14:56:26.000000 dover-lap-1.2.0/dover_lap/src/__init__.py
+-rw-r--r--   0 desh       (501) staff       (20)     2128 2023-04-16 15:32:21.000000 dover-lap-1.2.0/dover_lap/src/doverlap.py
+-rw-r--r--   0 desh       (501) staff       (20)     1969 2023-04-16 15:32:34.000000 dover-lap-1.2.0/dover_lap/src/label_mapping.py
+-rw-r--r--   0 desh       (501) staff       (20)     4385 2023-04-16 15:19:54.000000 dover-lap-1.2.0/dover_lap/src/label_voting.py
+drwxr-xr-x   0 desh       (501) staff       (20)        0 2023-04-16 15:40:47.201534 dover-lap-1.2.0/dover_lap/src/mapping/
+-rw-r--r--   0 desh       (501) staff       (20)       66 2023-03-27 18:35:28.000000 dover-lap-1.2.0/dover_lap/src/mapping/__init__.py
+-rw-r--r--   0 desh       (501) staff       (20)     7800 2023-04-15 19:23:06.000000 dover-lap-1.2.0/dover_lap/src/mapping/greedy.py
+-rw-r--r--   0 desh       (501) staff       (20)     4304 2023-04-16 15:32:07.000000 dover-lap-1.2.0/dover_lap/src/mapping/hungarian.py
+-rw-r--r--   0 desh       (501) staff       (20)     1548 2023-04-15 19:23:06.000000 dover-lap-1.2.0/dover_lap/src/mapping/map_utils.py
+drwxr-xr-x   0 desh       (501) staff       (20)        0 2023-04-16 15:40:47.201996 dover-lap-1.2.0/dover_lap/src/voting/
+-rw-r--r--   0 desh       (501) staff       (20)       42 2023-04-16 15:19:54.000000 dover-lap-1.2.0/dover_lap/src/voting/__init__.py
+-rw-r--r--   0 desh       (501) staff       (20)     2030 2023-04-16 15:19:54.000000 dover-lap-1.2.0/dover_lap/src/voting/average.py
+drwxr-xr-x   0 desh       (501) staff       (20)        0 2023-04-16 15:40:47.197884 dover-lap-1.2.0/dover_lap.egg-info/
+-rw-r--r--   0 desh       (501) staff       (20)     4931 2023-04-16 15:40:47.000000 dover-lap-1.2.0/dover_lap.egg-info/PKG-INFO
+-rw-r--r--   0 desh       (501) staff       (20)      733 2023-04-16 15:40:47.000000 dover-lap-1.2.0/dover_lap.egg-info/SOURCES.txt
+-rw-r--r--   0 desh       (501) staff       (20)        1 2023-04-16 15:40:47.000000 dover-lap-1.2.0/dover_lap.egg-info/dependency_links.txt
+-rw-r--r--   0 desh       (501) staff       (20)       55 2023-04-16 15:40:47.000000 dover-lap-1.2.0/dover_lap.egg-info/entry_points.txt
+-rw-r--r--   0 desh       (501) staff       (20)       75 2023-04-16 15:40:47.000000 dover-lap-1.2.0/dover_lap.egg-info/requires.txt
+-rw-r--r--   0 desh       (501) staff       (20)       10 2023-04-16 15:40:47.000000 dover-lap-1.2.0/dover_lap.egg-info/top_level.txt
+-rw-r--r--   0 desh       (501) staff       (20)       74 2023-04-15 19:23:06.000000 dover-lap-1.2.0/requirements.txt
+-rw-r--r--   0 desh       (501) staff       (20)       38 2023-04-16 15:40:47.202586 dover-lap-1.2.0/setup.cfg
+-rw-r--r--   0 desh       (501) staff       (20)      907 2023-04-15 19:23:06.000000 dover-lap-1.2.0/setup.py
```

### Comparing `dover-lap-1.1.0/PKG-INFO` & `dover-lap-1.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,143 +1,142 @@
 Metadata-Version: 2.1
 Name: dover-lap
-Version: 1.1.0
+Version: 1.2.0
 Summary: Combine overlap-aware diarization output RTTMs
 Home-page: https://github.com/desh2608/dover-lap
 Author: Desh Raj
 Author-email: r.desh26@gmail.com
 License: Apache-2.0 License
-Description: # DOVER-Lap
-        Official implementation for [DOVER-Lap: A method for combining overlap-aware diarization outputs](https://arxiv.org/pdf/2011.01997.pdf).
-        
-        ## Installation
-        
-        ```shell
-        pip install dover-lap
-        ```
-        
-        ## How to run
-        
-        After installation, run
-        
-        ```shell
-        dover-lap [OPTIONS] OUTPUT_RTTM [INPUT_RTTMS]...
-        ```
-        
-        Example:
-        
-        ```shell
-        dover-lap egs/ami/rttm_dl_test egs/ami/rttm_test_*
-        ```
-        
-        ## Usage instructions
-        
-        ```shell
-        Usage: dover-lap [OPTIONS] OUTPUT_RTTM [INPUT_RTTMS]...
-        
-          Apply the DOVER-Lap algorithm on the input RTTM files.
-        
-        Options:
-          --custom-weight TEXT            Weights for input RTTMs
-          --dover-weight FLOAT            DOVER weighting factor  [default: 0.1]
-          --weight-type [rank|custom]     Specify whether to use rank weighting or
-                                          provide custom weights  [default: rank]
-        
-          --tie-breaking [uniform|all]    Specify whether to assign tied regions to
-                                          all speakers or divide uniformly  [default:
-                                          all]
-        
-          --second-maximal                If this flag is set, run a second iteration
-                                          of the maximal matching for greedy label
-                                          mapping  [default: False]
-        
-          --sort-first                    If this flag is set, sort inputs by DER
-                                          first before label mapping (only applicable
-                                          when label mapping type is hungarian)
-                                          [default: False]
-        
-          --label-mapping [hungarian|greedy]
-                                          Choose label mapping algorithm to use
-                                          [default: greedy]
-        
-          --random-seed INTEGER
-          -c, --channel INTEGER           Use this value for output channel IDs
-                                          [default: 1]
-        
-          -u, --uem-file PATH             UEM file path
-          --help                          Show this message and exit.
-        ```
-        
-        **Note:** 
-        
-        1. If `--weight-type custom` is used, then `--custom-weight` must be provided. For example:
-        
-        ```shell
-        dover-lap egs/ami/rttm_dl_test egs/ami/rttm_test_* --weight-type custom --custom-weight '[0.4,0.3,0.3]'
-        ```
-        
-        2. `label-mapping` can be set to `greedy` (default) or `hungarian`, which was the mapping
-        technique originally proposed in [DOVER](https://arxiv.org/abs/1909.08090). 
-        
-        ## Results
-        
-        We provide a sample result on the AMI mix-headset test set. The results can be 
-        obtained using [`spyder`](https://github.com/desh2608/spyder), which is automatically
-        installed with `dover-lap`:
-        
-        ```shell
-        dover-lap egs/ami/rttm_dl_test egs/ami/rttm_test_*
-        spyder egs/ami/ref_rttm_test egs/ami/rttm_dl_test
-        ```
-        
-        and similarly for the input hypothesis. The DER results are shown below.
-        
-        |                                   |   MS  |  FA  | Conf. |  DER  |
-        |-----------------------------------|:-----:|:----:|:-----:|:-----:|
-        | Overlap-aware VB resegmentation   |  9.84 | **2.06** |  9.60 | 21.50 |
-        | Overlap-aware spectral clustering | 11.48 | 2.27 |  9.81 | 23.56 |
-        | Region Proposal Network           |  **9.49** | 7.68 |  8.25 | 25.43 |
-        | DOVER-Lap (Hungarian mapping)     | 9.81 | 2.80 | 8.10 | 20.70 |
-        | DOVER-Lap (Greedy mapping)        | 9.71 | 3.02 |  **7.68** | **20.40** |
-        
-        
-        
-        ## Running time
-        
-        The algorithm is implemented in pure Python with NumPy for tensor computations. 
-        The time complexity is expected to increase exponentially with the number of 
-        inputs, but it should be reasonable for combining up to 10 input hypotheses.
-        
-        For smaller number of inputs (up to 5), the algorithm should take only a few seconds
-        to run on a laptop.
-        
-        ## Combining 2 systems with DOVER-Lap
-        
-        DOVER-Lap is meant to be used to combine **more than 2 systems**, since
-        black-box voting between 2 systems does not make much sense. Still, if 2 systems
-        are provided as input, we fall back on the Hungarian algorithm for label mapping,
-        since it is provably optimal for this case. Both the systems are assigned equal
-        weights, and in case of voting conflicts, the region is equally divided among the
-        two labels. This is not the intended use case and will almost certainly lead
-        to performance degradation.
-        
-        ## Citation
-        
-        ```
-        @article{Raj2021Doverlap,
-          title={{DOVER-Lap}: A Method for Combining Overlap-aware Diarization Outputs},
-          author={D.Raj and P.Garcia and Z.Huang and S.Watanabe and D.Povey and A.Stolcke and S.Khudanpur},
-          journal={2021 IEEE Spoken Language Technology Workshop (SLT)},
-          year={2021}
-        }
-        ```
-        
-        ## Contact
-        
-        For issues/bug reports, please raise an Issue in this repository, or reach out to me at `draj@cs.jhu.edu`.
-        
 Keywords: diarization dover
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: BSD License
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# DOVER-Lap
+Official implementation for [DOVER-Lap: A method for combining overlap-aware diarization outputs](https://arxiv.org/pdf/2011.01997.pdf).
+
+## Installation
+
+```shell
+pip install dover-lap
+```
+
+## How to run
+
+After installation, run
+
+```shell
+dover-lap [OPTIONS] OUTPUT_RTTM [INPUT_RTTMS]...
+```
+
+Example:
+
+```shell
+dover-lap egs/ami/rttm_dl_test egs/ami/rttm_test_*
+```
+
+## Usage instructions
+
+```shell
+Usage: dover-lap [OPTIONS] OUTPUT_RTTM [INPUT_RTTMS]...
+
+  Apply the DOVER-Lap algorithm on the input RTTM files.
+
+Options:
+  --custom-weight TEXT            Weights for input RTTMs
+  --dover-weight FLOAT            DOVER weighting factor  [default: 0.1]
+  --weight-type [rank|custom]     Specify whether to use rank weighting or
+                                  provide custom weights  [default: rank]
+
+  --second-maximal                If this flag is set, run a second iteration
+                                  of the maximal matching for greedy label
+                                  mapping  [default: False]
+
+  --label-mapping [hungarian|greedy]
+                                  Choose label mapping algorithm to use
+                                  [default: greedy]
+
+  --random-seed INTEGER
+  -c, --channel INTEGER           Use this value for output channel IDs
+                                  [default: 1]
+
+  -u, --uem-file PATH             UEM file path
+  --help                          Show this message and exit.
+```
+
+**Note:** 
+
+1. If `--weight-type custom` is used, then `--custom-weight` must be provided. For example:
+
+```shell
+dover-lap egs/ami/rttm_dl_test egs/ami/rttm_test_* --weight-type custom --custom-weight '[0.4,0.3,0.3]'
+```
+
+2. `label-mapping` can be set to `greedy` (default) or `hungarian`, which is a modified version of the mapping
+technique originally proposed in [DOVER](https://arxiv.org/abs/1909.08090).
+
+## Results
+
+We provide a sample result on the AMI mix-headset test set. The results can be 
+obtained using [`spyder`](https://github.com/desh2608/spyder), which is automatically
+installed with `dover-lap`:
+
+```shell
+dover-lap egs/ami/rttm_dl_test egs/ami/rttm_test_*
+spyder egs/ami/ref_rttm_test egs/ami/rttm_dl_test
+```
+
+and similarly for the input hypothesis. The DER results are shown below.
+
+|                                   |   MS  |  FA  | Conf. |  DER  |
+|-----------------------------------|:-----:|:----:|:-----:|:-----:|
+| Overlap-aware VB resegmentation   |  9.84 | **2.06** |  9.60 | 21.50 |
+| Overlap-aware spectral clustering | 11.48 | 2.27 |  9.81 | 23.56 |
+| Region Proposal Network           |  **9.49** | 7.68 |  8.25 | 25.43 |
+| DOVER-Lap (Hungarian mapping)     | 9.81 | 2.76 | 8.17 | 20.73 |
+| DOVER-Lap (Greedy mapping)*        | 9.71 | 3.02 |  **7.68** | **20.40** |
+
+_* The Greedy label mapping is exponential in number of inputs (see [this paper](https://arxiv.org/abs/2104.01954))._
+
+## Running time
+
+The algorithm is implemented in pure Python with NumPy for tensor computations. 
+The time complexity is expected to increase exponentially with the number of 
+inputs, but it should be reasonable for combining up to 10 input hypotheses. For 
+combining more than 10 inputs, we recommend setting `--label-mapping hungarian`.
+
+For smaller number of inputs (up to 5), the algorithm should take only a few seconds
+to run on a laptop.
+
+## Combining 2 systems with DOVER-Lap
+
+DOVER-Lap is meant to be used to combine **more than 2 systems**, since
+black-box voting between 2 systems does not make much sense. Still, if 2 systems
+are provided as input, we fall back on the Hungarian algorithm for label mapping,
+since it is provably optimal for this case. Both the systems are assigned equal
+weights, and in case of voting conflicts, the region is assigned to both
+labels. This is not the intended use case and will almost certainly lead
+to performance degradation.
+
+## Citation
+
+```
+@article{Raj2021Doverlap,
+  title={{DOVER-Lap}: A Method for Combining Overlap-aware Diarization Outputs},
+  author={D.Raj and P.Garcia and Z.Huang and S.Watanabe and D.Povey and A.Stolcke and S.Khudanpur},
+  journal={2021 IEEE Spoken Language Technology Workshop (SLT)},
+  year={2021}
+}
+
+@article{Raj2021ReformulatingDL,
+  title={Reformulating {DOVER-Lap} Label Mapping as a Graph Partitioning Problem},
+  author={Desh Raj and S. Khudanpur},
+  journal={INTERSPEECH},
+  year={2021},
+}
+```
+
+## Contact
+
+For issues/bug reports, please raise an Issue in this repository, or reach out to me at `draj@cs.jhu.edu`.
```

### Comparing `dover-lap-1.1.0/README.md` & `dover-lap-1.2.0/dover_lap.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: dover-lap
+Version: 1.2.0
+Summary: Combine overlap-aware diarization output RTTMs
+Home-page: https://github.com/desh2608/dover-lap
+Author: Desh Raj
+Author-email: r.desh26@gmail.com
+License: Apache-2.0 License
+Keywords: diarization dover
+Classifier: Development Status :: 3 - Alpha
+Classifier: Topic :: Utilities
+Classifier: License :: OSI Approved :: BSD License
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # DOVER-Lap
 Official implementation for [DOVER-Lap: A method for combining overlap-aware diarization outputs](https://arxiv.org/pdf/2011.01997.pdf).
 
 ## Installation
 
 ```shell
 pip install dover-lap
@@ -30,27 +45,18 @@
 
 Options:
   --custom-weight TEXT            Weights for input RTTMs
   --dover-weight FLOAT            DOVER weighting factor  [default: 0.1]
   --weight-type [rank|custom]     Specify whether to use rank weighting or
                                   provide custom weights  [default: rank]
 
-  --tie-breaking [uniform|all]    Specify whether to assign tied regions to
-                                  all speakers or divide uniformly  [default:
-                                  all]
-
   --second-maximal                If this flag is set, run a second iteration
                                   of the maximal matching for greedy label
                                   mapping  [default: False]
 
-  --sort-first                    If this flag is set, sort inputs by DER
-                                  first before label mapping (only applicable
-                                  when label mapping type is hungarian)
-                                  [default: False]
-
   --label-mapping [hungarian|greedy]
                                   Choose label mapping algorithm to use
                                   [default: greedy]
 
   --random-seed INTEGER
   -c, --channel INTEGER           Use this value for output channel IDs
                                   [default: 1]
@@ -63,16 +69,16 @@
 
 1. If `--weight-type custom` is used, then `--custom-weight` must be provided. For example:
 
 ```shell
 dover-lap egs/ami/rttm_dl_test egs/ami/rttm_test_* --weight-type custom --custom-weight '[0.4,0.3,0.3]'
 ```
 
-2. `label-mapping` can be set to `greedy` (default) or `hungarian`, which was the mapping
-technique originally proposed in [DOVER](https://arxiv.org/abs/1909.08090). 
+2. `label-mapping` can be set to `greedy` (default) or `hungarian`, which is a modified version of the mapping
+technique originally proposed in [DOVER](https://arxiv.org/abs/1909.08090).
 
 ## Results
 
 We provide a sample result on the AMI mix-headset test set. The results can be 
 obtained using [`spyder`](https://github.com/desh2608/spyder), which is automatically
 installed with `dover-lap`:
 
@@ -84,45 +90,53 @@
 and similarly for the input hypothesis. The DER results are shown below.
 
 |                                   |   MS  |  FA  | Conf. |  DER  |
 |-----------------------------------|:-----:|:----:|:-----:|:-----:|
 | Overlap-aware VB resegmentation   |  9.84 | **2.06** |  9.60 | 21.50 |
 | Overlap-aware spectral clustering | 11.48 | 2.27 |  9.81 | 23.56 |
 | Region Proposal Network           |  **9.49** | 7.68 |  8.25 | 25.43 |
-| DOVER-Lap (Hungarian mapping)     | 9.81 | 2.80 | 8.10 | 20.70 |
-| DOVER-Lap (Greedy mapping)        | 9.71 | 3.02 |  **7.68** | **20.40** |
-
+| DOVER-Lap (Hungarian mapping)     | 9.81 | 2.76 | 8.17 | 20.73 |
+| DOVER-Lap (Greedy mapping)*        | 9.71 | 3.02 |  **7.68** | **20.40** |
 
+_* The Greedy label mapping is exponential in number of inputs (see [this paper](https://arxiv.org/abs/2104.01954))._
 
 ## Running time
 
 The algorithm is implemented in pure Python with NumPy for tensor computations. 
 The time complexity is expected to increase exponentially with the number of 
-inputs, but it should be reasonable for combining up to 10 input hypotheses.
+inputs, but it should be reasonable for combining up to 10 input hypotheses. For 
+combining more than 10 inputs, we recommend setting `--label-mapping hungarian`.
 
 For smaller number of inputs (up to 5), the algorithm should take only a few seconds
 to run on a laptop.
 
 ## Combining 2 systems with DOVER-Lap
 
 DOVER-Lap is meant to be used to combine **more than 2 systems**, since
 black-box voting between 2 systems does not make much sense. Still, if 2 systems
 are provided as input, we fall back on the Hungarian algorithm for label mapping,
 since it is provably optimal for this case. Both the systems are assigned equal
-weights, and in case of voting conflicts, the region is equally divided among the
-two labels. This is not the intended use case and will almost certainly lead
+weights, and in case of voting conflicts, the region is assigned to both
+labels. This is not the intended use case and will almost certainly lead
 to performance degradation.
 
 ## Citation
 
 ```
 @article{Raj2021Doverlap,
   title={{DOVER-Lap}: A Method for Combining Overlap-aware Diarization Outputs},
   author={D.Raj and P.Garcia and Z.Huang and S.Watanabe and D.Povey and A.Stolcke and S.Khudanpur},
   journal={2021 IEEE Spoken Language Technology Workshop (SLT)},
   year={2021}
 }
+
+@article{Raj2021ReformulatingDL,
+  title={Reformulating {DOVER-Lap} Label Mapping as a Graph Partitioning Problem},
+  author={Desh Raj and S. Khudanpur},
+  journal={INTERSPEECH},
+  year={2021},
+}
 ```
 
 ## Contact
 
 For issues/bug reports, please raise an Issue in this repository, or reach out to me at `draj@cs.jhu.edu`.
```

### Comparing `dover-lap-1.1.0/dover_lap/dover_lap.py` & `dover-lap-1.2.0/dover_lap/dover_lap.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,39 +62,32 @@
     "--label-mapping",
     type=click.Choice(["hungarian", "greedy"]),
     default="greedy",
     show_default=True,
     help="Choose label mapping algorithm to use",
 )
 @click.option(
-    "--sort-first",
-    is_flag=True,
-    default=False,
-    show_default=True,
-    help="If this flag is set, sort inputs by DER first before label mapping "
-    "(only applicable when label mapping type is hungarian)",
-)
-@click.option(
     "--second-maximal",
     is_flag=True,
     default=False,
     show_default=True,
     help="If this flag is set, run a second iteration of the maximal matching for"
     " greedy label mapping",
 )
 @click.option(
-    "--tie-breaking",
-    type=click.Choice(["uniform", "all"]),
-    default="all",
-    help="Specify whether to assign tied regions to all speakers or divide uniformly",
+    "--voting-method",
+    type=click.Choice(["average"]),
+    default="average",
     show_default=True,
+    help="Choose voting method to use:"
+    " average: use weighted average to combine input RTTMs",
 )
 @click.option(
     "--weight-type",
-    type=click.Choice(["rank", "custom"]),
+    type=click.Choice(["rank", "custom", "norm"]),
     default="rank",
     help="Specify whether to use rank weighting or provide custom weights",
     show_default=True,
 )
 @click.option(
     "--dover-weight",
     type=float,
@@ -103,15 +96,15 @@
     show_default=True,
 )
 @click.option(
     "--custom-weight", cls=PythonLiteralOption, help="Weights for input RTTMs"
 )
 @click.command(
     cls=command_required_option(
-        "weight_type", {"custom": "custom_weight", "rank": "dover_weight"}
+        "weight_type", {"custom": "custom_weight", "rank": "dover_weight", "norm": None}
     )
 )
 def main(
     input_rttms: List[click.Path],
     output_rttm: click.Path,
     uem_file: click.Path,
     channel: int,
```

### Comparing `dover-lap-1.1.0/dover_lap/libs/rttm.py` & `dover-lap-1.2.0/dover_lap/libs/rttm.py`

 * *Files identical despite different names*

### Comparing `dover-lap-1.1.0/dover_lap/libs/turn.py` & `dover-lap-1.2.0/dover_lap/libs/turn.py`

 * *Files identical despite different names*

### Comparing `dover-lap-1.1.0/dover_lap/libs/uem.py` & `dover-lap-1.2.0/dover_lap/libs/uem.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,21 +5,18 @@
 file that will be scored.
 
 Taken from https://github.com/nryant/dscore
 """
 from collections import defaultdict
 from collections.abc import MutableMapping
 
-import itertools
 import os
 
 from intervaltree import IntervalTree
 
-from .utils import format_float
-
 
 class UEM(MutableMapping):
     """Un-partitioned evaluation map (UEM).
 
     A UEM defines a mapping from file ids to scoring regions.
     """
```

### Comparing `dover-lap-1.1.0/dover_lap/libs/utils.py` & `dover-lap-1.2.0/dover_lap/libs/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,31 +60,38 @@
 
 def groupby(iterable, keyfunc):
     """Wrapper around ``itertools.groupby`` which sorts data first."""
     iterable = sorted(iterable, key=keyfunc)
     for key, group in itertools.groupby(iterable, keyfunc):
         yield key, group
 
+
 # If an option is selected, other options become required
 def command_required_option(require_name, require_map):
     class CommandOptionRequiredClass(click.Command):
         def invoke(self, ctx):
             require = ctx.params[require_name]
             if require not in require_map:
                 raise click.ClickException(
-                    "Unexpected value for --'{}': {}".format(
-                        require_name, require))
-            if ctx.params[require_map[require].lower()] is None:
+                    "Unexpected value for --'{}': {}".format(require_name, require)
+                )
+            if (
+                require_map[require] is not None
+                and ctx.params[require_map[require].lower()] is None
+            ):
                 raise click.ClickException(
                     "With {}={} must specify option --{}".format(
-                        require_name, require, require_map[require]))
+                        require_name, require, require_map[require]
+                    )
+                )
             super(CommandOptionRequiredClass, self).invoke(ctx)
 
     return CommandOptionRequiredClass
 
+
 # Class to accept list of arguments as Click option
 class PythonLiteralOption(click.Option):
     def type_cast_value(self, ctx, value):
         try:
             return ast.literal_eval(value)
         except:
             return None
```

### Comparing `dover-lap-1.1.0/dover_lap/src/doverlap.py` & `dover-lap-1.2.0/dover_lap/src/doverlap.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,52 +1,62 @@
 import numpy as np
 
 from typing import List, Union, Optional
 
-from dover_lap.libs.turn import Turn
+from dover_lap.libs.turn import Turn, merge_turns
 from dover_lap.src.label_mapping import LabelMapping
 from dover_lap.src.label_voting import LabelVoting
 
 
 class DOVERLap:
     @classmethod
     def combine_turns_list(
         cls,
         turns_list: List[List[Turn]],
         file_id: str,
         label_mapping: Optional[str] = "greedy",
-        sort_first: Optional[bool] = False,
         second_maximal: Optional[bool] = False,
-        tie_breaking: Optional[str] = "uniform",
+        voting_method: Optional[str] = "average",
         weight_type: Optional[str] = "rank",
         dover_weight: Optional[float] = 0.1,
         custom_weight: Optional[List[str]] = None,
     ) -> List[List[Turn]]:
 
         # Label mapping stage
-        mapped_turns_list, ranks = LabelMapping.get_mapped_turns_list(
+        mapped_turns_list, weights = LabelMapping.get_mapped_turns_list(
             turns_list,
             file_id,
             method=label_mapping,
             second_maximal=second_maximal,
-            sort_first=sort_first,
         )
 
         # Compute weights based on rank
         if weight_type == "rank":
+            ranks = cls.__get_ranks(weights)
             weights = cls.__compute_weights(ranks, dover_weight)
-        else:
+        elif weight_type == "custom":
             assert isinstance(custom_weight, list)
             weights = np.array([float(x) for x in custom_weight])
+        elif weight_type == "norm":
+            weights /= np.linalg.norm(weights, ord=1)  # use normalized weights
 
         # Label voting stage
         combined_turns_list = LabelVoting.get_combined_turns(
-            mapped_turns_list, file_id, tie_breaking, weights
+            mapped_turns_list, file_id, voting_method, weights
         )
-
+        # Merge consecutive turns with the same label
+        combined_turns_list = merge_turns(combined_turns_list)
         return combined_turns_list
 
+    def __get_ranks(weights: np.array) -> np.array:
+
+        weights /= np.linalg.norm(weights, ord=1)
+        temp = weights.argsort()
+        ranks = np.empty_like(temp)
+        ranks[temp] = np.arange(len(weights)) + 1
+        return ranks
+
     def __compute_weights(ranks: np.array, weight: float) -> np.array:
 
         out_weights = 1 / np.power(ranks, weight)
         out_weights /= np.linalg.norm(out_weights, ord=1)
         return out_weights
```

### Comparing `dover-lap-1.1.0/dover_lap/src/label_mapping.py` & `dover-lap-1.2.0/dover_lap/src/label_mapping.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,32 @@
-import numpy as np
-import sys
+from typing import List, Dict, Optional
 
-from typing import List, Dict, Tuple, Optional
-
-from dover_lap.libs.utils import groupby, info
+from dover_lap.libs.utils import groupby
 from dover_lap.libs.turn import Turn
 
 from dover_lap.src.mapping import HungarianMap, GreedyMap
 
 
 class LabelMapping:
     @classmethod
     def get_mapped_turns_list(
         cls,
         turns_list: List[List[Turn]],
         file_id: str,
         method: Optional[str] = "greedy",
-        sort_first: Optional[bool] = False,
         second_maximal: Optional[bool] = False,
     ) -> List[List[Turn]]:
         """
         This function takes turns list from all RTTMs and applies an n-dimensional
         matching approximation algorithm to map all to a common label space.
         """
 
         if (len(turns_list) == 2) or (method == "hungarian"):
             # We replace the original turns list with one sorted by average DER
-            hungarian_map = HungarianMap(sort_first=sort_first)
+            hungarian_map = HungarianMap()
             label_mapping, weights = hungarian_map.compute_mapping(turns_list)
             turns_list = hungarian_map.sorted_turns_list
 
         elif method == "greedy":
             greedy_map = GreedyMap(second_maximal=second_maximal)
             label_mapping, weights = greedy_map.compute_mapping(turns_list)
 
@@ -51,17 +47,8 @@
                             turn.offset,
                             speaker_id=new_spk_id,
                             file_id=file_id,
                         )
                     )
             mapped_turns_list.append(mapped_turns)
 
-        ranks = cls.__get_ranks(weights)
-        return mapped_turns_list, ranks
-
-    def __get_ranks(weights: np.array) -> np.array:
-
-        weights /= np.linalg.norm(weights, ord=1)
-        temp = weights.argsort()
-        ranks = np.empty_like(temp)
-        ranks[temp] = np.arange(len(weights)) + 1
-        return ranks
+        return mapped_turns_list, weights
```

### Comparing `dover-lap-1.1.0/dover_lap/src/label_voting.py` & `dover-lap-1.2.0/dover_lap/src/label_voting.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,103 +1,71 @@
 import numpy as np
 
 from typing import List, Optional, Tuple
 
 from dover_lap.libs.turn import Turn
+from dover_lap.src.voting import WeightedAverageVoting
 
 
 class LabelVoting:
     EPS = 1e-3  # to avoid float equality check errors
 
     @classmethod
-    def get_combined_turns(cls,
-        turns_list: List[Turn],
+    def get_combined_turns(
+        cls,
+        turns_list: List[List[Turn]],
         file_id: str,
-        tie_breaking: Optional[str]='uniform',
-        weights: Optional[np.array]=None
+        voting_method: Optional[str] = "average",
+        weights: Optional[np.array] = None,
     ) -> List[Turn]:
         """
         Implements combination using the DOVER-Lap label voting method.
-        :param turns_list, list of mapped speaker turns
+        :param turns_list, list of mapped speaker turns (from each hypothesis)
         :param file_id, name of the file (recording/session)
-        :param tie_breaking, which method to use for breaking ties. Options:
-            - `uniform`: divide ties uniformly between speakers
-            - `all`: assign region to all tied speakers
+        :param voting_method, which method to use for combining labels. Options:
+            - `average`: use weighted average of labels
+            - `hmm`: use a HMM-based voting method
         :param weights, hypothesis weights to use for rank weighting
         """
-        combined_turns_list = []
-        regions = cls.__get_regions(turns_list, weights)
+        regions, start_end = cls.__get_regions(turns_list, weights)
 
-        for region in regions:
-            # Remove problematic regions
-            if np.abs(region[1] - region[0]) < cls.EPS:
-                continue
-            
-            # Get a list of speakers in this region in decreasing order of their weights
-            spk_weights = sorted(region[2], key=lambda x: x[1], reverse=True)
-
-            # Estimate the number of speakers in this region. This is computing by
-            # adding all the speaker weights in this region (which is simply equal
-            # to the weighted mean of number of speakers in the hypotheses).
-            num_spk = int(round(sum([spk_weights[1] for spk_weights in region[2]])))
-            
-            i = 0
-            while i < num_spk and len(spk_weights) > 0:
-                cur_weight = spk_weights[0][1]
-                filtered_ids = [
-                    spk_id
-                    for (spk_id, weight) in spk_weights
-                    if np.abs(weight - cur_weight) < cls.EPS
-                ]
+        if voting_method == "average":
+            voter = WeightedAverageVoting()
+        else:
+            raise ValueError("Unknown voting method: {}".format(voting_method))
 
-                for j, spk_id in enumerate(filtered_ids):
-                    if tie_breaking == 'uniform':
-                        dur = (region[1] - region[0]) / len(filtered_ids)
-                        start_time = region[0] + j * dur
-                        offset = region[0] + (j + 1) * dur
-                    elif tie_breaking == 'all':
-                        start_time = region[0]
-                        offset = region[1]
-                
-                    turn = Turn(
-                        start_time,
-                        offset=offset,
-                        speaker_id=spk_id,
-                        file_id=file_id,
-                    )
-                    combined_turns_list.append(turn)
-                    
-                i += len(filtered_ids)
-                spk_weights = spk_weights[
-                    len(filtered_ids) :
-                ]  # remove the spk ids that have been seen
+        combined_turns_list = voter.get_combined_turns(regions, start_end, file_id)
 
         return combined_turns_list
 
     @classmethod
-    def __get_regions(cls,
-        turns_list: List[Turn],
-        weights: Optional[np.array]=None
-    ) -> List[Tuple[float,float,List[Tuple[int,float]]]]:
+    def __get_regions(
+        cls, turns_list: List[List[Turn]], weights: Optional[np.array] = None
+    ) -> List[Tuple[float, float, List[Tuple[int, float]]]]:
         """
-        Returns homogeneous time regions of the inputs as list of tuples. Regions are
-        demarcated by start or end times of speaker intervals in any of the input
-        hypothesis. Each region tuple also contains a list of the speakers (along
-        with their weights) in that region.
+        Returns homogeneous time regions of the input.
         """
+        # Map speaker ids to consecutive integers (0, 1, 2, ...)
+        spk_index = {}
+        for turns in turns_list:
+            for turn in turns:
+                if turn.speaker_id not in spk_index:
+                    spk_index[turn.speaker_id] = len(spk_index)
+
+        # Add weights to turns, and update speaker id
         if weights is None:
             weights = np.array([1] * len(turns_list))
         weighted_turns_list = []
 
         for turns, weight in zip(turns_list, weights):
             weighted_turns = [
                 Turn(
                     turn.onset,
                     offset=turn.offset,
-                    speaker_id=turn.speaker_id,
+                    speaker_id=spk_index[turn.speaker_id],
                     file_id=turn.file_id,
                     weight=weight,
                 )
                 for turn in turns
             ]
             weighted_turns_list.append(weighted_turns)
         all_turns = [turn for turns in weighted_turns_list for turn in turns]
@@ -106,30 +74,40 @@
         for turn in all_turns:
             # Name is 'START' (not 'BEG') so that 'END' tokens come first for same timestamp
             tokens.append(("START", turn.onset, turn.speaker_id, turn.weight))
             tokens.append(("END", turn.offset, turn.speaker_id, turn.weight))
 
         sorted_tokens = sorted(tokens, key=lambda x: (x[1], x[0]))
 
-        regions = []
+        regions_list = []
         region_start = sorted_tokens[0][1]
         running_speakers_dict = {sorted_tokens[0][2]: sorted_tokens[0][3]}
         for token in sorted_tokens[1:]:
-            if token[1] > region_start:
+            if token[1] - region_start > cls.EPS:
                 running_speakers = [
                     (k, v) for k, v in running_speakers_dict.items() if v > 0
                 ]
                 if len(running_speakers) > 0:
-                    regions.append((region_start, token[1], running_speakers.copy()))
+                    regions_list.append(
+                        (region_start, token[1], running_speakers.copy())
+                    )
             if token[0] == "START":
                 if token[2] in running_speakers_dict:
                     running_speakers_dict[token[2]] += token[3]
                 else:
                     running_speakers_dict[token[2]] = token[3]
             else:
                 running_speakers_dict[token[2]] -= token[3]
                 if running_speakers_dict[token[2]] <= cls.EPS:
                     running_speakers_dict[token[2]] = 0
             region_start = token[1]
 
-        return regions
-        
+        # Build regions matrix and start_end matrix
+        regions = np.zeros((len(regions_list), len(spk_index)), dtype=np.float32)
+        start_end = np.zeros((len(regions_list), 2), dtype=np.float32)
+        for i, region in enumerate(regions_list):
+            start_end[i, 0] = region[0]
+            start_end[i, 1] = region[1]
+            for spk, weight in region[2]:
+                regions[i, spk] = weight
+
+        return regions, start_end
```

### Comparing `dover-lap-1.1.0/dover_lap/src/mapping/greedy.py` & `dover-lap-1.2.0/dover_lap/src/mapping/greedy.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         weights = np.array([0] * N, dtype=float)
         for i in range(N):
             cur_pairwise_costs = [
                 np.squeeze(x) for x in pairwise_costs.values() if x.shape[i] != 1
             ]
             weights[i] = -1 * sum([np.sum(x) for x in cur_pairwise_costs])
 
-        label_mapping = self.__apply_maximal_matching(
+        label_mapping = self._apply_maximal_matching(
             cost_tensor,
             get_speaker_keys(turns_list),
         )
         return (label_mapping, weights)
 
     def compute_cost_tensor(self, turns_list: List[List[Turn]]) -> np.ndarray:
 
@@ -91,15 +91,15 @@
             for val in vals[1:]:
                 cost_tensor = np.add(cost_tensor, val)
         else:
             # otherwise use broadcasting
             cost_tensor = np.sum(list(pairwise_costs.values()))
         return cost_tensor, pairwise_costs
 
-    def __apply_maximal_matching(
+    def _apply_maximal_matching(
         self,
         cost_tensor: np.ndarray,
         speakers_dict: Dict[Tuple[int, int], str],
     ) -> List[List[Turn]]:
 
         # Sort the cost tensor
         sorted_idx = np.transpose(
@@ -117,32 +117,32 @@
             info(
                 "Iteration {}: {} labels left to be mapped".format(
                     iter,
                     sum([len(v) for v in remaining_idx.values()]),
                 ),
                 file=sys.stderr,
             )
-            sorted_idx_filtered = self.__filter_sorted_index_list(
+            sorted_idx_filtered = self._filter_sorted_index_list(
                 sorted_idx, remaining_idx
             )
 
             # find initial maximal matching
             M_cur = []
             for idx in sorted_idx_filtered:
-                if not self.__contradicts(M_cur, idx):
+                if not self._contradicts(M_cur, idx):
                     M_cur.append(idx)
 
             if self.second_maximal:
                 # find second maximal matching
                 change = True
                 while change:
                     change = False
                     for idx in list(M_cur):
                         M_cur.remove(idx)
-                        M_r = self.__find_remaining_maximal_matching(
+                        M_r = self._find_remaining_maximal_matching(
                             M_cur, sorted_idx_filtered
                         )
                         if len(M_r) > 1:
                             M_cur = M_cur + M_r
                             change = True
                         else:
                             M_cur.append(idx)
@@ -165,35 +165,35 @@
             for i, j in enumerate(idx_tuple):
                 old_spk_id = speakers_dict[(i, j)]
                 if (i, old_spk_id) not in label_mapping:
                     label_mapping[(i, old_spk_id)] = k
 
         return label_mapping
 
-    def __find_remaining_maximal_matching(
+    def _find_remaining_maximal_matching(
         self, M: List[Dict[int, int]], idx_list: List[Tuple[int, int]]
     ) -> List[Tuple[int, int]]:
         """
         Given a list of index tuples and a matching M, find a maximal
         matching on the "remaining" list, i.e., using only those index
         tuples which are not present in the original matching.
         """
         S_r = []
         for idx in list(idx_list):
-            if not self.__contradicts(M, idx):
+            if not self._contradicts(M, idx):
                 S_r.append(idx)
 
         M_r = []
         for idx in S_r:
-            if not self.__contradicts(M_r, idx):
+            if not self._contradicts(M_r, idx):
                 M_r.append(idx)
 
         return M_r
 
-    def __filter_sorted_index_list(
+    def _filter_sorted_index_list(
         self, sorted_idx: List[np.ndarray], remaining_idx: List[Tuple[int, int]]
     ) -> List[np.ndarray]:
         """
         Filter the sorted list of index tuples to only retain tuples for which
         at least one element is in the remaining list.
         """
         sorted_idx_filtered = []
@@ -203,15 +203,15 @@
                 if i in remaining_idx and j in remaining_idx[i]:
                     remaining = True
                     break
             if remaining:
                 sorted_idx_filtered.append(idx_tuple)
         return sorted_idx_filtered
 
-    def __contradicts(self, M: List[Dict[int, int]], idx_tuple: List[int]) -> bool:
+    def _contradicts(self, M: List[Dict[int, int]], idx_tuple: List[int]) -> bool:
         """
         Check if an index tuple contradicts a matching, i.e. return True if
         any index in the tuple is already present in the matching.
         """
         for i, index in enumerate(idx_tuple):
             existing_idx = [idx[i] for idx in M]
             if index in existing_idx:
```

### Comparing `dover-lap-1.1.0/dover_lap/src/mapping/map_utils.py` & `dover-lap-1.2.0/dover_lap/src/mapping/map_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,12 @@
-import sys
-import random
+from typing import List, Dict, Tuple
 
-from typing import List, Dict, Tuple, Optional
-from collections import defaultdict
-
-from dover_lap.libs.utils import groupby, info
+from dover_lap.libs.utils import groupby
 from dover_lap.libs.turn import Turn
 
-import numpy as np
-
 
 def compute_spk_overlap(ref_spk_turns: List[Turn], sys_spk_turns: List[Turn]) -> float:
     """
     Computes 'relative' overlap, i.e. Intersection Over Union
     """
     tokens = []
     all_turns = ref_spk_turns + sys_spk_turns
```

### Comparing `dover-lap-1.1.0/dover_lap.egg-info/SOURCES.txt` & `dover-lap-1.2.0/dover_lap.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,28 @@
+LICENSE
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
 dover_lap/__init__.py
 dover_lap/dover_lap.py
 dover_lap.egg-info/PKG-INFO
 dover_lap.egg-info/SOURCES.txt
 dover_lap.egg-info/dependency_links.txt
 dover_lap.egg-info/entry_points.txt
 dover_lap.egg-info/requires.txt
 dover_lap.egg-info/top_level.txt
 dover_lap/libs/__init__.py
-dover_lap/libs/metrics.py
 dover_lap/libs/rttm.py
 dover_lap/libs/turn.py
 dover_lap/libs/uem.py
 dover_lap/libs/utils.py
 dover_lap/src/__init__.py
 dover_lap/src/doverlap.py
 dover_lap/src/label_mapping.py
 dover_lap/src/label_voting.py
 dover_lap/src/mapping/__init__.py
 dover_lap/src/mapping/greedy.py
 dover_lap/src/mapping/hungarian.py
-dover_lap/src/mapping/map_utils.py
+dover_lap/src/mapping/map_utils.py
+dover_lap/src/voting/__init__.py
+dover_lap/src/voting/average.py
```

### Comparing `dover-lap-1.1.0/setup.py` & `dover-lap-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 long_description = open("README.md").read()
 
 dev_requires = ["pre-commit", "black", "flake8"]
 
 setup(
     name="dover-lap",
-    version="1.1.0",
+    version="1.2.0",
     author="Desh Raj",
     author_email="r.desh26@gmail.com",
     description="Combine overlap-aware diarization output RTTMs",
     keywords="diarization dover",
     url="https://github.com/desh2608/dover-lap",
     license="Apache-2.0 License",
     packages=find_packages(),
```

