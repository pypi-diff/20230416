# Comparing `tmp/nazo_rand-0.0.5.tar.gz` & `tmp/nazo_rand-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nazo_rand-0.0.5.tar", last modified: Sat Apr 15 15:37:14 2023, max compression
+gzip compressed data, was "nazo_rand-0.0.6.tar", last modified: Sun Apr 16 12:37:35 2023, max compression
```

## Comparing `nazo_rand-0.0.5.tar` & `nazo_rand-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:37:14.293792 nazo_rand-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-15 15:36:54.000000 nazo_rand-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-15 15:36:54.000000 nazo_rand-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-04-15 15:37:14.293792 nazo_rand-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-15 15:36:54.000000 nazo_rand-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:37:14.293792 nazo_rand-0.0.5/nazo_rand/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-15 15:36:54.000000 nazo_rand-0.0.5/nazo_rand/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   205123 2023-04-15 15:37:04.000000 nazo_rand-0.0.5/nazo_rand/nazo_rand.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-15 15:36:54.000000 nazo_rand-0.0.5/nazo_rand/nazo_rand.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-15 15:36:54.000000 nazo_rand-0.0.5/nazo_rand/nazo_rand.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-04-15 15:36:54.000000 nazo_rand-0.0.5/nazo_rand/nazo_rand.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-15 15:36:54.000000 nazo_rand-0.0.5/nazo_rand/nazo_rand.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:37:14.293792 nazo_rand-0.0.5/nazo_rand.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-04-15 15:37:14.000000 nazo_rand-0.0.5/nazo_rand.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-15 15:37:14.000000 nazo_rand-0.0.5/nazo_rand.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 15:37:14.000000 nazo_rand-0.0.5/nazo_rand.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-15 15:37:14.000000 nazo_rand-0.0.5/nazo_rand.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-15 15:36:54.000000 nazo_rand-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 15:37:14.293792 nazo_rand-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-04-15 15:36:54.000000 nazo_rand-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:37:35.718857 nazo_rand-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-04-16 12:37:15.000000 nazo_rand-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-16 12:37:15.000000 nazo_rand-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-04-16 12:37:35.718857 nazo_rand-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-16 12:37:15.000000 nazo_rand-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:37:35.718857 nazo_rand-0.0.6/nazo_rand/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-16 12:37:15.000000 nazo_rand-0.0.6/nazo_rand/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   235337 2023-04-16 12:37:25.000000 nazo_rand-0.0.6/nazo_rand/nazo_rand.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-04-16 12:37:15.000000 nazo_rand-0.0.6/nazo_rand/nazo_rand.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-16 12:37:15.000000 nazo_rand-0.0.6/nazo_rand/nazo_rand.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-04-16 12:37:15.000000 nazo_rand-0.0.6/nazo_rand/nazo_rand.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-04-16 12:37:15.000000 nazo_rand-0.0.6/nazo_rand/nazo_rand.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 12:37:35.718857 nazo_rand-0.0.6/nazo_rand.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-04-16 12:37:35.000000 nazo_rand-0.0.6/nazo_rand.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-16 12:37:35.000000 nazo_rand-0.0.6/nazo_rand.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 12:37:35.000000 nazo_rand-0.0.6/nazo_rand.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-16 12:37:35.000000 nazo_rand-0.0.6/nazo_rand.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-16 12:37:15.000000 nazo_rand-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 12:37:35.718857 nazo_rand-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-04-16 12:37:15.000000 nazo_rand-0.0.6/setup.py
```

### Comparing `nazo_rand-0.0.5/LICENSE` & `nazo_rand-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nazo_rand-0.0.5/PKG-INFO` & `nazo_rand-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nazo_rand
-Version: 0.0.5
+Version: 0.0.6
 Summary: A fast random number generator for python
 Author: bymoye
 Author-email: s3moye@gmail.com
 License: Free for non-commercial use
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `nazo_rand-0.0.5/README.md` & `nazo_rand-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `nazo_rand-0.0.5/nazo_rand/nazo_rand.cpp` & `nazo_rand-0.0.6/nazo_rand/nazo_rand.cpp`

 * *Files 9% similar despite different names*

```diff
@@ -994,15 +994,15 @@
 static const char *__pyx_f[] = {
   "nazo_rand/nazo_rand.pyx",
 };
 
 /*--- Type declarations ---*/
 struct __pyx_opt_args_9nazo_rand_9nazo_rand_randrange;
 
-/* "nazo_rand/nazo_rand.pxd":10
+/* "nazo_rand/nazo_rand.pxd":12
  * cpdef int randbelow(int a)
  * cpdef int randint(int a,int b)
  * cpdef int randrange(int start,int stop=?,int step=?)             # <<<<<<<<<<<<<<
  * cpdef double random_double(double a, double b)
  * cpdef double random_double_noargs()
  */
 struct __pyx_opt_args_9nazo_rand_9nazo_rand_randrange {
@@ -1138,14 +1138,26 @@
 
 /* ArgTypeTest.proto */
 #define __Pyx_ArgTypeTest(obj, type, none_allowed, name, exact)\
     ((likely((Py_TYPE(obj) == type) | (none_allowed && (obj == Py_None)))) ? 1 :\
         __Pyx__ArgTypeTest(obj, type, name, exact))
 static int __Pyx__ArgTypeTest(PyObject *obj, PyTypeObject *type, const char *name, int exact);
 
+/* RaiseArgTupleInvalid.proto */
+static void __Pyx_RaiseArgtupleInvalid(const char* func_name, int exact,
+    Py_ssize_t num_min, Py_ssize_t num_max, Py_ssize_t num_found);
+
+/* RaiseDoubleKeywords.proto */
+static void __Pyx_RaiseDoubleKeywordsError(const char* func_name, PyObject* kw_name);
+
+/* ParseKeywords.proto */
+static int __Pyx_ParseOptionalKeywords(PyObject *kwds, PyObject **argnames[],\
+    PyObject *kwds2, PyObject *values[], Py_ssize_t num_pos_args,\
+    const char* function_name);
+
 /* GetItemInt.proto */
 #define __Pyx_GetItemInt(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
     (__Pyx_fits_Py_ssize_t(i, type, is_signed) ?\
     __Pyx_GetItemInt_Fast(o, (Py_ssize_t)i, is_list, wraparound, boundscheck) :\
     (is_list ? (PyErr_SetString(PyExc_IndexError, "list index out of range"), (PyObject*)NULL) :\
                __Pyx_GetItemInt_Generic(o, to_py_func(i))))
 #define __Pyx_GetItemInt_List(o, i, type, is_signed, to_py_func, is_list, wraparound, boundscheck)\
@@ -1160,25 +1172,40 @@
     (PyErr_SetString(PyExc_IndexError, "tuple index out of range"), (PyObject*)NULL))
 static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Tuple_Fast(PyObject *o, Py_ssize_t i,
                                                               int wraparound, int boundscheck);
 static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j);
 static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Fast(PyObject *o, Py_ssize_t i,
                                                      int is_list, int wraparound, int boundscheck);
 
-/* RaiseArgTupleInvalid.proto */
-static void __Pyx_RaiseArgtupleInvalid(const char* func_name, int exact,
-    Py_ssize_t num_min, Py_ssize_t num_max, Py_ssize_t num_found);
+/* ListCompAppend.proto */
+#if CYTHON_USE_PYLIST_INTERNALS && CYTHON_ASSUME_SAFE_MACROS
+static CYTHON_INLINE int __Pyx_ListComp_Append(PyObject* list, PyObject* x) {
+    PyListObject* L = (PyListObject*) list;
+    Py_ssize_t len = Py_SIZE(list);
+    if (likely(L->allocated > len)) {
+        Py_INCREF(x);
+        PyList_SET_ITEM(list, len, x);
+        __Pyx_SET_SIZE(list, len + 1);
+        return 0;
+    }
+    return PyList_Append(list, x);
+}
+#else
+#define __Pyx_ListComp_Append(L,x) PyList_Append(L,x)
+#endif
 
-/* RaiseDoubleKeywords.proto */
-static void __Pyx_RaiseDoubleKeywordsError(const char* func_name, PyObject* kw_name);
+/* PyObjectCall.proto */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw);
+#else
+#define __Pyx_PyObject_Call(func, arg, kw) PyObject_Call(func, arg, kw)
+#endif
 
-/* ParseKeywords.proto */
-static int __Pyx_ParseOptionalKeywords(PyObject *kwds, PyObject **argnames[],\
-    PyObject *kwds2, PyObject *values[], Py_ssize_t num_pos_args,\
-    const char* function_name);
+/* RaiseException.proto */
+static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
 
 /* FetchCommonType.proto */
 static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type);
 
 /* CythonFunctionShared.proto */
 #define __Pyx_CyFunction_USED 1
 #define __Pyx_CYFUNCTION_STATICMETHOD  0x01
@@ -1335,94 +1362,114 @@
 
 /* Module declarations from 'libc.stdint' */
 
 /* Module declarations from 'nazo_rand.nazo_rand' */
 static void __pyx_f_9nazo_rand_9nazo_rand_shuffle(PyObject *, int __pyx_skip_dispatch); /*proto*/
 static int __pyx_f_9nazo_rand_9nazo_rand_random_integer_noargs(int __pyx_skip_dispatch); /*proto*/
 static PyObject *__pyx_f_9nazo_rand_9nazo_rand_random_choice(PyObject *, int __pyx_skip_dispatch); /*proto*/
+static PyObject *__pyx_f_9nazo_rand_9nazo_rand_random_choices(PyObject *, Py_ssize_t, int __pyx_skip_dispatch); /*proto*/
+static PyObject *__pyx_f_9nazo_rand_9nazo_rand_random_sample(PyObject *, Py_ssize_t, int __pyx_skip_dispatch); /*proto*/
 static int __pyx_f_9nazo_rand_9nazo_rand_randbelow(int, int __pyx_skip_dispatch); /*proto*/
 static int __pyx_f_9nazo_rand_9nazo_rand_randint(int, int, int __pyx_skip_dispatch); /*proto*/
 static int __pyx_f_9nazo_rand_9nazo_rand_randrange(int, int __pyx_skip_dispatch, struct __pyx_opt_args_9nazo_rand_9nazo_rand_randrange *__pyx_optional_args); /*proto*/
 static double __pyx_f_9nazo_rand_9nazo_rand_random_double(double, double, int __pyx_skip_dispatch); /*proto*/
 static double __pyx_f_9nazo_rand_9nazo_rand_random_double_noargs(int __pyx_skip_dispatch); /*proto*/
 #define __Pyx_MODULE_NAME "nazo_rand.nazo_rand"
 extern int __pyx_module_is_main_nazo_rand__nazo_rand;
 int __pyx_module_is_main_nazo_rand__nazo_rand = 0;
 
 /* Implementation of 'nazo_rand.nazo_rand' */
 static PyObject *__pyx_builtin_reversed;
 static PyObject *__pyx_builtin_range;
+static PyObject *__pyx_builtin_ValueError;
 static const char __pyx_k_a[] = "a";
 static const char __pyx_k_b[] = "b";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_step[] = "step";
 static const char __pyx_k_stop[] = "stop";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_array[] = "array";
+static const char __pyx_k_count[] = "count";
 static const char __pyx_k_range[] = "range";
 static const char __pyx_k_start[] = "start";
 static const char __pyx_k_randint[] = "randint";
 static const char __pyx_k_shuffle[] = "shuffle";
-static const char __pyx_k_elements[] = "elements";
 static const char __pyx_k_reversed[] = "reversed";
+static const char __pyx_k_container[] = "container";
 static const char __pyx_k_randbelow[] = "randbelow";
 static const char __pyx_k_randrange[] = "randrange";
+static const char __pyx_k_ValueError[] = "ValueError";
 static const char __pyx_k_random_choice[] = "random_choice";
 static const char __pyx_k_random_double[] = "random_double";
