# Comparing `tmp/fastapi_all_out-0.2.1.tar.gz` & `tmp/fastapi_all_out-0.2.2.tar.gz`

## Comparing `fastapi_all_out-0.2.1.tar` & `fastapi_all_out-0.2.2.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/__init__.py
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/app.py
--rw-r--r--   0        0        0     5047 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/code_responses.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/enums.py
--rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/lazy.py
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/mailing.py
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/models.py
--rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/responses.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/schemas.py
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/auth/__init__.py
--rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/auth/base.py
--rw-r--r--   0        0        0     5512 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/auth/router.py
--rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/auth/schemas.py
--rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/auth/user_service.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/auth/jwt/__init__.py
--rw-r--r--   0        0        0     6716 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/auth/jwt/backend.py
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/auth/jwt/schemas.py
--rw-r--r--   0        0        0     4278 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/auth/jwt/strategy.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/auth/roles/__init__.py
--rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/auth/roles/router.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/auth/roles/schemas.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/contrib/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/contrib/tortoise/__init__.py
--rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/contrib/tortoise/conntection.py
--rw-r--r--   0        0        0    32984 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/contrib/tortoise/repository.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/contrib/tortoise/repository_meta.py
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/contrib/tortoise/user_repository.py
--rw-r--r--   0        0        0     3271 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/contrib/tortoise/user_service.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/contrib/tortoise/fields/__init__.py
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/contrib/tortoise/fields/name_enum_field.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/contrib/tortoise/filters/__init__.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/contrib/tortoise/filters/fk.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/contrib/tortoise/filters/int.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/contrib/tortoise/filters/simple.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/contrib/tortoise/filters/str.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/contrib/tortoise/models/__init__.py
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/contrib/tortoise/models/base.py
--rw-r--r--   0        0        0     3050 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/contrib/tortoise/models/base_user.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/contrib/tortoise/models/content_type.py
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/contrib/tortoise/models/permissions.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/management/__init__.py
--rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/management/command.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/pydantic/__init__.py
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/pydantic/camel_model.py
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/pydantic/comma_separated.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/pydantic/fields/__init__.py
--rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/pydantic/fields/field_in_related_model.py
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/pydantic/fields/password.py
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/pydantic/fields/phonenumber.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/pydantic/fields/related_list.py
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/pydantic/fields/username.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/routers/__init__.py
--rw-r--r--   0        0        0     5101 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/routers/base_repository.py
--rw-r--r--   0        0        0    20297 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/routers/crud_router.py
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/routers/exceptions.py
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/routers/utils.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/routers/filters/__init__.py
--rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/routers/filters/base.py
--rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/routers/filters/bool.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/routers/filters/fk.py
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/routers/filters/int.py
--rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/routers/filters/int_btw.py
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/routers/filters/str.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/templates/activation.html
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/fastapi_all_out/templates/password_reset.html
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/LICENSE.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/README.md
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/__init__.py
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/app.py
+-rw-r--r--   0        0        0     5047 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/code_responses.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/enums.py
+-rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/lazy.py
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/mailing.py
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/models.py
+-rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/responses.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/schemas.py
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/auth/__init__.py
+-rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/auth/base.py
+-rw-r--r--   0        0        0     5512 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/auth/router.py
+-rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/auth/schemas.py
+-rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/auth/user_service.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/auth/jwt/__init__.py
+-rw-r--r--   0        0        0     6716 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/auth/jwt/backend.py
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/auth/jwt/schemas.py
+-rw-r--r--   0        0        0     4278 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/auth/jwt/strategy.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/auth/roles/__init__.py
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/auth/roles/router.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/auth/roles/schemas.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/contrib/tortoise/__init__.py
+-rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/contrib/tortoise/conntection.py
+-rw-r--r--   0        0        0    33336 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/contrib/tortoise/repository.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/contrib/tortoise/repository_meta.py
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/contrib/tortoise/user_repository.py
+-rw-r--r--   0        0        0     3271 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/contrib/tortoise/user_service.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/contrib/tortoise/fields/__init__.py
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/contrib/tortoise/fields/name_enum_field.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/contrib/tortoise/filters/__init__.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/contrib/tortoise/filters/fk.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/contrib/tortoise/filters/int.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/contrib/tortoise/filters/simple.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/contrib/tortoise/filters/str.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/contrib/tortoise/models/__init__.py
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/contrib/tortoise/models/base.py
+-rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/contrib/tortoise/models/base_user.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/contrib/tortoise/models/content_type.py
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/contrib/tortoise/models/permissions.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/management/__init__.py
+-rw-r--r--   0        0        0     1182 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/management/command.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/pydantic/__init__.py
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/pydantic/camel_model.py
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/pydantic/comma_separated.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/pydantic/fields/__init__.py
+-rw-r--r--   0        0        0     2207 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/pydantic/fields/field_in_related_model.py
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/pydantic/fields/password.py
+-rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/pydantic/fields/phonenumber.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/pydantic/fields/related_list.py
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/pydantic/fields/username.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/routers/__init__.py
+-rw-r--r--   0        0        0     5101 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/routers/base_repository.py
+-rw-r--r--   0        0        0    20297 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/routers/crud_router.py
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/routers/exceptions.py
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/routers/utils.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/routers/filters/__init__.py
+-rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/routers/filters/base.py
+-rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/routers/filters/bool.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/routers/filters/fk.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/routers/filters/int.py
+-rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/routers/filters/int_btw.py
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/routers/filters/str.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/templates/activation.html
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/fastapi_all_out/templates/password_reset.html
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/LICENSE.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/README.md
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 fastapi_all_out-0.2.2/PKG-INFO
```

### Comparing `fastapi_all_out-0.2.1/fastapi_all_out/app.py` & `fastapi_all_out-0.2.2/fastapi_all_out/app.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.1/fastapi_all_out/code_responses.py` & `fastapi_all_out-0.2.2/fastapi_all_out/code_responses.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.1/fastapi_all_out/lazy.py` & `fastapi_all_out-0.2.2/fastapi_all_out/lazy.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.1/fastapi_all_out/mailing.py` & `fastapi_all_out-0.2.2/fastapi_all_out/mailing.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.1/fastapi_all_out/models.py` & `fastapi_all_out-0.2.2/fastapi_all_out/models.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.1/fastapi_all_out/responses.py` & `fastapi_all_out-0.2.2/fastapi_all_out/responses.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.1/fastapi_all_out/settings.py` & `fastapi_all_out-0.2.2/fastapi_all_out/settings.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.1/fastapi_all_out/auth/base.py` & `fastapi_all_out-0.2.2/fastapi_all_out/auth/base.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.1/fastapi_all_out/auth/router.py` & `fastapi_all_out-0.2.2/fastapi_all_out/auth/router.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.1/fastapi_all_out/auth/schemas.py` & `fastapi_all_out-0.2.2/fastapi_all_out/auth/schemas.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.1/fastapi_all_out/auth/user_service.py` & `fastapi_all_out-0.2.2/fastapi_all_out/auth/user_service.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.1/fastapi_all_out/auth/jwt/backend.py` & `fastapi_all_out-0.2.2/fastapi_all_out/auth/jwt/backend.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.1/fastapi_all_out/auth/jwt/schemas.py` & `fastapi_all_out-0.2.2/fastapi_all_out/auth/jwt/schemas.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.1/fastapi_all_out/auth/jwt/strategy.py` & `fastapi_all_out-0.2.2/fastapi_all_out/auth/jwt/strategy.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.1/fastapi_all_out/auth/roles/router.py` & `fastapi_all_out-0.2.2/fastapi_all_out/auth/roles/router.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.1/fastapi_all_out/auth/roles/schemas.py` & `fastapi_all_out-0.2.2/fastapi_all_out/auth/roles/schemas.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.1/fastapi_all_out/contrib/tortoise/conntection.py` & `fastapi_all_out-0.2.2/fastapi_all_out/contrib/tortoise/conntection.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.1/fastapi_all_out/contrib/tortoise/repository.py` & `fastapi_all_out-0.2.2/fastapi_all_out/contrib/tortoise/repository.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 
 from tortoise.models import MetaInfo
 from tortoise.fields import ManyToManyRelation, Field, DateField, DatetimeField, TimeField
 from tortoise.queryset import QuerySet
 from tortoise.transactions import in_transaction
 
 from fastapi_all_out.routers.base_repository import BaseRepository, PK, ModelPrefix, Updated
