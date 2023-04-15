# Comparing `tmp/jaeger-1.3.4.tar.gz` & `tmp/jaeger-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaeger-1.3.4.tar", max compression
+gzip compressed data, was "jaeger-1.4.0.tar", max compression
```

## Comparing `jaeger-1.3.4.tar` & `jaeger-1.4.0.tar`

### file list

```diff
@@ -1,74 +1,74 @@
--rw-r--r--   0        0        0     1504 2023-04-13 00:20:40.277423 jaeger-1.3.4/LICENSE.md
--rw-r--r--   0        0        0     2386 2023-04-13 00:20:40.277643 jaeger-1.3.4/README.md
--rw-r--r--   0        0        0     3309 2023-04-13 00:20:40.285686 jaeger-1.3.4/pyproject.toml
--rw-r--r--   0        0        0     1745 2023-04-13 00:20:40.286122 jaeger-1.3.4/python/jaeger/__init__.py
--rw-r--r--   0        0        0    20331 2023-04-13 00:20:40.286430 jaeger-1.3.4/python/jaeger/__main__.py
--rw-r--r--   0        0        0       61 2023-04-13 00:20:40.286736 jaeger-1.3.4/python/jaeger/actor/__init__.py
--rw-r--r--   0        0        0     5033 2023-04-13 00:20:40.286972 jaeger-1.3.4/python/jaeger/actor/actor.py
--rw-r--r--   0        0        0      816 2023-04-13 00:20:40.287269 jaeger-1.3.4/python/jaeger/actor/commands/__init__.py
--rw-r--r--   0        0        0     1029 2023-04-13 00:20:40.287485 jaeger-1.3.4/python/jaeger/actor/commands/alerts.py
--rw-r--r--   0        0        0     1182 2023-04-13 00:20:40.287730 jaeger-1.3.4/python/jaeger/actor/commands/can.py
--rw-r--r--   0        0        0     3381 2023-04-13 00:20:40.287971 jaeger-1.3.4/python/jaeger/actor/commands/chiller.py
--rw-r--r--   0        0        0    33052 2023-04-13 00:20:40.288303 jaeger-1.3.4/python/jaeger/actor/commands/configuration.py
--rw-r--r--   0        0        0      721 2023-04-13 00:20:40.288552 jaeger-1.3.4/python/jaeger/actor/commands/debug.py
--rw-r--r--   0        0        0     2690 2023-04-13 00:20:40.288773 jaeger-1.3.4/python/jaeger/actor/commands/disable.py
--rw-r--r--   0        0        0    14510 2023-04-13 00:20:40.289025 jaeger-1.3.4/python/jaeger/actor/commands/fvc.py
--rw-r--r--   0        0        0    11347 2023-04-13 00:20:40.289269 jaeger-1.3.4/python/jaeger/actor/commands/home.py
--rw-r--r--   0        0        0     5314 2023-04-13 00:20:40.289486 jaeger-1.3.4/python/jaeger/actor/commands/ieb.py
--rw-r--r--   0        0        0     1410 2023-04-13 00:20:40.289680 jaeger-1.3.4/python/jaeger/actor/commands/pollers.py
--rw-r--r--   0        0        0    16070 2023-04-13 00:20:40.289991 jaeger-1.3.4/python/jaeger/actor/commands/positioner.py
--rw-r--r--   0        0        0     9994 2023-04-13 00:20:40.290231 jaeger-1.3.4/python/jaeger/actor/commands/power.py
--rw-r--r--   0        0        0      990 2023-04-13 00:20:40.290434 jaeger-1.3.4/python/jaeger/actor/commands/snapshot.py
--rw-r--r--   0        0        0     1323 2023-04-13 00:20:40.290639 jaeger-1.3.4/python/jaeger/actor/commands/talk.py
--rw-r--r--   0        0        0     1034 2023-04-13 00:20:40.290963 jaeger-1.3.4/python/jaeger/actor/commands/testing.py
--rw-r--r--   0        0        0     3579 2023-04-13 00:20:40.291184 jaeger-1.3.4/python/jaeger/actor/commands/unwind.py
--rw-r--r--   0        0        0      949 2023-04-13 00:20:40.291388 jaeger-1.3.4/python/jaeger/actor/commands/version.py
--rw-r--r--   0        0        0    14065 2023-04-13 00:20:40.291629 jaeger-1.3.4/python/jaeger/alerts.py
--rw-r--r--   0        0        0    21709 2023-04-13 00:20:40.291936 jaeger-1.3.4/python/jaeger/can.py
--rw-r--r--   0        0        0     5220 2023-04-13 00:20:40.292193 jaeger-1.3.4/python/jaeger/chiller.py
--rw-r--r--   0        0        0     3964 2023-04-13 00:20:40.292482 jaeger-1.3.4/python/jaeger/commands/__init__.py
--rw-r--r--   0        0        0    22135 2023-04-13 00:20:40.292772 jaeger-1.3.4/python/jaeger/commands/base.py
--rw-r--r--   0        0        0     9010 2023-04-13 00:20:40.293027 jaeger-1.3.4/python/jaeger/commands/bootloader.py
--rw-r--r--   0        0        0    12181 2023-04-13 00:20:40.293252 jaeger-1.3.4/python/jaeger/commands/calibration.py
--rw-r--r--   0        0        0    10788 2023-04-13 00:20:40.293480 jaeger-1.3.4/python/jaeger/commands/goto.py
--rw-r--r--   0        0        0     6013 2023-04-13 00:20:40.293687 jaeger-1.3.4/python/jaeger/commands/status.py
--rw-r--r--   0        0        0    26689 2023-04-13 00:20:40.293995 jaeger-1.3.4/python/jaeger/commands/trajectory.py
--rw-r--r--   0        0        0    10030 2023-04-13 00:20:40.294321 jaeger-1.3.4/python/jaeger/etc/chiller_APO.yaml
--rw-r--r--   0        0        0     7487 2023-04-13 00:20:40.294546 jaeger-1.3.4/python/jaeger/etc/chiller_APO_variables.csv
--rw-r--r--   0        0        0     1317 2023-04-13 00:20:40.294767 jaeger-1.3.4/python/jaeger/etc/fvc.yaml
--rw-r--r--   0        0        0    10541 2023-04-13 00:20:40.294986 jaeger-1.3.4/python/jaeger/etc/ieb_APO.yaml
--rw-r--r--   0        0        0    10539 2023-04-13 00:20:40.295210 jaeger-1.3.4/python/jaeger/etc/ieb_LCO.yaml
--rw-r--r--   0        0        0     3256 2023-04-13 00:20:40.295426 jaeger-1.3.4/python/jaeger/etc/jaeger_APO.yml
--rw-r--r--   0        0        0     3188 2023-04-13 00:20:40.295631 jaeger-1.3.4/python/jaeger/etc/jaeger_LCO.yml
--rw-r--r--   0        0        0     8711 2023-04-13 00:20:40.295846 jaeger-1.3.4/python/jaeger/etc/schema.json
--rw-r--r--   0        0        0     1815 2023-04-13 00:20:40.296116 jaeger-1.3.4/python/jaeger/etc/sextants/epfl.yaml
--rw-r--r--   0        0        0     2367 2023-04-13 00:20:40.296297 jaeger-1.3.4/python/jaeger/etc/sextants/osu.yaml
--rw-r--r--   0        0        0     1512 2023-04-13 00:20:40.296535 jaeger-1.3.4/python/jaeger/etc/sextants/schema.json
--rw-r--r--   0        0        0     2364 2023-04-13 00:20:40.296761 jaeger-1.3.4/python/jaeger/etc/sextants/uw.yaml
--rw-r--r--   0        0        0     3545 2023-04-13 00:20:40.296967 jaeger-1.3.4/python/jaeger/exceptions.py
--rw-r--r--   0        0        0    51683 2023-04-13 00:20:40.297390 jaeger-1.3.4/python/jaeger/fps.py
--rw-r--r--   0        0        0    39277 2023-04-13 00:20:40.297790 jaeger-1.3.4/python/jaeger/fvc.py
--rw-r--r--   0        0        0     4510 2023-04-13 00:20:40.301959 jaeger-1.3.4/python/jaeger/ieb.py
--rw-r--r--   0        0        0      162 2023-04-13 00:20:40.302244 jaeger-1.3.4/python/jaeger/interfaces/__init__.py
--rw-r--r--   0        0        0     1142 2023-04-13 00:20:40.302443 jaeger-1.3.4/python/jaeger/interfaces/bus.py
--rw-r--r--   0        0        0     6759 2023-04-13 00:20:40.302734 jaeger-1.3.4/python/jaeger/interfaces/cannet.py
--rw-r--r--   0        0        0    12892 2023-04-13 00:20:40.302984 jaeger-1.3.4/python/jaeger/interfaces/message.py
--rw-r--r--   0        0        0     1874 2023-04-13 00:20:40.303204 jaeger-1.3.4/python/jaeger/interfaces/notifier.py
--rw-r--r--   0        0        0     1199 2023-04-13 00:20:40.303397 jaeger-1.3.4/python/jaeger/interfaces/virtual.py
--rw-r--r--   0        0        0    19795 2023-04-13 00:20:40.303664 jaeger-1.3.4/python/jaeger/kaiju.py
--rw-r--r--   0        0        0     8034 2023-04-13 00:20:40.303916 jaeger-1.3.4/python/jaeger/maskbits.py
--rw-r--r--   0        0        0     7296 2023-04-13 00:20:40.304126 jaeger-1.3.4/python/jaeger/plotting.py
--rw-r--r--   0        0        0    18121 2023-04-13 00:20:40.304401 jaeger-1.3.4/python/jaeger/positioner.py
--rw-r--r--   0        0        0        0 2023-04-13 00:20:40.304684 jaeger-1.3.4/python/jaeger/scripts/__init__.py
--rw-r--r--   0        0        0     1825 2023-04-13 00:20:40.304899 jaeger-1.3.4/python/jaeger/scripts/generate_chiller_yaml.py
--rwxr-xr-x   0        0        0    19977 2023-04-13 00:20:40.305203 jaeger-1.3.4/python/jaeger/scripts/robotcalib.py
--rw-r--r--   0        0        0      293 2023-04-13 00:20:40.305615 jaeger-1.3.4/python/jaeger/target/__init__.py
--rw-r--r--   0        0        0    62360 2023-04-13 00:20:40.306077 jaeger-1.3.4/python/jaeger/target/configuration.py
--rw-r--r--   0        0        0     8410 2023-04-13 00:20:40.306357 jaeger-1.3.4/python/jaeger/target/design.py
--rw-r--r--   0        0        0    11807 2023-04-13 00:20:40.306683 jaeger-1.3.4/python/jaeger/target/tools.py
--rw-r--r--   0        0        0    12403 2023-04-13 00:20:40.306916 jaeger-1.3.4/python/jaeger/testing.py
--rw-r--r--   0        0        0       60 2023-04-13 00:20:40.307196 jaeger-1.3.4/python/jaeger/utils/__init__.py
--rw-r--r--   0        0        0     9562 2023-04-13 00:20:40.307427 jaeger-1.3.4/python/jaeger/utils/database.py
--rw-r--r--   0        0        0    14766 2023-04-13 00:20:40.307671 jaeger-1.3.4/python/jaeger/utils/helpers.py
--rw-r--r--   0        0        0     9549 2023-04-13 00:20:40.307900 jaeger-1.3.4/python/jaeger/utils/utils.py
--rw-r--r--   0        0        0     3926 1970-01-01 00:00:00.000000 jaeger-1.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1504 2023-04-15 22:03:57.419847 jaeger-1.4.0/LICENSE.md
+-rw-r--r--   0        0        0     2386 2023-04-15 22:03:57.420070 jaeger-1.4.0/README.md
+-rw-r--r--   0        0        0     3288 2023-04-15 22:03:57.429053 jaeger-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1745 2023-04-15 22:03:57.429493 jaeger-1.4.0/python/jaeger/__init__.py
+-rw-r--r--   0        0        0    20331 2023-04-15 22:03:57.429845 jaeger-1.4.0/python/jaeger/__main__.py
+-rw-r--r--   0        0        0       61 2023-04-15 22:03:57.430189 jaeger-1.4.0/python/jaeger/actor/__init__.py
+-rw-r--r--   0        0        0     5033 2023-04-15 22:03:57.430448 jaeger-1.4.0/python/jaeger/actor/actor.py
+-rw-r--r--   0        0        0      816 2023-04-15 22:03:57.430761 jaeger-1.4.0/python/jaeger/actor/commands/__init__.py
+-rw-r--r--   0        0        0     1029 2023-04-15 22:03:57.431002 jaeger-1.4.0/python/jaeger/actor/commands/alerts.py
+-rw-r--r--   0        0        0     1182 2023-04-15 22:03:57.431242 jaeger-1.4.0/python/jaeger/actor/commands/can.py
+-rw-r--r--   0        0        0     3381 2023-04-15 22:03:57.431492 jaeger-1.4.0/python/jaeger/actor/commands/chiller.py
+-rw-r--r--   0        0        0    34192 2023-04-15 22:03:57.431854 jaeger-1.4.0/python/jaeger/actor/commands/configuration.py
+-rw-r--r--   0        0        0      721 2023-04-15 22:03:57.432140 jaeger-1.4.0/python/jaeger/actor/commands/debug.py
+-rw-r--r--   0        0        0     2690 2023-04-15 22:03:57.432390 jaeger-1.4.0/python/jaeger/actor/commands/disable.py
+-rw-r--r--   0        0        0    14510 2023-04-15 22:03:57.432686 jaeger-1.4.0/python/jaeger/actor/commands/fvc.py
+-rw-r--r--   0        0        0    11347 2023-04-15 22:03:57.433054 jaeger-1.4.0/python/jaeger/actor/commands/home.py
+-rw-r--r--   0        0        0     5314 2023-04-15 22:03:57.433330 jaeger-1.4.0/python/jaeger/actor/commands/ieb.py
+-rw-r--r--   0        0        0     1410 2023-04-15 22:03:57.433645 jaeger-1.4.0/python/jaeger/actor/commands/pollers.py
+-rw-r--r--   0        0        0    16070 2023-04-15 22:03:57.433995 jaeger-1.4.0/python/jaeger/actor/commands/positioner.py
+-rw-r--r--   0        0        0     9994 2023-04-15 22:03:57.434262 jaeger-1.4.0/python/jaeger/actor/commands/power.py
+-rw-r--r--   0        0        0      990 2023-04-15 22:03:57.434496 jaeger-1.4.0/python/jaeger/actor/commands/snapshot.py
+-rw-r--r--   0        0        0     1323 2023-04-15 22:03:57.434749 jaeger-1.4.0/python/jaeger/actor/commands/talk.py
+-rw-r--r--   0        0        0     1034 2023-04-15 22:03:57.434961 jaeger-1.4.0/python/jaeger/actor/commands/testing.py
+-rw-r--r--   0        0        0     3579 2023-04-15 22:03:57.435181 jaeger-1.4.0/python/jaeger/actor/commands/unwind.py
+-rw-r--r--   0        0        0      949 2023-04-15 22:03:57.435383 jaeger-1.4.0/python/jaeger/actor/commands/version.py
+-rw-r--r--   0        0        0    14065 2023-04-15 22:03:57.435651 jaeger-1.4.0/python/jaeger/alerts.py
+-rw-r--r--   0        0        0    21709 2023-04-15 22:03:57.435980 jaeger-1.4.0/python/jaeger/can.py
+-rw-r--r--   0        0        0     5220 2023-04-15 22:03:57.436234 jaeger-1.4.0/python/jaeger/chiller.py
+-rw-r--r--   0        0        0     3964 2023-04-15 22:03:57.436555 jaeger-1.4.0/python/jaeger/commands/__init__.py
+-rw-r--r--   0        0        0    22135 2023-04-15 22:03:57.436887 jaeger-1.4.0/python/jaeger/commands/base.py
+-rw-r--r--   0        0        0     9010 2023-04-15 22:03:57.437156 jaeger-1.4.0/python/jaeger/commands/bootloader.py
+-rw-r--r--   0        0        0    12181 2023-04-15 22:03:57.437395 jaeger-1.4.0/python/jaeger/commands/calibration.py
+-rw-r--r--   0        0        0    10788 2023-04-15 22:03:57.437633 jaeger-1.4.0/python/jaeger/commands/goto.py
+-rw-r--r--   0        0        0     6013 2023-04-15 22:03:57.437856 jaeger-1.4.0/python/jaeger/commands/status.py
+-rw-r--r--   0        0        0    26689 2023-04-15 22:03:57.438178 jaeger-1.4.0/python/jaeger/commands/trajectory.py
+-rw-r--r--   0        0        0    10030 2023-04-15 22:03:57.438541 jaeger-1.4.0/python/jaeger/etc/chiller_APO.yaml
+-rw-r--r--   0        0        0     7487 2023-04-15 22:03:57.438787 jaeger-1.4.0/python/jaeger/etc/chiller_APO_variables.csv
+-rw-r--r--   0        0        0     1317 2023-04-15 22:03:57.439437 jaeger-1.4.0/python/jaeger/etc/fvc.yaml
+-rw-r--r--   0        0        0    10541 2023-04-15 22:03:57.439695 jaeger-1.4.0/python/jaeger/etc/ieb_APO.yaml
+-rw-r--r--   0        0        0    10539 2023-04-15 22:03:57.439976 jaeger-1.4.0/python/jaeger/etc/ieb_LCO.yaml
+-rw-r--r--   0        0        0     3256 2023-04-15 22:03:57.440200 jaeger-1.4.0/python/jaeger/etc/jaeger_APO.yml
+-rw-r--r--   0        0        0     3188 2023-04-15 22:03:57.440718 jaeger-1.4.0/python/jaeger/etc/jaeger_LCO.yml
+-rw-r--r--   0        0        0     8711 2023-04-15 22:03:57.440981 jaeger-1.4.0/python/jaeger/etc/schema.json
+-rw-r--r--   0        0        0     1815 2023-04-15 22:03:57.441655 jaeger-1.4.0/python/jaeger/etc/sextants/epfl.yaml
+-rw-r--r--   0        0        0     2367 2023-04-15 22:03:57.441902 jaeger-1.4.0/python/jaeger/etc/sextants/osu.yaml
+-rw-r--r--   0        0        0     1512 2023-04-15 22:03:57.442282 jaeger-1.4.0/python/jaeger/etc/sextants/schema.json
+-rw-r--r--   0        0        0     2364 2023-04-15 22:03:57.442536 jaeger-1.4.0/python/jaeger/etc/sextants/uw.yaml
+-rw-r--r--   0        0        0     3545 2023-04-15 22:03:57.442785 jaeger-1.4.0/python/jaeger/exceptions.py
+-rw-r--r--   0        0        0    51683 2023-04-15 22:03:57.443232 jaeger-1.4.0/python/jaeger/fps.py
+-rw-r--r--   0        0        0    39277 2023-04-15 22:03:57.443681 jaeger-1.4.0/python/jaeger/fvc.py
+-rw-r--r--   0        0        0     4510 2023-04-15 22:03:57.443941 jaeger-1.4.0/python/jaeger/ieb.py
+-rw-r--r--   0        0        0      162 2023-04-15 22:03:57.444261 jaeger-1.4.0/python/jaeger/interfaces/__init__.py
+-rw-r--r--   0        0        0     1142 2023-04-15 22:03:57.444479 jaeger-1.4.0/python/jaeger/interfaces/bus.py
+-rw-r--r--   0        0        0     6759 2023-04-15 22:03:57.444766 jaeger-1.4.0/python/jaeger/interfaces/cannet.py
+-rw-r--r--   0        0        0    12892 2023-04-15 22:03:57.445051 jaeger-1.4.0/python/jaeger/interfaces/message.py
+-rw-r--r--   0        0        0     1874 2023-04-15 22:03:57.445315 jaeger-1.4.0/python/jaeger/interfaces/notifier.py
+-rw-r--r--   0        0        0     1199 2023-04-15 22:03:57.445595 jaeger-1.4.0/python/jaeger/interfaces/virtual.py
+-rw-r--r--   0        0        0    19795 2023-04-15 22:03:57.445895 jaeger-1.4.0/python/jaeger/kaiju.py
+-rw-r--r--   0        0        0     8034 2023-04-15 22:03:57.446328 jaeger-1.4.0/python/jaeger/maskbits.py
+-rw-r--r--   0        0        0     7296 2023-04-15 22:03:57.446600 jaeger-1.4.0/python/jaeger/plotting.py
+-rw-r--r--   0        0        0    18121 2023-04-15 22:03:57.447266 jaeger-1.4.0/python/jaeger/positioner.py
+-rw-r--r--   0        0        0        0 2023-04-15 22:03:57.447606 jaeger-1.4.0/python/jaeger/scripts/__init__.py
+-rw-r--r--   0        0        0     1825 2023-04-15 22:03:57.447908 jaeger-1.4.0/python/jaeger/scripts/generate_chiller_yaml.py
+-rwxr-xr-x   0        0        0    19977 2023-04-15 22:03:57.448252 jaeger-1.4.0/python/jaeger/scripts/robotcalib.py
+-rw-r--r--   0        0        0      293 2023-04-15 22:03:57.448655 jaeger-1.4.0/python/jaeger/target/__init__.py
+-rw-r--r--   0        0        0    64242 2023-04-15 22:03:57.449167 jaeger-1.4.0/python/jaeger/target/configuration.py
+-rw-r--r--   0        0        0     8598 2023-04-15 22:03:57.449600 jaeger-1.4.0/python/jaeger/target/design.py
+-rw-r--r--   0        0        0    11807 2023-04-15 22:03:57.449874 jaeger-1.4.0/python/jaeger/target/tools.py
+-rw-r--r--   0        0        0    12403 2023-04-15 22:03:57.450157 jaeger-1.4.0/python/jaeger/testing.py
+-rw-r--r--   0        0        0       60 2023-04-15 22:03:57.450443 jaeger-1.4.0/python/jaeger/utils/__init__.py
+-rw-r--r--   0        0        0     9562 2023-04-15 22:03:57.450682 jaeger-1.4.0/python/jaeger/utils/database.py
+-rw-r--r--   0        0        0    14766 2023-04-15 22:03:57.450935 jaeger-1.4.0/python/jaeger/utils/helpers.py
+-rw-r--r--   0        0        0     9549 2023-04-15 22:03:57.451173 jaeger-1.4.0/python/jaeger/utils/utils.py
+-rw-r--r--   0        0        0     3926 1970-01-01 00:00:00.000000 jaeger-1.4.0/PKG-INFO
```

### Comparing `jaeger-1.3.4/LICENSE.md` & `jaeger-1.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/README.md` & `jaeger-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/pyproject.toml` & `jaeger-1.4.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jaeger"
-version = "1.3.4"
+version = "1.4.0"
 description = "Controllers for the SDSS-V FPS"
 authors = ["José Sánchez-Gallego <gallegoj@uw.edu>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/sdss/jaeger"
 repository = "https://github.com/sdss/jaeger"
 documentation = "https://sdss-jaeger.readthedocs.io/en/latest/"
@@ -25,15 +25,15 @@
 [tool.poetry.dependencies]
 python = "^3.8,<3.12"
 sdss-drift = "^1.0.0"
 sdss-clu = "^1.9.1"
 sdsstools = "^1.0.0"
 sdssdb = "^0.6.0"
 sdss-kaiju = "^1.3.1"
-sdss-coordio = "^1.6.0"
+sdss-coordio = "^1.7.0"
 astropy = "^5.0.0"
 pydl = "1.0.0rc1"
 click_default_group = "^1.2.2"
 pandas = "^1.3.4"
 tables = "^3.6.1"
 "zc.lockfile" = "^2.0"
 
@@ -43,15 +43,14 @@
 flake8 = ">=3.7.9"
 doc8 = ">=0.8.0"
 pytest = ">=5.2.2"
 progressbar2 = ">=3.39.3"
 pytest-asyncio = ">=0.10.0"
 pytest-cov = ">=2.8.1"
 pytest-sugar = ">=0.9.2"
-codecov = ">=2.0.15"
 isort = ">=5.0.0"
 coverage = {version = ">=5.0", extras = ["toml"]}
 Sphinx = {version = ">=3.0"}
 sphinx-click = {version = ">=2.3.0"}
 ipdb = ">=0.13.3"
 autopep8 = ">=1.5.4"
 black = {version = ">=21.10b0", allow-prereleases = true}
```

### Comparing `jaeger-1.3.4/python/jaeger/__init__.py` & `jaeger-1.4.0/python/jaeger/__init__.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/python/jaeger/__main__.py` & `jaeger-1.4.0/python/jaeger/__main__.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/python/jaeger/actor/actor.py` & `jaeger-1.4.0/python/jaeger/actor/actor.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/python/jaeger/actor/commands/__init__.py` & `jaeger-1.4.0/python/jaeger/actor/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/python/jaeger/actor/commands/alerts.py` & `jaeger-1.4.0/python/jaeger/actor/commands/alerts.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/python/jaeger/actor/commands/can.py` & `jaeger-1.4.0/python/jaeger/actor/commands/can.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/python/jaeger/actor/commands/chiller.py` & `jaeger-1.4.0/python/jaeger/actor/commands/chiller.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/python/jaeger/actor/commands/configuration.py` & `jaeger-1.4.0/python/jaeger/actor/commands/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,17 +53,19 @@
     design_id: int | None = None,
     preload: bool = False,
     no_clone: bool = False,
     scale: float | None = None,
     fudge_factor: float | None = None,
     epoch: float | None = None,
     epoch_delay: float = 0.0,
+    boss_wavelength: float | None = None,
+    apogee_wavelength: float | None = None,
     get_paths: bool = True,
     path_generation_mode: str | None = None,
-    safety_factor: float = 0.1,
+    safety_factor: float = 1,
     offset_min_skybrightness: float = 0.5,
 ):
     """Helper to load or preload a design."""
 
     if design_id is None:
         design_id, _epoch_delay = get_designid_from_queue(
             pop=not preload,
@@ -200,14 +202,16 @@
 
             design = await Design.create_async(
                 design_id,
                 epoch=epoch,
                 scale=scale,
                 safety_factor=safety_factor,
                 offset_min_skybrightness=offset_min_skybrightness,
+                boss_wavelength=boss_wavelength,
+                apogee_wavelength=apogee_wavelength,
             )
         except Exception as err:
             command.error(error=f"Failed retrieving design: {err}")
             return False
 
         configuration = design.configuration
 
@@ -252,14 +256,24 @@
 @click.option(
     "--epoch-delay",
     type=float,
     default=0.0,
     help="A delay in seconds for the epoch for which the configuration is calculated.",
 )
 @click.option(
+    "--boss-wavelength",
+    type=click.FloatRange(3000, 10000),
+    help="Optimise positioning of BOSS fibres to this wavelength.",
+)
+@click.option(
+    "--apogee-wavelength",
+    type=click.FloatRange(16000, 17000),
+    help="Optimise positioning of APOGEE fibres to this wavelength.",
+)
+@click.option(
     "--from-positions",
     is_flag=True,
     help="Loads a configuration from the current robot positions.",
 )
 @click.option(
     "--from-preloaded",
     is_flag=True,
@@ -307,15 +321,15 @@
     "--path-generation-mode",
     type=click.Choice(["greedy", "mdp"], case_sensitive=False),
     help="The path generation algorithm to use.",
 )
 @click.option(
     "--safety-factor",
     type=float,
-    default=0.1,
+    default=1,
     help="Safety factor to pass to the offset calculation function.",
 )
 @click.option(
     "--offset-min-skybrightness",
     type=float,
     default=0.5,
     help="Minimum sky brightness for the offset.",
@@ -328,23 +342,25 @@
     reload: bool = False,
     replace: bool = False,
     from_positions: bool = False,
     from_preloaded: bool = False,
     generate_paths: bool = False,
     epoch: float | None = None,
     epoch_delay: float = 0.0,
+    apogee_wavelength: float | None = None,
+    boss_wavelength: float | None = None,
     ingest: bool = False,
     write_summary: bool = False,
     execute: bool = False,
     reissue: bool = False,
     scale: float | None = None,
     fudge_factor: float | None = None,
     no_clone: bool = False,
     path_generation_mode: str | None = None,
-    safety_factor: float = 0.1,
+    safety_factor: float = 1,
     offset_min_skybrightness: float = 0.5,
 ):
     """Creates and ingests a configuration from a design in the database."""
 
     assert command.actor is not None
 
     if reissue is True:
@@ -379,14 +395,16 @@
             design_id=designid,
             fudge_factor=fudge_factor,
             preload=False,
             no_clone=no_clone,
             scale=scale,
             epoch=epoch,
             epoch_delay=epoch_delay,
+            boss_wavelength=boss_wavelength,
+            apogee_wavelength=apogee_wavelength,
             get_paths=False,
             path_generation_mode=path_generation_mode,
             safety_factor=safety_factor,
             offset_min_skybrightness=offset_min_skybrightness,
         )
 
         if configuration is False:
