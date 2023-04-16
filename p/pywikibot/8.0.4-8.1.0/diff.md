# Comparing `tmp/pywikibot-8.0.4.tar.gz` & `tmp/pywikibot-8.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywikibot-8.0.4.tar", last modified: Thu Apr 13 11:27:17 2023, max compression
+gzip compressed data, was "pywikibot-8.1.0.tar", last modified: Sun Apr 16 15:00:32 2023, max compression
```

## Comparing `pywikibot-8.0.4.tar` & `pywikibot-8.1.0.tar`

### file list

```diff
@@ -1,311 +1,311 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 11:27:17.018679 pywikibot-8.0.4/
--rw-rw-rw-   0        0        0     4115 2023-04-10 16:20:49.000000 pywikibot-8.0.4/AUTHORS.rst
--rw-rw-rw-   0        0        0     1086 2023-04-10 16:20:49.000000 pywikibot-8.0.4/LICENSE
--rw-rw-rw-   0        0        0       40 2023-04-10 16:20:49.000000 pywikibot-8.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0    14465 2023-04-13 11:27:17.018679 pywikibot-8.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     5495 2023-04-10 16:20:49.000000 pywikibot-8.0.4/README.rst
--rw-rw-rw-   0        0        0     6057 2023-04-13 11:26:42.000000 pywikibot-8.0.4/make_dist.py
-drwxrwxrwx   0        0        0        0 2023-04-13 11:27:15.715347 pywikibot-8.0.4/pywikibot/
--rw-rw-rw-   0        0        0    55733 2023-04-13 10:49:37.000000 pywikibot-8.0.4/pywikibot/__init__.py
--rw-rw-rw-   0        0        0      794 2023-04-13 10:49:37.000000 pywikibot-8.0.4/pywikibot/__metadata__.py
--rw-rw-rw-   0        0        0     1886 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/_wbtypes.py
--rw-rw-rw-   0        0        0     4476 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/backports.py
--rw-rw-rw-   0        0        0    95911 2023-04-13 10:49:37.000000 pywikibot-8.0.4/pywikibot/bot.py
--rw-rw-rw-   0        0        0    21207 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/bot_choice.py
-drwxrwxrwx   0        0        0        0 2023-04-13 11:27:15.755242 pywikibot-8.0.4/pywikibot/comms/
--rw-rw-rw-   0        0        0      121 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/comms/__init__.py
--rw-rw-rw-   0        0        0    15749 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/comms/eventstreams.py
--rw-rw-rw-   0        0        0    19142 2023-04-13 10:49:37.000000 pywikibot-8.0.4/pywikibot/comms/http.py
--rw-rw-rw-   0        0        0    46157 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/config.py
--rw-rw-rw-   0        0        0    46135 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/cosmetic_changes.py
--rw-rw-rw-   0        0        0     2090 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/daemonize.py
-drwxrwxrwx   0        0        0        0 2023-04-13 11:27:15.793140 pywikibot-8.0.4/pywikibot/data/
--rw-rw-rw-   0        0        0      160 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 11:27:15.798128 pywikibot-8.0.4/pywikibot/data/api/
--rw-rw-rw-   0        0        0     3174 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/data/api/__init__.py
--rw-rw-rw-   0        0        0    41816 2023-04-10 17:33:59.000000 pywikibot-8.0.4/pywikibot/data/api/_generators.py
--rw-rw-rw-   0        0        0     7398 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/data/api/_optionset.py
--rw-rw-rw-   0        0        0    23233 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/data/api/_paraminfo.py
--rw-rw-rw-   0        0        0    53223 2023-04-13 10:49:37.000000 pywikibot-8.0.4/pywikibot/data/api/_requests.py
--rw-rw-rw-   0        0        0    14143 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/data/memento.py
--rw-rw-rw-   0        0        0     2919 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/data/mysql.py
--rw-rw-rw-   0        0        0     8969 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/data/sparql.py
--rw-rw-rw-   0        0        0     3970 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/data/wikistats.py
--rw-rw-rw-   0        0        0    96943 2023-04-13 10:49:37.000000 pywikibot-8.0.4/pywikibot/date.py
--rw-rw-rw-   0        0        0    24879 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/diff.py
--rw-rw-rw-   0        0        0     2054 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/echo.py
--rw-rw-rw-   0        0        0     7830 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/editor.py
--rw-rw-rw-   0        0        0    20031 2023-04-13 10:49:37.000000 pywikibot-8.0.4/pywikibot/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-04-13 11:27:16.027319 pywikibot-8.0.4/pywikibot/families/
--rw-rw-rw-   0        0        0      118 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/families/__init__.py
--rw-rw-rw-   0        0        0     4303 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/families/commons_family.py
--rw-rw-rw-   0        0        0      443 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/families/foundation_family.py
--rw-rw-rw-   0        0        0      463 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/families/i18n_family.py
--rw-rw-rw-   0        0        0      355 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/families/incubator_family.py
--rw-rw-rw-   0        0        0      662 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/families/lingualibre_family.py
--rw-rw-rw-   0        0        0      401 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/families/mediawiki_family.py
--rw-rw-rw-   0        0        0      593 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/families/meta_family.py
--rw-rw-rw-   0        0        0     1330 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/families/osm_family.py
--rw-rw-rw-   0        0        0      369 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/families/outreach_family.py
--rw-rw-rw-   0        0        0      361 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/families/species_family.py
--rw-rw-rw-   0        0        0      638 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/families/vikidia_family.py
--rw-rw-rw-   0        0        0     2418 2023-04-13 08:33:09.000000 pywikibot-8.0.4/pywikibot/families/wikibooks_family.py
--rw-rw-rw-   0        0        0     3782 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/families/wikidata_family.py
--rw-rw-rw-   0        0        0     1742 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/families/wikihow_family.py
--rw-rw-rw-   0        0        0     1009 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/families/wikimania_family.py
--rw-rw-rw-   0        0        0      777 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/families/wikimediachapter_family.py
--rw-rw-rw-   0        0        0     1825 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/families/wikinews_family.py
--rw-rw-rw-   0        0        0    10721 2023-04-13 08:33:09.000000 pywikibot-8.0.4/pywikibot/families/wikipedia_family.py
--rw-rw-rw-   0        0        0     2886 2023-04-13 08:33:09.000000 pywikibot-8.0.4/pywikibot/families/wikiquote_family.py
--rw-rw-rw-   0        0        0     5335 2023-04-13 08:33:09.000000 pywikibot-8.0.4/pywikibot/families/wikisource_family.py
--rw-rw-rw-   0        0        0      495 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/families/wikispore_family.py
--rw-rw-rw-   0        0        0      425 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/families/wikitech_family.py
--rw-rw-rw-   0        0        0     1150 2023-04-13 08:33:09.000000 pywikibot-8.0.4/pywikibot/families/wikiversity_family.py
--rw-rw-rw-   0        0        0     1027 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/families/wikivoyage_family.py
--rw-rw-rw-   0        0        0     3827 2023-04-13 08:33:09.000000 pywikibot-8.0.4/pywikibot/families/wiktionary_family.py
--rw-rw-rw-   0        0        0     2404 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/families/wowwiki_family.py
--rw-rw-rw-   0        0        0    37565 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/family.py
--rw-rw-rw-   0        0        0    33191 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/fixes.py
--rw-rw-rw-   0        0        0    20119 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/flow.py
--rw-rw-rw-   0        0        0    28565 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/i18n.py
--rw-rw-rw-   0        0        0     8343 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/interwiki_graph.py
--rw-rw-rw-   0        0        0    13245 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/logentries.py
--rw-rw-rw-   0        0        0    12508 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/logging.py
--rw-rw-rw-   0        0        0    22815 2023-04-10 16:39:25.000000 pywikibot-8.0.4/pywikibot/login.py
-drwxrwxrwx   0        0        0        0 2023-04-13 11:27:16.039289 pywikibot-8.0.4/pywikibot/page/
--rw-rw-rw-   0        0        0     2350 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/page/__init__.py
--rw-rw-rw-   0        0        0    86837 2023-04-13 10:49:37.000000 pywikibot-8.0.4/pywikibot/page/_basepage.py
--rw-rw-rw-   0        0        0    14617 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/page/_category.py
--rw-rw-rw-   0        0        0    19000 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/page/_collections.py
--rw-rw-rw-   0        0        0     2183 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/page/_decorators.py
--rw-rw-rw-   0        0        0    14648 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/page/_filepage.py
--rw-rw-rw-   0        0        0    29601 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/page/_links.py
--rw-rw-rw-   0        0        0     8515 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/page/_page.py
--rw-rw-rw-   0        0        0     2997 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/page/_revision.py
--rw-rw-rw-   0        0        0     4049 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/page/_toolforge.py
--rw-rw-rw-   0        0        0    16348 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/page/_user.py
--rw-rw-rw-   0        0        0    86179 2023-04-13 10:49:37.000000 pywikibot-8.0.4/pywikibot/page/_wikibase.py
-drwxrwxrwx   0        0        0        0 2023-04-13 11:27:16.076221 pywikibot-8.0.4/pywikibot/pagegenerators/
--rw-rw-rw-   0        0        0    28720 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/pagegenerators/__init__.py
--rw-rw-rw-   0        0        0    40342 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/pagegenerators/_factory.py
--rw-rw-rw-   0        0        0    19272 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/pagegenerators/_filters.py
--rw-rw-rw-   0        0        0    44438 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/pagegenerators/_generators.py
--rw-rw-rw-   0        0        0     3938 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/plural.py
--rw-rw-rw-   0        0        0    48779 2023-04-13 10:49:37.000000 pywikibot-8.0.4/pywikibot/proofreadpage.py
-drwxrwxrwx   0        0        0        0 2023-04-13 11:27:16.140020 pywikibot-8.0.4/pywikibot/scripts/
--rw-rw-rw-   0        0        0      882 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/scripts/__init__.py
--rw-rw-rw-   0        0        0    10348 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/scripts/generate_family_file.py
--rw-rw-rw-   0        0        0    19989 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/scripts/generate_user_files.py
-drwxrwxrwx   0        0        0        0 2023-04-13 11:27:16.147999 pywikibot-8.0.4/pywikibot/scripts/i18n/
--rw-rw-rw-   0        0        0      309 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 11:27:16.929915 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/
--rw-rw-rw-   0        0        0      166 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ab.json
--rw-rw-rw-   0        0        0      511 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/af.json
--rw-rw-rw-   0        0        0      121 2022-04-07 08:52:21.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/an.json
--rw-rw-rw-   0        0        0     1227 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ar.json
--rw-rw-rw-   0        0        0      131 2022-04-07 08:52:21.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/arc.json
--rw-rw-rw-   0        0        0     1042 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ast.json
--rw-rw-rw-   0        0        0      163 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/av.json
--rw-rw-rw-   0        0        0      150 2022-04-07 08:52:21.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/awa.json
--rw-rw-rw-   0        0        0      898 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/az.json
--rw-rw-rw-   0        0        0      982 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/azb.json
--rw-rw-rw-   0        0        0     1362 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ba.json
--rw-rw-rw-   0        0        0      210 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/bar.json
--rw-rw-rw-   0        0        0      989 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/bcc.json
--rw-rw-rw-   0        0        0     1491 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/be-tarask.json
--rw-rw-rw-   0        0        0      894 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/be.json
--rw-rw-rw-   0        0        0      535 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/bg.json
--rw-rw-rw-   0        0        0      203 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/bjn.json
--rw-rw-rw-   0        0        0      642 2023-04-06 12:04:37.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/bn.json
--rw-rw-rw-   0        0        0      179 2022-04-07 08:52:21.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/bo.json
--rw-rw-rw-   0        0        0     1048 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/br.json
--rw-rw-rw-   0        0        0      998 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/bs.json
--rw-rw-rw-   0        0        0     1198 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ca.json
--rw-rw-rw-   0        0        0      981 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ce.json
--rw-rw-rw-   0        0        0      768 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ckb.json
--rw-rw-rw-   0        0        0     1178 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/cs.json
--rw-rw-rw-   0        0        0     1013 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/csb.json
--rw-rw-rw-   0        0        0      995 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/cy.json
--rw-rw-rw-   0        0        0     1022 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/da.json
--rw-rw-rw-   0        0        0     1065 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/de.json
--rw-rw-rw-   0        0        0     1025 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/diq.json
--rw-rw-rw-   0        0        0     1647 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/el.json
--rw-rw-rw-   0        0        0     1027 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/en.json
--rw-rw-rw-   0        0        0     1121 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/eo.json
--rw-rw-rw-   0        0        0     1203 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/es.json
--rw-rw-rw-   0        0        0      333 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/et.json
--rw-rw-rw-   0        0        0     1043 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/eu.json
--rw-rw-rw-   0        0        0     1424 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/fa.json
--rw-rw-rw-   0        0        0      660 2022-04-15 15:42:25.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/fi.json
--rw-rw-rw-   0        0        0      812 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/fo.json
--rw-rw-rw-   0        0        0     1291 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/fr.json
--rw-rw-rw-   0        0        0      227 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/frp.json
--rw-rw-rw-   0        0        0      988 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/frr.json
--rw-rw-rw-   0        0        0       95 2022-04-07 08:52:21.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/fy.json
--rw-rw-rw-   0        0        0      104 2022-04-07 08:52:21.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ga.json
--rw-rw-rw-   0        0        0     1082 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/gl.json
--rw-rw-rw-   0        0        0      786 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/gsw.json
--rw-rw-rw-   0        0        0      711 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/hak.json
--rw-rw-rw-   0        0        0      858 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/haw.json
--rw-rw-rw-   0        0        0     1192 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/he.json
--rw-rw-rw-   0        0        0     1699 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/hi.json
--rw-rw-rw-   0        0        0      201 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/hr.json
--rw-rw-rw-   0        0        0      593 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/hsb.json
--rw-rw-rw-   0        0        0     1022 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/hu.json
--rw-rw-rw-   0        0        0      259 2022-04-15 15:42:25.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/hy.json
--rw-rw-rw-   0        0        0     1085 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ia.json
--rw-rw-rw-   0        0        0     1146 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/id.json
--rw-rw-rw-   0        0        0      205 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ie.json
--rw-rw-rw-   0        0        0      114 2022-04-07 08:52:21.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ig.json
--rw-rw-rw-   0        0        0      220 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ilo.json
--rw-rw-rw-   0        0        0     1011 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/io.json
--rw-rw-rw-   0        0        0      735 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/is.json
--rw-rw-rw-   0        0        0     1063 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/it.json
--rw-rw-rw-   0        0        0     1125 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ja.json
--rw-rw-rw-   0        0        0      196 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/jv.json
--rw-rw-rw-   0        0        0      581 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/kab.json
--rw-rw-rw-   0        0        0     1068 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/kk.json
--rw-rw-rw-   0        0        0     1381 2022-04-07 08:52:21.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/km.json
--rw-rw-rw-   0        0        0      993 2022-04-07 08:52:21.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/kn.json
--rw-rw-rw-   0        0        0     1140 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ko.json
--rw-rw-rw-   0        0        0     1409 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/krc.json
--rw-rw-rw-   0        0        0     1188 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ksh.json
--rw-rw-rw-   0        0        0      318 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ku.json
--rw-rw-rw-   0        0        0      331 2022-04-07 08:52:21.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ky.json
--rw-rw-rw-   0        0        0      100 2022-04-07 08:52:21.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/la.json
--rw-rw-rw-   0        0        0      988 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/lb.json
--rw-rw-rw-   0        0        0      209 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/li.json
--rw-rw-rw-   0        0        0      174 2022-04-07 08:52:21.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/lki.json
--rw-rw-rw-   0        0        0      963 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/lt.json
--rw-rw-rw-   0        0        0      691 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/lv.json
--rw-rw-rw-   0        0        0      752 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/map-bms.json
--rw-rw-rw-   0        0        0      967 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/mg.json
--rw-rw-rw-   0        0        0      673 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/min.json
--rw-rw-rw-   0        0        0     1353 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/mk.json
--rw-rw-rw-   0        0        0     1943 2022-04-28 20:36:36.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ml.json
--rw-rw-rw-   0        0        0      168 2022-04-07 08:52:21.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/mni.json
--rw-rw-rw-   0        0        0      267 2022-04-15 15:42:25.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/mr.json
--rw-rw-rw-   0        0        0      968 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ms.json
--rw-rw-rw-   0        0        0      203 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/mt.json
--rw-rw-rw-   0        0        0     1335 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/my.json
--rw-rw-rw-   0        0        0     1049 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/nan.json
--rw-rw-rw-   0        0        0     1003 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/nb.json
--rw-rw-rw-   0        0        0      983 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/nds-nl.json
--rw-rw-rw-   0        0        0      197 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/nds.json
--rw-rw-rw-   0        0        0     1562 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ne.json
--rw-rw-rw-   0        0        0      891 2022-04-07 08:52:21.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/new.json
--rw-rw-rw-   0        0        0     1037 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/nl.json
--rw-rw-rw-   0        0        0      232 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/nn.json
--rw-rw-rw-   0        0        0     1344 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/nqo.json
--rw-rw-rw-   0        0        0      148 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/nyn.json
--rw-rw-rw-   0        0        0      226 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/oc.json
--rw-rw-rw-   0        0        0      258 2022-04-07 08:52:21.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/olo.json
--rw-rw-rw-   0        0        0      154 2022-04-07 08:52:21.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/or.json
--rw-rw-rw-   0        0        0      216 2022-04-07 08:52:21.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/pa.json
--rw-rw-rw-   0        0        0      157 2023-04-06 12:04:37.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/pdc.json
--rw-rw-rw-   0        0        0      102 2022-04-07 08:52:21.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/pfl.json
--rw-rw-rw-   0        0        0     1011 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/pl.json
--rw-rw-rw-   0        0        0      870 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/pms.json
--rw-rw-rw-   0        0        0     1070 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/pt-br.json
--rw-rw-rw-   0        0        0     1187 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/pt.json
--rw-rw-rw-   0        0        0     1749 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/qqq.json
--rw-rw-rw-   0        0        0     1149 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ro.json
--rw-rw-rw-   0        0        0     1582 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ru.json
--rw-rw-rw-   0        0        0      149 2022-04-07 08:52:21.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/scn.json
--rw-rw-rw-   0        0        0      749 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/sco.json
--rw-rw-rw-   0        0        0      311 2022-04-07 08:52:21.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/sd.json
--rw-rw-rw-   0        0        0      551 2022-04-07 08:52:21.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/sh.json
--rw-rw-rw-   0        0        0      528 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/si.json
--rw-rw-rw-   0        0        0     1046 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/sk.json
--rw-rw-rw-   0        0        0      193 2023-04-06 12:04:37.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/skr-arab.json
--rw-rw-rw-   0        0        0     1078 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/sl.json
--rw-rw-rw-   0        0        0      127 2022-04-07 08:52:21.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/sms.json
--rw-rw-rw-   0        0        0      725 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/so.json
--rw-rw-rw-   0        0        0      452 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/sq.json
--rw-rw-rw-   0        0        0     1439 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/sr.json
--rw-rw-rw-   0        0        0      347 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/su.json
--rw-rw-rw-   0        0        0     1047 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/sv.json
--rw-rw-rw-   0        0        0      650 2022-04-07 08:52:21.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/sw.json
--rw-rw-rw-   0        0        0      124 2022-04-07 08:52:21.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/szl.json
--rw-rw-rw-   0        0        0      683 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ta.json
--rw-rw-rw-   0        0        0     1390 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/te.json
--rw-rw-rw-   0        0        0      101 2023-04-06 12:04:37.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/tg.json
--rw-rw-rw-   0        0        0     1414 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/th.json
--rw-rw-rw-   0        0        0      155 2023-04-06 12:04:37.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/tk.json
--rw-rw-rw-   0        0        0      219 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/tl.json
--rw-rw-rw-   0        0        0     1115 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/tly.json
--rw-rw-rw-   0        0        0     1159 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/tr.json
--rw-rw-rw-   0        0        0      316 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/tt.json
--rw-rw-rw-   0        0        0     1417 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/uk.json
--rw-rw-rw-   0        0        0      789 2022-04-28 20:36:36.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ur.json
--rw-rw-rw-   0        0        0      208 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/uz.json
--rw-rw-rw-   0        0        0      253 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/vec.json
--rw-rw-rw-   0        0        0      121 2022-04-07 08:52:22.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/vep.json
--rw-rw-rw-   0        0        0     1105 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/vi.json
--rw-rw-rw-   0        0        0      116 2022-04-07 08:52:22.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/vo.json
--rw-rw-rw-   0        0        0      218 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/war.json
--rw-rw-rw-   0        0        0      461 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/yi.json
--rw-rw-rw-   0        0        0      850 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/yue.json
--rw-rw-rw-   0        0        0     1084 2023-04-01 15:38:09.000000 pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/zh.json
--rw-rw-rw-   0        0        0     6093 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/scripts/login.py
--rw-rw-rw-   0        0        0     3246 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/scripts/preload_sites.py
--rw-rw-rw-   0        0        0     1791 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/scripts/shell.py
--rw-rw-rw-   0        0        0     3313 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/scripts/version.py
--rw-rw-rw-   0        0        0    18491 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/scripts/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-04-13 11:27:16.943879 pywikibot-8.0.4/pywikibot/site/
--rw-rw-rw-   0        0        0      744 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/site/__init__.py
--rw-rw-rw-   0        0        0   112319 2023-04-13 10:49:37.000000 pywikibot-8.0.4/pywikibot/site/_apisite.py
--rw-rw-rw-   0        0        0    15756 2023-04-13 10:49:37.000000 pywikibot-8.0.4/pywikibot/site/_basesite.py
--rw-rw-rw-   0        0        0    38276 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/site/_datasite.py
--rw-rw-rw-   0        0        0     4254 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/site/_decorators.py
--rw-rw-rw-   0        0        0    27978 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/site/_extensions.py
--rw-rw-rw-   0        0        0    92439 2023-04-13 10:49:37.000000 pywikibot-8.0.4/pywikibot/site/_generators.py
--rw-rw-rw-   0        0        0     3003 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/site/_interwikimap.py
--rw-rw-rw-   0        0        0    14558 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/site/_namespace.py
--rw-rw-rw-   0        0        0     1667 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/site/_obsoletesites.py
--rw-rw-rw-   0        0        0    14354 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/site/_siteinfo.py
--rw-rw-rw-   0        0        0     4703 2023-04-13 10:49:37.000000 pywikibot-8.0.4/pywikibot/site/_tokenwallet.py
--rw-rw-rw-   0        0        0    25321 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/site/_upload.py
--rw-rw-rw-   0        0        0    10800 2023-04-13 10:49:37.000000 pywikibot-8.0.4/pywikibot/site_detect.py
-drwxrwxrwx   0        0        0        0 2023-04-13 11:27:16.967813 pywikibot-8.0.4/pywikibot/specialbots/
--rw-rw-rw-   0        0        0      371 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/specialbots/__init__.py
--rw-rw-rw-   0        0        0     3109 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/specialbots/_unlink.py
--rw-rw-rw-   0        0        0    20247 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/specialbots/_upload.py
--rw-rw-rw-   0        0        0    84825 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/textlib.py
--rw-rw-rw-   0        0        0    12074 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/throttle.py
--rw-rw-rw-   0        0        0    15061 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/time.py
--rw-rw-rw-   0        0        0     3267 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/titletranslate.py
-drwxrwxrwx   0        0        0        0 2023-04-13 11:27:16.994741 pywikibot-8.0.4/pywikibot/tools/
--rw-rw-rw-   0        0        0    27088 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/tools/__init__.py
--rw-rw-rw-   0        0        0    25467 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/tools/_deprecate.py
--rw-rw-rw-   0        0        0     1205 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/tools/_logging.py
--rw-rw-rw-   0        0        0    22207 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/tools/_unidata.py
--rw-rw-rw-   0        0        0     3116 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/tools/chars.py
--rw-rw-rw-   0        0        0     8765 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/tools/collections.py
--rw-rw-rw-   0        0        0    11075 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/tools/djvu.py
--rw-rw-rw-   0        0        0     4021 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/tools/formatter.py
--rw-rw-rw-   0        0        0     9745 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/tools/itertools.py
--rw-rw-rw-   0        0        0     7334 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/tools/threading.py
-drwxrwxrwx   0        0        0        0 2023-04-13 11:27:17.016683 pywikibot-8.0.4/pywikibot/userinterfaces/
--rw-rw-rw-   0        0        0      870 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/userinterfaces/__init__.py
--rw-rw-rw-   0        0        0     1906 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/userinterfaces/_interface_base.py
--rw-rw-rw-   0        0        0     2687 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/userinterfaces/buffer_interface.py
--rw-rw-rw-   0        0        0    21724 2023-04-13 10:49:37.000000 pywikibot-8.0.4/pywikibot/userinterfaces/gui.py
--rw-rw-rw-   0        0        0      457 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/userinterfaces/terminal_interface.py
--rw-rw-rw-   0        0        0    24536 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/userinterfaces/terminal_interface_base.py
--rw-rw-rw-   0        0        0     2114 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/userinterfaces/terminal_interface_unix.py
--rw-rw-rw-   0        0        0     2012 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/userinterfaces/terminal_interface_win32.py
--rw-rw-rw-   0        0        0    90310 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/userinterfaces/transliteration.py
--rw-rw-rw-   0        0        0    16698 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/version.py
--rw-rw-rw-   0        0        0     7366 2023-04-10 16:20:49.000000 pywikibot-8.0.4/pywikibot/xmlreader.py
-drwxrwxrwx   0        0        0        0 2023-04-13 11:27:15.744272 pywikibot-8.0.4/pywikibot.egg-info/
--rw-rw-rw-   0        0        0    14465 2023-04-13 11:27:15.000000 pywikibot-8.0.4/pywikibot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    10447 2023-04-13 11:27:15.000000 pywikibot-8.0.4/pywikibot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 11:27:15.000000 pywikibot-8.0.4/pywikibot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-04-13 11:27:15.000000 pywikibot-8.0.4/pywikibot.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0     1228 2023-04-13 11:27:15.000000 pywikibot-8.0.4/pywikibot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-13 11:27:15.000000 pywikibot-8.0.4/pywikibot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 11:27:17.019676 pywikibot-8.0.4/setup.cfg
--rw-rw-rw-   0        0        0    13116 2023-04-13 08:00:35.000000 pywikibot-8.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-13 11:27:17.017712 pywikibot-8.0.4/tests/
--rw-rw-rw-   0        0        0     2792 2023-04-13 10:49:37.000000 pywikibot-8.0.4/tests/tests_tests.py
+drwxrwxrwx   0        0        0        0 2023-04-16 15:00:32.257337 pywikibot-8.1.0/
+-rw-rw-rw-   0        0        0     4115 2023-04-10 16:20:49.000000 pywikibot-8.1.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0     1086 2023-04-10 16:20:49.000000 pywikibot-8.1.0/LICENSE
+-rw-rw-rw-   0        0        0       40 2023-04-10 16:20:49.000000 pywikibot-8.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    15494 2023-04-16 15:00:32.257337 pywikibot-8.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5495 2023-04-10 16:20:49.000000 pywikibot-8.1.0/README.rst
+-rw-rw-rw-   0        0        0     6351 2023-04-16 15:00:25.000000 pywikibot-8.1.0/make_dist.py
+drwxrwxrwx   0        0        0        0 2023-04-16 15:00:30.905407 pywikibot-8.1.0/pywikibot/
+-rw-rw-rw-   0        0        0    55820 2023-04-14 09:45:27.000000 pywikibot-8.1.0/pywikibot/__init__.py
+-rw-rw-rw-   0        0        0      794 2023-04-16 13:54:05.000000 pywikibot-8.1.0/pywikibot/__metadata__.py
+-rw-rw-rw-   0        0        0     1886 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/_wbtypes.py
+-rw-rw-rw-   0        0        0     4476 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/backports.py
+-rw-rw-rw-   0        0        0    96117 2023-04-14 14:19:20.000000 pywikibot-8.1.0/pywikibot/bot.py
+-rw-rw-rw-   0        0        0    21207 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/bot_choice.py
+drwxrwxrwx   0        0        0        0 2023-04-16 15:00:30.956314 pywikibot-8.1.0/pywikibot/comms/
+-rw-rw-rw-   0        0        0      121 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/comms/__init__.py
+-rw-rw-rw-   0        0        0    15749 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/comms/eventstreams.py
+-rw-rw-rw-   0        0        0    19597 2023-04-14 09:45:27.000000 pywikibot-8.1.0/pywikibot/comms/http.py
+-rw-rw-rw-   0        0        0    46527 2023-04-14 14:19:20.000000 pywikibot-8.1.0/pywikibot/config.py
+-rw-rw-rw-   0        0        0    46135 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/cosmetic_changes.py
+-rw-rw-rw-   0        0        0     2090 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/daemonize.py
+drwxrwxrwx   0        0        0        0 2023-04-16 15:00:31.006224 pywikibot-8.1.0/pywikibot/data/
+-rw-rw-rw-   0        0        0      160 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 15:00:31.055135 pywikibot-8.1.0/pywikibot/data/api/
+-rw-rw-rw-   0        0        0     3174 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/data/api/__init__.py
+-rw-rw-rw-   0        0        0    41816 2023-04-14 14:19:36.000000 pywikibot-8.1.0/pywikibot/data/api/_generators.py
+-rw-rw-rw-   0        0        0     7398 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/data/api/_optionset.py
+-rw-rw-rw-   0        0        0    23233 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/data/api/_paraminfo.py
+-rw-rw-rw-   0        0        0    52510 2023-04-14 09:45:27.000000 pywikibot-8.1.0/pywikibot/data/api/_requests.py
+-rw-rw-rw-   0        0        0    14143 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/data/memento.py
+-rw-rw-rw-   0        0        0     2919 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/data/mysql.py
+-rw-rw-rw-   0        0        0     8969 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/data/sparql.py
+-rw-rw-rw-   0        0        0     3970 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/data/wikistats.py
+-rw-rw-rw-   0        0        0    96940 2023-04-14 09:45:27.000000 pywikibot-8.1.0/pywikibot/date.py
+-rw-rw-rw-   0        0        0    24879 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/diff.py
+-rw-rw-rw-   0        0        0     2054 2023-04-15 09:05:00.000000 pywikibot-8.1.0/pywikibot/echo.py
+-rw-rw-rw-   0        0        0     7830 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/editor.py
+-rw-rw-rw-   0        0        0    21221 2023-04-14 09:45:27.000000 pywikibot-8.1.0/pywikibot/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-04-16 15:00:31.287712 pywikibot-8.1.0/pywikibot/families/
+-rw-rw-rw-   0        0        0      118 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/families/__init__.py
+-rw-rw-rw-   0        0        0     4303 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/families/commons_family.py
+-rw-rw-rw-   0        0        0      443 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/families/foundation_family.py
+-rw-rw-rw-   0        0        0      463 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/families/i18n_family.py
+-rw-rw-rw-   0        0        0      355 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/families/incubator_family.py
+-rw-rw-rw-   0        0        0      662 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/families/lingualibre_family.py
+-rw-rw-rw-   0        0        0      401 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/families/mediawiki_family.py
+-rw-rw-rw-   0        0        0      593 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/families/meta_family.py
+-rw-rw-rw-   0        0        0     1330 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/families/osm_family.py
+-rw-rw-rw-   0        0        0      369 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/families/outreach_family.py
+-rw-rw-rw-   0        0        0      361 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/families/species_family.py
+-rw-rw-rw-   0        0        0      638 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/families/vikidia_family.py
+-rw-rw-rw-   0        0        0     2418 2023-04-16 13:54:05.000000 pywikibot-8.1.0/pywikibot/families/wikibooks_family.py
+-rw-rw-rw-   0        0        0     3782 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/families/wikidata_family.py
+-rw-rw-rw-   0        0        0     1742 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/families/wikihow_family.py
+-rw-rw-rw-   0        0        0     1009 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/families/wikimania_family.py
+-rw-rw-rw-   0        0        0      777 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/families/wikimediachapter_family.py
+-rw-rw-rw-   0        0        0     1825 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/families/wikinews_family.py
+-rw-rw-rw-   0        0        0    10730 2023-04-16 13:54:05.000000 pywikibot-8.1.0/pywikibot/families/wikipedia_family.py
+-rw-rw-rw-   0        0        0     2886 2023-04-16 13:54:05.000000 pywikibot-8.1.0/pywikibot/families/wikiquote_family.py
+-rw-rw-rw-   0        0        0     5335 2023-04-16 13:54:05.000000 pywikibot-8.1.0/pywikibot/families/wikisource_family.py
+-rw-rw-rw-   0        0        0      495 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/families/wikispore_family.py
+-rw-rw-rw-   0        0        0      425 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/families/wikitech_family.py
+-rw-rw-rw-   0        0        0     1150 2023-04-14 14:19:20.000000 pywikibot-8.1.0/pywikibot/families/wikiversity_family.py
+-rw-rw-rw-   0        0        0     1027 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/families/wikivoyage_family.py
+-rw-rw-rw-   0        0        0     3827 2023-04-16 13:54:05.000000 pywikibot-8.1.0/pywikibot/families/wiktionary_family.py
+-rw-rw-rw-   0        0        0     2404 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/families/wowwiki_family.py
+-rw-rw-rw-   0        0        0    37565 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/family.py
+-rw-rw-rw-   0        0        0    33191 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/fixes.py
+-rw-rw-rw-   0        0        0    20119 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/flow.py
+-rw-rw-rw-   0        0        0    30038 2023-04-14 14:19:20.000000 pywikibot-8.1.0/pywikibot/i18n.py
+-rw-rw-rw-   0        0        0     8343 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/interwiki_graph.py
+-rw-rw-rw-   0        0        0    13245 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/logentries.py
+-rw-rw-rw-   0        0        0    12508 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/logging.py
+-rw-rw-rw-   0        0        0    22781 2023-04-14 14:19:20.000000 pywikibot-8.1.0/pywikibot/login.py
+drwxrwxrwx   0        0        0        0 2023-04-16 15:00:31.407494 pywikibot-8.1.0/pywikibot/page/
+-rw-rw-rw-   0        0        0     2350 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/page/__init__.py
+-rw-rw-rw-   0        0        0    86912 2023-04-14 09:45:27.000000 pywikibot-8.1.0/pywikibot/page/_basepage.py
+-rw-rw-rw-   0        0        0    14617 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/page/_category.py
+-rw-rw-rw-   0        0        0    19000 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/page/_collections.py
+-rw-rw-rw-   0        0        0     2183 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/page/_decorators.py
+-rw-rw-rw-   0        0        0    14648 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/page/_filepage.py
+-rw-rw-rw-   0        0        0    29601 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/page/_links.py
+-rw-rw-rw-   0        0        0     8515 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/page/_page.py
+-rw-rw-rw-   0        0        0     2997 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/page/_revision.py
+-rw-rw-rw-   0        0        0     4049 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/page/_toolforge.py
+-rw-rw-rw-   0        0        0    16348 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/page/_user.py
+-rw-rw-rw-   0        0        0    86381 2023-04-15 09:05:00.000000 pywikibot-8.1.0/pywikibot/page/_wikibase.py
+drwxrwxrwx   0        0        0        0 2023-04-16 15:00:31.453410 pywikibot-8.1.0/pywikibot/pagegenerators/
+-rw-rw-rw-   0        0        0    29164 2023-04-14 16:24:14.000000 pywikibot-8.1.0/pywikibot/pagegenerators/__init__.py
+-rw-rw-rw-   0        0        0    40342 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/pagegenerators/_factory.py
+-rw-rw-rw-   0        0        0    19272 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/pagegenerators/_filters.py
+-rw-rw-rw-   0        0        0    44438 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/pagegenerators/_generators.py
+-rw-rw-rw-   0        0        0     3938 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/plural.py
+-rw-rw-rw-   0        0        0    48967 2023-04-14 09:45:27.000000 pywikibot-8.1.0/pywikibot/proofreadpage.py
+drwxrwxrwx   0        0        0        0 2023-04-16 15:00:31.516298 pywikibot-8.1.0/pywikibot/scripts/
+-rw-rw-rw-   0        0        0      882 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/scripts/__init__.py
+-rw-rw-rw-   0        0        0    11972 2023-04-16 09:28:42.000000 pywikibot-8.1.0/pywikibot/scripts/generate_family_file.py
+-rw-rw-rw-   0        0        0    19989 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/scripts/generate_user_files.py
+drwxrwxrwx   0        0        0        0 2023-04-16 15:00:31.523283 pywikibot-8.1.0/pywikibot/scripts/i18n/
+-rw-rw-rw-   0        0        0      309 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 15:00:31.938529 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/
+-rw-rw-rw-   0        0        0      166 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ab.json
+-rw-rw-rw-   0        0        0      511 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/af.json
+-rw-rw-rw-   0        0        0      121 2022-04-07 08:52:21.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/an.json
+-rw-rw-rw-   0        0        0     1227 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ar.json
+-rw-rw-rw-   0        0        0      131 2022-04-07 08:52:21.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/arc.json
+-rw-rw-rw-   0        0        0     1042 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ast.json
+-rw-rw-rw-   0        0        0      163 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/av.json
+-rw-rw-rw-   0        0        0      150 2022-04-07 08:52:21.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/awa.json
+-rw-rw-rw-   0        0        0      898 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/az.json
+-rw-rw-rw-   0        0        0      982 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/azb.json
+-rw-rw-rw-   0        0        0     1362 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ba.json
+-rw-rw-rw-   0        0        0      210 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/bar.json
+-rw-rw-rw-   0        0        0      989 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/bcc.json
+-rw-rw-rw-   0        0        0     1491 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/be-tarask.json
+-rw-rw-rw-   0        0        0      894 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/be.json
+-rw-rw-rw-   0        0        0      535 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/bg.json
+-rw-rw-rw-   0        0        0      203 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/bjn.json
+-rw-rw-rw-   0        0        0      642 2023-04-06 12:04:37.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/bn.json
+-rw-rw-rw-   0        0        0      179 2022-04-07 08:52:21.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/bo.json
+-rw-rw-rw-   0        0        0     1048 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/br.json
+-rw-rw-rw-   0        0        0      998 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/bs.json
+-rw-rw-rw-   0        0        0     1198 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ca.json
+-rw-rw-rw-   0        0        0      981 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ce.json
+-rw-rw-rw-   0        0        0      768 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ckb.json
+-rw-rw-rw-   0        0        0     1178 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/cs.json
+-rw-rw-rw-   0        0        0     1013 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/csb.json
+-rw-rw-rw-   0        0        0      995 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/cy.json
+-rw-rw-rw-   0        0        0     1022 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/da.json
+-rw-rw-rw-   0        0        0     1065 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/de.json
+-rw-rw-rw-   0        0        0     1025 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/diq.json
+-rw-rw-rw-   0        0        0     1647 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/el.json
+-rw-rw-rw-   0        0        0     1027 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/en.json
+-rw-rw-rw-   0        0        0     1121 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/eo.json
+-rw-rw-rw-   0        0        0     1203 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/es.json
+-rw-rw-rw-   0        0        0      333 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/et.json
+-rw-rw-rw-   0        0        0     1043 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/eu.json
+-rw-rw-rw-   0        0        0     1424 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/fa.json
+-rw-rw-rw-   0        0        0      660 2022-04-15 15:42:25.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/fi.json
+-rw-rw-rw-   0        0        0      812 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/fo.json
+-rw-rw-rw-   0        0        0     1291 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/fr.json
+-rw-rw-rw-   0        0        0      227 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/frp.json
+-rw-rw-rw-   0        0        0      988 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/frr.json
+-rw-rw-rw-   0        0        0       95 2022-04-07 08:52:21.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/fy.json
+-rw-rw-rw-   0        0        0      104 2022-04-07 08:52:21.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ga.json
+-rw-rw-rw-   0        0        0     1082 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/gl.json
+-rw-rw-rw-   0        0        0      786 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/gsw.json
+-rw-rw-rw-   0        0        0      711 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/hak.json
+-rw-rw-rw-   0        0        0      858 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/haw.json
+-rw-rw-rw-   0        0        0     1192 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/he.json
+-rw-rw-rw-   0        0        0     1699 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/hi.json
+-rw-rw-rw-   0        0        0      201 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/hr.json
+-rw-rw-rw-   0        0        0      593 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/hsb.json
+-rw-rw-rw-   0        0        0     1022 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/hu.json
+-rw-rw-rw-   0        0        0      259 2022-04-15 15:42:25.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/hy.json
+-rw-rw-rw-   0        0        0     1085 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ia.json
+-rw-rw-rw-   0        0        0     1146 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/id.json
+-rw-rw-rw-   0        0        0      205 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ie.json
+-rw-rw-rw-   0        0        0      114 2022-04-07 08:52:21.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ig.json
+-rw-rw-rw-   0        0        0      220 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ilo.json
+-rw-rw-rw-   0        0        0     1011 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/io.json
+-rw-rw-rw-   0        0        0      735 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/is.json
+-rw-rw-rw-   0        0        0     1063 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/it.json
+-rw-rw-rw-   0        0        0     1125 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ja.json
+-rw-rw-rw-   0        0        0      196 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/jv.json
+-rw-rw-rw-   0        0        0      581 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/kab.json
+-rw-rw-rw-   0        0        0     1068 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/kk.json
+-rw-rw-rw-   0        0        0     1381 2022-04-07 08:52:21.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/km.json
+-rw-rw-rw-   0        0        0      993 2022-04-07 08:52:21.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/kn.json
+-rw-rw-rw-   0        0        0     1140 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ko.json
+-rw-rw-rw-   0        0        0     1409 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/krc.json
+-rw-rw-rw-   0        0        0     1188 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ksh.json
+-rw-rw-rw-   0        0        0      318 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ku.json
+-rw-rw-rw-   0        0        0      331 2022-04-07 08:52:21.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ky.json
+-rw-rw-rw-   0        0        0      100 2022-04-07 08:52:21.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/la.json
+-rw-rw-rw-   0        0        0      988 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/lb.json
+-rw-rw-rw-   0        0        0      209 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/li.json
+-rw-rw-rw-   0        0        0      174 2022-04-07 08:52:21.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/lki.json
+-rw-rw-rw-   0        0        0      963 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/lt.json
+-rw-rw-rw-   0        0        0      691 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/lv.json
+-rw-rw-rw-   0        0        0      752 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/map-bms.json
+-rw-rw-rw-   0        0        0      967 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/mg.json
+-rw-rw-rw-   0        0        0      673 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/min.json
+-rw-rw-rw-   0        0        0     1353 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/mk.json
+-rw-rw-rw-   0        0        0     1943 2022-04-28 20:36:36.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ml.json
+-rw-rw-rw-   0        0        0      168 2022-04-07 08:52:21.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/mni.json
+-rw-rw-rw-   0        0        0      267 2022-04-15 15:42:25.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/mr.json
+-rw-rw-rw-   0        0        0      968 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ms.json
+-rw-rw-rw-   0        0        0      203 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/mt.json
+-rw-rw-rw-   0        0        0     1335 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/my.json
+-rw-rw-rw-   0        0        0     1049 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/nan.json
+-rw-rw-rw-   0        0        0     1003 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/nb.json
+-rw-rw-rw-   0        0        0      983 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/nds-nl.json
+-rw-rw-rw-   0        0        0      197 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/nds.json
+-rw-rw-rw-   0        0        0     1562 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ne.json
+-rw-rw-rw-   0        0        0      891 2022-04-07 08:52:21.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/new.json
+-rw-rw-rw-   0        0        0     1037 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/nl.json
+-rw-rw-rw-   0        0        0      232 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/nn.json
+-rw-rw-rw-   0        0        0     1344 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/nqo.json
+-rw-rw-rw-   0        0        0      148 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/nyn.json
+-rw-rw-rw-   0        0        0      226 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/oc.json
+-rw-rw-rw-   0        0        0      258 2022-04-07 08:52:21.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/olo.json
+-rw-rw-rw-   0        0        0      154 2022-04-07 08:52:21.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/or.json
+-rw-rw-rw-   0        0        0      216 2022-04-07 08:52:21.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/pa.json
+-rw-rw-rw-   0        0        0      157 2023-04-06 12:04:37.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/pdc.json
+-rw-rw-rw-   0        0        0      102 2022-04-07 08:52:21.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/pfl.json
+-rw-rw-rw-   0        0        0     1011 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/pl.json
+-rw-rw-rw-   0        0        0      870 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/pms.json
+-rw-rw-rw-   0        0        0     1070 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/pt-br.json
+-rw-rw-rw-   0        0        0     1187 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/pt.json
+-rw-rw-rw-   0        0        0     1749 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/qqq.json
+-rw-rw-rw-   0        0        0     1149 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ro.json
+-rw-rw-rw-   0        0        0     1582 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ru.json
+-rw-rw-rw-   0        0        0      149 2022-04-07 08:52:21.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/scn.json
+-rw-rw-rw-   0        0        0      749 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/sco.json
+-rw-rw-rw-   0        0        0      311 2022-04-07 08:52:21.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/sd.json
+-rw-rw-rw-   0        0        0      551 2022-04-07 08:52:21.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/sh.json
+-rw-rw-rw-   0        0        0      528 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/si.json
+-rw-rw-rw-   0        0        0     1046 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/sk.json
+-rw-rw-rw-   0        0        0      193 2023-04-06 12:04:37.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/skr-arab.json
+-rw-rw-rw-   0        0        0     1078 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/sl.json
+-rw-rw-rw-   0        0        0      127 2022-04-07 08:52:21.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/sms.json
+-rw-rw-rw-   0        0        0      725 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/so.json
+-rw-rw-rw-   0        0        0      452 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/sq.json
+-rw-rw-rw-   0        0        0     1439 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/sr.json
+-rw-rw-rw-   0        0        0      347 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/su.json
+-rw-rw-rw-   0        0        0     1047 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/sv.json
+-rw-rw-rw-   0        0        0      650 2022-04-07 08:52:21.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/sw.json
+-rw-rw-rw-   0        0        0      124 2022-04-07 08:52:21.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/szl.json
+-rw-rw-rw-   0        0        0      683 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ta.json
+-rw-rw-rw-   0        0        0     1390 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/te.json
+-rw-rw-rw-   0        0        0      101 2023-04-06 12:04:37.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/tg.json
+-rw-rw-rw-   0        0        0     1414 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/th.json
+-rw-rw-rw-   0        0        0      155 2023-04-06 12:04:37.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/tk.json
+-rw-rw-rw-   0        0        0      219 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/tl.json
+-rw-rw-rw-   0        0        0     1115 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/tly.json
+-rw-rw-rw-   0        0        0     1159 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/tr.json
+-rw-rw-rw-   0        0        0      316 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/tt.json
+-rw-rw-rw-   0        0        0     1417 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/uk.json
+-rw-rw-rw-   0        0        0      789 2022-04-28 20:36:36.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ur.json
+-rw-rw-rw-   0        0        0      208 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/uz.json
+-rw-rw-rw-   0        0        0      253 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/vec.json
+-rw-rw-rw-   0        0        0      121 2022-04-07 08:52:22.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/vep.json
+-rw-rw-rw-   0        0        0     1105 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/vi.json
+-rw-rw-rw-   0        0        0      116 2022-04-07 08:52:22.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/vo.json
+-rw-rw-rw-   0        0        0      218 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/war.json
+-rw-rw-rw-   0        0        0      461 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/yi.json
+-rw-rw-rw-   0        0        0      850 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/yue.json
+-rw-rw-rw-   0        0        0     1084 2023-04-01 15:38:09.000000 pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/zh.json
+-rw-rw-rw-   0        0        0     6093 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/scripts/login.py
+-rw-rw-rw-   0        0        0     3246 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/scripts/preload_sites.py
+-rw-rw-rw-   0        0        0     1791 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/scripts/shell.py
+-rw-rw-rw-   0        0        0     3313 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/scripts/version.py
+-rw-rw-rw-   0        0        0    18491 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/scripts/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-04-16 15:00:32.061304 pywikibot-8.1.0/pywikibot/site/
+-rw-rw-rw-   0        0        0      744 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/site/__init__.py
+-rw-rw-rw-   0        0        0   112500 2023-04-14 09:45:27.000000 pywikibot-8.1.0/pywikibot/site/_apisite.py
+-rw-rw-rw-   0        0        0    15864 2023-04-15 09:05:00.000000 pywikibot-8.1.0/pywikibot/site/_basesite.py
+-rw-rw-rw-   0        0        0    38276 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/site/_datasite.py
+-rw-rw-rw-   0        0        0     4254 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/site/_decorators.py
+-rw-rw-rw-   0        0        0    27978 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/site/_extensions.py
+-rw-rw-rw-   0        0        0    93641 2023-04-14 16:24:14.000000 pywikibot-8.1.0/pywikibot/site/_generators.py
+-rw-rw-rw-   0        0        0     3003 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/site/_interwikimap.py
+-rw-rw-rw-   0        0        0    14558 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/site/_namespace.py
+-rw-rw-rw-   0        0        0     1667 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/site/_obsoletesites.py
+-rw-rw-rw-   0        0        0    14354 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/site/_siteinfo.py
+-rw-rw-rw-   0        0        0     4868 2023-04-14 09:45:27.000000 pywikibot-8.1.0/pywikibot/site/_tokenwallet.py
+-rw-rw-rw-   0        0        0    25321 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/site/_upload.py
+-rw-rw-rw-   0        0        0    11231 2023-04-16 10:49:33.000000 pywikibot-8.1.0/pywikibot/site_detect.py
+drwxrwxrwx   0        0        0        0 2023-04-16 15:00:32.085649 pywikibot-8.1.0/pywikibot/specialbots/
+-rw-rw-rw-   0        0        0      371 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/specialbots/__init__.py
+-rw-rw-rw-   0        0        0     3109 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/specialbots/_unlink.py
+-rw-rw-rw-   0        0        0    20247 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/specialbots/_upload.py
+-rw-rw-rw-   0        0        0    84825 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/textlib.py
+-rw-rw-rw-   0        0        0    12074 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/throttle.py
+-rw-rw-rw-   0        0        0    15061 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/time.py
+-rw-rw-rw-   0        0        0     3267 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/titletranslate.py
+drwxrwxrwx   0        0        0        0 2023-04-16 15:00:32.175486 pywikibot-8.1.0/pywikibot/tools/
+-rw-rw-rw-   0        0        0    27088 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/tools/__init__.py
+-rw-rw-rw-   0        0        0    25467 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/tools/_deprecate.py
+-rw-rw-rw-   0        0        0     1205 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/tools/_logging.py
+-rw-rw-rw-   0        0        0    22207 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/tools/_unidata.py
+-rw-rw-rw-   0        0        0     3116 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/tools/chars.py
+-rw-rw-rw-   0        0        0     8765 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/tools/collections.py
+-rw-rw-rw-   0        0        0    11075 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/tools/djvu.py
+-rw-rw-rw-   0        0        0     4021 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/tools/formatter.py
+-rw-rw-rw-   0        0        0     9745 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/tools/itertools.py
+-rw-rw-rw-   0        0        0     7334 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/tools/threading.py
+drwxrwxrwx   0        0        0        0 2023-04-16 15:00:32.246357 pywikibot-8.1.0/pywikibot/userinterfaces/
+-rw-rw-rw-   0        0        0      870 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/userinterfaces/__init__.py
+-rw-rw-rw-   0        0        0     1906 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/userinterfaces/_interface_base.py
+-rw-rw-rw-   0        0        0     2687 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/userinterfaces/buffer_interface.py
+-rw-rw-rw-   0        0        0    22100 2023-04-14 09:45:27.000000 pywikibot-8.1.0/pywikibot/userinterfaces/gui.py
+-rw-rw-rw-   0        0        0      457 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/userinterfaces/terminal_interface.py
+-rw-rw-rw-   0        0        0    24536 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/userinterfaces/terminal_interface_base.py
+-rw-rw-rw-   0        0        0     2114 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/userinterfaces/terminal_interface_unix.py
+-rw-rw-rw-   0        0        0     2012 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/userinterfaces/terminal_interface_win32.py
+-rw-rw-rw-   0        0        0    90310 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/userinterfaces/transliteration.py
+-rw-rw-rw-   0        0        0    16698 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/version.py
+-rw-rw-rw-   0        0        0     7366 2023-04-10 16:20:49.000000 pywikibot-8.1.0/pywikibot/xmlreader.py
+drwxrwxrwx   0        0        0        0 2023-04-16 15:00:30.933357 pywikibot-8.1.0/pywikibot.egg-info/
+-rw-rw-rw-   0        0        0    15494 2023-04-16 15:00:30.000000 pywikibot-8.1.0/pywikibot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    10447 2023-04-16 15:00:30.000000 pywikibot-8.1.0/pywikibot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 15:00:30.000000 pywikibot-8.1.0/pywikibot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-04-16 15:00:30.000000 pywikibot-8.1.0/pywikibot.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0     1228 2023-04-16 15:00:30.000000 pywikibot-8.1.0/pywikibot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-16 15:00:30.000000 pywikibot-8.1.0/pywikibot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-16 15:00:32.257337 pywikibot-8.1.0/setup.cfg
+-rw-rw-rw-   0        0        0    13116 2023-04-15 09:02:53.000000 pywikibot-8.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 15:00:32.255340 pywikibot-8.1.0/tests/
+-rw-rw-rw-   0        0        0     2814 2023-04-14 09:45:27.000000 pywikibot-8.1.0/tests/tests_tests.py
```

### Comparing `pywikibot-8.0.4/AUTHORS.rst` & `pywikibot-8.1.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/LICENSE` & `pywikibot-8.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/PKG-INFO` & `pywikibot-8.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywikibot
-Version: 8.0.4
+Version: 8.1.0
 Summary: Python MediaWiki Bot Framework
 Home-page: https://www.mediawiki.org/wiki/Manual:Pywikibot
 Download-URL: https://pywikibot.toolforge.org/
 Maintainer: The Pywikibot team
 Maintainer-email: pywikibot@lists.wikimedia.org
 License: MIT License
 Project-URL: Documentation, https://doc.wikimedia.org/pywikibot/stable/
