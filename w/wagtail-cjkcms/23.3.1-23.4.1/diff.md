# Comparing `tmp/wagtail-cjkcms-23.3.1.tar.gz` & `tmp/wagtail-cjkcms-23.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-cjkcms-23.3.1.tar", last modified: Sun Mar 12 10:10:56 2023, max compression
+gzip compressed data, was "wagtail-cjkcms-23.4.1.tar", last modified: Sun Apr 16 16:31:36 2023, max compression
```

## Comparing `wagtail-cjkcms-23.3.1.tar` & `wagtail-cjkcms-23.4.1.tar`

### file list

```diff
@@ -1,268 +1,264 @@
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-03-12 10:10:56.513049 wagtail-cjkcms-23.3.1/
--rw-r--r--   0 grze      (1000) grze      (1000)     6185 2023-03-12 10:10:05.000000 wagtail-cjkcms-23.3.1/CHANGELOG.md
--rw-r--r--   0 grze      (1000) grze      (1000)     1542 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/LICENSE
--rw-r--r--   0 grze      (1000) grze      (1000)      239 2022-12-04 00:45:57.000000 wagtail-cjkcms-23.3.1/MANIFEST.in
--rw-r--r--   0 grze      (1000) grze      (1000)     2828 2023-03-12 10:10:56.513049 wagtail-cjkcms-23.3.1/PKG-INFO
--rw-r--r--   0 grze      (1000) grze      (1000)     1688 2023-02-11 16:22:42.000000 wagtail-cjkcms-23.3.1/README.md
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-03-12 10:10:56.483049 wagtail-cjkcms-23.3.1/cjkcms/
--rw-r--r--   0 grze      (1000) grze      (1000)      272 2023-03-12 10:09:10.000000 wagtail-cjkcms-23.3.1/cjkcms/__init__.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-03-12 10:10:56.483049 wagtail-cjkcms-23.3.1/cjkcms/api/
--rw-r--r--   0 grze      (1000) grze      (1000)        0 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/api/__init__.py
--rw-r--r--   0 grze      (1000) grze      (1000)     2832 2023-02-11 16:38:47.000000 wagtail-cjkcms-23.3.1/cjkcms/api/mailchimp.py
--rw-r--r--   0 grze      (1000) grze      (1000)      173 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/apps.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-03-12 10:10:56.483049 wagtail-cjkcms-23.3.1/cjkcms/bin/
--rw-r--r--   0 grze      (1000) grze      (1000)        0 2022-12-04 00:45:03.000000 wagtail-cjkcms-23.3.1/cjkcms/bin/__init__.py
--rw-r--r--   0 grze      (1000) grze      (1000)     5752 2023-03-12 09:50:25.000000 wagtail-cjkcms-23.3.1/cjkcms/bin/cjkcms.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-03-12 10:10:56.483049 wagtail-cjkcms-23.3.1/cjkcms/blocks/
--rw-r--r--   0 grze      (1000) grze      (1000)     3166 2022-11-05 00:52:16.000000 wagtail-cjkcms-23.3.1/cjkcms/blocks/__init__.py
--rw-r--r--   0 grze      (1000) grze      (1000)    10455 2023-02-11 16:38:50.000000 wagtail-cjkcms-23.3.1/cjkcms/blocks/base_blocks.py
--rw-r--r--   0 grze      (1000) grze      (1000)     8476 2023-02-11 18:09:33.000000 wagtail-cjkcms-23.3.1/cjkcms/blocks/content_blocks.py
--rw-r--r--   0 grze      (1000) grze      (1000)     9292 2023-02-11 18:15:03.000000 wagtail-cjkcms-23.3.1/cjkcms/blocks/html_blocks.py
--rw-r--r--   0 grze      (1000) grze      (1000)     3337 2023-02-11 16:39:50.000000 wagtail-cjkcms-23.3.1/cjkcms/blocks/layout_blocks.py
--rw-r--r--   0 grze      (1000) grze      (1000)      171 2022-11-06 21:05:14.000000 wagtail-cjkcms-23.3.1/cjkcms/blocks/searchable_html_block.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-03-12 10:10:56.483049 wagtail-cjkcms-23.3.1/cjkcms/draftail/
--rw-r--r--   0 grze      (1000) grze      (1000)      305 2022-12-04 00:45:57.000000 wagtail-cjkcms-23.3.1/cjkcms/draftail/__init__.py
--rw-r--r--   0 grze      (1000) grze      (1000)     3157 2023-02-11 16:38:48.000000 wagtail-cjkcms-23.3.1/cjkcms/draftail/draftail_extensions.py
--rw-r--r--   0 grze      (1000) grze      (1000)     5157 2022-11-05 00:41:52.000000 wagtail-cjkcms-23.3.1/cjkcms/draftail/draftail_icons.py
--rw-r--r--   0 grze      (1000) grze      (1000)     3191 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/fields.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-03-12 10:10:56.483049 wagtail-cjkcms-23.3.1/cjkcms/finders/
--rw-r--r--   0 grze      (1000) grze      (1000)        0 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/finders/__init__.py
--rw-r--r--   0 grze      (1000) grze      (1000)     2459 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/finders/oembed.py
--rw-r--r--   0 grze      (1000) grze      (1000)      361 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/forms.py
--rw-r--r--   0 grze      (1000) grze      (1000)     1804 2022-10-08 14:57:40.000000 wagtail-cjkcms-23.3.1/cjkcms/image_formats.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-03-12 10:10:56.473049 wagtail-cjkcms-23.3.1/cjkcms/management/
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-03-12 10:10:56.483049 wagtail-cjkcms-23.3.1/cjkcms/management/commands/
--rw-r--r--   0 grze      (1000) grze      (1000)        0 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/management/commands/__init__.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-03-12 10:10:56.483049 wagtail-cjkcms-23.3.1/cjkcms/management/commands/__pycache__/
--rw-r--r--   0 grze      (1000) grze      (1000)      170 2022-09-07 17:29:54.000000 wagtail-cjkcms-23.3.1/cjkcms/management/commands/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 grze      (1000) grze      (1000)      187 2023-02-11 16:21:57.000000 wagtail-cjkcms-23.3.1/cjkcms/management/commands/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 grze      (1000) grze      (1000)      837 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/management/commands/__pycache__/clear-embeds.cpython-310.pyc
--rw-r--r--   0 grze      (1000) grze      (1000)     1129 2023-02-11 16:21:57.000000 wagtail-cjkcms-23.3.1/cjkcms/management/commands/__pycache__/clear-embeds.cpython-311.pyc
--rw-r--r--   0 grze      (1000) grze      (1000)     2746 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/management/commands/__pycache__/import-csv.cpython-310.pyc
--rw-r--r--   0 grze      (1000) grze      (1000)     4680 2023-02-11 16:21:57.000000 wagtail-cjkcms-23.3.1/cjkcms/management/commands/__pycache__/import-csv.cpython-311.pyc
--rw-r--r--   0 grze      (1000) grze      (1000)     1211 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/management/commands/__pycache__/init-collections.cpython-310.pyc
--rw-r--r--   0 grze      (1000) grze      (1000)     1691 2023-02-11 16:40:28.000000 wagtail-cjkcms-23.3.1/cjkcms/management/commands/__pycache__/init-collections.cpython-311.pyc
--rw-r--r--   0 grze      (1000) grze      (1000)     2796 2022-09-07 18:55:45.000000 wagtail-cjkcms-23.3.1/cjkcms/management/commands/__pycache__/init-navbar.cpython-310.pyc
--rw-r--r--   0 grze      (1000) grze      (1000)     4303 2023-02-11 16:40:28.000000 wagtail-cjkcms-23.3.1/cjkcms/management/commands/__pycache__/init-navbar.cpython-311.pyc
--rw-r--r--   0 grze      (1000) grze      (1000)     2897 2022-10-08 15:59:38.000000 wagtail-cjkcms-23.3.1/cjkcms/management/commands/__pycache__/init-website.cpython-310.pyc
--rw-r--r--   0 grze      (1000) grze      (1000)     4641 2023-02-11 16:40:28.000000 wagtail-cjkcms-23.3.1/cjkcms/management/commands/__pycache__/init-website.cpython-311.pyc
--rw-r--r--   0 grze      (1000) grze      (1000)      453 2022-10-08 15:54:38.000000 wagtail-cjkcms-23.3.1/cjkcms/management/commands/clear-embeds.py
--rw-r--r--   0 grze      (1000) grze      (1000)     2565 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/management/commands/import-csv.py
--rw-r--r--   0 grze      (1000) grze      (1000)      952 2023-02-11 16:38:46.000000 wagtail-cjkcms-23.3.1/cjkcms/management/commands/init-collections.py
--rw-r--r--   0 grze      (1000) grze      (1000)     3560 2023-02-11 16:38:45.000000 wagtail-cjkcms-23.3.1/cjkcms/management/commands/init-navbar.py
--rw-r--r--   0 grze      (1000) grze      (1000)     3820 2023-02-11 16:38:43.000000 wagtail-cjkcms-23.3.1/cjkcms/management/commands/init-website.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-03-12 10:10:56.493049 wagtail-cjkcms-23.3.1/cjkcms/migrations/
--rw-r--r--   0 grze      (1000) grze      (1000)   216350 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/migrations/0001_initial.py
--rw-r--r--   0 grze      (1000) grze      (1000)      835 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/migrations/0002_alter_body_to_cjkcmsstreamfield.py
--rw-r--r--   0 grze      (1000) grze      (1000)      668 2022-09-02 22:15:20.000000 wagtail-cjkcms-23.3.1/cjkcms/migrations/0003_alter_footer_content_alter_navbar_menu_items.py
--rw-r--r--   0 grze      (1000) grze      (1000)     1027 2022-11-27 18:28:34.000000 wagtail-cjkcms-23.3.1/cjkcms/migrations/0004_layoutsettings_articles_date_format_and_more.py
--rw-r--r--   0 grze      (1000) grze      (1000)     1709 2023-01-27 23:37:48.000000 wagtail-cjkcms-23.3.1/cjkcms/migrations/0005_layoutsettings_custom_font_and_more.py
--rw-r--r--   0 grze      (1000) grze      (1000)     2886 2023-02-24 14:27:04.000000 wagtail-cjkcms-23.3.1/cjkcms/migrations/0006_analyticssettings_consent_modal_layout_and_more.py
--rw-r--r--   0 grze      (1000) grze      (1000)        0 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/migrations/__init__.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-03-12 10:10:56.493049 wagtail-cjkcms-23.3.1/cjkcms/models/
--rw-r--r--   0 grze      (1000) grze      (1000)      232 2022-10-08 15:46:13.000000 wagtail-cjkcms-23.3.1/cjkcms/models/__init__.py
--rw-r--r--   0 grze      (1000) grze      (1000)      395 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/models/admin_sidebar.py
--rw-r--r--   0 grze      (1000) grze      (1000)     2356 2022-10-08 15:42:58.000000 wagtail-cjkcms-23.3.1/cjkcms/models/cms_models.py
--rw-r--r--   0 grze      (1000) grze      (1000)     6302 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/models/integration_models.py
--rw-r--r--   0 grze      (1000) grze      (1000)    19651 2023-02-11 16:38:49.000000 wagtail-cjkcms-23.3.1/cjkcms/models/page_models.py
--rw-r--r--   0 grze      (1000) grze      (1000)    12522 2023-02-11 16:38:53.000000 wagtail-cjkcms-23.3.1/cjkcms/models/snippet_models.py
--rw-r--r--   0 grze      (1000) grze      (1000)    18053 2023-02-20 23:04:05.000000 wagtail-cjkcms-23.3.1/cjkcms/models/wagtailsettings_models.py
--rw-r--r--   0 grze      (1000) grze      (1000)      125 2023-02-11 17:55:54.000000 wagtail-cjkcms-23.3.1/cjkcms/search_urls.py
--rw-r--r--   0 grze      (1000) grze      (1000)     9215 2023-02-21 10:30:29.000000 wagtail-cjkcms-23.3.1/cjkcms/settings.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-03-12 10:10:56.473049 wagtail-cjkcms-23.3.1/cjkcms/static/
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-03-12 10:10:56.473049 wagtail-cjkcms-23.3.1/cjkcms/static/cjkcms/
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-03-12 10:10:56.493049 wagtail-cjkcms-23.3.1/cjkcms/static/cjkcms/css/
--rw-r--r--   0 grze      (1000) grze      (1000)      846 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/static/cjkcms/css/cjkcms-admin.css
--rw-r--r--   0 grze      (1000) grze      (1000)     1039 2022-11-05 00:56:18.000000 wagtail-cjkcms-23.3.1/cjkcms/static/cjkcms/css/cjkcms-editor.css
--rw-r--r--   0 grze      (1000) grze      (1000)     4375 2023-02-21 19:32:59.000000 wagtail-cjkcms-23.3.1/cjkcms/static/cjkcms/css/cjkcms-front.css
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-03-12 10:10:56.473049 wagtail-cjkcms-23.3.1/cjkcms/static/cjkcms/images/
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-03-12 10:10:56.493049 wagtail-cjkcms-23.3.1/cjkcms/static/cjkcms/images/avatars/
--rw-r--r--   0 grze      (1000) grze      (1000)      535 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/static/cjkcms/images/avatars/default.png
--rw-r--r--   0 grze      (1000) grze      (1000)      384 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/static/cjkcms/images/avatars/default.svg
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-03-12 10:10:56.493049 wagtail-cjkcms-23.3.1/cjkcms/static/cjkcms/images/icons/
--rw-r--r--   0 grze      (1000) grze      (1000)      705 2022-12-04 00:45:57.000000 wagtail-cjkcms-23.3.1/cjkcms/static/cjkcms/images/icons/quote.svg
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-03-12 10:10:56.493049 wagtail-cjkcms-23.3.1/cjkcms/static/cjkcms/images/logos/
--rw-r--r--   0 grze      (1000) grze      (1000)     4166 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/static/cjkcms/images/logos/cms-logo-long.svg
--rw-r--r--   0 grze      (1000) grze      (1000)     4218 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/static/cjkcms/images/logos/cms-logo-square.svg
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-03-12 10:10:56.493049 wagtail-cjkcms-23.3.1/cjkcms/static/cjkcms/images/patterns/
--rw-r--r--   0 grze      (1000) grze      (1000)    47935 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/static/cjkcms/images/patterns/pattern1.jpg
--rw-r--r--   0 grze      (1000) grze      (1000)    31707 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/static/cjkcms/images/patterns/pattern2.jpg
--rw-r--r--   0 grze      (1000) grze      (1000)    38190 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/static/cjkcms/images/patterns/pattern3.jpg
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-03-12 10:10:56.493049 wagtail-cjkcms-23.3.1/cjkcms/static/cjkcms/js/
--rw-r--r--   0 grze      (1000) grze      (1000)      444 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/static/cjkcms/js/cjkcms-editor.js
--rw-r--r--   0 grze      (1000) grze      (1000)     5780 2023-02-23 11:19:34.000000 wagtail-cjkcms-23.3.1/cjkcms/static/cjkcms/js/cjkcms-front.js
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-03-12 10:10:56.493049 wagtail-cjkcms-23.3.1/cjkcms/static/cookieconsent/
--rw-r--r--   0 grze      (1000) grze      (1000)    18803 2023-02-20 19:07:02.000000 wagtail-cjkcms-23.3.1/cjkcms/static/cookieconsent/cookieconsent.css
--rw-r--r--   0 grze      (1000) grze      (1000)    18743 2023-02-20 19:07:02.000000 wagtail-cjkcms-23.3.1/cjkcms/static/cookieconsent/cookieconsent.js
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-03-12 10:10:56.493049 wagtail-cjkcms-23.3.1/cjkcms/templates/
--rw-r--r--   0 grze      (1000) grze      (1000)     4176 2023-02-11 18:47:44.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/404.html
--rw-r--r--   0 grze      (1000) grze      (1000)     4802 2023-02-11 18:53:12.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/500.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-03-12 10:10:56.493049 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-03-12 10:10:56.503049 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/
--rw-r--r--   0 grze      (1000) grze      (1000)     1443 2022-11-25 23:18:05.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/accordion_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      974 2022-10-08 14:57:40.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/article_block_card.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1132 2022-10-08 14:57:40.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/article_masonry_card.html
--rw-r--r--   0 grze      (1000) grze      (1000)      188 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/base_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)     2505 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/base_link_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      740 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/button_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      746 2022-11-25 22:51:18.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/card_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      856 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/card_blurb.html
--rw-r--r--   0 grze      (1000) grze      (1000)      786 2022-11-05 02:21:33.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/card_foot.html
--rw-r--r--   0 grze      (1000) grze      (1000)      730 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/card_head.html
--rw-r--r--   0 grze      (1000) grze      (1000)      771 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/card_head_foot.html
--rw-r--r--   0 grze      (1000) grze      (1000)      990 2022-11-07 01:06:28.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/card_horizontal.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1104 2022-11-07 00:10:24.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/card_horizontal2.html
--rw-r--r--   0 grze      (1000) grze      (1000)      786 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/card_img.html
--rw-r--r--   0 grze      (1000) grze      (1000)     2618 2022-11-25 22:22:40.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/card_landing1.html
--rw-r--r--   0 grze      (1000) grze      (1000)     2758 2023-01-19 18:18:18.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/card_landing2.html
--rw-r--r--   0 grze      (1000) grze      (1000)      678 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/cardgrid_columns.html
--rw-r--r--   0 grze      (1000) grze      (1000)      450 2022-11-05 02:24:30.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/cardgrid_deck.html
--rw-r--r--   0 grze      (1000) grze      (1000)      277 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/cardgrid_group.html
--rw-r--r--   0 grze      (1000) grze      (1000)      276 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/cardgrid_zero.html
--rw-r--r--   0 grze      (1000) grze      (1000)     2698 2023-02-21 20:05:05.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/carousel_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      406 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/column_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      137 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/document_link_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      920 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/download_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      103 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/embed_video_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)       95 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/external_link_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      424 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/grid_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      200 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/h1_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      200 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/h2_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      200 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/h3_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      790 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/hero_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      275 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/image_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1400 2023-01-28 03:28:52.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/image_gallery_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      627 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/image_link_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1020 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/modal_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      164 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/page_link_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      787 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/pagelist_article_card_columns.html
--rw-r--r--   0 grze      (1000) grze      (1000)      642 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/pagelist_article_card_deck.html
--rw-r--r--   0 grze      (1000) grze      (1000)      361 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/pagelist_article_card_group.html
--rw-r--r--   0 grze      (1000) grze      (1000)      956 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/pagelist_article_media.html
--rw-r--r--   0 grze      (1000) grze      (1000)      397 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/pagelist_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      610 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/pagelist_list_group.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1224 2023-02-04 17:34:09.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/pagelist_toc_nextprev.html
--rw-r--r--   0 grze      (1000) grze      (1000)      300 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/pagepreview_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      793 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/pagepreview_card.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1065 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/pagepreview_form.html
--rw-r--r--   0 grze      (1000) grze      (1000)      244 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/pricelist_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      513 2023-02-11 18:10:08.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/pricelistitem_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      353 2022-11-26 22:35:13.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/quote_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)      852 2022-12-04 00:45:57.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/quote_block_leftbar.html
--rw-r--r--   0 grze      (1000) grze      (1000)      998 2022-12-04 00:45:57.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/quote_block_start_end_quote.html
--rw-r--r--   0 grze      (1000) grze      (1000)      216 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/reusable_content_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)       91 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/rich_text_block.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1095 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/table_block.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-03-12 10:10:56.503049 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/cookieconsent/
--rw-r--r--   0 grze      (1000) grze      (1000)     3672 2023-02-20 22:22:58.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/cookieconsent/languages.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-03-12 10:10:56.503049 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/formfields/
--rw-r--r--   0 grze      (1000) grze      (1000)      267 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/formfields/date.html
--rw-r--r--   0 grze      (1000) grze      (1000)      416 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/formfields/datetime.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-03-12 10:10:56.503049 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/formfields/mailchimp/
--rw-r--r--   0 grze      (1000) grze      (1000)     9267 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/formfields/mailchimp/_2vanilla_subscriber_integration_js.html
--rw-r--r--   0 grze      (1000) grze      (1000)     6469 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/formfields/mailchimp/subscriber_integration_js.html
--rw-r--r--   0 grze      (1000) grze      (1000)      793 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/formfields/mailchimp/subscriber_integration_widget.html
--rw-r--r--   0 grze      (1000) grze      (1000)      264 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/formfields/time.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-03-12 10:10:56.503049 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/icons/
--rw-r--r--   0 grze      (1000) grze      (1000)      465 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/icons/align-left.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      573 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/icons/check-square-o.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      277 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/icons/columns.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      359 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/icons/desktop.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      571 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/icons/font.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      292 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/icons/google.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      813 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/icons/hand-pointer-o.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      666 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/icons/hashtag.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      840 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/icons/header.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      835 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/icons/list-alt.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      459 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/icons/map.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      448 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/icons/newspaper-o.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      721 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/icons/puzzle-piece.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      635 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/icons/recycle.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      174 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/icons/stop.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      505 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/icons/th-large.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      762 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/icons/universal-access.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      548 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/icons/usd.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      225 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/icons/window-maximize.svg
--rw-r--r--   0 grze      (1000) grze      (1000)      199 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/icons/window-minimize.svg
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-03-12 10:10:56.503049 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/includes/
--rw-r--r--   0 grze      (1000) grze      (1000)      286 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/includes/cjkcms_banner.html
--rw-r--r--   0 grze      (1000) grze      (1000)      689 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/includes/classifier_dropdowns.html
--rw-r--r--   0 grze      (1000) grze      (1000)      579 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/includes/classifier_nav.html
--rw-r--r--   0 grze      (1000) grze      (1000)      286 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/includes/codered_banner.html
--rw-r--r--   0 grze      (1000) grze      (1000)      268 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/includes/form_honeypot.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1061 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/includes/pagination.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-03-12 10:10:56.503049 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/includes/stream_forms/
--rw-r--r--   0 grze      (1000) grze      (1000)      532 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/includes/stream_forms/render_field.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-03-12 10:10:56.513049 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/pages/
--rw-r--r--   0 grze      (1000) grze      (1000)     2002 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/pages/article_index_page.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1705 2022-11-27 18:34:57.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/pages/article_page.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1018 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/pages/article_page.search.html
--rw-r--r--   0 grze      (1000) grze      (1000)     7931 2023-02-23 11:05:35.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/pages/base.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1104 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/pages/form_page.html
--rw-r--r--   0 grze      (1000) grze      (1000)      248 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/pages/form_page_landing.html
--rw-r--r--   0 grze      (1000) grze      (1000)       50 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/pages/home_page.html
--rw-r--r--   0 grze      (1000) grze      (1000)     2610 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/pages/search.html
--rw-r--r--   0 grze      (1000) grze      (1000)      582 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/pages/search_result.html
--rw-r--r--   0 grze      (1000) grze      (1000)     2462 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/pages/stream_form_page.html
--rw-r--r--   0 grze      (1000) grze      (1000)      838 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/pages/web_page.html
--rw-r--r--   0 grze      (1000) grze      (1000)      623 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/pages/web_page_notitle.html
--rw-r--r--   0 grze      (1000) grze      (1000)      122 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/robots.txt
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-03-12 10:10:56.513049 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/snippets/
--rw-r--r--   0 grze      (1000) grze      (1000)      430 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/snippets/footer.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1794 2023-01-28 00:30:46.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/snippets/frontend_assets.html
--rw-r--r--   0 grze      (1000) grze      (1000)     1196 2023-01-28 00:24:34.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/snippets/frontend_scripts.html
--rw-r--r--   0 grze      (1000) grze      (1000)      836 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/snippets/lang_selector.html
--rw-r--r--   0 grze      (1000) grze      (1000)     2586 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/snippets/navbar.html
--rw-r--r--   0 grze      (1000) grze      (1000)      386 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/snippets/navbar_search.html
--rw-r--r--   0 grze      (1000) grze      (1000)      158 2023-02-23 11:21:17.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/snippets/tracking_g3.html
--rw-r--r--   0 grze      (1000) grze      (1000)      831 2023-02-23 11:21:47.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/snippets/tracking_g4.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-03-12 10:10:56.513049 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/widgets/
--rw-r--r--   0 grze      (1000) grze      (1000)     1384 2022-09-02 22:36:35.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/widgets/checkbox_classifiers.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-03-12 10:10:56.483049 wagtail-cjkcms-23.3.1/cjkcms/templates/wagtailadmin/
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-03-12 10:10:56.513049 wagtail-cjkcms-23.3.1/cjkcms/templates/wagtailadmin/block_forms/
--rw-r--r--   0 grze      (1000) grze      (1000)      754 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/wagtailadmin/block_forms/base_block_settings_struct.html
--rw-r--r--   0 grze      (1000) grze      (1000)      550 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/wagtailadmin/block_forms/struct.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-03-12 10:10:56.513049 wagtail-cjkcms-23.3.1/cjkcms/templates/wagtailadmin/shared/
--rw-r--r--   0 grze      (1000) grze      (1000)      885 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templates/wagtailadmin/shared/cr_main_nav_2fix.html
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-03-12 10:10:56.513049 wagtail-cjkcms-23.3.1/cjkcms/templatetags/
--rw-r--r--   0 grze      (1000) grze      (1000)        0 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templatetags/__init__.py
--rw-r--r--   0 grze      (1000) grze      (1000)      327 2022-11-30 10:05:15.000000 wagtail-cjkcms-23.3.1/cjkcms/templatetags/auth_extras.py
--rw-r--r--   0 grze      (1000) grze      (1000)     6684 2023-02-20 22:56:25.000000 wagtail-cjkcms-23.3.1/cjkcms/templatetags/cjkcms_tags.py
--rw-r--r--   0 grze      (1000) grze      (1000)     4962 2022-10-08 15:53:44.000000 wagtail-cjkcms-23.3.1/cjkcms/templatetags/friendly_loader.py
--rw-r--r--   0 grze      (1000) grze      (1000)     1127 2023-02-11 16:38:37.000000 wagtail-cjkcms-23.3.1/cjkcms/templatetags/gravatar.py
--rw-r--r--   0 grze      (1000) grze      (1000)     1224 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/templatetags/txtutils_tags.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-03-12 10:10:56.513049 wagtail-cjkcms-23.3.1/cjkcms/tests/
--rw-r--r--   0 grze      (1000) grze      (1000)        0 2022-10-08 16:21:48.000000 wagtail-cjkcms-23.3.1/cjkcms/tests/__init__.py
--rw-r--r--   0 grze      (1000) grze      (1000)     4228 2023-02-11 16:38:36.000000 wagtail-cjkcms-23.3.1/cjkcms/tests/test_articlepages.py
--rw-r--r--   0 grze      (1000) grze      (1000)     2629 2022-10-08 16:06:08.000000 wagtail-cjkcms-23.3.1/cjkcms/tests/test_gravatar.py
--rw-r--r--   0 grze      (1000) grze      (1000)     4639 2023-02-11 16:38:35.000000 wagtail-cjkcms-23.3.1/cjkcms/tests/test_search_blocks.py
--rw-r--r--   0 grze      (1000) grze      (1000)     2665 2023-02-11 16:38:34.000000 wagtail-cjkcms-23.3.1/cjkcms/tests/test_settings.py
--rw-r--r--   0 grze      (1000) grze      (1000)     3511 2023-02-20 23:01:01.000000 wagtail-cjkcms-23.3.1/cjkcms/tests/test_templatetags.py
--rw-r--r--   0 grze      (1000) grze      (1000)     2678 2023-02-11 16:38:32.000000 wagtail-cjkcms-23.3.1/cjkcms/tests/test_urls.py
--rw-r--r--   0 grze      (1000) grze      (1000)     1522 2023-02-11 16:38:30.000000 wagtail-cjkcms-23.3.1/cjkcms/tests/test_webpage.py
--rw-r--r--   0 grze      (1000) grze      (1000)      506 2023-02-11 18:51:48.000000 wagtail-cjkcms-23.3.1/cjkcms/urls.py
--rw-r--r--   0 grze      (1000) grze      (1000)      573 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/utils.py
--rw-r--r--   0 grze      (1000) grze      (1000)     4488 2022-10-08 15:10:04.000000 wagtail-cjkcms-23.3.1/cjkcms/views.py
--rw-r--r--   0 grze      (1000) grze      (1000)     6211 2023-02-21 10:30:15.000000 wagtail-cjkcms-23.3.1/cjkcms/wagtail_hooks.py
--rw-r--r--   0 grze      (1000) grze      (1000)     1531 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/cjkcms/widgets.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-03-12 10:10:56.513049 wagtail-cjkcms-23.3.1/docs/
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-03-12 10:10:56.513049 wagtail-cjkcms-23.3.1/docs/how-to/
--rw-r--r--   0 grze      (1000) grze      (1000)     1481 2022-10-08 16:32:05.000000 wagtail-cjkcms-23.3.1/docs/how-to/oembed_finder.md
--rw-r--r--   0 grze      (1000) grze      (1000)      530 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/docs/index.md
--rw-r--r--   0 grze      (1000) grze      (1000)     4690 2022-11-12 15:47:30.000000 wagtail-cjkcms-23.3.1/docs/installation.md
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-03-12 10:10:56.513049 wagtail-cjkcms-23.3.1/docs/management_commands/
--rw-r--r--   0 grze      (1000) grze      (1000)      318 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/docs/management_commands/clear-embeds.md
--rw-r--r--   0 grze      (1000) grze      (1000)      193 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/docs/management_commands/index.md
--rw-r--r--   0 grze      (1000) grze      (1000)      420 2022-10-08 16:31:47.000000 wagtail-cjkcms-23.3.1/docs/management_commands/init-collections.md
--rw-r--r--   0 grze      (1000) grze      (1000)     3253 2022-11-12 15:48:02.000000 wagtail-cjkcms-23.3.1/docs/quick-start.md
--rw-r--r--   0 grze      (1000) grze      (1000)     1220 2022-10-08 16:30:54.000000 wagtail-cjkcms-23.3.1/docs/why-another-cms.md
--rw-r--r--   0 grze      (1000) grze      (1000)       93 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/pyproject.toml
--rw-r--r--   0 grze      (1000) grze      (1000)     1541 2023-03-12 10:10:56.513049 wagtail-cjkcms-23.3.1/setup.cfg
--rw-r--r--   0 grze      (1000) grze      (1000)       38 2022-09-01 08:26:22.000000 wagtail-cjkcms-23.3.1/setup.py
-drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-03-12 10:10:56.513049 wagtail-cjkcms-23.3.1/wagtail_cjkcms.egg-info/
--rw-r--r--   0 grze      (1000) grze      (1000)     2828 2023-03-12 10:10:56.000000 wagtail-cjkcms-23.3.1/wagtail_cjkcms.egg-info/PKG-INFO
--rw-r--r--   0 grze      (1000) grze      (1000)     9845 2023-03-12 10:10:56.000000 wagtail-cjkcms-23.3.1/wagtail_cjkcms.egg-info/SOURCES.txt
--rw-r--r--   0 grze      (1000) grze      (1000)        1 2023-03-12 10:10:56.000000 wagtail-cjkcms-23.3.1/wagtail_cjkcms.egg-info/dependency_links.txt
--rw-r--r--   0 grze      (1000) grze      (1000)       50 2023-03-12 10:10:56.000000 wagtail-cjkcms-23.3.1/wagtail_cjkcms.egg-info/entry_points.txt
--rw-r--r--   0 grze      (1000) grze      (1000)       79 2023-03-12 10:10:56.000000 wagtail-cjkcms-23.3.1/wagtail_cjkcms.egg-info/requires.txt
--rw-r--r--   0 grze      (1000) grze      (1000)        7 2023-03-12 10:10:56.000000 wagtail-cjkcms-23.3.1/wagtail_cjkcms.egg-info/top_level.txt
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.924526 wagtail-cjkcms-23.4.1/
+-rw-r--r--   0 grze      (1000) grze      (1000)     6374 2023-04-16 16:25:02.000000 wagtail-cjkcms-23.4.1/CHANGELOG.md
+-rw-r--r--   0 grze      (1000) grze      (1000)     1542 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/LICENSE
+-rw-r--r--   0 grze      (1000) grze      (1000)      239 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/MANIFEST.in
+-rw-r--r--   0 grze      (1000) grze      (1000)     2847 2023-04-16 16:31:36.924526 wagtail-cjkcms-23.4.1/PKG-INFO
+-rw-r--r--   0 grze      (1000) grze      (1000)     1688 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/README.md
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.874526 wagtail-cjkcms-23.4.1/cjkcms/
+-rw-r--r--   0 grze      (1000) grze      (1000)      272 2023-04-16 16:23:34.000000 wagtail-cjkcms-23.4.1/cjkcms/__init__.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.874526 wagtail-cjkcms-23.4.1/cjkcms/api/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/api/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     2832 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/api/mailchimp.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      173 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/apps.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.874526 wagtail-cjkcms-23.4.1/cjkcms/bin/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/bin/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     5752 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/bin/cjkcms.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.874526 wagtail-cjkcms-23.4.1/cjkcms/blocks/
+-rw-r--r--   0 grze      (1000) grze      (1000)     3166 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/blocks/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)    10455 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/blocks/base_blocks.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     8476 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/blocks/content_blocks.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     9292 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/blocks/html_blocks.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     3337 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/blocks/layout_blocks.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      171 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/blocks/searchable_html_block.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.874526 wagtail-cjkcms-23.4.1/cjkcms/draftail/
+-rw-r--r--   0 grze      (1000) grze      (1000)      305 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/draftail/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     3157 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/draftail/draftail_extensions.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     5157 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/draftail/draftail_icons.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     3191 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/fields.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.874526 wagtail-cjkcms-23.4.1/cjkcms/finders/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/finders/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     2459 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/finders/oembed.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      361 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/forms.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     1804 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/image_formats.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.854526 wagtail-cjkcms-23.4.1/cjkcms/management/
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.884526 wagtail-cjkcms-23.4.1/cjkcms/management/commands/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/management/commands/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      453 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/management/commands/clear-embeds.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     2565 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/management/commands/import-csv.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      952 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/management/commands/init-collections.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     3560 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/management/commands/init-navbar.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     3820 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/management/commands/init-website.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.884526 wagtail-cjkcms-23.4.1/cjkcms/migrations/
+-rw-r--r--   0 grze      (1000) grze      (1000)   216350 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/migrations/0001_initial.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      835 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/migrations/0002_alter_body_to_cjkcmsstreamfield.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      668 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/migrations/0003_alter_footer_content_alter_navbar_menu_items.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     1027 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/migrations/0004_layoutsettings_articles_date_format_and_more.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     1709 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/migrations/0005_layoutsettings_custom_font_and_more.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     2886 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/migrations/0006_analyticssettings_consent_modal_layout_and_more.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      594 2023-04-16 16:02:39.000000 wagtail-cjkcms-23.4.1/cjkcms/migrations/0007_layoutsettings_bootstrap_icons.py
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/migrations/__init__.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.884526 wagtail-cjkcms-23.4.1/cjkcms/models/
+-rw-r--r--   0 grze      (1000) grze      (1000)      232 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/models/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      395 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/models/admin_sidebar.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     2356 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/models/cms_models.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     6302 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/models/integration_models.py
+-rw-r--r--   0 grze      (1000) grze      (1000)    19651 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/models/page_models.py
+-rw-r--r--   0 grze      (1000) grze      (1000)    12522 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/models/snippet_models.py
+-rw-r--r--   0 grze      (1000) grze      (1000)    18294 2023-04-16 16:01:13.000000 wagtail-cjkcms-23.4.1/cjkcms/models/wagtailsettings_models.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      125 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/search_urls.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     9215 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/settings.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.864526 wagtail-cjkcms-23.4.1/cjkcms/static/
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.864526 wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.884526 wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/bi/
+-rw-r--r--   0 grze      (1000) grze      (1000)    93729 2023-04-03 17:02:22.000000 wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/bi/bootstrap-icons.css
+-rw-r--r--   0 grze      (1000) grze      (1000)    49971 2023-04-03 17:02:22.000000 wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/bi/bootstrap-icons.json
+-rw-r--r--   0 grze      (1000) grze      (1000)    55169 2023-04-03 17:02:22.000000 wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/bi/bootstrap-icons.scss
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.884526 wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/bi/fonts/
+-rw-r--r--   0 grze      (1000) grze      (1000)   164360 2023-04-03 17:02:22.000000 wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/bi/fonts/bootstrap-icons.woff
+-rw-r--r--   0 grze      (1000) grze      (1000)   121340 2023-04-03 17:02:22.000000 wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/bi/fonts/bootstrap-icons.woff2
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.884526 wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/css/
+-rw-r--r--   0 grze      (1000) grze      (1000)      846 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/css/cjkcms-admin.css
+-rw-r--r--   0 grze      (1000) grze      (1000)     1039 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/css/cjkcms-editor.css
+-rw-r--r--   0 grze      (1000) grze      (1000)     4375 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/css/cjkcms-front.css
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.864526 wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/images/
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.884526 wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/images/avatars/
+-rw-r--r--   0 grze      (1000) grze      (1000)      535 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/images/avatars/default.png
+-rw-r--r--   0 grze      (1000) grze      (1000)      384 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/images/avatars/default.svg
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.884526 wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/images/icons/
+-rw-r--r--   0 grze      (1000) grze      (1000)      705 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/images/icons/quote.svg
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.884526 wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/images/logos/
+-rw-r--r--   0 grze      (1000) grze      (1000)     4166 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/images/logos/cms-logo-long.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)     4218 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/images/logos/cms-logo-square.svg
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.884526 wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/images/patterns/
+-rw-r--r--   0 grze      (1000) grze      (1000)    47935 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/images/patterns/pattern1.jpg
+-rw-r--r--   0 grze      (1000) grze      (1000)    31707 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/images/patterns/pattern2.jpg
+-rw-r--r--   0 grze      (1000) grze      (1000)    38190 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/images/patterns/pattern3.jpg
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.894526 wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/js/
+-rw-r--r--   0 grze      (1000) grze      (1000)      444 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/js/cjkcms-editor.js
+-rw-r--r--   0 grze      (1000) grze      (1000)     5780 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/js/cjkcms-front.js
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.894526 wagtail-cjkcms-23.4.1/cjkcms/static/cookieconsent/
+-rw-r--r--   0 grze      (1000) grze      (1000)    18803 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/static/cookieconsent/cookieconsent.css
+-rw-r--r--   0 grze      (1000) grze      (1000)    18743 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/static/cookieconsent/cookieconsent.js
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.894526 wagtail-cjkcms-23.4.1/cjkcms/templates/
+-rw-r--r--   0 grze      (1000) grze      (1000)     4176 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/404.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     4802 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/500.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.894526 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.904526 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/
+-rw-r--r--   0 grze      (1000) grze      (1000)     1443 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/accordion_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      974 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/article_block_card.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1132 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/article_masonry_card.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      188 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/base_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     2505 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/base_link_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      740 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/button_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      746 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/card_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      856 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/card_blurb.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      786 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/card_foot.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      730 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/card_head.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      771 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/card_head_foot.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      990 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/card_horizontal.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1104 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/card_horizontal2.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      786 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/card_img.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     2618 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/card_landing1.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     2758 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/card_landing2.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      678 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/cardgrid_columns.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      450 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/cardgrid_deck.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      277 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/cardgrid_group.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      276 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/cardgrid_zero.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     2698 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/carousel_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      406 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/column_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      137 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/document_link_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      920 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/download_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      103 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/embed_video_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)       95 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/external_link_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      424 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/grid_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      200 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/h1_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      200 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/h2_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      200 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/h3_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      790 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/hero_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      275 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/image_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1400 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/image_gallery_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      627 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/image_link_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1020 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/modal_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      164 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/page_link_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      787 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/pagelist_article_card_columns.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      642 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/pagelist_article_card_deck.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      361 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/pagelist_article_card_group.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      956 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/pagelist_article_media.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      397 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/pagelist_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      610 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/pagelist_list_group.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1224 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/pagelist_toc_nextprev.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      300 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/pagepreview_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      793 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/pagepreview_card.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1065 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/pagepreview_form.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      244 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/pricelist_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      513 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/pricelistitem_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      353 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/quote_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      852 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/quote_block_leftbar.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      998 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/quote_block_start_end_quote.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      216 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/reusable_content_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)       91 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/rich_text_block.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1095 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/table_block.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.904526 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/cookieconsent/
+-rw-r--r--   0 grze      (1000) grze      (1000)     3672 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/cookieconsent/languages.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.904526 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/formfields/
+-rw-r--r--   0 grze      (1000) grze      (1000)      267 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/formfields/date.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      416 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/formfields/datetime.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.904526 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/formfields/mailchimp/
+-rw-r--r--   0 grze      (1000) grze      (1000)     9267 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/formfields/mailchimp/_2vanilla_subscriber_integration_js.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     6469 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/formfields/mailchimp/subscriber_integration_js.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      793 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/formfields/mailchimp/subscriber_integration_widget.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      264 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/formfields/time.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.914526 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/icons/
+-rw-r--r--   0 grze      (1000) grze      (1000)      465 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/icons/align-left.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      573 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/icons/check-square-o.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      277 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/icons/columns.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      359 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/icons/desktop.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      571 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/icons/font.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      292 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/icons/google.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      813 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/icons/hand-pointer-o.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      666 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/icons/hashtag.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      840 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/icons/header.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      835 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/icons/list-alt.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      459 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/icons/map.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      448 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/icons/newspaper-o.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      721 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/icons/puzzle-piece.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      635 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/icons/recycle.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      174 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/icons/stop.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      505 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/icons/th-large.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      762 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/icons/universal-access.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      548 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/icons/usd.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      225 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/icons/window-maximize.svg
+-rw-r--r--   0 grze      (1000) grze      (1000)      199 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/icons/window-minimize.svg
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.914526 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/includes/
+-rw-r--r--   0 grze      (1000) grze      (1000)      286 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/includes/cjkcms_banner.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      689 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/includes/classifier_dropdowns.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      579 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/includes/classifier_nav.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      286 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/includes/codered_banner.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      268 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/includes/form_honeypot.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1061 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/includes/pagination.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.914526 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/includes/stream_forms/
+-rw-r--r--   0 grze      (1000) grze      (1000)      532 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/includes/stream_forms/render_field.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.914526 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/pages/
+-rw-r--r--   0 grze      (1000) grze      (1000)     2002 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/pages/article_index_page.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1705 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/pages/article_page.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1018 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/pages/article_page.search.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     7931 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/pages/base.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1104 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/pages/form_page.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      248 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/pages/form_page_landing.html
+-rw-r--r--   0 grze      (1000) grze      (1000)       50 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/pages/home_page.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     2610 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/pages/search.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      582 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/pages/search_result.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     2462 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/pages/stream_form_page.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      838 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/pages/web_page.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      623 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/pages/web_page_notitle.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      122 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/robots.txt
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.914526 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/snippets/
+-rw-r--r--   0 grze      (1000) grze      (1000)      430 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/snippets/footer.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     2027 2023-04-16 16:13:17.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/snippets/frontend_assets.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     1196 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/snippets/frontend_scripts.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      836 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/snippets/lang_selector.html
+-rw-r--r--   0 grze      (1000) grze      (1000)     2586 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/snippets/navbar.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      386 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/snippets/navbar_search.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      158 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/snippets/tracking_g3.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      831 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/snippets/tracking_g4.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.914526 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/widgets/
+-rw-r--r--   0 grze      (1000) grze      (1000)     1384 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/widgets/checkbox_classifiers.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.864526 wagtail-cjkcms-23.4.1/cjkcms/templates/wagtailadmin/
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.914526 wagtail-cjkcms-23.4.1/cjkcms/templates/wagtailadmin/block_forms/
+-rw-r--r--   0 grze      (1000) grze      (1000)      754 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/wagtailadmin/block_forms/base_block_settings_struct.html
+-rw-r--r--   0 grze      (1000) grze      (1000)      550 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/wagtailadmin/block_forms/struct.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.914526 wagtail-cjkcms-23.4.1/cjkcms/templates/wagtailadmin/shared/
+-rw-r--r--   0 grze      (1000) grze      (1000)      885 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templates/wagtailadmin/shared/cr_main_nav_2fix.html
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.924526 wagtail-cjkcms-23.4.1/cjkcms/templatetags/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templatetags/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      327 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templatetags/auth_extras.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     6684 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templatetags/cjkcms_tags.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     4962 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templatetags/friendly_loader.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     1127 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templatetags/gravatar.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     1224 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/templatetags/txtutils_tags.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.924526 wagtail-cjkcms-23.4.1/cjkcms/tests/
+-rw-r--r--   0 grze      (1000) grze      (1000)        0 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/tests/__init__.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     4228 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/tests/test_articlepages.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     2629 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/tests/test_gravatar.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     4639 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/tests/test_search_blocks.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     2665 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/tests/test_settings.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     3511 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/tests/test_templatetags.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     2678 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/tests/test_urls.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     1522 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/tests/test_webpage.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      506 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/urls.py
+-rw-r--r--   0 grze      (1000) grze      (1000)      573 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/utils.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     4488 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/views.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     6211 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/wagtail_hooks.py
+-rw-r--r--   0 grze      (1000) grze      (1000)     1531 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/cjkcms/widgets.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.924526 wagtail-cjkcms-23.4.1/docs/
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.924526 wagtail-cjkcms-23.4.1/docs/how-to/
+-rw-r--r--   0 grze      (1000) grze      (1000)     1481 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/docs/how-to/oembed_finder.md
+-rw-r--r--   0 grze      (1000) grze      (1000)      537 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/docs/index.md
+-rw-r--r--   0 grze      (1000) grze      (1000)     5520 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/docs/installation.md
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.924526 wagtail-cjkcms-23.4.1/docs/management_commands/
+-rw-r--r--   0 grze      (1000) grze      (1000)      318 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/docs/management_commands/clear-embeds.md
+-rw-r--r--   0 grze      (1000) grze      (1000)      193 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/docs/management_commands/index.md
+-rw-r--r--   0 grze      (1000) grze      (1000)      420 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/docs/management_commands/init-collections.md
+-rw-r--r--   0 grze      (1000) grze      (1000)      936 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/docs/quick-start.md
+-rw-r--r--   0 grze      (1000) grze      (1000)       13 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/docs/requirements.txt
+-rw-r--r--   0 grze      (1000) grze      (1000)     1220 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/docs/why-another-cms.md
+-rw-r--r--   0 grze      (1000) grze      (1000)       93 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/pyproject.toml
+-rw-r--r--   0 grze      (1000) grze      (1000)     1541 2023-04-16 16:31:36.924526 wagtail-cjkcms-23.4.1/setup.cfg
+-rw-r--r--   0 grze      (1000) grze      (1000)       38 2023-04-16 15:48:31.000000 wagtail-cjkcms-23.4.1/setup.py
+drwxr-xr-x   0 grze      (1000) grze      (1000)        0 2023-04-16 16:31:36.924526 wagtail-cjkcms-23.4.1/wagtail_cjkcms.egg-info/
+-rw-r--r--   0 grze      (1000) grze      (1000)     2847 2023-04-16 16:31:36.000000 wagtail-cjkcms-23.4.1/wagtail_cjkcms.egg-info/PKG-INFO
+-rw-r--r--   0 grze      (1000) grze      (1000)     9351 2023-04-16 16:31:36.000000 wagtail-cjkcms-23.4.1/wagtail_cjkcms.egg-info/SOURCES.txt
+-rw-r--r--   0 grze      (1000) grze      (1000)        1 2023-04-16 16:31:36.000000 wagtail-cjkcms-23.4.1/wagtail_cjkcms.egg-info/dependency_links.txt
+-rw-r--r--   0 grze      (1000) grze      (1000)       51 2023-04-16 16:31:36.000000 wagtail-cjkcms-23.4.1/wagtail_cjkcms.egg-info/entry_points.txt
+-rw-r--r--   0 grze      (1000) grze      (1000)       79 2023-04-16 16:31:36.000000 wagtail-cjkcms-23.4.1/wagtail_cjkcms.egg-info/requires.txt
+-rw-r--r--   0 grze      (1000) grze      (1000)        7 2023-04-16 16:31:36.000000 wagtail-cjkcms-23.4.1/wagtail_cjkcms.egg-info/top_level.txt
```

### Comparing `wagtail-cjkcms-23.3.1/CHANGELOG.md` & `wagtail-cjkcms-23.4.1/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -160,8 +160,11 @@
 - Removed unnecessary requirement re: wagtail 4.2 from migration 0006
 
 # 23.2.6 (2023-02-23)
 - Fixed problem with migration broken by 23.2.5
 
 # 23.3.1 (2023-03-12)
 - Added "cjkcms start [projectname]" command to create a new project with wagtail-cjkcms installed
