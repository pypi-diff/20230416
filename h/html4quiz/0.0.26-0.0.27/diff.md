# Comparing `tmp/html4quiz-0.0.26.tar.gz` & `tmp/html4quiz-0.0.27.tar.gz`

## Comparing `html4quiz-0.0.26.tar` & `html4quiz-0.0.27.tar`

### file list

```diff
@@ -1,29 +1,10 @@
--rw-r--r--   0        0        0     3984 2020-02-02 00:00:00.000000 html4quiz-0.0.26/0.0.22README.md
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 html4quiz-0.0.26/0.0.22pyproject.toml
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 html4quiz-0.0.26/0.0.25pyproject.toml
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 html4quiz-0.0.26/updatePackage.txt
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 html4quiz-0.0.26/src/html4quiz/__init__.py
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 html4quiz-0.0.26/src/html4quiz/_common.py
--rw-r--r--   0        0        0    28066 2020-02-02 00:00:00.000000 html4quiz-0.0.26/src/html4quiz/_generateEm.py
--rw-r--r--   0        0        0    11135 2020-02-02 00:00:00.000000 html4quiz-0.0.26/src/html4quiz/_scoreEm.py
--rw-r--r--   0        0        0    14972 2020-02-02 00:00:00.000000 html4quiz-0.0.26/src/html4quiz/makeChoices.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 html4quiz-0.0.26/src - 0.0.21/html4quiz/__init__.py
--rw-r--r--   0        0        0     2789 2020-02-02 00:00:00.000000 html4quiz-0.0.26/src - 0.0.21/html4quiz/_common.py
--rw-r--r--   0        0        0    11158 2020-02-02 00:00:00.000000 html4quiz-0.0.26/src - 0.0.21/html4quiz/_generateEm.py
--rw-r--r--   0        0        0    17875 2020-02-02 00:00:00.000000 html4quiz-0.0.26/src - 0.0.21/html4quiz/_generateMakeHTMLs.py
--rw-r--r--   0        0        0    10486 2020-02-02 00:00:00.000000 html4quiz-0.0.26/src - 0.0.21/html4quiz/_scoreEm.py
--rw-r--r--   0        0        0    14972 2020-02-02 00:00:00.000000 html4quiz-0.0.26/src - 0.0.21/html4quiz/makeChoices.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 html4quiz-0.0.26/src - 0.0.22/html4quiz/__init__.py
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 html4quiz-0.0.26/src - 0.0.22/html4quiz/_common.py
--rw-r--r--   0        0        0    26651 2020-02-02 00:00:00.000000 html4quiz-0.0.26/src - 0.0.22/html4quiz/_generateEm.py
--rw-r--r--   0        0        0    11135 2020-02-02 00:00:00.000000 html4quiz-0.0.26/src - 0.0.22/html4quiz/_scoreEm.py
--rw-r--r--   0        0        0    14972 2020-02-02 00:00:00.000000 html4quiz-0.0.26/src - 0.0.22/html4quiz/makeChoices.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 html4quiz-0.0.26/src - 0.0.25/html4quiz/__init__.py
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 html4quiz-0.0.26/src - 0.0.25/html4quiz/_common.py
--rw-r--r--   0        0        0    26651 2020-02-02 00:00:00.000000 html4quiz-0.0.26/src - 0.0.25/html4quiz/_generateEm.py
--rw-r--r--   0        0        0    11135 2020-02-02 00:00:00.000000 html4quiz-0.0.26/src - 0.0.25/html4quiz/_scoreEm.py
--rw-r--r--   0        0        0    14972 2020-02-02 00:00:00.000000 html4quiz-0.0.26/src - 0.0.25/html4quiz/makeChoices.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 html4quiz-0.0.26/LICENSE.txt
--rw-r--r--   0        0        0     4724 2020-02-02 00:00:00.000000 html4quiz-0.0.26/README.md
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 html4quiz-0.0.26/pyproject.toml
--rw-r--r--   0        0        0     5508 2020-02-02 00:00:00.000000 html4quiz-0.0.26/PKG-INFO
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 html4quiz-0.0.27/updatePackage.txt
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 html4quiz-0.0.27/src/html4quiz/__init__.py
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 html4quiz-0.0.27/src/html4quiz/_common.py
+-rw-r--r--   0        0        0    28066 2020-02-02 00:00:00.000000 html4quiz-0.0.27/src/html4quiz/_generateEm.py
+-rw-r--r--   0        0        0    11135 2020-02-02 00:00:00.000000 html4quiz-0.0.27/src/html4quiz/_scoreEm.py
+-rw-r--r--   0        0        0    14972 2020-02-02 00:00:00.000000 html4quiz-0.0.27/src/html4quiz/makeChoices.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 html4quiz-0.0.27/LICENSE.txt
+-rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 html4quiz-0.0.27/README.md
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 html4quiz-0.0.27/pyproject.toml
+-rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 html4quiz-0.0.27/PKG-INFO
```

