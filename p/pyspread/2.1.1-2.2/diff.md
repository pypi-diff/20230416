# Comparing `tmp/pyspread-2.1.1.tar.gz` & `tmp/pyspread-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyspread-2.1.1.tar", last modified: Sun Nov 13 16:37:14 2022, max compression
+gzip compressed data, was "pyspread-2.2.tar", last modified: Sun Apr 16 18:40:47 2023, max compression
```

## Comparing `pyspread-2.1.1.tar` & `pyspread-2.2.tar`

### file list

```diff
@@ -1,348 +1,366 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-13 16:37:14.851643 pyspread-2.1.1/
--rw-rw-rw-   0 root         (0) root         (0)       87 2022-11-13 16:35:51.000000 pyspread-2.1.1/AUTHORS
--rw-rw-rw-   0 root         (0) root         (0)    35141 2022-11-13 16:35:51.000000 pyspread-2.1.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      307 2022-11-13 16:35:51.000000 pyspread-2.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5062 2022-11-13 16:37:14.851643 pyspread-2.1.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2608 2022-11-13 16:35:51.000000 pyspread-2.1.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      382 2022-11-13 16:35:51.000000 pyspread-2.1.1/THANKS
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-11-13 16:35:51.000000 pyspread-2.1.1/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14090 2022-11-13 16:35:51.000000 pyspread-2.1.1/changelog
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-13 16:37:14.739632 pyspread-2.1.1/pyspread/
--rw-rw-rw-   0 root         (0) root         (0)       93 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      993 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)    45430 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/actions.py
--rw-rw-rw-   0 root         (0) root         (0)     3393 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/cli.py
--rw-rw-rw-   0 root         (0) root         (0)    34733 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/commands.py
--rw-rw-rw-   0 root         (0) root         (0)    56918 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/dialogs.py
--rw-rw-rw-   0 root         (0) root         (0)     5900 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/entryline.py
--rw-rw-rw-   0 root         (0) root         (0)    95105 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/grid.py
--rw-rw-rw-   0 root         (0) root         (0)    28907 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/grid_renderer.py
--rw-rw-rw-   0 root         (0) root         (0)     8693 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/icons.py
--rw-rw-rw-   0 root         (0) root         (0)    10819 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/installer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-13 16:37:14.742632 pyspread-2.1.1/pyspread/interfaces/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/interfaces/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    19438 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/interfaces/pys.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-13 16:37:14.747633 pyspread-2.1.1/pyspread/lib/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/lib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1060 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/lib/attrdict.py
--rw-rw-rw-   0 root         (0) root         (0)     9886 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/lib/charts.py
--rw-rw-rw-   0 root         (0) root         (0)     4889 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/lib/csv.py
--rw-rw-rw-   0 root         (0) root         (0)    45208 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/lib/dataclasses.py
--rw-rw-rw-   0 root         (0) root         (0)     2109 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/lib/exception_handling.py
--rw-rw-rw-   0 root         (0) root         (0)     4077 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/lib/file_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     2522 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/lib/hashing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-13 16:37:14.748633 pyspread-2.1.1/pyspread/lib/packaging/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/lib/packaging/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2022 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/lib/packaging/_structures.py
--rw-rw-rw-   0 root         (0) root         (0)     1437 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/lib/packaging/_typing.py
--rw-rw-rw-   0 root         (0) root         (0)    15480 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/lib/packaging/version.py
--rwxrwxrwx   0 root         (0) root         (0)    10984 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/lib/qimage2ndarray.py
--rw-rw-rw-   0 root         (0) root         (0)     2686 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/lib/qimage_svg.py
--rw-rw-rw-   0 root         (0) root         (0)    21086 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/lib/selection.py
--rw-rw-rw-   0 root         (0) root         (0)    25092 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/lib/spelltextedit.py
--rw-rw-rw-   0 root         (0) root         (0)     2093 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/lib/string_helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-13 16:37:14.755634 pyspread-2.1.1/pyspread/lib/test/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/lib/test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2289 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/lib/test/compat.py
--rw-rw-rw-   0 root         (0) root         (0)       13 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/lib/test/invalid1.csv
--rw-rw-rw-   0 root         (0) root         (0)       13 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/lib/test/invalid2.csv
--rw-rw-rw-   0 root         (0) root         (0)     3569 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/lib/test/test_array2qimage.py
--rw-rw-rw-   0 root         (0) root         (0)     5101 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/lib/test/test_csv.py
--rw-rw-rw-   0 root         (0) root         (0)     1457 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/lib/test/test_file_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     2868 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/lib/test/test_hashing.py
--rw-rw-rw-   0 root         (0) root         (0)     5235 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/lib/test/test_qimageview.py
--rw-rw-rw-   0 root         (0) root         (0)    16899 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/lib/test/test_selection.py
--rw-rw-rw-   0 root         (0) root         (0)     1936 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/lib/test/test_string_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)       18 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/lib/test/valid1.csv
--rw-rw-rw-   0 root         (0) root         (0)       18 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/lib/test/valid2.csv
--rw-rw-rw-   0 root         (0) root         (0)  2287092 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/lib/test/valid3.csv
--rw-rw-rw-   0 root         (0) root         (0)       24 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/lib/test/valid4.csv
--rw-rw-rw-   0 root         (0) root         (0)     2740 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/lib/typechecks.py
--rw-rw-rw-   0 root         (0) root         (0)    27757 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/main_window.py
--rw-rw-rw-   0 root         (0) root         (0)    16608 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/menus.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-13 16:37:14.756634 pyspread-2.1.1/pyspread/model/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/model/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    51496 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/model/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-13 16:37:14.757634 pyspread-2.1.1/pyspread/model/test/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/model/test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    19920 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/model/test/test_model.py
--rw-rw-rw-   0 root         (0) root         (0)     4539 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/panels.py
--rwxrwxrwx   0 root         (0) root         (0)     2503 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/pyspread.py
--rw-rw-rw-   0 root         (0) root         (0)    12092 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-13 16:37:14.757634 pyspread-2.1.1/pyspread/share/
--rw-rw-rw-   0 root         (0) root         (0)    35141 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-13 16:37:14.757634 pyspread-2.1.1/pyspread/share/applications/
--rwxrwxrwx   0 root         (0) root         (0)      761 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/applications/io.gitlab.pyspread.pyspread.desktop
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-13 16:37:14.726631 pyspread-2.1.1/pyspread/share/doc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-13 16:37:14.760634 pyspread-2.1.1/pyspread/share/doc/manual/
--rw-rw-rw-   0 root         (0) root         (0)     3575 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/doc/manual/advanced_topics.md
--rw-rw-rw-   0 root         (0) root         (0)    10408 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/doc/manual/basic_concepts.md
--rw-rw-rw-   0 root         (0) root         (0)     4852 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/doc/manual/edit_menu.md
--rw-rw-rw-   0 root         (0) root         (0)     7506 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/doc/manual/file_menu.md
--rw-rw-rw-   0 root         (0) root         (0)     6821 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/doc/manual/format_menu.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-13 16:37:14.765635 pyspread-2.1.1/pyspread/share/doc/manual/images/
--rw-rw-rw-   0 root         (0) root         (0)    18661 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/doc/manual/images/screenshot_approve_dialog.png
--rw-rw-rw-   0 root         (0) root         (0)   130518 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/doc/manual/images/screenshot_chartdialog.png
--rw-rw-rw-   0 root         (0) root         (0)    24102 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/doc/manual/images/screenshot_csv_export.png
--rw-rw-rw-   0 root         (0) root         (0)    26708 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/doc/manual/images/screenshot_csv_import.png
--rw-rw-rw-   0 root         (0) root         (0)     7186 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/doc/manual/images/screenshot_find_dialog.png
--rw-rw-rw-   0 root         (0) root         (0)     7586 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/doc/manual/images/screenshot_macros.png
--rw-rw-rw-   0 root         (0) root         (0)    91836 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/doc/manual/images/screenshot_main_window.png
--rw-rw-rw-   0 root         (0) root         (0)    11767 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/doc/manual/images/screenshot_new_dialog.png
--rw-rw-rw-   0 root         (0) root         (0)     8572 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/doc/manual/images/screenshot_paste_as.png
--rw-rw-rw-   0 root         (0) root         (0)    19022 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/doc/manual/images/screenshot_preferences_dialog.png
--rw-rw-rw-   0 root         (0) root         (0)    10973 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/doc/manual/images/screenshot_print_preview_1.png
--rw-rw-rw-   0 root         (0) root         (0)    27303 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/doc/manual/images/screenshot_print_preview_2.png
--rw-rw-rw-   0 root         (0) root         (0)    16783 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/doc/manual/images/screenshot_replace_dialog.png
--rw-rw-rw-   0 root         (0) root         (0)     1773 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/doc/manual/macro_menu.md
--rw-rw-rw-   0 root         (0) root         (0)     1289 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/doc/manual/overview.md
--rw-rw-rw-   0 root         (0) root         (0)     2016 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/doc/manual/view_menu.md
--rw-rw-rw-   0 root         (0) root         (0)     5723 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/doc/manual/workspace.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-13 16:37:14.765635 pyspread-2.1.1/pyspread/share/doc/tutorial/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-13 16:37:14.767635 pyspread-2.1.1/pyspread/share/doc/tutorial/images/
--rw-rw-rw-   0 root         (0) root         (0)    61117 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/doc/tutorial/images/Tutorial1.png
--rw-rw-rw-   0 root         (0) root         (0)    45217 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/doc/tutorial/images/Tutorial2.png
--rw-rw-rw-   0 root         (0) root         (0)    54732 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/doc/tutorial/images/Tutorial3.png
--rw-rw-rw-   0 root         (0) root         (0)    64569 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/doc/tutorial/images/Tutorial4.png
--rw-rw-rw-   0 root         (0) root         (0)     4877 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/doc/tutorial/tutorial.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-13 16:37:14.778636 pyspread-2.1.1/pyspread/share/examples/
--rw-rw-rw-   0 root         (0) root         (0)  8812542 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/examples/big.csv
--rw-rw-rw-   0 root         (0) root         (0)      433 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/examples/conditional_formatting.pysu
--rw-rw-rw-   0 root         (0) root         (0)    17191 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/examples/images and charts.pysu
--rw-rw-rw-   0 root         (0) root         (0)     4185 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/examples/pivot.pysu
--rw-rw-rw-   0 root         (0) root         (0)    29100 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/examples/test_write.csv
--rw-rw-rw-   0 root         (0) root         (0)    21717 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/examples/wagner_whitin.pysu
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-13 16:37:14.728631 pyspread-2.1.1/pyspread/share/icons/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-13 16:37:14.816640 pyspread-2.1.1/pyspread/share/icons/actions/
--rw-rw-rw-   0 root         (0) root         (0)   136218 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/document-approve.svg
--rw-rw-rw-   0 root         (0) root         (0)    24975 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/document-export.svg
--rw-rw-rw-   0 root         (0) root         (0)    21023 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/document-import.svg
--rw-rw-rw-   0 root         (0) root         (0)    19127 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/document-log-out.svg
--rw-rw-rw-   0 root         (0) root         (0)   165172 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/document-new-gpg-key.svg
--rw-rw-rw-   0 root         (0) root         (0)    17406 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/document-new.svg
--rw-rw-rw-   0 root         (0) root         (0)    30805 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/document-open.svg
--rw-rw-rw-   0 root         (0) root         (0)    29401 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/document-page-setup.svg
--rw-rw-rw-   0 root         (0) root         (0)    33813 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/document-print-preview.svg
--rw-rw-rw-   0 root         (0) root         (0)    23333 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/document-print.svg
--rw-rw-rw-   0 root         (0) root         (0)    25424 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/document-properties.svg
--rw-rw-rw-   0 root         (0) root         (0)    31913 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/document-save-as.svg
--rw-rw-rw-   0 root         (0) root         (0)    29894 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/document-save.svg
--rw-rw-rw-   0 root         (0) root         (0)    19499 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/edit-clear.svg
--rw-rw-rw-   0 root         (0) root         (0)    16456 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/edit-copy-results.svg
--rw-rw-rw-   0 root         (0) root         (0)    15595 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/edit-copy.svg
--rw-rw-rw-   0 root         (0) root         (0)    23051 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/edit-cut.svg
--rw-rw-rw-   0 root         (0) root         (0)    35153 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/edit-delete-column.svg
--rw-rw-rw-   0 root         (0) root         (0)    24107 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/edit-delete-row.svg
--rw-rw-rw-   0 root         (0) root         (0)    21308 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/edit-delete-table.svg
--rw-rw-rw-   0 root         (0) root         (0)    54926 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/edit-delete.svg
--rw-rw-rw-   0 root         (0) root         (0)     4953 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/edit-find-next.svg
--rw-rw-rw-   0 root         (0) root         (0)    45880 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/edit-find-replace.svg
--rw-rw-rw-   0 root         (0) root         (0)    35412 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/edit-find.svg
--rw-rw-rw-   0 root         (0) root         (0)    14246 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/edit-insert-column.svg
--rw-rw-rw-   0 root         (0) root         (0)    13993 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/edit-insert-row.svg
--rw-rw-rw-   0 root         (0) root         (0)    12163 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/edit-insert-table.svg
--rw-rw-rw-   0 root         (0) root         (0)     8988 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/edit-paste-as.svg
--rw-rw-rw-   0 root         (0) root         (0)    23755 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/edit-paste.svg
--rw-rw-rw-   0 root         (0) root         (0)    37205 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/edit-quote.svg
--rw-rw-rw-   0 root         (0) root         (0)     9331 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/edit-redo.svg
--rw-rw-rw-   0 root         (0) root         (0)     6028 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/edit-resize-grid.svg
--rw-rw-rw-   0 root         (0) root         (0)    15903 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/edit-select-all.svg
--rw-rw-rw-   0 root         (0) root         (0)    17679 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/edit-sort-ascending.svg
--rw-rw-rw-   0 root         (0) root         (0)    18405 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/edit-sort-descending.svg
--rw-rw-rw-   0 root         (0) root         (0)     9235 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/edit-undo.svg
--rw-rw-rw-   0 root         (0) root         (0)    10364 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/format-background-color.svg
--rw-rw-rw-   0 root         (0) root         (0)     1992 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/format-borders-0.svg
--rw-rw-rw-   0 root         (0) root         (0)     2273 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/format-borders-1.svg
--rw-rw-rw-   0 root         (0) root         (0)     2275 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/format-borders-16.svg
--rw-rw-rw-   0 root         (0) root         (0)     2273 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/format-borders-2.svg
--rw-rw-rw-   0 root         (0) root         (0)     2275 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/format-borders-32.svg
--rw-rw-rw-   0 root         (0) root         (0)     2273 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/format-borders-4.svg
--rw-rw-rw-   0 root         (0) root         (0)     2274 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/format-borders-64.svg
--rw-rw-rw-   0 root         (0) root         (0)     2275 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/format-borders-8.svg
--rw-rw-rw-   0 root         (0) root         (0)     3709 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/format-borders-all.svg
--rw-rw-rw-   0 root         (0) root         (0)     3947 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/format-borders-bottom.svg
--rw-rw-rw-   0 root         (0) root         (0)     3906 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/format-borders-inner.svg
--rw-rw-rw-   0 root         (0) root         (0)     4029 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/format-borders-left.svg
--rw-rw-rw-   0 root         (0) root         (0)     3799 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/format-borders-outer.svg
--rw-rw-rw-   0 root         (0) root         (0)     4029 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/format-borders-right.svg
--rw-rw-rw-   0 root         (0) root         (0)     3879 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/format-borders-top-bottom.svg
--rw-rw-rw-   0 root         (0) root         (0)     3883 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/format-borders-top.svg
--rw-rw-rw-   0 root         (0) root         (0)     3801 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/format-button.svg
--rw-rw-rw-   0 root         (0) root         (0)    44063 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/format-cell-chart.svg
--rw-rw-rw-   0 root         (0) root         (0)   718331 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/format-cell-image.svg
--rw-rw-rw-   0 root         (0) root         (0)    41228 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/format-cell-markup.svg
--rw-rw-rw-   0 root         (0) root         (0)    14454 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/format-cell-rotate-0.svg
--rw-rw-rw-   0 root         (0) root         (0)    14581 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/format-cell-rotate-180.svg
--rw-rw-rw-   0 root         (0) root         (0)    14580 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/format-cell-rotate-270.svg
--rw-rw-rw-   0 root         (0) root         (0)    15749 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/format-cell-rotate-90.svg
--rw-rw-rw-   0 root         (0) root         (0)    27835 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/format-cell-text.svg
--rw-rw-rw-   0 root         (0) root         (0)    12343 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/format-copy.svg
--rw-rw-rw-   0 root         (0) root         (0)    12731 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/format-font.svg
--rw-rw-rw-   0 root         (0) root         (0)    18923 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/format-freeze.svg
--rw-rw-rw-   0 root         (0) root         (0)    13344 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/format-justify-center.svg
--rw-rw-rw-   0 root         (0) root         (0)    13332 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/format-justify-fill.svg
--rw-rw-rw-   0 root         (0) root         (0)    11136 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/format-justify-left.svg
--rw-rw-rw-   0 root         (0) root         (0)    13382 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/format-justify-right.svg
--rw-rw-rw-   0 root         (0) root         (0)     7716 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/format-line-color.svg
--rw-rw-rw-   0 root         (0) root         (0)     8658 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/format-line-color2.svg
--rw-rw-rw-   0 root         (0) root         (0)   143193 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/format-lock.svg
--rw-rw-rw-   0 root         (0) root         (0)     2441 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/format-merge-cells.svg
--rw-rw-rw-   0 root         (0) root         (0)    37466 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/format-paste.svg
--rw-rw-rw-   0 root         (0) root         (0)    12457 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/format-text-align-bottom.svg
--rw-rw-rw-   0 root         (0) root         (0)    12574 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/format-text-align-center.svg
--rw-rw-rw-   0 root         (0) root         (0)    12794 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/format-text-align-top.svg
--rw-rw-rw-   0 root         (0) root         (0)    10953 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/format-text-bold.svg
--rw-rw-rw-   0 root         (0) root         (0)     6484 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/format-text-color.svg
--rw-rw-rw-   0 root         (0) root         (0)    11302 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/format-text-italic.svg
--rw-rw-rw-   0 root         (0) root         (0)    14525 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/format-text-strikethrough.svg
--rw-rw-rw-   0 root         (0) root         (0)    14583 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/format-text-underline.svg
--rw-rw-rw-   0 root         (0) root         (0)   121867 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/help-browser.svg
--rw-rw-rw-   0 root         (0) root         (0)   353099 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/help-dependencies.svg
--rw-rw-rw-   0 root         (0) root         (0)     5737 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/help-faq.svg
--rw-rw-rw-   0 root         (0) root         (0)      503 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/help-tutorial.svg
--rw-rw-rw-   0 root         (0) root         (0)    41994 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/macro-insert-chart.svg
--rw-rw-rw-   0 root         (0) root         (0)   396438 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/macro-insert-image.svg
--rw-rw-rw-   0 root         (0) root         (0)    21889 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/macro-insert-sum.svg
--rw-rw-rw-   0 root         (0) root         (0)   388308 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/macro-link-image.svg
--rw-rw-rw-   0 root         (0) root         (0)    10037 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/macro-open.svg
--rw-rw-rw-   0 root         (0) root         (0)    10693 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/macro-save.svg
--rw-rw-rw-   0 root         (0) root         (0)    19612 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/menu-manager.svg
--rw-rw-rw-   0 root         (0) root         (0)    23289 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/view-check-spelling.svg
--rw-rw-rw-   0 root         (0) root         (0)    20295 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/view-fullscreen.svg
--rw-rw-rw-   0 root         (0) root         (0)     3176 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/view-goto-cell.svg
--rw-rw-rw-   0 root         (0) root         (0)    16868 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/view-refresh.svg
--rw-rw-rw-   0 root         (0) root         (0)    20510 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/view-show-frozen.svg
--rw-rw-rw-   0 root         (0) root         (0)     6161 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/view-timer.svg
--rw-rw-rw-   0 root         (0) root         (0)    24550 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/view-zoom-in.svg
--rw-rw-rw-   0 root         (0) root         (0)    24925 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/view-zoom-original.svg
--rw-rw-rw-   0 root         (0) root         (0)    24352 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/actions/view-zoom-out.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-13 16:37:14.839642 pyspread-2.1.1/pyspread/share/icons/charts/
--rw-rw-rw-   0 root         (0) root         (0)     7186 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_area_1_1.svg
--rw-rw-rw-   0 root         (0) root         (0)     7163 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_area_1_2.svg
--rw-rw-rw-   0 root         (0) root         (0)     6953 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_area_1_3.svg
--rw-rw-rw-   0 root         (0) root         (0)     7282 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_bar_1_1.svg
--rw-rw-rw-   0 root         (0) root         (0)     8140 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_bar_1_2.svg
--rw-rw-rw-   0 root         (0) root         (0)     8922 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_bar_1_3.svg
--rw-rw-rw-   0 root         (0) root         (0)     9125 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_boxplot_1_1.svg
--rw-rw-rw-   0 root         (0) root         (0)     8637 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_boxplot_1_2.svg
--rw-rw-rw-   0 root         (0) root         (0)    11228 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_boxplot_2_1.svg
--rw-rw-rw-   0 root         (0) root         (0)    11076 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_boxplot_2_2.svg
--rw-rw-rw-   0 root         (0) root         (0)     8346 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_bubble_1_1.svg
--rw-rw-rw-   0 root         (0) root         (0)    10056 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_bubble_1_2.svg
--rw-rw-rw-   0 root         (0) root         (0)    11693 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_color_polar_1_1.svg
--rw-rw-rw-   0 root         (0) root         (0)     9249 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_colored_1_1.svg
--rw-rw-rw-   0 root         (0) root         (0)     7079 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_column_1_1.svg
--rw-rw-rw-   0 root         (0) root         (0)     7821 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_column_1_2.svg
--rw-rw-rw-   0 root         (0) root         (0)     8811 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_column_1_3.svg
--rw-rw-rw-   0 root         (0) root         (0)     8849 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_contour_1_1.svg
--rw-rw-rw-   0 root         (0) root         (0)     9078 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_contour_1_2.svg
--rw-rw-rw-   0 root         (0) root         (0)     9557 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_contour_2_1.svg
--rw-rw-rw-   0 root         (0) root         (0)     9544 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_contour_2_2.svg
--rw-rw-rw-   0 root         (0) root         (0)    10796 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_contour_polar_1_1.svg
--rw-rw-rw-   0 root         (0) root         (0)     8201 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_dropbar_1_1.svg
--rw-rw-rw-   0 root         (0) root         (0)     8325 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_dropbar_1_2.svg
--rw-rw-rw-   0 root         (0) root         (0)     8348 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_dropbar_1_3.svg
--rw-rw-rw-   0 root         (0) root         (0)     8485 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_dropbar_1_4.svg
--rw-rw-rw-   0 root         (0) root         (0)     7829 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_histogram_1_1.svg
--rw-rw-rw-   0 root         (0) root         (0)     8372 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_histogram_1_2.svg
--rw-rw-rw-   0 root         (0) root         (0)    10603 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_histogram_1_3.svg
--rw-rw-rw-   0 root         (0) root         (0)    10879 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_histogram_1_4.svg
--rw-rw-rw-   0 root         (0) root         (0)     7984 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_histogram_2_1.svg
--rw-rw-rw-   0 root         (0) root         (0)     7187 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_line_1_1.svg
--rw-rw-rw-   0 root         (0) root         (0)     7179 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_line_1_2.svg
--rw-rw-rw-   0 root         (0) root         (0)     6831 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_line_1_3.svg
--rw-rw-rw-   0 root         (0) root         (0)    10289 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_line_2_1.svg
--rw-rw-rw-   0 root         (0) root         (0)    10249 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_line_2_2.svg
--rw-rw-rw-   0 root         (0) root         (0)     9901 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_line_2_3.svg
--rw-rw-rw-   0 root         (0) root         (0)    17196 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_matrix_1_1.svg
--rw-rw-rw-   0 root         (0) root         (0)    17576 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_matrix_1_2.svg
--rw-rw-rw-   0 root         (0) root         (0)    17575 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_matrix_1_3.svg
--rw-rw-rw-   0 root         (0) root         (0)     8307 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_minmax_1_1.svg
--rw-rw-rw-   0 root         (0) root         (0)     8118 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_minmax_1_2.svg
--rw-rw-rw-   0 root         (0) root         (0)    10151 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_minmax_1_3.svg
--rw-rw-rw-   0 root         (0) root         (0)    10108 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_minmax_1_4.svg
--rw-rw-rw-   0 root         (0) root         (0)    10598 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_minmax_2_1.svg
--rw-rw-rw-   0 root         (0) root         (0)    10502 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_minmax_2_2.svg
--rw-rw-rw-   0 root         (0) root         (0)    11256 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_minmax_2_3.svg
--rw-rw-rw-   0 root         (0) root         (0)    14956 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_minmax_2_4.svg
--rw-rw-rw-   0 root         (0) root         (0)     9173 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_pie_1_1.svg
--rw-rw-rw-   0 root         (0) root         (0)     7522 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_pie_2_1.svg
--rw-rw-rw-   0 root         (0) root         (0)     7644 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_pie_3_1.svg
--rw-rw-rw-   0 root         (0) root         (0)     7603 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_pie_3_2.svg
--rw-rw-rw-   0 root         (0) root         (0)     9193 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_polar_1_1.svg
--rw-rw-rw-   0 root         (0) root         (0)     7456 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_prob_1_1.svg
--rw-rw-rw-   0 root         (0) root         (0)     8665 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_radar_1_1.svg
--rw-rw-rw-   0 root         (0) root         (0)    11428 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_radar_1_2.svg
--rw-rw-rw-   0 root         (0) root         (0)     8669 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_radar_1_3.svg
--rw-rw-rw-   0 root         (0) root         (0)    10288 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_ring_1_1.svg
--rw-rw-rw-   0 root         (0) root         (0)    10284 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_ring_1_2.svg
--rw-rw-rw-   0 root         (0) root         (0)     8886 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_scatter_1_1.svg
--rw-rw-rw-   0 root         (0) root         (0)     9688 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_scatter_3_1.svg
--rw-rw-rw-   0 root         (0) root         (0)     6618 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_scatter_3_2.svg
--rw-rw-rw-   0 root         (0) root         (0)     6903 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_scatter_3_3.svg
--rw-rw-rw-   0 root         (0) root         (0)     6721 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_scatter_4_1.svg
--rw-rw-rw-   0 root         (0) root         (0)     6887 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_scatter_4_2.svg
--rw-rw-rw-   0 root         (0) root         (0)     6933 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_scatter_4_3.svg
--rw-rw-rw-   0 root         (0) root         (0)     6933 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_scatter_4_4.svg
--rw-rw-rw-   0 root         (0) root         (0)     9907 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_scatterhist_1_1.svg
--rw-rw-rw-   0 root         (0) root         (0)    44800 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_surface_2_1.svg
--rw-rw-rw-   0 root         (0) root         (0)    45240 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_surface_2_2.svg
--rw-rw-rw-   0 root         (0) root         (0)    45395 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/charts/chart_surface_2_3.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-13 16:37:14.728631 pyspread-2.1.1/pyspread/share/icons/hicolor/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-13 16:37:14.840642 pyspread-2.1.1/pyspread/share/icons/hicolor/64x64/
--rw-rw-rw-   0 root         (0) root         (0)    10550 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/hicolor/64x64/pyspread.ico
--rw-rw-rw-   0 root         (0) root         (0)     5285 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/hicolor/64x64/pyspread.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-13 16:37:14.840642 pyspread-2.1.1/pyspread/share/icons/hicolor/svg/
--rw-rw-rw-   0 root         (0) root         (0)   330549 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/hicolor/svg/pyspread.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-13 16:37:14.841642 pyspread-2.1.1/pyspread/share/icons/status/
--rw-rw-rw-   0 root         (0) root         (0)     4870 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/status/status-safe-mode.svg
--rw-rw-rw-   0 root         (0) root         (0)    24423 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/icons/status/status-selection-mode.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-13 16:37:14.842642 pyspread-2.1.1/pyspread/share/metainfo/
--rw-rw-rw-   0 root         (0) root         (0)     2199 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/metainfo/io.gitlab.pyspread.pyspread.metainfo.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-13 16:37:14.729631 pyspread-2.1.1/pyspread/share/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-13 16:37:14.847643 pyspread-2.1.1/pyspread/share/templates/matplotlib/
--rw-rw-rw-   0 root         (0) root         (0)     2801 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/templates/matplotlib/COPYING
--rw-rw-rw-   0 root         (0) root         (0)      341 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/templates/matplotlib/chart_area_1_1.py
--rw-rw-rw-   0 root         (0) root         (0)     1883 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/templates/matplotlib/chart_bar_1_3.py
--rw-rw-rw-   0 root         (0) root         (0)      795 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/templates/matplotlib/chart_boxplot_2_2.py
--rw-rw-rw-   0 root         (0) root         (0)      377 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/templates/matplotlib/chart_bubble_1_1.py
--rw-rw-rw-   0 root         (0) root         (0)     1071 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/templates/matplotlib/chart_column_1_1.py
--rw-rw-rw-   0 root         (0) root         (0)      659 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/templates/matplotlib/chart_column_1_2.py
--rw-rw-rw-   0 root         (0) root         (0)      669 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/templates/matplotlib/chart_contour_1_2.py
--rw-rw-rw-   0 root         (0) root         (0)      379 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/templates/matplotlib/chart_histogram_1_1.py
--rw-rw-rw-   0 root         (0) root         (0)     1365 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/templates/matplotlib/chart_histogram_1_4.py
--rw-rw-rw-   0 root         (0) root         (0)      247 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/templates/matplotlib/chart_line_1_1.py
--rw-rw-rw-   0 root         (0) root         (0)      503 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/templates/matplotlib/chart_matrix_1_1.py
--rw-rw-rw-   0 root         (0) root         (0)      456 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/templates/matplotlib/chart_pie_1_1.py
--rw-rw-rw-   0 root         (0) root         (0)      378 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/templates/matplotlib/chart_polar_1_1.py
--rw-rw-rw-   0 root         (0) root         (0)      529 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/templates/matplotlib/chart_ring_1_1.py
--rw-rw-rw-   0 root         (0) root         (0)      385 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/templates/matplotlib/chart_scatter_1_1.py
--rw-rw-rw-   0 root         (0) root         (0)     1392 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/templates/matplotlib/chart_scatterhist_1_1.py
--rw-rw-rw-   0 root         (0) root         (0)      542 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/share/templates/matplotlib/chart_surface_2_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-13 16:37:14.851643 pyspread-2.1.1/pyspread/test/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/test/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     2223 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/test/test_cli.py
--rw-rw-rw-   0 root         (0) root         (0)    40334 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/test/test_grid.py
--rw-rw-rw-   0 root         (0) root         (0)     5076 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/test/test_grid_renderer.py
--rw-rw-rw-   0 root         (0) root         (0)      120 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/test/test_invalid_unsigned_1.pysu
--rw-rw-rw-   0 root         (0) root         (0)      124 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/test/test_invalid_unsigned_2.pysu
--rw-rw-rw-   0 root         (0) root         (0)      126 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/test/test_invalid_unsigned_3.pysu
--rw-rw-rw-   0 root         (0) root         (0)     2691 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/test/test_pyspread.py
--rw-rw-rw-   0 root         (0) root         (0)      118 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/test/test_valid_signed.pysu
--rw-rw-rw-   0 root         (0) root         (0)      123 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/test/test_valid_unsigned.pysu
--rwxrwxrwx   0 root         (0) root         (0)     6822 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/test/test_workflows.py
--rw-rw-rw-   0 root         (0) root         (0)    11099 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/toolbar.py
--rw-rw-rw-   0 root         (0) root         (0)    22344 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/widgets.py
--rw-rw-rw-   0 root         (0) root         (0)    70811 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread/workflows.py
--rwxrwxrwx   0 root         (0) root         (0)      735 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread.desktop
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-13 16:37:14.741632 pyspread-2.1.1/pyspread.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5062 2022-11-13 16:37:14.000000 pyspread-2.1.1/pyspread.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    13917 2022-11-13 16:37:14.000000 pyspread-2.1.1/pyspread.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-13 16:37:14.000000 pyspread-2.1.1/pyspread.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2022-11-13 16:37:14.000000 pyspread-2.1.1/pyspread.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      147 2022-11-13 16:37:14.000000 pyspread-2.1.1/pyspread.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2022-11-13 16:37:14.000000 pyspread-2.1.1/pyspread.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)        9 2022-11-13 16:35:51.000000 pyspread-2.1.1/pyspread.pth
--rw-rw-rw-   0 root         (0) root         (0)      187 2022-11-13 16:35:51.000000 pyspread-2.1.1/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)       93 2022-11-13 16:37:14.852643 pyspread-2.1.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3495 2022-11-13 16:35:51.000000 pyspread-2.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:40:47.785955 pyspread-2.2/
+-rw-rw-rw-   0 root         (0) root         (0)       87 2023-04-16 18:39:21.000000 pyspread-2.2/AUTHORS
+-rw-rw-rw-   0 root         (0) root         (0)    35141 2023-04-16 18:39:21.000000 pyspread-2.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      307 2023-04-16 18:39:21.000000 pyspread-2.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5106 2023-04-16 18:40:47.785955 pyspread-2.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2608 2023-04-16 18:39:21.000000 pyspread-2.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      382 2023-04-16 18:39:21.000000 pyspread-2.2/THANKS
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 18:39:21.000000 pyspread-2.2/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14668 2023-04-16 18:39:21.000000 pyspread-2.2/changelog
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:40:47.671944 pyspread-2.2/pyspread/
+-rw-rw-rw-   0 root         (0) root         (0)       91 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      993 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)    48145 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/actions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3393 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    34733 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/commands.py
+-rw-rw-rw-   0 root         (0) root         (0)    58195 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/dialogs.py
+-rw-rw-rw-   0 root         (0) root         (0)     5900 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/entryline.py
+-rw-rw-rw-   0 root         (0) root         (0)    96463 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/grid.py
+-rw-rw-rw-   0 root         (0) root         (0)    31006 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/grid_renderer.py
+-rw-rw-rw-   0 root         (0) root         (0)     9372 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/icons.py
+-rw-rw-rw-   0 root         (0) root         (0)    11094 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/installer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:40:47.673944 pyspread-2.2/pyspread/interfaces/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/interfaces/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    19559 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/interfaces/pys.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:40:47.678944 pyspread-2.2/pyspread/lib/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1060 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/attrdict.py
+-rw-rw-rw-   0 root         (0) root         (0)     9886 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/charts.py
+-rw-rw-rw-   0 root         (0) root         (0)     4889 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/csv.py
+-rw-rw-rw-   0 root         (0) root         (0)    45208 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/dataclasses.py
+-rw-rw-rw-   0 root         (0) root         (0)     2109 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/exception_handling.py
+-rw-rw-rw-   0 root         (0) root         (0)     4077 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/file_helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2522 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/hashing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:40:47.679944 pyspread-2.2/pyspread/lib/packaging/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/packaging/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2022 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/packaging/_structures.py
+-rw-rw-rw-   0 root         (0) root         (0)     1437 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/packaging/_typing.py
+-rw-rw-rw-   0 root         (0) root         (0)    15480 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/packaging/version.py
+-rwxrwxrwx   0 root         (0) root         (0)    10984 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/qimage2ndarray.py
+-rw-rw-rw-   0 root         (0) root         (0)     2686 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/qimage_svg.py
+-rw-rw-rw-   0 root         (0) root         (0)    21086 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/selection.py
+-rw-rw-rw-   0 root         (0) root         (0)    25092 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/spelltextedit.py
+-rw-rw-rw-   0 root         (0) root         (0)     2093 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/string_helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:40:47.686945 pyspread-2.2/pyspread/lib/test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/test/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2289 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/test/compat.py
+-rw-rw-rw-   0 root         (0) root         (0)       13 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/test/invalid1.csv
+-rw-rw-rw-   0 root         (0) root         (0)       13 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/test/invalid2.csv
+-rw-rw-rw-   0 root         (0) root         (0)     3569 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/test/test_array2qimage.py
+-rw-rw-rw-   0 root         (0) root         (0)     5101 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/test/test_csv.py
+-rw-rw-rw-   0 root         (0) root         (0)     1457 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/test/test_file_helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2868 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/test/test_hashing.py
+-rw-rw-rw-   0 root         (0) root         (0)     5235 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/test/test_qimageview.py
+-rw-rw-rw-   0 root         (0) root         (0)    16899 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/test/test_selection.py
+-rw-rw-rw-   0 root         (0) root         (0)     1936 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/test/test_string_helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)       18 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/test/valid1.csv
+-rw-rw-rw-   0 root         (0) root         (0)       18 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/test/valid2.csv
+-rw-rw-rw-   0 root         (0) root         (0)  2287092 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/test/valid3.csv
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/test/valid4.csv
+-rw-rw-rw-   0 root         (0) root         (0)     2740 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/lib/typechecks.py
+-rw-rw-rw-   0 root         (0) root         (0)    27821 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/main_window.py
+-rw-rw-rw-   0 root         (0) root         (0)    16608 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/menus.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:40:47.687945 pyspread-2.2/pyspread/model/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/model/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    51556 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/model/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:40:47.688945 pyspread-2.2/pyspread/model/test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/model/test/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    19920 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/model/test/test_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     4539 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/panels.py
+-rwxrwxrwx   0 root         (0) root         (0)     2503 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/pyspread.py
+-rw-rw-rw-   0 root         (0) root         (0)    12573 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:40:47.688945 pyspread-2.2/pyspread/share/
+-rw-rw-rw-   0 root         (0) root         (0)    35141 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:40:47.688945 pyspread-2.2/pyspread/share/applications/
+-rwxrwxrwx   0 root         (0) root         (0)      761 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/applications/io.gitlab.pyspread.pyspread.desktop
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:40:47.657942 pyspread-2.2/pyspread/share/doc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:40:47.691946 pyspread-2.2/pyspread/share/doc/manual/
+-rw-rw-rw-   0 root         (0) root         (0)     3575 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/doc/manual/advanced_topics.md
+-rw-rw-rw-   0 root         (0) root         (0)    10408 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/doc/manual/basic_concepts.md
+-rw-rw-rw-   0 root         (0) root         (0)     4852 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/doc/manual/edit_menu.md
+-rw-rw-rw-   0 root         (0) root         (0)     7506 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/doc/manual/file_menu.md
+-rw-rw-rw-   0 root         (0) root         (0)     6821 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/doc/manual/format_menu.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:40:47.696946 pyspread-2.2/pyspread/share/doc/manual/images/
+-rw-rw-rw-   0 root         (0) root         (0)    18661 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/doc/manual/images/screenshot_approve_dialog.png
+-rw-rw-rw-   0 root         (0) root         (0)   130518 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/doc/manual/images/screenshot_chartdialog.png
+-rw-rw-rw-   0 root         (0) root         (0)    24102 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/doc/manual/images/screenshot_csv_export.png
+-rw-rw-rw-   0 root         (0) root         (0)    26708 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/doc/manual/images/screenshot_csv_import.png
+-rw-rw-rw-   0 root         (0) root         (0)     7186 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/doc/manual/images/screenshot_find_dialog.png
+-rw-rw-rw-   0 root         (0) root         (0)     7586 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/doc/manual/images/screenshot_macros.png
+-rw-rw-rw-   0 root         (0) root         (0)    91836 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/doc/manual/images/screenshot_main_window.png
+-rw-rw-rw-   0 root         (0) root         (0)    11767 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/doc/manual/images/screenshot_new_dialog.png
+-rw-rw-rw-   0 root         (0) root         (0)     8572 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/doc/manual/images/screenshot_paste_as.png
+-rw-rw-rw-   0 root         (0) root         (0)    19022 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/doc/manual/images/screenshot_preferences_dialog.png
+-rw-rw-rw-   0 root         (0) root         (0)    10973 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/doc/manual/images/screenshot_print_preview_1.png
+-rw-rw-rw-   0 root         (0) root         (0)    27303 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/doc/manual/images/screenshot_print_preview_2.png
+-rw-rw-rw-   0 root         (0) root         (0)    16783 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/doc/manual/images/screenshot_replace_dialog.png
+-rw-rw-rw-   0 root         (0) root         (0)     2360 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/doc/manual/macro_menu.md
+-rw-rw-rw-   0 root         (0) root         (0)     1289 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/doc/manual/overview.md
+-rw-rw-rw-   0 root         (0) root         (0)     2016 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/doc/manual/view_menu.md
+-rw-rw-rw-   0 root         (0) root         (0)     5723 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/doc/manual/workspace.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:40:47.696946 pyspread-2.2/pyspread/share/doc/tutorial/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:40:47.698946 pyspread-2.2/pyspread/share/doc/tutorial/images/
+-rw-rw-rw-   0 root         (0) root         (0)    61117 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/doc/tutorial/images/Tutorial1.png
+-rw-rw-rw-   0 root         (0) root         (0)    45217 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/doc/tutorial/images/Tutorial2.png
+-rw-rw-rw-   0 root         (0) root         (0)    54732 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/doc/tutorial/images/Tutorial3.png
+-rw-rw-rw-   0 root         (0) root         (0)    64569 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/doc/tutorial/images/Tutorial4.png
+-rw-rw-rw-   0 root         (0) root         (0)     4877 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/doc/tutorial/tutorial.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:40:47.709947 pyspread-2.2/pyspread/share/examples/
+-rw-rw-rw-   0 root         (0) root         (0)  8812542 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/examples/big.csv
+-rw-rw-rw-   0 root         (0) root         (0)      433 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/examples/conditional_formatting.pysu
+-rw-rw-rw-   0 root         (0) root         (0)    17191 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/examples/images and charts.pysu
+-rw-rw-rw-   0 root         (0) root         (0)     4185 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/examples/pivot.pysu
+-rw-rw-rw-   0 root         (0) root         (0)    11840 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/examples/pyspred_with_plotnine.pysu
+-rw-rw-rw-   0 root         (0) root         (0)     5841 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/examples/rpy2_example.pysu
+-rw-rw-rw-   0 root         (0) root         (0)    29100 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/examples/test_write.csv
+-rw-rw-rw-   0 root         (0) root         (0)    21717 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/examples/wagner_whitin.pysu
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:40:47.659942 pyspread-2.2/pyspread/share/icons/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:40:47.746951 pyspread-2.2/pyspread/share/icons/actions/
+-rw-rw-rw-   0 root         (0) root         (0)   136218 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/document-approve.svg
+-rw-rw-rw-   0 root         (0) root         (0)    24975 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/document-export.svg
+-rw-rw-rw-   0 root         (0) root         (0)    21023 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/document-import.svg
+-rw-rw-rw-   0 root         (0) root         (0)    19127 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/document-log-out.svg
+-rw-rw-rw-   0 root         (0) root         (0)   165172 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/document-new-gpg-key.svg
+-rw-rw-rw-   0 root         (0) root         (0)    17406 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/document-new.svg
+-rw-rw-rw-   0 root         (0) root         (0)    30805 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/document-open.svg
+-rw-rw-rw-   0 root         (0) root         (0)    29401 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/document-page-setup.svg
+-rw-rw-rw-   0 root         (0) root         (0)    33813 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/document-print-preview.svg
+-rw-rw-rw-   0 root         (0) root         (0)    23333 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/document-print.svg
+-rw-rw-rw-   0 root         (0) root         (0)    25424 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/document-properties.svg
+-rw-rw-rw-   0 root         (0) root         (0)    31913 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/document-save-as.svg
+-rw-rw-rw-   0 root         (0) root         (0)    29894 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/document-save.svg
+-rw-rw-rw-   0 root         (0) root         (0)    19499 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/edit-clear.svg
+-rw-rw-rw-   0 root         (0) root         (0)    16456 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/edit-copy-results.svg
+-rw-rw-rw-   0 root         (0) root         (0)    15595 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/edit-copy.svg
+-rw-rw-rw-   0 root         (0) root         (0)    23051 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/edit-cut.svg
+-rw-rw-rw-   0 root         (0) root         (0)    35153 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/edit-delete-column.svg
+-rw-rw-rw-   0 root         (0) root         (0)    24107 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/edit-delete-row.svg
+-rw-rw-rw-   0 root         (0) root         (0)    21308 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/edit-delete-table.svg
+-rw-rw-rw-   0 root         (0) root         (0)    54926 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/edit-delete.svg
+-rw-rw-rw-   0 root         (0) root         (0)     4953 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/edit-find-next.svg
+-rw-rw-rw-   0 root         (0) root         (0)    45880 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/edit-find-replace.svg
+-rw-rw-rw-   0 root         (0) root         (0)    35412 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/edit-find.svg
+-rw-rw-rw-   0 root         (0) root         (0)    14246 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/edit-insert-column.svg
+-rw-rw-rw-   0 root         (0) root         (0)    13993 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/edit-insert-row.svg
+-rw-rw-rw-   0 root         (0) root         (0)    12163 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/edit-insert-table.svg
+-rw-rw-rw-   0 root         (0) root         (0)     8988 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/edit-paste-as.svg
+-rw-rw-rw-   0 root         (0) root         (0)    23755 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/edit-paste.svg
+-rw-rw-rw-   0 root         (0) root         (0)    37205 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/edit-quote.svg
+-rw-rw-rw-   0 root         (0) root         (0)     9331 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/edit-redo.svg
+-rw-rw-rw-   0 root         (0) root         (0)     6028 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/edit-resize-grid.svg
+-rw-rw-rw-   0 root         (0) root         (0)    15903 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/edit-select-all.svg
+-rw-rw-rw-   0 root         (0) root         (0)    17679 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/edit-sort-ascending.svg
+-rw-rw-rw-   0 root         (0) root         (0)    18405 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/edit-sort-descending.svg
+-rw-rw-rw-   0 root         (0) root         (0)     9235 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/edit-undo.svg
+-rw-rw-rw-   0 root         (0) root         (0)    10364 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-background-color.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1992 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-borders-0.svg
+-rw-rw-rw-   0 root         (0) root         (0)     2273 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-borders-1.svg
+-rw-rw-rw-   0 root         (0) root         (0)     2275 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-borders-16.svg
+-rw-rw-rw-   0 root         (0) root         (0)     2273 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-borders-2.svg
+-rw-rw-rw-   0 root         (0) root         (0)     2275 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-borders-32.svg
+-rw-rw-rw-   0 root         (0) root         (0)     2273 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-borders-4.svg
+-rw-rw-rw-   0 root         (0) root         (0)     2274 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-borders-64.svg
+-rw-rw-rw-   0 root         (0) root         (0)     2275 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-borders-8.svg
+-rw-rw-rw-   0 root         (0) root         (0)     3709 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-borders-all.svg
+-rw-rw-rw-   0 root         (0) root         (0)     3947 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-borders-bottom.svg
+-rw-rw-rw-   0 root         (0) root         (0)     3906 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-borders-inner.svg
+-rw-rw-rw-   0 root         (0) root         (0)     4029 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-borders-left.svg
+-rw-rw-rw-   0 root         (0) root         (0)     3799 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-borders-outer.svg
+-rw-rw-rw-   0 root         (0) root         (0)     4029 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-borders-right.svg
+-rw-rw-rw-   0 root         (0) root         (0)     3879 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-borders-top-bottom.svg
+-rw-rw-rw-   0 root         (0) root         (0)     3883 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-borders-top.svg
+-rw-rw-rw-   0 root         (0) root         (0)     3801 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-button.svg
+-rw-rw-rw-   0 root         (0) root         (0)    44063 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-cell-chart.svg
+-rw-rw-rw-   0 root         (0) root         (0)   718331 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-cell-image.svg
+-rw-rw-rw-   0 root         (0) root         (0)    41228 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-cell-markup.svg
+-rw-rw-rw-   0 root         (0) root         (0)    14454 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-cell-rotate-0.svg
+-rw-rw-rw-   0 root         (0) root         (0)    14581 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-cell-rotate-180.svg
+-rw-rw-rw-   0 root         (0) root         (0)    14580 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-cell-rotate-270.svg
+-rw-rw-rw-   0 root         (0) root         (0)    15749 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-cell-rotate-90.svg
+-rw-rw-rw-   0 root         (0) root         (0)    27835 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-cell-text.svg
+-rw-rw-rw-   0 root         (0) root         (0)    12343 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-copy.svg
+-rw-rw-rw-   0 root         (0) root         (0)    12731 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-font.svg
+-rw-rw-rw-   0 root         (0) root         (0)    18923 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-freeze.svg
+-rw-rw-rw-   0 root         (0) root         (0)    13344 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-justify-center.svg
+-rw-rw-rw-   0 root         (0) root         (0)    13332 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-justify-fill.svg
+-rw-rw-rw-   0 root         (0) root         (0)    11136 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-justify-left.svg
+-rw-rw-rw-   0 root         (0) root         (0)    13382 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-justify-right.svg
+-rw-rw-rw-   0 root         (0) root         (0)     7716 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-line-color.svg
+-rw-rw-rw-   0 root         (0) root         (0)     8658 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-line-color2.svg
+-rw-rw-rw-   0 root         (0) root         (0)   143193 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-lock.svg
+-rw-rw-rw-   0 root         (0) root         (0)     2441 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-merge-cells.svg
+-rw-rw-rw-   0 root         (0) root         (0)    37466 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-paste.svg
+-rw-rw-rw-   0 root         (0) root         (0)    12457 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-text-align-bottom.svg
+-rw-rw-rw-   0 root         (0) root         (0)    12574 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-text-align-center.svg
+-rw-rw-rw-   0 root         (0) root         (0)    12794 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-text-align-top.svg
+-rw-rw-rw-   0 root         (0) root         (0)    10953 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-text-bold.svg
+-rw-rw-rw-   0 root         (0) root         (0)     6484 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-text-color.svg
+-rw-rw-rw-   0 root         (0) root         (0)    11302 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-text-italic.svg
+-rw-rw-rw-   0 root         (0) root         (0)    14525 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-text-strikethrough.svg
+-rw-rw-rw-   0 root         (0) root         (0)    14583 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/format-text-underline.svg
+-rw-rw-rw-   0 root         (0) root         (0)   121867 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/help-browser.svg
+-rw-rw-rw-   0 root         (0) root         (0)   353099 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/help-dependencies.svg
+-rw-rw-rw-   0 root         (0) root         (0)     5737 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/help-faq.svg
+-rw-rw-rw-   0 root         (0) root         (0)      503 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/help-tutorial.svg
+-rw-rw-rw-   0 root         (0) root         (0)    41994 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/macro-insert-chart.svg
+-rw-rw-rw-   0 root         (0) root         (0)   396438 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/macro-insert-image.svg
+-rw-rw-rw-   0 root         (0) root         (0)    21889 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/macro-insert-sum.svg
+-rw-rw-rw-   0 root         (0) root         (0)   388308 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/macro-link-image.svg
+-rw-rw-rw-   0 root         (0) root         (0)    10037 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/macro-open.svg
+-rw-rw-rw-   0 root         (0) root         (0)    10693 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/macro-save.svg
+-rw-rw-rw-   0 root         (0) root         (0)    19612 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/menu-manager.svg
+-rw-rw-rw-   0 root         (0) root         (0)    23289 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/view-check-spelling.svg
+-rw-rw-rw-   0 root         (0) root         (0)    20295 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/view-fullscreen.svg
+-rw-rw-rw-   0 root         (0) root         (0)     3176 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/view-goto-cell.svg
+-rw-rw-rw-   0 root         (0) root         (0)    16868 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/view-refresh.svg
+-rw-rw-rw-   0 root         (0) root         (0)    20510 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/view-show-frozen.svg
+-rw-rw-rw-   0 root         (0) root         (0)     6161 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/view-timer.svg
+-rw-rw-rw-   0 root         (0) root         (0)    24550 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/view-zoom-in.svg
+-rw-rw-rw-   0 root         (0) root         (0)    24925 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/view-zoom-original.svg
+-rw-rw-rw-   0 root         (0) root         (0)    24352 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/actions/view-zoom-out.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:40:47.771954 pyspread-2.2/pyspread/share/icons/charts/
+-rw-rw-rw-   0 root         (0) root         (0)     7186 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_area_1_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)     7163 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_area_1_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)     6953 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_area_1_3.svg
+-rw-rw-rw-   0 root         (0) root         (0)     7282 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_bar_1_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)     8140 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_bar_1_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)     8922 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_bar_1_3.svg
+-rw-rw-rw-   0 root         (0) root         (0)     9125 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_boxplot_1_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)     8637 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_boxplot_1_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)    11228 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_boxplot_2_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)    11076 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_boxplot_2_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)     8346 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_bubble_1_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)    10056 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_bubble_1_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)    11693 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_color_polar_1_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)     9249 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_colored_1_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)     7079 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_column_1_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)     7821 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_column_1_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)     8811 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_column_1_3.svg
+-rw-rw-rw-   0 root         (0) root         (0)     8849 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_contour_1_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)     9078 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_contour_1_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)     9557 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_contour_2_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)     9544 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_contour_2_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)    10796 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_contour_polar_1_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)     8201 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_dropbar_1_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)     8325 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_dropbar_1_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)     8348 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_dropbar_1_3.svg
+-rw-rw-rw-   0 root         (0) root         (0)     8485 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_dropbar_1_4.svg
+-rw-rw-rw-   0 root         (0) root         (0)     7829 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_histogram_1_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)     8372 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_histogram_1_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)    10603 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_histogram_1_3.svg
+-rw-rw-rw-   0 root         (0) root         (0)    10879 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_histogram_1_4.svg
+-rw-rw-rw-   0 root         (0) root         (0)     7984 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_histogram_2_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)     7187 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_line_1_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)     7179 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_line_1_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)     6831 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_line_1_3.svg
+-rw-rw-rw-   0 root         (0) root         (0)    10289 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_line_2_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)    10249 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_line_2_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)     9901 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_line_2_3.svg
+-rw-rw-rw-   0 root         (0) root         (0)    17196 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_matrix_1_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)    17576 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_matrix_1_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)    17575 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_matrix_1_3.svg
+-rw-rw-rw-   0 root         (0) root         (0)     8307 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_minmax_1_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)     8118 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_minmax_1_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)    10151 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_minmax_1_3.svg
+-rw-rw-rw-   0 root         (0) root         (0)    10108 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_minmax_1_4.svg
+-rw-rw-rw-   0 root         (0) root         (0)    10598 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_minmax_2_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)    10502 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_minmax_2_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)    11256 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_minmax_2_3.svg
+-rw-rw-rw-   0 root         (0) root         (0)    14956 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_minmax_2_4.svg
+-rw-rw-rw-   0 root         (0) root         (0)     9173 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_pie_1_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)     7522 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_pie_2_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)     7644 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_pie_3_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)     7603 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_pie_3_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)    14131 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_plotnine_geom_bar_1_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)     9193 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_polar_1_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)     7456 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_prob_1_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)    11134 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_r_ggplot2_geom_boxplot_1_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)    11371 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_r_ggplot2_geom_density2d_1_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)    11557 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_r_ggplot2_geom_point_1_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)     9745 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_r_graphics_barplot_1_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)    47553 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_r_lattice_wireframe_2_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)    11561 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_r_lattice_xyplot_1_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)     8665 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_radar_1_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)    11428 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_radar_1_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)     8669 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_radar_1_3.svg
+-rw-rw-rw-   0 root         (0) root         (0)    10288 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_ring_1_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)    10284 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_ring_1_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)     8886 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_scatter_1_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)     9688 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_scatter_3_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)     6618 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_scatter_3_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)     6903 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_scatter_3_3.svg
+-rw-rw-rw-   0 root         (0) root         (0)     6721 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_scatter_4_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)     6887 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_scatter_4_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)     6933 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_scatter_4_3.svg
+-rw-rw-rw-   0 root         (0) root         (0)     6933 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_scatter_4_4.svg
+-rw-rw-rw-   0 root         (0) root         (0)     9907 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_scatterhist_1_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)    44800 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_surface_2_1.svg
+-rw-rw-rw-   0 root         (0) root         (0)    45240 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_surface_2_2.svg
+-rw-rw-rw-   0 root         (0) root         (0)    45395 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/charts/chart_surface_2_3.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:40:47.659942 pyspread-2.2/pyspread/share/icons/hicolor/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:40:47.772954 pyspread-2.2/pyspread/share/icons/hicolor/64x64/
+-rw-rw-rw-   0 root         (0) root         (0)    10550 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/hicolor/64x64/pyspread.ico
+-rw-rw-rw-   0 root         (0) root         (0)     5285 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/hicolor/64x64/pyspread.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:40:47.772954 pyspread-2.2/pyspread/share/icons/hicolor/svg/
+-rw-rw-rw-   0 root         (0) root         (0)   330549 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/hicolor/svg/pyspread.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:40:47.773954 pyspread-2.2/pyspread/share/icons/status/
+-rw-rw-rw-   0 root         (0) root         (0)     4870 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/status/status-safe-mode.svg
+-rw-rw-rw-   0 root         (0) root         (0)    24423 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/icons/status/status-selection-mode.svg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:40:47.774954 pyspread-2.2/pyspread/share/metainfo/
+-rw-rw-rw-   0 root         (0) root         (0)     2199 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/metainfo/io.gitlab.pyspread.pyspread.metainfo.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:40:47.660942 pyspread-2.2/pyspread/share/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:40:47.779955 pyspread-2.2/pyspread/share/templates/matplotlib/
+-rw-rw-rw-   0 root         (0) root         (0)     2879 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/templates/matplotlib/COPYING
+-rw-rw-rw-   0 root         (0) root         (0)      341 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/templates/matplotlib/chart_area_1_1.py
+-rw-rw-rw-   0 root         (0) root         (0)     1883 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/templates/matplotlib/chart_bar_1_3.py
+-rw-rw-rw-   0 root         (0) root         (0)      795 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/templates/matplotlib/chart_boxplot_2_2.py
+-rw-rw-rw-   0 root         (0) root         (0)      377 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/templates/matplotlib/chart_bubble_1_1.py
+-rw-rw-rw-   0 root         (0) root         (0)     1071 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/templates/matplotlib/chart_column_1_1.py
+-rw-rw-rw-   0 root         (0) root         (0)      659 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/templates/matplotlib/chart_column_1_2.py
+-rw-rw-rw-   0 root         (0) root         (0)      669 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/templates/matplotlib/chart_contour_1_2.py
+-rw-rw-rw-   0 root         (0) root         (0)      379 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/templates/matplotlib/chart_histogram_1_1.py
+-rw-rw-rw-   0 root         (0) root         (0)     1365 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/templates/matplotlib/chart_histogram_1_4.py
+-rw-rw-rw-   0 root         (0) root         (0)      247 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/templates/matplotlib/chart_line_1_1.py
+-rw-rw-rw-   0 root         (0) root         (0)      503 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/templates/matplotlib/chart_matrix_1_1.py
+-rw-rw-rw-   0 root         (0) root         (0)      456 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/templates/matplotlib/chart_pie_1_1.py
+-rw-rw-rw-   0 root         (0) root         (0)      378 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/templates/matplotlib/chart_polar_1_1.py
+-rw-rw-rw-   0 root         (0) root         (0)      529 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/templates/matplotlib/chart_ring_1_1.py
+-rw-rw-rw-   0 root         (0) root         (0)      385 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/templates/matplotlib/chart_scatter_1_1.py
+-rw-rw-rw-   0 root         (0) root         (0)     1392 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/templates/matplotlib/chart_scatterhist_1_1.py
+-rw-rw-rw-   0 root         (0) root         (0)      542 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/templates/matplotlib/chart_surface_2_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:40:47.779955 pyspread-2.2/pyspread/share/templates/plotnine/
+-rw-rw-rw-   0 root         (0) root         (0)      190 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/templates/plotnine/chart_plotnine_geom_bar_1_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:40:47.781955 pyspread-2.2/pyspread/share/templates/rpy2/
+-rw-rw-rw-   0 root         (0) root         (0)      679 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/templates/rpy2/chart_r_ggplot2_geom_boxplot_1_2.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/templates/rpy2/chart_r_ggplot2_geom_density2d_1_2.py
+-rw-rw-rw-   0 root         (0) root         (0)      687 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/templates/rpy2/chart_r_ggplot2_geom_point_1_1.py
+-rw-rw-rw-   0 root         (0) root         (0)      416 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/templates/rpy2/chart_r_graphics_barplot_1_1.py
+-rw-rw-rw-   0 root         (0) root         (0)      777 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/templates/rpy2/chart_r_lattice_wireframe_2_1.py
+-rw-rw-rw-   0 root         (0) root         (0)      744 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/share/templates/rpy2/chart_r_lattice_xyplot_1_1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:40:47.785955 pyspread-2.2/pyspread/test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/test/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     2223 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/test/test_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    40334 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/test/test_grid.py
+-rw-rw-rw-   0 root         (0) root         (0)     5076 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/test/test_grid_renderer.py
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/test/test_invalid_unsigned_1.pysu
+-rw-rw-rw-   0 root         (0) root         (0)      124 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/test/test_invalid_unsigned_2.pysu
+-rw-rw-rw-   0 root         (0) root         (0)      126 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/test/test_invalid_unsigned_3.pysu
+-rw-rw-rw-   0 root         (0) root         (0)     2691 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/test/test_pyspread.py
+-rw-rw-rw-   0 root         (0) root         (0)      118 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/test/test_valid_signed.pysu
+-rw-rw-rw-   0 root         (0) root         (0)      123 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/test/test_valid_unsigned.pysu
+-rwxrwxrwx   0 root         (0) root         (0)     6822 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/test/test_workflows.py
+-rw-rw-rw-   0 root         (0) root         (0)    14289 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/toolbar.py
+-rw-rw-rw-   0 root         (0) root         (0)    22344 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/widgets.py
+-rw-rw-rw-   0 root         (0) root         (0)    71033 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread/workflows.py
+-rwxrwxrwx   0 root         (0) root         (0)      735 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread.desktop
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 18:40:47.673944 pyspread-2.2/pyspread.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5106 2023-04-16 18:40:47.000000 pyspread-2.2/pyspread.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    14895 2023-04-16 18:40:47.000000 pyspread-2.2/pyspread.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 18:40:47.000000 pyspread-2.2/pyspread.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-04-16 18:40:47.000000 pyspread-2.2/pyspread.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      191 2023-04-16 18:40:47.000000 pyspread-2.2/pyspread.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-04-16 18:40:47.000000 pyspread-2.2/pyspread.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)        9 2023-04-16 18:39:21.000000 pyspread-2.2/pyspread.pth
+-rw-rw-rw-   0 root         (0) root         (0)      218 2023-04-16 18:39:21.000000 pyspread-2.2/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)       93 2023-04-16 18:40:47.786955 pyspread-2.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3578 2023-04-16 18:39:21.000000 pyspread-2.2/setup.py
```

### Comparing `pyspread-2.1.1/LICENSE` & `pyspread-2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/PKG-INFO` & `pyspread-2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspread
-Version: 2.1.1
+Version: 2.2
 Summary: Pyspread is a non-traditional spreadsheet application that is based on and written in the programming language Python.
 Home-page: https://pyspread.gitlab.io
 Author: Martin Manns
 Author-email: mmanns@gmx.net
 License: GPL v3 :: GNU General Public License
 Project-URL: Bug Tracker, https://gitlab.com/pyspread/pyspread/issues
 Project-URL: Documentation, https://pyspread.gitlab.io/docs.html