@@ -257,22 +257,39 @@
 
 Roadmap
 =======
 
 Current release
 ---------------
 
-* L10N Updates
-* Minimal needed mwparserfromhell was decreased to 0.5.2 (T326498, T327600)
-* No longer lazy load password cookies (T271858, T326779, T329132, T330488, T331315)
+* generate_family_filescript was improved (T334775)
+* A ``quiet`` parameter was added to APISite.preloadpages()
+  which is True by default
+* Fix getting HTTPStatus enum in site_detect check_response (T334728)
+* Do not show a logging in message if password is entered (T178061)
+* Enable preleading ``Bot:`` prefix with twtranslate messages (T161459)
+* Disable command.log if -nolog option is given (T334381)
+* Guess the last needed token key if the token is not found (T334288)
+* Show parameters with APIError (T333957)
+* Raise exceptions.NoSiteLinkErrorinstead of exceptions.NoPageErrorwhen sitelink
+  is missing in ItemPage.getSitelink()(T332341)
+* exceptions.ClientErrorwas added
+* Raise exceptions.NoPageErrorwhen deleting a missing Page (T332924)
+* ``text`` parameter of proofreadpage.PagesTagParserhas a default value
+* L10N updates
+* Ignore talk pages with APISite.watched_pages()(T330806)
+* Load page info when creating a page if not updated previously (T330980)
+* Improve flush exception logging
 
 
 Deprecations
 ------------
 