### Comparing `html4quiz-0.0.26/0.0.22README.md` & `html4quiz-0.0.27/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,67 +1,78 @@
 # html4quiz
 
 ## What is it?
 
-html4quiz is a package that generates question papers as HTML files to be distributed over the network and grades the answers in text files submitted by students.
-
-## Help
-<ul>
-<li><a href="https://github.com/generateNscore/html4quiz/wiki">Documentation</a></li>
-</ul>
+html4quiz is a package that helps you generate question sheets with as many HTML files as you want and grade answers from text files submitted by students.
 
 ## Features
 <ul>
-<li>Generates as many personalized question sheets in HTML files as one wants with a few strings of text.</li>
-<li>The amount of random personalization is under full control of users.</li>
-<li>Each HTML file with a name corresponding to the identification number.</li>
-<li>Multi-choice as well as short, default, questions can be made.</li>
-<li>A figure, although a pre-made image can be used, can be varied as well as questions.</li>
-<li>Mathematical equations can be included in questions with Latex.</li>
-<li>User defined functions can be easily added.</li>
-<li>With the question sheets in HTML files, students require only a web browser to answer and send text files including the answers over the network.</li>
-<li>Scoring all different answers in text files submitted can be done in a second.</li>
+<li>Everything is on your local PC, grows with your creativity, and you own them all.</li>
+<li>Question sheets in HTML files, each named with a corresponding identification number, are distributed to students over the network.</li>
+<li>Students use their mobile devices to read, answer questions, save answers to a text file for submission within the same HTML page, and submit the text file as directed over the network.</li>
+<li>Grading answers from text files submitted by students can be done with a few keystrokes.</li>
+<li>A question begins with a short answer in a number or word.</li>
+<li>Questions with numeric answers can be converted to multiple choice questions simply by flipping the flag.</li>
+<li>Questions can start with multiple choice.</li>
+<li>Mathematical equations in LaTeX format can be included in both question texts and choices.</li>
+<li>Figures can be included in both question text and choices.</li>
+<li>Question text, mathematical equations, and figures are all randomly selected for each question sheet in a controlled manner.</li>
+<li>Randomness is acquired by executing the answer string, which is a short Python script, that is part of question.</li>
+<li>To increase your creativity, user-defined functions can be easily added for the answer string.</li>
 </ul>
 
 ## Where to get it
-<ul>
-<li>The source code is currently hosted on GitHub at: <a href="https://github.com/generateNscore/html4quiz">https://github.com/generateNscore/html4quiz</a></li>
-<br>
 
 <pre lang=sh>pip install html4quiz</pre>
 
+<ul>
+<li>The source code is currently hosted on GitHub at: <a href="https://github.com/generateNscore/html4quiz">https://github.com/generateNscore/html4quiz</a></li>
 </ul>
 
 
 ## Dependencies
 <ul><li>None</li></ul>
 
 
 ## Changes
-
+<ul>
+<li>Version 0.0.27</li>
+<ul><li>Deleted a incomplete feature.</li>
+<ul><li>It is postponed.</li></ul>
+</ul>
+<br>
+<li>Version 0.0.26</li>
+<ul><li>A bug in Javascript script in radiobuttons.</li>
+<ul><li>Fixed.</li></ul>
+</ul>
+<br>
+<li>Version 0.0.25</li>
+<ul><li>Testing for README.md link to GitHub.</li>
+</ul>
+<br>
 <li>Version 0.0.22</li>
 <ul><li>Added "res" folder to GitHub for the Javascript scripts of figures and additional data saved in JSON format.</li>
 <li>Added a "getResource()" function to the package to access the data.</li>
 <li>Some procedures of calling functions were removed to simplify the usages of package.</li>
 </ul>
-
+<br>
 <li>Version 0.0.21</li>
 <ul><li>Package name has been changed from htmlfilesforquiz to html4quiz</li>
 <li>So is the name of repository in GitHub.</li></ul>
