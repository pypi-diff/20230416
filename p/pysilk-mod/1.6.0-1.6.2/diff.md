# Comparing `tmp/pysilk-mod-1.6.0.tar.gz` & `tmp/pysilk-mod-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysilk-mod-1.6.0.tar", last modified: Fri May 20 16:44:12 2022, max compression
+gzip compressed data, was "pysilk-mod-1.6.2.tar", last modified: Sun Apr 16 16:25:16 2023, max compression
```

## Comparing `pysilk-mod-1.6.0.tar` & `pysilk-mod-1.6.2.tar`

### file list

```diff
@@ -1,134 +1,137 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 16:44:12.590392 pysilk-mod-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (121)     6277 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      565 2022-05-20 16:44:12.590392 pysilk-mod-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1892 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      372 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      649 2022-05-20 16:44:12.590392 pysilk-mod-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     5771 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 16:44:12.578392 pysilk-mod-1.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 16:44:12.582392 pysilk-mod-1.6.0/src/pysilk/
--rw-r--r--   0 runner    (1001) docker     (121)      356 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/pysilk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2530 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/pysilk/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2661 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/pysilk/pysilk.py
--rw-r--r--   0 runner    (1001) docker     (121)     1325 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/pysilk/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1232 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/pysilk/wav.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 16:44:12.582392 pysilk-mod-1.6.0/src/pysilk_mod.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      565 2022-05-20 16:44:12.000000 pysilk-mod-1.6.0/src/pysilk_mod.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4737 2022-05-20 16:44:12.000000 pysilk-mod-1.6.0/src/pysilk_mod.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-20 16:44:12.000000 pysilk-mod-1.6.0/src/pysilk_mod.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-05-20 16:44:12.000000 pysilk-mod-1.6.0/src/pysilk_mod.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-20 16:44:10.000000 pysilk-mod-1.6.0/src/pysilk_mod.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 16:44:12.582392 pysilk-mod-1.6.0/src/silk/
--rw-r--r--   0 runner    (1001) docker     (121)     3564 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/_pysilk.cpp
--rw-r--r--   0 runner    (1001) docker     (121)     9635 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/codec.cpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-20 16:44:12.590392 pysilk-mod-1.6.0/src/silk/src/
--rw-r--r--   0 runner    (1001) docker     (121)    11860 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_A2NLSF.c
--rw-r--r--   0 runner    (1001) docker     (121)     6867 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_CNG.c
--rw-r--r--   0 runner    (1001) docker     (121)     6490 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_HP_variable_cutoff_FIX.c
--rw-r--r--   0 runner    (1001) docker     (121)     2135 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_LBRR_reset.c
--rw-r--r--   0 runner    (1001) docker     (121)     6972 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_LPC_inv_pred_gain.c
--rw-r--r--   0 runner    (1001) docker     (121)     5643 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_LPC_synthesis_filter.c
--rw-r--r--   0 runner    (1001) docker     (121)     8684 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_LPC_synthesis_order16.c
--rw-r--r--   0 runner    (1001) docker     (121)     9548 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_LP_variable_cutoff.c
--rw-r--r--   0 runner    (1001) docker     (121)     4397 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_LSF_cos_table.c
--rw-r--r--   0 runner    (1001) docker     (121)     4154 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_LTP_analysis_filter_FIX.c
--rw-r--r--   0 runner    (1001) docker     (121)     3926 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_LTP_scale_ctrl_FIX.c
--rw-r--r--   0 runner    (1001) docker     (121)     5503 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_MA.c
--rw-r--r--   0 runner    (1001) docker     (121)     6430 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_NLSF2A.c
--rw-r--r--   0 runner    (1001) docker     (121)     2892 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_NLSF2A_stable.c
--rw-r--r--   0 runner    (1001) docker     (121)     4632 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_NLSF_MSVQ_decode.c
--rw-r--r--   0 runner    (1001) docker     (121)    12040 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_NLSF_MSVQ_encode_FIX.c
--rw-r--r--   0 runner    (1001) docker     (121)     3731 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_NLSF_VQ_rate_distortion_FIX.c
--rw-r--r--   0 runner    (1001) docker     (121)     4298 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_NLSF_VQ_sum_error_FIX.c
--rw-r--r--   0 runner    (1001) docker     (121)     4048 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_NLSF_VQ_weights_laroia.c
--rw-r--r--   0 runner    (1001) docker     (121)     6495 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_NLSF_stabilize.c
--rw-r--r--   0 runner    (1001) docker     (121)    24508 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_NSQ.c
--rw-r--r--   0 runner    (1001) docker     (121)    40858 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_NSQ_del_dec.c
--rw-r--r--   0 runner    (1001) docker     (121)    20279 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_PLC.c
--rw-r--r--   0 runner    (1001) docker     (121)    13915 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_VAD.c
--rw-r--r--   0 runner    (1001) docker     (121)     8315 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_VQ_nearest_neighbor_FIX.c
--rw-r--r--   0 runner    (1001) docker     (121)     4378 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_ana_filt_bank_1.c
--rw-r--r--   0 runner    (1001) docker     (121)     5973 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_apply_sine_window.c
--rw-r--r--   0 runner    (1001) docker     (121)     3534 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_array_maxabs.c
--rw-r--r--   0 runner    (1001) docker     (121)     4379 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_autocorr.c
--rw-r--r--   0 runner    (1001) docker     (121)     3704 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_biquad.c
--rw-r--r--   0 runner    (1001) docker     (121)     4055 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_biquad_alt.c
--rw-r--r--   0 runner    (1001) docker     (121)    13965 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_burg_modified.c
--rw-r--r--   0 runner    (1001) docker     (121)     2792 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_bwexpander.c
--rw-r--r--   0 runner    (1001) docker     (121)     2486 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_bwexpander_32.c
--rw-r--r--   0 runner    (1001) docker     (121)     4529 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_code_signs.c
--rw-r--r--   0 runner    (1001) docker     (121)     7085 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_control_audio_bandwidth.c
--rw-r--r--   0 runner    (1001) docker     (121)    18828 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_control_codec_FIX.c
--rw-r--r--   0 runner    (1001) docker     (121)     7868 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_corrMatrix_FIX.c
--rw-r--r--   0 runner    (1001) docker     (121)     2482 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_create_init_destroy.c
--rw-r--r--   0 runner    (1001) docker     (121)    12284 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_dec_API.c
--rw-r--r--   0 runner    (1001) docker     (121)    16135 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_decode_core.c
--rw-r--r--   0 runner    (1001) docker     (121)     6995 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_decode_frame.c
--rw-r--r--   0 runner    (1001) docker     (121)    11628 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_decode_parameters.c
--rw-r--r--   0 runner    (1001) docker     (121)     2956 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_decode_pitch.c
--rw-r--r--   0 runner    (1001) docker     (121)     5238 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_decode_pulses.c
--rw-r--r--   0 runner    (1001) docker     (121)     3951 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_decoder_set_fs.c
--rw-r--r--   0 runner    (1001) docker     (121)     3951 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_detect_SWB_input.c
--rw-r--r--   0 runner    (1001) docker     (121)     1930 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_div_oabi.c
--rw-r--r--   0 runner    (1001) docker     (121)    10875 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_enc_API.c
--rw-r--r--   0 runner    (1001) docker     (121)    20263 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_encode_frame_FIX.c
--rw-r--r--   0 runner    (1001) docker     (121)     7020 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_encode_parameters.c
--rw-r--r--   0 runner    (1001) docker     (121)     8143 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_encode_pulses.c
--rw-r--r--   0 runner    (1001) docker     (121)     7472 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_find_LPC_FIX.c
--rw-r--r--   0 runner    (1001) docker     (121)    12797 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_find_LTP_FIX.c
--rw-r--r--   0 runner    (1001) docker     (121)     6758 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_find_pitch_lags_FIX.c
--rw-r--r--   0 runner    (1001) docker     (121)     6599 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_find_pred_coefs_FIX.c
--rw-r--r--   0 runner    (1001) docker     (121)     4827 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_gain_quant.c
--rw-r--r--   0 runner    (1001) docker     (121)     2736 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_init_encoder_FIX.c
--rw-r--r--   0 runner    (1001) docker     (121)     3701 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_inner_prod_aligned.c
--rw-r--r--   0 runner    (1001) docker     (121)     2702 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_interpolate.c
--rw-r--r--   0 runner    (1001) docker     (121)     3309 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_k2a.c
--rw-r--r--   0 runner    (1001) docker     (121)     3285 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_k2a_Q16.c
--rw-r--r--   0 runner    (1001) docker     (121)     2949 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_lin2log.c
--rw-r--r--   0 runner    (1001) docker     (121)     3309 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_log2lin.c
--rw-r--r--   0 runner    (1001) docker     (121)    25529 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_noise_shape_analysis_FIX.c
--rw-r--r--   0 runner    (1001) docker     (121)    34681 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_pitch_analysis_core.c
--rw-r--r--   0 runner    (1001) docker     (121)     3776 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_pitch_est_tables.c
--rw-r--r--   0 runner    (1001) docker     (121)    12337 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_prefilter_FIX.c
--rw-r--r--   0 runner    (1001) docker     (121)     6754 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_process_NLSFs_FIX.c
--rw-r--r--   0 runner    (1001) docker     (121)     6088 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_process_gains_FIX.c
--rw-r--r--   0 runner    (1001) docker     (121)     5172 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_quant_LTP_gains_FIX.c
--rw-r--r--   0 runner    (1001) docker     (121)    14380 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_range_coder.c
--rw-r--r--   0 runner    (1001) docker     (121)     2517 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_regularize_correlations_FIX.c
--rw-r--r--   0 runner    (1001) docker     (121)    14265 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_resampler.c
--rw-r--r--   0 runner    (1001) docker     (121)     4048 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_resampler_down2.c
--rw-r--r--   0 runner    (1001) docker     (121)     5061 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_resampler_down2_3.c
--rw-r--r--   0 runner    (1001) docker     (121)     4568 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_resampler_down3.c
--rw-r--r--   0 runner    (1001) docker     (121)     3051 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_resampler_private_AR2.c
--rw-r--r--   0 runner    (1001) docker     (121)     4126 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_resampler_private_ARMA4.c
--rw-r--r--   0 runner    (1001) docker     (121)     5685 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_resampler_private_IIR_FIR.c
--rw-r--r--   0 runner    (1001) docker     (121)     2688 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_resampler_private_copy.c
--rw-r--r--   0 runner    (1001) docker     (121)     4196 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_resampler_private_down4.c
--rw-r--r--   0 runner    (1001) docker     (121)     8103 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_resampler_private_down_FIR.c
--rw-r--r--   0 runner    (1001) docker     (121)     6299 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_resampler_private_up2_HQ.c
--rw-r--r--   0 runner    (1001) docker     (121)     4171 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_resampler_private_up4.c
--rw-r--r--   0 runner    (1001) docker     (121)     9277 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_resampler_rom.c
--rw-r--r--   0 runner    (1001) docker     (121)     3967 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_resampler_up2.c
--rw-r--r--   0 runner    (1001) docker     (121)     4601 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_residual_energy16_FIX.c
--rw-r--r--   0 runner    (1001) docker     (121)     4598 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_residual_energy_FIX.c
--rw-r--r--   0 runner    (1001) docker     (121)     2338 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_scale_copy_vector16.c
--rw-r--r--   0 runner    (1001) docker     (121)     2330 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_scale_vector.c
--rw-r--r--   0 runner    (1001) docker     (121)     4550 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_schur.c
--rw-r--r--   0 runner    (1001) docker     (121)     4198 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_schur64.c
--rw-r--r--   0 runner    (1001) docker     (121)     7834 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_shell_coder.c
--rw-r--r--   0 runner    (1001) docker     (121)     3835 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_sigm_Q15.c
--rw-r--r--   0 runner    (1001) docker     (121)    10369 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_solve_LS_FIX.c
--rw-r--r--   0 runner    (1001) docker     (121)     5986 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_sort.c
--rw-r--r--   0 runner    (1001) docker     (121)     4654 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_sum_sqr_shift.c
--rw-r--r--   0 runner    (1001) docker     (121)     7829 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_tables_LTP.c
--rw-r--r--   0 runner    (1001) docker     (121)    30558 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_tables_NLSF_CB0_10.c
--rw-r--r--   0 runner    (1001) docker     (121)    75456 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_tables_NLSF_CB0_16.c
--rw-r--r--   0 runner    (1001) docker     (121)    20070 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_tables_NLSF_CB1_10.c
--rw-r--r--   0 runner    (1001) docker     (121)    39000 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_tables_NLSF_CB1_16.c
--rw-r--r--   0 runner    (1001) docker     (121)     3604 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_tables_gain.c
--rw-r--r--   0 runner    (1001) docker     (121)     6978 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_tables_other.c
--rw-r--r--   0 runner    (1001) docker     (121)    11652 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_tables_pitch_lag.c
--rw-r--r--   0 runner    (1001) docker     (121)     9867 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_tables_pulses_per_block.c
--rw-r--r--   0 runner    (1001) docker     (121)     2228 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_tables_sign.c
--rw-r--r--   0 runner    (1001) docker     (121)     2227 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_tables_type_offset.c
--rw-r--r--   0 runner    (1001) docker     (121)     4381 2022-05-20 16:43:59.000000 pysilk-mod-1.6.0/src/silk/src/SKP_Silk_warped_autocorrelation_FIX.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:16.350314 pysilk-mod-1.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-16 16:25:16.350314 pysilk-mod-1.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-16 16:25:16.350314 pysilk-mod-1.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:16.334313 pysilk-mod-1.6.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:16.338313 pysilk-mod-1.6.2/src/pysilk/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/pysilk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/pysilk/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/pysilk/pysilk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/pysilk/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/pysilk/wav.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:16.338313 pysilk-mod-1.6.2/src/pysilk_mod.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-04-16 16:25:16.000000 pysilk-mod-1.6.2/src/pysilk_mod.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-04-16 16:25:16.000000 pysilk-mod-1.6.2/src/pysilk_mod.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 16:25:16.000000 pysilk-mod-1.6.2/src/pysilk_mod.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-16 16:25:16.000000 pysilk-mod-1.6.2/src/pysilk_mod.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 16:25:16.000000 pysilk-mod-1.6.2/src/pysilk_mod.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:16.338313 pysilk-mod-1.6.2/src/silk/
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/_pysilk.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9635 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/codec.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:16.350314 pysilk-mod-1.6.2/src/silk/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    11860 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_A2NLSF.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6867 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_CNG.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6490 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_HP_variable_cutoff_FIX.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_LBRR_reset.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6972 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_LPC_inv_pred_gain.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_LPC_synthesis_filter.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_LPC_synthesis_order16.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_LP_variable_cutoff.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_LSF_cos_table.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_LTP_analysis_filter_FIX.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_LTP_scale_ctrl_FIX.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_MA.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6430 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_NLSF2A.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_NLSF2A_stable.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_NLSF_MSVQ_decode.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12040 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_NLSF_MSVQ_encode_FIX.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_NLSF_VQ_rate_distortion_FIX.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_NLSF_VQ_sum_error_FIX.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_NLSF_VQ_weights_laroia.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6495 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_NLSF_stabilize.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24508 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_NSQ.c
+-rw-r--r--   0 runner    (1001) docker     (123)    40858 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_NSQ_del_dec.c
+-rw-r--r--   0 runner    (1001) docker     (123)    20279 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_PLC.c
+-rw-r--r--   0 runner    (1001) docker     (123)    13915 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_VAD.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8315 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_VQ_nearest_neighbor_FIX.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_ana_filt_bank_1.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5973 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_apply_sine_window.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_array_maxabs.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_autocorr.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_biquad.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_biquad_alt.c
+-rw-r--r--   0 runner    (1001) docker     (123)    13965 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_burg_modified.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_bwexpander.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_bwexpander_32.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4529 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_code_signs.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7085 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_control_audio_bandwidth.c
+-rw-r--r--   0 runner    (1001) docker     (123)    18828 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_control_codec_FIX.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7868 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_corrMatrix_FIX.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_create_init_destroy.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12284 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_dec_API.c
+-rw-r--r--   0 runner    (1001) docker     (123)    16135 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_decode_core.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6995 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_decode_frame.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11628 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_decode_parameters.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_decode_pitch.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_decode_pulses.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_decoder_set_fs.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_detect_SWB_input.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_div_oabi.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10875 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_enc_API.c
+-rw-r--r--   0 runner    (1001) docker     (123)    20263 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_encode_frame_FIX.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7020 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_encode_parameters.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8143 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_encode_pulses.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7472 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_find_LPC_FIX.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12797 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_find_LTP_FIX.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_find_pitch_lags_FIX.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_find_pred_coefs_FIX.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_gain_quant.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_init_encoder_FIX.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_inner_prod_aligned.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_interpolate.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_k2a.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_k2a_Q16.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_lin2log.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_log2lin.c
+-rw-r--r--   0 runner    (1001) docker     (123)    25529 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_noise_shape_analysis_FIX.c
+-rw-r--r--   0 runner    (1001) docker     (123)    34681 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_pitch_analysis_core.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_pitch_est_tables.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12337 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_prefilter_FIX.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6754 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_process_NLSFs_FIX.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_process_gains_FIX.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_quant_LTP_gains_FIX.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14380 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_range_coder.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_regularize_correlations_FIX.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14265 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_resampler.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_resampler_down2.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_resampler_down2_3.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4568 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_resampler_down3.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_resampler_private_AR2.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_resampler_private_ARMA4.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_resampler_private_IIR_FIR.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_resampler_private_copy.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_resampler_private_down4.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8103 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_resampler_private_down_FIR.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6299 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_resampler_private_up2_HQ.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_resampler_private_up4.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9277 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_resampler_rom.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3967 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_resampler_up2.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4601 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_residual_energy16_FIX.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_residual_energy_FIX.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_scale_copy_vector16.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_scale_vector.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_schur.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_schur64.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7834 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_shell_coder.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_sigm_Q15.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10369 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_solve_LS_FIX.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5986 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_sort.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_sum_sqr_shift.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7829 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_tables_LTP.c
+-rw-r--r--   0 runner    (1001) docker     (123)    30558 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_tables_NLSF_CB0_10.c
+-rw-r--r--   0 runner    (1001) docker     (123)    75456 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_tables_NLSF_CB0_16.c
+-rw-r--r--   0 runner    (1001) docker     (123)    20070 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_tables_NLSF_CB1_10.c
+-rw-r--r--   0 runner    (1001) docker     (123)    39000 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_tables_NLSF_CB1_16.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_tables_gain.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6978 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_tables_other.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11652 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_tables_pitch_lag.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9867 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_tables_pulses_per_block.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_tables_sign.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_tables_type_offset.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/src/silk/src/SKP_Silk_warped_autocorrelation_FIX.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 16:25:16.350314 pysilk-mod-1.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/tests/test_decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-04-16 16:25:08.000000 pysilk-mod-1.6.2/tests/test_encode.py
```

### Comparing `pysilk-mod-1.6.0/LICENSE` & `pysilk-mod-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/PKG-INFO` & `pysilk-mod-1.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysilk-mod
-Version: 1.6.0
+Version: 1.6.2
 Summary: Python silk decode/encoder
 Home-page: https://github.com/DCZYewen/Python-Silk-Module
 Author: DCZYewen
 Author-email: contact@basicws.net
 Maintainer: wyapx
 Maintainer-email: admin@nullcat.cn
 License: see LICENSE
