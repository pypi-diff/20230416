# Comparing `tmp/badi_users-0.9.3.tar.gz` & `tmp/badi_users-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "badi_users-0.9.3.tar", last modified: Tue Apr 11 07:16:26 2023, max compression
+gzip compressed data, was "badi_users-0.9.4.tar", last modified: Sun Apr 16 12:32:09 2023, max compression
```

## Comparing `badi_users-0.9.3.tar` & `badi_users-0.9.4.tar`

### file list

```diff
@@ -1,311 +1,311 @@
-drwxrwxrwx   0        0        0        0 2023-04-11 07:16:26.233570 badi_users-0.9.3/
--rw-rw-rw-   0        0        0     1093 2022-09-24 06:05:13.000000 badi_users-0.9.3/LICENSE
--rw-rw-rw-   0        0        0     1066 2022-11-10 17:03:20.000000 badi_users-0.9.3/MANIFEST.in
--rw-rw-rw-   0        0        0      419 2023-04-11 07:16:26.232573 badi_users-0.9.3/PKG-INFO
--rw-rw-rw-   0        0        0      143 2022-10-02 09:04:41.000000 badi_users-0.9.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-11 07:16:26.012714 badi_users-0.9.3/badi_ticket/
--rw-rw-rw-   0        0        0        0 2023-04-11 06:26:43.000000 badi_users-0.9.3/badi_ticket/__init__.py
--rw-rw-rw-   0        0        0      143 2023-04-11 06:26:43.000000 badi_users-0.9.3/badi_ticket/admin.py
--rw-rw-rw-   0        0        0     9803 2023-04-11 06:38:59.000000 badi_users-0.9.3/badi_ticket/api.py
--rw-rw-rw-   0        0        0      129 2023-04-11 06:26:43.000000 badi_users-0.9.3/badi_ticket/apps.py
-drwxrwxrwx   0        0        0        0 2023-04-11 07:16:25.987792 badi_users-0.9.3/badi_ticket/locale/
-drwxrwxrwx   0        0        0        0 2023-04-11 07:16:25.987792 badi_users-0.9.3/badi_ticket/locale/fa/
-drwxrwxrwx   0        0        0        0 2023-04-11 07:16:26.013710 badi_users-0.9.3/badi_ticket/locale/fa/LC_MESSAGES/
--rw-rw-rw-   0        0        0     2637 2023-04-11 06:17:23.000000 badi_users-0.9.3/badi_ticket/locale/fa/LC_MESSAGES/django.mo
-drwxrwxrwx   0        0        0        0 2023-04-11 07:16:26.014708 badi_users-0.9.3/badi_ticket/migrations/
--rw-rw-rw-   0        0        0        0 2022-08-06 18:28:13.000000 badi_users-0.9.3/badi_ticket/migrations/__init__.py
--rw-rw-rw-   0        0        0     3101 2023-04-11 06:26:43.000000 badi_users-0.9.3/badi_ticket/models.py
--rw-rw-rw-   0        0        0      313 2023-04-11 06:26:43.000000 badi_users-0.9.3/badi_ticket/routers.py
--rw-rw-rw-   0        0        0     2082 2023-04-11 06:26:43.000000 badi_users-0.9.3/badi_ticket/serializers.py
-drwxrwxrwx   0        0        0        0 2023-04-11 07:16:25.988778 badi_users-0.9.3/badi_ticket/static/
-drwxrwxrwx   0        0        0        0 2023-04-11 07:16:25.989784 badi_users-0.9.3/badi_ticket/static/ticket/
-drwxrwxrwx   0        0        0        0 2023-04-11 07:16:26.015704 badi_users-0.9.3/badi_ticket/static/ticket/js/
--rw-rw-rw-   0        0        0     2147 2023-04-11 06:26:43.000000 badi_users-0.9.3/badi_ticket/static/ticket/js/chat.js
-drwxrwxrwx   0        0        0        0 2023-04-11 07:16:26.015704 badi_users-0.9.3/badi_ticket/templates/
--rw-rw-rw-   0        0        0        0 2023-04-11 06:26:43.000000 badi_users-0.9.3/badi_ticket/templates/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 07:16:26.020692 badi_users-0.9.3/badi_ticket/templates/ticket/
--rw-rw-rw-   0        0        0     6358 2023-04-11 06:26:43.000000 badi_users-0.9.3/badi_ticket/templates/ticket/admin_tickets.html
--rw-rw-rw-   0        0        0     5265 2023-04-11 06:26:43.000000 badi_users-0.9.3/badi_ticket/templates/ticket/message_list.html
--rw-rw-rw-   0        0        0     9642 2023-04-11 06:26:43.000000 badi_users-0.9.3/badi_ticket/templates/ticket/my_tickets.html
--rw-rw-rw-   0        0        0     7541 2023-04-11 07:13:57.000000 badi_users-0.9.3/badi_ticket/templates/ticket/ticket_create.html
--rw-rw-rw-   0        0        0     1639 2023-04-11 06:26:43.000000 badi_users-0.9.3/badi_ticket/templates/ticket/ticket_update.html
--rw-rw-rw-   0        0        0       63 2023-04-11 06:26:43.000000 badi_users-0.9.3/badi_ticket/tests.py
--rw-rw-rw-   0        0        0      583 2023-04-11 06:26:43.000000 badi_users-0.9.3/badi_ticket/urls.py
--rw-rw-rw-   0        0        0     2057 2023-04-11 06:26:43.000000 badi_users-0.9.3/badi_ticket/views.py
-drwxrwxrwx   0        0        0        0 2023-04-11 07:16:26.024682 badi_users-0.9.3/badi_user/
--rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.3/badi_user/__init__.py
--rw-rw-rw-   0        0        0      166 2023-03-27 19:00:31.000000 badi_users-0.9.3/badi_user/admin.py
-drwxrwxrwx   0        0        0        0 2023-04-11 07:16:26.027674 badi_users-0.9.3/badi_user/api/
--rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.3/badi_user/api/__init__.py
--rw-rw-rw-   0        0        0    29693 2023-03-27 19:00:31.000000 badi_users-0.9.3/badi_user/api/api.py
--rw-rw-rw-   0        0        0      485 2023-03-27 19:00:31.000000 badi_users-0.9.3/badi_user/api/routers.py
--rw-rw-rw-   0        0        0     6013 2023-03-27 19:00:31.000000 badi_users-0.9.3/badi_user/api/serializers.py
--rw-rw-rw-   0        0        0      183 2023-03-27 19:00:31.000000 badi_users-0.9.3/badi_user/apps.py
--rw-rw-rw-   0        0        0     3428 2023-03-27 19:00:31.000000 badi_users-0.9.3/badi_user/filter.py
-drwxrwxrwx   0        0        0        0 2023-04-11 07:16:25.992768 badi_users-0.9.3/badi_user/locale/
-drwxrwxrwx   0        0        0        0 2023-04-11 07:16:25.992768 badi_users-0.9.3/badi_user/locale/fa/
-drwxrwxrwx   0        0        0        0 2023-04-11 07:16:26.028670 badi_users-0.9.3/badi_user/locale/fa/LC_MESSAGES/
--rw-rw-rw-   0        0        0     3724 2023-04-11 06:17:23.000000 badi_users-0.9.3/badi_user/locale/fa/LC_MESSAGES/django.mo
-drwxrwxrwx   0        0        0        0 2023-04-11 07:16:26.029668 badi_users-0.9.3/badi_user/migrations/
--rw-rw-rw-   0        0        0        0 2022-08-06 18:28:13.000000 badi_users-0.9.3/badi_user/migrations/__init__.py
--rw-rw-rw-   0        0        0     6551 2023-03-27 19:00:31.000000 badi_users-0.9.3/badi_user/models.py
-drwxrwxrwx   0        0        0        0 2023-04-11 07:16:26.030665 badi_users-0.9.3/badi_user/templates/
--rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.3/badi_user/templates/__init__.py
--rw-rw-rw-   0        0        0       27 2023-03-27 19:00:31.000000 badi_users-0.9.3/badi_user/templates/badi-user-test.html
-drwxrwxrwx   0        0        0        0 2023-04-11 07:16:26.032660 badi_users-0.9.3/badi_user/templates/group/
--rw-rw-rw-   0        0        0     8558 2023-03-27 19:00:31.000000 badi_users-0.9.3/badi_user/templates/group/group_create.html
--rw-rw-rw-   0        0        0     5472 2023-03-27 19:00:31.000000 badi_users-0.9.3/badi_user/templates/group/group_update.html
-drwxrwxrwx   0        0        0        0 2023-04-11 07:16:26.034655 badi_users-0.9.3/badi_user/templates/log/
--rw-rw-rw-   0        0        0     3987 2023-03-27 19:00:31.000000 badi_users-0.9.3/badi_user/templates/log/log_list.html
-drwxrwxrwx   0        0        0        0 2023-04-11 07:16:26.035652 badi_users-0.9.3/badi_user/templates/login-theme/
--rw-rw-rw-   0        0        0     7336 2023-03-27 19:00:31.000000 badi_users-0.9.3/badi_user/templates/login-theme/login-1.html
-drwxrwxrwx   0        0        0        0 2023-04-11 07:16:26.038644 badi_users-0.9.3/badi_user/templates/member/
--rw-rw-rw-   0        0        0     6863 2023-03-27 19:00:31.000000 badi_users-0.9.3/badi_user/templates/member/member_create.html
--rw-rw-rw-   0        0        0    22635 2023-03-27 19:00:31.000000 badi_users-0.9.3/badi_user/templates/member/member_list.html
--rw-rw-rw-   0        0        0     4783 2023-03-28 07:29:01.000000 badi_users-0.9.3/badi_user/templates/member/member_self_update.html
--rw-rw-rw-   0        0        0     6525 2023-03-27 19:00:31.000000 badi_users-0.9.3/badi_user/templates/member/member_update.html
-drwxrwxrwx   0        0        0        0 2023-04-11 07:16:26.041635 badi_users-0.9.3/badi_user/templates/user/
--rw-rw-rw-   0        0        0     6745 2023-03-27 19:00:31.000000 badi_users-0.9.3/badi_user/templates/user/change_password.html
--rw-rw-rw-   0        0        0     5973 2023-03-27 19:00:31.000000 badi_users-0.9.3/badi_user/templates/user/user_create.html
--rw-rw-rw-   0        0        0     4019 2023-03-27 19:00:31.000000 badi_users-0.9.3/badi_user/templates/user/user_list.html
--rw-rw-rw-   0        0        0     5005 2023-03-27 19:00:31.000000 badi_users-0.9.3/badi_user/templates/user/user_update.html
-drwxrwxrwx   0        0        0        0 2023-04-11 07:16:26.043630 badi_users-0.9.3/badi_user/templatetags/
--rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.3/badi_user/templatetags/__init__.py
--rw-rw-rw-   0        0        0     5950 2023-03-27 19:00:31.000000 badi_users-0.9.3/badi_user/templatetags/appfilter.py
--rw-rw-rw-   0        0        0      500 2023-03-27 19:00:31.000000 badi_users-0.9.3/badi_user/tests.py
-drwxrwxrwx   0        0        0        0 2023-04-11 07:16:26.049615 badi_users-0.9.3/badi_user/ui/
--rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.3/badi_user/ui/__init__.py
--rw-rw-rw-   0        0        0     1484 2023-03-27 19:00:31.000000 badi_users-0.9.3/badi_user/ui/forms.py
--rw-rw-rw-   0        0        0      320 2023-03-27 19:00:31.000000 badi_users-0.9.3/badi_user/ui/log_views.py
--rw-rw-rw-   0        0        0     1706 2023-03-28 08:00:41.000000 badi_users-0.9.3/badi_user/ui/member_views.py
--rw-rw-rw-   0        0        0      672 2023-03-27 19:00:31.000000 badi_users-0.9.3/badi_user/ui/notification_views.py
--rw-rw-rw-   0        0        0      644 2023-03-27 19:00:31.000000 badi_users-0.9.3/badi_user/ui/roles_views.py
--rw-rw-rw-   0        0        0     1614 2023-03-27 19:00:31.000000 badi_users-0.9.3/badi_user/ui/urls.py
--rw-rw-rw-   0        0        0     2633 2023-03-27 19:00:31.000000 badi_users-0.9.3/badi_user/ui/views.py
-drwxrwxrwx   0        0        0        0 2023-04-11 07:16:26.066453 badi_users-0.9.3/badi_users.egg-info/
--rw-rw-rw-   0        0        0      419 2023-04-11 07:16:25.000000 badi_users-0.9.3/badi_users.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    10750 2023-04-11 07:16:25.000000 badi_users-0.9.3/badi_users.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-11 07:16:25.000000 badi_users-0.9.3/badi_users.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-04-11 07:16:25.000000 badi_users-0.9.3/badi_users.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-11 07:16:26.078262 badi_users-0.9.3/badi_utils/
--rw-rw-rw-   0        0        0        0 2022-09-24 05:54:56.000000 badi_users-0.9.3/badi_utils/__init__.py
--rw-rw-rw-   0        0        0     6835 2022-09-24 08:08:59.000000 badi_users-0.9.3/badi_utils/date_calc.py
--rw-rw-rw-   0        0        0    28225 2023-01-30 19:13:21.000000 badi_users-0.9.3/badi_utils/dynamic.py
--rw-rw-rw-   0        0        0    22478 2022-12-03 08:13:14.000000 badi_users-0.9.3/badi_utils/dynamic_api.py
--rw-rw-rw-   0        0        0     3412 2022-10-29 14:49:57.000000 badi_users-0.9.3/badi_utils/dynamic_models.py
--rw-rw-rw-   0        0        0     2990 2022-09-26 04:39:36.000000 badi_users-0.9.3/badi_utils/email.py
--rw-rw-rw-   0        0        0      252 2022-09-26 05:16:38.000000 badi_users-0.9.3/badi_utils/errors.py
--rw-rw-rw-   0        0        0     1509 2022-11-12 15:50:44.000000 badi_users-0.9.3/badi_utils/logging.py
--rw-rw-rw-   0        0        0      947 2022-08-06 18:28:12.000000 badi_users-0.9.3/badi_utils/responses.py
--rw-rw-rw-   0        0        0      904 2023-02-06 12:51:34.000000 badi_users-0.9.3/badi_utils/rss.py
--rw-rw-rw-   0        0        0     1529 2022-09-24 12:31:48.000000 badi_users-0.9.3/badi_utils/select2.py
--rw-rw-rw-   0        0        0     2132 2023-03-27 18:55:33.000000 badi_users-0.9.3/badi_utils/sms.py
-drwxrwxrwx   0        0        0        0 2023-04-11 07:16:25.995759 badi_users-0.9.3/badi_utils/static/
-drwxrwxrwx   0        0        0        0 2023-04-11 07:16:25.996756 badi_users-0.9.3/badi_utils/static/badi_utils/
-drwxrwxrwx   0        0        0        0 2023-04-11 07:16:26.079259 badi_users-0.9.3/badi_utils/static/badi_utils/css/
--rw-rw-rw-   0        0        0    40504 2023-01-30 18:56:15.000000 badi_users-0.9.3/badi_utils/static/badi_utils/css/custom.css
-drwxrwxrwx   0        0        0        0 2023-04-11 07:16:26.127222 badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/
--rw-rw-rw-   0        0        0    59778 2022-08-14 04:14:25.000000 badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).eot
--rw-rw-rw-   0        0        0    59532 2022-08-14 04:14:25.000000 badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).ttf
--rw-rw-rw-   0        0        0    38401 2022-08-14 04:14:25.000000 badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).woff
--rw-rw-rw-   0        0        0    31304 2022-08-14 04:14:25.000000 badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).woff2
--rw-rw-rw-   0        0        0    59778 2022-08-14 04:14:25.000000 badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_2.eot
--rw-rw-rw-   0        0        0    31992 2022-08-14 04:14:25.000000 badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.eot
--rw-rw-rw-   0        0        0    57268 2022-08-14 04:14:26.000000 badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.ttf
--rw-rw-rw-   0        0        0    36069 2022-08-14 04:14:26.000000 badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.woff
--rw-rw-rw-   0        0        0    28856 2022-08-14 04:14:26.000000 badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.woff2
--rw-rw-rw-   0        0        0    31992 2022-08-14 04:14:26.000000 badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold_2.eot
--rw-rw-rw-   0        0        0    35477 2022-08-14 04:14:26.000000 badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.eot
--rw-rw-rw-   0        0        0    60584 2022-08-14 04:14:26.000000 badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.ttf
--rw-rw-rw-   0        0        0    39557 2022-08-14 04:14:26.000000 badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.woff
--rw-rw-rw-   0        0        0    32344 2022-08-14 04:14:26.000000 badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.woff2
--rw-rw-rw-   0        0        0    35477 2022-08-14 04:14:26.000000 badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light_2.eot
--rw-rw-rw-   0        0        0    32043 2022-08-14 04:14:26.000000 badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.eot
--rw-rw-rw-   0        0        0    58192 2022-08-14 04:14:26.000000 badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.ttf
--rw-rw-rw-   0        0        0    36145 2022-08-14 04:14:26.000000 badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.woff
--rw-rw-rw-   0        0        0    28912 2022-08-14 04:14:26.000000 badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.woff2
--rw-rw-rw-   0        0        0    32043 2022-08-14 04:14:26.000000 badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium_2.eot
--rw-rw-rw-   0        0        0    33102 2022-08-14 04:14:26.000000 badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.eot
--rw-rw-rw-   0        0        0    56352 2022-08-14 04:14:26.000000 badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.ttf
--rw-rw-rw-   0        0        0    36913 2022-08-14 04:14:26.000000 badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.woff
--rw-rw-rw-   0        0        0    30072 2022-08-14 04:14:26.000000 badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.woff2
--rw-rw-rw-   0        0        0    33102 2022-08-14 04:14:26.000000 badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight_2.eot
--rw-rw-rw-   0        0        0    58886 2022-08-14 04:14:26.000000 badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb.eot
--rw-rw-rw-   0        0        0    38473 2022-08-14 04:14:26.000000 badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb.woff
--rw-rw-rw-   0        0        0    31320 2022-08-14 04:14:26.000000 badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb.woff2
--rw-rw-rw-   0        0        0    58886 2022-08-14 04:14:26.000000 badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_2.eot
--rw-rw-rw-   0        0        0    57974 2022-08-14 04:14:26.000000 badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.eot
--rw-rw-rw-   0        0        0    57760 2022-08-14 04:14:26.000000 badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.ttf
--rw-rw-rw-   0        0        0    36629 2022-08-14 04:14:26.000000 badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.woff
--rw-rw-rw-   0        0        0    29688 2022-08-14 04:14:26.000000 badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.woff2
--rw-rw-rw-   0        0        0    57974 2022-08-14 04:14:26.000000 badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold_2.eot
--rw-rw-rw-   0        0        0    57974 2022-08-14 04:14:26.000000 badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold_3.eot
--rw-rw-rw-   0        0        0    35458 2022-08-14 04:14:26.000000 badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.eot
--rw-rw-rw-   0        0        0    59968 2022-08-14 04:14:26.000000 badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.ttf
--rw-rw-rw-   0        0        0    39693 2022-08-14 04:14:26.000000 badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.woff
--rw-rw-rw-   0        0        0    32420 2022-08-14 04:14:26.000000 badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.woff2
--rw-rw-rw-   0        0        0    35458 2022-08-14 04:14:26.000000 badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light_2.eot
--rw-rw-rw-   0        0        0    31983 2022-08-14 04:14:26.000000 badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.eot
--rw-rw-rw-   0        0        0    57544 2022-08-14 04:14:26.000000 badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.ttf
--rw-rw-rw-   0        0        0    36141 2022-08-14 04:14:26.000000 badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.woff
--rw-rw-rw-   0        0        0    28916 2022-08-14 04:14:26.000000 badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.woff2
--rw-rw-rw-   0        0        0    31983 2022-08-14 04:14:26.000000 badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium_2.eot
--rw-rw-rw-   0        0        0    33044 2022-08-14 04:14:26.000000 badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.eot
--rw-rw-rw-   0        0        0    55640 2022-08-14 04:14:26.000000 badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.ttf
--rw-rw-rw-   0        0        0    36945 2022-08-14 04:14:26.000000 badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.woff
--rw-rw-rw-   0        0        0    29840 2022-08-14 04:14:26.000000 badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.woff2
--rw-rw-rw-   0        0        0    33044 2022-08-14 04:14:26.000000 badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight_2.eot
--rw-rw-rw-   0        0        0    93376 2022-08-14 04:14:26.000000 badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/Ray-Black.ttf
--rw-rw-rw-   0        0        0    94304 2022-08-14 04:14:26.000000 badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/Ray-Bold.ttf
--rw-rw-rw-   0        0        0    94740 2022-08-14 04:14:26.000000 badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/Ray.ttf
-drwxrwxrwx   0        0        0        0 2023-04-11 07:16:26.140189 badi_users-0.9.3/badi_utils/static/badi_utils/js/
--rw-rw-rw-   0        0        0   478686 2023-01-03 13:51:41.000000 badi_users-0.9.3/badi_utils/static/badi_utils/js/apexchart.js
--rw-rw-rw-   0        0        0    19110 2022-08-14 04:14:25.000000 badi_users-0.9.3/badi_utils/static/badi_utils/js/api-login.js
--rw-rw-rw-   0        0        0    20445 2022-12-01 13:15:11.000000 badi_users-0.9.3/badi_utils/static/badi_utils/js/api.js
--rw-rw-rw-   0        0        0    25944 2023-03-29 06:15:03.000000 badi_users-0.9.3/badi_utils/static/badi_utils/js/base.js
--rw-rw-rw-   0        0        0     2149 2022-08-14 04:14:25.000000 badi_users-0.9.3/badi_utils/static/badi_utils/js/chat.js
--rw-rw-rw-   0        0        0     3167 2022-08-14 04:14:25.000000 badi_users-0.9.3/badi_utils/static/badi_utils/js/custom-vue.js
--rw-rw-rw-   0        0        0    18560 2023-03-27 14:51:58.000000 badi_users-0.9.3/badi_utils/static/badi_utils/js/datatable.js
--rw-rw-rw-   0        0        0     2470 2022-08-15 18:25:55.000000 badi_users-0.9.3/badi_utils/static/badi_utils/js/image-field.js
--rw-rw-rw-   0        0        0    30541 2023-03-29 06:13:24.000000 badi_users-0.9.3/badi_utils/static/badi_utils/js/main.js
--rw-rw-rw-   0        0        0      959 2022-08-14 04:14:26.000000 badi_users-0.9.3/badi_utils/static/badi_utils/js/notification.js
--rw-rw-rw-   0        0        0     2213 2022-08-14 04:14:26.000000 badi_users-0.9.3/badi_utils/static/badi_utils/js/pagination-vue.js
--rw-rw-rw-   0        0        0    20317 2023-03-30 04:45:54.000000 badi_users-0.9.3/badi_utils/static/badi_utils/js/tableexport.js
--rw-rw-rw-   0        0        0      654 2022-08-14 04:14:26.000000 badi_users-0.9.3/badi_utils/static/badi_utils/js/transaction.js
--rw-rw-rw-   0        0        0   354110 2022-08-14 04:14:26.000000 badi_users-0.9.3/badi_utils/static/badi_utils/js/vue.js
--rw-rw-rw-   0        0        0   268386 2023-03-30 05:07:06.000000 badi_users-0.9.3/badi_utils/static/badi_utils/js/xlsx.mini.min.js
-drwxrwxrwx   0        0        0        0 2023-04-11 07:16:26.142183 badi_users-0.9.3/badi_utils/templates/
--rw-rw-rw-   0        0        0        0 2022-09-24 07:28:02.000000 badi_users-0.9.3/badi_utils/templates/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 07:16:26.160221 badi_users-0.9.3/badi_utils/templates/component/
--rw-rw-rw-   0        0        0     1777 2022-10-25 06:27:38.000000 badi_users-0.9.3/badi_utils/templates/component/createModal.html
--rw-rw-rw-   0        0        0     1645 2022-08-14 04:14:27.000000 badi_users-0.9.3/badi_utils/templates/component/createTitle.html
--rw-rw-rw-   0        0        0     1054 2022-08-14 04:14:27.000000 badi_users-0.9.3/badi_utils/templates/component/filter-form.html
--rw-rw-rw-   0        0        0      729 2022-08-14 04:14:27.000000 badi_users-0.9.3/badi_utils/templates/component/form-errors.html
--rw-rw-rw-   0        0        0     1340 2022-08-14 04:14:27.000000 badi_users-0.9.3/badi_utils/templates/component/form-progressbar-js.html
--rw-rw-rw-   0        0        0      491 2022-08-14 04:14:27.000000 badi_users-0.9.3/badi_utils/templates/component/form-progressbar.html
--rw-rw-rw-   0        0        0      342 2022-08-14 04:14:27.000000 badi_users-0.9.3/badi_utils/templates/component/form.html
--rw-rw-rw-   0        0        0     1231 2022-08-14 04:14:27.000000 badi_users-0.9.3/badi_utils/templates/component/image-field.html
--rw-rw-rw-   0        0        0    34439 2022-08-14 04:14:27.000000 badi_users-0.9.3/badi_utils/templates/component/index-menu.html
--rw-rw-rw-   0        0        0     2346 2022-08-14 04:14:27.000000 badi_users-0.9.3/badi_utils/templates/component/input.html
--rw-rw-rw-   0        0        0       69 2022-08-14 04:14:27.000000 badi_users-0.9.3/badi_utils/templates/component/loader.html
--rw-rw-rw-   0        0        0      468 2022-10-02 09:59:19.000000 badi_users-0.9.3/badi_utils/templates/component/menu-item.html
--rw-rw-rw-   0        0        0      362 2022-10-02 09:59:19.000000 badi_users-0.9.3/badi_utils/templates/component/menu-list.html
--rw-rw-rw-   0        0        0      746 2022-08-14 04:14:27.000000 badi_users-0.9.3/badi_utils/templates/component/messages.html
--rw-rw-rw-   0        0        0     1134 2022-12-31 05:14:56.000000 badi_users-0.9.3/badi_utils/templates/component/pagination-vue.html
--rw-rw-rw-   0        0        0      361 2022-08-14 04:14:27.000000 badi_users-0.9.3/badi_utils/templates/component/profile_item.html
--rw-rw-rw-   0        0        0      204 2022-08-14 04:14:27.000000 badi_users-0.9.3/badi_utils/templates/component/space-between.html
--rw-rw-rw-   0        0        0      430 2022-10-02 09:59:19.000000 badi_users-0.9.3/badi_utils/templates/component/svg-button-with-text.html
--rw-rw-rw-   0        0        0      428 2022-10-02 09:59:19.000000 badi_users-0.9.3/badi_utils/templates/component/svg-button.html
--rw-rw-rw-   0        0        0     1411 2022-08-14 04:14:27.000000 badi_users-0.9.3/badi_utils/templates/component/table-item.html
--rw-rw-rw-   0        0        0     2114 2022-08-14 04:14:27.000000 badi_users-0.9.3/badi_utils/templates/component/user-card.html
--rw-rw-rw-   0        0        0      257 2022-08-14 04:14:27.000000 badi_users-0.9.3/badi_utils/templates/component/yesno.html
-drwxrwxrwx   0        0        0        0 2023-04-11 07:16:26.207081 badi_users-0.9.3/badi_utils/templates/svg/
--rw-rw-rw-   0        0        0     1949 2022-08-06 18:28:13.000000 badi_users-0.9.3/badi_utils/templates/svg/Incoming-box.html
--rw-rw-rw-   0        0        0     1159 2022-08-06 18:28:13.000000 badi_users-0.9.3/badi_utils/templates/svg/add-user.html
--rw-rw-rw-   0        0        0     1092 2022-08-06 18:28:13.000000 badi_users-0.9.3/badi_utils/templates/svg/address-book.html
--rw-rw-rw-   0        0        0     1095 2022-08-06 18:28:13.000000 badi_users-0.9.3/badi_utils/templates/svg/arrow-left.html
--rw-rw-rw-   0        0        0     1081 2022-08-06 18:28:13.000000 badi_users-0.9.3/badi_utils/templates/svg/arrow-right.html
--rw-rw-rw-   0        0        0     2024 2022-08-14 04:14:27.000000 badi_users-0.9.3/badi_utils/templates/svg/bitcoin.html
--rw-rw-rw-   0        0        0      697 2022-08-06 18:28:13.000000 badi_users-0.9.3/badi_utils/templates/svg/box.html
--rw-rw-rw-   0        0        0     1378 2022-08-06 18:28:13.000000 badi_users-0.9.3/badi_utils/templates/svg/calendar-day.html
--rw-rw-rw-   0        0        0     1489 2022-08-06 18:28:13.000000 badi_users-0.9.3/badi_utils/templates/svg/calendar-gym.html
--rw-rw-rw-   0        0        0      925 2022-08-06 18:28:13.000000 badi_users-0.9.3/badi_utils/templates/svg/calendar.html
--rw-rw-rw-   0        0        0     1223 2022-12-01 08:20:56.000000 badi_users-0.9.3/badi_utils/templates/svg/call.html
--rw-rw-rw-   0        0        0     1385 2022-08-06 18:28:13.000000 badi_users-0.9.3/badi_utils/templates/svg/category.html
--rw-rw-rw-   0        0        0     1270 2022-08-14 04:14:27.000000 badi_users-0.9.3/badi_utils/templates/svg/chat.html
--rw-rw-rw-   0        0        0      938 2022-08-06 18:28:13.000000 badi_users-0.9.3/badi_utils/templates/svg/check.html
--rw-rw-rw-   0        0        0      344 2022-08-06 18:28:13.000000 badi_users-0.9.3/badi_utils/templates/svg/circle.html
--rw-rw-rw-   0        0        0     1686 2022-08-06 18:28:13.000000 badi_users-0.9.3/badi_utils/templates/svg/city.html
--rw-rw-rw-   0        0        0     1430 2022-08-06 18:28:13.000000 badi_users-0.9.3/badi_utils/templates/svg/clipboard-list.html
--rw-rw-rw-   0        0        0     2247 2022-08-06 18:28:13.000000 badi_users-0.9.3/badi_utils/templates/svg/clock.html
--rw-rw-rw-   0        0        0      645 2022-08-06 18:28:13.000000 badi_users-0.9.3/badi_utils/templates/svg/close.html
--rw-rw-rw-   0        0        0     2483 2022-08-06 18:28:13.000000 badi_users-0.9.3/badi_utils/templates/svg/collection.html
--rw-rw-rw-   0        0        0     1046 2022-08-14 04:14:27.000000 badi_users-0.9.3/badi_utils/templates/svg/comment.html
--rw-rw-rw-   0        0        0     1103 2022-08-06 18:28:13.000000 badi_users-0.9.3/badi_utils/templates/svg/dashboard.html
--rw-rw-rw-   0        0        0      893 2022-08-06 18:28:13.000000 badi_users-0.9.3/badi_utils/templates/svg/delete.html
--rw-rw-rw-   0        0        0     1505 2022-08-06 18:28:13.000000 badi_users-0.9.3/badi_utils/templates/svg/download.html
--rw-rw-rw-   0        0        0      901 2022-08-06 18:28:13.000000 badi_users-0.9.3/badi_utils/templates/svg/edit.html
--rw-rw-rw-   0        0        0     1361 2022-08-06 18:28:13.000000 badi_users-0.9.3/badi_utils/templates/svg/file-check.html
--rw-rw-rw-   0        0        0      988 2022-08-06 18:28:13.000000 badi_users-0.9.3/badi_utils/templates/svg/file.html
--rw-rw-rw-   0        0        0     2111 2022-08-06 18:28:13.000000 badi_users-0.9.3/badi_utils/templates/svg/film.html
--rw-rw-rw-   0        0        0      681 2022-08-14 04:14:27.000000 badi_users-0.9.3/badi_utils/templates/svg/fire.html
--rw-rw-rw-   0        0        0     1648 2022-08-06 18:28:13.000000 badi_users-0.9.3/badi_utils/templates/svg/group-chat.html
--rw-rw-rw-   0        0        0     1213 2022-08-06 18:28:13.000000 badi_users-0.9.3/badi_utils/templates/svg/group.html
--rw-rw-rw-   0        0        0     1394 2022-08-14 04:14:27.000000 badi_users-0.9.3/badi_utils/templates/svg/half_star.html
--rw-rw-rw-   0        0        0      944 2022-08-06 18:28:13.000000 badi_users-0.9.3/badi_utils/templates/svg/home.html
--rw-rw-rw-   0        0        0     1906 2022-08-14 04:14:27.000000 badi_users-0.9.3/badi_utils/templates/svg/hourse.html
--rw-rw-rw-   0        0        0      631 2022-08-06 18:28:13.000000 badi_users-0.9.3/badi_utils/templates/svg/image.html
--rw-rw-rw-   0        0        0      508 2022-08-06 18:28:13.000000 badi_users-0.9.3/badi_utils/templates/svg/info.html
--rw-rw-rw-   0        0        0     1394 2022-08-06 18:28:13.000000 badi_users-0.9.3/badi_utils/templates/svg/interview.html
--rw-rw-rw-   0        0        0     1389 2022-08-06 18:28:13.000000 badi_users-0.9.3/badi_utils/templates/svg/key.html
--rw-rw-rw-   0        0        0     2472 2022-08-06 18:28:13.000000 badi_users-0.9.3/badi_utils/templates/svg/logout.html
--rw-rw-rw-   0        0        0      940 2022-08-14 04:14:27.000000 badi_users-0.9.3/badi_utils/templates/svg/mail.html
--rw-rw-rw-   0        0        0      731 2022-08-06 18:28:13.000000 badi_users-0.9.3/badi_utils/templates/svg/map.html
--rw-rw-rw-   0        0        0     1601 2022-08-06 18:28:13.000000 badi_users-0.9.3/badi_utils/templates/svg/message.html
--rw-rw-rw-   0        0        0     1607 2022-08-06 18:28:13.000000 badi_users-0.9.3/badi_utils/templates/svg/messages.html
--rw-rw-rw-   0        0        0      683 2022-08-14 04:14:27.000000 badi_users-0.9.3/badi_utils/templates/svg/notification.html
--rw-rw-rw-   0        0        0      708 2022-08-06 18:28:13.000000 badi_users-0.9.3/badi_utils/templates/svg/plus.html
--rw-rw-rw-   0        0        0      753 2022-08-14 04:14:27.000000 badi_users-0.9.3/badi_utils/templates/svg/puzzle.html
--rw-rw-rw-   0        0        0      882 2022-08-14 04:14:27.000000 badi_users-0.9.3/badi_utils/templates/svg/question.html
--rw-rw-rw-   0        0        0     1174 2022-08-06 18:28:13.000000 badi_users-0.9.3/badi_utils/templates/svg/refresh.html
--rw-rw-rw-   0        0        0     1416 2022-08-06 18:28:13.000000 badi_users-0.9.3/badi_utils/templates/svg/safe.html
--rw-rw-rw-   0        0        0     1091 2022-09-21 07:25:46.000000 badi_users-0.9.3/badi_utils/templates/svg/search.html
--rw-rw-rw-   0        0        0     1114 2022-08-06 18:28:13.000000 badi_users-0.9.3/badi_utils/templates/svg/shield-protected.html
--rw-rw-rw-   0        0        0     1219 2022-08-06 18:28:13.000000 badi_users-0.9.3/badi_utils/templates/svg/shield-user.html
--rw-rw-rw-   0        0        0      451 2022-08-06 18:28:13.000000 badi_users-0.9.3/badi_utils/templates/svg/slide.html
--rw-rw-rw-   0        0        0     1587 2022-08-06 18:28:13.000000 badi_users-0.9.3/badi_utils/templates/svg/timer.html
--rw-rw-rw-   0        0        0     1043 2022-08-06 18:28:13.000000 badi_users-0.9.3/badi_utils/templates/svg/town.html
--rw-rw-rw-   0        0        0      804 2022-08-06 18:28:13.000000 badi_users-0.9.3/badi_utils/templates/svg/user.html
--rw-rw-rw-   0        0        0      936 2022-08-06 18:28:13.000000 badi_users-0.9.3/badi_utils/templates/svg/wallet.html
--rw-rw-rw-   0        0        0      933 2022-08-06 18:28:13.000000 badi_users-0.9.3/badi_utils/templates/svg/warning.html
--rw-rw-rw-   0        0        0       19 2022-09-27 11:24:17.000000 badi_users-0.9.3/badi_utils/templates/test.html
-drwxrwxrwx   0        0        0        0 2023-04-11 07:16:26.209081 badi_users-0.9.3/badi_utils/templatetags/
--rw-rw-rw-   0        0        0        0 2022-09-24 07:28:02.000000 badi_users-0.9.3/badi_utils/templatetags/__init__.py
--rw-rw-rw-   0        0        0      148 2022-09-27 11:23:20.000000 badi_users-0.9.3/badi_utils/templatetags/badi_utils.py
--rw-rw-rw-   0        0        0     7102 2023-02-16 09:10:01.000000 badi_users-0.9.3/badi_utils/utils.py
--rw-rw-rw-   0        0        0     1911 2022-09-26 05:21:35.000000 badi_users-0.9.3/badi_utils/validations.py
-drwxrwxrwx   0        0        0        0 2023-04-11 07:16:26.212074 badi_users-0.9.3/badi_visit/
--rw-rw-rw-   0        0        0        0 2022-08-14 04:14:27.000000 badi_users-0.9.3/badi_visit/__init__.py
--rw-rw-rw-   0        0        0      167 2022-11-10 16:59:20.000000 badi_users-0.9.3/badi_visit/admin.py
-drwxrwxrwx   0        0        0        0 2023-04-11 07:16:26.214068 badi_users-0.9.3/badi_visit/api/
--rw-rw-rw-   0        0        0        0 2022-10-24 15:37:24.000000 badi_users-0.9.3/badi_visit/api/__init__.py
--rw-rw-rw-   0        0        0     2871 2022-11-10 16:59:20.000000 badi_users-0.9.3/badi_visit/api/api.py
--rw-rw-rw-   0        0        0      208 2022-11-10 16:59:20.000000 badi_users-0.9.3/badi_visit/api/routers.py
--rw-rw-rw-   0        0        0      185 2022-11-10 16:59:20.000000 badi_users-0.9.3/badi_visit/apps.py
-drwxrwxrwx   0        0        0        0 2023-04-11 07:16:26.215065 badi_users-0.9.3/badi_visit/migrations/
--rw-rw-rw-   0        0        0        0 2022-08-14 04:14:27.000000 badi_users-0.9.3/badi_visit/migrations/__init__.py
--rw-rw-rw-   0        0        0     1614 2022-11-10 16:59:20.000000 badi_users-0.9.3/badi_visit/models.py
--rw-rw-rw-   0        0        0       63 2022-08-14 04:14:27.000000 badi_users-0.9.3/badi_visit/tests.py
-drwxrwxrwx   0        0        0        0 2023-04-11 07:16:26.220053 badi_users-0.9.3/badi_wallet/
--rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.3/badi_wallet/__init__.py
--rw-rw-rw-   0        0        0     8873 2023-03-27 19:00:31.000000 badi_users-0.9.3/badi_wallet/action.py
--rw-rw-rw-   0        0        0      202 2023-03-27 19:00:31.000000 badi_users-0.9.3/badi_wallet/admin.py
-drwxrwxrwx   0        0        0        0 2023-04-11 07:16:26.223597 badi_users-0.9.3/badi_wallet/api/
--rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.3/badi_wallet/api/__init__.py
--rw-rw-rw-   0        0        0      241 2023-03-27 19:00:31.000000 badi_users-0.9.3/badi_wallet/api/routers.py
--rw-rw-rw-   0        0        0      543 2023-03-27 19:00:31.000000 badi_users-0.9.3/badi_wallet/api/serializers.py
--rw-rw-rw-   0        0        0     8037 2023-03-29 08:19:18.000000 badi_users-0.9.3/badi_wallet/api/view_sets.py
--rw-rw-rw-   0        0        0      243 2023-03-27 19:00:31.000000 badi_users-0.9.3/badi_wallet/apps.py
--rw-rw-rw-   0        0        0      350 2023-03-28 19:16:55.000000 badi_users-0.9.3/badi_wallet/filter.py
-drwxrwxrwx   0        0        0        0 2023-04-11 07:16:25.999748 badi_users-0.9.3/badi_wallet/locale/
-drwxrwxrwx   0        0        0        0 2023-04-11 07:16:25.999748 badi_users-0.9.3/badi_wallet/locale/fa/
-drwxrwxrwx   0        0        0        0 2023-04-11 07:16:26.224594 badi_users-0.9.3/badi_wallet/locale/fa/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1633 2023-04-11 06:17:23.000000 badi_users-0.9.3/badi_wallet/locale/fa/LC_MESSAGES/django.mo
-drwxrwxrwx   0        0        0        0 2023-04-11 07:16:26.225592 badi_users-0.9.3/badi_wallet/migrations/
--rw-rw-rw-   0        0        0        0 2022-08-06 18:28:13.000000 badi_users-0.9.3/badi_wallet/migrations/__init__.py
--rw-rw-rw-   0        0        0     3146 2023-03-30 05:05:34.000000 badi_users-0.9.3/badi_wallet/models.py
-drwxrwxrwx   0        0        0        0 2023-04-11 07:16:26.225592 badi_users-0.9.3/badi_wallet/templates/
--rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.3/badi_wallet/templates/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-11 07:16:26.229581 badi_users-0.9.3/badi_wallet/templates/transaction/
--rw-rw-rw-   0        0        0     6145 2023-03-29 08:22:24.000000 badi_users-0.9.3/badi_wallet/templates/transaction/all_transaction_list.html
--rw-rw-rw-   0        0        0    10786 2023-03-30 06:06:40.000000 badi_users-0.9.3/badi_wallet/templates/transaction/all_transaction_report.html
--rw-rw-rw-   0        0        0     2251 2023-03-27 19:00:31.000000 badi_users-0.9.3/badi_wallet/templates/transaction/request-transaction.html
--rw-rw-rw-   0        0        0     6203 2023-03-29 08:22:11.000000 badi_users-0.9.3/badi_wallet/templates/transaction/transaction_list.html
--rw-rw-rw-   0        0        0     3547 2023-03-27 19:00:31.000000 badi_users-0.9.3/badi_wallet/templates/transaction/transaction_result.html
--rw-rw-rw-   0        0        0       63 2023-03-27 19:00:31.000000 badi_users-0.9.3/badi_wallet/tests.py
-drwxrwxrwx   0        0        0        0 2023-04-11 07:16:26.231575 badi_users-0.9.3/badi_wallet/ui/
--rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.3/badi_wallet/ui/__init__.py
--rw-rw-rw-   0        0        0      577 2023-03-28 19:11:37.000000 badi_users-0.9.3/badi_wallet/ui/urls.py
--rw-rw-rw-   0        0        0     1449 2023-03-28 19:16:42.000000 badi_users-0.9.3/badi_wallet/ui/views.py
--rw-rw-rw-   0        0        0       42 2023-04-11 07:16:26.233570 badi_users-0.9.3/setup.cfg
--rw-rw-rw-   0        0        0      498 2023-04-11 07:16:09.000000 badi_users-0.9.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 12:32:09.493437 badi_users-0.9.4/
+-rw-rw-rw-   0        0        0     1093 2022-09-24 06:05:13.000000 badi_users-0.9.4/LICENSE
+-rw-rw-rw-   0        0        0     1066 2022-11-10 17:03:20.000000 badi_users-0.9.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      419 2023-04-16 12:32:09.492437 badi_users-0.9.4/PKG-INFO
+-rw-rw-rw-   0        0        0      143 2022-10-02 09:04:41.000000 badi_users-0.9.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-16 12:32:09.282639 badi_users-0.9.4/badi_ticket/
+-rw-rw-rw-   0        0        0        0 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_ticket/__init__.py
+-rw-rw-rw-   0        0        0      143 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_ticket/admin.py
+-rw-rw-rw-   0        0        0     9803 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_ticket/api.py
+-rw-rw-rw-   0        0        0      129 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_ticket/apps.py
+drwxrwxrwx   0        0        0        0 2023-04-16 12:32:09.254712 badi_users-0.9.4/badi_ticket/locale/
+drwxrwxrwx   0        0        0        0 2023-04-16 12:32:09.254712 badi_users-0.9.4/badi_ticket/locale/fa/
+drwxrwxrwx   0        0        0        0 2023-04-16 12:32:09.283635 badi_users-0.9.4/badi_ticket/locale/fa/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     2781 2023-04-16 12:25:05.000000 badi_users-0.9.4/badi_ticket/locale/fa/LC_MESSAGES/django.mo
+drwxrwxrwx   0        0        0        0 2023-04-16 12:32:09.283635 badi_users-0.9.4/badi_ticket/migrations/
+-rw-rw-rw-   0        0        0        0 2022-08-06 18:28:13.000000 badi_users-0.9.4/badi_ticket/migrations/__init__.py
+-rw-rw-rw-   0        0        0     3657 2023-04-16 09:10:44.000000 badi_users-0.9.4/badi_ticket/models.py
+-rw-rw-rw-   0        0        0      313 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_ticket/routers.py
+-rw-rw-rw-   0        0        0     2082 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_ticket/serializers.py
+drwxrwxrwx   0        0        0        0 2023-04-16 12:32:09.255710 badi_users-0.9.4/badi_ticket/static/
+drwxrwxrwx   0        0        0        0 2023-04-16 12:32:09.256708 badi_users-0.9.4/badi_ticket/static/ticket/
+drwxrwxrwx   0        0        0        0 2023-04-16 12:32:09.284632 badi_users-0.9.4/badi_ticket/static/ticket/js/
+-rw-rw-rw-   0        0        0     2448 2023-04-16 09:16:22.000000 badi_users-0.9.4/badi_ticket/static/ticket/js/chat.js
+drwxrwxrwx   0        0        0        0 2023-04-16 12:32:09.285629 badi_users-0.9.4/badi_ticket/templates/
+-rw-rw-rw-   0        0        0        0 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_ticket/templates/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 12:32:09.290161 badi_users-0.9.4/badi_ticket/templates/ticket/
+-rw-rw-rw-   0        0        0     6358 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_ticket/templates/ticket/admin_tickets.html
+-rw-rw-rw-   0        0        0     5265 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_ticket/templates/ticket/message_list.html
+-rw-rw-rw-   0        0        0     9642 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_ticket/templates/ticket/my_tickets.html
+-rw-rw-rw-   0        0        0     7097 2023-04-16 08:20:08.000000 badi_users-0.9.4/badi_ticket/templates/ticket/ticket_create.html
+-rw-rw-rw-   0        0        0     1639 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_ticket/templates/ticket/ticket_update.html
+-rw-rw-rw-   0        0        0       63 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_ticket/tests.py
+-rw-rw-rw-   0        0        0      583 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_ticket/urls.py
+-rw-rw-rw-   0        0        0     2057 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_ticket/views.py
+drwxrwxrwx   0        0        0        0 2023-04-16 12:32:09.294658 badi_users-0.9.4/badi_user/
+-rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.4/badi_user/__init__.py
+-rw-rw-rw-   0        0        0      166 2023-03-27 19:00:31.000000 badi_users-0.9.4/badi_user/admin.py
+drwxrwxrwx   0        0        0        0 2023-04-16 12:32:09.297649 badi_users-0.9.4/badi_user/api/
+-rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.4/badi_user/api/__init__.py
+-rw-rw-rw-   0        0        0    29106 2023-04-16 11:46:57.000000 badi_users-0.9.4/badi_user/api/api.py
+-rw-rw-rw-   0        0        0      485 2023-03-27 19:00:31.000000 badi_users-0.9.4/badi_user/api/routers.py
+-rw-rw-rw-   0        0        0     6013 2023-03-27 19:00:31.000000 badi_users-0.9.4/badi_user/api/serializers.py
+-rw-rw-rw-   0        0        0      183 2023-03-27 19:00:31.000000 badi_users-0.9.4/badi_user/apps.py
+-rw-rw-rw-   0        0        0     3428 2023-03-27 19:00:31.000000 badi_users-0.9.4/badi_user/filter.py
+drwxrwxrwx   0        0        0        0 2023-04-16 12:32:09.258701 badi_users-0.9.4/badi_user/locale/
+drwxrwxrwx   0        0        0        0 2023-04-16 12:32:09.258701 badi_users-0.9.4/badi_user/locale/fa/
+drwxrwxrwx   0        0        0        0 2023-04-16 12:32:09.298645 badi_users-0.9.4/badi_user/locale/fa/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     4486 2023-04-16 12:25:06.000000 badi_users-0.9.4/badi_user/locale/fa/LC_MESSAGES/django.mo
+drwxrwxrwx   0        0        0        0 2023-04-16 12:32:09.299642 badi_users-0.9.4/badi_user/migrations/
+-rw-rw-rw-   0        0        0        0 2022-08-06 18:28:13.000000 badi_users-0.9.4/badi_user/migrations/__init__.py
+-rw-rw-rw-   0        0        0     6551 2023-03-27 19:00:31.000000 badi_users-0.9.4/badi_user/models.py
+drwxrwxrwx   0        0        0        0 2023-04-16 12:32:09.300639 badi_users-0.9.4/badi_user/templates/
+-rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.4/badi_user/templates/__init__.py
+-rw-rw-rw-   0        0        0       27 2023-03-27 19:00:31.000000 badi_users-0.9.4/badi_user/templates/badi-user-test.html
+drwxrwxrwx   0        0        0        0 2023-04-16 12:32:09.301637 badi_users-0.9.4/badi_user/templates/group/
+-rw-rw-rw-   0        0        0     8558 2023-03-27 19:00:31.000000 badi_users-0.9.4/badi_user/templates/group/group_create.html
+-rw-rw-rw-   0        0        0     5472 2023-03-27 19:00:31.000000 badi_users-0.9.4/badi_user/templates/group/group_update.html
+drwxrwxrwx   0        0        0        0 2023-04-16 12:32:09.302635 badi_users-0.9.4/badi_user/templates/log/
+-rw-rw-rw-   0        0        0     3987 2023-03-27 19:00:31.000000 badi_users-0.9.4/badi_user/templates/log/log_list.html
+drwxrwxrwx   0        0        0        0 2023-04-16 12:32:09.303632 badi_users-0.9.4/badi_user/templates/login-theme/
+-rw-rw-rw-   0        0        0     7336 2023-03-27 19:00:31.000000 badi_users-0.9.4/badi_user/templates/login-theme/login-1.html
+drwxrwxrwx   0        0        0        0 2023-04-16 12:32:09.306625 badi_users-0.9.4/badi_user/templates/member/
+-rw-rw-rw-   0        0        0     6863 2023-03-27 19:00:31.000000 badi_users-0.9.4/badi_user/templates/member/member_create.html
+-rw-rw-rw-   0        0        0    22635 2023-03-27 19:00:31.000000 badi_users-0.9.4/badi_user/templates/member/member_list.html
+-rw-rw-rw-   0        0        0     4783 2023-03-28 07:29:01.000000 badi_users-0.9.4/badi_user/templates/member/member_self_update.html
+-rw-rw-rw-   0        0        0     6525 2023-03-27 19:00:31.000000 badi_users-0.9.4/badi_user/templates/member/member_update.html
+drwxrwxrwx   0        0        0        0 2023-04-16 12:32:09.309616 badi_users-0.9.4/badi_user/templates/user/
+-rw-rw-rw-   0        0        0     5056 2023-04-16 12:18:39.000000 badi_users-0.9.4/badi_user/templates/user/change_password.html
+-rw-rw-rw-   0        0        0     5973 2023-03-27 19:00:31.000000 badi_users-0.9.4/badi_user/templates/user/user_create.html
+-rw-rw-rw-   0        0        0     4019 2023-03-27 19:00:31.000000 badi_users-0.9.4/badi_user/templates/user/user_list.html
+-rw-rw-rw-   0        0        0     5005 2023-03-27 19:00:31.000000 badi_users-0.9.4/badi_user/templates/user/user_update.html
+drwxrwxrwx   0        0        0        0 2023-04-16 12:32:09.311610 badi_users-0.9.4/badi_user/templatetags/
+-rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.4/badi_user/templatetags/__init__.py
+-rw-rw-rw-   0        0        0     5950 2023-03-27 19:00:31.000000 badi_users-0.9.4/badi_user/templatetags/appfilter.py
+-rw-rw-rw-   0        0        0      500 2023-03-27 19:00:31.000000 badi_users-0.9.4/badi_user/tests.py
+drwxrwxrwx   0        0        0        0 2023-04-16 12:32:09.317423 badi_users-0.9.4/badi_user/ui/
+-rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.4/badi_user/ui/__init__.py
+-rw-rw-rw-   0        0        0     1484 2023-03-27 19:00:31.000000 badi_users-0.9.4/badi_user/ui/forms.py
+-rw-rw-rw-   0        0        0      320 2023-03-27 19:00:31.000000 badi_users-0.9.4/badi_user/ui/log_views.py
+-rw-rw-rw-   0        0        0     1706 2023-03-28 08:00:41.000000 badi_users-0.9.4/badi_user/ui/member_views.py
+-rw-rw-rw-   0        0        0      672 2023-03-27 19:00:31.000000 badi_users-0.9.4/badi_user/ui/notification_views.py
+-rw-rw-rw-   0        0        0      644 2023-03-27 19:00:31.000000 badi_users-0.9.4/badi_user/ui/roles_views.py
+-rw-rw-rw-   0        0        0     1624 2023-04-16 08:12:22.000000 badi_users-0.9.4/badi_user/ui/urls.py
+-rw-rw-rw-   0        0        0     2633 2023-03-27 19:00:31.000000 badi_users-0.9.4/badi_user/ui/views.py
+drwxrwxrwx   0        0        0        0 2023-04-16 12:32:09.332485 badi_users-0.9.4/badi_users.egg-info/
+-rw-rw-rw-   0        0        0      419 2023-04-16 12:32:09.000000 badi_users-0.9.4/badi_users.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    10750 2023-04-16 12:32:09.000000 badi_users-0.9.4/badi_users.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 12:32:09.000000 badi_users-0.9.4/badi_users.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-04-16 12:32:09.000000 badi_users-0.9.4/badi_users.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 12:32:09.344457 badi_users-0.9.4/badi_utils/
+-rw-rw-rw-   0        0        0        0 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/__init__.py
+-rw-rw-rw-   0        0        0     6835 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/date_calc.py
+-rw-rw-rw-   0        0        0    28225 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/dynamic.py
+-rw-rw-rw-   0        0        0    22478 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/dynamic_api.py
+-rw-rw-rw-   0        0        0     3412 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/dynamic_models.py
+-rw-rw-rw-   0        0        0     2990 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/email.py
+-rw-rw-rw-   0        0        0      252 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/errors.py
+-rw-rw-rw-   0        0        0     1509 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/logging.py
+-rw-rw-rw-   0        0        0      947 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/responses.py
+-rw-rw-rw-   0        0        0      904 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/rss.py
+-rw-rw-rw-   0        0        0     1529 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/select2.py
+-rw-rw-rw-   0        0        0     2956 2023-04-16 12:07:37.000000 badi_users-0.9.4/badi_utils/sms.py
+drwxrwxrwx   0        0        0        0 2023-04-16 12:32:09.263689 badi_users-0.9.4/badi_utils/static/
+drwxrwxrwx   0        0        0        0 2023-04-16 12:32:09.264688 badi_users-0.9.4/badi_utils/static/badi_utils/
+drwxrwxrwx   0        0        0        0 2023-04-16 12:32:09.345454 badi_users-0.9.4/badi_utils/static/badi_utils/css/
+-rw-rw-rw-   0        0        0    40504 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/css/custom.css
+drwxrwxrwx   0        0        0        0 2023-04-16 12:32:09.390334 badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/
+-rw-rw-rw-   0        0        0    59778 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).eot
+-rw-rw-rw-   0        0        0    59532 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).ttf
+-rw-rw-rw-   0        0        0    38401 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).woff
+-rw-rw-rw-   0        0        0    31304 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).woff2
+-rw-rw-rw-   0        0        0    59778 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_2.eot
+-rw-rw-rw-   0        0        0    31992 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.eot
+-rw-rw-rw-   0        0        0    57268 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.ttf
+-rw-rw-rw-   0        0        0    36069 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.woff
+-rw-rw-rw-   0        0        0    28856 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.woff2
+-rw-rw-rw-   0        0        0    31992 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold_2.eot
+-rw-rw-rw-   0        0        0    35477 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.eot
+-rw-rw-rw-   0        0        0    60584 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.ttf
+-rw-rw-rw-   0        0        0    39557 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.woff
+-rw-rw-rw-   0        0        0    32344 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.woff2
+-rw-rw-rw-   0        0        0    35477 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light_2.eot
+-rw-rw-rw-   0        0        0    32043 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.eot
+-rw-rw-rw-   0        0        0    58192 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.ttf
+-rw-rw-rw-   0        0        0    36145 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.woff
+-rw-rw-rw-   0        0        0    28912 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.woff2
+-rw-rw-rw-   0        0        0    32043 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium_2.eot
+-rw-rw-rw-   0        0        0    33102 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.eot
+-rw-rw-rw-   0        0        0    56352 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.ttf
+-rw-rw-rw-   0        0        0    36913 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.woff
+-rw-rw-rw-   0        0        0    30072 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.woff2
+-rw-rw-rw-   0        0        0    33102 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight_2.eot
+-rw-rw-rw-   0        0        0    58886 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb.eot
+-rw-rw-rw-   0        0        0    38473 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb.woff
+-rw-rw-rw-   0        0        0    31320 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb.woff2
+-rw-rw-rw-   0        0        0    58886 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_2.eot
+-rw-rw-rw-   0        0        0    57974 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.eot
+-rw-rw-rw-   0        0        0    57760 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.ttf
+-rw-rw-rw-   0        0        0    36629 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.woff
+-rw-rw-rw-   0        0        0    29688 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.woff2
+-rw-rw-rw-   0        0        0    57974 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold_2.eot
+-rw-rw-rw-   0        0        0    57974 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold_3.eot
+-rw-rw-rw-   0        0        0    35458 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.eot
+-rw-rw-rw-   0        0        0    59968 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.ttf
+-rw-rw-rw-   0        0        0    39693 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.woff
+-rw-rw-rw-   0        0        0    32420 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.woff2
+-rw-rw-rw-   0        0        0    35458 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light_2.eot
+-rw-rw-rw-   0        0        0    31983 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.eot
+-rw-rw-rw-   0        0        0    57544 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.ttf
+-rw-rw-rw-   0        0        0    36141 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.woff
+-rw-rw-rw-   0        0        0    28916 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.woff2
+-rw-rw-rw-   0        0        0    31983 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium_2.eot
+-rw-rw-rw-   0        0        0    33044 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.eot
+-rw-rw-rw-   0        0        0    55640 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.ttf
+-rw-rw-rw-   0        0        0    36945 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.woff
+-rw-rw-rw-   0        0        0    29840 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.woff2
+-rw-rw-rw-   0        0        0    33044 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight_2.eot
+-rw-rw-rw-   0        0        0    93376 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/Ray-Black.ttf
+-rw-rw-rw-   0        0        0    94304 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/Ray-Bold.ttf
+-rw-rw-rw-   0        0        0    94740 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/Ray.ttf
+drwxrwxrwx   0        0        0        0 2023-04-16 12:32:09.404297 badi_users-0.9.4/badi_utils/static/badi_utils/js/
+-rw-rw-rw-   0        0        0   478686 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/js/apexchart.js
+-rw-rw-rw-   0        0        0    19110 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/js/api-login.js
+-rw-rw-rw-   0        0        0    20445 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/js/api.js
+-rw-rw-rw-   0        0        0    25944 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/js/base.js
+-rw-rw-rw-   0        0        0     2149 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/js/chat.js
+-rw-rw-rw-   0        0        0     3167 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/js/custom-vue.js
+-rw-rw-rw-   0        0        0    18560 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/js/datatable.js
+-rw-rw-rw-   0        0        0     2470 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/js/image-field.js
+-rw-rw-rw-   0        0        0    30541 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/js/main.js
+-rw-rw-rw-   0        0        0      959 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/js/notification.js
+-rw-rw-rw-   0        0        0     2213 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/js/pagination-vue.js
+-rw-rw-rw-   0        0        0    20317 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/js/tableexport.js
+-rw-rw-rw-   0        0        0      654 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/js/transaction.js
+-rw-rw-rw-   0        0        0   354110 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/js/vue.js
+-rw-rw-rw-   0        0        0   268386 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/static/badi_utils/js/xlsx.mini.min.js
+drwxrwxrwx   0        0        0        0 2023-04-16 12:32:09.406292 badi_users-0.9.4/badi_utils/templates/
+-rw-rw-rw-   0        0        0        0 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 12:32:09.423245 badi_users-0.9.4/badi_utils/templates/component/
+-rw-rw-rw-   0        0        0     1777 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/component/createModal.html
+-rw-rw-rw-   0        0        0     1645 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/component/createTitle.html
+-rw-rw-rw-   0        0        0     1054 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/component/filter-form.html
+-rw-rw-rw-   0        0        0      729 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/component/form-errors.html
+-rw-rw-rw-   0        0        0     1340 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/component/form-progressbar-js.html
+-rw-rw-rw-   0        0        0      491 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/component/form-progressbar.html
+-rw-rw-rw-   0        0        0      342 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/component/form.html
+-rw-rw-rw-   0        0        0     1231 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/component/image-field.html
+-rw-rw-rw-   0        0        0    34439 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/component/index-menu.html
+-rw-rw-rw-   0        0        0     2346 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/component/input.html
+-rw-rw-rw-   0        0        0       69 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/component/loader.html
+-rw-rw-rw-   0        0        0      468 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/component/menu-item.html
+-rw-rw-rw-   0        0        0      362 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/component/menu-list.html
+-rw-rw-rw-   0        0        0      746 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/component/messages.html
+-rw-rw-rw-   0        0        0     1134 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/component/pagination-vue.html
+-rw-rw-rw-   0        0        0      361 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/component/profile_item.html
+-rw-rw-rw-   0        0        0      204 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/component/space-between.html
+-rw-rw-rw-   0        0        0      430 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/component/svg-button-with-text.html
+-rw-rw-rw-   0        0        0      428 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/component/svg-button.html
+-rw-rw-rw-   0        0        0     1411 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/component/table-item.html
+-rw-rw-rw-   0        0        0     2114 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/component/user-card.html
+-rw-rw-rw-   0        0        0      257 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/component/yesno.html
+drwxrwxrwx   0        0        0        0 2023-04-16 12:32:09.467217 badi_users-0.9.4/badi_utils/templates/svg/
+-rw-rw-rw-   0        0        0     1949 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/svg/Incoming-box.html
+-rw-rw-rw-   0        0        0     1159 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/svg/add-user.html
+-rw-rw-rw-   0        0        0     1092 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/svg/address-book.html
+-rw-rw-rw-   0        0        0     1095 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/svg/arrow-left.html
+-rw-rw-rw-   0        0        0     1081 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/svg/arrow-right.html
+-rw-rw-rw-   0        0        0     2024 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/svg/bitcoin.html
+-rw-rw-rw-   0        0        0      697 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/svg/box.html
+-rw-rw-rw-   0        0        0     1378 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/svg/calendar-day.html
+-rw-rw-rw-   0        0        0     1489 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/svg/calendar-gym.html
+-rw-rw-rw-   0        0        0      925 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/svg/calendar.html
+-rw-rw-rw-   0        0        0     1223 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/svg/call.html
+-rw-rw-rw-   0        0        0     1385 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/svg/category.html
+-rw-rw-rw-   0        0        0     1270 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/svg/chat.html
+-rw-rw-rw-   0        0        0      938 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/svg/check.html
+-rw-rw-rw-   0        0        0      344 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/svg/circle.html
+-rw-rw-rw-   0        0        0     1686 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/svg/city.html
+-rw-rw-rw-   0        0        0     1430 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/svg/clipboard-list.html
+-rw-rw-rw-   0        0        0     2247 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/svg/clock.html
+-rw-rw-rw-   0        0        0      645 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/svg/close.html
+-rw-rw-rw-   0        0        0     2483 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/svg/collection.html
+-rw-rw-rw-   0        0        0     1046 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/svg/comment.html
+-rw-rw-rw-   0        0        0     1103 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/svg/dashboard.html
+-rw-rw-rw-   0        0        0      893 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/svg/delete.html
+-rw-rw-rw-   0        0        0     1505 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/svg/download.html
+-rw-rw-rw-   0        0        0      901 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/svg/edit.html
+-rw-rw-rw-   0        0        0     1361 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/svg/file-check.html
+-rw-rw-rw-   0        0        0      988 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/svg/file.html
+-rw-rw-rw-   0        0        0     2111 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/svg/film.html
+-rw-rw-rw-   0        0        0      681 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/svg/fire.html
+-rw-rw-rw-   0        0        0     1648 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/svg/group-chat.html
+-rw-rw-rw-   0        0        0     1213 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/svg/group.html
+-rw-rw-rw-   0        0        0     1394 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/svg/half_star.html
+-rw-rw-rw-   0        0        0      944 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/svg/home.html
+-rw-rw-rw-   0        0        0     1906 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/svg/hourse.html
+-rw-rw-rw-   0        0        0      631 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/svg/image.html
+-rw-rw-rw-   0        0        0      508 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/svg/info.html
+-rw-rw-rw-   0        0        0     1394 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/svg/interview.html
+-rw-rw-rw-   0        0        0     1389 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/svg/key.html
+-rw-rw-rw-   0        0        0     2472 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/svg/logout.html
+-rw-rw-rw-   0        0        0      940 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/svg/mail.html
+-rw-rw-rw-   0        0        0      731 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/svg/map.html
+-rw-rw-rw-   0        0        0     1601 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/svg/message.html
+-rw-rw-rw-   0        0        0     1607 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/svg/messages.html
+-rw-rw-rw-   0        0        0      683 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/svg/notification.html
+-rw-rw-rw-   0        0        0      708 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/svg/plus.html
+-rw-rw-rw-   0        0        0      753 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/svg/puzzle.html
+-rw-rw-rw-   0        0        0      882 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/svg/question.html
+-rw-rw-rw-   0        0        0     1174 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/svg/refresh.html
+-rw-rw-rw-   0        0        0     1416 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/svg/safe.html
+-rw-rw-rw-   0        0        0     1091 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/svg/search.html
+-rw-rw-rw-   0        0        0     1114 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/svg/shield-protected.html
+-rw-rw-rw-   0        0        0     1219 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/svg/shield-user.html
+-rw-rw-rw-   0        0        0      451 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/svg/slide.html
+-rw-rw-rw-   0        0        0     1587 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/svg/timer.html
+-rw-rw-rw-   0        0        0     1043 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/svg/town.html
+-rw-rw-rw-   0        0        0      804 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/svg/user.html
+-rw-rw-rw-   0        0        0      936 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/svg/wallet.html
+-rw-rw-rw-   0        0        0      933 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/svg/warning.html
+-rw-rw-rw-   0        0        0       19 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templates/test.html
+drwxrwxrwx   0        0        0        0 2023-04-16 12:32:09.469214 badi_users-0.9.4/badi_utils/templatetags/
+-rw-rw-rw-   0        0        0        0 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templatetags/__init__.py
+-rw-rw-rw-   0        0        0      148 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/templatetags/badi_utils.py
+-rw-rw-rw-   0        0        0     7102 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/utils.py
+-rw-rw-rw-   0        0        0     1911 2023-04-11 07:22:40.000000 badi_users-0.9.4/badi_utils/validations.py
+drwxrwxrwx   0        0        0        0 2023-04-16 12:32:09.472837 badi_users-0.9.4/badi_visit/
+-rw-rw-rw-   0        0        0        0 2022-08-14 04:14:27.000000 badi_users-0.9.4/badi_visit/__init__.py
+-rw-rw-rw-   0        0        0      167 2022-11-10 16:59:20.000000 badi_users-0.9.4/badi_visit/admin.py
+drwxrwxrwx   0        0        0        0 2023-04-16 12:32:09.474832 badi_users-0.9.4/badi_visit/api/
+-rw-rw-rw-   0        0        0        0 2022-10-24 15:37:24.000000 badi_users-0.9.4/badi_visit/api/__init__.py
+-rw-rw-rw-   0        0        0     2871 2022-11-10 16:59:20.000000 badi_users-0.9.4/badi_visit/api/api.py
+-rw-rw-rw-   0        0        0      208 2022-11-10 16:59:20.000000 badi_users-0.9.4/badi_visit/api/routers.py
+-rw-rw-rw-   0        0        0      185 2022-11-10 16:59:20.000000 badi_users-0.9.4/badi_visit/apps.py
+drwxrwxrwx   0        0        0        0 2023-04-16 12:32:09.475830 badi_users-0.9.4/badi_visit/migrations/
+-rw-rw-rw-   0        0        0        0 2022-08-14 04:14:27.000000 badi_users-0.9.4/badi_visit/migrations/__init__.py
+-rw-rw-rw-   0        0        0     1614 2022-11-10 16:59:20.000000 badi_users-0.9.4/badi_visit/models.py
+-rw-rw-rw-   0        0        0       63 2022-08-14 04:14:27.000000 badi_users-0.9.4/badi_visit/tests.py
+drwxrwxrwx   0        0        0        0 2023-04-16 12:32:09.480816 badi_users-0.9.4/badi_wallet/
+-rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.4/badi_wallet/__init__.py
+-rw-rw-rw-   0        0        0     8873 2023-03-27 19:00:31.000000 badi_users-0.9.4/badi_wallet/action.py
+-rw-rw-rw-   0        0        0      202 2023-03-27 19:00:31.000000 badi_users-0.9.4/badi_wallet/admin.py
+drwxrwxrwx   0        0        0        0 2023-04-16 12:32:09.483808 badi_users-0.9.4/badi_wallet/api/
+-rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.4/badi_wallet/api/__init__.py
+-rw-rw-rw-   0        0        0      241 2023-03-27 19:00:31.000000 badi_users-0.9.4/badi_wallet/api/routers.py
+-rw-rw-rw-   0        0        0      543 2023-03-27 19:00:31.000000 badi_users-0.9.4/badi_wallet/api/serializers.py
+-rw-rw-rw-   0        0        0     8037 2023-03-29 08:19:18.000000 badi_users-0.9.4/badi_wallet/api/view_sets.py
+-rw-rw-rw-   0        0        0      243 2023-03-27 19:00:31.000000 badi_users-0.9.4/badi_wallet/apps.py
+-rw-rw-rw-   0        0        0      350 2023-03-28 19:16:55.000000 badi_users-0.9.4/badi_wallet/filter.py
+drwxrwxrwx   0        0        0        0 2023-04-16 12:32:09.268676 badi_users-0.9.4/badi_wallet/locale/
+drwxrwxrwx   0        0        0        0 2023-04-16 12:32:09.268676 badi_users-0.9.4/badi_wallet/locale/fa/
+drwxrwxrwx   0        0        0        0 2023-04-16 12:32:09.483808 badi_users-0.9.4/badi_wallet/locale/fa/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1633 2023-04-16 12:25:06.000000 badi_users-0.9.4/badi_wallet/locale/fa/LC_MESSAGES/django.mo
+drwxrwxrwx   0        0        0        0 2023-04-16 12:32:09.484805 badi_users-0.9.4/badi_wallet/migrations/
+-rw-rw-rw-   0        0        0        0 2022-08-06 18:28:13.000000 badi_users-0.9.4/badi_wallet/migrations/__init__.py
+-rw-rw-rw-   0        0        0     3146 2023-03-30 05:05:34.000000 badi_users-0.9.4/badi_wallet/models.py
+drwxrwxrwx   0        0        0        0 2023-04-16 12:32:09.485803 badi_users-0.9.4/badi_wallet/templates/
+-rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.4/badi_wallet/templates/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 12:32:09.489445 badi_users-0.9.4/badi_wallet/templates/transaction/
+-rw-rw-rw-   0        0        0     6145 2023-03-29 08:22:24.000000 badi_users-0.9.4/badi_wallet/templates/transaction/all_transaction_list.html
+-rw-rw-rw-   0        0        0    10786 2023-03-30 06:06:20.000000 badi_users-0.9.4/badi_wallet/templates/transaction/all_transaction_report.html
+-rw-rw-rw-   0        0        0     2251 2023-03-27 19:00:31.000000 badi_users-0.9.4/badi_wallet/templates/transaction/request-transaction.html
+-rw-rw-rw-   0        0        0     6203 2023-03-29 08:22:11.000000 badi_users-0.9.4/badi_wallet/templates/transaction/transaction_list.html
+-rw-rw-rw-   0        0        0     3547 2023-03-27 19:00:31.000000 badi_users-0.9.4/badi_wallet/templates/transaction/transaction_result.html
+-rw-rw-rw-   0        0        0       63 2023-03-27 19:00:31.000000 badi_users-0.9.4/badi_wallet/tests.py
+drwxrwxrwx   0        0        0        0 2023-04-16 12:32:09.491440 badi_users-0.9.4/badi_wallet/ui/
+-rw-rw-rw-   0        0        0        0 2023-03-27 19:00:31.000000 badi_users-0.9.4/badi_wallet/ui/__init__.py
+-rw-rw-rw-   0        0        0      577 2023-03-28 19:11:37.000000 badi_users-0.9.4/badi_wallet/ui/urls.py
+-rw-rw-rw-   0        0        0     1449 2023-03-28 19:16:42.000000 badi_users-0.9.4/badi_wallet/ui/views.py
+-rw-rw-rw-   0        0        0       42 2023-04-16 12:32:09.493437 badi_users-0.9.4/setup.cfg
+-rw-rw-rw-   0        0        0      498 2023-04-16 12:26:19.000000 badi_users-0.9.4/setup.py
```

### Comparing `badi_users-0.9.3/LICENSE` & `badi_users-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/MANIFEST.in` & `badi_users-0.9.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_ticket/api.py` & `badi_users-0.9.4/badi_ticket/api.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_ticket/locale/fa/LC_MESSAGES/django.mo` & `badi_users-0.9.4/badi_ticket/locale/fa/LC_MESSAGES/django.mo`

 * *Files 20% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-11 09:46+0330\n"
+"POT-Creation-Date: 2023-04-16 15:52+0330\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
@@ -37,14 +37,17 @@
 
 msgid "Download"
 msgstr "دریافت"
 
 msgid "File"
 msgstr "فایل"
 
+msgid "File must be less than %(limit_value)d mb!"
+msgstr "فایل باید کمتر از %(limit_value)d mb باشد!"
+
 msgid "File must be less than 1 mb!"
 msgstr "فایل باید کمتر از 1 مگ باشد!"
 
 msgid "Is seen by admin"
 msgstr "دیده شده توسط مدیر"
 
 msgid "Is seen by user"
```

