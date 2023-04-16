# Comparing `tmp/crcengine-0.4.0.tar.gz` & `tmp/crcengine-0.4a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crcengine-0.4.0.tar", max compression
+gzip compressed data, was "crcengine-0.4a2.tar", max compression
```

## Comparing `crcengine-0.4.0.tar` & `crcengine-0.4a2.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0    35149 2019-11-20 00:22:26.746553 crcengine-0.4.0/LICENSE
--rw-r--r--   0        0        0     1568 2023-04-16 19:42:38.904253 crcengine-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     4709 2023-04-16 16:19:57.461023 crcengine-0.4.0/README.rst
--rw-r--r--   0        0        0     2196 2023-04-16 19:24:52.211690 crcengine-0.4.0/src/crcengine/__init__.py
--rw-r--r--   0        0        0     4841 2023-04-16 16:19:57.516051 crcengine-0.4.0/src/crcengine/__main__.py
--rw-r--r--   0        0        0     9635 2023-04-16 19:24:52.211690 crcengine-0.4.0/src/crcengine/algorithms.py
--rw-r--r--   0        0        0    26155 2023-04-16 19:24:52.211690 crcengine-0.4.0/src/crcengine/calc.py
--rw-r--r--   0        0        0    26198 2023-04-16 17:37:45.621759 crcengine-0.4.0/src/crcengine/calc.py.bak
--rw-r--r--   0        0        0     7979 2023-04-16 16:19:57.522054 crcengine-0.4.0/src/crcengine/codegen.py
--rw-r--r--   0        0        0     1300 2022-06-29 00:12:05.496134 crcengine-0.4.0/src/crcengine/templates/c_template
--rw-r--r--   0        0        0      291 2020-01-30 21:41:28.593946 crcengine-0.4.0/src/crcengine/templates/h_template
--rw-r--r--   0        0        0      458 2021-04-11 18:09:19.465181 crcengine-0.4.0/src/crcengine/templates/test_template
--rw-r--r--   0        0        0     5835 1970-01-01 00:00:00.000000 crcengine-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2019-11-13 08:29:00.381942 crcengine-0.4a2/LICENSE
+-rw-r--r--   0        0        0     1570 2023-04-15 23:37:54.480008 crcengine-0.4a2/pyproject.toml
+-rw-r--r--   0        0        0     4709 2023-04-15 23:26:27.574057 crcengine-0.4a2/README.rst
+-rw-r--r--   0        0        0     1972 2023-04-15 23:26:27.589686 crcengine-0.4a2/src/crcengine/__init__.py
+-rw-r--r--   0        0        0     4841 2023-04-15 23:26:27.589686 crcengine-0.4a2/src/crcengine/__main__.py
+-rw-r--r--   0        0        0     9245 2023-04-15 23:26:27.589686 crcengine-0.4a2/src/crcengine/algorithms.py
+-rw-r--r--   0        0        0    23912 2023-04-15 23:26:27.589686 crcengine-0.4a2/src/crcengine/calc.py
+-rw-r--r--   0        0        0     7979 2023-04-15 23:26:27.589686 crcengine-0.4a2/src/crcengine/codegen.py
+-rw-r--r--   0        0        0     1300 2023-04-15 23:26:27.589686 crcengine-0.4a2/src/crcengine/templates/c_template
+-rw-r--r--   0        0        0      291 2019-12-21 11:49:25.832968 crcengine-0.4a2/src/crcengine/templates/h_template
+-rw-r--r--   0        0        0      458 2021-04-05 22:32:42.944797 crcengine-0.4a2/src/crcengine/templates/test_template
+-rw-r--r--   0        0        0     5835 1970-01-01 00:00:00.000000 crcengine-0.4a2/PKG-INFO
```

### Comparing `crcengine-0.4.0/LICENSE` & `crcengine-0.4a2/LICENSE`

 * *Files identical despite different names*

### Comparing `crcengine-0.4.0/pyproject.toml` & `crcengine-0.4a2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,21 @@
 build-backend = "poetry.core.masonry.api"
 
 # Old build system settings for setuptools
 #[build-system]
 #requires = ["setuptools", "wheel"]
 #build-backend = "setuptools.build_meta"
 
+[tool.isort]
+profile = "black"
+multi_line_output = 3
+
 [tool.poetry]
 name = "crcengine"
-version = "0.4.0"
+version = "0.4a2"
 description = "A library for CRC calculation and code generation"
 authors = [ "Garden Tools <gardensofdorwinion@gmail.com>"]
 license = "GPL-3.0-only"
 readme = "README.rst"
 repository = "https://github.com/GardenTools/crcengine"
 documentation = "https://crcengine.readthedocs.io/en/latest/"
 keywords = ["crcengine", "CRC", "cyclic", "redundancy", "check", "checksum", "code-generation", "Castagnoli", "CRC32", "CRC16-CCITT"]