```

### Comparing `pysilk-mod-1.6.0/README.md` & `pysilk-mod-1.6.2/README.md`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/setup.cfg` & `pysilk-mod-1.6.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/setup.py` & `pysilk-mod-1.6.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 try:
     from pybind11.setup_helpers import Pybind11Extension as Extension
     from pybind11.setup_helpers import build_ext
 except ImportError:
     from setuptools import Extension
     from distutils.command.build_ext import build_ext
 
-__version__ = "1.6.0"
+__version__ = "1.6.2"
 basic_dependency = ["pybind11", "setuptools"]
 
 if version_info.major != 3 or version_info.minor < 6:
     raise RuntimeError("pysilk only support python 3.6 or newer")
 
 
 class CustomBuilder(build_ext):
```

### Comparing `pysilk-mod-1.6.0/src/pysilk/__main__.py` & `pysilk-mod-1.6.2/src/pysilk/__main__.py`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/pysilk/pysilk.py` & `pysilk-mod-1.6.2/src/pysilk/pysilk.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,30 @@
+import sys
 import asyncio
 import functools
-from concurrent.futures import ThreadPoolExecutor
+
 from io import BytesIO
 from os import cpu_count
 from typing import Union, BinaryIO
+from concurrent.futures import ThreadPoolExecutor
 
