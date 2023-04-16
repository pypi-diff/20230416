# Comparing `tmp/RIFT-0.0.15.8rc6.tar.gz` & `tmp/RIFT-0.0.15.8rc7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/RIFT-0.0.15.8rc6.tar", last modified: Fri Apr  7 18:25:00 2023, max compression
+gzip compressed data, was "dist/RIFT-0.0.15.8rc7.tar", last modified: Sun Apr 16 18:25:20 2023, max compression
```

## Comparing `RIFT-0.0.15.8rc6.tar` & `RIFT-0.0.15.8rc7.tar`

### file list

```diff
@@ -1,186 +1,187 @@
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-07 18:25:00.000000 RIFT-0.0.15.8rc6/
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1118 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/LICENSE.md
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    22146 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/GETTING_STARTED.md
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6132 2022-09-24 12:18:48.000000 RIFT-0.0.15.8rc6/TROUBLESHOOTING.md
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6136 2022-09-24 12:18:48.000000 RIFT-0.0.15.8rc6/howto.md
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      204 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MANIFEST.in
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-07 18:25:00.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-07 18:25:00.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-07 18:25:00.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)   241367 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/lalsimutils.py
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-07 18:25:00.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/integrators/
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7235 2022-10-24 14:00:10.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/integrators/statutils.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    18359 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/integrators/MonteCarloEnsemble.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/integrators/__init__.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    68867 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsamplerGPU.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    53601 2023-03-12 13:15:08.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsampler.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    33113 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/integrators/weighted_gmm.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2592 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/integrators/direct_quadrature.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2901 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/integrators/multivariate_truncnorm.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    20255 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/integrators/gaussian_mixture_model.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    28094 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsamplerEnsemble.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      163 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/__init__.py
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-07 18:25:00.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/interpolators/
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    26826 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/interpolators/senni.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3835 2022-10-23 22:26:00.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/interpolators/ConstrainedQuadraticLikelihood.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1655 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/interpolators/gp.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/interpolators/__init__.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3488 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/interpolators/interp_gpu.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9944 2022-10-23 22:26:00.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/interpolators/BayesianLeastSquares.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5558 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/interpolators/internal_GP.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2658 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/interpolators/efficient_save_sklearn_gp.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2518 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/interpolators/gpytorch_wrapper.py
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-07 18:25:00.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/physics/
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    52302 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/physics/ROMWaveformManager.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)       68 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/physics/__init__.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    31276 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/physics/EOBTidalExternalC.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2654 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/physics/MonotonicSpline.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    26126 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/physics/EOBTidalExternal.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    19507 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/physics/PrecessingFisherMatrix.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    23733 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/physics/effectiveFisher.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4664 2023-03-12 13:15:08.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/physics/GWSignal.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    63089 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/physics/EOSManager.py
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-07 18:25:00.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9324 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/modules.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)       65 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/__init__.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      229 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/common_cl.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7367 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/bounded_kde.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2641 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/weight_simulations.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    29427 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/amrlib.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    23083 2022-10-11 14:57:54.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/our_corner.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8657 2023-03-12 13:15:08.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/xmlutils.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    10915 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/samples_utils.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    30542 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/ourparams.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2901 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/sky_rotations.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    10623 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/spokes.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6975 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/tools.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    70947 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/ModifiedScikitFit.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)   108434 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/dag_utils.py
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-07 18:25:00.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/likelihood/
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1643 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/likelihood/Q_inner_product.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5269 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/likelihood/optimized_gpu_tools.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1211 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/likelihood/priors_utils.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/likelihood/__init__.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    33438 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/likelihood/SphericalHarmonics_gpu.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4007 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/likelihood/vectorized_general_tools.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4706 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/likelihood/vectorized_lal_tools.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    94119 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/likelihood/factored_likelihood.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1525 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/likelihood/cuda_Q_inner_product.cu
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-07 18:25:00.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    34265 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_AMRGrid.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2778 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_HyperCombine.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    10752 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_NRNearestSimulationTo.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1018 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_ILEROMdagPostprocess.sh
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3250 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_FetchExternalGrid.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6671 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_NRDumpDetectorResponse.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      219 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_CacheFileConvert.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      256 2022-10-11 14:57:54.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_ForOSG_MakeLocalFramesDir.sh
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)   163149 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_ConstructIntrinsicPosterior_GenericCoordinates.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    11799 2023-03-12 13:15:08.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/convert_output_format_ile2inference
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      354 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/switcheroo
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2698 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_JoinXML.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    50356 2022-10-11 14:57:54.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_ManualOverlapGrid.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3080 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_ResampleILEOutputWithExtrinsic.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1436 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_CharacterizePosterior.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      457 2022-10-15 00:56:03.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_TruncateMergeFrames.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6162 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_GenerateMaxlnLWaveform_NRFromIndex.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2800 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/config_yank.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6780 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_InitMargTable
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    18544 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_AnalyticFisherGrid.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3377 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_NR_GWMemory.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    11893 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/calibration_reweighting.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3266 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_FrameZeroNoiseSNR.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1640 2023-03-12 13:15:08.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_ForOSG_MakeTruncatedLocalFramesDir.sh
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3696 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_AdaptiveExponent.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2784 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_WriteInjectionFile.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5424 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_RIFT_MultiMetaPipe.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2223 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_GridRecenter.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    40228 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_IterativeFisher.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8723 2022-10-11 14:57:54.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/assess_propose_CIP_convergence_sequence.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    15127 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_CompareWaveformsInDetectors.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    13979 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/create_postprocessing_event_dag.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    12414 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_ParameterPuffball.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1028 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_CIPdagPostprocess.sh
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1886 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/helper_OnlinePSDCleanup.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3746 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/resample_uniform_comoving.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1675 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_RandomizeOverlapOrder.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      389 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_EstimateWaveformDuration.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1087 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_PosteriorPostprocess.sh
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7195 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_MarginalizedLikelihoodEOSIntegralFromIntermediate.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      829 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_ILENextGeneration.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    11553 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_GenerateMaxlnLWaveform.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2768 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/create_ile_sub_dag.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4982 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_TestSpokesIO.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8109 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_LALCompareApproximantsOnSamples.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1955 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_WriteXMLWithEOS.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    55368 2022-11-28 22:41:57.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_ConstructIntrinsicPosterior_GaussianResampling.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    10380 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_ConstructBNSMarginalEOSRank.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6293 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_ROMWriteFrame.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    35804 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_RIFT_pseudo_pipe_lowlatency.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    71601 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_BasicMultiApproxIteration
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8821 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_NRBestOfIndex.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    20394 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_NRExtrudeOverlapGrid.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    73473 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_RIFT_pseudo_pipe.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3934 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_CleanILE.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1214 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_MassGrid.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1490 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_NRdagPostprocess.sh
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5408 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/make_uni_comov_skymap.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5672 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_NRIndexedFminCutToILE.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2314 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_CoordinateNamesAngularToCartesianSpins.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    37686 2023-03-12 13:15:08.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/plot_posterior_corner.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    98549 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic_batchmode
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7587 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_TEOBResumSWriteFrame.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5156 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_HyperparameterPuffball.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3302 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_PrintInjection.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7660 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_LALWriteFrame.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      876 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_CoincIFOUtility.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9830 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_NRWriteFrame.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7130 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_BatchConvertResampleILEOutput.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6140 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/convergence_test_amr.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2013 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/convert_psd_ascii2xml
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    11254 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_TidalPlotSimulationStrain.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    20152 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/ile_postproc_add_time
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      814 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_TestXMLParameterStorage.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1224 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/convert_dat_to_hdf5.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    33506 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/create_eos_posterior_pipeline
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      853 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_ConsolidateDAGsUnderMaster.sh
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      541 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/convert_output_format_ascii2h5.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    95698 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/helper_LDG_Events.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2450 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_MassGridCoalesce.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4794 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_NRRelabelILE.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4553 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_IntermediateEOSIntegralFromFit.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1920 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/convert_output_format_allnet2xml
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    13919 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_GridSubsetOfTemplateBank.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2349 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_ParameterFilter.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    83560 2023-03-12 13:15:08.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1590 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_HyperparameterGrid.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    14569 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/create_event_dag_via_grid
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8994 2022-10-11 14:57:54.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/convergence_test_samples.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)   113357 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_BasicIteration
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    88335 2022-10-11 14:57:54.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_AlternateIteration
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    18630 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic_no-op
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9633 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_EOBTideWriteFrame.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    33198 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_ConstructEOSPosterior.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1597 2022-10-11 14:57:54.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_ILEdagPostprocess.sh
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8166 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/convert_output_format_inference2ile
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9065 2022-10-11 14:57:54.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/create_CIP_convergence_sequence.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3430 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_WriteFrameAndCacheFromXML.sh
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3665 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_ParameterRandomize.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3792 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_SimInspiralToCoinc.py
--rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    27796 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_FitAndEvaluate_GenericCoordinates.py
-drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-07 18:25:00.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT.egg-info/
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6991 2023-04-07 18:24:59.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT.egg-info/PKG-INFO
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        5 2023-04-07 18:24:59.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT.egg-info/top_level.txt
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    10419 2023-04-07 18:24:59.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT.egg-info/SOURCES.txt
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      142 2023-04-07 18:24:59.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT.egg-info/requires.txt
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        1 2023-04-07 18:24:59.000000 RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT.egg-info/dependency_links.txt
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)       38 2023-04-07 18:25:00.000000 RIFT-0.0.15.8rc6/setup.cfg
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1364 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/INSTALL_OPTIONAL_DEPENDENCIES.md
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      184 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc6/requirements.txt
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1042 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/AUTOMATED_OR_ONLINE.md
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3488 2022-09-24 12:18:48.000000 RIFT-0.0.15.8rc6/PACKAGING.md
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3557 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc6/INSTALL.md
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6991 2023-04-07 18:25:00.000000 RIFT-0.0.15.8rc6/PKG-INFO
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2934 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc6/setup.py
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1755 2022-11-28 22:41:57.000000 RIFT-0.0.15.8rc6/Dockerfile
--rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5821 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc6/README.md
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-16 18:25:20.000000 RIFT-0.0.15.8rc7/
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-16 18:25:19.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-16 18:25:19.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-16 18:25:20.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8109 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_LALCompareApproximantsOnSamples.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1224 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/convert_dat_to_hdf5.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      389 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_EstimateWaveformDuration.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9633 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_EOBTideWriteFrame.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6671 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_NRDumpDetectorResponse.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1597 2022-10-11 14:57:54.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_ILEdagPostprocess.sh
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2013 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/convert_psd_ascii2xml
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    14569 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/create_event_dag_via_grid
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8994 2022-10-11 14:57:54.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/convergence_test_samples.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2223 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_GridRecenter.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    20152 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/ile_postproc_add_time
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    99712 2023-04-16 18:23:39.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic_batchmode
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    35804 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_RIFT_pseudo_pipe_lowlatency.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    11254 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_TidalPlotSimulationStrain.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    40228 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_IterativeFisher.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2314 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_CoordinateNamesAngularToCartesianSpins.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      541 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/convert_output_format_ascii2h5.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1955 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_WriteXMLWithEOS.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2450 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_MassGridCoalesce.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3430 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_WriteFrameAndCacheFromXML.sh
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7195 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_MarginalizedLikelihoodEOSIntegralFromIntermediate.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3377 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_NR_GWMemory.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4982 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_TestSpokesIO.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2698 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_JoinXML.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1018 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_ILEROMdagPostprocess.sh
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5672 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_NRIndexedFminCutToILE.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    34265 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_AMRGrid.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      814 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_TestXMLParameterStorage.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    55368 2022-11-28 22:41:57.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_ConstructIntrinsicPosterior_GaussianResampling.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6780 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_InitMargTable
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8723 2022-10-11 14:57:54.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/assess_propose_CIP_convergence_sequence.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8821 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_NRBestOfIndex.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1529 2023-04-16 18:23:39.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/combine_weights_and_rejection_sample.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    33198 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_ConstructEOSPosterior.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3080 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_ResampleILEOutputWithExtrinsic.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2778 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_HyperCombine.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    88335 2022-10-11 14:57:54.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_AlternateIteration
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      853 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_ConsolidateDAGsUnderMaster.sh
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    37686 2023-03-12 13:15:08.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/plot_posterior_corner.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1640 2023-03-12 13:15:08.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_ForOSG_MakeTruncatedLocalFramesDir.sh
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3665 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_ParameterRandomize.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)   163149 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_ConstructIntrinsicPosterior_GenericCoordinates.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6162 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_GenerateMaxlnLWaveform_NRFromIndex.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)   117293 2023-04-16 18:23:39.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_BasicIteration
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3792 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_SimInspiralToCoinc.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    27796 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_FitAndEvaluate_GenericCoordinates.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1490 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_NRdagPostprocess.sh
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    33506 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/create_eos_posterior_pipeline
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3302 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_PrintInjection.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5408 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/make_uni_comov_skymap.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    11553 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_GenerateMaxlnLWaveform.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9065 2022-10-11 14:57:54.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/create_CIP_convergence_sequence.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3746 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/resample_uniform_comoving.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7660 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_LALWriteFrame.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    74024 2023-04-16 18:23:39.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_RIFT_pseudo_pipe.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8166 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/convert_output_format_inference2ile
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1590 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_HyperparameterGrid.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1087 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_PosteriorPostprocess.sh
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4553 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_IntermediateEOSIntegralFromFit.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    18630 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic_no-op
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    13919 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_GridSubsetOfTemplateBank.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1920 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/convert_output_format_allnet2xml
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    18544 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_AnalyticFisherGrid.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7587 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_TEOBResumSWriteFrame.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2349 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_ParameterFilter.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    12192 2023-04-16 18:23:39.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/calibration_reweighting.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6140 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/convergence_test_amr.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4794 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_NRRelabelILE.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      354 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/switcheroo
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2784 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_WriteInjectionFile.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    11799 2023-03-12 13:15:08.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/convert_output_format_ile2inference
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    96043 2023-04-16 18:23:39.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/helper_LDG_Events.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5424 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_RIFT_MultiMetaPipe.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    10752 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_NRNearestSimulationTo.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2768 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/create_ile_sub_dag.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7130 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_BatchConvertResampleILEOutput.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    20394 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_NRExtrudeOverlapGrid.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6293 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_ROMWriteFrame.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1436 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_CharacterizePosterior.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      829 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_ILENextGeneration.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5156 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_HyperparameterPuffball.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1028 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_CIPdagPostprocess.sh
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    12414 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_ParameterPuffball.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3696 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_AdaptiveExponent.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3266 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_FrameZeroNoiseSNR.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    83560 2023-03-12 13:15:08.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      256 2022-10-11 14:57:54.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_ForOSG_MakeLocalFramesDir.sh
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    13979 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/create_postprocessing_event_dag.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    15127 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_CompareWaveformsInDetectors.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      457 2022-10-15 00:56:03.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_TruncateMergeFrames.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      219 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_CacheFileConvert.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      876 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_CoincIFOUtility.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3250 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_FetchExternalGrid.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2800 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/config_yank.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3934 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_CleanILE.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1886 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/helper_OnlinePSDCleanup.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    50356 2022-10-11 14:57:54.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_ManualOverlapGrid.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1214 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_MassGrid.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    71601 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_BasicMultiApproxIteration
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9830 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_NRWriteFrame.py
+-rwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1675 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_RandomizeOverlapOrder.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    10380 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_ConstructBNSMarginalEOSRank.py
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-16 18:25:19.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT.egg-info/
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      142 2023-04-16 18:25:19.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT.egg-info/requires.txt
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6991 2023-04-16 18:25:19.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT.egg-info/PKG-INFO
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        5 2023-04-16 18:25:19.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT.egg-info/top_level.txt
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        1 2023-04-16 18:25:19.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT.egg-info/dependency_links.txt
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    10494 2023-04-16 18:25:19.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT.egg-info/SOURCES.txt
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-16 18:25:19.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)   241710 2023-04-16 18:23:39.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/lalsimutils.py
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-16 18:25:19.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/integrators/
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    28330 2023-04-16 18:23:39.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsamplerEnsemble.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7235 2022-10-24 14:00:10.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/integrators/statutils.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    53601 2023-03-12 13:15:08.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsampler.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2901 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/integrators/multivariate_truncnorm.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/integrators/__init__.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    20255 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/integrators/gaussian_mixture_model.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    33113 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/integrators/weighted_gmm.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2592 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/integrators/direct_quadrature.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    68867 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsamplerGPU.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    18724 2023-04-16 18:23:39.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/integrators/MonteCarloEnsemble.py
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-16 18:25:20.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/physics/
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    26126 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/physics/EOBTidalExternal.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    31276 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/physics/EOBTidalExternalC.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2654 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/physics/MonotonicSpline.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)       68 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/physics/__init__.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4664 2023-03-12 13:15:08.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/physics/GWSignal.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    23733 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/physics/effectiveFisher.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    63089 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/physics/EOSManager.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    52302 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/physics/ROMWaveformManager.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    19507 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/physics/PrecessingFisherMatrix.py
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-16 18:25:19.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/interpolators/
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    26826 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/interpolators/senni.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3835 2022-10-23 22:26:00.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/interpolators/ConstrainedQuadraticLikelihood.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5558 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/interpolators/internal_GP.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/interpolators/__init__.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3488 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/interpolators/interp_gpu.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2518 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/interpolators/gpytorch_wrapper.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2658 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/interpolators/efficient_save_sklearn_gp.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9944 2022-10-23 22:26:00.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/interpolators/BayesianLeastSquares.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1655 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/interpolators/gp.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      163 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/__init__.py
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-16 18:25:19.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/likelihood/
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/likelihood/__init__.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5269 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/likelihood/optimized_gpu_tools.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1525 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/likelihood/cuda_Q_inner_product.cu
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    94119 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/likelihood/factored_likelihood.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    33438 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/likelihood/SphericalHarmonics_gpu.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4706 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/likelihood/vectorized_lal_tools.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1643 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/likelihood/Q_inner_product.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     4007 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/likelihood/vectorized_general_tools.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1211 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/likelihood/priors_utils.py
+drwxrwxr-x   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)        0 2023-04-16 18:25:20.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/misc/
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    10915 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/misc/samples_utils.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     8657 2023-03-12 13:15:08.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/misc/xmlutils.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)   108901 2023-04-16 18:23:39.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/misc/dag_utils.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     9324 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/misc/modules.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    10623 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/misc/spokes.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)       65 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/misc/__init__.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6975 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/misc/tools.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2641 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/misc/weight_simulations.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    30542 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/misc/ourparams.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2901 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/misc/sky_rotations.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    23083 2022-10-11 14:57:54.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/misc/our_corner.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      229 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/misc/common_cl.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     7367 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/misc/bounded_kde.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    29427 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/misc/amrlib.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    70947 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/misc/ModifiedScikitFit.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3557 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/INSTALL.md
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1364 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/INSTALL_OPTIONAL_DEPENDENCIES.md
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1755 2022-11-28 22:41:57.000000 RIFT-0.0.15.8rc7/Dockerfile
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     5821 2023-04-07 18:24:37.000000 RIFT-0.0.15.8rc7/README.md
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6136 2022-09-24 12:18:48.000000 RIFT-0.0.15.8rc7/howto.md
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1042 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/AUTOMATED_OR_ONLINE.md
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6991 2023-04-16 18:25:20.000000 RIFT-0.0.15.8rc7/PKG-INFO
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     2934 2023-04-16 18:23:39.000000 RIFT-0.0.15.8rc7/setup.py
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      204 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/MANIFEST.in
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     3488 2022-09-24 12:18:48.000000 RIFT-0.0.15.8rc7/PACKAGING.md
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     1118 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/LICENSE.md
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)     6132 2022-09-24 12:18:48.000000 RIFT-0.0.15.8rc7/TROUBLESHOOTING.md
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)       38 2023-04-16 18:25:20.000000 RIFT-0.0.15.8rc7/setup.cfg
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)    22146 2022-09-24 12:18:47.000000 RIFT-0.0.15.8rc7/GETTING_STARTED.md
+-rw-rw-r--   0 richard.oshaughnessy (40428) richard.oshaughnessy (40428)      184 2023-03-24 18:44:03.000000 RIFT-0.0.15.8rc7/requirements.txt
```

### Comparing `RIFT-0.0.15.8rc6/LICENSE.md` & `RIFT-0.0.15.8rc7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/GETTING_STARTED.md` & `RIFT-0.0.15.8rc7/GETTING_STARTED.md`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/TROUBLESHOOTING.md` & `RIFT-0.0.15.8rc7/TROUBLESHOOTING.md`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/howto.md` & `RIFT-0.0.15.8rc7/howto.md`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/lalsimutils.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/lalsimutils.py`

 * *Files 0% similar despite different names*

