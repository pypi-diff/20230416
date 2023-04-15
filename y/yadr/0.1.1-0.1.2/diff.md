# Comparing `tmp/yadr-0.1.1.tar.gz` & `tmp/yadr-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yadr-0.1.1.tar", last modified: Sun Jul 31 14:01:56 2022, max compression
+gzip compressed data, was "yadr-0.1.2.tar", last modified: Sat Apr 15 23:19:14 2023, max compression
```

## Comparing `yadr-0.1.1.tar` & `yadr-0.1.2.tar`

### file list

```diff
@@ -1,28 +1,35 @@
-drwxr-xr-x   0 pji        (501) staff       (20)        0 2022-07-31 14:01:56.902325 yadr-0.1.1/
--rw-r--r--   0 pji        (501) staff       (20)     1069 2021-11-15 07:15:50.000000 yadr-0.1.1/LICENSE
--rw-r--r--   0 pji        (501) staff       (20)     4175 2022-07-31 14:01:56.902436 yadr-0.1.1/PKG-INFO
--rw-r--r--   0 pji        (501) staff       (20)     3701 2021-12-01 13:38:32.000000 yadr-0.1.1/README.rst
--rw-r--r--   0 pji        (501) staff       (20)       90 2021-12-01 13:26:36.000000 yadr-0.1.1/pyproject.toml
--rw-r--r--   0 pji        (501) staff       (20)      812 2022-07-31 14:01:56.903034 yadr-0.1.1/setup.cfg
-drwxr-xr-x   0 pji        (501) staff       (20)        0 2022-07-31 14:01:56.900190 yadr-0.1.1/yadr/
--rw-r--r--   0 pji        (501) staff       (20)       93 2022-07-31 14:01:34.000000 yadr-0.1.1/yadr/__init__.py
--rw-r--r--   0 pji        (501) staff       (20)      156 2022-07-31 14:01:34.000000 yadr-0.1.1/yadr/__main__.py
--rw-r--r--   0 pji        (501) staff       (20)    17257 2022-07-31 14:01:34.000000 yadr-0.1.1/yadr/base.py
-drwxr-xr-x   0 pji        (501) staff       (20)        0 2022-07-31 14:01:56.900664 yadr-0.1.1/yadr/data/
--rw-r--r--   0 pji        (501) staff       (20)        0 2022-07-30 15:19:28.000000 yadr-0.1.1/yadr/data/__init__.py
--rw-r--r--   0 pji        (501) staff       (20)      904 2021-11-30 13:16:10.000000 yadr-0.1.1/yadr/data/dice_maps.yadn
--rw-r--r--   0 pji        (501) staff       (20)     1630 2022-07-31 14:01:34.000000 yadr-0.1.1/yadr/encode.py
--rw-r--r--   0 pji        (501) staff       (20)    11656 2022-07-31 14:01:34.000000 yadr-0.1.1/yadr/lex.py
--rw-r--r--   0 pji        (501) staff       (20)     7207 2022-07-31 14:01:34.000000 yadr-0.1.1/yadr/maps.py
--rw-r--r--   0 pji        (501) staff       (20)     3682 2022-07-31 14:01:34.000000 yadr-0.1.1/yadr/model.py
--rw-r--r--   0 pji        (501) staff       (20)     6366 2022-07-31 14:01:34.000000 yadr-0.1.1/yadr/operator.py
--rw-r--r--   0 pji        (501) staff       (20)     9273 2022-07-31 14:01:34.000000 yadr-0.1.1/yadr/parser.py
--rw-r--r--   0 pji        (501) staff       (20)     3444 2022-07-31 14:01:34.000000 yadr-0.1.1/yadr/pools.py
--rw-r--r--   0 pji        (501) staff       (20)        0 2022-07-31 13:18:36.000000 yadr-0.1.1/yadr/py.typed
--rw-r--r--   0 pji        (501) staff       (20)     4682 2022-07-31 14:01:34.000000 yadr-0.1.1/yadr/yadr.py
-drwxr-xr-x   0 pji        (501) staff       (20)        0 2022-07-31 14:01:56.902083 yadr-0.1.1/yadr.egg-info/
--rw-r--r--   0 pji        (501) staff       (20)     4175 2022-07-31 14:01:56.000000 yadr-0.1.1/yadr.egg-info/PKG-INFO
--rw-r--r--   0 pji        (501) staff       (20)      431 2022-07-31 14:01:56.000000 yadr-0.1.1/yadr.egg-info/SOURCES.txt
--rw-r--r--   0 pji        (501) staff       (20)        1 2022-07-31 14:01:56.000000 yadr-0.1.1/yadr.egg-info/dependency_links.txt
--rw-r--r--   0 pji        (501) staff       (20)        1 2021-12-01 13:47:53.000000 yadr-0.1.1/yadr.egg-info/not-zip-safe
--rw-r--r--   0 pji        (501) staff       (20)        5 2022-07-31 14:01:56.000000 yadr-0.1.1/yadr.egg-info/top_level.txt
+drwxr-xr-x   0 pji        (501) staff       (20)        0 2023-04-15 23:19:14.911226 yadr-0.1.2/
+-rw-r--r--   0 pji        (501) staff       (20)     1069 2021-11-15 07:15:50.000000 yadr-0.1.2/LICENSE
+-rw-r--r--   0 pji        (501) staff       (20)     4177 2023-04-15 23:19:14.911427 yadr-0.1.2/PKG-INFO
+-rw-r--r--   0 pji        (501) staff       (20)     3703 2023-04-12 13:04:13.000000 yadr-0.1.2/README.rst
+-rw-r--r--   0 pji        (501) staff       (20)       90 2021-12-01 13:26:36.000000 yadr-0.1.2/pyproject.toml
+-rw-r--r--   0 pji        (501) staff       (20)      812 2023-04-15 23:19:14.912532 yadr-0.1.2/setup.cfg
+drwxr-xr-x   0 pji        (501) staff       (20)        0 2023-04-15 23:19:14.903863 yadr-0.1.2/tests/
+-rw-r--r--   0 pji        (501) staff       (20)     1524 2023-04-15 22:46:13.000000 yadr-0.1.2/tests/test_encoder.py
+-rw-r--r--   0 pji        (501) staff       (20)    26052 2023-04-15 22:46:13.000000 yadr-0.1.2/tests/test_lex.py
+-rw-r--r--   0 pji        (501) staff       (20)     8452 2023-04-15 22:46:13.000000 yadr-0.1.2/tests/test_maps.py
+-rw-r--r--   0 pji        (501) staff       (20)    10646 2023-04-15 22:46:13.000000 yadr-0.1.2/tests/test_operator.py
+-rw-r--r--   0 pji        (501) staff       (20)    19434 2023-04-15 22:46:13.000000 yadr-0.1.2/tests/test_parser.py
+-rw-r--r--   0 pji        (501) staff       (20)     3717 2023-04-15 22:46:13.000000 yadr-0.1.2/tests/test_yadr.py
+drwxr-xr-x   0 pji        (501) staff       (20)        0 2023-04-15 23:19:14.899067 yadr-0.1.2/yadr/
+-rw-r--r--   0 pji        (501) staff       (20)      128 2023-04-15 22:46:13.000000 yadr-0.1.2/yadr/__init__.py
+-rw-r--r--   0 pji        (501) staff       (20)      163 2023-04-15 22:46:13.000000 yadr-0.1.2/yadr/__main__.py
+-rw-r--r--   0 pji        (501) staff       (20)    17602 2023-04-15 22:46:13.000000 yadr-0.1.2/yadr/base.py
+drwxr-xr-x   0 pji        (501) staff       (20)        0 2023-04-15 23:19:14.899588 yadr-0.1.2/yadr/data/
+-rw-r--r--   0 pji        (501) staff       (20)        0 2022-07-30 15:19:28.000000 yadr-0.1.2/yadr/data/__init__.py
+-rw-r--r--   0 pji        (501) staff       (20)      904 2021-11-30 13:16:10.000000 yadr-0.1.2/yadr/data/dice_maps.yadn
+-rw-r--r--   0 pji        (501) staff       (20)     1688 2023-04-15 22:46:13.000000 yadr-0.1.2/yadr/encode.py
+-rw-r--r--   0 pji        (501) staff       (20)    11664 2023-04-15 22:46:13.000000 yadr-0.1.2/yadr/lex.py
+-rw-r--r--   0 pji        (501) staff       (20)     7743 2023-04-15 22:46:13.000000 yadr-0.1.2/yadr/maps.py
+-rw-r--r--   0 pji        (501) staff       (20)     3586 2023-04-15 22:46:13.000000 yadr-0.1.2/yadr/model.py
+-rw-r--r--   0 pji        (501) staff       (20)     6784 2023-04-15 22:46:13.000000 yadr-0.1.2/yadr/operator.py
+-rw-r--r--   0 pji        (501) staff       (20)    13348 2023-04-15 22:46:13.000000 yadr-0.1.2/yadr/parser.py
+-rw-r--r--   0 pji        (501) staff       (20)     3587 2023-04-15 22:46:13.000000 yadr-0.1.2/yadr/pools.py
+-rw-r--r--   0 pji        (501) staff       (20)        0 2022-07-31 13:18:36.000000 yadr-0.1.2/yadr/py.typed
+-rw-r--r--   0 pji        (501) staff       (20)     5460 2023-04-15 22:46:13.000000 yadr-0.1.2/yadr/yadr.py
+drwxr-xr-x   0 pji        (501) staff       (20)        0 2023-04-15 23:19:14.910709 yadr-0.1.2/yadr.egg-info/
+-rw-r--r--   0 pji        (501) staff       (20)     4177 2023-04-15 23:19:14.000000 yadr-0.1.2/yadr.egg-info/PKG-INFO
+-rw-r--r--   0 pji        (501) staff       (20)      553 2023-04-15 23:19:14.000000 yadr-0.1.2/yadr.egg-info/SOURCES.txt
+-rw-r--r--   0 pji        (501) staff       (20)        1 2023-04-15 23:19:14.000000 yadr-0.1.2/yadr.egg-info/dependency_links.txt
+-rw-r--r--   0 pji        (501) staff       (20)        1 2023-04-15 23:19:14.000000 yadr-0.1.2/yadr.egg-info/not-zip-safe
+-rw-r--r--   0 pji        (501) staff       (20)        5 2023-04-15 23:19:14.000000 yadr-0.1.2/yadr.egg-info/top_level.txt
```

### Comparing `yadr-0.1.1/LICENSE` & `yadr-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yadr-0.1.1/PKG-INFO` & `yadr-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yadr
-Version: 0.1.1
+Version: 0.1.2
 Summary: Yet another dice roller for Python.
 Home-page: https://github.com/pji/yadr
 Author: Paul J. Iutzi
 Author-email: pji@mac.com
 Project-URL: Bug Tracker, https://github.com/pji/yadr/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
