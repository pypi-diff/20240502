# Comparing `tmp/pythonmonkey-0.4.0.tar.gz` & `tmp/pythonmonkey-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythonmonkey-0.4.0.tar", max compression
+gzip compressed data, was "pythonmonkey-0.6.0.tar", max compression
```

## Comparing `pythonmonkey-0.4.0.tar` & `pythonmonkey-0.6.0.tar`

### file list

```diff
@@ -1,198 +1,192 @@
--rw-r--r--   0        0        0     3761 2024-04-04 20:46:11.196825 pythonmonkey-0.4.0/CMakeLists.txt
--rw-r--r--   0        0        0    21412 2024-04-04 20:45:48.572215 pythonmonkey-0.4.0/LICENSE
--rw-r--r--   0        0        0    20130 2024-04-04 20:45:48.572215 pythonmonkey-0.4.0/README.md
--rw-r--r--   0        0        0     2162 2024-04-04 20:45:48.572215 pythonmonkey-0.4.0/build.py
--rw-r--r--   0        0        0      921 2024-04-04 20:45:48.572215 pythonmonkey-0.4.0/cmake/docs/CMakeLists.txt
--rw-r--r--   0        0        0     2082 2024-04-04 20:45:48.572215 pythonmonkey-0.4.0/cmake/docs/Doxyfile.in
--rw-r--r--   0        0        0    82882 2024-04-04 20:45:48.572215 pythonmonkey-0.4.0/cmake/docs/PythonMonkey-icon.png
--rw-r--r--   0        0        0     4286 2024-04-04 20:45:48.572215 pythonmonkey-0.4.0/cmake/docs/favicon.ico
--rw-r--r--   0        0        0     5940 2024-04-04 20:45:48.572215 pythonmonkey-0.4.0/cmake/docs/header.html
--rw-r--r--   0        0        0      957 2024-04-04 20:45:48.572215 pythonmonkey-0.4.0/cmake/externals/autopep8/CMakeLists.txt
--rw-r--r--   0        0        0     1498 2024-04-04 20:45:48.572215 pythonmonkey-0.4.0/cmake/externals/uncrustify/CMakeLists.txt
--rw-r--r--   0        0        0     3571 2024-04-04 20:45:48.572215 pythonmonkey-0.4.0/cmake/format/CMakeLists.txt
--rw-r--r--   0        0        0     4714 2024-04-04 20:45:48.572215 pythonmonkey-0.4.0/cmake/format/uncrustify.cfg
--rw-r--r--   0        0        0     4971 2024-04-04 20:45:48.572215 pythonmonkey-0.4.0/cmake/modules/FindSpiderMonkey.cmake
--rw-r--r--   0        0        0      646 2024-04-04 20:45:48.572215 pythonmonkey-0.4.0/include/BoolType.hh
--rw-r--r--   0        0        0     2334 2024-04-04 20:45:48.572215 pythonmonkey-0.4.0/include/BufferType.hh
--rw-r--r--   0        0        0      954 2024-04-04 20:45:48.572215 pythonmonkey-0.4.0/include/DateType.hh
--rw-r--r--   0        0        0      909 2024-04-04 20:45:48.572215 pythonmonkey-0.4.0/include/DictType.hh
--rw-r--r--   0        0        0     1280 2024-04-04 20:45:48.572215 pythonmonkey-0.4.0/include/ExceptionType.hh
--rw-r--r--   0        0        0      682 2024-04-04 20:45:48.572215 pythonmonkey-0.4.0/include/FloatType.hh
--rw-r--r--   0        0        0      716 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/include/FuncType.hh
--rw-r--r--   0        0        0     1074 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/include/IntType.hh
--rw-r--r--   0        0        0     2637 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/include/JSArrayIterProxy.hh
--rw-r--r--   0        0        0    13420 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/include/JSArrayProxy.hh
--rw-r--r--   0        0        0     2151 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/include/JSFunctionProxy.hh
--rw-r--r--   0        0        0     2278 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/include/JSMethodProxy.hh
--rw-r--r--   0        0        0     3699 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/include/JSObjectItemsProxy.hh
--rw-r--r--   0        0        0     2751 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/include/JSObjectIterProxy.hh
--rw-r--r--   0        0        0     5776 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/include/JSObjectKeysProxy.hh
--rw-r--r--   0        0        0    11952 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/include/JSObjectProxy.hh
--rw-r--r--   0        0        0     4123 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/include/JSObjectValuesProxy.hh
--rw-r--r--   0        0        0      819 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/include/JSStringProxy.hh
--rw-r--r--   0        0        0     4364 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/include/JobQueue.hh
--rw-r--r--   0        0        0      691 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/include/ListType.hh
--rw-r--r--   0        0        0      509 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/include/NoneType.hh
--rw-r--r--   0        0        0      603 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/include/NullType.hh
--rw-r--r--   0        0        0     2004 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/include/PromiseType.hh
--rw-r--r--   0        0        0     1589 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/include/PyBaseProxyHandler.hh
--rw-r--r--   0        0        0     4538 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/include/PyDictProxyHandler.hh
--rw-r--r--   0        0        0     9870 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/include/PyEventLoop.hh
--rw-r--r--   0        0        0     1734 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/include/PyListProxyHandler.hh
--rw-r--r--   0        0        0     7243 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/include/PyObjectProxyHandler.hh
--rw-r--r--   0        0        0      658 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/include/PyType.hh
--rw-r--r--   0        0        0     1739 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/include/StrType.hh
--rw-r--r--   0        0        0      552 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/include/TupleType.hh
--rw-r--r--   0        0        0      538 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/include/TypeEnum.hh
--rw-r--r--   0        0        0      590 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/include/internalBinding.hh
--rw-r--r--   0        0        0     1855 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/include/jsTypeFactory.hh
--rw-r--r--   0        0        0     2836 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/include/modules/pythonmonkey/pythonmonkey.hh
--rw-r--r--   0        0        0      973 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/include/pyTypeFactory.hh
--rw-r--r--   0        0        0     1061 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/include/setSpiderMonkeyException.hh
--rw-r--r--   0        0        0     1925 2024-04-04 20:46:11.192825 pythonmonkey-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      394 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/python/pythonmonkey/__init__.py
--rw-r--r--   0        0        0     1604 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/python/pythonmonkey/builtin_modules/XMLHttpRequest-internal.d.ts
--rw-r--r--   0        0        0     4564 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/python/pythonmonkey/builtin_modules/XMLHttpRequest-internal.py
--rw-r--r--   0        0        0    22096 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/python/pythonmonkey/builtin_modules/XMLHttpRequest.js
--rw-r--r--   0        0        0      673 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/python/pythonmonkey/builtin_modules/base64.d.ts
--rw-r--r--   0        0        0      684 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/python/pythonmonkey/builtin_modules/base64.py
--rw-r--r--   0        0        0     6081 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/python/pythonmonkey/builtin_modules/console.js
--rw-r--r--   0        0        0     2578 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/python/pythonmonkey/builtin_modules/dom-exception.d.ts
--rw-r--r--   0        0        0      345 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/python/pythonmonkey/builtin_modules/dom-exception.js
--rw-r--r--   0        0        0     5525 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/python/pythonmonkey/builtin_modules/event-target.js
--rw-r--r--   0        0        0     1992 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/python/pythonmonkey/builtin_modules/internal-binding.d.ts
--rw-r--r--   0        0        0      176 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/python/pythonmonkey/builtin_modules/internal-binding.py
--rw-r--r--   0        0        0     4322 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/python/pythonmonkey/builtin_modules/timers.js
--rw-r--r--   0        0        0     4579 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/python/pythonmonkey/builtin_modules/url.d.ts
--rw-r--r--   0        0        0      448 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/python/pythonmonkey/builtin_modules/url.js
--rw-r--r--   0        0        0    28201 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/python/pythonmonkey/builtin_modules/util.js
--rw-r--r--   0        0        0        0 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/python/pythonmonkey/cli/__init__.py
--rwxr-xr-x   0        0        0    13813 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/python/pythonmonkey/cli/pmjs.py
--rw-r--r--   0        0        0     2645 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/python/pythonmonkey/global.d.ts
--rw-r--r--   0        0        0     1636 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/python/pythonmonkey/helpers.py
--rw-r--r--   0        0        0     6332 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/python/pythonmonkey/lib/pmdb.py
--rw-r--r--   0        0        0     1398 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/python/pythonmonkey/lib/pmjs/global-init.js
--rw-r--r--   0        0        0     1896 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/python/pythonmonkey/pythonmonkey.pyi
--rw-r--r--   0        0        0    16224 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/python/pythonmonkey/require.py
--rw-r--r--   0        0        0      422 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/python/pythonmonkey/tsconfig.json
--rwxr-xr-x   0        0        0     3744 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/setup.sh
--rw-r--r--   0        0        0      510 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/src/BoolType.cc
--rw-r--r--   0        0        0     8766 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/src/BufferType.cc
--rw-r--r--   0        0        0     1386 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/src/CMakeLists.txt
--rw-r--r--   0        0        0     2196 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/src/DateType.cc
--rw-r--r--   0        0        0      995 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/src/DictType.cc
--rw-r--r--   0        0        0     8870 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/src/ExceptionType.cc
--rw-r--r--   0        0        0      601 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/src/FloatType.cc
--rw-r--r--   0        0        0      818 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/src/FuncType.cc
--rw-r--r--   0        0        0     8286 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/src/IntType.cc
--rw-r--r--   0        0        0     2183 2024-04-04 20:45:48.576215 pythonmonkey-0.4.0/src/JSArrayIterProxy.cc
--rw-r--r--   0        0        0    40855 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/src/JSArrayProxy.cc
--rw-r--r--   0        0        0     2106 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/src/JSFunctionProxy.cc
--rw-r--r--   0        0        0     2321 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/src/JSMethodProxy.cc
--rw-r--r--   0        0        0     3482 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/src/JSObjectItemsProxy.cc
--rw-r--r--   0        0        0     3219 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/src/JSObjectIterProxy.cc
--rw-r--r--   0        0        0     9782 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/src/JSObjectKeysProxy.cc
--rw-r--r--   0        0        0    22422 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/src/JSObjectProxy.cc
--rw-r--r--   0        0        0     4434 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/src/JSObjectValuesProxy.cc
--rw-r--r--   0        0        0     4392 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/src/JobQueue.cc
--rw-r--r--   0        0        0      873 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/src/ListType.cc
--rw-r--r--   0        0        0      334 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/src/NoneType.cc
--rw-r--r--   0        0        0      422 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/src/NullType.cc
--rw-r--r--   0        0        0     6811 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/src/PromiseType.cc
--rw-r--r--   0        0        0     1825 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/src/PyBaseProxyHandler.cc
--rw-r--r--   0        0        0     3616 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/src/PyDictProxyHandler.cc
--rw-r--r--   0        0        0     8844 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/src/PyEventLoop.cc
--rw-r--r--   0        0        0    61286 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/src/PyListProxyHandler.cc
--rw-r--r--   0        0        0     7258 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/src/PyObjectProxyHandler.cc
--rw-r--r--   0        0        0      538 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/src/PyType.cc
--rw-r--r--   0        0        0     6680 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/src/StrType.cc
--rw-r--r--   0        0        0      348 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/src/TupleType.cc
--rw-r--r--   0        0        0     3236 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/src/internalBinding/timers.cc
--rw-r--r--   0        0        0     4046 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/src/internalBinding/utils.cc
--rw-r--r--   0        0        0     2377 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/src/internalBinding.cc
--rw-r--r--   0        0        0    13780 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/src/jsTypeFactory.cc
--rw-r--r--   0        0        0    26752 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/src/modules/pythonmonkey/pythonmonkey.cc
--rw-r--r--   0        0        0     4654 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/src/pyTypeFactory.cc
--rw-r--r--   0        0        0     4106 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/src/setSpiderMonkeyException.cc
--rw-r--r--   0        0        0      761 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/collide.simple
--rwxr-xr-x   0        0        0     1351 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/commonjs-modules.bash
--rw-r--r--   0        0        0     5738 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/console-methods.simple
--rw-r--r--   0        0        0      602 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/console-smoke.simple
--rwxr-xr-x   0        0        0      935 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/console-stdio.bash
--rw-r--r--   0        0        0     1008 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/console-this.simple
--rw-r--r--   0        0        0      528 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/eval-test.simple
--rw-r--r--   0        0        0      532 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/is-compilable-unit.simple
--rw-r--r--   0        0        0      962 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/js2py/array-change-index.simple
--rw-r--r--   0        0        0      873 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/js2py/arraybuffer.simple
--rw-r--r--   0        0        0      787 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/js2py/bigint.simple
--rw-r--r--   0        0        0      866 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/js2py/boolean.simple
--rw-r--r--   0        0        0     1175 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/js2py/datetime.simple
--rw-r--r--   0        0        0     2003 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/js2py/datetime2.simple
--rw-r--r--   0        0        0     1221 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/js2py/error.simple
--rw-r--r--   0        0        0      810 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/js2py/function-curry.simple
--rw-r--r--   0        0        0      733 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/js2py/higher-order-function.simple
--rw-r--r--   0        0        0      849 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/js2py/object-mutation.simple
--rw-r--r--   0        0        0      547 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/js2py/object.simple
--rw-r--r--   0        0        0      846 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/js2py/promise-await-in-python.simple
--rw-r--r--   0        0        0      718 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/js2py/promise.simple
--rw-r--r--   0        0        0      699 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/js2py/string.simple
--rw-r--r--   0        0        0      519 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/js2py/trivial-function.simple
--rw-r--r--   0        0        0      278 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/load-cjs-module.simple
--rw-r--r--   0        0        0      368 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/load-cjs-python-module.simple
--rw-r--r--   0        0        0      268 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/modules/cjs-module.js
--rw-r--r--   0        0        0       29 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/modules/collide.js
--rw-r--r--   0        0        0       26 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/modules/collide.py
--rw-r--r--   0        0        0       67 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/modules/print-load.js
--rw-r--r--   0        0        0      246 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/modules/python-cjs-module.py
--rw-r--r--   0        0        0      371 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/modules/vm-tools.py
--rw-r--r--   0        0        0      447 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/not-strict-mode.simple
--rwxr-xr-x   0        0        0      750 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/pmjs-eopt.bash
--rwxr-xr-x   0        0        0     1211 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/pmjs-global-arguments.bash
--rwxr-xr-x   0        0        0     1289 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/pmjs-interactive-smoke.bash
--rwxr-xr-x   0        0        0      747 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/pmjs-popt.bash
--rwxr-xr-x   0        0        0     1089 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/pmjs-require-cache.bash
--rwxr-xr-x   0        0        0      753 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/pmjs-ropt.bash
--rw-r--r--   0        0        0     1169 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/program-module.simple
--rwxr-xr-x   0        0        0      635 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/program.js
--rw-r--r--   0        0        0      639 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/py2js/array-change-index.simple
--rw-r--r--   0        0        0      681 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/py2js/arraybuffer.simple
--rw-r--r--   0        0        0     1026 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/py2js/boolean.simple
--rw-r--r--   0        0        0     1515 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/py2js/datetime.simple
--rw-r--r--   0        0        0      810 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/py2js/error.simple
--rw-r--r--   0        0        0      903 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/py2js/function-curry.simple.failing
--rw-r--r--   0        0        0      666 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/py2js/higher-order-function.simple
--rw-r--r--   0        0        0      591 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/py2js/integer.simple
--rw-r--r--   0        0        0     1288 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/py2js/object-methods.simple
--rw-r--r--   0        0        0      532 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/py2js/object.simple
--rw-r--r--   0        0        0      669 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/py2js/promise.simple.failing
--rw-r--r--   0        0        0      538 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/py2js/string.simple
--rw-r--r--   0        0        0      471 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/py2js/trivial-function.simple
--rw-r--r--   0        0        0     1706 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/quint.js
--rwxr-xr-x   0        0        0      796 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/require-module-stack.bash.failing
--rw-r--r--   0        0        0       63 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/resources/eval-test.js
--rw-r--r--   0        0        0      896 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/set-timeout.simple
--rw-r--r--   0        0        0     1672 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/test-atob-btoa.simple
--rw-r--r--   0        0        0      330 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/throw-filename.js
--rwxr-xr-x   0        0        0     1208 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/typeofs-segfaults.simple.failing
--rwxr-xr-x   0        0        0     1667 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/typeofs.simple
--rw-r--r--   0        0        0    32001 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/url-search-params.simple
--rw-r--r--   0        0        0    27371 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/url.simple
--rw-r--r--   0        0        0      432 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/use-strict.simple
--rw-r--r--   0        0        0      795 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/util-module.simple
--rw-r--r--   0        0        0     3063 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/js/xhr.simple
--rw-r--r--   0        0        0      356 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/python/conftest.py
--rw-r--r--   0        0        0    67687 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/python/test_arrays.py
--rw-r--r--   0        0        0     6491 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/python/test_bigints.py
--rw-r--r--   0        0        0    11020 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/python/test_buffer_typed_array.py
--rw-r--r--   0        0        0    16099 2024-04-04 20:45:48.580215 pythonmonkey-0.4.0/tests/python/test_dict_methods.py
--rw-r--r--   0        0        0    10670 2024-04-04 20:45:48.584215 pythonmonkey-0.4.0/tests/python/test_dicts.py
--rw-r--r--   0        0        0    15358 2024-04-04 20:45:48.584215 pythonmonkey-0.4.0/tests/python/test_event_loop.py
--rw-r--r--   0        0        0      460 2024-04-04 20:45:48.584215 pythonmonkey-0.4.0/tests/python/test_finalizationregistry.py
--rw-r--r--   0        0        0     4812 2024-04-04 20:45:48.584215 pythonmonkey-0.4.0/tests/python/test_functions_this.py
--rw-r--r--   0        0        0     1188 2024-04-04 20:45:48.584215 pythonmonkey-0.4.0/tests/python/test_list_array.py
--rw-r--r--   0        0        0    27254 2024-04-04 20:45:48.584215 pythonmonkey-0.4.0/tests/python/test_lists.py
--rw-r--r--   0        0        0     3010 2024-04-04 20:45:48.584215 pythonmonkey-0.4.0/tests/python/test_objects.py
--rw-r--r--   0        0        0    12854 2024-04-04 20:45:48.584215 pythonmonkey-0.4.0/tests/python/test_pythonmonkey_eval.py
--rw-r--r--   0        0        0      576 2024-04-04 20:45:48.584215 pythonmonkey-0.4.0/tests/python/test_reentrance_smoke.py
--rw-r--r--   0        0        0     9095 2024-04-04 20:45:48.584215 pythonmonkey-0.4.0/tests/python/test_strings.py
--rw-r--r--   0        0        0    20720 1970-01-01 00:00:00.000000 pythonmonkey-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     4934 2024-05-02 19:34:22.336245 pythonmonkey-0.6.0/CMakeLists.txt
+-rw-r--r--   0        0        0    21412 2024-05-02 19:24:49.414734 pythonmonkey-0.6.0/LICENSE
+-rw-r--r--   0        0        0    20736 2024-05-02 19:24:49.414734 pythonmonkey-0.6.0/README.md
+-rw-r--r--   0        0        0     2691 2024-05-02 19:24:49.414734 pythonmonkey-0.6.0/build.py
+-rw-r--r--   0        0        0      549 2024-05-02 19:24:49.414734 pythonmonkey-0.6.0/cmake/docs/CMakeLists.txt
+-rw-r--r--   0        0        0     1964 2024-05-02 19:24:49.418734 pythonmonkey-0.6.0/cmake/docs/Doxyfile.in
+-rw-r--r--   0        0        0    82882 2024-05-02 19:24:49.418734 pythonmonkey-0.6.0/cmake/docs/PythonMonkey-icon.png
+-rw-r--r--   0        0        0     4286 2024-05-02 19:24:49.418734 pythonmonkey-0.6.0/cmake/docs/favicon.ico
+-rw-r--r--   0        0        0     5940 2024-05-02 19:24:49.418734 pythonmonkey-0.6.0/cmake/docs/header.html
+-rw-r--r--   0        0        0     4976 2024-05-02 19:24:49.418734 pythonmonkey-0.6.0/cmake/modules/FindSpiderMonkey.cmake
+-rw-r--r--   0        0        0      534 2024-05-02 19:24:49.418734 pythonmonkey-0.6.0/include/BoolType.hh
+-rw-r--r--   0        0        0     2415 2024-05-02 19:24:49.418734 pythonmonkey-0.6.0/include/BufferType.hh
+-rw-r--r--   0        0        0      959 2024-05-02 19:24:49.418734 pythonmonkey-0.6.0/include/DateType.hh
+-rw-r--r--   0        0        0      870 2024-05-02 19:24:49.418734 pythonmonkey-0.6.0/include/DictType.hh
+-rw-r--r--   0        0        0     1253 2024-05-02 19:24:49.418734 pythonmonkey-0.6.0/include/ExceptionType.hh
+-rw-r--r--   0        0        0      544 2024-05-02 19:24:49.418734 pythonmonkey-0.6.0/include/FloatType.hh
+-rw-r--r--   0        0        0      596 2024-05-02 19:24:49.418734 pythonmonkey-0.6.0/include/FuncType.hh
+-rw-r--r--   0        0        0     1100 2024-05-02 19:24:49.418734 pythonmonkey-0.6.0/include/IntType.hh
+-rw-r--r--   0        0        0     2807 2024-05-02 19:24:49.418734 pythonmonkey-0.6.0/include/JSArrayIterProxy.hh
+-rw-r--r--   0        0        0    14001 2024-05-02 19:24:49.418734 pythonmonkey-0.6.0/include/JSArrayProxy.hh
+-rw-r--r--   0        0        0     2151 2024-05-02 19:24:49.418734 pythonmonkey-0.6.0/include/JSFunctionProxy.hh
+-rw-r--r--   0        0        0     2278 2024-05-02 19:24:49.418734 pythonmonkey-0.6.0/include/JSMethodProxy.hh
+-rw-r--r--   0        0        0     3897 2024-05-02 19:24:49.418734 pythonmonkey-0.6.0/include/JSObjectItemsProxy.hh
+-rw-r--r--   0        0        0     2924 2024-05-02 19:24:49.418734 pythonmonkey-0.6.0/include/JSObjectIterProxy.hh
+-rw-r--r--   0        0        0     5878 2024-05-02 19:24:49.418734 pythonmonkey-0.6.0/include/JSObjectKeysProxy.hh
+-rw-r--r--   0        0        0    12675 2024-05-02 19:24:49.418734 pythonmonkey-0.6.0/include/JSObjectProxy.hh
+-rw-r--r--   0        0        0     4324 2024-05-02 19:24:49.418734 pythonmonkey-0.6.0/include/JSObjectValuesProxy.hh
+-rw-r--r--   0        0        0      819 2024-05-02 19:24:49.418734 pythonmonkey-0.6.0/include/JSStringProxy.hh
+-rw-r--r--   0        0        0     4364 2024-05-02 19:24:49.418734 pythonmonkey-0.6.0/include/JobQueue.hh
+-rw-r--r--   0        0        0      611 2024-05-02 19:24:49.418734 pythonmonkey-0.6.0/include/ListType.hh
+-rw-r--r--   0        0        0      480 2024-05-02 19:24:49.418734 pythonmonkey-0.6.0/include/NoneType.hh
+-rw-r--r--   0        0        0      554 2024-05-02 19:24:49.418734 pythonmonkey-0.6.0/include/NullType.hh
+-rw-r--r--   0        0        0     2043 2024-05-02 19:24:49.418734 pythonmonkey-0.6.0/include/PromiseType.hh
+-rw-r--r--   0        0        0     1589 2024-05-02 19:24:49.418734 pythonmonkey-0.6.0/include/PyBaseProxyHandler.hh
+-rw-r--r--   0        0        0     4490 2024-05-02 19:24:49.418734 pythonmonkey-0.6.0/include/PyDictProxyHandler.hh
+-rw-r--r--   0        0        0    10100 2024-05-02 19:24:49.418734 pythonmonkey-0.6.0/include/PyEventLoop.hh
+-rw-r--r--   0        0        0     1002 2024-05-02 19:24:49.418734 pythonmonkey-0.6.0/include/PyIterableProxyHandler.hh
+-rw-r--r--   0        0        0     1707 2024-05-02 19:24:49.418734 pythonmonkey-0.6.0/include/PyListProxyHandler.hh
+-rw-r--r--   0        0        0     7224 2024-05-02 19:24:49.418734 pythonmonkey-0.6.0/include/PyObjectProxyHandler.hh
+-rw-r--r--   0        0        0     1461 2024-05-02 19:24:49.418734 pythonmonkey-0.6.0/include/StrType.hh
+-rw-r--r--   0        0        0      590 2024-05-02 19:24:49.418734 pythonmonkey-0.6.0/include/internalBinding.hh
+-rw-r--r--   0        0        0     1846 2024-05-02 19:24:49.418734 pythonmonkey-0.6.0/include/jsTypeFactory.hh
+-rw-r--r--   0        0        0     2622 2024-05-02 19:24:49.418734 pythonmonkey-0.6.0/include/modules/pythonmonkey/pythonmonkey.hh
+-rw-r--r--   0        0        0      952 2024-05-02 19:24:49.418734 pythonmonkey-0.6.0/include/pyTypeFactory.hh
+-rw-r--r--   0        0        0     1061 2024-05-02 19:24:49.418734 pythonmonkey-0.6.0/include/setSpiderMonkeyException.hh
+-rw-r--r--   0        0        0     2070 2024-05-02 19:34:22.332245 pythonmonkey-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      395 2024-05-02 19:24:49.418734 pythonmonkey-0.6.0/python/pythonmonkey/__init__.py
+-rw-r--r--   0        0        0     1604 2024-05-02 19:24:49.418734 pythonmonkey-0.6.0/python/pythonmonkey/builtin_modules/XMLHttpRequest-internal.d.ts
+-rw-r--r--   0        0        0     4139 2024-05-02 19:24:49.418734 pythonmonkey-0.6.0/python/pythonmonkey/builtin_modules/XMLHttpRequest-internal.py
+-rw-r--r--   0        0        0    22096 2024-05-02 19:24:49.418734 pythonmonkey-0.6.0/python/pythonmonkey/builtin_modules/XMLHttpRequest.js
+-rw-r--r--   0        0        0      673 2024-05-02 19:24:49.418734 pythonmonkey-0.6.0/python/pythonmonkey/builtin_modules/base64.d.ts
+-rw-r--r--   0        0        0      700 2024-05-02 19:24:49.418734 pythonmonkey-0.6.0/python/pythonmonkey/builtin_modules/base64.py
+-rw-r--r--   0        0        0     6081 2024-05-02 19:24:49.418734 pythonmonkey-0.6.0/python/pythonmonkey/builtin_modules/console.js
+-rw-r--r--   0        0        0     2578 2024-05-02 19:24:49.418734 pythonmonkey-0.6.0/python/pythonmonkey/builtin_modules/dom-exception.d.ts
+-rw-r--r--   0        0        0      345 2024-05-02 19:24:49.418734 pythonmonkey-0.6.0/python/pythonmonkey/builtin_modules/dom-exception.js
+-rw-r--r--   0        0        0     5525 2024-05-02 19:24:49.418734 pythonmonkey-0.6.0/python/pythonmonkey/builtin_modules/event-target.js
+-rw-r--r--   0        0        0     2086 2024-05-02 19:24:49.418734 pythonmonkey-0.6.0/python/pythonmonkey/builtin_modules/internal-binding.d.ts
+-rw-r--r--   0        0        0      176 2024-05-02 19:24:49.418734 pythonmonkey-0.6.0/python/pythonmonkey/builtin_modules/internal-binding.py
+-rw-r--r--   0        0        0     6566 2024-05-02 19:24:49.418734 pythonmonkey-0.6.0/python/pythonmonkey/builtin_modules/timers.js
+-rw-r--r--   0        0        0     4579 2024-05-02 19:24:49.418734 pythonmonkey-0.6.0/python/pythonmonkey/builtin_modules/url.d.ts
+-rw-r--r--   0        0        0      448 2024-05-02 19:24:49.418734 pythonmonkey-0.6.0/python/pythonmonkey/builtin_modules/url.js
+-rw-r--r--   0        0        0    28953 2024-05-02 19:24:49.418734 pythonmonkey-0.6.0/python/pythonmonkey/builtin_modules/util.js
+-rw-r--r--   0        0        0        0 2024-05-02 19:24:49.418734 pythonmonkey-0.6.0/python/pythonmonkey/cli/__init__.py
+-rwxr-xr-x   0        0        0    13260 2024-05-02 19:24:49.418734 pythonmonkey-0.6.0/python/pythonmonkey/cli/pmjs.py
+-rw-r--r--   0        0        0     2818 2024-05-02 19:24:49.418734 pythonmonkey-0.6.0/python/pythonmonkey/global.d.ts
+-rw-r--r--   0        0        0     1593 2024-05-02 19:24:49.418734 pythonmonkey-0.6.0/python/pythonmonkey/helpers.py
+-rw-r--r--   0        0        0     6324 2024-05-02 19:24:49.418734 pythonmonkey-0.6.0/python/pythonmonkey/lib/pmdb.py
+-rw-r--r--   0        0        0     1400 2024-05-02 19:24:49.418734 pythonmonkey-0.6.0/python/pythonmonkey/lib/pmjs/global-init.js
+-rw-r--r--   0        0        0     1859 2024-05-02 19:24:49.418734 pythonmonkey-0.6.0/python/pythonmonkey/pythonmonkey.pyi
+-rw-r--r--   0        0        0    16067 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/python/pythonmonkey/require.py
+-rw-r--r--   0        0        0      422 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/python/pythonmonkey/tsconfig.json
+-rwxr-xr-x   0        0        0     4404 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/setup.sh
+-rw-r--r--   0        0        0      371 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/src/BoolType.cc
+-rw-r--r--   0        0        0     8792 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/src/BufferType.cc
+-rw-r--r--   0        0        0     1475 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/src/CMakeLists.txt
+-rw-r--r--   0        0        0     2177 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/src/DateType.cc
+-rw-r--r--   0        0        0      826 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/src/DictType.cc
+-rw-r--r--   0        0        0     8967 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/src/ExceptionType.cc
+-rw-r--r--   0        0        0      438 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/src/FloatType.cc
+-rw-r--r--   0        0        0      654 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/src/FuncType.cc
+-rw-r--r--   0        0        0     8170 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/src/IntType.cc
+-rw-r--r--   0        0        0     2285 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/src/JSArrayIterProxy.cc
+-rw-r--r--   0        0        0    41432 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/src/JSArrayProxy.cc
+-rw-r--r--   0        0        0     2182 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/src/JSFunctionProxy.cc
+-rw-r--r--   0        0        0     2397 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/src/JSMethodProxy.cc
+-rw-r--r--   0        0        0     3621 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/src/JSObjectItemsProxy.cc
+-rw-r--r--   0        0        0     3476 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/src/JSObjectIterProxy.cc
+-rw-r--r--   0        0        0     9918 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/src/JSObjectKeysProxy.cc
+-rw-r--r--   0        0        0    23667 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/src/JSObjectProxy.cc
+-rw-r--r--   0        0        0     4576 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/src/JSObjectValuesProxy.cc
+-rw-r--r--   0        0        0     4449 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/src/JobQueue.cc
+-rw-r--r--   0        0        0      735 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/src/ListType.cc
+-rw-r--r--   0        0        0      367 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/src/NoneType.cc
+-rw-r--r--   0        0        0      488 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/src/NullType.cc
+-rw-r--r--   0        0        0     6723 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/src/PromiseType.cc
+-rw-r--r--   0        0        0     1825 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/src/PyBaseProxyHandler.cc
+-rw-r--r--   0        0        0     3607 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/src/PyDictProxyHandler.cc
+-rw-r--r--   0        0        0    10345 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/src/PyEventLoop.cc
+-rw-r--r--   0        0        0     6580 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/src/PyIterableProxyHandler.cc
+-rw-r--r--   0        0        0    61820 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/src/PyListProxyHandler.cc
+-rw-r--r--   0        0        0     7335 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/src/PyObjectProxyHandler.cc
+-rw-r--r--   0        0        0     6942 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/src/StrType.cc
+-rw-r--r--   0        0        0     3277 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/src/internalBinding/timers.cc
+-rw-r--r--   0        0        0     4045 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/src/internalBinding/utils.cc
+-rw-r--r--   0        0        0     2362 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/src/internalBinding.cc
+-rw-r--r--   0        0        0    14180 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/src/jsTypeFactory.cc
+-rw-r--r--   0        0        0    27577 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/src/modules/pythonmonkey/pythonmonkey.cc
+-rw-r--r--   0        0        0     4751 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/src/pyTypeFactory.cc
+-rw-r--r--   0        0        0     4105 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/src/setSpiderMonkeyException.cc
+-rw-r--r--   0        0        0      765 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/collide.simple
+-rwxr-xr-x   0        0        0     1351 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/commonjs-modules.bash
+-rw-r--r--   0        0        0     5738 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/console-methods.simple
+-rw-r--r--   0        0        0      602 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/console-smoke.simple
+-rwxr-xr-x   0        0        0      935 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/console-stdio.bash
+-rw-r--r--   0        0        0     1008 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/console-this.simple
+-rw-r--r--   0        0        0      540 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/eval-test.simple
+-rw-r--r--   0        0        0      532 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/is-compilable-unit.simple
+-rw-r--r--   0        0        0      963 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/js2py/array-change-index.simple
+-rw-r--r--   0        0        0      873 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/js2py/arraybuffer.simple
+-rw-r--r--   0        0        0      787 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/js2py/bigint.simple
+-rw-r--r--   0        0        0      866 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/js2py/boolean.simple
+-rw-r--r--   0        0        0     1175 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/js2py/datetime.simple
+-rw-r--r--   0        0        0     2003 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/js2py/datetime2.simple
+-rw-r--r--   0        0        0     1234 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/js2py/error.simple
+-rw-r--r--   0        0        0      838 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/js2py/function-curry.simple
+-rw-r--r--   0        0        0      733 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/js2py/higher-order-function.simple
+-rw-r--r--   0        0        0      849 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/js2py/object-mutation.simple
+-rw-r--r--   0        0        0      547 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/js2py/object.simple
+-rw-r--r--   0        0        0      833 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/js2py/promise-await-in-python.simple
+-rw-r--r--   0        0        0      703 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/js2py/promise.simple
+-rw-r--r--   0        0        0      699 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/js2py/string.simple
+-rw-r--r--   0        0        0      519 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/js2py/trivial-function.simple
+-rw-r--r--   0        0        0      278 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/load-cjs-module.simple
+-rw-r--r--   0        0        0      368 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/load-cjs-python-module.simple
+-rw-r--r--   0        0        0      268 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/modules/cjs-module.js
+-rw-r--r--   0        0        0       30 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/modules/collide.js
+-rw-r--r--   0        0        0       28 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/modules/collide.py
+-rw-r--r--   0        0        0       35 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/modules/print-load.js
+-rw-r--r--   0        0        0      247 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/modules/python-cjs-module.py
+-rw-r--r--   0        0        0      371 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/modules/vm-tools.py
+-rw-r--r--   0        0        0      447 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/not-strict-mode.simple
+-rwxr-xr-x   0        0        0      750 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/pmjs-eopt.bash
+-rwxr-xr-x   0        0        0     1211 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/pmjs-global-arguments.bash
+-rwxr-xr-x   0        0        0     1289 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/pmjs-interactive-smoke.bash
+-rwxr-xr-x   0        0        0      747 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/pmjs-popt.bash
+-rwxr-xr-x   0        0        0     1089 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/pmjs-require-cache.bash
+-rwxr-xr-x   0        0        0      753 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/pmjs-ropt.bash
+-rw-r--r--   0        0        0     1171 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/program-module.simple
+-rwxr-xr-x   0        0        0      635 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/program.js
+-rw-r--r--   0        0        0      639 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/py2js/array-change-index.simple
+-rw-r--r--   0        0        0      681 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/py2js/arraybuffer.simple
+-rw-r--r--   0        0        0     1026 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/py2js/boolean.simple
+-rw-r--r--   0        0        0     1518 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/py2js/datetime.simple
+-rw-r--r--   0        0        0      815 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/py2js/error.simple
+-rw-r--r--   0        0        0      903 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/py2js/function-curry.simple.failing
+-rw-r--r--   0        0        0      666 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/py2js/higher-order-function.simple
+-rw-r--r--   0        0        0      591 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/py2js/integer.simple
+-rw-r--r--   0        0        0     1288 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/py2js/object-methods.simple
+-rw-r--r--   0        0        0      532 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/py2js/object.simple
+-rw-r--r--   0        0        0      669 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/py2js/promise.simple.failing
+-rw-r--r--   0        0        0      538 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/py2js/string.simple
+-rw-r--r--   0        0        0      471 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/py2js/trivial-function.simple
+-rw-r--r--   0        0        0     1706 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/quint.js
+-rwxr-xr-x   0        0        0      796 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/require-module-stack.bash.failing
+-rw-r--r--   0        0        0       63 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/resources/eval-test.js
+-rw-r--r--   0        0        0      935 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/set-interval.bash
+-rw-r--r--   0        0        0      900 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/set-timeout.simple
+-rw-r--r--   0        0        0     1680 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/test-atob-btoa.simple
+-rw-r--r--   0        0        0      331 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/throw-filename.js
+-rwxr-xr-x   0        0        0     1208 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/typeofs-segfaults.simple.failing
+-rwxr-xr-x   0        0        0     1680 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/typeofs.simple
+-rw-r--r--   0        0        0    32197 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/url-search-params.simple
+-rw-r--r--   0        0        0    27484 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/url.simple
+-rw-r--r--   0        0        0      432 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/use-strict.simple
+-rw-r--r--   0        0        0      795 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/util-module.simple
+-rw-r--r--   0        0        0     3160 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/js/xhr.simple
+-rw-r--r--   0        0        0      345 2024-05-02 19:24:49.422734 pythonmonkey-0.6.0/tests/python/conftest.py
+-rw-r--r--   0        0        0    67365 2024-05-02 19:24:49.426734 pythonmonkey-0.6.0/tests/python/test_arrays.py
+-rw-r--r--   0        0        0     6291 2024-05-02 19:24:49.426734 pythonmonkey-0.6.0/tests/python/test_bigints.py
+-rw-r--r--   0        0        0    10581 2024-05-02 19:24:49.426734 pythonmonkey-0.6.0/tests/python/test_buffer_typed_array.py
+-rw-r--r--   0        0        0    15507 2024-05-02 19:24:49.426734 pythonmonkey-0.6.0/tests/python/test_dict_methods.py
+-rw-r--r--   0        0        0    10276 2024-05-02 19:24:49.426734 pythonmonkey-0.6.0/tests/python/test_dicts.py
+-rw-r--r--   0        0        0    16379 2024-05-02 19:24:49.426734 pythonmonkey-0.6.0/tests/python/test_event_loop.py
+-rw-r--r--   0        0        0      459 2024-05-02 19:24:49.426734 pythonmonkey-0.6.0/tests/python/test_finalizationregistry.py
+-rw-r--r--   0        0        0     4812 2024-05-02 19:24:49.426734 pythonmonkey-0.6.0/tests/python/test_functions_this.py
+-rw-r--r--   0        0        0     1099 2024-05-02 19:24:49.426734 pythonmonkey-0.6.0/tests/python/test_list_array.py
+-rw-r--r--   0        0        0    25072 2024-05-02 19:24:49.426734 pythonmonkey-0.6.0/tests/python/test_lists.py
+-rw-r--r--   0        0        0     2997 2024-05-02 19:24:49.426734 pythonmonkey-0.6.0/tests/python/test_objects.py
+-rw-r--r--   0        0        0    11995 2024-05-02 19:24:49.426734 pythonmonkey-0.6.0/tests/python/test_pythonmonkey_eval.py
+-rw-r--r--   0        0        0      570 2024-05-02 19:24:49.426734 pythonmonkey-0.6.0/tests/python/test_reentrance_smoke.py
+-rw-r--r--   0        0        0     8158 2024-05-02 19:24:49.426734 pythonmonkey-0.6.0/tests/python/test_strings.py
+-rw-r--r--   0        0        0    21387 1970-01-01 00:00:00.000000 pythonmonkey-0.6.0/PKG-INFO
```

### Comparing `pythonmonkey-0.4.0/LICENSE` & `pythonmonkey-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.4.0/README.md` & `pythonmonkey-0.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,21 @@
     - rust
     - python3.8 or later with header files (python3-dev)
     - spidermonkey 115.1.0 or later
     - npm (nodejs)
     - [Poetry](https://python-poetry.org/docs/#installation)
     - [poetry-dynamic-versioning](https://github.com/mtkennerly/poetry-dynamic-versioning)
 
-2. Run `poetry install`. This command automatically compiles the project and installs the project as well as dependencies into the poetry virtualenv.
+2. Run `poetry install`. This command automatically compiles the project and installs the project as well as dependencies into the poetry virtualenv. If you would like to build the docs, set the `BUILD_DOCS` environment variable, like so: `BUILD_DOCS=1 poetry install`.
+PythonMonkey supports multiple build types, which you can build by setting the `BUILD_TYPE` environment variable, like so: `BUILD_TYPE=Debug poetry install`. The build types are (case-insensitive):
+- `Release`: stripped symbols, maximum optimizations (default)
+- `DRelease`: same as `Release`, except symbols are not stripped
+- `Debug`: minimal optimizations
+- `Profile`: same as `Debug`, except profiling is enabled 
+- `None`: don't compile (useful if you only want to build the docs)
 
 If you are using VSCode, you can just press <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>B</kbd> to [run build task](https://code.visualstudio.com/docs/editor/tasks#_custom-tasks) - We have [the `tasks.json` file configured for you](.vscode/tasks.json).
 
 ## Running tests
 1. Compile the project
 2. Install development dependencies: `poetry install --no-root --only=dev`
 3. From the root directory, run `poetry run pytest ./tests/python`
```

### Comparing `pythonmonkey-0.4.0/cmake/docs/Doxyfile.in` & `pythonmonkey-0.6.0/cmake/docs/Doxyfile.in`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 OUTPUT_DIRECTORY      = "@CMAKE_BINARY_DIR@/docs/"
 INPUT                 = "@CMAKE_SOURCE_DIR@/README.md" \
-                        "@CMAKE_SOURCE_DIR@/docs/" \
                         "@CMAKE_SOURCE_DIR@/src/" \
                         "@CMAKE_SOURCE_DIR@/include/" \
                         "@CMAKE_SOURCE_DIR@/python/pythonmonkey/"
 RECURSIVE             = YES
 
 PROJECT_NAME          = "PythonMonkey"
 PROJECT_NUMBER        = "  v@CMAKE_PROJECT_VERSION@ (dev)"
@@ -16,16 +15,16 @@
 
 EXTRACT_ALL = YES
 GENERATE_LATEX = NO
 GENERATE_XML = YES
 OPTIMIZE_OUTPUT_JAVA = YES
 STRIP_FROM_PATH = "@CMAKE_SOURCE_DIR@"
 
-FILE_PATTERNS = *.cc *.hh *.py *.pyi *.js *.ts *.md
-EXTENSION_MAPPING = pyi=python js=javascript ts=javascript
+FILE_PATTERNS = *.cc *.hh *.py *.pyi *.md
+EXTENSION_MAPPING = pyi=python
 
 # Doxygen Theme
 # https://jothepro.github.io/doxygen-awesome-css/
 GENERATE_TREEVIEW     = YES
 DISABLE_INDEX         = NO
 FULL_SIDEBAR          = NO
 HTML_HEADER           = @CMAKE_CURRENT_SOURCE_DIR@/header.html
@@ -34,14 +33,13 @@
                         @CMAKE_CURRENT_SOURCE_DIR@/doxygen-awesome-css/doxygen-awesome-sidebar-only-darkmode-toggle.css
 HTML_EXTRA_FILES      = @CMAKE_CURRENT_SOURCE_DIR@/favicon.ico \
                         @CMAKE_CURRENT_SOURCE_DIR@/doxygen-awesome-css/doxygen-awesome-darkmode-toggle.js \
                         @CMAKE_CURRENT_SOURCE_DIR@/doxygen-awesome-css/doxygen-awesome-fragment-copy-button.js \
                         @CMAKE_CURRENT_SOURCE_DIR@/doxygen-awesome-css/doxygen-awesome-paragraph-link.js \
                         @CMAKE_CURRENT_SOURCE_DIR@/doxygen-awesome-css/doxygen-awesome-interactive-toc.js
 HTML_COLORSTYLE       = LIGHT
-HTML_TIMESTAMP        = YES
+TIMESTAMP        = YES
 
 # Diagrams with Graphviz
 HAVE_DOT = YES
 DOT_IMAGE_FORMAT = svg
-DOT_TRANSPARENT = YES
 INTERACTIVE_SVG = YES
```

### Comparing `pythonmonkey-0.4.0/cmake/docs/PythonMonkey-icon.png` & `pythonmonkey-0.6.0/cmake/docs/PythonMonkey-icon.png`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.4.0/cmake/docs/favicon.ico` & `pythonmonkey-0.6.0/cmake/docs/favicon.ico`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.4.0/cmake/docs/header.html` & `pythonmonkey-0.6.0/cmake/docs/header.html`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.4.0/cmake/modules/FindSpiderMonkey.cmake` & `pythonmonkey-0.6.0/cmake/modules/FindSpiderMonkey.cmake`

 * *Files 6% similar despite different names*

```diff
@@ -89,16 +89,16 @@
 list(APPEND CMAKE_REQUIRED_DEFINITIONS ${SPIDERMONKEY_DEFINITIONS})
 list(APPEND CMAKE_REQUIRED_LIBRARIES ${SPIDERMONKEY_LIBRARY})
 
 check_cxx_source_compiles(
 	"#include <jsapi.h>
 	int main()
 	{
-    JSRuntime *rt = JS_NewRuntime(8L * 1024L * 1024L);
-		if (rt != NULL)
+    JSContext *cx = JS_NewContext(JS::DefaultHeapMaxBytes);
+		if (cx != NULL)
 		{
 		return 0;
   }
   return 1;
 	}"
 
 	SPIDERMONKEY_BUILDS
```

### Comparing `pythonmonkey-0.4.0/include/BoolType.hh` & `pythonmonkey-0.6.0/include/BoolType.hh`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 /**
  * @file BoolType.hh
- * @author Caleb Aikens (caleb@distributive.network)
+ * @author Caleb Aikens (caleb@distributive.network) and Philippe Laporte (philippe@distributive.network)
  * @brief Struct for representing python bools
  * @date 2022-12-02
  *
- * @copyright Copyright (c) 2022 Distributive Corp.
+ * @copyright Copyright (c) 2022,2024 Distributive Corp.
  *
  */
 
 #ifndef PythonMonkey_BoolType_
 #define PythonMonkey_BoolType_
 
-#include "PyType.hh"
-#include "TypeEnum.hh"
-
 #include <Python.h>
 
 /**
- * @brief This struct represents the 'bool' type in Python, which is represented as a 'long' in C++. It inherits from the PyType struct
+ * @brief This struct represents the 'bool' type in Python, which is represented as a 'long' in C++
  */
-struct BoolType : public PyType {
+struct BoolType {
 public:
-  BoolType(PyObject *object);
-  BoolType(long n);
-  const TYPE returnType = TYPE::BOOL;
-  long getValue() const;
+  static PyObject *getPyObject(long n);
 };
 
 #endif
```

### Comparing `pythonmonkey-0.4.0/include/BufferType.hh` & `pythonmonkey-0.6.0/include/BufferType.hh`

 * *Files 8% similar despite different names*

```diff
@@ -1,49 +1,45 @@
 /**
  * @file BufferType.hh
- * @author Tom Tang (xmader@distributive.network)
+ * @author Tom Tang (xmader@distributive.network) and Philippe Laporte (philippe@distributive.network)
  * @brief Struct for representing ArrayBuffers
  * @date 2023-04-27
  *
- * @copyright Copyright (c) 2023 Distributive Corp.
+ * @copyright Copyright (c) 2023,2024 Distributive Corp.
  *
  */
 
 #ifndef PythonMonkey_BufferType_
 #define PythonMonkey_BufferType_
 
-#include "PyType.hh"
-#include "TypeEnum.hh"
-
 #include <jsapi.h>
 #include <js/ScalarType.h>
 
 #include <Python.h>
 
-struct BufferType : public PyType {
+struct BufferType {
 public:
-  BufferType(PyObject *object);
-
   /**
    * @brief Construct a new BufferType object from a JS TypedArray or ArrayBuffer, as a Python [memoryview](https://docs.python.org/3.9/c-api/memoryview.html) object
    *
    * @param cx - javascript context pointer
    * @param bufObj - JS object to be coerced
+   *
+   * @returns PyObject* pointer to the resulting PyObject
    */
-  BufferType(JSContext *cx, JS::HandleObject bufObj);
-
-  const TYPE returnType = TYPE::BUFFER;
+  static PyObject *getPyObject(JSContext *cx, JS::HandleObject bufObj);
 
   /**
    * @brief Convert a Python object that [provides the buffer interface](https://docs.python.org/3.9/c-api/typeobj.html#buffer-object-structures) to JS TypedArray.
    * The subtype (Uint8Array, Float64Array, ...) is automatically determined by the Python buffer's [format](https://docs.python.org/3.9/c-api/buffer.html#c.Py_buffer.format)
    *
    * @param cx - javascript context pointer
+   * @param pyObject - the object to be converted
    */
-  JSObject *toJsTypedArray(JSContext *cx);
+  static JSObject *toJsTypedArray(JSContext *cx, PyObject *pyObject);
 
   /**
    * @returns Is the given JS object either a TypedArray or an ArrayBuffer?
    */
   static bool isSupportedJsTypes(JSObject *obj);
 
 protected:
```

### Comparing `pythonmonkey-0.4.0/include/DateType.hh` & `pythonmonkey-0.6.0/include/DateType.hh`

 * *Files 19% similar despite different names*

```diff
@@ -1,43 +1,38 @@
 /**
  * @file DateType.hh
- * @author Caleb Aikens (caleb@distributive.network)
+ * @author Caleb Aikens (caleb@distributive.network) and Philippe Laporte (philippe@distributive.network)
  * @brief Struct for representing python dates
  * @date 2022-12-21
  *
- * @copyright Copyright (c) 2022 Distributive Corp.
+ * @copyright Copyright (c) 2022,2024 Distributive Corp.
  *
  */
 
 #ifndef PythonMonkey_DateType_
 #define PythonMonkey_DateType_
 
-#include "PyType.hh"
-#include "TypeEnum.hh"
-
 #include <jsapi.h>
 #include <js/Date.h>
 
 #include <Python.h>
 
 /**
- * @brief This struct represents the 'datetime' type in Python from the datetime module, which is represented as a 'Date' object in JS. It inherits from the PyType struct
+ * @brief This struct represents the 'datetime' type in Python from the datetime module, which is represented as a 'Date' object in JS
  */
-struct DateType : public PyType {
+struct DateType {
 public:
-  DateType(PyObject *object);
   /**
    * @brief Convert a JS Date object to Python datetime
    */
-  DateType(JSContext *cx, JS::HandleObject dateObj);
-
-  const TYPE returnType = TYPE::DATE;
+  static PyObject *getPyObject(JSContext *cx, JS::HandleObject dateObj);
 
   /**
    * @brief Convert a Python datetime object to JS Date
    *
    * @param cx - javascript context pointer
+   * @param pyObject - the python datetime object to be converted
    */
-  JSObject *toJsDate(JSContext *cx);
+  static JSObject *toJsDate(JSContext *cx, PyObject *pyObject);
 };
 
 #endif
```

### Comparing `pythonmonkey-0.4.0/include/DictType.hh` & `pythonmonkey-0.6.0/include/DictType.hh`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,36 @@
 /**
  * @file DictType.hh
- * @author Caleb Aikens (caleb@distributive.network) & Giovanni Tedesco (giovanni@distributive.network)
+ * @author Caleb Aikens (caleb@distributive.network), Giovanni Tedesco (giovanni@distributive.network) and Philippe Laporte (philippe@distributive.network)
  * @brief Struct representing python dictionaries
  * @date 2022-08-10
  *
- * @copyright Copyright (c) 2022 Distributive Corp.
+ * @copyright Copyright (c) 2022,2024 Distributive Corp.
  *
  */
 
 #ifndef PythonMonkey_DictType_
 #define PythonMonkey_DictType_
 
-#include "PyType.hh"
-#include "TypeEnum.hh"
-
 #include <jsapi.h>
 
 #include <Python.h>
 
 /**
- * @brief This struct represents a dictionary in python. It derives from the PyType struct
+ * @brief This struct represents a dictionary in python.
  *
  * @author Giovanni
  */
-struct DictType : public PyType {
+struct DictType {
 public:
-  DictType();
-  DictType(PyObject *object);
-
   /**
    * @brief Construct a new DictType object from a JSObject.
    *
    * @param cx - pointer to the JSContext
    * @param jsObject - pointer to the JSObject to be coerced
+   *
+   * @returns PyObject* pointer to the resulting PyObject
    */
-  DictType(JSContext *cx, JS::Handle<JS::Value> jsObject);
-
-  const TYPE returnType = TYPE::DICT;
+  static PyObject *getPyObject(JSContext *cx, JS::Handle<JS::Value> jsObject);
 };
 
 #endif
```

### Comparing `pythonmonkey-0.4.0/include/ExceptionType.hh` & `pythonmonkey-0.6.0/include/ExceptionType.hh`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,38 @@
 /**
  * @file ExceptionType.hh
  * @author Tom Tang (xmader@distributive.network) and Philippe Laporte (philippe@distributive.network)
  * @brief Struct for representing Python Exception objects from a corresponding JS Error object
  * @date 2023-04-11
  *
- * @copyright Copyright (c) 2023-2024 Distributive Corp.
+ * @copyright Copyright (c) 2023,2024 Distributive Corp.
  *
  */
 
 #ifndef PythonMonkey_ExceptionType_
 #define PythonMonkey_ExceptionType_
 
-#include "PyType.hh"
-#include "TypeEnum.hh"
-
 #include <jsapi.h>
 
 #include <Python.h>
 
 /**
  * @brief This struct represents a Python Exception object from the corresponding JS Error object
  */
-struct ExceptionType : public PyType {
+struct ExceptionType {
 public:
   /**
    * @brief Construct a new SpiderMonkeyError from the JS Error object.
    *
    * @param cx - javascript context pointer
    * @param error - JS Error object to be converted
+   *
+   * @returns PyObject* pointer to the resulting PyObject
    */
-  ExceptionType(JSContext *cx, JS::HandleObject error);
-
-  const TYPE returnType = TYPE::EXCEPTION;
+  static PyObject *getPyObject(JSContext *cx, JS::HandleObject error);
 
   /**
    * @brief Convert a python Exception object to a JS Error object
    *
    * @param cx - javascript context pointer
    * @param exceptionValue - Exception object pointer, cannot be NULL
    * @param traceBack - Exception traceback pointer, can be NULL
```

### Comparing `pythonmonkey-0.4.0/include/FloatType.hh` & `pythonmonkey-0.6.0/include/FloatType.hh`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,24 @@
 /**
  * @file FloatType.hh
- * @author Caleb Aikens (caleb@distributive.network)
+ * @author Caleb Aikens (caleb@distributive.network) and Philippe Laporte (philippe@distributive.network)
  * @brief Struct for representing python floats
  * @date 2022-12-02
  *
- * @copyright Copyright (c) 2022 Distributive Corp.
+ * @copyright Copyright (c) 2022,2024 Distributive Corp.
  *
  */
 
 #ifndef PythonMonkey_FloatType_
 #define PythonMonkey_FloatType_
 
-#include "PyType.hh"
-#include "TypeEnum.hh"
-
 #include <Python.h>
 
 /**
- * @brief This struct represents the 'float' type in Python, which is represented as a 'double' in C++. It inherits from the PyType struct
+ * @brief This struct represents the 'float' type in Python, which is represented as a 'double' in C++
  */
-struct FloatType : public PyType {
+struct FloatType {
 public:
-  FloatType(PyObject *object);
-  FloatType(long n);
-  FloatType(double n);
-  const TYPE returnType = TYPE::FLOAT;
-  double getValue() const;
+  static PyObject *getPyObject(double n);
 };
 
 #endif
```

### Comparing `pythonmonkey-0.4.0/include/FuncType.hh` & `pythonmonkey-0.6.0/include/FuncType.hh`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,26 @@
 /**
  * @file FuncType.hh
- * @author Caleb Aikens (caleb@distributive.network) & Giovanni Tedesco (giovanni@distributive.network)
+ * @author Caleb Aikens (caleb@distributive.network), Giovanni Tedesco (giovanni@distributive.network) and Philippe Laporte (philippe@distributive.network)
  * @brief Struct representing python functions
  * @date 2022-08-08
  *
- * @copyright Copyright (c) 2022 Distributive Corp.
+ * @copyright Copyright (c) 2022,2024 Distributive Corp.
  *
  */
 
 #ifndef PythonMonkey_FuncType_
 #define PythonMonkey_FuncType_
 
-#include "PyType.hh"
-#include "TypeEnum.hh"
-
 #include <jsapi.h>
 
 #include <Python.h>
 
 /**
- * @brief This struct represents the 'function' type in Python. It inherits from the PyType struct
+ * @brief This struct represents the 'function' type in Python
  */
-struct FuncType : public PyType {
+struct FuncType {
 public:
-  FuncType(PyObject *object);
-  FuncType(JSContext *cx, JS::HandleValue fval);
-  const TYPE returnType = TYPE::FUNC;
-  const char *getValue() const;
+  static PyObject *getPyObject(JSContext *cx, JS::HandleValue fval);
 };
 
 #endif
```

### Comparing `pythonmonkey-0.4.0/include/IntType.hh` & `pythonmonkey-0.6.0/include/IntType.hh`

 * *Files 13% similar despite different names*

```diff
@@ -1,47 +1,42 @@
 /**
  * @file IntType.hh
- * @author Caleb Aikens (caleb@distributive.network) & Giovanni Tedesco (giovanni@distributive.network) & Tom Tang (xmader@distributive.network)
+ * @author Caleb Aikens (caleb@distributive.network), Giovanni Tedesco (giovanni@distributive.network), Tom Tang (xmader@distributive.network) and Philippe Laporte (philippe@distributive.network)
  * @brief Struct for representing python ints
  * @date 2023-03-16
  *
- * @copyright Copyright (c) 2023 Distributive Corp.
+ * @copyright Copyright (c) 2023,2024 Distributive Corp.
  *
  */
 
 #ifndef PythonMonkey_IntType_
 #define PythonMonkey_IntType_
 
-#include "PyType.hh"
-#include "TypeEnum.hh"
-
 #include <jsapi.h>
 
 #include <Python.h>
 
 /**
- * @brief This struct represents the 'int' type (arbitrary-precision) in Python. It inherits from the PyType struct
+ * @brief This struct represents the 'int' type (arbitrary-precision) in Python
  */
-struct IntType : public PyType {
+struct IntType {
 public:
-  IntType(PyObject *object);
-  IntType(long n);
-
   /**
-   * @brief Construct a new IntType object from a JS::BigInt.
+   * @brief Construct a new PyObject from a JS::BigInt.
    *
    * @param cx - javascript context pointer
    * @param bigint - JS::BigInt pointer
+   *
+   * @returns PyObject* pointer to the resulting PyObject
    */
-  IntType(JSContext *cx, JS::BigInt *bigint);
-
-  const TYPE returnType = TYPE::INT;
+  static PyObject *getPyObject(JSContext *cx, JS::BigInt *bigint);
 
   /**
-   * @brief Convert the IntType object to a JS::BigInt
+   * @brief Convert an int object to a JS::BigInt
    *
    * @param cx - javascript context pointer
+   * @param pyObject - the int object to be converted
    */
-  JS::BigInt *toJsBigInt(JSContext *cx);
+  static JS::BigInt *toJsBigInt(JSContext *cx, PyObject *pyObject);
 };
 
 #endif
```

### Comparing `pythonmonkey-0.4.0/include/JSArrayIterProxy.hh` & `pythonmonkey-0.6.0/include/JSArrayIterProxy.hh`

 * *Files 6% similar despite different names*

```diff
@@ -47,21 +47,29 @@
    */
   static void JSArrayIterProxy_dealloc(JSArrayIterProxy *self);
 
   /**
    * @brief .tp_traverse method
    *
    * @param self - The JSArrayIterProxy
-   * @param visitproc - The function to be applied on each element of the list
+   * @param visit - The function to be applied on each element of the list
    * @param arg - The argument to the visit function
    * @return 0 on success
    */
   static int JSArrayIterProxy_traverse(JSArrayIterProxy *self, visitproc visit, void *arg);
 
   /**
+   * @brief .tp_clear method
+   *
+   * @param self - The JSArrayIterProxy
+   * @return 0 on success
+   */
+  static int JSArrayIterProxy_clear(JSArrayIterProxy *self);
+
+  /**
    * @brief .tp_iter method
    *
    * @param self - The JSArrayIterProxy
    * @return PyObject* - an interator over the iterator
    */
   static PyObject *JSArrayIterProxy_iter(JSArrayIterProxy *self);
```

### Comparing `pythonmonkey-0.4.0/include/JSArrayProxy.hh` & `pythonmonkey-0.6.0/include/JSArrayProxy.hh`

 * *Files 1% similar despite different names*

```diff
@@ -191,15 +191,15 @@
    */
   static PyObject *JSArrayProxy_insert(JSArrayProxy *self, PyObject *const *args, Py_ssize_t nargs);
 
   /**
    * @brief extend method
    *
    * @param self - The JSArrayProxy
-   * @param value - The value to be appended
+   * @param iterable - The value to be appended
    * @return PyObject* NULL on exception, None otherwise
    */
   static PyObject *JSArrayProxy_extend(JSArrayProxy *self, PyObject *iterable);
 
   /**
    * @brief pop method
    *
@@ -246,19 +246,38 @@
    */
   static PyObject *JSArrayProxy_reverse(JSArrayProxy *self);
 
   /**
    * @brief sort method   sort in place
    *
    * @param self - The JSArrayProxy
-   * @param args - arguments to the sort method
+   * @param args - arguments to the sort method (not used)
    * @param nargs - number of arguments to the sort method
+   * @param kwnames - keyword arguments to the sort method (reverse=True|False, key=keyfunction)
    * @return PyObject* NULL on exception, None otherwise
    */
   static PyObject *JSArrayProxy_sort(JSArrayProxy *self, PyObject *const *args, Py_ssize_t nargs, PyObject *kwnames);
+
+  /**
+   * @brief tp_traverse
+   *
+   * @param self - The JSArrayProxy
+   * @param visit - The function to be applied on each element of the list
+   * @param arg - The argument to the visit function
+   * @return 0 on success
+   */
+  static int JSArrayProxy_traverse(JSArrayProxy *self, visitproc visit, void *arg);
+
+  /**
+   * @brief tp_clear
+   *
+   * @param self - The JSArrayProxy
+   * @return 0 on success
+   */
+  static int JSArrayProxy_clear(JSArrayProxy *self);
 };
 
 
 /**
  * @brief Struct for the methods that define the Mapping protocol
  *
  */
```

### Comparing `pythonmonkey-0.4.0/include/JSFunctionProxy.hh` & `pythonmonkey-0.6.0/include/JSFunctionProxy.hh`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.4.0/include/JSMethodProxy.hh` & `pythonmonkey-0.6.0/include/JSMethodProxy.hh`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.4.0/include/JSObjectItemsProxy.hh` & `pythonmonkey-0.6.0/include/JSObjectItemsProxy.hh`

 * *Files 2% similar despite different names*

```diff
@@ -37,21 +37,29 @@
    */
   static void JSObjectItemsProxy_dealloc(JSObjectItemsProxy *self);
 
   /**
    * @brief .tp_traverse method
    *
    * @param self - The JSObjectItemsProxy
-   * @param visitproc - The function to be applied on each element of the list
+   * @param visit - The function to be applied on each element of the list
    * @param arg - The argument to the visit function
    * @return 0 on success
    */
   static int JSObjectItemsProxy_traverse(JSObjectItemsProxy *self, visitproc visit, void *arg);
 
   /**
+   * @brief .tp_clear method
+   *
+   * @param self - The JSObjectItemsProxy
+   * @return 0 on success
+   */
+  static int JSObjectItemsProxy_clear(JSObjectItemsProxy *self);
+
+  /**
    * @brief Length method (.sq_length), returns the number of key-value pairs in the JSObject, used by the python len() method
    *
    * @param self - The JSObjectProxy
    * @return Py_ssize_t The length of the JSObjectProxy
    */
   static Py_ssize_t JSObjectItemsProxy_length(JSObjectItemsProxy *self);
 
@@ -79,14 +87,15 @@
    */
   static PyObject *JSObjectItemsProxy_iter_reverse(JSObjectItemsProxy *self);
 
   /**
    * @brief mapping method
    *
    * @param self - The JSObjectItemsProxy
+   * @param Py_UNUSED
    * @return PyObject* The resulting new dict
    */
   static PyObject *JSObjectItemsProxy_mapping(PyObject *self, void *Py_UNUSED(ignored));
 };
 
 /**
  * @brief Struct for the methods that define the Sequence protocol
```

### Comparing `pythonmonkey-0.4.0/include/JSObjectIterProxy.hh` & `pythonmonkey-0.6.0/include/JSObjectIterProxy.hh`

 * *Files 2% similar despite different names*

```diff
@@ -53,21 +53,29 @@
    */
   static void JSObjectIterProxy_dealloc(JSObjectIterProxy *self);
 
   /**
    * @brief .tp_traverse method
    *
    * @param self - The JSObjectIterProxy
-   * @param visitproc - The function to be applied on each element of the list
+   * @param visit - The function to be applied on each element of the list
    * @param arg - The argument to the visit function
    * @return 0 on success
    */
   static int JSObjectIterProxy_traverse(JSObjectIterProxy *self, visitproc visit, void *arg);
 
   /**
+   * @brief .tp_clear method
+   *
+   * @param self - The JSObjectIterProxy
+   * @return 0 on success
+   */
+  static int JSObjectIterProxy_clear(JSObjectIterProxy *self);
+
+  /**
    * @brief .tp_iter method
    *
    * @param self - The JSObjectIterProxy
    * @return PyObject* - an interator over the iterator
    */
   static PyObject *JSObjectIterProxy_iter(JSObjectIterProxy *self);
```

### Comparing `pythonmonkey-0.4.0/include/JSObjectKeysProxy.hh` & `pythonmonkey-0.6.0/include/JSObjectKeysProxy.hh`

 * *Files 2% similar despite different names*

```diff
@@ -37,21 +37,29 @@
    */
   static void JSObjectKeysProxy_dealloc(JSObjectKeysProxy *self);
 
   /**
    * @brief .tp_traverse method
    *
    * @param self - The JSObjectKeysProxy
-   * @param visitproc - The function to be applied on each element of the list
+   * @param visit - The function to be applied on each element of the list
    * @param arg - The argument to the visit function
    * @return 0 on success
    */
   static int JSObjectKeysProxy_traverse(JSObjectKeysProxy *self, visitproc visit, void *arg);
 
   /**
+   * @brief .tp_clear method
+   *
+   * @param self - The JSObjectKeysProxy
+   * @return 0 on success
+   */
+  static int JSObjectKeysProxy_clear(JSObjectKeysProxy *self);
+
+  /**
    * @brief Length method (.sq_length), returns the number of key-value pairs in the JSObject, used by the python len() method
    *
    * @param self - The JSObjectProxy
    * @return Py_ssize_t The length of the JSObjectProxy
    */
   static Py_ssize_t JSObjectKeysProxy_length(JSObjectKeysProxy *self);
 
@@ -108,23 +116,23 @@
    */
   static PyObject *JSObjectKeysProxy_isDisjoint(JSObjectKeysProxy *self, PyObject *other);
 
   /**
    * @brief reverse iterator method
    *
    * @param self - The JSObjectKeysProxy
-   * @param other - The other PyObject to be and'd, expected to be dict or JSObjectKeysProxy
    * @return PyObject* The resulting new dict
    */
   static PyObject *JSObjectKeysProxy_iter_reverse(JSObjectKeysProxy *self);
 
   /**
    * @brief mapping method
    *
    * @param self - The JSObjectKeysProxy
+   * @param Py_UNUSED
    * @return PyObject* The resulting new dict
    */
   static PyObject *JSObjectKeysProxy_mapping(PyObject *self, void *Py_UNUSED(ignored));
 };
 
 /**
  * @brief Struct for the methods that define the Sequence protocol
```

### Comparing `pythonmonkey-0.4.0/include/JSObjectProxy.hh` & `pythonmonkey-0.6.0/include/JSObjectProxy.hh`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 #include <jsapi.h>
 
 #include <Python.h>
 
 #include <unordered_map>
 
+
 /**
  * @brief The typedef for the backing store that will be used by JSObjectProxy objects. All it contains is a pointer to the JSObject
  *
  */
 typedef struct {
   PyDictObject dict;
   JS::PersistentRootedObject *jsObject;
@@ -110,14 +111,22 @@
    *
    * @param self - The JSObjectProxy
    * @return PyObject* - iterator object
    */
   static PyObject *JSObjectProxy_iter(JSObjectProxy *self);
 
   /**
+   * @brief Implements next operator function
+   *
+   * @param self - The JSObjectProxy
+   * @return PyObject* - call result
+   */
+  static PyObject *JSObjectProxy_iter_next(JSObjectProxy *self);
+
+  /**
    * @brief Compute a string representation of the JSObjectProxy
    *
    * @param self - The JSObjectProxy
    * @return the string representation (a PyUnicodeObject) on success, NULL on failure
    */
   static PyObject *JSObjectProxy_repr(JSObjectProxy *self);
 
@@ -186,15 +195,15 @@
   static PyObject *JSObjectProxy_copy_method(JSObjectProxy *self);
 
   /**
    * @brief update method    update the dict with another dict or iterable
    *
    * @param self - The JSObjectProxy
    * @param args - arguments to the sort method
-   * @param nargs - number of arguments to the sort method
+   * @param kwds - keyword arguments to the sort method (key-value pairs to be updated in the dict)
    * @return None
    */
   static PyObject *JSObjectProxy_update_method(JSObjectProxy *self, PyObject *args, PyObject *kwds);
 
   /**
    * @brief keys method
    *
@@ -214,14 +223,32 @@
   /**
    * @brief items method
    *
    * @param self - The JSObjectProxy
    * @return PyObject* items view of the dict
    */
   static PyObject *JSObjectProxy_items_method(JSObjectProxy *self);
+
+  /**
+   * @brief tp_traverse
+   *
+   * @param self - The JSObjectProxy
+   * @param visit - The function to be applied on each element of the object
+   * @param arg - The argument to the visit function
+   * @return 0 on success
+   */
+  static int JSObjectProxy_traverse(JSObjectProxy *self, visitproc visit, void *arg);
+
+  /**
+   * @brief tp_clear
+   *
+   * @param self - The JSObjectProxy
+   * @return 0 on success
+   */
+  static int JSObjectProxy_clear(JSObjectProxy *self);
 };
 
 
 // docs for methods, copied from cpython
 PyDoc_STRVAR(getitem__doc__,
   "__getitem__($self, key, /)\n--\n\nReturn self[key].");
```

### Comparing `pythonmonkey-0.4.0/include/JSObjectValuesProxy.hh` & `pythonmonkey-0.6.0/include/JSObjectValuesProxy.hh`

 * *Files 2% similar despite different names*

```diff
@@ -37,21 +37,29 @@
    */
   static void JSObjectValuesProxy_dealloc(JSObjectValuesProxy *self);
 
   /**
    * @brief .tp_traverse method
    *
    * @param self - The JSObjectValuesProxy
-   * @param visitproc - The function to be applied on each element of the list
+   * @param visit - The function to be applied on each element of the list
    * @param arg - The argument to the visit function
    * @return 0 on success
    */
   static int JSObjectValuesProxy_traverse(JSObjectValuesProxy *self, visitproc visit, void *arg);
 
   /**
+   * @brief .tp_clear method
+   *
+   * @param self - The JSObjectValuesProxy
+   * @return 0 on success
+   */
+  static int JSObjectValuesProxy_clear(JSObjectValuesProxy *self);
+
+  /**
    * @brief Length method (.sq_length), returns the number of key-value pairs in the JSObject, used by the python len() method
    *
    * @param self - The JSObjectProxy
    * @return Py_ssize_t The length of the JSObjectProxy
    */
   static Py_ssize_t JSObjectValuesProxy_length(JSObjectValuesProxy *self);
 
@@ -88,14 +96,15 @@
    */
   static PyObject *JSObjectValuesProxy_iter_reverse(JSObjectValuesProxy *self);
 
   /**
    * @brief mapping method
    *
    * @param self - The JSObjectValuesProxy
+   * @param Py_UNUSED
    * @return PyObject* The resulting new dict
    */
   static PyObject *JSObjectValuesProxy_mapping(PyObject *self, void *Py_UNUSED(ignored));
 };
 
 /**
  * @brief Struct for the methods that define the Sequence protocol
```

### Comparing `pythonmonkey-0.4.0/include/JSStringProxy.hh` & `pythonmonkey-0.6.0/include/JSStringProxy.hh`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.4.0/include/JobQueue.hh` & `pythonmonkey-0.6.0/include/JobQueue.hh`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.4.0/include/NullType.hh` & `pythonmonkey-0.6.0/include/NullType.hh`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 /**
  * @file NullType.hh
- * @author Caleb Aikens (caleb@distributive.network)
+ * @author Caleb Aikens (caleb@distributive.network) and Philippe Laporte (philippe@distributive.network)
  * @brief Struct for representing JS null in a python object
  * @date 2023-02-22
  *
- * @copyright Copyright (c) 2023 Distributive Corp.
+ * @copyright Copyright (c) 2023,2024 Distributive Corp.
  *
  */
 
 #ifndef PythonMonkey_NullType_
 #define PythonMonkey_NullType_
 
-#include "PyType.hh"
-#include "TypeEnum.hh"
+#include <Python.h>
 
 /**
- * @brief This struct represents the JS null type in Python using a singleton object on the pythonmonkey module. It inherits from the PyType struct
+ * @brief This struct represents the JS null type in Python using a singleton object on the pythonmonkey module
  */
-struct NullType : public PyType {
+struct NullType {
 public:
-  NullType();
-  const TYPE returnType = TYPE::PYTHONMONKEY_NULL;
+  static PyObject *getPyObject();
 };
 
 #endif
```

### Comparing `pythonmonkey-0.4.0/include/PromiseType.hh` & `pythonmonkey-0.6.0/include/PromiseType.hh`

 * *Files 10% similar despite different names*

```diff
@@ -1,51 +1,47 @@
 /**
  * @file PromiseType.hh
- * @author Tom Tang (xmader@distributive.network)
+ * @author Tom Tang (xmader@distributive.network) and Philippe Laporte (philippe@distributive.network)
  * @brief Struct for representing Promises
  * @date 2023-03-29
  *
- * @copyright Copyright (c) 2023 Distributive Corp.
+ * @copyright Copyright (c) 2023,2024 Distributive Corp.
  *
  */
 
 #ifndef PythonMonkey_PromiseType_
 #define PythonMonkey_PromiseType_
 
-#include "PyType.hh"
-#include "TypeEnum.hh"
-
 #include <jsapi.h>
 #include <js/Promise.h>
 
 #include <Python.h>
 
 /**
- * @brief This struct represents the JS Promise type in Python using our custom pythonmonkey.promise type. It inherits from the PyType struct
+ * @brief This struct represents the JS Promise type in Python using our custom pythonmonkey.promise type
  */
-struct PromiseType : public PyType {
+struct PromiseType {
 public:
-  PromiseType(PyObject *object);
-
   /**
    * @brief Construct a new PromiseType object from a JS::PromiseObject.
    *
    * @param cx - javascript context pointer
    * @param promise - JS::PromiseObject to be coerced
+   *
+   * @returns PyObject* pointer to the resulting PyObject
    */
-  PromiseType(JSContext *cx, JS::HandleObject promise);
-
-  const TYPE returnType = TYPE::PYTHONMONKEY_PROMISE;
+  static PyObject *getPyObject(JSContext *cx, JS::HandleObject promise);
 
   /**
    * @brief Convert a Python [awaitable](https://docs.python.org/3/library/asyncio-task.html#awaitables) object to JS Promise
    *
    * @param cx - javascript context pointer
+   * @param pyObject - the python awaitable to be converted
    */
-  JSObject *toJsPromise(JSContext *cx);
+  static JSObject *toJsPromise(JSContext *cx, PyObject *pyObject);
 };
 
 /**
  * @brief Check if the object can be used in Python await expression.
  * `PyAwaitable_Check` hasn't been and has no plan to be added to the Python C API as of CPython 3.9
  */
 bool PythonAwaitable_Check(PyObject *obj);
```

### Comparing `pythonmonkey-0.4.0/include/PyBaseProxyHandler.hh` & `pythonmonkey-0.6.0/include/PyBaseProxyHandler.hh`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.4.0/include/PyDictProxyHandler.hh` & `pythonmonkey-0.6.0/include/PyDictProxyHandler.hh`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /**
  * @file PyDictProxyHandler.hh
  * @author Caleb Aikens (caleb@distributive.network) and Philippe Laporte (philippe@distributive.network)
- * @brief Structs for creating JS proxy objects. Used by DictType for object coercion
+ * @brief Struct for creating JS proxy objects for Dicts
  * @date 2023-04-20
  *
  * @copyright Copyright (c) 2023-2024 Distributive Corp.
  *
  */
 
 #ifndef PythonMonkey_PyDictProxy_
@@ -73,17 +73,15 @@
     JS::HandleValue v, JS::HandleValue receiver,
     JS::ObjectOpResult &result) const override;
   /**
    * @brief [[Enumerate]]
    *
    * @param cx - pointer to JSContext
    * @param proxy - The proxy object who's keys we output
-   * @param props - out-parameter of object IDsoverride;
-
-     /**
+   * @param props - out-parameter of object IDs
    * @return true - call succeeded
    * @return false - call failed and an exception has been raised
    */
   bool enumerate(JSContext *cx, JS::HandleObject proxy,
     JS::MutableHandleIdVector props) const override;
 
   /**
```

### Comparing `pythonmonkey-0.4.0/include/PyEventLoop.hh` & `pythonmonkey-0.6.0/include/PyEventLoop.hh`

 * *Files 4% similar despite different names*

```diff
@@ -28,34 +28,46 @@
 
   /**
    * @brief C++ wrapper for Python `asyncio.Handle` class
    * @see https://docs.python.org/3/library/asyncio-eventloop.html#asyncio.Handle
    */
   struct AsyncHandle {
     using id_t = uint32_t;
-    using id_ptr_pair = std::pair<id_t, AsyncHandle *>;
   public:
     explicit AsyncHandle(PyObject *handle) : _handle(handle) {};
     AsyncHandle(const AsyncHandle &old) = delete; // forbid copy-initialization
     AsyncHandle(AsyncHandle &&old) : _handle(std::exchange(old._handle, nullptr)), _refed(old._refed.exchange(false)) {}; // clear the moved-from object
     ~AsyncHandle() {
       if (Py_IsInitialized()) { // the Python runtime has already been finalized when `_timeoutIdMap` is cleared at exit
         Py_XDECREF(_handle);
       }
     }
-    static inline id_ptr_pair newEmpty() {
+
+    /**
+     * @brief Create a new `AsyncHandle` without an associated `asyncio.Handle` Python object
+     * @return the timeoutId
+     */
+    static inline id_t newEmpty() {
       auto handle = AsyncHandle(Py_None);
-      return AsyncHandle::getUniqueIdAndPtr(std::move(handle));
+      return AsyncHandle::getUniqueId(std::move(handle));
     }
 
     /**
      * @brief Cancel the scheduled event-loop job.
      * If the job has already been canceled or executed, this method has no effect.
      */
     void cancel();
+    /**
+     * @return true if the job has been cancelled.
+     */
+    bool cancelled();
+    /**
+     * @return true if the job function has already been executed or cancelled.
+     */
+    bool _finishedOrCancelled();
 
     /**
      * @brief Get the unique `timeoutID` for JS `setTimeout`/`clearTimeout` methods
      * @see https://developer.mozilla.org/en-US/docs/Web/API/setTimeout#return_value
      */
     static inline id_t getUniqueId(AsyncHandle &&handle) {
       // TODO (Tom Tang): mutex lock
@@ -65,19 +77,14 @@
     static inline AsyncHandle *fromId(id_t timeoutID) {
       try {
         return &_timeoutIdMap.at(timeoutID);
       } catch (...) { // std::out_of_range&
         return nullptr; // invalid timeoutID
       }
     }
-    static inline id_ptr_pair getUniqueIdAndPtr(AsyncHandle &&handle) {
-      auto timeoutID = getUniqueId(std::move(handle));
-      auto ptr = fromId(timeoutID);
-      return std::make_pair(timeoutID, ptr);
-    }
 
     /**
      * @brief Get the underlying `asyncio.Handle` Python object
      */
     inline PyObject *getHandleObject() const {
       Py_INCREF(_handle); // otherwise the object would be GC-ed as the AsyncHandle destructor decreases the reference count
       return _handle;
@@ -100,15 +107,17 @@
 
     /**
      * @brief Ref the timer so that the event-loop won't exit as long as the timer is active
      */
     inline void addRef() {
       if (!_refed) {
         _refed = true;
-        PyEventLoop::_locker->incCounter();
+        if (!_finishedOrCancelled()) { // noop if the timer is finished or canceled
+          PyEventLoop::_locker->incCounter();
+        }
       }
     }
 
     /**
      * @brief Unref the timer so that the event-loop can exit
      */
     inline void removeRef() {
@@ -128,17 +137,18 @@
    * @return a AsyncHandle, the value can be safely ignored
    */
   AsyncHandle enqueue(PyObject *jobFn);
   /**
    * @brief Schedule a job to the Python event-loop, with the given delay
    * @param jobFn - The JS event-loop job converted to a Python function
    * @param delaySeconds - The job function will be called after the given number of seconds
-   * @return the timeoutId and a pointer to the AsyncHandle
+   * @param repeat - If true, the job will be executed repeatedly on a fixed interval
+   * @return the timeoutId
    */
-  [[nodiscard]] AsyncHandle::id_ptr_pair enqueueWithDelay(PyObject *jobFn, double delaySeconds);
+  [[nodiscard]] AsyncHandle::id_t enqueueWithDelay(PyObject *jobFn, double delaySeconds, bool repeat);
 
   /**
    * @brief C++ wrapper for Python `asyncio.Future` class
    * @see https://docs.python.org/3/library/asyncio-future.html#asyncio.Future
    */
   struct Future {
   public:
```

### Comparing `pythonmonkey-0.4.0/include/PyListProxyHandler.hh` & `pythonmonkey-0.6.0/include/PyListProxyHandler.hh`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /**
  * @file PyListProxyHandler.hh
  * @author Philippe Laporte (philippe@distributive.network)
- * @brief Structs for creating JS proxy objects. Used by ListType for List coercion
+ * @brief Struct for creating JS proxy objects for Lists
  * @date 2023-12-01
  *
  * @copyright Copyright (c) 2023-2024 Distributive Corp.
  *
  */
 
 #ifndef PythonMonkey_PyListProxy_
```

### Comparing `pythonmonkey-0.4.0/include/PyObjectProxyHandler.hh` & `pythonmonkey-0.6.0/include/PyObjectProxyHandler.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /**
  * @file PyObjectProxyHandler.hh
  * @author Caleb Aikens (caleb@distributive.network)
- * @brief Structs for creating JS proxy objects. Used for default object coercion
+ * @brief Struct for creating JS proxy objects for all objects
  * @date 2024-01-25
  *
  * @copyright Copyright (c) 2023 Distributive Corp.
  *
  */
 
 #ifndef PythonMonkey_PyObjectProxy_
```

### Comparing `pythonmonkey-0.4.0/include/PyType.hh` & `pythonmonkey-0.6.0/src/FuncType.cc`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,21 @@
 /**
- * @file PyType.hh
- * @author Caleb Aikens (caleb@distributive.network) & Giovanni Tedesco (giovanni@distributive.network)
- * @brief Struct representing python types
- * @date 2022-07-27
+ * @file FuncType.cc
+ * @author Caleb Aikens (caleb@distributive.network), Giovanni Tedesco (giovanni@distributive.network) and Philippe Laporte (philippe@distributive.network)
+ * @brief Struct representing python functions
+ * @date 2022-08-08
  *
- * @copyright Copyright (c) 2022 Distributive Corp.
+ * @copyright Copyright (c) 2022,2024 Distributive Corp.
  *
  */
 
-#ifndef PythonMonkey_PyType_
-#define PythonMonkey_PyType_
+#include "include/FuncType.hh"
+#include "include/JSFunctionProxy.hh"
 
-#include "TypeEnum.hh"
+#include <jsapi.h>
 
-#include <Python.h>
 
-/**
- * @brief Abstract struct that serves as a base for the different type relations in C++/Python
- */
-struct PyType {
-public:
-  PyType();
-  PyType(PyObject *object);
-  const TYPE returnType = TYPE::DEFAULT;
-  PyObject *getPyObject();
-  ~PyType();
-
-protected:
-  PyObject *pyObject = nullptr;
-};
-#endif
+PyObject *FuncType::getPyObject(JSContext *cx, JS::HandleValue fval) {
+  JSFunctionProxy *proxy = (JSFunctionProxy *)PyObject_CallObject((PyObject *)&JSFunctionProxyType, NULL);
+  proxy->jsFunc->set(&fval.toObject());
+  return (PyObject *)proxy;
+}
```

### Comparing `pythonmonkey-0.4.0/include/StrType.hh` & `pythonmonkey-0.6.0/include/StrType.hh`

 * *Files 24% similar despite different names*

```diff
@@ -1,55 +1,42 @@
 /**
  * @file StrType.hh
- * @author Caleb Aikens (caleb@distributive.network) & Giovanni Tedesco (giovanni@distributive.network)
+ * @author Caleb Aikens (caleb@distributive.network), Giovanni Tedesco (giovanni@distributive.network) and Philippe Laporte (philippe@distributive.network)
  * @brief Struct for representing python strings
  * @date 2022-08-08
  *
- * @copyright Copyright (c) 2022 Distributive Corp.
+ * @copyright Copyright (c) 2022,2024 Distributive Corp.
  *
  */
 
 #ifndef PythonMonkey_StrType_
 #define PythonMonkey_StrType_
 
-#include "PyType.hh"
-#include "TypeEnum.hh"
-
 #include <jsapi.h>
 
 #include <Python.h>
 
 /**
- * @brief This struct represents the 'string' type in Python, which is represented as a 'char*' in C++. It inherits from the PyType struct
+ * @brief This struct represents the 'string' type in Python, which is represented as a 'char*' in C++
  */
-struct StrType : public PyType {
+struct StrType {
 public:
-  StrType(PyObject *object);
-  StrType(char *string);
-
   /**
-   * @brief Construct a new StrType object from a JSString. Automatically handles encoding conversion for latin1 & UCS2:
+   * @brief Construct a new unicode PyObject from a JSString. Automatically handles encoding conversion for latin1 & UCS2:
    * codepoint     | Python          | Spidermonkey     | identical representation?
    * 000000-0000FF | latin1          | latin1           | Yes
    * 000100-00D7FF | UCS2            | UTF16            | Yes
    * 00D800-00DFFF | UCS2 (unpaired) | UTF16 (unpaired) | Yes
    * 00E000-00FFFF | UCS2            | UTF16            | Yes
-   * 010000-10FFFF | UCS4            | UTF16            | No, conversion and new backing store required, user must explicitly call asUCS4()
+   * 010000-10FFFF | UCS4            | UTF16            | No, conversion and new backing store required, user must explicitly call asUCS4() -> static in code
    *
    * @param cx - javascript context pointer
    * @param str - JSString pointer
-   */
-  StrType(JSContext *cx, JSString *str);
-
-  const TYPE returnType = TYPE::STRING;
-  const char *getValue() const;
-
-  /**
-   * @brief creates new UCS4-encoded pyObject string. This must be called by the user if the original JSString contains any surrogate pairs
-   *
-   * @return PyObject* - the UCS4-encoding of the pyObject string
    *
+   * @returns PyObject* pointer to the resulting PyObject
    */
-  static PyObject *asUCS4(PyObject *pyObject);
+  static PyObject *getPyObject(JSContext *cx, JSString *str);
+
+  static const char *getValue(JSContext *cx, JSString *str);
 };
 
 #endif
```

### Comparing `pythonmonkey-0.4.0/include/internalBinding.hh` & `pythonmonkey-0.6.0/include/internalBinding.hh`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.4.0/include/jsTypeFactory.hh` & `pythonmonkey-0.6.0/include/jsTypeFactory.hh`

 * *Files 5% similar despite different names*

```diff
@@ -7,18 +7,18 @@
  * @copyright Copyright (c) 2023 Distributive Corp.
  *
  */
 
 #ifndef PythonMonkey_JsTypeFactory_
 #define PythonMonkey_JsTypeFactory_
 
-#include "include/PyType.hh"
-
 #include <jsapi.h>
 
+#include <Python.h>
+
 
 struct PythonExternalString;
 
 /**
  * @brief Function that makes a UTF16-encoded copy of a UCS4 string
  *
  * @param chars - pointer to the UCS4-encoded string
```

### Comparing `pythonmonkey-0.4.0/include/modules/pythonmonkey/pythonmonkey.hh` & `pythonmonkey-0.6.0/include/modules/pythonmonkey/pythonmonkey.hh`

 * *Files 14% similar despite different names*

```diff
@@ -6,32 +6,33 @@
  *
  * @copyright Copyright (c) 2022-2024 Distributive Corp.
  *
  */
 #ifndef PythonMonkey_Module_PythonMonkey
 #define PythonMonkey_Module_PythonMonkey
 
-#include "include/PyType.hh"
 #include "include/JobQueue.hh"
 
 #include <jsapi.h>
 #include <js/CompilationAndEvaluation.h>
 #include <js/Initialization.h>
 
 #include <Python.h>
 
-#define PythonMonkey_Null   PyObject_GetAttrString(PyState_FindModule(&pythonmonkey), "null")   /**< macro for pythonmonkey.null object*/
-#define PythonMonkey_BigInt PyObject_GetAttrString(PyState_FindModule(&pythonmonkey), "bigint") /**< macro for pythonmonkey.bigint class object */
 
 extern JSContext *GLOBAL_CX; /**< pointer to PythonMonkey's JSContext */
 extern JS::PersistentRootedObject jsFunctionRegistry; /**<// this is a FinalizationRegistry for JSFunctions that depend on Python functions. It is used to handle reference counts when the JSFunction is finalized */
 static JS::Rooted<JSObject *> *global; /**< pointer to the global object of PythonMonkey's JSContext */
 static JSAutoRealm *autoRealm; /**< pointer to PythonMonkey's AutoRealm */
 static JobQueue *JOB_QUEUE; /**< pointer to PythonMonkey's event-loop job queue */
 
+// Get handle on global object
+PyObject *getPythonMonkeyNull();
+PyObject *getPythonMonkeyBigInt();
+
 /**
  * @brief Destroys the JSContext and deletes associated memory. Called when python quits or faces a fatal exception.
  *
  */
 static void cleanup();
 
 /**
```

### Comparing `pythonmonkey-0.4.0/include/pyTypeFactory.hh` & `pythonmonkey-0.6.0/include/pyTypeFactory.hh`

 * *Files 12% similar despite different names*

```diff
@@ -7,24 +7,22 @@
  * @copyright Copyright (c) 2022, 2023, 2024 Distributive Corp.
  *
  */
 
 #ifndef PythonMonkey_PyTypeFactory_
 #define PythonMonkey_PyTypeFactory_
 
-#include "PyType.hh"
-
 #include <jsapi.h>
 
 #include <Python.h>
 
 
 /**
- * @brief Function that takes a JS::Value and returns a corresponding PyType* object, doing shared memory management when necessary
+ * @brief Function that takes a JS::Value and returns a corresponding PyObject* object, doing shared memory management when necessary
  *
  * @param cx - Pointer to the javascript context of the JS::Value
  * @param rval - The JS::Value who's type and value we wish to encapsulate
- * @return PyType* - Pointer to a PyType object corresponding to the JS::Value
+ * @return PyObject* - Pointer to the object corresponding to the JS::Value
  */
-PyType *pyTypeFactory(JSContext *cx, JS::HandleValue rval);
+PyObject *pyTypeFactory(JSContext *cx, JS::HandleValue rval);
 
 #endif
```

### Comparing `pythonmonkey-0.4.0/include/setSpiderMonkeyException.hh` & `pythonmonkey-0.6.0/include/setSpiderMonkeyException.hh`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.4.0/pyproject.toml` & `pythonmonkey-0.6.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pythonmonkey"
-version = "0.4.0" # automatically set by poetry-dynamic-versioning
+version = "0.6.0" # automatically set by poetry-dynamic-versioning
 description = ""
 authors = ["Caleb Aikens <caleb@distributive.network>", "Tom Tang <xmader@distributive.network>", "Wes Garland <wes@distributive.network>", "Hamada Gasmallah <hamada@distributive.network>", "Philippe Laporte <philippe@distributive.network>"]
 readme = "README.md"
 packages = [
   { include = "pythonmonkey", from = "python" },
 ]
 include = [
@@ -25,16 +25,16 @@
   { path = "*.sh", format = "sdist" },
 ]
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pyreadline3 = { version = "^3.4.1", platform = "win32" }
-aiohttp = { version = "^3.9.3", extras = ["speedups"] }
-pminit = { version = "*", allow-prereleases = true }
+aiohttp = { version = "^3.9.5", extras = ["speedups"] }
+pminit = { version = ">=0.4.0", allow-prereleases = true }
 
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 style = "pep440"
 bump = true
@@ -62,7 +62,15 @@
 ]
 pminit = { path = "./python/pminit", develop = true }
 
 
 [build-system]
 requires = ["poetry-core>=1.1.1", "poetry-dynamic-versioning==1.1.1"]
 build-backend = "poetry_dynamic_versioning.backend"
+
+[tool.autopep8]
+max_line_length=120
+ignore="E111,E114,E121" # allow 2-space indents
+verbose=true
+indent-size=2
+aggressive=3
+exit-code=true
```

### Comparing `pythonmonkey-0.4.0/python/pythonmonkey/builtin_modules/XMLHttpRequest-internal.d.ts` & `pythonmonkey-0.6.0/python/pythonmonkey/builtin_modules/XMLHttpRequest-internal.d.ts`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.4.0/python/pythonmonkey/builtin_modules/XMLHttpRequest-internal.py` & `pythonmonkey-0.6.0/python/pythonmonkey/builtin_modules/XMLHttpRequest-internal.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,25 +8,27 @@
 import aiohttp
 import yarl
 import io
 import platform
 import pythonmonkey as pm
 from typing import Union, ByteString, Callable, TypedDict
 
+
 class XHRResponse(TypedDict, total=True):
-    """
-    See definitions in `XMLHttpRequest-internal.d.ts`
-    """
-    url: str
-    status: int
-    statusText: str
-    contentLength: int
-    getResponseHeader: Callable[[str], Union[str, None]]
-    getAllResponseHeaders: Callable[[], str]
-    abort: Callable[[], None]
+  """
+  See definitions in `XMLHttpRequest-internal.d.ts`
+  """
+  url: str
+  status: int
+  statusText: str
+  contentLength: int
+  getResponseHeader: Callable[[str], Union[str, None]]
+  getAllResponseHeaders: Callable[[], str]
+  abort: Callable[[], None]
+
 
 async def request(
     method: str,
     url: str,
     headers: dict,
     body: Union[str, ByteString],
     timeoutMs: float,
@@ -38,87 +40,91 @@
     processBodyChunk: Callable[[bytearray], None],
     processEndOfBody: Callable[[], None],
     # callbacks for known exceptions
     onTimeoutError: Callable[[asyncio.TimeoutError], None],
     onNetworkError: Callable[[aiohttp.ClientError], None],
     /
 ):
-    debug = pm.bootstrap.require("debug");
+  debug = pm.bootstrap.require("debug")
+
+  class BytesPayloadWithProgress(aiohttp.BytesPayload):
+    _chunkMaxLength = 2**16  # aiohttp default
+
+    async def write(self, writer) -> None:
+      debug('xhr:io')('begin chunked write')
+      buf = io.BytesIO(self._value)
+      chunk = buf.read(self._chunkMaxLength)
+      while chunk:
+        debug('xhr:io')('  writing', len(chunk), 'bytes')
+        await writer.write(chunk)
+        processRequestBodyChunkLength(len(chunk))
+        chunk = buf.read(self._chunkMaxLength)
+      processRequestEndOfBody()
+      debug('xhr:io')('finish chunked write')
+
+  if isinstance(body, str):
+    body = bytes(body, "utf-8")
+
+  # set default headers
+  headers.setdefault("user-agent", f"Python/{platform.python_version()} PythonMonkey/{pm.__version__}")
+  debug('xhr:headers')('after set default\n', headers)
+
+  if timeoutMs > 0:
+    timeoutOptions = aiohttp.ClientTimeout(total=timeoutMs / 1000)  # convert to seconds
+  else:
+    timeoutOptions = aiohttp.ClientTimeout()  # default timeout
+
+  try:
+    debug('xhr:aiohttp')('creating request for', url)
+    async with aiohttp.request(method=method,
+                               url=yarl.URL(url, encoded=True),
+                               headers=headers,
+                               data=BytesPayloadWithProgress(body) if body else None,
+                               timeout=timeoutOptions,
+                               ) as res:
+      debug('xhr:aiohttp')('got', res.content_type, 'result')
+
+      def getResponseHeader(name: str):
+        return res.headers.get(name)
+
+      def getAllResponseHeaders():
+        headers = []
+        for name, value in res.headers.items():
+          headers.append(f"{name.lower()}: {value}")
+        headers.sort()
+        return "\r\n".join(headers)
+
+      def abort():
+        debug('xhr:io')('abort')
+        res.close()
+
+      # readyState HEADERS_RECEIVED
+      processResponse({
+          'url': str(res.real_url),
+          'status': res.status,
+          'statusText': str(res.reason or ''),
+
+          'getResponseHeader': getResponseHeader,
+          'getAllResponseHeaders': getAllResponseHeaders,
+          'abort': abort,
+          'contentLength': res.content_length or 0,
+      })
+
+      async for data in res.content.iter_any():
+        processBodyChunk(bytearray(data))  # PythonMonkey only accepts the mutable bytearray type
+      # readyState DONE
+      processEndOfBody()
+  except asyncio.TimeoutError as e:
+    onTimeoutError(e)
+    raise  # rethrow
+  except aiohttp.ClientError as e:
+    onNetworkError(e)
+    raise  # rethrow
 
-    class BytesPayloadWithProgress(aiohttp.BytesPayload):
-        _chunkMaxLength = 2**16 # aiohttp default
 
-        async def write(self, writer) -> None:
-            debug('xhr:io')('begin chunked write')
-            buf = io.BytesIO(self._value)
-            chunk = buf.read(self._chunkMaxLength)
-            while chunk:
-                debug('xhr:io')('  writing', len(chunk), 'bytes')
-                await writer.write(chunk)
-                processRequestBodyChunkLength(len(chunk))
-                chunk = buf.read(self._chunkMaxLength)
-            processRequestEndOfBody()
-            debug('xhr:io')('finish chunked write')
-
-    if isinstance(body, str):
-        body = bytes(body, "utf-8")
-
-    # set default headers
-    headers.setdefault("user-agent", f"Python/{platform.python_version()} PythonMonkey/{pm.__version__}")
-    debug('xhr:headers')('after set default\n', headers)
-
-    if timeoutMs > 0:
-        timeoutOptions = aiohttp.ClientTimeout(total=timeoutMs/1000) # convert to seconds
-    else:
-        timeoutOptions = aiohttp.ClientTimeout() # default timeout
-
-    try:
-        debug('xhr:aiohttp')('creating request for', url)
-        async with aiohttp.request(method=method,
-                                url=yarl.URL(url, encoded=True),
-                                headers=headers,
-                                data=BytesPayloadWithProgress(body) if body else None,
-                                timeout=timeoutOptions,
-        ) as res:
-            debug('xhr:aiohttp')('got', res.content_type, 'result')
-            def getResponseHeader(name: str):
-                return res.headers.get(name)
-            def getAllResponseHeaders():
-                headers = []
-                for name, value in res.headers.items():
-                    headers.append(f"{name.lower()}: {value}")
-                headers.sort()
-                return "\r\n".join(headers)
-            def abort():
-                debug('xhr:io')('abort')
-                res.close()
-
-            # readyState HEADERS_RECEIVED
-            responseData: XHRResponse = { # FIXME: PythonMonkey bug: the dict will be GCed if directly as an argument
-                'url': str(res.real_url),
-                'status': res.status,
-                'statusText': str(res.reason or ''),
-
-                'getResponseHeader': getResponseHeader,
-                'getAllResponseHeaders': getAllResponseHeaders,
-                'abort': abort,
-                'contentLength': res.content_length or 0,
-            }
-            processResponse(responseData)
-
-            async for data in res.content.iter_any():
-                processBodyChunk(bytearray(data)) # PythonMonkey only accepts the mutable bytearray type
-            # readyState DONE
-            processEndOfBody()
-    except asyncio.TimeoutError as e:
-        onTimeoutError(e)
-        raise # rethrow
-    except aiohttp.ClientError as e:
-        onNetworkError(e)
-        raise # rethrow
+def decodeStr(data: bytes, encoding='utf-8'):  # XXX: Remove this once we get proper TextDecoder support
+  return str(data, encoding=encoding)
 
-def decodeStr(data: bytes, encoding='utf-8'): # XXX: Remove this once we get proper TextDecoder support
-    return str(data, encoding=encoding)
 
 # Module exports
-exports['request'] = request # type: ignore
-exports['decodeStr'] = decodeStr # type: ignore
+exports['request'] = request  # type: ignore
+exports['decodeStr'] = decodeStr  # type: ignore
```

### Comparing `pythonmonkey-0.4.0/python/pythonmonkey/builtin_modules/XMLHttpRequest.js` & `pythonmonkey-0.6.0/python/pythonmonkey/builtin_modules/XMLHttpRequest.js`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.4.0/python/pythonmonkey/builtin_modules/base64.d.ts` & `pythonmonkey-0.6.0/python/pythonmonkey/builtin_modules/base64.d.ts`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.4.0/python/pythonmonkey/builtin_modules/console.js` & `pythonmonkey-0.6.0/python/pythonmonkey/builtin_modules/console.js`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.4.0/python/pythonmonkey/builtin_modules/dom-exception.d.ts` & `pythonmonkey-0.6.0/python/pythonmonkey/builtin_modules/dom-exception.d.ts`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.4.0/python/pythonmonkey/builtin_modules/event-target.js` & `pythonmonkey-0.6.0/python/pythonmonkey/builtin_modules/event-target.js`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.4.0/python/pythonmonkey/builtin_modules/internal-binding.d.ts` & `pythonmonkey-0.6.0/python/pythonmonkey/builtin_modules/internal-binding.d.ts`

 * *Files 6% similar despite different names*

```diff
@@ -30,20 +30,22 @@
    * @return `undefined` if it's not a proxy
    */
   getProxyDetails<T extends object>(proxy: T): undefined | [target: T, handler: ProxyHandler<T>];
 };
 
 declare function internalBinding(namespace: "timers"): {
   /**
-   * internal binding helper for the `setTimeout` global function
+   * internal binding helper for the `setTimeout`/`setInterval` global functions
    * 
    * **UNSAFE**, does not perform argument type checks
+   * 
+   * @param repeat The call is to `setInterval` if true
    * @return timeoutId
    */
-  enqueueWithDelay(handler: Function, delaySeconds: number): number;
+  enqueueWithDelay(handler: Function, delaySeconds: number, repeat: boolean): number;
 
   /**
    * internal binding helper for the `clearTimeout` global function
    */
   cancelByTimeoutId(timeoutId: number): void;
 
   /**
```

### Comparing `pythonmonkey-0.4.0/python/pythonmonkey/builtin_modules/timers.js` & `pythonmonkey-0.6.0/python/pythonmonkey/builtin_modules/timers.js`

 * *Files 22% similar despite different names*

#### js-beautify {}

```diff
@@ -11,14 +11,18 @@
     enqueueWithDelay,
     cancelByTimeoutId,
     timerHasRef,
     timerAddRef,
     timerRemoveRef,
 } = internalBinding('timers');
 
+const {
+    DOMException
+} = require('dom-exception');
+
 /**
  * Implement Node.js-style `timeoutId` class returned from setTimeout() and setInterval()
  * @see https://nodejs.org/api/timers.html#class-timeout
  */
 class Timeout {
     /** @type {number} an integer */
     #numericId;
@@ -54,60 +58,89 @@
      */
     unref() {
         timerRemoveRef(this.#numericId);
         return this; // allow chaining
     }
 
     /**
-     * @returns a number that can be used to reference this timeout
-     */
-    [Symbol.toPrimitive]() {
-        return this.#numericId;
+     * Sets the timer's start time to the current time, 
+     * and reschedules the timer to call its callback at the previously specified duration adjusted to the current time.
+     * 
+     * Using this on a timer that has already called its callback will reactivate the timer.
+     */
+    refresh() {
+        throw new DOMException('Timeout.refresh() method is not supported by PythonMonkey.', 'NotSupportedError');
+        // TODO: Do we really need to closely resemble the Node.js API?
+        // This one is not easy to implement since we need to memorize the callback function and delay parameters in every `setTimeout`/`setInterval` call.
     }
 
     /**
      * Cancels the timeout.
      * @deprecated legacy Node.js API. Use `clearTimeout()` instead
      */
     close() {
         return clearTimeout(this);
     }
+
+    /**
+     * @returns a number that can be used to reference this timeout
+     */
+    [Symbol.toPrimitive]() {
+        return this.#numericId;
+    }
 }
 
 /**
- * Implement the `setTimeout` global function
- * @see https://developer.mozilla.org/en-US/docs/Web/API/setTimeout and
- * @see https://html.spec.whatwg.org/multipage/timers-and-user-prompts.html#dom-settimeout
+ * Normalize the arguments to `setTimeout` or `setInterval`
  * @param {Function | string} handler
- * @param {number} delayMs timeout milliseconds, use value of 0 if this is omitted
- * @param {any[]} args additional arguments to be passed to the `handler`
- * @return {Timeout} timeoutId
+ * @param {number} delayMs timeout milliseconds
+ * @param {any[]} additionalArgs additional arguments to be passed to the `handler`
  */
-function setTimeout(handler, delayMs = 0, ...args) {
+function _normalizeTimerArgs(handler, delayMs, additionalArgs) {
     // Ensure the first parameter is a function
     // We support passing a `code` string to `setTimeout` as the callback function
     if (typeof handler !== 'function')
         handler = new Function(handler);
 
     // `setTimeout` allows passing additional arguments to the callback, as spec-ed
     // FIXME (Tom Tang): the spec doesn't allow additional arguments to be passed if the original `handler` is not a function
     const thisArg = globalThis; // HTML spec requires `thisArg` to be the global object
     // Wrap the job function into a bound function with the given additional arguments
     //    https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/bind
     /** @type {Function} */
-    const boundHandler = handler.bind(thisArg, ...args);
+    const boundHandler = handler.bind(thisArg, ...additionalArgs);
 
     // Get the delay time in seconds
     //  JS `setTimeout` takes milliseconds, but Python takes seconds
     delayMs = Number(delayMs) || 0; // ensure the `delayMs` is a `number`, explicitly do type coercion
     if (delayMs < 0)
         delayMs = 0; // as spec-ed
     const delaySeconds = delayMs / 1000; // convert ms to s
 
-    return new Timeout(enqueueWithDelay(boundHandler, delaySeconds));
+    return {
+        boundHandler,
+        delaySeconds
+    };
+}
+
+/**
+ * Implement the `setTimeout` global function
+ * @see https://developer.mozilla.org/en-US/docs/Web/API/setTimeout and
+ * @see https://html.spec.whatwg.org/multipage/timers-and-user-prompts.html#dom-settimeout
+ * @param {Function | string} handler
+ * @param {number} delayMs timeout milliseconds, use value of 0 if this is omitted
+ * @param {any[]} args additional arguments to be passed to the `handler`
+ * @return {Timeout} timeoutId
+ */
+function setTimeout(handler, delayMs = 0, ...args) {
+    const {
+        boundHandler,
+        delaySeconds
+    } = _normalizeTimerArgs(handler, delayMs, args);
+    return new Timeout(enqueueWithDelay(boundHandler, delaySeconds, false));
 }
 
 /**
  * Implement the `clearTimeout` global function
  * @see https://developer.mozilla.org/en-US/docs/Web/API/clearTimeout and
  * @see https://html.spec.whatwg.org/multipage/timers-and-user-prompts.html#dom-cleartimeout
  * @param {Timeout | number} timeoutId
@@ -117,17 +150,49 @@
     // silently does nothing when an invalid timeoutId (should be a Timeout instance or an int32 value) is passed in
     if (!(timeoutId instanceof Timeout) && !Number.isInteger(timeoutId))
         return;
 
     return cancelByTimeoutId(Number(timeoutId));
 }
 
+/**
+ * Implement the `setInterval` global function
+ * @see https://developer.mozilla.org/en-US/docs/Web/API/setInterval and
+ * @see https://html.spec.whatwg.org/multipage/timers-and-user-prompts.html#dom-setinterval
+ * @param {Function | string} handler
+ * @param {number} delayMs timeout milliseconds, use value of 0 if this is omitted
+ * @param {any[]} args additional arguments to be passed to the `handler`
+ * @return {Timeout} timeoutId
+ */
+function setInterval(handler, delayMs = 0, ...args) {
+    const {
+        boundHandler,
+        delaySeconds
+    } = _normalizeTimerArgs(handler, delayMs, args);
+    return new Timeout(enqueueWithDelay(boundHandler, delaySeconds, true));
+}
+
+/**
+ * Implement the `clearInterval` global function
+ * @alias to `clearTimeout`
+ * @see https://developer.mozilla.org/en-US/docs/Web/API/clearInterval
+ */
+const clearInterval = clearTimeout;
+
 // expose the `Timeout` class
 setTimeout.Timeout = Timeout;
+setInterval.Timeout = Timeout;
 
 if (!globalThis.setTimeout)
     globalThis.setTimeout = setTimeout;
 if (!globalThis.clearTimeout)
     globalThis.clearTimeout = clearTimeout;
 
+if (!globalThis.setInterval)
+    globalThis.setInterval = setInterval;
+if (!globalThis.clearInterval)
+    globalThis.clearInterval = clearInterval;
+
 exports.setTimeout = setTimeout;
-exports.clearTimeout = clearTimeout;
+exports.clearTimeout = clearTimeout;
+exports.setInterval = setInterval;
+exports.clearInterval = clearInterval;
```

### Comparing `pythonmonkey-0.4.0/python/pythonmonkey/builtin_modules/url.d.ts` & `pythonmonkey-0.6.0/python/pythonmonkey/builtin_modules/url.d.ts`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.4.0/python/pythonmonkey/builtin_modules/util.js` & `pythonmonkey-0.6.0/python/pythonmonkey/builtin_modules/util.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -5,41 +5,42 @@
  *
  * @author   Tom Tang <xmader@distributive.network>
  * @date     June 2023
  * 
  * @copyright Copyright (c) 2023 Distributive Corp.
  */
 
-const internalBinding = require("internal-binding")
+const internalBinding = require('internal-binding');
 
 const {
     isAnyArrayBuffer,
     isPromise,
     isRegExp,
     isTypedArray,
     getPromiseDetails,
     getProxyDetails,
-} = internalBinding("utils")
+} = internalBinding('utils');
 
-const customInspectSymbol = Symbol.for('nodejs.util.inspect.custom')
+const customInspectSymbol = Symbol.for('nodejs.util.inspect.custom');
 
 // Keep this in sync with both SpiderMonkey and V8
 /** @type {PromiseState.Pending} */
 const kPending = 0;
 /** @type {PromiseState.Fulfilled} */
+// eslint-disable-next-line no-unused-vars
 const kFulfilled = 1;
 /** @type {PromiseState.Rejected} */
 const kRejected = 2;
 
 /**
  * @param {string[]} output 
  * @param {string} separator 
  */
 function join(output, separator) {
-    return output.join(separator)
+    return output.join(separator);
 }
 
 /**
  * @return {o is Error}
  */
 function isError(e) {
     return objectToString(e) === '[object Error]' || e instanceof Error;
@@ -84,28 +85,28 @@
 function objectToString(o) {
     return Object.prototype.toString.call(o);
 }
 
 // https://github.com/nodejs/node/blob/v8.17.0/lib/internal/util.js#L189-L202
 function getConstructorOf(obj) {
     while (obj) {
-        var descriptor = Object.getOwnPropertyDescriptor(obj, 'constructor');
+        let descriptor = Object.getOwnPropertyDescriptor(obj, 'constructor');
         if (descriptor !== undefined &&
             typeof descriptor.value === 'function' &&
             descriptor.value.name !== '') {
             return descriptor.value;
         }
 
         obj = Object.getPrototypeOf(obj);
     }
 
     return null;
 }
 
-/*! Start verbatim Node.js
+/* ! Start verbatim Node.js
  *  https://github.com/nodejs/node/blob/v8.17.0/lib/util.js#L59-L852
  */
 const inspectDefaultOptions = Object.seal({
     showHidden: false,
     depth: 2,
     colors: true,
     customInspect: true,
@@ -115,27 +116,28 @@
 });
 
 const propertyIsEnumerable = Object.prototype.propertyIsEnumerable;
 const regExpToString = RegExp.prototype.toString;
 const dateToISOString = Date.prototype.toISOString;
 
 /** Return String(val) surrounded by appropriate ANSI escape codes to change the console text colour. */
+// eslint-disable-next-line no-unused-vars
 function colour(colourCode, val) {
     const esc = String.fromCharCode(27);
-    return `${esc}[${colourCode}m${val}${esc}[0m`
+    return `${esc}[${colourCode}m${val}${esc}[0m`;
 }
 
-var CIRCULAR_ERROR_MESSAGE;
+let CIRCULAR_ERROR_MESSAGE;
 
 /* eslint-disable */
 const strEscapeSequencesRegExp = /[\x00-\x1f\x27\x5c]/;
 const strEscapeSequencesReplacer = /[\x00-\x1f\x27\x5c]/g;
+const colorRegExp = /\u001b\[\d\d?m/g;
 /* eslint-enable */
 const keyStrRegExp = /^[a-zA-Z_][a-zA-Z_0-9]*$/;
-const colorRegExp = /\u001b\[\d\d?m/g;
 const numberRegExp = /^(0|[1-9][0-9]*)$/;
 
 // Escaped special characters. Use empty strings to fill up unused entries.
 const meta = [
     '\\u0000', '\\u0001', '\\u0002', '\\u0003', '\\u0004',
     '\\u0005', '\\u0006', '\\u0007', '\\b', '\\t',
     '\\n', '\\u000b', '\\f', '\\r', '\\u000e',
@@ -157,17 +159,18 @@
 // This is similar to JSON stringify escaping.
 function strEscape(str) {
     // Some magic numbers that worked out fine while benchmarking with v8 6.0
     if (str.length < 5000 && !strEscapeSequencesRegExp.test(str))
         return `'${str}'`;
     if (str.length > 100)
         return `'${str.replace(strEscapeSequencesReplacer, escapeFn)}'`;
-    var result = '';
-    var last = 0;
-    for (var i = 0; i < str.length; i++) {
+    let result = '';
+    let last = 0;
+    let i;
+    for (i = 0; i < str.length; i++) {
         const point = str.charCodeAt(i);
         if (point === 39 || point === 92 || point < 32) {
             if (last === i) {
                 result += meta[point];
             } else {
                 result += `${str.slice(last, i)}${meta[point]}`;
             }
@@ -188,42 +191,42 @@
     } catch (err) {
         // Populate the circular error message lazily
         if (!CIRCULAR_ERROR_MESSAGE) {
             try {
                 const a = {};
                 a.a = a;
                 JSON.stringify(a);
-            } catch (err) {
-                CIRCULAR_ERROR_MESSAGE = err.message;
+            } catch (err2) {
+                CIRCULAR_ERROR_MESSAGE = err2.message;
             }
         }
         if (err.name === 'TypeError' && err.message === CIRCULAR_ERROR_MESSAGE)
             return '[Circular]';
         throw err;
     }
 }
 
 function format(f) {
-    var i, tempStr;
+    let i, tempStr;
     if (typeof f !== 'string') {
         if (arguments.length === 0) return '';
-        var res = '';
+        let res = '';
         for (i = 0; i < arguments.length - 1; i++) {
             res += inspect(arguments[i]);
             res += ' ';
         }
         res += inspect(arguments[i]);
         return res;
     }
 
     if (arguments.length === 1) return f;
 
-    var str = '';
-    var a = 1;
-    var lastPos = 0;
+    let str = '';
+    let a = 1;
+    let lastPos = 0;
     for (i = 0; i < f.length - 1; i++) {
         if (f.charCodeAt(i) === 37) { // '%'
             const nextChar = f.charCodeAt(++i);
             if (a !== arguments.length) {
                 switch (nextChar) {
                     case 115: // 's'
                         tempStr = String(arguments[a++]);
@@ -241,15 +244,15 @@
                         tempStr = inspect(arguments[a++], {
                             showHidden: true,
                             depth: 4,
                             showProxy: true
                         });
                         break;
                     case 105: // 'i'
-                        tempStr = `${parseInt(arguments[a++])}`;
+                        tempStr = `${parseInt(arguments[a++], 10)}`;
                         break;
                     case 102: // 'f'
                         tempStr = `${parseFloat(arguments[a++])}`;
                         break;
                     case 37: // '%'
                         str += f.slice(lastPos, i);
                         lastPos = i + 1;
@@ -314,15 +317,15 @@
         }
     }
     // Set user-specified options
     if (typeof opts === 'boolean') {
         ctx.showHidden = opts;
     } else if (opts) {
         const optKeys = Object.keys(opts);
-        for (var i = 0; i < optKeys.length; i++) {
+        for (let i = 0; i < optKeys.length; i++) {
             ctx[optKeys[i]] = opts[optKeys[i]];
         }
     }
     if (ctx.colors) ctx.stylize = stylizeWithColor;
     if (ctx.maxArrayLength === null) ctx.maxArrayLength = Infinity;
     return formatValue(ctx, obj, ctx.depth);
 }
@@ -333,15 +336,14 @@
         return inspectDefaultOptions;
     },
     set(options) {
         if (options === null || typeof options !== 'object') {
             throw new TypeError('"options" must be an object');
         }
         Object.assign(inspectDefaultOptions, options);
-        return inspectDefaultOptions;
     }
 });
 
 // http://en.wikipedia.org/wiki/ANSI_escape_code#graphics
 inspect.colors = Object.assign(Object.create(null), {
     'bold': [1, 22],
     'italic': [3, 23],
@@ -394,15 +396,15 @@
     if (value === null) {
         return ctx.stylize('null', 'null');
     }
 
     if (ctx.showProxy) {
         const proxy = getProxyDetails(value);
         if (proxy !== undefined) {
-            if (recurseTimes != null) {
+            if (recurseTimes !== null) {
                 if (recurseTimes < 0)
                     return ctx.stylize('Proxy [Array]', 'special');
                 recurseTimes -= 1;
             }
             ctx.indentationLvl += 2;
             const res = [
                 formatValue(ctx, proxy[0], recurseTimes),
@@ -415,34 +417,36 @@
     }
 
     // Provide a hook for user-specified inspect functions.
     // Check that value is an object with an inspect function on it
     if (ctx.customInspect) {
         const maybeCustomInspect = value[customInspectSymbol] || value.inspect;
 
-        if (typeof maybeCustomInspect === 'function' &&
+        if (typeof maybeCustomInspect === 'function'
             // Filter out the util module, its inspect function is special
-            maybeCustomInspect !== inspect &&
+            &&
+            maybeCustomInspect !== inspect
             // Also filter out any prototype objects using the circular check.
+            &&
             !(value.constructor && value.constructor.prototype === value)) {
             const ret = maybeCustomInspect.call(value, recurseTimes, ctx);
 
             // If the custom inspection method returned `this`, don't go into
             // infinite recursion.
             if (ret !== value) {
                 if (typeof ret !== 'string') {
                     return formatValue(ctx, ret, recurseTimes);
                 }
                 return ret;
             }
         }
     }
 
-    var keys;
-    var symbols = Object.getOwnPropertySymbols(value);
+    let keys;
+    let symbols = Object.getOwnPropertySymbols(value);
 
     // Look up the keys of the object.
     if (ctx.showHidden) {
         keys = Object.getOwnPropertyNames(value);
     } else {
         keys = Object.keys(value);
         if (symbols.length !== 0)
@@ -450,19 +454,19 @@
     }
 
     const keyLength = keys.length + symbols.length;
     const constructor = getConstructorOf(value);
     const ctorName = constructor && constructor.name ?
         `${constructor.name} ` : '';
 
-    var base = '';
-    var formatter = formatObject;
-    var braces;
-    var noIterator = true;
-    var raw;
+    let base = '';
+    let formatter = formatObject;
+    let braces;
+    let noIterator = true;
+    let raw;
 
     // Iterators and the rest are split to reduce checks
     if (value[Symbol.iterator]) {
         noIterator = false;
         if (Array.isArray(value)) {
             // Only set the constructor for non ordinary ("Array [...]") arrays.
             braces = [`${ctorName === 'Array ' ? '' : ctorName}[`, ']'];
@@ -593,27 +597,27 @@
     }
 
     // Using an array here is actually better for the average case than using
     // a Set. `seen` will only check for the depth and will never grow to large.
     if (ctx.seen.indexOf(value) !== -1)
         return ctx.stylize('[Circular]', 'special');
 
-    if (recurseTimes != null) {
+    if (recurseTimes !== null) {
         if (recurseTimes < 0) {
             if (Array.isArray(value))
                 return ctx.stylize('[Array]', 'special');
             return ctx.stylize('[Object]', 'special');
         }
         recurseTimes -= 1;
     }
 
     ctx.seen.push(value);
     const output = formatter(ctx, value, recurseTimes, keys);
 
-    for (var i = 0; i < symbols.length; i++) {
+    for (let i = 0; i < symbols.length; i++) {
         output.push(formatProperty(ctx, value, recurseTimes, symbols[i], 0));
     }
     ctx.seen.pop();
 
     return reduceToSingleString(ctx, output, base, braces, ln);
 }
 
@@ -651,40 +655,39 @@
         return ctx.stylize(str, 'error2');
     }
 
     const stackEls = error.stack
         .split('\n')
         .filter(a => a.length > 0)
         .map(a => `    ${a}`);
-    const retstr =
-        `${error.name}: ${error.message}\n` +
+    const retstr = `${error.name}: ${error.message}\n` +
         stackEls[0] + '\n' +
         style(stackEls.slice(1).join('\n'));
     return retstr;
 }
 
 function formatObject(ctx, value, recurseTimes, keys) {
     const len = keys.length;
     const output = new Array(len);
-    for (var i = 0; i < len; i++)
+    for (let i = 0; i < len; i++)
         output[i] = formatProperty(ctx, value, recurseTimes, keys[i], 0);
     return output;
 }
 
 // The array is sparse and/or has extra keys
 function formatSpecialArray(ctx, value, recurseTimes, keys, maxLength, valLen) {
     const output = [];
     const keyLen = keys.length;
-    var visibleLength = 0;
-    var i = 0;
+    let visibleLength = 0;
+    let i = 0;
     if (keyLen !== 0 && numberRegExp.test(keys[0])) {
         for (const key of keys) {
             if (visibleLength === maxLength)
                 break;
-            const index = +key;
+            const index = Number(key);
             // Arrays can only have up to 2^32 - 1 entries
             if (index > 2 ** 32 - 2)
                 break;
             if (i !== index) {
                 if (!numberRegExp.test(key))
                     break;
                 const emptyItems = index - i;
@@ -720,18 +723,18 @@
         keyLen > valLen && keys[valLen - 1] === `${valLen - 1}`) {
         // The array is not sparse
         for (i = valLen; i < keyLen; i++)
             output.push(formatProperty(ctx, value, recurseTimes, keys[i], 2));
     } else if (keys[keyLen - 1] !== `${valLen - 1}`) {
         const extra = [];
         // Only handle special keys
-        var key;
+        let key;
         for (i = keys.length - 1; i >= 0; i--) {
             key = keys[i];
-            if (numberRegExp.test(key) && +key < 2 ** 32 - 1)
+            if (numberRegExp.test(key) && Number(key) < 2 ** 32 - 1)
                 break;
             extra.push(formatProperty(ctx, value, recurseTimes, key, 2));
         }
         for (i = extra.length - 1; i >= 0; i--)
             output.push(extra[i]);
     }
     return output;
@@ -743,28 +746,30 @@
     const valLen = value.length;
     const keyLen = keys.length - hidden;
     if (keyLen !== valLen || keys[keyLen - 1] !== `${valLen - 1}`)
         return formatSpecialArray(ctx, value, recurseTimes, keys, len, valLen);
 
     const remaining = valLen - len;
     const output = new Array(len + (remaining > 0 ? 1 : 0) + hidden);
-    for (var i = 0; i < len; i++)
+    let i;
+    for (i = 0; i < len; i++)
         output[i] = formatProperty(ctx, value, recurseTimes, keys[i], 1);
     if (remaining > 0)
         output[i++] = `... ${remaining} more item${remaining > 1 ? 's' : ''}`;
     if (ctx.showHidden === true)
         output[i] = formatProperty(ctx, value, recurseTimes, 'length', 2);
     return output;
 }
 
 function formatTypedArray(ctx, value, recurseTimes, keys) {
     const maxLength = Math.min(Math.max(0, ctx.maxArrayLength), value.length);
     const remaining = value.length - maxLength;
     const output = new Array(maxLength + (remaining > 0 ? 1 : 0));
-    for (var i = 0; i < maxLength; ++i)
+    let i;
+    for (i = 0; i < maxLength; ++i)
         output[i] = formatNumber(ctx.stylize, value[i]);
     if (remaining > 0)
         output[i] = `... ${remaining} more item${remaining > 1 ? 's' : ''}`;
     if (ctx.showHidden) {
         // .buffer goes last, it's not a primitive like the others.
         const extraKeys = [
             'BYTES_PER_ELEMENT',
@@ -784,64 +789,65 @@
         output.push(formatProperty(ctx, value, recurseTimes, keys[i], 2));
     }
     return output;
 }
 
 function formatSet(ctx, value, recurseTimes, keys) {
     const output = new Array(value.size + keys.length + (ctx.showHidden ? 1 : 0));
-    var i = 0;
+    let i = 0;
     for (const v of value)
         output[i++] = formatValue(ctx, v, recurseTimes);
     // With `showHidden`, `length` will display as a hidden property for
     // arrays. For consistency's sake, do the same for `size`, even though this
     // property isn't selected by Object.getOwnPropertyNames().
     if (ctx.showHidden)
         output[i++] = `[size]: ${ctx.stylize(`${value.size}`, 'number')}`;
-    for (var n = 0; n < keys.length; n++) {
+    for (let n = 0; n < keys.length; n++) {
         output[i++] = formatProperty(ctx, value, recurseTimes, keys[n], 0);
     }
     return output;
 }
 
 function formatMap(ctx, value, recurseTimes, keys) {
     const output = new Array(value.size + keys.length + (ctx.showHidden ? 1 : 0));
-    var i = 0;
+    let i = 0;
     for (const [k, v] of value)
         output[i++] = `${formatValue(ctx, k, recurseTimes)} => ` +
         formatValue(ctx, v, recurseTimes);
     // See comment in formatSet
     if (ctx.showHidden)
         output[i++] = `[size]: ${ctx.stylize(`${value.size}`, 'number')}`;
-    for (var n = 0; n < keys.length; n++) {
+    for (let n = 0; n < keys.length; n++) {
         output[i++] = formatProperty(ctx, value, recurseTimes, keys[n], 0);
     }
     return output;
 }
 
 function formatPromise(ctx, value, recurseTimes, keys) {
-    var output;
+    let output;
     const [state, result] = getPromiseDetails(value);
     if (state === kPending) {
         output = ['<pending>'];
     } else {
         const str = formatValue(ctx, result, recurseTimes);
         output = [state === kRejected ? `<rejected> ${str}` : str];
     }
-    for (var n = 0; n < keys.length; n++) {
+    for (let n = 0; n < keys.length; n++) {
         output.push(formatProperty(ctx, value, recurseTimes, keys[n], 0));
     }
     return output;
 }
 
 function formatProperty(ctx, value, recurseTimes, key, array) {
-    var name, str;
-    const desc = Object.getOwnPropertyDescriptor(value, key) || {
-        value: value[key],
-        enumerable: true
-    };
+    let name, str;
+    const desc = Object.getOwnPropertyDescriptor(value, key) ||
+        {
+            value: value[key],
+            enumerable: true
+        };
     if (desc.value !== undefined) {
         const diff = array === 0 ? 3 : 2;
         ctx.indentationLvl += diff;
         str = formatValue(ctx, desc.value, recurseTimes, array === 0);
         ctx.indentationLvl -= diff;
     } else if (desc.get !== undefined) {
         if (desc.set !== undefined) {
@@ -869,16 +875,16 @@
 
     return `${name}: ${str}`;
 }
 
 function reduceToSingleString(ctx, output, base, braces, addLn) {
     const breakLength = ctx.breakLength;
     if (output.length * 2 <= breakLength) {
-        var length = 0;
-        for (var i = 0; i < output.length && length <= breakLength; i++) {
+        let length = 0;
+        for (let i = 0; i < output.length && length <= breakLength; i++) {
             if (ctx.colors) {
                 length += output[i].replace(colorRegExp, '').length + 1;
             } else {
                 length += output[i].length + 1;
             }
         }
         if (length <= breakLength) {
@@ -896,15 +902,15 @@
     const ln = base === '' && braces[0].length === 1 ?
         ' ' : `${base}\n${indentation}  `;
     const str = join(output, `,\n${indentation}  `);
 
     return `${extraLn}${braces[0]}${ln}${str} ${braces[1]}`;
 }
 
-/*!
+/* !
  * End of verbatim Node.js excerpt
  */
 
 module.exports = exports = {
     customInspectSymbol,
     format,
     inspect,
```

### Comparing `pythonmonkey-0.4.0/python/pythonmonkey/cli/pmjs.py` & `pythonmonkey-0.6.0/python/pythonmonkey/cli/pmjs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 #! /usr/bin/env python3
 # @file         pmjs - PythonMonkey REPL
 # @author       Wes Garland, wes@distributive.network
 # @date         June 2023
 # @copyright Copyright (c) 2023 Distributive Corp.
 
-import sys, os, signal, getopt
+import sys
+import os
+import signal
+import getopt
 import readline
 import asyncio
 import pythonmonkey as pm
 from pythonmonkey.lib import pmdb
 
 globalThis = pm.eval("globalThis")
-evalOpts = { 'filename': __file__, 'fromPythonFrame': True, 'strict': False } # type: pm.EvalOptions
+evalOpts = {'filename': __file__, 'fromPythonFrame': True, 'strict': False}  # type: pm.EvalOptions
 
 if (os.getenv('PMJS_PATH')):
-    requirePath = list(map(os.path.abspath, os.getenv('PMJS_PATH').split(',')))
+  requirePath = list(map(os.path.abspath, os.getenv('PMJS_PATH').split(',')))
 else:
-    requirePath = False;
+  requirePath = False
 
 pm.eval("""'use strict';
 const cmds = {};
 
 cmds.help = function help() {
   return '.' +
 `exit     Exit the REPL
@@ -140,150 +143,151 @@
   }
   catch(error)
   {
     globalThis._error = error;
     return util.inspect(error);
   }
 }
-""", evalOpts);
+""", evalOpts)
+
 
 async def repl():
+  """
+  Start a REPL to evaluate JavaScript code in the extra-module environment. Multi-line statements and
+  readline history are supported. ^C support is sketchy. Exit the REPL with ^D or ".quit".
+  """
+
+  print('Welcome to PythonMonkey v' + pm.__version__ + '.')
+  print('Type ".help" for more information.')
+  readline.parse_and_bind('set editing-mode emacs')
+  histfile = os.getenv('PMJS_REPL_HISTORY') or os.path.expanduser('~/.pmjs_history')
+  if (os.path.exists(histfile)):
+    try:
+      readline.read_history_file(histfile)
+    except BaseException:
+      pass
+
+  got_sigint = 0
+  statement = ''
+  readline_skip_chars = 0
+  inner_loop = False
+
+  def save_history():
+    nonlocal histfile
+    readline.write_history_file(histfile)
+
+  import atexit
+  atexit.register(save_history)
+
+  def quit():
     """
-    Start a REPL to evaluate JavaScript code in the extra-module environment. Multi-line statements and
-    readline history are supported. ^C support is sketchy. Exit the REPL with ^D or ".quit".
+    Quit the REPL. Repl saved by atexit handler.
     """
+    globalThis.python.exit()  # need for python.exit.code in require.py
 
-    print('Welcome to PythonMonkey v' + pm.__version__ +'.')
-    print('Type ".help" for more information.')
-    readline.parse_and_bind('set editing-mode emacs')
-    histfile = os.getenv('PMJS_REPL_HISTORY') or os.path.expanduser('~/.pmjs_history')
-    if (os.path.exists(histfile)):
-        try:
-            readline.read_history_file(histfile)
-        except:
-            pass
-
-    got_sigint = 0
-    statement = ''
-    readline_skip_chars = 0
-    inner_loop = False
-
-    def save_history():
-        nonlocal histfile
-        readline.write_history_file(histfile)
-
-    import atexit
-    atexit.register(save_history)
-
-    def quit():
-        """
-        Quit the REPL. Repl saved by atexit handler.
-        """
-        globalThis.python.exit(); # need for python.exit.code in require.py
-
-    def sigint_handler(signum, frame):
-        """
-        Handle ^C by aborting the entry of the current statement and quitting when double-struck.
-
-        Sometimes this happens in the main input() function. When that happens statement is "", because
-        we have not yet returned from input(). Sometimes it happens in the middle of the inner loop's
-        input() - in that case, statement is the beginning of a multiline expression. Hitting ^C in the
-        middle of a multiline express cancels its input, but readline's input() doesn't return, so we
-        have to print the extra > prompt and fake it by later getting rid of the first readline_skip_chars
-        characters from the input buffer.
-        """
-        nonlocal got_sigint
-        nonlocal statement
-        nonlocal readline_skip_chars
-        nonlocal inner_loop
-
-        got_sigint = got_sigint + 1
-        if (got_sigint > 1):
-            raise EOFError
-
-        if (inner_loop != True):
-            if (got_sigint == 1 and len(readline.get_line_buffer()) == readline_skip_chars):
-                # First ^C with nothing in the input buffer
-                sys.stdout.write("\n(To exit, press Ctrl+C again or Ctrl+D or type .exit)")
-            elif (got_sigint == 1 and readline.get_line_buffer() != ""):
-                # Input buffer has text - clear it
-                got_sigint = 0
-                readline_skip_chars = len(readline.get_line_buffer())
-        else:
-            if (got_sigint == 1 and statement == "" and len(readline.get_line_buffer()) == readline_skip_chars):
-                # statement == "" means that the inner loop has already seen ^C and is now faking the outer loop
-                sys.stdout.write("\n(To exit, press Ctrl+C again or Ctrl+D or type .exit)")
-            elif (got_sigint == 1 and statement != ""):
-                # ^C happened on inner loop while it was still thinking we were doing a multiline-expression; since
-                # we can't break the input() function, we set it up to return an outer expression and fake the outer loop
-                got_sigint = 0
-                readline_skip_chars = len(readline.get_line_buffer())
+  def sigint_handler(signum, frame):
+    """
+    Handle ^C by aborting the entry of the current statement and quitting when double-struck.
 
-        sys.stdout.write("\n> ")
+    Sometimes this happens in the main input() function. When that happens statement is "", because
+    we have not yet returned from input(). Sometimes it happens in the middle of the inner loop's
+    input() - in that case, statement is the beginning of a multiline expression. Hitting ^C in the
+    middle of a multiline express cancels its input, but readline's input() doesn't return, so we
+    have to print the extra > prompt and fake it by later getting rid of the first readline_skip_chars
+    characters from the input buffer.
+    """
+    nonlocal got_sigint
+    nonlocal statement
+    nonlocal readline_skip_chars
+    nonlocal inner_loop
+
+    got_sigint = got_sigint + 1
+    if (got_sigint > 1):
+      raise EOFError
+
+    if (not inner_loop):
+      if (got_sigint == 1 and len(readline.get_line_buffer()) == readline_skip_chars):
+        # First ^C with nothing in the input buffer
+        sys.stdout.write("\n(To exit, press Ctrl+C again or Ctrl+D or type .exit)")
+      elif (got_sigint == 1 and readline.get_line_buffer() != ""):
+        # Input buffer has text - clear it
+        got_sigint = 0
+        readline_skip_chars = len(readline.get_line_buffer())
+    else:
+      if (got_sigint == 1 and statement == "" and len(readline.get_line_buffer()) == readline_skip_chars):
+        # statement == "" means that the inner loop has already seen ^C and is now faking the outer loop
+        sys.stdout.write("\n(To exit, press Ctrl+C again or Ctrl+D or type .exit)")
+      elif (got_sigint == 1 and statement != ""):
+        # ^C happened on inner loop while it was still thinking we were doing a multiline-expression; since
+        # we can't break the input() function, we set it up to return an outer expression and fake the outer loop
+        got_sigint = 0
+        readline_skip_chars = len(readline.get_line_buffer())
+
+    sys.stdout.write("\n> ")
+    statement = ""
+  signal.signal(signal.SIGINT, sigint_handler)
+
+  # Main Loop
+  #
+  # Read lines entered by the user and collect them in a statement. Once the statement is a candiate
+  # for JavaScript evaluation (determined by pm.isCompilableUnit(), send it to replEval(). Statements
+  # beginning with a . are interpreted as REPL commands and sent to replCmd().
+  #
+  # Beware - extremely tricky interplay between readline and the SIGINT handler. This is largely because we
+  # we can't clear the pending line buffer, so we have to fake it by re-displaying the prompt and subtracting
+  # characters. Another complicating factor is that the handler will suspend and resume readline, but there
+  # is no mechanism to force readline to return before the user presses enter.
+  #
+  while got_sigint < 2:
+    try:
+      await asyncio.sleep(0)
+      inner_loop = False
+      if (statement == ""):
+        statement = input('> ')[readline_skip_chars:]
+      readline_skip_chars = 0
+
+      if (len(statement) == 0):
+        continue
+      if (statement[0] == '.'):
+        cmd_output = globalThis.replCmd(statement[1:])
+        if (cmd_output is not None):
+          print(cmd_output)
         statement = ""
-    signal.signal(signal.SIGINT, sigint_handler)
-
-    # Main Loop
-    #
-    # Read lines entered by the user and collect them in a statement. Once the statement is a candiate
-    # for JavaScript evaluation (determined by pm.isCompilableUnit(), send it to replEval(). Statements
-    # beginning with a . are interpreted as REPL commands and sent to replCmd().
-    #
-    # Beware - extremely tricky interplay between readline and the SIGINT handler. This is largely because we
-    # we can't clear the pending line buffer, so we have to fake it by re-displaying the prompt and subtracting
-    # characters. Another complicating factor is that the handler will suspend and resume readline, but there
-    # is no mechanism to force readline to return before the user presses enter.
-    #
-    while got_sigint < 2:
-        try:
-            await asyncio.sleep(0)
-            inner_loop = False
-            if (statement == ""):
-                statement = input('> ')[readline_skip_chars:]
-            readline_skip_chars = 0
-
-            if (len(statement) == 0):
-                continue
-            if (statement[0] == '.'):
-                cmd_output = globalThis.replCmd(statement[1:]);
-                if (cmd_output != None):
-                  print(cmd_output)
-                statement = ""
-                continue
-            if (pm.isCompilableUnit(statement)):
-                print(globalThis.replEval(statement))
-                statement = ""
-                got_sigint = 0
-            else:
-                got_sigint = 0
-                # This loop builds a multi-line statement, but if the user hits ^C during this build, we
-                # abort the statement. The tricky part here is that the input('... ') doesn't quit when
-                # SIGINT is received, so we have to patch things up so that the next-entered line is
-                # treated as the input at the top of the loop.
-                while (got_sigint == 0):
-                    await asyncio.sleep(0)
-                    inner_loop = True
-                    lineBuffer = input('... ')
-                    more = lineBuffer[readline_skip_chars:]
-                    readline_skip_chars = 0
-                    if (got_sigint > 0):
-                        statement = more
-                        break
-                    statement = statement + '\n' + more
-                    if (pm.isCompilableUnit(statement)):
-                        print(globalThis.replEval(statement))
-                        statement = ""
-                        break
-        except EOFError:
-            print()
-            quit()
+        continue
+      if (pm.isCompilableUnit(statement)):
+        print(globalThis.replEval(statement))
+        statement = ""
+        got_sigint = 0
+      else:
+        got_sigint = 0
+        # This loop builds a multi-line statement, but if the user hits ^C during this build, we
+        # abort the statement. The tricky part here is that the input('... ') doesn't quit when
+        # SIGINT is received, so we have to patch things up so that the next-entered line is
+        # treated as the input at the top of the loop.
+        while (got_sigint == 0):
+          await asyncio.sleep(0)
+          inner_loop = True
+          lineBuffer = input('... ')
+          more = lineBuffer[readline_skip_chars:]
+          readline_skip_chars = 0
+          if (got_sigint > 0):
+            statement = more
+            break
+          statement = statement + '\n' + more
+          if (pm.isCompilableUnit(statement)):
+            print(globalThis.replEval(statement))
+            statement = ""
+            break
+    except EOFError:
+      print()
+      quit()
 
 
 def usage():
-    print("""Usage: pmjs [options] [ script.js ] [arguments]
+  print("""Usage: pmjs [options] [ script.js ] [arguments]
 
 Options:
   -                    script read from stdin (default if no file name is provided, interactive mode if a tty)
   --                   indicate the end of node options
   -e, --eval=...       evaluate script
   -h, --help           print pnode command line options (currently set)
   -i, --interactive    always enter the REPL even if stdin does not appear to be a terminal
@@ -293,82 +297,96 @@
   --use-strict         evaluate -e, -p, and REPL code in strict mode
   --inspect            enable pmdb, a gdb-like JavaScript debugger interface
 
 Environment variables:
 TZ                            specify the timezone configuration
 PMJS_PATH                     ':'-separated list of directories prefixed to the module search path
 PMJS_REPL_HISTORY             path to the persistent REPL history file"""
-    )
+        )
+
 
 def initGlobalThis():
-    """
-    Initialize globalThis for pmjs use in the extra-module context (eg -r, -e, -p). This context
-    needs a require function which resolves modules relative to the current working directory at pmjs
-    launch. The global require is to the JS function using a trick instead of a JS-wrapped-Python-wrapped function
-    """
-    global requirePath
+  """
+  Initialize globalThis for pmjs use in the extra-module context (eg -r, -e, -p). This context
+  needs a require function which resolves modules relative to the current working directory at pmjs
+  launch. The global require is to the JS function using a trick instead of a JS-wrapped-Python-wrapped function
+  """
+  global requirePath
+
+  require = pm.createRequire(os.path.abspath(os.getcwd() + '/__pmjs_virtual__'), requirePath)
+  globalThis.require = require
+  globalInitModule = require(
+      os.path.realpath(
+          os.path.dirname(__file__) +
+          "/../lib/pmjs/global-init"))  # module load has side-effects
+  globalThis.arguments = sys.argv
+  return globalInitModule
 
-    require = pm.createRequire(os.path.abspath(os.getcwd() + '/__pmjs_virtual__'), requirePath)
-    globalThis.require = require
-    globalInitModule = require(os.path.realpath(os.path.dirname(__file__) + "/../lib/pmjs/global-init")) # module load has side-effects
-    globalThis.arguments = sys.argv
-    return globalInitModule
 
 def main():
-    """
-    Main program entry point
-    """
-    enterRepl = sys.stdin.isatty()
-    forceRepl = False
-    globalInitModule = initGlobalThis()
-    global requirePath
+  """
+  Main program entry point
+  """
+  enterRepl = sys.stdin.isatty()
+  forceRepl = False
+  globalInitModule = initGlobalThis()
+  global requirePath
+
+  try:
+    opts, args = getopt.getopt(sys.argv[1:], "hie:p:r:v", ["help", "eval=", "print=",
+                               "require=", "version", "interactive", "use-strict", "inspect"])
+  except getopt.GetoptError as err:
+    # print help information and exit:
+    print(err)  # will print something like "option -a not recognized"
+    usage()
+    sys.exit(2)
+  output = None
+  verbose = False
+  for o, a in opts:
+    if o in ("-v", "--version"):
+      print(pm.__version__)
+      sys.exit()
+    elif o in ("--use-strict"):
+      evalOpts['strict'] = True
+    elif o in ("-h", "--help"):
+      usage()
+      sys.exit()
+    elif o in ("-i", "--interactive"):
+      forceRepl = True
+    elif o in ("-e", "--eval"):
+      async def runEval():
+        pm.eval(a, evalOpts)
+        await pm.wait()
+      asyncio.run(runEval())
+      enterRepl = False
+    elif o in ("-p", "--print"):
+      async def runEvalPrint():
+        ret = pm.eval(a, evalOpts)
+        pm.eval("ret => console.log(ret)", evalOpts)(ret)
+        await pm.wait()
+      asyncio.run(runEvalPrint())
+      enterRepl = False
+    elif o in ("-r", "--require"):
+      globalThis.require(a)
+    elif o in ("--inspect"):
+      pmdb.enable()
+    else:
+      assert False, "unhandled option"
+
+  if (len(args) > 0):
+    async def runJS():
+      globalInitModule.patchGlobalRequire()
+      pm.runProgramModule(args[0], args, requirePath)
+      await pm.wait()  # blocks until all asynchronous calls finish
+    asyncio.run(runJS())
+  elif (enterRepl or forceRepl):
+    async def runREPL():
+      globalInitModule.initReplLibs()
+      await repl()
+      await pm.wait()
+    asyncio.run(runREPL())
 
-    try:
-        opts, args = getopt.getopt(sys.argv[1:], "hie:p:r:v", ["help", "eval=", "print=", "require=", "version", "interactive", "use-strict", "inspect"])
-    except getopt.GetoptError as err:
-        # print help information and exit:
-        print(err)  # will print something like "option -a not recognized"
-        usage()
-        sys.exit(2)
-    output = None
-    verbose = False
-    for o, a in opts:
-        if o in ("-v", "--version"):
-            print(pm.__version__)
-            sys.exit()
-        elif o in ("--use-strict"):
-            evalOpts['strict'] = True
-        elif o in ("-h", "--help"):
-            usage()
-            sys.exit()
-        elif o in ("-i", "--interactive"):
-            forceRepl = True
-        elif o in ("-e", "--eval"):
-            pm.eval(a, evalOpts)
-            enterRepl = False
-        elif o in ("-p", "--print"):
-            print(pm.eval(a, evalOpts))
-            enterRepl = False
-        elif o in ("-r", "--require"):
-            globalThis.require(a)
-        elif o in ("--inspect"):
-            pmdb.enable()
-        else:
-            assert False, "unhandled option"
-
-    if (len(args) > 0):
-        async def runJS():
-            globalInitModule.patchGlobalRequire()
-            pm.runProgramModule(args[0], args, requirePath)
-            await pm.wait() # blocks until all asynchronous calls finish
-        asyncio.run(runJS())
-    elif (enterRepl or forceRepl):
-        async def runREPL():
-            globalInitModule.initReplLibs()
-            await repl()
-            await pm.wait()
-        asyncio.run(runREPL())
+  globalThis.python.exit()  # need for python.exit.code in require.py
 
-    globalThis.python.exit(); # need for python.exit.code in require.py
 
 if __name__ == "__main__":
-    main()
+  main()
```

### Comparing `pythonmonkey-0.4.0/python/pythonmonkey/global.d.ts` & `pythonmonkey-0.6.0/python/pythonmonkey/global.d.ts`

 * *Files 5% similar despite different names*

```diff
@@ -52,14 +52,17 @@
 // Expose `atob`/`btoa` as properties of the global object
 declare var atob: typeof import("base64").atob;
 declare var btoa: typeof import("base64").btoa;
 
 // Expose `setTimeout`/`clearTimeout` APIs
 declare var setTimeout: typeof import("timers").setTimeout;
 declare var clearTimeout: typeof import("timers").clearTimeout;
+// Expose `setInterval`/`clearInterval` APIs
+declare var setInterval: typeof import("timers").setInterval;
+declare var clearInterval: typeof import("timers").clearInterval;
 
 // Expose `URL`/`URLSearchParams` APIs
 declare var URL: typeof import("url").URL;
 declare var URLSearchParams: typeof import("url").URLSearchParams;
 
 // Expose `XMLHttpRequest` (XHR) API
 declare var XMLHttpRequest: typeof import("XMLHttpRequest").XMLHttpRequest;
```

### Comparing `pythonmonkey-0.4.0/python/pythonmonkey/helpers.py` & `pythonmonkey-0.6.0/python/pythonmonkey/helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,57 +3,60 @@
 #               - new operator wrapper
 #
 # @author       Wes Garland, wes@distributive.network
 # @date         July 2023
 #
 # @copyright Copyright (c) 2023 Distributive Corp.
 
-from . import pythonmonkey as pm 
-evalOpts = { 'filename': __file__, 'fromPythonFrame': True }
+from . import pythonmonkey as pm
+evalOpts = {'filename': __file__, 'fromPythonFrame': True}
+
 
 def typeof(jsval):
-    """
-    typeof function - wraps JS typeof operator
-    """
-    return pm.eval("""'use strict'; (
-function pmTypeof(jsval) 
+  """
+  typeof function - wraps JS typeof operator
+  """
+  return pm.eval("""'use strict'; (
+function pmTypeof(jsval)
 {
   return typeof jsval;
 }
-    )""", evalOpts)(jsval);
+    )""", evalOpts)(jsval)
+
 
 def new(ctor):
-    """
-    new function - emits function which wraps JS new operator, emitting a lambda which constructs a new
-    JS object upon invocation.
-    """
-    if (typeof(ctor) == 'string'):
-        ctor = pm.eval(ctor)
+  """
+  new function - emits function which wraps JS new operator, emitting a lambda which constructs a new
+  JS object upon invocation.
+  """
+  if (typeof(ctor) == 'string'):
+    ctor = pm.eval(ctor)
 
-    newCtor = pm.eval("""'use strict'; (
+  newCtor = pm.eval("""'use strict'; (
 function pmNewFactory(ctor)
 {
   return function newCtor(args) {
     args = Array.from(args || []);
     return new ctor(...args);
   };
 }
     )""", evalOpts)(ctor)
-    return (lambda *args: newCtor(list(args)))
+  return (lambda *args: newCtor(list(args)))
+
 
 # List which symbols are exposed to the pythonmonkey module.
-__all__ = [ "new", "typeof" ]
+__all__ = ["new", "typeof"]
 
 # Add the non-enumerable properties of globalThis which don't collide with pythonmonkey.so as exports:
-globalThis = pm.eval('globalThis');
+globalThis = pm.eval('globalThis')
 pmGlobals = vars(pm)
 
 exports = pm.eval("""
 Object.getOwnPropertyNames(globalThis)
 .filter(prop => Object.keys(globalThis).indexOf(prop) === -1);
 """, evalOpts)
 
 for index in range(0, len(exports)):
-    name = exports[index]
-    if (pmGlobals.get(name) == None):
-        globals().update({name: globalThis[name]})
-        __all__.append(name)
+  name = exports[index]
+  if (pmGlobals.get(name) is None):
+    globals().update({name: globalThis[name]})
+    __all__.append(name)
```

### Comparing `pythonmonkey-0.4.0/python/pythonmonkey/lib/pmdb.py` & `pythonmonkey-0.6.0/python/pythonmonkey/lib/pmdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 # @file     pmdb - A gdb-like JavaScript debugger interface
 # @author   Tom Tang <xmader@distributive.network>
 # @date     July 2023
 # @copyright Copyright (c) 2023 Distributive Corp.
 
 import pythonmonkey as pm
 
+
 def debuggerInput(prompt: str):
   try:
-    return input(prompt) # blocking
+    return input(prompt)  # blocking
   except KeyboardInterrupt:
-    print("\b\bQuit") # to match the behaviour of gdb 
+    print("\b\bQuit")  # to match the behaviour of gdb
     return ""
   except Exception as e:
     print(e)
     return ""
 
-def enable(debuggerGlobalObject = pm.eval("debuggerGlobal")):
+
+def enable(debuggerGlobalObject=pm.eval("debuggerGlobal")):
   if debuggerGlobalObject._pmdbEnabled:
-    return # already enabled, skipping
+    return  # already enabled, skipping
 
   debuggerGlobalObject._pmdbEnabled = True
   debuggerGlobalObject.eval("""(debuggerInput, _pythonPrint, _pythonExit) => {
   const dbg = new Debugger()
   const mainDebuggee = dbg.addDebuggee(mainGlobal)
   dbg.uncaughtExceptionHook = (e) => {
     _pythonPrint(e)
@@ -36,40 +38,40 @@
     }
   }
 
   function print (...args) {
     const logger = makeDebuggeeValue(mainGlobal.console.log)
     logger.apply(logger, args.map(makeDebuggeeValue))
   }
-  
+
   function printErr (...args) {
     const logger = makeDebuggeeValue(mainGlobal.console.error)
     logger.apply(logger, args.map(makeDebuggeeValue))
   }
-  
+
   function printSource (frame, location) {
     const src = frame.script.source.text
     const line = src.split('\\n').slice(location.lineNumber-1, location.lineNumber).join('\\n')
     print(line)
     print(" ".repeat(location.columnNumber) + "^") // indicate column position
   }
-  
+
   function getCommandInputs () {
     const input = debuggerInput("(pmdb) > ") // blocking
     const [_, command, rest] = input.match(/\\s*(\\w+)?(?:\\s+(.*))?/)
     return { command, rest }
   }
 
   function enterDebuggerLoop (frame, checkIsBreakpoint = false) {
     const metadata = frame.script.getOffsetMetadata(frame.offset)
     if (checkIsBreakpoint && !metadata.isBreakpoint) {
       // This bytecode offset does not qualify as a breakpoint, skipping
       return
     }
-    
+
     blockingLoop: while (true) {
       const { command, rest } = getCommandInputs() // blocking
       switch (command) {
         case "b":
         case "break": {
           // Set breakpoint on specific line number
           const lineNum = Number(rest)
```

### Comparing `pythonmonkey-0.4.0/python/pythonmonkey/lib/pmjs/global-init.js` & `pythonmonkey-0.6.0/python/pythonmonkey/lib/pmjs/global-init.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -24,12 +24,12 @@
  *
  * This patch swaps in a descended version of require(), which has the same require.cache, but that has
  * side effects in terms of local module id resolution, so this patch happens only right before we want
  * to fire up the program module.
  */
 exports.patchGlobalRequire = function pmjs$$patchGlobalRequire() {
     globalThis.require = require;
-}
+};
 
 exports.initReplLibs = function pmjs$$initReplLibs() {
     globalThis.util = require('util');
-}
+};
```

### Comparing `pythonmonkey-0.4.0/python/pythonmonkey/pythonmonkey.pyi` & `pythonmonkey-0.6.0/python/pythonmonkey/pythonmonkey.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,72 +1,87 @@
 """
 @see https://typing.readthedocs.io/en/latest/source/stubs.html
 """
 
 import typing as _typing
 
+
 class EvalOptions(_typing.TypedDict, total=False):
-    filename: str
-    lineno: int
-    column: int
-    mutedErrors: bool
-    noScriptRval: bool
-    selfHosting: bool
-    strict: bool
-    module: bool
-    fromPythonFrame: bool
+  filename: str
+  lineno: int
+  column: int
+  mutedErrors: bool
+  noScriptRval: bool
+  selfHosting: bool
+  strict: bool
+  module: bool
+  fromPythonFrame: bool
 
 # pylint: disable=redefined-builtin
+
+
 def eval(code: str, evalOpts: EvalOptions = {}, /) -> _typing.Any:
-    """
-    JavaScript evaluator in Python
-    """
+  """
+  JavaScript evaluator in Python
+  """
+
 
 def wait() -> _typing.Awaitable[None]:
-    """
-    Block until all asynchronous jobs (Promise/setTimeout/etc.) finish.
-    
-    ```py
-    await pm.wait()
-    ```
+  """
+  Block until all asynchronous jobs (Promise/setTimeout/etc.) finish.
+
+  ```py
+  await pm.wait()
+  ```
+
+  This is the event-loop shield that protects the loop from being prematurely terminated.
+  """
 
-    This is the event-loop shield that protects the loop from being prematurely terminated.
-    """
 
 def isCompilableUnit(code: str) -> bool:
-    """
-    Hint if a string might be compilable Javascript without actual evaluation
-    """
+  """
+  Hint if a string might be compilable Javascript without actual evaluation
+  """
+
 
 def collect() -> None:
-    """
-    Calls the spidermonkey garbage collector
-    """
+  """
+  Calls the spidermonkey garbage collector
+  """
+
+
 class JSFunctionProxy():
   """
   JavaScript Function proxy
   """
+
+
 class JSMethodProxy(JSFunctionProxy, object):
+  """
+  JavaScript Method proxy
+  This constructs a callable object based on the first argument, bound to the second argument
+  Useful when you wish to implement a method on a class object with JavaScript
+  Example:
+  import pythonmonkey as pm
+
+  jsFunc = pm.eval("(function(value) { this.value = value})")
+  class Class:
+    def __init__(self):
+      self.value = 0
+      self.setValue = pm.JSMethodProxy(jsFunc, self) #setValue will be bound to self, so `this` will always be `self`
+
+  myObject = Class()
+  print(myObject.value) # 0
+  myObject.setValue(42)
+  print(myObject.value) # 42.0
+  """
+
+  def __init__(self) -> None:
     """
-    JavaScript Method proxy
-    This constructs a callable object based on the first argument, bound to the second argument
-    Useful when you wish to implement a method on a class object with JavaScript
-    Example:
-    import pythonmonkey as pm
-
-    jsFunc = pm.eval("(function(value) { this.value = value})")
-    class Class:
-      def __init__(self):
-        self.value = 0
-        self.setValue = pm.JSMethodProxy(jsFunc, self) #setValue will be bound to self, so `this` will always be `self`
-    
-    myObject = Class()
-    print(myObject.value) # 0
-    myObject.setValue(42)
-    print(myObject.value) # 42.0
+    PythonMonkey init function
     """
-    def __init__(self) -> None: ...
+
 
 null = _typing.Annotated[
     _typing.NewType("pythonmonkey.null", object),
     "Representing the JS null type in Python using a singleton object",
 ]
```

### Comparing `pythonmonkey-0.4.0/python/pythonmonkey/require.py` & `pythonmonkey-0.6.0/python/pythonmonkey/require.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,70 +35,75 @@
 #                 is, and has a higher precedence.
 #
 # @author       Wes Garland, wes@distributive.network
 # @date         May 2023
 #
 # @copyright Copyright (c) 2023-2024 Distributive Corp.
 
-import sys, os, io
+import sys
+import os
+import io
 from typing import Union, Dict, Literal, List
 import importlib
 import importlib.util
 from importlib import machinery
 import inspect
 import functools
 
-from . import pythonmonkey as pm 
+from . import pythonmonkey as pm
 
 node_modules = os.path.abspath(
   os.path.join(
-    importlib.util.find_spec("pminit").submodule_search_locations[0], # type: ignore
+    importlib.util.find_spec("pminit").submodule_search_locations[0],  # type: ignore
     "..",
     "pythonmonkey",
     "node_modules"
   )
 )
-evalOpts = { 'filename': __file__, 'fromPythonFrame': True } # type: pm.EvalOptions
+evalOpts = {'filename': __file__, 'fromPythonFrame': True}  # type: pm.EvalOptions
 
 # Force to use UTF-8 encoding
 # Windows may use other encodings / code pages that have many characters missing/unrepresentable
-if isinstance(sys.stdin,  io.TextIOWrapper): sys.stdin.reconfigure(encoding='utf-8')
-if isinstance(sys.stdout, io.TextIOWrapper): sys.stdout.reconfigure(encoding='utf-8')
-if isinstance(sys.stderr, io.TextIOWrapper): sys.stderr.reconfigure(encoding='utf-8')
+if isinstance(sys.stdin, io.TextIOWrapper):
+  sys.stdin.reconfigure(encoding='utf-8')
+if isinstance(sys.stdout, io.TextIOWrapper):
+  sys.stdout.reconfigure(encoding='utf-8')
+if isinstance(sys.stderr, io.TextIOWrapper):
+  sys.stderr.reconfigure(encoding='utf-8')
 
 # Add some python functions to the global python object for code in this file to use.
 globalThis = pm.eval("globalThis;", evalOpts)
-pm.eval("globalThis.python = { pythonMonkey: {}, stdout: {}, stderr: {} }", evalOpts);
+pm.eval("globalThis.python = { pythonMonkey: {}, stdout: {}, stderr: {} }", evalOpts)
 globalThis.pmEval = pm.eval
 globalThis.python.pythonMonkey.dir = os.path.dirname(__file__)
 globalThis.python.pythonMonkey.isCompilableUnit = pm.isCompilableUnit
 globalThis.python.pythonMonkey.nodeModules = node_modules
-globalThis.python.print  = print
+globalThis.python.print = print
 globalThis.python.stdout.write = lambda s: sys.stdout.write(s)
 globalThis.python.stderr.write = lambda s: sys.stderr.write(s)
 globalThis.python.stdout.read = lambda n: sys.stdout.read(n)
 globalThis.python.stderr.read = lambda n: sys.stderr.read(n)
 globalThis.python.eval = eval
 globalThis.python.exec = exec
 globalThis.python.getenv = os.getenv
-globalThis.python.paths  = sys.path
+globalThis.python.paths = sys.path
 
 globalThis.python.exit = pm.eval("""'use strict';
 (exit) => function pythonExitWrapper(exitCode) {
   if (typeof exitCode === 'undefined')
     exitCode = pythonExitWrapper.code;
   if (typeof exitCode == 'undefined')
     exitCode = 0n;
   if (typeof exitCode === 'number')
     exitCode = BigInt(Math.floor(exitCode));
   if (typeof exitCode !== 'bigint')
     exitCode = 1n;
   exit(exitCode);
 }
-""", evalOpts)(sys.exit);
+""", evalOpts)(sys.exit)
 
 # bootstrap is effectively a scoping object which keeps us from polluting the global JS scope.
 # The idea is that we hold a reference to the bootstrap object in Python-load, for use by the
 # innermost code in ctx-module, without forcing ourselves to expose this minimalist code to
 # userland-require
 bootstrap = pm.eval("""
 'use strict'; (function IIFE(python) {
@@ -198,99 +203,108 @@
 bootstrap.modules.fs = {
   constants: { S_IFDIR: 16384 },
   statSync: function statSync(filename) {
     const ret = bootstrap.modules.fs.statSync_inner(filename);
     if (ret)
       return ret;
 
-    const err = new Error('file not found: ' + filename); 
-    err.code='ENOENT'; 
+    const err = new Error('file not found: ' + filename);
+    err.code='ENOENT';
     throw err;
   },
 };
 
 /* Modules which will be available to all requires */
 bootstrap.builtinModules = { debug: bootstrap.modules.debug };
 
 return bootstrap;
 })(globalThis.python)""", evalOpts)
 
+
 def statSync_inner(filename: str) -> Union[Dict[str, int], bool]:
-    """
-    Inner function for statSync.
+  """
+  Inner function for statSync.
+
+  Returns:
+      Union[Dict[str, int], False]: The mode of the file or False if the file doesn't exist.
+  """
+  from os import stat
+  filename = os.path.normpath(filename)
+  if (os.path.exists(filename)):
+    sb = stat(filename)
+    return {'mode': sb.st_mode}
+  else:
+    return False
 
-    Returns:
-        Union[Dict[str, int], False]: The mode of the file or False if the file doesn't exist.
-    """
-    from os import stat
-    filename = os.path.normpath(filename)
-    if (os.path.exists(filename)):
-        sb = stat(filename)
-        return { 'mode': sb.st_mode }
-    else:
-        return False
 
 def readFileSync(filename, charset) -> str:
-    """
-    Utility function for reading files.
-    Returns:
-        str: The contents of the file
-    """
-    filename = os.path.normpath(filename)
-    with open(filename, "r", encoding=charset) as fileHnd:
-        return fileHnd.read()
+  """
+  Utility function for reading files.
+  Returns:
+      str: The contents of the file
+  """
+  filename = os.path.normpath(filename)
+  with open(filename, "r", encoding=charset) as fileHnd:
+    return fileHnd.read()
+
 
 def existsSync(filename: str) -> bool:
-    filename = os.path.normpath(filename)
-    return os.path.exists(filename)
+  filename = os.path.normpath(filename)
+  return os.path.exists(filename)
+
 
 bootstrap.modules.fs.statSync_inner = statSync_inner
-bootstrap.modules.fs.readFileSync   = readFileSync
-bootstrap.modules.fs.existsSync     = existsSync
+bootstrap.modules.fs.readFileSync = readFileSync
+bootstrap.modules.fs.existsSync = existsSync
 
 # Read ctx-module module from disk and invoke so that this file is the "main module" and ctx-module has
 # require and exports symbols injected from the bootstrap object above. Current PythonMonkey bugs
 # prevent us from injecting names properly so they are stolen from trail left behind in the global
 # scope until that can be fixed.
 #
 # lineno should be -5 but jsapi 102 uses unsigned line numbers, so we take the newlines out of the
 # wrapper prologue to make stack traces line up.
 with open(node_modules + "/ctx-module/ctx-module.js", "r") as ctxModuleSource:
-    initCtxModule = pm.eval("""'use strict';
+  initCtxModule = pm.eval("""'use strict';
 (function moduleWrapper_forCtxModule(require, exports)
 {
 """ + ctxModuleSource.read() + """
 })
-""", { 'filename': node_modules + "/ctx-module/ctx-module.js", 'lineno': 0 });
+""", {'filename': node_modules + "/ctx-module/ctx-module.js", 'lineno': 0})
 initCtxModule(bootstrap.require, bootstrap.modules['ctx-module'])
 
-def load(filename: str) -> Dict:  
-    """
-    Loads a python module using the importlib machinery sourcefileloader, prefills it with an exports object and returns the module.
-    If the module is already loaded, returns it.
-
-    Args:
-        filename (str): The filename of the python module to load.
-
-    Returns:
-        : The loaded python module
-    """
-
-    filename = os.path.normpath(filename)
-    name = os.path.basename(filename)
-    if name not in sys.modules:
-        sourceFileLoader = machinery.SourceFileLoader(name, filename)
-        spec: machinery.ModuleSpec = importlib.util.spec_from_loader(sourceFileLoader.name, sourceFileLoader) # type: ignore
-        module = importlib.util.module_from_spec(spec)
-        sys.modules[name] = module
-        module.exports = {} # type: ignore
-        spec.loader.exec_module(module) # type: ignore
-    else:
-        module = sys.modules[name]
-    return module.exports
+
+def load(filename: str) -> Dict:
+  """
+  Loads a python module using the importlib machinery sourcefileloader, prefills it with an exports object and returns
+  the module.
+  If the module is already loaded, returns it.
+
+  Args:
+      filename (str): The filename of the python module to load.
+
+  Returns:
+      : The loaded python module
+  """
+
+  filename = os.path.normpath(filename)
+  name = os.path.basename(filename)
+  if name not in sys.modules:
+    sourceFileLoader = machinery.SourceFileLoader(name, filename)
+    spec: machinery.ModuleSpec = importlib.util.spec_from_loader(
+      sourceFileLoader.name, sourceFileLoader)  # type: ignore
+    module = importlib.util.module_from_spec(spec)
+    sys.modules[name] = module
+    module.exports = {}  # type: ignore
+    spec.loader.exec_module(module)  # type: ignore
+  else:
+    module = sys.modules[name]
+  return module.exports
+
+
 globalThis.python.load = load
 
 createRequireInner = pm.eval("""'use strict';(
 /**
  * Factory function which returns a fresh 'require' function. The module cache will inherit from
  * globalThis.require, assuming it has been defined.
  *
@@ -352,59 +366,67 @@
     module.require.path.splice(module.require.path.length, 0, ...(extraPaths.split(',')));
 
   return module.require;
 })""", evalOpts)
 
 # API: pm.createRequire
 # We cache the return value of createRequire to always use the same require for the same filename
-def createRequire(filename, extraPaths: Union[List[str], Literal[False]] = False, isMain = False):
-    """
-    returns a require function that resolves modules relative to the filename argument. 
-    Conceptually the same as node:module.createRequire().
-
-    example:
-    from pythonmonkey import createRequire
-    require = createRequire(__file__)
-    require('./my-javascript-module')
-    """
-    fullFilename: str = os.path.abspath(filename)
-    if (extraPaths):
-        extraPathsStr = ':'.join(extraPaths)
-    else:
-        extraPathsStr = ''
-    return createRequireInner(fullFilename, bootstrap, extraPathsStr, isMain)
+
+
+def createRequire(filename, extraPaths: Union[List[str], Literal[False]] = False, isMain=False):
+  """
+  returns a require function that resolves modules relative to the filename argument.
+  Conceptually the same as node:module.createRequire().
+
+  example:
+  from pythonmonkey import createRequire
+  require = createRequire(__file__)
+  require('./my-javascript-module')
+  """
+  fullFilename: str = os.path.abspath(filename)
+  if (extraPaths):
+    extraPathsStr = ':'.join(extraPaths)
+  else:
+    extraPathsStr = ''
+  return createRequireInner(fullFilename, bootstrap, extraPathsStr, isMain)
+
 
 bootstrap.requireFromDisk = createRequireInner(None, bootstrap, '', False)
 bootstrap.inspect = bootstrap.requireFromDisk('util').inspect
 
 # API: pm.runProgramModule
+
+
 def runProgramModule(filename, argv, extraPaths=[]):
-    """
-    Run the program module. This loads the code from disk, sets up the execution environment, and then
-    invokes the program module (aka main module). The program module is different from other modules in that
-    1. it cannot return (must throw)
-    2. the outermost block scope is the global scope, effectively making its scope a super-global to
-       other modules
-    """
-    fullFilename = os.path.abspath(filename)
-    createRequire(fullFilename, extraPaths, True)
-    globalThis.__filename = fullFilename;
-    globalThis.__dirname = os.path.dirname(fullFilename);
-    with open(fullFilename, encoding="utf-8", mode="r") as mainModuleSource:
-        pm.eval(mainModuleSource.read(), {'filename': fullFilename})
+  """
+  Run the program module. This loads the code from disk, sets up the execution environment, and then
+  invokes the program module (aka main module). The program module is different from other modules in that
+  1. it cannot return (must throw)
+  2. the outermost block scope is the global scope, effectively making its scope a super-global to
+     other modules
+  """
+  fullFilename = os.path.abspath(filename)
+  createRequire(fullFilename, extraPaths, True)
+  globalThis.__filename = fullFilename
+  globalThis.__dirname = os.path.dirname(fullFilename)
+  with open(fullFilename, encoding="utf-8", mode="r") as mainModuleSource:
+    pm.eval(mainModuleSource.read(), {'filename': fullFilename})
 
 # The pythonmonkey require export. Every time it is used, the stack is inspected so that the filename
 # passed to createRequire is correct. This is necessary so that relative requires work. If the filename
 # found on the stack doesn't exist, we assume we're in the REPL or something and simply use the current
 # directory as the location of a virtual module for relative require purposes.
 #
 # todo: instead of cwd+__main_virtual__, use a full pathname which includes the directory that the
 #       running python program is in.
 #
+
+
 def require(moduleIdentifier: str):
-    filename = inspect.stack()[1].filename
-    if not os.path.exists(filename):
-      filename = os.path.join(os.getcwd(), "__main_virtual__")
-    return createRequire(filename)(moduleIdentifier)
+  filename = inspect.stack()[1].filename
+  if not os.path.exists(filename):
+    filename = os.path.join(os.getcwd(), "__main_virtual__")
+  return createRequire(filename)(moduleIdentifier)
+
 
 # Restrict what symbols are exposed to the pythonmonkey module.
 __all__ = ["globalThis", "require", "createRequire", "runProgramModule", "bootstrap"]
```

### Comparing `pythonmonkey-0.4.0/setup.sh` & `pythonmonkey-0.6.0/setup.sh`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 #!/bin/bash
 set -euo pipefail
 IFS=$'\n\t'
 
+# set git hooks
+ln -s -f ../../githooks/pre-commit .git/hooks/pre-commit
+# set blame ignore file
+git config blame.ignorerevsfile .git-blame-ignore-revs
 
 # Get number of CPU cores
 CPUS=$(getconf _NPROCESSORS_ONLN 2>/dev/null || getconf NPROCESSORS_ONLN 2>/dev/null || echo 1)
 
 echo "Installing dependencies"
 if [[ "$OSTYPE" == "linux-gnu"* ]]; then # Linux
   sudo apt-get update --yes
@@ -32,16 +36,33 @@
 curl -sSL https://install.python-poetry.org | python3 - --version "1.7.1"
 if [[ "$OSTYPE" == "msys"* ]]; then # Windows
   POETRY_BIN="$APPDATA/Python/Scripts/poetry"
 else
   POETRY_BIN=`echo ~/.local/bin/poetry` # expand tilde
 fi
 $POETRY_BIN self add 'poetry-dynamic-versioning[plugin]'
+poetry run pip install autopep8
 echo "Done installing dependencies"
 
+echo "Downloading uncrustify source code"
+wget -c -q https://github.com/uncrustify/uncrustify/archive/refs/tags/uncrustify-0.78.1.tar.gz
+mkdir -p uncrustify-source
+tar -xzvf uncrustify-0.78.1.tar.gz -C uncrustify-source --strip-components=1 # strip the root folder
+echo "Done downloading uncrustify source code"
+
+echo "Building uncrustify"
+cd uncrustify-source
+mkdir -p build
+cd build
+cmake ../
+make -j4
+cp uncrustify ../../uncrustify
+cd ../..
+echo "Done building uncrustify"
+
 echo "Downloading spidermonkey source code"
 wget -c -q https://ftp.mozilla.org/pub/firefox/releases/115.8.0esr/source/firefox-115.8.0esr.source.tar.xz
 mkdir -p firefox-source
 tar xf firefox-115.8.0esr.source.tar.xz -C firefox-source --strip-components=1 # strip the root folder
 echo "Done downloading spidermonkey source code"
 
 echo "Building spidermonkey"
@@ -73,8 +94,8 @@
 make install 
 if [[ "$OSTYPE" == "darwin"* ]]; then # macOS
   cd ../../../../_spidermonkey_install/lib/
   # Set the `install_name` field to use RPATH instead of an absolute path
   # overrides https://hg.mozilla.org/releases/mozilla-esr102/file/89d799cb/js/src/build/Makefile.in#l83
   install_name_tool -id @rpath/$(basename ./libmozjs*) ./libmozjs* # making it work for whatever name the libmozjs dylib is called
 fi
-echo "Done installing spidermonkey"
+echo "Done installing spidermonkey"
```

### Comparing `pythonmonkey-0.4.0/src/BufferType.cc` & `pythonmonkey-0.6.0/src/BufferType.cc`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 /**
  * @file BufferType.cc
- * @author Tom Tang (xmader@distributive.network)
+ * @author Tom Tang (xmader@distributive.network) and Philippe Laporte (philippe@distributive.network)
  * @brief Struct for representing ArrayBuffers
  * @date 2023-04-27
  *
- * @copyright Copyright (c) 2023 Distributive Corp.
+ * @copyright Copyright (c) 2023,2024 Distributive Corp.
  *
  */
 
 #include "include/BufferType.hh"
 
-#include "include/PyType.hh"
-#include "include/TypeEnum.hh"
 
 #include <jsapi.h>
 #include <js/ArrayBuffer.h>
 #include <js/experimental/TypedData.h>
 #include <js/ScalarType.h>
 
-#include <Python.h>
 
-BufferType::BufferType(PyObject *object) : PyType(object) {}
-
-BufferType::BufferType(JSContext *cx, JS::HandleObject bufObj) {
+PyObject *BufferType::getPyObject(JSContext *cx, JS::HandleObject bufObj) {
+  PyObject *pyObject;
   if (JS_IsTypedArrayObject(bufObj)) {
     pyObject = fromJsTypedArray(cx, bufObj);
   } else if (JS::IsArrayBufferObject(bufObj)) {
     pyObject = fromJsArrayBuffer(cx, bufObj);
   } else {
     // TODO (Tom Tang): Add support for JS [DataView](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/DataView)
     PyErr_SetString(PyExc_TypeError, "`bufObj` is neither a TypedArray object nor an ArraryBuffer object.");
     pyObject = nullptr;
   }
+
+  return pyObject;
 }
 
 /* static */
 bool BufferType::isSupportedJsTypes(JSObject *obj) {
   return JS::IsArrayBufferObject(obj) || JS_IsTypedArrayObject(obj);
 }
 
@@ -88,15 +86,17 @@
     .readonly = false,
     .ndim = 1 /* 1-dimensional array */,
     .format = (char *)"B" /* uint8 array */,
   };
   return PyMemoryView_FromBuffer(&bufInfo);
 }
 
-JSObject *BufferType::toJsTypedArray(JSContext *cx) {
+JSObject *BufferType::toJsTypedArray(JSContext *cx, PyObject *pyObject) {
+  Py_INCREF(pyObject);
+
   // Get the pyObject's underlying buffer pointer and size
   Py_buffer *view = new Py_buffer{};
   if (PyObject_GetBuffer(pyObject, view, PyBUF_ND | PyBUF_WRITABLE /* C-contiguous and writable */ | PyBUF_FORMAT) < 0) {
     // the buffer is immutable (e.g., Python `bytes` type is read-only)
     return nullptr; // raises a PyExc_BufferError
   }
   if (view->ndim != 1) {
@@ -206,17 +206,17 @@
     return "x"; // type code for pad bytes, no value
   }
 }
 
 JSObject *BufferType::_newTypedArrayWithBuffer(JSContext *cx, JS::Scalar::Type subtype, JS::HandleObject arrayBuffer) {
   switch (subtype) {
 #define NEW_TYPED_ARRAY_WITH_BUFFER(ExternalType, NativeType, Name) \
-case JS::Scalar::Name: \
-  return JS_New ## Name ## ArrayWithBuffer(cx, arrayBuffer, 0 /* byteOffset */, -1 /* use up the ArrayBuffer */);
+        case JS::Scalar::Name: \
+          return JS_New ## Name ## ArrayWithBuffer(cx, arrayBuffer, 0 /* byteOffset */, -1 /* use up the ArrayBuffer */);
 
-    JS_FOR_EACH_TYPED_ARRAY(NEW_TYPED_ARRAY_WITH_BUFFER)
+  JS_FOR_EACH_TYPED_ARRAY(NEW_TYPED_ARRAY_WITH_BUFFER)
 #undef NEW_TYPED_ARRAY_WITH_BUFFER
   default: // invalid
     PyErr_SetString(PyExc_TypeError, "Invalid Python buffer type.");
     return nullptr;
   }
-}
+}
```

### Comparing `pythonmonkey-0.4.0/src/CMakeLists.txt` & `pythonmonkey-0.6.0/src/CMakeLists.txt`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 list(APPEND PYTHONMONKEY_SOURCE_FILES ${SOURCE_FILES} "${CMAKE_SOURCE_DIR}/src/modules/pythonmonkey/pythonmonkey.cc")
 
 add_library(pythonmonkey SHARED
     ${PYTHONMONKEY_SOURCE_FILES}
 )
 
 target_include_directories(pythonmonkey PUBLIC ..)
+target_compile_definitions(pythonmonkey PRIVATE BUILD_TYPE="${PM_BUILD_TYPE} $<CONFIG>")
 
 if(WIN32)
   set_target_properties(
     pythonmonkey
     PROPERTIES
       PREFIX ""
       SUFFIX ".pyd"
```

### Comparing `pythonmonkey-0.4.0/src/DateType.cc` & `pythonmonkey-0.6.0/src/DateType.cc`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,25 @@
 /**
  * @file DateType.cc
- * @author Caleb Aikens (caleb@distributive.network)
+ * @author Caleb Aikens (caleb@distributive.network) and Philippe Laporte (philippe@distributive.network)
  * @brief Struct for representing python dates
  * @date 2022-12-21
  *
- * @copyright Copyright (c) 2022 Distributive Corp.
+ * @copyright Copyright (c) 2022,2024 Distributive Corp.
  *
  */
 
 #include "include/DateType.hh"
 
-#include "include/PyType.hh"
-#include "include/TypeEnum.hh"
-
 #include <jsapi.h>
 #include <js/Date.h>
 
-#include <Python.h>
 #include <datetime.h>
 
-DateType::DateType(PyObject *object) : PyType(object) {}
-
-DateType::DateType(JSContext *cx, JS::HandleObject dateObj) {
+PyObject *DateType::getPyObject(JSContext *cx, JS::HandleObject dateObj) {
   if (!PyDateTimeAPI) { PyDateTime_IMPORT; } // for PyDateTime_FromTimestamp
 
   JS::Rooted<JS::ValueArray<0>> args(cx);
   JS::Rooted<JS::Value> year(cx);
   JS::Rooted<JS::Value> month(cx);
   JS::Rooted<JS::Value> day(cx);
   JS::Rooted<JS::Value> hour(cx);
@@ -36,25 +30,27 @@
   JS_CallFunctionName(cx, dateObj, "getUTCMonth", args, &month);
   JS_CallFunctionName(cx, dateObj, "getUTCDate", args, &day);
   JS_CallFunctionName(cx, dateObj, "getUTCHours", args, &hour);
   JS_CallFunctionName(cx, dateObj, "getUTCMinutes", args, &minute);
   JS_CallFunctionName(cx, dateObj, "getUTCSeconds", args, &second);
   JS_CallFunctionName(cx, dateObj, "getUTCMilliseconds", args, &usecond);
 
-  pyObject = PyDateTimeAPI->DateTime_FromDateAndTime(
+  PyObject *pyObject = PyDateTimeAPI->DateTime_FromDateAndTime(
     year.toNumber(), month.toNumber() + 1, day.toNumber(),
     hour.toNumber(), minute.toNumber(), second.toNumber(),
     usecond.toNumber() * 1000,
     PyDateTime_TimeZone_UTC, // Make the resulting Python datetime object timezone-aware
                              // See https://docs.python.org/3/library/datetime.html#aware-and-naive-objects
     PyDateTimeAPI->DateTimeType
   );
   Py_INCREF(PyDateTime_TimeZone_UTC);
+
+  return pyObject;
 }
 
-JSObject *DateType::toJsDate(JSContext *cx) {
+JSObject *DateType::toJsDate(JSContext *cx, PyObject *pyObject) {
   // See https://docs.python.org/3/library/datetime.html#datetime.datetime.timestamp
   PyObject *timestamp = PyObject_CallMethod(pyObject, "timestamp", NULL); // the result is in seconds
   double milliseconds = PyFloat_AsDouble(timestamp) * 1000;
   Py_DECREF(timestamp);
   return JS::NewDateObject(cx, JS::TimeClip(milliseconds));
-}
+}
```

### Comparing `pythonmonkey-0.4.0/src/DictType.cc` & `pythonmonkey-0.6.0/src/DictType.cc`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,29 @@
 /**
  * @file DictType.cc
  * @author Caleb Aikens (caleb@distributive.network), Giovanni Tedesco (giovanni@distributive.network) and Philippe Laporte (philippe@distributive.network)
  * @brief Struct representing python dictionaries
  * @date 2022-08-10
  *
- * @copyright Copyright (c) 2022 Distributive Corp.
+ * @copyright Copyright (c) 2022,2024 Distributive Corp.
  *
  */
 
 
 #include "include/DictType.hh"
 
 #include "include/JSObjectProxy.hh"
-#include "include/PyType.hh"
 
-#include <jsfriendapi.h>
 #include <jsapi.h>
 
-#include <Python.h>
 
-
-DictType::DictType() {
-  this->pyObject = PyDict_New();
-}
-
-DictType::DictType(PyObject *object) : PyType(object) {}
-
-DictType::DictType(JSContext *cx, JS::Handle<JS::Value> jsObject) {
+PyObject *DictType::getPyObject(JSContext *cx, JS::Handle<JS::Value> jsObject) {
   JSObjectProxy *proxy = (JSObjectProxy *)PyObject_CallObject((PyObject *)&JSObjectProxyType, NULL);
   if (proxy != NULL) {
     JS::RootedObject obj(cx);
     JS_ValueToObject(cx, jsObject, &obj);
     proxy->jsObject = new JS::PersistentRootedObject(cx);
     proxy->jsObject->set(obj);
-    this->pyObject = (PyObject *)proxy;
+    return (PyObject *)proxy;
   }
+  return NULL;
 }
```

### Comparing `pythonmonkey-0.4.0/src/ExceptionType.cc` & `pythonmonkey-0.6.0/src/ExceptionType.cc`

 * *Files 3% similar despite different names*

```diff
@@ -13,34 +13,34 @@
 
 #include "include/ExceptionType.hh"
 #include "include/StrType.hh"
 
 #include <jsapi.h>
 #include <js/Exception.h>
 
-#include <Python.h>
 #include <frameobject.h>
 
 
 // TODO (Tom Tang): preserve the original Python exception object somewhere in the JS obj for lossless two-way conversion
 
-ExceptionType::ExceptionType(JSContext *cx, JS::HandleObject error) {
+PyObject *ExceptionType::getPyObject(JSContext *cx, JS::HandleObject error) {
   // Convert the JS Error object to a Python string
   JS::RootedValue errValue(cx, JS::ObjectValue(*error)); // err
   JS::RootedObject errStack(cx, JS::ExceptionStackOrNull(error)); // err.stack
   PyObject *errStr = getExceptionString(cx, JS::ExceptionStack(cx, errValue, errStack), true);
 
   // Construct a new SpiderMonkeyError python object
-  //    pyObject = SpiderMonkeyError(errStr)
   #if PY_VERSION_HEX >= 0x03090000
-  pyObject = PyObject_CallOneArg(SpiderMonkeyError, errStr); // _PyErr_CreateException, https://github.com/python/cpython/blob/3.9/Python/errors.c#L100
+  PyObject *pyObject = PyObject_CallOneArg(SpiderMonkeyError, errStr); // _PyErr_CreateException, https://github.com/python/cpython/blob/3.9/Python/errors.c#L100
   #else
-  pyObject = PyObject_CallFunction(SpiderMonkeyError, "O", errStr); // PyObject_CallOneArg is not available in Python < 3.9
+  PyObject *pyObject = PyObject_CallFunction(SpiderMonkeyError, "O", errStr); // PyObject_CallOneArg is not available in Python < 3.9
   #endif
   Py_XDECREF(errStr);
+
+  return pyObject;
 }
 
 
 // Generating trace information
 
 #define PyTraceBack_LIMIT 1000
 
@@ -76,28 +76,31 @@
   return err;
 }
 
 JSObject *ExceptionType::toJsError(JSContext *cx, PyObject *exceptionValue, PyObject *traceBack) {
   assert(exceptionValue != NULL);
 
   // Gather JS context
+  #pragma GCC diagnostic push
+  #pragma GCC diagnostic ignored "-Wformat-zero-length"
   JS_ReportErrorASCII(cx, ""); // throw JS error and gather all details
+  #pragma GCC diagnostic pop
 
   JS::ExceptionStack exceptionStack(cx);
   if (!JS::GetPendingExceptionStack(cx, &exceptionStack)) {
     return NULL;
   }
   JS_ClearPendingException(cx);
 
   std::stringstream stackStream;
   JS::RootedObject stackObj(cx, exceptionStack.stack());
   if (stackObj.get()) {
     JS::RootedString stackStr(cx);
     JS::BuildStackString(cx, nullptr, stackObj, &stackStr, 2, js::StackFormat::SpiderMonkey);
-    stackStream << "\nJS Stack Trace:\n" << StrType(cx, stackStr).getValue();
+    stackStream << "\nJS Stack Trace:\n" << StrType::getValue(cx, stackStr);
   }
 
 
   // Gather Python context
   PyObject *pyErrType = PyObject_Type(exceptionValue);
   const char *pyErrTypeName = _PyType_Name((PyTypeObject *)pyErrType);
```

### Comparing `pythonmonkey-0.4.0/src/IntType.cc` & `pythonmonkey-0.6.0/src/IntType.cc`

 * *Files 10% similar despite different names*

```diff
@@ -6,22 +6,18 @@
  *
  * @copyright Copyright (c) 2023 Distributive Corp.
  *
  */
 
 #include "include/modules/pythonmonkey/pythonmonkey.hh"
 #include "include/IntType.hh"
-#include "include/PyType.hh"
-#include "include/TypeEnum.hh"
 
 #include <jsapi.h>
 #include <js/BigInt.h>
 
-#include <Python.h>
-
 #include <vector>
 
 #define SIGN_BIT_MASK 0b1000 // https://hg.mozilla.org/releases/mozilla-esr102/file/tip/js/src/vm/BigIntType.h#l40
 #define CELL_HEADER_LENGTH 8 // https://hg.mozilla.org/releases/mozilla-esr102/file/tip/js/src/gc/Cell.h#l602
 
 #define JS_DIGIT_BIT JS_BITS_PER_WORD
 #define PY_DIGIT_BIT PYLONG_BITS_IN_DIGIT
@@ -68,19 +64,16 @@
 #else // Python version is less than 3.12
   // see https://github.com/python/cpython/blob/v3.9.16/Objects/longobject.c#L977
   Py_ssize_t pyDigitCount = Py_SIZE(op); // negative on negative numbers
   return pyDigitCount < 0;
 #endif
 }
 
-IntType::IntType(PyObject *object) : PyType(object) {}
-
-IntType::IntType(long n) : PyType(Py_BuildValue("i", n)) {}
 
-IntType::IntType(JSContext *cx, JS::BigInt *bigint) {
+PyObject *IntType::getPyObject(JSContext *cx, JS::BigInt *bigint) {
   // Get the sign bit
   bool isNegative = BigIntIsNegative(bigint);
 
   // Read the digits count in this JS BigInt
   //    see https://hg.mozilla.org/releases/mozilla-esr102/file/tip/js/src/vm/BigIntType.h#l48
   //        https://hg.mozilla.org/releases/mozilla-esr102/file/tip/js/src/gc/Cell.h#l623
   uint32_t jsDigitCount = ((uint32_t *)bigint)[1];
@@ -106,27 +99,29 @@
   const uint8_t *bytes = const_cast<const uint8_t *>((uint8_t *)jsDigits);
   PyObject *pyIntObj = _PyLong_FromByteArray(bytes, jsDigitCount * JS_DIGIT_BYTE, true, false);
 
   // Cast to a pythonmonkey.bigint to differentiate it from a normal Python int,
   //  allowing Py<->JS two-way BigInt conversion.
   // We don't do `Py_SET_TYPE` because `_PyLong_FromByteArray` may cache and reuse objects for small ints
   #if PY_VERSION_HEX >= 0x03090000
-  pyObject = PyObject_CallOneArg(PythonMonkey_BigInt, pyIntObj); // pyObject = pythonmonkey.bigint(pyIntObj)
+  PyObject *pyObject = PyObject_CallOneArg(getPythonMonkeyBigInt(), pyIntObj); // pyObject = pythonmonkey.bigint(pyIntObj)
   #else
-  pyObject = PyObject_CallFunction(PythonMonkey_BigInt, "O", pyIntObj); // PyObject_CallOneArg is not available in Python < 3.9
+  PyObject *pyObject = PyObject_CallFunction(getPythonMonkeyBigInt(), "O", pyIntObj); // PyObject_CallOneArg is not available in Python < 3.9
   #endif
   Py_DECREF(pyIntObj);
 
   // Set the sign bit
   if (isNegative) {
     PythonLong_SetSign((PyLongObject *)pyObject, -1);
   }
+
+  return pyObject;
 }
 
-JS::BigInt *IntType::toJsBigInt(JSContext *cx) {
+JS::BigInt *IntType::toJsBigInt(JSContext *cx, PyObject *pyObject) {
   // Figure out how many 64-bit "digits" we would have for JS BigInt
   //    see https://github.com/python/cpython/blob/3.9/Modules/_randommodule.c#L306
   size_t bitCount = _PyLong_NumBits(pyObject);
   if (bitCount == (size_t)-1 && PyErr_Occurred())
     return nullptr;
   uint32_t jsDigitCount = bitCount == 0 ? 1 : (bitCount - 1) / JS_DIGIT_BIT + 1;
   // Get the sign bit
@@ -171,8 +166,8 @@
 
     // Set the sign bit
     // https://hg.mozilla.org/releases/mozilla-esr102/file/tip/js/src/vm/BigIntType.cpp#l1801
     /* flagsField */ ((uint32_t *)bigint)[0] |= SIGN_BIT_MASK;
   }
 
   return bigint;
-}
+}
```

### Comparing `pythonmonkey-0.4.0/src/JSArrayIterProxy.cc` & `pythonmonkey-0.6.0/src/JSArrayIterProxy.cc`

 * *Files 6% similar despite different names*

```diff
@@ -30,14 +30,19 @@
 }
 
 int JSArrayIterProxyMethodDefinitions::JSArrayIterProxy_traverse(JSArrayIterProxy *self, visitproc visit, void *arg) {
   Py_VISIT(self->it.it_seq);
   return 0;
 }
 
+int JSArrayIterProxyMethodDefinitions::JSArrayIterProxy_clear(JSArrayIterProxy *self) {
+  Py_CLEAR(self->it.it_seq);
+  return 0;
+}
+
 PyObject *JSArrayIterProxyMethodDefinitions::JSArrayIterProxy_iter(JSArrayIterProxy *self) {
   Py_INCREF(&self->it);
   return (PyObject *)&self->it;
 }
 
 PyObject *JSArrayIterProxyMethodDefinitions::JSArrayIterProxy_next(JSArrayIterProxy *self) {
   PyListObject *seq = self->it.it_seq;
@@ -45,22 +50,22 @@
     return NULL;
   }
 
   if (self->it.reversed) {
     if (self->it.it_index >= 0) {
       JS::RootedValue elementVal(GLOBAL_CX);
       JS_GetElement(GLOBAL_CX, *(((JSArrayProxy *)seq)->jsArray), self->it.it_index--, &elementVal);
-      return pyTypeFactory(GLOBAL_CX, elementVal)->getPyObject();
+      return pyTypeFactory(GLOBAL_CX, elementVal);
     }
   }
   else {
     if (self->it.it_index < JSArrayProxyMethodDefinitions::JSArrayProxy_length((JSArrayProxy *)seq)) {
       JS::RootedValue elementVal(GLOBAL_CX);
       JS_GetElement(GLOBAL_CX, *(((JSArrayProxy *)seq)->jsArray), self->it.it_index++, &elementVal);
-      return pyTypeFactory(GLOBAL_CX, elementVal)->getPyObject();
+      return pyTypeFactory(GLOBAL_CX, elementVal);
     }
   }
 
   self->it.it_seq = NULL;
   Py_DECREF(seq);
   return NULL;
 }
```

### Comparing `pythonmonkey-0.4.0/src/JSArrayProxy.cc` & `pythonmonkey-0.6.0/src/JSArrayProxy.cc`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,28 @@
 #include <Python.h>
 
 
 void JSArrayProxyMethodDefinitions::JSArrayProxy_dealloc(JSArrayProxy *self)
 {
   self->jsArray->set(nullptr);
   delete self->jsArray;
-  Py_TYPE(self)->tp_free((PyObject *)self);
+  PyObject_GC_UnTrack(self);
+  PyObject_GC_Del(self);
+}
+
+int JSArrayProxyMethodDefinitions::JSArrayProxy_traverse(JSArrayProxy *self, visitproc visit, void *arg)
+{
+  // Nothing to be done
+  return 0;
+}
+
+int JSArrayProxyMethodDefinitions::JSArrayProxy_clear(JSArrayProxy *self)
+{
+  // Nothing to be done
+  return 0;
 }
 
 Py_ssize_t JSArrayProxyMethodDefinitions::JSArrayProxy_length(JSArrayProxy *self)
 {
   uint32_t length;
   JS::GetArrayLength(GLOBAL_CX, *(self->jsArray), &length);
   return (Py_ssize_t)length;
@@ -54,15 +67,15 @@
       JS::RootedValue value(GLOBAL_CX);
       JS_GetPropertyById(GLOBAL_CX, *(self->jsArray), id, &value);
       if (value.isUndefined() && PyUnicode_Check(key)) {
         if (strcmp("__class__", PyUnicode_AsUTF8(key)) == 0) {
           return PyObject_GenericGetAttr((PyObject *)self, key);
         }
       }
-      return pyTypeFactory(GLOBAL_CX, value)->getPyObject();
+      return pyTypeFactory(GLOBAL_CX, value);
     }
     else {
       if (strcmp(methodName, PyUnicode_AsUTF8(key)) == 0) {
         return PyObject_GenericGetAttr((PyObject *)self, key);
       }
     }
   }
@@ -75,15 +88,15 @@
   jArgs[0].setInt32(ilow);
   jArgs[1].setInt32(ihigh);
   JS::RootedValue jReturnedArray(GLOBAL_CX);
   if (!JS_CallFunctionName(GLOBAL_CX, *(self->jsArray), "slice", jArgs, &jReturnedArray)) {
     PyErr_Format(PyExc_SystemError, "%s JSAPI call failed", JSArrayProxyType.tp_name);
     return NULL;
   }
-  return pyTypeFactory(GLOBAL_CX, jReturnedArray)->getPyObject();
+  return pyTypeFactory(GLOBAL_CX, jReturnedArray);
 }
 
 PyObject *JSArrayProxyMethodDefinitions::JSArrayProxy_get_subscript(JSArrayProxy *self, PyObject *key)
 {
   if (PyIndex_Check(key)) {
     Py_ssize_t index = PyNumber_AsSsize_t(key, PyExc_IndexError);
     if (index == -1 && PyErr_Occurred()) {
@@ -103,15 +116,15 @@
 
     JS::RootedId id(GLOBAL_CX);
     JS_IndexToId(GLOBAL_CX, index, &id);
 
     JS::RootedValue value(GLOBAL_CX);
     JS_GetPropertyById(GLOBAL_CX, *(self->jsArray), id, &value);
 
-    return pyTypeFactory(GLOBAL_CX, value)->getPyObject();
+    return pyTypeFactory(GLOBAL_CX, value);
   }
   else if (PySlice_Check(key)) {
     Py_ssize_t start, stop, step, slicelength, index;
 
     if (PySlice_Unpack(key, &start, &stop, &step) < 0) {
       return NULL;
     }
@@ -132,15 +145,15 @@
         JS_GetElement(GLOBAL_CX, *(self->jsArray), cur, &elementVal);
         JS_SetElement(GLOBAL_CX, jCombinedArray, index, elementVal);
       }
 
       JS::RootedValue jCombinedArrayValue(GLOBAL_CX);
       jCombinedArrayValue.setObjectOrNull(jCombinedArray);
 
-      return pyTypeFactory(GLOBAL_CX, jCombinedArrayValue)->getPyObject();
+      return pyTypeFactory(GLOBAL_CX, jCombinedArrayValue);
     }
   }
   else {
     PyErr_Format(PyExc_TypeError, "list indices must be integers or slices, not %.200s", Py_TYPE(key)->tp_name);
     return NULL;
   }
 }
@@ -180,15 +193,14 @@
       }
       result = list_ass_slice(self, ilow, ihigh, v);
       Py_DECREF(v);
       return result;
     }
     v_as_SF = PySequence_Fast(v, "can only assign an iterable");
     if (v_as_SF == NULL) {
-      Py_XDECREF(v_as_SF);
       return result;
     }
     n = PySequence_Fast_GET_SIZE(v_as_SF);
     vitem = PySequence_Fast_ITEMS(v_as_SF);
   }
 
   if (ilow < 0) {
@@ -438,21 +450,25 @@
   JS::RootedValue elementVal(GLOBAL_CX);
 
   Py_ssize_t index;
   /* Search for the first index where items are different */
   for (index = 0; index < selfLength && index < otherLength; index++) {
     JS_GetElement(GLOBAL_CX, *(self->jsArray), index, &elementVal);
 
-    PyObject *leftItem = pyTypeFactory(GLOBAL_CX, elementVal)->getPyObject();
+    PyObject *leftItem = pyTypeFactory(GLOBAL_CX, elementVal);
     PyObject *rightItem;
+
+    bool needToDecRefRightItem;
     if (PyObject_TypeCheck(other, &JSArrayProxyType)) {
       JS_GetElement(GLOBAL_CX, *(((JSArrayProxy *)other)->jsArray), index, &elementVal);
-      rightItem = pyTypeFactory(GLOBAL_CX, elementVal)->getPyObject();
+      rightItem = pyTypeFactory(GLOBAL_CX, elementVal);
+      needToDecRefRightItem = true;
     } else {
       rightItem = ((PyListObject *)other)->ob_item[index];
+      needToDecRefRightItem = false;
     }
 
     if (leftItem == rightItem) {
       continue;
     }
 
     Py_INCREF(leftItem);
@@ -462,14 +478,19 @@
     Py_DECREF(rightItem);
     if (k < 0) {
       return NULL;
     }
     if (!k) {
       break;
     }
+
+    Py_DECREF(leftItem);
+    if (needToDecRefRightItem) {
+      Py_DECREF(rightItem);
+    }
   }
 
   if (index >= selfLength || index >= otherLength) {
     /* No more items to compare -- compare sizes */
     Py_RETURN_RICHCOMPARE(selfLength, otherLength, op);
   }
 
@@ -479,15 +500,18 @@
   }
   else if (op == Py_NE) {
     Py_RETURN_TRUE;
   }
 
   JS_GetElement(GLOBAL_CX, *(self->jsArray), index, &elementVal);
   /* Compare the final item again using the proper operator */
-  return PyObject_RichCompare(pyTypeFactory(GLOBAL_CX, elementVal)->getPyObject(), ((PyListObject *)other)->ob_item[index], op);
+  PyObject *pyElementVal = pyTypeFactory(GLOBAL_CX, elementVal);
+  PyObject *result = PyObject_RichCompare(pyElementVal, ((PyListObject *)other)->ob_item[index], op);
+  Py_DECREF(pyElementVal);
+  return result;
 }
 
 PyObject *JSArrayProxyMethodDefinitions::JSArrayProxy_repr(JSArrayProxy *self) {
   Py_ssize_t selfLength = JSArrayProxy_length(self);
 
   if (selfLength == 0) {
     return PyUnicode_FromString("[]");
@@ -521,15 +545,17 @@
 
     JS_GetElement(GLOBAL_CX, *(self->jsArray), index, &elementVal);
 
     PyObject *s;
     if (&elementVal.toObject() == (*(self->jsArray)).get()) {
       s = PyObject_Repr((PyObject *)self);
     } else {
-      s = PyObject_Repr(pyTypeFactory(GLOBAL_CX, elementVal)->getPyObject());
+      PyObject *pyElementVal = pyTypeFactory(GLOBAL_CX, elementVal);
+      s = PyObject_Repr(pyElementVal);
+      Py_DECREF(pyElementVal);
     }
     if (s == NULL) {
       goto error;
     }
 
     if (_PyUnicodeWriter_WriteStr(&writer, s) < 0) {
       Py_DECREF(s);
@@ -626,15 +652,15 @@
       JS_SetElement(GLOBAL_CX, jCombinedArray, sizeSelf + inputIdx, elementVal);
     }
   }
 
   JS::RootedValue jCombinedArrayValue(GLOBAL_CX);
   jCombinedArrayValue.setObjectOrNull(jCombinedArray);
 
-  return pyTypeFactory(GLOBAL_CX, jCombinedArrayValue)->getPyObject();
+  return pyTypeFactory(GLOBAL_CX, jCombinedArrayValue);
 }
 
 PyObject *JSArrayProxyMethodDefinitions::JSArrayProxy_repeat(JSArrayProxy *self, Py_ssize_t n) {
   const Py_ssize_t input_size = JSArrayProxy_length(self);
   if (input_size == 0 || n <= 0) {
     return PyList_New(0);
   }
@@ -653,30 +679,31 @@
       JS_SetElement(GLOBAL_CX, jCombinedArray, repeatIdx * input_size + inputIdx, elementVal);
     }
   }
 
   JS::RootedValue jCombinedArrayValue(GLOBAL_CX);
   jCombinedArrayValue.setObjectOrNull(jCombinedArray);
 
-  return pyTypeFactory(GLOBAL_CX, jCombinedArrayValue)->getPyObject();
+  return pyTypeFactory(GLOBAL_CX, jCombinedArrayValue);
 }
 
 int JSArrayProxyMethodDefinitions::JSArrayProxy_contains(JSArrayProxy *self, PyObject *element) {
   Py_ssize_t index;
   int cmp;
 
   Py_ssize_t numElements = JSArrayProxy_length(self);
 
   JS::RootedValue elementVal(GLOBAL_CX);
   for (index = 0, cmp = 0; cmp == 0 && index < numElements; ++index) {
     JS_GetElement(GLOBAL_CX, *(self->jsArray), index, &elementVal);
-    PyObject *item = pyTypeFactory(GLOBAL_CX, elementVal)->getPyObject();
+    PyObject *item = pyTypeFactory(GLOBAL_CX, elementVal);
     Py_INCREF(item);
     cmp = PyObject_RichCompareBool(item, element, Py_EQ);
     Py_DECREF(item);
+    Py_DECREF(item);
   }
   return cmp;
 }
 
 PyObject *JSArrayProxyMethodDefinitions::JSArrayProxy_inplace_concat(JSArrayProxy *self, PyObject *value) {
   Py_ssize_t selfLength = JSArrayProxy_length(self);
   Py_ssize_t valueLength = Py_SIZE(value);
@@ -740,15 +767,15 @@
   jArgs[0].setInt32(0);
   jArgs[1].setInt32(JSArrayProxy_length(self));
   JS::RootedValue jReturnedArray(GLOBAL_CX);
   if (!JS_CallFunctionName(GLOBAL_CX, *(self->jsArray), "slice", jArgs, &jReturnedArray)) {
     PyErr_Format(PyExc_SystemError, "%s JSAPI call failed", JSArrayProxyType.tp_name);
     return NULL;
   }
-  return pyTypeFactory(GLOBAL_CX, jReturnedArray)->getPyObject();
+  return pyTypeFactory(GLOBAL_CX, jReturnedArray);
 }
 
 PyObject *JSArrayProxyMethodDefinitions::JSArrayProxy_append(JSArrayProxy *self, PyObject *value) {
   Py_ssize_t len = JSArrayProxy_length(self);
 
   JS::SetArrayLength(GLOBAL_CX, *(self->jsArray), len + 1);
   JS::RootedValue jValue(GLOBAL_CX, jsTypeFactory(GLOBAL_CX, value));
@@ -917,27 +944,28 @@
   }
 
   // need the value in the returned array, not the array itself
   JS::RootedObject rootedReturnedArray(GLOBAL_CX, jReturnedArray.toObjectOrNull());
   JS::RootedValue elementVal(GLOBAL_CX);
   JS_GetElement(GLOBAL_CX, rootedReturnedArray, 0, &elementVal);
 
-  return pyTypeFactory(GLOBAL_CX, elementVal)->getPyObject();
+  return pyTypeFactory(GLOBAL_CX, elementVal);
 }
 
 PyObject *JSArrayProxyMethodDefinitions::JSArrayProxy_remove(JSArrayProxy *self, PyObject *value) {
   Py_ssize_t selfSize = JSArrayProxy_length(self);
 
   JS::RootedValue elementVal(GLOBAL_CX);
   for (Py_ssize_t index = 0; index < selfSize; index++) {
     JS_GetElement(GLOBAL_CX, *(self->jsArray), index, &elementVal);
-    PyObject *obj = pyTypeFactory(GLOBAL_CX, elementVal)->getPyObject();
+    PyObject *obj = pyTypeFactory(GLOBAL_CX, elementVal);
     Py_INCREF(obj);
     int cmp = PyObject_RichCompareBool(obj, value, Py_EQ);
     Py_DECREF(obj);
+    Py_DECREF(obj);
     if (cmp > 0) {
       JS::Rooted<JS::ValueArray<2>> jArgs(GLOBAL_CX);
       jArgs[0].setInt32(index);
       jArgs[1].setInt32(1);
       JS::RootedValue jReturnedArray(GLOBAL_CX);
       if (!JS_CallFunctionName(GLOBAL_CX, *(self->jsArray), "splice", jArgs, &jReturnedArray)) {
         PyErr_Format(PyExc_SystemError, "%s JSAPI call failed", JSArrayProxyType.tp_name);
@@ -991,18 +1019,19 @@
       stop = 0;
     }
   }
 
   JS::RootedValue elementVal(GLOBAL_CX);
   for (Py_ssize_t index = start; index < stop && index < selfSize; index++) {
     JS_GetElement(GLOBAL_CX, *(self->jsArray), index, &elementVal);
-    PyObject *obj = pyTypeFactory(GLOBAL_CX, elementVal)->getPyObject();
+    PyObject *obj = pyTypeFactory(GLOBAL_CX, elementVal);
     Py_INCREF(obj);
     int cmp = PyObject_RichCompareBool(obj, value, Py_EQ);
     Py_DECREF(obj);
+    Py_DECREF(obj);
     if (cmp > 0) {
       return PyLong_FromSsize_t(index);
     }
     else if (cmp < 0) {
       return NULL;
     }
   }
@@ -1014,18 +1043,19 @@
 PyObject *JSArrayProxyMethodDefinitions::JSArrayProxy_count(JSArrayProxy *self, PyObject *value) {
   Py_ssize_t count = 0;
 
   Py_ssize_t length = JSArrayProxy_length(self);
   JS::RootedValue elementVal(GLOBAL_CX);
   for (Py_ssize_t index = 0; index < length; index++) {
     JS_GetElement(GLOBAL_CX, *(self->jsArray), index, &elementVal);
-    PyObject *obj = pyTypeFactory(GLOBAL_CX, elementVal)->getPyObject();
+    PyObject *obj = pyTypeFactory(GLOBAL_CX, elementVal);
     Py_INCREF(obj);
     int cmp = PyObject_RichCompareBool(obj, value, Py_EQ);
     Py_DECREF(obj);
+    Py_DECREF(obj);
     if (cmp > 0) {
       count++;
     }
     else if (cmp < 0) {
       return NULL;
     }
   }
@@ -1061,23 +1091,25 @@
   if (!JS_GetProperty(cx, callee, "_reverse_param", &reverseValue)) {
     PyErr_Format(PyExc_SystemError, "%s JSAPI call failed", JSArrayProxyType.tp_name);
     return false;
   }
   bool reverse = reverseValue.toBoolean();
 
   JS::RootedValue elementVal0(cx, args[0]);
-  PyObject *args_0 = pyTypeFactory(cx, elementVal0)->getPyObject();
+  PyObject *args_0 = pyTypeFactory(cx, elementVal0);
   PyObject *args_0_result = PyObject_CallFunction(keyfunc, "O", args_0);
+  Py_DECREF(args_0);
   if (!args_0_result) {
     return false;
   }
 
   JS::RootedValue elementVal1(cx, args[1]);
-  PyObject *args_1 = pyTypeFactory(cx, elementVal1)->getPyObject();
+  PyObject *args_1 = pyTypeFactory(cx, elementVal1);
   PyObject *args_1_result = PyObject_CallFunction(keyfunc, "O", args_1);
+  Py_DECREF(args_1);
   if (!args_1_result) {
     return false;
   }
 
   int cmp = PyObject_RichCompareBool(args_0_result, args_1_result, Py_LT);
   if (cmp > 0) {
     args.rval().setInt32(reverse ? 1 : -1);
@@ -1109,39 +1141,45 @@
   if (!JS_GetProperty(cx, callee, "_reverse_param", &reverseValue)) {
     PyErr_Format(PyExc_SystemError, "%s JSAPI call failed", JSArrayProxyType.tp_name);
     return false;
   }
   bool reverse = reverseValue.toBoolean();
 
   JS::RootedValue elementVal0(cx, args[0]);
-  PyObject *args_0 = pyTypeFactory(cx, elementVal0)->getPyObject();
+  PyObject *args_0 = pyTypeFactory(cx, elementVal0);
 
   JS::RootedValue elementVal1(cx, args[1]);
-  PyObject *args_1 = pyTypeFactory(cx, elementVal1)->getPyObject();
+  PyObject *args_1 = pyTypeFactory(cx, elementVal1);
 
   int cmp = PyObject_RichCompareBool(args_0, args_1, Py_LT);
   if (cmp > 0) {
     args.rval().setInt32(reverse ? 1 : -1);
   }
   else if (cmp == 0) {
     cmp = PyObject_RichCompareBool(args_0, args_1, Py_EQ);
     if (cmp > 0) {
       args.rval().setInt32(0);
     }
     else if (cmp == 0) {
       args.rval().setInt32(reverse ? -1 : 1);
     }
     else {
+      Py_DECREF(args_0);
+      Py_DECREF(args_1);
       return false;
     }
   }
   else {
+    Py_DECREF(args_0);
+    Py_DECREF(args_1);
     return false;
   }
 
+  Py_DECREF(args_0);
+  Py_DECREF(args_1);
   return true;
 }
 
 PyObject *JSArrayProxyMethodDefinitions::JSArrayProxy_sort(JSArrayProxy *self, PyObject *const *args, Py_ssize_t nargs, PyObject *kwnames) {
   #if defined(Py_BUILD_CORE) && !defined(Py_BUILD_CORE_MODULE)
 
   #define NUM_KEYWORDS 2
```

### Comparing `pythonmonkey-0.4.0/src/JSFunctionProxy.cc` & `pythonmonkey-0.6.0/src/JSFunctionProxy.cc`

 * *Files 5% similar despite different names*

```diff
@@ -41,23 +41,27 @@
   JS::RootedVector<JS::Value> jsArgsVector(cx);
   Py_ssize_t nargs = PyTuple_Size(args);
   for (size_t i = 0; i < nargs; i++) {
     JS::Value jsValue = jsTypeFactory(cx, PyTuple_GetItem(args, i));
     if (PyErr_Occurred()) { // Check if an exception has already been set in the flow of control
       return NULL; // Fail-fast
     }
-    jsArgsVector.append(jsValue);
+    if (!jsArgsVector.append(jsValue)) {
+      // out of memory
+      setSpiderMonkeyException(cx);
+      return NULL;
+    }
   }
 
   JS::HandleValueArray jsArgs(jsArgsVector);
   JS::RootedValue jsReturnVal(cx);
   if (!JS_CallFunctionValue(cx, thisObj, jsFunc, jsArgs, &jsReturnVal)) {
     setSpiderMonkeyException(cx);
     return NULL;
   }
 
   if (PyErr_Occurred()) {
     return NULL;
   }
 
-  return pyTypeFactory(cx, jsReturnVal)->getPyObject();
+  return pyTypeFactory(cx, jsReturnVal);
 }
```

### Comparing `pythonmonkey-0.4.0/src/JSMethodProxy.cc` & `pythonmonkey-0.6.0/src/JSMethodProxy.cc`

 * *Files 6% similar despite different names*

```diff
@@ -52,23 +52,27 @@
 
   JS::RootedVector<JS::Value> jsArgsVector(cx);
   for (size_t i = 0; i < PyTuple_Size(args); i++) {
     JS::Value jsValue = jsTypeFactory(cx, PyTuple_GetItem(args, i));
     if (PyErr_Occurred()) { // Check if an exception has already been set in the flow of control
       return NULL; // Fail-fast
     }
-    jsArgsVector.append(jsValue);
+    if (!jsArgsVector.append(jsValue)) {
+      // out of memory
+      setSpiderMonkeyException(cx);
+      return NULL;
+    }
   }
 
   JS::HandleValueArray jsArgs(jsArgsVector);
   JS::RootedValue jsReturnVal(cx);
   if (!JS_CallFunctionValue(cx, selfObject, jsFunc, jsArgs, &jsReturnVal)) {
     setSpiderMonkeyException(cx);
     return NULL;
   }
 
   if (PyErr_Occurred()) {
     return NULL;
   }
 
-  return pyTypeFactory(cx, jsReturnVal)->getPyObject();
+  return pyTypeFactory(cx, jsReturnVal);
 }
```

### Comparing `pythonmonkey-0.4.0/src/JSObjectItemsProxy.cc` & `pythonmonkey-0.6.0/src/JSObjectItemsProxy.cc`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,19 @@
 }
 
 int JSObjectItemsProxyMethodDefinitions::JSObjectItemsProxy_traverse(JSObjectItemsProxy *self, visitproc visit, void *arg) {
   Py_VISIT(self->dv.dv_dict);
   return 0;
 }
 
+int JSObjectItemsProxyMethodDefinitions::JSObjectItemsProxy_clear(JSObjectItemsProxy *self) {
+  Py_CLEAR(self->dv.dv_dict);
+  return 0;
+}
+
 PyObject *JSObjectItemsProxyMethodDefinitions::JSObjectItemsProxy_iter(JSObjectItemsProxy *self) {
   JSObjectIterProxy *iterator = PyObject_GC_New(JSObjectIterProxy, &JSObjectIterProxyType);
   if (iterator == NULL) {
     return NULL;
   }
   iterator->it.reversed = false;
   iterator->it.it_index = 0;
```

### Comparing `pythonmonkey-0.4.0/src/JSObjectIterProxy.cc` & `pythonmonkey-0.6.0/src/JSObjectIterProxy.cc`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,19 @@
 }
 
 int JSObjectIterProxyMethodDefinitions::JSObjectIterProxy_traverse(JSObjectIterProxy *self, visitproc visit, void *arg) {
   Py_VISIT(self->it.di_dict);
   return 0;
 }
 
+int JSObjectIterProxyMethodDefinitions::JSObjectIterProxy_clear(JSObjectIterProxy *self) {
+  Py_CLEAR(self->it.di_dict);
+  return 0;
+}
+
 PyObject *JSObjectIterProxyMethodDefinitions::JSObjectIterProxy_iter(JSObjectIterProxy *self) {
   Py_INCREF(&self->it);
   return (PyObject *)&self->it;
 }
 
 PyObject *JSObjectIterProxyMethodDefinitions::JSObjectIterProxy_nextkey(JSObjectIterProxy *self) {
   PyDictObject *dict = self->it.di_dict;
@@ -55,53 +60,62 @@
       JS::HandleId id = (*(self->it.props))[(self->it.it_index)--];
       PyObject *key = idToKey(GLOBAL_CX, id);
       PyObject *value;
 
       if (self->it.kind != KIND_KEYS) {
         JS::RootedValue jsVal(GLOBAL_CX);
         JS_GetPropertyById(GLOBAL_CX, *(((JSObjectProxy *)(self->it.di_dict))->jsObject), id, &jsVal);
-        value = pyTypeFactory(GLOBAL_CX, jsVal)->getPyObject();
+        value = pyTypeFactory(GLOBAL_CX, jsVal);
       }
 
       PyObject *ret;
       if (self->it.kind == KIND_ITEMS) {
         ret = PyTuple_Pack(2, key, value);
       }
       else if (self->it.kind == KIND_VALUES) {
         ret = value;
       }
       else {
         ret = key;
       }
 
+      if (self->it.kind != KIND_KEYS) {
+        Py_DECREF(value);
+      }
+
       Py_INCREF(ret);
       return ret;
     }
   } else {
     if (self->it.it_index < JSObjectProxyMethodDefinitions::JSObjectProxy_length((JSObjectProxy *)dict)) {
       JS::HandleId id = (*(self->it.props))[(self->it.it_index)++];
       PyObject *key = idToKey(GLOBAL_CX, id);
       PyObject *value;
 
       if (self->it.kind != KIND_KEYS) {
         JS::RootedValue jsVal(GLOBAL_CX);
         JS_GetPropertyById(GLOBAL_CX, *(((JSObjectProxy *)(self->it.di_dict))->jsObject), id, &jsVal);
-        value = pyTypeFactory(GLOBAL_CX, jsVal)->getPyObject();
+        value = pyTypeFactory(GLOBAL_CX, jsVal);
       }
 
       PyObject *ret;
       if (self->it.kind == KIND_ITEMS) {
         ret = PyTuple_Pack(2, key, value);
       }
       else if (self->it.kind == KIND_VALUES) {
         ret = value;
       }
       else {
         ret = key;
       }
+
+      if (self->it.kind != KIND_KEYS) {
+        Py_DECREF(value);
+      }
+
       Py_INCREF(ret);
       return ret;
     }
   }
 
   self->it.di_dict = NULL;
   Py_DECREF(dict);
```

### Comparing `pythonmonkey-0.4.0/src/JSObjectKeysProxy.cc` & `pythonmonkey-0.6.0/src/JSObjectKeysProxy.cc`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,19 @@
 }
 
 int JSObjectKeysProxyMethodDefinitions::JSObjectKeysProxy_traverse(JSObjectKeysProxy *self, visitproc visit, void *arg) {
   Py_VISIT(self->dv.dv_dict);
   return 0;
 }
 
+int JSObjectKeysProxyMethodDefinitions::JSObjectKeysProxy_clear(JSObjectKeysProxy *self) {
+  Py_CLEAR(self->dv.dv_dict);
+  return 0;
+}
+
 // private
 static int all_contained_in(PyObject *self, PyObject *other) {
   PyObject *iter = PyObject_GetIter(self);
   int ok = 1;
 
   if (iter == NULL) {
     return -1;
```

### Comparing `pythonmonkey-0.4.0/src/JSObjectProxy.cc` & `pythonmonkey-0.6.0/src/JSObjectProxy.cc`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 #include "include/JSObjectItemsProxy.hh"
 
 #include "include/modules/pythonmonkey/pythonmonkey.hh"
 #include "include/jsTypeFactory.hh"
 #include "include/pyTypeFactory.hh"
 #include "include/PyBaseProxyHandler.hh"
 
+#include "include/JSFunctionProxy.hh"
+
 #include <jsapi.h>
 #include <jsfriendapi.h>
 
 #include <Python.h>
 
 #include <object.h>
 
@@ -45,15 +47,28 @@
   }
 }
 
 void JSObjectProxyMethodDefinitions::JSObjectProxy_dealloc(JSObjectProxy *self)
 {
   self->jsObject->set(nullptr);
   delete self->jsObject;
-  Py_TYPE(self)->tp_free((PyObject *)self);
+  PyObject_GC_UnTrack(self);
+  PyObject_GC_Del(self);
+}
+
+int JSObjectProxyMethodDefinitions::JSObjectProxy_traverse(JSObjectProxy *self, visitproc visit, void *arg)
+{
+  // Nothing to be done
+  return 0;
+}
+
+int JSObjectProxyMethodDefinitions::JSObjectProxy_clear(JSObjectProxy *self)
+{
+  // Nothing to be done
+  return 0;
 }
 
 Py_ssize_t JSObjectProxyMethodDefinitions::JSObjectProxy_length(JSObjectProxy *self)
 {
   JS::RootedIdVector props(GLOBAL_CX);
   if (!js::GetPropertyKeys(GLOBAL_CX, *(self->jsObject), JSITER_OWNONLY, &props))
   {
@@ -102,24 +117,24 @@
       }
       else if (value.isUndefined() && PyUnicode_Check(key)) {
         if (strcmp("__class__", PyUnicode_AsUTF8(key)) == 0) {
           return PyObject_GenericGetAttr((PyObject *)self, key);
         }
       }
 
-      return pyTypeFactory(GLOBAL_CX, value)->getPyObject();
+      return pyTypeFactory(GLOBAL_CX, value);
     }
     else {
       if (strcmp(methodName, PyUnicode_AsUTF8(key)) == 0) {
         if (checkPropertyShadowsMethod) {
           // just make sure no property is shadowing a method by name
           JS::RootedValue value(GLOBAL_CX);
           JS_GetPropertyById(GLOBAL_CX, *(self->jsObject), id, &value);
           if (!value.isUndefined()) {
-            return pyTypeFactory(GLOBAL_CX, value)->getPyObject();
+            return pyTypeFactory(GLOBAL_CX, value);
           }
         }
 
         return PyObject_GenericGetAttr((PyObject *)self, key);
       }
     }
   }
@@ -150,17 +165,17 @@
 int JSObjectProxyMethodDefinitions::JSObjectProxy_contains(JSObjectProxy *self, PyObject *key)
 {
   JS::RootedId id(GLOBAL_CX);
   if (!keyToId(key, &id)) {
     PyErr_SetString(PyExc_AttributeError, "JSObjectProxy property name must be of type str or int");
     return -1;
   }
-  JS::RootedValue *value = new JS::RootedValue(GLOBAL_CX);
-  JS_GetPropertyById(GLOBAL_CX, *(self->jsObject), id, value);
-  return value->isUndefined() ? 0 : 1;
+  JS::RootedValue value(GLOBAL_CX);
+  JS_GetPropertyById(GLOBAL_CX, *(self->jsObject), id, &value);
+  return value.isUndefined() ? 0 : 1;
 }
 
 static inline void assignKeyValue(JSObjectProxy *self, PyObject *key, JS::HandleId id, PyObject *value) {
   if (value) { // we are setting a value
     JS::RootedValue jValue(GLOBAL_CX, jsTypeFactory(GLOBAL_CX, value));
     JS_SetPropertyById(GLOBAL_CX, *(self->jsObject), id, jValue);
   } else { // we are deleting a value
@@ -237,17 +252,18 @@
   size_t length = props.length();
   for (size_t i = 0; i < length; i++)
   {
     JS::HandleId id = props[i];
     JS::RootedValue key(GLOBAL_CX);
     key.setString(id.toString());
 
-    PyObject *pyKey = pyTypeFactory(GLOBAL_CX, key)->getPyObject();
+    PyObject *pyKey = pyTypeFactory(GLOBAL_CX, key);
     PyObject *pyVal1 = PyObject_GetItem((PyObject *)self, pyKey);
     PyObject *pyVal2 = PyObject_GetItem((PyObject *)other, pyKey);
+    Py_DECREF(pyKey);
     if (!pyVal2) { // if other.key is NULL then not equal
       return false;
     }
     if (pyVal1 && Py_TYPE(pyVal1) == &JSObjectProxyType) { // if either subvalue is a JSObjectProxy, we need to pass around our visited map
       if (!JSObjectProxy_richcompare_helper((JSObjectProxy *)pyVal1, pyVal2, visited))
       {
         return false;
@@ -283,14 +299,48 @@
   if (!js::GetPropertyKeys(GLOBAL_CX, *(self->jsObject), JSITER_OWNONLY, iterator->it.props)) {
     return NULL;
   }
   PyObject_GC_Track(iterator);
   return (PyObject *)iterator;
 }
 
+PyObject *JSObjectProxyMethodDefinitions::JSObjectProxy_iter_next(JSObjectProxy *self) {
+  PyObject *key = PyUnicode_FromString("next");
+  JS::RootedId id(GLOBAL_CX);
+  if (!keyToId(key, &id)) {
+    PyErr_SetString(PyExc_SystemError, "JSObjectProxy failed type conversion");
+    return NULL;
+  }
+
+  PyObject *nextFunction = getKey(self, key, id, false);
+  Py_DECREF(key);
+  if (nextFunction == NULL) {
+    PyErr_SetString(PyExc_SystemError, "JSObjectProxy could not retrieve key");
+    return NULL;
+  }
+
+  PyObject *retVal = JSFunctionProxyMethodDefinitions::JSFunctionProxy_call(nextFunction, PyTuple_New(0), NULL);
+  Py_DECREF(nextFunction);
+
+  // check if end of iteration
+  key = PyUnicode_FromString("done");
+  PyObject *done = JSObjectProxy_get((JSObjectProxy *)retVal, key);
+  Py_DECREF(key);
+  if (done == Py_True) {
+    PyErr_SetNone(PyExc_StopIteration);
+    return NULL;
+  }
+
+  key = PyUnicode_FromString("value");
+  PyObject *value = JSObjectProxy_get((JSObjectProxy *)retVal, key);
+  Py_DECREF(key);
+
+  return value;
+}
+
 PyObject *JSObjectProxyMethodDefinitions::JSObjectProxy_repr(JSObjectProxy *self) {
   Py_ssize_t i = Py_ReprEnter((PyObject *)self);
   if (i != 0) {
     return i > 0 ? PyUnicode_FromString("{...}") : NULL;
   }
 
   Py_ssize_t selfLength = JSObjectProxy_length(self);
@@ -358,18 +408,18 @@
     }
 
     JS::RootedValue elementVal(GLOBAL_CX);
     JS_GetPropertyById(GLOBAL_CX, *(self->jsObject), id, &elementVal);
 
     if (&elementVal.toObject() == (*(self->jsObject)).get()) {
       value = (PyObject *)self;
+      Py_INCREF(value);
     } else {
-      value = pyTypeFactory(GLOBAL_CX, elementVal)->getPyObject();
+      value = pyTypeFactory(GLOBAL_CX, elementVal);
     }
-    Py_INCREF(value);
 
     s = PyObject_Repr(value);
     if (s == NULL) {
       goto error;
     }
 
     res = _PyUnicodeWriter_WriteStr(&writer, s);
@@ -503,15 +553,15 @@
     JS::RootedObject rootedObject(GLOBAL_CX, Object.toObjectOrNull());
     JS::RootedValue ret(GLOBAL_CX);
 
     if (!JS_CallFunctionName(GLOBAL_CX, rootedObject, "assign", args, &ret)) {
       PyErr_Format(PyExc_SystemError, "%s JSAPI call failed", JSObjectProxyType.tp_name);
       return NULL;
     }
-    return pyTypeFactory(GLOBAL_CX, ret)->getPyObject();
+    return pyTypeFactory(GLOBAL_CX, ret);
   }
 }
 
 PyObject *JSObjectProxyMethodDefinitions::JSObjectProxy_ior(JSObjectProxy *self, PyObject *other) {
   if (PyDict_Check(other)) {
     JS::Rooted<JS::ValueArray<2>> args(GLOBAL_CX);
     args[0].setObjectOrNull(*(self->jsObject));
@@ -630,15 +680,15 @@
     _PyErr_SetKeyError(key);
     return NULL;
   }
   else {
     JS::ObjectOpResult ignoredResult;
     JS_DeletePropertyById(GLOBAL_CX, *(self->jsObject), id, ignoredResult);
 
-    return pyTypeFactory(GLOBAL_CX, value)->getPyObject();
+    return pyTypeFactory(GLOBAL_CX, value);
   }
 }
 
 PyObject *JSObjectProxyMethodDefinitions::JSObjectProxy_clear_method(JSObjectProxy *self) {
   JS::RootedIdVector props(GLOBAL_CX);
   if (!js::GetPropertyKeys(GLOBAL_CX, *(self->jsObject), JSITER_OWNONLY, &props))
   {
@@ -671,15 +721,15 @@
 
   JS::RootedObject rootedObject(GLOBAL_CX, Object.toObjectOrNull());
   JS::RootedValue ret(GLOBAL_CX);
   if (!JS_CallFunctionName(GLOBAL_CX, rootedObject, "assign", args, &ret)) {
     PyErr_Format(PyExc_SystemError, "%s JSAPI call failed", JSObjectProxyType.tp_name);
     return NULL;
   }
-  return pyTypeFactory(GLOBAL_CX, ret)->getPyObject();
+  return pyTypeFactory(GLOBAL_CX, ret);
 }
 
 PyObject *JSObjectProxyMethodDefinitions::JSObjectProxy_update_method(JSObjectProxy *self, PyObject *args, PyObject *kwds) {
   PyObject *arg = NULL;
   int result = 0;
 
   if (!PyArg_UnpackTuple(args, "update", 0, 1, &arg)) {
```

### Comparing `pythonmonkey-0.4.0/src/JSObjectValuesProxy.cc` & `pythonmonkey-0.6.0/src/JSObjectValuesProxy.cc`

 * *Files 3% similar despite different names*

```diff
@@ -49,14 +49,19 @@
 }
 
 int JSObjectValuesProxyMethodDefinitions::JSObjectValuesProxy_traverse(JSObjectValuesProxy *self, visitproc visit, void *arg) {
   Py_VISIT(self->dv.dv_dict);
   return 0;
 }
 
+int JSObjectValuesProxyMethodDefinitions::JSObjectValuesProxy_clear(JSObjectValuesProxy *self) {
+  Py_CLEAR(self->dv.dv_dict);
+  return 0;
+}
+
 // private
 static int all_contained_in(PyObject *self, PyObject *other) {
   PyObject *iter = PyObject_GetIter(self);
   int ok = 1;
 
   if (iter == NULL) {
     return -1;
```

### Comparing `pythonmonkey-0.4.0/src/JobQueue.cc` & `pythonmonkey-0.6.0/src/JobQueue.cc`

 * *Files 2% similar despite different names*

```diff
@@ -17,40 +17,41 @@
 
 #include <jsfriendapi.h>
 #include <mozilla/Unused.h>
 
 #include <stdexcept>
 
 JobQueue::JobQueue(JSContext *cx) {
-  finalizationRegistryCallbacks = new JS::PersistentRooted<FunctionVector>(cx);
+  finalizationRegistryCallbacks = new JS::PersistentRooted<FunctionVector>(cx);   // Leaks but it's OK since freed at process exit
 }
 
 JSObject *JobQueue::getIncumbentGlobal(JSContext *cx) {
   return JS::CurrentGlobalOrNull(cx);
 }
 
 bool JobQueue::enqueuePromiseJob(JSContext *cx,
   [[maybe_unused]] JS::HandleObject promise,
   JS::HandleObject job,
   [[maybe_unused]] JS::HandleObject allocationSite,
   JS::HandleObject incumbentGlobal) {
 
   // Convert the `job` JS function to a Python function for event-loop callback
   JS::RootedValue jobv(cx, JS::ObjectValue(*job));
-  PyObject *callback = pyTypeFactory(cx, jobv)->getPyObject();
+  PyObject *callback = pyTypeFactory(cx, jobv);
 
   // Send job to the running Python event-loop
   PyEventLoop loop = PyEventLoop::getRunningLoop();
   if (!loop.initialized()) return false;
 
   // Inform the JS runtime that the job queue is no longer empty
   JS::JobQueueMayNotBeEmpty(cx);
 
   loop.enqueue(callback);
 
+  Py_DECREF(callback);
   return true;
 }
 
 void JobQueue::runJobs(JSContext *cx) {
   // Do nothing
 }
 
@@ -110,15 +111,15 @@
     PyGILState_Release(gstate);
     return false;
   }
   loop.enqueue(pyFunc);
 
   PyGILState_Release(gstate);
   return true;
-}  
+}
 
 void JobQueue::queueFinalizationRegistryCallback(JSFunction *callback) {
   mozilla::Unused << finalizationRegistryCallbacks->append(callback);
 }
 
 bool JobQueue::runFinalizationRegistryCallbacks(JSContext *cx) {
   bool ranCallbacks = false;
```

### Comparing `pythonmonkey-0.4.0/src/ListType.cc` & `pythonmonkey-0.6.0/src/ListType.cc`

 * *Files 22% similar despite different names*

```diff
@@ -6,25 +6,20 @@
  *
  * @copyright Copyright (c) 2022, 2023, 2024 Distributive Corp
  *
  */
 
 
 #include "include/ListType.hh"
-#include "include/PyType.hh"
-#include "include/JSArrayProxy.hh"
-
-#include <Python.h>
 
+#include "include/JSArrayProxy.hh"
 
-ListType::ListType() : PyType(PyList_New(0)) {}
-
-ListType::ListType(PyObject *object) : PyType(object) {}
 
-ListType::ListType(JSContext *cx, JS::HandleObject jsArrayObj) {
+PyObject *ListType::getPyObject(JSContext *cx, JS::HandleObject jsArrayObj) {
   JSArrayProxy *proxy = (JSArrayProxy *)PyObject_CallObject((PyObject *)&JSArrayProxyType, NULL);
   if (proxy != NULL) {
     proxy->jsArray = new JS::PersistentRootedObject(cx);
     proxy->jsArray->set(jsArrayObj);
-    this->pyObject = (PyObject *)proxy;
+    return (PyObject *)proxy;
   }
+  return NULL;
 }
```

### Comparing `pythonmonkey-0.4.0/src/PromiseType.cc` & `pythonmonkey-0.6.0/src/PromiseType.cc`

 * *Files 3% similar despite different names*

```diff
@@ -7,25 +7,21 @@
  * @copyright Copyright (c) 2023 Distributive Corp.
  *
  */
 
 #include "include/modules/pythonmonkey/pythonmonkey.hh"
 #include "include/PromiseType.hh"
 #include "include/PyEventLoop.hh"
-#include "include/PyType.hh"
-#include "include/TypeEnum.hh"
 #include "include/pyTypeFactory.hh"
 #include "include/jsTypeFactory.hh"
 
 #include <jsapi.h>
 #include <jsfriendapi.h>
 #include <js/Promise.h>
 
-#include <Python.h>
-
 // slot ids to access the python object in JS callbacks
 #define PY_FUTURE_OBJ_SLOT 0
 #define PROMISE_OBJ_SLOT 1
 
 static bool onResolvedCb(JSContext *cx, unsigned argc, JS::Value *vp) {
   JS::CallArgs args = JS::CallArgsFromVp(argc, vp);
 
@@ -33,24 +29,24 @@
   JS::Value promiseObjVal = js::GetFunctionNativeReserved(&args.callee(), PROMISE_OBJ_SLOT);
   JS::RootedObject promise(cx, &promiseObjVal.toObject());
   JS::PromiseState state = JS::GetPromiseState(promise);
 
   // Convert the Promise's result (either fulfilled resolution or rejection reason) to a Python object
   //  The result might be another JS function, so we must keep them alive
   JS::RootedValue resultArg(cx, args[0]);
-  PyObject *result = pyTypeFactory(cx, resultArg)->getPyObject();
+  PyObject *result = pyTypeFactory(cx, resultArg);
   if (state == JS::PromiseState::Rejected && !PyExceptionInstance_Check(result)) {
     // Wrap the result object into a SpiderMonkeyError object
     // because only *Exception objects can be thrown in Python `raise` statement and alike
     #if PY_VERSION_HEX >= 0x03090000
     PyObject *wrapped = PyObject_CallOneArg(SpiderMonkeyError, result); // wrapped = SpiderMonkeyError(result)
     #else
     PyObject *wrapped = PyObject_CallFunction(SpiderMonkeyError, "O", result); // PyObject_CallOneArg is not available in Python < 3.9
     #endif
-    Py_XDECREF(result);
+    Py_DECREF(result);
     result = wrapped;
   }
 
   // Get the `asyncio.Future` Python object from function's reserved slot
   JS::Value futureObjVal = js::GetFunctionNativeReserved(&args.callee(), PY_FUTURE_OBJ_SLOT);
   PyObject *futureObj = (PyObject *)(futureObjVal.toPrivate());
 
@@ -58,32 +54,31 @@
   PyEventLoop::Future future = PyEventLoop::Future(futureObj);
   if (state == JS::PromiseState::Fulfilled) {
     future.setResult(result);
   } else { // state == JS::PromiseState::Rejected
     future.setException(result);
   }
 
+  Py_DECREF(result);
   return true;
 }
 
-PromiseType::PromiseType(PyObject *object) : PyType(object) {}
-
-PromiseType::PromiseType(JSContext *cx, JS::HandleObject promise) {
+PyObject *PromiseType::getPyObject(JSContext *cx, JS::HandleObject promise) {
   // Create a python asyncio.Future on the running python event-loop
   PyEventLoop loop = PyEventLoop::getRunningLoop();
-  if (!loop.initialized()) return;
+  if (!loop.initialized()) return NULL;
   PyEventLoop::Future future = loop.createFuture();
 
   // Callbacks to settle the Python asyncio.Future once the JS Promise is resolved
   JS::RootedObject onResolved = JS::RootedObject(cx, (JSObject *)js::NewFunctionWithReserved(cx, onResolvedCb, 1, 0, NULL));
   js::SetFunctionNativeReserved(onResolved, PY_FUTURE_OBJ_SLOT, JS::PrivateValue(future.getFutureObject()));
   js::SetFunctionNativeReserved(onResolved, PROMISE_OBJ_SLOT, JS::ObjectValue(*promise));
   AddPromiseReactions(cx, promise, onResolved, onResolved);
 
-  pyObject = future.getFutureObject(); // must be a new reference
+  return future.getFutureObject(); // must be a new reference
 }
 
 // Callback to resolve or reject the JS Promise when the Future is done
 static PyObject *futureOnDoneCallback(PyObject *futureCallbackTuple, PyObject *args) {
   JSContext *cx = (JSContext *)PyLong_AsVoidPtr(PyTuple_GetItem(futureCallbackTuple, 0));
   JS::PersistentRootedObject *rootedPtr = (JS::PersistentRootedObject *)PyLong_AsVoidPtr(PyTuple_GetItem(futureCallbackTuple, 1));
   JS::HandleObject promise = *rootedPtr;
@@ -113,15 +108,15 @@
   delete rootedPtr; // no longer needed to be rooted, clean it up
 
   // Py_DECREF(futureObj) // would cause bug, because `Future` constructor didn't increase futureObj's ref count, but the destructor will decrease it
   Py_RETURN_NONE;
 }
 static PyMethodDef futureCallbackDef = {"futureOnDoneCallback", futureOnDoneCallback, METH_VARARGS, NULL};
 
-JSObject *PromiseType::toJsPromise(JSContext *cx) {
+JSObject *PromiseType::toJsPromise(JSContext *cx, PyObject *pyObject) {
   // Create a new JS Promise object
   JSObject *promise = JS::NewPromiseObject(cx, nullptr);
 
   // Convert the python awaitable to an asyncio.Future object
   PyEventLoop loop = PyEventLoop::getRunningLoop();
   if (!loop.initialized()) return nullptr;
   PyEventLoop::Future future = loop.ensureFuture(pyObject);
@@ -129,17 +124,17 @@
   PyEventLoop::_locker->incCounter();
 
   // Resolve or Reject the JS Promise once the python awaitable is done
   JS::PersistentRooted<JSObject *> *rootedPtr = new JS::PersistentRooted<JSObject *>(cx, promise); // `promise` is required to be rooted from here to the end of onDoneCallback
   PyObject *futureCallbackTuple = PyTuple_Pack(2, PyLong_FromVoidPtr(cx), PyLong_FromVoidPtr(rootedPtr));
   PyObject *onDoneCb = PyCFunction_New(&futureCallbackDef, futureCallbackTuple);
   future.addDoneCallback(onDoneCb);
-
+  Py_INCREF(pyObject);
   return promise;
 }
 
 bool PythonAwaitable_Check(PyObject *obj) {
   // see https://docs.python.org/3/c-api/typeobj.html#c.PyAsyncMethods
   PyTypeObject *tp = Py_TYPE(obj);
   bool isAwaitable = tp->tp_as_async != NULL && tp->tp_as_async->am_await != NULL;
   return isAwaitable;
-}
+}
```

### Comparing `pythonmonkey-0.4.0/src/PyBaseProxyHandler.cc` & `pythonmonkey-0.6.0/src/PyBaseProxyHandler.cc`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.4.0/src/PyDictProxyHandler.cc` & `pythonmonkey-0.6.0/src/PyDictProxyHandler.cc`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 /**
  * @file PyDictProxyHandler.cc
  * @author Caleb Aikens (caleb@distributive.network) and Philippe Laporte (philippe@distributive.network)
- * @brief Struct for creating JS proxy objects. Used by DictType for object coercion TODO
+ * @brief Struct for creating JS proxy objects for Dicts
  * @date 2023-04-20
  *
  * @copyright Copyright (c) 2023-2024 Distributive Corp.
  *
  */
 
 #include "include/PyDictProxyHandler.hh"
 
 #include "include/jsTypeFactory.hh"
 #include "include/pyTypeFactory.hh"
-#include "include/StrType.hh"
 
 #include <jsapi.h>
 #include <jsfriendapi.h>
 #include <js/Conversions.h>
 #include <js/Proxy.h>
 #include <js/Symbol.h>
 #include <js/friend/ErrorMessages.h>
@@ -65,17 +64,20 @@
 bool PyDictProxyHandler::set(JSContext *cx, JS::HandleObject proxy, JS::HandleId id,
   JS::HandleValue v, JS::HandleValue receiver,
   JS::ObjectOpResult &result) const {
   JS::RootedValue rootedV(cx, v);
   PyObject *attrName = idToKey(cx, id);
 
   PyObject *self = JS::GetMaybePtrFromReservedSlot<PyObject>(proxy, PyObjectSlot);
-  if (PyDict_SetItem(self, attrName, pyTypeFactory(cx, rootedV)->getPyObject())) {
+  PyObject *value = pyTypeFactory(cx, rootedV);
+  if (PyDict_SetItem(self, attrName, value)) {
+    Py_DECREF(value);
     return result.failCantSetInterposed(); // raises JS exception
   }
+  Py_DECREF(value);
   return result.succeed();
 }
 
 bool PyDictProxyHandler::enumerate(JSContext *cx, JS::HandleObject proxy,
   JS::MutableHandleIdVector props) const {
   return this->ownPropertyKeys(cx, proxy, props);
 }
```

### Comparing `pythonmonkey-0.4.0/src/PyEventLoop.cc` & `pythonmonkey-0.6.0/src/PyEventLoop.cc`

 * *Files 17% similar despite different names*

```diff
@@ -24,53 +24,78 @@
     return NULL;
   } else {
     Py_RETURN_NONE;
   }
 }
 static PyMethodDef loopJobWrapperDef = {"eventLoopJobWrapper", eventLoopJobWrapper, METH_NOARGS, NULL};
 
+static PyObject *_enqueueWithDelay(PyObject *_loop, PyEventLoop::AsyncHandle::id_t handleId, PyObject *jobFn, double delaySeconds, bool repeat);
+
 /**
  * @brief Wrapper to remove the reference of the timer after the job finishes
  */
-static PyObject *timerJobWrapper(PyObject *jobFn, PyObject *handlerPtr) {
-  auto handle = (PyEventLoop::AsyncHandle *)PyLong_AsVoidPtr(handlerPtr);
+static PyObject *timerJobWrapper(PyObject *jobFn, PyObject *args) {
+  PyObject *_loop = PyTuple_GetItem(args, 0);
+  PyEventLoop::AsyncHandle::id_t handleId = PyLong_AsLong(PyTuple_GetItem(args, 1));
+  double delaySeconds = PyFloat_AsDouble(PyTuple_GetItem(args, 2));
+  bool repeat = (bool)PyLong_AsLong(PyTuple_GetItem(args, 3));
+  auto handle = PyEventLoop::AsyncHandle::fromId(handleId);
+
   PyObject *ret = PyObject_CallObject(jobFn, NULL); // jobFn()
   Py_XDECREF(ret); // don't care about its return value
-  handle->removeRef();
-  if (PyErr_Occurred()) {
+
+  PyObject *errType, *errValue, *traceback; // we can't call any Python code unless the error indicator is clear
+  PyErr_Fetch(&errType, &errValue, &traceback);
+  if (repeat && !handle->cancelled()) {
+    _enqueueWithDelay(_loop, handleId, jobFn, delaySeconds, repeat);
+  } else {
+    handle->removeRef();
+  }
+
+  if (errType != NULL) { // PyErr_Occurred()
+    PyErr_Restore(errType, errValue, traceback);
     return NULL;
   } else {
     Py_RETURN_NONE;
   }
 }
-static PyMethodDef timerJobWrapperDef = {"timerJobWrapper", timerJobWrapper, METH_O, NULL};
+static PyMethodDef timerJobWrapperDef = {"timerJobWrapper", timerJobWrapper, METH_VARARGS, NULL};
 
 PyEventLoop::AsyncHandle PyEventLoop::enqueue(PyObject *jobFn) {
   PyEventLoop::_locker->incCounter();
   PyObject *wrapper = PyCFunction_New(&loopJobWrapperDef, jobFn);
   // Enqueue job to the Python event-loop
   //    https://docs.python.org/3/library/asyncio-eventloop.html#asyncio.loop.call_soon
   PyObject *asyncHandle = PyObject_CallMethod(_loop, "call_soon_threadsafe", "O", wrapper);
   return PyEventLoop::AsyncHandle(asyncHandle);
 }
 
-PyEventLoop::AsyncHandle::id_ptr_pair PyEventLoop::enqueueWithDelay(PyObject *jobFn, double delaySeconds) {
-  auto handler = PyEventLoop::AsyncHandle::newEmpty();
+static PyObject *_enqueueWithDelay(PyObject *_loop, PyEventLoop::AsyncHandle::id_t handleId, PyObject *jobFn, double delaySeconds, bool repeat) {
   PyObject *wrapper = PyCFunction_New(&timerJobWrapperDef, jobFn);
-  PyObject *handlerPtr = PyLong_FromVoidPtr(handler.second);
   // Schedule job to the Python event-loop
   //    https://docs.python.org/3/library/asyncio-eventloop.html#asyncio.loop.call_later
-  PyObject *asyncHandle = PyObject_CallMethod(_loop, "call_later", "dOO", delaySeconds, wrapper, handlerPtr); // https://docs.python.org/3/c-api/arg.html#c.Py_BuildValue
-  if (asyncHandle == nullptr) {
+  PyObject *asyncHandle = PyObject_CallMethod(_loop, "call_later", "dOOIdb", delaySeconds, wrapper, _loop, handleId, delaySeconds, repeat); // https://docs.python.org/3/c-api/arg.html#c.Py_BuildValue
+  if (!asyncHandle) {
+    return nullptr; // RuntimeError
+  }
+
+  auto handle = PyEventLoop::AsyncHandle::fromId(handleId);
+  Py_XDECREF(handle->swap(asyncHandle));
+
+  return asyncHandle;
+}
+
+PyEventLoop::AsyncHandle::id_t PyEventLoop::enqueueWithDelay(PyObject *jobFn, double delaySeconds, bool repeat) {
+  auto handleId = PyEventLoop::AsyncHandle::newEmpty();
+  if (!_enqueueWithDelay(_loop, handleId, jobFn, delaySeconds, repeat)) {
     PyErr_Print(); // RuntimeError: Non-thread-safe operation invoked on an event loop other than the current one
-    return handler;
   }
-  handler.second->swap(asyncHandle);
-  handler.second->addRef();
-  return handler;
+  auto handle = PyEventLoop::AsyncHandle::fromId(handleId);
+  handle->addRef();
+  return handleId;
 }
 
 PyEventLoop::Future PyEventLoop::createFuture() {
   //    https://docs.python.org/3/library/asyncio-eventloop.html#asyncio.loop.create_future
   PyObject *futureObj = PyObject_CallMethod(_loop, "create_future", NULL);
   return PyEventLoop::Future(futureObj);
 }
@@ -168,27 +193,39 @@
 
 /* static */
 PyEventLoop PyEventLoop::getRunningLoop() {
   return _getLoopOnThread(_getCurrentThread());
 }
 
 void PyEventLoop::AsyncHandle::cancel() {
-  PyObject *scheduled = PyObject_GetAttrString(_handle, "_scheduled"); // this attribute only exists on asyncio.TimerHandle returned by loop.call_later
-                                                                       // NULL if no such attribute (on a strict asyncio.Handle returned by loop.call_soon)
-  bool finishedOrCanceled = scheduled && scheduled == Py_False; // the job function has already been executed or canceled
-  if (!finishedOrCanceled) {
+  if (!_finishedOrCancelled()) {
     removeRef(); // automatically unref at finish
   }
-  Py_XDECREF(scheduled);
 
   // https://docs.python.org/3/library/asyncio-eventloop.html#asyncio.Handle.cancel
   PyObject *ret = PyObject_CallMethod(_handle, "cancel", NULL); // returns None
   Py_XDECREF(ret);
 }
 
+bool PyEventLoop::AsyncHandle::cancelled() {
+  // https://docs.python.org/3/library/asyncio-eventloop.html#asyncio.Handle.cancelled
+  PyObject *ret = PyObject_CallMethod(_handle, "cancelled", NULL); // returns Python bool
+  bool cancelled = ret == Py_True;
+  Py_XDECREF(ret);
+  return cancelled;
+}
+
+bool PyEventLoop::AsyncHandle::_finishedOrCancelled() {
+  PyObject *scheduled = PyObject_GetAttrString(_handle, "_scheduled"); // this attribute only exists on asyncio.TimerHandle returned by loop.call_later
+                                                                       // NULL if no such attribute (on a strict asyncio.Handle returned by loop.call_soon)
+  bool notScheduled = scheduled && scheduled == Py_False; // not scheduled means the job function has already been executed or canceled
+  Py_XDECREF(scheduled);
+  return notScheduled;
+}
+
 void PyEventLoop::Future::setResult(PyObject *result) {
   // https://docs.python.org/3/library/asyncio-future.html#asyncio.Future.set_result
   PyObject *ret = PyObject_CallMethod(_future, "set_result", "O", result); // returns None
   Py_XDECREF(ret);
 }
 
 void PyEventLoop::Future::setException(PyObject *exception) {
```

### Comparing `pythonmonkey-0.4.0/src/PyListProxyHandler.cc` & `pythonmonkey-0.6.0/src/PyListProxyHandler.cc`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 /**
  * @file PyListProxyHandler.cc
  * @author Philippe Laporte (philippe@distributive.network)
- * @brief Struct for creating JS proxy objects. Used by ListType for List coercion
+ * @brief Struct for creating JS proxy objects for Lists
  * @date 2023-12-01
  *
  * @copyright Copyright (c) 2023-2024 Distributive Corp.
  *
  */
 
 #include "include/PyListProxyHandler.hh"
 #include "include/PyBaseProxyHandler.hh"
 
 #include "include/jsTypeFactory.hh"
 #include "include/JSArrayProxy.hh"
 #include "include/JSFunctionProxy.hh"
 #include "include/pyTypeFactory.hh"
-#include "include/StrType.hh"
 
 #include <jsapi.h>
 #include <jsfriendapi.h>
 #include <js/Conversions.h>
 #include <js/Proxy.h>
 #include <js/Symbol.h>
 #include <js/friend/ErrorMessages.h>
@@ -42,16 +41,17 @@
     PyErr_Format(PyExc_TypeError, "unbound python functions do not have a 'self' to bind");
     return false;
   }
 
   PyObject *func = PyMethod_Function(method);
   JS::RootedValue thisValue(cx);
   thisValue.setObject(*thisObject);
-  PyObject *newSelf = pyTypeFactory(cx, thisValue)->getPyObject();
+  PyObject *newSelf = pyTypeFactory(cx, thisValue);
   function.set(jsTypeFactory(cx, PyMethod_New(func, newSelf)));
+  Py_DECREF(newSelf);
 
   return true;
 }
 
 static bool array_reverse(JSContext *cx, unsigned argc, JS::Value *vp) {
   JS::CallArgs args = JS::CallArgsFromVp(argc, vp);
 
@@ -108,17 +108,20 @@
   }
   PyObject *self = JS::GetMaybePtrFromReservedSlot<PyObject>(proxy, PyObjectSlot);
 
   unsigned numArgs = args.length();
   JS::RootedValue elementVal(cx);
   for (unsigned index = 0; index < numArgs; index++) {
     elementVal.set(args[index].get());
-    if (PyList_Append(self, pyTypeFactory(cx, elementVal)->getPyObject()) < 0) {
+    PyObject *value = pyTypeFactory(cx, elementVal);
+    if (PyList_Append(self, value) < 0) {
+      Py_DECREF(value);
       return false;
     }
+    Py_DECREF(value);
   }
 
   args.rval().setInt32(PyList_GET_SIZE(self));
   return true;
 }
 
 static bool array_shift(JSContext *cx, unsigned argc, JS::Value *vp) {
@@ -157,17 +160,20 @@
     return false;
   }
   PyObject *self = JS::GetMaybePtrFromReservedSlot<PyObject>(proxy, PyObjectSlot);
 
   JS::RootedValue elementVal(cx);
   for (int index = args.length() - 1; index >= 0; index--) {
     elementVal.set(args[index].get());
-    if (PyList_Insert(self, 0, pyTypeFactory(cx, elementVal)->getPyObject()) < 0) {
+    PyObject *value = pyTypeFactory(cx, elementVal);
+    if (PyList_Insert(self, 0, value) < 0) {
+      Py_DECREF(value);
       return false;
     }
+    Py_DECREF(value);
   }
 
   args.rval().setInt32(PyList_GET_SIZE(self));
   return true;
 }
 
 // private util
@@ -269,15 +275,17 @@
       if (d >= 0) {
         start = d;
       }
     }
   }
 
   JS::RootedValue elementVal(cx, args[0].get());
-  PyObject *result = PyObject_CallMethod(self, "index", "Oi", pyTypeFactory(cx, elementVal)->getPyObject(), start);
+  PyObject *value = pyTypeFactory(cx, elementVal);
+  PyObject *result = PyObject_CallMethod(self, "index", "Oi", value, start);
+  Py_DECREF(value);
 
   if (!result) {
     PyErr_Clear();
     args.rval().setInt32(-1);
     return true;
   }
 
@@ -350,15 +358,16 @@
   if (!inserted) {
     return false;
   }
 
   JS::RootedValue elementVal(cx);
   for (int index = 0; index < insertCount; index++) {
     elementVal.set(args[index + 2].get());
-    if (PyList_SetItem(inserted, index, pyTypeFactory(cx, elementVal)->getPyObject()) < 0) {
+    PyObject *value = pyTypeFactory(cx, elementVal);
+    if (PyList_SetItem(inserted, index, value) < 0) {
       return false;
     }
   }
 
   if (PyList_SetSlice(self, actualStart, actualStart + actualDeleteCount, inserted) < 0) {
     return false;
   }
@@ -414,21 +423,27 @@
   if (relativeEnd < 0) {
     actualEnd = uint64_t(std::max(double(selfLength) + relativeEnd, 0.0));
   } else {
     actualEnd = uint64_t(std::min(double(relativeEnd), double(selfLength)));
   }
 
   JS::RootedValue fillValue(cx, args[0].get());
-  PyObject *fillValueItem = pyTypeFactory(cx, fillValue)->getPyObject();
+  PyObject *fillValueItem = pyTypeFactory(cx, fillValue);
+  bool setItemCalled = false;
   for (int index = actualStart; index < actualEnd; index++) {
+    setItemCalled = true;
     if (PyList_SetItem(self, index, fillValueItem) < 0) {
       return false;
     }
   }
 
+  if (!setItemCalled) {
+    Py_DECREF(fillValueItem);
+  }
+
   // return ref to self
   args.rval().set(jsTypeFactory(cx, self));
   return true;
 }
 
 static bool array_copyWithin(JSContext *cx, unsigned argc, JS::Value *vp) {
   JS::CallArgs args = JS::CallArgsFromVp(argc, vp);
@@ -543,41 +558,53 @@
   }
 
   unsigned numArgs = args.length();
   JS::RootedValue elementVal(cx);
   for (unsigned index = 0; index < numArgs; index++) {
     elementVal.set(args[index].get());
 
-    PyObject *item = pyTypeFactory(cx, elementVal)->getPyObject();
+    PyObject *item = pyTypeFactory(cx, elementVal);
     if (PyObject_TypeCheck(item, &JSArrayProxyType)) {
       // flatten the array only a depth 1
       Py_ssize_t itemLength = JSArrayProxyMethodDefinitions::JSArrayProxy_length((JSArrayProxy *)item);
       for (Py_ssize_t flatIndex = 0; flatIndex < itemLength; flatIndex++) {
         if (!JS_GetElement(cx, *(((JSArrayProxy *)item)->jsArray), flatIndex, &elementVal)) {
+          Py_DECREF(item);
           return false;
         }
-        if (PyList_Append(result, pyTypeFactory(cx, elementVal)->getPyObject()) < 0) {
+        PyObject *value = pyTypeFactory(cx, elementVal);
+        if (PyList_Append(result, value) < 0) {
+          Py_DECREF(item);
+          Py_DECREF(value);
           return false;
         }
+        Py_DECREF(value);
       }
     }
     else if (PyObject_TypeCheck(item, &PyList_Type)) {
       // flatten the array only at depth 1
       Py_ssize_t itemLength = PyList_GET_SIZE(item);
       for (Py_ssize_t flatIndex = 0; flatIndex < itemLength; flatIndex++) {
         if (PyList_Append(result, PyList_GetItem(item, flatIndex)) < 0) {
+          Py_DECREF(item);
           return false;
         }
       }
     }
     else {
-      if (PyList_Append(result, pyTypeFactory(cx, elementVal)->getPyObject()) < 0) {
+      PyObject *value = pyTypeFactory(cx, elementVal);
+      if (PyList_Append(result, value) < 0) {
+        Py_DECREF(item);
+        Py_DECREF(value);
         return false;
       }
+      Py_DECREF(value);
     }
+
+    Py_DECREF(item);
   }
 
   args.rval().set(jsTypeFactory(cx, result));
   Py_DECREF(result);
   return true;
 }
 
@@ -617,28 +644,31 @@
       start = uint64_t(d);
     } else if (n < double(start)) {
       start = uint64_t(n);
     }
   }
 
   JS::RootedValue elementVal(cx, args[0].get());
-  PyObject *element = pyTypeFactory(cx, elementVal)->getPyObject();
+  PyObject *element = pyTypeFactory(cx, elementVal);
   for (int64_t index = start; index >= 0; index--) {
     PyObject *item = PyList_GetItem(self, index);
     Py_INCREF(item);
     int cmp = PyObject_RichCompareBool(item, element, Py_EQ);
     Py_DECREF(item);
     if (cmp < 0) {
+      Py_XDECREF(element);
       return false;
     }
     else if (cmp == 1) {
+      Py_XDECREF(element);
       args.rval().setInt32(index);
       return true;
     }
   }
+  Py_XDECREF(element);
 
   args.rval().setInt32(-1);
   return true;
 }
 
 static bool array_includes(JSContext *cx, unsigned argc, JS::Value *vp) {
   JS::CallArgs args = JS::CallArgsFromVp(argc, vp);
@@ -1232,23 +1262,22 @@
   Py_ssize_t sourceLen, uint32_t start, uint32_t depth) {
 
   uint32_t targetIndex = start;
 
   JS::RootedValue elementVal(cx);
 
   for (uint32_t sourceIndex = 0; sourceIndex < sourceLen; sourceIndex++) {
-
     if (PyObject_TypeCheck(source, &JSArrayProxyType)) {
       JS_GetElement(cx, *(((JSArrayProxy *)source)->jsArray), sourceIndex, &elementVal);
     }
     else if (PyObject_TypeCheck(source, &PyList_Type)) {
       elementVal.set(jsTypeFactory(cx, PyList_GetItem(source, sourceIndex)));
     }
 
-    PyObject *element = pyTypeFactory(cx, elementVal)->getPyObject();
+    PyObject *element = pyTypeFactory(cx, elementVal);
 
     bool shouldFlatten;
     if (depth > 0) {
       shouldFlatten = PyObject_TypeCheck(element, &JSArrayProxyType) || PyObject_TypeCheck(element, &PyList_Type);
     } else {
       shouldFlatten = false;
     }
@@ -1279,14 +1308,16 @@
         JS::SetArrayLength(cx, rootedRetArray, targetIndex + 1);
       }
 
       JS_SetElement(cx, rootedRetArray, targetIndex, elementVal);
 
       targetIndex++;
     }
+
+    Py_DECREF(element);
   }
 
   return targetIndex;
 }
 
 // private
 static uint32_t FlattenIntoArrayWithCallBack(JSContext *cx,
@@ -1312,15 +1343,15 @@
     jArgs[0].set(elementVal);
     jArgs[1].setInt32(sourceIndex);
     jArgs[2].set(sourceValue);
     if (!JS_CallFunctionValue(cx, thisArg, callBack, jArgs, &retVal)) {
       return false;
     }
 
-    PyObject *element = pyTypeFactory(cx, retVal)->getPyObject();
+    PyObject *element = pyTypeFactory(cx, retVal);
 
     bool shouldFlatten;
     if (depth > 0) {
       shouldFlatten = PyObject_TypeCheck(element, &JSArrayProxyType) || PyObject_TypeCheck(element, &PyList_Type);
     } else {
       shouldFlatten = false;
     }
@@ -1376,14 +1407,16 @@
         }
 
         JS_SetElement(cx, rootedRetArray, targetIndex, retVal);
 
         targetIndex++;
       }
     }
+
+    Py_DECREF(element);
   }
 
   return targetIndex;
 }
 
 static bool array_flat(JSContext *cx, unsigned argc, JS::Value *vp) {
   JS::CallArgs args = JS::CallArgsFromVp(argc, vp);
@@ -2087,15 +2120,15 @@
     return result.failNotDataDescriptor();
   }
   if (!desc.hasValue()) {
     return result.failInvalidDescriptor();
   }
 
   JS::RootedValue itemV(cx, desc.value());
-  PyObject *item = pyTypeFactory(cx, itemV)->getPyObject();
+  PyObject *item = pyTypeFactory(cx, itemV);
   PyObject *self = JS::GetMaybePtrFromReservedSlot<PyObject>(proxy, PyObjectSlot);
   if (PyList_SetItem(self, index, item) < 0) {
     // we are out-of-bounds and need to expand
     Py_ssize_t len = PyList_GET_SIZE(self);
     // fill the space until the inserted index
     for (Py_ssize_t i = len; i < index; i++) {
       PyList_Append(self, Py_None);
```

### Comparing `pythonmonkey-0.4.0/src/PyObjectProxyHandler.cc` & `pythonmonkey-0.6.0/src/PyObjectProxyHandler.cc`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 /**
  * @file PyObjectProxyHandler.cc
  * @author Caleb Aikens (caleb@distributive.network)
- * @brief
+ * @brief Struct for creating JS proxy objects for all objects
  * @date 2024-01-30
  *
  * @copyright Copyright (c) 2023 Distributive Corp.
  *
  */
 
 #include "include/PyObjectProxyHandler.hh"
 
 #include "include/jsTypeFactory.hh"
 #include "include/pyTypeFactory.hh"
-#include "include/StrType.hh"
 
 #include <jsapi.h>
 #include <jsfriendapi.h>
 #include <js/Conversions.h>
 #include <js/Proxy.h>
 #include <js/Symbol.h>
 #include <js/friend/ErrorMessages.h>
@@ -171,17 +170,20 @@
 bool PyObjectProxyHandler::set(JSContext *cx, JS::HandleObject proxy, JS::HandleId id,
   JS::HandleValue v, JS::HandleValue receiver,
   JS::ObjectOpResult &result) const {
   JS::RootedValue rootedV(cx, v);
   PyObject *attrName = idToKey(cx, id);
 
   PyObject *self = JS::GetMaybePtrFromReservedSlot<PyObject>(proxy, PyObjectSlot);
-  if (PyObject_SetAttr(self, attrName, pyTypeFactory(cx, rootedV)->getPyObject())) {
+  PyObject *value = pyTypeFactory(cx, rootedV);
+  if (PyObject_SetAttr(self, attrName, value)) {
+    Py_DECREF(value);
     return result.failCantSetInterposed(); // raises JS exception
   }
+  Py_DECREF(value);
   return result.succeed();
 }
 
 bool PyObjectProxyHandler::enumerate(JSContext *cx, JS::HandleObject proxy,
   JS::MutableHandleIdVector props) const {
   return this->ownPropertyKeys(cx, proxy, props);
 }
```

### Comparing `pythonmonkey-0.4.0/src/StrType.cc` & `pythonmonkey-0.6.0/src/StrType.cc`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 /**
  * @file StrType.cc
- * @author Caleb Aikens (caleb@distributive.network) & Giovanni Tedesco (giovanni@distributive.network)
+ * @author Caleb Aikens (caleb@distributive.network), Giovanni Tedesco (giovanni@distributive.network) and Philippe Laporte (philippe@distributive.network)
  * @brief Struct for representing python strings
  * @date 2022-08-08
  *
- * @copyright Copyright (c) 2022 Distributive Corp.
+ * @copyright Copyright (c) 2022,2024 Distributive Corp.
  *
  */
 
 #include "include/StrType.hh"
-#include "include/PyType.hh"
 #include "include/JSStringProxy.hh"
 
-#include <Python.h>
-
 #include <jsapi.h>
 #include <js/String.h>
 
 #define PY_UNICODE_HAS_WSTR (PY_VERSION_HEX < 0x030c0000) // Python version is less than 3.12
 
 #define HIGH_SURROGATE_START 0xD800
 #define HIGH_SURROGATE_END 0xDBFF
@@ -51,27 +48,65 @@
     if (Py_UNICODE_IS_SURROGATE(chars[i])) {
       return true;
     }
   }
   return false;
 }
 
-StrType::StrType(PyObject *object) : PyType(object) {}
+/**
+ * @brief creates new UCS4-encoded pyObject string. This must be called by the user if the original JSString contains any surrogate pairs
+ *
+ * @return PyObject* - the UCS4-encoding of the pyObject string
+ *
+ */
+static PyObject *asUCS4(PyObject *pyObject) {
+  if (PyUnicode_KIND(pyObject) != PyUnicode_2BYTE_KIND) {
+    // return a new reference to match the behaviour of `PyUnicode_FromKindAndData`
+    Py_INCREF(pyObject);
+    return pyObject;
+  }
+
+  uint16_t *chars = PY_UNICODE_OBJECT_DATA_UCS2(pyObject);
+  size_t length = PY_UNICODE_OBJECT_LENGTH(pyObject);
+
+  uint32_t *ucs4String = new uint32_t[length];
+  size_t ucs4Length = 0;
+
+  for (size_t i = 0; i < length; i++, ucs4Length++) {
+    if (Py_UNICODE_IS_LOW_SURROGATE(chars[i])) { // character is an unpaired low surrogate
+      delete[] ucs4String;
+      return NULL;
+    } else if (Py_UNICODE_IS_HIGH_SURROGATE(chars[i])) { // character is a high surrogate
+      if ((i + 1 < length) && Py_UNICODE_IS_LOW_SURROGATE(chars[i+1])) { // next character is a low surrogate
+        ucs4String[ucs4Length] = Py_UNICODE_JOIN_SURROGATES(chars[i], chars[i+1]);
+        i++; // skip over low surrogate
+      }
+      else { // next character is not a low surrogate
+        delete[] ucs4String;
+        return NULL;
+      }
+    } else { // character is not a surrogate, and is in the BMP
+      ucs4String[ucs4Length] = chars[i];
+    }
+  }
 
-StrType::StrType(char *string) : PyType(Py_BuildValue("s", string)) {}
+  PyObject *ret = PyUnicode_FromKindAndData(PyUnicode_4BYTE_KIND, ucs4String, ucs4Length);
+  delete[] ucs4String;
+  return ret;
+}
 
-StrType::StrType(JSContext *cx, JSString *str) {
+static PyObject *processString(JSContext *cx, JSString *str) {
   JSLinearString *lstr = JS_EnsureLinearString(cx, str);
   JS::AutoCheckCannotGC nogc;
   PyObject *p;
 
   size_t length = JS::GetLinearStringLength(lstr);
 
-  pyObject = (PyObject *)PyObject_New(JSStringProxy, &JSStringProxyType); // new reference
-  Py_INCREF(pyObject); // XXX: Why?
+  PyObject *pyObject = (PyObject *)PyObject_New(JSStringProxy, &JSStringProxyType); // new reference
+  Py_INCREF(pyObject);
 
   ((JSStringProxy *)pyObject)->jsString.setString((JSString *)lstr);
 
   // Initialize as legacy string (https://github.com/python/cpython/blob/v3.12.0b1/Include/cpython/unicodeobject.h#L78-L93)
   // see https://github.com/python/cpython/blob/v3.11.3/Objects/unicodeobject.c#L1230-L1245
   PY_UNICODE_OBJECT_HASH(pyObject) = -1;
   PY_UNICODE_OBJECT_STATE(pyObject).interned = 0;
@@ -117,54 +152,27 @@
   #endif
 
     if (containsSurrogatePair(chars, length)) {
       // We must convert to UCS4 here because Python does not support decoding string containing surrogate pairs to bytes
       PyObject *ucs4Obj = asUCS4(pyObject); // convert to a new PyUnicodeObject with UCS4 data
       if (!ucs4Obj) {
         // conversion fails, keep the original `pyObject`
-        return;
+        return pyObject;
       }
-      Py_DECREF(pyObject); // cleanup the old `pyObject`
-      Py_INCREF(ucs4Obj); // XXX: Same as the above `Py_INCREF(pyObject);`. Why double freed on GC?
-      pyObject = ucs4Obj;
+      Py_DECREF(pyObject);
+      return ucs4Obj;
     }
   }
-}
 
-const char *StrType::getValue() const {
-  return PyUnicode_AsUTF8(pyObject);
+  return pyObject;
 }
 
-/* static */
-PyObject *StrType::asUCS4(PyObject *pyObject) {
-  if (PyUnicode_KIND(pyObject) != PyUnicode_2BYTE_KIND) {
-    // return a new reference to match the behaviour of `PyUnicode_FromKindAndData`
-    Py_INCREF(pyObject);
-    return pyObject;
-  }
-
-  uint16_t *chars = PY_UNICODE_OBJECT_DATA_UCS2(pyObject);
-  size_t length = PY_UNICODE_OBJECT_LENGTH(pyObject);
-
-  uint32_t *ucs4String = new uint32_t[length];
-  size_t ucs4Length = 0;
-
-  for (size_t i = 0; i < length; i++, ucs4Length++) {
-    if (Py_UNICODE_IS_LOW_SURROGATE(chars[i])) { // character is an unpaired low surrogate
-      return NULL;
-    } else if (Py_UNICODE_IS_HIGH_SURROGATE(chars[i])) { // character is a high surrogate
-      if ((i + 1 < length) && Py_UNICODE_IS_LOW_SURROGATE(chars[i+1])) { // next character is a low surrogate
-        ucs4String[ucs4Length] = Py_UNICODE_JOIN_SURROGATES(chars[i], chars[i+1]);
-        i++; // skip over low surrogate
-      }
-      else { // next character is not a low surrogate
-        return NULL;
-      }
-    } else { // character is not a surrogate, and is in the BMP
-      ucs4String[ucs4Length] = chars[i];
-    }
-  }
+PyObject *StrType::getPyObject(JSContext *cx, JSString *str) {
+  return processString(cx, str);
+}
 
-  PyObject *ret = PyUnicode_FromKindAndData(PyUnicode_4BYTE_KIND, ucs4String, ucs4Length);
-  delete[] ucs4String;
-  return ret;
+const char *StrType::getValue(JSContext *cx, JSString *str) {
+  PyObject *pyObject = processString(cx, str);
+  const char *value = PyUnicode_AsUTF8(pyObject);
+  Py_DECREF(pyObject);
+  return value;
 }
```

### Comparing `pythonmonkey-0.4.0/src/internalBinding/timers.cc` & `pythonmonkey-0.6.0/src/internalBinding/timers.cc`

 * *Files 8% similar despite different names*

```diff
@@ -19,25 +19,27 @@
  *    `declare function internalBinding(namespace: "timers")`
  */
 
 static bool enqueueWithDelay(JSContext *cx, unsigned argc, JS::Value *vp) {
   JS::CallArgs args = JS::CallArgsFromVp(argc, vp);
   JS::HandleValue jobArgVal = args.get(0);
   double delaySeconds = args.get(1).toNumber();
+  bool repeat = args.get(2).toBoolean();
 
   // Convert to a Python function
   JS::RootedValue jobArg(cx, jobArgVal);
-  PyObject *job = pyTypeFactory(cx, jobArg)->getPyObject();
+  PyObject *job = pyTypeFactory(cx, jobArg);
   // Schedule job to the running Python event-loop
   PyEventLoop loop = PyEventLoop::getRunningLoop();
   if (!loop.initialized()) return false;
-  PyEventLoop::AsyncHandle::id_ptr_pair handler = loop.enqueueWithDelay(job, delaySeconds);
+  PyEventLoop::AsyncHandle::id_t handleId = loop.enqueueWithDelay(job, delaySeconds, repeat);
+  Py_DECREF(job);
 
   // Return the `timeoutID` to use in `clearTimeout`
-  args.rval().setNumber(handler.first);
+  args.rval().setNumber(handleId);
   return true;
 }
 
 static bool cancelByTimeoutId(JSContext *cx, unsigned argc, JS::Value *vp) {
   JS::CallArgs args = JS::CallArgsFromVp(argc, vp);
   double timeoutID = args.get(0).toNumber();
```

### Comparing `pythonmonkey-0.4.0/src/internalBinding/utils.cc` & `pythonmonkey-0.6.0/src/internalBinding/utils.cc`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 /**
  * @file utils.cc
  * @author Tom Tang (xmader@distributive.network)
  * @brief Implement functions in `internalBinding("utils")`
- * 
+ *
  * @copyright Copyright (c) 2023 Distributive Corp.
  */
 
 #include "include/internalBinding.hh"
 
 #include <jsapi.h>
 #include <js/Array.h>
```

### Comparing `pythonmonkey-0.4.0/src/internalBinding.cc` & `pythonmonkey-0.6.0/src/internalBinding.cc`

 * *Files 2% similar despite different names*

```diff
@@ -56,9 +56,9 @@
  */
 PyObject *getInternalBindingPyFn(JSContext *cx) {
   // Create the JS `internalBinding` function
   JSObject *jsFn = (JSObject *)createInternalBinding(cx);
 
   // Convert to a Python function
   JS::RootedValue jsFnVal(cx, JS::ObjectValue(*jsFn));
-  return pyTypeFactory(cx, jsFnVal)->getPyObject();
+  return pyTypeFactory(cx, jsFnVal);
 }
```

### Comparing `pythonmonkey-0.4.0/src/jsTypeFactory.cc` & `pythonmonkey-0.6.0/src/jsTypeFactory.cc`

 * *Files 4% similar despite different names*

```diff
@@ -7,26 +7,24 @@
  * @copyright 2023-2024 Distributive Corp.
  *
  */
 
 #include "include/jsTypeFactory.hh"
 
 #include "include/modules/pythonmonkey/pythonmonkey.hh"
-#include "include/PyType.hh"
-#include "include/FuncType.hh"
 #include "include/JSFunctionProxy.hh"
 #include "include/JSMethodProxy.hh"
 #include "include/JSObjectProxy.hh"
 #include "include/JSArrayProxy.hh"
 #include "include/PyDictProxyHandler.hh"
 #include "include/JSStringProxy.hh"
 #include "include/PyListProxyHandler.hh"
 #include "include/PyObjectProxyHandler.hh"
+#include "include/PyIterableProxyHandler.hh"
 #include "include/pyTypeFactory.hh"
-#include "include/StrType.hh"
 #include "include/IntType.hh"
 #include "include/PromiseType.hh"
 #include "include/DateType.hh"
 #include "include/ExceptionType.hh"
 #include "include/BufferType.hh"
 #include "include/setSpiderMonkeyException.hh"
 
@@ -45,14 +43,15 @@
 #define LOW_SURROGATE_START 0xDC00
 #define LOW_SURROGATE_END 0xDFFF
 #define BMP_END 0x10000
 
 static PyDictProxyHandler pyDictProxyHandler;
 static PyObjectProxyHandler pyObjectProxyHandler;
 static PyListProxyHandler pyListProxyHandler;
+static PyIterableProxyHandler pyIterableProxyHandler;
 
 std::unordered_map<char16_t *, PyObject *> charToPyObjectMap; // a map of char16_t buffers to their corresponding PyObjects, used when finalizing JSExternalStrings
 
 struct PythonExternalString : public JSExternalStringCallbacks {
   void finalize(char16_t *chars) const override {
     // We cannot call Py_DECREF here when shutting down as the thread state is gone.
     // Then, when shutting down, there is only on reference left, and we don't need
@@ -95,16 +94,16 @@
 
   JS::RootedValue returnType(cx);
 
   if (PyBool_Check(object)) {
     returnType.setBoolean(PyLong_AsLong(object));
   }
   else if (PyLong_Check(object)) {
-    if (PyObject_IsInstance(object, PythonMonkey_BigInt)) { // pm.bigint is a subclass of the builtin int type
-      JS::BigInt *bigint = IntType(object).toJsBigInt(cx);
+    if (PyObject_IsInstance(object, getPythonMonkeyBigInt())) { // pm.bigint is a subclass of the builtin int type
+      JS::BigInt *bigint = IntType::toJsBigInt(cx, object);
       returnType.setBigInt(bigint);
     } else if (_PyLong_NumBits(object) <= 53) { // num <= JS Number.MAX_SAFE_INTEGER, the mantissa of a float64 is 53 bits (with 52 explicitly stored and the highest bit always being 1)
       int64_t num = PyLong_AsLongLong(object);
       returnType.setNumber(num);
     } else {
       PyErr_SetString(PyExc_OverflowError, "Absolute value of the integer exceeds JS Number.MAX_SAFE_INTEGER. Use pythonmonkey.bigint instead.");
     }
@@ -181,20 +180,19 @@
       returnType.setObject(*error);
     }
     else {
       returnType.setUndefined();
     }
   }
   else if (PyDateTime_Check(object)) {
-    JSObject *dateObj = DateType(object).toJsDate(cx);
+    JSObject *dateObj = DateType::toJsDate(cx, object);
     returnType.setObject(*dateObj);
   }
   else if (PyObject_CheckBuffer(object)) {
-    BufferType *pmBuffer = new BufferType(object);
-    JSObject *typedArray = pmBuffer->toJsTypedArray(cx); // may return null
+    JSObject *typedArray = BufferType::toJsTypedArray(cx, object); // may return null
     returnType.setObjectOrNull(typedArray);
   }
   else if (PyObject_TypeCheck(object, &JSObjectProxyType)) {
     returnType.setObject(**((JSObjectProxy *)object)->jsObject);
   }
   else if (PyObject_TypeCheck(object, &JSMethodProxyType)) {
     JS::RootedObject func(cx, *((JSMethodProxy *)object)->jsFunc);
@@ -242,19 +240,29 @@
     Py_INCREF(object);
     JS::SetReservedSlot(proxy, PyObjectSlot, JS::PrivateValue(object));
     returnType.setObject(*proxy);
   }
   else if (object == Py_None) {
     returnType.setUndefined();
   }
-  else if (object == PythonMonkey_Null) {
+  else if (object == getPythonMonkeyNull()) {
     returnType.setNull();
   }
   else if (PythonAwaitable_Check(object)) {
-    returnType.setObjectOrNull((new PromiseType(object))->toJsPromise(cx));
+    returnType.setObjectOrNull(PromiseType::toJsPromise(cx, object));
+  }
+  else if (PyIter_Check(object)) {
+    JS::RootedValue v(cx);
+    JS::RootedObject objectPrototype(cx);
+    JS_GetClassPrototype(cx, JSProto_Object, &objectPrototype); // so that instanceof will work, not that prototype methods will
+    JSObject *proxy = js::NewProxyObject(cx, &pyIterableProxyHandler, v, objectPrototype.get());
+    PyObject *iterable = PyObject_GetIter(object);
+    Py_INCREF(iterable);
+    JS::SetReservedSlot(proxy, PyObjectSlot, JS::PrivateValue(iterable));
+    returnType.setObject(*proxy);
   }
   else {
     JS::RootedValue v(cx);
     JS::RootedObject objectPrototype(cx);
     JS_GetClassPrototype(cx, JSProto_Object, &objectPrototype); // so that instanceof will work, not that prototype methods will
     JSObject *proxy = js::NewProxyObject(cx, &pyObjectProxyHandler, v, objectPrototype.get());
     Py_INCREF(object);
@@ -325,17 +333,15 @@
     return true;
   }
 
   // populate python args tuple
   PyObject *pyArgs = PyTuple_New(callArgsLength);
   for (size_t i = 0; i < callArgsLength; i++) {
     JS::RootedValue jsArg(cx, callargs[i]);
-    PyType *pyArg = pyTypeFactory(cx, jsArg);
-    if (!pyArg) return false; // error occurred
-    PyObject *pyArgObj = pyArg->getPyObject();
+    PyObject *pyArgObj = pyTypeFactory(cx, jsArg);
     if (!pyArgObj) return false; // error occurred
     PyTuple_SetItem(pyArgs, i, pyArgObj);
   }
 
   PyObject *pyRval = PyObject_Call(pyFunc, pyArgs, NULL);
   if (PyErr_Occurred()) {
     setPyException(cx);
```

### Comparing `pythonmonkey-0.4.0/src/modules/pythonmonkey/pythonmonkey.cc` & `pythonmonkey-0.6.0/src/modules/pythonmonkey/pythonmonkey.cc`

 * *Files 4% similar despite different names*

```diff
@@ -6,32 +6,26 @@
  *
  * @copyright Copyright (c) 2023-2024 Distributive Corp.
  *
  */
 
 #include "include/modules/pythonmonkey/pythonmonkey.hh"
 
-#include "include/BoolType.hh"
 #include "include/setSpiderMonkeyException.hh"
-#include "include/DateType.hh"
-#include "include/FloatType.hh"
-#include "include/FuncType.hh"
 #include "include/JSFunctionProxy.hh"
 #include "include/JSMethodProxy.hh"
 #include "include/JSArrayIterProxy.hh"
 #include "include/JSArrayProxy.hh"
 #include "include/JSObjectIterProxy.hh"
 #include "include/JSObjectKeysProxy.hh"
 #include "include/JSObjectValuesProxy.hh"
 #include "include/JSObjectItemsProxy.hh"
 #include "include/JSObjectProxy.hh"
 #include "include/JSStringProxy.hh"
-#include "include/PyType.hh"
 #include "include/pyTypeFactory.hh"
-#include "include/StrType.hh"
 #include "include/PyEventLoop.hh"
 #include "include/internalBinding.hh"
 
 #include <jsapi.h>
 #include <jsfriendapi.h>
 #include <js/friend/ErrorMessages.h>
 #include <js/friend/DOMProxy.h>
@@ -67,31 +61,47 @@
   return true;
 }
 
 static void cleanupFinalizationRegistry(JSFunction *callback, JSObject *global [[maybe_unused]], void *user_data [[maybe_unused]]) {
   JOB_QUEUE->queueFinalizationRegistryCallback(callback);
 }
 
+static PyObject *PythonMonkey_Null;
+static PyObject *PythonMonkey_BigInt;
+
+PyObject *getPythonMonkeyNull() {
+  if (!PythonMonkey_Null) {
+    PythonMonkey_Null = PyObject_GetAttrString(PyState_FindModule(&pythonmonkey), "null");
+  }
+  return PythonMonkey_Null;
+}
+
+PyObject *getPythonMonkeyBigInt() {
+  if (!PythonMonkey_BigInt) {
+    PythonMonkey_BigInt = PyObject_GetAttrString(PyState_FindModule(&pythonmonkey), "bigint");
+  }
+  return PythonMonkey_BigInt;
+}
+
+
 typedef struct {
   PyObject_HEAD
 } NullObject;
 
 static PyTypeObject NullType = {
   .ob_base = PyVarObject_HEAD_INIT(NULL, 0)
   .tp_name = "pythonmonkey.null",
   .tp_basicsize = sizeof(NullObject),
   .tp_flags = Py_TPFLAGS_DEFAULT,
   .tp_doc = PyDoc_STR("Javascript null object")
 };
 
 static PyTypeObject BigIntType = {
   .tp_name = PyLong_Type.tp_name,
-  .tp_flags = Py_TPFLAGS_DEFAULT
-  | Py_TPFLAGS_LONG_SUBCLASS
-  | Py_TPFLAGS_BASETYPE,     // can be subclassed
+  .tp_flags = Py_TPFLAGS_DEFAULT | Py_TPFLAGS_LONG_SUBCLASS,
   .tp_doc = PyDoc_STR("Javascript BigInt object"),
   .tp_base = &PyLong_Type
 };
 
 PyTypeObject JSObjectProxyType = {
   .ob_base = PyVarObject_HEAD_INIT(NULL, 0)
   .tp_name = PyDict_Type.tp_name,
@@ -100,28 +110,29 @@
   .tp_dealloc = (destructor)JSObjectProxyMethodDefinitions::JSObjectProxy_dealloc,
   .tp_repr = (reprfunc)JSObjectProxyMethodDefinitions::JSObjectProxy_repr,
   .tp_as_number = &JSObjectProxy_number_methods,
   .tp_as_sequence = &JSObjectProxy_sequence_methods,
   .tp_as_mapping = &JSObjectProxy_mapping_methods,
   .tp_getattro = (getattrofunc)JSObjectProxyMethodDefinitions::JSObjectProxy_get,
   .tp_setattro = (setattrofunc)JSObjectProxyMethodDefinitions::JSObjectProxy_assign,
-  .tp_flags = Py_TPFLAGS_DEFAULT | Py_TPFLAGS_DICT_SUBCLASS,
+  .tp_flags = Py_TPFLAGS_DEFAULT | Py_TPFLAGS_DICT_SUBCLASS | Py_TPFLAGS_HAVE_GC,
   .tp_doc = PyDoc_STR("Javascript Object proxy dict"),
+  .tp_traverse = (traverseproc)JSObjectProxyMethodDefinitions::JSObjectProxy_traverse,
+  .tp_clear = (inquiry)JSObjectProxyMethodDefinitions::JSObjectProxy_clear,
   .tp_richcompare = (richcmpfunc)JSObjectProxyMethodDefinitions::JSObjectProxy_richcompare,
   .tp_iter = (getiterfunc)JSObjectProxyMethodDefinitions::JSObjectProxy_iter,
+  .tp_iternext = (iternextfunc)JSObjectProxyMethodDefinitions::JSObjectProxy_iter_next,
   .tp_methods = JSObjectProxy_methods,
   .tp_base = &PyDict_Type
 };
 
 PyTypeObject JSStringProxyType = {
   .tp_name = PyUnicode_Type.tp_name,
   .tp_basicsize = sizeof(JSStringProxy),
-  .tp_flags = Py_TPFLAGS_DEFAULT
-  | Py_TPFLAGS_UNICODE_SUBCLASS
-  | Py_TPFLAGS_BASETYPE,     // can be subclassed
+  .tp_flags = Py_TPFLAGS_DEFAULT | Py_TPFLAGS_UNICODE_SUBCLASS,
   .tp_doc = PyDoc_STR("Javascript String value"),
   .tp_base = &PyUnicode_Type
 };
 
 PyTypeObject JSFunctionProxyType = {
   .ob_base = PyVarObject_HEAD_INIT(NULL, 0)
   .tp_name = "pythonmonkey.JSFunctionProxy",
@@ -150,16 +161,18 @@
   .tp_basicsize = sizeof(JSArrayProxy),
   .tp_itemsize = 0,
   .tp_dealloc = (destructor)JSArrayProxyMethodDefinitions::JSArrayProxy_dealloc,
   .tp_repr = (reprfunc)JSArrayProxyMethodDefinitions::JSArrayProxy_repr,
   .tp_as_sequence = &JSArrayProxy_sequence_methods,
   .tp_as_mapping = &JSArrayProxy_mapping_methods,
   .tp_getattro = (getattrofunc)JSArrayProxyMethodDefinitions::JSArrayProxy_get,
-  .tp_flags = Py_TPFLAGS_DEFAULT | Py_TPFLAGS_LIST_SUBCLASS,
+  .tp_flags = Py_TPFLAGS_DEFAULT | Py_TPFLAGS_LIST_SUBCLASS | Py_TPFLAGS_HAVE_GC,
   .tp_doc = PyDoc_STR("Javascript Array proxy list"),
+  .tp_traverse = (traverseproc)JSArrayProxyMethodDefinitions::JSArrayProxy_traverse,
+  .tp_clear = (inquiry)JSArrayProxyMethodDefinitions::JSArrayProxy_clear,
   .tp_richcompare = (richcmpfunc)JSArrayProxyMethodDefinitions::JSArrayProxy_richcompare,
   .tp_iter = (getiterfunc)JSArrayProxyMethodDefinitions::JSArrayProxy_iter,
   .tp_methods = JSArrayProxy_methods,
   .tp_base = &PyList_Type
 };
 
 PyTypeObject JSArrayIterProxyType = {
@@ -168,14 +181,15 @@
   .tp_basicsize = sizeof(JSArrayIterProxy),
   .tp_itemsize = 0,
   .tp_dealloc = (destructor)JSArrayIterProxyMethodDefinitions::JSArrayIterProxy_dealloc,
   .tp_getattro = PyObject_GenericGetAttr,
   .tp_flags = Py_TPFLAGS_DEFAULT | Py_TPFLAGS_HAVE_GC,
   .tp_doc = PyDoc_STR("Javascript Array proxy iterator"),
   .tp_traverse =  (traverseproc)JSArrayIterProxyMethodDefinitions::JSArrayIterProxy_traverse,
+  .tp_clear = (inquiry)JSArrayIterProxyMethodDefinitions::JSArrayIterProxy_clear,
   .tp_iter = (getiterfunc)JSArrayIterProxyMethodDefinitions::JSArrayIterProxy_iter,
   .tp_iternext = (iternextfunc)JSArrayIterProxyMethodDefinitions::JSArrayIterProxy_next,
   .tp_methods = JSArrayIterProxy_methods,
   .tp_base = &PyListIter_Type
 };
 
 PyTypeObject JSObjectIterProxyType = {
@@ -184,14 +198,15 @@
   .tp_basicsize = sizeof(JSObjectIterProxy),
   .tp_itemsize = 0,
   .tp_dealloc = (destructor)JSObjectIterProxyMethodDefinitions::JSObjectIterProxy_dealloc,
   .tp_getattro = PyObject_GenericGetAttr,
   .tp_flags = Py_TPFLAGS_DEFAULT | Py_TPFLAGS_HAVE_GC,
   .tp_doc = PyDoc_STR("Javascript Object proxy key iterator"),
   .tp_traverse =  (traverseproc)JSObjectIterProxyMethodDefinitions::JSObjectIterProxy_traverse,
+  .tp_clear = (inquiry)JSObjectIterProxyMethodDefinitions::JSObjectIterProxy_clear,
   .tp_iter = (getiterfunc)JSObjectIterProxyMethodDefinitions::JSObjectIterProxy_iter,
   .tp_iternext = (iternextfunc)JSObjectIterProxyMethodDefinitions::JSObjectIterProxy_nextkey,
   .tp_methods = JSObjectIterProxy_methods,
   .tp_base = &PyDictIterKey_Type
 };
 
 PyTypeObject JSObjectKeysProxyType = {
@@ -203,14 +218,15 @@
   .tp_repr = (reprfunc)JSObjectKeysProxyMethodDefinitions::JSObjectKeysProxy_repr,
   .tp_as_number = &JSObjectKeysProxy_number_methods,
   .tp_as_sequence = &JSObjectKeysProxy_sequence_methods,
   .tp_getattro = PyObject_GenericGetAttr,
   .tp_flags = Py_TPFLAGS_DEFAULT | Py_TPFLAGS_HAVE_GC,
   .tp_doc = PyDoc_STR("Javascript Object Keys proxy"),
   .tp_traverse =  (traverseproc)JSObjectKeysProxyMethodDefinitions::JSObjectKeysProxy_traverse,
+  .tp_clear = (inquiry)JSObjectKeysProxyMethodDefinitions::JSObjectKeysProxy_clear,
   .tp_richcompare = (richcmpfunc)JSObjectKeysProxyMethodDefinitions::JSObjectKeysProxy_richcompare,
   .tp_iter = (getiterfunc)JSObjectKeysProxyMethodDefinitions::JSObjectKeysProxy_iter,
   .tp_methods = JSObjectKeysProxy_methods,
   .tp_getset = JSObjectKeysProxy_getset,
   .tp_base = &PyDictKeys_Type
 };
 
@@ -222,14 +238,15 @@
   .tp_dealloc = (destructor)JSObjectValuesProxyMethodDefinitions::JSObjectValuesProxy_dealloc,
   .tp_repr = (reprfunc)JSObjectValuesProxyMethodDefinitions::JSObjectValuesProxy_repr,
   .tp_as_sequence = &JSObjectValuesProxy_sequence_methods,
   .tp_getattro = PyObject_GenericGetAttr,
   .tp_flags = Py_TPFLAGS_DEFAULT | Py_TPFLAGS_HAVE_GC,
   .tp_doc = PyDoc_STR("Javascript Object Values proxy"),
   .tp_traverse =  (traverseproc)JSObjectValuesProxyMethodDefinitions::JSObjectValuesProxy_traverse,
+  .tp_clear = (inquiry)JSObjectValuesProxyMethodDefinitions::JSObjectValuesProxy_clear,
   .tp_iter = (getiterfunc)JSObjectValuesProxyMethodDefinitions::JSObjectValuesProxy_iter,
   .tp_methods = JSObjectValuesProxy_methods,
   .tp_getset = JSObjectValuesProxy_getset,
   .tp_base = &PyDictValues_Type
 };
 
 PyTypeObject JSObjectItemsProxyType = {
@@ -241,22 +258,25 @@
   .tp_repr = (reprfunc)JSObjectItemsProxyMethodDefinitions::JSObjectItemsProxy_repr,
   // .tp_as_number = defaults are fine
   .tp_as_sequence = &JSObjectItemsProxy_sequence_methods,
   .tp_getattro = PyObject_GenericGetAttr,
   .tp_flags = Py_TPFLAGS_DEFAULT | Py_TPFLAGS_HAVE_GC,
   .tp_doc = PyDoc_STR("Javascript Object Items proxy"),
   .tp_traverse =  (traverseproc)JSObjectItemsProxyMethodDefinitions::JSObjectItemsProxy_traverse,
+  .tp_clear = (inquiry)JSObjectItemsProxyMethodDefinitions::JSObjectItemsProxy_clear,
   // .tp_richcompare = TODO tuple support
   .tp_iter = (getiterfunc)JSObjectItemsProxyMethodDefinitions::JSObjectItemsProxy_iter,
   .tp_methods = JSObjectItemsProxy_methods,
   .tp_getset = JSObjectItemsProxy_getset,
   .tp_base = &PyDictKeys_Type
 };
 
 static void cleanup() {
+  Py_XDECREF(PythonMonkey_Null);
+  Py_XDECREF(PythonMonkey_BigInt);
   delete autoRealm;
   delete global;
   if (GLOBAL_CX) JS_DestroyContext(GLOBAL_CX);
   delete JOB_QUEUE;
   JS_ShutDown();
 }
 
@@ -318,25 +338,21 @@
 static PyObject *eval(PyObject *self, PyObject *args) {
   size_t argc = PyTuple_GET_SIZE(args);
   if (argc > 2 || argc == 0) {
     PyErr_SetString(PyExc_TypeError, "pythonmonkey.eval accepts one or two arguments");
     return NULL;
   }
 
-  StrType *code = NULL;
+  PyObject *code = NULL;
   FILE *file = NULL;
   PyObject *arg0 = PyTuple_GetItem(args, 0);
   PyObject *arg1 = argc == 2 ? PyTuple_GetItem(args, 1) : NULL;
 
   if (PyUnicode_Check(arg0)) {
-    code = new StrType(arg0);
-    if (!code || !PyUnicode_Check(code->getPyObject())) {
-      PyErr_SetString(PyExc_TypeError, "JS code must originate from a Unicode string");
-      return NULL;
-    }
+    code = arg0;
   } else if (1 /*PyFile_Check(arg0)*/) {
     /* First argument is an open file. Open a stream with a dup of the underlying fd (so we can fclose
      * the stream later). Future: seek to current Python file position IFF the fd is for a real file.
      */
     int fd = PyObject_AsFileDescriptor(arg0);
     int fd2 = fd == -1 ? -1 : dup(fd);
     file = fd2 == -1 ? NULL : fdopen(fd, "rb");
@@ -402,20 +418,19 @@
   } /* eval options */
 
   // compile the code to execute
   JS::RootedScript script(GLOBAL_CX);
   JS::Rooted<JS::Value> *rval = new JS::Rooted<JS::Value>(GLOBAL_CX);
   if (code) {
     JS::SourceText<mozilla::Utf8Unit> source;
-    if (!source.init(GLOBAL_CX, code->getValue(), strlen(code->getValue()), JS::SourceOwnership::Borrowed)) {
+    const char *codeChars = PyUnicode_AsUTF8(code);
+    if (!source.init(GLOBAL_CX, codeChars, strlen(codeChars), JS::SourceOwnership::Borrowed)) {
       setSpiderMonkeyException(GLOBAL_CX);
-      delete code;
       return NULL;
     }
-    delete code;
     script = JS::Compile(GLOBAL_CX, options, source);
   } else {
     assert(file);
     script = JS::CompileUtf8File(GLOBAL_CX, options, file);
     fclose(file);
   }
 
@@ -427,15 +442,15 @@
   // execute the compiled code; last expr goes to rval
   if (!JS_ExecuteScript(GLOBAL_CX, script, rval)) {
     setSpiderMonkeyException(GLOBAL_CX);
     return NULL;
   }
 
   // translate to the proper python type
-  PyType *returnValue = pyTypeFactory(GLOBAL_CX, *rval);
+  PyObject *returnValue = pyTypeFactory(GLOBAL_CX, *rval);
   if (PyErr_Occurred()) {
     return NULL;
   }
 
   // TODO: Find a way to root strings for the lifetime of a proxying python string
   js::ESClass cls = js::ESClass::Other;   // placeholder if `rval` is not a JSObject
   if (rval->isObject()) {
@@ -443,15 +458,15 @@
   }
 
   if (!(rval->isString() || cls == js::ESClass::String)) {   // rval may be a string which must be kept alive.
     delete rval;
   }
 
   if (returnValue) {
-    return returnValue->getPyObject();
+    return returnValue;
   }
   else {
     Py_RETURN_NONE;
   }
 }
 
 static PyObject *waitForEventLoop(PyObject *Py_UNUSED(self), PyObject *Py_UNUSED(_)) {
@@ -462,37 +477,33 @@
   if (!loop.initialized()) return NULL;
   PyObject_SetAttrString(waiter, "_loop", loop._loop);
 
   return PyObject_CallMethod(waiter, "wait", NULL);
 }
 
 static PyObject *isCompilableUnit(PyObject *self, PyObject *args) {
-  StrType *buffer = new StrType(PyTuple_GetItem(args, 0));
-  const char *bufferUtf8;
-  bool compilable;
-
-  if (!PyUnicode_Check(buffer->getPyObject())) {
+  PyObject *item = PyTuple_GetItem(args, 0);
+  if (!PyUnicode_Check(item)) {
     PyErr_SetString(PyExc_TypeError, "pythonmonkey.eval expects a string as its first argument");
     return NULL;
   }
 
-  bufferUtf8 = buffer->getValue();
-  compilable = JS_Utf8BufferIsCompilableUnit(GLOBAL_CX, *global, bufferUtf8, strlen(bufferUtf8));
+  const char *bufferUtf8 = PyUnicode_AsUTF8(item);
 
-  if (compilable)
+  if (JS_Utf8BufferIsCompilableUnit(GLOBAL_CX, *global, bufferUtf8, strlen(bufferUtf8)))
     Py_RETURN_TRUE;
   else
     Py_RETURN_FALSE;
 }
 
 PyMethodDef PythonMonkeyMethods[] = {
   {"eval", eval, METH_VARARGS, "Javascript evaluator in Python"},
   {"wait", waitForEventLoop, METH_NOARGS, "The event-loop shield. Blocks until all asynchronous jobs finish."},
   {"isCompilableUnit", isCompilableUnit, METH_VARARGS, "Hint if a string might be compilable Javascript"},
-  {"collect", collect, METH_VARARGS, "Calls the spidermonkey garbage collector"},
+  {"collect", collect, METH_VARARGS, "Calls the Spidermonkey garbage collector"},
   {NULL, NULL, 0, NULL}
 };
 
 struct PyModuleDef pythonmonkey =
 {
   PyModuleDef_HEAD_INIT,
   "pythonmonkey",                                   /* name of module */
@@ -566,15 +577,14 @@
   // In https://hg.mozilla.org/releases/mozilla-esr102/file/3b574e1/js/src/jit/CacheIR.cpp#l317, trying to use the callback returned by `js::GetDOMProxyShadowsCheck()` even it's unset (nullptr)
   // Temporarily solved by explicitly setting the `domProxyShadowsCheck` callback here
   JS::SetDOMProxyInformation(nullptr,
     [](JSContext *, JS::HandleObject, JS::HandleId) {   // domProxyShadowsCheck
       return JS::DOMProxyShadowsResult::ShadowCheckFailed;
     }, nullptr);
 
-  PyObject *pyModule;
   if (PyType_Ready(&NullType) < 0)
     return NULL;
   if (PyType_Ready(&BigIntType) < 0)
     return NULL;
   if (PyType_Ready(&JSObjectProxyType) < 0)
     return NULL;
   if (PyType_Ready(&JSStringProxyType) < 0)
@@ -592,15 +602,15 @@
   if (PyType_Ready(&JSObjectKeysProxyType) < 0)
     return NULL;
   if (PyType_Ready(&JSObjectValuesProxyType) < 0)
     return NULL;
   if (PyType_Ready(&JSObjectItemsProxyType) < 0)
     return NULL;
 
-  pyModule = PyModule_Create(&pythonmonkey);
+  PyObject *pyModule = PyModule_Create(&pythonmonkey);
   if (pyModule == NULL)
     return NULL;
 
   Py_INCREF(&NullType);
   if (PyModule_AddObject(pyModule, "null", (PyObject *)&NullType) < 0) {
     Py_DECREF(&NullType);
     Py_DECREF(pyModule);
@@ -714,8 +724,8 @@
   }
   jsFunctionRegistry.init(GLOBAL_CX);
   jsFunctionRegistry.set(registryObject);
 
   JS::SetHostCleanupFinalizationRegistryCallback(GLOBAL_CX, cleanupFinalizationRegistry, NULL);
 
   return pyModule;
-}
+}
```

### Comparing `pythonmonkey-0.4.0/src/pyTypeFactory.cc` & `pythonmonkey-0.6.0/src/pyTypeFactory.cc`

 * *Files 9% similar despite different names*

```diff
@@ -22,106 +22,103 @@
 #include "include/ListType.hh"
 #include "include/NoneType.hh"
 #include "include/NullType.hh"
 #include "include/PromiseType.hh"
 #include "include/PyDictProxyHandler.hh"
 #include "include/PyListProxyHandler.hh"
 #include "include/PyObjectProxyHandler.hh"
-#include "include/PyType.hh"
+#include "include/PyIterableProxyHandler.hh"
 #include "include/setSpiderMonkeyException.hh"
 #include "include/StrType.hh"
-#include "include/TupleType.hh"
 #include "include/modules/pythonmonkey/pythonmonkey.hh"
 
 #include <jsapi.h>
 #include <jsfriendapi.h>
 #include <js/Object.h>
 #include <js/ValueArray.h>
 
-#include <Python.h>
-
-
-PyType *pyTypeFactory(JSContext *cx, JS::HandleValue rval) {
+PyObject *pyTypeFactory(JSContext *cx, JS::HandleValue rval) {
   if (rval.isUndefined()) {
-    return new NoneType();
+    return NoneType::getPyObject();
   }
   else if (rval.isNull()) {
-    return new NullType();
+    return NullType::getPyObject();
   }
   else if (rval.isBoolean()) {
-    return new BoolType(rval.toBoolean());
+    return BoolType::getPyObject(rval.toBoolean());
   }
   else if (rval.isNumber()) {
-    return new FloatType(rval.toNumber());
+    return FloatType::getPyObject(rval.toNumber());
   }
   else if (rval.isString()) {
-    return new StrType(cx, rval.toString());
+    return StrType::getPyObject(cx, rval.toString());
   }
   else if (rval.isSymbol()) {
     printf("symbol type is not handled by PythonMonkey yet");
   }
   else if (rval.isBigInt()) {
-    return new IntType(cx, rval.toBigInt());
+    return IntType::getPyObject(cx, rval.toBigInt());
   }
   else if (rval.isObject()) {
     JS::Rooted<JSObject *> obj(cx);
     JS_ValueToObject(cx, rval, &obj);
+
     if (JS::GetClass(obj)->isProxyObject()) {
-      if (js::GetProxyHandler(obj)->family() == &PyDictProxyHandler::family) { // this is one of our proxies for python dicts
-        return new DictType(JS::GetMaybePtrFromReservedSlot<PyObject>(obj, PyObjectSlot));
-      }
-      if (js::GetProxyHandler(obj)->family() == &PyListProxyHandler::family) { // this is one of our proxies for python lists
-        return new ListType(JS::GetMaybePtrFromReservedSlot<PyObject>(obj, PyObjectSlot));
-      }
-      if (js::GetProxyHandler(obj)->family() == &PyObjectProxyHandler::family) { // this is one of our proxies for python objects
-        return new PyType(JS::GetMaybePtrFromReservedSlot<PyObject>(obj, PyObjectSlot));
+      if (js::GetProxyHandler(obj)->family() == &PyDictProxyHandler::family ||                // this is one of our proxies for python dicts
+          js::GetProxyHandler(obj)->family() == &PyListProxyHandler::family ||                // this is one of our proxies for python lists
+          js::GetProxyHandler(obj)->family() == &PyIterableProxyHandler::family ||            // this is one of our proxies for python iterables
+          js::GetProxyHandler(obj)->family() == &PyObjectProxyHandler::family) {              // this is one of our proxies for python objects
+
+        PyObject *pyObject = JS::GetMaybePtrFromReservedSlot<PyObject>(obj, PyObjectSlot);
+        Py_INCREF(pyObject);
+        return pyObject;
       }
     }
+
     js::ESClass cls;
     JS::GetBuiltinClass(cx, obj, &cls);
     if (JS_ObjectIsBoundFunction(obj)) {
       cls = js::ESClass::Function; // In SpiderMonkey 115 ESR, bound function is no longer a JSFunction but a js::BoundFunctionObject.
                                    // js::ESClass::Function only assigns to JSFunction objects by JS::GetBuiltinClass.
     }
+
     JS::RootedValue unboxed(cx);
     switch (cls) {
     case js::ESClass::Boolean:
     case js::ESClass::Number:
     case js::ESClass::BigInt:
     case js::ESClass::String:
       js::Unbox(cx, obj, &unboxed);
       return pyTypeFactory(cx, unboxed);
     case js::ESClass::Date:
-      return new DateType(cx, obj);
+      return DateType::getPyObject(cx, obj);
     case js::ESClass::Promise:
-      return new PromiseType(cx, obj);
+      return PromiseType::getPyObject(cx, obj);
     case js::ESClass::Error:
-      return new ExceptionType(cx, obj);
+      return ExceptionType::getPyObject(cx, obj);
     case js::ESClass::Function: {
-        PyObject *pyFunc;
-        FuncType *f;
         if (JS_IsNativeFunction(obj, callPyFunc)) { // It's a wrapped python function by us
           // Get the underlying python function from the 0th reserved slot
           JS::Value pyFuncVal = js::GetFunctionNativeReserved(obj, 0);
-          pyFunc = (PyObject *)(pyFuncVal.toPrivate());
-          f = new FuncType(pyFunc);
+          PyObject *pyFunc = (PyObject *)(pyFuncVal.toPrivate());
+          Py_INCREF(pyFunc);
+          return pyFunc;
         } else {
-          f = new FuncType(cx, rval);
+          return FuncType::getPyObject(cx, rval);
         }
-        return f;
       }
     case js::ESClass::Array:
-      return new ListType(cx, obj);
+      return ListType::getPyObject(cx, obj);
     default:
       if (BufferType::isSupportedJsTypes(obj)) { // TypedArray or ArrayBuffer
         // TODO (Tom Tang): ArrayBuffers have cls == js::ESClass::ArrayBuffer
-        return new BufferType(cx, obj);
+        return BufferType::getPyObject(cx, obj);
       }
     }
-    return new DictType(cx, rval);
+    return DictType::getPyObject(cx, rval);
   }
   else if (rval.isMagic()) {
     printf("magic type is not handled by PythonMonkey yet\n");
   }
 
   std::string errorString("pythonmonkey cannot yet convert Javascript value of: ");
   JS::RootedString str(cx, JS::ToString(cx, rval));
```

### Comparing `pythonmonkey-0.4.0/src/setSpiderMonkeyException.cc` & `pythonmonkey-0.6.0/src/setSpiderMonkeyException.cc`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
   outStrStream << reportBuilder.toStringResult().c_str() << "\n";
 
   if (printStack) {
     JS::RootedObject stackObj(cx, exceptionStack.stack());
     if (stackObj.get()) {
       JS::RootedString stackStr(cx);
       BuildStackString(cx, nullptr, stackObj, &stackStr, 2, js::StackFormat::SpiderMonkey);
-      outStrStream << "Stack Trace:\n" << StrType(cx, stackStr).getValue();
+      outStrStream << "Stack Trace:\n" << StrType::getValue(cx, stackStr);
     }
   }
 
   return PyUnicode_FromString(outStrStream.str().c_str());
 }
 
 void setSpiderMonkeyException(JSContext *cx) {
```

### Comparing `pythonmonkey-0.4.0/tests/js/collide.simple` & `pythonmonkey-0.6.0/tests/js/collide.simple`

 * *Files 3% similar despite different names*

```diff
@@ -2,19 +2,19 @@
  * @file        collide.simple
  *              Test to ensure require module identitifier collision that resolves both py and js
  *              modules correctly prefers py modules.
  * @author      Wes Garland <wes@distributive.network>
  * @date        Mar 2024
  */
 
-const { which } = require('./modules/collide')
+const { which } = require('./modules/collide');
 const whichjs = require('./modules/collide.js').which;
 const whichpy = require('./modules/collide.py').which;
 
 if (which !== 'python')
-  throw new Error(`python module was not preferred, got ${which} instead`)
+  throw new Error(`python module was not preferred, got ${which} instead`);
 
 if (whichpy !== 'python')
-  throw new Error(`python module was not explicitly loaded, got ${whichpy} instead`)
+  throw new Error(`python module was not explicitly loaded, got ${whichpy} instead`);
 
 if (whichjs !== 'javascript')
-  throw new Error(`javascript module was not explicitly loaded, got ${whichjs} instead`)
+  throw new Error(`javascript module was not explicitly loaded, got ${whichjs} instead`);
```

### Comparing `pythonmonkey-0.4.0/tests/js/commonjs-modules.bash` & `pythonmonkey-0.6.0/tests/js/commonjs-modules.bash`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.4.0/tests/js/console-methods.simple` & `pythonmonkey-0.6.0/tests/js/console-methods.simple`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.4.0/tests/js/console-smoke.simple` & `pythonmonkey-0.6.0/tests/js/console-smoke.simple`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.4.0/tests/js/console-stdio.bash` & `pythonmonkey-0.6.0/tests/js/console-stdio.bash`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.4.0/tests/js/console-this.simple` & `pythonmonkey-0.6.0/tests/js/console-this.simple`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.4.0/tests/js/eval-test.simple` & `pythonmonkey-0.6.0/tests/js/eval-test.simple`

 * *Files 4% similar despite different names*

```diff
@@ -8,11 +8,11 @@
 'use strict';
 
 python.exec(`
 import os
 
 globalThis = pm.eval('globalThis')
 globalThis.result = pm.eval(open(os.path.join(os.getcwd(), "tests", "js", "resources", "eval-test.js"), "rb"))
-`)
+`);
 
-if (result !== 18436572)
+if (globalThis.result !== 18436572)
   throw new Error('incorrect result from eval-test.js');
```

### Comparing `pythonmonkey-0.4.0/tests/js/is-compilable-unit.simple` & `pythonmonkey-0.6.0/tests/js/is-compilable-unit.simple`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.4.0/tests/js/js2py/array-change-index.simple` & `pythonmonkey-0.6.0/tests/js/js2py/array-change-index.simple`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 const numbers = [1,2,3,4,5,6,7,8,9];
 
 python.exec(`
 def setArrayAtIndex(array, index, new):
   array[1] = new # can't index "array" based on "index"... probably because index is a float. So just pass "1"
   return array
 `);
-const setArrayAtIndex = python.eval("setArrayAtIndex")
+const setArrayAtIndex = python.eval('setArrayAtIndex');
 const numbersBack = setArrayAtIndex(numbers, 1, 999);
 
 // check that the array data was modified by reference in python
 if (numbers[1] !== 999)
   throw new Error('array not modified by python');
 
 // check that the array we get from python is the same reference as defined in js
```

### Comparing `pythonmonkey-0.4.0/tests/js/js2py/arraybuffer.simple` & `pythonmonkey-0.6.0/tests/js/js2py/arraybuffer.simple`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.4.0/tests/js/js2py/bigint.simple` & `pythonmonkey-0.6.0/tests/js/js2py/bigint.simple`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.4.0/tests/js/js2py/boolean.simple` & `pythonmonkey-0.6.0/tests/js/js2py/boolean.simple`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.4.0/tests/js/js2py/datetime.simple` & `pythonmonkey-0.6.0/tests/js/js2py/datetime.simple`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.4.0/tests/js/js2py/datetime2.simple` & `pythonmonkey-0.6.0/tests/js/js2py/datetime2.simple`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.4.0/tests/js/js2py/error.simple` & `pythonmonkey-0.6.0/tests/js/js2py/error.simple`

 * *Files 4% similar despite different names*

```diff
@@ -7,42 +7,48 @@
  * @date        July 2023
  */
 'use strict';
 
 const throughJS = x => x; 
 let errorFlag = false;
 
-function tester(exceptionpy, exceptionjs) {
+function tester(exceptionpy, exceptionjs) 
+{
   if (!exceptionpy.toString() === exceptionjs.toString())
   {
     console.error('Expected\n', exceptionpy.toString(), '\nbut got\n', exceptionjs.toString());
     errorFlag = true;
-  } else {
+  }
+  else 
+  {
     console.log('pass -', exceptionpy.toString());
   }
 }
 
-function inbuiltError() {
-  const exceptionpy = python.eval(`Exception('I know Python!')`);
+function inbuiltError() 
+{
+  const exceptionpy = python.eval('Exception(\'I know Python!\')');
   const exceptionjs = throughJS(exceptionpy);
   tester(exceptionpy, exceptionjs);
 }
 
-function customError() {
+function customError() 
+{
   python.exec(
     `class IAmAnError(Exception):
       def __init__(self, message):            
         super().__init__(message)
     `
     );
-  const exceptionpy = python.eval(`IAmAnError('I know Python!')`);
+  const exceptionpy = python.eval('IAmAnError(\'I know Python!\')');
   const exceptionjs = throughJS(exceptionpy);
   tester(exceptionpy, exceptionjs);
 }
 
 inbuiltError();
 customError();
 
-if (errorFlag) {
+if (errorFlag) 
+{
   throw new Error('test failed');
 }
```

### Comparing `pythonmonkey-0.4.0/tests/js/js2py/function-curry.simple` & `pythonmonkey-0.6.0/tests/js/js2py/function-curry.simple`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 /**
  * @file        js2py/function-curry.simple
  *              Curries a function in JS, pass it to python, apply it in JS.
  * @author      Liang Wang, liang@distributive.network
  * @date        July 2023
  */
 
-'use strict'
-const curry = (fn) => {
-  return function curried(...args) {
-    if (args.length >= fn.length) {
-      return fn.apply(this, args);
-    } else {
-      return function(...args2) {
-        return curried.apply(this, args.concat(args2));
-      }
+'use strict';
+const curry = (fn) => 
+{
+  return function curried(...args) 
+  {
+    if (args.length >= fn.length) 
+    {
+      return fn.apply(null, args);
+    }
+    else 
+    {
+      return function(...args2) 
+      {
+        return curried.apply(null, args.concat(args2));
+      };
     }
   };
-}
+};
 
 const takeMiddle = (_x, y, _z) => y;
 
 const throughPython = python.eval('(lambda x: x)');
 const pTakeMiddle = throughPython(curry(takeMiddle));
 const middle = pTakeMiddle(1)(2)(3);
```

### Comparing `pythonmonkey-0.4.0/tests/js/js2py/higher-order-function.simple` & `pythonmonkey-0.6.0/tests/js/js2py/higher-order-function.simple`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.4.0/tests/js/js2py/object-mutation.simple` & `pythonmonkey-0.6.0/tests/js/js2py/object-mutation.simple`

 * *Files 27% similar despite different names*

```diff
@@ -13,25 +13,25 @@
 def change_and_return(obj):
   obj["a"] = 5;
   return obj;
 `;
 
 python.exec(pcode);
 
-const fun = python.eval("change_and_return");
+const fun = python.eval('change_and_return');
 const obj2 = fun(obj);
 
-if (obj.a !== 5 || obj2["a"] !== 5)
+if (obj.a !== 5 || obj2['a'] !== 5)
 {
   console.error('Object isn\'t sharing memory.');
   throw new Error('Test failed');
 }
 
 obj.a = 1000;
 
-if (obj.a !== 1000 || obj2["a"] !== 1000)
+if (obj.a !== 1000 || obj2['a'] !== 1000)
 {
   console.error('Object isn\'t sharing memory.');
   throw new Error('Test failed');
 }
 
 console.log('Test passed');
```

### Comparing `pythonmonkey-0.4.0/tests/js/js2py/object.simple` & `pythonmonkey-0.6.0/tests/js/js2py/object.simple`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.4.0/tests/js/js2py/promise-await-in-python.simple` & `pythonmonkey-0.6.0/tests/js/js2py/promise-await-in-python.simple`

 * *Files 18% similar despite different names*

```diff
@@ -2,32 +2,35 @@
  * @file        js2py/promise-await-in-python.simple
  *              Simple test to await a javascript promise as a python awaitable, resolving with the correct value.
  * @author      Ryan Saweczko ryansaweczko@distributive.network
  * @date        July 2023
  */
 'use strict';
 
-var resolve, reject;
+var resolve;
 var valToResolve = 1;
-const examplePromise = new Promise((res, rej) => {resolve = res, reject = rej});
+const examplePromise = new Promise((res, rej) => 
+{
+  resolve = res;
+});
 
 const pythonCode = `
 import asyncio
 
 async def awaitPromise(promise):
   ret = await promise
   return ret
 `;
 
 python.exec(pythonCode);
-const pythonFunction = python.eval("awaitPromise")
+const pythonFunction = python.eval('awaitPromise');
 
 async function test()
 {
   const backValue = await pythonFunction(examplePromise);
   if (backValue !== 1)
-    throw new Error(`Received value ${backValue} instead of ${valToResolve} from awaiting a JS promise in python`)
+    throw new Error(`Received value ${backValue} instead of ${valToResolve} from awaiting a JS promise in python`);
 }
-test()
+test();
 
 resolve(valToResolve);
```

### Comparing `pythonmonkey-0.4.0/tests/js/js2py/string.simple` & `pythonmonkey-0.6.0/tests/js/js2py/string.simple`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.4.0/tests/js/js2py/trivial-function.simple` & `pythonmonkey-0.6.0/tests/js/js2py/trivial-function.simple`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.4.0/tests/js/pmjs-eopt.bash` & `pythonmonkey-0.6.0/tests/js/pmjs-eopt.bash`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.4.0/tests/js/pmjs-global-arguments.bash` & `pythonmonkey-0.6.0/tests/js/pmjs-global-arguments.bash`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.4.0/tests/js/pmjs-interactive-smoke.bash` & `pythonmonkey-0.6.0/tests/js/pmjs-interactive-smoke.bash`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.4.0/tests/js/pmjs-popt.bash` & `pythonmonkey-0.6.0/tests/js/pmjs-popt.bash`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.4.0/tests/js/pmjs-require-cache.bash` & `pythonmonkey-0.6.0/tests/js/pmjs-require-cache.bash`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.4.0/tests/js/pmjs-ropt.bash` & `pythonmonkey-0.6.0/tests/js/pmjs-ropt.bash`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.4.0/tests/js/program-module.simple` & `pythonmonkey-0.6.0/tests/js/program-module.simple`

 * *Files 9% similar despite different names*

```diff
@@ -15,22 +15,22 @@
   console[facility](message + ':', testResult ? 'PASS' : 'FAIL');
   if (!testResult)
     failures++;    
 }
   
 check('require.main is an object',              typeof require.main === 'object');
 check('require.main is the current module',     require.main === module);
-check('require is the global require',          require === globalThis.require)
+check('require is the global require',          require === globalThis.require);
 check('exports is the global exports',          exports === globalThis.exports);
 check('module is the global module',            module  === globalThis.module);
 
 // eslint-disable-next-line no-global-assign
 module = {};
 check('free module symbol is global symbol',    module  === globalThis.module);
-check('arguments.length is ' + arguments.length, ...arguments)
+check('arguments.length is ' + arguments.length, ...arguments);
 
 if (failures)
   console.log(`${failures} sub-tests failing`);
 else
   console.log('all sub-tests pass', typeof failures);
 
 python.exit(failures);
```

### Comparing `pythonmonkey-0.4.0/tests/js/program.js` & `pythonmonkey-0.6.0/tests/js/program.js`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.4.0/tests/js/py2js/array-change-index.simple` & `pythonmonkey-0.6.0/tests/js/py2js/array-change-index.simple`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.4.0/tests/js/py2js/arraybuffer.simple` & `pythonmonkey-0.6.0/tests/js/py2js/arraybuffer.simple`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.4.0/tests/js/py2js/boolean.simple` & `pythonmonkey-0.6.0/tests/js/py2js/boolean.simple`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.4.0/tests/js/py2js/datetime.simple` & `pythonmonkey-0.6.0/tests/js/py2js/datetime.simple`

 * *Files 16% similar despite different names*

```diff
@@ -2,41 +2,41 @@
  * @file        py2js/datetime.simple.failing
  *              Simple test which shows that sending Python datetime.datetimes to JS and getting them back into
  *              Python works as expected
  * 
  * @author      Elijah Deluzio, elijah@distributive.network
  * @date        July 2023
  */
-'use strict'
+'use strict';
 
 const throughJS = x => x;
 var expectedJsTimestamp;
 var actualJsTimestamp;
 var jsDate;
 var pyDate;
 
 // Test 1: Date from timestamp of 0 (1970 - 01 - 01), timestamp = 0
 expectedJsTimestamp = 0;
-python.exec(`from datetime import timezone`)
-python.exec(`import datetime`);
+python.exec('from datetime import timezone');
+python.exec('import datetime');
 pyDate = python.eval(`datetime.datetime.fromtimestamp(${expectedJsTimestamp}, tz=timezone.utc)`);
 jsDate = throughJS(pyDate);
 
 if (jsDate.getTime() !== expectedJsTimestamp)
 {
   console.error('expected', expectedJsTimestamp, 'but got', jsDate.getTime());
   throw new Error('test failed');
 }
 
 console.log('pass -', jsDate);
 
 // Test 2: Date from 21st century (2222 - 02 - 03), timestamp = 7955193600
 expectedJsTimestamp = 7955193600;
-python.exec(`from datetime import timezone`)
-python.exec(`import datetime`);
+python.exec('from datetime import timezone');
+python.exec('import datetime');
 pyDate = python.eval(`datetime.datetime.fromtimestamp(${expectedJsTimestamp}, tz=timezone.utc)`);
 jsDate = throughJS(pyDate);
 
 actualJsTimestamp = jsDate.getTime() / 1000; // JS timestamp is in milliseconds, convert it to seconds
 if (actualJsTimestamp !== expectedJsTimestamp)
 {
   console.error('expected', expectedJsTimestamp, 'but got', actualJsTimestamp);
```

### Comparing `pythonmonkey-0.4.0/tests/js/py2js/error.simple` & `pythonmonkey-0.6.0/tests/js/py2js/error.simple`

 * *Files 19% similar despite different names*

```diff
@@ -4,23 +4,26 @@
  *              There will be a lossful conversion of error properties from JS to Py.
  * 
  * @author      David Courtis, david@distributive.network
  * @date        July 2023
  */
 'use strict';
 
-class RandomError extends Error {
-  constructor(message) {
+class RandomError extends Error 
+{
+  constructor(message) 
+  {
     super(message);
   }
 }
 
-const exceptionjs = new RandomError("I was created!");
+const exceptionjs = new RandomError('I was created!');
 const throughPython = python.eval('(lambda x: x)');
 const exceptionpy = throughPython(exceptionjs);
 
-if (!exceptionpy.toString().includes(exceptionjs.toString())) {
+if (!exceptionpy.toString().includes(exceptionjs.toString())) 
+{
   console.error('Expected\n', exceptionjs.toString(), '\nbut got\n', exceptionpy.toString());
   throw new Error('test failed');
 }
 
 console.log('pass -', exceptionjs);
```

### Comparing `pythonmonkey-0.4.0/tests/js/py2js/function-curry.simple.failing` & `pythonmonkey-0.6.0/tests/js/py2js/function-curry.simple.failing`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.4.0/tests/js/py2js/higher-order-function.simple` & `pythonmonkey-0.6.0/tests/js/py2js/higher-order-function.simple`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.4.0/tests/js/py2js/integer.simple` & `pythonmonkey-0.6.0/tests/js/py2js/integer.simple`

 * *Files 26% similar despite different names*

```diff
@@ -11,12 +11,12 @@
 if (typeof number !== 'number')
 {
   console.error(`expected number but got ${typeof number}`);
   throw new Error('test failed');
 }
 if (number !== 777)
 {
-  console.error(`expected ${777} but got ${bigint}`);
+  console.error(`expected ${777} but got ${number}`);
   throw new Error('test failed');
 }
 
 console.log('pass -', number);
```

### Comparing `pythonmonkey-0.4.0/tests/js/py2js/object-methods.simple` & `pythonmonkey-0.6.0/tests/js/py2js/object-methods.simple`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.4.0/tests/js/py2js/object.simple` & `pythonmonkey-0.6.0/tests/js/py2js/object.simple`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.4.0/tests/js/py2js/promise.simple.failing` & `pythonmonkey-0.6.0/tests/js/py2js/promise.simple.failing`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.4.0/tests/js/py2js/string.simple` & `pythonmonkey-0.6.0/tests/js/py2js/string.simple`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.4.0/tests/js/quint.js` & `pythonmonkey-0.6.0/tests/js/quint.js`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.4.0/tests/js/require-module-stack.bash.failing` & `pythonmonkey-0.6.0/tests/js/require-module-stack.bash.failing`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.4.0/tests/js/set-timeout.simple` & `pythonmonkey-0.6.0/tests/js/set-timeout.simple`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  * - must fire later than 100ms
  * - must fire before 10s
  * - 10s is well before 100s but very CI-load-tolerant; the idea is not to check for accurancy, but
  *  rather ensure we haven't mixed up seconds and milliseconds somewhere.
  */
 function check100ms()
 {
-  end = time();
+  let end = time();
 
   if (end - start < 0.1)
     throw new Error('timer fired too soon');
   if (end - start > 10)
     throw new Error('timer fired too late');
 
   console.log('done - timer fired after ', (end-start) * 1000, 'ms');
```

### Comparing `pythonmonkey-0.4.0/tests/js/typeofs-segfaults.simple.failing` & `pythonmonkey-0.6.0/tests/js/typeofs-segfaults.simple.failing`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.4.0/tests/js/url-search-params.simple` & `pythonmonkey-0.6.0/tests/js/url-search-params.simple`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,16 @@
  */
 
 const DESCRIPTORS = true;
 const NODE = false;
 
 const { getPrototypeOf, getOwnPropertyDescriptor } = Object;
 
-QUnit.test('URLSearchParams', assert => {
+QUnit.test('URLSearchParams', assert => 
+{
   assert.isFunction(URLSearchParams);
   assert.arity(URLSearchParams, 0);
   assert.name(URLSearchParams, 'URLSearchParams');
   if (!NODE) assert.looksNative(URLSearchParams);
 
   assert.same(String(new URLSearchParams()), '');
   assert.same(String(new URLSearchParams('')), '');
@@ -120,46 +121,53 @@
     { input: { '+': '%C2' }, output: [['+', '%C2']], name: 'object with +' },
     { input: { c: 'x', a: '?' }, output: [['c', 'x'], ['a', '?']], name: 'object with two keys' },
     { input: [['c', 'x'], ['a', '?']], output: [['c', 'x'], ['a', '?']], name: 'array with two keys' },
     // eslint-disable-next-line max-len -- ignore
     // !!! { input: { 'a\0b': '42', 'c\uD83D': '23', dሴ: 'foo' }, output: [['a\0b', '42'], ['c\uFFFD', '23'], ['d\u1234', 'foo']], name: 'object with NULL, non-ASCII, and surrogate keys' },
   ];
 
-  for (const { input, output, name } of testData) {
+  for (const { input, output, name } of testData) 
+  {
     params = new URLSearchParams(input);
     let i = 0;
-    params.forEach((value, key) => {
+    params.forEach((value, key) => 
+    {
       const [reqKey, reqValue] = output[i++];
       assert.same(key, reqKey, `construct with ${ name }`);
       assert.same(value, reqValue, `construct with ${ name }`);
     });
   }
 
-  assert.throws(() => {
+  assert.throws(() => 
+  {
+    // eslint-disable-next-line new-cap
     URLSearchParams('');
   }, 'TypeError: Incorrect invocation'); // throws w/o `new`
 
-  assert.throws(() => {
+  assert.throws(() => 
+  {
     new URLSearchParams([[1, 2, 3]]);
   }, 'TypeError: Expected sequence with length 2');
 
   // assert.throws(() => {
   //   new URLSearchParams([createIterable([createIterable([1, 2, 3])])]);
   // }, 'sequence elements must be pairs #2');
 
-  assert.throws(() => {
+  assert.throws(() => 
+  {
     new URLSearchParams([[1]]);
   }, 'TypeError: Expected sequence with length 2');
 
   // assert.throws(() => {
   //   new URLSearchParams([createIterable([createIterable([1])])]);
   // }, 'sequence elements must be pairs #4');
 });
 
-QUnit.test('URLSearchParams#append', assert => {
+QUnit.test('URLSearchParams#append', assert => 
+{
   const { append } = URLSearchParams.prototype;
   assert.isFunction(append);
   assert.arity(append, 2);
   assert.name(append, 'append');
   assert.enumerable(URLSearchParams.prototype, 'append');
   if (!NODE) assert.looksNative(append);
 
@@ -199,20 +207,22 @@
   assert.true(params.has('first'), 'search params object has name "first"');
   assert.same(params.get('first'), '1', 'search params object has name "first" with value "1"');
   assert.same(params.get('second'), '2', 'search params object has name "second" with value "2"');
   assert.same(params.get('third'), '', 'search params object has name "third" with value ""');
   params.append('first', 10);
   assert.same(params.get('first'), '1', 'search params object has name "first" with value "1"');
 
-  assert.throws(() => {
+  assert.throws(() => 
+  {
     return new URLSearchParams('').append();
   }, 'TypeError: Not enough arguments'); // throws w/o arguments
 });
 
-QUnit.test('URLSearchParams#delete', assert => {
+QUnit.test('URLSearchParams#delete', assert => 
+{
   const $delete = URLSearchParams.prototype.delete;
   assert.isFunction($delete);
   assert.arity($delete, 1);
   assert.enumerable(URLSearchParams.prototype, 'delete');
   if (!NODE) assert.looksNative($delete);
 
   let params = new URLSearchParams('a=b&c=d');
@@ -254,33 +264,36 @@
   params.delete('a', null);
   assert.same(String(params), 'a=1&a=2&a=3&b=4');
 
   params = new URLSearchParams('a=1&a=2&a=null&a=3&b=4');
   params.delete('a', undefined);
   assert.same(String(params), 'b=4');
 
-  if (DESCRIPTORS) {
+  if (DESCRIPTORS) 
+  {
     let url = new URL('http://example.com/?param1&param2');
     url.searchParams.delete('param1');
     url.searchParams.delete('param2');
     assert.same(String(url), 'http://example.com/', 'url.href does not have ?');
     assert.same(url.search, '', 'url.search does not have ?');
 
     url = new URL('http://example.com/?');
     url.searchParams.delete('param1');
     // assert.same(String(url), 'http://example.com/', 'url.href does not have ?'); // Safari bug
     assert.same(url.search, '', 'url.search does not have ?');
   }
 
-  assert.throws(() => {
+  assert.throws(() => 
+  {
     return new URLSearchParams('').delete();
   }, 'TypeError: Not enough arguments');
 });
 
-QUnit.test('URLSearchParams#get', assert => {
+QUnit.test('URLSearchParams#get', assert => 
+{
   const { get } = URLSearchParams.prototype;
   assert.isFunction(get);
   assert.arity(get, 1);
   assert.name(get, 'get');
   assert.enumerable(URLSearchParams.prototype, 'get');
   if (!NODE) assert.looksNative(get);
 
@@ -334,20 +347,22 @@
   assert.same(new URLSearchParams('a\uD83D\uDCA9b=c').get('a\uD83D\uDCA9b'), 'c', 'parse \\uD83D\\uDCA9');
 
   assert.same(new URLSearchParams('a=b%f0%9f%92%a9c').get('a'), 'b\uD83D\uDCA9c', 'parse %f0%9f%92%a9');
   assert.same(new URLSearchParams('a%f0%9f%92%a9b=c').get('a\uD83D\uDCA9b'), 'c', 'parse %f0%9f%92%a9');
 
   assert.same(new URLSearchParams('=').get(''), '', 'parse =');
 
-  assert.throws(() => {
+  assert.throws(() => 
+  {
     return new URLSearchParams('').get();
   }, 'TypeError: Not enough arguments');
 });
 
-QUnit.test('URLSearchParams#getAll', assert => {
+QUnit.test('URLSearchParams#getAll', assert => 
+{
   const { getAll } = URLSearchParams.prototype;
   assert.isFunction(getAll);
   assert.arity(getAll, 1);
   assert.name(getAll, 'getAll');
   assert.enumerable(URLSearchParams.prototype, 'getAll');
   if (!NODE) assert.looksNative(getAll);
 
@@ -366,20 +381,22 @@
   assert.arrayEqual(params.getAll('a'), ['', 'e']);
 
   params = new URLSearchParams('a=1&a=2&a=3&a');
   assert.arrayEqual(params.getAll('a'), ['1', '2', '3', ''], 'search params object has expected name "a" values');
   params.set('a', 'one');
   assert.arrayEqual(params.getAll('a'), ['one'], 'search params object has expected name "a" values');
 
-  assert.throws(() => {
+  assert.throws(() => 
+  {
     return new URLSearchParams('').getAll();
   }, 'TypeError: Not enough arguments');
 });
 
-QUnit.test('URLSearchParams#has', assert => {
+QUnit.test('URLSearchParams#has', assert => 
+{
   const { has } = URLSearchParams.prototype;
   assert.isFunction(has);
   assert.arity(has, 1);
   assert.name(has, 'has');
   assert.enumerable(URLSearchParams.prototype, 'has');
   if (!NODE) assert.looksNative(has);
 
@@ -412,20 +429,22 @@
   assert.true(params.has('a', null));
   assert.false(params.has('a', 4));
   assert.true(params.has('b', 4));
   assert.false(params.has('b', null));
   assert.true(params.has('b', undefined));
   assert.false(params.has('c', undefined));
 
-  assert.throws(() => {
+  assert.throws(() => 
+  {
     return new URLSearchParams('').has();
   }, 'TypeError: Not enough arguments');
 });
 
-QUnit.test('URLSearchParams#set', assert => {
+QUnit.test('URLSearchParams#set', assert => 
+{
   const { set } = URLSearchParams.prototype;
   assert.isFunction(set);
   assert.arity(set, 2);
   assert.name(set, 'set');
   assert.enumerable(URLSearchParams.prototype, 'set');
   if (!NODE) assert.looksNative(set);
 
@@ -447,20 +466,22 @@
   assert.same(params.get('a'), '1', 'search params object has name "a" with value "1"');
   assert.same(String(params), 'a=1&a=2&a=3&first=4');
   params.set('a', 4);
   assert.true(params.has('a'), 'search params object has name "a"');
   assert.same(params.get('a'), '4', 'search params object has name "a" with value "4"');
   assert.same(String(params), 'a=4&first=4');
 
-  assert.throws(() => {
+  assert.throws(() => 
+  {
     return new URLSearchParams('').set();
   }, 'TypeError: Not enough arguments');
 });
 
-QUnit.test('URLSearchParams#sort', assert => {
+QUnit.test('URLSearchParams#sort', assert => 
+{
   const { sort } = URLSearchParams.prototype;
   assert.isFunction(sort);
   assert.arity(sort, 0);
   assert.name(sort, 'sort');
   assert.enumerable(URLSearchParams.prototype, 'sort');
   if (!NODE) assert.looksNative(sort);
 
@@ -519,44 +540,49 @@
     },
     {
       input: 'a🌈&a💩',
       output: [['a🌈', ''], ['a💩', '']],
     },
   ];
 
-  for (const { input, output } of testData) {
+  for (const { input, output } of testData) 
+  {
     let i = 0;
     params = new URLSearchParams(input);
     params.sort();
-    params.forEach((value, key) => {
+    params.forEach((value, key) => 
+    {
       const [reqKey, reqValue] = output[i++];
       assert.same(key, reqKey);
       assert.same(value, reqValue);
     });
 
     i = 0;
     const url = new URL(`?${ input }`, 'https://example/');
     params = url.searchParams;
     params.sort();
-    params.forEach((value, key) => {
+    params.forEach((value, key) => 
+    {
       const [reqKey, reqValue] = output[i++];
       assert.same(key, reqKey);
       assert.same(value, reqValue);
     });
   }
 
-  if (DESCRIPTORS) {
+  if (DESCRIPTORS) 
+  {
     const url = new URL('http://example.com/?');
     url.searchParams.sort();
     assert.same(url.href, 'http://example.com/', 'Sorting non-existent params removes ? from URL');
     assert.same(url.search, '', 'Sorting non-existent params removes ? from URL');
   }
 });
 
-QUnit.test('URLSearchParams#toString', assert => {
+QUnit.test('URLSearchParams#toString', assert => 
+{
   const { toString } = URLSearchParams.prototype;
   assert.isFunction(toString);
   assert.arity(toString, 0);
   assert.name(toString, 'toString');
   if (!NODE) assert.looksNative(toString);
 
   let params = new URLSearchParams();
@@ -646,276 +672,308 @@
   assert.same(String(params), 'a=b&c=d&e=');
   params = new URLSearchParams('a = b &a=b&c=d%20');
   assert.same(String(params), 'a+=+b+&a=b&c=d+');
   params = new URLSearchParams('a=&a=b');
   assert.same(String(params), 'a=&a=b');
 });
 
-QUnit.test('URLSearchParams#forEach', assert => {
+QUnit.test('URLSearchParams#forEach', assert => 
+{
   const { forEach } = URLSearchParams.prototype;
   assert.isFunction(forEach);
   assert.arity(forEach, 1);
   assert.name(forEach, 'forEach');
   assert.enumerable(URLSearchParams.prototype, 'forEach');
   if (!NODE) assert.looksNative(forEach);
 
   const expectedValues = { a: '1', b: '2', c: '3' };
   let params = new URLSearchParams('a=1&b=2&c=3');
   let result = '';
-  params.forEach((value, key, that) => {
+  params.forEach((value, key, that) => 
+  {
     assert.same(params.get(key), expectedValues[key]);
     assert.same(value, expectedValues[key]);
     assert.same(that, params);
     result += key;
   });
   assert.same(result, 'abc');
 
-  new URL('http://a.b/c').searchParams.forEach(() => {
+  new URL('http://a.b/c').searchParams.forEach(() => 
+  {
     assert.avoid();
   });
 
   // fails in Chrome 66-
-  if (DESCRIPTORS) {
+  if (DESCRIPTORS) 
+  {
     const url = new URL('http://a.b/c?a=1&b=2&c=3&d=4');
     params = url.searchParams;
     result = '';
-    params.forEach((val, key) => {
+    params.forEach((val, key) => 
+    {
       url.search = 'x=1&y=2&z=3';
       result += key + val;
     });
     assert.same(result, 'a1y2z3');
   }
 
   // fails in Chrome 66-
   params = new URLSearchParams('a=1&b=2&c=3');
   result = '';
-  params.forEach((value, key) => {
+  params.forEach((value, key) => 
+  {
     params.delete('b');
     result += key + value;
   });
   assert.same(result, 'a1c3');
 });
 
-QUnit.test('URLSearchParams#entries', assert => {
+QUnit.test('URLSearchParams#entries', assert => 
+{
   const { entries } = URLSearchParams.prototype;
   assert.isFunction(entries);
   assert.arity(entries, 0);
   assert.name(entries, 'entries');
   assert.enumerable(URLSearchParams.prototype, 'entries');
   if (!NODE) assert.looksNative(entries);
 
   const expectedValues = { a: '1', b: '2', c: '3' };
   let params = new URLSearchParams('a=1&b=2&c=3');
   let iterator = params.entries();
   let result = '';
   let entry;
-  while (!(entry = iterator.next()).done) {
+  while (!(entry = iterator.next()).done) 
+  {
     const [key, value] = entry.value;
     assert.same(params.get(key), expectedValues[key]);
     assert.same(value, expectedValues[key]);
     result += key;
   }
   assert.same(result, 'abc');
 
   assert.true(new URL('http://a.b/c').searchParams.entries().next().done, 'should be finished');
 
   // fails in Chrome 66-
-  if (DESCRIPTORS) {
+  if (DESCRIPTORS) 
+  {
     const url = new URL('http://a.b/c?a=1&b=2&c=3&d=4');
     iterator = url.searchParams.entries();
     result = '';
-    while (!(entry = iterator.next()).done) {
+    while (!(entry = iterator.next()).done) 
+    {
       const [key, value] = entry.value;
       url.search = 'x=1&y=2&z=3';
       result += key + value;
     }
     assert.same(result, 'a1y2z3');
   }
 
   // fails in Chrome 66-
   params = new URLSearchParams('a=1&b=2&c=3');
   iterator = params.entries();
   result = '';
-  while (!(entry = iterator.next()).done) {
+  while (!(entry = iterator.next()).done) 
+  {
     params.delete('b');
     const [key, value] = entry.value;
     result += key + value;
   }
   assert.same(result, 'a1c3');
 
   if (DESCRIPTORS) assert.true(getOwnPropertyDescriptor(getPrototypeOf(new URLSearchParams().entries()), 'next').enumerable, 'enumerable .next');
 });
 
-QUnit.test('URLSearchParams#keys', assert => {
+QUnit.test('URLSearchParams#keys', assert => 
+{
   const { keys } = URLSearchParams.prototype;
   assert.isFunction(keys);
   assert.arity(keys, 0);
   assert.name(keys, 'keys');
   assert.enumerable(URLSearchParams.prototype, 'keys');
   if (!NODE) assert.looksNative(keys);
 
   let iterator = new URLSearchParams('a=1&b=2&c=3').keys();
   let result = '';
   let entry;
-  while (!(entry = iterator.next()).done) {
+  while (!(entry = iterator.next()).done) 
+  {
     result += entry.value;
   }
   assert.same(result, 'abc');
 
   assert.true(new URL('http://a.b/c').searchParams.keys().next().done, 'should be finished');
 
   // fails in Chrome 66-
-  if (DESCRIPTORS) {
+  if (DESCRIPTORS) 
+  {
     const url = new URL('http://a.b/c?a=1&b=2&c=3&d=4');
     iterator = url.searchParams.keys();
     result = '';
-    while (!(entry = iterator.next()).done) {
+    while (!(entry = iterator.next()).done) 
+    {
       const key = entry.value;
       url.search = 'x=1&y=2&z=3';
       result += key;
     }
     assert.same(result, 'ayz');
   }
 
   // fails in Chrome 66-
   const params = new URLSearchParams('a=1&b=2&c=3');
   iterator = params.keys();
   result = '';
-  while (!(entry = iterator.next()).done) {
+  while (!(entry = iterator.next()).done) 
+  {
     params.delete('b');
     const key = entry.value;
     result += key;
   }
   assert.same(result, 'ac');
 
   if (DESCRIPTORS) assert.true(getOwnPropertyDescriptor(getPrototypeOf(new URLSearchParams().keys()), 'next').enumerable, 'enumerable .next');
 });
 
-QUnit.test('URLSearchParams#values', assert => {
+QUnit.test('URLSearchParams#values', assert => 
+{
   const { values } = URLSearchParams.prototype;
   assert.isFunction(values);
   assert.arity(values, 0);
   assert.name(values, 'values');
   assert.enumerable(URLSearchParams.prototype, 'values');
   if (!NODE) assert.looksNative(values);
 
   let iterator = new URLSearchParams('a=1&b=2&c=3').values();
   let result = '';
   let entry;
-  while (!(entry = iterator.next()).done) {
+  while (!(entry = iterator.next()).done) 
+  {
     result += entry.value;
   }
   assert.same(result, '123');
 
   assert.true(new URL('http://a.b/c').searchParams.values().next().done, 'should be finished');
 
   // fails in Chrome 66-
-  if (DESCRIPTORS) {
+  if (DESCRIPTORS) 
+  {
     const url = new URL('http://a.b/c?a=a&b=b&c=c&d=d');
     iterator = url.searchParams.keys();
     result = '';
-    while (!(entry = iterator.next()).done) {
+    while (!(entry = iterator.next()).done) 
+    {
       const { value } = entry;
       url.search = 'x=x&y=y&z=z';
       result += value;
     }
     assert.same(result, 'ayz');
   }
 
   // fails in Chrome 66-
   const params = new URLSearchParams('a=1&b=2&c=3');
   iterator = params.values();
   result = '';
-  while (!(entry = iterator.next()).done) {
+  while (!(entry = iterator.next()).done) 
+  {
     params.delete('b');
     const key = entry.value;
     result += key;
   }
   assert.same(result, '13');
 
   if (DESCRIPTORS) assert.true(getOwnPropertyDescriptor(getPrototypeOf(new URLSearchParams().values()), 'next').enumerable, 'enumerable .next');
 });
 
-QUnit.test('URLSearchParams#@@iterator', assert => {
+QUnit.test('URLSearchParams#@@iterator', assert => 
+{
   const entries = URLSearchParams.prototype[Symbol.iterator];
   assert.isFunction(entries);
   assert.arity(entries, 0);
   assert.name(entries, 'entries');
   if (!NODE) assert.looksNative(entries);
 
   assert.same(entries, URLSearchParams.prototype.entries);
 
   const expectedValues = { a: '1', b: '2', c: '3' };
   let params = new URLSearchParams('a=1&b=2&c=3');
   let iterator = params[Symbol.iterator]();
   let result = '';
   let entry;
-  while (!(entry = iterator.next()).done) {
+  while (!(entry = iterator.next()).done) 
+  {
     const [key, value] = entry.value;
     assert.same(params.get(key), expectedValues[key]);
     assert.same(value, expectedValues[key]);
     result += key;
   }
   assert.same(result, 'abc');
 
   assert.true(new URL('http://a.b/c').searchParams[Symbol.iterator]().next().done, 'should be finished');
 
   // fails in Chrome 66-
-  if (DESCRIPTORS) {
+  if (DESCRIPTORS) 
+  {
     const url = new URL('http://a.b/c?a=1&b=2&c=3&d=4');
     iterator = url.searchParams[Symbol.iterator]();
     result = '';
-    while (!(entry = iterator.next()).done) {
+    while (!(entry = iterator.next()).done) 
+    {
       const [key, value] = entry.value;
       url.search = 'x=1&y=2&z=3';
       result += key + value;
     }
     assert.same(result, 'a1y2z3');
   }
 
   // fails in Chrome 66-
   params = new URLSearchParams('a=1&b=2&c=3');
   iterator = params[Symbol.iterator]();
   result = '';
-  while (!(entry = iterator.next()).done) {
+  while (!(entry = iterator.next()).done) 
+  {
     params.delete('b');
     const [key, value] = entry.value;
     result += key + value;
   }
   assert.same(result, 'a1c3');
 
   if (DESCRIPTORS) assert.true(getOwnPropertyDescriptor(getPrototypeOf(new URLSearchParams()[Symbol.iterator]()), 'next').enumerable, 'enumerable .next');
 });
 
-QUnit.test('URLSearchParams#size', assert => {
+QUnit.test('URLSearchParams#size', assert => 
+{
   const params = new URLSearchParams('a=1&b=2&b=3');
   assert.true('size' in params);
   assert.same(params.size, 3);
 
-  if (DESCRIPTORS) {
+  if (DESCRIPTORS) 
+  {
     assert.true('size' in URLSearchParams.prototype);
 
     const { enumerable, configurable, get } = getOwnPropertyDescriptor(URLSearchParams.prototype, 'size');
 
     assert.true(enumerable, 'enumerable');
     assert.true(configurable, 'configurable');
 
     if (!NODE) assert.looksNative(get);
 
     assert.throws(() => get.call([]), 'TypeError: Incompatible receiver, URLSearchParams required');
   }
 });
 
-QUnit.test('URLSearchParams#@@toStringTag', assert => {
+QUnit.test('URLSearchParams#@@toStringTag', assert => 
+{
   const params = new URLSearchParams('a=b');
   assert.same(({}).toString.call(params), '[object URLSearchParams]');
 });
 
-if (typeof Request == 'function') {
-  QUnit.test('URLSearchParams with Request', assert => {
+if (typeof Request === 'function') 
+{
+  QUnit.test('URLSearchParams with Request', assert => 
+  {
     const async = assert.async();
-    new Request('http://zloirock.ru', { body: new URLSearchParams({ foo: 'baz' }), method: 'POST' }).text().then(text => {
+    new Request('http://zloirock.ru', { body: new URLSearchParams({ foo: 'baz' }), method: 'POST' }).text().then(text => 
+    {
       assert.same(text, 'foo=baz');
       async();
     });
   });
 }
```

### Comparing `pythonmonkey-0.4.0/tests/js/url.simple` & `pythonmonkey-0.6.0/tests/js/url.simple`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,16 @@
  */
 
 const DESCRIPTORS = true;
 const NODE = false;
 
 const { hasOwnProperty } = Object.prototype;
 
-QUnit.test('URL constructor', assert => {
+QUnit.test('URL constructor', assert => 
+{
   assert.isFunction(URL);
   if (!NODE) assert.arity(URL, 1);
   assert.name(URL, 'URL');
   if (!NODE) assert.looksNative(URL);
 
   assert.same(String(new URL('http://www.domain.com/a/b')), 'http://www.domain.com/a/b');
   assert.same(String(new URL('/c/d', 'http://www.domain.com/a/b')), 'http://www.domain.com/c/d');
@@ -63,29 +64,32 @@
   assert.throws(() => new URL('//abc', null), 'TypeError: Invalid scheme');
   assert.throws(() => new URL('http://[20:0:0:1:0:0:0:ff'), 'TypeError: Invalid host');
   assert.throws(() => new URL('http://[20:0:0:1:0:0:0:fg]'), 'TypeError: Invalid host');
   // assert.throws(() => new URL('http://a%b'), 'forbidden host code point'); // no error in FF
   assert.throws(() => new URL('1http://zloirock.ru'), 'TypeError: Invalid scheme');
 });
 
-QUnit.test('URL#href', assert => {
+QUnit.test('URL#href', assert => 
+{
   let url = new URL('http://zloirock.ru/');
 
-  if (DESCRIPTORS) {
+  if (DESCRIPTORS) 
+  {
     assert.false(hasOwnProperty.call(url, 'href'));
     const descriptor = Object.getOwnPropertyDescriptor(URL.prototype, 'href');
     assert.true(descriptor.enumerable);
     assert.true(descriptor.configurable);
     assert.same(typeof descriptor.get, 'function');
     assert.same(typeof descriptor.set, 'function');
   }
 
   assert.same(url.href, 'http://zloirock.ru/');
 
-  if (DESCRIPTORS) {
+  if (DESCRIPTORS) 
+  {
     url.searchParams.append('foo', 'bar');
     assert.same(url.href, 'http://zloirock.ru/?foo=bar');
 
     url = new URL('http://zloirock.ru/foo');
     url.href = 'https://測試';
     assert.same(url.href, 'https://xn--g6w251d/', 'unicode parsing');
     assert.same(String(url), 'https://xn--g6w251d/', 'unicode parsing');
@@ -139,45 +143,50 @@
     // assert.throws(() => new URL('http://zloirock.ru/').href = 'http://[20:0:0:1:0:0:0:ff', 'incorrect IPv6'); // no error in Chrome
     // assert.throws(() => new URL('http://zloirock.ru/').href = 'http://[20:0:0:1:0:0:0:fg]', 'incorrect IPv6'); // no error in Chrome
     // assert.throws(() => new URL('http://zloirock.ru/').href = 'http://a%b', 'forbidden host code point'); // no error in Chrome and FF
     // assert.throws(() => new URL('http://zloirock.ru/').href = '1http://zloirock.ru', 'incorrect scheme'); // no error in Chrome
   }
 });
 
-QUnit.test('URL#origin', assert => {
+QUnit.test('URL#origin', assert => 
+{
   const url = new URL('http://es6.zloirock.ru/tests.html');
 
-  if (DESCRIPTORS) {
+  if (DESCRIPTORS) 
+  {
     assert.false(hasOwnProperty.call(url, 'origin'));
     const descriptor = Object.getOwnPropertyDescriptor(URL.prototype, 'origin');
     assert.true(descriptor.enumerable);
     assert.true(descriptor.configurable);
     assert.same(typeof descriptor.get, 'function');
   }
 
   assert.same(url.origin, 'http://es6.zloirock.ru');
 
   assert.same(new URL('https://測試/tests').origin, 'https://xn--g6w251d');
 });
 
-QUnit.test('URL#protocol', assert => {
+QUnit.test('URL#protocol', assert => 
+{
   let url = new URL('http://zloirock.ru/');
 
-  if (DESCRIPTORS) {
+  if (DESCRIPTORS) 
+  {
     assert.false(hasOwnProperty.call(url, 'protocol'));
     const descriptor = Object.getOwnPropertyDescriptor(URL.prototype, 'protocol');
     assert.true(descriptor.enumerable);
     assert.true(descriptor.configurable);
     assert.same(typeof descriptor.get, 'function');
     assert.same(typeof descriptor.set, 'function');
   }
 
   assert.same(url.protocol, 'http:');
 
-  if (DESCRIPTORS) {
+  if (DESCRIPTORS) 
+  {
     url = new URL('http://zloirock.ru/');
     url.protocol = 'https';
     assert.same(url.protocol, 'https:');
     assert.same(String(url), 'https://zloirock.ru/');
 
     // https://nodejs.org/api/url.html#url_special_schemes
     // url = new URL('http://zloirock.ru/');
@@ -190,43 +199,48 @@
     url.protocol = '1http';
     assert.same(url.protocol, 'http:');
     assert.same(url.href, 'http://zloirock.ru/', 'incorrect scheme');
     assert.same(String(url), 'http://zloirock.ru/', 'incorrect scheme');
   }
 });
 
-QUnit.test('URL#username', assert => {
+QUnit.test('URL#username', assert => 
+{
   let url = new URL('http://zloirock.ru/');
 
-  if (DESCRIPTORS) {
+  if (DESCRIPTORS) 
+  {
     assert.false(hasOwnProperty.call(url, 'username'));
     const descriptor = Object.getOwnPropertyDescriptor(URL.prototype, 'username');
     assert.true(descriptor.enumerable);
     assert.true(descriptor.configurable);
     assert.same(typeof descriptor.get, 'function');
     assert.same(typeof descriptor.set, 'function');
   }
 
   assert.same(url.username, '');
 
   url = new URL('http://username@zloirock.ru/');
   assert.same(url.username, 'username');
 
-  if (DESCRIPTORS) {
+  if (DESCRIPTORS) 
+  {
     url = new URL('http://zloirock.ru/');
     url.username = 'username';
     assert.same(url.username, 'username');
     assert.same(String(url), 'http://username@zloirock.ru/');
   }
 });
 
-QUnit.test('URL#password', assert => {
+QUnit.test('URL#password', assert => 
+{
   let url = new URL('http://zloirock.ru/');
 
-  if (DESCRIPTORS) {
+  if (DESCRIPTORS) 
+  {
     assert.false(hasOwnProperty.call(url, 'password'));
     const descriptor = Object.getOwnPropertyDescriptor(URL.prototype, 'password');
     assert.true(descriptor.enumerable);
     assert.true(descriptor.configurable);
     assert.same(typeof descriptor.get, 'function');
     assert.same(typeof descriptor.set, 'function');
   }
@@ -235,43 +249,47 @@
 
   url = new URL('http://username:password@zloirock.ru/');
   assert.same(url.password, 'password');
 
   // url = new URL('http://:password@zloirock.ru/'); // TypeError in FF
   // assert.same(url.password, 'password');
 
-  if (DESCRIPTORS) {
+  if (DESCRIPTORS) 
+  {
     url = new URL('http://zloirock.ru/');
     url.username = 'username';
     url.password = 'password';
     assert.same(url.password, 'password');
     assert.same(String(url), 'http://username:password@zloirock.ru/');
 
     // url = new URL('http://zloirock.ru/');
     // url.password = 'password';
     // assert.same(url.password, 'password'); // '' in FF
     // assert.same(String(url), 'http://:password@zloirock.ru/'); // 'http://zloirock.ru/' in FF
   }
 });
 
-QUnit.test('URL#host', assert => {
+QUnit.test('URL#host', assert => 
+{
   let url = new URL('http://zloirock.ru:81/path');
 
-  if (DESCRIPTORS) {
+  if (DESCRIPTORS) 
+  {
     assert.false(hasOwnProperty.call(url, 'host'));
     const descriptor = Object.getOwnPropertyDescriptor(URL.prototype, 'host');
     assert.true(descriptor.enumerable);
     assert.true(descriptor.configurable);
     assert.same(typeof descriptor.get, 'function');
     assert.same(typeof descriptor.set, 'function');
   }
 
   assert.same(url.host, 'zloirock.ru:81');
 
-  if (DESCRIPTORS) {
+  if (DESCRIPTORS) 
+  {
     url = new URL('http://zloirock.ru:81/path');
     url.host = 'example.com:82';
     assert.same(url.host, 'example.com:82');
     assert.same(String(url), 'http://example.com:82/path');
 
     // url = new URL('http://zloirock.ru:81/path');
     // url.host = 'other?domain.com';
@@ -328,29 +346,32 @@
     // url = new URL('http://zloirock.ru/');
     // url.host = 'a%b';
     // assert.same(url.host, 'zloirock.ru', 'forbidden host code point'); // '' in Chrome, 'a%b' in FF
     // assert.same(String(url), 'http://zloirock.ru/', 'forbidden host code point'); // 'http://a%25b/' in Chrome, 'http://a%b/' in FF
   }
 });
 
-QUnit.test('URL#hostname', assert => {
+QUnit.test('URL#hostname', assert => 
+{
   let url = new URL('http://zloirock.ru:81/');
 
-  if (DESCRIPTORS) {
+  if (DESCRIPTORS) 
+  {
     assert.false(hasOwnProperty.call(url, 'hostname'));
     const descriptor = Object.getOwnPropertyDescriptor(URL.prototype, 'hostname');
     assert.true(descriptor.enumerable);
     assert.true(descriptor.configurable);
     assert.same(typeof descriptor.get, 'function');
     assert.same(typeof descriptor.set, 'function');
   }
 
   assert.same(url.hostname, 'zloirock.ru');
 
-  if (DESCRIPTORS) {
+  if (DESCRIPTORS) 
+  {
     url = new URL('http://zloirock.ru:81/');
     url.hostname = 'example.com';
     assert.same(url.hostname, 'example.com');
     assert.same(String(url), 'http://example.com:81/');
 
     // url = new URL('http://zloirock.ru:81/');
     // url.hostname = 'example.com:82';
@@ -400,29 +421,32 @@
     // url = new URL('http://zloirock.ru/');
     // url.hostname = 'a%b';
     // assert.same(url.hostname, 'zloirock.ru', 'forbidden host code point'); // '' in Chrome, 'a%b' in FF
     // assert.same(String(url), 'http://zloirock.ru/', 'forbidden host code point'); // 'http://a%25b/' in Chrome, 'http://a%b/' in FF
   }
 });
 
-QUnit.test('URL#port', assert => {
+QUnit.test('URL#port', assert => 
+{
   let url = new URL('http://zloirock.ru:1337/');
 
-  if (DESCRIPTORS) {
+  if (DESCRIPTORS) 
+  {
     assert.false(hasOwnProperty.call(url, 'port'));
     const descriptor = Object.getOwnPropertyDescriptor(URL.prototype, 'port');
     assert.true(descriptor.enumerable);
     assert.true(descriptor.configurable);
     assert.same(typeof descriptor.get, 'function');
     assert.same(typeof descriptor.set, 'function');
   }
 
   assert.same(url.port, '1337');
 
-  if (DESCRIPTORS) {
+  if (DESCRIPTORS) 
+  {
     url = new URL('http://zloirock.ru/');
     url.port = 80;
     assert.same(url.port, '');
     assert.same(String(url), 'http://zloirock.ru/');
     url.port = 1337;
     assert.same(url.port, '1337');
     assert.same(String(url), 'http://zloirock.ru:1337/');
@@ -437,54 +461,60 @@
     assert.same(String(url), 'http://zloirock.ru:1234/');
     // url.port = 1e10;
     // assert.same(url.port, '1234'); // '0' in Chrome
     // assert.same(String(url), 'http://zloirock.ru:1234/'); // 'http://zloirock.ru:0/' in Chrome
   }
 });
 
-QUnit.test('URL#pathname', assert => {
+QUnit.test('URL#pathname', assert => 
+{
   let url = new URL('http://zloirock.ru/foo/bar');
 
-  if (DESCRIPTORS) {
+  if (DESCRIPTORS) 
+  {
     assert.false(hasOwnProperty.call(url, 'pathname'));
     const descriptor = Object.getOwnPropertyDescriptor(URL.prototype, 'pathname');
     assert.true(descriptor.enumerable);
     assert.true(descriptor.configurable);
     assert.same(typeof descriptor.get, 'function');
     assert.same(typeof descriptor.set, 'function');
   }
 
   assert.same(url.pathname, '/foo/bar');
 
-  if (DESCRIPTORS) {
+  if (DESCRIPTORS) 
+  {
     url = new URL('http://zloirock.ru/');
     url.pathname = 'bar/baz';
     assert.same(url.pathname, '/bar/baz');
     assert.same(String(url), 'http://zloirock.ru/bar/baz');
   }
 });
 
-QUnit.test('URL#search', assert => {
+QUnit.test('URL#search', assert => 
+{
   let url = new URL('http://zloirock.ru/');
 
-  if (DESCRIPTORS) {
+  if (DESCRIPTORS) 
+  {
     assert.false(hasOwnProperty.call(url, 'search'));
     const descriptor = Object.getOwnPropertyDescriptor(URL.prototype, 'search');
     assert.true(descriptor.enumerable);
     assert.true(descriptor.configurable);
     assert.same(typeof descriptor.get, 'function');
     assert.same(typeof descriptor.set, 'function');
   }
 
   assert.same(url.search, '');
 
   url = new URL('http://zloirock.ru/?foo=bar');
   assert.same(url.search, '?foo=bar');
 
-  if (DESCRIPTORS) {
+  if (DESCRIPTORS) 
+  {
     url = new URL('http://zloirock.ru/?');
     assert.same(url.search, '');
     assert.same(String(url), 'http://zloirock.ru/?');
     url.search = 'foo=bar';
     assert.same(url.search, '?foo=bar');
     assert.same(String(url), 'http://zloirock.ru/?foo=bar');
     url.search = '?bar=baz';
@@ -492,48 +522,53 @@
     assert.same(String(url), 'http://zloirock.ru/?bar=baz');
     url.search = '';
     assert.same(url.search, '');
     assert.same(String(url), 'http://zloirock.ru/');
   }
 });
 
-QUnit.test('URL#searchParams', assert => {
+QUnit.test('URL#searchParams', assert => 
+{
   let url = new URL('http://zloirock.ru/?foo=bar&bar=baz');
 
-  if (DESCRIPTORS) {
+  if (DESCRIPTORS) 
+  {
     assert.false(hasOwnProperty.call(url, 'searchParams'));
     const descriptor = Object.getOwnPropertyDescriptor(URL.prototype, 'searchParams');
     assert.true(descriptor.enumerable);
     assert.true(descriptor.configurable);
     assert.same(typeof descriptor.get, 'function');
   }
 
   assert.true(url.searchParams instanceof URLSearchParams);
   assert.same(url.searchParams.get('foo'), 'bar');
   assert.same(url.searchParams.get('bar'), 'baz');
 
-  if (DESCRIPTORS) {
+  if (DESCRIPTORS) 
+  {
     url = new URL('http://zloirock.ru/');
     url.searchParams.append('foo', 'bar');
     assert.same(String(url), 'http://zloirock.ru/?foo=bar');
 
     url = new URL('http://zloirock.ru/');
     url.search = 'foo=bar';
     assert.same(url.searchParams.get('foo'), 'bar');
 
     url = new URL('http://zloirock.ru/?foo=bar&bar=baz');
     url.search = '';
     assert.false(url.searchParams.has('foo'));
   }
 });
 
-QUnit.test('URL#hash', assert => {
+QUnit.test('URL#hash', assert => 
+{
   let url = new URL('http://zloirock.ru/');
 
-  if (DESCRIPTORS) {
+  if (DESCRIPTORS) 
+  {
     assert.false(hasOwnProperty.call(url, 'hash'));
     const descriptor = Object.getOwnPropertyDescriptor(URL.prototype, 'hash');
     assert.true(descriptor.enumerable);
     assert.true(descriptor.configurable);
     assert.same(typeof descriptor.get, 'function');
     assert.same(typeof descriptor.set, 'function');
   }
@@ -543,15 +578,16 @@
   url = new URL('http://zloirock.ru/#foo');
   assert.same(url.hash, '#foo');
 
   url = new URL('http://zloirock.ru/#');
   assert.same(url.hash, '');
   assert.same(String(url), 'http://zloirock.ru/#');
 
-  if (DESCRIPTORS) {
+  if (DESCRIPTORS) 
+  {
     url = new URL('http://zloirock.ru/#');
     url.hash = 'foo';
     assert.same(url.hash, '#foo');
     assert.same(String(url), 'http://zloirock.ru/#foo');
     url.hash = '';
     assert.same(url.hash, '');
     assert.same(String(url), 'http://zloirock.ru/');
@@ -571,64 +607,71 @@
 
     // url = new URL('http://zloirock.ru/');
     // url.hash = '\udc01\ud802a';
     // assert.same(url.hash, '#%EF%BF%BD%EF%BF%BDa', 'unmatched surrogates');
   }
 });
 
-QUnit.test('URL#toJSON', assert => {
+QUnit.test('URL#toJSON', assert => 
+{
   const { toJSON } = URL.prototype;
   assert.isFunction(toJSON);
   assert.arity(toJSON, 0);
   assert.name(toJSON, 'toJSON');
   assert.enumerable(URL.prototype, 'toJSON');
   if (!NODE) assert.looksNative(toJSON);
 
   const url = new URL('http://zloirock.ru/');
   assert.same(url.toJSON(), 'http://zloirock.ru/');
 
-  if (DESCRIPTORS) {
+  if (DESCRIPTORS) 
+  {
     url.searchParams.append('foo', 'bar');
     assert.same(url.toJSON(), 'http://zloirock.ru/?foo=bar');
   }
 });
 
-QUnit.test('URL#toString', assert => {
+QUnit.test('URL#toString', assert => 
+{
   const { toString } = URL.prototype;
   assert.isFunction(toString);
   assert.arity(toString, 0);
   assert.name(toString, 'toString');
   assert.enumerable(URL.prototype, 'toString');
   if (!NODE) assert.looksNative(toString);
 
   const url = new URL('http://zloirock.ru/');
   assert.same(url.toString(), 'http://zloirock.ru/');
 
-  if (DESCRIPTORS) {
+  if (DESCRIPTORS) 
+  {
     url.searchParams.append('foo', 'bar');
     assert.same(url.toString(), 'http://zloirock.ru/?foo=bar');
   }
 });
 
-QUnit.test('URL#@@toStringTag', assert => {
+QUnit.test('URL#@@toStringTag', assert => 
+{
   const url = new URL('http://zloirock.ru/');
   assert.same(({}).toString.call(url), '[object URL]');
 });
 
-QUnit.test('URL.sham', assert => {
+QUnit.test('URL.sham', assert => 
+{
   assert.same(URL.sham, DESCRIPTORS ? undefined : true);
 });
 
 /* !
  * Modified from https://github.com/zloirock/core-js/blob/d99baeff/tests/unit-global/web.url.can-parse.js
  * core-js
  * MIT License
  */
 
-QUnit.test('URL.canParse', assert => {
+QUnit.test('URL.canParse', assert => 
+{
   const { canParse } = URL;
 
   assert.isFunction(canParse);
   assert.arity(canParse, 1);
   assert.name(canParse, 'canParse');
   if (!NODE) assert.looksNative(canParse);
 
@@ -642,10 +685,16 @@
   assert.true(canParse(undefined, 'q:/w'), 'undefined, q:/w');
   assert.false(canParse('https://login:password@examp:le.com:8080/?a=1&b=2&a=3&c=4#fragment'), 'https://login:password@examp:le.com:8080/?a=1&b=2&a=3&c=4#fragment');
   assert.true(canParse('https://login:password@example.com:8080/?a=1&b=2&a=3&c=4#fragment'), 'https://login:password@example.com:8080/?a=1&b=2&a=3&c=4#fragment');
   assert.true(canParse('https://login:password@example.com:8080/?a=1&b=2&a=3&c=4#fragment', undefined), 'https://login:password@example.com:8080/?a=1&b=2&a=3&c=4#fragment, undefined');
   assert.true(canParse('x', 'https://login:password@example.com:8080/?a=1&b=2&a=3&c=4#fragment'), 'x, https://login:password@example.com:8080/?a=1&b=2&a=3&c=4#fragment');
 
   assert.throws(() => canParse(), 'TypeError: Not enough arguments');
-  assert.throws(() => canParse({ toString() { throw Error('conversion thrower #1'); } }), 'conversion thrower #1');
-  assert.throws(() => canParse('q:w', { toString() { throw Error('conversion thrower #2'); } }), 'conversion thrower #2');
+  assert.throws(() => canParse({ toString() 
+  {
+    throw Error('conversion thrower #1'); 
+  } }), 'conversion thrower #1');
+  assert.throws(() => canParse('q:w', { toString() 
+  {
+    throw Error('conversion thrower #2'); 
+  } }), 'conversion thrower #2');
 });
```

### Comparing `pythonmonkey-0.4.0/tests/js/util-module.simple` & `pythonmonkey-0.6.0/tests/js/util-module.simple`

 * *Files identical despite different names*

### Comparing `pythonmonkey-0.4.0/tests/js/xhr.simple` & `pythonmonkey-0.6.0/tests/js/xhr.simple`

 * *Files 13% similar despite different names*

```diff
@@ -52,75 +52,91 @@
     domain in literature without prior coordination or asking for permission.</p>
     <p><a href="https://www.iana.org/domains/example">More information...</a></p>
 </div>
 </body>
 </html>
 `;
 
-new Promise(function (resolve, reject) {
+new Promise(function (resolve, reject) 
+{
   let xhr = new XMLHttpRequest();
   xhr.open('GET', 'http://www.example.org/');
 
-  xhr.onload = function () {
-    if (this.status >= 200 && this.status < 300) {
+  xhr.onload = function () 
+  {
+    if (this.status >= 200 && this.status < 300) 
+    {
       resolve(this.response);
     }
-    else {
-      reject({
-      status: this.status,
-      statusText:  this.statusText
-      });
+    else 
+    {
+      reject(new Error({
+        status: this.status,
+        statusText:  this.statusText
+      }));
     }
   };
 
-  xhr.onerror = function () {
-    reject({
+  xhr.onerror = function () 
+  {
+    reject(new Error({
       status: this.status,
       statusText: this.statusText
-    });
+    }));
   };
 
   xhr.send();
-}).then((value) => {
-  if (value != expectedBody) {
+}).then((value) => 
+{
+  if (value !== expectedBody) 
+  {
     console.error('expected ', expectedBody, ' but got ', value);
     throw new Error('Test failed');
   }
   console.log('Test passed');
-}).catch((error) => {
-    throw error;
-})
+}).catch((error) => 
+{
+  throw error;
+});
 
 
-new Promise(function (resolve, reject) {
+new Promise(function (resolve, reject) 
+{
   let xhr = new XMLHttpRequest();
   xhr.open('POST', 'http://httpbin.org/post');
 
-  xhr.onload = function () {
-    if (this.status >= 200 && this.status < 300) {
+  xhr.onload = function () 
+  {
+    if (this.status >= 200 && this.status < 300) 
+    {
       resolve(this.response);
     }
-    else {
-      reject({
-      status: this.status,
-      statusText:  this.statusText
-      });
+    else 
+    {
+      reject(new Error({
+        status: this.status,
+        statusText:  this.statusText
+      }));
     }
   };
 
-  xhr.onerror = function () {
-    reject({
+  xhr.onerror = function () 
+  {
+    reject(new Error({
       status: this.status,
       statusText: this.statusText
-    });
+    }));
   };
 
   xhr.send();
-}).then((value) => {
-  value = JSON.parse(value)
-  if (!value["headers"]["User-Agent"].startsWith("Python/")) {
-    console.error("expected Python/* User-Agent, but got ", value.headers["User-Agent"])
+}).then((value) => 
+{
+  value = JSON.parse(value);
+  if (!value['headers']['User-Agent'].startsWith('Python/')) 
+  {
+    console.error('expected Python/* User-Agent, but got ', value.headers['User-Agent']);
   }
   console.log('Test passed');
-}).catch((error) => {
-    throw error;
-})
+}).catch((error) => 
+{
+  throw error;
+});
```

### Comparing `pythonmonkey-0.4.0/tests/python/test_arrays.py` & `pythonmonkey-0.6.0/tests/python/test_arrays.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,841 +1,988 @@
 import pythonmonkey as pm
 from datetime import datetime
 
+
 def test_assign():
-    items = [1,2,3]
-    pm.eval("(arr) => {arr[0] = 42}")(items)
-    assert items[0] == 42
+  items = [1, 2, 3]
+  pm.eval("(arr) => {arr[0] = 42}")(items)
+  assert items[0] == 42
+
 
 def test_get():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr[1]}")(result, items)
-    assert result[0] == 2
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr[1]}")(result, items)
+  assert result[0] == 2
+
 
 def test_get_length():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.length}")(result, items)
-    assert result[0] == 3    
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.length}")(result, items)
+  assert result[0] == 3
+
 
 def test_missing_func():
-    items = [1,2,3]
-    try:
-        pm.eval("(arr) => {arr.after()}")(items)         
-        assert (False)
-    except Exception as e:    
-        assert str(type(e)) == "<class 'pythonmonkey.SpiderMonkeyError'>"
-        assert str(e).__contains__('TypeError: arr.after is not a function')        
+  items = [1, 2, 3]
+  try:
+    pm.eval("(arr) => {arr.after()}")(items)
+    assert False
+  except Exception as e:
+    assert str(type(e)) == "<class 'pythonmonkey.SpiderMonkeyError'>"
+    assert str(e).__contains__('TypeError: arr.after is not a function')
+
+# reverse
+
 
-#reverse
 def test_reverse():
-    items = [1,2,3]
-    pm.eval("(arr) => {arr.reverse()}")(items)
-    assert items == [3,2,1]   
+  items = [1, 2, 3]
+  pm.eval("(arr) => {arr.reverse()}")(items)
+  assert items == [3, 2, 1]
+
 
 def test_reverse_size_one():
-    items = [1]
-    pm.eval("(arr) => {arr.reverse()}")(items)
-    assert items == [1]  
+  items = [1]
+  pm.eval("(arr) => {arr.reverse()}")(items)
+  assert items == [1]
+
 
 def test_reverse_size_zero():
-    items = []
-    pm.eval("(arr) => {arr.reverse()}")(items)
-    assert items == []          
+  items = []
+  pm.eval("(arr) => {arr.reverse()}")(items)
+  assert items == []
+
 
 def test_reverse_returns_reference():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.reverse(); result[0][0] = 4}")(result, items)
-    assert result[0] == [4,2,1]
-    assert items == [4,2,1]      
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.reverse(); result[0][0] = 4}")(result, items)
+  assert result[0] == [4, 2, 1]
+  assert items == [4, 2, 1]
+
 
 def test_reverse_ignores_extra_args():
-    items = [1,2,3]
-    pm.eval("(arr) => {arr.reverse(9)}")(items)
-    assert items == [3,2,1]   
+  items = [1, 2, 3]
+  pm.eval("(arr) => {arr.reverse(9)}")(items)
+  assert items == [3, 2, 1]
+
+# pop
+
 
-#pop
 def test_pop():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.pop()}")(result, items)
-    assert items == [1,2]
-    assert result[0] == 3      
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.pop()}")(result, items)
+  assert items == [1, 2]
+  assert result[0] == 3
+
 
 def test_pop_empty():
-    items = []
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.pop()}")(result, items)
-    assert items == []
-    assert result[0] is None       
+  items = []
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.pop()}")(result, items)
+  assert items == []
+  assert result[0] is None
+
 
 def test_pop_ignore_extra_args():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.pop(1)}")(result, items)
-    assert items == [1,2]
-    assert result[0] == 3      
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.pop(1)}")(result, items)
+  assert items == [1, 2]
+  assert result[0] == 3
+
+# join
+
 
-#join
 def test_join_no_arg():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.join()}")(result, items)
-    assert result[0] == '1,2,3'     
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.join()}")(result, items)
+  assert result[0] == '1,2,3'
+
 
 def test_join_empty_array():
-    items = []
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.join()}")(result, items)
-    assert result[0] == ''       
+  items = []
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.join()}")(result, items)
+  assert result[0] == ''
+
 
 def test_join_no_arg_diff_types():
-    items = [1,False,"END"]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.join()}")(result, items)
-    assert result[0] == '1,false,END'     
+  items = [1, False, "END"]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.join()}")(result, items)
+  assert result[0] == '1,false,END'
+
 
 def test_join_no_arg_with_embedded_list_type():
-    items = [1,[2,3],"END"]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.join()}")(result, items)
-    assert result[0] == '1,2,3,END'   
+  items = [1, [2, 3], "END"]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.join()}")(result, items)
+  assert result[0] == '1,2,3,END'
+
 
 def test_join_with_sep():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.join('-')}")(result, items)
-    assert result[0] == '1-2-3'
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.join('-')}")(result, items)
+  assert result[0] == '1-2-3'
+
 
 def test_join_none():
-    items = [None,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.join()}")(result, items)
-    assert result[0] == ',2,3'    
+  items = [None, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.join()}")(result, items)
+  assert result[0] == ',2,3'
+
 
 def test_join_null():
-    items = [pm.null,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.join()}")(result, items)
-    assert result[0] == ',2,3'  
+  items = [pm.null, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.join()}")(result, items)
+  assert result[0] == ',2,3'
+
 
 def test_join_utf8():
-    prices = ["￥7", 500, 8123, 12]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.join()}")(result, prices)
-    assert result[0] == '￥7,500,8123,12'               
+  prices = ["￥7", 500, 8123, 12]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.join()}")(result, prices)
+  assert result[0] == '￥7,500,8123,12'
+
+# toString
+
 
-#toString
 def test_toString():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.toString()}")(result, items)
-    assert result[0] == '1,2,3'
-    
-#push
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.toString()}")(result, items)
+  assert result[0] == '1,2,3'
+
+# push
+
+
 def test_push():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.push(4)}")(result, items)
-    assert items == [1,2,3,4]
-    assert result[0] == 4       
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.push(4)}")(result, items)
+  assert items == [1, 2, 3, 4]
+  assert result[0] == 4
+
 
 def test_push_no_arg():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.push()}")(result, items)
-    assert items == [1,2,3,]
-    assert result[0] == 3 
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.push()}")(result, items)
+  assert items == [1, 2, 3,]
+  assert result[0] == 3
+
 
 def test_push_two_args():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.push(4,false)}")(result, items)
-    assert items == [1,2,3,4,False]
-    assert result[0] == 5   
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.push(4,false)}")(result, items)
+  assert items == [1, 2, 3, 4, False]
+  assert result[0] == 5
+
 
 def test_push_list():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.push([4,5])}")(result, items)
-    assert items == [1,2,3,[4,5]]
-    assert result[0] == 4   
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.push([4,5])}")(result, items)
+  assert items == [1, 2, 3, [4, 5]]
+  assert result[0] == 4
+
+# shift
+
 
-#shift
 def test_shift():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.shift()}")(result, items)
-    assert items == [2,3]
-    assert result[0] == 1    
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.shift()}")(result, items)
+  assert items == [2, 3]
+  assert result[0] == 1
+
 
 def test_shift_empty():
-    items = []
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.shift()}")(result, items)
-    assert items == []
-    assert result[0] is None   
+  items = []
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.shift()}")(result, items)
+  assert items == []
+  assert result[0] is None
+
+# unshift
+
 
-#unshift     
 def test_unshift_zero_arg():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.unshift()}")(result, items)
-    assert items == [1,2,3]
-    assert result[0] == 3
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.unshift()}")(result, items)
+  assert items == [1, 2, 3]
+  assert result[0] == 3
+
 
 def test_unshift_one_arg():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.unshift(6)}")(result, items)
-    assert items == [6,1,2,3]
-    assert result[0] == 4    
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.unshift(6)}")(result, items)
+  assert items == [6, 1, 2, 3]
+  assert result[0] == 4
+
 
 def test_unshift_two_args():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.unshift(6,7)}")(result, items)
-    assert items == [6,7,1,2,3]
-    assert result[0] == 5      
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.unshift(6,7)}")(result, items)
+  assert items == [6, 7, 1, 2, 3]
+  assert result[0] == 5
+
+# concat
+
 
-#concat
 def test_concat_primitive():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.concat(4)}")(result, items)
-    assert items == [1,2,3]
-    assert result[0] == [1,2,3,4]
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.concat(4)}")(result, items)
+  assert items == [1, 2, 3]
+  assert result[0] == [1, 2, 3, 4]
+
 
 def test_concat_array():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.concat([4,5])}")(result, items)
-    assert items == [1,2,3]
-    assert result[0] == [1,2,3,4,5]    
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.concat([4,5])}")(result, items)
+  assert items == [1, 2, 3]
+  assert result[0] == [1, 2, 3, 4, 5]
+
 
 def test_concat_empty_arg():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.concat()}")(result, items)
-    assert items == [1,2,3]
-    assert result[0] == [1,2,3]  
-    assert items is not result[0]
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.concat()}")(result, items)
+  assert items == [1, 2, 3]
+  assert result[0] == [1, 2, 3]
+  assert items is not result[0]
+
 
 def test_concat_two_arrays():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.concat([7,8], [0,1])}")(result, items)
-    assert items == [1,2,3]
-    assert result[0] == [1,2,3,7,8,0,1]         
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.concat([7,8], [0,1])}")(result, items)
+  assert items == [1, 2, 3]
+  assert result[0] == [1, 2, 3, 7, 8, 0, 1]
+
 
 def test_concat_mix():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.concat([7,8], true, [0,1])}")(result, items)
-    assert items == [1,2,3]
-    assert result[0] == [1,2,3,7,8,True,0,1]    
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.concat([7,8], true, [0,1])}")(result, items)
+  assert items == [1, 2, 3]
+  assert result[0] == [1, 2, 3, 7, 8, True, 0, 1]
+
 
 def test_concat_object_element():
-    d = {"a":1}
-    items = [1, 2, d]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.concat()}")(result, items)
-    assert items == [1, 2, d]
-    assert result[0] == [1, 2, d]
-    assert items is not result[0]
-    assert d is items[2]
-    assert d is result[0][2]    
+  d = {"a": 1}
+  items = [1, 2, d]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.concat()}")(result, items)
+  assert items == [1, 2, d]
+  assert result[0] == [1, 2, d]
+  assert items is not result[0]
+  assert d is items[2]
+  assert d is result[0][2]
+
+# slice
+
 
-#slice
 def test_slice():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.slice(1,2)}")(result, items)
-    assert items == [1,2,3]
-    assert result[0] == [2]   
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.slice(1,2)}")(result, items)
+  assert items == [1, 2, 3]
+  assert result[0] == [2]
+
 
 def test_slice_copy():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.slice(0,3)}")(result, items)
-    assert items == [1,2,3]
-    assert result[0] == [1,2,3]
-    assert items is not result[0]    
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.slice(0,3)}")(result, items)
+  assert items == [1, 2, 3]
+  assert result[0] == [1, 2, 3]
+  assert items is not result[0]
+
 
 def test_slice_start_zero():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.slice(0,2)}")(result, items)
-    assert items == [1,2,3]
-    assert result[0] == [1,2]      
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.slice(0,2)}")(result, items)
+  assert items == [1, 2, 3]
+  assert result[0] == [1, 2]
+
 
 def test_slice_stop_length():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.slice(1,3)}")(result, items)
-    assert items == [1,2,3]
-    assert result[0] == [2,3]     
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.slice(1,3)}")(result, items)
+  assert items == [1, 2, 3]
+  assert result[0] == [2, 3]
+
 
 def test_slice_stop_beyond_length():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.slice(1,4)}")(result, items)
-    assert items == [1,2,3]
-    assert result[0] == [2,3]   
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.slice(1,4)}")(result, items)
+  assert items == [1, 2, 3]
+  assert result[0] == [2, 3]
+
 
 def test_slice_start_negative():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.slice(-3,-1)}")(result, items)
-    assert result[0] == [1,2]      
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.slice(-3,-1)}")(result, items)
+  assert result[0] == [1, 2]
+
+# indexOf
+
 
-#indexOf
 def test_indexOf():
-    items = [1,2,3,1]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.indexOf(1)}")(result, items)
-    assert result[0] == 0     
+  items = [1, 2, 3, 1]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.indexOf(1)}")(result, items)
+  assert result[0] == 0
+
 
 def test_indexOf_with_start():
-    items = [1,2,3,4,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.indexOf(3, 3)}")(result, items)
-    assert result[0] == 4
+  items = [1, 2, 3, 4, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.indexOf(3, 3)}")(result, items)
+  assert result[0] == 4
+
 
 def test_indexOf_with_negative_start():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.indexOf(3, -2)}")(result, items)
-    assert result[0] == 2 
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.indexOf(3, -2)}")(result, items)
+  assert result[0] == 2
+
 
 def test_indexOf_zero_size():
-    items = []
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.indexOf(1)}")(result, items)
-    assert result[0] == -1    
+  items = []
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.indexOf(1)}")(result, items)
+  assert result[0] == -1
+
 
 def test_indexOf_start_beyond_length():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.indexOf(1, 10)}")(result, items)
-    assert result[0] == -1    
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.indexOf(1, 10)}")(result, items)
+  assert result[0] == -1
+
 
 def test_indexOf_not_found():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.indexOf(10)}")(result, items)
-    assert result[0] == -1  
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.indexOf(10)}")(result, items)
+  assert result[0] == -1
+
 
 def test_indexOf_small_start():
-    items = [1,2,3,1]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.indexOf(1, -10)}")(result, items)
-    assert result[0] == 0        
+  items = [1, 2, 3, 1]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.indexOf(1, -10)}")(result, items)
+  assert result[0] == 0
+
+# lastIndexOf
+
 
-#lastIndexOf
 def test_lastIndexOf():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.lastIndexOf(1)}")(result, items)
-    assert result[0] == 0    
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.lastIndexOf(1)}")(result, items)
+  assert result[0] == 0
+
 
 def test_lastIndexOf_dup():
-    items = [1,2,3,1]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.lastIndexOf(1)}")(result, items)
-    assert result[0] == 3    
+  items = [1, 2, 3, 1]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.lastIndexOf(1)}")(result, items)
+  assert result[0] == 3
+
 
 def test_lastIndexOf_with_from_index():
-    items = [1,2,3,1]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.lastIndexOf(1, 2)}")(result, items)
-    assert result[0] == 0       
+  items = [1, 2, 3, 1]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.lastIndexOf(1, 2)}")(result, items)
+  assert result[0] == 0
+
 
 def test_lastIndexOf_with_from_index_greater_than_size():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.lastIndexOf(1, 10)}")(result, items)
-    assert result[0] == 0    
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.lastIndexOf(1, 10)}")(result, items)
+  assert result[0] == 0
+
 
 def test_lastIndexOf_with_negative_from_index():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.lastIndexOf(1, -2)}")(result, items)
-    assert result[0] == 0                     
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.lastIndexOf(1, -2)}")(result, items)
+  assert result[0] == 0
+
 
 def test_lastIndexOf_not_found():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.lastIndexOf(3, 0)}")(result, items)
-    assert result[0] == -1   
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.lastIndexOf(3, 0)}")(result, items)
+  assert result[0] == -1
+
 
 def test_lastIndexOf_small_start():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.lastIndexOf(1, -10)}")(result, items)
-    assert result[0] == -1      
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.lastIndexOf(1, -10)}")(result, items)
+  assert result[0] == -1
+
+# splice
+
 
-#splice
 def test_splice_no_args():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.splice()}")(result, items)
-    assert items == [1,2,3]
-    assert result[0] == []     
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.splice()}")(result, items)
+  assert items == [1, 2, 3]
+  assert result[0] == []
+
 
 def test_splice_one_arg():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.splice(1)}")(result, items)
-    assert items == [1]
-    assert result[0] == [2,3]      
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.splice(1)}")(result, items)
+  assert items == [1]
+  assert result[0] == [2, 3]
+
 
 def test_splice_one_arg_negative():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.splice(-2)}")(result, items)
-    assert items == [1]
-    assert result[0] == [2,3]    
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.splice(-2)}")(result, items)
+  assert items == [1]
+  assert result[0] == [2, 3]
+
 
 def test_splice_two_args_negative_count():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.splice(1, -1)}")(result, items)
-    assert items == [1,2,3]
-    assert result[0] == []  
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.splice(1, -1)}")(result, items)
+  assert items == [1, 2, 3]
+  assert result[0] == []
+
 
 def test_splice_two_args_zero_count():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.splice(1, 0)}")(result, items)
-    assert items == [1,2,3]
-    assert result[0] == []       
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.splice(1, 0)}")(result, items)
+  assert items == [1, 2, 3]
+  assert result[0] == []
+
 
 def test_splice_two_args_one_count():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.splice(1, 1)}")(result, items)
-    assert items == [1,3]
-    assert result[0] == [2]   
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.splice(1, 1)}")(result, items)
+  assert items == [1, 3]
+  assert result[0] == [2]
+
 
 def test_splice_two_args_two_count():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.splice(1, 2)}")(result, items)
-    assert items == [1]
-    assert result[0] == [2,3]      
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.splice(1, 2)}")(result, items)
+  assert items == [1]
+  assert result[0] == [2, 3]
+
 
 def test_splice_three_args_zero_count():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.splice(1,0,5)}")(result, items)
-    assert items == [1,5,2,3]
-    assert result[0] == []   
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.splice(1,0,5)}")(result, items)
+  assert items == [1, 5, 2, 3]
+  assert result[0] == []
+
 
 def test_splice_three_args_one_count():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.splice(1,1,5)}")(result, items)
-    assert items == [1,5,3]
-    assert result[0] == [2] 
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.splice(1,1,5)}")(result, items)
+  assert items == [1, 5, 3]
+  assert result[0] == [2]
+
 
 def test_splice_three_args_two_count():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.splice(1,2,5)}")(result, items)
-    assert items == [1,5]
-    assert result[0] == [2,3]     
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.splice(1,2,5)}")(result, items)
+  assert items == [1, 5]
+  assert result[0] == [2, 3]
+
 
 def test_splice_four_args_zero_count():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.splice(1,0,5,6)}")(result, items)
-    assert items == [1,5,6,2,3]
-    assert result[0] == []   
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.splice(1,0,5,6)}")(result, items)
+  assert items == [1, 5, 6, 2, 3]
+  assert result[0] == []
+
 
 def test_splice_four_args_one_count():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.splice(1,1,5,6)}")(result, items)
-    assert items == [1,5,6,3]
-    assert result[0] == [2] 
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.splice(1,1,5,6)}")(result, items)
+  assert items == [1, 5, 6, 3]
+  assert result[0] == [2]
+
 
 def test_splice_four_args_two_count():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.splice(1,2,5,6)}")(result, items)
-    assert items == [1,5,6]
-    assert result[0] == [2,3]                               
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.splice(1,2,5,6)}")(result, items)
+  assert items == [1, 5, 6]
+  assert result[0] == [2, 3]
+
+# fill
+
 
-#fill
 def test_fill_returns_ref_to_self():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.fill(8)}")(result, items)
-    assert items == [8,8,8]
-    assert items is result[0]
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.fill(8)}")(result, items)
+  assert items == [8, 8, 8]
+  assert items is result[0]
+
 
 def test_fill_other_type():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.fill(false)}")(result, items)
-    assert items == [False,False,False]  
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.fill(false)}")(result, items)
+  assert items == [False, False, False]
+
 
 def test_fill_with_start():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.fill(8,1)}")(result, items)
-    assert items == [1,8,8] 
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.fill(8,1)}")(result, items)
+  assert items == [1, 8, 8]
+
 
 def test_fill_with_start_negative():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.fill(8,-2)}")(result, items)
-    assert items == [1,8,8]    
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.fill(8,-2)}")(result, items)
+  assert items == [1, 8, 8]
+
 
 def test_fill_with_start_too_high():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.fill(8,7)}")(result, items)
-    assert items == [1,2,3]  
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.fill(8,7)}")(result, items)
+  assert items == [1, 2, 3]
+
 
 def test_fill_with_stop_smaller_than_start():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.fill(8,7,2)}")(result, items)
-    assert items == [1,2,3]          
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.fill(8,7,2)}")(result, items)
+  assert items == [1, 2, 3]
+
 
 def test_fill_with_stop():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.fill(8,1,2)}")(result, items)
-    assert items == [1,8,3]    
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.fill(8,1,2)}")(result, items)
+  assert items == [1, 8, 3]
+
 
 def test_fill_with_negative_stop():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.fill(8,1,-1)}")(result, items)
-    assert items == [1,8,3]    
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.fill(8,1,-1)}")(result, items)
+  assert items == [1, 8, 3]
+
 
 def test_fill_with_negative_stop_too_low():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.fill(8,1,-10)}")(result, items)
-    assert items == [1,2,3]       
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.fill(8,1,-10)}")(result, items)
+  assert items == [1, 2, 3]
+
 
 def test_fill_with_stop_too_high():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.fill(8,1,10)}")(result, items)
-    assert items == [1,8,8]  
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.fill(8,1,10)}")(result, items)
+  assert items == [1, 8, 8]
+
 
 def test_fill_object():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {let a = {a:1}; result[0] = arr.fill(a)}")(result, items)
-    assert items == [{"a":1},{"a":1},{"a":1}]
-    assert items is result[0]
-    assert items[0] is items[1] is items[2]    
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {let a = {a:1}; result[0] = arr.fill(a)}")(result, items)
+  assert items == [{"a": 1}, {"a": 1}, {"a": 1}]
+  assert items is result[0]
+  assert items[0] is items[1] is items[2]
+
+# copyWithin
+
 
-#copyWithin
 def test_copyWithin():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.copyWithin(0,1)}")(result, items)
-    assert items == [2,3,3]
-    assert items is result[0]
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.copyWithin(0,1)}")(result, items)
+  assert items == [2, 3, 3]
+  assert items is result[0]
+
 
 def test_copyWithin_no_args():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.copyWithin()}")(result, items)
-    assert items == [1,2,3]     
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.copyWithin()}")(result, items)
+  assert items == [1, 2, 3]
+
 
 def test_copyWithin_target_only_overwrite_all():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.copyWithin(0)}")(result, items)
-    assert items == [1,2,3]  
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.copyWithin(0)}")(result, items)
+  assert items == [1, 2, 3]
+
 
 def test_copyWithin_target_only():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.copyWithin(1)}")(result, items)
-    assert items == [1,1,2]     
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.copyWithin(1)}")(result, items)
+  assert items == [1, 1, 2]
+
 
 def test_copyWithin_negative_target_only():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.copyWithin(-1)}")(result, items)
-    assert items == [1,2,1] 
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.copyWithin(-1)}")(result, items)
+  assert items == [1, 2, 1]
+
 
 def test_copyWithin_target_too_large():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.copyWithin(10)}")(result, items)
-    assert items == [1,2,3]     
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.copyWithin(10)}")(result, items)
+  assert items == [1, 2, 3]
+
 
 def test_copyWithin_target_and_start():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.copyWithin(1, 2)}")(result, items)
-    assert items == [1,3,3]   
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.copyWithin(1, 2)}")(result, items)
+  assert items == [1, 3, 3]
+
 
 def test_copyWithin_target_and_start_too_large():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.copyWithin(1, 10)}")(result, items)
-    assert items == [1,2,3]       
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.copyWithin(1, 10)}")(result, items)
+  assert items == [1, 2, 3]
+
 
 def test_copyWithin_target_and_negative_start():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.copyWithin(1, -1)}")(result, items)
-    assert items == [1,3,3]   
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.copyWithin(1, -1)}")(result, items)
+  assert items == [1, 3, 3]
+
 
 def test_copyWithin_target_and_start_and_end():
-    items = [1,2,3,4,5]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.copyWithin(1,2,3)}")(result, items)
-    assert items == [1,3,3,4,5]    
+  items = [1, 2, 3, 4, 5]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.copyWithin(1,2,3)}")(result, items)
+  assert items == [1, 3, 3, 4, 5]
+
 
 def test_copyWithin_target_and_start_and_negative_end():
-    items = [1,2,3,4,5]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.copyWithin(1,2,-2)}")(result, items)
-    assert items == [1,3,3,4,5]    
+  items = [1, 2, 3, 4, 5]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.copyWithin(1,2,-2)}")(result, items)
+  assert items == [1, 3, 3, 4, 5]
+
 
 def test_copyWithin_target_too_small_and_start():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.copyWithin(-10,2)}")(result, items)
-    assert items == [3,2,3]  
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.copyWithin(-10,2)}")(result, items)
+  assert items == [3, 2, 3]
+
 
 def test_copyWithin_target_greater_than_start():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => { result[0] = arr.copyWithin(2,1)}")(result, items)
-    assert items == [1,2,2]      
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => { result[0] = arr.copyWithin(2,1)}")(result, items)
+  assert items == [1, 2, 2]
+
 
 def test_copyWithin_target_and_start_too_small():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.copyWithin(1, -10)}")(result, items)
-    assert items == [1,1,2]  
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.copyWithin(1, -10)}")(result, items)
+  assert items == [1, 1, 2]
+
 
 def test_copyWithin_target_and_start_and_end_too_small():
-    items = [1,2,3,4,5]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.copyWithin(1,2,-10)}")(result, items)
-    assert items == [1,2,3,4,5]    
+  items = [1, 2, 3, 4, 5]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.copyWithin(1,2,-10)}")(result, items)
+  assert items == [1, 2, 3, 4, 5]
+
 
 def test_copyWithin_target_and_start_and_end_too_large():
-    items = [1,2,3,4,5]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.copyWithin(2,1,10)}")(result, items)
-    assert items == [1,2,2,3,4]      
+  items = [1, 2, 3, 4, 5]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.copyWithin(2,1,10)}")(result, items)
+  assert items == [1, 2, 2, 3, 4]
+
 
 def test_copyWithin_target_and_start_greater_than_end():
-    items = [1,2,3,4,5]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.copyWithin(2,3,2)}")(result, items)
-    assert items == [1,2,3,4,5]     
+  items = [1, 2, 3, 4, 5]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.copyWithin(2,3,2)}")(result, items)
+  assert items == [1, 2, 3, 4, 5]
+
+# includes
+
 
-#includes
 def test_includes():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.includes(1)}")(result, items)
-    assert result[0] == True   
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.includes(1)}")(result, items)
+  assert result[0]
+
 
 def test_includes_start_index():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.includes(1, 1)}")(result, items)
-    assert result[0] == False
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.includes(1, 1)}")(result, items)
+  assert not result[0]
+
 
 def test_includes_start_index_negative():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.includes(1, -1)}")(result, items)
-    assert result[0] == False    
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.includes(1, -1)}")(result, items)
+  assert not result[0]
+
 
 def test_includes_start_index_negative_large():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.includes(1, -10)}")(result, items)
-    assert result[0] == True    
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.includes(1, -10)}")(result, items)
+  assert result[0]
+
 
 def test_includes_start_index_large():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.includes(1, 10)}")(result, items)
-    assert result[0] == False          
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.includes(1, 10)}")(result, items)
+  assert not result[0]
+
 
 def test_includes_other_type():
-    items = [1,2,'Hi']
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.includes('Hi')}")(result, items)
-    assert result[0] == True         
+  items = [1, 2, 'Hi']
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.includes('Hi')}")(result, items)
+  assert result[0]
+
 
 def test_includes_not():
-    items = [1,2,3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.includes(5)}")(result, items)
-    assert result[0] == False   
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.includes(5)}")(result, items)
+  assert not result[0]
+
 
 def test_includes_not_other_type():
-    items = [1,2,'Hi']
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.includes('Joe')}")(result, items)
-    assert result[0] == False   
+  items = [1, 2, 'Hi']
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.includes('Joe')}")(result, items)
+  assert not result[0]
+
 
 def test_includes_too_few_args():
-    items = [4,2,6,7]
-    try:
-        pm.eval("(arr) => {arr.includes()}")(items)      
-        assert (False)
-    except Exception as e:    
-        assert str(type(e)) == "<class 'pythonmonkey.SpiderMonkeyError'>"
-        assert str(e).__contains__("TypeError: includes: At least 1 argument required, but only 0 passed")   
+  items = [4, 2, 6, 7]
+  try:
+    pm.eval("(arr) => {arr.includes()}")(items)
+    assert (False)
+  except Exception as e:
+    assert str(type(e)) == "<class 'pythonmonkey.SpiderMonkeyError'>"
+    assert str(e).__contains__("TypeError: includes: At least 1 argument required, but only 0 passed")
+
+# sort
+
 
-#sort
 def test_sort_empty():
-    items = []
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.sort()}")(result, items)
-    assert result[0] is items
-    assert items == []
+  items = []
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.sort()}")(result, items)
+  assert result[0] is items
+  assert items == []
+
 
 def test_sort_one():
-    items = [5]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.sort()}")(result, items)
-    assert result[0] is items
-    assert items == [5]    
+  items = [5]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.sort()}")(result, items)
+  assert result[0] is items
+  assert items == [5]
+
 
 def test_sort_numbers():
-    items = [4,2,6,7]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.sort()}")(result, items)
-    assert result[0] is items
-    assert items == [2,4,6,7]
+  items = [4, 2, 6, 7]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.sort()}")(result, items)
+  assert result[0] is items
+  assert items == [2, 4, 6, 7]
+
 
 def test_sort_strings():
-    items = ['Four', 'Three', 'One']   
-    pm.eval("(arr) => {arr.sort()}")(items)
-    assert items == ['Four', 'One', 'Three']   
+  items = ['Four', 'Three', 'One']
+  pm.eval("(arr) => {arr.sort()}")(items)
+  assert items == ['Four', 'One', 'Three']
+
 
 def test_sort_with_two_args_keyfunc():
-    items = ['Four', 'Three', 'One']   
-    def myFunc(e, f):
-        return len(e) - len(f) 
-    pm.eval("(arr, compareFun) => {arr.sort(compareFun)}")(items, myFunc)      
-    assert items == ['One', 'Four', 'Three'] 
+  items = ['Four', 'Three', 'One']
+
+  def myFunc(e, f):
+    return len(e) - len(f)
+  pm.eval("(arr, compareFun) => {arr.sort(compareFun)}")(items, myFunc)
+  assert items == ['One', 'Four', 'Three']
+
 
 def test_sort_with_two_args_keyfunc_wrong_return_type():
-    items = ['Four', 'Three', 'One'] 
-    def myFunc(e,f):
-        return e + f 
-    try:
-        pm.eval("(arr, compareFun) => {arr.sort(compareFun)}")(items, myFunc)      
-        assert (False)
-    except Exception as e:  
-        assert str(type(e)) == "<class 'TypeError'>"
-        assert str(e) == "incorrect compare function return type"      
- 
+  items = ['Four', 'Three', 'One']
+
+  def myFunc(e, f):
+    return e + f
+  try:
+    pm.eval("(arr, compareFun) => {arr.sort(compareFun)}")(items, myFunc)
+    assert (False)
+  except Exception as e:
+    assert str(type(e)) == "<class 'TypeError'>"
+    assert str(e) == "incorrect compare function return type"
+
+
 def test_sort_with_two_args_keyfunc_wrong_data_type():
-    items = [4,2,6,7]
-    def myFunc(e,f):
-        return len(e) - len(f)  
-    try:
-        pm.eval("(arr, compareFun) => {arr.sort(compareFun)}")(items, myFunc)      
-        assert (False)
-    except Exception as e:    
-        assert str(type(e)) == "<class 'pythonmonkey.SpiderMonkeyError'>"
-        assert "object of type 'float' has no len()" in str(e)  
-        assert "test_arrays.py" in str(e)   
-        assert "line 751" in str(e)  
-        assert "in myFunc" in str(e) 
-        assert "JS Stack Trace" in str(e) 
-        assert "@evaluate:1:27" in str(e) 
+  items = [4, 2, 6, 7]
+
+  def myFunc(e, f):
+    return len(e) - len(f)
+  try:
+    pm.eval("(arr, compareFun) => {arr.sort(compareFun)}")(items, myFunc)
+    assert (False)
+  except Exception as e:
+    assert str(type(e)) == "<class 'pythonmonkey.SpiderMonkeyError'>"
+    assert "object of type 'float' has no len()" in str(e)
+    assert "test_arrays.py" in str(e)
+    assert "line 883" in str(e)
+    assert "in myFunc" in str(e)
+    assert "JS Stack Trace" in str(e)
+    assert "@evaluate:1:27" in str(e)
+
 
 def test_sort_with_one_arg_keyfunc():
-    items = ['Four', 'Three', 'One']   
-    def myFunc(e):
-        return len(e)  
-    try:
-        pm.eval("(arr, compareFun) => {arr.sort(compareFun)}")(items, myFunc)      
-        assert (False)
-    except Exception as e:    
-        assert str(type(e)) == "<class 'pythonmonkey.SpiderMonkeyError'>"
-        assert "takes 1 positional argument but 2 were given" in str(e)
-        assert "JS Stack Trace" in str(e) 
-        assert "@evaluate:1:27" in str(e)  
+  items = ['Four', 'Three', 'One']
+
+  def myFunc(e):
+    return len(e)
+  try:
+    pm.eval("(arr, compareFun) => {arr.sort(compareFun)}")(items, myFunc)
+    assert (False)
+  except Exception as e:
+    assert str(type(e)) == "<class 'pythonmonkey.SpiderMonkeyError'>"
+    assert "takes 1 positional argument but 2 were given" in str(e)
+    assert "JS Stack Trace" in str(e)
+    assert "@evaluate:1:27" in str(e)
+
 
 def test_sort_with_builtin_keyfunc():
-    items = ['Four', 'Three', 'One']   
-    try:
-        pm.eval("(arr, compareFun) => {arr.sort(compareFun)}")(items, len)      
-        assert (False)
-    except Exception as e:  
-        assert str(type(e)) == "<class 'pythonmonkey.SpiderMonkeyError'>"
-        assert "len() takes exactly one argument (2 given)" in str(e)
-        assert "JS Stack Trace" in str(e) 
-        assert "@evaluate:1:27" in str(e)      
+  items = ['Four', 'Three', 'One']
+  try:
+    pm.eval("(arr, compareFun) => {arr.sort(compareFun)}")(items, len)
+    assert (False)
+  except Exception as e:
+    assert str(type(e)) == "<class 'pythonmonkey.SpiderMonkeyError'>"
+    assert "len() takes exactly one argument (2 given)" in str(e)
+    assert "JS Stack Trace" in str(e)
+    assert "@evaluate:1:27" in str(e)
+
 
 def test_sort_with_js_func():
-    items = ['Four', 'Three', 'One']  
-    result = [None]
-    myFunc = pm.eval("((a, b) => a.toLocaleUpperCase() < b.toLocaleUpperCase() ? -1 : 1)")
-    pm.eval("(result, arr, compareFun) => {result[0] = arr.sort(compareFun)}")(result, items, myFunc)
-    assert result[0] is items
-    assert items == ['Four', 'One', 'Three'] 
+  items = ['Four', 'Three', 'One']
+  result = [None]
+  myFunc = pm.eval("((a, b) => a.toLocaleUpperCase() < b.toLocaleUpperCase() ? -1 : 1)")
+  pm.eval("(result, arr, compareFun) => {result[0] = arr.sort(compareFun)}")(result, items, myFunc)
+  assert result[0] is items
+  assert items == ['Four', 'One', 'Three']
+
 
 def test_sort_numbers_tricky():
-    items = [1, 30, 4, 21, 100000]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.sort()}")(result, items)
-    assert result[0] is items
-    assert items == [1, 100000, 21, 30, 4]    
+  items = [1, 30, 4, 21, 100000]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.sort()}")(result, items)
+  assert result[0] is items
+  assert items == [1, 100000, 21, 30, 4]
+
 
 def test_sort_with_js_func_wrong_data_type():
-    items = [4,2,6,7]
-    myFunc = pm.eval("((a, b) => a.toLocaleUpperCase() < b.toLocaleUpperCase() ? -1 : 1)")
-    try:
-        pm.eval("(arr, compareFun) => {arr.sort(compareFun)}")(items, myFunc)      
-        assert (False)
-    except Exception as e:    
-        assert str(type(e)) == "<class 'pythonmonkey.SpiderMonkeyError'>"
-        assert str(e).__contains__("TypeError: a.toLocaleUpperCase is not a function")   
+  items = [4, 2, 6, 7]
+  myFunc = pm.eval("((a, b) => a.toLocaleUpperCase() < b.toLocaleUpperCase() ? -1 : 1)")
+  try:
+    pm.eval("(arr, compareFun) => {arr.sort(compareFun)}")(items, myFunc)
+    assert (False)
+  except Exception as e:
+    assert str(type(e)) == "<class 'pythonmonkey.SpiderMonkeyError'>"
+    assert str(e).__contains__("TypeError: a.toLocaleUpperCase is not a function")
+
+# forEach
+
 
-#forEach
 def test_forEach():
-    items = ['Four', 'Three', 'One'] 
-    result = ['']
-    returnResult = [0]
-    pm.eval("(returnResult, result, arr) => {returnResult[0] = arr.forEach((element) => result[0] += element)}")(returnResult, result, items)
-    assert items == ['Four', 'Three', 'One']   
-    assert result == ['FourThreeOne'] 
-    assert returnResult == [None] 
+  items = ['Four', 'Three', 'One']
+  result = ['']
+  returnResult = [0]
+  pm.eval("""
+    (returnResult, result, arr) => {
+      returnResult[0] = arr.forEach((element) => result[0] += element);
+    }
+  """)(returnResult, result, items)
+  assert items == ['Four', 'Three', 'One']
+  assert result == ['FourThreeOne']
+  assert returnResult == [None]
+
 
 def test_forEach_check_index():
-    items = ['Four', 'Three', 'One'] 
-    result = ['']
-    pm.eval("(result, arr) => {arr.forEach((element, index) => result[0] += index)}")(result, items) 
-    assert result == ['012']    
+  items = ['Four', 'Three', 'One']
+  result = ['']
+  pm.eval("(result, arr) => {arr.forEach((element, index) => result[0] += index)}")(result, items)
+  assert result == ['012']
+
 
 def test_forEach_check_array():
-    items = ['Four', 'Three', 'One'] 
-    result = ['']
-    pm.eval("(result, arr) => {arr.forEach((element, index, array) => result[0] = array)}")(result, items)
-    assert result == [items]
-    assert result[0] is items        
+  items = ['Four', 'Three', 'One']
+  result = ['']
+  pm.eval("(result, arr) => {arr.forEach((element, index, array) => result[0] = array)}")(result, items)
+  assert result == [items]
+  assert result[0] is items
+
 
 def test_forEach_check_this_arg():
   items = ['Four', 'Three', 'One']
   result = [None]
   pm.eval(
     """
     (result, arr) => {
@@ -852,130 +999,174 @@
       obj.add(arr);
       result[0] = obj.count;
     }
     """
   )(result, items)
   assert result == [3]
 
+
 def test_forEach_check_this_arg_wrong_type():
-    items = ['Four', 'Three', 'One'] 
-    result = [None]
-    a = 9
-    try:
-        pm.eval("(result, arr, a) => {class Counter { constructor() { this.count = 0;} add(array) { array.forEach(function countEntry(entry) { ++this.count; }, a);}} const obj = new Counter(); obj.add(arr); result[0] = obj.count;}")(result, items, a)       
-        assert (False)
-    except Exception as e:    
-        assert str(type(e)) == "<class 'pythonmonkey.SpiderMonkeyError'>"
-        assert str(e).__contains__("TypeError: 'this' argument is not an object or null")    
+  items = ['Four', 'Three', 'One']
+  result = [None]
+  a = 9
+  try:
+    pm.eval("""
+      (result, arr, a) => {
+        class Counter {
+          constructor() {
+            this.count = 0;
+          }
+          add(array) {
+            array.forEach(function countEntry(entry) { ++this.count; }, a);
+          }
+        }
+        const obj = new Counter();
+        obj.add(arr);
+        result[0] = obj.count;
+      }
+    """)(result, items, a)
+    assert (False)
+  except Exception as e:
+    assert str(type(e)) == "<class 'pythonmonkey.SpiderMonkeyError'>"
+    assert str(e).__contains__("TypeError: 'this' argument is not an object or null")
 
 # TODO python function support
 
+
 def test_forEach_with_python_function():
-   def func(element, index, array):
-      array[int(index)] = "to each his own"
-   items = ['Four', 'Three', 'One'] 
-   returnResult = [0]
-   pm.eval("(returnResult, arr, func) => {returnResult[0] = arr.forEach(func)}")(returnResult, items, func)
-   assert items == ['to each his own', 'to each his own', 'to each his own']    
-   assert returnResult == [None]   
+  def func(element, index, array):
+    array[int(index)] = "to each his own"
+  items = ['Four', 'Three', 'One']
+  returnResult = [0]
+  pm.eval("(returnResult, arr, func) => {returnResult[0] = arr.forEach(func)}")(returnResult, items, func)
+  assert items == ['to each his own', 'to each his own', 'to each his own']
+  assert returnResult == [None]
+
 
 def test_forEach_self_pymethod():
- items = ['Four', 'Three', 'One']
- class Counter:
-   def __init__(self):
-     self.count = 0
-   def increment(self, element, index, array):
-     self.count += 1
-  
- obj = Counter()
- assert obj.count == 0
- result = pm.eval("""
+  items = ['Four', 'Three', 'One']
+
+  class Counter:
+    def __init__(self):
+      self.count = 0
+
+    def increment(self, element, index, array):
+      self.count += 1
+
+  obj = Counter()
+  assert obj.count == 0
+  result = pm.eval("""
  (arr, increment, result) => {
    let jsObj = {count: 0}
    arr.forEach(increment, jsObj);
    return jsObj.count;
  }
  """)(items, obj.increment)
- assert obj.count == 0
- assert result == 3    
+  assert obj.count == 0
+  assert result == 3
+
 
 def test_forEach_self_pyfunction():
   items = ['Four', 'Three', 'One']
+
   def increment(self, element, index, array):
     self.count += 1
-  
+
   try:
     pm.eval("""
     (arr, increment, result) => {
       let jsObj = {count: 0}
       arr.forEach(increment, jsObj);
       return jsObj.count;
     }
     """)(items, increment)
     assert False
   except Exception as e:
     assert type(e) is TypeError
-    assert str(e).__contains__("unbound python functions do not have a 'self' to bind") 
+    assert str(e).__contains__("unbound python functions do not have a 'self' to bind")
+
 
 def test_forEach_self_jsfunction():
   items = ['Four', 'Three', 'One']
-  
+
   result = pm.eval("""
   (arr) => {
     function increment(element, index, array) {
       this.count++
     }
     let jsObj = {count: 0}
     arr.forEach(increment, jsObj);
     return jsObj.count;
   }
   """)(items)
   assert result == 3
 
 # TODO should not pass
+
+
 def test_forEach_check_this_arg_null():
-    items = ['Four', 'Three', 'One'] 
-    result = [None]
-    try:
-        pm.eval("(result, arr) => {class Counter { constructor() { this.count = 0;} add(array) { array.forEach(function countEntry(entry) { ++this.count; }, null);}} const obj = new Counter(); obj.add(arr); result[0] = obj.count;}")(result, items)       
-        assert (False)
-    except Exception as e:    
-        assert str(type(e)) == "<class 'pythonmonkey.SpiderMonkeyError'>"
-        assert str(e).__contains__("TypeError: this is null")              
+  items = ['Four', 'Three', 'One']
+  result = [None]
+  try:
+    pm.eval("""
+      (result, arr) => {
+        class Counter {
+          constructor() {
+            this.count = 0;
+          }
+          add(array) {
+            array.forEach(function countEntry(entry) {++this.count; }, null);
+          }
+        }
+        const obj = new Counter();
+        obj.add(arr);
+        result[0] = obj.count;
+      }
+    """)(result, items)
+    assert (False)
+  except Exception as e:
+    assert str(type(e)) == "<class 'pythonmonkey.SpiderMonkeyError'>"
+    assert str(e).__contains__("TypeError: this is null")
+
 
 def test_forEach_too_few_args():
-    items = [4,2,6,7]
-    try:
-        pm.eval("(arr) => {arr.forEach()}")(items)      
-        assert (False)
-    except Exception as e:    
-        assert str(type(e)) == "<class 'pythonmonkey.SpiderMonkeyError'>"
-        assert str(e).__contains__("TypeError: forEach: At least 1 argument required, but only 0 passed")          
+  items = [4, 2, 6, 7]
+  try:
+    pm.eval("(arr) => {arr.forEach()}")(items)
+    assert (False)
+  except Exception as e:
+    assert str(type(e)) == "<class 'pythonmonkey.SpiderMonkeyError'>"
+    assert str(e).__contains__("TypeError: forEach: At least 1 argument required, but only 0 passed")
+
+# map
+
 
-#map   
 def test_map():
-    items = [4,2,6,7]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.map((x) => x * x)}")(result, items)
-    assert items == [4,2,6,7]
-    assert result[0] == [16,4,36,49]
+  items = [4, 2, 6, 7]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.map((x) => x * x)}")(result, items)
+  assert items == [4, 2, 6, 7]
+  assert result[0] == [16, 4, 36, 49]
+
 
 def test_map_check_index():
-    items = [4,2,6,7]
-    result = ['']
-    pm.eval("(result, arr) => {arr.map((x, index) => result[0] += index)}")(result, items)
-    assert items == [4,2,6,7]
-    assert result[0] == '0123'
+  items = [4, 2, 6, 7]
+  result = ['']
+  pm.eval("(result, arr) => {arr.map((x, index) => result[0] += index)}")(result, items)
+  assert items == [4, 2, 6, 7]
+  assert result[0] == '0123'
+
 
 def test_map_check_array():
-    items = ['Four', 'Three', 'One'] 
-    result = ['']
-    pm.eval("(result, arr) => {arr.map((element, index, array) => result[0] = array)}")(result, items)
-    assert result == [items]
-    assert result[0] is items       
+  items = ['Four', 'Three', 'One']
+  result = ['']
+  pm.eval("(result, arr) => {arr.map((element, index, array) => result[0] = array)}")(result, items)
+  assert result == [items]
+  assert result[0] is items
+
 
 def test_map_check_this_arg():
   items = ['Four', 'Three', 'One']
   result = [None]
   pm.eval(
     """
     (result, arr) => {
@@ -990,125 +1181,140 @@
       }
       const obj = new Counter();
       obj.add(arr);
       result[0] = obj.count;
     }
     """
   )(result, items)
-  assert result == [3]    
+  assert result == [3]
+
 
 def test_map_too_few_args():
-    items = [4,2,6,7]
-    try:
-        pm.eval("(arr) => {arr.map()}")(items)      
-        assert (False)
-    except Exception as e:    
-        assert str(type(e)) == "<class 'pythonmonkey.SpiderMonkeyError'>"
-        assert str(e).__contains__("TypeError: map: At least 1 argument required, but only 0 passed")     
+  items = [4, 2, 6, 7]
+  try:
+    pm.eval("(arr) => {arr.map()}")(items)
+    assert (False)
+  except Exception as e:
+    assert str(type(e)) == "<class 'pythonmonkey.SpiderMonkeyError'>"
+    assert str(e).__contains__("TypeError: map: At least 1 argument required, but only 0 passed")
+
 
 def test_map_arg_wrong_type():
-    items = [4,2,6,7]
-    try:
-        pm.eval("(arr) => {arr.map(8)}")(items)      
-        assert (False)
-    except Exception as e:    
-        assert str(type(e)) == "<class 'pythonmonkey.SpiderMonkeyError'>"
-        assert str(e).__contains__("TypeError: map: callback is not a function")            
+  items = [4, 2, 6, 7]
+  try:
+    pm.eval("(arr) => {arr.map(8)}")(items)
+    assert (False)
+  except Exception as e:
+    assert str(type(e)) == "<class 'pythonmonkey.SpiderMonkeyError'>"
+    assert str(e).__contains__("TypeError: map: callback is not a function")
+
 
 def test_map_check_array_mutation():
-    items = ['Four', 'Three', 'One'] 
-    result = ['']
-    pm.eval("(result, arr) => {arr.map((element, index, array) => {array[0] = 'Ten'; result[0] = array})}")(result, items)
-    assert result[0] == ['Ten', 'Three', 'One']
-    assert items == ['Ten', 'Three', 'One']
+  items = ['Four', 'Three', 'One']
+  result = ['']
+  pm.eval("(result, arr) => {arr.map((element, index, array) => {array[0] = 'Ten'; result[0] = array})}")(result, items)
+  assert result[0] == ['Ten', 'Three', 'One']
+  assert items == ['Ten', 'Three', 'One']
+
 
 def test_map_with_python_function():
-   def func(element, index, array):
-      array[int(index)] = "to each his own"
-      return 42
-   items = ['Four', 'Three', 'One'] 
-   returnResult = [0]
-   pm.eval("(returnResult, arr, func) => {returnResult[0] = arr.map(func)}")(returnResult, items, func)
-   assert items == ['to each his own', 'to each his own', 'to each his own']    
-   assert returnResult == [[42.0, 42.0, 42.0]]   
+  def func(element, index, array):
+    array[int(index)] = "to each his own"
+    return 42
+  items = ['Four', 'Three', 'One']
+  returnResult = [0]
+  pm.eval("(returnResult, arr, func) => {returnResult[0] = arr.map(func)}")(returnResult, items, func)
+  assert items == ['to each his own', 'to each his own', 'to each his own']
+  assert returnResult == [[42.0, 42.0, 42.0]]
+
 
 def test_map_self_pymethod():
- items = ['Four', 'Three', 'One']
- class Counter:
-   def __init__(self):
-     self.count = 0
-   def increment(self, element, index, array):
-     self.count += 1
-  
- obj = Counter()
- assert obj.count == 0
- result = pm.eval("""
+  items = ['Four', 'Three', 'One']
+
+  class Counter:
+    def __init__(self):
+      self.count = 0
+
+    def increment(self, element, index, array):
+      self.count += 1
+
+  obj = Counter()
+  assert obj.count == 0
+  result = pm.eval("""
  (arr, increment, result) => {
    let jsObj = {count: 0}
    arr.map(increment, jsObj);
    return jsObj.count;
  }
  """)(items, obj.increment)
- assert obj.count == 0
- assert result == 3    
+  assert obj.count == 0
+  assert result == 3
+
 
 def test_map_self_pyfunction():
   items = ['Four', 'Three', 'One']
+
   def increment(self, element, index, array):
     self.count += 1
-  
+
   try:
     pm.eval("""
     (arr, increment, result) => {
       let jsObj = {count: 0}
       arr.map(increment, jsObj);
       return jsObj.count;
     }
     """)(items, increment)
     assert False
   except Exception as e:
     assert type(e) is TypeError
-    assert str(e).__contains__("unbound python functions do not have a 'self' to bind") 
+    assert str(e).__contains__("unbound python functions do not have a 'self' to bind")
+
 
 def test_map_self_jsfunction():
   items = ['Four', 'Three', 'One']
-  
+
   result = pm.eval("""
   (arr) => {
     function increment(element, index, array) {
       this.count++
     }
     let jsObj = {count: 0}
     arr.map(increment, jsObj);
     return jsObj.count;
   }
   """)(items)
-  assert result == 3     
-    
-#filter
+  assert result == 3
+
+# filter
+
+
 def test_filter():
-    words = ['spray', 'elite', 'exuberant', 'destruction', 'present']
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.filter((word) => word.length > 6)}")(result, words)
-    assert words == ['spray', 'elite', 'exuberant', 'destruction', 'present']
-    assert result[0] == ['exuberant', 'destruction', 'present']
+  words = ['spray', 'elite', 'exuberant', 'destruction', 'present']
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.filter((word) => word.length > 6)}")(result, words)
+  assert words == ['spray', 'elite', 'exuberant', 'destruction', 'present']
+  assert result[0] == ['exuberant', 'destruction', 'present']
+
 
 def test_filter_check_index():
-    items = [4,2,6,7]
-    result = ['']
-    pm.eval("(result, arr) => {arr.filter((x, index) => result[0] += index)}")(result, items)
-    assert items == [4,2,6,7]
-    assert result[0] == '0123'
+  items = [4, 2, 6, 7]
+  result = ['']
+  pm.eval("(result, arr) => {arr.filter((x, index) => result[0] += index)}")(result, items)
+  assert items == [4, 2, 6, 7]
+  assert result[0] == '0123'
+
 
 def test_filter_check_array():
-    items = ['Four', 'Three', 'One'] 
-    result = ['']
-    pm.eval("(result, arr) => {arr.filter((element, index, array) => result[0] = array)}")(result, items)
-    assert result == [items]
-    assert result[0] is items    
+  items = ['Four', 'Three', 'One']
+  result = ['']
+  pm.eval("(result, arr) => {arr.filter((element, index, array) => result[0] = array)}")(result, items)
+  assert result == [items]
+  assert result[0] is items
+
 
 def test_filter_check_this_arg():
   items = ['Four', 'Three', 'One']
   result = [None]
   pm.eval(
     """
     (result, arr) => {
@@ -1123,219 +1329,313 @@
       }
       const obj = new Counter();
       obj.add(arr);
       result[0] = obj.count;
     }
     """
   )(result, items)
-  assert result == [3]       
+  assert result == [3]
+
 
 def test_filter_too_few_args():
-    items = [4,2,6,7]
-    try:
-        pm.eval("(arr) => {arr.filter()}")(items)      
-        assert (False)
-    except Exception as e:    
-        assert str(type(e)) == "<class 'pythonmonkey.SpiderMonkeyError'>"
-        assert str(e).__contains__("TypeError: filter: At least 1 argument required, but only 0 passed")   
+  items = [4, 2, 6, 7]
+  try:
+    pm.eval("(arr) => {arr.filter()}")(items)
+    assert (False)
+  except Exception as e:
+    assert str(type(e)) == "<class 'pythonmonkey.SpiderMonkeyError'>"
+    assert str(e).__contains__("TypeError: filter: At least 1 argument required, but only 0 passed")
+
 
 def test_filter_python_function():
-   def func(element, index, array):
-      array[int(index)] = "to each his own"
-   items = ['Four', 'Three', 'One'] 
-   returnResult = [0]
-   pm.eval("(returnResult, arr, func) => {returnResult[0] = arr.filter(func)}")(returnResult, items, func)
-   assert items == ['to each his own', 'to each his own', 'to each his own']    
-   assert returnResult == [[]]   
+  def func(element, index, array):
+    array[int(index)] = "to each his own"
+  items = ['Four', 'Three', 'One']
+  returnResult = [0]
+  pm.eval("(returnResult, arr, func) => {returnResult[0] = arr.filter(func)}")(returnResult, items, func)
+  assert items == ['to each his own', 'to each his own', 'to each his own']
+  assert returnResult == [[]]
+
 
 def test_filter_self_pymethod():
- items = ['Four', 'Three', 'One']
- class Counter:
-   def __init__(self):
-     self.count = 0
-   def increment(self, element, index, array):
-     self.count += 1
-  
- obj = Counter()
- assert obj.count == 0
- result = pm.eval("""
+  items = ['Four', 'Three', 'One']
+
+  class Counter:
+    def __init__(self):
+      self.count = 0
+
+    def increment(self, element, index, array):
+      self.count += 1
+
+  obj = Counter()
+  assert obj.count == 0
+  result = pm.eval("""
  (arr, increment, result) => {
    let jsObj = {count: 0}
    arr.filter(increment, jsObj);
    return jsObj.count;
  }
  """)(items, obj.increment)
- assert obj.count == 0
- assert result == 3    
+  assert obj.count == 0
+  assert result == 3
+
 
 def test_filter_self_pyfunction():
   items = ['Four', 'Three', 'One']
+
   def increment(self, element, index, array):
     self.count += 1
-  
+
   try:
     pm.eval("""
     (arr, increment, result) => {
       let jsObj = {count: 0}
       arr.filter(increment, jsObj);
       return jsObj.count;
     }
     """)(items, increment)
     assert False
   except Exception as e:
     assert type(e) is TypeError
-    assert str(e).__contains__("unbound python functions do not have a 'self' to bind") 
+    assert str(e).__contains__("unbound python functions do not have a 'self' to bind")
+
 
 def test_filter_self_jsfunction():
   items = ['Four', 'Three', 'One']
-  
+
   result = pm.eval("""
   (arr) => {
     function increment(element, index, array) {
       this.count++
     }
     let jsObj = {count: 0}
     arr.filter(increment, jsObj);
     return jsObj.count;
   }
   """)(items)
-  assert result == 3                
+  assert result == 3
+
+# reduce
+
 
-#reduce
 def test_reduce():
-    items = [1,2,3,4,5]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.reduce((accumulator, currentValue) => accumulator + currentValue, 0)}")(result, items)
-    assert items == [1,2,3,4,5]
-    assert result[0] == 15
+  items = [1, 2, 3, 4, 5]
+  result = [None]
+  pm.eval("""
+    (result, arr) => {
+      result[0] = arr.reduce((accumulator, currentValue) => accumulator + currentValue, 0);
+    }
+  """)(result, items)
+  assert items == [1, 2, 3, 4, 5]
+  assert result[0] == 15
+
 
 def test_reduce_empty_array_no_accumulator():
-    items = []
-    try:
-        pm.eval("(arr) => {arr.reduce((accumulator, currentValue) => accumulator + currentValue)}")(items)    
-        assert (False)
-    except Exception as e:    
-        assert str(type(e)) == "<class 'pythonmonkey.SpiderMonkeyError'>"
-        assert str(e).__contains__("TypeError: reduce of empty array with no initial value")          
+  items = []
+  try:
+    pm.eval("(arr) => {arr.reduce((accumulator, currentValue) => accumulator + currentValue)}")(items)
+    assert (False)
+  except Exception as e:
+    assert str(type(e)) == "<class 'pythonmonkey.SpiderMonkeyError'>"
+    assert str(e).__contains__("TypeError: reduce of empty array with no initial value")
+
 
 def test_reduce_float():
-    items = [1.9, 4.6, 9.3, 16.5]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.reduce((accumulator, currentValue) => accumulator + currentValue, 0)}")(result, items)
-    assert result[0] == 32.3    
+  items = [1.9, 4.6, 9.3, 16.5]
+  result = [None]
+  pm.eval("""
+    (result, arr) => {
+      result[0] = arr.reduce((accumulator, currentValue) => accumulator + currentValue, 0);
+    }
+  """)(result, items)
+  assert result[0] == 32.3
+
 
 def test_reduce_string():
-    items = ['Hi', 'There']
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.reduce((accumulator, currentValue) => accumulator + currentValue, "")}")(result, items)
-    assert result[0] == 'HiThere'    
+  items = ['Hi', 'There']
+  result = [None]
+  pm.eval("""
+      (result, arr) => {
+        result[0] = arr.reduce((accumulator, currentValue) => accumulator + currentValue, "");
+      }
+  """)(result, items)
+  assert result[0] == 'HiThere'
+
 
 def test_reduce_initial_value_not_zero():
-    items = [1,2,3,4,5]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.reduce((accumulator, currentValue) => accumulator + currentValue, 5)}")(result, items)
-    assert items == [1,2,3,4,5]
-    assert result[0] == 20  
+  items = [1, 2, 3, 4, 5]
+  result = [None]
+  pm.eval("""
+    (result, arr) => {
+      result[0] = arr.reduce((accumulator, currentValue) => accumulator + currentValue, 5);
+    }
+  """)(result, items)
+  assert items == [1, 2, 3, 4, 5]
+  assert result[0] == 20
+
 
 def test_reduce_no_initial_value():
-    items = [1,2,3,4,5]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.reduce((accumulator, currentValue) => accumulator + currentValue)}")(result, items)
-    assert items == [1,2,3,4,5]
-    assert result[0] == 15  
+  items = [1, 2, 3, 4, 5]
+  result = [None]
+  pm.eval("""
+    (result, arr) => {
+      result[0] = arr.reduce((accumulator, currentValue) => accumulator + currentValue);
+    }
+  """)(result, items)
+  assert items == [1, 2, 3, 4, 5]
+  assert result[0] == 15
+
 
 def test_reduce_length_one_with_initial_value():
-    items = [1]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.reduce((accumulator, currentValue) => accumulator + currentValue, 2)}")(result, items)
-    assert result[0] == 3       
+  items = [1]
+  result = [None]
+  pm.eval("""
+    (result, arr) => {
+      result[0] = arr.reduce((accumulator, currentValue) => accumulator + currentValue, 2);
+    }
+  """)(result, items)
+  assert result[0] == 3
+
 
 def test_reduce_length_one_no_initial_value():
-    items = [1]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.reduce((accumulator, currentValue) => accumulator + currentValue)}")(result, items)
-    assert result[0] == 1      
+  items = [1]
+  result = [None]
+  pm.eval("""
+    (result, arr) => {
+      result[0] = arr.reduce((accumulator, currentValue) => accumulator + currentValue);
+    }
+  """)(result, items)
+  assert result[0] == 1
+
 
 def test_reduce_list_meaningless():
-    items = [['Hi', 'There']]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.reduce((x) => x * 2)}")(result, items)
-    assert result[0] == ['Hi', 'There']  
+  items = [['Hi', 'There']]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.reduce((x) => x * 2)}")(result, items)
+  assert result[0] == ['Hi', 'There']
+
+# reduceRight
+
 
-#reduceRight
 def test_reduceRight_list_concat():
-    items = [[0, 1],[2, 3],[4, 5]]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.reduceRight((accumulator, currentValue) => accumulator.concat(currentValue))}")(result, items)
-    assert result[0] == [4, 5, 2, 3, 0, 1]
+  items = [[0, 1], [2, 3], [4, 5]]
+  result = [None]
+  pm.eval("""
+    (result, arr) => {
+      result[0] = arr.reduceRight((accumulator, currentValue) => accumulator.concat(currentValue));
+    }
+  """)(result, items)
+  assert result[0] == [4, 5, 2, 3, 0, 1]
+
 
 def test_reduceRight_list_concat_with_initial_value():
-    items = [[0, 1],[2, 3],[4, 5]]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.reduceRight((accumulator, currentValue) => accumulator.concat(currentValue), [7,8])}")(result, items)
-    assert result[0] == [7, 8, 4, 5, 2, 3, 0, 1]
+  items = [[0, 1], [2, 3], [4, 5]]
+  result = [None]
+  pm.eval("""
+    (result, arr) => {
+      result[0] = arr.reduceRight((accumulator, currentValue) => accumulator.concat(currentValue), [7,8]);
+    }
+  """)(result, items)
+  assert result[0] == [7, 8, 4, 5, 2, 3, 0, 1]
+
 
 def test_reduceRight():
-    items = [0,1,2,3,4]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.reduceRight((accumulator, currentValue, index, array) => accumulator + currentValue)}")(result, items)
-    assert result[0] == 10  
+  items = [0, 1, 2, 3, 4]
+  result = [None]
+  pm.eval("""
+    (result, arr) => {
+      result[0] = arr.reduceRight((accumulator, currentValue, index, array) => accumulator + currentValue);
+    }
+  """)(result, items)
+  assert result[0] == 10
+
 
 def test_reduceRight_with_initial_value():
-    items = [0,1,2,3,4]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.reduceRight((accumulator, currentValue, index, array) => accumulator + currentValue, 5)}")(result, items)
-    assert result[0] == 15        
+  items = [0, 1, 2, 3, 4]
+  result = [None]
+  pm.eval("""
+    (result, arr) => {
+      result[0] = arr.reduceRight((accumulator, currentValue, index, array) => accumulator + currentValue, 5);
+    }
+  """)(result, items)
+  assert result[0] == 15
+
 
 def test_reduceRight_float():
-    items = [1.9, 4.6, 9.3, 16.5]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.reduceRight((accumulator, currentValue, index, array) => accumulator + currentValue)}")(result, items)
-    assert result[0] == 32.3    
+  items = [1.9, 4.6, 9.3, 16.5]
+  result = [None]
+  pm.eval("""
+    (result, arr) => {
+      result[0] = arr.reduceRight((accumulator, currentValue, index, array) => accumulator + currentValue);
+    }
+  """)(result, items)
+  assert result[0] == 32.3
+
 
 def test_reduceRight_check_index():
-    items = [1.9, 4.6, 9.3, 16.5]
-    result = ['']
-    pm.eval("(result, arr) => {arr.reduceRight((accumulator, currentValue, index, array) => {accumulator + currentValue; result[0] += index})}")(result, items)
-    assert result[0] == '210'    
+  items = [1.9, 4.6, 9.3, 16.5]
+  result = ['']
+  pm.eval("""
+    (result, arr) => {
+      arr.reduceRight((accumulator, currentValue, index, array) => {
+        accumulator + currentValue;
+        result[0] += index
+      });
+    }
+  """)(result, items)
+  assert result[0] == '210'
+
 
 def test_reduceRight_check_array():
-    items = ['Four', 'Three', 'One'] 
-    result = [None]
-    pm.eval("(result, arr) => {arr.reduceRight((accumulator, currentValue, index, array) => {accumulator + currentValue; result[0] = array})}")(result, items)
-    assert result == [items]
-    assert result[0] is items        
+  items = ['Four', 'Three', 'One']
+  result = [None]
+  pm.eval("""
+    (result, arr) => {
+      arr.reduceRight((accumulator, currentValue, index, array) => {
+          accumulator + currentValue;
+          result[0] = array;
+      });
+    }
+  """)(result, items)
+  assert result == [items]
+  assert result[0] is items
+
+# some
+
 
-#some
 def test_some_true():
-    items = [1, 2, 3, 4, 5]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.some((element) => element % 2 === 0)}")(result, items)
-    assert items == [1, 2, 3, 4, 5]
-    assert result[0] == True    
+  items = [1, 2, 3, 4, 5]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.some((element) => element % 2 === 0)}")(result, items)
+  assert items == [1, 2, 3, 4, 5]
+  assert result[0]
+
 
 def test_some_false():
-    items = [1,3,5]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.some((element) => element % 2 === 0)}")(result, items)
-    assert result[0] == False  
+  items = [1, 3, 5]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.some((element) => element % 2 === 0)}")(result, items)
+  assert not result[0]
+
 
 def test_some_check_index():
-    items = [4,2,6,7]
-    result = ['']
-    pm.eval("(result, arr) => {arr.some((x, index) => result[0] += index)}")(result, items)
-    assert items == [4,2,6,7]
-    assert result[0] == '0123'
+  items = [4, 2, 6, 7]
+  result = ['']
+  pm.eval("(result, arr) => {arr.some((x, index) => result[0] += index)}")(result, items)
+  assert items == [4, 2, 6, 7]
+  assert result[0] == '0123'
+
 
 def test_some_check_array():
-    items = ['Four', 'Three', 'One'] 
-    result = ['']
-    pm.eval("(result, arr) => {arr.some((element, index, array) => result[0] = array)}")(result, items)
-    assert result == [items]
-    assert result[0] is items    
+  items = ['Four', 'Three', 'One']
+  result = ['']
+  pm.eval("(result, arr) => {arr.some((element, index, array) => result[0] = array)}")(result, items)
+  assert result == [items]
+  assert result[0] is items
+
 
 def test_some_check_this_arg():
   items = ['Four', 'Three', 'One']
   result = [None]
   pm.eval(
     """
     (result, arr) => {
@@ -1350,126 +1650,140 @@
       }
       const obj = new Counter();
       obj.add(arr);
       result[0] = obj.count;
     }
     """
   )(result, items)
-  assert result == [3]       
+  assert result == [3]
+
 
 def test_some_truthy_conversion():
-    result = [None]
-    pm.eval(
-      """
+  result = [None]
+  pm.eval(
+    """
       (result) => {
         const TRUTHY_VALUES = [true, "true", 1, {}];
         function getBoolean(value) {
           if (typeof value === "string") {
             value = value.toLowerCase().trim();
-          } 
+          }
            return TRUTHY_VALUES.some((t) => t === value);
         }
         result[0] = getBoolean(1);
       }
     """)(result)
-    assert result[0] == True  
+  assert result[0]
+
 
 def test_some_with_python_function():
-   def func(element, index, array):
-      array[int(index)] = "to each his own"
-      return False
-   items = ['Four', 'Three', 'One'] 
-   returnResult = [0]
-   pm.eval("(returnResult, arr, func) => {returnResult[0] = arr.some(func)}")(returnResult, items, func)
-   assert items == ['to each his own', 'to each his own', 'to each his own']    
-   assert returnResult == [False]   
+  def func(element, index, array):
+    array[int(index)] = "to each his own"
+    return False
+  items = ['Four', 'Three', 'One']
+  returnResult = [0]
+  pm.eval("(returnResult, arr, func) => {returnResult[0] = arr.some(func)}")(returnResult, items, func)
+  assert items == ['to each his own', 'to each his own', 'to each his own']
+  assert returnResult == [False]
+
 
 def test_some_self_pymethod():
- items = ['Four', 'Three', 'One']
- class Counter:
-   def __init__(self):
-     self.count = 0
-   def increment(self, element, index, array):
-     self.count += 1
-     return False
-  
- obj = Counter()
- assert obj.count == 0
- result = pm.eval("""
+  items = ['Four', 'Three', 'One']
+
+  class Counter:
+    def __init__(self):
+      self.count = 0
+
+    def increment(self, element, index, array):
+      self.count += 1
+      return False
+
+  obj = Counter()
+  assert obj.count == 0
+  result = pm.eval("""
  (arr, increment, result) => {
    let jsObj = {count: 0}
    arr.some(increment, jsObj);
    return jsObj.count;
  }
  """)(items, obj.increment)
- assert obj.count == 0
- assert result == 3    
+  assert obj.count == 0
+  assert result == 3
+
 
 def test_some_self_pyfunction():
   items = ['Four', 'Three', 'One']
+
   def increment(self, element, index, array):
     self.count += 1
     return False
-  
+
   try:
     pm.eval("""
     (arr, increment, result) => {
       let jsObj = {count: 0}
       arr.some(increment, jsObj);
       return jsObj.count;
     }
     """)(items, increment)
     assert False
   except Exception as e:
     assert type(e) is TypeError
-    assert str(e).__contains__("unbound python functions do not have a 'self' to bind") 
+    assert str(e).__contains__("unbound python functions do not have a 'self' to bind")
+
 
 def test_some_self_jsfunction():
   items = ['Four', 'Three', 'One']
-  
+
   result = pm.eval("""
   (arr) => {
     function increment(element, index, array) {
       this.count++;
       return false;
     }
     let jsObj = {count: 0}
     arr.some(increment, jsObj);
     return jsObj.count;
   }
   """)(items)
-  assert result == 3     
+  assert result == 3
+
+# every
+
 
-#every        
 def test_every_true():
-    items = [2,4,6]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.every((element) => element % 2 === 0)}")(result, items)
-    assert items == [2,4,6]
-    assert result[0] == True    
+  items = [2, 4, 6]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.every((element) => element % 2 === 0)}")(result, items)
+  assert items == [2, 4, 6]
+  assert result[0]
+
 
 def test_every_false():
-    items = [1,2,4,6]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.every((element) => element % 2 === 0)}")(result, items)
-    assert result[0] == False    
+  items = [1, 2, 4, 6]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.every((element) => element % 2 === 0)}")(result, items)
+  assert not result[0]
+
 
 def test_every_check_index():
-    items = [4,2,6,7]
-    result = ['']
-    pm.eval("(result, arr) => {arr.every((x, index) => result[0] += index)}")(result, items)
-    assert items == [4,2,6,7]
-    assert result[0] == '0'
+  items = [4, 2, 6, 7]
+  result = ['']
+  pm.eval("(result, arr) => {arr.every((x, index) => result[0] += index)}")(result, items)
+  assert items == [4, 2, 6, 7]
+  assert result[0] == '0'
+
 
 def test_every_check_array():
-    items = ['Four', 'Three', 'One'] 
-    result = ['']
-    pm.eval("(result, arr) => {arr.every((element, index, array) => result[0] = array)}")(result, items)
-    assert result == [items]
-    assert result[0] is items    
+  items = ['Four', 'Three', 'One']
+  result = ['']
+  pm.eval("(result, arr) => {arr.every((element, index, array) => result[0] = array)}")(result, items)
+  assert result == [items]
+  assert result[0] is items
+
 
 def test_every_check_this_arg():
   items = ['Four', 'Three', 'One']
   result = [None]
   pm.eval(
     """
     (result, arr) => {
@@ -1484,114 +1798,128 @@
       }
       const obj = new Counter();
       obj.add(arr);
       result[0] = obj.count;
     }
     """
   )(result, items)
-  assert result == [1]   
+  assert result == [1]
+
 
 def test_every_with_python_function():
-   def func(element, index, array):
-      array[int(index)] = "to each his own"
-      return True
-   items = ['Four', 'Three', 'One'] 
-   returnResult = [0]
-   pm.eval("(returnResult, arr, func) => {returnResult[0] = arr.every(func)}")(returnResult, items, func)
-   assert items == ['to each his own', 'to each his own', 'to each his own']    
-   assert returnResult == [True]   
+  def func(element, index, array):
+    array[int(index)] = "to each his own"
+    return True
+  items = ['Four', 'Three', 'One']
+  returnResult = [0]
+  pm.eval("(returnResult, arr, func) => {returnResult[0] = arr.every(func)}")(returnResult, items, func)
+  assert items == ['to each his own', 'to each his own', 'to each his own']
+  assert returnResult == [True]
+
 
 def test_every_self_pymethod():
- items = ['Four', 'Three', 'One']
- class Counter:
-   def __init__(self):
-     self.count = 0
-   def increment(self, element, index, array):
-     self.count += 1
-     return True
-  
- obj = Counter()
- assert obj.count == 0
- result = pm.eval("""
+  items = ['Four', 'Three', 'One']
+
+  class Counter:
+    def __init__(self):
+      self.count = 0
+
+    def increment(self, element, index, array):
+      self.count += 1
+      return True
+
+  obj = Counter()
+  assert obj.count == 0
+  result = pm.eval("""
  (arr, increment, result) => {
    let jsObj = {count: 0}
    arr.every(increment, jsObj);
    return jsObj.count;
  }
  """)(items, obj.increment)
- assert obj.count == 0
- assert result == 3         
+  assert obj.count == 0
+  assert result == 3
+
 
 def test_every_self_pyfunction():
   items = ['Four', 'Three', 'One']
+
   def increment(self, element, index, array):
     self.count += 1
-  
+
   try:
     pm.eval("""
     (arr, increment, result) => {
       let jsObj = {count: 0}
       arr.every(increment, jsObj);
       return jsObj.count;
     }
     """)(items, increment)
     assert False
   except Exception as e:
     assert type(e) is TypeError
-    assert str(e).__contains__("unbound python functions do not have a 'self' to bind") 
+    assert str(e).__contains__("unbound python functions do not have a 'self' to bind")
+
 
 def test_every_self_jsfunction():
   items = ['Four', 'Three', 'One']
-  
+
   result = pm.eval("""
   (arr) => {
     function increment(element, index, array) {
       this.count++
       return true;
     }
     let jsObj = {count: 0}
     arr.every(increment, jsObj);
     return jsObj.count;
   }
   """)(items)
   assert result == 3
 
-#find
+# find
+
+
 def test_find_found_once():
-    items = [5, 12, 8, 130, 44]
-    result = [0]
-    pm.eval("(result, arr) => {result[0] = arr.find((element) => element > 100)}")(result, items)
-    assert items == [5, 12, 8, 130, 44]
-    assert result[0] == 130  
+  items = [5, 12, 8, 130, 44]
+  result = [0]
+  pm.eval("(result, arr) => {result[0] = arr.find((element) => element > 100)}")(result, items)
+  assert items == [5, 12, 8, 130, 44]
+  assert result[0] == 130
+
 
 def test_find_found_twice():
-    items = [5, 12, 8, 130, 4]
-    result = [0]
-    pm.eval("(result, arr) => {result[0] = arr.find((element) => element > 10)}")(result, items)
-    assert result[0] == 12   
+  items = [5, 12, 8, 130, 4]
+  result = [0]
+  pm.eval("(result, arr) => {result[0] = arr.find((element) => element > 10)}")(result, items)
+  assert result[0] == 12
+
 
 def test_find_not_found():
-    items = [5, 12, 8, 130, 44]
-    result = [0]
-    pm.eval("(result, arr) => {result[0] = arr.find((element) => element > 1000)}")(result, items)
-    assert result[0] is None  
+  items = [5, 12, 8, 130, 44]
+  result = [0]
+  pm.eval("(result, arr) => {result[0] = arr.find((element) => element > 1000)}")(result, items)
+  assert result[0] is None
+
 
 def test_find_check_index():
-    items = [4,2,6,7]
-    result = ['']
-    pm.eval("(result, arr) => {arr.find((x, index) => result[0] += index)}")(result, items)
-    assert items == [4,2,6,7]
-    assert result[0] == '0123'
+  items = [4, 2, 6, 7]
+  result = ['']
+  pm.eval("(result, arr) => {arr.find((x, index) => result[0] += index)}")(result, items)
+  assert items == [4, 2, 6, 7]
+  assert result[0] == '0123'
+
 
 def test_find_check_array():
-    items = ['Four', 'Three', 'One'] 
-    result = ['']
-    pm.eval("(result, arr) => {arr.find((element, index, array) => result[0] = array)}")(result, items)
-    assert result == [items]
-    assert result[0] is items    
+  items = ['Four', 'Three', 'One']
+  result = ['']
+  pm.eval("(result, arr) => {arr.find((element, index, array) => result[0] = array)}")(result, items)
+  assert result == [items]
+  assert result[0] is items
+
 
 def test_find_check_this_arg():
   items = ['Four', 'Three', 'One']
   result = [None]
   pm.eval(
     """
     (result, arr) => {
@@ -1606,115 +1934,129 @@
       }
       const obj = new Counter();
       obj.add(arr);
       result[0] = obj.count;
     }
     """
   )(result, items)
-  assert result == [3]         
+  assert result == [3]
+
 
 def test_find_with_python_function():
-   def func(element, index, array):
-      array[int(index)] = "to each his own"
-      return False
-   items = ['Four', 'Three', 'One'] 
-   returnResult = [0]
-   pm.eval("(returnResult, arr, func) => {returnResult[0] = arr.find(func)}")(returnResult, items, func)
-   assert items == ['to each his own', 'to each his own', 'to each his own']    
-   assert returnResult == [None]   
+  def func(element, index, array):
+    array[int(index)] = "to each his own"
+    return False
+  items = ['Four', 'Three', 'One']
+  returnResult = [0]
+  pm.eval("(returnResult, arr, func) => {returnResult[0] = arr.find(func)}")(returnResult, items, func)
+  assert items == ['to each his own', 'to each his own', 'to each his own']
+  assert returnResult == [None]
+
 
 def test_find_self_pymethod():
- items = ['Four', 'Three', 'One']
- class Counter:
-   def __init__(self):
-     self.count = 0
-   def increment(self, element, index, array):
-     self.count += 1
-     return False
-  
- obj = Counter()
- assert obj.count == 0
- result = pm.eval("""
+  items = ['Four', 'Three', 'One']
+
+  class Counter:
+    def __init__(self):
+      self.count = 0
+
+    def increment(self, element, index, array):
+      self.count += 1
+      return False
+
+  obj = Counter()
+  assert obj.count == 0
+  result = pm.eval("""
  (arr, increment, result) => {
    let jsObj = {count: 0}
    arr.find(increment, jsObj);
    return jsObj.count;
  }
  """)(items, obj.increment)
- assert obj.count == 0
- assert result == 3    
+  assert obj.count == 0
+  assert result == 3
+
 
 def test_find_self_pyfunction():
   items = ['Four', 'Three', 'One']
+
   def increment(self, element, index, array):
     self.count += 1
     return False
-  
+
   try:
     pm.eval("""
     (arr, increment, result) => {
       let jsObj = {count: 0}
       arr.find(increment, jsObj);
       return jsObj.count;
     }
     """)(items, increment)
     assert False
   except Exception as e:
     assert type(e) is TypeError
-    assert str(e).__contains__("unbound python functions do not have a 'self' to bind") 
+    assert str(e).__contains__("unbound python functions do not have a 'self' to bind")
+
 
 def test_find_self_jsfunction():
   items = ['Four', 'Three', 'One']
-  
+
   result = pm.eval("""
   (arr) => {
     function increment(element, index, array) {
       this.count++;
       return false;
     }
     let jsObj = {count: 0}
     arr.find(increment, jsObj);
     return jsObj.count;
   }
   """)(items)
-  assert result == 3       
+  assert result == 3
+
+# findIndex
+
 
-#findIndex
 def test_findIndex_found_once():
-    items = [5, 12, 8, 130, 44]
-    result = [0]
-    pm.eval("(result, arr) => {result[0] = arr.findIndex((element) => element > 100)}")(result, items)
-    assert items == [5, 12, 8, 130, 44]
-    assert result[0] == 3  
+  items = [5, 12, 8, 130, 44]
+  result = [0]
+  pm.eval("(result, arr) => {result[0] = arr.findIndex((element) => element > 100)}")(result, items)
+  assert items == [5, 12, 8, 130, 44]
+  assert result[0] == 3
+
 
 def test_findIndex_found_twice():
-    items = [5, 12, 8, 130, 4]
-    result = [0]
-    pm.eval("(result, arr) => {result[0] = arr.findIndex((element) => element > 10)}")(result, items)
-    assert result[0] == 1    
+  items = [5, 12, 8, 130, 4]
+  result = [0]
+  pm.eval("(result, arr) => {result[0] = arr.findIndex((element) => element > 10)}")(result, items)
+  assert result[0] == 1
+
 
 def test_findIndex_not_found():
-    items = [5, 12, 8, 130, 4]
-    result = [0]
-    pm.eval("(result, arr) => {result[0] = arr.findIndex((element) => element > 1000)}")(result, items)
-    assert result[0] == -1      
+  items = [5, 12, 8, 130, 4]
+  result = [0]
+  pm.eval("(result, arr) => {result[0] = arr.findIndex((element) => element > 1000)}")(result, items)
+  assert result[0] == -1
+
 
 def test_findIndex_check_index():
-    items = [4,2,6,7]
-    result = ['']
-    pm.eval("(result, arr) => {arr.findIndex((x, index) => result[0] += index)}")(result, items)
-    assert items == [4,2,6,7]
-    assert result[0] == '0123'
+  items = [4, 2, 6, 7]
+  result = ['']
+  pm.eval("(result, arr) => {arr.findIndex((x, index) => result[0] += index)}")(result, items)
+  assert items == [4, 2, 6, 7]
+  assert result[0] == '0123'
+
 
 def test_findIndex_check_array():
-    items = ['Four', 'Three', 'One'] 
-    result = ['']
-    pm.eval("(result, arr) => {arr.findIndex((element, index, array) => result[0] = array)}")(result, items)
-    assert result == [items]
-    assert result[0] is items    
+  items = ['Four', 'Three', 'One']
+  result = ['']
+  pm.eval("(result, arr) => {arr.findIndex((element, index, array) => result[0] = array)}")(result, items)
+  assert result == [items]
+  assert result[0] is items
+
 
 def test_findIndex_check_this_arg():
   items = ['Four', 'Three', 'One']
   result = [None]
   pm.eval(
     """
     (result, arr) => {
@@ -1729,169 +2071,193 @@
       }
       const obj = new Counter();
       obj.add(arr);
       result[0] = obj.count;
     }
     """
   )(result, items)
-  assert result == [3]      
+  assert result == [3]
+
 
 def test_findIndex_with_python_function():
-   def func(element, index, array):
-      array[int(index)] = "to each his own"
-   items = ['Four', 'Three', 'One'] 
-   returnResult = [0]
-   pm.eval("(returnResult, arr, func) => {returnResult[0] = arr.findIndex(func)}")(returnResult, items, func)
-   assert items == ['to each his own', 'to each his own', 'to each his own']    
-   assert returnResult == [-1]   
+  def func(element, index, array):
+    array[int(index)] = "to each his own"
+  items = ['Four', 'Three', 'One']
+  returnResult = [0]
+  pm.eval("(returnResult, arr, func) => {returnResult[0] = arr.findIndex(func)}")(returnResult, items, func)
+  assert items == ['to each his own', 'to each his own', 'to each his own']
+  assert returnResult == [-1]
+
 
 def test_findIndex_self_pymethod():
- items = ['Four', 'Three', 'One']
- class Counter:
-   def __init__(self):
-     self.count = 0
-   def increment(self, element, index, array):
-     self.count += 1
-  
- obj = Counter()
- assert obj.count == 0
- result = pm.eval("""
+  items = ['Four', 'Three', 'One']
+
+  class Counter:
+    def __init__(self):
+      self.count = 0
+
+    def increment(self, element, index, array):
+      self.count += 1
+
+  obj = Counter()
+  assert obj.count == 0
+  result = pm.eval("""
  (arr, increment, result) => {
    let jsObj = {count: 0}
    arr.findIndex(increment, jsObj);
    return jsObj.count;
  }
  """)(items, obj.increment)
- assert obj.count == 0
- assert result == 3    
+  assert obj.count == 0
+  assert result == 3
+
 
 def test_findIndex_self_pyfunction():
   items = ['Four', 'Three', 'One']
+
   def increment(self, element, index, array):
     self.count += 1
-  
+
   try:
     pm.eval("""
     (arr, increment, result) => {
       let jsObj = {count: 0}
       arr.findIndex(increment, jsObj);
       return jsObj.count;
     }
     """)(items, increment)
     assert False
   except Exception as e:
     assert type(e) is TypeError
-    assert str(e).__contains__("unbound python functions do not have a 'self' to bind") 
+    assert str(e).__contains__("unbound python functions do not have a 'self' to bind")
+
 
 def test_findIndex_self_jsfunction():
   items = ['Four', 'Three', 'One']
-  
+
   result = pm.eval("""
   (arr) => {
     function increment(element, index, array) {
       this.count++
     }
     let jsObj = {count: 0}
     arr.findIndex(increment, jsObj);
     return jsObj.count;
   }
   """)(items)
-  assert result == 3         
+  assert result == 3
+
+# flat
+
 
-#flat
 def test_flat():
-    items = [0, 1, 2, [3, 4]]
-    result = [0]
-    pm.eval("(result, arr) => {result[0] = arr.flat()}")(result, items)
-    assert items == [0, 1, 2, [3, 4]]
-    assert result[0] == [0, 1, 2, 3, 4]
+  items = [0, 1, 2, [3, 4]]
+  result = [0]
+  pm.eval("(result, arr) => {result[0] = arr.flat()}")(result, items)
+  assert items == [0, 1, 2, [3, 4]]
+  assert result[0] == [0, 1, 2, 3, 4]
+
 
 def test_flat_with_js_array():
-    items = [0, 1, 2, [3, 4]]
-    result = [0]
-    pm.eval("(result, arr) => {arr[1] = [10,11]; result[0] = arr.flat()}")(result, items)
-    assert items == [0, [10, 11], 2, [3, 4]]
-    assert result[0] == [0, 10, 11, 2, 3, 4]
+  items = [0, 1, 2, [3, 4]]
+  result = [0]
+  pm.eval("(result, arr) => {arr[1] = [10,11]; result[0] = arr.flat()}")(result, items)
+  assert items == [0, [10, 11], 2, [3, 4]]
+  assert result[0] == [0, 10, 11, 2, 3, 4]
+
 
 def test_flat_depth_zero():
-    items = [0, 1, [2, [3, [4, 5]]]]
-    result = [0]
-    pm.eval("(result, arr) => {result[0] = arr.flat(0)}")(result, items)
-    assert result[0] == [0, 1, [2, [3, [4, 5]]]]
+  items = [0, 1, [2, [3, [4, 5]]]]
+  result = [0]
+  pm.eval("(result, arr) => {result[0] = arr.flat(0)}")(result, items)
+  assert result[0] == [0, 1, [2, [3, [4, 5]]]]
+
 
 def test_flat_depth_one():
-    items = [0, 1, [2, [3, [4, 5]]]]
-    result = [0]
-    pm.eval("(result, arr) => {result[0] = arr.flat(1)}")(result, items)
-    assert items == [0, 1, [2, [3, [4, 5]]]]
-    assert result[0] == [0, 1, 2, [3, [4, 5]]]    
+  items = [0, 1, [2, [3, [4, 5]]]]
+  result = [0]
+  pm.eval("(result, arr) => {result[0] = arr.flat(1)}")(result, items)
+  assert items == [0, 1, [2, [3, [4, 5]]]]
+  assert result[0] == [0, 1, 2, [3, [4, 5]]]
+
 
 def test_flat_depth_two():
-    items = [0, 1, [2, [3, [4, 5]]]]
-    result = [0]
-    pm.eval("(result, arr) => {result[0] = arr.flat(2)}")(result, items)
-    assert items == [0, 1, [2, [3, [4, 5]]]]
-    assert result[0] == [0, 1, 2, 3, [4, 5]]    
+  items = [0, 1, [2, [3, [4, 5]]]]
+  result = [0]
+  pm.eval("(result, arr) => {result[0] = arr.flat(2)}")(result, items)
+  assert items == [0, 1, [2, [3, [4, 5]]]]
+  assert result[0] == [0, 1, 2, 3, [4, 5]]
+
 
 def test_flat_depth_large():
-    items = [0, 1, [2, [3, [4, 5]]]]
-    result = [0]
-    pm.eval("(result, arr) => {result[0] = arr.flat(10)}")(result, items)
-    assert result[0] == [0, 1, 2, 3, 4, 5]      
+  items = [0, 1, [2, [3, [4, 5]]]]
+  result = [0]
+  pm.eval("(result, arr) => {result[0] = arr.flat(10)}")(result, items)
+  assert result[0] == [0, 1, 2, 3, 4, 5]
+
+# flatMap
+
 
-#flatMap
 def test_flatMap():
-    items = [1, 2, 1]
-    result = [0]
-    pm.eval("(result, arr) => {result[0] = arr.flatMap((num) => (num === 2 ? [2, 2] : 1))}")(result, items)
-    assert items == [1,2,1]
-    assert result[0] == [1,2,2,1]
+  items = [1, 2, 1]
+  result = [0]
+  pm.eval("(result, arr) => {result[0] = arr.flatMap((num) => (num === 2 ? [2, 2] : 1))}")(result, items)
+  assert items == [1, 2, 1]
+  assert result[0] == [1, 2, 2, 1]
+
 
 def test_flatMap_with_js_array():
-    items = [1,2,2,1]
-    result = [0]
-    pm.eval("(result, arr) => {arr[1] = [10,11]; result[0] = arr.flatMap((num) => (num === 2 ? [2, 2] : 1))}")(result, items)
-    assert items == [1, [10, 11], 2, 1]
-    assert result[0] == [1, 1, 2, 2, 1]  
+  items = [1, 2, 2, 1]
+  result = [0]
+  pm.eval("(result, arr) => {arr[1] = [10,11]; result[0] = arr.flatMap((num) => (num === 2 ? [2, 2] : 1))}")(
+    result, items)
+  assert items == [1, [10, 11], 2, 1]
+  assert result[0] == [1, 1, 2, 2, 1]
+
 
 def test_flatMap_no_replace():
-    items = [1,2,[4,5]]
-    result = [0]
-    pm.eval("(result, arr) => {result[0] = arr.flatMap((num) => (num === 2 ? [2, 2] : 1))}")(result, items)
-    assert items == [1, 2, [4, 5]]
-    assert result[0] == [1, 2, 2, 1]    
+  items = [1, 2, [4, 5]]
+  result = [0]
+  pm.eval("(result, arr) => {result[0] = arr.flatMap((num) => (num === 2 ? [2, 2] : 1))}")(result, items)
+  assert items == [1, 2, [4, 5]]
+  assert result[0] == [1, 2, 2, 1]
+
 
 def test_flatMap_no_replace_depth_one():
-    items = [1,2,[4,5]]
-    result = [0]
-    pm.eval("(result, arr) => {result[0] = arr.flatMap((num) => (num === 2 ? [2, [2, 2]] : 1))}")(result, items)
-    assert items == [1, 2, [4, 5]]
-    assert result[0] == [1, 2, [2, 2], 1]       
- 
+  items = [1, 2, [4, 5]]
+  result = [0]
+  pm.eval("(result, arr) => {result[0] = arr.flatMap((num) => (num === 2 ? [2, [2, 2]] : 1))}")(result, items)
+  assert items == [1, 2, [4, 5]]
+  assert result[0] == [1, 2, [2, 2], 1]
+
+
 def test_flatMap_equivalence():
-    items = [1, 2, 1]
-    result = [0]
-    result2 = [0]
-    pm.eval("(result, arr) => {result[0] = arr.flatMap((num) => (num === 2 ? [2, 2] : 1))}")(result, items)
-    pm.eval("(result, arr) => {result[0] = arr.map((num) => (num === 2 ? [2, 2] : 1)).flat()}")(result2, items)
-    assert result[0] == result2[0]   
+  items = [1, 2, 1]
+  result = [0]
+  result2 = [0]
+  pm.eval("(result, arr) => {result[0] = arr.flatMap((num) => (num === 2 ? [2, 2] : 1))}")(result, items)
+  pm.eval("(result, arr) => {result[0] = arr.map((num) => (num === 2 ? [2, 2] : 1)).flat()}")(result2, items)
+  assert result[0] == result2[0]
+
 
 def test_flatMap_check_index():
-    items = [4,2,6,7]
-    result = ['']
-    pm.eval("(result, arr) => {arr.flatMap((x, index) => result[0] += index)}")(result, items)
-    assert items == [4,2,6,7]
-    assert result[0] == '0123'
+  items = [4, 2, 6, 7]
+  result = ['']
+  pm.eval("(result, arr) => {arr.flatMap((x, index) => result[0] += index)}")(result, items)
+  assert items == [4, 2, 6, 7]
+  assert result[0] == '0123'
+
 
 def test_flatMap_check_array():
-    items = ['Four', 'Three', 'One'] 
-    result = ['']
-    pm.eval("(result, arr) => {arr.flatMap((element, index, array) => result[0] = array)}")(result, items)
-    assert result == [items]
-    assert result[0] is items    
+  items = ['Four', 'Three', 'One']
+  result = ['']
+  pm.eval("(result, arr) => {arr.flatMap((element, index, array) => result[0] = array)}")(result, items)
+  assert result == [items]
+  assert result[0] is items
+
 
 def test_flatMap_check_this_arg():
   items = ['Four', 'Three', 'One']
   result = [None]
   pm.eval(
     """
     (result, arr) => {
@@ -1906,268 +2272,407 @@
       }
       const obj = new Counter();
       obj.add(arr);
       result[0] = obj.count;
     }
     """
   )(result, items)
-  assert result == [3]   
+  assert result == [3]
+
 
 def test_flatMap_with_python_function():
-   def func(element, index, array):
-      array[int(index)] = "to each his own"
-      return 42
-   items = ['Four', 'Three', 'One'] 
-   returnResult = [0]
-   pm.eval("(returnResult, arr, func) => {returnResult[0] = arr.flatMap(func)}")(returnResult, items, func)
-   assert items == ['to each his own', 'to each his own', 'to each his own']    
-   assert returnResult == [[42.0, 42.0, 42.0]]
+  def func(element, index, array):
+    array[int(index)] = "to each his own"
+    return 42
+  items = ['Four', 'Three', 'One']
+  returnResult = [0]
+  pm.eval("(returnResult, arr, func) => {returnResult[0] = arr.flatMap(func)}")(returnResult, items, func)
+  assert items == ['to each his own', 'to each his own', 'to each his own']
+  assert returnResult == [[42.0, 42.0, 42.0]]
+
 
 def test_flatMap_self_pymethod():
- items = ['Four', 'Three', 'One']
- class Counter:
-   def __init__(self):
-     self.count = 0
-   def increment(self, element, index, array):
-     self.count += 1
-  
- obj = Counter()
- assert obj.count == 0
- result = pm.eval("""
+  items = ['Four', 'Three', 'One']
+
+  class Counter:
+    def __init__(self):
+      self.count = 0
+
+    def increment(self, element, index, array):
+      self.count += 1
+
+  obj = Counter()
+  assert obj.count == 0
+  result = pm.eval("""
  (arr, increment, result) => {
    let jsObj = {count: 0}
    arr.flatMap(increment, jsObj);
    return jsObj.count;
  }
  """)(items, obj.increment)
- assert obj.count == 0
- assert result == 3    
+  assert obj.count == 0
+  assert result == 3
+
 
 def test_flatMap_self_pyfunction():
   items = ['Four', 'Three', 'One']
+
   def increment(self, element, index, array):
     self.count += 1
-  
+
   try:
     pm.eval("""
     (arr, increment, result) => {
       let jsObj = {count: 0}
       arr.flatMap(increment, jsObj);
       return jsObj.count;
     }
     """)(items, increment)
     assert False
   except Exception as e:
     assert type(e) is TypeError
-    assert str(e).__contains__("unbound python functions do not have a 'self' to bind") 
+    assert str(e).__contains__("unbound python functions do not have a 'self' to bind")
+
 
 def test_flatMap_self_jsfunction():
   items = ['Four', 'Three', 'One']
-  
+
   result = pm.eval("""
   (arr) => {
     function increment(element, index, array) {
       this.count++
     }
     let jsObj = {count: 0}
     arr.flatMap(increment, jsObj);
     return jsObj.count;
   }
   """)(items)
-  assert result == 3                
+  assert result == 3
+
+# valueOf
+
 
-#valueOf
 def test_valueOf():
-    items = [1, 2, 1]
-    result = [0]
-    pm.eval("(result, arr) => {result[0] = arr.valueOf()}")(result, items)
-    assert items == [1,2,1] 
-    assert result[0] is items
+  items = [1, 2, 1]
+  result = [0]
+  pm.eval("(result, arr) => {result[0] = arr.valueOf()}")(result, items)
+  assert items == [1, 2, 1]
+  assert result[0] is items
+
+# toLocaleString
+
 
-#toLocaleString
 def test_toLocaleString():
-    prices = ["￥7", 500, 8123, 12]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.toLocaleString('ja-JP', { style: 'currency', currency: 'JPY' })}")(result, prices)
-    assert result[0] == '￥7,￥500,￥8,123,￥12'   
+  prices = ["￥7", 500, 8123, 12]
+  result = [None]
+  pm.eval("""
+    (result, arr) => {
+      result[0] = arr.toLocaleString('ja-JP', { style: 'currency', currency: 'JPY' });
+    }
+  """)(result, prices)
+  assert result[0] == '￥7,￥500,￥8,123,￥12'
+
 
 def test_toLocaleString_with_none():
-    prices = ["￥7", 500, 8123, None]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.toLocaleString('ja-JP', { style: 'currency', currency: 'JPY' })}")(result, prices)
-    assert result[0] == '￥7,￥500,￥8,123,'     
+  prices = ["￥7", 500, 8123, None]
+  result = [None]
+  pm.eval("""
+    (result, arr) => {
+      result[0] = arr.toLocaleString('ja-JP', { style: 'currency', currency: 'JPY' });
+    }
+  """)(result, prices)
+  assert result[0] == '￥7,￥500,￥8,123,'
+
 
 def test_toLocaleString_with_null():
-    prices = ["￥7", 500, 8123, pm.null]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.toLocaleString('ja-JP', { style: 'currency', currency: 'JPY' })}")(result, prices)
-    assert result[0] == '￥7,￥500,￥8,123,'        
+  prices = ["￥7", 500, 8123, pm.null]
+  result = [None]
+  pm.eval("""
+    (result, arr) => {
+      result[0] = arr.toLocaleString('ja-JP', { style: 'currency', currency: 'JPY' });
+    }
+  """)(result, prices)
+  assert result[0] == '￥7,￥500,￥8,123,'
+
 
 def test_toLocaleString_no_args():
-    prices = ["￥7", 500, 8123, 12]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.toLocaleString()}")(result, prices)
-    assert result[0] == '￥7,500,8,123,12'     
+  prices = ["￥7", 500, 8123, 12]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.toLocaleString()}")(result, prices)
+  assert result[0] == '￥7,500,8,123,12'
+
 
 def test_toLocaleString_one_arg_():
-    prices = ["￥7", 500, 8123, 12]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.toLocaleString('ja-JP')}")(result, prices)
-    assert result[0] == '￥7,500,8,123,12'     
+  prices = ["￥7", 500, 8123, 12]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.toLocaleString('ja-JP')}")(result, prices)
+  assert result[0] == '￥7,500,8,123,12'
+
 
 def test_toLocaleString_one_arg_invalid_locale():
-    prices = ["￥7", 500, 8123, 12]
-    result = [None]
-    try:
-        pm.eval("(result, arr) => {result[0] = arr.toLocaleString('asfasfsafsdf')}")(result, prices)   
-        assert (False)
-    except Exception as e:    
-        assert str(type(e)) == "<class 'pythonmonkey.SpiderMonkeyError'>"
-        assert str(e).__contains__("RangeError: invalid language tag:")       
+  prices = ["￥7", 500, 8123, 12]
+  result = [None]
+  try:
+    pm.eval("(result, arr) => {result[0] = arr.toLocaleString('asfasfsafsdf')}")(result, prices)
+    assert (False)
+  except Exception as e:
+    assert str(type(e)) == "<class 'pythonmonkey.SpiderMonkeyError'>"
+    assert str(e).__contains__("RangeError: invalid language tag:")
+
 
 def test_toLocaleString_two_args_invalid_currency():
-    prices = ["￥7", 500, 8123, 12]
-    result = [None]
-    try:
-        pm.eval("(result, arr) => {result[0] = arr.toLocaleString('ja-JP', { style: 'currency', currency: 'JPYsdagasfgas' })}")(result, prices)    
-        assert (False)
-    except Exception as e:    
-        assert str(type(e)) == "<class 'pythonmonkey.SpiderMonkeyError'>"
-        assert str(e).__contains__("RangeError: invalid currency code in NumberFormat():")       
+  prices = ["￥7", 500, 8123, 12]
+  result = [None]
+  try:
+    pm.eval("""
+      (result, arr) => {
+        result[0] = arr.toLocaleString('ja-JP', { style: 'currency', currency: 'JPYsdagasfgas' });
+      }
+    """)(result, prices)
+    assert (False)
+  except Exception as e:
+    assert str(type(e)) == "<class 'pythonmonkey.SpiderMonkeyError'>"
+    assert str(e).__contains__("RangeError: invalid currency code in NumberFormat():")
+
 
 def test_toLocaleString_with_datetime():
-    prices = [500, datetime(year=2020, month=1, day=31, hour=13, minute=14, second=31)]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr.toLocaleString('en-uk')}")(result, prices)
-    assert result[0] == '500,31/01/2020, 13:14:31'          
+  prices = [500, datetime(year=2020, month=1, day=31, hour=13, minute=14, second=31)]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr.toLocaleString('en-uk')}")(result, prices)
+  assert result[0] == '500,31/01/2020, 13:14:31'
+
+# entries
+
 
-#entries
 def test_entries_next():
-    items = ['a', 'b', 'c']
-    result = [0]
-    pm.eval("(result, arr) => {result[0] = arr.entries(); result[0] = result[0].next().value}")(result, items)
-    assert items == ['a', 'b', 'c']
-    assert result[0] == [0, 'a']      
+  items = ['a', 'b', 'c']
+  result = [0]
+  pm.eval("(result, arr) => {result[0] = arr.entries(); result[0] = result[0].next().value}")(result, items)
+  assert items == ['a', 'b', 'c']
+  assert result[0] == [0, 'a']
+
 
 def test_entries_next_next():
-    items = ['a', 'b', 'c']
-    result = [0]
-    pm.eval("(result, arr) => {result[0] = arr.entries(); result[0].next(); result[0] = result[0].next().value}")(result, items)
-    assert result[0] == [1, 'b']    
+  items = ['a', 'b', 'c']
+  result = [0]
+  pm.eval("(result, arr) => {result[0] = arr.entries(); result[0].next(); result[0] = result[0].next().value}")(
+    result, items)
+  assert result[0] == [1, 'b']
+
 
 def test_entries_next_next_undefined():
-    items = ['a']
-    result = [0]
-    pm.eval("(result, arr) => {result[0] = arr.entries(); result[0].next(); result[0] = result[0].next().value}")(result, items)
-    assert result[0] == None    
+  items = ['a']
+  result = [0]
+  pm.eval("(result, arr) => {result[0] = arr.entries(); result[0].next(); result[0] = result[0].next().value}")(
+    result, items)
+  assert result[0] is None
+
+# keys
+
 
-#keys
 def test_keys_iterator():
-    items = ['a', 'b', 'c']
-    result = [7,8,9]
-    pm.eval("(result, arr) => { index = 0; iterator = arr.keys(); for (const key of iterator) { result[index] = key; index++;} }")(result, items)
-    assert result == [0,1,2]    
+  items = ['a', 'b', 'c']
+  result = [7, 8, 9]
+  pm.eval("""
+    (result, arr) => {
+      index = 0;
+      iterator = arr.keys();
+      for (const key of iterator) {
+        result[index] = key;
+        index++;
+      }
+    }
+  """)(result, items)
+  assert result == [0, 1, 2]
+
+# values
+
 
-#values
 def test_values_iterator():
-    items = ['a', 'b', 'c']
-    result = [7,8,9]
-    pm.eval("(result, arr) => { index = 0; iterator = arr.values(); for (const value of iterator) { result[index] = value; index++;} }")(result, items)
-    assert result == ['a', 'b', 'c']
-    assert result is not items
-    
-#constructor property
+  items = ['a', 'b', 'c']
+  result = [7, 8, 9]
+  pm.eval("""
+    (result, arr) => {
+      index = 0;
+      iterator = arr.values();
+      for (const value of iterator) {
+        result[index] = value;
+        index++;
+      }
+    }
+  """)(result, items)
+  assert result == ['a', 'b', 'c']
+  assert result is not items
+
+# constructor property
+
+
 def test_constructor_creates_array():
-    items = [1,2]
-    result = [0]
-    pm.eval("(result, arr) => { result[0] = arr.constructor; result[0] = new result[0]; result[0][0] = 9}")(result, items)
-    assert result[0] == [9]     
+  items = [1, 2]
+  result = [0]
+  pm.eval("(result, arr) => { result[0] = arr.constructor; result[0] = new result[0]; result[0][0] = 9}")(result, items)
+  assert result[0] == [9]
+
+# length property
+
 
-#length property
 def test_constructor_creates_array():
-    items = [1,2]
-    result = [0]
-    pm.eval("(result, arr) => { result[0] = arr.length}")(result, items)
-    assert result[0] == 2      
+  items = [1, 2]
+  result = [0]
+  pm.eval("(result, arr) => { result[0] = arr.length}")(result, items)
+  assert result[0] == 2
+
+# iterator symbol property
+
 
-#iterator symbol property
 def test_iterator_type_function():
-    items = [1,2]
-    result = [0]
-    pm.eval("(result, arr) => { result[0] = typeof arr[Symbol.iterator]}")(result, items)
-    assert result[0] == 'function'         
+  items = [1, 2]
+  result = [0]
+  pm.eval("(result, arr) => { result[0] = typeof arr[Symbol.iterator]}")(result, items)
+  assert result[0] == 'function'
+
 
 def test_iterator_first_next():
-    items = [1,2]
-    result = [0]
-    pm.eval("(result, arr) => { result[0] = arr[Symbol.iterator]().next()}")(result, items)
-    assert result[0].value == 1    
-    assert result[0].done == False     
+  items = [1, 2]
+  result = [0]
+  pm.eval("(result, arr) => { result[0] = arr[Symbol.iterator]().next()}")(result, items)
+  assert result[0].value == 1
+  assert not result[0].done
+
 
 def test_iterator_second_next():
-    items = [1,2]
-    result = [0]
-    pm.eval("(result, arr) => { let iterator = arr[Symbol.iterator](); iterator.next(); result[0] = iterator.next()}")(result, items)
-    assert result[0].value == 2    
-    assert result[0].done == False 
+  items = [1, 2]
+  result = [0]
+  pm.eval("(result, arr) => { let iterator = arr[Symbol.iterator](); iterator.next(); result[0] = iterator.next()}")(
+    result, items)
+  assert result[0].value == 2
+  assert not result[0].done
+
 
 def test_iterator_last_next():
-    items = [1,2]
-    result = [0]
-    pm.eval("(result, arr) => { let iterator = arr[Symbol.iterator](); iterator.next(); iterator.next(); result[0] = iterator.next()}")(result, items)
-    assert result[0].value == None
-    assert result[0].done == True      
+  items = [1, 2]
+  result = [0]
+  pm.eval("""
+    (result, arr) => {
+      let iterator = arr[Symbol.iterator]();
+      iterator.next();
+      iterator.next();
+      result[0] = iterator.next();
+    }
+  """)(result, items)
+  assert result[0].value is None
+  assert result[0].done
+
 
 def test_iterator_iterator():
-    items = [1,2,3,4]
-    result = [0]
-    pm.eval("(result, arr) => {let iter = arr[Symbol.iterator](); let head = iter.next().value; result[0] = [...iter] }")(result, items)
-    assert result[0] == [2,3,4]        
+  items = [1, 2, 3, 4]
+  result = [0]
+  pm.eval("(result, arr) => {let iter = arr[Symbol.iterator](); let head = iter.next().value; result[0] = [...iter] }")(
+    result, items)
+  assert result[0] == [2, 3, 4]
+
+# Array.from
+
 
-#Array.from
 def test_array_from():
-    items = [1,2]
-    result = [0]
-    pm.eval("(result, arr) => { result[0] = Array.from(arr)}")(result, items)
-    assert result[0] == [1,2]
-    assert result[0] is not items    
+  items = [1, 2]
+  result = [0]
+  pm.eval("(result, arr) => { result[0] = Array.from(arr)}")(result, items)
+  assert result[0] == [1, 2]
+  assert result[0] is not items
 
 # bad index size expansion
+
+
 def test_assign_bad_index():
-    items = [1,2,3]
-    result = []
-    pm.eval("(result, arr) => {result[0] = 4}")(result, items) 
-    assert result[0] == 4
+  result = []
+  pm.eval("(result) => {result[0] = 4}")(result)
+  assert result[0] == 4
+
 
 def test_assign_bad_index_with_existing_next():
-    items = [1,2,3]
-    result = [8]
-    pm.eval("(result, arr) => {result[1] = 4}")(result, items) 
-    assert result == [8,4]    
+  result = [8]
+  pm.eval("(result) => {result[1] = 4}")(result)
+  assert result == [8, 4]
+
 
 def test_assign_bad_index_with_gap():
-    items = [1,2,3]
-    result = []
-    pm.eval("(result, arr) => {result[0] = 4; result[5] = 6}")(result, items) 
-    assert result == [4, None, None, None, None, 6]
+  result = []
+  pm.eval("(result) => {result[0] = 4; result[5] = 6}")(result)
+  assert result == [4, None, None, None, None, 6]
+
 
 def test_array_subclass_behaves_as_array():
-     my_JS_function = pm.eval("""
+  my_JS_function = pm.eval("""
                       () => {
                         class MyClass extends Array {
                           constructor(...args)
                           {
                             super(...args);
                             return this;
                           }
                         }
                         return new MyClass(1,2);
                       }
                       """)
-     
-     a = my_JS_function()
-     assert a == [1,2]
-     result = []
-     for i in a:
-        result.append(i)
-     assert result == [1,2]
-     assert a is not result
+
+  a = my_JS_function()
+  assert a == [1, 2]
+  result = []
+  for i in a:
+    result.append(i)
+  assert result == [1, 2]
+  assert a is not result
+
+
+def test_iter_operator_tuple():
+  myit = iter((1, 2))
+  result = [None, None, None]
+  pm.eval('(result, myit) => { result[0] = myit.next(); result[1] = myit.next(); result[2] = myit.next()}')(
+    result, myit)
+  assert result[0] == {'done': False, 'value': 1.0}
+  assert result[1] == {'done': False, 'value': 2.0}
+  assert result[2] == {'done': True}
+
+
+def test_iter_operator_array():
+  myit = iter([1, 2, 3])
+  result = [None, None, None, None]
+  pm.eval("""
+    (result, myit) => {
+      result[0] = myit.next();
+      result[1] = myit.next();
+      result[2] = myit.next();
+      result[3] = myit.next();
+    }
+  """)(result, myit)
+  assert result[0] == {'done': False, 'value': 1.0}
+  assert result[1] == {'done': False, 'value': 2.0}
+  assert result[2] == {'done': False, 'value': 3.0}
+  assert result[3] == {'done': True}
+
+
+def test_iter_reentrance():
+  myit = iter((1, 2))
+  result = pm.eval("(iter) => iter")(myit)
+  assert myit is result
+
+
+def test_iter_reentrace_next():
+  myit = iter((1, 2))
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr}")(result, myit)
+  next(result[0]) == 1
+  next(result[0]) == 2
+  try:
+    third = next(result[0])
+    assert (False)
+  except StopIteration as e:
+    assert (True)
+
+
+def test_iter_for_of():
+  myit = iter((1, 2))
+  result = [None, None]
+  pm.eval("""(result, myit) => {let index = 0; for (const value of myit) {result[index++] = value}}""")(result, myit)
+  assert result[0] == 1.0
+  assert result[1] == 2.0
```

### Comparing `pythonmonkey-0.4.0/tests/python/test_bigints.py` & `pythonmonkey-0.6.0/tests/python/test_bigints.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,143 +1,156 @@
 import pytest
 import pythonmonkey as pm
 import random
 
-def test_eval_numbers_bigints():
-    def test_bigint(py_number: int):
-        js_number = pm.eval(f'{repr(py_number)}n')
-        assert py_number == js_number
-
-    test_bigint(0)
-    test_bigint(1)
-    test_bigint(-1)
-
-    # CPython would reuse the objects for small ints in range [-5, 256] 
-    # Making sure we don't do any changes on them
-    def test_cached_int_object(py_number):
-        # type is still int
-        assert type(py_number) == int
-        assert type(py_number) != pm.bigint
-        test_bigint(py_number)
-        assert type(py_number) == int
-        assert type(py_number) != pm.bigint
-        # the value doesn't change
-        # TODO (Tom Tang): Find a way to create a NEW int object with the same value, because int literals also reuse the cached int objects
-    for _ in range(2):
-        test_cached_int_object(0) # _PyLong_FromByteArray reuses the int 0 object,
-                                  # see https://github.com/python/cpython/blob/3.9/Objects/longobject.c#L862
-        for i in range(10):
-            test_cached_int_object(random.randint(-5, 256))
-
-    test_bigint(18014398509481984)      #  2**54
-    test_bigint(-18014398509481984)     # -2**54
-    test_bigint(18446744073709551615)   #  2**64-1
-    test_bigint(18446744073709551616)   #  2**64
-    test_bigint(-18446744073709551617)  # -2**64-1
 
-    limit = 2037035976334486086268445688409378161051468393665936250636140449354381299763336706183397376
-    #     = 2**300
+def test_eval_numbers_bigints():
+  def test_bigint(py_number: int):
+    js_number = pm.eval(f'{repr(py_number)}n')
+    assert py_number == js_number
+
+  test_bigint(0)
+  test_bigint(1)
+  test_bigint(-1)
+
+  # CPython would reuse the objects for small ints in range [-5, 256]
+  # Making sure we don't do any changes on them
+  def test_cached_int_object(py_number):
+
+    # type is still int
+    assert type(py_number) is int
+    assert not isinstance(py_number, pm.bigint)
+    test_bigint(py_number)
+    assert type(py_number) is int
+    assert not isinstance(py_number, pm.bigint)
+    # the value doesn't change
+   # TODO (Tom Tang): Find a way to create a NEW int object with the same
+   # value, because int literals also reuse the cached int objects
+  for _ in range(2):
+    test_cached_int_object(0)  # _PyLong_FromByteArray reuses the int 0 object,
+    # see https://github.com/python/cpython/blob/3.9/Objects/longobject.c#L862
     for i in range(10):
-        py_number = random.randint(-limit, limit)
-        test_bigint(py_number)
+      test_cached_int_object(random.randint(-5, 256))
+
+  test_bigint(18014398509481984)  # 2**54
+  test_bigint(-18014398509481984)     # -2**54
+  test_bigint(18446744073709551615)  # 2**64-1
+  test_bigint(18446744073709551616)  # 2**64
+  test_bigint(-18446744073709551617)  # -2**64-1
+
+  limit = 2037035976334486086268445688409378161051468393665936250636140449354381299763336706183397376
+  #     = 2**300
+  for i in range(10):
+    py_number = random.randint(-limit, limit)
+    test_bigint(py_number)
+
+  # TODO (Tom Tang): test -0 (negative zero)
+  # There's no -0 in both Python int and JS BigInt,
+  # but this could be possible in JS BigInt's internal representation as it uses a sign bit flag.
+  # On the other hand, Python int uses `ob_size` 0 for 0, >0 for positive values, <0 for negative values
 
-    # TODO (Tom Tang): test -0 (negative zero)
-    # There's no -0 in both Python int and JS BigInt, 
-    # but this could be possible in JS BigInt's internal representation as it uses a sign bit flag.
-    # On the other hand, Python int uses `ob_size` 0 for 0, >0 for positive values, <0 for negative values
 
 def test_eval_boxed_numbers_bigints():
-    def test_boxed_bigint(py_number: int):
-        # `BigInt()` can only be called without `new`
-        #   https://tc39.es/ecma262/#sec-bigint-constructor
-        js_number = pm.eval(f'new Object({repr(py_number)}n)')
-        assert py_number == js_number
-
-    test_boxed_bigint(0)
-    test_boxed_bigint(1)
-    test_boxed_bigint(-1)
+  def test_boxed_bigint(py_number: int):
+    # `BigInt()` can only be called without `new`
+    #   https://tc39.es/ecma262/#sec-bigint-constructor
+    js_number = pm.eval(f'new Object({repr(py_number)}n)')
+    assert py_number == js_number
+
+  test_boxed_bigint(0)
+  test_boxed_bigint(1)
+  test_boxed_bigint(-1)
+
+  limit = 2037035976334486086268445688409378161051468393665936250636140449354381299763336706183397376
+  #     = 2**300
+  for i in range(10):
+    py_number = random.randint(-limit, limit)
+    test_boxed_bigint(py_number)
 
-    limit = 2037035976334486086268445688409378161051468393665936250636140449354381299763336706183397376
-    #     = 2**300
-    for i in range(10):
-        py_number = random.randint(-limit, limit)
-        test_boxed_bigint(py_number)
 
 def test_eval_functions_bigints():
-    ident = pm.eval("(a) => { return a }")
-    add = pm.eval("(a, b) => { return a + b }")
+  ident = pm.eval("(a) => { return a }")
+  add = pm.eval("(a, b) => { return a + b }")
 
-    int1 = random.randint(-1000000,1000000)
-    bigint1 = pm.bigint(int1)
-    assert int1 == bigint1
-
-    # should return pm.bigint
-    assert type(ident(bigint1)) == pm.bigint
-    assert ident(bigint1) is not bigint1
-    # should return float (because JS number is float64)
-    assert type(ident(int1)) == float
-    assert ident(int1) == ident(bigint1)
-
-    # should raise exception on ints > (2^53-1), or < -(2^53-1)
-    def not_raise(num):
-        ident(num)
-    def should_raise(num):
-        with pytest.raises(OverflowError, match="Use pythonmonkey.bigint instead"):
-            ident(num)
-    not_raise(9007199254740991)     #   2**53-1, 0x433_FFFFFFFFFFFFF in float64
-    should_raise(9007199254740992)  #   2**53,   0x434_0000000000000 in float64
-    should_raise(9007199254740993)  #   2**53+1, NOT 0x434_0000000000001 (2**53+2)
-    not_raise(-9007199254740991)    # -(2**53-1)
-    should_raise(-9007199254740992) # -(2**53)
-    should_raise(-9007199254740993) # -(2**53+1)
-
-    # should also raise exception on large integers (>=2**53) that can be exactly represented by a float64
-    #   in our current implementation
-    should_raise(9007199254740994)  #   2**53+2, 0x434_0000000000001 in float64
-    should_raise(2**61+2**9)        #            0x43C_0000000000001 in float64
-
-    # should raise "Use pythonmonkey.bigint" instead of `PyLong_AsLongLong`'s "OverflowError: int too big to convert" on ints larger than 64bits
-    should_raise(2**65)
-    should_raise(-2**65)
-    not_raise(pm.bigint(2**65))
-    not_raise(pm.bigint(-2**65))
-
-    # should raise JS error when mixing a BigInt with a number in arithmetic operations
-    def should_js_error(a, b):
-        with pytest.raises(pm.SpiderMonkeyError, match="can't convert BigInt to number"):
-            add(a, b)
-    should_js_error(pm.bigint(0), 0)
-    should_js_error(pm.bigint(1), 2)
-    should_js_error(3, pm.bigint(4))
-    should_js_error(-5, pm.bigint(6))
-
-    assert add(pm.bigint(0), pm.bigint(0)) == 0
-    assert add(pm.bigint(1), pm.bigint(0)) == 1
-    assert add(pm.bigint(1), pm.bigint(2)) == 3
-    assert add(pm.bigint(-1), pm.bigint(1)) == 0
-    assert add(pm.bigint(2**60), pm.bigint(0)) == 1152921504606846976
-    assert add(pm.bigint(2**65), pm.bigint(-2**65-1)) == -1
+  int1 = random.randint(-1000000, 1000000)
+  bigint1 = pm.bigint(int1)
+  assert int1 == bigint1
+
+  # should return pm.bigint
+  assert type(ident(bigint1)) == pm.bigint
+  assert ident(bigint1) is not bigint1
+  # should return float (because JS number is float64)
+  assert type(ident(int1)) == float
+  assert ident(int1) == ident(bigint1)
+
+  # should raise exception on ints > (2^53-1), or < -(2^53-1)
+  def not_raise(num):
+    ident(num)
+
+  def should_raise(num):
+    with pytest.raises(OverflowError, match="Use pythonmonkey.bigint instead"):
+      ident(num)
+  # autopep8: off
+  not_raise(9007199254740991)      # +(2**53-1),     0x433_FFFFFFFFFFFFF in float64
+  should_raise(9007199254740992)   # +(2**53  ),     0x434_0000000000000 in float64
+  should_raise(9007199254740993)   # +(2**53+1), NOT 0x434_0000000000001 (2**53+2)
+  not_raise(-9007199254740991)     # -(2**53-1)
+  should_raise(-9007199254740992)  # -(2**53  )
+  should_raise(-9007199254740993)  # -(2**53+1)
+  # autopep8: on
+
+  # should also raise exception on large integers (>=2**53) that can be exactly represented by a float64
+  #   in our current implementation
+  # autopep8: off
+  should_raise(9007199254740994)  # 2**53+2, 0x434_0000000000001 in float64
+  should_raise(2**61 + 2**9)      #          0x43C_0000000000001 in float64
+  # autopep8: on
+
+  # should raise "Use pythonmonkey.bigint" instead of `PyLong_AsLongLong`'s
+  # "OverflowError: int too big to convert" on ints larger than 64bits
+  should_raise(2**65)
+  should_raise(-2**65)
+  not_raise(pm.bigint(2**65))
+  not_raise(pm.bigint(-2**65))
+
+  # should raise JS error when mixing a BigInt with a number in arithmetic operations
+  def should_js_error(a, b):
+    with pytest.raises(pm.SpiderMonkeyError, match="can't convert BigInt to number"):
+      add(a, b)
+  should_js_error(pm.bigint(0), 0)
+  should_js_error(pm.bigint(1), 2)
+  should_js_error(3, pm.bigint(4))
+  should_js_error(-5, pm.bigint(6))
+
+  assert add(pm.bigint(0), pm.bigint(0)) == 0
+  assert add(pm.bigint(1), pm.bigint(0)) == 1
+  assert add(pm.bigint(1), pm.bigint(2)) == 3
+  assert add(pm.bigint(-1), pm.bigint(1)) == 0
+  assert add(pm.bigint(2**60), pm.bigint(0)) == 1152921504606846976
+  assert add(pm.bigint(2**65), pm.bigint(-2**65 - 1)) == -1
+
+  # fuzztest
+  limit = 2037035976334486086268445688409378161051468393665936250636140449354381299763336706183397376  # 2**300
+  for i in range(10):
+    num1 = random.randint(-limit, limit)
+    num2 = random.randint(-limit, limit)
+    assert add(pm.bigint(num1), pm.bigint(num2)) == num1 + num2
 
-    # fuzztest
-    limit = 2037035976334486086268445688409378161051468393665936250636140449354381299763336706183397376 # 2**300
-    for i in range(10):
-        num1 = random.randint(-limit, limit)
-        num2 = random.randint(-limit, limit)
-        assert add(pm.bigint(num1), pm.bigint(num2)) == num1+num2
 
 def test_eval_functions_bigint_factorial():
-    factorial = pm.eval("(num) => {let r = 1n; for(let i = 0n; i<num; i++){r *= num - i}; return r}")
-    assert factorial(pm.bigint(1)) == 1
-    assert factorial(pm.bigint(18)) == 6402373705728000
-    assert factorial(pm.bigint(19)) == 121645100408832000 # > Number.MAX_SAFE_INTEGER
-    assert factorial(pm.bigint(21)) == 51090942171709440000 # > 64 bit int
-    assert factorial(pm.bigint(35)) == 10333147966386144929666651337523200000000 # > 128 bit
+  factorial = pm.eval("(num) => {let r = 1n; for(let i = 0n; i<num; i++){r *= num - i}; return r}")
+  assert factorial(pm.bigint(1)) == 1
+  assert factorial(pm.bigint(18)) == 6402373705728000
+  assert factorial(pm.bigint(19)) == 121645100408832000  # > Number.MAX_SAFE_INTEGER
+  assert factorial(pm.bigint(21)) == 51090942171709440000  # > 64 bit int
+  assert factorial(pm.bigint(35)) == 10333147966386144929666651337523200000000  # > 128 bit
+
 
 def test_eval_functions_bigint_crc32():
-    crc_table_at = pm.eval("""
+  crc_table_at = pm.eval("""
     // translated from https://rosettacode.org/wiki/CRC-32#Python
     const crc_table = (function create_table() {
         const a = []
         for (let i = 0n; i < 256n; i++) {
             let k = i
             for (let j = 0n; j < 8n; j++) {
                 // must use bigint here as js number is trimmed to int32 in bitwise operations
@@ -146,11 +159,11 @@
             }
             a.push(k)
         }
         return a
     })();
     (n) => crc_table[n]
     """)
-    assert type(crc_table_at(1)) == pm.bigint
-    assert crc_table_at(0) == 0
-    assert crc_table_at(1) == 1996959894
-    assert crc_table_at(255) == 755167117 # last item
+  assert type(crc_table_at(1)) == pm.bigint
+  assert crc_table_at(0) == 0
+  assert crc_table_at(1) == 1996959894
+  assert crc_table_at(255) == 755167117  # last item
```

### Comparing `pythonmonkey-0.4.0/tests/python/test_buffer_typed_array.py` & `pythonmonkey-0.6.0/tests/python/test_buffer_typed_array.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,198 +1,211 @@
 import pytest
 import pythonmonkey as pm
 import gc
-import numpy, array, struct
+import numpy
+import array
+import struct
+
 
 def test_py_buffer_to_js_typed_array():
-    # JS TypedArray/ArrayBuffer should coerce to Python memoryview type
-    def assert_js_to_py_memoryview(buf: memoryview):
-        assert type(buf) is memoryview
-        assert None == buf.obj # https://docs.python.org/3.9/c-api/buffer.html#c.Py_buffer.obj
-        assert 2 * 4 == buf.nbytes # 2 elements * sizeof(int32_t)
-        assert "02000000ffffffff" == buf.hex() # native (little) endian
-    buf1 = pm.eval("new Int32Array([2,-1])")
-    buf2 = pm.eval("new Int32Array([2,-1]).buffer")
-    assert_js_to_py_memoryview(buf1)
-    assert_js_to_py_memoryview(buf2)
-    assert [2, -1] == buf1.tolist()
-    assert [2, 0, 0, 0, 255, 255, 255, 255] == buf2.tolist()
-    assert -1 == buf1[1]
-    assert 255 == buf2[7]
-    with pytest.raises(IndexError, match="index out of bounds on dimension 1"):
-        buf1[2]
-    with pytest.raises(IndexError, match="index out of bounds on dimension 1"):
-        buf2[8]
-    del buf1, buf2
-
-    # test element value ranges
-    buf3 = pm.eval("new Uint8Array(1)")
-    with pytest.raises(ValueError, match="memoryview: invalid value for format 'B'"):
-        buf3[0] = 256
-    with pytest.raises(ValueError, match="memoryview: invalid value for format 'B'"):
-        buf3[0] = -1
-    with pytest.raises(IndexError, match="index out of bounds on dimension 1"): # no automatic resize
-        buf3[1] = 0
-    del buf3
-
-    # Python buffers should coerce to JS TypedArray
-    # and the typecode maps to TypedArray subtype (Uint8Array, Float64Array, ...)
-    assert True == pm.eval("(arr)=>arr instanceof Uint8Array")( bytearray([1,2,3]) )
-    assert True == pm.eval("(arr)=>arr instanceof Uint8Array")( numpy.array([1], dtype=numpy.uint8) )
-    assert True == pm.eval("(arr)=>arr instanceof Uint16Array")( numpy.array([1], dtype=numpy.uint16) )
-    assert True == pm.eval("(arr)=>arr instanceof Uint32Array")( numpy.array([1], dtype=numpy.uint32) )
-    assert True == pm.eval("(arr)=>arr instanceof BigUint64Array")( numpy.array([1], dtype=numpy.uint64) )
-    assert True == pm.eval("(arr)=>arr instanceof Int8Array")( numpy.array([1], dtype=numpy.int8) )
-    assert True == pm.eval("(arr)=>arr instanceof Int16Array")( numpy.array([1], dtype=numpy.int16) )
-    assert True == pm.eval("(arr)=>arr instanceof Int32Array")( numpy.array([1], dtype=numpy.int32) )
-    assert True == pm.eval("(arr)=>arr instanceof BigInt64Array")( numpy.array([1], dtype=numpy.int64) )
-    assert True == pm.eval("(arr)=>arr instanceof Float32Array")( numpy.array([1], dtype=numpy.float32) )
-    assert True == pm.eval("(arr)=>arr instanceof Float64Array")( numpy.array([1], dtype=numpy.float64) )
-    assert pm.eval("new Uint8Array([1])").format == "B"
-    assert pm.eval("new Uint16Array([1])").format == "H"
-    assert pm.eval("new Uint32Array([1])").format == "I" # FIXME (Tom Tang): this is "L" on 32-bit systems
-    assert pm.eval("new BigUint64Array([1n])").format == "Q"
-    assert pm.eval("new Int8Array([1])").format == "b"
-    assert pm.eval("new Int16Array([1])").format == "h"
-    assert pm.eval("new Int32Array([1])").format == "i"
-    assert pm.eval("new BigInt64Array([1n])").format == "q"
-    assert pm.eval("new Float32Array([1])").format == "f"
-    assert pm.eval("new Float64Array([1])").format == "d"
-
-    # not enough bytes to populate an element of the TypedArray
-    with pytest.raises(pm.SpiderMonkeyError, match="RangeError: buffer length for BigInt64Array should be a multiple of 8"):
-        pm.eval("(arr) => new BigInt64Array(arr.buffer)")(array.array('i', [-11111111]))
-
-    # TypedArray with `byteOffset` and `length`
-    arr1 = array.array('i', [-11111111, 22222222, -33333333, 44444444])
-    with pytest.raises(pm.SpiderMonkeyError, match="RangeError: invalid or out-of-range index"):
-        pm.eval("(arr) => new Int32Array(arr.buffer, /*byteOffset*/ -4)")(arr1)
-    with pytest.raises(pm.SpiderMonkeyError, match="RangeError: start offset of Int32Array should be a multiple of 4"):
-        pm.eval("(arr) => new Int32Array(arr.buffer, /*byteOffset*/ 1)")(arr1)
-    with pytest.raises(pm.SpiderMonkeyError, match="RangeError: size of buffer is too small for Int32Array with byteOffset"):
-        pm.eval("(arr) => new Int32Array(arr.buffer, /*byteOffset*/ 20)")(arr1)
-    with pytest.raises(pm.SpiderMonkeyError, match="RangeError: invalid or out-of-range index"):
-        pm.eval("(arr) => new Int32Array(arr.buffer, /*byteOffset*/ 4, /*length*/ -1)")(arr1)
-    with pytest.raises(pm.SpiderMonkeyError, match="RangeError: attempting to construct out-of-bounds Int32Array on ArrayBuffer"):
-        pm.eval("(arr) => new Int32Array(arr.buffer, /*byteOffset*/ 4, /*length*/ 4)")(arr1)
-    arr2 = pm.eval("(arr) => new Int32Array(arr.buffer, /*byteOffset*/ 4, /*length*/ 2)")(arr1)
-    assert 2 * 4 == arr2.nbytes # 2 elements * sizeof(int32_t)
-    assert [22222222, -33333333] == arr2.tolist()
-    assert "8e155301ab5f03fe" == arr2.hex() # native (little) endian
-    assert 22222222 == arr2[0] # offset 1 int32
-    with pytest.raises(IndexError, match="index out of bounds on dimension 1"):
-        arr2[2]
-    arr3 = pm.eval("(arr) => new Int32Array(arr.buffer, 16 /* byteOffset */)")(arr1) # empty Int32Array
-    assert 0 == arr3.nbytes
-    del arr3
-
-    # test GC
-    del arr1
-    gc.collect(), pm.collect()
-    gc.collect(), pm.collect()
-    # TODO (Tom Tang): the 0th element in the underlying buffer is still accessible after GC, even is not referenced by the JS TypedArray with byteOffset
-    del arr2
-
-    # mutation
-    mut_arr_original = bytearray(4)
-    pm.eval("""
+  # JS TypedArray/ArrayBuffer should coerce to Python memoryview type
+  def assert_js_to_py_memoryview(buf: memoryview):
+    assert type(buf) is memoryview
+    assert None is buf.obj  # https://docs.python.org/3.9/c-api/buffer.html#c.Py_buffer.obj
+    assert 2 * 4 == buf.nbytes  # 2 elements * sizeof(int32_t)
+    assert "02000000ffffffff" == buf.hex()  # native (little) endian
+  buf1 = pm.eval("new Int32Array([2,-1])")
+  buf2 = pm.eval("new Int32Array([2,-1]).buffer")
+  assert_js_to_py_memoryview(buf1)
+  assert_js_to_py_memoryview(buf2)
+  assert [2, -1] == buf1.tolist()
+  assert [2, 0, 0, 0, 255, 255, 255, 255] == buf2.tolist()
+  assert -1 == buf1[1]
+  assert 255 == buf2[7]
+  with pytest.raises(IndexError, match="index out of bounds on dimension 1"):
+    buf1[2]
+  with pytest.raises(IndexError, match="index out of bounds on dimension 1"):
+    buf2[8]
+  del buf1, buf2
+
+  # test element value ranges
+  buf3 = pm.eval("new Uint8Array(1)")
+  with pytest.raises(ValueError, match="memoryview: invalid value for format 'B'"):
+    buf3[0] = 256
+  with pytest.raises(ValueError, match="memoryview: invalid value for format 'B'"):
+    buf3[0] = -1
+  with pytest.raises(IndexError, match="index out of bounds on dimension 1"):  # no automatic resize
+    buf3[1] = 0
+  del buf3
+
+  # Python buffers should coerce to JS TypedArray
+  # and the typecode maps to TypedArray subtype (Uint8Array, Float64Array, ...)
+  assert pm.eval("(arr)=>arr instanceof Uint8Array")(bytearray([1, 2, 3]))
+  assert pm.eval("(arr)=>arr instanceof Uint8Array")(numpy.array([1], dtype=numpy.uint8))
+  assert pm.eval("(arr)=>arr instanceof Uint16Array")(numpy.array([1], dtype=numpy.uint16))
+  assert pm.eval("(arr)=>arr instanceof Uint32Array")(numpy.array([1], dtype=numpy.uint32))
+  assert pm.eval("(arr)=>arr instanceof BigUint64Array")(numpy.array([1], dtype=numpy.uint64))
+  assert pm.eval("(arr)=>arr instanceof Int8Array")(numpy.array([1], dtype=numpy.int8))
+  assert pm.eval("(arr)=>arr instanceof Int16Array")(numpy.array([1], dtype=numpy.int16))
+  assert pm.eval("(arr)=>arr instanceof Int32Array")(numpy.array([1], dtype=numpy.int32))
+  assert pm.eval("(arr)=>arr instanceof BigInt64Array")(numpy.array([1], dtype=numpy.int64))
+  assert pm.eval("(arr)=>arr instanceof Float32Array")(numpy.array([1], dtype=numpy.float32))
+  assert pm.eval("(arr)=>arr instanceof Float64Array")(numpy.array([1], dtype=numpy.float64))
+  assert pm.eval("new Uint8Array([1])").format == "B"
+  assert pm.eval("new Uint16Array([1])").format == "H"
+  assert pm.eval("new Uint32Array([1])").format == "I"  # FIXME (Tom Tang): this is "L" on 32-bit systems
+  assert pm.eval("new BigUint64Array([1n])").format == "Q"
+  assert pm.eval("new Int8Array([1])").format == "b"
+  assert pm.eval("new Int16Array([1])").format == "h"
+  assert pm.eval("new Int32Array([1])").format == "i"
+  assert pm.eval("new BigInt64Array([1n])").format == "q"
+  assert pm.eval("new Float32Array([1])").format == "f"
+  assert pm.eval("new Float64Array([1])").format == "d"
+
+  # not enough bytes to populate an element of the TypedArray
+  with pytest.raises(pm.SpiderMonkeyError,
+                     match="RangeError: buffer length for BigInt64Array should be a multiple of 8"):
+    pm.eval("(arr) => new BigInt64Array(arr.buffer)")(array.array('i', [-11111111]))
+
+  # TypedArray with `byteOffset` and `length`
+  arr1 = array.array('i', [-11111111, 22222222, -33333333, 44444444])
+  with pytest.raises(pm.SpiderMonkeyError, match="RangeError: invalid or out-of-range index"):
+    pm.eval("(arr) => new Int32Array(arr.buffer, /*byteOffset*/ -4)")(arr1)
+  with pytest.raises(pm.SpiderMonkeyError, match="RangeError: start offset of Int32Array should be a multiple of 4"):
+    pm.eval("(arr) => new Int32Array(arr.buffer, /*byteOffset*/ 1)")(arr1)
+  with pytest.raises(pm.SpiderMonkeyError,
+                     match="RangeError: size of buffer is too small for Int32Array with byteOffset"):
+    pm.eval("(arr) => new Int32Array(arr.buffer, /*byteOffset*/ 20)")(arr1)
+  with pytest.raises(pm.SpiderMonkeyError, match="RangeError: invalid or out-of-range index"):
+    pm.eval("(arr) => new Int32Array(arr.buffer, /*byteOffset*/ 4, /*length*/ -1)")(arr1)
+  with pytest.raises(pm.SpiderMonkeyError,
+                     match="RangeError: attempting to construct out-of-bounds Int32Array on ArrayBuffer"):
+    pm.eval("(arr) => new Int32Array(arr.buffer, /*byteOffset*/ 4, /*length*/ 4)")(arr1)
+  arr2 = pm.eval("(arr) => new Int32Array(arr.buffer, /*byteOffset*/ 4, /*length*/ 2)")(arr1)
+  assert 2 * 4 == arr2.nbytes  # 2 elements * sizeof(int32_t)
+  assert [22222222, -33333333] == arr2.tolist()
+  assert "8e155301ab5f03fe" == arr2.hex()  # native (little) endian
+  assert 22222222 == arr2[0]  # offset 1 int32
+  with pytest.raises(IndexError, match="index out of bounds on dimension 1"):
+    arr2[2]
+  arr3 = pm.eval("(arr) => new Int32Array(arr.buffer, 16 /* byteOffset */)")(arr1)  # empty Int32Array
+  assert 0 == arr3.nbytes
+  del arr3
+
+  # test GC
+  del arr1
+  gc.collect(), pm.collect()
+  gc.collect(), pm.collect()
+  # TODO (Tom Tang): the 0th element in the underlying buffer is still
+  # accessible after GC, even is not referenced by the JS TypedArray with
+  # byteOffset
+  del arr2
+
+  # mutation
+  mut_arr_original = bytearray(4)
+  pm.eval("""
     (/* @type Uint8Array */ arr) => {
         // 2.25 in float32 little endian
         arr[2] = 0x10
         arr[3] = 0x40
     }
     """)(mut_arr_original)
-    assert 0x10 == mut_arr_original[2]
-    assert 0x40 == mut_arr_original[3]
-    # mutation to a different TypedArray accessing the same underlying data block will also change the original buffer
-    def do_mutation(mut_arr_js):
-        assert 2.25 == mut_arr_js[0]
-        mut_arr_js[0] = 225.50048828125 # float32 little endian: 0x 20 80 61 43 
-        assert "20806143" == mut_arr_original.hex()
-        assert 225.50048828125 == array.array("f", mut_arr_original)[0]
-    mut_arr_new = pm.eval("""
+  assert 0x10 == mut_arr_original[2]
+  assert 0x40 == mut_arr_original[3]
+  # mutation to a different TypedArray accessing the same underlying data block will also change the original buffer
+
+  def do_mutation(mut_arr_js):
+    assert 2.25 == mut_arr_js[0]
+    mut_arr_js[0] = 225.50048828125  # float32 little endian: 0x 20 80 61 43
+    assert "20806143" == mut_arr_original.hex()
+    assert 225.50048828125 == array.array("f", mut_arr_original)[0]
+  mut_arr_new = pm.eval("""
     (/* @type Uint8Array */ arr, do_mutation) => {
         const mut_arr_js = new Float32Array(arr.buffer)
         do_mutation(mut_arr_js)
         return arr
     }
     """)(mut_arr_original, do_mutation)
-    assert [0x20, 0x80, 0x61, 0x43] == mut_arr_new.tolist()
+  assert [0x20, 0x80, 0x61, 0x43] == mut_arr_new.tolist()
 
-    # simple 1-D numpy array should just work as well
-    numpy_int16_array = numpy.array([0, 1, 2, 3], dtype=numpy.int16)
-    assert "0,1,2,3" == pm.eval("(typedArray) => typedArray.toString()")(numpy_int16_array)
-    assert 3.0 == pm.eval("(typedArray) => typedArray[3]")(numpy_int16_array)
-    assert True == pm.eval("(typedArray) => typedArray instanceof Int16Array")(numpy_int16_array)
-    numpy_memoryview = pm.eval("(typedArray) => typedArray")(numpy_int16_array)
-    assert 2 == numpy_memoryview[2]
-    assert 4 * 2 == numpy_memoryview.nbytes # 4 elements * sizeof(int16_t)
-    assert "h" == numpy_memoryview.format # the type code for int16 is 'h', see https://docs.python.org/3.9/library/array.html
-    with pytest.raises(IndexError, match="index out of bounds on dimension 1"):
-        numpy_memoryview[4]
-
-    # can work for empty Python buffer
-    def assert_empty_py_buffer(buf, type: str):
-        assert 0 == pm.eval("(typedArray) => typedArray.length")(buf)
-        assert None == pm.eval("(typedArray) => typedArray[0]")(buf) # `undefined`
-        assert True == pm.eval("(typedArray) => typedArray instanceof "+type)(buf)
-    assert_empty_py_buffer(bytearray(b''), "Uint8Array")
-    assert_empty_py_buffer(numpy.array([], dtype=numpy.uint64), "BigUint64Array")
-    assert_empty_py_buffer(array.array('d', []), "Float64Array")
-
-    # can work for empty TypedArray
-    def assert_empty_typedarray(buf: memoryview, typecode: str):
-        assert typecode == buf.format
-        assert struct.calcsize(typecode) == buf.itemsize
-        assert 0 == buf.nbytes
-        assert "" == buf.hex()
-        assert b"" == buf.tobytes()
-        assert [] == buf.tolist()
-        buf.release()
-    assert_empty_typedarray(pm.eval("new BigInt64Array()"), "q")
-    assert_empty_typedarray(pm.eval("new Float32Array(new ArrayBuffer(4), 4 /*byteOffset*/)"), "f")
-    assert_empty_typedarray(pm.eval("(arr)=>arr")( bytearray([]) ), "B")
-    assert_empty_typedarray(pm.eval("(arr)=>arr")( numpy.array([], dtype=numpy.uint16) ),"H")
-    assert_empty_typedarray(pm.eval("(arr)=>arr")( array.array("d", []) ),"d")
-
-    # can work for empty ArrayBuffer
-    def assert_empty_arraybuffer(buf):
-        assert "B" == buf.format
-        assert 1 == buf.itemsize
-        assert 0 == buf.nbytes
-        assert "" == buf.hex()
-        assert b"" == buf.tobytes()
-        assert [] == buf.tolist()
-        buf.release()
-    assert_empty_arraybuffer(pm.eval("new ArrayBuffer()"))
-    assert_empty_arraybuffer(pm.eval("new Uint8Array().buffer"))
-    assert_empty_arraybuffer(pm.eval("new Float64Array().buffer"))
-    assert_empty_arraybuffer(pm.eval("(arr)=>arr.buffer")( bytearray([]) ))
-    assert_empty_arraybuffer(pm.eval("(arr)=>arr.buffer")( pm.eval("(arr)=>arr.buffer")(bytearray()) ))
-    assert_empty_arraybuffer(pm.eval("(arr)=>arr.buffer")( numpy.array([], dtype=numpy.uint64) ))
-    assert_empty_arraybuffer(pm.eval("(arr)=>arr.buffer")( array.array("d", []) ))
-
-    # TODO (Tom Tang): shared ArrayBuffer should be disallowed
-    # pm.eval("new WebAssembly.Memory({ initial: 1, maximum: 1, shared: true }).buffer")
-
-    # TODO (Tom Tang): once a JS ArrayBuffer is transferred to a worker thread, it should be invalidated in Python-land as well
-
-    # TODO (Tom Tang): error for detached ArrayBuffer, or should it be considered as empty?
-
-    # should error on immutable Python buffers 
-    # Note: Python `bytes` type must be converted to a (mutable) `bytearray` because there's no such a concept of read-only ArrayBuffer in JS
-    with pytest.raises(BufferError, match="Object is not writable."):
-        pm.eval("(typedArray) => {}")(b'')
-    immutable_numpy_array = numpy.arange(10)
-    immutable_numpy_array.setflags(write=False)
-    with pytest.raises(ValueError, match="buffer source array is read-only"):
-        pm.eval("(typedArray) => {}")(immutable_numpy_array)
-
-    # buffer should be in C order (row major)
-    fortran_order_arr = numpy.array([[1, 2], [3, 4]], order="F") # 1-D array is always considered C-contiguous because it doesn't matter if it's row or column major in 1-D
-    with pytest.raises(ValueError, match="ndarray is not C-contiguous"):
-        pm.eval("(typedArray) => {}")(fortran_order_arr)
-
-    # disallow multidimensional array
-    numpy_2d_array = numpy.array([[1, 2], [3, 4]], order="C")
-    with pytest.raises(BufferError, match="multidimensional arrays are not allowed"):
-        pm.eval("(typedArray) => {}")(numpy_2d_array)
+  # simple 1-D numpy array should just work as well
+  numpy_int16_array = numpy.array([0, 1, 2, 3], dtype=numpy.int16)
+  assert "0,1,2,3" == pm.eval("(typedArray) => typedArray.toString()")(numpy_int16_array)
+  assert 3.0 == pm.eval("(typedArray) => typedArray[3]")(numpy_int16_array)
+  assert pm.eval("(typedArray) => typedArray instanceof Int16Array")(numpy_int16_array)
+  numpy_memoryview = pm.eval("(typedArray) => typedArray")(numpy_int16_array)
+  assert 2 == numpy_memoryview[2]
+  assert 4 * 2 == numpy_memoryview.nbytes  # 4 elements * sizeof(int16_t)
+  # the type code for int16 is 'h', see https://docs.python.org/3.9/library/array.html
+  assert "h" == numpy_memoryview.format
+  with pytest.raises(IndexError, match="index out of bounds on dimension 1"):
+    numpy_memoryview[4]
+
+  # can work for empty Python buffer
+  def assert_empty_py_buffer(buf, type: str):
+    assert 0 == pm.eval("(typedArray) => typedArray.length")(buf)
+    assert None is pm.eval("(typedArray) => typedArray[0]")(buf)  # `undefined`
+    assert pm.eval("(typedArray) => typedArray instanceof " + type)(buf)
+  assert_empty_py_buffer(bytearray(b''), "Uint8Array")
+  assert_empty_py_buffer(numpy.array([], dtype=numpy.uint64), "BigUint64Array")
+  assert_empty_py_buffer(array.array('d', []), "Float64Array")
+
+  # can work for empty TypedArray
+  def assert_empty_typedarray(buf: memoryview, typecode: str):
+    assert typecode == buf.format
+    assert struct.calcsize(typecode) == buf.itemsize
+    assert 0 == buf.nbytes
+    assert "" == buf.hex()
+    assert b"" == buf.tobytes()
+    assert [] == buf.tolist()
+    buf.release()
+  assert_empty_typedarray(pm.eval("new BigInt64Array()"), "q")
+  assert_empty_typedarray(pm.eval("new Float32Array(new ArrayBuffer(4), 4 /*byteOffset*/)"), "f")
+  assert_empty_typedarray(pm.eval("(arr)=>arr")(bytearray([])), "B")
+  assert_empty_typedarray(pm.eval("(arr)=>arr")(numpy.array([], dtype=numpy.uint16)), "H")
+  assert_empty_typedarray(pm.eval("(arr)=>arr")(array.array("d", [])), "d")
+
+  # can work for empty ArrayBuffer
+  def assert_empty_arraybuffer(buf):
+    assert "B" == buf.format
+    assert 1 == buf.itemsize
+    assert 0 == buf.nbytes
+    assert "" == buf.hex()
+    assert b"" == buf.tobytes()
+    assert [] == buf.tolist()
+    buf.release()
+  assert_empty_arraybuffer(pm.eval("new ArrayBuffer()"))
+  assert_empty_arraybuffer(pm.eval("new Uint8Array().buffer"))
+  assert_empty_arraybuffer(pm.eval("new Float64Array().buffer"))
+  assert_empty_arraybuffer(pm.eval("(arr)=>arr.buffer")(bytearray([])))
+  assert_empty_arraybuffer(pm.eval("(arr)=>arr.buffer")(pm.eval("(arr)=>arr.buffer")(bytearray())))
+  assert_empty_arraybuffer(pm.eval("(arr)=>arr.buffer")(numpy.array([], dtype=numpy.uint64)))
+  assert_empty_arraybuffer(pm.eval("(arr)=>arr.buffer")(array.array("d", [])))
+
+  # TODO (Tom Tang): shared ArrayBuffer should be disallowed
+  # pm.eval("new WebAssembly.Memory({ initial: 1, maximum: 1, shared: true }).buffer")
+
+  # TODO (Tom Tang): once a JS ArrayBuffer is transferred to a worker
+  # thread, it should be invalidated in Python-land as well
+
+  # TODO (Tom Tang): error for detached ArrayBuffer, or should it be considered as empty?
+
+  # should error on immutable Python buffers
+  # Note: Python `bytes` type must be converted to a (mutable) `bytearray`
+  # because there's no such a concept of read-only ArrayBuffer in JS
+  with pytest.raises(BufferError, match="Object is not writable."):
+    pm.eval("(typedArray) => {}")(b'')
+  immutable_numpy_array = numpy.arange(10)
+  immutable_numpy_array.setflags(write=False)
+  with pytest.raises(ValueError, match="buffer source array is read-only"):
+    pm.eval("(typedArray) => {}")(immutable_numpy_array)
+
+  # buffer should be in C order (row major)
+  # 1-D array is always considered C-contiguous because it doesn't matter if it's row or column major in 1-D
+  fortran_order_arr = numpy.array([[1, 2], [3, 4]], order="F")
+  with pytest.raises(ValueError, match="ndarray is not C-contiguous"):
+    pm.eval("(typedArray) => {}")(fortran_order_arr)
+
+  # disallow multidimensional array
+  numpy_2d_array = numpy.array([[1, 2], [3, 4]], order="C")
+  with pytest.raises(BufferError, match="multidimensional arrays are not allowed"):
+    pm.eval("(typedArray) => {}")(numpy_2d_array)
```

### Comparing `pythonmonkey-0.4.0/tests/python/test_dict_methods.py` & `pythonmonkey-0.6.0/tests/python/test_dict_methods.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,462 +1,557 @@
 import pythonmonkey as pm
 
 # get
+
+
 def test_get_no_default():
-    likes = pm.eval('({"color": "blue", "fruit": "apple", "pet": "dog"})')
-    foundKey = likes.get('fruit')
-    assert foundKey == 'apple'
+  likes = pm.eval('({"color": "blue", "fruit": "apple", "pet": "dog"})')
+  foundKey = likes.get('fruit')
+  assert foundKey == 'apple'
+
 
 def test_get_no_default_not_found():
-    likes = pm.eval('({"color": "blue", "fruit": "apple", "pet": "dog"})')
-    foundKey = likes.get('fuit')
-    assert foundKey == None
+  likes = pm.eval('({"color": "blue", "fruit": "apple", "pet": "dog"})')
+  foundKey = likes.get('fuit')
+  assert foundKey is None
+
 
 def test_get_default_not_found():
-    likes = pm.eval('({"color": "blue", "fruit": "apple", "pet": "dog"})')
-    foundKey = likes.get('fuit', 'orange')
-    assert foundKey == 'orange'
+  likes = pm.eval('({"color": "blue", "fruit": "apple", "pet": "dog"})')
+  foundKey = likes.get('fuit', 'orange')
+  assert foundKey == 'orange'
+
 
 def test_get_no_params():
-    likes = pm.eval('({"color": "blue", "fruit": "apple", "pet": "dog"})')
-    try:
-        likes.get()           
-        assert (False)
-    except Exception as e:   
-        assert str(type(e)) == "<class 'TypeError'>"
-        assert str(e) == "get expected at least 1 argument, got 0"
+  likes = pm.eval('({"color": "blue", "fruit": "apple", "pet": "dog"})')
+  try:
+    likes.get()
+    assert (False)
+  except Exception as e:
+    assert str(type(e)) == "<class 'TypeError'>"
+    assert str(e) == "get expected at least 1 argument, got 0"
 
 # setdefault
+
+
 def test_setdefault_found():
-    likes = pm.eval('({"color": "blue", "fruit": "apple", "pet": "dog"})')
-    foundKey = likes.setdefault('color')
-    assert foundKey == 'blue'
+  likes = pm.eval('({"color": "blue", "fruit": "apple", "pet": "dog"})')
+  foundKey = likes.setdefault('color')
+  assert foundKey == 'blue'
+
 
 def test_setdefault_found_ignore_default():
-    likes = pm.eval('({"color": "blue", "fruit": "apple", "pet": "dog"})')
-    foundKey = likes.setdefault('color', 'yello')
-    assert foundKey == 'blue'
+  likes = pm.eval('({"color": "blue", "fruit": "apple", "pet": "dog"})')
+  foundKey = likes.setdefault('color', 'yello')
+  assert foundKey == 'blue'
+
 
 def test_setdefault_not_found_no_default():
-    likes = pm.eval('({"color": "blue", "fruit": "apple", "pet": "dog"})')
-    foundKey = likes.setdefault('colo')
-    assert likes['colo'] == None
-    assert foundKey == None    
+  likes = pm.eval('({"color": "blue", "fruit": "apple", "pet": "dog"})')
+  foundKey = likes.setdefault('colo')
+  assert likes['colo'] is None
+  assert foundKey is None
+
 
 def test_setdefault_not_found_with_default():
-    likes = pm.eval('({"color": "blue", "fruit": "apple", "pet": "dog"})')
-    foundKey = likes.setdefault('colo', 'yello')
-    assert likes['colo'] == 'yello'
-    assert foundKey == 'yello'  
+  likes = pm.eval('({"color": "blue", "fruit": "apple", "pet": "dog"})')
+  foundKey = likes.setdefault('colo', 'yello')
+  assert likes['colo'] == 'yello'
+  assert foundKey == 'yello'
+
 
 def test_setdefault_no_params():
-    likes = pm.eval('({"color": "blue", "fruit": "apple", "pet": "dog"})')
-    try:
-        likes.setdefault()           
-        assert (False)
-    except Exception as e:    
-        assert str(type(e)) == "<class 'TypeError'>"
-        assert str(e) == "setdefault expected at least 1 argument, got 0"    
+  likes = pm.eval('({"color": "blue", "fruit": "apple", "pet": "dog"})')
+  try:
+    likes.setdefault()
+    assert (False)
+  except Exception as e:
+    assert str(type(e)) == "<class 'TypeError'>"
+    assert str(e) == "setdefault expected at least 1 argument, got 0"
+
 
 def test_setdefault_with_shadowing():
-    jsObj = pm.eval("({get: 'value'})")
-    a = jsObj.setdefault("get", "val")
-    assert a == 'value'
+  jsObj = pm.eval("({get: 'value'})")
+  a = jsObj.setdefault("get", "val")
+  assert a == 'value'
+
+# pop
+
 
-#pop
 def test_pop_found():
-    likes = pm.eval('({"color": "blue", "fruit": "apple", "pet": "dog"})')
-    foundKey = likes.pop('color')
-    assert likes['color'] == None
-    assert foundKey == 'blue'
+  likes = pm.eval('({"color": "blue", "fruit": "apple", "pet": "dog"})')
+  foundKey = likes.pop('color')
+  assert likes['color'] is None
+  assert foundKey == 'blue'
+
 
 def test_pop_not_found():
-    likes = pm.eval('({"color": "blue", "fruit": "apple", "pet": "dog"})')
-    try:
-        likes.pop('colo')          
-        assert (False)
-    except Exception as e:    
-        assert str(type(e)) == "<class 'KeyError'>"
-        assert str(e) == "'colo'"   
+  likes = pm.eval('({"color": "blue", "fruit": "apple", "pet": "dog"})')
+  try:
+    likes.pop('colo')
+    assert (False)
+  except Exception as e:
+    assert str(type(e)) == "<class 'KeyError'>"
+    assert str(e) == "'colo'"
+
 
 def test_pop_twice_not_found():
-    likes = pm.eval('({"color": "blue", "fruit": "apple", "pet": "dog"})')
+  likes = pm.eval('({"color": "blue", "fruit": "apple", "pet": "dog"})')
+  likes.pop('color')
+  try:
     likes.pop('color')
-    try:
-        likes.pop('color')          
-        assert (False)
-    except Exception as e:    
-        assert str(type(e)) == "<class 'KeyError'>"
-        assert str(e) == "'color'"         
+    assert (False)
+  except Exception as e:
+    assert str(type(e)) == "<class 'KeyError'>"
+    assert str(e) == "'color'"
+
 
 def test_pop_found_ignore_default():
-    likes = pm.eval('({"color": "blue", "fruit": "apple", "pet": "dog"})')
-    foundKey = likes.pop('color', 'u')
-    assert foundKey == 'blue'
+  likes = pm.eval('({"color": "blue", "fruit": "apple", "pet": "dog"})')
+  foundKey = likes.pop('color', 'u')
+  assert foundKey == 'blue'
+
 
 def test_pop_not_found_with_default():
-    likes = pm.eval('({"color": "blue", "fruit": "apple", "pet": "dog"})')
-    foundKey = likes.pop('colo', 'unameit')
-    assert foundKey == 'unameit'
+  likes = pm.eval('({"color": "blue", "fruit": "apple", "pet": "dog"})')
+  foundKey = likes.pop('colo', 'unameit')
+  assert foundKey == 'unameit'
+
 
 def test_pop_not_found_no_default():
-    likes = pm.eval('({"color": "blue", "fruit": "apple", "pet": "dog"})')
-    try:
-        likes.pop('colo')           
-        assert (False)
-    except Exception as e:    
-        assert str(type(e)) == "<class 'KeyError'>"
-        assert str(e) == "'colo'"        
+  likes = pm.eval('({"color": "blue", "fruit": "apple", "pet": "dog"})')
+  try:
+    likes.pop('colo')
+    assert (False)
+  except Exception as e:
+    assert str(type(e)) == "<class 'KeyError'>"
+    assert str(e) == "'colo'"
+
 
 def test_pop_no_params():
-    likes = pm.eval('({"color": "blue", "fruit": "apple", "pet": "dog"})')
-    try:
-        likes.pop()           
-        assert (False)
-    except Exception as e:    
-        assert str(type(e)) == "<class 'TypeError'>"
-        assert str(e) == "pop expected at least 1 argument, got 0"      
+  likes = pm.eval('({"color": "blue", "fruit": "apple", "pet": "dog"})')
+  try:
+    likes.pop()
+    assert (False)
+  except Exception as e:
+    assert str(type(e)) == "<class 'TypeError'>"
+    assert str(e) == "pop expected at least 1 argument, got 0"
+
+# clear
+
 
-#clear
 def test_clear():
-    likes = pm.eval('({"color": "blue", "fruit": "apple", "pet": "dog"})')
-    likes.clear()
-    assert len(likes) == 0
+  likes = pm.eval('({"color": "blue", "fruit": "apple", "pet": "dog"})')
+  likes.clear()
+  assert len(likes) == 0
+
+# copy
+
 
-#copy
 def test_copy():
-    likes = pm.eval('({"color": "blue", "fruit": "apple", "pet": "dog"})')
-    otherLikes = likes.copy()
-    otherLikes["color"] = "yellow"
+  likes = pm.eval('({"color": "blue", "fruit": "apple", "pet": "dog"})')
+  otherLikes = likes.copy()
+  otherLikes["color"] = "yellow"
+
+  assert likes == {"color": "blue", "fruit": "apple", "pet": "dog"}
+  assert otherLikes == {"color": "yellow", "fruit": "apple", "pet": "dog"}
+
+# update
 
-    assert likes == {"color": "blue", "fruit": "apple", "pet": "dog"}
-    assert otherLikes == {"color": "yellow", "fruit": "apple", "pet": "dog"}
 
-#update
 def test_update_true_dict_right():
-    a = pm.eval("({'c':5})")
-    b = {'d':6.0}
-    a.update(b)
-    assert a == {'c': 5.0, 'd': 6.0}   
-    assert b == {'d': 6.0}  
+  a = pm.eval("({'c':5})")
+  b = {'d': 6.0}
+  a.update(b)
+  assert a == {'c': 5.0, 'd': 6.0}
+  assert b == {'d': 6.0}
+
 
 def test_update_true_dict_left():
-    a = {'d':6.0}
-    b = pm.eval("({'c':5})") 
-    a.update(b)
-    assert a == {'c': 5.0, 'd': 6.0}   
-    assert b == {'c': 5.0}      
+  a = {'d': 6.0}
+  b = pm.eval("({'c':5})")
+  a.update(b)
+  assert a == {'c': 5.0, 'd': 6.0}
+  assert b == {'c': 5.0}
+
 
 def test_update_true_two_pm_dicts():
-    a = pm.eval("({'c':5})")
-    b = pm.eval("({'d':6})")
-    a.update(b)
-    assert a == {'c': 5.0, 'd': 6.0}   
-    assert b == {'d': 6.0}  
+  a = pm.eval("({'c':5})")
+  b = pm.eval("({'d':6})")
+  a.update(b)
+  assert a == {'c': 5.0, 'd': 6.0}
+  assert b == {'d': 6.0}
+
 
 def test_update_two_args():
-    a = pm.eval("({'c':5})")
-    a.update(B='For', C='Geeks')
-    assert a == {'c': 5.0, 'B': 'For', 'C': 'Geeks'}       
+  a = pm.eval("({'c':5})")
+  a.update(B='For', C='Geeks')
+  assert a == {'c': 5.0, 'B': 'For', 'C': 'Geeks'}
+
 
 def test_update_iterable():
-    car = pm.eval('({"brand": "Ford","model": "Mustang","year": 1964})')
-    car.update([('y', 3), ('z', 0)])
-    assert car == {'brand': 'Ford', 'model': 'Mustang', 'year': 1964, 'y': 3, 'z': 0}       
- 
+  car = pm.eval('({"brand": "Ford","model": "Mustang","year": 1964})')
+  car.update([('y', 3), ('z', 0)])
+  assert car == {'brand': 'Ford', 'model': 'Mustang', 'year': 1964, 'y': 3, 'z': 0}
+
+
 def test_update_iterable_wrong_type():
-    car = pm.eval('({"brand": "Ford","model": "Mustang","year": 1964})')
-    a = [1,2]
-    try:
-        car.update(a)          
-        assert (False)
-    except Exception as e:    
-        assert str(type(e)) == "<class 'TypeError'>"
-        assert str(e) == "cannot convert dictionary update sequence element #0 to a sequence"       
+  car = pm.eval('({"brand": "Ford","model": "Mustang","year": 1964})')
+  a = [1, 2]
+  try:
+    car.update(a)
+    assert (False)
+  except Exception as e:
+    assert str(type(e)) == "<class 'TypeError'>"
+    assert str(e) == "cannot convert dictionary update sequence element #0 to a sequence"
+
+# keys
+
 
-#keys
 def test_keys_iter():
-    obj = pm.eval("({ a: 123, b: 'test' })")
-    result = []
-    for i in obj.keys():
-        result.append(i)
-    assert result == ['a', 'b']
+  obj = pm.eval("({ a: 123, b: 'test' })")
+  result = []
+  for i in obj.keys():
+    result.append(i)
+  assert result == ['a', 'b']
+
 
 def test_keys_iter_reverse():
-    obj = pm.eval("({ a: 123, b: 'test' })")
-    result = []
-    for i in reversed(obj.keys()):
-        result.append(i)
-    assert result == ['b', 'a']    
+  obj = pm.eval("({ a: 123, b: 'test' })")
+  result = []
+  for i in reversed(obj.keys()):
+    result.append(i)
+  assert result == ['b', 'a']
+
 
 def test_keys_list():
-    obj = pm.eval("({ a: 123, b: 'test' })")
-    assert list(obj.keys()) == ['a', 'b']      
+  obj = pm.eval("({ a: 123, b: 'test' })")
+  assert list(obj.keys()) == ['a', 'b']
+
 
 def test_keys_repr():
-    car = pm.eval('({"brand": "Ford","model": "Mustang","year": 1964})')
-    a = car.keys()
-    assert str(a) == "dict_keys(['brand', 'model', 'year'])"
+  car = pm.eval('({"brand": "Ford","model": "Mustang","year": 1964})')
+  a = car.keys()
+  assert str(a) == "dict_keys(['brand', 'model', 'year'])"
+
 
 def test_keys_substract():
-    car = pm.eval('({"brand": "Ford","model": "Mustang","year": 1964})')
-    a = car.keys()
-    b = a - ['brand']
-    assert b == {'model', 'year'}  
+  car = pm.eval('({"brand": "Ford","model": "Mustang","year": 1964})')
+  a = car.keys()
+  b = a - ['brand']
+  assert b == {'model', 'year'}
+
 
 def test_keys_richcompare_two_own():
-    car = pm.eval('({"brand": "Ford","model": "Mustang","year": 1964})')
-    a = car.keys()
-    b = car.keys()    
-    assert a == b
-    assert a is not b  
-    assert a <= b
-    assert not(a < b)
-    assert a >= b
-    assert not(a > b)
+  car = pm.eval('({"brand": "Ford","model": "Mustang","year": 1964})')
+  a = car.keys()
+  b = car.keys()
+  assert a == b
+  assert a is not b
+  assert a <= b
+  assert not (a < b)
+  assert a >= b
+  assert not (a > b)
+
 
 def test_keys_richcompare_one_own():
-    car = pm.eval('({"brand": "Ford","model": "Mustang","year": 1964})')
-    a = car.keys()
-    care = {"brand": "Ford","model": "Mustang","year": 1964}
-    b = care.keys()    
-    assert a == b
-    assert b == a
-    assert a <= b
-    assert not(a < b)
-    assert a >= b
-    assert not(a > b)
-    assert b <= a
-    assert not(b > a)
-    assert b >= a
-    assert not(b > a)
+  car = pm.eval('({"brand": "Ford","model": "Mustang","year": 1964})')
+  a = car.keys()
+  care = {"brand": "Ford", "model": "Mustang", "year": 1964}
+  b = care.keys()
+  assert a == b
+  assert b == a
+  assert a <= b
+  assert not (a < b)
+  assert a >= b
+  assert not (a > b)
+  assert b <= a
+  assert not (b > a)
+  assert b >= a
+  assert not (b > a)
+
 
 def test_keys_intersect_one_own_smaller():
-    dishes = pm.eval("({'eggs': 2, 'sausage': 1, 'bacon': 1, 'spam': 500})")
-    keys = dishes.keys()
-    b = keys & {'eggs', 'bacon', 'salad', 'jam'}
-    c = {'eggs', 'bacon', 'salad', 'jam'} & keys
-    assert b == {'bacon', 'eggs'} == c
+  dishes = pm.eval("({'eggs': 2, 'sausage': 1, 'bacon': 1, 'spam': 500})")
+  keys = dishes.keys()
+  b = keys & {'eggs', 'bacon', 'salad', 'jam'}
+  c = {'eggs', 'bacon', 'salad', 'jam'} & keys
+  assert b == {'bacon', 'eggs'} == c
+
 
 def test_keys_intersect_two_own_smaller():
-    dishes = pm.eval("({'eggs': 2, 'sausage': 1, 'bacon': 1, 'spam': 500})")
-    keys = dishes.keys()
-    dishes1 = pm.eval("({'eggs': 2, 'sausage': 1, 'bacon': 1})")
-    keys1 = dishes1.keys()
-    b = keys & keys1
-    c = keys1 & keys
-    assert b == {'bacon', 'eggs', 'sausage'} == c 
+  dishes = pm.eval("({'eggs': 2, 'sausage': 1, 'bacon': 1, 'spam': 500})")
+  keys = dishes.keys()
+  dishes1 = pm.eval("({'eggs': 2, 'sausage': 1, 'bacon': 1})")
+  keys1 = dishes1.keys()
+  b = keys & keys1
+  c = keys1 & keys
+  assert b == {'bacon', 'eggs', 'sausage'} == c
+
 
 def test_keys_intersect_one_own():
-    dishes = pm.eval("({'eggs': 2, 'sausage': 1, 'bacon': 1, 'spam': 500})")
-    keys = dishes.keys()
-    dishes1 = {'eggs': 2, 'sausage': 1, 'bacon': 1, 'peas':6}
-    keys1 = dishes1.keys()
-    b = keys & keys1
-    c = keys1 & keys
-    assert b == {'bacon', 'eggs', 'sausage'} == c     
+  dishes = pm.eval("({'eggs': 2, 'sausage': 1, 'bacon': 1, 'spam': 500})")
+  keys = dishes.keys()
+  dishes1 = {'eggs': 2, 'sausage': 1, 'bacon': 1, 'peas': 6}
+  keys1 = dishes1.keys()
+  b = keys & keys1
+  c = keys1 & keys
+  assert b == {'bacon', 'eggs', 'sausage'} == c
+
 
 def test_keys_or():
-    dishes =pm.eval("({'eggs': 2, 'sausage': 1, 'bacon': 1, 'spam': 500})")
-    keys = dishes.keys()
-    others = keys | ['juice', 'juice', 'juice']
-    assert others == {'bacon', 'spam', 'juice', 'sausage', 'eggs'}
-    others = ['apple'] | keys
-    assert others == {'bacon', 'spam', 'sausage', 'apple', 'eggs'}
+  dishes = pm.eval("({'eggs': 2, 'sausage': 1, 'bacon': 1, 'spam': 500})")
+  keys = dishes.keys()
+  others = keys | ['juice', 'juice', 'juice']
+  assert others == {'bacon', 'spam', 'juice', 'sausage', 'eggs'}
+  others = ['apple'] | keys
+  assert others == {'bacon', 'spam', 'sausage', 'apple', 'eggs'}
+
 
 def test_keys_xor():
-    dishes = pm.eval("({'eggs': 2, 'sausage': 1, 'bacon': 1, 'spam': 500})")
-    keys = dishes.keys()
-    others = keys ^ {'sausage', 'juice'}
-    assert others == {'bacon', 'spam', 'juice', 'eggs'}
+  dishes = pm.eval("({'eggs': 2, 'sausage': 1, 'bacon': 1, 'spam': 500})")
+  keys = dishes.keys()
+  others = keys ^ {'sausage', 'juice'}
+  assert others == {'bacon', 'spam', 'juice', 'eggs'}
+
 
 def test_keys_len():
-    dishes = pm.eval("({'eggs': 2, 'sausage': 1, 'bacon': 1, 'spam': 500})")
-    keys = dishes.keys()
-    assert len(keys) == 4
+  dishes = pm.eval("({'eggs': 2, 'sausage': 1, 'bacon': 1, 'spam': 500})")
+  keys = dishes.keys()
+  assert len(keys) == 4
+
 
 def test_keys_contains():
-    dishes = pm.eval("({'eggs': 2, 'sausage': 1, 'bacon': 1, 'spam': 500})")
-    keys = dishes.keys()
-    assert 'eggs' in keys
-    assert 'egg' not in keys
+  dishes = pm.eval("({'eggs': 2, 'sausage': 1, 'bacon': 1, 'spam': 500})")
+  keys = dishes.keys()
+  assert 'eggs' in keys
+  assert 'egg' not in keys
+
 
 def test_keys_isdisjoint_self():
-    dishes = pm.eval("({'eggs': 2, 'sausage': 1, 'bacon': 1, 'spam': 500})")
-    keys = dishes.keys()
-    assert not keys.isdisjoint(keys)    
+  dishes = pm.eval("({'eggs': 2, 'sausage': 1, 'bacon': 1, 'spam': 500})")
+  keys = dishes.keys()
+  assert not keys.isdisjoint(keys)
+
 
 def test_keys_isdisjoint_true_keys():
-    dishes = pm.eval("({'eggs': 2, 'sausage': 1, 'bacon': 1, 'spam': 500})")
-    keys = dishes.keys()
-    assert keys.isdisjoint({ "egg": 4, "e": 5, "f": 6}.keys())     
+  dishes = pm.eval("({'eggs': 2, 'sausage': 1, 'bacon': 1, 'spam': 500})")
+  keys = dishes.keys()
+  assert keys.isdisjoint({"egg": 4, "e": 5, "f": 6}.keys())
+
 
 def test_keys_isnotdisjoint_true_keys():
-    dishes = pm.eval("({'eggs': 2, 'sausage': 1, 'bacon': 1, 'spam': 500})")
-    keys = dishes.keys()
-    assert not keys.isdisjoint({ "eggs": 4, "e": 5, "f": 6}.keys())      
+  dishes = pm.eval("({'eggs': 2, 'sausage': 1, 'bacon': 1, 'spam': 500})")
+  keys = dishes.keys()
+  assert not keys.isdisjoint({"eggs": 4, "e": 5, "f": 6}.keys())
+
 
 def test_keys_isnotdisjoint_own_keys():
-    dishes = pm.eval("({'eggs': 2, 'sausage': 1, 'bacon': 1, 'spam': 500})")
-    keys = dishes.keys()
-    dishese = pm.eval("({'eggs': 2, 'sausage': 1, 'bacon': 1, 'spam': 500})")
-    keys1 = dishese.keys()
-    assert not keys.isdisjoint(keys1)       
+  dishes = pm.eval("({'eggs': 2, 'sausage': 1, 'bacon': 1, 'spam': 500})")
+  keys = dishes.keys()
+  dishese = pm.eval("({'eggs': 2, 'sausage': 1, 'bacon': 1, 'spam': 500})")
+  keys1 = dishese.keys()
+  assert not keys.isdisjoint(keys1)
+
 
 def test_keys_isnotdisjoint_own_keys_longer():
-    dishes = pm.eval("({'eggs': 2, 'sausage': 1, 'bacon': 1, 'spam': 500})")
-    keys = dishes.keys()
-    dishese = pm.eval("({'eggs': 2, 'sausage': 1, 'bacon': 1, 'spam': 500, 'juice':6467})")
-    keys1 = dishese.keys()
-    assert not keys.isdisjoint(keys1)   
+  dishes = pm.eval("({'eggs': 2, 'sausage': 1, 'bacon': 1, 'spam': 500})")
+  keys = dishes.keys()
+  dishese = pm.eval("({'eggs': 2, 'sausage': 1, 'bacon': 1, 'spam': 500, 'juice':6467})")
+  keys1 = dishese.keys()
+  assert not keys.isdisjoint(keys1)
+
 
 def test_keys_isnotdisjoint_true_keys_longer():
-    dishes = pm.eval("({'eggs': 2, 'sausage': 1, 'bacon': 1, 'spam': 500})")
-    keys = dishes.keys()
-    dishese = {'eggs': 2, 'sausage': 1, 'bacon': 1, 'spam': 500, 'juice':6467}
-    keys1 = dishese.keys()
-    assert not keys.isdisjoint(keys1)        
+  dishes = pm.eval("({'eggs': 2, 'sausage': 1, 'bacon': 1, 'spam': 500})")
+  keys = dishes.keys()
+  dishese = {'eggs': 2, 'sausage': 1, 'bacon': 1, 'spam': 500, 'juice': 6467}
+  keys1 = dishese.keys()
+  assert not keys.isdisjoint(keys1)
+
 
 def test_keys_update_object_updates_the_keys():
-    employee = pm.eval("({'name': 'Phil', 'age': 22})")
-    dictionaryKeys = employee.keys()
-    employee.update({'salary': 3500.0})
-    assert str(dictionaryKeys) == "dict_keys(['name', 'age', 'salary'])" 
+  employee = pm.eval("({'name': 'Phil', 'age': 22})")
+  dictionaryKeys = employee.keys()
+  employee.update({'salary': 3500.0})
+  assert str(dictionaryKeys) == "dict_keys(['name', 'age', 'salary'])"
+
 
 def test_keys_mapping():
-    dishes = pm.eval("({'eggs': 2, 'sausage': 1, 'bacon': 1, 'spam': 500})")
-    keys = dishes.keys()
-    assert str(keys.mapping) == "{'eggs': 2.0, 'sausage': 1.0, 'bacon': 1.0, 'spam': 500.0}"
-    assert keys.mapping['spam'] == 500
+  dishes = pm.eval("({'eggs': 2, 'sausage': 1, 'bacon': 1, 'spam': 500})")
+  keys = dishes.keys()
+  assert str(keys.mapping) == "{'eggs': 2.0, 'sausage': 1.0, 'bacon': 1.0, 'spam': 500.0}"
+  assert keys.mapping['spam'] == 500
+
+# values
+
 
-#values
 def test_values_iter():
-    obj = pm.eval("({ a: 123, b: 'test' })")
-    result = []
-    for i in obj.values():
-        result.append(i)
-    assert result == [123, 'test']    
+  obj = pm.eval("({ a: 123, b: 'test' })")
+  result = []
+  for i in obj.values():
+    result.append(i)
+  assert result == [123, 'test']
+
 
 def test_values_iter_reversed():
-    obj = pm.eval("({ a: 123, b: 'test' })")
-    result = []
-    for i in reversed(obj.values()):
-        result.append(i)
-    assert result == ['test', 123]        
+  obj = pm.eval("({ a: 123, b: 'test' })")
+  result = []
+  for i in reversed(obj.values()):
+    result.append(i)
+  assert result == ['test', 123]
+
 
 def test_values_list():
-    obj = pm.eval("({ a: 123, b: 'test' })")
-    assert list(obj.values()) == [123, 'test']      
+  obj = pm.eval("({ a: 123, b: 'test' })")
+  assert list(obj.values()) == [123, 'test']
+
 
 def test_values_repr():
-    car = pm.eval('({"brand": "Ford","model": "Mustang","year": 1964})')
-    a = car.values()
-    assert str(a) == "dict_values(['Ford', 'Mustang', 1964.0])"   
+  car = pm.eval('({"brand": "Ford","model": "Mustang","year": 1964})')
+  a = car.values()
+  assert str(a) == "dict_values(['Ford', 'Mustang', 1964.0])"
+
 
 def test_values_update_object_updates_the_values():
-    employee = pm.eval("({'name': 'Phil', 'age': 22})")
-    dictionaryValues = employee.values()
-    employee.update({'salary': 3500.0})
-    assert str(dictionaryValues) == "dict_values(['Phil', 22.0, 3500.0])"     
+  employee = pm.eval("({'name': 'Phil', 'age': 22})")
+  dictionaryValues = employee.values()
+  employee.update({'salary': 3500.0})
+  assert str(dictionaryValues) == "dict_values(['Phil', 22.0, 3500.0])"
+
 
 def test_values_mapping():
-    dishes = pm.eval("({'eggs': 2, 'sausage': 1, 'bacon': 1, 'spam': 500})")
-    values = dishes.values()
-    assert str(values.mapping) == "{'eggs': 2.0, 'sausage': 1.0, 'bacon': 1.0, 'spam': 500.0}"
-    assert values.mapping['spam'] == 500     
+  dishes = pm.eval("({'eggs': 2, 'sausage': 1, 'bacon': 1, 'spam': 500})")
+  values = dishes.values()
+  assert str(values.mapping) == "{'eggs': 2.0, 'sausage': 1.0, 'bacon': 1.0, 'spam': 500.0}"
+  assert values.mapping['spam'] == 500
+
+# items
+
 
-#items
 def test_items_iter():
-    obj = pm.eval("({ a: 123, b: 'test' })")
-    result = []
-    for i in obj.items():
-        result.append(i)
-    assert result == [('a', 123.0), ('b', 'test')]       
+  obj = pm.eval("({ a: 123, b: 'test' })")
+  result = []
+  for i in obj.items():
+    result.append(i)
+  assert result == [('a', 123.0), ('b', 'test')]
+
 
 def test_items_iter_reversed():
-    obj = pm.eval("({ a: 123, b: 'test' })")
-    result = []
-    for i in reversed(obj.items()):
-        result.append(i)
-    assert result == [ ('b', 'test'), ('a', 123.0)]        
-    
+  obj = pm.eval("({ a: 123, b: 'test' })")
+  result = []
+  for i in reversed(obj.items()):
+    result.append(i)
+  assert result == [('b', 'test'), ('a', 123.0)]
+
+
 def test_items_list():
-    obj = pm.eval("({ a: 123, b: 'test' })")
-    assert list(obj.items()) == [('a', 123.0), ('b', 'test')]    
+  obj = pm.eval("({ a: 123, b: 'test' })")
+  assert list(obj.items()) == [('a', 123.0), ('b', 'test')]
+
 
 def test_items_repr():
-    car = pm.eval('({"brand": "Ford","model": "Mustang","year": 1964})')
-    a = car.items()
-    assert str(a) == "dict_items([('brand', 'Ford'), ('model', 'Mustang'), ('year', 1964.0)])"       
+  car = pm.eval('({"brand": "Ford","model": "Mustang","year": 1964})')
+  a = car.items()
+  assert str(a) == "dict_items([('brand', 'Ford'), ('model', 'Mustang'), ('year', 1964.0)])"
+
 
 def test_items_substract():
-    car = pm.eval('({"brand": "Ford","model": "Mustang","year": 1964})')
-    a = car.items()
-    b = a - [('brand', 'Ford')]
-    assert b == {('model', 'Mustang'), ('year', 1964.0)}  
+  car = pm.eval('({"brand": "Ford","model": "Mustang","year": 1964})')
+  a = car.items()
+  b = a - [('brand', 'Ford')]
+  assert b == {('model', 'Mustang'), ('year', 1964.0)}
+
 
 def test_items_or():
-    dishes = pm.eval("({'eggs': 2, 'sausage': 1, 'bacon': 1, 'spam': 500})")
-    items = dishes.items()
-    others = items | [('juice', 'apple')]
-    assert others == {('spam', 500.0), ('juice', 'apple'), ('eggs', 2.0), ('sausage', 1.0), ('bacon', 1.0)}
-    others = [('juice', 'raisin')] | items
-    assert others == {('spam', 500.0), ('juice', 'raisin'), ('eggs', 2.0), ('sausage', 1.0), ('bacon', 1.0)}
+  dishes = pm.eval("({'eggs': 2, 'sausage': 1, 'bacon': 1, 'spam': 500})")
+  items = dishes.items()
+  others = items | [('juice', 'apple')]
+  assert others == {('spam', 500.0), ('juice', 'apple'), ('eggs', 2.0), ('sausage', 1.0), ('bacon', 1.0)}
+  others = [('juice', 'raisin')] | items
+  assert others == {('spam', 500.0), ('juice', 'raisin'), ('eggs', 2.0), ('sausage', 1.0), ('bacon', 1.0)}
+
 
 def test_items_xor():
-    dishes = pm.eval("({'eggs': 2, 'sausage': 1, 'bacon': 1, 'spam': 500})")
-    items = dishes.items()
-    others = items ^ {('eggs', 2)}
-    assert others == {('spam', 500), ('bacon', 1), ('sausage', 1)}   
+  dishes = pm.eval("({'eggs': 2, 'sausage': 1, 'bacon': 1, 'spam': 500})")
+  items = dishes.items()
+  others = items ^ {('eggs', 2)}
+  assert others == {('spam', 500), ('bacon', 1), ('sausage', 1)}
+
 
 def test_items_intersect_one_own_smaller():
-    dishes = pm.eval("({'eggs': 2, 'sausage': 1, 'bacon': 1, 'spam': 500})")
-    items = dishes.items()# TODO causes crash
-    b = items & {('eggs', 2), ('bacon', 1), ('salad', 12), ('jam', 34)}
-    c = {('eggs', 2), ('bacon', 1), ('salad', 12), ('jam', 34)} & items
-    assert b == {('bacon', 1), ('eggs', 2)} == c
-
-def test_items_intersect_one():    
-    dishes = pm.eval("({'eggs': 2, 'sausage': 1, 'bacon': 1, 'spam': 500})")
-    items = dishes.items()
-    b = items & {('eggs', 2)}
-    assert b == {('eggs', 2)}
-
-def test_items_intersect_none():    
-    dishes = pm.eval("({'eggs': 2, 'sausage': 1, 'bacon': 1, 'spam': 500})")
-    items = dishes.items()
-    b = items & {('ketchup', 12)}
-    assert str(b) == "set()"
+  dishes = pm.eval("({'eggs': 2, 'sausage': 1, 'bacon': 1, 'spam': 500})")
+  items = dishes.items()
+  b = items & {('eggs', 2), ('bacon', 1), ('salad', 12), ('jam', 34)}
+  c = {('eggs', 2), ('bacon', 1), ('salad', 12), ('jam', 34)} & items
+  assert b == {('bacon', 1), ('eggs', 2)} == c
+
+
+def test_items_intersect_one():
+  dishes = pm.eval("({'eggs': 2, 'sausage': 1, 'bacon': 1, 'spam': 500})")
+  items = dishes.items()
+  b = items & {('eggs', 2)}
+  assert b == {('eggs', 2)}
+
+
+def test_items_intersect_none():
+  dishes = pm.eval("({'eggs': 2, 'sausage': 1, 'bacon': 1, 'spam': 500})")
+  items = dishes.items()
+  b = items & {('ketchup', 12)}
+  assert str(b) == "set()"
+
 
 def test_items_len():
-    dishes = pm.eval("({'eggs': 2, 'sausage': 1, 'bacon': 1, 'spam': 500})")
-    items = dishes.items()
-    assert len(items) == 4
-# TODO causes crash
+  dishes = pm.eval("({'eggs': 2, 'sausage': 1, 'bacon': 1, 'spam': 500})")
+  items = dishes.items()
+  assert len(items) == 4
+
 # TODO tuple support
-#def test_items_contains(): 
+# def test_items_contains():
 #    dishes = pm.eval("({'eggs': 2, 'sausage': 1, 'bacon': 1, 'spam': 500})")
 #    items = dishes.items()
 #    assert {('eggs', 2)} in items
-    
+
+
 def test_items_update_object_updates_the_items():
-    employee = pm.eval("({'name': 'Phil', 'age': 22})")
-    dictionaryItems = employee.items()
-    employee.update({('salary', 3500.0)})
-    assert str(dictionaryItems) == "dict_items([('name', 'Phil'), ('age', 22.0), ('salary', 3500.0)])"         
-    
+  employee = pm.eval("({'name': 'Phil', 'age': 22})")
+  dictionaryItems = employee.items()
+  employee.update({('salary', 3500.0)})
+  assert str(dictionaryItems) == "dict_items([('name', 'Phil'), ('age', 22.0), ('salary', 3500.0)])"
+
+
 def test_items_mapping():
-    dishes = pm.eval("({'eggs': 2, 'sausage': 1, 'bacon': 1, 'spam': 500})")
-    items = dishes.items()
-    assert str(items.mapping) == "{'eggs': 2.0, 'sausage': 1.0, 'bacon': 1.0, 'spam': 500.0}"
-    assert items.mapping['spam'] == 500
-
-#get method
-def test_get_method():     
-    dishes = pm.eval("({'eggs': 2, 'sausage': 1, 'bacon': 1, 'spam': 500})")
-    assert dishes.get('eggs') == 2
+  dishes = pm.eval("({'eggs': 2, 'sausage': 1, 'bacon': 1, 'spam': 500})")
+  items = dishes.items()
+  assert str(items.mapping) == "{'eggs': 2.0, 'sausage': 1.0, 'bacon': 1.0, 'spam': 500.0}"
+  assert items.mapping['spam'] == 500
+
+# get method
+
+
+def test_get_method():
+  dishes = pm.eval("({'eggs': 2, 'sausage': 1, 'bacon': 1, 'spam': 500})")
+  assert dishes.get('eggs') == 2
+
+# get method shadowing
+
 
-#get method shadowing
 def test_method_shadowing():
-    jsObj = pm.eval("({get: 'value'})")
-    assert repr(jsObj.get).__contains__("<built-in method get of dict object at")
-    assert jsObj['get'] == 'value'
+  jsObj = pm.eval("({get: 'value'})")
+  assert repr(jsObj.get).__contains__("<built-in method get of dict object at")
+  assert jsObj['get'] == 'value'
+
+
+# next operator
+def test_next_operator():
+  myit = pm.eval('function* makeIt() { yield 1; yield 2; }; makeIt')()
+  first = next(myit)
+  assert (first == 1.0)
+  second = next(myit)
+  assert (second == 2.0)
+  try:
+    third = next(myit)
+    assert (False)
+  except StopIteration as e:
+    assert (True)
+  fourth = next(myit, 'default')
+  assert fourth == 'default'
```

### Comparing `pythonmonkey-0.4.0/tests/python/test_dicts.py` & `pythonmonkey-0.6.0/tests/python/test_dicts.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,333 +1,389 @@
 import pythonmonkey as pm
 import sys
 import subprocess
 
+
 def test_eval_dicts():
-    d = {"a":1}
-    proxy_d = pm.eval("(dict) => { return dict; }")(d)
-    assert d is proxy_d
+  d = {"a": 1}
+  proxy_d = pm.eval("(dict) => { return dict; }")(d)
+  assert d is proxy_d
+
 
 def test_eval_dicts_subdicts():
-    d = {"a":1, "b":{"c": 2}}
-    
-    assert pm.eval("(dict) => { return dict.a; }")(d) == 1.0
-    assert pm.eval("(dict) => { return dict.b; }")(d) is d["b"]
-    assert pm.eval("(dict) => { return dict.b.c; }")(d) == 2.0
+  d = {"a": 1, "b": {"c": 2}}
+
+  assert pm.eval("(dict) => { return dict.a; }")(d) == 1.0
+  assert pm.eval("(dict) => { return dict.b; }")(d) is d["b"]
+  assert pm.eval("(dict) => { return dict.b.c; }")(d) == 2.0
+
 
 def test_eval_dicts_cycle():
-    d: dict = {"a":1, "b":2}
-    d["recursive"] = d
-    
-    assert pm.eval("(dict) => { return dict.a; }")(d) == 1.0
-    assert pm.eval("(dict) => { return dict.b; }")(d) == 2.0
-    assert pm.eval("(dict) => { return dict.recursive; }")(d) is d["recursive"]
+  d: dict = {"a": 1, "b": 2}
+  d["recursive"] = d
+
+  assert pm.eval("(dict) => { return dict.a; }")(d) == 1.0
+  assert pm.eval("(dict) => { return dict.b; }")(d) == 2.0
+  assert pm.eval("(dict) => { return dict.recursive; }")(d) is d["recursive"]
+
 
 def test_eval_objects():
-    pyObj = pm.eval("Object({a:1.0})")
-    assert pyObj == {'a':1.0}
+  pyObj = pm.eval("Object({a:1.0})")
+  assert pyObj == {'a': 1.0}
+
 
 def test_eval_objects_subobjects():
-    pyObj = pm.eval("Object({a:1.0, b:{c:2.0}})")
+  pyObj = pm.eval("Object({a:1.0, b:{c:2.0}})")
+
+  assert pyObj['a'] == 1.0
+  assert pyObj['b'] == {'c': 2.0}
+  assert pyObj['b']['c'] == 2.0
 
-    assert pyObj['a'] == 1.0
-    assert pyObj['b'] == {'c': 2.0}
-    assert pyObj['b']['c'] == 2.0
 
 def test_eval_objects_cycle():
-    pyObj = pm.eval("Object({a:1.0, b:2.0, recursive: function() { this.recursive = this; return this; }}.recursive())")
-    
-    assert pyObj['a'] == 1.0
-    assert pyObj['b'] == 2.0
-    assert pyObj['recursive'] == pyObj
+  pyObj = pm.eval("Object({a:1.0, b:2.0, recursive: function() { this.recursive = this; return this; }}.recursive())")
+
+  assert pyObj['a'] == 1.0
+  assert pyObj['b'] == 2.0
+  assert pyObj['recursive'] == pyObj
+
 
 def test_eval_objects_proxy_get():
-    f = pm.eval("(obj) => { return obj.a}")
-    assert f({'a':42.0}) == 42.0
+  f = pm.eval("(obj) => { return obj.a}")
+  assert f({'a': 42.0}) == 42.0
+
 
 def test_eval_objects_proxy_set():
-    f = pm.eval("(obj) => { obj.a = 42.0; return;}")
-    pyObj = {}
-    f(pyObj)
-    assert pyObj['a'] == 42.0
-    
+  f = pm.eval("(obj) => { obj.a = 42.0; return;}")
+  pyObj = {}
+  f(pyObj)
+  assert pyObj['a'] == 42.0
+
+
 def test_eval_objects_proxy_keys():
-    f = pm.eval("(obj) => { return Object.keys(obj)[0]}")
-    assert f({'a':42.0}) == 'a'
+  f = pm.eval("(obj) => { return Object.keys(obj)[0]}")
+  assert f({'a': 42.0}) == 'a'
+
 
 def test_eval_objects_proxy_delete():
-    f = pm.eval("(obj) => { delete obj.a }")
-    pyObj = {'a': 42.0}
-    f(pyObj)
-    assert 'a' not in pyObj
+  f = pm.eval("(obj) => { delete obj.a }")
+  pyObj = {'a': 42.0}
+  f(pyObj)
+  assert 'a' not in pyObj
+
 
 def test_eval_objects_proxy_has():
-    f = pm.eval("(obj) => { return 'a' in obj }")
-    pyObj = {'a': 42.0}
-    assert(f(pyObj))
+  f = pm.eval("(obj) => { return 'a' in obj }")
+  pyObj = {'a': 42.0}
+  assert (f(pyObj))
+
 
 def test_eval_objects_proxy_not_extensible():
-    assert False == pm.eval("(o) => Object.isExtensible(o)")({})
-    assert False == pm.eval("(o) => Object.isExtensible(o)")({ "abc": 1 })
-    assert True == pm.eval("(o) => Object.preventExtensions(o) === o")({})
+  assert not pm.eval("(o) => Object.isExtensible(o)")({})
+  assert not pm.eval("(o) => Object.isExtensible(o)")({"abc": 1})
+  assert pm.eval("(o) => Object.preventExtensions(o) === o")({})
+
 
 def test_eval_objects_jsproxy_contains():
-    a = pm.eval("({'c':5})")
-    assert 'c' in a
+  a = pm.eval("({'c':5})")
+  assert 'c' in a
+
 
 def test_eval_objects_jsproxy_does_not_contain():
-    a = pm.eval("({'c':5})")
-    assert not(4 in a)
+  a = pm.eval("({'c':5})")
+  assert not (4 in a)
+
 
 def test_eval_objects_jsproxy_does_not_contain_value():
-    a = pm.eval("({'c':5})")
-    assert not(5 in a)
+  a = pm.eval("({'c':5})")
+  assert not (5 in a)
+
 
 def test_eval_objects_jsproxy_or():
-  if sys.version_info[0] >= 3 and sys.version_info[1] >= 9: # | is not implemented for dicts in 3.8 or less
+  if sys.version_info[0] >= 3 and sys.version_info[1] >= 9:  # | is not implemented for dicts in 3.8 or less
     a = pm.eval("({'c':5})")
     b = pm.eval("({'d':6})")
     c = a | b
-    assert a == {'c': 5.0}  
-    assert c == {'c': 5.0, 'd': 6.0}   
-    assert b == {'d': 6.0} 
+    assert a == {'c': 5.0}
+    assert c == {'c': 5.0, 'd': 6.0}
+    assert b == {'d': 6.0}
+
 
 def test_eval_objects_jsproxy_or_true_dict_right():
-  if sys.version_info[0] >= 3 and sys.version_info[1] >= 9: # | is not implemented for dicts in 3.8 or less
+  if sys.version_info[0] >= 3 and sys.version_info[1] >= 9:  # | is not implemented for dicts in 3.8 or less
     a = pm.eval("({'c':5})")
     b = {'d': 6.0}
     c = a | b
-    assert a == {'c': 5.0}  
-    assert c == {'c': 5.0, 'd': 6.0}   
-    assert b == {'d': 6.0} 
+    assert a == {'c': 5.0}
+    assert c == {'c': 5.0, 'd': 6.0}
+    assert b == {'d': 6.0}
+
 
 def test_eval_objects_jsproxy_or_true_dict_left():
-  if sys.version_info[0] >= 3 and sys.version_info[1] >= 9: # | is not implemented for dicts in 3.8 or less
-    a = {'c':5}
+  if sys.version_info[0] >= 3 and sys.version_info[1] >= 9:  # | is not implemented for dicts in 3.8 or less
+    a = {'c': 5}
     b = pm.eval("({'d':6})")
     c = a | b
-    assert a == {'c': 5.0}  
-    assert c == {'c': 5.0, 'd': 6.0}   
-    assert b == {'d': 6.0} 
+    assert a == {'c': 5.0}
+    assert c == {'c': 5.0, 'd': 6.0}
+    assert b == {'d': 6.0}
+
 
 def test_eval_objects_jsproxy_inplace_or():
-  if sys.version_info[0] >= 3 and sys.version_info[1] >= 9: # | is not implemented for dicts in 3.8 or less
+  if sys.version_info[0] >= 3 and sys.version_info[1] >= 9:  # | is not implemented for dicts in 3.8 or less
     a = pm.eval("({'c':5})")
     b = pm.eval("({'d':6})")
     a |= b
-    assert a == {'c': 5.0, 'd': 6.0}   
-    assert b == {'d': 6.0}       
+    assert a == {'c': 5.0, 'd': 6.0}
+    assert b == {'d': 6.0}
+
 
 def test_eval_objects_jsproxy_inplace_or_true_dict_right():
-  if sys.version_info[0] >= 3 and sys.version_info[1] >= 9: # | is not implemented for dicts in 3.8 or less
+  if sys.version_info[0] >= 3 and sys.version_info[1] >= 9:  # | is not implemented for dicts in 3.8 or less
     a = pm.eval("({'c':5})")
-    b = {'d':6.0}
+    b = {'d': 6.0}
     a |= b
-    assert a == {'c': 5.0, 'd': 6.0}   
-    assert b == {'d': 6.0}       
+    assert a == {'c': 5.0, 'd': 6.0}
+    assert b == {'d': 6.0}
+
 
 def test_eval_objects_jsproxy_inplace_or_true_dict_left():
-  if sys.version_info[0] >= 3 and sys.version_info[1] >= 9: # | is not implemented for dicts in 3.8 or less
-    a = {'c':5.0}
+  if sys.version_info[0] >= 3 and sys.version_info[1] >= 9:  # | is not implemented for dicts in 3.8 or less
+    a = {'c': 5.0}
     b = pm.eval("({'d':6})")
     a |= b
-    assert a == {'c': 5.0, 'd': 6.0}   
-    assert b == {'d': 6.0}   
-    assert True == pm.eval("(o) => Object.preventExtensions(o) === o")({ "abc": 1 })
+    assert a == {'c': 5.0, 'd': 6.0}
+    assert b == {'d': 6.0}
+    assert pm.eval("(o) => Object.preventExtensions(o) === o")({"abc": 1})
+
 
 def test_instanceof_object():
-    a = {'c':5.0}
-    result = [None]
-    pm.eval("(result, obj) => {result[0] = obj instanceof Object}")(result, a)
-    assert result[0] == True
+  a = {'c': 5.0}
+  result = [None]
+  pm.eval("(result, obj) => {result[0] = obj instanceof Object}")(result, a)
+  assert result[0]
+
+# iter
+
 
-#iter
 def test_eval_objects_proxy_iterate():
-    obj = pm.eval("({ a: 123, b: 'test' })")
-    result = []
-    for i in obj:
-        result.append(i)
-    assert result == ['a', 'b']
+  obj = pm.eval("({ a: 123, b: 'test' })")
+  result = []
+  for i in obj:
+    result.append(i)
+  assert result == ['a', 'b']
+
 
 def test_eval_objects_proxy_min():
-    obj = pm.eval("({ a: 123, b: 'test' })")
-    assert min(obj) == 'a'
+  obj = pm.eval("({ a: 123, b: 'test' })")
+  assert min(obj) == 'a'
+
 
 def test_eval_objects_proxy_max():
-    obj = pm.eval("({ a: 123, b: 'test' })")
-    assert max(obj) == 'b'
+  obj = pm.eval("({ a: 123, b: 'test' })")
+  assert max(obj) == 'b'
+
 
 def test_eval_objects_proxy_repr():
-    obj = pm.eval("({ a: 123, b: 'test' , c: { d: 1 }})")
-    obj.e = obj # supporting circular references
-    expected = "{'a': 123.0, 'b': 'test', 'c': {'d': 1.0}, 'e': {...}}"
-    assert repr(obj) == expected
-    assert str(obj) == expected
+  obj = pm.eval("({ a: 123, b: 'test' , c: { d: 1 }})")
+  obj.e = obj  # supporting circular references
+  expected = "{'a': 123.0, 'b': 'test', 'c': {'d': 1.0}, 'e': {...}}"
+  assert repr(obj) == expected
+  assert str(obj) == expected
+
 
 def test_eval_objects_proxy_dict_conversion():
-    obj = pm.eval("({ a: 123, b: 'test' , c: { d: 1 }})")
-    d = dict(obj)
-    assert type(obj) is not dict # dict subclass
-    assert type(d) is dict # strict dict
-    assert repr(d) == "{'a': 123.0, 'b': 'test', 'c': {'d': 1.0}}"
-    assert str(obj.keys()) == "dict_keys(['a', 'b', 'c'])"
-    assert obj == d
+  obj = pm.eval("({ a: 123, b: 'test' , c: { d: 1 }})")
+  d = dict(obj)
+  assert type(obj) is not dict  # dict subclass
+  assert type(d) is dict  # strict dict
+  assert repr(d) == "{'a': 123.0, 'b': 'test', 'c': {'d': 1.0}}"
+  assert str(obj.keys()) == "dict_keys(['a', 'b', 'c'])"
+  assert obj == d
+
 
 def test_eval_objects_jsproxy_get():
-    proxy = pm.eval("({a: 1})")
-    assert 1.0 == proxy['a']
-    assert 1.0 == proxy.a
+  proxy = pm.eval("({a: 1})")
+  assert 1.0 == proxy['a']
+  assert 1.0 == proxy.a
+
 
 def test_eval_objects_jsproxy_set():
-    proxy = pm.eval("({a: 1})")
-    proxy.a = 2.0
-    assert 2.0 == proxy['a']
-    proxy['a'] = 3.0
-    assert 3.0 == proxy.a
-    proxy.b = 1.0
-    assert 1.0 == proxy['b']
-    proxy['b'] = 2.0
-    assert 2.0 == proxy.b
+  proxy = pm.eval("({a: 1})")
+  proxy.a = 2.0
+  assert 2.0 == proxy['a']
+  proxy['a'] = 3.0
+  assert 3.0 == proxy.a
+  proxy.b = 1.0
+  assert 1.0 == proxy['b']
+  proxy['b'] = 2.0
+  assert 2.0 == proxy.b
+
 
 def test_eval_objects_jsproxy_length():
-    proxy = pm.eval("({a: 1, b:2})")
-    assert 2 == len(proxy)
+  proxy = pm.eval("({a: 1, b:2})")
+  assert 2 == len(proxy)
+
 
 def test_eval_objects_jsproxy_delete():
-    proxy = pm.eval("({a: 1})")
-    del proxy.a
-    assert None == proxy.a
-    assert None == proxy['a']
+  proxy = pm.eval("({a: 1})")
+  del proxy.a
+  assert None is proxy.a
+  assert None is proxy['a']
+
 
 def test_eval_objects_jsproxy_compare():
-    proxy = pm.eval("({a: 1, b:2})")
-    assert proxy == {'a': 1.0, 'b': 2.0}
+  proxy = pm.eval("({a: 1, b:2})")
+  assert proxy == {'a': 1.0, 'b': 2.0}
+
 
 def test_eval_objects_jsproxy_contains():
-    a = pm.eval("({'c':5})")
-    assert 'c' in a
+  a = pm.eval("({'c':5})")
+  assert 'c' in a
+
 
 def test_eval_objects_jsproxy_does_not_contain():
-    a = pm.eval("({'c':5})")
-    assert not(4 in a)
+  a = pm.eval("({'c':5})")
+  assert not (4 in a)
+
 
 def test_eval_objects_jsproxy_does_not_contain_value():
-    a = pm.eval("({'c':5})")
-    assert not(5 in a)
+  a = pm.eval("({'c':5})")
+  assert not (5 in a)
+
 
 def test_eval_objects_jsproxy_or():
-  if sys.version_info[0] >= 3 and sys.version_info[1] >= 9: # | is not implemented for dicts in 3.8 or less
+  if sys.version_info[0] >= 3 and sys.version_info[1] >= 9:  # | is not implemented for dicts in 3.8 or less
     a = pm.eval("({'c':5})")
     b = pm.eval("({'d':6})")
     c = a | b
-    assert a == {'c': 5.0}  
-    assert c == {'c': 5.0, 'd': 6.0}   
-    assert b == {'d': 6.0} 
+    assert a == {'c': 5.0}
+    assert c == {'c': 5.0, 'd': 6.0}
+    assert b == {'d': 6.0}
+
 
 def test_eval_objects_jsproxy_or_true_dict_right():
-  if sys.version_info[0] >= 3 and sys.version_info[1] >= 9: # | is not implemented for dicts in 3.8 or less
+  if sys.version_info[0] >= 3 and sys.version_info[1] >= 9:  # | is not implemented for dicts in 3.8 or less
     a = pm.eval("({'c':5})")
     b = {'d': 6.0}
     c = a | b
-    assert a == {'c': 5.0}  
-    assert c == {'c': 5.0, 'd': 6.0}   
-    assert b == {'d': 6.0} 
+    assert a == {'c': 5.0}
+    assert c == {'c': 5.0, 'd': 6.0}
+    assert b == {'d': 6.0}
+
 
 def test_eval_objects_jsproxy_or_true_dict_left():
-  if sys.version_info[0] >= 3 and sys.version_info[1] >= 9: # | is not implemented for dicts in 3.8 or less
-    a = {'c':5}
+  if sys.version_info[0] >= 3 and sys.version_info[1] >= 9:  # | is not implemented for dicts in 3.8 or less
+    a = {'c': 5}
     b = pm.eval("({'d':6})")
     c = a | b
-    assert a == {'c': 5.0}  
-    assert c == {'c': 5.0, 'd': 6.0}   
-    assert b == {'d': 6.0} 
+    assert a == {'c': 5.0}
+    assert c == {'c': 5.0, 'd': 6.0}
+    assert b == {'d': 6.0}
+
 
 def test_eval_objects_jsproxy_inplace_or():
-  if sys.version_info[0] >= 3 and sys.version_info[1] >= 9: # | is not implemented for dicts in 3.8 or less
+  if sys.version_info[0] >= 3 and sys.version_info[1] >= 9:  # | is not implemented for dicts in 3.8 or less
     a = pm.eval("({'c':5})")
     b = pm.eval("({'d':6})")
     a |= b
-    assert a == {'c': 5.0, 'd': 6.0}   
-    assert b == {'d': 6.0}       
+    assert a == {'c': 5.0, 'd': 6.0}
+    assert b == {'d': 6.0}
+
 
 def test_eval_objects_jsproxy_inplace_or_true_dict_right():
-  if sys.version_info[0] >= 3 and sys.version_info[1] >= 9: # | is not implemented for dicts in 3.8 or less
+  if sys.version_info[0] >= 3 and sys.version_info[1] >= 9:  # | is not implemented for dicts in 3.8 or less
     a = pm.eval("({'c':5})")
-    b = {'d':6.0}
+    b = {'d': 6.0}
     a |= b
-    assert a == {'c': 5.0, 'd': 6.0}   
-    assert b == {'d': 6.0}       
+    assert a == {'c': 5.0, 'd': 6.0}
+    assert b == {'d': 6.0}
+
 
 def test_eval_objects_jsproxy_inplace_or_true_dict_left():
-  if sys.version_info[0] >= 3 and sys.version_info[1] >= 9: # | is not implemented for dicts in 3.8 or less
-    a = {'c':5.0}
+  if sys.version_info[0] >= 3 and sys.version_info[1] >= 9:  # | is not implemented for dicts in 3.8 or less
+    a = {'c': 5.0}
     b = pm.eval("({'d':6})")
     a |= b
-    assert a == {'c': 5.0, 'd': 6.0}   
+    assert a == {'c': 5.0, 'd': 6.0}
     assert b == {'d': 6.0}
 
+
 def test_eval_objects_jsproxy_inplace_or_true_dict_left_iterable_right():
-  if sys.version_info[0] >= 3 and sys.version_info[1] >= 9: # | is not implemented for dicts in 3.8 or less
+  if sys.version_info[0] >= 3 and sys.version_info[1] >= 9:  # | is not implemented for dicts in 3.8 or less
     a = {'c': 5}
     a |= [('y', 3), ('z', 0)]
-    assert a == {'c': 5, 'y': 3, 'z':0}   
+    assert a == {'c': 5, 'y': 3, 'z': 0}
+
 
 def test_update_inplace_or_iterable_wrong_type():
-    car = pm.eval('({"brand": "Ford","model": "Mustang","year": 1964})')
-    a = [1,2]
-    try:
-        car |= a          
-        assert (False)
-    except Exception as e:    
-        assert str(type(e)) == "<class 'TypeError'>"
-        assert str(e) == "cannot convert dictionary update sequence element #0 to a sequence"       
+  car = pm.eval('({"brand": "Ford","model": "Mustang","year": 1964})')
+  a = [1, 2]
+  try:
+    car |= a
+    assert (False)
+  except Exception as e:
+    assert str(type(e)) == "<class 'TypeError'>"
+    assert str(e) == "cannot convert dictionary update sequence element #0 to a sequence"
+
 
 def test_instanceof_object():
-    items = {'a': 10}
-    result = [None]
-    pm.eval("(result, obj) => {result[0] = obj instanceof Object}")(result, items)
-    assert result[0] == True         
+  items = {'a': 10}
+  result = [None]
+  pm.eval("(result, obj) => {result[0] = obj instanceof Object}")(result, items)
+  assert result[0]
+
 
 def test_not_instanceof_string():
-    items = {'a': 10}
-    result = [None]
-    pm.eval("(result, obj) => {result[0] = obj instanceof String}")(result, items)
-    assert result[0] == False           
+  items = {'a': 10}
+  result = [None]
+  pm.eval("(result, obj) => {result[0] = obj instanceof String}")(result, items)
+  assert not result[0]
+
+# valueOf
+
 
-#valueOf
 def test_valueOf():
-    items = {'a': 10}
-    result = [0]
-    pm.eval("(result, obj) => {result[0] = obj.valueOf()}")(result, items)
-    assert items == {'a': 10} 
-    assert result[0] is items
+  items = {'a': 10}
+  result = [0]
+  pm.eval("(result, obj) => {result[0] = obj.valueOf()}")(result, items)
+  assert items == {'a': 10}
+  assert result[0] is items
 
 # toString
+
+
 def test_toString():
-    items = {'a': 10}
-    result = [0]
-    pm.eval("(result, obj) => {result[0] = obj.toString()}")(result, items)
-    assert result[0] == '[object Object]'  
+  items = {'a': 10}
+  result = [0]
+  pm.eval("(result, obj) => {result[0] = obj.toString()}")(result, items)
+  assert result[0] == '[object Object]'
 
 # toLocaleString
+
+
 def test_toLocaleString():
-    items = {'a': 10}
-    result = [0]
-    pm.eval("(result, obj) => {result[0] = obj.toLocaleString()}")(result, items)
-    assert result[0] == '[object Object]'
-    
-#repr
+  items = {'a': 10}
+  result = [0]
+  pm.eval("(result, obj) => {result[0] = obj.toLocaleString()}")(result, items)
+  assert result[0] == '[object Object]'
+
+# repr
+
+
 def test_repr_max_recursion_depth():
-    subprocess.check_call('npm install crypto-js', shell=True)
-    CryptoJS = pm.require('crypto-js')
-    assert str(CryptoJS).__contains__("{'lib': {'Base': {'extend':")  
-     
-
-#__class__
-def test___class__attribute():  
-    items = pm.eval("({'a': 10})")
-    assert repr(items.__class__) == "<class 'dict'>"
-
-#none value attribute
-def test___none__attribute():  
-    a = pm.eval("({'0': 1, '1': 2})")
-    assert a[2] is None    
+  subprocess.check_call('npm install crypto-js', shell=True)
+  CryptoJS = pm.require('crypto-js')
+  assert str(CryptoJS).__contains__("{'lib': {'Base': {'extend':")
+
+
+# __class__
+def test___class__attribute():
+  items = pm.eval("({'a': 10})")
+  assert repr(items.__class__) == "<class 'dict'>"
+
+# none value attribute
+
+
+def test___none__attribute():
+  a = pm.eval("({'0': 1, '1': 2})")
+  assert a[2] is None
```

### Comparing `pythonmonkey-0.4.0/tests/python/test_event_loop.py` & `pythonmonkey-0.6.0/tests/python/test_event_loop.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,275 +1,363 @@
 import pytest
 import pythonmonkey as pm
 import asyncio
 
-def test_timers_unref():
-    async def async_fn():
-        obj = {'val': 0}
-        pm.eval("""(obj) => {
-            setTimeout(()=>{ obj.val = 2 }, 1000).ref().ref().unref().ref().unref().unref(); 
+
+def test_setTimeout_unref():
+  async def async_fn():
+    obj = {'val': 0}
+    pm.eval("""(obj) => {
+            setTimeout(()=>{ obj.val = 2 }, 1000).ref().ref().unref().ref().unref().unref();
                 // chaining, no use on the first two ref calls since it's already refed initially
             setTimeout(()=>{ obj.val = 1 }, 100);
         }""")(obj)
-        await pm.wait() # we shouldn't wait until the first timer is fired since it's currently unrefed
-        assert obj['val'] == 1
+    await pm.wait()  # we shouldn't wait until the first timer is fired since it's currently unrefed
+    assert obj['val'] == 1
+
+    # making sure the async_fn is run
+    return True
+  assert asyncio.run(async_fn())
+
+
+def test_setInterval_unref():
+  async def async_fn():
+    obj = {'val': 0}
+    pm.eval("""(obj) => {
+            setInterval(()=>{ obj.val++ }, 200).unref()
+            setTimeout(()=>{ }, 500)
+        }""")(obj)
+    await pm.wait()  # It should stop after the setTimeout timer's 500ms.
+    assert obj['val'] == 2  # The setInterval timer should only run twice (500 // 200 == 2)
+    return True
+  assert asyncio.run(async_fn())
+
+
+def test_finished_timer_ref():
+  async def async_fn():
+    # Making sure the event-loop won't be activated again when a finished timer gets re-refed.
+    pm.eval("""
+            const timer = setTimeout(()=>{}, 100);
+            setTimeout(()=>{ timer.ref() }, 200);
+        """)
+    await pm.wait()
+    return True
+  assert asyncio.run(async_fn())
 
-        # making sure the async_fn is run
-        return True
-    assert asyncio.run(async_fn())
 
 def test_set_clear_timeout():
-    # throw RuntimeError outside a coroutine
-    with pytest.raises(RuntimeError, match="PythonMonkey cannot find a running Python event-loop to make asynchronous calls."):
-        pm.eval("setTimeout")(print)
-
-    async def async_fn():
-        # standalone `setTimeout`
-        loop = asyncio.get_running_loop()
-        f0 = loop.create_future()
-        def add(a, b, c):
-          f0.set_result(a + b + c)
-        pm.eval("setTimeout")(add, 0, 1, 2, 3)
-        assert 6.0 == await f0
-
-        # test `clearTimeout`
-        f1 = loop.create_future()
-        def to_raise(msg):
-            f1.set_exception(TypeError(msg))
-        timeout_id0 = pm.eval("setTimeout")(to_raise, 100, "going to be there")
-        # `setTimeout` should return a `Timeout` instance wrapping a positive integer value
-        assert pm.eval("(t) => t instanceof setTimeout.Timeout")(timeout_id0)
-        assert pm.eval("(t) => Number(t) > 0")(timeout_id0)
-        assert pm.eval("(t) => Number.isInteger(Number(t))")(timeout_id0)
-        with pytest.raises(TypeError, match="going to be there"):
-            await f1                                # `clearTimeout` not called
-        f1 = loop.create_future()
-        timeout_id1 = pm.eval("setTimeout")(to_raise, 100, "shouldn't be here")
-        pm.eval("clearTimeout")(timeout_id1)
-        with pytest.raises(asyncio.exceptions.TimeoutError):
-            await asyncio.wait_for(f1, timeout=0.5) # `clearTimeout` is called
-
-        # `this` value in `setTimeout` callback should be the global object, as spec-ed
-        assert await pm.eval("new Promise(function (resolve) { setTimeout(function(){ resolve(this == globalThis) }) })")
-        # `setTimeout` should allow passing additional arguments to the callback, as spec-ed
-        assert 3.0 == await pm.eval("new Promise((resolve) => setTimeout(function(){ resolve(arguments.length) }, 100, 90, 91, 92))")
-        assert 92.0 == await pm.eval("new Promise((resolve) => setTimeout((...args) => { resolve(args[2]) }, 100, 90, 91, 92))")
-        # test `setTimeout` setting delay to 0 if < 0
-        await asyncio.wait_for(pm.eval("new Promise((resolve) => setTimeout(resolve, 0))"), timeout=0.05)
-        await asyncio.wait_for(pm.eval("new Promise((resolve) => setTimeout(resolve, -10000))"), timeout=0.05) # won't be precisely 0s
-        # test `setTimeout` accepting string as the delay, coercing to a number.
-        # Number('100') -> 100, pass if the actual delay is > 90ms and < 150ms
-        await asyncio.wait_for(pm.eval("new Promise((resolve) => setTimeout(resolve, '100'))"), timeout=0.15) # won't be precisely 100ms
-        with pytest.raises(asyncio.exceptions.TimeoutError):
-            await asyncio.wait_for(pm.eval("new Promise((resolve) => setTimeout(resolve, '100'))"), timeout=0.09)
-        # Number("1 second") -> NaN -> delay turns to be 0s
-        await asyncio.wait_for(pm.eval("new Promise((resolve) => setTimeout(resolve, '1 second'))"), timeout=0.5) # won't be precisely 0s
-
-        # passing an invalid ID to `clearTimeout` should silently do nothing; no exception is thrown.
-        pm.eval("clearTimeout(NaN)")
-        pm.eval("clearTimeout(999)")
-        pm.eval("clearTimeout(-1)")
-        pm.eval("clearTimeout('a')")
-        pm.eval("clearTimeout(undefined)")
-        pm.eval("clearTimeout()")
+  # throw RuntimeError outside a coroutine
+  with pytest.raises(RuntimeError,
+                     match="PythonMonkey cannot find a running Python event-loop to make asynchronous calls."):
+    pm.eval("setTimeout")(print)
+
+  async def async_fn():
+    # standalone `setTimeout`
+    loop = asyncio.get_running_loop()
+    f0 = loop.create_future()
+
+    def add(a, b, c):
+      f0.set_result(a + b + c)
+    pm.eval("setTimeout")(add, 0, 1, 2, 3)
+    assert 6.0 == await f0
+
+    # test `clearTimeout`
+    f1 = loop.create_future()
+
+    def to_raise(msg):
+      f1.set_exception(TypeError(msg))
+    timeout_id0 = pm.eval("setTimeout")(to_raise, 100, "going to be there")
+    # `setTimeout` should return a `Timeout` instance wrapping a positive integer value
+    assert pm.eval("(t) => t instanceof setTimeout.Timeout")(timeout_id0)
+    assert pm.eval("(t) => Number(t) > 0")(timeout_id0)
+    assert pm.eval("(t) => Number.isInteger(Number(t))")(timeout_id0)
+    with pytest.raises(TypeError, match="going to be there"):
+      await f1                                # `clearTimeout` not called
+    f1 = loop.create_future()
+    timeout_id1 = pm.eval("setTimeout")(to_raise, 100, "shouldn't be here")
+    pm.eval("clearTimeout")(timeout_id1)
+    with pytest.raises(asyncio.exceptions.TimeoutError):
+      await asyncio.wait_for(f1, timeout=0.5)  # `clearTimeout` is called
+
+    # `this` value in `setTimeout` callback should be the global object, as spec-ed
+    assert await pm.eval("new Promise(function (resolve) { setTimeout(function(){ resolve(this == globalThis) }) })")
+    # `setTimeout` should allow passing additional arguments to the callback, as spec-ed
+    assert 3.0 == await pm.eval("""
+                    new Promise((resolve) => setTimeout(function(){
+                      resolve(arguments.length);
+                    },
+                    100, 90, 91, 92))
+                  """)
+    assert 92.0 == await pm.eval("""
+                      new Promise((resolve) => setTimeout((...args) => {
+                        resolve(args[2]);
+                      },
+                      100, 90, 91, 92))
+                    """)
+    # test `setTimeout` setting delay to 0 if < 0
+    await asyncio.wait_for(pm.eval("new Promise((resolve) => setTimeout(resolve, 0))"), timeout=0.05)
+    # won't be precisely 0s
+    await asyncio.wait_for(pm.eval("new Promise((resolve) => setTimeout(resolve, -10000))"), timeout=0.05)
+    # test `setTimeout` accepting string as the delay, coercing to a number.
+    # Number('100') -> 100, pass if the actual delay is > 90ms and < 150ms
+    # won't be precisely 100ms
+    await asyncio.wait_for(pm.eval("new Promise((resolve) => setTimeout(resolve, '100'))"), timeout=0.15)
+    with pytest.raises(asyncio.exceptions.TimeoutError):
+      await asyncio.wait_for(pm.eval("new Promise((resolve) => setTimeout(resolve, '100'))"), timeout=0.09)
+    # Number("1 second") -> NaN -> delay turns to be 0s
+    # won't be precisely 0s
+    await asyncio.wait_for(pm.eval("new Promise((resolve) => setTimeout(resolve, '1 second'))"), timeout=0.5)
+
+    # passing an invalid ID to `clearTimeout` should silently do nothing; no exception is thrown.
+    pm.eval("clearTimeout(NaN)")
+    pm.eval("clearTimeout(999)")
+    pm.eval("clearTimeout(-1)")
+    pm.eval("clearTimeout('a')")
+    pm.eval("clearTimeout(undefined)")
+    pm.eval("clearTimeout()")
 
-        # passing a `code` string to `setTimeout` as the callback function
-        assert "code string" == await pm.eval("""
+    # passing a `code` string to `setTimeout` as the callback function
+    assert "code string" == await pm.eval("""
         new Promise((resolve) => {
             globalThis._resolve = resolve
             setTimeout("globalThis._resolve('code string'); delete globalThis._resolve", 100)
         })
         """)
 
-        # making sure the async_fn is run
-        return True
-    assert asyncio.run(async_fn())
-
-    # throw RuntimeError outside a coroutine (the event-loop has ended)
-    with pytest.raises(RuntimeError, match="PythonMonkey cannot find a running Python event-loop to make asynchronous calls."):
-        pm.eval("setTimeout")(print)
+    # making sure the async_fn is run
+    return True
+  assert asyncio.run(async_fn())
+
+  # throw RuntimeError outside a coroutine (the event-loop has ended)
+  with pytest.raises(RuntimeError,
+                     match="PythonMonkey cannot find a running Python event-loop to make asynchronous calls."):
+    pm.eval("setTimeout")(print)
+
 
 def test_promises():
-    # should throw RuntimeError if Promises are created outside a coroutine
-    create_promise = pm.eval("() => Promise.resolve(1)")
-    with pytest.raises(RuntimeError, match="PythonMonkey cannot find a running Python event-loop to make asynchronous calls."):
-        create_promise()
-
-    async def async_fn():
-        create_promise() # inside a coroutine, no error
-
-        # Python awaitables to JS Promise coercion
-        # 1. Python asyncio.Future to JS promise
-        loop = asyncio.get_running_loop()
-        f0 = loop.create_future()
-        f0.set_result(2561)
-        assert type(f0) == asyncio.Future
-        assert 2561 == await f0
-        assert pm.eval("(p) => p instanceof Promise")(f0) is True
-        assert 2561 == await pm.eval("(p) => p")(f0)
-        del f0
-
-        # 2. Python asyncio.Task to JS promise
-        async def coro_fn(x):
-            await asyncio.sleep(0.01)
-            return x
-        task = loop.create_task(coro_fn("from a Task"))
-        assert type(task) == asyncio.Task
-        assert type(task) != asyncio.Future
-        assert isinstance(task, asyncio.Future)
-        assert "from a Task" == await task
-        assert pm.eval("(p) => p instanceof Promise")(task) is True
-        assert "from a Task" == await pm.eval("(p) => p")(task)
-        del task
-
-        # 3. Python coroutine to JS promise
-        coro = coro_fn("from a Coroutine")
-        assert asyncio.iscoroutine(coro)
-        # assert "a Coroutine" == await coro                            # coroutines cannot be awaited more than once
-        # assert pm.eval("(p) => p instanceof Promise")(coro) is True   #   RuntimeError: cannot reuse already awaited coroutine
-        assert "from a Coroutine" == await pm.eval("(p) => (p instanceof Promise) && p")(coro)
-        del coro
-
-        # JS Promise to Python awaitable coercion
-        assert 100 == await pm.eval("new Promise((r)=>{ r(100) })")
-        assert 10010 == await pm.eval("Promise.resolve(10010)")
-        with pytest.raises(pm.SpiderMonkeyError, match="^TypeError: (.|\\n)+ is not a constructor$"):
-            await pm.eval("Promise.resolve")(10086)
-        assert 10086 == await pm.eval("Promise.resolve.bind(Promise)")(10086)
-
-        assert "promise returning a function" == (await pm.eval("Promise.resolve(() => { return 'promise returning a function' })"))()
-        assert "function 2" == (await pm.eval("Promise.resolve(x=>x)"))("function 2")
-        def aaa(n):
-            return n
-        ident0 = await (pm.eval("Promise.resolve.bind(Promise)")(aaa))
-        assert "from aaa" == ident0("from aaa")
-        ident1 = await pm.eval("async (aaa) => x=>aaa(x)")(aaa)
-        assert "from ident1" == ident1("from ident1")
-        ident2 = await pm.eval("() => Promise.resolve(x=>x)")()
-        assert "from ident2" == ident2("from ident2")
-        ident3 = await pm.eval("(aaa) => Promise.resolve(x=>aaa(x))")(aaa)
-        assert "from ident3" == ident3("from ident3")
-        del aaa
-
-        # promise returning a JS Promise<Function> that calls a Python function inside
-        def fn0(n):
-            return n + 100
-        def fn1():
-            return pm.eval("async x=>x")(fn0)
-        fn2 = await pm.eval("async (fn1) => { const fn0 = await fn1(); return Promise.resolve(x=>fn0(x)) }")(fn1)
-        assert 101.2 == fn2(1.2)
-        fn3 = await pm.eval("async (fn1) => { const fn0 = await fn1(); return Promise.resolve(async x => { return fn0(x) }) }")(fn1)
-        assert 101.3 == await fn3(1.3)
-        fn4 = await pm.eval("async (fn1) => { return Promise.resolve(async x => { const fn0 = await fn1(); return fn0(x) }) }")(fn1)
-        assert 101.4 == await fn4(1.4)
-        
-        # chained JS promises
-        assert "chained" == await (pm.eval("async () => new Promise((resolve) => resolve( Promise.resolve().then(()=>'chained') ))")())
-
-        # chained Python awaitables
-        async def a():
-            await asyncio.sleep(0.01)
-            return "nested"
-        async def b():
-            await asyncio.sleep(0.01)
-            return a()
-        async def c():
-            await asyncio.sleep(0.01)
-            return b()
-        # JS `await` supports chaining. However, on Python-land, it actually requires `await (await (await c()))`
-        assert "nested" == await pm.eval("async (promise) => await promise")(c())
-        assert "nested" == await pm.eval("async (promise) => await promise")(await c())
-        assert "nested" == await pm.eval("async (promise) => await promise")(await (await c()))
-        assert "nested" == await pm.eval("async (promise) => await promise")(await (await (await c())))
-        assert "nested" == await pm.eval("async (promise) => promise")(c())
-        assert "nested" == await pm.eval("async (promise) => promise")(await c())
-        assert "nested" == await pm.eval("async (promise) => promise")(await (await c()))
-        assert "nested" == await pm.eval("async (promise) => promise")(await (await (await c())))
-        assert "nested" == await pm.eval("(promise) => Promise.resolve(promise)")(c())
-        assert "nested" == await pm.eval("(promise) => Promise.resolve(promise)")(await c())
-        assert "nested" == await pm.eval("(promise) => Promise.resolve(promise)")(await (await c()))
-        assert "nested" == await pm.eval("(promise) => Promise.resolve(promise)")(await (await (await c())))
-        assert "nested" == await pm.eval("(promise) => promise")(c())
-        assert "nested" == await pm.eval("(promise) => promise")(await c())
-        assert "nested" == await pm.eval("(promise) => promise")(await (await c()))
-        with pytest.raises(TypeError, match="object str can't be used in 'await' expression"):
-            await pm.eval("(promise) => promise")(await (await (await c())))
-
-        # Python awaitable throwing exceptions
-        async def coro_to_throw0():
-            await asyncio.sleep(0.01)
-            print([].non_exist) # type: ignore
-        with pytest.raises(pm.SpiderMonkeyError, match="Python AttributeError: 'list' object has no attribute 'non_exist'"):
-            await (pm.eval("(promise) => promise")(coro_to_throw0()))
-        with pytest.raises(pm.SpiderMonkeyError, match="Python AttributeError: 'list' object has no attribute 'non_exist'"):
-            await (pm.eval("async (promise) => promise")(coro_to_throw0()))
-        with pytest.raises(pm.SpiderMonkeyError, match="Python AttributeError: 'list' object has no attribute 'non_exist'"):
-            await (pm.eval("(promise) => Promise.resolve().then(async () => await promise)")(coro_to_throw0()))
-        async def coro_to_throw1():
-            await asyncio.sleep(0.01)
-            raise TypeError("reason")
-        with pytest.raises(pm.SpiderMonkeyError, match="Python TypeError: reason"):
-            await (pm.eval("(promise) => promise")(coro_to_throw1()))
-        assert 'rejected <Python TypeError: reason>' == await pm.eval("(promise) => promise.then(()=>{}, (err)=>`rejected <${err.message}>`)")(coro_to_throw1())
-
-        # JS Promise throwing exceptions
-        with pytest.raises(pm.SpiderMonkeyError, match="nan"):
-            await pm.eval("Promise.reject(NaN)") # JS can throw anything
-        with pytest.raises(pm.SpiderMonkeyError, match="123.0"):
-            await (pm.eval("async () => { throw 123 }")())
-            # await (pm.eval("async () => { throw {} }")())
-        with pytest.raises(pm.SpiderMonkeyError, match="anything"):
-            await pm.eval("Promise.resolve().then(()=>{ throw 'anything' })")
-            # FIXME (Tom Tang): We currently handle Promise exceptions by converting the object thrown to a Python Exception object through `pyTypeFactory`
-            #               <objects of this type are not handled by PythonMonkey yet>
-            # await pm.eval("Promise.resolve().then(()=>{ throw {a:1,toString(){return'anything'}} })")
-        with pytest.raises(pm.SpiderMonkeyError, match="on line 1, column 31:\nTypeError: undefined has no properties"): # not going through the conversion
-            await pm.eval("Promise.resolve().then(()=>{ (undefined).prop })")
-
-        # TODO (Tom Tang): Modify this testcase once we support ES2020-style dynamic import
-        # pm.eval("import('some_module')") # dynamic import returns a Promise, see https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/import
-        with pytest.raises(pm.SpiderMonkeyError, match="\nError: Dynamic module import is disabled or not supported in this context"):
-            await pm.eval("import('some_module')")
-        # TODO (Tom Tang): properly test unhandled rejection
-
-        # await scheduled jobs on the Python event-loop
-        js_sleep = pm.eval("(seconds) => new Promise((resolve) => setTimeout(resolve, seconds*1000))")
-        def py_sleep(seconds): # asyncio.sleep has issues on Python 3.8
-            loop = asyncio.get_running_loop()
-            future = loop.create_future()
-            loop.call_later(seconds, lambda:future.set_result(None))
-            return future
-        both_sleep = pm.eval("(js_sleep, py_sleep) => async (seconds) => { await js_sleep(seconds); await py_sleep(seconds) }")(js_sleep, py_sleep)
-        await asyncio.wait_for(both_sleep(0.1), timeout=0.3) # won't be precisely 0.2s 
-        with pytest.raises(asyncio.exceptions.TimeoutError):
-            await asyncio.wait_for(both_sleep(0.1), timeout=0.19)
-
-        # making sure the async_fn is run
-        return True
-    assert asyncio.run(async_fn())
-
-    # should throw a RuntimeError if created outside a coroutine (the event-loop has ended)
-    with pytest.raises(RuntimeError, match="PythonMonkey cannot find a running Python event-loop to make asynchronous calls."):
-        pm.eval("new Promise(() => { })")
+  # should throw RuntimeError if Promises are created outside a coroutine
+  create_promise = pm.eval("() => Promise.resolve(1)")
+  with pytest.raises(RuntimeError,
+                     match="PythonMonkey cannot find a running Python event-loop to make asynchronous calls."):
+    create_promise()
+
+  async def async_fn():
+    create_promise()  # inside a coroutine, no error
+
+    # Python awaitables to JS Promise coercion
+    # 1. Python asyncio.Future to JS promise
+    loop = asyncio.get_running_loop()
+    f0 = loop.create_future()
+    f0.set_result(2561)
+
+    assert type(f0) is asyncio.Future
+    assert 2561 == await f0
+    assert pm.eval("(p) => p instanceof Promise")(f0) is True
+    assert 2561 == await pm.eval("(p) => p")(f0)
+    del f0
+
+    # 2. Python asyncio.Task to JS promise
+    async def coro_fn(x):
+      await asyncio.sleep(0.01)
+      return x
+    task = loop.create_task(coro_fn("from a Task"))
+    assert type(task) is asyncio.Task
+    assert type(task) is not asyncio.Future
+    assert isinstance(task, asyncio.Future)
+    assert "from a Task" == await task
+    assert pm.eval("(p) => p instanceof Promise")(task) is True
+    assert "from a Task" == await pm.eval("(p) => p")(task)
+    del task
+
+    # 3. Python coroutine to JS promise
+    coro = coro_fn("from a Coroutine")
+    assert asyncio.iscoroutine(coro)
+    # assert "a Coroutine" == await coro                   # coroutines cannot be awaited more than once
+    # assert pm.eval("(p) => p instanceof Promise")(coro)  # RuntimeError: cannot reuse already awaited coroutine
+    assert "from a Coroutine" == await pm.eval("(p) => (p instanceof Promise) && p")(coro)
+    del coro
+
+    # JS Promise to Python awaitable coercion
+    assert 100 == await pm.eval("new Promise((r)=>{ r(100) })")
+    assert 10010 == await pm.eval("Promise.resolve(10010)")
+    with pytest.raises(pm.SpiderMonkeyError, match="^TypeError: (.|\\n)+ is not a constructor$"):
+      await pm.eval("Promise.resolve")(10086)
+    assert 10086 == await pm.eval("Promise.resolve.bind(Promise)")(10086)
+
+    assert "promise returning a function" == (await pm.eval("""
+                                                              Promise.resolve(() => {
+                                                                return 'promise returning a function';
+                                                              });
+                                                            """))()
+    assert "function 2" == (await pm.eval("Promise.resolve(x=>x)"))("function 2")
+
+    def aaa(n):
+      return n
+    ident0 = await (pm.eval("Promise.resolve.bind(Promise)")(aaa))
+    assert "from aaa" == ident0("from aaa")
+    ident1 = await pm.eval("async (aaa) => x=>aaa(x)")(aaa)
+    assert "from ident1" == ident1("from ident1")
+    ident2 = await pm.eval("() => Promise.resolve(x=>x)")()
+    assert "from ident2" == ident2("from ident2")
+    ident3 = await pm.eval("(aaa) => Promise.resolve(x=>aaa(x))")(aaa)
+    assert "from ident3" == ident3("from ident3")
+    del aaa
+
+    # promise returning a JS Promise<Function> that calls a Python function inside
+    def fn0(n):
+      return n + 100
+
+    def fn1():
+      return pm.eval("async x=>x")(fn0)
+    fn2 = await pm.eval("async (fn1) => { const fn0 = await fn1(); return Promise.resolve(x=>fn0(x)) }")(fn1)
+    assert 101.2 == fn2(1.2)
+    fn3 = await pm.eval("""
+      async (fn1) => {
+        const fn0 = await fn1();
+        return Promise.resolve(async x => { return fn0(x); });
+      }
+    """)(fn1)
+    assert 101.3 == await fn3(1.3)
+    fn4 = await pm.eval("""
+      async (fn1) => {
+        return Promise.resolve(async x => {
+          const fn0 = await fn1();
+          return fn0(x);
+        });
+      }
+    """)(fn1)
+    assert 101.4 == await fn4(1.4)
+
+    # chained JS promises
+    assert "chained" == await pm.eval("""
+                          async () => new Promise((resolve) => resolve( Promise.resolve().then(()=>'chained') ))
+                        """)()
+
+    # chained Python awaitables
+    async def a():
+      await asyncio.sleep(0.01)
+      return "nested"
+
+    async def b():
+      await asyncio.sleep(0.01)
+      return a()
+
+    async def c():
+      await asyncio.sleep(0.01)
+      return b()
+    # JS `await` supports chaining. However, on Python-land, it actually requires `await (await (await c()))`
+    assert "nested" == await pm.eval("async (promise) => await promise")(c())
+    assert "nested" == await pm.eval("async (promise) => await promise")(await c())
+    assert "nested" == await pm.eval("async (promise) => await promise")(await (await c()))
+    assert "nested" == await pm.eval("async (promise) => await promise")(await (await (await c())))
+    assert "nested" == await pm.eval("async (promise) => promise")(c())
+    assert "nested" == await pm.eval("async (promise) => promise")(await c())
+    assert "nested" == await pm.eval("async (promise) => promise")(await (await c()))
+    assert "nested" == await pm.eval("async (promise) => promise")(await (await (await c())))
+    assert "nested" == await pm.eval("(promise) => Promise.resolve(promise)")(c())
+    assert "nested" == await pm.eval("(promise) => Promise.resolve(promise)")(await c())
+    assert "nested" == await pm.eval("(promise) => Promise.resolve(promise)")(await (await c()))
+    assert "nested" == await pm.eval("(promise) => Promise.resolve(promise)")(await (await (await c())))
+    assert "nested" == await pm.eval("(promise) => promise")(c())
+    assert "nested" == await pm.eval("(promise) => promise")(await c())
+    assert "nested" == await pm.eval("(promise) => promise")(await (await c()))
+    with pytest.raises(TypeError, match="object str can't be used in 'await' expression"):
+      await pm.eval("(promise) => promise")(await (await (await c())))
+
+    # Python awaitable throwing exceptions
+    async def coro_to_throw0():
+      await asyncio.sleep(0.01)
+      print([].non_exist)  # type: ignore
+    with pytest.raises(pm.SpiderMonkeyError, match="Python AttributeError: 'list' object has no attribute 'non_exist'"):
+      await (pm.eval("(promise) => promise")(coro_to_throw0()))
+    with pytest.raises(pm.SpiderMonkeyError, match="Python AttributeError: 'list' object has no attribute 'non_exist'"):
+      await (pm.eval("async (promise) => promise")(coro_to_throw0()))
+    with pytest.raises(pm.SpiderMonkeyError, match="Python AttributeError: 'list' object has no attribute 'non_exist'"):
+      await (pm.eval("(promise) => Promise.resolve().then(async () => await promise)")(coro_to_throw0()))
+
+    async def coro_to_throw1():
+      await asyncio.sleep(0.01)
+      raise TypeError("reason")
+    with pytest.raises(pm.SpiderMonkeyError, match="Python TypeError: reason"):
+      await (pm.eval("(promise) => promise")(coro_to_throw1()))
+    assert 'rejected <Python TypeError: reason>' == await pm.eval("""
+                                                                  (promise) => promise.then(
+                                                                    ()=>{},
+                                                                    (err)=>`rejected <${err.message}>`
+                                                                  )
+                                                                  """)(coro_to_throw1())
+
+    # JS Promise throwing exceptions
+    with pytest.raises(pm.SpiderMonkeyError, match="nan"):
+      await pm.eval("Promise.reject(NaN)")  # JS can throw anything
+    with pytest.raises(pm.SpiderMonkeyError, match="123.0"):
+      await (pm.eval("async () => { throw 123 }")())
+      # await (pm.eval("async () => { throw {} }")())
+    with pytest.raises(pm.SpiderMonkeyError, match="anything"):
+      await pm.eval("Promise.resolve().then(()=>{ throw 'anything' })")
+      # FIXME (Tom Tang): We currently handle Promise exceptions by converting the object thrown to a Python Exception
+      # object through `pyTypeFactory
+      #               <objects of this type are not handled by PythonMonkey yet>
+      # await pm.eval("Promise.resolve().then(()=>{ throw {a:1,toString(){return'anything'}} })")
+    # not going through the conversion
+    with pytest.raises(pm.SpiderMonkeyError, match="on line 1, column 31:\nTypeError: undefined has no properties"):
+      await pm.eval("Promise.resolve().then(()=>{ (undefined).prop })")
+
+    # TODO (Tom Tang): Modify this testcase once we support ES2020-style dynamic import
+    # pm.eval("import('some_module')") # dynamic import returns a Promise, see
+    # https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/import
+    with pytest.raises(pm.SpiderMonkeyError,
+                       match="\nError: Dynamic module import is disabled or not supported in this context"):
+      await pm.eval("import('some_module')")
+    # TODO (Tom Tang): properly test unhandled rejection
+
+    # await scheduled jobs on the Python event-loop
+    js_sleep = pm.eval("(seconds) => new Promise((resolve) => setTimeout(resolve, seconds*1000))")
+
+    def py_sleep(seconds):  # asyncio.sleep has issues on Python 3.8
+      loop = asyncio.get_running_loop()
+      future = loop.create_future()
+      loop.call_later(seconds, lambda: future.set_result(None))
+      return future
+    both_sleep = pm.eval("""
+      (js_sleep, py_sleep) => async (seconds) => {
+        await js_sleep(seconds);
+        await py_sleep(seconds);
+      }
+    """)(js_sleep, py_sleep)
+    await asyncio.wait_for(both_sleep(0.1), timeout=0.3)  # won't be precisely 0.2s
+    with pytest.raises(asyncio.exceptions.TimeoutError):
+      await asyncio.wait_for(both_sleep(0.1), timeout=0.19)
+
+    # making sure the async_fn is run
+    return True
+  assert asyncio.run(async_fn())
+
+  # should throw a RuntimeError if created outside a coroutine (the event-loop has ended)
+  with pytest.raises(RuntimeError,
+                     match="PythonMonkey cannot find a running Python event-loop to make asynchronous calls."):
+    pm.eval("new Promise(() => { })")
 
 # off-thread promises
+
+
 def test_webassembly():
-    async def async_fn():
-        # off-thread promises can run
-        assert 'instantiated' == await pm.eval("""
+  async def async_fn():
+    # off-thread promises can run
+    assert 'instantiated' == await pm.eval("""
         // https://github.com/mdn/webassembly-examples/blob/main/js-api-examples/simple.wasm
         var code = new Uint8Array([
             0,  97, 115, 109,   1,   0,   0,   0,   1,   8,   2,  96,
             1, 127,   0,  96,   0,   0,   2,  25,   1,   7, 105, 109,
         112, 111, 114, 116, 115,  13, 105, 109, 112, 111, 114, 116,
         101, 100,  95, 102, 117, 110,  99,   0,   0,   3,   2,   1,
             1,   7,  17,   1,  13, 101, 120, 112, 111, 114, 116, 101,
         100,  95, 102, 117, 110,  99,   0,   1,  10,   8,   1,   6,
             0,  65,  42,  16,   0,  11
         ]);
 
         WebAssembly.instantiate(code, { imports: { imported_func() {} } }).then(() => 'instantiated')
         """)
 
-        # making sure the async_fn is run
-        return True
-    assert asyncio.run(async_fn())
+    # making sure the async_fn is run
+    return True
+  assert asyncio.run(async_fn())
```

### Comparing `pythonmonkey-0.4.0/tests/python/test_functions_this.py` & `pythonmonkey-0.6.0/tests/python/test_functions_this.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 import pythonmonkey as pm
 import subprocess
 import weakref
 import sys
 
+
 def test_python_functions_self():
   def pyFunc(param):
     return param
-  
+
   assert 1 == pyFunc(1)
   assert 2 == pm.eval("""(pyFunc) => {
     return pyFunc(2);
   }
   """)(pyFunc)
   assert 3 == pm.eval("""(pyFunc) => {
     let jsObj = {};
     jsObj.pyFunc = pyFunc;
     return pyFunc(3);
   }
   """)(pyFunc)
 
+
 def test_python_methods_self():
   def pyFunc(self, param):
     return [self, param]
 
   class Class:
     pass
   Class.pyMethod = pyFunc
@@ -40,33 +42,34 @@
   assert pyObj == result[0] and 3 == result[1]
   result = pm.eval("""(pyObj) => {
     let jsObj = {};
     jsObj.pyMethod = pyObj.pyMethod;
     return jsObj.pyMethod(4);
   }
   """)(pyObj)
-  assert pyObj == result[0] and 4 == result[1] #pyMethod is bound to pyObj, so `self` is not `jsObj`
+  assert pyObj == result[0] and 4 == result[1]  # pyMethod is bound to pyObj, so `self` is not `jsObj`
   result = pm.eval("""(pyObj) => {
     let pyMethod = pyObj.pyMethod;
     return pyMethod(5);
   }
   """)(pyObj)
-  assert pyObj == result[0] and 5 == result[1] #pyMethod is bound to pyObj, so `self` is not `globalThis`
+  assert pyObj == result[0] and 5 == result[1]  # pyMethod is bound to pyObj, so `self` is not `globalThis`
+
 
 def test_javascript_functions_this():
   jsFunc = pm.eval("""
   (function(param) {
     return [this, param];
   })
   """)
 
   class Class:
     pass
-  Class.jsFunc = jsFunc # jsFunc is not bound to Class, so `this` will be `globalThis`, not the object
-  
+  Class.jsFunc = jsFunc  # jsFunc is not bound to Class, so `this` will be `globalThis`, not the object
+
   pyObj = Class()
   jsObj = pm.eval("({})")
   jsObj.jsFunc = jsFunc
   globalThis = pm.eval("globalThis")
   result = jsFunc(1)
   assert globalThis == result[0] and 1 == result[1]
   result = pyObj.jsFunc(2)
@@ -85,26 +88,27 @@
   assert pyObj == result[0] and 5 == result[1]
   result = pm.eval("""(jsObj) => {
     return jsObj.jsFunc(6);
   }
   """)(jsObj)
   assert jsObj == result[0] and 6 == result[1]
 
+
 def test_JSMethodProxy_this():
   jsFunc = pm.eval("""
   (function(param) {
     return [this, param];
   })
   """)
 
   class Class:
     pass
-  
+
   pyObj = Class()
-  pyObj.jsMethod = pm.JSMethodProxy(jsFunc, pyObj) # jsMethod is bound to pyObj, so `this` will always be `pyObj`
+  pyObj.jsMethod = pm.JSMethodProxy(jsFunc, pyObj)  # jsMethod is bound to pyObj, so `this` will always be `pyObj`
   jsObj = pm.eval("({})")
   jsObj.jsMethod = pyObj.jsMethod
   globalThis = pm.eval("globalThis")
   result = pyObj.jsMethod(1)
   assert pyObj == result[0] and 1 == result[1]
   result = jsObj.jsMethod(2)
   assert pyObj == result[0] and 2 == result[1]
@@ -115,21 +119,24 @@
   assert pyObj == result[0] and 3 == result[1]
   result = pm.eval("""(jsObj) => {
     return jsObj.jsMethod(4);
   }
   """)(jsObj)
   assert pyObj == result[0] and 4 == result[1]
 
-#require
+# require
+
+
 def test_require_correct_this():
-    subprocess.check_call('npm install crypto-js', shell=True)
-    CryptoJS = pm.require('crypto-js')
-    cipher = CryptoJS.SHA256("Hello, World!").toString()
-    assert cipher == "dffd6021bb2bd5b0af676290809ec3a53191dd81c7f70a4b28688a362182986f"
-    subprocess.check_call('npm uninstall crypto-js', shell=True)
+  subprocess.check_call('npm install crypto-js', shell=True)
+  CryptoJS = pm.require('crypto-js')
+  cipher = CryptoJS.SHA256("Hello, World!").toString()
+  assert cipher == "dffd6021bb2bd5b0af676290809ec3a53191dd81c7f70a4b28688a362182986f"
+  subprocess.check_call('npm uninstall crypto-js', shell=True)
+
 
 def test_require_correct_this_old_style_class():
   example = pm.eval("""
   () => {
     // old style class
     function Rectangle(w, h) {
       this.w = w;
@@ -160,37 +167,38 @@
         return this.w * this.h;
       }
     }
 
     return { Rectangle: Rectangle, Rectangle2: Rectangle2};
   }
   """)()
-  r = pm.new(example.Rectangle)(1,2)
+  r = pm.new(example.Rectangle)(1, 2)
 
   assert r.getArea() == 2
   assert r.getThis() == r
 
-  r2 = pm.new(example.Rectangle2)(1,2)
+  r2 = pm.new(example.Rectangle2)(1, 2)
 
   assert r2.getArea() == 2
   assert r2.getThis() == r2
 
+
 def test_function_finalization():
   ref = []
   starting_ref_count = []
 
   def outerScope():
     def pyFunc():
       return 42
-    
+
     ref.append(weakref.ref(pyFunc))
     starting_ref_count.append(sys.getrefcount(pyFunc))
     assert 42 == pm.eval("(func) => func()")(pyFunc)
 
     assert ref[0]() is pyFunc
     current_ref_count = sys.getrefcount(pyFunc)
     assert current_ref_count == starting_ref_count[0] + 1
 
   outerScope()
-  pm.collect() # this should collect the JS proxy to pyFunc, which should decref pyFunc
-  #pyFunc should be collected by now
-  assert ref[0]() is None
+  pm.collect()  # this should collect the JS proxy to pyFunc, which should decref pyFunc
+  # pyFunc should be collected by now
+  assert ref[0]() is None
```

### Comparing `pythonmonkey-0.4.0/tests/python/test_list_array.py` & `pythonmonkey-0.6.0/tests/python/test_list_array.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,47 @@
 import pythonmonkey as pm
 
+
 def test_eval_array_is_list():
-    pythonList = pm.eval('[]')
-    assert isinstance(pythonList, list) 
+  pythonList = pm.eval('[]')
+  assert isinstance(pythonList, list)
 
 # extra nice but not necessary
+
+
 def test_eval_array_is_list_type_string():
-    pythonListTypeString = str(type(pm.eval('[]')))
-    assert pythonListTypeString == "<class 'list'>"
+  pythonListTypeString = str(type(pm.eval('[]')))
+  assert pythonListTypeString == "<class 'list'>"
+
 
 def test_eval_list_is_array():
-    items = [1, 2, 3]
-    isArray = pm.eval('Array.isArray')(items)
-    assert isArray == True
+  items = [1, 2, 3]
+  isArray = pm.eval('Array.isArray')(items)
+  assert isArray
+
 
 def test_typeof_array():
-    items = [1, 2, 3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = typeof arr}")(result, items)
-    assert result[0] == 'object' 
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = typeof arr}")(result, items)
+  assert result[0] == 'object'
+
 
 def test_instanceof_array():
-    items = [1, 2, 3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr instanceof Array}")(result, items)
-    assert result[0] == True   
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr instanceof Array}")(result, items)
+  assert result[0]
+
 
 def test_instanceof_object():
-    items = [1, 2, 3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr instanceof Object}")(result, items)
-    assert result[0] == True       
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr instanceof Object}")(result, items)
+  assert result[0]
+
 
 def test_not_instanceof_string():
-    items = [1, 2, 3]
-    result = [None]
-    pm.eval("(result, arr) => {result[0] = arr instanceof String}")(result, items)
-    assert result[0] == False           
+  items = [1, 2, 3]
+  result = [None]
+  pm.eval("(result, arr) => {result[0] = arr instanceof String}")(result, items)
+  assert not result[0]
```

### Comparing `pythonmonkey-0.4.0/tests/python/test_lists.py` & `pythonmonkey-0.6.0/tests/python/test_lists.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,1058 +1,1246 @@
 import pythonmonkey as pm
-from functools import reduce 
+from functools import reduce
+
 
 def test_eval_lists():
-    d = [1]
-    proxy_d = pm.eval("(list) => { return list; }")(d)
-    assert d is proxy_d
+  d = [1]
+  proxy_d = pm.eval("(list) => { return list; }")(d)
+  assert d is proxy_d
+
 
 def test_equal_lists_left_literal_right():
-    pyArray = pm.eval("Array(1,2)")
-    assert pyArray == [1,2]
+  pyArray = pm.eval("Array(1,2)")
+  assert pyArray == [1, 2]
+
 
 def test_equal_no_object_lists_left_literal_right():
-    pyArray = pm.eval("[1,2]")
-    assert pyArray == [1,2]    
+  pyArray = pm.eval("[1,2]")
+  assert pyArray == [1, 2]
+
 
 def test_equal_lists_right_literal_left():
-    pyArray = pm.eval("Array(1,2)")
-    assert [1,2] == pyArray
+  pyArray = pm.eval("Array(1,2)")
+  assert [1, 2] == pyArray
+
 
 def test_equal_lists_left_list_right():
-    pyArray = pm.eval("Array(1,2)")
-    b = [1,2]
-    assert pyArray == b
+  pyArray = pm.eval("Array(1,2)")
+  b = [1, 2]
+  assert pyArray == b
+
 
 def test_equal_lists_right_literal_left():
-    pyArray = pm.eval("Array(1,2)")
-    b = [1,2]
-    assert b == pyArray
+  pyArray = pm.eval("Array(1,2)")
+  b = [1, 2]
+  assert b == pyArray
+
 
 def test_not_equal_lists_left_literal_right():
-    pyArray = pm.eval("Array(1,2)")
-    assert pyArray != [1,3]  
+  pyArray = pm.eval("Array(1,2)")
+  assert pyArray != [1, 3]
+
 
 def test_smaller_lists_left_literal_right():
-    pyArray = pm.eval("Array(1,2)")
-    assert pyArray < [1,3]  
+  pyArray = pm.eval("Array(1,2)")
+  assert pyArray < [1, 3]
+
 
 def test_equal_sublist():
-    pyArray = pm.eval("Array(1,2,[3,4])")
-    assert pyArray == [1,2,[3,4]]
+  pyArray = pm.eval("Array(1,2,[3,4])")
+  assert pyArray == [1, 2, [3, 4]]
+
 
 def test_not_equal_sublist_right_not_sublist():
-    pyArray = pm.eval("Array(1,2,[3,4])")
-    assert pyArray != [1,2,3,4]  
+  pyArray = pm.eval("Array(1,2,[3,4])")
+  assert pyArray != [1, 2, 3, 4]
+
 
 def test_equal_self():
-    a = pm.eval("([1,2,3,4])")
-    b = a
-    assert b == a 
+  a = pm.eval("([1,2,3,4])")
+  b = a
+  assert b == a
+
 
 def test_equal_other_instance():
-    a = pm.eval("([1,2,3,4])")
-    b = [1,2,3,4]
-    assert b == a   
+  a = pm.eval("([1,2,3,4])")
+  b = [1, 2, 3, 4]
+  assert b == a
+
 
 def test_not_equal_size():
-    a = pm.eval("([1,2,3,4])")
-    b = [1,2]
-    assert b != a  
+  a = pm.eval("([1,2,3,4])")
+  b = [1, 2]
+  assert b != a
+
 
 def test_equal_other_js_instance():
-    a = pm.eval("([1,2,3,4])")
-    b = pm.eval("([1,2,3,4])")
-    assert b == a  
+  a = pm.eval("([1,2,3,4])")
+  b = pm.eval("([1,2,3,4])")
+  assert b == a
+
 
 def test_not_equal_other_js_instance():
-    a = pm.eval("([1,2,3,4])")
-    b = pm.eval("([1,2,4,3])")
-    assert b != a          
+  a = pm.eval("([1,2,3,4])")
+  b = pm.eval("([1,2,4,3])")
+  assert b != a
+
 
 def test_not_smaller_self():
-    a = pm.eval("([1,2,3,4])")
-    b = a
-    assert not(b < a)   
+  a = pm.eval("([1,2,3,4])")
+  b = a
+  assert not (b < a)
+
 
 def test_not_smaller_equal_self():
-    a = pm.eval("([1,2,3,4])")
-    b = a
-    assert b <= a          
+  a = pm.eval("([1,2,3,4])")
+  b = a
+  assert b <= a
+
 
 def test_eval_arrays_proxy_get():
-    f = pm.eval("(arr) => { return arr[0]}")
-    assert f([1,2]) == 1.0
+  f = pm.eval("(arr) => { return arr[0]}")
+  assert f([1, 2]) == 1.0
+
 
 def test_eval_arrays_proxy_set():
-    f = pm.eval("(arr) => { arr[0] = 42.0; return;}")
-    pyObj = [1]
-    f(pyObj)
-    assert pyObj[0] == 42.0
+  f = pm.eval("(arr) => { arr[0] = 42.0; return;}")
+  pyObj = [1]
+  f(pyObj)
+  assert pyObj[0] == 42.0
+
+# get
+
 
-#get
 def test_get():
-    pyArray = pm.eval("[1,2]")
-    assert pyArray[0] == 1   
+  pyArray = pm.eval("[1,2]")
+  assert pyArray[0] == 1
+
 
 def test_get_negative_index():
-    pyArray = pm.eval("[1,2]")
-    assert pyArray[-1] == 2    
+  pyArray = pm.eval("[1,2]")
+  assert pyArray[-1] == 2
+
 
 def test_get_index_out_of_range():
-    pyArray = pm.eval("[1,2]")
-    try:
-        pyArray[3]          
-        assert (False)
-    except Exception as e:    
-        assert str(type(e)) == "<class 'IndexError'>"
-        assert str(e) == 'list index out of range'       
+  pyArray = pm.eval("[1,2]")
+  try:
+    pyArray[3]
+    assert (False)
+  except Exception as e:
+    assert str(type(e)) == "<class 'IndexError'>"
+    assert str(e) == 'list index out of range'
+
 
 def test_get_index_wrong_type_str():
-    pyArray = pm.eval("[1,2]")
-    try:
-        pyArray["g"]          
-        assert (False)
-    except Exception as e:    
-        assert str(type(e)) == "<class 'TypeError'>"
-        assert str(e) == 'list indices must be integers or slices, not str'
+  pyArray = pm.eval("[1,2]")
+  try:
+    pyArray["g"]
+    assert (False)
+  except Exception as e:
+    assert str(type(e)) == "<class 'TypeError'>"
+    assert str(e) == 'list indices must be integers or slices, not str'
+
 
 def test_get_index_wrong_type_list():
-    pyArray = pm.eval("[1,2]")
-    try:
-        pyArray[[2]]          
-        assert (False)
-    except Exception as e:    
-        assert str(type(e)) == "<class 'TypeError'>"
-        assert str(e) == 'list indices must be integers or slices, not list'     
+  pyArray = pm.eval("[1,2]")
+  try:
+    pyArray[[2]]
+    assert (False)
+  except Exception as e:
+    assert str(type(e)) == "<class 'TypeError'>"
+    assert str(e) == 'list indices must be integers or slices, not list'
+
 
 def test_delete():
-    pyArray = pm.eval("[1,2]")
-    del pyArray[0]
-    assert pyArray == [None, 2]              
+  pyArray = pm.eval("[1,2]")
+  del pyArray[0]
+  assert pyArray == [None, 2]
 
 
-#assign
+# assign
 def test_assign():
-    pyArray = pm.eval("[1,2]")
-    pyArray[0] = 6
-    assert pyArray[0] == 6  
+  pyArray = pm.eval("[1,2]")
+  pyArray[0] = 6
+  assert pyArray[0] == 6
+
 
 def test_assign_negative_index():
-    pyArray = pm.eval("[1,2]")
-    pyArray[-1] = 6
-    assert pyArray[1] == 6     
+  pyArray = pm.eval("[1,2]")
+  pyArray[-1] = 6
+  assert pyArray[1] == 6
+
 
 def test_assign_index_out_of_range():
-    pyArray = pm.eval("[1,2]")
-    try:
-        pyArray[3] = 8          
-        assert (False)
-    except Exception as e:    
-        assert str(type(e)) == "<class 'IndexError'>"
-        assert str(e) == 'list assignment index out of range'     
+  pyArray = pm.eval("[1,2]")
+  try:
+    pyArray[3] = 8
+    assert (False)
+  except Exception as e:
+    assert str(type(e)) == "<class 'IndexError'>"
+    assert str(e) == 'list assignment index out of range'
+
 
 def test_assign_index_wrong_type_str():
-    pyArray = pm.eval("[1,2]")
-    try:
-        pyArray["g"] = 4         
-        assert (False)
-    except Exception as e:    
-        assert str(type(e)) == "<class 'TypeError'>"
-        assert str(e) == 'list indices must be integers or slices, not str'          
+  pyArray = pm.eval("[1,2]")
+  try:
+    pyArray["g"] = 4
+    assert (False)
+  except Exception as e:
+    assert str(type(e)) == "<class 'TypeError'>"
+    assert str(e) == 'list indices must be integers or slices, not str'
 
 
 def test_assign_index_wrong_type_list():
-    pyArray = pm.eval("[1,2]")
-    try:
-        pyArray[[2]] = 9          
-        assert (False)
-    except Exception as e:    
-        assert str(type(e)) == "<class 'TypeError'>"
-        assert str(e) == 'list indices must be integers or slices, not list'               
+  pyArray = pm.eval("[1,2]")
+  try:
+    pyArray[[2]] = 9
+    assert (False)
+  except Exception as e:
+    assert str(type(e)) == "<class 'TypeError'>"
+    assert str(e) == 'list indices must be integers or slices, not list'
 
 
-#repr
+# repr
 def test_repr_empty_array():
-    pyArray = pm.eval("[]")
-    expected = "[]"
-    assert repr(pyArray) == expected
-    assert str(pyArray) == expected 
+  pyArray = pm.eval("[]")
+  expected = "[]"
+  assert repr(pyArray) == expected
+  assert str(pyArray) == expected
+
 
 def test_repr_non_empty_array():
-    pyArray = pm.eval("[1,2]")
-    expected = "[1.0, 2.0]"
-    assert repr(pyArray) == expected
-    assert str(pyArray) == expected 
+  pyArray = pm.eval("[1,2]")
+  expected = "[1.0, 2.0]"
+  assert repr(pyArray) == expected
+  assert str(pyArray) == expected
+
 
 def test_repr_recursion():
-    pyArray = pm.eval("""
+  pyArray = pm.eval("""
     () => {
         let arr = [1,2];
         arr.push(arr);
         return arr;
     }
     """)()
-    expected = "[1.0, 2.0, [...]]"
-    assert repr(pyArray) == expected
-    assert str(pyArray) == expected    
+  expected = "[1.0, 2.0, [...]]"
+  assert repr(pyArray) == expected
+  assert str(pyArray) == expected
+
+# concat
+
 
-#concat
 def test_concat_wrong_type():
-    likes = pm.eval('([1,2])')
-    try:
-        likes + 3          
-        assert (False)
-    except Exception as e:    
-        assert str(type(e)) == "<class 'TypeError'>"
-        assert str(e) == 'can only concatenate list (not "int") to list'      
+  likes = pm.eval('([1,2])')
+  try:
+    likes + 3
+    assert (False)
+  except Exception as e:
+    assert str(type(e)) == "<class 'TypeError'>"
+    assert str(e) == 'can only concatenate list (not "int") to list'
+
 
 def test_concat_empty_empty():
-    pyArray = pm.eval("[]")
-    pyArray + []
-    assert pyArray == []
+  pyArray = pm.eval("[]")
+  pyArray + []
+  assert pyArray == []
+
 
 def test_concat_not_empty_empty():
-    pyArray = pm.eval("[1,2]")
-    pyArray + []
-    assert pyArray == [1,2]
+  pyArray = pm.eval("[1,2]")
+  pyArray + []
+  assert pyArray == [1, 2]
+
 
 def test_concat_not_in_place():
-    pyArray = pm.eval("[1,2]")
-    b = pyArray + [3,4]
-    assert pyArray == [1,2]
+  pyArray = pm.eval("[1,2]")
+  b = pyArray + [3, 4]
+  assert pyArray == [1, 2]
 
 # TODO
-#def test_concat_array_right():
+# def test_concat_array_right():
 #    pyArray = pm.eval("[1,2]")
 #    b = [3,4] + pyArray
 #    assert b == [1,2,3,4]
 
+
 def test_concat_pm_array_right():
-    a = pm.eval("[1,2]")
-    b = pm.eval("[3,4]")
-    c = a + b
-    assert c == [1,2,3,4]
+  a = pm.eval("[1,2]")
+  b = pm.eval("[3,4]")
+  c = a + b
+  assert c == [1, 2, 3, 4]
+
+# repeat
+
 
-#repeat
 def test_repeat_negative():
-    a = pm.eval("[1,2]")
-    b = a * -1
-    assert b == []
+  a = pm.eval("[1,2]")
+  b = a * -1
+  assert b == []
+
 
 def test_repeat_zero():
-    a = pm.eval("[1,2]")
-    b = a * 0
-    assert b == []    
+  a = pm.eval("[1,2]")
+  b = a * 0
+  assert b == []
+
 
 def test_repeat_once():
-    a = pm.eval("[1,2]")
-    b = a * 1
-    assert b == [1,2]  
-    assert a is not b  
+  a = pm.eval("[1,2]")
+  b = a * 1
+  assert b == [1, 2]
+  assert a is not b
+
 
 def test_repeat_twice():
-    a = pm.eval("[1,2]")
-    b = a * 2
-    assert b == [1,2,1,2]    
+  a = pm.eval("[1,2]")
+  b = a * 2
+  assert b == [1, 2, 1, 2]
+
 
 def test_repeat_wrong_type():
-    a = pm.eval('([1,2])')
-    try:
-        a * 1.0         
-        assert (False)
-    except Exception as e:    
-        assert str(type(e)) == "<class 'TypeError'>"
-        assert str(e) == "can't multiply sequence by non-int of type 'float'"       
+  a = pm.eval('([1,2])')
+  try:
+    a * 1.0
+    assert (False)
+  except Exception as e:
+    assert str(type(e)) == "<class 'TypeError'>"
+    assert str(e) == "can't multiply sequence by non-int of type 'float'"
+
 
 def test_repeat_not_in_place():
-    a = pm.eval("[1,2]")
-    b = a * 3
-    assert b == [1.0, 2.0, 1.0, 2.0, 1.0, 2.0]
-    assert a == [1,2]
+  a = pm.eval("[1,2]")
+  b = a * 3
+  assert b == [1.0, 2.0, 1.0, 2.0, 1.0, 2.0]
+  assert a == [1, 2]
+
+# contains
+
 
-#contains
 def test_contains_found():
-    a = pm.eval("[1,2]")
-    assert 1 in a
+  a = pm.eval("[1,2]")
+  assert 1 in a
+
 
 def test_contains_not_found():
-    a = pm.eval("[1,2]")
-    assert 7 not in a    
+  a = pm.eval("[1,2]")
+  assert 7 not in a
+
 
 def test_contains_not_found_odd_type():
-    a = pm.eval("[1,2]")
-    assert [1] not in a    
+  a = pm.eval("[1,2]")
+  assert [1] not in a
+
+# concat in place  +=
+
 
-#concat in place  +=
 def test_concat_is_inplace():
-    pyArray = pm.eval("[1,2]")
-    pyArray += [3]
-    assert pyArray == [1,2,3]
+  pyArray = pm.eval("[1,2]")
+  pyArray += [3]
+  assert pyArray == [1, 2, 3]
+
 
 def test_concat_in_place_empty_empty():
-    pyArray = pm.eval("[]")
-    pyArray += []
-    assert pyArray == []
+  pyArray = pm.eval("[]")
+  pyArray += []
+  assert pyArray == []
+
 
 def test_concat_not_empty_empty():
-    pyArray = pm.eval("[1,2]")
-    pyArray += []
-    assert pyArray == [1,2]     
+  pyArray = pm.eval("[1,2]")
+  pyArray += []
+  assert pyArray == [1, 2]
+
+# repeat in place  *=
+
 
-#repeat in place  *=
 def test_repeat_is_in_place():
-    a = pm.eval("[1,2]")
-    a *= 3
-    assert a == [1,2,1,2,1,2]
+  a = pm.eval("[1,2]")
+  a *= 3
+  assert a == [1, 2, 1, 2, 1, 2]
+
 
 def test_repeat_negative():
-    a = pm.eval("[1,2]")
-    a *= -1
-    assert a == []
+  a = pm.eval("[1,2]")
+  a *= -1
+  assert a == []
+
 
 def test_repeat_zero():
-    a = pm.eval("[1,2]")
-    a *= 0
-    assert a == []
+  a = pm.eval("[1,2]")
+  a *= 0
+  assert a == []
+
 
 def test_repeat_twice():
-    a = pm.eval("[1,2]")
-    a *= 2
-    assert a == [1,2,1,2]    
+  a = pm.eval("[1,2]")
+  a *= 2
+  assert a == [1, 2, 1, 2]
+
 
 def test_repeat_wrong_type():
-    a = pm.eval('([1,2])')
-    try:
-        a *= 1.7         
-        assert (False)
-    except Exception as e:    
-        assert str(type(e)) == "<class 'TypeError'>"
-        assert str(e) == "can't multiply sequence by non-int of type 'float'"     
+  a = pm.eval('([1,2])')
+  try:
+    a *= 1.7
+    assert (False)
+  except Exception as e:
+    assert str(type(e)) == "<class 'TypeError'>"
+    assert str(e) == "can't multiply sequence by non-int of type 'float'"
 
 
-#clear
+# clear
 def test_clear():
-    a = pm.eval("[1,2]")
-    a.clear()
-    assert a == []
+  a = pm.eval("[1,2]")
+  a.clear()
+  assert a == []
+
 
 def test_clear_with_arg():
-    a = pm.eval('([1,2])')
-    try:
-        a.clear(8)         
-        assert (False)
-    except Exception as e:    
-        assert str(type(e)) == "<class 'TypeError'>"
-        assert str(e).__contains__('clear() takes no arguments (1 given)')         
+  a = pm.eval('([1,2])')
+  try:
+    a.clear(8)
+    assert (False)
+  except Exception as e:
+    assert str(type(e)) == "<class 'TypeError'>"
+    assert str(e).__contains__('clear() takes no arguments (1 given)')
+
+# copy
+
 
-#copy
 def test_copy():
-    a = pm.eval("[1,2]")
-    b = a.copy()
-    b[0] = 8
-    assert a[0] == 1
-    assert b[0] == 8
+  a = pm.eval("[1,2]")
+  b = a.copy()
+  b[0] = 8
+  assert a[0] == 1
+  assert b[0] == 8
+
 
 def test_copy_with_arg():
-    a = pm.eval('([1,2])')
-    try:
-        b = a.copy(8)         
-        assert (False)
-    except Exception as e:    
-        assert str(type(e)) == "<class 'TypeError'>"
-        assert str(e).__contains__('copy() takes no arguments (1 given)')          
+  a = pm.eval('([1,2])')
+  try:
+    b = a.copy(8)
+    assert (False)
+  except Exception as e:
+    assert str(type(e)) == "<class 'TypeError'>"
+    assert str(e).__contains__('copy() takes no arguments (1 given)')
+
+# append
+
 
-#append
 def test_append():
-    a = pm.eval("[1,2]")
-    b = a.append(3)
-    assert a == [1,2,3]
-    assert b == None
+  a = pm.eval("[1,2]")
+  b = a.append(3)
+  assert a == [1, 2, 3]
+  assert b is None
+
+# insert
+
 
-#insert
 def test_insert_list():
-    a = pm.eval("[1,2]")
-    a.insert(0, [3,4])
-    assert a == [[3,4],1,2]
+  a = pm.eval("[1,2]")
+  a.insert(0, [3, 4])
+  assert a == [[3, 4], 1, 2]
+
 
 def test_insert_boolean():
-    a = pm.eval("[1,2]")
-    a.insert(0, True)
-    assert a == [True,1,2]
+  a = pm.eval("[1,2]")
+  a.insert(0, True)
+  assert a == [True, 1, 2]
+
 
 def test_insert_int():
-    a = pm.eval("[1,2]")
-    a.insert(0, 3)
-    assert a == [3,1,2]    
+  a = pm.eval("[1,2]")
+  a.insert(0, 3)
+  assert a == [3, 1, 2]
+
 
 def test_insert_float():
-    a = pm.eval("[1,2]")
-    a.insert(0, 4.5)
-    assert a == [4.5,1,2] 
+  a = pm.eval("[1,2]")
+  a.insert(0, 4.5)
+  assert a == [4.5, 1, 2]
+
 
 def test_insert_string():
-    a = pm.eval("[1,2]")
-    a.insert(0, "Hey")
-    assert a == ["Hey",1,2]     
+  a = pm.eval("[1,2]")
+  a.insert(0, "Hey")
+  assert a == ["Hey", 1, 2]
+
 
 def test_insert_none():
-    a = pm.eval("[1,2]")
-    a.insert(0, None)
-    assert a == [None,1,2]  
+  a = pm.eval("[1,2]")
+  a.insert(0, None)
+  assert a == [None, 1, 2]
+
 
 def test_insert_function():
-    def f():
-        return
-    a = pm.eval("[1,2]")
-    a.insert(0, f)
-    assert len(a) == 3    
+  def f():
+    return
+  a = pm.eval("[1,2]")
+  a.insert(0, f)
+  assert len(a) == 3
+
 
 def test_insert_int_neg_index():
-    a = pm.eval("[1,2]")
-    a.insert(-1, 3)
-    assert a == [1,3,2] 
+  a = pm.eval("[1,2]")
+  a.insert(-1, 3)
+  assert a == [1, 3, 2]
+
 
 def test_insert_int_too_large_index():
-    a = pm.eval("[1,2]")
-    a.insert(5, 3)
-    assert a == [1,2,3]  
+  a = pm.eval("[1,2]")
+  a.insert(5, 3)
+  assert a == [1, 2, 3]
+
 
 def test_insert_int_too_many_args():
-    a = pm.eval('([1,2])')
-    try:
-        a.insert(5,6,7)     
-        assert (False)
-    except Exception as e:    
-        assert str(type(e)) == "<class 'TypeError'>"
-        assert str(e) == "insert expected 2 arguments, got 3" 
+  a = pm.eval('([1,2])')
+  try:
+    a.insert(5, 6, 7)
+    assert (False)
+  except Exception as e:
+    assert str(type(e)) == "<class 'TypeError'>"
+    assert str(e) == "insert expected 2 arguments, got 3"
+
 
 def test_insert_int_too_few_args():
-    a = pm.eval('([1,2])')
-    try:
-        a.insert()     
-        assert (False)
-    except Exception as e:    
-        assert str(type(e)) == "<class 'TypeError'>"
-        assert str(e) == "insert expected 2 arguments, got 0"          
+  a = pm.eval('([1,2])')
+  try:
+    a.insert()
+    assert (False)
+  except Exception as e:
+    assert str(type(e)) == "<class 'TypeError'>"
+    assert str(e) == "insert expected 2 arguments, got 0"
 
 # extend
+
+
 def test_extend_with_list():
-    a = pm.eval("[1,2]")
-    a.extend([3,4])
-    assert a == [1,2,3,4]
+  a = pm.eval("[1,2]")
+  a.extend([3, 4])
+  assert a == [1, 2, 3, 4]
+
 
 def test_extend_with_dict_single():
-    a = pm.eval("[1,2]")
-    a.extend({'key':5})
-    assert a == [1,2,'key']
+  a = pm.eval("[1,2]")
+  a.extend({'key': 5})
+  assert a == [1, 2, 'key']
+
 
 def test_extend_with_dict_double():
-    a = pm.eval("[1,2]")
-    a.extend({'key':5, 'otherKey':6})
-    assert a == [1,2,'key','otherKey']    
+  a = pm.eval("[1,2]")
+  a.extend({'key': 5, 'otherKey': 6})
+  assert a == [1, 2, 'key', 'otherKey']
+
 
 def test_extend_with_number():
-    a = pm.eval('([1,2])')
-    try:
-        a.extend(3)     
-        assert (False)
-    except Exception as e:    
-        assert str(type(e)) == "<class 'TypeError'>"
-        assert str(e) == "'int' object is not iterable"    
+  a = pm.eval('([1,2])')
+  try:
+    a.extend(3)
+    assert (False)
+  except Exception as e:
+    assert str(type(e)) == "<class 'TypeError'>"
+    assert str(e) == "'int' object is not iterable"
+
 
 def test_extend_with_own_list():
-    a = pm.eval("[1,2]")
-    a.extend(a)
-    assert a == [1,2,1,2]
+  a = pm.eval("[1,2]")
+  a.extend(a)
+  assert a == [1, 2, 1, 2]
+
 
 def test_extend_with_pm_list():
-    a = pm.eval("[1,2]")
-    b = pm.eval("[3,4]")
-    a.extend(b)
-    assert a == [1,2,3,4]    
+  a = pm.eval("[1,2]")
+  b = pm.eval("[3,4]")
+  a.extend(b)
+  assert a == [1, 2, 3, 4]
 
 # TODO iterable dict
+
+
 def test_extend_with_own_dict():
-    a = pm.eval("[1,2]")
-    b = pm.eval("({'key':5, 'key2':6})")
-    a.extend(b)
-    assert a == [1,2,"key","key2"]
+  a = pm.eval("[1,2]")
+  b = pm.eval("({'key':5, 'key2':6})")
+  a.extend(b)
+  assert a == [1, 2, "key", "key2"]
+
+# pop
+
 
-#pop
 def test_pop_no_arg():
-    a = pm.eval("[1,2]")
-    b = a.pop()
-    assert a == [1]
-    assert b == 2
+  a = pm.eval("[1,2]")
+  b = a.pop()
+  assert a == [1]
+  assert b == 2
+
 
 def test_pop_empty_list():
-    a = pm.eval('([])')
-    try:
-        a.pop()     
-        assert (False)
-    except Exception as e:    
-        assert str(type(e)) == "<class 'IndexError'>"
-        assert str(e) == "pop from empty list"  
+  a = pm.eval('([])')
+  try:
+    a.pop()
+    assert (False)
+  except Exception as e:
+    assert str(type(e)) == "<class 'IndexError'>"
+    assert str(e) == "pop from empty list"
+
 
 def test_pop_list_no_arg():
-    a = pm.eval("[1,[2,3]]")
-    b = a.pop()
-    assert a == [1]
-    assert b == [2,3]    
+  a = pm.eval("[1,[2,3]]")
+  b = a.pop()
+  assert a == [1]
+  assert b == [2, 3]
+
 
 def test_pop_first_item():
-    a = pm.eval("[1,2]")
-    b = a.pop(0)
-    assert a == [2]
-    assert b == 1
+  a = pm.eval("[1,2]")
+  b = a.pop(0)
+  assert a == [2]
+  assert b == 1
+
 
 def test_pop_second_item():
-    a = pm.eval("[1,2]")
-    b = a.pop(1)
-    assert a == [1]
-    assert b == 2
+  a = pm.eval("[1,2]")
+  b = a.pop(1)
+  assert a == [1]
+  assert b == 2
+
 
 def test_pop_negative_item():
-    a = pm.eval("[1,2]")
-    b = a.pop(-1)
-    assert a == [1]
-    assert b == 2
+  a = pm.eval("[1,2]")
+  b = a.pop(-1)
+  assert a == [1]
+  assert b == 2
+
 
 def test_pop_out_of_bounds_item():
-    a = pm.eval('([1,2])')
-    try:
-        a.pop(3)     
-        assert (False)
-    except Exception as e:    
-        assert str(type(e)) == "<class 'IndexError'>"
-        assert str(e) == "pop index out of range"  
+  a = pm.eval('([1,2])')
+  try:
+    a.pop(3)
+    assert (False)
+  except Exception as e:
+    assert str(type(e)) == "<class 'IndexError'>"
+    assert str(e) == "pop index out of range"
+
+# remove
+
 
-#remove
 def test_remove_found_once():
-    a = pm.eval("[1,2]")
-    a.remove(1)
-    assert a == [2]
+  a = pm.eval("[1,2]")
+  a.remove(1)
+  assert a == [2]
+
 
 def test_remove_found_twice():
-    a = pm.eval("[1,2,1,2]")
-    a.remove(1)
-    assert a == [2,1,2]    
+  a = pm.eval("[1,2,1,2]")
+  a.remove(1)
+  assert a == [2, 1, 2]
+
 
 def test_remove_no_args():
-    a = pm.eval('([1,2])')
-    try:
-        a.remove()     
-        assert (False)
-    except Exception as e:    
-        assert str(type(e)) == "<class 'TypeError'>"
-        assert str(e).__contains__('remove() takes exactly one argument (0 given)')    
+  a = pm.eval('([1,2])')
+  try:
+    a.remove()
+    assert (False)
+  except Exception as e:
+    assert str(type(e)) == "<class 'TypeError'>"
+    assert str(e).__contains__('remove() takes exactly one argument (0 given)')
+
 
 def test_remove_not_found():
-    a = pm.eval('([1,2])')
-    try:
-        a.remove(3)     
-        assert (False)
-    except Exception as e:    
-        assert str(type(e)) == "<class 'ValueError'>"
-        assert str(e) == "list.remove(x): x not in list"        
+  a = pm.eval('([1,2])')
+  try:
+    a.remove(3)
+    assert (False)
+  except Exception as e:
+    assert str(type(e)) == "<class 'ValueError'>"
+    assert str(e) == "list.remove(x): x not in list"
+
+# index
+
 
-#index          
 def test_index_found():
-    a = pm.eval("[1,2,3,4]")
-    b = a.index(3)
-    assert b == 2  
+  a = pm.eval("[1,2,3,4]")
+  b = a.index(3)
+  assert b == 2
+
 
 def test_index_not_found():
-    a = pm.eval('([1,2])')
-    try:
-        a.index(3)     
-        assert (False)
-    except Exception as e:    
-        assert str(type(e)) == "<class 'ValueError'>"
-        assert str(e) == "3 is not in list"  
+  a = pm.eval('([1,2])')
+  try:
+    a.index(3)
+    assert (False)
+  except Exception as e:
+    assert str(type(e)) == "<class 'ValueError'>"
+    assert str(e) == "3 is not in list"
+
 
 def test_index_no_args():
-    a = pm.eval('([1,2,3,4])')
-    try:
-        a.index()     
-        assert (False)
-    except Exception as e:    
-        assert str(type(e)) == "<class 'TypeError'>"
-        assert str(e) == "index expected at least 1 argument, got 0"   
+  a = pm.eval('([1,2,3,4])')
+  try:
+    a.index()
+    assert (False)
+  except Exception as e:
+    assert str(type(e)) == "<class 'TypeError'>"
+    assert str(e) == "index expected at least 1 argument, got 0"
+
 
 def test_index_too_many_args():
-    a = pm.eval('([1,2,3,4])')
-    try:
-        a.index(2,3,4,5)     
-        assert (False)
-    except Exception as e:    
-        assert str(type(e)) == "<class 'TypeError'>"
-        assert str(e) == "index expected at most 3 arguments, got 4"   
+  a = pm.eval('([1,2,3,4])')
+  try:
+    a.index(2, 3, 4, 5)
+    assert (False)
+  except Exception as e:
+    assert str(type(e)) == "<class 'TypeError'>"
+    assert str(e) == "index expected at most 3 arguments, got 4"
+
 
 def test_index_found_with_start():
-    a = pm.eval("[1,2,3,4]")
-    b = a.index(3, 0)
-    assert b == 2  
+  a = pm.eval("[1,2,3,4]")
+  b = a.index(3, 0)
+  assert b == 2
+
 
 def test_index_found_with_negative_start():
-    a = pm.eval("[1,2,3,4]")
-    b = a.index(3, -3)
-    assert b == 2            
+  a = pm.eval("[1,2,3,4]")
+  b = a.index(3, -3)
+  assert b == 2
+
 
 def test_index_not_found_with_start():
-    a = pm.eval('([1,2,3,4])')
-    try:
-        a.index(3, 4)     
-        assert (False)
-    except Exception as e:    
-        assert str(type(e)) == "<class 'ValueError'>"
-        assert str(e) == "3 is not in list"     
+  a = pm.eval('([1,2,3,4])')
+  try:
+    a.index(3, 4)
+    assert (False)
+  except Exception as e:
+    assert str(type(e)) == "<class 'ValueError'>"
+    assert str(e) == "3 is not in list"
+
 
 def test_index_found_with_start_and_stop():
-    a = pm.eval("[1,2,3,4]")
-    b = a.index(3,1,4)
-    assert b == 2              
+  a = pm.eval("[1,2,3,4]")
+  b = a.index(3, 1, 4)
+  assert b == 2
+
 
 def test_index_found_with_start_and_negative_stop():
-    a = pm.eval("[1,2,3,4]")
-    b = a.index(3,1,-1)
-    assert b == 2       
+  a = pm.eval("[1,2,3,4]")
+  b = a.index(3, 1, -1)
+  assert b == 2
+
 
 def test_index_not_found_with_start_and_stop():
-    a = pm.eval('([1,2,3,4])')
-    try:
-        a.index(3,4,4)     
-        assert (False)
-    except Exception as e:    
-        assert str(type(e)) == "<class 'ValueError'>"
-        assert str(e) == "3 is not in list"  
+  a = pm.eval('([1,2,3,4])')
+  try:
+    a.index(3, 4, 4)
+    assert (False)
+  except Exception as e:
+    assert str(type(e)) == "<class 'ValueError'>"
+    assert str(e) == "3 is not in list"
+
 
 def test_index_not_found_with_start_and_outofbounds_stop():
-    a = pm.eval('([1,2,3,4])')
-    try:
-        a.index(3,4,7)     
-        assert (False)
-    except Exception as e:    
-        assert str(type(e)) == "<class 'ValueError'>"
-        assert str(e) == "3 is not in list"       
+  a = pm.eval('([1,2,3,4])')
+  try:
+    a.index(3, 4, 7)
+    assert (False)
+  except Exception as e:
+    assert str(type(e)) == "<class 'ValueError'>"
+    assert str(e) == "3 is not in list"
+
+# count
+
 
-#count
 def test_count_found_once():
-    a = pm.eval("[1,2,3,4]")
-    b = a.count(1)
-    assert b == 1   
+  a = pm.eval("[1,2,3,4]")
+  b = a.count(1)
+  assert b == 1
+
 
 def test_count_found_once_non_primitive_type():
-    a = pm.eval("[1,2,[3,4]]")
-    b = a.count([3,4])
-    assert b == 1      
+  a = pm.eval("[1,2,[3,4]]")
+  b = a.count([3, 4])
+  assert b == 1
+
 
 def test_count_found_twice():
-    a = pm.eval("[1,2,3,4,5,1,2]")
-    b = a.count(2)
-    assert b == 2   
+  a = pm.eval("[1,2,3,4,5,1,2]")
+  b = a.count(2)
+  assert b == 2
+
 
 def test_count_not_found():
-    a = pm.eval("[1,2,3,4,5,1,2]")
-    b = a.count(7)
-    assert b == 0      
+  a = pm.eval("[1,2,3,4,5,1,2]")
+  b = a.count(7)
+  assert b == 0
+
+# reverse
+
 
-#reverse
 def test_reverse():
-    a = pm.eval("[1,2,3,4]")
-    b = a.reverse()
-    assert a == [4,3,2,1]
-    assert b == None    
+  a = pm.eval("[1,2,3,4]")
+  b = a.reverse()
+  assert a == [4, 3, 2, 1]
+  assert b is None
+
 
 def test_reverse_zero_length():
-    a = pm.eval("[]")
-    a.reverse()
-    assert a == []       
+  a = pm.eval("[]")
+  a.reverse()
+  assert a == []
+
 
 def test_reverse_one_length():
-    a = pm.eval("[2]")
-    a.reverse()
-    assert a == [2]  
+  a = pm.eval("[2]")
+  a.reverse()
+  assert a == [2]
+
 
 def test_reverse_too_many_args():
-    a = pm.eval('([1,2,3,4])')
-    try:
-        a.reverse(3)     
-        assert (False)
-    except Exception as e:    
-        assert str(type(e)) == "<class 'TypeError'>"
-        assert str(e).__contains__('reverse() takes no arguments (1 given)')       
+  a = pm.eval('([1,2,3,4])')
+  try:
+    a.reverse(3)
+    assert (False)
+  except Exception as e:
+    assert str(type(e)) == "<class 'TypeError'>"
+    assert str(e).__contains__('reverse() takes no arguments (1 given)')
+
+# sort
+
 
-#sort
 def test_sort():
-    a = pm.eval("[5,1,2,4,9,6,3,7,8]")
-    a.sort()
-    assert a == [1,2,3,4,5,6,7,8,9]       
+  a = pm.eval("[5,1,2,4,9,6,3,7,8]")
+  a.sort()
+  assert a == [1, 2, 3, 4, 5, 6, 7, 8, 9]
+
 
 def test_sort_reverse():
-    a = pm.eval("[5,1,2,4,9,6,3,7,8]")
-    a.sort(reverse=True)
-    assert a == [9,8,7,6,5,4,3,2,1]   
+  a = pm.eval("[5,1,2,4,9,6,3,7,8]")
+  a.sort(reverse=True)
+  assert a == [9, 8, 7, 6, 5, 4, 3, 2, 1]
+
 
 def test_sort_reverse_false():
-    a = pm.eval("[5,1,2,4,9,6,3,7,8]")
-    a.sort(reverse=False)
-    assert a == [1,2,3,4,5,6,7,8,9]      
+  a = pm.eval("[5,1,2,4,9,6,3,7,8]")
+  a.sort(reverse=False)
+  assert a == [1, 2, 3, 4, 5, 6, 7, 8, 9]
+
 
 def test_sort_with_function():
-    def myFunc(e,f):
-        return len(e) - len(f)     
-    a = pm.eval("(['Ford', 'Mitsubishi', 'BMW', 'VW'])")
-    a.sort(key=myFunc)
-    assert a == ['VW', 'BMW', 'Ford', 'Mitsubishi']   
+  def myFunc(e, f):
+    return len(e) - len(f)
+  a = pm.eval("(['Ford', 'Mitsubishi', 'BMW', 'VW'])")
+  a.sort(key=myFunc)
+  assert a == ['VW', 'BMW', 'Ford', 'Mitsubishi']
+
 
 def test_sort_with_js_function():
-    a = pm.eval("(['Ford', 'Mitsubishi', 'BMW', 'VW'])")
-    myFunc = pm.eval("((a, b) => a.toLocaleUpperCase() < b.toLocaleUpperCase() ? -1 : 1)")
-    a.sort(key=myFunc)
-    assert a == ['BMW', 'Ford', 'Mitsubishi', 'VW']    
+  a = pm.eval("(['Ford', 'Mitsubishi', 'BMW', 'VW'])")
+  myFunc = pm.eval("((a, b) => a.toLocaleUpperCase() < b.toLocaleUpperCase() ? -1 : 1)")
+  a.sort(key=myFunc)
+  assert a == ['BMW', 'Ford', 'Mitsubishi', 'VW']
+
 
 def test_sort_with_one_arg_function():
-    def myFunc(e):
-        return len(e)     
-    a = pm.eval("(['Ford', 'Mitsubishi', 'BMW', 'VW'])")
-    a.sort(key=myFunc)
-    assert a == ['VW', 'BMW', 'Ford', 'Mitsubishi'] 
+  def myFunc(e):
+    return len(e)
+  a = pm.eval("(['Ford', 'Mitsubishi', 'BMW', 'VW'])")
+  a.sort(key=myFunc)
+  assert a == ['VW', 'BMW', 'Ford', 'Mitsubishi']
+
 
 def test_sort_with_one_arg_function_wrong_data_type():
-    def myFunc(e):
-        return len(e)     
-    a = pm.eval('([1,2,3,4])')
-    try:
-        a.sort(key=myFunc)   
-        assert (False)
-    except Exception as e:    
-        assert str(type(e)) == "<class 'TypeError'>"
-        assert str(e) == "object of type 'float' has no len()"    
+  def myFunc(e):
+    return len(e)
+  a = pm.eval('([1,2,3,4])')
+  try:
+    a.sort(key=myFunc)
+    assert (False)
+  except Exception as e:
+    assert str(type(e)) == "<class 'TypeError'>"
+    assert str(e) == "object of type 'float' has no len()"
+
 
 def test_sort_with_function_two_args_and_reverse_false():
-    def myFunc(e,f):
-        return len(e) - len(f)     
-    a = pm.eval("(['Ford', 'Mitsubishi', 'BMW', 'VW'])")
-    a.sort(key=myFunc, reverse=False)
-    assert a == ['VW', 'BMW', 'Ford', 'Mitsubishi']   
+  def myFunc(e, f):
+    return len(e) - len(f)
+  a = pm.eval("(['Ford', 'Mitsubishi', 'BMW', 'VW'])")
+  a.sort(key=myFunc, reverse=False)
+  assert a == ['VW', 'BMW', 'Ford', 'Mitsubishi']
+
 
 def test_sort_with_js_function_and_reverse_false():
-    a = pm.eval("(['Ford', 'Mitsubishi', 'BMW', 'VW'])")
-    myFunc = pm.eval("((a, b) => a.toLocaleUpperCase() < b.toLocaleUpperCase() ? -1 : 1)")
-    a.sort(key=myFunc, reverse=False)
-    assert a == ['BMW', 'Ford', 'Mitsubishi', 'VW']    
+  a = pm.eval("(['Ford', 'Mitsubishi', 'BMW', 'VW'])")
+  myFunc = pm.eval("((a, b) => a.toLocaleUpperCase() < b.toLocaleUpperCase() ? -1 : 1)")
+  a.sort(key=myFunc, reverse=False)
+  assert a == ['BMW', 'Ford', 'Mitsubishi', 'VW']
+
 
 def test_sort_with_function_and_reverse():
-    def myFunc(e,f):
-        return len(e) - len(f)     
-    a = pm.eval("(['Ford', 'Mitsubishi', 'BMW', 'VW'])")
-    a.sort(key=myFunc, reverse=True)
-    assert a == ['Mitsubishi', 'Ford', 'BMW', 'VW']
+  def myFunc(e, f):
+    return len(e) - len(f)
+  a = pm.eval("(['Ford', 'Mitsubishi', 'BMW', 'VW'])")
+  a.sort(key=myFunc, reverse=True)
+  assert a == ['Mitsubishi', 'Ford', 'BMW', 'VW']
+
 
 def test_sort_with_js_function_and_reverse():
-    a = pm.eval("(['Ford', 'Mitsubishi', 'BMW', 'VW'])")
-    myFunc = pm.eval("((a, b) => a.toLocaleUpperCase() < b.toLocaleUpperCase() ? -1 : 1)")
-    a.sort(key=myFunc, reverse=True)
-    assert a == ['VW', 'Mitsubishi', 'Ford', 'BMW']      
+  a = pm.eval("(['Ford', 'Mitsubishi', 'BMW', 'VW'])")
+  myFunc = pm.eval("((a, b) => a.toLocaleUpperCase() < b.toLocaleUpperCase() ? -1 : 1)")
+  a.sort(key=myFunc, reverse=True)
+  assert a == ['VW', 'Mitsubishi', 'Ford', 'BMW']
+
 
 def test_sort_with_function_wrong_type():
-    a = pm.eval('([1,2,3,4])')
-    try:
-        b = 9
-        a.sort(key=b)    
-        assert (False)
-    except Exception as e:    
-        assert str(type(e)) == "<class 'TypeError'>"
-        assert str(e) == "'int' object is not callable"       
+  a = pm.eval('([1,2,3,4])')
+  try:
+    b = 9
+    a.sort(key=b)
+    assert (False)
+  except Exception as e:
+    assert str(type(e)) == "<class 'TypeError'>"
+    assert str(e) == "'int' object is not callable"
+
 
 def test_tricky_sort():
-    a = pm.eval("[6, -2, 2, -7]")
-    a.sort()
-    assert a == [-7, -2, 2, 6]  
+  a = pm.eval("[6, -2, 2, -7]")
+  a.sort()
+  assert a == [-7, -2, 2, 6]
+
 
 def test_tricky_sort_reverse():
-    a = pm.eval("[6, -2, 2, -7]")
-    a.sort(reverse=True)
-    assert a == [6, 2, -2, -7]  
+  a = pm.eval("[6, -2, 2, -7]")
+  a.sort(reverse=True)
+  assert a == [6, 2, -2, -7]
+
 
 def test_sort_with_builtin_function():     # + wrong type of entries
-    a = pm.eval("(['Ford', 'Mitsubishi', 'BMW', 'VW'])")
-    a.sort(key=len)
-    assert a == ['VW', 'BMW', 'Ford', 'Mitsubishi']     
+  a = pm.eval("(['Ford', 'Mitsubishi', 'BMW', 'VW'])")
+  a.sort(key=len)
+  assert a == ['VW', 'BMW', 'Ford', 'Mitsubishi']
+
 
 def test_sort_with_builtin_function_and_reverse():     # + wrong type of entries
-    a = pm.eval("(['Ford', 'Mitsubishi', 'BMW', 'VW'])")
-    a.sort(key=len, reverse=True)
-    assert a == ['Mitsubishi', 'Ford', 'BMW', 'VW']        
+  a = pm.eval("(['Ford', 'Mitsubishi', 'BMW', 'VW'])")
+  a.sort(key=len, reverse=True)
+  assert a == ['Mitsubishi', 'Ford', 'BMW', 'VW']
+
 
 def test_sort_with_builtin_function_wrong_data_type():
-    a = pm.eval('([1,2,3,4])')
-    try:
-        a.sort(key=len)   
-        assert (False)
-    except Exception as e:    
-        assert str(type(e)) == "<class 'TypeError'>"
-        assert str(e) == "object of type 'float' has no len()"       
+  a = pm.eval('([1,2,3,4])')
+  try:
+    a.sort(key=len)
+    assert (False)
+  except Exception as e:
+    assert str(type(e)) == "<class 'TypeError'>"
+    assert str(e) == "object of type 'float' has no len()"
+
+# iter
+
 
-#iter
 def iter_min():
-    a = pm.eval("([7,9,1,2,3,4,5,6])")
-    b = min(a)
-    assert b == 1    
+  a = pm.eval("([7,9,1,2,3,4,5,6])")
+  b = min(a)
+  assert b == 1
+
 
 def iter_max():
-    a = pm.eval("([7,9,1,2,3,4,5,6])")
-    b = max(a)
-    assert b == 9   
+  a = pm.eval("([7,9,1,2,3,4,5,6])")
+  b = max(a)
+  assert b == 9
+
 
 def iter_for():
-    a = pm.eval("(['this is a test', 'another test'])")
-    b = [item.upper() for item in a]
-    assert b ==  ['THIS IS A TEST', 'ANOTHER TEST']   
+  a = pm.eval("(['this is a test', 'another test'])")
+  b = [item.upper() for item in a]
+  assert b == ['THIS IS A TEST', 'ANOTHER TEST']
+
 
 def test_reduce():
-    a = pm.eval("([1, 3, 5, 6, 2])")
-    result = reduce(lambda a, b: a+b, a)
-    assert result == 17  
+  a = pm.eval("([1, 3, 5, 6, 2])")
+  result = reduce(lambda a, b: a + b, a)
+  assert result == 17
+
 
 def test_iter_next():
-    a = pm.eval("([1, 3, 5, 6, 2])")
-    iterator = iter(a)
-    try:
-        while True:
-            element = next(iterator)
-        assert(False)    
-    except StopIteration:
-        assert(True)   
+  a = pm.eval("([1, 3, 5, 6, 2])")
+  iterator = iter(a)
+  try:
+    while True:
+      element = next(iterator)
+    assert (False)
+  except StopIteration:
+    assert (True)
+
+# reverse_iter
+
 
-#reverse_iter
 def iter_reverse():
-    a = pm.eval("(['7','9','1','2','3','4','5','6'])")
-    b = ""
-    for i in reversed(a):
-        b += i
-    assert b == '65432197' 
+  a = pm.eval("(['7','9','1','2','3','4','5','6'])")
+  b = ""
+  for i in reversed(a):
+    b += i
+  assert b == '65432197'
 
 # slice subscript
+
+
 def test_slice_full_array_single_subscript():
-    a = pm.eval("([1,2,3,4,5,6])")
-    b = a[:]
-    assert b == [1,2,3,4,5,6]  
+  a = pm.eval("([1,2,3,4,5,6])")
+  b = a[:]
+  assert b == [1, 2, 3, 4, 5, 6]
+
 
 def test_slice_full_array_double_subscript():
-    a = pm.eval("([1,2,3,4,5,6])")
-    b = a[::]
-    assert b == [1,2,3,4,5,6]      
+  a = pm.eval("([1,2,3,4,5,6])")
+  b = a[::]
+  assert b == [1, 2, 3, 4, 5, 6]
+
 
 def test_slice_empty_length_left():
-    a = pm.eval("([1,2,3,4,5,6])")
-    b = a[len(a):]
-    assert b == []            
+  a = pm.eval("([1,2,3,4,5,6])")
+  b = a[len(a):]
+  assert b == []
+
 
 def test_slice_full_length_right():
-    a = pm.eval("([1,2,3,4,5,6])")
-    b = a[:len(a)]
-    assert b == [1,2,3,4,5,6]    
+  a = pm.eval("([1,2,3,4,5,6])")
+  b = a[:len(a)]
+  assert b == [1, 2, 3, 4, 5, 6]
+
 
 def test_slice_zero_to_length():
-    a = pm.eval("([1,2,3,4,5,6])")
-    b = a[0:6]
-    assert b == [1,2,3,4,5,6]  
+  a = pm.eval("([1,2,3,4,5,6])")
+  b = a[0:6]
+  assert b == [1, 2, 3, 4, 5, 6]
+
 
 def test_slice():
-    a = pm.eval("([1,2,3,4,5,6])")
-    b = a[1:5]
-    assert b == [2,3,4,5]   
+  a = pm.eval("([1,2,3,4,5,6])")
+  b = a[1:5]
+  assert b == [2, 3, 4, 5]
+
 
 def test_slice_negative_start():
-    a = pm.eval("([1,2,3,4,5,6])")
-    b = a[-3:5]
-    assert b == [4,5] 
+  a = pm.eval("([1,2,3,4,5,6])")
+  b = a[-3:5]
+  assert b == [4, 5]
+
 
 def test_slice_negative_end():
-    a = pm.eval("([1,2,3,4,5,6])")
-    b = a[2:-1]
-    assert b == [3,4,5]   
+  a = pm.eval("([1,2,3,4,5,6])")
+  b = a[2:-1]
+  assert b == [3, 4, 5]
+
 
 def test_slice_negative_start_negative_end():
-    a = pm.eval("([1,2,3,4,5,6])")
-    b = a[-3:-1]
-    assert b == [4,5]  
+  a = pm.eval("([1,2,3,4,5,6])")
+  b = a[-3:-1]
+  assert b == [4, 5]
+
 
 def test_slice_step_zero():
-    a = pm.eval('([1,2,3,4])')
-    try:
-        a[0:6:0]    
-        assert (False)
-    except Exception as e:    
-        assert str(type(e)) == "<class 'ValueError'>"
-        assert str(e) == "slice step cannot be zero"     
+  a = pm.eval('([1,2,3,4])')
+  try:
+    a[0:6:0]
+    assert (False)
+  except Exception as e:
+    assert str(type(e)) == "<class 'ValueError'>"
+    assert str(e) == "slice step cannot be zero"
+
 
 def test_slice_step_negative():
-    a = pm.eval("([1,2,3,4,5,6])")
-    b = a[0:5:-1]
-    assert b == []    
+  a = pm.eval("([1,2,3,4,5,6])")
+  b = a[0:5:-1]
+  assert b == []
+
 
 def test_slice_step_one():
-    a = pm.eval("([1,2,3,4,5,6])")
-    b = a[1:5:1]
-    assert b == [2,3,4,5] 
+  a = pm.eval("([1,2,3,4,5,6])")
+  b = a[1:5:1]
+  assert b == [2, 3, 4, 5]
+
 
 def test_slice_step_two():
-    a = pm.eval("([1,2,3,4,5,6])")
-    b = a[1:5:2]
-    assert b == [2,4]    
+  a = pm.eval("([1,2,3,4,5,6])")
+  b = a[1:5:2]
+  assert b == [2, 4]
+
 
 def test_slice_step_three():
-    a = pm.eval("([1,2,3,4,5,6])")
-    b = a[1:5:3]
-    assert b == [2,5]           
+  a = pm.eval("([1,2,3,4,5,6])")
+  b = a[1:5:3]
+  assert b == [2, 5]
+
+# slice subscript assign
+
 
-#slice subscript assign
 def test_slice_assign_partial_array():
-    a = pm.eval("([1,2,3,4,5,6])")
-    a[2:4] = [7,8,9,0,1,2]
-    assert a == [1,2,7,8,9,0,1,2,5,6] 
+  a = pm.eval("([1,2,3,4,5,6])")
+  a[2:4] = [7, 8, 9, 0, 1, 2]
+  assert a == [1, 2, 7, 8, 9, 0, 1, 2, 5, 6]
+
 
 def test_slice_delete_partial_array():
-    a = pm.eval("([1,2,3,4,5,6])")
-    del a[2:4]
-    assert a == [1,2,5,6]   
+  a = pm.eval("([1,2,3,4,5,6])")
+  del a[2:4]
+  assert a == [1, 2, 5, 6]
+
 
 def test_slice_assign_own_array():
-    a = pm.eval("([1,2,3,4,5,6])")
-    a[2:4] = a
-    assert a == [1,2,1,2,3,4,5,6,5,6]     
+  a = pm.eval("([1,2,3,4,5,6])")
+  a[2:4] = a
+  assert a == [1, 2, 1, 2, 3, 4, 5, 6, 5, 6]
+
 
 def test_slice_assign_pm_array():
-    a = pm.eval("([1,2,3,4,5,6])")
-    b = pm.eval("([7,8])")
-    a[2:4] = b
-    assert a == [1,2,7,8,5,6]       
+  a = pm.eval("([1,2,3,4,5,6])")
+  b = pm.eval("([7,8])")
+  a[2:4] = b
+  assert a == [1, 2, 7, 8, 5, 6]
+
 
 def test_slice_assign_wrong_type():
-    a = pm.eval('([1,2,3,4])')
-    try:
-        a[2:4] = 6  
-        assert (False)
-    except Exception as e:    
-        assert str(type(e)) == "<class 'TypeError'>"
-        assert str(e) == "can only assign an iterable"       
+  a = pm.eval('([1,2,3,4])')
+  try:
+    a[2:4] = 6
+    assert (False)
+  except Exception as e:
+    assert str(type(e)) == "<class 'TypeError'>"
+    assert str(e) == "can only assign an iterable"
+
 
 def test_slice_assign_negative_low():
-    a = pm.eval("([1,2,3,4,5,6])")
-    a[-3:6] = [7,8]
-    assert a == [1,2,3,7,8]
+  a = pm.eval("([1,2,3,4,5,6])")
+  a[-3:6] = [7, 8]
+  assert a == [1, 2, 3, 7, 8]
+
 
 def test_slice_assign_negative_low_negative_high():
-    a = pm.eval("([1,2,3,4,5,6])")
-    a[-3:-1] = [7,8]
-    assert a == [1,2,3,7,8,6]    
+  a = pm.eval("([1,2,3,4,5,6])")
+  a[-3:-1] = [7, 8]
+  assert a == [1, 2, 3, 7, 8, 6]
+
 
 def test_slice_assign_high_larger_than_length():
-    a = pm.eval("([1,2,3,4,5,6])")
-    a[1:8] = [7,8]
-    assert a == [1,7,8]   
+  a = pm.eval("([1,2,3,4,5,6])")
+  a[1:8] = [7, 8]
+  assert a == [1, 7, 8]
+
 
 def test_slice_assign_clear():
-    a = pm.eval("([1,2,3,4,5,6,7,8,9,1,2])")
-    a[0:32] = []
-    assert a == []    
+  a = pm.eval("([1,2,3,4,5,6,7,8,9,1,2])")
+  a[0:32] = []
+  assert a == []
+
 
 def test_slice_delete_partial_array_step_negative():
-    a = pm.eval("([1,2,3,4,5,6])")
-    del a[0:4:-1]
-    assert a == [1,2,3,4,5,6]  
+  a = pm.eval("([1,2,3,4,5,6])")
+  del a[0:4:-1]
+  assert a == [1, 2, 3, 4, 5, 6]
+
 
 def test_slice_delete_partial_array_step_one():
-    a = pm.eval("([1,2,3,4,5,6])")
-    del a[2:4:1]
-    assert a == [1,2,5,6]       
+  a = pm.eval("([1,2,3,4,5,6])")
+  del a[2:4:1]
+  assert a == [1, 2, 5, 6]
+
 
 def test_slice_delete_partial_array_step_two():
-    a = pm.eval("([1,2,3,4,5,6])")
-    del a[2:6:2]
-    assert a == [1,2,4,6]    
+  a = pm.eval("([1,2,3,4,5,6])")
+  del a[2:6:2]
+  assert a == [1, 2, 4, 6]
+
 
 def test_slice_delete_partial_array_step_three():
-    a = pm.eval("([1,2,3,4,5,6])")
-    del a[0:6:3]
-    assert a == [2,3,5,6]    
+  a = pm.eval("([1,2,3,4,5,6])")
+  del a[0:6:3]
+  assert a == [2, 3, 5, 6]
+
 
 def test_slice_delete_partial_array_step_two_negative_start():
-    a = pm.eval("([1,2,3,4,5,6])")
-    del a[-5:6:2]
-    assert a == [1,3,5] 
+  a = pm.eval("([1,2,3,4,5,6])")
+  del a[-5:6:2]
+  assert a == [1, 3, 5]
+
 
 def test_slice_delete_partial_array_step_two_negative_start_negative_end():
-    a = pm.eval("([1,2,3,4,5,6])")
-    del a[-5:-2:2]
-    assert a == [1,3,5,6]     
+  a = pm.eval("([1,2,3,4,5,6])")
+  del a[-5:-2:2]
+  assert a == [1, 3, 5, 6]
+
 
 def test_slice_assign_step_wrong_list_size():
-    a = pm.eval('([1,2,3,4])')
-    try:
-        a[0:4:2] = [1]  
-        assert (False)
-    except Exception as e:    
-        assert str(type(e)) == "<class 'ValueError'>"
-        assert str(e) == "attempt to assign sequence of size 1 to extended slice of size 2"    
+  a = pm.eval('([1,2,3,4])')
+  try:
+    a[0:4:2] = [1]
+    assert (False)
+  except Exception as e:
+    assert str(type(e)) == "<class 'ValueError'>"
+    assert str(e) == "attempt to assign sequence of size 1 to extended slice of size 2"
+
 
 def test_slice_assign_partial_array_step_negative():
-    a = pm.eval("([1,2,3,4,5,6])")
-    a[2:4:2] = [7]
-    assert a == [1,2,7,4,5,6]    
+  a = pm.eval("([1,2,3,4,5,6])")
+  a[2:4:2] = [7]
+  assert a == [1, 2, 7, 4, 5, 6]
+
 
 def test_slice_assign_step_zero():
-    a = pm.eval('([1,2,3,4])')
-    try:
-        a[0:4:0] = [1]  
-        assert (False)
-    except Exception as e:    
-        assert str(type(e)) == "<class 'ValueError'>"
-        assert str(e) == "slice step cannot be zero"               
+  a = pm.eval('([1,2,3,4])')
+  try:
+    a[0:4:0] = [1]
+    assert (False)
+  except Exception as e:
+    assert str(type(e)) == "<class 'ValueError'>"
+    assert str(e) == "slice step cannot be zero"
+
 
 def test_slice_assign_partial_array_step_2():
-    a = pm.eval("([1,2,3,4,5,6])")
-    a[2:4:2] = [7]
-    assert a == [1,2,7,4,5,6]     
+  a = pm.eval("([1,2,3,4,5,6])")
+  a[2:4:2] = [7]
+  assert a == [1, 2, 7, 4, 5, 6]
+
 
 def test_slice_assign_step_wrong_type():
-    a = pm.eval('([1,2,3,4])')
-    try:
-        a[2:4:2] = 6  
-        assert (False)
-    except Exception as e:    
-        assert str(type(e)) == "<class 'TypeError'>"
-        assert str(e) == "must assign iterable to extended slice"  
+  a = pm.eval('([1,2,3,4])')
+  try:
+    a[2:4:2] = 6
+    assert (False)
+  except Exception as e:
+    assert str(type(e)) == "<class 'TypeError'>"
+    assert str(e) == "must assign iterable to extended slice"
+
 
 def test_slice_assign_partial_array_negative_start():
-    a = pm.eval("([1,2,3,4,5,6])")
-    a[-5:4:2] = [7,8]
-    assert a == [1, 7, 3, 8, 5, 6]    
+  a = pm.eval("([1,2,3,4,5,6])")
+  a[-5:4:2] = [7, 8]
+  assert a == [1, 7, 3, 8, 5, 6]
+
 
 def test_slice_assign_partial_array_negative_start_negative_stop():
-    a = pm.eval("([1,2,3,4,5,6])")
-    a[-5:-1:2] = [7,8]
-    assert a == [1, 7, 3, 8, 5, 6]   
+  a = pm.eval("([1,2,3,4,5,6])")
+  a[-5:-1:2] = [7, 8]
+  assert a == [1, 7, 3, 8, 5, 6]
+
 
 def test_slice_assign_own_array_no_match():
-    a = pm.eval("([1,2,3,4,5,6])")
-    try:
-        a[0:4:2] = a  
-        assert (False)
-    except Exception as e:    
-        assert str(type(e)) == "<class 'ValueError'>"
-        assert str(e) == "attempt to assign sequence of size 0 to extended slice of size 2"           
+  a = pm.eval("([1,2,3,4,5,6])")
+  try:
+    a[0:4:2] = a
+    assert (False)
+  except Exception as e:
+    assert str(type(e)) == "<class 'ValueError'>"
+    assert str(e) == "attempt to assign sequence of size 0 to extended slice of size 2"
+
 
 def test_slice_assign_pm_array_step_2():
-    a = pm.eval("([1,2,3,4,5,6])")
-    b = pm.eval("([1,2,3])")
-    a[0:10:2] = b
-    assert a == [1, 2, 2, 4, 3, 6]
-
-#__class__
-def test___class__attribute():  
-    items = pm.eval("([1,2,3,4,5,6])")
-    assert repr(items.__class__) == "<class 'list'>"          
+  a = pm.eval("([1,2,3,4,5,6])")
+  b = pm.eval("([1,2,3])")
+  a[0:10:2] = b
+  assert a == [1, 2, 2, 4, 3, 6]
+
+# __class__
+
+
+def test___class__attribute():
+  items = pm.eval("([1,2,3,4,5,6])")
+  assert repr(items.__class__) == "<class 'list'>"
```

### Comparing `pythonmonkey-0.4.0/tests/python/test_objects.py` & `pythonmonkey-0.6.0/tests/python/test_objects.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,136 +1,150 @@
 import pythonmonkey as pm
 
+
 def test_eval_pyobjects():
   class MyClass:
     pass
 
   o = MyClass()
   proxy_o = pm.eval("(obj) => { return obj; }")(o)
   assert o is proxy_o
 
+
 def test_eval_pyobjects_subobjects():
   class InnerClass:
     def __init__(self):
       self.c = 2
 
   class OuterClass:
     def __init__(self):
       self.a = 1
       self.b = InnerClass()
-  
+
   o = OuterClass()
 
   assert pm.eval("(obj) => { return obj.a;   }")(o) == 1.0
   assert pm.eval("(obj) => { return obj.b;   }")(o) is o.b
   assert pm.eval("(obj) => { return obj.b.c; }")(o) == 2.0
 
+
 def test_eval_pyobjects_cycle():
   class MyClass:
     def __init__(self):
       self.a = 1
       self.b = 2
       self.recursive = self
-  
+
   o = MyClass()
-  
+
   assert pm.eval("(obj) => { return obj.a;         }")(o) == 1.0
   assert pm.eval("(obj) => { return obj.b;         }")(o) == 2.0
   assert pm.eval("(obj) => { return obj.recursive; }")(o) is o.recursive
 
+
 def test_eval_pyobjects_proxy_get():
   class MyClass:
     def __init__(self):
       self.a = 42
-  
+
   o = MyClass()
 
   assert pm.eval("(obj) => { return obj.a}")(o) == 42.0
 
+
 def test_eval_pyobjects_proxy_set():
   class MyClass:
     def __init__(self):
       self.a = 42
-  
+
   o = MyClass()
 
   pm.eval("(obj) => { obj.b = 43; }")(o)
   assert o.b == 43.0
 
+
 def test_eval_pyobjects_proxy_keys():
   class MyClass:
     def __init__(self):
       self.a = 42
-  
+
   o = MyClass()
 
   assert pm.eval("(obj) => { return Object.keys(obj)[0]; }")(o) == 'a'
 
+
 def test_eval_pyobjects_proxy_delete():
   class MyClass:
     def __init__(self):
       self.a = 42
-  
+
   o = MyClass()
 
   pm.eval("(obj) => { delete obj.a; }")(o)
   assert not hasattr(o, 'a')
 
+
 def test_eval_pyobjects_proxy_has():
   class MyClass:
     def __init__(self):
       self.a = 42
-  
+
   o = MyClass()
 
   assert pm.eval("(obj) => { return 'a' in obj; }")(o)
 
+
 def test_eval_pyobjects_proxy_not_extensible():
   class MyClass:
     def __init__(self):
       self.a = 42
-  
+
   o = MyClass()
 
   assert not pm.eval("(o) => Object.isExtensible(o)")(o)
   assert pm.eval("(o) => Object.preventExtensions(o) === o")(o)
 
+
 def test_instanceof_pyobject():
   class MyClass:
     def __init__(self):
       self.a = 42
-  
+
   o = MyClass()
   assert pm.eval("(obj) => { return obj instanceof Object; }")(o)
 
+
 def test_pyobjects_not_instanceof_string():
   class MyClass:
     def __init__(self):
       self.a = 42
-  
+
   o = MyClass()
 
   assert not pm.eval("(obj) => { return obj instanceof String; }")(o)
 
+
 def test_pyobjects_valueOf():
   class MyClass:
     def __init__(self):
       self.a = 42
-  
+
   o = MyClass()
   assert o is pm.eval("(obj) => { return obj.valueOf(); }")(o)
 
+
 def test_pyobjects_toString():
   class MyClass:
     def __init__(self):
       self.a = 42
-  
+
   o = MyClass()
   assert '[object Object]' == pm.eval("(obj) => { return obj.toString(); }")(o)
 
+
 def test_pyobjects_toLocaleString():
   class MyClass:
     def __init__(self):
       self.a = 42
-  
+
   o = MyClass()
-  assert '[object Object]' == pm.eval("(obj) => { return obj.toLocaleString(); }")(o)
+  assert '[object Object]' == pm.eval("(obj) => { return obj.toLocaleString(); }")(o)
```

### Comparing `pythonmonkey-0.4.0/tests/python/test_pythonmonkey_eval.py` & `pythonmonkey-0.6.0/tests/python/test_pythonmonkey_eval.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,351 +2,389 @@
 import pythonmonkey as pm
 import random
 from datetime import datetime, timedelta, timezone
 import math
 from io import StringIO
 import sys
 
+
 def test_passes():
-    assert True
+  assert True
+
 
 def test_eval_numbers_floats():
-    for _ in range(10):
-        py_number = random.uniform(-1000000,1000000)
-        js_number = pm.eval(repr(py_number))
-        assert py_number == js_number
+  for _ in range(10):
+    py_number = random.uniform(-1000000, 1000000)
+    js_number = pm.eval(repr(py_number))
+    assert py_number == js_number
+
 
 def test_eval_numbers_floats_nan():
-    jsNaN = pm.eval("NaN")
-    assert math.isnan(jsNaN)
+  jsNaN = pm.eval("NaN")
+  assert math.isnan(jsNaN)
+
 
 def test_eval_numbers_floats_negative_zero():
-    jsNegZero = pm.eval("-0")
-    assert jsNegZero == 0
-    assert jsNegZero == 0.0 # expected that -0.0 == 0.0 == 0
-    # https://docs.python.org/3/library/math.html#math.copysign
-    assert math.copysign(1.0, jsNegZero) == -1.0
+  jsNegZero = pm.eval("-0")
+  assert jsNegZero == 0
+  assert jsNegZero == 0.0  # expected that -0.0 == 0.0 == 0
+  # https://docs.python.org/3/library/math.html#math.copysign
+  assert math.copysign(1.0, jsNegZero) == -1.0
+
 
 def test_eval_numbers_floats_inf():
-    jsPosInf = pm.eval("Infinity")
-    jsNegInf = pm.eval("-Infinity")
-    assert jsPosInf == float("+inf")
-    assert jsNegInf == float("-inf")
+  jsPosInf = pm.eval("Infinity")
+  jsNegInf = pm.eval("-Infinity")
+  assert jsPosInf == float("+inf")
+  assert jsNegInf == float("-inf")
+
 
 def test_eval_numbers_integers():
-    for _ in range(10):
-        py_number = random.randint(-1000000,1000000)
-        js_number = pm.eval(repr(py_number))
-        assert py_number == js_number
+  for _ in range(10):
+    py_number = random.randint(-1000000, 1000000)
+    js_number = pm.eval(repr(py_number))
+    assert py_number == js_number
+
 
 def test_eval_booleans():
-    py_bool = True
-    js_bool = pm.eval('true')
-    assert py_bool == js_bool
-    py_bool = False
-    js_bool = pm.eval('false')
-    assert py_bool == js_bool
+  py_bool = True
+  js_bool = pm.eval('true')
+  assert py_bool == js_bool
+  py_bool = False
+  js_bool = pm.eval('false')
+  assert py_bool == js_bool
+
 
 def test_eval_dates():
-    MIN_YEAR = 1 # https://docs.python.org/3/library/datetime.html#datetime.MINYEAR
-    MAX_YEAR = 2023
-    start = datetime(MIN_YEAR, 1, 1, 00, 00, 00, tzinfo=timezone.utc)
-    years = MAX_YEAR - MIN_YEAR + 1
-    end = start + timedelta(days=365 * years)
-    for _ in range(10):
-        py_date = start + (end - start) * random.random()
-        # round to milliseconds precision because the smallest unit for js Date is 1ms
-        py_date = py_date.replace(microsecond=min(round(py_date.microsecond, -3), 999000)) # microsecond must be in 0..999999, but it would be rounded to 1000000 if >= 999500
-        js_date = pm.eval(f'new Date("{py_date.isoformat()}")')
-        assert py_date == js_date
+  MIN_YEAR = 1  # https://docs.python.org/3/library/datetime.html#datetime.MINYEAR
+  MAX_YEAR = 2023
+  start = datetime(MIN_YEAR, 1, 1, 00, 00, 00, tzinfo=timezone.utc)
+  years = MAX_YEAR - MIN_YEAR + 1
+  end = start + timedelta(days=365 * years)
+  for _ in range(10):
+    py_date = start + (end - start) * random.random()
+    # round to milliseconds precision because the smallest unit for js Date is 1ms
+    # microsecond must be in 0..999999, but it would be rounded to 1000000 if >= 999500
+    py_date = py_date.replace(microsecond=min(round(py_date.microsecond, -3), 999000))
+    js_date = pm.eval(f'new Date("{py_date.isoformat()}")')
+    assert py_date == js_date
+
 
 def test_eval_boxed_booleans():
-    py_bool = True
-    js_bool = pm.eval('new Boolean(true)')
-    assert py_bool == js_bool
-    py_bool = False
-    js_bool = pm.eval('new Boolean(false)')
-    assert py_bool == js_bool
+  py_bool = True
+  js_bool = pm.eval('new Boolean(true)')
+  assert py_bool == js_bool
+  py_bool = False
+  js_bool = pm.eval('new Boolean(false)')
+  assert py_bool == js_bool
+
 
 def test_eval_boxed_numbers_floats():
-    for _ in range(10):
-        py_number = random.uniform(-1000000,1000000)
-        js_number = pm.eval(f'new Number({repr(py_number)})')
-        assert py_number == js_number
+  for _ in range(10):
+    py_number = random.uniform(-1000000, 1000000)
+    js_number = pm.eval(f'new Number({repr(py_number)})')
+    assert py_number == js_number
+
 
 def test_eval_boxed_numbers_integers():
-    for _ in range(10):
-        py_number = random.randint(-1000000,1000000)
-        js_number = pm.eval(f'new Number({repr(py_number)})')
-        assert py_number == js_number
+  for _ in range(10):
+    py_number = random.randint(-1000000, 1000000)
+    js_number = pm.eval(f'new Number({repr(py_number)})')
+    assert py_number == js_number
+
 
 def test_eval_exceptions():
-    # should print out the correct error messages
-    with pytest.raises(pm.SpiderMonkeyError, match='SyntaxError: "" literal not terminated before end of script'):
-        pm.eval('"123')
-    with pytest.raises(pm.SpiderMonkeyError, match="SyntaxError: missing } in compound statement"):
-        pm.eval('{')
-    with pytest.raises(pm.SpiderMonkeyError, match="TypeError: can't convert BigInt to number"):
-        pm.eval('1n + 1')
-    with pytest.raises(pm.SpiderMonkeyError, match="ReferenceError: RANDOM_VARIABLE is not defined"):
-        pm.eval('RANDOM_VARIABLE')
-    with pytest.raises(pm.SpiderMonkeyError, match="RangeError: invalid array length"):
-        pm.eval('new Array(-1)')
-    with pytest.raises(pm.SpiderMonkeyError, match="Error: abc"):
-        # manually by the `throw` statement
-        pm.eval('throw new Error("abc")')
-
-    # ANYTHING can be thrown in JS
-    with pytest.raises(pm.SpiderMonkeyError, match="uncaught exception: 9007199254740993"):
-        pm.eval('throw 9007199254740993n') # 2**53+1
-    with pytest.raises(pm.SpiderMonkeyError, match="uncaught exception: null"):
-        pm.eval('throw null')
-    with pytest.raises(pm.SpiderMonkeyError, match="uncaught exception: undefined"):
-        pm.eval('throw undefined')
-    with pytest.raises(pm.SpiderMonkeyError, match="uncaught exception: something from toString"):
-        # (side effect) calls the `toString` method if an object is thrown
-        pm.eval('throw { toString() { return "something from toString" } }')
-
-    # convert JS Error object to a Python Exception object for later use (in a `raise` statement)
-    js_err = pm.eval("new RangeError('to be raised in Python')")
-    assert isinstance(js_err, BaseException)
-    assert isinstance(js_err, Exception)
-    assert type(js_err) == pm.SpiderMonkeyError
-    with pytest.raises(pm.SpiderMonkeyError, match="RangeError: to be raised in Python"):
-        raise js_err
-
-    # convert Python Exception object to a JS Error object
-    get_err_msg = pm.eval("(err) => err.message")
-    assert "Python BufferError: ttt" == get_err_msg(BufferError("ttt"))
-    js_rethrow = pm.eval("(err) => { throw err }")
-    with pytest.raises(pm.SpiderMonkeyError, match="Error: Python BaseException: 123"):
-        js_rethrow(BaseException("123"))
+  # should print out the correct error messages
+  with pytest.raises(pm.SpiderMonkeyError, match='SyntaxError: "" literal not terminated before end of script'):
+    pm.eval('"123')
+  with pytest.raises(pm.SpiderMonkeyError, match="SyntaxError: missing } in compound statement"):
+    pm.eval('{')
+  with pytest.raises(pm.SpiderMonkeyError, match="TypeError: can't convert BigInt to number"):
+    pm.eval('1n + 1')
+  with pytest.raises(pm.SpiderMonkeyError, match="ReferenceError: RANDOM_VARIABLE is not defined"):
+    pm.eval('RANDOM_VARIABLE')
+  with pytest.raises(pm.SpiderMonkeyError, match="RangeError: invalid array length"):
+    pm.eval('new Array(-1)')
+  with pytest.raises(pm.SpiderMonkeyError, match="Error: abc"):
+    # manually by the `throw` statement
+    pm.eval('throw new Error("abc")')
+
+  # ANYTHING can be thrown in JS
+  with pytest.raises(pm.SpiderMonkeyError, match="uncaught exception: 9007199254740993"):
+    pm.eval('throw 9007199254740993n')  # 2**53+1
+  with pytest.raises(pm.SpiderMonkeyError, match="uncaught exception: null"):
+    pm.eval('throw null')
+  with pytest.raises(pm.SpiderMonkeyError, match="uncaught exception: undefined"):
+    pm.eval('throw undefined')
+  with pytest.raises(pm.SpiderMonkeyError, match="uncaught exception: something from toString"):
+    # (side effect) calls the `toString` method if an object is thrown
+    pm.eval('throw { toString() { return "something from toString" } }')
+
+  # convert JS Error object to a Python Exception object for later use (in a `raise` statement)
+  js_err = pm.eval("new RangeError('to be raised in Python')")
+  assert isinstance(js_err, BaseException)
+  assert isinstance(js_err, Exception)
+  assert type(js_err) is pm.SpiderMonkeyError
+  with pytest.raises(pm.SpiderMonkeyError, match="RangeError: to be raised in Python"):
+    raise js_err
+
+  # convert Python Exception object to a JS Error object
+  get_err_msg = pm.eval("(err) => err.message")
+  assert "Python BufferError: ttt" == get_err_msg(BufferError("ttt"))
+  js_rethrow = pm.eval("(err) => { throw err }")
+  with pytest.raises(pm.SpiderMonkeyError, match="Error: Python BaseException: 123"):
+    js_rethrow(BaseException("123"))
+
 
 def test_eval_exceptions_nested_py_js_py():
-    def c():
-        raise Exception('this is an exception')
-    b = pm.eval('''(x) => {
-        try { 
-            x() 
+  def c():
+    raise Exception('this is an exception')
+  b = pm.eval('''(x) => {
+        try {
+            x()
         } catch(e) {
             return "Caught in JS " + e;
         }
     }''')
-    assert str(b(c)).__contains__("Caught in JS Error: Python Exception: this is an exception")
-    assert str(b(c)).__contains__("test_pythonmonkey_eval.py")
-    assert str(b(c)).__contains__("line 126")
-    assert str(b(c)).__contains__("in c")
+  assert str(b(c)).__contains__("Caught in JS Error: Python Exception: this is an exception")
+  assert str(b(c)).__contains__("test_pythonmonkey_eval.py")
+  assert str(b(c)).__contains__("line 140")
+  assert str(b(c)).__contains__("in c")
+
 
 def test_eval_exceptions_nested_js_py_js():
-    c = pm.eval("() => { throw TypeError('this is an exception'); }")
+  c = pm.eval("() => { throw TypeError('this is an exception'); }")
+
+  def b(x):
+    try:
+      x()
+      return ""
+    except Exception as e:
+      return "Caught in Py " + str(e)
+  ret = b(c)
+  assert ("Caught in Py Error in" in ret) and ("TypeError: this is an exception" in ret)
 
-    def b(x):
-        try:
-            x()
-            return ""
-        except Exception as e:
-            return "Caught in Py " + str(e)
-    ret = b(c)
-    assert ("Caught in Py Error in" in ret) and ("TypeError: this is an exception" in ret)
 
 def test_eval_undefined():
-    x = pm.eval("undefined")
-    assert x == None
+  x = pm.eval("undefined")
+  assert x is None
+
 
 def test_eval_null():
-    x = pm.eval("null")
-    assert x == pm.null
-    
+  x = pm.eval("null")
+  assert x == pm.null
+
+
 def test_eval_functions():
-    f = pm.eval("() => { return undefined }")
-    assert f() == None
+  f = pm.eval("() => { return undefined }")
+  assert f() is None
+
+  g = pm.eval("() => { return null}")
+  assert g() == pm.null
+
+  h = pm.eval("(a, b) => {return a + b}")
+  n = 10
+  for _ in range(n):
+    a = random.randint(-1000, 1000)
+    b = random.randint(-1000, 1000)
+    assert h(a, b) == (a + b)
+
+  for _ in range(n):
+    a = random.uniform(-1000.0, 1000.0)
+    b = random.uniform(-1000.0, 1000.0)
+    assert h(a, b) == (a + b)
 
-    g = pm.eval("() => { return null}")
-    assert g() == pm.null
+  assert math.isnan(h(float("nan"), 1))
+  assert math.isnan(h(float("+inf"), float("-inf")))
 
-    h = pm.eval("(a, b) => {return a + b}")
-    n = 10
-    for _ in range(n):
-        a = random.randint(-1000, 1000)
-        b = random.randint(-1000, 1000)
-        assert h(a, b) == (a + b)
-    
-    for _ in range (n):
-        a = random.uniform(-1000.0, 1000.0)
-        b = random.uniform(-1000.0, 1000.0)
-        assert h(a, b) == (a + b)
-    
-    assert math.isnan(h(float("nan"), 1))
-    assert math.isnan(h(float("+inf"), float("-inf")))
 
 def test_eval_functions_latin1_string_args():
-    concatenate = pm.eval("(a, b) => { return a + b}")
-    n = 10
-    for i in range(n):
-        length1 = random.randint(0x0000, 0xFFFF)
-        length2 = random.randint(0x0000, 0xFFFF)
-        string1 = ''
-        string2 = ''
-
-        for j in range(length1):
-            codepoint = random.randint(0x00, 0xFFFF)
-            string1 += chr(codepoint) # add random chr in ucs2 range
-        for j in range(length2):
-            codepoint = random.randint(0x00, 0xFFFF)
-            string2 += chr(codepoint)
-        
-        assert concatenate(string1, string2) == (string1 + string2)
+  concatenate = pm.eval("(a, b) => { return a + b}")
+  n = 10
+  for i in range(n):
+    length1 = random.randint(0x0000, 0xFFFF)
+    length2 = random.randint(0x0000, 0xFFFF)
+    string1 = ''
+    string2 = ''
+
+    for j in range(length1):
+      codepoint = random.randint(0x00, 0xFFFF)
+      string1 += chr(codepoint)  # add random chr in ucs2 range
+    for j in range(length2):
+      codepoint = random.randint(0x00, 0xFFFF)
+      string2 += chr(codepoint)
+
+    assert concatenate(string1, string2) == (string1 + string2)
+
 
 def test_eval_functions_ucs2_string_args():
-    concatenate = pm.eval("(a, b) => { return a + b}")
-    n = 10
-    for i in range(n):
-        length1 = random.randint(0x0000, 0xFFFF)
-        length2 = random.randint(0x0000, 0xFFFF)
-        string1 = ''
-        string2 = ''
-
-        for j in range(length1):
-            codepoint = random.randint(0x00, 0xFF)
-            string1 += chr(codepoint) # add random chr in latin1 range
-        for j in range(length2):
-            codepoint = random.randint(0x00, 0xFF)
-            string2 += chr(codepoint)
-        
-        assert concatenate(string1, string2) == (string1 + string2)
+  concatenate = pm.eval("(a, b) => { return a + b}")
+  n = 10
+  for i in range(n):
+    length1 = random.randint(0x0000, 0xFFFF)
+    length2 = random.randint(0x0000, 0xFFFF)
+    string1 = ''
+    string2 = ''
+
+    for j in range(length1):
+      codepoint = random.randint(0x00, 0xFF)
+      string1 += chr(codepoint)  # add random chr in latin1 range
+    for j in range(length2):
+      codepoint = random.randint(0x00, 0xFF)
+      string2 += chr(codepoint)
+
+    assert concatenate(string1, string2) == (string1 + string2)
+
 
 def test_eval_functions_ucs4_string_args():
-    concatenate = pm.eval("(a, b) => { return a + b}")
-    n = 10
-    for i in range(n):
-        length1 = random.randint(0x0000, 0xFFFF)
-        length2 = random.randint(0x0000, 0xFFFF)
-        string1 = ''
-        string2 = ''
-
-        for j in range(length1):
-            codepoint = random.randint(0x010000, 0x10FFFF)
-            string1 += chr(codepoint) # add random chr outside BMP
-        for j in range(length2):
-            codepoint = random.randint(0x010000, 0x10FFFF)
-            string2 += chr(codepoint)
-        
-        assert concatenate(string1, string2) == (string1 + string2)
+  concatenate = pm.eval("(a, b) => { return a + b}")
+  n = 10
+  for i in range(n):
+    length1 = random.randint(0x0000, 0xFFFF)
+    length2 = random.randint(0x0000, 0xFFFF)
+    string1 = ''
+    string2 = ''
+
+    for j in range(length1):
+      codepoint = random.randint(0x010000, 0x10FFFF)
+      string1 += chr(codepoint)  # add random chr outside BMP
+    for j in range(length2):
+      codepoint = random.randint(0x010000, 0x10FFFF)
+      string2 += chr(codepoint)
+
+    assert concatenate(string1, string2) == (string1 + string2)
+
 
 def test_eval_functions_roundtrip():
-    # BF-60 https://github.com/Distributive-Network/PythonMonkey/pull/18
-    def ident(x):
-        return x
-    js_fn_back = pm.eval("(py_fn) => py_fn(()=>{ return 'YYZ' })")(ident)
-    # pm.collect() # TODO: to be fixed in BF-59
-    assert "YYZ" == js_fn_back()
+  # BF-60 https://github.com/Distributive-Network/PythonMonkey/pull/18
+  def ident(x):
+    return x
+  js_fn_back = pm.eval("(py_fn) => py_fn(()=>{ return 'YYZ' })")(ident)
+  # pm.collect() # TODO: to be fixed in BF-59
+  assert "YYZ" == js_fn_back()
+
 
 def test_eval_functions_pyfunction_in_closure():
-    # BF-58 https://github.com/Distributive-Network/PythonMonkey/pull/19
-    def fn1():
-        def fn0(n):
-            return n + 100
-        return fn0
-    assert 101.9 == fn1()(1.9)
-    assert 101.9 == pm.eval("(fn1) => { return fn1 }")(fn1())(1.9)
-    assert 101.9 == pm.eval("(fn1, x) => { return fn1()(x) }")(fn1, 1.9)
-    assert 101.9 == pm.eval("(fn1) => { return fn1() }")(fn1)(1.9)
+  # BF-58 https://github.com/Distributive-Network/PythonMonkey/pull/19
+  def fn1():
+    def fn0(n):
+      return n + 100
+    return fn0
+  assert 101.9 == fn1()(1.9)
+  assert 101.9 == pm.eval("(fn1) => { return fn1 }")(fn1())(1.9)
+  assert 101.9 == pm.eval("(fn1, x) => { return fn1()(x) }")(fn1, 1.9)
+  assert 101.9 == pm.eval("(fn1) => { return fn1() }")(fn1)(1.9)
+
 
 def test_unwrap_py_function():
-    # https://github.com/Distributive-Network/PythonMonkey/issues/65
-    def pyFunc():
-        pass
-    unwrappedPyFunc = pm.eval("(wrappedPyFunc) => { return wrappedPyFunc }")(pyFunc)
-    assert unwrappedPyFunc is pyFunc
+  # https://github.com/Distributive-Network/PythonMonkey/issues/65
+  def pyFunc():
+    pass
+  unwrappedPyFunc = pm.eval("(wrappedPyFunc) => { return wrappedPyFunc }")(pyFunc)
+  assert unwrappedPyFunc is pyFunc
+
 
 def test_unwrap_js_function():
-    # https://github.com/Distributive-Network/PythonMonkey/issues/65
-    wrappedJSFunc = pm.eval("const JSFunc = () => { return 0 }\nJSFunc")
-    assert pm.eval("(unwrappedJSFunc) => { return unwrappedJSFunc === JSFunc }")(wrappedJSFunc)
+  # https://github.com/Distributive-Network/PythonMonkey/issues/65
+  wrappedJSFunc = pm.eval("const JSFunc = () => { return 0 }\nJSFunc")
+  assert pm.eval("(unwrappedJSFunc) => { return unwrappedJSFunc === JSFunc }")(wrappedJSFunc)
+
 
 def test_eval_functions_pyfunctions_ints():
-    caller = pm.eval("(func, param1, param2) => { return func(param1, param2) }")
-    def add(a, b):
-        return a + b
-    n = 10
-    for i in range(n):
-        int1 = random.randint(0x0000, 0xFFFF)
-        int2 = random.randint(0x0000, 0xFFFF)
-        assert caller(add, int1, int2) == int1 + int2
+  caller = pm.eval("(func, param1, param2) => { return func(param1, param2) }")
+
+  def add(a, b):
+    return a + b
+  n = 10
+  for i in range(n):
+    int1 = random.randint(0x0000, 0xFFFF)
+    int2 = random.randint(0x0000, 0xFFFF)
+    assert caller(add, int1, int2) == int1 + int2
+
 
 def test_eval_functions_pyfunctions_strs():
-    caller = pm.eval("(func, param1, param2) => { return func(param1, param2) }")
-    def concatenate(a, b):
-        return a + b
-    n = 10
-    for i in range(n):
-        length1 = random.randint(0x0000, 0xFFFF)
-        length2 = random.randint(0x0000, 0xFFFF)
-        string1 = ''
-        string2 = ''
-
-        for j in range(length1):
-            codepoint = random.randint(0x0000, 0xFFFF)
-            string1 += chr(codepoint) # add random chr
-        for j in range(length2):
-            codepoint = random.randint(0x0000, 0xFFFF)
-            string2 += chr(codepoint)
-        assert caller(concatenate, string1, string2) == string1 + string2  
+  caller = pm.eval("(func, param1, param2) => { return func(param1, param2) }")
+
+  def concatenate(a, b):
+    return a + b
+  n = 10
+  for i in range(n):
+    length1 = random.randint(0x0000, 0xFFFF)
+    length2 = random.randint(0x0000, 0xFFFF)
+    string1 = ''
+    string2 = ''
+
+    for j in range(length1):
+      codepoint = random.randint(0x0000, 0xFFFF)
+      string1 += chr(codepoint)  # add random chr
+    for j in range(length2):
+      codepoint = random.randint(0x0000, 0xFFFF)
+      string2 += chr(codepoint)
+    assert caller(concatenate, string1, string2) == string1 + string2
+
 
 def test_py_evaloptions_string_type():
-    evalOpts = {'filename': 'GoodFile'}     
-    try:
-        pm.eval("{throw new Error()}", evalOpts) 
-    except Exception as e:    
-        assert str(e).__contains__("Error in file GoodFile")           
+  evalOpts = {'filename': 'GoodFile'}
+  try:
+    pm.eval("{throw new Error()}", evalOpts)
+  except Exception as e:
+    assert str(e).__contains__("Error in file GoodFile")
+
 
 def test_js_evaloptions_string_type():
-    evalOpts = pm.eval("({'filename': 'GoodFile'})")  
-    try:
-        pm.eval("{throw new Error()}", evalOpts) 
-    except Exception as e:    
-        assert str(e).__contains__("Error in file GoodFile")        
+  evalOpts = pm.eval("({'filename': 'GoodFile'})")
+  try:
+    pm.eval("{throw new Error()}", evalOpts)
+  except Exception as e:
+    assert str(e).__contains__("Error in file GoodFile")
+
 
 def test_py_evaloptions_long_type():
-    evalOpts = {'lineno': 10}     
-    try:
-        pm.eval("{throw new Error()}", evalOpts) 
-    except Exception as e:    
-        assert str(e).__contains__("on line 10")           
+  evalOpts = {'lineno': 10}
+  try:
+    pm.eval("{throw new Error()}", evalOpts)
+  except Exception as e:
+    assert str(e).__contains__("on line 10")
+
 
 def test_js_evaloptions_long_type():
-    evalOpts = pm.eval("({'lineno': 10})")  
-    try:
-        pm.eval("{throw new Error()}", evalOpts) 
-    except Exception as e:    
-        assert str(e).__contains__("on line 10")     
+  evalOpts = pm.eval("({'lineno': 10})")
+  try:
+    pm.eval("{throw new Error()}", evalOpts)
+  except Exception as e:
+    assert str(e).__contains__("on line 10")
+
 
 def test_py_evaloptions_boolean_type():
-    evalOpts = {'strict': True}     
-    try:
-        pm.eval("{a = 9}", evalOpts) 
-    except Exception as e:    
-        assert str(e).__contains__("ReferenceError: assignment to undeclared variable a")           
+  evalOpts = {'strict': True}
+  try:
+    pm.eval("{a = 9}", evalOpts)
+  except Exception as e:
+    assert str(e).__contains__("ReferenceError: assignment to undeclared variable a")
+
 
 def test_js_evaloptions_boolean_type():
-    evalOpts = pm.eval("({'strict': true})")  
-    try:
-        pm.eval("{a = 9}", evalOpts) 
-    except Exception as e:    
-        assert str(e).__contains__("ReferenceError: assignment to undeclared variable a")
+  evalOpts = pm.eval("({'strict': true})")
+  try:
+    pm.eval("{a = 9}", evalOpts)
+  except Exception as e:
+    assert str(e).__contains__("ReferenceError: assignment to undeclared variable a")
+
 
 def test_globalThis():
-    obj = pm.eval('globalThis')
-    assert str(obj).__contains__("{'python': {'pythonMonkey':")
+  obj = pm.eval('globalThis')
+  assert str(obj).__contains__("{'python': {'pythonMonkey':")
+
 
 def test_console_globalThis():
-    temp_out = StringIO()
-    sys.stdout = temp_out
-    pm.eval('console.log(globalThis)')
-    assert temp_out.getvalue().__contains__("{ python: \n   { pythonMonkey: \n")    
+  temp_out = StringIO()
+  sys.stdout = temp_out
+  pm.eval('console.log(globalThis)')
+  assert temp_out.getvalue().__contains__("{ python: \n   { pythonMonkey: \n")
+
 
 def test_console_array():
-    temp_out = StringIO()
-    sys.stdout = temp_out
-    items = [1, 2, 3]
-    pm.eval('console.log')(items)
-    assert temp_out.getvalue() == "[ \x1b[33m1\x1b[39m, \x1b[33m2\x1b[39m, \x1b[33m3\x1b[39m ]\n"    
+  temp_out = StringIO()
+  sys.stdout = temp_out
+  items = [1, 2, 3]
+  pm.eval('console.log')(items)
+  assert temp_out.getvalue() == "[ \x1b[33m1\x1b[39m, \x1b[33m2\x1b[39m, \x1b[33m3\x1b[39m ]\n"
```

### Comparing `pythonmonkey-0.4.0/tests/python/test_reentrance_smoke.py` & `pythonmonkey-0.6.0/tests/python/test_reentrance_smoke.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # @file         reentrance-smoke.py
 #               Basic smoke test which shows that JS->Python->JS->Python calls work. Failures are
 #               indicated by segfaults.
 # @author       Wes Garland, wes@distributive.network
 # @date         June 2023
 
-import sys, os
+import sys
+import os
 import pythonmonkey as pm
 
 
 def test_reentrance():
-    globalThis = pm.eval("globalThis;");
-    globalThis.pmEval = pm.eval;
-    globalThis.pyEval = eval;
+  globalThis = pm.eval("globalThis;")
+  globalThis.pmEval = pm.eval
+  globalThis.pyEval = eval
 
-    abc=(pm.eval("() => { return {def: pyEval('123')} };"))()
-    assert(abc['def'] == 123)
-    print(pm.eval("pmEval(`pyEval(\"'test passed'\")`)"))
+  abc = (pm.eval("() => { return {def: pyEval('123')} };"))()
+  assert (abc['def'] == 123)
+  print(pm.eval("pmEval(`pyEval(\"'test passed'\")`)"))
```

### Comparing `pythonmonkey-0.4.0/tests/python/test_strings.py` & `pythonmonkey-0.6.0/tests/python/test_strings.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,256 +1,267 @@
 import pythonmonkey as pm
 import gc
 import random
 
+
 def test_eval_ascii_string_matches_evaluated_string():
-    py_ascii_string = "abc"
-    js_ascii_string = pm.eval(repr(py_ascii_string))
-    assert py_ascii_string == js_ascii_string
+  py_ascii_string = "abc"
+  js_ascii_string = pm.eval(repr(py_ascii_string))
+  assert py_ascii_string == js_ascii_string
+
 
 def test_eval_latin1_string_matches_evaluated_string():
-    py_latin1_string = "a©Ð"
-    js_latin1_string = pm.eval(repr(py_latin1_string))
-    assert py_latin1_string == js_latin1_string
+  py_latin1_string = "a©Ð"
+  js_latin1_string = pm.eval(repr(py_latin1_string))
+  assert py_latin1_string == js_latin1_string
+
 
 def test_eval_null_character_string_matches_evaluated_string():
-    py_null_character_string = "a\x00©"
-    js_null_character_string = pm.eval(repr(py_null_character_string))
-    assert py_null_character_string == js_null_character_string
+  py_null_character_string = "a\x00©"
+  js_null_character_string = pm.eval(repr(py_null_character_string))
+  assert py_null_character_string == js_null_character_string
+
 
 def test_eval_ucs2_string_matches_evaluated_string():
-    py_ucs2_string = "ՄԸՋ"
-    js_ucs2_string = pm.eval(repr(py_ucs2_string))
-    assert py_ucs2_string == js_ucs2_string
+  py_ucs2_string = "ՄԸՋ"
+  js_ucs2_string = pm.eval(repr(py_ucs2_string))
+  assert py_ucs2_string == js_ucs2_string
+
 
 def test_eval_unpaired_surrogate_string_matches_evaluated_string():
-    py_unpaired_surrogate_string = "Ջ©\ud8fe"
-    js_unpaired_surrogate_string = pm.eval(repr(py_unpaired_surrogate_string))
-    assert py_unpaired_surrogate_string == js_unpaired_surrogate_string
+  py_unpaired_surrogate_string = "Ջ©\ud8fe"
+  js_unpaired_surrogate_string = pm.eval(repr(py_unpaired_surrogate_string))
+  assert py_unpaired_surrogate_string == js_unpaired_surrogate_string
+
 
 def test_eval_ucs4_string_matches_evaluated_string():
-    py_ucs4_string = "🀄🀛🜢"
-    js_ucs4_string = pm.eval(repr(py_ucs4_string))
-    assert py_ucs4_string == js_ucs4_string
+  py_ucs4_string = "🀄🀛🜢"
+  js_ucs4_string = pm.eval(repr(py_ucs4_string))
+  assert py_ucs4_string == js_ucs4_string
+
 
 def test_eval_latin1_string_fuzztest():
-    n = 10
-    for _ in range(n):
-        length = random.randint(0x0000, 0xFFFF)
-        string1 = ''
-
-        for _ in range(length):
-            codepoint = random.randint(0x00, 0xFF)
-            string1 += chr(codepoint) # add random chr in latin1 range
-        
-        
-        INITIAL_STRING = string1
-        m = 10
-        for _ in range(m):
-            string2 = pm.eval(repr(string1))
-            assert len(string1) == length
-            assert len(string2) == length
-            assert len(string1) == len(string2)
-            assert string1 == string2
-
-            gc.collect()
-            pm.collect()
-            
-            #garbage collection should not collect variables still in scope
-            assert len(string1) == length
-            assert len(string2) == length
-            assert len(string1) == len(string2)
-            assert string1 == string2
+  n = 10
+  for _ in range(n):
+    length = random.randint(0x0000, 0xFFFF)
+    string1 = ''
+
+    for _ in range(length):
+      codepoint = random.randint(0x00, 0xFF)
+      string1 += chr(codepoint)  # add random chr in latin1 range
+
+    INITIAL_STRING = string1
+    m = 10
+    for _ in range(m):
+      string2 = pm.eval(repr(string1))
+      assert len(string1) == length
+      assert len(string2) == length
+      assert len(string1) == len(string2)
+      assert string1 == string2
+
+      gc.collect()
+      pm.collect()
+
+      # garbage collection should not collect variables still in scope
+      assert len(string1) == length
+      assert len(string2) == length
+      assert len(string1) == len(string2)
+      assert string1 == string2
+
+      string1 = string2
+    assert INITIAL_STRING == string1  # strings should still match after a bunch of iterations through JS
 
-            string1 = string2
-        assert INITIAL_STRING == string1 #strings should still match after a bunch of iterations through JS
 
 def test_eval_ucs2_string_fuzztest():
-    n = 10
-    for _ in range(n):
-        length = random.randint(0x0000, 0xFFFF)
-        string1 = ''
-
-        for _i in range(length):
-            codepoint = random.randint(0x00, 0xFFFF)
-            string1 += chr(codepoint) # add random chr in ucs2 range
-        
-        
-        INITIAL_STRING = string1
-        m = 10
-        for _ in range(m):
-            string2 = pm.eval(repr(string1))
-            assert len(string1) == length
-            assert len(string2) == length
-            assert len(string1) == len(string2)
-            assert string1 == string2
-
-            gc.collect()
-            pm.collect()
-            
-            #garbage collection should not collect variables still in scope
-            assert len(string1) == length
-            assert len(string2) == length
-            assert len(string1) == len(string2)
-            assert string1 == string2
+  n = 10
+  for _ in range(n):
+    length = random.randint(0x0000, 0xFFFF)
+    string1 = ''
+
+    for _i in range(length):
+      codepoint = random.randint(0x00, 0xFFFF)
+      string1 += chr(codepoint)  # add random chr in ucs2 range
+
+    INITIAL_STRING = string1
+    m = 10
+    for _ in range(m):
+      string2 = pm.eval(repr(string1))
+      assert len(string1) == length
+      assert len(string2) == length
+      assert len(string1) == len(string2)
+      assert string1 == string2
+
+      gc.collect()
+      pm.collect()
+
+      # garbage collection should not collect variables still in scope
+      assert len(string1) == length
+      assert len(string2) == length
+      assert len(string1) == len(string2)
+      assert string1 == string2
+
+      string1 = string2
+    assert INITIAL_STRING == string1  # strings should still match after a bunch of iterations through JS
 
-            string1 = string2
-        assert INITIAL_STRING == string1 #strings should still match after a bunch of iterations through JS
 
 def test_eval_ucs4_string_fuzztest():
-    n = 10
-    for _ in range(n):
-        length = random.randint(0x0000, 0xFFFF)
-        string1 = ''
-
-        for _ in range(length):
-            codepoint = random.randint(0x010000, 0x10FFFF)
-            string1 += chr(codepoint) # add random chr outside BMP
-        
-        
-        INITIAL_STRING = string1
-        m = 10
-        for _ in range(m):
-            string2 = pm.eval("'" + string1 + "'")
-            assert len(string1) == length
-            assert len(string2) == length
-            assert len(string1) == len(string2)
-            assert string1 == string2
-
-            gc.collect()
-            pm.collect()
-            
-            #garbage collection should not collect variables still in scope
-            assert len(string1) == length
-            assert len(string2) == length
-            assert len(string1) == len(string2)
-            assert string1 == string2
+  n = 10
+  for _ in range(n):
+    length = random.randint(0x0000, 0xFFFF)
+    string1 = ''
+
+    for _ in range(length):
+      codepoint = random.randint(0x010000, 0x10FFFF)
+      string1 += chr(codepoint)  # add random chr outside BMP
+
+    INITIAL_STRING = string1
+    m = 10
+    for _ in range(m):
+      string2 = pm.eval("'" + string1 + "'")
+      assert len(string1) == length
+      assert len(string2) == length
+      assert len(string1) == len(string2)
+      assert string1 == string2
+
+      gc.collect()
+      pm.collect()
+
+      # garbage collection should not collect variables still in scope
+      assert len(string1) == length
+      assert len(string2) == length
+      assert len(string1) == len(string2)
+      assert string1 == string2
 
-            string1 = string2
-        assert INITIAL_STRING == string1 #strings should still match after a bunch of iterations through JS
+      string1 = string2
+    assert INITIAL_STRING == string1  # strings should still match after a bunch of iterations through JS
 
 
 def test_eval_boxed_ascii_string_matches_evaluated_string():
-    py_ascii_string = "abc"
-    js_ascii_string = pm.eval(f'new String({repr(py_ascii_string)})')
-    assert py_ascii_string == js_ascii_string
+  py_ascii_string = "abc"
+  js_ascii_string = pm.eval(f'new String({repr(py_ascii_string)})')
+  assert py_ascii_string == js_ascii_string
+
 
 def test_eval_boxed_latin1_string_matches_evaluated_string():
-    py_latin1_string = "a©Ð"
-    js_latin1_string = pm.eval(f'new String({repr(py_latin1_string)})')
-    assert py_latin1_string == js_latin1_string
+  py_latin1_string = "a©Ð"
+  js_latin1_string = pm.eval(f'new String({repr(py_latin1_string)})')
+  assert py_latin1_string == js_latin1_string
+
 
 def test_eval_boxed_null_character_string_matches_evaluated_string():
-    py_null_character_string = "a\x00©"
-    js_null_character_string = pm.eval(f'new String({repr(py_null_character_string)})')
-    assert py_null_character_string == js_null_character_string
+  py_null_character_string = "a\x00©"
+  js_null_character_string = pm.eval(f'new String({repr(py_null_character_string)})')
+  assert py_null_character_string == js_null_character_string
+
 
 def test_eval_boxed_ucs2_string_matches_evaluated_string():
-    py_ucs2_string = "ՄԸՋ"
-    js_ucs2_string = pm.eval(f'new String({repr(py_ucs2_string)})')
-    assert py_ucs2_string == js_ucs2_string
+  py_ucs2_string = "ՄԸՋ"
+  js_ucs2_string = pm.eval(f'new String({repr(py_ucs2_string)})')
+  assert py_ucs2_string == js_ucs2_string
+
 
 def test_eval_boxed_unpaired_surrogate_string_matches_evaluated_string():
-    py_unpaired_surrogate_string = "Ջ©\ud8fe"
-    js_unpaired_surrogate_string = pm.eval(f'new String({repr(py_unpaired_surrogate_string)})')
-    assert py_unpaired_surrogate_string == js_unpaired_surrogate_string
+  py_unpaired_surrogate_string = "Ջ©\ud8fe"
+  js_unpaired_surrogate_string = pm.eval(f'new String({repr(py_unpaired_surrogate_string)})')
+  assert py_unpaired_surrogate_string == js_unpaired_surrogate_string
+
 
 def test_eval_boxed_ucs4_string_matches_evaluated_string():
-    py_ucs4_string = "🀄🀛🜢"
-    js_ucs4_string = pm.eval(f'new String({repr(py_ucs4_string)})')
-    assert py_ucs4_string == js_ucs4_string
+  py_ucs4_string = "🀄🀛🜢"
+  js_ucs4_string = pm.eval(f'new String({repr(py_ucs4_string)})')
+  assert py_ucs4_string == js_ucs4_string
+
 
 def test_eval_boxed_latin1_string_fuzztest():
-    n = 10
-    for _ in range(n):
-        length = random.randint(0x0000, 0xFFFF)
-        string1 = ''
-
-        for _ in range(length):
-            codepoint = random.randint(0x00, 0xFF)
-            string1 += chr(codepoint) # add random chr in latin1 range
-        
-        
-        INITIAL_STRING = string1
-        m = 10
-        for _ in range(m):
-            string2 = pm.eval(f'new String({repr(string1)})')
-            assert len(string1) == length
-            assert len(string2) == length
-            assert len(string1) == len(string2)
-            assert string1 == string2
-
-            gc.collect()
-            pm.collect()
-            
-            #garbage collection should not collect variables still in scope
-            assert len(string1) == length
-            assert len(string2) == length
-            assert len(string1) == len(string2)
-            assert string1 == string2
+  n = 10
+  for _ in range(n):
+    length = random.randint(0x0000, 0xFFFF)
+    string1 = ''
+
+    for _ in range(length):
+      codepoint = random.randint(0x00, 0xFF)
+      string1 += chr(codepoint)  # add random chr in latin1 range
+
+    INITIAL_STRING = string1
+    m = 10
+    for _ in range(m):
+      string2 = pm.eval(f'new String({repr(string1)})')
+      assert len(string1) == length
+      assert len(string2) == length
+      assert len(string1) == len(string2)
+      assert string1 == string2
+
+      gc.collect()
+      pm.collect()
+
+      # garbage collection should not collect variables still in scope
+      assert len(string1) == length
+      assert len(string2) == length
+      assert len(string1) == len(string2)
+      assert string1 == string2
+
+      string1 = string2
+    assert INITIAL_STRING == string1  # strings should still match after a bunch of iterations through JS
 
-            string1 = string2
-        assert INITIAL_STRING == string1 #strings should still match after a bunch of iterations through JS
 
 def test_eval_boxed_ucs2_string_fuzztest():
-    n = 10
-    for _ in range(n):
-        length = random.randint(0x0000, 0xFFFF)
-        string1 = ''
-
-        for _ in range(length):
-            codepoint = random.randint(0x00, 0xFFFF)
-            string1 += chr(codepoint) # add random chr in ucs2 range
-        
-        
-        INITIAL_STRING = string1
-        m = 10
-        for _ in range(m):
-            string2 = pm.eval(f'new String({repr(string1)})')
-            assert len(string1) == length
-            assert len(string2) == length
-            assert len(string1) == len(string2)
-            assert string1 == string2
-
-            gc.collect()
-            pm.collect()
-            
-            #garbage collection should not collect variables still in scope
-            assert len(string1) == length
-            assert len(string2) == length
-            assert len(string1) == len(string2)
-            assert string1 == string2
+  n = 10
+  for _ in range(n):
+    length = random.randint(0x0000, 0xFFFF)
+    string1 = ''
+
+    for _ in range(length):
+      codepoint = random.randint(0x00, 0xFFFF)
+      string1 += chr(codepoint)  # add random chr in ucs2 range
+
+    INITIAL_STRING = string1
+    m = 10
+    for _ in range(m):
+      string2 = pm.eval(f'new String({repr(string1)})')
+      assert len(string1) == length
+      assert len(string2) == length
+      assert len(string1) == len(string2)
+      assert string1 == string2
+
+      gc.collect()
+      pm.collect()
+
+      # garbage collection should not collect variables still in scope
+      assert len(string1) == length
+      assert len(string2) == length
+      assert len(string1) == len(string2)
+      assert string1 == string2
+
+      string1 = string2
+    assert INITIAL_STRING == string1  # strings should still match after a bunch of iterations through JS
 
-            string1 = string2
-        assert INITIAL_STRING == string1 #strings should still match after a bunch of iterations through JS
 
 def test_eval_boxed_ucs4_string_fuzztest():
-    n = 10
-    for _ in range(n):
-        length = random.randint(0x0000, 0xFFFF)
-        string1 = ''
-
-        for _ in range(length):
-            codepoint = random.randint(0x010000, 0x10FFFF)
-            string1 += chr(codepoint) # add random chr outside BMP
-        
-        
-        INITIAL_STRING = string1
-        m = 10
-        for _ in range(m):
-            string2 = pm.eval(f'new String("{string1}")')
-            assert len(string1) == length
-            assert len(string2) == length
-            assert len(string1) == len(string2)
-            assert string1 == string2
-
-            gc.collect()
-            pm.collect()
-            
-            #garbage collection should not collect variables still in scope
-            assert len(string1) == length
-            assert len(string2) == length
-            assert len(string1) == len(string2)
-            assert string1 == string2
+  n = 10
+  for _ in range(n):
+    length = random.randint(0x0000, 0xFFFF)
+    string1 = ''
+
+    for _ in range(length):
+      codepoint = random.randint(0x010000, 0x10FFFF)
+      string1 += chr(codepoint)  # add random chr outside BMP
+
+    INITIAL_STRING = string1
+    m = 10
+    for _ in range(m):
+      string2 = pm.eval(f'new String("{string1}")')
+      assert len(string1) == length
+      assert len(string2) == length
+      assert len(string1) == len(string2)
+      assert string1 == string2
+
+      gc.collect()
+      pm.collect()
+
+      # garbage collection should not collect variables still in scope
+      assert len(string1) == length
+      assert len(string2) == length
+      assert len(string1) == len(string2)
+      assert string1 == string2
 
-            string1 = string2
-        assert INITIAL_STRING == string1 #strings should still match after a bunch of iterations through JS
+      string1 = string2
+    assert INITIAL_STRING == string1  # strings should still match after a bunch of iterations through JS
```

### Comparing `pythonmonkey-0.4.0/PKG-INFO` & `pythonmonkey-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: pythonmonkey
-Version: 0.4.0
+Version: 0.6.0
 Summary: 
 Author: Caleb Aikens
 Author-email: caleb@distributive.network
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: aiohttp[speedups] (>=3.9.3,<4.0.0)
-Requires-Dist: pminit
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: aiohttp[speedups] (>=3.9.5,<4.0.0)
+Requires-Dist: pminit (>=0.4.0)
 Requires-Dist: pyreadline3 (>=3.4.1,<4.0.0) ; sys_platform == "win32"
 Description-Content-Type: text/markdown
 
 # PythonMonkey
 
 ![Testing Suite](https://github.com/Kings-Distributed-Systems/PythonMonkey/actions/workflows/tests.yaml/badge.svg)
 
@@ -91,15 +92,21 @@
     - rust
     - python3.8 or later with header files (python3-dev)
     - spidermonkey 115.1.0 or later
     - npm (nodejs)
     - [Poetry](https://python-poetry.org/docs/#installation)
     - [poetry-dynamic-versioning](https://github.com/mtkennerly/poetry-dynamic-versioning)
 
-2. Run `poetry install`. This command automatically compiles the project and installs the project as well as dependencies into the poetry virtualenv.
+2. Run `poetry install`. This command automatically compiles the project and installs the project as well as dependencies into the poetry virtualenv. If you would like to build the docs, set the `BUILD_DOCS` environment variable, like so: `BUILD_DOCS=1 poetry install`.
+PythonMonkey supports multiple build types, which you can build by setting the `BUILD_TYPE` environment variable, like so: `BUILD_TYPE=Debug poetry install`. The build types are (case-insensitive):
+- `Release`: stripped symbols, maximum optimizations (default)
+- `DRelease`: same as `Release`, except symbols are not stripped
+- `Debug`: minimal optimizations
+- `Profile`: same as `Debug`, except profiling is enabled 
+- `None`: don't compile (useful if you only want to build the docs)
 
 If you are using VSCode, you can just press <kbd>Ctrl</kbd> + <kbd>Shift</kbd> + <kbd>B</kbd> to [run build task](https://code.visualstudio.com/docs/editor/tasks#_custom-tasks) - We have [the `tasks.json` file configured for you](.vscode/tasks.json).
 
 ## Running tests
 1. Compile the project
 2. Install development dependencies: `poetry install --no-root --only=dev`
 3. From the root directory, run `poetry run pytest ./tests/python`
```

