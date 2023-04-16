# Comparing `tmp/ib110hw-0.0.6.tar.gz` & `tmp/ib110hw-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ib110hw-0.0.6.tar", last modified: Thu Apr  6 00:49:52 2023, max compression
+gzip compressed data, was "ib110hw-0.1.0.tar", last modified: Sun Apr 16 21:02:35 2023, max compression
```

## Comparing `ib110hw-0.0.6.tar` & `ib110hw-0.1.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 00:49:52.816638 ib110hw-0.0.6/
--rw-rw-rw-   0        0        0     1090 2023-01-20 12:57:50.000000 ib110hw-0.0.6/LICENSE
--rw-rw-rw-   0        0        0    13313 2023-04-06 00:49:52.815630 ib110hw-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0    12931 2023-04-02 23:02:46.000000 ib110hw-0.0.6/README.md
--rw-rw-rw-   0        0        0       42 2023-04-06 00:49:52.816638 ib110hw-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      649 2023-04-06 00:48:28.000000 ib110hw-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-06 00:49:52.762807 ib110hw-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-04-06 00:49:52.774348 ib110hw-0.0.6/src/ib110hw/
--rw-rw-rw-   0        0        0        0 2023-02-08 22:35:52.000000 ib110hw-0.0.6/src/ib110hw/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-06 00:49:52.802657 ib110hw-0.0.6/src/ib110hw/automaton/
--rw-rw-rw-   0        0        0        0 2022-10-30 17:04:59.000000 ib110hw-0.0.6/src/ib110hw/automaton/__init__.py
--rw-rw-rw-   0        0        0     2188 2023-04-06 00:38:14.000000 ib110hw-0.0.6/src/ib110hw/automaton/base.py
--rw-rw-rw-   0        0        0     8171 2023-04-06 00:37:57.000000 ib110hw-0.0.6/src/ib110hw/automaton/dfa.py
--rw-rw-rw-   0        0        0     8443 2023-04-06 00:38:34.000000 ib110hw-0.0.6/src/ib110hw/automaton/nfa.py
--rw-rw-rw-   0        0        0     1439 2023-02-10 23:11:04.000000 ib110hw-0.0.6/src/ib110hw/automaton/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-06 00:49:52.808664 ib110hw-0.0.6/src/ib110hw/turing/
--rw-rw-rw-   0        0        0        0 2022-11-28 20:58:41.000000 ib110hw-0.0.6/src/ib110hw/turing/__init__.py
--rw-rw-rw-   0        0        0     1042 2023-04-02 22:58:05.000000 ib110hw-0.0.6/src/ib110hw/turing/_helpers.py
--rw-rw-rw-   0        0        0     1239 2023-04-06 00:41:42.000000 ib110hw-0.0.6/src/ib110hw/turing/base.py
--rw-rw-rw-   0        0        0     4608 2023-04-06 00:42:06.000000 ib110hw-0.0.6/src/ib110hw/turing/dtm.py
--rw-rw-rw-   0        0        0     5704 2023-04-06 00:44:32.000000 ib110hw-0.0.6/src/ib110hw/turing/mtm.py
--rw-rw-rw-   0        0        0     3474 2023-04-06 00:42:49.000000 ib110hw-0.0.6/src/ib110hw/turing/tape.py
-drwxrwxrwx   0        0        0        0 2023-04-06 00:49:52.792041 ib110hw-0.0.6/src/ib110hw.egg-info/
--rw-rw-rw-   0        0        0    13313 2023-04-06 00:49:52.000000 ib110hw-0.0.6/src/ib110hw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      597 2023-04-06 00:49:52.000000 ib110hw-0.0.6/src/ib110hw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 00:49:52.000000 ib110hw-0.0.6/src/ib110hw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-04-06 00:49:52.000000 ib110hw-0.0.6/src/ib110hw.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-06 00:49:52.814377 ib110hw-0.0.6/tests/
--rw-rw-rw-   0        0        0     3455 2023-04-02 22:49:15.000000 ib110hw-0.0.6/tests/test.py
--rw-rw-rw-   0        0        0     7220 2023-03-05 22:42:15.000000 ib110hw-0.0.6/tests/test_dfa.py
--rw-rw-rw-   0        0        0     2369 2023-04-02 20:51:44.000000 ib110hw-0.0.6/tests/test_dtm.py
--rw-rw-rw-   0        0        0     2028 2023-04-02 20:51:33.000000 ib110hw-0.0.6/tests/test_mtm.py
--rw-rw-rw-   0        0        0     8579 2023-03-25 22:51:22.000000 ib110hw-0.0.6/tests/test_nfa.py
+drwxrwxrwx   0        0        0        0 2023-04-16 21:02:35.575616 ib110hw-0.1.0/
+-rw-rw-rw-   0        0        0     1090 2023-01-20 12:57:50.000000 ib110hw-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0    26611 2023-04-16 21:02:35.575616 ib110hw-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0    26229 2023-04-16 20:59:38.000000 ib110hw-0.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-16 21:02:35.575616 ib110hw-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      649 2023-04-16 21:00:19.000000 ib110hw-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-16 21:02:35.531004 ib110hw-0.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-04-16 21:02:35.541619 ib110hw-0.1.0/src/ib110hw/
+-rw-rw-rw-   0        0        0        0 2023-02-08 22:35:52.000000 ib110hw-0.1.0/src/ib110hw/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-16 21:02:35.562615 ib110hw-0.1.0/src/ib110hw/automaton/
+-rw-rw-rw-   0        0        0        0 2022-10-30 17:04:59.000000 ib110hw-0.1.0/src/ib110hw/automaton/__init__.py
+-rw-rw-rw-   0        0        0     2304 2023-04-16 00:59:04.000000 ib110hw-0.1.0/src/ib110hw/automaton/base.py
+-rw-rw-rw-   0        0        0     8262 2023-04-16 19:56:06.000000 ib110hw-0.1.0/src/ib110hw/automaton/dfa.py
+-rw-rw-rw-   0        0        0     8539 2023-04-16 19:56:24.000000 ib110hw-0.1.0/src/ib110hw/automaton/nfa.py
+-rw-rw-rw-   0        0        0     1439 2023-02-10 23:11:04.000000 ib110hw-0.1.0/src/ib110hw/automaton/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-16 21:02:35.569615 ib110hw-0.1.0/src/ib110hw/turing/
+-rw-rw-rw-   0        0        0        0 2022-11-28 20:58:41.000000 ib110hw-0.1.0/src/ib110hw/turing/__init__.py
+-rw-rw-rw-   0        0        0     4911 2023-04-11 20:33:53.000000 ib110hw-0.1.0/src/ib110hw/turing/_helpers.py
+-rw-rw-rw-   0        0        0     1239 2023-04-06 00:41:42.000000 ib110hw-0.1.0/src/ib110hw/turing/base.py
+-rw-rw-rw-   0        0        0     4606 2023-04-11 17:53:39.000000 ib110hw-0.1.0/src/ib110hw/turing/dtm.py
+-rw-rw-rw-   0        0        0     5704 2023-04-06 00:44:32.000000 ib110hw-0.1.0/src/ib110hw/turing/mtm.py
+-rw-rw-rw-   0        0        0     3474 2023-04-06 00:42:49.000000 ib110hw-0.1.0/src/ib110hw/turing/tape.py
+-rw-rw-rw-   0        0        0     1357 2023-04-11 20:31:00.000000 ib110hw-0.1.0/src/ib110hw/turing/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-16 21:02:35.557614 ib110hw-0.1.0/src/ib110hw.egg-info/
+-rw-rw-rw-   0        0        0    26611 2023-04-16 21:02:35.000000 ib110hw-0.1.0/src/ib110hw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      611 2023-04-16 21:02:35.000000 ib110hw-0.1.0/src/ib110hw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-16 21:02:35.000000 ib110hw-0.1.0/src/ib110hw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-16 21:02:35.000000 ib110hw-0.1.0/src/ib110hw.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-16 21:02:35.573614 ib110hw-0.1.0/tests/
+-rw-rw-rw-   0        0        0     7220 2023-04-16 19:57:54.000000 ib110hw-0.1.0/tests/test_dfa.py
+-rw-rw-rw-   0        0        0     2369 2023-04-02 20:51:44.000000 ib110hw-0.1.0/tests/test_dtm.py
+-rw-rw-rw-   0        0        0     2028 2023-04-02 20:51:33.000000 ib110hw-0.1.0/tests/test_mtm.py
+-rw-rw-rw-   0        0        0     8579 2023-04-16 19:57:58.000000 ib110hw-0.1.0/tests/test_nfa.py
```

### Comparing `ib110hw-0.0.6/LICENSE` & `ib110hw-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ib110hw-0.0.6/setup.py` & `ib110hw-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ib110hw",
-    version="0.0.6",
+    version="0.1.0",
     author="Martin Pilát",
     author_email="8pilatmartin8@gmail.com",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