+static const char __pyx_k_random_sample[] = "random_sample";
+static const char __pyx_k_random_choices[] = "random_choices";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_nazo_rand_nazo_rand[] = "nazo_rand.nazo_rand";
 static const char __pyx_k_random_double_noargs[] = "random_double_noargs";
 static const char __pyx_k_random_integer_noargs[] = "random_integer_noargs";
 static const char __pyx_k_nazo_rand_nazo_rand_pyx[] = "nazo_rand/nazo_rand.pyx";
+static const char __pyx_k_Sample_larger_than_population[] = "Sample larger than population";
+static PyObject *__pyx_kp_u_Sample_larger_than_population;
+static PyObject *__pyx_n_s_ValueError;
 static PyObject *__pyx_n_s_a;
 static PyObject *__pyx_n_s_array;
 static PyObject *__pyx_n_s_b;
 static PyObject *__pyx_n_s_cline_in_traceback;
-static PyObject *__pyx_n_s_elements;
+static PyObject *__pyx_n_s_container;
+static PyObject *__pyx_n_s_count;
 static PyObject *__pyx_n_s_main;
 static PyObject *__pyx_n_s_name;
 static PyObject *__pyx_n_s_nazo_rand_nazo_rand;
 static PyObject *__pyx_kp_s_nazo_rand_nazo_rand_pyx;
 static PyObject *__pyx_n_s_randbelow;
 static PyObject *__pyx_n_s_randint;
 static PyObject *__pyx_n_s_random_choice;
+static PyObject *__pyx_n_s_random_choices;
 static PyObject *__pyx_n_s_random_double;
 static PyObject *__pyx_n_s_random_double_noargs;
 static PyObject *__pyx_n_s_random_integer_noargs;