```diff
@@ -3114,15 +3114,15 @@
 
 
 ## Version protection
 #   Pull out arguments of the ModesFromPolarizations function
 #argist_FromPolarizations=lalsim.SimInspiralTDModesFromPolarizations.__doc__.split('->')[0].replace('SimInspiralTDModesFromPolarizations','').replace('REAL8','').replace('Dict','').replace('Approximant','').replace('(','').replace(')','').split(',')
 
 
-def hlmoft(P, Lmax=2,nr_polarization_convention=False, fixed_tapering=False ):
+def hlmoft(P, Lmax=2,nr_polarization_convention=False, fixed_tapering=False, silent=True, **kwargs ):
     """
     Generate the TD h_lm -2-spin-weighted spherical harmonic modes of a GW
     with parameters P. Returns a SphHarmTimeSeries, a linked-list of modes with
     a COMPLEX16TimeSeries and indices l and m for each node.
 
     The linked list will contain all modes with l <= Lmax
     and all values of m for these l.
@@ -3140,29 +3140,33 @@
     if (P.approx == lalIMRPhenomHM or P.approx == lalIMRPhenomXHM or P.approx == lalIMRPhenomXPHM or P.approx == lalSEOBNRv4HM_ROM or check_FD_pending(P.approx)) and is_ChooseFDModes_present:
        if P.fref==0 and (P.approx == lalIMRPhenomXPHM):
           P.fref=P.fmin
        extra_params = P.to_lal_dict()
        fNyq = 0.5/P.deltaT
        TDlen = int(1./(P.deltaT*P.deltaF))
        fNyq_offset = fNyq - P.deltaF
+       # Argh: https://git.ligo.org/waveforms/reviews/imrphenomxhm-amplitude-recalibration/-/wikis/home#review-statement
+       if P.approx == lalIMRPhenomXPHM and 'release' in kwargs:
+           lalsim.SimInspiralWaveformParamsInsertPhenomXHMReleaseVersion(extra_params, kwargs['release'])
        hlms_struct = lalsim.SimInspiralChooseFDModes(P.m1, P.m2, \
                                                      P.s1x, P.s1y, P.s1z, \
                                                      P.s2x, P.s2y, P.s2z, \
                                                      P.deltaF, P.fmin, fNyq, P.fref, P.phiref, P.dist, P.incl, extra_params, P.approx)
        hlmsT = {}
        hlms = {}
        hlmsdict = SphHarmFrequencySeries_to_dict(hlms_struct,Lmax)
        for mode in hlmsdict:
           hlmsdict[mode] = lal.ResizeCOMPLEX16FrequencySeries(hlmsdict[mode],0, TDlen)
           hlmsT[mode] = DataInverseFourier(hlmsdict[mode])
           hlmsT[mode].data.data = -1*hlmsT[mode].data.data
           hlmsT[mode].data.data = np.roll(hlmsT[mode].data.data,-int(hlmsT[mode].data.length/2))
           hlmsT[mode].epoch = -(hlmsT[mode].data.length*hlmsT[mode].deltaT/2)
        if P.deltaF is not None:
-          print(hlmsT[mode].data.length,TDlen, " and in seconds ", hlmsT[mode].data.length*hlmsT[mode].deltaT,TDlen*P.deltaT, " with deltaT={} {}".format(hlmsT[mode].deltaT,P.deltaT))
+          if not silent:
+              print(hlmsT[mode].data.length,TDlen, " and in seconds ", hlmsT[mode].data.length*hlmsT[mode].deltaT,TDlen*P.deltaT, " with deltaT={} {}".format(hlmsT[mode].deltaT,P.deltaT))
           for mode in hlmsT:
              hlms[mode] = lal.ResizeCOMPLEX16TimeSeries(hlmsT[mode],0,TDlen)
        return hlms
 
     if (P.approx == lalsim.SEOBNRv2 or P.approx == lalsim.SEOBNRv1 or P.approx == lalSEOBv4 or P.approx==lalsim.SEOBNRv4_opt or P.approx == lalsim.EOBNRv2 or P.approx == lalTEOBv2 or P.approx==lalTEOBv4 or P.approx == lalSEOBNRv4HM):
         hlm_out = hlmoft_SEOB_dict(P,Lmax=Lmax)
         if True: #not (P.taper == lsu_TAPER_NONE): #True: #P.taper:
```

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/integrators/statutils.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/integrators/statutils.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/integrators/MonteCarloEnsemble.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/integrators/MonteCarloEnsemble.py`

 * *Files 2% similar despite different names*

```diff
@@ -250,28 +250,30 @@
         
             # calculate the effective samples
             self.total_value += summed_vals
             self.max_value = max(scale_factor, self.max_value)
             self.eff_samp = self.total_value / self.max_value
         else: # using lnI return values
             # Evaluate integral and effective sample count
