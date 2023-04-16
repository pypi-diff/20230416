# Comparing `tmp/mimesis-7.1.0.tar.gz` & `tmp/mimesis-8.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mimesis-7.1.0.tar", max compression
+gzip compressed data, was "mimesis-8.0.0.tar", max compression
```

## Comparing `mimesis-7.1.0.tar` & `mimesis-8.0.0.tar`

### file list

```diff
@@ -1,286 +1,286 @@
--rw-r--r--   0        0        0     1123 2023-04-06 21:11:08.800162 mimesis-7.1.0/LICENSE
--rw-r--r--   0        0        0     6945 2023-04-06 21:11:08.800162 mimesis-7.1.0/README.rst
--rw-r--r--   0        0        0     2286 2023-04-06 21:11:08.804162 mimesis-7.1.0/mimesis/__init__.py
--rw-r--r--   0        0        0      552 2023-04-06 21:11:08.804162 mimesis-7.1.0/mimesis/builtins/__init__.py
--rw-r--r--   0        0        0      428 2023-04-06 21:11:08.804162 mimesis-7.1.0/mimesis/builtins/base.py
--rw-r--r--   0        0        0     3671 2023-04-06 21:11:08.804162 mimesis-7.1.0/mimesis/builtins/da.py
--rw-r--r--   0        0        0     1776 2023-04-06 21:11:08.804162 mimesis-7.1.0/mimesis/builtins/en.py
--rw-r--r--   0        0        0     1543 2023-04-06 21:11:08.804162 mimesis-7.1.0/mimesis/builtins/it.py
--rw-r--r--   0        0        0     1535 2023-04-06 21:11:08.804162 mimesis-7.1.0/mimesis/builtins/nl.py
--rw-r--r--   0        0        0     3281 2023-04-06 21:11:08.804162 mimesis-7.1.0/mimesis/builtins/pl.py
--rw-r--r--   0        0        0     3354 2023-04-06 21:11:08.804162 mimesis-7.1.0/mimesis/builtins/pt_br.py
--rw-r--r--   0        0        0     7494 2023-04-06 21:11:08.804162 mimesis-7.1.0/mimesis/builtins/ru.py
--rw-r--r--   0        0        0     1083 2023-04-06 21:11:08.808162 mimesis-7.1.0/mimesis/builtins/uk.py
--rw-r--r--   0        0        0      127 2023-04-06 21:11:08.808162 mimesis-7.1.0/mimesis/compat.py
--rw-r--r--   0        0        0      403 2023-04-06 21:11:08.808162 mimesis-7.1.0/mimesis/data/__init__.py
--rw-r--r--   0        0        0   182787 2023-04-06 21:11:08.808162 mimesis-7.1.0/mimesis/data/bin/sample.aac
--rw-r--r--   0        0        0   385692 2023-04-06 21:11:08.808162 mimesis-7.1.0/mimesis/data/bin/sample.docx
--rw-r--r--   0        0        0   115256 2023-04-06 21:11:08.808162 mimesis-7.1.0/mimesis/data/bin/sample.gif
--rw-r--r--   0        0        0      269 2023-04-06 21:11:08.808162 mimesis-7.1.0/mimesis/data/bin/sample.gz
--rw-r--r--   0        0        0    88187 2023-04-06 21:11:08.808162 mimesis-7.1.0/mimesis/data/bin/sample.jpg
--rw-r--r--   0        0        0   281424 2023-04-06 21:11:08.812162 mimesis-7.1.0/mimesis/data/bin/sample.mov
--rw-r--r--   0        0        0    67911 2023-04-06 21:11:08.812162 mimesis-7.1.0/mimesis/data/bin/sample.mp3
--rw-r--r--   0        0        0   304520 2023-04-06 21:11:08.812162 mimesis-7.1.0/mimesis/data/bin/sample.mp4
--rw-r--r--   0        0        0   414593 2023-04-06 21:11:08.816162 mimesis-7.1.0/mimesis/data/bin/sample.pdf
--rw-r--r--   0        0        0   221697 2023-04-06 21:11:08.816162 mimesis-7.1.0/mimesis/data/bin/sample.png
--rw-r--r--   0        0        0   223362 2023-04-06 21:11:08.816162 mimesis-7.1.0/mimesis/data/bin/sample.pptx
--rw-r--r--   0        0        0     4857 2023-04-06 21:11:08.816162 mimesis-7.1.0/mimesis/data/bin/sample.xlsx
--rw-r--r--   0        0        0      673 2023-04-06 21:11:08.816162 mimesis-7.1.0/mimesis/data/bin/sample.zip
--rw-r--r--   0        0        0    79583 2023-04-06 21:11:28.872534 mimesis-7.1.0/mimesis/data/cs/address.json
--rw-r--r--   0        0        0      515 2023-04-06 21:11:28.872534 mimesis-7.1.0/mimesis/data/cs/datetime.json
--rw-r--r--   0        0        0      360 2023-04-06 21:11:28.872534 mimesis-7.1.0/mimesis/data/cs/finance.json
--rw-r--r--   0        0        0     1845 2023-04-06 21:11:28.872534 mimesis-7.1.0/mimesis/data/cs/food.json
--rw-r--r--   0        0        0    33117 2023-04-06 21:11:28.876534 mimesis-7.1.0/mimesis/data/cs/person.json
--rw-r--r--   0        0        0    49335 2023-04-06 21:11:28.876534 mimesis-7.1.0/mimesis/data/cs/text.json
--rw-r--r--   0        0        0    82900 2023-04-06 21:11:28.880534 mimesis-7.1.0/mimesis/data/da/address.json
--rw-r--r--   0        0        0      494 2023-04-06 21:11:28.880534 mimesis-7.1.0/mimesis/data/da/datetime.json
--rw-r--r--   0        0        0     3481 2023-04-06 21:11:28.880534 mimesis-7.1.0/mimesis/data/da/finance.json
--rw-r--r--   0        0        0     3873 2023-04-06 21:11:28.880534 mimesis-7.1.0/mimesis/data/da/food.json
--rw-r--r--   0        0        0    23273 2023-04-06 21:11:28.880534 mimesis-7.1.0/mimesis/data/da/person.json
--rw-r--r--   0        0        0    17323 2023-04-06 21:11:28.880534 mimesis-7.1.0/mimesis/data/da/text.json
--rw-r--r--   0        0        0   251577 2023-04-06 21:11:28.888534 mimesis-7.1.0/mimesis/data/de/address.json
--rw-r--r--   0        0        0      512 2023-04-06 21:11:28.892534 mimesis-7.1.0/mimesis/data/de/datetime.json
--rw-r--r--   0        0        0     1718 2023-04-06 21:11:28.892534 mimesis-7.1.0/mimesis/data/de/finance.json
--rw-r--r--   0        0        0     6237 2023-04-06 21:11:28.892534 mimesis-7.1.0/mimesis/data/de/food.json
--rw-r--r--   0        0        0    18346 2023-04-06 21:11:28.892534 mimesis-7.1.0/mimesis/data/de/person.json
--rw-r--r--   0        0        0   773143 2023-04-06 21:11:28.908534 mimesis-7.1.0/mimesis/data/de/text.json
--rw-r--r--   0        0        0    73006 2023-04-06 21:11:28.908534 mimesis-7.1.0/mimesis/data/de-at/address.json
--rw-r--r--   0        0        0        2 2023-04-06 21:11:28.912535 mimesis-7.1.0/mimesis/data/de-at/datetime.json
--rw-r--r--   0        0        0     2759 2023-04-06 21:11:28.912535 mimesis-7.1.0/mimesis/data/de-at/finance.json
--rw-r--r--   0        0        0     2335 2023-04-06 21:11:28.912535 mimesis-7.1.0/mimesis/data/de-at/food.json
--rw-r--r--   0        0        0    28622 2023-04-06 21:11:28.912535 mimesis-7.1.0/mimesis/data/de-at/person.json
--rw-r--r--   0        0        0        2 2023-04-06 21:11:28.912535 mimesis-7.1.0/mimesis/data/de-at/text.json
--rw-r--r--   0        0        0    42841 2023-04-06 21:11:28.912535 mimesis-7.1.0/mimesis/data/de-ch/address.json
--rw-r--r--   0        0        0        2 2023-04-06 21:11:28.912535 mimesis-7.1.0/mimesis/data/de-ch/datetime.json
--rw-r--r--   0        0        0     4371 2023-04-06 21:11:28.912535 mimesis-7.1.0/mimesis/data/de-ch/finance.json
--rw-r--r--   0        0        0      152 2023-04-06 21:11:28.912535 mimesis-7.1.0/mimesis/data/de-ch/food.json
--rw-r--r--   0        0        0    71143 2023-04-06 21:11:28.916535 mimesis-7.1.0/mimesis/data/de-ch/person.json
--rw-r--r--   0        0        0        2 2023-04-06 21:11:28.916535 mimesis-7.1.0/mimesis/data/de-ch/text.json
--rw-r--r--   0        0        0    99824 2023-04-06 21:11:28.916535 mimesis-7.1.0/mimesis/data/el/address.json
--rw-r--r--   0        0        0      817 2023-04-06 21:11:28.920535 mimesis-7.1.0/mimesis/data/el/datetime.json
--rw-r--r--   0        0        0     1612 2023-04-06 21:11:28.920535 mimesis-7.1.0/mimesis/data/el/finance.json
--rw-r--r--   0        0        0     4461 2023-04-06 21:11:28.920535 mimesis-7.1.0/mimesis/data/el/food.json
--rw-r--r--   0        0        0    14494 2023-04-06 21:11:28.920535 mimesis-7.1.0/mimesis/data/el/person.json
--rw-r--r--   0        0        0    10297 2023-04-06 21:11:28.920535 mimesis-7.1.0/mimesis/data/el/text.json
--rw-r--r--   0        0        0    50488 2023-04-06 21:11:28.920535 mimesis-7.1.0/mimesis/data/en/address.json
--rw-r--r--   0        0        0        2 2023-04-06 21:11:28.920535 mimesis-7.1.0/mimesis/data/en/builtin.json
--rw-r--r--   0        0        0      501 2023-04-06 21:11:28.920535 mimesis-7.1.0/mimesis/data/en/datetime.json
--rw-r--r--   0        0        0    20887 2023-04-06 21:11:28.920535 mimesis-7.1.0/mimesis/data/en/finance.json
--rw-r--r--   0        0        0    14076 2023-04-06 21:11:28.924535 mimesis-7.1.0/mimesis/data/en/food.json
--rw-r--r--   0        0        0    64738 2023-04-06 21:11:28.924535 mimesis-7.1.0/mimesis/data/en/person.json
--rw-r--r--   0        0        0   343508 2023-04-06 21:11:28.932535 mimesis-7.1.0/mimesis/data/en/text.json
--rw-r--r--   0        0        0    68774 2023-04-06 21:11:28.936535 mimesis-7.1.0/mimesis/data/en-au/address.json
--rw-r--r--   0        0        0       49 2023-04-06 21:11:28.936535 mimesis-7.1.0/mimesis/data/en-au/datetime.json
--rw-r--r--   0        0        0   115714 2023-04-06 21:11:28.936535 mimesis-7.1.0/mimesis/data/en-au/finance.json
--rw-r--r--   0        0        0      504 2023-04-06 21:11:28.936535 mimesis-7.1.0/mimesis/data/en-au/food.json
--rw-r--r--   0        0        0    41658 2023-04-06 21:11:28.940535 mimesis-7.1.0/mimesis/data/en-au/person.json
--rw-r--r--   0        0        0        2 2023-04-06 21:11:28.940535 mimesis-7.1.0/mimesis/data/en-au/text.json
--rw-r--r--   0        0        0    24229 2023-04-06 21:11:28.940535 mimesis-7.1.0/mimesis/data/en-ca/address.json
--rw-r--r--   0        0        0       49 2023-04-06 21:11:28.940535 mimesis-7.1.0/mimesis/data/en-ca/datetime.json
--rw-r--r--   0        0        0     2892 2023-04-06 21:11:28.940535 mimesis-7.1.0/mimesis/data/en-ca/finance.json
--rw-r--r--   0        0        0        2 2023-04-06 21:11:28.940535 mimesis-7.1.0/mimesis/data/en-ca/food.json
--rw-r--r--   0        0        0    13729 2023-04-06 21:11:28.940535 mimesis-7.1.0/mimesis/data/en-ca/person.json
--rw-r--r--   0        0        0        2 2023-04-06 21:11:28.940535 mimesis-7.1.0/mimesis/data/en-ca/text.json
--rw-r--r--   0        0        0    84033 2023-04-06 21:11:28.944535 mimesis-7.1.0/mimesis/data/en-gb/address.json
--rw-r--r--   0        0        0       49 2023-04-06 21:11:28.944535 mimesis-7.1.0/mimesis/data/en-gb/datetime.json
--rw-r--r--   0        0        0     6514 2023-04-06 21:11:28.944535 mimesis-7.1.0/mimesis/data/en-gb/finance.json
--rw-r--r--   0        0        0     1316 2023-04-06 21:11:28.944535 mimesis-7.1.0/mimesis/data/en-gb/food.json
--rw-r--r--   0        0        0    45054 2023-04-06 21:11:28.944535 mimesis-7.1.0/mimesis/data/en-gb/person.json
--rw-r--r--   0        0        0        2 2023-04-06 21:11:28.944535 mimesis-7.1.0/mimesis/data/en-gb/text.json
--rw-r--r--   0        0        0    23805 2023-04-06 21:11:28.944535 mimesis-7.1.0/mimesis/data/es/address.json
--rw-r--r--   0        0        0      561 2023-04-06 21:11:28.948536 mimesis-7.1.0/mimesis/data/es/datetime.json
--rw-r--r--   0        0        0     1850 2023-04-06 21:11:28.948536 mimesis-7.1.0/mimesis/data/es/finance.json
--rw-r--r--   0        0        0     4757 2023-04-06 21:11:28.948536 mimesis-7.1.0/mimesis/data/es/food.json
--rw-r--r--   0        0        0    14143 2023-04-06 21:11:28.948536 mimesis-7.1.0/mimesis/data/es/person.json
--rw-r--r--   0        0        0   128149 2023-04-06 21:11:28.952535 mimesis-7.1.0/mimesis/data/es/text.json
--rw-r--r--   0        0        0    11619 2023-04-06 21:11:28.952535 mimesis-7.1.0/mimesis/data/es-mx/address.json
--rw-r--r--   0        0        0        2 2023-04-06 21:11:28.952535 mimesis-7.1.0/mimesis/data/es-mx/datetime.json
--rw-r--r--   0        0        0     2411 2023-04-06 21:11:28.952535 mimesis-7.1.0/mimesis/data/es-mx/finance.json
--rw-r--r--   0        0        0     1081 2023-04-06 21:11:28.952535 mimesis-7.1.0/mimesis/data/es-mx/food.json
--rw-r--r--   0        0        0    16998 2023-04-06 21:11:28.952535 mimesis-7.1.0/mimesis/data/es-mx/person.json
--rw-r--r--   0        0        0        2 2023-04-06 21:11:28.952535 mimesis-7.1.0/mimesis/data/es-mx/text.json
--rw-r--r--   0        0        0    21806 2023-04-06 21:11:28.952535 mimesis-7.1.0/mimesis/data/et/address.json
--rw-r--r--   0        0        0      533 2023-04-06 21:11:28.952535 mimesis-7.1.0/mimesis/data/et/datetime.json
--rw-r--r--   0        0        0     6381 2023-04-06 21:11:28.952535 mimesis-7.1.0/mimesis/data/et/finance.json
--rw-r--r--   0        0        0     3683 2023-04-06 21:11:28.952535 mimesis-7.1.0/mimesis/data/et/food.json
--rw-r--r--   0        0        0    33842 2023-04-06 21:11:28.956536 mimesis-7.1.0/mimesis/data/et/person.json
--rw-r--r--   0        0        0    11545 2023-04-06 21:11:28.956536 mimesis-7.1.0/mimesis/data/et/text.json
--rw-r--r--   0        0        0    13562 2023-04-06 21:11:28.956536 mimesis-7.1.0/mimesis/data/fa/address.json
--rw-r--r--   0        0        0      665 2023-04-06 21:11:28.956536 mimesis-7.1.0/mimesis/data/fa/datetime.json
--rw-r--r--   0        0        0     2398 2023-04-06 21:11:28.956536 mimesis-7.1.0/mimesis/data/fa/finance.json
--rw-r--r--   0        0        0     6628 2023-04-06 21:11:28.956536 mimesis-7.1.0/mimesis/data/fa/food.json
--rw-r--r--   0        0        0    56905 2023-04-06 21:11:28.956536 mimesis-7.1.0/mimesis/data/fa/person.json
--rw-r--r--   0        0        0    11302 2023-04-06 21:11:28.960536 mimesis-7.1.0/mimesis/data/fa/text.json
--rw-r--r--   0        0        0     5488 2023-04-06 21:11:28.960536 mimesis-7.1.0/mimesis/data/fi/address.json
--rw-r--r--   0        0        0      542 2023-04-06 21:11:28.960536 mimesis-7.1.0/mimesis/data/fi/datetime.json
--rw-r--r--   0        0        0     7726 2023-04-06 21:11:28.960536 mimesis-7.1.0/mimesis/data/fi/finance.json
--rw-r--r--   0        0        0     3674 2023-04-06 21:11:28.960536 mimesis-7.1.0/mimesis/data/fi/food.json
--rw-r--r--   0        0        0    26719 2023-04-06 21:11:28.960536 mimesis-7.1.0/mimesis/data/fi/person.json
--rw-r--r--   0        0        0    57968 2023-04-06 21:11:28.964536 mimesis-7.1.0/mimesis/data/fi/text.json
--rw-r--r--   0        0        0    39318 2023-04-06 21:11:28.964536 mimesis-7.1.0/mimesis/data/fr/address.json
--rw-r--r--   0        0        0      529 2023-04-06 21:11:28.964536 mimesis-7.1.0/mimesis/data/fr/datetime.json
--rw-r--r--   0        0        0     2520 2023-04-06 21:11:28.964536 mimesis-7.1.0/mimesis/data/fr/finance.json
--rw-r--r--   0        0        0     7024 2023-04-06 21:11:28.964536 mimesis-7.1.0/mimesis/data/fr/food.json
--rw-r--r--   0        0        0    46272 2023-04-06 21:11:28.964536 mimesis-7.1.0/mimesis/data/fr/person.json
--rw-r--r--   0        0        0    37433 2023-04-06 21:11:28.968536 mimesis-7.1.0/mimesis/data/fr/text.json
--rw-r--r--   0        0        0    13842 2023-04-06 21:11:28.968536 mimesis-7.1.0/mimesis/data/hu/address.json
--rw-r--r--   0        0        0      515 2023-04-06 21:11:28.968536 mimesis-7.1.0/mimesis/data/hu/datetime.json
--rw-r--r--   0        0        0      545 2023-04-06 21:11:28.968536 mimesis-7.1.0/mimesis/data/hu/finance.json
--rw-r--r--   0        0        0     4302 2023-04-06 21:11:28.968536 mimesis-7.1.0/mimesis/data/hu/food.json
--rw-r--r--   0        0        0    26944 2023-04-06 21:11:28.968536 mimesis-7.1.0/mimesis/data/hu/person.json
--rw-r--r--   0        0        0    22876 2023-04-06 21:11:28.968536 mimesis-7.1.0/mimesis/data/hu/text.json
--rw-r--r--   0        0        0      398 2023-04-06 21:11:08.840163 mimesis-7.1.0/mimesis/data/int/__init__.py
--rw-r--r--   0        0        0    20986 2023-04-06 21:11:08.840163 mimesis-7.1.0/mimesis/data/int/address.py
--rw-r--r--   0        0        0     2735 2023-04-06 21:11:08.840163 mimesis-7.1.0/mimesis/data/int/code.py
--rw-r--r--   0        0        0     2223 2023-04-06 21:11:08.840163 mimesis-7.1.0/mimesis/data/int/common.py
--rw-r--r--   0        0        0    27537 2023-04-06 21:11:08.840163 mimesis-7.1.0/mimesis/data/int/cryptographic.py
--rw-r--r--   0        0        0    11625 2023-04-06 21:11:08.840163 mimesis-7.1.0/mimesis/data/int/datetime.py
--rw-r--r--   0        0        0     7778 2023-04-06 21:11:08.840163 mimesis-7.1.0/mimesis/data/int/development.py
--rw-r--r--   0        0        0    67892 2023-04-06 21:11:08.840163 mimesis-7.1.0/mimesis/data/int/file.py
--rw-r--r--   0        0        0   264126 2023-04-06 21:11:08.844164 mimesis-7.1.0/mimesis/data/int/finance.py
--rw-r--r--   0        0        0     5221 2023-04-06 21:11:08.844164 mimesis-7.1.0/mimesis/data/int/hardware.py
--rw-r--r--   0        0        0    37473 2023-04-06 21:11:08.844164 mimesis-7.1.0/mimesis/data/int/internet.py
--rw-r--r--   0        0        0      320 2023-04-06 21:11:08.844164 mimesis-7.1.0/mimesis/data/int/path.py
--rw-r--r--   0        0        0      171 2023-04-06 21:11:08.844164 mimesis-7.1.0/mimesis/data/int/payment.py
--rw-r--r--   0        0        0   140341 2023-04-06 21:11:08.844164 mimesis-7.1.0/mimesis/data/int/person.py
--rw-r--r--   0        0        0      606 2023-04-06 21:11:08.844164 mimesis-7.1.0/mimesis/data/int/scientific.py
--rw-r--r--   0        0        0      364 2023-04-06 21:11:08.844164 mimesis-7.1.0/mimesis/data/int/text.py
--rw-r--r--   0        0        0    31498 2023-04-06 21:11:08.844164 mimesis-7.1.0/mimesis/data/int/transport.py
--rw-r--r--   0        0        0   121675 2023-04-06 21:11:28.972536 mimesis-7.1.0/mimesis/data/is/address.json
--rw-r--r--   0        0        0      546 2023-04-06 21:11:28.976536 mimesis-7.1.0/mimesis/data/is/datetime.json
--rw-r--r--   0        0        0     1473 2023-04-06 21:11:28.976536 mimesis-7.1.0/mimesis/data/is/finance.json
--rw-r--r--   0        0        0     1651 2023-04-06 21:11:28.976536 mimesis-7.1.0/mimesis/data/is/food.json
--rw-r--r--   0        0        0    68768 2023-04-06 21:11:28.976536 mimesis-7.1.0/mimesis/data/is/person.json
--rw-r--r--   0        0        0    51794 2023-04-06 21:11:28.980536 mimesis-7.1.0/mimesis/data/is/text.json
--rw-r--r--   0        0        0   123349 2023-04-06 21:11:28.984536 mimesis-7.1.0/mimesis/data/it/address.json
--rw-r--r--   0        0        0      142 2023-04-06 21:11:28.984536 mimesis-7.1.0/mimesis/data/it/builtin.json
--rw-r--r--   0        0        0      535 2023-04-06 21:11:28.984536 mimesis-7.1.0/mimesis/data/it/datetime.json
--rw-r--r--   0        0        0     4416 2023-04-06 21:11:28.984536 mimesis-7.1.0/mimesis/data/it/finance.json
--rw-r--r--   0        0        0     5352 2023-04-06 21:11:28.984536 mimesis-7.1.0/mimesis/data/it/food.json
--rw-r--r--   0        0        0    64650 2023-04-06 21:11:28.984536 mimesis-7.1.0/mimesis/data/it/person.json
--rw-r--r--   0        0        0    77862 2023-04-06 21:11:28.988536 mimesis-7.1.0/mimesis/data/it/text.json
--rw-r--r--   0        0        0    10631 2023-04-06 21:11:28.988536 mimesis-7.1.0/mimesis/data/ja/address.json
--rw-r--r--   0        0        0      494 2023-04-06 21:11:28.988536 mimesis-7.1.0/mimesis/data/ja/datetime.json
--rw-r--r--   0        0        0    22437 2023-04-06 21:11:28.988536 mimesis-7.1.0/mimesis/data/ja/finance.json
--rw-r--r--   0        0        0    13902 2023-04-06 21:11:28.988536 mimesis-7.1.0/mimesis/data/ja/food.json
--rw-r--r--   0        0        0    69460 2023-04-06 21:11:28.992536 mimesis-7.1.0/mimesis/data/ja/person.json
--rw-r--r--   0        0        0    56672 2023-04-06 21:11:28.992536 mimesis-7.1.0/mimesis/data/ja/text.json
--rw-r--r--   0        0        0    33301 2023-04-06 21:11:28.992536 mimesis-7.1.0/mimesis/data/kk/address.json
--rw-r--r--   0        0        0      768 2023-04-06 21:11:28.992536 mimesis-7.1.0/mimesis/data/kk/datetime.json
--rw-r--r--   0        0        0     6526 2023-04-06 21:11:28.992536 mimesis-7.1.0/mimesis/data/kk/finance.json
--rw-r--r--   0        0        0       95 2023-04-06 21:11:28.992536 mimesis-7.1.0/mimesis/data/kk/food.json
--rw-r--r--   0        0        0    28448 2023-04-06 21:11:28.996537 mimesis-7.1.0/mimesis/data/kk/person.json
--rw-r--r--   0        0        0    14350 2023-04-06 21:11:28.996537 mimesis-7.1.0/mimesis/data/kk/text.json
--rw-r--r--   0        0        0    30313 2023-04-06 21:11:28.996537 mimesis-7.1.0/mimesis/data/ko/address.json
--rw-r--r--   0        0        0      492 2023-04-06 21:11:28.996537 mimesis-7.1.0/mimesis/data/ko/datetime.json
--rw-r--r--   0        0        0    17399 2023-04-06 21:11:28.996537 mimesis-7.1.0/mimesis/data/ko/finance.json
--rw-r--r--   0        0        0    12695 2023-04-06 21:11:28.996537 mimesis-7.1.0/mimesis/data/ko/food.json
--rw-r--r--   0        0        0    39279 2023-04-06 21:11:29.000537 mimesis-7.1.0/mimesis/data/ko/person.json
--rw-r--r--   0        0        0    68560 2023-04-06 21:11:29.000537 mimesis-7.1.0/mimesis/data/ko/text.json
--rw-r--r--   0        0        0    60825 2023-04-06 21:11:29.004537 mimesis-7.1.0/mimesis/data/nl/address.json
--rw-r--r--   0        0        0      507 2023-04-06 21:11:29.004537 mimesis-7.1.0/mimesis/data/nl/datetime.json
--rw-r--r--   0        0        0     1312 2023-04-06 21:11:29.004537 mimesis-7.1.0/mimesis/data/nl/finance.json
--rw-r--r--   0        0        0     7412 2023-04-06 21:11:29.004537 mimesis-7.1.0/mimesis/data/nl/food.json
--rw-r--r--   0        0        0   109294 2023-04-06 21:11:29.008537 mimesis-7.1.0/mimesis/data/nl/person.json
--rw-r--r--   0        0        0   202851 2023-04-06 21:11:29.012537 mimesis-7.1.0/mimesis/data/nl/text.json
--rw-r--r--   0        0        0    53656 2023-04-06 21:11:29.012537 mimesis-7.1.0/mimesis/data/nl-be/address.json
--rw-r--r--   0        0        0       31 2023-04-06 21:11:29.012537 mimesis-7.1.0/mimesis/data/nl-be/datetime.json
--rw-r--r--   0        0        0     2097 2023-04-06 21:11:29.012537 mimesis-7.1.0/mimesis/data/nl-be/finance.json
--rw-r--r--   0        0        0        2 2023-04-06 21:11:29.016537 mimesis-7.1.0/mimesis/data/nl-be/food.json
--rw-r--r--   0        0        0     1371 2023-04-06 21:11:29.016537 mimesis-7.1.0/mimesis/data/nl-be/person.json
--rw-r--r--   0        0        0        2 2023-04-06 21:11:29.016537 mimesis-7.1.0/mimesis/data/nl-be/text.json
--rw-r--r--   0        0        0    40052 2023-04-06 21:11:29.016537 mimesis-7.1.0/mimesis/data/no/address.json
--rw-r--r--   0        0        0      500 2023-04-06 21:11:29.016537 mimesis-7.1.0/mimesis/data/no/datetime.json
--rw-r--r--   0        0        0     9629 2023-04-06 21:11:29.016537 mimesis-7.1.0/mimesis/data/no/finance.json
--rw-r--r--   0        0        0     4479 2023-04-06 21:11:29.016537 mimesis-7.1.0/mimesis/data/no/food.json
--rw-r--r--   0        0        0    43488 2023-04-06 21:11:29.016537 mimesis-7.1.0/mimesis/data/no/person.json
--rw-r--r--   0        0        0    31334 2023-04-06 21:11:29.020537 mimesis-7.1.0/mimesis/data/no/text.json
--rw-r--r--   0        0        0    80118 2023-04-06 21:11:29.020537 mimesis-7.1.0/mimesis/data/pl/address.json
--rw-r--r--   0        0        0      567 2023-04-06 21:11:29.020537 mimesis-7.1.0/mimesis/data/pl/datetime.json
--rw-r--r--   0        0        0     9475 2023-04-06 21:11:29.024537 mimesis-7.1.0/mimesis/data/pl/finance.json
--rw-r--r--   0        0        0     4693 2023-04-06 21:11:29.024537 mimesis-7.1.0/mimesis/data/pl/food.json
--rw-r--r--   0        0        0    27705 2023-04-06 21:11:29.024537 mimesis-7.1.0/mimesis/data/pl/person.json
--rw-r--r--   0        0        0    65088 2023-04-06 21:11:29.024537 mimesis-7.1.0/mimesis/data/pl/text.json
--rw-r--r--   0        0        0    19169 2023-04-06 21:11:29.028537 mimesis-7.1.0/mimesis/data/pt/address.json
--rw-r--r--   0        0        0      563 2023-04-06 21:11:29.028537 mimesis-7.1.0/mimesis/data/pt/datetime.json
--rw-r--r--   0        0        0     1336 2023-04-06 21:11:29.028537 mimesis-7.1.0/mimesis/data/pt/finance.json
--rw-r--r--   0        0        0     4310 2023-04-06 21:11:29.028537 mimesis-7.1.0/mimesis/data/pt/food.json
--rw-r--r--   0        0        0    38175 2023-04-06 21:11:29.028537 mimesis-7.1.0/mimesis/data/pt/person.json
--rw-r--r--   0        0        0    25766 2023-04-06 21:11:29.028537 mimesis-7.1.0/mimesis/data/pt/text.json
--rw-r--r--   0        0        0    94350 2023-04-06 21:11:29.032538 mimesis-7.1.0/mimesis/data/pt-br/address.json
--rw-r--r--   0        0        0      564 2023-04-06 21:11:29.032538 mimesis-7.1.0/mimesis/data/pt-br/datetime.json
--rw-r--r--   0        0        0    23474 2023-04-06 21:11:29.032538 mimesis-7.1.0/mimesis/data/pt-br/finance.json
--rw-r--r--   0        0        0     3162 2023-04-06 21:11:29.032538 mimesis-7.1.0/mimesis/data/pt-br/food.json
--rw-r--r--   0        0        0    63714 2023-04-06 21:11:29.036538 mimesis-7.1.0/mimesis/data/pt-br/person.json
--rw-r--r--   0        0        0        2 2023-04-06 21:11:29.036538 mimesis-7.1.0/mimesis/data/pt-br/text.json
--rw-r--r--   0        0        0   101129 2023-04-06 21:11:29.036538 mimesis-7.1.0/mimesis/data/ru/address.json
--rw-r--r--   0        0        0    10949 2023-04-06 21:11:29.036538 mimesis-7.1.0/mimesis/data/ru/builtin.json
--rw-r--r--   0        0        0      790 2023-04-06 21:11:29.040538 mimesis-7.1.0/mimesis/data/ru/datetime.json
--rw-r--r--   0        0        0    21038 2023-04-06 21:11:29.040538 mimesis-7.1.0/mimesis/data/ru/finance.json
--rw-r--r--   0        0        0    20262 2023-04-06 21:11:29.040538 mimesis-7.1.0/mimesis/data/ru/food.json
--rw-r--r--   0        0        0    86369 2023-04-06 21:11:29.040538 mimesis-7.1.0/mimesis/data/ru/person.json
--rw-r--r--   0        0        0    89215 2023-04-06 21:11:29.044538 mimesis-7.1.0/mimesis/data/ru/text.json
--rw-r--r--   0        0        0    38882 2023-04-06 21:11:29.044538 mimesis-7.1.0/mimesis/data/sk/address.json
--rw-r--r--   0        0        0      485 2023-04-06 21:11:29.044538 mimesis-7.1.0/mimesis/data/sk/datetime.json
--rw-r--r--   0        0        0      236 2023-04-06 21:11:29.044538 mimesis-7.1.0/mimesis/data/sk/finance.json
--rw-r--r--   0        0        0      284 2023-04-06 21:11:29.044538 mimesis-7.1.0/mimesis/data/sk/food.json
--rw-r--r--   0        0        0     5828 2023-04-06 21:11:29.044538 mimesis-7.1.0/mimesis/data/sk/person.json
--rw-r--r--   0        0        0      752 2023-04-06 21:11:29.044538 mimesis-7.1.0/mimesis/data/sk/text.json
--rw-r--r--   0        0        0    97258 2023-04-06 21:11:29.048538 mimesis-7.1.0/mimesis/data/sv/address.json
--rw-r--r--   0        0        0      508 2023-04-06 21:11:29.048538 mimesis-7.1.0/mimesis/data/sv/datetime.json
--rw-r--r--   0        0        0     4278 2023-04-06 21:11:29.048538 mimesis-7.1.0/mimesis/data/sv/finance.json
--rw-r--r--   0        0        0     6863 2023-04-06 21:11:29.048538 mimesis-7.1.0/mimesis/data/sv/food.json
--rw-r--r--   0        0        0    32781 2023-04-06 21:11:29.052538 mimesis-7.1.0/mimesis/data/sv/person.json
--rw-r--r--   0        0        0    41878 2023-04-06 21:11:29.052538 mimesis-7.1.0/mimesis/data/sv/text.json
--rw-r--r--   0        0        0    12375 2023-04-06 21:11:29.052538 mimesis-7.1.0/mimesis/data/tr/address.json
--rw-r--r--   0        0        0      508 2023-04-06 21:11:29.052538 mimesis-7.1.0/mimesis/data/tr/datetime.json
--rw-r--r--   0        0        0    10537 2023-04-06 21:11:29.052538 mimesis-7.1.0/mimesis/data/tr/finance.json
--rw-r--r--   0        0        0     1819 2023-04-06 21:11:29.052538 mimesis-7.1.0/mimesis/data/tr/food.json
--rw-r--r--   0        0        0    29265 2023-04-06 21:11:29.056538 mimesis-7.1.0/mimesis/data/tr/person.json
--rw-r--r--   0        0        0     8857 2023-04-06 21:11:29.056538 mimesis-7.1.0/mimesis/data/tr/text.json
--rw-r--r--   0        0        0    54571 2023-04-06 21:11:29.056538 mimesis-7.1.0/mimesis/data/uk/address.json
--rw-r--r--   0        0        0     6247 2023-04-06 21:11:29.056538 mimesis-7.1.0/mimesis/data/uk/builtin.json
--rw-r--r--   0        0        0      790 2023-04-06 21:11:29.056538 mimesis-7.1.0/mimesis/data/uk/datetime.json
--rw-r--r--   0        0        0     5734 2023-04-06 21:11:29.056538 mimesis-7.1.0/mimesis/data/uk/finance.json
--rw-r--r--   0        0        0     9121 2023-04-06 21:11:29.056538 mimesis-7.1.0/mimesis/data/uk/food.json
--rw-r--r--   0        0        0    52753 2023-04-06 21:11:29.060538 mimesis-7.1.0/mimesis/data/uk/person.json
--rw-r--r--   0        0        0    21072 2023-04-06 21:11:29.060538 mimesis-7.1.0/mimesis/data/uk/text.json
--rw-r--r--   0        0        0    10240 2023-04-06 21:11:29.060538 mimesis-7.1.0/mimesis/data/zh/address.json
--rw-r--r--   0        0        0      539 2023-04-06 21:11:29.060538 mimesis-7.1.0/mimesis/data/zh/datetime.json
--rw-r--r--   0        0        0     1762 2023-04-06 21:11:29.060538 mimesis-7.1.0/mimesis/data/zh/finance.json
--rw-r--r--   0        0        0     2301 2023-04-06 21:11:29.060538 mimesis-7.1.0/mimesis/data/zh/food.json
--rw-r--r--   0        0        0    96427 2023-04-06 21:11:29.064538 mimesis-7.1.0/mimesis/data/zh/person.json
--rw-r--r--   0        0        0    17796 2023-04-06 21:11:29.064538 mimesis-7.1.0/mimesis/data/zh/text.json
--rw-r--r--   0        0        0      377 2023-04-06 21:11:08.864164 mimesis-7.1.0/mimesis/entrypoints.py
--rw-r--r--   0        0        0     6827 2023-04-06 21:11:08.864164 mimesis-7.1.0/mimesis/enums.py
--rw-r--r--   0        0        0     1712 2023-04-06 21:11:08.864164 mimesis-7.1.0/mimesis/exceptions.py
--rw-r--r--   0        0        0      507 2023-04-06 21:11:08.864164 mimesis-7.1.0/mimesis/locales.py
--rw-r--r--   0        0        0     1450 2023-04-06 21:11:08.864164 mimesis-7.1.0/mimesis/providers/__init__.py
--rw-r--r--   0        0        0     7716 2023-04-06 21:11:08.864164 mimesis-7.1.0/mimesis/providers/address.py
--rw-r--r--   0        0        0     7676 2023-04-06 21:11:08.864164 mimesis-7.1.0/mimesis/providers/base.py
--rw-r--r--   0        0        0     3058 2023-04-06 21:11:08.864164 mimesis-7.1.0/mimesis/providers/binaryfile.py
--rw-r--r--   0        0        0     3190 2023-04-06 21:11:08.864164 mimesis-7.1.0/mimesis/providers/choice.py
--rw-r--r--   0        0        0     2655 2023-04-06 21:11:08.864164 mimesis-7.1.0/mimesis/providers/code.py
--rw-r--r--   0        0        0     3325 2023-04-06 21:11:08.864164 mimesis-7.1.0/mimesis/providers/cryptographic.py
--rw-r--r--   0        0        0     8676 2023-04-06 21:11:08.864164 mimesis-7.1.0/mimesis/providers/date.py
--rw-r--r--   0        0        0     2768 2023-04-06 21:11:08.864164 mimesis-7.1.0/mimesis/providers/development.py
--rw-r--r--   0        0        0     2136 2023-04-06 21:11:08.864164 mimesis-7.1.0/mimesis/providers/file.py
--rw-r--r--   0        0        0     3556 2023-04-06 21:11:08.864164 mimesis-7.1.0/mimesis/providers/finance.py
--rw-r--r--   0        0        0     1712 2023-04-06 21:11:08.868164 mimesis-7.1.0/mimesis/providers/food.py
--rw-r--r--   0        0        0     5419 2023-04-06 21:11:08.868164 mimesis-7.1.0/mimesis/providers/generic.py
--rw-r--r--   0        0        0     3044 2023-04-06 21:11:08.868164 mimesis-7.1.0/mimesis/providers/hardware.py
--rw-r--r--   0        0        0    15706 2023-04-06 21:11:08.868164 mimesis-7.1.0/mimesis/providers/internet.py
--rw-r--r--   0        0        0     7042 2023-04-06 21:11:08.868164 mimesis-7.1.0/mimesis/providers/numeric.py
--rw-r--r--   0        0        0     2746 2023-04-06 21:11:08.868164 mimesis-7.1.0/mimesis/providers/path.py
--rw-r--r--   0        0        0     5199 2023-04-06 21:11:08.868164 mimesis-7.1.0/mimesis/providers/payment.py
--rw-r--r--   0        0        0    13766 2023-04-06 21:11:08.868164 mimesis-7.1.0/mimesis/providers/person.py
--rw-r--r--   0        0        0     2126 2023-04-06 21:11:08.868164 mimesis-7.1.0/mimesis/providers/science.py
--rw-r--r--   0        0        0     4375 2023-04-06 21:11:08.868164 mimesis-7.1.0/mimesis/providers/text.py
--rw-r--r--   0        0        0     1454 2023-04-06 21:11:08.868164 mimesis-7.1.0/mimesis/providers/transport.py
--rw-r--r--   0        0        0        1 2023-04-06 21:11:08.868164 mimesis-7.1.0/mimesis/py.typed
--rw-r--r--   0        0        0     4502 2023-04-06 21:11:08.868164 mimesis-7.1.0/mimesis/random.py
--rw-r--r--   0        0        0    11691 2023-04-06 21:11:08.868164 mimesis-7.1.0/mimesis/schema.py
--rw-r--r--   0        0        0     1373 2023-04-06 21:11:08.868164 mimesis-7.1.0/mimesis/shortcuts.py
--rw-r--r--   0        0        0     1190 2023-04-06 21:11:08.868164 mimesis-7.1.0/mimesis/types.py
--rw-r--r--   0        0        0     2743 2023-04-06 21:11:08.868164 mimesis-7.1.0/pyproject.toml
--rw-r--r--   0        0        0     8504 1970-01-01 00:00:00.000000 mimesis-7.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1123 2023-04-16 14:18:20.002791 mimesis-8.0.0/LICENSE
+-rw-r--r--   0        0        0     6945 2023-04-16 14:18:20.002791 mimesis-8.0.0/README.rst
+-rw-r--r--   0        0        0     2312 2023-04-16 14:18:20.010791 mimesis-8.0.0/mimesis/__init__.py
+-rw-r--r--   0        0        0      552 2023-04-16 14:18:20.010791 mimesis-8.0.0/mimesis/builtins/__init__.py
+-rw-r--r--   0        0        0      428 2023-04-16 14:18:20.010791 mimesis-8.0.0/mimesis/builtins/base.py
+-rw-r--r--   0        0        0     3671 2023-04-16 14:18:20.010791 mimesis-8.0.0/mimesis/builtins/da.py
+-rw-r--r--   0        0        0     1776 2023-04-16 14:18:20.010791 mimesis-8.0.0/mimesis/builtins/en.py
+-rw-r--r--   0        0        0     1543 2023-04-16 14:18:20.010791 mimesis-8.0.0/mimesis/builtins/it.py
+-rw-r--r--   0        0        0     1535 2023-04-16 14:18:20.010791 mimesis-8.0.0/mimesis/builtins/nl.py
+-rw-r--r--   0        0        0     3281 2023-04-16 14:18:20.010791 mimesis-8.0.0/mimesis/builtins/pl.py
+-rw-r--r--   0        0        0     3354 2023-04-16 14:18:20.010791 mimesis-8.0.0/mimesis/builtins/pt_br.py
+-rw-r--r--   0        0        0     7494 2023-04-16 14:18:20.010791 mimesis-8.0.0/mimesis/builtins/ru.py
+-rw-r--r--   0        0        0     1083 2023-04-16 14:18:20.010791 mimesis-8.0.0/mimesis/builtins/uk.py
+-rw-r--r--   0        0        0      127 2023-04-16 14:18:20.010791 mimesis-8.0.0/mimesis/compat.py
+-rw-r--r--   0        0        0      403 2023-04-16 14:18:20.010791 mimesis-8.0.0/mimesis/data/__init__.py
+-rw-r--r--   0        0        0   182787 2023-04-16 14:18:20.010791 mimesis-8.0.0/mimesis/data/bin/sample.aac
+-rw-r--r--   0        0        0   385692 2023-04-16 14:18:20.014791 mimesis-8.0.0/mimesis/data/bin/sample.docx
+-rw-r--r--   0        0        0   115256 2023-04-16 14:18:20.014791 mimesis-8.0.0/mimesis/data/bin/sample.gif
+-rw-r--r--   0        0        0      269 2023-04-16 14:18:20.014791 mimesis-8.0.0/mimesis/data/bin/sample.gz
+-rw-r--r--   0        0        0    88187 2023-04-16 14:18:20.014791 mimesis-8.0.0/mimesis/data/bin/sample.jpg
+-rw-r--r--   0        0        0   281424 2023-04-16 14:18:20.014791 mimesis-8.0.0/mimesis/data/bin/sample.mov
+-rw-r--r--   0        0        0    67911 2023-04-16 14:18:20.018791 mimesis-8.0.0/mimesis/data/bin/sample.mp3
+-rw-r--r--   0        0        0   304520 2023-04-16 14:18:20.018791 mimesis-8.0.0/mimesis/data/bin/sample.mp4
+-rw-r--r--   0        0        0   414593 2023-04-16 14:18:20.022791 mimesis-8.0.0/mimesis/data/bin/sample.pdf
+-rw-r--r--   0        0        0   221697 2023-04-16 14:18:20.022791 mimesis-8.0.0/mimesis/data/bin/sample.png
+-rw-r--r--   0        0        0   223362 2023-04-16 14:18:20.022791 mimesis-8.0.0/mimesis/data/bin/sample.pptx
+-rw-r--r--   0        0        0     4857 2023-04-16 14:18:20.022791 mimesis-8.0.0/mimesis/data/bin/sample.xlsx
+-rw-r--r--   0        0        0      673 2023-04-16 14:18:20.022791 mimesis-8.0.0/mimesis/data/bin/sample.zip
+-rw-r--r--   0        0        0    79583 2023-04-16 14:18:41.762841 mimesis-8.0.0/mimesis/data/cs/address.json
+-rw-r--r--   0        0        0      515 2023-04-16 14:18:41.762841 mimesis-8.0.0/mimesis/data/cs/datetime.json
+-rw-r--r--   0        0        0     1340 2023-04-16 14:18:41.762841 mimesis-8.0.0/mimesis/data/cs/finance.json
+-rw-r--r--   0        0        0     1845 2023-04-16 14:18:41.762841 mimesis-8.0.0/mimesis/data/cs/food.json
+-rw-r--r--   0        0        0    33117 2023-04-16 14:18:41.766841 mimesis-8.0.0/mimesis/data/cs/person.json
+-rw-r--r--   0        0        0    49335 2023-04-16 14:18:41.766841 mimesis-8.0.0/mimesis/data/cs/text.json
+-rw-r--r--   0        0        0    82900 2023-04-16 14:18:41.770841 mimesis-8.0.0/mimesis/data/da/address.json
+-rw-r--r--   0        0        0      494 2023-04-16 14:18:41.770841 mimesis-8.0.0/mimesis/data/da/datetime.json
+-rw-r--r--   0        0        0     4656 2023-04-16 14:18:41.770841 mimesis-8.0.0/mimesis/data/da/finance.json
+-rw-r--r--   0        0        0     3873 2023-04-16 14:18:41.770841 mimesis-8.0.0/mimesis/data/da/food.json
+-rw-r--r--   0        0        0    23273 2023-04-16 14:18:41.770841 mimesis-8.0.0/mimesis/data/da/person.json
+-rw-r--r--   0        0        0    17323 2023-04-16 14:18:41.770841 mimesis-8.0.0/mimesis/data/da/text.json
+-rw-r--r--   0        0        0   251577 2023-04-16 14:18:41.778841 mimesis-8.0.0/mimesis/data/de/address.json
+-rw-r--r--   0        0        0      512 2023-04-16 14:18:41.778841 mimesis-8.0.0/mimesis/data/de/datetime.json
+-rw-r--r--   0        0        0     3497 2023-04-16 14:18:41.782841 mimesis-8.0.0/mimesis/data/de/finance.json
+-rw-r--r--   0        0        0     6237 2023-04-16 14:18:41.782841 mimesis-8.0.0/mimesis/data/de/food.json
+-rw-r--r--   0        0        0    18346 2023-04-16 14:18:41.782841 mimesis-8.0.0/mimesis/data/de/person.json
+-rw-r--r--   0        0        0   773143 2023-04-16 14:18:41.798841 mimesis-8.0.0/mimesis/data/de/text.json
+-rw-r--r--   0        0        0    73006 2023-04-16 14:18:41.798841 mimesis-8.0.0/mimesis/data/de-at/address.json
+-rw-r--r--   0        0        0        2 2023-04-16 14:18:41.798841 mimesis-8.0.0/mimesis/data/de-at/datetime.json
+-rw-r--r--   0        0        0     4538 2023-04-16 14:18:41.798841 mimesis-8.0.0/mimesis/data/de-at/finance.json
+-rw-r--r--   0        0        0     2335 2023-04-16 14:18:41.798841 mimesis-8.0.0/mimesis/data/de-at/food.json
+-rw-r--r--   0        0        0    28622 2023-04-16 14:18:41.802841 mimesis-8.0.0/mimesis/data/de-at/person.json
+-rw-r--r--   0        0        0        2 2023-04-16 14:18:41.802841 mimesis-8.0.0/mimesis/data/de-at/text.json
+-rw-r--r--   0        0        0    42841 2023-04-16 14:18:41.802841 mimesis-8.0.0/mimesis/data/de-ch/address.json
+-rw-r--r--   0        0        0        2 2023-04-16 14:18:41.802841 mimesis-8.0.0/mimesis/data/de-ch/datetime.json
+-rw-r--r--   0        0        0     9750 2023-04-16 14:18:41.802841 mimesis-8.0.0/mimesis/data/de-ch/finance.json
+-rw-r--r--   0        0        0      152 2023-04-16 14:18:41.802841 mimesis-8.0.0/mimesis/data/de-ch/food.json
+-rw-r--r--   0        0        0    71143 2023-04-16 14:18:41.806841 mimesis-8.0.0/mimesis/data/de-ch/person.json
+-rw-r--r--   0        0        0        2 2023-04-16 14:18:41.806841 mimesis-8.0.0/mimesis/data/de-ch/text.json
+-rw-r--r--   0        0        0    99824 2023-04-16 14:18:41.806841 mimesis-8.0.0/mimesis/data/el/address.json
+-rw-r--r--   0        0        0      817 2023-04-16 14:18:41.806841 mimesis-8.0.0/mimesis/data/el/datetime.json
+-rw-r--r--   0        0        0     2249 2023-04-16 14:18:41.806841 mimesis-8.0.0/mimesis/data/el/finance.json
+-rw-r--r--   0        0        0     4461 2023-04-16 14:18:41.806841 mimesis-8.0.0/mimesis/data/el/food.json
+-rw-r--r--   0        0        0    14494 2023-04-16 14:18:41.806841 mimesis-8.0.0/mimesis/data/el/person.json
+-rw-r--r--   0        0        0    10297 2023-04-16 14:18:41.806841 mimesis-8.0.0/mimesis/data/el/text.json
+-rw-r--r--   0        0        0    50488 2023-04-16 14:18:41.810841 mimesis-8.0.0/mimesis/data/en/address.json
+-rw-r--r--   0        0        0        2 2023-04-16 14:18:41.810841 mimesis-8.0.0/mimesis/data/en/builtin.json
+-rw-r--r--   0        0        0      501 2023-04-16 14:18:41.810841 mimesis-8.0.0/mimesis/data/en/datetime.json
+-rw-r--r--   0        0        0    24968 2023-04-16 14:18:41.810841 mimesis-8.0.0/mimesis/data/en/finance.json
+-rw-r--r--   0        0        0    14076 2023-04-16 14:18:41.810841 mimesis-8.0.0/mimesis/data/en/food.json
+-rw-r--r--   0        0        0    64738 2023-04-16 14:18:41.814841 mimesis-8.0.0/mimesis/data/en/person.json
+-rw-r--r--   0        0        0   343508 2023-04-16 14:18:41.822841 mimesis-8.0.0/mimesis/data/en/text.json
+-rw-r--r--   0        0        0    68774 2023-04-16 14:18:41.822841 mimesis-8.0.0/mimesis/data/en-au/address.json
+-rw-r--r--   0        0        0       49 2023-04-16 14:18:41.822841 mimesis-8.0.0/mimesis/data/en-au/datetime.json
+-rw-r--r--   0        0        0   117507 2023-04-16 14:18:41.826841 mimesis-8.0.0/mimesis/data/en-au/finance.json
+-rw-r--r--   0        0        0      504 2023-04-16 14:18:41.826841 mimesis-8.0.0/mimesis/data/en-au/food.json
+-rw-r--r--   0        0        0    41658 2023-04-16 14:18:41.826841 mimesis-8.0.0/mimesis/data/en-au/person.json
+-rw-r--r--   0        0        0        2 2023-04-16 14:18:41.826841 mimesis-8.0.0/mimesis/data/en-au/text.json
+-rw-r--r--   0        0        0    24229 2023-04-16 14:18:41.826841 mimesis-8.0.0/mimesis/data/en-ca/address.json
+-rw-r--r--   0        0        0       49 2023-04-16 14:18:41.826841 mimesis-8.0.0/mimesis/data/en-ca/datetime.json
+-rw-r--r--   0        0        0     3053 2023-04-16 14:18:41.826841 mimesis-8.0.0/mimesis/data/en-ca/finance.json
+-rw-r--r--   0        0        0        2 2023-04-16 14:18:41.826841 mimesis-8.0.0/mimesis/data/en-ca/food.json
+-rw-r--r--   0        0        0    13729 2023-04-16 14:18:41.826841 mimesis-8.0.0/mimesis/data/en-ca/person.json
+-rw-r--r--   0        0        0        2 2023-04-16 14:18:41.826841 mimesis-8.0.0/mimesis/data/en-ca/text.json
+-rw-r--r--   0        0        0    84033 2023-04-16 14:18:41.830841 mimesis-8.0.0/mimesis/data/en-gb/address.json
+-rw-r--r--   0        0        0       49 2023-04-16 14:18:41.830841 mimesis-8.0.0/mimesis/data/en-gb/datetime.json
+-rw-r--r--   0        0        0     9072 2023-04-16 14:18:41.830841 mimesis-8.0.0/mimesis/data/en-gb/finance.json
+-rw-r--r--   0        0        0     1316 2023-04-16 14:18:41.830841 mimesis-8.0.0/mimesis/data/en-gb/food.json
+-rw-r--r--   0        0        0    45054 2023-04-16 14:18:41.830841 mimesis-8.0.0/mimesis/data/en-gb/person.json
+-rw-r--r--   0        0        0        2 2023-04-16 14:18:41.830841 mimesis-8.0.0/mimesis/data/en-gb/text.json
+-rw-r--r--   0        0        0    23805 2023-04-16 14:18:41.834841 mimesis-8.0.0/mimesis/data/es/address.json
+-rw-r--r--   0        0        0      561 2023-04-16 14:18:41.834841 mimesis-8.0.0/mimesis/data/es/datetime.json
+-rw-r--r--   0        0        0     2416 2023-04-16 14:18:41.834841 mimesis-8.0.0/mimesis/data/es/finance.json
+-rw-r--r--   0        0        0     4757 2023-04-16 14:18:41.834841 mimesis-8.0.0/mimesis/data/es/food.json
+-rw-r--r--   0        0        0    14143 2023-04-16 14:18:41.834841 mimesis-8.0.0/mimesis/data/es/person.json
+-rw-r--r--   0        0        0   128149 2023-04-16 14:18:41.838841 mimesis-8.0.0/mimesis/data/es/text.json
+-rw-r--r--   0        0        0    11619 2023-04-16 14:18:41.838841 mimesis-8.0.0/mimesis/data/es-mx/address.json
+-rw-r--r--   0        0        0        2 2023-04-16 14:18:41.838841 mimesis-8.0.0/mimesis/data/es-mx/datetime.json
+-rw-r--r--   0        0        0     2610 2023-04-16 14:18:41.838841 mimesis-8.0.0/mimesis/data/es-mx/finance.json
+-rw-r--r--   0        0        0     1081 2023-04-16 14:18:41.838841 mimesis-8.0.0/mimesis/data/es-mx/food.json
+-rw-r--r--   0        0        0    16998 2023-04-16 14:18:41.838841 mimesis-8.0.0/mimesis/data/es-mx/person.json
+-rw-r--r--   0        0        0        2 2023-04-16 14:18:41.838841 mimesis-8.0.0/mimesis/data/es-mx/text.json
+-rw-r--r--   0        0        0    21806 2023-04-16 14:18:41.838841 mimesis-8.0.0/mimesis/data/et/address.json
+-rw-r--r--   0        0        0      533 2023-04-16 14:18:41.838841 mimesis-8.0.0/mimesis/data/et/datetime.json
+-rw-r--r--   0        0        0     6635 2023-04-16 14:18:41.838841 mimesis-8.0.0/mimesis/data/et/finance.json
+-rw-r--r--   0        0        0     3683 2023-04-16 14:18:41.838841 mimesis-8.0.0/mimesis/data/et/food.json
+-rw-r--r--   0        0        0    33842 2023-04-16 14:18:41.842841 mimesis-8.0.0/mimesis/data/et/person.json
+-rw-r--r--   0        0        0    11545 2023-04-16 14:18:41.842841 mimesis-8.0.0/mimesis/data/et/text.json
+-rw-r--r--   0        0        0    13562 2023-04-16 14:18:41.842841 mimesis-8.0.0/mimesis/data/fa/address.json
+-rw-r--r--   0        0        0      665 2023-04-16 14:18:41.842841 mimesis-8.0.0/mimesis/data/fa/datetime.json
+-rw-r--r--   0        0        0     2589 2023-04-16 14:18:41.842841 mimesis-8.0.0/mimesis/data/fa/finance.json
+-rw-r--r--   0        0        0     6628 2023-04-16 14:18:41.842841 mimesis-8.0.0/mimesis/data/fa/food.json
+-rw-r--r--   0        0        0    56905 2023-04-16 14:18:41.846841 mimesis-8.0.0/mimesis/data/fa/person.json
+-rw-r--r--   0        0        0    11302 2023-04-16 14:18:41.846841 mimesis-8.0.0/mimesis/data/fa/text.json
+-rw-r--r--   0        0        0     5488 2023-04-16 14:18:41.846841 mimesis-8.0.0/mimesis/data/fi/address.json
+-rw-r--r--   0        0        0      542 2023-04-16 14:18:41.846841 mimesis-8.0.0/mimesis/data/fi/datetime.json
+-rw-r--r--   0        0        0     7886 2023-04-16 14:18:41.846841 mimesis-8.0.0/mimesis/data/fi/finance.json
+-rw-r--r--   0        0        0     3674 2023-04-16 14:18:41.846841 mimesis-8.0.0/mimesis/data/fi/food.json
+-rw-r--r--   0        0        0    26719 2023-04-16 14:18:41.846841 mimesis-8.0.0/mimesis/data/fi/person.json
+-rw-r--r--   0        0        0    57968 2023-04-16 14:18:41.850841 mimesis-8.0.0/mimesis/data/fi/text.json
+-rw-r--r--   0        0        0    39318 2023-04-16 14:18:41.850841 mimesis-8.0.0/mimesis/data/fr/address.json
+-rw-r--r--   0        0        0      529 2023-04-16 14:18:41.850841 mimesis-8.0.0/mimesis/data/fr/datetime.json
+-rw-r--r--   0        0        0     4390 2023-04-16 14:18:41.850841 mimesis-8.0.0/mimesis/data/fr/finance.json
+-rw-r--r--   0        0        0     7024 2023-04-16 14:18:41.850841 mimesis-8.0.0/mimesis/data/fr/food.json
+-rw-r--r--   0        0        0    46272 2023-04-16 14:18:41.854841 mimesis-8.0.0/mimesis/data/fr/person.json
+-rw-r--r--   0        0        0    37433 2023-04-16 14:18:41.854841 mimesis-8.0.0/mimesis/data/fr/text.json
+-rw-r--r--   0        0        0    13842 2023-04-16 14:18:41.854841 mimesis-8.0.0/mimesis/data/hu/address.json
+-rw-r--r--   0        0        0      515 2023-04-16 14:18:41.854841 mimesis-8.0.0/mimesis/data/hu/datetime.json
+-rw-r--r--   0        0        0      762 2023-04-16 14:18:41.854841 mimesis-8.0.0/mimesis/data/hu/finance.json
+-rw-r--r--   0        0        0     4302 2023-04-16 14:18:41.854841 mimesis-8.0.0/mimesis/data/hu/food.json
+-rw-r--r--   0        0        0    26944 2023-04-16 14:18:41.858841 mimesis-8.0.0/mimesis/data/hu/person.json
+-rw-r--r--   0        0        0    22876 2023-04-16 14:18:41.858841 mimesis-8.0.0/mimesis/data/hu/text.json
+-rw-r--r--   0        0        0      398 2023-04-16 14:18:20.050791 mimesis-8.0.0/mimesis/data/int/__init__.py
+-rw-r--r--   0        0        0    20986 2023-04-16 14:18:20.050791 mimesis-8.0.0/mimesis/data/int/address.py
+-rw-r--r--   0        0        0     2735 2023-04-16 14:18:20.050791 mimesis-8.0.0/mimesis/data/int/code.py
+-rw-r--r--   0        0        0     2223 2023-04-16 14:18:20.050791 mimesis-8.0.0/mimesis/data/int/common.py
+-rw-r--r--   0        0        0    27537 2023-04-16 14:18:20.050791 mimesis-8.0.0/mimesis/data/int/cryptographic.py
+-rw-r--r--   0        0        0    11625 2023-04-16 14:18:20.050791 mimesis-8.0.0/mimesis/data/int/datetime.py
+-rw-r--r--   0        0        0     7778 2023-04-16 14:18:20.050791 mimesis-8.0.0/mimesis/data/int/development.py
+-rw-r--r--   0        0        0    67892 2023-04-16 14:18:20.050791 mimesis-8.0.0/mimesis/data/int/file.py
+-rw-r--r--   0        0        0   264126 2023-04-16 14:18:20.050791 mimesis-8.0.0/mimesis/data/int/finance.py
+-rw-r--r--   0        0        0     5221 2023-04-16 14:18:20.050791 mimesis-8.0.0/mimesis/data/int/hardware.py
+-rw-r--r--   0        0        0    37473 2023-04-16 14:18:20.050791 mimesis-8.0.0/mimesis/data/int/internet.py
+-rw-r--r--   0        0        0      320 2023-04-16 14:18:20.050791 mimesis-8.0.0/mimesis/data/int/path.py
+-rw-r--r--   0        0        0      171 2023-04-16 14:18:20.050791 mimesis-8.0.0/mimesis/data/int/payment.py
+-rw-r--r--   0        0        0   140341 2023-04-16 14:18:20.050791 mimesis-8.0.0/mimesis/data/int/person.py
+-rw-r--r--   0        0        0      606 2023-04-16 14:18:20.050791 mimesis-8.0.0/mimesis/data/int/scientific.py
+-rw-r--r--   0        0        0      364 2023-04-16 14:18:20.050791 mimesis-8.0.0/mimesis/data/int/text.py
+-rw-r--r--   0        0        0    31498 2023-04-16 14:18:20.050791 mimesis-8.0.0/mimesis/data/int/transport.py
+-rw-r--r--   0        0        0   121675 2023-04-16 14:18:41.862841 mimesis-8.0.0/mimesis/data/is/address.json
+-rw-r--r--   0        0        0      546 2023-04-16 14:18:41.862841 mimesis-8.0.0/mimesis/data/is/datetime.json
+-rw-r--r--   0        0        0     1539 2023-04-16 14:18:41.862841 mimesis-8.0.0/mimesis/data/is/finance.json
+-rw-r--r--   0        0        0     1651 2023-04-16 14:18:41.862841 mimesis-8.0.0/mimesis/data/is/food.json
+-rw-r--r--   0        0        0    68768 2023-04-16 14:18:41.866841 mimesis-8.0.0/mimesis/data/is/person.json
+-rw-r--r--   0        0        0    51794 2023-04-16 14:18:41.866841 mimesis-8.0.0/mimesis/data/is/text.json
+-rw-r--r--   0        0        0   123349 2023-04-16 14:18:41.870841 mimesis-8.0.0/mimesis/data/it/address.json
+-rw-r--r--   0        0        0      142 2023-04-16 14:18:41.870841 mimesis-8.0.0/mimesis/data/it/builtin.json
+-rw-r--r--   0        0        0      535 2023-04-16 14:18:41.870841 mimesis-8.0.0/mimesis/data/it/datetime.json
+-rw-r--r--   0        0        0     5058 2023-04-16 14:18:41.870841 mimesis-8.0.0/mimesis/data/it/finance.json
+-rw-r--r--   0        0        0     5352 2023-04-16 14:18:41.870841 mimesis-8.0.0/mimesis/data/it/food.json
+-rw-r--r--   0        0        0    64650 2023-04-16 14:18:41.874841 mimesis-8.0.0/mimesis/data/it/person.json
+-rw-r--r--   0        0        0    77862 2023-04-16 14:18:41.874841 mimesis-8.0.0/mimesis/data/it/text.json
+-rw-r--r--   0        0        0    10631 2023-04-16 14:18:41.874841 mimesis-8.0.0/mimesis/data/ja/address.json
+-rw-r--r--   0        0        0      494 2023-04-16 14:18:41.874841 mimesis-8.0.0/mimesis/data/ja/datetime.json
+-rw-r--r--   0        0        0    23842 2023-04-16 14:18:41.874841 mimesis-8.0.0/mimesis/data/ja/finance.json
+-rw-r--r--   0        0        0    13902 2023-04-16 14:18:41.874841 mimesis-8.0.0/mimesis/data/ja/food.json
+-rw-r--r--   0        0        0    69460 2023-04-16 14:18:41.878841 mimesis-8.0.0/mimesis/data/ja/person.json
+-rw-r--r--   0        0        0    56672 2023-04-16 14:18:41.878841 mimesis-8.0.0/mimesis/data/ja/text.json
+-rw-r--r--   0        0        0    33301 2023-04-16 14:18:41.878841 mimesis-8.0.0/mimesis/data/kk/address.json
+-rw-r--r--   0        0        0      768 2023-04-16 14:18:41.878841 mimesis-8.0.0/mimesis/data/kk/datetime.json
+-rw-r--r--   0        0        0     6707 2023-04-16 14:18:41.878841 mimesis-8.0.0/mimesis/data/kk/finance.json
+-rw-r--r--   0        0        0       95 2023-04-16 14:18:41.882841 mimesis-8.0.0/mimesis/data/kk/food.json
+-rw-r--r--   0        0        0    28448 2023-04-16 14:18:41.882841 mimesis-8.0.0/mimesis/data/kk/person.json
+-rw-r--r--   0        0        0    14350 2023-04-16 14:18:41.882841 mimesis-8.0.0/mimesis/data/kk/text.json
+-rw-r--r--   0        0        0    30313 2023-04-16 14:18:41.882841 mimesis-8.0.0/mimesis/data/ko/address.json
+-rw-r--r--   0        0        0      492 2023-04-16 14:18:41.882841 mimesis-8.0.0/mimesis/data/ko/datetime.json
+-rw-r--r--   0        0        0    17722 2023-04-16 14:18:41.882841 mimesis-8.0.0/mimesis/data/ko/finance.json
+-rw-r--r--   0        0        0    12695 2023-04-16 14:18:41.882841 mimesis-8.0.0/mimesis/data/ko/food.json
+-rw-r--r--   0        0        0    39279 2023-04-16 14:18:41.886841 mimesis-8.0.0/mimesis/data/ko/person.json
+-rw-r--r--   0        0        0    68560 2023-04-16 14:18:41.886841 mimesis-8.0.0/mimesis/data/ko/text.json
+-rw-r--r--   0        0        0    60825 2023-04-16 14:18:41.890841 mimesis-8.0.0/mimesis/data/nl/address.json
+-rw-r--r--   0        0        0      507 2023-04-16 14:18:41.890841 mimesis-8.0.0/mimesis/data/nl/datetime.json
+-rw-r--r--   0        0        0     2771 2023-04-16 14:18:41.890841 mimesis-8.0.0/mimesis/data/nl/finance.json
+-rw-r--r--   0        0        0     7412 2023-04-16 14:18:41.890841 mimesis-8.0.0/mimesis/data/nl/food.json
+-rw-r--r--   0        0        0   109294 2023-04-16 14:18:41.894841 mimesis-8.0.0/mimesis/data/nl/person.json
+-rw-r--r--   0        0        0   202851 2023-04-16 14:18:41.898841 mimesis-8.0.0/mimesis/data/nl/text.json
+-rw-r--r--   0        0        0    53656 2023-04-16 14:18:41.898841 mimesis-8.0.0/mimesis/data/nl-be/address.json
+-rw-r--r--   0        0        0       31 2023-04-16 14:18:41.898841 mimesis-8.0.0/mimesis/data/nl-be/datetime.json
+-rw-r--r--   0        0        0     2303 2023-04-16 14:18:41.902841 mimesis-8.0.0/mimesis/data/nl-be/finance.json
+-rw-r--r--   0        0        0        2 2023-04-16 14:18:41.902841 mimesis-8.0.0/mimesis/data/nl-be/food.json
+-rw-r--r--   0        0        0     1371 2023-04-16 14:18:41.902841 mimesis-8.0.0/mimesis/data/nl-be/person.json
+-rw-r--r--   0        0        0        2 2023-04-16 14:18:41.902841 mimesis-8.0.0/mimesis/data/nl-be/text.json
+-rw-r--r--   0        0        0    40052 2023-04-16 14:18:41.902841 mimesis-8.0.0/mimesis/data/no/address.json
+-rw-r--r--   0        0        0      500 2023-04-16 14:18:41.902841 mimesis-8.0.0/mimesis/data/no/datetime.json
+-rw-r--r--   0        0        0     9731 2023-04-16 14:18:41.902841 mimesis-8.0.0/mimesis/data/no/finance.json
+-rw-r--r--   0        0        0     4479 2023-04-16 14:18:41.902841 mimesis-8.0.0/mimesis/data/no/food.json
+-rw-r--r--   0        0        0    43488 2023-04-16 14:18:41.902841 mimesis-8.0.0/mimesis/data/no/person.json
+-rw-r--r--   0        0        0    31334 2023-04-16 14:18:41.906841 mimesis-8.0.0/mimesis/data/no/text.json
+-rw-r--r--   0        0        0    80118 2023-04-16 14:18:41.906841 mimesis-8.0.0/mimesis/data/pl/address.json
+-rw-r--r--   0        0        0      567 2023-04-16 14:18:41.906841 mimesis-8.0.0/mimesis/data/pl/datetime.json
+-rw-r--r--   0        0        0    10830 2023-04-16 14:18:41.906841 mimesis-8.0.0/mimesis/data/pl/finance.json
+-rw-r--r--   0        0        0     4693 2023-04-16 14:18:41.910841 mimesis-8.0.0/mimesis/data/pl/food.json
+-rw-r--r--   0        0        0    27705 2023-04-16 14:18:41.910841 mimesis-8.0.0/mimesis/data/pl/person.json
+-rw-r--r--   0        0        0    65088 2023-04-16 14:18:41.910841 mimesis-8.0.0/mimesis/data/pl/text.json
+-rw-r--r--   0        0        0    19169 2023-04-16 14:18:41.914841 mimesis-8.0.0/mimesis/data/pt/address.json
+-rw-r--r--   0        0        0      563 2023-04-16 14:18:41.914841 mimesis-8.0.0/mimesis/data/pt/datetime.json
+-rw-r--r--   0        0        0     2572 2023-04-16 14:18:41.914841 mimesis-8.0.0/mimesis/data/pt/finance.json
+-rw-r--r--   0        0        0     4310 2023-04-16 14:18:41.914841 mimesis-8.0.0/mimesis/data/pt/food.json
+-rw-r--r--   0        0        0    38175 2023-04-16 14:18:41.914841 mimesis-8.0.0/mimesis/data/pt/person.json
+-rw-r--r--   0        0        0    25766 2023-04-16 14:18:41.914841 mimesis-8.0.0/mimesis/data/pt/text.json
+-rw-r--r--   0        0        0    94350 2023-04-16 14:18:41.918841 mimesis-8.0.0/mimesis/data/pt-br/address.json
+-rw-r--r--   0        0        0      564 2023-04-16 14:18:41.918841 mimesis-8.0.0/mimesis/data/pt-br/datetime.json
+-rw-r--r--   0        0        0    24208 2023-04-16 14:18:41.918841 mimesis-8.0.0/mimesis/data/pt-br/finance.json
+-rw-r--r--   0        0        0     3162 2023-04-16 14:18:41.918841 mimesis-8.0.0/mimesis/data/pt-br/food.json
+-rw-r--r--   0        0        0    63714 2023-04-16 14:18:41.922841 mimesis-8.0.0/mimesis/data/pt-br/person.json
+-rw-r--r--   0        0        0        2 2023-04-16 14:18:41.922841 mimesis-8.0.0/mimesis/data/pt-br/text.json
+-rw-r--r--   0        0        0   101129 2023-04-16 14:18:41.922841 mimesis-8.0.0/mimesis/data/ru/address.json
+-rw-r--r--   0        0        0    10949 2023-04-16 14:18:41.922841 mimesis-8.0.0/mimesis/data/ru/builtin.json
+-rw-r--r--   0        0        0      790 2023-04-16 14:18:41.922841 mimesis-8.0.0/mimesis/data/ru/datetime.json
+-rw-r--r--   0        0        0    22783 2023-04-16 14:18:41.922841 mimesis-8.0.0/mimesis/data/ru/finance.json
+-rw-r--r--   0        0        0    20262 2023-04-16 14:18:41.926841 mimesis-8.0.0/mimesis/data/ru/food.json
+-rw-r--r--   0        0        0    86369 2023-04-16 14:18:41.926841 mimesis-8.0.0/mimesis/data/ru/person.json
+-rw-r--r--   0        0        0    89215 2023-04-16 14:18:41.930841 mimesis-8.0.0/mimesis/data/ru/text.json
+-rw-r--r--   0        0        0    38882 2023-04-16 14:18:41.930841 mimesis-8.0.0/mimesis/data/sk/address.json
+-rw-r--r--   0        0        0      485 2023-04-16 14:18:41.930841 mimesis-8.0.0/mimesis/data/sk/datetime.json
+-rw-r--r--   0        0        0      816 2023-04-16 14:18:41.930841 mimesis-8.0.0/mimesis/data/sk/finance.json
+-rw-r--r--   0        0        0      284 2023-04-16 14:18:41.930841 mimesis-8.0.0/mimesis/data/sk/food.json
+-rw-r--r--   0        0        0     5828 2023-04-16 14:18:41.930841 mimesis-8.0.0/mimesis/data/sk/person.json
+-rw-r--r--   0        0        0      752 2023-04-16 14:18:41.930841 mimesis-8.0.0/mimesis/data/sk/text.json
+-rw-r--r--   0        0        0    97258 2023-04-16 14:18:41.934841 mimesis-8.0.0/mimesis/data/sv/address.json
+-rw-r--r--   0        0        0      508 2023-04-16 14:18:41.934841 mimesis-8.0.0/mimesis/data/sv/datetime.json
+-rw-r--r--   0        0        0     5035 2023-04-16 14:18:41.934841 mimesis-8.0.0/mimesis/data/sv/finance.json
+-rw-r--r--   0        0        0     6863 2023-04-16 14:18:41.934841 mimesis-8.0.0/mimesis/data/sv/food.json
+-rw-r--r--   0        0        0    32781 2023-04-16 14:18:41.934841 mimesis-8.0.0/mimesis/data/sv/person.json
+-rw-r--r--   0        0        0    41878 2023-04-16 14:18:41.938841 mimesis-8.0.0/mimesis/data/sv/text.json
+-rw-r--r--   0        0        0    12375 2023-04-16 14:18:41.938841 mimesis-8.0.0/mimesis/data/tr/address.json
+-rw-r--r--   0        0        0      508 2023-04-16 14:18:41.938841 mimesis-8.0.0/mimesis/data/tr/datetime.json
+-rw-r--r--   0        0        0    11988 2023-04-16 14:18:41.938841 mimesis-8.0.0/mimesis/data/tr/finance.json
+-rw-r--r--   0        0        0     1819 2023-04-16 14:18:41.938841 mimesis-8.0.0/mimesis/data/tr/food.json
+-rw-r--r--   0        0        0    29265 2023-04-16 14:18:41.938841 mimesis-8.0.0/mimesis/data/tr/person.json
+-rw-r--r--   0        0        0     8857 2023-04-16 14:18:41.938841 mimesis-8.0.0/mimesis/data/tr/text.json
+-rw-r--r--   0        0        0    54571 2023-04-16 14:18:41.942841 mimesis-8.0.0/mimesis/data/uk/address.json
+-rw-r--r--   0        0        0     6247 2023-04-16 14:18:41.942841 mimesis-8.0.0/mimesis/data/uk/builtin.json
+-rw-r--r--   0        0        0      790 2023-04-16 14:18:41.942841 mimesis-8.0.0/mimesis/data/uk/datetime.json
+-rw-r--r--   0        0        0     6981 2023-04-16 14:18:41.942841 mimesis-8.0.0/mimesis/data/uk/finance.json
+-rw-r--r--   0        0        0     9121 2023-04-16 14:18:41.942841 mimesis-8.0.0/mimesis/data/uk/food.json
+-rw-r--r--   0        0        0    52753 2023-04-16 14:18:41.942841 mimesis-8.0.0/mimesis/data/uk/person.json
+-rw-r--r--   0        0        0    21072 2023-04-16 14:18:41.942841 mimesis-8.0.0/mimesis/data/uk/text.json
+-rw-r--r--   0        0        0    10240 2023-04-16 14:18:41.942841 mimesis-8.0.0/mimesis/data/zh/address.json
+-rw-r--r--   0        0        0      539 2023-04-16 14:18:41.942841 mimesis-8.0.0/mimesis/data/zh/datetime.json
+-rw-r--r--   0        0        0     3604 2023-04-16 14:18:41.946841 mimesis-8.0.0/mimesis/data/zh/finance.json
+-rw-r--r--   0        0        0     2301 2023-04-16 14:18:41.946841 mimesis-8.0.0/mimesis/data/zh/food.json
+-rw-r--r--   0        0        0    96427 2023-04-16 14:18:41.946841 mimesis-8.0.0/mimesis/data/zh/person.json
+-rw-r--r--   0        0        0    17796 2023-04-16 14:18:41.946841 mimesis-8.0.0/mimesis/data/zh/text.json
+-rw-r--r--   0        0        0      377 2023-04-16 14:18:20.074791 mimesis-8.0.0/mimesis/entrypoints.py
+-rw-r--r--   0        0        0     6827 2023-04-16 14:18:20.074791 mimesis-8.0.0/mimesis/enums.py
+-rw-r--r--   0        0        0     1901 2023-04-16 14:18:20.074791 mimesis-8.0.0/mimesis/exceptions.py
+-rw-r--r--   0        0        0      507 2023-04-16 14:18:20.074791 mimesis-8.0.0/mimesis/locales.py
+-rw-r--r--   0        0        0     1450 2023-04-16 14:18:20.074791 mimesis-8.0.0/mimesis/providers/__init__.py
+-rw-r--r--   0        0        0     7754 2023-04-16 14:18:20.074791 mimesis-8.0.0/mimesis/providers/address.py
+-rw-r--r--   0        0        0     7676 2023-04-16 14:18:20.074791 mimesis-8.0.0/mimesis/providers/base.py
+-rw-r--r--   0        0        0     3058 2023-04-16 14:18:20.074791 mimesis-8.0.0/mimesis/providers/binaryfile.py
+-rw-r--r--   0        0        0     3190 2023-04-16 14:18:20.074791 mimesis-8.0.0/mimesis/providers/choice.py
+-rw-r--r--   0        0        0     2655 2023-04-16 14:18:20.074791 mimesis-8.0.0/mimesis/providers/code.py
+-rw-r--r--   0        0        0     3325 2023-04-16 14:18:20.074791 mimesis-8.0.0/mimesis/providers/cryptographic.py
+-rw-r--r--   0        0        0     8676 2023-04-16 14:18:20.074791 mimesis-8.0.0/mimesis/providers/date.py
+-rw-r--r--   0        0        0     2768 2023-04-16 14:18:20.074791 mimesis-8.0.0/mimesis/providers/development.py
+-rw-r--r--   0        0        0     2136 2023-04-16 14:18:20.074791 mimesis-8.0.0/mimesis/providers/file.py
+-rw-r--r--   0        0        0     3754 2023-04-16 14:18:20.074791 mimesis-8.0.0/mimesis/providers/finance.py
+-rw-r--r--   0        0        0     1712 2023-04-16 14:18:20.074791 mimesis-8.0.0/mimesis/providers/food.py
+-rw-r--r--   0        0        0     5534 2023-04-16 14:18:20.074791 mimesis-8.0.0/mimesis/providers/generic.py
+-rw-r--r--   0        0        0     3044 2023-04-16 14:18:20.074791 mimesis-8.0.0/mimesis/providers/hardware.py
+-rw-r--r--   0        0        0    15706 2023-04-16 14:18:20.074791 mimesis-8.0.0/mimesis/providers/internet.py
+-rw-r--r--   0        0        0     7042 2023-04-16 14:18:20.074791 mimesis-8.0.0/mimesis/providers/numeric.py
+-rw-r--r--   0        0        0     2746 2023-04-16 14:18:20.074791 mimesis-8.0.0/mimesis/providers/path.py
+-rw-r--r--   0        0        0     5199 2023-04-16 14:18:20.074791 mimesis-8.0.0/mimesis/providers/payment.py
+-rw-r--r--   0        0        0    13766 2023-04-16 14:18:20.074791 mimesis-8.0.0/mimesis/providers/person.py
+-rw-r--r--   0        0        0     2126 2023-04-16 14:18:20.074791 mimesis-8.0.0/mimesis/providers/science.py
+-rw-r--r--   0        0        0     4375 2023-04-16 14:18:20.074791 mimesis-8.0.0/mimesis/providers/text.py
+-rw-r--r--   0        0        0     1454 2023-04-16 14:18:20.074791 mimesis-8.0.0/mimesis/providers/transport.py
+-rw-r--r--   0        0        0        1 2023-04-16 14:18:20.074791 mimesis-8.0.0/mimesis/py.typed
+-rw-r--r--   0        0        0     4502 2023-04-16 14:18:20.074791 mimesis-8.0.0/mimesis/random.py
+-rw-r--r--   0        0        0    13900 2023-04-16 14:18:20.074791 mimesis-8.0.0/mimesis/schema.py
+-rw-r--r--   0        0        0     1373 2023-04-16 14:18:20.074791 mimesis-8.0.0/mimesis/shortcuts.py
+-rw-r--r--   0        0        0     1190 2023-04-16 14:18:20.074791 mimesis-8.0.0/mimesis/types.py
+-rw-r--r--   0        0        0     2748 2023-04-16 14:18:20.078791 mimesis-8.0.0/pyproject.toml
+-rw-r--r--   0        0        0     8588 1970-01-01 00:00:00.000000 mimesis-8.0.0/PKG-INFO
```

### Comparing `mimesis-7.1.0/LICENSE` & `mimesis-8.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/README.rst` & `mimesis-8.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/__init__.py` & `mimesis-8.0.0/mimesis/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     Path,
     Payment,
     Person,
     Science,
     Text,
     Transport,
 )