-from fastapi_all_out.routers.exceptions import ItemNotFound, ObjectErrors, NotUnique, ListFieldError, NotFoundFK, \
-    FieldRequired
+from fastapi_all_out.routers.exceptions import ItemNotFound, ObjectErrors, FieldError, NotUnique, ListFieldError,\
+    NotFoundFK, FieldRequired
 from .repository_meta import TortoiseRepositoryMeta
 from .models import BaseModel
 
 if TYPE_CHECKING:
     from fastapi_all_out.routers.filters import BaseFilter
 
 
@@ -114,22 +114,25 @@
         model: Type[DB_MODEL] = model or self.model
         fk_fields, bfk_fields, o2o_fields, bo2o_fields, m2m_fields = exclude_fk_bfk_o2o_bo2o_m2m(model, data)
         exclude_dict = get_exclude_dict(exclude or set())
         errors = ObjectErrors()
         defaults = defaults or {}
 
         async def get_new_instance() -> DB_MODEL:
-            await self.clean_data(
-                model=model, data=data, prefix=prefix, create=True,
-                fk_fields=fk_fields,
-                bfk_fields=bfk_fields,
-                o2o_fields=o2o_fields,
-                bo2o_fields=bo2o_fields,
-                m2m_fields=m2m_fields,
-            )
+            try:
+                await self.clean_data(
+                    model=model, data=data, prefix=prefix, create=True,
+                    fk_fields=fk_fields,
+                    bfk_fields=bfk_fields,
+                    o2o_fields=o2o_fields,
+                    bo2o_fields=bo2o_fields,
+                    m2m_fields=m2m_fields,
+                )
+            except ObjectErrors as e:
+                raise errors.merge(e)
             try:
                 await self.check_unique(data=data, model=model, prefix=prefix)
             except ObjectErrors as e:
                 errors.merge(e)
 
             # Сначала создаём o2o и fk, потому что они могут быть not null, из-за этого вылетает ошибка.
             created_o2o, picked_fks = {}, {}