+* 8.1.0: Dependency of exceptions.NoSiteLinkErrorfrom exceptions.NoPageErrorwill be removed
+* 8.1.0: ``exceptions.Server414Error`` is deprecated in favour of exceptions.Client414Error
 * 8.0.0: Timestamp.clone()method is deprecated
   in favour of ``Timestamp.replace()`` method.
 * 8.0.0: family.Family.maximum_GET_lengthmethod is deprecated in favour of
   config.maximum_GET_length(T325957)
 * 8.0.0: ``addOnly`` parameter of textlib.replaceLanguageLinksand
   textlib.replaceCategoryLinksare deprecated in favour of ``add_only``
 * 8.0.0: textlib.TimeStripperregex attributes ``ptimeR``, ``ptimeznR``, ``pyearR``, ``pmonthR``,
```

### Comparing `pywikibot-8.0.4/README.rst` & `pywikibot-8.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/make_dist.py` & `pywikibot-8.1.0/make_dist.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,75 +1,86 @@
 #!/usr/bin/env python3
-"""Script to create a new distribution.
+"""Script to create a new distribution. Requires Python 3.7+.
 
 The following options are supported:
 
 -help      Print documentation of this file and of setup.py
 
 -local     Install the distribution as a local site-package. If a
            Pywikibot package is already there, it will be uninstalled
-           first.
+           first. Clears old dist folders first.
 
 -remote    Upload the package to pypi. This cannot be done if the
-           Pywikibot version is a development release.
+           Pywikibot version is a development release.  Clears old dist
+           folders first.
 
--clear     Clear old dist folders
+-clear     Clear old dist folders and leave. Does not create a
+           distribution.
 
--upgrade   Upgrade distribution packages pip, setuptools, wheel and twine
-           first
-
--nodist    Do not create a distribution. Useful to -clear or -upgrade only.
+-upgrade   Upgrade distribution packages pip, setuptools, wheel and
+           twine first
 
 Usage::
 
     [pwb] make_dist [options]
 
 .. versionadded:: 7.3
 .. versionchanged:: 7.4
 
    - updates pip, setuptools, wheel and twine packages first
    - installs pre-releases over stable versions
    - also creates built distribution together with source distribution
-   - `-upgrade` option was added
+   - *-upgrade* option was added
 
 .. versionchanged:: 7.5
 
-   - `clear` option was added
-   - `nodist` option was added
+   - *clear* option was added
+   - *nodist* option was added
+
+.. versionchanged:: 8.1
+   Python 3.7+ required because *dataclasses* module is used.
+   *nodist* option was removed, *clear* option does not create a
+   distribution. *local* and *remote* option clears old distributions
+   first.
 """
 #
 # (C) Pywikibot team, 2022-2023
 #
 # Distributed under the terms of the MIT license.
 #
 import abc
 import shutil
 import sys
+from dataclasses import dataclass, field
 from pathlib import Path
 from subprocess import check_call, run
 
 import setup
 from pywikibot import __version__, error, info, input_yn, warning
 from pywikibot.backports import Tuple
 
 
+@dataclass
 class SetupBase(abc.ABC):
 
     """Setup distribution base class.
 
     .. versionadded:: 8.0
+    .. versionchanged:: 8.1
+       *dataclass* is used.
     """
 
-    def __init__(self, local, remote, clear, upgrade, nodist) -> None:
-        """Initializer."""
-        self.local = local
-        self.remote = remote
-        self.clear = clear
-        self.upgrade = upgrade
-        self.nodist = nodist
+    local: bool
+    remote: bool
+    clear: bool
+    upgrade: bool
+    folder: Path = field(init=False)
+
+    def __post_init__(self) -> None:
+        """Post-init initializer."""
         self.folder = Path().resolve()
 
     def clear_old_dist(self) -> None:  # pragma: no cover
         """Delete old dist folders.
 
         .. versionadded:: 7.5
         """
@@ -90,19 +101,18 @@
     def run(self) -> None:  # pragma: no cover
         """Run the installer script."""
         if self.upgrade:
             check_call('python -m pip install --upgrade pip', shell=True)
             check_call(
                 'pip install --upgrade setuptools wheel twine ', shell=True)
 
-        if self.clear:
+        if self.local or self.remote or self.clear:
             self.clear_old_dist()
-
-        if self.nodist:
-            return
+            if self.clear:
+                return
 
         self.copy_files()
         try:
             setup.main()  # create a new package
         except SystemExit as e:
             error(e)
             return
@@ -177,25 +187,21 @@
         info(setup.__doc__)
         sys.exit()
 
     local = '-local' in sys.argv
     remote = '-remote' in sys.argv
     clear = '-clear' in sys.argv
     upgrade = '-upgrade' in sys.argv
-    nodist = '-nodist' in sys.argv
-
-    if nodist:
-        local, remote = False, False
 
     if remote and 'dev' in __version__:
         warning('Distribution must not be a developmental release to upload.')
         remote = False
 
-    sys.argv = [sys.argv[0], 'sdist']#, 'bdist_wheel']
-    return local, remote, clear, upgrade, nodist
+    sys.argv = [sys.argv[0], 'sdist', 'bdist_wheel']
+    return local, remote, clear, upgrade
 
 
 def main() -> None:  # pragma: no cover
     """Script entry point."""
     args = handle_args()
     SetupPywikibot(*args).run()
```

### Comparing `pywikibot-8.0.4/pywikibot/__init__.py` & `pywikibot-8.1.0/pywikibot/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -705,14 +705,17 @@
         return self.FORMATSTR.format(self.year, self.month, self.day,
                                      self.hour, self.minute, self.second)
 
     def toTimestamp(self, timezone_aware: bool = False) -> Timestamp:
         """
         Convert the data to a pywikibot.Timestamp.
 
