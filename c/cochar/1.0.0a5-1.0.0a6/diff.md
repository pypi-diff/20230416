# Comparing `tmp/cochar-1.0.0a5.tar.gz` & `tmp/cochar-1.0.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cochar-1.0.0a5.tar", last modified: Thu Jan  5 14:47:21 2023, max compression
+gzip compressed data, was "cochar-1.0.0a6.tar", last modified: Tue Jan 24 22:49:26 2023, max compression
```

## Comparing `cochar-1.0.0a5.tar` & `cochar-1.0.0a6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 walu      (1000) walu      (1000)        0 2023-01-05 14:47:21.059688 cochar-1.0.0a5/
--rw-rw-r--   0 walu      (1000) walu      (1000)    35149 2022-05-08 15:45:42.000000 cochar-1.0.0a5/LICENSE
--rw-rw-r--   0 walu      (1000) walu      (1000)       78 2022-05-08 15:45:42.000000 cochar-1.0.0a5/MANIFEST.in
--rw-rw-r--   0 walu      (1000) walu      (1000)     4815 2023-01-05 14:47:21.059688 cochar-1.0.0a5/PKG-INFO
--rw-rw-r--   0 walu      (1000) walu      (1000)     3352 2023-01-05 14:25:40.000000 cochar-1.0.0a5/README.md
-drwxrwxr-x   0 walu      (1000) walu      (1000)        0 2023-01-05 14:47:21.059688 cochar-1.0.0a5/cochar/
--rwxrwxr-x   0 walu      (1000) walu      (1000)     3545 2023-01-05 13:47:25.000000 cochar-1.0.0a5/cochar/__init__.py
--rw-rw-r--   0 walu      (1000) walu      (1000)     2631 2022-12-17 20:10:52.000000 cochar-1.0.0a5/cochar/__main__.py
--rw-rw-r--   0 walu      (1000) walu      (1000)    13755 2022-12-26 12:42:28.000000 cochar-1.0.0a5/cochar/character.py
--rw-rw-r--   0 walu      (1000) walu      (1000)    19941 2023-01-05 11:39:23.000000 cochar-1.0.0a5/cochar/cochar.py
-drwxrwxr-x   0 walu      (1000) walu      (1000)        0 2023-01-05 14:47:21.059688 cochar-1.0.0a5/cochar/data/
--rw-rw-r--   0 walu      (1000) walu      (1000)    12997 2022-12-17 20:10:52.000000 cochar-1.0.0a5/cochar/data/occupations.json
--rw-rw-r--   0 walu      (1000) walu      (1000)     8915 2022-11-23 19:59:52.000000 cochar-1.0.0a5/cochar/data/popPyramid.json
--rw-rw-r--   0 walu      (1000) walu      (1000)      313 2023-01-02 12:02:52.000000 cochar-1.0.0a5/cochar/data/settings.json
--rw-rw-r--   0 walu      (1000) walu      (1000)    11510 2023-01-05 13:47:25.000000 cochar-1.0.0a5/cochar/data/skills.json
--rw-rw-r--   0 walu      (1000) walu      (1000)     7085 2023-01-02 12:02:52.000000 cochar-1.0.0a5/cochar/error.py
--rw-rw-r--   0 walu      (1000) walu      (1000)     2712 2023-01-05 13:47:25.000000 cochar-1.0.0a5/cochar/interface.py
--rw-rw-r--   0 walu      (1000) walu      (1000)     5863 2023-01-05 11:39:56.000000 cochar-1.0.0a5/cochar/occup.py
--rw-rw-r--   0 walu      (1000) walu      (1000)    12061 2022-12-27 18:24:12.000000 cochar-1.0.0a5/cochar/skill.py
--rw-rw-r--   0 walu      (1000) walu      (1000)     2117 2023-01-02 12:02:52.000000 cochar-1.0.0a5/cochar/utils.py
-drwxrwxr-x   0 walu      (1000) walu      (1000)        0 2023-01-05 14:47:21.059688 cochar-1.0.0a5/cochar.egg-info/
--rw-rw-r--   0 walu      (1000) walu      (1000)     4815 2023-01-05 14:47:20.000000 cochar-1.0.0a5/cochar.egg-info/PKG-INFO
--rw-rw-r--   0 walu      (1000) walu      (1000)      486 2023-01-05 14:47:21.000000 cochar-1.0.0a5/cochar.egg-info/SOURCES.txt
--rw-rw-r--   0 walu      (1000) walu      (1000)        1 2023-01-05 14:47:20.000000 cochar-1.0.0a5/cochar.egg-info/dependency_links.txt
--rw-rw-r--   0 walu      (1000) walu      (1000)       49 2023-01-05 14:47:20.000000 cochar-1.0.0a5/cochar.egg-info/entry_points.txt
--rw-rw-r--   0 walu      (1000) walu      (1000)        6 2023-01-05 14:47:20.000000 cochar-1.0.0a5/cochar.egg-info/requires.txt
--rw-rw-r--   0 walu      (1000) walu      (1000)        7 2023-01-05 14:47:20.000000 cochar-1.0.0a5/cochar.egg-info/top_level.txt
--rw-rw-r--   0 walu      (1000) walu      (1000)       38 2023-01-05 14:47:21.059688 cochar-1.0.0a5/setup.cfg
--rw-rw-r--   0 walu      (1000) walu      (1000)     1297 2023-01-05 14:11:48.000000 cochar-1.0.0a5/setup.py
+drwxrwxr-x   0 walu      (1000) walu      (1000)        0 2023-01-24 22:49:26.107073 cochar-1.0.0a6/
+-rw-rw-r--   0 walu      (1000) walu      (1000)    34523 2023-01-15 16:11:00.000000 cochar-1.0.0a6/LICENSE
+-rw-rw-r--   0 walu      (1000) walu      (1000)       78 2022-05-08 15:45:42.000000 cochar-1.0.0a6/MANIFEST.in
+-rw-rw-r--   0 walu      (1000) walu      (1000)     5766 2023-01-24 22:49:26.107073 cochar-1.0.0a6/PKG-INFO
+-rw-rw-r--   0 walu      (1000) walu      (1000)     4108 2023-01-15 16:11:00.000000 cochar-1.0.0a6/README.md
+drwxrwxr-x   0 walu      (1000) walu      (1000)        0 2023-01-24 22:49:26.107073 cochar-1.0.0a6/cochar/
+-rwxrwxr-x   0 walu      (1000) walu      (1000)     4295 2023-01-24 22:49:23.000000 cochar-1.0.0a6/cochar/__init__.py
+-rw-rw-r--   0 walu      (1000) walu      (1000)     3379 2023-01-15 16:11:00.000000 cochar-1.0.0a6/cochar/__main__.py
+-rw-rw-r--   0 walu      (1000) walu      (1000)    14517 2023-01-15 16:11:00.000000 cochar-1.0.0a6/cochar/character.py
+-rw-rw-r--   0 walu      (1000) walu      (1000)    20703 2023-01-15 16:11:00.000000 cochar-1.0.0a6/cochar/cochar.py
+drwxrwxr-x   0 walu      (1000) walu      (1000)        0 2023-01-24 22:49:26.107073 cochar-1.0.0a6/cochar/data/
+-rw-rw-r--   0 walu      (1000) walu      (1000)    13643 2023-01-15 12:08:56.000000 cochar-1.0.0a6/cochar/data/occupations.json
+-rw-rw-r--   0 walu      (1000) walu      (1000)     8915 2022-11-23 19:59:52.000000 cochar-1.0.0a6/cochar/data/popPyramid.json
+-rw-rw-r--   0 walu      (1000) walu      (1000)      313 2023-01-02 12:02:52.000000 cochar-1.0.0a6/cochar/data/settings.json
+-rw-rw-r--   0 walu      (1000) walu      (1000)    11510 2023-01-05 13:47:25.000000 cochar-1.0.0a6/cochar/data/skills.json
+-rw-rw-r--   0 walu      (1000) walu      (1000)     7845 2023-01-15 16:11:00.000000 cochar-1.0.0a6/cochar/error.py
+-rw-rw-r--   0 walu      (1000) walu      (1000)     3474 2023-01-15 16:11:00.000000 cochar-1.0.0a6/cochar/interface.py
+-rw-rw-r--   0 walu      (1000) walu      (1000)     6625 2023-01-15 16:11:00.000000 cochar-1.0.0a6/cochar/occup.py
+-rw-rw-r--   0 walu      (1000) walu      (1000)    12823 2023-01-15 16:11:00.000000 cochar-1.0.0a6/cochar/skill.py
+-rw-rw-r--   0 walu      (1000) walu      (1000)     2894 2023-01-15 16:11:00.000000 cochar-1.0.0a6/cochar/utils.py
+drwxrwxr-x   0 walu      (1000) walu      (1000)        0 2023-01-24 22:49:26.107073 cochar-1.0.0a6/cochar.egg-info/
+-rw-rw-r--   0 walu      (1000) walu      (1000)     5766 2023-01-24 22:49:26.000000 cochar-1.0.0a6/cochar.egg-info/PKG-INFO
+-rw-rw-r--   0 walu      (1000) walu      (1000)      486 2023-01-24 22:49:26.000000 cochar-1.0.0a6/cochar.egg-info/SOURCES.txt
+-rw-rw-r--   0 walu      (1000) walu      (1000)        1 2023-01-24 22:49:26.000000 cochar-1.0.0a6/cochar.egg-info/dependency_links.txt
+-rw-rw-r--   0 walu      (1000) walu      (1000)       49 2023-01-24 22:49:26.000000 cochar-1.0.0a6/cochar.egg-info/entry_points.txt
+-rw-rw-r--   0 walu      (1000) walu      (1000)        6 2023-01-24 22:49:26.000000 cochar-1.0.0a6/cochar.egg-info/requires.txt
+-rw-rw-r--   0 walu      (1000) walu      (1000)        7 2023-01-24 22:49:26.000000 cochar-1.0.0a6/cochar.egg-info/top_level.txt
+-rw-rw-r--   0 walu      (1000) walu      (1000)       38 2023-01-24 22:49:26.107073 cochar-1.0.0a6/setup.cfg
+-rw-rw-r--   0 walu      (1000) walu      (1000)     1889 2023-01-24 22:49:23.000000 cochar-1.0.0a6/setup.py
```

### Comparing `cochar-1.0.0a5/LICENSE` & `cochar-1.0.0a6/LICENSE`

 * *Files 6% similar despite different names*

```diff
@@ -1,82 +1,70 @@
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
+                    GNU AFFERO GENERAL PUBLIC LICENSE
+                       Version 3, 19 November 2007
 
  Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
  Everyone is permitted to copy and distribute verbatim copies
  of this license document, but changing it is not allowed.
 
                             Preamble
 
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
+  The GNU Affero General Public License is a free, copyleft license for
+software and other kinds of works, specifically designed to ensure
+cooperation with the community in the case of network server software.
 
   The licenses for most software and other practical works are designed
 to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
