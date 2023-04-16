# Comparing `tmp/uvicore-0.1.8.tar.gz` & `tmp/uvicore-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uvicore-0.1.8.tar", last modified: Mon Mar 22 20:33:26 2021, max compression
+gzip compressed data, was "uvicore-0.1.9.tar", last modified: Mon Mar 22 21:24:02 2021, max compression
```

## Comparing `uvicore-0.1.8.tar` & `uvicore-0.1.9.tar`

### file list

```diff
@@ -1,196 +1,195 @@
--rw-r--r--   0        0        0     1082 2021-03-22 20:00:01.058788 uvicore-0.1.8/LICENSE
--rw-r--r--   0        0        0     2517 2020-12-03 22:25:41.581951 uvicore-0.1.8/README.md
--rw-r--r--   0        0        0     2657 2021-03-22 20:32:58.942766 uvicore-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     3537 2021-01-28 23:57:53.792892 uvicore-0.1.8/uvicore/NOTES.md
--rw-r--r--   0        0        0     2055 2021-03-22 20:33:16.636142 uvicore-0.1.8/uvicore/__init__.py
--rw-r--r--   0        0        0       23 2021-03-13 03:32:22.776409 uvicore-0.1.8/uvicore/auth/__init__.py
--rw-r--r--   0        0        0       80 2021-02-18 23:17:24.966073 uvicore-0.1.8/uvicore/auth/auth.py
--rw-r--r--   0        0        0       46 2021-03-13 03:32:22.776409 uvicore-0.1.8/uvicore/auth/authenticators/__init__.py
--rw-r--r--   0        0        0     2141 2021-03-22 15:01:04.718027 uvicore-0.1.8/uvicore/auth/authenticators/base.py
--rw-r--r--   0        0        0     2451 2021-03-22 15:01:04.718027 uvicore-0.1.8/uvicore/auth/authenticators/basic.py
--rw-r--r--   0        0        0     5902 2021-03-22 15:01:04.718027 uvicore-0.1.8/uvicore/auth/authenticators/jwt.py
--rw-r--r--   0        0        0      102 2020-09-30 23:16:47.907315 uvicore-0.1.8/uvicore/auth/commands/db.py
--rw-r--r--   0        0        0     2980 2021-03-02 19:39:30.880258 uvicore-0.1.8/uvicore/auth/config/package.py
--rw-r--r--   0        0        0       80 2020-11-29 06:49:41.064263 uvicore-0.1.8/uvicore/auth/contractsOLD/__init__.py
--rw-r--r--   0        0        0      343 2020-11-29 06:49:41.064263 uvicore-0.1.8/uvicore/auth/contractsOLD/group.py
--rw-r--r--   0        0        0      404 2020-11-29 06:49:41.064263 uvicore-0.1.8/uvicore/auth/contractsOLD/user.py
--rw-r--r--   0        0        0      414 2020-11-29 06:49:41.064263 uvicore-0.1.8/uvicore/auth/contractsOLD/user_info.py
--rw-r--r--   0        0        0      291 2021-03-04 01:20:55.374569 uvicore-0.1.8/uvicore/auth/database/seeders/__init__.py
--rw-r--r--   0        0        0      727 2021-03-22 16:30:17.120378 uvicore-0.1.8/uvicore/auth/database/seeders/groups.py
--rw-r--r--   0        0        0     1376 2021-03-04 01:20:55.374569 uvicore-0.1.8/uvicore/auth/database/seeders/permissions.py
--rw-r--r--   0        0        0      901 2021-03-22 16:34:48.566697 uvicore-0.1.8/uvicore/auth/database/seeders/roles.py
--rw-r--r--   0        0        0      994 2021-03-22 16:35:52.681797 uvicore-0.1.8/uvicore/auth/database/seeders/users.py
--rw-r--r--   0        0        0      266 2021-03-04 01:20:55.374569 uvicore-0.1.8/uvicore/auth/database/tables/__init__.py
--rw-r--r--   0        0        0     1108 2021-03-02 19:39:30.880258 uvicore-0.1.8/uvicore/auth/database/tables/group_roles.py
--rw-r--r--   0        0        0      902 2021-03-02 19:39:30.880258 uvicore-0.1.8/uvicore/auth/database/tables/groups.py
--rw-r--r--   0        0        0      908 2021-03-02 19:39:30.880258 uvicore-0.1.8/uvicore/auth/database/tables/permissions.py
--rw-r--r--   0        0        0     1143 2021-03-02 19:39:30.880258 uvicore-0.1.8/uvicore/auth/database/tables/role_permissions.py
--rw-r--r--   0        0        0      894 2021-03-22 16:34:58.619773 uvicore-0.1.8/uvicore/auth/database/tables/roles.py
--rw-r--r--   0        0        0     1211 2021-03-02 19:39:30.880258 uvicore-0.1.8/uvicore/auth/database/tables/user_groups.py
--rw-r--r--   0        0        0     1101 2021-03-04 01:20:55.374569 uvicore-0.1.8/uvicore/auth/database/tables/user_roles.py
--rw-r--r--   0        0        0     2174 2021-03-22 15:01:04.718027 uvicore-0.1.8/uvicore/auth/database/tables/users.py
--rw-r--r--   0        0        0       26 2021-01-28 23:57:53.792892 uvicore-0.1.8/uvicore/auth/http/public/assets/js/app.js
--rw-r--r--   0        0        0        2 2021-01-28 23:57:53.792892 uvicore-0.1.8/uvicore/auth/http/public/robots.txt
--rw-r--r--   0        0        0       15 2021-01-28 23:57:53.792892 uvicore-0.1.8/uvicore/auth/http/public/test.txt
--rw-r--r--   0        0        0       73 2021-03-14 14:29:52.918516 uvicore-0.1.8/uvicore/auth/middleware/__init__.py
--rw-r--r--   0        0        0     9337 2021-03-14 14:29:52.918516 uvicore-0.1.8/uvicore/auth/middleware/auth_OLD.py
--rw-r--r--   0        0        0     3102 2021-03-13 03:32:22.779743 uvicore-0.1.8/uvicore/auth/middleware/basic_OLD.py
--rw-r--r--   0        0        0     7288 2021-03-13 03:32:22.779743 uvicore-0.1.8/uvicore/auth/middleware/jwt_OLD.py
--rw-r--r--   0        0        0      106 2021-03-02 19:39:30.880258 uvicore-0.1.8/uvicore/auth/models/__init__.py
--rw-r--r--   0        0        0     1008 2021-03-02 19:39:30.880258 uvicore-0.1.8/uvicore/auth/models/group.py
--rw-r--r--   0        0        0      707 2021-03-02 19:39:30.880258 uvicore-0.1.8/uvicore/auth/models/permission.py
--rw-r--r--   0        0        0     1073 2021-03-22 16:35:03.689644 uvicore-0.1.8/uvicore/auth/models/role.py
--rw-r--r--   0        0        0     3756 2021-03-22 16:14:54.240910 uvicore-0.1.8/uvicore/auth/models/user.py
--rw-r--r--   0        0        0     2965 2021-03-02 19:39:30.880258 uvicore-0.1.8/uvicore/auth/services.py
--rw-r--r--   0        0        0     1408 2021-03-02 19:39:30.880258 uvicore-0.1.8/uvicore/auth/support/password.py
--rw-r--r--   0        0        0     2611 2021-03-14 14:29:52.918516 uvicore-0.1.8/uvicore/auth/user.py
--rw-r--r--   0        0        0       42 2021-03-13 03:32:22.779743 uvicore-0.1.8/uvicore/auth/user_providers/__init__.py
--rw-r--r--   0        0        0     3018 2021-03-22 15:01:04.718027 uvicore-0.1.8/uvicore/auth/user_providers/jwt.py
--rw-r--r--   0        0        0     6090 2021-03-22 16:33:01.604157 uvicore-0.1.8/uvicore/auth/user_providers/orm.py
--rw-r--r--   0        0        0       25 2021-03-02 19:39:30.880258 uvicore-0.1.8/uvicore/cache/backends/__init__.py
--rw-r--r--   0        0        0     6614 2021-03-02 19:39:30.880258 uvicore-0.1.8/uvicore/cache/backends/redis.py
--rw-r--r--   0        0        0      619 2021-03-02 19:39:30.880258 uvicore-0.1.8/uvicore/cache/handlers/bootstrap.py
--rw-r--r--   0        0        0     1526 2021-03-02 19:39:30.880258 uvicore-0.1.8/uvicore/cache/manager.py
--rw-r--r--   0        0        0     1264 2021-03-02 19:39:30.880258 uvicore-0.1.8/uvicore/cache/services.py
--rw-r--r--   0        0        0      464 2020-11-29 06:49:41.067596 uvicore-0.1.8/uvicore/configuration/__init__.py
--rw-r--r--   0        0        0      815 2021-01-22 23:57:24.015514 uvicore-0.1.8/uvicore/configuration/commands/config.py
--rw-r--r--   0        0        0     2739 2021-03-02 19:39:30.880258 uvicore-0.1.8/uvicore/configuration/configuration.py
--rw-r--r--   0        0        0     2189 2021-03-02 19:39:30.880258 uvicore-0.1.8/uvicore/configuration/services.py
--rw-r--r--   0        0        0      615 2021-03-02 19:39:30.880258 uvicore-0.1.8/uvicore/console/__init__.py
--rw-r--r--   0        0        0     6010 2020-09-30 23:16:47.907315 uvicore-0.1.8/uvicore/console/click_colors.py
--rw-r--r--   0        0        0      191 2020-12-31 21:18:43.988616 uvicore-0.1.8/uvicore/console/commands/generators.py
--rw-r--r--   0        0        0      205 2021-01-19 20:08:05.748406 uvicore-0.1.8/uvicore/console/commands/stubs/command.py
--rw-r--r--   0        0        0     1995 2021-03-02 19:39:30.880258 uvicore-0.1.8/uvicore/console/console.py
--rw-r--r--   0        0        0      640 2020-11-30 00:42:15.223566 uvicore-0.1.8/uvicore/console/decorators.py
--rw-r--r--   0        0        0     2430 2021-03-02 19:39:30.880258 uvicore-0.1.8/uvicore/console/handlers/bootstrap.py
--rw-r--r--   0        0        0     1137 2021-03-02 19:39:30.880258 uvicore-0.1.8/uvicore/console/provider.py
--rw-r--r--   0        0        0     1414 2021-03-02 19:39:30.880258 uvicore-0.1.8/uvicore/console/services.py
--rw-r--r--   0        0        0      101 2020-11-29 06:49:41.070929 uvicore-0.1.8/uvicore/container/__init__.py
--rw-r--r--   0        0        0     2234 2021-03-02 19:39:30.880258 uvicore-0.1.8/uvicore/container/commands/ioc.py
--rw-r--r--   0        0        0    12755 2021-03-02 19:39:30.880258 uvicore-0.1.8/uvicore/container/ioc.py
--rw-r--r--   0        0        0     1043 2021-03-13 03:32:22.779743 uvicore-0.1.8/uvicore/contracts/__init__.py
--rw-r--r--   0        0        0     3226 2021-03-02 19:39:30.880258 uvicore-0.1.8/uvicore/contracts/application.py
--rw-r--r--   0        0        0      552 2021-03-22 15:01:04.718027 uvicore-0.1.8/uvicore/contracts/authenticator.py
--rw-r--r--   0        0        0     3872 2021-03-20 03:33:25.304279 uvicore-0.1.8/uvicore/contracts/builder.py
--rw-r--r--   0        0        0     2002 2021-03-02 19:39:30.880258 uvicore-0.1.8/uvicore/contracts/cache.py
--rw-r--r--   0        0        0      828 2021-01-23 07:50:00.140302 uvicore-0.1.8/uvicore/contracts/config.py
--rw-r--r--   0        0        0      781 2021-01-23 08:40:53.308916 uvicore-0.1.8/uvicore/contracts/connection.py
--rw-r--r--   0        0        0     4951 2020-12-03 22:25:41.581951 uvicore-0.1.8/uvicore/contracts/database.py
--rw-r--r--   0        0        0     2110 2021-03-02 19:39:30.880258 uvicore-0.1.8/uvicore/contracts/dispatcher.py
--rw-r--r--   0        0        0      564 2021-03-02 19:39:30.880258 uvicore-0.1.8/uvicore/contracts/event.py
--rw-r--r--   0        0        0      652 2020-11-29 06:49:41.074262 uvicore-0.1.8/uvicore/contracts/field.py
--rw-r--r--   0        0        0     2109 2021-03-02 19:39:30.883592 uvicore-0.1.8/uvicore/contracts/ioc.py
--rw-r--r--   0        0        0     2423 2020-10-25 05:26:03.842510 uvicore-0.1.8/uvicore/contracts/logger.py
--rw-r--r--   0        0        0      288 2020-11-29 06:49:41.074262 uvicore-0.1.8/uvicore/contracts/mapper.py
--rw-r--r--   0        0        0     3814 2021-03-02 19:39:30.883592 uvicore-0.1.8/uvicore/contracts/model.py
--rw-r--r--   0        0        0     3070 2021-03-22 15:01:04.718027 uvicore-0.1.8/uvicore/contracts/package.py
--rw-r--r--   0        0        0     2610 2021-01-22 23:57:24.015514 uvicore-0.1.8/uvicore/contracts/provider.py
--rw-r--r--   0        0        0      742 2020-11-29 06:49:41.074262 uvicore-0.1.8/uvicore/contracts/relation.py
--rw-r--r--   0        0        0     3232 2021-03-14 14:29:52.918516 uvicore-0.1.8/uvicore/contracts/router.py
--rw-r--r--   0        0        0      808 2021-03-02 19:39:30.883592 uvicore-0.1.8/uvicore/contracts/routes-OLD.py
--rw-r--r--   0        0        0      496 2020-09-30 23:16:47.910648 uvicore-0.1.8/uvicore/contracts/server.py
--rw-r--r--   0        0        0      534 2020-09-30 23:16:47.910648 uvicore-0.1.8/uvicore/contracts/template.py
--rw-r--r--   0        0        0     2225 2021-03-12 00:13:43.690341 uvicore-0.1.8/uvicore/contracts/user.py
--rw-r--r--   0        0        0     2784 2021-03-22 15:01:04.718027 uvicore-0.1.8/uvicore/contracts/user_provider.py
--rw-r--r--   0        0        0     5329 2020-09-30 23:16:47.910648 uvicore-0.1.8/uvicore/database/OBSOLETE/OLD-__init__.py
--rw-r--r--   0        0        0     1645 2020-09-30 23:16:47.910648 uvicore-0.1.8/uvicore/database/OBSOLETE/db_OLD.py
--rw-r--r--   0        0        0     3845 2020-09-30 23:16:47.910648 uvicore-0.1.8/uvicore/database/OBSOLETE/db_OLD2.py
--rw-r--r--   0        0        0     3620 2020-09-30 23:16:47.910648 uvicore-0.1.8/uvicore/database/OBSOLETE/db_OLD_sync.py
--rw-r--r--   0        0        0     1303 2020-09-30 23:16:47.910648 uvicore-0.1.8/uvicore/database/OBSOLETE/idea__init__.py
--rw-r--r--   0        0        0      689 2021-03-02 19:39:30.883592 uvicore-0.1.8/uvicore/database/__init__.py
--rw-r--r--   0        0        0    17002 2021-03-02 19:39:30.883592 uvicore-0.1.8/uvicore/database/builder.py
--rw-r--r--   0        0        0     7873 2021-03-02 19:39:30.883592 uvicore-0.1.8/uvicore/database/commands/db.py
--rw-r--r--   0        0        0     1094 2021-01-19 20:08:05.748406 uvicore-0.1.8/uvicore/database/commands/generators.py
--rw-r--r--   0        0        0      583 2021-03-02 19:39:30.883592 uvicore-0.1.8/uvicore/database/commands/stubs/seeder.py
--rw-r--r--   0        0        0     1764 2021-01-19 20:08:05.748406 uvicore-0.1.8/uvicore/database/commands/stubs/table.py
--rw-r--r--   0        0        0    11208 2021-03-20 03:33:42.111173 uvicore-0.1.8/uvicore/database/db.py
--rw-r--r--   0        0        0     1744 2021-03-02 19:39:30.883592 uvicore-0.1.8/uvicore/database/handlers/bootstrap.py
--rw-r--r--   0        0        0     3271 2021-03-02 19:39:30.883592 uvicore-0.1.8/uvicore/database/provider.py
--rw-r--r--   0        0        0     5085 2021-03-20 03:33:34.624404 uvicore-0.1.8/uvicore/database/query.py
--rw-r--r--   0        0        0     1873 2021-03-02 19:39:30.883592 uvicore-0.1.8/uvicore/database/services.py
--rw-r--r--   0        0        0     2962 2020-12-03 22:25:41.585284 uvicore-0.1.8/uvicore/database/table.py
--rw-r--r--   0        0        0      287 2021-03-02 19:39:30.883592 uvicore-0.1.8/uvicore/events/__init__.py
--rw-r--r--   0        0        0     1196 2021-03-02 19:39:30.883592 uvicore-0.1.8/uvicore/events/commands/event.py
--rw-r--r--   0        0        0    12127 2021-03-02 19:39:30.883592 uvicore-0.1.8/uvicore/events/dispatcher.py
--rw-r--r--   0        0        0     1715 2021-03-02 19:39:30.883592 uvicore-0.1.8/uvicore/events/event.py
--rw-r--r--   0        0        0      143 2021-03-02 19:39:30.883592 uvicore-0.1.8/uvicore/events/handler.py
--rw-r--r--   0        0        0       49 2020-09-30 23:16:47.910648 uvicore-0.1.8/uvicore/factories/__init__.py
--rw-r--r--   0        0        0      252 2020-09-30 23:16:47.910648 uvicore-0.1.8/uvicore/factories/logger.py
--rw-r--r--   0        0        0    11209 2021-03-22 15:01:04.718027 uvicore-0.1.8/uvicore/foundation/application.py
--rw-r--r--   0        0        0     3590 2021-03-02 19:39:30.883592 uvicore-0.1.8/uvicore/foundation/config/package.py
--rw-r--r--   0        0        0      224 2021-03-02 19:39:30.883592 uvicore-0.1.8/uvicore/foundation/decorators/__init__.py
--rw-r--r--   0        0        0      439 2021-03-02 19:39:30.883592 uvicore-0.1.8/uvicore/foundation/decorators/controller.py
--rw-r--r--   0        0        0      472 2021-03-02 19:39:30.883592 uvicore-0.1.8/uvicore/foundation/decorators/event.py
--rw-r--r--   0        0        0      522 2021-03-02 19:39:30.883592 uvicore-0.1.8/uvicore/foundation/decorators/model.py
--rw-r--r--   0        0        0      482 2021-03-02 19:39:30.883592 uvicore-0.1.8/uvicore/foundation/decorators/provider.py
--rw-r--r--   0        0        0      431 2021-03-02 19:39:30.883592 uvicore-0.1.8/uvicore/foundation/decorators/routes.py
--rw-r--r--   0        0        0      475 2021-03-02 19:39:30.883592 uvicore-0.1.8/uvicore/foundation/decorators/seeder.py
--rw-r--r--   0        0        0      637 2021-03-02 19:39:30.883592 uvicore-0.1.8/uvicore/foundation/decorators/service.py
--rw-r--r--   0        0        0      470 2021-03-02 19:39:30.883592 uvicore-0.1.8/uvicore/foundation/decorators/table.py
--rw-r--r--   0        0        0      893 2021-03-02 19:39:30.883592 uvicore-0.1.8/uvicore/foundation/events/app.py
--rw-r--r--   0        0        0     4314 2021-03-02 19:39:30.883592 uvicore-0.1.8/uvicore/foundation/services.py
--rw-r--r--   0        0        0      749 2020-09-30 23:16:47.913981 uvicore-0.1.8/uvicore/http/OBSOLETE/router.py
--rw-r--r--   0        0        0     1956 2021-03-02 19:39:30.883592 uvicore-0.1.8/uvicore/http/OBSOLETE/routes-OLD.py
--rw-r--r--   0        0        0      772 2021-03-02 19:39:30.883592 uvicore-0.1.8/uvicore/http/__init__.py
--rw-r--r--   0        0        0    19213 2021-03-22 16:25:35.129592 uvicore-0.1.8/uvicore/http/bootstrap.py
--rw-r--r--   0        0        0      570 2020-12-02 20:34:40.502696 uvicore-0.1.8/uvicore/http/commands/serve.py
--rw-r--r--   0        0        0       62 2021-03-02 19:39:30.883592 uvicore-0.1.8/uvicore/http/controllers/__init__.py
--rw-r--r--   0        0        0     5354 2021-03-02 19:39:30.883592 uvicore-0.1.8/uvicore/http/controllers/api.py
--rw-r--r--   0        0        0     5908 2021-03-02 19:39:30.883592 uvicore-0.1.8/uvicore/http/controllers/web.py
--rw-r--r--   0        0        0      788 2021-03-02 19:39:30.883592 uvicore-0.1.8/uvicore/http/events/server.py
--rw-r--r--   0        0        0     2023 2021-03-22 16:41:07.059577 uvicore-0.1.8/uvicore/http/exceptions.py
--rw-r--r--   0        0        0      845 2021-03-13 03:32:22.779743 uvicore-0.1.8/uvicore/http/middleware/__init__.py
--rw-r--r--   0        0        0    10470 2021-03-22 16:32:02.700665 uvicore-0.1.8/uvicore/http/middleware/authentication.py
--rw-r--r--   0        0        0     4441 2021-03-02 19:39:30.883592 uvicore-0.1.8/uvicore/http/provider.py
--rw-r--r--   0        0        0       99 2021-03-13 03:32:22.779743 uvicore-0.1.8/uvicore/http/request.py
--rw-r--r--   0        0        0     1192 2021-03-13 03:32:22.779743 uvicore-0.1.8/uvicore/http/response.py
--rw-r--r--   0        0        0      299 2021-03-14 14:29:52.918516 uvicore-0.1.8/uvicore/http/routing/__init__.py
--rw-r--r--   0        0        0     9434 2021-03-22 17:12:04.335115 uvicore-0.1.8/uvicore/http/routing/api_router.py
--rw-r--r--   0        0        0     4655 2021-03-22 15:01:04.718027 uvicore-0.1.8/uvicore/http/routing/guard.py
--rw-r--r--   0        0        0    10967 2021-03-14 14:29:52.918516 uvicore-0.1.8/uvicore/http/routing/model_router.py
--rw-r--r--   0        0        0    19365 2021-03-22 17:13:45.480842 uvicore-0.1.8/uvicore/http/routing/router.py
--rw-r--r--   0        0        0     9840 2021-03-22 17:12:27.454889 uvicore-0.1.8/uvicore/http/routing/web_router.py
--rw-r--r--   0        0        0     3521 2021-03-02 19:39:30.883592 uvicore-0.1.8/uvicore/http/server.py
--rw-r--r--   0        0        0      797 2021-03-02 19:39:30.883592 uvicore-0.1.8/uvicore/http/servers/api.py
--rw-r--r--   0        0        0      393 2021-03-02 19:39:30.883592 uvicore-0.1.8/uvicore/http/servers/web.py
--rw-r--r--   0        0        0     6296 2021-03-02 19:39:30.883592 uvicore-0.1.8/uvicore/http/services.py
--rw-r--r--   0        0        0      865 2021-03-02 19:39:30.883592 uvicore-0.1.8/uvicore/http/static.py
--rw-r--r--   0        0        0     2517 2021-03-02 19:39:30.883592 uvicore-0.1.8/uvicore/http/status.py
--rw-r--r--   0        0        0      778 2021-03-22 15:01:04.718027 uvicore-0.1.8/uvicore/http/templating/context_functions.py
--rw-r--r--   0        0        0     2803 2021-03-02 19:39:30.883592 uvicore-0.1.8/uvicore/http/templating/jinja.py
--rw-r--r--   0        0        0    15001 2021-03-02 19:39:30.886925 uvicore-0.1.8/uvicore/logging/logger.py
--rw-r--r--   0        0        0     2092 2021-03-02 19:39:30.886925 uvicore-0.1.8/uvicore/logging/services.py
--rw-r--r--   0        0        0      166 2020-12-03 22:25:41.585284 uvicore-0.1.8/uvicore/orm/__init__.py
--rw-r--r--   0        0        0      756 2021-01-19 20:08:05.748406 uvicore-0.1.8/uvicore/orm/commands/generators.py
--rw-r--r--   0        0        0      874 2021-01-19 20:08:05.748406 uvicore-0.1.8/uvicore/orm/commands/stubs/model.py
--rw-r--r--   0        0        0    13770 2021-03-02 19:39:30.886925 uvicore-0.1.8/uvicore/orm/fields.py
--rw-r--r--   0        0        0     6025 2021-03-02 19:39:30.886925 uvicore-0.1.8/uvicore/orm/mapper.py
--rw-r--r--   0        0        0    16061 2021-03-02 19:39:30.886925 uvicore-0.1.8/uvicore/orm/metaclass.py
--rw-r--r--   0        0        0    30594 2021-03-22 16:24:48.129457 uvicore-0.1.8/uvicore/orm/model.py
--rw-r--r--   0        0        0    45210 2021-03-11 01:41:18.329097 uvicore-0.1.8/uvicore/orm/query.py
--rw-r--r--   0        0        0     2100 2021-03-02 19:39:30.886925 uvicore-0.1.8/uvicore/orm/services.py
--rw-r--r--   0        0        0      450 2021-02-07 17:42:02.228208 uvicore-0.1.8/uvicore/package/__init__.py
--rw-r--r--   0        0        0     1859 2021-03-11 01:41:18.329097 uvicore-0.1.8/uvicore/package/commands/package.py
--rw-r--r--   0        0        0     2163 2021-03-04 01:20:55.377902 uvicore-0.1.8/uvicore/package/package.py
--rw-r--r--   0        0        0     3321 2021-03-02 19:39:30.886925 uvicore-0.1.8/uvicore/package/provider.py
--rw-r--r--   0        0        0       25 2021-03-02 19:39:30.886925 uvicore-0.1.8/uvicore/redis/__init__.py
--rw-r--r--   0        0        0     1083 2021-03-02 19:39:30.886925 uvicore-0.1.8/uvicore/redis/bootstrap.py
--rw-r--r--   0        0        0      397 2021-03-02 19:39:30.886925 uvicore-0.1.8/uvicore/redis/provider.py
--rw-r--r--   0        0        0     3260 2021-03-02 19:39:30.886925 uvicore-0.1.8/uvicore/redis/redis.py
--rw-r--r--   0        0        0      765 2021-03-02 19:39:30.886925 uvicore-0.1.8/uvicore/redis/services.py
--rw-r--r--   0        0        0      407 2020-09-30 23:16:47.913981 uvicore-0.1.8/uvicore/support/README.md
--rw-r--r--   0        0        0      296 2020-09-30 23:16:47.913981 uvicore-0.1.8/uvicore/support/classes.py
--rw-r--r--   0        0        0     3646 2021-01-22 23:57:24.015514 uvicore-0.1.8/uvicore/support/collection.py
--rw-r--r--   0        0        0     1650 2021-03-02 19:39:30.886925 uvicore-0.1.8/uvicore/support/concurrency.py
--rw-r--r--   0        0        0     1237 2021-03-02 19:39:30.886925 uvicore-0.1.8/uvicore/support/dictionary.py
--rw-r--r--   0        0        0     1680 2021-01-27 21:25:20.094702 uvicore-0.1.8/uvicore/support/dumper.py
--rw-r--r--   0        0        0      411 2021-03-02 19:39:30.886925 uvicore-0.1.8/uvicore/support/hash.py
--rw-r--r--   0        0        0     3771 2021-01-22 23:57:24.015514 uvicore-0.1.8/uvicore/support/module.py
--rw-r--r--   0        0        0      567 2020-09-30 23:16:47.917315 uvicore-0.1.8/uvicore/support/path.py
--rw-r--r--   0        0        0     1835 2021-01-19 20:08:05.748406 uvicore-0.1.8/uvicore/support/schematic.py
--rw-r--r--   0        0        0      623 2020-07-20 18:33:04.439377 uvicore-0.1.8/uvicore/support/singleton.py
--rw-r--r--   0        0        0     2066 2020-12-31 21:18:43.991950 uvicore-0.1.8/uvicore/support/str.py
--rw-r--r--   0        0        0     2330 2021-03-13 03:32:22.779743 uvicore-0.1.8/uvicore/typing/__init__.py
--rw-r--r--   0        0        0    11526 2021-03-02 19:39:30.886925 uvicore-0.1.8/uvicore/typing/dictionary.py
--rw-r--r--   0        0        0     5504 2021-03-22 20:33:26.851321 uvicore-0.1.8/setup.py
--rw-r--r--   0        0        0     4914 2021-03-22 20:33:26.851703 uvicore-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1082 2021-03-22 20:00:01.058788 uvicore-0.1.9/LICENSE
+-rw-r--r--   0        0        0     2517 2020-12-03 22:25:41.581951 uvicore-0.1.9/README.md
+-rw-r--r--   0        0        0     2657 2021-03-22 21:23:51.930854 uvicore-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     3537 2021-01-28 23:57:53.792892 uvicore-0.1.9/uvicore/NOTES.md
+-rw-r--r--   0        0        0     2055 2021-03-22 21:24:00.474229 uvicore-0.1.9/uvicore/__init__.py
+-rw-r--r--   0        0        0       23 2021-03-13 03:32:22.776409 uvicore-0.1.9/uvicore/auth/__init__.py
+-rw-r--r--   0        0        0       80 2021-02-18 23:17:24.966073 uvicore-0.1.9/uvicore/auth/auth.py
+-rw-r--r--   0        0        0       46 2021-03-13 03:32:22.776409 uvicore-0.1.9/uvicore/auth/authenticators/__init__.py
+-rw-r--r--   0        0        0     2141 2021-03-22 15:01:04.718027 uvicore-0.1.9/uvicore/auth/authenticators/base.py
+-rw-r--r--   0        0        0     2451 2021-03-22 15:01:04.718027 uvicore-0.1.9/uvicore/auth/authenticators/basic.py
+-rw-r--r--   0        0        0     5902 2021-03-22 15:01:04.718027 uvicore-0.1.9/uvicore/auth/authenticators/jwt.py
+-rw-r--r--   0        0        0      102 2020-09-30 23:16:47.907315 uvicore-0.1.9/uvicore/auth/commands/db.py
+-rw-r--r--   0        0        0     2980 2021-03-02 19:39:30.880258 uvicore-0.1.9/uvicore/auth/config/package.py
+-rw-r--r--   0        0        0       80 2020-11-29 06:49:41.064263 uvicore-0.1.9/uvicore/auth/contractsOLD/__init__.py
+-rw-r--r--   0        0        0      343 2020-11-29 06:49:41.064263 uvicore-0.1.9/uvicore/auth/contractsOLD/group.py
+-rw-r--r--   0        0        0      404 2020-11-29 06:49:41.064263 uvicore-0.1.9/uvicore/auth/contractsOLD/user.py
+-rw-r--r--   0        0        0      414 2020-11-29 06:49:41.064263 uvicore-0.1.9/uvicore/auth/contractsOLD/user_info.py
+-rw-r--r--   0        0        0      291 2021-03-04 01:20:55.374569 uvicore-0.1.9/uvicore/auth/database/seeders/__init__.py
+-rw-r--r--   0        0        0      727 2021-03-22 16:30:17.120378 uvicore-0.1.9/uvicore/auth/database/seeders/groups.py
+-rw-r--r--   0        0        0     1376 2021-03-04 01:20:55.374569 uvicore-0.1.9/uvicore/auth/database/seeders/permissions.py
+-rw-r--r--   0        0        0      901 2021-03-22 16:34:48.566697 uvicore-0.1.9/uvicore/auth/database/seeders/roles.py
+-rw-r--r--   0        0        0      994 2021-03-22 16:35:52.681797 uvicore-0.1.9/uvicore/auth/database/seeders/users.py
+-rw-r--r--   0        0        0      266 2021-03-04 01:20:55.374569 uvicore-0.1.9/uvicore/auth/database/tables/__init__.py
+-rw-r--r--   0        0        0     1108 2021-03-02 19:39:30.880258 uvicore-0.1.9/uvicore/auth/database/tables/group_roles.py
+-rw-r--r--   0        0        0      902 2021-03-02 19:39:30.880258 uvicore-0.1.9/uvicore/auth/database/tables/groups.py
+-rw-r--r--   0        0        0      908 2021-03-02 19:39:30.880258 uvicore-0.1.9/uvicore/auth/database/tables/permissions.py
+-rw-r--r--   0        0        0     1143 2021-03-02 19:39:30.880258 uvicore-0.1.9/uvicore/auth/database/tables/role_permissions.py
+-rw-r--r--   0        0        0      894 2021-03-22 16:34:58.619773 uvicore-0.1.9/uvicore/auth/database/tables/roles.py
+-rw-r--r--   0        0        0     1211 2021-03-02 19:39:30.880258 uvicore-0.1.9/uvicore/auth/database/tables/user_groups.py
+-rw-r--r--   0        0        0     1101 2021-03-04 01:20:55.374569 uvicore-0.1.9/uvicore/auth/database/tables/user_roles.py
+-rw-r--r--   0        0        0     2174 2021-03-22 15:01:04.718027 uvicore-0.1.9/uvicore/auth/database/tables/users.py
+-rw-r--r--   0        0        0       26 2021-01-28 23:57:53.792892 uvicore-0.1.9/uvicore/auth/http/public/assets/js/app.js
+-rw-r--r--   0        0        0        2 2021-01-28 23:57:53.792892 uvicore-0.1.9/uvicore/auth/http/public/robots.txt
+-rw-r--r--   0        0        0       15 2021-01-28 23:57:53.792892 uvicore-0.1.9/uvicore/auth/http/public/test.txt
+-rw-r--r--   0        0        0       73 2021-03-14 14:29:52.918516 uvicore-0.1.9/uvicore/auth/middleware/__init__.py
+-rw-r--r--   0        0        0     9337 2021-03-14 14:29:52.918516 uvicore-0.1.9/uvicore/auth/middleware/auth_OLD.py
+-rw-r--r--   0        0        0     3102 2021-03-13 03:32:22.779743 uvicore-0.1.9/uvicore/auth/middleware/basic_OLD.py
+-rw-r--r--   0        0        0     7288 2021-03-13 03:32:22.779743 uvicore-0.1.9/uvicore/auth/middleware/jwt_OLD.py
+-rw-r--r--   0        0        0      106 2021-03-02 19:39:30.880258 uvicore-0.1.9/uvicore/auth/models/__init__.py
+-rw-r--r--   0        0        0     1008 2021-03-02 19:39:30.880258 uvicore-0.1.9/uvicore/auth/models/group.py
+-rw-r--r--   0        0        0      707 2021-03-02 19:39:30.880258 uvicore-0.1.9/uvicore/auth/models/permission.py
+-rw-r--r--   0        0        0     1073 2021-03-22 16:35:03.689644 uvicore-0.1.9/uvicore/auth/models/role.py
+-rw-r--r--   0        0        0     3756 2021-03-22 16:14:54.240910 uvicore-0.1.9/uvicore/auth/models/user.py
+-rw-r--r--   0        0        0     2965 2021-03-02 19:39:30.880258 uvicore-0.1.9/uvicore/auth/services.py
+-rw-r--r--   0        0        0     1408 2021-03-02 19:39:30.880258 uvicore-0.1.9/uvicore/auth/support/password.py
+-rw-r--r--   0        0        0     2611 2021-03-14 14:29:52.918516 uvicore-0.1.9/uvicore/auth/user.py
+-rw-r--r--   0        0        0       42 2021-03-13 03:32:22.779743 uvicore-0.1.9/uvicore/auth/user_providers/__init__.py
+-rw-r--r--   0        0        0     3018 2021-03-22 15:01:04.718027 uvicore-0.1.9/uvicore/auth/user_providers/jwt.py
+-rw-r--r--   0        0        0     6090 2021-03-22 16:33:01.604157 uvicore-0.1.9/uvicore/auth/user_providers/orm.py
+-rw-r--r--   0        0        0       25 2021-03-02 19:39:30.880258 uvicore-0.1.9/uvicore/cache/backends/__init__.py
+-rw-r--r--   0        0        0     6614 2021-03-02 19:39:30.880258 uvicore-0.1.9/uvicore/cache/backends/redis.py
+-rw-r--r--   0        0        0     1526 2021-03-02 19:39:30.880258 uvicore-0.1.9/uvicore/cache/manager.py
+-rw-r--r--   0        0        0     1219 2021-03-22 20:59:23.397395 uvicore-0.1.9/uvicore/cache/services.py
+-rw-r--r--   0        0        0      464 2020-11-29 06:49:41.067596 uvicore-0.1.9/uvicore/configuration/__init__.py
+-rw-r--r--   0        0        0      815 2021-01-22 23:57:24.015514 uvicore-0.1.9/uvicore/configuration/commands/config.py
+-rw-r--r--   0        0        0     2739 2021-03-02 19:39:30.880258 uvicore-0.1.9/uvicore/configuration/configuration.py
+-rw-r--r--   0        0        0     2189 2021-03-02 19:39:30.880258 uvicore-0.1.9/uvicore/configuration/services.py
+-rw-r--r--   0        0        0      615 2021-03-02 19:39:30.880258 uvicore-0.1.9/uvicore/console/__init__.py
+-rw-r--r--   0        0        0     6010 2020-09-30 23:16:47.907315 uvicore-0.1.9/uvicore/console/click_colors.py
+-rw-r--r--   0        0        0      191 2020-12-31 21:18:43.988616 uvicore-0.1.9/uvicore/console/commands/generators.py
+-rw-r--r--   0        0        0      205 2021-01-19 20:08:05.748406 uvicore-0.1.9/uvicore/console/commands/stubs/command.py
+-rw-r--r--   0        0        0     1995 2021-03-02 19:39:30.880258 uvicore-0.1.9/uvicore/console/console.py
+-rw-r--r--   0        0        0      640 2020-11-30 00:42:15.223566 uvicore-0.1.9/uvicore/console/decorators.py
+-rw-r--r--   0        0        0     2430 2021-03-02 19:39:30.880258 uvicore-0.1.9/uvicore/console/handlers/bootstrap.py
+-rw-r--r--   0        0        0     1003 2021-03-22 20:58:24.497352 uvicore-0.1.9/uvicore/console/provider.py
+-rw-r--r--   0        0        0     1414 2021-03-02 19:39:30.880258 uvicore-0.1.9/uvicore/console/services.py
+-rw-r--r--   0        0        0      101 2020-11-29 06:49:41.070929 uvicore-0.1.9/uvicore/container/__init__.py
+-rw-r--r--   0        0        0     2234 2021-03-02 19:39:30.880258 uvicore-0.1.9/uvicore/container/commands/ioc.py
+-rw-r--r--   0        0        0    12755 2021-03-02 19:39:30.880258 uvicore-0.1.9/uvicore/container/ioc.py
+-rw-r--r--   0        0        0     1043 2021-03-22 21:21:29.780110 uvicore-0.1.9/uvicore/contracts/__init__.py
+-rw-r--r--   0        0        0     3226 2021-03-02 19:39:30.880258 uvicore-0.1.9/uvicore/contracts/application.py
+-rw-r--r--   0        0        0      593 2021-03-22 21:21:23.620075 uvicore-0.1.9/uvicore/contracts/authenticator.py
+-rw-r--r--   0        0        0     3959 2021-03-22 20:44:21.526141 uvicore-0.1.9/uvicore/contracts/builder.py
+-rw-r--r--   0        0        0     2002 2021-03-02 19:39:30.880258 uvicore-0.1.9/uvicore/contracts/cache.py
+-rw-r--r--   0        0        0      828 2021-01-23 07:50:00.140302 uvicore-0.1.9/uvicore/contracts/config.py
+-rw-r--r--   0        0        0      781 2021-01-23 08:40:53.308916 uvicore-0.1.9/uvicore/contracts/connection.py
+-rw-r--r--   0        0        0     5123 2021-03-22 20:46:33.139781 uvicore-0.1.9/uvicore/contracts/database.py
+-rw-r--r--   0        0        0     2110 2021-03-02 19:39:30.880258 uvicore-0.1.9/uvicore/contracts/dispatcher.py
+-rw-r--r--   0        0        0      564 2021-03-02 19:39:30.880258 uvicore-0.1.9/uvicore/contracts/event.py
+-rw-r--r--   0        0        0      652 2020-11-29 06:49:41.074262 uvicore-0.1.9/uvicore/contracts/field.py
+-rw-r--r--   0        0        0     2109 2021-03-02 19:39:30.883592 uvicore-0.1.9/uvicore/contracts/ioc.py
+-rw-r--r--   0        0        0     2423 2020-10-25 05:26:03.842510 uvicore-0.1.9/uvicore/contracts/logger.py
+-rw-r--r--   0        0        0      288 2020-11-29 06:49:41.074262 uvicore-0.1.9/uvicore/contracts/mapper.py
+-rw-r--r--   0        0        0     3814 2021-03-02 19:39:30.883592 uvicore-0.1.9/uvicore/contracts/model.py
+-rw-r--r--   0        0        0     3070 2021-03-22 15:01:04.718027 uvicore-0.1.9/uvicore/contracts/package.py
+-rw-r--r--   0        0        0     2610 2021-01-22 23:57:24.015514 uvicore-0.1.9/uvicore/contracts/provider.py
+-rw-r--r--   0        0        0      742 2020-11-29 06:49:41.074262 uvicore-0.1.9/uvicore/contracts/relation.py
+-rw-r--r--   0        0        0     3232 2021-03-14 14:29:52.918516 uvicore-0.1.9/uvicore/contracts/router.py
+-rw-r--r--   0        0        0      808 2021-03-02 19:39:30.883592 uvicore-0.1.9/uvicore/contracts/routes-OLD.py
+-rw-r--r--   0        0        0      532 2021-03-22 20:43:49.282721 uvicore-0.1.9/uvicore/contracts/server.py
+-rw-r--r--   0        0        0      534 2020-09-30 23:16:47.910648 uvicore-0.1.9/uvicore/contracts/template.py
+-rw-r--r--   0        0        0     2225 2021-03-12 00:13:43.690341 uvicore-0.1.9/uvicore/contracts/user.py
+-rw-r--r--   0        0        0     2884 2021-03-22 21:20:51.763224 uvicore-0.1.9/uvicore/contracts/user_provider.py
+-rw-r--r--   0        0        0     5329 2020-09-30 23:16:47.910648 uvicore-0.1.9/uvicore/database/OBSOLETE/OLD-__init__.py
+-rw-r--r--   0        0        0     1645 2020-09-30 23:16:47.910648 uvicore-0.1.9/uvicore/database/OBSOLETE/db_OLD.py
+-rw-r--r--   0        0        0     3845 2020-09-30 23:16:47.910648 uvicore-0.1.9/uvicore/database/OBSOLETE/db_OLD2.py
+-rw-r--r--   0        0        0     3620 2020-09-30 23:16:47.910648 uvicore-0.1.9/uvicore/database/OBSOLETE/db_OLD_sync.py
+-rw-r--r--   0        0        0     1303 2020-09-30 23:16:47.910648 uvicore-0.1.9/uvicore/database/OBSOLETE/idea__init__.py
+-rw-r--r--   0        0        0      689 2021-03-02 19:39:30.883592 uvicore-0.1.9/uvicore/database/__init__.py
+-rw-r--r--   0        0        0    17002 2021-03-02 19:39:30.883592 uvicore-0.1.9/uvicore/database/builder.py
+-rw-r--r--   0        0        0     7873 2021-03-02 19:39:30.883592 uvicore-0.1.9/uvicore/database/commands/db.py
+-rw-r--r--   0        0        0     1094 2021-01-19 20:08:05.748406 uvicore-0.1.9/uvicore/database/commands/generators.py
+-rw-r--r--   0        0        0      583 2021-03-02 19:39:30.883592 uvicore-0.1.9/uvicore/database/commands/stubs/seeder.py
+-rw-r--r--   0        0        0     1764 2021-01-19 20:08:05.748406 uvicore-0.1.9/uvicore/database/commands/stubs/table.py
+-rw-r--r--   0        0        0    11208 2021-03-20 03:33:42.111173 uvicore-0.1.9/uvicore/database/db.py
+-rw-r--r--   0        0        0     1744 2021-03-02 19:39:30.883592 uvicore-0.1.9/uvicore/database/handlers/bootstrap.py
+-rw-r--r--   0        0        0     3271 2021-03-02 19:39:30.883592 uvicore-0.1.9/uvicore/database/provider.py
+-rw-r--r--   0        0        0     5085 2021-03-20 03:33:34.624404 uvicore-0.1.9/uvicore/database/query.py
+-rw-r--r--   0        0        0     1873 2021-03-02 19:39:30.883592 uvicore-0.1.9/uvicore/database/services.py
+-rw-r--r--   0        0        0     2962 2020-12-03 22:25:41.585284 uvicore-0.1.9/uvicore/database/table.py
+-rw-r--r--   0        0        0      287 2021-03-02 19:39:30.883592 uvicore-0.1.9/uvicore/events/__init__.py
+-rw-r--r--   0        0        0     1196 2021-03-02 19:39:30.883592 uvicore-0.1.9/uvicore/events/commands/event.py
+-rw-r--r--   0        0        0    12127 2021-03-02 19:39:30.883592 uvicore-0.1.9/uvicore/events/dispatcher.py
+-rw-r--r--   0        0        0     1715 2021-03-02 19:39:30.883592 uvicore-0.1.9/uvicore/events/event.py
+-rw-r--r--   0        0        0      143 2021-03-02 19:39:30.883592 uvicore-0.1.9/uvicore/events/handler.py
+-rw-r--r--   0        0        0       49 2020-09-30 23:16:47.910648 uvicore-0.1.9/uvicore/factories/__init__.py
+-rw-r--r--   0        0        0      252 2020-09-30 23:16:47.910648 uvicore-0.1.9/uvicore/factories/logger.py
+-rw-r--r--   0        0        0    11169 2021-03-22 20:54:03.233785 uvicore-0.1.9/uvicore/foundation/application.py
+-rw-r--r--   0        0        0     3590 2021-03-02 19:39:30.883592 uvicore-0.1.9/uvicore/foundation/config/package.py
+-rw-r--r--   0        0        0      224 2021-03-02 19:39:30.883592 uvicore-0.1.9/uvicore/foundation/decorators/__init__.py
+-rw-r--r--   0        0        0      439 2021-03-02 19:39:30.883592 uvicore-0.1.9/uvicore/foundation/decorators/controller.py
+-rw-r--r--   0        0        0      472 2021-03-02 19:39:30.883592 uvicore-0.1.9/uvicore/foundation/decorators/event.py
+-rw-r--r--   0        0        0      522 2021-03-02 19:39:30.883592 uvicore-0.1.9/uvicore/foundation/decorators/model.py
+-rw-r--r--   0        0        0      482 2021-03-02 19:39:30.883592 uvicore-0.1.9/uvicore/foundation/decorators/provider.py
+-rw-r--r--   0        0        0      431 2021-03-02 19:39:30.883592 uvicore-0.1.9/uvicore/foundation/decorators/routes.py
+-rw-r--r--   0        0        0      475 2021-03-02 19:39:30.883592 uvicore-0.1.9/uvicore/foundation/decorators/seeder.py
+-rw-r--r--   0        0        0      637 2021-03-02 19:39:30.883592 uvicore-0.1.9/uvicore/foundation/decorators/service.py
+-rw-r--r--   0        0        0      470 2021-03-02 19:39:30.883592 uvicore-0.1.9/uvicore/foundation/decorators/table.py
+-rw-r--r--   0        0        0      893 2021-03-02 19:39:30.883592 uvicore-0.1.9/uvicore/foundation/events/app.py
+-rw-r--r--   0        0        0     4314 2021-03-02 19:39:30.883592 uvicore-0.1.9/uvicore/foundation/services.py
+-rw-r--r--   0        0        0      749 2020-09-30 23:16:47.913981 uvicore-0.1.9/uvicore/http/OBSOLETE/router.py
+-rw-r--r--   0        0        0     1956 2021-03-02 19:39:30.883592 uvicore-0.1.9/uvicore/http/OBSOLETE/routes-OLD.py
+-rw-r--r--   0        0        0      773 2021-03-22 21:05:40.394285 uvicore-0.1.9/uvicore/http/__init__.py
+-rw-r--r--   0        0        0    19213 2021-03-22 16:25:35.129592 uvicore-0.1.9/uvicore/http/bootstrap.py
+-rw-r--r--   0        0        0      570 2020-12-02 20:34:40.502696 uvicore-0.1.9/uvicore/http/commands/serve.py
+-rw-r--r--   0        0        0       62 2021-03-02 19:39:30.883592 uvicore-0.1.9/uvicore/http/controllers/__init__.py
+-rw-r--r--   0        0        0     5354 2021-03-02 19:39:30.883592 uvicore-0.1.9/uvicore/http/controllers/api.py
+-rw-r--r--   0        0        0     5908 2021-03-02 19:39:30.883592 uvicore-0.1.9/uvicore/http/controllers/web.py
+-rw-r--r--   0        0        0      788 2021-03-02 19:39:30.883592 uvicore-0.1.9/uvicore/http/events/server.py
+-rw-r--r--   0        0        0     2023 2021-03-22 16:41:07.059577 uvicore-0.1.9/uvicore/http/exceptions.py
+-rw-r--r--   0        0        0      845 2021-03-13 03:32:22.779743 uvicore-0.1.9/uvicore/http/middleware/__init__.py
+-rw-r--r--   0        0        0    10470 2021-03-22 16:32:02.700665 uvicore-0.1.9/uvicore/http/middleware/authentication.py
+-rw-r--r--   0        0        0     4441 2021-03-02 19:39:30.883592 uvicore-0.1.9/uvicore/http/provider.py
+-rw-r--r--   0        0        0       99 2021-03-22 20:51:34.440278 uvicore-0.1.9/uvicore/http/request.py
+-rw-r--r--   0        0        0     1192 2021-03-13 03:32:22.779743 uvicore-0.1.9/uvicore/http/response.py
+-rw-r--r--   0        0        0      299 2021-03-14 14:29:52.918516 uvicore-0.1.9/uvicore/http/routing/__init__.py
+-rw-r--r--   0        0        0     9434 2021-03-22 17:12:04.335115 uvicore-0.1.9/uvicore/http/routing/api_router.py
+-rw-r--r--   0        0        0     4655 2021-03-22 15:01:04.718027 uvicore-0.1.9/uvicore/http/routing/guard.py
+-rw-r--r--   0        0        0    10967 2021-03-14 14:29:52.918516 uvicore-0.1.9/uvicore/http/routing/model_router.py
+-rw-r--r--   0        0        0    19365 2021-03-22 17:13:45.480842 uvicore-0.1.9/uvicore/http/routing/router.py
+-rw-r--r--   0        0        0     9840 2021-03-22 17:12:27.454889 uvicore-0.1.9/uvicore/http/routing/web_router.py
+-rw-r--r--   0        0        0     3521 2021-03-02 19:39:30.883592 uvicore-0.1.9/uvicore/http/server.py
+-rw-r--r--   0        0        0      797 2021-03-02 19:39:30.883592 uvicore-0.1.9/uvicore/http/servers/api.py
+-rw-r--r--   0        0        0      393 2021-03-02 19:39:30.883592 uvicore-0.1.9/uvicore/http/servers/web.py
+-rw-r--r--   0        0        0     6296 2021-03-02 19:39:30.883592 uvicore-0.1.9/uvicore/http/services.py
+-rw-r--r--   0        0        0      865 2021-03-02 19:39:30.883592 uvicore-0.1.9/uvicore/http/static.py
+-rw-r--r--   0        0        0     2517 2021-03-02 19:39:30.883592 uvicore-0.1.9/uvicore/http/status.py
+-rw-r--r--   0        0        0      778 2021-03-22 15:01:04.718027 uvicore-0.1.9/uvicore/http/templating/context_functions.py
+-rw-r--r--   0        0        0     2803 2021-03-02 19:39:30.883592 uvicore-0.1.9/uvicore/http/templating/jinja.py
+-rw-r--r--   0        0        0    15001 2021-03-02 19:39:30.886925 uvicore-0.1.9/uvicore/logging/logger.py
+-rw-r--r--   0        0        0     2092 2021-03-02 19:39:30.886925 uvicore-0.1.9/uvicore/logging/services.py
+-rw-r--r--   0        0        0      166 2020-12-03 22:25:41.585284 uvicore-0.1.9/uvicore/orm/__init__.py
+-rw-r--r--   0        0        0      756 2021-01-19 20:08:05.748406 uvicore-0.1.9/uvicore/orm/commands/generators.py
+-rw-r--r--   0        0        0      874 2021-01-19 20:08:05.748406 uvicore-0.1.9/uvicore/orm/commands/stubs/model.py
+-rw-r--r--   0        0        0    13770 2021-03-02 19:39:30.886925 uvicore-0.1.9/uvicore/orm/fields.py
+-rw-r--r--   0        0        0     6025 2021-03-02 19:39:30.886925 uvicore-0.1.9/uvicore/orm/mapper.py
+-rw-r--r--   0        0        0    16061 2021-03-02 19:39:30.886925 uvicore-0.1.9/uvicore/orm/metaclass.py
+-rw-r--r--   0        0        0    30594 2021-03-22 16:24:48.129457 uvicore-0.1.9/uvicore/orm/model.py
+-rw-r--r--   0        0        0    45210 2021-03-11 01:41:18.329097 uvicore-0.1.9/uvicore/orm/query.py
+-rw-r--r--   0        0        0     2100 2021-03-02 19:39:30.886925 uvicore-0.1.9/uvicore/orm/services.py
+-rw-r--r--   0        0        0      450 2021-02-07 17:42:02.228208 uvicore-0.1.9/uvicore/package/__init__.py
+-rw-r--r--   0        0        0     1859 2021-03-11 01:41:18.329097 uvicore-0.1.9/uvicore/package/commands/package.py
+-rw-r--r--   0        0        0     2163 2021-03-04 01:20:55.377902 uvicore-0.1.9/uvicore/package/package.py
+-rw-r--r--   0        0        0     3321 2021-03-02 19:39:30.886925 uvicore-0.1.9/uvicore/package/provider.py
+-rw-r--r--   0        0        0       25 2021-03-02 19:39:30.886925 uvicore-0.1.9/uvicore/redis/__init__.py
+-rw-r--r--   0        0        0     1083 2021-03-02 19:39:30.886925 uvicore-0.1.9/uvicore/redis/bootstrap.py
+-rw-r--r--   0        0        0      263 2021-03-22 21:08:01.565148 uvicore-0.1.9/uvicore/redis/provider.py
+-rw-r--r--   0        0        0     3260 2021-03-02 19:39:30.886925 uvicore-0.1.9/uvicore/redis/redis.py
+-rw-r--r--   0        0        0      765 2021-03-02 19:39:30.886925 uvicore-0.1.9/uvicore/redis/services.py
+-rw-r--r--   0        0        0      407 2020-09-30 23:16:47.913981 uvicore-0.1.9/uvicore/support/README.md
+-rw-r--r--   0        0        0      296 2020-09-30 23:16:47.913981 uvicore-0.1.9/uvicore/support/classes.py
+-rw-r--r--   0        0        0     3646 2021-01-22 23:57:24.015514 uvicore-0.1.9/uvicore/support/collection.py
+-rw-r--r--   0        0        0     2419 2021-03-22 20:57:40.140650 uvicore-0.1.9/uvicore/support/concurrency.py
+-rw-r--r--   0        0        0     1237 2021-03-02 19:39:30.886925 uvicore-0.1.9/uvicore/support/dictionary.py
+-rw-r--r--   0        0        0     1680 2021-01-27 21:25:20.094702 uvicore-0.1.9/uvicore/support/dumper.py
+-rw-r--r--   0        0        0      411 2021-03-02 19:39:30.886925 uvicore-0.1.9/uvicore/support/hash.py
+-rw-r--r--   0        0        0     3771 2021-03-22 21:01:26.820810 uvicore-0.1.9/uvicore/support/module.py
+-rw-r--r--   0        0        0      567 2020-09-30 23:16:47.917315 uvicore-0.1.9/uvicore/support/path.py
+-rw-r--r--   0        0        0     1835 2021-01-19 20:08:05.748406 uvicore-0.1.9/uvicore/support/schematic.py
+-rw-r--r--   0        0        0      623 2020-07-20 18:33:04.439377 uvicore-0.1.9/uvicore/support/singleton.py
+-rw-r--r--   0        0        0     2066 2020-12-31 21:18:43.991950 uvicore-0.1.9/uvicore/support/str.py
+-rw-r--r--   0        0        0     2437 2021-03-22 21:15:13.387409 uvicore-0.1.9/uvicore/typing/__init__.py
+-rw-r--r--   0        0        0    11526 2021-03-02 19:39:30.886925 uvicore-0.1.9/uvicore/typing/dictionary.py
+-rw-r--r--   0        0        0     5477 2021-03-22 21:24:03.131033 uvicore-0.1.9/setup.py
+-rw-r--r--   0        0        0     4914 2021-03-22 21:24:03.131398 uvicore-0.1.9/PKG-INFO
```

### Comparing `uvicore-0.1.8/LICENSE` & `uvicore-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/README.md` & `uvicore-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/pyproject.toml` & `uvicore-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "uvicore"
-version = "0.1.8"
+version = "0.1.9"
 license = "MIT"
 authors = ["Matthew Reschke <mail@mreschke.com>"]
 description = "The Async Python Framework for Artisans. An Elegant Fullstack Python Web, API and CLI Framework"
 readme = "README.md"
 homepage = "https://github.com/uvicore/framework"
 documentation = "https://github.com/uvicore/framework"
 repository = "https://github.com/uvicore/framework"