+        .. versionchanged:: 8.0.1
+           *timezone_aware* parameter was added.
+
         :param timezone_aware: Whether the timezone should be passed to
             the Timestamp object.
         :raises ValueError: instance value cannot be represented using
             Timestamp
         """
         if self.year <= 0:
             raise ValueError('You cannot turn BC dates into a Timestamp')
```

### Comparing `pywikibot-8.0.4/pywikibot/__metadata__.py` & `pywikibot-8.1.0/pywikibot/__metadata__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # Distributed under the terms of the MIT license.
 #
 from time import strftime
 
 
 __name__ = 'pywikibot'
-__version__ = '8.0.4'
+__version__ = '8.1.0'
 __description__ = 'Python MediaWiki Bot Framework'
 __maintainer__ = 'The Pywikibot team'
 __maintainer_email__ = 'pywikibot@lists.wikimedia.org'
 __license__ = 'MIT License'
 __url__ = 'https://www.mediawiki.org/wiki/Manual:Pywikibot'
 __download_url__ = 'https://pywikibot.toolforge.org/'
 __copyright__ = '(C) Pywikibot team, 2003-' + strftime('%Y')
```

### Comparing `pywikibot-8.0.4/pywikibot/_wbtypes.py` & `pywikibot-8.1.0/pywikibot/_wbtypes.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/backports.py` & `pywikibot-8.1.0/pywikibot/backports.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/bot.py` & `pywikibot-8.1.0/pywikibot/bot.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,14 +224,15 @@
 -log              Enable the log file, using the default filename
                   '{}-bot.log'
                   Logs will be stored in the logs subdirectory.
 
 -log:xyz          Enable the log file, using 'xyz' as the filename.
 
 -nolog            Disable the log file (if it is enabled by default).
+                  Also disable command.log.
 
 -maxlag           Sets a new maxlag parameter to a number of seconds.
                   Defer bot edits during periods of database server lag.
                   Default is set by config.py
 
 -putthrottle:n    Set the minimum time (in seconds) the bot will wait
 -pt:n             between saving pages.
@@ -884,14 +885,16 @@
        *-cosmetic_changes* and *-cc* may be set directly instead of
        toggling the value. Refer :func:`tools.strtobool` for valid values.
     .. versionchanged:: 7.7
        *-config* global option was added.
     .. versionchanged:: 8.0
        Short site value can be given if site code is equal to family
        like ``-site:meta``.
+    .. versionchanged:: 8.1
+       ``-nolog`` option also discards command.log.
 
     :param args: Command line arguments. If None,
         :meth:`pywikibot.argvu<userinterfaces._interface_base.ABUIC.argvu>`
         is used which is a copy of ``sys.argv``
     :param do_help: Handle parameter '-help' to show help and invoke sys.exit
     :return: list of arguments not recognised globally
     """
@@ -907,14 +910,15 @@
 
     # get the name of the module calling this function. This is
     # required because the -help option loads the module's docstring and
     # because the module name will be used for the filename of the log.
     module_name = calledModuleName() or 'terminal-interface'
     non_global_args = []
     username = None
+    commandlog = True
     do_help_val: Union[bool, str, None] = None if do_help else False
     assert args is not None
     for arg in args:
         option, _, value = arg.partition(':')
         if do_help_val is not False and option == '-help':
             do_help_val = value or True
         # these are handled by config.py
@@ -935,14 +939,15 @@
             config.put_throttle = float(value)
         elif option == '-log':
             if module_name not in config.log:
                 config.log.append(module_name)
             if value:
                 config.logfilename = value
         elif option == '-nolog':
+            commandlog = False
             config.log = []
         elif option in ('-cosmeticchanges', '-cc'):
             config.cosmetic_changes = (strtobool(value) if value
                                        else not config.cosmetic_changes)
             output('NOTE: option cosmetic_changes is {}\n'
                    .format(config.cosmetic_changes))
         elif option == '-simulate':
@@ -1004,15 +1009,16 @@
         if calledModuleName() == 'wrapper':
             pywikibot._sites.clear()
 
     if username:
         config.usernames[config.family][config.mylang] = username
 
     init_handlers()
-    writeToCommandLogFile()
+    if commandlog:
+        writeToCommandLogFile()
 
     if config.verbose_output:
         pywikibot.info('Python ' + sys.version)
 
     if do_help_val:
         show_help(show_global=do_help_val == 'global')
         sys.exit(0)
```

### Comparing `pywikibot-8.0.4/pywikibot/bot_choice.py` & `pywikibot-8.1.0/pywikibot/bot_choice.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/comms/eventstreams.py` & `pywikibot-8.1.0/pywikibot/comms/eventstreams.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/comms/http.py` & `pywikibot-8.1.0/pywikibot/comms/http.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,29 +30,30 @@
 #
 # Distributed under the terms of the MIT license.
 #
 import atexit
 import codecs
 import re
 import sys
+import traceback
 from contextlib import suppress
 from http import HTTPStatus, cookiejar
 from string import Formatter
 from typing import Optional, Union
 from urllib.parse import quote, urlparse
 from warnings import warn
 
 import requests
 
 import pywikibot
 from pywikibot import config, tools
 from pywikibot.backports import Tuple
 from pywikibot.exceptions import (
+    Client414Error,
     FatalServerError,
-    Server414Error,
     Server504Error,
     ServerError,
 )
 from pywikibot.logging import critical, debug, error, log, warning
 from pywikibot.tools import file_mode_checker
 
 
@@ -104,22 +105,38 @@
 #: global :class:`PywikibotCookieJar` instance.
 cookie_jar = PywikibotCookieJar()
 #: global :class:`requests.Session`.
 session = requests.Session()
 session.cookies = cookie_jar
 
 
-# Prepare flush on quit
 def flush() -> None:  # pragma: no cover
-    """Close the session object. This is called when the module terminates."""
+    """Close the session object. This is called when the module terminates.
+
+    .. versionchanged:: 8.1
+       log the traceback and show the exception value in the critical
+       message
+    """
     log('Closing network session.')
     session.close()
 
     if hasattr(sys, 'last_type'):
-        critical(f'Exiting due to uncaught exception {sys.last_type}')
+        log(
+            ''.join(
+                traceback.format_exception(
+                    sys.last_type,
+                    value=sys.last_value,
+                    tb=sys.last_traceback
+                )
+            )
+        )
+        critical(
+            f'Exiting due to uncaught exception {sys.last_type.__name__}: '
+            f'{sys.last_value}'
+        )
 
     log('Network session closed.')
 
 
 atexit.register(flush)
 
 USER_AGENT_PRODUCTS = {
@@ -312,15 +329,15 @@
     if isinstance(response, Exception):
         with suppress(Exception):
             # request exception may contain response and request attribute
             error('An error occurred for uri ' + response.request.url)
         raise response from None
 
     if response.status_code == HTTPStatus.REQUEST_URI_TOO_LONG:
-        raise Server414Error('Too long GET request')
+        raise Client414Error(HTTPStatus(response.status_code).description)
 
     if response.status_code == HTTPStatus.GATEWAY_TIMEOUT:
         raise Server504Error('Server {} timed out'
                              .format(urlparse(response.url).netloc))
 
     if (not response.ok
             and response.status_code >= HTTPStatus.INTERNAL_SERVER_ERROR):
```

### Comparing `pywikibot-8.0.4/pywikibot/config.py` & `pywikibot-8.1.0/pywikibot/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -237,14 +237,22 @@
 password_file = None
 
 # edit summary to use if not supplied by bot script
 # WARNING: this should NEVER be used in practice, ALWAYS supply a more
 #          relevant summary for bot edits
 default_edit_summary = 'Pywikibot ' + pwb_version
 
+# Edit summary prefix
+# if a str, always use this as summary prefix e.g. 'Bot:' for all sites
+# if True, always use a summary prefix from i18n
+# if False, never use a summary prefix
+# if None, the i18n summary prefix is used for botflag accounts only
+# NOTE: this feature is not yet implemented for all scripts
+bot_prefix_summary: Union[bool, str, None] = None
+
 # What permissions to use to set private files to it
 # such as password file.
 #
 # stat.S_IRWXU 0o700 mask for owner permissions
 # stat.S_IRUSR 0o400 read permission for owner
 # stat.S_IWUSR 0o200 write permission for owner
 # stat.S_IXUSR 0o100 execute permission for owner
```

### Comparing `pywikibot-8.0.4/pywikibot/cosmetic_changes.py` & `pywikibot-8.1.0/pywikibot/cosmetic_changes.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/daemonize.py` & `pywikibot-8.1.0/pywikibot/daemonize.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/data/api/__init__.py` & `pywikibot-8.1.0/pywikibot/data/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/data/api/_generators.py` & `pywikibot-8.1.0/pywikibot/data/api/_generators.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/data/api/_optionset.py` & `pywikibot-8.1.0/pywikibot/data/api/_optionset.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/data/api/_paraminfo.py` & `pywikibot-8.1.0/pywikibot/data/api/_paraminfo.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/data/api/_requests.py` & `pywikibot-8.1.0/pywikibot/data/api/_requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,19 +21,19 @@
 from warnings import warn
 
 import pywikibot
 from pywikibot import config
 from pywikibot.backports import Callable, Dict, Match, Tuple, removeprefix
 from pywikibot.comms import http
 from pywikibot.exceptions import (
+    Client414Error,
     Error,
     FatalServerError,
     MaxlagTimeoutError,
     NoUsernameError,
-    Server414Error,
     Server504Error,
     SiteDefinitionError,
     TimeoutError,
 )
 from pywikibot.login import LoginStatus
 from pywikibot.textlib import removeDisabledParts, removeHTMLParts
 from pywikibot.tools import PYTHON_VERSION
@@ -179,16 +179,16 @@
                action=paraminfo if the action requires a POST.
         :param parameters: The parameters used for the request to the API.
         :type parameters: dict
         :param kwargs: The parameters used for the request to the API.
         """
         if site is None:
             self.site = pywikibot.Site()
-            warn('Request() invoked without a site; setting to {}'
-                 .format(self.site), RuntimeWarning, 2)
+            warn(f'Request() invoked without a site; setting to {self.site}',
+                 RuntimeWarning, 2)
         else:
             self.site = site
 
         self.mime = mime
         if isinstance(mime, bool):
             raise TypeError('mime param in api.Request() must not be boolean')
 
@@ -235,21 +235,20 @@
         if self.write:
             try:
                 username = self.site.userinfo['name']
             except KeyError:
                 raise Error('API write action attempted without user name')
 
             if 'anon' in self.site.userinfo:
-                raise Error("API write action attempted as IP '{}'"
-                            .format(username))
+                raise Error(f'API write action attempted as IP {username!r}')
 
             if not self.site.user() or self.site.username() != username:
                 pywikibot.warning(
-                    'API write action by unexpected username {} commenced.\n'
-                    'userinfo: {!r}'.format(username, self.site.userinfo))
+                    f'API write action by unexpected username {username} '
+                    f'commenced.\nuserinfo: {self.site.userinfo!r}')
 
         # Make sure user is logged in
         if self.write:
             pywikibot.debug('Adding user assertion')
             self['assert'] = 'user'
 
     @classmethod
@@ -297,16 +296,16 @@
 
         args = set()
         for super_cls in inspect.getmro(cls):
             if not super_cls.__name__.endswith('Request'):
                 break
             args |= set(inspect.getfullargspec(super_cls.__init__).args)
         else:
-            raise ValueError('Request was not a super class of '
-                             '{!r}'.format(cls))
+            raise ValueError(f'Request was not a super class of {cls!r}')
+
         args -= {'self'}
         old_kwargs = set(kwargs)
         # all kwargs defined above but not in args indicate 'kwargs' mode
         if old_kwargs - args:
             # Move all kwargs into parameters
             parameters = {name: value for name, value in kwargs.items()
                           if name not in args or name == 'parameters'}
@@ -339,17 +338,16 @@
 
         All other datatypes are converted to string.
         """
         if isinstance(value, datetime.datetime):
             return value.strftime(pywikibot.Timestamp.ISO8601Format)
         if isinstance(value, pywikibot.page.BasePage):
             if value.site != self.site:
-                raise RuntimeError(
-                    'value.site {!r} is different from Request.site {!r}'
-                    .format(value.site, self.site))
+                raise RuntimeError(f'value.site {value.site!r} is different '
+                                   f'from Request.site {self.site!r}')
             return value.title(with_section=False)
         return str(value)
 
     def __getitem__(self, key):
         """Implement dict interface."""
         return self._params[key]
 
@@ -448,15 +446,15 @@
             self['wrap'] = ''
 
         if config.maxlag:
             self._params.setdefault('maxlag', [str(config.maxlag)])
         self._params.setdefault('format', ['json'])
         if self['format'] != ['json']:
             raise TypeError(
-                "Query format '{}' cannot be parsed.".format(self['format']))
+                f'Query format {self["format"]!r} cannot be parsed.')
 
         self.__defaulted = True  # skipcq: PTC-W0037
 
     def _encoded_items(self) -> Dict[str, Union[str, bytes]]:
         """
         Build a dict of params with minimal encoding needed for the site.
 
@@ -492,16 +490,16 @@
             try:
                 value.encode('ascii')
             except UnicodeError:
                 try:
                     value = value.encode(self.site.encoding())
                 except Exception:
                     pywikibot.error(
-                        "_encoded_items: '{}' could not be encoded as '{}':"
-                        ' {!r}'.format(key, self.site.encoding(), value))
+                        f'_encoded_items: {key!r} could not be encoded as '
+                        f'{self.site.encoding()!r}: {value!r}')
             assert key.encode('ascii')
             assert isinstance(key, str)
             params[key] = value
         return params
 
     def _http_param_string(self):
         """
@@ -519,17 +517,16 @@
         """Return a string representation."""
         return unquote(self.site.scriptpath()
                        + '/api.php?'
                        + self._http_param_string())
 
     def __repr__(self) -> str:
         """Return internal representation."""
-        return '{}.{}<{}->{!r}>'.format(self.__class__.__module__,
-                                        self.__class__.__name__,
-                                        self.site, str(self))
+        cls = type(self)
+        return f"{cls.__module__}.{cls.__name__}<{self.site}->'{self}'>"
 
     def _simulate(self, action):
         """Simulate action."""
         if action and config.simulate and (
                 self.write or action in config.actions_to_block):
             pywikibot.info(
                 f'<<black;yellow>>SIMULATION: {action} action blocked.')
@@ -665,17 +662,16 @@
 
             if use_get:
                 uri = f'{uri}?{paramstring}'
                 body = None
             else:
                 body = paramstring
 
-        pywikibot.debug('API request to {} (uses get: {}):\n'
-                        'Headers: {!r}\nURI: {!r}\nBody: {!r}'
-                        .format(self.site, use_get, headers, uri, body))
+        pywikibot.debug(f'API request to {self.site} (uses get: {use_get}):\n'
+                        f'Headers: {headers!r}\nURI: {uri!r}\nBody: {body!r}')
         return use_get, uri, body, headers
 
     def _http_request(self, use_get: bool, uri: str, data, headers,
                       paramstring) -> tuple:
         """Get or post a http request with exception handling.
 
         :return: a tuple containing requests.Response object from
@@ -683,21 +679,21 @@
         """
         try:
             response = http.request(self.site, uri=uri,
                                     method='GET' if use_get else 'POST',
                                     data=data, headers=headers)
         except Server504Error:
             pywikibot.log('Caught HTTP 504 error; retrying')
-        except Server414Error:
+        except Client414Error:
             if use_get:
                 pywikibot.log('Caught HTTP 414 error; retrying')
                 use_get = False
             else:
-                pywikibot.warning('Caught HTTP 414 error, although not '
-                                  'using GET.')
+                pywikibot.warning(
+                    'Caught HTTP 414 error, although not using GET.')
                 raise
         except (ConnectionError, FatalServerError):
             # This error is not going to be fixed by just waiting
             pywikibot.error(traceback.format_exc())
             raise
         # TODO: what other exceptions can occur here?
         except Exception:
@@ -737,16 +733,16 @@
 {text}
 """
 
             # Do not retry for AutoFamily but raise a SiteDefinitionError
             # Note: family.AutoFamily is a function to create that class
             if self.site.family.__class__.__name__ == 'AutoFamily':
                 pywikibot.debug(msg)
-                raise SiteDefinitionError('Invalid AutoFamily({!r})'
-                                          .format(self.site.family.domain))
+                raise SiteDefinitionError(
+                    f'Invalid AutoFamily({self.site.family.domain!r})')
 
             if not self.json_warning:  # warn only once
                 pywikibot.warning(msg)
                 self.json_warning = True
 
             # there might also be an overflow, so try a smaller limit
             for param in self._params:
@@ -759,30 +755,29 @@
         else:
             return result or {}
         self.wait()
         return None
 
     def _relogin(self, message: str = '') -> None:
         """Force re-login and inform user."""
-        pywikibot.error('{}{}Forcing re-login.'.format(message,
-                                                       ' ' if message else ''))
+        message += ' Forcing re-login.'
+        pywikibot.error(f'{message.strip()}')
         self.site._relogin()
 
     def _userinfo_query(self, result) -> bool:
         """Handle userinfo query."""
         if self.action == 'query' and 'userinfo' in result.get('query', ()):
             # if we get passed userinfo in the query result, we can confirm
             # that we are logged in as the correct user. If this is not the
             # case, force a re-login.
             username = result['query']['userinfo']['name']
             if (self.site.user() is not None and self.site.user() != username
                     and self.site._loginstatus != LoginStatus.IN_PROGRESS):
-                message = ("Logged in as '{actual}' instead of '{expected}'."
-                           .format(actual=username, expected=self.site.user()))
-                self._relogin(message)
+                self._relogin(f'Logged in as {username!r} instead of '
+                              f'{self.site.user()!r}.')
                 return True
         return False
 
     def _handle_warnings(self, result: Dict[str, Any]) -> bool:
         """Handle warnings; return True to retry request, False to resume.
 
         .. versionchanged:: 7.2
@@ -797,27 +792,27 @@
                 continue
             if '*' in warning:
                 text = warning['*']
             elif 'html' in warning:
                 # bug T51978
                 text = warning['html']['*']
             else:
-                pywikibot.warning('API warning ({}) of unknown format: {}'
-                                  .format(mod, warning))
+                pywikibot.warning(
+                    f'API warning ({mod}) of unknown format: {warning}')
                 continue
 
             # multiple warnings are in text separated by a newline
             for single_warning in text.splitlines():
                 if (not callable(self._warning_handler)
                         or not self._warning_handler(mod, single_warning)):
                     handled = self._default_warning_handler(mod,
                                                             single_warning)
                     if handled is None:
-                        pywikibot.warning('API warning ({}): {}'
-                                          .format(mod, single_warning))
+                        pywikibot.warning(
+                            f'API warning ({mod}): {single_warning}')
                     else:
                         retry = retry or handled
         return retry
 
     def _default_warning_handler(self, mode: str, msg: str) -> Optional[bool]:
         """A default warning handler to handle specific warnings.
 
@@ -891,20 +886,17 @@
                                'ReadOnlyError',  # T61227
                                'readonly',  # T154011
                                ]
 
         pywikibot.error('Detected MediaWiki API exception {}{}'
                         .format(e, '; retrying' if retry else '; raising'))
         param_repr = str(self._params)
-        pywikibot.log('MediaWiki exception {} details:\n'
-                      '          query=\n{}\n'
-                      '          response=\n{}'
-                      .format(class_name,
-                              pprint.pformat(param_repr),
-                              result))
+        pywikibot.log(f'MediaWiki exception {class_name} details:\n'
+                      f'          query=\n{pprint.pformat(param_repr)}\n'
+                      f'          response=\n{result}')
         if not retry:
             raise e
 
         self.wait()
         return True
 
     def _ratelimited(self) -> None:
@@ -931,29 +923,28 @@
         <pywikibot.site._tokenwallet.TokenWallet.update_tokens>` method
         to update the bunch of tokens and continue loop in :meth:`submit`.
         """
         if code != 'badtoken':  # Other code not handled here
             return False
 
         if self.site._loginstatus == LoginStatus.IN_PROGRESS:
-            pywikibot.log('Login status: {}'
-                          .format(self.site._loginstatus.name))
+            pywikibot.log(f'Login status: {self.site._loginstatus.name}')
             return False
 
         # invalidate superior wiki cookies (T224712)
         pywikibot.data.api._invalidate_superior_cookies(self.site.family)
         # update tokens
         tokens = self.site.tokens.update_tokens(self._params['token'])
         self._params['token'] = tokens
         return True
 
     def submit(self) -> dict:
         """Submit a query and parse the response.
 
-        .. versionchanged:: 8.0.4
+        .. versionchanged:: 8.1
            in addition to *readapidenied* also try to login when API
            response is *notloggedin*.
 
         :return: a dict containing data retrieved from api.php
         """
         self._add_defaults()
         use_get = self._use_get()
@@ -1052,21 +1043,19 @@
                 self.site.login()
                 continue
 
             if self._bad_token(code):
                 continue
 
             if 'mwoauth-invalid-authorization' in code:
+                msg = f'OAuth authentication for {self.site}: {info}'
                 if 'Nonce already used' in info:
-                    pywikibot.error(
-                        'Retrying failed OAuth authentication for {}: {}'
-                        .format(self.site, info))
+                    pywikibot.error(f'Retrying failed {msg}')
                     continue
-                raise NoUsernameError('Failed OAuth authentication for {}: {}'
-                                      .format(self.site, info))
+                raise NoUsernameError(f'Failed {msg}')
             if code == 'cirrussearch-too-busy-error':  # T170647
                 self.wait()
                 continue
 
             if code in ('search-title-disabled', 'search-text-disabled'):
                 prefix = 'gsr' if 'gsrsearch' in self._params else 'sr'
                 del self._params[prefix + 'what']
@@ -1086,19 +1075,21 @@
                 else:  # not logged in; show the IP
                     uinfo = self.site.userinfo
                     error['current user'] = uinfo['name']
 
             # raise error
             try:
                 param_repr = str(self._params)
