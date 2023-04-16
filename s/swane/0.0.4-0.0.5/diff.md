# Comparing `tmp/swane-0.0.4.tar.gz` & `tmp/swane-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swane-0.0.4.tar", last modified: Tue Apr 11 08:24:09 2023, max compression
+gzip compressed data, was "swane-0.0.5.tar", last modified: Sun Apr 16 17:02:37 2023, max compression
```

## Comparing `swane-0.0.4.tar` & `swane-0.0.5.tar`

### file list

```diff
@@ -1,90 +1,91 @@
-drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-04-11 08:24:09.752565 swane-0.0.4/
--rw-rw-r--   0 mau       (1000) mau       (1000)     1976 2023-03-29 17:07:54.000000 swane-0.0.4/LICENSE
--rw-rw-r--   0 mau       (1000) mau       (1000)      184 2023-03-29 17:07:54.000000 swane-0.0.4/MANIFEST.in
--rw-rw-r--   0 mau       (1000) mau       (1000)      427 2023-04-11 08:24:09.752565 swane-0.0.4/PKG-INFO
--rw-rw-r--   0 mau       (1000) mau       (1000)        0 2023-03-29 17:07:54.000000 swane-0.0.4/README.md
--rw-rw-r--   0 mau       (1000) mau       (1000)       38 2023-04-11 08:24:09.752565 swane-0.0.4/setup.cfg
--rw-rw-r--   0 mau       (1000) mau       (1000)     1202 2023-04-11 08:22:48.000000 swane-0.0.4/setup.py
-drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-04-11 08:24:09.744566 swane-0.0.4/swane/
--rw-rw-r--   0 mau       (1000) mau       (1000)       50 2023-04-05 07:58:56.000000 swane-0.0.4/swane/__init__.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     1827 2023-03-29 17:07:54.000000 swane-0.0.4/swane/__main__.py
-drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-04-11 08:24:09.744566 swane-0.0.4/swane/nipype_pipeline/
--rw-rw-r--   0 mau       (1000) mau       (1000)    18398 2023-03-30 15:50:36.000000 swane-0.0.4/swane/nipype_pipeline/MainWorkflow.py
--rw-rw-r--   0 mau       (1000) mau       (1000)        0 2023-03-29 17:07:54.000000 swane-0.0.4/swane/nipype_pipeline/__init__.py
-drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-04-11 08:24:09.744566 swane-0.0.4/swane/nipype_pipeline/engine/
--rw-rw-r--   0 mau       (1000) mau       (1000)     7906 2023-04-06 16:01:54.000000 swane-0.0.4/swane/nipype_pipeline/engine/CustomWorkflow.py
--rw-rw-r--   0 mau       (1000) mau       (1000)      405 2023-04-06 16:01:54.000000 swane-0.0.4/swane/nipype_pipeline/engine/NodeListEntry.py
--rw-rw-r--   0 mau       (1000) mau       (1000)        0 2023-03-29 17:07:54.000000 swane-0.0.4/swane/nipype_pipeline/engine/__init__.py
-drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-04-11 08:24:09.748566 swane-0.0.4/swane/nipype_pipeline/nodes/
--rw-rw-r--   0 mau       (1000) mau       (1000)     2537 2023-04-06 16:01:54.000000 swane-0.0.4/swane/nipype_pipeline/nodes/AsymmetryIndex.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     2263 2023-04-06 16:01:54.000000 swane-0.0.4/swane/nipype_pipeline/nodes/CustomBEDPOSTX5.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     1245 2023-04-06 16:01:54.000000 swane-0.0.4/swane/nipype_pipeline/nodes/CustomDcm2niix.py
--rw-rw-r--   0 mau       (1000) mau       (1000)      489 2023-04-06 16:01:54.000000 swane-0.0.4/swane/nipype_pipeline/nodes/CustomDilateImage.py
--rw-rw-r--   0 mau       (1000) mau       (1000)      661 2023-04-06 16:01:54.000000 swane-0.0.4/swane/nipype_pipeline/nodes/CustomLabel2Vol.py
--rw-rw-r--   0 mau       (1000) mau       (1000)      923 2023-04-06 16:01:54.000000 swane-0.0.4/swane/nipype_pipeline/nodes/CustomProbTrackX2.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     2356 2023-04-06 16:01:54.000000 swane-0.0.4/swane/nipype_pipeline/nodes/CustomSliceTimer.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     2737 2023-04-06 16:01:54.000000 swane-0.0.4/swane/nipype_pipeline/nodes/DOmapOutliersMask.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     2437 2023-04-06 16:01:54.000000 swane-0.0.4/swane/nipype_pipeline/nodes/DeleteVolumes.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     4520 2023-04-06 16:01:54.000000 swane-0.0.4/swane/nipype_pipeline/nodes/FMRIGenSpec.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     2506 2023-04-06 16:01:54.000000 swane-0.0.4/swane/nipype_pipeline/nodes/ForceOrient.py
--rw-rw-r--   0 mau       (1000) mau       (1000)      458 2023-04-06 16:01:54.000000 swane-0.0.4/swane/nipype_pipeline/nodes/FslCluster.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     1600 2023-04-06 16:01:54.000000 swane-0.0.4/swane/nipype_pipeline/nodes/FslNVols.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     1601 2023-04-06 16:01:54.000000 swane-0.0.4/swane/nipype_pipeline/nodes/GetNiftiTR.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     1650 2023-04-06 16:01:54.000000 swane-0.0.4/swane/nipype_pipeline/nodes/MergeTargets.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     1849 2023-04-06 16:01:54.000000 swane-0.0.4/swane/nipype_pipeline/nodes/Orient.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     1400 2023-04-06 16:01:54.000000 swane-0.0.4/swane/nipype_pipeline/nodes/RandomSeedGenerator.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     2741 2023-04-06 16:01:54.000000 swane-0.0.4/swane/nipype_pipeline/nodes/SegmentHA.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     3247 2023-04-06 16:01:54.000000 swane-0.0.4/swane/nipype_pipeline/nodes/SumMultiTracks.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     3025 2023-04-06 16:01:54.000000 swane-0.0.4/swane/nipype_pipeline/nodes/ThrROI.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     2378 2023-04-06 16:01:54.000000 swane-0.0.4/swane/nipype_pipeline/nodes/VenousCheck.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     2703 2023-04-06 16:01:54.000000 swane-0.0.4/swane/nipype_pipeline/nodes/Zscore.py
--rw-rw-r--   0 mau       (1000) mau       (1000)       25 2023-03-29 17:07:54.000000 swane-0.0.4/swane/nipype_pipeline/nodes/__init__.py
--rw-rw-r--   0 mau       (1000) mau       (1000)      178 2023-04-06 16:01:54.000000 swane-0.0.4/swane/nipype_pipeline/nodes/utils.py
-drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-04-11 08:24:09.748566 swane-0.0.4/swane/nipype_pipeline/workflows/
--rw-rw-r--   0 mau       (1000) mau       (1000)        0 2023-03-29 17:07:54.000000 swane-0.0.4/swane/nipype_pipeline/workflows/__init__.py
--rw-rw-r--   0 mau       (1000) mau       (1000)    13690 2023-03-31 12:25:20.000000 swane-0.0.4/swane/nipype_pipeline/workflows/domap_workflow.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     7922 2023-04-04 03:17:58.000000 swane-0.0.4/swane/nipype_pipeline/workflows/dti_preproc_workflow.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     7690 2023-04-01 08:02:25.000000 swane-0.0.4/swane/nipype_pipeline/workflows/freesurfer_workflow.py
--rw-rw-r--   0 mau       (1000) mau       (1000)    10956 2023-04-04 03:17:58.000000 swane-0.0.4/swane/nipype_pipeline/workflows/func_map_workflow.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     3504 2023-04-02 08:01:53.000000 swane-0.0.4/swane/nipype_pipeline/workflows/linear_reg_workflow.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     3142 2023-03-29 20:08:41.000000 swane-0.0.4/swane/nipype_pipeline/workflows/nonlinear_reg_workflow.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     2180 2023-04-02 07:46:38.000000 swane-0.0.4/swane/nipype_pipeline/workflows/ref_workflow.py
--rw-rw-r--   0 mau       (1000) mau       (1000)    19603 2023-04-02 08:03:23.000000 swane-0.0.4/swane/nipype_pipeline/workflows/task_fMRI_workflow.py
--rw-rw-r--   0 mau       (1000) mau       (1000)    13745 2023-04-01 08:02:25.000000 swane-0.0.4/swane/nipype_pipeline/workflows/tractography_workflow.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     6335 2023-04-02 08:03:52.000000 swane-0.0.4/swane/nipype_pipeline/workflows/venous_workflow.py
-drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-04-11 08:24:09.748566 swane-0.0.4/swane/slicer/
--rw-rw-r--   0 mau       (1000) mau       (1000)     1857 2023-03-29 17:07:54.000000 swane-0.0.4/swane/slicer/SlicerCheckWorker.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     1256 2023-03-29 17:07:54.000000 swane-0.0.4/swane/slicer/SlicerExportWorker.py
--rw-rw-r--   0 mau       (1000) mau       (1000)        0 2023-03-29 17:07:54.000000 swane-0.0.4/swane/slicer/__init__.py
--rw-rw-r--   0 mau       (1000) mau       (1000)      159 2023-03-29 17:07:54.000000 swane-0.0.4/swane/slicer/slicer_script_freesurfer_module_check.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     8841 2023-04-01 08:02:25.000000 swane-0.0.4/swane/slicer/slicer_script_result.py
--rw-rw-r--   0 mau       (1000) mau       (1000)    12032 2023-04-05 09:49:56.000000 swane-0.0.4/swane/strings.py
-drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-04-11 08:24:09.748566 swane-0.0.4/swane/ui/
--rw-rw-r--   0 mau       (1000) mau       (1000)     1378 2023-03-31 12:13:49.000000 swane-0.0.4/swane/ui/CustomTreeWidgetItem.py
--rw-rw-r--   0 mau       (1000) mau       (1000)    18206 2023-04-05 07:58:18.000000 swane-0.0.4/swane/ui/MainWindow.py
--rw-rw-r--   0 mau       (1000) mau       (1000)      844 2023-03-29 17:07:54.000000 swane-0.0.4/swane/ui/PersistentProgressDialog.py
--rw-rw-r--   0 mau       (1000) mau       (1000)    19160 2023-03-29 20:42:46.000000 swane-0.0.4/swane/ui/PreferencesWindow.py
--rw-rw-r--   0 mau       (1000) mau       (1000)    33668 2023-04-04 03:00:01.000000 swane-0.0.4/swane/ui/PtTab.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     1001 2023-03-29 17:07:54.000000 swane-0.0.4/swane/ui/VerticalScrollArea.py
--rw-rw-r--   0 mau       (1000) mau       (1000)        0 2023-03-29 17:07:54.000000 swane-0.0.4/swane/ui/__init__.py
-drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-04-11 08:24:09.748566 swane-0.0.4/swane/ui/workers/
--rw-rw-r--   0 mau       (1000) mau       (1000)     4152 2023-03-29 17:07:54.000000 swane-0.0.4/swane/ui/workers/DicomSearchWorker.py
--rw-rw-r--   0 mau       (1000) mau       (1000)      725 2023-03-29 17:07:54.000000 swane-0.0.4/swane/ui/workers/WorkflowGeneratorWorker.py
--rw-rw-r--   0 mau       (1000) mau       (1000)      631 2023-03-29 17:07:54.000000 swane-0.0.4/swane/ui/workers/WorkflowMonitorWorker.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     3670 2023-04-04 02:58:13.000000 swane-0.0.4/swane/ui/workers/WorkflowProcess.py
--rw-rw-r--   0 mau       (1000) mau       (1000)        0 2023-03-29 17:07:54.000000 swane-0.0.4/swane/ui/workers/__init__.py
-drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-04-11 08:24:09.752565 swane-0.0.4/swane/utils/
--rw-rw-r--   0 mau       (1000) mau       (1000)     9139 2023-03-30 16:32:11.000000 swane-0.0.4/swane/utils/ConfigManager.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     2514 2023-03-30 17:00:25.000000 swane-0.0.4/swane/utils/DataInput.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     5568 2023-03-29 17:07:54.000000 swane-0.0.4/swane/utils/PreferenceEntry.py
--rw-rw-r--   0 mau       (1000) mau       (1000)        0 2023-03-29 17:07:54.000000 swane-0.0.4/swane/utils/__init__.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     1749 2023-03-29 17:07:54.000000 swane-0.0.4/swane/utils/check_dependency.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     3267 2023-03-29 17:07:54.000000 swane-0.0.4/swane/utils/fsl_conflict_handler.py
--rw-rw-r--   0 mau       (1000) mau       (1000)     4385 2023-04-11 10:17:10.000000 swane-0.0.4/swane/utils/shortcut_manager.py
-drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-04-11 08:24:09.744566 swane-0.0.4/swane.egg-info/
--rw-rw-r--   0 mau       (1000) mau       (1000)      427 2023-04-11 08:24:09.000000 swane-0.0.4/swane.egg-info/PKG-INFO
--rw-rw-r--   0 mau       (1000) mau       (1000)     2882 2023-04-11 08:24:09.000000 swane-0.0.4/swane.egg-info/SOURCES.txt
--rw-rw-r--   0 mau       (1000) mau       (1000)        1 2023-04-11 08:24:09.000000 swane-0.0.4/swane.egg-info/dependency_links.txt
--rw-rw-r--   0 mau       (1000) mau       (1000)       42 2023-04-11 08:24:09.000000 swane-0.0.4/swane.egg-info/entry_points.txt
--rw-rw-r--   0 mau       (1000) mau       (1000)      109 2023-04-11 08:24:09.000000 swane-0.0.4/swane.egg-info/requires.txt
--rw-rw-r--   0 mau       (1000) mau       (1000)        6 2023-04-11 08:24:09.000000 swane-0.0.4/swane.egg-info/top_level.txt
+drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-04-16 17:02:37.781633 swane-0.0.5/
+-rw-rw-r--   0 mau       (1000) mau       (1000)     1976 2023-03-29 17:07:54.000000 swane-0.0.5/LICENSE
+-rw-rw-r--   0 mau       (1000) mau       (1000)      184 2023-03-29 17:07:54.000000 swane-0.0.5/MANIFEST.in
+-rw-rw-r--   0 mau       (1000) mau       (1000)      427 2023-04-16 17:02:37.781633 swane-0.0.5/PKG-INFO
+-rw-rw-r--   0 mau       (1000) mau       (1000)        0 2023-03-29 17:07:54.000000 swane-0.0.5/README.md
+-rw-rw-r--   0 mau       (1000) mau       (1000)       38 2023-04-16 17:02:37.781633 swane-0.0.5/setup.cfg
+-rw-rw-r--   0 mau       (1000) mau       (1000)     1202 2023-04-11 08:22:48.000000 swane-0.0.5/setup.py
+drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-04-16 17:02:37.765633 swane-0.0.5/swane/
+-rw-rw-r--   0 mau       (1000) mau       (1000)       50 2023-04-16 17:02:08.000000 swane-0.0.5/swane/__init__.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     1827 2023-03-29 17:07:54.000000 swane-0.0.5/swane/__main__.py
+drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-04-16 17:02:37.765633 swane-0.0.5/swane/nipype_pipeline/
+-rw-rw-r--   0 mau       (1000) mau       (1000)    18408 2023-04-15 15:05:28.000000 swane-0.0.5/swane/nipype_pipeline/MainWorkflow.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)        0 2023-03-29 17:07:54.000000 swane-0.0.5/swane/nipype_pipeline/__init__.py
+drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-04-16 17:02:37.765633 swane-0.0.5/swane/nipype_pipeline/engine/
+-rw-rw-r--   0 mau       (1000) mau       (1000)     7906 2023-04-06 16:01:54.000000 swane-0.0.5/swane/nipype_pipeline/engine/CustomWorkflow.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     2795 2023-04-16 08:37:06.000000 swane-0.0.5/swane/nipype_pipeline/engine/MonitoredMultiProcPlugin.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)      405 2023-04-06 16:01:54.000000 swane-0.0.5/swane/nipype_pipeline/engine/NodeListEntry.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)        0 2023-03-29 17:07:54.000000 swane-0.0.5/swane/nipype_pipeline/engine/__init__.py
+drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-04-16 17:02:37.773633 swane-0.0.5/swane/nipype_pipeline/nodes/
+-rw-rw-r--   0 mau       (1000) mau       (1000)     2537 2023-04-06 16:01:54.000000 swane-0.0.5/swane/nipype_pipeline/nodes/AsymmetryIndex.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     2263 2023-04-06 16:01:54.000000 swane-0.0.5/swane/nipype_pipeline/nodes/CustomBEDPOSTX5.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     1245 2023-04-06 16:01:54.000000 swane-0.0.5/swane/nipype_pipeline/nodes/CustomDcm2niix.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)      489 2023-04-06 16:01:54.000000 swane-0.0.5/swane/nipype_pipeline/nodes/CustomDilateImage.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)      661 2023-04-06 16:01:54.000000 swane-0.0.5/swane/nipype_pipeline/nodes/CustomLabel2Vol.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)      923 2023-04-06 16:01:54.000000 swane-0.0.5/swane/nipype_pipeline/nodes/CustomProbTrackX2.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     2356 2023-04-06 16:01:54.000000 swane-0.0.5/swane/nipype_pipeline/nodes/CustomSliceTimer.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     2737 2023-04-06 16:01:54.000000 swane-0.0.5/swane/nipype_pipeline/nodes/DOmapOutliersMask.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     2437 2023-04-06 16:01:54.000000 swane-0.0.5/swane/nipype_pipeline/nodes/DeleteVolumes.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     4520 2023-04-06 16:01:54.000000 swane-0.0.5/swane/nipype_pipeline/nodes/FMRIGenSpec.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     2506 2023-04-06 16:01:54.000000 swane-0.0.5/swane/nipype_pipeline/nodes/ForceOrient.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)      458 2023-04-06 16:01:54.000000 swane-0.0.5/swane/nipype_pipeline/nodes/FslCluster.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     1600 2023-04-06 16:01:54.000000 swane-0.0.5/swane/nipype_pipeline/nodes/FslNVols.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     1601 2023-04-06 16:01:54.000000 swane-0.0.5/swane/nipype_pipeline/nodes/GetNiftiTR.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     1650 2023-04-06 16:01:54.000000 swane-0.0.5/swane/nipype_pipeline/nodes/MergeTargets.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     1849 2023-04-06 16:01:54.000000 swane-0.0.5/swane/nipype_pipeline/nodes/Orient.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     1400 2023-04-06 16:01:54.000000 swane-0.0.5/swane/nipype_pipeline/nodes/RandomSeedGenerator.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     2741 2023-04-06 16:01:54.000000 swane-0.0.5/swane/nipype_pipeline/nodes/SegmentHA.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     3247 2023-04-06 16:01:54.000000 swane-0.0.5/swane/nipype_pipeline/nodes/SumMultiTracks.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     3025 2023-04-06 16:01:54.000000 swane-0.0.5/swane/nipype_pipeline/nodes/ThrROI.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     2378 2023-04-06 16:01:54.000000 swane-0.0.5/swane/nipype_pipeline/nodes/VenousCheck.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     2703 2023-04-06 16:01:54.000000 swane-0.0.5/swane/nipype_pipeline/nodes/Zscore.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)       25 2023-03-29 17:07:54.000000 swane-0.0.5/swane/nipype_pipeline/nodes/__init__.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)      178 2023-04-06 16:01:54.000000 swane-0.0.5/swane/nipype_pipeline/nodes/utils.py
+drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-04-16 17:02:37.777633 swane-0.0.5/swane/nipype_pipeline/workflows/
+-rw-rw-r--   0 mau       (1000) mau       (1000)        0 2023-03-29 17:07:54.000000 swane-0.0.5/swane/nipype_pipeline/workflows/__init__.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)    13690 2023-03-31 12:25:20.000000 swane-0.0.5/swane/nipype_pipeline/workflows/domap_workflow.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     7922 2023-04-04 03:17:58.000000 swane-0.0.5/swane/nipype_pipeline/workflows/dti_preproc_workflow.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     7690 2023-04-01 08:02:25.000000 swane-0.0.5/swane/nipype_pipeline/workflows/freesurfer_workflow.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)    10956 2023-04-04 03:17:58.000000 swane-0.0.5/swane/nipype_pipeline/workflows/func_map_workflow.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     3504 2023-04-02 08:01:53.000000 swane-0.0.5/swane/nipype_pipeline/workflows/linear_reg_workflow.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     3142 2023-03-29 20:08:41.000000 swane-0.0.5/swane/nipype_pipeline/workflows/nonlinear_reg_workflow.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     2180 2023-04-02 07:46:38.000000 swane-0.0.5/swane/nipype_pipeline/workflows/ref_workflow.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)    19603 2023-04-02 08:03:23.000000 swane-0.0.5/swane/nipype_pipeline/workflows/task_fMRI_workflow.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)    13745 2023-04-01 08:02:25.000000 swane-0.0.5/swane/nipype_pipeline/workflows/tractography_workflow.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     6335 2023-04-02 08:03:52.000000 swane-0.0.5/swane/nipype_pipeline/workflows/venous_workflow.py
+drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-04-16 17:02:37.777633 swane-0.0.5/swane/slicer/
+-rw-rw-r--   0 mau       (1000) mau       (1000)     1930 2023-04-15 15:05:28.000000 swane-0.0.5/swane/slicer/SlicerCheckWorker.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     1331 2023-04-15 15:05:28.000000 swane-0.0.5/swane/slicer/SlicerExportWorker.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)        0 2023-03-29 17:07:54.000000 swane-0.0.5/swane/slicer/__init__.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)      302 2023-04-15 15:05:28.000000 swane-0.0.5/swane/slicer/slicer_script_freesurfer_module_check.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)    11931 2023-04-15 15:05:28.000000 swane-0.0.5/swane/slicer/slicer_script_result.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)    12030 2023-04-15 15:05:28.000000 swane-0.0.5/swane/strings.py
+drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-04-16 17:02:37.777633 swane-0.0.5/swane/ui/
+-rw-rw-r--   0 mau       (1000) mau       (1000)     1378 2023-03-31 12:13:49.000000 swane-0.0.5/swane/ui/CustomTreeWidgetItem.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)    18206 2023-04-05 07:58:18.000000 swane-0.0.5/swane/ui/MainWindow.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)      844 2023-03-29 17:07:54.000000 swane-0.0.5/swane/ui/PersistentProgressDialog.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)    19160 2023-03-29 20:42:46.000000 swane-0.0.5/swane/ui/PreferencesWindow.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)    33778 2023-04-16 08:37:06.000000 swane-0.0.5/swane/ui/PtTab.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     1001 2023-03-29 17:07:54.000000 swane-0.0.5/swane/ui/VerticalScrollArea.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)        0 2023-03-29 17:07:54.000000 swane-0.0.5/swane/ui/__init__.py
+drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-04-16 17:02:37.781633 swane-0.0.5/swane/ui/workers/
+-rw-rw-r--   0 mau       (1000) mau       (1000)     4152 2023-03-29 17:07:54.000000 swane-0.0.5/swane/ui/workers/DicomSearchWorker.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)      725 2023-03-29 17:07:54.000000 swane-0.0.5/swane/ui/workers/WorkflowGeneratorWorker.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)      631 2023-03-29 17:07:54.000000 swane-0.0.5/swane/ui/workers/WorkflowMonitorWorker.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     3829 2023-04-16 08:37:06.000000 swane-0.0.5/swane/ui/workers/WorkflowProcess.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)        0 2023-03-29 17:07:54.000000 swane-0.0.5/swane/ui/workers/__init__.py
+drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-04-16 17:02:37.781633 swane-0.0.5/swane/utils/
+-rw-rw-r--   0 mau       (1000) mau       (1000)     9139 2023-03-30 16:32:11.000000 swane-0.0.5/swane/utils/ConfigManager.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     2514 2023-03-30 17:00:25.000000 swane-0.0.5/swane/utils/DataInput.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     5568 2023-03-29 17:07:54.000000 swane-0.0.5/swane/utils/PreferenceEntry.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)        0 2023-03-29 17:07:54.000000 swane-0.0.5/swane/utils/__init__.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     1749 2023-03-29 17:07:54.000000 swane-0.0.5/swane/utils/check_dependency.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     3267 2023-03-29 17:07:54.000000 swane-0.0.5/swane/utils/fsl_conflict_handler.py
+-rw-rw-r--   0 mau       (1000) mau       (1000)     4385 2023-04-11 10:17:10.000000 swane-0.0.5/swane/utils/shortcut_manager.py
+drwxrwxr-x   0 mau       (1000) mau       (1000)        0 2023-04-16 17:02:37.765633 swane-0.0.5/swane.egg-info/
+-rw-rw-r--   0 mau       (1000) mau       (1000)      427 2023-04-16 17:02:37.000000 swane-0.0.5/swane.egg-info/PKG-INFO
+-rw-rw-r--   0 mau       (1000) mau       (1000)     2939 2023-04-16 17:02:37.000000 swane-0.0.5/swane.egg-info/SOURCES.txt
+-rw-rw-r--   0 mau       (1000) mau       (1000)        1 2023-04-16 17:02:37.000000 swane-0.0.5/swane.egg-info/dependency_links.txt
+-rw-rw-r--   0 mau       (1000) mau       (1000)       42 2023-04-16 17:02:37.000000 swane-0.0.5/swane.egg-info/entry_points.txt
+-rw-rw-r--   0 mau       (1000) mau       (1000)      109 2023-04-16 17:02:37.000000 swane-0.0.5/swane.egg-info/requires.txt
+-rw-rw-r--   0 mau       (1000) mau       (1000)        6 2023-04-16 17:02:37.000000 swane-0.0.5/swane.egg-info/top_level.txt
```

### Comparing `swane-0.0.4/LICENSE` & `swane-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `swane-0.0.4/setup.py` & `swane-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.4/swane/__main__.py` & `swane-0.0.5/swane/__main__.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.4/swane/nipype_pipeline/MainWorkflow.py` & `swane-0.0.5/swane/nipype_pipeline/MainWorkflow.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,85 +1,97 @@
 import os
 from multiprocessing import cpu_count
 from os.path import abspath
 
 import swane_supplement
 
+from swane.utils.ConfigManager import ConfigManager
+from swane.utils.DataInput import DataInputList
+
 from swane.nipype_pipeline.engine.CustomWorkflow import CustomWorkflow
 
 from swane.nipype_pipeline.workflows.linear_reg_workflow import linear_reg_workflow
 from swane.nipype_pipeline.workflows.task_fMRI_workflow import task_fMRI_workflow
 from swane.nipype_pipeline.workflows.nonlinear_reg_workflow import nonlinear_reg_workflow
 from swane.nipype_pipeline.workflows.ref_workflow import ref_workflow
 from swane.nipype_pipeline.workflows.freesurfer_workflow import freesurfer_workflow
 from swane.nipype_pipeline.workflows.domap_workflow import domap_workflow
 from swane.nipype_pipeline.workflows.func_map_workflow import func_map_workflow
 from swane.nipype_pipeline.workflows.venous_workflow import venous_workflow
 from swane.nipype_pipeline.workflows.dti_preproc_workflow import dti_preproc_workflow
 from swane.nipype_pipeline.workflows.tractography_workflow import tractography_workflow, SIDES
-from swane.utils.DataInput import DataInputList
 
 
 DEBUG = False
 
 
 # TODO implementazione error manager
-# todo valutare nome parlante per node
 class MainWorkflow(CustomWorkflow):
     SCENE_DIR = 'scene'
 
-    # TODO forse non serve, valutare eliminazione
-    def __init__(self, name, base_dir=None):
-        super(MainWorkflow, self).__init__(name, base_dir)
-
-    def add_input_folders(self, global_config, pt_config, data_input_list):
-
-        # global_config: configurazione globale dell'app
-        # pt_config: configurazione specifica del paziente
-        # data_input_list dictionary che ha come key tutte le possibili serie caricabili ciascuna con valore true/false
+    def add_input_folders(self, global_config: ConfigManager, pt_config: ConfigManager, data_input_list: DataInputList):
+        """
+        Create the Workflows and their sub-workflows based on the list of available data inputs 
+
+        Parameters
+        ----------
+        global_config : ConfigManager
+            The app global configurations.
+        pt_config : ConfigManager
+            The patient specific configurations.
+        data_input_list : DataInputList
+            The list of all available input data from the DICOM directory.
+
+        Returns
+        -------
+        None.
 
+        """
+        
         if not data_input_list.is_ref_loaded:
             return
 
-        # definizione dei boleani che saranno checkati prima della definizione dei specifici workflow
+        # Check for FreeSurfer requirement and request
         is_freesurfer = pt_config.is_freesurfer() and pt_config.get_pt_wf_freesurfer()
         is_hippo_amyg_labels = pt_config.is_freesurfer_matlab() and pt_config.get_pt_wf_hippo()
+        # Check for DOMap requirement and request
         is_domap = pt_config.getboolean('WF_OPTION', 'DOmap') and data_input_list[DataInputList.FLAIR3D].loaded
+        # Check for Asymmetry Index request
         is_ai = pt_config.getboolean('WF_OPTION', 'ai')
+        # Check for Tractography request
         is_tractography = pt_config.getboolean('WF_OPTION', 'tractography')
 
-        # definizione dei core assegnati al workflow e a ciascun nodo del workflow
+        # Core management
         self.max_cpu = global_config.getint('MAIN', 'maxPtCPU')
         if self.max_cpu > 0:
             max_node_cpu = max(int(self.max_cpu / 2), 1)
         else:
             max_node_cpu = max(int((cpu_count() - 2) / 2), 1)
 
-        # WORKFLOW 1: ELABORAZIONE T1 3D
+        # 3D T1w
         ref_dir = data_input_list.get_dicom_dir(DataInputList.T13D)
         t1 = ref_workflow(data_input_list[DataInputList.T13D].wf_name, ref_dir)
         t1.long_name = "3D T1w analysis"
         self.add_nodes([t1])
 
         t1.sink_result(self.base_dir, "outputnode", 'ref', self.SCENE_DIR)
         t1.sink_result(self.base_dir, "outputnode", 'ref_brain', self.SCENE_DIR)
 
-        # WORKFLOW 3: REGISTRAZIONE AD ALTANTE SIMMETRICO PER EVENTUALI ASIMMETRY index
         if is_ai and (data_input_list[DataInputList.ASL].loaded or data_input_list[DataInputList.PET].loaded):
+            # Non linear registration for Asymmetry Index
             sym = nonlinear_reg_workflow("sym")
             sym.long_name = "Symmetric atlas registration"
 
             sym_inputnode = sym.get_node("inputnode")
             sym_template = swane_supplement.sym_template
             sym_inputnode.inputs.atlas = sym_template
             self.connect(t1, "outputnode.ref_brain", sym, "inputnode.in_file")
 
-        # WORKFLOW 4: ELABORAZIONE FREESURFER
         if is_freesurfer:
-
+            # FreeSurfer analysis
             freesurfer = freesurfer_workflow("freesurfer", is_hippo_amyg_labels)
             freesurfer.long_name = "Freesurfer analysis"
 
             freesurfer_inputnode = freesurfer.get_node("inputnode")
             freesurfer_inputnode.inputs.max_node_cpu = max_node_cpu
             freesurfer_inputnode.inputs.subjects_dir = self.base_dir
             self.connect(t1, "outputnode.ref", freesurfer, "inputnode.ref")
@@ -88,40 +100,40 @@
             freesurfer.sink_result(self.base_dir, "outputnode", 'white', self.SCENE_DIR)
             freesurfer.sink_result(self.base_dir, "outputnode", 'vol_label_file', self.SCENE_DIR)
             if is_hippo_amyg_labels:
                 regex_subs = [("-T1.*.mgz", ".mgz")]
                 freesurfer.sink_result(self.base_dir, "outputnode", 'lh_hippoAmygLabels', 'scene.segmentHA', regex_subs)
                 freesurfer.sink_result(self.base_dir, "outputnode", 'rh_hippoAmygLabels', 'scene.segmentHA', regex_subs)
 
-        # WORKFLOW 5: ELABORAZIONE FLAIR
         if data_input_list[DataInputList.FLAIR3D].loaded:
+            # 3D Flair analysis
             flair_dir = data_input_list.get_dicom_dir(DataInputList.FLAIR3D)
             flair = linear_reg_workflow(data_input_list[DataInputList.FLAIR3D].wf_name, flair_dir)
             flair.long_name = "3D Flair analysis"
             self.add_nodes([flair])
 
             flair_inputnode = flair.get_node("inputnode")
             flair_inputnode.inputs.frac = 0.5
             flair_inputnode.inputs.crop = True
             flair_inputnode.inputs.output_name = "r-flair_brain.nii.gz"
             self.connect(t1, "outputnode.ref_brain", flair, "inputnode.reference")
 
             flair.sink_result(self.base_dir, "outputnode", 'registered_file', self.SCENE_DIR)
 
         if is_domap:
-            # WORKFLOW 6: REGISTRAZIONE AD ALTANTE MNI1mm (SERVE SOLO PER DOmap)
+            # Non linear registration to MNI1mm Atlas for DOmap
             mni1 = nonlinear_reg_workflow("mni1")
             mni1.long_name = "MNI atlas registration"
 
             mni1_inputnode = mni1.get_node("inputnode")
             mni1_path = abspath(os.path.join(os.environ["FSLDIR"], 'data/standard/MNI152_T1_1mm_brain.nii.gz'))
             mni1_inputnode.inputs.atlas = mni1_path
             self.connect(t1, "outputnode.ref_brain", mni1, "inputnode.in_file")
 
-            # WORKFLOW 7: ELABORAZIONE script_DOmap
+            # DOmap analysis
             domap = domap_workflow("DOmap", mni1_path)
             domap.long_name = "DOmap analysis"
 
             self.connect(t1, "outputnode.ref_brain", domap, "inputnode.ref_brain")
             self.connect(flair, "outputnode.registered_file", domap, "inputnode.flair_brain")
             self.connect(mni1, "outputnode.fieldcoeff_file", domap, "inputnode.ref_2_mni1_warp")
             self.connect(mni1, "outputnode.inverse_warp", domap, "inputnode.ref_2_mni1_inverse_warp")
@@ -141,32 +153,31 @@
                 flair2d_tra_inputnode.inputs.frac = 0.5
                 flair2d_tra_inputnode.inputs.crop = False
                 flair2d_tra_inputnode.inputs.output_name = "r-flair2d_%s_brain.nii.gz" % plane
                 self.connect(t1, "outputnode.ref_brain", flair2d, "inputnode.reference")
 
                 flair2d.sink_result(self.base_dir, "outputnode", 'registered_file', self.SCENE_DIR)
 
-        # WORKFLOW 11: ELABORAZIONE MDC
         if data_input_list[DataInputList.MDC].loaded:
+            # MDC analysis
             mdc_dir = data_input_list.get_dicom_dir(DataInputList.MDC)
             mdc = linear_reg_workflow(data_input_list[DataInputList.MDC].wf_name, mdc_dir)
             mdc.long_name = "Post-contrast 3D T1w analysis"
             self.add_nodes([mdc])
 
             mdc_inputnode = mdc.get_node("inputnode")
             mdc_inputnode.inputs.frac = 0.3
             mdc_inputnode.inputs.crop = True
             mdc_inputnode.inputs.output_name = "r-mdc_brain.nii.gz"
             self.connect(t1, "outputnode.ref_brain", mdc, "inputnode.reference")
 
             mdc.sink_result(self.base_dir, "outputnode", 'registered_file', self.SCENE_DIR)
 
-        # ELABORAZIONE ASL
         if data_input_list[DataInputList.ASL].loaded:
-
+            # ASL analysis
             asl_dir = data_input_list.get_dicom_dir(DataInputList.ASL)
             asl = func_map_workflow(data_input_list[DataInputList.ASL].wf_name, asl_dir, is_freesurfer, is_ai)
             asl.long_name = "Arterial Spin Labelling analysis"
 
             self.connect(t1, 'outputnode.ref_brain', asl, 'inputnode.reference')
             self.connect(t1, 'outputnode.ref_mask', asl, 'inputnode.brain_mask')
 
@@ -189,17 +200,16 @@
 
                 asl.sink_result(self.base_dir, "outputnode", 'ai', self.SCENE_DIR)
 
                 if is_freesurfer:
                     asl.sink_result(self.base_dir, "outputnode", 'ai_surf_lh', self.SCENE_DIR)
                     asl.sink_result(self.base_dir, "outputnode", 'ai_surf_rh', self.SCENE_DIR)
 
-        # ELABORAZIONE PET
         if data_input_list[DataInputList.PET].loaded:  # and check_input['ct_brain']:
-
+            # PET analysis
             pet_dir = data_input_list.get_dicom_dir(DataInputList.PET)
             pet = func_map_workflow(data_input_list[DataInputList.PET].wf_name, pet_dir, is_freesurfer, is_ai)
             pet.long_name = "Pet analysis"
 
             self.connect(t1, 'outputnode.ref', pet, 'inputnode.reference')
             self.connect(t1, 'outputnode.ref_mask', pet, 'inputnode.brain_mask')
 
@@ -222,30 +232,29 @@
 
                 pet.sink_result(self.base_dir, "outputnode", 'ai', self.SCENE_DIR)
 
                 if is_freesurfer:
                     pet.sink_result(self.base_dir, "outputnode", 'ai_surf_lh', self.SCENE_DIR)
                     pet.sink_result(self.base_dir, "outputnode", 'ai_surf_rh', self.SCENE_DIR)
 
-        # ELABORAZIONE VENOSA
         if data_input_list[DataInputList.VENOUS].loaded:
+            # Venous analysis
             venous_dir = data_input_list.get_dicom_dir(DataInputList.VENOUS)
             venous2_dir = None
             if data_input_list[DataInputList.VENOUS2].loaded:
                 venous2_dir = data_input_list.get_dicom_dir(DataInputList.VENOUS2)
             venous = venous_workflow(data_input_list[DataInputList.VENOUS].wf_name, venous_dir, venous2_dir)
             venous.long_name = "Venous MRA analysis"
 
             self.connect(t1, "outputnode.ref_brain", venous, "inputnode.ref_brain")
 
             venous.sink_result(self.base_dir, "outputnode", 'veins', self.SCENE_DIR)
 
-        # ELABORAZIONE DTI
         if data_input_list[DataInputList.DTI].loaded:
-
+            # DTI analysis
             dti_dir = data_input_list.get_dicom_dir(DataInputList.DTI)
             mni_dir = abspath(os.path.join(os.environ["FSLDIR"], 'data/standard/MNI152_T1_2mm_brain.nii.gz'))
 
             dti_preproc = dti_preproc_workflow(data_input_list[DataInputList.DTI].wf_name, dti_dir, mni_dir, is_tractography=is_tractography)
             dti_preproc.long_name = "Diffusion Tensor Imaging preprocessing"
             self.connect(t1, "outputnode.ref_brain", dti_preproc, "inputnode.ref_brain")
 
@@ -270,15 +279,15 @@
 
                         for side in SIDES:
                             tract_workflow.sink_result(self.base_dir, "outputnode", "waytotal_%s" % side,
                                                              self.SCENE_DIR + ".dti")
                             tract_workflow.sink_result(self.base_dir, "outputnode", "fdt_paths_%s" % side,
                                                              self.SCENE_DIR + ".dti")
 
-        # CONTROLLO SE SONO STATE CARICATE SEQUENZE FMRI ED EVENTUALMENTE LE ANALIZZO SINGOLARMENTE
+        # Check for Task FMRI sequences
         for y in range(DataInputList.FMRI_NUM):
 
             if data_input_list[DataInputList.FMRI+'_%d' % y].loaded:
 
                 task_a_name = pt_config['FMRI']["task_%d_name_a" % y]
                 task_b_name = pt_config['FMRI']["task_%d_name_b" % y]
                 task_duration = pt_config['FMRI'].getint('task_%d_duration' % y)
```

