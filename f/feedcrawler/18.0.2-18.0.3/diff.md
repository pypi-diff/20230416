# Comparing `tmp/feedcrawler-18.0.2.tar.gz` & `tmp/feedcrawler-18.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feedcrawler-18.0.2.tar", last modified: Mon Apr 10 12:23:28 2023, max compression
+gzip compressed data, was "feedcrawler-18.0.3.tar", last modified: Sun Apr 16 11:51:33 2023, max compression
```

## Comparing `feedcrawler-18.0.2.tar` & `feedcrawler-18.0.3.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:28.471537 feedcrawler-18.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-04-10 12:23:28.471537 feedcrawler-18.0.2/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     7047 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:28.455536 feedcrawler-18.0.2/feedcrawler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10864 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/crawler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:28.459536 feedcrawler-18.0.2/feedcrawler/external_sites/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_sites/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:28.459536 feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44484 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/content_all.py
--rw-r--r--   0 runner    (1001) docker     (123)    20331 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/content_shows.py
--rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:28.459536 feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/sites/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/sites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9381 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/sites/content_all_by.py
--rw-r--r--   0 runner    (1001) docker     (123)     8603 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/sites/content_all_dw.py
--rw-r--r--   0 runner    (1001) docker     (123)     7555 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/sites/content_all_ff.py
--rw-r--r--   0 runner    (1001) docker     (123)    10073 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/sites/content_all_fx.py
--rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/sites/content_all_hw.py
--rw-r--r--   0 runner    (1001) docker     (123)     8177 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/sites/content_all_nk.py
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/sites/content_all_nx.py
--rw-r--r--   0 runner    (1001) docker     (123)     7417 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/sites/content_all_ww.py
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/sites/content_custom_dd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/sites/content_shows_dj.py
--rw-r--r--   0 runner    (1001) docker     (123)    11056 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/sites/content_shows_sf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/sites/content_shows_sj.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:28.459536 feedcrawler-18.0.2/feedcrawler/external_sites/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_sites/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_sites/metadata/imdb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:28.463537 feedcrawler-18.0.2/feedcrawler/external_sites/web_search/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_sites/web_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16818 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_sites/web_search/content_all.py
--rw-r--r--   0 runner    (1001) docker     (123)    14426 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_sites/web_search/content_shows.py
--rw-r--r--   0 runner    (1001) docker     (123)    10470 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_sites/web_search/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:28.463537 feedcrawler-18.0.2/feedcrawler/external_sites/web_search/sites/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_sites/web_search/sites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_sites/web_search/sites/content_all_by.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_sites/web_search/sites/content_all_dw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_sites/web_search/sites/content_all_fx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_sites/web_search/sites/content_all_hw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_sites/web_search/sites/content_all_nk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_sites/web_search/sites/content_all_nx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:28.463537 feedcrawler-18.0.2/feedcrawler/external_tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42357 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_tools/myjd_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10406 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_tools/ombi_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5806 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_tools/overseerr_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8805 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/external_tools/plex_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:28.463537 feedcrawler-18.0.2/feedcrawler/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15020 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/jobs/feed_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    20797 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/jobs/package_watcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:28.467537 feedcrawler-18.0.2/feedcrawler/providers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21041 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/providers/common_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7403 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/providers/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10469 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/providers/gui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:28.467537 feedcrawler-18.0.2/feedcrawler/providers/http_requests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/providers/http_requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/providers/http_requests/cache_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9333 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/providers/http_requests/cloudflare_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/providers/http_requests/request_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    46194 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/providers/myjd_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9607 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/providers/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/providers/shared_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/providers/sqlite_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     7178 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/providers/url_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/providers/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:28.467537 feedcrawler-18.0.2/feedcrawler/web_interface/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/web_interface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:28.455536 feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:28.467537 feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:28.471537 feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    82113 2023-04-10 12:23:28.000000 feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/@formkit-18209bb1.js
--rw-r--r--   0 runner    (1001) docker     (123)    20729 2023-04-10 12:23:28.000000 feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/@popperjs-9847b28c.js
--rw-r--r--   0 runner    (1001) docker     (123)    63885 2023-04-10 12:23:28.000000 feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/@vue-d42f3502.js
--rw-r--r--   0 runner    (1001) docker     (123)     8868 2023-04-10 12:23:28.000000 feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/@vueuse-8ce5afe9.js
--rw-r--r--   0 runner    (1001) docker     (123)    28794 2023-04-10 12:23:28.000000 feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/axios-707ed124.js
--rw-r--r--   0 runner    (1001) docker     (123)    60695 2023-04-10 12:23:28.000000 feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-163e1b4f.js
--rw-r--r--   0 runner    (1001) docker     (123)   194314 2023-04-10 12:23:28.000000 feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-48fa63fb.css
--rw-r--r--   0 runner    (1001) docker     (123)   164360 2023-04-10 12:23:28.000000 feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-999550fa.woff
--rw-r--r--   0 runner    (1001) docker     (123)   121340 2023-04-10 12:23:28.000000 feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-cfe45b98.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    79982 2023-04-10 12:23:28.000000 feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-f7e350bb.css
--rw-r--r--   0 runner    (1001) docker     (123)    10842 2023-04-10 12:23:28.000000 feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/index-137a91df.css
--rw-r--r--   0 runner    (1001) docker     (123)   144621 2023-04-10 12:23:28.000000 feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/index-67e298b0.js
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-04-10 12:23:28.000000 feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/tippy-a1ae07b3.css
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 12:23:28.000000 feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-4ed993c7.js
--rw-r--r--   0 runner    (1001) docker     (123)    22669 2023-04-10 12:23:28.000000 feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-router-4bccd9ac.js
--rw-r--r--   0 runner    (1001) docker     (123)    50726 2023-04-10 12:23:28.000000 feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-tippy-2fb47e86.js
--rw-r--r--   0 runner    (1001) docker     (123)    18088 2023-04-10 12:23:28.000000 feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-toastification-2a2137d8.js
--rw-r--r--   0 runner    (1001) docker     (123)    12865 2023-04-10 12:23:28.000000 feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-toastification-4522082c.css
--rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-04-10 12:23:28.000000 feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/vuejs-paginate-next-23a274fb.js
--rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-04-10 12:23:28.000000 feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/vuex-c2e7db49.js
--rw-r--r--   0 runner    (1001) docker     (123)    17818 2023-04-10 12:23:27.000000 feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-10 12:23:28.000000 feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    83010 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/feedcrawler/web_interface/web_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:28.459536 feedcrawler-18.0.2/feedcrawler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-04-10 12:23:28.000000 feedcrawler-18.0.2/feedcrawler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-04-10 12:23:28.000000 feedcrawler-18.0.2/feedcrawler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 12:23:28.000000 feedcrawler-18.0.2/feedcrawler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-10 12:23:28.000000 feedcrawler-18.0.2/feedcrawler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 12:23:28.000000 feedcrawler-18.0.2/feedcrawler.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-10 12:23:28.000000 feedcrawler-18.0.2/feedcrawler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-10 12:23:28.000000 feedcrawler-18.0.2/feedcrawler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 12:23:28.471537 feedcrawler-18.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-10 12:23:01.000000 feedcrawler-18.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:51:33.730427 feedcrawler-18.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-04-16 11:51:33.730427 feedcrawler-18.0.3/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7047 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:51:33.718427 feedcrawler-18.0.3/feedcrawler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10734 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/crawler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:51:33.718427 feedcrawler-18.0.3/feedcrawler/external_sites/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_sites/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:51:33.718427 feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44484 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/content_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20327 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/content_shows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/shared.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:51:33.722427 feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/sites/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/sites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9381 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/sites/content_all_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8603 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/sites/content_all_dw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7555 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/sites/content_all_ff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10073 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/sites/content_all_fx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/sites/content_all_hw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8177 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/sites/content_all_nk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/sites/content_all_nx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7417 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/sites/content_all_ww.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/sites/content_custom_dd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/sites/content_shows_dj.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11339 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/sites/content_shows_sf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/sites/content_shows_sj.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:51:33.722427 feedcrawler-18.0.3/feedcrawler/external_sites/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_sites/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8998 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_sites/metadata/imdb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:51:33.722427 feedcrawler-18.0.3/feedcrawler/external_sites/web_search/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_sites/web_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16818 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_sites/web_search/content_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14651 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_sites/web_search/content_shows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10470 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_sites/web_search/shared.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:51:33.722427 feedcrawler-18.0.3/feedcrawler/external_sites/web_search/sites/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_sites/web_search/sites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_sites/web_search/sites/content_all_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_sites/web_search/sites/content_all_dw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_sites/web_search/sites/content_all_fx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_sites/web_search/sites/content_all_hw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_sites/web_search/sites/content_all_nk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_sites/web_search/sites/content_all_nx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:51:33.722427 feedcrawler-18.0.3/feedcrawler/external_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42357 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_tools/myjd_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10404 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_tools/ombi_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_tools/overseerr_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8805 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_tools/plex_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:51:33.722427 feedcrawler-18.0.3/feedcrawler/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14941 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/jobs/feed_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20682 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/jobs/package_watcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:51:33.726427 feedcrawler-18.0.3/feedcrawler/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20929 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/providers/common_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7403 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/providers/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10469 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/providers/gui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:51:33.726427 feedcrawler-18.0.3/feedcrawler/providers/http_requests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/providers/http_requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/providers/http_requests/cache_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9333 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/providers/http_requests/cloudflare_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/providers/http_requests/request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44206 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/providers/myjd_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9607 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/providers/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/providers/shared_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/providers/sqlite_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7178 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/providers/url_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/providers/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:51:33.726427 feedcrawler-18.0.3/feedcrawler/web_interface/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/web_interface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:51:33.718427 feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:51:33.726427 feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:51:33.730427 feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    82113 2023-04-16 11:51:33.000000 feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/@formkit-18209bb1.js
+-rw-r--r--   0 runner    (1001) docker     (123)    20729 2023-04-16 11:51:33.000000 feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/@popperjs-9847b28c.js
+-rw-r--r--   0 runner    (1001) docker     (123)    63885 2023-04-16 11:51:33.000000 feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/@vue-d42f3502.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8868 2023-04-16 11:51:33.000000 feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/@vueuse-8ce5afe9.js
+-rw-r--r--   0 runner    (1001) docker     (123)    28794 2023-04-16 11:51:33.000000 feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/axios-707ed124.js
+-rw-r--r--   0 runner    (1001) docker     (123)    60695 2023-04-16 11:51:33.000000 feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-163e1b4f.js
+-rw-r--r--   0 runner    (1001) docker     (123)   194314 2023-04-16 11:51:33.000000 feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-48fa63fb.css
+-rw-r--r--   0 runner    (1001) docker     (123)   164360 2023-04-16 11:51:33.000000 feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-999550fa.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   121340 2023-04-16 11:51:33.000000 feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-cfe45b98.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    79982 2023-04-16 11:51:33.000000 feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-f7e350bb.css
+-rw-r--r--   0 runner    (1001) docker     (123)    10842 2023-04-16 11:51:33.000000 feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/index-137a91df.css
+-rw-r--r--   0 runner    (1001) docker     (123)   144763 2023-04-16 11:51:33.000000 feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/index-44ade789.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-04-16 11:51:33.000000 feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/tippy-a1ae07b3.css
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 11:51:33.000000 feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-4ed993c7.js
+-rw-r--r--   0 runner    (1001) docker     (123)    22669 2023-04-16 11:51:33.000000 feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-router-4bccd9ac.js
+-rw-r--r--   0 runner    (1001) docker     (123)    50726 2023-04-16 11:51:33.000000 feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-tippy-2fb47e86.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18088 2023-04-16 11:51:33.000000 feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-toastification-2a2137d8.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12865 2023-04-16 11:51:33.000000 feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-toastification-4522082c.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-04-16 11:51:33.000000 feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/vuejs-paginate-next-23a274fb.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-04-16 11:51:33.000000 feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/vuex-c2e7db49.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17818 2023-04-16 11:51:32.000000 feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-16 11:51:33.000000 feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    82905 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/web_interface/web_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:51:33.718427 feedcrawler-18.0.3/feedcrawler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-04-16 11:51:33.000000 feedcrawler-18.0.3/feedcrawler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-04-16 11:51:33.000000 feedcrawler-18.0.3/feedcrawler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 11:51:33.000000 feedcrawler-18.0.3/feedcrawler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-16 11:51:33.000000 feedcrawler-18.0.3/feedcrawler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 11:51:33.000000 feedcrawler-18.0.3/feedcrawler.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-16 11:51:33.000000 feedcrawler-18.0.3/feedcrawler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-16 11:51:33.000000 feedcrawler-18.0.3/feedcrawler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 11:51:33.730427 feedcrawler-18.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/setup.py
```

### Comparing `feedcrawler-18.0.2/LICENSE.md` & `feedcrawler-18.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.2/PKG-INFO` & `feedcrawler-18.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feedcrawler
-Version: 18.0.2
+Version: 18.0.3
 Summary: Automate downloads using predefined sites and the My JDownloader API
 Home-page: https://github.com/rix1337/FeedCrawler
 Author: rix1337
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `feedcrawler-18.0.2/README.md` & `feedcrawler-18.0.3/README.md`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.2/feedcrawler/crawler.py` & `feedcrawler-18.0.3/feedcrawler/crawler.py`

 * *Files 5% similar despite different names*

```diff
@@ -84,16 +84,14 @@
                 string = string.replace('https://', '').replace('http://', '')
                 string = re.findall(r'([a-z-.]*\.[a-z]*)', string)[0]
                 hostnames.save(host, string)
             if string and re.match(r'.*[A-Z].*', string):
                 hostnames.save(host, string.lower())
             if string:
                 print('Hostname für ' + host.upper() + ": " + string)
