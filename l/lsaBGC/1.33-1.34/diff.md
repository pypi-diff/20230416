# Comparing `tmp/lsaBGC-1.33.tar.gz` & `tmp/lsaBGC-1.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsaBGC-1.33.tar", last modified: Thu Mar  2 20:49:38 2023, max compression
+gzip compressed data, was "lsaBGC-1.34.tar", last modified: Sun Apr 16 16:19:05 2023, max compression
```

## Comparing `lsaBGC-1.33.tar` & `lsaBGC-1.34.tar`

### file list

```diff
@@ -1,42 +1,45 @@
-drwxrwxr-x   0 salamzade  (1010) salamzade  (1011)        0 2023-03-02 20:49:38.156970 lsaBGC-1.33/
--rwxrwxr-x   0 salamzade  (1010) salamzade  (1011)     1517 2023-01-16 18:04:03.000000 lsaBGC-1.33/LICENSE
--rw-rw-r--   0 salamzade  (1010) salamzade  (1011)      398 2023-03-02 20:49:38.156970 lsaBGC-1.33/PKG-INFO
--rwxrwxr-x   0 salamzade  (1010) salamzade  (1011)    17314 2023-03-02 18:46:47.000000 lsaBGC-1.33/README.md
-drwxrwxr-x   0 salamzade  (1010) salamzade  (1011)        0 2023-03-02 20:49:38.152970 lsaBGC-1.33/bin/
--rwxrwxr-x   0 salamzade  (1010) salamzade  (1011)     8594 2023-01-16 18:04:03.000000 lsaBGC-1.33/bin/lsaBGC-Cluster.py
--rwxrwxr-x   0 salamzade  (1010) salamzade  (1011)    13282 2023-01-16 18:06:00.000000 lsaBGC-1.33/bin/lsaBGC-DiscoVary.py
--rwxrwxr-x   0 salamzade  (1010) salamzade  (1011)    10520 2023-01-16 18:04:03.000000 lsaBGC-1.33/bin/lsaBGC-Divergence.py
--rwxrwxr-x   0 salamzade  (1010) salamzade  (1011)    14715 2023-01-16 18:04:03.000000 lsaBGC-1.33/bin/lsaBGC-Expansion.py
--rwxrwxr-x   0 salamzade  (1010) salamzade  (1011)    13175 2023-01-16 18:04:03.000000 lsaBGC-1.33/bin/lsaBGC-PopGene.py
--rw-rw-r--   0 salamzade  (1010) salamzade  (1011)    36269 2023-02-28 18:51:49.000000 lsaBGC-1.33/bin/lsaBGC-Ready.py
--rwxrwxr-x   0 salamzade  (1010) salamzade  (1011)     7712 2023-01-16 18:04:03.000000 lsaBGC-1.33/bin/lsaBGC-Refiner.py
--rwxrwxr-x   0 salamzade  (1010) salamzade  (1011)    11201 2023-01-16 18:04:03.000000 lsaBGC-1.33/bin/lsaBGC-See.py
-drwxrwxr-x   0 salamzade  (1010) salamzade  (1011)        0 2023-03-02 20:49:38.152970 lsaBGC-1.33/lsaBGC/
--rwxrwxr-x   0 salamzade  (1010) salamzade  (1011)        0 2023-01-16 18:04:03.000000 lsaBGC-1.33/lsaBGC/__init__.py
--rwxrwxr-x   0 salamzade  (1010) salamzade  (1011)    14437 2023-01-16 18:04:03.000000 lsaBGC-1.33/lsaBGC/processing.py
--rwxrwxr-x   0 salamzade  (1010) salamzade  (1011)   110406 2023-02-28 19:28:24.000000 lsaBGC-1.33/lsaBGC/util.py
-drwxrwxr-x   0 salamzade  (1010) salamzade  (1011)        0 2023-03-02 20:49:38.152970 lsaBGC-1.33/lsaBGC.egg-info/
--rw-rw-r--   0 salamzade  (1010) salamzade  (1011)      398 2023-03-02 20:49:38.000000 lsaBGC-1.33/lsaBGC.egg-info/PKG-INFO
--rw-rw-r--   0 salamzade  (1010) salamzade  (1011)      936 2023-03-02 20:49:38.000000 lsaBGC-1.33/lsaBGC.egg-info/SOURCES.txt
--rw-rw-r--   0 salamzade  (1010) salamzade  (1011)        1 2023-03-02 20:49:38.000000 lsaBGC-1.33/lsaBGC.egg-info/dependency_links.txt
--rw-rw-r--   0 salamzade  (1010) salamzade  (1011)        1 2023-03-02 20:49:38.000000 lsaBGC-1.33/lsaBGC.egg-info/not-zip-safe
--rw-rw-r--   0 salamzade  (1010) salamzade  (1011)        7 2023-03-02 20:49:38.000000 lsaBGC-1.33/lsaBGC.egg-info/top_level.txt
-drwxrwxr-x   0 salamzade  (1010) salamzade  (1011)        0 2023-03-02 20:49:38.152970 lsaBGC-1.33/scripts/
--rw-rw-r--   0 salamzade  (1010) salamzade  (1011)    23594 2023-03-02 18:47:51.000000 lsaBGC-1.33/scripts/GSeeF.py
--rw-rw-r--   0 salamzade  (1010) salamzade  (1011)     7624 2023-01-16 18:04:03.000000 lsaBGC-1.33/scripts/compareBGCtoGenomeCodonUsage.py
--rw-rw-r--   0 salamzade  (1010) salamzade  (1011)     2984 2023-01-16 18:04:03.000000 lsaBGC-1.33/scripts/createPickleOfSampleAnnotationListingFile.py
--rw-rw-r--   0 salamzade  (1010) salamzade  (1011)     6276 2023-01-16 18:04:03.000000 lsaBGC-1.33/scripts/listAllBGCGenbanksInDirectory.py
--rw-rw-r--   0 salamzade  (1010) salamzade  (1011)    10399 2023-01-16 18:04:03.000000 lsaBGC-1.33/scripts/listAllGenomesInDirectory.py
--rw-rw-r--   0 salamzade  (1010) salamzade  (1011)    16757 2023-01-16 18:04:03.000000 lsaBGC-1.33/scripts/popSizeAndSampleSelector.py
--rw-rw-r--   0 salamzade  (1010) salamzade  (1011)     7962 2023-01-16 18:04:03.000000 lsaBGC-1.33/scripts/processAndReformatNCBIGenbanks.py
--rw-rw-r--   0 salamzade  (1010) salamzade  (1011)     8298 2023-01-16 18:04:03.000000 lsaBGC-1.33/scripts/readifyAdditionalGenomes.py
--rw-rw-r--   0 salamzade  (1010) salamzade  (1011)     7465 2023-02-21 04:25:25.000000 lsaBGC-1.33/scripts/runProdigalAndMakeProperGenbank.py
--rw-rw-r--   0 salamzade  (1010) salamzade  (1011)     4135 2023-01-16 18:04:03.000000 lsaBGC-1.33/scripts/setup_annotation_dbs.py
--rw-rw-r--   0 salamzade  (1010) salamzade  (1011)     3185 2023-01-16 18:04:03.000000 lsaBGC-1.33/scripts/setup_bigscape.py
--rw-rw-r--   0 salamzade  (1010) salamzade  (1011)     3447 2023-01-16 18:04:03.000000 lsaBGC-1.33/scripts/simpleProteinExtraction.py
--rw-rw-r--   0 salamzade  (1010) salamzade  (1011)       38 2023-03-02 20:49:38.156970 lsaBGC-1.33/setup.cfg
--rwxrwxr-x   0 salamzade  (1010) salamzade  (1011)     1612 2023-03-02 18:22:38.000000 lsaBGC-1.33/setup.py
-drwxrwxr-x   0 salamzade  (1010) salamzade  (1011)        0 2023-03-02 20:49:38.156970 lsaBGC-1.33/workflows/
--rw-rw-r--   0 salamzade  (1010) salamzade  (1011)    30619 2023-01-16 18:04:03.000000 lsaBGC-1.33/workflows/lsaBGC-AutoAnalyze.py
--rw-rw-r--   0 salamzade  (1010) salamzade  (1011)    18129 2023-01-16 18:04:03.000000 lsaBGC-1.33/workflows/lsaBGC-AutoExpansion.py
--rw-rw-r--   0 salamzade  (1010) salamzade  (1011)    43280 2023-03-02 18:34:41.000000 lsaBGC-1.33/workflows/lsaBGC-Easy.py
+drwxrwxr-x   0 rauf      (1000) rauf      (1000)        0 2023-04-16 16:19:05.538323 lsaBGC-1.34/
+-rwxrwxr-x   0 rauf      (1000) rauf      (1000)     1517 2023-04-16 12:26:58.000000 lsaBGC-1.34/LICENSE
+-rw-rw-r--   0 rauf      (1000) rauf      (1000)      398 2023-04-16 16:19:05.538323 lsaBGC-1.34/PKG-INFO
+-rwxrwxr-x   0 rauf      (1000) rauf      (1000)     6374 2023-04-16 12:26:58.000000 lsaBGC-1.34/README.md
+drwxrwxr-x   0 rauf      (1000) rauf      (1000)        0 2023-04-16 16:19:05.534323 lsaBGC-1.34/bin/
+-rwxrwxr-x   0 rauf      (1000) rauf      (1000)     8651 2023-04-16 12:26:58.000000 lsaBGC-1.34/bin/lsaBGC-Cluster.py
+-rwxrwxr-x   0 rauf      (1000) rauf      (1000)    13310 2023-04-16 12:26:58.000000 lsaBGC-1.34/bin/lsaBGC-DiscoVary.py
+-rwxrwxr-x   0 rauf      (1000) rauf      (1000)    10541 2023-04-16 12:26:58.000000 lsaBGC-1.34/bin/lsaBGC-Divergence.py
+-rwxrwxr-x   0 rauf      (1000) rauf      (1000)    14738 2023-04-16 12:26:58.000000 lsaBGC-1.34/bin/lsaBGC-Expansion.py
+-rw-rw-r--   0 rauf      (1000) rauf      (1000)    15751 2023-04-16 12:26:58.000000 lsaBGC-1.34/bin/lsaBGC-MIBiGMapper.py
+-rwxrwxr-x   0 rauf      (1000) rauf      (1000)    12808 2023-04-16 12:26:58.000000 lsaBGC-1.34/bin/lsaBGC-PopGene.py
+-rw-rw-r--   0 rauf      (1000) rauf      (1000)    37287 2023-04-16 13:01:21.000000 lsaBGC-1.34/bin/lsaBGC-Ready.py
+-rwxrwxr-x   0 rauf      (1000) rauf      (1000)     7734 2023-04-16 12:26:58.000000 lsaBGC-1.34/bin/lsaBGC-Refiner.py
+-rwxrwxr-x   0 rauf      (1000) rauf      (1000)    11168 2023-04-16 12:26:58.000000 lsaBGC-1.34/bin/lsaBGC-See.py
+drwxrwxr-x   0 rauf      (1000) rauf      (1000)        0 2023-04-16 16:19:05.534323 lsaBGC-1.34/lsaBGC/
+-rwxrwxr-x   0 rauf      (1000) rauf      (1000)        0 2023-04-16 12:26:58.000000 lsaBGC-1.34/lsaBGC/__init__.py
+-rwxrwxr-x   0 rauf      (1000) rauf      (1000)    14437 2023-04-16 12:26:58.000000 lsaBGC-1.34/lsaBGC/processing.py
+-rwxrwxr-x   0 rauf      (1000) rauf      (1000)   105244 2023-04-16 12:26:58.000000 lsaBGC-1.34/lsaBGC/util.py
+drwxrwxr-x   0 rauf      (1000) rauf      (1000)        0 2023-04-16 16:19:05.534323 lsaBGC-1.34/lsaBGC.egg-info/
+-rw-rw-r--   0 rauf      (1000) rauf      (1000)      398 2023-04-16 16:19:05.000000 lsaBGC-1.34/lsaBGC.egg-info/PKG-INFO
+-rw-rw-r--   0 rauf      (1000) rauf      (1000)     1020 2023-04-16 16:19:05.000000 lsaBGC-1.34/lsaBGC.egg-info/SOURCES.txt
+-rw-rw-r--   0 rauf      (1000) rauf      (1000)        1 2023-04-16 16:19:05.000000 lsaBGC-1.34/lsaBGC.egg-info/dependency_links.txt
+-rw-rw-r--   0 rauf      (1000) rauf      (1000)        1 2023-04-16 16:19:05.000000 lsaBGC-1.34/lsaBGC.egg-info/not-zip-safe
+-rw-rw-r--   0 rauf      (1000) rauf      (1000)        7 2023-04-16 16:19:05.000000 lsaBGC-1.34/lsaBGC.egg-info/top_level.txt
+drwxrwxr-x   0 rauf      (1000) rauf      (1000)        0 2023-04-16 16:19:05.538323 lsaBGC-1.34/scripts/
+-rw-rw-r--   0 rauf      (1000) rauf      (1000)    23594 2023-04-16 12:26:58.000000 lsaBGC-1.34/scripts/GSeeF.py
+-rw-rw-r--   0 rauf      (1000) rauf      (1000)     7624 2023-04-16 12:26:58.000000 lsaBGC-1.34/scripts/compareBGCtoGenomeCodonUsage.py
+-rw-rw-r--   0 rauf      (1000) rauf      (1000)     2984 2023-04-16 12:26:58.000000 lsaBGC-1.34/scripts/createPickleOfSampleAnnotationListingFile.py
+-rw-rw-r--   0 rauf      (1000) rauf      (1000)     6276 2023-04-16 12:26:58.000000 lsaBGC-1.34/scripts/listAllBGCGenbanksInDirectory.py
+-rw-rw-r--   0 rauf      (1000) rauf      (1000)    10399 2023-04-16 12:26:58.000000 lsaBGC-1.34/scripts/listAllGenomesInDirectory.py
+-rw-rw-r--   0 rauf      (1000) rauf      (1000)    16757 2023-04-16 12:26:58.000000 lsaBGC-1.34/scripts/popSizeAndSampleSelector.py
+-rw-rw-r--   0 rauf      (1000) rauf      (1000)     7962 2023-04-16 12:26:58.000000 lsaBGC-1.34/scripts/processAndReformatNCBIGenbanks.py
+-rw-rw-r--   0 rauf      (1000) rauf      (1000)     8298 2023-04-16 12:26:58.000000 lsaBGC-1.34/scripts/readifyAdditionalGenomes.py
+-rw-rw-r--   0 rauf      (1000) rauf      (1000)     7465 2023-04-16 12:26:58.000000 lsaBGC-1.34/scripts/runProdigalAndMakeProperGenbank.py
+-rw-rw-r--   0 rauf      (1000) rauf      (1000)     5055 2023-04-16 12:26:58.000000 lsaBGC-1.34/scripts/setup_annotation_dbs.py
+-rw-rw-r--   0 rauf      (1000) rauf      (1000)     3185 2023-04-16 12:26:58.000000 lsaBGC-1.34/scripts/setup_bigscape.py
+-rw-rw-r--   0 rauf      (1000) rauf      (1000)     3447 2023-04-16 12:26:58.000000 lsaBGC-1.34/scripts/simpleProteinExtraction.py
+-rw-rw-r--   0 rauf      (1000) rauf      (1000)    12961 2023-04-16 12:26:58.000000 lsaBGC-1.34/scripts/visualize_BGC-Ome.py
+-rw-rw-r--   0 rauf      (1000) rauf      (1000)       38 2023-04-16 16:19:05.538323 lsaBGC-1.34/setup.cfg
+-rwxrwxr-x   0 rauf      (1000) rauf      (1000)     1749 2023-04-16 12:26:58.000000 lsaBGC-1.34/setup.py
+drwxrwxr-x   0 rauf      (1000) rauf      (1000)        0 2023-04-16 16:19:05.538323 lsaBGC-1.34/workflows/
+-rw-rw-r--   0 rauf      (1000) rauf      (1000)    37391 2023-04-16 12:26:58.000000 lsaBGC-1.34/workflows/lsaBGC-AutoAnalyze.py
+-rw-rw-r--   0 rauf      (1000) rauf      (1000)    18148 2023-04-16 12:26:58.000000 lsaBGC-1.34/workflows/lsaBGC-AutoExpansion.py
+-rw-rw-r--   0 rauf      (1000) rauf      (1000)    43849 2023-04-16 13:09:44.000000 lsaBGC-1.34/workflows/lsaBGC-Easy.py
+-rw-rw-r--   0 rauf      (1000) rauf      (1000)    37686 2023-04-16 13:09:44.000000 lsaBGC-1.34/workflows/lsaBGC-Euk-Easy.py
```

### Comparing `lsaBGC-1.33/LICENSE` & `lsaBGC-1.34/LICENSE`

 * *Files identical despite different names*

### Comparing `lsaBGC-1.33/bin/lsaBGC-Cluster.py` & `lsaBGC-1.34/bin/lsaBGC-Cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,26 +46,27 @@
 	""" Parse arguments """
 	parser = argparse.ArgumentParser(description="""
 	Program: lsaBGC-Cluster.py
 	Author: Rauf Salamzade
 	Affiliation: Kalan Lab, UW Madison, Department of Medical Microbiology and Immunology
 
 	This program will cluster BGC Genbanks using MCL based on similarity exhibited in ortholog group presence/
-	absence data. Clustering uses MCL.""", formatter_class=argparse.RawTextHelpFormatter)
+	absence data. Clustering uses MCL.
+	""", formatter_class=argparse.RawTextHelpFormatter)
 
-	parser.add_argument('-b', '--bgc_listings', help='BGC listing file. Tab delimited 2-column file: (1) sample name (2) path to predicted BGC in Genbank format.', required=True)
+	parser.add_argument('-b', '--bgc_listings', help='BGC listing file. Tab delimited 2-column file: (1) sample name (2) path\nto predicted BGC in Genbank format.', required=True)
 	parser.add_argument('-m', '--orthofinder_matrix', help="OrthoFinder matrix.", required=True)
 	parser.add_argument('-o', '--output_directory', help="Output directory.", required=True)
-	parser.add_argument('-p', '--bgc_prediction_software', help='Software used to predict BGCs (Options: antiSMASH, DeepBGC, GECCO).\nDefault is antiSMASH.', default='antiSMASH', required=False)
-	parser.add_argument('-c', '--cpus', type=int, help="Number of cpus to use for MCL step.", required=False, default=1)
-	parser.add_argument('-i', '--mcl_inflation', type=float, help="Inflation parameter to be used for MCL.", required=False, default=1.4)
-	parser.add_argument('-j', '--jaccard_cutoff', type=float, help="Cutoff for Jaccard similarity of homolog groups shared between two BGCs.", required=False, default=50.0)
-	parser.add_argument('-r', '--syntenic_correlation_cutoff', type=float, help="Minimum absolute correlation coefficient between two BGCs.", required=False, default=0.0)
+	parser.add_argument('-p', '--bgc_prediction_software', help='Software used to predict BGCs (Options: antiSMASH, DeepBGC,\nGECCO)\n[Default is antiSMASH].', default='antiSMASH', required=False)
+	parser.add_argument('-i', '--mcl_inflation', type=float, help="Inflation parameter to be used for MCL [Default is 1.4].", required=False, default=1.4)
+	parser.add_argument('-j', '--jaccard_cutoff', type=float, help="Cutoff for Jaccard similarity of homolog groups shared between two BGCs [Default is 50.0].", required=False, default=50.0)
+	parser.add_argument('-r', '--syntenic_correlation_cutoff', type=float, help="Minimum absolute correlation coefficient between two BGCs [Default is 0.0].", required=False, default=0.0)
 	parser.add_argument('-s', '--split_by_annotation', action='store_true', help="Partition BGCs into groups based on annotation first.", required=False, default=False)
 	parser.add_argument('-t', '--run_parameter_tests', action='store_true', help="Run tests for selecting the best inflation parameter and jaccard for MCL analysis and exit.", required=False, default=False)
+	parser.add_argument('-c', '--cpus', type=int, help="Number of cpus to use for MCL step.", required=False, default=1)
 	args = parser.parse_args()
 	return args
 
 def lsaBGC_Cluster():
 	"""
 	Void function which runs primary workflow for program.
 	"""
@@ -120,15 +121,15 @@
 	logObject.info('Running lsaBGC version %s' % version_string)
 
 	# Step 0: Log input arguments and update reference and query FASTA files.
 	logObject.info("Saving parameters for future records.")
 	parameters_file = outdir + 'Parameter_Inputs.txt'
 	parameter_values = [bgc_listings_file, orthofinder_matrix_file, outdir, bgc_prediction_software, cpus, mcl_inflation,
 						jaccard_cutoff, syntenic_correlation_cutoff, run_parameter_tests, split_by_annotation]
-	parameter_names = ["BGC Listing File", "OrthoFinder Orthogroups.csv File", "Output Directory",
+	parameter_names = ["BGC Listing File", "OrthoFinder Orthogroups.tsv File", "Output Directory",
 					   "BGC Prediction Method", "cpus", "MCL Inflation Parameter", "Jaccard Similarity Cutoff",
 					   "Syntenic Correlation Coefficient Cutoff", "Run Inflation Parameter Tests?",
 					   "Split BGCs into Annotation Categories First Prior to Clustering?"]
 	util.logParametersToFile(parameters_file, parameter_names, parameter_values)
 	logObject.info("Done saving parameters!")
 
 	# Create Pan object
```

### Comparing `lsaBGC-1.33/bin/lsaBGC-DiscoVary.py` & `lsaBGC-1.34/bin/lsaBGC-DiscoVary.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,24 +54,24 @@
 	it will map raw paired-end Illumina sequencing data to each non-redundant instance of a homolog group and 
 	report: (i) support for different alleles of homolog groups being present in the reads and (ii) identify any
 	novel SNVs.	
 	""", formatter_class=argparse.RawTextHelpFormatter)
 
     parser.add_argument('-g', '--gcf_listing', help='BGC specifications file. Tab delimited: 1st column contains path to BGC Genbanks and 2nd column contains sample name.', required=True)
     parser.add_argument('-s', '--sequencing_readsets_listing', help="Sequencing data specifications file. Tab delimited: 1st column contains metagenomic sample name, whereas 2nd, 3rd, and so on columns contain full paths to sequencing reads.", required=True)
