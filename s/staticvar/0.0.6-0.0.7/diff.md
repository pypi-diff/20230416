# Comparing `tmp/staticvar-0.0.6.tar.gz` & `tmp/staticvar-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "staticvar-0.0.6.tar", max compression
+gzip compressed data, was "staticvar-0.0.7.tar", max compression
```

## Comparing `staticvar-0.0.6.tar` & `staticvar-0.0.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1080 2023-04-14 22:41:09.473574 staticvar-0.0.6/LICENSE.txt
--rw-r--r--   0        0        0      647 2023-04-14 22:41:09.473574 staticvar-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     3195 2023-04-14 22:41:09.473574 staticvar-0.0.6/README.md
--rw-r--r--   0        0        0        0 2023-04-14 22:41:09.473574 staticvar-0.0.6/staticvar/__init__.py
--rw-r--r--   0        0        0     2084 2023-04-14 22:41:09.473574 staticvar-0.0.6/staticvar/Static.py
--rw-r--r--   0        0        0     3851 1970-01-01 00:00:00.000000 staticvar-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-04-15 20:19:30.256792 staticvar-0.0.7/LICENSE.txt
+-rw-r--r--   0        0        0      647 2023-04-15 20:19:30.256792 staticvar-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     3753 2023-04-15 20:19:30.256792 staticvar-0.0.7/README.md
+-rw-r--r--   0        0        0       51 2023-04-15 20:19:30.266831 staticvar-0.0.7/staticvar/__init__.py
+-rw-r--r--   0        0        0     2084 2023-04-15 20:19:30.266831 staticvar-0.0.7/staticvar/Static.py
+-rw-r--r--   0        0        0     4399 1970-01-01 00:00:00.000000 staticvar-0.0.7/PKG-INFO
```

### Comparing `staticvar-0.0.6/LICENSE.txt` & `staticvar-0.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `staticvar-0.0.6/pyproject.toml` & `staticvar-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "staticvar"
-version = "0.0.6"
+version = "0.0.7"
 description = "The horrors of C Static variables for Python, with Python."
 authors = ["AbdelRahman <abdelrahman.rahal.mail@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/AbdelRahmanRahal/staticvar"
 repository = "https://github.com/AbdelRahmanRahal/staticvar"
 classifiers = [
```

### Comparing `staticvar-0.0.6/README.md` & `staticvar-0.0.7/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,57 +1,62 @@
 # staticvar
