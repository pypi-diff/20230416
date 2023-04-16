# Comparing `tmp/paper-admin-6.0.0rc1.tar.gz` & `tmp/paper-admin-6.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paper-admin-6.0.0rc1.tar", last modified: Sun Apr 16 17:43:52 2023, max compression
+gzip compressed data, was "paper-admin-6.0.0rc2.tar", last modified: Sun Apr 16 18:17:11 2023, max compression
```

## Comparing `paper-admin-6.0.0rc1.tar` & `paper-admin-6.0.0rc2.tar`

### file list

```diff
@@ -1,310 +1,310 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:52.342761 paper-admin-6.0.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)     9827 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    19928 2023-04-16 17:43:52.342761 paper-admin-6.0.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18590 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:52.310761 paper-admin-6.0.0rc1/paper_admin/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:52.310761 paper-admin-6.0.0rc1/paper_admin/admin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14140 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/admin/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/admin/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/admin/renderers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/admin/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/admin/widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:52.302760 paper-admin-6.0.0rc1/paper_admin/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:52.302760 paper-admin-6.0.0rc1/paper_admin/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:52.310761 paper-admin-6.0.0rc1/paper_admin/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/locale/ru/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/locale/ru/LC_MESSAGES/djangojs.po
--rw-r--r--   0 runner    (1001) docker     (123)    18123 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/menu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/monkey_patch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:52.310761 paper-admin-6.0.0rc1/paper_admin/patches/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/patches/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:52.310761 paper-admin-6.0.0rc1/paper_admin/patches/dal/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/patches/dal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/patches/dal/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:52.302760 paper-admin-6.0.0rc1/paper_admin/patches/dal/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:52.310761 paper-admin-6.0.0rc1/paper_admin/patches/dal/static/autocomplete_light/
--rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/patches/dal/static/autocomplete_light/select2.js
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/patches/dal/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:52.310761 paper-admin-6.0.0rc1/paper_admin/patches/django/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/patches/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/patches/django/changelist.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/patches/django/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/patches/django/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/patches/django/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/patches/django/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:52.310761 paper-admin-6.0.0rc1/paper_admin/patches/django/prepopulate/
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/patches/django/prepopulate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/patches/django/prepopulate/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:52.314761 paper-admin-6.0.0rc1/paper_admin/patches/django/renderer/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/patches/django/renderer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/patches/django/renderer/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/patches/django/renderer/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/patches/django/renderer/widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/patches/django/sites.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:52.314761 paper-admin-6.0.0rc1/paper_admin/patches/django/sortable/
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/patches/django/sortable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/patches/django/sortable/changelist.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/patches/django/sortable/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/patches/django/sortable/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:52.314761 paper-admin-6.0.0rc1/paper_admin/patches/django/styles/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/patches/django/styles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/patches/django/styles/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:52.314761 paper-admin-6.0.0rc1/paper_admin/patches/django/tabs/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/patches/django/tabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/patches/django/tabs/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/patches/django/tabs/options.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/patches/django/tabs/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:52.314761 paper-admin-6.0.0rc1/paper_admin/patches/django/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/patches/django/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/patches/django/widgets/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/patches/django/widgets/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:52.314761 paper-admin-6.0.0rc1/paper_admin/patches/django_solo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/patches/django_solo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:52.306760 paper-admin-6.0.0rc1/paper_admin/patches/django_solo/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:52.306760 paper-admin-6.0.0rc1/paper_admin/patches/django_solo/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:52.314761 paper-admin-6.0.0rc1/paper_admin/patches/django_solo/templates/admin/solo/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/patches/django_solo/templates/admin/solo/change_form.html
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/patches/django_solo/templates/admin/solo/object_history.html
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/patches/formfield_defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:52.314761 paper-admin-6.0.0rc1/paper_admin/patches/logentry_admin/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/patches/logentry_admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/patches/logentry_admin/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/patches/logentry_admin/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:52.306760 paper-admin-6.0.0rc1/paper_admin/patches/logentry_admin/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:52.306760 paper-admin-6.0.0rc1/paper_admin/patches/logentry_admin/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:52.306760 paper-admin-6.0.0rc1/paper_admin/patches/logentry_admin/templates/admin/admin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:52.314761 paper-admin-6.0.0rc1/paper_admin/patches/logentry_admin/templates/admin/admin/logentry/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/patches/logentry_admin/templates/admin/admin/logentry/change_form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:52.314761 paper-admin-6.0.0rc1/paper_admin/patches/mptt/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/patches/mptt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/patches/mptt/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/patches/mptt/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:52.306760 paper-admin-6.0.0rc1/paper_admin/patches/mptt/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:52.314761 paper-admin-6.0.0rc1/paper_admin/patches/mptt/templates/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/patches/mptt/templates/admin/mptt_change_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/patches/mptt/templates/admin/mptt_change_list_results.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:52.314761 paper-admin-6.0.0rc1/paper_admin/patches/mptt/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/patches/mptt/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/patches/mptt/templatetags/paper_mptt_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:52.314761 paper-admin-6.0.0rc1/paper_admin/patches/post_office/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/patches/post_office/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/patches/post_office/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/patches/post_office/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:52.314761 paper-admin-6.0.0rc1/paper_admin/patches/tree_queries/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/patches/tree_queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/patches/tree_queries/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/patches/tree_queries/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/patches/tree_queries/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:52.306760 paper-admin-6.0.0rc1/paper_admin/patches/tree_queries/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:52.318760 paper-admin-6.0.0rc1/paper_admin/patches/tree_queries/templates/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/patches/tree_queries/templates/admin/tree_queries_change_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/patches/tree_queries/templates/admin/tree_queries_change_list_results.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:52.318760 paper-admin-6.0.0rc1/paper_admin/patches/tree_queries/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/patches/tree_queries/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/patches/tree_queries/templatetags/paper_tree_queries_list.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:52.306760 paper-admin-6.0.0rc1/paper_admin/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:52.306760 paper-admin-6.0.0rc1/paper_admin/static/admin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:52.318760 paper-admin-6.0.0rc1/paper_admin/static/admin/img/
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/static/admin/img/icon-no.svg
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/static/admin/img/icon-yes.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:52.306760 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:52.326761 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/
--rw-r--r--   0 runner    (1001) docker     (123)   104606 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/app.414cc3e6d494e1a0d3f3.js
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/app.414cc3e6d494e1a0d3f3.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)   423364 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/app.414cc3e6d494e1a0d3f3.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    81823 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/app.styles.da7fec8fb0b40ec91140.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:52.330761 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   139232 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/assets/Roboto.woff
--rw-r--r--   0 runner    (1001) docker     (123)    85728 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/assets/Roboto.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   141648 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/assets/RobotoBold.woff
--rw-r--r--   0 runner    (1001) docker     (123)    87220 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/assets/RobotoBold.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   161688 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/assets/RobotoBoldItalic.woff
--rw-r--r--   0 runner    (1001) docker     (123)   100928 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/assets/RobotoBoldItalic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   161288 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/assets/RobotoItalic.woff
--rw-r--r--   0 runner    (1001) docker     (123)   100120 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/assets/RobotoItalic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   137580 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/assets/RobotoLight.woff
--rw-r--r--   0 runner    (1001) docker     (123)    84520 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/assets/RobotoLight.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   165600 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/assets/RobotoLightItalic.woff
--rw-r--r--   0 runner    (1001) docker     (123)   101884 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/assets/RobotoLightItalic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   141032 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/assets/RobotoMedium.woff
--rw-r--r--   0 runner    (1001) docker     (123)    87464 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/assets/RobotoMedium.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   102368 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/assets/RobotoMediumItalic.woff
--rw-r--r--   0 runner    (1001) docker     (123)    75068 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/assets/RobotoMediumItalic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   164360 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/assets/bootstrap-icons.woff
--rw-r--r--   0 runner    (1001) docker     (123)   121340 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/assets/bootstrap-icons.woff2
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/assets/cross.svg
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/assets/default_favicon.png
--rw-r--r--   0 runner    (1001) docker     (123)   125964 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/assets/login_bg.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    47315 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/assets/menu_bg.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/assets/sortable.svg
--rw-r--r--   0 runner    (1001) docker     (123)    14958 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/changeform.e4e3561b61eb70807245.js
--rw-r--r--   0 runner    (1001) docker     (123)    72700 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/changeform.e4e3561b61eb70807245.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     9752 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/changelist.43ca4ce1d79e97204dbf.js
--rw-r--r--   0 runner    (1001) docker     (123)    42199 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/changelist.43ca4ce1d79e97204dbf.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-16 17:43:25.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/critical.11e9b5fdb3be652e8277.js
--rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-04-16 17:43:25.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/critical.11e9b5fdb3be652e8277.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    17816 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/npm.animejs.0610cb68d4b2f57e8eb8.js
--rw-r--r--   0 runner    (1001) docker     (123)    76238 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/npm.animejs.0610cb68d4b2f57e8eb8.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    73515 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/npm.bootstrap.59081124c9ac6decacff.js
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/npm.bootstrap.59081124c9ac6decacff.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)   259900 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/npm.bootstrap.59081124c9ac6decacff.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/npm.clockpicker.ac0071909818cc80b526.js
--rw-r--r--   0 runner    (1001) docker     (123)    37342 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/npm.clockpicker.ac0071909818cc80b526.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    40658 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/npm.core-js-pure.1bc2fd98475787ba1164.js
--rw-r--r--   0 runner    (1001) docker     (123)   214496 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/npm.core-js-pure.1bc2fd98475787ba1164.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    14600 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/npm.es-abstract.6d963e08114704c8e4d0.js
--rw-r--r--   0 runner    (1001) docker     (123)    56652 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/npm.es-abstract.6d963e08114704c8e4d0.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    96852 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/npm.flatpickr.365327b4124495649c9b.js
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/npm.flatpickr.365327b4124495649c9b.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)   324190 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/npm.flatpickr.365327b4124495649c9b.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    90183 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/npm.jquery.00f10cc5d0570a88ed04.js
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/npm.jquery.00f10cc5d0570a88ed04.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)   472782 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/npm.jquery.00f10cc5d0570a88ed04.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    21003 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/npm.popper.js.fa6168d95a0931432fac.js
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/npm.popper.js.fa6168d95a0931432fac.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)   124107 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/npm.popper.js.fa6168d95a0931432fac.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    77612 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/npm.select2.62432bf0675ff2408a99.js
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/npm.select2.62432bf0675ff2408a99.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)   267313 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/npm.select2.62432bf0675ff2408a99.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    35738 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/npm.sortablejs.73e6a37ecdb386aaa55f.js
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/npm.sortablejs.73e6a37ecdb386aaa55f.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)   175915 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/npm.sortablejs.73e6a37ecdb386aaa55f.js.map
--rw-r--r--   0 runner    (1001) docker     (123)   114414 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/npm.xregexp.98d0b833497d9fd631e9.js
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/npm.xregexp.98d0b833497d9fd631e9.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)   311042 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/npm.xregexp.98d0b833497d9fd631e9.js.map
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/popup.64e2e99cf69da31de176.js
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/popup.64e2e99cf69da31de176.js.map
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/runtime.ed9326a7fe0d75a9fc4a.js
--rw-r--r--   0 runner    (1001) docker     (123)    18354 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/runtime.ed9326a7fe0d75a9fc4a.js.map
--rw-r--r--   0 runner    (1001) docker     (123)    76213 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/vendors.bootstrap-icons.90724fbd0d69e806d41c.css
--rw-r--r--   0 runner    (1001) docker     (123)   149491 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/vendors.bootstrap.826aff9f09cf99cf7eb4.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:52.306760 paper-admin-6.0.0rc1/paper_admin/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:52.334761 paper-admin-6.0.0rc1/paper_admin/templates/admin/
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/admin/actions.html
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/admin/app_index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:52.306760 paper-admin-6.0.0rc1/paper_admin/templates/admin/auth/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:52.334761 paper-admin-6.0.0rc1/paper_admin/templates/admin/auth/user/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/admin/auth/user/add_form.html
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/admin/auth/user/change_password.html
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/admin/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     8367 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/admin/base_site.html
--rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/admin/change_form.html
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/admin/change_form_object_tools.html
--rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/admin/change_list.html
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/admin/change_list_object_tools.html
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/admin/change_list_results.html
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/admin/date_hierarchy.html
--rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/admin/delete_confirmation.html
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/admin/delete_selected_confirmation.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:52.334761 paper-admin-6.0.0rc1/paper_admin/templates/admin/edit_inline/
--rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/admin/edit_inline/_stacked_form.html
--rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/admin/edit_inline/_tabular_form.html
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/admin/edit_inline/stacked.html
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/admin/edit_inline/tabular.html
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/admin/filter.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:52.334761 paper-admin-6.0.0rc1/paper_admin/templates/admin/includes/
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/admin/includes/fieldset.html
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/admin/includes/object_delete_summary.html
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/admin/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/admin/invalid_setup.html
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/admin/login.html
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/admin/object_history.html
--rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/admin/pagination.html
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/admin/popup_response.html
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/admin/prepopulated_fields_js.html
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/admin/search_form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:52.334761 paper-admin-6.0.0rc1/paper_admin/templates/admin/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/admin/widgets/related_widget_wrapper.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:52.306760 paper-admin-6.0.0rc1/paper_admin/templates/auth/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:52.334761 paper-admin-6.0.0rc1/paper_admin/templates/auth/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/auth/widgets/read_only_password_hash.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:52.306760 paper-admin-6.0.0rc1/paper_admin/templates/django/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:52.306760 paper-admin-6.0.0rc1/paper_admin/templates/django/forms/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:52.338761 paper-admin-6.0.0rc1/paper_admin/templates/django/forms/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/django/forms/widgets/checkbox_custom.html
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/django/forms/widgets/clearable_file_input.html
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/django/forms/widgets/date.html
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/django/forms/widgets/datetime.html
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/django/forms/widgets/email.html
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/django/forms/widgets/file.html
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/django/forms/widgets/foreign_key_raw_id.html
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/django/forms/widgets/ip.html
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/django/forms/widgets/many_to_many_raw_id.html
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/django/forms/widgets/multiple_hidden.html
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/django/forms/widgets/multiple_input.html
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/django/forms/widgets/multiwidget.html
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/django/forms/widgets/number.html
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/django/forms/widgets/password.html
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/django/forms/widgets/radio_custom.html
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/django/forms/widgets/radio_option_custom.html
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/django/forms/widgets/select.html
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/django/forms/widgets/select_date.html
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/django/forms/widgets/select_multiple.html
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/django/forms/widgets/splitdatetime.html
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/django/forms/widgets/splithiddendatetime.html
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/django/forms/widgets/switch.html
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/django/forms/widgets/textarea.html
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/django/forms/widgets/time.html
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/django/forms/widgets/url.html
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/django/forms/widgets/uuid.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:52.338761 paper-admin-6.0.0rc1/paper_admin/templates/paper_admin/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-16 17:43:25.000000 paper-admin-6.0.0rc1/paper_admin/templates/paper_admin/app.critical.html
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-16 17:43:51.000000 paper-admin-6.0.0rc1/paper_admin/templates/paper_admin/app.head.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:52.342761 paper-admin-6.0.0rc1/paper_admin/templates/paper_admin/filters/
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/paper_admin/filters/checkbox.html
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/paper_admin/filters/daterange.html
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/paper_admin/filters/hierarchy.html
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/paper_admin/filters/list.html
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/paper_admin/filters/radio.html
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/paper_admin/filters/select.html
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/paper_admin/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/paper_admin/header_buttons.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:52.342761 paper-admin-6.0.0rc1/paper_admin/templates/paper_admin/includes/
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/paper_admin/includes/admin_checkbox.html
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/paper_admin/includes/admin_field.html
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/paper_admin/includes/changelist_field.html
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/paper_admin/includes/changelist_tools.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:52.342761 paper-admin-6.0.0rc1/paper_admin/templates/paper_admin/menu/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/paper_admin/menu/divider.html
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/paper_admin/menu/group.html
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/paper_admin/menu/item.html
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/paper_admin/menu/submenu.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:52.342761 paper-admin-6.0.0rc1/paper_admin/templates/registration/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/registration/logged_out.html
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/registration/password_change_done.html
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/registration/password_change_form.html
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/registration/password_reset_complete.html
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/registration/password_reset_confirm.html
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/registration/password_reset_done.html
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/registration/password_reset_email.html
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/registration/password_reset_email_alt.html
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templates/registration/password_reset_form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:52.342761 paper-admin-6.0.0rc1/paper_admin/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templatetags/load_paper.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templatetags/paper_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templatetags/paper_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templatetags/paper_menu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templatetags/paper_modify.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templatetags/paper_paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/paper_admin/templatetags/paper_styles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 17:43:52.310761 paper-admin-6.0.0rc1/paper_admin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19928 2023-04-16 17:43:52.000000 paper-admin-6.0.0rc1/paper_admin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-04-16 17:43:52.000000 paper-admin-6.0.0rc1/paper_admin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 17:43:52.000000 paper-admin-6.0.0rc1/paper_admin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 17:43:52.000000 paper-admin-6.0.0rc1/paper_admin.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-16 17:43:52.000000 paper-admin-6.0.0rc1/paper_admin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-16 17:43:52.000000 paper-admin-6.0.0rc1/paper_admin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-04-16 17:43:52.346761 paper-admin-6.0.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-16 17:42:57.000000 paper-admin-6.0.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:17:11.781740 paper-admin-6.0.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)     9827 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    19928 2023-04-16 18:17:11.781740 paper-admin-6.0.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18590 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:17:11.749740 paper-admin-6.0.0rc2/paper_admin/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:17:11.749740 paper-admin-6.0.0rc2/paper_admin/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14140 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/admin/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/admin/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/admin/renderers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/admin/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/admin/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:17:11.745740 paper-admin-6.0.0rc2/paper_admin/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:17:11.745740 paper-admin-6.0.0rc2/paper_admin/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:17:11.753740 paper-admin-6.0.0rc2/paper_admin/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/locale/ru/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/locale/ru/LC_MESSAGES/djangojs.po
+-rw-r--r--   0 runner    (1001) docker     (123)    18209 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/monkey_patch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:17:11.753740 paper-admin-6.0.0rc2/paper_admin/patches/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/patches/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:17:11.753740 paper-admin-6.0.0rc2/paper_admin/patches/dal/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/patches/dal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/patches/dal/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:17:11.745740 paper-admin-6.0.0rc2/paper_admin/patches/dal/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:17:11.753740 paper-admin-6.0.0rc2/paper_admin/patches/dal/static/autocomplete_light/
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/patches/dal/static/autocomplete_light/select2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/patches/dal/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:17:11.753740 paper-admin-6.0.0rc2/paper_admin/patches/django/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/patches/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/patches/django/changelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/patches/django/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/patches/django/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/patches/django/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/patches/django/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:17:11.753740 paper-admin-6.0.0rc2/paper_admin/patches/django/prepopulate/
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/patches/django/prepopulate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/patches/django/prepopulate/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:17:11.753740 paper-admin-6.0.0rc2/paper_admin/patches/django/renderer/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/patches/django/renderer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/patches/django/renderer/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/patches/django/renderer/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/patches/django/renderer/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/patches/django/sites.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:17:11.753740 paper-admin-6.0.0rc2/paper_admin/patches/django/sortable/
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/patches/django/sortable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/patches/django/sortable/changelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/patches/django/sortable/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/patches/django/sortable/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:17:11.753740 paper-admin-6.0.0rc2/paper_admin/patches/django/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/patches/django/styles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/patches/django/styles/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:17:11.753740 paper-admin-6.0.0rc2/paper_admin/patches/django/tabs/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/patches/django/tabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/patches/django/tabs/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/patches/django/tabs/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/patches/django/tabs/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:17:11.753740 paper-admin-6.0.0rc2/paper_admin/patches/django/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/patches/django/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/patches/django/widgets/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/patches/django/widgets/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:17:11.753740 paper-admin-6.0.0rc2/paper_admin/patches/django_solo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/patches/django_solo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:17:11.745740 paper-admin-6.0.0rc2/paper_admin/patches/django_solo/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:17:11.745740 paper-admin-6.0.0rc2/paper_admin/patches/django_solo/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:17:11.753740 paper-admin-6.0.0rc2/paper_admin/patches/django_solo/templates/admin/solo/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/patches/django_solo/templates/admin/solo/change_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/patches/django_solo/templates/admin/solo/object_history.html
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/patches/formfield_defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:17:11.753740 paper-admin-6.0.0rc2/paper_admin/patches/logentry_admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/patches/logentry_admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/patches/logentry_admin/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/patches/logentry_admin/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:17:11.745740 paper-admin-6.0.0rc2/paper_admin/patches/logentry_admin/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:17:11.745740 paper-admin-6.0.0rc2/paper_admin/patches/logentry_admin/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:17:11.745740 paper-admin-6.0.0rc2/paper_admin/patches/logentry_admin/templates/admin/admin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:17:11.753740 paper-admin-6.0.0rc2/paper_admin/patches/logentry_admin/templates/admin/admin/logentry/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/patches/logentry_admin/templates/admin/admin/logentry/change_form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:17:11.757740 paper-admin-6.0.0rc2/paper_admin/patches/mptt/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/patches/mptt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/patches/mptt/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/patches/mptt/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:17:11.745740 paper-admin-6.0.0rc2/paper_admin/patches/mptt/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:17:11.757740 paper-admin-6.0.0rc2/paper_admin/patches/mptt/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/patches/mptt/templates/admin/mptt_change_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/patches/mptt/templates/admin/mptt_change_list_results.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:17:11.757740 paper-admin-6.0.0rc2/paper_admin/patches/mptt/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/patches/mptt/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/patches/mptt/templatetags/paper_mptt_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:17:11.757740 paper-admin-6.0.0rc2/paper_admin/patches/post_office/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/patches/post_office/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/patches/post_office/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/patches/post_office/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:17:11.757740 paper-admin-6.0.0rc2/paper_admin/patches/tree_queries/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/patches/tree_queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/patches/tree_queries/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/patches/tree_queries/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/patches/tree_queries/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:17:11.745740 paper-admin-6.0.0rc2/paper_admin/patches/tree_queries/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:17:11.757740 paper-admin-6.0.0rc2/paper_admin/patches/tree_queries/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/patches/tree_queries/templates/admin/tree_queries_change_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/patches/tree_queries/templates/admin/tree_queries_change_list_results.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:17:11.757740 paper-admin-6.0.0rc2/paper_admin/patches/tree_queries/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/patches/tree_queries/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/patches/tree_queries/templatetags/paper_tree_queries_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:17:11.745740 paper-admin-6.0.0rc2/paper_admin/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:17:11.745740 paper-admin-6.0.0rc2/paper_admin/static/admin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:17:11.757740 paper-admin-6.0.0rc2/paper_admin/static/admin/img/
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/static/admin/img/icon-no.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/static/admin/img/icon-yes.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:17:11.745740 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:17:11.769740 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)   104606 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/app.414cc3e6d494e1a0d3f3.js
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/app.414cc3e6d494e1a0d3f3.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   423364 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/app.414cc3e6d494e1a0d3f3.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    81823 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/app.styles.da7fec8fb0b40ec91140.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:17:11.773740 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   139232 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/assets/Roboto.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    85728 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/assets/Roboto.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   141648 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/assets/RobotoBold.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    87220 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/assets/RobotoBold.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   161688 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/assets/RobotoBoldItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   100928 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/assets/RobotoBoldItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   161288 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/assets/RobotoItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   100120 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/assets/RobotoItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   137580 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/assets/RobotoLight.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    84520 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/assets/RobotoLight.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   165600 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/assets/RobotoLightItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   101884 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/assets/RobotoLightItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   141032 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/assets/RobotoMedium.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    87464 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/assets/RobotoMedium.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   102368 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/assets/RobotoMediumItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    75068 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/assets/RobotoMediumItalic.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   164360 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/assets/bootstrap-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   121340 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/assets/bootstrap-icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/assets/cross.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/assets/default_favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)   125964 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/assets/login_bg.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    47315 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/assets/menu_bg.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/assets/sortable.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    14958 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/changeform.e4e3561b61eb70807245.js
+-rw-r--r--   0 runner    (1001) docker     (123)    72700 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/changeform.e4e3561b61eb70807245.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     9752 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/changelist.43ca4ce1d79e97204dbf.js
+-rw-r--r--   0 runner    (1001) docker     (123)    42199 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/changelist.43ca4ce1d79e97204dbf.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-16 18:16:47.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/critical.11e9b5fdb3be652e8277.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3915 2023-04-16 18:16:47.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/critical.11e9b5fdb3be652e8277.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    17816 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/npm.animejs.0610cb68d4b2f57e8eb8.js
+-rw-r--r--   0 runner    (1001) docker     (123)    76238 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/npm.animejs.0610cb68d4b2f57e8eb8.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    73515 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/npm.bootstrap.59081124c9ac6decacff.js
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/npm.bootstrap.59081124c9ac6decacff.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   259900 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/npm.bootstrap.59081124c9ac6decacff.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/npm.clockpicker.ac0071909818cc80b526.js
+-rw-r--r--   0 runner    (1001) docker     (123)    37342 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/npm.clockpicker.ac0071909818cc80b526.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    40658 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/npm.core-js-pure.1bc2fd98475787ba1164.js
+-rw-r--r--   0 runner    (1001) docker     (123)   214496 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/npm.core-js-pure.1bc2fd98475787ba1164.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    14600 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/npm.es-abstract.6d963e08114704c8e4d0.js
+-rw-r--r--   0 runner    (1001) docker     (123)    56652 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/npm.es-abstract.6d963e08114704c8e4d0.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    96852 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/npm.flatpickr.365327b4124495649c9b.js
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/npm.flatpickr.365327b4124495649c9b.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   324190 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/npm.flatpickr.365327b4124495649c9b.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    90183 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/npm.jquery.00f10cc5d0570a88ed04.js
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/npm.jquery.00f10cc5d0570a88ed04.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   472782 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/npm.jquery.00f10cc5d0570a88ed04.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    21003 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/npm.popper.js.fa6168d95a0931432fac.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/npm.popper.js.fa6168d95a0931432fac.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   124107 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/npm.popper.js.fa6168d95a0931432fac.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    77612 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/npm.select2.62432bf0675ff2408a99.js
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/npm.select2.62432bf0675ff2408a99.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   267313 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/npm.select2.62432bf0675ff2408a99.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    35738 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/npm.sortablejs.73e6a37ecdb386aaa55f.js
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/npm.sortablejs.73e6a37ecdb386aaa55f.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   175915 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/npm.sortablejs.73e6a37ecdb386aaa55f.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)   114414 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/npm.xregexp.98d0b833497d9fd631e9.js
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/npm.xregexp.98d0b833497d9fd631e9.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   311042 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/npm.xregexp.98d0b833497d9fd631e9.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/popup.64e2e99cf69da31de176.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/popup.64e2e99cf69da31de176.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/runtime.ed9326a7fe0d75a9fc4a.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18354 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/runtime.ed9326a7fe0d75a9fc4a.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)    76213 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/vendors.bootstrap-icons.90724fbd0d69e806d41c.css
+-rw-r--r--   0 runner    (1001) docker     (123)   149491 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/vendors.bootstrap.826aff9f09cf99cf7eb4.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:17:11.749740 paper-admin-6.0.0rc2/paper_admin/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:17:11.773740 paper-admin-6.0.0rc2/paper_admin/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/admin/actions.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/admin/app_index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:17:11.745740 paper-admin-6.0.0rc2/paper_admin/templates/admin/auth/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:17:11.773740 paper-admin-6.0.0rc2/paper_admin/templates/admin/auth/user/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/admin/auth/user/add_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/admin/auth/user/change_password.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/admin/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8367 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/admin/base_site.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/admin/change_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/admin/change_form_object_tools.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/admin/change_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/admin/change_list_object_tools.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/admin/change_list_results.html
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/admin/date_hierarchy.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/admin/delete_confirmation.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/admin/delete_selected_confirmation.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:17:11.777740 paper-admin-6.0.0rc2/paper_admin/templates/admin/edit_inline/
+-rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/admin/edit_inline/_stacked_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/admin/edit_inline/_tabular_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/admin/edit_inline/stacked.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/admin/edit_inline/tabular.html
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/admin/filter.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:17:11.777740 paper-admin-6.0.0rc2/paper_admin/templates/admin/includes/
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/admin/includes/fieldset.html
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/admin/includes/object_delete_summary.html
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/admin/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/admin/invalid_setup.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/admin/login.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/admin/object_history.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/admin/pagination.html
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/admin/popup_response.html
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/admin/prepopulated_fields_js.html
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/admin/search_form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:17:11.777740 paper-admin-6.0.0rc2/paper_admin/templates/admin/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/admin/widgets/related_widget_wrapper.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:17:11.745740 paper-admin-6.0.0rc2/paper_admin/templates/auth/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:17:11.777740 paper-admin-6.0.0rc2/paper_admin/templates/auth/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/auth/widgets/read_only_password_hash.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:17:11.749740 paper-admin-6.0.0rc2/paper_admin/templates/django/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:17:11.749740 paper-admin-6.0.0rc2/paper_admin/templates/django/forms/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:17:11.777740 paper-admin-6.0.0rc2/paper_admin/templates/django/forms/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/django/forms/widgets/checkbox_custom.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/django/forms/widgets/clearable_file_input.html
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/django/forms/widgets/date.html
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/django/forms/widgets/datetime.html
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/django/forms/widgets/email.html
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/django/forms/widgets/file.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/django/forms/widgets/foreign_key_raw_id.html
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/django/forms/widgets/ip.html
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/django/forms/widgets/many_to_many_raw_id.html
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/django/forms/widgets/multiple_hidden.html
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/django/forms/widgets/multiple_input.html
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/django/forms/widgets/multiwidget.html
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/django/forms/widgets/number.html
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/django/forms/widgets/password.html
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/django/forms/widgets/radio_custom.html
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/django/forms/widgets/radio_option_custom.html
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/django/forms/widgets/select.html
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/django/forms/widgets/select_date.html
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/django/forms/widgets/select_multiple.html
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/django/forms/widgets/splitdatetime.html
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/django/forms/widgets/splithiddendatetime.html
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/django/forms/widgets/switch.html
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/django/forms/widgets/textarea.html
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/django/forms/widgets/time.html
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/django/forms/widgets/url.html
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/django/forms/widgets/uuid.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:17:11.777740 paper-admin-6.0.0rc2/paper_admin/templates/paper_admin/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-16 18:16:47.000000 paper-admin-6.0.0rc2/paper_admin/templates/paper_admin/app.critical.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-16 18:17:10.000000 paper-admin-6.0.0rc2/paper_admin/templates/paper_admin/app.head.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:17:11.781740 paper-admin-6.0.0rc2/paper_admin/templates/paper_admin/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/paper_admin/filters/checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/paper_admin/filters/daterange.html
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/paper_admin/filters/hierarchy.html
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/paper_admin/filters/list.html
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/paper_admin/filters/radio.html
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/paper_admin/filters/select.html
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/paper_admin/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/paper_admin/header_buttons.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:17:11.781740 paper-admin-6.0.0rc2/paper_admin/templates/paper_admin/includes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/paper_admin/includes/admin_checkbox.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/paper_admin/includes/admin_field.html
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/paper_admin/includes/changelist_field.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/paper_admin/includes/changelist_tools.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:17:11.781740 paper-admin-6.0.0rc2/paper_admin/templates/paper_admin/menu/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/paper_admin/menu/divider.html
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/paper_admin/menu/group.html
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/paper_admin/menu/item.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/paper_admin/menu/submenu.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:17:11.781740 paper-admin-6.0.0rc2/paper_admin/templates/registration/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/registration/logged_out.html
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/registration/password_change_done.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/registration/password_change_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/registration/password_reset_complete.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/registration/password_reset_confirm.html
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/registration/password_reset_done.html
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/registration/password_reset_email.html
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/registration/password_reset_email_alt.html
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templates/registration/password_reset_form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:17:11.781740 paper-admin-6.0.0rc2/paper_admin/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templatetags/load_paper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templatetags/paper_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templatetags/paper_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templatetags/paper_menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templatetags/paper_modify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templatetags/paper_paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/paper_admin/templatetags/paper_styles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 18:17:11.749740 paper-admin-6.0.0rc2/paper_admin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19928 2023-04-16 18:17:11.000000 paper-admin-6.0.0rc2/paper_admin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-04-16 18:17:11.000000 paper-admin-6.0.0rc2/paper_admin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 18:17:11.000000 paper-admin-6.0.0rc2/paper_admin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 18:17:11.000000 paper-admin-6.0.0rc2/paper_admin.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-16 18:17:11.000000 paper-admin-6.0.0rc2/paper_admin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-16 18:17:11.000000 paper-admin-6.0.0rc2/paper_admin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-04-16 18:17:11.785740 paper-admin-6.0.0rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-16 18:16:21.000000 paper-admin-6.0.0rc2/setup.py
```

### Comparing `paper-admin-6.0.0rc1/CHANGELOG.md` & `paper-admin-6.0.0rc2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/CONTRIBUTING.md` & `paper-admin-6.0.0rc2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/LICENSE` & `paper-admin-6.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/PKG-INFO` & `paper-admin-6.0.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-admin
-Version: 6.0.0rc1
+Version: 6.0.0rc2
 Summary: Custom Django admin interface.
 Home-page: https://github.com/dldevinc/paper-admin
 Author: Mihail Mishakin
 Author-email: x896321475@gmail.com
 Maintainer: Mihail Mishakin
 Maintainer-email: x896321475@gmail.com
 License: BSD license