-    parser.add_argument('-i', '--gcf_id', help="GCF identifier.", required=False, default='GCF_X')
     parser.add_argument('-l', '--input_listing', type=str, help="Tab delimited text file for samples with three columns: (1) sample name\n(2) path to whole-genome generated Genbank file (*.gbk), and (3)path to whole-genome generated\npredicted-proteome file (*.faa).", required=True)
     parser.add_argument('-m', '--orthofinder_matrix', help="OrthoFinder matrix.", required=True)
     parser.add_argument('-o', '--output_directory', help="Prefix for output files.", required=True)
+    parser.add_argument('-i', '--gcf_id', help="GCF identifier [Default is GCF_X].", required=False, default='GCF_X')
     parser.add_argument('-a', '--codon_alignments', help="File listing the codon alignments for each homolog group in the GCF.\nCan be found as part of PopGene output.", required=True)
     parser.add_argument('-p', '--bgc_prediction_software', help='Software used to predict BGCs (Options: antiSMASH, DeepBGC, GECCO).\nDefault is antiSMASH.', default='antiSMASH', required=False)
     parser.add_argument('-awl', '--ambiguity_window_length', help='Length around beginning, end and ambiguous sites in codon alignments to avoid calling SNVs on due to more challenging alignment for reads. Default is 50.', required=False, default=50)
     parser.add_argument('-ch', '--core_homologs', nargs="+", help="List of homolog group identifiers comprising the core of the BGC/GCF.", required=False, default=[])
     parser.add_argument('-ap', '--allow_phasing', action='store_true', help="Allow phasing with DESMAN. Requires manual installation of\nDESMAN (not through conda) and $PATH to be updated.", required=False, default=False)
-    parser.add_argument('-c', '--cpus', type=int, help="The number of cpus to use.", required=False, default=1)
+    parser.add_argument('-c', '--cpus', type=int, help="The number of CPUs to use [Default ", required=False, default=1)
 
     args = parser.parse_args()
 
     return args
 
 def lsaBGC_DiscoVary():
     """
```

### Comparing `lsaBGC-1.33/bin/lsaBGC-Divergence.py` & `lsaBGC-1.34/bin/lsaBGC-Divergence.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,38 +38,38 @@
 import os
 import sys
 import traceback
 from time import sleep
 import argparse
 from collections import defaultdict
 from lsaBGC import util
-from lsaBGC.classes.GCF import GCF
-from lsaBGC.classes.Pan import Pan
+import warnings
+warnings.filterwarnings('ignore')
 
 def create_parser():
     """ Parse arguments """
     parser = argparse.ArgumentParser(description="""
 	Program: lsaBGC-Divergence.py
 	Author: Rauf Salamzade
 	Affiliation: Kalan Lab, UW Madison, Department of Medical Microbiology and Immunology
 
 	This program will calculate Beta-RD, the ratio of the estimated amino acid distances between orthologous BGCs from 
 	two samples to the expected differences based on core protein alignments performed by requesting GToTree analysis in 
 	lsaBGC-Ready, for all pairs of samples featuring a BGC belonging to a focal GCF of interest.
 	""", formatter_class=argparse.RawTextHelpFormatter)
 
-    parser.add_argument('-g', '--gcf_listing', help='BGC specifications file. Tab delimited: 1st column contains path to BGC Genbank and 2nd column contains sample name.', required=True)
-    parser.add_argument('-l', '--input_listing', help="Path to tab delimited file listing: (1) sample name (2) path to Prokka Genbank and (3) path to Prokka predicted proteome. This file is produced by lsaBGC-Process.py.", required=True)
-    parser.add_argument('-a', '--codon_alignments', help="File listing the codon alignments for each homolog group in the GCF. Can be found as part of PopGene output.", required=True)
+    parser.add_argument('-g', '--gcf_listing', help='BGC specifications file. Tab delimited: 1st column contains\npath to BGC GenBank and 2nd column contains sample name.', required=True)
+    parser.add_argument('-l', '--input_listing', help="Path to tab delimited file listing: (1) sample name (2) path to Prokka\nGenBank and (3) path to Prokka predicted proteome. This file is\nproduced by lsaBGC-Process.py.", required=True)
+    parser.add_argument('-a', '--codon_alignments', help="File listing the codon alignments for each homolog group in the GCF.\nCan be found as part of PopGene output.", required=True)
     parser.add_argument('-w', '--expected_similarities', help="Path to file listing expected similarities between genomes/samples. This is\ncomputed most easily by running lsaBGC-Ready.py with '-t' specified, which will estimate\nsample to sample similarities based on alignment used to create species phylogeny.", required=True)
-    parser.add_argument('-i', '--gcf_id', help="GCF identifier.", required=False, default='GCF_X')
+    parser.add_argument('-i', '--gcf_id', help="GCF identifier [Default is GCF_X].", required=False, default='GCF_X')
     parser.add_argument('-o', '--output_directory', help="Prefix for output files.", required=True)
-    parser.add_argument('-k', '--sample_set', help="Sample set to keep in analysis. Should be file with one sample id per line.", required=False)
-    parser.add_argument('-n', '--use_codon', help="Expected sample to sample similarities are reflective of DNA distances instead of protein distances (e.g. if FastANI or MASH were used in computeGenomeWideDistances.py).", required=False, default=False)
-    parser.add_argument('-c', '--cpus', type=int, help="The number of cpus to use.", required=False, default=1)
+    parser.add_argument('-k', '--sample_set', help="Sample set to keep in analysis. Should be file with\none sample id per line.", required=False)
+    parser.add_argument('-n', '--use_codon', help="Expected sample to sample similarities are reflective of\nDNA distances instead of protein distances (e.g. if FastANI or\nMASH were used in computeGenomeWideDistances.py).", required=False, default=False)
+    parser.add_argument('-c', '--cpus', type=int, help="The number of CPUs to use [Default is 1].", required=False, default=1)
     args = parser.parse_args()
 
     return args
 
 def lsaBGC_Divergence():
     """
     Void function which runs primary workflow for program.
```

### Comparing `lsaBGC-1.33/bin/lsaBGC-Expansion.py` & `lsaBGC-1.34/bin/lsaBGC-Expansion.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,28 +60,28 @@
 	""", formatter_class=argparse.RawTextHelpFormatter)
 
     parser.add_argument('-g', '--gcf_listing', help='BGC listings file for a gcf. Tab delimited: 1st column lists sample\nname while the 2nd column is the path to a BGC prediction in Genbank format.', required=True)
     parser.add_argument('-m', '--orthofinder_matrix', help="OrthoFinder matrix.", required=True)
     parser.add_argument('-l', '--initial_listing', type=str, help="Tab delimited text file for primary samples with three columns: (1) sample name\n(2) path to whole-genome generated Genbank file (*.gbk), and (3)path to whole-genome generated\npredicted-proteome file (*.faa).", required=True)
     parser.add_argument('-e', '--expansion_listing', type=str, help="Tab delimited text file for additional/draft samples in the expansion set with three columns: (1) sample name\n(2)path to whole-genome Genbank file (*.gbk), and (3)path to whole-genome\npredicted-proteome file (*.faa).", required=True)
     parser.add_argument('-o', '--output_directory', help="Path to output directory.", required=True)
-    parser.add_argument('-i', '--gcf_id', help="GCF identifier.", required=False, default='GCF_X')
-    parser.add_argument('-p', '--bgc_prediction_software', help='Software used to predict BGCs (Options: antiSMASH, DeepBGC, GECCO).\nDefault is antiSMASH.', default='antiSMASH', required=False)
-    parser.add_argument('-ms', '--min_segment_size', type=float, help="The minimum number of homolog groups (>3) needed to report discrete segments of the GCF. Ignored if GCF specific or functionally core (e.g. harboring key domain for detection of BGC) homolog group is found in segment. Default is 5.", required=False, default=5)
-    parser.add_argument('-mcs', '--min_segment_core_size', type=float, help="The minimum number of core (to the known instances of the GCF) homololog groups needed\nto report discrete segments of the GCF. Default is 3.", required=False, default=3)
-    parser.add_argument('-sct', '--syntenic_correlation_threshold', type=float, help="The minimum syntenic correlation needed to at least one known\nGCF instance to report segment.", required=False, default=0.8)
-    parser.add_argument('-tg', '--transition_from_gcf_to_gcf', type=float, help="GCF to GCF state transition probability for HMM. Should be between\n0.0 and 1.0. Default is 0.9.", required=False, default=0.9)
-    parser.add_argument('-tb', '--transition_from_bg_to_bg', type=float, help="Background to background state transition probability for HMM. Should be\nbetween 0.0 and 1.0. Default is 0.9.", required=False, default=0.9)
-    parser.add_argument('-c', '--cpus', type=int, help="The number of cpus to use.", required=False, default=1)
-    parser.add_argument('-q', '--quick_mode', action='store_true', help="Run in quick-mode. Instead of running HMMScan for each homolog group, a consensus\nsequence is emitted and Diamond is used for searching instead. Method inspired by Melnyk et al. 2019", required=False, default=False)
+    parser.add_argument('-i', '--gcf_id', help="GCF identifier [Default is GCF_X].", required=False, default='GCF_X')
+    parser.add_argument('-p', '--bgc_prediction_software', help='Software used to predict BGCs (Options: antiSMASH, DeepBGC, GECCO).\n[Default is antiSMASH].', default='antiSMASH', required=False)
+    parser.add_argument('-ms', '--min_segment_size', type=float, help="The minimum number of homolog groups (>3) needed to report discrete\nsegments of the GCF. Ignored if GCF specific or functionally core (e.g. harboring key domain for\ndetection of BGC) homolog group is found in segment [Default is 5].", required=False, default=5)
+    parser.add_argument('-mcs', '--min_segment_core_size', type=float, help="The minimum number of core (to the known instances of the GCF) homololog groups needed\nto report discrete segments of the GCF [Default is 3].", required=False, default=3)
+    parser.add_argument('-sct', '--syntenic_correlation_threshold', type=float, help="The minimum syntenic correlation needed to at least one known\nGCF instance to report segment [Default is 0.8].", required=False, default=0.8)
+    parser.add_argument('-tg', '--transition_from_gcf_to_gcf', type=float, help="GCF to GCF state transition probability for HMM. Should be between\n0.0 and 1.0 [Default is 0.9].", required=False, default=0.9)
+    parser.add_argument('-tb', '--transition_from_bg_to_bg', type=float, help="Background to background state transition probability for HMM. Should be\nbetween 0.0 and 1.0 [Default is 0.9].", required=False, default=0.9)
+    parser.add_argument('-q', '--quick_mode', action='store_true', help="Run in quick-mode. Instead of running HMMScan for each homolog group, a consensus\nsequence is emitted and Diamond is used for searching instead.", required=False, default=False)
     parser.add_argument('-no', '--no_orthogroup_matrix', action='store_true', help="Avoid writing the updated OrthoFinder matrix at the end.", required=False, default=False)
-    parser.add_argument('-w', '--loose', action='store_true', help="Remove requirement for proto-core/rule-based homolog group being detected in a single\nneighborhood for GCF to be reported as present.", required=False, default=False)
+    parser.add_argument('-w', '--loose', action='store_true', help="Remove requirement for proto-core/rule-based homolog group being detected in\na single neighborhood for GCF to be reported as present.", required=False, default=False)
     parser.add_argument('-ph', '--protocore_homologs', nargs="+", help="List of homolog group identifiers comprising the core of the BGC/GCF of which at\nleast one is required for GCF to be reported. Please provide as space-seperated list\nwith quotes surrounding: \"OG1 OG2 ...\"", required=False, default=[])
-    parser.add_argument('-ap', '--all_primary', action='store_true', help='Treat all known GCF instances as primary (use if BGC Genbanks were not processed through lsaBGC-Ready).', required=False, default=False)
-    parser.add_argument('-z', '--pickle_expansion_annotation_data', help="Pickle file with serialization of annotation data in the expansion listing file.", required=False, default=None)
+    parser.add_argument('-ap', '--all_primary', action='store_true', help='Treat all known GCF instances as primary (use if BGC Genbanks\nwere not processed through lsaBGC-Ready).', required=False, default=False)
+    parser.add_argument('-z', '--pickle_expansion_annotation_data', help="Pickle file with serialization of annotation data in the expansion\nlisting file.", required=False, default=None)
+    parser.add_argument('-c', '--cpus', type=int, help="The number of CPUs to use [Default is 1].", required=False, default=1)
 
     args = parser.parse_args()
 
     return args
 
 def lsaBGC_Expansion():
     """
```

### Comparing `lsaBGC-1.33/bin/lsaBGC-PopGene.py` & `lsaBGC-1.34/bin/lsaBGC-PopGene.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,39 +38,40 @@
 import os
 import sys
 from time import sleep
 import argparse
 from collections import defaultdict
 from lsaBGC import util
 from lsaBGC.classes.GCF import GCF
+import warnings
+warnings.filterwarnings('ignore')
 
 def create_parser():
     """ Parse arguments """
     parser = argparse.ArgumentParser(description="""
 	Program: lsaBGC-PopGene.py
 	Author: Rauf Salamzade
 	Affiliation: Kalan Lab, UW Madison, Department of Medical Microbiology and Immunology
 
 	This program investigates conservation and population genetic related statistics for each homolog group 
 	observed in BGCs belonging to a single GCF.
 	""", formatter_class=argparse.RawTextHelpFormatter)
 
-    parser.add_argument('-g', '--gcf_listing', help='BGC listings file for a gcf. Tab delimited: 1st column lists sample name while the 2nd column is the path to a BGC prediction in Genbank format.', required=True)
-    parser.add_argument('-m', '--orthofinder_matrix', help="OrthoFinder matrix.", required=True)
-    parser.add_argument('-i', '--gcf_id', help="GCF identifier.", required=False, default='GCF_X')
+    parser.add_argument('-g', '--gcf_listing', help='BGC listings file for a gcf. Tab delimited: 1st column lists sample name\nwhile the 2nd column is the path to a BGC prediction in Genbank format.', required=True)
+    parser.add_argument('-m', '--orthofinder_matrix', help="OrthoFinder homolog by sample matrix.", required=True)
+    parser.add_argument('-i', '--gcf_id', help="GCF identifier [Default is GCF_X].", required=False, default='GCF_X')
     parser.add_argument('-o', '--output_directory', help="Path to output directory.", required=True)
-    parser.add_argument('-k', '--sample_set', help="Sample set to keep in analysis. Should be file with one sample id per line.", required=False)
-    parser.add_argument('-s', '--species_phylogeny', help="The species phylogeny in Newick format. Specifies that dN/dS should be calculated by comparing extant homolog-group sequences to ancestral state reconstruction. Does not currently work!!!", required=False, default=None)
-    parser.add_argument('-u', '--population_classification', help='Popualation classifications for each sample. Tab delemited: 1st column lists sample name while the 2nd column is an identifier for the population the sample belongs to.', required=False, default=None)
-    parser.add_argument('-p', '--bgc_prediction_software', help='Software used to predict BGCs (Options: antiSMASH, DeepBGC, GECCO).\nDefault is antiSMASH.', default='antiSMASH', required=False)
-    parser.add_argument('-c', '--cpus', type=int, help="The number of cpus to use.", required=False, default=1)
-    parser.add_argument('-d', '--regular_mafft', action='store_true', help="Run mafft --linsi and not the MAGUS divide-and-conquer approach which allows for scalability and more efficient computing.", default=False, required=False)
+    parser.add_argument('-k', '--sample_set', help="Sample set to keep in analysis. Should be file with one\nsample id per line.", required=False)
+    parser.add_argument('-u', '--population_classification', help='Popualation classifications for each sample. Tab delemited: 1st column lists sample\nname while the 2nd column is an identifier for the population the sample\nbelongs to.', required=False, default=None)
+    parser.add_argument('-p', '--bgc_prediction_software', help='Software used to predict BGCs (Options: antiSMASH, DeepBGC, GECCO)\n[Default is antiSMASH].', default='antiSMASH', required=False)
+    parser.add_argument('-d', '--regular_mafft', action='store_true', help="Run mafft --linsi and not the MAGUS divide-and-conquer approach which\nallows for scalability and more efficient computing.", default=False, required=False)
     parser.add_argument('-e', '--each_pop', action='store_true', help='Run analyses individually for each population as well.', required=False, default=False)
