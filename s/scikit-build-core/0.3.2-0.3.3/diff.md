# Comparing `tmp/scikit_build_core-0.3.2.tar.gz` & `tmp/scikit_build_core-0.3.3.tar.gz`

## Comparing `scikit_build_core-0.3.2.tar` & `scikit_build_core-0.3.3.tar`

### file list

```diff
@@ -1,215 +1,216 @@
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/.git_archival.txt
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/.gitattributes
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/.packit.yaml
--rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/.readthedocs.yml
--rw-r--r--   0        0        0     3189 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/noxfile.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/.distro/python-scikit-build-core.rpmlintrc
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/.distro/scikit-build-core.spec
--rw-r--r--   0        0        0     9786 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/.github/codecov.yml
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/.github/dependabot.yml
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/.github/matchers/pylint.json
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/.github/workflows/cd.yml
--rw-r--r--   0        0        0     6765 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0    12842 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/changelog.md
--rw-r--r--   0        0        0     2882 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/cmakelists.md
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/conf.py
--rw-r--r--   0        0        0    12247 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/configuration.md
--rw-r--r--   0        0        0     9062 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/getting_started.md
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/index.md
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/api/scikit_build_core.build.rst
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/api/scikit_build_core.builder.rst
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/api/scikit_build_core.file_api.model.rst
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/api/scikit_build_core.file_api.rst
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/api/scikit_build_core.metadata.rst
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/api/scikit_build_core.resources.find_python.rst
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/api/scikit_build_core.resources.rst
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/api/scikit_build_core.rst
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/api/scikit_build_core.settings.rst
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/api/scikit_build_core.setuptools.rst
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/examples/getting_started/test.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/examples/getting_started/abi3/CMakeLists.txt
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/examples/getting_started/abi3/example.c
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/examples/getting_started/abi3/pyproject.toml
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/examples/getting_started/c/CMakeLists.txt
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/examples/getting_started/c/example.c
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/examples/getting_started/c/pyproject.toml
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/examples/getting_started/cython/CMakeLists.txt
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/examples/getting_started/cython/example.pyx
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/examples/getting_started/cython/pyproject.toml
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/examples/getting_started/fortran/CMakeLists.txt
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/examples/getting_started/fortran/example.f
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/examples/getting_started/fortran/pyproject.toml
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/examples/getting_started/pybind11/CMakeLists.txt
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/examples/getting_started/pybind11/example.cpp
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/examples/getting_started/pybind11/pyproject.toml
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/examples/getting_started/swig/CMakeLists.txt
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/examples/getting_started/swig/example.c
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/examples/getting_started/swig/example.i
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/docs/examples/getting_started/swig/pyproject.toml
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/__init__.py
--rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/_logging.py
--rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/_shutil.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/_version.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/_version.pyi
--rw-r--r--   0        0        0     8505 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/cmake.py
--rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/errors.py
--rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/program_search.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/py.typed
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/_compat/__init__.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/_compat/builtins.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/_compat/tomllib.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/_compat/typing.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/_compat/importlib/__init__.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/_compat/importlib/metadata.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/_compat/importlib/resources.py
--rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/build/__init__.py
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/build/_file_processor.py
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/build/_init.py
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/build/_pathutil.py
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/build/_scripts.py
--rw-r--r--   0        0        0     7458 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/build/_wheelfile.py
--rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/build/sdist.py
--rw-r--r--   0        0        0     9106 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/build/wheel.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/builder/__init__.py
--rw-r--r--   0        0        0     7095 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/builder/builder.py
--rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/builder/generator.py
--rw-r--r--   0        0        0     3547 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/builder/get_requires.py
--rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/builder/macos.py
--rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/builder/sysconfig.py
--rw-r--r--   0        0        0     4290 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/builder/wheel_tag.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/file_api/__init__.py
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/file_api/_cattrs_converter.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/file_api/query.py
--rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/file_api/reply.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/file_api/model/__init__.py
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/file_api/model/cache.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/file_api/model/cmakefiles.py
--rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/file_api/model/codemodel.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/file_api/model/common.py
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/file_api/model/directory.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/file_api/model/index.py
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/file_api/model/toolchains.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/metadata/__init__.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/metadata/fancy_pypi_readme.py
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/metadata/setuptools_scm.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/resources/__init__.py
--rw-r--r--   0        0        0     3773 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/resources/_editable_redirect.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/resources/known_wheels.toml
--rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/resources/find_python/Copyright.txt
--rw-r--r--   0        0        0    23174 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/resources/find_python/FindPackageHandleStandardArgs.cmake
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/resources/find_python/FindPackageMessage.cmake
--rw-r--r--   0        0        0    22536 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/resources/find_python/FindPython.cmake
--rw-r--r--   0        0        0    19036 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/resources/find_python/FindPython3.cmake
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/resources/find_python/__init__.py
--rw-r--r--   0        0        0   198528 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/resources/find_python/FindPython/Support.cmake
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/settings/__init__.py
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/settings/_load_provider.py
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/settings/metadata.py
--rw-r--r--   0        0        0     5256 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/settings/skbuild_model.py
--rw-r--r--   0        0        0     4916 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/settings/skbuild_read_settings.py
--rw-r--r--   0        0        0    16489 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/settings/sources.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/setuptools/__init__.py
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/setuptools/build_meta.py
--rw-r--r--   0        0        0     5503 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/src/scikit_build_core/setuptools/extension.py
--rw-r--r--   0        0        0     8897 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/conftest.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/constraints.txt
--rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/test_builder.py
--rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/test_cmake_config.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/test_custom_modules.py
--rw-r--r--   0        0        0     8426 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/test_dynamic_metadata.py
--rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/test_fileapi.py
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/test_fortran.py
--rw-r--r--   0        0        0    15811 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/test_generator_default.py
--rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/test_get_requires.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/test_logging.py
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/test_module_dir.py
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/test_name_main.py
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/test_prepare_metadata.py
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/test_process_scripts.py
--rw-r--r--   0        0        0     4009 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/test_program_search.py
--rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/test_pyproject_abi3.py
--rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/test_pyproject_extra_dirs.py
--rw-r--r--   0        0        0     6387 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/test_pyproject_pep517.py
--rw-r--r--   0        0        0     4367 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/test_pyproject_pep518.py
--rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/test_pyproject_pep660.py
--rw-r--r--   0        0        0    14021 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/test_settings.py
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/test_setuptools_abi3.py
--rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/test_setuptools_pep517.py
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/test_setuptools_pep518.py
--rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/test_simple_pure.py
--rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/test_simplest_c.py
--rw-r--r--   0        0        0    11951 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/test_skbuild_settings.py
--rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/test_wheelfile_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/api/simple_pure/.cmake/api/v1/query/cache-v2
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/api/simple_pure/.cmake/api/v1/query/cmakeFiles-v1
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/api/simple_pure/.cmake/api/v1/query/codemodel-v2
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/api/simple_pure/.cmake/api/v1/query/toolchains-v1
--rw-r--r--   0        0        0    20671 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/api/simple_pure/.cmake/api/v1/reply/cache-v2-2dececcab32f1eda138d.json
--rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/api/simple_pure/.cmake/api/v1/reply/cmakeFiles-v1-74870fd87af7f965b597.json
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/api/simple_pure/.cmake/api/v1/reply/codemodel-v2-ea39b5a28cb1a3e0a069.json
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/api/simple_pure/.cmake/api/v1/reply/directory-.-5e7a28751b0c9235cbe7.json
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/api/simple_pure/.cmake/api/v1/reply/index-2022-09-12T15-23-13-0135.json
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/api/simple_pure/.cmake/api/v1/reply/target-simple_pure-7eb73eb5c359b881e083.json
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/api/simple_pure/.cmake/api/v1/reply/toolchains-v1-06b92b86597808b5f980.json
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/abi3_pyproject_ext/CMakeLists.txt
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/abi3_pyproject_ext/abi3_example.c
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/abi3_pyproject_ext/pyproject.toml
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/abi3_setuptools_ext/CMakeLists.txt
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/abi3_setuptools_ext/abi3_example.c
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/abi3_setuptools_ext/pyproject.toml
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/abi3_setuptools_ext/setup.cfg
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/abi3_setuptools_ext/setup.py
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/custom_cmake/CMakeLists.txt
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/custom_cmake/pyproject.toml
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/custom_cmake/extern/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/__init__.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_modules/ExampleInclude.cmake
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_modules/__init__.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_prefix/ExamplePkgConfig.cmake
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_prefix/__init__.py
--rwxr-xr-x   0        0        0       80 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/custom_cmake/scripts/script1
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/dynamic_metadata/CMakeLists.txt
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/dynamic_metadata/dual_project.toml
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/dynamic_metadata/faulty_dual_project.toml
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/dynamic_metadata/faulty_project.toml
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/dynamic_metadata/local_pyproject.toml
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/dynamic_metadata/plugin_project.toml
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/dynamic_metadata/pyproject.toml
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/dynamic_metadata/warn_project.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/dynamic_metadata/plugins/local/version/__init__.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/dynamic_metadata/plugins/local/version/nested/__init__.py
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/dynamic_metadata/src/module.c
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/dynamic_metadata/src/dynamic/__init__.py
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/filepath_pure/CMakeLists.txt
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/filepath_pure/pyproject.toml
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/fortran_example/CMakeLists.txt
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/fortran_example/fib1.f
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/fortran_example/pyproject.toml
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/simple_pure/CMakeLists.txt
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/simple_pure/simple_pure.cpp
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/simple_pyproject_ext/CMakeLists.txt
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/simple_pyproject_ext/pyproject.toml
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/simple_pyproject_ext/src/main.cpp
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/simple_setuptools_ext/CMakeLists.txt
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/simple_setuptools_ext/pyproject.toml
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/simple_setuptools_ext/setup.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/simple_setuptools_ext/src/main.cpp
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/simplest_c/.gitignore
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/simplest_c/CMakeLists.txt
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/simplest_c/pyproject.toml
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/simplest_c/src/module.c
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/simplest_c/src/not_a_package/simple.txt
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/simplest_c/src/simplest/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/simplest_c/src/simplest/artifact_ignored.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/simplest_c/src/simplest/data.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/simplest_c/src/simplest/excluded.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/simplest_c/src/simplest/ignored.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/simplest_c/src/simplest/ignored_included.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/tests/packages/simplest_c/src/simplest/sdist_only.txt
--rw-r--r--   0        0        0     2432 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/.gitignore
--rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/LICENSE
--rw-r--r--   0        0        0     9505 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/README.md
--rw-r--r--   0        0        0     7918 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/pyproject.toml
--rw-r--r--   0        0        0    12297 2020-02-02 00:00:00.000000 scikit_build_core-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/.git_archival.txt
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/.gitattributes
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/.packit.yaml
+-rw-r--r--   0        0        0     3313 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/.readthedocs.yml
+-rw-r--r--   0        0        0     3189 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/noxfile.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/.distro/python-scikit-build-core.rpmlintrc
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/.distro/scikit-build-core.spec
+-rw-r--r--   0        0        0     9786 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/.github/codecov.yml
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/.github/dependabot.yml
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/.github/matchers/pylint.json
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     6765 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/.github/workflows/ci.yml
+-rw-r--r--   0        0        0    13231 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/changelog.md
+-rw-r--r--   0        0        0     2882 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/cmakelists.md
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/conf.py
+-rw-r--r--   0        0        0    12247 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/configuration.md
+-rw-r--r--   0        0        0     9062 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/getting_started.md
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/index.md
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/api/scikit_build_core.build.rst
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/api/scikit_build_core.builder.rst
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/api/scikit_build_core.file_api.model.rst
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/api/scikit_build_core.file_api.rst
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/api/scikit_build_core.metadata.rst
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/api/scikit_build_core.resources.find_python.rst
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/api/scikit_build_core.resources.rst
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/api/scikit_build_core.rst
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/api/scikit_build_core.settings.rst
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/api/scikit_build_core.setuptools.rst
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/examples/getting_started/test.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/examples/getting_started/abi3/CMakeLists.txt
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/examples/getting_started/abi3/example.c
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/examples/getting_started/abi3/pyproject.toml
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/examples/getting_started/c/CMakeLists.txt
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/examples/getting_started/c/example.c
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/examples/getting_started/c/pyproject.toml
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/examples/getting_started/cython/CMakeLists.txt
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/examples/getting_started/cython/example.pyx
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/examples/getting_started/cython/pyproject.toml
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/examples/getting_started/fortran/CMakeLists.txt
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/examples/getting_started/fortran/example.f
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/examples/getting_started/fortran/pyproject.toml
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/examples/getting_started/pybind11/CMakeLists.txt
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/examples/getting_started/pybind11/example.cpp
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/examples/getting_started/pybind11/pyproject.toml
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/examples/getting_started/swig/CMakeLists.txt
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/examples/getting_started/swig/example.c
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/examples/getting_started/swig/example.i
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/docs/examples/getting_started/swig/pyproject.toml
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/__init__.py
+-rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/_logging.py
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/_shutil.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/_version.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/_version.pyi
+-rw-r--r--   0        0        0     8594 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/cmake.py
+-rw-r--r--   0        0        0     2093 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/errors.py
+-rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/program_search.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/py.typed
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/_compat/__init__.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/_compat/builtins.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/_compat/tomllib.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/_compat/typing.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/_compat/importlib/__init__.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/_compat/importlib/metadata.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/_compat/importlib/resources.py
+-rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/build/__init__.py
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/build/_file_processor.py
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/build/_init.py
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/build/_pathutil.py
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/build/_scripts.py
+-rw-r--r--   0        0        0     7458 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/build/_wheelfile.py
+-rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/build/sdist.py
+-rw-r--r--   0        0        0     9106 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/build/wheel.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/builder/__init__.py
+-rw-r--r--   0        0        0     7095 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/builder/builder.py
+-rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/builder/generator.py
+-rw-r--r--   0        0        0     3547 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/builder/get_requires.py
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/builder/macos.py
+-rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/builder/sysconfig.py
+-rw-r--r--   0        0        0     4290 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/builder/wheel_tag.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/file_api/__init__.py
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/file_api/_cattrs_converter.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/file_api/query.py
+-rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/file_api/reply.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/file_api/model/__init__.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/file_api/model/cache.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/file_api/model/cmakefiles.py
+-rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/file_api/model/codemodel.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/file_api/model/common.py
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/file_api/model/directory.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/file_api/model/index.py
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/file_api/model/toolchains.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/metadata/__init__.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/metadata/fancy_pypi_readme.py
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/metadata/setuptools_scm.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/resources/__init__.py
+-rw-r--r--   0        0        0     3773 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/resources/_editable_redirect.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/resources/known_wheels.toml
+-rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/resources/find_python/Copyright.txt
+-rw-r--r--   0        0        0    23174 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/resources/find_python/FindPackageHandleStandardArgs.cmake
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/resources/find_python/FindPackageMessage.cmake
+-rw-r--r--   0        0        0    22536 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/resources/find_python/FindPython.cmake
+-rw-r--r--   0        0        0    19036 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/resources/find_python/FindPython3.cmake
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/resources/find_python/__init__.py
+-rw-r--r--   0        0        0   198528 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/resources/find_python/FindPython/Support.cmake
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/settings/__init__.py
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/settings/_load_provider.py
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/settings/metadata.py
+-rw-r--r--   0        0        0     5256 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/settings/skbuild_model.py
+-rw-r--r--   0        0        0     4916 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/settings/skbuild_read_settings.py
+-rw-r--r--   0        0        0    16489 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/settings/sources.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/setuptools/__init__.py
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/setuptools/build_meta.py
+-rw-r--r--   0        0        0     5503 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/src/scikit_build_core/setuptools/extension.py
+-rw-r--r--   0        0        0     8864 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/conftest.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/constraints.txt
+-rw-r--r--   0        0        0     6449 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/test_builder.py
+-rw-r--r--   0        0        0     3524 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/test_cmake_config.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/test_custom_modules.py
+-rw-r--r--   0        0        0     8426 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/test_dynamic_metadata.py
+-rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/test_fileapi.py
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/test_fortran.py
+-rw-r--r--   0        0        0    15811 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/test_generator_default.py
+-rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/test_get_requires.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/test_logging.py
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/test_module_dir.py
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/test_name_main.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/test_prepare_metadata.py
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/test_process_scripts.py
+-rw-r--r--   0        0        0     4009 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/test_program_search.py
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/test_pyproject_abi3.py
+-rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/test_pyproject_extra_dirs.py
+-rw-r--r--   0        0        0     6387 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/test_pyproject_pep517.py
+-rw-r--r--   0        0        0     4367 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/test_pyproject_pep518.py
+-rw-r--r--   0        0        0     2099 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/test_pyproject_pep660.py
+-rw-r--r--   0        0        0    14021 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/test_settings.py
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/test_setuptools_abi3.py
+-rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/test_setuptools_pep517.py
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/test_setuptools_pep518.py
+-rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/test_simple_pure.py
+-rw-r--r--   0        0        0     4034 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/test_simplest_c.py
+-rw-r--r--   0        0        0    11951 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/test_skbuild_settings.py
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/test_wheelfile_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/api/simple_pure/.cmake/api/v1/query/cache-v2
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/api/simple_pure/.cmake/api/v1/query/cmakeFiles-v1
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/api/simple_pure/.cmake/api/v1/query/codemodel-v2
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/api/simple_pure/.cmake/api/v1/query/toolchains-v1
+-rw-r--r--   0        0        0    20671 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/api/simple_pure/.cmake/api/v1/reply/cache-v2-2dececcab32f1eda138d.json
+-rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/api/simple_pure/.cmake/api/v1/reply/cmakeFiles-v1-74870fd87af7f965b597.json
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/api/simple_pure/.cmake/api/v1/reply/codemodel-v2-ea39b5a28cb1a3e0a069.json
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/api/simple_pure/.cmake/api/v1/reply/directory-.-5e7a28751b0c9235cbe7.json
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/api/simple_pure/.cmake/api/v1/reply/index-2022-09-12T15-23-13-0135.json
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/api/simple_pure/.cmake/api/v1/reply/target-simple_pure-7eb73eb5c359b881e083.json
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/api/simple_pure/.cmake/api/v1/reply/toolchains-v1-06b92b86597808b5f980.json
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/abi3_pyproject_ext/CMakeLists.txt
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/abi3_pyproject_ext/abi3_example.c
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/abi3_pyproject_ext/pyproject.toml
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/abi3_setuptools_ext/CMakeLists.txt
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/abi3_setuptools_ext/abi3_example.c
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/abi3_setuptools_ext/pyproject.toml
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/abi3_setuptools_ext/setup.cfg
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/abi3_setuptools_ext/setup.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/custom_cmake/CMakeLists.txt
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/custom_cmake/pyproject.toml
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/custom_cmake/extern/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/__init__.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_modules/ExampleInclude.cmake
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_modules/__init__.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_prefix/ExamplePkgConfig.cmake
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_prefix/__init__.py
+-rwxr-xr-x   0        0        0       80 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/custom_cmake/scripts/script1
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/dynamic_metadata/CMakeLists.txt
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/dynamic_metadata/dual_project.toml
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/dynamic_metadata/faulty_dual_project.toml
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/dynamic_metadata/faulty_project.toml
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/dynamic_metadata/local_pyproject.toml
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/dynamic_metadata/plugin_project.toml
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/dynamic_metadata/pyproject.toml
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/dynamic_metadata/warn_project.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/dynamic_metadata/plugins/local/version/__init__.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/dynamic_metadata/plugins/local/version/nested/__init__.py
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/dynamic_metadata/src/module.c
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/dynamic_metadata/src/dynamic/__init__.py
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/filepath_pure/CMakeLists.txt
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/filepath_pure/pyproject.toml
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/fortran_example/CMakeLists.txt
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/fortran_example/fib1.f
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/fortran_example/pyproject.toml
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/simple_pure/CMakeLists.txt
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/simple_pure/simple_pure.cpp
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/simple_pyproject_ext/CMakeLists.txt
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/simple_pyproject_ext/pyproject.toml
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/simple_pyproject_ext/src/main.cpp
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/simple_setuptools_ext/CMakeLists.txt
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/simple_setuptools_ext/pyproject.toml
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/simple_setuptools_ext/setup.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/simple_setuptools_ext/src/main.cpp
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/simplest_c/.gitignore
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/simplest_c/CMakeLists.txt
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/simplest_c/pyproject.toml
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/simplest_c/src/module.c
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/simplest_c/src/not_a_package/simple.txt
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/simplest_c/src/simplest/__init__.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/simplest_c/src/simplest/_module.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/simplest_c/src/simplest/artifact_ignored.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/simplest_c/src/simplest/data.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/simplest_c/src/simplest/excluded.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/simplest_c/src/simplest/ignored.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/simplest_c/src/simplest/ignored_included.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/tests/packages/simplest_c/src/simplest/sdist_only.txt
+-rw-r--r--   0        0        0     2432 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/.gitignore
+-rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/LICENSE
+-rw-r--r--   0        0        0     9546 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/README.md
+-rw-r--r--   0        0        0     8009 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0    12338 2020-02-02 00:00:00.000000 scikit_build_core-0.3.3/PKG-INFO
```

