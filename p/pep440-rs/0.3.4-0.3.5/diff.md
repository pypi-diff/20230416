# Comparing `tmp/pep440_rs-0.3.4.tar.gz` & `tmp/pep440_rs-0.3.5.tar.gz`

## Comparing `pep440_rs-0.3.4.tar` & `pep440_rs-0.3.5.tar`

### file list

```diff
@@ -1,19 +1,15 @@
--rw-r--r--   0        0        0      841 1970-01-01 00:00:00.000000 pep440_rs-0.3.4/Cargo.toml
--rw-r--r--   0      501       20      208 2023-04-04 13:33:21.000000 pep440_rs-0.3.4/.github/dependabot.yml
--rw-r--r--   0      501       20     4386 2023-04-04 13:33:21.000000 pep440_rs-0.3.4/.github/workflows/release.yml
--rw-r--r--   0      501       20     1326 2023-04-04 13:33:21.000000 pep440_rs-0.3.4/.github/workflows/test.yml
--rw-r--r--   0      501       20       39 2023-04-04 13:33:21.000000 pep440_rs-0.3.4/.gitignore
--rw-r--r--   0      501       20      760 2023-04-04 13:33:21.000000 pep440_rs-0.3.4/Changelog.md
--rw-r--r--   0      501       20     2734 2023-04-04 13:33:21.000000 pep440_rs-0.3.4/README.md
--rw-r--r--   0      501       20     2734 2023-04-04 13:33:21.000000 pep440_rs-0.3.4/Readme.md
--rw-r--r--   0      501       20       10 2023-04-04 13:34:10.000000 pep440_rs-0.3.4/dist/pep440_rs-0.3.4.tar.gz
--rw-r--r--   0      501       20      274 2023-04-04 13:33:21.000000 pep440_rs-0.3.4/pyproject.toml
--rw-r--r--   0      501       20     2105 2023-04-04 13:33:21.000000 pep440_rs-0.3.4/python/Readme.md
--rw-r--r--   0      501       20      534 2023-04-04 13:33:21.000000 pep440_rs-0.3.4/python/pep440_rs/__init__.py
--rw-r--r--   0      501       20     1084 2023-04-04 13:33:21.000000 pep440_rs-0.3.4/python/pep440_rs/__init__.pyi
--rw-r--r--   0      501       20     4043 2023-04-04 13:33:21.000000 pep440_rs-0.3.4/src/lib.rs
--rw-r--r--   0      501       20    39057 2023-04-04 13:33:21.000000 pep440_rs-0.3.4/src/version.rs
--rw-r--r--   0      501       20    42027 2023-04-04 13:33:21.000000 pep440_rs-0.3.4/src/version_specifier.rs
--rw-r--r--   0      501       20     1436 2023-04-04 13:33:21.000000 pep440_rs-0.3.4/test/test_python.py
--rw-r--r--   0      501       20    11645 2023-04-04 13:33:21.000000 pep440_rs-0.3.4/Cargo.lock
--rw-r--r--   0        0        0     2410 1970-01-01 00:00:00.000000 pep440_rs-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0      917 1970-01-01 00:00:00.000000 pep440_rs-0.3.5/Cargo.toml
+-rw-r--r--   0      501       20      869 2023-04-16 16:42:50.000000 pep440_rs-0.3.5/Changelog.md
+-rw-r--r--   0      501       20    10173 2023-04-16 16:42:50.000000 pep440_rs-0.3.5/License-Apache
+-rw-r--r--   0      501       20     1293 2023-04-16 16:42:50.000000 pep440_rs-0.3.5/License-BSD
+-rw-r--r--   0      501       20     2978 2023-04-16 16:42:50.000000 pep440_rs-0.3.5/README.md
+-rw-r--r--   0      501       20     2978 2023-04-16 16:42:50.000000 pep440_rs-0.3.5/Readme.md
+-rw-r--r--   0      501       20      274 2023-04-16 16:42:50.000000 pep440_rs-0.3.5/pyproject.toml
+-rw-r--r--   0      501       20     2105 2023-04-16 16:42:50.000000 pep440_rs-0.3.5/python/Readme.md
+-rw-r--r--   0      501       20     4043 2023-04-16 16:42:50.000000 pep440_rs-0.3.5/src/lib.rs
+-rw-r--r--   0      501       20    39057 2023-04-16 16:42:50.000000 pep440_rs-0.3.5/src/version.rs
+-rw-r--r--   0      501       20    42526 2023-04-16 16:42:50.000000 pep440_rs-0.3.5/src/version_specifier.rs
+-rw-r--r--   0      501       20    10919 2023-04-16 16:42:50.000000 pep440_rs-0.3.5/Cargo.lock
+-rw-r--r--   0      501       20     1084 2023-04-16 16:42:50.000000 pep440_rs-0.3.5/python/pep440_rs/__init__.pyi
+-rw-r--r--   0      501       20      534 2023-04-16 16:42:50.000000 pep440_rs-0.3.5/python/pep440_rs/__init__.py
+-rw-r--r--   0        0        0     2410 1970-01-01 00:00:00.000000 pep440_rs-0.3.5/PKG-INFO
```