-    parser.add_argument('-t', '--filter_for_outliers', action='store_true', help='Filter instances of homolog groups which deviate too much from the median gene length observed for the initial set of proteins.', required=False, default=False)
-    parser.add_argument('-w', '--expected_similarities', help="Path to file listing expected similarities between genomes/samples. This is\ncomputed most easily by running lsaBGC-Ready.py with '-t' specified, which will estimate\nsample to sample similarities based on alignment used to create species phylogeny.", required=False, default=None)
+    parser.add_argument('-t', '--filter_for_outliers', action='store_true', help='Filter instances of homolog groups which deviate too much from\nthe median gene length observed for the initial set of proteins.', required=False, default=False)
+    parser.add_argument('-w', '--expected_similarities', help="Path to file listing expected similarities between genomes/samples. This is\ncomputed most easily by running lsaBGC-Ready.py with '-t' specified,\nwhich will estimate\nsample to sample similarities based on alignment used to create\nspecies phylogeny.", required=False, default=None)
+    parser.add_argument('-c', '--cpus', type=int, help="The number of CPUs to use [Default is 1].", required=False, default=1)
     args = parser.parse_args()
 
     return args
 
 def lsaBGC_PopGene():
     """
     Void function which runs primary workflow for program.
@@ -98,15 +99,15 @@
     else:
         os.system('mkdir %s' % outdir)
 
     """
     PARSE OPTIONAL INPUTS
     """
 
-    species_phylogeny = myargs.species_phylogeny
+    #species_phylogeny = myargs.species_phylogeny
     sample_set_file = myargs.sample_set
     gcf_id = myargs.gcf_id
     bgc_prediction_software = myargs.bgc_prediction_software.upper()
     cpus = myargs.cpus
     population_classification_file = myargs.population_classification
     run_for_each_pop = myargs.each_pop
     filter_for_outliers = myargs.filter_for_outliers
@@ -127,20 +128,20 @@
     version_string = util.parseVersionFromSetupPy()
     logObject.info('Running lsaBGC version %s' % version_string)
 
     # Log input arguments and update reference and query FASTA files.
     logObject.info("Saving parameters for future records.")
     parameters_file = outdir + 'Parameter_Inputs.txt'
     parameter_values = [gcf_listing_file, orthofinder_matrix_file, outdir, gcf_id, bgc_prediction_software,
-                        population_classification_file, sample_set_file, species_phylogeny, run_for_each_pop,
+                        population_classification_file, sample_set_file, run_for_each_pop,
                         filter_for_outliers, expected_distances, regular_mafft, cpus]
     parameter_names = ["GCF Listing File", "OrthoFinder Orthogroups.csv File", "Output Directory", "GCF Identifier",
                        "BGC Prediction Software", "Populations Specification/Listing File", "Sample Retention Set",
-                       "Species Phylogeny Newick File", "Run Analysis for Each Population",
-                       "Filter for Outlier Homolog Group Instances", "File with Expected Amino Acid Differences Between Genomes/Samples",
+                       "Run Analysis for Each Population", "Filter for Outlier Homolog Group Instances",
+                       "File with Expected Amino Acid Differences Between Genomes/Samples",
                        "AAI Similarity Instead of ANI", "Use Regular MAFFT - not MAGUS?", "cpus"]
     util.logParametersToFile(parameters_file, parameter_names, parameter_values)
     logObject.info("Done saving parameters!")
 
     # Create GCF object
     GCF_Object = GCF(gcf_listing_file, gcf_id=gcf_id, logObject=logObject)
 
@@ -198,21 +199,21 @@
     populations = [None]
     population_analysis_on = False
     if population_classification_file:
         populations = populations + list(sorted(set(GCF_Object.sample_population.values())))
         population_analysis_on = True
     if run_for_each_pop:
         for pop in populations:
-            GCF_Object.runPopulationGeneticsAnalysis(outdir, cpus=cpus, population=pop, filter_outliers=False, population_analysis_on=population_analysis_on, gw_pairwise_similarities=gw_pairwise_similarities, use_translation=True, species_phylogeny=species_phylogeny)
+            GCF_Object.runPopulationGeneticsAnalysis(outdir, cpus=cpus, population=pop, filter_outliers=False, population_analysis_on=population_analysis_on, gw_pairwise_similarities=gw_pairwise_similarities, use_translation=True)
             if filter_for_outliers:
-                GCF_Object.runPopulationGeneticsAnalysis(outdir, cpus=cpus, population=pop, filter_outliers=True, population_analysis_on=population_analysis_on, gw_pairwise_similarities=gw_pairwise_similarities, use_translation=True, species_phylogeny=species_phylogeny)
+                GCF_Object.runPopulationGeneticsAnalysis(outdir, cpus=cpus, population=pop, filter_outliers=True, population_analysis_on=population_analysis_on, gw_pairwise_similarities=gw_pairwise_similarities, use_translation=True)
     else:
-        GCF_Object.runPopulationGeneticsAnalysis(outdir, cpus=cpus, population=None, filter_outliers=False, population_analysis_on=population_analysis_on, gw_pairwise_similarities=gw_pairwise_similarities, use_translation=True, species_phylogeny=species_phylogeny)
+        GCF_Object.runPopulationGeneticsAnalysis(outdir, cpus=cpus, population=None, filter_outliers=False, population_analysis_on=population_analysis_on, gw_pairwise_similarities=gw_pairwise_similarities, use_translation=True)
         if filter_for_outliers:
-            GCF_Object.runPopulationGeneticsAnalysis(outdir, cpus=cpus, population=None, filter_outliers=True, population_analysis_on=population_analysis_on, gw_pairwise_similarities=gw_pairwise_similarities, use_translation=True, species_phylogeny=species_phylogeny)
+            GCF_Object.runPopulationGeneticsAnalysis(outdir, cpus=cpus, population=None, filter_outliers=True, population_analysis_on=population_analysis_on, gw_pairwise_similarities=gw_pairwise_similarities, use_translation=True)
     logObject.info("Successfully ran population genetics and evolutionary analyses of each codon alignment.")
 
     # Write checkpoint file for lsaBGC-AutoAnalyze.py
     checkpoint_file = outdir + 'CHECKPOINT.txt'
     checkpoint_handle = open(checkpoint_file, 'w')
     checkpoint_handle.write('lsaBGC-PopGene completed successfully!')
     checkpoint_handle.close()
```

### Comparing `lsaBGC-1.33/bin/lsaBGC-Ready.py` & `lsaBGC-1.34/bin/lsaBGC-Ready.py`

 * *Files 6% similar despite different names*

```diff
@@ -92,40 +92,35 @@
          please consider using lsaBGC-Cluster.py, we use similar methods to BiG-SCAPE, though the algorithms are 
          mostly designed for complete BGCs in mind for lsaBGC-Cluster.py, while BiG-SCAPE has some nice settings 
          to handle fragmented BGCs. lsaBGC-Expansion/AutoExpansion are specifically designed for detecting fragmented
          GCF instances in draft assemblies and can be run on the initial "primary" genome set as well.
 	***************************************************************************************************************** 
 	""", formatter_class=argparse.RawTextHelpFormatter)
 
-    parser.add_argument('-i', '--genome_listing',
-                        help='Tab-delimited, two column file for primary samples (ideally with high-quality or complete genomes)\nwhere the first column is the sample/isolate/genome name and the second is the\nfull path to the genome file (Genbank or FASTA).\nCheck note above about available scripts to automatically create this.',
-                        required=True)
-    parser.add_argument('-d', '--additional_genome_listing', help='Tab-delimited, two column file for samples with additional/draft\ngenomes (same format as for the "--genome_listing" argument). The genomes/BGCs of these\nsamples won\'t be used in ortholog-grouping of proteins and clustering of BGCs, but will simply have gene\ncalling run for them. This will enable more sensitive/expanded detection of GCF instances later\nusing lsaBGC-Expansion/AutoExpansion.\nCheck note above about available scripts to automatically create this.',
-                        required=False, default=None)
-    parser.add_argument('-l', '--bgc_genbank_listing',
-                        help='Tab-delimited, two column file listing BGC predictions results for primary samples\n(those from the "--genome_listing" argument), where the first column is the sample name and the second\nis the full path to BGC prediction in Genbank format.',
-                        required=True)
-    parser.add_argument('-p', '--bgc_prediction_software', help='Software used to predict BGCs (Options: antiSMASH, DeepBGC, GECCO).\nDefault is antiSMASH.', default='antiSMASH', required=False)
-    parser.add_argument('-b', '--bigscape_results', help='Path to BiG-SCAPE results directory of antiSMASH/DeepBGC/GECCO results predicted in primary\ngenomes.Please make sure the sample names match what is provided for "--genome_listings".', required=False,
-                        default=None)
+    parser.add_argument('-i', '--genome_listing', help='Tab-delimited, two column file for primary samples (ideally with high-quality or complete genomes)\nwhere the first column is the sample/isolate/genome name and the second is the\nfull path to the genome file (Genbank or FASTA).\nCheck note above about available scripts to automatically create this.', required=True)
+    parser.add_argument('-d', '--additional_genome_listing', help='Tab-delimited, two column file for samples with additional/draft\ngenomes (same format as for the "--genome_listing" argument). The genomes/BGCs of these\nsamples won\'t be used in ortholog-grouping of proteins and clustering of BGCs, but will simply have gene\ncalling run for them. This will enable more sensitive/expanded detection of GCF instances later\nusing lsaBGC-Expansion/AutoExpansion.\nCheck note above about available scripts to automatically create this.', required=False, default=None)
+    parser.add_argument('-l', '--bgc_genbank_listing', help='Tab-delimited, two column file listing BGC predictions results for primary samples\n(those from the "--genome_listing" argument), where the first column is the sample name and the second\nis the full path to BGC prediction in Genbank format.', required=True)
+    parser.add_argument('-p', '--bgc_prediction_software', help='Software used to predict BGCs (Options: antiSMASH, DeepBGC, GECCO).\n[Default is antiSMASH].', default='antiSMASH', required=False)
+    parser.add_argument('-b', '--bigscape_results', help='Path to BiG-SCAPE results directory of antiSMASH/DeepBGC/GECCO results predicted\nin primary genomes. Please make sure the sample names match what is provided for "--genome_listings".', required=False, default=None)
     parser.add_argument('-o', '--output_directory', help='Parent output/workspace directory.', required=True)
-    parser.add_argument('-m', '--orthofinder_mode', help='Method for running OrthoFinder2. (Options: Genome_Wide, BGC_Only). Default is Genome_Wide.', required=False, default='Genome_Wide')
-    parser.add_argument('-mc', '--run_coarse_orthofinder', action='store_true', help='Use coarse clustering of homolog groups in OrthoFinder instead of more resolute hierarchical determined homolog groups.', required=False, default=False)
-    parser.add_argument('-a', '--annotate', action='store_true',
-                        help='Perform annotation of BGC proteins using KOfam and PGAP (including TIGR) HMM profiles.', required=False, default=False)
+    parser.add_argument('-m', '--orthofinder_mode', help='Method for running OrthoFinder2. (Options: Genome_Wide,\nBGC_Only) [Default is Genome_Wide].', required=False, default='Genome_Wide')
+    parser.add_argument('-mc', '--run_coarse_orthofinder', action='store_true', help='Use coarse clustering of homolog groups in OrthoFinder instead of more\nresolute hierarchical determined homolog groups.', required=False, default=False)
+    parser.add_argument('-a', '--annotate', action='store_true', help='Perform annotation of BGC proteins using KOfam and PGAP (including TIGR)\nHMM profiles.', required=False, default=False)
     parser.add_argument('-t', '--run_gtotree', action='store_true', help='Whether to create phylogeny and expected sample-vs-sample\ndivergence for downstream analyses using GToTree.', required=False, default=False)
-    parser.add_argument('-gtm', '--gtotree_model', help='Set of core genes to use for phylogeny construction in GToTree. Default is Universal_Hug_et_al', required=False, default="Universal_Hug_et_al")
-    parser.add_argument('-lc', '--lsabgc_cluster', action='store_true', help='Run lsaBGC-Cluster with default parameters. Note, we recommend running lsaBGC-Cluster manually\nand exploring parameters through its ability to generate a user-report for setting clustering parameters.', required=False, default=False)
+    parser.add_argument('-gtm', '--gtotree_model', help='Set of core genes to use for phylogeny construction in GToTree\n[Default is Universal_Hug_et_al].', required=False, default="Universal_Hug_et_al")
+    parser.add_argument('-lc', '--lsabgc_cluster', action='store_true', help='Run lsaBGC-Cluster with default parameters. Note, we recommend running lsaBGC-Cluster\nmanually and exploring parameters through its ability to generate a user-report for setting\nclustering parameters.', required=False, default=False)
+    parser.add_argument('-lci', '--lsabgc_cluster_inflation', type=float, help='Value for MCL inflation parameter to use in lsaBGC-Cluster [Default is 4.0].', required=False, default=4.0)
+    parser.add_argument('-lcj', '--lsabgc_cluster_jaccard', type=float, help='Minimal Jaccard Index cutoff to regard two BGCs as potentially homologous\nin lsaBGC-Cluster [Default is 20.0].', required=False, default=20.0)
+    parser.add_argument('-lcr', '--lsabgc_cluster_synteny', type=float, help='Minimal absolute correlation coefficient to measure syntenic similarity and\nregard two BGCs as potentially homologous in lsaBGC-Cluster [Default is 0.7].', required=False, default=0.7)
     parser.add_argument('-le', '--lsabgc_expansion', action='store_true', help='Run lsaBGC-AutoExpansion with default parameters. Assumes either "--bigscape_results" or\n"--lsabgc_cluster" is specified.', default=False, required=False)
-    parser.add_argument('-c', '--cpus', type=int,
-                        help="Total number of cpus/threads to use for running OrthoFinder2/prodigal.", required=False,
-                        default=1)
-    parser.add_argument('-k', '--keep_intermediates', action='store_true', help='Keep intermediate directories / files which are likely not useful for downstream analyses.', required=False, default=False)
+    parser.add_argument('-k', '--keep_intermediates', action='store_true', help='Keep intermediate directories / files which are likely not\nuseful for downstream analyses.', required=False, default=False)
     parser.add_argument('-spe', '--skip_primary_expansion', action='store_true', help='Skip expansion on primary genomes as well.', required=False, default=False)
     parser.add_argument('-py', '--use_pyrodigal', action='store_true', help='Use pyrodigal instead of prodigal.', required=False, default=False)
+    parser.add_argument('-c', '--cpus', type=int, help="Total number of CPUs to use [Default is 1].", required=False, default=1)
+
     args = parser.parse_args()
     return args
 
 def lsaBGC_Ready():
     """
 	Void function which runs primary workflow for program.
 	"""
@@ -173,14 +168,17 @@
     annotate = myargs.annotate
     run_lsabgc_cluster = myargs.lsabgc_cluster
     run_lsabgc_expansion = myargs.lsabgc_expansion
     run_coarse_orthofinder = myargs.run_coarse_orthofinder
     keep_intermediates = myargs.keep_intermediates
     skip_primary_expansion = myargs.skip_primary_expansion
     use_pyrodigal = myargs.use_pyrodigal
+    lsabgc_cluster_inflation = myargs.lsabgc_cluster_inflation
+    lsabgc_cluster_jaccard = myargs.lsabgc_cluster_jaccard
+    lsabgc_cluster_synteny = myargs.lsabgc_cluster_synteny
 
     try:
         assert(orthofinder_mode in set(['GENOME_WIDE', 'BGC_ONLY']))
     except:
         raise RuntimeError('BGC prediction software option is not a valid option.')
 
     try:
@@ -241,20 +239,23 @@
     version_string = util.parseVersionFromSetupPy()
     logObject.info('Running lsaBGC version %s' % version_string)
 
     logObject.info("Saving parameters for future records.")
     parameters_file = outdir + 'Parameter_Inputs.txt'
     parameter_values = [genome_listing_file, bgc_genbank_listing_file, outdir, additional_genome_listing_file,
                         bgc_prediction_software, orthofinder_mode, bigscape_results_dir, annotate, run_lsabgc_cluster,
-                        run_lsabgc_expansion, keep_intermediates, use_pyrodigal, cpus]
+                        lsabgc_cluster_inflation, lsabgc_cluster_jaccard, lsabgc_cluster_synteny, run_lsabgc_expansion,
+                        keep_intermediates, use_pyrodigal, cpus]
     parameter_names = ["Primary Genome Listing File", "BGC Predictions Genbanks Listing File", "Output Directory",
                        "Additional Genome Listing File", "BGC Prediction Software", "OrthoFinder Mode",
                        "BiG-SCAPE Results Directory", "Perform KOfam/PGAP Annotation?", "Run lsaBGC-Cluster Analysis?",
+                       "Inflation Parameter Value for MCL clustering in lsaBGC-Cluster",
+                       "Jaccard Index Threshold for lsaBGC-Cluster", "Syntenic Similarity Threshold for lsaBGC-Cluster",
                        "Run lsaBGC-AutoExpansion Analysis?", "Keep Intermediate Files/Directories?",
-                       "Use pyrodigal instead of prodigal", "Number of cpus"]
+                       "Use pyrodigal instead of prodigal", "Number of CPUs"]
     util.logParametersToFile(parameters_file, parameter_names, parameter_values)
     logObject.info("Done saving parameters!")
 
     # Step 1: Process Primary Genomes
     sample_genomes, format_prediction = util.parseSampleGenomes(genome_listing_file, logObject)
 
     if format_prediction == 'mixed':
@@ -378,16 +379,16 @@
 
     # Step 5: Perform KOfam/PGAP annotation if requested and update BGCs (including references to them)
     protein_annotations = None
     if annotate:
         annot_directory = outdir + 'Annotations/'
         util.setupReadyDirectory([annot_directory])
         protein_annotations = util.performKOFamAndPGAPAnnotation(sample_bgc_proteins, bgc_prot_directory,
-                                                                       annot_directory, kofam_hmm_file, pgap_hmm_file,
-                                                                       kofam_pro_list, pgap_inf_list, logObject, cpus=cpus)
+                                                                 annot_directory, kofam_hmm_file, pgap_hmm_file,
+                                                                 kofam_pro_list, pgap_inf_list, logObject, cpus=cpus)
         bgcs_directory_updated = outdir + 'BGCs_Retagged_and_Annotated/'
         util.setupReadyDirectory([bgcs_directory_updated])
 
         sample_bgcs_update, bgc_to_sample_update, sample_bgc_proteins_update = util.updateBGCGenbanksToIncludeAnnotations(protein_annotations, bgc_to_sample, sample_bgc_proteins,
                                                                                                     bgcs_directory,
                                                                                                     bgcs_directory_updated,
                                                                                                     logObject)
@@ -476,16 +477,17 @@
         if not os.path.isdir(bigscape_reformat_directory) or not os.path.isdir(gcf_listings_directory):
             util.setupReadyDirectory([bigscape_reformat_directory, gcf_listings_directory])
         util.createGCFListingsDirectory(sample_bgcs, bgc_to_sample, bigscape_results_dir, gcf_listings_directory,
                                         logObject)
     elif run_lsabgc_cluster:
         lsabgc_cluster_results_dir = outdir + 'lsaBGC_Cluster_Results/'
         lsabgc_cluster_cmd = ['lsaBGC-Cluster.py', '-b', primary_bgc_listing_file, '-m', primary_orthofinder_matrix_file,
-                              '-c', str(cpus), '-o', lsabgc_cluster_results_dir, '-r', '0.7', '-i', '4.0', '-j',
-                              '20.0', '-p', bgc_prediction_software]
+                              '-c', str(cpus), '-o', lsabgc_cluster_results_dir, '-r', str(lsabgc_cluster_synteny),
+                              '-i', str(lsabgc_cluster_inflation), '-j', str(lsabgc_cluster_jaccard), '-p',
+                              bgc_prediction_software]
         try:
             subprocess.call(' '.join(lsabgc_cluster_cmd), shell=True, stdout=subprocess.DEVNULL,
                             stderr=subprocess.DEVNULL,
                             executable='/bin/bash')
             assert(os.path.isdir(lsabgc_cluster_results_dir + 'GCF_Listings/'))
             if logObject:
                 logObject.info('Successfully ran: %s' % ' '.join(lsabgc_cluster_cmd))
