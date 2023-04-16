# Comparing `tmp/uncms-0.0.7.tar.gz` & `tmp/uncms-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uncms-0.0.7.tar", last modified: Sun Mar 12 16:00:45 2023, max compression
+gzip compressed data, was "uncms-0.0.8.tar", last modified: Sun Apr 16 17:14:25 2023, max compression
```

## Comparing `uncms-0.0.7.tar` & `uncms-0.0.8.tar`

### file list

```diff
@@ -1,311 +1,326 @@
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.752554 uncms-0.0.7/
--rw-rw-r--   0 you       (1000) you       (1000)     1604 2023-01-15 00:42:46.000000 uncms-0.0.7/LICENSE
--rw-rw-r--   0 you       (1000) you       (1000)      234 2023-01-15 00:42:46.000000 uncms-0.0.7/MANIFEST.in
--rw-rw-r--   0 you       (1000) you       (1000)     1037 2023-03-12 16:00:45.752554 uncms-0.0.7/PKG-INFO
--rw-rw-r--   0 you       (1000) you       (1000)      392 2023-01-15 00:42:46.000000 uncms-0.0.7/README.md
--rw-rw-r--   0 you       (1000) you       (1000)     1208 2023-03-12 15:58:11.000000 uncms-0.0.7/pyproject.toml
--rw-rw-r--   0 you       (1000) you       (1000)       38 2023-03-12 16:00:45.752554 uncms-0.0.7/setup.cfg
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.696554 uncms-0.0.7/src/
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.708554 uncms-0.0.7/src/uncms/
--rw-rw-r--   0 you       (1000) you       (1000)       93 2023-01-15 00:42:46.000000 uncms-0.0.7/src/uncms/__init__.py
--rw-rw-r--   0 you       (1000) you       (1000)    10209 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/admin.py
--rw-rw-r--   0 you       (1000) you       (1000)      332 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/apps.py
--rw-rw-r--   0 you       (1000) you       (1000)     3738 2023-02-19 15:13:41.000000 uncms-0.0.7/src/uncms/checks.py
--rw-rw-r--   0 you       (1000) you       (1000)     5355 2023-02-19 15:03:23.000000 uncms-0.0.7/src/uncms/conf.py
--rw-rw-r--   0 you       (1000) you       (1000)     2802 2023-02-19 14:21:21.000000 uncms-0.0.7/src/uncms/forms.py
--rw-rw-r--   0 you       (1000) you       (1000)     3031 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/html.py
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.708554 uncms-0.0.7/src/uncms/jinja2_environment/
--rw-rw-r--   0 you       (1000) you       (1000)        0 2023-01-15 00:42:46.000000 uncms-0.0.7/src/uncms/jinja2_environment/__init__.py
--rw-rw-r--   0 you       (1000) you       (1000)     1026 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/jinja2_environment/all.py
--rw-rw-r--   0 you       (1000) you       (1000)       82 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/jinja2_environment/base.py
--rw-rw-r--   0 you       (1000) you       (1000)      134 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/jinja2_environment/media.py
--rw-rw-r--   0 you       (1000) you       (1000)     1741 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/jinja2_environment/pages.py
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.708554 uncms-0.0.7/src/uncms/links/
--rw-rw-r--   0 you       (1000) you       (1000)       39 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/links/__init__.py
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.712554 uncms-0.0.7/src/uncms/links/migrations/
--rw-rw-r--   0 you       (1000) you       (1000)      865 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/links/migrations/0001_initial.py
--rw-rw-r--   0 you       (1000) you       (1000)      723 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/links/migrations/0002_auto_20171020_1320.py
--rw-rw-r--   0 you       (1000) you       (1000)      329 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/links/migrations/0003_remove_link_new_window.py
--rw-rw-r--   0 you       (1000) you       (1000)      519 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/links/migrations/0004_link_permanent_redirect.py
--rw-rw-r--   0 you       (1000) you       (1000)        0 2023-01-15 00:42:46.000000 uncms-0.0.7/src/uncms/links/migrations/__init__.py
--rw-rw-r--   0 you       (1000) you       (1000)      757 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/links/models.py
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.696554 uncms-0.0.7/src/uncms/links/static/
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.696554 uncms-0.0.7/src/uncms/links/static/links/
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.712554 uncms-0.0.7/src/uncms/links/static/links/img/
--rw-rw-r--   0 you       (1000) you       (1000)     1545 2023-01-15 00:42:46.000000 uncms-0.0.7/src/uncms/links/static/links/img/link.png
--rw-rw-r--   0 you       (1000) you       (1000)      163 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/links/urls.py
--rw-rw-r--   0 you       (1000) you       (1000)      297 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/links/views.py
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.712554 uncms-0.0.7/src/uncms/media/
--rw-rw-r--   0 you       (1000) you       (1000)       43 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/media/__init__.py
--rw-rw-r--   0 you       (1000) you       (1000)    10043 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/media/admin.py
--rw-rw-r--   0 you       (1000) you       (1000)      149 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/media/apps.py
--rw-rw-r--   0 you       (1000) you       (1000)     1586 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/media/fields.py
--rw-rw-r--   0 you       (1000) you       (1000)     2534 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/media/filetypes.py
--rw-rw-r--   0 you       (1000) you       (1000)     8469 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/media/forms.py
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.716554 uncms-0.0.7/src/uncms/media/migrations/
--rw-rw-r--   0 you       (1000) you       (1000)     2547 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/media/migrations/0001_initial.py
--rw-rw-r--   0 you       (1000) you       (1000)      551 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/media/migrations/0002_auto_20150713_1408.py
--rw-rw-r--   0 you       (1000) you       (1000)      381 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/media/migrations/0003_file_alt_text.py
--rw-rw-r--   0 you       (1000) you       (1000)      687 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/media/migrations/0004_auto_20170407_1442.py
--rw-rw-r--   0 you       (1000) you       (1000)      679 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/media/migrations/0005_auto_20171107_1537.py
--rw-rw-r--   0 you       (1000) you       (1000)      348 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/media/migrations/0006_remove_video_webm.py
--rw-rw-r--   0 you       (1000) you       (1000)     1039 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/media/migrations/0007_auto_20180801_1419.py
--rw-rw-r--   0 you       (1000) you       (1000)      491 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/media/migrations/0008_auto_20180801_1633.py
--rw-rw-r--   0 you       (1000) you       (1000)      593 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/media/migrations/0009_auto_20181207_1318.py
--rw-rw-r--   0 you       (1000) you       (1000)     1143 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/media/migrations/0010_auto_20190523_1638.py
--rw-rw-r--   0 you       (1000) you       (1000)      293 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/media/migrations/0011_delete_video.py
--rw-rw-r--   0 you       (1000) you       (1000)      425 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/media/migrations/0012_alter_file_options.py
--rw-rw-r--   0 you       (1000) you       (1000)        0 2023-01-15 00:42:46.000000 uncms-0.0.7/src/uncms/media/migrations/__init__.py
--rw-rw-r--   0 you       (1000) you       (1000)     8883 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/media/models.py
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.696554 uncms-0.0.7/src/uncms/media/static/
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.700554 uncms-0.0.7/src/uncms/media/static/media/
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.716554 uncms-0.0.7/src/uncms/media/static/media/css/
--rw-rw-r--   0 you       (1000) you       (1000)     1809 2023-01-15 00:42:46.000000 uncms-0.0.7/src/uncms/media/static/media/css/media-list.css
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.716554 uncms-0.0.7/src/uncms/media/static/media/img/
--rw-rw-r--   0 you       (1000) you       (1000)     2314 2023-01-15 00:42:46.000000 uncms-0.0.7/src/uncms/media/static/media/img/audio-x-generic.png
--rw-rw-r--   0 you       (1000) you       (1000)     2791 2023-01-15 00:42:46.000000 uncms-0.0.7/src/uncms/media/static/media/img/image-x-generic.png
--rw-rw-r--   0 you       (1000) you       (1000)     1942 2023-01-15 00:42:46.000000 uncms-0.0.7/src/uncms/media/static/media/img/text-x-generic-template.png
--rw-rw-r--   0 you       (1000) you       (1000)     1895 2023-01-15 00:42:46.000000 uncms-0.0.7/src/uncms/media/static/media/img/text-x-generic.png
--rw-rw-r--   0 you       (1000) you       (1000)     1935 2023-01-15 00:42:46.000000 uncms-0.0.7/src/uncms/media/static/media/img/video-x-generic.png
--rw-rw-r--   0 you       (1000) you       (1000)     2061 2023-01-15 00:42:46.000000 uncms-0.0.7/src/uncms/media/static/media/img/x-office-document.png
--rw-rw-r--   0 you       (1000) you       (1000)     1811 2023-01-15 00:42:46.000000 uncms-0.0.7/src/uncms/media/static/media/img/x-office-spreadsheet.png
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.716554 uncms-0.0.7/src/uncms/media/static/media/js/
--rw-rw-r--   0 you       (1000) you       (1000)      609 2023-01-15 00:42:46.000000 uncms-0.0.7/src/uncms/media/static/media/js/prepopulate-title.js
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.700554 uncms-0.0.7/src/uncms/media/templates/
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.700554 uncms-0.0.7/src/uncms/media/templates/admin/
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.700554 uncms-0.0.7/src/uncms/media/templates/admin/media/
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.716554 uncms-0.0.7/src/uncms/media/templates/admin/media/file/
--rw-rw-r--   0 you       (1000) you       (1000)      526 2023-01-15 00:42:46.000000 uncms-0.0.7/src/uncms/media/templates/admin/media/file/change_form.html
--rw-rw-r--   0 you       (1000) you       (1000)      234 2023-01-21 07:57:32.000000 uncms-0.0.7/src/uncms/media/templates/admin/media/file/change_list.html
--rw-rw-r--   0 you       (1000) you       (1000)     4487 2023-01-15 00:42:46.000000 uncms-0.0.7/src/uncms/media/templates/admin/media/file/image_editor.html
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.716554 uncms-0.0.7/src/uncms/media/templates/admin/media/includes/
--rw-rw-r--   0 you       (1000) you       (1000)      856 2023-01-15 00:42:46.000000 uncms-0.0.7/src/uncms/media/templates/admin/media/includes/file_used_on.html
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.716554 uncms-0.0.7/src/uncms/media/templates/admin/widgets/
--rw-rw-r--   0 you       (1000) you       (1000)      301 2023-01-15 00:42:46.000000 uncms-0.0.7/src/uncms/media/templates/admin/widgets/image_raw_id.html
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.716554 uncms-0.0.7/src/uncms/media/templates/media/
--rw-rw-r--   0 you       (1000) you       (1000)     1059 2023-01-15 00:42:46.000000 uncms-0.0.7/src/uncms/media/templates/media/multi_format_image.html
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.716554 uncms-0.0.7/src/uncms/media/templatetags/
--rw-rw-r--   0 you       (1000) you       (1000)        0 2023-01-15 00:42:46.000000 uncms-0.0.7/src/uncms/media/templatetags/__init__.py
--rw-rw-r--   0 you       (1000) you       (1000)      153 2023-01-15 00:42:46.000000 uncms-0.0.7/src/uncms/media/templatetags/uncms_images.py
--rw-rw-r--   0 you       (1000) you       (1000)     1987 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/media/types.py
--rw-rw-r--   0 you       (1000) you       (1000)      423 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/media/urls.py
--rw-rw-r--   0 you       (1000) you       (1000)     4945 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/media/views.py
--rw-rw-r--   0 you       (1000) you       (1000)      737 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/media/widgets.py
--rw-rw-r--   0 you       (1000) you       (1000)     2370 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/middleware.py
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.716554 uncms-0.0.7/src/uncms/models/
--rw-rw-r--   0 you       (1000) you       (1000)      509 2023-01-15 00:42:46.000000 uncms-0.0.7/src/uncms/models/__init__.py
--rw-rw-r--   0 you       (1000) you       (1000)    10863 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/models/base.py
--rw-rw-r--   0 you       (1000) you       (1000)     2652 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/models/fields.py
--rw-rw-r--   0 you       (1000) you       (1000)     2887 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/models/managers.py
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.716554 uncms-0.0.7/src/uncms/moderation/
--rw-rw-r--   0 you       (1000) you       (1000)        0 2023-01-15 00:42:46.000000 uncms-0.0.7/src/uncms/moderation/__init__.py
--rw-rw-r--   0 you       (1000) you       (1000)      949 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/moderation/admin.py
--rw-rw-r--   0 you       (1000) you       (1000)      749 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/moderation/models.py
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.720554 uncms-0.0.7/src/uncms/pages/
--rw-rw-r--   0 you       (1000) you       (1000)      155 2023-01-15 00:42:46.000000 uncms-0.0.7/src/uncms/pages/__init__.py
--rw-rw-r--   0 you       (1000) you       (1000)    28973 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/pages/admin.py
--rw-rw-r--   0 you       (1000) you       (1000)      400 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/pages/apps.py
--rw-rw-r--   0 you       (1000) you       (1000)      207 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/pages/context_processors.py
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.700554 uncms-0.0.7/src/uncms/pages/jinja2/
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.720554 uncms-0.0.7/src/uncms/pages/jinja2/pages/
--rw-rw-r--   0 you       (1000) you       (1000)     1114 2023-01-15 00:42:46.000000 uncms-0.0.7/src/uncms/pages/jinja2/pages/breadcrumbs.jinja2
--rw-rw-r--   0 you       (1000) you       (1000)      782 2023-01-15 00:42:46.000000 uncms-0.0.7/src/uncms/pages/jinja2/pages/head_meta.jinja2
--rw-rw-r--   0 you       (1000) you       (1000)     6323 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/pages/middleware.py
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.720554 uncms-0.0.7/src/uncms/pages/migrations/
--rw-rw-r--   0 you       (1000) you       (1000)     6112 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/pages/migrations/0001_initial.py
--rw-rw-r--   0 you       (1000) you       (1000)      364 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/pages/migrations/0002_page_requires_authentication.py
--rw-rw-r--   0 you       (1000) you       (1000)      442 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/pages/migrations/0003_page_hide_from_anonymous.py
--rw-rw-r--   0 you       (1000) you       (1000)      341 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/pages/migrations/0004_url_title_migration.py
--rw-rw-r--   0 you       (1000) you       (1000)     4065 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/pages/migrations/0005_social_fields.py
--rw-rw-r--   0 you       (1000) you       (1000)     4855 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/pages/migrations/0006_auto_20151002_1655.py
--rw-rw-r--   0 you       (1000) you       (1000)      394 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/pages/migrations/0007_remove_page_cached_url.py
--rw-rw-r--   0 you       (1000) you       (1000)      567 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/pages/migrations/0008_auto_20191108_1506.py
--rw-rw-r--   0 you       (1000) you       (1000)      464 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/pages/migrations/0009_auto_20200406_1508.py
--rw-rw-r--   0 you       (1000) you       (1000)      928 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/pages/migrations/0010_auto_20200812_1546.py
--rw-rw-r--   0 you       (1000) you       (1000)      875 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/pages/migrations/0011_remove_localisation.py
--rw-rw-r--   0 you       (1000) you       (1000)        0 2023-01-15 00:42:46.000000 uncms-0.0.7/src/uncms/pages/migrations/__init__.py
--rw-rw-r--   0 you       (1000) you       (1000)    15434 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/pages/models.py
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.700554 uncms-0.0.7/src/uncms/pages/static/
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.700554 uncms-0.0.7/src/uncms/pages/static/pages/
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.720554 uncms-0.0.7/src/uncms/pages/static/pages/css/
--rw-rw-r--   0 you       (1000) you       (1000)      922 2023-01-15 00:42:46.000000 uncms-0.0.7/src/uncms/pages/static/pages/css/page-type-selector.css
--rw-rw-r--   0 you       (1000) you       (1000)     1152 2023-01-15 00:42:46.000000 uncms-0.0.7/src/uncms/pages/static/pages/css/sample-navigation.css
--rw-rw-r--   0 you       (1000) you       (1000)     1421 2023-01-15 00:42:46.000000 uncms-0.0.7/src/uncms/pages/static/pages/css/sitemap-module.css
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.724554 uncms-0.0.7/src/uncms/pages/static/pages/img/
--rw-rw-r--   0 you       (1000) you       (1000)     3208 2023-01-15 00:42:46.000000 uncms-0.0.7/src/uncms/pages/static/pages/img/ajax-loader.gif
--rw-rw-r--   0 you       (1000) you       (1000)      258 2023-01-15 00:42:46.000000 uncms-0.0.7/src/uncms/pages/static/pages/img/arrows.png
--rw-rw-r--   0 you       (1000) you       (1000)     1239 2023-01-15 00:42:46.000000 uncms-0.0.7/src/uncms/pages/static/pages/img/content.png
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.700554 uncms-0.0.7/src/uncms/pages/templates/
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.700554 uncms-0.0.7/src/uncms/pages/templates/admin/
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.700554 uncms-0.0.7/src/uncms/pages/templates/admin/pages/
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.724554 uncms-0.0.7/src/uncms/pages/templates/admin/pages/page/
--rw-rw-r--   0 you       (1000) you       (1000)     1330 2023-01-15 00:42:46.000000 uncms-0.0.7/src/uncms/pages/templates/admin/pages/page/select_page_type.html
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.724554 uncms-0.0.7/src/uncms/pages/templates/pages/
--rw-rw-r--   0 you       (1000) you       (1000)     1114 2023-01-15 00:42:46.000000 uncms-0.0.7/src/uncms/pages/templates/pages/breadcrumbs.html
--rw-rw-r--   0 you       (1000) you       (1000)      730 2023-01-15 00:42:46.000000 uncms-0.0.7/src/uncms/pages/templates/pages/head_meta.html
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.724554 uncms-0.0.7/src/uncms/pages/templates/pages/navigation/
--rw-rw-r--   0 you       (1000) you       (1000)      277 2023-01-15 00:42:46.000000 uncms-0.0.7/src/uncms/pages/templates/pages/navigation/navigation.html
--rw-rw-r--   0 you       (1000) you       (1000)      892 2023-01-15 00:42:46.000000 uncms-0.0.7/src/uncms/pages/templates/pages/navigation/navigation_item.html
--rw-rw-r--   0 you       (1000) you       (1000)      243 2023-01-15 00:42:46.000000 uncms-0.0.7/src/uncms/pages/templates/pages/navigation/navigation_submenu.html
--rw-rw-r--   0 you       (1000) you       (1000)      888 2023-01-15 00:42:46.000000 uncms-0.0.7/src/uncms/pages/templates/pages/navigation/navigation_submenu_item.html
--rw-rw-r--   0 you       (1000) you       (1000)       12 2023-01-15 00:42:46.000000 uncms-0.0.7/src/uncms/pages/templates/pages/title.html
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.724554 uncms-0.0.7/src/uncms/pages/templatetags/
--rw-rw-r--   0 you       (1000) you       (1000)       43 2023-01-15 00:42:46.000000 uncms-0.0.7/src/uncms/pages/templatetags/__init__.py
--rw-rw-r--   0 you       (1000) you       (1000)    11938 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/pages/templatetags/_common.py
--rw-rw-r--   0 you       (1000) you       (1000)     4820 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/pages/templatetags/uncms_pages.py
--rw-rw-r--   0 you       (1000) you       (1000)     3501 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/pages/types.py
--rw-rw-r--   0 you       (1000) you       (1000)      254 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/pages/urls.py
--rw-rw-r--   0 you       (1000) you       (1000)      948 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/pages/views.py
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.724554 uncms-0.0.7/src/uncms/plugins/
--rw-rw-r--   0 you       (1000) you       (1000)        0 2023-01-15 00:42:46.000000 uncms-0.0.7/src/uncms/plugins/__init__.py
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.724554 uncms-0.0.7/src/uncms/redirects/
--rw-rw-r--   0 you       (1000) you       (1000)        0 2023-02-12 13:06:23.000000 uncms-0.0.7/src/uncms/redirects/__init__.py
--rw-rw-r--   0 you       (1000) you       (1000)     5149 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/redirects/admin.py
--rw-rw-r--   0 you       (1000) you       (1000)      156 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/redirects/apps.py
--rw-rw-r--   0 you       (1000) you       (1000)     1666 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/redirects/forms.py
--rw-rw-r--   0 you       (1000) you       (1000)     4268 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/redirects/importer.py
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.724554 uncms-0.0.7/src/uncms/redirects/management/
--rw-rw-r--   0 you       (1000) you       (1000)        0 2023-02-12 13:06:23.000000 uncms-0.0.7/src/uncms/redirects/management/__init__.py
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.728554 uncms-0.0.7/src/uncms/redirects/management/commands/
--rw-rw-r--   0 you       (1000) you       (1000)        0 2023-02-12 13:06:23.000000 uncms-0.0.7/src/uncms/redirects/management/commands/__init__.py
--rw-rw-r--   0 you       (1000) you       (1000)     2618 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/redirects/management/commands/import_redirects_csv.py
--rw-rw-r--   0 you       (1000) you       (1000)      976 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/redirects/middleware.py
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.728554 uncms-0.0.7/src/uncms/redirects/migrations/
--rw-rw-r--   0 you       (1000) you       (1000)     1713 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/redirects/migrations/0001_initial.py
--rw-rw-r--   0 you       (1000) you       (1000)        0 2023-02-12 13:06:23.000000 uncms-0.0.7/src/uncms/redirects/migrations/__init__.py
--rw-rw-r--   0 you       (1000) you       (1000)     7823 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/redirects/models.py
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.700554 uncms-0.0.7/src/uncms/redirects/static/
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.700554 uncms-0.0.7/src/uncms/redirects/static/uncms/
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.728554 uncms-0.0.7/src/uncms/redirects/static/uncms/js/
--rw-rw-r--   0 you       (1000) you       (1000)      876 2023-02-12 13:06:23.000000 uncms-0.0.7/src/uncms/redirects/static/uncms/js/redirect-fields.js
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.700554 uncms-0.0.7/src/uncms/redirects/templates/
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.700554 uncms-0.0.7/src/uncms/redirects/templates/admin/
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.700554 uncms-0.0.7/src/uncms/redirects/templates/admin/redirects/
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.728554 uncms-0.0.7/src/uncms/redirects/templates/admin/redirects/redirect/
--rw-rw-r--   0 you       (1000) you       (1000)      366 2023-02-12 13:06:23.000000 uncms-0.0.7/src/uncms/redirects/templates/admin/redirects/redirect/change_list.html
--rw-rw-r--   0 you       (1000) you       (1000)     3572 2023-02-12 13:06:23.000000 uncms-0.0.7/src/uncms/redirects/templates/admin/redirects/redirect/import_form.html
--rw-rw-r--   0 you       (1000) you       (1000)      214 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/redirects/types.py
--rw-rw-r--   0 you       (1000) you       (1000)     2368 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/robots.py
--rw-rw-r--   0 you       (1000) you       (1000)     3059 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/sitemaps.py
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.704553 uncms-0.0.7/src/uncms/static/
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.704553 uncms-0.0.7/src/uncms/static/cms/
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.704553 uncms-0.0.7/src/uncms/static/cms/js/
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.728554 uncms-0.0.7/src/uncms/static/cms/js/imgeditor/
--rw-rw-r--   0 you       (1000) you       (1000)    31397 2023-01-15 00:42:46.000000 uncms-0.0.7/src/uncms/static/cms/js/imgeditor/image-editor.css
--rw-rw-r--   0 you       (1000) you       (1000)  1589044 2023-01-15 00:42:46.000000 uncms-0.0.7/src/uncms/static/cms/js/imgeditor/image-editor.js
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.704553 uncms-0.0.7/src/uncms/static/cms/svg/
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.736554 uncms-0.0.7/src/uncms/static/cms/svg/image-editor/
--rwxrwxr-x   0 you       (1000) you       (1000)    20048 2023-01-15 00:42:46.000000 uncms-0.0.7/src/uncms/static/cms/svg/image-editor/icon-a.svg
--rwxrwxr-x   0 you       (1000) you       (1000)    19665 2023-01-15 00:42:46.000000 uncms-0.0.7/src/uncms/static/cms/svg/image-editor/icon-b.svg
--rwxrwxr-x   0 you       (1000) you       (1000)    19665 2023-01-15 00:42:46.000000 uncms-0.0.7/src/uncms/static/cms/svg/image-editor/icon-c.svg
--rwxrwxr-x   0 you       (1000) you       (1000)    19665 2023-01-15 00:42:46.000000 uncms-0.0.7/src/uncms/static/cms/svg/image-editor/icon-d.svg
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.704553 uncms-0.0.7/src/uncms/static/uncms/
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.736554 uncms-0.0.7/src/uncms/static/uncms/css/
--rw-rw-r--   0 you       (1000) you       (1000)      878 2023-01-27 01:17:56.000000 uncms-0.0.7/src/uncms/static/uncms/css/trumbowyg-tweak.css
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.736554 uncms-0.0.7/src/uncms/static/uncms/js/
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.736554 uncms-0.0.7/src/uncms/static/uncms/js/trumbowyg-imagelibrary/
--rw-rw-r--   0 you       (1000) you       (1000)     8285 2023-02-19 16:07:10.000000 uncms-0.0.7/src/uncms/static/uncms/js/trumbowyg-imagelibrary/trumbowyg.imagelibrary.js
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.736554 uncms-0.0.7/src/uncms/static/uncms/js/trumbowyg-imagelibrary/ui/
--rw-rw-r--   0 you       (1000) you       (1000)     1288 2023-01-21 07:57:32.000000 uncms-0.0.7/src/uncms/static/uncms/js/trumbowyg-imagelibrary/ui/trumbowyg.imagelibrary.css
--rw-rw-r--   0 you       (1000) you       (1000)     2180 2023-03-12 15:51:22.000000 uncms-0.0.7/src/uncms/static/uncms/js/wysiwyg.js
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.704553 uncms-0.0.7/src/uncms/static/uncms/vendor/
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.736554 uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.748554 uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/
--rw-rw-r--   0 you       (1000) you       (1000)     1664 2022-11-14 15:37:02.000000 uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/ar.js
--rw-rw-r--   0 you       (1000) you       (1000)     1559 2022-11-14 15:37:02.000000 uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/bg.js
--rw-rw-r--   0 you       (1000) you       (1000)     2060 2022-11-14 15:37:02.000000 uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/bn.js
--rw-rw-r--   0 you       (1000) you       (1000)     1762 2022-11-14 15:37:02.000000 uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/by.js
--rw-rw-r--   0 you       (1000) you       (1000)     1349 2022-11-14 15:37:02.000000 uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/ca.js
--rw-rw-r--   0 you       (1000) you       (1000)     1454 2022-11-14 15:37:02.000000 uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/cs.js
--rw-rw-r--   0 you       (1000) you       (1000)     1420 2022-11-14 15:37:02.000000 uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/da.js
--rw-rw-r--   0 you       (1000) you       (1000)     1343 2022-11-14 15:37:02.000000 uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/de.js
--rw-rw-r--   0 you       (1000) you       (1000)     1888 2022-11-14 15:37:02.000000 uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/el.js
--rw-rw-r--   0 you       (1000) you       (1000)     1430 2022-11-14 15:37:02.000000 uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/es.js
--rw-rw-r--   0 you       (1000) you       (1000)     1325 2022-11-14 15:37:02.000000 uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/es_ar.js
--rw-rw-r--   0 you       (1000) you       (1000)     1437 2022-11-14 15:37:02.000000 uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/et.js
--rw-rw-r--   0 you       (1000) you       (1000)     1492 2022-11-14 15:37:02.000000 uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/fa.js
--rw-rw-r--   0 you       (1000) you       (1000)     1299 2022-11-14 15:37:02.000000 uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/fi.js
--rw-rw-r--   0 you       (1000) you       (1000)     1623 2022-11-14 15:37:02.000000 uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/fr.js
--rw-rw-r--   0 you       (1000) you       (1000)     1382 2022-11-14 15:37:02.000000 uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/he.js
--rw-rw-r--   0 you       (1000) you       (1000)     1302 2022-11-14 15:37:02.000000 uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/hr.js
--rw-rw-r--   0 you       (1000) you       (1000)     1361 2022-11-14 15:37:02.000000 uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/hu.js
--rw-rw-r--   0 you       (1000) you       (1000)     1338 2022-11-14 15:37:02.000000 uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/id.js
--rw-rw-r--   0 you       (1000) you       (1000)     1405 2022-11-14 15:37:02.000000 uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/it.js
--rw-rw-r--   0 you       (1000) you       (1000)     1495 2022-11-14 15:37:02.000000 uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/ja.js
--rw-rw-r--   0 you       (1000) you       (1000)     1558 2022-11-14 15:37:02.000000 uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/ko.js
--rw-rw-r--   0 you       (1000) you       (1000)     1381 2022-11-14 15:37:02.000000 uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/lt.js
--rw-rw-r--   0 you       (1000) you       (1000)     1641 2022-11-14 15:37:02.000000 uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/mn.js
--rw-rw-r--   0 you       (1000) you       (1000)     1240 2022-11-14 15:37:02.000000 uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/my.js
--rw-rw-r--   0 you       (1000) you       (1000)     1381 2022-11-14 15:37:02.000000 uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/nl.js
--rw-rw-r--   0 you       (1000) you       (1000)     1287 2022-11-14 15:37:02.000000 uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/no_nb.js
--rw-rw-r--   0 you       (1000) you       (1000)     1251 2022-11-14 15:37:02.000000 uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/ph.js
--rw-rw-r--   0 you       (1000) you       (1000)     1273 2022-11-14 15:37:02.000000 uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/pl.js
--rw-rw-r--   0 you       (1000) you       (1000)     1547 2022-11-14 15:37:02.000000 uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/pt.js
--rw-rw-r--   0 you       (1000) you       (1000)     1543 2022-11-14 15:37:02.000000 uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/pt_br.js
--rw-rw-r--   0 you       (1000) you       (1000)     1407 2022-11-14 15:37:02.000000 uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/ro.js
--rw-rw-r--   0 you       (1000) you       (1000)     1563 2022-11-14 15:37:02.000000 uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/rs.js
--rw-rw-r--   0 you       (1000) you       (1000)     1326 2022-11-14 15:37:02.000000 uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/rs_latin.js
--rw-rw-r--   0 you       (1000) you       (1000)     1785 2022-11-14 15:37:02.000000 uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/ru.js
--rw-rw-r--   0 you       (1000) you       (1000)     1281 2022-11-14 15:37:02.000000 uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/sk.js
--rw-rw-r--   0 you       (1000) you       (1000)     1373 2022-11-14 15:37:02.000000 uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/sl.js
--rw-rw-r--   0 you       (1000) you       (1000)     1401 2022-11-14 15:37:02.000000 uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/sq.js
--rw-rw-r--   0 you       (1000) you       (1000)     1330 2022-11-14 15:37:02.000000 uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/sv.js
--rw-rw-r--   0 you       (1000) you       (1000)     1530 2022-11-14 15:37:02.000000 uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/th.js
--rw-rw-r--   0 you       (1000) you       (1000)     1437 2022-11-14 15:37:02.000000 uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/tr.js
--rw-rw-r--   0 you       (1000) you       (1000)     1583 2022-11-14 15:37:02.000000 uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/ua.js
--rw-rw-r--   0 you       (1000) you       (1000)     1392 2022-11-14 15:37:02.000000 uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/vi.js
--rw-rw-r--   0 you       (1000) you       (1000)     1281 2022-11-14 15:37:02.000000 uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/zh_cn.js
--rw-rw-r--   0 you       (1000) you       (1000)     1489 2022-11-14 15:37:02.000000 uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/zh_tw.js
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.704553 uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/plugins/
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.748554 uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/plugins/cleanpaste/
--rw-rw-r--   0 you       (1000) you       (1000)     5821 2022-11-14 15:37:02.000000 uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/plugins/cleanpaste/trumbowyg.cleanpaste.js
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.748554 uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/plugins/preformatted/
--rw-rw-r--   0 you       (1000) you       (1000)     4799 2022-11-14 15:37:02.000000 uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/plugins/preformatted/trumbowyg.preformatted.js
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.748554 uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/plugins/table/
--rw-rw-r--   0 you       (1000) you       (1000)    19549 2022-11-14 15:37:02.000000 uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/plugins/table/trumbowyg.table.js
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.748554 uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/plugins/table/ui/
--rw-rw-r--   0 you       (1000) you       (1000)      969 2022-11-14 15:37:02.000000 uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/plugins/table/ui/trumbowyg.table.css
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.748554 uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/plugins/upload/
--rw-rw-r--   0 you       (1000) you       (1000)    12986 2022-11-14 15:37:02.000000 uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/plugins/upload/trumbowyg.upload.js
--rw-rw-r--   0 you       (1000) you       (1000)    71140 2022-11-14 15:37:02.000000 uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/trumbowyg.js
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.748554 uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/ui/
--rw-rw-r--   0 you       (1000) you       (1000)    30702 2022-11-14 15:37:02.000000 uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/ui/icons.svg
--rw-rw-r--   0 you       (1000) you       (1000)    22676 2022-11-14 15:37:02.000000 uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/ui/trumbowyg.css
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.748554 uncms-0.0.7/src/uncms/templates/
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.704553 uncms-0.0.7/src/uncms/templates/admin/
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.748554 uncms-0.0.7/src/uncms/templates/admin/dashboard_modules/
--rw-rw-r--   0 you       (1000) you       (1000)      506 2023-01-15 00:42:46.000000 uncms-0.0.7/src/uncms/templates/admin/dashboard_modules/sitemap.html
--rw-rw-r--   0 you       (1000) you       (1000)     2095 2023-01-15 00:42:46.000000 uncms-0.0.7/src/uncms/templates/admin/dashboard_modules/sitemap_items.html
--rw-rw-r--   0 you       (1000) you       (1000)      491 2023-01-15 00:42:46.000000 uncms-0.0.7/src/uncms/templates/base.html
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.748554 uncms-0.0.7/src/uncms/templates/pagination/
--rw-rw-r--   0 you       (1000) you       (1000)      897 2023-01-15 00:42:46.000000 uncms-0.0.7/src/uncms/templates/pagination/pagination.html
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.748554 uncms-0.0.7/src/uncms/templatetags/
--rw-rw-r--   0 you       (1000) you       (1000)       41 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/templatetags/__init__.py
--rw-rw-r--   0 you       (1000) you       (1000)      826 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/templatetags/_common.py
--rw-rw-r--   0 you       (1000) you       (1000)      245 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/templatetags/uncms_html.py
--rw-rw-r--   0 you       (1000) you       (1000)     1637 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/templatetags/uncms_pagination.py
--rw-rw-r--   0 you       (1000) you       (1000)      581 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/utils.py
--rw-rw-r--   0 you       (1000) you       (1000)     1183 2023-02-18 21:37:05.000000 uncms-0.0.7/src/uncms/views.py
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.708554 uncms-0.0.7/src/uncms.egg-info/
--rw-rw-r--   0 you       (1000) you       (1000)     1037 2023-03-12 16:00:45.000000 uncms-0.0.7/src/uncms.egg-info/PKG-INFO
--rw-rw-r--   0 you       (1000) you       (1000)     9895 2023-03-12 16:00:45.000000 uncms-0.0.7/src/uncms.egg-info/SOURCES.txt
--rw-rw-r--   0 you       (1000) you       (1000)        1 2023-03-12 16:00:45.000000 uncms-0.0.7/src/uncms.egg-info/dependency_links.txt
--rw-rw-r--   0 you       (1000) you       (1000)      336 2023-03-12 16:00:45.000000 uncms-0.0.7/src/uncms.egg-info/requires.txt
--rw-rw-r--   0 you       (1000) you       (1000)        6 2023-03-12 16:00:45.000000 uncms-0.0.7/src/uncms.egg-info/top_level.txt
-drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-03-12 16:00:45.752554 uncms-0.0.7/tests/
--rw-rw-r--   0 you       (1000) you       (1000)     2291 2023-02-18 21:37:05.000000 uncms-0.0.7/tests/test_admin.py
--rw-rw-r--   0 you       (1000) you       (1000)     2606 2023-02-19 15:10:18.000000 uncms-0.0.7/tests/test_checks.py
--rw-rw-r--   0 you       (1000) you       (1000)     1789 2023-02-18 21:37:05.000000 uncms-0.0.7/tests/test_conf.py
--rw-rw-r--   0 you       (1000) you       (1000)     1225 2023-02-19 14:24:22.000000 uncms-0.0.7/tests/test_forms.py
--rw-rw-r--   0 you       (1000) you       (1000)     3799 2023-02-18 21:37:05.000000 uncms-0.0.7/tests/test_html.py
--rw-rw-r--   0 you       (1000) you       (1000)      437 2023-02-18 21:37:05.000000 uncms-0.0.7/tests/test_jinja2_environment.py
--rw-rw-r--   0 you       (1000) you       (1000)     2469 2023-02-18 21:37:05.000000 uncms-0.0.7/tests/test_middleware.py
--rw-rw-r--   0 you       (1000) you       (1000)      622 2023-02-18 21:37:05.000000 uncms-0.0.7/tests/test_models.py
--rw-rw-r--   0 you       (1000) you       (1000)     3146 2023-02-18 21:37:05.000000 uncms-0.0.7/tests/test_models_base.py
--rw-rw-r--   0 you       (1000) you       (1000)      949 2023-02-18 21:37:05.000000 uncms-0.0.7/tests/test_models_fields.py
--rw-rw-r--   0 you       (1000) you       (1000)     5537 2023-02-18 21:37:05.000000 uncms-0.0.7/tests/test_robots.py
--rw-rw-r--   0 you       (1000) you       (1000)     1718 2023-02-18 21:37:05.000000 uncms-0.0.7/tests/test_sitemaps.py
--rw-rw-r--   0 you       (1000) you       (1000)      256 2023-02-18 21:37:05.000000 uncms-0.0.7/tests/test_templatetags_html.py
--rw-rw-r--   0 you       (1000) you       (1000)      962 2023-02-18 21:37:05.000000 uncms-0.0.7/tests/test_templatetags_pagination.py
--rw-rw-r--   0 you       (1000) you       (1000)      595 2023-02-18 21:37:05.000000 uncms-0.0.7/tests/test_utils.py
--rw-rw-r--   0 you       (1000) you       (1000)      794 2023-02-18 21:37:05.000000 uncms-0.0.7/tests/test_views.py
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.686981 uncms-0.0.8/
+-rw-rw-r--   0 you       (1000) you       (1000)     1604 2023-01-15 00:42:46.000000 uncms-0.0.8/LICENSE
+-rw-rw-r--   0 you       (1000) you       (1000)      328 2023-03-13 03:55:33.000000 uncms-0.0.8/MANIFEST.in
+-rw-rw-r--   0 you       (1000) you       (1000)     1065 2023-04-16 17:14:25.686981 uncms-0.0.8/PKG-INFO
+-rw-rw-r--   0 you       (1000) you       (1000)      392 2023-01-15 00:42:46.000000 uncms-0.0.8/README.md
+-rw-rw-r--   0 you       (1000) you       (1000)     1253 2023-04-16 17:12:56.000000 uncms-0.0.8/pyproject.toml
+-rw-rw-r--   0 you       (1000) you       (1000)       38 2023-04-16 17:14:25.686981 uncms-0.0.8/setup.cfg
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.626981 uncms-0.0.8/src/
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.638981 uncms-0.0.8/src/uncms/
+-rw-rw-r--   0 you       (1000) you       (1000)       93 2023-01-15 00:42:46.000000 uncms-0.0.8/src/uncms/__init__.py
+-rw-rw-r--   0 you       (1000) you       (1000)    10209 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/admin.py
+-rw-rw-r--   0 you       (1000) you       (1000)      332 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/apps.py
+-rw-rw-r--   0 you       (1000) you       (1000)     3738 2023-02-19 15:13:41.000000 uncms-0.0.8/src/uncms/checks.py
+-rw-rw-r--   0 you       (1000) you       (1000)     5355 2023-02-19 15:03:23.000000 uncms-0.0.8/src/uncms/conf.py
+-rw-rw-r--   0 you       (1000) you       (1000)     2802 2023-02-19 14:21:21.000000 uncms-0.0.8/src/uncms/forms.py
+-rw-rw-r--   0 you       (1000) you       (1000)     3031 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/html.py
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.638981 uncms-0.0.8/src/uncms/jinja2_environment/
+-rw-rw-r--   0 you       (1000) you       (1000)        0 2023-01-15 00:42:46.000000 uncms-0.0.8/src/uncms/jinja2_environment/__init__.py
+-rw-rw-r--   0 you       (1000) you       (1000)     1026 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/jinja2_environment/all.py
+-rw-rw-r--   0 you       (1000) you       (1000)       82 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/jinja2_environment/base.py
+-rw-rw-r--   0 you       (1000) you       (1000)      134 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/jinja2_environment/media.py
+-rw-rw-r--   0 you       (1000) you       (1000)     1741 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/jinja2_environment/pages.py
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.638981 uncms-0.0.8/src/uncms/links/
+-rw-rw-r--   0 you       (1000) you       (1000)       39 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/links/__init__.py
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.638981 uncms-0.0.8/src/uncms/links/migrations/
+-rw-rw-r--   0 you       (1000) you       (1000)      865 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/links/migrations/0001_initial.py
+-rw-rw-r--   0 you       (1000) you       (1000)      723 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/links/migrations/0002_auto_20171020_1320.py
+-rw-rw-r--   0 you       (1000) you       (1000)      329 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/links/migrations/0003_remove_link_new_window.py
+-rw-rw-r--   0 you       (1000) you       (1000)      519 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/links/migrations/0004_link_permanent_redirect.py
+-rw-rw-r--   0 you       (1000) you       (1000)        0 2023-01-15 00:42:46.000000 uncms-0.0.8/src/uncms/links/migrations/__init__.py
+-rw-rw-r--   0 you       (1000) you       (1000)      757 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/links/models.py
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.626981 uncms-0.0.8/src/uncms/links/static/
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.626981 uncms-0.0.8/src/uncms/links/static/links/
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.638981 uncms-0.0.8/src/uncms/links/static/links/img/
+-rw-rw-r--   0 you       (1000) you       (1000)     1545 2023-01-15 00:42:46.000000 uncms-0.0.8/src/uncms/links/static/links/img/link.png
+-rw-rw-r--   0 you       (1000) you       (1000)      163 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/links/urls.py
+-rw-rw-r--   0 you       (1000) you       (1000)      297 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/links/views.py
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.642981 uncms-0.0.8/src/uncms/media/
+-rw-rw-r--   0 you       (1000) you       (1000)       43 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/media/__init__.py
+-rw-rw-r--   0 you       (1000) you       (1000)    10043 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/media/admin.py
+-rw-rw-r--   0 you       (1000) you       (1000)      149 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/media/apps.py
+-rw-rw-r--   0 you       (1000) you       (1000)     1586 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/media/fields.py
+-rw-rw-r--   0 you       (1000) you       (1000)     2534 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/media/filetypes.py
+-rw-rw-r--   0 you       (1000) you       (1000)     8469 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/media/forms.py
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.642981 uncms-0.0.8/src/uncms/media/migrations/
+-rw-rw-r--   0 you       (1000) you       (1000)     2547 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/media/migrations/0001_initial.py
+-rw-rw-r--   0 you       (1000) you       (1000)      551 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/media/migrations/0002_auto_20150713_1408.py
+-rw-rw-r--   0 you       (1000) you       (1000)      381 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/media/migrations/0003_file_alt_text.py
+-rw-rw-r--   0 you       (1000) you       (1000)      687 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/media/migrations/0004_auto_20170407_1442.py
+-rw-rw-r--   0 you       (1000) you       (1000)      679 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/media/migrations/0005_auto_20171107_1537.py
+-rw-rw-r--   0 you       (1000) you       (1000)      348 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/media/migrations/0006_remove_video_webm.py
+-rw-rw-r--   0 you       (1000) you       (1000)     1039 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/media/migrations/0007_auto_20180801_1419.py
+-rw-rw-r--   0 you       (1000) you       (1000)      491 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/media/migrations/0008_auto_20180801_1633.py
+-rw-rw-r--   0 you       (1000) you       (1000)      593 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/media/migrations/0009_auto_20181207_1318.py
+-rw-rw-r--   0 you       (1000) you       (1000)     1143 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/media/migrations/0010_auto_20190523_1638.py
+-rw-rw-r--   0 you       (1000) you       (1000)      293 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/media/migrations/0011_delete_video.py
+-rw-rw-r--   0 you       (1000) you       (1000)      425 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/media/migrations/0012_alter_file_options.py
+-rw-rw-r--   0 you       (1000) you       (1000)        0 2023-01-15 00:42:46.000000 uncms-0.0.8/src/uncms/media/migrations/__init__.py
+-rw-rw-r--   0 you       (1000) you       (1000)     8883 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/media/models.py
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.626981 uncms-0.0.8/src/uncms/media/static/
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.626981 uncms-0.0.8/src/uncms/media/static/media/
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.642981 uncms-0.0.8/src/uncms/media/static/media/css/
+-rw-rw-r--   0 you       (1000) you       (1000)     1809 2023-01-15 00:42:46.000000 uncms-0.0.8/src/uncms/media/static/media/css/media-list.css
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.646981 uncms-0.0.8/src/uncms/media/static/media/img/
+-rw-rw-r--   0 you       (1000) you       (1000)     2314 2023-01-15 00:42:46.000000 uncms-0.0.8/src/uncms/media/static/media/img/audio-x-generic.png
+-rw-rw-r--   0 you       (1000) you       (1000)     2791 2023-01-15 00:42:46.000000 uncms-0.0.8/src/uncms/media/static/media/img/image-x-generic.png
+-rw-rw-r--   0 you       (1000) you       (1000)     1942 2023-01-15 00:42:46.000000 uncms-0.0.8/src/uncms/media/static/media/img/text-x-generic-template.png
+-rw-rw-r--   0 you       (1000) you       (1000)     1895 2023-01-15 00:42:46.000000 uncms-0.0.8/src/uncms/media/static/media/img/text-x-generic.png
+-rw-rw-r--   0 you       (1000) you       (1000)     1935 2023-01-15 00:42:46.000000 uncms-0.0.8/src/uncms/media/static/media/img/video-x-generic.png
+-rw-rw-r--   0 you       (1000) you       (1000)     2061 2023-01-15 00:42:46.000000 uncms-0.0.8/src/uncms/media/static/media/img/x-office-document.png
+-rw-rw-r--   0 you       (1000) you       (1000)     1811 2023-01-15 00:42:46.000000 uncms-0.0.8/src/uncms/media/static/media/img/x-office-spreadsheet.png
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.646981 uncms-0.0.8/src/uncms/media/static/media/js/
+-rw-rw-r--   0 you       (1000) you       (1000)      609 2023-01-15 00:42:46.000000 uncms-0.0.8/src/uncms/media/static/media/js/prepopulate-title.js
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.626981 uncms-0.0.8/src/uncms/media/templates/
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.626981 uncms-0.0.8/src/uncms/media/templates/admin/
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.626981 uncms-0.0.8/src/uncms/media/templates/admin/media/
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.646981 uncms-0.0.8/src/uncms/media/templates/admin/media/file/
+-rw-rw-r--   0 you       (1000) you       (1000)      526 2023-01-15 00:42:46.000000 uncms-0.0.8/src/uncms/media/templates/admin/media/file/change_form.html
+-rw-rw-r--   0 you       (1000) you       (1000)      234 2023-01-21 07:57:32.000000 uncms-0.0.8/src/uncms/media/templates/admin/media/file/change_list.html
+-rw-rw-r--   0 you       (1000) you       (1000)     4487 2023-01-15 00:42:46.000000 uncms-0.0.8/src/uncms/media/templates/admin/media/file/image_editor.html
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.646981 uncms-0.0.8/src/uncms/media/templates/admin/media/includes/
+-rw-rw-r--   0 you       (1000) you       (1000)      856 2023-01-15 00:42:46.000000 uncms-0.0.8/src/uncms/media/templates/admin/media/includes/file_used_on.html
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.646981 uncms-0.0.8/src/uncms/media/templates/admin/widgets/
+-rw-rw-r--   0 you       (1000) you       (1000)      301 2023-01-15 00:42:46.000000 uncms-0.0.8/src/uncms/media/templates/admin/widgets/image_raw_id.html
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.646981 uncms-0.0.8/src/uncms/media/templates/media/
+-rw-rw-r--   0 you       (1000) you       (1000)     1059 2023-01-15 00:42:46.000000 uncms-0.0.8/src/uncms/media/templates/media/multi_format_image.html
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.646981 uncms-0.0.8/src/uncms/media/templatetags/
+-rw-rw-r--   0 you       (1000) you       (1000)        0 2023-01-15 00:42:46.000000 uncms-0.0.8/src/uncms/media/templatetags/__init__.py
+-rw-rw-r--   0 you       (1000) you       (1000)      153 2023-01-15 00:42:46.000000 uncms-0.0.8/src/uncms/media/templatetags/uncms_images.py
+-rw-rw-r--   0 you       (1000) you       (1000)     1987 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/media/types.py
+-rw-rw-r--   0 you       (1000) you       (1000)      423 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/media/urls.py
+-rw-rw-r--   0 you       (1000) you       (1000)     4945 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/media/views.py
+-rw-rw-r--   0 you       (1000) you       (1000)      737 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/media/widgets.py
+-rw-rw-r--   0 you       (1000) you       (1000)     2370 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/middleware.py
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.646981 uncms-0.0.8/src/uncms/models/
+-rw-rw-r--   0 you       (1000) you       (1000)      509 2023-01-15 00:42:46.000000 uncms-0.0.8/src/uncms/models/__init__.py
+-rw-rw-r--   0 you       (1000) you       (1000)    10863 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/models/base.py
+-rw-rw-r--   0 you       (1000) you       (1000)     2652 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/models/fields.py
+-rw-rw-r--   0 you       (1000) you       (1000)     2887 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/models/managers.py
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.646981 uncms-0.0.8/src/uncms/moderation/
+-rw-rw-r--   0 you       (1000) you       (1000)        0 2023-01-15 00:42:46.000000 uncms-0.0.8/src/uncms/moderation/__init__.py
+-rw-rw-r--   0 you       (1000) you       (1000)      949 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/moderation/admin.py
+-rw-rw-r--   0 you       (1000) you       (1000)      749 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/moderation/models.py
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.650981 uncms-0.0.8/src/uncms/pages/
+-rw-rw-r--   0 you       (1000) you       (1000)      155 2023-01-15 00:42:46.000000 uncms-0.0.8/src/uncms/pages/__init__.py
+-rw-rw-r--   0 you       (1000) you       (1000)    28973 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/pages/admin.py
+-rw-rw-r--   0 you       (1000) you       (1000)      400 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/pages/apps.py
+-rw-rw-r--   0 you       (1000) you       (1000)      207 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/pages/context_processors.py
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.630981 uncms-0.0.8/src/uncms/pages/jinja2/
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.650981 uncms-0.0.8/src/uncms/pages/jinja2/pages/
+-rw-rw-r--   0 you       (1000) you       (1000)     1114 2023-01-15 00:42:46.000000 uncms-0.0.8/src/uncms/pages/jinja2/pages/breadcrumbs.jinja2
+-rw-rw-r--   0 you       (1000) you       (1000)      782 2023-01-15 00:42:46.000000 uncms-0.0.8/src/uncms/pages/jinja2/pages/head_meta.jinja2
+-rw-rw-r--   0 you       (1000) you       (1000)     6323 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/pages/middleware.py
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.650981 uncms-0.0.8/src/uncms/pages/migrations/
+-rw-rw-r--   0 you       (1000) you       (1000)     6112 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/pages/migrations/0001_initial.py
+-rw-rw-r--   0 you       (1000) you       (1000)      364 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/pages/migrations/0002_page_requires_authentication.py
+-rw-rw-r--   0 you       (1000) you       (1000)      442 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/pages/migrations/0003_page_hide_from_anonymous.py
+-rw-rw-r--   0 you       (1000) you       (1000)      341 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/pages/migrations/0004_url_title_migration.py
+-rw-rw-r--   0 you       (1000) you       (1000)     4065 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/pages/migrations/0005_social_fields.py
+-rw-rw-r--   0 you       (1000) you       (1000)     4855 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/pages/migrations/0006_auto_20151002_1655.py
+-rw-rw-r--   0 you       (1000) you       (1000)      394 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/pages/migrations/0007_remove_page_cached_url.py
+-rw-rw-r--   0 you       (1000) you       (1000)      567 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/pages/migrations/0008_auto_20191108_1506.py
+-rw-rw-r--   0 you       (1000) you       (1000)      464 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/pages/migrations/0009_auto_20200406_1508.py
+-rw-rw-r--   0 you       (1000) you       (1000)      928 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/pages/migrations/0010_auto_20200812_1546.py
+-rw-rw-r--   0 you       (1000) you       (1000)      875 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/pages/migrations/0011_remove_localisation.py
+-rw-rw-r--   0 you       (1000) you       (1000)        0 2023-01-15 00:42:46.000000 uncms-0.0.8/src/uncms/pages/migrations/__init__.py
+-rw-rw-r--   0 you       (1000) you       (1000)    15434 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/pages/models.py
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.630981 uncms-0.0.8/src/uncms/pages/static/
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.630981 uncms-0.0.8/src/uncms/pages/static/pages/
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.650981 uncms-0.0.8/src/uncms/pages/static/pages/css/
+-rw-rw-r--   0 you       (1000) you       (1000)      922 2023-01-15 00:42:46.000000 uncms-0.0.8/src/uncms/pages/static/pages/css/page-type-selector.css
+-rw-rw-r--   0 you       (1000) you       (1000)     1152 2023-01-15 00:42:46.000000 uncms-0.0.8/src/uncms/pages/static/pages/css/sample-navigation.css
+-rw-rw-r--   0 you       (1000) you       (1000)     1421 2023-01-15 00:42:46.000000 uncms-0.0.8/src/uncms/pages/static/pages/css/sitemap-module.css
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.650981 uncms-0.0.8/src/uncms/pages/static/pages/img/
+-rw-rw-r--   0 you       (1000) you       (1000)     3208 2023-01-15 00:42:46.000000 uncms-0.0.8/src/uncms/pages/static/pages/img/ajax-loader.gif
+-rw-rw-r--   0 you       (1000) you       (1000)      258 2023-01-15 00:42:46.000000 uncms-0.0.8/src/uncms/pages/static/pages/img/arrows.png
+-rw-rw-r--   0 you       (1000) you       (1000)     1239 2023-01-15 00:42:46.000000 uncms-0.0.8/src/uncms/pages/static/pages/img/content.png
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.630981 uncms-0.0.8/src/uncms/pages/templates/
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.630981 uncms-0.0.8/src/uncms/pages/templates/admin/
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.630981 uncms-0.0.8/src/uncms/pages/templates/admin/pages/
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.650981 uncms-0.0.8/src/uncms/pages/templates/admin/pages/page/
+-rw-rw-r--   0 you       (1000) you       (1000)     1330 2023-01-15 00:42:46.000000 uncms-0.0.8/src/uncms/pages/templates/admin/pages/page/select_page_type.html
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.654981 uncms-0.0.8/src/uncms/pages/templates/pages/
+-rw-rw-r--   0 you       (1000) you       (1000)     1114 2023-01-15 00:42:46.000000 uncms-0.0.8/src/uncms/pages/templates/pages/breadcrumbs.html
+-rw-rw-r--   0 you       (1000) you       (1000)      730 2023-01-15 00:42:46.000000 uncms-0.0.8/src/uncms/pages/templates/pages/head_meta.html
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.654981 uncms-0.0.8/src/uncms/pages/templates/pages/navigation/
+-rw-rw-r--   0 you       (1000) you       (1000)      277 2023-01-15 00:42:46.000000 uncms-0.0.8/src/uncms/pages/templates/pages/navigation/navigation.html
+-rw-rw-r--   0 you       (1000) you       (1000)      892 2023-01-15 00:42:46.000000 uncms-0.0.8/src/uncms/pages/templates/pages/navigation/navigation_item.html
+-rw-rw-r--   0 you       (1000) you       (1000)      243 2023-01-15 00:42:46.000000 uncms-0.0.8/src/uncms/pages/templates/pages/navigation/navigation_submenu.html
+-rw-rw-r--   0 you       (1000) you       (1000)      888 2023-01-15 00:42:46.000000 uncms-0.0.8/src/uncms/pages/templates/pages/navigation/navigation_submenu_item.html
+-rw-rw-r--   0 you       (1000) you       (1000)       12 2023-01-15 00:42:46.000000 uncms-0.0.8/src/uncms/pages/templates/pages/title.html
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.654981 uncms-0.0.8/src/uncms/pages/templatetags/
+-rw-rw-r--   0 you       (1000) you       (1000)       43 2023-01-15 00:42:46.000000 uncms-0.0.8/src/uncms/pages/templatetags/__init__.py
+-rw-rw-r--   0 you       (1000) you       (1000)    11938 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/pages/templatetags/_common.py
+-rw-rw-r--   0 you       (1000) you       (1000)     4820 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/pages/templatetags/uncms_pages.py
+-rw-rw-r--   0 you       (1000) you       (1000)     3501 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/pages/types.py
+-rw-rw-r--   0 you       (1000) you       (1000)      254 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/pages/urls.py
+-rw-rw-r--   0 you       (1000) you       (1000)      948 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/pages/views.py
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.654981 uncms-0.0.8/src/uncms/plugins/
+-rw-rw-r--   0 you       (1000) you       (1000)        0 2023-01-15 00:42:46.000000 uncms-0.0.8/src/uncms/plugins/__init__.py
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.654981 uncms-0.0.8/src/uncms/redirects/
+-rw-rw-r--   0 you       (1000) you       (1000)        0 2023-02-12 13:06:23.000000 uncms-0.0.8/src/uncms/redirects/__init__.py
+-rw-rw-r--   0 you       (1000) you       (1000)     5149 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/redirects/admin.py
+-rw-rw-r--   0 you       (1000) you       (1000)      156 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/redirects/apps.py
+-rw-rw-r--   0 you       (1000) you       (1000)     1666 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/redirects/forms.py
+-rw-rw-r--   0 you       (1000) you       (1000)     4268 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/redirects/importer.py
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.654981 uncms-0.0.8/src/uncms/redirects/management/
+-rw-rw-r--   0 you       (1000) you       (1000)        0 2023-02-12 13:06:23.000000 uncms-0.0.8/src/uncms/redirects/management/__init__.py
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.654981 uncms-0.0.8/src/uncms/redirects/management/commands/
+-rw-rw-r--   0 you       (1000) you       (1000)        0 2023-02-12 13:06:23.000000 uncms-0.0.8/src/uncms/redirects/management/commands/__init__.py
+-rw-rw-r--   0 you       (1000) you       (1000)     2618 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/redirects/management/commands/import_redirects_csv.py
+-rw-rw-r--   0 you       (1000) you       (1000)      976 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/redirects/middleware.py
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.654981 uncms-0.0.8/src/uncms/redirects/migrations/
+-rw-rw-r--   0 you       (1000) you       (1000)     1713 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/redirects/migrations/0001_initial.py
+-rw-rw-r--   0 you       (1000) you       (1000)        0 2023-02-12 13:06:23.000000 uncms-0.0.8/src/uncms/redirects/migrations/__init__.py
+-rw-rw-r--   0 you       (1000) you       (1000)     7823 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/redirects/models.py
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.630981 uncms-0.0.8/src/uncms/redirects/static/
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.630981 uncms-0.0.8/src/uncms/redirects/static/uncms/
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.654981 uncms-0.0.8/src/uncms/redirects/static/uncms/js/
+-rw-rw-r--   0 you       (1000) you       (1000)      876 2023-02-12 13:06:23.000000 uncms-0.0.8/src/uncms/redirects/static/uncms/js/redirect-fields.js
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.630981 uncms-0.0.8/src/uncms/redirects/templates/
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.630981 uncms-0.0.8/src/uncms/redirects/templates/admin/
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.630981 uncms-0.0.8/src/uncms/redirects/templates/admin/redirects/
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.654981 uncms-0.0.8/src/uncms/redirects/templates/admin/redirects/redirect/
+-rw-rw-r--   0 you       (1000) you       (1000)      366 2023-02-12 13:06:23.000000 uncms-0.0.8/src/uncms/redirects/templates/admin/redirects/redirect/change_list.html
+-rw-rw-r--   0 you       (1000) you       (1000)     3572 2023-02-12 13:06:23.000000 uncms-0.0.8/src/uncms/redirects/templates/admin/redirects/redirect/import_form.html
+-rw-rw-r--   0 you       (1000) you       (1000)      214 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/redirects/types.py
+-rw-rw-r--   0 you       (1000) you       (1000)     2368 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/robots.py
+-rw-rw-r--   0 you       (1000) you       (1000)     3059 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/sitemaps.py
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.630981 uncms-0.0.8/src/uncms/static/
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.630981 uncms-0.0.8/src/uncms/static/cms/
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.630981 uncms-0.0.8/src/uncms/static/cms/js/
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.658981 uncms-0.0.8/src/uncms/static/cms/js/imgeditor/
+-rw-rw-r--   0 you       (1000) you       (1000)    31397 2023-01-15 00:42:46.000000 uncms-0.0.8/src/uncms/static/cms/js/imgeditor/image-editor.css
+-rw-rw-r--   0 you       (1000) you       (1000)  1589044 2023-01-15 00:42:46.000000 uncms-0.0.8/src/uncms/static/cms/js/imgeditor/image-editor.js
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.630981 uncms-0.0.8/src/uncms/static/cms/svg/
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.666981 uncms-0.0.8/src/uncms/static/cms/svg/image-editor/
+-rwxrwxr-x   0 you       (1000) you       (1000)    20048 2023-01-15 00:42:46.000000 uncms-0.0.8/src/uncms/static/cms/svg/image-editor/icon-a.svg
+-rwxrwxr-x   0 you       (1000) you       (1000)    19665 2023-01-15 00:42:46.000000 uncms-0.0.8/src/uncms/static/cms/svg/image-editor/icon-b.svg
+-rwxrwxr-x   0 you       (1000) you       (1000)    19665 2023-01-15 00:42:46.000000 uncms-0.0.8/src/uncms/static/cms/svg/image-editor/icon-c.svg
+-rwxrwxr-x   0 you       (1000) you       (1000)    19665 2023-01-15 00:42:46.000000 uncms-0.0.8/src/uncms/static/cms/svg/image-editor/icon-d.svg
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.630981 uncms-0.0.8/src/uncms/static/uncms/
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.666981 uncms-0.0.8/src/uncms/static/uncms/css/
+-rw-rw-r--   0 you       (1000) you       (1000)      878 2023-01-27 01:17:56.000000 uncms-0.0.8/src/uncms/static/uncms/css/trumbowyg-tweak.css
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.666981 uncms-0.0.8/src/uncms/static/uncms/js/
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.666981 uncms-0.0.8/src/uncms/static/uncms/js/trumbowyg-imagelibrary/
+-rw-rw-r--   0 you       (1000) you       (1000)     8285 2023-02-19 16:07:10.000000 uncms-0.0.8/src/uncms/static/uncms/js/trumbowyg-imagelibrary/trumbowyg.imagelibrary.js
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.670981 uncms-0.0.8/src/uncms/static/uncms/js/trumbowyg-imagelibrary/ui/
+-rw-rw-r--   0 you       (1000) you       (1000)     1288 2023-01-21 07:57:32.000000 uncms-0.0.8/src/uncms/static/uncms/js/trumbowyg-imagelibrary/ui/trumbowyg.imagelibrary.css
+-rw-rw-r--   0 you       (1000) you       (1000)     2180 2023-03-12 15:51:22.000000 uncms-0.0.8/src/uncms/static/uncms/js/wysiwyg.js
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.630981 uncms-0.0.8/src/uncms/static/uncms/vendor/
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.670981 uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.678981 uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/
+-rw-rw-r--   0 you       (1000) you       (1000)     1664 2022-11-14 15:37:02.000000 uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/ar.js
+-rw-rw-r--   0 you       (1000) you       (1000)     1559 2022-11-14 15:37:02.000000 uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/bg.js
+-rw-rw-r--   0 you       (1000) you       (1000)     2060 2022-11-14 15:37:02.000000 uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/bn.js
+-rw-rw-r--   0 you       (1000) you       (1000)     1762 2022-11-14 15:37:02.000000 uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/by.js
+-rw-rw-r--   0 you       (1000) you       (1000)     1349 2022-11-14 15:37:02.000000 uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/ca.js
+-rw-rw-r--   0 you       (1000) you       (1000)     1454 2022-11-14 15:37:02.000000 uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/cs.js
+-rw-rw-r--   0 you       (1000) you       (1000)     1420 2022-11-14 15:37:02.000000 uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/da.js
+-rw-rw-r--   0 you       (1000) you       (1000)     1343 2022-11-14 15:37:02.000000 uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/de.js
+-rw-rw-r--   0 you       (1000) you       (1000)     1888 2022-11-14 15:37:02.000000 uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/el.js
+-rw-rw-r--   0 you       (1000) you       (1000)     1430 2022-11-14 15:37:02.000000 uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/es.js
+-rw-rw-r--   0 you       (1000) you       (1000)     1325 2022-11-14 15:37:02.000000 uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/es_ar.js
+-rw-rw-r--   0 you       (1000) you       (1000)     1437 2022-11-14 15:37:02.000000 uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/et.js
+-rw-rw-r--   0 you       (1000) you       (1000)     1492 2022-11-14 15:37:02.000000 uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/fa.js
+-rw-rw-r--   0 you       (1000) you       (1000)     1299 2022-11-14 15:37:02.000000 uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/fi.js
+-rw-rw-r--   0 you       (1000) you       (1000)     1623 2022-11-14 15:37:02.000000 uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/fr.js
+-rw-rw-r--   0 you       (1000) you       (1000)     1382 2022-11-14 15:37:02.000000 uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/he.js
+-rw-rw-r--   0 you       (1000) you       (1000)     1302 2022-11-14 15:37:02.000000 uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/hr.js
+-rw-rw-r--   0 you       (1000) you       (1000)     1361 2022-11-14 15:37:02.000000 uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/hu.js
+-rw-rw-r--   0 you       (1000) you       (1000)     1338 2022-11-14 15:37:02.000000 uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/id.js
+-rw-rw-r--   0 you       (1000) you       (1000)     1405 2022-11-14 15:37:02.000000 uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/it.js
+-rw-rw-r--   0 you       (1000) you       (1000)     1495 2022-11-14 15:37:02.000000 uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/ja.js
+-rw-rw-r--   0 you       (1000) you       (1000)     1558 2022-11-14 15:37:02.000000 uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/ko.js
+-rw-rw-r--   0 you       (1000) you       (1000)     1381 2022-11-14 15:37:02.000000 uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/lt.js
+-rw-rw-r--   0 you       (1000) you       (1000)     1641 2022-11-14 15:37:02.000000 uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/mn.js
+-rw-rw-r--   0 you       (1000) you       (1000)     1240 2022-11-14 15:37:02.000000 uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/my.js
+-rw-rw-r--   0 you       (1000) you       (1000)     1381 2022-11-14 15:37:02.000000 uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/nl.js
+-rw-rw-r--   0 you       (1000) you       (1000)     1287 2022-11-14 15:37:02.000000 uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/no_nb.js
+-rw-rw-r--   0 you       (1000) you       (1000)     1251 2022-11-14 15:37:02.000000 uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/ph.js
+-rw-rw-r--   0 you       (1000) you       (1000)     1273 2022-11-14 15:37:02.000000 uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/pl.js
+-rw-rw-r--   0 you       (1000) you       (1000)     1547 2022-11-14 15:37:02.000000 uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/pt.js
+-rw-rw-r--   0 you       (1000) you       (1000)     1543 2022-11-14 15:37:02.000000 uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/pt_br.js
+-rw-rw-r--   0 you       (1000) you       (1000)     1407 2022-11-14 15:37:02.000000 uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/ro.js
+-rw-rw-r--   0 you       (1000) you       (1000)     1563 2022-11-14 15:37:02.000000 uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/rs.js
+-rw-rw-r--   0 you       (1000) you       (1000)     1326 2022-11-14 15:37:02.000000 uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/rs_latin.js
+-rw-rw-r--   0 you       (1000) you       (1000)     1785 2022-11-14 15:37:02.000000 uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/ru.js
+-rw-rw-r--   0 you       (1000) you       (1000)     1281 2022-11-14 15:37:02.000000 uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/sk.js
+-rw-rw-r--   0 you       (1000) you       (1000)     1373 2022-11-14 15:37:02.000000 uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/sl.js
+-rw-rw-r--   0 you       (1000) you       (1000)     1401 2022-11-14 15:37:02.000000 uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/sq.js
+-rw-rw-r--   0 you       (1000) you       (1000)     1330 2022-11-14 15:37:02.000000 uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/sv.js
+-rw-rw-r--   0 you       (1000) you       (1000)     1530 2022-11-14 15:37:02.000000 uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/th.js
+-rw-rw-r--   0 you       (1000) you       (1000)     1437 2022-11-14 15:37:02.000000 uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/tr.js
+-rw-rw-r--   0 you       (1000) you       (1000)     1583 2022-11-14 15:37:02.000000 uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/ua.js
+-rw-rw-r--   0 you       (1000) you       (1000)     1392 2022-11-14 15:37:02.000000 uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/vi.js
+-rw-rw-r--   0 you       (1000) you       (1000)     1281 2022-11-14 15:37:02.000000 uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/zh_cn.js
+-rw-rw-r--   0 you       (1000) you       (1000)     1489 2022-11-14 15:37:02.000000 uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/zh_tw.js
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.634981 uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/plugins/
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.678981 uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/plugins/cleanpaste/
+-rw-rw-r--   0 you       (1000) you       (1000)     5821 2022-11-14 15:37:02.000000 uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/plugins/cleanpaste/trumbowyg.cleanpaste.js
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.678981 uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/plugins/preformatted/
+-rw-rw-r--   0 you       (1000) you       (1000)     4799 2022-11-14 15:37:02.000000 uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/plugins/preformatted/trumbowyg.preformatted.js
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.678981 uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/plugins/table/
+-rw-rw-r--   0 you       (1000) you       (1000)    19549 2022-11-14 15:37:02.000000 uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/plugins/table/trumbowyg.table.js
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.678981 uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/plugins/table/ui/
+-rw-rw-r--   0 you       (1000) you       (1000)      969 2022-11-14 15:37:02.000000 uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/plugins/table/ui/trumbowyg.table.css
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.678981 uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/plugins/upload/
+-rw-rw-r--   0 you       (1000) you       (1000)    12986 2022-11-14 15:37:02.000000 uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/plugins/upload/trumbowyg.upload.js
+-rw-rw-r--   0 you       (1000) you       (1000)    71140 2022-11-14 15:37:02.000000 uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/trumbowyg.js
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.678981 uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/ui/
+-rw-rw-r--   0 you       (1000) you       (1000)    30702 2022-11-14 15:37:02.000000 uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/ui/icons.svg
+-rw-rw-r--   0 you       (1000) you       (1000)    22676 2022-11-14 15:37:02.000000 uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/ui/trumbowyg.css
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.678981 uncms-0.0.8/src/uncms/templates/
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.634981 uncms-0.0.8/src/uncms/templates/admin/
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.678981 uncms-0.0.8/src/uncms/templates/admin/dashboard_modules/
+-rw-rw-r--   0 you       (1000) you       (1000)      506 2023-01-15 00:42:46.000000 uncms-0.0.8/src/uncms/templates/admin/dashboard_modules/sitemap.html
+-rw-rw-r--   0 you       (1000) you       (1000)     2095 2023-01-15 00:42:46.000000 uncms-0.0.8/src/uncms/templates/admin/dashboard_modules/sitemap_items.html
+-rw-rw-r--   0 you       (1000) you       (1000)      491 2023-01-15 00:42:46.000000 uncms-0.0.8/src/uncms/templates/base.html
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.682981 uncms-0.0.8/src/uncms/templates/pagination/
+-rw-rw-r--   0 you       (1000) you       (1000)      897 2023-01-15 00:42:46.000000 uncms-0.0.8/src/uncms/templates/pagination/pagination.html
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.682981 uncms-0.0.8/src/uncms/templatetags/
+-rw-rw-r--   0 you       (1000) you       (1000)       41 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/templatetags/__init__.py
+-rw-rw-r--   0 you       (1000) you       (1000)      826 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/templatetags/_common.py
+-rw-rw-r--   0 you       (1000) you       (1000)      245 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/templatetags/uncms_html.py
+-rw-rw-r--   0 you       (1000) you       (1000)     1637 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/templatetags/uncms_pagination.py
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.682981 uncms-0.0.8/src/uncms/testhelpers/
+-rw-rw-r--   0 you       (1000) you       (1000)        0 2023-03-13 03:29:20.000000 uncms-0.0.8/src/uncms/testhelpers/__init__.py
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.682981 uncms-0.0.8/src/uncms/testhelpers/factories/
+-rw-rw-r--   0 you       (1000) you       (1000)     1400 2023-03-13 03:31:07.000000 uncms-0.0.8/src/uncms/testhelpers/factories/__init__.py
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.682981 uncms-0.0.8/src/uncms/testhelpers/factories/data/
+-rw-rw-r--   0 you       (1000) you       (1000)    46607 2023-03-13 03:36:43.000000 uncms-0.0.8/src/uncms/testhelpers/factories/data/1920x1080.jpg
+-rw-rw-r--   0 you       (1000) you       (1000)     7940 2023-03-13 03:36:43.000000 uncms-0.0.8/src/uncms/testhelpers/factories/data/1920x1080.png
+-rw-rw-r--   0 you       (1000) you       (1000)    11498 2023-03-13 03:36:43.000000 uncms-0.0.8/src/uncms/testhelpers/factories/data/1920x1080.webp
+-rw-rw-r--   0 you       (1000) you       (1000)     9722 2023-03-13 03:36:43.000000 uncms-0.0.8/src/uncms/testhelpers/factories/data/800x600.png
+-rw-rw-r--   0 you       (1000) you       (1000)     1369 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/testhelpers/factories/media.py
+-rw-rw-r--   0 you       (1000) you       (1000)     2296 2023-03-13 04:28:44.000000 uncms-0.0.8/src/uncms/testhelpers/factories/pages.py
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.682981 uncms-0.0.8/src/uncms/testhelpers/migrations/
+-rw-rw-r--   0 you       (1000) you       (1000)      649 2023-03-13 04:46:59.000000 uncms-0.0.8/src/uncms/testhelpers/migrations/0001_initial.py
+-rw-rw-r--   0 you       (1000) you       (1000)        0 2023-03-13 04:45:24.000000 uncms-0.0.8/src/uncms/testhelpers/migrations/__init__.py
+-rw-rw-r--   0 you       (1000) you       (1000)       88 2023-03-13 04:28:06.000000 uncms-0.0.8/src/uncms/testhelpers/models.py
+-rw-rw-r--   0 you       (1000) you       (1000)      581 2023-02-18 21:37:05.000000 uncms-0.0.8/src/uncms/utils.py
+-rw-rw-r--   0 you       (1000) you       (1000)     1183 2023-03-15 03:12:57.000000 uncms-0.0.8/src/uncms/views.py
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.638981 uncms-0.0.8/src/uncms.egg-info/
+-rw-rw-r--   0 you       (1000) you       (1000)     1065 2023-04-16 17:14:25.000000 uncms-0.0.8/src/uncms.egg-info/PKG-INFO
+-rw-rw-r--   0 you       (1000) you       (1000)    10384 2023-04-16 17:14:25.000000 uncms-0.0.8/src/uncms.egg-info/SOURCES.txt
+-rw-rw-r--   0 you       (1000) you       (1000)        1 2023-04-16 17:14:25.000000 uncms-0.0.8/src/uncms.egg-info/dependency_links.txt
+-rw-rw-r--   0 you       (1000) you       (1000)      370 2023-04-16 17:14:25.000000 uncms-0.0.8/src/uncms.egg-info/requires.txt
+-rw-rw-r--   0 you       (1000) you       (1000)        6 2023-04-16 17:14:25.000000 uncms-0.0.8/src/uncms.egg-info/top_level.txt
+drwxrwxr-x   0 you       (1000) you       (1000)        0 2023-04-16 17:14:25.686981 uncms-0.0.8/tests/
+-rw-rw-r--   0 you       (1000) you       (1000)     2303 2023-03-13 03:42:31.000000 uncms-0.0.8/tests/test_admin.py
+-rw-rw-r--   0 you       (1000) you       (1000)     2606 2023-03-13 03:36:43.000000 uncms-0.0.8/tests/test_checks.py
+-rw-rw-r--   0 you       (1000) you       (1000)     1789 2023-03-13 03:36:43.000000 uncms-0.0.8/tests/test_conf.py
+-rw-rw-r--   0 you       (1000) you       (1000)     1225 2023-03-13 03:36:43.000000 uncms-0.0.8/tests/test_forms.py
+-rw-rw-r--   0 you       (1000) you       (1000)     3811 2023-03-13 03:42:31.000000 uncms-0.0.8/tests/test_html.py
+-rw-rw-r--   0 you       (1000) you       (1000)      437 2023-03-13 03:36:44.000000 uncms-0.0.8/tests/test_jinja2_environment.py
+-rw-rw-r--   0 you       (1000) you       (1000)     2493 2023-03-13 03:42:31.000000 uncms-0.0.8/tests/test_middleware.py
+-rw-rw-r--   0 you       (1000) you       (1000)      622 2023-03-13 03:36:44.000000 uncms-0.0.8/tests/test_models.py
+-rw-rw-r--   0 you       (1000) you       (1000)     3146 2023-03-13 03:36:43.000000 uncms-0.0.8/tests/test_models_base.py
+-rw-rw-r--   0 you       (1000) you       (1000)      949 2023-03-13 03:36:44.000000 uncms-0.0.8/tests/test_models_fields.py
+-rw-rw-r--   0 you       (1000) you       (1000)     5537 2023-03-13 03:36:43.000000 uncms-0.0.8/tests/test_robots.py
+-rw-rw-r--   0 you       (1000) you       (1000)     1718 2023-03-13 03:36:43.000000 uncms-0.0.8/tests/test_sitemaps.py
+-rw-rw-r--   0 you       (1000) you       (1000)      256 2023-03-13 03:36:43.000000 uncms-0.0.8/tests/test_templatetags_html.py
+-rw-rw-r--   0 you       (1000) you       (1000)      962 2023-03-13 03:36:43.000000 uncms-0.0.8/tests/test_templatetags_pagination.py
+-rw-rw-r--   0 you       (1000) you       (1000)      595 2023-03-13 03:36:43.000000 uncms-0.0.8/tests/test_utils.py
+-rw-rw-r--   0 you       (1000) you       (1000)      794 2023-03-13 03:36:43.000000 uncms-0.0.8/tests/test_views.py
```

### Comparing `uncms-0.0.7/LICENSE` & `uncms-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/PKG-INFO` & `uncms-0.0.8/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: uncms
-Version: 0.0.7
+Version: 0.0.8
 Summary: A CMS toolkit for Django emphasising simplicity, speed, and familiarity.
 Author-email: Lewis Collard <lewiscollard@gmail.com>
 Project-URL: homepage, https://uncms.dev/
 Project-URL: documentation, https://docs.uncms.dev/
 Project-URL: repository, https://github.com/uncms-dev/uncms
 Classifier: Development Status :: 3 - Alpha
-Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: jinja2
+Provides-Extra: testhelpers
 License-File: LICENSE
 
 # UnCMS: a developer's CMS toolkit for Django
 
 **Warning: UnCMS is in alpha. It is recommended only for the curious and fearless. Do not use it in production.**
 
 UnCMS is a developer's CMS toolkit for Django emphasising simplicity, speed, and familiarity.
```

### Comparing `uncms-0.0.7/pyproject.toml` & `uncms-0.0.8/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "uncms"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
     { name="Lewis Collard", email="lewiscollard@gmail.com" },
 ]
 readme = "README.md"
 description = "A CMS toolkit for Django emphasising simplicity, speed, and familiarity."
-requires-python = ">=3.6"
+requires-python = ">=3.8"
 classifiers = [
     "Development Status :: 3 - Alpha",
-    "Framework :: Django :: 3.2",
+    "Framework :: Django :: 4.2",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: BSD License",
 ]
 
 dependencies = [
     "Pillow",
     "sorl-thumbnail",
     "beautifulsoup4",
     "bleach>=5.0.1,<6",
-    "django>=3.2,<4.2",
+    "django>=4.2,<4.3",
     "django-watson",
     "django-reversion",
     "python-magic>=0.4.15",
 ]
 
 [project.optional-dependencies]
 dev = [
@@ -45,11 +45,15 @@
     "twine==4.0.2",
 ]
 
 jinja2 = [
     "Jinja2>=3.1.2,<4",
 ]
 