### Comparing `pep440_rs-0.3.4/Cargo.toml` & `pep440_rs-0.3.5/Cargo.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [package]
 name = "pep440_rs"
-version = "0.3.4"
+version = "0.3.5"
 description = "A library for python version numbers and specifiers, implementing PEP 440"
 edition = "2021"
 # Same license as pypa/packaging where the tests are from
 license = "Apache-2.0 OR BSD-2-Clause"
 repository = "https://github.com/konstin/pep440-rs"
-
+include = ["/src", "Changelog.md", "License-Apache", "License-BSD", "Readme.md", "pyproject.toml"]
 
 [lib]
 name = "pep440_rs"
 crate-type = ["rlib", "cdylib"]
 
 [dependencies]
 lazy_static = "1.4.0"
-pyo3 = { version = "0.18.2", optional = true, features = ["extension-module", "abi3-py37", "multiple-pymethods"] }
+pyo3 = { version = "0.18.2", optional = true, features = ["extension-module", "abi3-py37"] }
 regex = { version = "1.7.0", default-features = false, features = ["std", "perf", "unicode-case", "unicode-perl"] }
 serde = { version = "1.0.150", features = ["derive"], optional = true }
 tracing = "0.1.37"
 unicode-width = "0.1.10"
 
 [dev-dependencies]
 indoc = "2.0.1"
```

### Comparing `pep440_rs-0.3.4/Changelog.md` & `pep440_rs-0.3.5/Changelog.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+## 0.3.5
+
+* Make string serialization look more like poetry's
+* Implement `__hash__` for `VersionSpecifier`
+
 ## 0.3.4
 
 * Python bindings for `VersionSpecifiers`
 
 ## 0.3.3
 
 * Implement `Display` for `VersionSpecifiers`
```

### Comparing `pep440_rs-0.3.4/README.md` & `pep440_rs-0.3.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # PEP440 in rust
 
