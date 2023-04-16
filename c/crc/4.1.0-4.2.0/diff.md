# Comparing `tmp/crc-4.1.0.tar.gz` & `tmp/crc-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crc-4.1.0.tar", max compression
+gzip compressed data, was "crc-4.2.0.tar", max compression
```

## Comparing `crc-4.1.0.tar` & `crc-4.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1300 2022-12-18 15:53:07.228415 crc-4.1.0/LICENSE.txt
--rw-r--r--   0        0        0     4437 2022-12-18 15:53:07.228415 crc-4.1.0/README.md
--rw-r--r--   0        0        0    15843 2022-12-18 15:53:07.228415 crc-4.1.0/crc.py
--rw-r--r--   0        0        0     1680 2022-12-18 15:53:07.232415 crc-4.1.0/pyproject.toml
--rw-r--r--   0        0        0     5271 1970-01-01 00:00:00.000000 crc-4.1.0/setup.py
--rw-r--r--   0        0        0     5530 1970-01-01 00:00:00.000000 crc-4.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1301 2023-04-16 09:43:05.059044 crc-4.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     4467 2023-04-16 09:43:05.059044 crc-4.2.0/README.md
+-rw-r--r--   0        0        0    16059 2023-04-16 09:43:05.059044 crc-4.2.0/crc.py
+-rw-r--r--   0        0        0     1711 2023-04-16 09:43:05.059044 crc-4.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5300 1970-01-01 00:00:00.000000 crc-4.2.0/setup.py
+-rw-r--r--   0        0        0     5560 1970-01-01 00:00:00.000000 crc-4.2.0/PKG-INFO
```

### Comparing `crc-4.1.0/LICENSE.txt` & `crc-4.2.0/LICENSE.txt`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -15,8 +15,8 @@
 WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
 DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR CONTRIBUTORS BE LIABLE FOR
 ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
 (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
 LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
 ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
-WARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+WARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `crc-4.1.0/README.md` & `crc-4.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -30,30 +30,30 @@
 * Documentation: [https://nicoretti.github.io/crc](https://nicoretti.github.io/crc)
 * Source Code: [https://github.com/Nicoretti/crc](https://github.com/Nicoretti/crc)
 ---
 
 ## Available CRC Configurations
 For convince various frequently used crc configurations ship with the library out of the box.
 
-| CRC8 | CRC16 | CRC32 | CRC64 |
-|------|-------|-------|-------|
-| CCITT | CCITT | CRC32 | CRC64 |
-| AUTOSAR | GSM | AUTOSAR | |
+| CRC8 | CRC16    | CRC32 | CRC64 |
+|------|----------|-------|-------|
+| CCITT | CCITT    | CRC32 | CRC64 |
+| AUTOSAR | GSM      | AUTOSAR | |
 | SAJ1850 | PROFIBUS | BZIP2 | |
-| BLUETOOTH | | POSIX | |
-| MAXIM-DOW | | | | |
+| BLUETOOTH | MODBUS   | POSIX | |
+| MAXIM-DOW |          | | | |
 
 If you find yourself in the position, where having a new configuration available out of the
 box would be desirable, feel free to create a [PR](https://github.com/Nicoretti/crc/pulls) or file an [issue](https://github.com/Nicoretti/crc/issues).
 
 ## Custom Configurations
 
 If you want to create a custom configuration, you should have the following information available:
 
-🗒 Note: 
+🗒 Note:
 
     This library currently only supports bit widths of full bytes 8, 16, 24, 32, ...
 
 * **width**
 * **polynom**
 * **init value**
 * **final xor value**
@@ -182,8 +182,7 @@
 assert expected == register.digest()
 ```
 
 References & Resources
 -----------------------
 * [A Painless guide to crc error detection algorithms](http://www.zlib.net/crc_v3.txt)
 * [CRC-Catalogue](http://reveng.sourceforge.net/crc-catalogue/all.htm)
-
```

#### html2text {}

```diff
@@ -3,49 +3,49 @@
                            custom CRC configurations
  [Checks_Master] [Coverage] [License] [Downloads] [Supported_Python_Versions]
                                 [PyPi_Package]
 --- * Documentation: [https://nicoretti.github.io/crc](https://
 nicoretti.github.io/crc) * Source Code: [https://github.com/Nicoretti/crc]
 (https://github.com/Nicoretti/crc) --- ## Available CRC Configurations For
 convince various frequently used crc configurations ship with the library out
-of the box. | CRC8 | CRC16 | CRC32 | CRC64 | |------|-------|-------|-------| |
-CCITT | CCITT | CRC32 | CRC64 | | AUTOSAR | GSM | AUTOSAR | | | SAJ1850 |
-PROFIBUS | BZIP2 | | | BLUETOOTH | | POSIX | | | MAXIM-DOW | | | | | If you
-find yourself in the position, where having a new configuration available out
-of the box would be desirable, feel free to create a [PR](https://github.com/
-Nicoretti/crc/pulls) or file an [issue](https://github.com/Nicoretti/crc/
-issues). ## Custom Configurations If you want to create a custom configuration,
-you should have the following information available: ð Note: This library
-currently only supports bit widths of full bytes 8, 16, 24, 32, ... * **width**
-* **polynom** * **init value** * **final xor value** * **reversed input** *
-**reversed output** In case you only have a name of a specific crc
-configuration/algorithm and you are unsure what are the specific parameters of
-it, a look into this [crc-catalogue](http://reveng.sourceforge.net/crc-
-catalogue/all.htm) might help. ## Requirements * [\>= Python 3.8](https://
-www.python.org) ## Installation ```shell pip install crc ``` ## Examples ###
-Create a Calculator #### Pre defined configuration ```python from crc import
-Calculator, Crc8 calculator = Calculator(Crc8.CCITT) ``` #### Custom
-configuration ```python from crc import Calculator, Configuration config =
-Configuration( width=8, polynomial=0x07, init_value=0x00, final_xor_value=0x00,
-reverse_input=False, reverse_output=False, ) calculator = Calculator(config)
-``` ### Calculate a checksum #### Standard ```python from crc import
-Calculator, Crc8 expected = 0xBC data = bytes([0, 1, 2, 3, 4, 5]) calculator =
-Calculator(Crc8.CCITT) assert expected == calculator.checksum(data) ``` ####
-Optimized for speed ```python from crc import Calculator, Crc8 expected = 0xBC
-data = bytes([0, 1, 2, 3, 4, 5]) calculator = Calculator(Crc8.CCITT,
-optimized=True) assert expected == calculator.checksum(data) ``` ### Verify a
+of the box. | CRC8 | CRC16 | CRC32 | CRC64 | |------|----------|-------|-------
+| | CCITT | CCITT | CRC32 | CRC64 | | AUTOSAR | GSM | AUTOSAR | | | SAJ1850 |
+PROFIBUS | BZIP2 | | | BLUETOOTH | MODBUS | POSIX | | | MAXIM-DOW | | | | | If
+you find yourself in the position, where having a new configuration available
+out of the box would be desirable, feel free to create a [PR](https://
+github.com/Nicoretti/crc/pulls) or file an [issue](https://github.com/
+Nicoretti/crc/issues). ## Custom Configurations If you want to create a custom
+configuration, you should have the following information available: ð Note:
+This library currently only supports bit widths of full bytes 8, 16, 24, 32,
+... * **width** * **polynom** * **init value** * **final xor value** *
+**reversed input** * **reversed output** In case you only have a name of a
+specific crc configuration/algorithm and you are unsure what are the specific
+parameters of it, a look into this [crc-catalogue](http://
+reveng.sourceforge.net/crc-catalogue/all.htm) might help. ## Requirements *
+[\>= Python 3.8](https://www.python.org) ## Installation ```shell pip install
+crc ``` ## Examples ### Create a Calculator #### Pre defined configuration
+```python from crc import Calculator, Crc8 calculator = Calculator(Crc8.CCITT)
+``` #### Custom configuration ```python from crc import Calculator,
+Configuration config = Configuration( width=8, polynomial=0x07,
+init_value=0x00, final_xor_value=0x00, reverse_input=False,
+reverse_output=False, ) calculator = Calculator(config) ``` ### Calculate a
 checksum #### Standard ```python from crc import Calculator, Crc8 expected =
 0xBC data = bytes([0, 1, 2, 3, 4, 5]) calculator = Calculator(Crc8.CCITT)
-assert calculator.verify(data, expected) ``` #### Optimized for speed ```python
-from crc import Calculator, Crc8 expected = 0xBC data = bytes([0, 1, 2, 3, 4,
-5]) calculator = Calculator(Crc8.CCITT, optimized=True) assert
-calculator.verify(data, expected) ``` ### Calculate a checksum with raw
-registers #### Register ```python from crc import Crc8, Register expected =
-0xBC data = bytes([0, 1, 2, 3, 4, 5]) register = Register(Crc8.CCITT)
-register.init() register.update(data) assert expected == register.digest() ```
-#### TableBasedRegister ```python from crc import Crc8, TableBasedRegister
-expected = 0xBC data = bytes([0, 1, 2, 3, 4, 5]) register = TableBasedRegister
-(Crc8.CCITT) register.init() register.update(data) assert expected ==
-register.digest() ``` References & Resources ----------------------- * [A
-Painless guide to crc error detection algorithms](http://www.zlib.net/
+assert expected == calculator.checksum(data) ``` #### Optimized for speed
+```python from crc import Calculator, Crc8 expected = 0xBC data = bytes([0, 1,
+2, 3, 4, 5]) calculator = Calculator(Crc8.CCITT, optimized=True) assert
+expected == calculator.checksum(data) ``` ### Verify a checksum #### Standard
+```python from crc import Calculator, Crc8 expected = 0xBC data = bytes([0, 1,
+2, 3, 4, 5]) calculator = Calculator(Crc8.CCITT) assert calculator.verify(data,
+expected) ``` #### Optimized for speed ```python from crc import Calculator,
+Crc8 expected = 0xBC data = bytes([0, 1, 2, 3, 4, 5]) calculator = Calculator
+(Crc8.CCITT, optimized=True) assert calculator.verify(data, expected) ``` ###
+Calculate a checksum with raw registers #### Register ```python from crc import
+Crc8, Register expected = 0xBC data = bytes([0, 1, 2, 3, 4, 5]) register =
+Register(Crc8.CCITT) register.init() register.update(data) assert expected ==
+register.digest() ``` #### TableBasedRegister ```python from crc import Crc8,
+TableBasedRegister expected = 0xBC data = bytes([0, 1, 2, 3, 4, 5]) register =
+TableBasedRegister(Crc8.CCITT) register.init() register.update(data) assert
+expected == register.digest() ``` References & Resources ----------------------
+- * [A Painless guide to crc error detection algorithms](http://www.zlib.net/
 crc_v3.txt) * [CRC-Catalogue](http://reveng.sourceforge.net/crc-catalogue/
 all.htm)
```

### Comparing `crc-4.1.0/crc.py` & `crc-4.2.0/crc.py`

 * *Files 1% similar despite different names*

```diff
@@ -406,15 +406,15 @@
     data: Union[int, ByteString, BinaryIO, Iterable[ByteString]]
 ) -> Iterable[bytes]:
     if isinstance(data, int):
         yield data.to_bytes(1, "big")
     elif isinstance(data, ByteString):
         yield bytes(data)
     elif isinstance(data, (Iterable, BinaryIO)):
-        yield from data
+        yield from (bytes(e) for e in data)
     else:
         raise TypeError(f"Unsupported parameter type: {type(data)}")
 
 
 @enum.unique
 class Crc8(enum.Enum):
     CCITT = Configuration(
@@ -488,14 +488,23 @@
         polynomial=0x1DCF,
         init_value=0xFFFF,
         final_xor_value=0xFFFF,
         reverse_input=False,
         reverse_output=False,
     )
 
+    MODBUS = Configuration(
+        width=16,
+        polynomial=0x8005,
+        init_value=0xFFFF,
+        final_xor_value=0x0000,
+        reverse_input=True,
+        reverse_output=True,
+    )
+
 
 @enum.unique
 class Crc32(enum.Enum):
     CRC32 = Configuration(
         width=32,
         polynomial=0x04C11DB7,
         init_value=0xFFFFFFFF,
```

### Comparing `crc-4.1.0/pyproject.toml` & `crc-4.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "crc"
-version = "4.1.0"
+version = "4.2.0"
 description = "Library and CLI to calculate and verify all kinds of CRC checksums"
 packages = [
     { include = "crc.py" },
 ]
 authors = ["Nicola Coretti <nico.coretti@gmail.com>"]
 maintainers = ["Nicola Coretti <nico.coretti@gmail.com>"]
 license = "BSD-2-Clause"
@@ -25,30 +25,30 @@
 [tool.poetry.scripts]
 crc = "crc:main"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.2.0"
-pylint = "^2.12.2"
-black = "^22.1.0"
-isort = "^5.10.1"
-coveralls = "^3.3.1"
-mkdocs = "^1.4.2"
-mkdocs-material = "^8.5.10"
-pyupgrade = "^3.2.2"
-shed = "^0.10.7"
-mypy = "^0.991"
-invoke = "^1.7.3"
-mkdocs-autorefs = "^0.4.1"
-mkdocstrings = "^0.19.0"
-mkdocstrings-python = "^0.8.2"
-pytkdocs = "^0.16.1"
-
+pytest = ">=7.2.0"
+pylint = ">=2.12.2"
+black = ">=22.1.0"
+isort = ">=5.10.1"
+coveralls = ">=3.3.1"
+mkdocs = ">=1.4.2"
+mkdocs-material = ">=9.0.6"
+pyupgrade = ">=3.2.2"
+shed = ">=0.10.7"
+mypy = ">=0.991"
+invoke = ">=2"
+mkdocs-autorefs = ">=0.4.1"
+mkdocstrings = ">=0.20.0"
+mkdocstrings-python = ">=0.8.2"
+pytkdocs = ">=0.16.1"
+pre-commit = "^3.1.1"
 
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.coverage.run]
```

### Comparing `crc-4.1.0/setup.py` & `crc-4.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 modules = \
 ['crc']
 entry_points = \
 {'console_scripts': ['crc = crc:main']}
 
 setup_kwargs = {
     'name': 'crc',
-    'version': '4.1.0',
+    'version': '4.2.0',
     'description': 'Library and CLI to calculate and verify all kinds of CRC checksums',
-    'long_description': '<h1 align="center">CRC</h1>\n<p align="center">\n\nCalculate CRC checksums, verify CRC checksum, predefined CRC configurations, custom CRC configurations\n</p>\n\n<p align="center">\n\n<a href="https://github.com/Nicoretti/crc/actions">\n    <img src="https://img.shields.io/github/checks-status/nicoretti/crc/master" alt="Checks Master">\n</a>\n<a href="https://coveralls.io/github/Nicoretti/crc">\n    <img src="https://img.shields.io/coverallsCoverage/github/Nicoretti/crc" alt="Coverage">\n</a>\n<a href="https://opensource.org/licenses/BSD-2-Clause">\n    <img src="https://img.shields.io/pypi/l/crc" alt="License">\n</a>\n<a href="https://pypi.org/project/crc/">\n    <img src="https://img.shields.io/pypi/dm/crc" alt="Downloads">\n</a>\n<a href="https://pypi.org/project/crc/">\n    <img src="https://img.shields.io/pypi/pyversions/crc" alt="Supported Python Versions">\n</a>\n<a href="https://pypi.org/project/crc/">\n    <img src="https://img.shields.io/pypi/v/crc" alt="PyPi Package">\n</a>\n</p>\n\n---\n* Documentation: [https://nicoretti.github.io/crc](https://nicoretti.github.io/crc)\n* Source Code: [https://github.com/Nicoretti/crc](https://github.com/Nicoretti/crc)\n---\n\n## Available CRC Configurations\nFor convince various frequently used crc configurations ship with the library out of the box.\n\n| CRC8 | CRC16 | CRC32 | CRC64 |\n|------|-------|-------|-------|\n| CCITT | CCITT | CRC32 | CRC64 |\n| AUTOSAR | GSM | AUTOSAR | |\n| SAJ1850 | PROFIBUS | BZIP2 | |\n| BLUETOOTH | | POSIX | |\n| MAXIM-DOW | | | | |\n\nIf you find yourself in the position, where having a new configuration available out of the\nbox would be desirable, feel free to create a [PR](https://github.com/Nicoretti/crc/pulls) or file an [issue](https://github.com/Nicoretti/crc/issues).\n\n## Custom Configurations\n\nIf you want to create a custom configuration, you should have the following information available:\n\n🗒 Note: \n\n    This library currently only supports bit widths of full bytes 8, 16, 24, 32, ...\n\n* **width**\n* **polynom**\n* **init value**\n* **final xor value**\n* **reversed input**\n* **reversed output**\n\nIn case you only have a name of a specific crc configuration/algorithm and you are unsure what are the specific parameters\nof it, a look into this [crc-catalogue](http://reveng.sourceforge.net/crc-catalogue/all.htm) might help.\n\n\n## Requirements\n* [\\>= Python 3.8](https://www.python.org)\n\n## Installation\n\n```shell\npip install crc\n```\n\n## Examples\n\n### Create a Calculator\n\n#### Pre defined configuration\n\n```python\nfrom crc import Calculator, Crc8\n\ncalculator = Calculator(Crc8.CCITT)\n```\n#### Custom configuration\n\n```python\nfrom crc import Calculator, Configuration\n\nconfig = Configuration(\n    width=8,\n    polynomial=0x07,\n    init_value=0x00,\n    final_xor_value=0x00,\n    reverse_input=False,\n    reverse_output=False,\n)\n\ncalculator = Calculator(config)\n```\n\n### Calculate a checksum\n\n#### Standard\n\n```python\nfrom crc import Calculator, Crc8\n\nexpected = 0xBC\ndata = bytes([0, 1, 2, 3, 4, 5])\ncalculator = Calculator(Crc8.CCITT)\n\nassert expected == calculator.checksum(data)\n```\n\n#### Optimized for speed\n\n```python\nfrom crc import Calculator, Crc8\n\nexpected = 0xBC\ndata = bytes([0, 1, 2, 3, 4, 5])\ncalculator = Calculator(Crc8.CCITT, optimized=True)\n\nassert expected == calculator.checksum(data)\n```\n\n### Verify a checksum\n\n#### Standard\n\n```python\nfrom crc import Calculator, Crc8\n\nexpected = 0xBC\ndata = bytes([0, 1, 2, 3, 4, 5])\ncalculator = Calculator(Crc8.CCITT)\n\nassert calculator.verify(data, expected)\n```\n\n#### Optimized for speed\n\n```python\nfrom crc import Calculator, Crc8\n\nexpected = 0xBC\ndata = bytes([0, 1, 2, 3, 4, 5])\ncalculator = Calculator(Crc8.CCITT, optimized=True)\n\nassert calculator.verify(data, expected)\n```\n\n### Calculate a checksum with raw registers\n\n#### Register\n\n```python\nfrom crc import Crc8, Register\n\nexpected = 0xBC\ndata = bytes([0, 1, 2, 3, 4, 5])\nregister = Register(Crc8.CCITT)\n\nregister.init()\nregister.update(data)\nassert expected == register.digest()\n```\n#### TableBasedRegister\n\n```python\nfrom crc import Crc8, TableBasedRegister\n\nexpected = 0xBC\ndata = bytes([0, 1, 2, 3, 4, 5])\nregister = TableBasedRegister(Crc8.CCITT)\n\nregister.init()\nregister.update(data)\nassert expected == register.digest()\n```\n\nReferences & Resources\n-----------------------\n* [A Painless guide to crc error detection algorithms](http://www.zlib.net/crc_v3.txt)\n* [CRC-Catalogue](http://reveng.sourceforge.net/crc-catalogue/all.htm)\n\n',
+    'long_description': '<h1 align="center">CRC</h1>\n<p align="center">\n\nCalculate CRC checksums, verify CRC checksum, predefined CRC configurations, custom CRC configurations\n</p>\n\n<p align="center">\n\n<a href="https://github.com/Nicoretti/crc/actions">\n    <img src="https://img.shields.io/github/checks-status/nicoretti/crc/master" alt="Checks Master">\n</a>\n<a href="https://coveralls.io/github/Nicoretti/crc">\n    <img src="https://img.shields.io/coverallsCoverage/github/Nicoretti/crc" alt="Coverage">\n</a>\n<a href="https://opensource.org/licenses/BSD-2-Clause">\n    <img src="https://img.shields.io/pypi/l/crc" alt="License">\n</a>\n<a href="https://pypi.org/project/crc/">\n    <img src="https://img.shields.io/pypi/dm/crc" alt="Downloads">\n</a>\n<a href="https://pypi.org/project/crc/">\n    <img src="https://img.shields.io/pypi/pyversions/crc" alt="Supported Python Versions">\n</a>\n<a href="https://pypi.org/project/crc/">\n    <img src="https://img.shields.io/pypi/v/crc" alt="PyPi Package">\n</a>\n</p>\n\n---\n* Documentation: [https://nicoretti.github.io/crc](https://nicoretti.github.io/crc)\n* Source Code: [https://github.com/Nicoretti/crc](https://github.com/Nicoretti/crc)\n---\n\n## Available CRC Configurations\nFor convince various frequently used crc configurations ship with the library out of the box.\n\n| CRC8 | CRC16    | CRC32 | CRC64 |\n|------|----------|-------|-------|\n| CCITT | CCITT    | CRC32 | CRC64 |\n| AUTOSAR | GSM      | AUTOSAR | |\n| SAJ1850 | PROFIBUS | BZIP2 | |\n| BLUETOOTH | MODBUS   | POSIX | |\n| MAXIM-DOW |          | | | |\n\nIf you find yourself in the position, where having a new configuration available out of the\nbox would be desirable, feel free to create a [PR](https://github.com/Nicoretti/crc/pulls) or file an [issue](https://github.com/Nicoretti/crc/issues).\n\n## Custom Configurations\n\nIf you want to create a custom configuration, you should have the following information available:\n\n🗒 Note:\n\n    This library currently only supports bit widths of full bytes 8, 16, 24, 32, ...\n\n* **width**\n* **polynom**\n* **init value**\n* **final xor value**\n* **reversed input**\n* **reversed output**\n\nIn case you only have a name of a specific crc configuration/algorithm and you are unsure what are the specific parameters\nof it, a look into this [crc-catalogue](http://reveng.sourceforge.net/crc-catalogue/all.htm) might help.\n\n\n## Requirements\n* [\\>= Python 3.8](https://www.python.org)\n\n## Installation\n\n```shell\npip install crc\n```\n\n## Examples\n\n### Create a Calculator\n\n#### Pre defined configuration\n\n```python\nfrom crc import Calculator, Crc8\n\ncalculator = Calculator(Crc8.CCITT)\n```\n#### Custom configuration\n\n```python\nfrom crc import Calculator, Configuration\n\nconfig = Configuration(\n    width=8,\n    polynomial=0x07,\n    init_value=0x00,\n    final_xor_value=0x00,\n    reverse_input=False,\n    reverse_output=False,\n)\n\ncalculator = Calculator(config)\n```\n\n### Calculate a checksum\n\n#### Standard\n\n```python\nfrom crc import Calculator, Crc8\n\nexpected = 0xBC\ndata = bytes([0, 1, 2, 3, 4, 5])\ncalculator = Calculator(Crc8.CCITT)\n\nassert expected == calculator.checksum(data)\n```\n\n#### Optimized for speed\n\n```python\nfrom crc import Calculator, Crc8\n\nexpected = 0xBC\ndata = bytes([0, 1, 2, 3, 4, 5])\ncalculator = Calculator(Crc8.CCITT, optimized=True)\n\nassert expected == calculator.checksum(data)\n```\n\n### Verify a checksum\n\n#### Standard\n\n```python\nfrom crc import Calculator, Crc8\n\nexpected = 0xBC\ndata = bytes([0, 1, 2, 3, 4, 5])\ncalculator = Calculator(Crc8.CCITT)\n\nassert calculator.verify(data, expected)\n```\n\n#### Optimized for speed\n\n```python\nfrom crc import Calculator, Crc8\n\nexpected = 0xBC\ndata = bytes([0, 1, 2, 3, 4, 5])\ncalculator = Calculator(Crc8.CCITT, optimized=True)\n\nassert calculator.verify(data, expected)\n```\n\n### Calculate a checksum with raw registers\n\n#### Register\n\n```python\nfrom crc import Crc8, Register\n\nexpected = 0xBC\ndata = bytes([0, 1, 2, 3, 4, 5])\nregister = Register(Crc8.CCITT)\n\nregister.init()\nregister.update(data)\nassert expected == register.digest()\n```\n#### TableBasedRegister\n\n```python\nfrom crc import Crc8, TableBasedRegister\n\nexpected = 0xBC\ndata = bytes([0, 1, 2, 3, 4, 5])\nregister = TableBasedRegister(Crc8.CCITT)\n\nregister.init()\nregister.update(data)\nassert expected == register.digest()\n```\n\nReferences & Resources\n-----------------------\n* [A Painless guide to crc error detection algorithms](http://www.zlib.net/crc_v3.txt)\n* [CRC-Catalogue](http://reveng.sourceforge.net/crc-catalogue/all.htm)\n',
     'author': 'Nicola Coretti',
     'author_email': 'nico.coretti@gmail.com',
     'maintainer': 'Nicola Coretti',
     'maintainer_email': 'nico.coretti@gmail.com',
     'url': 'https://github.com/Nicoretti/crc',
     'py_modules': modules,
     'entry_points': entry_points,
```

#### html2text {}

```diff
@@ -1,49 +1,49 @@
 # -*- coding: utf-8 -*- from setuptools import setup modules = \ ['crc']
 entry_points = \ {'console_scripts': ['crc = crc:main']} setup_kwargs =
-{ 'name': 'crc', 'version': '4.1.0', 'description': 'Library and CLI to
+{ 'name': 'crc', 'version': '4.2.0', 'description': 'Library and CLI to
 calculate and verify all kinds of CRC checksums', 'long_description': '
                                ****** CRC ******
 \n
        \n\nCalculate CRC checksums, verify CRC checksum, predefined CRC
                   configurations, custom CRC configurations\n
 \n\n
 \n\n\n_[Checks_Master]\n\n\n_[Coverage]\n\n\n_[License]\n\n\n_[Downloads]\n\n\n
              [Supported_Python_Versions]\n\n\n_[PyPi_Package]\n\n
 \n\n---\n* Documentation: [https://nicoretti.github.io/crc](https://
 nicoretti.github.io/crc)\n* Source Code: [https://github.com/Nicoretti/crc]
 (https://github.com/Nicoretti/crc)\n---\n\n## Available CRC Configurations\nFor
 convince various frequently used crc configurations ship with the library out
-of the box.\n\n| CRC8 | CRC16 | CRC32 | CRC64 |\n|------|-------|-------|------
--|\n| CCITT | CCITT | CRC32 | CRC64 |\n| AUTOSAR | GSM | AUTOSAR | |\n| SAJ1850
-| PROFIBUS | BZIP2 | |\n| BLUETOOTH | | POSIX | |\n| MAXIM-DOW | | | | |\n\nIf
-you find yourself in the position, where having a new configuration available
-out of the\nbox would be desirable, feel free to create a [PR](https://
-github.com/Nicoretti/crc/pulls) or file an [issue](https://github.com/
-Nicoretti/crc/issues).\n\n## Custom Configurations\n\nIf you want to create a
-custom configuration, you should have the following information available:
-\n\nð Note: \n\n This library currently only supports bit widths of full
-bytes 8, 16, 24, 32, ...\n\n* **width**\n* **polynom**\n* **init value**\n*
-**final xor value**\n* **reversed input**\n* **reversed output**\n\nIn case you
-only have a name of a specific crc configuration/algorithm and you are unsure
-what are the specific parameters\nof it, a look into this [crc-catalogue](http:
-//reveng.sourceforge.net/crc-catalogue/all.htm) might help.\n\n\n##
-Requirements\n* [\\>= Python 3.8](https://www.python.org)\n\n##
-Installation\n\n```shell\npip install crc\n```\n\n## Examples\n\n### Create a
-Calculator\n\n#### Pre defined configuration\n\n```python\nfrom crc import
-Calculator, Crc8\n\ncalculator = Calculator(Crc8.CCITT)\n```\n#### Custom
-configuration\n\n```python\nfrom crc import Calculator, Configuration\n\nconfig
-= Configuration(\n width=8,\n polynomial=0x07,\n init_value=0x00,\n
-final_xor_value=0x00,\n reverse_input=False,\n
-reverse_output=False,\n)\n\ncalculator = Calculator(config)\n```\n\n###
-Calculate a checksum\n\n#### Standard\n\n```python\nfrom crc import Calculator,
-Crc8\n\nexpected = 0xBC\ndata = bytes([0, 1, 2, 3, 4, 5])\ncalculator =
-Calculator(Crc8.CCITT)\n\nassert expected == calculator.checksum
-(data)\n```\n\n#### Optimized for speed\n\n```python\nfrom crc import
-Calculator, Crc8\n\nexpected = 0xBC\ndata = bytes([0, 1, 2, 3, 4,
+of the box.\n\n| CRC8 | CRC16 | CRC32 | CRC64 |\n|------|----------|-------|---
+----|\n| CCITT | CCITT | CRC32 | CRC64 |\n| AUTOSAR | GSM | AUTOSAR | |\n|
+SAJ1850 | PROFIBUS | BZIP2 | |\n| BLUETOOTH | MODBUS | POSIX | |\n| MAXIM-DOW |
+| | | |\n\nIf you find yourself in the position, where having a new
+configuration available out of the\nbox would be desirable, feel free to create
+a [PR](https://github.com/Nicoretti/crc/pulls) or file an [issue](https://
+github.com/Nicoretti/crc/issues).\n\n## Custom Configurations\n\nIf you want to
+create a custom configuration, you should have the following information
+available:\n\nð Note:\n\n This library currently only supports bit widths of
+full bytes 8, 16, 24, 32, ...\n\n* **width**\n* **polynom**\n* **init
+value**\n* **final xor value**\n* **reversed input**\n* **reversed
+output**\n\nIn case you only have a name of a specific crc configuration/
+algorithm and you are unsure what are the specific parameters\nof it, a look
+into this [crc-catalogue](http://reveng.sourceforge.net/crc-catalogue/all.htm)
+might help.\n\n\n## Requirements\n* [\\>= Python 3.8](https://
+www.python.org)\n\n## Installation\n\n```shell\npip install crc\n```\n\n##
+Examples\n\n### Create a Calculator\n\n#### Pre defined
+configuration\n\n```python\nfrom crc import Calculator, Crc8\n\ncalculator =
+Calculator(Crc8.CCITT)\n```\n#### Custom configuration\n\n```python\nfrom crc
+import Calculator, Configuration\n\nconfig = Configuration(\n width=8,\n
+polynomial=0x07,\n init_value=0x00,\n final_xor_value=0x00,\n
+reverse_input=False,\n reverse_output=False,\n)\n\ncalculator = Calculator
+(config)\n```\n\n### Calculate a checksum\n\n#### Standard\n\n```python\nfrom
+crc import Calculator, Crc8\n\nexpected = 0xBC\ndata = bytes([0, 1, 2, 3, 4,
+5])\ncalculator = Calculator(Crc8.CCITT)\n\nassert expected ==
+calculator.checksum(data)\n```\n\n#### Optimized for speed\n\n```python\nfrom
+crc import Calculator, Crc8\n\nexpected = 0xBC\ndata = bytes([0, 1, 2, 3, 4,
 5])\ncalculator = Calculator(Crc8.CCITT, optimized=True)\n\nassert expected ==
 calculator.checksum(data)\n```\n\n### Verify a checksum\n\n####
 Standard\n\n```python\nfrom crc import Calculator, Crc8\n\nexpected =
 0xBC\ndata = bytes([0, 1, 2, 3, 4, 5])\ncalculator = Calculator
 (Crc8.CCITT)\n\nassert calculator.verify(data, expected)\n```\n\n#### Optimized
 for speed\n\n```python\nfrom crc import Calculator, Crc8\n\nexpected =
 0xBC\ndata = bytes([0, 1, 2, 3, 4, 5])\ncalculator = Calculator(Crc8.CCITT,
@@ -54,12 +54,12 @@
 (data)\nassert expected == register.digest()\n```\n####
 TableBasedRegister\n\n```python\nfrom crc import Crc8,
 TableBasedRegister\n\nexpected = 0xBC\ndata = bytes([0, 1, 2, 3, 4,
 5])\nregister = TableBasedRegister(Crc8.CCITT)\n\nregister.init
 ()\nregister.update(data)\nassert expected == register.digest
 ()\n```\n\nReferences & Resources\n-----------------------\n* [A Painless guide
 to crc error detection algorithms](http://www.zlib.net/crc_v3.txt)\n* [CRC-
-Catalogue](http://reveng.sourceforge.net/crc-catalogue/all.htm)\n\n', 'author':
+Catalogue](http://reveng.sourceforge.net/crc-catalogue/all.htm)\n', 'author':
 'Nicola Coretti', 'author_email': 'nico.coretti@gmail.com', 'maintainer':
 'Nicola Coretti', 'maintainer_email': 'nico.coretti@gmail.com', 'url': 'https:/
 /github.com/Nicoretti/crc', 'py_modules': modules, 'entry_points':
 entry_points, 'python_requires': '>=3.8,<4.0', } setup(**setup_kwargs)
```

### Comparing `crc-4.1.0/PKG-INFO` & `crc-4.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crc
-Version: 4.1.0
+Version: 4.2.0
 Summary: Library and CLI to calculate and verify all kinds of CRC checksums
 Home-page: https://github.com/Nicoretti/crc
 License: BSD-2-Clause
 Keywords: CRC,CRC8,CRC16,CRC32,CRC64
 Author: Nicola Coretti
 Author-email: nico.coretti@gmail.com
 Maintainer: Nicola Coretti
@@ -56,30 +56,30 @@
 * Documentation: [https://nicoretti.github.io/crc](https://nicoretti.github.io/crc)
 * Source Code: [https://github.com/Nicoretti/crc](https://github.com/Nicoretti/crc)
 ---
 
 ## Available CRC Configurations
 For convince various frequently used crc configurations ship with the library out of the box.
 
-| CRC8 | CRC16 | CRC32 | CRC64 |
-|------|-------|-------|-------|
-| CCITT | CCITT | CRC32 | CRC64 |
-| AUTOSAR | GSM | AUTOSAR | |
+| CRC8 | CRC16    | CRC32 | CRC64 |
+|------|----------|-------|-------|
+| CCITT | CCITT    | CRC32 | CRC64 |
+| AUTOSAR | GSM      | AUTOSAR | |
 | SAJ1850 | PROFIBUS | BZIP2 | |
-| BLUETOOTH | | POSIX | |
-| MAXIM-DOW | | | | |
+| BLUETOOTH | MODBUS   | POSIX | |
+| MAXIM-DOW |          | | | |
 
 If you find yourself in the position, where having a new configuration available out of the
 box would be desirable, feel free to create a [PR](https://github.com/Nicoretti/crc/pulls) or file an [issue](https://github.com/Nicoretti/crc/issues).
 
 ## Custom Configurations
 
 If you want to create a custom configuration, you should have the following information available:
 
-🗒 Note: 
+🗒 Note:
 
     This library currently only supports bit widths of full bytes 8, 16, 24, 32, ...
 
 * **width**
 * **polynom**
 * **init value**
 * **final xor value**
@@ -209,8 +209,7 @@
 ```
 
 References & Resources
 -----------------------
 * [A Painless guide to crc error detection algorithms](http://www.zlib.net/crc_v3.txt)
 * [CRC-Catalogue](http://reveng.sourceforge.net/crc-catalogue/all.htm)
 
-
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: crc Version: 4.1.0 Summary: Library and CLI to
+Metadata-Version: 2.1 Name: crc Version: 4.2.0 Summary: Library and CLI to
 calculate and verify all kinds of CRC checksums Home-page: https://github.com/
 Nicoretti/crc License: BSD-2-Clause Keywords: CRC,CRC8,CRC16,CRC32,CRC64
 Author: Nicola Coretti Author-email: nico.coretti@gmail.com Maintainer: Nicola
 Coretti Maintainer-email: nico.coretti@gmail.com Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: BSD License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
@@ -18,49 +18,49 @@
                            custom CRC configurations
  [Checks_Master] [Coverage] [License] [Downloads] [Supported_Python_Versions]
                                 [PyPi_Package]
 --- * Documentation: [https://nicoretti.github.io/crc](https://
 nicoretti.github.io/crc) * Source Code: [https://github.com/Nicoretti/crc]
 (https://github.com/Nicoretti/crc) --- ## Available CRC Configurations For
 convince various frequently used crc configurations ship with the library out
-of the box. | CRC8 | CRC16 | CRC32 | CRC64 | |------|-------|-------|-------| |
-CCITT | CCITT | CRC32 | CRC64 | | AUTOSAR | GSM | AUTOSAR | | | SAJ1850 |
-PROFIBUS | BZIP2 | | | BLUETOOTH | | POSIX | | | MAXIM-DOW | | | | | If you
-find yourself in the position, where having a new configuration available out
-of the box would be desirable, feel free to create a [PR](https://github.com/
-Nicoretti/crc/pulls) or file an [issue](https://github.com/Nicoretti/crc/
-issues). ## Custom Configurations If you want to create a custom configuration,
-you should have the following information available: ð Note: This library
-currently only supports bit widths of full bytes 8, 16, 24, 32, ... * **width**
-* **polynom** * **init value** * **final xor value** * **reversed input** *
-**reversed output** In case you only have a name of a specific crc
-configuration/algorithm and you are unsure what are the specific parameters of
-it, a look into this [crc-catalogue](http://reveng.sourceforge.net/crc-
-catalogue/all.htm) might help. ## Requirements * [\>= Python 3.8](https://
-www.python.org) ## Installation ```shell pip install crc ``` ## Examples ###
-Create a Calculator #### Pre defined configuration ```python from crc import
-Calculator, Crc8 calculator = Calculator(Crc8.CCITT) ``` #### Custom
-configuration ```python from crc import Calculator, Configuration config =
-Configuration( width=8, polynomial=0x07, init_value=0x00, final_xor_value=0x00,
-reverse_input=False, reverse_output=False, ) calculator = Calculator(config)
-``` ### Calculate a checksum #### Standard ```python from crc import
-Calculator, Crc8 expected = 0xBC data = bytes([0, 1, 2, 3, 4, 5]) calculator =
-Calculator(Crc8.CCITT) assert expected == calculator.checksum(data) ``` ####
-Optimized for speed ```python from crc import Calculator, Crc8 expected = 0xBC
-data = bytes([0, 1, 2, 3, 4, 5]) calculator = Calculator(Crc8.CCITT,
-optimized=True) assert expected == calculator.checksum(data) ``` ### Verify a
+of the box. | CRC8 | CRC16 | CRC32 | CRC64 | |------|----------|-------|-------
+| | CCITT | CCITT | CRC32 | CRC64 | | AUTOSAR | GSM | AUTOSAR | | | SAJ1850 |
+PROFIBUS | BZIP2 | | | BLUETOOTH | MODBUS | POSIX | | | MAXIM-DOW | | | | | If
+you find yourself in the position, where having a new configuration available
+out of the box would be desirable, feel free to create a [PR](https://
+github.com/Nicoretti/crc/pulls) or file an [issue](https://github.com/
+Nicoretti/crc/issues). ## Custom Configurations If you want to create a custom
+configuration, you should have the following information available: ð Note:
+This library currently only supports bit widths of full bytes 8, 16, 24, 32,
+... * **width** * **polynom** * **init value** * **final xor value** *
+**reversed input** * **reversed output** In case you only have a name of a
+specific crc configuration/algorithm and you are unsure what are the specific
+parameters of it, a look into this [crc-catalogue](http://
+reveng.sourceforge.net/crc-catalogue/all.htm) might help. ## Requirements *
+[\>= Python 3.8](https://www.python.org) ## Installation ```shell pip install
+crc ``` ## Examples ### Create a Calculator #### Pre defined configuration
+```python from crc import Calculator, Crc8 calculator = Calculator(Crc8.CCITT)
+``` #### Custom configuration ```python from crc import Calculator,
+Configuration config = Configuration( width=8, polynomial=0x07,
+init_value=0x00, final_xor_value=0x00, reverse_input=False,
+reverse_output=False, ) calculator = Calculator(config) ``` ### Calculate a
 checksum #### Standard ```python from crc import Calculator, Crc8 expected =
 0xBC data = bytes([0, 1, 2, 3, 4, 5]) calculator = Calculator(Crc8.CCITT)
-assert calculator.verify(data, expected) ``` #### Optimized for speed ```python
-from crc import Calculator, Crc8 expected = 0xBC data = bytes([0, 1, 2, 3, 4,
-5]) calculator = Calculator(Crc8.CCITT, optimized=True) assert
-calculator.verify(data, expected) ``` ### Calculate a checksum with raw
-registers #### Register ```python from crc import Crc8, Register expected =
-0xBC data = bytes([0, 1, 2, 3, 4, 5]) register = Register(Crc8.CCITT)
-register.init() register.update(data) assert expected == register.digest() ```
-#### TableBasedRegister ```python from crc import Crc8, TableBasedRegister
-expected = 0xBC data = bytes([0, 1, 2, 3, 4, 5]) register = TableBasedRegister
-(Crc8.CCITT) register.init() register.update(data) assert expected ==
-register.digest() ``` References & Resources ----------------------- * [A
-Painless guide to crc error detection algorithms](http://www.zlib.net/
+assert expected == calculator.checksum(data) ``` #### Optimized for speed
+```python from crc import Calculator, Crc8 expected = 0xBC data = bytes([0, 1,
+2, 3, 4, 5]) calculator = Calculator(Crc8.CCITT, optimized=True) assert
+expected == calculator.checksum(data) ``` ### Verify a checksum #### Standard
+```python from crc import Calculator, Crc8 expected = 0xBC data = bytes([0, 1,
+2, 3, 4, 5]) calculator = Calculator(Crc8.CCITT) assert calculator.verify(data,
+expected) ``` #### Optimized for speed ```python from crc import Calculator,
+Crc8 expected = 0xBC data = bytes([0, 1, 2, 3, 4, 5]) calculator = Calculator
+(Crc8.CCITT, optimized=True) assert calculator.verify(data, expected) ``` ###
+Calculate a checksum with raw registers #### Register ```python from crc import
+Crc8, Register expected = 0xBC data = bytes([0, 1, 2, 3, 4, 5]) register =
+Register(Crc8.CCITT) register.init() register.update(data) assert expected ==
+register.digest() ``` #### TableBasedRegister ```python from crc import Crc8,
+TableBasedRegister expected = 0xBC data = bytes([0, 1, 2, 3, 4, 5]) register =
+TableBasedRegister(Crc8.CCITT) register.init() register.update(data) assert
+expected == register.digest() ``` References & Resources ----------------------
+- * [A Painless guide to crc error detection algorithms](http://www.zlib.net/
 crc_v3.txt) * [CRC-Catalogue](http://reveng.sourceforge.net/crc-catalogue/
 all.htm)
```