@@ -127,10 +127,12 @@
 Requires: PyQt5 (>=5.10)
 Requires: setuptools (>=40.0)
 Requires: markdown2 (>=2.3)
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: matplotlib
 Provides-Extra: pip
+Provides-Extra: plotnine
 Provides-Extra: py-moneyed
 Provides-Extra: pyenchant
 Provides-Extra: python-dateutil
+Provides-Extra: rpy2
```

### Comparing `pyspread-2.1.1/README.md` & `pyspread-2.2/README.md`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/changelog` & `pyspread-2.2/changelog`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,28 @@
 Changelog for pyspread
 ======================
 
 Note: This changelog does not comprise development of pyspread for Python2
       It starts with the first Alpha release 1.99.0.0
 
 
+2.2
+---
+
+This release adds R charts via rpy2. Examples are available in the chart dialog.
+Note that the R packages graphics, lattice and ggplot2 are used for the examples.
+
+Dependencies:
+ * Mandatory: Python (≥ 3.6), numpy (>=1.1), PyQt5 (≥ 5.10, requires PyQt5.Svg), setuptools (>=40.0), markdown2 (>= 2.3)
+ * Recommended: matplotlib (>=1.1.1), pyenchant (>=1.1), pip (>=18), python-dateutil (>= 2.7.0), py-moneyed (>=2.0), rpy2 (>=3.4), plotnine (>=0.8)
+ * For building the apidocs with Sphinx see apidocs/requirements.txt
+
+Bug fixes:
+ * Thick lines are now antialiased
+ 
 2.1.1
 -----
 
 This is a bugfix release
 
 Dependencies:
  * Mandatory: Python (≥ 3.6), numpy (>=1.1), PyQt5 (≥ 5.10, requires PyQt5.Svg), setuptools (>=40.0), markdown2 (>= 2.3)