-            log_sum_weights = logsumexp(log_weights) - log_scale_factor
+            # Note with lnI return values, no more need to keep track of a scale factor at all
+            log_sum_weights = logsumexp(log_weights) 
             log_integral_here = log_sum_weights - np.log(self.n)
             if not(self.integral ):
-                self.integral = log_integral_here + log_scale_factor
-                self.total_value = log_sum_weights +log_scale_factor
+                self.integral = log_integral_here  
+                self.total_value = log_sum_weights  
                 self.max_value = log_scale_factor
             else:
                 self.integral = logsumexp([ self.integral +np.log(self.iterations), log_integral_here]) - np.log(self.iterations+1)
-                self.total_value= logsumexp([self.total_value, log_sum_weights+log_scale_factor])
-                self.max_value = np.max([self.max_value,log_scale_factor])
+                self.total_value= logsumexp([self.total_value, log_sum_weights])
+                self.max_value = np.max([self.max_value,np.max(log_weights)])
             self.eff_samp = np.exp(self.total_value - (self.max_value  ))
 
             # Evaluate error squared, avoiding overflow
-            log_scaled_error_squared = np.log(np.var(np.exp(log_weights - log_scale_factor)))
+            tmp_max = np.max(log_weights)
+            log_scaled_error_squared = np.log(np.var(np.exp(log_weights - tmp_max))) + 2*tmp_max   - np.log(self.n)
             if not(self.scaled_error_squared):
                 self.scaled_error_squared = log_scaled_error_squared
             else:
                 self.scaled_error_squared = logsumexp([ self.scaled_error_squared + np.log(self.iterations), log_scaled_error_squared]) - np.log(self.iterations+1)
 
     def _reset(self):
         ### reset GMMs
@@ -357,15 +359,18 @@
                 print(traceback.format_exc())
                 print('Error calculating results, resetting...')
                 err_count += 1
                 self._reset()
                 continue
             self.iterations += 1
             self.ntotal += self.n
-            if self.iterations >= min_iter and np.log(self.scaled_error_squared) + self.log_error_scale_factor < np.log(var_thresh):
+            testval =self.scaled_error_squared
+            if not(self.return_lnI):
+                testval = np.log(self.scaled_error_squared) + self.log_error_scale_factor
+            if self.iterations >= min_iter and testval < np.log(var_thresh):
                 break
             try:
                 if adapting:
                     self._train()
             except KeyboardInterrupt:
                 print('KeyboardInterrupt, exiting...')
                 break
@@ -381,12 +386,12 @@
                     if self.gmm_dict[k] is not None:
                         self.gmm_dict[k].print_params()
             if epoch is not None and self.iterations % epoch == 0:
                 self._reset()
             if verbose:
                 # Standard mcsampler message, to monitor convergence
                 if not(self.return_lnI):
-                    print(" : {} {} {} {} {} ".format((self.iterations-1)*self.n, self.eff_samp, np.sqrt(2*np.max(self.cumulative_values)), np.sqrt(2*np.log(self.integral)), "-" ) )
+                    print(" : {} {} {} {} {} ".format((self.iterations-1)*self.n, self.eff_samp, np.sqrt(2*np.max(self.cumulative_values)), np.sqrt(2*(np.log(self.integral))),  np.sqrt(self.scaled_error_squared )/self.integral/np.sqrt(self.iterations ) ) )
                 else:
-                    print(" : {} {} {} {} {} ".format((self.iterations-1)*self.n, self.eff_samp, np.sqrt(2*np.max(self.cumulative_values)), np.sqrt(2*self.integral), "-" ) )
+                    print(" : {} {} {} {} {} ".format((self.iterations-1)*self.n, self.eff_samp, np.sqrt(2*np.max(self.cumulative_values)), np.sqrt(2*self.integral), np.exp(0.5*(self.scaled_error_squared - self.integral*2) )/np.sqrt(self.iterations)))
         print('cumulative eval time: ', cumulative_eval_time)
         print('integrator iterations: ', self.iterations)
```

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsamplerGPU.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsamplerGPU.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsampler.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsampler.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/integrators/weighted_gmm.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/integrators/weighted_gmm.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/integrators/direct_quadrature.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/integrators/direct_quadrature.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/integrators/multivariate_truncnorm.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/integrators/multivariate_truncnorm.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/integrators/gaussian_mixture_model.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/integrators/gaussian_mixture_model.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsamplerEnsemble.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/integrators/mcsamplerEnsemble.py`

 * *Files 2% similar despite different names*

