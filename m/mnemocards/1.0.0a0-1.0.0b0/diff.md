# Comparing `tmp/mnemocards-1.0.0a0.tar.gz` & `tmp/mnemocards-1.0.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mnemocards-1.0.0a0.tar", max compression
+gzip compressed data, was "mnemocards-1.0.0b0.tar", max compression
```

## Comparing `mnemocards-1.0.0a0.tar` & `mnemocards-1.0.0b0.tar`

### file list

```diff
@@ -1,35 +1,39 @@
--rw-r--r--   0        0        0     1097 2023-03-07 00:51:39.603756 mnemocards-1.0.0a0/LICENSE
--rw-r--r--   0        0        0     7317 2023-03-07 00:51:39.603756 mnemocards-1.0.0a0/README.md
--rw-r--r--   0        0        0     3523 2023-03-07 00:53:54.259044 mnemocards-1.0.0a0/pyproject.toml
--rw-r--r--   0        0        0      258 2023-03-07 00:51:39.607756 mnemocards-1.0.0a0/src/mnemocards/__init__.py
--rw-r--r--   0        0        0      117 2023-03-07 00:51:39.607756 mnemocards-1.0.0a0/src/mnemocards/__main__.py
--rw-r--r--   0        0        0     3763 2023-03-07 00:51:39.607756 mnemocards-1.0.0a0/src/mnemocards/cli.py
--rw-r--r--   0        0        0        0 2023-03-07 00:51:39.607756 mnemocards-1.0.0a0/src/mnemocards/py.typed
--rw-r--r--   0        0        0     1887 2023-03-07 00:51:39.607756 mnemocards-1.0.0a0/src/mnemocards/runner.py
--rw-r--r--   0        0        0      562 2023-03-07 00:51:39.607756 mnemocards-1.0.0a0/src/mnemocards/task.py
--rw-r--r--   0        0        0      144 2023-03-07 00:51:39.607756 mnemocards-1.0.0a0/src/mnemocards/types.py
--rw-r--r--   0        0        0     2441 2023-03-07 00:51:39.607756 mnemocards-1.0.0a0/src/mnemocards/utils.py
--rw-r--r--   0        0        0      393 2023-03-07 00:51:39.607756 mnemocards-1.0.0a0/src/mnemocards/version.py
--rw-r--r--   0        0        0      304 2023-03-07 00:51:39.607756 mnemocards-1.0.0a0/src/mnemocards_anki/__init__.py
--rw-r--r--   0        0        0      996 2023-03-07 00:51:39.607756 mnemocards-1.0.0a0/src/mnemocards_anki/configure.py
--rw-r--r--   0        0        0     1305 2023-03-07 00:51:39.607756 mnemocards-1.0.0a0/src/mnemocards_anki/models.py
--rw-r--r--   0        0        0     2458 2023-03-07 00:51:39.607756 mnemocards-1.0.0a0/src/mnemocards_anki/package.py
--rw-r--r--   0        0        0      961 2023-03-07 00:51:39.607756 mnemocards-1.0.0a0/src/mnemocards_anki/pronounce.py
--rw-r--r--   0        0        0      812 2023-03-07 00:51:39.607756 mnemocards-1.0.0a0/src/mnemocards_anki/simple_vocabulary.py
--rw-r--r--   0        0        0      238 2023-03-07 00:51:39.607756 mnemocards-1.0.0a0/src/mnemocards_anki/utils.py
--rw-r--r--   0        0        0     2366 2023-03-07 00:51:39.607756 mnemocards-1.0.0a0/src/mnemocards_anki/vocabulary.py
--rw-r--r--   0        0        0      599 2023-03-07 00:51:39.607756 mnemocards-1.0.0a0/src/mnemocards_essentials/__init__.py
--rw-r--r--   0        0        0      759 2023-03-07 00:51:39.607756 mnemocards-1.0.0a0/src/mnemocards_essentials/append_to_property.py
--rw-r--r--   0        0        0      931 2023-03-07 00:51:39.607756 mnemocards-1.0.0a0/src/mnemocards_essentials/directory.py
--rw-r--r--   0        0        0     1033 2023-03-07 00:51:39.607756 mnemocards-1.0.0a0/src/mnemocards_essentials/file.py
--rw-r--r--   0        0        0      517 2023-03-07 00:51:39.607756 mnemocards-1.0.0a0/src/mnemocards_essentials/git.py
--rw-r--r--   0        0        0     3773 2023-03-07 00:51:39.607756 mnemocards-1.0.0a0/src/mnemocards_essentials/markdown_card_extension.py
--rw-r--r--   0        0        0      815 2023-03-07 00:51:39.607756 mnemocards-1.0.0a0/src/mnemocards_essentials/pipeline.py
--rw-r--r--   0        0        0     1574 2023-03-07 00:51:39.607756 mnemocards-1.0.0a0/src/mnemocards_essentials/print.py
--rw-r--r--   0        0        0        0 2023-03-07 00:51:39.607756 mnemocards-1.0.0a0/src/mnemocards_essentials/py.typed
--rw-r--r--   0        0        0     3108 2023-03-07 00:51:39.607756 mnemocards-1.0.0a0/src/mnemocards_essentials/readers.py
--rw-r--r--   0        0        0      308 2023-03-07 00:51:39.607756 mnemocards-1.0.0a0/src/mnemocards_essentials/set_property.py
--rw-r--r--   0        0        0      792 2023-03-07 00:51:39.607756 mnemocards-1.0.0a0/src/mnemocards_essentials/stats.py
--rw-r--r--   0        0        0      828 2023-03-07 00:51:39.607756 mnemocards-1.0.0a0/src/mnemocards_essentials/union_pipeline.py
--rw-r--r--   0        0        0     8605 1970-01-01 00:00:00.000000 mnemocards-1.0.0a0/setup.py
--rw-r--r--   0        0        0     8430 1970-01-01 00:00:00.000000 mnemocards-1.0.0a0/PKG-INFO
+-rw-r--r--   0        0        0     1097 2023-04-16 04:08:51.875389 mnemocards-1.0.0b0/LICENSE
+-rw-r--r--   0        0        0     8821 2023-04-16 04:08:51.875389 mnemocards-1.0.0b0/README.md
+-rw-r--r--   0        0        0     3750 2023-04-16 04:09:29.119545 mnemocards-1.0.0b0/pyproject.toml
+-rw-r--r--   0        0        0      300 2023-04-16 04:08:51.879389 mnemocards-1.0.0b0/src/mnemocards/__init__.py
+-rw-r--r--   0        0        0      117 2023-04-16 04:08:51.879389 mnemocards-1.0.0b0/src/mnemocards/__main__.py
+-rw-r--r--   0        0        0     3903 2023-04-16 04:08:51.879389 mnemocards-1.0.0b0/src/mnemocards/cli.py
+-rw-r--r--   0        0        0        0 2023-04-16 04:08:51.879389 mnemocards-1.0.0b0/src/mnemocards/py.typed
+-rw-r--r--   0        0        0     1993 2023-04-16 04:08:51.879389 mnemocards-1.0.0b0/src/mnemocards/runner.py
+-rw-r--r--   0        0        0     1097 2023-04-16 04:08:51.879389 mnemocards-1.0.0b0/src/mnemocards/task.py
+-rw-r--r--   0        0        0      659 2023-04-16 04:08:51.879389 mnemocards-1.0.0b0/src/mnemocards/types.py
+-rw-r--r--   0        0        0     2769 2023-04-16 04:08:51.879389 mnemocards-1.0.0b0/src/mnemocards/utils.py
+-rw-r--r--   0        0        0      393 2023-04-16 04:08:51.879389 mnemocards-1.0.0b0/src/mnemocards/version.py
+-rw-r--r--   0        0        0      445 2023-04-16 04:08:51.879389 mnemocards-1.0.0b0/src/mnemocards_anki/__init__.py
+-rw-r--r--   0        0        0      996 2023-04-16 04:08:51.879389 mnemocards-1.0.0b0/src/mnemocards_anki/configure.py
+-rw-r--r--   0        0        0     1305 2023-04-16 04:08:51.879389 mnemocards-1.0.0b0/src/mnemocards_anki/models.py
+-rw-r--r--   0        0        0     2710 2023-04-16 04:08:51.879389 mnemocards-1.0.0b0/src/mnemocards_anki/package.py
+-rw-r--r--   0        0        0     2801 2023-04-16 04:08:51.879389 mnemocards-1.0.0b0/src/mnemocards_anki/pronounce.py
+-rw-r--r--   0        0        0        0 2023-04-16 04:08:51.879389 mnemocards-1.0.0b0/src/mnemocards_anki/py.typed
+-rw-r--r--   0        0        0      812 2023-04-16 04:08:51.879389 mnemocards-1.0.0b0/src/mnemocards_anki/simple_vocabulary_note_type.py
+-rw-r--r--   0        0        0      238 2023-04-16 04:08:51.879389 mnemocards-1.0.0b0/src/mnemocards_anki/utils.py
+-rw-r--r--   0        0        0     3524 2023-04-16 04:08:51.879389 mnemocards-1.0.0b0/src/mnemocards_anki/vocabulary_note_type.py
+-rw-r--r--   0        0        0      875 2023-04-16 04:08:51.879389 mnemocards-1.0.0b0/src/mnemocards_essentials/__init__.py
+-rw-r--r--   0        0        0     1234 2023-04-16 04:08:51.879389 mnemocards-1.0.0b0/src/mnemocards_essentials/append_to_property.py
+-rw-r--r--   0        0        0      885 2023-04-16 04:08:51.879389 mnemocards-1.0.0b0/src/mnemocards_essentials/directory.py
+-rw-r--r--   0        0        0      518 2023-04-16 04:08:51.879389 mnemocards-1.0.0b0/src/mnemocards_essentials/git.py
+-rw-r--r--   0        0        0     3765 2023-04-16 04:08:51.879389 mnemocards-1.0.0b0/src/mnemocards_essentials/markdown_card_extension.py
+-rw-r--r--   0        0        0     1014 2023-04-16 04:08:51.879389 mnemocards-1.0.0b0/src/mnemocards_essentials/pipeline.py
+-rw-r--r--   0        0        0     1981 2023-04-16 04:08:51.879389 mnemocards-1.0.0b0/src/mnemocards_essentials/print.py
+-rw-r--r--   0        0        0        0 2023-04-16 04:08:51.879389 mnemocards-1.0.0b0/src/mnemocards_essentials/py.typed
+-rw-r--r--   0        0        0      794 2023-04-16 04:08:51.879389 mnemocards-1.0.0b0/src/mnemocards_essentials/read_csv.py
+-rw-r--r--   0        0        0      460 2023-04-16 04:08:51.879389 mnemocards-1.0.0b0/src/mnemocards_essentials/read_json.py
+-rw-r--r--   0        0        0      818 2023-04-16 04:08:51.879389 mnemocards-1.0.0b0/src/mnemocards_essentials/read_toml.py
+-rw-r--r--   0        0        0      837 2023-04-16 04:08:51.879389 mnemocards-1.0.0b0/src/mnemocards_essentials/read_tsv.py
+-rw-r--r--   0        0        0      793 2023-04-16 04:08:51.879389 mnemocards-1.0.0b0/src/mnemocards_essentials/read_xml.py
+-rw-r--r--   0        0        0      479 2023-04-16 04:08:51.879389 mnemocards-1.0.0b0/src/mnemocards_essentials/read_yaml.py
+-rw-r--r--   0        0        0      308 2023-04-16 04:08:51.879389 mnemocards-1.0.0b0/src/mnemocards_essentials/set_property.py
+-rw-r--r--   0        0        0      792 2023-04-16 04:08:51.879389 mnemocards-1.0.0b0/src/mnemocards_essentials/stats.py
+-rw-r--r--   0        0        0      828 2023-04-16 04:08:51.879389 mnemocards-1.0.0b0/src/mnemocards_essentials/union_pipeline.py
+-rw-r--r--   0        0        0    10105 1970-01-01 00:00:00.000000 mnemocards-1.0.0b0/PKG-INFO
```

### Comparing `mnemocards-1.0.0a0/LICENSE` & `mnemocards-1.0.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `mnemocards-1.0.0a0/README.md` & `mnemocards-1.0.0b0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <p align="center">
     <a href="https://guiferviz.github.io/mnemocards" target="_blank">
-        <img src="/mnemocards/images/logo.jpg"
+        <img src="https://guiferviz.com/mnemocards/images/logo.jpg"
              alt="Mnemocards logo"
              width="200">
     </a>
 </p>
 <p align="center">
     <a href="https://github.com/guiferviz/mnemocards/actions/workflows/cicd.yaml" target="_blank">
         <img src="https://github.com/guiferviz/mnemocards/actions/workflows/cicd.yaml/badge.svg"
@@ -44,55 +44,62 @@
 :keyboard: **Source Code**:
 <a href="https://github.com/guiferviz/mnemocards" target="_blank">
     https://github.com/guiferviz/mnemocards
 </a>
 
 ---
 
+<p align="center">
+    <a href="https://guiferviz.github.io/mnemocards" target="_blank">
+        <img src="https://guiferviz.com/mnemocards/images/hello_hola_note.png"
+             alt="Mnemocards generated vocabulary card"
+             width="500">
+    </a>
+</p>
+
 ## 🤔 What is this?
 
 **Mnemocards** is a Python package originally intended for creating Anki
 flashcards from text files. It allows users to define a series of steps to read
 flashcards from any source, transform them and export them to different formats
-such as Anki APKG packages. Mnemocards is designed to be fully extensible,
-which means that users can create their own tasks and customize the card
-generation process to their specific needs.
-
-Reading **flashcards from text files** has several **advantages** over binary
-formats or manually creating cards in the Anki app. Text files are easily
-readable and editable by humans. This means that users can easily understand
-and modify the flashcard content **using common text editors**, and also can
-use version control systems like **Git to track changes and collaborate** with
-others.
+such as Anki APKG packages.
+
+Mnemocards is designed to be fully extensible, which means that users can
+create their own tasks and customize the card generation process to their
+specific needs. Indeed, Mnemocards has the versatility to be used for purposes
+beyond generating Anki decks.
 
 
 ## 🏷️ Features
 
-* Generates Anki APKG packages that you can later import into the Anki app.
-* Auto generate pronunciations from the words that you are learning.
-* Generates flashcards from text files that can be stored in Git repositories.
-This brings several positive things:
-    * Keep track of changes.
-    * Maintain different versions of flashcards using Git branches.
-    * Easily share and collaborate with others. If you know how to work with
-      Git you can create forks and pull requests to existing repositories.
-* Fully extensible architecture that allows you to define tasks that perform
-custom transformations on a list of notes.
-    * Possibility to export flashcards to other existing flashcards apps.
-    * Create indexes or analyze your collection of cards, create
-      visualizations, clustering, analyze how the cards relate to each other...
+* **Generate Anki APKG packages** that you can later import into the Anki app.
+* Auto **generate pronunciations** from the words that you are learning in any
+language supported by Google Translator.
+* Generate **flashcards from text files** that can be stored in Git
+repositories. This brings several positive things:
+    * Keep **track of changes**.
+    * Edit cards using your **favourite text editor**. I :heart: VIM.
+    * Easily **share and collaborate with others**. If you know how to work
+    with Git you can create forks and pull requests to existing repositories.
+* **Fully extensible architecture** that allows you to define custom
+transformations on a list of notes.
+    * Possibility to implement another way of exporting flashcards to other
+      existing flashcards apps. Contributions are welcome.
+    * Possibility to create search indexes, analyze your collection of cards,
+      create visualizations, clustering, analyze how the cards relate to each
+      other... Contributions are welcome.
 
 
-## 🤓 How it works?
+## ⚙️ Installation
 
 To get started with Mnemocards, you'll need to have Python >= 3.10 installed on
 your computer. Then, you can install Mnemocards using `pip`:
 
 ```cmd