```

### Comparing `uvicore-0.1.8/uvicore/NOTES.md` & `uvicore-0.1.9/uvicore/NOTES.md`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/__init__.py` & `uvicore-0.1.9/uvicore/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from . import contracts
 from uvicore.typing import Dict
 from uvicore.foundation.decorators import event, model, seeder, service, table, provider, routes, controller
 
 
 # Uvicore version.  Also available in app.version
-__version__ = '0.1.8'
+__version__ = '0.1.9'
 
 # Core (non service provider based) singletons as globals
 ioc: contracts.Ioc = None
 events: contracts.Dispatcher = None
 app: contracts.Application = None
 
 # Core (service provider based) singletons as globals
```

### Comparing `uvicore-0.1.8/uvicore/auth/authenticators/base.py` & `uvicore-0.1.9/uvicore/auth/authenticators/base.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/auth/authenticators/basic.py` & `uvicore-0.1.9/uvicore/auth/authenticators/basic.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/auth/authenticators/jwt.py` & `uvicore-0.1.9/uvicore/auth/authenticators/jwt.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/auth/config/package.py` & `uvicore-0.1.9/uvicore/auth/config/package.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/auth/database/seeders/groups.py` & `uvicore-0.1.9/uvicore/auth/database/seeders/groups.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/auth/database/seeders/permissions.py` & `uvicore-0.1.9/uvicore/auth/database/seeders/permissions.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/auth/database/seeders/roles.py` & `uvicore-0.1.9/uvicore/auth/database/seeders/roles.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/auth/database/seeders/users.py` & `uvicore-0.1.9/uvicore/auth/database/seeders/users.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/auth/database/tables/group_roles.py` & `uvicore-0.1.9/uvicore/auth/database/tables/group_roles.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/auth/database/tables/groups.py` & `uvicore-0.1.9/uvicore/auth/database/tables/groups.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/auth/database/tables/permissions.py` & `uvicore-0.1.9/uvicore/auth/database/tables/permissions.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/auth/database/tables/role_permissions.py` & `uvicore-0.1.9/uvicore/auth/database/tables/role_permissions.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/auth/database/tables/roles.py` & `uvicore-0.1.9/uvicore/auth/database/tables/roles.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/auth/database/tables/user_groups.py` & `uvicore-0.1.9/uvicore/auth/database/tables/user_groups.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/auth/database/tables/user_roles.py` & `uvicore-0.1.9/uvicore/auth/database/tables/user_roles.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/auth/database/tables/users.py` & `uvicore-0.1.9/uvicore/auth/database/tables/users.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/auth/middleware/auth_OLD.py` & `uvicore-0.1.9/uvicore/auth/middleware/auth_OLD.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/auth/middleware/basic_OLD.py` & `uvicore-0.1.9/uvicore/auth/middleware/basic_OLD.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/auth/middleware/jwt_OLD.py` & `uvicore-0.1.9/uvicore/auth/middleware/jwt_OLD.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/auth/models/group.py` & `uvicore-0.1.9/uvicore/auth/models/group.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/auth/models/permission.py` & `uvicore-0.1.9/uvicore/auth/models/permission.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/auth/models/role.py` & `uvicore-0.1.9/uvicore/auth/models/role.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/auth/models/user.py` & `uvicore-0.1.9/uvicore/auth/models/user.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/auth/services.py` & `uvicore-0.1.9/uvicore/auth/services.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/auth/support/password.py` & `uvicore-0.1.9/uvicore/auth/support/password.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/auth/user.py` & `uvicore-0.1.9/uvicore/auth/user.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/auth/user_providers/jwt.py` & `uvicore-0.1.9/uvicore/auth/user_providers/jwt.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/auth/user_providers/orm.py` & `uvicore-0.1.9/uvicore/auth/user_providers/orm.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/cache/backends/redis.py` & `uvicore-0.1.9/uvicore/cache/backends/redis.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/cache/manager.py` & `uvicore-0.1.9/uvicore/cache/manager.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/cache/services.py` & `uvicore-0.1.9/uvicore/cache/services.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import uvicore
 from uvicore.package import ServiceProvider
 from uvicore.support.dumper import dump, dd