### Comparing `swane-0.0.4/swane/nipype_pipeline/engine/CustomWorkflow.py` & `swane-0.0.5/swane/nipype_pipeline/engine/CustomWorkflow.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.4/swane/nipype_pipeline/nodes/AsymmetryIndex.py` & `swane-0.0.5/swane/nipype_pipeline/nodes/AsymmetryIndex.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.4/swane/nipype_pipeline/nodes/CustomBEDPOSTX5.py` & `swane-0.0.5/swane/nipype_pipeline/nodes/CustomBEDPOSTX5.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.4/swane/nipype_pipeline/nodes/CustomDcm2niix.py` & `swane-0.0.5/swane/nipype_pipeline/nodes/CustomDcm2niix.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.4/swane/nipype_pipeline/nodes/CustomLabel2Vol.py` & `swane-0.0.5/swane/nipype_pipeline/nodes/CustomLabel2Vol.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.4/swane/nipype_pipeline/nodes/CustomProbTrackX2.py` & `swane-0.0.5/swane/nipype_pipeline/nodes/CustomProbTrackX2.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.4/swane/nipype_pipeline/nodes/CustomSliceTimer.py` & `swane-0.0.5/swane/nipype_pipeline/nodes/CustomSliceTimer.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.4/swane/nipype_pipeline/nodes/DOmapOutliersMask.py` & `swane-0.0.5/swane/nipype_pipeline/nodes/DOmapOutliersMask.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.4/swane/nipype_pipeline/nodes/DeleteVolumes.py` & `swane-0.0.5/swane/nipype_pipeline/nodes/DeleteVolumes.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.4/swane/nipype_pipeline/nodes/FMRIGenSpec.py` & `swane-0.0.5/swane/nipype_pipeline/nodes/FMRIGenSpec.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.4/swane/nipype_pipeline/nodes/ForceOrient.py` & `swane-0.0.5/swane/nipype_pipeline/nodes/ForceOrient.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.4/swane/nipype_pipeline/nodes/FslNVols.py` & `swane-0.0.5/swane/nipype_pipeline/nodes/FslNVols.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.4/swane/nipype_pipeline/nodes/GetNiftiTR.py` & `swane-0.0.5/swane/nipype_pipeline/nodes/GetNiftiTR.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.4/swane/nipype_pipeline/nodes/MergeTargets.py` & `swane-0.0.5/swane/nipype_pipeline/nodes/MergeTargets.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.4/swane/nipype_pipeline/nodes/Orient.py` & `swane-0.0.5/swane/nipype_pipeline/nodes/Orient.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.4/swane/nipype_pipeline/nodes/RandomSeedGenerator.py` & `swane-0.0.5/swane/nipype_pipeline/nodes/RandomSeedGenerator.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.4/swane/nipype_pipeline/nodes/SegmentHA.py` & `swane-0.0.5/swane/nipype_pipeline/nodes/SegmentHA.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.4/swane/nipype_pipeline/nodes/SumMultiTracks.py` & `swane-0.0.5/swane/nipype_pipeline/nodes/SumMultiTracks.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.4/swane/nipype_pipeline/nodes/ThrROI.py` & `swane-0.0.5/swane/nipype_pipeline/nodes/ThrROI.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.4/swane/nipype_pipeline/nodes/VenousCheck.py` & `swane-0.0.5/swane/nipype_pipeline/nodes/VenousCheck.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.4/swane/nipype_pipeline/nodes/Zscore.py` & `swane-0.0.5/swane/nipype_pipeline/nodes/Zscore.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.4/swane/nipype_pipeline/workflows/domap_workflow.py` & `swane-0.0.5/swane/nipype_pipeline/workflows/domap_workflow.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.4/swane/nipype_pipeline/workflows/dti_preproc_workflow.py` & `swane-0.0.5/swane/nipype_pipeline/workflows/dti_preproc_workflow.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.4/swane/nipype_pipeline/workflows/freesurfer_workflow.py` & `swane-0.0.5/swane/nipype_pipeline/workflows/freesurfer_workflow.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.4/swane/nipype_pipeline/workflows/func_map_workflow.py` & `swane-0.0.5/swane/nipype_pipeline/workflows/func_map_workflow.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.4/swane/nipype_pipeline/workflows/linear_reg_workflow.py` & `swane-0.0.5/swane/nipype_pipeline/workflows/linear_reg_workflow.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.4/swane/nipype_pipeline/workflows/nonlinear_reg_workflow.py` & `swane-0.0.5/swane/nipype_pipeline/workflows/nonlinear_reg_workflow.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.4/swane/nipype_pipeline/workflows/ref_workflow.py` & `swane-0.0.5/swane/nipype_pipeline/workflows/ref_workflow.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.4/swane/nipype_pipeline/workflows/task_fMRI_workflow.py` & `swane-0.0.5/swane/nipype_pipeline/workflows/task_fMRI_workflow.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.4/swane/nipype_pipeline/workflows/tractography_workflow.py` & `swane-0.0.5/swane/nipype_pipeline/workflows/tractography_workflow.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.4/swane/nipype_pipeline/workflows/venous_workflow.py` & `swane-0.0.5/swane/nipype_pipeline/workflows/venous_workflow.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.4/swane/slicer/SlicerCheckWorker.py` & `swane-0.0.5/swane/slicer/SlicerCheckWorker.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,19 @@
 
 
 class SlicerCheckSignaler(QObject):
     slicer = Signal(str, str, bool)
 
 
 class SlicerCheckWorker(QRunnable):