```

### Comparing `lsaBGC-1.33/bin/lsaBGC-Refiner.py` & `lsaBGC-1.34/bin/lsaBGC-Refiner.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,17 +53,17 @@
 	whittle them down to include only annotations/features in between user specified homolog groups. It is particularly
 	useful for curation of GCFs which featuere distinct BGCs aggregated together due to close physical proximity as 
 	described in: https://msystems.asm.org/content/6/2/e00057-21/article-info 
 	""", formatter_class=argparse.RawTextHelpFormatter)
 
     parser.add_argument('-g', '--gcf_listing', help='BGC listings file for a gcf. Tab delimited: 1st column lists sample name while the 2nd column is the path to a BGC prediction in Genbank format.', required=True)
     parser.add_argument('-m', '--orthofinder_matrix', help="OrthoFinder homolog by sample matrix.", required=True)
-    parser.add_argument('-i', '--gcf_id', help="GCF identifier.", required=False, default='GCF_X')
     parser.add_argument('-o', '--output_directory', help="Output directory.", required=True)
-    parser.add_argument('-p', '--bgc_prediction_software', help='Software used to predict BGCs (Options: antiSMASH, DeepBGC, GECCO).\nDefault is antiSMASH.', default='antiSMASH', required=False)
+    parser.add_argument('-i', '--gcf_id', help="GCF identifier [Default is GCF_X].", required=False, default='GCF_X')
+    parser.add_argument('-p', '--bgc_prediction_software', help='Software used to predict BGCs (Options: antiSMASH, DeepBGC, GECCO).=\n[Default is antiSMASH].', default='antiSMASH', required=False)
     parser.add_argument('-b1', '--first_boundary_homolog', help="Identifier for the first homolog group to be used as boundary for pruning BGCs..", required=True)
     parser.add_argument('-b2', '--second_boundary_homolog', help="Identifier for the second homolog group to be used as boundary for pruning BGCs.", required=True)
     args = parser.parse_args()
     return args
 
 def lsaBGC_Refiner():
     """
```

### Comparing `lsaBGC-1.33/bin/lsaBGC-See.py` & `lsaBGC-1.34/bin/lsaBGC-See.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,42 +37,39 @@
 
 import os
 import sys
 from time import sleep
 import argparse
 from lsaBGC import util
 from lsaBGC.classes.GCF import GCF
+import warnings
+warnings.filterwarnings('ignore')
 
 def create_parser():
     """ Parse arguments """
     parser = argparse.ArgumentParser(description="""
 	Program: lsaBGC-See.py
 	Author: Rauf Salamzade
 	Affiliation: Kalan Lab, UW Madison, Department of Medical Microbiology and Immunology
 
 	This program will create automatic visuals depicting genes across a species or BGC-specific phylogeny as well as
 	iTol tracks visualizing BGCs from a single GCF across a species tree. Alternatively, if a species tree is not 
 	available, it will also create a phylogeny based on single copy core genes of the GCF.
 	""", formatter_class=argparse.RawTextHelpFormatter)
 
-    parser.add_argument('-g', '--gcf_listing',
-                        help='BGC listings file for a gcf. Tab delimited: 1st column lists sample name while the 2nd column is the path to a BGC prediction in Genbank format.', required=True)
+    parser.add_argument('-g', '--gcf_listing', help='BGC listings file for a GCF. Tab delimited:\n1st column lists sample name while the 2nd column\nis the path to a BGC prediction in Genbank format.', required=True)
     parser.add_argument('-m', '--orthofinder_matrix', help="OrthoFinder matrix.", required=True)
     parser.add_argument('-o', '--output_directory', help="Output directory.", required=True)
-    parser.add_argument('-i', '--gcf_id', help="GCF identifier.", required=False, default='GCF_X')
     parser.add_argument('-s', '--species_phylogeny', help="The species phylogeny in Newick format.", required=False, default=None)
-    parser.add_argument('-p', '--bgc_prediction_software', help='Software used to predict BGCs (Options: antiSMASH, DeepBGC, GECCO).\nDefault is antiSMASH.', default='antiSMASH', required=False)
-    parser.add_argument('-c', '--cpus', type=int, help="Number of cpus to use for MCL step.", required=False, default=1)
-    parser.add_argument('-k', '--sample_set',
-                        help="Sample set to keep in analysis. Should be file with one sample id per line.", required=False)
-    parser.add_argument('-y', '--create_gcf_phylogeny', action='store_true',
-                        help="Create phylogeny from sequences of homolog groups in GCF.", required=False, default=False)
-    parser.add_argument('-f', '--only_scc', action='store_true',
-                        help="Use only single-copy-core homolog groups for constructing GCF phylogeny.", required=False,
-                        default=False)
+    parser.add_argument('-i', '--gcf_id', help="GCF identifier [Default is GCF_X].", required=False, default='GCF_X')
+    parser.add_argument('-p', '--bgc_prediction_software', help='Software used to predict BGCs (Options: antiSMASH, DeepBGC, GECCO)\n[Default is antiSMASH].', default='antiSMASH', required=False)
+    parser.add_argument('-k', '--sample_set', help="Sample set to keep in analysis. Should be file with one sample id per line.", required=False)
+    parser.add_argument('-y', '--create_gcf_phylogeny', action='store_true', help="Create phylogeny from sequences of homolog groups in GCF.", required=False, default=False)
+    parser.add_argument('-f', '--only_scc', action='store_true', help="Use only single-copy-core homolog groups for constructing GCF phylogeny.", required=False, default=False)
+    parser.add_argument('-c', '--cpus', type=int, help="Number of CPUs to use for MCL step [Default is 1].", required=False, default=1)
 
 
     args = parser.parse_args()
     return args
 
 def lsaBGC_See():
     """
```

### Comparing `lsaBGC-1.33/lsaBGC/processing.py` & `lsaBGC-1.34/lsaBGC/processing.py`

 * *Files identical despite different names*

### Comparing `lsaBGC-1.33/lsaBGC/util.py` & `lsaBGC-1.34/lsaBGC/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,19 +15,77 @@
 from ete3 import Tree
 import itertools
 import math
 import numpy as np
 import gzip
 import pathlib
 import operator
+import warnings
+warnings.filterwarnings('ignore')
+
 
 valid_alleles = set(['A', 'C', 'G', 'T'])
 curr_dir = os.path.abspath(pathlib.Path(__file__).parent.resolve()) + '/'
 main_dir = '/'.join(curr_dir.split('/')[:-2]) + '/'
 
+def parseCDSCoord(str_gbk_loc):
+	try:
+		start = None
+		end = None
+		direction = None
+		all_coords = []
+		is_multi_part = False
+		if not 'join' in str(str_gbk_loc) and not 'order' in str(str_gbk_loc):
+			start = min([int(x.strip('>').strip('<')) for x in
+						 str(str_gbk_loc)[1:].split(']')[0].split(':')]) + 1
+			end = max([int(x.strip('>').strip('<')) for x in
+					   str(str_gbk_loc)[1:].split(']')[0].split(':')])
+			direction = str(str_gbk_loc).split('(')[1].split(')')[0]
+			all_coords.append([start, end, direction])
+		elif 'order' in str(str_gbk_loc):
+			is_multi_part = True
+			all_starts = []
+			all_ends = []
+			all_directions = []
+			for exon_coord in str(str_gbk_loc)[6:-1].split(', '):
+				ec_start = min(
+					[int(x.strip('>').strip('<')) for x in exon_coord[1:].split(']')[0].split(':')]) + 1
+				ec_end = max(
+					[int(x.strip('>').strip('<')) for x in exon_coord[1:].split(']')[0].split(':')])
+				ec_direction = exon_coord.split('(')[1].split(')')[0]
+				all_starts.append(ec_start)
+				all_ends.append(ec_end)
+				all_directions.append(ec_direction)
+				all_coords.append([ec_start, ec_end, ec_direction])
+			assert (len(set(all_directions)) == 1)
+			start = min(all_starts)
+			end = max(all_ends)
+			direction = all_directions[0]
+		else:
+			is_multi_part = True
+			all_starts = []
+			all_ends = []
+			all_directions = []
+			for exon_coord in str(str_gbk_loc)[5:-1].split(', '):
+				ec_start = min(
+					[int(x.strip('>').strip('<')) for x in exon_coord[1:].split(']')[0].split(':')]) + 1
+				ec_end = max(
+					[int(x.strip('>').strip('<')) for x in exon_coord[1:].split(']')[0].split(':')])
+				ec_direction = exon_coord.split('(')[1].split(')')[0]
+				all_starts.append(ec_start)
+				all_ends.append(ec_end)
+				all_directions.append(ec_direction)
+				all_coords.append([ec_start, ec_end, ec_direction])
+			assert (len(set(all_directions)) == 1)
+			start = min(all_starts)
+			end = max(all_ends)
+			direction = all_directions[0]
+		return(all_coords, start, end, direction, is_multi_part)
+	except Exception as e:
+		raise RuntimeError(traceback.format_exc())
 
 def writeRefinedProteomes(s, sample_bgcs, refined_proteomes_outdir, logObject):
 	try:
 		refined_proteome_handle = open(refined_proteomes_outdir + s + '.faa', 'w')
 		for bgc in sample_bgcs:
 			with open(bgc) as obgc:
 				for rec in SeqIO.parse(obgc, 'genbank'):
@@ -688,57 +746,15 @@
 				new_seq_object = Seq(filtered_seq)
 
 				updated_rec = copy.deepcopy(rec)
 				updated_rec.seq = new_seq_object
 
 				updated_features = []
 				for feature in rec.features:
-					start = None
-					end = None
-					direction = None
-					all_coords = []
-
-					if not 'join' in str(feature.location) and not 'order' in str(feature.location):
-						start = min([int(x.strip('>').strip('<')) for x in
-									 str(feature.location)[1:].split(']')[0].split(':')]) + 1
-						end = max(
-							[int(x.strip('>').strip('<')) for x in str(feature.location)[1:].split(']')[0].split(':')])
-						direction = str(feature.location).split('(')[1].split(')')[0]
-						all_coords.append([start, end, direction])
-					elif 'order' in str(feature.location):
-						all_starts = []
-						all_ends = []
-						all_directions = []
-						for exon_coord in str(feature.location)[6:-1].split(', '):
-							start = min(
-								[int(x.strip('>').strip('<')) for x in exon_coord[1:].split(']')[0].split(':')]) + 1
-							end = max([int(x.strip('>').strip('<')) for x in exon_coord[1:].split(']')[0].split(':')])
-							direction = exon_coord.split('(')[1].split(')')[0]
-							all_starts.append(start)
-							all_ends.append(end)
-							all_directions.append(direction)
-							all_coords.append([start, end, direction])
-						start = min(all_starts)
-						end = max(all_ends)
-					else:
-						all_starts = []
-						all_ends = []
-						all_directions = []
-						for exon_coord in str(feature.location)[5:-1].split(', '):
-							start = min(
-								[int(x.strip('>').strip('<')) for x in exon_coord[1:].split(']')[0].split(':')]) + 1
-							end = max([int(x.strip('>').strip('<')) for x in exon_coord[1:].split(']')[0].split(':')])
-							direction = exon_coord.split('(')[1].split(')')[0]
-							all_starts.append(start)
-							all_ends.append(end)
-							all_directions.append(direction)
-							all_coords.append([start, end, direction])
-						start = min(all_starts)
-						end = max(all_ends)
-
+					all_coords, start, end, direction, is_multi_part = parseCDSCoord(str(feature.location))
 					feature_coords = set(range(start, end + 1))
 					if len(feature_coords.intersection(pruned_coords)) > 0:
 						fls = []
 						for sc, ec, dc in all_coords:
 							updated_start = sc - start_coord + 1
 							updated_end = ec - start_coord + 1
 							if ec > end_coord:
@@ -803,36 +819,15 @@
 		boundary_ranges = set(range(1, distance_to_scaffold_boundary + 1)).union(
 			set(range(scaffold_length - distance_to_scaffold_boundary, scaffold_length + 1)))
 		gene_starts = []
 		for feature in rec.features:
 			if not feature.type == 'CDS': continue
 			locus_tag = feature.qualifiers.get('locus_tag')[0]
 
-			start = None
-			end = None
-			direction = None
-			if not 'join' in str(feature.location):
-				start = min(
-					[int(x.strip('>').strip('<')) for x in str(feature.location)[1:].split(']')[0].split(':')]) + 1
-				end = max([int(x.strip('>').strip('<')) for x in str(feature.location)[1:].split(']')[0].split(':')])
-				direction = str(feature.location).split('(')[1].split(')')[0]
-			else:
-				all_starts = []
-				all_ends = []
-				all_directions = []
-				for exon_coord in str(feature.location)[5:-1].split(', '):
-					start = min([int(x.strip('>').strip('<')) for x in exon_coord[1:].split(']')[0].split(':')]) + 1
-					end = max([int(x.strip('>').strip('<')) for x in exon_coord[1:].split(']')[0].split(':')])
-					direction = exon_coord.split('(')[1].split(')')[0]
-					all_starts.append(start)
-					all_ends.append(end)
-					all_directions.append(direction)
-				start = min(all_starts)
-				end = max(all_ends)
-				direction = all_directions[0]
+			all_coords, start, end, direction, is_multi_part = parseCDSCoord(str(feature.location))
 
 			gene_location[locus_tag] = {'scaffold': scaffold, 'start': start, 'end': end, 'direction': direction}
 			scaffold_genes[scaffold].add(locus_tag)
 
 			gene_range = set(range(start, end + 1))
 			if len(gene_range.intersection(boundary_ranges)) > 0:
 				boundary_genes.add(locus_tag)
@@ -1486,43 +1481,15 @@
 						scaff_id, bgc_prediction_software, scaff_start)
 						rec.id = scaff_id
 						updated_rec = copy.deepcopy(rec)
 						updated_features = []
 						for feature in rec.features:
 							if feature.type == 'CDS':
 								try:
-									start = None
-									end = None
-									all_starts = []
-									all_ends = []
-									all_directions = []
-									all_coords = []
-									if not 'join' in str(feature.location):
-										start = min(
-											[int(x.strip('>').strip('<')) for x in
-											 str(feature.location)[1:].split(']')[0].split(':')]) + 1
-										end = max([int(x.strip('>').strip('<')) for x in
-												   str(feature.location)[1:].split(']')[0].split(':')])
-										direction = str(feature.location).split('(')[1].split(')')[0]
-										all_starts.append(start)
-										all_ends.append(end)
-									else:
-										all_starts = []
-										all_ends = []
-										all_directions = []
-										for exon_coord in str(feature.location)[5:-1].split(', '):
-											start = min([int(x.strip('>').strip('<')) for x in
-														 exon_coord[1:].split(']')[0].split(':')]) + 1
-											end = max([int(x.strip('>').strip('<')) for x in
-													   exon_coord[1:].split(']')[0].split(':')])
-											direction = exon_coord.split('(')[1].split(')')[0]
-											all_starts.append(start)
-											all_ends.append(end)
-									start = min(all_starts)
-									end = max(all_ends)
+									all_coords, start, end, direction, is_multi_part = parseCDSCoord(str(feature.location))
 									start = scaff_start + start
 									end = scaff_start + end
 									loc_tuple = tuple([scaff_id, str(start), str(end)])
 									prot_seq = str(feature.qualifiers.get('translation')[0]).replace('*', '')
 									prot_id = loc_to_tag[loc_tuple]
 									prot_id_by_seq = seq_to_tag[prot_seq]
 									assert (prot_id_by_seq == prot_id)
@@ -1554,47 +1521,15 @@
 				with open(bgc) as obf:
 					for rec in SeqIO.parse(obf, 'genbank'):
 						scaff_id = rec.id
 						scaff_start = int(rec.description.split()[-1].strip())
 						for feature in rec.features:
 							if feature.type == 'CDS':
 								prot_lt = feature.qualifiers.get('locus_tag')[0]
-								start = None
-								end = None
-								direction = None
-								all_starts = []
-								all_ends = []
-								all_directions = []
-								if not 'join' in str(feature.location):
-									start = min(
-										[int(x.strip('>').strip('<')) for x in
-										 str(feature.location)[1:].split(']')[0].split(':')]) + 1
-									end = max([int(x.strip('>').strip('<')) for x in
-											   str(feature.location)[1:].split(']')[0].split(':')])
-									direction = str(feature.location).split('(')[1].split(')')[0]
-									all_starts.append(start);
-									all_ends.append(end);
-									all_directions.append(direction)
-								else:
-									all_starts = []
-									all_ends = []
-									all_directions = []
-									for exon_coord in str(feature.location)[5:-1].split(', '):
-										start = min([int(x.strip('>').strip('<')) for x in
-													 exon_coord[1:].split(']')[0].split(':')]) + 1
-										end = max([int(x.strip('>').strip('<')) for x in
-												   exon_coord[1:].split(']')[0].split(':')])
-										direction = exon_coord.split('(')[1].split(')')[0]
-										all_starts.append(start);
-										all_ends.append(end);
-										all_directions.append(direction)
-								assert (len(set(all_directions)) == 1)
-								start = min(all_starts)
-								end = max(all_ends)
-								direction = all_directions[0]
+								all_coords, start, end, direction, is_multi_part = parseCDSCoord(str(feature.location))
 								prot_seq = str(feature.qualifiers.get('translation')[0]).replace('*', '')
 								sample_bgc_prots[sample][bgc].add(prot_lt)
 								samp_bgc_prot_handle.write('>' + ' '.join([str(x) for x in
 																		   [prot_lt, scaff_id, start, end,
 																			direction]]) + '\n' + prot_seq + '\n')
 			samp_bgc_prot_handle.close()
 	except Exception as e:
@@ -1983,31 +1918,15 @@
 					for rec in SeqIO.parse(obf, 'genbank'):
 						scaff_id = rec.id
 						scaff_start = int(rec.description.split()[-1].strip())
 						for feature in rec.features:
 							if feature.type == 'CDS':
 								prot_lt = feature.qualifiers.get('locus_tag')[0]
 								if prot_lt in bgc_prots_1x:
-									all_coords = []
-									if not 'join' in str(feature.location):
-										start = scaff_start + min(
-											[int(x.strip('>').strip('<')) for x in
-											 str(feature.location)[1:].split(']')[0].split(':')]) + 1
-										end = scaff_start + max([int(x.strip('>').strip('<')) for x in
-																 str(feature.location)[1:].split(']')[0].split(':')])
-										direction = str(feature.location).split('(')[1].split(')')[0]
-										all_coords.append([start, end, direction])
-									else:
-										for exon_coord in str(feature.location)[5:-1].split(', '):
-											start = scaff_start + min([int(x.strip('>').strip('<')) for x in
-																	   exon_coord[1:].split(']')[0].split(':')]) + 1
-											end = scaff_start + max([int(x.strip('>').strip('<')) for x in
-																	 exon_coord[1:].split(']')[0].split(':')])
-											direction = exon_coord.split('(')[1].split(')')[0]
-											all_coords.append([start, end, direction])
+									all_coords, start, end, direction, is_multi_part = parseCDSCoord(str(feature.location))
 									fls = []
 									for sc, ec, dc in all_coords:
 										dir = 1
 										if dc == '-': dir = -1
 										fls.append(FeatureLocation(sc - 1, ec, strand=dir))
 									feat_loc = fls[0]
 									if len(fls) > 1:
@@ -2069,47 +1988,27 @@
 						if protein_annotations == None:
 							feature.qualifiers['product'] = 'hypothetical protein'
 						else:
 							feature.qualifiers['product'] = [protein_annotations[sample][prot_lt]]
 						feature.qualifiers.move_to_end('translation')
 						if prot_lt in sample_lts_to_prune: continue
 						updated_features.append(feature)
-						all_starts = []
-						if not 'join' in str(feature.location):
-							start = min([int(x.strip('>').strip('<')) for x in
-										 str(feature.location)[1:].split(']')[0].split(':')]) + 1
-							all_starts.append(start)
-						else:
-							for exon_coord in str(feature.location)[5:-1].split(', '):
-								start = min(
-									[int(x.strip('>').strip('<')) for x in exon_coord[1:].split(']')[0].split(':')]) + 1
-								all_starts.append(start)
-						start = min(all_starts)
+						all_coords, start, end, direction, is_multi_part = parseCDSCoord(str(feature.location))
 						starts.append([cds_iter, start])
 						cds_iter += 1
 				for feature in sample_lts_to_add_genbank_features[rec.id]:
 					if feature.type == 'CDS':
 						prot_lt = feature.qualifiers.get('locus_tag')[0]
 						if protein_annotations == None:
 							feature.qualifiers['product'] = 'hypothetical protein'
 						else:
 							feature.qualifiers['product'] = [protein_annotations[sample][prot_lt]]
 						feature.qualifiers.move_to_end('translation')
 						updated_features.append(feature)
-						all_starts = []
-						if not 'join' in str(feature.location):
-							start = min([int(x.strip('>').strip('<')) for x in
-										 str(feature.location)[1:].split(']')[0].split(':')]) + 1
-							all_starts.append(start)
-						else:
-							for exon_coord in str(feature.location)[5:-1].split(', '):
-								start = min(
-									[int(x.strip('>').strip('<')) for x in exon_coord[1:].split(']')[0].split(':')]) + 1
-								all_starts.append(start)
-						start = min(all_starts)
+						all_coords, start, end, direction, is_multi_part = parseCDSCoord(str(feature.location))
 						starts.append([cds_iter, start])
 						cds_iter += 1
 				sorted_updated_features = []
 				for sort_i in sorted(starts, key=itemgetter(1)):
 					sorted_updated_features.append(updated_features[sort_i[0]])
 				rec.features = sorted_updated_features
 				SeqIO.write(rec, gbk_handle, 'genbank')
@@ -2221,30 +2120,15 @@
 					for rec in SeqIO.parse(obf, 'genbank'):
 						scaff_id = rec.id
 						scaff_start = int(rec.description.split()[-1].strip())
 						for feature in rec.features:
 							if feature.type == 'CDS':
 								prot_lt = feature.qualifiers.get('locus_tag')[0]
 								if not prot_lt in bgc_prots_1x: continue
-								all_coords = []
-								if not 'join' in str(feature.location):
-									start = scaff_start + min(
-										[int(x) for x in str(feature.location)[1:].split(']')[0].split(':')]) + 1
-									end = scaff_start + max(
-										[int(x) for x in str(feature.location)[1:].split(']')[0].split(':')])
-									direction = str(feature.location).split('(')[1].split(')')[0]
-									all_coords.append([start, end, direction])
-								else:
-									for exon_coord in str(feature.location)[5:-1].split(', '):
-										start = scaff_start + min([int(x.strip('>').strip('<')) for x in
-																   exon_coord[1:].split(']')[0].split(':')]) + 1
-										end = scaff_start + max([int(x.strip('>').strip('<')) for x in
-																 exon_coord[1:].split(']')[0].split(':')])
-										direction = exon_coord.split('(')[1].split(')')[0]
-										all_coords.append([start, end, direction])
+								all_coords, start, end, direction, is_multi_part = parseCDSCoord(str(feature.location))
 								fls = []
 								for sc, ec, dc in all_coords:
 									dir = 1
 									if dc == '-': dir = -1
 									fls.append(FeatureLocation(sc - 1, ec, strand=dir))
 								feat_loc = fls[0]
 								if len(fls) > 1:
@@ -2296,47 +2180,27 @@
 						if protein_annotations == None:
 							feature.qualifiers['product'] = 'hypothetical protein'
 						else:
 							feature.qualifiers['product'] = [protein_annotations[sample][prot_lt]]
 						feature.qualifiers.move_to_end('translation')
 						if prot_lt in sample_lts_to_prune: continue
 						updated_features.append(feature)
-						all_starts = []
-						if not 'join' in str(feature.location):
-							start = min([int(x.strip('>').strip('<')) for x in
-										 str(feature.location)[1:].split(']')[0].split(':')]) + 1
-							all_starts.append(start)
-						else:
-							for exon_coord in str(feature.location)[5:-1].split(', '):
-								start = min(
-									[int(x.strip('>').strip('<')) for x in exon_coord[1:].split(']')[0].split(':')]) + 1
-								all_starts.append(start)
-						start = min(all_starts)
+						all_coords, start, end, direction, is_multi_part = parseCDSCoord(str(feature.location))
 						starts.append([cds_iter, start])
 						cds_iter += 1
 				for feature in sample_lts_to_add_genbank_features[rec.id]:
 					if feature.type == 'CDS':
 						prot_lt = feature.qualifiers.get('locus_tag')[0]
 						if protein_annotations == None:
 							feature.qualifiers['product'] = 'hypothetical protein'
 						else:
 							feature.qualifiers['product'] = [protein_annotations[sample][prot_lt]]
 						feature.qualifiers.move_to_end('translation')
 						updated_features.append(feature)
-						all_starts = []
-						if not 'join' in str(feature.location):
-							start = min([int(x.strip('>').strip('<')) for x in
-										 str(feature.location)[1:].split(']')[0].split(':')]) + 1
-							all_starts.append(start)
-						else:
-							for exon_coord in str(feature.location)[5:-1].split(', '):
-								start = min(
-									[int(x.strip('>').strip('<')) for x in exon_coord[1:].split(']')[0].split(':')]) + 1
-								all_starts.append(start)
-						start = min(all_starts)
+						all_coords, start, end, direction, is_multi_part = parseCDSCoord(str(feature.location))
 						starts.append([cds_iter, start])
 						cds_iter += 1
 				sorted_updated_features = []
 				for sort_i in sorted(starts, key=itemgetter(1)):
 					sorted_updated_features.append(updated_features[sort_i[0]])
 				rec.features = sorted_updated_features
 				SeqIO.write(rec, gbk_handle, 'genbank')
@@ -2747,29 +2611,32 @@
 
 	e1 = float(c1) / a1
 	e2 = float(c2) / ((a1 ** 2) + a2)
 	if S >= 3:
 		D = (float(pi - (float(S) / a1)) / math.sqrt((e1 * S) + ((e2 * S) * (S - 1))))
 		return (D)
 	else:
-		return ("NA")
+		return ("< 3 segregating sites")
 
 
 def is_numeric(x):
 	try:
 		x = float(x)
 		return True
 	except:
 		return False
 
 
 def castToNumeric(x):
 	try:
-		x = float(x)
-		return (x)
+		if x != '< 3 segregating sites':
+			x = float(x)
+			return(x)
+		else:
+			return(x)
 	except:
 		return float('nan')
 
 
 numeric_columns = set(['GCF Count', 'hg order index', 'hg consensus direction', 'median gene length',
 					   'proportion of samples with hg', 'proportion of total populations with hg',
 					   'hg median copy count', 'num of hg instances', 'samples with hg', 'ambiguous sites proporition',
@@ -2844,56 +2711,76 @@
 		panda_df = pd.DataFrame(panda_dict)
 
 	except Exception as e:
 		raise RuntimeError(traceback.format_exc())
 	return panda_df
 
 
-def loadTableInPandaDataFrame(input_file):
+def loadTableInPandaDataFrame(input_file, mibig_info=None):
 	import pandas as pd
 	panda_df = None
 	try:
 		data = []
+		mibig_col = []
 		with open(input_file) as oif:
-			for line in oif:
+			for i, line in enumerate(oif):
 				line = line.strip('\n')
 				ls = line.split('\t')
 				data.append(ls)
+				gcf = ls[0]
+				hg = ls[2]
+				key = gcf + '|' + hg
+				if mibig_info != None and i > 0:
+					if len(mibig_info[key]) > 0:
+						mibig_col.append('; '.join(sorted(mibig_info[key])))
+					else:
+						mibig_col.append('NA')
 
 		panda_dict = {}
 		for ls in zip(*data):
 			key = ' '.join(ls[0].split('_'))
 			cast_vals = ls[1:]
 			if key in numeric_columns:
 				cast_vals = []
 				for val in ls[1:]:
 					cast_vals.append(castToNumeric(val))
 			panda_dict[key] = cast_vals
+			if key == 'annotation' and mibig_info != None and len(mibig_info) > 0:
+				panda_dict['MIBiG mapping'] = mibig_col
 		panda_df = pd.DataFrame(panda_dict)
 
 	except Exception as e:
 		raise RuntimeError(traceback.format_exc())
 	return panda_df
 
 
-def loadCustomPopGeneTableInPandaDataFrame(input_file):
+def loadCustomPopGeneTableInPandaDataFrame(input_file, mibig_info=None):
 	import pandas as pd
 	panda_df = None
 	try:
 		ignore_data_cats = {'hg_median_copy_count', 'proportion_of_total_populations_with_hg',
 							'proportion_variable_sites', 'proportion_nondominant_major_allele', 'median_dn_ds',
 							'mad_dn_ds', 'all_domains', 'most_significant_Fisher_exact_pvalues_presence_absence',
 							'median_Tajimas_D_per_population', 'mad_Tajimas_D_per_population',
 							'most_negative_population_Tajimas_D', 'most_positive_population_Tajimas_D',
 							'population_entropy', 'median_fst_like_estimate'}
 		data = []
+		mibig_col = []
 		with open(input_file) as oif:
-			for line in oif:
+			for i, line in enumerate(oif):
 				line = line.strip('\n')
 				ls = line.split('\t')
+				gcf = ls[0]
+				hg = ls[2]
+				key = gcf + '|' + hg
+				if mibig_info != None and i > 0:
+					if len(mibig_info[key]) > 0:
+						mibig_col.append('; '.join(sorted(mibig_info[key])))
+					else:
+						mibig_col.append('NA')
 				data.append(ls)
 
 		panda_dict = {}
 		for ls in zip(*data):
 			if ls[0] in ignore_data_cats: continue
 			if ls[0] == 'gcf_annotation':
 				updated_ans = []
@@ -2913,18 +2800,21 @@
 						if a != 'hypothetical protein':
 							ca.append(a)
 					if len(ca) == 0:
 						cleaned_annots.append('hypothetical protein')
 					else:
 						cleaned_annots.append('; '.join(ca))
 				panda_dict[key] = cleaned_annots
+				if mibig_info != None and len(mibig_info) > 0:
+					panda_dict['MIBiG mapping'] = mibig_col
 			else:
 				key = ' '.join(ls[0].split('_'))
 				cast_vals = ls[1:]
 				if key in numeric_columns:
+
 					cast_vals = []
 					for val in ls[1:]:
 						cast_vals.append(castToNumeric(val))
 				panda_dict[key] = cast_vals
 		panda_df = pd.DataFrame(panda_dict)
 
 	except Exception as e:
```

### Comparing `lsaBGC-1.33/lsaBGC.egg-info/SOURCES.txt` & `lsaBGC-1.34/lsaBGC.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.md
 setup.py
 bin/lsaBGC-Cluster.py
 bin/lsaBGC-DiscoVary.py
 bin/lsaBGC-Divergence.py
 bin/lsaBGC-Expansion.py
+bin/lsaBGC-MIBiGMapper.py
 bin/lsaBGC-PopGene.py
 bin/lsaBGC-Ready.py
 bin/lsaBGC-Refiner.py
 bin/lsaBGC-See.py
 lsaBGC/__init__.py
 lsaBGC/processing.py
 lsaBGC/util.py
@@ -25,10 +26,12 @@
 scripts/popSizeAndSampleSelector.py
 scripts/processAndReformatNCBIGenbanks.py
 scripts/readifyAdditionalGenomes.py
 scripts/runProdigalAndMakeProperGenbank.py
 scripts/setup_annotation_dbs.py
 scripts/setup_bigscape.py
 scripts/simpleProteinExtraction.py
+scripts/visualize_BGC-Ome.py
 workflows/lsaBGC-AutoAnalyze.py
 workflows/lsaBGC-AutoExpansion.py
-workflows/lsaBGC-Easy.py
+workflows/lsaBGC-Easy.py
+workflows/lsaBGC-Euk-Easy.py
```

### Comparing `lsaBGC-1.33/scripts/GSeeF.py` & `lsaBGC-1.34/scripts/GSeeF.py`

 * *Files identical despite different names*

### Comparing `lsaBGC-1.33/scripts/compareBGCtoGenomeCodonUsage.py` & `lsaBGC-1.34/scripts/compareBGCtoGenomeCodonUsage.py`

 * *Files identical despite different names*

### Comparing `lsaBGC-1.33/scripts/createPickleOfSampleAnnotationListingFile.py` & `lsaBGC-1.34/scripts/createPickleOfSampleAnnotationListingFile.py`

 * *Files identical despite different names*

### Comparing `lsaBGC-1.33/scripts/listAllBGCGenbanksInDirectory.py` & `lsaBGC-1.34/scripts/listAllBGCGenbanksInDirectory.py`

 * *Files identical despite different names*

### Comparing `lsaBGC-1.33/scripts/listAllGenomesInDirectory.py` & `lsaBGC-1.34/scripts/listAllGenomesInDirectory.py`

 * *Files identical despite different names*

### Comparing `lsaBGC-1.33/scripts/popSizeAndSampleSelector.py` & `lsaBGC-1.34/scripts/popSizeAndSampleSelector.py`

 * *Files identical despite different names*

### Comparing `lsaBGC-1.33/scripts/processAndReformatNCBIGenbanks.py` & `lsaBGC-1.34/scripts/processAndReformatNCBIGenbanks.py`

 * *Files identical despite different names*

### Comparing `lsaBGC-1.33/scripts/readifyAdditionalGenomes.py` & `lsaBGC-1.34/scripts/readifyAdditionalGenomes.py`

 * *Files identical despite different names*

### Comparing `lsaBGC-1.33/scripts/runProdigalAndMakeProperGenbank.py` & `lsaBGC-1.34/scripts/runProdigalAndMakeProperGenbank.py`

 * *Files identical despite different names*

### Comparing `lsaBGC-1.33/scripts/setup_annotation_dbs.py` & `lsaBGC-1.34/scripts/setup_annotation_dbs.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,11 @@
 import os
 import sys
 import argparse
 from Bio import SeqIO
-from collections import defaultdict
-from time import sleep
-from lsaBGC import util
-import subprocess
-import traceback
-import multiprocessing
 
 lsaBGC_main_directory = '/'.join(os.path.realpath(__file__).split('/')[:-2]) + '/'
 
 def create_parser():
     """ Parse arguments """
     parser = argparse.ArgumentParser(description="""
 	Program: setup_annotation_dbs.py