-- 
+
+# 23.4.1 (2023-04-16)
+- Added new layout setting (bootstrap_icon) + static files to load Bootstrap icons css+woff locally.
+- Modified frontend_assets template to load bootstrap icons if set.
```

### Comparing `wagtail-cjkcms-23.3.1/LICENSE` & `wagtail-cjkcms-23.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/PKG-INFO` & `wagtail-cjkcms-23.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: wagtail-cjkcms
-Version: 23.3.1
+Version: 23.4.1
 Summary: Wagtail Content Management System, installable as a Django app into any Wagtail 4.x site. Based on Codered CRX.
 Home-page: https://github.com/cjkpl/wagtail-cjkcms
 Author: Grzegorz Krol
 Author-email: gk@cjk.pl
 License: BSD-3-Clause  # Example license
+Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Wagtail :: 4
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -49,7 +50,8 @@
 pytest ../wagtail-cjkcms/cjkcms --ds=devsite.settings.dev --doctest-modules --durations=0
 
 ### running pytest from testproject folder:
 pytest ../cjkcms --ds=testproject.settings.dev --doctest-modules --durations=0
 
 ## Contact & support
 Please use [Github's Issue Tracker](https://github.com/cjkpl/wagtail-cjkcms/issues) to report bugs, request features, or request support.
+
```

### Comparing `wagtail-cjkcms-23.3.1/README.md` & `wagtail-cjkcms-23.4.1/README.md`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/api/mailchimp.py` & `wagtail-cjkcms-23.4.1/cjkcms/api/mailchimp.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/bin/cjkcms.py` & `wagtail-cjkcms-23.4.1/cjkcms/bin/cjkcms.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/blocks/__init__.py` & `wagtail-cjkcms-23.4.1/cjkcms/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/blocks/base_blocks.py` & `wagtail-cjkcms-23.4.1/cjkcms/blocks/base_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/blocks/content_blocks.py` & `wagtail-cjkcms-23.4.1/cjkcms/blocks/content_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/blocks/html_blocks.py` & `wagtail-cjkcms-23.4.1/cjkcms/blocks/html_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/blocks/layout_blocks.py` & `wagtail-cjkcms-23.4.1/cjkcms/blocks/layout_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/draftail/draftail_extensions.py` & `wagtail-cjkcms-23.4.1/cjkcms/draftail/draftail_extensions.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/draftail/draftail_icons.py` & `wagtail-cjkcms-23.4.1/cjkcms/draftail/draftail_icons.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/fields.py` & `wagtail-cjkcms-23.4.1/cjkcms/fields.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/finders/oembed.py` & `wagtail-cjkcms-23.4.1/cjkcms/finders/oembed.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/image_formats.py` & `wagtail-cjkcms-23.4.1/cjkcms/image_formats.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/management/commands/__pycache__/init-collections.cpython-310.pyc` & `wagtail-cjkcms-23.4.1/cjkcms/management/commands/init-collections.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,76 +1,60 @@
-00000000: 6f0d 0d0a 0000 0000 0083 f162 c403 0000  o..........b....
-00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 3000 0000 6400  .....@...s0...d.
-00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
-00000040: 6402 6c03 6d04 5a04 0100 4700 6403 6404  d.l.m.Z...G.d.d.
-00000050: 8400 6404 6501 8303 5a05 6405 5300 2906  ..d.e...Z.d.S.).
-00000060: e900 0000 0029 02da 0b42 6173 6543 6f6d  .....)...BaseCom
-00000070: 6d61 6e64 da0c 436f 6d6d 616e 6445 7272  mand..CommandErr
-00000080: 6f72 2901 da0a 436f 6c6c 6563 7469 6f6e  or)...Collection
-00000090: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-000000a0: 0002 0000 0040 0000 0073 1c00 0000 6500  .....@...s....e.
-000000b0: 5a01 6400 5a02 6401 5a03 6402 5a04 6403  Z.d.Z.d.Z.d.Z.d.
-000000c0: 6404 8400 5a05 6405 5300 2906 da07 436f  d...Z.d.S.)...Co
-000000d0: 6d6d 616e 647a 7943 7265 6174 6520 6120  mmandzyCreate a 
-000000e0: 7365 7420 6f66 2063 6f6d 6d6f 6e6c 7920  set of commonly 
-000000f0: 7573 6564 2063 6f6c 6c65 6374 696f 6e73  used collections
-00000100: 2066 6f72 2061 206e 6577 2077 6562 7369   for a new websi
-00000110: 7465 3a0a 2020 2020 636f 7665 7273 2c20  te:.    covers, 
-00000120: 6c6f 676f 732c 2072 6573 6f75 7263 6573  logos, resources
-00000130: 2c20 7065 6f70 6c65 2c20 6172 7469 636c  , people, articl
-00000140: 6573 2c20 6361 7264 732c 2069 636f 6e73  es, cards, icons
-00000150: 7a63 4372 6561 7465 2061 2073 6574 206f  zcCreate a set o
-00000160: 6620 636f 6d6d 6f6e 6c79 2075 7365 6420  f commonly used 
-00000170: 636f 6c6c 6563 7469 6f6e 733a 2063 6f76  collections: cov
-00000180: 6572 732c 206c 6f67 6f73 2c20 7265 736f  ers, logos, reso
-00000190: 7572 6365 732c 2070 656f 706c 652c 2061  urces, people, a
-000001a0: 7274 6963 6c65 732c 2063 6172 6473 2c20  rticles, cards, 
-000001b0: 6963 6f6e 7363 0100 0000 0000 0000 0000  iconsc..........
-000001c0: 0000 0600 0000 0600 0000 4f00 0000 736c  ..........O...sl
-000001d0: 0000 0067 0064 01a2 017d 0374 00a0 01a1  ...g.d...}.t....
-000001e0: 007d 047c 0473 0c64 0053 007c 0344 005d  .}.|.s.d.S.|.D.]
-000001f0: 257d 0574 006a 026a 037c 0564 028d 01a0  %}.t.j.j.|.d....
-00000200: 04a1 0072 247c 006a 05a0 0664 037c 059b  ...r$|.j...d.|..
-00000210: 0064 049d 03a1 0101 0071 0e7c 046a 077c  .d.......q.|.j.|
-00000220: 0564 028d 0101 007c 006a 05a0 0664 057c  .d.....|.j...d.|
-00000230: 059b 009d 02a1 0101 0071 0e64 0053 0029  .........q.d.S.)
-00000240: 064e 2907 5a06 436f 7665 7273 5a05 4c6f  .N).Z.CoversZ.Lo
-00000250: 676f 735a 0952 6573 6f75 7263 6573 5a06  gosZ.ResourcesZ.
-00000260: 5065 6f70 6c65 5a08 4172 7469 636c 6573  PeopleZ.Articles
-00000270: 5a05 4361 7264 735a 0549 636f 6e73 2901  Z.CardsZ.Icons).
-00000280: da04 6e61 6d65 7a0b 436f 6c6c 6563 7469  ..namez.Collecti
-00000290: 6f6e 207a 2320 616c 7265 6164 7920 6578  on z# already ex
-000002a0: 6973 7473 2c20 736b 6970 7069 6e67 2063  ists, skipping c
-000002b0: 7265 6174 696f 6e2e 7a13 4372 6561 7465  reation.z.Create
-000002c0: 6420 636f 6c6c 6563 7469 6f6e 2029 0872  d collection ).r
-000002d0: 0400 0000 da13 6765 745f 6669 7273 745f  ......get_first_
-000002e0: 726f 6f74 5f6e 6f64 65da 076f 626a 6563  root_node..objec
-000002f0: 7473 da06 6669 6c74 6572 da06 6578 6973  ts..filter..exis
-00000300: 7473 da06 7374 646f 7574 da05 7772 6974  ts..stdout..writ
-00000310: 65da 0961 6464 5f63 6869 6c64 2906 da04  e..add_child)...
-00000320: 7365 6c66 da04 6172 6773 da07 6f70 7469  self..args..opti
-00000330: 6f6e 73da 056e 616d 6573 5a09 726f 6f74  ons..namesZ.root
-00000340: 5f63 6f6c 6cda 016e a900 7213 0000 00fa  _coll..n..r.....
-00000350: 532f 686f 6d65 2f67 727a 652f 6370 7974  S/home/grze/cpyt
-00000360: 686f 6e2f 636d 732f 646a 616e 676f 2d63  hon/cms/django-c
-00000370: 6a6b 636d 732f 636a 6b63 6d73 2f6d 616e  jkcms/cjkcms/man
-00000380: 6167 656d 656e 742f 636f 6d6d 616e 6473  agement/commands
-00000390: 2f69 6e69 742d 636f 6c6c 6563 7469 6f6e  /init-collection
-000003a0: 732e 7079 da06 6861 6e64 6c65 0b00 0000  s.py..handle....
-000003b0: 7316 0000 0008 0108 0404 0204 0208 0212  s...............
-000003c0: 0114 0102 010c 0114 0104 fb7a 0e43 6f6d  ...........z.Com
-000003d0: 6d61 6e64 2e68 616e 646c 654e 2906 da08  mand.handleN)...
-000003e0: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
-000003f0: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
-00000400: 5f5f da07 5f5f 646f 635f 5fda 0468 656c  __..__doc__..hel
-00000410: 7072 1500 0000 7213 0000 0072 1300 0000  pr....r....r....
-00000420: 7213 0000 0072 1400 0000 7205 0000 0005  r....r....r.....
-00000430: 0000 0073 0800 0000 0800 0401 0403 0c02  ...s............
-00000440: 7205 0000 004e 2906 da1b 646a 616e 676f  r....N)...django
-00000450: 2e63 6f72 652e 6d61 6e61 6765 6d65 6e74  .core.management
-00000460: 2e62 6173 6572 0200 0000 7203 0000 00da  .baser....r.....
-00000470: 1377 6167 7461 696c 2e63 6f72 652e 6d6f  .wagtail.core.mo
-00000480: 6465 6c73 7204 0000 0072 0500 0000 7213  delsr....r....r.
-00000490: 0000 0072 1300 0000 7213 0000 0072 1400  ...r....r....r..
-000004a0: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-000004b0: 7306 0000 0010 000c 0114 03              s..........
+00000000: 6672 6f6d 2064 6a61 6e67 6f2e 636f 7265  from django.core
+00000010: 2e6d 616e 6167 656d 656e 742e 6261 7365  .management.base
+00000020: 2069 6d70 6f72 7420 4261 7365 436f 6d6d   import BaseComm
+00000030: 616e 640a 6672 6f6d 2077 6167 7461 696c  and.from wagtail
+00000040: 2e6d 6f64 656c 7320 696d 706f 7274 2043  .models import C
+00000050: 6f6c 6c65 6374 696f 6e0a 0a0a 636c 6173  ollection...clas
+00000060: 7320 436f 6d6d 616e 6428 4261 7365 436f  s Command(BaseCo
+00000070: 6d6d 616e 6429 3a0a 2020 2020 2222 2243  mmand):.    """C
+00000080: 7265 6174 6520 6120 7365 7420 6f66 2063  reate a set of c
+00000090: 6f6d 6d6f 6e6c 7920 7573 6564 2063 6f6c  ommonly used col
+000000a0: 6c65 6374 696f 6e73 2066 6f72 2061 206e  lections for a n
+000000b0: 6577 2077 6562 7369 7465 3a0a 2020 2020  ew website:.    
+000000c0: 636f 7665 7273 2c20 6c6f 676f 732c 2072  covers, logos, r
+000000d0: 6573 6f75 7263 6573 2c20 7065 6f70 6c65  esources, people
+000000e0: 2c20 6172 7469 636c 6573 2c20 6361 7264  , articles, card
+000000f0: 732c 2069 636f 6e73 2222 220a 0a20 2020  s, icons"""..   
+00000100: 2068 656c 7020 3d20 2243 7265 6174 6520   help = "Create 
+00000110: 6120 7365 7420 6f66 2063 6f6d 6d6f 6e6c  a set of commonl
+00000120: 7920 7573 6564 2063 6f6c 6c65 6374 696f  y used collectio
+00000130: 6e73 3a20 220a 2020 2020 2263 6f76 6572  ns: ".    "cover
+00000140: 732c 206c 6f67 6f73 2c20 7265 736f 7572  s, logos, resour
+00000150: 6365 732c 2070 656f 706c 652c 2061 7274  ces, people, art
+00000160: 6963 6c65 732c 2063 6172 6473 2c20 6963  icles, cards, ic
+00000170: 6f6e 7322 0a0a 2020 2020 6465 6620 6861  ons"..    def ha
+00000180: 6e64 6c65 2873 656c 662c 202a 6172 6773  ndle(self, *args
+00000190: 2c20 2a2a 6f70 7469 6f6e 7329 3a0a 2020  , **options):.  
+000001a0: 2020 2020 2020 6e61 6d65 7320 3d20 5b22        names = ["
+000001b0: 436f 7665 7273 222c 2022 4c6f 676f 7322  Covers", "Logos"
+000001c0: 2c20 2252 6573 6f75 7263 6573 222c 2022  , "Resources", "
+000001d0: 5065 6f70 6c65 222c 2022 4172 7469 636c  People", "Articl
+000001e0: 6573 222c 2022 4361 7264 7322 2c20 2249  es", "Cards", "I
+000001f0: 636f 6e73 225d 0a0a 2020 2020 2020 2020  cons"]..        
+00000200: 2320 7472 7920 6372 6561 7469 6e67 2063  # try creating c
+00000210: 6f6c 6c65 6374 696f 6e2c 2069 6620 646f  ollection, if do
+00000220: 6573 206e 6f74 2065 7869 7374 0a0a 2020  es not exist..  
+00000230: 2020 2020 2020 726f 6f74 5f63 6f6c 6c20        root_coll 
+00000240: 3d20 436f 6c6c 6563 7469 6f6e 2e67 6574  = Collection.get
+00000250: 5f66 6972 7374 5f72 6f6f 745f 6e6f 6465  _first_root_node
+00000260: 2829 0a0a 2020 2020 2020 2020 6966 206e  ()..        if n
+00000270: 6f74 2072 6f6f 745f 636f 6c6c 3a0a 0a20  ot root_coll:.. 
+00000280: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00000290: 6e0a 0a20 2020 2020 2020 2066 6f72 206e  n..        for n
+000002a0: 2069 6e20 6e61 6d65 733a 0a20 2020 2020   in names:.     
+000002b0: 2020 2020 2020 2069 6620 436f 6c6c 6563         if Collec
+000002c0: 7469 6f6e 2e6f 626a 6563 7473 2e66 696c  tion.objects.fil
+000002d0: 7465 7228 6e61 6d65 3d6e 292e 6578 6973  ter(name=n).exis
+000002e0: 7473 2829 3a0a 2020 2020 2020 2020 2020  ts():.          
+000002f0: 2020 2020 2020 7365 6c66 2e73 7464 6f75        self.stdou
+00000300: 742e 7772 6974 6528 6622 436f 6c6c 6563  t.write(f"Collec
+00000310: 7469 6f6e 207b 6e7d 2061 6c72 6561 6479  tion {n} already
+00000320: 2065 7869 7374 732c 2073 6b69 7070 696e   exists, skippin
+00000330: 6720 6372 6561 7469 6f6e 2e22 290a 2020  g creation.").  
+00000340: 2020 2020 2020 2020 2020 2020 2020 636f                co
+00000350: 6e74 696e 7565 0a20 2020 2020 2020 2020  ntinue.         
+00000360: 2020 2072 6f6f 745f 636f 6c6c 2e61 6464     root_coll.add
+00000370: 5f63 6869 6c64 286e 616d 653d 6e29 0a20  _child(name=n). 
+00000380: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00000390: 7374 646f 7574 2e77 7269 7465 2866 2243  stdout.write(f"C
+000003a0: 7265 6174 6564 2063 6f6c 6c65 6374 696f  reated collectio
+000003b0: 6e20 7b6e 7d22 290a                      n {n}").
```

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/management/commands/import-csv.py` & `wagtail-cjkcms-23.4.1/cjkcms/management/commands/import-csv.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/management/commands/init-navbar.py` & `wagtail-cjkcms-23.4.1/cjkcms/management/commands/init-navbar.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/management/commands/init-website.py` & `wagtail-cjkcms-23.4.1/cjkcms/management/commands/init-website.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/migrations/0001_initial.py` & `wagtail-cjkcms-23.4.1/cjkcms/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/migrations/0002_alter_body_to_cjkcmsstreamfield.py` & `wagtail-cjkcms-23.4.1/cjkcms/migrations/0002_alter_body_to_cjkcmsstreamfield.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/migrations/0003_alter_footer_content_alter_navbar_menu_items.py` & `wagtail-cjkcms-23.4.1/cjkcms/migrations/0003_alter_footer_content_alter_navbar_menu_items.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/migrations/0004_layoutsettings_articles_date_format_and_more.py` & `wagtail-cjkcms-23.4.1/cjkcms/migrations/0004_layoutsettings_articles_date_format_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/migrations/0005_layoutsettings_custom_font_and_more.py` & `wagtail-cjkcms-23.4.1/cjkcms/migrations/0005_layoutsettings_custom_font_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/migrations/0006_analyticssettings_consent_modal_layout_and_more.py` & `wagtail-cjkcms-23.4.1/cjkcms/migrations/0006_analyticssettings_consent_modal_layout_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/models/cms_models.py` & `wagtail-cjkcms-23.4.1/cjkcms/models/cms_models.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/models/integration_models.py` & `wagtail-cjkcms-23.4.1/cjkcms/models/integration_models.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/models/page_models.py` & `wagtail-cjkcms-23.4.1/cjkcms/models/page_models.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/models/snippet_models.py` & `wagtail-cjkcms-23.4.1/cjkcms/models/snippet_models.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/models/wagtailsettings_models.py` & `wagtail-cjkcms-23.4.1/cjkcms/models/wagtailsettings_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,14 +196,20 @@
 
     awesome_cdn = models.BooleanField(
         default=False,
         verbose_name=_("Font Awesome"),
         help_text=_("Load font awesome from CDN"),
     )
 
+    bootstrap_icons = models.BooleanField(
+        default=False,
+        verbose_name=_("Bootstrap Icons CSS"),
+        help_text=_("Load bootstrap icons css from local/static folder"),
+    )
+
     custom_font = models.BooleanField(
         default=False,
         verbose_name=_("Use custom font"),
         help_text=_("Custom body font e.g. from CDN & include css body override"),
     )
 
     font_url = models.CharField(
@@ -277,14 +283,15 @@
             heading=_("Site Footers"),
         ),
         MultiFieldPanel(
             [
                 FieldPanel("frontend_theme"),
                 FieldPanel("base_template"),
                 FieldPanel("awesome_cdn"),
+                FieldPanel("bootstrap_icons"),
                 FieldPanel("custom_font"),
                 FieldPanel("font_url"),
                 FieldPanel("font_family"),
             ],
             heading=_("Theming"),
         ),
         MultiFieldPanel(
```

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/settings.py` & `wagtail-cjkcms-23.4.1/cjkcms/settings.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/static/cjkcms/css/cjkcms-admin.css` & `wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/css/cjkcms-admin.css`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/static/cjkcms/css/cjkcms-editor.css` & `wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/css/cjkcms-editor.css`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/static/cjkcms/css/cjkcms-front.css` & `wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/css/cjkcms-front.css`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/static/cjkcms/images/avatars/default.png` & `wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/images/avatars/default.png`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/static/cjkcms/images/icons/quote.svg` & `wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/images/icons/quote.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/static/cjkcms/images/logos/cms-logo-long.svg` & `wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/images/logos/cms-logo-long.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/static/cjkcms/images/logos/cms-logo-square.svg` & `wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/images/logos/cms-logo-square.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/static/cjkcms/images/patterns/pattern1.jpg` & `wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/images/patterns/pattern1.jpg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/static/cjkcms/images/patterns/pattern2.jpg` & `wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/images/patterns/pattern2.jpg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/static/cjkcms/images/patterns/pattern3.jpg` & `wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/images/patterns/pattern3.jpg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/static/cjkcms/js/cjkcms-front.js` & `wagtail-cjkcms-23.4.1/cjkcms/static/cjkcms/js/cjkcms-front.js`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/static/cookieconsent/cookieconsent.css` & `wagtail-cjkcms-23.4.1/cjkcms/static/cookieconsent/cookieconsent.css`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/static/cookieconsent/cookieconsent.js` & `wagtail-cjkcms-23.4.1/cjkcms/static/cookieconsent/cookieconsent.js`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/404.html` & `wagtail-cjkcms-23.4.1/cjkcms/templates/404.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/500.html` & `wagtail-cjkcms-23.4.1/cjkcms/templates/500.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/accordion_block.html` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/accordion_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/article_block_card.html` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/article_block_card.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/article_masonry_card.html` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/article_masonry_card.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/base_link_block.html` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/base_link_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/button_block.html` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/button_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/card_block.html` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/card_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/card_blurb.html` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/card_blurb.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/card_foot.html` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/card_foot.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/card_head.html` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/card_head.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/card_head_foot.html` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/card_head_foot.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/card_horizontal.html` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/card_horizontal.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/card_horizontal2.html` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/card_horizontal2.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/card_img.html` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/card_img.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/card_landing1.html` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/card_landing1.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/card_landing2.html` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/card_landing2.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/cardgrid_columns.html` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/cardgrid_columns.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/carousel_block.html` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/carousel_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/download_block.html` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/download_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/hero_block.html` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/hero_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/image_gallery_block.html` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/image_gallery_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/image_link_block.html` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/image_link_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/modal_block.html` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/modal_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/pagelist_article_card_columns.html` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/pagelist_article_card_columns.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/pagelist_article_card_deck.html` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/pagelist_article_card_deck.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/pagelist_article_media.html` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/pagelist_article_media.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/pagelist_list_group.html` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/pagelist_list_group.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/pagelist_toc_nextprev.html` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/pagelist_toc_nextprev.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/pagepreview_card.html` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/pagepreview_card.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/pagepreview_form.html` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/pagepreview_form.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/pricelistitem_block.html` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/pricelistitem_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/quote_block_leftbar.html` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/quote_block_leftbar.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/quote_block_start_end_quote.html` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/quote_block_start_end_quote.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/blocks/table_block.html` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/blocks/table_block.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/cookieconsent/languages.html` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/cookieconsent/languages.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/formfields/mailchimp/_2vanilla_subscriber_integration_js.html` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/formfields/mailchimp/_2vanilla_subscriber_integration_js.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/formfields/mailchimp/subscriber_integration_js.html` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/formfields/mailchimp/subscriber_integration_js.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/formfields/mailchimp/subscriber_integration_widget.html` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/formfields/mailchimp/subscriber_integration_widget.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/icons/check-square-o.svg` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/icons/check-square-o.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/icons/font.svg` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/icons/font.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/icons/hand-pointer-o.svg` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/icons/hand-pointer-o.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/icons/hashtag.svg` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/icons/hashtag.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/icons/header.svg` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/icons/header.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/icons/list-alt.svg` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/icons/list-alt.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/icons/puzzle-piece.svg` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/icons/puzzle-piece.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/icons/recycle.svg` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/icons/recycle.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/icons/universal-access.svg` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/icons/universal-access.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/icons/usd.svg` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/icons/usd.svg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/includes/classifier_dropdowns.html` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/includes/classifier_dropdowns.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/includes/classifier_nav.html` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/includes/classifier_nav.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/includes/pagination.html` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/includes/pagination.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/includes/stream_forms/render_field.html` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/includes/stream_forms/render_field.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/pages/article_index_page.html` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/pages/article_index_page.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/pages/article_page.html` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/pages/article_page.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/pages/article_page.search.html` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/pages/article_page.search.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/pages/base.html` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/pages/base.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/pages/form_page.html` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/pages/form_page.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/pages/search.html` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/pages/search.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/pages/search_result.html` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/pages/search_result.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/pages/stream_form_page.html` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/pages/stream_form_page.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/pages/web_page.html` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/pages/web_page.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/pages/web_page_notitle.html` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/pages/web_page_notitle.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/snippets/frontend_assets.html` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/snippets/frontend_assets.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-{% load friendly_loader wagtailcore_tags wagtailsettings_tags cjkcms_tags %}
+{% load friendly_loader wagtailcore_tags wagtailsettings_tags cjkcms_tags static %}
 {% friendly_load webpack_loader %}
     {% if settings.cjkcms.LayoutSettings.frontend_theme == 'python-webpack' %} {# use python-webpack from Michael Yin #}
         {% if_has_tag stylesheet_pack %}
             {% stylesheet_pack 'app' %}
         {% endif_has_tag %}
     {% elif settings.cjkcms.LayoutSettings.frontend_theme == 'mdb.light' %}
         <link
@@ -16,14 +16,21 @@
             crossorigin="anonymous">
     {% else %}
         <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha1/dist/css/bootstrap.min.css" 
             rel="stylesheet" 
             integrity="sha384-GLhlTQ8iRABdZLl6O3oVMWSktQOp6b7In1Zl3/Jr59b6EGGoI1aFkw7cmDA6j6gD" 
             crossorigin="anonymous">
     {% endif %}
+    {% if settings.cjkcms.LayoutSettings.bootstrap_icons %}
+        <!-- Bootstrap icons (local) -->
+        <link
+            href="{% static 'cjkcms/bi/bootstrap-icons.css' %}"
+            rel="stylesheet">
+    {% endif %}
+
     {% if settings.cjkcms.LayoutSettings.awesome_cdn %}
         <!-- Font Awesome -->
         <link
             href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css"
             rel="stylesheet"
             crossorigin="anonymous">
     {% endif %}
```

#### html2text {}

```diff
@@ -1,11 +1,12 @@
-{% load friendly_loader wagtailcore_tags wagtailsettings_tags cjkcms_tags %} {%
-friendly_load webpack_loader %} {% if
+{% load friendly_loader wagtailcore_tags wagtailsettings_tags cjkcms_tags
+static %} {% friendly_load webpack_loader %} {% if
 settings.cjkcms.LayoutSettings.frontend_theme == 'python-webpack' %} {# use
 python-webpack from Michael Yin #} {% if_has_tag stylesheet_pack %} {%
 stylesheet_pack 'app' %} {% endif_has_tag %} {% elif
 settings.cjkcms.LayoutSettings.frontend_theme == 'mdb.light' %}
  {% elif settings.cjkcms.LayoutSettings.frontend_theme == 'mdb.dark' %}
  {% else %}
+ {% endif %} {% if settings.cjkcms.LayoutSettings.bootstrap_icons %}
  {% endif %} {% if settings.cjkcms.LayoutSettings.awesome_cdn %}
  {% endif %} {% if settings.cjkcms.LayoutSettings.custom_font %}
  {% endif %}
```

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/snippets/frontend_scripts.html` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/snippets/frontend_scripts.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/snippets/lang_selector.html` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/snippets/lang_selector.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/snippets/navbar.html` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/snippets/navbar.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/snippets/tracking_g4.html` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/snippets/tracking_g4.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/cjkcms/widgets/checkbox_classifiers.html` & `wagtail-cjkcms-23.4.1/cjkcms/templates/cjkcms/widgets/checkbox_classifiers.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/wagtailadmin/block_forms/base_block_settings_struct.html` & `wagtail-cjkcms-23.4.1/cjkcms/templates/wagtailadmin/block_forms/base_block_settings_struct.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/wagtailadmin/block_forms/struct.html` & `wagtail-cjkcms-23.4.1/cjkcms/templates/wagtailadmin/block_forms/struct.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templates/wagtailadmin/shared/cr_main_nav_2fix.html` & `wagtail-cjkcms-23.4.1/cjkcms/templates/wagtailadmin/shared/cr_main_nav_2fix.html`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templatetags/cjkcms_tags.py` & `wagtail-cjkcms-23.4.1/cjkcms/templatetags/cjkcms_tags.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templatetags/friendly_loader.py` & `wagtail-cjkcms-23.4.1/cjkcms/templatetags/friendly_loader.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templatetags/gravatar.py` & `wagtail-cjkcms-23.4.1/cjkcms/templatetags/gravatar.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/templatetags/txtutils_tags.py` & `wagtail-cjkcms-23.4.1/cjkcms/templatetags/txtutils_tags.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/tests/test_articlepages.py` & `wagtail-cjkcms-23.4.1/cjkcms/tests/test_articlepages.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/tests/test_gravatar.py` & `wagtail-cjkcms-23.4.1/cjkcms/tests/test_gravatar.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/tests/test_search_blocks.py` & `wagtail-cjkcms-23.4.1/cjkcms/tests/test_search_blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/tests/test_settings.py` & `wagtail-cjkcms-23.4.1/cjkcms/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/tests/test_templatetags.py` & `wagtail-cjkcms-23.4.1/cjkcms/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/tests/test_urls.py` & `wagtail-cjkcms-23.4.1/cjkcms/tests/test_urls.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/tests/test_webpage.py` & `wagtail-cjkcms-23.4.1/cjkcms/tests/test_webpage.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/utils.py` & `wagtail-cjkcms-23.4.1/cjkcms/utils.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/views.py` & `wagtail-cjkcms-23.4.1/cjkcms/views.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/wagtail_hooks.py` & `wagtail-cjkcms-23.4.1/cjkcms/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/cjkcms/widgets.py` & `wagtail-cjkcms-23.4.1/cjkcms/widgets.py`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/docs/how-to/oembed_finder.md` & `wagtail-cjkcms-23.4.1/docs/how-to/oembed_finder.md`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/docs/index.md` & `wagtail-cjkcms-23.4.1/docs/index.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Overview
 
 ## Guides
 
 * [Quick start](quick-start.md) - A quick start guide for new projects.
-* [Installation details](installation.md) - A step by step installation guide.
+* [Manual installation details](installation.md) - A step by step installation guide.
 
 
 ## Management commands
 
 CjkCMS offers a [set of management commands](management_commands/index.md) to help you manage your content.
 * `init-collections` - Initialize either a default set of collections, or a custom set.
 * `clear-embeds` - Clear OEmbed cache.
```

### Comparing `wagtail-cjkcms-23.3.1/docs/installation.md` & `wagtail-cjkcms-23.4.1/docs/installation.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-# Installation details
+# Manual installation details
 
 ## Project folder
 The first step when setting up a new project is to create a folder for the project. We will call our project `cmsdemo`
 
 ```
 mkdir cmsdemo
 cd cmsdemo
 ```
-We will assume that we are in the home folder /home/, for the purpose of illustration, as later on we will have three nested folders with the same name, and it may get confusing!
+We will assume that we are in user's home folder /home/, for the purpose of illustration, as later on we will have three nested folders with the same name, and it may get confusing!
 
 The resulting folder structure should be: `/home/cmsdemo/`
 
 
 ## Virtual environment
 It is strongly recommended to use a virtual environment for the development of your project.
 Typical steps for creating a virtual environment are listed below.
 
 !!! note
     There are two typical approaches to naming a virtual environment:
 
     * always the same name, e.g.: `venv`
     * a name that is different for each project, e.g.: `env-cmsdemo`
     
-    We recommend the second approach, so that when you activate the virtual environment, you can see its' name in the terminal, and it is harder to confuse it with other virtual environments.
+    We use the second approach, so that when you activate the virtual environment, you can see its' name in the terminal, and it is harder to confuse it with other virtual environments.
 
 ```
 python3 -m venv ./env-cmsdemo/
 source ./env-cmsdemo/bin/activate
 ```
 or on Windows:
 ```
@@ -36,21 +36,16 @@
 
 ## Install wagtail-cjkcms
 ```
 pip install wagtail-cjkcms
 ```
 This will install all required dependencies into the virtual environment, including Wagtail and Django.
 
-## Note for version 0.2.1
-
-Until Codered's packages wagtail-seo and wagtail-cache are updated for compatibility with Wagtail 4, the cjkcms switches to forked versions of these packages. You will need to install them manually with:
-```
-pip install git+https://github.com/cjkpl/wagtail-cache.git
-pip install git+https://github.com/cjkpl/wagtail-seo.git
-```
+## Quick install
+If you are starting from scratch, you can use the quick install below. If you already have a project, you can follow the manual install steps below to add CjkCMS as a new app into your Wagtail project. See [quick start](quick-start.md) for more details. Otherwise follow the steps below.
 
 ## Start new Wagtail project
 With all required packages installed, you can start a new Wagtail project. We will name it `cmsdemo`, like the parent folder.
 ```
 wagtail start cmsdemo
 cd cmsdemo
 ```
@@ -69,20 +64,16 @@
 ## Start the dev server
 Start the development server and make sure you can see the default Wagtail page:
 ```
 python manage.py runserver
 ```
 This lets you make sure that the default Wagtail setup worked. CMS will be activated in the next step.
 
-## Activate CMS: update project config
-* Add CjkCMS and its requirements to ```INSTALLED_APPS``` in your project configuration
-(/home/cmsdemo/cmsdemo/cmsdemo/settings/base.py)).
-!!! note
-    Yes, there are three nested folders named `cmsdemo`: your main project folder, and inside two folders created by Wagtail.
 
+* Add CjkCMS and its requirements to ```INSTALLED_APPS``` in your project configuration (e.g. ```base.py```):
 ```python
 INSTALLED_APPS = [
     ...
     ### wagtail-cjkcms ###
     "cjkcms",
     ### wagtail-cjkcms requirements ###
     "wagtailseo",
@@ -91,43 +82,74 @@
     "wagtail.contrib.settings",
     "wagtail.contrib.modeladmin",
     "django_bootstrap5",
     "wagtail.contrib.sitemaps",
     "django.contrib.sitemaps",
     ### end wagtail-cjkcms ###
 ```
-
-Restart the development server, if it is not running. You should see a message like this:
+* Run migrations:
 ```
-You have 4 unapplied migration(s). Your project may not work properly until you apply the migrations for app(s): cjkcms, wagtailseo.
-Run 'python manage.py migrate' to apply them.
+python manage.py migrate
 ```
-
-Proceed as per message above. Stop the server, execute the `migrate` command, and restart the server.
-
-## Add utility URLs provided by CjkCMS
-
-* Add cjkcms-specific urls, which provide SEO-related pages: favicon.ico, robots.txt, sitemap.xml.
-* Replace default wagtail `search` with cjkcms-specific search: comment out the `search` view.
-
+* Add ```cjkcms.urls``` to ```urls.py``` in your project:
 ```python
-# in the main urls.py in your project:
 from cjkcms import urls as cjkcms_urls
 
 urlpatterns = [
     ...
-    # replace wagtail search with cjkcms version (comment out line below)
-    # path('search/', search_views.search, name='search'),
+    # add cjkcms urls
+    path("", include(cjkcms_urls)),
 
-    # and add cjkcms urls
-    path('', include(cjkcms_urls)),
+    # comment out the default wagtail search view,
+    # it will be replaced by the cjkcms search view
+    # path("search/", search_views.search, name="search"),
     ...
 ]
 ```
 
+## Optional setup steps
+
+Out of the box, CjkCMS can provide your project with generic, reusable pages:
+`ArticleIndex`, `Article`, `WebPage` which you can use in your project, or extend with additional functionality. CjkCMS pages provide you with a generic "body" section and, using ```wagtail-seo``` package, a basic SEO functionality.
+
+
+## Changing the homepage: 
+By default, Wagtail adds a homepage inherited from Page. If you want to use CjkCMS WebPage as your homepage, you need to change the homepage to `WebPage`. Otherwise you can start adding new CjkCMS pages to your project anywhere in the page tree.
+
+### Change to WebPage model:
+
+If you are starting a new website, you may want to replace it with CjkCMS WebPage, for the additional functionality provided by CjkCMS. 
+
+To do this, you need to:
+
+- log in to the wagtail admin
+- go to Pages
+- add a new page (any CjkCMS page type, e.g. most generic WebPage) at the top level, next to the Homepage
+- go to Settings -> Sites and change the root page of your site to the new CMS page
+- go back to pages, if there is no custom content in the default (old) homepage, you can delete it.
+
+### Old Homepage cleanup
+
+You cannot remove the HomePage model from home/models.py - first you need to delete that page in the admin panel - see section above. A safer solution is to keep the HomePage model, bug deactivate it by adding `max_count = 0` to the Homepage model, which effectively hides it from admin interface.
+
+In `/home/models.py` change this:
+
+```
+class HomePage(Page):
+    pass
+```
+
+to that:
+
+```
+class HomePage(Page):
+    max_count = 0
+```
+
+
 ## Summary and next steps
 
 At this stage you should be able to log in to the Wagtail admin interface. Visit `localhost:8000/admin/` and you should see the login page.
 
 After you log in using the superuser credentials, you should see the admin panel with CMS-specific additions:
 * `Navigation Bars` in the side menu
 * Additional menu items in `Settings`: `Social Media`, `Layout`, `Tracking`, `General`, `Mailchimp API`, `Adobe API`, `SEO`
```

### Comparing `wagtail-cjkcms-23.3.1/docs/why-another-cms.md` & `wagtail-cjkcms-23.4.1/docs/why-another-cms.md`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/setup.cfg` & `wagtail-cjkcms-23.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `wagtail-cjkcms-23.3.1/wagtail_cjkcms.egg-info/PKG-INFO` & `wagtail-cjkcms-23.4.1/wagtail_cjkcms.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: wagtail-cjkcms
-Version: 23.3.1
+Version: 23.4.1
 Summary: Wagtail Content Management System, installable as a Django app into any Wagtail 4.x site. Based on Codered CRX.
 Home-page: https://github.com/cjkpl/wagtail-cjkcms
 Author: Grzegorz Krol
 Author-email: gk@cjk.pl
 License: BSD-3-Clause  # Example license
+Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Wagtail :: 4
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -49,7 +50,8 @@
 pytest ../wagtail-cjkcms/cjkcms --ds=devsite.settings.dev --doctest-modules --durations=0
 
 ### running pytest from testproject folder:
 pytest ../cjkcms --ds=testproject.settings.dev --doctest-modules --durations=0
 
 ## Contact & support
 Please use [Github's Issue Tracker](https://github.com/cjkpl/wagtail-cjkcms/issues) to report bugs, request features, or request support.
+
```

### Comparing `wagtail-cjkcms-23.3.1/wagtail_cjkcms.egg-info/SOURCES.txt` & `wagtail-cjkcms-23.4.1/wagtail_cjkcms.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -34,40 +34,34 @@
 cjkcms/finders/oembed.py
 cjkcms/management/commands/__init__.py
 cjkcms/management/commands/clear-embeds.py
 cjkcms/management/commands/import-csv.py
 cjkcms/management/commands/init-collections.py
 cjkcms/management/commands/init-navbar.py
 cjkcms/management/commands/init-website.py
-cjkcms/management/commands/__pycache__/__init__.cpython-310.pyc
-cjkcms/management/commands/__pycache__/__init__.cpython-311.pyc
-cjkcms/management/commands/__pycache__/clear-embeds.cpython-310.pyc
-cjkcms/management/commands/__pycache__/clear-embeds.cpython-311.pyc
-cjkcms/management/commands/__pycache__/import-csv.cpython-310.pyc
-cjkcms/management/commands/__pycache__/import-csv.cpython-311.pyc
-cjkcms/management/commands/__pycache__/init-collections.cpython-310.pyc
-cjkcms/management/commands/__pycache__/init-collections.cpython-311.pyc
-cjkcms/management/commands/__pycache__/init-navbar.cpython-310.pyc
-cjkcms/management/commands/__pycache__/init-navbar.cpython-311.pyc
-cjkcms/management/commands/__pycache__/init-website.cpython-310.pyc
-cjkcms/management/commands/__pycache__/init-website.cpython-311.pyc
 cjkcms/migrations/0001_initial.py
 cjkcms/migrations/0002_alter_body_to_cjkcmsstreamfield.py
 cjkcms/migrations/0003_alter_footer_content_alter_navbar_menu_items.py
 cjkcms/migrations/0004_layoutsettings_articles_date_format_and_more.py
 cjkcms/migrations/0005_layoutsettings_custom_font_and_more.py
 cjkcms/migrations/0006_analyticssettings_consent_modal_layout_and_more.py
+cjkcms/migrations/0007_layoutsettings_bootstrap_icons.py
 cjkcms/migrations/__init__.py
 cjkcms/models/__init__.py
 cjkcms/models/admin_sidebar.py
 cjkcms/models/cms_models.py
 cjkcms/models/integration_models.py
 cjkcms/models/page_models.py
 cjkcms/models/snippet_models.py
 cjkcms/models/wagtailsettings_models.py
+cjkcms/static/cjkcms/bi/bootstrap-icons.css
+cjkcms/static/cjkcms/bi/bootstrap-icons.json
+cjkcms/static/cjkcms/bi/bootstrap-icons.scss
+cjkcms/static/cjkcms/bi/fonts/bootstrap-icons.woff
+cjkcms/static/cjkcms/bi/fonts/bootstrap-icons.woff2
 cjkcms/static/cjkcms/css/cjkcms-admin.css
 cjkcms/static/cjkcms/css/cjkcms-editor.css
 cjkcms/static/cjkcms/css/cjkcms-front.css
 cjkcms/static/cjkcms/images/avatars/default.png
 cjkcms/static/cjkcms/images/avatars/default.svg
 cjkcms/static/cjkcms/images/icons/quote.svg
 cjkcms/static/cjkcms/images/logos/cms-logo-long.svg
@@ -207,14 +201,15 @@
 cjkcms/tests/test_settings.py
 cjkcms/tests/test_templatetags.py
 cjkcms/tests/test_urls.py
 cjkcms/tests/test_webpage.py
 docs/index.md
 docs/installation.md
 docs/quick-start.md
+docs/requirements.txt
 docs/why-another-cms.md
 docs/how-to/oembed_finder.md
 docs/management_commands/clear-embeds.md
 docs/management_commands/index.md
 docs/management_commands/init-collections.md
 wagtail_cjkcms.egg-info/PKG-INFO
 wagtail_cjkcms.egg-info/SOURCES.txt
```