-from uvicore.cache.handlers import bootstrap
 from uvicore.foundation.events import app as AppEvents
 
 
 @uvicore.provider()
 class Cache(ServiceProvider):
 
     def register(self) -> None:
```

### Comparing `uvicore-0.1.8/uvicore/configuration/commands/config.py` & `uvicore-0.1.9/uvicore/configuration/commands/config.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/configuration/configuration.py` & `uvicore-0.1.9/uvicore/configuration/configuration.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/configuration/services.py` & `uvicore-0.1.9/uvicore/configuration/services.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/console/__init__.py` & `uvicore-0.1.9/uvicore/console/__init__.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/console/click_colors.py` & `uvicore-0.1.9/uvicore/console/click_colors.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/console/console.py` & `uvicore-0.1.9/uvicore/console/console.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/console/decorators.py` & `uvicore-0.1.9/uvicore/console/decorators.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/console/handlers/bootstrap.py` & `uvicore-0.1.9/uvicore/console/handlers/bootstrap.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/console/provider.py` & `uvicore-0.1.9/uvicore/console/provider.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-from uvicore.support.dumper import dump, dd
-from uvicore.typing import Dict, List
-from uvicore.support.module import location
-from uvicore.database import Connection
+from uvicore.typing import Dict
 
 
 class Cli:
     """CLI Service Provider Mixin"""
 
     def commands(self, items: Dict[str, Dict] = None, *, group: str = None, help: str = None, commands: Dict = None):
         """Add commands as a dictionary or kwargs"""