+our General Public Licenses are intended to guarantee your freedom to
 share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
+software for all its users.
 
   When we speak of free software, we are referring to freedom, not
 price.  Our General Public Licenses are designed to make sure that you
 have the freedom to distribute copies of free software (and charge for
 them if you wish), that you receive source code or can get it if you
 want it, that you can change the software or use pieces of it in new
 free programs, and that you know you can do these things.
 
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
+  Developers that use our General Public Licenses protect your rights
+with two steps: (1) assert copyright on the software, and (2) offer
+you this License which gives you legal permission to copy, distribute
+and/or modify the software.
+
+  A secondary benefit of defending all users' freedom is that
+improvements made in alternate versions of the program, if they
+receive widespread use, become available for other developers to
+incorporate.  Many developers of free software are heartened and
+encouraged by the resulting cooperation.  However, in the case of
+software used on network servers, this result may fail to come about.
+The GNU General Public License permits making a modified version and
+letting the public access it on a server without ever releasing its
+source code to the public.
+
+  The GNU Affero General Public License is designed specifically to
+ensure that, in such cases, the modified source code becomes available
+to the community.  It requires the operator of a network server to
+provide the source code of the modified version running there to the
+users of that server.  Therefore, public use of a modified version, on
+a publicly accessible server, gives the public access to the source
+code of the modified version.
+
+  An older license, called the Affero General Public License and
+published by Affero, was designed to accomplish similar goals.  This is
+a different license, not a version of the Affero GPL, but Affero has
+released a new version of the Affero GPL which permits relicensing under
+this license.
 
   The precise terms and conditions for copying, distribution and
 modification follow.
 
                        TERMS AND CONDITIONS
 
   0. Definitions.
 