```diff
@@ -327,15 +327,19 @@
         integrator.integrate(func, min_iter=min_iter, max_iter=max_iter, var_thresh=var_thresh, neff=neff, nmax=nmax,max_err=max_err,verbose=verbose,progress=super_verbose,tripwire_fraction=tripwire_fraction,tripwire_epsion=tripwire_epsilon,use_lnL=use_lnL,return_lnI=return_lnI)
 
         # get results
 
         self.n = int(integrator.n)
         self.ntotal = int(integrator.ntotal)
         integral = integrator.integral
-        error_squared = integrator.scaled_error_squared * np.exp(integrator.log_error_scale_factor)
+        print("Result ",integrator.scaled_error_squared, integrator.integral)
+        if not(return_lnI):
+            error_squared = integrator.scaled_error_squared * np.exp(integrator.log_error_scale_factor)/ (self.ntotal/self.n)
+        else:
+            error_squared = integrator.scaled_error_squared  - np.log(self.ntotal/self.n)
         eff_samp = integrator.eff_samp
         sample_array = integrator.cumulative_samples
         if not(return_lnI):
             value_array = np.exp(integrator.cumulative_values)  # stored as ln(integrand) !
         else:
             value_array = integrator.cumulative_values
         p_array = integrator.cumulative_p_s
```

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/interpolators/senni.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/interpolators/senni.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/interpolators/ConstrainedQuadraticLikelihood.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/interpolators/ConstrainedQuadraticLikelihood.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/interpolators/gp.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/interpolators/gp.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/interpolators/interp_gpu.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/interpolators/interp_gpu.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/interpolators/BayesianLeastSquares.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/interpolators/BayesianLeastSquares.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/interpolators/internal_GP.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/interpolators/internal_GP.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/interpolators/efficient_save_sklearn_gp.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/interpolators/efficient_save_sklearn_gp.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/interpolators/gpytorch_wrapper.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/interpolators/gpytorch_wrapper.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/physics/ROMWaveformManager.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/physics/ROMWaveformManager.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/physics/EOBTidalExternalC.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/physics/EOBTidalExternalC.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/physics/MonotonicSpline.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/physics/MonotonicSpline.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/physics/EOBTidalExternal.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/physics/EOBTidalExternal.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/physics/PrecessingFisherMatrix.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/physics/PrecessingFisherMatrix.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/physics/effectiveFisher.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/physics/effectiveFisher.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/physics/GWSignal.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/physics/GWSignal.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/physics/EOSManager.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/physics/EOSManager.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/modules.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/misc/modules.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/bounded_kde.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/misc/bounded_kde.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/weight_simulations.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/misc/weight_simulations.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/amrlib.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/misc/amrlib.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/our_corner.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/misc/our_corner.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/xmlutils.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/misc/xmlutils.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/samples_utils.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/misc/samples_utils.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/ourparams.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/misc/ourparams.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/sky_rotations.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/misc/sky_rotations.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/spokes.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/misc/spokes.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/tools.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/misc/tools.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/ModifiedScikitFit.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/misc/ModifiedScikitFit.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/misc/dag_utils.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/misc/dag_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -875,14 +875,23 @@
 #    if use_cvmfs_frames:
 #        transfer_files += ["../local.cache"]
     # To change interactively:
     #   condor_qedit
     # for example: 
     #    for i in `condor_q -hold  | grep oshaughn | awk '{print $1}'`; do condor_qedit $i RequestMemory 30000; done; condor_release -all 
 
+    # Avoid undesirable hosts in RIFT_AVOID_HOSTS
+    if 'RIFT_AVOID_HOSTS' in os.environ:
+        line = os.environ['RIFT_AVOID_HOSTS']
+        line = line.rstrip()
+        if line:
+            name_list = line.split(',')
+            for name in name_list:
+                requirements.append('TARGET.Machine =!= "{}" '.format(name))
+
     # Write requirements
     # From https://github.com/lscsoft/lalsuite/blob/master/lalinference/python/lalinference/lalinference_pipe_utils.py
     ile_job.add_condor_cmd('requirements', '&&'.join('({0})'.format(r) for r in requirements))
 
     try:
         ile_job.add_condor_cmd('accounting_group',os.environ['LIGO_ACCOUNTING'])
         ile_job.add_condor_cmd('accounting_group_user',os.environ['LIGO_USER_NAME'])
@@ -1967,15 +1976,17 @@
     #
     # Add mandatory options
     ile_job.add_opt('data_dump_file', str(pickle_file))
     ile_job.add_opt('posterior_sample_file', str(posterior_file))
     ile_job.add_opt('number_of_calibration_curves', '100')
     ile_job.add_opt('reevaluate_likelihood', 'True')
     ile_job.add_opt('use_rift_samples', 'True')
-    ile_job.add_opt('time_marginalization', str(time_marg))
+    if time_marg:
+        # problem with this argument: 'False' is often parsed as 'True' by argparsing (weird). Default is 'false'
+        ile_job.add_opt('time_marginalization', str(time_marg))
 
     lmax=None
     if ile_args:
         ile_args_split = ile_args.split('--')
         fmin_list = []
         fmin_template = None
         for line in ile_args_split:
@@ -1985,15 +1996,15 @@
                     fmin_list += [line_split[1]]
                 if line_split[0] == 'fmin-template':
                     fmin_template = line_split[1]
                 elif line_split[0] == 'l-max':
                     lmax = int(line_split[1])
 #        fmin = np.min(fmin_list)
         if fmin_template:
-            ile_job.add_arg(" --fmin-template {} ".format(fmin_template))  # code will fail without this, and it is always written anyways, but 
+            ile_job.add_arg(" --fmin {} ".format(fmin_template))  # code will fail without this, and it is always written anyways, but 
         if lmax:
             ile_job.add_arg(" --l-max {} ".format(lmax))
 
     #
     # Add normal arguments
     #
     for opt, param in list(kwargs.items()):
@@ -2080,21 +2091,21 @@
     # Workaround: https://stackoverflow.com/questions/2885190/using-configparser-to-read-a-file-without-section-name
     config = configparser.ConfigParser()
     config.optionxform=str # force preserve case! Important for --choose-data-LI-seglen
     with open(bilby_ini_file) as stream:
         config.read_string("[top]\n" + stream.read())
         bilby_items = dict(config["top"])
         ifo_list = list(bilby_items['channel-dict'])  # PSDs must be listed, implicitly provides all ifos
-    bilby_data_dict = {}
     # remove entries with the None keyword, as misleading
-    dict_names = list(bilby_data_dict)
+    dict_names = list(bilby_items)
     for name in dict_names:
-        if bilby_data_dict[name] == 'None':
-            del bilby_data_dict[name]
+        if bilby_items[name] == 'None':
+            del bilby_items[name]
     if not('data-dict' in bilby_items):
+        bilby_data_dict = {}
         if cache_file:
             print(" calmarg: bilby ini file does not have data_dict, attempting to identify data from (host) directory: {} ".format(frames_dir))
             cache_lines = np.loadtxt(cache_file,dtype=str)
             if len(cache_lines) > len(ifo_list):
                 raise Exception(" Pipeline failure: cache file must contain one line per IFO to identify files in this approach")
             for indx in np.arange(len(cache_lines)):
                 ifo = cache_lines[indx][0]+"1"
@@ -2116,15 +2127,15 @@
             print(" ==== WARNING FALLTHROUGH : calmarg attempting to identify correct frame files to use but falling back to 'magic' options from bilby ===")
         # add to command-line arguments, IF NONEMPTY.  Otherwise we're stuck, and we have to hope magic works
         if len(list(bilby_data_dict))>0:
             data_argstr = '{}'.format(bilby_data_dict)
             data_argstr = '  --data-dict ""{}""  '.format(data_argstr.replace(' ',''))  # double "" because we are in a condor submit script!  Annoying but seemt to be correct
             ile_job.add_arg(data_argstr)
         else:
-            print(" ==== WARNING FALLTHROUGH : calmarg failed to pull out options  ===",bilby_data_dict)
+            print(" ==== WARNING FALLTHROUGH : calmarg failed to pull out options  ===",bilby_data_dict,bilby_items)
 
 
     # Other required settings from ILE
     # approximant: if ile_args present, ALWAYS parse it and set it that way, so we are consistent with our own analysis
     if ile_args:
         approx = bilby_items['waveform-approximant']
         ile_args_split = ile_args.split('--')