```

### Comparing `uvicore-0.1.8/uvicore/console/services.py` & `uvicore-0.1.9/uvicore/console/services.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/container/commands/ioc.py` & `uvicore-0.1.9/uvicore/container/commands/ioc.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/container/ioc.py` & `uvicore-0.1.9/uvicore/container/ioc.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/contracts/__init__.py` & `uvicore-0.1.9/uvicore/contracts/__init__.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/contracts/application.py` & `uvicore-0.1.9/uvicore/contracts/application.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/contracts/authenticator.py` & `uvicore-0.1.9/uvicore/contracts/authenticator.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 from abc import ABC, abstractmethod
 from uvicore.contracts.user import User
-from uvicore.http.request import HTTPConnection
 from uvicore.typing import Optional, Tuple, Dict, List, Union
+try:
+    from starlette.requests import HTTPConnection
+except:
+    HTTPConnection = None
 
 
 class Authenticator(ABC):
 
     @abstractmethod
     async def authenticate(self, conn: HTTPConnection) -> Union[User, bool]:
         pass
```

### Comparing `uvicore-0.1.8/uvicore/contracts/builder.py` & `uvicore-0.1.9/uvicore/contracts/builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from typing import Any, Generic, List, Tuple, TypeVar, Union
 
-import sqlalchemy as sa
-from sqlalchemy.engine.result import RowProxy
-from sqlalchemy.sql.expression import BinaryExpression
+try:
+    import sqlalchemy as sa
+    from sqlalchemy.engine.result import RowProxy
+    from sqlalchemy.sql.expression import BinaryExpression
+except:
+    sa = None
+    RowProxy = None
+    BinaryExpression = None
 
 B = TypeVar("B")  # Builder Type (DbQueryBuilder or OrmQueryBuilder)
 E = TypeVar("E")  # Entity Model
 
 
 class QueryBuilder(Generic[B, E], ABC):
     @abstractmethod
