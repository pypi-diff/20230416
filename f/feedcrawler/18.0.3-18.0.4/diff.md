# Comparing `tmp/feedcrawler-18.0.3.tar.gz` & `tmp/feedcrawler-18.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feedcrawler-18.0.3.tar", last modified: Sun Apr 16 11:51:33 2023, max compression
+gzip compressed data, was "feedcrawler-18.0.4.tar", last modified: Sun Apr 16 13:23:50 2023, max compression
```

## Comparing `feedcrawler-18.0.3.tar` & `feedcrawler-18.0.4.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:51:33.730427 feedcrawler-18.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-04-16 11:51:33.730427 feedcrawler-18.0.3/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     7047 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:51:33.718427 feedcrawler-18.0.3/feedcrawler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10734 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/crawler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:51:33.718427 feedcrawler-18.0.3/feedcrawler/external_sites/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_sites/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:51:33.718427 feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44484 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/content_all.py
--rw-r--r--   0 runner    (1001) docker     (123)    20327 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/content_shows.py
--rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:51:33.722427 feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/sites/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/sites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9381 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/sites/content_all_by.py
--rw-r--r--   0 runner    (1001) docker     (123)     8603 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/sites/content_all_dw.py
--rw-r--r--   0 runner    (1001) docker     (123)     7555 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/sites/content_all_ff.py
--rw-r--r--   0 runner    (1001) docker     (123)    10073 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/sites/content_all_fx.py
--rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/sites/content_all_hw.py
--rw-r--r--   0 runner    (1001) docker     (123)     8177 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/sites/content_all_nk.py
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/sites/content_all_nx.py
--rw-r--r--   0 runner    (1001) docker     (123)     7417 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/sites/content_all_ww.py
--rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/sites/content_custom_dd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/sites/content_shows_dj.py
--rw-r--r--   0 runner    (1001) docker     (123)    11339 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/sites/content_shows_sf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/sites/content_shows_sj.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:51:33.722427 feedcrawler-18.0.3/feedcrawler/external_sites/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_sites/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8998 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_sites/metadata/imdb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:51:33.722427 feedcrawler-18.0.3/feedcrawler/external_sites/web_search/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_sites/web_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16818 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_sites/web_search/content_all.py
--rw-r--r--   0 runner    (1001) docker     (123)    14651 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_sites/web_search/content_shows.py
--rw-r--r--   0 runner    (1001) docker     (123)    10470 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_sites/web_search/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:51:33.722427 feedcrawler-18.0.3/feedcrawler/external_sites/web_search/sites/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_sites/web_search/sites/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_sites/web_search/sites/content_all_by.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_sites/web_search/sites/content_all_dw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_sites/web_search/sites/content_all_fx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_sites/web_search/sites/content_all_hw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_sites/web_search/sites/content_all_nk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_sites/web_search/sites/content_all_nx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:51:33.722427 feedcrawler-18.0.3/feedcrawler/external_tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42357 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_tools/myjd_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10404 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_tools/ombi_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_tools/overseerr_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8805 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/external_tools/plex_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:51:33.722427 feedcrawler-18.0.3/feedcrawler/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14941 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/jobs/feed_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    20682 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/jobs/package_watcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:51:33.726427 feedcrawler-18.0.3/feedcrawler/providers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20929 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/providers/common_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7403 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/providers/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10469 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/providers/gui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:51:33.726427 feedcrawler-18.0.3/feedcrawler/providers/http_requests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/providers/http_requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/providers/http_requests/cache_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9333 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/providers/http_requests/cloudflare_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/providers/http_requests/request_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    44206 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/providers/myjd_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     9607 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/providers/notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/providers/shared_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/providers/sqlite_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     7178 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/providers/url_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/providers/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:51:33.726427 feedcrawler-18.0.3/feedcrawler/web_interface/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/web_interface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:51:33.718427 feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:51:33.726427 feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:51:33.730427 feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    82113 2023-04-16 11:51:33.000000 feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/@formkit-18209bb1.js
--rw-r--r--   0 runner    (1001) docker     (123)    20729 2023-04-16 11:51:33.000000 feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/@popperjs-9847b28c.js
--rw-r--r--   0 runner    (1001) docker     (123)    63885 2023-04-16 11:51:33.000000 feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/@vue-d42f3502.js
--rw-r--r--   0 runner    (1001) docker     (123)     8868 2023-04-16 11:51:33.000000 feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/@vueuse-8ce5afe9.js
--rw-r--r--   0 runner    (1001) docker     (123)    28794 2023-04-16 11:51:33.000000 feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/axios-707ed124.js
--rw-r--r--   0 runner    (1001) docker     (123)    60695 2023-04-16 11:51:33.000000 feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-163e1b4f.js
--rw-r--r--   0 runner    (1001) docker     (123)   194314 2023-04-16 11:51:33.000000 feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-48fa63fb.css
--rw-r--r--   0 runner    (1001) docker     (123)   164360 2023-04-16 11:51:33.000000 feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-999550fa.woff
--rw-r--r--   0 runner    (1001) docker     (123)   121340 2023-04-16 11:51:33.000000 feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-cfe45b98.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    79982 2023-04-16 11:51:33.000000 feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-f7e350bb.css
--rw-r--r--   0 runner    (1001) docker     (123)    10842 2023-04-16 11:51:33.000000 feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/index-137a91df.css
--rw-r--r--   0 runner    (1001) docker     (123)   144763 2023-04-16 11:51:33.000000 feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/index-44ade789.js
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-04-16 11:51:33.000000 feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/tippy-a1ae07b3.css
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 11:51:33.000000 feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-4ed993c7.js
--rw-r--r--   0 runner    (1001) docker     (123)    22669 2023-04-16 11:51:33.000000 feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-router-4bccd9ac.js
--rw-r--r--   0 runner    (1001) docker     (123)    50726 2023-04-16 11:51:33.000000 feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-tippy-2fb47e86.js
--rw-r--r--   0 runner    (1001) docker     (123)    18088 2023-04-16 11:51:33.000000 feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-toastification-2a2137d8.js
--rw-r--r--   0 runner    (1001) docker     (123)    12865 2023-04-16 11:51:33.000000 feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-toastification-4522082c.css
--rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-04-16 11:51:33.000000 feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/vuejs-paginate-next-23a274fb.js
--rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-04-16 11:51:33.000000 feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/vuex-c2e7db49.js
--rw-r--r--   0 runner    (1001) docker     (123)    17818 2023-04-16 11:51:32.000000 feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-16 11:51:33.000000 feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    82905 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/feedcrawler/web_interface/web_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 11:51:33.718427 feedcrawler-18.0.3/feedcrawler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-04-16 11:51:33.000000 feedcrawler-18.0.3/feedcrawler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-04-16 11:51:33.000000 feedcrawler-18.0.3/feedcrawler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 11:51:33.000000 feedcrawler-18.0.3/feedcrawler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-16 11:51:33.000000 feedcrawler-18.0.3/feedcrawler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 11:51:33.000000 feedcrawler-18.0.3/feedcrawler.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-16 11:51:33.000000 feedcrawler-18.0.3/feedcrawler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-16 11:51:33.000000 feedcrawler-18.0.3/feedcrawler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 11:51:33.730427 feedcrawler-18.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-16 11:51:12.000000 feedcrawler-18.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:23:50.439161 feedcrawler-18.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-04-16 13:23:50.439161 feedcrawler-18.0.4/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7047 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:23:50.423161 feedcrawler-18.0.4/feedcrawler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10734 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/crawler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:23:50.427161 feedcrawler-18.0.4/feedcrawler/external_sites/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_sites/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:23:50.427161 feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44484 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/content_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20327 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/content_shows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/shared.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:23:50.427161 feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/sites/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/sites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9381 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/sites/content_all_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8603 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/sites/content_all_dw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7555 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/sites/content_all_ff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10073 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/sites/content_all_fx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/sites/content_all_hw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8177 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/sites/content_all_nk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/sites/content_all_nx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7417 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/sites/content_all_ww.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/sites/content_custom_dd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/sites/content_shows_dj.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11339 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/sites/content_shows_sf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/sites/content_shows_sj.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:23:50.427161 feedcrawler-18.0.4/feedcrawler/external_sites/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_sites/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8998 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_sites/metadata/imdb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:23:50.427161 feedcrawler-18.0.4/feedcrawler/external_sites/web_search/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_sites/web_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16818 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_sites/web_search/content_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14651 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_sites/web_search/content_shows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10470 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_sites/web_search/shared.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:23:50.427161 feedcrawler-18.0.4/feedcrawler/external_sites/web_search/sites/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_sites/web_search/sites/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_sites/web_search/sites/content_all_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_sites/web_search/sites/content_all_dw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_sites/web_search/sites/content_all_fx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_sites/web_search/sites/content_all_hw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_sites/web_search/sites/content_all_nk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_sites/web_search/sites/content_all_nx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:23:50.431161 feedcrawler-18.0.4/feedcrawler/external_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42357 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_tools/myjd_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10404 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_tools/ombi_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5804 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_tools/overseerr_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8805 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/external_tools/plex_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:23:50.431161 feedcrawler-18.0.4/feedcrawler/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14941 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/jobs/feed_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20682 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/jobs/package_watcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:23:50.431161 feedcrawler-18.0.4/feedcrawler/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20929 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/providers/common_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/providers/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10469 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/providers/gui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:23:50.431161 feedcrawler-18.0.4/feedcrawler/providers/http_requests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/providers/http_requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/providers/http_requests/cache_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9333 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/providers/http_requests/cloudflare_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7792 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/providers/http_requests/request_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44206 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/providers/myjd_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9607 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/providers/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/providers/shared_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7345 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/providers/sqlite_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/providers/url_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/providers/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:23:50.431161 feedcrawler-18.0.4/feedcrawler/web_interface/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/web_interface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:23:50.423161 feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:23:50.431161 feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:23:50.435161 feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    82113 2023-04-16 13:23:49.000000 feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/@formkit-18209bb1.js
+-rw-r--r--   0 runner    (1001) docker     (123)    20729 2023-04-16 13:23:49.000000 feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/@popperjs-9847b28c.js
+-rw-r--r--   0 runner    (1001) docker     (123)    63885 2023-04-16 13:23:49.000000 feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/@vue-d42f3502.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8868 2023-04-16 13:23:49.000000 feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/@vueuse-8ce5afe9.js
+-rw-r--r--   0 runner    (1001) docker     (123)    28794 2023-04-16 13:23:49.000000 feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/axios-707ed124.js
+-rw-r--r--   0 runner    (1001) docker     (123)    60695 2023-04-16 13:23:49.000000 feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-163e1b4f.js
+-rw-r--r--   0 runner    (1001) docker     (123)   194314 2023-04-16 13:23:49.000000 feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-48fa63fb.css
+-rw-r--r--   0 runner    (1001) docker     (123)   164360 2023-04-16 13:23:49.000000 feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-999550fa.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   121340 2023-04-16 13:23:49.000000 feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-cfe45b98.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    79982 2023-04-16 13:23:49.000000 feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-f7e350bb.css
+-rw-r--r--   0 runner    (1001) docker     (123)    10842 2023-04-16 13:23:49.000000 feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/index-137a91df.css
+-rw-r--r--   0 runner    (1001) docker     (123)   144763 2023-04-16 13:23:49.000000 feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/index-44ade789.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-04-16 13:23:49.000000 feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/tippy-a1ae07b3.css
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 13:23:49.000000 feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-4ed993c7.js
+-rw-r--r--   0 runner    (1001) docker     (123)    22669 2023-04-16 13:23:49.000000 feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-router-4bccd9ac.js
+-rw-r--r--   0 runner    (1001) docker     (123)    50726 2023-04-16 13:23:49.000000 feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-tippy-2fb47e86.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18088 2023-04-16 13:23:49.000000 feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-toastification-2a2137d8.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12865 2023-04-16 13:23:49.000000 feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-toastification-4522082c.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-04-16 13:23:49.000000 feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/vuejs-paginate-next-23a274fb.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-04-16 13:23:49.000000 feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/vuex-c2e7db49.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17818 2023-04-16 13:23:49.000000 feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-16 13:23:49.000000 feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    82905 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/feedcrawler/web_interface/web_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 13:23:50.423161 feedcrawler-18.0.4/feedcrawler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-04-16 13:23:50.000000 feedcrawler-18.0.4/feedcrawler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-04-16 13:23:50.000000 feedcrawler-18.0.4/feedcrawler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 13:23:50.000000 feedcrawler-18.0.4/feedcrawler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-16 13:23:50.000000 feedcrawler-18.0.4/feedcrawler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 13:23:50.000000 feedcrawler-18.0.4/feedcrawler.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-16 13:23:50.000000 feedcrawler-18.0.4/feedcrawler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-16 13:23:50.000000 feedcrawler-18.0.4/feedcrawler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 13:23:50.439161 feedcrawler-18.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-16 13:23:16.000000 feedcrawler-18.0.4/setup.py
```

### Comparing `feedcrawler-18.0.3/LICENSE.md` & `feedcrawler-18.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/PKG-INFO` & `feedcrawler-18.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feedcrawler
-Version: 18.0.3
+Version: 18.0.4
 Summary: Automate downloads using predefined sites and the My JDownloader API
 Home-page: https://github.com/rix1337/FeedCrawler
 Author: rix1337
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `feedcrawler-18.0.3/README.md` & `feedcrawler-18.0.4/README.md`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/feedcrawler/crawler.py` & `feedcrawler-18.0.4/feedcrawler/crawler.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/content_all.py` & `feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/content_all.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/content_shows.py` & `feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/content_shows.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/shared.py` & `feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/shared.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/sites/content_all_by.py` & `feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/sites/content_all_by.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/sites/content_all_dw.py` & `feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/sites/content_all_dw.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/sites/content_all_ff.py` & `feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/sites/content_all_ff.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/sites/content_all_fx.py` & `feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/sites/content_all_fx.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/sites/content_all_hw.py` & `feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/sites/content_all_hw.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/sites/content_all_nk.py` & `feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/sites/content_all_nk.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/sites/content_all_nx.py` & `feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/sites/content_all_nx.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/sites/content_all_ww.py` & `feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/sites/content_all_ww.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/sites/content_custom_dd.py` & `feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/sites/content_custom_dd.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/sites/content_shows_dj.py` & `feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/sites/content_shows_dj.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/sites/content_shows_sf.py` & `feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/sites/content_shows_sf.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/feedcrawler/external_sites/feed_search/sites/content_shows_sj.py` & `feedcrawler-18.0.4/feedcrawler/external_sites/feed_search/sites/content_shows_sj.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/feedcrawler/external_sites/metadata/imdb.py` & `feedcrawler-18.0.4/feedcrawler/external_sites/metadata/imdb.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/feedcrawler/external_sites/web_search/content_all.py` & `feedcrawler-18.0.4/feedcrawler/external_sites/web_search/content_all.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/feedcrawler/external_sites/web_search/content_shows.py` & `feedcrawler-18.0.4/feedcrawler/external_sites/web_search/content_shows.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/feedcrawler/external_sites/web_search/shared.py` & `feedcrawler-18.0.4/feedcrawler/external_sites/web_search/shared.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/feedcrawler/external_sites/web_search/sites/content_all_by.py` & `feedcrawler-18.0.4/feedcrawler/external_sites/web_search/sites/content_all_by.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/feedcrawler/external_sites/web_search/sites/content_all_dw.py` & `feedcrawler-18.0.4/feedcrawler/external_sites/web_search/sites/content_all_dw.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/feedcrawler/external_sites/web_search/sites/content_all_fx.py` & `feedcrawler-18.0.4/feedcrawler/external_sites/web_search/sites/content_all_fx.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/feedcrawler/external_sites/web_search/sites/content_all_hw.py` & `feedcrawler-18.0.4/feedcrawler/external_sites/web_search/sites/content_all_hw.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/feedcrawler/external_sites/web_search/sites/content_all_nk.py` & `feedcrawler-18.0.4/feedcrawler/external_sites/web_search/sites/content_all_nk.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/feedcrawler/external_sites/web_search/sites/content_all_nx.py` & `feedcrawler-18.0.4/feedcrawler/external_sites/web_search/sites/content_all_nx.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/feedcrawler/external_tools/myjd_api.py` & `feedcrawler-18.0.4/feedcrawler/external_tools/myjd_api.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/feedcrawler/external_tools/ombi_api.py` & `feedcrawler-18.0.4/feedcrawler/external_tools/ombi_api.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/feedcrawler/external_tools/overseerr_api.py` & `feedcrawler-18.0.4/feedcrawler/external_tools/overseerr_api.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/feedcrawler/external_tools/plex_api.py` & `feedcrawler-18.0.4/feedcrawler/external_tools/plex_api.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/feedcrawler/jobs/feed_search.py` & `feedcrawler-18.0.4/feedcrawler/jobs/feed_search.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/feedcrawler/jobs/package_watcher.py` & `feedcrawler-18.0.4/feedcrawler/jobs/package_watcher.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/feedcrawler/providers/common_functions.py` & `feedcrawler-18.0.4/feedcrawler/providers/common_functions.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/feedcrawler/providers/gui.py` & `feedcrawler-18.0.4/feedcrawler/providers/gui.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/feedcrawler/providers/http_requests/cache_handler.py` & `feedcrawler-18.0.4/feedcrawler/providers/http_requests/cache_handler.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/feedcrawler/providers/http_requests/cloudflare_handlers.py` & `feedcrawler-18.0.4/feedcrawler/providers/http_requests/cloudflare_handlers.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/feedcrawler/providers/http_requests/request_handler.py` & `feedcrawler-18.0.4/feedcrawler/providers/http_requests/request_handler.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/feedcrawler/providers/myjd_connection.py` & `feedcrawler-18.0.4/feedcrawler/providers/myjd_connection.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/feedcrawler/providers/notifications.py` & `feedcrawler-18.0.4/feedcrawler/providers/notifications.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/feedcrawler/providers/shared_state.py` & `feedcrawler-18.0.4/feedcrawler/providers/shared_state.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/feedcrawler/providers/sqlite_database.py` & `feedcrawler-18.0.4/feedcrawler/providers/sqlite_database.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
         'cdc',
         'crawldog',
         'crawltimes',
         'episode_remover',
         'site_status',
         'flaresolverr',
         'sponsors_helper',
