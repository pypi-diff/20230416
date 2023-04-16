# Comparing `tmp/pomegranate-0.9.0.tar.gz` & `tmp/pomegranate-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pomegranate-0.9.0.tar", last modified: Wed Jan  3 10:56:54 2018, max compression
+gzip compressed data, was "pomegranate-1.0.0.tar", last modified: Sun Apr 16 07:10:25 2023, max compression
```

## Comparing `pomegranate-0.9.0.tar` & `pomegranate-1.0.0.tar`

### file list

```diff
@@ -1,33 +1,43 @@
-drwxr-xr-x   0 jmschr    (1000) jmschr    (1000)        0 2018-01-03 10:56:54.000000 pomegranate-0.9.0/
--rw-r--r--   0 jmschr    (1000) jmschr    (1000)       38 2018-01-03 10:56:54.000000 pomegranate-0.9.0/setup.cfg
--rw-r--r--   0 jmschr    (1000) jmschr    (1000)      127 2017-12-26 23:18:46.000000 pomegranate-0.9.0/dev-requirements.txt
--rw-r--r--   0 jmschr    (1000) jmschr    (1000)     1905 2018-01-03 09:28:23.000000 pomegranate-0.9.0/setup.py
--rw-r--r--   0 jmschr    (1000) jmschr    (1000)     6313 2017-11-06 03:56:57.000000 pomegranate-0.9.0/README.md
--rw-r--r--   0 jmschr    (1000) jmschr    (1000)       64 2017-08-09 21:31:35.000000 pomegranate-0.9.0/MANIFEST.in
--rw-r--r--   0 jmschr    (1000) jmschr    (1000)      359 2018-01-03 10:56:54.000000 pomegranate-0.9.0/PKG-INFO
-drwxr-xr-x   0 jmschr    (1000) jmschr    (1000)        0 2018-01-03 10:56:54.000000 pomegranate-0.9.0/pomegranate/
--rw-r--r--   0 jmschr    (1000) jmschr    (1000)      615 2018-01-03 09:28:21.000000 pomegranate-0.9.0/pomegranate/__init__.py
--rw-r--r--   0 jmschr    (1000) jmschr    (1000)      582 2017-05-25 07:51:12.000000 pomegranate-0.9.0/pomegranate/bayes.pxd
--rw-r--r--   0 jmschr    (1000) jmschr    (1000)   610446 2018-01-01 19:54:28.000000 pomegranate-0.9.0/pomegranate/base.c
--rw-r--r--   0 jmschr    (1000) jmschr    (1000)  3742129 2018-01-03 10:44:00.000000 pomegranate-0.9.0/pomegranate/distributions.c
--rw-r--r--   0 jmschr    (1000) jmschr    (1000)   584349 2018-01-01 19:54:25.000000 pomegranate-0.9.0/pomegranate/utils.c
--rw-r--r--   0 jmschr    (1000) jmschr    (1000)      679 2017-10-28 00:25:26.000000 pomegranate-0.9.0/pomegranate/base.pxd
--rw-r--r--   0 jmschr    (1000) jmschr    (1000)  1315374 2018-01-02 05:09:31.000000 pomegranate-0.9.0/pomegranate/gmm.c
--rw-r--r--   0 jmschr    (1000) jmschr    (1000)     3378 2017-12-27 00:49:06.000000 pomegranate-0.9.0/pomegranate/distributions.pxd
--rw-r--r--   0 jmschr    (1000) jmschr    (1000)   455538 2018-01-01 19:53:39.000000 pomegranate-0.9.0/pomegranate/BayesClassifier.c
--rw-r--r--   0 jmschr    (1000) jmschr    (1000)  3174740 2018-01-02 05:09:44.000000 pomegranate-0.9.0/pomegranate/hmm.c
--rw-r--r--   0 jmschr    (1000) jmschr    (1000)   330190 2017-12-25 03:27:13.000000 pomegranate-0.9.0/pomegranate/MarkovChain.c
--rw-r--r--   0 jmschr    (1000) jmschr    (1000)  1622489 2018-01-01 19:54:06.000000 pomegranate-0.9.0/pomegranate/bayes.c
--rw-r--r--   0 jmschr    (1000) jmschr    (1000)  1267218 2018-01-01 19:53:56.000000 pomegranate-0.9.0/pomegranate/FactorGraph.c
--rw-r--r--   0 jmschr    (1000) jmschr    (1000)   766079 2018-01-01 19:54:23.000000 pomegranate-0.9.0/pomegranate/parallel.c
--rw-r--r--   0 jmschr    (1000) jmschr    (1000)   889971 2018-01-01 19:54:22.000000 pomegranate-0.9.0/pomegranate/kmeans.c
--rw-r--r--   0 jmschr    (1000) jmschr    (1000)  1068940 2018-01-02 05:09:12.000000 pomegranate-0.9.0/pomegranate/NaiveBayes.c
--rw-r--r--   0 jmschr    (1000) jmschr    (1000)      504 2017-12-27 00:49:06.000000 pomegranate-0.9.0/pomegranate/utils.pxd
--rw-r--r--   0 jmschr    (1000) jmschr    (1000)  2930621 2018-01-03 10:43:53.000000 pomegranate-0.9.0/pomegranate/BayesianNetwork.c
-drwxr-xr-x   0 jmschr    (1000) jmschr    (1000)        0 2018-01-03 10:56:54.000000 pomegranate-0.9.0/pomegranate.egg-info/
--rw-r--r--   0 jmschr    (1000) jmschr    (1000)       12 2018-01-03 10:56:54.000000 pomegranate-0.9.0/pomegranate.egg-info/top_level.txt
--rw-r--r--   0 jmschr    (1000) jmschr    (1000)        1 2018-01-03 10:56:54.000000 pomegranate-0.9.0/pomegranate.egg-info/dependency_links.txt
--rw-r--r--   0 jmschr    (1000) jmschr    (1000)      359 2018-01-03 10:56:54.000000 pomegranate-0.9.0/pomegranate.egg-info/PKG-INFO
--rw-r--r--   0 jmschr    (1000) jmschr    (1000)       64 2018-01-03 10:56:54.000000 pomegranate-0.9.0/pomegranate.egg-info/requires.txt
--rw-r--r--   0 jmschr    (1000) jmschr    (1000)      665 2018-01-03 10:56:54.000000 pomegranate-0.9.0/pomegranate.egg-info/SOURCES.txt
--rw-r--r--   0 jmschr    (1000) jmschr    (1000)       74 2017-10-09 16:53:26.000000 pomegranate-0.9.0/requirements.txt
+drwxrwxr-x   0 jmschr    (1000) jmschr    (1000)        0 2023-04-16 07:10:25.796798 pomegranate-1.0.0/
+-rw-rw-r--   0 jmschr    (1000) jmschr    (1000)     1072 2023-04-16 04:43:00.000000 pomegranate-1.0.0/LICENSE
+-rw-rw-r--   0 jmschr    (1000) jmschr    (1000)      272 2023-04-16 07:10:25.796798 pomegranate-1.0.0/PKG-INFO
+-rw-rw-r--   0 jmschr    (1000) jmschr    (1000)     7923 2023-04-16 04:43:00.000000 pomegranate-1.0.0/README.md
+drwxrwxr-x   0 jmschr    (1000) jmschr    (1000)        0 2023-04-16 07:10:25.792798 pomegranate-1.0.0/pomegranate/
+-rw-rw-r--   0 jmschr    (1000) jmschr    (1000)       22 2023-04-16 04:52:26.000000 pomegranate-1.0.0/pomegranate/__init__.py
+-rw-rw-r--   0 jmschr    (1000) jmschr    (1000)     9945 2023-04-16 04:43:00.000000 pomegranate-1.0.0/pomegranate/_bayes.py
+-rw-rw-r--   0 jmschr    (1000) jmschr    (1000)    13465 2023-04-16 04:43:00.000000 pomegranate-1.0.0/pomegranate/_utils.py
+-rw-rw-r--   0 jmschr    (1000) jmschr    (1000)     6669 2023-04-16 04:43:00.000000 pomegranate-1.0.0/pomegranate/bayes_classifier.py
+-rw-rw-r--   0 jmschr    (1000) jmschr    (1000)    36893 2023-04-16 04:53:18.000000 pomegranate-1.0.0/pomegranate/bayesian_network.py
+drwxrwxr-x   0 jmschr    (1000) jmschr    (1000)        0 2023-04-16 07:10:25.796798 pomegranate-1.0.0/pomegranate/distributions/
+-rw-rw-r--   0 jmschr    (1000) jmschr    (1000)      491 2023-04-16 05:16:03.000000 pomegranate-1.0.0/pomegranate/distributions/__init__.py
+-rw-rw-r--   0 jmschr    (1000) jmschr    (1000)     2296 2023-04-16 04:43:00.000000 pomegranate-1.0.0/pomegranate/distributions/_distribution.py
+-rw-rw-r--   0 jmschr    (1000) jmschr    (1000)     6670 2023-04-16 04:43:00.000000 pomegranate-1.0.0/pomegranate/distributions/bernoulli.py
+-rw-rw-r--   0 jmschr    (1000) jmschr    (1000)     7769 2023-04-16 04:43:00.000000 pomegranate-1.0.0/pomegranate/distributions/categorical.py
+-rw-rw-r--   0 jmschr    (1000) jmschr    (1000)     5376 2023-04-16 04:43:00.000000 pomegranate-1.0.0/pomegranate/distributions/conditional_categorical.py
+-rw-rw-r--   0 jmschr    (1000) jmschr    (1000)     5769 2023-04-16 04:43:00.000000 pomegranate-1.0.0/pomegranate/distributions/dirac_delta.py
+-rw-rw-r--   0 jmschr    (1000) jmschr    (1000)     6683 2023-04-16 04:43:00.000000 pomegranate-1.0.0/pomegranate/distributions/exponential.py
+-rw-rw-r--   0 jmschr    (1000) jmschr    (1000)     8337 2023-04-16 04:43:00.000000 pomegranate-1.0.0/pomegranate/distributions/gamma.py
+-rw-rw-r--   0 jmschr    (1000) jmschr    (1000)     6317 2023-04-16 04:43:00.000000 pomegranate-1.0.0/pomegranate/distributions/independent_components.py
+-rw-rw-r--   0 jmschr    (1000) jmschr    (1000)     9269 2023-04-16 04:43:00.000000 pomegranate-1.0.0/pomegranate/distributions/joint_categorical.py
+-rw-rw-r--   0 jmschr    (1000) jmschr    (1000)    10191 2023-04-16 04:43:00.000000 pomegranate-1.0.0/pomegranate/distributions/normal.py
+-rw-rw-r--   0 jmschr    (1000) jmschr    (1000)     6572 2023-04-16 04:43:00.000000 pomegranate-1.0.0/pomegranate/distributions/poisson.py
+-rw-rw-r--   0 jmschr    (1000) jmschr    (1000)     5493 2023-04-16 04:43:00.000000 pomegranate-1.0.0/pomegranate/distributions/student_t.py
+-rw-rw-r--   0 jmschr    (1000) jmschr    (1000)     6961 2023-04-16 04:43:00.000000 pomegranate-1.0.0/pomegranate/distributions/uniform.py
+-rw-rw-r--   0 jmschr    (1000) jmschr    (1000)     8398 2023-04-16 04:51:57.000000 pomegranate-1.0.0/pomegranate/distributions/zero_inflated.py
+-rw-rw-r--   0 jmschr    (1000) jmschr    (1000)    19118 2023-04-16 04:53:35.000000 pomegranate-1.0.0/pomegranate/factor_graph.py
+-rw-rw-r--   0 jmschr    (1000) jmschr    (1000)    11218 2023-04-16 04:43:00.000000 pomegranate-1.0.0/pomegranate/gmm.py
+drwxrwxr-x   0 jmschr    (1000) jmschr    (1000)        0 2023-04-16 07:10:25.796798 pomegranate-1.0.0/pomegranate/hmm/
+-rw-rw-r--   0 jmschr    (1000) jmschr    (1000)      133 2023-04-16 04:43:00.000000 pomegranate-1.0.0/pomegranate/hmm/__init__.py
+-rw-rw-r--   0 jmschr    (1000) jmschr    (1000)    24250 2023-04-16 04:43:00.000000 pomegranate-1.0.0/pomegranate/hmm/_base.py
+-rw-rw-r--   0 jmschr    (1000) jmschr    (1000)    21664 2023-04-16 04:43:00.000000 pomegranate-1.0.0/pomegranate/hmm/dense_hmm.py
+-rw-rw-r--   0 jmschr    (1000) jmschr    (1000)    23282 2023-04-16 04:43:00.000000 pomegranate-1.0.0/pomegranate/hmm/sparse_hmm.py
+-rw-rw-r--   0 jmschr    (1000) jmschr    (1000)    11873 2023-04-16 04:43:00.000000 pomegranate-1.0.0/pomegranate/kmeans.py
+-rw-rw-r--   0 jmschr    (1000) jmschr    (1000)     9465 2023-04-16 04:43:00.000000 pomegranate-1.0.0/pomegranate/markov_chain.py
+drwxrwxr-x   0 jmschr    (1000) jmschr    (1000)        0 2023-04-16 07:10:25.792798 pomegranate-1.0.0/pomegranate.egg-info/
+-rw-rw-r--   0 jmschr    (1000) jmschr    (1000)      272 2023-04-16 07:10:25.000000 pomegranate-1.0.0/pomegranate.egg-info/PKG-INFO
+-rw-rw-r--   0 jmschr    (1000) jmschr    (1000)     1163 2023-04-16 07:10:25.000000 pomegranate-1.0.0/pomegranate.egg-info/SOURCES.txt
+-rw-rw-r--   0 jmschr    (1000) jmschr    (1000)        1 2023-04-16 07:10:25.000000 pomegranate-1.0.0/pomegranate.egg-info/dependency_links.txt
+-rw-rw-r--   0 jmschr    (1000) jmschr    (1000)       98 2023-04-16 07:10:25.000000 pomegranate-1.0.0/pomegranate.egg-info/requires.txt
+-rw-rw-r--   0 jmschr    (1000) jmschr    (1000)       12 2023-04-16 07:10:25.000000 pomegranate-1.0.0/pomegranate.egg-info/top_level.txt
+-rw-rw-r--   0 jmschr    (1000) jmschr    (1000)       38 2023-04-16 07:10:25.796798 pomegranate-1.0.0/setup.cfg
+-rw-rw-r--   0 jmschr    (1000) jmschr    (1000)      523 2023-04-16 05:25:56.000000 pomegranate-1.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