@@ -36,14 +30,16 @@
     download_path = os.path.abspath(myargs.download_path) + '/'
 
     try:
         assert(os.path.isdir(download_path))
     except:
         sys.stderr.write('Error: Provided directory for downloading annotation files does not exist!\n')
 
+    listing_file = lsaBGC_main_directory + 'db/database_location_paths.txt'
+
     # download files in requested directory
     try:
         os.chdir(download_path)
 
         ko_annot_info_file = download_path + 'ko_list'
         ko_phmm_file = download_path + 'profile.hmm'
 
@@ -61,15 +57,14 @@
 
             if os.path.isfile(ko_phmm_file):
                 os.system('rm -f %s' % ko_phmm_file)
             for f in os.listdir(download_path + 'profiles/'):
                 os.system('cat %s >> %s' % (download_path + 'profiles/' + f, ko_phmm_file))
 
             assert(os.path.isfile(ko_phmm_file))
-            listing_file = lsaBGC_main_directory + 'db/database_location_paths.txt'
             listing_handle = open(listing_file, 'w')
             listing_handle.write('ko\t' + ko_annot_info_file + '\t' + ko_phmm_file + '\n')
             listing_handle.close()
             os.system('rm -rf %s %s' % (download_path + 'profiles/', download_path + 'profiles.tar.gz'))
 
         pgap_info_file = download_path + 'hmm_PGAP.tsv'
         pgap_hmm_file = download_path + 'PGAP.hmm'
@@ -83,19 +78,40 @@
 
             assert(os.path.isfile(pgap_info_file))
             assert(os.path.isdir(download_path + 'hmm_PGAP/'))
 
             for f in os.listdir(download_path + 'hmm_PGAP/'):
                 os.system('cat %s >> %s' % (download_path + 'hmm_PGAP/' + f, pgap_hmm_file))
             assert(os.path.isfile(ko_phmm_file))
-            listing_file = lsaBGC_main_directory + 'db/database_location_paths.txt'
             listing_handle = open(listing_file, 'a+')
             listing_handle.write('pgap\t' + pgap_info_file + '\t' + pgap_hmm_file + '\n')
             listing_handle.close()
             os.system('rm -rf %s %s' % (download_path + 'hmm_PGAP/', download_path + 'hmm_PGAP.HMM.tgz'))
 
+
+        mibig_faa_file = download_path + 'mibig_prot_seqs_3.1.fasta'
+        mibig_dmnd_file = download_path + 'mibig.dmnd'
+        mibig_info_file = download_path + 'mibig_info.txt'
+
+        if not os.path.isfile(mibig_info_file) or not os.path.isfile(mibig_dmnd_file):
+            # Download MIBiG
+            print('Setting up MIBiGv3.1 database!')
+            os.system('wget https://dl.secondarymetabolites.org/mibig/mibig_prot_seqs_3.1.fasta')
+            assert(os.path.isfile(mibig_faa_file))
+            os.system(' '.join(['diamond', 'makedb', '--in', mibig_faa_file, '-d', mibig_dmnd_file]))
+            assert(os.path.isfile(mibig_dmnd_file))
+            mdf_handle = open(mibig_info_file, 'w')
+            with open(mibig_faa_file) as omf:
+                for rec in SeqIO.parse(omf, 'fasta'):
+                    mdf_handle.write(rec.id + '\t' + rec.description + '\n')
+            mdf_handle.close()
+            assert(os.path.isfile(mibig_info_file))
+
+            listing_handle = open(listing_file, 'a+')
+            listing_handle.write('mibig\t' + mibig_info_file + '\t' + mibig_dmnd_file + '\n')
+            listing_handle.close()
     except:
         sys.stderr.write('Error: issues with downloading or seting up annotation database files! Please post to Github issues if unable to figure out!\n')
 
     sys.exit(0)
 
 setup_annot_dbs()
```

### Comparing `lsaBGC-1.33/scripts/setup_bigscape.py` & `lsaBGC-1.34/scripts/setup_bigscape.py`

 * *Files identical despite different names*

### Comparing `lsaBGC-1.33/scripts/simpleProteinExtraction.py` & `lsaBGC-1.34/scripts/simpleProteinExtraction.py`

 * *Files identical despite different names*

### Comparing `lsaBGC-1.33/setup.py` & `lsaBGC-1.34/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 from setuptools import setup
 
 setup(name='lsaBGC',
-      version='1.33',
+      version='1.34',
       description='Suite for comparative genomic, population genetics and evolutionary analysis, as well as metagenomic mining of micro-evolutionary novelty in BGCs all in the context of a single lineage of interest.',
       url='http://github.com/Kalan-Lab/lsaBGC/',
       author='Rauf Salamzade',
       author_email='salamzader@gmail.com',
       license='BSD-3',
       packages=['lsaBGC'],
       scripts=['scripts/setup_annotation_dbs.py',
                'scripts/setup_bigscape.py',
                'scripts/GSeeF.py',
                'scripts/compareBGCtoGenomeCodonUsage.py',
                'scripts/listAllGenomesInDirectory.py',
                'scripts/listAllBGCGenbanksInDirectory.py',
                'scripts/runProdigalAndMakeProperGenbank.py',
+               'scripts/visualize_BGC-Ome.py',
                'scripts/processAndReformatNCBIGenbanks.py',
                'scripts/simpleProteinExtraction.py',
                'scripts/createPickleOfSampleAnnotationListingFile.py',
                'scripts/popSizeAndSampleSelector.py',
                'scripts/readifyAdditionalGenomes.py',
                'workflows/lsaBGC-Easy.py',
+               'workflows/lsaBGC-Euk-Easy.py',
                'workflows/lsaBGC-AutoAnalyze.py',
                'workflows/lsaBGC-AutoExpansion.py',
                'bin/lsaBGC-Ready.py',
                'bin/lsaBGC-Cluster.py',
                'bin/lsaBGC-See.py',
                'bin/lsaBGC-PopGene.py', 
                'bin/lsaBGC-Refiner.py', 
                'bin/lsaBGC-Expansion.py', 
                'bin/lsaBGC-Divergence.py', 
-               'bin/lsaBGC-DiscoVary.py'],
-      zip_safe=False)
+               'bin/lsaBGC-DiscoVary.py',
+               'bin/lsaBGC-MIBiGMapper.py'],
+      zip_safe=False)
```

### Comparing `lsaBGC-1.33/workflows/lsaBGC-AutoAnalyze.py` & `lsaBGC-1.34/workflows/lsaBGC-AutoAnalyze.py`

 * *Files 27% similar despite different names*

```diff
@@ -42,19 +42,22 @@
 from operator import itemgetter
 import argparse
 from collections import defaultdict
 from Bio import SeqIO
 from lsaBGC import util
 import pandas as pd
 from ete3 import Tree
