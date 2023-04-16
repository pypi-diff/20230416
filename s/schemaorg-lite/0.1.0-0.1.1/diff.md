# Comparing `tmp/schemaorg_lite-0.1.0.tar.gz` & `tmp/schemaorg_lite-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schemaorg_lite-0.1.0.tar", last modified: Sun Apr 16 04:42:19 2023, max compression
+gzip compressed data, was "schemaorg_lite-0.1.1.tar", last modified: Sun Apr 16 15:35:52 2023, max compression
```

## Comparing `schemaorg_lite-0.1.0.tar` & `schemaorg_lite-0.1.1.tar`

### file list

```diff
@@ -1,249 +1,247 @@
--rw-r--r--   0        0        0     1949 2023-04-16 04:35:04.054230 schemaorg_lite-0.1.0/README.md
--rw-r--r--   0        0        0     1756 2023-04-16 04:42:19.748019 schemaorg_lite-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-13 08:01:43.682908 schemaorg_lite-0.1.0/schemaorg/__init__.py
--rw-r--r--   0        0        0     4546 2023-04-13 08:01:43.683147 schemaorg_lite-0.1.0/schemaorg/data/__init__.py
--rw-r--r--   0        0        0     1172 2023-04-13 08:01:43.683440 schemaorg_lite-0.1.0/schemaorg/data/ext/attic/attic.ttl
--rw-r--r--   0        0        0    15040 2023-04-13 08:01:43.683599 schemaorg_lite-0.1.0/schemaorg/data/ext/auto/auto.ttl
--rw-r--r--   0        0        0     8238 2023-04-13 08:01:43.683857 schemaorg_lite-0.1.0/schemaorg/data/ext/bib/bsdo-1.0.ttl
--rw-r--r--   0        0        0     1877 2023-04-13 08:01:43.684052 schemaorg_lite-0.1.0/schemaorg/data/ext/bib/bsdo-atlas-examples.txt
--rw-r--r--   0        0        0     7042 2023-04-13 08:01:43.684260 schemaorg_lite-0.1.0/schemaorg/data/ext/bib/bsdo-audiobook-examples.txt
--rw-r--r--   0        0        0     2488 2023-04-13 08:01:43.684467 schemaorg_lite-0.1.0/schemaorg/data/ext/bib/bsdo-chapter-examples.txt
--rw-r--r--   0        0        0     6616 2023-04-13 08:01:43.684673 schemaorg_lite-0.1.0/schemaorg/data/ext/bib/bsdo-collection-examples.txt
--rw-r--r--   0        0        0     1833 2023-04-13 08:01:43.684867 schemaorg_lite-0.1.0/schemaorg/data/ext/bib/bsdo-newspaper-examples.txt
--rw-r--r--   0        0        0     1830 2023-04-13 08:01:43.684995 schemaorg_lite-0.1.0/schemaorg/data/ext/bib/bsdo-thesis-examples.txt
--rw-r--r--   0        0        0     4832 2023-04-13 08:01:43.685114 schemaorg_lite-0.1.0/schemaorg/data/ext/bib/bsdo-translation-examples.txt
--rw-r--r--   0        0        0     6636 2023-04-13 08:01:43.685263 schemaorg_lite-0.1.0/schemaorg/data/ext/bib/comics-examples.txt
--rw-r--r--   0        0        0     6731 2023-04-13 08:01:43.685464 schemaorg_lite-0.1.0/schemaorg/data/ext/health-lifesci/MedicalScholarlyArticle-examples.txt
--rw-r--r--   0        0        0    11809 2023-04-13 08:01:43.685736 schemaorg_lite-0.1.0/schemaorg/data/ext/health-lifesci/drug-example.txt
--rw-r--r--   0        0        0   111243 2023-04-13 08:01:43.686364 schemaorg_lite-0.1.0/schemaorg/data/ext/health-lifesci/med-health-core.ttl
--rw-r--r--   0        0        0    12613 2023-04-13 08:01:43.686665 schemaorg_lite-0.1.0/schemaorg/data/ext/health-lifesci/medicalCondition-examples.txt
--rw-r--r--   0        0        0     4079 2023-04-13 08:01:43.687068 schemaorg_lite-0.1.0/schemaorg/data/ext/health-lifesci/medicalGuideline-examples.txt
--rw-r--r--   0        0        0     3512 2023-04-13 08:01:43.687302 schemaorg_lite-0.1.0/schemaorg/data/ext/health-lifesci/medicalWebpage-examples.txt
--rw-r--r--   0        0        0     6390 2023-04-13 08:01:43.687545 schemaorg_lite-0.1.0/schemaorg/data/ext/health-lifesci/physical-activity-and-exercise.ttl
--rw-r--r--   0        0        0     3106 2023-04-13 08:01:43.687825 schemaorg_lite-0.1.0/schemaorg/data/ext/meta/meta.jsonld.someday.txt
--rw-r--r--   0        0        0     2392 2023-04-13 08:01:43.688103 schemaorg_lite-0.1.0/schemaorg/data/ext/meta/meta.ttl
--rw-r--r--   0        0        0     1043 2023-04-13 08:01:43.688374 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1045-examples.txt
--rw-r--r--   0        0        0     1204 2023-04-13 08:01:43.688643 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1045.ttl
--rw-r--r--   0        0        0      520 2023-04-13 08:01:43.688819 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1050-examples.txt
--rw-r--r--   0        0        0      683 2023-04-13 08:01:43.689005 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1050.ttl
--rw-r--r--   0        0        0     4270 2023-04-13 08:01:43.689180 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1062-examples.txt
--rw-r--r--   0        0        0     8854 2023-04-13 08:01:43.689445 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1062.ttl
--rw-r--r--   0        0        0      749 2023-04-13 08:01:43.689662 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1083.ttl
--rw-r--r--   0        0        0    15348 2023-04-13 08:01:43.689875 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1156-examples.txt
--rw-r--r--   0        0        0    16540 2023-04-13 08:01:43.690166 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1156.ttl
--rw-r--r--   0        0        0     2235 2023-04-13 08:01:43.690949 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1244.ttl
--rw-r--r--   0        0        0    14646 2023-04-13 08:01:43.691231 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1253-examples.txt
--rw-r--r--   0        0        0    13369 2023-04-13 08:01:43.691369 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1253.ttl
--rw-r--r--   0        0        0     5291 2023-04-13 08:01:43.691599 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1375.ttl
--rw-r--r--   0        0        0     1329 2023-04-13 08:01:43.691827 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1389-examples.txt
--rw-r--r--   0        0        0     1177 2023-04-13 08:01:43.692104 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1397.ttl
--rw-r--r--   0        0        0     1477 2023-04-13 08:01:43.692281 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1401.ttl
--rw-r--r--   0        0        0      693 2023-04-13 08:01:43.692461 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1423-examples.txt
--rw-r--r--   0        0        0     1210 2023-04-13 08:01:43.692688 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1423.ttl
--rw-r--r--   0        0        0     1583 2023-04-13 08:01:43.692916 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1425.ttl
--rw-r--r--   0        0        0     1494 2023-04-13 08:01:43.693194 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1448.ttl
--rw-r--r--   0        0        0     3998 2023-04-13 08:01:43.693434 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1457-examples.txt
--rw-r--r--   0        0        0     5565 2023-04-13 08:01:43.693684 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1457.ttl
--rw-r--r--   0        0        0      563 2023-04-13 08:01:43.694214 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1495.ttl
--rw-r--r--   0        0        0     1909 2023-04-13 08:01:43.694651 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1525-examples.txt
--rw-r--r--   0        0        0    12791 2023-04-13 08:01:43.695062 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1525.ttl
--rw-r--r--   0        0        0      573 2023-04-13 08:01:43.695372 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1559.ttl
--rw-r--r--   0        0        0      640 2023-04-13 08:01:43.695603 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1576.ttl
--rw-r--r--   0        0        0     1423 2023-04-13 08:01:43.695790 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1589.ttl
--rw-r--r--   0        0        0      596 2023-04-13 08:01:43.695959 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1591.ttl
--rw-r--r--   0        0        0      695 2023-04-13 08:01:43.696148 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1624.ttl
--rw-r--r--   0        0        0      365 2023-04-13 08:01:43.696448 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1670-examples.txt
--rw-r--r--   0        0        0      809 2023-04-13 08:01:43.696669 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1672.ttl
--rw-r--r--   0        0        0     3007 2023-04-13 08:01:43.696829 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1688.ttl
--rw-r--r--   0        0        0      989 2023-04-13 08:01:43.696998 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1689-examples.txt
--rw-r--r--   0        0        0     2997 2023-04-13 08:01:43.697191 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1698-examples.txt
--rw-r--r--   0        0        0     1121 2023-04-13 08:01:43.697411 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1741-examples.txt
--rw-r--r--   0        0        0     1915 2023-04-13 08:01:43.697665 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1755.ttl
--rw-r--r--   0        0        0    15775 2023-04-13 08:01:43.697880 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1758-examples.txt
--rw-r--r--   0        0        0     2263 2023-04-13 08:01:43.698153 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1758.ttl
--rw-r--r--   0        0        0     3023 2023-04-13 08:01:43.698337 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1759-examples.txt
--rw-r--r--   0        0        0      967 2023-04-13 08:01:43.698497 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1759.ttl
--rw-r--r--   0        0        0    10050 2023-04-13 08:01:43.698691 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1779-examples.txt
--rw-r--r--   0        0        0     3567 2023-04-13 08:01:43.698861 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1779.ttl
--rw-r--r--   0        0        0     4042 2023-04-13 08:01:43.699068 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1797.ttl
--rw-r--r--   0        0        0    47424 2023-04-13 08:01:43.699403 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1810-examples.txt
--rw-r--r--   0        0        0     4081 2023-04-13 08:01:43.699619 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1810.ttl
--rw-r--r--   0        0        0      739 2023-04-13 08:01:43.699839 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1816.ttl
--rw-r--r--   0        0        0     2113 2023-04-13 08:01:43.700021 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1828.ttl
--rw-r--r--   0        0        0     3227 2023-04-13 08:01:43.700224 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1842-examples.txt
--rw-r--r--   0        0        0     3574 2023-04-13 08:01:43.700425 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1842.ttl
--rw-r--r--   0        0        0     1732 2023-04-13 08:01:43.700686 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1886.ttl
--rw-r--r--   0        0        0      764 2023-04-13 08:01:43.700912 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1909.ttl
--rw-r--r--   0        0        0     1039 2023-04-13 08:01:43.701111 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1950-examples.txt
--rw-r--r--   0        0        0     1309 2023-04-13 08:01:43.701343 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1950.ttl
--rw-r--r--   0        0        0      454 2023-04-13 08:01:43.701655 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1951.ttl
--rw-r--r--   0        0        0      569 2023-04-13 08:01:43.701840 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1976.ttl
--rw-r--r--   0        0        0      407 2023-04-13 08:01:43.702019 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2021-examples.txt
--rw-r--r--   0        0        0      943 2023-04-13 08:01:43.702220 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2021.ttl
--rw-r--r--   0        0        0      460 2023-04-13 08:01:43.702484 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2083-examples.txt
--rw-r--r--   0        0        0      785 2023-04-13 08:01:43.702743 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2083.ttl
--rw-r--r--   0        0        0      391 2023-04-13 08:01:43.702953 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2085-examples.txt
--rw-r--r--   0        0        0      738 2023-04-13 08:01:43.703207 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2085.ttl
--rw-r--r--   0        0        0      861 2023-04-13 08:01:43.703511 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2108-examples.txt
--rw-r--r--   0        0        0     1723 2023-04-13 08:01:43.703783 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2108.ttl
--rw-r--r--   0        0        0      288 2023-04-13 08:01:43.704062 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2109-examples.txt
--rw-r--r--   0        0        0     1095 2023-04-13 08:01:43.704365 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2109.ttl
--rw-r--r--   0        0        0      667 2023-04-13 08:01:43.704592 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2110.ttl
--rw-r--r--   0        0        0      995 2023-04-13 08:01:43.704849 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2111.ttl
--rw-r--r--   0        0        0      639 2023-04-13 08:01:43.705042 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2126.ttl
--rw-r--r--   0        0        0     1114 2023-04-13 08:01:43.705222 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2140.ttl
--rw-r--r--   0        0        0     1609 2023-04-13 08:01:43.705502 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2173-examples.txt
--rw-r--r--   0        0        0      954 2023-04-13 08:01:43.705693 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2173.ttl
--rw-r--r--   0        0        0     1627 2023-04-13 08:01:43.705888 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2192-examples.txt
--rw-r--r--   0        0        0      588 2023-04-13 08:01:43.706061 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2192.ttl
--rw-r--r--   0        0        0      623 2023-04-13 08:01:43.706234 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2242.ttl
--rw-r--r--   0        0        0     1100 2023-04-13 08:01:43.706606 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2244.ttl
--rw-r--r--   0        0        0     3793 2023-04-13 08:01:43.706807 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2288.ttl
--rw-r--r--   0        0        0     3407 2023-04-13 08:01:43.706998 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2289-examples.txt
--rw-r--r--   0        0        0     5154 2023-04-13 08:01:43.707271 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2289.ttl
--rw-r--r--   0        0        0     5585 2023-04-13 08:01:43.707476 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2291.ttl
--rw-r--r--   0        0        0      709 2023-04-13 08:01:43.707665 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2294-examples.txt
--rw-r--r--   0        0        0      758 2023-04-13 08:01:43.707842 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2296-examples.txt
--rw-r--r--   0        0        0      645 2023-04-13 08:01:43.708010 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2296.ttl
--rw-r--r--   0        0        0      776 2023-04-13 08:01:43.708187 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2300.ttl
--rw-r--r--   0        0        0     1403 2023-04-13 08:01:43.708510 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2311.ttl
--rw-r--r--   0        0        0      664 2023-04-13 08:01:43.708822 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2329.ttl
--rw-r--r--   0        0        0      455 2023-04-13 08:01:43.710376 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2341.ttl
--rw-r--r--   0        0        0     1825 2023-04-13 08:01:43.710634 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2348.ttl
--rw-r--r--   0        0        0      994 2023-04-13 08:01:43.710935 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2358.ttl
--rw-r--r--   0        0        0     2528 2023-04-13 08:01:43.711136 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2366-examples.txt
--rw-r--r--   0        0        0     8265 2023-04-13 08:01:43.711356 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2373.ttl
--rw-r--r--   0        0        0    11319 2023-04-13 08:01:43.711576 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2374.ttl
--rw-r--r--   0        0        0    15964 2023-04-13 08:01:43.711800 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2381.ttl
--rw-r--r--   0        0        0      424 2023-04-13 08:01:43.712035 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2382.ttl
--rw-r--r--   0        0        0     1022 2023-04-13 08:01:43.712206 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2384-examples.txt
--rw-r--r--   0        0        0     2154 2023-04-13 08:01:43.712382 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2384.ttl
--rw-r--r--   0        0        0      678 2023-04-13 08:01:43.712683 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2394.ttl
--rw-r--r--   0        0        0     1684 2023-04-13 08:01:43.712888 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2396-examples.txt
--rw-r--r--   0        0        0      963 2023-04-13 08:01:43.713106 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2396.ttl
--rw-r--r--   0        0        0    12843 2023-04-13 08:01:43.713400 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2405-examples.txt
--rw-r--r--   0        0        0     1669 2023-04-13 08:01:43.713635 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2405.ttl
--rw-r--r--   0        0        0      684 2023-04-13 08:01:43.713895 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2418.ttl
--rw-r--r--   0        0        0      659 2023-04-13 08:01:43.715639 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2419-examples.txt
--rw-r--r--   0        0        0     4492 2023-04-13 08:01:43.715980 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2419.ttl
--rw-r--r--   0        0        0      411 2023-04-13 08:01:43.716348 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2420.ttl
--rw-r--r--   0        0        0     1308 2023-04-13 08:01:43.716552 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2421-examples.txt
--rw-r--r--   0        0        0      457 2023-04-13 08:01:43.716720 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2421.ttl
--rw-r--r--   0        0        0     1094 2023-04-13 08:01:43.716918 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2427.ttl
--rw-r--r--   0        0        0     1588 2023-04-13 08:01:43.717143 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2450-examples.txt
--rw-r--r--   0        0        0    18209 2023-04-13 08:01:43.717439 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2450.ttl
--rw-r--r--   0        0        0     1796 2023-04-13 08:01:43.717732 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2454.ttl
--rw-r--r--   0        0        0     1137 2023-04-13 08:01:43.717989 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2460.ttl
--rw-r--r--   0        0        0     2129 2023-04-13 08:01:43.718278 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2469.ttl
--rw-r--r--   0        0        0     3065 2023-04-13 08:01:43.718471 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2482-examples.txt
--rw-r--r--   0        0        0      818 2023-04-13 08:01:43.718718 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2483.ttl
--rw-r--r--   0        0        0      511 2023-04-13 08:01:43.718940 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2486.ttl
--rw-r--r--   0        0        0     3602 2023-04-13 08:01:43.719234 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2490-examples.txt
--rw-r--r--   0        0        0     9453 2023-04-13 08:01:43.719554 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2490.ttl
--rw-r--r--   0        0        0      511 2023-04-13 08:01:43.719765 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2493.ttl
--rw-r--r--   0        0        0      428 2023-04-13 08:01:43.719950 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2496.ttl
--rw-r--r--   0        0        0      577 2023-04-13 08:01:43.720159 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2500.ttl
--rw-r--r--   0        0        0    12915 2023-04-13 08:01:43.720510 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2506.ttl
--rw-r--r--   0        0        0     1342 2023-04-13 08:01:43.720779 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2514-examples.txt
--rw-r--r--   0        0        0      894 2023-04-13 08:01:43.721032 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2514.ttl
--rw-r--r--   0        0        0     7821 2023-04-13 08:01:43.721247 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2521.ttl
--rw-r--r--   0        0        0      537 2023-04-13 08:01:43.721497 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2526.ttl
--rw-r--r--   0        0        0     1361 2023-04-13 08:01:43.721748 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2534-examples.txt
--rw-r--r--   0        0        0     3814 2023-04-13 08:01:43.721968 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2534.ttl
--rw-r--r--   0        0        0      713 2023-04-13 08:01:43.722176 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2543-examples.txt
--rw-r--r--   0        0        0    14775 2023-04-13 08:01:43.722438 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2543.ttl
--rw-r--r--   0        0        0      672 2023-04-13 08:01:43.722646 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2599-examples.txt
--rw-r--r--   0        0        0      754 2023-04-13 08:01:43.722838 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2599.ttl
--rw-r--r--   0        0        0      681 2023-04-13 08:01:43.723019 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2605.ttl
--rw-r--r--   0        0        0      525 2023-04-13 08:01:43.723212 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2611.ttl
--rw-r--r--   0        0        0      731 2023-04-13 08:01:43.723417 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2636.ttl
--rw-r--r--   0        0        0      604 2023-04-13 08:01:43.723643 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2646.ttl
--rw-r--r--   0        0        0     1036 2023-04-13 08:01:43.723855 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2659.ttl
--rw-r--r--   0        0        0      695 2023-04-13 08:01:43.724045 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2665.ttl
--rw-r--r--   0        0        0     7939 2023-04-13 08:01:43.724275 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2670.ttl
--rw-r--r--   0        0        0      711 2023-04-13 08:01:43.724485 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2681-examples.txt
--rw-r--r--   0        0        0     1569 2023-04-13 08:01:43.724681 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2681.ttl
--rw-r--r--   0        0        0     4149 2023-04-13 08:01:43.724871 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2689.ttl
--rw-r--r--   0        0        0      862 2023-04-13 08:01:43.725038 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-271-examples.txt
--rw-r--r--   0        0        0     1200 2023-04-13 08:01:43.725215 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-271.ttl
--rw-r--r--   0        0        0     2401 2023-04-13 08:01:43.725409 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2712.ttl
--rw-r--r--   0        0        0      582 2023-04-13 08:01:43.725586 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2722-example.txt
--rw-r--r--   0        0        0      684 2023-04-13 08:01:43.726650 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2722.ttl
--rw-r--r--   0        0        0      912 2023-04-13 08:01:43.726975 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2740-examples.txt
--rw-r--r--   0        0        0     1423 2023-04-13 08:01:43.727256 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2740.ttl
--rw-r--r--   0        0        0      579 2023-04-13 08:01:43.727478 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-276.ttl
--rw-r--r--   0        0        0     3012 2023-04-13 08:01:43.727654 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2766.ttl
--rw-r--r--   0        0        0     2577 2023-04-13 08:01:43.727873 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2811-examples.txt
--rw-r--r--   0        0        0    23965 2023-04-13 08:01:43.728115 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2811.ttl
--rw-r--r--   0        0        0     1024 2023-04-13 08:01:43.728463 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2832-examples.txt
--rw-r--r--   0        0        0     2101 2023-04-13 08:01:43.728696 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2832.ttl
--rw-r--r--   0        0        0      837 2023-04-13 08:01:43.729150 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2862-examples.txt
--rw-r--r--   0        0        0    17229 2023-04-13 08:01:43.729470 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2862.ttl
--rw-r--r--   0        0        0      669 2023-04-13 08:01:43.729915 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2877.ttl
--rw-r--r--   0        0        0      966 2023-04-13 08:01:43.730180 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2907.ttl
--rw-r--r--   0        0        0      784 2023-04-13 08:01:43.730446 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2912.ttl
--rw-r--r--   0        0        0      845 2023-04-13 08:01:43.730691 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2915.ttl
--rw-r--r--   0        0        0      712 2023-04-13 08:01:43.730893 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2927.ttl
--rw-r--r--   0        0        0     4844 2023-04-13 08:01:43.731088 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2989.ttl
--rw-r--r--   0        0        0      677 2023-04-13 08:01:43.731258 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-3001.ttl
--rw-r--r--   0        0        0     1006 2023-04-13 08:01:43.731436 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-3028-examples.txt
--rw-r--r--   0        0        0     1007 2023-04-13 08:01:43.731643 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-3028.ttl
--rw-r--r--   0        0        0      556 2023-04-13 08:01:43.731834 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-3052.ttl
--rw-r--r--   0        0        0     2446 2023-04-13 08:01:43.732030 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-3057.ttl
--rw-r--r--   0        0        0     1925 2023-04-13 08:01:43.732295 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-3058.ttl
--rw-r--r--   0        0        0     1177 2023-04-13 08:01:43.732510 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-3123.ttl
--rw-r--r--   0        0        0     1530 2023-04-13 08:01:43.732693 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-3134.ttl
--rw-r--r--   0        0        0      876 2023-04-13 08:01:43.732864 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-3135-examples.txt
--rw-r--r--   0        0        0      794 2023-04-13 08:01:43.733142 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-3135.ttl
--rw-r--r--   0        0        0     5409 2023-04-13 08:01:43.733340 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-373-examples.txt
--rw-r--r--   0        0        0     1661 2023-04-13 08:01:43.733577 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-373.ttl
--rw-r--r--   0        0        0     5952 2023-04-13 08:01:43.733795 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-383-examples.txt
--rw-r--r--   0        0        0     5541 2023-04-13 08:01:43.734020 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-383.ttl
--rw-r--r--   0        0        0     1616 2023-04-13 08:01:43.734206 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-447-examples.txt
--rw-r--r--   0        0        0     1625 2023-04-13 08:01:43.734367 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-447.ttl
--rw-r--r--   0        0        0    10722 2023-04-13 08:01:43.734567 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-894-examples.txt
--rw-r--r--   0        0        0     3867 2023-04-13 08:01:43.734858 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-894.ttl
--rw-r--r--   0        0        0      768 2023-04-13 08:01:43.735085 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-987.ttl
--rw-r--r--   0        0        0     1065 2023-04-13 08:01:43.735300 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-991.ttl
--rw-r--r--   0        0        0      251 2023-04-13 08:01:43.735503 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-template-examples.txt
--rw-r--r--   0        0        0      141 2023-04-13 08:01:43.735672 schemaorg_lite-0.1.0/schemaorg/data/ext/pending/pending-header.jsonld
--rw-r--r--   0        0        0   410358 2023-04-13 08:01:43.737975 schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/httpequivs.ttl
--rw-r--r--   0        0        0  2962722 2023-04-13 08:01:43.752851 schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schema-all.html
--rw-r--r--   0        0        0  1015192 2023-04-13 08:01:43.761478 schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-all-examples.txt
--rw-r--r--   0        0        0   461447 2023-04-13 08:01:43.765263 schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-all-http-properties.csv
--rw-r--r--   0        0        0  2176246 2023-04-13 08:01:43.779595 schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-all-http-types.csv
--rw-r--r--   0        0        0  1400370 2023-04-13 08:01:43.789260 schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-all-http.jsonld
--rw-r--r--   0        0        0  2502842 2023-04-13 08:01:43.798935 schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-all-http.nq
--rw-r--r--   0        0        0  2094592 2023-04-13 08:01:43.806733 schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-all-http.nt
--rw-r--r--   0        0        0  1388115 2023-04-13 08:01:43.815039 schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-all-http.rdf
--rw-r--r--   0        0        0  1000440 2023-04-13 08:01:43.820580 schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-all-http.ttl
--rw-r--r--   0        0        0   467969 2023-04-13 08:01:43.821812 schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-all-https-properties.csv
--rw-r--r--   0        0        0  2237356 2023-04-13 08:01:43.830981 schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-all-https-types.csv
--rw-r--r--   0        0        0  1401553 2023-04-13 08:01:43.833298 schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-all-https.jsonld
--rw-r--r--   0        0        0  2549224 2023-04-13 08:01:43.838886 schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-all-https.nq
--rw-r--r--   0        0        0  2124644 2023-04-13 08:01:43.845950 schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-all-https.nt
--rw-r--r--   0        0        0  1397406 2023-04-13 08:01:43.851802 schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-all-https.rdf
--rw-r--r--   0        0        0  1001623 2023-04-13 08:01:43.853503 schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-all-https.ttl
--rw-r--r--   0        0        0   459750 2023-04-13 08:01:43.854914 schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-current-http-properties.csv
--rw-r--r--   0        0        0  2173210 2023-04-13 08:01:43.861402 schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-current-http-types.csv
--rw-r--r--   0        0        0  1393407 2023-04-13 08:01:43.868361 schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-current-http.jsonld
--rw-r--r--   0        0        0  2490302 2023-04-13 08:01:43.875993 schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-current-http.nq
--rw-r--r--   0        0        0  2084102 2023-04-13 08:01:43.882530 schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-current-http.nt
--rw-r--r--   0        0        0  1381444 2023-04-13 08:01:43.885799 schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-current-http.rdf
--rw-r--r--   0        0        0   995515 2023-04-13 08:01:43.888969 schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-current-http.ttl
--rw-r--r--   0        0        0   466246 2023-04-13 08:01:43.890385 schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-current-https-properties.csv
--rw-r--r--   0        0        0  2234262 2023-04-13 08:01:43.897684 schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-current-https-types.csv
--rw-r--r--   0        0        0  1394578 2023-04-13 08:01:43.899929 schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-current-https.jsonld
--rw-r--r--   0        0        0  2536436 2023-04-13 08:01:43.903668 schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-current-https.nq
--rw-r--r--   0        0        0  2113988 2023-04-13 08:01:43.911036 schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-current-https.nt
--rw-r--r--   0        0        0  1390690 2023-04-13 08:01:43.913298 schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-current-https.rdf
--rw-r--r--   0        0        0   996686 2023-04-13 08:01:43.914998 schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-current-https.ttl
--rw-r--r--   0        0        0   343608 2023-04-13 08:01:43.916598 schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-shapes.shacl
--rw-r--r--   0        0        0   946637 2023-04-13 08:01:43.920801 schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-shapes.shexj
--rw-r--r--   0        0        0    58391 2023-04-13 08:01:43.921508 schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-subclasses.shacl
--rw-r--r--   0        0        0  1901171 2023-04-13 08:01:43.927780 schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg.owl
--rw-r--r--   0        0        0   172009 2023-04-13 08:01:43.928961 schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorgcontext.jsonld
--rw-r--r--   0        0        0     9245 2023-04-13 08:01:43.929314 schemaorg_lite-0.1.0/schemaorg/main.py
--rw-r--r--   0        0        0     1402 2023-04-13 08:01:43.929637 schemaorg_lite-0.1.0/schemaorg/tests/recipe.yml
--rw-r--r--   0        0        0     2379 2023-04-13 08:01:43.929889 schemaorg_lite-0.1.0/schemaorg/tests/test_schema.py
--rw-r--r--   0        0        0     3017 1970-01-01 00:00:00.000000 schemaorg_lite-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      548 2023-04-16 15:33:33.383589 schemaorg_lite-0.1.1/README.md
+-rw-r--r--   0        0        0     1860 2023-04-16 15:35:52.181578 schemaorg_lite-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-13 08:01:43.682908 schemaorg_lite-0.1.1/schemaorg_lite/__init__.py
+-rw-r--r--   0        0        0     4586 2023-04-16 15:00:59.358171 schemaorg_lite-0.1.1/schemaorg_lite/data/__init__.py
+-rw-r--r--   0        0        0     1172 2023-04-13 08:01:43.683440 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/attic/attic.ttl
+-rw-r--r--   0        0        0    15040 2023-04-13 08:01:43.683599 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/auto/auto.ttl
+-rw-r--r--   0        0        0     8238 2023-04-13 08:01:43.683857 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/bib/bsdo-1.0.ttl
+-rw-r--r--   0        0        0     1877 2023-04-13 08:01:43.684052 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/bib/bsdo-atlas-examples.txt
+-rw-r--r--   0        0        0     7042 2023-04-13 08:01:43.684260 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/bib/bsdo-audiobook-examples.txt
+-rw-r--r--   0        0        0     2488 2023-04-13 08:01:43.684467 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/bib/bsdo-chapter-examples.txt
+-rw-r--r--   0        0        0     6616 2023-04-13 08:01:43.684673 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/bib/bsdo-collection-examples.txt
+-rw-r--r--   0        0        0     1833 2023-04-13 08:01:43.684867 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/bib/bsdo-newspaper-examples.txt
+-rw-r--r--   0        0        0     1830 2023-04-13 08:01:43.684995 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/bib/bsdo-thesis-examples.txt
+-rw-r--r--   0        0        0     4832 2023-04-13 08:01:43.685114 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/bib/bsdo-translation-examples.txt
+-rw-r--r--   0        0        0     6636 2023-04-13 08:01:43.685263 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/bib/comics-examples.txt
+-rw-r--r--   0        0        0     6731 2023-04-13 08:01:43.685464 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/health-lifesci/MedicalScholarlyArticle-examples.txt
+-rw-r--r--   0        0        0    11809 2023-04-13 08:01:43.685736 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/health-lifesci/drug-example.txt
+-rw-r--r--   0        0        0   111243 2023-04-13 08:01:43.686364 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/health-lifesci/med-health-core.ttl
+-rw-r--r--   0        0        0    12613 2023-04-13 08:01:43.686665 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/health-lifesci/medicalCondition-examples.txt
+-rw-r--r--   0        0        0     4079 2023-04-13 08:01:43.687068 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/health-lifesci/medicalGuideline-examples.txt
+-rw-r--r--   0        0        0     3512 2023-04-13 08:01:43.687302 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/health-lifesci/medicalWebpage-examples.txt
+-rw-r--r--   0        0        0     6390 2023-04-13 08:01:43.687545 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/health-lifesci/physical-activity-and-exercise.ttl
+-rw-r--r--   0        0        0     3106 2023-04-13 08:01:43.687825 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/meta/meta.jsonld.someday.txt
+-rw-r--r--   0        0        0     2392 2023-04-13 08:01:43.688103 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/meta/meta.ttl
+-rw-r--r--   0        0        0     1043 2023-04-13 08:01:43.688374 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1045-examples.txt
+-rw-r--r--   0        0        0     1204 2023-04-13 08:01:43.688643 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1045.ttl
+-rw-r--r--   0        0        0      520 2023-04-13 08:01:43.688819 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1050-examples.txt
+-rw-r--r--   0        0        0      683 2023-04-13 08:01:43.689005 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1050.ttl
+-rw-r--r--   0        0        0     4270 2023-04-13 08:01:43.689180 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1062-examples.txt
+-rw-r--r--   0        0        0     8854 2023-04-13 08:01:43.689445 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1062.ttl
+-rw-r--r--   0        0        0      749 2023-04-13 08:01:43.689662 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1083.ttl
+-rw-r--r--   0        0        0    15348 2023-04-13 08:01:43.689875 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1156-examples.txt
+-rw-r--r--   0        0        0    16540 2023-04-13 08:01:43.690166 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1156.ttl
+-rw-r--r--   0        0        0     2235 2023-04-13 08:01:43.690949 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1244.ttl
+-rw-r--r--   0        0        0    14646 2023-04-13 08:01:43.691231 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1253-examples.txt
+-rw-r--r--   0        0        0    13369 2023-04-13 08:01:43.691369 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1253.ttl
+-rw-r--r--   0        0        0     5291 2023-04-13 08:01:43.691599 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1375.ttl
+-rw-r--r--   0        0        0     1329 2023-04-13 08:01:43.691827 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1389-examples.txt
+-rw-r--r--   0        0        0     1177 2023-04-13 08:01:43.692104 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1397.ttl
+-rw-r--r--   0        0        0     1477 2023-04-13 08:01:43.692281 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1401.ttl
+-rw-r--r--   0        0        0      693 2023-04-13 08:01:43.692461 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1423-examples.txt
+-rw-r--r--   0        0        0     1210 2023-04-13 08:01:43.692688 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1423.ttl
+-rw-r--r--   0        0        0     1583 2023-04-13 08:01:43.692916 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1425.ttl
+-rw-r--r--   0        0        0     1494 2023-04-13 08:01:43.693194 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1448.ttl
+-rw-r--r--   0        0        0     3998 2023-04-13 08:01:43.693434 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1457-examples.txt
+-rw-r--r--   0        0        0     5565 2023-04-13 08:01:43.693684 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1457.ttl
+-rw-r--r--   0        0        0      563 2023-04-13 08:01:43.694214 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1495.ttl
+-rw-r--r--   0        0        0     1909 2023-04-13 08:01:43.694651 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1525-examples.txt
+-rw-r--r--   0        0        0    12791 2023-04-13 08:01:43.695062 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1525.ttl
+-rw-r--r--   0        0        0      573 2023-04-13 08:01:43.695372 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1559.ttl
+-rw-r--r--   0        0        0      640 2023-04-13 08:01:43.695603 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1576.ttl
+-rw-r--r--   0        0        0     1423 2023-04-13 08:01:43.695790 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1589.ttl
+-rw-r--r--   0        0        0      596 2023-04-13 08:01:43.695959 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1591.ttl
+-rw-r--r--   0        0        0      695 2023-04-13 08:01:43.696148 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1624.ttl
+-rw-r--r--   0        0        0      365 2023-04-13 08:01:43.696448 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1670-examples.txt
+-rw-r--r--   0        0        0      809 2023-04-13 08:01:43.696669 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1672.ttl
+-rw-r--r--   0        0        0     3007 2023-04-13 08:01:43.696829 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1688.ttl
+-rw-r--r--   0        0        0      989 2023-04-13 08:01:43.696998 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1689-examples.txt
+-rw-r--r--   0        0        0     2997 2023-04-13 08:01:43.697191 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1698-examples.txt
+-rw-r--r--   0        0        0     1121 2023-04-13 08:01:43.697411 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1741-examples.txt
+-rw-r--r--   0        0        0     1915 2023-04-13 08:01:43.697665 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1755.ttl
+-rw-r--r--   0        0        0    15775 2023-04-13 08:01:43.697880 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1758-examples.txt
+-rw-r--r--   0        0        0     2263 2023-04-13 08:01:43.698153 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1758.ttl
+-rw-r--r--   0        0        0     3023 2023-04-13 08:01:43.698337 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1759-examples.txt
+-rw-r--r--   0        0        0      967 2023-04-13 08:01:43.698497 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1759.ttl
+-rw-r--r--   0        0        0    10050 2023-04-13 08:01:43.698691 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1779-examples.txt
+-rw-r--r--   0        0        0     3567 2023-04-13 08:01:43.698861 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1779.ttl
+-rw-r--r--   0        0        0     4042 2023-04-13 08:01:43.699068 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1797.ttl
+-rw-r--r--   0        0        0    47424 2023-04-13 08:01:43.699403 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1810-examples.txt
+-rw-r--r--   0        0        0     4081 2023-04-13 08:01:43.699619 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1810.ttl
+-rw-r--r--   0        0        0      739 2023-04-13 08:01:43.699839 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1816.ttl
+-rw-r--r--   0        0        0     2113 2023-04-13 08:01:43.700021 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1828.ttl
+-rw-r--r--   0        0        0     3227 2023-04-13 08:01:43.700224 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1842-examples.txt
+-rw-r--r--   0        0        0     3574 2023-04-13 08:01:43.700425 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1842.ttl
+-rw-r--r--   0        0        0     1732 2023-04-13 08:01:43.700686 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1886.ttl
+-rw-r--r--   0        0        0      764 2023-04-13 08:01:43.700912 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1909.ttl
+-rw-r--r--   0        0        0     1039 2023-04-13 08:01:43.701111 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1950-examples.txt
+-rw-r--r--   0        0        0     1309 2023-04-13 08:01:43.701343 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1950.ttl
+-rw-r--r--   0        0        0      454 2023-04-13 08:01:43.701655 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1951.ttl
+-rw-r--r--   0        0        0      569 2023-04-13 08:01:43.701840 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1976.ttl
+-rw-r--r--   0        0        0      407 2023-04-13 08:01:43.702019 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2021-examples.txt
+-rw-r--r--   0        0        0      943 2023-04-13 08:01:43.702220 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2021.ttl
+-rw-r--r--   0        0        0      460 2023-04-13 08:01:43.702484 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2083-examples.txt
+-rw-r--r--   0        0        0      785 2023-04-13 08:01:43.702743 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2083.ttl
+-rw-r--r--   0        0        0      391 2023-04-13 08:01:43.702953 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2085-examples.txt
+-rw-r--r--   0        0        0      738 2023-04-13 08:01:43.703207 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2085.ttl
+-rw-r--r--   0        0        0      861 2023-04-13 08:01:43.703511 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2108-examples.txt
+-rw-r--r--   0        0        0     1723 2023-04-13 08:01:43.703783 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2108.ttl
+-rw-r--r--   0        0        0      288 2023-04-13 08:01:43.704062 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2109-examples.txt
+-rw-r--r--   0        0        0     1095 2023-04-13 08:01:43.704365 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2109.ttl
+-rw-r--r--   0        0        0      667 2023-04-13 08:01:43.704592 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2110.ttl
+-rw-r--r--   0        0        0      995 2023-04-13 08:01:43.704849 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2111.ttl
+-rw-r--r--   0        0        0      639 2023-04-13 08:01:43.705042 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2126.ttl
+-rw-r--r--   0        0        0     1114 2023-04-13 08:01:43.705222 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2140.ttl
+-rw-r--r--   0        0        0     1609 2023-04-13 08:01:43.705502 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2173-examples.txt
+-rw-r--r--   0        0        0      954 2023-04-13 08:01:43.705693 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2173.ttl
+-rw-r--r--   0        0        0     1627 2023-04-13 08:01:43.705888 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2192-examples.txt
+-rw-r--r--   0        0        0      588 2023-04-13 08:01:43.706061 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2192.ttl
+-rw-r--r--   0        0        0      623 2023-04-13 08:01:43.706234 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2242.ttl
+-rw-r--r--   0        0        0     1100 2023-04-13 08:01:43.706606 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2244.ttl
+-rw-r--r--   0        0        0     3793 2023-04-13 08:01:43.706807 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2288.ttl
+-rw-r--r--   0        0        0     3407 2023-04-13 08:01:43.706998 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2289-examples.txt
+-rw-r--r--   0        0        0     5154 2023-04-13 08:01:43.707271 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2289.ttl
+-rw-r--r--   0        0        0     5585 2023-04-13 08:01:43.707476 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2291.ttl
+-rw-r--r--   0        0        0      709 2023-04-13 08:01:43.707665 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2294-examples.txt
+-rw-r--r--   0        0        0      758 2023-04-13 08:01:43.707842 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2296-examples.txt
+-rw-r--r--   0        0        0      645 2023-04-13 08:01:43.708010 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2296.ttl
+-rw-r--r--   0        0        0      776 2023-04-13 08:01:43.708187 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2300.ttl
+-rw-r--r--   0        0        0     1403 2023-04-13 08:01:43.708510 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2311.ttl
+-rw-r--r--   0        0        0      664 2023-04-13 08:01:43.708822 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2329.ttl
+-rw-r--r--   0        0        0      455 2023-04-13 08:01:43.710376 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2341.ttl
+-rw-r--r--   0        0        0     1825 2023-04-13 08:01:43.710634 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2348.ttl
+-rw-r--r--   0        0        0      994 2023-04-13 08:01:43.710935 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2358.ttl
+-rw-r--r--   0        0        0     2528 2023-04-13 08:01:43.711136 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2366-examples.txt
+-rw-r--r--   0        0        0     8265 2023-04-13 08:01:43.711356 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2373.ttl
+-rw-r--r--   0        0        0    11319 2023-04-13 08:01:43.711576 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2374.ttl
+-rw-r--r--   0        0        0    15964 2023-04-13 08:01:43.711800 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2381.ttl
+-rw-r--r--   0        0        0      424 2023-04-13 08:01:43.712035 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2382.ttl
+-rw-r--r--   0        0        0     1022 2023-04-13 08:01:43.712206 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2384-examples.txt
+-rw-r--r--   0        0        0     2154 2023-04-13 08:01:43.712382 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2384.ttl
+-rw-r--r--   0        0        0      678 2023-04-13 08:01:43.712683 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2394.ttl
+-rw-r--r--   0        0        0     1684 2023-04-13 08:01:43.712888 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2396-examples.txt
+-rw-r--r--   0        0        0      963 2023-04-13 08:01:43.713106 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2396.ttl
+-rw-r--r--   0        0        0    12843 2023-04-13 08:01:43.713400 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2405-examples.txt
+-rw-r--r--   0        0        0     1669 2023-04-13 08:01:43.713635 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2405.ttl
+-rw-r--r--   0        0        0      684 2023-04-13 08:01:43.713895 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2418.ttl
+-rw-r--r--   0        0        0      659 2023-04-13 08:01:43.715639 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2419-examples.txt
+-rw-r--r--   0        0        0     4492 2023-04-13 08:01:43.715980 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2419.ttl
+-rw-r--r--   0        0        0      411 2023-04-13 08:01:43.716348 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2420.ttl
+-rw-r--r--   0        0        0     1308 2023-04-13 08:01:43.716552 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2421-examples.txt
+-rw-r--r--   0        0        0      457 2023-04-13 08:01:43.716720 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2421.ttl
+-rw-r--r--   0        0        0     1094 2023-04-13 08:01:43.716918 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2427.ttl
+-rw-r--r--   0        0        0     1588 2023-04-13 08:01:43.717143 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2450-examples.txt
+-rw-r--r--   0        0        0    18209 2023-04-13 08:01:43.717439 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2450.ttl
+-rw-r--r--   0        0        0     1796 2023-04-13 08:01:43.717732 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2454.ttl
+-rw-r--r--   0        0        0     1137 2023-04-13 08:01:43.717989 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2460.ttl
+-rw-r--r--   0        0        0     2129 2023-04-13 08:01:43.718278 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2469.ttl
+-rw-r--r--   0        0        0     3065 2023-04-13 08:01:43.718471 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2482-examples.txt
+-rw-r--r--   0        0        0      818 2023-04-13 08:01:43.718718 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2483.ttl
+-rw-r--r--   0        0        0      511 2023-04-13 08:01:43.718940 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2486.ttl
+-rw-r--r--   0        0        0     3602 2023-04-13 08:01:43.719234 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2490-examples.txt
+-rw-r--r--   0        0        0     9453 2023-04-13 08:01:43.719554 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2490.ttl
+-rw-r--r--   0        0        0      511 2023-04-13 08:01:43.719765 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2493.ttl
+-rw-r--r--   0        0        0      428 2023-04-13 08:01:43.719950 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2496.ttl
+-rw-r--r--   0        0        0      577 2023-04-13 08:01:43.720159 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2500.ttl
+-rw-r--r--   0        0        0    12915 2023-04-13 08:01:43.720510 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2506.ttl
+-rw-r--r--   0        0        0     1342 2023-04-13 08:01:43.720779 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2514-examples.txt
+-rw-r--r--   0        0        0      894 2023-04-13 08:01:43.721032 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2514.ttl
+-rw-r--r--   0        0        0     7821 2023-04-13 08:01:43.721247 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2521.ttl
+-rw-r--r--   0        0        0      537 2023-04-13 08:01:43.721497 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2526.ttl
+-rw-r--r--   0        0        0     1361 2023-04-13 08:01:43.721748 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2534-examples.txt
+-rw-r--r--   0        0        0     3814 2023-04-13 08:01:43.721968 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2534.ttl
+-rw-r--r--   0        0        0      713 2023-04-13 08:01:43.722176 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2543-examples.txt
+-rw-r--r--   0        0        0    14775 2023-04-13 08:01:43.722438 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2543.ttl
+-rw-r--r--   0        0        0      672 2023-04-13 08:01:43.722646 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2599-examples.txt
+-rw-r--r--   0        0        0      754 2023-04-13 08:01:43.722838 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2599.ttl
+-rw-r--r--   0        0        0      681 2023-04-13 08:01:43.723019 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2605.ttl
+-rw-r--r--   0        0        0      525 2023-04-13 08:01:43.723212 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2611.ttl
+-rw-r--r--   0        0        0      731 2023-04-13 08:01:43.723417 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2636.ttl
+-rw-r--r--   0        0        0      604 2023-04-13 08:01:43.723643 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2646.ttl
+-rw-r--r--   0        0        0     1036 2023-04-13 08:01:43.723855 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2659.ttl
+-rw-r--r--   0        0        0      695 2023-04-13 08:01:43.724045 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2665.ttl
+-rw-r--r--   0        0        0     7939 2023-04-13 08:01:43.724275 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2670.ttl
+-rw-r--r--   0        0        0      711 2023-04-13 08:01:43.724485 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2681-examples.txt
+-rw-r--r--   0        0        0     1569 2023-04-13 08:01:43.724681 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2681.ttl
+-rw-r--r--   0        0        0     4149 2023-04-13 08:01:43.724871 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2689.ttl
+-rw-r--r--   0        0        0      862 2023-04-13 08:01:43.725038 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-271-examples.txt
+-rw-r--r--   0        0        0     1200 2023-04-13 08:01:43.725215 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-271.ttl
+-rw-r--r--   0        0        0     2401 2023-04-13 08:01:43.725409 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2712.ttl
+-rw-r--r--   0        0        0      582 2023-04-13 08:01:43.725586 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2722-example.txt
+-rw-r--r--   0        0        0      684 2023-04-13 08:01:43.726650 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2722.ttl
+-rw-r--r--   0        0        0      912 2023-04-13 08:01:43.726975 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2740-examples.txt
+-rw-r--r--   0        0        0     1423 2023-04-13 08:01:43.727256 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2740.ttl
+-rw-r--r--   0        0        0      579 2023-04-13 08:01:43.727478 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-276.ttl
+-rw-r--r--   0        0        0     3012 2023-04-13 08:01:43.727654 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2766.ttl
+-rw-r--r--   0        0        0     2577 2023-04-13 08:01:43.727873 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2811-examples.txt
+-rw-r--r--   0        0        0    23965 2023-04-13 08:01:43.728115 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2811.ttl
+-rw-r--r--   0        0        0     1024 2023-04-13 08:01:43.728463 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2832-examples.txt
+-rw-r--r--   0        0        0     2101 2023-04-13 08:01:43.728696 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2832.ttl
+-rw-r--r--   0        0        0      837 2023-04-13 08:01:43.729150 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2862-examples.txt
+-rw-r--r--   0        0        0    17229 2023-04-13 08:01:43.729470 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2862.ttl
+-rw-r--r--   0        0        0      669 2023-04-13 08:01:43.729915 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2877.ttl
+-rw-r--r--   0        0        0      966 2023-04-13 08:01:43.730180 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2907.ttl
+-rw-r--r--   0        0        0      784 2023-04-13 08:01:43.730446 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2912.ttl
+-rw-r--r--   0        0        0      845 2023-04-13 08:01:43.730691 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2915.ttl
+-rw-r--r--   0        0        0      712 2023-04-13 08:01:43.730893 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2927.ttl
+-rw-r--r--   0        0        0     4844 2023-04-13 08:01:43.731088 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2989.ttl
+-rw-r--r--   0        0        0      677 2023-04-13 08:01:43.731258 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-3001.ttl
+-rw-r--r--   0        0        0     1006 2023-04-13 08:01:43.731436 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-3028-examples.txt
+-rw-r--r--   0        0        0     1007 2023-04-13 08:01:43.731643 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-3028.ttl
+-rw-r--r--   0        0        0      556 2023-04-13 08:01:43.731834 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-3052.ttl
+-rw-r--r--   0        0        0     2446 2023-04-13 08:01:43.732030 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-3057.ttl
+-rw-r--r--   0        0        0     1925 2023-04-13 08:01:43.732295 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-3058.ttl
+-rw-r--r--   0        0        0     1177 2023-04-13 08:01:43.732510 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-3123.ttl
+-rw-r--r--   0        0        0     1530 2023-04-13 08:01:43.732693 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-3134.ttl
+-rw-r--r--   0        0        0      876 2023-04-13 08:01:43.732864 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-3135-examples.txt
+-rw-r--r--   0        0        0      794 2023-04-13 08:01:43.733142 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-3135.ttl
+-rw-r--r--   0        0        0     5409 2023-04-13 08:01:43.733340 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-373-examples.txt
+-rw-r--r--   0        0        0     1661 2023-04-13 08:01:43.733577 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-373.ttl
+-rw-r--r--   0        0        0     5952 2023-04-13 08:01:43.733795 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-383-examples.txt
+-rw-r--r--   0        0        0     5541 2023-04-13 08:01:43.734020 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-383.ttl
+-rw-r--r--   0        0        0     1616 2023-04-13 08:01:43.734206 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-447-examples.txt
+-rw-r--r--   0        0        0     1625 2023-04-13 08:01:43.734367 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-447.ttl
+-rw-r--r--   0        0        0    10722 2023-04-13 08:01:43.734567 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-894-examples.txt
+-rw-r--r--   0        0        0     3867 2023-04-13 08:01:43.734858 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-894.ttl
+-rw-r--r--   0        0        0      768 2023-04-13 08:01:43.735085 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-987.ttl
+-rw-r--r--   0        0        0     1065 2023-04-13 08:01:43.735300 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-991.ttl
+-rw-r--r--   0        0        0      251 2023-04-13 08:01:43.735503 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-template-examples.txt
+-rw-r--r--   0        0        0      141 2023-04-13 08:01:43.735672 schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/pending-header.jsonld
+-rw-r--r--   0        0        0   410358 2023-04-13 08:01:43.737975 schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/httpequivs.ttl
+-rw-r--r--   0        0        0  2962722 2023-04-13 08:01:43.752851 schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schema-all.html
+-rw-r--r--   0        0        0  1015192 2023-04-13 08:01:43.761478 schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-all-examples.txt
+-rw-r--r--   0        0        0   461447 2023-04-13 08:01:43.765263 schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-all-http-properties.csv
+-rw-r--r--   0        0        0  2176246 2023-04-13 08:01:43.779595 schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-all-http-types.csv
+-rw-r--r--   0        0        0  1400370 2023-04-13 08:01:43.789260 schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-all-http.jsonld
+-rw-r--r--   0        0        0  2502842 2023-04-13 08:01:43.798935 schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-all-http.nq
+-rw-r--r--   0        0        0  2094592 2023-04-13 08:01:43.806733 schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-all-http.nt
+-rw-r--r--   0        0        0  1388115 2023-04-13 08:01:43.815039 schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-all-http.rdf
+-rw-r--r--   0        0        0  1000440 2023-04-13 08:01:43.820580 schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-all-http.ttl
+-rw-r--r--   0        0        0   467969 2023-04-13 08:01:43.821812 schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-all-https-properties.csv
+-rw-r--r--   0        0        0  2237356 2023-04-13 08:01:43.830981 schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-all-https-types.csv
+-rw-r--r--   0        0        0  1401553 2023-04-13 08:01:43.833298 schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-all-https.jsonld
+-rw-r--r--   0        0        0  2549224 2023-04-13 08:01:43.838886 schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-all-https.nq
+-rw-r--r--   0        0        0  2124644 2023-04-13 08:01:43.845950 schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-all-https.nt
+-rw-r--r--   0        0        0  1397406 2023-04-13 08:01:43.851802 schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-all-https.rdf
+-rw-r--r--   0        0        0  1001623 2023-04-13 08:01:43.853503 schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-all-https.ttl
+-rw-r--r--   0        0        0   459750 2023-04-13 08:01:43.854914 schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-current-http-properties.csv
+-rw-r--r--   0        0        0  2173210 2023-04-13 08:01:43.861402 schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-current-http-types.csv
+-rw-r--r--   0        0        0  1393407 2023-04-13 08:01:43.868361 schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-current-http.jsonld
+-rw-r--r--   0        0        0  2490302 2023-04-13 08:01:43.875993 schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-current-http.nq
+-rw-r--r--   0        0        0  2084102 2023-04-13 08:01:43.882530 schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-current-http.nt
+-rw-r--r--   0        0        0  1381444 2023-04-13 08:01:43.885799 schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-current-http.rdf
+-rw-r--r--   0        0        0   995515 2023-04-13 08:01:43.888969 schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-current-http.ttl
+-rw-r--r--   0        0        0   466246 2023-04-13 08:01:43.890385 schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-current-https-properties.csv
+-rw-r--r--   0        0        0  2234262 2023-04-13 08:01:43.897684 schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-current-https-types.csv
+-rw-r--r--   0        0        0  1394578 2023-04-13 08:01:43.899929 schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-current-https.jsonld
+-rw-r--r--   0        0        0  2536436 2023-04-13 08:01:43.903668 schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-current-https.nq
+-rw-r--r--   0        0        0  2113988 2023-04-13 08:01:43.911036 schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-current-https.nt
+-rw-r--r--   0        0        0  1390690 2023-04-13 08:01:43.913298 schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-current-https.rdf
+-rw-r--r--   0        0        0   996686 2023-04-13 08:01:43.914998 schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-current-https.ttl
+-rw-r--r--   0        0        0   343608 2023-04-13 08:01:43.916598 schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-shapes.shacl
+-rw-r--r--   0        0        0   946637 2023-04-13 08:01:43.920801 schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-shapes.shexj
+-rw-r--r--   0        0        0    58391 2023-04-13 08:01:43.921508 schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-subclasses.shacl
+-rw-r--r--   0        0        0  1901171 2023-04-13 08:01:43.927780 schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg.owl
+-rw-r--r--   0        0        0   172009 2023-04-13 08:01:43.928961 schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorgcontext.jsonld
+-rw-r--r--   0        0        0     9242 2023-04-16 15:33:33.391118 schemaorg_lite-0.1.1/schemaorg_lite/main.py
+-rw-r--r--   0        0        0     1619 1970-01-01 00:00:00.000000 schemaorg_lite-0.1.1/PKG-INFO
```

### Comparing `schemaorg_lite-0.1.0/pyproject.toml` & `schemaorg_lite-0.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 [tool.pdm.dev-dependencies]
 dev = [
-    "ipython>=8.11.0",
     "pytest>=7.2.2",
+    "ruff>=0.0.261",
+    "isort>=5.12.0",
+    "mypy>=1.2.0",
+    "black>=23.3.0",
+    "deptry>=0.8.0",
+    "refurb>=1.15.0",
 ]
 
 [tool.ruff]
 line-length = 88
 target-version = "py311"
 
 [tool.ruff.isort]
 split-on-trailing-comma = true
 force-wrap-aliases = true