+    """
+    Spawn a thread for 3D Slicer dependency check 
+
+    """
+    
     def __init__(self, parent=None):
         super(SlicerCheckWorker, self).__init__(parent)
         self.signal = SlicerCheckSignaler()
 
     def run(self):
         import platform
         if platform.system() == "Darwin":
```

### Comparing `swane-0.0.4/swane/slicer/SlicerExportWorker.py` & `swane-0.0.5/swane/slicer/SlicerExportWorker.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,14 +4,19 @@
 
 
 class SlicerExportSignaler(QObject):
     export = Signal(str)
 
 
 class SlicerExportWorker(QRunnable):
+    """
+    Spawn a thread for 3D Slicer result export 
+
+    """
+    
     PROGRESS_MSG_PREFIX = 'SLICERLOADER: '
     END_MSG = "ENDLOADING"
 
     def __init__(self, slicer_path, pt_folder, scene_ext, parent=None):
         super(SlicerExportWorker, self).__init__(parent)
         self.signal = SlicerExportSignaler()
         self.slicer_path = slicer_path
```

### Comparing `swane-0.0.4/swane/slicer/slicer_script_result.py` & `swane-0.0.5/swane/slicer/slicer_script_result.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,59 @@
+# slicerpython script for module checking
+# Warning: slicer library is not required beacuse the script is executed in Slicer environment
+
 import sys
 import os
 import subprocess
 