-  "This License" refers to version 3 of the GNU General Public License.
+  "This License" refers to version 3 of the GNU Affero General Public License.
 
   "Copyright" also means copyright-like laws that apply to other kinds of
 works, such as semiconductor masks.
 
   "The Program" refers to any copyrightable work licensed under this
 License.  Each licensee is addressed as "you".  "Licensees" and
 "recipients" may be individuals or organizations.
@@ -545,43 +533,53 @@
 covered work so as to satisfy simultaneously your obligations under this
 License and any other pertinent obligations, then as a consequence you may
 not convey it at all.  For example, if you agree to terms that obligate you
 to collect a royalty for further conveying from those to whom you convey
 the Program, the only way you could satisfy both those terms and this
 License would be to refrain entirely from conveying the Program.
 
-  13. Use with the GNU Affero General Public License.
+  13. Remote Network Interaction; Use with the GNU General Public License.
+
+  Notwithstanding any other provision of this License, if you modify the
+Program, your modified version must prominently offer all users
+interacting with it remotely through a computer network (if your version
+supports such interaction) an opportunity to receive the Corresponding
+Source of your version by providing access to the Corresponding Source
+from a network server at no charge, through some standard or customary
+means of facilitating copying of software.  This Corresponding Source
+shall include the Corresponding Source for any work covered by version 3
+of the GNU General Public License that is incorporated pursuant to the
+following paragraph.
 
   Notwithstanding any other provision of this License, you have
 permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
