# Comparing `tmp/scikit_build_core-0.3.0.tar.gz` & `tmp/scikit_build_core-0.3.1.tar.gz`

## Comparing `scikit_build_core-0.3.0.tar` & `scikit_build_core-0.3.1.tar`

### file list

```diff
@@ -1,215 +1,215 @@
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/.git_archival.txt
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/.gitattributes
--rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/.packit.yaml
--rw-r--r--   0        0        0     3189 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/.readthedocs.yml
--rw-r--r--   0        0        0     3189 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/noxfile.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/.distro/python-scikit-build-core.rpmlintrc
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/.distro/scikit-build-core.spec
--rw-r--r--   0        0        0     8828 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/.github/codecov.yml
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/.github/matchers/pylint.json
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/.github/workflows/cd.yml
--rw-r--r--   0        0        0     6765 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0    11915 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/changelog.md
--rw-r--r--   0        0        0     2882 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/cmakelists.md
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/conf.py
--rw-r--r--   0        0        0    12029 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/configuration.md
--rw-r--r--   0        0        0     9065 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/getting_started.md
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/index.md
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/api/scikit_build_core.build.rst
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/api/scikit_build_core.builder.rst
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/api/scikit_build_core.file_api.model.rst
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/api/scikit_build_core.file_api.rst
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/api/scikit_build_core.metadata.rst
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/api/scikit_build_core.resources.find_python.rst
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/api/scikit_build_core.resources.rst
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/api/scikit_build_core.rst
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/api/scikit_build_core.settings.rst
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/api/scikit_build_core.setuptools.rst
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/examples/getting_started/test.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/examples/getting_started/abi3/CMakeLists.txt
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/examples/getting_started/abi3/example.c
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/examples/getting_started/abi3/pyproject.toml
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/examples/getting_started/c/CMakeLists.txt
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/examples/getting_started/c/example.c
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/examples/getting_started/c/pyproject.toml
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/examples/getting_started/cython/CMakeLists.txt
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/examples/getting_started/cython/example.pyx
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/examples/getting_started/cython/pyproject.toml
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/examples/getting_started/fortran/CMakeLists.txt
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/examples/getting_started/fortran/example.f
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/examples/getting_started/fortran/pyproject.toml
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/examples/getting_started/pybind11/CMakeLists.txt
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/examples/getting_started/pybind11/example.cpp
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/examples/getting_started/pybind11/pyproject.toml
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/examples/getting_started/swig/CMakeLists.txt
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/examples/getting_started/swig/example.c
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/examples/getting_started/swig/example.i
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/docs/examples/getting_started/swig/pyproject.toml
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/__init__.py
--rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/_logging.py
--rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/_shutil.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/_version.py
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/_version.pyi
--rw-r--r--   0        0        0     8478 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/cmake.py
--rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/errors.py
--rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/program_search.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/py.typed
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/_compat/__init__.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/_compat/builtins.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/_compat/tomllib.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/_compat/typing.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/_compat/importlib/__init__.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/_compat/importlib/metadata.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/_compat/importlib/resources.py
--rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/build/__init__.py
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/build/_file_processor.py
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/build/_init.py
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/build/_pathutil.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/build/_scripts.py
--rw-r--r--   0        0        0     7458 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/build/_wheelfile.py
--rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/build/sdist.py
--rw-r--r--   0        0        0     9066 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/build/wheel.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/builder/__init__.py
--rw-r--r--   0        0        0     6979 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/builder/builder.py
--rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/builder/generator.py
--rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/builder/get_requires.py
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/builder/macos.py
--rw-r--r--   0        0        0     4223 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/builder/sysconfig.py
--rw-r--r--   0        0        0     4290 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/builder/wheel_tag.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/file_api/__init__.py
--rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/file_api/_cattrs_converter.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/file_api/query.py
--rw-r--r--   0        0        0     4017 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/file_api/reply.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/file_api/model/__init__.py
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/file_api/model/cache.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/file_api/model/cmakefiles.py
--rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/file_api/model/codemodel.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/file_api/model/common.py
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/file_api/model/directory.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/file_api/model/index.py
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/file_api/model/toolchains.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/metadata/__init__.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/metadata/fancy_pypi_readme.py
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/metadata/setuptools_scm.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/resources/__init__.py
--rw-r--r--   0        0        0     3773 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/resources/_editable_redirect.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/resources/known_wheels.toml
--rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/resources/find_python/Copyright.txt
--rw-r--r--   0        0        0    23174 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/resources/find_python/FindPackageHandleStandardArgs.cmake
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/resources/find_python/FindPackageMessage.cmake
--rw-r--r--   0        0        0    22536 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/resources/find_python/FindPython.cmake
--rw-r--r--   0        0        0    19036 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/resources/find_python/FindPython3.cmake
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/resources/find_python/__init__.py
--rw-r--r--   0        0        0   198528 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/resources/find_python/FindPython/Support.cmake
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/settings/__init__.py
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/settings/_load_provider.py
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/settings/metadata.py
--rw-r--r--   0        0        0     5256 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/settings/skbuild_model.py
--rw-r--r--   0        0        0     4916 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/settings/skbuild_read_settings.py
--rw-r--r--   0        0        0    16489 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/settings/sources.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/setuptools/__init__.py
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/setuptools/build_meta.py
--rw-r--r--   0        0        0     5503 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/src/scikit_build_core/setuptools/extension.py
--rw-r--r--   0        0        0     8775 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/conftest.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/constraints.txt
--rw-r--r--   0        0        0     6428 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/test_builder.py
--rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/test_cmake_config.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/test_custom_modules.py
--rw-r--r--   0        0        0     8426 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/test_dynamic_metadata.py
--rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/test_fileapi.py
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/test_fortran.py
--rw-r--r--   0        0        0    15811 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/test_generator_default.py
--rw-r--r--   0        0        0     2827 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/test_get_requires.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/test_logging.py
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/test_module_dir.py
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/test_name_main.py
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/test_prepare_metadata.py
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/test_process_scripts.py
--rw-r--r--   0        0        0     4009 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/test_program_search.py
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/test_pyproject_abi3.py
--rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/test_pyproject_extra_dirs.py
--rw-r--r--   0        0        0     6414 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/test_pyproject_pep517.py
--rw-r--r--   0        0        0     4396 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/test_pyproject_pep518.py
--rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/test_pyproject_pep660.py
--rw-r--r--   0        0        0    14021 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/test_settings.py
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/test_setuptools_abi3.py
--rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/test_setuptools_pep517.py
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/test_setuptools_pep518.py
--rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/test_simple_pure.py
--rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/test_simplest_c.py
--rw-r--r--   0        0        0    11951 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/test_skbuild_settings.py
--rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/test_wheelfile_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/api/simple_pure/.cmake/api/v1/query/cache-v2
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/api/simple_pure/.cmake/api/v1/query/cmakeFiles-v1
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/api/simple_pure/.cmake/api/v1/query/codemodel-v2
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/api/simple_pure/.cmake/api/v1/query/toolchains-v1
--rw-r--r--   0        0        0    20671 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/api/simple_pure/.cmake/api/v1/reply/cache-v2-2dececcab32f1eda138d.json
--rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/api/simple_pure/.cmake/api/v1/reply/cmakeFiles-v1-74870fd87af7f965b597.json
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/api/simple_pure/.cmake/api/v1/reply/codemodel-v2-ea39b5a28cb1a3e0a069.json
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/api/simple_pure/.cmake/api/v1/reply/directory-.-5e7a28751b0c9235cbe7.json
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/api/simple_pure/.cmake/api/v1/reply/index-2022-09-12T15-23-13-0135.json
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/api/simple_pure/.cmake/api/v1/reply/target-simple_pure-7eb73eb5c359b881e083.json
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/api/simple_pure/.cmake/api/v1/reply/toolchains-v1-06b92b86597808b5f980.json
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/abi3_pyproject_ext/CMakeLists.txt
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/abi3_pyproject_ext/abi3_example.c
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/abi3_pyproject_ext/pyproject.toml
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/abi3_setuptools_ext/CMakeLists.txt
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/abi3_setuptools_ext/abi3_example.c
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/abi3_setuptools_ext/pyproject.toml
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/abi3_setuptools_ext/setup.cfg
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/abi3_setuptools_ext/setup.py
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/custom_cmake/CMakeLists.txt
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/custom_cmake/pyproject.toml
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/custom_cmake/extern/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/__init__.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_modules/ExampleInclude.cmake
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_modules/__init__.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_prefix/ExamplePkgConfig.cmake
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_prefix/__init__.py
--rwxr-xr-x   0        0        0       80 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/custom_cmake/scripts/script1
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/dynamic_metadata/CMakeLists.txt
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/dynamic_metadata/dual_project.toml
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/dynamic_metadata/faulty_dual_project.toml
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/dynamic_metadata/faulty_project.toml
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/dynamic_metadata/local_pyproject.toml
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/dynamic_metadata/plugin_project.toml
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/dynamic_metadata/pyproject.toml
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/dynamic_metadata/warn_project.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/dynamic_metadata/plugins/local/version/__init__.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/dynamic_metadata/plugins/local/version/nested/__init__.py
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/dynamic_metadata/src/module.c
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/dynamic_metadata/src/dynamic/__init__.py
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/filepath_pure/CMakeLists.txt
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/filepath_pure/pyproject.toml
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/fortran_example/CMakeLists.txt
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/fortran_example/fib1.f
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/fortran_example/pyproject.toml
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/simple_pure/CMakeLists.txt
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/simple_pure/simple_pure.cpp
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/simple_pyproject_ext/CMakeLists.txt
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/simple_pyproject_ext/pyproject.toml
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/simple_pyproject_ext/src/main.cpp
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/simple_setuptools_ext/CMakeLists.txt
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/simple_setuptools_ext/pyproject.toml
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/simple_setuptools_ext/setup.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/simple_setuptools_ext/src/main.cpp
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/simplest_c/.gitignore
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/simplest_c/CMakeLists.txt
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/simplest_c/pyproject.toml
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/simplest_c/src/module.c
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/simplest_c/src/not_a_package/simple.txt
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/simplest_c/src/simplest/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/simplest_c/src/simplest/artifact_ignored.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/simplest_c/src/simplest/data.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/simplest_c/src/simplest/excluded.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/simplest_c/src/simplest/ignored.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/simplest_c/src/simplest/ignored_included.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/tests/packages/simplest_c/src/simplest/sdist_only.txt
--rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/.gitignore
--rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/LICENSE
--rw-r--r--   0        0        0     9505 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/README.md
--rw-r--r--   0        0        0     6112 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/pyproject.toml
--rw-r--r--   0        0        0    12297 2020-02-02 00:00:00.000000 scikit_build_core-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/.git_archival.txt
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/.gitattributes
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/.packit.yaml
+-rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/.readthedocs.yml
+-rw-r--r--   0        0        0     3189 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/noxfile.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/.distro/python-scikit-build-core.rpmlintrc
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/.distro/scikit-build-core.spec
+-rw-r--r--   0        0        0     8835 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/.github/codecov.yml
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/.github/matchers/pylint.json
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     6765 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0    12468 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/changelog.md
+-rw-r--r--   0        0        0     2882 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/cmakelists.md
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/conf.py
+-rw-r--r--   0        0        0    12069 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/configuration.md
+-rw-r--r--   0        0        0     9066 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/getting_started.md
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/index.md
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/api/scikit_build_core.build.rst
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/api/scikit_build_core.builder.rst
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/api/scikit_build_core.file_api.model.rst
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/api/scikit_build_core.file_api.rst
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/api/scikit_build_core.metadata.rst
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/api/scikit_build_core.resources.find_python.rst
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/api/scikit_build_core.resources.rst
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/api/scikit_build_core.rst
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/api/scikit_build_core.settings.rst
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/api/scikit_build_core.setuptools.rst
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/examples/getting_started/test.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/examples/getting_started/abi3/CMakeLists.txt
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/examples/getting_started/abi3/example.c
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/examples/getting_started/abi3/pyproject.toml
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/examples/getting_started/c/CMakeLists.txt
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/examples/getting_started/c/example.c
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/examples/getting_started/c/pyproject.toml
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/examples/getting_started/cython/CMakeLists.txt
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/examples/getting_started/cython/example.pyx
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/examples/getting_started/cython/pyproject.toml
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/examples/getting_started/fortran/CMakeLists.txt
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/examples/getting_started/fortran/example.f
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/examples/getting_started/fortran/pyproject.toml
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/examples/getting_started/pybind11/CMakeLists.txt
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/examples/getting_started/pybind11/example.cpp
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/examples/getting_started/pybind11/pyproject.toml
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/examples/getting_started/swig/CMakeLists.txt
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/examples/getting_started/swig/example.c
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/examples/getting_started/swig/example.i
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/docs/examples/getting_started/swig/pyproject.toml
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/__init__.py
+-rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/_logging.py
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/_shutil.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/_version.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/_version.pyi
+-rw-r--r--   0        0        0     8478 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/cmake.py
+-rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/errors.py
+-rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/program_search.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/py.typed
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/_compat/__init__.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/_compat/builtins.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/_compat/tomllib.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/_compat/typing.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/_compat/importlib/__init__.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/_compat/importlib/metadata.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/_compat/importlib/resources.py
+-rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/build/__init__.py
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/build/_file_processor.py
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/build/_init.py
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/build/_pathutil.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/build/_scripts.py
+-rw-r--r--   0        0        0     7458 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/build/_wheelfile.py
+-rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/build/sdist.py
+-rw-r--r--   0        0        0     9066 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/build/wheel.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/builder/__init__.py
+-rw-r--r--   0        0        0     7089 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/builder/builder.py
+-rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/builder/generator.py
+-rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/builder/get_requires.py
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/builder/macos.py
+-rw-r--r--   0        0        0     4223 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/builder/sysconfig.py
+-rw-r--r--   0        0        0     4290 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/builder/wheel_tag.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/file_api/__init__.py
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/file_api/_cattrs_converter.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/file_api/query.py
+-rw-r--r--   0        0        0     4017 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/file_api/reply.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/file_api/model/__init__.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/file_api/model/cache.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/file_api/model/cmakefiles.py
+-rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/file_api/model/codemodel.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/file_api/model/common.py
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/file_api/model/directory.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/file_api/model/index.py
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/file_api/model/toolchains.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/metadata/__init__.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/metadata/fancy_pypi_readme.py
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/metadata/setuptools_scm.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/resources/__init__.py
+-rw-r--r--   0        0        0     3773 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/resources/_editable_redirect.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/resources/known_wheels.toml
+-rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/resources/find_python/Copyright.txt
+-rw-r--r--   0        0        0    23174 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/resources/find_python/FindPackageHandleStandardArgs.cmake
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/resources/find_python/FindPackageMessage.cmake
+-rw-r--r--   0        0        0    22536 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/resources/find_python/FindPython.cmake
+-rw-r--r--   0        0        0    19036 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/resources/find_python/FindPython3.cmake
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/resources/find_python/__init__.py
+-rw-r--r--   0        0        0   198528 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/resources/find_python/FindPython/Support.cmake
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/settings/__init__.py
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/settings/_load_provider.py
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/settings/metadata.py
+-rw-r--r--   0        0        0     5256 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/settings/skbuild_model.py
+-rw-r--r--   0        0        0     4916 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/settings/skbuild_read_settings.py
+-rw-r--r--   0        0        0    16489 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/settings/sources.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/setuptools/__init__.py
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/setuptools/build_meta.py
+-rw-r--r--   0        0        0     5503 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/src/scikit_build_core/setuptools/extension.py
+-rw-r--r--   0        0        0     8775 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/conftest.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/constraints.txt
+-rw-r--r--   0        0        0     6428 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/test_builder.py
+-rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/test_cmake_config.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/test_custom_modules.py
+-rw-r--r--   0        0        0     8426 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/test_dynamic_metadata.py
+-rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/test_fileapi.py
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/test_fortran.py
+-rw-r--r--   0        0        0    15811 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/test_generator_default.py
+-rw-r--r--   0        0        0     2827 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/test_get_requires.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/test_logging.py
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/test_module_dir.py
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/test_name_main.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/test_prepare_metadata.py
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/test_process_scripts.py
+-rw-r--r--   0        0        0     4009 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/test_program_search.py
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/test_pyproject_abi3.py
+-rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/test_pyproject_extra_dirs.py
+-rw-r--r--   0        0        0     6414 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/test_pyproject_pep517.py
+-rw-r--r--   0        0        0     4396 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/test_pyproject_pep518.py
+-rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/test_pyproject_pep660.py
+-rw-r--r--   0        0        0    14021 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/test_settings.py
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/test_setuptools_abi3.py
+-rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/test_setuptools_pep517.py
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/test_setuptools_pep518.py
+-rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/test_simple_pure.py
+-rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/test_simplest_c.py
+-rw-r--r--   0        0        0    11951 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/test_skbuild_settings.py
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/test_wheelfile_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/api/simple_pure/.cmake/api/v1/query/cache-v2
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/api/simple_pure/.cmake/api/v1/query/cmakeFiles-v1
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/api/simple_pure/.cmake/api/v1/query/codemodel-v2
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/api/simple_pure/.cmake/api/v1/query/toolchains-v1
+-rw-r--r--   0        0        0    20671 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/api/simple_pure/.cmake/api/v1/reply/cache-v2-2dececcab32f1eda138d.json
+-rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/api/simple_pure/.cmake/api/v1/reply/cmakeFiles-v1-74870fd87af7f965b597.json
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/api/simple_pure/.cmake/api/v1/reply/codemodel-v2-ea39b5a28cb1a3e0a069.json
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/api/simple_pure/.cmake/api/v1/reply/directory-.-5e7a28751b0c9235cbe7.json
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/api/simple_pure/.cmake/api/v1/reply/index-2022-09-12T15-23-13-0135.json
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/api/simple_pure/.cmake/api/v1/reply/target-simple_pure-7eb73eb5c359b881e083.json
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/api/simple_pure/.cmake/api/v1/reply/toolchains-v1-06b92b86597808b5f980.json
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/abi3_pyproject_ext/CMakeLists.txt
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/abi3_pyproject_ext/abi3_example.c
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/abi3_pyproject_ext/pyproject.toml
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/abi3_setuptools_ext/CMakeLists.txt
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/abi3_setuptools_ext/abi3_example.c
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/abi3_setuptools_ext/pyproject.toml
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/abi3_setuptools_ext/setup.cfg
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/abi3_setuptools_ext/setup.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/custom_cmake/CMakeLists.txt
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/custom_cmake/pyproject.toml
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/custom_cmake/extern/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/__init__.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_modules/ExampleInclude.cmake
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_modules/__init__.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_prefix/ExamplePkgConfig.cmake
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_prefix/__init__.py
+-rwxr-xr-x   0        0        0       80 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/custom_cmake/scripts/script1
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/dynamic_metadata/CMakeLists.txt
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/dynamic_metadata/dual_project.toml
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/dynamic_metadata/faulty_dual_project.toml
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/dynamic_metadata/faulty_project.toml
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/dynamic_metadata/local_pyproject.toml
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/dynamic_metadata/plugin_project.toml
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/dynamic_metadata/pyproject.toml
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/dynamic_metadata/warn_project.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/dynamic_metadata/plugins/local/version/__init__.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/dynamic_metadata/plugins/local/version/nested/__init__.py
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/dynamic_metadata/src/module.c
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/dynamic_metadata/src/dynamic/__init__.py
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/filepath_pure/CMakeLists.txt
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/filepath_pure/pyproject.toml
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/fortran_example/CMakeLists.txt
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/fortran_example/fib1.f
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/fortran_example/pyproject.toml
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/simple_pure/CMakeLists.txt
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/simple_pure/simple_pure.cpp
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/simple_pyproject_ext/CMakeLists.txt
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/simple_pyproject_ext/pyproject.toml
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/simple_pyproject_ext/src/main.cpp
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/simple_setuptools_ext/CMakeLists.txt
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/simple_setuptools_ext/pyproject.toml
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/simple_setuptools_ext/setup.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/simple_setuptools_ext/src/main.cpp
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/simplest_c/.gitignore
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/simplest_c/CMakeLists.txt
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/simplest_c/pyproject.toml
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/simplest_c/src/module.c
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/simplest_c/src/not_a_package/simple.txt
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/simplest_c/src/simplest/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/simplest_c/src/simplest/artifact_ignored.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/simplest_c/src/simplest/data.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/simplest_c/src/simplest/excluded.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/simplest_c/src/simplest/ignored.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/simplest_c/src/simplest/ignored_included.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/tests/packages/simplest_c/src/simplest/sdist_only.txt
+-rw-r--r--   0        0        0     2432 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/.gitignore
+-rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/LICENSE
+-rw-r--r--   0        0        0     9505 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/README.md
+-rw-r--r--   0        0        0     6112 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0    12297 2020-02-02 00:00:00.000000 scikit_build_core-0.3.1/PKG-INFO
```