+def load_anat(scene_dir: str, volume_name: str):
+    """
+    Creates a scalar node from a NIFTI file.
+
+    Parameters
+    ----------
+    scene_dir : str
+        The scene directory.
+    volume_name : str
+        The NIFTI file name (without extension).
+
+    Returns
+    -------
+    node : MRMLCore.vtkMRMLScalarVolumeNode
+        The scalar node generated from the NIFTI file.
 
-def load_anat(scene_dir, volume_name):
+    """
+    
     file = os.path.join(scene_dir, volume_name + ".nii.gz")
     node = None
     if os.path.exists(file):
         try:
             print("SLICERLOADER: Loading " + volume_name)
             node = slicer.util.loadVolume(file)
         except:
             pass
+        
     return node
 
 
-def lesion_segment(scene_dir):
+def lesion_segment(scene_dir: str):
+    """
+    Prepares an empty segment for optional manual segmentation.
+
+    Parameters
+    ----------
+    scene_dir : str
+        The scene directory.
+
+    Returns
+    -------
+    None.
+
+    """
+    
     file = os.path.join(scene_dir, "seg_lesions.seg.nrrd")
     if os.path.exists(file):
         print("SLICERLOADER: Loading existing lesion segment")
         slicer.util.loadSegmentation(file)
     else:
         print("SLICERLOADER: Creating lesion segment")
         seg_node = slicer.mrmlScene.AddNewNodeByClass('vtkMRMLSegmentationNode', "seg_lesions")