-from mimesis.schema import Field, Schema
+from mimesis.schema import Field, Fieldset, Schema
 
 __all__ = [
     "Address",
     "BaseDataProvider",
     "BaseProvider",
     "BinaryFile",
     "Finance",
@@ -79,14 +79,15 @@
     "Text",
     "Transport",
     "Cryptographic",
     # Has all:
     "Generic",
     # Schema:
     "Field",
+    "Fieldset",
     "Schema",
     # Locale:
     "Locale",
     # Enums:
     "Algorithm",
     "AudioFile",
     "CardType",
@@ -115,14 +116,14 @@
     "__description__",
     "__url__",
     "__author__",
     "__author_email__",
     "__license__",
 ]
 
-__version__ = "7.1.0"
+__version__ = "8.0.0"
 __title__ = "mimesis"
 __description__ = "Mimesis: Fake Data Generator."
 __url__ = "https://github.com/lk-geimfari/mimesis"
 __author__ = "Isaak Uchakaev (Likid Geimfari)"
 __author_email__ = "likid.geimfari@gmail.com"
 __license__ = "MIT License"
```

### Comparing `mimesis-7.1.0/mimesis/builtins/__init__.py` & `mimesis-8.0.0/mimesis/builtins/__init__.py`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/builtins/da.py` & `mimesis-8.0.0/mimesis/builtins/da.py`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/builtins/en.py` & `mimesis-8.0.0/mimesis/builtins/en.py`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/builtins/it.py` & `mimesis-8.0.0/mimesis/builtins/it.py`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/builtins/nl.py` & `mimesis-8.0.0/mimesis/builtins/nl.py`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/builtins/pl.py` & `mimesis-8.0.0/mimesis/builtins/pl.py`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/builtins/pt_br.py` & `mimesis-8.0.0/mimesis/builtins/pt_br.py`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/builtins/ru.py` & `mimesis-8.0.0/mimesis/builtins/ru.py`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/builtins/uk.py` & `mimesis-8.0.0/mimesis/builtins/uk.py`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/bin/sample.aac` & `mimesis-8.0.0/mimesis/data/bin/sample.aac`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/bin/sample.docx` & `mimesis-8.0.0/mimesis/data/bin/sample.docx`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/bin/sample.gif` & `mimesis-8.0.0/mimesis/data/bin/sample.gif`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/bin/sample.jpg` & `mimesis-8.0.0/mimesis/data/bin/sample.jpg`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/bin/sample.mov` & `mimesis-8.0.0/mimesis/data/bin/sample.mov`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/bin/sample.mp3` & `mimesis-8.0.0/mimesis/data/bin/sample.mp3`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/bin/sample.mp4` & `mimesis-8.0.0/mimesis/data/bin/sample.mp4`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/bin/sample.pdf` & `mimesis-8.0.0/mimesis/data/bin/sample.pdf`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/bin/sample.png` & `mimesis-8.0.0/mimesis/data/bin/sample.png`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/bin/sample.pptx` & `mimesis-8.0.0/mimesis/data/bin/sample.pptx`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/bin/sample.xlsx` & `mimesis-8.0.0/mimesis/data/bin/sample.xlsx`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/bin/sample.zip` & `mimesis-8.0.0/mimesis/data/bin/sample.zip`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/cs/address.json` & `mimesis-8.0.0/mimesis/data/cs/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/cs/datetime.json` & `mimesis-8.0.0/mimesis/data/cs/datetime.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/cs/food.json` & `mimesis-8.0.0/mimesis/data/cs/food.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/cs/person.json` & `mimesis-8.0.0/mimesis/data/cs/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/cs/text.json` & `mimesis-8.0.0/mimesis/data/cs/text.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/da/address.json` & `mimesis-8.0.0/mimesis/data/da/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/da/food.json` & `mimesis-8.0.0/mimesis/data/da/food.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/da/person.json` & `mimesis-8.0.0/mimesis/data/da/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/da/text.json` & `mimesis-8.0.0/mimesis/data/da/text.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/de/address.json` & `mimesis-8.0.0/mimesis/data/de/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/de/datetime.json` & `mimesis-8.0.0/mimesis/data/de/datetime.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/de/food.json` & `mimesis-8.0.0/mimesis/data/de/food.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/de/person.json` & `mimesis-8.0.0/mimesis/data/de/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/de/text.json` & `mimesis-8.0.0/mimesis/data/de/text.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/de-at/address.json` & `mimesis-8.0.0/mimesis/data/de-at/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/de-at/food.json` & `mimesis-8.0.0/mimesis/data/de-at/food.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/de-at/person.json` & `mimesis-8.0.0/mimesis/data/de-at/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/de-ch/address.json` & `mimesis-8.0.0/mimesis/data/de-ch/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/de-ch/person.json` & `mimesis-8.0.0/mimesis/data/de-ch/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/el/address.json` & `mimesis-8.0.0/mimesis/data/el/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/el/datetime.json` & `mimesis-8.0.0/mimesis/data/el/datetime.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/el/finance.json` & `mimesis-8.0.0/mimesis/data/el/finance.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6666666666666666%*

 * *Differences: {"'banks'": "['Αlpha Βank Α.Ε.', 'Eurobank Ergasias Α.Ε.', 'National Bank of Greece Α.Ε.', "*

 * *            "'Piraeus Bank Α.Ε.', 'Attica Bank Α.Ε.', 'Cooperative Bank of Chania Α.Ε.', "*

 * *            "'Cooperative Bank of Drama Α.Ε.', 'Cooperative Bank of Epirus Α.Ε.', 'Cooperative "*

 * *            "Bank of Evros Α.Ε.', 'Cooperative Bank of Karditsa Α.Ε.', 'Cooperative Bank of "*

 * *            "Kastoria Α.Ε.', 'Cooperative Bank of Kefalonia, Ithaca & Lefkada Α.Ε.', 'Cooperative "*

 * *            "Bank of Peloponnese Α.Ε. […]*

```diff
@@ -1,8 +1,28 @@
 {
+    "banks": [
+        "\u0391lpha \u0392ank \u0391.\u0395.",
+        "Eurobank Ergasias \u0391.\u0395.",
+        "National Bank of Greece \u0391.\u0395.",
+        "Piraeus Bank \u0391.\u0395.",
+        "Attica Bank \u0391.\u0395.",
+        "Cooperative Bank of Chania \u0391.\u0395.",
+        "Cooperative Bank of Drama \u0391.\u0395.",
+        "Cooperative Bank of Epirus \u0391.\u0395.",
+        "Cooperative Bank of Evros \u0391.\u0395.",
+        "Cooperative Bank of Karditsa \u0391.\u0395.",
+        "Cooperative Bank of Kastoria \u0391.\u0395.",
+        "Cooperative Bank of Kefalonia, Ithaca & Lefkada \u0391.\u0395.",
+        "Cooperative Bank of Peloponnese \u0391.\u0395.",
+        "Cooperative Bank of Pieria \u0391.\u0395.",
+        "Cooperative Bank of Serres \u0391.\u0395.",
+        "Cooperative Bank of Thessaly \u0391.\u0395.",
+        "Pancretan Cooperative Bank \u0391.\u0395.",
+        "Credicom Consumer Finance Bank \u0391.\u0395."
+    ],
     "company": {
         "name": [
             "ANEK Lines",
             "Alpha Bank",
             "Alumil S.A",
             "Attica Bank",
             "Eurobank",
```

### Comparing `mimesis-7.1.0/mimesis/data/el/food.json` & `mimesis-8.0.0/mimesis/data/el/food.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/el/person.json` & `mimesis-8.0.0/mimesis/data/el/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/el/text.json` & `mimesis-8.0.0/mimesis/data/el/text.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/en/address.json` & `mimesis-8.0.0/mimesis/data/en/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/en/finance.json` & `mimesis-8.0.0/mimesis/data/pt-br/finance.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.4761299046571324%*

 * *Differences: {"'banks'": "['Banco do Brasil S.A.', 'Itaú Unibanco Holding S.A.', 'Caixa Econômica Federal', "*

 * *            "'Banco Bradesco S.A.', 'Banco Santander S.A.', 'Banco Safra S.A.', 'Banco Votorantim "*

 * *            "S.A.', 'Banco BTG Pactual S.A.', 'Banco BMG S.A.', 'Banco Pan S.A.', 'Banco Inter "*

 * *            "S.A.', 'Banco ABC Brasil S.A.', 'Banco Original S.A.', 'Banco Topázio S.A.', 'Banco "*

 * *            "do Estado do Rio Grande do Sul S.A.', 'Banco Indusval S.A.', 'Banco Modal S.A.', "*

 * *            "'Banco Fib […]*

```diff
@@ -1,66 +1,91 @@
 {
+    "banks": [
+        "Banco do Brasil S.A.",
+        "Ita\u00fa Unibanco Holding S.A.",
+        "Caixa Econ\u00f4mica Federal",
+        "Banco Bradesco S.A.",
+        "Banco Santander S.A.",
+        "Banco Safra S.A.",
+        "Banco Votorantim S.A.",
+        "Banco BTG Pactual S.A.",
+        "Banco BMG S.A.",
+        "Banco Pan S.A.",
+        "Banco Inter S.A.",
+        "Banco ABC Brasil S.A.",
+        "Banco Original S.A.",
+        "Banco Top\u00e1zio S.A.",
+        "Banco do Estado do Rio Grande do Sul S.A.",
+        "Banco Indusval S.A.",
+        "Banco Modal S.A.",
+        "Banco Fibra S.A.",
+        "Banco Daycoval S.A.",
+        "Banco Renner S.A.",
+        "Banco C6 S.A.",
+        "Banco Tri\u00e2ngulo S.A.",
+        "Banco Cetelem S.A.",
+        "Banco do Estado de Sergipe S.A.",
+        "Banco Alfa S.A.",
+        "Banco Pine S.A.",
+        "Banco do Estado do Par\u00e1 S.A.",
+        "Banco do Nordeste do Brasil S.A.",
+        "Banco do Estado do Esp\u00edrito Santo S.A.",
+        "Banco Rendimento S.A."
+    ],
     "company": {
         "name": [
-            "Infinity Investment Plan",
             "A Plus Lawn Care",
             "A+ Electronics",
             "A+ Investments",
-            "ABM Industries",
-            "ABX Air",
-            "AC Lens",
-            "ACCO Brands",
-            "ACN Inc.",
-            "ADC Telecommunications",
-            "AECOM",
-            "AES Corporation",
-            "AGCO",
-            "AGL Resources",
-            "AK Steel Holding",
-            "AMC Entertainment",
-            "AMETEK",
-            "AMR Corporation",
-            "AND1",
-            "AOL",
-            "ASARCO",
-            "AT&T",
-            "AVST",
+            "a21",
             "Aaron's, Inc.",
             "Abbott Laboratories",
             "Abercrombie & Fitch",
+            "ABM Industries",
+            "ABX Air",
+            "AC Lens",
             "Access Asia",
+            "ACCO Brands",
             "Accord Investments",
             "Accuquote",
             "Ace Hardware",
+            "Acesita\tA\u00e7o",
             "Acme Brick Company",
+            "ACN Inc.",
             "Activision Blizzard",
             "Acuity Brands",
             "Acuserv",
             "Adapt",
             "Adaptabiz",
             "Adaptas",
             "Adaptaz",
             "Adaptec",
+            "ADC Telecommunications",
             "Adobe Systems Inc.",
             "Advance Auto Parts",
             "Advanced Micro Devices",
-            "Advanced Micro Devices",
             "Advanced Processing & Imaging",
             "Advansed Teksyztems",
+            "AECOM",
+            "AES Corporation",
             "Aetna",
             "Affiliated Computer Services",
             "Affinity Investment Group",
             "Afforda",
             "Afforda Merchant Services",
             "Aflac",
+            "AGCO",
             "Agilent Technologies",
+            "AGL Resources",
+            "Agrale",
             "Agriprocessors",
             "Air Products & Chemicals",
-            "AirTran Holdings",
             "Airgas",
+            "AirTran Holdings",
+            "AK Steel Holding",
             "Alaska Air Group",
             "Albemarle Corporation",
             "Albertsons LLC",
             "Alcoa",
             "Aleris International",
             "Alert Alarm Company",
             "Alexander & Baldwin",
@@ -75,15 +100,18 @@
             "Alliant Techsystems",
             "Allstate",
             "Aloha Airlines",
             "Altec Lansing",
             "Altria Group",
             "Always",
             "Amazon.com",
+            "AmBev",
+            "AMC Entertainment",
             "Ameren",
+            "Am\u00e9rica Latina Log\u00edstica",
             "America Online",
             "American Airlines",
             "American Apparel",
             "American Axle",
             "American Broadcasting Company",
             "American Eagle Outfitters",
             "American Electric Power",
@@ -93,99 +121,119 @@
             "American Greetings",
             "American Home Mortgage",
             "American International Group",
             "American Reprographics Company",
             "Amerigroup",
             "Ameriprise Financial",
             "AmerisourceBergen",
+            "AMETEK",
             "Amgen",
+            "Amil\tSeguro\tAMIL3\t Rio de Janeiro",
             "Amkor Technology",
             "Amphenol Corporation",
+            "Ampla\tUtilit\u00e1rios",
+            "AMR Corporation",
             "Amtrak",
             "Amy's Kitchen",
-            "AnaSpec",
             "Anadarko Petroleum Corporation",
             "Analog Devices",
+            "AnaSpec",
             "Anchor Bay Entertainment",
+            "AND1",
+            "Andrade Gutierrez",
             "Anixter International",
             "Ann Taylor",
             "Antec",
+            "AOL",
             "Aon Corporation",
             "Apache Software Foundation",
             "Apollo Group",
             "Apple Inc.",
             "Applebee's",
             "Applied Biosystems",
             "Applied Industrial Technologies",
             "Applied Materials",
             "Aramark",
             "Arbitron",
             "Arch Coal",
             "Archer Daniels Midland",
             "Architectural Genie",
             "Arctic Cat",
+            "Arezzo",
             "Ariba",
             "Arizona Stock Exchange",
             "Arkeia Software",
             "Armstrong World Industries",
             "Arrow Electronics",
             "Arryx",
             "ArvinMeritor",
+            "ASARCO",
             "Asbury Automotive Group",
             "Ashland Inc.",
             "Asian Answers",
             "Asian Fusion",
             "Asian Junction",
             "Asian Plan",
             "Asian Solutions",
             "Asiatic Solutions",
             "AskMeNow",
             "Aspyr Media",
             "Assurant",
+            "AT&T",
             "Atari",
             "Atlas Architectural Designs",
             "Atlas Realty",
             "Atmos Energy",
             "Audiovox",
             "Auto-Owners Insurance",
-            "AutoNation",
-            "AutoZone",
+            "AutoBAn",
             "Autodesk",
             "Autoliv",
             "Automatic Data Processing",
+            "AutoNation",
+            "AutoZone",
             "Avant Garde Appraisal",
             "Avant Garde Appraisal Group",
             "Avant Garde Interior Designs",
             "Avaya",
             "Avery Dennison",
+            "Avianca Brasil",
+            "Avibr\u00e1s\tAeroespacial",
             "Avis Budget Group",
             "Avnet",
             "Avon Products",
+            "AVST",
             "Awthentikz",
+            "Azaleia\tVestu\u00e1rio",
+            "Azul Linhas A\u00e9reas Brasileiras",
             "A\u00e9ropostale",
             "B/E Aerospace",
-            "BB&T Corporation",
-            "BFG Technologies",
-            "BJ Services Company",
-            "BJ's Wholesale Club",
-            "BMC Software",
-            "BNSF Railway",
+            "B2W Varejo",
             "Babcock and Wilcox",
             "Back To Basics Chiropractic Clinic",
             "Bain & Company",
             "Bain Capital",
             "Baker Hughes",
             "Balanced Fortune",
             "Baldor Electric Company",
             "Ball Corp.",
+            "Banco BMG",
+            "Banco Bradesco",
+            "Banco do Brasil",
+            "Banco Mercantil do Brasil",
+            "Banco Safra",
+            "Banestes",
             "Bank of America",
             "Bank of New York Mellon",
+            "Banpar\u00e1",
+            "Banrisul",
             "Barnes & Noble",
             "Bath & Body Works",
             "Baxter International",
+            "BB&T Corporation",
             "Bealls",
             "BearingPoint",
             "Beasts of Beauty",
             "Beazer Homes USA",
             "Bebo",
             "Bechtel",
             "Beckman Coulter",
@@ -200,143 +248,177 @@
             "Benchmark Electronics",
             "Benesome",
             "Berkshire Hathaway",
             "Berry Plastics",
             "Best Biz Survis",
             "Best Buy",
             "Better Business Ideas and Services",
+            "BFG Technologies",
             "Big Lots",
             "Biggby Coffee",
             "Bio-Rad Laboratories",
             "Biomet",
             "Birdwell",
+            "BJ Services Company",
+            "BJ's Wholesale Club",
             "Black & Decker",
             "BlackRock",
             "Blockbuster Inc.",
             "BlueLinx Holdings",
             "Blyth, Inc.",
+            "BM&F",
+            "BMC Software",
+            "BNSF Railway",
             "Bob Evans Restaurants",
+            "Bob's\tRestaurantes",
             "Body Fate",
             "Body Toning",
             "Boeing",
             "Boise Cascade",
             "Bold Ideas",
+            "Bombril\tProdutos",
+            "Bompre\u00e7o",
             "Bonanza Produce Stores",
             "Borders Group",
             "BorgWarner",
             "Bosch Brewing Company",
             "Bose Corporation",
             "Boston Acoustics",
             "Boston Scientific",
             "Bountiful Harvest Health Food Store",
             "Boyd Gaming",
+            "Bradespar\tServi\u00e7os banc\u00e1rios",
             "Bradley Pharmaceuticals",
+            "Brasil Foods",
+            "Brasil Telecom",
+            "Braskem\tEnergia",
+            "Bravox",
             "Briggs & Stratton",
             "Brightpoint",
             "Brilliant Home Designs",
             "Brinker International",
             "Brinks",
             "Bristol-Myers Squibb",
+            "Brit\u00e2nia",
             "Broadcom",
             "Brookdale Senior Living",
             "Brown-Forman Corporation",
             "Brunswick Corporation",
+            "BTG Pactual",
             "Bucyrus International",
             "Buena Vista Garden Maintenance",
             "Buena Vista Realty Service",
             "Burger King Holdings",
             "Burlington Coat Factory",
             "Bushmaster Firearms International",
+            "Busscar",
             "Butler America",
             "C.H. Robinson Worldwide",
             "CA, Inc.",
-            "CBS Corporation",
-            "CDI Corporation",
-            "CIGNA",
-            "CKE Restaurants",
-            "CNA",
-            "CNET",
-            "CVS Pharmacy",
+            "Caixa Econ\u00f4mica Federal",
+            "Cal\u00e7ados Beira-Rio",
             "Calista Corporation",
             "Calpine",
+            "Camargo Correa",
             "Capital One",
             "Capitalcorp",
             "Carnival Corporation & plc",
             "Carnival Cruise Lines",
             "Cartoon Network Studios",
             "Casco Bay Lines",
             "Castle Realty",
             "Caterpillar Inc.",
+            "CBS Corporation",
+            "CCR",
+            "CDI Corporation",
+            "CEB",
+            "CEG",
+            "Celesc",
+            "CELG",
+            "CEMIG",
             "Cerner Corporation",
+            "CESP",
             "Chargepal",
             "Chem-Dry",
             "Chevron",
             "ChexSystems",
             "Chicago Bridge & Iron Company",
             "Choices",
             "Chrysler",
             "Chugach Alaska Corporation",
+            "Cielo",
+            "CIGNA",
             "Circuit Design",
             "Cisco Systems, Inc.",
             "Citigroup",
             "Citrix",
+            "CKE Restaurants",
             "Clear Channel Communications",
+            "CNA",
+            "CNET",
             "Cogent Communications",
             "Cognizant Technology Solutions",
             "Cole Haan",
             "Colgate-Palmolive",
             "Colt Defense",
             "Colt's Manufacturing Company",
             "Columbia Pictures",
             "Columbia Sussex",
             "Comcast",
+            "Comg\u00e1s",
             "Comodo",
+            "Companhia Sider\u00fargica Nacional",
+            "Companhia Zaffari",
             "Complete Tech",
             "ConocoPhillips",
             "Conseco",
             "Continental Airlines",
             "Control Data Corporation",
             "Convergys Corp.",
             "Converse",
             "CoolTouch Monitors",
+            "Copacol",
+            "Copel",
             "Copeland's",
             "Corinthian Designs",
             "Corning Incorporated",
             "Corpbay",
             "Corsair Memory",
+            "Cosan\tPetroqu\u00edmicos",
             "Costco",
             "Cougar Investment",
             "Coventry Health Care",
+            "CPFL",
             "Crazy Eddie",
             "Crazy Tiger",
             "Creative Wealth",
             "Creative Wealth Management",
             "Crowley Maritime Corporation",
             "Custom Lawn Care",
             "Custom Lawn Service",
             "Cut Above",
             "Cut Rite",
             "Cut Rite Lawn Care",
-            "DC Comics",
-            "DC Shoes",
-            "DISH Network",
-            "DRS Technologies",
-            "DST Systems",
-            "DTE Energy",
-            "DaVita",
+            "CVS Pharmacy",
+            "Cyrela Brazil Realty",
+            "Dafra",
             "Danaher",
             "Darden Restaurants",
             "Datacorp",
+            "DaVita",
+            "DC Comics",
+            "DC Shoes",
             "Dean Foods",
             "Deere & Company",
             "Del Monte Foods",
             "Dell, Inc.",
             "Delphi",
             "Delta Air Lines",
             "Dereon",
+            "DERSA",
             "Desert Garden Help",
             "Destiny Planners",
             "Destiny Realty",
             "Destiny Realty Solutions",
             "Devon Energy",
             "Dex One",
             "DiC Entertainment",
@@ -345,351 +427,416 @@
             "Digi-Key",
             "Dillard's",
             "DineEquity",
             "Dippin' Dots",
             "DirecTV",
             "Discover Financial Services",
             "Discovery Communications",
+            "DISH Network",
             "DivX, Inc.",
+            "DocDigital",
             "Doculabs",
             "Dole Foods",
             "Dollar General",
             "Dollar Tree",
             "Dominion Resources",
             "Domtar",
             "Dover Corporation",
             "Dow Chemical Company",
             "Dow Jones & Company",
             "Dr Pepper Snapple Group",
             "Dream Home Improvements",
             "Dream Home Real Estate Service",
             "Dreamscape Garden Care",
             "Dresser Inc.",
-            "DuPont",
+            "Drogasil",
+            "DRS Technologies",
+            "DST Systems",
+            "DTE Energy",
             "Duke Energy",
             "Dun & Bradstreet",
             "Dun Rite Lawn Care",
             "Dun Rite Lawn Maintenance",
-            "DynCorp International",
+            "DuPont",
+            "Duratex",
+            "Dynamine",
             "Dynatronics Accessories",
+            "DynCorp International",
             "Dynegy",
             "E-zhe Source",
-            "EMC Corporation",
             "Earthworks Garden Kare",
             "Earthworks Yard Maintenance",
             "Eastman Chemical Company",
             "Eastman Kodak",
+            "eBay",
+            "EBX",
             "Ecolab",
             "Eddie Bauer",
             "Eden Lawn Service",
             "Edge Garden Services",
             "Edge Yard Service",
             "Ejecta",
             "El Paso Corp.",
             "Electric Boat",
             "Electronic Arts",
             "Electronic Data Systems",
             "Electronic Geek",
             "Electronics Source",
+            "Eletrobras",
+            "Eletrobr\u00e1s",
+            "Eletrosul",
             "Eli Lilly and Company",
             "Elizabeth Arden",
+            "Embraco",
+            "Embraer\tAeroespacial",
+            "Embratel",
+            "EMC Corporation",
             "Emcor",
             "Emerson Electric Company",
             "Emerson Radio",
             "Energizer Holdings",
             "Energy East",
             "Enrich Garden Services",
             "Enterasys Networks",
             "Entergy",
             "Enterprise GP Holdings",
             "Enviro Architectural Designs",
-            "EnviroSource Design",
             "Environ Architectural Design",
+            "EnviroSource Design",
             "Envirotecture Design",
             "Envirotecture Design Service",
             "Equifax",
             "Erie Insurance Group",
             "Ernod",
             "Esselte",
+            "Estrela\tBrinquedos",
             "Est\u00e9e Lauder Companies",
             "Eureka",
             "Exact Realty",
             "Exact Solutions",
             "Excella",
             "Exelon Corporation",
             "Expeditors International",
             "Express Merchant Service",
             "Express Scripts Incorporated",
             "ExxonMobil",
+            "Fabral",
             "Fabrik Inc.",
+            "facebook",
             "Fairchild Semiconductor",
             "Farnod",
-            "FedEx",
             "Federal Home Loan Mortgage Corporation",
             "Federal National Mortgage Association",
+            "FedEx",
             "Fellowship Investments",
             "Fender Musical Instruments Corporation",
+            "Fibria",
             "Fidelity Investments",
             "FileMaker Inc., formerly Claris Corp.",
             "Fireball",
             "Firestone Tire and Rubber Company",
             "First Choice Garden Maintenance",
             "First Choice Yard Help",
             "First Hawaiian Bank",
             "First Rate Choice",
             "Fiserv",
             "Fisher Electronics",
             "Fisker Automotive",
             "Fit Tonic",
+            "Fleury S.A.",
             "Flexus",
             "Fluor Corp",
             "Ford Motor Company",
             "Formula Gray",
             "Formula Grey",
             "Forum Communications",
             "Four Leaf Clover",
             "Fox Film Corporation",
             "Fragrant Flower Lawn Services",
             "Frasca International",
             "Fred Meyer, Inc.",
-            "FreeWave Technologies",
             "Freedom Map",
+            "FreeWave Technologies",
             "Fresh Start",
             "Fresh&Easy Neighbourhood Market",
             "Friendly Advice",
             "Friendly Interior Design",
             "Frontier Airlines",
             "Fruit of the Loom",
             "Full Color",
             "Future Bright",
             "Future Plan",
-            "GE Consumer & Industrial",
-            "GEICO",
-            "GHD Inc.",
-            "GTECH",
+            "Gafisa",
             "Galaxy Man",
             "Gamma Gas",
             "Gamma Grays",
             "Gamma Realty",
             "Gap",
             "Garden Guru",
             "Garden Master",
             "Garmin",
+            "Garoto",
             "Gartner",
             "Gas Depot",
             "Gas Legion",
             "Gas Zone",
             "Gateway Computers",
             "Gatorade",
+            "GE Consumer & Industrial",
+            "GEICO",
             "Gemini Sound Products",
             "General Communication",
             "General Dynamics",
             "General Electric",
             "General Mills",
             "General Motors",
             "Gentiva Health Services",
             "Georgia Pacific",
+            "Gerax",
+            "Gerdau",
+            "GHD Inc.",
             "Giant Food",
             "Gibson Guitar Corporation",
             "Gillette",
             "Global Insight",
             "Go Daddy",
+            "Gol Transportes A\u00e9reos",
             "Gold Leaf Garden Management",
             "Gold Touch",
+            "Golden Cross",
             "Golden Joy",
             "Goldman Sachs",
             "Good Times",
             "Goodrich Corporation",
             "Goodyear Tire and Rubber Company",
             "Google",
             "Gore-Tex",
             "Grade A Investment",
+            "Gradiente",
             "Grass Roots Yard Services",
+            "Grendene",
             "Grey Fade",
             "Greyvoid",
             "Ground Round",
             "Group O",
             "Growmark",
-            "H&R Block",
+            "Grupo Abril",
+            "Grupo EXBR",
+            "Grupo Folha",
+            "Grupo Globo",
+            "Grupo Guararapes",
+            "Grupo P\u00e3o de A\u00e7\u00facar",
+            "Grupo RBS\tMidia",
+            "Grupo Schincariol",
+            "GTECH",
+            "GVT\tTelecomunica\u00e7\u00f5es",
             "H-E-B",
             "H. J. Heinz Company",
+            "H&R Block",
+            "Habib's",
             "Halliburton",
             "Hallmark Cards",
             "Happy Bear Investment",
             "Happy Family",
             "Hardee's",
             "Harley-Davidson",
             "Harman International Industries",
             "Hasbro",
             "Hastings Entertainment",
             "Hawaiian Airlines",
+            "Helibr\u00e1s",
             "Helios Air",
             "Helping Hand",
+            "Hering",
             "Hewlett-Packard",
             "Hi-Point Firearms",
             "Hilton Hotels Corporation",
             "Home City Ice Co.",
             "Home Depot",
             "Honest Air Group",
             "Honeywell",
             "Hornbeck Offshore Services",
             "Hot Topic",
+            "Hoteis Othon",
             "Houchens Industries",
             "Houlihan's",
             "House of Gas",
             "Hoyden",
+            "Huge Networks\tUtilit\u00e1rios",
             "Human Kinetics",
             "Hunt Petroleum",
             "Hyland Software",
-            "ION Media Networks",
+            "Hypermarcas",
+            "i-flex Solutions",
             "Idea Infinity",
             "Ideal Garden Maintenance",
             "Ideal Garden Management",
             "Ideal Industries",
             "Imation",
             "Incluesiv",
             "Independent Investors",
             "Independent Wealth Management",
             "Indiewealth",
             "Infinite Wealth",
             "Infinite Wealth Planners",
+            "Infinity Investment Plan",
             "Infor",
             "Informix",
+            "Infraero",
+            "Insinuante",
             "Integra Design",
             "Integra Investment Plan",
             "Integra Investment Service",
             "Integra Wealth",
             "Integra Wealth Planners",
             "Intel",
             "Intelacard",
+            "Intelbras\tTecnologia",
             "Intelli Wealth Group",
             "Intercontinental Manufacturing Company",
-            "International Business Machines",
-            "IBM",
-            "International Game Technology",
-            "IGT",
+            "International Business Machines (IBM)",
+            "International Game Technology (IGT)",
             "International Paper",
             "Interplay Entertainment",
             "Interstate Batteries",
             "Intuit",
+            "Iochpe-Maxion",
+            "ION Media Networks",
+            "iRobot",
             "Iron Mountain",
+            "Itaro\tAutomotivo",
+            "Ita\u00fa Unibanco",
+            "Ita\u00fasa",
+            "Itautec",
             "J. C. Penny",
             "J. P. Morgan Chase and Co.",
-            "JCPenney",
-            "JL Audio",
-            "JN-International Medical Corporation",
             "Jack in the Box",
             "Jackhammer Technologies",
             "Jackpot Consultant",
             "Jarden",
+            "JBS S.A.",
+            "JCPenney",
             "JetBlue Airways",
             "Jimmy John's",
+            "JL Audio",
+            "JN-International Medical Corporation",
             "Johnson & Johnson",
             "Johnson Controls",
             "Jones Soda Co.",
             "Journal Communications",
             "Just For Fun",
             "KBR",
-            "KFC",
-            "KPMG",
             "Kellogg Company",
             "Kenexa Corporation",
             "Kenworth",
+            "Kepler Weber",
             "Kerr-McGee",
+            "KFC",
             "Kimberly-Clark",
             "Kingston Technology",
+            "Klabin",
             "Klipsch Audio Technologies",
             "Kmart",
             "Knockout Kickboxing",
             "Koch Industries",
             "Kohler Company",
             "Komerci",
             "Konsili",
+            "KPMG",
             "Kraft Foods",
             "Kroger",
             "Kurzweil Educational Systems",
-            "L&L Hawaiian Barbecue",
             "L.L.Bean",
+            "L&L Hawaiian Barbecue",
             "Landskip Yard Care",
             "Landskip Yard Service",
             "Las Vegas Yard Management",
             "Laserfiche",
             "Lawn N' Order Garden Care",
             "Lawnscape Garden Maintenance",
             "Lazysize",
             "LeapFrog Enterprises",
             "Lee",
+            "Leil\u00e3o dos Girass\u00f3is",
             "Lennox International",
             "Lexmark",
             "Libera",
             "Liberty Wealth Planner",
             "Liberty Wealth Planners",
             "Life Map",
             "Life Map Planners",
             "Life Plan Counselling",
             "Life's Gold",
+            "Light\tUtilit\u00e1rios",
             "Limited Brands",
             "LinkedIn",
             "Listen Up",
             "Liz Claiborne",
             "Local Matters",
+            "Localiza",
             "Lockheed Martin",
             "Locost Accessories",
+            "Lojas Americanas",
+            "Lojas Amor de Anjo",
+            "Lojas Riachuelo",
             "Lone Wolf Wealth Planning",
             "Louisiana Pacific",
             "Lowe's",
             "Lucas Oil",
             "Lucasfilm",
             "Lumencraft",
-            "MCI Inc.",
-            "MTX Audio",
+            "M. Dias Branco",
             "Macro Design",
             "Macroserve",
             "Magik Gray",
             "Magik Grey",
             "Magik Lamp",
             "Magna Architectural Design",
-            "Magna Architectural Design",
             "Magna Consulting",
             "Magna Gases",
             "Magna Solution",
             "Magna Wealth",
             "MagnaSolution",
             "Magnavox",
             "ManCharm",
             "ManPower",
             "Manu Connection",
             "Marantz",
             "Marathon Oil",
+            "Marcopolo",
             "Marriott Corporation",
             "Mars Incorporated",
             "Marsh & McLennan",
             "Marshall Pottery",
             "Martel Communication",
             "Martha Stewart Living Omnimedia",
             "Martin Marietta Materials",
             "Master Builder Design Services",
             "MasterCard",
             "Matrix Architectural Service",
-            "Matrix Architectural Service",
             "Matrix Design",
             "Matrix Interior Design",
             "Mattel",
             "Mauna Loa Macadamia Nut Corp.",
             "Maxaprofit",
             "Maxi-Tech",
             "Maxiserve",
             "Maxtor Corporation",
             "McConn & Company",
+            "MCI Inc.",
             "Medimix International",
             "MegaSolutions",
             "Megatronic",
             "Megatronic Mux",
+            "Megatube",
             "Memorec",
+            "Mendes J\u00fanior\tConstru\u00e7\u00e3o",
             "Merrymaking",
+            "Metaltex",
+            "Metr\u00f4 Rio",
             "Microcat",
             "Midway Games",
             "Midwest Communications",
             "Mikro Designs",
             "Mikrotechnic",
             "Millenia Life",
             "Miller Brewing",
@@ -710,102 +857,115 @@
             "Monlinks",
             "Monmax",
             "Monsanto Company",
             "Monsource",
             "Morgan Stanley",
             "Motorola",
             "Mozilla Foundation",
+            "MRS Log\u00edstica S.A.",
+            "MRV Engenharia",
+            "MTX Audio",
             "Multi Tech Development",
             "Multi-Systems Merchant Services",
             "Multicerv",
             "Muscle Factory",
             "Musco Lighting",
             "Mutual of Omaha",
             "Myspace",
-            "NBC Universal",
-            "NCR Corporation",
             "Nabisco",
+            "Nacional Soft Ltda",
             "National Railway Equipment Company",
             "Nationwide Insurance",
+            "Natura",
             "Naturohair",
-            "NetApp",
-            "NetDNA",
-            "NetZero",
+            "NBC Universal",
+            "NCR Corporation",
+            "Net",
             "Netaid",
+            "NetApp",
             "Netcom Business Services",
             "Netcordia",
             "Netcore",
+            "NetDNA",
             "Netgear",
             "Netobill",
             "Netstars Matrix Design",
             "Network Air",
+            "NetZero",
             "New Balance",
             "New Era Tickets",
             "New World",
             "New World Realty",
             "Newhair",
             "News Corporation",
             "Nike",
+            "NKF Acess\u00f3rios",
             "Nordstrom",
             "Nortax",
             "Northern Star",
             "Northrop Grumman",
             "Northwest Airlines",
             "Novell",
             "Novellus Systems",
             "Numark",
             "Nutri G",
             "Nvidia",
+            "O Botic\u00e1rio",
             "O'Reilly",
-            "OCZ Technology",
-            "ONEOK",
-            "OPOWER",
-            "OSI Restaurant Partners",
             "Oberweis Dairy",
             "Ocean Spray",
+            "OCZ Technology",
+            "Odebrecht\tConstru\u00e7\u00e3o",
             "Office Depot",
             "Office Max",
+            "Oi\tTelecomunica\u00e7\u00f5es",
             "Olan Mills, Inc.",
             "Omni Architectural Designs",
             "Omni Group",
             "Omni Realty",
             "Omni Source",
             "Omni Tech",
             "Omni Tech Solutions",
             "Omnicare",
             "One-Up Realtors",
             "One-Up Realty",
+            "ONEOK",
             "Onvia",
             "Open Interface",
             "OpenMarket Inc.",
+            "OPOWER",
             "Opti-Tek",
             "Opticomp",
             "Oracle Corporation",
             "Oreck Corporation",
             "Orion",
+            "OSI Restaurant Partners",
             "Overcast Media",
             "PACCAR",
-            "PC Power and Cooling",
-            "Pacific Gas & Electric Company",
-            "PG&E",
+            "Pacific Gas & Electric Company (PG&E)",
             "PalmOne, Inc.",
             "PalmSource, Inc.",
+            "Panapan\u00e1 Bijuterias",
+            "Pantanal Linhas A\u00e9reas",
             "Pantone",
             "Papa John's Pizza",
             "Parallel Px",
             "Paramount Pictures",
             "Parts and Pieces",
             "Paxton Media Group",
             "Payless ShoeSource",
+            "PC Power and Cooling",
             "Pearl Architectural Design",
             "PepsiCo",
             "Perdue Farms",
             "Perisolution",
             "Personal & Corporate Design",
             "Peterbilt",
+            "Petrobras",
+            "Petr\u00f3leo Ipiranga",
             "Pfizer",
             "Pier 1 Imports",
             "Pilgrim's Pride",
             "Pinnacle Systems",
             "Pizza Hut",
             "Plan Future",
             "Plan Smart",
@@ -815,14 +975,15 @@
             "Platinum Interior Design",
             "Plochman's",
             "Pluto Marine",
             "Pointers",
             "Polaris Industries",
             "Polaroid Corporation",
             "Popeyes Chicken & Biscuits",
+            "Positivo Inform\u00e1tica",
             "Powerbod",
             "Practi-Plan",
             "Practi-Plan Mapping",
             "Prahject Planner",
             "Precision Castparts Corporation",
             "Prestiga-Biz",
             "Prestigabiz",
@@ -837,85 +998,91 @@
             "Procter & Gamble",
             "Profitpros",
             "Progressive Corporation",
             "Prospa-Pal",
             "Protean",
             "Publix",
             "QCR Holdings",
-            "QVC",
             "Qpass",
             "Qualcomm",
             "Quality Event Planner",
             "Quality Merchant Services",
             "Quality Realty Service",
             "Quanta Services",
             "Quantrix",
+            "Queiroz Galv\u00e3o",
             "Quest Software",
             "Quest Technology Service",
-            "QuickTrip",
             "Quickbiz",
+            "QuickTrip",
             "Quincy Newspapers",
             "Quiznos",
+            "QVC",
             "Qwest",
             "R. R. Donnelley & Sons",
-            "RCA",
             "RadioShack",
             "Rainbow Life",
             "Rayovac",
             "Raytheon",
+            "RCA",
             "Realty Depot",
             "Realty Solution",
             "Realty Zone",
             "Red Bears Tavern",
             "Red Fox Tavern",
             "Red Hat",
             "Red River Broadcasting",
+            "Rede Globo",
+            "Rede Record",
+            "Redecard",
+            "RedeTV!",
             "Regis Corporation",
             "Reliable Garden Management",
             "Reliable Guidance",
             "Reliable Investments",
             "Rent-A-Wreck",
             "Renys",
             "Respironics, Inc.",
+            "Ricardo Eletro",
             "Rich and Happy",
             "Rite Aid Corporation",
             "Rite Solution",
             "Rivera Property Maintenance",
             "Riverdeep",
             "Road Runner Lawn Services",
             "Rockford Fosgate",
             "Rockstar Games",
             "Rockwell Automation",
             "Rockwell Collins",
             "Rollins Inc.",
             "Romp",
+            "Rossi Residencial",
             "Royal Caribbean International",
             "Royal Gas",
             "Russell Investment Group",
             "Russell Stovers",
             "Ryder System, Inc.",
             "S3 Graphics",
-            "SBC Communications",
-            "STX",
             "Safeco Corporation",
             "Safeway Inc.",
             "Salary.com",
             "Salem Communications",
             "SanDisk",
             "Sauer-Danfoss",
+            "SBC Communications",
+            "Scherm\tTecnologia",
             "Schoep's Ice Cream",
-            "Science Applications International Corporation",
-            "SAIC",
+            "Science Applications International Corporation (SAIC)",
             "Seagate Technology",
             "Sears",
             "Seattle's Best Coffee",
             "Seksi Ladi",
             "Seksi Lady",
             "Sequoia Voting Systems",
-            "Service Corporation International",
+            "Service Corporation International (SCI)",
             "Sexsi Senorita",
             "Sexy Babe",
             "Shirokiya",
             "Shure Incorporated",
             "Signa Air",
             "Silicon Graphics",
             "Silicon Image",
@@ -963,40 +1130,46 @@
             "Stratapro",
             "Strategic Profit",
             "Strategy Consulting",
             "Strategy Planner",
             "Strength Gurus",
             "Strong Life",
             "Strongbod",
+            "STX",
             "Suadela Investment",
             "Subway",
             "Success Is Yours",
             "Sun Microsystems, Inc.",
             "Sunburst Garden Management",
             "Sunny Delight Beverages",
             "Sunny Real Estate Investments",
             "Sunoco",
+            "Super G\u00e1s Br\u00e1s",
             "Superior Appraisals",
             "Superior Interior Design",
             "Supervalu",
             "Sur La Table",
             "Symantec",
             "Syntel",
             "System Star",
             "System Star Solutions",
-            "THQ",
             "Taco Tico",
             "Take-Two Interactive",
+            "TAM Airlines",
             "Tanadgusix Corporation",
             "Target Corporation",
             "Target Realty",
             "Target Source",
+            "Taurus\tArmas de fogo",
             "Team Designers and Associates",
             "Team Uno",
             "Techo Solutions",
+            "Tectoy\tBrinquedos",
+            "Telequartz\tMinera\u00e7\u00e3o",
+            "Telesp\tTelecomunica\u00e7\u00f5es",
             "Tempur-Pedic",
             "Terra",
             "Terra Nova Garden Services",
             "Tesla Motors",
             "Tesoro",
             "Testor Corporation",
             "Texas Instruments",
@@ -1009,108 +1182,121 @@
             "The Happy Bear",
             "The Hertz Corporation",
             "The High Heelers",
             "The Independent Planners",
             "The Jolly Farmer",
             "The Lawn Guru",
             "The Liberty Corporation",
-            "TLC",
+            "The Library Corporation (TLC)",
             "The Network Chef",
             "The Pink Pig Tavern",
             "The Polka Dot Bear Tavern",
             "The Serendipity Dip",
             "The Spotted Cougar",
             "The Vanguard Group",
             "The Walt Disney Company",
             "The Weinstein Company",
             "The White Rabbit",
             "The White Swan",
+            "THQ",
+            "TIM\tTelecomunica\u00e7\u00f5es",
             "Time Warner Cable",
             "Titania",
+            "Total Linhas A\u00e9reas",
             "Total Network Development",
             "Total Quality",
             "Total Serve",
             "Total Sources",
             "Total Yard Maintenance",
             "Total Yard Management",
             "Towers Perrin",
             "TransDigm Group",
+            "Transmiss\u00e3o Paulista\tUtilit\u00e1rios",
             "Transocean",
             "Trinity Industries Inc.",
+            "TRIP Linhas A\u00e9reas",
             "Triumph Group",
+            "Troller",
             "Tropicana Products",
             "Tully's Coffee",
             "Tupperware Brands Corporation",
+            "TV Cultura",
             "Twitter",
             "U.S. Robotics",
             "U.S. Steel",
-            "US Airways",
-            "US Cellular",
-            "UTStarcom",
             "Ubu Productions",
             "Ultimate Software",
+            "Ultrapar\tEnergia",
             "Under Armour",
-            "Union Oil Company of California",
+            "Union Oil Company of California (Unocal)",
             "Union Pacific Railroad",
             "Unisys",
             "United Airlines",
-            "United Parcel Service",
-            "UPS",
+            "United Parcel Service (UPS)",
             "United Services Automobile Association",
             "United Technologies",
             "Universal Design Partners",
             "Universal Studios",
+            "Universo Online",
             "Universo Realtors",
+            "US Airways",
+            "US Cellular",
+            "Usiminas",
+            "UTStarcom",
             "Uwajimaya",
-            "VECO Corporation",
-            "VF Corporation",
-            "VIZ Media",
-            "VMware",
+            "Vale\tMinera\u00e7\u00e3o",
             "Valero Energy Corporation",
             "Vantec",
             "Vari-Tec",
             "Vaughan & Bushnell Manufacturing",
+            "VECO Corporation",
             "Vectren",
             "Venus Swimwear",
             "Veramons",
             "Verbatim Corporation",
             "Verizon",
             "Verizon Wireless",
             "Vermeer Industries",
             "Vertex Pharmaceuticals",
+            "VF Corporation",
             "Viacom",
             "Vibrant Man",
             "Victoria's Secret",
             "ViewSonic",
             "Visa Inc.",
             "Vistikon",
-            "VitaGrey",
             "Vitagee",
+            "VitaGrey",
             "Vitamax Health Food Center",
             "Vivitar",
+            "Vivo\tTelecomunica\u00e7\u00f5es",
+            "VIZ Media",
             "Vizio",
+            "VMware",
             "Vocera Communications",
             "VonMaur",
+            "Votorantim",
             "Vulcan Corporation",
             "W. L. Gore & Associates",
             "W. R. Berkley",
             "W. R. Grace and Company",
             "W.C. Bradley Co.",
-            "WWE",
-            "WWW Realty",
             "Wahl Clipper",
             "Walgreens",
             "Walmart",
             "Walt Disney Company",
             "Warner Bros. Entertainment",
             "Washburn Guitars",
             "Watco Companies",
+            "Water Pumps\tCom\u00e9rcio de bombas industriais",
             "Wealth Zone Group",
             "Wealthy Ideas",
             "Webcom Business Services",
+            "WebJet Linhas A\u00e9reas",
+            "WEG Ind\u00fastrias",
             "Welch's",
             "WellPoint",
             "Wells Fargo Bank, N.A.",
             "Wendy's/Arby's Group",
             "Werner Enterprises",
             "West Liberty Foods",
             "Westat",
@@ -1123,55 +1309,55 @@
             "Winnebago Industries",
             "Wise Appraisals",
             "Wise Solutions",
             "Wizards of the Coast",
             "World Airways",
             "World Financial Group",
             "World of Fun",
+            "WWE",
+            "WWW Realty",
             "Wynn Resorts",
-            "XPAC",
-            "XPLANE",
             "Xerox",
             "Xilinx",
+            "XPAC",
+            "XPLANE",
             "Xray Eye & Vision Clinics",
+            "Yahoo!",
             "YASH Technologies",
             "YRC Worldwide Inc.",
-            "Yahoo!",
             "Yum! Brands, Inc.",
-            "ZOMM, LLC",
             "Zapata",
             "Zappos.com",
             "Zaxby's",
             "Zenith Electronics",
             "Zephyr Investments",
             "Zig Zag Children Clothes",
+            "ZOMM, LLC",
             "Zoo York",
             "Zoom Technologies",
-            "Zune",
-            "eBay",
-            "Facebook"
+            "Zune"
         ],
         "type": {
             "abbr": [
                 "Corp.",
                 "Inc.",
                 "Ltd.",
-                "LLLP",
+                "EIRELI",
                 "LLP",
                 "LP",
                 "PLLC",
                 "P.C"
             ],
             "title": [
-                "Corporation",
-                "Incorporated",
-                "Limited Liability Company",
-                "Limited Liability Limited Partnership",
-                "Limited Liability Partnership",
-                "Limited Partnership",
-                "Professional Limited Liability Company",
-                "Professional corporation"
+                "Corpora\u00e7\u00e3o",
+                "Incorpora\u00e7\u00e3o",
+                "Sociedade Limitada",
+                "Empresa Individual de Resposabilidade Limitada",
+                "Empresa Individual",
+                "Parceria Limitada",
+                "Sociedade Simples",
+                "Corpora\u00e7\u00e3o Profissional"
             ]
         }
     },
-    "currency-code": "USD"
+    "currency-code": "BRL"
 }
```

### Comparing `mimesis-7.1.0/mimesis/data/en/food.json` & `mimesis-8.0.0/mimesis/data/en/food.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/en/person.json` & `mimesis-8.0.0/mimesis/data/en/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/en/text.json` & `mimesis-8.0.0/mimesis/data/en/text.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/en-au/address.json` & `mimesis-8.0.0/mimesis/data/en-au/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/en-au/finance.json` & `mimesis-8.0.0/mimesis/data/en-au/finance.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6666666666666666%*

 * *Differences: {"'banks'": "['Australia and New Zealand Banking Group Limited', 'Commonwealth Bank of Australia', "*

 * *            "'National Australia Bank Limited', 'Westpac Banking Corporation', 'Macquarie Bank "*

 * *            "Limited', 'Bendigo and Adelaide Bank Limited', 'Bank of Queensland Limited', "*

 * *            "'Suncorp-Metway Limited', 'ING Bank Limited', 'Bank of Western Australia Limited', "*

 * *            "'Bank of South Australia Limited', 'Adelaide Bank Limited', 'Bank of Melbourne "*

 * *            "Limited', 'Bank o […]*

```diff
@@ -1,8 +1,73 @@
 {
+    "banks": [
+        "Australia and New Zealand Banking Group Limited",
+        "Commonwealth Bank of Australia",
+        "National Australia Bank Limited",
+        "Westpac Banking Corporation",
+        "Macquarie Bank Limited",
+        "Bendigo and Adelaide Bank Limited",
+        "Bank of Queensland Limited",
+        "Suncorp-Metway Limited",
+        "ING Bank Limited",
+        "Bank of Western Australia Limited",
+        "Bank of South Australia Limited",
+        "Adelaide Bank Limited",
+        "Bank of Melbourne Limited",
+        "Bank of Cyprus Australia Pty Limited",
+        "Bank of China (Australia) Limited",
+        "Bank of Sydney Ltd",
+        "Auswide Bank Ltd",
+        "AWA Alliance Bank",
+        "Bank Australia",
+        "Bank of Heritage Isle",
+        "Bank of us",
+        "Beyond Bank Australia Limited",
+        "Central Murray Credit Union Ltd",
+        "Community First Credit Union Limited",
+        "CUA",
+        "Defence Bank Limited",
+        "Endeavour Mutual Bank Limited",
+        "Family First Credit Union Ltd",
+        "Firefighters Mutual Bank",
+        "First Choice Credit Union",
+        "G&C Mutual Bank",
+        "Gateway Bank",
+        "Heritage Bank Limited",
+        "Horizon Bank",
+        "Hume Bank Limited",
+        "Illawarra Credit Union Limited",
+        "IMB Ltd",
+        "Laboratories Credit Union Ltd",
+        "Macquarie Credit Union Limited",
+        "Maitland Mutual Building Society Ltd",
+        "MyState Bank Limited",
+        "Northern Beaches Credit Union Ltd",
+        "Northern Inland Credit Union Limited",
+        "P&N Bank",
+        "People's Choice Credit Union",
+        "Police Credit Union Limited",
+        "Police Bank Ltd",
+        "QT Mutual Bank Limited",
+        "Queensland Country Credit Union Ltd",
+        "Regional Australia Bank",
+        "Select Encompass Credit Union Limited",
+        "South West Slopes Credit Union Limited",
+        "Southern Cross Credit Union Ltd",
+        "Summerland Credit Union Ltd",
+        "Teachers Mutual Bank Limited",
+        "The Capricornian Ltd",
+        "The Mac Credit Union Co-operative Ltd",
+        "The Mutual Bank",
+        "The Rock Building Society Ltd",
+        "Unity Bank Limited",
+        "WAW Credit Union Co-operative Limited",
+        "Warwick Credit Union Ltd",
+        "Woolworths Employees' Credit Union Limited"
+    ],
     "company": {
         "name": [
             "MOQ LIMITED",
             "1-PAGE LIMITED",
             "1300 SMILES LIMITED",
             "1ST GROUP LIMITED",
             "333D LIMITED",
```

### Comparing `mimesis-7.1.0/mimesis/data/en-au/person.json` & `mimesis-8.0.0/mimesis/data/en-au/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/en-ca/address.json` & `mimesis-8.0.0/mimesis/data/en-ca/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/en-ca/finance.json` & `mimesis-8.0.0/mimesis/data/en-ca/finance.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6666666666666666%*

 * *Differences: {"'banks'": "['Bank of Montreal', 'Bank of Nova Scotia', 'Canadian Imperial Bank of Commerce', "*

 * *            "'Royal Bank of Canada', 'Toronto-Dominion Bank', 'National Bank of Canada']"}*

```diff
@@ -1,8 +1,16 @@
 {
+    "banks": [
+        "Bank of Montreal",
+        "Bank of Nova Scotia",
+        "Canadian Imperial Bank of Commerce",
+        "Royal Bank of Canada",
+        "Toronto-Dominion Bank",
+        "National Bank of Canada"
+    ],
     "company": {
         "name": [
             "ATI technologies",
             "AVI Sound International",
             "Addition Elle",
             "Advance Gold",
             "Advanced Cyclotron Systems",
```

### Comparing `mimesis-7.1.0/mimesis/data/en-ca/person.json` & `mimesis-8.0.0/mimesis/data/en-ca/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/en-gb/address.json` & `mimesis-8.0.0/mimesis/data/en-gb/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/en-gb/food.json` & `mimesis-8.0.0/mimesis/data/en-gb/food.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/en-gb/person.json` & `mimesis-8.0.0/mimesis/data/en-gb/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/es/address.json` & `mimesis-8.0.0/mimesis/data/es/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/es/datetime.json` & `mimesis-8.0.0/mimesis/data/es/datetime.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/es/finance.json` & `mimesis-8.0.0/mimesis/data/es/finance.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6666666666666666%*

 * *Differences: {"'banks'": "['Banco Santander, S.A.', 'Banco Bilbao Vizcaya Argentaria, S.A.', 'CaixaBank, S.A.', "*

 * *            "'Banco Sabadell, S.A.', 'Bankinter, S.A.', 'Banco Popular Español, S.A.', 'Unicaja "*

 * *            "Banco, S.A.', 'Ibercaja Banco, S.A.', 'Abanca Corporación Bancaria, S.A.', "*

 * *            "'Kutxabank, S.A.', 'Banco Mare Nostrum, S.A.', 'Liberbank, S.A.', 'Banco Cooperativo "*

 * *            "Español, S.A.', 'Caja Rural de Navarra, S.C.C.', 'Caja Rural del Sur, S.C.C.', 'Banco "*

 * *            "Mediolanu […]*

```diff
@@ -1,8 +1,30 @@
 {
+    "banks": [
+        "Banco Santander, S.A.",
+        "Banco Bilbao Vizcaya Argentaria, S.A.",
+        "CaixaBank, S.A.",
+        "Banco Sabadell, S.A.",
+        "Bankinter, S.A.",
+        "Banco Popular Espa\u00f1ol, S.A.",
+        "Unicaja Banco, S.A.",
+        "Ibercaja Banco, S.A.",
+        "Abanca Corporaci\u00f3n Bancaria, S.A.",
+        "Kutxabank, S.A.",
+        "Banco Mare Nostrum, S.A.",
+        "Liberbank, S.A.",
+        "Banco Cooperativo Espa\u00f1ol, S.A.",
+        "Caja Rural de Navarra, S.C.C.",
+        "Caja Rural del Sur, S.C.C.",
+        "Banco Mediolanum, S.A.",
+        "Caja Rural Central, S.C.C.",
+        "Banca March, S.A.",
+        "Caja de Cr\u00e9dito de los Ingenieros, S.C.C.",
+        "Caja Laboral Popular, Coop. de Cr\u00e9dito"
+    ],
     "company": {
         "name": [
             "3scale",
             "ASTANO",
             "Abengoa",
             "Abertis",
             "Acciona",
```

### Comparing `mimesis-7.1.0/mimesis/data/es/food.json` & `mimesis-8.0.0/mimesis/data/es/food.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/es/person.json` & `mimesis-8.0.0/mimesis/data/es/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/es/text.json` & `mimesis-8.0.0/mimesis/data/es/text.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/es-mx/address.json` & `mimesis-8.0.0/mimesis/data/es-mx/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/es-mx/finance.json` & `mimesis-8.0.0/mimesis/data/es-mx/finance.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6666666666666666%*

 * *Differences: {"'banks'": "['BBVA Bancomer', 'Grupo Financiero Banorte', 'Santander México', 'Citibanamex', "*

 * *            "'HSBC México', 'Scotiabank México', 'Inbursa', 'Banco Azteca', 'Afirme Grupo "*

 * *            "Financiero', 'Invex Grupo Financiero']"}*

```diff
@@ -1,8 +1,20 @@
 {
+    "banks": [
+        "BBVA Bancomer",
+        "Grupo Financiero Banorte",
+        "Santander M\u00e9xico",
+        "Citibanamex",
+        "HSBC M\u00e9xico",
+        "Scotiabank M\u00e9xico",
+        "Inbursa",
+        "Banco Azteca",
+        "Afirme Grupo Financiero",
+        "Invex Grupo Financiero"
+    ],
     "company": {
         "name": [
             "ALFA",
             "AeroUnion",
             "Aeromexpress",
             "Aerom\u00e9xico",
             "Aerom\u00e9xico Connect",
```

### Comparing `mimesis-7.1.0/mimesis/data/es-mx/food.json` & `mimesis-8.0.0/mimesis/data/es-mx/food.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/es-mx/person.json` & `mimesis-8.0.0/mimesis/data/es-mx/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/et/address.json` & `mimesis-8.0.0/mimesis/data/et/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/et/datetime.json` & `mimesis-8.0.0/mimesis/data/et/datetime.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/et/finance.json` & `mimesis-8.0.0/mimesis/data/et/finance.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6666666666666666%*

 * *Differences: {"'banks'": "['Swedbank AS', 'SEB Pank AS', 'LHV Pank AS', 'Luminor Bank AS', 'Coop Pank AS', "*

 * *            "'Citadele Banka Eesti Filiaal', 'Bigbank AS', 'Versobank AS', 'Inbank AS', 'Eesti "*

 * *            "Krediidipank AS', 'Tallinna Äripank AS', 'Tartu Hoiu-laenuühistu', 'MTÜ Eesti "*

 * *            "Ühistupank']"}*

```diff
@@ -1,8 +1,23 @@
 {
+    "banks": [
+        "Swedbank AS",
+        "SEB Pank AS",
+        "LHV Pank AS",
+        "Luminor Bank AS",
+        "Coop Pank AS",
+        "Citadele Banka Eesti Filiaal",
+        "Bigbank AS",
+        "Versobank AS",
+        "Inbank AS",
+        "Eesti Krediidipank AS",
+        "Tallinna \u00c4ripank AS",
+        "Tartu Hoiu-laenu\u00fchistu",
+        "MT\u00dc Eesti \u00dchistupank"
+    ],
     "company": {
         "name": [
             "A.L.A.R.A.",
             "A. Le Coq Group",
             "A. T\u00f5nisson & Ko",
             "ABB AS",
             "Abja Linavabrik",
```

### Comparing `mimesis-7.1.0/mimesis/data/et/food.json` & `mimesis-8.0.0/mimesis/data/et/food.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/et/person.json` & `mimesis-8.0.0/mimesis/data/et/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/et/text.json` & `mimesis-8.0.0/mimesis/data/et/text.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/fa/address.json` & `mimesis-8.0.0/mimesis/data/fa/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/fa/datetime.json` & `mimesis-8.0.0/mimesis/data/fa/datetime.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/fa/finance.json` & `mimesis-8.0.0/mimesis/data/fa/finance.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6666666666666666%*

 * *Differences: {"'banks'": "['Bank Melli Iran', 'Bank Mellat', 'Bank Saderat Iran', 'Export Development Bank of "*

 * *            "Iran', 'Bank Pasargad', 'Karafarin Bank', 'Eghtesad Novin Bank', 'EN Bank', 'Tejarat "*

 * *            "Bank', 'Parsian Bank']"}*

```diff
@@ -1,8 +1,20 @@
 {
+    "banks": [
+        "Bank Melli Iran",
+        "Bank Mellat",
+        "Bank Saderat Iran",
+        "Export Development Bank of Iran",
+        "Bank Pasargad",
+        "Karafarin Bank",
+        "Eghtesad Novin Bank",
+        "EN Bank",
+        "Tejarat Bank",
+        "Parsian Bank"
+    ],
     "company": {
         "name": [
             "\u0634\u0631\u06a9\u062a \u0645\u0644\u06cc \u0646\u0641\u062a \u0627\u06cc\u0631\u0627\u0646",
             "\u0645\u0639\u0627\u062f\u0646 \u0627\u06cc\u0631\u0627\u0646",
             "\u0633\u0627\u0632\u0645\u0627\u0646 \u0646\u0648\u0633\u0627\u0632\u06cc ",
             "\u0627\u06cc\u0631\u0627\u0646 \u062e\u0648\u062f\u0631\u0648",
             "\u0627\u0645\u06cc\u062f\u0627\u0646 \u062a\u062c\u0627\u0631\u062a \u06a9\u06cc\u0634 ",
```

### Comparing `mimesis-7.1.0/mimesis/data/fa/food.json` & `mimesis-8.0.0/mimesis/data/fa/food.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/fa/person.json` & `mimesis-8.0.0/mimesis/data/fa/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/fa/text.json` & `mimesis-8.0.0/mimesis/data/fa/text.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/fi/address.json` & `mimesis-8.0.0/mimesis/data/fi/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/fi/datetime.json` & `mimesis-8.0.0/mimesis/data/fi/datetime.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/fi/finance.json` & `mimesis-8.0.0/mimesis/data/fi/finance.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6666666666666666%*

 * *Differences: {"'banks'": "['Aktia Bank plc', 'Danske Bank plc', 'Handelsbanken', 'Nordea Bank', 'Oma "*

 * *            "Säästöpankki', 'OP Financial Group', 'POP Bank Group', 'S-Bank', 'Ålandsbanken']"}*

```diff
@@ -1,8 +1,19 @@
 {
+    "banks": [
+        "Aktia Bank plc",
+        "Danske Bank plc",
+        "Handelsbanken",
+        "Nordea Bank",
+        "Oma S\u00e4\u00e4st\u00f6pankki",
+        "OP Financial Group",
+        "POP Bank Group",
+        "S-Bank",
+        "\u00c5landsbanken"
+    ],
     "company": {
         "name": [
             "9lives",
             "A-insin\u00f6\u00f6rit",
             "A-katsastus",
             "A. honko",
             "Aalto university executive education",
```

### Comparing `mimesis-7.1.0/mimesis/data/fi/food.json` & `mimesis-8.0.0/mimesis/data/fi/food.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/fi/person.json` & `mimesis-8.0.0/mimesis/data/fi/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/fi/text.json` & `mimesis-8.0.0/mimesis/data/fi/text.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/fr/address.json` & `mimesis-8.0.0/mimesis/data/fr/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/fr/datetime.json` & `mimesis-8.0.0/mimesis/data/fr/datetime.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/fr/food.json` & `mimesis-8.0.0/mimesis/data/fr/food.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/fr/person.json` & `mimesis-8.0.0/mimesis/data/fr/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/fr/text.json` & `mimesis-8.0.0/mimesis/data/fr/text.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/hu/address.json` & `mimesis-8.0.0/mimesis/data/hu/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/hu/datetime.json` & `mimesis-8.0.0/mimesis/data/hu/datetime.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/hu/food.json` & `mimesis-8.0.0/mimesis/data/hu/food.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/hu/person.json` & `mimesis-8.0.0/mimesis/data/hu/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/hu/text.json` & `mimesis-8.0.0/mimesis/data/hu/text.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/int/address.py` & `mimesis-8.0.0/mimesis/data/int/address.py`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/int/code.py` & `mimesis-8.0.0/mimesis/data/int/code.py`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/int/common.py` & `mimesis-8.0.0/mimesis/data/int/common.py`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/int/cryptographic.py` & `mimesis-8.0.0/mimesis/data/int/cryptographic.py`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/int/datetime.py` & `mimesis-8.0.0/mimesis/data/int/datetime.py`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/int/development.py` & `mimesis-8.0.0/mimesis/data/int/development.py`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/int/file.py` & `mimesis-8.0.0/mimesis/data/int/file.py`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/int/finance.py` & `mimesis-8.0.0/mimesis/data/int/finance.py`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/int/hardware.py` & `mimesis-8.0.0/mimesis/data/int/hardware.py`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/int/internet.py` & `mimesis-8.0.0/mimesis/data/int/internet.py`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/int/person.py` & `mimesis-8.0.0/mimesis/data/int/person.py`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/int/scientific.py` & `mimesis-8.0.0/mimesis/data/int/scientific.py`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/int/transport.py` & `mimesis-8.0.0/mimesis/data/int/transport.py`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/is/address.json` & `mimesis-8.0.0/mimesis/data/is/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/is/datetime.json` & `mimesis-8.0.0/mimesis/data/is/datetime.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/is/finance.json` & `mimesis-8.0.0/mimesis/data/is/finance.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6666666666666666%*

 * *Differences: {"'banks'": "['Arion Banki hf.', 'Islandsbanki hf.', 'Landsbankinn hf.']"}*

```diff
@@ -1,8 +1,13 @@
 {
+    "banks": [
+        "Arion Banki hf.",
+        "Islandsbanki hf.",
+        "Landsbankinn hf."
+    ],
     "company": {
         "name": [
             "365 - mi\u00f0lar",
             "Actavis Group",
             "Advania",
             "Arctic Trucks \u00cdsland",
             "Bakkav\u00f6r Group",
```

### Comparing `mimesis-7.1.0/mimesis/data/is/food.json` & `mimesis-8.0.0/mimesis/data/is/food.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/is/person.json` & `mimesis-8.0.0/mimesis/data/is/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/is/text.json` & `mimesis-8.0.0/mimesis/data/is/text.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/it/address.json` & `mimesis-8.0.0/mimesis/data/it/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/it/datetime.json` & `mimesis-8.0.0/mimesis/data/it/datetime.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/it/finance.json` & `mimesis-8.0.0/mimesis/data/it/finance.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6666666666666666%*

 * *Differences: {"'banks'": "['Intesa Sanpaolo S.p.A.', 'Unicredit S.p.A.', 'Credito Emiliano S.p.A.', 'Banco BPM "*

 * *            "S.p.A.', 'Credito Valtellinese S.C.', 'Banca di Credito Cooperativo di Roma Scrl', "*

 * *            "'Banca Monte dei Paschi di Siena S.p.A.', 'Banca Popolare di Sondrio S.C.p.A.', "*

 * *            "'Banca Sella Holding S.p.A.', 'Banca del Piemonte S.p.A.', 'Banco di Sardegna "*

 * *            "S.p.A.', 'Banco Popolare Società Cooperativa', 'BPER Banca S.p.A.', 'Cariparma "*

 * *            'S.p.A.\', "Cassa Ce […]*

```diff
@@ -1,8 +1,30 @@
 {
+    "banks": [
+        "Intesa Sanpaolo S.p.A.",
+        "Unicredit S.p.A.",
+        "Credito Emiliano S.p.A.",
+        "Banco BPM S.p.A.",
+        "Credito Valtellinese S.C.",
+        "Banca di Credito Cooperativo di Roma Scrl",
+        "Banca Monte dei Paschi di Siena S.p.A.",
+        "Banca Popolare di Sondrio S.C.p.A.",
+        "Banca Sella Holding S.p.A.",
+        "Banca del Piemonte S.p.A.",
+        "Banco di Sardegna S.p.A.",
+        "Banco Popolare Societ\u00e0 Cooperativa",
+        "BPER Banca S.p.A.",
+        "Cariparma S.p.A.",
+        "Cassa Centrale Raiffeisen dell'Alto Adige",
+        "Cassa di Risparmio di Bolzano S.p.A.",
+        "Cassa di Risparmio di Bra S.p.A.",
+        "Cassa di Risparmio di Cesena S.p.A.",
+        "Cassa di Risparmio di Fermo S.p.A.",
+        "Cassa di Risparmio di Ferrara S.p.A."
+    ],
     "company": {
         "name": [
             "55dsl",
             "ALAN",
             "Abici",
             "Air Dolomiti",
             "Air Italy",
```

### Comparing `mimesis-7.1.0/mimesis/data/it/food.json` & `mimesis-8.0.0/mimesis/data/it/food.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/it/person.json` & `mimesis-8.0.0/mimesis/data/it/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/it/text.json` & `mimesis-8.0.0/mimesis/data/it/text.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/ja/address.json` & `mimesis-8.0.0/mimesis/data/ja/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/ja/finance.json` & `mimesis-8.0.0/mimesis/data/ja/finance.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6666666666666666%*

 * *Differences: {"'banks'": "['三菱UFJフィナンシャル・グループ', '三井住友フィナンシャルグループ', 'みずほフィナンシャルグループ', 'りそなグループ', '三菱UFJ信託銀行', "*

 * *            "'北海道銀行', '三菱UFJニコス', '住信SBIネット銀行', 'ゆうちょ銀行', 'オリックス銀行', 'SMBCフレンド証券', '埼玉りそな銀行', "*

 * *            "'静岡銀行', '八十二銀行', '関西アーバン銀行', '埼玉県信用金庫', '岩手銀行', '三菱UFJリース', '栃木銀行', '山口銀行', "*

 * *            "'日本政策投資銀行', '楽天証券', 'JAバンク', '福島銀行', 'オリエントコーポレーション', '東北電力金庫', 'フューチャーズ', '武蔵野銀行', "*

 * *            "'りそなアセットマネジメント', '大和証券', '岡山県信用農業協同組合連合会', '茨城銀行', '東日本旅客鉄道金融', '三菱UFJ国際投信', '富士銀行', "*

 * *            "'住友生命保険', '山形銀行 […]*

```diff
@@ -1,8 +1,64 @@
 {
+    "banks": [
+        "\u4e09\u83f1UFJ\u30d5\u30a3\u30ca\u30f3\u30b7\u30e3\u30eb\u30fb\u30b0\u30eb\u30fc\u30d7",
+        "\u4e09\u4e95\u4f4f\u53cb\u30d5\u30a3\u30ca\u30f3\u30b7\u30e3\u30eb\u30b0\u30eb\u30fc\u30d7",
+        "\u307f\u305a\u307b\u30d5\u30a3\u30ca\u30f3\u30b7\u30e3\u30eb\u30b0\u30eb\u30fc\u30d7",
+        "\u308a\u305d\u306a\u30b0\u30eb\u30fc\u30d7",
+        "\u4e09\u83f1UFJ\u4fe1\u8a17\u9280\u884c",
+        "\u5317\u6d77\u9053\u9280\u884c",
+        "\u4e09\u83f1UFJ\u30cb\u30b3\u30b9",
+        "\u4f4f\u4fe1SBI\u30cd\u30c3\u30c8\u9280\u884c",
+        "\u3086\u3046\u3061\u3087\u9280\u884c",
+        "\u30aa\u30ea\u30c3\u30af\u30b9\u9280\u884c",
+        "SMBC\u30d5\u30ec\u30f3\u30c9\u8a3c\u5238",
+        "\u57fc\u7389\u308a\u305d\u306a\u9280\u884c",
+        "\u9759\u5ca1\u9280\u884c",
+        "\u516b\u5341\u4e8c\u9280\u884c",
+        "\u95a2\u897f\u30a2\u30fc\u30d0\u30f3\u9280\u884c",
+        "\u57fc\u7389\u770c\u4fe1\u7528\u91d1\u5eab",
+        "\u5ca9\u624b\u9280\u884c",
+        "\u4e09\u83f1UFJ\u30ea\u30fc\u30b9",
+        "\u6803\u6728\u9280\u884c",
+        "\u5c71\u53e3\u9280\u884c",
+        "\u65e5\u672c\u653f\u7b56\u6295\u8cc7\u9280\u884c",
+        "\u697d\u5929\u8a3c\u5238",
+        "JA\u30d0\u30f3\u30af",
+        "\u798f\u5cf6\u9280\u884c",
+        "\u30aa\u30ea\u30a8\u30f3\u30c8\u30b3\u30fc\u30dd\u30ec\u30fc\u30b7\u30e7\u30f3",
+        "\u6771\u5317\u96fb\u529b\u91d1\u5eab",
+        "\u30d5\u30e5\u30fc\u30c1\u30e3\u30fc\u30ba",
+        "\u6b66\u8535\u91ce\u9280\u884c",
+        "\u308a\u305d\u306a\u30a2\u30bb\u30c3\u30c8\u30de\u30cd\u30b8\u30e1\u30f3\u30c8",
+        "\u5927\u548c\u8a3c\u5238",
+        "\u5ca1\u5c71\u770c\u4fe1\u7528\u8fb2\u696d\u5354\u540c\u7d44\u5408\u9023\u5408\u4f1a",
+        "\u8328\u57ce\u9280\u884c",
+        "\u6771\u65e5\u672c\u65c5\u5ba2\u9244\u9053\u91d1\u878d",
+        "\u4e09\u83f1UFJ\u56fd\u969b\u6295\u4fe1",
+        "\u5bcc\u58eb\u9280\u884c",
+        "\u4f4f\u53cb\u751f\u547d\u4fdd\u967a",
+        "\u5c71\u5f62\u9280\u884c",
+        "\u5343\u8449\u9280\u884c",
+        "\u65b0\u5149\u8a3c\u5238",
+        "\u6771\u4eac\u6d77\u4e0a\u65e5\u52d5\u706b\u707d\u4fdd\u967a",
+        "\u682a\u5f0f\u4f1a\u793e\u307f\u305a\u307b\u30b3\u30fc\u30dd\u30ec\u30fc\u30c8\u9280\u884c",
+        "\u30b8\u30e3\u30b9\u30c0\u30c3\u30af",
+        "\u65e5\u672c\u53d6\u5f15\u6240\u30b0\u30eb\u30fc\u30d7",
+        "\u4fe1\u7528\u4e0d\u52d5\u7523\u6295\u8cc7\u6cd5\u4eba",
+        "\u91ce\u6751\u4e0d\u52d5\u7523",
+        "\u91d1\u878d\u5546\u54c1\u53d6\u5f15\u6cd5\u4eba",
+        "\u5bcc\u5c71\u770c\u4fe1\u7528\u8fb2\u696d\u5354\u540c\u7d44\u5408\u9023\u5408\u4f1a",
+        "\u718a\u672c\u9280\u884c",
+        "\u65b0\u6f5f\u770c\u4fe1\u7528\u8fb2\u696d\u5354\u540c\u7d44\u5408\u9023\u5408\u4f1a",
+        "\u5c71\u68a8\u4e2d\u592e\u9280\u884c",
+        "\u611b\u5a9b\u770c\u4fe1\u7528\u8fb2\u696d\u5354\u540c\u7d44\u5408\u9023\u5408\u4f1a",
+        "\u9ad8\u77e5\u770c\u4fe1\u7528\u8fb2\u696d\u5354\u540c\u7d44\u5408\u9023\u5408\u4f1a",
+        "\u5317\u9678\u96fb\u529b\u91d1\u5eab",
+        "\u307f\u305a\u307b\u4fe1\u8a17\u9280\u884c"
+    ],
     "company": {
         "name": [
             "\u30ad\u30c3\u30c4",
             "\u795e\u6238\u88fd\u92fc\u6240",
             "\u4f4f\u53cb\u8efd\u91d1\u5c5e",
             "\u540c\u548c\u9271\u696d",
             "\u65e5\u9271\u91d1\u5c5e\u52a0\u5de5",
```

### Comparing `mimesis-7.1.0/mimesis/data/ja/food.json` & `mimesis-8.0.0/mimesis/data/ja/food.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/ja/person.json` & `mimesis-8.0.0/mimesis/data/ja/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/ja/text.json` & `mimesis-8.0.0/mimesis/data/ja/text.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/kk/address.json` & `mimesis-8.0.0/mimesis/data/kk/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/kk/datetime.json` & `mimesis-8.0.0/mimesis/data/kk/datetime.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/kk/finance.json` & `mimesis-8.0.0/mimesis/data/kk/finance.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6666666666666666%*

 * *Differences: {"'banks'": "['Halyk Bank Kazakhstan', 'Kazkommertsbank', 'ForteBank', 'Eurasian Bank', 'Bank "*

 * *            "CenterCredit', 'First Heartland Jysan Bank', 'Bank RBK', 'Bank ATFBank', "*

 * *            "'Tsesnabank', 'Bank Kaspi']"}*

```diff
@@ -1,8 +1,20 @@
 {
+    "banks": [
+        "Halyk Bank Kazakhstan",
+        "Kazkommertsbank",
+        "ForteBank",
+        "Eurasian Bank",
+        "Bank CenterCredit",
+        "First Heartland Jysan Bank",
+        "Bank RBK",
+        "Bank ATFBank",
+        "Tsesnabank",
+        "Bank Kaspi"
+    ],
     "company": {
         "name": [
             "ADVANCE MANAGEMENT",
             "ADVANCED BUSINESS TECHNOLOGIES",
             "AFL-ASTANA",
             "AISSANA",
             "AJE&N",
```

### Comparing `mimesis-7.1.0/mimesis/data/kk/person.json` & `mimesis-8.0.0/mimesis/data/kk/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/kk/text.json` & `mimesis-8.0.0/mimesis/data/kk/text.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/ko/address.json` & `mimesis-8.0.0/mimesis/data/ko/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/ko/finance.json` & `mimesis-8.0.0/mimesis/data/ko/finance.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6666666666666666%*

 * *Differences: {"'banks'": "['국민은행', '신한은행', '하나은행', '우리은행', '기업은행', 'SC제일은행', '대구은행', '광주은행', '부산은행', '전북은행', "*

 * *            "'제주은행', '수협은행', '축협은행', '우체국', '한국씨티은행', 'BNK금융지주', '케이뱅크', '카카오뱅크', '롯데카드', "*

 * *            "'하나SK카드']"}*

```diff
@@ -1,8 +1,30 @@
 {
+    "banks": [
+        "\uad6d\ubbfc\uc740\ud589",
+        "\uc2e0\ud55c\uc740\ud589",
+        "\ud558\ub098\uc740\ud589",
+        "\uc6b0\ub9ac\uc740\ud589",
+        "\uae30\uc5c5\uc740\ud589",
+        "SC\uc81c\uc77c\uc740\ud589",
+        "\ub300\uad6c\uc740\ud589",
+        "\uad11\uc8fc\uc740\ud589",
+        "\ubd80\uc0b0\uc740\ud589",
+        "\uc804\ubd81\uc740\ud589",
+        "\uc81c\uc8fc\uc740\ud589",
+        "\uc218\ud611\uc740\ud589",
+        "\ucd95\ud611\uc740\ud589",
+        "\uc6b0\uccb4\uad6d",
+        "\ud55c\uad6d\uc528\ud2f0\uc740\ud589",
+        "BNK\uae08\uc735\uc9c0\uc8fc",
+        "\ucf00\uc774\ubc45\ud06c",
+        "\uce74\uce74\uc624\ubc45\ud06c",
+        "\ub86f\ub370\uce74\ub4dc",
+        "\ud558\ub098SK\uce74\ub4dc"
+    ],
     "company": {
         "name": [
             "21\uc138\uae30\uc870\uc120",
             "\uac00\uc628\uc804\uc120",
             "\uac15\ub0a8\ub3c4\uc2dc\uac00\uc2a4",
             "\uac15\uc6d0\ub79c\ub4dc",
             "\uac1c\uc131\uc57d\ud488",
```

### Comparing `mimesis-7.1.0/mimesis/data/ko/food.json` & `mimesis-8.0.0/mimesis/data/ko/food.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/ko/person.json` & `mimesis-8.0.0/mimesis/data/ko/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/ko/text.json` & `mimesis-8.0.0/mimesis/data/ko/text.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/nl/address.json` & `mimesis-8.0.0/mimesis/data/nl/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/nl/food.json` & `mimesis-8.0.0/mimesis/data/nl/food.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/nl/person.json` & `mimesis-8.0.0/mimesis/data/nl/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/nl/text.json` & `mimesis-8.0.0/mimesis/data/nl/text.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/nl-be/address.json` & `mimesis-8.0.0/mimesis/data/nl-be/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/nl-be/finance.json` & `mimesis-8.0.0/mimesis/data/nl-be/finance.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6666666666666666%*

 * *Differences: {"'banks'": "['KBC Bank NV', 'Belfius Banque SA', 'BNP Paribas Fortis SA/NV', 'ING Belgique "*

 * *            "SA/NV', 'CBC Banque SA', 'Bpost Banque SA', 'AXA Bank Belgium SA', 'Euroclear Bank "*

 * *            "SA/NV', 'Crelan NV', 'Argenta Spaarbank NV']"}*

```diff
@@ -1,8 +1,20 @@
 {
+    "banks": [
+        "KBC Bank NV",
+        "Belfius Banque SA",
+        "BNP Paribas Fortis SA/NV",
+        "ING Belgique SA/NV",
+        "CBC Banque SA",
+        "Bpost Banque SA",
+        "AXA Bank Belgium SA",
+        "Euroclear Bank SA/NV",
+        "Crelan NV",
+        "Argenta Spaarbank NV"
+    ],
     "company": {
         "name": [
             "AG Real Estate",
             "AIM Productions",
             "ASL Airlines Belgium",
             "Abelag Aviation",
             "Ablynx",
```

### Comparing `mimesis-7.1.0/mimesis/data/nl-be/person.json` & `mimesis-8.0.0/mimesis/data/nl-be/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/no/address.json` & `mimesis-8.0.0/mimesis/data/no/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/no/finance.json` & `mimesis-8.0.0/mimesis/data/no/finance.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6666666666666666%*

 * *Differences: {"'banks'": "['DNB Bank ASA', 'Nordea Bank Abp filial i Norge', 'Danske Bank', 'Handelsbanken', "*

 * *            "'Sparebank 1']"}*

```diff
@@ -1,8 +1,15 @@
 {
+    "banks": [
+        "DNB Bank ASA",
+        "Nordea Bank Abp filial i Norge",
+        "Danske Bank",
+        "Handelsbanken",
+        "Sparebank 1"
+    ],
     "company": {
         "name": [
             "A Wilhelmsen",
             "A-K Holding Auctus",
             "A-Pressen",
             "ABB Holding",
             "ABG Sundal Colliera",
```

### Comparing `mimesis-7.1.0/mimesis/data/no/food.json` & `mimesis-8.0.0/mimesis/data/no/food.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/no/person.json` & `mimesis-8.0.0/mimesis/data/no/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/no/text.json` & `mimesis-8.0.0/mimesis/data/no/text.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/pl/address.json` & `mimesis-8.0.0/mimesis/data/pl/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/pl/datetime.json` & `mimesis-8.0.0/mimesis/data/pl/datetime.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/pl/finance.json` & `mimesis-8.0.0/mimesis/data/pl/finance.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6666666666666666%*

 * *Differences: {"'banks'": "['Bank Polska Kasa Opieki SA', 'Bank Pekao SA', 'Bank Gospodarstwa Krajowego', "*

 * *            "'Santander Bank Polska SA', 'mBank SA', 'ING Bank Śląski SA', 'Bank Millennium SA', "*

 * *            "'Getin Noble Bank SA', 'BGŻ BNP Paribas SA', 'Alior Bank SA', 'Raiffeisen Bank Polska "*

 * *            "SA', 'Bank Zachodni WBK SA', 'PKO Bank Polski SA', 'Eurobank SA', 'BNP Paribas Bank "*

 * *            "Polska SA', 'Nest Bank SA', 'Bank Ochrony Środowiska SA', 'Toyota Bank Polska SA', "*

 * *            "'Bank BG […]*

```diff
@@ -1,8 +1,62 @@
 {
+    "banks": [
+        "Bank Polska Kasa Opieki SA",
+        "Bank Pekao SA",
+        "Bank Gospodarstwa Krajowego",
+        "Santander Bank Polska SA",
+        "mBank SA",
+        "ING Bank \u015al\u0105ski SA",
+        "Bank Millennium SA",
+        "Getin Noble Bank SA",
+        "BG\u017b BNP Paribas SA",
+        "Alior Bank SA",
+        "Raiffeisen Bank Polska SA",
+        "Bank Zachodni WBK SA",
+        "PKO Bank Polski SA",
+        "Eurobank SA",
+        "BNP Paribas Bank Polska SA",
+        "Nest Bank SA",
+        "Bank Ochrony \u015arodowiska SA",
+        "Toyota Bank Polska SA",
+        "Bank BG\u017b BNP Paribas SA",
+        "Idea Bank SA",
+        "Deutsche Bank Polska SA",
+        "Credit Agricole Bank Polska SA",
+        "Bank Handlowy w Warszawie SA",
+        "Invest Bank SA",
+        "Powszechna Kasa Oszcz\u0119dno\u015bci Bank Polski SA",
+        "Bank Polskiej Sp\u00f3\u0142dzielczo\u015bci SA",
+        "Plus Bank SA",
+        "Societe Generale SA Oddzia\u0142 w Polsce",
+        "Bank Ochrony Praw Konsumenta SA",
+        "Bank Sp\u00f3\u0142dzielczy w Skierniewicach",
+        "Bank \u015al\u0105ski SA",
+        "Idea Bank SA",
+        "Deutsche Bank Polska SA",
+        "Credit Agricole Bank Polska SA",
+        "Bank Handlowy w Warszawie SA",
+        "Invest Bank SA",
+        "Powszechna Kasa Oszcz\u0119dno\u015bci Bank Polski SA",
+        "Bank Polskiej Sp\u00f3\u0142dzielczo\u015bci SA",
+        "Plus Bank SA",
+        "Societe Generale SA Oddzia\u0142 w Polsce",
+        "Bank Ochrony Praw Konsumenta SA",
+        "Bank Sp\u00f3\u0142dzielczy w Skierniewicach",
+        "Bank \u015al\u0105ski SA",
+        "Alior Bank SA",
+        "Raiffeisen Polbank",
+        "ING Bank \u015al\u0105ski SA",
+        "Santander Consumer Bank SA",
+        "Bank BPH SA",
+        "Deutsche Bank PBC SA",
+        "Bank Pocztowy SA",
+        "Bank DNB Nord Polska SA",
+        "Bank Gospodarki \u017bywno\u015bciowej SA"
+    ],
     "company": {
         "name": [
             "3maki",
             "4F",
             "A & B",
             "A. Zyska",
             "ABM Dr\u00f3b",
```

### Comparing `mimesis-7.1.0/mimesis/data/pl/food.json` & `mimesis-8.0.0/mimesis/data/pl/food.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/pl/person.json` & `mimesis-8.0.0/mimesis/data/pl/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/pl/text.json` & `mimesis-8.0.0/mimesis/data/pl/text.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/pt/address.json` & `mimesis-8.0.0/mimesis/data/pt/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/pt/datetime.json` & `mimesis-8.0.0/mimesis/data/pt/datetime.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/pt/food.json` & `mimesis-8.0.0/mimesis/data/pt/food.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/pt/person.json` & `mimesis-8.0.0/mimesis/data/pt/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/pt/text.json` & `mimesis-8.0.0/mimesis/data/pt/text.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/pt-br/address.json` & `mimesis-8.0.0/mimesis/data/pt-br/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/pt-br/datetime.json` & `mimesis-8.0.0/mimesis/data/pt-br/datetime.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/pt-br/food.json` & `mimesis-8.0.0/mimesis/data/pt-br/food.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/pt-br/person.json` & `mimesis-8.0.0/mimesis/data/pt-br/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/ru/address.json` & `mimesis-8.0.0/mimesis/data/ru/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/ru/builtin.json` & `mimesis-8.0.0/mimesis/data/ru/builtin.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/ru/datetime.json` & `mimesis-8.0.0/mimesis/data/ru/datetime.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/ru/finance.json` & `mimesis-8.0.0/mimesis/data/ru/finance.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.666243654822335%*

 * *Differences: {"'banks'": "['Абсолют Банк', 'Авангард Банк', 'Ак Барс Банк', 'Альфа-Банк', 'Банк Бинбанк', 'Банк "*

 * *            "Восточный', 'Банк Зенит', 'Банк Интеза', 'Банк Москвы', 'Банк Открытие', 'Банк ПСА "*

 * *            "Финанс Рус', 'Банк Первомайский', 'Банк Приморье', 'Банк СГБ', 'Банк "*

 * *            "Санкт-Петербург', 'Банк Сетелем', 'Банк Союз', 'Банк УралФДП', 'Банк Уралсиб', 'Банк "*

 * *            "ФК Открытие', 'Банк Финансы и Кредит', 'Банк Хоум Кредит', 'Банк ЮГРА', 'Бинбанк "*

 * *            "кредитные системы',  […]*

```diff
@@ -1,8 +1,68 @@
 {
+    "banks": [
+        "\u0410\u0431\u0441\u043e\u043b\u044e\u0442 \u0411\u0430\u043d\u043a",
+        "\u0410\u0432\u0430\u043d\u0433\u0430\u0440\u0434 \u0411\u0430\u043d\u043a",
+        "\u0410\u043a \u0411\u0430\u0440\u0441 \u0411\u0430\u043d\u043a",
+        "\u0410\u043b\u044c\u0444\u0430-\u0411\u0430\u043d\u043a",
+        "\u0411\u0430\u043d\u043a \u0411\u0438\u043d\u0431\u0430\u043d\u043a",
+        "\u0411\u0430\u043d\u043a \u0412\u043e\u0441\u0442\u043e\u0447\u043d\u044b\u0439",
+        "\u0411\u0430\u043d\u043a \u0417\u0435\u043d\u0438\u0442",
+        "\u0411\u0430\u043d\u043a \u0418\u043d\u0442\u0435\u0437\u0430",
+        "\u0411\u0430\u043d\u043a \u041c\u043e\u0441\u043a\u0432\u044b",
+        "\u0411\u0430\u043d\u043a \u041e\u0442\u043a\u0440\u044b\u0442\u0438\u0435",
+        "\u0411\u0430\u043d\u043a \u041f\u0421\u0410 \u0424\u0438\u043d\u0430\u043d\u0441 \u0420\u0443\u0441",
+        "\u0411\u0430\u043d\u043a \u041f\u0435\u0440\u0432\u043e\u043c\u0430\u0439\u0441\u043a\u0438\u0439",
+        "\u0411\u0430\u043d\u043a \u041f\u0440\u0438\u043c\u043e\u0440\u044c\u0435",
+        "\u0411\u0430\u043d\u043a \u0421\u0413\u0411",
+        "\u0411\u0430\u043d\u043a \u0421\u0430\u043d\u043a\u0442-\u041f\u0435\u0442\u0435\u0440\u0431\u0443\u0440\u0433",
+        "\u0411\u0430\u043d\u043a \u0421\u0435\u0442\u0435\u043b\u0435\u043c",
+        "\u0411\u0430\u043d\u043a \u0421\u043e\u044e\u0437",
+        "\u0411\u0430\u043d\u043a \u0423\u0440\u0430\u043b\u0424\u0414\u041f",
+        "\u0411\u0430\u043d\u043a \u0423\u0440\u0430\u043b\u0441\u0438\u0431",
+        "\u0411\u0430\u043d\u043a \u0424\u041a \u041e\u0442\u043a\u0440\u044b\u0442\u0438\u0435",
+        "\u0411\u0430\u043d\u043a \u0424\u0438\u043d\u0430\u043d\u0441\u044b \u0438 \u041a\u0440\u0435\u0434\u0438\u0442",
+        "\u0411\u0430\u043d\u043a \u0425\u043e\u0443\u043c \u041a\u0440\u0435\u0434\u0438\u0442",
+        "\u0411\u0430\u043d\u043a \u042e\u0413\u0420\u0410",
+        "\u0411\u0438\u043d\u0431\u0430\u043d\u043a \u043a\u0440\u0435\u0434\u0438\u0442\u043d\u044b\u0435 \u0441\u0438\u0441\u0442\u0435\u043c\u044b",
+        "\u0412\u0422\u0411 24",
+        "\u0412\u0422\u0411 \u0411\u0430\u043d\u043a",
+        "\u0412\u043e\u0437\u0440\u043e\u0436\u0434\u0435\u043d\u0438\u0435",
+        "\u0413\u0430\u0437\u043f\u0440\u043e\u043c\u0431\u0430\u043d\u043a",
+        "\u0418\u043d\u0432\u0435\u0441\u0442\u0442\u043e\u0440\u0433\u0431\u0430\u043d\u043a",
+        "\u041a\u0440\u0435\u0434\u0438\u0442 \u0411\u0430\u043d\u043a \u041c\u043e\u0441\u043a\u0432\u0430",
+        "\u041a\u0440\u0435\u0434\u0438\u0442 \u0415\u0432\u0440\u043e\u043f\u0430 \u0411\u0430\u043d\u043a",
+        "\u041b\u043e\u043a\u043e-\u0411\u0430\u043d\u043a",
+        "\u041c\u0422\u0421 \u0411\u0430\u043d\u043a",
+        "\u041c\u043e\u0441\u043a\u043e\u0432\u0441\u043a\u0438\u0439 \u0418\u043d\u0434\u0443\u0441\u0442\u0440\u0438\u0430\u043b\u044c\u043d\u044b\u0439 \u0411\u0430\u043d\u043a",
+        "\u041c\u043e\u0441\u043a\u043e\u0432\u0441\u043a\u0438\u0439 \u041a\u0440\u0435\u0434\u0438\u0442\u043d\u044b\u0439 \u0411\u0430\u043d\u043a",
+        "\u041c\u043e\u0441\u043a\u043e\u0432\u0441\u043a\u0438\u0439 \u041e\u0431\u043b\u0430\u0441\u0442\u043d\u043e\u0439 \u0411\u0430\u043d\u043a",
+        "\u041f\u0435\u0440\u0432\u044b\u0439 \u0420\u0435\u0441\u043f\u0443\u0431\u043b\u0438\u043a\u0430\u043d\u0441\u043a\u0438\u0439 \u0411\u0430\u043d\u043a",
+        "\u041f\u043e\u0447\u0442\u0430 \u0411\u0430\u043d\u043a",
+        "\u041f\u0440\u043e\u043c\u0441\u0432\u044f\u0437\u044c\u0431\u0430\u043d\u043a",
+        "\u0420\u041d\u041a\u0411 \u0411\u0430\u043d\u043a",
+        "\u0420\u0430\u0439\u0444\u0444\u0430\u0439\u0437\u0435\u043d\u0431\u0430\u043d\u043a",
+        "\u0420\u043e\u0441\u0431\u0430\u043d\u043a",
+        "\u0420\u043e\u0441\u0433\u043e\u0441\u0441\u0442\u0440\u0430\u0445 \u0411\u0430\u043d\u043a",
+        "\u0420\u043e\u0441\u0441\u0435\u043b\u044c\u0445\u043e\u0437\u0431\u0430\u043d\u043a",
+        "\u0420\u043e\u0441\u0441\u0438\u0439\u0441\u043a\u0438\u0439 \u041a\u0430\u043f\u0438\u0442\u0430\u043b",
+        "\u0420\u043e\u0441\u0441\u0438\u0439\u0441\u043a\u0438\u0439 \u0421\u0435\u043b\u044c\u0441\u043a\u043e\u0445\u043e\u0437\u044f\u0439\u0441\u0442\u0432\u0435\u043d\u043d\u044b\u0439 \u0411\u0430\u043d\u043a",
+        "\u0420\u0443\u0441\u0441\u043a\u0438\u0439 \u0421\u0442\u0430\u043d\u0434\u0430\u0440\u0442 \u0411\u0430\u043d\u043a",
+        "\u0420\u0443\u0441\u0444\u0438\u043d\u0430\u043d\u0441 \u0411\u0430\u043d\u043a",
+        "\u0421\u041c\u041f \u0411\u0430\u043d\u043a",
+        "\u0421\u0431\u0435\u0440\u0431\u0430\u043d\u043a",
+        "\u0421\u0431\u0435\u0440\u0431\u0430\u043d\u043a \u0420\u043e\u0441\u0441\u0438\u0438",
+        "\u0421\u0438\u0442\u0438\u0431\u0430\u043d\u043a \u041a\u0430\u0437\u0430\u0445\u0441\u0442\u0430\u043d",
+        "\u0421\u0438\u0442\u0438\u0431\u0430\u043d\u043a \u0420\u043e\u0441\u0441\u0438\u044f",
+        "\u0421\u043e\u0432\u043a\u043e\u043c\u0431\u0430\u043d\u043a",
+        "\u0422\u0438\u043d\u044c\u043a\u043e\u0444\u0444 \u0411\u0430\u043d\u043a",
+        "\u0423\u0440\u0430\u043b\u0441\u0438\u0431",
+        "\u0425\u0430\u043d\u0442\u044b-\u041c\u0430\u043d\u0441\u0438\u0439\u0441\u043a\u0438\u0439 \u0431\u0430\u043d\u043a \u041e\u0442\u043a\u0440\u044b\u0442\u0438\u0435",
+        "\u042e\u043d\u0438\u041a\u0440\u0435\u0434\u0438\u0442 \u0411\u0430\u043d\u043a"
+    ],
     "company": {
         "name": [
             "Crocus Group",
             "Dixis",
             "Genser",
             "Google",
             "IBS",
@@ -209,15 +269,15 @@
             "\u0410\u041a \u00ab\u0422\u0440\u0430\u043d\u0441\u043d\u0435\u0444\u0442\u044c\u00bb",
             "\u0410\u0421\u0422",
             "\u0410\u0422\u042d\u041a/\u041a\u0435\u0441\u043d\u043e-\u041c",
             "\u0410\u0424\u041a \u00ab\u0421\u0438\u0441\u0442\u0435\u043c\u0430\u00bb",
             "\u0410\u0431\u0441\u043e\u043b\u044e\u0442 \u0431\u0430\u043d\u043a",
             "\u0410\u0432\u0438\u0430\u043a\u043e\u043c\u043f\u0430\u043d\u0438\u044f \u00ab\u0422\u0440\u0430\u043d\u0441\u0430\u044d\u0440\u043e\u00bb",
             "\u0410\u0432\u0438\u0430\u043a\u043e\u043c\u043f\u0430\u043d\u0438\u044f \u00ab\u042e\u0422\u044d\u0439\u0440\u00bb",
-            "\u0410\u0432\u0442\u043e \u041c\u043e\u0442\u043e\u0440 \u0413\u0440\u0443\u043f\u043f\u0430 (\u0410\u0440\u043c\u0430\u043d\u0434)",
+            "\u0410\u0432\u0442\u043e \u041c\u043e\u0442\u043e\u0440 \u0413\u0440\u0443\u043f\u043f\u0430",
             "\u0410\u0432\u0442\u043e\u0412\u0410\u0417\u0430\u0433\u0440\u0435\u0433\u0430\u0442",
             "\u0410\u0432\u0442\u043e\u043c\u0438\u0440",
             "\u0410\u0432\u0442\u043e\u0442\u043e\u0440",
             "\u0410\u0432\u0442\u043e\u0442\u043e\u0440 \u0445\u043e\u043b\u0434\u0438\u043d\u0433",
             "\u0410\u0433\u0440\u043e\u0433\u0440\u0443\u043f\u043f\u0430 \u00ab\u0425\u043e\u0440\u043e\u0448\u0435\u0435 \u0434\u0435\u043b\u043e\u00bb",
             "\u0410\u0433\u0440\u043e\u043a\u043e\u043c\u043f\u043b\u0435\u043a\u0441 \u0438\u043c\u0435\u043d\u0438 \u041d. \u0418. \u0422\u043a\u0430\u0447\u0435\u0432\u0430",
             "\u0410\u0433\u0440\u043e\u043f\u0440\u043e\u043c\u044b\u0448\u043b\u0435\u043d\u043d\u0430\u044f \u0433\u0440\u0443\u043f\u043f\u0430 \u00ab\u041f\u0440\u043e\u0434\u043e\u00bb",
@@ -402,15 +462,15 @@
             "\u041c\u0424\u0421-6",
             "\u041c\u0430\u0433\u043d\u0438\u0442\u043e\u0433\u043e\u0440\u0441\u043a\u0438\u0439 \u043c\u0435\u0442\u0430\u043b\u043b\u0443\u0440\u0433\u0438\u0447\u0435\u0441\u043a\u0438\u0439 \u043a\u043e\u043c\u0431\u0438\u043d\u0430\u0442",
             "\u041c\u0430\u0440\u0438\u0439\u0441\u043a\u0438\u0439 \u041d\u041f\u0417",
             "\u041c\u0430\u0440\u0442\u0430",
             "\u041c\u0430\u0441\u043b\u043e\u044d\u043a\u0441\u0442\u0440\u0430\u043a\u0446\u0438\u043e\u043d\u043d\u044b\u0439 \u0437\u0430\u0432\u043e\u0434 \u00ab\u042e\u0433 \u0420\u0443\u0441\u0438\u00bb",
             "\u041c\u0430\u0448\u0438\u043d\u043e\u0441\u0442\u0440\u043e\u0438\u0442\u0435\u043b\u044c\u043d\u044b\u0439 \u0437\u0430\u0432\u043e\u0434 \u0438\u043c\u0435\u043d\u0438 \u041c. \u0418. \u041a\u0430\u043b\u0438\u043d\u0438\u043d\u0430",
             "\u041c\u0435\u0433\u0430\u0424\u043e\u043d",
-            "\u041c\u0435\u0433\u0430\u043f\u043e\u043b\u0438\u0441 (\u043a\u043e\u043c\u043f\u0430\u043d\u0438\u044f)",
+            "\u041c\u0435\u0433\u0430\u043f\u043e\u043b\u0438\u0441",
             "\u041c\u0435\u0436\u0434\u0443\u043d\u0430\u0440\u043e\u0434\u043d\u044b\u0439 \u0430\u044d\u0440\u043e\u043f\u043e\u0440\u0442 \u0428\u0435\u0440\u0435\u043c\u0435\u0442\u044c\u0435\u0432\u043e",
             "\u041c\u0435\u0442\u0430\u043b\u043b\u043e\u0438\u043d\u0432\u0435\u0441\u0442",
             "\u041c\u0435\u0442\u0430\u043b\u043b\u0441\u0435\u0440\u0432\u0438\u0441",
             "\u041c\u0438\u0440",
             "\u041c\u0438\u0440\u0430\u0442\u043e\u0440\u0433",
             "\u041c\u0438\u044d\u043b\u044c-\u041d\u0435\u0434\u0432\u0438\u0436\u0438\u043c\u043e\u0441\u0442\u044a",
             "\u041c\u043e\u0440\u043e\u043d",
@@ -576,15 +636,15 @@
             "\u0426\u0435\u043d\u0442\u0440 \u044d\u043a\u0441\u043f\u043b\u0443\u0430\u0442\u0430\u0446\u0438\u0438 \u043e\u0431\u044a\u0435\u043a\u0442\u043e\u0432 \u043d\u0430\u0437\u0435\u043c\u043d\u043e\u0439 \u043a\u043e\u0441\u043c\u0438\u0447\u0435\u0441\u043a\u043e\u0439 \u0438\u043d\u0444\u0440\u0430\u0441\u0442\u0440\u0443\u043a\u0442\u0443\u0440\u044b",
             "\u0426\u0435\u043d\u0442\u0440\u0430\u043b\u044c\u043d\u0430\u044f \u043f\u0440\u0438\u0433\u043e\u0440\u043e\u0434\u043d\u0430\u044f \u043f\u0430\u0441\u0441\u0430\u0436\u0438\u0440\u0441\u043a\u0430\u044f \u043a\u043e\u043c\u043f\u0430\u043d\u0438\u044f",
             "\u0426\u0438\u0444\u0440\u043e\u0433\u0440\u0430\u0434",
             "\u0427\u0435\u043b\u044f\u0431\u0438\u043d\u0441\u043a\u0438\u0439 \u044d\u043b\u0435\u043a\u0442\u0440\u043e\u043c\u0435\u0442\u0430\u043b\u043b\u0443\u0440\u0433\u0438\u0447\u0435\u0441\u043a\u0438\u0439 \u043a\u043e\u043c\u0431\u0438\u043d\u0430\u0442",
             "\u0427\u0443\u043a\u043e\u0442\u0441\u043a\u0430\u044f \u0433\u043e\u0440\u043d\u043e-\u0433\u0435\u043e\u043b\u043e\u0433\u0438\u0447\u0435\u0441\u043a\u0430\u044f \u043a\u043e\u043c\u043f\u0430\u043d\u0438\u044f",
             "\u042d\u043a\u0441\u0438\u043c\u0430",
             "\u042d\u043a\u0441\u043f\u0435\u0440\u0442-\u041a\u043e\u0440\u0441\u043e",
-            "\u042d\u043b\u044c\u0434\u043e\u0440\u0430\u0434\u043e (\u0441\u0435\u0442\u044c \u043c\u0430\u0433\u0430\u0437\u0438\u043d\u043e\u0432)",
+            "\u042d\u043b\u044c\u0434\u043e\u0440\u0430\u0434\u043e",
             "\u042d\u043d\u0435\u0440\u0433\u043e\u0441\u0431\u044b\u0442\u043e\u0432\u0430\u044f \u043a\u043e\u043c\u043f\u0430\u043d\u0438\u044f \u00ab\u0412\u043e\u0441\u0442\u043e\u043a\u00bb",
             "\u042d\u043d\u0435\u0440\u0433\u043e\u0441\u0442\u0440\u043e\u0439\u0438\u043d\u0432\u0435\u0441\u0442-\u0425\u043e\u043b\u0434\u0438\u043d\u0433",
             "\u042e\u041d\u042d\u041a\u0422",
             "\u042e\u0433 \u0420\u0443\u0441\u0438",
             "\u042e\u0433\u0442\u0440\u0430\u043d\u0437\u0438\u0442\u0441\u0435\u0440\u0432\u0438\u0441",
             "\u042e\u0436\u043d\u0430\u044f \u043d\u0435\u0444\u0442\u0435\u043f\u0435\u0440\u0435\u0440\u0430\u0431\u0430\u0442\u044b\u0432\u0430\u044e\u0449\u0430\u044f \u043a\u043e\u043c\u043f\u0430\u043d\u0438\u044f",
             "\u042e\u043d\u0438\u043a\u0440\u0435\u0434\u0438\u0442\u0431\u0430\u043d\u043a",
```

### Comparing `mimesis-7.1.0/mimesis/data/ru/food.json` & `mimesis-8.0.0/mimesis/data/ru/food.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/ru/person.json` & `mimesis-8.0.0/mimesis/data/ru/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/ru/text.json` & `mimesis-8.0.0/mimesis/data/ru/text.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/sk/address.json` & `mimesis-8.0.0/mimesis/data/sk/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/sk/person.json` & `mimesis-8.0.0/mimesis/data/sk/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/sk/text.json` & `mimesis-8.0.0/mimesis/data/sk/text.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/sv/address.json` & `mimesis-8.0.0/mimesis/data/sv/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/sv/finance.json` & `mimesis-8.0.0/mimesis/data/sv/finance.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6666666666666666%*

 * *Differences: {"'banks'": "['Swedbank AB', 'Nordea Bank Abp, filial i Sverige', 'Handelsbanken', 'Skandinaviska "*

 * *            "Enskilda Banken AB', 'Danske Bank', 'Länsförsäkringar Bank AB', 'SEB Kort AB', 'Ikano "*

 * *            "Bank AB', 'Resurs Bank AB', 'ICA Banken AB', 'Sparbanken Syd', 'Marginalen Bank "*

 * *            "Bankaktiebolag', 'Svea Ekonomi AB', 'Svenska Handelsbanken AB', 'Söderberg & Partners "*

 * *            "AB', 'BlueStep Bank AB', 'Dnb Bank Asa, Sverige Filial', 'Carnegie Investment Bank "*

 * *            "AB', […]*

```diff
@@ -1,8 +1,40 @@
 {
+    "banks": [
+        "Swedbank AB",
+        "Nordea Bank Abp, filial i Sverige",
+        "Handelsbanken",
+        "Skandinaviska Enskilda Banken AB",
+        "Danske Bank",
+        "L\u00e4nsf\u00f6rs\u00e4kringar Bank AB",
+        "SEB Kort AB",
+        "Ikano Bank AB",
+        "Resurs Bank AB",
+        "ICA Banken AB",
+        "Sparbanken Syd",
+        "Marginalen Bank Bankaktiebolag",
+        "Svea Ekonomi AB",
+        "Svenska Handelsbanken AB",
+        "S\u00f6derberg & Partners AB",
+        "BlueStep Bank AB",
+        "Dnb Bank Asa, Sverige Filial",
+        "Carnegie Investment Bank AB",
+        "Nordnet Bank AB",
+        "Nordax Bank AB",
+        "L\u00e4nsf\u00f6rs\u00e4kringar Hypotek AB",
+        "Handelsbanken Finans AB",
+        "SBAB Bank AB",
+        "CitiBank N.A., Sverige Filial",
+        "BNP Paribas SA, Sverige Filial",
+        "BNP Paribas Fortis SA/NV, Sverige Filial",
+        "J.P. Morgan AG, Stockholm Filial",
+        "Svenska Exportkredit AB",
+        "Morgonstj\u00e4rnan AB",
+        "JAK Medlemsbank Ekonomisk F\u00f6rening"
+    ],
     "company": {
         "name": [
             "3H Biomedical",
             "AB Svensk Filmindustri",
             "ABU Garcia",
             "AGA",
             "AP&T",
```

### Comparing `mimesis-7.1.0/mimesis/data/sv/food.json` & `mimesis-8.0.0/mimesis/data/sv/food.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/sv/person.json` & `mimesis-8.0.0/mimesis/data/sv/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/sv/text.json` & `mimesis-8.0.0/mimesis/data/sv/text.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/tr/address.json` & `mimesis-8.0.0/mimesis/data/tr/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/tr/finance.json` & `mimesis-8.0.0/mimesis/data/tr/finance.json`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6666666666666666%*

 * *Differences: {"'banks'": "['Akbank T.A.S.', 'Turkiye Garanti Bankasi A.S.', 'Turkiye Is Bankasi A.S.', 'Turkiye "*

 * *            "Halk Bankasi A.S.', 'Turkiye Vakiflar Bankasi T.A.O.', 'Yapi ve Kredi Bankasi A.S.', "*

 * *            "'Ziraat Bankasi A.S.', 'QNB Finansbank A.S.', 'Turkiye Sinai Kalkinma Bankasi A.S.', "*

 * *            "'TEB Kobi Finansmani A.S.', 'Burgan Bank A.S.', 'Turkiye Finans Katilim Bankasi "*

 * *            "A.S.', 'Denizbank A.S.', 'ICBC Turkey Bank A.S.', 'HSBC Bank A.S.', 'Alternatifbank "*

 * *            "A.S. […]*

```diff
@@ -1,8 +1,59 @@
 {
+    "banks": [
+        "Akbank T.A.S.",
+        "Turkiye Garanti Bankasi A.S.",
+        "Turkiye Is Bankasi A.S.",
+        "Turkiye Halk Bankasi A.S.",
+        "Turkiye Vakiflar Bankasi T.A.O.",
+        "Yapi ve Kredi Bankasi A.S.",
+        "Ziraat Bankasi A.S.",
+        "QNB Finansbank A.S.",
+        "Turkiye Sinai Kalkinma Bankasi A.S.",
+        "TEB Kobi Finansmani A.S.",
+        "Burgan Bank A.S.",
+        "Turkiye Finans Katilim Bankasi A.S.",
+        "Denizbank A.S.",
+        "ICBC Turkey Bank A.S.",
+        "HSBC Bank A.S.",
+        "Alternatifbank A.S.",
+        "ING Bank A.S.",
+        "Anadolubank A.S.",
+        "Odea Bank A.S.",
+        "Aktif Bank A.S.",
+        "T.C. Ziraat Bankasi Londra Subesi",
+        "JPMorgan Chase Bank N.A. Istanbul Branch",
+        "Deutsche Bank A.S.",
+        "The Royal Bank of Scotland plc",
+        "Citibank A.S.",
+        "Turk Ekonomi Bankasi A.S.",
+        "Abu Dhabi Islamic Bank PJSC Turkey",
+        "Turkland Bank A.S.",
+        "Qatar National Bank Turkey",
+        "Bank of America N.A. Istanbul Branch",
+        "Standard Chartered Yatirim Bankasi Turkiye A.S.",
+        "Garanti BBVA International S.A.",
+        "BNP Paribas Turkey",
+        "Akbank International N.V.",
+        "HSBC Bank A.S. Paris Branch",
+        "Turk Eximbank",
+        "Sumitomo Mitsui Banking Corporation Europe Limited",
+        "Turkish Bank Ltd.",
+        "Pasha Yatirim Bankasi A.S.",
+        "Ptt Finansal Hizmetler A.S.",
+        "Garanti BBVA Securities International S.A.",
+        "Rabobank International Istanbul Branch",
+        "Citi Menkul Degerler A.S.",
+        "Societe Generale Istanbul Branch",
+        "QNB Finansinvest A.S.",
+        "Commerzbank A.G. Istanbul Branch",
+        "Banco Bilbao Vizcaya Argentaria S.A. Istanbul Branch",
+        "Turk Ekonomi Bankasi A.S. Frankfurt Branch",
+        "Banco Santander S.A. Istanbul Branch"
+    ],
     "company": {
         "name": [
             "Ac\u0131selsan Ac\u0131payam Sel\u00fcloz",
             "Adana",
             "Adel Kalemcilik Ticaret ve Sanayi",
             "Adese Al\u0131\u015fveri\u015f Merkezleri Ticaret A.\u015e",
             "Afyon",
```

### Comparing `mimesis-7.1.0/mimesis/data/tr/food.json` & `mimesis-8.0.0/mimesis/data/tr/food.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/tr/person.json` & `mimesis-8.0.0/mimesis/data/tr/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/tr/text.json` & `mimesis-8.0.0/mimesis/data/tr/text.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/uk/address.json` & `mimesis-8.0.0/mimesis/data/uk/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/uk/builtin.json` & `mimesis-8.0.0/mimesis/data/uk/builtin.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/uk/datetime.json` & `mimesis-8.0.0/mimesis/data/uk/datetime.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/uk/finance.json` & `mimesis-8.0.0/mimesis/data/uk/finance.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6666666666666666%*

 * *Differences: {"'banks'": "['Абанк', 'Аваль', 'Альфа-Банк', 'Альянс', 'Асвіо Банк', 'Банк Восток', 'Банк Грант', "*

 * *            "'Банк Дніпро', 'Банк Ідея Банк', 'Банк Кредит Дніпро', 'Банк Михайлівський', 'Банк "*

 * *            "Пивденкомбанк', 'Банк Поділля', 'Банк Ренесанс Капітал', 'Банк Січ', 'Банк Українська "*

 * *            "Фінансова Група', 'Банк Фінанси та Кредит', 'Банк Хоум Кредит', 'БАНК-КЛІРИНГОВИХ "*

 * *            "ТЕХНОЛОГІЙ', 'БАНКОВА КОЛЕГІЯ', 'БАНКОВИЙ ДІМ', 'БАНКОВСЬКИЙ ЦЕНТР КРЕДИТУ', 'БОНУС "*

 * *            "БАН […]*

```diff
@@ -1,8 +1,55 @@
 {
+    "banks": [
+        "\u0410\u0431\u0430\u043d\u043a",
+        "\u0410\u0432\u0430\u043b\u044c",
+        "\u0410\u043b\u044c\u0444\u0430-\u0411\u0430\u043d\u043a",
+        "\u0410\u043b\u044c\u044f\u043d\u0441",
+        "\u0410\u0441\u0432\u0456\u043e \u0411\u0430\u043d\u043a",
+        "\u0411\u0430\u043d\u043a \u0412\u043e\u0441\u0442\u043e\u043a",
+        "\u0411\u0430\u043d\u043a \u0413\u0440\u0430\u043d\u0442",
+        "\u0411\u0430\u043d\u043a \u0414\u043d\u0456\u043f\u0440\u043e",
+        "\u0411\u0430\u043d\u043a \u0406\u0434\u0435\u044f \u0411\u0430\u043d\u043a",
+        "\u0411\u0430\u043d\u043a \u041a\u0440\u0435\u0434\u0438\u0442 \u0414\u043d\u0456\u043f\u0440\u043e",
+        "\u0411\u0430\u043d\u043a \u041c\u0438\u0445\u0430\u0439\u043b\u0456\u0432\u0441\u044c\u043a\u0438\u0439",
+        "\u0411\u0430\u043d\u043a \u041f\u0438\u0432\u0434\u0435\u043d\u043a\u043e\u043c\u0431\u0430\u043d\u043a",
+        "\u0411\u0430\u043d\u043a \u041f\u043e\u0434\u0456\u043b\u043b\u044f",
+        "\u0411\u0430\u043d\u043a \u0420\u0435\u043d\u0435\u0441\u0430\u043d\u0441 \u041a\u0430\u043f\u0456\u0442\u0430\u043b",
+        "\u0411\u0430\u043d\u043a \u0421\u0456\u0447",
+        "\u0411\u0430\u043d\u043a \u0423\u043a\u0440\u0430\u0457\u043d\u0441\u044c\u043a\u0430 \u0424\u0456\u043d\u0430\u043d\u0441\u043e\u0432\u0430 \u0413\u0440\u0443\u043f\u0430",
+        "\u0411\u0430\u043d\u043a \u0424\u0456\u043d\u0430\u043d\u0441\u0438 \u0442\u0430 \u041a\u0440\u0435\u0434\u0438\u0442",
+        "\u0411\u0430\u043d\u043a \u0425\u043e\u0443\u043c \u041a\u0440\u0435\u0434\u0438\u0442",
+        "\u0411\u0410\u041d\u041a-\u041a\u041b\u0406\u0420\u0418\u041d\u0413\u041e\u0412\u0418\u0425 \u0422\u0415\u0425\u041d\u041e\u041b\u041e\u0413\u0406\u0419",
+        "\u0411\u0410\u041d\u041a\u041e\u0412\u0410 \u041a\u041e\u041b\u0415\u0413\u0406\u042f",
+        "\u0411\u0410\u041d\u041a\u041e\u0412\u0418\u0419 \u0414\u0406\u041c",
+        "\u0411\u0410\u041d\u041a\u041e\u0412\u0421\u042c\u041a\u0418\u0419 \u0426\u0415\u041d\u0422\u0420 \u041a\u0420\u0415\u0414\u0418\u0422\u0423",
+        "\u0411\u041e\u041d\u0423\u0421 \u0411\u0410\u041d\u041a",
+        "\u0411\u0423\u0414\u0406\u0412\u0415\u041b\u042c\u041d\u0418\u0419 \u041a\u041e\u041c\u0415\u0420\u0426\u0406\u0419\u041d\u0418\u0419 \u0411\u0410\u041d\u041a",
+        "\u0412\u0415\u0421\u0422\u0410",
+        "\u0413\u0420\u0410\u041d\u0406\u0422 \u0411\u0410\u041d\u041a",
+        "\u0414\u0415\u041c\u0415\u0422\u0420\u0410",
+        "\u0414\u041d\u0406\u0421\u0422\u0415\u0420",
+        "\u0415\u041d\u0415\u0420\u0413\u041e\u0411\u0410\u041d\u041a",
+        "\u0415\u0420\u0421 \u0411\u0430\u043d\u043a",
+        "\u0406\u041d\u0412\u0415\u0421\u0422 \u0411\u0410\u041d\u041a",
+        "\u041a\u0418\u0407\u0412",
+        "\u041c\u0415\u0413\u0410\u0411\u0410\u041d\u041a",
+        "\u041c\u0406\u041d\u0411\u0410\u041d\u041a",
+        "\u041d\u0410\u0422\u0406\u041e\u041d\u0410\u041b\u042c\u041d\u0418\u0419 \u041a\u0420\u0415\u0414\u0418\u0422",
+        "\u041e\u0429\u0410\u0414\u0411\u0410\u041d\u041a",
+        "\u041f\u0420\u0410\u0412\u0415\u041a\u0421-\u0411\u0410\u041d\u041a",
+        "\u041f\u0420\u0418\u0412\u0410\u0422\u0411\u0410\u041d\u041a",
+        "\u041f\u0423\u041c\u0411",
+        "\u0420\u0430\u0439\u0444\u0444\u0430\u0439\u0437\u0435\u043d \u0411\u0430\u043d\u043a \u0410\u0432\u0430\u043b\u044c",
+        "\u0423\u043a\u0440\u0433\u0430\u0437\u0431\u0430\u043d\u043a",
+        "\u0423\u043a\u0440\u0435\u043a\u0441\u0456\u043c\u0431\u0430\u043d\u043a",
+        "\u0423\u043a\u0440\u0441\u0438\u0431\u0431\u0430\u043d\u043a",
+        "\u0423\u043a\u0440\u0441\u043e\u0446\u0431\u0430\u043d\u043a",
+        "\u0423\u043d\u0456\u043a\u0440\u0435\u0434\u0438\u0442 \u0431\u0430\u043d\u043a"
+    ],
     "company": {
         "name": [
             "\u041d\u0430\u0444\u0442\u043e\u0433\u0430\u0437",
             "\u041c\u0435\u0442\u0456\u043d\u0432\u0435\u0441\u0442",
             "\u0414\u041f \u0415\u043d\u0435\u0440\u0433\u043e\u0440\u0438\u043d\u043e\u043a",
             "\u0423\u043a\u0440\u0437\u0430\u043b\u0456\u0437\u043d\u0438\u0446\u044f",
             "\u0406\u0421\u0414",
```

### Comparing `mimesis-7.1.0/mimesis/data/uk/food.json` & `mimesis-8.0.0/mimesis/data/uk/food.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/uk/person.json` & `mimesis-8.0.0/mimesis/data/uk/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/uk/text.json` & `mimesis-8.0.0/mimesis/data/uk/text.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/zh/address.json` & `mimesis-8.0.0/mimesis/data/zh/address.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/zh/datetime.json` & `mimesis-8.0.0/mimesis/data/zh/datetime.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/zh/food.json` & `mimesis-8.0.0/mimesis/data/zh/food.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/zh/person.json` & `mimesis-8.0.0/mimesis/data/zh/person.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/data/zh/text.json` & `mimesis-8.0.0/mimesis/data/zh/text.json`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/enums.py` & `mimesis-8.0.0/mimesis/enums.py`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/exceptions.py` & `mimesis-8.0.0/mimesis/exceptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -56,7 +56,14 @@
         self.message = "Field «{}» is not supported."
         self.message_none = "The field cannot have the value None."
 
     def __str__(self) -> str:
         if self.name is None:
             return self.message_none
         return self.message.format(self.name)
+
+
+class FieldsetError(ValueError):
+    """Raised when a resulting fieldset is empty."""
+
+    def __str__(self) -> str:
+        return "The «iterations» parameter must be greater than 1."
```

### Comparing `mimesis-7.1.0/mimesis/providers/__init__.py` & `mimesis-8.0.0/mimesis/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/providers/address.py` & `mimesis-8.0.0/mimesis/providers/address.py`

 * *Files 3% similar despite different names*

```diff
@@ -179,27 +179,30 @@
         :param code: Enum object CountryCode.
         :return: Country code in selected format.
         :raises KeyError: if fmt is not supported.
         """
         key = self.validate_enum(code, CountryCode)
         return self.random.choice(COUNTRY_CODES[key])
 
-    def country(self, allow_random: bool = False) -> str:
-        """Get the country of the current locale.
+    def default_country(self) -> str:
+        """Get the country associated with the current locale.
 
-        :param allow_random: Return a random country name.
-        :return: The Country.
+        :return: The country associated with current locale.
         """
-        if allow_random:
-            countries: t.List[str] = self.extract(["country", "name"])
-            return self.random.choice(countries)
-
         country: str = self.extract(["country", "current_locale"])
         return country
 
+    def country(self) -> str:
+        """Get a random country.
+
+        :return: The Country.
+        """
+        countries: t.List[str] = self.extract(["country", "name"])
+        return self.random.choice(countries)
+
     def city(self) -> str:
         """Get a random city.
 
         :return: City name.
         """
         cities: t.List[str] = self.extract(["city"])
         return self.random.choice(cities)
```

### Comparing `mimesis-7.1.0/mimesis/providers/base.py` & `mimesis-8.0.0/mimesis/providers/base.py`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/providers/binaryfile.py` & `mimesis-8.0.0/mimesis/providers/binaryfile.py`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/providers/choice.py` & `mimesis-8.0.0/mimesis/providers/choice.py`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/providers/code.py` & `mimesis-8.0.0/mimesis/providers/code.py`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/providers/cryptographic.py` & `mimesis-8.0.0/mimesis/providers/cryptographic.py`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/providers/date.py` & `mimesis-8.0.0/mimesis/providers/date.py`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/providers/development.py` & `mimesis-8.0.0/mimesis/providers/development.py`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/providers/file.py` & `mimesis-8.0.0/mimesis/providers/file.py`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/providers/finance.py` & `mimesis-8.0.0/mimesis/providers/finance.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,14 +61,22 @@
         """
         code: str = self.extract(["currency-code"])
 
         if allow_random:
             return self.random.choice(CURRENCY_ISO_CODES)
         return code
 
+    def bank(self) -> str:
+        """Get a random bank name.
+
+        :return: Bank name.
+        """
+        banks: t.List[str] = self.extract(["banks"])
+        return self.random.choice(banks)
+
     def cryptocurrency_iso_code(self) -> str:
         """Get symbol of random cryptocurrency.
 
         :return: Symbol of cryptocurrency.
         """
         return self.random.choice(CRYPTOCURRENCY_ISO_CODES)
```

### Comparing `mimesis-7.1.0/mimesis/providers/food.py` & `mimesis-8.0.0/mimesis/providers/food.py`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/providers/generic.py` & `mimesis-8.0.0/mimesis/providers/generic.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,18 @@
 
         The list of result will be used in AbstractField to
         determine method's class.
 
         :return: List of attributes.
         """
         attributes = []
-        exclude = BaseProvider().__dict__.keys()
+        exclude = list(BaseProvider().__dict__.keys())
+        # Exclude locale explicitly because
+        # it is not a provider.
+        exclude.append("locale")
 
         for attr in self.__dict__:
             if attr not in exclude:
                 if attr.startswith("_"):
                     attribute = attr.replace("_", "", 1)
                     attributes.append(attribute)
                 else:
```

### Comparing `mimesis-7.1.0/mimesis/providers/hardware.py` & `mimesis-8.0.0/mimesis/providers/hardware.py`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/providers/internet.py` & `mimesis-8.0.0/mimesis/providers/internet.py`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/providers/numeric.py` & `mimesis-8.0.0/mimesis/providers/numeric.py`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/providers/path.py` & `mimesis-8.0.0/mimesis/providers/path.py`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/providers/payment.py` & `mimesis-8.0.0/mimesis/providers/payment.py`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/providers/person.py` & `mimesis-8.0.0/mimesis/providers/person.py`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/providers/science.py` & `mimesis-8.0.0/mimesis/providers/science.py`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/providers/text.py` & `mimesis-8.0.0/mimesis/providers/text.py`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/providers/transport.py` & `mimesis-8.0.0/mimesis/providers/transport.py`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/random.py` & `mimesis-8.0.0/mimesis/random.py`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/schema.py` & `mimesis-8.0.0/mimesis/schema.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,27 +3,28 @@
 import csv
 import json
 import pickle
 import re
 import typing as t
 import warnings
 
-from mimesis.exceptions import FieldError, SchemaError
+from mimesis.exceptions import FieldError, FieldsetError, SchemaError
 from mimesis.locales import Locale
+from mimesis.providers.base import BaseProvider
 from mimesis.providers.generic import Generic
 from mimesis.types import (
     JSON,
     CallableSchema,
     FieldCache,
     Key,
     MissingSeed,
     Seed,
 )
 
-__all__ = ["BaseField", "Field", "Schema"]
+__all__ = ["BaseField", "Field", "Fieldset", "Schema"]
 
 
 class BaseField:
     def __init__(
         self,
         locale: Locale = Locale.DEFAULT,
         seed: Seed = MissingSeed,
@@ -73,16 +74,17 @@
 
         :param name: The field name.
         :return: Callable object.
         :raise FieldError: When field is invalid.
         """
         for provider in dir(self._gen):
             provider = getattr(self._gen, provider)
-            if name in dir(provider):
-                return getattr(provider, name)
+            if isinstance(provider, BaseProvider):
+                if name in dir(provider):
+                    return getattr(provider, name)
 
         raise FieldError(name)
 
     def _lookup_method(self, name: str) -> t.Any:
         """Lookup method by the field name.
 
         :param name: The field name.
@@ -170,24 +172,89 @@
             for i in range(1000):
                 field = Field()
 
         You doing it **wrong**! It is a terrible idea that will lead to a memory leak.
 
         Forewarned is forearmed.
 
-    Example:
+    Here is usage example:
+
         >>> _ = Field()
         >>> _('username')
         Dogtag_1836
     """
 
     def __call__(self, *args: t.Any, **kwargs: t.Any) -> t.Any:
         return self.perform(*args, **kwargs)
 
 
+class Fieldset(BaseField):
+    """Greedy fieldset (evaluates immediately).
+
+    Works like a field, but returns a list of values.
+
+    Here is usage example:
+
+        >>> fieldset = Fieldset(i=100)
+        >>> fieldset('username')
+        ['pot_1821', 'vhs_1915', ..., 'reviewed_1849']
+
+    You may also specify the number of iterations by passing the **i** keyword
+    argument to the callable instance of fieldset:
+
+        >>> fieldset = Fieldset()
+        >>> fieldset('username', i=2)
+        ['pot_1821', 'vhs_1915']
+
+    When **i** is not specified, the reasonable default is used — **10**.
+
+    See "Field vs Fieldset" section of documentation for more details.
+
+    :cvar fieldset_default_iterations: Default iterations. Default is **10**.
+    :cvar fieldset_iterations_kwarg: Keyword argument for iterations. Default is **i**.
+    """
+
+    fieldset_default_iterations: int = 10
+    fieldset_iterations_kwarg: str = "i"
+
+    def __init__(self, *args: t.Any, **kwargs: t.Any) -> None:
+        """Initialize fieldset.
+
+        Accepts additional keyword argument **i** which is used
+        to specify the number of iterations.
+
+        The name of the keyword argument can be changed by
+        overriding **fieldset_iterations_kwarg** attribute of this class.
+        """
+        self._iterations = kwargs.pop(
+            self.fieldset_iterations_kwarg,
+            self.fieldset_default_iterations,
+        )
+        super().__init__(*args, **kwargs)
+
+    def __call__(self, *args: t.Any, **kwargs: t.Any) -> t.List[t.Any]:
+        """Perform fieldset.
+
+        :param args: Arguments for field.
+        :param kwargs: Keyword arguments for field.
+        :raises FieldsetError: If iterations less than 1.
+        :return: List of values.
+        """
+        min_iterations = 1
+        iterations = kwargs.pop(
+            self.fieldset_iterations_kwarg,
+            self._iterations,
+        )
+
+        if iterations < min_iterations:
+            raise FieldsetError()
+
+        return [self.perform(*args, **kwargs) for _ in range(iterations)]
+
+
 class Schema:
     """Class which return list of filled schemas."""
 
     _MIN_ITERATIONS_VALUE: t.ClassVar[int] = 1
 
     __slots__ = ("_schema",)
```

### Comparing `mimesis-7.1.0/mimesis/shortcuts.py` & `mimesis-8.0.0/mimesis/shortcuts.py`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/mimesis/types.py` & `mimesis-8.0.0/mimesis/types.py`

 * *Files identical despite different names*

### Comparing `mimesis-7.1.0/pyproject.toml` & `mimesis-8.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mimesis"
-version = "7.1.0"
+version = "8.0.0"
 description = "Mimesis: Fake Data Generator."
 authors = ["Isaak Uchakaev <likid.geimfari@gmail.com>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/lk-geimfari/mimesis"
 repository = "https://github.com/lk-geimfari/mimesis"
 documentation = "https://mimesis.name"
@@ -42,19 +42,19 @@
 ]
 exclude = [
     "mimesis/data/locale_template",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
+coverage = "^7.2.3"
+pytest-cov = "^4.0.0"
 
 [tool.poetry.group.dev.dependencies]
-codecov = "^2.1"
 pytest = "^7.2"
-pytest-cov = "^3.0"
 pytest-mock = "^3.10"
 requests = "^2.28"
 mypy = "^1.1"
 colorama = "^0.4.6"
 pygments = "^2.13"
 pytest-randomly = "^3.12"
 pytz = "^2023.3"
```

### Comparing `mimesis-7.1.0/PKG-INFO` & `mimesis-8.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mimesis
-Version: 7.1.0
+Version: 8.0.0
 Summary: Mimesis: Fake Data Generator.
 Home-page: https://github.com/lk-geimfari/mimesis
 License: MIT
 Keywords: data,datascince,database,dummy,fake,faker,fixtures,generate,mimesis,mock,populate,testing
 Author: Isaak Uchakaev
 Author-email: likid.geimfari@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -25,14 +25,16 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Utilities
+Requires-Dist: coverage (>=7.2.3,<8.0.0)
+Requires-Dist: pytest-cov (>=4.0.0,<5.0.0)
 Project-URL: Documentation, https://mimesis.name
 Project-URL: Repository, https://github.com/lk-geimfari/mimesis
 Description-Content-Type: text/x-rst
 
 Mimesis: The Fake Data Generator
 --------------------------------
```