### Comparing `ib110hw-0.0.6/src/ib110hw/automaton/base.py` & `ib110hw-0.1.0/src/ib110hw/automaton/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,19 +21,20 @@
     ) -> None:
         self.states = states or set()
         self.alphabet = alphabet or set()
         self.initial_state = initial_state
         self.final_states = final_states or set()
 
     def __repr__(self) -> str:
-        alphabet_str = ",".join(self.alphabet)
-        states_str = ",".join(self.states)
-        final_states_str = ",".join(self.final_states)
+        alphabet_str = f"alphabet: {','.join(sorted(self.alphabet))}"
+        states_str = f"states: {','.join(sorted(self.states))}"
+        initial_str = f"initial state: {self.initial_state}"
+        final_states_str = f"final states: {','.join(sorted(self.final_states))}"
 
-        return f"alphabet: {alphabet_str}\nstates: {states_str}\nfinal states: {final_states_str}\n"
+        return f"{alphabet_str}\n{states_str}\n{initial_str}\n{final_states_str}\n"
 
     def __repr_row_prefix__(self, state: str):
         if state == self.initial_state:
             return "<-> " if state in self.final_states else "--> "
 
         return "<-- " if state in self.final_states else "    "
```

### Comparing `ib110hw-0.0.6/src/ib110hw/automaton/dfa.py` & `ib110hw-0.1.0/src/ib110hw/automaton/dfa.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,18 @@
     def __init__(
         self,
         states: Set[str] = None,
         alphabet: Set[str] = None,
         initial_state: str = None,
         final_states: Set[str] = None,
         transitions: DFATransitions = None,
-    ):
+    ) -> None:
+        if transitions:
+            states = states or set(transitions.keys())
+
         super().__init__(states, alphabet, initial_state, final_states)
         self.transitions = transitions or {}
 
     def __repr__(self) -> str:
         return super().__repr__() + "\n" + self.__repr_transitions__()
 
     def __repr_transitions__(self) -> str:
@@ -70,15 +73,15 @@
         Returns:
             str: Next state if such transition exists, None otherwise.
         """
         return self.transitions.get(state_from, {}).get(symbol, None)
 
     def set_transition(self, state_from: str, state_to: str, symbol: str) -> None:
         """
-        Adds/changes transition to automaton.
+        Adds/changes transition.
         If the automaton already contains transition from 'state_from' by 'symbol', it will be overwritten.
 
         Args:
             state_from (str): State name where the transition starts.
             state_to (str): State name where the transition ends.
             symbol (str): Transition symbol.
         """
@@ -184,14 +187,16 @@
 
         Args:
             input_string (str): Input string to be tested.
 
         Returns:
             bool: True if word is accepted, False otherwise.
         """
+        assert self.is_valid(), "DFA needs to be valid."
+
         current_state = self.initial_state
 
         for symbol in input_string:
             if not (current_state := self.get_transition(current_state, symbol)):
                 return False
 
         return current_state in self.final_states
@@ -206,35 +211,29 @@
             5. The transition function contains characters only from its alphabet.
             6. The transition function contains states only from its states set.
             7. The transition function is total.
 
         Returns:
             bool: True if DFA is valid, False otherwise.
         """
+        t_values = self.transitions.values()
+
         # creates set of states used in the transition function
-        used_states = set(
-            sum((list(v.values()) for v in list(self.transitions.values())), [])
-        ) | set(self.transitions.keys())
+        used_states = set(sum((list(v.values()) for v in list(t_values)), [])) | set(
+            self.transitions.keys()
+        )
 
         # creates a set of symbols used in the transition function
-        used_symbols = set(sum((list(v.keys()) for v in self.transitions.values()), []))
-
-        # rules 1 - 6
-        if (
-            not super().is_valid()
-            or "" in self.alphabet
-            or self.states.symmetric_difference(used_states)
-            or used_symbols.symmetric_difference(self.alphabet)
-        ):
-            return False
-
-        # rule 7
-        if self.states - set(self.transitions.keys()) or any(
-            self.alphabet - {*rule.keys()} for rule in self.transitions.values()
-        ):
-            return False
+        used_symbols = set(sum((list(v.keys()) for v in t_values), []))
 
-        return True
+        return not (
+            not super().is_valid()  # rules 1-3
+            or "" in self.alphabet  # rule 4
+            or used_symbols.symmetric_difference(self.alphabet)  # rule 5
+            or self.states.symmetric_difference(used_states)  # rule 6
+            or self.states.difference(self.transitions.keys())  # rule 7
+            or any(self.alphabet.difference(rule.keys()) for rule in t_values)  # rule 7
+        )
 
 
 if __name__ == "__main__":
     pass
```

### Comparing `ib110hw-0.0.6/src/ib110hw/automaton/nfa.py` & `ib110hw-0.1.0/src/ib110hw/automaton/nfa.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,18 @@
     def __init__(
         self,
         states: Set[str] = None,
         alphabet: Set[str] = None,
         initial_state: str = None,
         final_states: Set[str] = None,
         transitions: NFATransitions = None,
-    ):
+    ) -> None:
+        if transitions:
+            states = states or set(transitions.keys())
+
         super().__init__(states, alphabet, initial_state, final_states)
         self.transitions = transitions or {}
 
     def __repr__(self) -> str:
         return super().__repr__() + "\n" + self.__repr_transitions__()
 
     def __repr_transitions__(self) -> str:
@@ -91,15 +94,15 @@
 
     def add_transition(self, state_from: str, state_to: str, symbol: str) -> bool:
         """
         Adds transition to the automaton and returns bool based on a change.
 
         Args:
             state_from (str): State name where the transition starts.