@@ -27,50 +61,121 @@
         seg_node.GetSegmentation().AddEmptySegment("Lesion", "Lesion", [1, 0, 0])
         seg_node.CreateClosedSurfaceRepresentation()
         my_storage_node = seg_node.CreateDefaultStorageNode()
         my_storage_node.SetFileName(file)
         my_storage_node.WriteData(seg_node)
 
 
-def load_freesurfer_surf(scene_dir, node_name, ref_node):
+def load_freesurfer_surf(scene_dir: str, node_name: str, ref_node):
+    """
+    Loads the FreeSurfer surface.
+
+    Parameters
+    ----------
+    scene_dir : str
+        The scene directory.
+    node_name : str
+        The surface file.
+    ref_node : MRMLCore.vtkMRMLScalarVolumeNode
+        The reference node for surface positioning.
+
+    Returns
+    -------
+    #TODO specificare tipo di surf_node
+    surf_node : TYPE
+        The slicer node with loaded surface.
+
+    """
+    
     file = os.path.join(scene_dir, node_name)
+    surf_node = None
+    
     if os.path.exists(file):
         try:
             print("SLICERLOADER: Loading surface " + node_name)
             surf_node = slicer.util.loadNodeFromFile(file, 'FreeSurferModelFile',
                                                     {"referenceVolumeID": ref_node.GetID()})
             surf_node.GetDisplayNode().SetColor(0.82, 0.82, 0.82)