- A module that adds the horrors of C Static variables to Python, with Python. <br><br>
+A module that adds the horrors of C Static variables to Python, with Python. <br><br>
 
 > In programming, a static variable is the one allocated “statically,” which means its lifetime is throughout the program run.
 
 [Learn About Static Variables in C](https://www.upgrad.com/blog/static-variable-in-c) <br><br>
 
 Python does not provide a quick native way to declare static variables. There are some *workarounds*, but they don't look very nice; so I made a module that does it for you. <br><br>
 
-Currently, this module only supports integer, float, string and boolean types. <br><br>
+> **Note**: Currently, staticvar only supports integer, float, string and boolean types.
+<br>
 
-#
+## Installation
 To get started, install staticvar by typing the following in your command line:
 
-```
-pip install staticvar
-```
-<br><br>
+	pip install staticvar
+<br>You can also manually download and install staticvar from [PyPI](https://pypi.org/project/staticvar/). <br><br>
 
+> **Warning**: staticvar currently only works with Python >= 3.10. Compatability with older versions are in the works.
+<br>
+
+## Usage
+### `Static()`
 In your project, import the staticvar module as follows:
 
 ```python
 from staticvar import Static
 ```
 <br>
 
-Next, declare the name of the static variable with its value and type as the arguments:
+Next, declare the name of the static variable with its value and type as the arguments as follows:
 
 ```python
 # Syntax: VARIABLE_NAME = Static(VALUE, "TYPE")
 foo = Static(3, "int")
 ```
 Supported types include:
 - `"int"` for integer type variables
 - `"float"` for float type variables
 - `"str"` for string type variables
 - `"bool"` for boolean type variables
 
-Alternatively, if no type is passed, staticvar will infer the type.
-<br><br>
+Alternatively, if no type is specified, staticvar will infer the type. <br><br>
 
+### `.get()`
 To access the value of the variable, use the `get()` method:
 
 ```python
 print(foo.get())
 ```
 Output:
 
 `> 3`<br><br>
 
+### `.set()`
 To change the value of the variable, use the `set()` method with the desired value as the argument:
 
 ```python
 # Syntax: VARIABLE_NAME.set(VALUE)
 foo.set(4)
 print(foo.get())
 ```
@@ -64,24 +69,26 @@
 ```python
 print(foo.set(5))
 ```
 Ouput:
 
 `> 5`<br><br>
 
+### `.getType()`
 To get the type of the variable, use the `getType()` method:
 
 ```python
 print(foo.getType())
 ```
 Output:
 
 `> int`<br><br>
 
-Variables set using the staticvar module are not dynamic. Trying to later assign data with different types from the originally set/inferred one will raise an error if it cannot be converted/casted:
+### Static all the way
+Variables set using the staticvar module are **not** dynamic. Trying to later assign data with different types from the originally set/inferred one will raise an error if it cannot be converted/casted:
 
 ```python
 foo.set(6.9) # A float value in an integer variable type will be casted as an integer
 print(foo.get())
 ```
 Output:
 
@@ -91,32 +98,35 @@
 foo.set("Hello, mum!") # Python will fail to convert this non-numerical string into integer and will raise an error
 print(foo.get())
 ```
 Output:
 
 `> ValueError: invalid literal for int() with base 10: 'Hello, mum!'`<br><br><br>
 
-# An example on how to utilise static variables in a simple program
+## An example on how to utilise staticvar and static variables in a simple program
 Though there are better ways to do it, we can use static variables to find the factorial of a number.
 ```python
 from staticvar import Static
 
 
 # Using recursion and static variables to find the factorial of a number
 def factorial(limit, reset = True):
 	count = Static(1, "int")
-	answer = Static(1) # If no type specified, staticvar will infer the type
+	answer = Static(1) # If no type is specified, staticvar will infer the type
 
 	if reset == True:
 		count.set(1)
 		answer.set(1)
 
 	if count.get() <= limit:
 		answer.set(answer.get() * (count.set(count.get() + 1) - 1))
 		factorial(limit, False)
 
 	return answer.get()
 
 
-user_input = eval(input("Enter a number: "))
+user_input = int(input("Enter a number: "))
 print(factorial(user_input))
 ```
+Console:
+
+![The number 5 is entered, to which the code successfully echos its factorial, 120](https://github.com/AbdelRahmanRahal/staticvar/blob/main/exampleconsole.gif?raw=true)
```

### Comparing `staticvar-0.0.6/staticvar/Static.py` & `staticvar-0.0.7/staticvar/Static.py`

 * *Files identical despite different names*

### Comparing `staticvar-0.0.6/PKG-INFO` & `staticvar-0.0.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: staticvar
-Version: 0.0.6
+Version: 0.0.7
 Summary: The horrors of C Static variables for Python, with Python.
 Home-page: https://github.com/AbdelRahmanRahal/staticvar
 License: MIT
 Author: AbdelRahman
 Author-email: abdelrahman.rahal.mail@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -15,63 +15,68 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: varname (>=0.11.0,<0.12.0)
 Project-URL: Repository, https://github.com/AbdelRahmanRahal/staticvar
 Description-Content-Type: text/markdown
 
 # staticvar
- A module that adds the horrors of C Static variables to Python, with Python. <br><br>
+A module that adds the horrors of C Static variables to Python, with Python. <br><br>
 
 > In programming, a static variable is the one allocated “statically,” which means its lifetime is throughout the program run.
 
 [Learn About Static Variables in C](https://www.upgrad.com/blog/static-variable-in-c) <br><br>
 
 Python does not provide a quick native way to declare static variables. There are some *workarounds*, but they don't look very nice; so I made a module that does it for you. <br><br>
 
-Currently, this module only supports integer, float, string and boolean types. <br><br>
+> **Note**: Currently, staticvar only supports integer, float, string and boolean types.
+<br>
 
-#
+## Installation
 To get started, install staticvar by typing the following in your command line:
 
-```
-pip install staticvar
-```
-<br><br>
+	pip install staticvar
+<br>You can also manually download and install staticvar from [PyPI](https://pypi.org/project/staticvar/). <br><br>
 
+> **Warning**: staticvar currently only works with Python >= 3.10. Compatability with older versions are in the works.
+<br>
+
+## Usage
+### `Static()`
 In your project, import the staticvar module as follows:
 
 ```python
 from staticvar import Static
 ```
 <br>
 
-Next, declare the name of the static variable with its value and type as the arguments:
+Next, declare the name of the static variable with its value and type as the arguments as follows:
 
 ```python
 # Syntax: VARIABLE_NAME = Static(VALUE, "TYPE")
 foo = Static(3, "int")
 ```
 Supported types include:
 - `"int"` for integer type variables
 - `"float"` for float type variables
 - `"str"` for string type variables
 - `"bool"` for boolean type variables
 
-Alternatively, if no type is passed, staticvar will infer the type.
-<br><br>
+Alternatively, if no type is specified, staticvar will infer the type. <br><br>
 
+### `.get()`
 To access the value of the variable, use the `get()` method:
 
 ```python
 print(foo.get())
 ```
 Output:
 
 `> 3`<br><br>
 
+### `.set()`
 To change the value of the variable, use the `set()` method with the desired value as the argument:
 
 ```python
 # Syntax: VARIABLE_NAME.set(VALUE)
 foo.set(4)
 print(foo.get())
 ```
@@ -84,24 +89,26 @@
 ```python
 print(foo.set(5))
 ```
 Ouput:
 
 `> 5`<br><br>
 
+### `.getType()`
 To get the type of the variable, use the `getType()` method:
 
 ```python
 print(foo.getType())
 ```
 Output:
 
 `> int`<br><br>
 
-Variables set using the staticvar module are not dynamic. Trying to later assign data with different types from the originally set/inferred one will raise an error if it cannot be converted/casted:
+### Static all the way
+Variables set using the staticvar module are **not** dynamic. Trying to later assign data with different types from the originally set/inferred one will raise an error if it cannot be converted/casted:
 
 ```python
 foo.set(6.9) # A float value in an integer variable type will be casted as an integer
 print(foo.get())
 ```
 Output:
 
@@ -111,33 +118,36 @@
 foo.set("Hello, mum!") # Python will fail to convert this non-numerical string into integer and will raise an error
 print(foo.get())
 ```
 Output:
 
 `> ValueError: invalid literal for int() with base 10: 'Hello, mum!'`<br><br><br>
 
-# An example on how to utilise static variables in a simple program
+## An example on how to utilise staticvar and static variables in a simple program
 Though there are better ways to do it, we can use static variables to find the factorial of a number.
 ```python
 from staticvar import Static
 
 
 # Using recursion and static variables to find the factorial of a number
 def factorial(limit, reset = True):
 	count = Static(1, "int")
-	answer = Static(1) # If no type specified, staticvar will infer the type
+	answer = Static(1) # If no type is specified, staticvar will infer the type
 
 	if reset == True:
 		count.set(1)
 		answer.set(1)
 
 	if count.get() <= limit:
 		answer.set(answer.get() * (count.set(count.get() + 1) - 1))
 		factorial(limit, False)
 
 	return answer.get()
 
 
-user_input = eval(input("Enter a number: "))
+user_input = int(input("Enter a number: "))
 print(factorial(user_input))
 ```
+Console:
+
+![The number 5 is entered, to which the code successfully echos its factorial, 120](https://github.com/AbdelRahmanRahal/staticvar/blob/main/exampleconsole.gif?raw=true)
```