```

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/likelihood/Q_inner_product.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/likelihood/Q_inner_product.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/likelihood/optimized_gpu_tools.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/likelihood/optimized_gpu_tools.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/likelihood/priors_utils.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/likelihood/priors_utils.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/likelihood/SphericalHarmonics_gpu.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/likelihood/SphericalHarmonics_gpu.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/likelihood/vectorized_general_tools.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/likelihood/vectorized_general_tools.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/likelihood/vectorized_lal_tools.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/likelihood/vectorized_lal_tools.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/likelihood/factored_likelihood.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/likelihood/factored_likelihood.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT/likelihood/cuda_Q_inner_product.cu` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT/likelihood/cuda_Q_inner_product.cu`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_AMRGrid.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_AMRGrid.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_HyperCombine.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_HyperCombine.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_NRNearestSimulationTo.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_NRNearestSimulationTo.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_ILEROMdagPostprocess.sh` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_ILEROMdagPostprocess.sh`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_FetchExternalGrid.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_FetchExternalGrid.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_NRDumpDetectorResponse.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_NRDumpDetectorResponse.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_ConstructIntrinsicPosterior_GenericCoordinates.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_ConstructIntrinsicPosterior_GenericCoordinates.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/convert_output_format_ile2inference` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/convert_output_format_ile2inference`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_JoinXML.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_JoinXML.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_ManualOverlapGrid.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_ManualOverlapGrid.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_ResampleILEOutputWithExtrinsic.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_ResampleILEOutputWithExtrinsic.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_CharacterizePosterior.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_CharacterizePosterior.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_GenerateMaxlnLWaveform_NRFromIndex.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_GenerateMaxlnLWaveform_NRFromIndex.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/config_yank.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/config_yank.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_InitMargTable` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_InitMargTable`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_AnalyticFisherGrid.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_AnalyticFisherGrid.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_NR_GWMemory.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_NR_GWMemory.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/calibration_reweighting.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/calibration_reweighting.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,14 +118,19 @@
             'a2x':'spin_2x', 'a2y':'spin_2y', 'a2z':'spin_2z', 'incl':'iota', 'time':'geocent_time',
         'phiorb':'phase', 'p':'log_prior', 'distance':'luminosity_distance', 'lambda1':'lambda_1', 'lambda2':'lambda_2'}
 
         for old_key in result.posterior.keys():
             if old_key in key_swap_dict:
                 result.posterior[key_swap_dict[old_key]] = result.posterior[old_key]
                 del result.posterior[old_key]
+        # add tides if not present
+        if not('lambda_1' in result.posterior):
+            print(" Populating empty tidal params to avoid hang")
+            result.posterior['lambda_1'] = np.zeros(end_index-start_index)
+            result.posterior['lambda_2'] = np.zeros(end_index-start_index)
 
 outdir = os.path.dirname(os.path.abspath(args.posterior_sample_file))
 
 ifos = data.interferometers
 time_marginalization_interval = args.time_marginalization_interval
 
 spline_calibration_envelope_dict = bilby_pipe.utils.convert_string_to_dict(
```

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_FrameZeroNoiseSNR.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_FrameZeroNoiseSNR.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_ForOSG_MakeTruncatedLocalFramesDir.sh` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_ForOSG_MakeTruncatedLocalFramesDir.sh`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_AdaptiveExponent.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_AdaptiveExponent.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_WriteInjectionFile.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_WriteInjectionFile.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_RIFT_MultiMetaPipe.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_RIFT_MultiMetaPipe.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_GridRecenter.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_GridRecenter.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_IterativeFisher.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_IterativeFisher.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/assess_propose_CIP_convergence_sequence.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/assess_propose_CIP_convergence_sequence.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_CompareWaveformsInDetectors.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_CompareWaveformsInDetectors.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/create_postprocessing_event_dag.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/create_postprocessing_event_dag.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_ParameterPuffball.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_ParameterPuffball.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_CIPdagPostprocess.sh` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_CIPdagPostprocess.sh`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/helper_OnlinePSDCleanup.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/helper_OnlinePSDCleanup.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/resample_uniform_comoving.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/resample_uniform_comoving.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_RandomizeOverlapOrder.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_RandomizeOverlapOrder.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_PosteriorPostprocess.sh` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_PosteriorPostprocess.sh`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_MarginalizedLikelihoodEOSIntegralFromIntermediate.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_MarginalizedLikelihoodEOSIntegralFromIntermediate.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_ILENextGeneration.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_ILENextGeneration.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_GenerateMaxlnLWaveform.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_GenerateMaxlnLWaveform.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/create_ile_sub_dag.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/create_ile_sub_dag.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_TestSpokesIO.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_TestSpokesIO.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_LALCompareApproximantsOnSamples.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_LALCompareApproximantsOnSamples.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_WriteXMLWithEOS.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_WriteXMLWithEOS.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_ConstructIntrinsicPosterior_GaussianResampling.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_ConstructIntrinsicPosterior_GaussianResampling.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_ConstructBNSMarginalEOSRank.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_ConstructBNSMarginalEOSRank.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_ROMWriteFrame.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_ROMWriteFrame.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_RIFT_pseudo_pipe_lowlatency.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_RIFT_pseudo_pipe_lowlatency.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_BasicMultiApproxIteration` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_BasicMultiApproxIteration`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_NRBestOfIndex.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_NRBestOfIndex.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_NRExtrudeOverlapGrid.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_NRExtrudeOverlapGrid.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_RIFT_pseudo_pipe.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_RIFT_pseudo_pipe.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,14 +116,15 @@
 parser.add_argument("--use-ini",default=None,type=str,help="Pass ini file for parsing. Intended to reproduce lalinference_pipe functionality. Overrides most other arguments. Full path recommended")
 parser.add_argument("--use-rundir",default=None,type=str,help="Intended to reproduce lalinference_pipe functionality. Must be absolute path.")
 parser.add_argument("--use-online-psd-file",default=None,type=str,help="Provides specific online PSD file, so no downloads are needed")
 parser.add_argument("--use-coinc",default=None,type=str,help="Intended to reproduce lalinference_pipe functionality")
 parser.add_argument("--manual-ifo-list",default=None,type=str,help="Overrides IFO list normally retrieve by event ID.  Use with care (e.g., glitch studies) or for events specified with --event-time.")
 parser.add_argument("--online",action='store_true')
 parser.add_argument("--calibration-reweighting",action='store_true',help="Option to add job to DAG to reweight posterior samples due to calibration uncertainty.")
+parser.add_argument("--calibration-reweighting-batchsize",type=int,default=None,help="If not 'None', tries to group the final set of points based on jobs of a fixed size")
 parser.add_argument("--distance-reweighting",action='store_true',help="Option to add job to DAG to reweight posterior samples due to different distance prior (LVK prod prior)")
 parser.add_argument("--extra-args-helper",action=None, help="Filename with arguments for the helper. Use to provide alternative channel names and other advanced configuration (--channel-name, data type)!")
 parser.add_argument("--manual-postfix",default='',type=str)
 parser.add_argument("--gracedb-id",default=None,type=str)
 parser.add_argument("--gracedb-exe",default="gracedb")
 parser.add_argument("--use-legacy-gracedb",action='store_true')
 parser.add_argument("--internal-use-gracedb-bayestar",action='store_true',help="Retrieve BS skymap from gracedb (bayestar.fits), and use it internally in integration with --use-skymap bayestar.fits.")
@@ -829,17 +830,23 @@
     #     n_max_cip *=3   # it is faster, so run longer; helps with correlated-sampling cases
     n_sample_target=opts.n_output_samples
     if indx < len(instructions_cip)-1: # on all but last iteration, cap the number of points coming out : this drives the total amount of work for AMR, etc!
         n_sample_target= np.min([opts.n_output_samples,10*opts.internal_cip_cap_neff])
     n_workers = 1
     if opts.cip_explode_jobs:
         n_workers = opts.cip_explode_jobs
-    n_eff_cip_here = int(n_sample_target/n_workers)
+    n_workers_last =n_workers
+    if opts.cip_explode_jobs_last:
+        n_workers_last = opts.cip_explode_jobs_last
+    n_eff_cip_last = int(n_sample_target/n_workers_last)
     if indx < len(instructions_cip)-1: # on all but 
+        n_eff_cip_here= int(n_sample_target/n_workers)
         n_eff_cip_here = np.amin([opts.internal_cip_cap_neff/n_workers + 1, n_eff_cip_here]) # n_eff: make sure to do *less* than the limit. Lowering this saves immensely on internal/exploration runtime
+    else:
+        n_eff_cip_here = n_eff_cip_last
     n_sample_min_per_worker = int(n_eff_cip_here/100)+2  # need at least 2 samples, and don't have any worker fall down on the job too much compared to the target
 
     # Analyze the iteration report
     n_eff_expected_max_easy = 1e-2 * n_max_cip
     n_eff_expected_max_hard = 1e-7 * n_max_cip
     print( " cip iteration group {} : n_eff likely will be between {} and {}, you are asking for at least {} and targeting {}".format(indx,n_eff_expected_max_easy, n_eff_expected_max_hard, n_sample_min_per_worker,n_eff_cip_here))
 
@@ -1092,14 +1099,16 @@
     cmd += " --ile-runtime-max-minutes {} ".format(opts.ile_runtime_max_minutes)
 if not(opts.internal_use_amr) or opts.internal_use_amr_puff:
     cmd+= " --puff-exe `which util_ParameterPuffball.py` --puff-cadence 1 --puff-max-it " + str(puff_max_it)+ " --puff-args `pwd`/args_puff.txt "
 if opts.assume_eccentric:
     cmd += " --use-eccentricity "
 if opts.calibration_reweighting and (not opts.bilby_pickle_file):
     cmd += " --calibration-reweighting --calibration-reweighting-exe `which calibration_reweighting.py` --bilby-ini-file {} --bilby-pickle-exe `which bilby_pipe_generation` ".format(str(opts.bilby_ini_file))
+    if opts.calibration_reweighting_batchsize:
+        cmd += " --calibration-reweighting-batchsize {} ".format(opts.calibration_reweighting_batchsize)
 elif opts.calibration_reweighting and opts.bilby_pickle_file:
     cmd += " --calibration-reweighting --calibration-reweighting-exe `which calibration_reweighting.py` --bilby-pickle-file {} ".format(str(opts.bilby_pickle_file))
 
 if opts.distance_reweighting:
     cmd += " --comov-distance-reweighting --comov-distance-reweighting-exe `which make_uni_comov_skymap.py` --convert-ascii2h5-exe `which convert_output_format_ascii2h5.py` "
 if opts.use_gauss_early:
     cmd += " --cip-exe-G `which util_ConstructIntrinsicPosterior_GaussianResampling.py ` "
