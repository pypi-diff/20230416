# Comparing `tmp/appdaemon-4.4.1.tar.gz` & `tmp/appdaemon-4.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appdaemon-4.4.1.tar", last modified: Sun Apr  9 23:03:34 2023, max compression
+gzip compressed data, was "appdaemon-4.4.2.tar", last modified: Sun Apr 16 18:24:57 2023, max compression
```

## Comparing `appdaemon-4.4.1.tar` & `appdaemon-4.4.2.tar`

### file list

```diff
@@ -1,384 +1,384 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:34.808396 appdaemon-4.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    10480 2023-04-09 23:03:16.000000 appdaemon-4.4.1/LICENSE.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      175 2023-04-09 23:03:16.000000 appdaemon-4.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14369 2023-04-09 23:03:34.808396 appdaemon-4.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-09 23:03:16.000000 appdaemon-4.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-09 23:03:16.000000 appdaemon-4.4.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:34.740395 appdaemon-4.4.1/appdaemon/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13064 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   131485 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/adapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/adbase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/admin_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)    61514 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/app_management.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8634 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/appdaemon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:34.732395 appdaemon-4.4.1/appdaemon/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:34.740395 appdaemon-4.4.1/appdaemon/assets/aui/
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/aui/appdaemon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:34.740395 appdaemon-4.4.1/appdaemon/assets/aui/css/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/aui/css/app.css
--rw-r--r--   0 runner    (1001) docker     (123)   408122 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/aui/css/chunk-vendors.css
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/aui/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/aui/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:34.744395 appdaemon-4.4.1/appdaemon/assets/aui/js/
--rw-r--r--   0 runner    (1001) docker     (123)    41655 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/aui/js/app.js
--rw-r--r--   0 runner    (1001) docker     (123)   164271 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/aui/js/app.js.map
--rw-r--r--   0 runner    (1001) docker     (123)  1086461 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/aui/js/chunk-vendors.js
--rw-r--r--   0 runner    (1001) docker     (123)  3959700 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/aui/js/chunk-vendors.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:34.752395 appdaemon-4.4.1/appdaemon/assets/css/
--rw-r--r--   0 runner    (1001) docker     (123)    63156 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/css/all.css
--rwxr-xr-x   0 runner    (1001) docker     (123)      390 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/css/climacons-font.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:34.752395 appdaemon-4.4.1/appdaemon/assets/css/default/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2853 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/css/default/dashboard.css
--rwxr-xr-x   0 runner    (1001) docker     (123)    14951 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/css/default/variables.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    49025 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/css/fontawesome.min.css
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/css/fonts.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:34.752395 appdaemon-4.4.1/appdaemon/assets/css/glassic/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3761 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/css/glassic/dashboard.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:34.752395 appdaemon-4.4.1/appdaemon/assets/css/glassic/img/
--rwxr-xr-x   0 runner    (1001) docker     (123)   266843 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/css/glassic/img/carbon1.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)   240261 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/css/glassic/img/carbon2.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)   198334 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/css/glassic/img/carbon3.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)   209749 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/css/glassic/img/carbon4.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)   850628 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/css/glassic/img/glassic_bg.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)    16683 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/css/glassic/variables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:34.756395 appdaemon-4.4.1/appdaemon/assets/css/images/
--rw-r--r--   0 runner    (1001) docker     (123)     7006 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/css/images/ui-icons_444444_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     7074 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/css/images/ui-icons_555555_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/css/images/ui-icons_777620_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/css/images/ui-icons_777777_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/css/images/ui-icons_cc0000_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     6313 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/css/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)    37326 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/css/jquery-ui.css
--rwxr-xr-x   0 runner    (1001) docker     (123)     3644 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/css/jquery.gridster.css
--rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/css/main.css
--rw-r--r--   0 runner    (1001) docker     (123)   259834 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/css/materialdesignicons.min.css
--rwxr-xr-x   0 runner    (1001) docker     (123)     1827 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/css/non_dashboard.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:34.756395 appdaemon-4.4.1/appdaemon/assets/css/obsidian/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4332 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/css/obsidian/dashboard.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:34.760395 appdaemon-4.4.1/appdaemon/assets/css/obsidian/img/
--rwxr-xr-x   0 runner    (1001) docker     (123)   852722 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/css/obsidian/img/obsidian_bg.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)     9753 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/css/obsidian/img/obsidian_w_bg.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)   852722 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/css/obsidian/img/obsidianbg.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)     9753 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/css/obsidian/img/widgetbg.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)    15284 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/css/obsidian/variables.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/css/rickshaw.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:34.760395 appdaemon-4.4.1/appdaemon/assets/css/simplyred/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4263 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/css/simplyred/dashboard.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:34.760395 appdaemon-4.4.1/appdaemon/assets/css/simplyred/img/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1406 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/css/simplyred/img/goldgradient.png
--rwxr-xr-x   0 runner    (1001) docker     (123)   175552 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/css/simplyred/img/goldtexture.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:34.760395 appdaemon-4.4.1/appdaemon/assets/css/simplyred/js/
--rwxr-xr-x   0 runner    (1001) docker     (123)      884 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/css/simplyred/js/timer.js
--rwxr-xr-x   0 runner    (1001) docker     (123)    16040 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/css/simplyred/variables.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    26694 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/css/v4-shims.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:34.760395 appdaemon-4.4.1/appdaemon/assets/css/zen/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3287 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/css/zen/dashboard.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:34.760395 appdaemon-4.4.1/appdaemon/assets/css/zen/img/
--rwxr-xr-x   0 runner    (1001) docker     (123)    20639 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/css/zen/img/zen_bg.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)    78614 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/css/zen/img/zen_bg2.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)   178601 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/css/zen/img/zen_weatherbg.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)    16465 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/css/zen/variables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:34.768396 appdaemon-4.4.1/appdaemon/assets/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    31244 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/fonts/TickingTimebombBB.ttf
--rwxr-xr-x   0 runner    (1001) docker     (123)    18878 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/fonts/climacons-webfont.eot
--rwxr-xr-x   0 runner    (1001) docker     (123)   113691 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/fonts/climacons-webfont.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)    18692 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/fonts/climacons-webfont.ttf
--rwxr-xr-x   0 runner    (1001) docker     (123)    25484 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/fonts/climacons-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (123)    34638 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/fonts/digital-7-mono.eot
--rw-r--r--   0 runner    (1001) docker     (123)    34404 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/fonts/digital-7-mono.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   960632 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/fonts/materialdesignicons-webfont.eot
--rw-r--r--   0 runner    (1001) docker     (123)   960412 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/fonts/materialdesignicons-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   440564 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/fonts/materialdesignicons-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (123)   308440 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/fonts/materialdesignicons-webfont.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    38260 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/fonts/repetition.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:34.768396 appdaemon-4.4.1/appdaemon/assets/images/
--rwxr-xr-x   0 runner    (1001) docker     (123)       43 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/images/Blank.gif
--rwxr-xr-x   0 runner    (1001) docker     (123)      983 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/images/android-chrome-192x192.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     2087 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/images/android-chrome-512x512.png
--rwxr-xr-x   0 runner    (1001) docker     (123)      937 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/images/apple-touch-icon.png
--rwxr-xr-x   0 runner    (1001) docker     (123)      246 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/images/browserconfig.xml
--rwxr-xr-x   0 runner    (1001) docker     (123)      677 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/images/favicon-16x16.png
--rwxr-xr-x   0 runner    (1001) docker     (123)      722 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/images/favicon-32x32.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    15086 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/images/favicon.ico
--rwxr-xr-x   0 runner    (1001) docker     (123)      418 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/images/manifest.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      805 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/images/mstile-144x144.png
--rwxr-xr-x   0 runner    (1001) docker     (123)      893 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/images/mstile-150x150.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1052 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/images/mstile-310x150.png
--rwxr-xr-x   0 runner    (1001) docker     (123)     1541 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/images/mstile-310x310.png
--rwxr-xr-x   0 runner    (1001) docker     (123)      762 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/images/mstile-70x70.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:34.776396 appdaemon-4.4.1/appdaemon/assets/javascript/
--rw-r--r--   0 runner    (1001) docker     (123)    22009 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/javascript/admin.js
--rw-r--r--   0 runner    (1001) docker     (123)    17515 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/javascript/d3.layout.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    57229 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/javascript/d3.min.js
--rwxr-xr-x   0 runner    (1001) docker     (123)    12693 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/javascript/dashboard.js
--rw-r--r--   0 runner    (1001) docker     (123)    43741 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/javascript/gauge.min.js
--rwxr-xr-x   0 runner    (1001) docker     (123)    86709 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/javascript/jquery-3.1.1.min.js
--rw-r--r--   0 runner    (1001) docker     (123)   520709 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/javascript/jquery-ui.js
--rwxr-xr-x   0 runner    (1001) docker     (123)   148197 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/javascript/jquery.gridster.js
--rw-r--r--   0 runner    (1001) docker     (123)    38111 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/javascript/justgage.js
--rwxr-xr-x   0 runner    (1001) docker     (123)    60024 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/javascript/knockout-3.4.1.js
--rw-r--r--   0 runner    (1001) docker     (123)    18102 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/javascript/list.min.js
--rw-r--r--   0 runner    (1001) docker     (123)  2171966 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/javascript/plotly.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    92765 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/javascript/raphael-2.1.4.min.js
--rwxr-xr-x   0 runner    (1001) docker     (123)     3100 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/javascript/reconnecting-websocket.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    77893 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/javascript/rickshaw.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    62407 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/javascript/socket.io.js
--rw-r--r--   0 runner    (1001) docker     (123)    62848 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/javascript/sockjs.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     8739 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/javascript/stream.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:34.780396 appdaemon-4.4.1/appdaemon/assets/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    11473 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/templates/admin.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/templates/body_include.jinja2
--rwxr-xr-x   0 runner    (1001) docker     (123)     3564 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/templates/dashboard.jinja2
--rwxr-xr-x   0 runner    (1001) docker     (123)     3897 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/templates/dashinit.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/templates/error.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/templates/head_include.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/templates/list.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/templates/logon.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:34.784396 appdaemon-4.4.1/appdaemon/assets/webfonts/
--rw-r--r--   0 runner    (1001) docker     (123)   123540 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/webfonts/fa-brands-400.eot
--rw-r--r--   0 runner    (1001) docker     (123)   688936 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/webfonts/fa-brands-400.svg
--rw-r--r--   0 runner    (1001) docker     (123)   123304 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/webfonts/fa-brands-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    79752 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/webfonts/fa-brands-400.woff
--rw-r--r--   0 runner    (1001) docker     (123)    68240 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/webfonts/fa-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    40576 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/webfonts/fa-regular-400.eot
--rw-r--r--   0 runner    (1001) docker     (123)   142266 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/webfonts/fa-regular-400.svg
--rw-r--r--   0 runner    (1001) docker     (123)    40348 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/webfonts/fa-regular-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    18168 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/webfonts/fa-regular-400.woff
--rw-r--r--   0 runner    (1001) docker     (123)    14880 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/webfonts/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   191332 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/webfonts/fa-solid-900.eot
--rw-r--r--   0 runner    (1001) docker     (123)   725404 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/webfonts/fa-solid-900.svg
--rw-r--r--   0 runner    (1001) docker     (123)   191112 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/webfonts/fa-solid-900.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    92696 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/webfonts/fa-solid-900.woff
--rw-r--r--   0 runner    (1001) docker     (123)    72000 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/assets/webfonts/fa-solid-900.woff2
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/callbacks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    38576 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    25125 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    15417 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/events.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/futures.py
--rw-r--r--   0 runner    (1001) docker     (123)    40578 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/http.py
--rw-r--r--   0 runner    (1001) docker     (123)    25209 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    15303 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/plugin_management.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:34.784396 appdaemon-4.4.1/appdaemon/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:34.784396 appdaemon-4.4.1/appdaemon/plugins/dummy/
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/plugins/dummy/dummyapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/plugins/dummy/dummyplugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:34.784396 appdaemon-4.4.1/appdaemon/plugins/hass/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/plugins/hass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28151 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/plugins/hass/hassapi.py
--rw-r--r--   0 runner    (1001) docker     (123)    34594 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/plugins/hass/hassplugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:34.788396 appdaemon-4.4.1/appdaemon/plugins/mqtt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/plugins/mqtt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14862 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/plugins/mqtt/mqttapi.py
--rw-r--r--   0 runner    (1001) docker     (123)    25640 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/plugins/mqtt/mqttplugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/pyversions.py
--rw-r--r--   0 runner    (1001) docker     (123)    42222 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9492 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/sequences.py
--rw-r--r--   0 runner    (1001) docker     (123)     9889 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/services.py
--rw-r--r--   0 runner    (1001) docker     (123)    28748 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:34.788396 appdaemon-4.4.1/appdaemon/stream/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14399 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/stream/adstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/stream/socketio_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/stream/sockjs_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/stream/ws_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/thread_async.py
--rw-r--r--   0 runner    (1001) docker     (123)    48475 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/threading.py
--rw-r--r--   0 runner    (1001) docker     (123)     8888 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/utility_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)    22017 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:34.792396 appdaemon-4.4.1/appdaemon/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/AdminLog.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/AdminSummary.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/AdminTable.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1022 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/alarm.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:34.792396 appdaemon-4.4.1/appdaemon/widgets/basealarm/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1140 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/basealarm/basealarm.css
--rwxr-xr-x   0 runner    (1001) docker     (123)     2230 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/basealarm/basealarm.html
--rwxr-xr-x   0 runner    (1001) docker     (123)     6305 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/basealarm/basealarm.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:34.796396 appdaemon-4.4.1/appdaemon/widgets/basecamera/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/basecamera/basecamera.css
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/basecamera/basecamera.html
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/basecamera/basecamera.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:34.796396 appdaemon-4.4.1/appdaemon/widgets/baseclimate/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1239 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/baseclimate/baseclimate.css
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/baseclimate/baseclimate.html
--rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/baseclimate/baseclimate.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:34.796396 appdaemon-4.4.1/appdaemon/widgets/baseclock/
--rwxr-xr-x   0 runner    (1001) docker     (123)      162 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/baseclock/baseclock.css
--rwxr-xr-x   0 runner    (1001) docker     (123)      145 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/baseclock/baseclock.html
--rwxr-xr-x   0 runner    (1001) docker     (123)     2645 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/baseclock/baseclock.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:34.796396 appdaemon-4.4.1/appdaemon/widgets/basedatetime/
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/basedatetime/basedatetime.css
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/basedatetime/basedatetime.html
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/basedatetime/basedatetime.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:34.796396 appdaemon-4.4.1/appdaemon/widgets/basedisplay/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/basedisplay/basedisplay.css
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/basedisplay/basedisplay.html
--rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/basedisplay/basedisplay.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:34.796396 appdaemon-4.4.1/appdaemon/widgets/baseentitypicture/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/baseentitypicture/baseentitypicture.css
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/baseentitypicture/baseentitypicture.html
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/baseentitypicture/baseentitypicture.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:34.796396 appdaemon-4.4.1/appdaemon/widgets/baseerror/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/baseerror/baseerror.css
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/baseerror/baseerror.html
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/baseerror/baseerror.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:34.796396 appdaemon-4.4.1/appdaemon/widgets/basefan/
--rwxr-xr-x   0 runner    (1001) docker     (123)      573 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/basefan/basefan.css
--rwxr-xr-x   0 runner    (1001) docker     (123)      651 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/basefan/basefan.html
--rwxr-xr-x   0 runner    (1001) docker     (123)     5690 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/basefan/basefan.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:34.796396 appdaemon-4.4.1/appdaemon/widgets/basegauge/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/basegauge/basegauge.css
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/basegauge/basegauge.html
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/basegauge/basegauge.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:34.796396 appdaemon-4.4.1/appdaemon/widgets/baseheater/
--rwxr-xr-x   0 runner    (1001) docker     (123)      738 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/baseheater/baseheater.css
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/baseheater/baseheater.html
--rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/baseheater/baseheater.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:34.800396 appdaemon-4.4.1/appdaemon/widgets/baseicon/
--rwxr-xr-x   0 runner    (1001) docker     (123)      463 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/baseicon/baseicon.css
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/baseicon/baseicon.html
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/baseicon/baseicon.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:34.800396 appdaemon-4.4.1/appdaemon/widgets/baseiframe/
--rwxr-xr-x   0 runner    (1001) docker     (123)      636 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/baseiframe/baseiframe.css
--rwxr-xr-x   0 runner    (1001) docker     (123)      322 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/baseiframe/baseiframe.html
--rwxr-xr-x   0 runner    (1001) docker     (123)     2084 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/baseiframe/baseiframe.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:34.800396 appdaemon-4.4.1/appdaemon/widgets/baseinputnumber/
--rwxr-xr-x   0 runner    (1001) docker     (123)      986 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/baseinputnumber/baseinputnumber.css
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/baseinputnumber/baseinputnumber.html
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/baseinputnumber/baseinputnumber.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:34.800396 appdaemon-4.4.1/appdaemon/widgets/basejavascript/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/basejavascript/basejavascript.css
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/basejavascript/basejavascript.html
--rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/basejavascript/basejavascript.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:34.800396 appdaemon-4.4.1/appdaemon/widgets/baselight/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1181 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/baselight/baselight.css
--rwxr-xr-x   0 runner    (1001) docker     (123)      798 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/baselight/baselight.html
--rwxr-xr-x   0 runner    (1001) docker     (123)     5872 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/baselight/baselight.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:34.800396 appdaemon-4.4.1/appdaemon/widgets/basemedia/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1394 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/basemedia/basemedia.css
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/basemedia/basemedia.html
--rw-r--r--   0 runner    (1001) docker     (123)     8897 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/basemedia/basemedia.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:34.800396 appdaemon-4.4.1/appdaemon/widgets/baseradial/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/baseradial/baseradial.css
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/baseradial/baseradial.html
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/baseradial/baseradial.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:34.800396 appdaemon-4.4.1/appdaemon/widgets/baserss/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/baserss/baserss.css
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/baserss/baserss.html
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/baserss/baserss.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:34.800396 appdaemon-4.4.1/appdaemon/widgets/baseselect/
--rwxr-xr-x   0 runner    (1001) docker     (123)      651 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/baseselect/baseselect.css
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/baseselect/baseselect.html
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/baseselect/baseselect.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:34.800396 appdaemon-4.4.1/appdaemon/widgets/baseslider/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1222 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/baseslider/baseslider.css
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/baseslider/baseslider.html
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/baseslider/baseslider.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:34.804396 appdaemon-4.4.1/appdaemon/widgets/baseswitch/
--rwxr-xr-x   0 runner    (1001) docker     (123)      473 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/baseswitch/baseswitch.css
--rwxr-xr-x   0 runner    (1001) docker     (123)      389 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/baseswitch/baseswitch.html
--rwxr-xr-x   0 runner    (1001) docker     (123)     4231 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/baseswitch/baseswitch.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:34.804396 appdaemon-4.4.1/appdaemon/widgets/basetemperature/
--rwxr-xr-x   0 runner    (1001) docker     (123)      121 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/basetemperature/basetemperature.css
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/basetemperature/basetemperature.html
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/basetemperature/basetemperature.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:34.804396 appdaemon-4.4.1/appdaemon/widgets/basetext/
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/basetext/basetext.css
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/basetext/basetext.html
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/basetext/basetext.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:34.804396 appdaemon-4.4.1/appdaemon/widgets/baseweather/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1959 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/baseweather/baseweather.css
--rwxr-xr-x   0 runner    (1001) docker     (123)     4306 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/baseweather/baseweather.html
--rwxr-xr-x   0 runner    (1001) docker     (123)     4029 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/baseweather/baseweather.js
--rwxr-xr-x   0 runner    (1001) docker     (123)      588 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/binary_sensor.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      235 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/camera.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      662 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/climate.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      200 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/clock.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      700 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/cover.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      895 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/device_tracker.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/entitypicture.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1384 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/fan.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/gauge.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      881 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/group.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/heater.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/icon.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      235 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/iframe.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      769 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/input_boolean.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/input_datetime.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/input_number.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/input_select.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/input_slider.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/input_text.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/javascript.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      414 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/label.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      881 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/light.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      683 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/lock.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      524 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/london_underground.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1711 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/media_player.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      587 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/mode.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      444 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/navigate.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/person.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/radial.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      461 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/reload.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/rss.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      751 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/scene.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      745 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/script.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      647 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/sensor.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/sequence.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      713 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/switch.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/temperature.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)      680 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/text_sensor.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1710 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/weather.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1037 2023-04-09 23:03:16.000000 appdaemon-4.4.1/appdaemon/widgets/weather_summary.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:34.740395 appdaemon-4.4.1/appdaemon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14369 2023-04-09 23:03:34.000000 appdaemon-4.4.1/appdaemon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12334 2023-04-09 23:03:34.000000 appdaemon-4.4.1/appdaemon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 23:03:34.000000 appdaemon-4.4.1/appdaemon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-09 23:03:34.000000 appdaemon-4.4.1/appdaemon.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-09 23:03:34.000000 appdaemon-4.4.1/appdaemon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-09 23:03:34.000000 appdaemon-4.4.1/appdaemon.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:34.736395 appdaemon-4.4.1/conf/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:34.804396 appdaemon-4.4.1/conf/apps/
--rwxr-xr-x   0 runner    (1001) docker     (123)      205 2023-04-09 23:03:16.000000 appdaemon-4.4.1/conf/apps/hello.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:34.808396 appdaemon-4.4.1/conf/example_apps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:34.808396 appdaemon-4.4.1/conf/example_apps/ObjectTracker/
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-04-09 23:03:16.000000 appdaemon-4.4.1/conf/example_apps/ObjectTracker/general_app_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-04-09 23:03:16.000000 appdaemon-4.4.1/conf/example_apps/ObjectTracker/objectcontrole.py
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-04-09 23:03:16.000000 appdaemon-4.4.1/conf/example_apps/alexa.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1880 2023-04-09 23:03:16.000000 appdaemon-4.4.1/conf/example_apps/battery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-09 23:03:16.000000 appdaemon-4.4.1/conf/example_apps/bysykkel.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-09 23:03:16.000000 appdaemon-4.4.1/conf/example_apps/commute.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1976 2023-04-09 23:03:16.000000 appdaemon-4.4.1/conf/example_apps/dark_day.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      859 2023-04-09 23:03:16.000000 appdaemon-4.4.1/conf/example_apps/door_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-04-09 23:03:16.000000 appdaemon-4.4.1/conf/example_apps/eventCache.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-09 23:03:16.000000 appdaemon-4.4.1/conf/example_apps/eventMonitor.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-09 23:03:16.000000 appdaemon-4.4.1/conf/example_apps/globals.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1486 2023-04-09 23:03:16.000000 appdaemon-4.4.1/conf/example_apps/grandfather.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1010 2023-04-09 23:03:16.000000 appdaemon-4.4.1/conf/example_apps/hwcheck.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-09 23:03:16.000000 appdaemon-4.4.1/conf/example_apps/ical.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1688 2023-04-09 23:03:16.000000 appdaemon-4.4.1/conf/example_apps/minimote.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7049 2023-04-09 23:03:16.000000 appdaemon-4.4.1/conf/example_apps/modes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      978 2023-04-09 23:03:16.000000 appdaemon-4.4.1/conf/example_apps/momentary_switch.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1806 2023-04-09 23:03:16.000000 appdaemon-4.4.1/conf/example_apps/motion_lights.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      890 2023-04-09 23:03:16.000000 appdaemon-4.4.1/conf/example_apps/motion_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)    10434 2023-04-09 23:03:16.000000 appdaemon-4.4.1/conf/example_apps/occusim.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      905 2023-04-09 23:03:16.000000 appdaemon-4.4.1/conf/example_apps/outside_lights.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3789 2023-04-09 23:03:16.000000 appdaemon-4.4.1/conf/example_apps/presence.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-09 23:03:16.000000 appdaemon-4.4.1/conf/example_apps/ruter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11251 2023-04-09 23:03:16.000000 appdaemon-4.4.1/conf/example_apps/secure.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1405 2023-04-09 23:03:16.000000 appdaemon-4.4.1/conf/example_apps/sensor_notification.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1303 2023-04-09 23:03:16.000000 appdaemon-4.4.1/conf/example_apps/sensor_notify.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-09 23:03:16.000000 appdaemon-4.4.1/conf/example_apps/sequence.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4263 2023-04-09 23:03:16.000000 appdaemon-4.4.1/conf/example_apps/smart_heat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4438 2023-04-09 23:03:16.000000 appdaemon-4.4.1/conf/example_apps/sound.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2583 2023-04-09 23:03:16.000000 appdaemon-4.4.1/conf/example_apps/switch_reset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-04-09 23:03:16.000000 appdaemon-4.4.1/conf/example_apps/yr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-04-09 23:03:16.000000 appdaemon-4.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 23:03:34.808396 appdaemon-4.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 23:03:34.808396 appdaemon-4.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-09 23:03:16.000000 appdaemon-4.4.1/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:57.665031 appdaemon-4.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    10480 2023-04-16 18:24:39.000000 appdaemon-4.4.2/LICENSE.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      175 2023-04-16 18:24:39.000000 appdaemon-4.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14369 2023-04-16 18:24:57.665031 appdaemon-4.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-16 18:24:39.000000 appdaemon-4.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-16 18:24:39.000000 appdaemon-4.4.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:57.565031 appdaemon-4.4.2/appdaemon/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13064 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   131485 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/adapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/adbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/admin_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61641 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/app_management.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8634 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/appdaemon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:57.549031 appdaemon-4.4.2/appdaemon/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:57.565031 appdaemon-4.4.2/appdaemon/assets/aui/
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/aui/appdaemon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:57.565031 appdaemon-4.4.2/appdaemon/assets/aui/css/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/aui/css/app.css
+-rw-r--r--   0 runner    (1001) docker     (123)   408122 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/aui/css/chunk-vendors.css
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/aui/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/aui/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:57.573031 appdaemon-4.4.2/appdaemon/assets/aui/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    41655 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/aui/js/app.js
+-rw-r--r--   0 runner    (1001) docker     (123)   164271 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/aui/js/app.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)  1086461 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/aui/js/chunk-vendors.js
+-rw-r--r--   0 runner    (1001) docker     (123)  3959700 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/aui/js/chunk-vendors.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:57.581031 appdaemon-4.4.2/appdaemon/assets/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    63156 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/css/all.css
+-rwxr-xr-x   0 runner    (1001) docker     (123)      390 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/css/climacons-font.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:57.581031 appdaemon-4.4.2/appdaemon/assets/css/default/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2853 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/css/default/dashboard.css
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14951 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/css/default/variables.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    49025 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/css/fontawesome.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/css/fonts.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:57.581031 appdaemon-4.4.2/appdaemon/assets/css/glassic/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3761 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/css/glassic/dashboard.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:57.581031 appdaemon-4.4.2/appdaemon/assets/css/glassic/img/
+-rwxr-xr-x   0 runner    (1001) docker     (123)   266843 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/css/glassic/img/carbon1.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)   240261 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/css/glassic/img/carbon2.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)   198334 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/css/glassic/img/carbon3.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)   209749 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/css/glassic/img/carbon4.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)   850628 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/css/glassic/img/glassic_bg.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16683 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/css/glassic/variables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:57.585031 appdaemon-4.4.2/appdaemon/assets/css/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     7006 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/css/images/ui-icons_444444_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7074 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/css/images/ui-icons_555555_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/css/images/ui-icons_777620_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/css/images/ui-icons_777777_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4632 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/css/images/ui-icons_cc0000_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6313 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/css/images/ui-icons_ffffff_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)    37326 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/css/jquery-ui.css
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3644 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/css/jquery.gridster.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/css/main.css
+-rw-r--r--   0 runner    (1001) docker     (123)   259834 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/css/materialdesignicons.min.css
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1827 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/css/non_dashboard.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:57.585031 appdaemon-4.4.2/appdaemon/assets/css/obsidian/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4332 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/css/obsidian/dashboard.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:57.585031 appdaemon-4.4.2/appdaemon/assets/css/obsidian/img/
+-rwxr-xr-x   0 runner    (1001) docker     (123)   852722 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/css/obsidian/img/obsidian_bg.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9753 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/css/obsidian/img/obsidian_w_bg.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)   852722 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/css/obsidian/img/obsidianbg.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9753 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/css/obsidian/img/widgetbg.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15284 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/css/obsidian/variables.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/css/rickshaw.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:57.585031 appdaemon-4.4.2/appdaemon/assets/css/simplyred/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4263 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/css/simplyred/dashboard.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:57.585031 appdaemon-4.4.2/appdaemon/assets/css/simplyred/img/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1406 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/css/simplyred/img/goldgradient.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)   175552 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/css/simplyred/img/goldtexture.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:57.585031 appdaemon-4.4.2/appdaemon/assets/css/simplyred/js/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      884 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/css/simplyred/js/timer.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16040 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/css/simplyred/variables.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    26694 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/css/v4-shims.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:57.585031 appdaemon-4.4.2/appdaemon/assets/css/zen/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3287 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/css/zen/dashboard.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:57.585031 appdaemon-4.4.2/appdaemon/assets/css/zen/img/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20639 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/css/zen/img/zen_bg.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    78614 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/css/zen/img/zen_bg2.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)   178601 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/css/zen/img/zen_weatherbg.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16465 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/css/zen/variables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:57.593031 appdaemon-4.4.2/appdaemon/assets/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    31244 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/fonts/TickingTimebombBB.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18878 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/fonts/climacons-webfont.eot
+-rwxr-xr-x   0 runner    (1001) docker     (123)   113691 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/fonts/climacons-webfont.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18692 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/fonts/climacons-webfont.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25484 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/fonts/climacons-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    34638 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/fonts/digital-7-mono.eot
+-rw-r--r--   0 runner    (1001) docker     (123)    34404 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/fonts/digital-7-mono.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   960632 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/fonts/materialdesignicons-webfont.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   960412 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/fonts/materialdesignicons-webfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   440564 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/fonts/materialdesignicons-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   308440 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/fonts/materialdesignicons-webfont.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    38260 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/fonts/repetition.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:57.597031 appdaemon-4.4.2/appdaemon/assets/images/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       43 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/images/Blank.gif
+-rwxr-xr-x   0 runner    (1001) docker     (123)      983 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/images/android-chrome-192x192.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2087 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/images/android-chrome-512x512.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)      937 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/images/apple-touch-icon.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)      246 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/images/browserconfig.xml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      677 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/images/favicon-16x16.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)      722 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/images/favicon-32x32.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15086 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/images/favicon.ico
+-rwxr-xr-x   0 runner    (1001) docker     (123)      418 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/images/manifest.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      805 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/images/mstile-144x144.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)      893 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/images/mstile-150x150.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1052 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/images/mstile-310x150.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1541 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/images/mstile-310x310.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)      762 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/images/mstile-70x70.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:57.605031 appdaemon-4.4.2/appdaemon/assets/javascript/
+-rw-r--r--   0 runner    (1001) docker     (123)    22009 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/javascript/admin.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17515 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/javascript/d3.layout.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    57229 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/javascript/d3.min.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12693 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/javascript/dashboard.js
+-rw-r--r--   0 runner    (1001) docker     (123)    43741 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/javascript/gauge.min.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)    86709 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/javascript/jquery-3.1.1.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   520709 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/javascript/jquery-ui.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)   148197 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/javascript/jquery.gridster.js
+-rw-r--r--   0 runner    (1001) docker     (123)    38111 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/javascript/justgage.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)    60024 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/javascript/knockout-3.4.1.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18102 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/javascript/list.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)  2171966 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/javascript/plotly.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    92765 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/javascript/raphael-2.1.4.min.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3100 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/javascript/reconnecting-websocket.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    77893 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/javascript/rickshaw.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    62407 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/javascript/socket.io.js
+-rw-r--r--   0 runner    (1001) docker     (123)    62848 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/javascript/sockjs.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8739 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/javascript/stream.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:57.609031 appdaemon-4.4.2/appdaemon/assets/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    11473 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/templates/admin.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/templates/body_include.jinja2
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3564 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/templates/dashboard.jinja2
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3897 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/templates/dashinit.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/templates/error.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/templates/head_include.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/templates/list.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/templates/logon.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:57.617031 appdaemon-4.4.2/appdaemon/assets/webfonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   123540 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/webfonts/fa-brands-400.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   688936 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/webfonts/fa-brands-400.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   123304 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/webfonts/fa-brands-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    79752 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/webfonts/fa-brands-400.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    68240 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/webfonts/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    40576 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/webfonts/fa-regular-400.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   142266 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/webfonts/fa-regular-400.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    40348 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/webfonts/fa-regular-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    18168 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/webfonts/fa-regular-400.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    14880 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/webfonts/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   191332 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/webfonts/fa-solid-900.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   725404 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/webfonts/fa-solid-900.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   191112 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/webfonts/fa-solid-900.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    92696 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/webfonts/fa-solid-900.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    72000 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/assets/webfonts/fa-solid-900.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/callbacks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    38576 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25125 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15417 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40578 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25209 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16789 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/plugin_management.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:57.617031 appdaemon-4.4.2/appdaemon/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:57.617031 appdaemon-4.4.2/appdaemon/plugins/dummy/
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/plugins/dummy/dummyapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/plugins/dummy/dummyplugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:57.617031 appdaemon-4.4.2/appdaemon/plugins/hass/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/plugins/hass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28151 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/plugins/hass/hassapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33642 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/plugins/hass/hassplugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:57.617031 appdaemon-4.4.2/appdaemon/plugins/mqtt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/plugins/mqtt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14862 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/plugins/mqtt/mqttapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24674 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/plugins/mqtt/mqttplugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/pyversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42222 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9492 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/sequences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9889 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28748 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:57.621031 appdaemon-4.4.2/appdaemon/stream/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14399 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/stream/adstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/stream/socketio_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/stream/sockjs_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/stream/ws_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/thread_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48881 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/threading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8888 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/utility_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22017 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:57.633031 appdaemon-4.4.2/appdaemon/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/AdminLog.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/AdminSummary.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/AdminTable.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1022 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/alarm.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:57.633031 appdaemon-4.4.2/appdaemon/widgets/basealarm/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1140 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/basealarm/basealarm.css
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2230 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/basealarm/basealarm.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6305 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/basealarm/basealarm.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:57.633031 appdaemon-4.4.2/appdaemon/widgets/basecamera/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/basecamera/basecamera.css
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/basecamera/basecamera.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/basecamera/basecamera.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:57.637031 appdaemon-4.4.2/appdaemon/widgets/baseclimate/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1239 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/baseclimate/baseclimate.css
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/baseclimate/baseclimate.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/baseclimate/baseclimate.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:57.637031 appdaemon-4.4.2/appdaemon/widgets/baseclock/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      162 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/baseclock/baseclock.css
+-rwxr-xr-x   0 runner    (1001) docker     (123)      145 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/baseclock/baseclock.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2645 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/baseclock/baseclock.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:57.637031 appdaemon-4.4.2/appdaemon/widgets/basedatetime/
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/basedatetime/basedatetime.css
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/basedatetime/basedatetime.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/basedatetime/basedatetime.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:57.637031 appdaemon-4.4.2/appdaemon/widgets/basedisplay/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/basedisplay/basedisplay.css
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/basedisplay/basedisplay.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/basedisplay/basedisplay.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:57.637031 appdaemon-4.4.2/appdaemon/widgets/baseentitypicture/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/baseentitypicture/baseentitypicture.css
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/baseentitypicture/baseentitypicture.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/baseentitypicture/baseentitypicture.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:57.641031 appdaemon-4.4.2/appdaemon/widgets/baseerror/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/baseerror/baseerror.css
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/baseerror/baseerror.html
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/baseerror/baseerror.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:57.641031 appdaemon-4.4.2/appdaemon/widgets/basefan/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      573 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/basefan/basefan.css
+-rwxr-xr-x   0 runner    (1001) docker     (123)      651 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/basefan/basefan.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5690 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/basefan/basefan.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:57.641031 appdaemon-4.4.2/appdaemon/widgets/basegauge/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/basegauge/basegauge.css
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/basegauge/basegauge.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/basegauge/basegauge.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:57.641031 appdaemon-4.4.2/appdaemon/widgets/baseheater/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      738 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/baseheater/baseheater.css
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/baseheater/baseheater.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/baseheater/baseheater.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:57.645031 appdaemon-4.4.2/appdaemon/widgets/baseicon/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      463 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/baseicon/baseicon.css
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/baseicon/baseicon.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/baseicon/baseicon.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:57.645031 appdaemon-4.4.2/appdaemon/widgets/baseiframe/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      636 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/baseiframe/baseiframe.css
+-rwxr-xr-x   0 runner    (1001) docker     (123)      322 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/baseiframe/baseiframe.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2084 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/baseiframe/baseiframe.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:57.645031 appdaemon-4.4.2/appdaemon/widgets/baseinputnumber/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      986 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/baseinputnumber/baseinputnumber.css
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/baseinputnumber/baseinputnumber.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/baseinputnumber/baseinputnumber.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:57.645031 appdaemon-4.4.2/appdaemon/widgets/basejavascript/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/basejavascript/basejavascript.css
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/basejavascript/basejavascript.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/basejavascript/basejavascript.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:57.649031 appdaemon-4.4.2/appdaemon/widgets/baselight/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1181 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/baselight/baselight.css
+-rwxr-xr-x   0 runner    (1001) docker     (123)      798 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/baselight/baselight.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5872 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/baselight/baselight.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:57.649031 appdaemon-4.4.2/appdaemon/widgets/basemedia/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1394 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/basemedia/basemedia.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/basemedia/basemedia.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8897 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/basemedia/basemedia.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:57.649031 appdaemon-4.4.2/appdaemon/widgets/baseradial/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/baseradial/baseradial.css
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/baseradial/baseradial.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/baseradial/baseradial.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:57.649031 appdaemon-4.4.2/appdaemon/widgets/baserss/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/baserss/baserss.css
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/baserss/baserss.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/baserss/baserss.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:57.649031 appdaemon-4.4.2/appdaemon/widgets/baseselect/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      651 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/baseselect/baseselect.css
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/baseselect/baseselect.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/baseselect/baseselect.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:57.653031 appdaemon-4.4.2/appdaemon/widgets/baseslider/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1222 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/baseslider/baseslider.css
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/baseslider/baseslider.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/baseslider/baseslider.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:57.653031 appdaemon-4.4.2/appdaemon/widgets/baseswitch/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      473 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/baseswitch/baseswitch.css
+-rwxr-xr-x   0 runner    (1001) docker     (123)      389 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/baseswitch/baseswitch.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4231 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/baseswitch/baseswitch.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:57.653031 appdaemon-4.4.2/appdaemon/widgets/basetemperature/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      121 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/basetemperature/basetemperature.css
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/basetemperature/basetemperature.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/basetemperature/basetemperature.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:57.653031 appdaemon-4.4.2/appdaemon/widgets/basetext/
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/basetext/basetext.css
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/basetext/basetext.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/basetext/basetext.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:57.657031 appdaemon-4.4.2/appdaemon/widgets/baseweather/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1959 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/baseweather/baseweather.css
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4306 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/baseweather/baseweather.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4029 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/baseweather/baseweather.js
+-rwxr-xr-x   0 runner    (1001) docker     (123)      588 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/binary_sensor.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      235 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/camera.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      662 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/climate.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      200 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/clock.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      700 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/cover.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      895 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/device_tracker.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/entitypicture.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1384 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/fan.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/gauge.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      881 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/group.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/heater.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/icon.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      235 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/iframe.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      769 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/input_boolean.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/input_datetime.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/input_number.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/input_select.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/input_slider.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/input_text.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/javascript.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      414 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/label.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      881 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/light.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      683 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/lock.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      524 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/london_underground.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1711 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/media_player.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      587 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/mode.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      444 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/navigate.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/person.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/radial.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      461 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/reload.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/rss.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      751 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/scene.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      745 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/script.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      647 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/sensor.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/sequence.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      713 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/switch.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/temperature.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      680 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/text_sensor.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1710 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/weather.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1037 2023-04-16 18:24:39.000000 appdaemon-4.4.2/appdaemon/widgets/weather_summary.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:57.565031 appdaemon-4.4.2/appdaemon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14369 2023-04-16 18:24:57.000000 appdaemon-4.4.2/appdaemon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12334 2023-04-16 18:24:57.000000 appdaemon-4.4.2/appdaemon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 18:24:57.000000 appdaemon-4.4.2/appdaemon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-16 18:24:57.000000 appdaemon-4.4.2/appdaemon.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-16 18:24:57.000000 appdaemon-4.4.2/appdaemon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-16 18:24:57.000000 appdaemon-4.4.2/appdaemon.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:57.561031 appdaemon-4.4.2/conf/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:57.657031 appdaemon-4.4.2/conf/apps/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      205 2023-04-16 18:24:39.000000 appdaemon-4.4.2/conf/apps/hello.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:57.665031 appdaemon-4.4.2/conf/example_apps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:57.665031 appdaemon-4.4.2/conf/example_apps/ObjectTracker/
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-04-16 18:24:39.000000 appdaemon-4.4.2/conf/example_apps/ObjectTracker/general_app_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-04-16 18:24:39.000000 appdaemon-4.4.2/conf/example_apps/ObjectTracker/objectcontrole.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-04-16 18:24:39.000000 appdaemon-4.4.2/conf/example_apps/alexa.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1880 2023-04-16 18:24:39.000000 appdaemon-4.4.2/conf/example_apps/battery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-16 18:24:39.000000 appdaemon-4.4.2/conf/example_apps/bysykkel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-16 18:24:39.000000 appdaemon-4.4.2/conf/example_apps/commute.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1976 2023-04-16 18:24:39.000000 appdaemon-4.4.2/conf/example_apps/dark_day.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      859 2023-04-16 18:24:39.000000 appdaemon-4.4.2/conf/example_apps/door_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-04-16 18:24:39.000000 appdaemon-4.4.2/conf/example_apps/eventCache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-16 18:24:39.000000 appdaemon-4.4.2/conf/example_apps/eventMonitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-04-16 18:24:39.000000 appdaemon-4.4.2/conf/example_apps/globals.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1486 2023-04-16 18:24:39.000000 appdaemon-4.4.2/conf/example_apps/grandfather.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1010 2023-04-16 18:24:39.000000 appdaemon-4.4.2/conf/example_apps/hwcheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-16 18:24:39.000000 appdaemon-4.4.2/conf/example_apps/ical.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1688 2023-04-16 18:24:39.000000 appdaemon-4.4.2/conf/example_apps/minimote.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7049 2023-04-16 18:24:39.000000 appdaemon-4.4.2/conf/example_apps/modes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      978 2023-04-16 18:24:39.000000 appdaemon-4.4.2/conf/example_apps/momentary_switch.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1806 2023-04-16 18:24:39.000000 appdaemon-4.4.2/conf/example_apps/motion_lights.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      890 2023-04-16 18:24:39.000000 appdaemon-4.4.2/conf/example_apps/motion_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10434 2023-04-16 18:24:39.000000 appdaemon-4.4.2/conf/example_apps/occusim.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      905 2023-04-16 18:24:39.000000 appdaemon-4.4.2/conf/example_apps/outside_lights.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3789 2023-04-16 18:24:39.000000 appdaemon-4.4.2/conf/example_apps/presence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-16 18:24:39.000000 appdaemon-4.4.2/conf/example_apps/ruter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11251 2023-04-16 18:24:39.000000 appdaemon-4.4.2/conf/example_apps/secure.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1405 2023-04-16 18:24:39.000000 appdaemon-4.4.2/conf/example_apps/sensor_notification.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1303 2023-04-16 18:24:39.000000 appdaemon-4.4.2/conf/example_apps/sensor_notify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-16 18:24:39.000000 appdaemon-4.4.2/conf/example_apps/sequence.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4263 2023-04-16 18:24:39.000000 appdaemon-4.4.2/conf/example_apps/smart_heat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4438 2023-04-16 18:24:39.000000 appdaemon-4.4.2/conf/example_apps/sound.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2583 2023-04-16 18:24:39.000000 appdaemon-4.4.2/conf/example_apps/switch_reset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-04-16 18:24:39.000000 appdaemon-4.4.2/conf/example_apps/yr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-04-16 18:24:39.000000 appdaemon-4.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 18:24:57.665031 appdaemon-4.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:24:57.665031 appdaemon-4.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-16 18:24:39.000000 appdaemon-4.4.2/tests/test_main.py
```

### Comparing `appdaemon-4.4.1/LICENSE.md` & `appdaemon-4.4.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/PKG-INFO` & `appdaemon-4.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appdaemon
-Version: 4.4.1
+Version: 4.4.2
 Summary: Apps for the Home Assistant home automation package.
 Author-email: Andrew I Cockburn <appdaemon@acockburn.com>
 License: Apache License
         ==============
         
         _Version 2.0, January 2004_
         _&lt;<http://www.apache.org/licenses/>&gt;_