@@ -36,15 +36,15 @@
 past when looking into algorithms, and it seemed like writing a
 parser to handle different dice systems seemed a reasonable way to go.
 As reasonable as any thought involving, "I'll use BNF here," can be,
 I guess. And so was born Yet Another Dice Notation (YADN) and `yadr`.
 
 For a description of YADN see: YADN_
 
-.. _YADN: https://github.com/pji/yadr/blob/main/docs/dice_notation.rst
+.. _YADN: https://github.com/pji/yadr/docs/build/html/dice_notation.html
 
 
 Do we need another Python dice rolling package?
 ===============================================
 No. Probably not. Unsurprisingly, there seems to be a lot of people who
 play TTRPGs and write Python packages. This is yet another one.
```

### Comparing `yadr-0.1.1/README.rst` & `yadr-0.1.2/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 past when looking into algorithms, and it seemed like writing a
 parser to handle different dice systems seemed a reasonable way to go.
 As reasonable as any thought involving, "I'll use BNF here," can be,
 I guess. And so was born Yet Another Dice Notation (YADN) and `yadr`.
 
 For a description of YADN see: YADN_
 
-.. _YADN: https://github.com/pji/yadr/blob/main/docs/dice_notation.rst
+.. _YADN: https://github.com/pji/yadr/docs/build/html/dice_notation.html
 
 
 Do we need another Python dice rolling package?
 ===============================================
 No. Probably not. Unsurprisingly, there seems to be a lot of people who
 play TTRPGs and write Python packages. This is yet another one.