```

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_CleanILE.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_CleanILE.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_MassGrid.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_MassGrid.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_NRdagPostprocess.sh` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_NRdagPostprocess.sh`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/make_uni_comov_skymap.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/make_uni_comov_skymap.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_NRIndexedFminCutToILE.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_NRIndexedFminCutToILE.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_CoordinateNamesAngularToCartesianSpins.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_CoordinateNamesAngularToCartesianSpins.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/plot_posterior_corner.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/plot_posterior_corner.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic_batchmode` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic_batchmode`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import numpy as np
 import os
 try:
   import cupy
   xpy_default=cupy
   identity_convert = cupy.asnumpy
   identity_convert_togpu = cupy.asarray
+  identity_convert_lnL= identity_convert # see later, will be assigned something different if cupy active AND AC  AND gpu
   junk_to_check_installed = cupy.array(5)  # this will fail if GPU not installed correctly
   if not('RIFT_LOWLATENCY' in os.environ):
     print(cupy.show_config())  # print provenance/debugging information
 
     # Check memory allocation
     mem_info = cupy.cuda.Device().mem_info  # memory available in bytes
     n_mb_total = mem_info[1]/1024./1024.
@@ -34,14 +35,15 @@
   cupy_success=True
 except:
   print( ' no cupy')
 #  import numpy as cupy  # will automatically replace cupy calls with numpy!
   xpy_default=numpy  # just in case, to make replacement clear and to enable override
   identity_convert = lambda x: x  # trivial return itself
   identity_convert_togpu = lambda x: x
+  identity_convert_lnL= lambda x:x # see later
   cupy_success=False
 
 import lal
 from ligo.lw import utils, lsctables, table, ligolw
 from ligo.lw.utils import process
 import glue.lal
 
@@ -300,14 +302,18 @@
 #
 # Failure modes
 #
 ok_lnL_methods = ['GMM', 'adaptive_cartesian', 'adaptive_cartesian_gpu']
 if opts.internal_use_lnL and not(opts.sampler_method  in ok_lnL_methods ):
   print(" OPTION MISMATCH : --internal-use-lnL not compatible with", opts.sampler_method, " can only use ", ok_lnL_methods)
   sys.exit(99)
+# if we are on a GPU and using a GPU-accelerated likelihood, don't send the likelihood data back from the GPU needlessly
+if cupy_success and opts.gpu and opts.sampler_method == 'adaptive_cartesian_gpu':
+  identity_convert_lnL  = lambda x:x
+
 
 if opts.resample_time_marginalization:
   import scipy.special
 if opts.resample_time_marginalization and not(opts.fairdraw_extrinsic_output):
   raise Exception(" Resampled time output requires --fairdraw-extrinsic-output ")
 
 # Fairdraw is NOT YET IMPLEMENTED for these other integrators!
@@ -1299,16 +1305,16 @@
 
                 lnL = factored_likelihood.DiscreteFactoredLogLikelihoodViaArrayVectorNoLoop(tvals,
                         P, lookupNKDict, rholmArrayDict, ctUArrayDict, ctVArrayDict,epochDict,Lmax=opts.l_max,xpy=xpy_default)
 #                nEvals +=len(right_ascension)
                 if supplemental_ln_likelihood:
                   lnL += supplemental_ln_likelihood(P.phi, P.theta, P.phiref ,P.incl, P.psi, P.dist,xpy=xpy_default) # use these variables so they are already float-type
                 if return_lnL:
-                  return lnL -manual_avoid_overflow_logarithm
-                return identity_convert(xpy_default.exp(lnL-manual_avoid_overflow_logarithm))
+                  return identity_convert_lnL(lnL -manual_avoid_overflow_logarithm)
+                return identity_convert_lnL(xpy_default.exp(lnL-manual_avoid_overflow_logarithm))
             else:
               print( " Using direct distance marginalization  ")
               xmin = factored_likelihood.distMpcRef / dmax
               xmax = factored_likelihood.distMpcRef / dmin
               bmax = xpy_default.asarray(lookup_table["bmax"])
               sqrt_bmax = xpy_default.sqrt(bmax)
               bref = xpy_default.asarray(lookup_table["bref"])
@@ -1401,16 +1407,16 @@
 
                   lnL = factored_likelihood.DiscreteFactoredLogLikelihoodViaArrayVectorNoLoop(tvals,
                     P, lookupNKDict, rholmArrayDict, ctUArrayDict, ctVArrayDict,epochDict,Lmax=opts.l_max,xpy=xpy_default, loglikelihood=distmarg_loglikelihood, phase_marginalization=True)
 #                  nEvals +=len(right_ascension)
                   if supplemental_ln_likelihood:
                     lnL += supplemental_ln_likelihood(P.phi, P.theta, P.phiref ,P.incl, P.psi, 0,xpy=xpy_default) # Same API
                   if return_lnL:
-                    return lnL -manual_avoid_overflow_logarithm
-                  return identity_convert(xpy_default.exp(lnL-manual_avoid_overflow_logarithm))
+                    return identity_convert_lnL(lnL -manual_avoid_overflow_logarithm)
+                  return identity_convert_lnL(xpy_default.exp(lnL-manual_avoid_overflow_logarithm))
 
               else:
 
                 def likelihood_function(right_ascension, declination, phi_orb, inclination, psi):
 #                  global nEvals
                   tvals = xpy_default.linspace(-t_ref_wind,t_ref_wind,int((t_ref_wind)*2/P.deltaT))  # choose an array at the target sampling rate. P is inherited globally
                   P.phi = xpy_default.asarray(right_ascension, dtype=np.float64)  # cast to float
@@ -1444,16 +1450,16 @@
 
                   lnL = factored_likelihood.DiscreteFactoredLogLikelihoodViaArrayVectorNoLoop(tvals,
                     P, lookupNKDict, rholmArrayDict, ctUArrayDict, ctVArrayDict,epochDict,Lmax=opts.l_max,xpy=xpy_default, loglikelihood=distmarg_loglikelihood)
 #                  nEvals +=len(right_ascension)
                   if supplemental_ln_likelihood:
                     lnL += supplemental_ln_likelihood(P.phi, P.theta, P.phiref ,P.incl, P.psi, 0,xpy=xpy_default) # Same API
                   if return_lnL:
-                    return lnL -manual_avoid_overflow_logarithm
-                  return identity_convert(xpy_default.exp(lnL-manual_avoid_overflow_logarithm))
+                    return identity_convert_lnL(lnL -manual_avoid_overflow_logarithm)
+                  return identity_convert_lnL(xpy_default.exp(lnL-manual_avoid_overflow_logarithm))
 
      else: # integrate over intrinsic variables. Right now those variables ahave HARDCODED NAMES, alas
         def likelihood_function(right_ascension, declination, phi_orb, inclination,
                 psi, distance,q):
             dec = numpy.copy(declination).astype(numpy.float64)
             if opts.declination_cosine_sampler:
                 dec = numpy.pi/2 - numpy.arccos(dec)
@@ -1760,19 +1766,25 @@
     fname_output_txt = opts.output_file +"_"+str(indx)+"_" + ".dat"
     open(fname_output_txt,'a').close()  # create empty file
   if opts.internal_hard_fail_on_error:
     sys.exit(1)
 #  if len(exception_failure) >0:
 #    if "CUBLAS" in exception_failure[0]:  # Hard fail if a cuda error!
 #      sys.exit(1) 
-  if ("CUDA" in str(exception_failure)) or ('CUBLAS' in str(exception_failure)): # Hard fail if a cuda error with a catchable error code
+  if ("CUDA" in str(exception_failure)) or ('CUBLAS' in str(exception_failure) or ('cuda' in str(exception_failure))): # Hard fail if a cuda error with a catchable error code
     sys.exit(62)
+  if 'Out of memory' in str(exception_failure):   # should never happen, most likely a crappy node or failure to set correct memory limit for ILE.
+    sys.exit(63)
   str_err = " {} ".format(exception_failure)
-  if 'Zero prior failure' in str_err:
+  if ('Zero prior failure' in str_err) or ('effective samples' in str_err):
+    # common failures that require reset of sampler
+    #    - zero prior : very rare case where the prior is exactly zero for some reason. User error most likely (floors, etc). Should never happen
+    #    - effective samples = nan : error with AC where the integrator gets confused. Reset
     # reset all variables sampling, so we don't contaminate subsequent versions
+    #    - again, this should only be a problem if we are using multiply adaptive sampling, so it should NEVER happen on the first time through
     for name in sampler.params:
       sampler.reset_sampling(param)
 
   #a sketch of how I would do custom failure modes, but for sake of speed I'm just setting the above right now
   #for i,failure_mode in enumerate(opts.custom_fails):
   #  if failure_mode in str(exception_failure):
   #    sys.exit(opts.custom_fail_codes[i])
```

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_TEOBResumSWriteFrame.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_TEOBResumSWriteFrame.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_HyperparameterPuffball.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_HyperparameterPuffball.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_PrintInjection.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_PrintInjection.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_LALWriteFrame.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_LALWriteFrame.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_CoincIFOUtility.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_CoincIFOUtility.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_NRWriteFrame.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_NRWriteFrame.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_BatchConvertResampleILEOutput.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_BatchConvertResampleILEOutput.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/convergence_test_amr.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/convergence_test_amr.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/convert_psd_ascii2xml` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/convert_psd_ascii2xml`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_TidalPlotSimulationStrain.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_TidalPlotSimulationStrain.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/ile_postproc_add_time` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/ile_postproc_add_time`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_TestXMLParameterStorage.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_TestXMLParameterStorage.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/convert_dat_to_hdf5.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/convert_dat_to_hdf5.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/create_eos_posterior_pipeline` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/create_eos_posterior_pipeline`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_ConsolidateDAGsUnderMaster.sh` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_ConsolidateDAGsUnderMaster.sh`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/convert_output_format_ascii2h5.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/convert_output_format_ascii2h5.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/helper_LDG_Events.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/helper_LDG_Events.py`

 * *Files 1% similar despite different names*

```diff
@@ -709,18 +709,23 @@
     opts.fmax = unsafe_config_get(config,['engine','srate'])/2 -1  # LI default is not to set srate as an independent variable. Occasional danger with maximum frequency limit in PSD
     # overwrite arguments used with fmax, if provided. ASSUME same for all!
     if config.has_option('lalinference', 'fhigh'):
         fhigh_dict = unsafe_config_get(config,['lalinference','fhigh'])
         for name in fhigh_dict:
             opts.fmax = float(fhigh_dict[name])
 
-    srate = int(np.max([unsafe_config_get(config,['engine','srate']),srate]))  # raise the srate, but never lower it below the fiducial value
+    srate = int(unsafe_config_get(config,['engine','srate']))  # raise the srate
     if not(is_int_power_of_2(srate)):
         print("srate must be power of 2!")
         sys.exit(0)
+    # Print warning if srate < 4096
+    if srate < 4096:
+        print("""WARNING WARNING WARNING : 
+You are requesting srate < 4096 with your ini file.  Use at your own risk - all our comprehensive testing is at higher sampling rates.
+""")
     
     opts.fmin = fmin_fiducial # used only to estimate length; overridden later
 
     # Use ini file arguments, unless override
 
     # Force safe PSD
 