@@ -691,14 +694,15 @@
             o2o_fields: set[str],
             bo2o_fields: set[str],
             m2m_fields: set[str],
             instance: Optional[DB_MODEL] = None,
             create: bool = True,
     ) -> dict[str, Any]:
         related_fields = {*model._meta.db_fields, *fk_fields, *bfk_fields, *o2o_fields, *bo2o_fields, *m2m_fields}
+        errors = ObjectErrors()
         for field_name in related_fields:
             if field_name not in data:
                 continue
             func_name = f'clean_field_{prefix.plus(field_name)}'
             if hasattr(self, func_name):
                 func = getattr(self, func_name)
             elif field_name in fk_fields:
@@ -709,25 +713,30 @@
                 func = self._clean_o2o_field_default
             elif field_name in bo2o_fields:
                 func = self._clean_bo2o_field_default
             elif field_name in m2m_fields:
                 func = self._clean_m2m_field_default
             else:
                 func = self._clean_field_default
-            should_remove = await func(
-                model=model, data=data, field_name=field_name, instance=instance, create=create
-            )
-            if should_remove:
-                for set_ in (fk_fields, bfk_fields, o2o_fields, bo2o_fields, m2m_fields):
-                    if field_name in set_:
-                        set_.remove(field_name)
-                try:
-                    del data[field_name]
-                except KeyError:
-                    pass
+            try:
+                if await func(
+                        model=model, data=data,
+                        field_name=field_name, instance=instance, create=create
+                ):
+                    for set_ in (fk_fields, bfk_fields, o2o_fields, bo2o_fields, m2m_fields):
+                        if field_name in set_:
+                            set_.remove(field_name)
+                    try:
+                        del data[field_name]
+                    except KeyError:
+                        pass
+            except FieldError as e:
+                errors.add(field_name, e)
+        if errors:
+            raise errors
         return data
 
     async def _clean_field_default(
             self, model: Type[DB_MODEL], data: dict[str, Any], field_name: str,
             instance: Optional[DB_MODEL], create: bool
     ) -> bool:
         if create:
@@ -781,28 +790,28 @@
 
     async def check_unique(self, data: dict[str, Any], model: Type[DB_MODEL], prefix: ModelPrefix) -> None:
         errors = ObjectErrors()
         for field_name in model._meta.db_fields:
             field = model._meta.fields_map[field_name]
             if not field.unique or field.generated:
                 continue