+under version 3 of the GNU General Public License into a single
 combined work, and to convey the resulting work.  The terms of this
 License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
+but the work with which it is combined will remain governed by version
+3 of the GNU General Public License.
 
   14. Revised Versions of this License.
 
   The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
+the GNU Affero General Public License from time to time.  Such new versions
+will be similar in spirit to the present version, but may differ in detail to
 address new problems or concerns.
 
   Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
+Program specifies that a certain numbered version of the GNU Affero General
 Public License "or any later version" applies to it, you have the
 option of following the terms and conditions either of that numbered
 version or of any later version published by the Free Software
 Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
+GNU Affero General Public License, you may choose any version ever published
 by the Free Software Foundation.
 
   If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
+versions of the GNU Affero General Public License can be used, that proxy's
 public statement of acceptance of a version permanently authorizes you
 to choose that version for the Program.
 
   Later license versions may give you additional or different
 permissions.  However, no additional obligations are imposed on any
 author or copyright holder as a result of your choosing to follow a
 later version.
@@ -631,44 +629,33 @@
 state the exclusion of warranty; and each file should have at least
 the "copyright" line and a pointer to where the full notice is found.
 
     <one line to give the program's name and a brief idea of what it does.>
     Copyright (C) <year>  <name of author>
 
     This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
+    it under the terms of the GNU Affero General Public License as published by
     the Free Software Foundation, either version 3 of the License, or
     (at your option) any later version.
 
     This program is distributed in the hope that it will be useful,
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
+    GNU Affero General Public License for more details.
 
-    You should have received a copy of the GNU General Public License
+    You should have received a copy of the GNU Affero General Public License
     along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 Also add information on how to contact you by electronic and paper mail.
 
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
+  If your software can interact with users remotely through a computer
+network, you should also make sure that it provides a way for users to
+get its source.  For example, if your program is a web application, its
+interface could display a "Source" link that leads users to an archive
+of the code.  There are many ways you could offer source, and different
+solutions will be better for different programs; see section 13 for the
+specific requirements.
 
   You should also get your employer (if you work as a programmer) or school,
 if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