-                pywikibot.log('API Error: query=\n{}'
-                              .format(pprint.pformat(param_repr)))
+                pywikibot.log(
+                    f'API Error: query=\n{pprint.pformat(param_repr)}')
                 pywikibot.log(f'           response=\n{result}')
 
-                raise pywikibot.exceptions.APIError(**error)
+                args = {'param': body} if body else {}
+                args.update(error)
+                raise pywikibot.exceptions.APIError(**args)
             except TypeError:
                 raise RuntimeError(result)
 
         msg = 'Maximum retries attempted due to maxlag without success.'
         if os.environ.get('PYWIKIBOT_TEST_RUNNING', '0') == '1':
             import unittest
             raise unittest.SkipTest(msg)
@@ -1112,16 +1103,15 @@
             raise TimeoutError('Maximum retries attempted without success.')
 
         # double the next wait, but do not exceed config.retry_max seconds
         delay = delay or self.retry_wait
         delay *= 2 ** (self.current_retries - 1)
         delay = min(delay, config.retry_max)
 
-        pywikibot.warning('Waiting {:.1f} seconds before retrying.'
-                          .format(delay))
+        pywikibot.warning(f'Waiting {delay:.1f} seconds before retrying.')
         pywikibot.sleep(delay)
 
 
 class CachedRequest(Request):
 
     """Cached request."""
 
@@ -1190,15 +1180,15 @@
 
         if login_status >= LoginStatus.AS_USER:
             # This uses the format of Page.__repr__, without performing
             # config.console_encoding as done by Page.__repr__.
             # The returned value can't be encoded to anything other than
             # ascii otherwise it creates an exception when _create_file_name()
             # tries to encode it as utf-8.
-            user_key = 'User(User:{})'.format(self.site.userinfo['name'])
+            user_key = f'User(User:{self.site.userinfo["name"]})'
         else:
             user_key = repr(LoginStatus(LoginStatus.NOT_LOGGED_IN))
 
         request_key = repr(sorted(self._encoded_items().items()))
         return f'{self.site!r}{user_key}{request_key}'
 
     def _create_file_name(self) -> str:
```

### Comparing `pywikibot-8.0.4/pywikibot/data/memento.py` & `pywikibot-8.1.0/pywikibot/data/memento.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/data/mysql.py` & `pywikibot-8.1.0/pywikibot/data/mysql.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/data/sparql.py` & `pywikibot-8.1.0/pywikibot/data/sparql.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/data/wikistats.py` & `pywikibot-8.1.0/pywikibot/data/wikistats.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/date.py` & `pywikibot-8.1.0/pywikibot/date.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 """Date data and manipulation module."""
 #
-# (C) Pywikibot team, 2003-2022
+# (C) Pywikibot team, 2003-2023
 #
 # Distributed under the terms of the MIT license.
 #
 import calendar
 import datetime
 import re
 from collections import abc, defaultdict
 from contextlib import suppress
 from functools import singledispatch
 from string import digits as _decimalDigits  # noqa: N812
 from typing import Optional, Union
 
-import pywikibot.site
 from pywikibot import Site
 from pywikibot.backports import (
     Any,
     Callable,
     Dict,
     Iterator,
     List,
     Mapping,
     Pattern,
     Sequence,
     Tuple,
 )
+from pywikibot.site import BaseSite
 from pywikibot.textlib import NON_LATIN_DIGITS
 from pywikibot.tools import first_lower, first_upper
 
 
 #
 # Different collections of well known formats
 #
@@ -1966,15 +1966,15 @@
             else:
                 title = first_upper(title)
             return getAutoFormat(lang, title, ignoreFirstLetterCase=False)
     return None, None
 
 
 def format_date(month: int, day: int,
-                lang: Union[None, str, 'pywikibot.site.BaseSite'] = None,
+                lang: Union[None, str, BaseSite] = None,
                 year: int = 2000) -> str:
     """Format a date localized to given lang.
 
     :param month: month in range of 1..12
     :param day: day of month in range of 1..31
     :param lang: a site object or language key. Defaults to current site.
     :param year: year for which the date is to be formatted. always 29 will be
```

### Comparing `pywikibot-8.0.4/pywikibot/diff.py` & `pywikibot-8.1.0/pywikibot/diff.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/echo.py` & `pywikibot-8.1.0/pywikibot/echo.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/editor.py` & `pywikibot-8.1.0/pywikibot/editor.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/exceptions.py` & `pywikibot-8.1.0/pywikibot/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,28 +6,31 @@
     Exception
      +-- Error
           +-- APIError
           |    +-- APIMWError
           |    +-- UploadError
           +-- AutoblockUserError
           +-- CaptchaError
+          +-- ClientError
+          |    +-- Client414Error
           +-- InvalidTitleError
           +-- NoUsernameError
           +-- PageInUseError
           +-- PageRelatedError
           |    +-- CircularRedirectError
           |    +-- InterwikiRedirectPageError
           |    +-- IsNotRedirectPageError
           |    +-- IsRedirectPageError
           |    +-- NoMoveTargetError
           |    +-- NoPageError
           |    +-- NotEmailableError
           |    +-- PageLoadRelatedError
           |    |    +-- InconsistentTitleError
           |    |    +-- InvalidPageError
+          |    |    +-- NoSiteLinkError
           |    +-- PageSaveRelatedError
           |    |    +-- EditConflictError
           |    |    |    +-- ArticleExistsConflictError
           |    |    |    +-- PageCreatedConflictError
           |    |    |    +-- PageDeletedConflictError
           |    |    +-- LockedPageError
           |    |    |    +-- LockedNoPageError
@@ -37,15 +40,14 @@
           |    |    +-- SpamblacklistError
           |    |    +-- TitleblacklistError
           |    |    +-- AbuseFilterDisallowedError
           |    +-- UnsupportedPageError
           +-- SectionError
           +-- ServerError
           |    +-- FatalServerError
-          |    +-- Server414Error
           |    +-- Server504Error
           +-- SiteDefinitionError
           |    +-- UnknownFamilyError
           |    +-- UnknownSiteError
           +-- TimeoutError
           |    +-- MaxlagTimeoutError
           +-- TranslationError
@@ -64,25 +66,26 @@
 
     RuntimeWarning
      +-- NotImplementedWarning
 
 
 Error: Base class, all exceptions should the subclass of this class.
 
-  - NoUsernameError: Username is not in user config file, or it is invalid.
+  - CaptchaError: Captcha is asked and config.solve_captcha == False
+  - ClientError: A problem with the client request
   - AutoblockUserError: requested action on a virtual autoblock user not valid
-  - TranslationError: no language translation found
-  - UserRightsError: insufficient rights for requested action
   - InvalidTitleError: Invalid page title
-  - CaptchaError: Captcha is asked and config.solve_captcha == False
-  - i18n.TranslationError: i18n/l10n message not available
+  - NoUsernameError: Username is not in user config file, or it is invalid.
   - PageInUseError: Page cannot be reserved due to a lock
+  - SectionError: The section specified by # does not exist
+  - TranslationError: no language translation found
   - UnknownExtensionError: Extension is not defined for this site
+  - UserRightsError: insufficient rights for requested action
   - VersionParseError: failed to parse version information
-  - SectionError: The section specified by # does not exist
+  - i18n.TranslationError: i18n/l10n message not available
 
 APIError: wiki API returned an error
 
   - APIMWError: MediaWiki internal exception
   - UploadError: upload failed
 
 SiteDefinitionError: Site loading problem
@@ -100,14 +103,15 @@
   - InterwikiRedirectPageError: Page is a redirect to another site
   - InvalidPageError: Page is invalid e.g. without history
   - NotEmailableError: The target user has disabled email
   - NoMoveTargetError: An expected move target page does not exist
 
 PageLoadRelatedError: any exception which happens while loading a Page.
   - InconsistentTitleError: Page receives a title inconsistent with query
+  - NoSiteLinkError: ItemPage has no sitelink to given language
 
 PageSaveRelatedError: page exceptions within the save operation on a Page
 
   - AbuseFilterDisallowedError: AbuseFilter disallowed
   - SpamblacklistError: MediaWiki spam filter detected a blacklisted URL
   - TitleblacklistError: MediaWiki detected a blacklisted page title
   - OtherPageSaveError: misc. other save related exception.
@@ -156,25 +160,29 @@
 .. versionchanged:: 6.0
    exceptions were renamed and are ending with "Error".
 
 .. versionchanged:: 7.0
    All Pywikibot Error exceptions must be imported from
    ``pywikibot.exceptions``. Deprecated exceptions identifiers were
    removed.
+
+.. versionchanged:: 8.1
+   ``Server414Error`` class is deprecated; use :class:`Client414Error`
+   instead.
 """
 #
-# (C) Pywikibot team, 2008-2022
+# (C) Pywikibot team, 2008-2023
 #
 # Distributed under the terms of the MIT license.
 #
 import re
 from typing import Any, Optional, Union
 
 import pywikibot
-from pywikibot.tools import issue_deprecation_warning
+from pywikibot.tools import ModuleDeprecationWrapper, issue_deprecation_warning
 from pywikibot.tools._deprecate import _NotImplementedWarning
 
 
 class NotImplementedWarning(_NotImplementedWarning):
 
     """Feature that is no longer implemented."""
 
@@ -386,14 +394,34 @@
         :param actual: title obtained by query
 
         """
         self.message = f"Query on {{}} returned data on '{actual}'"
         super().__init__(page)
 
 
+class NoSiteLinkError(PageLoadRelatedError, NoPageError):
+
+    """ItemPage has no sitelink to the given language.
+
+    .. versionadded:: 8.1
+    .. deprecated:: 8.1
+       :exc:`NoPageError` dependency.
+    """
+
+    def __init__(self, page: 'pywikibot.page.ItemPage', lang: str) -> None:
+        """Initializer.
+
+        :param page: ItemPage that caused the exception
+        :param lang: language code of the queried sitelink
+
+        """
+        self.message = f'Item {{}} has no sitelink to language {lang!r}'
+        super().__init__(page)
+
+
 class SiteDefinitionError(Error):
 
     """Site does not exist."""
 
 
 class UnknownSiteError(SiteDefinitionError):
 
@@ -572,14 +600,30 @@
 class TitleblacklistError(PageSaveRelatedError):
 
     """Page save failed because MediaWiki detected a blacklisted page title."""
 
     message = 'Page {} is title-blacklisted.'
 
 
+class ClientError(Error):
+
+    """Got unexpected server response due to client issue.
+
+    .. versionadded:: 8.1
+    """
+
+
+class Client414Error(ClientError):
+
+    """Server returned with HTTP 414 code.
+
+    .. versionadded:: 8.1
+    """
+
+
 class ServerError(Error):
 
     """Got unexpected server response."""
 
 
 class FatalServerError(ServerError):
 
@@ -587,19 +631,14 @@
 
 
 class Server504Error(ServerError):
 
     """Server timed out with HTTP 504 code."""
 
 
-class Server414Error(ServerError):
-
-    """Server returned with HTTP 414 code."""
-
-
 class CaptchaError(Error):
 
     """Captcha is asked and config.solve_captcha == False."""
 
 
 class AutoblockUserError(Error):
 
@@ -677,7 +716,12 @@
 
     """Request failed with a timeout error."""
 
 
 class MaxlagTimeoutError(TimeoutError):
 
     """Request failed with a maxlag timeout error."""
+
+
+wrapper = ModuleDeprecationWrapper(__name__)
+wrapper.add_deprecated_attr(
+    'Server414Error', Client414Error, since='8.1.0')
```

### Comparing `pywikibot-8.0.4/pywikibot/families/commons_family.py` & `pywikibot-8.1.0/pywikibot/families/commons_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/families/lingualibre_family.py` & `pywikibot-8.1.0/pywikibot/families/lingualibre_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/families/meta_family.py` & `pywikibot-8.1.0/pywikibot/families/meta_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/families/osm_family.py` & `pywikibot-8.1.0/pywikibot/families/osm_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/families/vikidia_family.py` & `pywikibot-8.1.0/pywikibot/families/vikidia_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/families/wikibooks_family.py` & `pywikibot-8.1.0/pywikibot/families/wikibooks_family.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
     languages_by_size = [
         'en', 'vi', 'hu', 'de', 'fr', 'it', 'ja', 'pt', 'es', 'nl', 'pl', 'id',
         'he', 'fi', 'zh', 'fa', 'az', 'sq', 'ru', 'ca', 'eu', 'th', 'cs', 'da',
         'ko', 'ba', 'sv', 'gl', 'hi', 'sr', 'uk', 'hr', 'no', 'tr', 'sa', 'ar',
         'ta', 'bn', 'eo', 'sk', 'is', 'ro', 'si', 'bg', 'ms', 'mk', 'ka', 'tt',
         'lt', 'el', 'li', 'sl', 'tl', 'ur', 'km', 'la', 'mr', 'kk', 'te', 'et',
-        'be', 'ia', 'shn', 'ml', 'oc', 'hy', 'pa', 'ne', 'cv', 'tg', 'ku',
+        'be', 'ia', 'shn', 'ml', 'oc', 'pa', 'hy', 'ne', 'cv', 'tg', 'ku',
         'fy', 'af', 'bs', 'cy', 'mg', 'ky',
     ]
 
     category_redirect_templates = {
         '_default': (),
         'ar': ('تحويل تصنيف',),
         'en': ('Category redirect',),
```

### Comparing `pywikibot-8.0.4/pywikibot/families/wikidata_family.py` & `pywikibot-8.1.0/pywikibot/families/wikidata_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/families/wikihow_family.py` & `pywikibot-8.1.0/pywikibot/families/wikihow_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/families/wikimania_family.py` & `pywikibot-8.1.0/pywikibot/families/wikimania_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/families/wikimediachapter_family.py` & `pywikibot-8.1.0/pywikibot/families/wikimediachapter_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/families/wikinews_family.py` & `pywikibot-8.1.0/pywikibot/families/wikinews_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/families/wikipedia_family.py` & `pywikibot-8.1.0/pywikibot/families/wikipedia_family.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,41 +26,42 @@
     ]
 
     languages_by_size = [
         'en', 'ceb', 'de', 'sv', 'fr', 'nl', 'ru', 'es', 'it', 'arz', 'pl',
         'ja', 'zh', 'vi', 'war', 'uk', 'ar', 'pt', 'fa', 'ca', 'sr', 'id',
         'ko', 'no', 'ce', 'fi', 'hu', 'cs', 'tr', 'tt', 'sh', 'ro',
         'zh-min-nan', 'eu', 'ms', 'eo', 'he', 'hy', 'da', 'bg', 'cy', 'sk',
-        'azb', 'et', 'kk', 'be', 'simple', 'min', 'uz', 'el', 'hr', 'lt', 'gl',
+        'azb', 'et', 'kk', 'be', 'simple', 'uz', 'min', 'el', 'hr', 'lt', 'gl',
         'az', 'ur', 'sl', 'ka', 'nn', 'hi', 'th', 'ta', 'la', 'bn', 'mk',
         'ast', 'zh-yue', 'lld', 'lv', 'tg', 'af', 'my', 'mg', 'bs', 'mr', 'sq',
         'oc', 'nds', 'ml', 'be-tarask', 'te', 'ky', 'br', 'sw', 'jv', 'new',
         'vec', 'pnb', 'ht', 'pms', 'ba', 'lb', 'su', 'ku', 'ga', 'lmo', 'szl',
         'is', 'fy', 'cv', 'ckb', 'pa', 'tl', 'an', 'wuu', 'diq', 'io', 'sco',
         'vo', 'yo', 'ne', 'ia', 'gu', 'kn', 'als', 'avk', 'bar', 'scn', 'bpy',
         'ha', 'crh', 'qu', 'nv', 'mn', 'xmf', 'si', 'ban', 'ps', 'frr',
         'bat-smg', 'os', 'or', 'sah', 'cdo', 'gd', 'bug', 'yi', 'sd', 'ilo',
-        'am', 'nap', 'mzn', 'li', 'gor', 'hsb', 'fo', 'map-bms', 'ig', 'mai',
+        'am', 'nap', 'mzn', 'li', 'ig', 'gor', 'hsb', 'fo', 'map-bms', 'mai',
         'bcl', 'eml', 'shn', 'ace', 'zh-classical', 'sa', 'wa', 'as', 'ie',
-        'lij', 'zu', 'mhr', 'hyw', 'hif', 'mrj', 'sn', 'bjn', 'mni', 'tum',
+        'lij', 'zu', 'mhr', 'hyw', 'hif', 'mrj', 'sn', 'bjn', 'tum', 'mni',
         'km', 'hak', 'roa-tara', 'so', 'pam', 'rue', 'nso', 'bh', 'sat', 'se',
         'myv', 'mi', 'vls', 'nds-nl', 'nah', 'sc', 'kw', 'glk', 'vep', 'kab',
-        'tk', 'gan', 'ary', 'co', 'dag', 'fiu-vro', 'bo', 'ab', 'gv', 'skr',
-        'ug', 'zea', 'frp', 'rw', 'udm', 'pcd', 'kv', 'csb', 'mt', 'gn', 'smn',
-        'ay', 'nrm', 'lez', 'lfn', 'olo', 'stq', 'mwl', 'lo', 'ang', 'fur',
-        'rm', 'lad', 'gom', 'koi', 'ext', 'tyv', 'dsb', 'av', 'ln', 'dty',
-        'kaa', 'pap', 'cbk-zam', 'dv', 'mdf', 'ksh', 'tw', 'gag', 'ks', 'bxr',
-        'pfl', 'lg', 'za', 'pi', 'pag', 'szy', 'haw', 'awa', 'tay', 'blk',
-        'inh', 'krc', 'xal', 'pdc', 'to', 'atj', 'arc', 'tcy', 'mnw', 'jam',
-        'kbp', 'na', 'wo', 'kbd', 'nia', 'nov', 'shi', 'ki', 'nqo', 'bi',
-        'anp', 'tpi', 'tet', 'jbo', 'roa-rup', 'xh', 'fj', 'kg', 'lbe', 'om',
-        'ty', 'guw', 'cu', 'trv', 'srn', 'sm', 'alt', 'gcr', 'chr', 'ltg',
-        'tn', 'ny', 'mad', 'st', 'pih', 'got', 'ee', 'ami', 'rmy', 'bm', 'ff',
-        've', 'ts', 'chy', 'ss', 'kcg', 'rn', 'pcm', 'ch', 'ik', 'pnt', 'guc',
-        'ady', 'iu', 'ak', 'pwn', 'sg', 'din', 'ti', 'kl', 'dz', 'gur', 'cr',
+        'tk', 'ary', 'gan', 'co', 'dag', 'fiu-vro', 'bo', 'ab', 'rw', 'gv',
+        'skr', 'ug', 'zea', 'frp', 'udm', 'pcd', 'kv', 'csb', 'mt', 'gn',
+        'smn', 'ay', 'nrm', 'lez', 'lfn', 'olo', 'stq', 'mwl', 'lo', 'ang',
+        'fur', 'rm', 'lad', 'gom', 'koi', 'ext', 'tyv', 'dsb', 'av', 'ln',
+        'dty', 'kaa', 'pap', 'cbk-zam', 'dv', 'mdf', 'ksh', 'tw', 'ks', 'gag',
+        'bxr', 'pfl', 'lg', 'za', 'pi', 'pag', 'szy', 'haw', 'awa', 'tay',
+        'blk', 'inh', 'krc', 'xal', 'pdc', 'to', 'atj', 'arc', 'tcy', 'mnw',
+        'jam', 'kbp', 'na', 'wo', 'kbd', 'nia', 'nov', 'shi', 'ki', 'nqo',
+        'anp', 'bi', 'tpi', 'tet', 'jbo', 'roa-rup', 'xh', 'fj', 'om', 'kg',
+        'lbe', 'ty', 'guw', 'cu', 'trv', 'srn', 'sm', 'alt', 'gcr', 'chr',
+        'ltg', 'tn', 'ny', 'mad', 'st', 'pih', 'got', 'ee', 'rmy', 'ami', 'bm',
+        'ff', 've', 'ts', 'chy', 'ss', 'kcg', 'rn', 'pcm', 'ch', 'ik', 'pnt',
+        'guc', 'ady', 'iu', 'ak', 'pwn', 'sg', 'din', 'ti', 'kl', 'dz', 'gur',
+        'cr',
     ]
 
     # Sites we want to edit but not count as real languages
     test_codes = ['test', 'test2']
 
     # Templates that indicate a category redirect
     # Redirects to these templates are automatically included
```

### Comparing `pywikibot-8.0.4/pywikibot/families/wikiquote_family.py` & `pywikibot-8.1.0/pywikibot/families/wikiquote_family.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     ]
 
     languages_by_size = [
         'it', 'en', 'pl', 'ru', 'cs', 'et', 'pt', 'fa', 'uk', 'he', 'de', 'fr',
         'es', 'tr', 'eo', 'sk', 'bs', 'az', 'ca', 'fi', 'sr', 'zh', 'sl', 'lt',
         'ar', 'su', 'bg', 'hy', 'hr', 'id', 'el', 'nn', 'sv', 'li', 'hu', 'ko',
         'nl', 'sah', 'ja', 'la', 'ta', 'hi', 'gl', 'gu', 'ur', 'ig', 'be',
-        'te', 'guw', 'vi', 'tl', 'cy', 'no', 'bn', 'sq', 'ml', 'as', 'kn',
+        'guw', 'te', 'vi', 'tl', 'cy', 'no', 'bn', 'sq', 'ml', 'as', 'kn',
         'ro', 'eu', 'ku', 'uz', 'ka', 'da', 'sa', 'is', 'bcl', 'br', 'th',
         'mr', 'af', 'ky',
     ]
 
     category_redirect_templates = {
         '_default': (),
         'ar': ('تحويل تصنيف',),
```

### Comparing `pywikibot-8.0.4/pywikibot/families/wikisource_family.py` & `pywikibot-8.1.0/pywikibot/families/wikisource_family.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,16 +25,16 @@
     ]
 
     languages_by_size = [
         'pl', 'en', 'ru', 'de', 'fr', 'zh', 'he', 'it', 'uk', 'ar', 'es',
         'mul', 'gu', 'cs', 'sr', 'pt', 'fa', 'sv', 'bn', 'hu', 'ko', 'ta',
         'ml', 'sa', 'te', 'sl', 'tr', 'vi', 'hy', 'la', 'el', 'ja', 'ro', 'fi',
         'nl', 'nap', 'be', 'az', 'ca', 'hr', 'br', 'kn', 'no', 'id', 'th',
-        'hi', 'eo', 'is', 'vec', 'cy', 'ban', 'pms', 'mr', 'lij', 'da', 'et',
-        'mk', 'as', 'yi', 'bg', 'jv', 'wa', 'li', 'lt', 'pa', 'eu', 'or', 'gl',
+        'eo', 'hi', 'is', 'vec', 'cy', 'ban', 'pms', 'mr', 'lij', 'da', 'et',
+        'mk', 'as', 'yi', 'bg', 'jv', 'wa', 'li', 'lt', 'pa', 'or', 'eu', 'gl',
         'bs', 'sah', 'sk', 'zh-min-nan', 'fo',
     ]
 
     # Sites we want to edit but not count as real languages
     test_codes = ['beta']
 
     category_redirect_templates = {
```

### Comparing `pywikibot-8.0.4/pywikibot/families/wikiversity_family.py` & `pywikibot-8.1.0/pywikibot/families/wikiversity_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/families/wikivoyage_family.py` & `pywikibot-8.1.0/pywikibot/families/wikivoyage_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/families/wiktionary_family.py` & `pywikibot-8.1.0/pywikibot/families/wiktionary_family.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,24 +29,24 @@
     removed_wikis = [
         # https://noc.wikimedia.org/conf/highlight.php?file=dblists/deleted.dblist
         'als', 'ba', 'dk', 'mo', 'tlh', 'tokipona',
     ]
 
     languages_by_size = [
         'en', 'fr', 'mg', 'zh', 'ru', 'de', 'es', 'sh', 'sv', 'nl', 'el', 'pl',
-        'ku', 'lt', 'ca', 'it', 'hu', 'fi', 'ta', 'tr', 'pt', 'ja', 'io', 'hy',
+        'ku', 'lt', 'ca', 'it', 'hu', 'fi', 'ta', 'pt', 'tr', 'ja', 'io', 'hy',
         'ko', 'kn', 'vi', 'sr', 'th', 'hi', 'ro', 'no', 'id', 'et', 'cs',
         'skr', 'ml', 'my', 'uz', 'li', 'or', 'eo', 'te', 'fa', 'gl', 'ar',
         'oc', 'jv', 'az', 'uk', 'eu', 'sg', 'is', 'ast', 'br', 'bn', 'da',
         'mnw', 'lo', 'simple', 'la', 'hr', 'sk', 'shn', 'fj', 'ky', 'wa', 'bg',
         'tg', 'ur', 'ps', 'cy', 'lmo', 'he', 'vo', 'om', 'sl', 'af',
         'zh-min-nan', 'scn', 'ms', 'tl', 'pa', 'fy', 'sw', 'ka', 'nn', 'min',
         'lv', 'sq', 'nds', 'gor', 'lb', 'co', 'mn', 'pnb', 'bs', 'nah', 'yue',
         'sa', 'kk', 'km', 'ckb', 'vec', 'be', 'diq', 'tk', 'mk', 'nia', 'sm',
-        'hsb', 'ks', 'shy', 'su', 'gd', 'bcl', 'ga', 'an', 'gom', 'mr', 'wo',
+        'hsb', 'ks', 'shy', 'su', 'bcl', 'gd', 'ga', 'an', 'gom', 'mr', 'wo',
         'mni', 'bjn', 'ia', 'ang', 'mt', 'fo', 'sd', 'tt', 'gn', 'so', 'ie',
         'mi', 'csb', 'ha', 'ug', 'si', 'guw', 'st', 'hif', 'roa-rup', 'jbo',
         'kl', 'zu', 'ay', 'yi', 'ln', 'gu', 'na', 'gv', 'kw', 'tpi', 'am',
         'ne', 'rw', 'ts', 'ig', 'qu', 'ss', 'iu', 'chr', 'dv', 'ti', 'tn',
     ]
 
     category_redirect_templates = {
```

### Comparing `pywikibot-8.0.4/pywikibot/families/wowwiki_family.py` & `pywikibot-8.1.0/pywikibot/families/wowwiki_family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/family.py` & `pywikibot-8.1.0/pywikibot/family.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/fixes.py` & `pywikibot-8.1.0/pywikibot/fixes.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/flow.py` & `pywikibot-8.1.0/pywikibot/flow.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/i18n.py` & `pywikibot-8.1.0/pywikibot/i18n.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 The default message location may be changed by calling
 :py:obj:`set_message_package` with a package name. The package must contain an
 __init__.py, and a message bundle called 'pywikibot' containing messages.
 See :py:obj:`twtranslate` for more information on the messages.
 """
 #