### Comparing `scikit_build_core-0.3.0/.packit.yaml` & `scikit_build_core-0.3.1/.packit.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -41,16 +41,19 @@
       - fedora-development-x86_64
       - fedora-latest-x86_64
       - fedora-development-aarch64
       - fedora-latest-aarch64
   - job: propose_downstream
     trigger: release
     dist_git_branches:
-      - fedora-development
-      - fedora-latest
+      # TODO: Switch to fedora-development and fedora-latest
+      # There is an issue that the commits diverge on different PRs. In the meantime will create PRs on branched fedora
+      # manually
+      # https://github.com/packit/packit/issues/1724
+      - fedora-rawhide
   - job: koji_build
     trigger: commit
     dist_git_branches:
       - fedora-all
   - job: bodhi_update
     trigger: commit
     dist_git_branches:
```

### Comparing `scikit_build_core-0.3.0/.pre-commit-config.yaml` & `scikit_build_core-0.3.1/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -112,7 +112,12 @@
   - repo: local
     hooks:
       - id: disallow-caps
         name: Disallow improper capitalization
         language: pygrep
         entry: PyBind|Numpy|Cmake|CCache|Github|PyTest
         exclude: .pre-commit-config.yaml
+      - id: disallow-expressions
+        name: Disallow expressions
+        language: pygrep
+        entry: tool\.cmake
+        exclude: .pre-commit-config.yaml
```

### Comparing `scikit_build_core-0.3.0/noxfile.py` & `scikit_build_core-0.3.1/noxfile.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/.distro/scikit-build-core.spec` & `scikit_build_core-0.3.1/.distro/scikit-build-core.spec`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/.github/CONTRIBUTING.md` & `scikit_build_core-0.3.1/.github/CONTRIBUTING.md`

 * *Files 1% similar despite different names*