### Comparing `scikit_build_core-0.3.2/.packit.yaml` & `scikit_build_core-0.3.3/.packit.yaml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/.pre-commit-config.yaml` & `scikit_build_core-0.3.3/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -42,23 +42,23 @@
   - repo: https://github.com/cheshirekow/cmake-format-precommit
     rev: v0.6.13
     hooks:
       - id: cmake-format
         exclude: ^src/scikit_build_core/resources/find_python
 
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: "v3.0.0-alpha.6"
+    rev: "v3.0.0-alpha.9-for-vscode"
     hooks:
       - id: prettier
         types_or: [yaml, markdown, html, css, scss, javascript, json]
         args: [--prose-wrap=always]
         exclude: "^tests"
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.261
+    rev: v0.0.263
     hooks:
       - id: ruff
         args: ["--fix", "--show-fixes"]
 
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: v1.2.0
     hooks:
@@ -73,28 +73,27 @@
         args: []
         additional_dependencies:
           - build
           - cattrs
           - cmake
           - exceptiongroup
           - hatch-fancy-pypi-readme
-          - importlib-metadata
-          - importlib_resources
+          - importlib-metadata>=6.6.0
+          - importlib-resources
           - ninja
           - packaging
           - pyproject_metadata
           - pytest
           - rich
           - setuptools-scm
           - tomli
           - types-setuptools>=67.6.0.5