### Comparing `badi_users-0.9.3/badi_ticket/models.py` & `badi_users-0.9.4/badi_ticket/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,34 @@
+from django.utils.deconstruct import deconstructible
+
 from badi_utils.dynamic_models import BadiModel
-from django.core.validators import MaxLengthValidator
+from django.core.validators import MaxLengthValidator, BaseValidator
 from django.db import models
 from rest_framework.exceptions import ValidationError
-from django.utils.translation import gettext_lazy as _
+from django.utils.translation import gettext_lazy as _, ngettext_lazy
 from django.contrib.auth import get_user_model
 
 User = get_user_model()
 
 
+@deconstructible
+class MaxFileLengthValidator(BaseValidator):
+    message = ngettext_lazy(_('File must be less than %(limit_value)d mb!'),
+                            _('File must be less than %(limit_value)d mb!'),
+                            'limit_value',
+                            )
+    code = 'max_size'
+
+    def compare(self, a, b):
+        return a > (b * 1024 * 1024)
+
+    def clean(self, x):
+        return x.size if x else 0
+
+
 def file_size(value):  # add this to some file where you can import it from
     limit = 1 * 1024 * 1024
     try:
         if value and value.size > limit:
             raise ValidationError(_('File must be less than 1 mb!'))
     except:
         print(value.url + ' NOT FOUND!!!')