+testhelpers = [
+    "factory-boy==3.2.1",
+]
+
 [project.urls]
 "homepage" = "https://uncms.dev/"
 "documentation" = "https://docs.uncms.dev/"
 "repository" = "https://github.com/uncms-dev/uncms"
```

### Comparing `uncms-0.0.7/src/uncms/admin.py` & `uncms-0.0.8/src/uncms/admin.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/checks.py` & `uncms-0.0.8/src/uncms/checks.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/conf.py` & `uncms-0.0.8/src/uncms/conf.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/forms.py` & `uncms-0.0.8/src/uncms/forms.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/html.py` & `uncms-0.0.8/src/uncms/html.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/jinja2_environment/all.py` & `uncms-0.0.8/src/uncms/jinja2_environment/all.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/jinja2_environment/pages.py` & `uncms-0.0.8/src/uncms/jinja2_environment/pages.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/links/migrations/0001_initial.py` & `uncms-0.0.8/src/uncms/links/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/links/migrations/0002_auto_20171020_1320.py` & `uncms-0.0.8/src/uncms/links/migrations/0002_auto_20171020_1320.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/links/migrations/0004_link_permanent_redirect.py` & `uncms-0.0.8/src/uncms/links/migrations/0004_link_permanent_redirect.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/links/models.py` & `uncms-0.0.8/src/uncms/links/models.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/links/static/links/img/link.png` & `uncms-0.0.8/src/uncms/links/static/links/img/link.png`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/media/admin.py` & `uncms-0.0.8/src/uncms/media/admin.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/media/fields.py` & `uncms-0.0.8/src/uncms/media/fields.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/media/filetypes.py` & `uncms-0.0.8/src/uncms/media/filetypes.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/media/forms.py` & `uncms-0.0.8/src/uncms/media/forms.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/media/migrations/0001_initial.py` & `uncms-0.0.8/src/uncms/media/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/media/migrations/0002_auto_20150713_1408.py` & `uncms-0.0.8/src/uncms/media/migrations/0002_auto_20150713_1408.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/media/migrations/0004_auto_20170407_1442.py` & `uncms-0.0.8/src/uncms/media/migrations/0004_auto_20170407_1442.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/media/migrations/0005_auto_20171107_1537.py` & `uncms-0.0.8/src/uncms/media/migrations/0005_auto_20171107_1537.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/media/migrations/0007_auto_20180801_1419.py` & `uncms-0.0.8/src/uncms/media/migrations/0007_auto_20180801_1419.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/media/migrations/0009_auto_20181207_1318.py` & `uncms-0.0.8/src/uncms/media/migrations/0009_auto_20181207_1318.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/media/migrations/0010_auto_20190523_1638.py` & `uncms-0.0.8/src/uncms/media/migrations/0010_auto_20190523_1638.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/media/models.py` & `uncms-0.0.8/src/uncms/media/models.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/media/static/media/css/media-list.css` & `uncms-0.0.8/src/uncms/media/static/media/css/media-list.css`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/media/static/media/img/audio-x-generic.png` & `uncms-0.0.8/src/uncms/media/static/media/img/audio-x-generic.png`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/media/static/media/img/image-x-generic.png` & `uncms-0.0.8/src/uncms/media/static/media/img/image-x-generic.png`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/media/static/media/img/text-x-generic-template.png` & `uncms-0.0.8/src/uncms/media/static/media/img/text-x-generic-template.png`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/media/static/media/img/text-x-generic.png` & `uncms-0.0.8/src/uncms/media/static/media/img/text-x-generic.png`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/media/static/media/img/video-x-generic.png` & `uncms-0.0.8/src/uncms/media/static/media/img/video-x-generic.png`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/media/static/media/img/x-office-document.png` & `uncms-0.0.8/src/uncms/media/static/media/img/x-office-document.png`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/media/static/media/img/x-office-spreadsheet.png` & `uncms-0.0.8/src/uncms/media/static/media/img/x-office-spreadsheet.png`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/media/static/media/js/prepopulate-title.js` & `uncms-0.0.8/src/uncms/media/static/media/js/prepopulate-title.js`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/media/templates/admin/media/file/change_form.html` & `uncms-0.0.8/src/uncms/media/templates/admin/media/file/change_form.html`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/media/templates/admin/media/file/image_editor.html` & `uncms-0.0.8/src/uncms/media/templates/admin/media/file/image_editor.html`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/media/templates/admin/media/includes/file_used_on.html` & `uncms-0.0.8/src/uncms/media/templates/admin/media/includes/file_used_on.html`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/media/templates/media/multi_format_image.html` & `uncms-0.0.8/src/uncms/media/templates/media/multi_format_image.html`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/media/types.py` & `uncms-0.0.8/src/uncms/media/types.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/media/views.py` & `uncms-0.0.8/src/uncms/media/views.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/media/widgets.py` & `uncms-0.0.8/src/uncms/media/widgets.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/middleware.py` & `uncms-0.0.8/src/uncms/middleware.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/models/base.py` & `uncms-0.0.8/src/uncms/models/base.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/models/fields.py` & `uncms-0.0.8/src/uncms/models/fields.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/models/managers.py` & `uncms-0.0.8/src/uncms/models/managers.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/moderation/admin.py` & `uncms-0.0.8/src/uncms/moderation/admin.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/moderation/models.py` & `uncms-0.0.8/src/uncms/moderation/models.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/pages/admin.py` & `uncms-0.0.8/src/uncms/pages/admin.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/pages/jinja2/pages/breadcrumbs.jinja2` & `uncms-0.0.8/src/uncms/pages/jinja2/pages/breadcrumbs.jinja2`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/pages/jinja2/pages/head_meta.jinja2` & `uncms-0.0.8/src/uncms/pages/jinja2/pages/head_meta.jinja2`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/pages/middleware.py` & `uncms-0.0.8/src/uncms/pages/middleware.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/pages/migrations/0001_initial.py` & `uncms-0.0.8/src/uncms/pages/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/pages/migrations/0005_social_fields.py` & `uncms-0.0.8/src/uncms/pages/migrations/0005_social_fields.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/pages/migrations/0006_auto_20151002_1655.py` & `uncms-0.0.8/src/uncms/pages/migrations/0006_auto_20151002_1655.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/pages/migrations/0008_auto_20191108_1506.py` & `uncms-0.0.8/src/uncms/pages/migrations/0008_auto_20191108_1506.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/pages/migrations/0010_auto_20200812_1546.py` & `uncms-0.0.8/src/uncms/pages/migrations/0010_auto_20200812_1546.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/pages/migrations/0011_remove_localisation.py` & `uncms-0.0.8/src/uncms/pages/migrations/0011_remove_localisation.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/pages/models.py` & `uncms-0.0.8/src/uncms/pages/models.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/pages/static/pages/css/page-type-selector.css` & `uncms-0.0.8/src/uncms/pages/static/pages/css/page-type-selector.css`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/pages/static/pages/css/sample-navigation.css` & `uncms-0.0.8/src/uncms/pages/static/pages/css/sample-navigation.css`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/pages/static/pages/css/sitemap-module.css` & `uncms-0.0.8/src/uncms/pages/static/pages/css/sitemap-module.css`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/pages/static/pages/img/ajax-loader.gif` & `uncms-0.0.8/src/uncms/pages/static/pages/img/ajax-loader.gif`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/pages/static/pages/img/content.png` & `uncms-0.0.8/src/uncms/pages/static/pages/img/content.png`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/pages/templates/admin/pages/page/select_page_type.html` & `uncms-0.0.8/src/uncms/pages/templates/admin/pages/page/select_page_type.html`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/pages/templates/pages/breadcrumbs.html` & `uncms-0.0.8/src/uncms/pages/templates/pages/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/pages/templates/pages/head_meta.html` & `uncms-0.0.8/src/uncms/pages/templates/pages/head_meta.html`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/pages/templates/pages/navigation/navigation_item.html` & `uncms-0.0.8/src/uncms/pages/templates/pages/navigation/navigation_item.html`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/pages/templates/pages/navigation/navigation_submenu_item.html` & `uncms-0.0.8/src/uncms/pages/templates/pages/navigation/navigation_submenu_item.html`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/pages/templatetags/_common.py` & `uncms-0.0.8/src/uncms/pages/templatetags/_common.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/pages/templatetags/uncms_pages.py` & `uncms-0.0.8/src/uncms/pages/templatetags/uncms_pages.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/pages/types.py` & `uncms-0.0.8/src/uncms/pages/types.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/pages/views.py` & `uncms-0.0.8/src/uncms/pages/views.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/redirects/admin.py` & `uncms-0.0.8/src/uncms/redirects/admin.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/redirects/forms.py` & `uncms-0.0.8/src/uncms/redirects/forms.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/redirects/importer.py` & `uncms-0.0.8/src/uncms/redirects/importer.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/redirects/management/commands/import_redirects_csv.py` & `uncms-0.0.8/src/uncms/redirects/management/commands/import_redirects_csv.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/redirects/middleware.py` & `uncms-0.0.8/src/uncms/redirects/middleware.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/redirects/migrations/0001_initial.py` & `uncms-0.0.8/src/uncms/redirects/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/redirects/models.py` & `uncms-0.0.8/src/uncms/redirects/models.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/redirects/static/uncms/js/redirect-fields.js` & `uncms-0.0.8/src/uncms/redirects/static/uncms/js/redirect-fields.js`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/redirects/templates/admin/redirects/redirect/import_form.html` & `uncms-0.0.8/src/uncms/redirects/templates/admin/redirects/redirect/import_form.html`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/robots.py` & `uncms-0.0.8/src/uncms/robots.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/sitemaps.py` & `uncms-0.0.8/src/uncms/sitemaps.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/static/cms/js/imgeditor/image-editor.css` & `uncms-0.0.8/src/uncms/static/cms/js/imgeditor/image-editor.css`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/static/cms/js/imgeditor/image-editor.js` & `uncms-0.0.8/src/uncms/static/cms/js/imgeditor/image-editor.js`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/static/cms/svg/image-editor/icon-a.svg` & `uncms-0.0.8/src/uncms/static/cms/svg/image-editor/icon-a.svg`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/static/cms/svg/image-editor/icon-b.svg` & `uncms-0.0.8/src/uncms/static/cms/svg/image-editor/icon-b.svg`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/static/cms/svg/image-editor/icon-c.svg` & `uncms-0.0.8/src/uncms/static/cms/svg/image-editor/icon-c.svg`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/static/cms/svg/image-editor/icon-d.svg` & `uncms-0.0.8/src/uncms/static/cms/svg/image-editor/icon-d.svg`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/static/uncms/css/trumbowyg-tweak.css` & `uncms-0.0.8/src/uncms/static/uncms/css/trumbowyg-tweak.css`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/static/uncms/js/trumbowyg-imagelibrary/trumbowyg.imagelibrary.js` & `uncms-0.0.8/src/uncms/static/uncms/js/trumbowyg-imagelibrary/trumbowyg.imagelibrary.js`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/static/uncms/js/trumbowyg-imagelibrary/ui/trumbowyg.imagelibrary.css` & `uncms-0.0.8/src/uncms/static/uncms/js/trumbowyg-imagelibrary/ui/trumbowyg.imagelibrary.css`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/static/uncms/js/wysiwyg.js` & `uncms-0.0.8/src/uncms/static/uncms/js/wysiwyg.js`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/ar.js` & `uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/ar.js`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/bg.js` & `uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/bg.js`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/bn.js` & `uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/bn.js`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/by.js` & `uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/by.js`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/ca.js` & `uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/ca.js`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/cs.js` & `uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/cs.js`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/da.js` & `uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/da.js`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/de.js` & `uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/de.js`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/el.js` & `uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/el.js`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/es.js` & `uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/es.js`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/es_ar.js` & `uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/es_ar.js`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/et.js` & `uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/et.js`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/fa.js` & `uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/fa.js`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/fi.js` & `uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/fi.js`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/fr.js` & `uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/fr.js`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/he.js` & `uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/he.js`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/hr.js` & `uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/hr.js`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/hu.js` & `uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/hu.js`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/id.js` & `uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/id.js`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/it.js` & `uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/it.js`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/ja.js` & `uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/ja.js`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/ko.js` & `uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/ko.js`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/lt.js` & `uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/lt.js`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/mn.js` & `uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/mn.js`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/my.js` & `uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/my.js`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/nl.js` & `uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/nl.js`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/no_nb.js` & `uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/no_nb.js`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/ph.js` & `uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/ph.js`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/pl.js` & `uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/pl.js`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/pt.js` & `uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/pt.js`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/pt_br.js` & `uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/pt_br.js`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/ro.js` & `uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/ro.js`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/rs.js` & `uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/rs.js`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/rs_latin.js` & `uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/rs_latin.js`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/ru.js` & `uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/ru.js`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/sk.js` & `uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/sk.js`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/sl.js` & `uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/sl.js`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/sq.js` & `uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/sq.js`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/sv.js` & `uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/sv.js`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/th.js` & `uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/th.js`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/tr.js` & `uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/tr.js`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/ua.js` & `uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/ua.js`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/vi.js` & `uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/vi.js`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/zh_cn.js` & `uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/zh_cn.js`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/langs/zh_tw.js` & `uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/langs/zh_tw.js`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/plugins/cleanpaste/trumbowyg.cleanpaste.js` & `uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/plugins/cleanpaste/trumbowyg.cleanpaste.js`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/plugins/preformatted/trumbowyg.preformatted.js` & `uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/plugins/preformatted/trumbowyg.preformatted.js`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/plugins/table/trumbowyg.table.js` & `uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/plugins/table/trumbowyg.table.js`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/plugins/table/ui/trumbowyg.table.css` & `uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/plugins/table/ui/trumbowyg.table.css`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/plugins/upload/trumbowyg.upload.js` & `uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/plugins/upload/trumbowyg.upload.js`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/trumbowyg.js` & `uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/trumbowyg.js`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/ui/icons.svg` & `uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/ui/icons.svg`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/static/uncms/vendor/trumbowyg/ui/trumbowyg.css` & `uncms-0.0.8/src/uncms/static/uncms/vendor/trumbowyg/ui/trumbowyg.css`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/templates/admin/dashboard_modules/sitemap_items.html` & `uncms-0.0.8/src/uncms/templates/admin/dashboard_modules/sitemap_items.html`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/templates/pagination/pagination.html` & `uncms-0.0.8/src/uncms/templates/pagination/pagination.html`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/templatetags/_common.py` & `uncms-0.0.8/src/uncms/templatetags/_common.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/templatetags/uncms_pagination.py` & `uncms-0.0.8/src/uncms/templatetags/uncms_pagination.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/utils.py` & `uncms-0.0.8/src/uncms/utils.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms/views.py` & `uncms-0.0.8/src/uncms/views.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/src/uncms.egg-info/PKG-INFO` & `uncms-0.0.8/src/uncms.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: uncms
-Version: 0.0.7
+Version: 0.0.8
 Summary: A CMS toolkit for Django emphasising simplicity, speed, and familiarity.
 Author-email: Lewis Collard <lewiscollard@gmail.com>
 Project-URL: homepage, https://uncms.dev/
 Project-URL: documentation, https://docs.uncms.dev/
 Project-URL: repository, https://github.com/uncms-dev/uncms
 Classifier: Development Status :: 3 - Alpha
-Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: jinja2
+Provides-Extra: testhelpers
 License-File: LICENSE
 
 # UnCMS: a developer's CMS toolkit for Django
 
 **Warning: UnCMS is in alpha. It is recommended only for the curious and fearless. Do not use it in production.**
 
 UnCMS is a developer's CMS toolkit for Django emphasising simplicity, speed, and familiarity.
```

### Comparing `uncms-0.0.7/src/uncms.egg-info/SOURCES.txt` & `uncms-0.0.8/src/uncms.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -206,14 +206,25 @@
 src/uncms/templates/admin/dashboard_modules/sitemap.html
 src/uncms/templates/admin/dashboard_modules/sitemap_items.html
 src/uncms/templates/pagination/pagination.html
 src/uncms/templatetags/__init__.py
 src/uncms/templatetags/_common.py
 src/uncms/templatetags/uncms_html.py
 src/uncms/templatetags/uncms_pagination.py
+src/uncms/testhelpers/__init__.py
+src/uncms/testhelpers/models.py
+src/uncms/testhelpers/factories/__init__.py
+src/uncms/testhelpers/factories/media.py
+src/uncms/testhelpers/factories/pages.py
+src/uncms/testhelpers/factories/data/1920x1080.jpg
+src/uncms/testhelpers/factories/data/1920x1080.png
+src/uncms/testhelpers/factories/data/1920x1080.webp
+src/uncms/testhelpers/factories/data/800x600.png
+src/uncms/testhelpers/migrations/0001_initial.py
+src/uncms/testhelpers/migrations/__init__.py
 tests/test_admin.py
 tests/test_checks.py
 tests/test_conf.py
 tests/test_forms.py
 tests/test_html.py
 tests/test_jinja2_environment.py
 tests/test_middleware.py