@@ -43,11 +47,7 @@
 twine  = "*" # not sure this is still needed
 
 [tool.poetry.group.docs.dependencies]
 sphinx = "^5.0"
 
 [tool.poetry.scripts]
 crcengine = "crcengine.__main__:main"
-
-[tool.isort]
-profile = "black"
-multi_line_output = 3
```

### Comparing `crcengine-0.4.0/README.rst` & `crcengine-0.4a2/README.rst`

 * *Files identical despite different names*

### Comparing `crcengine-0.4.0/src/crcengine/__init__.py` & `crcengine-0.4a2/src/crcengine/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,70 +16,60 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with crcengine.  If not, see <https://www.gnu.org/licenses/>.
 
 try:
     # python 3.8 onwards
-    from importlib import metadata as importlib_metadata  # type:ignore
+    from importlib import metadata as importlib_metadata
 except ImportError:
     # python 3.7 support
-    import importlib_metadata  # type:ignore
+    import importlib_metadata # type:ignore
 
 __version__ = importlib_metadata.version('crcengine')
 
 from .algorithms import (
     AlgorithmNotFoundError,
     algorithms_available,
     CrcParams,
     get_algorithm_params,
     lookup_params,
     register_algorithm,
-    register_algorithm_params,
     unregister_algorithm,
 )
 from .calc import (
     available_calculation_engines,
     bit_reverse_byte,
     bit_reverse_n,
     create,
-    create_from_params,
     create_generic,
     create_lsb_table,
     create_msb_table,
     generic_crc,
     get_bits_max_value,
     new,
     table_crc,
 )
 
-from .codegen import (
-    generate_code,
-    generate_test
-)
-
+from .import codegen
 
 __all__ = [
     "AlgorithmNotFoundError",
     "algorithms_available",
     "available_calculation_engines",
     "bit_reverse_byte",
     "bit_reverse_n",
     "codegen",
     "CrcParams",
     "create",
-    "create_from_params",
     "create_generic",
     "create_lsb_table",
     "create_msb_table",
     "generic_crc",
-    "generate_code",
-    "generate_test",
     "get_algorithm_params",
     "get_bits_max_value",
     "lookup_params",
     "new",
     "register_algorithm",
-    "register_algorithm_params",
     "table_crc",
     "unregister_algorithm",
 ]
```

### Comparing `crcengine-0.4.0/src/crcengine/__main__.py` & `crcengine-0.4a2/src/crcengine/__main__.py`

 * *Files identical despite different names*

### Comparing `crcengine-0.4.0/src/crcengine/algorithms.py` & `crcengine-0.4a2/src/crcengine/algorithms.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     polynomial: int
     width: int
     seed: int
     reflect_in: bool
     reflect_out: bool
     xor_out: int
 