@@ -551,14 +569,24 @@
 @click.option(
     "--epoch-delay",
     type=float,
     default=0.0,
     help="A delay in seconds for the epoch for which the configuration is calculated.",
 )
 @click.option(
+    "--boss-wavelength",
+    type=click.FloatRange(3000, 10000),
+    help="Optimise positioning of BOSS fibres to this wavelength.",
+)
+@click.option(
+    "--apogee-wavelength",
+    type=click.FloatRange(16000, 17000),
+    help="Optimise positioning of APOGEE fibres to this wavelength.",
+)
+@click.option(
     "--scale",
     type=float,
     help="Focal plane scale factor. If not passes, uses coordio default.",
 )
 @click.option(
     "--fudge-factor",
     type=float,
@@ -580,15 +608,15 @@
     "--clear",
     is_flag=True,
     help="Clears the preloaded configuration.",
 )
 @click.option(
     "--safety-factor",
     type=float,
-    default=0.1,
+    default=1,
     help="Safety factor to pass to the offset calculation function.",
 )
 @click.option(
     "--offset-min-skybrightness",
     type=float,
     default=0.5,
     help="Minimum sky brightness for the offset.",
@@ -597,20 +625,22 @@
 @timeout(180)
 async def preload(
     command: JaegerCommandType,
     fps: FPS,
     designid: int | None = None,
     epoch: float | None = None,
     epoch_delay: float = 0.0,
+    apogee_wavelength: float | None = None,
+    boss_wavelength: float | None = None,
     scale: float | None = None,
     fudge_factor: float | None = None,
     no_clone: bool = False,
     make_active: bool = True,
     clear: bool = False,
-    safety_factor: float = 0.1,
+    safety_factor: float = 1,
     offset_min_skybrightness: float = 0.5,
 ):
     """Preloads a design.
 
     Preloading a design works similar to loading it, but no files are generated, no
     database entry is created, no configuration_loaded keyword is output, and the
     new configuration is stored separately. To make the preloaded configuration
@@ -629,14 +659,16 @@
         design_id=designid,
         preload=True,
         no_clone=no_clone,
         scale=scale,
         fudge_factor=fudge_factor,
         epoch=epoch,
         epoch_delay=epoch_delay,
+        boss_wavelength=boss_wavelength,
+        apogee_wavelength=apogee_wavelength,
         safety_factor=safety_factor,
         offset_min_skybrightness=offset_min_skybrightness,
     )
 
     if configuration is False:
         # _load_design already issues an error so we just fail.
         return command.fail()
```

### Comparing `jaeger-1.3.4/python/jaeger/actor/commands/debug.py` & `jaeger-1.4.0/python/jaeger/actor/commands/debug.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/python/jaeger/actor/commands/disable.py` & `jaeger-1.4.0/python/jaeger/actor/commands/disable.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/python/jaeger/actor/commands/fvc.py` & `jaeger-1.4.0/python/jaeger/actor/commands/fvc.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/python/jaeger/actor/commands/home.py` & `jaeger-1.4.0/python/jaeger/actor/commands/home.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/python/jaeger/actor/commands/ieb.py` & `jaeger-1.4.0/python/jaeger/actor/commands/ieb.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/python/jaeger/actor/commands/pollers.py` & `jaeger-1.4.0/python/jaeger/actor/commands/pollers.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/python/jaeger/actor/commands/positioner.py` & `jaeger-1.4.0/python/jaeger/actor/commands/positioner.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/python/jaeger/actor/commands/power.py` & `jaeger-1.4.0/python/jaeger/actor/commands/power.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/python/jaeger/actor/commands/snapshot.py` & `jaeger-1.4.0/python/jaeger/actor/commands/snapshot.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/python/jaeger/actor/commands/talk.py` & `jaeger-1.4.0/python/jaeger/actor/commands/talk.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/python/jaeger/actor/commands/testing.py` & `jaeger-1.4.0/python/jaeger/actor/commands/testing.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/python/jaeger/actor/commands/unwind.py` & `jaeger-1.4.0/python/jaeger/actor/commands/unwind.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/python/jaeger/actor/commands/version.py` & `jaeger-1.4.0/python/jaeger/actor/commands/version.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/python/jaeger/alerts.py` & `jaeger-1.4.0/python/jaeger/alerts.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/python/jaeger/can.py` & `jaeger-1.4.0/python/jaeger/can.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/python/jaeger/chiller.py` & `jaeger-1.4.0/python/jaeger/chiller.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/python/jaeger/commands/__init__.py` & `jaeger-1.4.0/python/jaeger/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/python/jaeger/commands/base.py` & `jaeger-1.4.0/python/jaeger/commands/base.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/python/jaeger/commands/bootloader.py` & `jaeger-1.4.0/python/jaeger/commands/bootloader.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/python/jaeger/commands/calibration.py` & `jaeger-1.4.0/python/jaeger/commands/calibration.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/python/jaeger/commands/goto.py` & `jaeger-1.4.0/python/jaeger/commands/goto.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/python/jaeger/commands/status.py` & `jaeger-1.4.0/python/jaeger/commands/status.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/python/jaeger/commands/trajectory.py` & `jaeger-1.4.0/python/jaeger/commands/trajectory.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/python/jaeger/etc/chiller_APO.yaml` & `jaeger-1.4.0/python/jaeger/etc/chiller_APO.yaml`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/python/jaeger/etc/chiller_APO_variables.csv` & `jaeger-1.4.0/python/jaeger/etc/chiller_APO_variables.csv`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/python/jaeger/etc/fvc.yaml` & `jaeger-1.4.0/python/jaeger/etc/fvc.yaml`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/python/jaeger/etc/ieb_APO.yaml` & `jaeger-1.4.0/python/jaeger/etc/ieb_APO.yaml`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/python/jaeger/etc/ieb_LCO.yaml` & `jaeger-1.4.0/python/jaeger/etc/ieb_LCO.yaml`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/python/jaeger/etc/jaeger_APO.yml` & `jaeger-1.4.0/python/jaeger/etc/jaeger_APO.yml`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/python/jaeger/etc/jaeger_LCO.yml` & `jaeger-1.4.0/python/jaeger/etc/jaeger_LCO.yml`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/python/jaeger/etc/schema.json` & `jaeger-1.4.0/python/jaeger/etc/schema.json`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/python/jaeger/etc/sextants/epfl.yaml` & `jaeger-1.4.0/python/jaeger/etc/sextants/epfl.yaml`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/python/jaeger/etc/sextants/osu.yaml` & `jaeger-1.4.0/python/jaeger/etc/sextants/osu.yaml`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/python/jaeger/etc/sextants/schema.json` & `jaeger-1.4.0/python/jaeger/etc/sextants/schema.json`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/python/jaeger/etc/sextants/uw.yaml` & `jaeger-1.4.0/python/jaeger/etc/sextants/uw.yaml`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/python/jaeger/exceptions.py` & `jaeger-1.4.0/python/jaeger/exceptions.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/python/jaeger/fps.py` & `jaeger-1.4.0/python/jaeger/fps.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/python/jaeger/fvc.py` & `jaeger-1.4.0/python/jaeger/fvc.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/python/jaeger/ieb.py` & `jaeger-1.4.0/python/jaeger/ieb.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/python/jaeger/interfaces/bus.py` & `jaeger-1.4.0/python/jaeger/interfaces/bus.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/python/jaeger/interfaces/cannet.py` & `jaeger-1.4.0/python/jaeger/interfaces/cannet.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/python/jaeger/interfaces/message.py` & `jaeger-1.4.0/python/jaeger/interfaces/message.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/python/jaeger/interfaces/notifier.py` & `jaeger-1.4.0/python/jaeger/interfaces/notifier.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/python/jaeger/interfaces/virtual.py` & `jaeger-1.4.0/python/jaeger/interfaces/virtual.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/python/jaeger/kaiju.py` & `jaeger-1.4.0/python/jaeger/kaiju.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/python/jaeger/maskbits.py` & `jaeger-1.4.0/python/jaeger/maskbits.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/python/jaeger/plotting.py` & `jaeger-1.4.0/python/jaeger/plotting.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/python/jaeger/positioner.py` & `jaeger-1.4.0/python/jaeger/positioner.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/python/jaeger/scripts/generate_chiller_yaml.py` & `jaeger-1.4.0/python/jaeger/scripts/generate_chiller_yaml.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/python/jaeger/scripts/robotcalib.py` & `jaeger-1.4.0/python/jaeger/scripts/robotcalib.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/python/jaeger/target/configuration.py` & `jaeger-1.4.0/python/jaeger/target/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,23 +30,28 @@
     Observed,
     PositionerApogee,
     PositionerBoss,
     Site,
     Wok,
 )
 from coordio import __version__ as coordio_version
-from coordio.defaults import INST_TO_WAVE, POSITIONER_HEIGHT, calibration
+from coordio.defaults import (
+    INST_TO_WAVE,
+    POSITIONER_HEIGHT,
+    VALID_WAVELENGTHS,
+    calibration,
+)
 from kaiju import __version__ as kaiju_version
 from sdssdb.peewee.sdss5db import opsdb, targetdb
 from sdsstools.time import get_sjd
 
 from jaeger import FPS
 from jaeger import __version__ as jaeger_version
 from jaeger import config, log
-from jaeger.exceptions import JaegerError, TrajectoryError
+from jaeger.exceptions import JaegerError, JaegerUserWarning, TrajectoryError
 from jaeger.ieb import IEB
 from jaeger.kaiju import (
     decollide_in_executor,
     dump_robot_grid,
     get_path_pair_in_executor,
     get_robot_grid,
     get_snapshot_async,
@@ -99,14 +104,15 @@
         ("racat", numpy.float64, -999.0),
         ("deccat", numpy.float64, -999.0),
         ("pmra", numpy.float32, -999.0),
         ("pmdec", numpy.float32, -999.0),
         ("parallax", numpy.float32, -999.0),
         ("ra", numpy.float64, -999.0),
         ("dec", numpy.float64, -999.0),
+        ("lambda_design", numpy.float32, -999.0),
         ("lambda_eff", numpy.float32, -999.0),
         ("coord_epoch", numpy.float32, -999.0),
         ("spectrographId", numpy.int16, -999),
         ("fiberId", numpy.int16, -999),
         ("mag", numpy.dtype(("<f4", (5,))), [-999.0] * 5),
         ("optical_prov", "U30", ""),
         ("bp_mag", numpy.float32, -999.0),
@@ -852,29 +858,30 @@
                     "yFocal": row_data.yfocal,
                     "alpha": row_data.alpha,
                     "beta": row_data.beta,
                     "ra": row_data.ra_epoch,
                     "dec": row_data.dec_epoch,
                     "spectrographId": spec_id,
                     "fiberId": row_data.fiberId,
+                    "lambda_eff": row_data.wavelength,
                 }
             )
 
             # And now only the one that is associated with a target.
             if row_data.assigned == 1 and design and hole_id in design.target_data:
                 target = design.target_data[hole_id]
                 row.update(
                     {
                         "racat": target["ra"],
                         "deccat": target["dec"],
                         "pmra": target["pmra"] or -999.0,
                         "pmdec": target["pmdec"] or -999.0,
                         "parallax": target["parallax"] or -999.0,
                         "coord_epoch": target["epoch"] or -999.0,
-                        "lambda_eff": target["lambda_eff"] or -999.0,
+                        "lambda_design": target["lambda_eff"] or -999.0,
                         "catalogid": target["catalogid"] or -999.0,
                         "carton_to_target_pk": target["carton_to_target_pk"] or -999.0,
                         "cadence": target["cadence"] or "",
                         "firstcarton": target["carton"] or "",
                         "program": target["program"] or "",
                         "category": target["category"] or "",
                         "delta_ra": target["delta_ra"] or 0.0,
@@ -937,20 +944,28 @@
     assignment_data: AssignmentData
 
     def __init__(
         self,
         design: Design,
         epoch: float | None = None,
         scale: float | None = None,
+        boss_wavelength: float | None = None,
+        apogee_wavelength: float | None = None,
     ):
         super().__init__(scale=scale)
 
         self.design = design
         self.design_id = design.design_id
-        self.assignment_data = AssignmentData(self, epoch=epoch, scale=scale)
+        self.assignment_data = AssignmentData(
+            self,
+            epoch=epoch,
+            scale=scale,
+            boss_wavelength=boss_wavelength,
+            apogee_wavelength=apogee_wavelength,
+        )
 
         assert self.assignment_data.site.time
 
         self.epoch = self.assignment_data.site.time.jd
         self.scale = scale
 
     def __repr__(self):
@@ -1246,20 +1261,25 @@
     ]
 
     def __init__(
         self,
         configuration: Configuration | ManualConfiguration | DitheredConfiguration,
         observatory: Optional[str] = None,
         scale: float | None = None,
+        boss_wavelength: float | None = None,
+        apogee_wavelength: float | None = None,
     ):
         self.configuration = configuration
 
         self.design = configuration.design
         self.design_id = self.configuration.design_id
 
+        self.boss_wavelength = boss_wavelength or INST_TO_WAVE["Boss"]
+        self.apogee_wavelength = apogee_wavelength or INST_TO_WAVE["Apogee"]
+
         self.observatory: str
         if observatory is None:
             if self.design is None:
                 raise ValueError("Cannot determine observatory.")
             self.observatory = self.design.field.observatory.upper()
         else:
             self.observatory = observatory
@@ -1305,14 +1325,26 @@
         jd
             The Julian Date for which to compute the coordinates.
 
         """
 
         raise NotImplementedError("Must be overridden by subclasses.")
 
+    def _get_wavelength(self, fibre_type: str):
+        """Returns the wavelength for a given fibre type."""
+
+        if fibre_type == "APOGEE":
+            return self.apogee_wavelength
+        elif fibre_type == "BOSS":
+            return self.boss_wavelength
+        elif fibre_type == "Metrology":
+            return INST_TO_WAVE["GFA"]
+
+        raise ValueError(f"Invalid fibre type {fibre_type!r}.")
+
     def _create_fibre_table(self):
         """Creates an empty fibre table."""
 
         names, dtypes, defaults = zip(*self._columns)
 
         # Create empty dataframe with zero values. Fill out all the index data.
         npositioner = len(self.wok_data)
@@ -1325,16 +1357,25 @@
 
         i = 0
         for pid in self.wok_data.index.tolist():
             for ft in ["APOGEE", "BOSS", "Metrology"]:
                 base["positioner_id"][i] = pid
                 base["fibre_type"][i] = ft
                 base["hole_id"][i] = self.wok_data.loc[pid].holeID
+                base["wavelength"][i] = self._get_wavelength(ft)
                 i += 1
 
+        valid_wavelengths = numpy.array(list(VALID_WAVELENGTHS))
+        if not numpy.all(numpy.in1d(base["wavelength"], valid_wavelengths)):
+            warnings.warn(
+                "Using non-default wavelengths. "
+                "Focal plane transformation may be sub-optimal.",
+                JaegerUserWarning,
+            )
+
         fibre_table = pandas.DataFrame(base)
 
         fibre_table.fibre_type = fibre_table.fibre_type.astype("category")
         fibre_table.hole_id = fibre_table.hole_id.astype("string")
 
         fibre_table.set_index(["positioner_id", "fibre_type"], inplace=True)
         fibre_table = fibre_table.sort_index()
@@ -1528,15 +1569,15 @@
         position_angle: float = 0.0,
         update: bool = True,
         **kwargs,
     ):
         """Converts from ICRS coordinates."""
 
         hole_id = self.wok_data.loc[positioner_id].holeID