```

### Comparing `uncms-0.0.7/tests/test_admin.py` & `uncms-0.0.8/tests/test_admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pytest
 from django.contrib.admin.sites import AdminSite
 from django.test import RequestFactory
 
-from tests.media.factories import MinimalGIFFileFactory
 from tests.testing_app.admin import RealPageBaseAdmin
 from tests.testing_app.models import OnlineBaseModel, PageBaseModel
 from uncms.admin import OnlineBaseAdmin, SEOQualityControlFilter
+from uncms.testhelpers.factories.media import MinimalGIFFileFactory
 
 
 @pytest.mark.django_db
 def test_onlinebaseadmin_publish_selected():
     page_admin = OnlineBaseAdmin(OnlineBaseModel, AdminSite())
 
     obj = OnlineBaseModel.objects.create(
```

### Comparing `uncms-0.0.7/tests/test_checks.py` & `uncms-0.0.8/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/tests/test_conf.py` & `uncms-0.0.8/tests/test_conf.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/tests/test_forms.py` & `uncms-0.0.8/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/tests/test_html.py` & `uncms-0.0.8/tests/test_html.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pytest
 from bs4 import BeautifulSoup
 from django.contrib.contenttypes.models import ContentType
 from django.test import override_settings
 
-from tests.media.factories import SamplePNGFileFactory
 from uncms.html import clean_all, clean_html, format_html
 from uncms.media.models import File
+from uncms.testhelpers.factories.media import SamplePNGFileFactory
 
 
 @pytest.mark.django_db
 def test_format_html():
     image = SamplePNGFileFactory()
     image_with_alt = SamplePNGFileFactory(alt_text='Alt text &')
```

### Comparing `uncms-0.0.7/tests/test_middleware.py` & `uncms-0.0.8/tests/test_middleware.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import pytest
 from django.contrib.auth.models import AnonymousUser
 from django.template.response import SimpleTemplateResponse
 from django.test import RequestFactory
 from django.test.utils import override_settings
 
-from tests.factories import UserFactory
-from tests.pages.factories import PageFactory
 from uncms.middleware import PublicationMiddleware
+from uncms.testhelpers.factories import UserFactory
+from uncms.testhelpers.factories.pages import PageFactory
 
 
 def test_publicationmiddleware_process_request():
     request = RequestFactory().get('/?preview=a')
     request.user = AnonymousUser()
     publication_middleware = PublicationMiddleware(lambda: None)
     publication_middleware.process_request(request)
```

### Comparing `uncms-0.0.7/tests/test_models.py` & `uncms-0.0.8/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/tests/test_models_base.py` & `uncms-0.0.8/tests/test_models_base.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/tests/test_models_fields.py` & `uncms-0.0.8/tests/test_models_fields.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/tests/test_robots.py` & `uncms-0.0.8/tests/test_robots.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/tests/test_sitemaps.py` & `uncms-0.0.8/tests/test_sitemaps.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/tests/test_templatetags_pagination.py` & `uncms-0.0.8/tests/test_templatetags_pagination.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/tests/test_utils.py` & `uncms-0.0.8/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `uncms-0.0.7/tests/test_views.py` & `uncms-0.0.8/tests/test_views.py`

 * *Files identical despite different names*