-$ pip install mnemocards
+$ pip install --pre mnemocards
 ```
 
 You can check that the installation went well by executing the following
 command:
 
 ```cmd
 $ mnemocards --version
@@ -103,67 +110,115 @@
 │ <A super mega funny joke here> │
 ╰────────────────────────────────╯
 ```
 
 If the joke made you laugh you can continue with this tutorial, otherwise this
 program is not for you and you should consider other alternatives.
 
-Once you have Mnemocards installed, you can start creating your own flashcards.
-Let's start creating our own vocabulary file.
 
-You can use the provided sample files as a starting point, or create your own.
-Mnemocards uses a configuration file to define the steps that will be used to
-process the flashcards. In this file, you can specify the tasks that you want
-to use, the order in which they will be executed, and any necessary parameters
-or settings.
+## ❓How it works?
+
+Once you have Mnemocards installed, you can start creating your own flashcards.
+Let's start creating our own vocabulary Anki cards.
 
-Here's an example of a simple configuration file that reads in a CSV file containing flashcard data, and then generates an Anki APKG package:
+Imagine you are learning Spanish and you have a list of vocabulary like this:
 
-```yaml
-steps:
-  - type: ReadFile
-    path: flashcards.csv
-  - type: Anki
-    deck:
-      name: My Flashcards
-      id: b45f6d48-d1ab-4d0e-80a9-08a2ab473a41
-    note_type:
-      type: BasicNoteType
-  - type: Package
+English | Spanish |
+--------|---------|
+Hello   | Hola    |
+Bye     | Adiós   |
+
+If you want to use Mnemocards to generate Anki cards for those words the first
+thing you need to do is to create a CSV file like the following:
+
+```csv title="vocabulary.csv"
+your_language_word,language_you_learn_word,id
+Hello,Hola,9a6c9728-7f86-4e3f-9dec-a2f804bd0a76
+Bye,Adiós,e600a85a-8a6b-4449-a188-f7401dc69d6b
 ```
 
-In this example, the first step reads in a CSV file called "flashcards.csv", the second step generates an Anki package with a deck named "My Flashcards" and a specific id, and the last step creates the APKG package.
+A CSV file is a text file that represents a table. The first line is the header
+of the table, after that header line we have one line per row. Each column is
+separated from the other with a column. CSV stands for Comma-Separated Values.
+
+The first column contains the word in your native language, in this case
+English. The second row is the word in the language you are learning, Spanish.
+The last column is a randomly generated ID.
+
+!!! question "Why do we need an ID?"
+
+    IDs are used to uniquely identify a note in Anki. We can use the Spanish
+    word as an ID, but if you start studing a card and you want to make an edit
+    later the card will be considered as a complete new one, loosing your
+    progress.
+
+    For example, imagine you write *Adios* and after several days of study you
+    realise that your miss the accent. If you chage *Adios* to *Adiós* the
+    ID of that note will be different. To avoid this kind of problems I decided
+    to include an ID column.
+
+Mnemocards uses a configuration file named `mnemocards.yaml` to define the
+steps that will be used to process our flashcards. In this file, you can
+specify the tasks that you want to use, the order in which they will be
+executed, and any necessary parameters.
 
-You can run the configuration file using the mnemocards command:
+Here is an example of a simple configuration file that reads in a CSV file
+containing vocabulary data, and then generates an Anki APKG package:
 
-Copy code
-mnemocards run my_config.yml
-This will execute the steps in the configuration file, and create the Anki APKG package.
+```yaml title="mnemocards.yaml"
+steps:
+  # Read a CSV file with our spanish vocabulary.
+  - type: ReadCsv
+    path: vocabulary.csv
+  # Tag the generated notes and assign them to an Anki deck.
+  - type: mnemocards_anki.Configure
+    tags: spanish, languages
+    deck:
+      name: Spanish
+      id: 429d2604-ca8a-4c0a-9b03-38d1df5b9af7
+    note_type: mnemocards_anki.VocabularyNoteType
+  # Pronounce the spanish words using Google Translator.
+  - type: mnemocards_anki.Pronounce
+    language: es
+    attribute_to_pronounce: language_you_learn_word
+  # Save the Anki package.
+  - type: mnemocards_anki.Package
+  # Show the generated tasks in the terminal.
+  # Do not print the note id, the note_type and the deck to avoid cluttering the terminal.
+  - type: Print
+    ignore_regex: id|note_type|deck
+  # Show some stats of the generation process.
+  - type: Stats
+```
 
-You can also use the package to export your flashcards to other flashcard apps like Quizlet by adding a Quizlet task to the configuration file and providing the necessary credentials.
+You can run the configuration file using the following command:
 
-With Mnemocards, you can customize the flashcard generation process to suit your needs and easily collaborate with others. Give it a try and see how it can help you learn more efficiently!
+```cmd
+$ mnemocards run mnemocards.yml
+```
 
-TODO
+This will execute the steps in the configuration file, and will generate an
+Anki package named `out.apkg` by default. The generated file is in the same
+directory as your `mnemocards.yaml`.
 
+If you import the `apkg` file to Anki you can start studying Spanish:
 
-## 🧪 Examples
+<img src="https://guiferviz.com/mnemocards/images/hello_hola_note.png"
+     alt="Mnemocards generated vocabulary card"
+     width="400">
 
-<details markdown>
-<summary markdown>Japanese Flashcards :jp:</summary>
-Thinks you will learn:
 
-* UnionPipeline task.
-* Audio generation.
-</details>
+## 🤓 What is next?
 