-        wavelength = INST_TO_WAVE.get(fibre_type.capitalize(), INST_TO_WAVE["GFA"])
+        wavelength = self._get_wavelength(fibre_type)
 
         with warnings.catch_warnings():
             warnings.simplefilter("ignore", RuntimeWarning)
 
             ra = target_data["ra"]
             if target_data["delta_ra"] is not None:
                 # delta_ra/delta_dec are in arcsec.
@@ -1566,14 +1607,15 @@
             observed = Observed(icrs_epoch, wavelength=wavelength, site=self.site)
             field = Field(observed, field_center=self.boresight)
             focal = FocalPlane(
                 field,
                 wavelength=wavelength,
                 site=self.site,
                 fpScale=self.scale,
+                use_closest_wavelength=True,
             )
             wok = Wok(focal, site=self.site, obsAngle=position_angle)
 
             positioner, tangent = wok_to_positioner(
                 hole_id,
                 self.site.name,
                 fibre_type,
@@ -1586,15 +1628,14 @@
             row = self._defaults.copy()
         else:
             row = {}
 
         row.update(
             {
                 "hole_id": hole_id,
-                "wavelength": INST_TO_WAVE[fibre_type.capitalize()],
                 "ra_icrs": icrs[0, 0],
                 "dec_icrs": icrs[0, 1],
                 "ra_epoch": icrs_epoch[0, 0],
                 "dec_epoch": icrs_epoch[0, 1],
                 "alt": observed[0, 0],
                 "az": observed[0, 1],
                 "xfocal": focal[0, 0],
@@ -1603,14 +1644,15 @@
                 "ywok": wok[0, 1],
                 "zwok": wok[0, 2],
                 "xtangent": tangent[0],
                 "ytangent": tangent[1],
                 "ztangent": tangent[2],
                 "alpha": positioner[0],
                 "beta": positioner[1],
+                "wavelength": wavelength,
             }
         )
         row.update(kwargs)
 
         if update:
             self.fibre_table.loc[
                 (positioner_id, fibre_type), row.keys()
@@ -1626,15 +1668,19 @@
         beta: float,
         position_angle: float | None = None,
         update: bool = True,
         **kwargs,
     ):
         """Converts from positioner to ICRS coordinates."""
 
-        wavelength = INST_TO_WAVE.get(fibre_type.capitalize(), INST_TO_WAVE["GFA"])
+        ft_row = self.fibre_table.loc[(positioner_id, fibre_type), :]
+        if ft_row.assigned:
+            wavelength = self._get_wavelength(fibre_type)
+        else:
+            wavelength = INST_TO_WAVE.get(fibre_type.capitalize(), INST_TO_WAVE["GFA"])
 
         assert self.site.time
 
         if position_angle is None:
             position_angle = self.design.field.position_angle if self.design else 0.0
 
         hole_id = self.wok_data.at[positioner_id, "holeID"]
@@ -1651,14 +1697,15 @@
             )
 
             focal = FocalPlane(
                 Wok([wok], site=self.site, obsAngle=position_angle),
                 wavelength=wavelength,
                 site=self.site,
                 fpScale=self.scale,
+                use_closest_wavelength=True,
             )
 
             if self.boresight is not None:
                 field = Field(focal, field_center=self.boresight)
                 obs = Observed(field, site=self.site, wavelength=wavelength)
                 icrs = ICRS(obs, epoch=self.site.time.jd)
             else:
@@ -1704,16 +1751,23 @@
 
     def __init__(
         self,
         configuration: Configuration | DitheredConfiguration,
         epoch: float | None = None,
         compute_coordinates: bool = True,
         scale: float | None = None,
+        boss_wavelength: float | None = None,
+        apogee_wavelength: float | None = None,
     ):
-        super().__init__(configuration, scale=scale)
+        super().__init__(
+            configuration,
+            scale=scale,
+            boss_wavelength=boss_wavelength,
+            apogee_wavelength=apogee_wavelength,
+        )
 
         if compute_coordinates:
             self.compute_coordinates(epoch)
 
     def compute_coordinates(self, jd: Optional[float] = None):
         """Computes coordinates in different systems.
```

### Comparing `jaeger-1.3.4/python/jaeger/target/design.py` & `jaeger-1.4.0/python/jaeger/target/design.py`

 * *Files 5% similar despite different names*

```diff
@@ -230,25 +230,29 @@
 
     @classmethod
     async def create_async(
         cls,
         design_id: int,
         epoch: float | None = None,
         scale: float | None = None,
+        boss_wavelength: float | None = None,
+        apogee_wavelength: float | None = None,
         **kwargs,
     ):
         """Returns a design while creating the configuration in an executor."""
 
         self = cls(design_id, load_configuration=False, **kwargs)
 
         configuration = await run_in_executor(
             Configuration,
             self,
             epoch=epoch,
             scale=scale,
+            boss_wavelength=boss_wavelength,
+            apogee_wavelength=apogee_wavelength,
         )
         self.configuration = configuration
 
         return self
 
     def __repr__(self):
         return f"<Design (design_id={self.design_id})>"
```

### Comparing `jaeger-1.3.4/python/jaeger/target/tools.py` & `jaeger-1.4.0/python/jaeger/target/tools.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/python/jaeger/testing.py` & `jaeger-1.4.0/python/jaeger/testing.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/python/jaeger/utils/database.py` & `jaeger-1.4.0/python/jaeger/utils/database.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/python/jaeger/utils/helpers.py` & `jaeger-1.4.0/python/jaeger/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/python/jaeger/utils/utils.py` & `jaeger-1.4.0/python/jaeger/utils/utils.py`

 * *Files identical despite different names*

### Comparing `jaeger-1.3.4/PKG-INFO` & `jaeger-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaeger
-Version: 1.3.4
+Version: 1.4.0
 Summary: Controllers for the SDSS-V FPS
 Home-page: https://github.com/sdss/jaeger
 License: BSD-3-Clause
 Keywords: astronomy,software
 Author: José Sánchez-Gallego
 Author-email: gallegoj@uw.edu
 Requires-Python: >=3.8,<3.12
@@ -21,15 +21,15 @@
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: astropy (>=5.0.0,<6.0.0)
 Requires-Dist: click_default_group (>=1.2.2,<2.0.0)
 Requires-Dist: pandas (>=1.3.4,<2.0.0)
 Requires-Dist: pydl (==1.0.0rc1)
 Requires-Dist: sdss-clu (>=1.9.1,<2.0.0)
-Requires-Dist: sdss-coordio (>=1.6.0,<2.0.0)
+Requires-Dist: sdss-coordio (>=1.7.0,<2.0.0)
 Requires-Dist: sdss-drift (>=1.0.0,<2.0.0)
 Requires-Dist: sdss-kaiju (>=1.3.1,<2.0.0)
 Requires-Dist: sdssdb (>=0.6.0,<0.7.0)
 Requires-Dist: sdsstools (>=1.0.0,<2.0.0)
 Requires-Dist: tables (>=3.6.1,<4.0.0)
 Requires-Dist: zc.lockfile (>=2.0,<3.0)
 Project-URL: Documentation, https://sdss-jaeger.readthedocs.io/en/latest/
```