-          - typing_extensions>=4;python_version<'3.11'
 
   - repo: https://github.com/henryiii/check-sdist
-    rev: "v0.1.1"
+    rev: "v0.1.2"
     hooks:
       - id: check-sdist
         args: [--inject-junk]
         additional_dependencies:
           - hatchling
           - hatch-vcs
```

### Comparing `scikit_build_core-0.3.2/noxfile.py` & `scikit_build_core-0.3.3/noxfile.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/.distro/scikit-build-core.spec` & `scikit_build_core-0.3.3/.distro/scikit-build-core.spec`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/.github/CONTRIBUTING.md` & `scikit_build_core-0.3.3/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/.github/matchers/pylint.json` & `scikit_build_core-0.3.3/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/.github/workflows/cd.yml` & `scikit_build_core-0.3.3/.github/workflows/cd.yml`

 * *Files 10% similar despite different names*

```diff
@@ -8,23 +8,24 @@
 
 env:
   FORCE_COLOR: 3
 
 jobs:
   deploy:
     runs-on: ubuntu-22.04
+    environment: pypi
+    permissions:
+      id-token: write
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
 
       - name: Build package
         run: pipx run build
 
       - uses: actions/upload-artifact@v3
         with:
           path: dist/*
 
       - uses: pypa/gh-action-pypi-publish@v1.8.5
         if: github.event_name == 'release' && github.event.action == 'published'
-        with:
-          password: ${{ secrets.pypi_password }}
```