-
+<br>
 <li>Version 0.0.20</li>
 
 <ul><li>Finallized a way to upload/download Javascript scripts saved in JSON files for figures.<a href="https://github.com/generateNscore/html4quiz/wiki#h-download-json-file-of-javascript-code-for-figure-contents">H. Download Json file of Javascript code for figure contents</a></li></ul>
 <br>
 
 <li>Version 0.0.16</li>
 
 <ul><li>In addition to typical short-answer questions that can be answered on the screen, a new kind questions for which students are required to "play" with mouse to complete a required task to answer is added.</li>
 <li>Example: <a href="https://generateNscore.github.io/html4quiz/Examples/Nk001/Nk001.py">Nk001.py</a></li>
-</ul></ul>
+</ul>
 <br>
 
 <li>Version 0.0.11</li>
 
 <ul><li>A way to stay in short-answer question is added as:</li>
   
 ```python
@@ -75,24 +86,25 @@
   ```python
   
 answer = [{'choices':None, 'ans':vA+vB, 'fn': 'variation0_int'}]
   
 ```
 
 <li>This is about <a href="https://github.com/generateNscore/html4quiz/wiki#2-specifying-method-of-converting-a-short-answer-to-a-set-of-choices">Specifying method of convering short-answer to a set of choices.</a></li></ul>
-
+</ul>
 
 
 ## Example shots
-
+<ul>
 <li>A short-answer question</li>
 <img src="https://generateNscore.github.io/html4quiz/img/example1-3.png">
 <li>A multiple-choice question</li>
 <img src="https://generateNscore.github.io/html4quiz/img/example1-6.png">
 <li>A multiple-choice question with a figure</li>
 <img src="https://generateNscore.github.io/html4quiz/img/example1-2.png">
 <li>A question with multiple-choice figures</li>
 <img src="https://generateNscore.github.io/html4quiz/img/example1-1.png">
 <li>A question with equation and with multiple-choices</li>
 <img src="https://generateNscore.github.io/html4quiz/img/example1-4.png">
 <li>A question with equation and with multiple-choice figures</li>
 <img src="https://generateNscore.github.io/html4quiz/img/example1-5.png">
+</ul>
```

#### html2text {}