```

### Comparing `paper-admin-6.0.0rc1/README.md` & `paper-admin-6.0.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/package.json` & `paper-admin-6.0.0rc2/package.json`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/admin/filters.py` & `paper-admin-6.0.0rc2/paper_admin/admin/filters.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/admin/renderers.py` & `paper-admin-6.0.0rc2/paper_admin/admin/renderers.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/admin/views.py` & `paper-admin-6.0.0rc2/paper_admin/admin/views.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/admin/widgets.py` & `paper-admin-6.0.0rc2/paper_admin/admin/widgets.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/apps.py` & `paper-admin-6.0.0rc2/paper_admin/apps.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/conf.py` & `paper-admin-6.0.0rc2/paper_admin/conf.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/locale/ru/LC_MESSAGES/django.mo` & `paper-admin-6.0.0rc2/paper_admin/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/locale/ru/LC_MESSAGES/django.po` & `paper-admin-6.0.0rc2/paper_admin/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/locale/ru/LC_MESSAGES/djangojs.mo` & `paper-admin-6.0.0rc2/paper_admin/locale/ru/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/locale/ru/LC_MESSAGES/djangojs.po` & `paper-admin-6.0.0rc2/paper_admin/locale/ru/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/menu.py` & `paper-admin-6.0.0rc2/paper_admin/menu.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,28 +4,32 @@
 from typing import (
     Any,
     Callable,
     Dict,
     Generator,
     Iterable,
     List,
-    Literal,
     Optional,
     Union,
 )
 from urllib import parse
 
 import anytree
 from anytree import NodeMixin, PreOrderIter
 from django.contrib.admin import site
 from django.core.exceptions import ImproperlyConfigured
 from django.core.handlers.wsgi import WSGIRequest
 from django.shortcuts import resolve_url
 from django.template import loader
 
+try:
+    from typing import Literal
+except ImportError:
+    from typing_extensions import Literal
+
 __all__ = ["Menu", "Item", "Group", "Divider"]
 
 PermissionType = Union[str, Callable[[WSGIRequest], bool]]
 
 
 class ExcludeItemError(Exception):
     """
```