@@ -63,14 +80,14 @@
 
     tickt = models.ForeignKey(Ticket, related_name='messages', null=True, on_delete=models.CASCADE,
                               verbose_name=_("Ticket"))
     text = models.TextField(verbose_name=_("Message Text"), validators=[MaxLengthValidator(400)])
     writer = models.ForeignKey(User, related_name='messages', null=True, on_delete=models.CASCADE,
                                verbose_name=_("Writer"))
     file = models.FileField(upload_to='messages/', blank=True, null=True, verbose_name=_("File"),
-                            validators=[file_size])
+                            validators=[MaxFileLengthValidator(1)])
     is_seen = models.BooleanField(default=False, verbose_name=_("Is seen by user"))
     is_seen_by_admin = models.BooleanField(default=False, verbose_name=_("Is seen by admin"))
     created_at = models.DateTimeField(auto_now_add=True, blank=True, verbose_name=_("Sent at"))
 
     def __str__(self):
         return self.tickt.title + ' - ' + self.writer.__str__()
```

### Comparing `badi_users-0.9.3/badi_ticket/serializers.py` & `badi_users-0.9.4/badi_ticket/serializers.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_ticket/static/ticket/js/chat.js` & `badi_users-0.9.4/badi_utils/static/badi_utils/js/chat.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -34,15 +34,15 @@
         sendMessage() {
             const pk = document.getElementById('id_tickt').value;
             this.loading = true;
             ApiAjax({
                 url: MESSAGES_API_URL,
                 method: 'POST',
                 file: true,
-                success_message: badiConfig.ticket_success_message,
+                success_message: 'با موفقیت ارسال شد',
                 success: (data) => {
                     document.getElementById('id_tickt').value = pk;
                     this.getMessages()
                 },
                 error: function(e) {
                     swalFireError();
                 }
```

### Comparing `badi_users-0.9.3/badi_ticket/templates/ticket/admin_tickets.html` & `badi_users-0.9.4/badi_ticket/templates/ticket/admin_tickets.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_ticket/templates/ticket/message_list.html` & `badi_users-0.9.4/badi_ticket/templates/ticket/message_list.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_ticket/templates/ticket/my_tickets.html` & `badi_users-0.9.4/badi_ticket/templates/ticket/my_tickets.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_ticket/templates/ticket/ticket_create.html` & `badi_users-0.9.4/badi_ticket/templates/ticket/ticket_create.html`

 * *Files 25% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 {% extends request.user.is_admin|yesno:"base.html,base-ui.html" %}
 {% load static %}
 {% load widget_tweaks %}
 {% load i18n %}
 {% block body %}
-    <div class="d-flex flex-column-fluid">
-        <!--begin::Container-->
-        <div class="{% if request.user.is_admin %}container-fluid{% else %}container{% endif %}">
-            <div class="row">
-                <div class="col-md-12">
-                    <!--begin::Card-->
-                    <div class="card card-custom">
-                        <div class="card-header">
-                            <h3 class="card-title">
-                                {% trans "List" %}
-                                {{ model_name }}
-                            </h3>
-                            <div class="modal fade card-border" id="ticketModal" tabindex="-1" role="dialog"
-                                 aria-labelledby="exampleModalLabel" aria-hidden="true">
-                                <div class="modal-dialog" role="document">
-                                    <div class="modal-content">
-                                        <div class="modal-header">
-                                            <h5 class="modal-title" id="exampleModalLabel">{% trans "Create" %} {% trans "Ticket" %}</h5>
-                                            <button type="button" class="close" data-dismiss="modal" aria-label="Close">
+	<div class="d-flex flex-column-fluid">
+		<!--begin::Container-->
+		<div class="{% if request.user.is_admin %}container-fluid{% else %}container{% endif %}">
+			<div class="row">
+				<div class="col-md-12">
+					<!--begin::Card-->
+					<div class="card card-custom">
+						<div class="card-header">
+							<h3 class="card-title">
+								{% trans "List" %}
+								{{ model_name }}
+							</h3>
+							<div class="modal fade card-border" id="ticketModal" tabindex="-1" role="dialog"
+								 aria-labelledby="exampleModalLabel" aria-hidden="true">
+								<div class="modal-dialog" role="document">
+									<div class="modal-content">
+										<div class="modal-header">
+											<h5 class="modal-title"
+												id="exampleModalLabel">{% trans "Create" %} {% trans "Ticket" %}</h5>
+											<button type="button" class="close" data-dismiss="modal" aria-label="Close">
 												<i aria-hidden="true" class="ki ki-close"></i>
 											</button>
 										</div>
 										<form id="form_ticket">
 											<div class="modal-body">
 												{% csrf_token %}
 												<div class="form-group">
@@ -34,74 +35,75 @@
 														   placeholder="{% trans 'Title' %}..." name="title"
 														   id="ticket-name">
 												</div>
 												<label class="d-none">
 													<input type="hidden" value="{{ object.writer }}" name="writer">
 												</label>
 												{% if request.user.is_admin %}
-												{{form.writer}}
+													{{ form.writer }}
 												{% endif %}
 											</div>
 											<div class="card-footer p-2">
-												<button type="button" class="btn mx-2 btn-light-primary font-weight-bold"
+												<button type="button"
+														class="btn mx-2 btn-light-primary font-weight-bold"
 														data-dismiss="modal">{% trans "Cancel" %}
 												</button>
 												<button class="btn btn-primary">
 													{% trans "Submit" %} {% trans "Ticket" %}
 												</button>
 											</div>
 										</form>
 									</div>
 								</div>
 							</div>
-                            <div class="card-toolbar">
-                                <button type="button" class="btn btn-primary" data-toggle="modal"
-                                        data-target="#ticketModal">
-                                    {% trans "Submit" %} {% trans "Ticket" %}
-                                </button>
-                            </div>
-
-                        </div>
-                        <div class="card-body">
-                            {% if not disableTable %}
-                                <table class="table table-striped table-custom-border text-center table-rounded table-borderless table-thead-primary"
-                                       id="table">
-                                    <thead>
-                                    {% for field in cols %}
-                                        <th>{{ field }}</th>
-                                    {% endfor %}
-                                    <th>{% trans "Action" %}</th>
-                                    </thead>
-                                    <tbody>
-                                    </tbody>
-                                </table>
-                            {% endif %}
-                        </div>
-                    </div>
-                    <!--end::Card-->
-                </div>
-            </div>
-        </div>
-        <!--end::Container-->
-    </div>
-<script>
-	document.getElementById('id_writer').classList.add('no-select2');
-</script>
+							<div class="card-toolbar">
+								<button type="button" class="btn btn-primary" data-toggle="modal"
+										data-target="#ticketModal">
+									{% trans "Submit" %} {% trans "Ticket" %}
+								</button>
+							</div>
+
+						</div>
+						<div class="card-body">
+							{% if not disableTable %}
+								<table class="table table-striped table-custom-border text-center table-rounded table-borderless table-thead-primary"
+									   id="table">
+									<thead>
+									{% for field in cols %}
+										<th>{{ field }}</th>
+									{% endfor %}
+									<th>{% trans "Action" %}</th>
+									</thead>
+									<tbody>
+									</tbody>
+								</table>
+							{% endif %}
+						</div>
+					</div>
+					<!--end::Card-->
+				</div>
+			</div>
+		</div>
+		<!--end::Container-->
+	</div>
+	<script>
+        document.getElementById('id_writer').classList.add('no-select2');
+	</script>
 
 {% endblock %}
 {% block script %}
 	<script src="{% static 'assets/plugins/custom/datatables/datatables.bundle.js' %}" type="text/javascript"></script>
 	<script src="{% static 'badi_utils/js/datatable.js' %}" type="text/javascript"></script>
 
-    <script>
-		window.data_table_cool_options['columnDefs'].push({
-			"targets": [1],
-			"visible": false,
-			"searchable": false
-		})
+	<script>
+        window.data_table_cool_options['columnDefs'].push({
+            "targets": [1],
+            "visible": false,
+            "searchable": false
+        })
         var table = datatable_simple_show({
             url: '{{ api_url }}datatable/',
             real_cols: {{cols|length}},
             hide_id: true,
             loading_all: true,
             responsive: true,
             datable_id: '#table',
@@ -113,46 +115,46 @@
             extra_filters: function (d) {
                 d.filter_type = true;
             },
 
         }, {
             rowCallback: function (row, data) {
                 {% if request.user.is_admin %}
-                $('td:eq(0)',row).prepend(data[1] +' - ')
+                    $('td:eq(0)', row).prepend(data[1] + ' - ')
                 {%endif%}
-				$(`td:last`, row)
-            {% if request.user.is_admin %}
-                .prepend(
-                {% else %}
-                .html(
-            {% endif %}
-            `
+                $(`td:last`, row)
+                {% if request.user.is_admin %}
+                    .prepend(
+                    {% else %}
+                    .html(
+                {% endif %}
+                `
     <a href="messages/${data[0]}" data-skin="dark" data-toggle="tooltip" data-placement="top" title="" data-original-title="{% trans 'Messages' %}" class="btn btn-sm btn-light-primary btn-icon"><span class="svg-icon svg-icon-md">{% include 'svg/message.html' %}</span></button>
                 `)
-                console.log('DATA',data)
-				const status_list = data[3]
-				const is_closed = status_list[0]
-				const count = status_list[1]
-				let last_message = status_list[2]
-				let color = 'dark'
-				if(last_message === -1){
+                console.log('DATA', data)
+                const status_list = data[3]
+                const is_closed = status_list[0]
+                const count = status_list[1]
+                let last_message = status_list[2]
+                let color = 'dark'
+                if (last_message === -1) {
                     last_message = '{% trans "empty ticket" %}'
-                } else if(last_message === 0){
+                } else if (last_message === 0) {
                     last_message = '{% trans "waiting to answer" %}'
-					color = 'danger'
-                } else if(last_message === 1){
+                    color = 'danger'
+                } else if (last_message === 1) {
                     last_message = '{% trans "answered" %}'
-					color = 'success'
+                    color = 'success'
                 }
-				$(`td:eq(1)`, row).html(
+                $(`td:eq(1)`, row).html(
                     `<label class="label label-xl label-inline font-weight-bold label-light-${color}">
 						<span class="label label-xl mr-2 label-dot label-${color}"></span> {% trans "Ticket" %}: ${is_closed ? '{% trans "close" %}' : '{% trans "open" %}'} - ${last_message}
 					</label>
 `
-				)
+                )
 
             },
 
         });
 
         $('#form_ticket').on('submit', function (e) {
             e.preventDefault();
@@ -160,28 +162,31 @@
             ApiAjax({
                 url: '{{api_url}}',
                 form: '#form_ticket',
                 method: 'POST',
                 button: button,
                 table: table,
                 modal: '#ticketModal',
-                            success_message: '{% trans "Done Successfully" %}',
+                success_message: '{% trans "Done Successfully" %}',
                 file: true,
+                success: (res) => {
+                    open('/dashboard/ticket/messages/' + res.id, '_self')
+                }
             })
         });
-		$('#id_writer').select2({
-				dir: "rtl",
-				ajax: {
-					url: "{{ api_url }}select2/",
-					data: function (params) {
-						var query = {
-							search: params.term,
-							page: params.page || 1
-						};
-
-						// Query parameters will be ?search=[term]&page=[page]
-						return query;
-					}
-				}
-			});
-    </script>
+        $('#id_writer').select2({
+            dir: "rtl",
+            ajax: {
+                url: "{{ api_url }}select2/",
+                data: function (params) {
+                    var query = {
+                        search: params.term,
+                        page: params.page || 1
+                    };
+
+                    // Query parameters will be ?search=[term]&page=[page]
+                    return query;
+                }
+            }
+        });
+	</script>
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 {% extends request.user.is_admin|yesno:"base.html,base-ui.html" %} {% load
 static %} {% load widget_tweaks %} {% load i18n %} {% block body %}
 **** {% trans "List" %} {{ model_name }} ****
 ** {% trans "Create" %} {% trans "Ticket" %} **
 
 {% csrf_token %}
 {% trans "Title" %}: [title               ]
-   {% if request.user.is_admin %} {{form.writer}} {% endif %}
+   {% if request.user.is_admin %} {{ form.writer }} {% endif %}
 {% trans "Cancel" %}   {% trans "Submit" %} {% trans "Ticket" %}
  {% trans "Submit" %} {% trans "Ticket" %}
 {% if not disableTable %}
 {% endif %}
  {% endblock %} {% block script %}
  {% endblock %}
```

### Comparing `badi_users-0.9.3/badi_ticket/templates/ticket/ticket_update.html` & `badi_users-0.9.4/badi_ticket/templates/ticket/ticket_update.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_ticket/urls.py` & `badi_users-0.9.4/badi_ticket/urls.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_ticket/views.py` & `badi_users-0.9.4/badi_ticket/views.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_user/api/api.py` & `badi_users-0.9.4/badi_user/api/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 from badi_utils.utils import random_with_N_digits, permissions_json
 from rest_framework_simplejwt.views import TokenRefreshView
 from badi_user.api.serializers import UserSerializer, GroupSerializer, MemberSerializer, LogSerializer, \
     UserProfileSerializer, UserRegisterSerializer
 from badi_user.filter import UserListFilter, MemberListFilter, LogFilter
 from badi_user.models import Token, Log
 from django.utils.translation import gettext_lazy as _
-from badi_utils.sms import IpPanelSms
 from django.contrib.auth import get_user_model
 from django.conf import settings
 
 MONTH_NAMES = ["Jan", "Feb", "Mar", "Apr", "Maj", "Jun", "Jul", "Aug", "Sep", "Okt", "Nov", "Dec"]
 BADI_AUTH_CONFIG = getattr(settings, "BADI_AUTH_CONFIG", {})
 
 User = get_user_model()
@@ -394,48 +393,39 @@
             errors['old_password'] = []
             errors['old_password'].append('رمز عبور فعلی اشتباه است')
 
         return JsonResponse(errors, status=HTTP_400_BAD_REQUEST)
 
     @action(methods=['post'], detail=False)
     def forgot_password(self, req, *args, **kwargs):
-        mobile_number = self.request.data.get('mobile_number')
-        user = User.objects.filter(mobile_number=mobile_number).first()
+        config = BADI_AUTH_CONFIG['forgot']
+        mobile_email = self.request.data.get(config.get('user_find_key'))
+        user = User.objects.filter(**{config.get('user_find_key'): mobile_email}).first()
         if not user:
-            return JsonResponse({'mobile_number': ['کاربری با شماره تماس وارد شده وجود ندارد!']},
+            return JsonResponse({config.get('user_find_key'): [_('There is no user with this specifications!')]},
                                 status=HTTP_400_BAD_REQUEST)
+        HTTP_ORIGIN = config.get('site_url') or req.META.get('HTTP_ORIGIN')
+        if user.token and user.token.is_enabled():
+            return JsonResponse({'mobile_number': ['شما به تازگی درخواست داده اید!']},
+                                status=HTTP_400_BAD_REQUEST)
+        hash_code = ''.join(random.choice(string.ascii_letters + string.digits) for x in range(10))
+        token = Token()
+        token.phone = user.username
+        token.last_send = datetime.datetime.now()
+        token.is_forgot = True
+        token.token = hash_code
+        token.save()
+        user.token = token
+        user.save()
+        token_id_hash = token.pk * 8569 - 1330
+        text = f'{HTTP_ORIGIN}/forgot_password/{token_id_hash}/{hash_code}'
+        print(f'لینک تغییر رمز عبور: %0D%0A {text}')
 
-        phone_number = self.request.data.get('mobile_number')
-        HTTP_ORIGIN = req.META.get('HTTP_ORIGIN')
-        if phone_number and len(phone_number) == 11:
-            user = User.objects.filter(mobile_number=phone_number).first()
-            if user:
-                if user.token and user.token.is_enabled():
-                    return JsonResponse({'mobile_number': ['شما به تازگی درخواست داده اید!']},
-                                        status=HTTP_400_BAD_REQUEST)
-                hash_code = ''.join(random.choice(string.ascii_letters + string.digits) for x in range(30))
-                token = Token()
-                token.user = user
-                token.last_send = datetime.datetime.now()
-                token.is_forgot = True
-                token.token = hash_code
-                token.save()
-                user.token = token
-                user.save()
-                token_id_hash = token.pk * 8569 - 1330
-                text = f'{HTTP_ORIGIN}/forgot_password/{token_id_hash}/{hash_code}'
-                print(f'لینک تغییر رمز عبور: %0D%0A {text}')
-                Sms.link(user.mobile_number, token_id_hash, hash_code)
-                return ResponseOk({})
-
-            else:
-                return JsonResponse({'mobile_number': ['کاربری با شماره تماس وارد شده وجود ندارد!']},
-                                    status=HTTP_400_BAD_REQUEST)
-
-        return JsonResponse({'mobile_number': ['مشکلی پیش آمده است!']}, status=HTTP_400_BAD_REQUEST)
+        config.get('class')(getattr(user, config.get('user_find_key'))).send_forgot_link(token_id_hash, hash_code)
+        return ResponseOk({})
 
     @action(methods=['post'], detail=False)
     def refresh(self, request, *args, **kwargs):
         serializer = TokenRefreshSerializer(data=request.data)
         try:
             serializer.is_valid(raise_exception=True)
         except TokenError as e:
```

### Comparing `badi_users-0.9.3/badi_user/api/serializers.py` & `badi_users-0.9.4/badi_user/api/serializers.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_user/filter.py` & `badi_users-0.9.4/badi_user/filter.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_user/locale/fa/LC_MESSAGES/django.mo` & `badi_users-0.9.4/badi_user/locale/fa/LC_MESSAGES/django.mo`

 * *Files 24% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-11 09:46+0330\n"
+"POT-Creation-Date: 2023-04-16 15:52+0330\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
@@ -25,14 +25,17 @@
 
 msgid "Back"
 msgstr "بازگشت"
 
 msgid "Birth Date"
 msgstr "تاریخ تولد"
 
+msgid "Cancel"
+msgstr "لغو"
+
 msgid "Change Password"
 msgstr "تغییر رمز عبور"
 
 msgid "Charge"
 msgstr "شارژ"
 
 msgid "Charge account"
@@ -58,44 +61,68 @@
 
 msgid "Got it"
 msgstr "متوجه شدم"
 
 msgid "Invalid username"
 msgstr "نام کاربری غیر معتبر"
 
+msgid "Is Seen"
+msgstr "دیده شده"
+
 msgid "LastName"
 msgstr "نام خانوادگی"
 
 msgid "List"
 msgstr "لیست"
 
+msgid "Log"
+msgstr "لاگ"
+
 msgid "Login"
 msgstr "ورود به حساب کاربری"
 
+msgid "Logs"
+msgstr "لاگ ها"
+
 msgid "Member"
 msgstr "عضو"
 
 msgid "Mobile Number"
 msgstr "شماره تماس"
 
 msgid "New Password"
 msgstr "رمز جدید"
 
+msgid "No active user found"
+msgstr "کاربر فعالی یافت نشد"
+
+msgid "Notifications"
+msgstr "اعلانات"
+
 msgid "Optional"
 msgstr "اختیاری"
 
 msgid "Password"
 msgstr "رمز عبور"
 
 msgid "Password changed successfully"
 msgstr "رمز عبور با موفقیت بروزرسانی شد"
 
+msgid "Persian"
+msgstr "فارسی"
+
 msgid "Picture"
 msgstr "تصویر پروفایل"
 
+msgid "Please try again"
+msgstr "لطفا دوباره تلاش کنید"
+
+msgid "Priority"
+msgstr "سطح اهمیت"
+
 msgid "Province"
 msgstr "استان"
 
 msgid "Repeat Password"
 msgstr "تکرار رمز عبور"
 
 msgid "Repeat Password and New Password are not equal"
@@ -115,14 +142,17 @@
 
 msgid "Send ticket"
 msgstr "ارسال تیکت"
 
 msgid "Submit"
 msgstr "ثبت"
 
+msgid "There is no user with this specifications!"
+msgstr "کاربری با مشخصات مورد نظر پیدا نشد!"
+
 msgid "This Field is required"
 msgstr "این فیلد ضروری است"
 
 msgid "This mobile number already registered"
 msgstr "این شماره تماس قبلا ثبت شده است"
 
 msgid "This username already taken"
@@ -163,15 +193,21 @@
 
 msgid "must be between 2 and 20 character"
 msgstr "باید بین 2 و 20 حرف باشد"
 
 msgid "must be between 6 and 20 character"
 msgstr "باید بین 6 تا 20 حرف باشد"
 
+msgid "new Password and repeat password must be equal!"
+msgstr "رمز جدید و تکرار رمز عبور باید یکسان باشند!"
+
 msgid "on"
 msgstr "روی"
 
 msgid "record"
 msgstr "رکورد"
 
 msgid "self information"
 msgstr "اطلاعات شخصی"
+
+msgid "to"
+msgstr "به"
```

### Comparing `badi_users-0.9.3/badi_user/models.py` & `badi_users-0.9.4/badi_user/models.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_user/templates/group/group_create.html` & `badi_users-0.9.4/badi_user/templates/group/group_create.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_user/templates/group/group_update.html` & `badi_users-0.9.4/badi_user/templates/group/group_update.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_user/templates/log/log_list.html` & `badi_users-0.9.4/badi_user/templates/log/log_list.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_user/templates/login-theme/login-1.html` & `badi_users-0.9.4/badi_user/templates/login-theme/login-1.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_user/templates/member/member_create.html` & `badi_users-0.9.4/badi_user/templates/member/member_create.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_user/templates/member/member_list.html` & `badi_users-0.9.4/badi_user/templates/member/member_list.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_user/templates/member/member_self_update.html` & `badi_users-0.9.4/badi_user/templates/member/member_self_update.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_user/templates/member/member_update.html` & `badi_users-0.9.4/badi_user/templates/member/member_update.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_user/templates/user/user_create.html` & `badi_users-0.9.4/badi_user/templates/user/user_create.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_user/templates/user/user_list.html` & `badi_users-0.9.4/badi_user/templates/user/user_list.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_user/templates/user/user_update.html` & `badi_users-0.9.4/badi_user/templates/user/user_update.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_user/templatetags/appfilter.py` & `badi_users-0.9.4/badi_user/templatetags/appfilter.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_user/ui/forms.py` & `badi_users-0.9.4/badi_user/ui/forms.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_user/ui/member_views.py` & `badi_users-0.9.4/badi_user/ui/member_views.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_user/ui/notification_views.py` & `badi_users-0.9.4/badi_user/ui/notification_views.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_user/ui/roles_views.py` & `badi_users-0.9.4/badi_user/ui/roles_views.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_user/ui/urls.py` & `badi_users-0.9.4/badi_user/ui/urls.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from badi_user.ui.views import *
 from django.contrib.auth import get_user_model
 
 User = get_user_model()
 urlpatterns = [
     path('login/', UserLoginView.as_view(), name='custom_login'),
     path('logout/', UserLogout.as_view(), name='user_logout'),
-    path('change_password/', ChangePasswordForgot.as_view(), name="forgot_password"),
+    path('change_password/', ChangePasswordViewTemplateView.as_view(), name="change_password"),
     path('forgot_password/<str:token_id>/<str:hash_code>', ChangePasswordForgot.as_view(),
          name="forgot_password"),
     generate_url(User(), create=UserCreateView),
     generate_url(User(), view=UserListView),
     generate_url(User(), update=UserUpdateView),
     path('member/list', MemberListView.as_view(), name='member_list'),
     path('member/create', MemberCreateView.as_view(), name='member_create'),
```

### Comparing `badi_users-0.9.3/badi_user/ui/views.py` & `badi_users-0.9.4/badi_user/ui/views.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_users.egg-info/SOURCES.txt` & `badi_users-0.9.4/badi_users.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/date_calc.py` & `badi_users-0.9.4/badi_utils/date_calc.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/dynamic.py` & `badi_users-0.9.4/badi_utils/dynamic.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/dynamic_api.py` & `badi_users-0.9.4/badi_utils/dynamic_api.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/dynamic_models.py` & `badi_users-0.9.4/badi_utils/dynamic_models.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/email.py` & `badi_users-0.9.4/badi_utils/email.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/logging.py` & `badi_users-0.9.4/badi_utils/logging.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/responses.py` & `badi_users-0.9.4/badi_utils/responses.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/rss.py` & `badi_users-0.9.4/badi_utils/rss.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/select2.py` & `badi_users-0.9.4/badi_utils/select2.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/sms.py` & `badi_users-0.9.4/badi_utils/sms.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,51 @@
 from os import getenv
 
 import requests
 
 SMS_SEND_URL = getenv('SMS__IP_PANEL_URL')
+SMS_POST_URL = getenv('SMS_POST_URL', 'http://ippanel.com/api/select')
 ORIGINATOR = getenv('SMS__IP_PANEL_ORGINATOR')
+SMS__USERNAME = getenv('SMS__USERNAME')
+SMS__PASSWORD = getenv('SMS__PASSWORD')
 SMS_ENABLE = getenv('SMS__ENABLE')
 SMS__IPPANEL_F_NUM_VERIFY_CODE = getenv('SMS__IPPANEL_F_NUM_VERIFY_CODE')
 SMS__IPPANEL_P_ID_VERIFY_CODE = getenv('SMS__IPPANEL_P_ID_VERIFY_CODE')
+SMS__IPPANEL_P_ID_FORGOT_LINK = getenv('SMS__IPPANEL_P_ID_FORGOT_LINK')
+SMS__IPPANEL_PATTERN_CODE_FORGOT_LINK = getenv('SMS__IPPANEL_PATTERN_CODE_FORGOT_LINK')
 SMS__IPPANEL_PARAM_NAME = getenv('SMS__IPPANEL_PARAM_NAME', "v-code")
+SMS__IPPANEL_FORGOT_LINK_V1 = getenv('SMS__IPPANEL_FORGOT_LINK_V1', "token")
+SMS__IPPANEL_FORGOT_LINK_V2 = getenv('SMS__IPPANEL_FORGOT_LINK_V2', "hash")
+SMS__IPPANEL_FROM_NUMBER_FORGOT_LINK = getenv('SMS__IPPANEL_FROM_NUMBER_FORGOT_LINK', SMS__IPPANEL_F_NUM_VERIFY_CODE)
 
 
 class IpPanelSms:
 
     def __init__(self, phone_number):
         self.phone_number = phone_number
 
-    def send_forgot_link(self, pattern_code, values):
-        print(f'Send Sms {str(values)}')
+    def send_forgot_link(self, token_id_hash, hash_code):
+        print(f'Send send_forgot_link', token_id_hash, hash_code)
         if not SMS_ENABLE:
             return
         for i in range(10):
             try:
-                requests.post(
+                result = requests.get(
                     SMS_SEND_URL,
-                    json={
-                        "originator": ORIGINATOR,
-                        "recipient": self.phone_number,
-                        "pattern_code": pattern_code,
-                        "values": values
+                    params={
+                        "apikey": ORIGINATOR,
+                        "fnum": SMS__IPPANEL_F_NUM_VERIFY_CODE,
+                        "tnum": self.phone_number,
+                        "pid": SMS__IPPANEL_PATTERN_CODE_FORGOT_LINK,
+                        "p1": SMS__IPPANEL_FORGOT_LINK_V1,
+                        "v1": str(token_id_hash),
+                        "p2": SMS__IPPANEL_FORGOT_LINK_V2,
+                        "v2": str(hash_code),
                     }, headers={
                         "Content-Type": "application/json",
-                        "Authorization": ORIGINATOR
                     })
                 return True
             except Exception as e:
                 print(e)
         return False
 
     def send_verify_code(self, text):
```

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/css/custom.css` & `badi_users-0.9.4/badi_utils/static/badi_utils/css/custom.css`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).eot` & `badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).ttf` & `badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).ttf`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).woff` & `badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).woff`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).woff2` & `badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum).woff2`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_2.eot` & `badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_2.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.eot` & `badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.ttf` & `badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.ttf`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.woff` & `badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.woff`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.woff2` & `badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold.woff2`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold_2.eot` & `badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Bold_2.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.eot` & `badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.ttf` & `badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.ttf`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.woff` & `badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.woff`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.woff2` & `badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light.woff2`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light_2.eot` & `badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Light_2.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.eot` & `badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.ttf` & `badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.ttf`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.woff` & `badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.woff`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.woff2` & `badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium.woff2`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium_2.eot` & `badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_Medium_2.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.eot` & `badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.ttf` & `badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.ttf`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.woff` & `badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.woff`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.woff2` & `badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight.woff2`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight_2.eot` & `badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb(FaNum)_UltraLight_2.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb.eot` & `badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb.woff` & `badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb.woff`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb.woff2` & `badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb.woff2`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_2.eot` & `badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_2.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.eot` & `badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.ttf` & `badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.ttf`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.woff` & `badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.woff`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.woff2` & `badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold.woff2`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold_2.eot` & `badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold_2.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold_3.eot` & `badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Bold_3.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.eot` & `badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.ttf` & `badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.ttf`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.woff` & `badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.woff`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.woff2` & `badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light.woff2`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light_2.eot` & `badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Light_2.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.eot` & `badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.ttf` & `badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.ttf`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.woff` & `badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.woff`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.woff2` & `badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium.woff2`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium_2.eot` & `badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_Medium_2.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.eot` & `badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.ttf` & `badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.ttf`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.woff` & `badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.woff`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.woff2` & `badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight.woff2`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight_2.eot` & `badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/IRANSansWeb_UltraLight_2.eot`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/Ray-Black.ttf` & `badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/Ray-Black.ttf`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/Ray-Bold.ttf` & `badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/Ray-Bold.ttf`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/css/fonts/Ray.ttf` & `badi_users-0.9.4/badi_utils/static/badi_utils/css/fonts/Ray.ttf`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/js/apexchart.js` & `badi_users-0.9.4/badi_utils/static/badi_utils/js/apexchart.js`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/js/api-login.js` & `badi_users-0.9.4/badi_utils/static/badi_utils/js/api-login.js`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/js/api.js` & `badi_users-0.9.4/badi_utils/static/badi_utils/js/api.js`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/js/base.js` & `badi_users-0.9.4/badi_utils/static/badi_utils/js/base.js`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/js/chat.js` & `badi_users-0.9.4/badi_ticket/static/ticket/js/chat.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -24,31 +24,37 @@
                     console.log(data)
                     this.messages = data.response;
                     this.loading = false;
                     this.tickt = data.ticket;
                 },
                 error: function(e) {
                     swalFireError();
+                    this.loading = false;
                 }
             })
         },
         sendMessage() {
             const pk = document.getElementById('id_tickt').value;
+            let fileEl = document.getElementById('id_file');
+            if ((fileEl.files[0]) && fileEl.files[0].size / 1024 / 1024 > 1) {
+                swalFireError(badiConfig.fileSizeError.replace('#size', '1mb'))
+                return
+            }
             this.loading = true;
             ApiAjax({
                 url: MESSAGES_API_URL,
                 method: 'POST',
                 file: true,
-                success_message: 'با موفقیت ارسال شد',
+                success_message: badiConfig.ticket_success_message,
                 success: (data) => {
                     document.getElementById('id_tickt').value = pk;
                     this.getMessages()
                 },
-                error: function(e) {
-                    swalFireError();
+                error: (e) => {
+                    this.getMessages()
                 }
             })
         },
         get(val) {
             if (val === true) {
                 return 'بله'
             } else {
```

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/js/custom-vue.js` & `badi_users-0.9.4/badi_utils/static/badi_utils/js/custom-vue.js`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/js/datatable.js` & `badi_users-0.9.4/badi_utils/static/badi_utils/js/datatable.js`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/js/image-field.js` & `badi_users-0.9.4/badi_utils/static/badi_utils/js/image-field.js`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/js/main.js` & `badi_users-0.9.4/badi_utils/static/badi_utils/js/main.js`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/js/notification.js` & `badi_users-0.9.4/badi_utils/static/badi_utils/js/notification.js`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/js/pagination-vue.js` & `badi_users-0.9.4/badi_utils/static/badi_utils/js/pagination-vue.js`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/js/tableexport.js` & `badi_users-0.9.4/badi_utils/static/badi_utils/js/tableexport.js`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/js/transaction.js` & `badi_users-0.9.4/badi_utils/static/badi_utils/js/transaction.js`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/js/vue.js` & `badi_users-0.9.4/badi_utils/static/badi_utils/js/vue.js`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/static/badi_utils/js/xlsx.mini.min.js` & `badi_users-0.9.4/badi_utils/static/badi_utils/js/xlsx.mini.min.js`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/component/createModal.html` & `badi_users-0.9.4/badi_utils/templates/component/createModal.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/component/createTitle.html` & `badi_users-0.9.4/badi_utils/templates/component/createTitle.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/component/filter-form.html` & `badi_users-0.9.4/badi_utils/templates/component/filter-form.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/component/form-errors.html` & `badi_users-0.9.4/badi_utils/templates/component/form-errors.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/component/form-progressbar-js.html` & `badi_users-0.9.4/badi_utils/templates/component/form-progressbar-js.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/component/image-field.html` & `badi_users-0.9.4/badi_utils/templates/component/image-field.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/component/index-menu.html` & `badi_users-0.9.4/badi_utils/templates/component/index-menu.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/component/input.html` & `badi_users-0.9.4/badi_utils/templates/component/input.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/component/messages.html` & `badi_users-0.9.4/badi_utils/templates/component/messages.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/component/pagination-vue.html` & `badi_users-0.9.4/badi_utils/templates/component/pagination-vue.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/component/table-item.html` & `badi_users-0.9.4/badi_utils/templates/component/table-item.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/component/user-card.html` & `badi_users-0.9.4/badi_utils/templates/component/user-card.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/svg/Incoming-box.html` & `badi_users-0.9.4/badi_utils/templates/svg/Incoming-box.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/svg/add-user.html` & `badi_users-0.9.4/badi_utils/templates/svg/add-user.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/svg/address-book.html` & `badi_users-0.9.4/badi_utils/templates/svg/address-book.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/svg/arrow-left.html` & `badi_users-0.9.4/badi_utils/templates/svg/arrow-left.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/svg/arrow-right.html` & `badi_users-0.9.4/badi_utils/templates/svg/arrow-right.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/svg/bitcoin.html` & `badi_users-0.9.4/badi_utils/templates/svg/bitcoin.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/svg/box.html` & `badi_users-0.9.4/badi_utils/templates/svg/box.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/svg/calendar-day.html` & `badi_users-0.9.4/badi_utils/templates/svg/calendar-day.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/svg/calendar-gym.html` & `badi_users-0.9.4/badi_utils/templates/svg/calendar-gym.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/svg/calendar.html` & `badi_users-0.9.4/badi_utils/templates/svg/calendar.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/svg/call.html` & `badi_users-0.9.4/badi_utils/templates/svg/call.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/svg/category.html` & `badi_users-0.9.4/badi_utils/templates/svg/category.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/svg/chat.html` & `badi_users-0.9.4/badi_utils/templates/svg/chat.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/svg/check.html` & `badi_users-0.9.4/badi_utils/templates/svg/check.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/svg/city.html` & `badi_users-0.9.4/badi_utils/templates/svg/city.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/svg/clipboard-list.html` & `badi_users-0.9.4/badi_utils/templates/svg/clipboard-list.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/svg/clock.html` & `badi_users-0.9.4/badi_utils/templates/svg/clock.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/svg/close.html` & `badi_users-0.9.4/badi_utils/templates/svg/close.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/svg/collection.html` & `badi_users-0.9.4/badi_utils/templates/svg/collection.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/svg/comment.html` & `badi_users-0.9.4/badi_utils/templates/svg/comment.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/svg/dashboard.html` & `badi_users-0.9.4/badi_utils/templates/svg/dashboard.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/svg/delete.html` & `badi_users-0.9.4/badi_utils/templates/svg/delete.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/svg/download.html` & `badi_users-0.9.4/badi_utils/templates/svg/download.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/svg/edit.html` & `badi_users-0.9.4/badi_utils/templates/svg/edit.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/svg/file-check.html` & `badi_users-0.9.4/badi_utils/templates/svg/file-check.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/svg/file.html` & `badi_users-0.9.4/badi_utils/templates/svg/file.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/svg/film.html` & `badi_users-0.9.4/badi_utils/templates/svg/film.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/svg/fire.html` & `badi_users-0.9.4/badi_utils/templates/svg/fire.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/svg/group-chat.html` & `badi_users-0.9.4/badi_utils/templates/svg/group-chat.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/svg/group.html` & `badi_users-0.9.4/badi_utils/templates/svg/group.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/svg/half_star.html` & `badi_users-0.9.4/badi_utils/templates/svg/half_star.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/svg/home.html` & `badi_users-0.9.4/badi_utils/templates/svg/home.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/svg/hourse.html` & `badi_users-0.9.4/badi_utils/templates/svg/hourse.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/svg/image.html` & `badi_users-0.9.4/badi_utils/templates/svg/image.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/svg/interview.html` & `badi_users-0.9.4/badi_utils/templates/svg/interview.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/svg/key.html` & `badi_users-0.9.4/badi_utils/templates/svg/key.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/svg/logout.html` & `badi_users-0.9.4/badi_utils/templates/svg/logout.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/svg/mail.html` & `badi_users-0.9.4/badi_utils/templates/svg/mail.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/svg/map.html` & `badi_users-0.9.4/badi_utils/templates/svg/map.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/svg/message.html` & `badi_users-0.9.4/badi_utils/templates/svg/message.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/svg/messages.html` & `badi_users-0.9.4/badi_utils/templates/svg/messages.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/svg/notification.html` & `badi_users-0.9.4/badi_utils/templates/svg/notification.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/svg/plus.html` & `badi_users-0.9.4/badi_utils/templates/svg/plus.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/svg/puzzle.html` & `badi_users-0.9.4/badi_utils/templates/svg/puzzle.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/svg/question.html` & `badi_users-0.9.4/badi_utils/templates/svg/question.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/svg/refresh.html` & `badi_users-0.9.4/badi_utils/templates/svg/refresh.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/svg/safe.html` & `badi_users-0.9.4/badi_utils/templates/svg/safe.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/svg/search.html` & `badi_users-0.9.4/badi_utils/templates/svg/search.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/svg/shield-protected.html` & `badi_users-0.9.4/badi_utils/templates/svg/shield-protected.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/svg/shield-user.html` & `badi_users-0.9.4/badi_utils/templates/svg/shield-user.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/svg/timer.html` & `badi_users-0.9.4/badi_utils/templates/svg/timer.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/svg/town.html` & `badi_users-0.9.4/badi_utils/templates/svg/town.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/svg/user.html` & `badi_users-0.9.4/badi_utils/templates/svg/user.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/svg/wallet.html` & `badi_users-0.9.4/badi_utils/templates/svg/wallet.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/templates/svg/warning.html` & `badi_users-0.9.4/badi_utils/templates/svg/warning.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/utils.py` & `badi_users-0.9.4/badi_utils/utils.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_utils/validations.py` & `badi_users-0.9.4/badi_utils/validations.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_visit/api/api.py` & `badi_users-0.9.4/badi_visit/api/api.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_visit/models.py` & `badi_users-0.9.4/badi_visit/models.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_wallet/action.py` & `badi_users-0.9.4/badi_wallet/action.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_wallet/api/serializers.py` & `badi_users-0.9.4/badi_wallet/api/serializers.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_wallet/api/view_sets.py` & `badi_users-0.9.4/badi_wallet/api/view_sets.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_wallet/locale/fa/LC_MESSAGES/django.mo` & `badi_users-0.9.4/badi_wallet/locale/fa/LC_MESSAGES/django.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,12 +1,12 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-04-11 09:46+0330\n"
+"POT-Creation-Date: 2023-04-16 15:52+0330\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
```

### Comparing `badi_users-0.9.3/badi_wallet/models.py` & `badi_users-0.9.4/badi_wallet/models.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_wallet/templates/transaction/all_transaction_list.html` & `badi_users-0.9.4/badi_wallet/templates/transaction/all_transaction_list.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_wallet/templates/transaction/all_transaction_report.html` & `badi_users-0.9.4/badi_wallet/templates/transaction/all_transaction_report.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_wallet/templates/transaction/request-transaction.html` & `badi_users-0.9.4/badi_wallet/templates/transaction/request-transaction.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_wallet/templates/transaction/transaction_list.html` & `badi_users-0.9.4/badi_wallet/templates/transaction/transaction_list.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_wallet/templates/transaction/transaction_result.html` & `badi_users-0.9.4/badi_wallet/templates/transaction/transaction_result.html`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_wallet/ui/urls.py` & `badi_users-0.9.4/badi_wallet/ui/urls.py`

 * *Files identical despite different names*

### Comparing `badi_users-0.9.3/badi_wallet/ui/views.py` & `badi_users-0.9.4/badi_wallet/ui/views.py`

 * *Files identical despite different names*