+[![Crates.io](https://img.shields.io/crates/v/pep440_rs.svg?logo=rust&style=flat-square)](https://crates.io/crates/maturin)
+[![PyPI](https://img.shields.io/pypi/v/pep440_rs.svg?logo=python&style=flat-square)](https://pypi.org/project/maturin)
+
 A library for python version numbers and specifiers, implementing
 [PEP 440](https://peps.python.org/pep-0440). See [Reimplementing PEP 440](https://cohost.org/konstin/post/514863-reimplementing-pep-4) for some background.
 
 Higher level bindings to the requirements syntax are available in [pep508_rs](https://github.com/konstin/pep508_rs).
 
 ```rust
 use std::str::FromStr;
```

### Comparing `pep440_rs-0.3.4/Readme.md` & `pep440_rs-0.3.5/Readme.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # PEP440 in rust
 
+[![Crates.io](https://img.shields.io/crates/v/pep440_rs.svg?logo=rust&style=flat-square)](https://crates.io/crates/maturin)
+[![PyPI](https://img.shields.io/pypi/v/pep440_rs.svg?logo=python&style=flat-square)](https://pypi.org/project/maturin)
+
 A library for python version numbers and specifiers, implementing
 [PEP 440](https://peps.python.org/pep-0440). See [Reimplementing PEP 440](https://cohost.org/konstin/post/514863-reimplementing-pep-4) for some background.
 
 Higher level bindings to the requirements syntax are available in [pep508_rs](https://github.com/konstin/pep508_rs).
 
 ```rust
 use std::str::FromStr;
```

### Comparing `pep440_rs-0.3.4/python/Readme.md` & `pep440_rs-0.3.5/python/Readme.md`

 * *Files identical despite different names*

### Comparing `pep440_rs-0.3.4/python/pep440_rs/__init__.py` & `pep440_rs-0.3.5/python/pep440_rs/__init__.py`

 * *Files identical despite different names*

### Comparing `pep440_rs-0.3.4/python/pep440_rs/__init__.pyi` & `pep440_rs-0.3.5/python/pep440_rs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pep440_rs-0.3.4/src/lib.rs` & `pep440_rs-0.3.5/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pep440_rs-0.3.4/src/version.rs` & `pep440_rs-0.3.5/src/version.rs`

 * *Files identical despite different names*

### Comparing `pep440_rs-0.3.4/src/version_specifier.rs` & `pep440_rs-0.3.5/src/version_specifier.rs`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,20 @@
     pyclass::CompareOp,
     pymethods, Py, PyRef, PyRefMut, PyResult,
 };
 use regex::Regex;
 #[cfg(feature = "serde")]
 use serde::{de, Deserialize, Deserializer, Serialize, Serializer};
 use std::cmp::Ordering;
+#[cfg(feature = "pyo3")]
+use std::collections::hash_map::DefaultHasher;
 use std::fmt::Formatter;
 use std::fmt::{Debug, Display};
+#[cfg(feature = "pyo3")]
+use std::hash::{Hash, Hasher};
 use std::ops::Deref;
 use std::str::FromStr;
 use tracing::warn;
 use unicode_width::UnicodeWidthStr;
 
 lazy_static! {
     /// Matches a python version specifier, such as `>=1.19.a1` or `4.1.*`. Extends the PEP 440
@@ -211,14 +215,20 @@
     // Since we don't bring FromStr to python
     /// Parse a PEP 440 version
     #[new]
     pub fn parse(version_specifier: String) -> PyResult<Self> {
         Self::from_str(&version_specifier).map_err(PyValueError::new_err)
     }
 
+    /// See [VersionSpecifier::contains]
+    #[pyo3(name = "contains")]
+    pub fn py_contains(&self, version: &PyVersion) -> bool {
+        self.contains(&version.0)
+    }
+
     /// Whether the version fulfills the specifier
     pub fn __contains__(&self, version: &PyVersion) -> bool {
         self.contains(&version.0)
     }
 
     /// Returns the normalized representation
     pub fn __str__(&self) -> String {
@@ -235,14 +245,21 @@
             Ok(self == other)
         } else {
             Err(PyNotImplementedError::new_err(
                 "Can only compare VersionSpecifier by equality",
             ))
         }
     }
+
+    /// Returns the normalized representation
+    pub fn __hash__(&self) -> u64 {
+        let mut hasher = DefaultHasher::new();
+        self.hash(&mut hasher);
+        hasher.finish()
+    }
 }
 
 /// https://github.com/serde-rs/serde/issues/1316#issue-332908452
 #[cfg(feature = "serde")]
 impl<'de> Deserialize<'de> for VersionSpecifier {
     fn deserialize<D>(deserializer: D) -> Result<Self, D::Error>
     where
@@ -324,24 +341,14 @@
 
     /// Get the version, e.g. `<=` in `<= 2.0.0`
     pub fn version(&self) -> &Version {
         &self.version
     }
 }
 
-#[cfg(feature = "pyo3")]
-#[pymethods]
-impl VersionSpecifier {
-    /// See [VersionSpecifier::contains]
-    #[pyo3(name = "contains")]
-    pub fn py_contains(&self, version: &PyVersion) -> bool {
-        self.contains(&version.0)
-    }
-}
-
 impl VersionSpecifier {
     /// Whether the given version satisfies the version range
     ///
     /// e.g. `>=1.19,<2.0` and `1.21` -> true
     /// <https://peps.python.org/pep-0440/#version-specifiers>
     ///
     /// Unlike `pypa/packaging`, prereleases are included by default
@@ -479,18 +486,18 @@
         let version_specifier = VersionSpecifier::new(operator, version, star)?;
         Ok(version_specifier)
     }
 }
 
 impl Display for VersionSpecifier {
     fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
-        if self.operator == Operator::EqualStar {
-            return write!(f, "{} {}.*", Operator::Equal, self.version);
+        if self.operator == Operator::EqualStar || self.operator == Operator::NotEqualStar {
+            return write!(f, "{}{}.*", self.operator, self.version);
         }
-        write!(f, "{} {}", self.operator, self.version)
+        write!(f, "{}{}", self.operator, self.version)
     }
 }
 
 /// Parses a list of specifiers such as `>= 1.0, != 1.3.*, < 2.0`.
 ///
 /// I recommend using [VersionSpecifiers::from_str] instead.
 ///
@@ -1241,26 +1248,34 @@
             }
         }
     }
 
     #[test]
     fn test_display_start() {
         assert_eq!(
-            VersionSpecifier::from_str("== 1.1.*").unwrap().to_string(),
-            "== 1.1.*"
+            VersionSpecifier::from_str("==     1.1.*")
+                .unwrap()
+                .to_string(),
+            "==1.1.*"
+        );
+        assert_eq!(
+            VersionSpecifier::from_str("!=     1.1.*")
+                .unwrap()
+                .to_string(),
+            "!=1.1.*"
         );
     }
 
     #[test]
     fn test_version_specifiers_str() {
         assert_eq!(
-            VersionSpecifiers::from_str(">=3.7").unwrap().to_string(),
-            ">= 3.7"
+            VersionSpecifiers::from_str(">= 3.7").unwrap().to_string(),
+            ">=3.7"
         );
         assert_eq!(
-            VersionSpecifiers::from_str(">=3.7, <4.0, != 3.9.0")
+            VersionSpecifiers::from_str(">=3.7, <      4.0, != 3.9.0")
                 .unwrap()
                 .to_string(),
-            ">= 3.7, < 4.0, != 3.9.0"
+            ">=3.7, <4.0, !=3.9.0"
         );
     }
 }
```

### Comparing `pep440_rs-0.3.4/Cargo.lock` & `pep440_rs-0.3.5/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -26,57 +26,26 @@
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
-name = "ctor"
-version = "0.2.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dd4056f63fce3b82d852c3da92b08ea59959890813a7f4ce9c0ff85b10cf301b"
-dependencies = [
- "quote",
- "syn 2.0.13",
-]
-
-[[package]]
-name = "ghost"
-version = "0.1.9"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e77ac7b51b8e6313251737fcef4b1c01a2ea102bde68415b62c0ee9268fec357"
-dependencies = [
- "proc-macro2",
- "quote",
- "syn 2.0.13",
-]
-
-[[package]]
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "indoc"
 version = "2.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9f2cb48b81b1dc9f39676bf99f5499babfec7cd8fe14307f7b3d747208fb5690"
 
 [[package]]
-name = "inventory"
-version = "0.3.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7741301a6d6a9b28ce77c0fb77a4eb116b6bc8f3bef09923f7743d059c4157d3"
-dependencies = [
- "ctor",
- "ghost",
-]
-
-[[package]]
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
@@ -136,15 +105,15 @@
  "redox_syscall",
  "smallvec",
  "windows-sys",
 ]
 
 [[package]]
 name = "pep440_rs"
-version = "0.3.4"
+version = "0.3.5"
 dependencies = [
  "indoc 2.0.1",
  "lazy_static",
  "pyo3",
  "regex",
  "serde",
  "tracing",
@@ -170,15 +139,14 @@
 name = "pyo3"
 version = "0.18.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cfb848f80438f926a9ebddf0a539ed6065434fd7aae03a89312a9821f81b8501"
 dependencies = [
  "cfg-if",
  "indoc 1.0.9",
- "inventory",
  "libc",
  "memoffset",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
```

### Comparing `pep440_rs-0.3.4/PKG-INFO` & `pep440_rs-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pep440_rs
-Version: 0.3.4
+Version: 0.3.5
 Summary: A library for python version numbers and specifiers, implementing PEP 440
 License: Apache-2.0 OR BSD-2-Clause
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/konstin/pep440-rs
 
 # PEP440 in rust
```