+import warnings
+warnings.filterwarnings('ignore')
 
 lsaBGC_main_directory = '/'.join(os.path.realpath(__file__).split('/')[:-2])
 RSCRIPT_FOR_NJTREECONSTRUCTION = lsaBGC_main_directory + '/lsaBGC/Rscripts/createNJTree.R'
 RSCRIPT_FOR_DEFINECLADES_FROM_PHYLO = lsaBGC_main_directory + '/lsaBGC/Rscripts/defineCladesFromPhylo.R'
 RSCRIPT_FOR_BIGPICTUREHEATMAP = lsaBGC_main_directory + '/lsaBGC/Rscripts/plotBigPictureHeatmap.R'
+RSCRIPT_FOR_BIGPICTUREPHYLO = lsaBGC_main_directory + '/lsaBGC/Rscripts/plotBigPicturePhyloWithLabels.R'
 RSCRIPT_FOR_GCFGENEPLOTS = lsaBGC_main_directory + '/lsaBGC/Rscripts/gcfGenePlots.R'
 RSCRIPT_FOR_DIVERGENCEPLOT = lsaBGC_main_directory + '/lsaBGC/Rscripts/divergencePlot.R'
 RSCRIPT_FOR_POPULATIONS_ON_PHYLO = lsaBGC_main_directory + '/lsaBGC/Rscripts/GeneRatePhylogeny.R'
 
 def create_parser():
 	""" Parse arguments """
 	parser = argparse.ArgumentParser(description="""
@@ -64,26 +67,27 @@
 
 	Wrapper program to automate running lsaBGC analytical programs for each GCF. 
 	
 	Iteratively runs lsaBGC-See.py, lsaBGC-PopGene.py, lsaBGC-Divergence.py, and optionally lsaBGC-DiscoVary.py for
 	each GCF in a GCF listings directory, produced by lsaBGC-Ready, lsaBGC-Cluster, or lsaBGC-AutoExpansion.py.
 	""", formatter_class=argparse.RawTextHelpFormatter)
 
-	parser.add_argument('-o', '--output_directory', help="Parent output/workspace directory.", required=True)
-	parser.add_argument('-i', '--input_listing', help="Path to tab delimited file listing: (1) sample name\n(2) path to whole-genome Genbank and (3) path to whole-genome predicted proteome\n(an output of lsaBGC-Ready.py or lsaBGC-AutoExpansion.py).", required=False, default=None)
+	parser.add_argument('-i', '--input_listing', help="Path to tab delimited file listing: (1) sample name\n(2) path to whole-genome Genbank and (3) path to whole-genome predicted proteome\n(an output of lsaBGC-Ready.py or lsaBGC-AutoExpansion.py).", required=True)
 	parser.add_argument('-g', '--gcf_listing_dir', help='Directory with GCF listing files.', required=True)
 	parser.add_argument('-m', '--orthofinder_matrix', help="OrthoFinder homolog group by sample matrix.", required=True)
-	parser.add_argument('-k', '--sample_set', help="Sample set to keep in analysis. Should be file with one sample id per line.", required=False)
-	parser.add_argument('-s', '--species_phylogeny', help="Path to species phylogeny. If not provided a FastANI based neighborjoining tree will be constructed and used.", default=None, required=False)
+	parser.add_argument('-o', '--output_directory', help="Parent output/workspace directory.", required=True)
+	parser.add_argument('-k', '--sample_set', help="Sample set to keep in analysis. Should be file with one sample\nid per line.", required=False, default=None)
+	parser.add_argument('-s', '--species_phylogeny', help="Path to species phylogeny. If not provided a FastANI based neighborjoining\ntree will be constructed and used.", default=None, required=False)
 	parser.add_argument('-w', '--expected_similarities', help="Path to file listing expected similarities between genomes/samples. This is\ncomputed most easily by running lsaBGC-Ready.py with '-t' specified, which will estimate\nsample to sample similarities based on alignment used to create species phylogeny.", required=True)
-	parser.add_argument('-p', '--bgc_prediction_software', help='Software used to predict BGCs (Options: antiSMASH, DeepBGC, GECCO).\nDefault is antiSMASH.', default='antiSMASH', required=False)
+	parser.add_argument('-p', '--bgc_prediction_software', help='Software used to predict BGCs (Options: antiSMASH, DeepBGC, GECCO)\n[Default is antiSMASH].', default='antiSMASH', required=False)
 	parser.add_argument('-u', '--populations', help='Path to user defined populations/groupings file. Tab delimited with 2 columns: (1) sample name and (2) group identifier.', required=False, default=None)
-	parser.add_argument('-l', '--discovary_input_listing', help="Sequencing readsets for DiscoVary analysis. Tab delimited file listing: (1) sample name, (2) forward readset, (3) reverse readset for metagenomic/isolate sequencing data.", required=False, default=None)
-	parser.add_argument('-n', '--discovary_analysis_name', help="Identifier/name for DiscoVary. Not providing this parameter will avoid running lsaBGC-DiscoVary step.", required=False, default=None)
-	parser.add_argument('-c', '--cpus', type=int, help="Total number of cpus to use.", required=False, default=1)
+	parser.add_argument('-l', '--discovary_input_listing', help="Sequencing readsets for DiscoVary analysis. Tab delimited file listing:\n(1) sample name, (2) forward readset, (3) reverse readset for metagenomic/isolate\nsequencing data.", required=False, default=None)
+	parser.add_argument('-n', '--discovary_analysis_name', help="Identifier/name for DiscoVary. Not providing this parameter will avoid\nrunning lsaBGC-DiscoVary step.", required=False, default=None)
+	parser.add_argument('-mb', '--run_mibig_mapper', action='store_true', help="Run MIBiG mapping analysis.", default=False, required=False)
+	parser.add_argument('-c', '--cpus', type=int, help="Total number of CPUs to use [Default is 1].", required=False, default=1)
 
 	args = parser.parse_args()
 	return args
 
 def lsaBGC_AutoAnalyze():
 	"""
 	Void function which runs primary workflow for program.
@@ -153,14 +157,15 @@
 	sample_set_file = myargs.sample_set
 	bgc_prediction_software = myargs.bgc_prediction_software.upper()
 	species_phylogeny_file = myargs.species_phylogeny
 	expected_distances = myargs.expected_similarities
 	population_listing_file = myargs.populations
 	discovary_analysis_id = myargs.discovary_analysis_name
 	discovary_input_listing = myargs.discovary_input_listing
+	run_mibig_mapper = myargs.run_mibig_mapper
 	cpus = myargs.cpus
 
 	try:
 		assert (bgc_prediction_software in set(['ANTISMASH', 'DEEPBGC', 'GECCO']))
 	except:
 		raise RuntimeError('BGC prediction software option is not a valid option.')
 
@@ -218,21 +223,22 @@
 	logObject.info('Running version %s' % version_string)
 
 	# Step 0: Log input arguments and update reference and query FASTA files.
 	logObject.info("Saving parameters for easier determination of results basis in the future.")
 	parameters_file = outdir + 'Parameter_Inputs.txt'
 	parameter_values = [gcf_listing_dir, input_listing_file, original_orthofinder_matrix_file, outdir,
 						species_phylogeny_file, expected_distances, population_listing_file,
-						discovary_analysis_id, discovary_input_listing, bgc_prediction_software, sample_set_file, cpus]
+						discovary_analysis_id, discovary_input_listing, bgc_prediction_software,
+						sample_set_file, run_mibig_mapper, cpus]
 	parameter_names = ["GCF Listings Directory", "Listing File of Sample Annotation Files for Initial Set of Samples",
 					   "OrthoFinder Homolog Matrix", "Output Directory", "Species Phylogeny File in Newick Format",
 					   "File with Expected Sample to Sample Amino Acid Distance Estimations",
 					   "Clade/Population Listings File", "DiscoVary Analysis ID",
 					   "DiscoVary Sequencing Data Location Specification File", "BGC Prediction Software",
-					   "Sample Retention Set", "cpus"]
+					   "Sample Retention Set", "Run MIBiG Mapping Analysis?", "CPUs"]
 	util.logParametersToFile(parameters_file, parameter_names, parameter_values)
 	logObject.info("Done saving parameters!")
 
 	# Step 0: (Optional) Parse sample set retention specifications file, if provided by the user.
 	sample_retention_set = util.getSampleRetentionSet(sample_set_file)
 
 	if sample_retention_set != None:
@@ -307,86 +313,113 @@
 				line = line.strip()
 				samp, pop = line.split('\t')
 				pop_size[pop] += 1
 
 	see_outdir = outdir + 'See/'
 	pop_outdir = outdir + 'PopGene/'
 	div_outdir = outdir + 'Divergence/'
+	mbmap_outdir = outdir + 'MIBiG_Mapping/'
+
 	if not os.path.isdir(see_outdir): os.system('mkdir %s' % see_outdir)
 	if not os.path.isdir(pop_outdir): os.system('mkdir %s' % pop_outdir)
 	if not os.path.isdir(div_outdir): os.system('mkdir %s' % div_outdir)
 
 	if discovary_analysis_id and discovary_input_listing:
 		dis_outdir = outdir + 'DiscoVary_' + '_'.join(discovary_analysis_id.split()) + '/'
 		if not os.path.isdir(dis_outdir): os.system('mkdir %s' % dis_outdir)
 
+	if run_mibig_mapper:
+		if not os.path.isdir(mbmap_outdir): os.system('mkdir %s' % mbmap_outdir)
+
 	for g in os.listdir(gcf_listing_dir):
 		gcf_id = g.split('.txt')[0]
 		gcf_listing_file = gcf_listing_dir + g
+
+		gcf_samples = set([])
+		with open(gcf_listing_file) as oglf:
+			for line in oglf:
+				line = line.strip()
+				sample, bgc_gbk = line.split('\t')
+				gcf_samples.add(sample)
+
 		orthofinder_matrix_file = original_orthofinder_matrix_file
 		logObject.info("Beginning analysis for GCF %s" % gcf_id)
 		sys.stderr.write("Beginning analysis for GCF %s\n" % gcf_id)
 
 		# 1. Run lsaBGC-See.py
 		gcf_see_outdir = see_outdir + gcf_id + '/'
 		lsabgc_see_checkpoint = gcf_see_outdir + 'CHECKPOINT.txt'
 		if not os.path.isfile(lsabgc_see_checkpoint):
 			os.system('rm -rf %s' % gcf_see_outdir)
-			os.system('mkdir %s' % gcf_see_outdir)
 			cmd = ['lsaBGC-See.py', '-g', gcf_listing_file, '-m', orthofinder_matrix_file, '-o', gcf_see_outdir,
 				   '-i', gcf_id, '-s', species_phylogeny_file, '-p', bgc_prediction_software, '-c', str(cpus)]
 			try:
+				#print(' '.join(cmd))
 				util.run_cmd(cmd, logObject)
 				assert(os.path.isfile(lsabgc_see_checkpoint))
 			except Exception as e:
 				logObject.warning("lsaBGC-See.py was unsuccessful for GCF %s" % gcf_id)
 				sys.stderr.write("Warning: lsaBGC-See.py was unsuccessful for GCF %s\n" % gcf_id)
 
 		# 2. Run lsaBGC-PopGene.py
 		gcf_pop_outdir = pop_outdir + gcf_id + '/'
 		lsabgc_popgene_checkpoint = gcf_pop_outdir + 'CHECKPOINT.txt'
 		if not os.path.isfile(lsabgc_popgene_checkpoint):
 			os.system('rm -rf %s' % gcf_pop_outdir)
-			os.system('mkdir %s' % gcf_pop_outdir)
 			cmd = ['lsaBGC-PopGene.py', '-g', gcf_listing_file, '-m', orthofinder_matrix_file, '-o', gcf_pop_outdir,
 				   '-i', gcf_id, '-p', bgc_prediction_software, '-c', str(cpus)]
 			if expected_distances != None:
 				cmd += ['-w', expected_distances]
 			if population_listing_file != None:
 				cmd += ['-u', population_listing_file]
 			try:
+				#print(' '.join(cmd))
 				util.run_cmd(cmd, logObject, stderr=sys.stderr, stdout=sys.stdout)
 				assert(os.path.isfile(lsabgc_popgene_checkpoint))
 			except Exception as e:
 				logObject.warning("lsaBGC-PopGene.py was unsuccessful for GCF %s" % gcf_id)
 				sys.stderr.write("Warning: lsaBGC-PopGene.py was unsuccessful for GCF %s\n" % gcf_id)
 
 		# 3. Run lsaBGC-Divergence.py
 		gcf_div_outdir = div_outdir + gcf_id + '/'
 		lsabgc_divergence_checkpoint = gcf_div_outdir + 'CHECKPOINT.txt'
-		if not os.path.isfile(lsabgc_divergence_checkpoint) and expected_distances:
+		if (not os.path.isfile(lsabgc_divergence_checkpoint)) and expected_distances and len(gcf_samples) > 1:
 			os.system('rm -rf %s' % gcf_div_outdir)
-			os.system('mkdir %s' % gcf_div_outdir)
 			cmd = ['lsaBGC-Divergence.py', '-g', gcf_listing_file, '-l', input_listing_file, '-o', gcf_div_outdir,
 				   '-i', gcf_id, '-a',	gcf_pop_outdir + 'Codon_Alignments_Listings.txt', '-c', str(cpus),'-w',
 				   expected_distances]
 			try:
+				#print(' '.join(cmd))
 				util.run_cmd(cmd, logObject)
 				assert(os.path.isfile(lsabgc_divergence_checkpoint))
 			except Exception as e:
 				logObject.warning("lsaBGC-Divergence.py was unsuccessful for GCF %s" % gcf_id)
 				sys.stderr.write("Warning: lsaBGC-Divergence.py was unsuccessful for GCF %s\n" % gcf_id)
 
-		# 4. Run lsaBGC-DiscoVary.py
+		# 4. Run lsaBGC-MIBiGMapper.py
+		gcf_mbm_outdir = mbmap_outdir + gcf_id + '/'
+		lsabgc_mibigmap_checkpoint = gcf_mbm_outdir + 'CHECKPOINT.txt'
+		if not os.path.isfile(lsabgc_mibigmap_checkpoint) and run_mibig_mapper:
+			os.system('rm -rf %s' % gcf_mbm_outdir)
+			cmd = ['lsaBGC-MIBiGMapper.py', '-g', gcf_listing_file, '-m', orthofinder_matrix_file, '-o', gcf_mbm_outdir,
+				   '-i', gcf_id,  '-c', str(cpus)]
+			try:
+				#print(' '.join(cmd))
+				util.run_cmd(cmd, logObject)
+				assert(os.path.isfile(lsabgc_mibigmap_checkpoint))
+			except Exception as e:
+				logObject.warning("lsaBGC-MIBiGMapper.py was unsuccessful for GCF %s" % gcf_id)
+				sys.stderr.write("Warning: lsaBGC-MIBiGMapper.py was unsuccessful for GCF %s\n" % gcf_id)
+
+		# 5. Run lsaBGC-DiscoVary.py
 		if discovary_analysis_id and discovary_input_listing:
 			gcf_dis_outdir = dis_outdir + gcf_id + '/'
 			lsabgc_discovary_checkpoint = gcf_dis_outdir + 'CHECKPOINT.txt'
 			if not os.path.isfile(lsabgc_discovary_checkpoint):
 				os.system('rm -rf %s' % gcf_dis_outdir)
-				os.system('mkdir %s' % gcf_dis_outdir)
 				cmd = ['lsaBGC-DiscoVary.py', '-g', gcf_listing_file, '-m', orthofinder_matrix_file, '-o',
 					   gcf_dis_outdir, '-i', gcf_id, '-c', str(cpus), '-p', discovary_input_listing, '-a',
 					   gcf_pop_outdir + 'Codon_Alignments_Listings.txt', '-l', input_listing_file]
 				try:
 					util.run_cmd(cmd, logObject, stderr=sys.stderr, stdout=sys.stdout)
 					assert (os.path.isfile(lsabgc_discovary_checkpoint))
 				except Exception as e:
@@ -396,46 +429,65 @@
 	combined_tajimd_plot_input_file = outdir + 'Tajimas_D_Plotting_Input.txt'
 	combined_betard_plot_input_file = outdir + 'Beta-RD_Plotting_Input.txt'
 	combined_conser_plot_input_file = outdir + 'HG_Conservation_Plotting_Input.txt'
 	combined_pmcopy_plot_input_file = outdir + 'HG_Proportion_MultiCopy_Plotting_Input.txt'
 	combined_consensus_similarity_file = outdir + 'GCF_Homolog_Group_Consensus_Sequence_Similarity.txt'
 	combined_divergence_results_file = outdir + 'GCF_Divergences.txt'
 	consolidated_popgene_report_file = outdir + 'GCF_Homolog_Group_Information.txt'
+	consolidated_mibig_report_file = outdir + 'Consolidated_MIBiG_Report.txt'
 
 	combined_tajimd_plot_input_handle = open(combined_tajimd_plot_input_file, 'w')
 	combined_betard_plot_input_handle = open(combined_betard_plot_input_file, 'w')
 	combined_pmcopy_plot_input_handle = open(combined_pmcopy_plot_input_file, 'w')
 	combined_conser_plot_input_handle = open(combined_conser_plot_input_file, 'w')
 	combined_consensus_similarity_handle = open(combined_consensus_similarity_file, 'w')
 	combined_orthoresults_unrefined_handle = open(consolidated_popgene_report_file, 'w')
 	combined_divergence_results_handle = open(combined_divergence_results_file, 'w')
+	combined_mibig_handle = open(consolidated_mibig_report_file, 'w')
+
+	if not run_mibig_mapper:
+		combined_mibig_handle.write('Did not request running lsaBGC-MIBiGMapper to map GCFs/homolog grousp to MIBiG.\n')
 
 	combined_tajimd_plot_input_handle.write('\t'.join(['GCF', 'HG', 'start', 'end', 'con_dir', 'proportion', 'core', 'Tajimas_D', 'Single_Copy_in_GCF']) + '\n')
 	combined_betard_plot_input_handle.write('\t'.join(['GCF', 'HG', 'start', 'end', 'con_dir', 'proportion', 'core', 'Beta_RD', 'Single_Copy_in_GCF']) + '\n')
 	combined_conser_plot_input_handle.write('\t'.join(['GCF', 'HG', 'order', 'core', 'population', 'count']) + '\n')
 	combined_pmcopy_plot_input_handle.write('\t'.join(['GCF', 'HG', 'start', 'end', 'con_dir', 'proportion', 'core', 'Prop_Multi_Copy', 'Single_Copy_in_GCF']) + '\n')
 	if sample_retention_set == None:
 		sample_retention_set = all_samples
 
+	gcf_hg_to_mibig_prot = defaultdict(set)
 	hg_gcfs = defaultdict(set)
 	likely_mge_hgs = set([])
 	combined_consensus_similarity_handle.write('\t'.join(['GCF', 'GCF_Order', 'Homolog_Group', 'Homolog_Group_Order', 'label', 'Difference_to_Consensus_Sequence']) + '\n')
 	for i, g in enumerate(os.listdir(gcf_listing_dir)):
 		gcf_id = g.split('.txt')[0]
+
 		gcf_pop_outdir = pop_outdir + gcf_id + '/'
 		gcf_div_outdir = div_outdir + gcf_id + '/'
+		gcf_mib_outdir = mbmap_outdir + gcf_id + '/'
 
 		gcf_pop_results_unrefined = gcf_pop_outdir + 'Homolog_Group_Information.txt'
 		gcf_div_results = gcf_div_outdir + 'Relative_Divergence_Report.txt'
+		gcf_mib_results = gcf_mib_outdir + 'GCF_to_MIBiG_Relations.txt'
 
 		include_header = False
 		if i == 0: include_header = True
 		if os.path.isfile(gcf_pop_results_unrefined): writeToOpenHandle(gcf_pop_results_unrefined, combined_orthoresults_unrefined_handle, include_header)
 		if os.path.isfile(gcf_div_results): writeToOpenHandle(gcf_div_results, combined_divergence_results_handle, include_header)
 
+		if os.path.isfile(gcf_mib_results):
+			with open(gcf_mib_results) as ogmr:
+				for i, line in enumerate(ogmr):
+					line = line.strip()
+					if i == 0 and not include_header:
+						continue
+					ls = line.split('\t')
+					gcf_hg_to_mibig_prot[ls[0] + '|' + ls[2]].add(ls[3])
+					combined_mibig_handle.write(line + '\n')
+
 		hg_data = {}
 		hg_coord_info = []
 		pop_info_available = False
 		with open(gcf_pop_results_unrefined) as ogpru:
 			for j, line in enumerate(ogpru):
 				line = line.strip('\n')
 				ls = line.split('\t')
@@ -515,27 +567,38 @@
 	combined_tajimd_plot_input_handle.close()
 	combined_betard_plot_input_handle.close()
 	combined_pmcopy_plot_input_handle.close()
 	combined_conser_plot_input_handle.close()
 	combined_consensus_similarity_handle.close()
 	combined_orthoresults_unrefined_handle.close()
 	combined_divergence_results_handle.close()
+	combined_mibig_handle.close()
 
 	# Create Final R plots:
 
 	# create big-picture heatmap of presence/sequence-similarity to consensus sequence of homolog groups from each gcf
 	big_picture_heatmap_pdf_file = outdir + 'Consensus_Sequence_Similarity_of_Homolog_Groups.pdf'
 	cmd = ['Rscript', RSCRIPT_FOR_BIGPICTUREHEATMAP, species_phylogeny_file, combined_consensus_similarity_file,
 		   str(population_listing_file), big_picture_heatmap_pdf_file]
 	try:
 		util.run_cmd(cmd, logObject)
 	except Exception as e:
 		logObject.error("Had issues with creating big picture heatmap.")
 		raise RuntimeError("Had issues with creating big picture heatmap.")
 
+	# create big-picture phylo with labels
+	big_picture_phylo_pdf_file = outdir + 'Phylogeny_with_Labels.pdf'
+	cmd = ['Rscript', RSCRIPT_FOR_BIGPICTUREPHYLO, species_phylogeny_file, str(population_listing_file),
+		   big_picture_phylo_pdf_file]
+	try:
+		util.run_cmd(cmd, logObject)
+	except Exception as e:
+		logObject.error("Had issues with creating big picture heatmap.")
+		raise RuntimeError("Had issues with creating big picture heatmap.")
+
 	# create gcf pop gen stats and conservation plots
 	gcf_gene_views_pdf_file = outdir + 'GCF_Conservation_and_PopStats_Views.pdf'
 	cmd = ['Rscript', RSCRIPT_FOR_GCFGENEPLOTS, combined_tajimd_plot_input_file, combined_betard_plot_input_file,
 		   combined_pmcopy_plot_input_file, combined_conser_plot_input_file, gcf_gene_views_pdf_file]
 	try:
 		util.run_cmd(cmd, logObject)
 	except Exception as e:
@@ -575,37 +638,112 @@
 						if i == 0:
 							corason_reference_faa_handle.write('>' + rec.id + '\n' + str(rec.seq) + '\n')
 			except:
 				pass
 	multi_gcf_hgs_handle.close()
 	corason_reference_faa_handle.close()
 
+	if not run_mibig_mapper: gcf_hg_to_mibig_prot = None
+	
 	# create Excel spreadsheet
 	writer = pd.ExcelWriter(outdir + 'lsaBGC_Pan_Secondary_Metabolome_Overview.xlsx', engine='xlsxwriter')
 	workbook = writer.book
 	dd_sheet = workbook.add_worksheet('Data Dictionary')
 	dd_sheet.write(0, 0, 'WARNING: some evolutionary statistics are experimental - evaluate with caution!!!')
 	dd_sheet.write(1, 0, 'Data Dictionary describing columns of "Overview" spreadsheets can be found on lsaBGC\'s Wiki at:')
 	dd_sheet.write(2, 0, 'https://github.com/Kalan-Lab/lsaBGC/wiki/10.-Population-Genetics-Analysis-of-Genes-Found-in-a-GCF#data-dictionary')
 	sl_df = util.loadSamplesIntoPandaDataFrame(input_listing_file, pop_spec_file=population_listing_file)
 	sl_df.to_excel(writer, sheet_name='Samples used in AutoAnalyze', index=False, na_rep="NA")
-	scprf_df = util.loadCustomPopGeneTableInPandaDataFrame(consolidated_popgene_report_file)
+	scprf_df = util.loadCustomPopGeneTableInPandaDataFrame(consolidated_popgene_report_file, mibig_info=gcf_hg_to_mibig_prot)
 	scprf_df.to_excel(writer, sheet_name='Overview - Simple', index=False, na_rep="NA")
 	cprf_df = util.loadTableInPandaDataFrame(multi_gcf_hgs_file)
 	cprf_df.to_excel(writer, sheet_name='Multi-GCF HGs', index=False, na_rep="NA")
 	stg_df = util.loadSampleToGCFIntoPandaDataFrame(gcf_listing_dir)
 	stg_df.to_excel(writer, sheet_name='GCF to Sample Listings', index=False, na_rep="NA")
-	cprf_df = util.loadTableInPandaDataFrame(consolidated_popgene_report_file)
+	if run_mibig_mapper:
+		mibig_df = util.loadTableInPandaDataFrame(consolidated_mibig_report_file)
+		mibig_df.to_excel(writer, sheet_name='GCFs and HGs to MIBiG Mapping', index=False, na_rep="NA")
+	cprf_df = util.loadTableInPandaDataFrame(consolidated_popgene_report_file, mibig_info=gcf_hg_to_mibig_prot)
 	cprf_df.to_excel(writer, sheet_name='Overview - Full', index=False, na_rep="NA")
-	workbook.close()
 
-	# TODO: Add formatting to the Overview - Simple sheet
-	#workbook = writer.book
-	#scprf_sheet = writer.sheets['Overview - Simple']
-	#workbook.close()
+	# format overview simple sheet
+	worksheet = writer.sheets['Overview - Simple']
+	num_rows, num_cols = scprf_df.shape
+
+	warn_format = workbook.add_format({'bg_color': '#bf241f', 'bold': True, 'font_color': '#FFFFFF'})
+	na_format = workbook.add_format({'font_color': '#a6a6a6', 'bg_color': '#FFFFFF', 'italic': True})
+	header_format = workbook.add_format(
+		{'bold': True, 'text_wrap': True, 'valign': 'top', 'fg_color': '#D7E4BC', 'border': 1})
+
+	worksheet.conditional_format('A2:BA' + str(num_rows), {'type': 'cell', 'criteria': '==', 'value': '"NA"', 'format': na_format})
+	worksheet.conditional_format('A1:BA1', {'type': 'cell', 'criteria': '!=', 'value': 'NA', 'format': header_format})
+
+	if run_mibig_mapper:
+		# warn against non-single-copy in GCF context
+		worksheet.conditional_format('I2:I' + str(num_rows), {'type': 'cell', 'criteria': '==', 'value': '"False"', 'format': warn_format})
+
+		# prop gene-clusters with hg
+		worksheet.conditional_format('N2:N' + str(num_rows),
+								 {'type': '2_color_scale', 'min_color': "#f7de99", 'max_color': "#c29006",
+								  "min_value": 0.0, "max_value": 1.0, 'min_type': 'num', 'max_type': 'num'})
+		# gene-lengths
+		worksheet.conditional_format('J2:J' + str(num_rows),
+									 {'type': '2_color_scale', 'min_color': "#a3dee3", 'max_color': "#1ebcc9",
+									  "min_value": 100, "max_value": 2500, 'min_type': 'num', 'max_type': 'num'})
+
+		# taj-d
+		worksheet.conditional_format('P2:P' + str(num_rows),
+									 {'type': '3_color_scale', 'min_color': "#f7a09c", "mid_color": "#e0e0e0",
+									  'min_type': 'num', 'max_type': 'num', 'mid_type': 'num',
+									  'max_color': "#87cefa", "min_value": -2.0, "mid_value": 0.0, "max_value": 2.0})
+
+		# beta-rd
+		worksheet.conditional_format('Q2:Q' + str(num_rows),
+									 {'type': '3_color_scale', 'min_color': "#fac087", "mid_color": "#e0e0e0",
+									  'min_type': 'num', 'max_type': 'num', 'mid_type': 'num',
+									  'max_color': "#9eb888", "min_value": 0.75, "mid_value": 1.0, "max_value": 1.25})
+
+		# max beta-rd gc
+		worksheet.conditional_format('R2:R' + str(num_rows),
+									 {'type': '3_color_scale', 'min_color': "#fac087", "mid_color": "#e0e0e0",
+									  'min_type': 'num', 'max_type': 'num', 'mid_type': 'num',
+									  'max_color': "#9eb888", "min_value": 0.75, "mid_value": 1.0, "max_value": 1.25})
+
+	else:
+		# warn against non-single-copy in GCF context
+		worksheet.conditional_format('H2:H' + str(num_rows), {'type': 'cell', 'criteria': '==', 'value': '"False"', 'format': warn_format})
+
+		# prop gene-clusters with hg
+		worksheet.conditional_format('M2:M' + str(num_rows),
+								 {'type': '2_color_scale', 'min_color': "#f7de99", 'max_color': "#c29006",
+								  "min_value": 0.0, "max_value": 1.0, 'min_type': 'num', 'max_type': 'num'})
+		# gene-lengths
+		worksheet.conditional_format('I2:I' + str(num_rows),
+									 {'type': '2_color_scale', 'min_color': "#a3dee3", 'max_color': "#1ebcc9",
+									  "min_value": 100, "max_value": 2500, 'min_type': 'num', 'max_type': 'num'})
+
+		# taj-d
+		worksheet.conditional_format('O2:O' + str(num_rows),
+									 {'type': '3_color_scale', 'min_color': "#f7a09c", "mid_color": "#e0e0e0",
+									  'min_type': 'num', 'max_type': 'num', 'mid_type': 'num',
+									  'max_color': "#87cefa", "min_value": -2.0, "mid_value": 0.0, "max_value": 2.0})
+
+		# beta-rd
+		worksheet.conditional_format('P2:P' + str(num_rows),
+									 {'type': '3_color_scale', 'min_color': "#fac087", "mid_color": "#e0e0e0",
+									  'min_type': 'num', 'max_type': 'num', 'mid_type': 'num',
+									  'max_color': "#9eb888", "min_value": 0.75, "mid_value": 1.0, "max_value": 1.25})
+
+		# max beta-rd gc
+		worksheet.conditional_format('Q2:Q' + str(num_rows),
+									 {'type': '3_color_scale', 'min_color': "#fac087", "mid_color": "#e0e0e0",
+									  'min_type': 'num', 'max_type': 'num', 'mid_type': 'num',
+									  'max_color': "#9eb888", "min_value": 0.75, "mid_value": 1.0, "max_value": 1.25})
+
+	workbook.close()
 
 	# clean up final directory:
 	final_results_dir = outdir + 'Final_Results/'
 	inter_results_dir = outdir + 'Intermediate_Results/'
 	util.setupReadyDirectory([final_results_dir, inter_results_dir])
 	for fd in os.listdir(outdir):
 		if os.path.isdir(fd): continue
@@ -630,8 +768,8 @@
 		for i, line in enumerate(ogrf):
 			if i == 0 and include_header:
 				combined_results_handle.write(line)
 			elif i != 0:
 				combined_results_handle.write(line)
 
 if __name__ == '__main__':
-	lsaBGC_AutoAnalyze()
+	lsaBGC_AutoAnalyze()
```

### Comparing `lsaBGC-1.33/workflows/lsaBGC-AutoExpansion.py` & `lsaBGC-1.34/workflows/lsaBGC-AutoExpansion.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,27 +60,26 @@
 
 	Program to run lsaBGC-Expansion on each GCF, resolve conflicts across GCFs, and then consolidate result files when
 	overlapping BGC predictions for different GCFs exist.
 	""", formatter_class=argparse.RawTextHelpFormatter)
 
 	parser.add_argument('-g', '--gcf_listing_dir', help='Directory with GCF listing files.', required=True)
 	parser.add_argument('-m', '--orthofinder_matrix', help="OrthoFinder homolog group by sample matrix.", required=True)