-combine-as-imports = true
+force-single-line = true
 force-sort-within-sections = true
 
 [tool.ruff.mccabe]
 max-complexity = 10
 
 [tool.ruff.pydocstyle]
 convention = "google"
@@ -30,23 +35,23 @@
 
 [tool.deptry]
 
 [tool.refurb]
 
 [project]
 name = "schemaorg-lite"
-version = "0.1.0"
+version = "0.1.1"
 description = "Python functions for applied use of schema.org"
 authors = [
     { name = "Vanessa Sochat", email = "vsoch@users.noreply.github.com" },
     { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
 ]
 dependencies = [
     "msgspec>=0.13.1",
-    "loguru>=0.6.0",
+    "loguru>=0.7.0",
 ]
 requires-python = ">=3.11"
 readme = "README.md"
 keywords = [
     "openschemas",
     "schema.org",
 ]
@@ -66,15 +71,15 @@
 
 [project.license]
 text = "BSD-3-Clause"
 
 [project.urls]
 Homepage = "https://github.com/lesleslie/schemaorg-lite"
 Documentation = "https://github.com/lesleslie/schemaorg-lite"
-Repository = "https://github.com/lesleslie/crackerjack"
+Repository = "https://github.com/lesleslie/schemaorg-lite"
 
 [project.scripts]
 
 [project.entry-points]
 
 [build-system]
 requires = [
```

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/__init__.py` & `schemaorg_lite-0.1.1/schemaorg_lite/data/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import csv
 from pathlib import Path
 
-from schemaorg.main import logger
+from schemaorg_lite.main import logger
 
 
 def get_installdir():
     """get_installdir returns the installation directory of the application"""
     return Path(__file__).parent.parent.parent
 
 
@@ -55,76 +55,76 @@
     versions = (base / "releases").iterdir()
     versions = [float(x.name) for x in versions]
     versions.sort()
     return [str(x) for x in versions]
 
 
 def get_schemaorg_version():
-    """determine the schemaorg version to use based on an environmental variable
+    """determine the schemaorg_lite version to use based on an environmental variable
     first followed by  using the latest.
     """
     version = get_versions()[-1]
 
-    logger.debug("schemaorg version %s selected" % version)
+    logger.debug("schemaorg_lite version %s selected" % version)
     return version
 
 
 def get_release(version=None):
     """get a subfolder for a particular release, defaults to latest"""
     base = get_database()
     if version is None:
         version = get_schemaorg_version()
     return base / "releases" / version
 
 
 def get_database():
     """get the data folder with "release" and "ext" subfolders"""
-    return get_installdir() / "schemaorg" / "data"
+    return get_installdir() / "schemaorg_lite" / "data"
 
 
 # courtesy functions for schema.org exports
 
 """ List of available csv --------------------------------------
 all-layers-properties.csv  ext-health-lifesci-properties.csv
 all-layers-types.csv       ext-health-lifesci-types.csv
 ext-attic-properties.csv   ext-meta-properties.csv
 ext-attic-types.csv        ext-meta-types.csv
 ext-auto-properties.csv    ext-pending-properties.csv
 ext-auto-types.csv         ext-pending-types.csv
-ext-bib-properties.csv     schemaorg-all-https-properties.csv
-ext-bib-types.csv          schemaorg-all-http-types.csv
+ext-bib-properties.csv     schemaorg_lite-all-https-properties.csv
+ext-bib-types.csv          schemaorg_lite-all-http-types.csv
 """
 
 
 def read_properties_csv(keyfield="id", version=None):
     """read in the properties csv (with all types), defaulting to using
     the "id" as the lookup key. We do this because the properties listed
     in the types csv include the full uri.
 
     Parameters
     ==========
     keyfield: the key to use to generate the lookup, a header in the csv
     version: release version under data/releases to use, defaults to latest
     """
     release_dir = get_release(version=version)
-    filename = release_dir / "schemaorg-all-https-properties.csv"
+    filename = release_dir / "schemaorg_lite-all-https-properties.csv"
     return read_csv(filename, keyfield=keyfield)
 
 
 def read_types_csv(keyfield="label", version=None):
     """read in the types csv, with default lookup key as "label" since the
     likely use case will be the user searching for an item of interest.
 
     Parameters
     ==========
     keyfield: the key to use to generate the lookup, a header in the csv
     version: release version under data/releases to use, defaults to latest
     """
     release_dir = get_release(version=version)
-    filename = release_dir / "schemaorg-all-https-types.csv"
+    filename = release_dir / "schemaorg_lite-all-https-types.csv"
     return read_csv(filename, keyfield=keyfield)
 
 
 def find_similar_types(term, version=None):
     """find similar types, with intent to show to the user in case
     capitalization was off.
```

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/attic/attic.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/attic/attic.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/auto/auto.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/auto/auto.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/bib/bsdo-1.0.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/bib/bsdo-1.0.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/bib/bsdo-atlas-examples.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/bib/bsdo-atlas-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/bib/bsdo-audiobook-examples.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/bib/bsdo-audiobook-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/bib/bsdo-chapter-examples.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/bib/bsdo-chapter-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/bib/bsdo-collection-examples.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/bib/bsdo-collection-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/bib/bsdo-newspaper-examples.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/bib/bsdo-newspaper-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/bib/bsdo-thesis-examples.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/bib/bsdo-thesis-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/bib/bsdo-translation-examples.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/bib/bsdo-translation-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/bib/comics-examples.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/bib/comics-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/health-lifesci/MedicalScholarlyArticle-examples.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/health-lifesci/MedicalScholarlyArticle-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/health-lifesci/drug-example.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/health-lifesci/drug-example.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/health-lifesci/med-health-core.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/health-lifesci/med-health-core.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/health-lifesci/medicalCondition-examples.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/health-lifesci/medicalCondition-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/health-lifesci/medicalGuideline-examples.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/health-lifesci/medicalGuideline-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/health-lifesci/medicalWebpage-examples.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/health-lifesci/medicalWebpage-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/health-lifesci/physical-activity-and-exercise.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/health-lifesci/physical-activity-and-exercise.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/meta/meta.jsonld.someday.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/meta/meta.jsonld.someday.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/meta/meta.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/meta/meta.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1045-examples.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1045-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1045.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1045.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1050-examples.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1050-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1050.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1050.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1062-examples.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1062-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1062.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1062.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1083.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1083.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1156-examples.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1156-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1156.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1156.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1244.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1244.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1253-examples.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1253-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1253.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1253.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1375.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1375.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1389-examples.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1389-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1397.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1397.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1401.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1401.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1423-examples.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1423-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1423.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1423.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1425.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1425.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1448.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1448.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1457-examples.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1457-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1457.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1457.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1495.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1495.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1525-examples.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1525-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1525.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1525.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1559.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1559.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1576.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1576.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1589.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1589.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1591.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1591.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1624.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1624.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1672.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1672.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1688.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1688.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1689-examples.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1689-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1698-examples.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1698-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1741-examples.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1741-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1755.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1755.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1758-examples.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1758-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1758.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1758.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1759-examples.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1759-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1759.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1759.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1779-examples.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1779-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1779.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1779.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1797.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1797.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1810-examples.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1810-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1810.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1810.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1816.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1816.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1828.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1828.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1842-examples.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1842-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1842.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1842.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1886.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1886.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1909.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1909.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1950-examples.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1950-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1950.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1950.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-1976.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-1976.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2021.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2021.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2083.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2083.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2085.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2085.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2108-examples.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2108-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2108.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2108.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2109.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2109.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2110.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2110.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2111.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2111.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2126.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2126.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2140.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2140.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2173-examples.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2173-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2173.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2173.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2192-examples.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2192-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2192.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2192.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2242.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2242.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2244.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2244.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2288.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2288.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2289-examples.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2289-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2289.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2289.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2291.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2291.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2294-examples.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2294-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2296-examples.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2296-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2296.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2296.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2300.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2300.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2311.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2311.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2329.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2329.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2348.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2348.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2358.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2358.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2366-examples.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2366-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2373.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2373.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2374.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2374.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2381.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2381.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2384-examples.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2384-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2384.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2384.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2394.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2394.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2396-examples.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2396-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2396.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2396.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2405-examples.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2405-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2405.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2405.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2418.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2418.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2419-examples.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2419-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2419.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2419.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2421-examples.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2421-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2427.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2427.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2450-examples.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2450-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2450.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2450.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2454.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2454.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2460.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2460.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2469.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2469.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2482-examples.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2482-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2483.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2483.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2490-examples.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2490-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2490.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2490.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2500.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2500.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2506.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2506.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2514-examples.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2514-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2514.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2514.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2521.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2521.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2526.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2526.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2534-examples.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2534-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2534.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2534.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2543-examples.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2543-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2543.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2543.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2599-examples.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2599-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2599.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2599.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2605.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2605.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2611.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2611.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2636.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2636.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2646.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2646.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2659.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2659.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2665.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2665.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2670.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2670.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2681-examples.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2681-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2681.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2681.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2689.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2689.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-271-examples.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-271-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-271.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-271.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2712.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2712.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2722-example.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2722-example.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2722.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2722.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2740-examples.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2740-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2740.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2740.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-276.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-276.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2766.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2766.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2811-examples.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2811-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2811.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2811.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2832-examples.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2832-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2832.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2832.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2862-examples.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2862-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2862.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2862.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2877.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2877.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2907.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2907.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2912.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2912.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2915.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2915.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2927.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2927.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-2989.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-2989.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-3001.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-3001.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-3028-examples.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-3028-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-3028.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-3028.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-3052.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-3052.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-3057.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-3057.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-3058.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-3058.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-3123.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-3123.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-3134.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-3134.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-3135-examples.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-3135-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-3135.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-3135.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-373-examples.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-373-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-373.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-373.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-383-examples.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-383-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-383.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-383.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-447-examples.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-447-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-447.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-447.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-894-examples.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-894-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-894.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-894.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-987.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-987.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/ext/pending/issue-991.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/ext/pending/issue-991.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/httpequivs.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/httpequivs.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schema-all.html` & `schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schema-all.html`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-all-examples.txt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-all-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-all-http-properties.csv` & `schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-all-http-properties.csv`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-all-http-types.csv` & `schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-all-http-types.csv`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-all-http.jsonld` & `schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-all-http.jsonld`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-all-http.nq` & `schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-all-http.nq`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-all-http.nt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-all-http.nt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-all-http.rdf` & `schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-all-http.rdf`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-all-http.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-all-http.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-all-https-properties.csv` & `schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-all-https-properties.csv`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-all-https-types.csv` & `schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-all-https-types.csv`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-all-https.jsonld` & `schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-all-https.jsonld`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-all-https.nq` & `schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-all-https.nq`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-all-https.nt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-all-https.nt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-all-https.rdf` & `schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-all-https.rdf`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-all-https.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-all-https.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-current-http-properties.csv` & `schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-current-http-properties.csv`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-current-http-types.csv` & `schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-current-http-types.csv`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-current-http.jsonld` & `schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-current-http.jsonld`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-current-http.nq` & `schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-current-http.nq`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-current-http.nt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-current-http.nt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-current-http.rdf` & `schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-current-http.rdf`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-current-http.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-current-http.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-current-https-properties.csv` & `schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-current-https-properties.csv`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-current-https-types.csv` & `schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-current-https-types.csv`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-current-https.jsonld` & `schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-current-https.jsonld`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-current-https.nq` & `schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-current-https.nq`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-current-https.nt` & `schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-current-https.nt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-current-https.rdf` & `schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-current-https.rdf`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-current-https.ttl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-current-https.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-shapes.shacl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-shapes.shacl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-shapes.shexj` & `schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-shapes.shexj`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg-subclasses.shacl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg-subclasses.shacl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorg.owl` & `schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorg.owl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/data/releases/15.0/schemaorgcontext.jsonld` & `schemaorg_lite-0.1.1/schemaorg_lite/data/releases/15.0/schemaorgcontext.jsonld`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.0/schemaorg/main.py` & `schemaorg_lite-0.1.1/schemaorg_lite/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import re
 from contextlib import suppress
 
 from loguru import logger
-from schemaorg.data import find_similar_types
-from schemaorg.data import get_versions
-from schemaorg.data import read_properties_csv
-from schemaorg.data import read_types_csv
+from schemaorg_lite.data import find_similar_types
+from schemaorg_lite.data import get_versions
+from schemaorg_lite.data import read_properties_csv
+from schemaorg_lite.data import read_types_csv
 
 
 class Schema(object):
     def __init__(self, schema_type, version=None, base=None):
         self.type = None
         self.properties = dict()
         self.loaded = dict()
@@ -61,17 +61,17 @@
         # If version is None, just use latest
         if version is None:
             version = available[-1]
 
         version = str(version)
 
         # Version not valid, default to use latest
-        if not version in available:
-            logger.warning(f"Version {version} is not found in the data folder.")
-            version = available[-1]
+        if version not in available:
+    logger.warning(f"Version {version} is not found in the data folder.")
+    version = available[-1]
 
         # logger.info(f"Using Version {version}")
         self.version = version
 
     # Properties
 
     def add_property(self, name, value):
@@ -80,15 +80,15 @@
         Parameters
         ==========
         name: the name of the property, made to lowercase
         value: the value to add
         """
         if value not in ["", None, [], ()]:
             if name in self._properties:
-                lookup = self._properties[name]
+                # self._properties[name]
                 self.properties[name] = value
                 logger.debug(f"{name} set to {value}")
 
     def remove_property(self, name):
         """remove a property, meaning the instance property > self.properties
 
         Parameters
```