-            return surf_node
         except:
             pass
-    return None
+        
+    return surf_node
 
 
-def load_freesurfer_overlay(scene_dir, node_name, surf_node):
+def load_freesurfer_overlay(scene_dir: str, node_name: str, surf_node):
+    """
+    Applies an overlay on the FreeSurfer surface.
+
+    Parameters
+    ----------
+    scene_dir : str
+        The scene directory.
+    node_name : str
+        The surface file.
+    #TODO specificare tipo di surf_node
+    surf_node : TYPE
+        The slicer node with loaded surface.
+
+    Returns
+    -------
+    None.
+
+    """
+    
     file = os.path.join(scene_dir, node_name)
     if os.path.exists(file):
         try:
             print("SLICERLOADER: Loading surface overlay " + node_name)
             overlay_node = slicer.util.loadNodeFromFile(file, 'FreeSurferScalarOverlayFile',
                                                        {"modelNodeId": surf_node.GetID()})
             overlay_node.GetDisplayNode().SetAndObserveColorNodeID('vtkMRMLColorTableNodeFileColdToHotRainbow.txt')
             overlay_node.GetDisplayNode().SetScalarVisibility(False)
         except:
             pass
 
 
-def load_freesurfer_segmentation_file(seg_file):
+def load_freesurfer_segmentation_file(seg_file: str):
+    """
+    Loads the FreeSurfer segmentation file.
+
+    Parameters
+    ----------
+    seg_file : str
+        The segmentation file name.
+
+    Returns
+    -------
+    None.
+
+    """
+    
     if os.path.exists(seg_file):
         try:
             slicer.util.loadNodeFromFile(seg_file, 'FreeSurferSegmentationFile')
         except:
             pass
 
 