+For more information on this, and how to apply and follow the GNU AGPL, see
 <https://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
-<https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `cochar-1.0.0a5/PKG-INFO` & `cochar-1.0.0a6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,48 @@
 Metadata-Version: 2.1
 Name: cochar
-Version: 1.0.0a5
+Version: 1.0.0a6
 Summary: Call of Cthulhu character generator
 Home-page: https://github.com/ajwalkiewicz/cochar
 Author: Adam Walkiewicz
-License: GPL 3.0
+License: AGPL v3
 Project-URL: Documentation, https://ajwalkiewicz.github.io/cochar/_build/html/index.html
-Description: [![PyPI version](https://badge.fury.io/py/cochar.svg)](https://badge.fury.io/py/cochar)
-        [![License: GNU GPL v3](https://img.shields.io/badge/License-GNU%20GPL%20v3-red.svg)](https://github.com/ajwalkiewicz/cochar/blob/main/LICENSE)
+Description: <!--
+        Cochar - create a random character for Call of Cthulhu RPG 7th ed.
+        Copyright (C) 2023  Adam Walkiewicz
+        
+        This program is free software: you can redistribute it and/or modify
+        it under the terms of the GNU Affero General Public License as published
+        by the Free Software Foundation, either version 3 of the License, or
+        (at your option) any later version.
+        
+        This program is distributed in the hope that it will be useful,
+        but WITHOUT ANY WARRANTY; without even the implied warranty of
+        MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+        GNU Affero General Public License for more details.
+        
+        You should have received a copy of the GNU Affero General Public License
+        along with this program.  If not, see <https://www.gnu.org/licenses/>.
+        -->
+        
+        [![PyPI version](https://badge.fury.io/py/cochar.svg)](https://badge.fury.io/py/cochar)
+        [![License: GNU AGPL v3](https://img.shields.io/badge/License-GNU%20AGPL%20v3-red.svg)](https://github.com/ajwalkiewicz/cochar/blob/main/LICENSE)
         [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
         [![Language: Python](https://img.shields.io/badge/Language-Python-blue.svg)](https://shields.io/)
         [![Author: Walu](https://img.shields.io/badge/Aurhor-Walu-gray.svg)](https://shields.io/)
         
         # **C**all **O**f **C**thulhu C**har**acter Generator
         
         Fast way of creating a random character for Call of Cthulhu RPG 7th ed.
         
         ## Summary
         
         `cochar` stands for `Call of Cthulhu Character`. It's a python package design to create a full characters for Call of Cthulhu RPG 7th ed.
         
-        A sample power `cochar` package can be observed on [www.cochar.pl](www.cochar.pl)
+        [www.cochar.pl](http://www.cochar.pl) demonstrates a power of `cochar` package.
         
         ## Table of Contents
         
         - [Project Title](#call-of-cthulhu-character-generator)
         - [Summary](#summary)
         - [Table of Contents](#table-of-contents)
         - [Installation](#installation)
@@ -98,24 +116,25 @@
         
         If you want to contribute to `cochar` project read [contribution](https://github.com/ajwalkiewicz/cochar/blob/main/CONTRIBUTION.md) for more information.
         
         ## Web Version
         
         > Web application is not a part of `cochar` package.
         
-        Web application was design to present the power of `cochar` package. You can check it out on [www.cochar.pl](www.cochar.pl)
+        Web application was design to present the power of `cochar` package. You can check it out on [www.cochar.pl](http://www.cochar.pl)
         
         ## Author
         
         Adam Walkiewicz
         
         ## License
         
-        Cochar is licensed under the terms of the [GNU GPL v3](https://github.com/ajwalkiewicz/cochar/blob/main/LICENSE)
+        Cochar is licensed under the terms of the [GNU AGPL v3](https://github.com/ajwalkiewicz/cochar/blob/main/LICENSE)
         
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

### Comparing `cochar-1.0.0a5/README.md` & `cochar-1.0.0a6/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,40 @@
+<!--
+Cochar - create a random character for Call of Cthulhu RPG 7th ed.
+Copyright (C) 2023  Adam Walkiewicz
+
+This program is free software: you can redistribute it and/or modify
+it under the terms of the GNU Affero General Public License as published
+by the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+This program is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU Affero General Public License for more details.
+
+You should have received a copy of the GNU Affero General Public License
+along with this program.  If not, see <https://www.gnu.org/licenses/>.
+-->
+
 [![PyPI version](https://badge.fury.io/py/cochar.svg)](https://badge.fury.io/py/cochar)
-[![License: GNU GPL v3](https://img.shields.io/badge/License-GNU%20GPL%20v3-red.svg)](https://github.com/ajwalkiewicz/cochar/blob/main/LICENSE)
+[![License: GNU AGPL v3](https://img.shields.io/badge/License-GNU%20AGPL%20v3-red.svg)](https://github.com/ajwalkiewicz/cochar/blob/main/LICENSE)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Language: Python](https://img.shields.io/badge/Language-Python-blue.svg)](https://shields.io/)
 [![Author: Walu](https://img.shields.io/badge/Aurhor-Walu-gray.svg)](https://shields.io/)
 
 # **C**all **O**f **C**thulhu C**har**acter Generator
 
 Fast way of creating a random character for Call of Cthulhu RPG 7th ed.
 
 ## Summary
 
 `cochar` stands for `Call of Cthulhu Character`. It's a python package design to create a full characters for Call of Cthulhu RPG 7th ed.
 
-A sample power `cochar` package can be observed on [www.cochar.pl](www.cochar.pl)
+[www.cochar.pl](http://www.cochar.pl) demonstrates a power of `cochar` package.
 
 ## Table of Contents
 
 - [Project Title](#call-of-cthulhu-character-generator)
 - [Summary](#summary)
 - [Table of Contents](#table-of-contents)
 - [Installation](#installation)
@@ -90,16 +108,16 @@
 
 If you want to contribute to `cochar` project read [contribution](https://github.com/ajwalkiewicz/cochar/blob/main/CONTRIBUTION.md) for more information.
 
 ## Web Version
 
 > Web application is not a part of `cochar` package.
 
-Web application was design to present the power of `cochar` package. You can check it out on [www.cochar.pl](www.cochar.pl)
+Web application was design to present the power of `cochar` package. You can check it out on [www.cochar.pl](http://www.cochar.pl)
 
 ## Author
 
 Adam Walkiewicz
 
 ## License
 
-Cochar is licensed under the terms of the [GNU GPL v3](https://github.com/ajwalkiewicz/cochar/blob/main/LICENSE)
+Cochar is licensed under the terms of the [GNU AGPL v3](https://github.com/ajwalkiewicz/cochar/blob/main/LICENSE)
```

### Comparing `cochar-1.0.0a5/cochar/character.py` & `cochar-1.0.0a6/cochar/character.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+# Cochar - create a random character for Call of Cthulhu RPG 7th ed.
+# Copyright (C) 2023  Adam Walkiewicz
+
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU Affero General Public License as published
+# by the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU Affero General Public License for more details.
+
+# You should have received a copy of the GNU Affero General Public License
+# along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """"This module contains classes related with Character object itself."""
 
 from abc import ABC, abstractmethod
 from typing import List, Union
 
 import randname
```

### Comparing `cochar-1.0.0a5/cochar/cochar.py` & `cochar-1.0.0a6/cochar/cochar.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+# Cochar - create a random character for Call of Cthulhu RPG 7th ed.
+# Copyright (C) 2023  Adam Walkiewicz
+
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU Affero General Public License as published
+# by the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU Affero General Public License for more details.
+
+# You should have received a copy of the GNU Affero General Public License
+# along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """**Cochar - main module**"""
 import json
 import random
 from typing import List, Tuple, Union
 
 import randname
```

### Comparing `cochar-1.0.0a5/cochar/data/occupations.json` & `cochar-1.0.0a6/cochar/data/occupations.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9523809523809523%*

 * *Differences: {"'computer programmer/technician'": "OrderedDict([('type', 'expansion'), ('era', 'modern'), "*

 * *                                     "('tags', []), ('groups', ['edu']), ('credit_rating', [10, "*

 * *                                     "70]), ('skills', ['computer use', 'electrical repair', "*

 * *                                     "'electronics', 'library use', 'science (mathematics)', 'spot "*

 * *                                     "hidden', '2*'])])",*

 * * "'deprogrammer'": "OrderedDict([('type', 'expansion'), ('era', ' […]*

```diff
@@ -175,14 +175,35 @@
             "1i",
             "1l",
             "1*"
         ],
         "tags": [],
         "type": "classic"
     },
+    "computer programmer/technician": {
+        "credit_rating": [
+            10,
+            70
+        ],
+        "era": "modern",
+        "groups": [
+            "edu"
+        ],
+        "skills": [
+            "computer use",
+            "electrical repair",
+            "electronics",
+            "library use",
+            "science (mathematics)",
+            "spot hidden",
+            "2*"
+        ],
+        "tags": [],
+        "type": "expansion"
+    },
     "criminal": {
         "credit_rating": [
             5,
             65
         ],
         "era": "classic-1920",
         "groups": [
@@ -206,14 +227,39 @@
             "1i"
         ],
         "tags": [
             "criminal"
         ],
         "type": "classic"
     },
+    "deprogrammer": {
+        "credit_rating": [
+            20,
+            50
+        ],
+        "era": "modern",
+        "groups": [
+            "edu"
+        ],
+        "skills": [
+            "2i",
+            "drive auto",
+            [
+                1,
+                "fighting (brawl)",
+                "firearms"
+            ],
+            "history",
+            "occult",
+            "psychology",
+            "stealth"
+        ],
+        "tags": [],
+        "type": "expansion"
+    },
     "dilettante": {
         "credit_rating": [
             50,
             99
         ],
         "era": "classic-1920",
         "groups": [
```

### Comparing `cochar-1.0.0a5/cochar/data/popPyramid.json` & `cochar-1.0.0a6/cochar/data/popPyramid.json`

 * *Files identical despite different names*

### Comparing `cochar-1.0.0a5/cochar/data/skills.json` & `cochar-1.0.0a6/cochar/data/skills.json`

 * *Files identical despite different names*

### Comparing `cochar-1.0.0a5/cochar/error.py` & `cochar-1.0.0a6/cochar/error.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,23 @@
-"""
-**Errors for cochar module**
-"""
+# Cochar - create a random character for Call of Cthulhu RPG 7th ed.
+# Copyright (C) 2023  Adam Walkiewicz
+
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU Affero General Public License as published
+# by the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU Affero General Public License for more details.
+
+# You should have received a copy of the GNU Affero General Public License
+# along with this program.  If not, see <https://www.gnu.org/licenses/>.
+"""**Errors for cochar module**"""
 from typing import Any
 
 
 class CocharError(Exception):
     pass
```

### Comparing `cochar-1.0.0a5/cochar/interface.py` & `cochar-1.0.0a6/cochar/interface.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+# Cochar - create a random character for Call of Cthulhu RPG 7th ed.
+# Copyright (C) 2023  Adam Walkiewicz
+
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU Affero General Public License as published
+# by the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU Affero General Public License for more details.
+
+# You should have received a copy of the GNU Affero General Public License
+# along with this program.  If not, see <https://www.gnu.org/licenses/>.
 from abc import ABC, abstractmethod, abstractproperty
 from pathlib import Path
 from typing import List, Dict
 
 import os
 import json
 import itertools
```

### Comparing `cochar-1.0.0a5/cochar/occup.py` & `cochar-1.0.0a6/cochar/occup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+# Cochar - create a random character for Call of Cthulhu RPG 7th ed.
+# Copyright (C) 2023  Adam Walkiewicz
+
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU Affero General Public License as published
+# by the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU Affero General Public License for more details.
+
+# You should have received a copy of the GNU Affero General Public License
+# along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """**Occupations**
 Occupations is a module that contains functions related
 with occupations
 """
 import copy
 import random
 from itertools import compress
```

### Comparing `cochar-1.0.0a5/cochar/skill.py` & `cochar-1.0.0a6/cochar/skill.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+# Cochar - create a random character for Call of Cthulhu RPG 7th ed.
+# Copyright (C) 2023  Adam Walkiewicz
+
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU Affero General Public License as published
+# by the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU Affero General Public License for more details.
+
+# You should have received a copy of the GNU Affero General Public License
+# along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """**Skills**
 Skills module contains all functions related with skills
 and Skills object, which is a container for skills
 
 """
 import random
 from collections import UserDict
```

### Comparing `cochar-1.0.0a5/cochar.egg-info/PKG-INFO` & `cochar-1.0.0a6/cochar.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,48 @@
 Metadata-Version: 2.1
 Name: cochar
-Version: 1.0.0a5
+Version: 1.0.0a6
 Summary: Call of Cthulhu character generator
 Home-page: https://github.com/ajwalkiewicz/cochar
 Author: Adam Walkiewicz
-License: GPL 3.0
+License: AGPL v3
 Project-URL: Documentation, https://ajwalkiewicz.github.io/cochar/_build/html/index.html
-Description: [![PyPI version](https://badge.fury.io/py/cochar.svg)](https://badge.fury.io/py/cochar)
-        [![License: GNU GPL v3](https://img.shields.io/badge/License-GNU%20GPL%20v3-red.svg)](https://github.com/ajwalkiewicz/cochar/blob/main/LICENSE)
+Description: <!--
+        Cochar - create a random character for Call of Cthulhu RPG 7th ed.
+        Copyright (C) 2023  Adam Walkiewicz
+        
+        This program is free software: you can redistribute it and/or modify
+        it under the terms of the GNU Affero General Public License as published
+        by the Free Software Foundation, either version 3 of the License, or
+        (at your option) any later version.
+        
+        This program is distributed in the hope that it will be useful,
+        but WITHOUT ANY WARRANTY; without even the implied warranty of
+        MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+        GNU Affero General Public License for more details.
+        
+        You should have received a copy of the GNU Affero General Public License
+        along with this program.  If not, see <https://www.gnu.org/licenses/>.
+        -->
+        
+        [![PyPI version](https://badge.fury.io/py/cochar.svg)](https://badge.fury.io/py/cochar)
+        [![License: GNU AGPL v3](https://img.shields.io/badge/License-GNU%20AGPL%20v3-red.svg)](https://github.com/ajwalkiewicz/cochar/blob/main/LICENSE)
         [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
         [![Language: Python](https://img.shields.io/badge/Language-Python-blue.svg)](https://shields.io/)
         [![Author: Walu](https://img.shields.io/badge/Aurhor-Walu-gray.svg)](https://shields.io/)
         
         # **C**all **O**f **C**thulhu C**har**acter Generator
         
         Fast way of creating a random character for Call of Cthulhu RPG 7th ed.
         
         ## Summary
         
         `cochar` stands for `Call of Cthulhu Character`. It's a python package design to create a full characters for Call of Cthulhu RPG 7th ed.
         
-        A sample power `cochar` package can be observed on [www.cochar.pl](www.cochar.pl)
+        [www.cochar.pl](http://www.cochar.pl) demonstrates a power of `cochar` package.
         
         ## Table of Contents
         
         - [Project Title](#call-of-cthulhu-character-generator)
         - [Summary](#summary)
         - [Table of Contents](#table-of-contents)
         - [Installation](#installation)
@@ -98,24 +116,25 @@
         
         If you want to contribute to `cochar` project read [contribution](https://github.com/ajwalkiewicz/cochar/blob/main/CONTRIBUTION.md) for more information.
         
         ## Web Version
         
         > Web application is not a part of `cochar` package.
         
-        Web application was design to present the power of `cochar` package. You can check it out on [www.cochar.pl](www.cochar.pl)
+        Web application was design to present the power of `cochar` package. You can check it out on [www.cochar.pl](http://www.cochar.pl)
         
         ## Author
         
         Adam Walkiewicz
         
         ## License
         
-        Cochar is licensed under the terms of the [GNU GPL v3](https://github.com/ajwalkiewicz/cochar/blob/main/LICENSE)
+        Cochar is licensed under the terms of the [GNU AGPL v3](https://github.com/ajwalkiewicz/cochar/blob/main/LICENSE)
         
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