@@ -1462,14 +1467,16 @@
             helper_cip_arg_list[indx] += " --lnL-offset " + str( lnL_start*(1.- 1.*indx/(n_levels-1.))  + lnL_end*indx/(n_levels-1.) )
 
     if opts.assume_matter and not(opts.internal_tabular_eos_file) and not(opts.assume_matter_eos):
         helper_puff_args += " --parameter LambdaTilde  --downselect-parameter s1z --downselect-parameter-range [-0.9,0.9] --downselect-parameter s2z --downselect-parameter-range [-0.9,0.9]  "  # Probably should also aggressively force sampling of low-lambda region
         helper_cip_args += " --input-tides --parameter-implied LambdaTilde  --parameter-nofit lambda2 " # For early fitting, just fit LambdaTilde
         if not(opts.assume_matter_but_primary_bh):
             helper_cip_args+= " --parameter-nofit lambda1 "
+        else:
+            helper_puff_args = helper_puff_args.replace(" --parameter LambdaTilde ", " --parameter lambda2 ")  # if primary a BH, only varying lambda2
         # Add LambdaTilde on top of the aligned spin runs
         for indx in np.arange(len(helper_cip_arg_list)):
             helper_cip_arg_list[indx]+= " --input-tides --parameter-implied LambdaTilde  --parameter-nofit lambda2 " 
             if not(opts.assume_matter_but_primary_bh):
                 helper_cip_arg_list[indx] += " --parameter-nofit lambda1 "
         # add --prior-lambda-linear to first iteration, to sample better at low lambda
         helper_cip_arg_list[0] += " --prior-lambda-linear "
```

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_MassGridCoalesce.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_MassGridCoalesce.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_NRRelabelILE.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_NRRelabelILE.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_IntermediateEOSIntegralFromFit.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_IntermediateEOSIntegralFromFit.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/convert_output_format_allnet2xml` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/convert_output_format_allnet2xml`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_GridSubsetOfTemplateBank.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_GridSubsetOfTemplateBank.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_ParameterFilter.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_ParameterFilter.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_HyperparameterGrid.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_HyperparameterGrid.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/create_event_dag_via_grid` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/create_event_dag_via_grid`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/convergence_test_samples.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/convergence_test_samples.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_BasicIteration` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_BasicIteration`

 * *Files 2% similar despite different names*

```diff
@@ -201,24 +201,26 @@
 parser.add_argument("--last-iteration-extrinsic-time-resampling",action='store_true',help="Last iterations use time resampling (+ the fairdraw is done inside ILE itself), so different code path for final stages")
 parser.add_argument("--ile-args",default=None,help="filename of args_ile.txt file  which holds ILE arguments.  Should NOT conflict with arguments auto-set by this DAG ... in particular, i/o arguments will be modified")
 parser.add_argument("--ile-exe",default=None,help="filename of ILE or equivalent executable. Will default to `which integrate_likelihood_extrinsic` in low-level code")
 parser.add_argument("--ile-retries",default=0,type=int,help="Number of retry attempts for ILE jobs. (These can fail)")
 parser.add_argument("--general-retries",default=0,type=int,help="Number of retry attempts for internal jobs (convert, CIP, ...). (These can fail, albeit more rarely, usually due to filesystem problems)")
 parser.add_argument("--general-request-disk",default="10M",type=str,help="Request disk passed to condor. Must be done for all jobs now")
 parser.add_argument("--ile-request-disk",default="10M",type=str,help="Request disk passed to condor for ILE. Must be done for all jobs now")
+parser.add_argument("--cal-request-disk",default="8G",type=str,help="Request disk passed to condor for ILE. Must be done for all jobs now")
 parser.add_argument("--ile-n-events-to-analyze",default=1,type=int,help="If >1, you are using ILE_batchmode.  Structures the DAG correctly to account for batch cadence")
 parser.add_argument("--ile-runtime-max-minutes",default=None,type=int,help="If not none, kills ILE jobs that take longer than the specified integer number of minutes. Do not use unless an expert")
 parser.add_argument("--cip-exe",default=None,help="filename of CIP or equivalent executable. Will default to `which util_ConstructIntrinsicPosterior_GenericCoordinates` in low-level code")
 parser.add_argument("--cip-exe-G",default=None,help="filename of CIP or equivalent executable, as ALTERNATE CIP used when a 'G' iteration is requested ")
 parser.add_argument("--use-eccentricity",default=False,action='store_true')
 parser.add_argument("--test-exe",default=None,help="filename of test code or equivalent executable.  Must have a --test-output <fname> argument.  Used for convergence testing or other termination. NOT ACTIVE; see 'convergence_test_samples.py' for example")
 parser.add_argument("--plot-exe",default=None,help="filename of plot code or equivalent executable.  Will default to `which plot_posterior_corner.py`.  Default is to plot last set of samples")
 parser.add_argument("--gridinit-exe",default=None,help="filename of initial grid creation or equivalent executable.  Will default to `which util_ManualOverlapGrid.py`.  Must create overlap-grid-0.xml.gz")
 parser.add_argument("--calibration-reweighting-exe",default=None,help="Calibration reweighting script")
 parser.add_argument("--calibration-reweighting",action='store_true',help="Run calibration reweighting on final posterior samples")
+parser.add_argument("--calibration-reweighting-batchsize",type=int,default=None,help="If not 'None', tries to group the final set of points based on jobs of a fixed size")
 parser.add_argument("--convert-ascii2h5-exe",default=None,help="Converting ascii to h5 file script")
 parser.add_argument("--comov-distance-reweighting-exe",default=None,help="Comoving distance reweighting script")
 parser.add_argument("--comov-distance-reweighting",action='store_true',help="Run comoving distance reweighting on final posterior samples")
 parser.add_argument("--bilby-pickle-exe",default=None,help="Bilby pickle generation script")
 parser.add_argument("--bilby-ini-file",default=None,help="Filename of bilby ini file used to generate pickle file (used for calibration reweighting)")
 parser.add_argument("--bilby-pickle-file",default=None,help="Filename of bilby pickle file used for calibration reweighting")
 parser.add_argument("--bw-exe",default=None,help="BayesWave location (or wrapper)")
@@ -1040,23 +1042,50 @@
     elif opts.last_iteration_extrinsic_time_resampling and opts.bilby_ini_file:
         calibration_job, calibration_job_name = dag_utils.write_calibration_uncertainty_reweighting_sub(tag='Calib_reweight',log_dir=None,posterior_file=opts.working_directory+"/extrinsic_posterior_samples.dat",time_marg=False,pickle_file=opts.working_directory+"/calmarg/data/calmarg_data_dump.pickle",exe=opts.calibration_reweighting_exe,universe=local_worker_universe,no_grid=no_worker_grid,ile_args=ile_args)
     elif (not opts.last_iteration_extrinsic_time_resampling) and opts.bilby_ini_file:
         calibration_job, calibration_job_name = dag_utils.write_calibration_uncertainty_reweighting_sub(tag='Calib_reweight',log_dir=None,posterior_file=opts.working_directory+"/extrinsic_posterior_samples.dat",time_marg=True,pickle_file=opts.working_directory+"/calmarg/data/calmarg_data_dump.pickle",exe=opts.calibration_reweighting_exe,universe=local_worker_universe,no_grid=no_worker_grid,cache_file=opts.cache_file,frames_dir=opts.frames_dir,ile_args=ile_args)
     elif (not opts.last_iteration_extrinsic_time_resampling) and opts.bilby_pickle_file:
         calibration_job, calibration_job_name = dag_utils.write_calibration_uncertainty_reweighting_sub(tag='Calib_reweight',log_dir=None,posterior_file=opts.working_directory+"/extrinsic_posterior_samples.dat",time_marg=True,pickle_file=opts.bilby_pickle_file,exe=opts.calibration_reweighting_exe,universe=local_worker_universe,no_grid=no_worker_grid,ile_args=ile_args)
         
-    calibration_job.set_log_file(opts.working_directory+"/calibration-$(cluster)-$(process).log")
-    calibration_job.set_stderr_file(opts.working_directory+"/calibration-$(cluster)-$(process).err")
-    calibration_job.set_stdout_file(opts.working_directory+"/calibration-$(cluster)-$(process).out")
+    if not(opts.calibration_reweighting_batchsize): # single run
+        calibration_job.set_log_file(opts.working_directory+"/iteration_$(macroiteration)_con/calibration-$(cluster)-$(process).log")
+        calibration_job.set_stderr_file(opts.working_directory+"/iteration_$(macroiteration)_con/calibration-$(cluster)-$(process).err")
+        calibration_job.set_stdout_file(opts.working_directory+"/iteration_$(macroiteration)_con/calibration-$(cluster)-$(process).out")
+    else:
+        calibration_job.add_condor_cmd("initialdir",opts.working_directory+"/calmarg/")
+        calibration_job.add_arg(" --start_index $(macrostartidx) ")
+        calibration_job.add_arg(" --end_index $(macroendidx) ")
+        calibration_job.set_log_file(opts.working_directory+"/iteration_$(macroiteration)_con/logs/calibration-$(macrostartidx)-$(cluster)-$(process).log")
+        calibration_job.set_stderr_file(opts.working_directory+"/iteration_$(macroiteration)_con/calibration-$(macrostartidx)-$(cluster)-$(process).err")
+        calibration_job.set_stdout_file(opts.working_directory+"/iteration_$(macroiteration)_con/calibration-$(macrostartidx)-$(cluster)-$(process).out")
     calibration_job.add_condor_cmd('request_disk',opts.general_request_disk)
 
     if opts.use_full_submit_paths:
         fname = opts.working_directory+"/"+calibration_job.get_sub_file()
         calibration_job.set_sub_file(fname)
     calibration_job.write_sub_file()