```

### Comparing `uvicore-0.1.8/uvicore/contracts/cache.py` & `uvicore-0.1.9/uvicore/contracts/cache.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/contracts/config.py` & `uvicore-0.1.9/uvicore/contracts/config.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/contracts/connection.py` & `uvicore-0.1.9/uvicore/contracts/connection.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/contracts/database.py` & `uvicore-0.1.9/uvicore/contracts/database.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,24 @@
 from abc import ABC, abstractmethod
 from typing import Any, Dict, List, Union, Mapping, Optional
 
-import sqlalchemy as sa
-from databases import Database as EncodeDatabase
-from sqlalchemy.sql import ClauseElement
-from uvicore.contracts import DbQueryBuilder
+try:
+    from sqlalchemy.engine import Engine
+    from sqlalchemy import MetaData, Table
+    from databases import Database as EncodeDatabase
+    from sqlalchemy.sql import ClauseElement
+except:
+    sa = None
+    Engine = None
+    Table = None
+    MetaData = None
+    EncodeDatabase = None
+    ClauseElement = None
 
+from uvicore.contracts import DbQueryBuilder
 from .connection import Connection
 from .package import Package
 
 
 class Database(ABC):
     pass
 
@@ -23,27 +32,27 @@
     @abstractmethod
     def connections(self) -> Dict[str, Connection]:
         """All connections from all packages, keyed by connection str name"""
         pass
 
     @property
     @abstractmethod