+static PyObject *__pyx_n_s_random_sample;
 static PyObject *__pyx_n_s_randrange;
 static PyObject *__pyx_n_s_range;
 static PyObject *__pyx_n_s_reversed;
 static PyObject *__pyx_n_s_shuffle;
 static PyObject *__pyx_n_s_start;
 static PyObject *__pyx_n_s_step;
 static PyObject *__pyx_n_s_stop;
 static PyObject *__pyx_n_s_test;
 static PyObject *__pyx_pf_9nazo_rand_9nazo_rand_random_integer_noargs(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_9nazo_rand_9nazo_rand_2shuffle(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_array); /* proto */
 static PyObject *__pyx_pf_9nazo_rand_9nazo_rand_4randbelow(CYTHON_UNUSED PyObject *__pyx_self, int __pyx_v_a); /* proto */
-static PyObject *__pyx_pf_9nazo_rand_9nazo_rand_6random_choice(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_elements); /* proto */
-static PyObject *__pyx_pf_9nazo_rand_9nazo_rand_8randint(CYTHON_UNUSED PyObject *__pyx_self, int __pyx_v_a, int __pyx_v_b); /* proto */
-static PyObject *__pyx_pf_9nazo_rand_9nazo_rand_10randrange(CYTHON_UNUSED PyObject *__pyx_self, int __pyx_v_start, int __pyx_v_stop, int __pyx_v_step); /* proto */
-static PyObject *__pyx_pf_9nazo_rand_9nazo_rand_12random_double(CYTHON_UNUSED PyObject *__pyx_self, double __pyx_v_a, double __pyx_v_b); /* proto */
-static PyObject *__pyx_pf_9nazo_rand_9nazo_rand_14random_double_noargs(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
-static PyObject *__pyx_codeobj_;
-static PyObject *__pyx_tuple__2;
-static PyObject *__pyx_tuple__4;
-static PyObject *__pyx_tuple__6;
-static PyObject *__pyx_tuple__8;
-static PyObject *__pyx_tuple__10;
-static PyObject *__pyx_tuple__12;
-static PyObject *__pyx_codeobj__3;
-static PyObject *__pyx_codeobj__5;
-static PyObject *__pyx_codeobj__7;
-static PyObject *__pyx_codeobj__9;
-static PyObject *__pyx_codeobj__11;
-static PyObject *__pyx_codeobj__13;
+static PyObject *__pyx_pf_9nazo_rand_9nazo_rand_6randint(CYTHON_UNUSED PyObject *__pyx_self, int __pyx_v_a, int __pyx_v_b); /* proto */
+static PyObject *__pyx_pf_9nazo_rand_9nazo_rand_8random_choice(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_container); /* proto */
+static PyObject *__pyx_pf_9nazo_rand_9nazo_rand_10random_choices(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_container, Py_ssize_t __pyx_v_count); /* proto */
+static PyObject *__pyx_pf_9nazo_rand_9nazo_rand_12random_sample(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_container, Py_ssize_t __pyx_v_count); /* proto */
+static PyObject *__pyx_pf_9nazo_rand_9nazo_rand_14randrange(CYTHON_UNUSED PyObject *__pyx_self, int __pyx_v_start, int __pyx_v_stop, int __pyx_v_step); /* proto */
+static PyObject *__pyx_pf_9nazo_rand_9nazo_rand_16random_double(CYTHON_UNUSED PyObject *__pyx_self, double __pyx_v_a, double __pyx_v_b); /* proto */
+static PyObject *__pyx_pf_9nazo_rand_9nazo_rand_18random_double_noargs(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_tuple_;
+static PyObject *__pyx_tuple__3;
+static PyObject *__pyx_tuple__5;
+static PyObject *__pyx_tuple__7;
+static PyObject *__pyx_tuple__9;
+static PyObject *__pyx_tuple__11;
+static PyObject *__pyx_tuple__13;
+static PyObject *__pyx_tuple__15;
+static PyObject *__pyx_tuple__17;
+static PyObject *__pyx_codeobj__2;
+static PyObject *__pyx_codeobj__4;
+static PyObject *__pyx_codeobj__6;
+static PyObject *__pyx_codeobj__8;
+static PyObject *__pyx_codeobj__10;
+static PyObject *__pyx_codeobj__12;
 static PyObject *__pyx_codeobj__14;
+static PyObject *__pyx_codeobj__16;
+static PyObject *__pyx_codeobj__18;
+static PyObject *__pyx_codeobj__19;
 /* Late includes */
 
 /* "nazo_rand/nazo_rand.pyx":15
  *     double uniform_real_variate(double a, double b)
  * 
  * cpdef int random_integer_noargs():             # <<<<<<<<<<<<<<
  *     return uniform_int_variate_noargs()
@@ -1671,15 +1718,15 @@
   __Pyx_RefNannySetupContext("randbelow", 0);
 
   /* "nazo_rand/nazo_rand.pyx":25
  * 
  * cpdef int randbelow(int a):
  *     return random_below(a)             # <<<<<<<<<<<<<<
  * 
- * @cython.boundscheck(False)
+ * cpdef int randint(int a, int b):
  */
   __pyx_r = Storm::random_below(__pyx_v_a);
   goto __pyx_L0;
 
   /* "nazo_rand/nazo_rand.pyx":24
  * 
  * 
@@ -1743,101 +1790,230 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "nazo_rand/nazo_rand.pyx":29
+/* "nazo_rand/nazo_rand.pyx":27
+ *     return random_below(a)
+ * 
+ * cpdef int randint(int a, int b):             # <<<<<<<<<<<<<<
+ *     return uniform_int_variate(a, b)
+ * 
+ */
+
+static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_7randint(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static int __pyx_f_9nazo_rand_9nazo_rand_randint(int __pyx_v_a, int __pyx_v_b, CYTHON_UNUSED int __pyx_skip_dispatch) {
+  int __pyx_r;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("randint", 0);
+
+  /* "nazo_rand/nazo_rand.pyx":28
+ * 
+ * cpdef int randint(int a, int b):
+ *     return uniform_int_variate(a, b)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_r = Storm::uniform_int_variate(__pyx_v_a, __pyx_v_b);
+  goto __pyx_L0;
+
+  /* "nazo_rand/nazo_rand.pyx":27
+ *     return random_below(a)
+ * 
+ * cpdef int randint(int a, int b):             # <<<<<<<<<<<<<<
+ *     return uniform_int_variate(a, b)
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* Python wrapper */
+static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_7randint(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_mdef_9nazo_rand_9nazo_rand_7randint = {"randint", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_9nazo_rand_9nazo_rand_7randint, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_7randint(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  int __pyx_v_a;
+  int __pyx_v_b;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("randint (wrapper)", 0);
+  {
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_a,&__pyx_n_s_b,0};
+    PyObject* values[2] = {0,0};
+    if (unlikely(__pyx_kwds)) {
+      Py_ssize_t kw_args;
+      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
+      switch (pos_args) {
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = PyDict_Size(__pyx_kwds);
+      switch (pos_args) {
+        case  0:
+        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_a)) != 0)) kw_args--;
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_b)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("randint", 1, 2, 2, 1); __PYX_ERR(0, 27, __pyx_L3_error)
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "randint") < 0)) __PYX_ERR(0, 27, __pyx_L3_error)
+      }
+    } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+    }
+    __pyx_v_a = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_a == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 27, __pyx_L3_error)
+    __pyx_v_b = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_b == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 27, __pyx_L3_error)
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("randint", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 27, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("nazo_rand.nazo_rand.randint", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_9nazo_rand_9nazo_rand_6randint(__pyx_self, __pyx_v_a, __pyx_v_b);
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_9nazo_rand_9nazo_rand_6randint(CYTHON_UNUSED PyObject *__pyx_self, int __pyx_v_a, int __pyx_v_b) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("randint", 0);
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_f_9nazo_rand_9nazo_rand_randint(__pyx_v_a, __pyx_v_b, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 27, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("nazo_rand.nazo_rand.randint", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "nazo_rand/nazo_rand.pyx":34
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
- * cpdef object random_choice(object elements):             # <<<<<<<<<<<<<<
- *     cdef Py_ssize_t index = randbelow(len(elements))
- *     return elements[index]
+ * cpdef object random_choice(object container):             # <<<<<<<<<<<<<<
+ *     cdef Py_ssize_t index = randbelow(len(container))
+ *     return container[index]
  */
 
-static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_7random_choice(PyObject *__pyx_self, PyObject *__pyx_v_elements); /*proto*/
-static PyObject *__pyx_f_9nazo_rand_9nazo_rand_random_choice(PyObject *__pyx_v_elements, CYTHON_UNUSED int __pyx_skip_dispatch) {
+static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_9random_choice(PyObject *__pyx_self, PyObject *__pyx_v_container); /*proto*/
+static PyObject *__pyx_f_9nazo_rand_9nazo_rand_random_choice(PyObject *__pyx_v_container, CYTHON_UNUSED int __pyx_skip_dispatch) {
   Py_ssize_t __pyx_v_index;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("random_choice", 0);
 
-  /* "nazo_rand/nazo_rand.pyx":30
+  /* "nazo_rand/nazo_rand.pyx":35
  * @cython.wraparound(False)
- * cpdef object random_choice(object elements):
- *     cdef Py_ssize_t index = randbelow(len(elements))             # <<<<<<<<<<<<<<
- *     return elements[index]
+ * cpdef object random_choice(object container):
+ *     cdef Py_ssize_t index = randbelow(len(container))             # <<<<<<<<<<<<<<
+ *     return container[index]
  * 
  */
-  __pyx_t_1 = PyObject_Length(__pyx_v_elements); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 30, __pyx_L1_error)
+  __pyx_t_1 = PyObject_Length(__pyx_v_container); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 35, __pyx_L1_error)
   __pyx_v_index = __pyx_f_9nazo_rand_9nazo_rand_randbelow(__pyx_t_1, 0);
 
-  /* "nazo_rand/nazo_rand.pyx":31
- * cpdef object random_choice(object elements):
- *     cdef Py_ssize_t index = randbelow(len(elements))
- *     return elements[index]             # <<<<<<<<<<<<<<
- * 
+  /* "nazo_rand/nazo_rand.pyx":36
+ * cpdef object random_choice(object container):
+ *     cdef Py_ssize_t index = randbelow(len(container))
+ *     return container[index]             # <<<<<<<<<<<<<<
  * 
+ * @cython.boundscheck(False)
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_elements, __pyx_v_index, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 31, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_container, __pyx_v_index, Py_ssize_t, 1, PyInt_FromSsize_t, 0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 36, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "nazo_rand/nazo_rand.pyx":29
+  /* "nazo_rand/nazo_rand.pyx":34
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
- * cpdef object random_choice(object elements):             # <<<<<<<<<<<<<<
- *     cdef Py_ssize_t index = randbelow(len(elements))
- *     return elements[index]
+ * cpdef object random_choice(object container):             # <<<<<<<<<<<<<<
+ *     cdef Py_ssize_t index = randbelow(len(container))
+ *     return container[index]
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_AddTraceback("nazo_rand.nazo_rand.random_choice", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_7random_choice(PyObject *__pyx_self, PyObject *__pyx_v_elements); /*proto*/
-static PyMethodDef __pyx_mdef_9nazo_rand_9nazo_rand_7random_choice = {"random_choice", (PyCFunction)__pyx_pw_9nazo_rand_9nazo_rand_7random_choice, METH_O, 0};
-static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_7random_choice(PyObject *__pyx_self, PyObject *__pyx_v_elements) {
+static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_9random_choice(PyObject *__pyx_self, PyObject *__pyx_v_container); /*proto*/
+static PyMethodDef __pyx_mdef_9nazo_rand_9nazo_rand_9random_choice = {"random_choice", (PyCFunction)__pyx_pw_9nazo_rand_9nazo_rand_9random_choice, METH_O, 0};
+static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_9random_choice(PyObject *__pyx_self, PyObject *__pyx_v_container) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("random_choice (wrapper)", 0);
-  __pyx_r = __pyx_pf_9nazo_rand_9nazo_rand_6random_choice(__pyx_self, ((PyObject *)__pyx_v_elements));
+  __pyx_r = __pyx_pf_9nazo_rand_9nazo_rand_8random_choice(__pyx_self, ((PyObject *)__pyx_v_container));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9nazo_rand_9nazo_rand_6random_choice(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_elements) {
+static PyObject *__pyx_pf_9nazo_rand_9nazo_rand_8random_choice(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_container) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("random_choice", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_9nazo_rand_9nazo_rand_random_choice(__pyx_v_elements, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 29, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_9nazo_rand_9nazo_rand_random_choice(__pyx_v_container, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -1846,66 +2022,379 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "nazo_rand/nazo_rand.pyx":34
- * 
+/* "nazo_rand/nazo_rand.pyx":40
+ * @cython.boundscheck(False)
+ * @cython.wraparound(False)
+ * cpdef list[object] random_choices(object container, Py_ssize_t count):             # <<<<<<<<<<<<<<
+ *     cdef Py_ssize_t container_length = len(container)
+ *     return [container[randbelow(container_length)] for _ in range(count)]
+ */
+
+static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_11random_choices(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyObject *__pyx_f_9nazo_rand_9nazo_rand_random_choices(PyObject *__pyx_v_container, Py_ssize_t __pyx_v_count, CYTHON_UNUSED int __pyx_skip_dispatch) {
+  Py_ssize_t __pyx_v_container_length;
+  CYTHON_UNUSED Py_ssize_t __pyx_7genexpr__pyx_v__;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  Py_ssize_t __pyx_t_1;
+  PyObject *__pyx_t_2 = NULL;
+  Py_ssize_t __pyx_t_3;
+  Py_ssize_t __pyx_t_4;
+  int __pyx_t_5;
+  PyObject *__pyx_t_6 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("random_choices", 0);
+
+  /* "nazo_rand/nazo_rand.pyx":41
+ * @cython.wraparound(False)
+ * cpdef list[object] random_choices(object container, Py_ssize_t count):
+ *     cdef Py_ssize_t container_length = len(container)             # <<<<<<<<<<<<<<
+ *     return [container[randbelow(container_length)] for _ in range(count)]
  * 
- * cpdef int randint(int a, int b):             # <<<<<<<<<<<<<<
- *     return uniform_int_variate(a, b)
+ */
+  __pyx_t_1 = PyObject_Length(__pyx_v_container); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 41, __pyx_L1_error)
+  __pyx_v_container_length = __pyx_t_1;
+
+  /* "nazo_rand/nazo_rand.pyx":42
+ * cpdef list[object] random_choices(object container, Py_ssize_t count):
+ *     cdef Py_ssize_t container_length = len(container)
+ *     return [container[randbelow(container_length)] for _ in range(count)]             # <<<<<<<<<<<<<<
  * 
+ * @cython.boundscheck(False)
  */
+  __Pyx_XDECREF(__pyx_r);
+  { /* enter inner scope */
+    __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 42, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __pyx_v_count;
+    __pyx_t_3 = __pyx_t_1;
+    for (__pyx_t_4 = 0; __pyx_t_4 < __pyx_t_3; __pyx_t_4+=1) {
+      __pyx_7genexpr__pyx_v__ = __pyx_t_4;
+      __pyx_t_5 = __pyx_f_9nazo_rand_9nazo_rand_randbelow(__pyx_v_container_length, 0);
+      __pyx_t_6 = __Pyx_GetItemInt(__pyx_v_container, __pyx_t_5, int, 1, __Pyx_PyInt_From_int, 0, 0, 0); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 42, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_6))) __PYX_ERR(0, 42, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    }
+  } /* exit inner scope */
+  __pyx_r = ((PyObject *)__pyx_t_2);
+  __pyx_t_2 = 0;
+  goto __pyx_L0;
 
-static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_9randint(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static int __pyx_f_9nazo_rand_9nazo_rand_randint(int __pyx_v_a, int __pyx_v_b, CYTHON_UNUSED int __pyx_skip_dispatch) {
-  int __pyx_r;
+  /* "nazo_rand/nazo_rand.pyx":40
+ * @cython.boundscheck(False)
+ * @cython.wraparound(False)
+ * cpdef list[object] random_choices(object container, Py_ssize_t count):             # <<<<<<<<<<<<<<
+ *     cdef Py_ssize_t container_length = len(container)
+ *     return [container[randbelow(container_length)] for _ in range(count)]
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_AddTraceback("nazo_rand.nazo_rand.random_choices", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* Python wrapper */
+static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_11random_choices(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_mdef_9nazo_rand_9nazo_rand_11random_choices = {"random_choices", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_9nazo_rand_9nazo_rand_11random_choices, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_11random_choices(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  PyObject *__pyx_v_container = 0;
+  Py_ssize_t __pyx_v_count;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("randint", 0);
+  __Pyx_RefNannySetupContext("random_choices (wrapper)", 0);
+  {
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_container,&__pyx_n_s_count,0};
+    PyObject* values[2] = {0,0};
+    if (unlikely(__pyx_kwds)) {
+      Py_ssize_t kw_args;
+      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
+      switch (pos_args) {
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = PyDict_Size(__pyx_kwds);
+      switch (pos_args) {
+        case  0:
+        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_container)) != 0)) kw_args--;
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_count)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("random_choices", 1, 2, 2, 1); __PYX_ERR(0, 40, __pyx_L3_error)
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "random_choices") < 0)) __PYX_ERR(0, 40, __pyx_L3_error)
+      }
+    } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+    }
+    __pyx_v_container = values[0];
+    __pyx_v_count = __Pyx_PyIndex_AsSsize_t(values[1]); if (unlikely((__pyx_v_count == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 40, __pyx_L3_error)
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("random_choices", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 40, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("nazo_rand.nazo_rand.random_choices", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_9nazo_rand_9nazo_rand_10random_choices(__pyx_self, __pyx_v_container, __pyx_v_count);
 
-  /* "nazo_rand/nazo_rand.pyx":35
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_9nazo_rand_9nazo_rand_10random_choices(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_container, Py_ssize_t __pyx_v_count) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("random_choices", 0);
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = __pyx_f_9nazo_rand_9nazo_rand_random_choices(__pyx_v_container, __pyx_v_count, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 40, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_AddTraceback("nazo_rand.nazo_rand.random_choices", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "nazo_rand/nazo_rand.pyx":46
+ * @cython.boundscheck(False)
+ * @cython.wraparound(False)
+ * cpdef list[object] random_sample(object container, Py_ssize_t count):             # <<<<<<<<<<<<<<
+ *     cdef Py_ssize_t container_length = len(container)
+ *     cdef Py_ssize_t i, j
+ */
+
+static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_13random_sample(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyObject *__pyx_f_9nazo_rand_9nazo_rand_random_sample(PyObject *__pyx_v_container, Py_ssize_t __pyx_v_count, CYTHON_UNUSED int __pyx_skip_dispatch) {
+  Py_ssize_t __pyx_v_container_length;
+  Py_ssize_t __pyx_v_i;
+  Py_ssize_t __pyx_v_j;
+  PyObject *__pyx_v_result = 0;
+  PyObject *__pyx_v_temp = 0;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  Py_ssize_t __pyx_t_1;
+  PyObject *__pyx_t_2 = NULL;
+  int __pyx_t_3;
+  Py_ssize_t __pyx_t_4;
+  Py_ssize_t __pyx_t_5;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("random_sample", 0);
+
+  /* "nazo_rand/nazo_rand.pyx":47
+ * @cython.wraparound(False)
+ * cpdef list[object] random_sample(object container, Py_ssize_t count):
+ *     cdef Py_ssize_t container_length = len(container)             # <<<<<<<<<<<<<<
+ *     cdef Py_ssize_t i, j
+ *     cdef list result = [None] * count
+ */
+  __pyx_t_1 = PyObject_Length(__pyx_v_container); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 47, __pyx_L1_error)
+  __pyx_v_container_length = __pyx_t_1;
+
+  /* "nazo_rand/nazo_rand.pyx":49
+ *     cdef Py_ssize_t container_length = len(container)
+ *     cdef Py_ssize_t i, j
+ *     cdef list result = [None] * count             # <<<<<<<<<<<<<<
+ *     cdef list temp = list(container)
  * 
- * cpdef int randint(int a, int b):
- *     return uniform_int_variate(a, b)             # <<<<<<<<<<<<<<
+ */
+  __pyx_t_2 = PyList_New(1 * ((__pyx_v_count<0) ? 0:__pyx_v_count)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 49, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  { Py_ssize_t __pyx_temp;
+    for (__pyx_temp=0; __pyx_temp < __pyx_v_count; __pyx_temp++) {
+      __Pyx_INCREF(Py_None);
+      __Pyx_GIVEREF(Py_None);
+      PyList_SET_ITEM(__pyx_t_2, __pyx_temp, Py_None);
+    }
+  }
+  __pyx_v_result = ((PyObject*)__pyx_t_2);
+  __pyx_t_2 = 0;
+
+  /* "nazo_rand/nazo_rand.pyx":50
+ *     cdef Py_ssize_t i, j
+ *     cdef list result = [None] * count
+ *     cdef list temp = list(container)             # <<<<<<<<<<<<<<
  * 
- * cpdef int randrange(int start, int stop=0, int step=1):
+ *     if count > container_length:
  */
-  __pyx_r = Storm::uniform_int_variate(__pyx_v_a, __pyx_v_b);
-  goto __pyx_L0;
+  __pyx_t_2 = PySequence_List(__pyx_v_container); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 50, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_v_temp = ((PyObject*)__pyx_t_2);
+  __pyx_t_2 = 0;
 
-  /* "nazo_rand/nazo_rand.pyx":34
+  /* "nazo_rand/nazo_rand.pyx":52
+ *     cdef list temp = list(container)
  * 
+ *     if count > container_length:             # <<<<<<<<<<<<<<
+ *         raise ValueError("Sample larger than population")
  * 
- * cpdef int randint(int a, int b):             # <<<<<<<<<<<<<<
- *     return uniform_int_variate(a, b)
+ */
+  __pyx_t_3 = ((__pyx_v_count > __pyx_v_container_length) != 0);
+  if (unlikely(__pyx_t_3)) {
+
+    /* "nazo_rand/nazo_rand.pyx":53
+ * 
+ *     if count > container_length:
+ *         raise ValueError("Sample larger than population")             # <<<<<<<<<<<<<<
+ * 
+ *     for i in range(count):
+ */
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 53, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_Raise(__pyx_t_2, 0, 0, 0);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __PYX_ERR(0, 53, __pyx_L1_error)
+
+    /* "nazo_rand/nazo_rand.pyx":52
+ *     cdef list temp = list(container)
+ * 
+ *     if count > container_length:             # <<<<<<<<<<<<<<
+ *         raise ValueError("Sample larger than population")
  * 
  */
+  }
+
+  /* "nazo_rand/nazo_rand.pyx":55
+ *         raise ValueError("Sample larger than population")
+ * 
+ *     for i in range(count):             # <<<<<<<<<<<<<<
+ *         j = uniform_int_variate(i, container_length - 1)
+ *         result[i] = temp[j]
+ */
+  __pyx_t_1 = __pyx_v_count;
+  __pyx_t_4 = __pyx_t_1;
+  for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_4; __pyx_t_5+=1) {
+    __pyx_v_i = __pyx_t_5;
+
+    /* "nazo_rand/nazo_rand.pyx":56
+ * 
+ *     for i in range(count):
+ *         j = uniform_int_variate(i, container_length - 1)             # <<<<<<<<<<<<<<
+ *         result[i] = temp[j]
+ *         temp[j] = temp[i]
+ */
+    __pyx_v_j = Storm::uniform_int_variate(__pyx_v_i, (__pyx_v_container_length - 1));
+
+    /* "nazo_rand/nazo_rand.pyx":57
+ *     for i in range(count):
+ *         j = uniform_int_variate(i, container_length - 1)
+ *         result[i] = temp[j]             # <<<<<<<<<<<<<<
+ *         temp[j] = temp[i]
+ * 
+ */
+    __pyx_t_2 = PyList_GET_ITEM(__pyx_v_temp, __pyx_v_j);
+    __Pyx_INCREF(__pyx_t_2);
+    if (unlikely(__Pyx_SetItemInt(__pyx_v_result, __pyx_v_i, __pyx_t_2, Py_ssize_t, 1, PyInt_FromSsize_t, 1, 0, 0) < 0)) __PYX_ERR(0, 57, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "nazo_rand/nazo_rand.pyx":58
+ *         j = uniform_int_variate(i, container_length - 1)
+ *         result[i] = temp[j]
+ *         temp[j] = temp[i]             # <<<<<<<<<<<<<<
+ * 
+ *     return result
+ */
+    __pyx_t_2 = PyList_GET_ITEM(__pyx_v_temp, __pyx_v_i);
+    __Pyx_INCREF(__pyx_t_2);
+    if (unlikely(__Pyx_SetItemInt(__pyx_v_temp, __pyx_v_j, __pyx_t_2, Py_ssize_t, 1, PyInt_FromSsize_t, 1, 0, 0) < 0)) __PYX_ERR(0, 58, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  }
+
+  /* "nazo_rand/nazo_rand.pyx":60
+ *         temp[j] = temp[i]
+ * 
+ *     return result             # <<<<<<<<<<<<<<
+ * 
+ * cpdef int randrange(int start, int stop=0, int step=1):
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_INCREF(__pyx_v_result);
+  __pyx_r = ((PyObject *)__pyx_v_result);
+  goto __pyx_L0;
+
+  /* "nazo_rand/nazo_rand.pyx":46
+ * @cython.boundscheck(False)
+ * @cython.wraparound(False)
+ * cpdef list[object] random_sample(object container, Py_ssize_t count):             # <<<<<<<<<<<<<<
+ *     cdef Py_ssize_t container_length = len(container)
+ *     cdef Py_ssize_t i, j
+ */
 
   /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_AddTraceback("nazo_rand.nazo_rand.random_sample", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = 0;
   __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_result);
+  __Pyx_XDECREF(__pyx_v_temp);
+  __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_9randint(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_mdef_9nazo_rand_9nazo_rand_9randint = {"randint", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_9nazo_rand_9nazo_rand_9randint, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_9randint(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
-  int __pyx_v_a;
-  int __pyx_v_b;
+static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_13random_sample(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_mdef_9nazo_rand_9nazo_rand_13random_sample = {"random_sample", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_9nazo_rand_9nazo_rand_13random_sample, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_13random_sample(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  PyObject *__pyx_v_container = 0;
+  Py_ssize_t __pyx_v_count;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("randint (wrapper)", 0);
+  __Pyx_RefNannySetupContext("random_sample (wrapper)", 0);
   {
-    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_a,&__pyx_n_s_b,0};
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_container,&__pyx_n_s_count,0};
     PyObject* values[2] = {0,0};
     if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
       const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
       switch (pos_args) {
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
@@ -1913,85 +2402,85 @@
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = PyDict_Size(__pyx_kwds);
       switch (pos_args) {
         case  0:
-        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_a)) != 0)) kw_args--;
+        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_container)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
-        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_b)) != 0)) kw_args--;
+        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_count)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("randint", 1, 2, 2, 1); __PYX_ERR(0, 34, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("random_sample", 1, 2, 2, 1); __PYX_ERR(0, 46, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "randint") < 0)) __PYX_ERR(0, 34, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "random_sample") < 0)) __PYX_ERR(0, 46, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
-    __pyx_v_a = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_a == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 34, __pyx_L3_error)
-    __pyx_v_b = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_b == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 34, __pyx_L3_error)
+    __pyx_v_container = values[0];
+    __pyx_v_count = __Pyx_PyIndex_AsSsize_t(values[1]); if (unlikely((__pyx_v_count == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 46, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("randint", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 34, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("random_sample", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 46, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("nazo_rand.nazo_rand.randint", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("nazo_rand.nazo_rand.random_sample", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_9nazo_rand_9nazo_rand_8randint(__pyx_self, __pyx_v_a, __pyx_v_b);
+  __pyx_r = __pyx_pf_9nazo_rand_9nazo_rand_12random_sample(__pyx_self, __pyx_v_container, __pyx_v_count);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9nazo_rand_9nazo_rand_8randint(CYTHON_UNUSED PyObject *__pyx_self, int __pyx_v_a, int __pyx_v_b) {
+static PyObject *__pyx_pf_9nazo_rand_9nazo_rand_12random_sample(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_container, Py_ssize_t __pyx_v_count) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("randint", 0);
+  __Pyx_RefNannySetupContext("random_sample", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_f_9nazo_rand_9nazo_rand_randint(__pyx_v_a, __pyx_v_b, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 34, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_9nazo_rand_9nazo_rand_random_sample(__pyx_v_container, __pyx_v_count, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 46, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("nazo_rand.nazo_rand.randint", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("nazo_rand.nazo_rand.random_sample", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "nazo_rand/nazo_rand.pyx":37
- *     return uniform_int_variate(a, b)
+/* "nazo_rand/nazo_rand.pyx":62
+ *     return result
  * 
  * cpdef int randrange(int start, int stop=0, int step=1):             # <<<<<<<<<<<<<<
  *     if stop == 0:
  *         stop, start = start, 0
  */
 
-static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_11randrange(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_15randrange(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static int __pyx_f_9nazo_rand_9nazo_rand_randrange(int __pyx_v_start, CYTHON_UNUSED int __pyx_skip_dispatch, struct __pyx_opt_args_9nazo_rand_9nazo_rand_randrange *__pyx_optional_args) {
   int __pyx_v_stop = ((int)0);
   int __pyx_v_step = ((int)1);
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
@@ -2002,73 +2491,73 @@
       __pyx_v_stop = __pyx_optional_args->stop;
       if (__pyx_optional_args->__pyx_n > 1) {
         __pyx_v_step = __pyx_optional_args->step;
       }
     }
   }
 
-  /* "nazo_rand/nazo_rand.pyx":38
+  /* "nazo_rand/nazo_rand.pyx":63
  * 
  * cpdef int randrange(int start, int stop=0, int step=1):
  *     if stop == 0:             # <<<<<<<<<<<<<<
  *         stop, start = start, 0
  *     return random_range(start, stop, step)
  */
   __pyx_t_1 = ((__pyx_v_stop == 0) != 0);
   if (__pyx_t_1) {
 
-    /* "nazo_rand/nazo_rand.pyx":39
+    /* "nazo_rand/nazo_rand.pyx":64
  * cpdef int randrange(int start, int stop=0, int step=1):
  *     if stop == 0:
  *         stop, start = start, 0             # <<<<<<<<<<<<<<
  *     return random_range(start, stop, step)
  * 
  */
     __pyx_t_2 = __pyx_v_start;
     __pyx_t_3 = 0;
     __pyx_v_stop = __pyx_t_2;
     __pyx_v_start = __pyx_t_3;
 
-    /* "nazo_rand/nazo_rand.pyx":38
+    /* "nazo_rand/nazo_rand.pyx":63
  * 
  * cpdef int randrange(int start, int stop=0, int step=1):
  *     if stop == 0:             # <<<<<<<<<<<<<<
  *         stop, start = start, 0
  *     return random_range(start, stop, step)
  */
   }
 
-  /* "nazo_rand/nazo_rand.pyx":40
+  /* "nazo_rand/nazo_rand.pyx":65
  *     if stop == 0:
  *         stop, start = start, 0
  *     return random_range(start, stop, step)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = Storm::random_range(__pyx_v_start, __pyx_v_stop, __pyx_v_step);
   goto __pyx_L0;
 
-  /* "nazo_rand/nazo_rand.pyx":37
- *     return uniform_int_variate(a, b)
+  /* "nazo_rand/nazo_rand.pyx":62
+ *     return result
  * 
  * cpdef int randrange(int start, int stop=0, int step=1):             # <<<<<<<<<<<<<<
  *     if stop == 0:
  *         stop, start = start, 0
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_11randrange(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_mdef_9nazo_rand_9nazo_rand_11randrange = {"randrange", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_9nazo_rand_9nazo_rand_11randrange, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_11randrange(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_15randrange(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_mdef_9nazo_rand_9nazo_rand_15randrange = {"randrange", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_9nazo_rand_9nazo_rand_15randrange, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_15randrange(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   int __pyx_v_start;
   int __pyx_v_stop;
   int __pyx_v_step;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
@@ -2105,70 +2594,70 @@
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_step);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "randrange") < 0)) __PYX_ERR(0, 37, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "randrange") < 0)) __PYX_ERR(0, 62, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
-    __pyx_v_start = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_start == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 37, __pyx_L3_error)
+    __pyx_v_start = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_start == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 62, __pyx_L3_error)
     if (values[1]) {
-      __pyx_v_stop = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_stop == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 37, __pyx_L3_error)
+      __pyx_v_stop = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_stop == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 62, __pyx_L3_error)
     } else {
       __pyx_v_stop = ((int)0);
     }
     if (values[2]) {
-      __pyx_v_step = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_step == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 37, __pyx_L3_error)
+      __pyx_v_step = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_step == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 62, __pyx_L3_error)
     } else {
       __pyx_v_step = ((int)1);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("randrange", 0, 1, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 37, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("randrange", 0, 1, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 62, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("nazo_rand.nazo_rand.randrange", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_9nazo_rand_9nazo_rand_10randrange(__pyx_self, __pyx_v_start, __pyx_v_stop, __pyx_v_step);
+  __pyx_r = __pyx_pf_9nazo_rand_9nazo_rand_14randrange(__pyx_self, __pyx_v_start, __pyx_v_stop, __pyx_v_step);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9nazo_rand_9nazo_rand_10randrange(CYTHON_UNUSED PyObject *__pyx_self, int __pyx_v_start, int __pyx_v_stop, int __pyx_v_step) {
+static PyObject *__pyx_pf_9nazo_rand_9nazo_rand_14randrange(CYTHON_UNUSED PyObject *__pyx_self, int __pyx_v_start, int __pyx_v_stop, int __pyx_v_step) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   struct __pyx_opt_args_9nazo_rand_9nazo_rand_randrange __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("randrange", 0);
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_2.__pyx_n = 2;
   __pyx_t_2.stop = __pyx_v_stop;
   __pyx_t_2.step = __pyx_v_step;
   __pyx_t_1 = __pyx_f_9nazo_rand_9nazo_rand_randrange(__pyx_v_start, 0, &__pyx_t_2); 
-  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 37, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 62, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_r = __pyx_t_3;
   __pyx_t_3 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -2177,56 +2666,56 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "nazo_rand/nazo_rand.pyx":43
+/* "nazo_rand/nazo_rand.pyx":68
  * 
  * 
  * cpdef double random_double(double a, double b):             # <<<<<<<<<<<<<<
  *     return uniform_real_variate(a, b)
  * 
  */
 
-static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_13random_double(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_17random_double(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
 static double __pyx_f_9nazo_rand_9nazo_rand_random_double(double __pyx_v_a, double __pyx_v_b, CYTHON_UNUSED int __pyx_skip_dispatch) {
   double __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("random_double", 0);
 
-  /* "nazo_rand/nazo_rand.pyx":44
+  /* "nazo_rand/nazo_rand.pyx":69
  * 
  * cpdef double random_double(double a, double b):
  *     return uniform_real_variate(a, b)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = Storm::uniform_real_variate(__pyx_v_a, __pyx_v_b);
   goto __pyx_L0;
 
-  /* "nazo_rand/nazo_rand.pyx":43
+  /* "nazo_rand/nazo_rand.pyx":68
  * 
  * 
  * cpdef double random_double(double a, double b):             # <<<<<<<<<<<<<<
  *     return uniform_real_variate(a, b)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_13random_double(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_mdef_9nazo_rand_9nazo_rand_13random_double = {"random_double", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_9nazo_rand_9nazo_rand_13random_double, METH_VARARGS|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_13random_double(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_17random_double(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_mdef_9nazo_rand_9nazo_rand_17random_double = {"random_double", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_9nazo_rand_9nazo_rand_17random_double, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_17random_double(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   double __pyx_v_a;
   double __pyx_v_b;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
@@ -2250,54 +2739,54 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_a)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_b)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("random_double", 1, 2, 2, 1); __PYX_ERR(0, 43, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("random_double", 1, 2, 2, 1); __PYX_ERR(0, 68, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "random_double") < 0)) __PYX_ERR(0, 43, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "random_double") < 0)) __PYX_ERR(0, 68, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
     }
-    __pyx_v_a = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_a == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 43, __pyx_L3_error)
-    __pyx_v_b = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_b == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 43, __pyx_L3_error)
+    __pyx_v_a = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_a == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 68, __pyx_L3_error)
+    __pyx_v_b = __pyx_PyFloat_AsDouble(values[1]); if (unlikely((__pyx_v_b == (double)-1) && PyErr_Occurred())) __PYX_ERR(0, 68, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("random_double", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 43, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("random_double", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 68, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("nazo_rand.nazo_rand.random_double", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_9nazo_rand_9nazo_rand_12random_double(__pyx_self, __pyx_v_a, __pyx_v_b);
+  __pyx_r = __pyx_pf_9nazo_rand_9nazo_rand_16random_double(__pyx_self, __pyx_v_a, __pyx_v_b);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9nazo_rand_9nazo_rand_12random_double(CYTHON_UNUSED PyObject *__pyx_self, double __pyx_v_a, double __pyx_v_b) {
+static PyObject *__pyx_pf_9nazo_rand_9nazo_rand_16random_double(CYTHON_UNUSED PyObject *__pyx_self, double __pyx_v_a, double __pyx_v_b) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("random_double", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble(__pyx_f_9nazo_rand_9nazo_rand_random_double(__pyx_v_a, __pyx_v_b, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 43, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(__pyx_f_9nazo_rand_9nazo_rand_random_double(__pyx_v_a, __pyx_v_b, 0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 68, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -2306,72 +2795,72 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "nazo_rand/nazo_rand.pyx":47
+/* "nazo_rand/nazo_rand.pyx":72
  * 
  * 
  * cpdef double random_double_noargs():             # <<<<<<<<<<<<<<
  *     return uniform_real_variate_noargs()
  */
 
-static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_15random_double_noargs(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_19random_double_noargs(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused); /*proto*/
 static double __pyx_f_9nazo_rand_9nazo_rand_random_double_noargs(CYTHON_UNUSED int __pyx_skip_dispatch) {
   double __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("random_double_noargs", 0);
 
-  /* "nazo_rand/nazo_rand.pyx":48
+  /* "nazo_rand/nazo_rand.pyx":73
  * 
  * cpdef double random_double_noargs():
  *     return uniform_real_variate_noargs()             # <<<<<<<<<<<<<<
  */
   __pyx_r = Storm::uniform_real_variate_noargs();
   goto __pyx_L0;
 
-  /* "nazo_rand/nazo_rand.pyx":47
+  /* "nazo_rand/nazo_rand.pyx":72
  * 
  * 
  * cpdef double random_double_noargs():             # <<<<<<<<<<<<<<
  *     return uniform_real_variate_noargs()
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_15random_double_noargs(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused); /*proto*/
-static PyMethodDef __pyx_mdef_9nazo_rand_9nazo_rand_15random_double_noargs = {"random_double_noargs", (PyCFunction)__pyx_pw_9nazo_rand_9nazo_rand_15random_double_noargs, METH_NOARGS, 0};
-static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_15random_double_noargs(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused) {
+static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_19random_double_noargs(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static PyMethodDef __pyx_mdef_9nazo_rand_9nazo_rand_19random_double_noargs = {"random_double_noargs", (PyCFunction)__pyx_pw_9nazo_rand_9nazo_rand_19random_double_noargs, METH_NOARGS, 0};
+static PyObject *__pyx_pw_9nazo_rand_9nazo_rand_19random_double_noargs(PyObject *__pyx_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("random_double_noargs (wrapper)", 0);
-  __pyx_r = __pyx_pf_9nazo_rand_9nazo_rand_14random_double_noargs(__pyx_self);
+  __pyx_r = __pyx_pf_9nazo_rand_9nazo_rand_18random_double_noargs(__pyx_self);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_9nazo_rand_9nazo_rand_14random_double_noargs(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_9nazo_rand_9nazo_rand_18random_double_noargs(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("random_double_noargs", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyFloat_FromDouble(__pyx_f_9nazo_rand_9nazo_rand_random_double_noargs(0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 47, __pyx_L1_error)
+  __pyx_t_1 = PyFloat_FromDouble(__pyx_f_9nazo_rand_9nazo_rand_random_double_noargs(0)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -2426,139 +2915,180 @@
     #define CYTHON_SMALL_CODE __attribute__((cold))
 #else
     #define CYTHON_SMALL_CODE
 #endif
 #endif
 
 static __Pyx_StringTabEntry __pyx_string_tab[] = {
+  {&__pyx_kp_u_Sample_larger_than_population, __pyx_k_Sample_larger_than_population, sizeof(__pyx_k_Sample_larger_than_population), 0, 1, 0, 0},
+  {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
   {&__pyx_n_s_a, __pyx_k_a, sizeof(__pyx_k_a), 0, 0, 1, 1},
   {&__pyx_n_s_array, __pyx_k_array, sizeof(__pyx_k_array), 0, 0, 1, 1},
   {&__pyx_n_s_b, __pyx_k_b, sizeof(__pyx_k_b), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
-  {&__pyx_n_s_elements, __pyx_k_elements, sizeof(__pyx_k_elements), 0, 0, 1, 1},
+  {&__pyx_n_s_container, __pyx_k_container, sizeof(__pyx_k_container), 0, 0, 1, 1},
+  {&__pyx_n_s_count, __pyx_k_count, sizeof(__pyx_k_count), 0, 0, 1, 1},
   {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
   {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
   {&__pyx_n_s_nazo_rand_nazo_rand, __pyx_k_nazo_rand_nazo_rand, sizeof(__pyx_k_nazo_rand_nazo_rand), 0, 0, 1, 1},
   {&__pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_k_nazo_rand_nazo_rand_pyx, sizeof(__pyx_k_nazo_rand_nazo_rand_pyx), 0, 0, 1, 0},
   {&__pyx_n_s_randbelow, __pyx_k_randbelow, sizeof(__pyx_k_randbelow), 0, 0, 1, 1},
   {&__pyx_n_s_randint, __pyx_k_randint, sizeof(__pyx_k_randint), 0, 0, 1, 1},
   {&__pyx_n_s_random_choice, __pyx_k_random_choice, sizeof(__pyx_k_random_choice), 0, 0, 1, 1},
+  {&__pyx_n_s_random_choices, __pyx_k_random_choices, sizeof(__pyx_k_random_choices), 0, 0, 1, 1},
   {&__pyx_n_s_random_double, __pyx_k_random_double, sizeof(__pyx_k_random_double), 0, 0, 1, 1},
   {&__pyx_n_s_random_double_noargs, __pyx_k_random_double_noargs, sizeof(__pyx_k_random_double_noargs), 0, 0, 1, 1},
   {&__pyx_n_s_random_integer_noargs, __pyx_k_random_integer_noargs, sizeof(__pyx_k_random_integer_noargs), 0, 0, 1, 1},
+  {&__pyx_n_s_random_sample, __pyx_k_random_sample, sizeof(__pyx_k_random_sample), 0, 0, 1, 1},
   {&__pyx_n_s_randrange, __pyx_k_randrange, sizeof(__pyx_k_randrange), 0, 0, 1, 1},
   {&__pyx_n_s_range, __pyx_k_range, sizeof(__pyx_k_range), 0, 0, 1, 1},
   {&__pyx_n_s_reversed, __pyx_k_reversed, sizeof(__pyx_k_reversed), 0, 0, 1, 1},
   {&__pyx_n_s_shuffle, __pyx_k_shuffle, sizeof(__pyx_k_shuffle), 0, 0, 1, 1},
   {&__pyx_n_s_start, __pyx_k_start, sizeof(__pyx_k_start), 0, 0, 1, 1},
   {&__pyx_n_s_step, __pyx_k_step, sizeof(__pyx_k_step), 0, 0, 1, 1},
   {&__pyx_n_s_stop, __pyx_k_stop, sizeof(__pyx_k_stop), 0, 0, 1, 1},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_reversed = __Pyx_GetBuiltinName(__pyx_n_s_reversed); if (!__pyx_builtin_reversed) __PYX_ERR(0, 19, __pyx_L1_error)
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 19, __pyx_L1_error)
+  __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(0, 53, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
+  /* "nazo_rand/nazo_rand.pyx":53
+ * 
+ *     if count > container_length:
+ *         raise ValueError("Sample larger than population")             # <<<<<<<<<<<<<<
+ * 
+ *     for i in range(count):
+ */
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_Sample_larger_than_population); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 53, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple_);
+  __Pyx_GIVEREF(__pyx_tuple_);
+
   /* "nazo_rand/nazo_rand.pyx":15
  *     double uniform_real_variate(double a, double b)
  * 
  * cpdef int random_integer_noargs():             # <<<<<<<<<<<<<<
  *     return uniform_int_variate_noargs()
  * 
  */
-  __pyx_codeobj_ = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_random_integer_noargs, 15, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj_)) __PYX_ERR(0, 15, __pyx_L1_error)
+  __pyx_codeobj__2 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_random_integer_noargs, 15, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__2)) __PYX_ERR(0, 15, __pyx_L1_error)
 
   /* "nazo_rand/nazo_rand.pyx":18
  *     return uniform_int_variate_noargs()
  * 
  * cpdef void shuffle(list array):             # <<<<<<<<<<<<<<
  *     for i in reversed(range(len(array) - 1)):
  *         j = randrange(i, len(array), 1)
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_n_s_array); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 18, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__2);
-  __Pyx_GIVEREF(__pyx_tuple__2);
-  __pyx_codeobj__3 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__2, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_shuffle, 18, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__3)) __PYX_ERR(0, 18, __pyx_L1_error)
+  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_n_s_array); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(0, 18, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__3);
+  __Pyx_GIVEREF(__pyx_tuple__3);
+  __pyx_codeobj__4 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__3, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_shuffle, 18, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__4)) __PYX_ERR(0, 18, __pyx_L1_error)
 
   /* "nazo_rand/nazo_rand.pyx":24
  * 
  * 
  * cpdef int randbelow(int a):             # <<<<<<<<<<<<<<
  *     return random_below(a)
  * 
  */
-  __pyx_tuple__4 = PyTuple_Pack(2, __pyx_n_s_a, __pyx_n_s_a); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(0, 24, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__4);
-  __Pyx_GIVEREF(__pyx_tuple__4);
-  __pyx_codeobj__5 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__4, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_randbelow, 24, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__5)) __PYX_ERR(0, 24, __pyx_L1_error)
+  __pyx_tuple__5 = PyTuple_Pack(2, __pyx_n_s_a, __pyx_n_s_a); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(0, 24, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__5);
+  __Pyx_GIVEREF(__pyx_tuple__5);
+  __pyx_codeobj__6 = (PyObject*)__Pyx_PyCode_New(1, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__5, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_randbelow, 24, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__6)) __PYX_ERR(0, 24, __pyx_L1_error)
 
-  /* "nazo_rand/nazo_rand.pyx":29
- * @cython.boundscheck(False)
- * @cython.wraparound(False)
- * cpdef object random_choice(object elements):             # <<<<<<<<<<<<<<
- *     cdef Py_ssize_t index = randbelow(len(elements))
- *     return elements[index]
- */
-  __pyx_tuple__6 = PyTuple_Pack(1, __pyx_n_s_elements); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 29, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__6);
-  __Pyx_GIVEREF(__pyx_tuple__6);
-  __pyx_codeobj__7 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_random_choice, 29, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__7)) __PYX_ERR(0, 29, __pyx_L1_error)
-
-  /* "nazo_rand/nazo_rand.pyx":34
- * 
+  /* "nazo_rand/nazo_rand.pyx":27
+ *     return random_below(a)
  * 
  * cpdef int randint(int a, int b):             # <<<<<<<<<<<<<<
  *     return uniform_int_variate(a, b)
  * 
  */
-  __pyx_tuple__8 = PyTuple_Pack(2, __pyx_n_s_a, __pyx_n_s_b); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 34, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__8);
-  __Pyx_GIVEREF(__pyx_tuple__8);
-  __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__8, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_randint, 34, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(0, 34, __pyx_L1_error)
+  __pyx_tuple__7 = PyTuple_Pack(2, __pyx_n_s_a, __pyx_n_s_b); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 27, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__7);
+  __Pyx_GIVEREF(__pyx_tuple__7);
+  __pyx_codeobj__8 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__7, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_randint, 27, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__8)) __PYX_ERR(0, 27, __pyx_L1_error)
 
-  /* "nazo_rand/nazo_rand.pyx":37
- *     return uniform_int_variate(a, b)
+  /* "nazo_rand/nazo_rand.pyx":34
+ * @cython.boundscheck(False)
+ * @cython.wraparound(False)
+ * cpdef object random_choice(object container):             # <<<<<<<<<<<<<<
+ *     cdef Py_ssize_t index = randbelow(len(container))
+ *     return container[index]
+ */
+  __pyx_tuple__9 = PyTuple_Pack(1, __pyx_n_s_container); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 34, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__9);
+  __Pyx_GIVEREF(__pyx_tuple__9);
+  __pyx_codeobj__10 = (PyObject*)__Pyx_PyCode_New(1, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__9, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_random_choice, 34, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__10)) __PYX_ERR(0, 34, __pyx_L1_error)
+
+  /* "nazo_rand/nazo_rand.pyx":40
+ * @cython.boundscheck(False)
+ * @cython.wraparound(False)
+ * cpdef list[object] random_choices(object container, Py_ssize_t count):             # <<<<<<<<<<<<<<
+ *     cdef Py_ssize_t container_length = len(container)
+ *     return [container[randbelow(container_length)] for _ in range(count)]
+ */
+  __pyx_tuple__11 = PyTuple_Pack(2, __pyx_n_s_container, __pyx_n_s_count); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 40, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__11);
+  __Pyx_GIVEREF(__pyx_tuple__11);
+  __pyx_codeobj__12 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_random_choices, 40, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__12)) __PYX_ERR(0, 40, __pyx_L1_error)
+
+  /* "nazo_rand/nazo_rand.pyx":46
+ * @cython.boundscheck(False)
+ * @cython.wraparound(False)
+ * cpdef list[object] random_sample(object container, Py_ssize_t count):             # <<<<<<<<<<<<<<
+ *     cdef Py_ssize_t container_length = len(container)
+ *     cdef Py_ssize_t i, j
+ */
+  __pyx_tuple__13 = PyTuple_Pack(2, __pyx_n_s_container, __pyx_n_s_count); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(0, 46, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__13);
+  __Pyx_GIVEREF(__pyx_tuple__13);
+  __pyx_codeobj__14 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__13, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_random_sample, 46, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__14)) __PYX_ERR(0, 46, __pyx_L1_error)
+
+  /* "nazo_rand/nazo_rand.pyx":62
+ *     return result
  * 
  * cpdef int randrange(int start, int stop=0, int step=1):             # <<<<<<<<<<<<<<
  *     if stop == 0:
  *         stop, start = start, 0
  */
-  __pyx_tuple__10 = PyTuple_Pack(3, __pyx_n_s_start, __pyx_n_s_stop, __pyx_n_s_step); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(0, 37, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__10);
-  __Pyx_GIVEREF(__pyx_tuple__10);
-  __pyx_codeobj__11 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__10, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_randrange, 37, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__11)) __PYX_ERR(0, 37, __pyx_L1_error)
+  __pyx_tuple__15 = PyTuple_Pack(3, __pyx_n_s_start, __pyx_n_s_stop, __pyx_n_s_step); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(0, 62, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__15);
+  __Pyx_GIVEREF(__pyx_tuple__15);
+  __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(3, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__15, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_randrange, 62, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(0, 62, __pyx_L1_error)
 
-  /* "nazo_rand/nazo_rand.pyx":43
+  /* "nazo_rand/nazo_rand.pyx":68
  * 
  * 
  * cpdef double random_double(double a, double b):             # <<<<<<<<<<<<<<
  *     return uniform_real_variate(a, b)
  * 
  */
-  __pyx_tuple__12 = PyTuple_Pack(2, __pyx_n_s_a, __pyx_n_s_b); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(0, 43, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__12);
-  __Pyx_GIVEREF(__pyx_tuple__12);
-  __pyx_codeobj__13 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__12, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_random_double, 43, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__13)) __PYX_ERR(0, 43, __pyx_L1_error)
+  __pyx_tuple__17 = PyTuple_Pack(2, __pyx_n_s_a, __pyx_n_s_b); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(0, 68, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__17);
+  __Pyx_GIVEREF(__pyx_tuple__17);
+  __pyx_codeobj__18 = (PyObject*)__Pyx_PyCode_New(2, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__17, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_random_double, 68, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__18)) __PYX_ERR(0, 68, __pyx_L1_error)
 
-  /* "nazo_rand/nazo_rand.pyx":47
+  /* "nazo_rand/nazo_rand.pyx":72
  * 
  * 
  * cpdef double random_double_noargs():             # <<<<<<<<<<<<<<
  *     return uniform_real_variate_noargs()
  */
-  __pyx_codeobj__14 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_random_double_noargs, 47, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__14)) __PYX_ERR(0, 47, __pyx_L1_error)
+  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(0, 0, 0, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_nazo_rand_nazo_rand_pyx, __pyx_n_s_random_double_noargs, 72, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -2599,14 +3129,16 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_function_export_code", 0);
   /*--- Function export code ---*/
   if (__Pyx_ExportFunction("shuffle", (void (*)(void))__pyx_f_9nazo_rand_9nazo_rand_shuffle, "void (PyObject *, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   if (__Pyx_ExportFunction("random_integer_noargs", (void (*)(void))__pyx_f_9nazo_rand_9nazo_rand_random_integer_noargs, "int (int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   if (__Pyx_ExportFunction("random_choice", (void (*)(void))__pyx_f_9nazo_rand_9nazo_rand_random_choice, "PyObject *(PyObject *, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ExportFunction("random_choices", (void (*)(void))__pyx_f_9nazo_rand_9nazo_rand_random_choices, "PyObject *(PyObject *, Py_ssize_t, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ExportFunction("random_sample", (void (*)(void))__pyx_f_9nazo_rand_9nazo_rand_random_sample, "PyObject *(PyObject *, Py_ssize_t, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   if (__Pyx_ExportFunction("randbelow", (void (*)(void))__pyx_f_9nazo_rand_9nazo_rand_randbelow, "int (int, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   if (__Pyx_ExportFunction("randint", (void (*)(void))__pyx_f_9nazo_rand_9nazo_rand_randint, "int (int, int, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   if (__Pyx_ExportFunction("randrange", (void (*)(void))__pyx_f_9nazo_rand_9nazo_rand_randrange, "int (int, int __pyx_skip_dispatch, struct __pyx_opt_args_9nazo_rand_9nazo_rand_randrange *__pyx_optional_args)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   if (__Pyx_ExportFunction("random_double", (void (*)(void))__pyx_f_9nazo_rand_9nazo_rand_random_double, "double (double, double, int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   if (__Pyx_ExportFunction("random_double_noargs", (void (*)(void))__pyx_f_9nazo_rand_9nazo_rand_random_double_noargs, "double (int __pyx_skip_dispatch)") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
@@ -2850,100 +3382,124 @@
   /* "nazo_rand/nazo_rand.pyx":15
  *     double uniform_real_variate(double a, double b)
  * 
  * cpdef int random_integer_noargs():             # <<<<<<<<<<<<<<
  *     return uniform_int_variate_noargs()
  * 
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_1random_integer_noargs, 0, __pyx_n_s_random_integer_noargs, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj_)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 15, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_1random_integer_noargs, 0, __pyx_n_s_random_integer_noargs, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__2)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_random_integer_noargs, __pyx_t_1) < 0) __PYX_ERR(0, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "nazo_rand/nazo_rand.pyx":18
  *     return uniform_int_variate_noargs()
  * 
  * cpdef void shuffle(list array):             # <<<<<<<<<<<<<<
  *     for i in reversed(range(len(array) - 1)):
  *         j = randrange(i, len(array), 1)
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_3shuffle, 0, __pyx_n_s_shuffle, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__3)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 18, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_3shuffle, 0, __pyx_n_s_shuffle, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__4)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 18, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_shuffle, __pyx_t_1) < 0) __PYX_ERR(0, 18, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "nazo_rand/nazo_rand.pyx":24
  * 
  * 
  * cpdef int randbelow(int a):             # <<<<<<<<<<<<<<
  *     return random_below(a)
  * 
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_5randbelow, 0, __pyx_n_s_randbelow, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__5)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 24, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_5randbelow, 0, __pyx_n_s_randbelow, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__6)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_randbelow, __pyx_t_1) < 0) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "nazo_rand/nazo_rand.pyx":29
+  /* "nazo_rand/nazo_rand.pyx":27
+ *     return random_below(a)
+ * 
+ * cpdef int randint(int a, int b):             # <<<<<<<<<<<<<<
+ *     return uniform_int_variate(a, b)
+ * 
+ */
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_7randint, 0, __pyx_n_s_randint, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__8)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 27, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_randint, __pyx_t_1) < 0) __PYX_ERR(0, 27, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "nazo_rand/nazo_rand.pyx":34
  * @cython.boundscheck(False)
  * @cython.wraparound(False)
- * cpdef object random_choice(object elements):             # <<<<<<<<<<<<<<
- *     cdef Py_ssize_t index = randbelow(len(elements))
- *     return elements[index]
+ * cpdef object random_choice(object container):             # <<<<<<<<<<<<<<
+ *     cdef Py_ssize_t index = randbelow(len(container))
+ *     return container[index]
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_7random_choice, 0, __pyx_n_s_random_choice, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__7)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 29, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_9random_choice, 0, __pyx_n_s_random_choice, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__10)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_random_choice, __pyx_t_1) < 0) __PYX_ERR(0, 29, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_random_choice, __pyx_t_1) < 0) __PYX_ERR(0, 34, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "nazo_rand/nazo_rand.pyx":34
- * 
- * 
- * cpdef int randint(int a, int b):             # <<<<<<<<<<<<<<
- *     return uniform_int_variate(a, b)
- * 
+  /* "nazo_rand/nazo_rand.pyx":40
+ * @cython.boundscheck(False)
+ * @cython.wraparound(False)
+ * cpdef list[object] random_choices(object container, Py_ssize_t count):             # <<<<<<<<<<<<<<
+ *     cdef Py_ssize_t container_length = len(container)
+ *     return [container[randbelow(container_length)] for _ in range(count)]
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_9randint, 0, __pyx_n_s_randint, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__9)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 34, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_11random_choices, 0, __pyx_n_s_random_choices, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__12)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 40, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_randint, __pyx_t_1) < 0) __PYX_ERR(0, 34, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_random_choices, __pyx_t_1) < 0) __PYX_ERR(0, 40, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "nazo_rand/nazo_rand.pyx":37
- *     return uniform_int_variate(a, b)
+  /* "nazo_rand/nazo_rand.pyx":46
+ * @cython.boundscheck(False)
+ * @cython.wraparound(False)
+ * cpdef list[object] random_sample(object container, Py_ssize_t count):             # <<<<<<<<<<<<<<
+ *     cdef Py_ssize_t container_length = len(container)
+ *     cdef Py_ssize_t i, j
+ */
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_13random_sample, 0, __pyx_n_s_random_sample, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__14)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 46, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_random_sample, __pyx_t_1) < 0) __PYX_ERR(0, 46, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "nazo_rand/nazo_rand.pyx":62
+ *     return result
  * 
  * cpdef int randrange(int start, int stop=0, int step=1):             # <<<<<<<<<<<<<<
  *     if stop == 0:
  *         stop, start = start, 0
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_11randrange, 0, __pyx_n_s_randrange, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__11)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 37, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_15randrange, 0, __pyx_n_s_randrange, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__16)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 62, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_randrange, __pyx_t_1) < 0) __PYX_ERR(0, 37, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_randrange, __pyx_t_1) < 0) __PYX_ERR(0, 62, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "nazo_rand/nazo_rand.pyx":43
+  /* "nazo_rand/nazo_rand.pyx":68
  * 
  * 
  * cpdef double random_double(double a, double b):             # <<<<<<<<<<<<<<
  *     return uniform_real_variate(a, b)
  * 
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_13random_double, 0, __pyx_n_s_random_double, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__13)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 43, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_17random_double, 0, __pyx_n_s_random_double, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__18)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 68, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_random_double, __pyx_t_1) < 0) __PYX_ERR(0, 43, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_random_double, __pyx_t_1) < 0) __PYX_ERR(0, 68, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "nazo_rand/nazo_rand.pyx":47
+  /* "nazo_rand/nazo_rand.pyx":72
  * 
  * 
  * cpdef double random_double_noargs():             # <<<<<<<<<<<<<<
  *     return uniform_real_variate_noargs()
  */
-  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_15random_double_noargs, 0, __pyx_n_s_random_double_noargs, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__14)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 47, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_CyFunction_New(&__pyx_mdef_9nazo_rand_9nazo_rand_19random_double_noargs, 0, __pyx_n_s_random_double_noargs, NULL, __pyx_n_s_nazo_rand_nazo_rand, __pyx_d, ((PyObject *)__pyx_codeobj__19)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_random_double_noargs, __pyx_t_1) < 0) __PYX_ERR(0, 47, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_random_double_noargs, __pyx_t_1) < 0) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "nazo_rand/nazo_rand.pyx":1
  * # cython: language_level=3             # <<<<<<<<<<<<<<
  * # distutils: language = c++
  * cimport cython
  */
@@ -3152,101 +3708,14 @@
     }
     PyErr_Format(PyExc_TypeError,
         "Argument '%.200s' has incorrect type (expected %.200s, got %.200s)",
         name, type->tp_name, Py_TYPE(obj)->tp_name);
     return 0;
 }
 
-/* GetItemInt */
-static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j) {
-    PyObject *r;
-    if (!j) return NULL;
-    r = PyObject_GetItem(o, j);
-    Py_DECREF(j);
-    return r;
-}
-static CYTHON_INLINE PyObject *__Pyx_GetItemInt_List_Fast(PyObject *o, Py_ssize_t i,
-                                                              CYTHON_NCP_UNUSED int wraparound,
-                                                              CYTHON_NCP_UNUSED int boundscheck) {
-#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    Py_ssize_t wrapped_i = i;
-    if (wraparound & unlikely(i < 0)) {
-        wrapped_i += PyList_GET_SIZE(o);
-    }
-    if ((!boundscheck) || likely(__Pyx_is_valid_index(wrapped_i, PyList_GET_SIZE(o)))) {
-        PyObject *r = PyList_GET_ITEM(o, wrapped_i);
-        Py_INCREF(r);
-        return r;
-    }
-    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
-#else
-    return PySequence_GetItem(o, i);
-#endif
-}
-static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Tuple_Fast(PyObject *o, Py_ssize_t i,
-                                                              CYTHON_NCP_UNUSED int wraparound,
-                                                              CYTHON_NCP_UNUSED int boundscheck) {
-#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    Py_ssize_t wrapped_i = i;
-    if (wraparound & unlikely(i < 0)) {
-        wrapped_i += PyTuple_GET_SIZE(o);
-    }
-    if ((!boundscheck) || likely(__Pyx_is_valid_index(wrapped_i, PyTuple_GET_SIZE(o)))) {
-        PyObject *r = PyTuple_GET_ITEM(o, wrapped_i);
-        Py_INCREF(r);
-        return r;
-    }
-    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
-#else
-    return PySequence_GetItem(o, i);
-#endif
-}
-static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Fast(PyObject *o, Py_ssize_t i, int is_list,
-                                                     CYTHON_NCP_UNUSED int wraparound,
-                                                     CYTHON_NCP_UNUSED int boundscheck) {
-#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS && CYTHON_USE_TYPE_SLOTS
-    if (is_list || PyList_CheckExact(o)) {
-        Py_ssize_t n = ((!wraparound) | likely(i >= 0)) ? i : i + PyList_GET_SIZE(o);
-        if ((!boundscheck) || (likely(__Pyx_is_valid_index(n, PyList_GET_SIZE(o))))) {
-            PyObject *r = PyList_GET_ITEM(o, n);
-            Py_INCREF(r);
-            return r;
-        }
-    }
-    else if (PyTuple_CheckExact(o)) {
-        Py_ssize_t n = ((!wraparound) | likely(i >= 0)) ? i : i + PyTuple_GET_SIZE(o);
-        if ((!boundscheck) || likely(__Pyx_is_valid_index(n, PyTuple_GET_SIZE(o)))) {
-            PyObject *r = PyTuple_GET_ITEM(o, n);
-            Py_INCREF(r);
-            return r;
-        }
-    } else {
-        PySequenceMethods *m = Py_TYPE(o)->tp_as_sequence;
-        if (likely(m && m->sq_item)) {
-            if (wraparound && unlikely(i < 0) && likely(m->sq_length)) {
-                Py_ssize_t l = m->sq_length(o);
-                if (likely(l >= 0)) {
-                    i += l;
-                } else {
-                    if (!PyErr_ExceptionMatches(PyExc_OverflowError))
-                        return NULL;
-                    PyErr_Clear();
-                }
-            }
-            return m->sq_item(o, i);
-        }
-    }
-#else
-    if (is_list || PySequence_Check(o)) {
-        return PySequence_GetItem(o, i);
-    }
-#endif
-    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
-}
-
 /* RaiseArgTupleInvalid */
 static void __Pyx_RaiseArgtupleInvalid(
     const char* func_name,
     int exact,
     Py_ssize_t num_min,
     Py_ssize_t num_max,
     Py_ssize_t num_found)
@@ -3381,14 +3850,280 @@
         "%s() got an unexpected keyword argument '%U'",
         function_name, key);
     #endif
 bad:
     return -1;
 }
 
+/* GetItemInt */
+static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j) {
+    PyObject *r;
+    if (!j) return NULL;
+    r = PyObject_GetItem(o, j);
+    Py_DECREF(j);
+    return r;
+}
+static CYTHON_INLINE PyObject *__Pyx_GetItemInt_List_Fast(PyObject *o, Py_ssize_t i,
+                                                              CYTHON_NCP_UNUSED int wraparound,
+                                                              CYTHON_NCP_UNUSED int boundscheck) {
+#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+    Py_ssize_t wrapped_i = i;
+    if (wraparound & unlikely(i < 0)) {
+        wrapped_i += PyList_GET_SIZE(o);
+    }
+    if ((!boundscheck) || likely(__Pyx_is_valid_index(wrapped_i, PyList_GET_SIZE(o)))) {
+        PyObject *r = PyList_GET_ITEM(o, wrapped_i);
+        Py_INCREF(r);
+        return r;
+    }
+    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
+#else
+    return PySequence_GetItem(o, i);
+#endif
+}
+static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Tuple_Fast(PyObject *o, Py_ssize_t i,
+                                                              CYTHON_NCP_UNUSED int wraparound,
+                                                              CYTHON_NCP_UNUSED int boundscheck) {
+#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
+    Py_ssize_t wrapped_i = i;
+    if (wraparound & unlikely(i < 0)) {
+        wrapped_i += PyTuple_GET_SIZE(o);
+    }
+    if ((!boundscheck) || likely(__Pyx_is_valid_index(wrapped_i, PyTuple_GET_SIZE(o)))) {
+        PyObject *r = PyTuple_GET_ITEM(o, wrapped_i);
+        Py_INCREF(r);
+        return r;
+    }
+    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
+#else
+    return PySequence_GetItem(o, i);
+#endif
+}
+static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Fast(PyObject *o, Py_ssize_t i, int is_list,
+                                                     CYTHON_NCP_UNUSED int wraparound,
+                                                     CYTHON_NCP_UNUSED int boundscheck) {
+#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS && CYTHON_USE_TYPE_SLOTS
+    if (is_list || PyList_CheckExact(o)) {
+        Py_ssize_t n = ((!wraparound) | likely(i >= 0)) ? i : i + PyList_GET_SIZE(o);
+        if ((!boundscheck) || (likely(__Pyx_is_valid_index(n, PyList_GET_SIZE(o))))) {
+            PyObject *r = PyList_GET_ITEM(o, n);
+            Py_INCREF(r);
+            return r;
+        }
+    }
+    else if (PyTuple_CheckExact(o)) {
+        Py_ssize_t n = ((!wraparound) | likely(i >= 0)) ? i : i + PyTuple_GET_SIZE(o);
+        if ((!boundscheck) || likely(__Pyx_is_valid_index(n, PyTuple_GET_SIZE(o)))) {
+            PyObject *r = PyTuple_GET_ITEM(o, n);
+            Py_INCREF(r);
+            return r;
+        }
+    } else {
+        PySequenceMethods *m = Py_TYPE(o)->tp_as_sequence;
+        if (likely(m && m->sq_item)) {
+            if (wraparound && unlikely(i < 0) && likely(m->sq_length)) {
+                Py_ssize_t l = m->sq_length(o);
+                if (likely(l >= 0)) {
+                    i += l;
+                } else {
+                    if (!PyErr_ExceptionMatches(PyExc_OverflowError))
+                        return NULL;
+                    PyErr_Clear();
+                }
+            }
+            return m->sq_item(o, i);
+        }
+    }
+#else
+    if (is_list || PySequence_Check(o)) {
+        return PySequence_GetItem(o, i);
+    }
+#endif
+    return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
+}
+
+/* PyObjectCall */
+#if CYTHON_COMPILING_IN_CPYTHON
+static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw) {
+    PyObject *result;
+    ternaryfunc call = Py_TYPE(func)->tp_call;
+    if (unlikely(!call))
+        return PyObject_Call(func, arg, kw);
+    if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
+        return NULL;
+    result = (*call)(func, arg, kw);
+    Py_LeaveRecursiveCall();
+    if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
+        PyErr_SetString(
+            PyExc_SystemError,
+            "NULL result without error in PyObject_Call");
+    }
+    return result;
+}
+#endif
+
+/* RaiseException */
+#if PY_MAJOR_VERSION < 3
+static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb,
+                        CYTHON_UNUSED PyObject *cause) {
+    __Pyx_PyThreadState_declare
+    Py_XINCREF(type);
+    if (!value || value == Py_None)
+        value = NULL;
+    else
+        Py_INCREF(value);
+    if (!tb || tb == Py_None)
+        tb = NULL;
+    else {
+        Py_INCREF(tb);
+        if (!PyTraceBack_Check(tb)) {
+            PyErr_SetString(PyExc_TypeError,
+                "raise: arg 3 must be a traceback or None");
+            goto raise_error;
+        }
+    }
+    if (PyType_Check(type)) {
+#if CYTHON_COMPILING_IN_PYPY
+        if (!value) {
+            Py_INCREF(Py_None);
+            value = Py_None;
+        }
+#endif
+        PyErr_NormalizeException(&type, &value, &tb);
+    } else {
+        if (value) {
+            PyErr_SetString(PyExc_TypeError,
+                "instance exception may not have a separate value");
+            goto raise_error;
+        }
+        value = type;
+        type = (PyObject*) Py_TYPE(type);
+        Py_INCREF(type);
+        if (!PyType_IsSubtype((PyTypeObject *)type, (PyTypeObject *)PyExc_BaseException)) {
+            PyErr_SetString(PyExc_TypeError,
+                "raise: exception class must be a subclass of BaseException");
+            goto raise_error;
+        }
+    }
+    __Pyx_PyThreadState_assign
+    __Pyx_ErrRestore(type, value, tb);
+    return;
+raise_error:
+    Py_XDECREF(value);
+    Py_XDECREF(type);
+    Py_XDECREF(tb);
+    return;
+}
+#else
+static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause) {
+    PyObject* owned_instance = NULL;
+    if (tb == Py_None) {
+        tb = 0;
+    } else if (tb && !PyTraceBack_Check(tb)) {
+        PyErr_SetString(PyExc_TypeError,
+            "raise: arg 3 must be a traceback or None");
+        goto bad;
+    }
+    if (value == Py_None)
+        value = 0;
+    if (PyExceptionInstance_Check(type)) {
+        if (value) {
+            PyErr_SetString(PyExc_TypeError,
+                "instance exception may not have a separate value");
+            goto bad;
+        }
+        value = type;
+        type = (PyObject*) Py_TYPE(value);
+    } else if (PyExceptionClass_Check(type)) {
+        PyObject *instance_class = NULL;
+        if (value && PyExceptionInstance_Check(value)) {
+            instance_class = (PyObject*) Py_TYPE(value);
+            if (instance_class != type) {
+                int is_subclass = PyObject_IsSubclass(instance_class, type);
+                if (!is_subclass) {
+                    instance_class = NULL;
+                } else if (unlikely(is_subclass == -1)) {
+                    goto bad;
+                } else {
+                    type = instance_class;
+                }
+            }
+        }
+        if (!instance_class) {
+            PyObject *args;
+            if (!value)
+                args = PyTuple_New(0);
+            else if (PyTuple_Check(value)) {
+                Py_INCREF(value);
+                args = value;
+            } else
+                args = PyTuple_Pack(1, value);
+            if (!args)
+                goto bad;
+            owned_instance = PyObject_Call(type, args, NULL);
+            Py_DECREF(args);
+            if (!owned_instance)
+                goto bad;
+            value = owned_instance;
+            if (!PyExceptionInstance_Check(value)) {
+                PyErr_Format(PyExc_TypeError,
+                             "calling %R should have returned an instance of "
+                             "BaseException, not %R",
+                             type, Py_TYPE(value));
+                goto bad;
+            }
+        }
+    } else {
+        PyErr_SetString(PyExc_TypeError,
+            "raise: exception class must be a subclass of BaseException");
+        goto bad;
+    }
+    if (cause) {
+        PyObject *fixed_cause;
+        if (cause == Py_None) {
+            fixed_cause = NULL;
+        } else if (PyExceptionClass_Check(cause)) {
+            fixed_cause = PyObject_CallObject(cause, NULL);
+            if (fixed_cause == NULL)
+                goto bad;
+        } else if (PyExceptionInstance_Check(cause)) {
+            fixed_cause = cause;
+            Py_INCREF(fixed_cause);
+        } else {
+            PyErr_SetString(PyExc_TypeError,
+                            "exception causes must derive from "
+                            "BaseException");
+            goto bad;
+        }
+        PyException_SetCause(value, fixed_cause);
+    }
+    PyErr_SetObject(type, value);
+    if (tb) {
+#if CYTHON_FAST_THREAD_STATE
+        PyThreadState *tstate = __Pyx_PyThreadState_Current;
+        PyObject* tmp_tb = tstate->curexc_traceback;
+        if (tb != tmp_tb) {
+            Py_INCREF(tb);
+            tstate->curexc_traceback = tb;
+            Py_XDECREF(tmp_tb);
+        }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
+#endif
+    }
+bad:
+    Py_XDECREF(owned_instance);
+    return;
+}
+#endif
+
 /* FetchCommonType */
 static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type) {
     PyObject* fake_module;
     PyTypeObject* cached_type = NULL;
     fake_module = PyImport_AddModule((char*) "_cython_" CYTHON_ABI);
     if (!fake_module) return NULL;
     Py_INCREF(fake_module);
```

### Comparing `nazo_rand-0.0.5/nazo_rand/nazo_rand.hpp` & `nazo_rand-0.0.6/nazo_rand/nazo_rand.hpp`

 * *Files identical despite different names*

### Comparing `nazo_rand-0.0.5/nazo_rand/nazo_rand.pyi` & `nazo_rand-0.0.6/nazo_rand/nazo_rand.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -5,14 +5,26 @@
     """清洗列表中的元素，使其随机排列。
 
     Args:
         array (list): 要清洗的列表。
     """
     ...
 
+def random_sample(container: Union[list, tuple, str, bytes], count: int) -> list[Any]:
+    """从容器中随机抽取count个元素。
+
+    Args:
+        container (Union[list, tuple, str, bytes]): 要抽取的容器。
+        count (int): 要抽取的元素个数。
+
+    Returns:
+        list[Any]: 抽取的元素。
+
+    """
+
 def random_integer_noargs() -> int:
     """生成一个随机整数
 
     Returns:
         int: 随机整数。
     """
     ...
@@ -24,25 +36,37 @@
         n (int): 范围的上限。
 
     Returns:
         int: 随机整数。
     """
     ...
 
-def random_choice(elements: Union[list, tuple, str, bytes]) -> Any:
+def random_choice(container: Union[list, tuple, str, bytes]) -> Any:
     """从列表、元组、字符串或字节串中随机选择一个元素。
 
     Args:
         elements (Union[list, tuple, str, bytes]): 要选择的元素。
 
     Returns:
         Any: 随机选择的元素。
     """
     ...
 
+def random_choices(container: Union[list, tuple, str, bytes], count: int) -> list[Any]:
+    """从列表、元组、字符串或字节串中随机选择count个元素。
+
+    Args:
+        elements (Union[list, tuple, str, bytes]): 要选择的元素。
+        count (int): 选择的元素个数。
+
+    Returns:
+        list[Any]: 随机选择的元素。
+    """
+    ...
+
 def randint(min: int, max: int) -> int:
     """返回一个随机整数，范围是[min, max]。
 
     Args:
         min (int): 最小值。
         max (int): 最大值。
```

### Comparing `nazo_rand-0.0.5/nazo_rand/nazo_rand.pyx` & `nazo_rand-0.0.6/nazo_rand/nazo_rand.pyx`

 * *Files 20% similar despite different names*

```diff
@@ -20,23 +20,48 @@
         j = randrange(i, len(array), 1)
         array[i], array[j] = array[j], array[i]
 
 
 cpdef int randbelow(int a):
     return random_below(a)
 
+cpdef int randint(int a, int b):
+    return uniform_int_variate(a, b)
+
+
+
+@cython.boundscheck(False)
+@cython.wraparound(False)
+cpdef object random_choice(object container):
+    cdef Py_ssize_t index = randbelow(len(container))
+    return container[index]
+
 @cython.boundscheck(False)
 @cython.wraparound(False)
-cpdef object random_choice(object elements):
-    cdef Py_ssize_t index = randbelow(len(elements))
-    return elements[index]
+cpdef list[object] random_choices(object container, Py_ssize_t count):
+    cdef Py_ssize_t container_length = len(container)
+    return [container[randbelow(container_length)] for _ in range(count)]
 
+@cython.boundscheck(False)
+@cython.wraparound(False)
+cpdef list[object] random_sample(object container, Py_ssize_t count):
+    cdef Py_ssize_t container_length = len(container)
+    cdef Py_ssize_t i, j
+    cdef list result = [None] * count
+    cdef list temp = list(container)
+
+    if count > container_length:
+        raise ValueError("Sample larger than population")
+
+    for i in range(count):
+        j = uniform_int_variate(i, container_length - 1)
+        result[i] = temp[j]
+        temp[j] = temp[i]
 
-cpdef int randint(int a, int b):
-    return uniform_int_variate(a, b)
+    return result
 
 cpdef int randrange(int start, int stop=0, int step=1):
     if stop == 0:
         stop, start = start, 0
     return random_range(start, stop, step)
```

### Comparing `nazo_rand-0.0.5/nazo_rand.egg-info/PKG-INFO` & `nazo_rand-0.0.6/nazo_rand.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nazo-rand
-Version: 0.0.5
+Version: 0.0.6
 Summary: A fast random number generator for python
 Author: bymoye
 Author-email: s3moye@gmail.com
 License: Free for non-commercial use
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `nazo_rand-0.0.5/setup.py` & `nazo_rand-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
             "wraparound": False,
             "binding": True,
             "cdivision": True,
         },
     ),
     author="bymoye",
     author_email="s3moye@gmail.com",
-    version="0.0.5",
+    version="0.0.6",
     description="A fast random number generator for python",
     long_description=readme(),
     long_description_content_type="text/markdown",
     license="Free for non-commercial use",
     package_data={
         "": [
             "nazo_rand/nazo_rand.pyi",
```