```diff
@@ -1,68 +1,87 @@
-# html4quiz ## What is it? html4quiz is a package that generates question
-papers as HTML files to be distributed over the network and grades the answers
-in text files submitted by students. ## Help
-    * Documentation
-## Features
-    * Generates as many personalized question sheets in HTML files as one wants
-      with a few strings of text.
-    * The amount of random personalization is under full control of users.
-    * Each HTML file with a name corresponding to the identification number.
-    * Multi-choice as well as short, default, questions can be made.
-    * A figure, although a pre-made image can be used, can be varied as well as
-      questions.
-    * Mathematical equations can be included in questions with Latex.
-    * User defined functions can be easily added.
-    * With the question sheets in HTML files, students require only a web
-      browser to answer and send text files including the answers over the
-      network.
-    * Scoring all different answers in text files submitted can be done in a
-      second.
+# html4quiz ## What is it? html4quiz is a package that helps you generate
+question sheets with as many HTML files as you want and grade answers from text
+files submitted by students. ## Features
+    * Everything is on your local PC, grows with your creativity, and you own
+      them all.
+    * Question sheets in HTML files, each named with a corresponding
+      identification number, are distributed to students over the network.
+    * Students use their mobile devices to read, answer questions, save answers
+      to a text file for submission within the same HTML page, and submit the
+      text file as directed over the network.
+    * Grading answers from text files submitted by students can be done with a
+      few keystrokes.
+    * A question begins with a short answer in a number or word.
+    * Questions with numeric answers can be converted to multiple choice
+      questions simply by flipping the flag.
+    * Questions can start with multiple choice.
+    * Mathematical equations in LaTeX format can be included in both question
+      texts and choices.
+    * Figures can be included in both question text and choices.
+    * Question text, mathematical equations, and figures are all randomly
+      selected for each question sheet in a controlled manner.
+    * Randomness is acquired by executing the answer string, which is a short
+      Python script, that is part of question.
+    * To increase your creativity, user-defined functions can be easily added
+      for the answer string.
 ## Where to get it
+pip install html4quiz
     * The source code is currently hosted on GitHub at: https://github.com/
       generateNscore/html4quiz
-    *
-      pip install html4quiz
 ## Dependencies
     * None
 ## Changes
-Version 0.0.22
-    * Added "res" folder to GitHub for the Javascript scripts of figures and
-      additional data saved in JSON format.
-    * Added a "getResource()" function to the package to access the data.
-    * Some procedures of calling functions were removed to simplify the usages
-      of package.
-Version 0.0.21
-    * Package name has been changed from htmlfilesforquiz to html4quiz
-    * So is the name of repository in GitHub.
-Version 0.0.20
-    * Finallized a way to upload/download Javascript scripts saved in JSON
-      files for figures.H._Download_Json_file_of_Javascript_code_for_figure
-      contents
-
-Version 0.0.16
-    * In addition to typical short-answer questions that can be answered on the
-      screen, a new kind questions for which students are required to "play"
-      with mouse to complete a required task to answer is added.
-    * Example: Nk001.py
-
-Version 0.0.11
-    * A way to stay in short-answer question is added as:
-    * ```python answer = [{'choices':None, 'ans': ans}] ```
-          o This answering form is different from the one of
-    * ```python answer = [{'choices':None, 'ans':vA+vB, 'fn':
-      'variation0_int'}] ```
-    * This is about Specifying_method_of_convering_short-answer_to_a_set_of
-      choices.
+    * Version 0.0.27
+          o Deleted a incomplete feature.
+                # It is postponed.
+    *
+    * Version 0.0.26
+          o A bug in Javascript script in radiobuttons.
+                # Fixed.
+    *
+    * Version 0.0.25
+          o Testing for README.md link to GitHub.
+    *
+    * Version 0.0.22
+          o Added "res" folder to GitHub for the Javascript scripts of figures
+            and additional data saved in JSON format.
+          o Added a "getResource()" function to the package to access the data.
+          o Some procedures of calling functions were removed to simplify the
+            usages of package.
+    *
+    * Version 0.0.21
+          o Package name has been changed from htmlfilesforquiz to html4quiz
+          o So is the name of repository in GitHub.
+    *
+    * Version 0.0.20
+          o Finallized a way to upload/download Javascript scripts saved in
+            JSON files for figures.H._Download_Json_file_of_Javascript_code_for
+            figure_contents
+    *
+    * Version 0.0.16
+          o In addition to typical short-answer questions that can be answered
+            on the screen, a new kind questions for which students are required
+            to "play" with mouse to complete a required task to answer is
+            added.
+          o Example: Nk001.py
+    *
+    * Version 0.0.11
+          o A way to stay in short-answer question is added as:
+          o ```python answer = [{'choices':None, 'ans': ans}] ```
+                # This answering form is different from the one of
+          o ```python answer = [{'choices':None, 'ans':vA+vB, 'fn':
+            'variation0_int'}] ```
+          o This is about Specifying_method_of_convering_short-answer_to_a_set
+            of_choices.
 ## Example shots
-A short-answer question
-[https://generateNscore.github.io/html4quiz/img/example1-3.png]
-A multiple-choice question
-[https://generateNscore.github.io/html4quiz/img/example1-6.png]
-A multiple-choice question with a figure
-[https://generateNscore.github.io/html4quiz/img/example1-2.png]
-A question with multiple-choice figures
-[https://generateNscore.github.io/html4quiz/img/example1-1.png]
-A question with equation and with multiple-choices
-[https://generateNscore.github.io/html4quiz/img/example1-4.png]
-A question with equation and with multiple-choice figures
-[https://generateNscore.github.io/html4quiz/img/example1-5.png]
+    * A short-answer question
+    * [https://generateNscore.github.io/html4quiz/img/example1-3.png]
+    * A multiple-choice question
+    * [https://generateNscore.github.io/html4quiz/img/example1-6.png]
+    * A multiple-choice question with a figure
+    * [https://generateNscore.github.io/html4quiz/img/example1-2.png]
+    * A question with multiple-choice figures
+    * [https://generateNscore.github.io/html4quiz/img/example1-1.png]
+    * A question with equation and with multiple-choices
+    * [https://generateNscore.github.io/html4quiz/img/example1-4.png]
+    * A question with equation and with multiple-choice figures
+    * [https://generateNscore.github.io/html4quiz/img/example1-5.png]
```

### Comparing `html4quiz-0.0.26/0.0.22pyproject.toml` & `html4quiz-0.0.27/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "html4quiz"
-version = "0.0.22"
+version = "0.0.27"
 authors = [
   { name="Sukmock Lee", email="smlee@inha.ac.kr" },
 ]
-description = "A package that generates question papers as HTML files to be distributed over the network and grades the answers in text files submitted by students."
+description = "A package that generates questionnaires as HTML files to be distributed over the network and scores answers in text files submitted by students."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Topic :: Education :: Testing",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Intended Audience :: Education",
     "Intended Audience :: End Users/Desktop",
     "Development Status :: 4 - Beta"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/generateNscore/html4quiz"