-    def engines(self) -> Dict[str, sa.engine.Engine]:
+    def engines(self) -> Dict[str, Engine]:
         """All engines for all unique (by metakey) connections, keyed by metakey"""
         pass
 
     @property
     @abstractmethod
     def databases(self) -> Dict[str, EncodeDatabase]:
         """All Encode Databases for all unique (by metakey) connections, keyed by metakey"""
         pass
 
     @property
     @abstractmethod
-    def metadatas(self) -> Dict[str, sa.MetaData]:
+    def metadatas(self) -> Dict[str, MetaData]:
         """All SQLAlchemy Metadata for all unique (by metakey) connections, keyed by metakey"""
         pass
 
     @abstractmethod
     def init(self, default: str, connections: List[Connection]) -> None:
         """Initialize the database system with a default connection str and List of all Connections from all packages"""
         pass
@@ -60,30 +69,30 @@
 
     @abstractmethod
     def connection(self, connection: str = None) -> Connection:
         """Get one connection by connection name"""
         pass
 
     @abstractmethod
-    def metadata(self, connection: str = None, metakey: str = None) -> sa.MetaData:
+    def metadata(self, connection: str = None, metakey: str = None) -> MetaData:
         """Get one SQLAlchemy Metadata by connection str or metakey"""
         pass
 
     @abstractmethod