### Comparing `paper-admin-6.0.0rc1/paper_admin/monkey_patch.py` & `paper-admin-6.0.0rc2/paper_admin/monkey_patch.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/patches/dal/static/autocomplete_light/select2.js` & `paper-admin-6.0.0rc2/paper_admin/patches/dal/static/autocomplete_light/select2.js`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/patches/dal/widgets.py` & `paper-admin-6.0.0rc2/paper_admin/patches/dal/widgets.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/patches/django/changelist.py` & `paper-admin-6.0.0rc2/paper_admin/patches/django/changelist.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/patches/django/filters.py` & `paper-admin-6.0.0rc2/paper_admin/patches/django/filters.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/patches/django/helpers.py` & `paper-admin-6.0.0rc2/paper_admin/patches/django/helpers.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/patches/django/options.py` & `paper-admin-6.0.0rc2/paper_admin/patches/django/options.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/patches/django/prepopulate/__init__.py` & `paper-admin-6.0.0rc2/paper_admin/patches/django/prepopulate/__init__.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/patches/django/prepopulate/helpers.py` & `paper-admin-6.0.0rc2/paper_admin/patches/django/prepopulate/helpers.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/patches/django/renderer/auth.py` & `paper-admin-6.0.0rc2/paper_admin/patches/django/renderer/auth.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/patches/django/renderer/options.py` & `paper-admin-6.0.0rc2/paper_admin/patches/django/renderer/options.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/patches/django/renderer/widgets.py` & `paper-admin-6.0.0rc2/paper_admin/patches/django/renderer/widgets.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/patches/django/sites.py` & `paper-admin-6.0.0rc2/paper_admin/patches/django/sites.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/patches/django/sortable/__init__.py` & `paper-admin-6.0.0rc2/paper_admin/patches/django/sortable/__init__.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/patches/django/sortable/changelist.py` & `paper-admin-6.0.0rc2/paper_admin/patches/django/sortable/changelist.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/patches/django/sortable/options.py` & `paper-admin-6.0.0rc2/paper_admin/patches/django/sortable/options.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/patches/django/styles/options.py` & `paper-admin-6.0.0rc2/paper_admin/patches/django/styles/options.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/patches/django/tabs/helpers.py` & `paper-admin-6.0.0rc2/paper_admin/patches/django/tabs/helpers.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/patches/django/tabs/options.py` & `paper-admin-6.0.0rc2/paper_admin/patches/django/tabs/options.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/patches/django/widgets/options.py` & `paper-admin-6.0.0rc2/paper_admin/patches/django/widgets/options.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/patches/django/widgets/widgets.py` & `paper-admin-6.0.0rc2/paper_admin/patches/django/widgets/widgets.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/patches/django_solo/templates/admin/solo/change_form.html` & `paper-admin-6.0.0rc2/paper_admin/patches/django_solo/templates/admin/solo/change_form.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/patches/django_solo/templates/admin/solo/object_history.html` & `paper-admin-6.0.0rc2/paper_admin/patches/django_solo/templates/admin/solo/object_history.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/patches/formfield_defaults.py` & `paper-admin-6.0.0rc2/paper_admin/patches/formfield_defaults.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/patches/logentry_admin/admin.py` & `paper-admin-6.0.0rc2/paper_admin/patches/logentry_admin/admin.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/patches/mptt/admin.py` & `paper-admin-6.0.0rc2/paper_admin/patches/mptt/admin.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/patches/mptt/templatetags/paper_mptt_list.py` & `paper-admin-6.0.0rc2/paper_admin/patches/mptt/templatetags/paper_mptt_list.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/patches/post_office/admin.py` & `paper-admin-6.0.0rc2/paper_admin/patches/post_office/admin.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/patches/tree_queries/admin.py` & `paper-admin-6.0.0rc2/paper_admin/patches/tree_queries/admin.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/patches/tree_queries/templatetags/paper_tree_queries_list.py` & `paper-admin-6.0.0rc2/paper_admin/patches/tree_queries/templatetags/paper_tree_queries_list.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/app.414cc3e6d494e1a0d3f3.js` & `paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/app.414cc3e6d494e1a0d3f3.js`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/app.414cc3e6d494e1a0d3f3.js.map` & `paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/app.414cc3e6d494e1a0d3f3.js.map`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/app.styles.da7fec8fb0b40ec91140.css` & `paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/app.styles.da7fec8fb0b40ec91140.css`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/assets/Roboto.woff` & `paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/assets/Roboto.woff`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/assets/Roboto.woff2` & `paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/assets/Roboto.woff2`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/assets/RobotoBold.woff` & `paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/assets/RobotoBold.woff`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/assets/RobotoBold.woff2` & `paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/assets/RobotoBold.woff2`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/assets/RobotoBoldItalic.woff` & `paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/assets/RobotoBoldItalic.woff`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/assets/RobotoBoldItalic.woff2` & `paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/assets/RobotoBoldItalic.woff2`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/assets/RobotoItalic.woff` & `paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/assets/RobotoItalic.woff`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/assets/RobotoItalic.woff2` & `paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/assets/RobotoItalic.woff2`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/assets/RobotoLight.woff` & `paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/assets/RobotoLight.woff`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/assets/RobotoLight.woff2` & `paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/assets/RobotoLight.woff2`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/assets/RobotoLightItalic.woff` & `paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/assets/RobotoLightItalic.woff`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/assets/RobotoLightItalic.woff2` & `paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/assets/RobotoLightItalic.woff2`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/assets/RobotoMedium.woff` & `paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/assets/RobotoMedium.woff`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/assets/RobotoMedium.woff2` & `paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/assets/RobotoMedium.woff2`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/assets/RobotoMediumItalic.woff` & `paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/assets/RobotoMediumItalic.woff`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/assets/RobotoMediumItalic.woff2` & `paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/assets/RobotoMediumItalic.woff2`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/assets/bootstrap-icons.woff` & `paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/assets/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/assets/bootstrap-icons.woff2` & `paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/assets/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/assets/default_favicon.png` & `paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/assets/default_favicon.png`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/assets/login_bg.jpg` & `paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/assets/login_bg.jpg`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/assets/menu_bg.jpg` & `paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/assets/menu_bg.jpg`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/assets/sortable.svg` & `paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/assets/sortable.svg`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/changeform.e4e3561b61eb70807245.js` & `paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/changeform.e4e3561b61eb70807245.js`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/changeform.e4e3561b61eb70807245.js.map` & `paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/changeform.e4e3561b61eb70807245.js.map`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/changelist.43ca4ce1d79e97204dbf.js` & `paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/changelist.43ca4ce1d79e97204dbf.js`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/changelist.43ca4ce1d79e97204dbf.js.map` & `paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/changelist.43ca4ce1d79e97204dbf.js.map`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/critical.11e9b5fdb3be652e8277.js` & `paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/critical.11e9b5fdb3be652e8277.js`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/critical.11e9b5fdb3be652e8277.js.map` & `paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/critical.11e9b5fdb3be652e8277.js.map`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/npm.animejs.0610cb68d4b2f57e8eb8.js` & `paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/npm.animejs.0610cb68d4b2f57e8eb8.js`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/npm.animejs.0610cb68d4b2f57e8eb8.js.map` & `paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/npm.animejs.0610cb68d4b2f57e8eb8.js.map`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/npm.bootstrap.59081124c9ac6decacff.js` & `paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/npm.bootstrap.59081124c9ac6decacff.js`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/npm.bootstrap.59081124c9ac6decacff.js.map` & `paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/npm.bootstrap.59081124c9ac6decacff.js.map`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/npm.clockpicker.ac0071909818cc80b526.js` & `paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/npm.clockpicker.ac0071909818cc80b526.js`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/npm.clockpicker.ac0071909818cc80b526.js.map` & `paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/npm.clockpicker.ac0071909818cc80b526.js.map`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/npm.core-js-pure.1bc2fd98475787ba1164.js` & `paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/npm.core-js-pure.1bc2fd98475787ba1164.js`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/npm.core-js-pure.1bc2fd98475787ba1164.js.map` & `paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/npm.core-js-pure.1bc2fd98475787ba1164.js.map`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/npm.es-abstract.6d963e08114704c8e4d0.js` & `paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/npm.es-abstract.6d963e08114704c8e4d0.js`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/npm.es-abstract.6d963e08114704c8e4d0.js.map` & `paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/npm.es-abstract.6d963e08114704c8e4d0.js.map`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/npm.flatpickr.365327b4124495649c9b.js` & `paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/npm.flatpickr.365327b4124495649c9b.js`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/npm.flatpickr.365327b4124495649c9b.js.LICENSE.txt` & `paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/npm.flatpickr.365327b4124495649c9b.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/npm.flatpickr.365327b4124495649c9b.js.map` & `paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/npm.flatpickr.365327b4124495649c9b.js.map`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/npm.jquery.00f10cc5d0570a88ed04.js` & `paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/npm.jquery.00f10cc5d0570a88ed04.js`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/npm.jquery.00f10cc5d0570a88ed04.js.map` & `paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/npm.jquery.00f10cc5d0570a88ed04.js.map`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/npm.popper.js.fa6168d95a0931432fac.js` & `paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/npm.popper.js.fa6168d95a0931432fac.js`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/npm.popper.js.fa6168d95a0931432fac.js.LICENSE.txt` & `paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/npm.popper.js.fa6168d95a0931432fac.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/npm.popper.js.fa6168d95a0931432fac.js.map` & `paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/npm.popper.js.fa6168d95a0931432fac.js.map`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/npm.select2.62432bf0675ff2408a99.js` & `paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/npm.select2.62432bf0675ff2408a99.js`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/npm.select2.62432bf0675ff2408a99.js.map` & `paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/npm.select2.62432bf0675ff2408a99.js.map`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/npm.sortablejs.73e6a37ecdb386aaa55f.js` & `paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/npm.sortablejs.73e6a37ecdb386aaa55f.js`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/npm.sortablejs.73e6a37ecdb386aaa55f.js.map` & `paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/npm.sortablejs.73e6a37ecdb386aaa55f.js.map`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/npm.xregexp.98d0b833497d9fd631e9.js` & `paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/npm.xregexp.98d0b833497d9fd631e9.js`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/npm.xregexp.98d0b833497d9fd631e9.js.LICENSE.txt` & `paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/npm.xregexp.98d0b833497d9fd631e9.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/npm.xregexp.98d0b833497d9fd631e9.js.map` & `paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/npm.xregexp.98d0b833497d9fd631e9.js.map`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/popup.64e2e99cf69da31de176.js.map` & `paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/popup.64e2e99cf69da31de176.js.map`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/runtime.ed9326a7fe0d75a9fc4a.js` & `paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/runtime.ed9326a7fe0d75a9fc4a.js`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/runtime.ed9326a7fe0d75a9fc4a.js.map` & `paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/runtime.ed9326a7fe0d75a9fc4a.js.map`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/vendors.bootstrap-icons.90724fbd0d69e806d41c.css` & `paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/vendors.bootstrap-icons.90724fbd0d69e806d41c.css`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/static/paper_admin/dist/vendors.bootstrap.826aff9f09cf99cf7eb4.css` & `paper-admin-6.0.0rc2/paper_admin/static/paper_admin/dist/vendors.bootstrap.826aff9f09cf99cf7eb4.css`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/templates/admin/actions.html` & `paper-admin-6.0.0rc2/paper_admin/templates/admin/actions.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/templates/admin/app_index.html` & `paper-admin-6.0.0rc2/paper_admin/templates/admin/app_index.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/templates/admin/auth/user/change_password.html` & `paper-admin-6.0.0rc2/paper_admin/templates/admin/auth/user/change_password.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/templates/admin/base.html` & `paper-admin-6.0.0rc2/paper_admin/templates/admin/base.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/templates/admin/base_site.html` & `paper-admin-6.0.0rc2/paper_admin/templates/admin/base_site.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/templates/admin/change_form.html` & `paper-admin-6.0.0rc2/paper_admin/templates/admin/change_form.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/templates/admin/change_form_object_tools.html` & `paper-admin-6.0.0rc2/paper_admin/templates/admin/change_form_object_tools.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/templates/admin/change_list.html` & `paper-admin-6.0.0rc2/paper_admin/templates/admin/change_list.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/templates/admin/change_list_results.html` & `paper-admin-6.0.0rc2/paper_admin/templates/admin/change_list_results.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/templates/admin/date_hierarchy.html` & `paper-admin-6.0.0rc2/paper_admin/templates/admin/date_hierarchy.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/templates/admin/delete_confirmation.html` & `paper-admin-6.0.0rc2/paper_admin/templates/admin/delete_confirmation.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/templates/admin/delete_selected_confirmation.html` & `paper-admin-6.0.0rc2/paper_admin/templates/admin/delete_selected_confirmation.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/templates/admin/edit_inline/_stacked_form.html` & `paper-admin-6.0.0rc2/paper_admin/templates/admin/edit_inline/_stacked_form.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/templates/admin/edit_inline/_tabular_form.html` & `paper-admin-6.0.0rc2/paper_admin/templates/admin/edit_inline/_tabular_form.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/templates/admin/edit_inline/stacked.html` & `paper-admin-6.0.0rc2/paper_admin/templates/admin/edit_inline/stacked.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/templates/admin/edit_inline/tabular.html` & `paper-admin-6.0.0rc2/paper_admin/templates/admin/edit_inline/tabular.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/templates/admin/filter.html` & `paper-admin-6.0.0rc2/paper_admin/templates/admin/filter.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/templates/admin/includes/fieldset.html` & `paper-admin-6.0.0rc2/paper_admin/templates/admin/includes/fieldset.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/templates/admin/login.html` & `paper-admin-6.0.0rc2/paper_admin/templates/admin/login.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/templates/admin/object_history.html` & `paper-admin-6.0.0rc2/paper_admin/templates/admin/object_history.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/templates/admin/pagination.html` & `paper-admin-6.0.0rc2/paper_admin/templates/admin/pagination.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/templates/admin/popup_response.html` & `paper-admin-6.0.0rc2/paper_admin/templates/admin/popup_response.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/templates/admin/search_form.html` & `paper-admin-6.0.0rc2/paper_admin/templates/admin/search_form.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/templates/admin/widgets/related_widget_wrapper.html` & `paper-admin-6.0.0rc2/paper_admin/templates/admin/widgets/related_widget_wrapper.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/templates/django/forms/widgets/clearable_file_input.html` & `paper-admin-6.0.0rc2/paper_admin/templates/django/forms/widgets/clearable_file_input.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/templates/django/forms/widgets/date.html` & `paper-admin-6.0.0rc2/paper_admin/templates/django/forms/widgets/date.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/templates/django/forms/widgets/email.html` & `paper-admin-6.0.0rc2/paper_admin/templates/django/forms/widgets/email.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/templates/django/forms/widgets/file.html` & `paper-admin-6.0.0rc2/paper_admin/templates/django/forms/widgets/file.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/templates/django/forms/widgets/foreign_key_raw_id.html` & `paper-admin-6.0.0rc2/paper_admin/templates/django/forms/widgets/foreign_key_raw_id.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/templates/django/forms/widgets/password.html` & `paper-admin-6.0.0rc2/paper_admin/templates/django/forms/widgets/password.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/templates/django/forms/widgets/select.html` & `paper-admin-6.0.0rc2/paper_admin/templates/django/forms/widgets/select.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/templates/django/forms/widgets/select_multiple.html` & `paper-admin-6.0.0rc2/paper_admin/templates/django/forms/widgets/select_multiple.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/templates/django/forms/widgets/time.html` & `paper-admin-6.0.0rc2/paper_admin/templates/django/forms/widgets/time.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/templates/django/forms/widgets/url.html` & `paper-admin-6.0.0rc2/paper_admin/templates/django/forms/widgets/url.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/templates/django/forms/widgets/uuid.html` & `paper-admin-6.0.0rc2/paper_admin/templates/django/forms/widgets/uuid.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/templates/paper_admin/app.head.html` & `paper-admin-6.0.0rc2/paper_admin/templates/paper_admin/app.head.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/templates/paper_admin/filters/checkbox.html` & `paper-admin-6.0.0rc2/paper_admin/templates/paper_admin/filters/checkbox.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/templates/paper_admin/filters/daterange.html` & `paper-admin-6.0.0rc2/paper_admin/templates/paper_admin/filters/daterange.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/templates/paper_admin/filters/hierarchy.html` & `paper-admin-6.0.0rc2/paper_admin/templates/paper_admin/filters/hierarchy.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/templates/paper_admin/filters/list.html` & `paper-admin-6.0.0rc2/paper_admin/templates/paper_admin/filters/list.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/templates/paper_admin/filters/radio.html` & `paper-admin-6.0.0rc2/paper_admin/templates/paper_admin/filters/radio.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/templates/paper_admin/footer.html` & `paper-admin-6.0.0rc2/paper_admin/templates/paper_admin/footer.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/templates/paper_admin/header_buttons.html` & `paper-admin-6.0.0rc2/paper_admin/templates/paper_admin/header_buttons.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/templates/paper_admin/includes/admin_checkbox.html` & `paper-admin-6.0.0rc2/paper_admin/templates/paper_admin/includes/admin_checkbox.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/templates/paper_admin/includes/admin_field.html` & `paper-admin-6.0.0rc2/paper_admin/templates/paper_admin/includes/admin_field.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/templates/paper_admin/includes/changelist_tools.html` & `paper-admin-6.0.0rc2/paper_admin/templates/paper_admin/includes/changelist_tools.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/templates/paper_admin/menu/item.html` & `paper-admin-6.0.0rc2/paper_admin/templates/paper_admin/menu/item.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/templates/paper_admin/menu/submenu.html` & `paper-admin-6.0.0rc2/paper_admin/templates/paper_admin/menu/submenu.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/templates/registration/password_change_form.html` & `paper-admin-6.0.0rc2/paper_admin/templates/registration/password_change_form.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/templates/registration/password_reset_confirm.html` & `paper-admin-6.0.0rc2/paper_admin/templates/registration/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/templates/registration/password_reset_done.html` & `paper-admin-6.0.0rc2/paper_admin/templates/registration/password_reset_done.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/templates/registration/password_reset_email.html` & `paper-admin-6.0.0rc2/paper_admin/templates/registration/password_reset_email.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/templates/registration/password_reset_email_alt.html` & `paper-admin-6.0.0rc2/paper_admin/templates/registration/password_reset_email_alt.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/templates/registration/password_reset_form.html` & `paper-admin-6.0.0rc2/paper_admin/templates/registration/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/templatetags/paper_filters.py` & `paper-admin-6.0.0rc2/paper_admin/templatetags/paper_filters.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/templatetags/paper_list.py` & `paper-admin-6.0.0rc2/paper_admin/templatetags/paper_list.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/templatetags/paper_menu.py` & `paper-admin-6.0.0rc2/paper_admin/templatetags/paper_menu.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/templatetags/paper_modify.py` & `paper-admin-6.0.0rc2/paper_admin/templatetags/paper_modify.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/templatetags/paper_paginator.py` & `paper-admin-6.0.0rc2/paper_admin/templatetags/paper_paginator.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin/templatetags/paper_styles.py` & `paper-admin-6.0.0rc2/paper_admin/templatetags/paper_styles.py`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/paper_admin.egg-info/PKG-INFO` & `paper-admin-6.0.0rc2/paper_admin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-admin
-Version: 6.0.0rc1
+Version: 6.0.0rc2
 Summary: Custom Django admin interface.
 Home-page: https://github.com/dldevinc/paper-admin
 Author: Mihail Mishakin
 Author-email: x896321475@gmail.com
 Maintainer: Mihail Mishakin
 Maintainer-email: x896321475@gmail.com
 License: BSD license
```

### Comparing `paper-admin-6.0.0rc1/paper_admin.egg-info/SOURCES.txt` & `paper-admin-6.0.0rc2/paper_admin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `paper-admin-6.0.0rc1/setup.cfg` & `paper-admin-6.0.0rc2/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 zip_safe = false
 python_requires = >= 3.7
 include_package_data = true
 install_requires = 
 	Django>=2.2
 	Pillow
 	anytree
+	typing_extensions
 packages = find_namespace:
 
 [options.packages.find]
 exclude = 
 	tests
 	tests.*
```