+        'secrets',
         'to_decrypt',
     ]
 
     cursor.execute("SELECT name FROM sqlite_master WHERE type='table'")
     table_names = [row[0] for row in cursor.fetchall()]
 
     tables_to_drop = set(table_names) - set(keep_tables)
```

### Comparing `feedcrawler-18.0.3/feedcrawler/providers/url_functions.py` & `feedcrawler-18.0.4/feedcrawler/providers/url_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
                 continue
 
         hostname = hostnames.get(site.lower())
         if not hostname:
             db_status.update_store(site + "_normal", "Blocked")
             db_status.update_store(site + "_advanced", "Blocked")
         else:
+            hostnames.save(site.lower(), hostname)
             db_status.delete(site + "_normal")
             db_status.delete(site + "_advanced")
             sponsors_helper_url = get_solver_url("sponsors_helper")
             flaresolverr_url = get_solver_url("flaresolverr")
             skip_sites = ["HW", "WW", ]  # SJ/DJ not listed, because they rarely block scraping attempts
             skip_normal_ip = (sponsors_helper_url or flaresolverr_url) and (site in skip_sites)
             if skip_normal_ip:
```

### Comparing `feedcrawler-18.0.3/feedcrawler/providers/version.py` & `feedcrawler-18.0.4/feedcrawler/providers/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import re
 from distutils.version import StrictVersion
 from urllib.request import urlopen
 
 
 def get_version():