```

### Comparing `pyspread-2.1.1/pyspread/__main__.py` & `pyspread-2.2/pyspread/__main__.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/actions.py` & `pyspread-2.2/pyspread/actions.py`

 * *Files 5% similar despite different names*

```diff
@@ -939,14 +939,70 @@
         self.chart_surface_2_1 = Action(self.parent, "Surface chart",
                                         self.parent.on_template,
                                         icon=Icon.chart_surface_2_1,
                                         statustip='Insert code for surface '
                                                   'chart')
         self.chart_surface_2_1.setData("chart_surface_2_1.py")
 
+        self.chart_plotnine_geom_bar_1_1 = \
+            Action(self.parent, "Plotnine geom_bar chart",
+                   self.parent.on_template,
+                   icon=Icon.chart_plotnine_geom_bar_1_1,
+                   statustip='Insert code for plotnine geom_bar chart')
+        self.chart_plotnine_geom_bar_1_1.setData(
+            "chart_plotnine_geom_bar_1_1.py")
+
+        self.chart_r_graphics_barplot_1_1 = \
+            Action(self.parent, "R graphics barplot chart",
+                   self.parent.on_template,
+                   icon=Icon.chart_r_graphics_barplot_1_1,
+                   statustip='Insert code for R graphics barplot chart')
+        self.chart_r_graphics_barplot_1_1.setData(
+            "chart_r_graphics_barplot_1_1.py")
+
+        self.chart_r_ggplot2_geom_boxplot_1_2 = \
+            Action(self.parent, "R ggplot2 geom_boxplot chart",
+                   self.parent.on_template,
+                   icon=Icon.chart_r_ggplot2_geom_boxplot_1_2,
+                   statustip='Insert code for R ggplot2 geom_boxplot chart')
+        self.chart_r_ggplot2_geom_boxplot_1_2.setData(
+            "chart_r_ggplot2_geom_boxplot_1_2.py")
+
+        self.chart_r_ggplot2_geom_point_1_1 = \
+            Action(self.parent, "R ggplot2 geom_point chart",
+                   self.parent.on_template,
+                   icon=Icon.chart_r_ggplot2_geom_point_1_1,
+                   statustip='Insert code for R ggplot2 geom_point chart')
+        self.chart_r_ggplot2_geom_point_1_1.setData(
+            "chart_r_ggplot2_geom_point_1_1.py")
+
+        self.chart_r_lattice_xyplot_1_1 = \
+            Action(self.parent, "R lattice xyplot chart",
+                   self.parent.on_template,
+                   icon=Icon.chart_r_lattice_xyplot_1_1,
+                   statustip='Insert code for R lattice xyplot chart')
+        self.chart_r_lattice_xyplot_1_1.setData(
+            "chart_r_lattice_xyplot_1_1.py")
+
+        self.chart_r_ggplot2_geom_density2d_1_2 = \
+            Action(self.parent, "R ggplot2 geom_density2d chart",
+                   self.parent.on_template,
+                   icon=Icon.chart_r_ggplot2_geom_density2d_1_2,
+                   statustip='Insert code for R ggplot2 geom_density2d chart')
+        self.chart_r_ggplot2_geom_density2d_1_2.setData(
+            "chart_r_ggplot2_geom_density2d_1_2.py")
+
+        self.chart_r_lattice_wireframe_2_1 = \
+            Action(self.parent, "R lattice wireframe chart",
+                   self.parent.on_template,
+                   icon=Icon.chart_r_lattice_wireframe_2_1,
+                   statustip='Insert code for surface chart')
+        self.chart_r_lattice_wireframe_2_1.setData(
+            "chart_r_lattice_wireframe_2_1.py")
+
 
 class SpellTextEditActions(AttrDict):
     """Holds QActions for SpellTextEdit"""
 
     def __init__(self, parent: QWidget):
         """
         :param parent: The parent object, normally :class:`pyspread.MainWindow`
```

### Comparing `pyspread-2.1.1/pyspread/cli.py` & `pyspread-2.2/pyspread/cli.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/commands.py` & `pyspread-2.2/pyspread/commands.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/dialogs.py` & `pyspread-2.2/pyspread/dialogs.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,38 +66,41 @@
             QFormLayout, QVBoxLayout, QGroupBox, QDialogButtonBox, QSplitter,
             QTextBrowser, QCheckBox, QGridLayout, QLayout, QHBoxLayout,
             QPushButton, QWidget, QComboBox, QTableView, QAbstractItemView,
             QPlainTextEdit, QToolBar, QMainWindow, QTabWidget, QInputDialog)
 from PyQt5.QtGui \
     import (QIntValidator, QImageWriter, QStandardItemModel, QStandardItem,
             QValidator, QWheelEvent)
-
+from PyQt5.QtSvg import QSvgWidget
 from PyQt5.QtPrintSupport import (QPrintPreviewDialog, QPrintPreviewWidget,
                                   QPrinter)
 
 try:
     from matplotlib.figure import Figure
     from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg
 except ImportError:
     Figure = None
 
 try:
     from pyspread.actions import ChartDialogActions
-    from pyspread.toolbar import ChartTemplatesToolBar
+    from pyspread.toolbar import ChartTemplatesToolBar, RChartTemplatesToolBar
     from pyspread.widgets import HelpBrowser, TypeMenuComboBox
     from pyspread.lib.csv import sniff, csv_reader, get_header, convert
     from pyspread.lib.spelltextedit import SpellTextEdit
-    from pyspread.settings import TUTORIAL_PATH, MANUAL_PATH, MPL_TEMPLATE_PATH
+    from pyspread.settings import (TUTORIAL_PATH, MANUAL_PATH,
+                                   MPL_TEMPLATE_PATH, RPY2_TEMPLATE_PATH,
+                                   PLOT9_TEMPLATE_PATH)
 except ImportError:
     from actions import ChartDialogActions
-    from toolbar import ChartTemplatesToolBar
+    from toolbar import ChartTemplatesToolBar, RChartTemplatesToolBar
     from widgets import HelpBrowser, TypeMenuComboBox
     from lib.csv import sniff, csv_reader, get_header, convert
     from lib.spelltextedit import SpellTextEdit
-    from settings import TUTORIAL_PATH, MANUAL_PATH, MPL_TEMPLATE_PATH
+    from settings import (TUTORIAL_PATH, MANUAL_PATH, MPL_TEMPLATE_PATH,
+                          RPY2_TEMPLATE_PATH, PLOT9_TEMPLATE_PATH)
 
 
 class DiscardChangesDialog:
     """Modal dialog that asks if the user wants to discard or save unsaved data
 
     The modal dialog is shown on accessing the property choice.
 