```diff
@@ -175,15 +175,15 @@
 ```python
 {"nested.one": "PEP 517 config"}
 ```
 
 And TOML:
 
 ```toml
-[tool.cmake]
+[tool.scikit-build]
 nested.one = "TOML config"
 ```
 
 The CMake config is pre-configured and available in `.settings.cmake_model`,
 usable as:
 
 ```python
```

### Comparing `scikit_build_core-0.3.0/.github/matchers/pylint.json` & `scikit_build_core-0.3.1/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/.github/workflows/cd.yml` & `scikit_build_core-0.3.1/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/.github/workflows/ci.yml` & `scikit_build_core-0.3.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/docs/changelog.md` & `scikit_build_core-0.3.1/docs/changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,32 @@
 # Changelog
 
+## Version 0.3.1
+
+This is a small release fixing a regression in some cases caused by adding
+`Python_LIBRARY`. This has been reverted on non-Windows platforms, since it is
+only needed on Windows.
+
+### What's Changed
+
+Fixes:
+
+- Support older setuptools-scm by @henryiii in #284
+- Only set the lib for FindPython on Windows by @henryiii in #285
+
+Docs:
+
+- Fix incorrect tool name by @henryiii in #276
+- Typo on tab Fortran (was Cython) by @zerothi in #279
+- Fix wheel.packages by @henryiii in #282
+
+Other:
+
+- Change Fedora PR targets by @LecrisUT in #273
+
 ## Version 0.3.0
 
 This version brings two new dynamic metadata plugins (wrappers for
 `setuptools_scm` & `hatch-pypi-fancy-readme`). Third-party packages can now add
 entry-points declaring `CMAKE_PREFIX_DIR` and `CMAKE_MODULE_DIR` entries.
 Support has been added for requesting metadata without building. And
 experimental support was added for editable installs, including an option for