### Comparing `scikit_build_core-0.3.2/.github/workflows/ci.yml` & `scikit_build_core-0.3.3/.github/workflows/ci.yml`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
       # packages so we remove those first (they then won't be tested)
       - name: Min requirements
         run: |
           pip uninstall -y cmake hatch-fancy-pypi-readme setuptools-scm
           pip install --constraint tests/constraints.txt .[test]
 
       - name: Setup CMake ${{ matrix.cmake-version }}
-        uses: jwlawson/actions-setup-cmake@v1.13
+        uses: jwlawson/actions-setup-cmake@v1.14
         with:
           cmake-version: "${{ matrix.cmake-version }}"
 
       # Skipped on pypy to keep the tests fast
       - name: Test min package
         if: matrix.python-version != 'pypy-3.8'
         run: pytest -ra --showlocals
@@ -230,15 +230,15 @@
         runs-on: [ubuntu-latest, macos-latest, windows-latest]
     runs-on: ${{ matrix.runs-on }}
     timeout-minutes: 15
 
     steps:
       - uses: actions/checkout@v3
 
-      - uses: wntrblm/nox@2022.11.21
+      - uses: wntrblm/nox@2023.04.22
         with:
           python-versions: "3.11"
 
       - name: Build docs
         run: nox -s docs
 
       - name: Check examples