-def load_freesurfer(scene_dir, ref_node):
+def load_freesurfer(scene_dir: str, ref_node):
+    """
+    Loads the FreeSurfer output.
+
+    Parameters
+    ----------
+    scene_dir : str
+        The scene directory.
+    ref_node : MRMLCore.vtkMRMLScalarVolumeNode
+        The reference node for surface positioning.
+
+    Returns
+    -------
+    None.
+
+    """
+    
     seg_list = ["r-aparc_aseg.mgz", "segmentHA/lh.hippoAmygLabels.mgz", "segmentHA/rh.hippoAmygLabels.mgz"]
     for file in seg_list:
         seg_file = os.path.join(scene_dir, file)
         load_freesurfer_segmentation_file(seg_file)
 
     lh_pial = load_freesurfer_surf(scene_dir, "lh.pial", ref_node)
     rh_pial = load_freesurfer_surf(scene_dir, "rh.pial", ref_node)
@@ -81,15 +186,31 @@
 
     overlays = ['pet_surf', 'pet_ai_surf', 'pet_zscore_surf', 'asl_surf', 'asl_ai_surf', 'asl_zscore_surf']
     for overlay in overlays:
         load_freesurfer_overlay(scene_dir, overlay + "_lh.mgz", lh_pial)
         load_freesurfer_overlay(scene_dir, overlay + "_rh.mgz", rh_pial)
 
 
-def load_vein(scene_dir):
+def load_vein(scene_dir: str, remove_vein: bool=False):
+    """
+    Loads the veins files and creates their 3d model.
+
+    Parameters
+    ----------
+    scene_dir : str
+        The scene directory.
+    remove_vein : bool, optional
+        True if the model must remove the original veins images. The default is False.
+
+    Returns
+    -------
+    None.
+
+    """
+    
     vein_volume_name = "r-veins_inskull"
     vein_node = load_anat(scene_dir, vein_volume_name)
     if vein_node is None:
         return
     print("SLICERLOADER: Creating 3D model: Veins")
 
     try:
@@ -112,18 +233,43 @@
     gray_maker = slicer.modules.grayscalemodelmaker
     slicer.cli.runSync(gray_maker, None, parameters)
     vein_model.GetDisplayNode().SetColor(0, 0, 1)
     vein_model.SetName("Veins")
     my_storage_node = vein_model.CreateDefaultStorageNode()
     my_storage_node.SetFileName(os.path.join(scene_dir, "veins.vtk"))
     my_storage_node.WriteData(vein_model)
-    slicer.mrmlScene.RemoveNode(vein_node)
+    
+    if remove_vein:
+        slicer.mrmlScene.RemoveNode(vein_node)
+
+
+def tract_model(segmentation_node, dti_dir: str, tract: str, side: str):
+    """
+    Creates the 3d model of a tract.
+
+    Parameters
+    ----------
+    #TODO verificare tipo
+    segmentation_node : TYPE
+        DESCRIPTION.
+    dti_dir : str
+        The DTI directory.
+    tract : str
+        The name of the tract.
+    side : str
+        The side of the tract:
+            - LH for left side
+            - RH for right side
+
+    Returns
+    -------
+    None.
 
-
-def tract_model(segmentation_node, dti_dir, tract, side):
+    """
+    
     tract_file = os.path.join(dti_dir, "r-" + tract['name'] + "_" + side + ".nii.gz")
     if not os.path.exists(tract_file):
         return
 
     waytotal_file = os.path.join(dti_dir, "r-" + tract['name'] + "_" + side + "_waytotal")
     waytotal = 0
     if os.path.exists(waytotal_file):
@@ -149,60 +295,79 @@
     segment_editor_widget.setMRMLSegmentEditorNode(segment_editor_node)
     segment_editor_widget.setSegmentationNode(segmentation_node)
     segment_editor_widget.setMasterVolumeNode(tract_node)
 
     # Create segment
     tract_segment_id = segmentation_node.GetSegmentation().AddEmptySegment(tract['name'], tract['name'], tract['color'])
     segment_editor_node.SetSelectedSegmentID(tract_segment_id)
+    
     # Fill by thresholding
     segment_editor_widget.setActiveEffectByName("Threshold")
     effect = segment_editor_widget.activeEffect()
     effect.setParameter("MinimumThreshold", thr)
     effect.self().onApply()
 
     # Delete temporary segment editor
     segment_editor_widget = None
     slicer.mrmlScene.RemoveNode(segment_editor_node)
     slicer.mrmlScene.RemoveNode(tract_node)
 
 
-def load_fmri(scene_dir):
+def load_fmri(scene_dir: str):
+    """
+    Loads the fMRI results.
+
+    Parameters
+    ----------
+    scene_dir : str
+        The scene directory.
+
+    Returns
+    -------
+    None.
+
+    """
+    
     fmri_path = os.path.join(scene_dir, "fMRI")
     if not os.path.exists(fmri_path):
         return
     print("SLICERLOADER: Loading fMRI")
     for file in os.listdir(fmri_path):
         if file.endswith('.nii.gz'):
             func_node = load_anat(fmri_path, file.replace(".nii.gz", ""))
             if func_node is not None:
                 func_node.GetDisplayNode().SetAndObserveColorNodeID('vtkMRMLPETProceduralColorNodePET-Rainbow2')
 
 
-def main_tract(dti_dir, scene_dir):
+def main_tract(dti_dir: str, scene_dir: str):
     sides = ["rh", "lh"]
     tracts = [
         {"name": "cst", "thr": "500", "color": [0, 1, 0]},
         {"name": "af", "thr": "1500", "color": [1, 0, 1]},
         {"name": "or", "thr": "500", "color": [1, 1, 0]}
     ]
 
     print("SLICERLOADER: Creating DTI tracts 3D models (some minutes!)")
 
     for side in sides:
         # Create segmentation
         segmentation_node = slicer.mrmlScene.AddNewNodeByClass("vtkMRMLSegmentationNode", "tracts_" + side)
         segmentation_node.CreateDefaultDisplayNodes()  # only needed for display
+        
         for tract in tracts:
             tract_model(segmentation_node, dti_dir, tract, side)
+            
         segmentation_node.CreateClosedSurfaceRepresentation()
         my_storage_node = segmentation_node.CreateDefaultStorageNode()
         my_storage_node.SetFileName(os.path.join(scene_dir, "tracts_" + side + ".seg.nrrd"))
         my_storage_node.WriteData(segmentation_node)
 