-            if value := data.get(field_name) is not None:
+            if (value := data.get(field_name)) is not None:
                 if hasattr(self, f'check_unique_{prefix.plus(field_name)}'):
                     check_unique_func = getattr(self, f'check_unique_{prefix.plus(field_name)}')
                 else:
                     check_unique_func = self._check_unique_default
-                if await check_unique_func(model=model, field_name=field_name, value=value):
+                if not await check_unique_func(model=model, field_name=field_name, value=value):
                     errors.add(field_name, NotUnique)
         if errors:
             raise errors
 
     async def _check_unique_default(self, model: Type[DB_MODEL], field_name: str, value: Any) -> bool:
         if field_name in model.IEXACT_FIELDS:
             field_name = field_name + '__iexact'
-        return await model.filter(**{field_name: value}).exists()
+        return not await model.filter(**{field_name: value}).exists()
 
     @classmethod
     def _get_bfk_model(cls, model: Type[BaseModel], field_name: str) -> Type[BaseModel]:
         return model._meta.fields_map[field_name].related_model
 
     @classmethod
     def _get_pk_attr(cls, model: Type[BaseModel]) -> str:
```

### Comparing `fastapi_all_out-0.2.1/fastapi_all_out/contrib/tortoise/user_repository.py` & `fastapi_all_out-0.2.2/fastapi_all_out/contrib/tortoise/user_repository.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.1/fastapi_all_out/contrib/tortoise/user_service.py` & `fastapi_all_out-0.2.2/fastapi_all_out/contrib/tortoise/user_service.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.1/fastapi_all_out/contrib/tortoise/fields/name_enum_field.py` & `fastapi_all_out-0.2.2/fastapi_all_out/contrib/tortoise/fields/name_enum_field.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.1/fastapi_all_out/contrib/tortoise/filters/simple.py` & `fastapi_all_out-0.2.2/fastapi_all_out/contrib/tortoise/filters/simple.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.1/fastapi_all_out/contrib/tortoise/filters/str.py` & `fastapi_all_out-0.2.2/fastapi_all_out/contrib/tortoise/filters/str.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.1/fastapi_all_out/contrib/tortoise/models/base.py` & `fastapi_all_out-0.2.2/fastapi_all_out/contrib/tortoise/models/base.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.1/fastapi_all_out/contrib/tortoise/models/base_user.py` & `fastapi_all_out-0.2.2/fastapi_all_out/contrib/tortoise/models/base_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from datetime import datetime, timedelta
 from uuid import UUID, uuid4
 
 from tortoise import fields, timezone
 
 from fastapi_all_out.lazy import get_user_model_path
 from fastapi_all_out.enums import TempCodeTriggers
-from . import BaseModel, PermissionMixin, max_len_of, ContentType
+from . import BaseModel, PermissionMixin, max_len_of
 
 
 USER_GET_BY_FIELDS = Literal['id', 'email', 'username', 'phone']
 
 
 class BaseUser(BaseModel):
     id: int
```

### Comparing `fastapi_all_out-0.2.1/fastapi_all_out/contrib/tortoise/models/content_type.py` & `fastapi_all_out-0.2.2/fastapi_all_out/contrib/tortoise/models/content_type.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.1/fastapi_all_out/contrib/tortoise/models/permissions.py` & `fastapi_all_out-0.2.2/fastapi_all_out/contrib/tortoise/models/permissions.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.1/fastapi_all_out/management/command.py` & `fastapi_all_out-0.2.2/fastapi_all_out/management/command.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.1/fastapi_all_out/pydantic/camel_model.py` & `fastapi_all_out-0.2.2/fastapi_all_out/pydantic/camel_model.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.1/fastapi_all_out/pydantic/comma_separated.py` & `fastapi_all_out-0.2.2/fastapi_all_out/pydantic/comma_separated.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.1/fastapi_all_out/pydantic/fields/field_in_related_model.py` & `fastapi_all_out-0.2.2/fastapi_all_out/pydantic/fields/field_in_related_model.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.1/fastapi_all_out/pydantic/fields/password.py` & `fastapi_all_out-0.2.2/fastapi_all_out/pydantic/fields/password.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.1/fastapi_all_out/pydantic/fields/phonenumber.py` & `fastapi_all_out-0.2.2/fastapi_all_out/pydantic/fields/phonenumber.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.1/fastapi_all_out/pydantic/fields/related_list.py` & `fastapi_all_out-0.2.2/fastapi_all_out/pydantic/fields/related_list.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.1/fastapi_all_out/pydantic/fields/username.py` & `fastapi_all_out-0.2.2/fastapi_all_out/pydantic/fields/username.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 from typing import Any
 
 from pydantic.validators import strict_str_validator
 
 
 class Username(str):
 