```

### Comparing `scikit_build_core-0.3.2/docs/changelog.md` & `scikit_build_core-0.3.3/docs/changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,24 @@
 # Changelog
 
+## Version 0.3.3
+
+This version improves WebAssembly support (Pyodide) and fixes a reported bug in
+the new editable mode.
+
+Fixes:
+
+- Support prefix dir if toolchain has `CMAKE_FIND_ROOT_PATH_MODE_PACKAGE ONLY`
+  by @henryiii in #303
+- Find wheel files before local files in editable installs by @henryiii in #305
+
+Other:
+
+- Use PyPI's new trusted publisher deployment by @henryiii in #306
+
 ## Version 0.3.2
 
 Some small fixes for edge cases. Several docs improvements, too.
 
 Fixes:
 
 - Suppress Unicode errors in scripts dir and move on by @henryiii in #294
```

### Comparing `scikit_build_core-0.3.2/docs/cmakelists.md` & `scikit_build_core-0.3.3/docs/cmakelists.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/docs/conf.py` & `scikit_build_core-0.3.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/docs/configuration.md` & `scikit_build_core-0.3.3/docs/configuration.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/docs/getting_started.md` & `scikit_build_core-0.3.3/docs/getting_started.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/docs/index.md` & `scikit_build_core-0.3.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/docs/api/scikit_build_core.build.rst` & `scikit_build_core-0.3.3/docs/api/scikit_build_core.build.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/docs/api/scikit_build_core.builder.rst` & `scikit_build_core-0.3.3/docs/api/scikit_build_core.builder.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/docs/api/scikit_build_core.file_api.model.rst` & `scikit_build_core-0.3.3/docs/api/scikit_build_core.file_api.model.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/docs/api/scikit_build_core.file_api.rst` & `scikit_build_core-0.3.3/docs/api/scikit_build_core.file_api.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/docs/api/scikit_build_core.metadata.rst` & `scikit_build_core-0.3.3/docs/api/scikit_build_core.metadata.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/docs/api/scikit_build_core.rst` & `scikit_build_core-0.3.3/docs/api/scikit_build_core.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/docs/api/scikit_build_core.settings.rst` & `scikit_build_core-0.3.3/docs/api/scikit_build_core.settings.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/docs/api/scikit_build_core.setuptools.rst` & `scikit_build_core-0.3.3/docs/api/scikit_build_core.setuptools.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/docs/examples/getting_started/abi3/example.c` & `scikit_build_core-0.3.3/docs/examples/getting_started/abi3/example.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/docs/examples/getting_started/c/example.c` & `scikit_build_core-0.3.3/docs/examples/getting_started/c/example.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/docs/examples/getting_started/cython/CMakeLists.txt` & `scikit_build_core-0.3.3/docs/examples/getting_started/cython/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/docs/examples/getting_started/fortran/CMakeLists.txt` & `scikit_build_core-0.3.3/docs/examples/getting_started/fortran/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/docs/examples/getting_started/swig/CMakeLists.txt` & `scikit_build_core-0.3.3/docs/examples/getting_started/swig/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/src/scikit_build_core/_logging.py` & `scikit_build_core-0.3.3/src/scikit_build_core/_logging.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/src/scikit_build_core/_shutil.py` & `scikit_build_core-0.3.3/src/scikit_build_core/_shutil.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/src/scikit_build_core/cmake.py` & `scikit_build_core-0.3.3/src/scikit_build_core/cmake.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,14 +145,15 @@
             if self.prefix_dirs:
                 prefix_dirs_str = ";".join(map(str, self.prefix_dirs)).replace(
                     "\\", "/"
                 )
                 f.write(
                     f'set(CMAKE_PREFIX_PATH [===[{prefix_dirs_str}]===] CACHE PATH "" FORCE)\n'
                 )
+                f.write('set(CMAKE_FIND_ROOT_PATH_MODE_PACKAGE "BOTH" CACHE PATH "")\n')
 
         contents = self.init_cache_file.read_text(encoding="utf-8").strip()
         logger.debug(
             "{}:\n{}",
             self.init_cache_file,
             textwrap.indent(contents.strip(), "  "),
         )