+###############################################################################
 
+# slicerpython execution code
 slicer.mrmlScene.Clear(0)
 sceneDir = os.path.join(os.getcwd(), "scene")
 
 if not os.path.isdir(sceneDir):
     print("SLICERLOADER: Results folder not found")
 else:
     refNode = load_anat(sceneDir, "ref")
@@ -224,14 +389,16 @@
         load_fmri(sceneDir)
 
         load_vein(sceneDir)
 
         load_freesurfer(sceneDir, refNode)
 
         ext = "mrb"
+        
+        #TODO valutare
         # Saving in MRML doesn't work well, disable extension choice for now
         # if sys.argv[1] is not None and sys.argv[1] == "1":
         #     ext = "mrml"
 
         print("SLICERLOADER: Saving multimodale scene (some minutes)")
         slicer.util.saveScene(os.path.join(sceneDir, "scene." + ext))
```

### Comparing `swane-0.0.4/swane/strings.py` & `swane-0.0.5/swane/strings.py`

 * *Files 0% similar despite different names*

```diff
@@ -200,9 +200,8 @@
 node_names["Level1Design"] = "FEAT files generation"
 node_names["FEATModel"] = "design file generation"
 node_names["FILMGLS"] = "General-Linear-Model estimation"
 node_names["SmoothEstimate"] = "smoothness estimation"
 node_names["FslCluster"] = "cluster extraction"
 node_names["SampleToSurface"] = "surface projection"
 node_names["FAST"] = "Tissue segmentation"
-node_names["DOmapOutliersMask"] = "outliers mask generation"
-
+node_names["DOmapOutliersMask"] = "outliers mask generation"
```

### Comparing `swane-0.0.4/swane/ui/CustomTreeWidgetItem.py` & `swane-0.0.5/swane/ui/CustomTreeWidgetItem.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.4/swane/ui/MainWindow.py` & `swane-0.0.5/swane/ui/MainWindow.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.4/swane/ui/PersistentProgressDialog.py` & `swane-0.0.5/swane/ui/PersistentProgressDialog.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.4/swane/ui/PreferencesWindow.py` & `swane-0.0.5/swane/ui/PreferencesWindow.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.4/swane/ui/PtTab.py` & `swane-0.0.5/swane/ui/PtTab.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from swane.ui.PersistentProgressDialog import PersistentProgressDialog
 from swane.ui.PreferencesWindow import PreferencesWindow
 from swane.ui.VerticalScrollArea import VerticalScrollArea
 from swane.utils.ConfigManager import ConfigManager
 from swane.ui.workers.DicomSearchWorker import DicomSearchWorker
 from swane.nipype_pipeline.workflows.freesurfer_workflow import FS_DIR
 from swane.utils.DataInput import DataInput, DataInputList
+from swane.nipype_pipeline.engine.MonitoredMultiProcPlugin import MonitoredMultiProcPlugin
 
 
 class PtTab(QTabWidget):
     DATATAB = 0
     EXECTAB = 1
     RESULTTAB = 2
     GRAPH_DIR_NAME = "graph"
@@ -110,17 +111,17 @@
         # Every message starts by "nipype_pt_x.", remove that
         split.pop(0)
 
         # Remaining message must be like: workflow_name.node_name.message_type
         if len(split) < 3:
             return
 
-        if split[2] == WorkflowProcess.NODE_STARTED:
+        if split[2] == MonitoredMultiProcPlugin.NODE_STARTED:
             icon = self.main_window.LOADING_MOVIE_FILE
-        elif split[2] == WorkflowProcess.NODE_COMPLETED:
+        elif split[2] == MonitoredMultiProcPlugin.NODE_COMPLETED:
             icon = self.main_window.OK_ICON_FILE
         else:
             icon = self.main_window.ERROR_ICON_FILE
 
         self.node_list[split[0]].node_list[split[1]].node_holder.setArt(icon)
 
         self.node_list[split[0]].node_holder.setExpanded(True)
```

### Comparing `swane-0.0.4/swane/ui/VerticalScrollArea.py` & `swane-0.0.5/swane/ui/VerticalScrollArea.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.4/swane/ui/workers/DicomSearchWorker.py` & `swane-0.0.5/swane/ui/workers/DicomSearchWorker.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.4/swane/ui/workers/WorkflowGeneratorWorker.py` & `swane-0.0.5/swane/ui/workers/WorkflowGeneratorWorker.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.4/swane/ui/workers/WorkflowMonitorWorker.py` & `swane-0.0.5/swane/ui/workers/WorkflowMonitorWorker.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.4/swane/ui/workers/WorkflowProcess.py` & `swane-0.0.5/swane/ui/workers/WorkflowProcess.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 from logging import Formatter
 import os
 import traceback
 from multiprocessing import Process, Event
 from threading import Thread
 from swane.ui.workers.WorkflowMonitorWorker import WorkflowMonitorWorker
 from nipype.external.cloghandler import ConcurrentRotatingFileHandler
-from nipype.pipeline.plugins.multiproc import MultiProcPlugin
+from swane.nipype_pipeline.engine.MonitoredMultiProcPlugin import MonitoredMultiProcPlugin
 
 
 class WorkflowProcess(Process):
-    NODE_STARTED = "start"
-    NODE_COMPLETED = "end"
-    NODE_ERROR = "exception"
+    # NODE_STARTED = "start"
+    # NODE_COMPLETED = "end"
+    # NODE_ERROR = "exception"
 
     LOG_CHANNELS = [
         "nipype.workflow",
         "nipype.utils",
         "nipype.filemanip",
         "nipype.interface",
     ]
@@ -37,20 +37,22 @@
     def add_handlers(handler):
         for channel in WorkflowProcess.LOG_CHANNELS:
             logging.getLogger(channel).addHandler(handler)
 
     def workflow_run_worker(self):
         plugin_args = {
             'mp_context': 'fork',
-            'status_callback': self.callback_function
+            'queue': self.queue
+            # 'status_callback': self.callback_function
         }
         if self.workflow.max_cpu > 0:
             plugin_args['n_procs'] = self.workflow.max_cpu
         try:
-            self.workflow.run(plugin=MultiProcPlugin(plugin_args=plugin_args))
+            # self.workflow.run(plugin=MultiProcPlugin(plugin_args=plugin_args))
+            self.workflow.run(plugin=MonitoredMultiProcPlugin(plugin_args=plugin_args))
         except:
             traceback.print_exc()
         self.stop_event.set()
 
     def callback_function(self, node, signal):
         try:
             self.queue.put(node.fullname + "." + signal)
```

### Comparing `swane-0.0.4/swane/utils/ConfigManager.py` & `swane-0.0.5/swane/utils/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.4/swane/utils/DataInput.py` & `swane-0.0.5/swane/utils/DataInput.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.4/swane/utils/PreferenceEntry.py` & `swane-0.0.5/swane/utils/PreferenceEntry.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.4/swane/utils/check_dependency.py` & `swane-0.0.5/swane/utils/check_dependency.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.4/swane/utils/fsl_conflict_handler.py` & `swane-0.0.5/swane/utils/fsl_conflict_handler.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.4/swane/utils/shortcut_manager.py` & `swane-0.0.5/swane/utils/shortcut_manager.py`

 * *Files identical despite different names*

### Comparing `swane-0.0.4/swane.egg-info/SOURCES.txt` & `swane-0.0.5/swane.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 swane.egg-info/dependency_links.txt
 swane.egg-info/entry_points.txt
 swane.egg-info/requires.txt
 swane.egg-info/top_level.txt
 swane/nipype_pipeline/MainWorkflow.py
 swane/nipype_pipeline/__init__.py
 swane/nipype_pipeline/engine/CustomWorkflow.py
+swane/nipype_pipeline/engine/MonitoredMultiProcPlugin.py
 swane/nipype_pipeline/engine/NodeListEntry.py
 swane/nipype_pipeline/engine/__init__.py
 swane/nipype_pipeline/nodes/AsymmetryIndex.py
 swane/nipype_pipeline/nodes/CustomBEDPOSTX5.py
 swane/nipype_pipeline/nodes/CustomDcm2niix.py
 swane/nipype_pipeline/nodes/CustomDilateImage.py
 swane/nipype_pipeline/nodes/CustomLabel2Vol.py
```