-# (C) Pywikibot team, 2004-2022
+# (C) Pywikibot team, 2004-2023
 #
 # Distributed under the terms of the MIT license.
 #
 import json
 import os
 import pkgutil
 import re
@@ -649,22 +649,59 @@
         # On error: parameter is for PLURAL variants only,
         # don't change the string
         with suppress(KeyError, TypeError):
             trans = trans % parameters
     return trans
 
 
-def twtranslate(source: STR_OR_SITE_TYPE,
-                twtitle: str,
-                parameters: Union[Sequence[str], Mapping[str, int],
-                                  None] = None,
-                *,
-                fallback: bool = True,
-                fallback_prompt: Optional[str] = None,
-                only_plural: bool = False) -> Optional[str]:
+def get_bot_prefix(source: STR_OR_SITE_TYPE, use_prefix: bool) -> str:
+    """Get the bot prefix string like 'Bot: ' including space delimiter.
+
+    .. note: If *source* is a str and ``config.bot_prefix`` is set to
+       None, it cannot be determined whether the current user is a bot
+       account. In this cas the prefix will be returned.
+    .. versionadded:: 8.1
+
+    :param source: When it's a site it's using the lang attribute and otherwise
+        it is using the value directly.
+    :param use_prefix: If True, return a bot prefix which depends on the
+        ``config.bot_prefix`` setting.
+    """
+    config_prefix = config.bot_prefix_summary
+    if not use_prefix or config_prefix is False:
+        return ''
+
+    if isinstance(config_prefix, str):
+        return config_prefix + ' '
+
+    try:
+        prefix = twtranslate(source, 'pywikibot-bot-prefix') + ' '
+    except pywikibot.exceptions.TranslationError:
+        # the 'pywikibot' package is available but the message key may
+        # be missing
+        prefix = 'Bot: '
+
+    if config_prefix is True \
+       or not hasattr(source, 'lang') \
+       or source.isBot(source.username()):
+        return prefix
+
+    return ''
+
+
+def twtranslate(
+    source: STR_OR_SITE_TYPE,
+    twtitle: str,
+    parameters: Union[Sequence[str], Mapping[str, int], None] = None,
+    *,
+    fallback: bool = True,
+    fallback_prompt: Optional[str] = None,
+    only_plural: bool = False,
+    bot_prefix: bool = False
+) -> Optional[str]:
     r"""
     Translate a message using JSON files in messages_package_name.
 
     fallback parameter must be True for i18n and False for L10N or testing
     purposes.
 
     Support for plural is implemented like in MediaWiki extension. If the
@@ -708,44 +745,50 @@
     'Robot: Changer seulement une page.'
     >>> # use format strings also outside
     >>> str(i18n.twtranslate(
     ...    'fr', 'test-plural', {'num': 10}, only_plural=True
     ... ) % {'descr': 'seulement'})
     'Robot: Changer seulement quelques pages.'
 
+    .. versionchanged:: 8.1
+       the *bot_prefix* parameter was added.
+
     :param source: When it's a site it's using the lang attribute and otherwise
-        it is using the value directly.
+        it is using the value directly. The site object is recommended.
     :param twtitle: The TranslateWiki string title, in <package>-<key> format
     :param parameters: For passing parameters. It should be a mapping but for
         backwards compatibility can also be a list, tuple or a single value.
         They are also used for plural entries in which case they must be a
         Mapping and will cause a TypeError otherwise.
     :param fallback: Try an alternate language code
     :param fallback_prompt: The English message if i18n is not available
     :param only_plural: Define whether the parameters should be only applied to
         plural instances. If this is False it will apply the parameters also
         to the resulting string. If this is True the placeholders must be
         manually applied afterwards.
+    :param bot_prefix: If True, prepend the message with a bot prefix
+        which depends on the ``config.bot_prefix`` setting
     :raise IndexError: If the language supports and requires more plurals than
         defined for the given translation template.
     """
+    prefix = get_bot_prefix(source, use_prefix=bot_prefix)
+
     if not messages_available():
         if fallback_prompt:
             if parameters and not only_plural:
                 return fallback_prompt % parameters
             return fallback_prompt
 
         raise pywikibot.exceptions.TranslationError(
             'Unable to load messages package {} for bundle {}'
             '\nIt can happen due to lack of i18n submodule or files. '
             'See {}/i18n'
             .format(_messages_package_name, twtitle, __url__))
 
     # if source is a site then use its lang attribute, otherwise it's a str
-
     lang = getattr(source, 'lang', source)
 
     # There are two possible failure modes: the translation dict might not have
     # the language altogether, or a specific key could be untranslated. Both
     # modes are caught with the KeyError.
     langs = [lang]
     if fallback:
@@ -770,16 +813,16 @@
         trans = _extract_plural(alt, trans, parameters)
 
     if parameters is not None and not isinstance(parameters, Mapping):
         raise ValueError('parameters should be a mapping, not {}'
                          .format(type(parameters).__name__))
 
     if not only_plural and parameters:
-        return trans % parameters
-    return trans
+        trans = trans % parameters
+    return prefix + trans
 
 
 def twhas_key(source: STR_OR_SITE_TYPE, twtitle: str) -> bool:
     """
     Check if a message has a translation in the specified language code.
 
     The translations are retrieved from i18n.<package>, based on the callers
```

### Comparing `pywikibot-8.0.4/pywikibot/interwiki_graph.py` & `pywikibot-8.1.0/pywikibot/interwiki_graph.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/logentries.py` & `pywikibot-8.1.0/pywikibot/logentries.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/logging.py` & `pywikibot-8.1.0/pywikibot/logging.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/login.py` & `pywikibot-8.1.0/pywikibot/login.py`

 * *Files 0% similar despite different names*

```diff
@@ -283,17 +283,17 @@
 
             # As we don't want the password to appear on the screen, we set
             # password = True
             self.password = pywikibot.input(
                 'Password for user {name} on {site} (no characters will be '
                 'shown):'.format(name=self.login_name, site=self.site),
                 password=True)
+        else:
+            pywikibot.info(f'Logging in to {self.site} as {self.login_name}')
 
-        pywikibot.info('Logging in to {site} as {name}'
-                       .format(name=self.login_name, site=self.site))
         try:
             self.login_to_site()
         except APIError as e:
             error_code = e.code
 
             # TODO: investigate other unhandled API codes
             if error_code in self._api_error:
```

### Comparing `pywikibot-8.0.4/pywikibot/page/__init__.py` & `pywikibot-8.1.0/pywikibot/page/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/page/_basepage.py` & `pywikibot-8.1.0/pywikibot/page/_basepage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1287,14 +1287,18 @@
 
         done = self.site.editpage(self, summary=summary, minor=minor,
                                   watch=watch, bot=botflag, **kwargs)
         if not done:
             if not quiet:
                 pywikibot.warning(f'Page {link} not saved')
             raise PageSaveRelatedError(self)
+
+        if not self.pageid:
+            self.site.loadpageinfo(self)
+
         if not quiet:
             pywikibot.info(f'Page {link} saved')
 
     def _cosmetic_changes_hook(self, summary: str) -> str:
         """The cosmetic changes hook.
 
         :param summary: The current edit summary.
```

### Comparing `pywikibot-8.0.4/pywikibot/page/_category.py` & `pywikibot-8.1.0/pywikibot/page/_category.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/page/_collections.py` & `pywikibot-8.1.0/pywikibot/page/_collections.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/page/_decorators.py` & `pywikibot-8.1.0/pywikibot/page/_decorators.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/page/_filepage.py` & `pywikibot-8.1.0/pywikibot/page/_filepage.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/page/_links.py` & `pywikibot-8.1.0/pywikibot/page/_links.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/page/_page.py` & `pywikibot-8.1.0/pywikibot/page/_page.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/page/_revision.py` & `pywikibot-8.1.0/pywikibot/page/_revision.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/page/_toolforge.py` & `pywikibot-8.1.0/pywikibot/page/_toolforge.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/page/_user.py` & `pywikibot-8.1.0/pywikibot/page/_user.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/page/_wikibase.py` & `pywikibot-8.1.0/pywikibot/page/_wikibase.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     EntityTypeUnknownError,
     Error,
     InterwikiRedirectPageError,
     InvalidTitleError,
     IsNotRedirectPageError,
     IsRedirectPageError,
     NoPageError,
+    NoSiteLinkError,
     NoWikibaseEntityError,
     WikiBaseError,
 )
 from pywikibot.family import Family
 from pywikibot.page._collections import (
     AliasesDict,
     ClaimCollection,
@@ -293,14 +294,17 @@
          - :meth:`WikibasePage.editLabels`
          - :meth:`WikibasePage.editDescriptions`
          - :meth:`WikibasePage.editAliases`
          - :meth:`ItemPage.setSitelinks`
 
          .. seealso:: :meth:`WikibasePage.editEntity`
 
+         .. versionchanged:: 8.0.1
+            Copy snak IDs/hashes (:phab:`T327607`)
+
         :param data: Data to be saved
         """
         update_self = False
         if data is None:
             data = self.toJSON(diffto=getattr(self, '_content', None))
             # We only want to copy the IDs from the updates
             # if data was not passed in.
@@ -1068,32 +1072,34 @@
         for sl in self.sitelinks.values():
             if family is None or family == sl.site.family:
                 pg = pywikibot.Page(sl)
                 pg._item = self
                 yield pg
 
     def getSitelink(self, site, force: bool = False) -> str:
-        """
-        Return the title for the specific site.
+        """Return the title for the specific site.
+
+        If the item doesn't have that language, raise NoSiteLinkError.
 
-        If the item doesn't have that language, raise NoPageError.
+        .. versionchanged:: 8.1
+           raises NoSiteLinkError instead of NoPageError.
 
         :param site: Site to find the linked page of.
         :type site: pywikibot.Site or database name
         :param force: override caching
         :param get_redirect: return the item content, do not follow the
                              redirect, do not raise an exception.
         :raise IsRedirectPageError: instance is a redirect page
-        :raise NoPageError: site is not in :attr:`sitelinks`
+        :raise NoSiteLinkError: site is not in :attr:`sitelinks`
         """
         if force or not hasattr(self, '_content'):
             self.get(force=force)
 
         if site not in self.sitelinks:
-            raise NoPageError(self)
+            raise NoSiteLinkError(self, site.lang)
 
         return self.sitelinks[site].canonical_title()
 
     def setSitelink(self, sitelink: SITELINK_TYPE, **kwargs) -> None:
         """Set sitelinks. Calls :meth:`setSitelinks`.
 
         A *sitelink* can be a Page object, a BaseLink object or a
@@ -1482,16 +1488,16 @@
             raise RuntimeError(first_upper(message.format('reference')))
 
     def __repr__(self) -> str:
         """Return the representation string."""
         cls_name = type(self).__name__
         if self.target:
             return f'{cls_name}.fromJSON({self.repo!r}, {self.toJSON()})'
-        else:
-            return f'{cls_name}({self.repo!r}, {self.id!r})'
+
+        return f'{cls_name}({self.repo!r}, {self.id!r})'
 
     def __eq__(self, other):
         if not isinstance(other, self.__class__):
             return False
 
         return self.same_as(other)
```

### Comparing `pywikibot-8.0.4/pywikibot/pagegenerators/__init__.py` & `pywikibot-8.1.0/pywikibot/pagegenerators/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 titles to standard output.
 
 These parameters are supported to specify which pages titles to print:
 
 &params;
 """
 #
-# (C) Pywikibot team, 2008-2022
+# (C) Pywikibot team, 2008-2023
 #
 # Distributed under the terms of the MIT license.
 #
 from typing import Any, Optional
 
 import pywikibot
 from pywikibot.backports import Callable, Dict, Iterable, Iterator, List, Set
@@ -609,54 +609,64 @@
                     break
             pywikibot.sleep(sleep_duration)
 
         yield from reversed(list(filtered_generator()))
 
 
 def PreloadingGenerator(generator: Iterable['pywikibot.page.Page'],
-                        groupsize: int = 50
+                        groupsize: int = 50,
+                        quiet: bool = False
                         ) -> Iterator['pywikibot.page.Page']:
-    """
-    Yield preloaded pages taken from another generator.
+    """Yield preloaded pages taken from another generator.
 
     :param generator: pages to iterate over
     :param groupsize: how many pages to preload at once
+    :param quiet: If False (default), show the "Retrieving pages"
+        message
     """
     # pages may be on more than one site, for example if an interwiki
     # generator is used, so use a separate preloader for each site
     sites: PRELOAD_SITE_TYPE = {}
     # build a list of pages for each site found in the iterator
     for page in generator:
         site = page.site
         sites.setdefault(site, []).append(page)
 
         groupsize = min(groupsize, site.maxlimit)
         if len(sites[site]) >= groupsize:
             # if this site is at the groupsize, process it
             group = sites.pop(site)
-            yield from site.preloadpages(group, groupsize=groupsize)
+            yield from site.preloadpages(group, groupsize=groupsize,
+                                         quiet=quiet)
 
     for site, pages in sites.items():
         # process any leftover sites that never reached the groupsize
-        yield from site.preloadpages(pages, groupsize=groupsize)
+        yield from site.preloadpages(pages, groupsize=groupsize, quiet=quiet)
 
 
 def DequePreloadingGenerator(generator: Iterable['pywikibot.page.Page'],
-                             groupsize: int = 50
+                             groupsize: int = 50,
+                             quiet: bool = False
                              ) -> Iterator['pywikibot.page.Page']:
-    """Preload generator of type DequeGenerator."""
+    """Preload generator of type DequeGenerator.
+
+    :param generator: pages to iterate over
+    :param groupsize: how many pages to preload at once
+    :param quiet: If False (default), show the "Retrieving pages"
+        message
+    """
     assert isinstance(generator, DequeGenerator), \
         'generator must be a DequeGenerator object'
 
     while True:
         page_count = min(len(generator), groupsize)
         if not page_count:
             return
 
-        yield from PreloadingGenerator(generator, page_count)
+        yield from PreloadingGenerator(generator, page_count, quiet)
 
 
 def PreloadingEntityGenerator(generator: Iterable['pywikibot.page.Page'],
                               groupsize: int = 50
                               ) -> Iterator['pywikibot.page.Page']:
     """
     Yield preloaded pages taken from another generator.
```

### Comparing `pywikibot-8.0.4/pywikibot/pagegenerators/_factory.py` & `pywikibot-8.1.0/pywikibot/pagegenerators/_factory.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/pagegenerators/_filters.py` & `pywikibot-8.1.0/pywikibot/pagegenerators/_filters.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/pagegenerators/_generators.py` & `pywikibot-8.1.0/pywikibot/pagegenerators/_generators.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/plural.py` & `pywikibot-8.1.0/pywikibot/plural.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/proofreadpage.py` & `pywikibot-8.1.0/pywikibot/proofreadpage.py`

 * *Files 0% similar despite different names*

```diff
@@ -218,14 +218,18 @@
 
     .. seealso::
        https://www.mediawiki.org/wiki/Help:Extension:ProofreadPage/Pages_tag
 
     Parse text and extract the first ``<pages ... />`` tag.
     Individual attributes will be accessible with dot notation.
 
+    >>> tp = PagesTagParser('<pages />')
+    >>> tp
+    PagesTagParser('<pages />')
+
     >>> tp = PagesTagParser(
     ... 'Text: <pages index="Index.pdf" from="first" to="last" />')
     >>> tp
     PagesTagParser('<pages index="Index.pdf" from="first" to="last" />')
 
     Attributes can be modified via dot notation. If an attribute is a
     number, it is converted to int.
@@ -265,44 +269,46 @@
     >>> 'to' in tp
     True
 
     >>> 'step' in tp
     False
 
     .. versionadded:: 8.0
+    .. versionchanged:: 8.1
+       *text* parameter is defaulted to ``'<pages />'``.
     """
 
     pat_tag = re.compile(r'<pages (?P<attrs>[^/]*?)/>')
     tokens = (
         'index',
         'from',
         'to',
         'include',
         'exclude',
         'step',
         'header',
-        'tosection',
         'fromsection',
+        'tosection',
         'onlysection',
     )
     tokens = '(' + '=|'.join(tokens) + '=)'
     pat_attr = re.compile(tokens)
 
     index = TagAttrDesc()
     ffrom = TagAttrDesc()
     to = TagAttrDesc()
     include = TagAttrDesc()
     exclude = TagAttrDesc()
     step = TagAttrDesc()
     header = TagAttrDesc()
-    tosection = TagAttrDesc()
     fromsection = TagAttrDesc()
+    tosection = TagAttrDesc()
     onlysection = TagAttrDesc()
 
-    def __init__(self, text):
+    def __init__(self, text='<pages />'):
         """Initializer."""
         m = self.pat_tag.search(text)
         if m is None:
             raise ValueError(f'Invalid text={text}')
 
         tag = m['attrs']
         matches = list(self.pat_attr.finditer(tag))
```

### Comparing `pywikibot-8.0.4/pywikibot/scripts/__init__.py` & `pywikibot-8.1.0/pywikibot/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/generate_family_file.py` & `pywikibot-8.1.0/pywikibot/scripts/generate_family_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,35 +8,39 @@
     pwb generate_family_file.py [<url>] [<name>] [<dointerwiki>] [<verify>]
 
 Parameters are optional. They must be given consecutively but may be
 omitted if there is no successor parameter. The parameters are::
 
     <url>:         an url from where the family settings are loaded
     <name>:        the family name without "_family.py" tail.
-    <dointerwiki>: predefined answer (y|n) to add multiple site codes
+    <dointerwiki>: predefined answer (y|s|n) to add multiple site codes
     <verify>:      disable certificate validaton `(y|n)
 
 Example::
 
     pwb generate_family_file.py https://www.mywiki.bogus/wiki/Main_Page mywiki
 
 This will create the file mywiki_family.py in families folder of your
 base directory.
 
 .. versionchanged:: 7.0
    moved to pywikibot.scripts folder; create family files in families
    folder of your base directory instead of pywikibot/families.
+.. versionchanged:: 8.1
+   [s]trict can be given for <dointerwiki> parameter to ensure that
+   sites are from the given domain.
 """
 #
-# (C) Pywikibot team, 2010-2022
+# (C) Pywikibot team, 2010-2023
 #
 # Distributed under the terms of the MIT license
 #
 import codecs
 import os
+import re
 import string
 import sys
 from contextlib import suppress
 from typing import Optional
 from urllib.parse import urlparse
 
 
@@ -59,16 +63,18 @@
                  verify: Optional[str] = None) -> None:
         """
         Parameters are optional. If not given the script asks for the values.
 
         :param url: an url from where the family settings are loaded
         :param name: the family name without "_family.py" tail.
         :param dointerwiki: Predefined answer to add multiple site
-            codes. Pass `Y` or `y` for yes `N` or `n` for no and
-            `E` or `e` if you want to edit the collection of sites.
+            codes. Pass `Y` or `y` for yes, `S` or `s` for strict which
+            only includes site of the same domain (usually for Wikimedia
+            sites), `N` or `n` for no and `E` or `e` if you want to edit
+            the collection of sites.
         :param verify: If a certificate verification failes, you may
             pass `Y` or `y` to disable certificate validaton `N` or `n`
             to keep it enabled.
         """
         from pywikibot.scripts import _import_with_no_user_config
 
         # from pywikibot.site_detect import MWSite and