-	parser.add_argument('-l', '--initial_listing', type=str, help="Path to tab delimited text file for samples with three columns: (1) sample name (2) Prokka generated Genbank file (*.gbk), and (3) Prokka generated predicted-proteome file (*.faa). Please remove troublesome characters in the sample name.", required=True)
-	parser.add_argument('-e', '--expansion_listing', help="Path to tab delimited file listing: (1) sample name (2) path to Prokka Genbank and (3) path to Prokka predicted proteome. This file is produced by lsaBGC-AutoProcess.py.", required=True)
+	parser.add_argument('-l', '--initial_listing', type=str, help="Path to tab delimited text file for samples with three columns: (1) sample\nname (2) Prokka generated Genbank file (*.gbk), and (3) Prokka generated predicted-proteome file\n(*.faa). Please remove troublesome characters in the sample name.", required=True)
+	parser.add_argument('-e', '--expansion_listing', help="Path to tab delimited file listing: (1) sample name (2) path to Prokka Genbank and\n(3) path to Prokka predicted proteome. This file is produced by\nlsaBGC-AutoProcess.py.", required=True)
 	parser.add_argument('-o', '--output_directory', help="Parent output/workspace directory.", required=True)
-	parser.add_argument('-p', '--bgc_prediction_software', help='Software used to predict BGCs (Options: antiSMASH, DeepBGC, GECCO).\nDefault is antiSMASH.', default='antiSMASH', required=False)
+	parser.add_argument('-p', '--bgc_prediction_software', help='Software used to predict BGCs (Options: antiSMASH, DeepBGC, GECCO)\n[Default is antiSMASH].', default='antiSMASH', required=False)
 	parser.add_argument('-q', '--quick_mode', action='store_true', help='Whether to run lsaBGC-Expansion in quick mode?', required=False, default=False)
 	parser.add_argument('-z', '--pickle_expansion_annotation_data', help="Pickle file with serialization of annotation data in the expansion listing file.", required=False, default=None)
-	parser.add_argument('-c', '--cpus', type=int, help="Total number of cpus to use.", required=False, default=1)
 	parser.add_argument('-ph', '--protocore_homologs', help="File with manual listings of proto-core homolog groups.\nThis should be provided as 2 column tab-delmited file: (1) GCF id and\n(2) space delmited listing of homolog groups.", required=False, default=None)
+	parser.add_argument('-c', '--cpus', type=int, help="Total number of CPUs to use [Default is 1].", required=False, default=1)
 
 	args = parser.parse_args()
 	return args
 