```

### Comparing `yadr-0.1.1/setup.cfg` & `yadr-0.1.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 	tests/*
 rst_files = *
 	docs/*
 unit_tests = tests
 
 [metadata]
 name = yadr
-version = 0.1.1
+version = 0.1.2
 author = Paul J. Iutzi
 author_email = pji@mac.com
 description = Yet another dice roller for Python.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/pji/yadr
 project_urls =
```

### Comparing `yadr-0.1.1/yadr/base.py` & `yadr-0.1.2/yadr/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,44 +1,72 @@
 """
 base
 ~~~~
 
-Base classes for the yadr package.
+Base classes for the :mod:`yadr` package.
 """
 from abc import ABC, abstractmethod
-from typing import Callable, Optional
+from collections.abc import Callable
+from typing import Optional
 
 from yadr.model import CompoundResult, Result, Token, TokenInfo
 
 
+# Types
+ResultMethod = Callable[[str], Result]
+StateMethod = Callable[[str], None]
+
+
 # Utility functions.
 def _mutable(value, type_=list):
     """Return an empty mutable type to avoid bugs where you put a
     mutable in the signature.
     """
     if not value:
         value = type_()
     return value
 
 
 # Base classes.
 class BaseLexer(ABC):
     """An abstract base class for building lexers.
 
-    :class:BaseLexer lexers are state machines used for translating
-    a text string into tokens for parsing. It accomplishes this by
-    processing the string one character at a time, allowing the
+    :param state_map: A dictionary mapping the state of the lexer
+        to the processing method for that state.
+    :param symbol_map: A dictionary mapping states of the lexer to
+        characters that could occur within the text being lexed.
+    :param bracket_states: (Optional.) A dictionary mapping opening
+        or delimiting states to a state that collects characters
+        within the brackets or delimiters to send to a more
+        specific lexer.
+    :param bracket_ends: (Optional.) A dictionary mapping bracket
+        states to a state that processes characters after the end
+        of the bracket state.
+    :param result_map: (Optional.) A dictionary mapping states
+        to a result transformation method to transform the data
+        in the lexed string before storing it in as a token
+        value.
+    :param no_store: (Optional.) A list of states that should not
+        be stored as tokens.
+    :param init_state: (Optional.) The initial state of the lexer.
+        It defaults to :class:`Token.START`.
+    :return: None.
+    :rtype: NoneType
+
+    :class:`yadr.base.BaseLexer` lexers are state machines used for
+    translating a text string into tokens for parsing. It accomplishes
+    this by processing the string one character at a time, allowing the
     current state of the lexer to determine whether the character is
     legal and what should be done with it.
 
 
     State
     -----
     The current state of the lexer is determined by the value of
-    the `state` attribute of the lexer. Its value will be a member
+    :attr:`yadr.base.BaseLexer.state`. Its value will be a member
     of the enumeration used to define the tokens that exist within
     the language. This state is used to define the rule used to
     process the next character in the string.
 
     Characters that do not cause the state of the lexer to change
     should be appended to the end of the `buffer` attribute of
     the lexer.
@@ -48,32 +76,32 @@
     ------------
     When the lexer encounters a character that represents the end of
     the previous token and the start of a new token, the state of
     the lexer changes. The specific details can vary based on the
     current state of the lexer, but by default the following occurs
     when the state is changed:
 
-    *   A new TokenInfo object is created that contains the current
-        state of the lexer and the current value of the `buffer`
+    *   A new :class:`model.TokenInfo` object is created that contains
+        the current state of the lexer and the current value of the
+        `buffer` attribute of the lexer.
+    *   That :class:`model.TokenInfo` object is appended to the `tokens`
         attribute of the lexer.
-    *   That TokenInfo object is appended to the `tokens` attribute
-        of the lexer.
     *   The `buffer` of the lexer is cleared.
     *   The `state` of the lexer is changed to the new state.
-    *   The `process()` method is changed to the process method for
-        the new state.
+    *   The :meth:`BaseLexer.process` method is changed to the process
+        method for the new state.
 
 
-    `BaseLexer.process()` and Processing Methods
-    --------------------------------------------
-    The `process()` method of a BaseLexer subclass should not be
-    defined. Instead the name should be assigned to a "processing"
-    method specific to the current state of the lexer. By
-    convention, the names of these method starts with an
-    underscore, which is followed by the name of the state in
+    :meth:`BaseLexer.process()` and Processing Methods
+    --------------------------------------------------
+    The :meth:`BaseLexer.process` method of a :class:`BaseLexer`
+    subclass should not be defined. Instead the name should be
+    assigned to a "processing" method specific to the current state
+    of the lexer. By convention, the names of these method starts
+    with an underscore, which is followed by the name of the state in
     lowercase letters. So the processing method for the state::
 
         Token.GROUP_OPEN
 
     would be::
 
         _group_open
@@ -85,33 +113,33 @@
     where `char` is the character being processed.
 
     While specific tokens may require different behavior, in general
     a processing method does two things:
 
     *   Define a list of states that are allowed to follow the
         current state within the syntax being lexed.
-    *   pass that list and the character to the internal `_check_char()`
-        method that handles the actual processing.
+    *   Pass that list and the character to :meth:`BaseLexer._check_char`,
+        which handles the actual processing.
 
     The end result of calling a processing method is usually that
     the characters in the string that make up the symbol for the
-    current state are stored in a "TokenInfo" tuple, which consists
-    of the token representing the state and the characters of the
-    symbol. These tokens will then be used by the parser to
+    current state are stored in a "TokenInfo" :class:`tuple`, which
+    consists of the token representing the state and the characters of
+    the symbol. These tokens will then be used by the parser to
     execute the command contained in the string.
 
 
     The State Map
     -------------
     To determine the correct processing method to use for a state, the
     lexer needs to have a mapping that defines the method for the state.
     This dictionary is the "state map." The tokens for the state are
     the keys, and the processing method for that state is the value
-    for the key. This dictionary is passed into the BaseLexer as the
-    `state_map` parameter when the lexer is initialized.
+    for the key. This dictionary is passed into the :class:`BaseLexer`
+    as the `state_map` parameter when the lexer is initialized.
 
 
     The Symbol Map
     --------------
     A BaseLexer uses a "symbol map" to associate characters in the
     string to a state. The symbol map is a dictionary. The keys are
     the tokens from the enumeration that defines state. The values
@@ -126,16 +154,17 @@
 
     The symbol map is passed to the `symbol_map` parameter when the
     lexer is initialized.
 
 
     Bracketing
     ----------
-    Instead of running each character through `_check_char()`, it is
-    possible for a processing method to instead "bracket" characters
+    Instead of running each character through
+    :class:`BaseLexer._check_char`, it is possible
+    for a processing method to instead "bracket" characters
     until a specific character is reached. For example, characters
     after a quotation mark can be collected as a substring until
     the lexer hits another quotation mark.
 
     Why do this? The main use for this is to turn the bracketed
     substring into a single token, rather than three tokens: the
     opening bracket/delimiter, the content of the bracket, and the
@@ -237,16 +266,16 @@
         >>> no_store = [
         >>>     Token.QUALIFIER_END,
         >>> ]
 
 
     Result Transformations
     ----------------------
-    By default, a BaseLexer stores the symbols for the token as a
-    string in the TokenInfo. This behavior can be changed with a
+    By default, a :class:`BaseLexer` stores the symbols for the token
+    as a string in the TokenInfo. This behavior can be changed with a
     "result transformation" method. By convention the name of a
     result transformation starts with an underscore, the letters "tf",
     an underscore, and the name of the state they affect in all lower
     case. So the name of a result transformation method for the
     `Token.NUMBER` state would be::
 
         _tf_number
@@ -266,88 +295,70 @@
     bracketed symbols to a different lexer and parser to allow syntax
     nesting.
 
 
     Result Map
     ----------
     In order to link the result transformation methods to a state,
-    a BaseLexer needs a "result map". The result map is a dictionary.
-    The keys are the states where the transforms are used. The values
-    are the result transformation methods to use for that state. For
-    example, the result map for a lexer that transforms numbers and
-    qualifiers might look like::
+    a :class:`BaseLexer` needs a "result map". The result map is a
+    dictionary. The keys are the states where the transforms are used.
+    The values are the result transformation methods to use for that
+    state. For example, the result map for a lexer that transforms
+    numbers and qualifiers might look like::
 
         >>> result_map = {
         >>>     Token.NUMBER: _tf_number,
         >>>     Token.QUALIFIER: _qualifier,
         >>> }
 
     The result map is passed to the `result_map` parameter when the
-    BaseLexer is initialized.
+    :class:`BaseLexer` is initialized.
     """
     def __init__(self,
-                 state_map: dict[Token, Callable],
+                 state_map: dict[Token, StateMethod],
                  symbol_map: dict[Token, list[str]],
                  bracket_states: Optional[dict[Token, Token]] = None,
                  bracket_ends: Optional[dict[Token, Token]] = None,
-                 result_map: Optional[dict[Token, Callable]] = None,
+                 result_map: Optional[dict[Token, ResultMethod]] = None,
                  no_store: Optional[list[Token]] = None,
                  init_state: Token = Token.START) -> None:
-        """Initialize an instance of :class:Lexer.
-
-        :param state_map: A dictionary mapping the state of the lexer
-            to the processing method for that state.
-        :param symbol_map: A dictionary mapping states of the lexer to
-            characters that could occur within the text being lexed.
-        :param bracket_states: (Optional.) A dictionary mapping opening
-            or delimiting states to a state that collects characters
-            within the brackets or delimiters to send to a more
-            specific lexer.
-        :param bracket_ends: (Optional.) A dictionary mapping bracket
-            states to a state that processes characters after the end
-            of the bracket state.
-        :param result_map: (Optional.) A dictionary mapping states
-            to a result transformation method to transform the data
-            in the lexed string before storing it in as a token
-            value.
-        :param no_store: (Optional.) A list of states that should not
-            be stored as tokens.
-        :param init_state: (Optional.) The initial state of the lexer.
-            It defaults to :class:Token.START.
-        :return: None.
-        :rtype: NoneType
-        """
+        """Initialize an instance of :class:`BaseLexer`."""
+        # Assign the passed parameters.
         self.state_map = state_map
         self.symbol_map = symbol_map
         self.bracket_states = _mutable(bracket_states, dict)
         self.bracket_ends = _mutable(bracket_ends, dict)
         self.result_map = _mutable(result_map, dict)
         self.no_store = _mutable(no_store)
         self.init_state = init_state
-        self.state = init_state
 
-        self.process = self._start
+        # Assign internal attributes.
+        self.state = init_state
+        self.process: StateMethod = self._start
         self.buffer = ''
         self.tokens: list[TokenInfo] = []
 
     # Public methods.
-    def lex(self, yadn: str) -> tuple[TokenInfo, ...]:
-        """Lex a dice notation string.
+    def lex(self, code: str) -> tuple[TokenInfo, ...]:
+        """Lex code into tokens for parsing.
 
-        :param yadn: A string of YADN representing a die roll. For
-            details on YADN, see here: YADN_
-        :return: A :class:tuple object.
+        :param code: A string of code to tranform into tokens.
+        :return: A :class:`tuple` object.
         :rtype: tuple
-
-        .. _YADN: https://github.com/pji/yadr/blob/main/docs/dice_notation.rst
         """
-        for char in yadn:
+        # Process each character in the code.
+        for char in code:
             self.process(char)
+
+        # Reset the lexer after processing the string in case the lexer
+        # is reused.
         else:
             self._change_state(self.init_state, '')
+
+        # Return the tokens from the code.
         return tuple(self.tokens)
 
     # Private operation method.
     def _is_token_start(self, token: Token, char: str) -> bool:
         """Is the given character the start of a new token."""
         valid = {s[0] for s in self.symbol_map[token]}
         return char in valid
```

### Comparing `yadr-0.1.1/yadr/data/dice_maps.yadn` & `yadr-0.1.2/yadr/data/dice_maps.yadn`

 * *Files identical despite different names*

### Comparing `yadr-0.1.1/yadr/encode.py` & `yadr-0.1.2/yadr/encode.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,26 +8,28 @@
 
 
 class Encoder:
     def __init__(self, yadn: str = '') -> None:
         self.yadn = yadn
 
     # Public methods.
-    def encode(self, data: Result | CompoundResult) -> str:
+    def encode(self, data: None | Result | CompoundResult) -> str:
         """Turn computed Python object results into a YADN string."""
         if isinstance(data, bool):
             self._encode_bool(data)
         elif isinstance(data, int):
             self._encode_int(data)
         elif isinstance(data, str):
             self._encode_str(data)
         elif isinstance(data, CompoundResult):
             self._encode_compound_result(data)
         elif isinstance(data, tuple):
             self._encode_tuple(data)
+        else:
+            self.yadn = 'No result.'
         return self.yadn
 
     # Private methods.
     def _encode_bool(self, data: bool) -> None:
         if data:
             self.yadn = f'{self.yadn}T'
         else:
```

### Comparing `yadr-0.1.1/yadr/lex.py` & `yadr-0.1.2/yadr/lex.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 """
 lex
 ~~~
 
 A lexer for `yadr` dice notation.
 """
-from functools import wraps
-from typing import Callable, Optional
+from typing import Optional
 
 from yadr import maps
 from yadr import pools
-from yadr.base import BaseLexer
+from yadr.base import BaseLexer, ResultMethod, StateMethod
 from yadr.model import (
     CompoundResult,
     Result,
     Token,
     TokenInfo,
     symbols
 )
 
 
 # Lexers.
 class Lexer(BaseLexer):
-    """A state-machine to lex dice notation."""
+    """A state-machine to lex :ref:`YADN` dice notation."""
     def __init__(self) -> None:
-        state_map: dict[Token, Callable] = {
+        state_map: dict[Token, StateMethod] = {
             Token.START: self._start,
             Token.AS_OPERATOR: self._as_operator,
             Token.BOOLEAN: self._boolean,
             Token.CHOICE_OPERATOR: self._choice_operator,
             Token.COMPARISON_OPERATOR: self._comparison_operator,
             Token.DICE_OPERATOR: self._dice_operator,
             Token.EX_OPERATOR: self._ex_operator,
@@ -59,15 +58,15 @@
         }
         bracket_ends: dict[Token, Token] = {
             Token.MAP: Token.MAP_END,
             Token.QUALIFIER: Token.QUALIFIER_END,
             Token.POOL: Token.POOL_END,
         }
         symbol_map: dict[Token, list[str]] = symbols
-        result_map: dict[Token, Callable] = {
+        result_map: dict[Token, ResultMethod] = {
             Token.BOOLEAN: self._tf_boolean,
             Token.MAP: self._tf_maps,
             Token.NUMBER: self._tf_number,
             Token.POOL: self._tf_pool,
             Token.QUALIFIER: self._tf_qualifier,
         }
         no_store: list[Token] = [
```

### Comparing `yadr-0.1.1/yadr/maps.py` & `yadr-0.1.2/yadr/maps.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """
 maps
 ~~~~
 
-A module for handling YADN dice maps.
+A module for handling :ref:`YADN` dice maps.
 """
 from typing import Callable, Optional
 
-from yadr.base import BaseLexer
+from yadr.base import BaseLexer, _mutable
 from yadr.model import NamedMap, Result, symbols, Token, TokenInfo
 
 
 # Lexing.
 class Lexer(BaseLexer):
+    """A state machine to lex dice maps in :ref:`YADN` dice notation."""
     def __init__(self) -> None:
         state_map: dict[Token, Callable] = {
             Token.START: self._start,
             Token.END: self._start,
             Token.KV_DELIMITER: self._kv_delimiter,
             Token.MAP_CLOSE: self._map_close,
             Token.MAP_OPEN: self._map_open,
@@ -156,29 +157,36 @@
             Token.WHITESPACE,
         ]
         self._check_char(char, can_follow)
 
 
 # Parsing.
 class Parser:
-    def __init__(self):
-        self.name = ''
-        self.pairs = []
+    """A state machine for parsing :ref:`YADN` dice maps."""
+    def __init__(self) -> None:
+        self.name: str = ''
+        self.pairs: list[tuple[int, str | int]] = []
         self.buffer: Optional[int] = None
         self.state = Token.START
         self.state_map = {
             Token.START: self._start,
             Token.END: self._start,
             Token.KEY: self._key,
             Token.NAME: self._name,
             Token.VALUE: self._value,
         }
 
     def parse(self, tokens: tuple[TokenInfo, ...]) -> NamedMap:
-        """Parse YADN dice mapping tokens."""
+        """Parse YADN dice mapping tokens.
+
+        :param tokens: A dice map as a sequence of :ref:`YADN` tokens
+            to parse.
+        :return: A class defined in :class:`yadr.model.NamedMap`.
+        :rtype: tuple
+        """
         for token_info in tokens:
             process = self.state_map[self.state]
             process(token_info)
         return (self.name, {k: v for k, v in self.pairs})
 
     # Parsing rules.
     def _key(self, token_info: tuple[Token, Result]) -> None:
@@ -191,28 +199,33 @@
             ...
         else:
             msg = f'KEY cannot contain {token.name}.'
             raise ValueError(msg)
 
     def _name(self, token_info: tuple[Token, Result]) -> None:
         token, value = token_info
-        if token == Token.QUALIFIER:
+        if token == Token.QUALIFIER and isinstance(value, str):
             self.name = value
         elif token == Token.NAME_DELIMITER:
             self.state = Token.KEY
         elif token == Token.MAP_CLOSE:
             ...
         else:
             msg = f'NAME cannot contain {token.name}.'
             raise ValueError(msg)
 
     def _value(self, token_info: tuple[Token, Result]) -> None:
         token, value = token_info
-        if (token == Token.QUALIFIER
-                or token == Token.NUMBER and isinstance(value, int)):
+        if (
+            isinstance(self.buffer, int)
+            and (
+                token == Token.QUALIFIER and isinstance(value, str)
+                or token == Token.NUMBER and isinstance(value, int)
+            )
+        ):
             key = self.buffer
             pair = (key, value)
             self.pairs.append(pair)
             self.buffer = None
         elif token == Token.PAIR_DELIMITER:
             self.state = Token.KEY
         elif token == Token.MAP_CLOSE:
```

### Comparing `yadr-0.1.1/yadr/model.py` & `yadr-0.1.2/yadr/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """
 model
 ~~~~~
 
 Common data elements for the yadr package.
 """
-from collections import UserString
-from enum import Enum, EnumMeta, auto
-from typing import Generic, NamedTuple, Sequence, Union, Tuple, TypeVar
+from enum import Enum, auto
+from typing import Union
 
 
 # YADN Tokens.
 class Token(Enum):
     START = auto()
     END = auto()
     AS_OPERATOR = auto()
@@ -123,29 +122,28 @@
     Token.U_POOL_DEGEN_OPERATOR: 'C N S',
     Token.VALUE: '',
     Token.WHITESPACE: '',
 }
 
 
 # Classes.
-class CompoundResult(Tuple):
+class CompoundResult(tuple):
     """The result of multiple rolls."""
 
 
 # Types.
 DiceMapping = dict[int, Union[int, str]]
-NamedMap = Tuple[str, DiceMapping]
-Pool = Tuple[int]
+NamedMap = tuple[str, DiceMapping]
+Pool = tuple[int, ...]
 Result = Union[
     int,
     bool,
     str,
     Pool,
     NamedMap,
-    None
 ]
 TokenInfo = tuple[Token, Result]
 
 
 # Symbols by token.
 symbols = {k: v.split() for k, v in yadn_symbols_raw.items()}
 symbols[Token.WHITESPACE] = [' ', '\t', '\n']
```

### Comparing `yadr-0.1.1/yadr/operator.py` & `yadr-0.1.2/yadr/operator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,27 @@
 """
 operator
 ~~~~~~~~
 
 Operators for handling the dice part of dice notation.
 """
+from collections.abc import Callable, Sequence
 import random
 import operator
-from typing import Sequence
+
+
+# Types for annotation.
+OptionsOp = Callable[[str, str], tuple[str, str]]
+ChoiceOp = Callable[[bool, tuple[str, str]], str]
+PoolGenOp = Callable[[int, int], tuple[int, ...]]
+DiceOp = Callable[[int, int], int]
+MathOp = Callable[[int, int], int]
+PoolOp = Callable[[Sequence[int], int], tuple[int, ...]]
+PoolDegenOp = Callable[[Sequence[int], int], int]
+UPoolDegenOp = Callable[[Sequence[int]], int]
 
 
 # Choice operators.
 def choice_options(a: str, b: str) -> tuple[str, str]:
     """Create the options for a choice."""
     return (a, b)
```

### Comparing `yadr-0.1.1/yadr/pools.py` & `yadr-0.1.2/yadr/pools.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """
 pools
 ~~~~~
 
-A module for handling YADN pools.
+A module for handling :ref:`YADN` pools.
 """
 from typing import Callable, Sequence
 
 from yadr.base import BaseLexer
 from yadr.model import symbols, Token, TokenInfo
 
 
 class Lexer(BaseLexer):
+    """A state machine to lex dice pools in :ref:`YADN` dice notation."""
     def __init__(self) -> None:
         state_map: dict[Token, Callable] = {
             Token.NUMBER: self._number,
             Token.MEMBER_DELIMITER: self._member_delimiter,
             Token.POOL: self._pool,
             Token.POOL_CLOSE: self._pool_close,
             Token.START: self._start,
@@ -98,14 +99,15 @@
         can_follow = [
             Token.POOL_OPEN,
         ]
         self._check_char(char, can_follow)
 
 
 class Parser:
+    """A state machine for parsing :ref:`YADN` dice pools."""
     def parse(self, tokens: Sequence[TokenInfo]) -> tuple[int, ...]:
         """Parse YADN pool tokens."""
         values = []
         for token in tokens:
             kind, value = token
             if kind == Token.NUMBER and isinstance(value, int):
                 values.append(value)
```

### Comparing `yadr-0.1.1/yadr/yadr.py` & `yadr-0.1.2/yadr/yadr.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,73 +1,75 @@
 """
 yadr
 ~~~~
 
-The core of the yadn package.
+The core of the :mod:`yadr` package.
 """
 from argparse import ArgumentParser
 from importlib.resources import open_text
 from pathlib import Path
 from typing import Optional
 
 from yadr import maps as m
 from yadr.encode import Encoder
 from yadr.lex import Lexer
-from yadr.model import CompoundResult, Result, TokenInfo
+from yadr.model import CompoundResult, DiceMapping, Result, TokenInfo
 from yadr.parser import dice_map, Parser
 
 
 # Execute YADN.
-def roll(yadn: str,
-         yadn_out: bool = False,
-         dice_map: Optional[dict[str, dict]] = None
-         ) -> str | Result | CompoundResult:
-    """Execute a string of YADN to roll dice.
+def roll(
+    yadn: str,
+    yadn_out: bool = False,
+    dice_map: Optional[dict[str, DiceMapping]] = None
+) -> None | Result | CompoundResult:
+    """Execute a string of :ref:`YADN` to roll dice.
 
-    :param yadn: A string of YADN that defines the die roll to execute.
-        YADN is described here: YADN_
+    :param yadn: A string of :ref:`YADN` that defines the die roll to
+        execute.
     :param yadn_out: (Optional.) Whether the output should be in native
-        Python objects or YADN notation. The default is native Python
-        objects.
-    :return: The result depends on the details of the die roll, but
-        could be a :class:int, :class:tuple, or :class:str object.
-    :rtype: int or tuple or str
-
-    .. _YADN: https://github.com/pji/yadr/blob/main/docs/dice_notation.rst
+        Python objects or :ref:`YADN` notation. The default is native
+        Python objects.
+    :param dice_map: (Optional.) A dictionary of maps for transforming
+        the value rolled. See :ref:`dice_maps` for details.
+    :return: The result depends on the details of the die roll.
+    :rtype: None, Result, or CompoundResult
 
     Usage::
 
         >>> import yadr
         >>>
         >>> yadr.roll('3d6')                        # doctest: +SKIP
         16
 
-    The specific result will depend on the YADN being executed. In the
-    example above, it will be an integer in the range of three to
+    The specific result will depend on the :ref:`YADN` being executed.
+    In the example above, it will be an integer in the range of three to
     eighteen that is created by generating three random integers in the
     range of one to six.
     """
-    def roll_dice(yadn: str,
-                  dice_map: dict,
-                  yadn_out: bool) -> str | Result | CompoundResult:
-        lexer = Lexer()
-        tokens = lexer.lex(yadn)
-        parser = Parser()
-        parser.dice_map = dice_map
-        result: Result | CompoundResult = parser.parse(tokens)
-        if yadn_out:
-            encoder = Encoder()
-            result = encoder.encode(result)
-        return result
-
+    # Get the default dice maps and add any passed into the roll.
     if not dice_map:
         dice_map = {}
     default_maps = get_default_maps()
     default_maps.update(dice_map)
-    return roll_dice(yadn, default_maps, yadn_out)
+
+    # Lex the YADN into tokens for parsing.
+    lexer = Lexer()
+    tokens = lexer.lex(yadn)
+
+    # Parse and execute the YADN tokens.
+    parser = Parser()
+    parser.dice_map = default_maps
+    result: None | Result | CompoundResult = parser.parse(tokens)
+
+    # If needed, encode the result into YADN and return the result.
+    if yadn_out:
+        encoder = Encoder()
+        result = encoder.encode(result)
+    return result
 
 
 # Utility.
 def read_file(loc: str | Path) -> str:
     """Read test from a file.
 
     :param loc: The file system location of the file.
@@ -76,56 +78,84 @@
     """
     path = Path(loc)
     with open(path) as fh:
         contents = fh.read()
     return contents
 
 
-def parse_map(yadn: str) -> dict[str, dict]:
+def parse_map(yadn: str) -> dict[str, DiceMapping]:
     """Parse the contents of a dice mapping file."""
     if ';' in yadn:
         yadn_parts = yadn.split(';')
         dice_map = {}
         for part in yadn_parts:
-            assert(';' not in part)
+            assert ';' not in part
             dice_map.update(parse_map(part))
         return dice_map
 
     mlexer = m.Lexer()
     mparser = m.Parser()
     tokens = mlexer.lex(yadn)
     name, value = mparser.parse(tokens)
     return {name: value, }
 
 
 # Command parsing.
-def add_dice_map(loc: str) -> dict[str, dict]:
-    """Load the dice-maps in the given file into memory.
+def add_dice_map(loc: str) -> dict[str, DiceMapping]:
+    """Load the dice-maps from a given file.
 
     :param loc: The location of the file of dice mappings to load.
     :return: None.
     :rtype: NoneType
+
+    Usage::
+
+        >>> from yadr import add_dice_map
+        >>>
+        >>> path = 'tests/data/__test_dice_map.txt'
+        >>> add_dice_map(path)              # doctest: +NORMALIZE_WHITESPACE
+        {'spam': {1: 'eggs', 2: 'bacon', 3: 'eggs', 4: 'tomato'}, 'fudge':
+        {1: '-', 2: '', 3: '+'}}
     """
     yadn = read_file(loc)
     return parse_map(yadn)
 
 
-def get_default_maps() -> dict[str, dict]:
-    """Get the default dice maps."""
+def get_default_maps() -> dict[str, DiceMapping]:
+    """Get the default dice maps.
+
+    :return: The default dice maps as a :class:`dict` of :class:`dict`
+        objects.
+    :rtype: dict
+
+    Usage::
+
+        >>> from yadr.yadr import get_default_maps
+        >>>
+        >>> get_default_maps()              # doctest: +ELLIPSIS
+        {'sweote boost': {1: '',...
+    """
     default_file = open_text('yadr.data', 'dice_maps.yadn')
     default_maps_yadn = default_file.read()
     default_file.close()
     return parse_map(default_maps_yadn)
 
 
 def list_dice_maps() -> str:
-    """Get the list of the currently loaded dice maps.
+    """Get the list of the default dice maps.
 
-    :return: A :class:str object.
+    :return: A :class:`str` object.
     :rtype: str
+
+    Usage::
+
+        >>> from yadr import list_dice_maps
+        >>>
+        >>> list_dice_maps()                # doctest: +ELLIPSIS
+        'sweote boost...
     """
     dice_map = get_default_maps()
     maps_ = '\n'.join(dice_map)
     return maps_
 
 
 def parse_cli() -> None:
@@ -142,15 +172,15 @@
         help='A string of YADN describing the die roll.',
         action='store',
         nargs='?',
         type=str
     )
     p.add_argument(
         '--list_dice_maps', '-l',
-        help='List the names of the loaded dice maps.',
+        help='List the names of the default dice maps.',
         action='store_true'
     )
     p.add_argument(
         '--add_dice_map', '-m',
         help='Load the dice mappings at the given file location.',
         nargs=1,
         action='store',
```

### Comparing `yadr-0.1.1/yadr.egg-info/PKG-INFO` & `yadr-0.1.2/yadr.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yadr
-Version: 0.1.1
+Version: 0.1.2
 Summary: Yet another dice roller for Python.
 Home-page: https://github.com/pji/yadr
 Author: Paul J. Iutzi
 Author-email: pji@mac.com
 Project-URL: Bug Tracker, https://github.com/pji/yadr/issues
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
@@ -36,15 +36,15 @@
 past when looking into algorithms, and it seemed like writing a
 parser to handle different dice systems seemed a reasonable way to go.
 As reasonable as any thought involving, "I'll use BNF here," can be,
 I guess. And so was born Yet Another Dice Notation (YADN) and `yadr`.
 
 For a description of YADN see: YADN_
 
-.. _YADN: https://github.com/pji/yadr/blob/main/docs/dice_notation.rst
+.. _YADN: https://github.com/pji/yadr/docs/build/html/dice_notation.html
 
 
 Do we need another Python dice rolling package?
 ===============================================
 No. Probably not. Unsurprisingly, there seems to be a lot of people who
 play TTRPGs and write Python packages. This is yet another one.
```