-    def validate(self) -> None:
+    def validate(self) -> bool:
         """raise an `InvalidParametersError` if the specified CRC parameters are
         not mutually consistent"""
         mask = (1 << self.width) - 1
         if (
                 ((self.polynomial & mask) != self.polynomial)
                 or ((self.seed & mask) != self.seed)
                 or ((self.xor_out & mask) != self.xor_out)
@@ -190,29 +190,15 @@
 
 def algorithms_available() -> Iterable[str]:
     """Obtain an iterable of available named CRC algorithms"""
     yield from _ALGORITHMS.keys()
     yield from _registered_algorithms.keys()
 
 
-def register_algorithm(name, polynomial, width, seed, reflect, xor_out, check=0):
-    """Register a CRC algorithm with custom parameters"""
-    poly_mask = (1 << width) - 1
-    _registered_algorithms[name] = (
-        polynomial & poly_mask,
-        width,
-        seed & poly_mask,
-        reflect,
-        reflect,
-        xor_out & poly_mask,
-        check,
-    )
-
-
-def register_algorithm_params(name: str, params: CrcParams, check=None) -> None:
+def register_algorithm(name: str, params: CrcParams, check=None) -> None:
     """Register a CRC algorithm with custom parameters"""
     poly_mask = (1 << params.width) - 1
     _registered_algorithms[name] = (
         params.polynomial & poly_mask,
         params.width,
         params.seed & poly_mask,
         params.reflect_in,
```

### Comparing `crcengine-0.4.0/src/crcengine/calc.py` & `crcengine-0.4a2/src/crcengine/calc.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with crcengine.  If not, see <https://www.gnu.org/licenses/>.
 
-from typing import Iterable, Optional
+from typing import Iterable
 import warnings
 
 from .algorithms import CrcParams, lookup_params
 
 _BYTEBITS = 8
 _DEFAULT_ENGINE = "table"
 
@@ -126,14 +126,21 @@
     """Generic most-significant-bit-first table-driven CRC calculation, allows
     unusual (and probably not useful) combinations of parameters such as
     reflecting the input without reflecting the output
     """
     def __init__(self, params: CrcParams, name=""):
         """
 
+        :param poly: polynomial representation, has implicit leading 1 bit
+        :param width:
+        :param seed:
+        :param ref_in:
+        :param ref_out:
+        :param xor_out:
+        :param name:
         """
         self._poly = params.polynomial
         self._width = params.width
         self._default_seed = params.seed
         self._xor_out = params.xor_out
         self._result_mask = (1 << params.width) - 1
 
@@ -303,23 +310,23 @@
             block_width -= first_bit
         return input_byte, block_width
 
     def __call__(self, data):
         return self.calculate(data)
 
 
-class _GenericReflectingLsbCrc:
+class _GenericLsbfCrc:
     """General purpose CRC calculation using LSB algorithm. Mainly here for
     reference, since the other algorithms cover all useful calculation combinations
     """
     # pylint: disable=too-many-arguments
-    def __init__(self, polynomial, width, seed, ref_in, ref_out, xor_out, name=""):
-        self._poly = polynomial
+    def __init__(self, lsb_poly, width, lsb_seed, ref_in, ref_out, xor_out, name=""):
+        self._poly = lsb_poly
         self._width = width
-        self._seed = seed
+        self._seed = lsb_seed
         self._xor_out = xor_out
         self._result_mask = (1 << width) - 1
         self._msbit = 1 << (width - 1)
         self._msb_lshift = width - 8
         self._ref_in = ref_in
         self._ref_out = ref_out
         self.name = name
@@ -327,16 +334,18 @@
     def calculate(self, data, seed=None):
         """Calculate a CRC on data
 
         :param data: bytes string whose CRC will be calculated
         :param seed: Optional seed
         :return: calculated CRC
         """
-        crc = seed if seed is not None else self._seed
-
+        if seed is not None:
+            crc = seed
+        else:
+            crc = self._seed
         if self._ref_in:
             poly = bit_reverse_n(self._poly, self._width)
         else:
             poly = self._poly
         for byte in data:
             if self._ref_in:
                 byte = _REV8BITS[byte]
@@ -357,15 +366,15 @@
 
 
 def new(name: str, calc_engine=_DEFAULT_ENGINE):
     """Create a new CRC calculation instance"""
     params = lookup_params(name)
     # the check field is not part of the definition, remove it before
     # creating the algorithm
-    algorithm = create_from_params(params, calc_engine)
+    algorithm = create(params, calc_engine)
     algorithm.name = name
     return algorithm
 
 
 @typing.no_type_check
 def table_crc(params: CrcParams):
     """Return a table-based CRC algorithm corresponding to `params`
@@ -379,70 +388,27 @@
 
     reverse_result = params.reflect_in != params.reflect_out
     algorithm = crc_class(table, params.width, params.seed, xor_out=params.xor_out,
                           reverse_result=reverse_result)
     return algorithm
 
 
-def create_from_params(params: CrcParams, calc_engine=_DEFAULT_ENGINE):
+def create(params: CrcParams, calc_engine=_DEFAULT_ENGINE):
     """Create a CRC calculation algorithm instance based on `params` using
     calculation engine `calc_engine` as the back end
 
     :param params:
     :param calc_engine:
     :return:
     """
     params.validate()
     creator_fun = _CREATOR_FUNCS[calc_engine]
     return creator_fun(params)
 
 
-def create(poly=None, width=None, seed=None,  # pylint: disable=too-many-arguments
-        ref_in=True, ref_out=True, name="", xor_out=0xFFFFFF, params: Optional[CrcParams] = None,
-        calc_engine=_DEFAULT_ENGINE):
-    """Create a table-driven CRC calculation engine
-
-    :param poly: polynomial (deprecated)
-    :param width: polynomial width in bits (deprecated)
-    :param seed: seed value for the CRC calculation to use (deprecated)
-    :param ref_in:  reflect input bits (deprecated)
-    :param ref_out: reflect output bits (deprecated)
-    :param name: associate a name with this algorithm (deprecated)
-    :param xor_out:  exclusive-or the output with this value (deprecated)
-    :param params: CRC parameters, same as specifying individual parameters
-    :param calc_engine: back-end calculation engine to use
-    :return:
-    """
-    if (params is not None) and (poly is None) and (width is None) and (seed is None):
-        if not isinstance(params, CrcParams):
-            raise ValueError("create: `params` must be a CrcParams")
-        return create_from_params(params, calc_engine)
-    if (params is None) and (poly is not None) and (width is not None) and (seed is not None):
-        warnings.warn("Passing separate parameters for poly, width and seed is"
-                      " deprecated, pass CrcParams instead", DeprecationWarning)
-        return _create_old(int(poly), int(width), int(seed), bool(ref_in), bool(ref_out), name,
-                           xor_out)
-    raise ValueError(f"Must specify either `params` ({params})"
-                     f" or `poly` ({poly}), `width` ({width}) and `seed` ({seed})")
-
-
-def _create_old(poly, width, seed, ref_in, ref_out, name, xor_out, ):
-    if ref_in:
-        table = create_lsb_table(poly, width)
-        algorithm = _ReflectedTableCrc(
-            table, width, seed, reverse_result=(ref_in != ref_out), xor_out=xor_out, name=name,
-        )
-    else:
-        table = create_msb_table(poly, width)
-        algorithm = _CrcMsbfTable(
-            table, width, seed, reverse_result=ref_out, xor_out=xor_out, name=name
-        )
-    return algorithm
-
-
 def create_generic(poly: int, width: int, seed: int, ref_in: bool, ref_out: bool,
                    xor_out: int, name=""):
     """Create generic non-table-driven CRC calculator
 
     :param poly: Polynomial
     :param width: calculator width in bits e.g. 32
     :param seed: calculation seed value
@@ -450,15 +416,15 @@
     :param ref_out: reflect result bits
     :param name: name to assign to calculator
     :param xor_out: pattern to XOR into result
     :return: A CRC calculation engine
     """
     warnings.warn("Use generic_crc instead of create_generic", DeprecationWarning)
     params = CrcParams(poly, width, seed, ref_in, ref_out, xor_out)
-    return _CrcGeneric(params, name)
+    return _CrcGeneric(params)
 
 
 def generic_crc(params: CrcParams):
     """Return a general-purpose MSB-first CRC algorithm
 
     :param params: CRC algorithm parameters
     :return: CRC algorithm
@@ -471,34 +437,21 @@
     and bit-length window to be specified on the CRC calculation
 
     :return: A CRC calculation engine
     """
     return _WindowedCrc(params)
 
 
-def create_generic_lsbf(
-    poly, width, seed, ref_in=True, ref_out=True, name="", xor_out=0xFFFFFF
-):
+def generic_lsb_first(lsb_poly, width, lsb_seed, xor_out=0xFFFFFF):
     """Create a CRC calculation engine that uses the Least-significant first
-    algorithm, but does not reflect the polynomial. If you use this, reflect
-    the polynomial before passing it in"""
-    return _GenericReflectingLsbCrc(
-        poly, width, seed, ref_in=ref_in, ref_out=ref_out, xor_out=xor_out, name=name
-    )
-
-
-def _create_reflecting_lsbf(params: CrcParams):
-    return _GenericReflectingLsbCrc(
-        params.polynomial,
-        params.width,
-        params.seed,
-        params.reflect_in,
-        params.reflect_out,
-        params.xor_out
-    )
+    algorithm, but does not reflect the polynomial or seed value. If you use
+    this, reflect the polynomial before passing it in
+    """
+    return _GenericLsbfCrc(
+        lsb_poly, width, lsb_seed, ref_in=False, ref_out=False, xor_out=xor_out)
 
 
 def create_msb_table_individual(poly, width):
     """Generate a CRC table calculating each entry.
     Mainly for demonstration and test, since calculate_msb_table() is
     much more efficient at calculating the same information
     :return: Generated table
@@ -516,17 +469,17 @@
                 crc <<= 1
         table[index] = crc & result_mask
     return table
 
 
 _CREATOR_FUNCS = {
     "table": table_crc,
-    "generic": generic_crc,
-    "generic_msbf": generic_crc,
-    "generic_lsbf": _create_reflecting_lsbf,
+    "generic": create_generic,
+    "generic_msbf": create_generic,
+    "generic_lsbf": generic_lsb_first,
     "windowed": windowed_crc,
 }
 
 
 def available_calculation_engines() -> Iterable[str]:
     """Return the list of available calculation back-ends. These can be used
     with :meth:`crcengine.create()`
```

### Comparing `crcengine-0.4.0/src/crcengine/codegen.py` & `crcengine-0.4a2/src/crcengine/codegen.py`

 * *Files identical despite different names*

### Comparing `crcengine-0.4.0/src/crcengine/templates/c_template` & `crcengine-0.4a2/src/crcengine/templates/c_template`

 * *Files identical despite different names*

### Comparing `crcengine-0.4.0/PKG-INFO` & `crcengine-0.4a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crcengine
-Version: 0.4.0
+Version: 0.4a2
 Summary: A library for CRC calculation and code generation
 Home-page: https://github.com/GardenTools/crcengine
 License: GPL-3.0-only
 Keywords: crcengine,CRC,cyclic,redundancy,check,checksum,code-generation,Castagnoli,CRC32,CRC16-CCITT
 Author: Garden Tools
 Author-email: gardensofdorwinion@gmail.com
 Requires-Python: >=3.7.2,<4.0.0
```