+    min_len = 4
+    max_len = 40
     pattern = re.compile(r'^(?=.*[a-zA-Z])[\w+.-]+$')
 
     @classmethod
     def __modify_schema__(cls, field_schema: dict[str, Any]) -> None:
         field_schema.update(type='string', format='username', example='sasha_molodez')
 
     @classmethod
@@ -17,8 +19,12 @@
         yield strict_str_validator
         yield cls.validate
 
     @classmethod
     def validate(cls, v: str):
         if cls.pattern.match(v) is None:
             raise ValueError('Username is invalid')
+        if getattr(cls, 'max_len', None) and len(v) > cls.max_len:
+            raise ValueError('Username is too long')
+        if getattr(cls, 'min_len', None) and len(v) < cls.min_len:
+            raise ValueError('Username is too short')
         return cls(v)
```

### Comparing `fastapi_all_out-0.2.1/fastapi_all_out/routers/base_repository.py` & `fastapi_all_out-0.2.2/fastapi_all_out/routers/base_repository.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.1/fastapi_all_out/routers/crud_router.py` & `fastapi_all_out-0.2.2/fastapi_all_out/routers/crud_router.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.1/fastapi_all_out/routers/exceptions.py` & `fastapi_all_out-0.2.2/fastapi_all_out/routers/exceptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,14 +21,18 @@
     key = 'notFoundFK'
 
 
 class FieldRequired(FieldError):
     key = 'requiredField'
 
 
+class MaximumFiveEmails(FieldError):
+    key = 'maximumFiveEmails'
+
+
 class ListFieldError(FieldError):
     objects_map: dict[int, Union["ObjectErrors", "FieldError"]]
 
     def __init__(self,  *args):
         super().__init__(*args)
         self.objects_map = {}
```

### Comparing `fastapi_all_out-0.2.1/fastapi_all_out/routers/utils.py` & `fastapi_all_out-0.2.2/fastapi_all_out/routers/utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.1/fastapi_all_out/routers/filters/base.py` & `fastapi_all_out-0.2.2/fastapi_all_out/routers/filters/base.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.1/fastapi_all_out/routers/filters/bool.py` & `fastapi_all_out-0.2.2/fastapi_all_out/routers/filters/bool.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.1/fastapi_all_out/routers/filters/int.py` & `fastapi_all_out-0.2.2/fastapi_all_out/routers/filters/int.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.1/fastapi_all_out/routers/filters/int_btw.py` & `fastapi_all_out-0.2.2/fastapi_all_out/routers/filters/int_btw.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.1/fastapi_all_out/routers/filters/str.py` & `fastapi_all_out-0.2.2/fastapi_all_out/routers/filters/str.py`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.1/fastapi_all_out/templates/activation.html` & `fastapi_all_out-0.2.2/fastapi_all_out/templates/activation.html`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.1/fastapi_all_out/templates/password_reset.html` & `fastapi_all_out-0.2.2/fastapi_all_out/templates/password_reset.html`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.1/LICENSE.md` & `fastapi_all_out-0.2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fastapi_all_out-0.2.1/pyproject.toml` & `fastapi_all_out-0.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.hatch.build]
 ignore-vcs = true
 include = ["fastapi_all_out"]
 
 [project]
 name = "fastapi-all-out"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
   { name="Alexandr Tamrazov", email="alta77@mail.ru" },
 ]
 maintainers = [
   { name="Alexandr Tamrazov", email="alta77@mail.ru" },
 ]
 keywords = ["DDD", "Domain-driven design", "Database", "WEB", "Architecture", "Backend"]
```

### Comparing `fastapi_all_out-0.2.1/PKG-INFO` & `fastapi_all_out-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-all-out
-Version: 0.2.1
+Version: 0.2.2
 Summary: Makes fastapi much easier and stronger, then Django
 Project-URL: Github, https://github.com/alta7700/fastapi_all_out/
 Author-email: Alexandr Tamrazov <alta77@mail.ru>
 Maintainer-email: Alexandr Tamrazov <alta77@mail.ru>
 License: Copyright © 2023 Alexandr Tamrazov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
```