```

### Comparing `scikit_build_core-0.3.2/src/scikit_build_core/errors.py` & `scikit_build_core-0.3.3/src/scikit_build_core/errors.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/src/scikit_build_core/program_search.py` & `scikit_build_core-0.3.3/src/scikit_build_core/program_search.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/src/scikit_build_core/_compat/typing.py` & `scikit_build_core-0.3.3/src/scikit_build_core/_compat/typing.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/src/scikit_build_core/_compat/importlib/metadata.py` & `scikit_build_core-0.3.3/src/scikit_build_core/_compat/importlib/metadata.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/src/scikit_build_core/build/__init__.py` & `scikit_build_core-0.3.3/src/scikit_build_core/build/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/src/scikit_build_core/build/_file_processor.py` & `scikit_build_core-0.3.3/src/scikit_build_core/build/_file_processor.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/src/scikit_build_core/build/_init.py` & `scikit_build_core-0.3.3/src/scikit_build_core/build/_init.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/src/scikit_build_core/build/_pathutil.py` & `scikit_build_core-0.3.3/src/scikit_build_core/build/_pathutil.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/src/scikit_build_core/build/_scripts.py` & `scikit_build_core-0.3.3/src/scikit_build_core/build/_scripts.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/src/scikit_build_core/build/_wheelfile.py` & `scikit_build_core-0.3.3/src/scikit_build_core/build/_wheelfile.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/src/scikit_build_core/build/sdist.py` & `scikit_build_core-0.3.3/src/scikit_build_core/build/sdist.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/src/scikit_build_core/build/wheel.py` & `scikit_build_core-0.3.3/src/scikit_build_core/build/wheel.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/src/scikit_build_core/builder/builder.py` & `scikit_build_core-0.3.3/src/scikit_build_core/builder/builder.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/src/scikit_build_core/builder/generator.py` & `scikit_build_core-0.3.3/src/scikit_build_core/builder/generator.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/src/scikit_build_core/builder/get_requires.py` & `scikit_build_core-0.3.3/src/scikit_build_core/builder/get_requires.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/src/scikit_build_core/builder/macos.py` & `scikit_build_core-0.3.3/src/scikit_build_core/builder/macos.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/src/scikit_build_core/builder/sysconfig.py` & `scikit_build_core-0.3.3/src/scikit_build_core/builder/sysconfig.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/src/scikit_build_core/builder/wheel_tag.py` & `scikit_build_core-0.3.3/src/scikit_build_core/builder/wheel_tag.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/src/scikit_build_core/file_api/_cattrs_converter.py` & `scikit_build_core-0.3.3/src/scikit_build_core/file_api/_cattrs_converter.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/src/scikit_build_core/file_api/query.py` & `scikit_build_core-0.3.3/src/scikit_build_core/file_api/query.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/src/scikit_build_core/file_api/reply.py` & `scikit_build_core-0.3.3/src/scikit_build_core/file_api/reply.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/src/scikit_build_core/file_api/model/codemodel.py` & `scikit_build_core-0.3.3/src/scikit_build_core/file_api/model/codemodel.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/src/scikit_build_core/file_api/model/directory.py` & `scikit_build_core-0.3.3/src/scikit_build_core/file_api/model/directory.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/src/scikit_build_core/file_api/model/index.py` & `scikit_build_core-0.3.3/src/scikit_build_core/file_api/model/index.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/src/scikit_build_core/file_api/model/toolchains.py` & `scikit_build_core-0.3.3/src/scikit_build_core/file_api/model/toolchains.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/src/scikit_build_core/metadata/fancy_pypi_readme.py` & `scikit_build_core-0.3.3/src/scikit_build_core/metadata/fancy_pypi_readme.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/src/scikit_build_core/metadata/setuptools_scm.py` & `scikit_build_core-0.3.3/src/scikit_build_core/metadata/setuptools_scm.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/src/scikit_build_core/resources/_editable_redirect.py` & `scikit_build_core-0.3.3/src/scikit_build_core/resources/_editable_redirect.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -35,24 +35,24 @@
 
     def find_spec(
         self,
         fullname: str,
         path: object = None,
         target: object = None,
     ) -> importlib.machinery.ModuleSpec | None:
-        if fullname in self.known_source_files:
-            redir = self.known_source_files[fullname]
-            return importlib.util.spec_from_file_location(fullname, redir)
         if fullname in self.known_wheel_files:
             redir = self.known_wheel_files[fullname]
             if self.rebuild_flag:
                 self.rebuild()
             return importlib.util.spec_from_file_location(
                 fullname, os.path.join(DIR, redir)
             )
+        if fullname in self.known_source_files:
+            redir = self.known_source_files[fullname]
+            return importlib.util.spec_from_file_location(fullname, redir)
 
         return None
 
     def rebuild(self) -> None:
         # Don't rebuild if not set to a local path
         if not self.path:
             return
```

### Comparing `scikit_build_core-0.3.2/src/scikit_build_core/resources/known_wheels.toml` & `scikit_build_core-0.3.3/src/scikit_build_core/resources/known_wheels.toml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/src/scikit_build_core/resources/find_python/Copyright.txt` & `scikit_build_core-0.3.3/src/scikit_build_core/resources/find_python/Copyright.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/src/scikit_build_core/resources/find_python/FindPackageHandleStandardArgs.cmake` & `scikit_build_core-0.3.3/src/scikit_build_core/resources/find_python/FindPackageHandleStandardArgs.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/src/scikit_build_core/resources/find_python/FindPackageMessage.cmake` & `scikit_build_core-0.3.3/src/scikit_build_core/resources/find_python/FindPackageMessage.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/src/scikit_build_core/resources/find_python/FindPython.cmake` & `scikit_build_core-0.3.3/src/scikit_build_core/resources/find_python/FindPython.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/src/scikit_build_core/resources/find_python/FindPython3.cmake` & `scikit_build_core-0.3.3/src/scikit_build_core/resources/find_python/FindPython3.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/src/scikit_build_core/resources/find_python/FindPython/Support.cmake` & `scikit_build_core-0.3.3/src/scikit_build_core/resources/find_python/FindPython/Support.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/src/scikit_build_core/settings/_load_provider.py` & `scikit_build_core-0.3.3/src/scikit_build_core/settings/_load_provider.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/src/scikit_build_core/settings/metadata.py` & `scikit_build_core-0.3.3/src/scikit_build_core/settings/metadata.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/src/scikit_build_core/settings/skbuild_model.py` & `scikit_build_core-0.3.3/src/scikit_build_core/settings/skbuild_model.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/src/scikit_build_core/settings/skbuild_read_settings.py` & `scikit_build_core-0.3.3/src/scikit_build_core/settings/skbuild_read_settings.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/src/scikit_build_core/settings/sources.py` & `scikit_build_core-0.3.3/src/scikit_build_core/settings/sources.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/src/scikit_build_core/setuptools/build_meta.py` & `scikit_build_core-0.3.3/src/scikit_build_core/setuptools/build_meta.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/src/scikit_build_core/setuptools/extension.py` & `scikit_build_core-0.3.3/src/scikit_build_core/setuptools/extension.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/tests/conftest.py` & `scikit_build_core-0.3.3/tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -291,14 +291,14 @@
         "setuptools",
         "virtualenv",
         "wheel",
     ]
     valid = []
     for package in interesting_packages:
         with contextlib.suppress(ModuleNotFoundError):
-            valid.append(f"{package}=={metadata.version(package)}")  # type: ignore[no-untyped-call]
+            valid.append(f"{package}=={metadata.version(package)}")
     reqs = " ".join(valid)
     lines = [
         f"installed packages of interest: {reqs}",
         f"sysconfig platform: {sysconfig.get_platform()}",
     ]
     return "\n".join(lines)