@@ -145,15 +151,22 @@
               '\n==================================\n'.format(w=w))
 
         self.getlangs(w)
         self.getapis()
         self.writefile(verify)
 
     def getlangs(self, w) -> None:
-        """Determine site code of a family."""
+        """Determine site code of a family.
+
+        .. versionchanged:: 8.1
+           with [e]dit the interwiki list can be given delimited by
+           space or comma or both. With [s]trict only sites with the
+           same domain are collected. A [h]elp answer was added to show
+           more information about possible answers.
+        """
         print('Determining other sites...', end='')
         try:
             self.langs = w.langs
             print(' '.join(sorted(wiki['prefix'] for wiki in self.langs)))
         except Exception as e:  # pragma: no cover
             self.langs = []
             print(e, '; continuing...')
@@ -165,62 +178,85 @@
                                'local': '',
                                'prefix': w.lang,
                                'url': w.iwpath})
 
         code_len = len(self.langs)
         if code_len > 1:
             if self.dointerwiki is None:
-                makeiw = input(
-                    '\nThere are {} sites available.'
-                    '\nDo you want to generate interwiki links? '
-                    'This might take a long time. ([y]es/[N]o/[e]dit)'
-                    .format(code_len)).lower()
+                while True:
+                    makeiw = input(
+                        '\n'
+                        f'There are {code_len} sites available.'
+                        ' Do you want to generate interwiki links?\n'
+                        'This might take a long time. '
+                        '([y]es, [s]trict, [N]o, [e]dit), [h]elp) ').lower()
+                    if makeiw in ('y', 's', 'n', 'e', ''):
+                        break
+                    print(
+                        '\n'
+                        '[y]es:    create interwiki links for all sites\n'
+                        '[s]trict: yes, but for sites with same domain only\n'
+                        '[N]o:     no, use the current site only (default)\n'
+                        '[e]dit:   get a list delimited with space or comma\n'
+                        '[h]elp:   this help message'
+                    )
             else:
                 makeiw = self.dointerwiki
 
-            if makeiw == 'n':
+            if makeiw in ('n', ''):
                 self.langs = [wiki for wiki in self.langs
                               if wiki['url'] == w.iwpath]
+            elif makeiw == 's':
+                domain = '.'.join(urlparse(w.server).hostname.split('.')[1:])
+                self.langs = [wiki for wiki in self.langs
+                              if domain in wiki['url']]
+
             elif makeiw == 'e':
                 for wiki in self.langs:
                     print(wiki['prefix'], wiki['url'])
-                do_langs = input('Which sites do you want: ')
+                do_langs = re.split(' *,| +',
+                                    input('Which sites do you want: '))
                 self.langs = [wiki for wiki in self.langs
                               if wiki['prefix'] in do_langs
                               or wiki['url'] == w.iwpath]
 
         for wiki in self.langs:
             assert all(x in CODE_CHARACTERS for x in wiki['prefix']), \
                 'Family {} code {} must be ASCII lowercase ' \
                 'letters and digits [a-z0-9] or underscore/dash [_-]' \
                 .format(self.name, wiki['prefix'])
 
     def getapis(self) -> None:
         """Load other site pages."""
-        print('Loading wikis... ')
+        print(f'Loading {len(self.langs)} wikis... ')
+        remove = []
         for lang in self.langs:
             key = lang['prefix']
             print(f'  * {key}... ', end='')
             if key not in self.wikis:
                 try:
                     self.wikis[key] = self.Wiki(lang['url'])
                     print('downloaded')
                 except Exception as e:  # pragma: no cover
                     print(e)
+                    remove.append(lang)
             else:
                 print('in cache')
 
+        for lang in remove:
+            self.langs.remove(lang)
+
     def writefile(self, verify) -> None:
         """Write the family file."""
         fn = os.path.join(self.base_dir, 'families',
                           f'{self.name}_family.py')
         print(f'Writing {fn}... ')
 
-        if os.path.exists(fn) and input('{} already exists. Overwrite? (y/n)'
-                                        .format(fn)).lower() == 'n':
+        if os.path.exists(fn) and input(
+                f'{fn} already exists. Overwrite? (y/n) ').lower() == 'n':
             print('Terminating.')
             sys.exit(1)
 
         code_hostname_pairs = '\n        '.join(
             "'{code}': '{hostname}',".format(
                 code=k, hostname=urlparse(w.server).netloc
             ) for k, w in self.wikis.items())
```

### Comparing `pywikibot-8.0.4/pywikibot/scripts/generate_user_files.py` & `pywikibot-8.1.0/pywikibot/scripts/generate_user_files.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ar.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ar.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ast.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ast.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/az.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/az.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/azb.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/azb.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ba.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ba.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/bcc.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/bcc.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/be-tarask.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/be-tarask.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/be.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/be.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/bg.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/bg.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/bn.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/bn.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/br.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/br.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/bs.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/bs.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ca.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ca.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ce.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ce.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ckb.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ckb.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/cs.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/cs.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/csb.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/csb.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/cy.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/cy.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/da.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/da.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/de.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/de.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/diq.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/diq.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/el.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/el.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/en.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/en.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/eo.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/eo.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/es.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/es.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/eu.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/eu.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/fa.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/fa.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/fi.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/fi.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/fo.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/fo.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/fr.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/fr.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/frr.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/frr.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/gl.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/gl.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/gsw.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/gsw.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/hak.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/hak.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/haw.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/haw.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/he.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/he.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/hi.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/hi.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/hsb.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/hsb.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/hu.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/hu.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ia.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ia.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/id.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/id.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/io.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/io.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/is.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/is.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/it.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/it.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ja.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ja.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/kab.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/kab.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/kk.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/kk.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/km.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/km.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/kn.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/kn.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ko.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ko.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/krc.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/krc.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ksh.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ksh.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/lb.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/lb.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/lt.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/lt.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/lv.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/lv.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/map-bms.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/map-bms.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/mg.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/mg.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/min.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/min.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/mk.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/mk.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ml.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ml.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ms.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ms.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/my.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/my.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/nan.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/nan.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/nb.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/nb.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/nds-nl.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/nds-nl.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ne.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ne.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/new.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/new.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/nl.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/nl.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/nqo.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/nqo.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/pl.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/pl.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/pms.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/pms.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/pt-br.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/pt-br.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/pt.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/pt.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/qqq.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/qqq.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ro.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ro.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ru.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ru.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/sco.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/sco.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/sh.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/sh.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/si.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/si.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/sk.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/sk.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/sl.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/sl.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/so.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/so.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/sr.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/sr.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/sv.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/sv.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/sw.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/sw.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ta.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ta.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/te.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/te.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/th.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/th.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/tly.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/tly.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/tr.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/tr.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/uk.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/uk.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/ur.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/ur.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/vi.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/vi.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/yue.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/yue.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/i18n/pywikibot/zh.json` & `pywikibot-8.1.0/pywikibot/scripts/i18n/pywikibot/zh.json`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/login.py` & `pywikibot-8.1.0/pywikibot/scripts/login.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/preload_sites.py` & `pywikibot-8.1.0/pywikibot/scripts/preload_sites.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/shell.py` & `pywikibot-8.1.0/pywikibot/scripts/shell.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/version.py` & `pywikibot-8.1.0/pywikibot/scripts/version.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/scripts/wrapper.py` & `pywikibot-8.1.0/pywikibot/scripts/wrapper.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/site/__init__.py` & `pywikibot-8.1.0/pywikibot/site/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/site/_apisite.py` & `pywikibot-8.1.0/pywikibot/site/_apisite.py`

 * *Files 1% similar despite different names*

```diff
@@ -328,17 +328,17 @@
         autocreate: bool = False,
         user: Optional[str] = None,
         *,
         cookie_only: bool = False
     ) -> None:
         """Log the user in if not already logged in.
 
-        .. versionchanged:: 8.0.0
-           lazy load cookies when logging in. This was dropped in 8.0.4
-        .. versionchanged:: 8.0.4
+        .. versionchanged:: 8.0
+           lazy load cookies when logging in. This was dropped in 8.1
+        .. versionchanged:: 8.1
            the *cookie_only* parameter was added and cookies are loaded
            whenever the site is initialized.
 
         .. seealso:: :api:`Login`
 
         :param autocreate: if true, allow auto-creation of the account
             using unified login
@@ -1980,14 +1980,15 @@
                             urls = ', '.join(err.other[err.code]['matches'])
                             raise exception(page, url=urls) from None
                         raise exception(page) from None
                     pywikibot.debug(
                         "editpage: Unexpected error code '{}' received."
                         .format(err.code))
                     raise
+
                 assert 'edit' in result and 'result' in result['edit'], result
 
                 if result['edit']['result'] == 'Success':
                     if 'nochange' in result['edit']:
                         # null edit, page not changed
                         pywikibot.log('Page [[{}]] saved without any changes.'
                                       .format(page.title()))
@@ -2022,40 +2023,42 @@
                                 'then type answer here:')
                             continue
 
                         pywikibot.error(
                             'editpage: unknown CAPTCHA response {}, '
                             'page not saved'
                             .format(captcha))
-                        return False
+                        break
 
                     if 'spamblacklist' in result['edit']:
                         raise SpamblacklistError(
                             page, result['edit']['spamblacklist']) from None
 
                     if 'code' in result['edit'] and 'info' in result['edit']:
                         pywikibot.error(
                             'editpage: {}\n{}, '
                             .format(result['edit']['code'],
                                     result['edit']['info']))
-                        return False
+                        break
 
                     pywikibot.error('editpage: unknown failure reason {}'
                                     .format(str(result)))
-                    return False
+                    break
 
                 pywikibot.error(
                     "editpage: Unknown result code '{}' received; "
                     'page not saved'.format(result['edit']['result']))
                 pywikibot.log(str(result))
-                return False
+                break
 
         finally:
             self.unlock_page(page)
 
+        return False
+
     OnErrorExc = namedtuple('OnErrorExc', 'exception on_new_page')
 
     # catalog of merge history errors for use in error messages
     _mh_errors = {
         'noapiwrite': 'API editing not enabled on {site} wiki',
         'writeapidenied':
             'User {user} is not authorized to edit on {site} wiki',
@@ -2376,15 +2379,14 @@
         'permissiondenied': 'User {user} not authorized to (un)delete '
                             'pages on {site} wiki.',
         'cantdelete':
             'Could not delete [[{title}]]. Maybe it was deleted already.',
         'cantundelete': 'Could not undelete [[{title}]]. '
                         'Revision may not exist or was already undeleted.',
         'nodeleteablefile': 'No such old version of file',
-        'missingtitle': "[[{title}]] doesn't exist.",
     }  # other errors shouldn't occur because of pre-submission checks
 
     @need_right('delete')
     def delete(
         self,
         page: Union['pywikibot.page.BasePage', int, str],
         reason: str,
@@ -2407,14 +2409,17 @@
 
         .. versionchanged:: 6.1
            keyword only parameter `oldimage` was added.
 
         .. versionchanged:: 7.1
            keyword only parameter `deletetalk` was added.
 
+        .. versionchanged:: 8.1
+           raises :exc:`exceptions.NoPageError` if page does not exist.
+
         :param page: Page to be deleted or its pageid.
         :param reason: Deletion reason.
         :param deletetalk: Also delete the talk page, if it exists.
         :param oldimage: oldimage id of the file version to be deleted.
             If a BasePage object is given with page parameter, it has to
             be a FilePage.
         :raises TypeError, ValueError: page has wrong type/value.
@@ -2448,19 +2453,23 @@
                 params['deletetalk'] = deletetalk
 
         req = self.simple_request(**params)
         self.lock_page(page)
         try:
             req.submit()
         except APIError as err:
+            if err.code == 'missingtitle':
+                raise NoPageError(page) from None
+
             errdata = {
                 'site': self,
                 'title': title,
                 'user': self.user(),
             }
+
             if err.code in self._dl_errors:
                 raise Error(
                     self._dl_errors[err.code].format_map(errdata)
                 ) from None
             pywikibot.debug('delete: Unexpected error code {!r} received.'
                             .format(err.code))
             raise
@@ -2866,23 +2875,24 @@
         Use pywikibot.diff's html_comparator() method to parse result.
         :param old: starting revision ID, title, Page, or Revision
         :param diff: ending revision ID, title, Page, or Revision
         :return: Returns an HTML string of a diff between two revisions.
         """
         # check old and diff types
         def get_param(item: object) -> Optional[Tuple[str, Union[str, int]]]:
+            param = None
             if isinstance(item, str):
-                return 'title', item
-            if isinstance(item, pywikibot.Page):
-                return 'title', item.title()
-            if isinstance(item, int):
-                return 'rev', item
-            if isinstance(item, pywikibot.page.Revision):
-                return 'rev', item.revid
-            return None
+                param = 'title', item
+            elif isinstance(item, pywikibot.Page):
+                param = 'title', item.title()
+            elif isinstance(item, int):
+                param = 'rev', item
+            elif isinstance(item, pywikibot.page.Revision):
+                param = 'rev', item.revid
+            return param
 
         old_t = get_param(old)
         if not old_t:
             raise TypeError('old parameter is of invalid type')
         diff_t = get_param(diff)
         if not diff_t:
             raise TypeError('diff parameter is of invalid type')
```

### Comparing `pywikibot-8.0.4/pywikibot/site/_basesite.py` & `pywikibot-8.1.0/pywikibot/site/_basesite.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 #
 # (C) Pywikibot team, 2008-2023
 #
 # Distributed under the terms of the MIT license.
 #
 import functools
 import re
+import sys
 import threading
 from typing import Optional
 from warnings import warn
 
 import pywikibot
 from pywikibot.backports import Pattern
 from pywikibot.exceptions import (
@@ -26,14 +27,17 @@
     SelfCallString,
     cached,
     first_upper,
     normalize_username,
 )
 
 
+PYTHON_312A7 = sys.version.split()[0] == '3.12.0a7'  # T334378 workaround
+
+
 class BaseSite(ComparableMixin):
 
     """Site methods that are independent of the communication interface."""
 
     def __init__(self, code: str, fam=None, user=None) -> None:
         """
         Initializer.
@@ -182,14 +186,16 @@
 
     def username(self) -> Optional[str]:
         """Return the username used for the site."""
         return self._username
 
     def __getattr__(self, attr):
         """Delegate undefined methods calls to the Family object."""
+        if PYTHON_312A7:  # T334378 workaround
+            print(end='')  # noqa: T001, T201
         try:
             method = getattr(self.family, attr)
             if not callable(method):
                 raise AttributeError
             f = functools.partial(method, self.code)
             if hasattr(method, '__doc__'):
                 f.__doc__ = method.__doc__
@@ -312,35 +318,32 @@
                     'name in {fam}_family file'.format(repo=repo_name,
                                                        fam=self.family.name))
 
             dp = pywikibot.ItemPage(repo, item)
             try:
                 name = dp.getSitelink(self)
             except NoPageError:
-                raise Error(
-                    'No disambiguation category name found in {repo} '
-                    'for {site}'.format(repo=repo_name, site=self))
+                raise Error(f'No disambiguation category name found in {repo} '
+                            f'for {self}')
 
         else:  # fallback for non WM sites
             try:
                 name = '{}:{}'.format(Namespace.CATEGORY,
                                       self.family.disambcatname[self.code])
             except KeyError:
-                raise Error(
-                    'No disambiguation category name found in '
-                    '{site.family.name}_family for {site}'.format(site=self))
+                raise Error(f'No disambiguation category name found in '
+                            f'{self.family.name}_family for {self}')
 
         return pywikibot.Category(pywikibot.Link(name, self))
 
     def isInterwikiLink(self, text):  # noqa: N802
         """Return True if text is in the form of an interwiki link.
 
-        If a link object constructed using "text" as the link text parses as
-        belonging to a different site, this method returns True.
-
+        If a link object constructed using "text" as the link text parses
+        as belonging to a different site, this method returns True.
         """
         linkfam, linkcode = pywikibot.Link(text, self).parse_site()
         return linkfam != self.family.name or linkcode != self.code
 
     def redirectRegex(  # noqa: N802
         self,
         pattern: Optional[str] = None
```

### Comparing `pywikibot-8.0.4/pywikibot/site/_datasite.py` & `pywikibot-8.1.0/pywikibot/site/_datasite.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/site/_decorators.py` & `pywikibot-8.1.0/pywikibot/site/_decorators.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/site/_extensions.py` & `pywikibot-8.1.0/pywikibot/site/_extensions.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/site/_generators.py` & `pywikibot-8.1.0/pywikibot/site/_generators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Objects representing API generators to MediaWiki site."""
 #