```

### Comparing `scikit_build_core-0.3.0/docs/cmakelists.md` & `scikit_build_core-0.3.1/docs/cmakelists.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/docs/conf.py` & `scikit_build_core-0.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/docs/configuration.md` & `scikit_build_core-0.3.1/docs/configuration.md`

 * *Files 1% similar despite different names*

```diff
@@ -145,23 +145,23 @@
 ## Customizing the built wheel
 
 The wheel will automatically look for Python packages at `<package_name>` and
 `src/<package_name>`. If you want to list packages explicitly, you can:
 
 ```toml
 [tool.scikit-build]
-packages = ["python/mypackage"]
+wheel.packages = ["python/mypackage"]
 ```
 
 Or you can disable Python file inclusion entirely, and rely only on CMake's
 installs, you can:
 
 ```toml
 [tool.scikit-build]
-packages = []
+wheel.packages = []
 ```
 
 The install directory is normally site-packages; however, you can manually set
 that to a different directory if you'd like to avoid changing your CMake files.
 For example, to mimic scikit-build classic:
 
 ```toml
@@ -318,15 +318,15 @@
 You can also manually specify the exact cmake args. Beyond the normal
 `SKBUILD_CMAKE_ARGS`, the `CMAKE_ARGS` environment variable is also supported
 (with some filtering for options scikit-build-core doesn't support overriding).
 
 ````{tab} pyproject.toml
 
 ```toml