-            states_to (Set[str]): Set of states where the transition ends.
+            state_to (str): State name where the transition ends.
             symbol (str): Transition symbol.
 
         Returns:
             bool: True if the transition function changed, otherwise False.
         """
         if state_from not in self.transitions.keys():
             self.transitions[state_from] = {symbol: {state_to}}
@@ -198,14 +201,15 @@
 
         Args:
             input_string (str): Input string to be tested.
 
         Returns:
             bool: True if word is accepted, False otherwise.
         """
+        assert self.is_valid(), "NFA needs to be valid."
 
         def is_accepted_rec(current_state: str, curr_input: str) -> bool:
             if not curr_input:
                 return current_state in self.final_states
 
             if not self.get_transition(current_state, curr_input[0]):
                 return False
@@ -227,27 +231,23 @@
             3. Final states are subset of states.
             4. The transition function contains characters only from its alphabet.
             5. The transition function contains states only from its states set.
 
         Returns:
             bool: True if NFA is valid, False otherwise.
         """
+        t_values = self.transitions.values()
+
         # creates set of states used in the transition function
         used_states = set().union(
-            *sum((list(v.values()) for v in list(self.transitions.values())), [])
+            *sum((list(v.values()) for v in list(t_values)), [])
         ) | set(self.transitions.keys())
 
-        # rule 5
-        if used_states - self.states:
-            return False
-
-        # rules 1-4
-        if not super().is_valid() or any(
-            set(rule.keys()) - self.alphabet for rule in self.transitions.values()
-        ):
-            return False
-
-        return True
+        return not (
+            not super().is_valid()  # rules 1-3
+            or any(set(rule.keys()) - self.alphabet for rule in t_values)  # rule 4
+            or used_states - self.states  # rule 5
+        )
 
 
 if __name__ == "__main__":
     pass
```

### Comparing `ib110hw-0.0.6/src/ib110hw/automaton/utils.py` & `ib110hw-0.1.0/src/ib110hw/automaton/utils.py`

 * *Files identical despite different names*

### Comparing `ib110hw-0.0.6/src/ib110hw/turing/base.py` & `ib110hw-0.1.0/src/ib110hw/turing/base.py`

 * *Files identical despite different names*

### Comparing `ib110hw-0.0.6/src/ib110hw/turing/dtm.py` & `ib110hw-0.1.0/src/ib110hw/turing/dtm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from os import name, system
 from time import sleep
 from typing import Dict, Optional, Set, Tuple
 
 from .base import BaseTuringMachine, MAX_STEPS_ERROR_MSG
 from .tape import Direction, Tape, START_SYMBOL
 from ._helpers import dtm_config_to_md, clear_console, close_file
 
@@ -31,15 +30,15 @@
             states,
             input_alphabet,
             acc_states,
             rej_states,
             initial_state,
             start_symbol,
         )
-        self.transitions = transitions or Tape()
+        self.transitions = transitions or {}
         self.tape = tape or Tape()
 
     def get_transition(self, state: str, read: str) -> Optional[DTMRule]:
         """
         Gets the transition based on the provided state and read symbol.
 
         Args:
@@ -91,14 +90,15 @@
             path (str, optional): Path to the .md file with the step history. Defaults to "simulation.md".
             delay (float, optional): The delay (s) between each step when printing to console. Defaults to 0.5.
 
         Returns:
             bool: False if the machine rejects the word or exceeds the 'max_steps' value, True otherwise.
         """
         state: str = self.initial_state
+        print("state", state)
         steps: int = 1
         output_file = None
 
         def get_rule_string() -> str:
             row = self.get_transition(state, self.tape.current.value)
             step_index = steps if row else steps - 1
             next_step = f"{state}, {self.tape.current.value}"
```

### Comparing `ib110hw-0.0.6/src/ib110hw/turing/mtm.py` & `ib110hw-0.1.0/src/ib110hw/turing/mtm.py`

 * *Files identical despite different names*

### Comparing `ib110hw-0.0.6/src/ib110hw/turing/tape.py` & `ib110hw-0.1.0/src/ib110hw/turing/tape.py`

 * *Files identical despite different names*

### Comparing `ib110hw-0.0.6/src/ib110hw.egg-info/SOURCES.txt` & `ib110hw-0.1.0/src/ib110hw.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -13,12 +13,12 @@
 src/ib110hw/automaton/utils.py
 src/ib110hw/turing/__init__.py
 src/ib110hw/turing/_helpers.py
 src/ib110hw/turing/base.py
 src/ib110hw/turing/dtm.py
 src/ib110hw/turing/mtm.py
 src/ib110hw/turing/tape.py
-tests/test.py
+src/ib110hw/turing/utils.py
 tests/test_dfa.py
 tests/test_dtm.py
 tests/test_mtm.py
 tests/test_nfa.py
```

### Comparing `ib110hw-0.0.6/tests/test_dfa.py` & `ib110hw-0.1.0/tests/test_dfa.py`

 * *Files identical despite different names*

### Comparing `ib110hw-0.0.6/tests/test_dtm.py` & `ib110hw-0.1.0/tests/test_dtm.py`

 * *Files identical despite different names*

### Comparing `ib110hw-0.0.6/tests/test_mtm.py` & `ib110hw-0.1.0/tests/test_mtm.py`

 * *Files identical despite different names*

### Comparing `ib110hw-0.0.6/tests/test_nfa.py` & `ib110hw-0.1.0/tests/test_nfa.py`

 * *Files identical despite different names*