-
 def lsaBGC_AutoExpansion():
 	"""
 	Void function which runs primary workflow for program.
 	"""
 
 	"""
 	PARSE REQUIRED INPUTS
@@ -146,15 +145,15 @@
 						pickle_expansion_annotation_data_file, quick_mode, bgc_prediction_software,
 						protocore_homologs_file, cpus]
 	parameter_names = ["GCF Listings Directory", "Listing File of Prokka Annotation Files for Initial Set of Samples",
 					   "Listing File of Prokka Annotation Files for Expansion/Additional Set of Samples",
 					   "OrthoFinder Homolog Matrix", "Output Directory",
 					   "Pickle File with Annotation Data in Expansion Listing for Quick Loading",
 					   "Run in Quick Mode?", "BGC Prediction Software", "ProtoCore-Like Homolog Group Specifications",
-					   "cpus"]
+					   "CPUs"]
 	util.logParametersToFile(parameters_file, parameter_names, parameter_values)
 	logObject.info("Done saving parameters!")
 
 	# parse manual proto-core homolog group specifications if provided
 	protocore_hgs = None
 	if protocore_homologs_file != None:
 		protocore_hgs = {}
```

### Comparing `lsaBGC-1.33/workflows/lsaBGC-Easy.py` & `lsaBGC-1.34/workflows/lsaBGC-Easy.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,126 +58,96 @@
 	""" Parse arguments """
 	parser = argparse.ArgumentParser(description="""
 	   __              ___   _____  _____
 	  / /  ___ ___ _  / _ ) / ___/ / ___/
 	 / /  (_-</ _ `/ / _  |/ (_ / / /__  
 	/_/  /___/\_,_/ /____/ \___/  \___/  
 	*******************************************************************************************************************
-	Program: lsaBGC-Easy.py (Version 1.31)
+	Program: lsaBGC-Easy.py
 	Author: Rauf Salamzade
 	Affiliation: Kalan Lab, UW Madison, Department of Medical Microbiology and Immunology
 	
-	QUICK DESCRIPTION: 
+	QUICK DESCRIPTION:
 	Workflow to run the majority of lsaBGC functionalities for a specific taxa or manually defined set of user-provided
 	genomes or both. For information on the workflow and examples on how to run please take a look at the Wiki:
-	https://github.com/Kalan-Lab/lsaBGC/wiki/14.-lsaBGC-Easy-Tutorial:-Combining-lsaBGC-with-ncbi-genome-download
+	https://github.com/Kalan-Lab/lsaBGC/wiki/14.-lsaBGC-Easy-Tutorial
 		
-	Currently only works for bacteria, but lsaBGC can handle fungi now - just not lsaBGC-Easy ... yet
+	If interested in fungal investigation please check out lsaBGC-Euk-Easy.py.
 	*******************************************************************************************************************
 	CONSIDERATIONS:	
 	* Check out the considerations wiki page: https://github.com/Kalan-Lab/lsaBGC/wiki/00.-Background-&-Considerations  	
 	* If interested in running just a directory of genomes (you don't want to downoad genomes from Genbank for some taxa)
 	  then you can just set the required -n argument to "None".
 	*******************************************************************************************************************
 	OVERVIEW OF STEPS TAKEN:	
 		- Check number of genomes for taxa is not too crazy (<1000) or too small (>10)
 		- Step 1: Get set of Genbank assembly accessions from recent GTDB release matching taxa.
 		- Step 2: Download all genomes in FASTA format using ncbi-genome-download and perform gene-calling with prodigal.
 		- Step 3: Run GToTree, Dereplicate, Group Samples into Populations/Clades, and Create genomes listing
-		- Step 4: Run GECCO based annotation of BGCs and crete BGC listing or Create Task File with antiSMASH/DeepBGC coomands
+		- Step 4: Run GECCO based annotation of BGCs and crete BGC listing or Create Task File with antiSMASH/DeepBGC commands
 		- Step 5: Run lsaBGC-Ready.py with lsaBGC-Cluster or BiG-SCAPE
 		- Step 6: Run lsaBGC-AutoExpansion.py polishing to find GCF instances fragmented on multiple scaffolds
 		- Step 7: Run lsaBGC-AutoAnalyze.py
+		- Step 8: Run GSeeF.py
 	*******************************************************************************************************************
-	AVAILBLE SCG MODELS IN GTOTREE:
-           Actinobacteria                    (138 genes)
-           Alphaproteobacteria               (117 genes)
-           Archaea                            (76 genes)
-           Bacteria                           (74 genes)
-           Bacteria_and_Archaea               (25 genes)
-           Bacteroidetes                      (90 genes)
-           Betaproteobacteria                (203 genes)
-           Chlamydiae                        (286 genes)
-           Cyanobacteria                     (251 genes)
-           Epsilonproteobacteria             (260 genes)
-           Firmicutes                        (119 genes)
-           Gammaproteobacteria               (172 genes)
-           Proteobacteria                    (119 genes)
-           Tenericutes                        (99 genes)
-           Universal_Hug_et_al                (16 genes)
+	GToTree taxa models available (more resolute taxonomic groups will have more genes to use for building phylogeny):
+	(1) Actinobacteria, (2) Alphaproteobacteria, (3) Archaea, (4) Bacteria, (5) Bacteria_and_Archaea, 
+ 	(6) Betaproteobacteria, (7) Chlamydiae, (8) Cyanobacteria, (9) Epsilonproteobacteria, (10) Firmicutes, 
+ 	(11) Firmicutes, (12) Gammaproteobacteria, (13) Proteobacteria, (14) Tenericutes, (15) Universal_Hug_et_al
+ 	*******************************************************************************************************************
 	""", formatter_class=argparse.RawTextHelpFormatter)
 
-	parser.add_argument('-n', '--taxa_name',
-						help='Name of the taxa of interest as listed in GTDB. Currently restricted to bacteria - but lsaBGC\nitself- when using antiSMASH BGC predictions can run on\nEuks - check out the tutorial!! If there is a space in the\nname, please surround by quotes.',
-						required=True)
+	parser.add_argument('-n', '--taxa_name', help='Name of the taxa of interest as listed in GTDB. If there is a space in the\nname, please surround by quotes.', required=True)
+	parser.add_argument('-g', '--user_genomes_directory', help='A directory with additional genomes, e.g. those recently sequenced by the\nuser, belonging to the taxa. Accepted formats include FASTA.\nAccepted suffices include: .fna, .fa, .fasta.', required=False, default=None)
 	parser.add_argument('-o', '--output_directory', help='Parent output/workspace directory.', required=True)
-	parser.add_argument('-g', '--user_genomes_directory',
-						help='A directory with additional genomes, e.g. those recently sequenced by the\nuser, belonging to the taxa. Accepted formats include FASTA.\nAccepted suffices include: .fna, .fa, .fasta.',
-						required=False, default=None)
-	parser.add_argument('-p', '--bgc_prediction_software',
-						help='Software used to predict BGCs (Options: antiSMASH, DeepBGC, GECCO).\nDefault is GECCO - which will be automatic. For the other two,\nlsaBGC-Easy will produce a task-file which you will need to run in a seperate environment\nwith antiSMASH or DeepBGC installed, then rerun lsaBGC-Easy.py using the original command..',
-						default='gecco', required=False)
-	parser.add_argument('-om', '--orthofinder_mode',
-						help="Method for running OrthoFinder2. (Options: Genome_Wide, BGC_Only).\nDefault is Genome_Wide (BGC_Only is slightly experimental but much faster and should work\nespecially well for taxa with many BGCs).",
-						default='Genome_Wide', required=False)
-	parser.add_argument('-sd', '--skip_dereplication', action='store_true',
-						help="Whether to skip dereplication based on GToTree alignments of SCGs - not\nrecommended and can cause issues if there are a lot of\ngenomes for the taxa of interest.",
-						default=False, required=False)
-	parser.add_argument('-gtm', '--gtotree_model',
-						help="SCG model for secondary GToTree analysis and wdhat would be used for dereplication. Default is to use the \"Bacteria\" SCG set (n=74 genes).",
-						default='Bacteria', required=False)
-	parser.add_argument('-iib', '--include_incomplete_bgcs', action='store_true',
-						help="Whether to account for incomplete BGCs prior to clustering - not recommended.",
-						default=False, required=False)
-	parser.add_argument('-mc', '--run_coarse_orthofinder', action='store_true',
-						help='Use coarse clustering of homolog groups in OrthoFinder instead of more\nresolute hierarchical determined homolog groups. There are some advantages to coarse OGs, including their construction being deterministic.',
-						required=False, default=False)
-	parser.add_argument('-b', '--use_bigscape', action='store_true',
-						help="Use BiG-SCAPE for BGC clustering into GCFs instead of lsaBGC-Cluster. Recommended if you want to include incomplete BGCs for clustering and are using antiSMASH.",
-						required=False, default=False)
-	parser.add_argument('-sae', '--skip_auto_expansion', action='store_true',
-						help="Skip lsaBGC-AutoExpansion.py to find missing pieces of BGCs due to assembly fragmentation.",
-						required=False, default=False)
-	parser.add_argument('-c', '--cpus', type=int,
-						help="Total number of cpus/threads. Note, this is the total number of\nthreads to use (Default is 4). BGC prediction commands (via GECCO, antiSMASH, and DeepBGC) will\neach be set to use 4 cpus by default.",
-						required=False, default=4)
-	parser.add_argument('-dt', '--dereplicate_threshold', type=float,
-						help="Amino acid similarity threshold of SCGs for considering\ntwo genomes as redundant. (Default is 0.999)",
-						default=0.999, required=False)
-	parser.add_argument('-pt', '--population_threshold', type=float,
-						help="Amino acid similarity threshold of SCGs for considering\ntwo genomes as belonging to the same population. (Default is 0.99)",
-						default=0.99, required=False)
-	parser.add_argument('-x', '--ignore_limits', action='store_true',
-						help="Ignore limitations on number of genomes allowed.\nE.g. allow for analyses of taxa with more than 2000 genomes available and more than 100 genomes\nafter dereplication. Not recommend, be cautious!!! Also note,\nyou can always delete \"Dereplicated_Set_of_Genomes.txt\" in the results directory and redo\ndereplication with different threshold.")
-	parser.add_argument('-py', '--use_pyrodigal', action='store_true', help='Use pyrodigal instead of prodigal.',
-						required=False, default=False)
+	parser.add_argument('-p', '--bgc_prediction_software', help='Software used to predict BGCs (Options: antiSMASH, DeepBGC, GECCO). GECCO is\nautomatic, but for the other two, lsaBGC-Easy will produce a task-file which you will need to run in a\nseperate environment with antiSMASH or DeepBGC installed, then rerun lsaBGC-Easy.py using the\noriginal command [Default is GECCO].', default='gecco', required=False)
+	parser.add_argument('-x', '--ignore_limits', action='store_true', help="Ignore limitations on number of genomes allowed.\nE.g. allow for analyses of taxa with more than 2000 genomes available and more than 100 genomes\nafter dereplication. Not recommend, be cautious!!! Also note,\nyou can always delete \"Dereplicated_Set_of_Genomes.txt\" in the results directory and redo\ndereplication with different threshold.")
+	parser.add_argument('-gtm', '--gtotree_model', help="SCG model for secondary GToTree analysis and what would be used for dereplication. [Default is \"Bacteria\"].", default='Bacteria', required=False)
+	parser.add_argument('-iib', '--include_incomplete_bgcs', action='store_true', help="Whether to account for incomplete BGCs (those near contig edges) prior to clustering.", default=False, required=False)
+	parser.add_argument('-b', '--use_bigscape', action='store_true', help="Use BiG-SCAPE for BGC clustering into GCFs instead of lsaBGC-Cluster. Recommended if\nyou want to include incomplete BGCs for clustering and are using antiSMASH.", required=False, default=False)
+	parser.add_argument('-lci', '--lsabgc_cluster_inflation', type=float, help='Value for MCL inflation parameter to use in lsaBGC-Cluster [Default is 4.0].', required=False, default=4.0)
+	parser.add_argument('-lcj', '--lsabgc_cluster_jaccard', type=float, help='Minimal Jaccard Index cutoff to regard two BGCs as potentially homologous\nin lsaBGC-Cluster [Default is 20.0].', required=False, default=20.0)
+	parser.add_argument('-lcr', '--lsabgc_cluster_synteny', type=float, help='Minimal absolute correlation coefficient to measure syntenic similarity and\nregard two BGCs as potentially homologous in lsaBGC-Cluster [Default is 0.7].', required=False, default=0.7)
+	parser.add_argument('-sae', '--skip_auto_expansion', action='store_true', help="Skip lsaBGC-AutoExpansion.py to find missing pieces of BGCs due to assembly fragmentation.", required=False, default=False)
+	parser.add_argument('-sd', '--skip_dereplication', action='store_true', help="Whether to skip dereplication based on GToTree alignments of SCGs - not\nrecommended and can cause issues if there are a lot of\ngenomes for the taxa of interest.", default=False, required=False)
+	parser.add_argument('-dt', '--dereplicate_threshold', type=float, help="Amino acid similarity threshold of SCGs for considering\ntwo genomes as redundant [Default is 0.999].", default=0.999, required=False)
+	parser.add_argument('-pt', '--population_threshold', type=float, help="Amino acid similarity threshold of SCGs for considering\ntwo genomes as belonging to the same population [Default is 0.99].", default=0.99, required=False)
+	parser.add_argument('-py', '--use_pyrodigal', action='store_true', help='Use pyrodigal instead of prodigal.', required=False, default=False)
+	parser.add_argument('-om', '--orthofinder_mode', help="Method for running OrthoFinder2. (Options: Genome_Wide, BGC_Only).\nBGC_Only is experimental but much faster and should work especially well for\ntaxa with many BGCs [Default is Genome_Wide].", default='Genome_Wide', required=False)
+	parser.add_argument('-mc', '--run_coarse_orthofinder', action='store_true', help='Use coarse clustering of homolog groups in OrthoFinder instead of more\nresolute hierarchical determined homolog groups. There are some advantages to coarse\nOGs, including their construction being deterministic.', required=False, default=False)
+	parser.add_argument('-c', '--cpus', type=int, help="Total number of CPUs to use [Default is 4].", required=False, default=4)
+	parser.add_argument('-a', '--antismash_prediction_cpus', type=int, help="Number of CPUs to specify for each antiSMASH command in\ntask file [Default is 4].", required=False, default=4)
 
 	args = parser.parse_args()
 	return args
 
 
 def lsaBGC_Easy():
 	myargs = create_parser()
 
 	taxa_name = myargs.taxa_name.strip('"').strip()
 	outdir = os.path.abspath(myargs.output_directory) + '/'
 	cpus = myargs.cpus
+	bgc_prediction_cpus = myargs.antismash_prediction_cpus
 	user_genomes_directory = myargs.user_genomes_directory
 	bgc_prediction_software = myargs.bgc_prediction_software.upper()
 	gtotree_model = myargs.gtotree_model
 	skip_dereplication_flag = myargs.skip_dereplication
 	include_incomplete_bgcs_flag = myargs.include_incomplete_bgcs
 	skip_auto_expansion_flag = myargs.skip_auto_expansion
 	dereplicate_threshold = myargs.dereplicate_threshold
 	population_threshold = myargs.population_threshold
 	run_coarse_orthofinder = myargs.run_coarse_orthofinder
 	orthofinder_mode = myargs.orthofinder_mode.upper()
 	use_bigscape_flag = myargs.use_bigscape
 	ignore_limits_flag = myargs.ignore_limits
 	use_pyrodigal = myargs.use_pyrodigal
+	lsabgc_cluster_inflation = myargs.lsabgc_cluster_inflation
+	lsabgc_cluster_jaccard = myargs.lsabgc_cluster_jaccard
+	lsabgc_cluster_synteny = myargs.lsabgc_cluster_synteny
 
 	try:
 		assert (orthofinder_mode in set(['GENOME_WIDE', 'BGC_ONLY']))
 	except:
 		sys.stderr.write('BGC prediction software option is not a valid option.\n')
 		sys.exit(1)
 	try:
@@ -552,16 +522,17 @@
 					gecco_cmd = ['gecco', 'run', '-j', '4', '-o', primary_bgc_pred_directory + s + '/', '-g',
 								 all_genome_listings_fna[s]]
 					if not include_incomplete_bgcs_flag:
 						gecco_cmd += ['-E', '10']
 					gecco_cmd += [logObject]
 					primary_bgc_pred_cmds.append(gecco_cmd)
 				if bgc_prediction_software == 'ANTISMASH':
-					antismash_cmd = ['antismash', '--output-dir', primary_bgc_pred_directory + s + '/', '-c', '4',
-									 '--genefinding-tool', 'none', '--output-basename', s, all_genome_listings_gbk[s]]
+					antismash_cmd = ['antismash', '--output-dir', primary_bgc_pred_directory + s + '/', '-c',
+									 str(bgc_prediction_cpus), '--genefinding-tool', 'none', '--output-basename', s,
+									 all_genome_listings_gbk[s]]
 					primary_bgc_pred_cmds.append(antismash_cmd)
 				elif bgc_prediction_software == 'DEEPBGC':
 					deepbgc_cmd = ['deepbgc', 'pipeline', '--output', primary_bgc_pred_directory + s + '/',
 								   all_genome_listings_fna[s]]
 					primary_bgc_pred_cmds.append(deepbgc_cmd)
 		primary_genomes_listing_handle.close()
 
@@ -572,15 +543,15 @@
 			p.close()
 		else:
 			cmd_handle = open(cmd_file, 'w')
 			for cmd in primary_bgc_pred_cmds:
 				cmd_handle.write(' '.join(cmd) + '\n')
 			cmd_handle.close()
 			logObject.info(
-				'%s BGC prediction commands written to %s.Please run these and afterwards restart lsaBGC-Easy.py with the same command afterwards.' % (
+				'%s BGC prediction commands written to %s.Please run these and afterwards restart lsaBGC-Easy.py with the same command as used initially.' % (
 				bgc_prediction_software, cmd_file))
 			sys.stdout.write(
 				'************************\nPlease run the following BGC prediction commands using a different conda envirnoment with the BGC prediction\nsoftware (%s) installed and afterwards restart lsaBGC-Easy.py with the same command as used initially.\nExiting now, see you back soon, here is the task file with the %s commands:\n%s\n' % (
 				bgc_prediction_software, bgc_prediction_software, cmd_file))
 			sys.exit(0)
 
 	bgc_prediciton_count = 0
@@ -637,15 +608,16 @@
 		lsabgc_ready_cmd = ['lsaBGC-Ready.py', '-i', primary_genomes_listing_file, '-l', primary_bgcs_listing_file,
 							'-o', lsabgc_ready_directory, '-c', str(cpus), '-p', bgc_prediction_software,
 							'-m', orthofinder_mode]
 
 		if use_bigscape_flag and os.path.isdir(bigscape_results_dir):
 			lsabgc_ready_cmd += ['-b', bigscape_results_dir]
 		else:
-			lsabgc_ready_cmd += ['-lc']
+			lsabgc_ready_cmd += ['-lc', '-lci', str(lsabgc_cluster_inflation), '-lcj', str(lsabgc_cluster_jaccard),
+								 '-lcr', str(lsabgc_cluster_synteny)]
 		if use_pyrodigal:
 			lsabgc_ready_cmd += ['-py']
 		if run_coarse_orthofinder:
 			lsabgc_ready_cmd += ['-mc']
 
 		db_listing_file = lsaBGC_main_directory + '/db/database_location_paths.txt'
 		if os.path.isfile(db_listing_file):
@@ -676,37 +648,39 @@
 
 	if skip_auto_expansion_flag:
 		exp_annotation_listing_file = annotation_listing_file
 		exp_orthogroups_matrix_file = orthogroups_matrix_file
 		exp_gcf_listing_dir = gcf_listing_dir
 
 	# Step 7: Run lsaBGC-AutoAnalyze.py
-	logObject.info('\n--------------------\nStep 7\n--------------------\nBeginning lsaBGC-AutoExpansion (which runs lsaBGC-See.py, lsaBGC-PopGene.py, and lsaBGC-Divergence.py + summarizes results across GCFs at the end.\n')
-	sys.stdout.write('--------------------\nStep 7\n--------------------\nBeginning lsaBGC-AutoExpansion (which runs lsaBGC-See.py, lsaBGC-PopGene.py,\nand lsaBGC-Divergence.py + summarizes results across GCFs at the end.\n')
+	logObject.info('\n--------------------\nStep 7\n--------------------\nBeginning lsaBGC-AutoAnalyze (which runs lsaBGC-See.py, lsaBGC-PopGene.py, and lsaBGC-Divergence.py + summarizes results across GCFs at the end.\n')
+	sys.stdout.write('--------------------\nStep 7\n--------------------\nBeginning lsaBGC-AutoAnalyze (which runs lsaBGC-See.py, lsaBGC-PopGene.py,\nand lsaBGC-Divergence.py + summarizes results across GCFs at the end.\n')
 
 	checkLsaBGCInputsExist(exp_annotation_listing_file, exp_gcf_listing_dir, exp_orthogroups_matrix_file)
 	try:
 		assert (os.path.isfile(species_tree_file) and os.path.isfile(expected_similarities_file) and os.path.isfile(
 			samples_to_keep_file))
 	except:
 		raise RuntimeError("Issue validating GToTree construction in lsaBGC-Ready was successful.")
 
 	lsabgc_autoanalyze_dir = outdir + 'lsaBGC_AutoAnalyze_Results/'
 	lsabgc_autoanalyze_results_dir = lsabgc_autoanalyze_dir + 'Final_Results/'
 	if not os.path.isdir(lsabgc_autoanalyze_results_dir):
 		os.system('rm -rf %s' % lsabgc_autoanalyze_dir)
 		lsabgc_autoanalyze_cmd = ['lsaBGC-AutoAnalyze.py', '-i', exp_annotation_listing_file, '-g', exp_gcf_listing_dir,
-								  '-m',
-								  exp_orthogroups_matrix_file, '-s', species_tree_file, '-w',
-								  expected_similarities_file, '-k',
-								  samples_to_keep_file, '-c', str(cpus), '-o', lsabgc_autoanalyze_dir, '-p',
-								  bgc_prediction_software, '-u', population_file]
+								  '-mb', '-m', exp_orthogroups_matrix_file, '-s', species_tree_file, '-w',
+								  expected_similarities_file, '-k', samples_to_keep_file, '-c', str(cpus), '-o',
+								  lsabgc_autoanalyze_dir, '-p', bgc_prediction_software, '-u', population_file]
 		runCmdViaSubprocess(lsabgc_autoanalyze_cmd, logObject, check_directories=[lsabgc_autoanalyze_results_dir])
 
 
+	# Step 8: Run lsaBGC-AutoAnalyze.py
+	logObject.info('\n--------------------\nStep 8\n--------------------\nBeginning GSeeF analysis.')
+	sys.stdout.write('--------------------\nStep 8\n--------------------\nBeginning GSeeF analysis.')
+
 	gseef_results_dir = outdir + 'GSeeF_Results/'
 	gseef_final_results_dir = gseef_results_dir + 'Final_Results/'
 	if not os.path.isdir(gseef_results_dir):
 		os.system('rm -rf %s' % gseef_results_dir)
 
 		pruned_species_tree_file = outdir + 'Species_Tree.pruned.tre'
 		try:
```