-[tool.cmake]
+[tool.scikit-build]
 cmake.args = ["-DSOME_DEFINE=ON", "-DOTHER=OFF"]
 ```
 
 ````
 
 `````{tab} config-settings
 
@@ -474,15 +474,15 @@
 You can select a custom build dir; by default scikit-build-core will use a
 temporary dir. If you select a persistent one, you can get major rebuild
 speedups.
 
 ````{tab} pyproject.toml
 
 ```toml
-[tool.cmake]
+[tool.scikit-build]
 build-dir = "build/{wheel_tag}"
 ```
 
 ````
 
 `````{tab} config-settings
 
@@ -522,20 +522,20 @@
 
 ````
 
 Scikit-build-core also strictly validates configuration; if you need to disable
 this, you can:
 
 ```toml
-[tool.cmake]
+[tool.scikit-build]
 strict-config = false
 ```
 
 Scikit-build-core also occasionally has experimental features. This is applied
 to features that do not yet carry the same forward compatibility (using
 minimum-version) guarantee that other scikit-build-core features have. These can
 only be used if you enable them:
 
 ```toml
-[tool.cmake]
+[tool.scikit-build]
 experimental = true
 ```
```

### Comparing `scikit_build_core-0.3.0/docs/getting_started.md` & `scikit_build_core-0.3.1/docs/getting_started.md`

 * *Files 0% similar despite different names*