@@ -927,15 +930,15 @@
         self.replace_all_button.clicked.connect(p_onreplaceall)
 
 
 class ChartDialog(QDialog):
     """The chart dialog"""
 
     def __init__(self, parent: QWidget, key: Tuple[int, int, int],
-                 size: Tuple[int, int] = (800, 600)):
+                 size: Tuple[int, int] = (1000, 700)):
         """
         :param parent: Parent window
         :param key: Target cell for chart
         :param size: Initial dialog size
 
         """
 
@@ -945,33 +948,41 @@
             raise ImportError
 
         super().__init__(parent)
 
         self.actions = ChartDialogActions(self)
 
         self.chart_templates_toolbar = ChartTemplatesToolBar(self)
+        self.rchart_templates_toolbar = RChartTemplatesToolBar(self)
 
         self.setWindowTitle(f"Chart dialog for cell {key}")
 
         self.resize(*size)
         self.parent = parent
 
         self.actions = ChartDialogActions(self)
 
         self.dialog_ui()
 
     def on_template(self):
         """Event handler for pressing a template toolbar button"""
 
         chart_template_name = self.sender().data()
-        chart_template_path = MPL_TEMPLATE_PATH / chart_template_name
-        try:
-            with open(chart_template_path, encoding='utf8') as template_file:
-                chart_template_code = template_file.read()
-        except OSError:
+        chart_template_code = None
+
+        tpl_paths = MPL_TEMPLATE_PATH, RPY2_TEMPLATE_PATH, PLOT9_TEMPLATE_PATH
+        for tpl_path in tpl_paths:
+            full_tpl_path = tpl_path / chart_template_name
+            try:
+                with open(full_tpl_path, encoding='utf8') as template_file:
+                    chart_template_code = template_file.read()
+            except OSError:
+                pass
+
+        if chart_template_code is None:
             return
 
         self.editor.insertPlainText(chart_template_code)
 
     def dialog_ui(self):
         """Sets up dialog UI"""
 
@@ -991,15 +1002,19 @@
         self.splitter.addWidget(self.editor)
         self.splitter.addWidget(self.message)
         self.splitter.setOpaqueResize(False)
         self.splitter.setSizes([9999, 9999])
 
         # Layout
         layout = QVBoxLayout(self)
-        layout.addWidget(self.chart_templates_toolbar)
+
+        toolbar_layout = QHBoxLayout()
+        toolbar_layout.addWidget(self.chart_templates_toolbar)
+        toolbar_layout.addWidget(self.rchart_templates_toolbar)
+        layout.addLayout(toolbar_layout)
 
         layout.addWidget(self.splitter)
         layout.addWidget(buttonbox)
 
         self.setLayout(layout)
 
     def apply(self):
@@ -1019,14 +1034,26 @@
         if isinstance(figure, Figure):
             canvas = FigureCanvasQTAgg(figure)
             self.splitter.replaceWidget(1, canvas)
             try:
                 canvas.draw()
             except Exception:
                 pass
+        elif isinstance(figure, bytes) or isinstance(figure, str):
+            with redirect_stdout(filelike):
+                if isinstance(figure, str):
+                    figure = bytearray(figure, encoding='utf-8')
+                svg_widget = QSvgWidget()
+                self.splitter.replaceWidget(1, svg_widget)
+                svg_widget.renderer().load(figure)
+            stdout_str = filelike.getvalue()
+            if stdout_str:
+                stdout_str += "\n \n"
+                msg = stdout_str + f"Error:\n{figure}"
+                self.message.setText(msg)
         else:
             if isinstance(figure, Exception):
                 msg = stdout_str + f"Error:\n{figure}"
                 self.message.setText(msg)
             else:
                 msg = stdout_str
                 msg_text = "Error:\n{} has type '{}', " + \
```

### Comparing `pyspread-2.1.1/pyspread/entryline.py` & `pyspread-2.2/pyspread/entryline.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/grid.py` & `pyspread-2.2/pyspread/grid.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,30 +60,38 @@
     import matplotlib.figure
 except ImportError:
     matplotlib = None
 
 try:
     from pyspread import commands
     from pyspread.dialogs import DiscardDataDialog
-    from pyspread.grid_renderer import painter_save, CellRenderer, QColorCache
+    from pyspread.grid_renderer import (painter_save, CellRenderer,
+                                        QColorCache, BorderWidthBottomCache,
+                                        BorderWidthRightCache,
+                                        EdgeBordersCache,
+                                        BorderColorRightCache,
+                                        BorderColorBottomCache)
     from pyspread.model.model import (CodeArray, CellAttribute,
                                       DefaultCellAttributeDict)
     from pyspread.lib.attrdict import AttrDict
     from pyspread.lib.selection import Selection
     from pyspread.lib.string_helpers import quote, wrap_text
     from pyspread.lib.qimage2ndarray import array2qimage
     from pyspread.lib.typechecks import is_svg, check_shape_validity
     from pyspread.menus import (GridContextMenu, TableChoiceContextMenu,
                                 HorizontalHeaderContextMenu,
                                 VerticalHeaderContextMenu)
     from pyspread.widgets import CellButton
 except ImportError:
     import commands
     from dialogs import DiscardDataDialog