-    return "18.0.3"
+    return "18.0.4"
 
 
 def create_version_file():
     version = get_version()
     version_clean = re.sub('[^\d\.]', '', version)
     if "a" in version:
         suffix = version.split("a")[1]
```

### Comparing `feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/@formkit-18209bb1.js` & `feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/@formkit-18209bb1.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/@popperjs-9847b28c.js` & `feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/@popperjs-9847b28c.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/@vue-d42f3502.js` & `feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/@vue-d42f3502.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/@vueuse-8ce5afe9.js` & `feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/@vueuse-8ce5afe9.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/axios-707ed124.js` & `feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/axios-707ed124.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-163e1b4f.js` & `feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-163e1b4f.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-48fa63fb.css` & `feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-48fa63fb.css`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-999550fa.woff` & `feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-999550fa.woff`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-cfe45b98.woff2` & `feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-cfe45b98.woff2`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-f7e350bb.css` & `feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/bootstrap-icons-f7e350bb.css`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/index-137a91df.css` & `feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/index-137a91df.css`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/index-44ade789.js` & `feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/index-44ade789.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/tippy-a1ae07b3.css` & `feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/tippy-a1ae07b3.css`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-router-4bccd9ac.js` & `feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-router-4bccd9ac.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-tippy-2fb47e86.js` & `feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-tippy-2fb47e86.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-toastification-2a2137d8.js` & `feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-toastification-2a2137d8.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-toastification-4522082c.css` & `feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/vue-toastification-4522082c.css`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/vuejs-paginate-next-23a274fb.js` & `feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/vuejs-paginate-next-23a274fb.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/assets/vuex-c2e7db49.js` & `feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/assets/vuex-c2e7db49.js`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/favicon.ico` & `feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/favicon.ico`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/feedcrawler/web_interface/vuejs_frontend/dist/index.html` & `feedcrawler-18.0.4/feedcrawler/web_interface/vuejs_frontend/dist/index.html`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/feedcrawler/web_interface/web_server.py` & `feedcrawler-18.0.4/feedcrawler/web_interface/web_server.py`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/feedcrawler.egg-info/PKG-INFO` & `feedcrawler-18.0.4/feedcrawler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feedcrawler
-Version: 18.0.3
+Version: 18.0.4
 Summary: Automate downloads using predefined sites and the My JDownloader API
 Home-page: https://github.com/rix1337/FeedCrawler
 Author: rix1337
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `feedcrawler-18.0.3/feedcrawler.egg-info/SOURCES.txt` & `feedcrawler-18.0.4/feedcrawler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `feedcrawler-18.0.3/setup.py` & `feedcrawler-18.0.4/setup.py`

 * *Files identical despite different names*