```

### Comparing `scikit_build_core-0.3.2/tests/test_builder.py` & `scikit_build_core-0.3.3/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/tests/test_cmake_config.py` & `scikit_build_core-0.3.3/tests/test_cmake_config.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/tests/test_dynamic_metadata.py` & `scikit_build_core-0.3.3/tests/test_dynamic_metadata.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/tests/test_fileapi.py` & `scikit_build_core-0.3.3/tests/test_fileapi.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/tests/test_fortran.py` & `scikit_build_core-0.3.3/tests/test_fortran.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/tests/test_generator_default.py` & `scikit_build_core-0.3.3/tests/test_generator_default.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/tests/test_get_requires.py` & `scikit_build_core-0.3.3/tests/test_get_requires.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/tests/test_module_dir.py` & `scikit_build_core-0.3.3/tests/test_module_dir.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/tests/test_name_main.py` & `scikit_build_core-0.3.3/tests/test_name_main.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/tests/test_prepare_metadata.py` & `scikit_build_core-0.3.3/tests/test_prepare_metadata.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/tests/test_process_scripts.py` & `scikit_build_core-0.3.3/tests/test_process_scripts.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/tests/test_program_search.py` & `scikit_build_core-0.3.3/tests/test_program_search.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/tests/test_pyproject_abi3.py` & `scikit_build_core-0.3.3/tests/test_pyproject_abi3.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/tests/test_pyproject_extra_dirs.py` & `scikit_build_core-0.3.3/tests/test_pyproject_extra_dirs.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/tests/test_pyproject_pep517.py` & `scikit_build_core-0.3.3/tests/test_pyproject_pep517.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/tests/test_pyproject_pep518.py` & `scikit_build_core-0.3.3/tests/test_pyproject_pep518.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/tests/test_pyproject_pep660.py` & `scikit_build_core-0.3.3/tests/test_pyproject_pep660.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/tests/test_settings.py` & `scikit_build_core-0.3.3/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/tests/test_setuptools_abi3.py` & `scikit_build_core-0.3.3/tests/test_setuptools_abi3.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/tests/test_setuptools_pep517.py` & `scikit_build_core-0.3.3/tests/test_setuptools_pep517.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/tests/test_setuptools_pep518.py` & `scikit_build_core-0.3.3/tests/test_setuptools_pep518.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/tests/test_simple_pure.py` & `scikit_build_core-0.3.3/tests/test_simple_pure.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/tests/test_simplest_c.py` & `scikit_build_core-0.3.3/tests/test_simplest_c.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
             f"simplest-0.0.1/{x}"
             for x in (
                 "CMakeLists.txt",
                 "pyproject.toml",
                 ".gitignore",
                 "src/module.c",
                 "src/simplest/__init__.py",
+                "src/simplest/_module.pyi",
                 "src/simplest/data.txt",
                 "src/simplest/sdist_only.txt",
                 "src/not_a_package/simple.txt",
                 "src/simplest/excluded.txt",
                 "PKG-INFO",
             )
         }
@@ -61,15 +62,15 @@
         with wheel.open("rb") as f:
             p = zipfile.Path(f)
             file_names = {x.name for x in p.iterdir()}
             simplest_pkg = {x.name for x in p.joinpath("simplest").iterdir()}
 
         filtered_pkg = {x for x in simplest_pkg if not x.startswith("_module")}
 