-            else:
-                print('Hostname für ' + host.upper() + ': -')
             return string
 
         set_hostnames = {}
         shared_state.set_sites()
         for name in shared_state.values["sites"]:
             name = name.lower()
             hostname = clean_up_hostname(name, hostnames.get(name))
@@ -129,45 +127,44 @@
                                 feedcrawler.save('myjd_device', one_device)
                                 set_device_from_config()
                 else:
                     myjd_input(arguments.port, arguments.jd_user, arguments.jd_pass,
                                arguments.jd_device)
 
         if not shared_state.values["test_run"]:
-            if shared_state.values["device"] and shared_state.values["device"].name:
+            if shared_state.get_device() and shared_state.get_device().name:
                 success = True
             else:
                 success = False
                 feedcrawler = CrawlerConfig('FeedCrawler')
 
                 device_name = feedcrawler.get('myjd_device')
                 if not device_name:
                     user = feedcrawler.get('myjd_user')
                     password = feedcrawler.get('myjd_pass')
                     one_device = get_if_one_device(user, password)
                     if one_device:
                         print('Gerätename "' + one_device + '" automatisch ermittelt.')
                         feedcrawler.save('myjd_device', one_device)
                         set_device_from_config()
-                        success = shared_state.values["device"] and shared_state.values["device"].name
+                        success = shared_state.get_device() and shared_state.get_device().name
                 if not success:
                     i = 0
                     while i < 10:
                         i += 1
                         print(
                             'Verbindungsversuch %s mit My JDownloader gescheitert. Gerätename: "%s"' % (
                                 i, device_name))
                         time.sleep(60)
                         set_device_from_config()
-                        success = shared_state.values["device"] and shared_state.values["device"].name
+                        success = shared_state.get_device() and shared_state.get_device().name
                         if success:
                             break
             if success:
-                print('Erfolgreich mit My JDownloader verbunden. Gerätename: "' + shared_state.values[
-                    "device"].name + '"')
+                print('Erfolgreich mit My JDownloader verbunden. Gerätename: "' + shared_state.get_device().name + '"')
             else:
                 print('My JDownloader Zugangsversuche nicht erfolgreich! Beende FeedCrawler!')
                 sys.exit(1)
 
         feedcrawler = CrawlerConfig('FeedCrawler')
         port = int(feedcrawler.get("port"))
         docker = False
```

### Comparing `feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/content_all.py` & `feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/content_all.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/content_shows.py` & `feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/content_shows.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,17 +57,17 @@
 
 
 def send_package(self, title, link, language_id, season, episode, site, source, size, imdb_id):
     englisch = ''
     if language_id == 2:
         englisch = '/Englisch'
     if self.filename == 'List_ContentShows_Shows':
-        release_type = '[Episode' + englisch + '] - '
+        release_type = '[Folge' + englisch + '] - '
     elif self.filename == 'List_ContentShows_Shows_Regex':
-        release_type = '[Episode/RegEx' + englisch + '] - '
+        release_type = '[Folge/RegEx' + englisch + '] - '
     elif self.filename == 'List_ContentShows_Seasons_Regex':
         release_type = '[Staffel/RegEx' + englisch + '] - '
     elif self.filename == 'List_ContentAll_Seasons':
         release_type = '[Staffel' + englisch + '] - '
     elif self.filename == 'List_CustomDJ_Documentaries':
         release_type = '[Doku] - ' + englisch
     elif self.filename == 'List_CustomDJ_Documentaries_Regex':
```

### Comparing `feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/shared.py` & `feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/shared.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/sites/content_all_by.py` & `feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/sites/content_all_by.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/sites/content_all_dw.py` & `feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/sites/content_all_dw.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/sites/content_all_ff.py` & `feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/sites/content_all_ff.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/sites/content_all_fx.py` & `feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/sites/content_all_fx.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/sites/content_all_hw.py` & `feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/sites/content_all_hw.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/sites/content_all_nk.py` & `feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/sites/content_all_nk.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/sites/content_all_nx.py` & `feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/sites/content_all_nx.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/sites/content_all_ww.py` & `feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/sites/content_all_ww.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/sites/content_custom_dd.py` & `feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/sites/content_custom_dd.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
                 if title:
                     title = title.replace(" ", ".")
                     titles.append(title)
         return titles
 
     def periodical_task(self):
         if not self.url:
-            shared_state.logger.debug("Kein Hostname gesetzt. Stoppe Suche für Episoden! (" + self.filename + ")")
+            shared_state.logger.debug("Kein Hostname gesetzt. Stoppe Suche für Folgen! (" + self.filename + ")")
             return
         else:
             for feed_id in self.feed_ids:
                 feed_url = self.url + '/rss/' + feed_id
                 feed = dd_rss_feed_to_feedparser_dict(get_url(feed_url))
                 for post in feed.entries:
                     current_epoch = datetime.utcnow().timestamp()
@@ -63,15 +63,15 @@
                         if not links:
                             shared_state.logger.debug("Release ignoriert - keine Links gefunden")
                         elif 'added' in storage:
                             shared_state.logger.debug(post.title + " - Release ignoriert (bereits gefunden)")
                         else:
                             if myjd_download(post.title, "FeedCrawler", links, self.url):
                                 self.db.store(post.title, 'added')
-                                log_entry = '[Episode/Englisch] - ' + post.title + ' - [' + self._SITE + '] - ' \
+                                log_entry = '[Folge/Englisch] - ' + post.title + ' - [' + self._SITE + '] - ' \
                                             + post.size + ' - ' + post.source
                                 shared_state.logger.info(log_entry)
                                 notify([{"text": log_entry, 'imdb_id': post.imdb_id}])
                     else:
                         shared_state.logger.debug(
                             post.title + " - Releases, die weniger als 30 Minuten alt sind, werden ignoriert (da Links noch hochgeladen werden).")
```

### Comparing `feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/sites/content_shows_dj.py` & `feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/sites/content_shows_dj.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/sites/content_shows_sf.py` & `feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/sites/content_shows_sf.py`

 * *Files 4% similar despite different names*

```diff
@@ -165,17 +165,15 @@
             info = json.loads(clean_response_content)
 
         is_episode = re.findall(r'.*\.(s\d{1,3}e\d{1,3})\..*', title, re.IGNORECASE)
         multiple_episodes = False
         if is_episode:
             episode_string = re.findall(r'.*S\d{1,3}(E\d{1,3}).*', is_episode[0])[0].lower()
             season_string = re.findall(r'.*(S\d{1,3})E\d{1,3}.*', is_episode[0])[0].lower()
-            season_title = rreplace(title.lower().replace(episode_string, ''), "-", ".*", 1).lower().replace(
-                ".repack", "")
-            season_title = season_title.replace(".untouched", ".*").replace(".dd+51", ".dd.51")
+            season_title = rreplace(title.lower().replace(episode_string, ''), "-", ".*", 1).lower()
             episode = str(int(episode_string.replace("e", "")))
             season = str(int(season_string.replace("s", "")))
             episode_name = re.findall(r'.*\.s\d{1,3}(\..*).german', season_title, re.IGNORECASE)
             if episode_name:
                 season_title = season_title.replace(episode_name[0], '')
             codec_tags = [".h264", ".x264"]
             for tag in codec_tags:
@@ -187,14 +185,27 @@
             season = False
             episode = False
             season_title = title
             multiple_episodes = re.findall(r'(e\d{1,3}-e*\d{1,3}\.)', season_title, re.IGNORECASE)
             if multiple_episodes:
                 season_title = season_title.replace(multiple_episodes[0], '.*')
 
+        season_title = season_title. \
+            replace(".internal", ""). \
+            replace(".extended", ""). \
+            replace(".uncut", ""). \
+            replace(".remastered", ""). \
+            replace(".remux", ""). \
+            replace(".repack", ""). \
+            replace(".dc", ""). \
+            replace(".untouched", ""). \
+            replace(".dd+51", ".dd.51")
+
+        season_title += ".*"
+
         content = BeautifulSoup(info['html'], "html.parser")
         try:
             release_info = content.find("small", text=re.compile(season_title, re.IGNORECASE)).parent.parent.parent
         except:
             print(title + " wird im Feed referenziert, fehlt jedoch auf der Download-Seite!")
             return False
```

### Comparing `feedcrawler-18.0.2/feedcrawler/external_sites/feed_search/sites/content_shows_sj.py` & `feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/sites/content_shows_sj.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.2/feedcrawler/external_sites/metadata/imdb.py` & `feedcrawler-18.0.3/feedcrawler/external_sites/metadata/imdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,16 +172,16 @@
                     eps.append(i)
                     i += 1
                 episodes[int(sn)] = eps
     except:
         pass
 
     if not episodes:
-        print("[IMDb] - %s - Keine Episoden gefunden" % imdb_id)
-        shared_state.logger.debug("[IMDb] - %s - Keine Episoden gefunden" % imdb_id)
+        print("[IMDb] - %s - Keine Folgen gefunden" % imdb_id)
+        shared_state.logger.debug("[IMDb] - %s - Keine Folgen gefunden" % imdb_id)
 
     return episodes
 
 
 @imdb_id_not_none
 def get_localized_title(imdb_id):
     localized_title = False
```

### Comparing `feedcrawler-18.0.2/feedcrawler/external_sites/web_search/content_all.py` & `feedcrawler-18.0.3/feedcrawler/external_sites/web_search/content_all.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.2/feedcrawler/external_sites/web_search/content_shows.py` & `feedcrawler-18.0.3/feedcrawler/external_sites/web_search/content_shows.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,18 +23,21 @@
 from feedcrawler.providers.notifications import notify
 from feedcrawler.providers.sqlite_database import ListDb, FeedDb
 from feedcrawler.providers.url_functions import get_url, get_redirected_url
 
 
 def get_best_result(title):
     try:
+        shared_state.logger.debug(f'Pushed search for: {title}')
         results = search_web(title, only_content_shows=True)
         sj_results = results[1]
         sf_results = results[2]
-    except:
+        shared_state.logger.debug(f'Got result for: {str(results)}')
+    except Exception as e:
+        shared_state.logger.debug("An exception was thrown: " + str(e))
         return False
 
     preferred_results = []
     if sf_results:
         shared_state.logger.debug('SF-Ergebnisse werden für ' + title + ' verwendet!')
         preferred_results = sf_results
     elif sj_results:
@@ -42,25 +45,25 @@
         preferred_results = sj_results
 
     best_difference = 999
     best_match = False
     best_payload = False
     for result in preferred_results:
         payload = result['payload']
-        result = result['title']
+        res_tit = result['title']
 
         len_search_term = len(title)
-        len_result = len(result)
+        len_result = len(res_tit)
 
         difference = abs(len_search_term - len_result)
 
-        if simplified_search_term_in_title(title, result):
+        if simplified_search_term_in_title(title, res_tit):
             if difference < best_difference:
                 best_difference = difference
-                best_match = result
+                best_match = res_tit
                 best_payload = payload
 
     if not best_match or not best_payload:
         shared_state.logger.debug('Kein Treffer für die Suche nach ' + title + '! Suchliste ergänzt.')
         listen = ["List_ContentShows_Shows", "List_ContentAll_Seasons"]
         for liste in listen:
             cont = ListDb(liste).retrieve()
```

### Comparing `feedcrawler-18.0.2/feedcrawler/external_sites/web_search/shared.py` & `feedcrawler-18.0.3/feedcrawler/external_sites/web_search/shared.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.2/feedcrawler/external_sites/web_search/sites/content_all_by.py` & `feedcrawler-18.0.3/feedcrawler/external_sites/web_search/sites/content_all_by.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.2/feedcrawler/external_sites/web_search/sites/content_all_dw.py` & `feedcrawler-18.0.3/feedcrawler/external_sites/web_search/sites/content_all_dw.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.2/feedcrawler/external_sites/web_search/sites/content_all_fx.py` & `feedcrawler-18.0.3/feedcrawler/external_sites/web_search/sites/content_all_fx.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.2/feedcrawler/external_sites/web_search/sites/content_all_hw.py` & `feedcrawler-18.0.3/feedcrawler/external_sites/web_search/sites/content_all_hw.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.2/feedcrawler/external_sites/web_search/sites/content_all_nk.py` & `feedcrawler-18.0.3/feedcrawler/external_sites/web_search/sites/content_all_nk.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.2/feedcrawler/external_sites/web_search/sites/content_all_nx.py` & `feedcrawler-18.0.3/feedcrawler/external_sites/web_search/sites/content_all_nx.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.2/feedcrawler/external_tools/myjd_api.py` & `feedcrawler-18.0.3/feedcrawler/external_tools/myjd_api.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.2/feedcrawler/external_tools/ombi_api.py` & `feedcrawler-18.0.3/feedcrawler/external_tools/ombi_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,14 +179,14 @@
                                                 feedcrawler.external_sites.web_search.content_shows.download(payload)
                                             for ep in eps:
                                                 e = str(ep)
                                                 if len(e) == 1:
                                                     e = "0" + e
                                                 se = s + "E" + e
                                                 db.store('show_' + str(imdb_id) + '_' + se, 'added')
-                                        print("Serie/Staffel/Episode: " + title + " durch Ombi hinzugefügt.")
+                                        print("Serie/Staffel/Folge: " + title + " durch Ombi hinzugefügt.")
         else:
             print("Eine Serie ohne IMDb-ID wurde in Ombi angefordert und kann nicht verarbeitet werden.")
             shared_state.logger.debug(
                 "Eine Serie ohne IMDb-ID wurde in Ombi angefordert und kann nicht verarbeitet werden.")
 
     return [len_movies, len_shows]
```

### Comparing `feedcrawler-18.0.2/feedcrawler/external_tools/overseerr_api.py` & `feedcrawler-18.0.3/feedcrawler/external_tools/overseerr_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,10 +112,10 @@
                 if title:
                     payload = feedcrawler.external_sites.web_search.content_shows.get_best_result(title)
                     if payload:
                         payload = decode_base64(payload).split("|")
                         payload = encode_base64(payload[0] + "|" + payload[1] + "|" + season)
                         if feedcrawler.external_sites.web_search.content_shows.download(payload):
                             db.store('show_' + str(item_id) + "_" + str(season), 'added')
-                            print("Serie/Staffel/Episode: " + title + " durch Overseerr hinzugefügt.")
+                            print("Serie/Staffel/Folge: " + title + " durch Overseerr hinzugefügt.")
 
     return [len_movies, len_shows]
```

### Comparing `feedcrawler-18.0.2/feedcrawler/external_tools/plex_api.py` & `feedcrawler-18.0.3/feedcrawler/external_tools/plex_api.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.2/feedcrawler/jobs/feed_search.py` & `feedcrawler-18.0.3/feedcrawler/jobs/feed_search.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from feedcrawler.external_sites.feed_search.sites.content_shows_sf import SF
 from feedcrawler.external_sites.feed_search.sites.content_shows_sj import SJ
 from feedcrawler.external_tools.ombi_api import ombi_search
 from feedcrawler.external_tools.overseerr_api import overseerr_search
 from feedcrawler.external_tools.plex_api import plex_search
 from feedcrawler.providers import gui
 from feedcrawler.providers import shared_state
-from feedcrawler.providers.common_functions import Unbuffered, is_device, readable_time
+from feedcrawler.providers.common_functions import Unbuffered, readable_time
 from feedcrawler.providers.config import CrawlerConfig
 from feedcrawler.providers.http_requests.cloudflare_handlers import get_solver_url
 from feedcrawler.providers.myjd_connection import get_info
 from feedcrawler.providers.myjd_connection import jdownloader_update
 from feedcrawler.providers.myjd_connection import set_device_from_config
 from feedcrawler.providers.sqlite_database import FeedDb
 from feedcrawler.providers.url_functions import check_url
@@ -101,15 +101,15 @@
         logger.debug("-----------Entferne Zeitpunkt des letzten Cloudflare-Umgehungs-Suchlaufes!-----------")
         print("-----------Entferne Zeitpunkt des letzten Cloudflare-Umgehungs-Suchlaufes!-----------")
         FeedDb('crawltimes').delete("last_cloudflare_run")
 
     while True:
         try:
             if not shared_state.values["test_run"]:
-                if not shared_state.values["device"] or not is_device(shared_state.values["device"]):
+                if not shared_state.get_device():
                     set_device_from_config()
             shared_state.clear_request_cache()
             start_time = time.time()
             check_url(start_time)
             crawltimes.update_store("active", "True")
             crawltimes.update_store("start_time", start_time * 1000)
             logger.debug("-----------Alle Suchläufe gestartet.-----------")
@@ -257,23 +257,23 @@
                         "JDownloader Update steht bereit und JDownloader ist inaktiv.\nFühre Update durch und starte JDownloader neu...")
                     jdownloader_update()
                 elif myjd_update_ready:
                     print(
                         "JDownloader Update steht bereit, aber JDownloader ist aktiv.\nFühre das Update nicht automatisch durch.")
             hide_donation_banner = CrawlerConfig('SponsorsHelper').get('hide_donation_banner')
             if hide_donation_banner:
-                current_donation_banner_setting = shared_state.values["device"].config.get(
+                current_donation_banner_setting = shared_state.get_device().config.get(
                     'org.jdownloader.settings.GraphicalUserInterfaceSettings',
                     'null',
                     'DonateButtonState')
                 if current_donation_banner_setting != "CUSTOM_HIDDEN":
                     print("Blende das Spenden-Banner im JDownloader aus.")
-                    shared_state.values["device"].config.set('org.jdownloader.settings.GraphicalUserInterfaceSettings',
-                                                             'null',
-                                                             'DonateButtonState', "CUSTOM_HIDDEN")
+                    shared_state.get_device().config.set('org.jdownloader.settings.GraphicalUserInterfaceSettings',
+                                                         'null',
+                                                         'DonateButtonState', "CUSTOM_HIDDEN")
 
             # Clean exit if test run active
             if shared_state.values["test_run"]:
                 logger.debug("-----------Testlauf beendet!-----------")
                 print("-----------Testlauf beendet!-----------")
                 return
```

### Comparing `feedcrawler-18.0.2/feedcrawler/jobs/package_watcher.py` & `feedcrawler-18.0.3/feedcrawler/jobs/package_watcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 import sys
 import time
 import traceback
 
 from feedcrawler.providers import gui
 from feedcrawler.providers import shared_state
 from feedcrawler.providers.common_functions import Unbuffered
-from feedcrawler.providers.common_functions import is_device
 from feedcrawler.providers.common_functions import longest_substr
 from feedcrawler.providers.config import CrawlerConfig
 from feedcrawler.providers.myjd_connection import add_decrypt
 from feedcrawler.providers.myjd_connection import get_info
 from feedcrawler.providers.myjd_connection import hoster_check
 from feedcrawler.providers.myjd_connection import jdownloader_start
 from feedcrawler.providers.myjd_connection import move_to_downloads
@@ -41,15 +40,15 @@
     autostart = crawljobs.get("autostart")
     db = FeedDb('crawldog')
 
     grabber_was_collecting = False
 
     while True:
         try:
-            if not shared_state.values["device"] or not is_device(shared_state.values["device"]):
+            if not shared_state.get_device():
                 set_device_from_config()
 
             myjd_packages = get_info()
             if myjd_packages:
                 grabber_collecting = myjd_packages[2]
 
                 if grabber_was_collecting or grabber_collecting:
@@ -100,15 +99,15 @@
 
                                                 if season_string:
                                                     more_episodes = FeedDb(
                                                         'episode_remover').retrieve_all_beginning_with(season_string)
                                                     for ep in more_episodes:
                                                         if title[0] not in ep:
                                                             additional_eps = FeedDb('episode_remover').retrieve(ep)
-                                                            # This happens if multiple Episodes are waiting for decryption
+                                                            # This happens if multiple Folges are waiting for decryption
                                                             if additional_eps:
                                                                 try:
                                                                     additional_eps = additional_eps.split("|")
                                                                 except:
                                                                     additional_eps = [additional_eps]
 
                                                                 episodes = episodes + additional_eps
```

### Comparing `feedcrawler-18.0.2/feedcrawler/providers/common_functions.py` & `feedcrawler-18.0.3/feedcrawler/providers/common_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 import datetime
 import os
 import re
 import socket
 import sys
 from urllib.parse import urlparse
 
-from feedcrawler.external_tools import myjd_api
 from feedcrawler.providers import gui
 from feedcrawler.providers import shared_state
 from feedcrawler.providers.config import CrawlerConfig
 from feedcrawler.providers.sqlite_database import FeedDb
 from feedcrawler.providers.sqlite_database import ListDb
 
 
@@ -152,15 +151,15 @@
                         else:
                             all_episodes = list(int_episodes)
                         if set(required_episodes).issubset(all_episodes):
                             for ep in all_episodes:
                                 if ep == int(episode_in_title):
                                     results = results + [result]
             except:
-                print("Fehler in Episodenerkennung. Bitte Issue auf Github öffnen: " + title)
+                print("Fehler in Folgen-Erkennung. Bitte Issue auf Github öffnen: " + title)
 
             season_search_title = search_title.replace(title_with_episodes[0], "") + "."
             season_results = db.retrieve_all_beginning_with(season_search_title)
             results = results + db.retrieve_all_beginning_with(search_title) + season_results
     else:
         db = FeedDb('FeedCrawler')
         results = db.retrieve_all_beginning_with(search_title)
@@ -333,18 +332,14 @@
             return packages
         else:
             return False
     except:
         return False
 
 
-def is_device(device):
-    return isinstance(device, (type, myjd_api.Jddevice))
-
-
 def is_hevc(key):
     key = key.lower()
     if "h265" in key or "x265" in key or "hevc" in key:
         return True
     else:
         return False
 
@@ -548,15 +543,15 @@
 def simplified_search_term_in_title(search_term, release_title, no_numbers=False):
     if no_numbers:
         match_regex = r'[^a-zA-Z\s\-\.]'
     else:
         match_regex = r'[^a-zA-Z0-9\s\-\.]'
 
     def unify(string):
-        return string.lower().replace("ß", "ss").replace("ä", "ae").replace("ö", "oe").replace(
+        return string.lower().replace(" (", "(").replace("ß", "ss").replace("ä", "ae").replace("ö", "oe").replace(
             "ü", "ue").replace(". ", " ").replace("+", ".").replace(" ", ".").replace("-.", "").strip()
 
     search_term = re.sub(match_regex, '', unify(search_term))
     release_title = re.sub(match_regex, '', unify(release_title))
 
     return search_term in release_title
```

### Comparing `feedcrawler-18.0.2/feedcrawler/providers/config.py` & `feedcrawler-18.0.3/feedcrawler/providers/config.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.2/feedcrawler/providers/gui.py` & `feedcrawler-18.0.3/feedcrawler/providers/gui.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.2/feedcrawler/providers/http_requests/cache_handler.py` & `feedcrawler-18.0.3/feedcrawler/providers/http_requests/cache_handler.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.2/feedcrawler/providers/http_requests/cloudflare_handlers.py` & `feedcrawler-18.0.3/feedcrawler/providers/http_requests/cloudflare_handlers.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.2/feedcrawler/providers/http_requests/request_handler.py` & `feedcrawler-18.0.3/feedcrawler/providers/http_requests/request_handler.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.2/feedcrawler/providers/myjd_connection.py` & `feedcrawler-18.0.3/feedcrawler/providers/myjd_connection.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,20 +5,19 @@
 
 import re
 import time
 
 from bs4 import BeautifulSoup
 
 import feedcrawler.external_tools.myjd_api
-from feedcrawler.external_tools.myjd_api import TokenExpiredException, RequestTimeoutException, MYJDException
+from feedcrawler.external_tools.myjd_api import TokenExpiredException, RequestTimeoutException, MYJDException, Jddevice
 from feedcrawler.providers import gui
 from feedcrawler.providers import shared_state
 from feedcrawler.providers.common_functions import check_hoster
 from feedcrawler.providers.common_functions import check_is_site
-from feedcrawler.providers.common_functions import is_device
 from feedcrawler.providers.common_functions import is_show
 from feedcrawler.providers.common_functions import longest_substr
 from feedcrawler.providers.common_functions import readable_size
 from feedcrawler.providers.common_functions import readable_time
 from feedcrawler.providers.common_functions import simplified_search_term_in_title
 from feedcrawler.providers.config import CrawlerConfig
 from feedcrawler.providers.sqlite_database import FeedDb
@@ -53,15 +52,15 @@
     try:
         jd.connect(myjd_user, myjd_pass)
         jd.update_devices()
         device = jd.get_device(myjd_device)
     except (TokenExpiredException, RequestTimeoutException, MYJDException) as e:
         print("Fehler bei der Verbindung mit My JDownloader: " + str(e))
         return False
-    if not device or not is_device(device):
+    if not device or not isinstance(device, (type, Jddevice)):
         return False
     else:
         shared_state.set_device(device)
         return True
 
 
 def set_device_from_config():
@@ -77,29 +76,29 @@
         try:
             jd.connect(myjd_user, myjd_pass)
             jd.update_devices()
             device = jd.get_device(myjd_device)
         except (TokenExpiredException, RequestTimeoutException, MYJDException) as e:
             print("Fehler bei der Verbindung mit My JDownloader: " + str(e).replace("\n", " "))
             return False
-        if not device or not is_device(device):
+        if not device or not isinstance(device, (type, Jddevice)):
             return False
         else:
             shared_state.set_device(device)
             return True
     elif myjd_user and myjd_pass:
         myjd_device = get_if_one_device(myjd_user, myjd_pass)
         try:
             jd.connect(myjd_user, myjd_pass)
             jd.update_devices()
             device = jd.get_device(myjd_device)
         except (TokenExpiredException, RequestTimeoutException, MYJDException) as e:
             print("Fehler bei der Verbindung mit My JDownloader: " + str(e).replace("\n", " "))
             return False
-        if not device or not is_device(device):
+        if not device or not isinstance(device, (type, Jddevice)):
             return False
         else:
             shared_state.set_device(device)
             return True
     else:
         return False
 
@@ -130,17 +129,17 @@
         return devices
     except (TokenExpiredException, RequestTimeoutException, MYJDException) as e:
         print("Fehler bei der Verbindung mit My JDownloader: " + str(e))
         return []
 
 
 def get_packages_in_downloader():
-    links = shared_state.values["device"].downloads.query_links()
+    links = shared_state.get_device().downloads.query_links()
 
-    packages = shared_state.values["device"].downloads.query_packages([{
+    packages = shared_state.get_device().downloads.query_packages([{
         "bytesLoaded": True,
         "bytesTotal": True,
         "comment": False,
         "enabled": True,
         "eta": True,
         "priority": False,
         "finished": True,
@@ -162,17 +161,17 @@
 
         return [failed, offline, decrypted]
     else:
         return [False, False, False]
 
 
 def get_packages_in_linkgrabber():
-    links = shared_state.values["device"].linkgrabber.query_links()
+    links = shared_state.get_device().linkgrabber.query_links()
 
-    packages = shared_state.values["device"].linkgrabber.query_packages(params=[
+    packages = shared_state.get_device().linkgrabber.query_packages(params=[
         {
             "bytesLoaded": True,
             "bytesTotal": True,
             "comment": True,
             "enabled": True,
             "eta": True,
             "priority": False,
@@ -329,26 +328,26 @@
     if not decrypted:
         decrypted = False
     return [failed, offline, decrypted]
 
 
 def get_state():
     try:
-        if not shared_state.values["device"] or not is_device(shared_state.values["device"]):
+        if not shared_state.get_device():
             set_device_from_config()
-        if shared_state.values["device"]:
+        if shared_state.get_device():
             try:
-                downloader_state = shared_state.values["device"].downloadcontroller.get_current_state()
-                grabber_collecting = shared_state.values["device"].linkgrabber.is_collecting()
+                downloader_state = shared_state.get_device().downloadcontroller.get_current_state()
+                grabber_collecting = shared_state.get_device().linkgrabber.is_collecting()
             except (TokenExpiredException, RequestTimeoutException, MYJDException):
                 set_device_from_config()
-                if not shared_state.values["device"] or not is_device(shared_state.values["device"]):
+                if not shared_state.get_device():
                     return False
-                downloader_state = shared_state.values["device"].downloadcontroller.get_current_state()
-                grabber_collecting = shared_state.values["device"].linkgrabber.is_collecting()
+                downloader_state = shared_state.get_device().downloadcontroller.get_current_state()
+                grabber_collecting = shared_state.get_device().linkgrabber.is_collecting()
             return [True, downloader_state, grabber_collecting]
         else:
             return False
     except (TokenExpiredException, RequestTimeoutException, MYJDException) as e:
         print("Fehler bei der Verbindung mit My JDownloader: " + str(e))
         return False
 
@@ -377,40 +376,40 @@
 
         resorted_failed_package.append(pk)
     return resorted_failed_package
 
 
 def get_info():
     try:
-        if not shared_state.values["device"] or not is_device(shared_state.values["device"]):
+        if not shared_state.get_device():
             set_device_from_config()
-        if shared_state.values["device"]:
+        if shared_state.get_device():
             try:
-                downloader_state = shared_state.values["device"].downloadcontroller.get_current_state()
-                grabber_collecting = shared_state.values["device"].linkgrabber.is_collecting()
-                shared_state.values["device"].update.run_update_check()
-                update_ready = shared_state.values["device"].update.is_update_available()
+                downloader_state = shared_state.get_device().downloadcontroller.get_current_state()
+                grabber_collecting = shared_state.get_device().linkgrabber.is_collecting()
+                shared_state.get_device().update.run_update_check()
+                update_ready = shared_state.get_device().update.is_update_available()
 
                 packages_in_downloader = get_packages_in_downloader()
                 packages_in_downloader_failed = packages_in_downloader[0]
                 packages_in_downloader_offline = packages_in_downloader[1]
                 packages_in_downloader_decrypted = packages_in_downloader[2]
 
                 packages_in_linkgrabber = get_packages_in_linkgrabber()
                 packages_in_linkgrabber_failed = packages_in_linkgrabber[0]
                 packages_in_linkgrabber_offline = packages_in_linkgrabber[1]
                 packages_in_linkgrabber_decrypted = packages_in_linkgrabber[2]
             except (TokenExpiredException, RequestTimeoutException, MYJDException):
                 set_device_from_config()
-                if not shared_state.values["device"] or not is_device(shared_state.values["device"]):
+                if not shared_state.get_device():
                     return False
-                downloader_state = shared_state.values["device"].downloadcontroller.get_current_state()
-                grabber_collecting = shared_state.values["device"].linkgrabber.is_collecting()
-                shared_state.values["device"].update.run_update_check()
-                update_ready = shared_state.values["device"].update.is_update_available()
+                downloader_state = shared_state.get_device().downloadcontroller.get_current_state()
+                grabber_collecting = shared_state.get_device().linkgrabber.is_collecting()
+                shared_state.get_device().update.run_update_check()
+                update_ready = shared_state.get_device().update.is_update_available()
 
                 packages_in_downloader = get_packages_in_downloader()
                 packages_in_downloader_failed = packages_in_downloader[0]
                 packages_in_downloader_offline = packages_in_downloader[1]
                 packages_in_downloader_decrypted = packages_in_downloader[2]
 
                 packages_in_linkgrabber = get_packages_in_linkgrabber()
@@ -446,146 +445,146 @@
     except (TokenExpiredException, RequestTimeoutException, MYJDException) as e:
         print("Fehler bei der Verbindung mit My JDownloader: " + str(e))
         return False
 
 
 def set_enabled(enable, linkids, uuid):
     try:
-        if not shared_state.values["device"] or not is_device(shared_state.values["device"]):
+        if not shared_state.get_device():
             set_device_from_config()
-        if shared_state.values["device"]:
+        if shared_state.get_device():
             try:
-                shared_state.values["device"].downloads.set_enabled(enable, linkids, uuid)
+                shared_state.get_device().downloads.set_enabled(enable, linkids, uuid)
             except (TokenExpiredException, RequestTimeoutException, MYJDException):
                 set_device_from_config()
-                if not shared_state.values["device"] or not is_device(shared_state.values["device"]):
+                if not shared_state.get_device():
                     return False
-                shared_state.values["device"].downloads.set_enabled(enable, linkids, uuid)
+                shared_state.get_device().downloads.set_enabled(enable, linkids, uuid)
             try:
-                shared_state.values["device"].linkgrabber.set_enabled(enable, linkids, uuid)
+                shared_state.get_device().linkgrabber.set_enabled(enable, linkids, uuid)
             except (TokenExpiredException, RequestTimeoutException, MYJDException):
                 set_device_from_config()
-                if not shared_state.values["device"] or not is_device(shared_state.values["device"]):
+                if not shared_state.get_device():
                     return False
-                shared_state.values["device"].linkgrabber.set_enabled(enable, linkids, uuid)
+                shared_state.get_device().linkgrabber.set_enabled(enable, linkids, uuid)
             return True
         else:
             return False
     except (TokenExpiredException, RequestTimeoutException, MYJDException) as e:
         print("Fehler bei der Verbindung mit My JDownloader: " + str(e))
         return False
 
 
 def move_to_downloads(linkids, uuid):
     try:
-        if not shared_state.values["device"] or not is_device(shared_state.values["device"]):
+        if not shared_state.get_device():
             set_device_from_config()
-        if shared_state.values["device"]:
+        if shared_state.get_device():
             try:
-                shared_state.values["device"].linkgrabber.move_to_downloadlist(linkids, uuid)
+                shared_state.get_device().linkgrabber.move_to_downloadlist(linkids, uuid)
             except (TokenExpiredException, RequestTimeoutException, MYJDException):
                 set_device_from_config()
-                if not shared_state.values["device"] or not is_device(shared_state.values["device"]):
+                if not shared_state.get_device():
                     return False
-                shared_state.values["device"].linkgrabber.move_to_downloadlist(linkids, uuid)
+                shared_state.get_device().linkgrabber.move_to_downloadlist(linkids, uuid)
             return True
         else:
             return False
     except (TokenExpiredException, RequestTimeoutException, MYJDException) as e:
         print("Fehler bei der Verbindung mit My JDownloader: " + str(e))
         return False
 
 
 def reset_in_downloads(linkids, uuid):
     try:
-        if not shared_state.values["device"] or not is_device(shared_state.values["device"]):
+        if not shared_state.get_device():
             set_device_from_config()
-        if shared_state.values["device"]:
+        if shared_state.get_device():
             try:
-                shared_state.values["device"].downloads.reset_links(linkids, uuid)
+                shared_state.get_device().downloads.reset_links(linkids, uuid)
             except (TokenExpiredException, RequestTimeoutException, MYJDException):
                 set_device_from_config()
-                if not shared_state.values["device"] or not is_device(shared_state.values["device"]):
+                if not shared_state.get_device():
                     return False
-                shared_state.values["device"].downloads.reset_links(linkids, uuid)
+                shared_state.get_device().downloads.reset_links(linkids, uuid)
             return True
         else:
             return False
     except (TokenExpiredException, RequestTimeoutException, MYJDException) as e:
         print("Fehler bei der Verbindung mit My JDownloader: " + str(e))
         return False
 
 
 def remove_from_linkgrabber(linkids, uuid):
     try:
-        if not shared_state.values["device"] or not is_device(shared_state.values["device"]):
+        if not shared_state.get_device():
             set_device_from_config()
-        if shared_state.values["device"]:
+        if shared_state.get_device():
             try:
-                shared_state.values["device"].linkgrabber.remove_links(linkids, uuid)
-                shared_state.values["device"].downloads.remove_links(linkids, uuid)
+                shared_state.get_device().linkgrabber.remove_links(linkids, uuid)
+                shared_state.get_device().downloads.remove_links(linkids, uuid)
             except (TokenExpiredException, RequestTimeoutException, MYJDException):
                 set_device_from_config()
-                if not shared_state.values["device"] or not is_device(shared_state.values["device"]):
+                if not shared_state.get_device():
                     return False
-                shared_state.values["device"].linkgrabber.remove_links(linkids, uuid)
-                shared_state.values["device"].downloads.remove_links(linkids, uuid)
+                shared_state.get_device().linkgrabber.remove_links(linkids, uuid)
+                shared_state.get_device().downloads.remove_links(linkids, uuid)
             return True
         else:
             return False
     except (TokenExpiredException, RequestTimeoutException, MYJDException) as e:
         print("Fehler bei der Verbindung mit My JDownloader: " + str(e))
         return False
 
 
 def rename_package_in_linkgrabber(package_id, new_name):
     try:
-        if not shared_state.values["device"] or not is_device(shared_state.values["device"]):
+        if not shared_state.get_device():
             set_device_from_config()
-        if shared_state.values["device"]:
+        if shared_state.get_device():
             try:
-                shared_state.values["device"].linkgrabber.rename_package(package_id, new_name)
+                shared_state.get_device().linkgrabber.rename_package(package_id, new_name)
             except (TokenExpiredException, RequestTimeoutException, MYJDException):
                 set_device_from_config()
-                if not shared_state.values["device"] or not is_device(shared_state.values["device"]):
+                if not shared_state.get_device():
                     return False
-                shared_state.values["device"].linkgrabber.rename_package(package_id, new_name)
+                shared_state.get_device().linkgrabber.rename_package(package_id, new_name)
             return True
         else:
             return False
     except (TokenExpiredException, RequestTimeoutException, MYJDException) as e:
         print("Fehler bei der Verbindung mit My JDownloader: " + str(e))
         return False
 
 
 def move_to_new_package(linkids, package_id, new_title, new_path):
     try:
-        if not shared_state.values["device"] or not is_device(shared_state.values["device"]):
+        if not shared_state.get_device():
             set_device_from_config()
-        if shared_state.values["device"]:
+        if shared_state.get_device():
             try:
-                shared_state.values["device"].linkgrabber.move_to_new_package(linkids, package_id, new_title, new_path)
-                shared_state.values["device"].downloads.move_to_new_package(linkids, package_id, new_title, new_path)
+                shared_state.get_device().linkgrabber.move_to_new_package(linkids, package_id, new_title, new_path)
+                shared_state.get_device().downloads.move_to_new_package(linkids, package_id, new_title, new_path)
             except (TokenExpiredException, RequestTimeoutException, MYJDException):
                 set_device_from_config()
-                if not shared_state.values["device"] or not is_device(shared_state.values["device"]):
+                if not shared_state.get_device():
                     return False
-                shared_state.values["device"].linkgrabber.move_to_new_package(linkids, package_id, new_title, new_path)
-                shared_state.values["device"].downloads.move_to_new_package(linkids, package_id, new_title, new_path)
+                shared_state.get_device().linkgrabber.move_to_new_package(linkids, package_id, new_title, new_path)
+                shared_state.get_device().downloads.move_to_new_package(linkids, package_id, new_title, new_path)
             return True
         else:
             return False
     except (TokenExpiredException, RequestTimeoutException, MYJDException) as e:
         print("Fehler bei der Verbindung mit My JDownloader: " + str(e))
         return False
 
 
 def download(title, subdir, old_links, password, full_path=None, autostart=False):
     try:
-        if not shared_state.values["device"] or not is_device(shared_state.values["device"]):
+        if not shared_state.get_device():
             set_device_from_config()
 
         if isinstance(old_links, list):
             links = []
             for link in old_links:
                 if link not in links:
                     links.append(link)
@@ -611,31 +610,31 @@
                 path = subdir + "/<jd:packagename>"
             else:
                 path = "<jd:packagename>"
         if "Remux" in path:
             priority = "LOWER"
 
         try:
-            shared_state.values["device"].linkgrabber.add_links(params=[
+            shared_state.get_device().linkgrabber.add_links(params=[
                 {
                     "autostart": autostart,
                     "links": links,
                     "packageName": title,
                     "extractPassword": password,
                     "priority": priority,
                     "downloadPassword": password,
                     "destinationFolder": path,
                     "comment": "FeedCrawler by rix1337",
                     "overwritePackagizerRules": False
                 }])
         except (TokenExpiredException, RequestTimeoutException, MYJDException):
             set_device_from_config()
-            if not shared_state.values["device"] or not is_device(shared_state.values["device"]):
+            if not shared_state.get_device():
                 return False
-            shared_state.values["device"].linkgrabber.add_links(params=[
+            shared_state.get_device().linkgrabber.add_links(params=[
                 {
                     "autostart": autostart,
                     "links": links,
                     "packageName": title,
                     "extractPassword": password,
                     "priority": priority,
                     "downloadPassword": password,
@@ -653,19 +652,19 @@
     except (TokenExpiredException, RequestTimeoutException, MYJDException) as e:
         print("Fehler bei der Verbindung mit My JDownloader: " + str(e))
         return False
 
 
 def retry_decrypt(linkids, uuid, links):
     try:
-        if not shared_state.values["device"] or not is_device(shared_state.values["device"]):
+        if not shared_state.get_device():
             set_device_from_config()
-        if shared_state.values["device"]:
+        if shared_state.get_device():
             try:
-                package = shared_state.values["device"].linkgrabber.query_packages(params=[
+                package = shared_state.get_device().linkgrabber.query_packages(params=[
                     {
                         "availableOfflineCount": True,
                         "availableOnlineCount": True,
                         "availableTempUnknownCount": True,
                         "availableUnknownCount": True,
                         "bytesTotal": True,
                         "childCount": True,
@@ -677,17 +676,17 @@
                         "priority": True,
                         "saveTo": True,
                         "startAt": 0,
                         "status": True
                     }])
             except (TokenExpiredException, RequestTimeoutException, MYJDException):
                 set_device_from_config()
-                if not shared_state.values["device"] or not is_device(shared_state.values["device"]):
+                if not shared_state.get_device():
                     return False
-                package = shared_state.values["device"].linkgrabber.query_packages(params=[
+                package = shared_state.get_device().linkgrabber.query_packages(params=[
                     {
                         "availableOfflineCount": True,
                         "availableOnlineCount": True,
                         "availableTempUnknownCount": True,
                         "availableUnknownCount": True,
                         "bytesTotal": True,
                         "childCount": True,
@@ -699,15 +698,15 @@
                         "priority": True,
                         "saveTo": True,
                         "startAt": 0,
                         "status": True
                     }])
             if not package:
                 try:
-                    package = shared_state.values["device"].downloads.query_packages(params=[
+                    package = shared_state.get_device().downloads.query_packages(params=[
                         {
                             "bytesLoaded": True,
                             "bytesTotal": True,
                             "comment": True,
                             "enabled": True,
                             "eta": True,
                             "priority": True,
@@ -720,17 +719,17 @@
                             "saveTo": True,
                             "maxResults": -1,
                             "packageUUIDs": uuid,
                             "startAt": 0,
                         }])
                 except (TokenExpiredException, RequestTimeoutException, MYJDException):
                     set_device_from_config()
-                    if not shared_state.values["device"] or not is_device(shared_state.values["device"]):
+                    if not shared_state.get_device():
                         return False
-                    package = shared_state.values["device"].downloads.query_packages(params=[
+                    package = shared_state.get_device().downloads.query_packages(params=[
                         {
                             "bytesLoaded": True,
                             "bytesTotal": True,
                             "comment": True,
                             "enabled": True,
                             "eta": True,
                             "priority": True,
@@ -745,97 +744,97 @@
                             "packageUUIDs": uuid,
                             "startAt": 0,
                         }])
             if package:
                 remove_from_linkgrabber(linkids, uuid)
                 title = package[0].get('name')
                 full_path = package[0].get('saveTo')
-                download(title, None, links, None, full_path)
-                return True
+                if download(title, None, links, None, full_path):
+                    return True
             else:
                 return False
         else:
             return False
     except (TokenExpiredException, RequestTimeoutException, MYJDException) as e:
         print("Fehler bei der Verbindung mit My JDownloader: " + str(e))
         return False
 
 
 def jdownloader_update():
     try:
-        if not shared_state.values["device"] or not is_device(shared_state.values["device"]):
+        if not shared_state.get_device():
             set_device_from_config()
-        if shared_state.values["device"]:
+        if shared_state.get_device():
             try:
-                shared_state.values["device"].update.restart_and_update()
+                shared_state.get_device().update.restart_and_update()
             except feedcrawler.external_tools.myjd_api.TokenExpiredException:
                 set_device_from_config()
-                if not shared_state.values["device"] or not is_device(shared_state.values["device"]):
+                if not shared_state.get_device():
                     return False
-                shared_state.values["device"].update.restart_and_update()
+                shared_state.get_device().update.restart_and_update()
             return True
         else:
             return False
     except feedcrawler.external_tools.myjd_api.MYJDException as e:
         print("Fehler bei der Verbindung mit My JDownloader: " + str(e))
         return False
 
 
 def jdownloader_start():
     try:
-        if not shared_state.values["device"] or not is_device(shared_state.values["device"]):
+        if not shared_state.get_device():
             set_device_from_config()
-        if shared_state.values["device"]:
+        if shared_state.get_device():
             try:
-                shared_state.values["device"].downloadcontroller.start_downloads()
+                shared_state.get_device().downloadcontroller.start_downloads()
             except (TokenExpiredException, RequestTimeoutException, MYJDException):
                 set_device_from_config()
-                if not shared_state.values["device"] or not is_device(shared_state.values["device"]):
+                if not shared_state.get_device():
                     return False
-                shared_state.values["device"].downloadcontroller.start_downloads()
+                shared_state.get_device().downloadcontroller.start_downloads()
             return True
         else:
             return False
     except (TokenExpiredException, RequestTimeoutException, MYJDException) as e:
         print("Fehler bei der Verbindung mit My JDownloader: " + str(e))
         return False
 
 
 def jdownloader_pause(bl):
     try:
-        if not shared_state.values["device"] or not is_device(shared_state.values["device"]):
+        if not shared_state.get_device():
             set_device_from_config()
-        if shared_state.values["device"]:
+        if shared_state.get_device():
             try:
-                shared_state.values["device"].downloadcontroller.pause_downloads(bl)
+                shared_state.get_device().downloadcontroller.pause_downloads(bl)
             except (TokenExpiredException, RequestTimeoutException, MYJDException):
                 set_device_from_config()
-                if not shared_state.values["device"] or not is_device(shared_state.values["device"]):
+                if not shared_state.get_device():
                     return False
-                shared_state.values["device"].downloadcontroller.pause_downloads(bl)
+                shared_state.get_device().downloadcontroller.pause_downloads(bl)
             return True
         else:
             return False
     except (TokenExpiredException, RequestTimeoutException, MYJDException) as e:
         print("Fehler bei der Verbindung mit My JDownloader: " + str(e))
         return False
 
 
 def jdownloader_stop():
     try:
-        if not shared_state.values["device"] or not is_device(shared_state.values["device"]):
+        if not shared_state.get_device():
             set_device_from_config()
-        if shared_state.values["device"]:
+        if shared_state.get_device():
             try:
-                shared_state.values["device"].downloadcontroller.stop_downloads()
+                shared_state.get_device().downloadcontroller.stop_downloads()
             except (TokenExpiredException, RequestTimeoutException, MYJDException):
                 set_device_from_config()
-                if not shared_state.values["device"] or not is_device(shared_state.values["device"]):
+                if not shared_state.get_device():
                     return False
-                shared_state.values["device"].downloadcontroller.stop_downloads()
+                shared_state.get_device().downloadcontroller.stop_downloads()
             return True
         else:
             return False
     except (TokenExpiredException, RequestTimeoutException, MYJDException) as e:
         print("Fehler bei der Verbindung mit My JDownloader: " + str(e))
         return False
 
@@ -852,15 +851,15 @@
                 for url in package['urls']:
                     if link == url or url in link or link in url:
                         return [failed[0], package['linkids'], package['uuid'], package['name'], package['path']]
     return False
 
 
 def myjd_download(title, subdir, links, password):
-    if shared_state.values["device"]:
+    if shared_state.get_device():
         is_episode = re.findall(r'[\w.\s]*S\d{1,2}(E\d{1,2})[\w.\s]*', title)
         if is_episode:
             exists = check_failed_link_exists(links)
             if exists:
                 broken_title = False
                 old_title = exists[3]
                 old_path = exists[4]
@@ -878,21 +877,20 @@
 
                 if not broken_title:
                     linkids = exists[1]
                     package_id = [exists[2]]
                     new_title = title.replace(new_episode, combined_episodes)
                     new_path = old_path.replace(old_title, new_title)
 
-                    shared_state.values["device"] = move_to_new_package(linkids, package_id, new_title, new_path)
-                    FeedDb('crawldog').store(new_title, 'added')
-                    FeedDb('crawldog').delete(old_title)
-                    return True
+                    if move_to_new_package(linkids, package_id, new_title, new_path):
+                        FeedDb('crawldog').store(new_title, 'added')
+                        FeedDb('crawldog').delete(old_title)
+                        return True
 
-        shared_state.values["device"] = download(title, subdir, links, password)
-        if shared_state.values["device"]:
+        if download(title, subdir, links, password):
             return True
     return False
 
 
 def remove_unfit_links(decrypted_packages, known_packages, keep_linkids, keep_uuids, delete_linkids,
                        delete_uuids, delete_packages, title):
     title = title.replace(" ", ".")
@@ -1019,22 +1017,22 @@
     mergable.append([mergable_titles, mergable_uuids, mergable_linkids])
     mergable.sort()
     return mergable
 
 
 def do_package_merge(title, uuids, linkids):
     try:
-        if not shared_state.values["device"] or not is_device(shared_state.values["device"]):
+        if not shared_state.get_device():
             set_device_from_config()
-        if shared_state.values["device"]:
+        if shared_state.get_device():
             try:
                 move_to_new_package(linkids, uuids, title, "<jd:packagename>")
             except (TokenExpiredException, RequestTimeoutException, MYJDException):
                 set_device_from_config()
-                if not shared_state.values["device"] or not is_device(shared_state.values["device"]):
+                if not shared_state.get_device():
                     return False
                 move_to_new_package(linkids, uuids, title, "<jd:packagename>")
             return True
         else:
             return False
     except (TokenExpiredException, RequestTimeoutException, MYJDException) as e:
         print("Fehler bei der Verbindung mit My JDownloader: " + str(e))
```

### Comparing `feedcrawler-18.0.2/feedcrawler/providers/notifications.py` & `feedcrawler-18.0.3/feedcrawler/providers/notifications.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.2/feedcrawler/providers/sqlite_database.py` & `feedcrawler-18.0.3/feedcrawler/providers/sqlite_database.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.2/feedcrawler/providers/url_functions.py` & `feedcrawler-18.0.3/feedcrawler/providers/url_functions.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.2/feedcrawler/providers/version.py` & `feedcrawler-18.0.3/feedcrawler/providers/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import re
 from distutils.version import StrictVersion
 from urllib.request import urlopen
 
 
 def get_version():
-    return "18.0.2"
+    return "18.0.3"
 
 
 def create_version_file():
     version = get_version()
     version_clean = re.sub('[^\d\.]', '', version)
     if "a" in version:
         suffix = version.split("a")[1]
```

### Comparing `feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/@formkit-18209bb1.js` & `feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/@formkit-18209bb1.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/@popperjs-9847b28c.js` & `feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/@popperjs-9847b28c.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/@vue-d42f3502.js` & `feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/@vue-d42f3502.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/@vueuse-8ce5afe9.js` & `feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/@vueuse-8ce5afe9.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/axios-707ed124.js` & `feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/axios-707ed124.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-163e1b4f.js` & `feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-163e1b4f.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-48fa63fb.css` & `feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-48fa63fb.css`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-999550fa.woff` & `feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-999550fa.woff`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-cfe45b98.woff2` & `feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-cfe45b98.woff2`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-f7e350bb.css` & `feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-f7e350bb.css`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/index-137a91df.css` & `feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/index-137a91df.css`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/index-67e298b0.js` & `feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/index-44ade789.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1787,15 +1787,15 @@
                         "messages-class": "text-danger",
                         placeholder: "Film- oder Serien-Titel eingeben",
                         type: "text",
                         validation: "required|length:3"
                     }, null, 8, ["modelValue"])]),
                     _: 1
                 })])), [
-                    [R, "Bequeme Suchfunktion für " + s(t).state.hostnames.search + ". Bei hellblau hinterlegten Serien werden alle verfügbaren Staffeln/Episoden hinzugefügt. Komplette Serien landen auch in der Suchliste. Alternativ kann eine einzelne Staffel/Episode per Komma am Titel ergänzt werden: 'Serien Titel,S01' oder 'Serien Titel,S01E01'. Die für die Feed-Suche gesetzte Auflösung und Filterliste werden berücksichtigt, aber nicht forciert. Bereits geladene Releases werden hier nicht ignoriert!"]
+                    [R, "Bequeme Suchfunktion für " + s(t).state.hostnames.search + ". Bei hellblau hinterlegten Serien werden alle verfügbaren Staffeln/Folgen hinzugefügt. Komplette Serien landen auch in der Suchliste. Alternativ kann eine einzelne Staffel/Folge per Komma am Titel ergänzt werden: 'Serien Titel,S01' oder 'Serien Titel,S01E01'. Die für die Feed-Suche gesetzte Auflösung und Filterliste werden berücksichtigt, aber nicht forciert. Bereits geladene Releases werden hier nicht ignoriert!"]
                 ]), e("div", jn, [e("div", Hn, [h(e("input", {
                     class: "form-check-input",
                     type: "checkbox",
                     id: "flexSwitchMovies",
                     "onUpdate:modelValue": w[3] || (w[3] = P => f.value = P)
                 }, null, 512), [
                     [ke, f.value]
@@ -1850,15 +1850,15 @@
     io = e("div", {
         class: "offcanvas-header"
     }, [e("h3", {
         id: "offcanvasBottomListsLabel",
         class: "offcanvas-title"
     }, [e("i", {
         class: "bi bi-text-left"
-    }), r(" Suchlisten")]), e("button", {
+    }), r(" Suchlisten ")]), e("button", {
         "aria-label": "Close",
         class: "btn-close text-reset",
         "data-bs-dismiss": "offcanvas",
         type: "button"
     })], -1),
     ro = {
         class: "offcanvas-body"
@@ -2080,38 +2080,38 @@
                     "incomplete-message": "Es müssen alle Felder korrekt ausgefüllt werden! Fehler sind rot markiert.",
                     "messages-class": "text-danger",
                     type: "form",
                     onSubmit: V[10] || (V[10] = o => _())
                 }, {
                     default: M(({
                         value: o
-                    }) => [s(t).state.misc.loaded_lists ? i("", !0) : (l(), a("h4", co, "Suchlisten werden geladen...")), s(t).state.misc.loaded_lists ? (l(), a("div", uo, [s(t).state.hostnames.bl !== "Nicht gesetzt!" ? (l(), a("div", ho, [e("h2", mo, [e("button", go, p(s(t).state.hostnames.bl), 1)]), e("div", po, [e("div", bo, [h((l(), a("div", null, [u(y, {
+                    }) => [s(t).state.misc.loaded_lists ? i("", !0) : (l(), a("h4", co, "Suchlisten werden geladen...")), s(t).state.misc.loaded_lists ? (l(), a("div", uo, [s(t).state.hostnames.bl !== "Nicht gesetzt!" ? (l(), a("div", ho, [e("h2", mo, [e("button", go, " Filme (" + p(s(t).state.hostnames.bl) + ") ", 1)]), e("div", po, [e("div", bo, [h((l(), a("div", null, [u(y, {
                         modelValue: s(t).state.lists.mb.filme,
                         "onUpdate:modelValue": V[0] || (V[0] = d => s(t).state.lists.mb.filme = d),
                         validation: [
                             ["?matches", /^[a-zA-Z0-9ÄäÖöÜüß\-+&\s]+$/]
                         ],
                         "validation-messages": {
                             matches: "Bitte nur Buchstaben, Zahlen, Leerzeichen oder folgende Sonderzeichen eingeben: - + &"
                         },
                         class: "liste form-control bg-light mb-4",
                         "help-class": "text-muted",
                         "input-class": "liste form-control bg-light mb-4",
-                        label: "Filme",
+                        label: "Reguläre Suche",
                         "messages-class": "text-danger",
                         placeholder: "Bspw. Film-Titel",
                         rows: "10",
                         type: "textarea",
                         "validation-visibility": "live"
                     }, null, 8, ["modelValue"])])), [
                         [B, "Pro Zeile ein Film-Titel"]
-                    ]), s(t).state.settings.mb.regex ? h((l(), a("div", _o, [e("h5", null, [r("Filme/Serien "), h((l(), a("span", {
+                    ]), s(t).state.settings.mb.regex ? h((l(), a("div", _o, [e("h5", null, [h((l(), a("span", {
                         class: "link-primary",
                         onClick: L
-                    }, [r("(RegEx)")])), [
+                    }, [r("RegEx-Suche")])), [
                         [B, "Hilfe zu RegEx öffnen"]
                     ])]), u(y, {
                         modelValue: s(t).state.lists.mb.regex,
                         "onUpdate:modelValue": V[1] || (V[1] = d => s(t).state.lists.mb.regex = d),
                         validation: [
                             ["?matches", /^[a-zA-Z0-9ÄäÖöÜüß\-\s.*+()|\[\]?!]+$/]
                         ],
@@ -2123,59 +2123,59 @@
                         "input-class": "liste form-control bg-light mb-4",
                         "messages-class": "text-danger",
                         placeholder: "Bspw. Film.*.Titel.*",
                         rows: "10",
                         type: "textarea",
                         "validation-visibility": "live"
                     }, null, 8, ["modelValue", "validation", "validation-messages"])])), [
-                        [B, "Pro Zeile ein Film-/Serien-Titel im RegEx-Format - Die Filterliste wird hier ignoriert."]
+                        [B, "Pro Zeile ein Film-/Serien-Titel im RegEx-Format (Filterliste wird hier ignoriert)"]
                     ]) : i("", !0), s(t).state.settings.mbsj.enabled && s(t).state.hostnames.s === "Nicht gesetzt!" ? h((l(), a("div", fo, [u(y, {
                         modelValue: s(t).state.lists.mbsj.staffeln,
                         "onUpdate:modelValue": V[2] || (V[2] = d => s(t).state.lists.mbsj.staffeln = d),
                         validation: [
                             ["?matches", /^[a-zA-Z0-9ÄäÖöÜüß\-+&\s]+$/]
                         ],
                         "validation-messages": {
                             matches: "Bitte nur Buchstaben, Zahlen, Leerzeichen oder folgende Sonderzeichen eingeben: - + &"
                         },
                         class: "liste form-control bg-light mb-4",
                         "help-class": "text-muted",
                         "input-class": "liste form-control bg-light mb-4",
-                        label: "Staffeln",
+                        label: "Reguläre Suche",
                         "messages-class": "text-danger",
                         placeholder: "Bspw. Serien-Titel",
                         rows: "10",
                         type: "textarea",
                         "validation-visibility": "live"
                     }, null, 8, ["modelValue"])])), [
-                        [B, "Pro Zeile ein Serien-Titel für ganze Staffeln."]
-                    ]) : i("", !0)])])])) : i("", !0), s(t).state.hostnames.s !== "Nicht gesetzt!" ? (l(), a("div", vo, [e("h2", ko, [e("button", yo, p(s(t).state.hostnames.s), 1)]), e("div", wo, [e("div", $o, [h((l(), a("div", null, [u(y, {
+                        [B, "Pro Zeile ein Serien-Titel (gesucht werden vollständige Staffeln)"]
+                    ]) : i("", !0)])])])) : i("", !0), s(t).state.hostnames.s !== "Nicht gesetzt!" ? (l(), a("div", vo, [e("h2", ko, [e("button", yo, " Folgen (" + p(s(t).state.hostnames.s) + ") ", 1)]), e("div", wo, [e("div", $o, [h((l(), a("div", null, [u(y, {
                         modelValue: s(t).state.lists.sj.serien,
                         "onUpdate:modelValue": V[3] || (V[3] = d => s(t).state.lists.sj.serien = d),
                         validation: [
                             ["?matches", /^[a-zA-Z0-9ÄäÖöÜüß\-+&\s]+$/]
                         ],
                         "validation-messages": {
                             matches: "Bitte nur Buchstaben, Zahlen, Leerzeichen oder folgende Sonderzeichen eingeben: - + &"
                         },
                         class: "liste form-control bg-light mb-4",
                         "help-class": "text-muted",
                         "input-class": "liste form-control bg-light mb-4",
-                        label: "Serien",
+                        label: "Reguläre Suche",
                         "messages-class": "text-danger",
                         placeholder: "Bspw. Serien-Titel",
                         rows: "10",
                         type: "textarea",
                         "validation-visibility": "live"
                     }, null, 8, ["modelValue"])])), [
-                        [B, "Pro Zeile ein Serien-Titel für Episoden."]
-                    ]), s(t).state.settings.sj.regex ? h((l(), a("div", xo, [e("h5", null, [r("Serien "), h((l(), a("span", {
+                        [B, "Pro Zeile ein Serien-Titel (gesucht werden Folgen)"]
+                    ]), s(t).state.settings.sj.regex ? h((l(), a("div", xo, [e("h5", null, [h((l(), a("span", {
                         class: "link-primary",
                         onClick: L
-                    }, [r("(RegEx)")])), [
+                    }, [r("RegEx-Suche")])), [
                         [B, "Hilfe zu RegEx öffnen"]
                     ])]), u(y, {
                         modelValue: s(t).state.lists.sj.regex,
                         "onUpdate:modelValue": V[4] || (V[4] = d => s(t).state.lists.sj.regex = d),
                         validation: [
                             ["?matches", /^[a-zA-Z0-9ÄäÖöÜüß\-\s.*+()|\[\]?!]+$/]
                         ],
@@ -2187,19 +2187,19 @@
                         "input-class": "liste form-control bg-light mb-4",
                         "messages-class": "text-danger",
                         placeholder: "Bspw. Serien.*.Titel.*",
                         rows: "10",
                         type: "textarea",
                         "validation-visibility": "live"
                     }, null, 8, ["modelValue", "validation", "validation-messages"])])), [
-                        [B, "Pro Zeile ein Serien-Titel im RegEx-Format - Die Filterliste wird hier ignoriert."]
-                    ]) : i("", !0), s(t).state.lists.sj.staffeln_regex ? h((l(), a("div", So, [e("h5", null, [r("Staffeln "), h((l(), a("span", {
+                        [B, "Pro Zeile ein Serien-Titel im RegEx-Format (Filterliste wird hier ignoriert)"]
+                    ]) : i("", !0), s(t).state.lists.sj.staffeln_regex ? h((l(), a("div", So, [e("h5", null, [h((l(), a("span", {
                         class: "link-primary",
                         onClick: L
-                    }, [r("(RegEx)")])), [
+                    }, [r("RegEx-Suche")])), [
                         [B, "Hilfe zu RegEx öffnen"]
                     ])]), s(t).state.lists.sj.staffeln_regex ? (l(), He(y, {
                         key: 0,
                         validation: [
                             ["?matches", /^[a-zA-Z0-9ÄäÖöÜüß\-\s.*+()|\[\]?!]+$/]
                         ],
                         "validation-messages": {
@@ -2210,79 +2210,79 @@
                         "input-class": "liste form-control bg-light mb-4",
                         "messages-class": "text-danger",
                         placeholder: "Bspw. Serien.*.Titel.*",
                         rows: "10",
                         type: "textarea",
                         "validation-visibility": "live"
                     }, null, 8, ["validation", "validation-messages"])) : i("", !0)])), [
-                        [B, "Pro Zeile ein Serien-Titel im RegEx-Format für Staffeln - Die Filterliste wird hier ignoriert."]
+                        [B, "Pro Zeile ein Serien-Titel im RegEx-Format für Staffeln (Filterliste wird hier ignoriert)"]
                     ]) : i("", !0), s(t).state.settings.mbsj.enabled && s(t).state.hostnames.bl === "Nicht gesetzt!" ? h((l(), a("div", Vo, [u(y, {
                         modelValue: s(t).state.lists.mbsj.staffeln,
                         "onUpdate:modelValue": V[5] || (V[5] = d => s(t).state.lists.mbsj.staffeln = d),
                         validation: [
                             ["?matches", /^[a-zA-Z0-9ÄäÖöÜüß\-+&\s]+$/]
                         ],
                         "validation-messages": {
                             matches: "Bitte nur Buchstaben, Zahlen, Leerzeichen oder folgende Sonderzeichen eingeben: - + &"
                         },
                         class: "liste form-control bg-light mb-4",
                         "help-class": "text-muted",
                         "input-class": "liste form-control bg-light mb-4",
-                        label: "Staffeln",
+                        label: "Reguläre Suche",
                         "messages-class": "text-danger",
                         placeholder: "Bspw. Serien-Titel",
                         rows: "10",
                         type: "textarea",
                         "validation-visibility": "live"
                     }, null, 8, ["modelValue"])])), [
-                        [B, "Pro Zeile ein Serien-Titel für ganze Staffeln."]
-                    ]) : i("", !0)])])])) : i("", !0), s(t).state.hostnames.sjbl !== "Nicht gesetzt!" && s(t).state.settings.mbsj.enabled && s(t).state.misc.sjbl_enabled ? (l(), a("div", Co, [e("h2", Do, [e("button", zo, p(s(t).state.hostnames.sjbl), 1)]), e("div", Lo, [e("div", Bo, [h((l(), a("div", null, [u(y, {
+                        [B, "Pro Zeile ein Serien-Titel (gesucht werden vollständige Staffeln)"]
+                    ]) : i("", !0)])])])) : i("", !0), s(t).state.hostnames.sjbl !== "Nicht gesetzt!" && s(t).state.settings.mbsj.enabled && s(t).state.misc.sjbl_enabled ? (l(), a("div", Co, [e("h2", Do, [e("button", zo, " Staffeln (" + p(s(t).state.hostnames.sjbl) + ") ", 1)]), e("div", Lo, [e("div", Bo, [h((l(), a("div", null, [u(y, {
                         modelValue: s(t).state.lists.mbsj.staffeln,
                         "onUpdate:modelValue": V[6] || (V[6] = d => s(t).state.lists.mbsj.staffeln = d),
                         validation: [
                             ["?matches", /^[a-zA-Z0-9ÄäÖöÜüß\-+&\s]+$/]
                         ],
                         "validation-messages": {
                             matches: "Bitte nur Buchstaben, Zahlen, Leerzeichen oder folgende Sonderzeichen eingeben: - + &"
                         },
                         class: "liste form-control bg-light mb-4",
                         "help-class": "text-muted",
                         "input-class": "liste form-control bg-light mb-4",
-                        label: "Staffeln",
+                        label: "Reguläre Suche",
                         "messages-class": "text-danger",
                         placeholder: "Bspw. Serien-Titel",
                         rows: "10",
                         type: "textarea",
                         "validation-visibility": "live"
                     }, null, 8, ["modelValue"])])), [
-                        [B, "Pro Zeile ein Serien-Titel für ganze Staffeln."]
-                    ])])])])) : i("", !0), s(t).state.hostnames.dj !== "Nicht gesetzt!" ? (l(), a("div", jo, [e("h2", Ho, [e("button", Fo, p(s(t).state.hostnames.dj), 1)]), e("div", Ro, [e("div", Uo, [h((l(), a("div", null, [u(y, {
+                        [B, "Pro Zeile ein Serien-Titel (gesucht werden vollständige Staffeln)"]
+                    ])])])])) : i("", !0), s(t).state.hostnames.dj !== "Nicht gesetzt!" ? (l(), a("div", jo, [e("h2", Ho, [e("button", Fo, " Dokus (" + p(s(t).state.hostnames.dj) + ") ", 1)]), e("div", Ro, [e("div", Uo, [h((l(), a("div", null, [u(y, {
                         modelValue: s(t).state.lists.dj.dokus,
                         "onUpdate:modelValue": V[7] || (V[7] = d => s(t).state.lists.dj.dokus = d),
                         validation: [
                             ["?matches", /^[a-zA-Z0-9ÄäÖöÜüß\-+&\s]+$/]
                         ],
                         "validation-messages": {
                             matches: "Bitte nur Buchstaben, Zahlen, Leerzeichen oder folgende Sonderzeichen eingeben: - + &"
                         },
                         class: "liste form-control bg-light mb-4",
                         "help-class": "text-muted",
                         "input-class": "liste form-control bg-light mb-4",
-                        label: "Dokus",
+                        label: "Reguläre Suche",
                         "messages-class": "text-danger",
                         placeholder: "Bspw. Doku-Titel",
                         rows: "10",
                         type: "textarea",
                         "validation-visibility": "live"
                     }, null, 8, ["modelValue"])])), [
                         [B, "Pro Zeile ein Doku-Titel"]
-                    ]), s(t).state.settings.dj.regex ? h((l(), a("div", Po, [e("h5", null, [r("Dokus "), h((l(), a("span", {
+                    ]), s(t).state.settings.dj.regex ? h((l(), a("div", Po, [e("h5", null, [h((l(), a("span", {
                         class: "link-primary",
                         onClick: L
-                    }, [r("(RegEx)")])), [
+                    }, [r("RegEx-Suche")])), [
                         [B, "Hilfe zu RegEx öffnen"]
                     ])]), u(y, {
                         modelValue: s(t).state.lists.dj.regex,
                         "onUpdate:modelValue": V[8] || (V[8] = d => s(t).state.lists.dj.regex = d),
                         validation: [
                             ["?matches", /^[a-zA-Z0-9ÄäÖöÜüß\-\s.*+()|\[\]?!]+$/]
                         ],
@@ -2294,28 +2294,28 @@
                         "input-class": "liste form-control bg-light mb-4",
                         "messages-class": "text-danger",
                         placeholder: "Bspw. Doku.*.Titel.*",
                         rows: "10",
                         type: "textarea",
                         "validation-visibility": "live"
                     }, null, 8, ["modelValue", "validation", "validation-messages"])])), [
-                        [B, "Pro Zeile ein Doku-Titel im RegEx-Format - Die Filterliste wird hier ignoriert."]
-                    ]) : i("", !0)])])])) : i("", !0), s(t).state.hostnames.dd !== "Nicht gesetzt!" ? (l(), a("div", No, [e("h2", Eo, [e("button", To, p(s(t).state.hostnames.dd), 1)]), e("div", Ao, [e("div", Wo, [h((l(), a("div", null, [u(y, {
+                        [B, "Pro Zeile ein Doku-Titel im RegEx-Format (Filterliste wird hier ignoriert)"]
+                    ]) : i("", !0)])])])) : i("", !0), s(t).state.hostnames.dd !== "Nicht gesetzt!" ? (l(), a("div", No, [e("h2", Eo, [e("button", To, " Folgen (" + p(s(t).state.hostnames.dd) + ") ", 1)]), e("div", Ao, [e("div", Wo, [h((l(), a("div", null, [u(y, {
                         modelValue: s(t).state.lists.dd.feeds,
                         "onUpdate:modelValue": V[9] || (V[9] = d => s(t).state.lists.dd.feeds = d),
                         validation: [
                             ["?matches", /^[0-9\n]+$/]
                         ],
                         "validation-messages": {
                             matches: "Bitte nur Zahlen eingeben."
                         },
                         class: "liste form-control bg-light mb-4",
                         "help-class": "text-muted",
                         "input-class": "liste form-control bg-light mb-4",
-                        label: "Feed-IDs",
+                        label: "Reguläre Suche",
                         "messages-class": "text-danger",
                         placeholder: "Bspw. 12345",
                         rows: "10",
                         type: "textarea",
                         "validation-visibility": "live"
                     }, null, 8, ["modelValue", "validation-messages"])])), [
                         [B, "Pro Zeile eine numerische RSS-Feed-ID"]
```

### Comparing `feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/tippy-a1ae07b3.css` & `feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/tippy-a1ae07b3.css`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-router-4bccd9ac.js` & `feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-router-4bccd9ac.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-tippy-2fb47e86.js` & `feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-tippy-2fb47e86.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-toastification-2a2137d8.js` & `feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-toastification-2a2137d8.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-toastification-4522082c.css` & `feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-toastification-4522082c.css`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/vuejs-paginate-next-23a274fb.js` & `feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/vuejs-paginate-next-23a274fb.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/assets/vuex-c2e7db49.js` & `feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/vuex-c2e7db49.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/favicon.ico` & `feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/favicon.ico`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.2/feedcrawler/web_interface/vuejs_frontend/dist/index.html` & `feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/index.html`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 <head>
     <meta charset="UTF-8">
     <meta content="width=device-width, initial-scale=1, shrink-to-fit=no" name="viewport">
 
     <link href="./favicon.ico" rel="icon" type="image/x-icon">
 
     <title>FeedCrawler</title>
-  <script type="module" crossorigin src="./assets/index-67e298b0.js"></script>
+  <script type="module" crossorigin src="./assets/index-44ade789.js"></script>
   <link rel="modulepreload" crossorigin href="./assets/@vue-d42f3502.js">
   <link rel="modulepreload" crossorigin href="./assets/vuex-c2e7db49.js">
   <link rel="modulepreload" crossorigin href="./assets/axios-707ed124.js">
   <link rel="modulepreload" crossorigin href="./assets/vue-router-4bccd9ac.js">
   <link rel="modulepreload" crossorigin href="./assets/@popperjs-9847b28c.js">
   <link rel="modulepreload" crossorigin href="./assets/bootstrap-163e1b4f.js">
   <link rel="modulepreload" crossorigin href="./assets/vue-toastification-2a2137d8.js">
```

### Comparing `feedcrawler-18.0.2/feedcrawler/web_interface/web_server.py` & `feedcrawler-18.0.3/feedcrawler/web_interface/web_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,14 @@
 from feedcrawler.external_tools.plex_api import get_plex_headers
 from feedcrawler.providers import gui
 from feedcrawler.providers import version, shared_state
 from feedcrawler.providers.common_functions import Unbuffered
 from feedcrawler.providers.common_functions import check_is_site
 from feedcrawler.providers.common_functions import decode_base64
 from feedcrawler.providers.common_functions import get_to_decrypt
-from feedcrawler.providers.common_functions import is_device
 from feedcrawler.providers.common_functions import keep_alphanumeric_with_regex_characters
 from feedcrawler.providers.common_functions import keep_alphanumeric_with_special_characters
 from feedcrawler.providers.common_functions import keep_numbers
 from feedcrawler.providers.common_functions import remove_decrypt
 from feedcrawler.providers.common_functions import rreplace
 from feedcrawler.providers.config import CrawlerConfig
 from feedcrawler.providers.myjd_connection import set_device
@@ -901,28 +900,32 @@
     @auth_basic(is_authenticated_user)
     def download_movie(title):
         try:
             payload = feedcrawler.external_sites.web_search.content_all.get_best_result(title)
             if payload:
                 matches = feedcrawler.external_sites.web_search.content_all.download(payload)
                 return "Success: " + str(matches)
-        except:
+        except Exception as e:
+            shared_state.logger.debug("An exception was thrown: " + str(e))
             pass
         return abort(400, "Failed")
 
     @app.post(prefix + "/api/download_show/<title>")
     @auth_basic(is_authenticated_user)
     def download_show(title):
+        shared_state.logger.debug(f'Recieved API-Request for: {title}')
         try:
             payload = feedcrawler.external_sites.web_search.content_shows.get_best_result(title)
+            shared_state.logger.debug(f'Found payload is: {payload}')
             if payload:
                 matches = feedcrawler.external_sites.web_search.content_shows.download(payload)
                 if matches:
                     return "Success: " + str(matches)
-        except:
+        except Exception as e:
+            shared_state.logger.debug("An exception was thrown: " + str(e))
             pass
         return abort(400, "Failed")
 
     @app.post(prefix + "/api/download_bl/<payload>")
     @auth_basic(is_authenticated_user)
     def download_bl(payload):
         try:
@@ -949,15 +952,15 @@
             try:
                 myjd = get_info()
                 packages_to_decrypt = get_to_decrypt()
                 general_conf = CrawlerConfig('FeedCrawler')
                 packages_per_myjd_page = to_int(general_conf.get("packages_per_myjd_page"))
             except (TokenExpiredException, RequestTimeoutException, MYJDException):
                 set_device_from_config()
-                if not shared_state.values["device"] or not is_device(shared_state.values["device"]):
+                if not shared_state.get_device():
                     return abort(500, "Failed")
                 myjd = get_info()
                 packages_to_decrypt = get_to_decrypt()
                 packages_per_myjd_page = 3
             if myjd:
                 return {
                     "downloader_state": myjd[1],
@@ -980,15 +983,15 @@
     @auth_basic(is_authenticated_user)
     def myjd_state():
         try:
             try:
                 myjd = get_state()
             except (TokenExpiredException, RequestTimeoutException, MYJDException):
                 set_device_from_config()
-                if not shared_state.values["device"] or not is_device(shared_state.values["device"]):
+                if not shared_state.get_device():
                     return abort(500, "Failed")
                 myjd = get_state()
             if myjd:
                 return {
                     "downloader_state": myjd[1],
                     "grabber_collecting": myjd[2]
                 }
@@ -1160,15 +1163,15 @@
     @auth_basic(is_authenticated_user)
     def myjd_start():
         try:
             try:
                 started = jdownloader_start()
             except (TokenExpiredException, RequestTimeoutException, MYJDException):
                 set_device_from_config()
-                if not shared_state.values["device"] or not is_device(shared_state.values["device"]):
+                if not shared_state.get_device():
                     return abort(500, "Failed")
                 started = jdownloader_start()
             if started:
                 return "Success"
         except:
             pass
         return abort(400, "Failed")
@@ -1178,15 +1181,15 @@
     def myjd_pause(bl):
         try:
             bl = json.loads(bl)
             try:
                 paused = jdownloader_pause(bl)
             except (TokenExpiredException, RequestTimeoutException, MYJDException):
                 set_device_from_config()
-                if not shared_state.values["device"] or not is_device(shared_state.values["device"]):
+                if not shared_state.get_device():
                     return abort(500, "Failed")
                 paused = jdownloader_pause(bl)
             if paused:
                 return "Success"
         except:
             pass
         return abort(400, "Failed")
@@ -1195,15 +1198,15 @@
     @auth_basic(is_authenticated_user)
     def myjd_stop():
         try:
             try:
                 stopped = jdownloader_stop()
             except (TokenExpiredException, RequestTimeoutException, MYJDException):
                 set_device_from_config()
-                if not shared_state.values["device"] or not is_device(shared_state.values["device"]):
+                if not shared_state.get_device():
                     return abort(500, "Failed")
                 stopped = jdownloader_stop()
             if stopped:
                 return "Success"
         except:
             pass
         return abort(400, "Failed")
@@ -1212,15 +1215,15 @@
     @auth_basic(is_authenticated_user)
     def myjd_update():
         try:
             try:
                 updated = jdownloader_update()
             except (TokenExpiredException, RequestTimeoutException, MYJDException):
                 set_device_from_config()
-                if not shared_state.values["device"] or not is_device(shared_state.values["device"]):
+                if not shared_state.get_device():
                     return abort(500, "Failed")
                 updated = jdownloader_update()
             if updated:
                 return "Success"
         except:
             pass
         return abort(400, "Failed")
@@ -1863,15 +1866,15 @@
     Server(app, listen='0.0.0.0', port=shared_state.values["port"]).serve_forever()
 
 
 def attempt_download(package_name, links, password, ids):
     global already_added
 
     FeedDb('crawldog').store(package_name, 'added')
-    if shared_state.values["device"]:
+    if shared_state.get_device():
         if ids:
             try:
                 ids = ids.replace("%20", "").split(";")
                 linkids = ids[0]
                 uuids = ids[1]
             except:
                 linkids = False
@@ -1920,15 +1923,15 @@
                 season_string = season_string[0].replace("s", "S")
             else:
                 season_string = "^unmatchable$"
             try:
                 packages = get_packages_in_linkgrabber()
             except (TokenExpiredException, RequestTimeoutException, MYJDException):
                 set_device_from_config()
-                if not shared_state.values["device"] or not is_device(shared_state.values["device"]):
+                if not shared_state.get_device():
                     return abort(500, "Failed")
                 packages = get_packages_in_linkgrabber()
 
             if packages:
                 failed = packages[0]
                 offline = packages[1]
```

### Comparing `feedcrawler-18.0.2/feedcrawler.egg-info/PKG-INFO` & `feedcrawler-18.0.3/feedcrawler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feedcrawler
-Version: 18.0.2
+Version: 18.0.3
 Summary: Automate downloads using predefined sites and the My JDownloader API
 Home-page: https://github.com/rix1337/FeedCrawler
 Author: rix1337
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `feedcrawler-18.0.2/feedcrawler.egg-info/SOURCES.txt` & `feedcrawler-18.0.3/feedcrawler.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 feedcrawler/web_interface/vuejs_frontend/dist/assets/axios-707ed124.js
 feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-163e1b4f.js
 feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-48fa63fb.css
 feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-999550fa.woff
 feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-cfe45b98.woff2
 feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-f7e350bb.css
 feedcrawler/web_interface/vuejs_frontend/dist/assets/index-137a91df.css
-feedcrawler/web_interface/vuejs_frontend/dist/assets/index-67e298b0.js
+feedcrawler/web_interface/vuejs_frontend/dist/assets/index-44ade789.js
 feedcrawler/web_interface/vuejs_frontend/dist/assets/tippy-a1ae07b3.css
 feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-4ed993c7.js
 feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-router-4bccd9ac.js
 feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-tippy-2fb47e86.js
 feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-toastification-2a2137d8.js
 feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-toastification-4522082c.css
 feedcrawler/web_interface/vuejs_frontend/dist/assets/vuejs-paginate-next-23a274fb.js
```

### Comparing `feedcrawler-18.0.2/setup.py` & `feedcrawler-18.0.3/setup.py`

 * *Files identical despite different names*