```diff
@@ -320,15 +320,15 @@
 CMake from searching for both `C` and `CXX` compilers (the default).
 
 You'll need to handle the generation of files by Cython directly at the moment.
 A helper (similar to scikti-build classic) might be added in the future.
 
 ````
 
-````{tab} Cython
+````{tab} Fortran
 
 ```{literalinclude} examples/getting_started/fortran/CMakeLists.txt
 :language: cmake
 ```
 
 Scikit-build requires CMake 3.15, so there's no need to set it lower than 3.15.
```

### Comparing `scikit_build_core-0.3.0/docs/index.md` & `scikit_build_core-0.3.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/docs/api/scikit_build_core.build.rst` & `scikit_build_core-0.3.1/docs/api/scikit_build_core.build.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/docs/api/scikit_build_core.builder.rst` & `scikit_build_core-0.3.1/docs/api/scikit_build_core.builder.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/docs/api/scikit_build_core.file_api.model.rst` & `scikit_build_core-0.3.1/docs/api/scikit_build_core.file_api.model.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/docs/api/scikit_build_core.file_api.rst` & `scikit_build_core-0.3.1/docs/api/scikit_build_core.file_api.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/docs/api/scikit_build_core.metadata.rst` & `scikit_build_core-0.3.1/docs/api/scikit_build_core.metadata.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/docs/api/scikit_build_core.rst` & `scikit_build_core-0.3.1/docs/api/scikit_build_core.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/docs/api/scikit_build_core.settings.rst` & `scikit_build_core-0.3.1/docs/api/scikit_build_core.settings.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/docs/api/scikit_build_core.setuptools.rst` & `scikit_build_core-0.3.1/docs/api/scikit_build_core.setuptools.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/docs/examples/getting_started/abi3/example.c` & `scikit_build_core-0.3.1/docs/examples/getting_started/abi3/example.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/docs/examples/getting_started/c/example.c` & `scikit_build_core-0.3.1/docs/examples/getting_started/c/example.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/docs/examples/getting_started/cython/CMakeLists.txt` & `scikit_build_core-0.3.1/docs/examples/getting_started/cython/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/docs/examples/getting_started/fortran/CMakeLists.txt` & `scikit_build_core-0.3.1/docs/examples/getting_started/fortran/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/docs/examples/getting_started/swig/CMakeLists.txt` & `scikit_build_core-0.3.1/docs/examples/getting_started/swig/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/src/scikit_build_core/_logging.py` & `scikit_build_core-0.3.1/src/scikit_build_core/_logging.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/src/scikit_build_core/_shutil.py` & `scikit_build_core-0.3.1/src/scikit_build_core/_shutil.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/src/scikit_build_core/cmake.py` & `scikit_build_core-0.3.1/src/scikit_build_core/cmake.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/src/scikit_build_core/errors.py` & `scikit_build_core-0.3.1/src/scikit_build_core/errors.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/src/scikit_build_core/program_search.py` & `scikit_build_core-0.3.1/src/scikit_build_core/program_search.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/src/scikit_build_core/_compat/typing.py` & `scikit_build_core-0.3.1/src/scikit_build_core/_compat/typing.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/src/scikit_build_core/_compat/importlib/metadata.py` & `scikit_build_core-0.3.1/src/scikit_build_core/_compat/importlib/metadata.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/src/scikit_build_core/build/__init__.py` & `scikit_build_core-0.3.1/src/scikit_build_core/build/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/src/scikit_build_core/build/_file_processor.py` & `scikit_build_core-0.3.1/src/scikit_build_core/build/_file_processor.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/src/scikit_build_core/build/_init.py` & `scikit_build_core-0.3.1/src/scikit_build_core/build/_init.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/src/scikit_build_core/build/_pathutil.py` & `scikit_build_core-0.3.1/src/scikit_build_core/build/_pathutil.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/src/scikit_build_core/build/_scripts.py` & `scikit_build_core-0.3.1/src/scikit_build_core/build/_scripts.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/src/scikit_build_core/build/_wheelfile.py` & `scikit_build_core-0.3.1/src/scikit_build_core/build/_wheelfile.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/src/scikit_build_core/build/sdist.py` & `scikit_build_core-0.3.1/src/scikit_build_core/build/sdist.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/src/scikit_build_core/build/wheel.py` & `scikit_build_core-0.3.1/src/scikit_build_core/build/wheel.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/src/scikit_build_core/builder/builder.py` & `scikit_build_core-0.3.1/src/scikit_build_core/builder/builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,15 +140,16 @@
 
         # Modern Find Python
         for prefix in ("Python", "Python3"):
             cache_config[f"{prefix}_EXECUTABLE"] = sys.executable
             cache_config[f"{prefix}_ROOT_DIR"] = sys.prefix
             cache_config[f"{prefix}_INCLUDE_DIR"] = python_include_dir
             cache_config[f"{prefix}_FIND_REGISTRY"] = "NEVER"
-            if python_library:
+            # FindPython may break if this is set - only useful on Windows
+            if python_library and sys.platform.startswith("win"):
                 cache_config[f"{prefix}_LIBRARY"] = python_library
 
         if limited_abi:
             cache_config["SKBUILD_SOABI"] = (
                 "" if sys.platform.startswith("win") else "abi3"
             )
         else:
```

### Comparing `scikit_build_core-0.3.0/src/scikit_build_core/builder/generator.py` & `scikit_build_core-0.3.1/src/scikit_build_core/builder/generator.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/src/scikit_build_core/builder/get_requires.py` & `scikit_build_core-0.3.1/src/scikit_build_core/builder/get_requires.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/src/scikit_build_core/builder/macos.py` & `scikit_build_core-0.3.1/src/scikit_build_core/builder/macos.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/src/scikit_build_core/builder/sysconfig.py` & `scikit_build_core-0.3.1/src/scikit_build_core/builder/sysconfig.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/src/scikit_build_core/builder/wheel_tag.py` & `scikit_build_core-0.3.1/src/scikit_build_core/builder/wheel_tag.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/src/scikit_build_core/file_api/_cattrs_converter.py` & `scikit_build_core-0.3.1/src/scikit_build_core/file_api/_cattrs_converter.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/src/scikit_build_core/file_api/query.py` & `scikit_build_core-0.3.1/src/scikit_build_core/file_api/query.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/src/scikit_build_core/file_api/reply.py` & `scikit_build_core-0.3.1/src/scikit_build_core/file_api/reply.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/src/scikit_build_core/file_api/model/codemodel.py` & `scikit_build_core-0.3.1/src/scikit_build_core/file_api/model/codemodel.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/src/scikit_build_core/file_api/model/directory.py` & `scikit_build_core-0.3.1/src/scikit_build_core/file_api/model/directory.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/src/scikit_build_core/file_api/model/index.py` & `scikit_build_core-0.3.1/src/scikit_build_core/file_api/model/index.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/src/scikit_build_core/file_api/model/toolchains.py` & `scikit_build_core-0.3.1/src/scikit_build_core/file_api/model/toolchains.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/src/scikit_build_core/metadata/fancy_pypi_readme.py` & `scikit_build_core-0.3.1/src/scikit_build_core/metadata/fancy_pypi_readme.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/src/scikit_build_core/metadata/setuptools_scm.py` & `scikit_build_core-0.3.1/src/scikit_build_core/metadata/setuptools_scm.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/src/scikit_build_core/resources/_editable_redirect.py` & `scikit_build_core-0.3.1/src/scikit_build_core/resources/_editable_redirect.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/src/scikit_build_core/resources/known_wheels.toml` & `scikit_build_core-0.3.1/src/scikit_build_core/resources/known_wheels.toml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/src/scikit_build_core/resources/find_python/Copyright.txt` & `scikit_build_core-0.3.1/src/scikit_build_core/resources/find_python/Copyright.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/src/scikit_build_core/resources/find_python/FindPackageHandleStandardArgs.cmake` & `scikit_build_core-0.3.1/src/scikit_build_core/resources/find_python/FindPackageHandleStandardArgs.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/src/scikit_build_core/resources/find_python/FindPackageMessage.cmake` & `scikit_build_core-0.3.1/src/scikit_build_core/resources/find_python/FindPackageMessage.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/src/scikit_build_core/resources/find_python/FindPython.cmake` & `scikit_build_core-0.3.1/src/scikit_build_core/resources/find_python/FindPython.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/src/scikit_build_core/resources/find_python/FindPython3.cmake` & `scikit_build_core-0.3.1/src/scikit_build_core/resources/find_python/FindPython3.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/src/scikit_build_core/resources/find_python/FindPython/Support.cmake` & `scikit_build_core-0.3.1/src/scikit_build_core/resources/find_python/FindPython/Support.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/src/scikit_build_core/settings/_load_provider.py` & `scikit_build_core-0.3.1/src/scikit_build_core/settings/_load_provider.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/src/scikit_build_core/settings/metadata.py` & `scikit_build_core-0.3.1/src/scikit_build_core/settings/metadata.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/src/scikit_build_core/settings/skbuild_model.py` & `scikit_build_core-0.3.1/src/scikit_build_core/settings/skbuild_model.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/src/scikit_build_core/settings/skbuild_read_settings.py` & `scikit_build_core-0.3.1/src/scikit_build_core/settings/skbuild_read_settings.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/src/scikit_build_core/settings/sources.py` & `scikit_build_core-0.3.1/src/scikit_build_core/settings/sources.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/src/scikit_build_core/setuptools/build_meta.py` & `scikit_build_core-0.3.1/src/scikit_build_core/setuptools/build_meta.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/src/scikit_build_core/setuptools/extension.py` & `scikit_build_core-0.3.1/src/scikit_build_core/setuptools/extension.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/tests/conftest.py` & `scikit_build_core-0.3.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/tests/test_builder.py` & `scikit_build_core-0.3.1/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/tests/test_cmake_config.py` & `scikit_build_core-0.3.1/tests/test_cmake_config.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/tests/test_dynamic_metadata.py` & `scikit_build_core-0.3.1/tests/test_dynamic_metadata.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/tests/test_fileapi.py` & `scikit_build_core-0.3.1/tests/test_fileapi.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/tests/test_fortran.py` & `scikit_build_core-0.3.1/tests/test_fortran.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/tests/test_generator_default.py` & `scikit_build_core-0.3.1/tests/test_generator_default.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/tests/test_get_requires.py` & `scikit_build_core-0.3.1/tests/test_get_requires.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/tests/test_module_dir.py` & `scikit_build_core-0.3.1/tests/test_module_dir.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/tests/test_name_main.py` & `scikit_build_core-0.3.1/tests/test_name_main.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/tests/test_prepare_metadata.py` & `scikit_build_core-0.3.1/tests/test_prepare_metadata.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/tests/test_process_scripts.py` & `scikit_build_core-0.3.1/tests/test_process_scripts.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/tests/test_program_search.py` & `scikit_build_core-0.3.1/tests/test_program_search.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/tests/test_pyproject_abi3.py` & `scikit_build_core-0.3.1/tests/test_pyproject_abi3.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/tests/test_pyproject_extra_dirs.py` & `scikit_build_core-0.3.1/tests/test_pyproject_extra_dirs.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/tests/test_pyproject_pep517.py` & `scikit_build_core-0.3.1/tests/test_pyproject_pep517.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/tests/test_pyproject_pep518.py` & `scikit_build_core-0.3.1/tests/test_pyproject_pep518.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/tests/test_pyproject_pep660.py` & `scikit_build_core-0.3.1/tests/test_pyproject_pep660.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/tests/test_settings.py` & `scikit_build_core-0.3.1/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/tests/test_setuptools_abi3.py` & `scikit_build_core-0.3.1/tests/test_setuptools_abi3.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/tests/test_setuptools_pep517.py` & `scikit_build_core-0.3.1/tests/test_setuptools_pep517.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/tests/test_setuptools_pep518.py` & `scikit_build_core-0.3.1/tests/test_setuptools_pep518.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/tests/test_simple_pure.py` & `scikit_build_core-0.3.1/tests/test_simple_pure.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/tests/test_simplest_c.py` & `scikit_build_core-0.3.1/tests/test_simplest_c.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/tests/test_skbuild_settings.py` & `scikit_build_core-0.3.1/tests/test_skbuild_settings.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/tests/test_wheelfile_utils.py` & `scikit_build_core-0.3.1/tests/test_wheelfile_utils.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/tests/api/simple_pure/.cmake/api/v1/reply/cache-v2-2dececcab32f1eda138d.json` & `scikit_build_core-0.3.1/tests/api/simple_pure/.cmake/api/v1/reply/cache-v2-2dececcab32f1eda138d.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/tests/api/simple_pure/.cmake/api/v1/reply/cmakeFiles-v1-74870fd87af7f965b597.json` & `scikit_build_core-0.3.1/tests/api/simple_pure/.cmake/api/v1/reply/cmakeFiles-v1-74870fd87af7f965b597.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/tests/api/simple_pure/.cmake/api/v1/reply/codemodel-v2-ea39b5a28cb1a3e0a069.json` & `scikit_build_core-0.3.1/tests/api/simple_pure/.cmake/api/v1/reply/codemodel-v2-ea39b5a28cb1a3e0a069.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/tests/api/simple_pure/.cmake/api/v1/reply/directory-.-5e7a28751b0c9235cbe7.json` & `scikit_build_core-0.3.1/tests/api/simple_pure/.cmake/api/v1/reply/directory-.-5e7a28751b0c9235cbe7.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/tests/api/simple_pure/.cmake/api/v1/reply/index-2022-09-12T15-23-13-0135.json` & `scikit_build_core-0.3.1/tests/api/simple_pure/.cmake/api/v1/reply/index-2022-09-12T15-23-13-0135.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/tests/api/simple_pure/.cmake/api/v1/reply/target-simple_pure-7eb73eb5c359b881e083.json` & `scikit_build_core-0.3.1/tests/api/simple_pure/.cmake/api/v1/reply/target-simple_pure-7eb73eb5c359b881e083.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/tests/api/simple_pure/.cmake/api/v1/reply/toolchains-v1-06b92b86597808b5f980.json` & `scikit_build_core-0.3.1/tests/api/simple_pure/.cmake/api/v1/reply/toolchains-v1-06b92b86597808b5f980.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/tests/packages/abi3_pyproject_ext/abi3_example.c` & `scikit_build_core-0.3.1/tests/packages/abi3_pyproject_ext/abi3_example.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/tests/packages/abi3_setuptools_ext/abi3_example.c` & `scikit_build_core-0.3.1/tests/packages/abi3_setuptools_ext/abi3_example.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/tests/packages/dynamic_metadata/plugin_project.toml` & `scikit_build_core-0.3.1/tests/packages/dynamic_metadata/plugin_project.toml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/tests/packages/dynamic_metadata/src/module.c` & `scikit_build_core-0.3.1/tests/packages/dynamic_metadata/src/module.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/tests/packages/filepath_pure/CMakeLists.txt` & `scikit_build_core-0.3.1/tests/packages/filepath_pure/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/tests/packages/fortran_example/CMakeLists.txt` & `scikit_build_core-0.3.1/tests/packages/fortran_example/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/tests/packages/simple_pyproject_ext/src/main.cpp` & `scikit_build_core-0.3.1/tests/packages/simple_pyproject_ext/src/main.cpp`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/tests/packages/simple_setuptools_ext/src/main.cpp` & `scikit_build_core-0.3.1/tests/packages/simple_setuptools_ext/src/main.cpp`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/tests/packages/simplest_c/CMakeLists.txt` & `scikit_build_core-0.3.1/tests/packages/simplest_c/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/tests/packages/simplest_c/src/module.c` & `scikit_build_core-0.3.1/tests/packages/simplest_c/src/module.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/.gitignore` & `scikit_build_core-0.3.1/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -164,7 +164,9 @@
 .DS_Store
 .DS_Store?
 ._*
 .Spotlight-V100
 .Trashes
 ehthumbs.db
 Thumbs.db
+
+.idea/
```

### Comparing `scikit_build_core-0.3.0/LICENSE` & `scikit_build_core-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/README.md` & `scikit_build_core-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/pyproject.toml` & `scikit_build_core-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.0/PKG-INFO` & `scikit_build_core-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit_build_core
-Version: 0.3.0
+Version: 0.3.1
 Summary: Build backend for CMake based projects
 Project-URL: Homepage, https://github.com/scikit-build/scikit-build-core
 Project-URL: Examples, https://github.com/scikit-build/scikit-build-core/tree/main/tests/packages
 Author-email: Henry Schreiner <henryfs@princeton.edu>
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