-# (C) Pywikibot team, 2008-2022
+# (C) Pywikibot team, 2008-2023
 #
 # Distributed under the terms of the MIT license.
 #
 import heapq
 import itertools
 import typing
 from contextlib import suppress
@@ -85,52 +85,64 @@
                 priority, page = heapq.heappop(prio_queue)
                 yield page
 
     def preloadpages(
         self,
         pagelist,
         *,
-        groupsize: int = 50,
+        groupsize: Optional[int] = None,
         templates: bool = False,
         langlinks: bool = False,
         pageprops: bool = False,
         categories: bool = False,
-        content: bool = True
+        content: bool = True,
+        quiet: bool = True
     ):
         """Return a generator to a list of preloaded pages.
 
-        Pages are iterated in the same order than in the underlying pagelist.
-        In case of duplicates in a groupsize batch, return the first entry.
+        Pages are iterated in the same order than in the underlying
+        pagelist. In case of duplicates in a groupsize batch, return the
+        first entry.
 
         .. versionchanged:: 7.6
            *content* parameter was added.
         .. versionchanged:: 7.7
            *categories* parameter was added.
+        .. versionchanged:: 8.1
+           *groupsize* is maxlimit by default. *quiet* parameter was
+           added. No longer show the "Retrieving pages from site"
+           message by default.
 
         :param pagelist: an iterable that returns Page objects
-        :param groupsize: how many Pages to query at a time
-        :param templates: preload pages (typically templates) transcluded in
-            the provided pages
-        :param langlinks: preload all language links from the provided pages
-            to other languages
-        :param pageprops: preload various properties defined in page content
+        :param groupsize: how many Pages to query at a time. If None
+            (default), :attr:`maxlimit
+            <pywikibot.site._apisite.APISite.maxlimit>` is used.
+        :param templates: preload pages (typically templates)
+            transcluded in the provided pages
+        :param langlinks: preload all language links from the provided
+            pages to other languages
+        :param pageprops: preload various properties defined in page
+            content
         :param categories: preload page categories
         :param content: preload page content
+        :param quiet: If True (default), do not show the "Retrieving
+            pages" message
         """
         props = 'revisions|info|categoryinfo'
         if templates:
             props += '|templates'
         if langlinks:
             props += '|langlinks'
         if pageprops:
             props += '|pageprops'
         if categories:
             props += '|categories'
 
-        for sublist in itergroup(pagelist, min(groupsize, self.maxlimit)):
+        groupsize = min(groupsize or self.maxlimit, self.maxlimit)
+        for sublist in itergroup(pagelist, groupsize):
             # Do not use p.pageid property as it will force page loading.
             pageids = [str(p._pageid) for p in sublist
                        if hasattr(p, '_pageid') and p._pageid > 0]
             cache = {}
             # In case of duplicates, return the first entry.
             for priority, page in enumerate(sublist):
                 try:
@@ -147,16 +159,16 @@
             if len(pageids) == len(sublist) \
                and len(set(pageids)) <= self.maxlimit:
                 # only use pageids if all pages have them
                 rvgen.request['pageids'] = set(pageids)
             else:
                 rvgen.request['titles'] = list(cache.keys())
             rvgen.request['rvprop'] = self._rvprops(content=content)
-            pywikibot.info('Retrieving {} pages from {}.'
-                           .format(len(cache), self))
+            if not quiet:
+                pywikibot.info(f'Retrieving {len(cache)} pages from {self}.')
 
             for pagedata in rvgen:
                 pywikibot.debug(f'Preloading {pagedata}')
                 try:
                     if pagedata['title'] not in cache:
                         # API always returns a "normalized" title which is
                         # usually the same as the canonical form returned by
@@ -1870,15 +1882,15 @@
         )
         for pageitem in gen:
             newpage = pywikibot.Page(self, pageitem['title'])
             if returndict:
                 yield (newpage, pageitem)
             else:
                 yield (newpage, pageitem['timestamp'], pageitem['newlen'],
-                       '', pageitem['user'], pageitem['comment'])
+                       '', pageitem['user'], pageitem.get('comment', ''))
 
     def querypage(self, special_page, total=True):
         """Yield Page objects retrieved from Special:{special_page}.
 
         .. seealso:: :api:`Querypage`
 
         Generic function for all special pages supported by the site MW API.
@@ -2106,25 +2118,43 @@
         """
         if propname not in self.get_property_names():
             raise NotImplementedError(
                 f'"{propname}" is not a valid page property')
         return self._generator(api.PageGenerator, type_arg='pageswithprop',
                                gpwppropname=propname, total=total)
 
-    def watched_pages(self, force: bool = False, total=None):
-        """
-        Return watchlist.
+    def watched_pages(
+        self,
+        force: bool = False,
+        total: Optional[int] = None, *,
+        with_talkpage: bool = True
+    ) -> Generator['pywikibot.Page', Any, None]:
+        """Return watchlist.
 
+        .. note:: ``watched_pages`` is a restartable generator. See
+           :class:`tools.collections.GeneratorWrapper` for its usage.
         .. seealso:: :api:`Watchlistraw`
+        .. versionadded:: 8.1
+           the *with_talkpage* parameter.
 
         :param force: Reload watchlist
         :param total: if not None, limit the generator to yielding this many
             items in total
-        :type total: int
-        :return: list of pages in watchlist
-        :rtype: list of pywikibot.Page objects
-        """
+        :param with_talkpage: if false, ignore talk pages and special
+            pages
+        :return: generator of pages in watchlist
+        """
+        def ignore_talkpages(page):
+            """Ignore talk pages and special pages."""
+            ns = page.namespace()
+            return ns >= 0 and not page.namespace() % 2
+
         expiry = None if force else pywikibot.config.API_config_expiry
         gen = api.PageGenerator(site=self, generator='watchlistraw',
                                 expiry=expiry)
         gen.set_maximum_items(total)
+
+        if not with_talkpage:
+            gen._namespaces = True
+            gen._check_result_namespace = ignore_talkpages
+
         return gen
```

### Comparing `pywikibot-8.0.4/pywikibot/site/_interwikimap.py` & `pywikibot-8.1.0/pywikibot/site/_interwikimap.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/site/_namespace.py` & `pywikibot-8.1.0/pywikibot/site/_namespace.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/site/_obsoletesites.py` & `pywikibot-8.1.0/pywikibot/site/_obsoletesites.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/site/_siteinfo.py` & `pywikibot-8.1.0/pywikibot/site/_siteinfo.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/site/_tokenwallet.py` & `pywikibot-8.1.0/pywikibot/site/_tokenwallet.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,16 @@
     """
 
     def __init__(self, site: 'APISite') -> None:
         """Initializer."""
         self.site: APISite = site
         self._tokens: Dict[str, str] = {}
         self._currentuser: Optional[str] = site.user()
+        # guess the needed token in update_tokens
+        self._last_token_key: Optional[str] = None
 
     def __getitem__(self, key: str) -> str:
         """Get token value for the given key."""
         if self.site.user() is None and key != 'login':
             self.site.login()
 
         if self.site.user() != self._currentuser:
@@ -54,14 +56,15 @@
         try:
             token = self._tokens[key]
         except KeyError:
             raise KeyError(
                 f'Invalid token {key!r} for user {self._currentuser!r} on '
                 f'{self.site} wiki.') from None
 
+        self._last_token_key = key
         return token
 
     def __contains__(self, key) -> bool:
         """Return True if the token name is cached for the current user."""
         try:
             self[key]
         except KeyError:
@@ -115,15 +118,15 @@
            r._params['token'] = r.site.tokens.update_tokens(r._params['token'])
 
         .. versionadded:: 8.0
         """
         # find the token types
         types = [key
                  for key, value in self._tokens.items() for token in tokens
-                 if value == token]
+                 if value == token] or [self._last_token_key]
         self.clear()  # clear the cache
         return [self[token_type] for token_type in types]
 
     @deprecated('clear()', since='8.0.0')
     def load_tokens(self, *args: Any, **kwargs: Any) -> None:
         """Clear cache to lazy load tokens when needed.
```

### Comparing `pywikibot-8.0.4/pywikibot/site/_upload.py` & `pywikibot-8.1.0/pywikibot/site/_upload.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/site_detect.py` & `pywikibot-8.1.0/pywikibot/site_detect.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from urllib.parse import urljoin, urlparse
 
 from requests.exceptions import RequestException
 
 import pywikibot
 from pywikibot.backports import removesuffix
 from pywikibot.comms.http import fetch
-from pywikibot.exceptions import ServerError
+from pywikibot.exceptions import ClientError, ServerError
 from pywikibot.tools import MediaWikiVersion
 
 
 try:
     from requests import JSONDecodeError
 except ImportError:  # requests < 2.27.0
     from json import JSONDecodeError
@@ -276,30 +276,36 @@
             if attrs['rel'] in ('EditURI', 'stylesheet', 'search'):
                 self.set_api_url(attrs['href'])
         elif tag == 'script' and 'src' in attrs:
             self.set_api_url(attrs['src'])
 
 
 def check_response(response):
-    """Raise ServerError if the response indicates a server error.
+    """Raise ClientError or ServerError depending on http status.
 
     .. versionadded:: 3.0
     .. versionchanged:: 7.0
-       Raise a generic ServerError if http status code is not
-       IANA-registered but unofficial code
-
-
+       Raise a generic :class:`exceptions.ServerError` if http status
+       code is not IANA-registered but unofficial code
+    .. versionchanged:: 8.1
+       Raise a :class:`exceptions.ClientError` if status code is 4XX
     """
-    if response.status_code >= HTTPStatus.INTERNAL_SERVER_ERROR:
-        try:
-            msg = HTTPStatus(response.status_code).phrase
-        except ValueError as err:
-            m = re.search(r'\d{3}', err.args[0], flags=re.ASCII)
-            if not m:
-                raise err
-            msg = f'Generic Server Error ({m.group()})'
+    for status_code, err_class, err_type in [
+        (HTTPStatus.INTERNAL_SERVER_ERROR, ServerError, 'Server'),
+        (HTTPStatus.BAD_REQUEST, ClientError, 'Client')
+    ]:  # highest http status code first
+        if response.status_code >= status_code:
+            try:
+                status = HTTPStatus(response.status_code)
+            except ValueError as err:
+                m = re.search(r'\d{3}', err.args[0], flags=re.ASCII)
+                if not m:
+                    raise err
+                msg = f'Generic {err_type} Error ({m.group()})'
+            else:
+                msg = f'({status}) {status.description}'
 
-        raise ServerError(msg)
+            raise err_class(msg)
 
     if response.status_code == HTTPStatus.OK \
        and SERVER_DB_ERROR_MSG in response.text:
         raise ServerError('Server cannot access the database')
```

### Comparing `pywikibot-8.0.4/pywikibot/specialbots/_unlink.py` & `pywikibot-8.1.0/pywikibot/specialbots/_unlink.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/specialbots/_upload.py` & `pywikibot-8.1.0/pywikibot/specialbots/_upload.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/textlib.py` & `pywikibot-8.1.0/pywikibot/textlib.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/throttle.py` & `pywikibot-8.1.0/pywikibot/throttle.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/time.py` & `pywikibot-8.1.0/pywikibot/time.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/titletranslate.py` & `pywikibot-8.1.0/pywikibot/titletranslate.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/tools/__init__.py` & `pywikibot-8.1.0/pywikibot/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/tools/_deprecate.py` & `pywikibot-8.1.0/pywikibot/tools/_deprecate.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/tools/_logging.py` & `pywikibot-8.1.0/pywikibot/tools/_logging.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/tools/_unidata.py` & `pywikibot-8.1.0/pywikibot/tools/_unidata.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/tools/chars.py` & `pywikibot-8.1.0/pywikibot/tools/chars.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/tools/collections.py` & `pywikibot-8.1.0/pywikibot/tools/collections.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/tools/djvu.py` & `pywikibot-8.1.0/pywikibot/tools/djvu.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/tools/formatter.py` & `pywikibot-8.1.0/pywikibot/tools/formatter.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/tools/itertools.py` & `pywikibot-8.1.0/pywikibot/tools/itertools.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/tools/threading.py` & `pywikibot-8.1.0/pywikibot/tools/threading.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/userinterfaces/__init__.py` & `pywikibot-8.1.0/pywikibot/userinterfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/userinterfaces/_interface_base.py` & `pywikibot-8.1.0/pywikibot/userinterfaces/_interface_base.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/userinterfaces/buffer_interface.py` & `pywikibot-8.1.0/pywikibot/userinterfaces/buffer_interface.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/userinterfaces/gui.py` & `pywikibot-8.1.0/pywikibot/userinterfaces/gui.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 """A window with a textfield where the user can edit.
 
 Useful for editing the contents of an article.
 
-.. note:: tkinter module is required
+.. note:: idlelib and tkinter modules are required
 """
 #
 # (C) Pywikibot team, 2003-2023
 #
 # Distributed under the terms of the MIT license.
 #
-from idlelib import replace as ReplaceDialog  # noqa: N812
-from idlelib import search as SearchDialog  # noqa: N812
-from idlelib.config import idleConf
-from idlelib.configdialog import ConfigDialog
-from idlelib.multicall import MultiCallCreator
 from typing import Optional
 
 import pywikibot
 from pywikibot.backports import Tuple
 from pywikibot.tools import PYTHON_VERSION
 
+try:
+    import idlelib
+except ImportError as e:
+    idlelib = e
+    ConfigDialog = ReplaceDialog = SearchDialog = object()
+    idleConf = MultiCallCreator = object()  # noqa:  N816
+else:
+    from idlelib import replace as ReplaceDialog  # noqa: N812
+    from idlelib import search as SearchDialog  # noqa: N812
+    from idlelib.config import idleConf
+    from idlelib.configdialog import ConfigDialog
+    from idlelib.multicall import MultiCallCreator
 
 try:
     import tkinter
 except ImportError as e:
     tkinter = e
     Frame = simpledialog = ScrolledText = object
 else:
@@ -45,16 +52,17 @@
 
     def __init__(self, master=None, **kwargs) -> None:
         """
         Initializer.
 
         Get default settings from user's IDLE configuration.
         """
-        if isinstance(tkinter, ImportError):
-            raise tkinter
+        for module in (idlelib, tkinter):
+            if isinstance(module, ImportError):
+                raise module
 
         textcf = self._initialize_config(idleConf.CurrentTheme())
 
         if idleConf.GetOption('main', 'EditorWindow', 'font-bold',
                               type='bool'):
             font_weight = 'bold'
         else:
@@ -278,16 +286,17 @@
 
 class EditBoxWindow(Frame):
 
     """Edit box window."""
 
     def __init__(self, parent=None, **kwargs) -> None:
         """Initializer."""
-        if isinstance(tkinter, ImportError):
-            raise tkinter
+        for module in (idlelib, tkinter):
+            if isinstance(module, ImportError):
+                raise module
 
         if parent is None:
             # create a new window
             parent = tkinter.Tk()
         self.parent = parent
         super().__init__(parent)
         self.editbox = MultiCallCreator(TextEditor)(self, **kwargs)
@@ -443,16 +452,17 @@
 
 class Tkdialog:
 
     """The dialog window for image info."""
 
     def __init__(self, photo_description, photo, filename) -> None:
         """Initializer."""
-        if isinstance(tkinter, ImportError):
-            raise tkinter
+        for module in (idlelib, tkinter):
+            if isinstance(module, ImportError):
+                raise module
 
         self.root = tkinter.Tk()
         # "%dx%d%+d%+d" % (width, height, xoffset, yoffset)
         self.root.geometry('{}x{}+10-10'
                            .format(int(pywikibot.config.tkhorsize),
                                    int(pywikibot.config.tkvertsize)))
```

### Comparing `pywikibot-8.0.4/pywikibot/userinterfaces/terminal_interface_base.py` & `pywikibot-8.1.0/pywikibot/userinterfaces/terminal_interface_base.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/userinterfaces/terminal_interface_unix.py` & `pywikibot-8.1.0/pywikibot/userinterfaces/terminal_interface_unix.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/userinterfaces/terminal_interface_win32.py` & `pywikibot-8.1.0/pywikibot/userinterfaces/terminal_interface_win32.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/userinterfaces/transliteration.py` & `pywikibot-8.1.0/pywikibot/userinterfaces/transliteration.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/version.py` & `pywikibot-8.1.0/pywikibot/version.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot/xmlreader.py` & `pywikibot-8.1.0/pywikibot/xmlreader.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot.egg-info/PKG-INFO` & `pywikibot-8.1.0/pywikibot.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywikibot
-Version: 8.0.4
+Version: 8.1.0
 Summary: Python MediaWiki Bot Framework
 Home-page: https://www.mediawiki.org/wiki/Manual:Pywikibot
 Download-URL: https://pywikibot.toolforge.org/
 Maintainer: The Pywikibot team
 Maintainer-email: pywikibot@lists.wikimedia.org
 License: MIT License
 Project-URL: Documentation, https://doc.wikimedia.org/pywikibot/stable/
@@ -257,22 +257,39 @@
 
 Roadmap
 =======
 
 Current release
 ---------------
 
-* L10N Updates
-* Minimal needed mwparserfromhell was decreased to 0.5.2 (T326498, T327600)
-* No longer lazy load password cookies (T271858, T326779, T329132, T330488, T331315)
+* generate_family_filescript was improved (T334775)
+* A ``quiet`` parameter was added to APISite.preloadpages()
+  which is True by default
+* Fix getting HTTPStatus enum in site_detect check_response (T334728)
+* Do not show a logging in message if password is entered (T178061)
+* Enable preleading ``Bot:`` prefix with twtranslate messages (T161459)
+* Disable command.log if -nolog option is given (T334381)
+* Guess the last needed token key if the token is not found (T334288)
+* Show parameters with APIError (T333957)
+* Raise exceptions.NoSiteLinkErrorinstead of exceptions.NoPageErrorwhen sitelink
+  is missing in ItemPage.getSitelink()(T332341)
+* exceptions.ClientErrorwas added
+* Raise exceptions.NoPageErrorwhen deleting a missing Page (T332924)
+* ``text`` parameter of proofreadpage.PagesTagParserhas a default value
+* L10N updates
+* Ignore talk pages with APISite.watched_pages()(T330806)
+* Load page info when creating a page if not updated previously (T330980)
+* Improve flush exception logging
 
 
 Deprecations
 ------------
 
+* 8.1.0: Dependency of exceptions.NoSiteLinkErrorfrom exceptions.NoPageErrorwill be removed
+* 8.1.0: ``exceptions.Server414Error`` is deprecated in favour of exceptions.Client414Error
 * 8.0.0: Timestamp.clone()method is deprecated
   in favour of ``Timestamp.replace()`` method.
 * 8.0.0: family.Family.maximum_GET_lengthmethod is deprecated in favour of
   config.maximum_GET_length(T325957)
 * 8.0.0: ``addOnly`` parameter of textlib.replaceLanguageLinksand
   textlib.replaceCategoryLinksare deprecated in favour of ``add_only``
 * 8.0.0: textlib.TimeStripperregex attributes ``ptimeR``, ``ptimeznR``, ``pyearR``, ``pmonthR``,
```

### Comparing `pywikibot-8.0.4/pywikibot.egg-info/SOURCES.txt` & `pywikibot-8.1.0/pywikibot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/pywikibot.egg-info/requires.txt` & `pywikibot-8.1.0/pywikibot.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/setup.py` & `pywikibot-8.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `pywikibot-8.0.4/tests/tests_tests.py` & `pywikibot-8.1.0/tests/tests_tests.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,27 +54,27 @@
     def test_assert_is_not_empty(self):
         """Test assertIsNotEmpty method."""
         self.assertIsNotEmpty(self.seq1)
         self.assertIsNotEmpty(self.seq2)
 
     @unittest.expectedFailure
     def test_assert_is_not_empty_fail(self):
-        """Test assertIsNotEmpty method."""
+        """Test that assertIsNotEmpty method may fail."""
         self.assertIsNotEmpty([])
         self.assertIsNotEmpty('')
 
     def test_assert_length(self):
-        """Test assertIsNotEmpty method."""
+        """Test assertLength method."""
         self.assertLength([], 0)
         self.assertLength(self.seq1, 3)
         self.assertLength(self.seq1, self.seq2)
 
     @unittest.expectedFailure
     def test_assert_length_fail(self):
-        """Test assertIsNotEmpty method."""
+        """Test that assertLength method is failing."""
         self.assertLength([], 1)
         self.assertLength(self.seq1, 0)
         self.assertLength(None, self.seq)
 
 
 class UtilsTests(TestCase):
```