+
+    # job to combine things. Write here to make logic human-readable
+    if (opts.calibration_reweighting_batchsize): # single run
+        reweight_merge_job, reweight_merge_job_name = dag_utils.write_convert_sub(exe=which('combine_weights_and_rejection_sample.py'),tag='CAL_REWEIGHT_COMBINE',log_dir=None,arg_str='',file_input=opts.working_directory+'/extrinsic_posterior_samples.dat weight_files/',file_output=None, out_dir=opts.working_directory,universe=local_worker_universe,no_grid=no_worker_grid)
+        reweight_merge_job.add_condor_cmd("initialdir",opts.working_directory+"/calmarg/")
+        reweight_merge_job.set_log_file(opts.working_directory+"/iteration_$(macroiteration)_con/logs/reweight-merge-$(cluster)-$(process).log")
+        reweight_merge_job.set_stderr_file(opts.working_directory+"/iteration_$(macroiteration)_con/logs/reweight-merge-$(cluster)-$(process).err")
+        reweight_merge_job.set_stdout_file(opts.working_directory+"/iteration_$(macroiteration)_con/logs/reweight-merge-$(cluster)-$(process).out")
+        reweight_merge_job.add_condor_cmd('request_disk',opts.cal_request_disk)
+        if opts.use_full_submit_paths:
+            fname = opts.working_directory+"/"+reweight_merge_job.get_sub_file()
+            reweight_merge_job.set_sub_file(fname)
+        if opts.use_osg:
+            reweight_merge_job.add_condor_cmd("+DESIRED_SITES",'"nogrid"')
+            reweight_merge_job.add_condor_cmd("+flock_local",'true')
+        reweight_merge_job.write_sub_file()
+
+
+
     
     if opts.bilby_ini_file:
         pickle_job, pickle_job_name = dag_utils.write_bilby_pickle_sub(tag='Bilby_pickle',log_dir=None,bilby_ini_file=opts.bilby_ini_file,exe=opts.bilby_pickle_exe,universe='local',no_grid=no_worker_grid,cache_file=opts.cache_file,frames_dir=opts.frames_dir,ile_args=ile_args)
         pickle_job.set_log_file(opts.working_directory+"/pickle-$(cluster)-$(process).log")
         pickle_job.set_stderr_file(opts.working_directory+"/pickle-$(cluster)-$(process).err")
         pickle_job.set_stdout_file(opts.working_directory+"/pickle-$(cluster)-$(process).out")
         pickle_job.add_condor_cmd('request_disk',opts.general_request_disk)
@@ -1562,19 +1591,40 @@
     if opts.bilby_ini_file:
         pickle_node = pipeline.CondorDAGNode(pickle_job)
         pickle_node.add_macro("macroiteration",it)
         pickle_node.set_category("PICKLE")
         pickle_node.add_parent(last_node)
         last_node=pickle_node
         dag.add_node(pickle_node)
-    calibration_node = pipeline.CondorDAGNode(calibration_job)
-    calibration_node.add_macro("macroiteration",it)
-    calibration_node.set_category("CALIBRATION")
-    calibration_node.add_parent(last_node)
-    dag.add_node(calibration_node)
+    # Do single job if only one needed, otherwise loop
+    if not(opts.calibration_reweighting_batchsize):
+        calibration_node = pipeline.CondorDAGNode(calibration_job)
+        calibration_node.add_macro("macroiteration",it)
+        calibration_node.set_category("CALIBRATION")
+        calibration_node.add_parent(last_node)
+        dag.add_node(calibration_node)
+    else:
+        # Make job to reweight everything, after producing samples
+        reweight_merge_node =    pipeline.CondorDAGNode(reweight_merge_job)
+        reweight_merge_node.add_macro("macroiteration",it)
+
+        # Make individual calibration nodes
+        for start_indx in np.arange(start=0,stop=opts.last_iteration_extrinsic_nsamples,step=opts.calibration_reweighting_batchsize):
+            end_indx = start_indx + opts.calibration_reweighting_batchsize  # end index is not included, python-style indexing so no fencepost problems
+            calibration_node = pipeline.CondorDAGNode(calibration_job)
+            calibration_node.add_macro("macroiteration",it)
+            calibration_node.add_macro("macrostartidx",start_indx)
+            calibration_node.add_macro("macroendidx",end_indx)
+            calibration_node.set_category("CALIBRATION")
+            calibration_node.add_parent(last_node)
+            reweight_merge_node.add_parent(calibration_node)
+            dag.add_node(calibration_node)
+            
+        # add the merge node.  Thouls be the last node
+        dag.add_node(reweight_merge_node)
     
 if opts.comov_distance_reweighting:
     convert_ascii_node = pipeline.CondorDAGNode(convert_ascii_job)
     convert_ascii_node.add_macro("macroiteration",it)
     convert_ascii_node.set_category("CONVERT_ASCII")
     convert_ascii_node.add_parent(last_node)
     dag.add_node(convert_ascii_node)
```

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_AlternateIteration` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/create_event_parameter_pipeline_AlternateIteration`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic_no-op` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/integrate_likelihood_extrinsic_no-op`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_EOBTideWriteFrame.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_EOBTideWriteFrame.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_ConstructEOSPosterior.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_ConstructEOSPosterior.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_ILEdagPostprocess.sh` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_ILEdagPostprocess.sh`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/convert_output_format_inference2ile` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/convert_output_format_inference2ile`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/create_CIP_convergence_sequence.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/create_CIP_convergence_sequence.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_WriteFrameAndCacheFromXML.sh` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_WriteFrameAndCacheFromXML.sh`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_ParameterRandomize.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_ParameterRandomize.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_SimInspiralToCoinc.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_SimInspiralToCoinc.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/bin/util_FitAndEvaluate_GenericCoordinates.py` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/bin/util_FitAndEvaluate_GenericCoordinates.py`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT.egg-info/PKG-INFO` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RIFT
-Version: 0.0.15.8rc6
+Version: 0.0.15.8rc7
 Summary: RIFT parameter estimation pipeline. Note branch used is temp-RIT-Tides-port_python3_restructure_package (which will become master shortly)!
 Home-page: https://git.ligo.org/rapidpe-rift/rift
 Author: Richard O'Shaughnessy
 Author-email: richard.oshaughnessy@ligo.org
 License: UNKNOWN
 Description: research-projects (temp-RIT-Tides and descendants)
         research-projects-RIT
```

### Comparing `RIFT-0.0.15.8rc6/MonteCarloMarginalizeCode/Code/RIFT.egg-info/SOURCES.txt` & `RIFT-0.0.15.8rc7/MonteCarloMarginalizeCode/Code/RIFT.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -68,14 +68,15 @@
 MonteCarloMarginalizeCode/Code/RIFT/physics/MonotonicSpline.py
 MonteCarloMarginalizeCode/Code/RIFT/physics/PrecessingFisherMatrix.py
 MonteCarloMarginalizeCode/Code/RIFT/physics/ROMWaveformManager.py
 MonteCarloMarginalizeCode/Code/RIFT/physics/__init__.py
 MonteCarloMarginalizeCode/Code/RIFT/physics/effectiveFisher.py
 MonteCarloMarginalizeCode/Code/bin/assess_propose_CIP_convergence_sequence.py
 MonteCarloMarginalizeCode/Code/bin/calibration_reweighting.py
+MonteCarloMarginalizeCode/Code/bin/combine_weights_and_rejection_sample.py
 MonteCarloMarginalizeCode/Code/bin/config_yank.py
 MonteCarloMarginalizeCode/Code/bin/convergence_test_amr.py
 MonteCarloMarginalizeCode/Code/bin/convergence_test_samples.py
 MonteCarloMarginalizeCode/Code/bin/convert_dat_to_hdf5.py
 MonteCarloMarginalizeCode/Code/bin/convert_output_format_allnet2xml
 MonteCarloMarginalizeCode/Code/bin/convert_output_format_ascii2h5.py
 MonteCarloMarginalizeCode/Code/bin/convert_output_format_ile2inference
```

### Comparing `RIFT-0.0.15.8rc6/INSTALL_OPTIONAL_DEPENDENCIES.md` & `RIFT-0.0.15.8rc7/INSTALL_OPTIONAL_DEPENDENCIES.md`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/AUTOMATED_OR_ONLINE.md` & `RIFT-0.0.15.8rc7/AUTOMATED_OR_ONLINE.md`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/PACKAGING.md` & `RIFT-0.0.15.8rc7/PACKAGING.md`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/INSTALL.md` & `RIFT-0.0.15.8rc7/INSTALL.md`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/PKG-INFO` & `RIFT-0.0.15.8rc7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RIFT
-Version: 0.0.15.8rc6
+Version: 0.0.15.8rc7
 Summary: RIFT parameter estimation pipeline. Note branch used is temp-RIT-Tides-port_python3_restructure_package (which will become master shortly)!
 Home-page: https://git.ligo.org/rapidpe-rift/rift
 Author: Richard O'Shaughnessy
 Author-email: richard.oshaughnessy@ligo.org
 License: UNKNOWN
 Description: research-projects (temp-RIT-Tides and descendants)
         research-projects-RIT
```

### Comparing `RIFT-0.0.15.8rc6/setup.py` & `RIFT-0.0.15.8rc7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 #  - ourio.py, ourparams.py
 #  - anything with 'test'
 #print " Identified scripts ", my_scripts\
 #print setuptools.find_packages('MonteCarloMarginalizeCode/Code')
 
 setuptools.setup(
     name="RIFT",
-    version="0.0.15.8rc6", # do not build on OSX machine, side effects
+    version="0.0.15.8rc7", # do not build on OSX machine, side effects
     author="Richard O'Shaughnessy",
     author_email="richard.oshaughnessy@ligo.org",
     description="RIFT parameter estimation pipeline. Note branch used is temp-RIT-Tides-port_python3_restructure_package (which will become master shortly)!",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://git.ligo.org/rapidpe-rift/rift",
     package_dir = {'':'MonteCarloMarginalizeCode/Code'},
```

### Comparing `RIFT-0.0.15.8rc6/Dockerfile` & `RIFT-0.0.15.8rc7/Dockerfile`

 * *Files identical despite different names*

### Comparing `RIFT-0.0.15.8rc6/README.md` & `RIFT-0.0.15.8rc7/README.md`

 * *Files identical despite different names*