-"Bug Tracker" = "https://github.com/generateNscore/html4quiz/issues"
+"Bug Tracker" = "https://github.com/generateNscore/html4quiz/issues"
+"Documentation" = "https://github.com/generateNscore/html4quiz/wiki"
+
```

### Comparing `html4quiz-0.0.26/updatePackage.txt` & `html4quiz-0.0.27/updatePackage.txt`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.26/src/html4quiz/_common.py` & `html4quiz-0.0.27/src/html4quiz/_common.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.26/src/html4quiz/_generateEm.py` & `html4quiz-0.0.27/src/html4quiz/_generateEm.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.26/src/html4quiz/_scoreEm.py` & `html4quiz-0.0.27/src/html4quiz/_scoreEm.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.26/src/html4quiz/makeChoices.py` & `html4quiz-0.0.27/src/html4quiz/makeChoices.py`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.26/LICENSE.txt` & `html4quiz-0.0.27/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `html4quiz-0.0.26/PKG-INFO` & `html4quiz-0.0.27/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html4quiz
-Version: 0.0.26
+Version: 0.0.27
 Summary: A package that generates questionnaires as HTML files to be distributed over the network and scores answers in text files submitted by students.
 Project-URL: Homepage, https://github.com/generateNscore/html4quiz
 Project-URL: Bug Tracker, https://github.com/generateNscore/html4quiz/issues
 Project-URL: Documentation, https://github.com/generateNscore/html4quiz/wiki
 Author-email: Sukmock Lee <smlee@inha.ac.kr>
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
@@ -33,15 +33,14 @@
 <li>Questions with numeric answers can be converted to multiple choice questions simply by flipping the flag.</li>
 <li>Questions can start with multiple choice.</li>
 <li>Mathematical equations in LaTeX format can be included in both question texts and choices.</li>
 <li>Figures can be included in both question text and choices.</li>
 <li>Question text, mathematical equations, and figures are all randomly selected for each question sheet in a controlled manner.</li>
 <li>Randomness is acquired by executing the answer string, which is a short Python script, that is part of question.</li>
 <li>To increase your creativity, user-defined functions can be easily added for the answer string.</li>
-<li>With some Javascript script coding, questions that require students to "play" for a period of time to answer correctly can be created.</li>
 </ul>
 
 ## Where to get it
 
 <pre lang=sh>pip install html4quiz</pre>
 
 <ul>
@@ -51,14 +50,19 @@
 
 ## Dependencies
 <ul><li>None</li></ul>
 
 
 ## Changes
 <ul>
+<li>Version 0.0.27</li>
+<ul><li>Deleted a incomplete feature.</li>
+<ul><li>It is postponed.</li></ul>
+</ul>
+<br>
 <li>Version 0.0.26</li>
 <ul><li>A bug in Javascript script in radiobuttons.</li>
 <ul><li>Fixed.</li></ul>
 </ul>
 <br>
 <li>Version 0.0.25</li>
 <ul><li>Testing for README.md link to GitHub.</li>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: html4quiz Version: 0.0.26 Summary: A package that
+Metadata-Version: 2.1 Name: html4quiz Version: 0.0.27 Summary: A package that
 generates questionnaires as HTML files to be distributed over the network and
 scores answers in text files submitted by students. Project-URL: Homepage,
 https://github.com/generateNscore/html4quiz Project-URL: Bug Tracker, https://
 github.com/generateNscore/html4quiz/issues Project-URL: Documentation, https://
 github.com/generateNscore/html4quiz/wiki Author-email: Sukmock Lee
 inha.ac.kr> License-File: LICENSE.txt Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Education Classifier: Intended Audience
@@ -30,23 +30,25 @@
     * Figures can be included in both question text and choices.
     * Question text, mathematical equations, and figures are all randomly
       selected for each question sheet in a controlled manner.
     * Randomness is acquired by executing the answer string, which is a short
       Python script, that is part of question.
     * To increase your creativity, user-defined functions can be easily added
       for the answer string.
-    * With some Javascript script coding, questions that require students to
-      "play" for a period of time to answer correctly can be created.
 ## Where to get it
 pip install html4quiz
     * The source code is currently hosted on GitHub at: https://github.com/
       generateNscore/html4quiz
 ## Dependencies
     * None
 ## Changes
+    * Version 0.0.27
+          o Deleted a incomplete feature.
+                # It is postponed.
+    *
     * Version 0.0.26
           o A bug in Javascript script in radiobuttons.
                 # Fixed.
     *
     * Version 0.0.25
           o Testing for README.md link to GitHub.
     *
```