-    def table(self, table: str, connection: str = None) -> sa.Table:
+    def table(self, table: str, connection: str = None) -> Table:
         """Get one SQLAlchemy Table by name (without prefix) and connection str or connection.tablename dot notation"""
         pass
 
     @abstractmethod
     def tablename(self, table: str, connection: str = None) -> str:
         """Get a SQLAlchemy tablename with prefix by name (without prefix) and connection str or connection.tablename dot notation"""
         pass
 
     @abstractmethod
-    def engine(self, connection: str = None, metakey: str = None) -> sa.engine.Engine:
+    def engine(self, connection: str = None, metakey: str = None) -> Engine:
         """Get one SQLAlchemy Engine by connection str or metakey"""
         pass
 
     @abstractmethod
     async def database(self, connection: str = None, metakey: str = None) -> EncodeDatabase:
         """Get one Encode Database by connection str or metakey"""
         pass
```

### Comparing `uvicore-0.1.8/uvicore/contracts/dispatcher.py` & `uvicore-0.1.9/uvicore/contracts/dispatcher.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/contracts/event.py` & `uvicore-0.1.9/uvicore/contracts/event.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/contracts/field.py` & `uvicore-0.1.9/uvicore/contracts/field.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/contracts/ioc.py` & `uvicore-0.1.9/uvicore/contracts/ioc.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/contracts/logger.py` & `uvicore-0.1.9/uvicore/contracts/logger.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/contracts/model.py` & `uvicore-0.1.9/uvicore/contracts/model.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/contracts/package.py` & `uvicore-0.1.9/uvicore/contracts/package.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/contracts/provider.py` & `uvicore-0.1.9/uvicore/contracts/provider.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/contracts/relation.py` & `uvicore-0.1.9/uvicore/contracts/relation.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/contracts/router.py` & `uvicore-0.1.9/uvicore/contracts/router.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/contracts/routes-OLD.py` & `uvicore-0.1.9/uvicore/contracts/routes-OLD.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/contracts/template.py` & `uvicore-0.1.9/uvicore/contracts/template.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/contracts/user.py` & `uvicore-0.1.9/uvicore/contracts/user.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/contracts/user_provider.py` & `uvicore-0.1.9/uvicore/contracts/user_provider.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 from abc import ABC, abstractmethod
 from uvicore.typing import Union, List, Dict
 from uvicore.contracts.user import User