-from .coder import silkEncode, silkDecode
 from .utils import get_file, is_silk_data
 from .wav import Wave
 
-_LOOP = asyncio.get_event_loop()
+try:
+    from .coder import silkEncode, silkDecode
+except ImportError:
+    if sys.platform == "win32":
+        raise RuntimeError(
+            "Visual C++ runtime not found\n"
+            "install it to continue: https://docs.microsoft.com/zh-CN/cpp/windows/latest-supported-vc-redist"
+        )
+    raise
+
+
 _EXECUTOR = ThreadPoolExecutor(cpu_count())
 
 
 def encode(data: bytes, data_rate=24000, *, sample_rate=24000) -> bytes:
     if data[8:12] == b"WAVE":
         return silkEncode(
             Wave.wav2pcm(BytesIO(data)), sample_rate, data_rate
@@ -46,51 +57,51 @@
     try:
         return decode(fd.read(), to_wav, sample_rate=sample_rate)
     finally:
         fd.close()
 
 
 async def async_encode(data: bytes, data_rate=24000, *, sample_rate=24000) -> bytes:
-    return await _LOOP.run_in_executor(
+    return await asyncio.get_running_loop().run_in_executor(
         _EXECUTOR,
         functools.partial(
             encode,
             data,
             data_rate,
             sample_rate=sample_rate
         )
     )
 
 
 async def async_decode(silk_data: bytes, to_wav=False, *, sample_rate=24000) -> bytes:
-    return await _LOOP.run_in_executor(
+    return await asyncio.get_running_loop().run_in_executor(
         _EXECUTOR,
         functools.partial(
             decode,
             silk_data,
             sample_rate=sample_rate,
             to_wav=to_wav
         )
     )
 
 
 async def async_encode_file(target: Union[str, BinaryIO], data_rate=24000, *, sample_rate=24000) -> bytes:
-    return await _LOOP.run_in_executor(
+    return await asyncio.get_running_loop().run_in_executor(
         _EXECUTOR,
         functools.partial(
             encode_file,
             target,
             data_rate,
             sample_rate=sample_rate
         )
     )
 
 
 async def async_decode_file(silk_file: Union[str, BinaryIO], to_wav=False, *, sample_rate=24000) -> bytes:
-    return await _LOOP.run_in_executor(
+    return await asyncio.get_running_loop().run_in_executor(
         _EXECUTOR,
         functools.partial(
             decode_file,
             silk_file,
             sample_rate=sample_rate,
             to_wav=to_wav
         )
```

### Comparing `pysilk-mod-1.6.0/src/pysilk/utils.py` & `pysilk-mod-1.6.2/src/pysilk/utils.py`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/pysilk/wav.py` & `pysilk-mod-1.6.2/src/pysilk/wav.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import itertools
 import wave
 from io import BytesIO
 from typing import BinaryIO
 
 
 class Wave:
     @staticmethod
@@ -16,24 +17,19 @@
 
     @staticmethod
     def wav2pcm(obj: BinaryIO) -> bytes:
         res = BytesIO()
         with wave.Wave_read(obj) as wav:
             if wav.getcomptype() != "NONE":
                 raise wave.Error("Unsupport with-compressed wave file")
-            elif wav.getnchannels() == 1:
+            else:
                 while True:
                     bl = wav.readframes(512)
                     if bl:
-                        res.write(bl)
-                    else:
-                        break
-            else:
-                channel_data = bytearray()
-                while True:
-                    frame = wav.readframes(1)
-                    if frame:
-                        channel_data.append(frame[0])
+                        res.write(
+                            bytearray(
+                                [i for i in itertools.islice(bl, 0, 0, wav.getnchannels())]
+                            )
+                        )
                     else:
                         break
-                res.write(channel_data)
         return res.getvalue()
```

### Comparing `pysilk-mod-1.6.0/src/pysilk_mod.egg-info/PKG-INFO` & `pysilk-mod-1.6.2/src/pysilk_mod.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysilk-mod
-Version: 1.6.0
+Version: 1.6.2
 Summary: Python silk decode/encoder
 Home-page: https://github.com/DCZYewen/Python-Silk-Module
 Author: DCZYewen
 Author-email: contact@basicws.net
 Maintainer: wyapx
 Maintainer-email: admin@nullcat.cn
 License: see LICENSE
```

### Comparing `pysilk-mod-1.6.0/src/pysilk_mod.egg-info/SOURCES.txt` & `pysilk-mod-1.6.2/src/pysilk_mod.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -120,8 +120,10 @@
 src/silk/src/SKP_Silk_tables_NLSF_CB1_16.c
 src/silk/src/SKP_Silk_tables_gain.c
 src/silk/src/SKP_Silk_tables_other.c
 src/silk/src/SKP_Silk_tables_pitch_lag.c
 src/silk/src/SKP_Silk_tables_pulses_per_block.c
 src/silk/src/SKP_Silk_tables_sign.c
 src/silk/src/SKP_Silk_tables_type_offset.c
-src/silk/src/SKP_Silk_warped_autocorrelation_FIX.c
+src/silk/src/SKP_Silk_warped_autocorrelation_FIX.c
+tests/test_decode.py
+tests/test_encode.py
```

### Comparing `pysilk-mod-1.6.0/src/silk/_pysilk.cpp` & `pysilk-mod-1.6.2/src/silk/_pysilk.cpp`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/codec.cpp` & `pysilk-mod-1.6.2/src/silk/codec.cpp`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_A2NLSF.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_A2NLSF.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_CNG.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_CNG.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_HP_variable_cutoff_FIX.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_HP_variable_cutoff_FIX.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_LBRR_reset.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_LBRR_reset.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_LPC_inv_pred_gain.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_LPC_inv_pred_gain.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_LPC_synthesis_filter.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_LPC_synthesis_filter.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_LPC_synthesis_order16.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_LPC_synthesis_order16.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_LP_variable_cutoff.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_LP_variable_cutoff.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_LSF_cos_table.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_LSF_cos_table.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_LTP_analysis_filter_FIX.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_LTP_analysis_filter_FIX.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_LTP_scale_ctrl_FIX.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_LTP_scale_ctrl_FIX.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_MA.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_MA.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_NLSF2A.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_NLSF2A.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_NLSF2A_stable.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_NLSF2A_stable.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_NLSF_MSVQ_decode.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_NLSF_MSVQ_decode.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_NLSF_MSVQ_encode_FIX.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_NLSF_MSVQ_encode_FIX.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_NLSF_VQ_rate_distortion_FIX.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_NLSF_VQ_rate_distortion_FIX.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_NLSF_VQ_sum_error_FIX.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_NLSF_VQ_sum_error_FIX.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_NLSF_VQ_weights_laroia.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_NLSF_VQ_weights_laroia.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_NLSF_stabilize.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_NLSF_stabilize.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_NSQ.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_NSQ.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_NSQ_del_dec.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_NSQ_del_dec.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_PLC.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_PLC.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_VAD.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_VAD.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_VQ_nearest_neighbor_FIX.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_VQ_nearest_neighbor_FIX.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_ana_filt_bank_1.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_ana_filt_bank_1.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_apply_sine_window.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_apply_sine_window.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_array_maxabs.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_array_maxabs.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_autocorr.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_autocorr.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_biquad.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_biquad.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_biquad_alt.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_biquad_alt.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_burg_modified.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_burg_modified.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_bwexpander.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_bwexpander.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_bwexpander_32.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_bwexpander_32.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_code_signs.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_code_signs.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_control_audio_bandwidth.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_control_audio_bandwidth.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_control_codec_FIX.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_control_codec_FIX.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_corrMatrix_FIX.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_corrMatrix_FIX.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_create_init_destroy.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_create_init_destroy.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_dec_API.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_dec_API.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_decode_core.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_decode_core.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_decode_frame.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_decode_frame.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_decode_parameters.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_decode_parameters.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_decode_pitch.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_decode_pitch.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_decode_pulses.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_decode_pulses.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_decoder_set_fs.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_decoder_set_fs.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_detect_SWB_input.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_detect_SWB_input.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_div_oabi.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_div_oabi.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_enc_API.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_enc_API.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_encode_frame_FIX.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_encode_frame_FIX.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_encode_parameters.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_encode_parameters.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_encode_pulses.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_encode_pulses.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_find_LPC_FIX.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_find_LPC_FIX.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_find_LTP_FIX.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_find_LTP_FIX.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_find_pitch_lags_FIX.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_find_pitch_lags_FIX.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_find_pred_coefs_FIX.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_find_pred_coefs_FIX.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_gain_quant.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_gain_quant.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_init_encoder_FIX.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_init_encoder_FIX.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_inner_prod_aligned.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_inner_prod_aligned.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_interpolate.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_interpolate.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_k2a.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_k2a.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_k2a_Q16.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_k2a_Q16.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_lin2log.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_lin2log.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_log2lin.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_log2lin.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_noise_shape_analysis_FIX.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_noise_shape_analysis_FIX.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_pitch_analysis_core.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_pitch_analysis_core.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_pitch_est_tables.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_pitch_est_tables.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_prefilter_FIX.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_prefilter_FIX.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_process_NLSFs_FIX.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_process_NLSFs_FIX.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_process_gains_FIX.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_process_gains_FIX.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_quant_LTP_gains_FIX.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_quant_LTP_gains_FIX.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_range_coder.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_range_coder.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_regularize_correlations_FIX.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_regularize_correlations_FIX.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_resampler.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_resampler.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_resampler_down2.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_resampler_down2.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_resampler_down2_3.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_resampler_down2_3.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_resampler_down3.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_resampler_down3.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_resampler_private_AR2.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_resampler_private_AR2.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_resampler_private_ARMA4.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_resampler_private_ARMA4.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_resampler_private_IIR_FIR.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_resampler_private_IIR_FIR.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_resampler_private_copy.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_resampler_private_copy.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_resampler_private_down4.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_resampler_private_down4.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_resampler_private_down_FIR.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_resampler_private_down_FIR.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_resampler_private_up2_HQ.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_resampler_private_up2_HQ.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_resampler_private_up4.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_resampler_private_up4.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_resampler_rom.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_resampler_rom.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_resampler_up2.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_resampler_up2.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_residual_energy16_FIX.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_residual_energy16_FIX.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_residual_energy_FIX.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_residual_energy_FIX.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_scale_copy_vector16.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_scale_copy_vector16.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_scale_vector.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_scale_vector.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_schur.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_schur.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_schur64.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_schur64.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_shell_coder.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_shell_coder.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_sigm_Q15.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_sigm_Q15.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_solve_LS_FIX.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_solve_LS_FIX.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_sort.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_sort.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_sum_sqr_shift.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_sum_sqr_shift.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_tables_LTP.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_tables_LTP.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_tables_NLSF_CB0_10.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_tables_NLSF_CB0_10.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_tables_NLSF_CB0_16.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_tables_NLSF_CB0_16.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_tables_NLSF_CB1_10.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_tables_NLSF_CB1_10.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_tables_NLSF_CB1_16.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_tables_NLSF_CB1_16.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_tables_gain.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_tables_gain.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_tables_other.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_tables_other.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_tables_pitch_lag.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_tables_pitch_lag.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_tables_pulses_per_block.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_tables_pulses_per_block.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_tables_sign.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_tables_sign.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_tables_type_offset.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_tables_type_offset.c`

 * *Files identical despite different names*

### Comparing `pysilk-mod-1.6.0/src/silk/src/SKP_Silk_warped_autocorrelation_FIX.c` & `pysilk-mod-1.6.2/src/silk/src/SKP_Silk_warped_autocorrelation_FIX.c`

 * *Files identical despite different names*