```

### Comparing `appdaemon-4.4.1/README.md` & `appdaemon-4.4.2/README.md`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/README.rst` & `appdaemon-4.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/__main__.py` & `appdaemon-4.4.2/appdaemon/__main__.py`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/adapi.py` & `appdaemon-4.4.2/appdaemon/adapi.py`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/adbase.py` & `appdaemon-4.4.2/appdaemon/adbase.py`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/admin.py` & `appdaemon-4.4.2/appdaemon/admin.py`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/admin_loop.py` & `appdaemon-4.4.2/appdaemon/admin_loop.py`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/app_management.py` & `appdaemon-4.4.2/appdaemon/app_management.py`

 * *Files 1% similar despite different names*

```diff
@@ -358,22 +358,23 @@
             self.logger.warning(
                 "Unable to find module module %s - '%s' is not loaded",
                 app_args["module"],
                 name,
             )
             await self.increase_inactive_apps(name)
 
-    def init_plugin_object(self, name, object):
+    def init_plugin_object(self, name: str, object: object, use_dictionary_unpacking: bool = False) -> None:
         self.objects[name] = {
             "type": "plugin",
             "object": object,
             "id": uuid.uuid4().hex,
             "pin_app": False,
             "pin_thread": -1,
             "running": False,
+            "use_dictionary_unpacking": use_dictionary_unpacking,
         }
 
     def init_sequence_object(self, name, object):
         """Initialize the sequence"""
 
         self.objects[name] = {
             "type": "sequence",
```

### Comparing `appdaemon-4.4.1/appdaemon/appdaemon.py` & `appdaemon-4.4.2/appdaemon/appdaemon.py`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/aui/appdaemon.png` & `appdaemon-4.4.2/appdaemon/assets/aui/appdaemon.png`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/aui/css/chunk-vendors.css` & `appdaemon-4.4.2/appdaemon/assets/aui/css/chunk-vendors.css`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/aui/favicon.ico` & `appdaemon-4.4.2/appdaemon/assets/aui/favicon.ico`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/aui/index.html` & `appdaemon-4.4.2/appdaemon/assets/aui/index.html`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/aui/js/app.js` & `appdaemon-4.4.2/appdaemon/assets/aui/js/app.js`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/aui/js/app.js.map` & `appdaemon-4.4.2/appdaemon/assets/aui/js/app.js.map`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/aui/js/chunk-vendors.js` & `appdaemon-4.4.2/appdaemon/assets/aui/js/chunk-vendors.js`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/aui/js/chunk-vendors.js.map` & `appdaemon-4.4.2/appdaemon/assets/aui/js/chunk-vendors.js.map`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/css/all.css` & `appdaemon-4.4.2/appdaemon/assets/css/all.css`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/css/default/dashboard.css` & `appdaemon-4.4.2/appdaemon/assets/css/default/dashboard.css`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/css/default/variables.yaml` & `appdaemon-4.4.2/appdaemon/assets/css/default/variables.yaml`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/css/fontawesome.min.css` & `appdaemon-4.4.2/appdaemon/assets/css/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/css/glassic/dashboard.css` & `appdaemon-4.4.2/appdaemon/assets/css/glassic/dashboard.css`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/css/glassic/img/carbon1.jpg` & `appdaemon-4.4.2/appdaemon/assets/css/glassic/img/carbon1.jpg`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/css/glassic/img/carbon2.jpg` & `appdaemon-4.4.2/appdaemon/assets/css/glassic/img/carbon2.jpg`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/css/glassic/img/carbon3.jpg` & `appdaemon-4.4.2/appdaemon/assets/css/glassic/img/carbon3.jpg`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/css/glassic/img/carbon4.jpg` & `appdaemon-4.4.2/appdaemon/assets/css/glassic/img/carbon4.jpg`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/css/glassic/img/glassic_bg.jpg` & `appdaemon-4.4.2/appdaemon/assets/css/glassic/img/glassic_bg.jpg`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/css/glassic/variables.yaml` & `appdaemon-4.4.2/appdaemon/assets/css/glassic/variables.yaml`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/css/images/ui-icons_444444_256x240.png` & `appdaemon-4.4.2/appdaemon/assets/css/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/css/images/ui-icons_555555_256x240.png` & `appdaemon-4.4.2/appdaemon/assets/css/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/css/images/ui-icons_777620_256x240.png` & `appdaemon-4.4.2/appdaemon/assets/css/images/ui-icons_777620_256x240.png`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/css/images/ui-icons_777777_256x240.png` & `appdaemon-4.4.2/appdaemon/assets/css/images/ui-icons_777777_256x240.png`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/css/images/ui-icons_cc0000_256x240.png` & `appdaemon-4.4.2/appdaemon/assets/css/images/ui-icons_cc0000_256x240.png`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/css/images/ui-icons_ffffff_256x240.png` & `appdaemon-4.4.2/appdaemon/assets/css/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/css/jquery-ui.css` & `appdaemon-4.4.2/appdaemon/assets/css/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/css/jquery.gridster.css` & `appdaemon-4.4.2/appdaemon/assets/css/jquery.gridster.css`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/css/main.css` & `appdaemon-4.4.2/appdaemon/assets/css/main.css`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/css/materialdesignicons.min.css` & `appdaemon-4.4.2/appdaemon/assets/css/materialdesignicons.min.css`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/css/non_dashboard.css` & `appdaemon-4.4.2/appdaemon/assets/css/non_dashboard.css`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/css/obsidian/dashboard.css` & `appdaemon-4.4.2/appdaemon/assets/css/obsidian/dashboard.css`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/css/obsidian/img/obsidian_bg.jpg` & `appdaemon-4.4.2/appdaemon/assets/css/obsidian/img/obsidian_bg.jpg`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/css/obsidian/img/obsidian_w_bg.jpg` & `appdaemon-4.4.2/appdaemon/assets/css/obsidian/img/obsidian_w_bg.jpg`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/css/obsidian/img/obsidianbg.jpg` & `appdaemon-4.4.2/appdaemon/assets/css/obsidian/img/obsidianbg.jpg`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/css/obsidian/img/widgetbg.jpg` & `appdaemon-4.4.2/appdaemon/assets/css/obsidian/img/widgetbg.jpg`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/css/obsidian/variables.yaml` & `appdaemon-4.4.2/appdaemon/assets/css/obsidian/variables.yaml`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/css/rickshaw.min.css` & `appdaemon-4.4.2/appdaemon/assets/css/rickshaw.min.css`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/css/simplyred/dashboard.css` & `appdaemon-4.4.2/appdaemon/assets/css/simplyred/dashboard.css`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/css/simplyred/img/goldgradient.png` & `appdaemon-4.4.2/appdaemon/assets/css/simplyred/img/goldgradient.png`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/css/simplyred/img/goldtexture.jpg` & `appdaemon-4.4.2/appdaemon/assets/css/simplyred/img/goldtexture.jpg`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/css/simplyred/js/timer.js` & `appdaemon-4.4.2/appdaemon/assets/css/simplyred/js/timer.js`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/css/simplyred/variables.yaml` & `appdaemon-4.4.2/appdaemon/assets/css/simplyred/variables.yaml`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/css/v4-shims.min.css` & `appdaemon-4.4.2/appdaemon/assets/css/v4-shims.min.css`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/css/zen/dashboard.css` & `appdaemon-4.4.2/appdaemon/assets/css/zen/dashboard.css`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/css/zen/img/zen_bg.jpg` & `appdaemon-4.4.2/appdaemon/assets/css/zen/img/zen_bg.jpg`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/css/zen/img/zen_bg2.jpg` & `appdaemon-4.4.2/appdaemon/assets/css/zen/img/zen_bg2.jpg`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/css/zen/img/zen_weatherbg.jpg` & `appdaemon-4.4.2/appdaemon/assets/css/zen/img/zen_weatherbg.jpg`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/css/zen/variables.yaml` & `appdaemon-4.4.2/appdaemon/assets/css/zen/variables.yaml`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/fonts/TickingTimebombBB.ttf` & `appdaemon-4.4.2/appdaemon/assets/fonts/TickingTimebombBB.ttf`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/fonts/climacons-webfont.eot` & `appdaemon-4.4.2/appdaemon/assets/fonts/climacons-webfont.eot`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/fonts/climacons-webfont.svg` & `appdaemon-4.4.2/appdaemon/assets/fonts/climacons-webfont.svg`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/fonts/climacons-webfont.ttf` & `appdaemon-4.4.2/appdaemon/assets/fonts/climacons-webfont.ttf`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/fonts/climacons-webfont.woff` & `appdaemon-4.4.2/appdaemon/assets/fonts/climacons-webfont.woff`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/fonts/digital-7-mono.eot` & `appdaemon-4.4.2/appdaemon/assets/fonts/digital-7-mono.eot`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/fonts/digital-7-mono.ttf` & `appdaemon-4.4.2/appdaemon/assets/fonts/digital-7-mono.ttf`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/fonts/materialdesignicons-webfont.eot` & `appdaemon-4.4.2/appdaemon/assets/fonts/materialdesignicons-webfont.eot`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/fonts/materialdesignicons-webfont.ttf` & `appdaemon-4.4.2/appdaemon/assets/fonts/materialdesignicons-webfont.ttf`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/fonts/materialdesignicons-webfont.woff` & `appdaemon-4.4.2/appdaemon/assets/fonts/materialdesignicons-webfont.woff`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/fonts/materialdesignicons-webfont.woff2` & `appdaemon-4.4.2/appdaemon/assets/fonts/materialdesignicons-webfont.woff2`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/fonts/repetition.ttf` & `appdaemon-4.4.2/appdaemon/assets/fonts/repetition.ttf`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/images/android-chrome-192x192.png` & `appdaemon-4.4.2/appdaemon/assets/images/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/images/android-chrome-512x512.png` & `appdaemon-4.4.2/appdaemon/assets/images/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/images/apple-touch-icon.png` & `appdaemon-4.4.2/appdaemon/assets/images/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/images/favicon-16x16.png` & `appdaemon-4.4.2/appdaemon/assets/images/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/images/favicon-32x32.png` & `appdaemon-4.4.2/appdaemon/assets/images/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/images/favicon.ico` & `appdaemon-4.4.2/appdaemon/assets/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/images/mstile-144x144.png` & `appdaemon-4.4.2/appdaemon/assets/images/mstile-144x144.png`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/images/mstile-150x150.png` & `appdaemon-4.4.2/appdaemon/assets/images/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/images/mstile-310x150.png` & `appdaemon-4.4.2/appdaemon/assets/images/mstile-310x150.png`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/images/mstile-310x310.png` & `appdaemon-4.4.2/appdaemon/assets/images/mstile-310x310.png`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/images/mstile-70x70.png` & `appdaemon-4.4.2/appdaemon/assets/images/mstile-70x70.png`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/javascript/admin.js` & `appdaemon-4.4.2/appdaemon/assets/javascript/admin.js`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/javascript/d3.layout.min.js` & `appdaemon-4.4.2/appdaemon/assets/javascript/d3.layout.min.js`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/javascript/d3.min.js` & `appdaemon-4.4.2/appdaemon/assets/javascript/d3.min.js`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/javascript/dashboard.js` & `appdaemon-4.4.2/appdaemon/assets/javascript/dashboard.js`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/javascript/gauge.min.js` & `appdaemon-4.4.2/appdaemon/assets/javascript/gauge.min.js`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/javascript/jquery-3.1.1.min.js` & `appdaemon-4.4.2/appdaemon/assets/javascript/jquery-3.1.1.min.js`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/javascript/jquery-ui.js` & `appdaemon-4.4.2/appdaemon/assets/javascript/jquery-ui.js`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/javascript/jquery.gridster.js` & `appdaemon-4.4.2/appdaemon/assets/javascript/jquery.gridster.js`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/javascript/justgage.js` & `appdaemon-4.4.2/appdaemon/assets/javascript/justgage.js`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/javascript/knockout-3.4.1.js` & `appdaemon-4.4.2/appdaemon/assets/javascript/knockout-3.4.1.js`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/javascript/list.min.js` & `appdaemon-4.4.2/appdaemon/assets/javascript/list.min.js`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/javascript/plotly.min.js` & `appdaemon-4.4.2/appdaemon/assets/javascript/plotly.min.js`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/javascript/raphael-2.1.4.min.js` & `appdaemon-4.4.2/appdaemon/assets/javascript/raphael-2.1.4.min.js`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/javascript/reconnecting-websocket.min.js` & `appdaemon-4.4.2/appdaemon/assets/javascript/reconnecting-websocket.min.js`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/javascript/rickshaw.min.js` & `appdaemon-4.4.2/appdaemon/assets/javascript/rickshaw.min.js`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/javascript/socket.io.js` & `appdaemon-4.4.2/appdaemon/assets/javascript/socket.io.js`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/javascript/sockjs.min.js` & `appdaemon-4.4.2/appdaemon/assets/javascript/sockjs.min.js`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/javascript/stream.js` & `appdaemon-4.4.2/appdaemon/assets/javascript/stream.js`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/templates/admin.jinja2` & `appdaemon-4.4.2/appdaemon/assets/templates/admin.jinja2`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/templates/dashboard.jinja2` & `appdaemon-4.4.2/appdaemon/assets/templates/dashboard.jinja2`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/templates/dashinit.jinja2` & `appdaemon-4.4.2/appdaemon/assets/templates/dashinit.jinja2`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/templates/error.jinja2` & `appdaemon-4.4.2/appdaemon/assets/templates/error.jinja2`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/templates/list.jinja2` & `appdaemon-4.4.2/appdaemon/assets/templates/list.jinja2`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/templates/logon.jinja2` & `appdaemon-4.4.2/appdaemon/assets/templates/logon.jinja2`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/webfonts/fa-brands-400.eot` & `appdaemon-4.4.2/appdaemon/assets/webfonts/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/webfonts/fa-brands-400.svg` & `appdaemon-4.4.2/appdaemon/assets/webfonts/fa-brands-400.svg`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/webfonts/fa-brands-400.ttf` & `appdaemon-4.4.2/appdaemon/assets/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/webfonts/fa-brands-400.woff` & `appdaemon-4.4.2/appdaemon/assets/webfonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/webfonts/fa-brands-400.woff2` & `appdaemon-4.4.2/appdaemon/assets/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/webfonts/fa-regular-400.eot` & `appdaemon-4.4.2/appdaemon/assets/webfonts/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/webfonts/fa-regular-400.svg` & `appdaemon-4.4.2/appdaemon/assets/webfonts/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/webfonts/fa-regular-400.ttf` & `appdaemon-4.4.2/appdaemon/assets/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/webfonts/fa-regular-400.woff` & `appdaemon-4.4.2/appdaemon/assets/webfonts/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/webfonts/fa-regular-400.woff2` & `appdaemon-4.4.2/appdaemon/assets/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/webfonts/fa-solid-900.eot` & `appdaemon-4.4.2/appdaemon/assets/webfonts/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/webfonts/fa-solid-900.svg` & `appdaemon-4.4.2/appdaemon/assets/webfonts/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/webfonts/fa-solid-900.ttf` & `appdaemon-4.4.2/appdaemon/assets/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/webfonts/fa-solid-900.woff` & `appdaemon-4.4.2/appdaemon/assets/webfonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/assets/webfonts/fa-solid-900.woff2` & `appdaemon-4.4.2/appdaemon/assets/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/callbacks.py` & `appdaemon-4.4.2/appdaemon/callbacks.py`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/dashboard.py` & `appdaemon-4.4.2/appdaemon/dashboard.py`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/entity.py` & `appdaemon-4.4.2/appdaemon/entity.py`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/events.py` & `appdaemon-4.4.2/appdaemon/events.py`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/futures.py` & `appdaemon-4.4.2/appdaemon/futures.py`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/http.py` & `appdaemon-4.4.2/appdaemon/http.py`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/logging.py` & `appdaemon-4.4.2/appdaemon/logging.py`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/plugin_management.py` & `appdaemon-4.4.2/appdaemon/plugin_management.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,17 +15,48 @@
     Base class for plugins to set up _logging
     """
 
     def __init__(self, ad: AppDaemon, name, args):
         self.AD = ad
         self.logger = self.AD.logging.get_child(name)
 
+        # Performance Data
+
+        self.bytes_sent = 0
+        self.bytes_recv = 0
+        self.requests_sent = 0
+        self.updates_recv = 0
+        self.last_check_ts = 0
+
     def set_log_level(self, level):
         self.logger.setLevel(self.AD.logging.log_levels[level])
 
+    async def perf_data(self):
+        data = {
+            "bytes_sent": self.bytes_sent,
+            "bytes_recv": self.bytes_recv,
+            "requests_sent": self.requests_sent,
+            "updates_recv": self.updates_recv,
+            "duration": await self.AD.sched.get_now_ts() - self.last_check_ts,
+        }
+
+        self.bytes_sent = 0
+        self.bytes_recv = 0
+        self.requests_sent = 0
+        self.updates_recv = 0
+        self.last_check_ts = await self.AD.sched.get_now_ts()
+
+        return data
+
+    def update_perf(self, **kwargs):
+        self.bytes_sent += kwargs.get("bytes_sent", 0)
+        self.bytes_recv += kwargs.get("bytes_recv", 0)
+        self.requests_sent += kwargs.get("requests_sent", 0)
+        self.updates_recv += kwargs.get("updates_recv", 0)
+
 
 class Plugins:
     required_meta = ["latitude", "longitude", "elevation", "time_zone"]
 
     def __init__(self, ad: AppDaemon, kwargs):
         self.AD = ad
         self.plugins = kwargs
@@ -70,14 +101,17 @@
                 else:
                     if "refresh_delay" not in self.plugins[name]:
                         self.plugins[name]["refresh_delay"] = 600
 
                     if "refresh_timeout" not in self.plugins[name]:
                         self.plugins[name]["refresh_timeout"] = 30
 
+                    if "use_dictionary_unpacking" not in self.plugins[name]:
+                        self.plugins[name]["use_dictionary_unpacking"] = True
+
                     basename = self.plugins[name]["type"]
                     type = self.plugins[name]["type"]
                     module_name = "{}plugin".format(basename)
                     class_name = "{}Plugin".format(basename.capitalize())
 
                     full_module_name = None
                     for plugin in plugins:
@@ -118,15 +152,16 @@
                             self.plugins[name]["namespace"] = namespace
 
                         self.plugin_objs[namespace] = {"object": plugin, "active": False, "name": name}
 
                         #
                         # Create app entry for the plugin so we can listen_state/event
                         #
-                        self.AD.app_management.init_plugin_object(name, plugin)
+                        use_dictionary_unpacking = self.plugins[name]["use_dictionary_unpacking"]
+                        self.AD.app_management.init_plugin_object(name, plugin, use_dictionary_unpacking)
 
                         self.AD.loop.create_task(plugin.get_updates())
                     except Exception:
                         self.logger.warning("error loading plugin: %s - ignoring", name)
                         self.logger.warning("-" * 60)
                         self.logger.warning(traceback.format_exc())
                         self.logger.warning("-" * 60)
@@ -262,15 +297,22 @@
                     #
                     # Create plugin entity
                     #
                     await self.AD.state.add_entity(
                         "admin",
                         "plugin.{}".format(name),
                         "active",
-                        {"bytes_sent_ps": 0, "bytes_recv_ps": 0, "requests_sent_ps": 0, "updates_recv_ps": 0},
+                        {
+                            "bytes_sent_ps": 0,
+                            "bytes_recv_ps": 0,
+                            "requests_sent_ps": 0,
+                            "updates_recv_ps": 0,
+                            "totalcallbacks": 0,
+                            "instancecallbacks": 0,
+                        },
                     )
 
                     self.logger.info("Got initial state from namespace %s", namespace)
 
                 self.plugin_objs[namespace]["active"] = True
                 await self.AD.events.process_event(namespace, {"event_type": "plugin_started", "data": {"name": name}})
         except Exception:
```

### Comparing `appdaemon-4.4.1/appdaemon/plugins/dummy/dummyapi.py` & `appdaemon-4.4.2/appdaemon/plugins/dummy/dummyapi.py`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/plugins/dummy/dummyplugin.py` & `appdaemon-4.4.2/appdaemon/plugins/dummy/dummyplugin.py`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/plugins/hass/hassapi.py` & `appdaemon-4.4.2/appdaemon/plugins/hass/hassapi.py`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/plugins/hass/hassplugin.py` & `appdaemon-4.4.2/appdaemon/plugins/hass/hassplugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,47 +79,16 @@
         # Internal state flags
         self.already_notified = False
         self.first_time = False
         self.hass_booting = False
         self.reading_messages = False
         self.stopping = False
 
-        # Performance Data
-
-        self.bytes_sent = 0
-        self.bytes_recv = 0
-        self.requests_sent = 0
-        self.updates_recv = 0
-        self.last_check_ts = 0
-
         self.logger.info("HASS Plugin initialization complete")
 
-    async def perf_data(self):
-        data = {
-            "bytes_sent": self.bytes_sent,
-            "bytes_recv": self.bytes_recv,
-            "requests_sent": self.requests_sent,
-            "updates_recv": self.updates_recv,
-            "duration": await self.AD.sched.get_now_ts() - self.last_check_ts,
-        }
-
-        self.bytes_sent = 0
-        self.bytes_recv = 0
-        self.requests_sent = 0
-        self.updates_recv = 0
-        self.last_check_ts = await self.AD.sched.get_now_ts()
-
-        return data
-
-    def update_perf(self, **kwargs):
-        self.bytes_sent += kwargs.get("bytes_sent", 0)
-        self.bytes_recv += kwargs.get("bytes_recv", 0)
-        self.requests_sent += kwargs.get("requests_sent", 0)
-        self.updates_recv += kwargs.get("updates_recv", 0)
-
     async def am_reading_messages(self):
         return self.reading_messages
 
     def stop(self):
         self.logger.debug("stop() called for %s", self.name)
         self.stopping = True
         if self.ws is not None:
@@ -540,15 +509,15 @@
         #
         # If data is a string just assume it's an entity_id
         #
         if isinstance(data, str):
             data = {"entity_id": data}
 
         if domain == "template" and service == "render":
-            api_url = "/api/template"
+            api_url = f"{self.ha_url}/api/template"
 
         elif domain == "database":
             return await self.get_history(**data)
 
         else:
             api_url = f"{self.ha_url}/api/services/{domain}/{service}"
```

### Comparing `appdaemon-4.4.1/appdaemon/plugins/mqtt/mqttapi.py` & `appdaemon-4.4.2/appdaemon/plugins/mqtt/mqttapi.py`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/plugins/mqtt/mqttplugin.py` & `appdaemon-4.4.2/appdaemon/plugins/mqtt/mqttplugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,22 +19,14 @@
         self.stopping = False
         self.config = args
         self.name = name
         self.initialized = False
         self.mqtt_connected = False
         self.state = {}
 
-        # Performance Data
-
-        self.bytes_sent = 0
-        self.bytes_recv = 0
-        self.requests_sent = 0
-        self.updates_recv = 0
-        self.last_check_ts = 0
-
         self.logger.info("MQTT Plugin Initializing")
 
         self.name = name
 
         if "namespace" in self.config:
             self.namespace = self.config["namespace"]
         else:
@@ -140,37 +132,14 @@
             "tls_version": self.mqtt_tls_version,
             "timeout": self.mqtt_client_timeout,
             "force_state": self.mqtt_client_force_start,
         }
 
         self.mqtt_connect_event = None
 
-    async def perf_data(self):
-        data = {
-            "bytes_sent": self.bytes_sent,
-            "bytes_recv": self.bytes_recv,
-            "requests_sent": self.requests_sent,
-            "updates_recv": self.updates_recv,
-            "duration": await self.AD.sched.get_now_ts() - self.last_check_ts,
-        }
-
-        self.bytes_sent = 0
-        self.bytes_recv = 0
-        self.requests_sent = 0
-        self.updates_recv = 0
-        self.last_check_ts = await self.AD.sched.get_now_ts()
-
-        return data
-
-    def update_perf(self, **kwargs):
-        self.bytes_sent += kwargs.get("bytes_sent", 0)
-        self.bytes_recv += kwargs.get("bytes_recv", 0)
-        self.requests_sent += kwargs.get("requests_sent", 0)
-        self.updates_recv += kwargs.get("updates_recv", 0)
-
     def stop(self):
         self.logger.debug("stop() called for %s", self.name)
         self.stopping = True
         if self.mqtt_connected:
             self.logger.info(
                 "Stopping MQTT Plugin and Unsubscribing from URL %s:%s",
                 self.mqtt_client_host,
```

### Comparing `appdaemon-4.4.1/appdaemon/pyversions.py` & `appdaemon-4.4.2/appdaemon/pyversions.py`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/scheduler.py` & `appdaemon-4.4.2/appdaemon/scheduler.py`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/sequences.py` & `appdaemon-4.4.2/appdaemon/sequences.py`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/services.py` & `appdaemon-4.4.2/appdaemon/services.py`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/state.py` & `appdaemon-4.4.2/appdaemon/state.py`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/stream/adstream.py` & `appdaemon-4.4.2/appdaemon/stream/adstream.py`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/stream/socketio_handler.py` & `appdaemon-4.4.2/appdaemon/stream/socketio_handler.py`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/stream/sockjs_handler.py` & `appdaemon-4.4.2/appdaemon/stream/sockjs_handler.py`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/stream/ws_handler.py` & `appdaemon-4.4.2/appdaemon/stream/ws_handler.py`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/thread_async.py` & `appdaemon-4.4.2/appdaemon/thread_async.py`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/threading.py` & `appdaemon-4.4.2/appdaemon/threading.py`

 * *Files 2% similar despite different names*

```diff
@@ -866,19 +866,27 @@
         error_logger = logging.getLogger("Error.{}".format(name))
         args["kwargs"]["__thread_id"] = thread_id
         callback = "{}() in {}".format(funcref.__name__, name)
         silent = False
         if "__silent" in args["kwargs"]:
             silent = args["kwargs"]["__silent"]
 
-        app_args = self.AD.app_management.app_config[args["name"]]
-        if "use_dictionary_unpacking" in app_args:
-            use_dictionary_unpacking = app_args["use_dictionary_unpacking"]
-        else:
-            use_dictionary_unpacking = self.AD.use_dictionary_unpacking
+        # first we get AD's level directive
+        use_dictionary_unpacking = self.AD.use_dictionary_unpacking
+
+        # app level config takes priority so processed after AD's
+        if args["name"] in self.AD.app_management.app_config:
+            app_args = self.AD.app_management.app_config[args["name"]]
+
+            if "use_dictionary_unpacking" in app_args:
+                use_dictionary_unpacking = app_args["use_dictionary_unpacking"]
+
+        elif args["name"] in self.AD.app_management.objects:
+            # plugin's directive is to use dictionary unpacking
+            use_dictionary_unpacking = self.AD.app_management.objects[args["name"]]["use_dictionary_unpacking"]
 
         app = await self.AD.app_management.get_app_instance(name, objectid)
         if app is not None:
             try:
                 if _type == "scheduler":
                     try:
                         await self.update_thread_info("async", callback, name, _type, _id, silent)
```

### Comparing `appdaemon-4.4.1/appdaemon/utility_loop.py` & `appdaemon-4.4.2/appdaemon/utility_loop.py`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/utils.py` & `appdaemon-4.4.2/appdaemon/utils.py`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/alarm.yaml` & `appdaemon-4.4.2/appdaemon/widgets/alarm.yaml`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/basealarm/basealarm.css` & `appdaemon-4.4.2/appdaemon/widgets/basealarm/basealarm.css`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/basealarm/basealarm.html` & `appdaemon-4.4.2/appdaemon/widgets/basealarm/basealarm.html`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/basealarm/basealarm.js` & `appdaemon-4.4.2/appdaemon/widgets/basealarm/basealarm.js`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/basecamera/basecamera.css` & `appdaemon-4.4.2/appdaemon/widgets/basecamera/basecamera.css`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/basecamera/basecamera.js` & `appdaemon-4.4.2/appdaemon/widgets/basecamera/basecamera.js`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/baseclimate/baseclimate.css` & `appdaemon-4.4.2/appdaemon/widgets/baseclimate/baseclimate.css`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/baseclimate/baseclimate.html` & `appdaemon-4.4.2/appdaemon/widgets/baseclimate/baseclimate.html`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/baseclimate/baseclimate.js` & `appdaemon-4.4.2/appdaemon/widgets/baseclimate/baseclimate.js`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/baseclock/baseclock.js` & `appdaemon-4.4.2/appdaemon/widgets/baseclock/baseclock.js`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/basedatetime/basedatetime.css` & `appdaemon-4.4.2/appdaemon/widgets/basedatetime/basedatetime.css`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/basedatetime/basedatetime.js` & `appdaemon-4.4.2/appdaemon/widgets/basedatetime/basedatetime.js`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/basedisplay/basedisplay.css` & `appdaemon-4.4.2/appdaemon/widgets/basedisplay/basedisplay.css`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/basedisplay/basedisplay.js` & `appdaemon-4.4.2/appdaemon/widgets/basedisplay/basedisplay.js`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/baseentitypicture/baseentitypicture.js` & `appdaemon-4.4.2/appdaemon/widgets/baseentitypicture/baseentitypicture.js`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/baseerror/baseerror.js` & `appdaemon-4.4.2/appdaemon/widgets/baseerror/baseerror.js`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/basefan/basefan.css` & `appdaemon-4.4.2/appdaemon/widgets/basefan/basefan.css`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/basefan/basefan.html` & `appdaemon-4.4.2/appdaemon/widgets/basefan/basefan.html`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/basefan/basefan.js` & `appdaemon-4.4.2/appdaemon/widgets/basefan/basefan.js`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/basegauge/basegauge.js` & `appdaemon-4.4.2/appdaemon/widgets/basegauge/basegauge.js`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/baseheater/baseheater.css` & `appdaemon-4.4.2/appdaemon/widgets/baseheater/baseheater.css`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/baseheater/baseheater.js` & `appdaemon-4.4.2/appdaemon/widgets/baseheater/baseheater.js`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/baseicon/baseicon.js` & `appdaemon-4.4.2/appdaemon/widgets/baseicon/baseicon.js`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/baseiframe/baseiframe.css` & `appdaemon-4.4.2/appdaemon/widgets/baseiframe/baseiframe.css`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/baseiframe/baseiframe.js` & `appdaemon-4.4.2/appdaemon/widgets/baseiframe/baseiframe.js`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/baseinputnumber/baseinputnumber.css` & `appdaemon-4.4.2/appdaemon/widgets/baseinputnumber/baseinputnumber.css`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/baseinputnumber/baseinputnumber.html` & `appdaemon-4.4.2/appdaemon/widgets/baseinputnumber/baseinputnumber.html`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/baseinputnumber/baseinputnumber.js` & `appdaemon-4.4.2/appdaemon/widgets/baseinputnumber/baseinputnumber.js`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/basejavascript/basejavascript.js` & `appdaemon-4.4.2/appdaemon/widgets/basejavascript/basejavascript.js`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/baselight/baselight.css` & `appdaemon-4.4.2/appdaemon/widgets/baselight/baselight.css`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/baselight/baselight.html` & `appdaemon-4.4.2/appdaemon/widgets/baselight/baselight.html`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/baselight/baselight.js` & `appdaemon-4.4.2/appdaemon/widgets/baselight/baselight.js`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/basemedia/basemedia.css` & `appdaemon-4.4.2/appdaemon/widgets/basemedia/basemedia.css`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/basemedia/basemedia.html` & `appdaemon-4.4.2/appdaemon/widgets/basemedia/basemedia.html`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/basemedia/basemedia.js` & `appdaemon-4.4.2/appdaemon/widgets/basemedia/basemedia.js`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/baseradial/baseradial.js` & `appdaemon-4.4.2/appdaemon/widgets/baseradial/baseradial.js`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/baserss/baserss.js` & `appdaemon-4.4.2/appdaemon/widgets/baserss/baserss.js`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/baseselect/baseselect.css` & `appdaemon-4.4.2/appdaemon/widgets/baseselect/baseselect.css`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/baseselect/baseselect.js` & `appdaemon-4.4.2/appdaemon/widgets/baseselect/baseselect.js`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/baseslider/baseslider.css` & `appdaemon-4.4.2/appdaemon/widgets/baseslider/baseslider.css`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/baseslider/baseslider.html` & `appdaemon-4.4.2/appdaemon/widgets/baseslider/baseslider.html`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/baseslider/baseslider.js` & `appdaemon-4.4.2/appdaemon/widgets/baseslider/baseslider.js`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/baseswitch/baseswitch.js` & `appdaemon-4.4.2/appdaemon/widgets/baseswitch/baseswitch.js`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/basetemperature/basetemperature.js` & `appdaemon-4.4.2/appdaemon/widgets/basetemperature/basetemperature.js`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/basetext/basetext.css` & `appdaemon-4.4.2/appdaemon/widgets/basetext/basetext.css`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/basetext/basetext.js` & `appdaemon-4.4.2/appdaemon/widgets/basetext/basetext.js`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/baseweather/baseweather.css` & `appdaemon-4.4.2/appdaemon/widgets/baseweather/baseweather.css`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/baseweather/baseweather.html` & `appdaemon-4.4.2/appdaemon/widgets/baseweather/baseweather.html`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/baseweather/baseweather.js` & `appdaemon-4.4.2/appdaemon/widgets/baseweather/baseweather.js`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/binary_sensor.yaml` & `appdaemon-4.4.2/appdaemon/widgets/binary_sensor.yaml`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/climate.yaml` & `appdaemon-4.4.2/appdaemon/widgets/climate.yaml`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/cover.yaml` & `appdaemon-4.4.2/appdaemon/widgets/cover.yaml`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/device_tracker.yaml` & `appdaemon-4.4.2/appdaemon/widgets/device_tracker.yaml`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/fan.yaml` & `appdaemon-4.4.2/appdaemon/widgets/fan.yaml`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/group.yaml` & `appdaemon-4.4.2/appdaemon/widgets/group.yaml`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/heater.yaml` & `appdaemon-4.4.2/appdaemon/widgets/heater.yaml`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/input_boolean.yaml` & `appdaemon-4.4.2/appdaemon/widgets/input_boolean.yaml`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/input_datetime.yaml` & `appdaemon-4.4.2/appdaemon/widgets/input_datetime.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,14 @@
 static_css:
   title_style: $input_datetime_title_style
   title2_style: $input_datetime_title2_style
   unit_style: ""
   date_value_style: $input_datetime_date_style
   time_value_style: $input_datetime_time_style
   widget_style: $input_datetime_widget_style
-  container_style: $input_datetime__container_style
+  container_style: $input_datetime_container_style
 post_service:
   service: input_datetime/set_datetime
   entity_id: "{{entity}}"
 css: []
 icons: []
 static_icons: []
```

### Comparing `appdaemon-4.4.1/appdaemon/widgets/input_number.yaml` & `appdaemon-4.4.2/appdaemon/widgets/input_number.yaml`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/input_slider.yaml` & `appdaemon-4.4.2/appdaemon/widgets/input_slider.yaml`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/light.yaml` & `appdaemon-4.4.2/appdaemon/widgets/light.yaml`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/lock.yaml` & `appdaemon-4.4.2/appdaemon/widgets/lock.yaml`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/london_underground.yaml` & `appdaemon-4.4.2/appdaemon/widgets/london_underground.yaml`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/media_player.yaml` & `appdaemon-4.4.2/appdaemon/widgets/media_player.yaml`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/mode.yaml` & `appdaemon-4.4.2/appdaemon/widgets/mode.yaml`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/person.yaml` & `appdaemon-4.4.2/appdaemon/widgets/person.yaml`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/scene.yaml` & `appdaemon-4.4.2/appdaemon/widgets/scene.yaml`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/script.yaml` & `appdaemon-4.4.2/appdaemon/widgets/script.yaml`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/sensor.yaml` & `appdaemon-4.4.2/appdaemon/widgets/sensor.yaml`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/sequence.yaml` & `appdaemon-4.4.2/appdaemon/widgets/sequence.yaml`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/switch.yaml` & `appdaemon-4.4.2/appdaemon/widgets/switch.yaml`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/text_sensor.yaml` & `appdaemon-4.4.2/appdaemon/widgets/text_sensor.yaml`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/weather.yaml` & `appdaemon-4.4.2/appdaemon/widgets/weather.yaml`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon/widgets/weather_summary.yaml` & `appdaemon-4.4.2/appdaemon/widgets/weather_summary.yaml`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon.egg-info/PKG-INFO` & `appdaemon-4.4.2/appdaemon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appdaemon
-Version: 4.4.1
+Version: 4.4.2
 Summary: Apps for the Home Assistant home automation package.
 Author-email: Andrew I Cockburn <appdaemon@acockburn.com>
 License: Apache License
         ==============
         
         _Version 2.0, January 2004_
         _&lt;<http://www.apache.org/licenses/>&gt;_
```

### Comparing `appdaemon-4.4.1/appdaemon.egg-info/SOURCES.txt` & `appdaemon-4.4.2/appdaemon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/appdaemon.egg-info/requires.txt` & `appdaemon-4.4.2/appdaemon.egg-info/requires.txt`

 * *Files 15% similar despite different names*

```diff
@@ -20,22 +20,22 @@
 [:python_version < "3.8"]
 importlib-metadata
 
 [:sys_platform != "win32"]
 uvloop==0.17.0
 
 [dev]
-pip-tools~=6.12.3
+pip-tools<6.14.0,>=6.12.3
 build~=0.10.0
 flake8~=6.0.0
 black<23.4,>=23.1
-pytest~=7.2.1
+pytest<7.4.0,>=7.2.1
 ruff~=0.0.261
 
 [dev:python_version > "3.7"]
 pre-commit<3.3.0,>=3.1.1
 
 [doc]
 sphinx-autobuild~=2021.3.14
 sphinx-rtd-theme==1.1.1
-pygments~=2.14.0
+pygments<2.16,>=2.14
 myst-parser==1.0.0
```

### Comparing `appdaemon-4.4.1/conf/example_apps/ObjectTracker/general_app_functions.py` & `appdaemon-4.4.2/conf/example_apps/ObjectTracker/general_app_functions.py`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/conf/example_apps/ObjectTracker/objectcontrole.py` & `appdaemon-4.4.2/conf/example_apps/ObjectTracker/objectcontrole.py`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/conf/example_apps/alexa.py` & `appdaemon-4.4.2/conf/example_apps/alexa.py`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/conf/example_apps/battery.py` & `appdaemon-4.4.2/conf/example_apps/battery.py`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/conf/example_apps/bysykkel.py` & `appdaemon-4.4.2/conf/example_apps/bysykkel.py`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/conf/example_apps/commute.py` & `appdaemon-4.4.2/conf/example_apps/commute.py`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/conf/example_apps/dark_day.py` & `appdaemon-4.4.2/conf/example_apps/dark_day.py`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/conf/example_apps/door_notification.py` & `appdaemon-4.4.2/conf/example_apps/door_notification.py`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/conf/example_apps/eventCache.py` & `appdaemon-4.4.2/conf/example_apps/eventCache.py`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/conf/example_apps/eventMonitor.py` & `appdaemon-4.4.2/conf/example_apps/eventMonitor.py`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/conf/example_apps/grandfather.py` & `appdaemon-4.4.2/conf/example_apps/grandfather.py`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/conf/example_apps/hwcheck.py` & `appdaemon-4.4.2/conf/example_apps/hwcheck.py`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/conf/example_apps/ical.py` & `appdaemon-4.4.2/conf/example_apps/ical.py`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/conf/example_apps/minimote.py` & `appdaemon-4.4.2/conf/example_apps/minimote.py`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/conf/example_apps/modes.py` & `appdaemon-4.4.2/conf/example_apps/modes.py`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/conf/example_apps/momentary_switch.py` & `appdaemon-4.4.2/conf/example_apps/momentary_switch.py`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/conf/example_apps/motion_lights.py` & `appdaemon-4.4.2/conf/example_apps/motion_lights.py`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/conf/example_apps/motion_notification.py` & `appdaemon-4.4.2/conf/example_apps/motion_notification.py`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/conf/example_apps/occusim.py` & `appdaemon-4.4.2/conf/example_apps/occusim.py`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/conf/example_apps/outside_lights.py` & `appdaemon-4.4.2/conf/example_apps/outside_lights.py`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/conf/example_apps/presence.py` & `appdaemon-4.4.2/conf/example_apps/presence.py`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/conf/example_apps/ruter.py` & `appdaemon-4.4.2/conf/example_apps/ruter.py`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/conf/example_apps/secure.py` & `appdaemon-4.4.2/conf/example_apps/secure.py`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/conf/example_apps/sensor_notification.py` & `appdaemon-4.4.2/conf/example_apps/sensor_notification.py`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/conf/example_apps/sensor_notify.py` & `appdaemon-4.4.2/conf/example_apps/sensor_notify.py`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/conf/example_apps/sequence.py` & `appdaemon-4.4.2/conf/example_apps/sequence.py`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/conf/example_apps/smart_heat.py` & `appdaemon-4.4.2/conf/example_apps/smart_heat.py`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/conf/example_apps/sound.py` & `appdaemon-4.4.2/conf/example_apps/sound.py`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/conf/example_apps/switch_reset.py` & `appdaemon-4.4.2/conf/example_apps/switch_reset.py`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/conf/example_apps/yr.py` & `appdaemon-4.4.2/conf/example_apps/yr.py`

 * *Files identical despite different names*

### Comparing `appdaemon-4.4.1/pyproject.toml` & `appdaemon-4.4.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -49,28 +49,28 @@
 repository = "https://github.com/AppDaemon"
 changelog = "https://github.com/AppDaemon/appdaemon/blob/master/docs/HISTORY.rst"
 
 
 # Declare development dependencies as optional
 [project.optional-dependencies]
 dev = [
-    "pip-tools ~= 6.12.3",
+    "pip-tools >= 6.12.3,< 6.14.0",
     "build ~= 0.10.0",
     "flake8 ~= 6.0.0",
     "black >= 23.1,< 23.4",
     'pre-commit >= 3.1.1,< 3.3.0; python_version>"3.7"',  # pre-commit does not support Python < 3.8
-    "pytest ~= 7.2.1",
+    "pytest >= 7.2.1,< 7.4.0",
     "ruff~= 0.0.261"
 ]
 
 # Dependencies required to build the documentation using sphinx
 doc = [
     "sphinx-autobuild ~= 2021.3.14",
     "sphinx-rtd-theme == 1.1.1",
-    "pygments ~= 2.14.0",
+    "pygments >= 2.14,< 2.16",
     "myst-parser == 1.0.0",
 ]
 
 
 # Define the main CLI script
 [project.scripts]
 appdaemon = "appdaemon.__main__:main"
```