-    from grid_renderer import painter_save, CellRenderer, QColorCache
+    from grid_renderer import (painter_save, CellRenderer, QColorCache,
+                               BorderWidthBottomCache, BorderWidthRightCache,
+                               EdgeBordersCache, BorderColorRightCache,
+                               BorderColorBottomCache)
     from model.model import CodeArray, CellAttribute, DefaultCellAttributeDict
     from lib.attrdict import AttrDict
     from lib.selection import Selection
     from lib.string_helpers import quote, wrap_text
     from lib.qimage2ndarray import array2qimage
     from lib.typechecks import is_svg, check_shape_validity
     from menus import (GridContextMenu, TableChoiceContextMenu,
@@ -101,25 +109,30 @@
 
         """
 
         super().__init__()
 
         self.main_window = main_window
 
-        self.qcolor_cache = QColorCache(self)
-
         shape = main_window.settings.shape
 
         if model is None:
             self.model = GridTableModel(main_window, shape)
         else:
             self.model = model
 
         self.setModel(self.model)
 
+        self.qcolor_cache = QColorCache(self)
+        self.borderwidth_bottom_cache = BorderWidthBottomCache(self)
+        self.borderwidth_right_cache = BorderWidthRightCache(self)
+        self.edge_borders_cache = EdgeBordersCache()
+        self.border_color_bottom_cache = BorderColorBottomCache(self)
+        self.border_color_right_cache = BorderColorRightCache(self)
+
         self.table_choice = main_window.table_choice
 
         self.widget_indices = []  # Store each index with an indexWidget here
 
         # Signals
         self.model.dataChanged.connect(self.on_data_changed)
         self.selectionModel().currentChanged.connect(self.on_current_changed)
@@ -546,22 +559,29 @@
 
         if merge_area is None:
             merge_sel = Selection([], [], [], [], [])
         else:
             top, left, bottom, right = merge_area
             merge_sel = Selection([(top, left)], [(bottom, right)], [], [], [])
 
-        return not(self.selection.single_cell_selected()
-                   or merge_sel.get_bbox() == self.selection.get_bbox())
+        return not (self.selection.single_cell_selected()
+                    or merge_sel.get_bbox() == self.selection.get_bbox())
 
     # Event handlers
 
     def on_data_changed(self):
         """Event handler for data changes"""
 
+        self.qcolor_cache.clear()
+        self.borderwidth_bottom_cache.clear()
+        self.borderwidth_right_cache.clear()
+        self.edge_borders_cache.clear()
+        self.border_color_bottom_cache.clear()
+        self.border_color_right_cache.clear()
+
         if not self.main_window.settings.changed_since_save:
             self.main_window.settings.changed_since_save = True
             main_window_title = "* " + self.main_window.windowTitle()
             self.main_window.setWindowTitle(main_window_title)
 
     def on_current_changed(self, *_: Any):
         """Event handler for change of current cell"""
@@ -594,37 +614,41 @@
     def on_selection_changed(self):
         """Selection changed event handler"""
 
         if not self.main_window.settings.show_statusbar_sum:
             return
 
         try:
-            bbox = self.selection.get_bbox()
+            selection = self.selection
+            code_array = self.model.code_array
+            single_cell_selected = selection.single_cell_selected()
         except AttributeError:
             return
 
-        if bbox[0] != bbox[1]:
-            selected_cell_gen = self.selection.cell_generator(self.model.shape,
-                                                              self.table)
-            cell_list = list(selected_cell_gen)
-            msg = f"Selection: {len(cell_list)} cells"
-
-            res_gen = (self.model.code_array[key] for key in cell_list)
-            sum_list = [res for res in res_gen if res is not None]
-            msg_tpl = "     " + "     ".join(["Σ={}", "max={}", "min={}"])
-            if sum_list:
-                try:
-                    msg += msg_tpl.format(sum(sum_list),
-                                          max(sum_list), min(sum_list))
-                except Exception:
-                    pass
-
-            self.main_window.statusBar().showMessage(msg)
-        else:
+        if not selection or single_cell_selected:
             self.main_window.statusBar().clearMessage()
+            return
+
+        selected_cell_list = list(selection.cell_generator(self.model.shape,
+                                                           self.table))
+
+        res_gen = (code_array[key] for key in selected_cell_list
+                   if code_array(key))
+        sum_list = list(filter(None, res_gen))
+
+        msg_tpl = "     " + "     ".join(["Σ={}", "max={}", "min={}"])
+        msg = f"Selection: {len(selected_cell_list)} cells"
+        if sum_list:
+            try:
+                msg += msg_tpl.format(sum(sum_list), max(sum_list),
+                                      min(sum_list))
+            except Exception:
+                pass
+
+        self.main_window.statusBar().showMessage(msg)
 
     def on_row_resized(self, row: int, old_height: float, new_height: float):
         """Row resized event handler
 
         :param row: Row that is resized
         :param old_height: Row height before resizing
         :param new_height: Row height after resizing
@@ -2298,14 +2322,18 @@
         if matplotlib is None:
             # matplotlib is not installed
             return
 
         key = index.row(), index.column(), self.grid.table
         figure = self.code_array[key]
 
+        if isinstance(figure, bytes) or isinstance(figure, str):
+            # We try rendering the content as SVG
+            return self._render_svg(painter, rect, index, figure)
+
         if not isinstance(figure, matplotlib.figure.Figure):
             return
 
         # Save SVG in a fake file object.
         with BytesIO() as filelike:
             try:
                 figure.savefig(filelike, format="svg", bbox_inches="tight")
```

### Comparing `pyspread-2.1.1/pyspread/grid_renderer.py` & `pyspread-2.2/pyspread/grid_renderer.py`

 * *Files 9% similar despite different names*

```diff
@@ -37,16 +37,18 @@
 try:
     from dataclasses import dataclass
 except ImportError:
     from pyspread.lib.dataclasses import dataclass  # Python 3.6 compatibility
 from typing import List, Tuple
 
 from PyQt5.QtCore import Qt, QModelIndex, QRectF, QPointF
-from PyQt5.QtGui import (QBrush, QColor, QPainter, QPalette, QPen,
+from PyQt5.QtGui import (QBrush, QPainter, QPalette, QPen,
                          QPainterPath, QPolygonF, QPainterPathStroker)
+
+from PyQt5.QtGui import QColor as __QColor
 from PyQt5.QtWidgets import QTableView, QStyleOptionViewItem
 
 
 @contextmanager
 def painter_save(painter: QPainter):
     """Context manager saving and restoring painter state
 
@@ -107,39 +109,49 @@
             painter.translate(-center_x, -center_y)
         elif angle in (90, 270):
             painter.translate(-center_y, -center_x)
             rect = QRectF(rect.y(), rect.x(), rect.height(), rect.width())
         yield rect
 
 
+class QColor(__QColor):
+    """Hashable QColor"""
+
+    def __hash__(self):
+        return self.rgba()
+
+
 class GridCellNavigator:
     """Find neighbors of a cell"""
 
     def __init__(self, grid: QTableView, key: Tuple[int, int, int]):
         """
         :param grid: The main grid widget
         :param key: Key of cell fow which neighbors are identified
 
         """
 
         self.grid = grid
         self.code_array = grid.model.code_array
         self.row, self.column, self.table = self.key = key
 
+        self.borderwidth_bottom_cache = grid.borderwidth_bottom_cache
+        self.borderwidth_right_cache = grid.borderwidth_right_cache
+
     @property
     def borderwidth_bottom(self) -> float:
         """Width of bottom border line"""
 
-        return self.code_array.cell_attributes[self.key].borderwidth_bottom
+        return self.borderwidth_bottom_cache[self.key]
 
     @property
     def borderwidth_right(self) -> float:
         """Width of right border line"""
 
-        return self.code_array.cell_attributes[self.key].borderwidth_right
+        return self.borderwidth_right_cache[self.key]
 
     @property
     def border_color_bottom(self) -> QColor:
         """Color of bottom border line"""
 
         return self.code_array.cell_attributes[self.key].bordercolor_bottom
 
@@ -151,83 +163,83 @@
 
     @property
     def merge_area(self) -> Tuple[int, int, int, int]:
         """Merge area of the key cell"""
 
         return self.code_array.cell_attributes[self.key].merge_area
 
-    def _merging_key(self, key: Tuple[int, int, int]) -> Tuple[int, int, int]:
+    def merging_key(self, key: Tuple[int, int, int]) -> Tuple[int, int, int]:
         """Merging cell if cell is merged else cell key
 
         :param key: Key of cell that is checked for being merged
 
         """
 
         merging_key = self.code_array.cell_attributes.get_merging_cell(key)
         return key if merging_key is None else merging_key
 
     def above_keys(self) -> List[Tuple[int, int, int]]:
         """Key list of neighboring cells above the key cell"""
 
         merge_area = self.merge_area
         if merge_area is None:
-            return [self._merging_key((self.row - 1, self.column, self.table))]
+            return [self.merging_key((self.row - 1, self.column, self.table))]
         _, left, _, right = merge_area
-        return [self._merging_key((self.row - 1, col, self.table))
+        return [self.merging_key((self.row - 1, col, self.table))
                 for col in range(left, right + 1)]
 
     def below_keys(self) -> List[Tuple[int, int, int]]:
         """Key list of neighboring cells below the key cell"""
 
         merge_area = self.merge_area
         if merge_area is None:
-            return [self._merging_key((self.row + 1, self.column, self.table))]
+            return [self.merging_key((self.row + 1, self.column, self.table))]
         _, left, _, right = merge_area
-        return [self._merging_key((self.row + 1, col, self.table))
+        return [self.merging_key((self.row + 1, col, self.table))
                 for col in range(left, right + 1)]
 
     def left_keys(self) -> List[Tuple[int, int, int]]:
         """Key list of neighboring cells left of the key cell"""
 
         merge_area = self.merge_area
         if merge_area is None:
-            return [self._merging_key((self.row, self.column - 1, self.table))]
+            return [self.merging_key((self.row, self.column - 1, self.table))]
         top, _, bottom, _ = merge_area
-        return [self._merging_key((row, self.column - 1, self.table))
+        return [self.merging_key((row, self.column - 1, self.table))
                 for row in range(top, bottom + 1)]
 
     def right_keys(self) -> List[Tuple[int, int, int]]:
         """Key list of neighboring cells right of the key cell"""
 
         merge_area = self.merge_area
         if merge_area is None:
-            return [self._merging_key((self.row, self.column + 1, self.table))]
+            return [self.merging_key((self.row, self.column + 1, self.table))]
         top, _, bottom, _ = merge_area
-        return [self._merging_key((row, self.column + 1, self.table))
+        return [self.merging_key((row, self.column + 1, self.table))
                 for row in range(top, bottom + 1)]
 
     def above_left_key(self) -> Tuple[int, int, int]:
         """Key of neighboring cell above left of the key cell"""
 
-        return self._merging_key((self.row - 1, self.column - 1, self.table))
+        return self.merging_key((self.row - 1, self.column - 1, self.table))
 
     def above_right_key(self) -> Tuple[int, int, int]:
         """Key of neighboring cell above right of the key cell"""
 
-        return self._merging_key((self.row - 1, self.column + 1, self.table))
+        return self.merging_key((self.row - 1, self.column + 1, self.table))
 
     def below_left_key(self) -> Tuple[int, int, int]:
         """Key of neighboring cell below left of the key cell"""
 
-        return self._merging_key((self.row + 1, self.column - 1, self.table))
+        return self.merging_key((self.row + 1, self.column - 1, self.table))
 
     def below_right_key(self) -> Tuple[int, int, int]:
         """Key of neighboring cell below right of the key cell"""
 
-        return self._merging_key((self.row + 1, self.column + 1, self.table))
+        return self.merging_key((self.row + 1, self.column + 1, self.table))
 
 
 @dataclass
 class EdgeBorders:
     """Holds border data for an edge and provides effective edge properties"""
 
     left_width: float
@@ -241,14 +253,16 @@
     bottom_color: QColor
 
     left_x: float
     right_x: float
     top_y: float
     bottom_y: float
 
+    _color_cache = None
+
     @property
     def _border_widths(self) -> Tuple[float, float, float, float]:
         """Tuple of border widths in order left, right, top, bottom"""
 
         return (self.left_width, self.right_width,
                 self.top_width, self.bottom_width)
 
@@ -271,87 +285,164 @@
 
         return max(self.left_width, self.right_width)
 
     @property
     def color(self) -> QColor:
         """Edge color, i.e. darkest color of thickest edge border"""
 
+        if self._color_cache is not None:
+            return self._color_cache
+
         max_border_width = max(self.width, self.height)
         colors = []
         for width, color in zip(self._border_widths, self._border_colors):
             if width == max_border_width:
                 colors.append(color)
         colors.sort(key=lambda color: color.lightnessF())
+        color = colors[0]
 
-        return colors[0]
+        self._color_cache = color
+
+        return color
 
 
 class CellEdgeRenderer:
     """Paints cell edges"""
 
+    intersection_cache = {}
+
     def __init__(self, painter: QPainter, center: QPointF,
-                 borders: EdgeBorders, clip_path: QPainterPath, zoom: float):
+                 borders: EdgeBorders, rect: QRectF, clip_path: QPainterPath,
+                 zoom: float):
         """
 
         Borders are provided by EdgeBorders in order: left, right, top, bottom
 
         :param painter: Painter with which edge is drawn
         :param center: Edge center
         :param borders: Border widths and colors
-        :param clip_path: Clip rectangle that is requuired for QtSVG clipping
+        :param rect: Rect of the clip_path
+        :param clip_path: Clip rectangle that is required for QtSVG clipping
         :param zoom: Current zoom level
 
         """
 
         self.painter = painter
         self.center = center
         self.borders = borders
+        self.rect = rect
         self.clip_path = clip_path
         self.zoom = zoom
 
     def paint(self):
         """Paints the edge"""
 
         if not self.borders.width or not self.borders.height:
             return  # Invisible edge
 
         x, y = self.center.x(), self.center.y()
         width = self.borders.width * self.zoom
         height = self.borders.height * self.zoom
 
-        rect = QRectF(x-width/2, y-height/2, width, height)
-
-        rect_path = QPainterPath()  # Required for clipping in SVG export
-        rect_path.addRect(rect)
+        cache_key = (self.rect.x(), self.rect.y(),
+                     self.rect.width(), self.rect.height(),
+                     x, y, width, height)
 
         color = self.borders.color
-
         self.painter.setPen(QPen(Qt.NoPen))
         self.painter.setBrush(QBrush(color))
 
-        self.painter.drawPath(self.clip_path.intersected(rect_path))
+        try:
+            intersection = self.intersection_cache[cache_key]
+        except KeyError:
+            rect = QRectF(x-width/2, y-height/2, width, height)
+            rect_path = QPainterPath()  # Required for clipping in SVG export
+            rect_path.addRect(rect)
+
+            intersection = self.clip_path.intersected(rect_path)
+
+            self.intersection_cache[cache_key] = intersection
+
+        self.painter.drawPath(intersection)
         self.painter.setPen(QPen(Qt.SolidLine))
 
 
 class QColorCache(dict):
     """QColor cache that returns default color for None"""
 
     def __init__(self, grid, *args, **kwargs):
         self.grid = grid
         super().__init__(*args, **kwargs)
 
     def __missing__(self, key):
         if key is None:
-            self[key] = qcolor = self.grid.palette().color(QPalette.Mid)
+            qcolor = QColor(self.grid.palette().color(QPalette.Mid))
         else:
-            self[key] = qcolor = QColor(*key)
+            qcolor = QColor(*key)
+
+        self[key] = qcolor
 
         return qcolor
 
 
+class BorderWidthBottomCache(dict):
+    """BorderWidthBottom cache"""
+
+    def __init__(self, grid, *args, **kwargs):
+        self.grid = grid
+        self.cell_attributes = grid.model.code_array.cell_attributes
+
+        super().__init__(*args, **kwargs)
+
+    def __missing__(self, key):
+        borderwidth_bottom = self.cell_attributes[key].borderwidth_bottom
+        self[key] = borderwidth_bottom
+
+        return borderwidth_bottom
+
+
+class BorderWidthRightCache(BorderWidthBottomCache):
+    """BorderWidthRight cache"""
+
+    def __missing__(self, key):
+        borderwidth_right = self.cell_attributes[key].borderwidth_right
+        self[key] = borderwidth_right
+
+        return borderwidth_right
+
+
+class EdgeBordersCache(dict):
+    """Cache of all EdgeBorders objects"""
+
+    def __missing__(self, key):
+        self[key] = edge_border = EdgeBorders(*key)
+
+        return edge_border
+
+
+class BorderColorBottomCache(BorderWidthBottomCache):
+    """BorderColorBottomCache cache"""
+
+    def __missing__(self, key):
+        border_color_bottom = self.cell_attributes[key].border_color_bottom
+        self[key] = border_color_bottom
+
+        return border_color_bottom
+
+
+class BorderColorRightCache(BorderWidthBottomCache):
+    """BorderColorBottomCache cache"""
+
+    def __missing__(self, key):
+        border_color_right = self.cell_attributes[key].border_color_right
+        self[key] = border_color_right
+
+        return border_color_right
+
+
 class CellRenderer:
     """Paints cells
 
     Cell rendering governs the area of a cell inside its borders.
     It is done in a  vector oriented way.
     Therefore, the following conventions shall apply:
      * Cell borders of width 1 shall be painted so that they appear only in the
@@ -360,50 +451,57 @@
      * Cell borders that are thicker than 1 are painted on all borders.
      * At the edges, borders are painted in the following order:
         1. Thin borders are painted first
         2. If border width is equal, lighter colors are painted first
 
     """
 
+    _pen_cache = {}
+
     def __init__(self, grid: QTableView, painter: QPainter,
                  option: QStyleOptionViewItem, index: QModelIndex):
         """
         :param grid: The main grid widget
         :param painter: Painter with which borders are drawn
         :param option: Style option for rendering
         :param index: Index of cell to be rendered
         """
 
         self.grid = grid
         self.painter = painter
         self.option = option
         self.index = index
 
+        self.painter.setRenderHint(QPainter.LosslessImageRendering, True)
+        self.painter.setRenderHint(QPainter.SmoothPixmapTransform, True)
+
         self.cell_attributes = grid.model.code_array.cell_attributes
         self.key = index.row(), index.column(), self.grid.table
 
         self.cell_nav = GridCellNavigator(grid, self.key)
 
-        self.qcolor_cache = self.grid.qcolor_cache
+        self.qcolor_cache = grid.qcolor_cache
+        self.borderwidth_bottom_cache = grid.borderwidth_bottom_cache
+        self.borderwidth_right_cache = grid.borderwidth_right_cache
 
     def inner_rect(self, rect: QRectF) -> QRectF:
         """Returns inner rect that is shrunk by border widths
 
         For merged cells, minimum top/left border widths are taken into account
 
         :param rect: Cell rect to be shrunk
 
         """
 
         above_keys = self.cell_nav.above_keys()
         left_keys = self.cell_nav.left_keys()
 
-        width_top = min(self.cell_attributes[above_key].borderwidth_bottom
+        width_top = min(self.borderwidth_bottom_cache[above_key]
                         for above_key in above_keys)
-        width_left = min(self.cell_attributes[left_key].borderwidth_right
+        width_left = min(self.borderwidth_right_cache[left_key]
                          for left_key in left_keys)
         width_bottom = self.cell_nav.borderwidth_bottom
         width_right = self.cell_nav.borderwidth_right
 
         width_top *= self.grid.zoom
         width_left *= self.grid.zoom
         width_bottom *= self.grid.zoom
@@ -423,87 +521,117 @@
         """
 
         with painter_zoom(self.painter, self.grid.zoom, rect) as zrect:
             self.grid.delegate.paint_(self.painter, zrect, self.option,
                                       self.index)
 
     def _get_border_pen(self, width, zoom):
-        """Gets zoomed border pen
+        """Gets zoomed border pen, white, fully transparent
 
         :param width: Unzoomed line width
         :param zoom: Current zoom level of grid
 
         """
 
+        try:
+            return self._pen_cache[(width, zoom)]
+        except KeyError:
+            pass
+
         zoomed_width = max(1, width * zoom)
 
-        return QPen(QColor(255, 255, 255, 0), zoomed_width,
-                    Qt.SolidLine, Qt.FlatCap, Qt.MiterJoin)
+        pen = QPen(QColor(255, 255, 255, 0), zoomed_width,
+                   Qt.SolidLine, Qt.FlatCap, Qt.MiterJoin)
+        self._pen_cache[(width, zoom)] = pen
+
+        return pen
+
+    def _draw_line(self, point1: QPointF, point2: QPointF, width: float,
+                   color: QColor, clip_path: QPainterPath):
+        """Draws line
+
+        Uses drawLine for screen painting and QPainterPathStroker for
+        svg painting.
+
+        :param point1: Start point of line
+        :param point2: End point of line
+        :param width: Line width
+        :param color: Line color
+        :param clip_path: Clip rectangle
+
+        """
+
+        zoom = self.grid.zoom
+        alpha = max(0, round(255 - 255 * width * zoom))
+
+        if width * zoom > 1.01:
+            self.painter.setRenderHint(QPainter.Antialiasing, True)
+
+        screen_painting = self.grid.main_window.print_area is None
+
+        if screen_painting:
+            # Rendering for the screen
+            pen = QPen(color)
+            pen.setWidthF(width * zoom)
+            self.painter.setPen(pen)
+            self.painter.drawLine(point1, point2)
+        else:
+            # Rendering for the printer
+            pen = self._get_border_pen(width, zoom)
+
+            line_polygon = QPolygonF((point1, point2))
+            line_path = QPainterPath()
+            line_path.addPolygon(line_polygon)
+
+            stroker = QPainterPathStroker(pen)
+            stroked_path = stroker.createStroke(line_path)
+
+            self.painter.setPen(QPen(QColor(255, 255, 255, alpha)))
+            self.painter.setBrush(QBrush(color))
+            self.painter.drawPath(clip_path.intersected(stroked_path))
+
+        self.painter.setRenderHint(QPainter.Antialiasing, False)
 
     def paint_bottom_border(self, rect: QRectF, clip_path: QPainterPath):
         """Paint bottom border of cell
 
         :param rect: Cell rect of the cell to be painted
         :param clip_path: Clip rectangle that is required for QtSVG clipping
 
         """
 
         if not self.cell_nav.borderwidth_bottom:
             return
 
-        line_color = self.qcolor_cache[self.cell_nav.border_color_bottom]
-
         point1 = QPointF(rect.x(), rect.y() + rect.height())
         point2 = QPointF(rect.x() + rect.width(), rect.y() + rect.height())
-        line_polygon = QPolygonF((point1, point2))
-        line_path = QPainterPath()
-        line_path.addPolygon(line_polygon)
-
-        pen = self._get_border_pen(self.cell_nav.borderwidth_bottom,
-                                   self.grid.zoom)
-        stroker = QPainterPathStroker(pen)
-        stroked_path = stroker.createStroke(line_path)
-
-        alpha = max(0, round(255 - 255 * self.cell_nav.borderwidth_bottom *
-                             self.grid.zoom))
-
-        self.painter.setPen(QPen(QColor(255, 255, 255, alpha)))
-        self.painter.setBrush(QBrush(line_color))
-        self.painter.drawPath(clip_path.intersected(stroked_path))
+
+        width = self.cell_nav.borderwidth_bottom
+        color = self.qcolor_cache[self.cell_nav.border_color_bottom]
+
+        self._draw_line(point1, point2, width, color, clip_path)
 
     def paint_right_border(self, rect: QRectF, clip_path: QPainterPath):
         """Paint right border of cell
 
         :param rect: Cell rect of the cell to be painted
         :param clip_path: Clip rectangle that is requuired for QtSVG clipping
 
         """
 
         if not self.cell_nav.borderwidth_right:
             return
 
-        line_color = self.qcolor_cache[self.cell_nav.border_color_right]
-
         point1 = QPointF(rect.x() + rect.width(), rect.y())
         point2 = QPointF(rect.x() + rect.width(), rect.y() + rect.height())
-        line_polygon = QPolygonF((point1, point2))
-        line_path = QPainterPath()
-        line_path.addPolygon(line_polygon)
-
-        pen = self._get_border_pen(self.cell_nav.borderwidth_right,
-                                   self.grid.zoom)
-        stroker = QPainterPathStroker(pen)
-        stroked_path = stroker.createStroke(line_path)
-
-        alpha = max(0, round(255 - 255 * self.cell_nav.borderwidth_bottom *
-                             self.grid.zoom))
-
-        self.painter.setPen(QPen(QColor(255, 255, 255, alpha)))
-        self.painter.setBrush(QBrush(line_color))
-        self.painter.drawPath(clip_path.intersected(stroked_path))
+
+        width = self.cell_nav.borderwidth_right
+        color = self.qcolor_cache[self.cell_nav.border_color_right]
+
+        self._draw_line(point1, point2, width, color, clip_path)
 
     def paint_above_borders(self, rect: QRectF, clip_path: QPainterPath):
         """Paint lower borders of all above cells
 
         :param rect: Cell rect of below cell, in which the borders are painted
         :param clip_path: Clip rectangle that is requuired for QtSVG clipping
 
@@ -520,34 +648,21 @@
             else:
                 _, left, _, right = merge_area
                 columns = list(range(left, right + 1))
             above_rect_x = self.grid.columnViewportPosition(columns[0])
             above_rect_width = sum(self.grid.columnWidth(column)
                                    for column in columns)
 
-            line_color = self.qcolor_cache[above_cell_nav.border_color_bottom]
-
             point1 = QPointF(above_rect_x, rect.y())
             point2 = QPointF(above_rect_x + above_rect_width, rect.y())
-            line_polygon = QPolygonF((point1, point2))
-            line_path = QPainterPath()
-            line_path.addPolygon(line_polygon)
 
-            pen = self._get_border_pen(above_cell_nav.borderwidth_bottom,
-                                       self.grid.zoom)
-            stroker = QPainterPathStroker(pen)
-            stroked_path = stroker.createStroke(line_path)
-
-            alpha = max(0, round(255 - 255 *
-                                 above_cell_nav.borderwidth_bottom *
-                                 self.grid.zoom))
+            width = above_cell_nav.borderwidth_bottom
+            color = self.qcolor_cache[above_cell_nav.border_color_bottom]
 
-            self.painter.setPen(QPen(QColor(255, 255, 255, alpha)))
-            self.painter.setBrush(QBrush(line_color))
-            self.painter.drawPath(clip_path.intersected(stroked_path))
+            self._draw_line(point1, point2, width, color, clip_path)
 
     def paint_left_borders(self, rect: QRectF, clip_path: QPainterPath):
         """Paint right borders of all left cells
 
         :param rect: Cell rect of right cell, in which the borders are painted
         :param clip_path: Clip rectangle that is requuired for QtSVG clipping
 
@@ -563,34 +678,21 @@
                 rows = [left_key[0]]
             else:
                 top, _, bottom, _ = merge_area
                 rows = list(range(top, bottom + 1))
             left_rect_y = self.grid.rowViewportPosition(rows[0])
             left_rect_height = sum(self.grid.rowHeight(row) for row in rows)
 
-            line_color = self.qcolor_cache[left_cell_nav.border_color_right]
-
             point1 = QPointF(rect.x(), left_rect_y)
             point2 = QPointF(rect.x(), left_rect_y + left_rect_height)
-            line_polygon = QPolygonF((point1, point2))
-            line_path = QPainterPath()
-            line_path.addPolygon(line_polygon)
-
-            pen = self._get_border_pen(left_cell_nav.borderwidth_right,
-                                       self.grid.zoom)
-            stroker = QPainterPathStroker(pen)
-            stroked_path = stroker.createStroke(line_path)
 
-            alpha = max(0, round(255 - 255 *
-                                 left_cell_nav.borderwidth_right *
-                                 self.grid.zoom))
+            width = left_cell_nav.borderwidth_right
+            color = self.qcolor_cache[left_cell_nav.border_color_right]
 
-            self.painter.setPen(QPen(QColor(255, 255, 255, alpha)))
-            self.painter.setBrush(QBrush(line_color))
-            self.painter.drawPath(clip_path.intersected(stroked_path))
+            self._draw_line(point1, point2, width, color, clip_path)
 
     def paint_top_left_edge(self, rect: QRectF, clip_path: QPainterPath):
         """Paints top left edge of the cell
 
         :param rect: Cell rect of cell, for which the edge is painted
         :param clip_path: Clip rectangle that is requuired for QtSVG clipping
 
@@ -623,20 +725,22 @@
         bottom_color = self.qcolor_cache[left_cell_nav.border_color_right]
 
         left_x = rect.x() - rect.width()
         right_x = rect.x()
         top_y = rect.y() - rect.height()
         bottom_y = rect.y()
 
-        borders = EdgeBorders(left_width, right_width, top_width, bottom_width,
-                              left_color, right_color, top_color, bottom_color,
-                              left_x, right_x, top_y, bottom_y)
+        key = (left_width, right_width, top_width, bottom_width,
+               left_color, right_color, top_color, bottom_color,
+               left_x, right_x, top_y, bottom_y)
+
+        borders = self.grid.edge_borders_cache[key]
 
-        renderer = CellEdgeRenderer(self.painter, center, borders, clip_path,
-                                    self.grid.zoom)
+        renderer = CellEdgeRenderer(self.painter, center, borders, rect,
+                                    clip_path, self.grid.zoom)
         renderer.paint()
 
     def paint_top_right_edge(self, rect: QRectF, clip_path: QPainterPath):
         """Paints top right edge of the cell
 
         :param rect: Cell rect of cell, for which the edge is painted
         :param clip_path: Clip rectangle that is requuired for QtSVG clipping
@@ -668,20 +772,22 @@
         bottom_color = self.qcolor_cache[self.cell_nav.border_color_right]
 
         left_x = rect.x() + rect.width()
         right_x = rect.x() + 2 * rect.width()
         top_y = rect.y() - rect.height()
         bottom_y = rect.y()
 
-        borders = EdgeBorders(left_width, right_width, top_width, bottom_width,
-                              left_color, right_color, top_color, bottom_color,
-                              left_x, right_x, top_y, bottom_y)
+        key = (left_width, right_width, top_width, bottom_width,
+               left_color, right_color, top_color, bottom_color,
+               left_x, right_x, top_y, bottom_y)
 
-        renderer = CellEdgeRenderer(self.painter, center, borders, clip_path,
-                                    self.grid.zoom)
+        borders = self.grid.edge_borders_cache[key]
+
+        renderer = CellEdgeRenderer(self.painter, center, borders, rect,
+                                    clip_path, self.grid.zoom)
         renderer.paint()
 
     def paint_bottom_left_edge(self, rect: QRectF, clip_path: QPainterPath):
         """Paints bottom left edge of the cell
 
         :param rect: Cell rect of cell, for which the edge is painted
         :param clip_path: Clip rectangle that is requuired for QtSVG clipping
@@ -714,20 +820,22 @@
             self.qcolor_cache[bottom_left_cell_nav.border_color_right]
 
         left_x = rect.x() - rect.width()
         right_x = rect.x()
         top_y = rect.y() + rect.height()
         bottom_y = rect.y() + 2 * rect.height()
 
-        borders = EdgeBorders(left_width, right_width, top_width, bottom_width,
-                              left_color, right_color, top_color, bottom_color,
-                              left_x, right_x, top_y, bottom_y)
+        key = (left_width, right_width, top_width, bottom_width,
+               left_color, right_color, top_color, bottom_color,
+               left_x, right_x, top_y, bottom_y)
+
+        borders = self.grid.edge_borders_cache[key]
 
-        renderer = CellEdgeRenderer(self.painter, center, borders, clip_path,
-                                    self.grid.zoom)
+        renderer = CellEdgeRenderer(self.painter, center, borders, rect,
+                                    clip_path, self.grid.zoom)
         renderer.paint()
 
     def paint_bottom_right_edge(self, rect: QRectF, clip_path: QPainterPath):
         """Paints bottom right edge of the cell
 
         :param rect: Cell rect of cell, for which the edge is painted
         :param clip_path: Clip rectangle that is requuired for QtSVG clipping
@@ -759,20 +867,22 @@
         bottom_color = self.qcolor_cache[bottom_cell_nav.border_color_right]
 
         left_x = rect.x() + rect.width()
         right_x = rect.x() + 2 * rect.width()
         top_y = rect.y() + rect.height()
         bottom_y = rect.y() + 2 * rect.height()
 
-        borders = EdgeBorders(left_width, right_width, top_width, bottom_width,
-                              left_color, right_color, top_color, bottom_color,
-                              left_x, right_x, top_y, bottom_y)
+        key = (left_width, right_width, top_width, bottom_width,
+               left_color, right_color, top_color, bottom_color,
+               left_x, right_x, top_y, bottom_y)
+
+        borders = self.grid.edge_borders_cache[key]
 
-        renderer = CellEdgeRenderer(self.painter, center, borders, clip_path,
-                                    self.grid.zoom)
+        renderer = CellEdgeRenderer(self.painter, center, borders, rect,
+                                    clip_path, self.grid.zoom)
         renderer.paint()
 
     def paint_borders(self, rect):
         """Paint cell borders"""
 
         clip_path = QPainterPath()  # Required for clipping in SVG export
         clip_path.addRect(rect)
```

### Comparing `pyspread-2.1.1/pyspread/icons.py` & `pyspread-2.2/pyspread/icons.py`

 * *Files 14% similar despite different names*

```diff
@@ -179,14 +179,30 @@
     chart_histogram_1_1 = CHARTS_PATH / 'chart_histogram_1_1.svg'
     chart_histogram_1_4 = CHARTS_PATH / 'chart_histogram_1_4.svg'
     chart_scatterhist_1_1 = CHARTS_PATH/'chart_scatterhist_1_1.svg'
     chart_matrix_1_1 = CHARTS_PATH / 'chart_matrix_1_1.svg'
     chart_contour_1_2 = CHARTS_PATH / 'chart_contour_1_2.svg'
     chart_surface_2_1 = CHARTS_PATH / 'chart_surface_2_1.svg'
 
+    chart_plotnine_geom_bar_1_1 = \
+        CHARTS_PATH / 'chart_plotnine_geom_bar_1_1.svg'
+
+    chart_r_graphics_barplot_1_1 = \
+        CHARTS_PATH / 'chart_r_graphics_barplot_1_1.svg'
+    chart_r_ggplot2_geom_boxplot_1_2 = \
+        CHARTS_PATH / 'chart_r_ggplot2_geom_boxplot_1_2.svg'
+    chart_r_ggplot2_geom_point_1_1 = \
+        CHARTS_PATH / 'chart_r_ggplot2_geom_point_1_1.svg'
+    chart_r_lattice_xyplot_1_1 = \
+        CHARTS_PATH / 'chart_r_lattice_xyplot_1_1.svg'
+    chart_r_ggplot2_geom_density2d_1_2 = \
+        CHARTS_PATH / 'chart_r_ggplot2_geom_density2d_1_2.svg'
+    chart_r_lattice_wireframe_2_1 =\
+        CHARTS_PATH / 'chart_r_lattice_wireframe_2_1.svg'
+
 
 class IconConverter(type):
     """Meta class that provides QIcons for IconPaths icons"""
 
     def __getattr__(cls, name: str) -> QIcon:
         """Provides QIcons for icon names
```

### Comparing `pyspread-2.1.1/pyspread/installer.py` & `pyspread-2.2/pyspread/installer.py`

 * *Files 4% similar despite different names*

```diff
@@ -123,14 +123,20 @@
     Module(name="python-dateutil",
            description="The dateutil module provides powerful extensions to "
                        "the standard datetime module, available in Python.",
            required_version=version.parse("2.7.0")),
     Module(name="py-moneyed",
            description="Import money from csv using the py-moneyed module",
            required_version=version.parse("2.0")),
+    Module(name="matplotlib",
+           description="Create charts",
+           required_version=version.parse("3.4")),
+    Module(name="plotnine",
+           description="Grammar of graphics for simpler R ggplot2 charts",
+           required_version=version.parse("0.8")),
 ]
 
 DEPENDENCIES = REQUIRED_DEPENDENCIES + OPTIONAL_DEPENDENCIES
 
 PIP_MODULE = Module(name="pip", description="pip installer",
                     required_version=version.parse("17.0"))
```

### Comparing `pyspread-2.1.1/pyspread/interfaces/pys.py` & `pyspread-2.2/pyspread/interfaces/pys.py`

 * *Files 0% similar despite different names*

```diff
@@ -410,16 +410,17 @@
                 key = ast.literal_eval(ele)
 
             else:
                 # Even cols are values
                 value = ast.literal_eval(ele)
                 attr_dict[key] = value
 
-        attr = CellAttribute(selection, tab, attr_dict)
-        self.code_array.cell_attributes.append(attr)
+        if attr_dict:  # Ignore empty attribute settings
+            attr = CellAttribute(selection, tab, attr_dict)
+            self.code_array.cell_attributes.append(attr)
 
     def _pys2row_heights(self, line: str):
         """Updates row_heights in code_array
 
         :param line: Pys file line to be parsed
 
         """
@@ -567,14 +568,17 @@
                (selection, tab) == purged_cell_attributes_keys[-1]:
                 purged_cell_attributes[-1][2].update(attr_dict)
             else:
                 purged_cell_attributes_keys.append((selection, tab))
                 purged_cell_attributes.append([selection, tab, attr_dict])
 
         for selection, tab, attr_dict in purged_cell_attributes:
+            if not attr_dict:
+                continue
+
             sel_list = [selection.block_tl, selection.block_br,
                         selection.rows, selection.columns, selection.cells]
 
             tab_list = [tab]
 
             attr_dict_list = []
             for key in attr_dict:
```

### Comparing `pyspread-2.1.1/pyspread/lib/attrdict.py` & `pyspread-2.2/pyspread/lib/attrdict.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/lib/charts.py` & `pyspread-2.2/pyspread/lib/charts.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/lib/csv.py` & `pyspread-2.2/pyspread/lib/csv.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/lib/dataclasses.py` & `pyspread-2.2/pyspread/lib/dataclasses.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/lib/exception_handling.py` & `pyspread-2.2/pyspread/lib/exception_handling.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/lib/file_helpers.py` & `pyspread-2.2/pyspread/lib/file_helpers.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/lib/hashing.py` & `pyspread-2.2/pyspread/lib/hashing.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/lib/packaging/_structures.py` & `pyspread-2.2/pyspread/lib/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/lib/packaging/_typing.py` & `pyspread-2.2/pyspread/lib/packaging/_typing.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/lib/packaging/version.py` & `pyspread-2.2/pyspread/lib/packaging/version.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/lib/qimage2ndarray.py` & `pyspread-2.2/pyspread/lib/qimage2ndarray.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/lib/qimage_svg.py` & `pyspread-2.2/pyspread/lib/qimage_svg.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/lib/selection.py` & `pyspread-2.2/pyspread/lib/selection.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/lib/spelltextedit.py` & `pyspread-2.2/pyspread/lib/spelltextedit.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/lib/string_helpers.py` & `pyspread-2.2/pyspread/lib/string_helpers.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/lib/test/compat.py` & `pyspread-2.2/pyspread/lib/test/compat.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/lib/test/test_array2qimage.py` & `pyspread-2.2/pyspread/lib/test/test_array2qimage.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/lib/test/test_csv.py` & `pyspread-2.2/pyspread/lib/test/test_csv.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/lib/test/test_file_helpers.py` & `pyspread-2.2/pyspread/lib/test/test_file_helpers.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/lib/test/test_hashing.py` & `pyspread-2.2/pyspread/lib/test/test_hashing.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/lib/test/test_qimageview.py` & `pyspread-2.2/pyspread/lib/test/test_qimageview.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/lib/test/test_selection.py` & `pyspread-2.2/pyspread/lib/test/test_selection.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/lib/test/test_string_helpers.py` & `pyspread-2.2/pyspread/lib/test/test_string_helpers.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/lib/test/valid3.csv` & `pyspread-2.2/pyspread/lib/test/valid3.csv`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/lib/typechecks.py` & `pyspread-2.2/pyspread/lib/typechecks.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/main_window.py` & `pyspread-2.2/pyspread/main_window.py`

 * *Files 1% similar despite different names*

```diff
@@ -408,14 +408,16 @@
             return
 
         # Create print dialog
         dialog = QPrintDialog(printer, self)
         if dialog.exec_() == QPrintDialog.Accepted:
             self.on_paint_request(printer)
 
+        self.print_area = None
+
     def on_preview(self):
         """Print preview event handler"""
 
         # Create printer
         printer = QPrinter(mode=QPrinter.HighResolution)
 
         # Get print area
@@ -426,14 +428,16 @@
 
         # Create print preview dialog
         dialog = PrintPreviewDialog(printer)
 
         dialog.paintRequested.connect(self.on_paint_request)
         dialog.exec_()
 
+        self.print_area = None
+
     def on_paint_request(self, printer: QPrinter):
         """Paints to printer
 
         :param printer: Target printer
 
         """
```

### Comparing `pyspread-2.1.1/pyspread/menus.py` & `pyspread-2.2/pyspread/menus.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/model/model.py` & `pyspread-2.2/pyspread/model/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -792,15 +792,15 @@
 
         :param key: Specifies the cell keys of the generator
 
         """
 
         for i, key_ele in enumerate(key):
 
-            # Get first element of key that is a slice
+            # Recursively replace first element of key that is a slice
             if isinstance(key_ele, slice):
                 slc_keys = range(*key_ele.indices(self.dict_grid.shape[i]))
                 key_list = list(key)
 
                 key_list[i] = None
 
                 has_subslice = any(isinstance(ele, slice) for ele in key_list)
@@ -1259,39 +1259,45 @@
                                      Union[int, slice]]) -> Any:
         """Returns _eval_cell
 
         :param key: Cell key for result retrieval (code if in safe mode)
 
         """
 
+        code = self(key)
+
+        if code is None:
+            return
+
+        # Cached cell handling
+
+        if repr(key) in self.result_cache:
+            return self.result_cache[repr(key)]
+
         if not any(isinstance(k, slice) for k in key):
             # Button cell handling
             if self.cell_attributes[key].button_cell is not False:
                 return
             # Frozen cell handling
             frozen_res = self.cell_attributes[key].frozen
             if frozen_res:
                 if repr(key) in self.frozen_cache:
                     return self.frozen_cache[repr(key)]
                 # Frozen cache is empty.
                 # Maybe we have a reload without the frozen cache
-                result = self._eval_cell(key, self(key))
+                result = self._eval_cell(key, code)
                 self.frozen_cache[repr(key)] = result
                 return result
 
         # Normal cell handling
 
-        if repr(key) in self.result_cache:
-            return self.result_cache[repr(key)]
-
-        elif self(key) is not None:
-            result = self._eval_cell(key, self(key))
-            self.result_cache[repr(key)] = result
+        result = self._eval_cell(key, code)
+        self.result_cache[repr(key)] = result
 
-            return result
+        return result
 
     def _make_nested_list(self, gen: Union[Iterable, Iterable[Iterable],
                                            Iterable[Iterable[Iterable]]]
                           ) -> Union[Sequence, Sequence[Sequence],
                                      Sequence[Sequence[Sequence]]]:
         """Makes nested list from generator for creating numpy.array"""
 
@@ -1323,15 +1329,15 @@
         env = globals().copy()
         env.update(env_dict)
 
         return env
 
     def exec_then_eval(self, code: str,
                        _globals: dict = None, _locals: dict = None):
-        """execs multuiline code and returns eval of last code line
+        """execs multiline code and returns eval of last code line
 
         :param code: Code to be executed / evaled
         :param _globals: Globals dict for code execution and eval
         :param _locals: Locals dict for code execution and eval
 
         """
```

### Comparing `pyspread-2.1.1/pyspread/model/test/test_model.py` & `pyspread-2.2/pyspread/model/test/test_model.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/panels.py` & `pyspread-2.2/pyspread/panels.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/pyspread.py` & `pyspread-2.2/pyspread/pyspread.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/settings.py` & `pyspread-2.2/pyspread/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,16 @@
 
 PYSPREAD_DIRNAME = abspath(join(dirname(__file__), ".."))
 PYSPREAD_PATH = Path(PYSPREAD_DIRNAME)
 DOC_PATH = PYSPREAD_PATH / "pyspread/share/doc"
 TUTORIAL_PATH = DOC_PATH / "tutorial"
 MANUAL_PATH = DOC_PATH / "manual"
 MPL_TEMPLATE_PATH = PYSPREAD_PATH / 'pyspread/share/templates/matplotlib'
+RPY2_TEMPLATE_PATH = PYSPREAD_PATH / 'pyspread/share/templates/rpy2'
+PLOT9_TEMPLATE_PATH = PYSPREAD_PATH / 'pyspread/share/templates/plotnine'
 ICON_PATH = PYSPREAD_PATH / 'pyspread/share/icons'
 ACTION_PATH = ICON_PATH / 'actions'
 STATUS_PATH = ICON_PATH / 'status'
 CHARTS_PATH = ICON_PATH / 'charts'
 WEB_URL = "https://pyspread.gitlab.io"  # Official Web page
 
 
@@ -65,15 +67,15 @@
 
     """Names of widgets with persistant states"""
 
     shape = 1000, 100, 3
     """Default shape of initial grid (rows, columns, tables)"""
 
     maxshape = 1000000, 100000, 100
-    """"Maximum shape of the grid"""
+    """Maximum shape of the grid"""
 
     changed_since_save = False
     """If `True` then File actions trigger a dialog"""
 
     last_file_input_path = Path.home()
     """Initial :class:`~pathlib.Path` for opening files"""
 
@@ -230,14 +232,15 @@
         settings.setValue("max_file_history", self.max_file_history)
         settings.value("file_history", [], 'QStringList')
         if self.file_history:
             settings.setValue("file_history", self.file_history)
         settings.setValue("timeout", self.timeout)
         settings.setValue("refresh_timeout", self.refresh_timeout)
         settings.setValue("signature_key", self.signature_key)
+        settings.setValue("show_statusbar_sum", self.show_statusbar_sum)
 
         # GUI state
         for widget_name in self.widget_names:
 
             if widget_name == "main_window":
                 widget = self.parent
             else:
@@ -267,14 +270,21 @@
                 settings.setValue("entry_line_isvisible", widget.isVisible())
 
         settings.sync()
 
     def restore(self):
         """Restores application state from QSettings"""
 
+        def qt_bool(value):
+            """Converts Qt setting string for bool into Python bool"""
+            if value == "true":
+                return True
+            else:
+                return False
+
         if self.reset_settings:
             return
 
         if system() == "Darwin":
             settings = QSettings(APP_NAME+".gitlab.io", APP_NAME)
         else:
             settings = QSettings(APP_NAME, APP_NAME)
@@ -298,14 +308,15 @@
         setting2attr("last_file_import_path")
         setting2attr("last_file_export_path")
         setting2attr("max_file_history", mapper=int)
         setting2attr("file_history")
         setting2attr("timeout", mapper=int)
         setting2attr("refresh_timeout", mapper=int)
         setting2attr("signature_key")
+        setting2attr("show_statusbar_sum", mapper=qt_bool)
 
         # GUI state
 
         for widget_name in self.widget_names:
             geometry_name = widget_name + '/geometry'
             widget_state_name = widget_name + '/windowState'
```

### Comparing `pyspread-2.1.1/pyspread/share/LICENSE` & `pyspread-2.2/pyspread/share/LICENSE`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/applications/io.gitlab.pyspread.pyspread.desktop` & `pyspread-2.2/pyspread/share/applications/io.gitlab.pyspread.pyspread.desktop`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/doc/manual/advanced_topics.md` & `pyspread-2.2/pyspread/share/doc/manual/advanced_topics.md`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/doc/manual/basic_concepts.md` & `pyspread-2.2/pyspread/share/doc/manual/basic_concepts.md`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/doc/manual/edit_menu.md` & `pyspread-2.2/pyspread/share/doc/manual/edit_menu.md`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/doc/manual/file_menu.md` & `pyspread-2.2/pyspread/share/doc/manual/file_menu.md`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/doc/manual/format_menu.md` & `pyspread-2.2/pyspread/share/doc/manual/format_menu.md`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/doc/manual/images/screenshot_approve_dialog.png` & `pyspread-2.2/pyspread/share/doc/manual/images/screenshot_approve_dialog.png`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/doc/manual/images/screenshot_chartdialog.png` & `pyspread-2.2/pyspread/share/doc/manual/images/screenshot_chartdialog.png`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/doc/manual/images/screenshot_csv_export.png` & `pyspread-2.2/pyspread/share/doc/manual/images/screenshot_csv_export.png`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/doc/manual/images/screenshot_csv_import.png` & `pyspread-2.2/pyspread/share/doc/manual/images/screenshot_csv_import.png`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/doc/manual/images/screenshot_find_dialog.png` & `pyspread-2.2/pyspread/share/doc/manual/images/screenshot_find_dialog.png`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/doc/manual/images/screenshot_macros.png` & `pyspread-2.2/pyspread/share/doc/manual/images/screenshot_macros.png`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/doc/manual/images/screenshot_main_window.png` & `pyspread-2.2/pyspread/share/doc/manual/images/screenshot_main_window.png`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/doc/manual/images/screenshot_new_dialog.png` & `pyspread-2.2/pyspread/share/doc/manual/images/screenshot_new_dialog.png`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/doc/manual/images/screenshot_paste_as.png` & `pyspread-2.2/pyspread/share/doc/manual/images/screenshot_paste_as.png`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/doc/manual/images/screenshot_preferences_dialog.png` & `pyspread-2.2/pyspread/share/doc/manual/images/screenshot_preferences_dialog.png`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/doc/manual/images/screenshot_print_preview_1.png` & `pyspread-2.2/pyspread/share/doc/manual/images/screenshot_print_preview_1.png`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/doc/manual/images/screenshot_print_preview_2.png` & `pyspread-2.2/pyspread/share/doc/manual/images/screenshot_print_preview_2.png`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/doc/manual/images/screenshot_replace_dialog.png` & `pyspread-2.2/pyspread/share/doc/manual/images/screenshot_replace_dialog.png`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/doc/manual/macro_menu.md` & `pyspread-2.2/pyspread/share/doc/manual/macro_menu.md`

 * *Files 22% similar despite different names*

```diff
@@ -24,12 +24,14 @@
 
 The preview is updated when pressing the `Apply` button. If an exception occurs of if no Figure object could be retrieved then an error message is displayed.
 
 Pressing the `Ok` button puts the code in the editor in the current cell and activates the matplotlib renderer.
 
 For further reference on how to create charts, the [matplotlib web site](https://matplotlib.org/users/index.html) is recommended.
 
+Starting from version 2.2, there is a second toolbar with [R](https://www.r-project.org/) charts. These comprise examples using [plotnine](https://plotnine.readthedocs.io/en/stable/) ([ggplot2](https://ggplot2.tidyverse.org/) based) charts as well as charts from [rpy2](https://rpy2.github.io/) using the [R](https://www.r-project.org/) modules [graphics](https://www.rdocumentation.org/packages/graphics), [ggplot2](https://ggplot2.tidyverse.org/) and [lattice](https://lattice.r-forge.r-project.org/). If the relevant R modules are not installed, the respective buttons are disabled.
+
 ### Note:
 
 With the upcoming Python 3 version of *pyspread* (i.e. v. 1.99.0+), the chart dialog has been completely rewritten.
 
 For easier transition from previous versions of *pyspread*, the special class `charts.ChartFigure` is provided. This class subclasses the matplotlib Figure class. The subclass takes matplotlib arguments and creates a figure in one step. It is recommended to replace code that uses this class.
```

### Comparing `pyspread-2.1.1/pyspread/share/doc/manual/overview.md` & `pyspread-2.2/pyspread/share/doc/manual/overview.md`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/doc/manual/view_menu.md` & `pyspread-2.2/pyspread/share/doc/manual/view_menu.md`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/doc/manual/workspace.md` & `pyspread-2.2/pyspread/share/doc/manual/workspace.md`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/doc/tutorial/images/Tutorial1.png` & `pyspread-2.2/pyspread/share/doc/tutorial/images/Tutorial1.png`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/doc/tutorial/images/Tutorial2.png` & `pyspread-2.2/pyspread/share/doc/tutorial/images/Tutorial2.png`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/doc/tutorial/images/Tutorial3.png` & `pyspread-2.2/pyspread/share/doc/tutorial/images/Tutorial3.png`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/doc/tutorial/images/Tutorial4.png` & `pyspread-2.2/pyspread/share/doc/tutorial/images/Tutorial4.png`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/doc/tutorial/tutorial.md` & `pyspread-2.2/pyspread/share/doc/tutorial/tutorial.md`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/examples/images and charts.pysu` & `pyspread-2.2/pyspread/share/examples/images and charts.pysu`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/examples/pivot.pysu` & `pyspread-2.2/pyspread/share/examples/pivot.pysu`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/examples/test_write.csv` & `pyspread-2.2/pyspread/share/examples/test_write.csv`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/examples/wagner_whitin.pysu` & `pyspread-2.2/pyspread/share/examples/wagner_whitin.pysu`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/document-approve.svg` & `pyspread-2.2/pyspread/share/icons/actions/document-approve.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/document-export.svg` & `pyspread-2.2/pyspread/share/icons/actions/document-export.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/document-import.svg` & `pyspread-2.2/pyspread/share/icons/actions/document-import.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/document-log-out.svg` & `pyspread-2.2/pyspread/share/icons/actions/document-log-out.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/document-new-gpg-key.svg` & `pyspread-2.2/pyspread/share/icons/actions/document-new-gpg-key.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/document-new.svg` & `pyspread-2.2/pyspread/share/icons/actions/document-new.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/document-open.svg` & `pyspread-2.2/pyspread/share/icons/actions/document-open.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/document-page-setup.svg` & `pyspread-2.2/pyspread/share/icons/actions/document-page-setup.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/document-print-preview.svg` & `pyspread-2.2/pyspread/share/icons/actions/document-print-preview.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/document-print.svg` & `pyspread-2.2/pyspread/share/icons/actions/document-print.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/document-properties.svg` & `pyspread-2.2/pyspread/share/icons/actions/document-properties.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/document-save-as.svg` & `pyspread-2.2/pyspread/share/icons/actions/document-save-as.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/document-save.svg` & `pyspread-2.2/pyspread/share/icons/actions/document-save.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/edit-clear.svg` & `pyspread-2.2/pyspread/share/icons/actions/edit-clear.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/edit-copy-results.svg` & `pyspread-2.2/pyspread/share/icons/actions/edit-copy-results.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/edit-copy.svg` & `pyspread-2.2/pyspread/share/icons/actions/edit-copy.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/edit-cut.svg` & `pyspread-2.2/pyspread/share/icons/actions/edit-cut.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/edit-delete-column.svg` & `pyspread-2.2/pyspread/share/icons/actions/edit-delete-column.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/edit-delete-row.svg` & `pyspread-2.2/pyspread/share/icons/actions/edit-delete-row.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/edit-delete-table.svg` & `pyspread-2.2/pyspread/share/icons/actions/edit-delete-table.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/edit-delete.svg` & `pyspread-2.2/pyspread/share/icons/actions/edit-delete.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/edit-find-next.svg` & `pyspread-2.2/pyspread/share/icons/actions/edit-find-next.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/edit-find-replace.svg` & `pyspread-2.2/pyspread/share/icons/actions/edit-find-replace.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/edit-find.svg` & `pyspread-2.2/pyspread/share/icons/actions/edit-find.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/edit-insert-column.svg` & `pyspread-2.2/pyspread/share/icons/actions/edit-insert-column.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/edit-insert-row.svg` & `pyspread-2.2/pyspread/share/icons/actions/edit-insert-row.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/edit-insert-table.svg` & `pyspread-2.2/pyspread/share/icons/actions/edit-insert-table.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/edit-paste-as.svg` & `pyspread-2.2/pyspread/share/icons/actions/edit-paste-as.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/edit-paste.svg` & `pyspread-2.2/pyspread/share/icons/actions/edit-paste.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/edit-quote.svg` & `pyspread-2.2/pyspread/share/icons/actions/edit-quote.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/edit-redo.svg` & `pyspread-2.2/pyspread/share/icons/actions/edit-redo.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/edit-resize-grid.svg` & `pyspread-2.2/pyspread/share/icons/actions/edit-resize-grid.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/edit-select-all.svg` & `pyspread-2.2/pyspread/share/icons/actions/edit-select-all.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/edit-sort-ascending.svg` & `pyspread-2.2/pyspread/share/icons/actions/edit-sort-ascending.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/edit-sort-descending.svg` & `pyspread-2.2/pyspread/share/icons/actions/edit-sort-descending.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/edit-undo.svg` & `pyspread-2.2/pyspread/share/icons/actions/edit-undo.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/format-background-color.svg` & `pyspread-2.2/pyspread/share/icons/actions/format-background-color.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/format-borders-0.svg` & `pyspread-2.2/pyspread/share/icons/actions/format-borders-0.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/format-borders-1.svg` & `pyspread-2.2/pyspread/share/icons/actions/format-borders-1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/format-borders-16.svg` & `pyspread-2.2/pyspread/share/icons/actions/format-borders-16.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/format-borders-2.svg` & `pyspread-2.2/pyspread/share/icons/actions/format-borders-2.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/format-borders-32.svg` & `pyspread-2.2/pyspread/share/icons/actions/format-borders-32.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/format-borders-4.svg` & `pyspread-2.2/pyspread/share/icons/actions/format-borders-4.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/format-borders-64.svg` & `pyspread-2.2/pyspread/share/icons/actions/format-borders-64.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/format-borders-8.svg` & `pyspread-2.2/pyspread/share/icons/actions/format-borders-8.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/format-borders-all.svg` & `pyspread-2.2/pyspread/share/icons/actions/format-borders-all.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/format-borders-bottom.svg` & `pyspread-2.2/pyspread/share/icons/actions/format-borders-bottom.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/format-borders-inner.svg` & `pyspread-2.2/pyspread/share/icons/actions/format-borders-inner.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/format-borders-left.svg` & `pyspread-2.2/pyspread/share/icons/actions/format-borders-left.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/format-borders-outer.svg` & `pyspread-2.2/pyspread/share/icons/actions/format-borders-outer.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/format-borders-right.svg` & `pyspread-2.2/pyspread/share/icons/actions/format-borders-right.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/format-borders-top-bottom.svg` & `pyspread-2.2/pyspread/share/icons/actions/format-borders-top-bottom.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/format-borders-top.svg` & `pyspread-2.2/pyspread/share/icons/actions/format-borders-top.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/format-button.svg` & `pyspread-2.2/pyspread/share/icons/actions/format-button.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/format-cell-chart.svg` & `pyspread-2.2/pyspread/share/icons/actions/format-cell-chart.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/format-cell-image.svg` & `pyspread-2.2/pyspread/share/icons/actions/format-cell-image.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/format-cell-markup.svg` & `pyspread-2.2/pyspread/share/icons/actions/format-cell-markup.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/format-cell-rotate-0.svg` & `pyspread-2.2/pyspread/share/icons/actions/format-cell-rotate-0.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/format-cell-rotate-180.svg` & `pyspread-2.2/pyspread/share/icons/actions/format-cell-rotate-180.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/format-cell-rotate-270.svg` & `pyspread-2.2/pyspread/share/icons/actions/format-cell-rotate-270.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/format-cell-rotate-90.svg` & `pyspread-2.2/pyspread/share/icons/actions/format-cell-rotate-90.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/format-cell-text.svg` & `pyspread-2.2/pyspread/share/icons/actions/format-cell-text.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/format-copy.svg` & `pyspread-2.2/pyspread/share/icons/actions/format-copy.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/format-font.svg` & `pyspread-2.2/pyspread/share/icons/actions/format-font.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/format-freeze.svg` & `pyspread-2.2/pyspread/share/icons/actions/format-freeze.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/format-justify-center.svg` & `pyspread-2.2/pyspread/share/icons/actions/format-justify-center.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/format-justify-fill.svg` & `pyspread-2.2/pyspread/share/icons/actions/format-justify-fill.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/format-justify-left.svg` & `pyspread-2.2/pyspread/share/icons/actions/format-justify-left.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/format-justify-right.svg` & `pyspread-2.2/pyspread/share/icons/actions/format-justify-right.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/format-line-color.svg` & `pyspread-2.2/pyspread/share/icons/actions/format-line-color.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/format-line-color2.svg` & `pyspread-2.2/pyspread/share/icons/actions/format-line-color2.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/format-lock.svg` & `pyspread-2.2/pyspread/share/icons/actions/format-lock.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/format-merge-cells.svg` & `pyspread-2.2/pyspread/share/icons/actions/format-merge-cells.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/format-paste.svg` & `pyspread-2.2/pyspread/share/icons/actions/format-paste.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/format-text-align-bottom.svg` & `pyspread-2.2/pyspread/share/icons/actions/format-text-align-bottom.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/format-text-align-center.svg` & `pyspread-2.2/pyspread/share/icons/actions/format-text-align-center.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/format-text-align-top.svg` & `pyspread-2.2/pyspread/share/icons/actions/format-text-align-top.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/format-text-bold.svg` & `pyspread-2.2/pyspread/share/icons/actions/format-text-bold.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/format-text-color.svg` & `pyspread-2.2/pyspread/share/icons/actions/format-text-color.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/format-text-italic.svg` & `pyspread-2.2/pyspread/share/icons/actions/format-text-italic.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/format-text-strikethrough.svg` & `pyspread-2.2/pyspread/share/icons/actions/format-text-strikethrough.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/format-text-underline.svg` & `pyspread-2.2/pyspread/share/icons/actions/format-text-underline.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/help-browser.svg` & `pyspread-2.2/pyspread/share/icons/actions/help-browser.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/help-dependencies.svg` & `pyspread-2.2/pyspread/share/icons/actions/help-dependencies.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/help-faq.svg` & `pyspread-2.2/pyspread/share/icons/actions/help-faq.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/macro-insert-chart.svg` & `pyspread-2.2/pyspread/share/icons/actions/macro-insert-chart.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/macro-insert-image.svg` & `pyspread-2.2/pyspread/share/icons/actions/macro-insert-image.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/macro-insert-sum.svg` & `pyspread-2.2/pyspread/share/icons/actions/macro-insert-sum.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/macro-link-image.svg` & `pyspread-2.2/pyspread/share/icons/actions/macro-link-image.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/macro-open.svg` & `pyspread-2.2/pyspread/share/icons/actions/macro-open.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/macro-save.svg` & `pyspread-2.2/pyspread/share/icons/actions/macro-save.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/menu-manager.svg` & `pyspread-2.2/pyspread/share/icons/actions/menu-manager.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/view-check-spelling.svg` & `pyspread-2.2/pyspread/share/icons/actions/view-check-spelling.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/view-fullscreen.svg` & `pyspread-2.2/pyspread/share/icons/actions/view-fullscreen.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/view-goto-cell.svg` & `pyspread-2.2/pyspread/share/icons/actions/view-goto-cell.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/view-refresh.svg` & `pyspread-2.2/pyspread/share/icons/actions/view-refresh.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/view-show-frozen.svg` & `pyspread-2.2/pyspread/share/icons/actions/view-show-frozen.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/view-timer.svg` & `pyspread-2.2/pyspread/share/icons/actions/view-timer.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/view-zoom-in.svg` & `pyspread-2.2/pyspread/share/icons/actions/view-zoom-in.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/view-zoom-original.svg` & `pyspread-2.2/pyspread/share/icons/actions/view-zoom-original.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/actions/view-zoom-out.svg` & `pyspread-2.2/pyspread/share/icons/actions/view-zoom-out.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_area_1_1.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_area_1_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_area_1_2.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_area_1_2.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_area_1_3.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_area_1_3.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_bar_1_1.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_bar_1_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_bar_1_2.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_bar_1_2.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_bar_1_3.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_bar_1_3.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_boxplot_1_1.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_boxplot_1_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_boxplot_1_2.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_boxplot_1_2.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_boxplot_2_1.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_boxplot_2_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_boxplot_2_2.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_boxplot_2_2.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_bubble_1_1.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_bubble_1_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_bubble_1_2.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_bubble_1_2.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_color_polar_1_1.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_color_polar_1_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_colored_1_1.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_colored_1_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_column_1_1.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_column_1_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_column_1_2.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_column_1_2.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_column_1_3.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_column_1_3.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_contour_1_1.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_contour_1_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_contour_1_2.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_contour_1_2.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_contour_2_1.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_contour_2_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_contour_2_2.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_contour_2_2.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_contour_polar_1_1.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_contour_polar_1_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_dropbar_1_1.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_dropbar_1_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_dropbar_1_2.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_dropbar_1_2.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_dropbar_1_3.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_dropbar_1_3.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_dropbar_1_4.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_dropbar_1_4.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_histogram_1_1.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_histogram_1_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_histogram_1_2.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_histogram_1_2.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_histogram_1_3.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_histogram_1_3.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_histogram_1_4.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_histogram_1_4.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_histogram_2_1.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_histogram_2_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_line_1_1.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_line_1_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_line_1_2.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_line_1_2.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_line_1_3.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_line_1_3.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_line_2_1.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_line_2_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_line_2_2.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_line_2_2.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_line_2_3.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_line_2_3.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_matrix_1_1.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_matrix_1_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_matrix_1_2.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_matrix_1_2.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_matrix_1_3.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_matrix_1_3.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_minmax_1_1.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_minmax_1_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_minmax_1_2.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_minmax_1_2.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_minmax_1_3.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_minmax_1_3.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_minmax_1_4.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_minmax_1_4.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_minmax_2_1.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_minmax_2_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_minmax_2_2.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_minmax_2_2.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_minmax_2_3.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_minmax_2_3.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_minmax_2_4.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_minmax_2_4.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_pie_1_1.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_pie_1_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_pie_2_1.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_pie_2_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_pie_3_1.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_pie_3_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_pie_3_2.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_pie_3_2.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_polar_1_1.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_polar_1_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_prob_1_1.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_prob_1_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_radar_1_1.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_radar_1_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_radar_1_2.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_radar_1_2.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_radar_1_3.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_radar_1_3.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_ring_1_1.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_ring_1_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_ring_1_2.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_ring_1_2.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_scatter_1_1.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_scatter_1_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_scatter_3_1.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_scatter_3_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_scatter_3_2.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_scatter_3_2.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_scatter_3_3.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_scatter_3_3.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_scatter_4_1.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_scatter_4_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_scatter_4_2.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_scatter_4_2.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_scatter_4_3.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_scatter_4_3.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_scatter_4_4.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_scatter_4_4.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_scatterhist_1_1.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_scatterhist_1_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_surface_2_1.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_surface_2_1.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_surface_2_2.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_surface_2_2.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/charts/chart_surface_2_3.svg` & `pyspread-2.2/pyspread/share/icons/charts/chart_surface_2_3.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/hicolor/64x64/pyspread.ico` & `pyspread-2.2/pyspread/share/icons/hicolor/64x64/pyspread.ico`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/hicolor/64x64/pyspread.png` & `pyspread-2.2/pyspread/share/icons/hicolor/64x64/pyspread.png`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/hicolor/svg/pyspread.svg` & `pyspread-2.2/pyspread/share/icons/hicolor/svg/pyspread.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/status/status-safe-mode.svg` & `pyspread-2.2/pyspread/share/icons/status/status-safe-mode.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/icons/status/status-selection-mode.svg` & `pyspread-2.2/pyspread/share/icons/status/status-selection-mode.svg`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/metainfo/io.gitlab.pyspread.pyspread.metainfo.xml` & `pyspread-2.2/pyspread/share/metainfo/io.gitlab.pyspread.pyspread.metainfo.xml`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/templates/matplotlib/COPYING` & `pyspread-2.2/pyspread/share/templates/matplotlib/COPYING`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-The files in this folder are adapted from the matplotlib gallery.
+The files in this folder are adapted from the matplotlib gallery and from the rpy2 tutorial pages.
 Adaptations comprise:
  + An initial line for instantiating a figure.
  + Changes from pylab to the object oriented interface.
  + Removal of features for simpler and shorter templates.
  + Addition of the final line that states the figure object.
+ + For the rpy2 files the conversion to SVG
 
 The files in this folder are licensed with the same license as matplolib (see https://matplotlib.org/3.1.1/users/license.html):
 
 1. This LICENSE AGREEMENT is between the Matplotlib Development Team ("MDT"), and the Individual or Organization ("Licensee") accessing and otherwise using matplotlib software in source or binary form and its associated documentation.
 
 2. Subject to the terms and conditions of this License Agreement, MDT hereby grants Licensee a nonexclusive, royalty-free, world-wide license to reproduce, analyze, test, perform and/or display publicly, prepare derivative works, distribute, and otherwise use matplotlib 3.1.1 alone or in any derivative version, provided, however, that MDT's License Agreement and MDT's notice of copyright, i.e., "Copyright (c) 2012-2013 Matplotlib Development Team; All Rights Reserved" are retained in matplotlib 3.1.1 alone or in any derivative version prepared by Licensee.
 
@@ -17,8 +18,8 @@
 
 5. MDT SHALL NOT BE LIABLE TO LICENSEE OR ANY OTHER USERS OF MATPLOTLIB 3.1.1 FOR ANY INCIDENTAL, SPECIAL, OR CONSEQUENTIAL DAMAGES OR LOSS AS A RESULT OF MODIFYING, DISTRIBUTING, OR OTHERWISE USING MATPLOTLIB 3.1.1, OR ANY DERIVATIVE THEREOF, EVEN IF ADVISED OF THE POSSIBILITY THEREOF.
 
 6. This License Agreement will automatically terminate upon a material breach of its terms and conditions.
 
 7. Nothing in this License Agreement shall be deemed to create any relationship of agency, partnership, or joint venture between MDT and Licensee. This License Agreement does not grant permission to use MDT trademarks or trade name in a trademark sense to endorse or promote products or services of Licensee, or any third party.
 
-8. By copying, installing or otherwise using matplotlib 3.1.1, Licensee agrees to be bound by the terms and conditions of this License Agreement.
+8. By copying, installing or otherwise using matplotlib 3.1.1, Licensee agrees to be bound by the terms and conditions of this License Agreement.
```

### Comparing `pyspread-2.1.1/pyspread/share/templates/matplotlib/chart_bar_1_3.py` & `pyspread-2.2/pyspread/share/templates/matplotlib/chart_bar_1_3.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/templates/matplotlib/chart_boxplot_2_2.py` & `pyspread-2.2/pyspread/share/templates/matplotlib/chart_boxplot_2_2.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/templates/matplotlib/chart_column_1_1.py` & `pyspread-2.2/pyspread/share/templates/matplotlib/chart_column_1_1.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/templates/matplotlib/chart_column_1_2.py` & `pyspread-2.2/pyspread/share/templates/matplotlib/chart_column_1_2.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/templates/matplotlib/chart_contour_1_2.py` & `pyspread-2.2/pyspread/share/templates/matplotlib/chart_contour_1_2.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/templates/matplotlib/chart_histogram_1_4.py` & `pyspread-2.2/pyspread/share/templates/matplotlib/chart_histogram_1_4.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/templates/matplotlib/chart_ring_1_1.py` & `pyspread-2.2/pyspread/share/templates/matplotlib/chart_ring_1_1.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/templates/matplotlib/chart_scatterhist_1_1.py` & `pyspread-2.2/pyspread/share/templates/matplotlib/chart_scatterhist_1_1.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/share/templates/matplotlib/chart_surface_2_1.py` & `pyspread-2.2/pyspread/share/templates/matplotlib/chart_surface_2_1.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/test/test_cli.py` & `pyspread-2.2/pyspread/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/test/test_grid.py` & `pyspread-2.2/pyspread/test/test_grid.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/test/test_grid_renderer.py` & `pyspread-2.2/pyspread/test/test_grid_renderer.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/test/test_pyspread.py` & `pyspread-2.2/pyspread/test/test_pyspread.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/test/test_workflows.py` & `pyspread-2.2/pyspread/test/test_workflows.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/toolbar.py` & `pyspread-2.2/pyspread/toolbar.py`

 * *Files 25% similar despite different names*

```diff
@@ -38,14 +38,25 @@
 
 try:
     import matplotlib.figure as matplotlib_figure
 except ImportError:
     matplotlib_figure = None
 
 try:
+    import rpy2
+    from rpy2.robjects.packages import importr
+except ImportError:
+    rpy2 = None
+
+try:
+    import plotnine
+except ImportError:
+    plotnine = None
+
+try:
     from pyspread.actions import MainWindowActions, ChartDialogActions
     from pyspread.icons import Icon
     from pyspread.menus import ToolbarManagerMenu
     from pyspread.widgets import FindEditor
 except ImportError:
     from actions import MainWindowActions, ChartDialogActions
     from icons import Icon
@@ -325,14 +336,16 @@
 
         self.addWidget(self.get_manager_button())
 
 
 class ChartTemplatesToolBar(ToolBarBase):
     """Toolbar for chart dialog for inserting template chart code"""
 
+    tooltip_tpl = "Package {} required but not installed"
+
     def __init__(self, parent: QWidget):
         """
         :param parent: Parent widget, e.g. chart dialog window
 
         """
 
         super().__init__("Chart templates toolbar", parent)
@@ -362,7 +375,88 @@
         self.addAction(actions.chart_histogram_1_4)
         self.addAction(actions.chart_scatterhist_1_1)
         self.addAction(actions.chart_matrix_1_1)
         self.addAction(actions.chart_contour_1_2)
         self.addAction(actions.chart_surface_2_1)
 
         self.addWidget(self.get_manager_button())
+
+
+class RChartTemplatesToolBar(ToolBarBase):
+    """Toolbar for chart dialog for inserting R template chart code
+
+    Requires rpy2 with ggplot, lattice and graphics packages
+
+    """
+
+    tooltip_tpl = "R Package {} required but not installed"
+
+    def __init__(self, parent: QWidget):
+        """
+        :param parent: Parent widget, e.g. chart dialog window
+
+        """
+
+        super().__init__("Chart templates toolbar", parent)
+
+        if rpy2 is None:
+            self.close()
+
+        self.setObjectName("R Chart templates toolbar")
+        self._create_toolbar(parent.actions)
+
+    @staticmethod
+    def is_r_package_installed(package_name):
+        """True if the R package is installed
+
+        :param package_name: Name of R package to checked
+
+        """
+
+        try:
+            importr(package_name)
+        except RuntimeError:
+            return False
+        return True
+
+    def _create_toolbar(self, actions: ChartDialogActions):
+        """Fills the chart dialog toolbar with QActions
+
+        :param actions: Chart dialog actions
+
+        """
+
+        self.addAction(actions.chart_r_graphics_barplot_1_1)
+        self.addAction(actions.chart_r_ggplot2_geom_boxplot_1_2)
+        self.addAction(actions.chart_r_ggplot2_geom_point_1_1)
+        self.addAction(actions.chart_r_lattice_xyplot_1_1)
+        self.addAction(actions.chart_r_ggplot2_geom_density2d_1_2)
+        self.addAction(actions.chart_r_lattice_wireframe_2_1)
+        self.addAction(actions.chart_plotnine_geom_bar_1_1)
+
+        if not self.is_r_package_installed("graphics"):
+            tooltip = self.tooltip_tpl.format("graphics")
+            actions.chart_r_graphics_barplot_1_1.setEnabled(False)
+            actions.chart_r_graphics_barplot_1_1.setToolTip(tooltip)
+
+        if not self.is_r_package_installed("lattice"):
+            tooltip = self.tooltip_tpl.format("lattice")
+            actions.chart_r_lattice_xyplot_1_1.setEnabled(False)
+            actions.chart_r_lattice_xyplot_1_1.setToolTip(tooltip)
+            actions.chart_r_lattice_wireframe_2_1.setEnabled(False)
+            actions.chart_r_lattice_wireframe_2_1.setToolTip(tooltip)
+
+        if not self.is_r_package_installed("ggplot2"):
+            tooltip = self.tooltip_tpl.format("ggplot2")
+            actions.chart_r_ggplot2_geom_boxplot_1_2.setEnabled(False)
+            actions.chart_r_ggplot2_geom_boxplot_1_2.setToolTip(tooltip)
+            actions.chart_r_ggplot2_geom_point_1_1.setEnabled(False)
+            actions.chart_r_ggplot2_geom_point_1_1.setToolTip(tooltip)
+            actions.chart_r_ggplot2_geom_density2d_1_2.setEnabled(False)
+            actions.chart_r_ggplot2_geom_density2d_1_2.setToolTip(tooltip)
+
+        if plotnine is None:
+            tooltip = self.tooltip_tpl.format("plotnine")
+            actions.chart_plotnine_geom_bar_1_1.setEnabled(False)
+            actions.chart_plotnine_geom_bar_1_1.setToolTip(tooltip)
+
+        self.addWidget(self.get_manager_button())
```

### Comparing `pyspread-2.1.1/pyspread/widgets.py` & `pyspread-2.2/pyspread/widgets.py`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread/workflows.py` & `pyspread-2.2/pyspread/workflows.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,31 +24,30 @@
 
 """
 
 from ast import literal_eval
 from base64 import b85encode
 import bz2
 from contextlib import contextmanager
+from copy import copy
 import csv
 from itertools import cycle
 import io
 import numpy
 import os.path
 from pathlib import Path
 from shutil import move
 from tempfile import NamedTemporaryFile
 from typing import Iterable, Tuple
 
-from PyQt5.QtCore import (
-    Qt, QMimeData, QModelIndex, QBuffer, QRect, QRectF, QItemSelectionModel,
-    QSize)
-from PyQt5.QtGui import QTextDocument, QImage, QPainter, QBrush, QPen
-from PyQt5.QtWidgets import (
-    QApplication, QMessageBox, QInputDialog, QStyleOptionViewItem, QTableView,
-    QUndoCommand)
+from PyQt5.QtCore import (Qt, QMimeData, QModelIndex, QBuffer, QRect, QRectF,
+                          QItemSelectionModel, QSize)
+from PyQt5.QtGui import QTextDocument, QImage, QPainter
+from PyQt5.QtWidgets import (QApplication, QMessageBox, QInputDialog,
+                             QStyleOptionViewItem, QTableView, QUndoCommand)
 try:
     from PyQt5.QtSvg import QSvgGenerator
 except ImportError:
     QSvgGenerator = None
 
 try:
     import matplotlib
@@ -805,14 +804,16 @@
             if svg_area is None:
                 # Get area for svg export
                 svg_area = SvgExportAreaDialog(self.main_window, grid,
                                                title="Svg export area").area
             if svg_area is None:
                 return
 
+            self.main_window.print_area = svg_area
+
             rows = self.get_paint_rows(svg_area.top, svg_area.bottom)
             columns = self.get_paint_columns(svg_area.left, svg_area.right)
             total_height = self.get_total_height(svg_area.top, svg_area.bottom)
             total_width = self.get_total_width(svg_area.left, svg_area.right)
 
             x_offset = grid.columnViewportPosition(0)
             y_offset = grid.rowViewportPosition(0)
@@ -828,14 +829,15 @@
             generator.setViewBox(paint_rect)
             option = QStyleOptionViewItem()
 
             painter = QPainter(generator)
             self.paint(painter, option, paint_rect, rows, columns)
 
             painter.end()
+            self.main_window.print_area = None
 
     def _qimage_export(self, filepath: Path, file_format: str):
         """Export to png file filepath
 
         :param filepath: Path of file to be exported
         :param file_format: File format to be exported, e.g. png
 
@@ -1825,18 +1827,20 @@
         (top, left), (_, _) = selection.get_grid_bbox(grid.model.shape)
 
         table_cell_attributes = cell_attributes.for_table(grid.table)
         for __selection, _, attrs in table_cell_attributes:
             new_selection = selection & __selection
             if new_selection:
                 # We do not copy merged cells and cell renderers
-                remove_tabu_keys(attrs)
+                __attrs = copy(attrs)
+                remove_tabu_keys(__attrs)
                 new_shifted_selection = new_selection.shifted(-top, -left)
-                cell_attribute = new_shifted_selection.parameters, attrs
-                new_cell_attributes.append(cell_attribute)
+                if __attrs:
+                    cell_attribute = new_shifted_selection.parameters, __attrs
+                    new_cell_attributes.append(cell_attribute)
 
         ca_repr = bytes(repr(new_cell_attributes), encoding='utf-8')
 
         clipboard = QApplication.clipboard()
         mime_data = QMimeData()
         mime_data.setData("application/x-pyspread-cell-attributes", ca_repr)
         clipboard.setMimeData(mime_data)
```

### Comparing `pyspread-2.1.1/pyspread.desktop` & `pyspread-2.2/pyspread.desktop`

 * *Files identical despite different names*

### Comparing `pyspread-2.1.1/pyspread.egg-info/PKG-INFO` & `pyspread-2.2/pyspread.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyspread
-Version: 2.1.1
+Version: 2.2
 Summary: Pyspread is a non-traditional spreadsheet application that is based on and written in the programming language Python.
 Home-page: https://pyspread.gitlab.io
 Author: Martin Manns
 Author-email: mmanns@gmx.net
 License: GPL v3 :: GNU General Public License
 Project-URL: Bug Tracker, https://gitlab.com/pyspread/pyspread/issues
 Project-URL: Documentation, https://pyspread.gitlab.io/docs.html
@@ -127,10 +127,12 @@
 Requires: PyQt5 (>=5.10)
 Requires: setuptools (>=40.0)
 Requires: markdown2 (>=2.3)
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: matplotlib
 Provides-Extra: pip
+Provides-Extra: plotnine
 Provides-Extra: py-moneyed
 Provides-Extra: pyenchant
 Provides-Extra: python-dateutil
+Provides-Extra: rpy2
```

### Comparing `pyspread-2.1.1/pyspread.egg-info/SOURCES.txt` & `pyspread-2.2/pyspread.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -103,14 +103,16 @@
 pyspread/share/doc/tutorial/images/Tutorial2.png
 pyspread/share/doc/tutorial/images/Tutorial3.png
 pyspread/share/doc/tutorial/images/Tutorial4.png
 pyspread/share/examples/big.csv
 pyspread/share/examples/conditional_formatting.pysu
 pyspread/share/examples/images and charts.pysu
 pyspread/share/examples/pivot.pysu
+pyspread/share/examples/pyspred_with_plotnine.pysu
+pyspread/share/examples/rpy2_example.pysu
 pyspread/share/examples/test_write.csv
 pyspread/share/examples/wagner_whitin.pysu
 pyspread/share/icons/actions/document-approve.svg
 pyspread/share/icons/actions/document-export.svg
 pyspread/share/icons/actions/document-import.svg
 pyspread/share/icons/actions/document-log-out.svg
 pyspread/share/icons/actions/document-new-gpg-key.svg
@@ -259,16 +261,23 @@
 pyspread/share/icons/charts/chart_minmax_2_2.svg
 pyspread/share/icons/charts/chart_minmax_2_3.svg
 pyspread/share/icons/charts/chart_minmax_2_4.svg
 pyspread/share/icons/charts/chart_pie_1_1.svg
 pyspread/share/icons/charts/chart_pie_2_1.svg
 pyspread/share/icons/charts/chart_pie_3_1.svg
 pyspread/share/icons/charts/chart_pie_3_2.svg
+pyspread/share/icons/charts/chart_plotnine_geom_bar_1_1.svg
 pyspread/share/icons/charts/chart_polar_1_1.svg
 pyspread/share/icons/charts/chart_prob_1_1.svg
+pyspread/share/icons/charts/chart_r_ggplot2_geom_boxplot_1_2.svg
+pyspread/share/icons/charts/chart_r_ggplot2_geom_density2d_1_2.svg
+pyspread/share/icons/charts/chart_r_ggplot2_geom_point_1_1.svg
+pyspread/share/icons/charts/chart_r_graphics_barplot_1_1.svg
+pyspread/share/icons/charts/chart_r_lattice_wireframe_2_1.svg
+pyspread/share/icons/charts/chart_r_lattice_xyplot_1_1.svg
 pyspread/share/icons/charts/chart_radar_1_1.svg
 pyspread/share/icons/charts/chart_radar_1_2.svg
 pyspread/share/icons/charts/chart_radar_1_3.svg
 pyspread/share/icons/charts/chart_ring_1_1.svg
 pyspread/share/icons/charts/chart_ring_1_2.svg
 pyspread/share/icons/charts/chart_scatter_1_1.svg
 pyspread/share/icons/charts/chart_scatter_3_1.svg
@@ -302,14 +311,21 @@
 pyspread/share/templates/matplotlib/chart_matrix_1_1.py
 pyspread/share/templates/matplotlib/chart_pie_1_1.py
 pyspread/share/templates/matplotlib/chart_polar_1_1.py
 pyspread/share/templates/matplotlib/chart_ring_1_1.py
 pyspread/share/templates/matplotlib/chart_scatter_1_1.py
 pyspread/share/templates/matplotlib/chart_scatterhist_1_1.py
 pyspread/share/templates/matplotlib/chart_surface_2_1.py
+pyspread/share/templates/plotnine/chart_plotnine_geom_bar_1_1.py
+pyspread/share/templates/rpy2/chart_r_ggplot2_geom_boxplot_1_2.py
+pyspread/share/templates/rpy2/chart_r_ggplot2_geom_density2d_1_2.py
+pyspread/share/templates/rpy2/chart_r_ggplot2_geom_point_1_1.py
+pyspread/share/templates/rpy2/chart_r_graphics_barplot_1_1.py
+pyspread/share/templates/rpy2/chart_r_lattice_wireframe_2_1.py
+pyspread/share/templates/rpy2/chart_r_lattice_xyplot_1_1.py
 pyspread/test/__init__.py
 pyspread/test/test_cli.py
 pyspread/test/test_grid.py
 pyspread/test/test_grid_renderer.py
 pyspread/test/test_invalid_unsigned_1.pysu
 pyspread/test/test_invalid_unsigned_2.pysu
 pyspread/test/test_invalid_unsigned_3.pysu
```

### Comparing `pyspread-2.1.1/setup.py` & `pyspread-2.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,30 +52,33 @@
             'share/*',
             'share/*/*',
             'share/*/*/*',
             'share/*/*/*/*',
             'share/*/*/*/*/*',
         ]
     },
-    data_files = [
-        ('pyspread/share/applications', ['pyspread/share/applications/io.gitlab.pyspread.pyspread.desktop']),
+    data_files=[
+        ('pyspread/share/applications',
+         ['pyspread/share/applications/io.gitlab.pyspread.pyspread.desktop']),
     ],
     license='GPL v3 :: GNU General Public License',
     keywords=['spreadsheet', 'pyspread'],
     python_requires='>=3.6',
     requires=['numpy (>=1.1)',
               'PyQt5 (>=5.10)',
               'setuptools (>=40.0)',
               'markdown2 (>=2.3)'],
     extras_require={
         'matplotlib': ['matplotlib (>=1.1.1)'],
         'pyenchant': ['pyenchant (>=1.1)'],
         'pip': ['pip (>=18)'],
         'python-dateutil': ['python-dateutil (>=2.7.0)'],
         'py-moneyed': ['py-moneyed (>=2.0)'],
+        'rpy2': ['rpy2 (>=3.4)'],
+        'plotnine': ['plotnine (>=0.8)'],
     },
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: X11 Applications :: Qt',
         'Environment :: Win32 (MS Windows)',
         'Intended Audience :: End Users/Desktop',
         'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
```