+If you have come this far, it is because you may have found this project
+interesting. Consider visiting the
+[documentation](https://guiferviz.com/mnemocards), in particular the
+[examples](https://guiferviz.com/mnemocards/examples) section to learn more.
 
-## DELETEME: Fast ideas
+As mentioned above, Mnemocards is fully extensible, so any data source you miss
+or any processing or analysis you want to do on your cards is more than
+welcome. Feel free to [post your
+idea](https://github.com/guiferviz/mnemocards/discussions/categories/ideas) to
+start a discussion. Do not worry if you do not know how to program, there may
+be someone who can do it for you.
 
-Mnemocards is a tool for processing your flashcards.
-Mnemocards first appeared with the objective of generating Anki APKG packages that you can later import into the Anki app.
-Mnemocards allow us to generate our cards from text files that we can store in repositories.
-Having text files in repos allow us to keep track of the changes, maintain different versions of our flashcards and easily collaborate with others (creating forks of existing projects or creating pull requests, for example).
-It is fully extensible, you can define tasks that perform transformations on a list of notes.
-You can also auto generate pronunciations from the words that you are learning.
-You may even export your flashcards to other existing flashcards apps.
-The possibilities are endless, you can create an index or somehow analyze your collection of cards, create visualizations, clustering, analyze how the cards relate to each other...
+Enjoy learning!!!
```

#### html2text {}

```diff
@@ -1,77 +1,94 @@
                                [Mnemocards_logo]
    [Mnemocards_CI_pipeline_status] [Mnemocards_coverage_status] [Mnemocards
   issues] [Mnemocards_contributors] [Mnemocards_total_downloads] [Mnemocards
                              downloads_per_month]
 In addition to helping you memorise, this code helps you do other things that I
                                don't remember...
 --- :books: **Documentation**: https://guiferviz.com/mnemocards :keyboard:
-**Source Code**: https://github.com/guiferviz/mnemocards --- ## ð¤ What is
-this? **Mnemocards** is a Python package originally intended for creating Anki
-flashcards from text files. It allows users to define a series of steps to read
-flashcards from any source, transform them and export them to different formats
-such as Anki APKG packages. Mnemocards is designed to be fully extensible,
-which means that users can create their own tasks and customize the card
-generation process to their specific needs. Reading **flashcards from text
-files** has several **advantages** over binary formats or manually creating
-cards in the Anki app. Text files are easily readable and editable by humans.
-This means that users can easily understand and modify the flashcard content
-**using common text editors**, and also can use version control systems like
-**Git to track changes and collaborate** with others. ## ð·ï¸ Features *
-Generates Anki APKG packages that you can later import into the Anki app. *
-Auto generate pronunciations from the words that you are learning. * Generates
-flashcards from text files that can be stored in Git repositories. This brings
-several positive things: * Keep track of changes. * Maintain different versions
-of flashcards using Git branches. * Easily share and collaborate with others.
-If you know how to work with Git you can create forks and pull requests to
-existing repositories. * Fully extensible architecture that allows you to
-define tasks that perform custom transformations on a list of notes. *
-Possibility to export flashcards to other existing flashcards apps. * Create
-indexes or analyze your collection of cards, create visualizations, clustering,
-analyze how the cards relate to each other... ## ð¤ How it works? To get
-started with Mnemocards, you'll need to have Python >= 3.10 installed on your
-computer. Then, you can install Mnemocards using `pip`: ```cmd $ pip install
-mnemocards ``` You can check that the installation went well by executing the
-following command: ```cmd $ mnemocards --version
+**Source Code**: https://github.com/guiferviz/mnemocards ---
+                    [Mnemocards_generated_vocabulary_card]
+## ð¤ What is this? **Mnemocards** is a Python package originally intended
+for creating Anki flashcards from text files. It allows users to define a
+series of steps to read flashcards from any source, transform them and export
+them to different formats such as Anki APKG packages. Mnemocards is designed to
+be fully extensible, which means that users can create their own tasks and
+customize the card generation process to their specific needs. Indeed,
+Mnemocards has the versatility to be used for purposes beyond generating Anki
+decks. ## ð·ï¸ Features * **Generate Anki APKG packages** that you can later
+import into the Anki app. * Auto **generate pronunciations** from the words
+that you are learning in any language supported by Google Translator. *
+Generate **flashcards from text files** that can be stored in Git repositories.
+This brings several positive things: * Keep **track of changes**. * Edit cards
+using your **favourite text editor**. I :heart: VIM. * Easily **share and
+collaborate with others**. If you know how to work with Git you can create
+forks and pull requests to existing repositories. * **Fully extensible
+architecture** that allows you to define custom transformations on a list of
+notes. * Possibility to implement another way of exporting flashcards to other
+existing flashcards apps. Contributions are welcome. * Possibility to create
+search indexes, analyze your collection of cards, create visualizations,
+clustering, analyze how the cards relate to each other... Contributions are
+welcome. ## âï¸ Installation To get started with Mnemocards, you'll need to
+have Python >= 3.10 installed on your computer. Then, you can install
+Mnemocards using `pip`: ```cmd $ pip install --pre mnemocards ``` You can check
+that the installation went well by executing the following command: ```cmd $
+mnemocards --version
 ââ¦âââââââââ¦âââââââââââ¬ââââ¬ââââ
 ââââââââ£ ââââ ââ âââ¤ââ¬â âââââ
 â© â©âââââââ© â©âââââââ´
 â´â´ââââ´ââââ X.Y.Z
 â­âââââââââââââââââââââââââââââââââ®
 â â
 â°âââââââââââââââââââââââââââââââââ¯
 ``` If the joke made you laugh you can continue with this tutorial, otherwise
-this program is not for you and you should consider other alternatives. Once
-you have Mnemocards installed, you can start creating your own flashcards.
-Let's start creating our own vocabulary file. You can use the provided sample
-files as a starting point, or create your own. Mnemocards uses a configuration
-file to define the steps that will be used to process the flashcards. In this
-file, you can specify the tasks that you want to use, the order in which they
-will be executed, and any necessary parameters or settings. Here's an example
-of a simple configuration file that reads in a CSV file containing flashcard
-data, and then generates an Anki APKG package: ```yaml steps: - type: ReadFile
-path: flashcards.csv - type: Anki deck: name: My Flashcards id: b45f6d48-d1ab-
-4d0e-80a9-08a2ab473a41 note_type: type: BasicNoteType - type: Package ``` In
-this example, the first step reads in a CSV file called "flashcards.csv", the
-second step generates an Anki package with a deck named "My Flashcards" and a
-specific id, and the last step creates the APKG package. You can run the
-configuration file using the mnemocards command: Copy code mnemocards run
-my_config.yml This will execute the steps in the configuration file, and create
-the Anki APKG package. You can also use the package to export your flashcards
-to other flashcard apps like Quizlet by adding a Quizlet task to the
-configuration file and providing the necessary credentials. With Mnemocards,
-you can customize the flashcard generation process to suit your needs and
-easily collaborate with others. Give it a try and see how it can help you learn
-more efficiently! TODO ## ð§ª Examples  Japanese Flashcards :jp: Thinks you
-will learn: * UnionPipeline task. * Audio generation.  ## DELETEME: Fast ideas
-Mnemocards is a tool for processing your flashcards. Mnemocards first appeared
-with the objective of generating Anki APKG packages that you can later import
-into the Anki app. Mnemocards allow us to generate our cards from text files
-that we can store in repositories. Having text files in repos allow us to keep
-track of the changes, maintain different versions of our flashcards and easily
-collaborate with others (creating forks of existing projects or creating pull
-requests, for example). It is fully extensible, you can define tasks that
-perform transformations on a list of notes. You can also auto generate
-pronunciations from the words that you are learning. You may even export your
-flashcards to other existing flashcards apps. The possibilities are endless,
-you can create an index or somehow analyze your collection of cards, create
-visualizations, clustering, analyze how the cards relate to each other...
+this program is not for you and you should consider other alternatives. ##
+âHow it works? Once you have Mnemocards installed, you can start creating
+your own flashcards. Let's start creating our own vocabulary Anki cards.
+Imagine you are learning Spanish and you have a list of vocabulary like this:
+English | Spanish | --------|---------| Hello | Hola | Bye | AdiÃ³s | If you
+want to use Mnemocards to generate Anki cards for those words the first thing
+you need to do is to create a CSV file like the following: ```csv
+title="vocabulary.csv" your_language_word,language_you_learn_word,id
+Hello,Hola,9a6c9728-7f86-4e3f-9dec-a2f804bd0a76 Bye,AdiÃ³s,e600a85a-8a6b-4449-
+a188-f7401dc69d6b ``` A CSV file is a text file that represents a table. The
+first line is the header of the table, after that header line we have one line
+per row. Each column is separated from the other with a column. CSV stands for
+Comma-Separated Values. The first column contains the word in your native
+language, in this case English. The second row is the word in the language you
+are learning, Spanish. The last column is a randomly generated ID. !!! question
+"Why do we need an ID?" IDs are used to uniquely identify a note in Anki. We
+can use the Spanish word as an ID, but if you start studing a card and you want
+to make an edit later the card will be considered as a complete new one,
+loosing your progress. For example, imagine you write *Adios* and after several
+days of study you realise that your miss the accent. If you chage *Adios* to
+*AdiÃ³s* the ID of that note will be different. To avoid this kind of problems
+I decided to include an ID column. Mnemocards uses a configuration file named
+`mnemocards.yaml` to define the steps that will be used to process our
+flashcards. In this file, you can specify the tasks that you want to use, the
+order in which they will be executed, and any necessary parameters. Here is an
+example of a simple configuration file that reads in a CSV file containing
+vocabulary data, and then generates an Anki APKG package: ```yaml
+title="mnemocards.yaml" steps: # Read a CSV file with our spanish vocabulary. -
+type: ReadCsv path: vocabulary.csv # Tag the generated notes and assign them to
+an Anki deck. - type: mnemocards_anki.Configure tags: spanish, languages deck:
+name: Spanish id: 429d2604-ca8a-4c0a-9b03-38d1df5b9af7 note_type:
+mnemocards_anki.VocabularyNoteType # Pronounce the spanish words using Google
+Translator. - type: mnemocards_anki.Pronounce language: es
+attribute_to_pronounce: language_you_learn_word # Save the Anki package. -
+type: mnemocards_anki.Package # Show the generated tasks in the terminal. # Do
+not print the note id, the note_type and the deck to avoid cluttering the
+terminal. - type: Print ignore_regex: id|note_type|deck # Show some stats of
+the generation process. - type: Stats ``` You can run the configuration file
+using the following command: ```cmd $ mnemocards run mnemocards.yml ``` This
+will execute the steps in the configuration file, and will generate an Anki
+package named `out.apkg` by default. The generated file is in the same
+directory as your `mnemocards.yaml`. If you import the `apkg` file to Anki you
+can start studying Spanish: [Mnemocards generated vocabulary card] ## ð¤ What
+is next? If you have come this far, it is because you may have found this
+project interesting. Consider visiting the [documentation](https://
+guiferviz.com/mnemocards), in particular the [examples](https://guiferviz.com/
+mnemocards/examples) section to learn more. As mentioned above, Mnemocards is
+fully extensible, so any data source you miss or any processing or analysis you
+want to do on your cards is more than welcome. Feel free to [post your idea]
+(https://github.com/guiferviz/mnemocards/discussions/categories/ideas) to start
+a discussion. Do not worry if you do not know how to program, there may be
+someone who can do it for you. Enjoy learning!!!
```

### Comparing `mnemocards-1.0.0a0/pyproject.toml` & `mnemocards-1.0.0b0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mnemocards"
-version = "1.0.0a0"
+version = "1.0.0b0"
 description = "In addition to helping you memorise, this code helps you do other things that I don't remember..."
 packages = [
     { include = "mnemocards", from = "src" },
     { include = "mnemocards_essentials", from = "src" },
     { include = "mnemocards_anki", from = "src" },
 ]
 authors = ["guiferviz <guiferviz@gmail.com>"]
@@ -23,48 +23,48 @@
 "Bug Tracker" = "https://github.com/guiferviz/mnemocards/issues"
 "Source" = "https://github.com/guiferviz/mnemocards"
 "Documentation" = "https://guiferviz.github.io/mnemocards"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 fire = "^0.5.0"
-rich = "^13.2.0"
-pydantic = "^1.10.4"
+rich = "^13.3.4"
+pydantic = "^1.10.7"
 pyyaml = "^6.0"
+gtts = "^2.3.1"
+toml = "^0.10.2"
+xmltodict = "^0.13.0"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.2.0"
+pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
 pytest-mock = "^3.10.0"
-pytest-html = "^3.1.1"
+pytest-html = "^3.2.0"
 
 [tool.poetry.group.lint.dependencies]
-pre-commit = "^2.18.1"
-black = "^22.3.0"
-isort = "^5.10.1"
+pre-commit = "^3.2.2"
+black = "^23.3.0"
+isort = "^5.12.0"
 flake8 = "^6.0.0"
-pyright = "^1.1.284"
+pyright = "^1.1.303"
 pdbpp = "^0.10.3"
-mypy = "^0.991"
-flake8-pyproject = "^1.2.1"
-pydocstyle = "^6.1.1"
+mypy = "^1.2.0"
+flake8-pyproject = "^1.2.3"
+pydocstyle = "^6.3.0"
 pep8-naming = "^0.13.3"
 
 [tool.poetry.group.docs.dependencies]
-mkdocs-material = "^8.4.0"
-mkdocstrings = {extras = ["python"], version = "^0.19.0"}
+mkdocs-material = "^9.1.6"
+mkdocstrings = {extras = ["python"], version = "^0.21.2"}
 mkdocs-charts-plugin = "^0.0.8"
 mkdocs-macros-plugin = "^0.7.0"
-
-[tool.poetry.group.readers.dependencies]
-toml = "^0.10.2"
-xmltodict = "^0.13.0"
+mkdocs-section-index = "^0.3.5"
 
 [tool.poetry.group.anki.dependencies]
-anki = "^2.1.56"
+anki = "^2.1.61"
 genanki-mnemocards = "^0.13.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
@@ -130,14 +130,21 @@
 max-line-length = 100
 # Print the total number of errors.
 count = true
 # Print the source code generating the error/warning in question.
 show-source = true
 # Count the number of occurrences of each error/warning code and print a report.
 statistics = true
+# Consider pydantic validator as a classmethod decorator to avoid this error:
+# N805 first argument of a method should be named 'self'
+classmethod-decorators = [
+    "classmethod",
+    "validator",
+    "root_validator",
+]
 
 [tool.pydocstyle]
 convention = "google"
 add_ignore = [
     "D100",  # Missing docstring in public module
     "D101",  # Missing docstring in public class
     "D102",  # Missing docstring in public method
```

### Comparing `mnemocards-1.0.0a0/src/mnemocards/cli.py` & `mnemocards-1.0.0b0/src/mnemocards/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 import random
+import uuid
 
 from rich.console import Console
 from rich.logging import RichHandler
 from rich.panel import Panel
 from rich.theme import Theme
 
 import mnemocards
@@ -72,27 +73,34 @@
     def _greet(self):
         logo = f"[logo]{_LOGO}"
         version = f"[version]{mnemocards.__version__}"
         self._console.print(f"{logo} {version}")
         joke = random.choice(_JOKES)
         self._console.print(Panel.fit(f"[joke]{joke}"))
 
-    def run(self, directory: PathLike = ".", filename: str = "mnemocards.yaml"):
+    def run(
+        self, directory: PathLike = ".", filename: str = "mnemocards.yaml"
+    ) -> int:
         """Run a given Mnemocard task.
 
         Args:
-            directory: Directory to search for a Mnemocard Task definition.
-            filename: File name with the Mnemocard Task configuration.
+            directory: Directory to search for a Mnemocards Task definition.
+            filename: File name with the Mnemocards Task configuration.
         """
         self._console.print("[info]Hi! :waving_hand:")
         try:
             create_and_run_task(directory, filename)
         except Exception:
+            self._console.print_exception(
+                show_locals=self._log_level == "DEBUG"
+            )
             self._console.print(
                 "[warning]Although things didn't go as well as we expected,"
                 " hope to see you soon! :call_me_hand:"
             )
-            self._console.print_exception(
-                show_locals=self._log_level == "DEBUG"
-            )
-        else:
-            self._console.print("See you soon! :call_me_hand:")
+            return -1
+        self._console.print("See you soon! :call_me_hand:")
+        return 0
+
+    def id(self):
+        id_ = str(uuid.uuid4())
+        self._console.print(id_)
```

### Comparing `mnemocards-1.0.0a0/src/mnemocards/runner.py` & `mnemocards-1.0.0b0/src/mnemocards/runner.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,50 +1,52 @@
 import logging
 import pathlib
 import textwrap
 from typing import Any, Iterator, Tuple
 
 import pydantic
+import yaml
 from rich.console import Console
 
-import mnemocards_essentials as essentials
 from mnemocards import types, utils
 from mnemocards.task import Task
 
 logger = logging.getLogger(__name__)
 
 
 def create_and_run_task(directory: types.PathLike, filename: str):
-    task_config = create_task(directory, filename)
-    run_task(task_config)
+    directory = pathlib.Path(str(directory)).absolute()
+    with utils.use_cwd(directory):
+        task_config = create_task(directory, filename)
+        run_task(task_config)
 
 
 def read_task_config(
     directory: types.PathLike, filename: str
 ) -> Tuple[pathlib.Path, Any]:
     Console().print("[info]Looking for config files... :page_with_curl:")
     full_path = pathlib.Path(str(directory))
     if full_path.is_dir():
         full_path /= filename
     if not full_path.exists():
         raise FileNotFoundError(full_path)
-    reader = essentials.readers.InferReader()
-    return full_path, reader.load(full_path)
+    return full_path, yaml.safe_load(open(full_path, "r"))
 
 
 def create_task(
     directory: types.PathLike,
-    filename: str,
+    filename: str = "mnemocards.yaml",
     default_task: str = "mnemocards_essentials.Pipeline",
 ) -> Task:
     full_path, data = read_task_config(directory, filename)
     data.setdefault("type", default_task)
     task = None
     try:
-        task = utils.ClassModel(**data).to_object()
+        with utils.use_cwd(full_path.parent):
+            task = utils.ClassModel(**data).to_object()
     except pydantic.ValidationError as e:
         error_message = e.__context__ or e
         Console().print(
             f"[error]Invalid task found in `{full_path}` :cross_mark:\n"
             + textwrap.indent(str(error_message), prefix="\t"),
         )
         raise
```

### Comparing `mnemocards-1.0.0a0/src/mnemocards/utils.py` & `mnemocards-1.0.0b0/src/mnemocards/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,17 @@
+import contextlib
 import importlib
+import os
 import sys
 from typing import Any, Dict, Optional, Union
 
 import pydantic
 
+from mnemocards.types import PathLike
+
 
 class PydanticType:
     @classmethod
     def __get_validators__(cls):
         yield cls.validate
 
     @classmethod
@@ -44,16 +48,18 @@
     @classmethod
     def validate_type_exists(cls, type_):
         if type_ is not None:
             try:
                 member_from_qualified_name(
                     type_, default_module="mnemocards_essentials"
                 )
-            except (AttributeError, ImportError):
-                raise ValueError(f"`{type_}` not found or errors during import")
+            except (AttributeError, ImportError) as e:
+                raise ValueError(
+                    f"`{type_}` not found or errors during import: {str(e)}"
+                )
         return type_
 
     def to_object(self):
         member = member_from_qualified_name(
             self.type_, default_module="mnemocards_essentials"
         )
         return member(**self.params)
@@ -72,7 +78,18 @@
             name = f"{default_module}.{name}"
         else:
             raise ImportError(
                 f"`{name}` is not a qualified name: module missing."
             )
     module_name, member_name = name.rsplit(".", 1)
     return get_module_member(module_name, member_name)
+
+
+@contextlib.contextmanager
+def use_cwd(new_wd: PathLike):
+    new_wd_str = str(new_wd)
+    old_path = os.getcwd()
+    try:
+        os.chdir(new_wd_str)
+        yield
+    finally:
+        os.chdir(old_path)
```

### Comparing `mnemocards-1.0.0a0/src/mnemocards_anki/configure.py` & `mnemocards-1.0.0b0/src/mnemocards_anki/configure.py`

 * *Files identical despite different names*

### Comparing `mnemocards-1.0.0a0/src/mnemocards_anki/models.py` & `mnemocards-1.0.0b0/src/mnemocards_anki/models.py`

 * *Files identical despite different names*

### Comparing `mnemocards-1.0.0a0/src/mnemocards_anki/package.py` & `mnemocards-1.0.0b0/src/mnemocards_anki/package.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 from collections import defaultdict
 from typing import Dict, List
 
 import genanki
 import pydantic
 
-from mnemocards import NoteDict, PydanticTask
+from mnemocards import NoteDict, Path, PydanticTask
 from mnemocards_anki import models
 from mnemocards_anki.models import Deck, NoteType
 from mnemocards_anki.utils import get_hash_id
 
 logger = logging.getLogger(__name__)
 
 
@@ -20,15 +20,21 @@
 
     @property
     def guid(self):
         return self.note_id
 
 
 class Package(PydanticTask):
-    path: str = "out.apkg"
+    """Create an Anki package.
+
+    Attributes:
+        path: Path (directory + filename) of the output `*.apkg` file.
+    """
+
+    path: Path = Path("out.apkg")
     _notes: Dict[Deck, Dict[NoteType, List[NoteDict]]] = pydantic.PrivateAttr(
         defaultdict(lambda: defaultdict(lambda: []))
     )
 
     def start(self):
         logger.debug("Anki packaging `start` method.")
 
@@ -38,14 +44,15 @@
         note_type = note["note_type"]
         self._notes[deck][note_type] += [note]
         return note
 
     def end(self):
         logger.debug("Anki packaging `end` method.")
         genanki_decks: List[genanki.Deck] = []
+        media_files: list[str] = []
         for deck, types2notes in self._notes.items():
             genanki_deck = genanki.Deck(deck.id, deck.name)
             for note_type, notes in types2notes.items():
                 fields = [
                     i
                     for i in note_type.model.__fields__
                     if i not in models.Note.__fields__
@@ -65,10 +72,11 @@
                     genanki_note = NoteID(
                         i["id"],
                         model=genanki_note_type,
                         fields=field_values,
                         tags=i["tags"],
                     )
                     genanki_deck.add_note(genanki_note)
+                    media_files.extend(i["media_files"])
             genanki_decks.append(genanki_deck)
-        package = genanki.Package(genanki_decks)
-        package.write_to_file(self.path)
+        package = genanki.Package(genanki_decks, media_files)
+        package.write_to_file(str(self.path))
```

### Comparing `mnemocards-1.0.0a0/src/mnemocards_anki/simple_vocabulary.py` & `mnemocards-1.0.0b0/src/mnemocards_anki/simple_vocabulary_note_type.py`

 * *Files identical despite different names*

### Comparing `mnemocards-1.0.0a0/src/mnemocards_anki/vocabulary.py` & `mnemocards-1.0.0b0/src/mnemocards_anki/vocabulary_note_type.py`

 * *Files 17% similar despite different names*

```diff
@@ -77,8 +77,34 @@
                 <div class="origin comment">{{your_language_description}}</div>
                 <hr>
                 <div class="destination word">{{language_you_learn_word}}</div>
                 <div class="destination fonetic">{{language_you_learn_pronunciation}}</div>
                 <div class="destination comment">{{language_you_learn_description}}</div>
             """,
         ),
+        models.CardSides(
+            name="Language you learn --> Your language",
+            front="""
+                <style>
+                    .card {
+                        background: {{color}};
+                    }
+                </style>
+                <div class="destination word">{{language_you_learn_word}}</div>
+                <div class="destination fonetic">{{language_you_learn_pronunciation}}</div>
+                <div class="destination comment">{{language_you_learn_description}}</div>
+            """,
+            back="""
+                <style>
+                    .card {
+                        background: {{color}};
+                    }
+                </style>
+                <div class="destination word">{{language_you_learn_word}}</div>
+                <div class="destination fonetic">{{language_you_learn_pronunciation}}</div>
+                <div class="destination comment">{{language_you_learn_description}}</div>
+                <hr>
+                <div class="origin word">{{your_language_word}}</div>
+                <div class="origin comment">{{your_language_description}}</div>
+            """,
+        ),
     ]
```

### Comparing `mnemocards-1.0.0a0/src/mnemocards_essentials/__init__.py` & `mnemocards-1.0.0b0/src/mnemocards_essentials/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,15 @@
-from mnemocards_essentials import readers as readers
 from mnemocards_essentials.append_to_property import (
     AppendToProperty as AppendToProperty,
 )
 from mnemocards_essentials.directory import Directory as Directory
-from mnemocards_essentials.file import File as File
 from mnemocards_essentials.pipeline import Pipeline as Pipeline
 from mnemocards_essentials.print import Print as Print
+from mnemocards_essentials.read_csv import ReadCsv as ReadCsv
+from mnemocards_essentials.read_json import ReadJson as ReadJson
+from mnemocards_essentials.read_toml import ReadToml as ReadToml
+from mnemocards_essentials.read_tsv import ReadTsv as ReadTsv
+from mnemocards_essentials.read_xml import ReadXml as ReadXml
+from mnemocards_essentials.read_yaml import ReadYaml as ReadYaml
 from mnemocards_essentials.set_property import SetProperty as SetProperty
 from mnemocards_essentials.stats import Stats as Stats
 from mnemocards_essentials.union_pipeline import UnionPipeline as UnionPipeline
```

### Comparing `mnemocards-1.0.0a0/src/mnemocards_essentials/directory.py` & `mnemocards-1.0.0b0/src/mnemocards_essentials/directory.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 import logging
 from typing import Iterable
 
 import pydantic
 
-from mnemocards import NoteDict, PydanticTask, Task, runner
+from mnemocards import NoteDict, Path, PydanticTask, Task, runner
 
 logger = logging.getLogger(__name__)
 
 
 class Directory(PydanticTask):
     """Read a pipeline object from another directory.
 
     Attributes:
         path: Path to the root directory in which the configuration file is.
             You can also specify a different configuration name.
     """
 
-    path: str
-    filename: str = "mnemocards.yaml"
+    path: Path
     _task: Task = pydantic.PrivateAttr()
 
     def start(self):
         logger.debug("Directory `start` method.")
-        self._task = runner.create_task(self.path, self.filename)
+        self._task = runner.create_task(self.path)
         self._task.start()
 
     def process(self, notes: Iterable[NoteDict]) -> Iterable[NoteDict]:
         logger.debug("Directory `process` method.")
         return self._task.process(notes)
 
     def end(self):
```

### Comparing `mnemocards-1.0.0a0/src/mnemocards_essentials/file.py` & `mnemocards-1.0.0b0/src/mnemocards_essentials/read_toml.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 import itertools
-from typing import Iterable
+from typing import Any, Iterable
 
-from mnemocards import NoteDict, PydanticTask
-from mnemocards_essentials import readers
+import toml
 
+from mnemocards import NoteDict, Path, PydanticTask
 
-def get_first_list_property(value, depth=10):
-    if type(value) == list:
-        return value
-    if type(value) == dict:
-        if len(value) != 1:
-            raise ValueError("Dictionary with more than one entry")
-        first_value = next(iter(value.values()))
-        return get_first_list_property(first_value, depth - 1)
-    raise TypeError("unknown data type returned by a reader")
 
+def _get_first_list_property(value) -> list:
+    if len(value) != 1:
+        raise ValueError("Dictionary with more than one entry")
+    return next(iter(value.values()))
 
-class File(PydanticTask):
-    """Read a file.
+
+class ReadToml(PydanticTask):
+    """Read a TOML file.
 
     Attributes:
-        path: Path (directory and filename) of the file to read.
-        reader: Class used to read the given file.
+        path: Path (directory + filename) of the TOML file to read.
+        options: Extra parameters to pass to the `toml.loads` function.
     """
 
-    path: str
-    reader: readers.Reader = readers.InferReader()
+    path: Path
+    options: dict[str, Any] = {}
 
     def process(self, notes: Iterable[NoteDict]) -> Iterable[NoteDict]:
-        notes_from_file = self.reader.load(self.path)
-        notes_from_file = get_first_list_property(notes_from_file)
-        return itertools.chain(notes, notes_from_file)
+        file = open(self.path, "r")
+        dictionary = toml.load(file, **self.options)
+        rows = _get_first_list_property(dictionary)
+        return itertools.chain(notes, rows)
```

### Comparing `mnemocards-1.0.0a0/src/mnemocards_essentials/git.py` & `mnemocards-1.0.0b0/src/mnemocards_essentials/git.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from mnemocards import PydanticTask
 
 
-class GitRepo(PydanticTask):
+class _GitRepo(PydanticTask):
     """Retrieve a Mnemocards project from an external Git repository.
 
     Attributes:
         repo_url: URL of the Git repository.
         clone_path: Local path where the repository will be cloned.
         config_path: Path to the configuration file within the repository.
     """
```

### Comparing `mnemocards-1.0.0a0/src/mnemocards_essentials/markdown_card_extension.py` & `mnemocards-1.0.0b0/src/mnemocards_essentials/markdown_card_extension.py`

 * *Files 5% similar despite different names*

```diff
@@ -92,10 +92,10 @@
 class MnemocardsCardExtension(Extension):
     def extendMarkdown(self, md):  # noqa: N802
         md.parser.blockprocessors.register(
             CardBlockProcessor(md.parser), "card", 175
         )
 
 
+# Method needed to convert this module in a markdown extension.
 def makeExtension(*args, **kwargs):  # noqa: N802
-    """Method needed to convert this module in a markdown extension."""
     return MnemocardsCardExtension(*args, **kwargs)
```

### Comparing `mnemocards-1.0.0a0/src/mnemocards_essentials/pipeline.py` & `mnemocards-1.0.0b0/src/mnemocards_essentials/union_pipeline.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Iterable, List, Optional
 
 import pydantic
 
 from mnemocards import NoteDict, PydanticTask, Task
 
 
-class Pipeline(PydanticTask):
+class UnionPipeline(PydanticTask):
     name: Optional[str] = None
     steps: List[Task]
 
     @pydantic.validator("steps")
     @classmethod
     def validate_at_least_one_step(cls, value):
         if value is not None and not len(value):
@@ -20,14 +20,14 @@
         return len(self.steps)
 
     def start(self):
         for i in self.steps:
             i.start()
 
     def process(self, notes: Iterable[NoteDict]) -> Iterable[NoteDict]:
-        for task in self.steps:
-            notes = task.process(notes)
-        yield from notes
+        for i in self.steps:
+            step_notes = i.process(notes)
+            yield from step_notes
 
     def end(self):
         for i in self.steps:
             i.end()
```

### Comparing `mnemocards-1.0.0a0/src/mnemocards_essentials/print.py` & `mnemocards-1.0.0b0/src/mnemocards_essentials/print.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,19 +10,30 @@
 from rich.syntax import Syntax
 
 from mnemocards import task
 from mnemocards.types import NoteDict
 
 
 class PrintFormat(str, Enum):
+    """Possible formats that can be used in [`Print`][mnemocards_essentials.print.Print]."""
+
     YAML = "yaml"
     JSON = "json"
 
 
 class Print(task.Task, pydantic.BaseModel):
+    """Print every processed note in the terminal.
+
+    Attributes:
+        format_: Format to use when printing the notes.
+        sort_keys: Show note properties sorted alphabetically.
+        ignore_regex: If any note property match this regex it will not be
+            included in the printed note.
+    """
+
     format_: PrintFormat = pydantic.Field(PrintFormat.YAML, alias="format")
     sort_keys: bool = False
     ignore_regex: Optional[Pattern] = None
     _count: int = pydantic.PrivateAttr(0)
 
     @pydantic.validator("ignore_regex", pre=True)
     @classmethod
```

### Comparing `mnemocards-1.0.0a0/src/mnemocards_essentials/stats.py` & `mnemocards-1.0.0b0/src/mnemocards_essentials/stats.py`

 * *Files identical despite different names*

### Comparing `mnemocards-1.0.0a0/setup.py` & `mnemocards-1.0.0b0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,256 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: mnemocards
+Version: 1.0.0b0
+Summary: In addition to helping you memorise, this code helps you do other things that I don't remember...
+Home-page: https://github.com/guiferviz/mnemocards
+License: MIT
+Keywords: mnemocards
+Author: guiferviz
+Author-email: guiferviz@gmail.com
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Software Development
+Requires-Dist: fire (>=0.5.0,<0.6.0)
+Requires-Dist: gtts (>=2.3.1,<3.0.0)
+Requires-Dist: pydantic (>=1.10.7,<2.0.0)
+Requires-Dist: pyyaml (>=6.0,<7.0)
+Requires-Dist: rich (>=13.3.4,<14.0.0)
+Requires-Dist: toml (>=0.10.2,<0.11.0)
+Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
+Project-URL: Bug Tracker, https://github.com/guiferviz/mnemocards/issues
+Project-URL: Documentation, https://guiferviz.github.io/mnemocards
+Project-URL: Repository, https://github.com/guiferviz/mnemocards
+Project-URL: Source, https://github.com/guiferviz/mnemocards
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': 'src',
- 'mnemocards_anki': 'src/mnemocards_anki',
- 'mnemocards_essentials': 'src/mnemocards_essentials'}
-
-packages = \
-['mnemocards', 'mnemocards_anki', 'mnemocards_essentials']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['fire>=0.5.0,<0.6.0',
- 'pydantic>=1.10.4,<2.0.0',
- 'pyyaml>=6.0,<7.0',
- 'rich>=13.2.0,<14.0.0']
-
-entry_points = \
-{'console_scripts': ['mnemocards = mnemocards.__main__:main']}
-
-setup_kwargs = {
-    'name': 'mnemocards',
-    'version': '1.0.0a0',
-    'description': "In addition to helping you memorise, this code helps you do other things that I don't remember...",
-    'long_description': '<p align="center">\n    <a href="https://guiferviz.github.io/mnemocards" target="_blank">\n        <img src="/mnemocards/images/logo.jpg"\n             alt="Mnemocards logo"\n             width="200">\n    </a>\n</p>\n<p align="center">\n    <a href="https://github.com/guiferviz/mnemocards/actions/workflows/cicd.yaml" target="_blank">\n        <img src="https://github.com/guiferviz/mnemocards/actions/workflows/cicd.yaml/badge.svg"\n             alt="Mnemocards CI pipeline status">\n    </a>\n    <a href="https://app.codecov.io/gh/guiferviz/mnemocards/" target="_blank">\n        <img src="https://img.shields.io/codecov/c/github/aidictive/mnemocards"\n             alt="Mnemocards coverage status">\n    </a>\n    <a href="https://github.com/guiferviz/mnemocards/issues" target="_blank">\n        <img src="https://img.shields.io/github/issues/guiferviz/mnemocards"\n             alt="Mnemocards issues">\n    </a>\n    <a href="https://github.com/aidictive/mnemocards/graphs/contributors" target="_blank">\n        <img src="https://img.shields.io/github/contributors/guiferviz/mnemocards"\n             alt="Mnemocards contributors">\n    </a>\n    <a href="https://pypi.org/project/mnemocards/" target="_blank">\n        <img src="https://pepy.tech/badge/mnemocards"\n             alt="Mnemocards total downloads">\n    </a>\n    <a href="https://pypi.org/project/mnemocards/" target="_blank">\n        <img src="https://pepy.tech/badge/mnemocards/month"\n             alt="Mnemocards downloads per month">\n    </a>\n    <br />\n    In addition to helping you memorise, this code helps you do other things that I don\'t remember...\n</p>\n\n---\n\n:books: **Documentation**:\n<a href="https://guiferviz.com/mnemocards" target="_blank">\n    https://guiferviz.com/mnemocards\n</a>\n\n:keyboard: **Source Code**:\n<a href="https://github.com/guiferviz/mnemocards" target="_blank">\n    https://github.com/guiferviz/mnemocards\n</a>\n\n---\n\n## 🤔 What is this?\n\n**Mnemocards** is a Python package originally intended for creating Anki\nflashcards from text files. It allows users to define a series of steps to read\nflashcards from any source, transform them and export them to different formats\nsuch as Anki APKG packages. Mnemocards is designed to be fully extensible,\nwhich means that users can create their own tasks and customize the card\ngeneration process to their specific needs.\n\nReading **flashcards from text files** has several **advantages** over binary\nformats or manually creating cards in the Anki app. Text files are easily\nreadable and editable by humans. This means that users can easily understand\nand modify the flashcard content **using common text editors**, and also can\nuse version control systems like **Git to track changes and collaborate** with\nothers.\n\n\n## 🏷️ Features\n\n* Generates Anki APKG packages that you can later import into the Anki app.\n* Auto generate pronunciations from the words that you are learning.\n* Generates flashcards from text files that can be stored in Git repositories.\nThis brings several positive things:\n    * Keep track of changes.\n    * Maintain different versions of flashcards using Git branches.\n    * Easily share and collaborate with others. If you know how to work with\n      Git you can create forks and pull requests to existing repositories.\n* Fully extensible architecture that allows you to define tasks that perform\ncustom transformations on a list of notes.\n    * Possibility to export flashcards to other existing flashcards apps.\n    * Create indexes or analyze your collection of cards, create\n      visualizations, clustering, analyze how the cards relate to each other...\n\n\n## 🤓 How it works?\n\nTo get started with Mnemocards, you\'ll need to have Python >= 3.10 installed on\nyour computer. Then, you can install Mnemocards using `pip`:\n\n```cmd\n$ pip install mnemocards\n```\n\nYou can check that the installation went well by executing the following\ncommand:\n\n```cmd\n$ mnemocards --version\n╔╦╗╔╗╔╔═╗╔╦╗╔═╗┌─┐┌─┐┬─┐┌┬┐┌─┐\n║║║║║║║╣ ║║║║ ║│  ├─┤├┬┘ ││└─┐\n╩ ╩╝╚╝╚═╝╩ ╩╚═╝└─┘┴ ┴┴└──┴┘└─┘ X.Y.Z\n╭────────────────────────────────╮\n│ <A super mega funny joke here> │\n╰────────────────────────────────╯\n```\n\nIf the joke made you laugh you can continue with this tutorial, otherwise this\nprogram is not for you and you should consider other alternatives.\n\nOnce you have Mnemocards installed, you can start creating your own flashcards.\nLet\'s start creating our own vocabulary file.\n\nYou can use the provided sample files as a starting point, or create your own.\nMnemocards uses a configuration file to define the steps that will be used to\nprocess the flashcards. In this file, you can specify the tasks that you want\nto use, the order in which they will be executed, and any necessary parameters\nor settings.\n\nHere\'s an example of a simple configuration file that reads in a CSV file containing flashcard data, and then generates an Anki APKG package:\n\n```yaml\nsteps:\n  - type: ReadFile\n    path: flashcards.csv\n  - type: Anki\n    deck:\n      name: My Flashcards\n      id: b45f6d48-d1ab-4d0e-80a9-08a2ab473a41\n    note_type:\n      type: BasicNoteType\n  - type: Package\n```\n\nIn this example, the first step reads in a CSV file called "flashcards.csv", the second step generates an Anki package with a deck named "My Flashcards" and a specific id, and the last step creates the APKG package.\n\nYou can run the configuration file using the mnemocards command:\n\nCopy code\nmnemocards run my_config.yml\nThis will execute the steps in the configuration file, and create the Anki APKG package.\n\nYou can also use the package to export your flashcards to other flashcard apps like Quizlet by adding a Quizlet task to the configuration file and providing the necessary credentials.\n\nWith Mnemocards, you can customize the flashcard generation process to suit your needs and easily collaborate with others. Give it a try and see how it can help you learn more efficiently!\n\nTODO\n\n\n## 🧪 Examples\n\n<details markdown>\n<summary markdown>Japanese Flashcards :jp:</summary>\nThinks you will learn:\n\n* UnionPipeline task.\n* Audio generation.\n</details>\n\n\n## DELETEME: Fast ideas\n\nMnemocards is a tool for processing your flashcards.\nMnemocards first appeared with the objective of generating Anki APKG packages that you can later import into the Anki app.\nMnemocards allow us to generate our cards from text files that we can store in repositories.\nHaving text files in repos allow us to keep track of the changes, maintain different versions of our flashcards and easily collaborate with others (creating forks of existing projects or creating pull requests, for example).\nIt is fully extensible, you can define tasks that perform transformations on a list of notes.\nYou can also auto generate pronunciations from the words that you are learning.\nYou may even export your flashcards to other existing flashcards apps.\nThe possibilities are endless, you can create an index or somehow analyze your collection of cards, create visualizations, clustering, analyze how the cards relate to each other...\n',
-    'author': 'guiferviz',
-    'author_email': 'guiferviz@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/guiferviz/mnemocards',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.10,<4.0',
-}
+<p align="center">
+    <a href="https://guiferviz.github.io/mnemocards" target="_blank">
+        <img src="https://guiferviz.com/mnemocards/images/logo.jpg"
+             alt="Mnemocards logo"
+             width="200">
+    </a>
+</p>
+<p align="center">
+    <a href="https://github.com/guiferviz/mnemocards/actions/workflows/cicd.yaml" target="_blank">
+        <img src="https://github.com/guiferviz/mnemocards/actions/workflows/cicd.yaml/badge.svg"
+             alt="Mnemocards CI pipeline status">
+    </a>
+    <a href="https://app.codecov.io/gh/guiferviz/mnemocards/" target="_blank">
+        <img src="https://img.shields.io/codecov/c/github/aidictive/mnemocards"
+             alt="Mnemocards coverage status">
+    </a>
+    <a href="https://github.com/guiferviz/mnemocards/issues" target="_blank">
+        <img src="https://img.shields.io/github/issues/guiferviz/mnemocards"
+             alt="Mnemocards issues">
+    </a>
+    <a href="https://github.com/aidictive/mnemocards/graphs/contributors" target="_blank">
+        <img src="https://img.shields.io/github/contributors/guiferviz/mnemocards"
+             alt="Mnemocards contributors">
+    </a>
+    <a href="https://pypi.org/project/mnemocards/" target="_blank">
+        <img src="https://pepy.tech/badge/mnemocards"
+             alt="Mnemocards total downloads">
+    </a>
+    <a href="https://pypi.org/project/mnemocards/" target="_blank">
+        <img src="https://pepy.tech/badge/mnemocards/month"
+             alt="Mnemocards downloads per month">
+    </a>
+    <br />
+    In addition to helping you memorise, this code helps you do other things that I don't remember...
+</p>
 
+---
+
+:books: **Documentation**:
+<a href="https://guiferviz.com/mnemocards" target="_blank">
+    https://guiferviz.com/mnemocards
+</a>
+
+:keyboard: **Source Code**:
+<a href="https://github.com/guiferviz/mnemocards" target="_blank">
+    https://github.com/guiferviz/mnemocards
+</a>
+
+---
+
+<p align="center">
+    <a href="https://guiferviz.github.io/mnemocards" target="_blank">
+        <img src="https://guiferviz.com/mnemocards/images/hello_hola_note.png"
+             alt="Mnemocards generated vocabulary card"
+             width="500">
+    </a>
+</p>
+
+## 🤔 What is this?
+
+**Mnemocards** is a Python package originally intended for creating Anki
+flashcards from text files. It allows users to define a series of steps to read
+flashcards from any source, transform them and export them to different formats
+such as Anki APKG packages.
+
+Mnemocards is designed to be fully extensible, which means that users can
+create their own tasks and customize the card generation process to their
+specific needs. Indeed, Mnemocards has the versatility to be used for purposes
+beyond generating Anki decks.
+
+
+## 🏷️ Features
+
+* **Generate Anki APKG packages** that you can later import into the Anki app.
+* Auto **generate pronunciations** from the words that you are learning in any
+language supported by Google Translator.
+* Generate **flashcards from text files** that can be stored in Git
+repositories. This brings several positive things:
+    * Keep **track of changes**.
+    * Edit cards using your **favourite text editor**. I :heart: VIM.
+    * Easily **share and collaborate with others**. If you know how to work
+    with Git you can create forks and pull requests to existing repositories.
+* **Fully extensible architecture** that allows you to define custom
+transformations on a list of notes.
+    * Possibility to implement another way of exporting flashcards to other
+      existing flashcards apps. Contributions are welcome.
+    * Possibility to create search indexes, analyze your collection of cards,
+      create visualizations, clustering, analyze how the cards relate to each
+      other... Contributions are welcome.
+
+
+## ⚙️ Installation
+
+To get started with Mnemocards, you'll need to have Python >= 3.10 installed on
+your computer. Then, you can install Mnemocards using `pip`:
+
+```cmd
+$ pip install --pre mnemocards
+```
+
+You can check that the installation went well by executing the following
+command:
+
+```cmd
+$ mnemocards --version
+╔╦╗╔╗╔╔═╗╔╦╗╔═╗┌─┐┌─┐┬─┐┌┬┐┌─┐
+║║║║║║║╣ ║║║║ ║│  ├─┤├┬┘ ││└─┐
+╩ ╩╝╚╝╚═╝╩ ╩╚═╝└─┘┴ ┴┴└──┴┘└─┘ X.Y.Z
+╭────────────────────────────────╮
+│ <A super mega funny joke here> │
+╰────────────────────────────────╯
+```
+
+If the joke made you laugh you can continue with this tutorial, otherwise this
+program is not for you and you should consider other alternatives.
+
+
+## ❓How it works?
+
+Once you have Mnemocards installed, you can start creating your own flashcards.
+Let's start creating our own vocabulary Anki cards.
+
+Imagine you are learning Spanish and you have a list of vocabulary like this:
+
+English | Spanish |
+--------|---------|
+Hello   | Hola    |
+Bye     | Adiós   |
+
+If you want to use Mnemocards to generate Anki cards for those words the first
+thing you need to do is to create a CSV file like the following:
+
+```csv title="vocabulary.csv"
+your_language_word,language_you_learn_word,id
+Hello,Hola,9a6c9728-7f86-4e3f-9dec-a2f804bd0a76
+Bye,Adiós,e600a85a-8a6b-4449-a188-f7401dc69d6b
+```
+
+A CSV file is a text file that represents a table. The first line is the header
+of the table, after that header line we have one line per row. Each column is
+separated from the other with a column. CSV stands for Comma-Separated Values.
+
+The first column contains the word in your native language, in this case
+English. The second row is the word in the language you are learning, Spanish.
+The last column is a randomly generated ID.
+
+!!! question "Why do we need an ID?"
+
+    IDs are used to uniquely identify a note in Anki. We can use the Spanish
+    word as an ID, but if you start studing a card and you want to make an edit
+    later the card will be considered as a complete new one, loosing your
+    progress.
+
+    For example, imagine you write *Adios* and after several days of study you
+    realise that your miss the accent. If you chage *Adios* to *Adiós* the
+    ID of that note will be different. To avoid this kind of problems I decided
+    to include an ID column.
+
+Mnemocards uses a configuration file named `mnemocards.yaml` to define the
+steps that will be used to process our flashcards. In this file, you can
+specify the tasks that you want to use, the order in which they will be
+executed, and any necessary parameters.
+
+Here is an example of a simple configuration file that reads in a CSV file
+containing vocabulary data, and then generates an Anki APKG package:
+
+```yaml title="mnemocards.yaml"
+steps:
+  # Read a CSV file with our spanish vocabulary.
+  - type: ReadCsv
+    path: vocabulary.csv
+  # Tag the generated notes and assign them to an Anki deck.
+  - type: mnemocards_anki.Configure
+    tags: spanish, languages
+    deck:
+      name: Spanish
+      id: 429d2604-ca8a-4c0a-9b03-38d1df5b9af7
+    note_type: mnemocards_anki.VocabularyNoteType
+  # Pronounce the spanish words using Google Translator.
+  - type: mnemocards_anki.Pronounce
+    language: es
+    attribute_to_pronounce: language_you_learn_word
+  # Save the Anki package.
+  - type: mnemocards_anki.Package
+  # Show the generated tasks in the terminal.
+  # Do not print the note id, the note_type and the deck to avoid cluttering the terminal.
+  - type: Print
+    ignore_regex: id|note_type|deck
+  # Show some stats of the generation process.
+  - type: Stats
+```
+
+You can run the configuration file using the following command:
+
+```cmd
+$ mnemocards run mnemocards.yml
+```
+
+This will execute the steps in the configuration file, and will generate an
+Anki package named `out.apkg` by default. The generated file is in the same
+directory as your `mnemocards.yaml`.
+
+If you import the `apkg` file to Anki you can start studying Spanish:
+
+<img src="https://guiferviz.com/mnemocards/images/hello_hola_note.png"
+     alt="Mnemocards generated vocabulary card"
+     width="400">
+
+
+## 🤓 What is next?
+
+If you have come this far, it is because you may have found this project
+interesting. Consider visiting the
+[documentation](https://guiferviz.com/mnemocards), in particular the
+[examples](https://guiferviz.com/mnemocards/examples) section to learn more.
+
+As mentioned above, Mnemocards is fully extensible, so any data source you miss
+or any processing or analysis you want to do on your cards is more than
+welcome. Feel free to [post your
+idea](https://github.com/guiferviz/mnemocards/discussions/categories/ideas) to
+start a discussion. Do not worry if you do not know how to program, there may
+be someone who can do it for you.
+
+Enjoy learning!!!
 
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,96 +1,111 @@
-# -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
-'src', 'mnemocards_anki': 'src/mnemocards_anki', 'mnemocards_essentials': 'src/
-mnemocards_essentials'} packages = \ ['mnemocards', 'mnemocards_anki',
-'mnemocards_essentials'] package_data = \ {'': ['*']} install_requires = \
-['fire>=0.5.0,<0.6.0', 'pydantic>=1.10.4,<2.0.0', 'pyyaml>=6.0,<7.0',
-'rich>=13.2.0,<14.0.0'] entry_points = \ {'console_scripts': ['mnemocards =
-mnemocards.__main__:main']} setup_kwargs = { 'name': 'mnemocards', 'version':
-'1.0.0a0', 'description': "In addition to helping you memorise, this code helps
-you do other things that I don't remember...", 'long_description': '
-               \n \n_n_alt="Mnemocards_logo"\n_width="200">\n\n
-\n
-\n \n_n_alt="Mnemocards_CI_pipeline_status">\n\n \n_n_alt="Mnemocards_coverage
-      status">\n\n \n_n_alt="Mnemocards_issues">\n\n \n_n_alt="Mnemocards
-      contributors">\n\n \n_n_alt="Mnemocards_total_downloads">\n\n \n_n
-                  alt="Mnemocards_downloads_per_month">\n\n
-  \n In addition to helping you memorise, this code helps you do other things
-                          that I don\'t remember...\n
-\n\n---\n\n:books: **Documentation**:\n\n_https://guiferviz.com/
-mnemocards\n\n\n:keyboard: **Source Code**:\n\n_https://github.com/guiferviz/
-mnemocards\n\n\n---\n\n## ð¤ What is this?\n\n**Mnemocards** is a Python
-package originally intended for creating Anki\nflashcards from text files. It
-allows users to define a series of steps to read\nflashcards from any source,
-transform them and export them to different formats\nsuch as Anki APKG
-packages. Mnemocards is designed to be fully extensible,\nwhich means that
-users can create their own tasks and customize the card\ngeneration process to
-their specific needs.\n\nReading **flashcards from text files** has several
-**advantages** over binary\nformats or manually creating cards in the Anki app.
-Text files are easily\nreadable and editable by humans. This means that users
-can easily understand\nand modify the flashcard content **using common text
-editors**, and also can\nuse version control systems like **Git to track
-changes and collaborate** with\nothers.\n\n\n## ð·ï¸ Features\n\n* Generates
-Anki APKG packages that you can later import into the Anki app.\n* Auto
-generate pronunciations from the words that you are learning.\n* Generates
-flashcards from text files that can be stored in Git repositories.\nThis brings
-several positive things:\n * Keep track of changes.\n * Maintain different
-versions of flashcards using Git branches.\n * Easily share and collaborate
-with others. If you know how to work with\n Git you can create forks and pull
-requests to existing repositories.\n* Fully extensible architecture that allows
-you to define tasks that perform\ncustom transformations on a list of notes.\n
-* Possibility to export flashcards to other existing flashcards apps.\n *
-Create indexes or analyze your collection of cards, create\n visualizations,
-clustering, analyze how the cards relate to each other...\n\n\n## ð¤ How it
-works?\n\nTo get started with Mnemocards, you\'ll need to have Python >= 3.10
-installed on\nyour computer. Then, you can install Mnemocards using `pip`:
-\n\n```cmd\n$ pip install mnemocards\n```\n\nYou can check that the
-installation went well by executing the following\ncommand:\n\n```cmd\n$
-mnemocards --
-version\nââ¦âââââââââ¦âââââââââââ¬ââââ¬ââââ\nââââââââ£
-ââââ ââ âââ¤ââ¬â âââââ\nâ©
-â©âââââââ© â©âââââââ´
-â´â´ââââ´ââââ
-X.Y.Z\nâ­âââââââââââââââââââââââââââââââââ®\nâ
-â\nâ°âââââââââââââââââââââââââââââââââ¯\n```\n\nIf
-the joke made you laugh you can continue with this tutorial, otherwise
-this\nprogram is not for you and you should consider other
-alternatives.\n\nOnce you have Mnemocards installed, you can start creating
-your own flashcards.\nLet\'s start creating our own vocabulary file.\n\nYou can
-use the provided sample files as a starting point, or create your
-own.\nMnemocards uses a configuration file to define the steps that will be
-used to\nprocess the flashcards. In this file, you can specify the tasks that
-you want\nto use, the order in which they will be executed, and any necessary
-parameters\nor settings.\n\nHere\'s an example of a simple configuration file
-that reads in a CSV file containing flashcard data, and then generates an Anki
-APKG package:\n\n```yaml\nsteps:\n - type: ReadFile\n path: flashcards.csv\n -
-type: Anki\n deck:\n name: My Flashcards\n id: b45f6d48-d1ab-4d0e-80a9-
-08a2ab473a41\n note_type:\n type: BasicNoteType\n - type: Package\n```\n\nIn
-this example, the first step reads in a CSV file called "flashcards.csv", the
-second step generates an Anki package with a deck named "My Flashcards" and a
-specific id, and the last step creates the APKG package.\n\nYou can run the
-configuration file using the mnemocards command:\n\nCopy code\nmnemocards run
-my_config.yml\nThis will execute the steps in the configuration file, and
-create the Anki APKG package.\n\nYou can also use the package to export your
-flashcards to other flashcard apps like Quizlet by adding a Quizlet task to the
-configuration file and providing the necessary credentials.\n\nWith Mnemocards,
-you can customize the flashcard generation process to suit your needs and
-easily collaborate with others. Give it a try and see how it can help you learn
-more efficiently!\n\nTODO\n\n\n## ð§ª Examples\n\n\nJapanese Flashcards :jp:
-\nThinks you will learn:\n\n* UnionPipeline task.\n* Audio
-generation.\n\n\n\n## DELETEME: Fast ideas\n\nMnemocards is a tool for
-processing your flashcards.\nMnemocards first appeared with the objective of
-generating Anki APKG packages that you can later import into the Anki
-app.\nMnemocards allow us to generate our cards from text files that we can
-store in repositories.\nHaving text files in repos allow us to keep track of
-the changes, maintain different versions of our flashcards and easily
-collaborate with others (creating forks of existing projects or creating pull
-requests, for example).\nIt is fully extensible, you can define tasks that
-perform transformations on a list of notes.\nYou can also auto generate
-pronunciations from the words that you are learning.\nYou may even export your
-flashcards to other existing flashcards apps.\nThe possibilities are endless,
-you can create an index or somehow analyze your collection of cards, create
-visualizations, clustering, analyze how the cards relate to each other...\n',
-'author': 'guiferviz', 'author_email': 'guiferviz@gmail.com', 'maintainer':
-'None', 'maintainer_email': 'None', 'url': 'https://github.com/guiferviz/
-mnemocards', 'package_dir': package_dir, 'packages': packages, 'package_data':
-package_data, 'install_requires': install_requires, 'entry_points':
-entry_points, 'python_requires': '>=3.10,<4.0', } setup(**setup_kwargs)
+Metadata-Version: 2.1 Name: mnemocards Version: 1.0.0b0 Summary: In addition to
+helping you memorise, this code helps you do other things that I don't
+remember... Home-page: https://github.com/guiferviz/mnemocards License: MIT
+Keywords: mnemocards Author: guiferviz Author-email: guiferviz@gmail.com
+Requires-Python: >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English Classifier: Programming Language ::
+Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 Classifier: Topic :: Software
+Development Requires-Dist: fire (>=0.5.0,<0.6.0) Requires-Dist: gtts
+(>=2.3.1,<3.0.0) Requires-Dist: pydantic (>=1.10.7,<2.0.0) Requires-Dist:
+pyyaml (>=6.0,<7.0) Requires-Dist: rich (>=13.3.4,<14.0.0) Requires-Dist: toml
+(>=0.10.2,<0.11.0) Requires-Dist: xmltodict (>=0.13.0,<0.14.0) Project-URL: Bug
+Tracker, https://github.com/guiferviz/mnemocards/issues Project-URL:
+Documentation, https://guiferviz.github.io/mnemocards Project-URL: Repository,
+https://github.com/guiferviz/mnemocards Project-URL: Source, https://
+github.com/guiferviz/mnemocards Description-Content-Type: text/markdown
+                               [Mnemocards_logo]
+   [Mnemocards_CI_pipeline_status] [Mnemocards_coverage_status] [Mnemocards
+  issues] [Mnemocards_contributors] [Mnemocards_total_downloads] [Mnemocards
+                             downloads_per_month]
+In addition to helping you memorise, this code helps you do other things that I
+                               don't remember...
+--- :books: **Documentation**: https://guiferviz.com/mnemocards :keyboard:
+**Source Code**: https://github.com/guiferviz/mnemocards ---
+                    [Mnemocards_generated_vocabulary_card]
+## ð¤ What is this? **Mnemocards** is a Python package originally intended
+for creating Anki flashcards from text files. It allows users to define a
+series of steps to read flashcards from any source, transform them and export
+them to different formats such as Anki APKG packages. Mnemocards is designed to
+be fully extensible, which means that users can create their own tasks and
+customize the card generation process to their specific needs. Indeed,
+Mnemocards has the versatility to be used for purposes beyond generating Anki
+decks. ## ð·ï¸ Features * **Generate Anki APKG packages** that you can later
+import into the Anki app. * Auto **generate pronunciations** from the words
+that you are learning in any language supported by Google Translator. *
+Generate **flashcards from text files** that can be stored in Git repositories.
+This brings several positive things: * Keep **track of changes**. * Edit cards
+using your **favourite text editor**. I :heart: VIM. * Easily **share and
+collaborate with others**. If you know how to work with Git you can create
+forks and pull requests to existing repositories. * **Fully extensible
+architecture** that allows you to define custom transformations on a list of
+notes. * Possibility to implement another way of exporting flashcards to other
+existing flashcards apps. Contributions are welcome. * Possibility to create
+search indexes, analyze your collection of cards, create visualizations,
+clustering, analyze how the cards relate to each other... Contributions are
+welcome. ## âï¸ Installation To get started with Mnemocards, you'll need to
+have Python >= 3.10 installed on your computer. Then, you can install
+Mnemocards using `pip`: ```cmd $ pip install --pre mnemocards ``` You can check
+that the installation went well by executing the following command: ```cmd $
+mnemocards --version
+ââ¦âââââââââ¦âââââââââââ¬ââââ¬ââââ
+ââââââââ£ ââââ ââ âââ¤ââ¬â âââââ
+â© â©âââââââ© â©âââââââ´
+â´â´ââââ´ââââ X.Y.Z
+â­âââââââââââââââââââââââââââââââââ®
+â â
+â°âââââââââââââââââââââââââââââââââ¯
+``` If the joke made you laugh you can continue with this tutorial, otherwise
+this program is not for you and you should consider other alternatives. ##
+âHow it works? Once you have Mnemocards installed, you can start creating
+your own flashcards. Let's start creating our own vocabulary Anki cards.
+Imagine you are learning Spanish and you have a list of vocabulary like this:
+English | Spanish | --------|---------| Hello | Hola | Bye | AdiÃ³s | If you
+want to use Mnemocards to generate Anki cards for those words the first thing
+you need to do is to create a CSV file like the following: ```csv
+title="vocabulary.csv" your_language_word,language_you_learn_word,id
+Hello,Hola,9a6c9728-7f86-4e3f-9dec-a2f804bd0a76 Bye,AdiÃ³s,e600a85a-8a6b-4449-
+a188-f7401dc69d6b ``` A CSV file is a text file that represents a table. The
+first line is the header of the table, after that header line we have one line
+per row. Each column is separated from the other with a column. CSV stands for
+Comma-Separated Values. The first column contains the word in your native
+language, in this case English. The second row is the word in the language you
+are learning, Spanish. The last column is a randomly generated ID. !!! question
+"Why do we need an ID?" IDs are used to uniquely identify a note in Anki. We
+can use the Spanish word as an ID, but if you start studing a card and you want
+to make an edit later the card will be considered as a complete new one,
+loosing your progress. For example, imagine you write *Adios* and after several
+days of study you realise that your miss the accent. If you chage *Adios* to
+*AdiÃ³s* the ID of that note will be different. To avoid this kind of problems
+I decided to include an ID column. Mnemocards uses a configuration file named
+`mnemocards.yaml` to define the steps that will be used to process our
+flashcards. In this file, you can specify the tasks that you want to use, the
+order in which they will be executed, and any necessary parameters. Here is an
+example of a simple configuration file that reads in a CSV file containing
+vocabulary data, and then generates an Anki APKG package: ```yaml
+title="mnemocards.yaml" steps: # Read a CSV file with our spanish vocabulary. -
+type: ReadCsv path: vocabulary.csv # Tag the generated notes and assign them to
+an Anki deck. - type: mnemocards_anki.Configure tags: spanish, languages deck:
+name: Spanish id: 429d2604-ca8a-4c0a-9b03-38d1df5b9af7 note_type:
+mnemocards_anki.VocabularyNoteType # Pronounce the spanish words using Google
+Translator. - type: mnemocards_anki.Pronounce language: es
+attribute_to_pronounce: language_you_learn_word # Save the Anki package. -
+type: mnemocards_anki.Package # Show the generated tasks in the terminal. # Do
+not print the note id, the note_type and the deck to avoid cluttering the
+terminal. - type: Print ignore_regex: id|note_type|deck # Show some stats of
+the generation process. - type: Stats ``` You can run the configuration file
+using the following command: ```cmd $ mnemocards run mnemocards.yml ``` This
+will execute the steps in the configuration file, and will generate an Anki
+package named `out.apkg` by default. The generated file is in the same
+directory as your `mnemocards.yaml`. If you import the `apkg` file to Anki you
+can start studying Spanish: [Mnemocards generated vocabulary card] ## ð¤ What
+is next? If you have come this far, it is because you may have found this
+project interesting. Consider visiting the [documentation](https://
+guiferviz.com/mnemocards), in particular the [examples](https://guiferviz.com/
+mnemocards/examples) section to learn more. As mentioned above, Mnemocards is
+fully extensible, so any data source you miss or any processing or analysis you
+want to do on your cards is more than welcome. Feel free to [post your idea]
+(https://github.com/guiferviz/mnemocards/discussions/categories/ideas) to start
+a discussion. Do not worry if you do not know how to program, there may be
+someone who can do it for you. Enjoy learning!!!
```