-from uvicore.http.request import HTTPConnection
+#from uvicore.contracts.http_connection import HTTPConnection
+try:
+    from starlette.requests import HTTPConnection
+except:
+    HTTPConnection = None
 
 
 class UserProvider(ABC):
 
     def __init__(self):
         # Default field mapping for each method below, easily overridable in your custom user providers!
         self.field_map = {
@@ -49,10 +53,7 @@
     # @abstractmethod
     # async def retrieve_by_username(self, username: str, request: HTTPConnection, options: Dict = {}) -> User:
     #     """Retrieve the user by username from the user provider backend.  No validation."""
 
     # @abstractmethod
     # async def retrieve_by_credentials(self, username: str, password: str, request: HTTPConnection, options: Dict = {}) -> User:
     #     """Retrieve the user by username from the user provider backend AND validate the password if not None"""
-
-
-
```

### Comparing `uvicore-0.1.8/uvicore/database/OBSOLETE/OLD-__init__.py` & `uvicore-0.1.9/uvicore/database/OBSOLETE/OLD-__init__.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/database/OBSOLETE/db_OLD.py` & `uvicore-0.1.9/uvicore/database/OBSOLETE/db_OLD.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/database/OBSOLETE/db_OLD2.py` & `uvicore-0.1.9/uvicore/database/OBSOLETE/db_OLD2.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/database/OBSOLETE/db_OLD_sync.py` & `uvicore-0.1.9/uvicore/database/OBSOLETE/db_OLD_sync.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/database/OBSOLETE/idea__init__.py` & `uvicore-0.1.9/uvicore/database/OBSOLETE/idea__init__.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/database/__init__.py` & `uvicore-0.1.9/uvicore/database/__init__.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/database/builder.py` & `uvicore-0.1.9/uvicore/database/builder.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/database/commands/db.py` & `uvicore-0.1.9/uvicore/database/commands/db.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/database/commands/generators.py` & `uvicore-0.1.9/uvicore/database/commands/generators.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/database/commands/stubs/seeder.py` & `uvicore-0.1.9/uvicore/database/commands/stubs/seeder.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/database/commands/stubs/table.py` & `uvicore-0.1.9/uvicore/database/commands/stubs/table.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/database/db.py` & `uvicore-0.1.9/uvicore/database/db.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/database/handlers/bootstrap.py` & `uvicore-0.1.9/uvicore/database/handlers/bootstrap.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/database/provider.py` & `uvicore-0.1.9/uvicore/database/provider.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/database/query.py` & `uvicore-0.1.9/uvicore/database/query.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/database/services.py` & `uvicore-0.1.9/uvicore/database/services.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/database/table.py` & `uvicore-0.1.9/uvicore/database/table.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/events/commands/event.py` & `uvicore-0.1.9/uvicore/events/commands/event.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/events/dispatcher.py` & `uvicore-0.1.9/uvicore/events/dispatcher.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/events/event.py` & `uvicore-0.1.9/uvicore/events/event.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/foundation/application.py` & `uvicore-0.1.9/uvicore/foundation/application.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from uvicore.typing import Any, List, NamedTuple, Tuple, Dict, OrderedDict
 from uvicore.package import Package
 from uvicore.contracts import Application as ApplicationInterface
 from uvicore.contracts import Config as ConfigInterface
 from uvicore.contracts import Package as PackageInterface
 from uvicore.contracts import Server as ServerInterface
 from uvicore.contracts import Template as TemplateInterface
-from uvicore.database import Connection
 from uvicore.support.collection import dotget
 from uvicore.support.dumper import dd, dump
 from uvicore.support.hash import md5
 from uvicore.support.module import load, location
 from uvicore.console import command_is
 
 #import uvicore.foundation.events.app
```

### Comparing `uvicore-0.1.8/uvicore/foundation/config/package.py` & `uvicore-0.1.9/uvicore/foundation/config/package.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/foundation/decorators/model.py` & `uvicore-0.1.9/uvicore/foundation/decorators/model.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/foundation/decorators/service.py` & `uvicore-0.1.9/uvicore/foundation/decorators/service.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/foundation/events/app.py` & `uvicore-0.1.9/uvicore/foundation/events/app.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/foundation/services.py` & `uvicore-0.1.9/uvicore/foundation/services.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/http/OBSOLETE/router.py` & `uvicore-0.1.9/uvicore/http/OBSOLETE/router.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/http/OBSOLETE/routes-OLD.py` & `uvicore-0.1.9/uvicore/http/OBSOLETE/routes-OLD.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/http/__init__.py` & `uvicore-0.1.9/uvicore/http/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from .request import Body, Form, Path, Query, Request
 from starlette.background import BackgroundTask, BackgroundTasks
 
+
 # No, causes to much to be imported just by importing anything from uvicore.http
 # from .routing import (ApiRoute, ApiRouter, Controller, ModelRouter, Router,
 #                       Routes, WebRoute, WebRouter)
 
 
 # NO - not used by user
 #from .server import Server
```

### Comparing `uvicore-0.1.8/uvicore/http/bootstrap.py` & `uvicore-0.1.9/uvicore/http/bootstrap.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/http/commands/serve.py` & `uvicore-0.1.9/uvicore/http/commands/serve.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/http/controllers/api.py` & `uvicore-0.1.9/uvicore/http/controllers/api.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/http/controllers/web.py` & `uvicore-0.1.9/uvicore/http/controllers/web.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/http/events/server.py` & `uvicore-0.1.9/uvicore/http/events/server.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/http/exceptions.py` & `uvicore-0.1.9/uvicore/http/exceptions.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/http/middleware/__init__.py` & `uvicore-0.1.9/uvicore/http/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/http/middleware/authentication.py` & `uvicore-0.1.9/uvicore/http/middleware/authentication.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/http/provider.py` & `uvicore-0.1.9/uvicore/http/provider.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/http/response.py` & `uvicore-0.1.9/uvicore/http/response.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/http/routing/api_router.py` & `uvicore-0.1.9/uvicore/http/routing/api_router.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/http/routing/guard.py` & `uvicore-0.1.9/uvicore/http/routing/guard.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/http/routing/model_router.py` & `uvicore-0.1.9/uvicore/http/routing/model_router.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/http/routing/router.py` & `uvicore-0.1.9/uvicore/http/routing/router.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/http/routing/web_router.py` & `uvicore-0.1.9/uvicore/http/routing/web_router.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/http/server.py` & `uvicore-0.1.9/uvicore/http/server.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/http/servers/api.py` & `uvicore-0.1.9/uvicore/http/servers/api.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/http/services.py` & `uvicore-0.1.9/uvicore/http/services.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/http/static.py` & `uvicore-0.1.9/uvicore/http/static.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/http/status.py` & `uvicore-0.1.9/uvicore/http/status.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/http/templating/context_functions.py` & `uvicore-0.1.9/uvicore/http/templating/context_functions.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/http/templating/jinja.py` & `uvicore-0.1.9/uvicore/http/templating/jinja.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/logging/logger.py` & `uvicore-0.1.9/uvicore/logging/logger.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/logging/services.py` & `uvicore-0.1.9/uvicore/logging/services.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/orm/commands/generators.py` & `uvicore-0.1.9/uvicore/orm/commands/generators.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/orm/commands/stubs/model.py` & `uvicore-0.1.9/uvicore/orm/commands/stubs/model.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/orm/fields.py` & `uvicore-0.1.9/uvicore/orm/fields.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/orm/mapper.py` & `uvicore-0.1.9/uvicore/orm/mapper.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/orm/metaclass.py` & `uvicore-0.1.9/uvicore/orm/metaclass.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/orm/model.py` & `uvicore-0.1.9/uvicore/orm/model.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/orm/query.py` & `uvicore-0.1.9/uvicore/orm/query.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/orm/services.py` & `uvicore-0.1.9/uvicore/orm/services.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/package/commands/package.py` & `uvicore-0.1.9/uvicore/package/commands/package.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/package/package.py` & `uvicore-0.1.9/uvicore/package/package.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/package/provider.py` & `uvicore-0.1.9/uvicore/package/provider.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/redis/bootstrap.py` & `uvicore-0.1.9/uvicore/redis/bootstrap.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/redis/redis.py` & `uvicore-0.1.9/uvicore/redis/redis.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/redis/services.py` & `uvicore-0.1.9/uvicore/redis/services.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/support/collection.py` & `uvicore-0.1.9/uvicore/support/collection.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/support/dictionary.py` & `uvicore-0.1.9/uvicore/support/dictionary.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/support/dumper.py` & `uvicore-0.1.9/uvicore/support/dumper.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/support/module.py` & `uvicore-0.1.9/uvicore/support/module.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/support/path.py` & `uvicore-0.1.9/uvicore/support/path.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/support/schematic.py` & `uvicore-0.1.9/uvicore/support/schematic.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/support/singleton.py` & `uvicore-0.1.9/uvicore/support/singleton.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/support/str.py` & `uvicore-0.1.9/uvicore/support/str.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/uvicore/typing/__init__.py` & `uvicore-0.1.9/uvicore/typing/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 from typing import *
-from starlette.types import Scope, Message, Receive, Send, ASGIApp
 from .dictionary import Dict, OrderedDict
+try:
+    from starlette.types import Scope, Message, Receive, Send, ASGIApp
+except:
+    Scope = None
+    Message = None
+    Receive = None
+    Send = None
+    ASGIApp = None
 
 # Decorator Type Helper
 # def handle() -> Callable[[Decorator], Decorator]:
 #     def decorator(func: Decorator) -> Decorator
 #         return func
 #     return decorator
 Decorator = TypeVar("Decorator", bound=Callable[..., Any])
```

### Comparing `uvicore-0.1.8/uvicore/typing/dictionary.py` & `uvicore-0.1.9/uvicore/typing/dictionary.py`

 * *Files identical despite different names*

### Comparing `uvicore-0.1.8/setup.py` & `uvicore-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
  'uvicore.auth.database.tables',
  'uvicore.auth.middleware',
  'uvicore.auth.models',
  'uvicore.auth.support',
  'uvicore.auth.user_providers',
  'uvicore.cache',
  'uvicore.cache.backends',
- 'uvicore.cache.handlers',
  'uvicore.configuration',
  'uvicore.configuration.commands',
  'uvicore.console',
  'uvicore.console.commands',
  'uvicore.console.commands.stubs',
  'uvicore.console.handlers',
  'uvicore.container',
@@ -68,30 +67,30 @@
  'cryptography>=3.4.0,<3.5.0',
  'environs>=9.3.0,<9.4.0',
  'prettyprinter>=0.18.0,<0.19.0']
 
 extras_require = \
 {'database': ['sqlalchemy>=1.3.0,<1.4.0',
               'alembic>=1.5.0,<1.6.0',
-              'databases[postgres,sqlite,mysql]>=0.4.0,<0.5.0'],
+              'databases[sqlite,postgres,mysql]>=0.4.0,<0.5.0'],
  'web': ['fastapi>=0.63.0,<0.64.0',
          'uvicorn>=0.13.0,<0.14.0',
          'gunicorn>=20.0.0,<20.1.0',
          'aiofiles>=0.6.0,<0.7.0',
          'Jinja2>=2.11.0,<2.12.0',
          'requests>=2.25.0,<2.26.0',
          'itsdangerous>=1.1.0,<1.2.0',
          'uvloop>=0.14.0,<0.15.0',
          'httptools>=0.1.0,<0.2.0',
          'python-multipart>=0.0.0,<0.1.0',
          'PyJWT>=2.0.0,<2.1.0']}
 
 setup_kwargs = {
     'name': 'uvicore',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'The Async Python Framework for Artisans. An Elegant Fullstack Python Web, API and CLI Framework',
     'long_description': "# Uvicore\n\n**The Async Python Framework for Artisans. An Elegant Fullstack Python Web, API and CLI Framework**\n\n\nThis is a full stack python framework with everything included.  Built on other micro frameworks such as Starlette and FastAPI but resembling neither.  Uvicore feels like no other python framework you have ever used.  Think Laravel instead of Django or Flask.\n\nMore to come later.\n\nUnder heavy development.  Do NOT use this repository yet.\n\n\n## Features\n\n* Super fast, built on Starlette, FastAPI (but feels like neither) and other libraries.\n* Equally well suited for complete CLI apps, Rest APIs with OpenAPI Docs and Traditional web applications.\n* Fully asynchronous including CLI apps for unix socket programming and of course Websockets.\n* Automatic API generation from all ORM models without a single line of View or Controller code.\n* Full OpenAPI 3 automatically generated docs.\n* All apps are packages and all packages are apps.  A modular framework with app override capability for configs, templates, assets, routes, models and more.  Reuse your app inside other apps as libraries for a Python native micro service architecture.  Or use the automatically generated API from ORM models for a Rest based micro service architecture with no extra work.\n* Custom IoC (Inversion of Control) system to swap any concrete implementation without changing imports.\n* Asynchronous database layer for MySQL, SQLite and Postgres.\n* All new custom asynchronous ORM (NOT another django ORM clone) with support for every relationship including polymorphism.  Enjoy Laravel's Eloquent ORM?  You'll love this one.\n* Full python type hinting for IDE code intellisense across every module including ORM model fields and methods.\n\n\n\n## ToDo\n\n* Write complete ORM tests with 100% coverage\n* Need better ORM where AND with OR mixed around.  Currently it only does all ANDs then all WHEREs which won't work for complex queries.  For example grouping 2 where ANDs with an OR like so\n\n```sql\nSELECT DISTINCT posts.id, posts.unique_slug, posts.title, posts.other, posts.creator_id, posts.owner_id, attributes.*\nFROM posts LEFT OUTER JOIN attributes ON attributes.attributable_type = 'posts' AND posts.id = attributes.attributable_id\nWHERE\n(attributes.key = 'post1-test1' and attributes.value = 'value for post1-test1')\nor\n(attributes.key = 'post2-test1' and attributes.value = 'value for post2-test1')\n```\n\n* Cannot update attributes from a parent (post.add('attributes'))...IntegrityError.  See posts seeder for notes.\n",
     'author': 'Matthew Reschke',
     'author_email': 'mail@mreschke.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/uvicore/framework',
```

### Comparing `uvicore-0.1.8/PKG-INFO` & `uvicore-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uvicore
-Version: 0.1.8
+Version: 0.1.9
 Summary: The Async Python Framework for Artisans. An Elegant Fullstack Python Web, API and CLI Framework
 Home-page: https://github.com/uvicore/framework
 License: MIT
 Author: Matthew Reschke
 Author-email: mail@mreschke.com
 Requires-Python: >=3.7,<4.0
 Classifier: Environment :: Web Environment
@@ -29,15 +29,15 @@
 Requires-Dist: aiofiles (>=0.6.0,<0.7.0); extra == "web"
 Requires-Dist: aioredis (>=1.3.0,<1.4.0)
 Requires-Dist: alembic (>=1.5.0,<1.6.0); extra == "database"
 Requires-Dist: argon2-cffi (>=20.1.0,<20.2.0)
 Requires-Dist: asyncclick (>=7.1.0,<7.2.0)
 Requires-Dist: colored (>=1.4.0,<1.5.0)
 Requires-Dist: cryptography (>=3.4.0,<3.5.0)
-Requires-Dist: databases[postgres,sqlite,mysql] (>=0.4.0,<0.5.0); extra == "database"
+Requires-Dist: databases[sqlite,postgres,mysql] (>=0.4.0,<0.5.0); extra == "database"
 Requires-Dist: environs (>=9.3.0,<9.4.0)
 Requires-Dist: fastapi (>=0.63.0,<0.64.0); extra == "web"
 Requires-Dist: gunicorn (>=20.0.0,<20.1.0); extra == "web"
 Requires-Dist: httptools (>=0.1.0,<0.2.0); extra == "web"
 Requires-Dist: itsdangerous (>=1.1.0,<1.2.0); extra == "web"
 Requires-Dist: prettyprinter (>=0.18.0,<0.19.0)
 Requires-Dist: python-multipart (>=0.0.0,<0.1.0); extra == "web"
```