-        assert len(filtered_pkg) == len(simplest_pkg) - 1
+        assert len(filtered_pkg) == len(simplest_pkg) - 2
         assert {"simplest-0.0.1.dist-info", "simplest"} == file_names
         assert {
             "__init__.py",
             "data.txt",
             "excluded.txt",
             "generated.txt",
             "sdist_only.txt",
@@ -110,15 +111,15 @@
             p = zipfile.Path(f)
             file_names = {x.name for x in p.iterdir()}
             simplest_pkg = {x.name for x in p.joinpath("simplest").iterdir()}
             not_a_pkg = {x.name for x in p.joinpath("not_a_package").iterdir()}
 
         filtered_pkg = {x for x in simplest_pkg if not x.startswith("_module")}
 
-        assert len(filtered_pkg) == len(simplest_pkg) - 1
+        assert len(filtered_pkg) == len(simplest_pkg) - 2
         assert {"simplest-0.0.1.dist-info", "simplest", "not_a_package"} == file_names
         assert {
             "__init__.py",
             "data.txt",
             "ignored_included.txt",
             "generated.txt",
             "sdist_only.txt",
```

### Comparing `scikit_build_core-0.3.2/tests/test_skbuild_settings.py` & `scikit_build_core-0.3.3/tests/test_skbuild_settings.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/tests/test_wheelfile_utils.py` & `scikit_build_core-0.3.3/tests/test_wheelfile_utils.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/tests/api/simple_pure/.cmake/api/v1/reply/cache-v2-2dececcab32f1eda138d.json` & `scikit_build_core-0.3.3/tests/api/simple_pure/.cmake/api/v1/reply/cache-v2-2dececcab32f1eda138d.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/tests/api/simple_pure/.cmake/api/v1/reply/cmakeFiles-v1-74870fd87af7f965b597.json` & `scikit_build_core-0.3.3/tests/api/simple_pure/.cmake/api/v1/reply/cmakeFiles-v1-74870fd87af7f965b597.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/tests/api/simple_pure/.cmake/api/v1/reply/codemodel-v2-ea39b5a28cb1a3e0a069.json` & `scikit_build_core-0.3.3/tests/api/simple_pure/.cmake/api/v1/reply/codemodel-v2-ea39b5a28cb1a3e0a069.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/tests/api/simple_pure/.cmake/api/v1/reply/directory-.-5e7a28751b0c9235cbe7.json` & `scikit_build_core-0.3.3/tests/api/simple_pure/.cmake/api/v1/reply/directory-.-5e7a28751b0c9235cbe7.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/tests/api/simple_pure/.cmake/api/v1/reply/index-2022-09-12T15-23-13-0135.json` & `scikit_build_core-0.3.3/tests/api/simple_pure/.cmake/api/v1/reply/index-2022-09-12T15-23-13-0135.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/tests/api/simple_pure/.cmake/api/v1/reply/target-simple_pure-7eb73eb5c359b881e083.json` & `scikit_build_core-0.3.3/tests/api/simple_pure/.cmake/api/v1/reply/target-simple_pure-7eb73eb5c359b881e083.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/tests/api/simple_pure/.cmake/api/v1/reply/toolchains-v1-06b92b86597808b5f980.json` & `scikit_build_core-0.3.3/tests/api/simple_pure/.cmake/api/v1/reply/toolchains-v1-06b92b86597808b5f980.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/tests/packages/abi3_pyproject_ext/abi3_example.c` & `scikit_build_core-0.3.3/tests/packages/abi3_pyproject_ext/abi3_example.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/tests/packages/abi3_setuptools_ext/abi3_example.c` & `scikit_build_core-0.3.3/tests/packages/abi3_setuptools_ext/abi3_example.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/tests/packages/dynamic_metadata/plugin_project.toml` & `scikit_build_core-0.3.3/tests/packages/dynamic_metadata/plugin_project.toml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/tests/packages/dynamic_metadata/src/module.c` & `scikit_build_core-0.3.3/tests/packages/dynamic_metadata/src/module.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/tests/packages/filepath_pure/CMakeLists.txt` & `scikit_build_core-0.3.3/tests/packages/filepath_pure/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/tests/packages/fortran_example/CMakeLists.txt` & `scikit_build_core-0.3.3/tests/packages/fortran_example/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/tests/packages/simple_pyproject_ext/src/main.cpp` & `scikit_build_core-0.3.3/tests/packages/simple_pyproject_ext/src/main.cpp`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/tests/packages/simple_setuptools_ext/src/main.cpp` & `scikit_build_core-0.3.3/tests/packages/simple_setuptools_ext/src/main.cpp`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/tests/packages/simplest_c/CMakeLists.txt` & `scikit_build_core-0.3.3/tests/packages/simplest_c/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/tests/packages/simplest_c/src/module.c` & `scikit_build_core-0.3.3/tests/packages/simplest_c/src/module.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/.gitignore` & `scikit_build_core-0.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/LICENSE` & `scikit_build_core-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.3.2/README.md` & `scikit_build_core-0.3.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -18,30 +18,31 @@
 <!-- SPHINX-START -->
 
 Features over classic Scikit-build:
 
 - Better warnings, errors, and logging
 - No warning about unused variables
 - Automatically adds Ninja and/or CMake only as required
-- No dependency on setuptools, distutils, or wheel.
-- Powerful config system, including config options support.
+- No dependency on setuptools, distutils, or wheel
+- Powerful config system, including config options support
 - Automatic inclusion of site-packages in `CMAKE_PREFIX_PATH`
 - FindPython is backported if running on CMake < 3.26.1 (configurable), supports
-  PyPY SOABI & Limited API / Stable ABI.
+  PyPY SOABI & Limited API / Stable ABI
 - Limited API / Stable ABI and pythonless tags supported via config option
 - No slow generator search, ninja/make or MSVC used by default, respects
   `CMAKE_GENERATOR`
 - SDists are reproducible by default (UNIX, Python 3.9+)
 - Support for caching between builds (opt-in by setting `build-dir`)
 - Support for writing out to extra wheel folders (scripts, headers, data)
 - Dedicated entrypoints for module and prefix directories
 - Several integrated dynamic metadata plugins (proposing standardized support
   soon)
 - Experimental editable mode support, with optional experimental auto rebuilds
-  on import.
+  on import
+- Supports WebAssembly (Emscripten/Pyodide).
 
 The following limitations are present compared to classic scikit-build:
 
 - The minimum supported CMake is 3.15
 - The minimum supported Python is 3.7
 
 Some known missing features that will be developed soon:
```

### Comparing `scikit_build_core-0.3.2/pyproject.toml` & `scikit_build_core-0.3.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -198,15 +198,16 @@
     "UP",          # pyupgrade
     "YTT",         # flake8-2020
 ]
 extend-ignore = [
     "PLR",     # Design rules for pylint
     "PLE1205", # Format check doesn't work with our custom logger
     "E501",    # Line too long
-    "PT004",
+    "PT004",   # Incorrect, just usefixtures instead.
+    "RUF009",  # Too easy to get a false positive
 ]
 target-version = "py37"
 typing-modules = ["scikit_build_core._compat.typing"]
 src = ["src"]
 unfixable = ["T20", "F841"]
 exclude = []
```

### Comparing `scikit_build_core-0.3.2/PKG-INFO` & `scikit_build_core-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit_build_core
-Version: 0.3.2
+Version: 0.3.3
 Summary: Build backend for CMake based projects
 Project-URL: Homepage, https://github.com/scikit-build/scikit-build-core
 Project-URL: Examples, https://github.com/scikit-build/scikit-build-core/tree/main/tests/packages
 Author-email: Henry Schreiner <henryfs@princeton.edu>
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -81,30 +81,31 @@
 <!-- SPHINX-START -->
 
 Features over classic Scikit-build:
 
 - Better warnings, errors, and logging
 - No warning about unused variables
 - Automatically adds Ninja and/or CMake only as required
-- No dependency on setuptools, distutils, or wheel.
-- Powerful config system, including config options support.
+- No dependency on setuptools, distutils, or wheel
+- Powerful config system, including config options support
 - Automatic inclusion of site-packages in `CMAKE_PREFIX_PATH`
 - FindPython is backported if running on CMake < 3.26.1 (configurable), supports
-  PyPY SOABI & Limited API / Stable ABI.
+  PyPY SOABI & Limited API / Stable ABI
 - Limited API / Stable ABI and pythonless tags supported via config option
 - No slow generator search, ninja/make or MSVC used by default, respects
   `CMAKE_GENERATOR`
 - SDists are reproducible by default (UNIX, Python 3.9+)
 - Support for caching between builds (opt-in by setting `build-dir`)
 - Support for writing out to extra wheel folders (scripts, headers, data)
 - Dedicated entrypoints for module and prefix directories
 - Several integrated dynamic metadata plugins (proposing standardized support
   soon)
 - Experimental editable mode support, with optional experimental auto rebuilds
-  on import.
+  on import
+- Supports WebAssembly (Emscripten/Pyodide).
 
 The following limitations are present compared to classic scikit-build:
 
 - The minimum supported CMake is 3.15
 - The minimum supported Python is 3.7
 
 Some known missing features that will be developed soon:
```

