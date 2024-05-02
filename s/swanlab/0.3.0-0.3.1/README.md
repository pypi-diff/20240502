# Comparing `tmp/swanlab-0.3.0.tar.gz` & `tmp/swanlab-0.3.1.tar.gz`

## Comparing `swanlab-0.3.0.tar` & `swanlab-0.3.1.tar`

### file list

```diff
@@ -1,817 +1,817 @@
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 swanlab-0.3.0/.eslintrc-auto-import.json
--rw-r--r--   0        0        0    26391 2020-02-02 00:00:00.000000 swanlab-0.3.0/README.md
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 swanlab-0.3.0/jsconfig.json
--rw-r--r--   0        0        0   235750 2020-02-02 00:00:00.000000 swanlab-0.3.0/package-lock.json
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 swanlab-0.3.0/package.json
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 swanlab-0.3.0/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swanlab-0.3.0/.config/copy_frontend.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 swanlab-0.3.0/.vscode/extensions.json
--rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 swanlab-0.3.0/.vscode/launch.json
--rw-r--r--   0        0        0     3112 2020-02-02 00:00:00.000000 swanlab-0.3.0/.vscode/settings.json
--rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 swanlab-0.3.0/.vscode/tailwind.json
--rw-r--r--   0        0        0   217919 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/.package-lock.json
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@alloc/quick-lru/package.json
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@antfu/utils/package.json
--rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@antv/adjust/package.json
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@antv/adjust/node_modules/tslib/package.json
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@antv/adjust/node_modules/tslib/modules/package.json
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@antv/adjust/node_modules/tslib/test/validateModuleExportsMatchCommonJS/package.json
--rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@antv/attr/package.json
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@antv/color-util/package.json
--rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@antv/component/package.json
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@antv/component/node_modules/@antv/path-util/package.json
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@antv/component/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@antv/coord/package.json
--rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@antv/dom-util/package.json
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@antv/event-emitter/package.json
--rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@antv/g-base/package.json
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@antv/g-base/node_modules/@antv/path-util/package.json
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@antv/g-base/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json
--rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@antv/g-canvas/package.json
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@antv/g-canvas/node_modules/@antv/path-util/package.json
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@antv/g-canvas/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@antv/g-math/package.json
--rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@antv/g-svg/package.json
--rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@antv/g2/package.json
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@antv/g2/node_modules/@antv/path-util/package.json
--rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@antv/g2/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json
--rw-r--r--   0        0        0     3969 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@antv/g2plot/package.json
--rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@antv/matrix-util/package.json
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@antv/path-util/package.json
--rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@antv/scale/package.json
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@antv/util/package.json
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@babel/parser/package.json
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@esbuild/linux-x64/package.json
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@eslint/eslintrc/package.json
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@eslint/js/package.json
--rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@eslint-community/eslint-utils/package.json
--rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@eslint-community/regexpp/package.json
--rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@headlessui/vue/package.json
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@humanwhocodes/config-array/package.json
--rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@humanwhocodes/module-importer/package.json
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@humanwhocodes/object-schema/package.json
--rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@intlify/core-base/package.json
--rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@intlify/message-compiler/package.json
--rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@intlify/shared/package.json
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@isaacs/cliui/package.json
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@isaacs/cliui/node_modules/ansi-regex/package.json
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@isaacs/cliui/node_modules/strip-ansi/package.json
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@jest/schemas/package.json
--rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@jridgewell/gen-mapping/package.json
--rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@jridgewell/resolve-uri/package.json
--rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@jridgewell/set-array/package.json
--rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@jridgewell/source-map/package.json
--rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@jridgewell/sourcemap-codec/package.json
--rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@jridgewell/trace-mapping/package.json
--rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@ljharb/resumer/package.json
--rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@ljharb/through/package.json
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@ljharb/through/tsconfig.json
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@nodelib/fs.scandir/package.json
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@nodelib/fs.stat/package.json
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@nodelib/fs.walk/package.json
--rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@pkgjs/parseargs/package.json
--rw-r--r--   0        0        0     4230 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@popperjs/core/package.json
--rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@rollup/pluginutils/package.json
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@rollup/pluginutils/dist/es/package.json
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@rollup/rollup-linux-x64-gnu/package.json
--rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@rollup/rollup-linux-x64-musl/package.json
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@sinclair/typebox/package.json
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@tanstack/virtual-core/package.json
--rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@tanstack/vue-virtual/package.json
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@types/d3-timer/package.json
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@types/estree/package.json
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@ungap/structured-clone/package.json
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@ungap/structured-clone/cjs/package.json
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@vitejs/plugin-vue/package.json
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@vitest/expect/package.json
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@vitest/runner/package.json
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@vitest/runner/node_modules/p-limit/package.json
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@vitest/runner/node_modules/yocto-queue/package.json
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@vitest/snapshot/package.json
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@vitest/spy/package.json
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@vitest/utils/package.json
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@vitest/utils/node_modules/estree-walker/package.json
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@vue/compiler-core/package.json
--rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@vue/compiler-dom/package.json
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@vue/compiler-sfc/package.json
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@vue/compiler-ssr/package.json
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@vue/devtools-api/package.json
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@vue/reactivity/package.json
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@vue/runtime-core/package.json
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@vue/runtime-dom/package.json
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@vue/server-renderer/package.json
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/@vue/shared/package.json
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/acorn/package.json
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/acorn-jsx/package.json
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/acorn-walk/package.json
--rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/ajv/package.json
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/ajv/lib/refs/data.json
--rw-r--r--   0        0        0     4357 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/ajv/lib/refs/json-schema-draft-04.json
--rw-r--r--   0        0        0     4445 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/ajv/lib/refs/json-schema-draft-06.json
--rw-r--r--   0        0        0     4879 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/ajv/lib/refs/json-schema-draft-07.json
--rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/ajv/lib/refs/json-schema-secure.json
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/align-text/package.json
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/amdefine/package.json
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/ansi-regex/package.json
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/ansi-styles/package.json
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/any-promise/package.json
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/anymatch/package.json
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/arg/package.json
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/argparse/package.json
--rw-r--r--   0        0        0     2473 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/array-buffer-byte-length/package.json
--rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/array-buffer-byte-length/tsconfig.json
--rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/arraybuffer.prototype.slice/package.json
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/assertion-error/package.json
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/asynckit/package.json
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/autoprefixer/package.json
--rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/available-typed-arrays/package.json
--rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/available-typed-arrays/tsconfig.json
--rw-r--r--   0        0        0     7633 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/axios/package.json
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/balanced-match/package.json
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/binary-extensions/binary-extensions.json
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/binary-extensions/package.json
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/boolbase/package.json
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/brace-expansion/package.json
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/braces/package.json
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/browserslist/package.json
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/buffer-from/package.json
--rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/cac/package.json
--rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/call-bind/package.json
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/callsites/package.json
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/camelcase/package.json
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/camelcase-css/package.json
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/caniuse-lite/package.json
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/center-align/package.json
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/chai/bower.json
--rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/chai/package.json
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/chalk/package.json
--rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/check-error/package.json
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/chokidar/package.json
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/chokidar/node_modules/glob-parent/package.json
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/cliui/package.json
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/color-convert/package.json
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/color-name/package.json
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/combined-stream/package.json
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/commander/package-support.json
--rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/commander/package.json
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/concat-map/package.json
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/confbox/package.json
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/contour_plot/package.json
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/cross-spawn/package.json
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/cssesc/package.json
--rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/csstype/package.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/d3-color/package.json
--rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/d3-ease/package.json
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/d3-hierarchy/package.json
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/d3-interpolate/package.json
--rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/d3-regression/package.json
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/d3-timer/package.json
--rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/data-view-buffer/package.json
--rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/data-view-buffer/tsconfig.json
--rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/data-view-byte-length/package.json
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/data-view-byte-length/tsconfig.json
--rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/data-view-byte-offset/package.json
--rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/data-view-byte-offset/tsconfig.json
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/debug/package.json
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/decamelize/package.json
--rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/deep-eql/package.json
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/deep-equal/package.json
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/deep-is/package.json
--rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/define-data-property/package.json
--rw-r--r--   0        0        0     4883 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/define-data-property/tsconfig.json
--rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/define-properties/package.json
--rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/defined/package.json
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/delayed-stream/package.json
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/detect-browser/package.json
--rwxr-xr-x   0        0        0      647 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/didyoumean/package.json
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/diff-sequences/package.json
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/dlv/package.json
--rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/doctrine/package.json
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/dotignore/package.json
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/eastasianwidth/package.json
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/electron-to-chromium/chromium-versions.json
--rw-r--r--   0        0        0    49626 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/electron-to-chromium/full-chromium-versions.json
--rw-r--r--   0        0        0    77590 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/electron-to-chromium/full-versions.json
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/electron-to-chromium/package.json
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/electron-to-chromium/versions.json
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/emoji-regex/package.json
--rw-r--r--   0        0        0     2883 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/entities/package.json
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/entities/lib/esm/package.json
--rw-r--r--   0        0        0     4929 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/es-abstract/package.json
--rw-r--r--   0        0        0    22346 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/es-abstract/helpers/caseFolding.json
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/es-abstract/node_modules/object-inspect/package-support.json
--rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/es-abstract/node_modules/object-inspect/package.json
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/es-define-property/package.json
--rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/es-define-property/tsconfig.json
--rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/es-errors/package.json
--rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/es-errors/tsconfig.json
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/es-object-atoms/package.json
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/es-object-atoms/tsconfig.json
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/es-set-tostringtag/package.json
--rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/es-set-tostringtag/tsconfig.json
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/es-to-primitive/package.json
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/esbuild/package.json
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/escalade/package.json
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/escape-string-regexp/package.json
--rw-r--r--   0        0        0     5566 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/eslint/package.json
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/eslint/conf/replacements.json
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/eslint/conf/rule-type-list.json
--rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/eslint/lib/cli-engine/formatters/formatters-meta.json
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/eslint-config-prettier/package.json
--rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/eslint-plugin-prettier/package.json
--rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/eslint-plugin-vue/package.json
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/eslint-plugin-vue/lib/utils/deprecated-html-elements.json
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/eslint-plugin-vue/lib/utils/html-elements.json
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/eslint-plugin-vue/lib/utils/inline-non-void-elements.json
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/eslint-plugin-vue/lib/utils/js-reserved.json
--rw-r--r--   0        0        0     5270 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/eslint-plugin-vue/lib/utils/key-aliases.json
--rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/eslint-plugin-vue/lib/utils/svg-attributes-weird-case.json
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/eslint-plugin-vue/lib/utils/svg-elements.json
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/eslint-plugin-vue/lib/utils/void-elements.json
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/eslint-plugin-vue/lib/utils/vue-component-options.json
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/eslint-plugin-vue/lib/utils/vue-reserved.json
--rw-r--r--   0        0        0     6650 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/eslint-plugin-vue/lib/utils/vue3-export-names.json
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/eslint-scope/package.json
--rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/eslint-visitor-keys/package.json
--rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/espree/package.json
--rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/esquery/package.json
--rwxr-xr-x   0        0        0     1165 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/esrecurse/package.json
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/estraverse/package.json
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/estree-walker/package.json
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/estree-walker/dist/esm/package.json
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/estree-walker/src/package.json
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/esutils/package.json
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/execa/package.json
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/fast-deep-equal/package.json
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/fast-diff/package.json
--rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/fast-glob/package.json
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/fast-glob/node_modules/glob-parent/package.json
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/fast-json-stable-stringify/package.json
--rw-r--r--   0        0        0     3828 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/fast-json-stable-stringify/benchmark/test.json
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/fast-levenshtein/package.json
--rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/fastq/package.json
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/fastq/test/tsconfig.json
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/fecha/package.json
--rw-r--r--   0        0        0     2756 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/file-entry-cache/package.json
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/fill-range/package.json
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/find-up/package.json
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/flat-cache/package.json
--rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/flatted/package.json
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/flatted/cjs/package.json
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/fmin/.eslintrc.json
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/fmin/package.json
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/follow-redirects/package.json
--rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/for-each/package.json
--rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/foreground-child/package.json
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/foreground-child/dist/cjs/package.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/foreground-child/dist/mjs/package.json
--rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/form-data/package.json
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/fraction.js/package.json
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/fs.realpath/package.json
--rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/function-bind/package.json
--rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/function.prototype.name/package.json
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/functions-have-names/package.json
--rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/get-func-name/package.json
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/get-intrinsic/package.json
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/get-stream/package.json
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/get-symbol-description/package.json
--rwxr-xr-x   0        0        0      630 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/gl-matrix/package.json
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/gl-matrix/mat2/package.json
--rwxr-xr-x   0        0        0       91 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/gl-matrix/mat2d/package.json
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/gl-matrix/mat3/package.json
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/gl-matrix/mat4/package.json
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/gl-matrix/quat/package.json
--rwxr-xr-x   0        0        0       91 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/gl-matrix/quat2/package.json
--rwxr-xr-x   0        0        0      100 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/gl-matrix/types.d.ts/package.json
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/gl-matrix/vec2/package.json
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/gl-matrix/vec3/package.json
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/gl-matrix/vec4/package.json
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/glob/package.json
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/glob-parent/package.json
--rw-r--r--   0        0        0    48140 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/globals/globals.json
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/globals/package.json
--rw-r--r--   0        0        0     2418 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/globalthis/package.json
--rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/gopd/package.json
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/graphemer/package.json
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/has/package.json
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/has-ansi/package.json
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/has-ansi/node_modules/ansi-regex/package.json
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/has-bigints/package.json
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/has-flag/package.json
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/has-property-descriptors/package.json
--rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/has-proto/package.json
--rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/has-proto/tsconfig.json
--rw-r--r--   0        0        0     2648 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/has-symbols/package.json
--rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/has-tostringtag/package.json
--rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/has-tostringtag/tsconfig.json
--rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/hasown/package.json
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/hasown/tsconfig.json
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/human-signals/package.json
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/husky/package.json
--rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/ignore/package.json
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/immutable/package.json
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/import-fresh/package.json
--rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/imurmurhash/package.json
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/inflight/package.json
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/inherits/package.json
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/internal-slot/package.json
--rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/is-arguments/package.json
--rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/is-array-buffer/package.json
--rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/is-array-buffer/tsconfig.json
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/is-bigint/package.json
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/is-binary-path/package.json
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/is-boolean-object/package.json
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/is-buffer/package.json
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/is-callable/package.json
--rw-r--r--   0        0        0     5769 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/is-core-module/core.json
--rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/is-core-module/package.json
--rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/is-data-view/package.json
--rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/is-data-view/tsconfig.json
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/is-date-object/package.json
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/is-extglob/package.json
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/is-fullwidth-code-point/package.json
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/is-glob/package.json
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/is-negative-zero/package.json
--rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/is-negative-zero/tsconfig.json
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/is-number/package.json
--rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/is-number-object/package.json
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/is-path-inside/package.json
--rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/is-regex/package.json
--rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/is-shared-array-buffer/package.json
--rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/is-shared-array-buffer/tsconfig.json
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/is-stream/package.json
--rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/is-string/package.json
--rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/is-symbol/package.json
--rw-r--r--   0        0        0     3228 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/is-typed-array/package.json
--rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/is-typed-array/tsconfig.json
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/is-weakref/package.json
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/isarray/package.json
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/isexe/package.json
--rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/jackspeak/package.json
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/jackspeak/dist/commonjs/package.json
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/jackspeak/dist/esm/package.json
--rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/jiti/package.json
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/js-tokens/package.json
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/js-yaml/package.json
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/json-buffer/package.json
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/json-schema-traverse/package.json
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/json-stable-stringify-without-jsonify/package.json
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/json2module/package.json
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/json5/package.json
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/keyv/package.json
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/kind-of/package.json
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/lazy-cache/package.json
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/levn/package.json
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/lilconfig/package.json
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/lines-and-columns/package.json
--rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/local-pkg/package.json
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/locate-path/package.json
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/lodash/package.json
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/lodash-es/package.json
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/lodash.merge/package.json
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/longest/package.json
--rw-r--r--   0        0        0     3860 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/loupe/package.json
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/lru-cache/package.json
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/magic-string/package.json
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/merge-stream/package.json
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/merge2/package.json
--rw-r--r--   0        0        0     2648 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/micromatch/package.json
--rw-r--r--   0        0        0   185882 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/mime-db/db.json
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/mime-db/package.json
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/mime-types/package.json
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/mimic-fn/package.json
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/minimatch/package.json
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/minimist/package.json
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/minipass/package.json
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/minipass/dist/commonjs/package.json
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/minipass/dist/esm/package.json
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/mlly/package.json
--rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/mock-property/package.json
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/mockjs/bower.json
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/mockjs/package.json
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/mockjs/test/bower.json
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/mockjs/test/package.json
--rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/moment/package.json
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/ms/package.json
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/mz/package.json
--rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/nanoid/package.json
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/nanoid/async/package.json
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/nanoid/non-secure/package.json
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/nanoid/url-alphabet/package.json
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/natural-compare/package.json
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/node-releases/package.json
--rw-r--r--   0        0        0    29857 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/node-releases/data/processed/envs.json
--rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/node-releases/data/release-schedule/release-schedule.json
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/normalize-path/package.json
--rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/normalize-range/package.json
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/npm-run-path/package.json
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/npm-run-path/node_modules/path-key/package.json
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/nth-check/package.json
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/nth-check/lib/esm/package.json
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/object-assign/package.json
--rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/object-hash/package.json
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/object-inspect/package-support.json
--rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/object-inspect/package.json
--rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/object-is/package.json
--rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/object-keys/package.json
--rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/object.assign/package.json
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/once/package.json
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/onetime/package.json
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/optionator/package.json
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/p-limit/package.json
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/p-locate/package.json
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/parent-module/package.json
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/path-exists/package.json
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/path-is-absolute/package.json
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/path-key/package.json
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/path-parse/package.json
--rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/path-scurry/package.json
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/path-scurry/dist/commonjs/package.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/path-scurry/dist/esm/package.json
--rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/path-scurry/node_modules/lru-cache/package.json
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/path-scurry/node_modules/lru-cache/dist/commonjs/package.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/path-scurry/node_modules/lru-cache/dist/esm/package.json
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/pathe/package.json
--rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/pathval/package.json
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/pdfast/package.json
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/picocolors/package.json
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/picomatch/package.json
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/pify/package.json
--rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/pinia/package.json
--rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/pinia/node_modules/vue-demi/package.json
--rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/pirates/package.json
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/pkg-types/package.json
--rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/possible-typed-array-names/package.json
--rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/possible-typed-array-names/tsconfig.json
--rwxr-xr-x   0        0        0     2496 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/postcss/package.json
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/postcss-import/package.json
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/postcss-js/package.json
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/postcss-load-config/package.json
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/postcss-load-config/node_modules/lilconfig/package.json
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/postcss-nested/package.json
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/postcss-selector-parser/package.json
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/postcss-value-parser/package.json
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/prelude-ls/package.json
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/prettier/package.json
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/prettier-linter-helpers/package.json
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/prettier-linter-helpers/.vscode/settings.json
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/pretty-format/package.json
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/pretty-format/node_modules/ansi-styles/package.json
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/proxy-from-env/package.json
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/punycode/package.json
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/queue-microtask/package.json
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/react-is/package.json
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/read-cache/package.json
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/readdirp/package.json
--rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/regexp.prototype.flags/package.json
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/repeat-string/package.json
--rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/resolve/package.json
--rw-r--r--   0        0        0     5769 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/resolve/lib/core.json
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/resolve/test/module_dir/zmodules/bbb/package.json
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/resolve/test/resolver/baz/package.json
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/resolve/test/resolver/browser_field/package.json
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/resolve/test/resolver/dot_main/package.json
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/resolve/test/resolver/dot_slash_main/package.json
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/resolve/test/resolver/false_main/package.json
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/resolve/test/resolver/incorrect_main/package.json
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/resolve/test/resolver/invalid_main/package.json
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/resolve/test/resolver/multirepo/lerna.json
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/resolve/test/resolver/multirepo/package.json
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/resolve/test/resolver/multirepo/packages/package-a/package.json
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/resolve/test/resolver/multirepo/packages/package-b/package.json
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/resolve/test/resolver/nested_symlinks/mylib/package.json
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/resolve/test/resolver/symlinked/package/package.json
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/resolve-from/package.json
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/reusify/package.json
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/right-align/package.json
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/rimraf/package.json
--rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/rollup/package.json
--rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/rollup/node_modules/ansi-regex/package.json
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/rollup/node_modules/ansi-styles/package.json
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/rollup/node_modules/chalk/package.json
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/rollup/node_modules/escape-string-regexp/package.json
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/rollup/node_modules/strip-ansi/package.json
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/rollup/node_modules/supports-color/package.json
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/run-parallel/package.json
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/rw/package.json
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/safe-array-concat/package.json
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/safe-array-concat/tsconfig.json
--rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/safe-regex-test/package.json
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/sass/package.json
--rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/scule/package.json
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/semver/package.json
--rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/set-function-length/package.json
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/set-function-length/tsconfig.json
--rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/set-function-name/package.json
--rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/set-function-name/tsconfig.json
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/shebang-command/package.json
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/shebang-regex/package.json
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/side-channel/package.json
--rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/side-channel/tsconfig.json
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/side-channel/node_modules/object-inspect/package-support.json
--rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/side-channel/node_modules/object-inspect/package.json
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/siginfo/package.json
--rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/signal-exit/package.json
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/signal-exit/dist/cjs/package.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/signal-exit/dist/mjs/package.json
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/size-sensor/package.json
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/source-map/package.json
--rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/source-map-js/package.json
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/source-map-support/package.json
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/stackback/package.json
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/std-env/package.json
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/string-width/package.json
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/string-width/node_modules/ansi-regex/package.json
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/string-width/node_modules/strip-ansi/package.json
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/string-width-cjs/package.json
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/string-width-cjs/node_modules/emoji-regex/package.json
--rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/string.prototype.trim/package.json
--rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/string.prototype.trimend/package.json
--rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/string.prototype.trimstart/package.json
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/strip-ansi/package.json
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/strip-ansi-cjs/package.json
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/strip-final-newline/package.json
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/strip-json-comments/package.json
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/strip-literal/package.json
--rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/sucrase/package.json
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/sucrase/node_modules/brace-expansion/package.json
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/sucrase/node_modules/commander/package.json
--rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/sucrase/node_modules/glob/package.json
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/sucrase/node_modules/glob/dist/commonjs/package.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/sucrase/node_modules/glob/dist/esm/package.json
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/sucrase/node_modules/minimatch/package.json
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/sucrase/node_modules/minimatch/dist/commonjs/package.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/sucrase/node_modules/minimatch/dist/esm/package.json
--rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/supports-color/package.json
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/supports-preserve-symlinks-flag/package.json
--rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/tailwindcss/package.json
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/tailwindcss/stubs/.prettierrc.json
--rw-r--r--   0        0        0     3563 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/tape/package.json
--rw-r--r--   0        0        0     3214 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/terser/package.json
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/terser/bin/package.json
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/terser/dist/package.json
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/terser/node_modules/commander/package.json
--rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/terser/node_modules/source-map/package.json
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/terser/node_modules/source-map-support/package.json
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/text-table/package.json
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/thenify/package.json
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/thenify-all/package.json
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/tinybench/package.json
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/tinypool/package.json
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/tinyspy/package.json
--rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/tippy.js/package.json
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/tippy.js/headless/package.json
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/to-regex-range/package.json
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/ts-interface-checker/package.json
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/tslib/package.json
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/tslib/modules/package.json
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/type-check/package.json
--rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/type-detect/package.json
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/type-fest/package.json
--rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/typed-array-buffer/package.json
--rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/typed-array-buffer/tsconfig.json
--rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/typed-array-byte-length/package.json
--rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/typed-array-byte-length/tsconfig.json
--rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/typed-array-byte-offset/package.json
--rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/typed-array-byte-offset/tsconfig.json
--rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/typed-array-length/package.json
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/typed-array-length/tsconfig.json
--rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/ufo/package.json
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/uglify-js/package.json
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/uglify-js/node_modules/source-map/package.json
--rw-r--r--   0        0        0   142838 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/uglify-js/tools/domprops.json
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/uglify-to-browserify/package.json
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/unbox-primitive/package.json
--rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/unimport/package.json
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/unimport/node_modules/escape-string-regexp/package.json
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/unimport/node_modules/estree-walker/package.json
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/unimport/node_modules/local-pkg/package.json
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/unplugin/package.json
--rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/unplugin-auto-import/package.json
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/unplugin-auto-import/node_modules/brace-expansion/package.json
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/unplugin-auto-import/node_modules/minimatch/package.json
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/unplugin-auto-import/node_modules/minimatch/dist/commonjs/package.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/unplugin-auto-import/node_modules/minimatch/dist/esm/package.json
--rw-r--r--   0        0        0     3437 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/unplugin-vue-components/package.json
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/unplugin-vue-components/node_modules/brace-expansion/package.json
--rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/unplugin-vue-components/node_modules/minimatch/package.json
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/unplugin-vue-components/node_modules/minimatch/dist/cjs/package.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/unplugin-vue-components/node_modules/minimatch/dist/mjs/package.json
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/update-browserslist-db/package.json
--rwxr-xr-x   0        0        0     2172 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/uri-js/package.json
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/util-deprecate/package.json
--rw-r--r--   0        0        0     4906 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/vite/package.json
--rw-r--r--   0        0        0    10665 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/vite/node_modules/rollup/package.json
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/vite/node_modules/rollup/dist/es/package.json
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/vite/types/package.json
--rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/vite-node/package.json
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/vite-plugin-json5/package.json
--rw-r--r--   0        0        0     4761 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/vitest/package.json
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/vitest/node_modules/local-pkg/package.json
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/vitest/node_modules/strip-literal/package.json
--rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/vue/package.json
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/vue/compiler-sfc/package.json
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/vue/jsx-runtime/package.json
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/vue/server-renderer/package.json
--rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/vue-eslint-parser/package.json
--rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/vue-i18n/package.json
--rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/vue-i18n/vetur/attributes.json
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/vue-i18n/vetur/tags.json
--rw-r--r--   0        0        0     5218 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/vue-router/package.json
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/vue-router/vetur/attributes.json
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/vue-router/vetur/tags.json
--rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/vue-tippy/package.json
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/vue-tippy/tsconfig.json
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/vue-tippy/vetur/attributes.json
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/vue-tippy/vetur/tags.json
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/webpack-sources/package.json
--rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/webpack-virtual-modules/package.json
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/which/package.json
--rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/which-boxed-primitive/package.json
--rw-r--r--   0        0        0     3231 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/which-typed-array/package.json
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/which-typed-array/tsconfig.json
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/why-is-node-running/package.json
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/window-size/package.json
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/word-wrap/package.json
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/wordwrap/package.json
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/wrap-ansi/package.json
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/wrap-ansi/node_modules/ansi-regex/package.json
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/wrap-ansi/node_modules/ansi-styles/package.json
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/wrap-ansi/node_modules/strip-ansi/package.json
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/wrap-ansi-cjs/package.json
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/wrap-ansi-cjs/node_modules/emoji-regex/package.json
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/wrap-ansi-cjs/node_modules/string-width/package.json
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/wrappy/package.json
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/xml-name-validator/package.json
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/yallist/package.json
--rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/yaml/package.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/yaml/browser/package.json
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/yargs/package.json
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 swanlab-0.3.0/node_modules/yocto-queue/package.json
--rwxr-xr-x   0        0        0      258 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/__init__.py
--rw-r--r--   0        0        0     6935 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/env.py
--rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/error.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/package.json
--rw-r--r--   0        0        0     5411 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/package.py
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/api/__init__.py
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/api/cos.py
--rw-r--r--   0        0        0     8842 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/api/http.py
--rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/api/info.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/api/auth/__init__.py
--rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/api/auth/login.py
--rw-r--r--   0        0        0     4802 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/api/upload/__init__.py
--rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/api/upload/model.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/cli/__init__.py
--rw-r--r--   0        0        0     5019 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/cli/main.py
--rw-r--r--   0        0        0     4172 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/cli/utils.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/cloud/__init__.py
--rw-r--r--   0        0        0     4045 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/cloud/_log_collector.py
--rw-r--r--   0        0        0     5508 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/cloud/start_thread.py
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/cloud/task_types.py
--rw-r--r--   0        0        0     4551 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/cloud/utils.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/cloud/dog/README.md
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/cloud/dog/__init__.py
--rw-r--r--   0        0        0     2719 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/cloud/dog/log_sniffer.py
--rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/cloud/dog/metadata_handle.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/cloud/dog/sniffer_queue.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/compat/README.md
--rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/compat/server/controller/experiment.py
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/data/__init__.py
--rw-r--r--   0        0        0     9826 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/data/config.py
--rw-r--r--   0        0        0    17830 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/data/sdk.py
--rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/data/settings.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/data/modules/__init__.py
--rw-r--r--   0        0        0     8232 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/data/modules/audio.py
--rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/data/modules/base.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/data/modules/chart.py
--rw-r--r--   0        0        0    13853 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/data/modules/image.py
--rw-r--r--   0        0        0     6511 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/data/modules/object_3d.py
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/data/modules/text.py
--rw-r--r--   0        0        0     7619 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/data/modules/video.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/data/modules/utils_modules/__init__.py
--rw-r--r--   0        0        0     4040 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/data/modules/utils_modules/bounding_boxes.py
--rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/data/modules/utils_modules/image_mask.py
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/data/run/__init__.py
--rw-r--r--   0        0        0    19749 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/data/run/exp.py
--rw-r--r--   0        0        0    22205 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/data/run/main.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/data/system/__init__.py
--rw-r--r--   0        0        0     8065 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/data/system/info.py
--rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/data/system/monitor.py
--rwxr-xr-x   0        0        0   337072 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/data/system/bin/apple_gpu_stats
--rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/data/utils/file.py
--rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/data/utils/model.py
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/db/__init__.py
--rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/db/db_connect.py
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/db/error.py
--rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/db/model.py
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/db/table_config.py
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/db/docs/Errors.md
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/db/docs/README.md
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/db/migrate/__init__.py
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/db/migrate/chart.py
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/db/migrate/experiment.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/db/migrate/namespace.py
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/db/migrate/project.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/db/migrate/tag.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/db/models/__init__.py
--rw-r--r--   0        0        0     9068 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/db/models/charts.py
--rw-r--r--   0        0        0     4179 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/db/models/displays.py
--rw-r--r--   0        0        0     7016 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/db/models/experiments.py
--rw-r--r--   0        0        0     6326 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/db/models/namespaces.py
--rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/db/models/projects.py
--rw-r--r--   0        0        0     3927 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/db/models/sources.py
--rw-r--r--   0        0        0     4334 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/db/models/tags.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/db/utils/__init__.py
--rw-r--r--   0        0        0     9078 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/db/utils/chart.py
--rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/integration/huggingface.py
--rw-r--r--   0        0        0     7307 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/integration/mmengine.py
--rw-r--r--   0        0        0     7182 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/integration/pytorch_lightning.py
--rw-r--r--   0        0        0     8539 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/integration/integration_utils/autologging.py
--rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/integration/integration_utils/get_modules.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/integration/integration_utils/timer.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/integration/openai/__init__.py
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/integration/openai/openai.py
--rw-r--r--   0        0        0    19701 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/integration/openai/resolver.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/integration/zhipuai/__init__.py
--rw-r--r--   0        0        0     7125 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/integration/zhipuai/resolver.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/integration/zhipuai/zhipuai.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/log/__init__.py
--rw-r--r--   0        0        0     5581 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/log/console.py
--rw-r--r--   0        0        0     8992 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/log/log.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/server/__init__.py
--rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/server/app.py
--rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/server/settings.py
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/server/controller/chart.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/server/controller/db.py
--rw-r--r--   0        0        0    16722 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/server/controller/experiment.py
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/server/controller/namespace.py
--rw-r--r--   0        0        0     8076 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/server/controller/project.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/server/controller/utils/__init__.py
--rw-r--r--   0        0        0     6976 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/server/controller/utils/charts.py
--rw-r--r--   0        0        0     5042 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/server/controller/utils/tag.py
--rw-r--r--   0        0        0     4212 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/server/middleware/common.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/server/module/__init__.py
--rw-r--r--   0        0        0     3578 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/server/module/resp.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/server/router/chart.py
--rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/server/router/experiment.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/server/router/media.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/server/router/namespace.py
--rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/server/router/project.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/template/index.html
--rw-r--r--   0        0        0     4395 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/template/assets/ChartPage-CR1Gy4nD.js
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/template/assets/ChartPage-DgOOkrVh.css
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/template/assets/ChartsView-Cp_w0mYy.js
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/template/assets/EnvHardware-UlpkNHre.js
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/template/assets/EnvIndex-QRnlb5o-.js
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/template/assets/EnvItems-BByd5_l_.js
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/template/assets/EnvItems-BfjcRO-X.css
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/template/assets/EnvRequirements-BqyzUHLZ.css
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/template/assets/EnvRequirements-C_C5xDM7.js
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/template/assets/EnvironmentPage-C6uSuWBq.css
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/template/assets/EnvironmentPage-DWu4jgoh.js
--rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/template/assets/ExperimentView-BwOYqQ05.js
--rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/template/assets/ExperimentView-CCDMXo4h.css
--rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/template/assets/FuncBar-BsXaYgxx.js
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/template/assets/FuncBar-DgVTuZfd.css
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/template/assets/HelpView-D9183KCW.js
--rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/template/assets/HomeView-BIJzBfvA.css
--rw-r--r--   0        0        0    11977 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/template/assets/HomeView-BM5pU9yO.js
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/template/assets/IndexPage-C5dvtib2.css
--rw-r--r--   0        0        0     4305 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/template/assets/IndexPage-DNYsYgRx.js
--rw-r--r--   0        0        0   273900 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/template/assets/JetBrainsMono-Regular-Dh36KTnx.ttf
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/template/assets/LogPage-DBzoauOW.css
--rw-r--r--   0        0        0     3634 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/template/assets/LogPage-fDtMFLcB.js
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/template/assets/NotFound--wQ84Mpr.js
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/template/assets/SLLoading-wlC0Kmfx.js
--rw-r--r--   0        0        0     5489 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/template/assets/SLStatusLabel-1A8U87-U.js
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/template/assets/SLStatusLabel-BRacn5XK.css
--rw-r--r--   0        0        0   119080 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/template/assets/SourceSansPro-Regular-J3NOkSfZ.ttf
--rw-r--r--   0        0        0   893736 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/template/assets/chart-B0yY4W3r.js
--rw-r--r--   0        0        0    11807 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/template/assets/chart-DXdkqIcq.css
--rw-r--r--   0        0        0   389080 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/template/assets/index-BH23qgZj.js
--rw-r--r--   0        0        0    36914 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/template/assets/index-DUgbEQPz.css
--rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/template/assets/logo-ChHf2ozk.ico
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/utils/__init__.py
--rw-r--r--   0        0        0     7816 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/utils/file.py
--rw-r--r--   0        0        0     8727 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/utils/font.py
--rw-r--r--   0        0        0     6680 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/utils/judgment.py
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/utils/key.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 swanlab-0.3.0/swanlab/utils/time.py
--rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 swanlab-0.3.0/test/create_experiment.py
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 swanlab-0.3.0/test/start_server.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 swanlab-0.3.0/test/config/config.json
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 swanlab-0.3.0/test/config/load.yaml
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 swanlab-0.3.0/test/unit/conftest.py
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 swanlab-0.3.0/test/unit/pytest_example.py
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 swanlab-0.3.0/test/unit/auth/pytest_login.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 swanlab-0.3.0/test/unit/data/pytest_sdk.py
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 swanlab-0.3.0/test/unit/data/run/pytest_main.py
--rw-r--r--   0        0        0     3588 2020-02-02 00:00:00.000000 swanlab-0.3.0/test/unit/log/pytest_log.py
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 swanlab-0.3.0/test/unit/server/controller/utils/utils.py
--rw-r--r--   0        0        0     6811 2020-02-02 00:00:00.000000 swanlab-0.3.0/test/unit/utils/pytest_file.py
--rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 swanlab-0.3.0/test/unit/utils/pytest_key.py
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 swanlab-0.3.0/test/unit/utils/pytest_package.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 swanlab-0.3.0/.gitignore
--rw-r--r--   0        0        0    10779 2020-02-02 00:00:00.000000 swanlab-0.3.0/LICENSE
--rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 swanlab-0.3.0/pyproject.toml
--rw-r--r--   0        0        0    28574 2020-02-02 00:00:00.000000 swanlab-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 swanlab-0.3.1/.eslintrc-auto-import.json
+-rw-r--r--   0        0        0    26391 2020-02-02 00:00:00.000000 swanlab-0.3.1/README.md
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 swanlab-0.3.1/jsconfig.json
+-rw-r--r--   0        0        0   235776 2020-02-02 00:00:00.000000 swanlab-0.3.1/package-lock.json
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 swanlab-0.3.1/package.json
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 swanlab-0.3.1/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 swanlab-0.3.1/.config/copy_frontend.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 swanlab-0.3.1/.vscode/extensions.json
+-rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 swanlab-0.3.1/.vscode/launch.json
+-rw-r--r--   0        0        0     3112 2020-02-02 00:00:00.000000 swanlab-0.3.1/.vscode/settings.json
+-rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 swanlab-0.3.1/.vscode/tailwind.json
+-rw-r--r--   0        0        0   217945 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/.package-lock.json
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@alloc/quick-lru/package.json
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@antfu/utils/package.json
+-rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@antv/adjust/package.json
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@antv/adjust/node_modules/tslib/package.json
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@antv/adjust/node_modules/tslib/modules/package.json
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@antv/adjust/node_modules/tslib/test/validateModuleExportsMatchCommonJS/package.json
+-rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@antv/attr/package.json
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@antv/color-util/package.json
+-rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@antv/component/package.json
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@antv/component/node_modules/@antv/path-util/package.json
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@antv/component/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@antv/coord/package.json
+-rw-r--r--   0        0        0     1524 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@antv/dom-util/package.json
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@antv/event-emitter/package.json
+-rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@antv/g-base/package.json
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@antv/g-base/node_modules/@antv/path-util/package.json
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@antv/g-base/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json
+-rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@antv/g-canvas/package.json
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@antv/g-canvas/node_modules/@antv/path-util/package.json
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@antv/g-canvas/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@antv/g-math/package.json
+-rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@antv/g-svg/package.json
+-rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@antv/g2/package.json
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@antv/g2/node_modules/@antv/path-util/package.json
+-rw-r--r--   0        0        0     1560 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@antv/g2/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json
+-rw-r--r--   0        0        0     3969 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@antv/g2plot/package.json
+-rw-r--r--   0        0        0     1589 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@antv/matrix-util/package.json
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@antv/path-util/package.json
+-rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@antv/scale/package.json
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@antv/util/package.json
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@babel/parser/package.json
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@esbuild/linux-x64/package.json
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@eslint/eslintrc/package.json
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@eslint/js/package.json
+-rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@eslint-community/eslint-utils/package.json
+-rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@eslint-community/regexpp/package.json
+-rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@headlessui/vue/package.json
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@humanwhocodes/config-array/package.json
+-rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@humanwhocodes/module-importer/package.json
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@humanwhocodes/object-schema/package.json
+-rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@intlify/core-base/package.json
+-rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@intlify/message-compiler/package.json
+-rw-r--r--   0        0        0     1593 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@intlify/shared/package.json
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@isaacs/cliui/package.json
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@isaacs/cliui/node_modules/ansi-regex/package.json
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@isaacs/cliui/node_modules/strip-ansi/package.json
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@jest/schemas/package.json
+-rw-r--r--   0        0        0     2291 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@jridgewell/gen-mapping/package.json
+-rw-r--r--   0        0        0     2063 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@jridgewell/resolve-uri/package.json
+-rw-r--r--   0        0        0     1987 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@jridgewell/set-array/package.json
+-rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@jridgewell/source-map/package.json
+-rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@jridgewell/sourcemap-codec/package.json
+-rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@jridgewell/trace-mapping/package.json
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@ljharb/resumer/package.json
+-rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@ljharb/through/package.json
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@ljharb/through/tsconfig.json
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@nodelib/fs.scandir/package.json
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@nodelib/fs.stat/package.json
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@nodelib/fs.walk/package.json
+-rw-r--r--   0        0        0      881 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@pkgjs/parseargs/package.json
+-rw-r--r--   0        0        0     4230 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@popperjs/core/package.json
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@rollup/pluginutils/package.json
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@rollup/pluginutils/dist/es/package.json
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@rollup/rollup-linux-x64-gnu/package.json
+-rw-r--r--   0        0        0      419 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@rollup/rollup-linux-x64-musl/package.json
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@sinclair/typebox/package.json
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@tanstack/virtual-core/package.json
+-rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@tanstack/vue-virtual/package.json
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@types/d3-timer/package.json
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@types/estree/package.json
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@ungap/structured-clone/package.json
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@ungap/structured-clone/cjs/package.json
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@vitejs/plugin-vue/package.json
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@vitest/expect/package.json
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@vitest/runner/package.json
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@vitest/runner/node_modules/p-limit/package.json
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@vitest/runner/node_modules/yocto-queue/package.json
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@vitest/snapshot/package.json
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@vitest/spy/package.json
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@vitest/utils/package.json
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@vitest/utils/node_modules/estree-walker/package.json
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@vue/compiler-core/package.json
+-rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@vue/compiler-dom/package.json
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@vue/compiler-sfc/package.json
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@vue/compiler-ssr/package.json
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@vue/devtools-api/package.json
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@vue/reactivity/package.json
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@vue/runtime-core/package.json
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@vue/runtime-dom/package.json
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@vue/server-renderer/package.json
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/@vue/shared/package.json
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/acorn/package.json
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/acorn-jsx/package.json
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/acorn-walk/package.json
+-rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/ajv/package.json
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/ajv/lib/refs/data.json
+-rw-r--r--   0        0        0     4357 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/ajv/lib/refs/json-schema-draft-04.json
+-rw-r--r--   0        0        0     4445 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/ajv/lib/refs/json-schema-draft-06.json
+-rw-r--r--   0        0        0     4879 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/ajv/lib/refs/json-schema-draft-07.json
+-rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/ajv/lib/refs/json-schema-secure.json
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/align-text/package.json
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/amdefine/package.json
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/ansi-regex/package.json
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/ansi-styles/package.json
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/any-promise/package.json
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/anymatch/package.json
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/arg/package.json
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/argparse/package.json
+-rw-r--r--   0        0        0     2473 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/array-buffer-byte-length/package.json
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/array-buffer-byte-length/tsconfig.json
+-rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/arraybuffer.prototype.slice/package.json
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/assertion-error/package.json
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/asynckit/package.json
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/autoprefixer/package.json
+-rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/available-typed-arrays/package.json
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/available-typed-arrays/tsconfig.json
+-rw-r--r--   0        0        0     7633 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/axios/package.json
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/balanced-match/package.json
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/binary-extensions/binary-extensions.json
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/binary-extensions/package.json
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/boolbase/package.json
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/brace-expansion/package.json
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/braces/package.json
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/browserslist/package.json
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/buffer-from/package.json
+-rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/cac/package.json
+-rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/call-bind/package.json
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/callsites/package.json
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/camelcase/package.json
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/camelcase-css/package.json
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/caniuse-lite/package.json
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/center-align/package.json
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/chai/bower.json
+-rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/chai/package.json
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/chalk/package.json
+-rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/check-error/package.json
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/chokidar/package.json
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/chokidar/node_modules/glob-parent/package.json
+-rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/cliui/package.json
+-rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/color-convert/package.json
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/color-name/package.json
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/combined-stream/package.json
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/commander/package-support.json
+-rw-r--r--   0        0        0     2127 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/commander/package.json
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/concat-map/package.json
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/confbox/package.json
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/contour_plot/package.json
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/cross-spawn/package.json
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/cssesc/package.json
+-rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/csstype/package.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/d3-color/package.json
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/d3-ease/package.json
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/d3-hierarchy/package.json
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/d3-interpolate/package.json
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/d3-regression/package.json
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/d3-timer/package.json
+-rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/data-view-buffer/package.json
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/data-view-buffer/tsconfig.json
+-rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/data-view-byte-length/package.json
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/data-view-byte-length/tsconfig.json
+-rw-r--r--   0        0        0     2426 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/data-view-byte-offset/package.json
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/data-view-byte-offset/tsconfig.json
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/debug/package.json
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/decamelize/package.json
+-rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/deep-eql/package.json
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/deep-equal/package.json
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/deep-is/package.json
+-rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/define-data-property/package.json
+-rw-r--r--   0        0        0     4883 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/define-data-property/tsconfig.json
+-rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/define-properties/package.json
+-rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/defined/package.json
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/delayed-stream/package.json
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/detect-browser/package.json
+-rwxr-xr-x   0        0        0      647 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/didyoumean/package.json
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/diff-sequences/package.json
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/dlv/package.json
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/doctrine/package.json
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/dotignore/package.json
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/eastasianwidth/package.json
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/electron-to-chromium/chromium-versions.json
+-rw-r--r--   0        0        0    49748 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/electron-to-chromium/full-chromium-versions.json
+-rw-r--r--   0        0        0    77770 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/electron-to-chromium/full-versions.json
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/electron-to-chromium/package.json
+-rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/electron-to-chromium/versions.json
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/emoji-regex/package.json
+-rw-r--r--   0        0        0     2883 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/entities/package.json
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/entities/lib/esm/package.json
+-rw-r--r--   0        0        0     4929 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/es-abstract/package.json
+-rw-r--r--   0        0        0    22346 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/es-abstract/helpers/caseFolding.json
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/es-abstract/node_modules/object-inspect/package-support.json
+-rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/es-abstract/node_modules/object-inspect/package.json
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/es-define-property/package.json
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/es-define-property/tsconfig.json
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/es-errors/package.json
+-rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/es-errors/tsconfig.json
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/es-object-atoms/package.json
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/es-object-atoms/tsconfig.json
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/es-set-tostringtag/package.json
+-rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/es-set-tostringtag/tsconfig.json
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/es-to-primitive/package.json
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/esbuild/package.json
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/escalade/package.json
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/escape-string-regexp/package.json
+-rw-r--r--   0        0        0     5566 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/eslint/package.json
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/eslint/conf/replacements.json
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/eslint/conf/rule-type-list.json
+-rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/eslint/lib/cli-engine/formatters/formatters-meta.json
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/eslint-config-prettier/package.json
+-rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/eslint-plugin-prettier/package.json
+-rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/eslint-plugin-vue/package.json
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/eslint-plugin-vue/lib/utils/deprecated-html-elements.json
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/eslint-plugin-vue/lib/utils/html-elements.json
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/eslint-plugin-vue/lib/utils/inline-non-void-elements.json
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/eslint-plugin-vue/lib/utils/js-reserved.json
+-rw-r--r--   0        0        0     5270 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/eslint-plugin-vue/lib/utils/key-aliases.json
+-rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/eslint-plugin-vue/lib/utils/svg-attributes-weird-case.json
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/eslint-plugin-vue/lib/utils/svg-elements.json
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/eslint-plugin-vue/lib/utils/void-elements.json
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/eslint-plugin-vue/lib/utils/vue-component-options.json
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/eslint-plugin-vue/lib/utils/vue-reserved.json
+-rw-r--r--   0        0        0     6650 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/eslint-plugin-vue/lib/utils/vue3-export-names.json
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/eslint-scope/package.json
+-rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/eslint-visitor-keys/package.json
+-rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/espree/package.json
+-rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/esquery/package.json
+-rwxr-xr-x   0        0        0     1165 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/esrecurse/package.json
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/estraverse/package.json
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/estree-walker/package.json
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/estree-walker/dist/esm/package.json
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/estree-walker/src/package.json
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/esutils/package.json
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/execa/package.json
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/fast-deep-equal/package.json
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/fast-diff/package.json
+-rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/fast-glob/package.json
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/fast-glob/node_modules/glob-parent/package.json
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/fast-json-stable-stringify/package.json
+-rw-r--r--   0        0        0     3828 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/fast-json-stable-stringify/benchmark/test.json
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/fast-levenshtein/package.json
+-rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/fastq/package.json
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/fastq/test/tsconfig.json
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/fecha/package.json
+-rw-r--r--   0        0        0     2756 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/file-entry-cache/package.json
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/fill-range/package.json
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/find-up/package.json
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/flat-cache/package.json
+-rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/flatted/package.json
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/flatted/cjs/package.json
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/fmin/.eslintrc.json
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/fmin/package.json
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/follow-redirects/package.json
+-rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/for-each/package.json
+-rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/foreground-child/package.json
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/foreground-child/dist/cjs/package.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/foreground-child/dist/mjs/package.json
+-rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/form-data/package.json
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/fraction.js/package.json
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/fs.realpath/package.json
+-rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/function-bind/package.json
+-rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/function.prototype.name/package.json
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/functions-have-names/package.json
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/get-func-name/package.json
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/get-intrinsic/package.json
+-rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/get-stream/package.json
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/get-symbol-description/package.json
+-rwxr-xr-x   0        0        0      630 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/gl-matrix/package.json
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/gl-matrix/mat2/package.json
+-rwxr-xr-x   0        0        0       91 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/gl-matrix/mat2d/package.json
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/gl-matrix/mat3/package.json
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/gl-matrix/mat4/package.json
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/gl-matrix/quat/package.json
+-rwxr-xr-x   0        0        0       91 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/gl-matrix/quat2/package.json
+-rwxr-xr-x   0        0        0      100 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/gl-matrix/types.d.ts/package.json
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/gl-matrix/vec2/package.json
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/gl-matrix/vec3/package.json
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/gl-matrix/vec4/package.json
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/glob/package.json
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/glob-parent/package.json
+-rw-r--r--   0        0        0    48140 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/globals/globals.json
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/globals/package.json
+-rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/globalthis/package.json
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/gopd/package.json
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/graphemer/package.json
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/has/package.json
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/has-ansi/package.json
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/has-ansi/node_modules/ansi-regex/package.json
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/has-bigints/package.json
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/has-flag/package.json
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/has-property-descriptors/package.json
+-rw-r--r--   0        0        0     2004 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/has-proto/package.json
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/has-proto/tsconfig.json
+-rw-r--r--   0        0        0     2648 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/has-symbols/package.json
+-rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/has-tostringtag/package.json
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/has-tostringtag/tsconfig.json
+-rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/hasown/package.json
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/hasown/tsconfig.json
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/human-signals/package.json
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/husky/package.json
+-rw-r--r--   0        0        0     1996 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/ignore/package.json
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/immutable/package.json
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/import-fresh/package.json
+-rw-r--r--   0        0        0      818 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/imurmurhash/package.json
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/inflight/package.json
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/inherits/package.json
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/internal-slot/package.json
+-rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/is-arguments/package.json
+-rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/is-array-buffer/package.json
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/is-array-buffer/tsconfig.json
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/is-bigint/package.json
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/is-binary-path/package.json
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/is-boolean-object/package.json
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/is-buffer/package.json
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/is-callable/package.json
+-rw-r--r--   0        0        0     5769 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/is-core-module/core.json
+-rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/is-core-module/package.json
+-rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/is-data-view/package.json
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/is-data-view/tsconfig.json
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/is-date-object/package.json
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/is-extglob/package.json
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/is-fullwidth-code-point/package.json
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/is-glob/package.json
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/is-negative-zero/package.json
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/is-negative-zero/tsconfig.json
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/is-number/package.json
+-rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/is-number-object/package.json
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/is-path-inside/package.json
+-rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/is-regex/package.json
+-rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/is-shared-array-buffer/package.json
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/is-shared-array-buffer/tsconfig.json
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/is-stream/package.json
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/is-string/package.json
+-rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/is-symbol/package.json
+-rw-r--r--   0        0        0     3228 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/is-typed-array/package.json
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/is-typed-array/tsconfig.json
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/is-weakref/package.json
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/isarray/package.json
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/isexe/package.json
+-rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/jackspeak/package.json
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/jackspeak/dist/commonjs/package.json
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/jackspeak/dist/esm/package.json
+-rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/jiti/package.json
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/js-tokens/package.json
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/js-yaml/package.json
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/json-buffer/package.json
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/json-schema-traverse/package.json
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/json-stable-stringify-without-jsonify/package.json
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/json2module/package.json
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/json5/package.json
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/keyv/package.json
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/kind-of/package.json
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/lazy-cache/package.json
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/levn/package.json
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/lilconfig/package.json
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/lines-and-columns/package.json
+-rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/local-pkg/package.json
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/locate-path/package.json
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/lodash/package.json
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/lodash-es/package.json
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/lodash.merge/package.json
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/longest/package.json
+-rw-r--r--   0        0        0     3860 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/loupe/package.json
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/lru-cache/package.json
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/magic-string/package.json
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/merge-stream/package.json
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/merge2/package.json
+-rw-r--r--   0        0        0     2648 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/micromatch/package.json
+-rw-r--r--   0        0        0   185882 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/mime-db/db.json
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/mime-db/package.json
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/mime-types/package.json
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/mimic-fn/package.json
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/minimatch/package.json
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/minimist/package.json
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/minipass/package.json
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/minipass/dist/commonjs/package.json
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/minipass/dist/esm/package.json
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/mlly/package.json
+-rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/mock-property/package.json
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/mockjs/bower.json
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/mockjs/package.json
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/mockjs/test/bower.json
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/mockjs/test/package.json
+-rw-r--r--   0        0        0     3556 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/moment/package.json
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/ms/package.json
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/mz/package.json
+-rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/nanoid/package.json
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/nanoid/async/package.json
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/nanoid/non-secure/package.json
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/nanoid/url-alphabet/package.json
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/natural-compare/package.json
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/node-releases/package.json
+-rw-r--r--   0        0        0    29857 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/node-releases/data/processed/envs.json
+-rw-r--r--   0        0        0     2137 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/node-releases/data/release-schedule/release-schedule.json
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/normalize-path/package.json
+-rw-r--r--   0        0        0     1184 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/normalize-range/package.json
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/npm-run-path/package.json
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/npm-run-path/node_modules/path-key/package.json
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/nth-check/package.json
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/nth-check/lib/esm/package.json
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/object-assign/package.json
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/object-hash/package.json
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/object-inspect/package-support.json
+-rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/object-inspect/package.json
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/object-is/package.json
+-rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/object-keys/package.json
+-rw-r--r--   0        0        0     2306 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/object.assign/package.json
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/once/package.json
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/onetime/package.json
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/optionator/package.json
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/p-limit/package.json
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/p-locate/package.json
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/parent-module/package.json
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/path-exists/package.json
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/path-is-absolute/package.json
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/path-key/package.json
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/path-parse/package.json
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/path-scurry/package.json
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/path-scurry/dist/commonjs/package.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/path-scurry/dist/esm/package.json
+-rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/path-scurry/node_modules/lru-cache/package.json
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/path-scurry/node_modules/lru-cache/dist/commonjs/package.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/path-scurry/node_modules/lru-cache/dist/esm/package.json
+-rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/pathe/package.json
+-rw-r--r--   0        0        0     2104 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/pathval/package.json
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/pdfast/package.json
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/picocolors/package.json
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/picomatch/package.json
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/pify/package.json
+-rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/pinia/package.json
+-rw-r--r--   0        0        0     1141 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/pinia/node_modules/vue-demi/package.json
+-rw-r--r--   0        0        0     1686 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/pirates/package.json
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/pkg-types/package.json
+-rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/possible-typed-array-names/package.json
+-rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/possible-typed-array-names/tsconfig.json
+-rwxr-xr-x   0        0        0     2496 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/postcss/package.json
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/postcss-import/package.json
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/postcss-js/package.json
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/postcss-load-config/package.json
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/postcss-load-config/node_modules/lilconfig/package.json
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/postcss-nested/package.json
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/postcss-selector-parser/package.json
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/postcss-value-parser/package.json
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/prelude-ls/package.json
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/prettier/package.json
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/prettier-linter-helpers/package.json
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/prettier-linter-helpers/.vscode/settings.json
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/pretty-format/package.json
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/pretty-format/node_modules/ansi-styles/package.json
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/proxy-from-env/package.json
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/punycode/package.json
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/queue-microtask/package.json
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/react-is/package.json
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/read-cache/package.json
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/readdirp/package.json
+-rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/regexp.prototype.flags/package.json
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/repeat-string/package.json
+-rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/resolve/package.json
+-rw-r--r--   0        0        0     5769 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/resolve/lib/core.json
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/resolve/test/module_dir/zmodules/bbb/package.json
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/resolve/test/resolver/baz/package.json
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/resolve/test/resolver/browser_field/package.json
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/resolve/test/resolver/dot_main/package.json
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/resolve/test/resolver/dot_slash_main/package.json
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/resolve/test/resolver/false_main/package.json
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/resolve/test/resolver/incorrect_main/package.json
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/resolve/test/resolver/invalid_main/package.json
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/resolve/test/resolver/multirepo/lerna.json
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/resolve/test/resolver/multirepo/package.json
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/resolve/test/resolver/multirepo/packages/package-a/package.json
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/resolve/test/resolver/multirepo/packages/package-b/package.json
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/resolve/test/resolver/nested_symlinks/mylib/package.json
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/resolve/test/resolver/symlinked/package/package.json
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/resolve-from/package.json
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/reusify/package.json
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/right-align/package.json
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/rimraf/package.json
+-rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/rollup/package.json
+-rw-r--r--   0        0        0     1189 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/rollup/node_modules/ansi-regex/package.json
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/rollup/node_modules/ansi-styles/package.json
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/rollup/node_modules/chalk/package.json
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/rollup/node_modules/escape-string-regexp/package.json
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/rollup/node_modules/strip-ansi/package.json
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/rollup/node_modules/supports-color/package.json
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/run-parallel/package.json
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/rw/package.json
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/safe-array-concat/package.json
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/safe-array-concat/tsconfig.json
+-rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/safe-regex-test/package.json
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/sass/package.json
+-rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/scule/package.json
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/semver/package.json
+-rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/set-function-length/package.json
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/set-function-length/tsconfig.json
+-rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/set-function-name/package.json
+-rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/set-function-name/tsconfig.json
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/shebang-command/package.json
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/shebang-regex/package.json
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/side-channel/package.json
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/side-channel/tsconfig.json
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/side-channel/node_modules/object-inspect/package-support.json
+-rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/side-channel/node_modules/object-inspect/package.json
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/siginfo/package.json
+-rw-r--r--   0        0        0     2573 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/signal-exit/package.json
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/signal-exit/dist/cjs/package.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/signal-exit/dist/mjs/package.json
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/size-sensor/package.json
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/source-map/package.json
+-rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/source-map-js/package.json
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/source-map-support/package.json
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/stackback/package.json
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/std-env/package.json
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/string-width/package.json
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/string-width/node_modules/ansi-regex/package.json
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/string-width/node_modules/strip-ansi/package.json
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/string-width-cjs/package.json
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/string-width-cjs/node_modules/emoji-regex/package.json
+-rw-r--r--   0        0        0     2450 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/string.prototype.trim/package.json
+-rw-r--r--   0        0        0     2009 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/string.prototype.trimend/package.json
+-rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/string.prototype.trimstart/package.json
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/strip-ansi/package.json
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/strip-ansi-cjs/package.json
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/strip-final-newline/package.json
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/strip-json-comments/package.json
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/strip-literal/package.json
+-rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/sucrase/package.json
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/sucrase/node_modules/brace-expansion/package.json
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/sucrase/node_modules/commander/package.json
+-rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/sucrase/node_modules/glob/package.json
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/sucrase/node_modules/glob/dist/commonjs/package.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/sucrase/node_modules/glob/dist/esm/package.json
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/sucrase/node_modules/minimatch/package.json
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/sucrase/node_modules/minimatch/dist/commonjs/package.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/sucrase/node_modules/minimatch/dist/esm/package.json
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/supports-color/package.json
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/supports-preserve-symlinks-flag/package.json
+-rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/tailwindcss/package.json
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/tailwindcss/stubs/.prettierrc.json
+-rw-r--r--   0        0        0     3563 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/tape/package.json
+-rw-r--r--   0        0        0     3214 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/terser/package.json
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/terser/bin/package.json
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/terser/dist/package.json
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/terser/node_modules/commander/package.json
+-rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/terser/node_modules/source-map/package.json
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/terser/node_modules/source-map-support/package.json
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/text-table/package.json
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/thenify/package.json
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/thenify-all/package.json
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/tinybench/package.json
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/tinypool/package.json
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/tinyspy/package.json
+-rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/tippy.js/package.json
+-rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/tippy.js/headless/package.json
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/to-regex-range/package.json
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/ts-interface-checker/package.json
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/tslib/package.json
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/tslib/modules/package.json
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/type-check/package.json
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/type-detect/package.json
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/type-fest/package.json
+-rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/typed-array-buffer/package.json
+-rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/typed-array-buffer/tsconfig.json
+-rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/typed-array-byte-length/package.json
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/typed-array-byte-length/tsconfig.json
+-rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/typed-array-byte-offset/package.json
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/typed-array-byte-offset/tsconfig.json
+-rw-r--r--   0        0        0     2915 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/typed-array-length/package.json
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/typed-array-length/tsconfig.json
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/ufo/package.json
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/uglify-js/package.json
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/uglify-js/node_modules/source-map/package.json
+-rw-r--r--   0        0        0   142838 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/uglify-js/tools/domprops.json
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/uglify-to-browserify/package.json
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/unbox-primitive/package.json
+-rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/unimport/package.json
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/unimport/node_modules/escape-string-regexp/package.json
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/unimport/node_modules/estree-walker/package.json
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/unimport/node_modules/local-pkg/package.json
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/unplugin/package.json
+-rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/unplugin-auto-import/package.json
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/unplugin-auto-import/node_modules/brace-expansion/package.json
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/unplugin-auto-import/node_modules/minimatch/package.json
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/unplugin-auto-import/node_modules/minimatch/dist/commonjs/package.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/unplugin-auto-import/node_modules/minimatch/dist/esm/package.json
+-rw-r--r--   0        0        0     3437 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/unplugin-vue-components/package.json
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/unplugin-vue-components/node_modules/brace-expansion/package.json
+-rw-r--r--   0        0        0     2148 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/unplugin-vue-components/node_modules/minimatch/package.json
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/unplugin-vue-components/node_modules/minimatch/dist/cjs/package.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/unplugin-vue-components/node_modules/minimatch/dist/mjs/package.json
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/update-browserslist-db/package.json
+-rwxr-xr-x   0        0        0     2172 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/uri-js/package.json
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/util-deprecate/package.json
+-rw-r--r--   0        0        0     4906 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/vite/package.json
+-rw-r--r--   0        0        0    10864 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/vite/node_modules/rollup/package.json
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/vite/node_modules/rollup/dist/es/package.json
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/vite/types/package.json
+-rw-r--r--   0        0        0     2323 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/vite-node/package.json
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/vite-plugin-json5/package.json
+-rw-r--r--   0        0        0     4761 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/vitest/package.json
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/vitest/node_modules/local-pkg/package.json
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/vitest/node_modules/strip-literal/package.json
+-rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/vue/package.json
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/vue/compiler-sfc/package.json
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/vue/jsx-runtime/package.json
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/vue/server-renderer/package.json
+-rw-r--r--   0        0        0     4007 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/vue-eslint-parser/package.json
+-rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/vue-i18n/package.json
+-rw-r--r--   0        0        0     2241 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/vue-i18n/vetur/attributes.json
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/vue-i18n/vetur/tags.json
+-rw-r--r--   0        0        0     5218 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/vue-router/package.json
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/vue-router/vetur/attributes.json
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/vue-router/vetur/tags.json
+-rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/vue-tippy/package.json
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/vue-tippy/tsconfig.json
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/vue-tippy/vetur/attributes.json
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/vue-tippy/vetur/tags.json
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/webpack-sources/package.json
+-rw-r--r--   0        0        0     2136 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/webpack-virtual-modules/package.json
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/which/package.json
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/which-boxed-primitive/package.json
+-rw-r--r--   0        0        0     3231 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/which-typed-array/package.json
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/which-typed-array/tsconfig.json
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/why-is-node-running/package.json
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/window-size/package.json
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/word-wrap/package.json
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/wordwrap/package.json
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/wrap-ansi/package.json
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/wrap-ansi/node_modules/ansi-regex/package.json
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/wrap-ansi/node_modules/ansi-styles/package.json
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/wrap-ansi/node_modules/strip-ansi/package.json
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/wrap-ansi-cjs/package.json
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/wrap-ansi-cjs/node_modules/emoji-regex/package.json
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/wrap-ansi-cjs/node_modules/string-width/package.json
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/wrappy/package.json
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/xml-name-validator/package.json
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/yallist/package.json
+-rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/yaml/package.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/yaml/browser/package.json
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/yargs/package.json
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 swanlab-0.3.1/node_modules/yocto-queue/package.json
+-rwxr-xr-x   0        0        0      258 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/__init__.py
+-rw-r--r--   0        0        0     6935 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/env.py
+-rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/error.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/package.json
+-rw-r--r--   0        0        0     5411 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/package.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/api/__init__.py
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/api/cos.py
+-rw-r--r--   0        0        0     8842 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/api/http.py
+-rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/api/info.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/api/auth/__init__.py
+-rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/api/auth/login.py
+-rw-r--r--   0        0        0     4802 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/api/upload/__init__.py
+-rw-r--r--   0        0        0     1049 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/api/upload/model.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/cli/__init__.py
+-rw-r--r--   0        0        0     5019 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/cli/main.py
+-rw-r--r--   0        0        0     4172 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/cli/utils.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/cloud/__init__.py
+-rw-r--r--   0        0        0     4045 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/cloud/_log_collector.py
+-rw-r--r--   0        0        0     5508 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/cloud/start_thread.py
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/cloud/task_types.py
+-rw-r--r--   0        0        0     4551 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/cloud/utils.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/cloud/dog/README.md
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/cloud/dog/__init__.py
+-rw-r--r--   0        0        0     2719 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/cloud/dog/log_sniffer.py
+-rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/cloud/dog/metadata_handle.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/cloud/dog/sniffer_queue.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/compat/README.md
+-rw-r--r--   0        0        0     2637 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/compat/server/controller/experiment.py
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/data/__init__.py
+-rw-r--r--   0        0        0     9826 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/data/config.py
+-rw-r--r--   0        0        0    18000 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/data/sdk.py
+-rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/data/settings.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/data/modules/__init__.py
+-rw-r--r--   0        0        0     8232 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/data/modules/audio.py
+-rw-r--r--   0        0        0     4355 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/data/modules/base.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/data/modules/chart.py
+-rw-r--r--   0        0        0    13853 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/data/modules/image.py
+-rw-r--r--   0        0        0     6511 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/data/modules/object_3d.py
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/data/modules/text.py
+-rw-r--r--   0        0        0     7619 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/data/modules/video.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/data/modules/utils_modules/__init__.py
+-rw-r--r--   0        0        0     4040 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/data/modules/utils_modules/bounding_boxes.py
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/data/modules/utils_modules/image_mask.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/data/run/__init__.py
+-rw-r--r--   0        0        0    19749 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/data/run/exp.py
+-rw-r--r--   0        0        0    22205 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/data/run/main.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/data/system/__init__.py
+-rw-r--r--   0        0        0     8065 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/data/system/info.py
+-rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/data/system/monitor.py
+-rwxr-xr-x   0        0        0   337072 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/data/system/bin/apple_gpu_stats
+-rw-r--r--   0        0        0     3632 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/data/utils/file.py
+-rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/data/utils/model.py
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/db/__init__.py
+-rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/db/db_connect.py
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/db/error.py
+-rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/db/model.py
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/db/table_config.py
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/db/docs/Errors.md
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/db/docs/README.md
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/db/migrate/__init__.py
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/db/migrate/chart.py
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/db/migrate/experiment.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/db/migrate/namespace.py
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/db/migrate/project.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/db/migrate/tag.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/db/models/__init__.py
+-rw-r--r--   0        0        0     9068 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/db/models/charts.py
+-rw-r--r--   0        0        0     4179 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/db/models/displays.py
+-rw-r--r--   0        0        0     7016 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/db/models/experiments.py
+-rw-r--r--   0        0        0     6326 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/db/models/namespaces.py
+-rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/db/models/projects.py
+-rw-r--r--   0        0        0     3927 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/db/models/sources.py
+-rw-r--r--   0        0        0     4334 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/db/models/tags.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/db/utils/__init__.py
+-rw-r--r--   0        0        0     9078 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/db/utils/chart.py
+-rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/integration/huggingface.py
+-rw-r--r--   0        0        0     7307 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/integration/mmengine.py
+-rw-r--r--   0        0        0     7182 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/integration/pytorch_lightning.py
+-rw-r--r--   0        0        0     8539 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/integration/integration_utils/autologging.py
+-rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/integration/integration_utils/get_modules.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/integration/integration_utils/timer.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/integration/openai/__init__.py
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/integration/openai/openai.py
+-rw-r--r--   0        0        0    19701 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/integration/openai/resolver.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/integration/zhipuai/__init__.py
+-rw-r--r--   0        0        0     7125 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/integration/zhipuai/resolver.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/integration/zhipuai/zhipuai.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/log/__init__.py
+-rw-r--r--   0        0        0     5581 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/log/console.py
+-rw-r--r--   0        0        0     8992 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/log/log.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/server/__init__.py
+-rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/server/app.py
+-rw-r--r--   0        0        0     2590 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/server/settings.py
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/server/controller/chart.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/server/controller/db.py
+-rw-r--r--   0        0        0    16722 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/server/controller/experiment.py
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/server/controller/namespace.py
+-rw-r--r--   0        0        0     8076 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/server/controller/project.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/server/controller/utils/__init__.py
+-rw-r--r--   0        0        0     6976 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/server/controller/utils/charts.py
+-rw-r--r--   0        0        0     5042 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/server/controller/utils/tag.py
+-rw-r--r--   0        0        0     4212 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/server/middleware/common.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/server/module/__init__.py
+-rw-r--r--   0        0        0     3578 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/server/module/resp.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/server/router/chart.py
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/server/router/experiment.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/server/router/media.py
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/server/router/namespace.py
+-rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/server/router/project.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/template/index.html
+-rw-r--r--   0        0        0     4395 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/template/assets/ChartPage-CR1Gy4nD.js
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/template/assets/ChartPage-DgOOkrVh.css
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/template/assets/ChartsView-Cp_w0mYy.js
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/template/assets/EnvHardware-UlpkNHre.js
+-rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/template/assets/EnvIndex-QRnlb5o-.js
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/template/assets/EnvItems-BByd5_l_.js
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/template/assets/EnvItems-BfjcRO-X.css
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/template/assets/EnvRequirements-BqyzUHLZ.css
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/template/assets/EnvRequirements-C_C5xDM7.js
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/template/assets/EnvironmentPage-C6uSuWBq.css
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/template/assets/EnvironmentPage-DWu4jgoh.js
+-rw-r--r--   0        0        0     3973 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/template/assets/ExperimentView-BwOYqQ05.js
+-rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/template/assets/ExperimentView-CCDMXo4h.css
+-rw-r--r--   0        0        0     1748 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/template/assets/FuncBar-BsXaYgxx.js
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/template/assets/FuncBar-DgVTuZfd.css
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/template/assets/HelpView-D9183KCW.js
+-rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/template/assets/HomeView-BIJzBfvA.css
+-rw-r--r--   0        0        0    11977 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/template/assets/HomeView-BM5pU9yO.js
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/template/assets/IndexPage-C5dvtib2.css
+-rw-r--r--   0        0        0     4305 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/template/assets/IndexPage-DNYsYgRx.js
+-rw-r--r--   0        0        0   273900 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/template/assets/JetBrainsMono-Regular-Dh36KTnx.ttf
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/template/assets/LogPage-DBzoauOW.css
+-rw-r--r--   0        0        0     3634 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/template/assets/LogPage-fDtMFLcB.js
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/template/assets/NotFound--wQ84Mpr.js
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/template/assets/SLLoading-wlC0Kmfx.js
+-rw-r--r--   0        0        0     5489 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/template/assets/SLStatusLabel-1A8U87-U.js
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/template/assets/SLStatusLabel-BRacn5XK.css
+-rw-r--r--   0        0        0   119080 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/template/assets/SourceSansPro-Regular-J3NOkSfZ.ttf
+-rw-r--r--   0        0        0   893736 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/template/assets/chart-B0yY4W3r.js
+-rw-r--r--   0        0        0    11807 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/template/assets/chart-DXdkqIcq.css
+-rw-r--r--   0        0        0   389080 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/template/assets/index-BH23qgZj.js
+-rw-r--r--   0        0        0    36914 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/template/assets/index-DUgbEQPz.css
+-rw-r--r--   0        0        0     4286 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/template/assets/logo-ChHf2ozk.ico
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/utils/__init__.py
+-rw-r--r--   0        0        0     7816 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/utils/file.py
+-rw-r--r--   0        0        0     8727 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/utils/font.py
+-rw-r--r--   0        0        0     6680 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/utils/judgment.py
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/utils/key.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 swanlab-0.3.1/swanlab/utils/time.py
+-rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 swanlab-0.3.1/test/create_experiment.py
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 swanlab-0.3.1/test/start_server.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 swanlab-0.3.1/test/config/config.json
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 swanlab-0.3.1/test/config/load.yaml
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 swanlab-0.3.1/test/unit/conftest.py
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 swanlab-0.3.1/test/unit/pytest_example.py
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 swanlab-0.3.1/test/unit/auth/pytest_login.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 swanlab-0.3.1/test/unit/data/pytest_sdk.py
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 swanlab-0.3.1/test/unit/data/run/pytest_main.py
+-rw-r--r--   0        0        0     3588 2020-02-02 00:00:00.000000 swanlab-0.3.1/test/unit/log/pytest_log.py
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 swanlab-0.3.1/test/unit/server/controller/utils/utils.py
+-rw-r--r--   0        0        0     6811 2020-02-02 00:00:00.000000 swanlab-0.3.1/test/unit/utils/pytest_file.py
+-rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 swanlab-0.3.1/test/unit/utils/pytest_key.py
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 swanlab-0.3.1/test/unit/utils/pytest_package.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 swanlab-0.3.1/.gitignore
+-rw-r--r--   0        0        0    10779 2020-02-02 00:00:00.000000 swanlab-0.3.1/LICENSE
+-rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 swanlab-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0    28574 2020-02-02 00:00:00.000000 swanlab-0.3.1/PKG-INFO
```

### Comparing `swanlab-0.3.0/.eslintrc-auto-import.json` & `swanlab-0.3.1/.eslintrc-auto-import.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/README.md` & `swanlab-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/package-lock.json` & `swanlab-0.3.1/package-lock.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9993094415696335%*

 * *Differences: {"'packages'": "{'node_modules/@babel/parser': {'version': '7.24.5', 'resolved': "*

 * *               "'https://registry.npmjs.org/@babel/parser/-/parser-7.24.5.tgz', 'integrity': "*

 * *               "'sha512-EOv5IK8arwh3LI47dz1b0tKUb/1uhHAnHJOrjgtQMIpu1uXd9mlFrJg9IUgGUgZ41Ch0K8REPTYpO7B76b4vJg=='}, "*

 * *               "'node_modules/@rollup/rollup-android-arm-eabi': {'version': '4.17.2', 'resolved': "*

 * *               "'https://registry.npmjs.org/@rollup/rollup-android-arm-eabi/-/rollup-android-arm-eabi-4.17.2.tgz', " […]*

```diff
@@ -350,17 +350,17 @@
         "node_modules/@babel/parser": {
             "bin": {
                 "parser": "bin/babel-parser.js"
             },
             "engines": {
                 "node": ">=6.0.0"
             },
-            "integrity": "sha512-zTvEBcghmeBma9QIGunWevvBAp4/Qu9Bdq+2k0Ot4fVMD6v3dsC9WOcRSKk7tRRyBM/53yKMJko9xOatGQAwSg==",
-            "resolved": "https://registry.npmjs.org/@babel/parser/-/parser-7.24.4.tgz",
-            "version": "7.24.4"
+            "integrity": "sha512-EOv5IK8arwh3LI47dz1b0tKUb/1uhHAnHJOrjgtQMIpu1uXd9mlFrJg9IUgGUgZ41Ch0K8REPTYpO7B76b4vJg==",
+            "resolved": "https://registry.npmjs.org/@babel/parser/-/parser-7.24.5.tgz",
+            "version": "7.24.5"
         },
         "node_modules/@esbuild/aix-ppc64": {
             "cpu": [
                 "ppc64"
             ],
             "dev": true,
             "engines": {
@@ -1077,216 +1077,216 @@
             "version": "5.1.0"
         },
         "node_modules/@rollup/rollup-android-arm-eabi": {
             "cpu": [
                 "arm"
             ],
             "dev": true,
-            "integrity": "sha512-P6Wg856Ou/DLpR+O0ZLneNmrv7QpqBg+hK4wE05ijbC/t349BRfMfx+UFj5Ha3fCFopIa6iSZlpdaB4agkWp2Q==",
+            "integrity": "sha512-NM0jFxY8bB8QLkoKxIQeObCaDlJKewVlIEkuyYKm5An1tdVZ966w2+MPQ2l8LBZLjR+SgyV+nRkTIunzOYBMLQ==",
             "optional": true,
             "os": [
                 "android"
             ],
-            "resolved": "https://registry.npmjs.org/@rollup/rollup-android-arm-eabi/-/rollup-android-arm-eabi-4.17.1.tgz",
-            "version": "4.17.1"
+            "resolved": "https://registry.npmjs.org/@rollup/rollup-android-arm-eabi/-/rollup-android-arm-eabi-4.17.2.tgz",
+            "version": "4.17.2"
         },
         "node_modules/@rollup/rollup-android-arm64": {
             "cpu": [
                 "arm64"
             ],
             "dev": true,
-            "integrity": "sha512-piwZDjuW2WiHr05djVdUkrG5JbjnGbtx8BXQchYCMfib/nhjzWoiScelZ+s5IJI7lecrwSxHCzW026MWBL+oJQ==",
+            "integrity": "sha512-yeX/Usk7daNIVwkq2uGoq2BYJKZY1JfyLTaHO/jaiSwi/lsf8fTFoQW/n6IdAsx5tx+iotu2zCJwz8MxI6D/Bw==",
             "optional": true,
             "os": [
                 "android"
             ],
-            "resolved": "https://registry.npmjs.org/@rollup/rollup-android-arm64/-/rollup-android-arm64-4.17.1.tgz",
-            "version": "4.17.1"
+            "resolved": "https://registry.npmjs.org/@rollup/rollup-android-arm64/-/rollup-android-arm64-4.17.2.tgz",
+            "version": "4.17.2"
         },
         "node_modules/@rollup/rollup-darwin-arm64": {
             "cpu": [
                 "arm64"
             ],
             "dev": true,
-            "integrity": "sha512-LsZXXIsN5Q460cKDT4Y+bzoPDhBmO5DTr7wP80d+2EnYlxSgkwdPfE3hbE+Fk8dtya+8092N9srjBTJ0di8RIA==",
+            "integrity": "sha512-kcMLpE6uCwls023+kknm71ug7MZOrtXo+y5p/tsg6jltpDtgQY1Eq5sGfHcQfb+lfuKwhBmEURDga9N0ol4YPw==",
             "optional": true,
             "os": [
                 "darwin"
             ],
-            "resolved": "https://registry.npmjs.org/@rollup/rollup-darwin-arm64/-/rollup-darwin-arm64-4.17.1.tgz",
-            "version": "4.17.1"
+            "resolved": "https://registry.npmjs.org/@rollup/rollup-darwin-arm64/-/rollup-darwin-arm64-4.17.2.tgz",
+            "version": "4.17.2"
         },
         "node_modules/@rollup/rollup-darwin-x64": {
             "cpu": [
                 "x64"
             ],
             "dev": true,
-            "integrity": "sha512-S7TYNQpWXB9APkxu/SLmYHezWwCoZRA9QLgrDeml+SR2A1LLPD2DBUdUlvmCF7FUpRMKvbeeWky+iizQj65Etw==",
+            "integrity": "sha512-AtKwD0VEx0zWkL0ZjixEkp5tbNLzX+FCqGG1SvOu993HnSz4qDI6S4kGzubrEJAljpVkhRSlg5bzpV//E6ysTQ==",
             "optional": true,
             "os": [
                 "darwin"
             ],
-            "resolved": "https://registry.npmjs.org/@rollup/rollup-darwin-x64/-/rollup-darwin-x64-4.17.1.tgz",
-            "version": "4.17.1"
+            "resolved": "https://registry.npmjs.org/@rollup/rollup-darwin-x64/-/rollup-darwin-x64-4.17.2.tgz",
+            "version": "4.17.2"
         },
         "node_modules/@rollup/rollup-linux-arm-gnueabihf": {
             "cpu": [
                 "arm"
             ],
             "dev": true,
-            "integrity": "sha512-Lq2JR5a5jsA5um2ZoLiXXEaOagnVyCpCW7xvlcqHC7y46tLwTEgUSTM3a2TfmmTMmdqv+jknUioWXlmxYxE9Yw==",
+            "integrity": "sha512-3reX2fUHqN7sffBNqmEyMQVj/CKhIHZd4y631duy0hZqI8Qoqf6lTtmAKvJFYa6bhU95B1D0WgzHkmTg33In0A==",
             "optional": true,
             "os": [
                 "linux"
             ],
-            "resolved": "https://registry.npmjs.org/@rollup/rollup-linux-arm-gnueabihf/-/rollup-linux-arm-gnueabihf-4.17.1.tgz",
-            "version": "4.17.1"
+            "resolved": "https://registry.npmjs.org/@rollup/rollup-linux-arm-gnueabihf/-/rollup-linux-arm-gnueabihf-4.17.2.tgz",
+            "version": "4.17.2"
         },
         "node_modules/@rollup/rollup-linux-arm-musleabihf": {
             "cpu": [
                 "arm"
             ],
             "dev": true,
-            "integrity": "sha512-9BfzwyPNV0IizQoR+5HTNBGkh1KXE8BqU0DBkqMngmyFW7BfuIZyMjQ0s6igJEiPSBvT3ZcnIFohZ19OqjhDPg==",
+            "integrity": "sha512-uSqpsp91mheRgw96xtyAGP9FW5ChctTFEoXP0r5FAzj/3ZRv3Uxjtc7taRQSaQM/q85KEKjKsZuiZM3GyUivRg==",
             "optional": true,
             "os": [
                 "linux"
             ],
-            "resolved": "https://registry.npmjs.org/@rollup/rollup-linux-arm-musleabihf/-/rollup-linux-arm-musleabihf-4.17.1.tgz",
-            "version": "4.17.1"
+            "resolved": "https://registry.npmjs.org/@rollup/rollup-linux-arm-musleabihf/-/rollup-linux-arm-musleabihf-4.17.2.tgz",
+            "version": "4.17.2"
         },
         "node_modules/@rollup/rollup-linux-arm64-gnu": {
             "cpu": [
                 "arm64"
             ],
             "dev": true,
-            "integrity": "sha512-e2uWaoxo/rtzA52OifrTSXTvJhAXb0XeRkz4CdHBK2KtxrFmuU/uNd544Ogkpu938BzEfvmWs8NZ8Axhw33FDw==",
+            "integrity": "sha512-EMMPHkiCRtE8Wdk3Qhtciq6BndLtstqZIroHiiGzB3C5LDJmIZcSzVtLRbwuXuUft1Cnv+9fxuDtDxz3k3EW2A==",
             "optional": true,
             "os": [
                 "linux"
             ],
-            "resolved": "https://registry.npmjs.org/@rollup/rollup-linux-arm64-gnu/-/rollup-linux-arm64-gnu-4.17.1.tgz",
-            "version": "4.17.1"
+            "resolved": "https://registry.npmjs.org/@rollup/rollup-linux-arm64-gnu/-/rollup-linux-arm64-gnu-4.17.2.tgz",
+            "version": "4.17.2"
         },
         "node_modules/@rollup/rollup-linux-arm64-musl": {
             "cpu": [
                 "arm64"
             ],
             "dev": true,
-            "integrity": "sha512-ekggix/Bc/d/60H1Mi4YeYb/7dbal1kEDZ6sIFVAE8pUSx7PiWeEh+NWbL7bGu0X68BBIkgF3ibRJe1oFTksQQ==",
+            "integrity": "sha512-NMPylUUZ1i0z/xJUIx6VUhISZDRT+uTWpBcjdv0/zkp7b/bQDF+NfnfdzuTiB1G6HTodgoFa93hp0O1xl+/UbA==",
             "optional": true,
             "os": [
                 "linux"
             ],
-            "resolved": "https://registry.npmjs.org/@rollup/rollup-linux-arm64-musl/-/rollup-linux-arm64-musl-4.17.1.tgz",
-            "version": "4.17.1"
+            "resolved": "https://registry.npmjs.org/@rollup/rollup-linux-arm64-musl/-/rollup-linux-arm64-musl-4.17.2.tgz",
+            "version": "4.17.2"
         },
         "node_modules/@rollup/rollup-linux-powerpc64le-gnu": {
             "cpu": [
                 "ppc64"
             ],
             "dev": true,
-            "integrity": "sha512-UGV0dUo/xCv4pkr/C8KY7XLFwBNnvladt8q+VmdKrw/3RUd3rD0TptwjisvE2TTnnlENtuY4/PZuoOYRiGp8Gw==",
+            "integrity": "sha512-T19My13y8uYXPw/L/k0JYaX1fJKFT/PWdXiHr8mTbXWxjVF1t+8Xl31DgBBvEKclw+1b00Chg0hxE2O7bTG7GQ==",
             "optional": true,
             "os": [
                 "linux"
             ],
-            "resolved": "https://registry.npmjs.org/@rollup/rollup-linux-powerpc64le-gnu/-/rollup-linux-powerpc64le-gnu-4.17.1.tgz",
-            "version": "4.17.1"
+            "resolved": "https://registry.npmjs.org/@rollup/rollup-linux-powerpc64le-gnu/-/rollup-linux-powerpc64le-gnu-4.17.2.tgz",
+            "version": "4.17.2"
         },
         "node_modules/@rollup/rollup-linux-riscv64-gnu": {
             "cpu": [
                 "riscv64"
             ],
             "dev": true,
-            "integrity": "sha512-gEYmYYHaehdvX46mwXrU49vD6Euf1Bxhq9pPb82cbUU9UT2NV+RSckQ5tKWOnNXZixKsy8/cPGtiUWqzPuAcXQ==",
+            "integrity": "sha512-BOaNfthf3X3fOWAB+IJ9kxTgPmMqPPH5f5k2DcCsRrBIbWnaJCgX2ll77dV1TdSy9SaXTR5iDXRL8n7AnoP5cg==",
             "optional": true,
             "os": [
                 "linux"
             ],
-            "resolved": "https://registry.npmjs.org/@rollup/rollup-linux-riscv64-gnu/-/rollup-linux-riscv64-gnu-4.17.1.tgz",
-            "version": "4.17.1"
+            "resolved": "https://registry.npmjs.org/@rollup/rollup-linux-riscv64-gnu/-/rollup-linux-riscv64-gnu-4.17.2.tgz",
+            "version": "4.17.2"
         },
         "node_modules/@rollup/rollup-linux-s390x-gnu": {
             "cpu": [
                 "s390x"
             ],
             "dev": true,
-            "integrity": "sha512-xeae5pMAxHFp6yX5vajInG2toST5lsCTrckSRUFwNgzYqnUjNBcQyqk1bXUxX5yhjWFl2Mnz3F8vQjl+2FRIcw==",
+            "integrity": "sha512-W0UP/x7bnn3xN2eYMql2T/+wpASLE5SjObXILTMPUBDB/Fg/FxC+gX4nvCfPBCbNhz51C+HcqQp2qQ4u25ok6g==",
             "optional": true,
             "os": [
                 "linux"
             ],
-            "resolved": "https://registry.npmjs.org/@rollup/rollup-linux-s390x-gnu/-/rollup-linux-s390x-gnu-4.17.1.tgz",
-            "version": "4.17.1"
+            "resolved": "https://registry.npmjs.org/@rollup/rollup-linux-s390x-gnu/-/rollup-linux-s390x-gnu-4.17.2.tgz",
+            "version": "4.17.2"
         },
         "node_modules/@rollup/rollup-linux-x64-gnu": {
             "cpu": [
                 "x64"
             ],
             "dev": true,
-            "integrity": "sha512-AsdnINQoDWfKpBzCPqQWxSPdAWzSgnYbrJYtn6W0H2E9It5bZss99PiLA8CgmDRfvKygt20UpZ3xkhFlIfX9zQ==",
+            "integrity": "sha512-Hy7pLwByUOuyaFC6mAr7m+oMC+V7qyifzs/nW2OJfC8H4hbCzOX07Ov0VFk/zP3kBsELWNFi7rJtgbKYsav9QQ==",
             "optional": true,
             "os": [
                 "linux"
             ],
-            "resolved": "https://registry.npmjs.org/@rollup/rollup-linux-x64-gnu/-/rollup-linux-x64-gnu-4.17.1.tgz",
-            "version": "4.17.1"
+            "resolved": "https://registry.npmjs.org/@rollup/rollup-linux-x64-gnu/-/rollup-linux-x64-gnu-4.17.2.tgz",
+            "version": "4.17.2"
         },
         "node_modules/@rollup/rollup-linux-x64-musl": {
             "cpu": [
                 "x64"
             ],
             "dev": true,
-            "integrity": "sha512-KoB4fyKXTR+wYENkIG3fFF+5G6N4GFvzYx8Jax8BR4vmddtuqSb5oQmYu2Uu067vT/Fod7gxeQYKupm8gAcMSQ==",
+            "integrity": "sha512-h1+yTWeYbRdAyJ/jMiVw0l6fOOm/0D1vNLui9iPuqgRGnXA0u21gAqOyB5iHjlM9MMfNOm9RHCQ7zLIzT0x11Q==",
             "optional": true,
             "os": [
                 "linux"
             ],
-            "resolved": "https://registry.npmjs.org/@rollup/rollup-linux-x64-musl/-/rollup-linux-x64-musl-4.17.1.tgz",
-            "version": "4.17.1"
+            "resolved": "https://registry.npmjs.org/@rollup/rollup-linux-x64-musl/-/rollup-linux-x64-musl-4.17.2.tgz",
+            "version": "4.17.2"
         },
         "node_modules/@rollup/rollup-win32-arm64-msvc": {
             "cpu": [
                 "arm64"
             ],
             "dev": true,
-            "integrity": "sha512-J0d3NVNf7wBL9t4blCNat+d0PYqAx8wOoY+/9Q5cujnafbX7BmtYk3XvzkqLmFECaWvXGLuHmKj/wrILUinmQg==",
+            "integrity": "sha512-tmdtXMfKAjy5+IQsVtDiCfqbynAQE/TQRpWdVataHmhMb9DCoJxp9vLcCBjEQWMiUYxO1QprH/HbY9ragCEFLA==",
             "optional": true,
             "os": [
                 "win32"
             ],
-            "resolved": "https://registry.npmjs.org/@rollup/rollup-win32-arm64-msvc/-/rollup-win32-arm64-msvc-4.17.1.tgz",
-            "version": "4.17.1"
+            "resolved": "https://registry.npmjs.org/@rollup/rollup-win32-arm64-msvc/-/rollup-win32-arm64-msvc-4.17.2.tgz",
+            "version": "4.17.2"
         },
         "node_modules/@rollup/rollup-win32-ia32-msvc": {
             "cpu": [
                 "ia32"
             ],
             "dev": true,
-            "integrity": "sha512-xjgkWUwlq7IbgJSIxvl516FJ2iuC/7ttjsAxSPpC9kkI5iQQFHKyEN5BjbhvJ/IXIZ3yIBcW5QDlWAyrA+TFag==",
+            "integrity": "sha512-7II/QCSTAHuE5vdZaQEwJq2ZACkBpQDOmQsE6D6XUbnBHW8IAhm4eTufL6msLJorzrHDFv3CF8oCA/hSIRuZeQ==",
             "optional": true,
             "os": [
                 "win32"
             ],
-            "resolved": "https://registry.npmjs.org/@rollup/rollup-win32-ia32-msvc/-/rollup-win32-ia32-msvc-4.17.1.tgz",
-            "version": "4.17.1"
+            "resolved": "https://registry.npmjs.org/@rollup/rollup-win32-ia32-msvc/-/rollup-win32-ia32-msvc-4.17.2.tgz",
+            "version": "4.17.2"
         },
         "node_modules/@rollup/rollup-win32-x64-msvc": {
             "cpu": [
                 "x64"
             ],
             "dev": true,
-            "integrity": "sha512-0QbCkfk6cnnVKWqqlC0cUrrUMDMfu5ffvYMTUHf+qMN2uAb3MKP31LPcwiMXBNsvoFGs/kYdFOsuLmvppCopXA==",
+            "integrity": "sha512-TGGO7v7qOq4CYmSBVEYpI1Y5xDuCEnbVC5Vth8mOsW0gDSzxNrVERPc790IGHsrT2dQSimgMr9Ub3Y1Jci5/8w==",
             "optional": true,
             "os": [
                 "win32"
             ],
-            "resolved": "https://registry.npmjs.org/@rollup/rollup-win32-x64-msvc/-/rollup-win32-x64-msvc-4.17.1.tgz",
-            "version": "4.17.1"
+            "resolved": "https://registry.npmjs.org/@rollup/rollup-win32-x64-msvc/-/rollup-win32-x64-msvc-4.17.2.tgz",
+            "version": "4.17.2"
         },
         "node_modules/@sinclair/typebox": {
             "dev": true,
             "integrity": "sha512-+Fj43pSMwJs4KRrH/938Uf+uAELIgVBmQzg/q1YG10djyfA3TnrU8N8XzqCh/okZdszqBQTZf96idMfE5lnwTA==",
             "resolved": "https://registry.npmjs.org/@sinclair/typebox/-/typebox-0.27.8.tgz",
             "version": "0.27.8"
         },
@@ -1342,39 +1342,39 @@
                 "vue": "^3.2.25"
             },
             "resolved": "https://registry.npmjs.org/@vitejs/plugin-vue/-/plugin-vue-4.6.2.tgz",
             "version": "4.6.2"
         },
         "node_modules/@vitest/expect": {
             "dependencies": {
-                "@vitest/spy": "1.5.2",
-                "@vitest/utils": "1.5.2",
+                "@vitest/spy": "1.5.3",
+                "@vitest/utils": "1.5.3",
                 "chai": "^4.3.10"
             },
             "dev": true,
             "funding": {
                 "url": "https://opencollective.com/vitest"
             },
-            "integrity": "sha512-rf7MTD1WCoDlN3FfYJ9Llfp0PbdtOMZ3FIF0AVkDnKbp3oiMW1c8AmvRZBcqbAhDUAvF52e9zx4WQM1r3oraVA==",
-            "resolved": "https://registry.npmjs.org/@vitest/expect/-/expect-1.5.2.tgz",
-            "version": "1.5.2"
+            "integrity": "sha512-y+waPz31pOFr3rD7vWTbwiLe5+MgsMm40jTZbQE8p8/qXyBX3CQsIXRx9XK12IbY7q/t5a5aM/ckt33b4PxK2g==",
+            "resolved": "https://registry.npmjs.org/@vitest/expect/-/expect-1.5.3.tgz",
+            "version": "1.5.3"
         },
         "node_modules/@vitest/runner": {
             "dependencies": {
-                "@vitest/utils": "1.5.2",
+                "@vitest/utils": "1.5.3",
                 "p-limit": "^5.0.0",
                 "pathe": "^1.1.1"
             },
             "dev": true,
             "funding": {
                 "url": "https://opencollective.com/vitest"
             },
-            "integrity": "sha512-7IJ7sJhMZrqx7HIEpv3WrMYcq8ZNz9L6alo81Y6f8hV5mIE6yVZsFoivLZmr0D777klm1ReqonE9LyChdcmw6g==",
-            "resolved": "https://registry.npmjs.org/@vitest/runner/-/runner-1.5.2.tgz",
-            "version": "1.5.2"
+            "integrity": "sha512-7PlfuReN8692IKQIdCxwir1AOaP5THfNkp0Uc4BKr2na+9lALNit7ub9l3/R7MP8aV61+mHKRGiqEKRIwu6iiQ==",
+            "resolved": "https://registry.npmjs.org/@vitest/runner/-/runner-1.5.3.tgz",
+            "version": "1.5.3"
         },
         "node_modules/@vitest/runner/node_modules/p-limit": {
             "dependencies": {
                 "yocto-queue": "^1.0.0"
             },
             "dev": true,
             "engines": {
@@ -1405,44 +1405,44 @@
                 "pathe": "^1.1.1",
                 "pretty-format": "^29.7.0"
             },
             "dev": true,
             "funding": {
                 "url": "https://opencollective.com/vitest"
             },
-            "integrity": "sha512-CTEp/lTYos8fuCc9+Z55Ga5NVPKUgExritjF5VY7heRFUfheoAqBneUlvXSUJHUZPjnPmyZA96yLRJDP1QATFQ==",
-            "resolved": "https://registry.npmjs.org/@vitest/snapshot/-/snapshot-1.5.2.tgz",
-            "version": "1.5.2"
+            "integrity": "sha512-K3mvIsjyKYBhNIDujMD2gfQEzddLe51nNOAf45yKRt/QFJcUIeTQd2trRvv6M6oCBHNVnZwFWbQ4yj96ibiDsA==",
+            "resolved": "https://registry.npmjs.org/@vitest/snapshot/-/snapshot-1.5.3.tgz",
+            "version": "1.5.3"
         },
         "node_modules/@vitest/spy": {
             "dependencies": {
                 "tinyspy": "^2.2.0"
             },
             "dev": true,
             "funding": {
                 "url": "https://opencollective.com/vitest"
             },
-            "integrity": "sha512-xCcPvI8JpCtgikT9nLpHPL1/81AYqZy1GCy4+MCHBE7xi8jgsYkULpW5hrx5PGLgOQjUpb6fd15lqcriJ40tfQ==",
-            "resolved": "https://registry.npmjs.org/@vitest/spy/-/spy-1.5.2.tgz",
-            "version": "1.5.2"
+            "integrity": "sha512-Llj7Jgs6lbnL55WoshJUUacdJfjU2honvGcAJBxhra5TPEzTJH8ZuhI3p/JwqqfnTr4PmP7nDmOXP53MS7GJlg==",
+            "resolved": "https://registry.npmjs.org/@vitest/spy/-/spy-1.5.3.tgz",
+            "version": "1.5.3"
         },
         "node_modules/@vitest/utils": {
             "dependencies": {
                 "diff-sequences": "^29.6.3",
                 "estree-walker": "^3.0.3",
                 "loupe": "^2.3.7",
                 "pretty-format": "^29.7.0"
             },
             "dev": true,
             "funding": {
                 "url": "https://opencollective.com/vitest"
             },
-            "integrity": "sha512-sWOmyofuXLJ85VvXNsroZur7mOJGiQeM0JN3/0D1uU8U9bGFM69X1iqHaRXl6R8BwaLY6yPCogP257zxTzkUdA==",
-            "resolved": "https://registry.npmjs.org/@vitest/utils/-/utils-1.5.2.tgz",
-            "version": "1.5.2"
+            "integrity": "sha512-rE9DTN1BRhzkzqNQO+kw8ZgfeEBCLXiHJwetk668shmNBpSagQxneT5eSqEBLP+cqSiAeecvQmbpFfdMyLcIQA==",
+            "resolved": "https://registry.npmjs.org/@vitest/utils/-/utils-1.5.3.tgz",
+            "version": "1.5.3"
         },
         "node_modules/@vitest/utils/node_modules/estree-walker": {
             "dependencies": {
                 "@types/estree": "^1.0.0"
             },
             "dev": true,
             "integrity": "sha512-7RUKfXgSMMkzt6ZuXmqapOurLGPPfgj6l9uRZ7lRGolvk0y2yocc35LdcxKC5PQZdn2DMqioAQ2NoWcrTKmm6g==",
@@ -2364,17 +2364,17 @@
             "dev": true,
             "integrity": "sha512-I88TYZWc9XiYHRQ4/3c5rjjfgkjhLyW2luGIheGERbNQ6OY7yTybanSpDXZa8y7VUP9YmDcYa+eyq4ca7iLqWA==",
             "resolved": "https://registry.npmjs.org/eastasianwidth/-/eastasianwidth-0.2.0.tgz",
             "version": "0.2.0"
         },
         "node_modules/electron-to-chromium": {
             "dev": true,
-            "integrity": "sha512-9ItEpeu15hW5m8jKdriL+BQrgwDTXEL9pn4SkillWFu73ZNNNQ2BKKLS+ZHv2vC9UkNhosAeyfxOf/5OSeTCPA==",
-            "resolved": "https://registry.npmjs.org/electron-to-chromium/-/electron-to-chromium-1.4.750.tgz",
-            "version": "1.4.750"
+            "integrity": "sha512-7Kr5jUdns5rL/M9wFFmMZAgFDuL2YOnanFH4OI4iFzUqyh3XOL7nAGbSlSMZdzKMIyyTpNSbqZsWG9odwLeKvA==",
+            "resolved": "https://registry.npmjs.org/electron-to-chromium/-/electron-to-chromium-1.4.754.tgz",
+            "version": "1.4.754"
         },
         "node_modules/emoji-regex": {
             "dev": true,
             "integrity": "sha512-L18DaJsXSUk2+42pv8mLs5jJT2hqFkFE4j21wOmgbUqsZ2hL72NsUU785g9RXgo3s0ZNgVl42TiHp3ZtOv/Vyg==",
             "resolved": "https://registry.npmjs.org/emoji-regex/-/emoji-regex-9.2.2.tgz",
             "version": "9.2.2"
         },
@@ -3160,25 +3160,26 @@
             },
             "integrity": "sha512-AhO5QUcj8llrbG09iWhPU2B204J1xnPeL8kQmVorSsy+Sjj1sk8gIyh6cUocGmH4L0UuhAJy+hJMRA4mgA4mFQ==",
             "resolved": "https://registry.npmjs.org/globals/-/globals-13.24.0.tgz",
             "version": "13.24.0"
         },
         "node_modules/globalthis": {
             "dependencies": {
-                "define-properties": "^1.1.3"
+                "define-properties": "^1.2.1",
+                "gopd": "^1.0.1"
             },
             "engines": {
                 "node": ">= 0.4"
             },
             "funding": {
                 "url": "https://github.com/sponsors/ljharb"
             },
-            "integrity": "sha512-sFdI5LyBiNTHjRd7cGPWapiHWMOXKyuBNX/cWJ3NfzrZQVa8GI/8cofCl74AOVqq9W5kNmguTIzJ/1s2gyI9wA==",
-            "resolved": "https://registry.npmjs.org/globalthis/-/globalthis-1.0.3.tgz",
-            "version": "1.0.3"
+            "integrity": "sha512-DpLKbNU4WylpxJykQujfCcwYWiV/Jhm50Goo0wrVILAv5jOr9d+H+UR3PhSCD2rCCEIg0uc+G+muBTwD54JhDQ==",
+            "resolved": "https://registry.npmjs.org/globalthis/-/globalthis-1.0.4.tgz",
+            "version": "1.0.4"
         },
         "node_modules/gopd": {
             "dependencies": {
                 "get-intrinsic": "^1.1.3"
             },
             "funding": {
                 "url": "https://github.com/sponsors/ljharb"
@@ -3992,21 +3993,21 @@
             "resolved": "https://registry.npmjs.org/minipass/-/minipass-7.0.4.tgz",
             "version": "7.0.4"
         },
         "node_modules/mlly": {
             "dependencies": {
                 "acorn": "^8.11.3",
                 "pathe": "^1.1.2",
-                "pkg-types": "^1.0.3",
-                "ufo": "^1.3.2"
+                "pkg-types": "^1.1.0",
+                "ufo": "^1.5.3"
             },
             "dev": true,
-            "integrity": "sha512-vLgaHvaeunuOXHSmEbZ9izxPx3USsk8KCQ8iC+aTlp5sKRSoZvwhHh5L9VbKSaVC6sJDqbyohIS76E2VmHIPAA==",
-            "resolved": "https://registry.npmjs.org/mlly/-/mlly-1.6.1.tgz",
-            "version": "1.6.1"
+            "integrity": "sha512-U9SDaXGEREBYQgfejV97coK0UL1r+qnF2SyO9A3qcI8MzKnsIFKHNVEkrDyNncQTKQQumsasmeq84eNMdBfsNQ==",
+            "resolved": "https://registry.npmjs.org/mlly/-/mlly-1.7.0.tgz",
+            "version": "1.7.0"
         },
         "node_modules/mock-property": {
             "dependencies": {
                 "define-data-property": "^1.1.1",
                 "functions-have-names": "^1.2.3",
                 "gopd": "^1.0.1",
                 "has-property-descriptors": "^1.0.0",
@@ -4968,17 +4969,17 @@
                 "chokidar": ">=3.0.0 <4.0.0",
                 "immutable": "^4.0.0",
                 "source-map-js": ">=0.6.2 <2.0.0"
             },
             "engines": {
                 "node": ">=14.0.0"
             },
-            "integrity": "sha512-ShMYi3WkrDWxExyxSZPst4/okE9ts46xZmJDSawJQrnte7M1V9fScVB+uNXOVKRBt0PggHOwoZcn8mYX4trnBw==",
-            "resolved": "https://registry.npmjs.org/sass/-/sass-1.75.0.tgz",
-            "version": "1.75.0"
+            "integrity": "sha512-nc3LeqvF2FNW5xGF1zxZifdW3ffIz5aBb7I7tSvOoNu7z1RQ6pFt9MBuiPtjgaI62YWrM/txjWlOCFiGtf2xpw==",
+            "resolved": "https://registry.npmjs.org/sass/-/sass-1.76.0.tgz",
+            "version": "1.76.0"
         },
         "node_modules/scule": {
             "dev": true,
             "integrity": "sha512-6FtHJEvt+pVMIB9IBY+IcCJ6Z5f1iQnytgyfKMhDKgmzYG+TeH/wx1y3l27rshSbLiSanrR9ffZDrEsmjlQF2g==",
             "resolved": "https://registry.npmjs.org/scule/-/scule-1.3.0.tgz",
             "version": "1.3.0"
         },
@@ -5482,17 +5483,17 @@
                 "acorn": "^8.8.2",
                 "commander": "^2.20.0",
                 "source-map-support": "~0.5.20"
             },
             "engines": {
                 "node": ">=10"
             },
-            "integrity": "sha512-xRdd0v64a8mFK9bnsKVdoNP9GQIKUAaJPTaqEQDL4w/J8WaW4sWXXoMZ+6SimPkfT5bElreXf8m9HnmPc3E1BQ==",
-            "resolved": "https://registry.npmjs.org/terser/-/terser-5.30.4.tgz",
-            "version": "5.30.4"
+            "integrity": "sha512-Q1JFAoUKE5IMfI4Z/lkE/E6+SwgzO+x4tq4v1AyBLRj8VSYvRO6A/rQrPg1yud4g0En9EKI1TvFRF2tQFcoUkg==",
+            "resolved": "https://registry.npmjs.org/terser/-/terser-5.31.0.tgz",
+            "version": "5.31.0"
         },
         "node_modules/terser/node_modules/commander": {
             "integrity": "sha512-GpVkmM8vF2vQUkj2LvZmD35JxeJOLCwJ9cUkugyk2nuhbv3+mJvpLYYt+0+USMxE+oj+ey/lJEnhZw75x/OMcQ==",
             "resolved": "https://registry.npmjs.org/commander/-/commander-2.20.3.tgz",
             "version": "2.20.3"
         },
         "node_modules/terser/node_modules/source-map": {
@@ -5939,15 +5940,15 @@
             "version": "7.4.6"
         },
         "node_modules/update-browserslist-db": {
             "bin": {
                 "update-browserslist-db": "cli.js"
             },
             "dependencies": {
-                "escalade": "^3.1.1",
+                "escalade": "^3.1.2",
                 "picocolors": "^1.0.0"
             },
             "dev": true,
             "funding": [
                 {
                     "type": "opencollective",
                     "url": "https://opencollective.com/browserslist"
@@ -5957,20 +5958,20 @@
                     "url": "https://tidelift.com/funding/github/npm/browserslist"
                 },
                 {
                     "type": "github",
                     "url": "https://github.com/sponsors/ai"
                 }
             ],
-            "integrity": "sha512-xebP81SNcPuNpPP3uzeW1NYXxI3rxyJzF3pD6sH4jE7o/IX+WtSpwnVU+qIsDPyk0d3hmFQ7mjqc6AtV604hbg==",
+            "integrity": "sha512-JixKH8GR2pWYshIPUg/NujK3JO7JiqEEUiNArE86NQyrgUuZeTlZQN3xuS/yiV5Kb48ev9K6RqNkaJjXsdg7Jw==",
             "peerDependencies": {
                 "browserslist": ">= 4.21.0"
             },
-            "resolved": "https://registry.npmjs.org/update-browserslist-db/-/update-browserslist-db-1.0.13.tgz",
-            "version": "1.0.13"
+            "resolved": "https://registry.npmjs.org/update-browserslist-db/-/update-browserslist-db-1.0.14.tgz",
+            "version": "1.0.14"
         },
         "node_modules/uri-js": {
             "dependencies": {
                 "punycode": "^2.1.0"
             },
             "dev": true,
             "integrity": "sha512-7rKUyy33Q1yc98pQ1DAmLtwX109F7TIfWlW1Ydo8Wl1ii1SeHieeh0HHfPeL2fMXK6z0s8ecKs9frCuLJvndBg==",
@@ -6052,17 +6053,17 @@
             "dev": true,
             "engines": {
                 "node": "^18.0.0 || >=20.0.0"
             },
             "funding": {
                 "url": "https://opencollective.com/vitest"
             },
-            "integrity": "sha512-Y8p91kz9zU+bWtF7HGt6DVw2JbhyuB2RlZix3FPYAYmUyZ3n7iTp8eSyLyY6sxtPegvxQtmlTMhfPhUfCUF93A==",
-            "resolved": "https://registry.npmjs.org/vite-node/-/vite-node-1.5.2.tgz",
-            "version": "1.5.2"
+            "integrity": "sha512-axFo00qiCpU/JLd8N1gu9iEYL3xTbMbMrbe5nDp9GL0nb6gurIdZLkkFogZXWnE8Oyy5kfSLwNVIcVsnhE7lgQ==",
+            "resolved": "https://registry.npmjs.org/vite-node/-/vite-node-1.5.3.tgz",
+            "version": "1.5.3"
         },
         "node_modules/vite-plugin-json5": {
             "dependencies": {
                 "json5": "^2.2.3"
             },
             "dev": true,
             "integrity": "sha512-V0EowrUhYRXAYPy62L9KLgPqd1L7lfVZcjvLh1fj+DIo5X2t6DT2/HOoiAV9FE4YEljdgFJByA+XwKxZ78uQww==",
@@ -6081,76 +6082,76 @@
                 "@types/estree": "1.0.5"
             },
             "dev": true,
             "engines": {
                 "node": ">=18.0.0",
                 "npm": ">=8.0.0"
             },
-            "integrity": "sha512-0gG94inrUtg25sB2V/pApwiv1lUb0bQ25FPNuzO89Baa+B+c0ccaaBKM5zkZV/12pUUdH+lWCSm9wmHqyocuVQ==",
+            "integrity": "sha512-/9ClTJPByC0U4zNLowV1tMBe8yMEAxewtR3cUNX5BoEpGH3dQEWpJLr6CLp0fPdYRF/fzVOgvDb1zXuakwF5kQ==",
             "optionalDependencies": {
-                "@rollup/rollup-android-arm-eabi": "4.17.1",
-                "@rollup/rollup-android-arm64": "4.17.1",
-                "@rollup/rollup-darwin-arm64": "4.17.1",
-                "@rollup/rollup-darwin-x64": "4.17.1",
-                "@rollup/rollup-linux-arm-gnueabihf": "4.17.1",
-                "@rollup/rollup-linux-arm-musleabihf": "4.17.1",
-                "@rollup/rollup-linux-arm64-gnu": "4.17.1",
-                "@rollup/rollup-linux-arm64-musl": "4.17.1",
-                "@rollup/rollup-linux-powerpc64le-gnu": "4.17.1",
-                "@rollup/rollup-linux-riscv64-gnu": "4.17.1",
-                "@rollup/rollup-linux-s390x-gnu": "4.17.1",
-                "@rollup/rollup-linux-x64-gnu": "4.17.1",
-                "@rollup/rollup-linux-x64-musl": "4.17.1",
-                "@rollup/rollup-win32-arm64-msvc": "4.17.1",
-                "@rollup/rollup-win32-ia32-msvc": "4.17.1",
-                "@rollup/rollup-win32-x64-msvc": "4.17.1",
+                "@rollup/rollup-android-arm-eabi": "4.17.2",
+                "@rollup/rollup-android-arm64": "4.17.2",
+                "@rollup/rollup-darwin-arm64": "4.17.2",
+                "@rollup/rollup-darwin-x64": "4.17.2",
+                "@rollup/rollup-linux-arm-gnueabihf": "4.17.2",
+                "@rollup/rollup-linux-arm-musleabihf": "4.17.2",
+                "@rollup/rollup-linux-arm64-gnu": "4.17.2",
+                "@rollup/rollup-linux-arm64-musl": "4.17.2",
+                "@rollup/rollup-linux-powerpc64le-gnu": "4.17.2",
+                "@rollup/rollup-linux-riscv64-gnu": "4.17.2",
+                "@rollup/rollup-linux-s390x-gnu": "4.17.2",
+                "@rollup/rollup-linux-x64-gnu": "4.17.2",
+                "@rollup/rollup-linux-x64-musl": "4.17.2",
+                "@rollup/rollup-win32-arm64-msvc": "4.17.2",
+                "@rollup/rollup-win32-ia32-msvc": "4.17.2",
+                "@rollup/rollup-win32-x64-msvc": "4.17.2",
                 "fsevents": "~2.3.2"
             },
-            "resolved": "https://registry.npmjs.org/rollup/-/rollup-4.17.1.tgz",
-            "version": "4.17.1"
+            "resolved": "https://registry.npmjs.org/rollup/-/rollup-4.17.2.tgz",
+            "version": "4.17.2"
         },
         "node_modules/vitest": {
             "bin": {
                 "vitest": "vitest.mjs"
             },
             "dependencies": {
-                "@vitest/expect": "1.5.2",
-                "@vitest/runner": "1.5.2",
-                "@vitest/snapshot": "1.5.2",
-                "@vitest/spy": "1.5.2",
-                "@vitest/utils": "1.5.2",
+                "@vitest/expect": "1.5.3",
+                "@vitest/runner": "1.5.3",
+                "@vitest/snapshot": "1.5.3",
+                "@vitest/spy": "1.5.3",
+                "@vitest/utils": "1.5.3",
                 "acorn-walk": "^8.3.2",
                 "chai": "^4.3.10",
                 "debug": "^4.3.4",
                 "execa": "^8.0.1",
                 "local-pkg": "^0.5.0",
                 "magic-string": "^0.30.5",
                 "pathe": "^1.1.1",
                 "picocolors": "^1.0.0",
                 "std-env": "^3.5.0",
                 "strip-literal": "^2.0.0",
                 "tinybench": "^2.5.1",
                 "tinypool": "^0.8.3",
                 "vite": "^5.0.0",
-                "vite-node": "1.5.2",
+                "vite-node": "1.5.3",
                 "why-is-node-running": "^2.2.2"
             },
             "dev": true,
             "engines": {
                 "node": "^18.0.0 || >=20.0.0"
             },
             "funding": {
                 "url": "https://opencollective.com/vitest"
             },
-            "integrity": "sha512-l9gwIkq16ug3xY7BxHwcBQovLZG75zZL0PlsiYQbf76Rz6QGs54416UWMtC0jXeihvHvcHrf2ROEjkQRVpoZYw==",
+            "integrity": "sha512-2oM7nLXylw3mQlW6GXnRriw+7YvZFk/YNV8AxIC3Z3MfFbuziLGWP9GPxxu/7nRlXhqyxBikpamr+lEEj1sUEw==",
             "peerDependencies": {
                 "@edge-runtime/vm": "*",
                 "@types/node": "^18.0.0 || >=20.0.0",
-                "@vitest/browser": "1.5.2",
-                "@vitest/ui": "1.5.2",
+                "@vitest/browser": "1.5.3",
+                "@vitest/ui": "1.5.3",
                 "happy-dom": "*",
                 "jsdom": "*"
             },
             "peerDependenciesMeta": {
                 "@edge-runtime/vm": {
                     "optional": true
                 },
@@ -6166,16 +6167,16 @@
                 "happy-dom": {
                     "optional": true
                 },
                 "jsdom": {
                     "optional": true
                 }
             },
-            "resolved": "https://registry.npmjs.org/vitest/-/vitest-1.5.2.tgz",
-            "version": "1.5.2"
+            "resolved": "https://registry.npmjs.org/vitest/-/vitest-1.5.3.tgz",
+            "version": "1.5.3"
         },
         "node_modules/vitest/node_modules/local-pkg": {
             "dependencies": {
                 "mlly": "^1.4.2",
                 "pkg-types": "^1.0.3"
             },
             "dev": true,
```

### Comparing `swanlab-0.3.0/package.json` & `swanlab-0.3.1/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/.vscode/extensions.json` & `swanlab-0.3.1/.vscode/extensions.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/.vscode/launch.json` & `swanlab-0.3.1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/.vscode/settings.json` & `swanlab-0.3.1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/.vscode/tailwind.json` & `swanlab-0.3.1/.vscode/tailwind.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/.package-lock.json` & `swanlab-0.3.1/node_modules/.package-lock.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995614961106642%*

 * *Differences: {"'packages'": "{'node_modules/@babel/parser': {'version': '7.24.5', 'resolved': "*

 * *               "'https://registry.npmjs.org/@babel/parser/-/parser-7.24.5.tgz', 'integrity': "*

 * *               "'sha512-EOv5IK8arwh3LI47dz1b0tKUb/1uhHAnHJOrjgtQMIpu1uXd9mlFrJg9IUgGUgZ41Ch0K8REPTYpO7B76b4vJg=='}, "*

 * *               "'node_modules/@rollup/rollup-linux-x64-gnu': {'version': '4.17.2', 'resolved': "*

 * *               "'https://registry.npmjs.org/@rollup/rollup-linux-x64-gnu/-/rollup-linux-x64-gnu-4.17.2.tgz', "*

 * *         […]*

```diff
@@ -314,17 +314,17 @@
         "node_modules/@babel/parser": {
             "bin": {
                 "parser": "bin/babel-parser.js"
             },
             "engines": {
                 "node": ">=6.0.0"
             },
-            "integrity": "sha512-zTvEBcghmeBma9QIGunWevvBAp4/Qu9Bdq+2k0Ot4fVMD6v3dsC9WOcRSKk7tRRyBM/53yKMJko9xOatGQAwSg==",
-            "resolved": "https://registry.npmjs.org/@babel/parser/-/parser-7.24.4.tgz",
-            "version": "7.24.4"
+            "integrity": "sha512-EOv5IK8arwh3LI47dz1b0tKUb/1uhHAnHJOrjgtQMIpu1uXd9mlFrJg9IUgGUgZ41Ch0K8REPTYpO7B76b4vJg==",
+            "resolved": "https://registry.npmjs.org/@babel/parser/-/parser-7.24.5.tgz",
+            "version": "7.24.5"
         },
         "node_modules/@esbuild/linux-x64": {
             "cpu": [
                 "x64"
             ],
             "dev": true,
             "engines": {
@@ -689,34 +689,34 @@
             "version": "5.1.0"
         },
         "node_modules/@rollup/rollup-linux-x64-gnu": {
             "cpu": [
                 "x64"
             ],
             "dev": true,
-            "integrity": "sha512-AsdnINQoDWfKpBzCPqQWxSPdAWzSgnYbrJYtn6W0H2E9It5bZss99PiLA8CgmDRfvKygt20UpZ3xkhFlIfX9zQ==",
+            "integrity": "sha512-Hy7pLwByUOuyaFC6mAr7m+oMC+V7qyifzs/nW2OJfC8H4hbCzOX07Ov0VFk/zP3kBsELWNFi7rJtgbKYsav9QQ==",
             "optional": true,
             "os": [
                 "linux"
             ],
-            "resolved": "https://registry.npmjs.org/@rollup/rollup-linux-x64-gnu/-/rollup-linux-x64-gnu-4.17.1.tgz",
-            "version": "4.17.1"
+            "resolved": "https://registry.npmjs.org/@rollup/rollup-linux-x64-gnu/-/rollup-linux-x64-gnu-4.17.2.tgz",
+            "version": "4.17.2"
         },
         "node_modules/@rollup/rollup-linux-x64-musl": {
             "cpu": [
                 "x64"
             ],
             "dev": true,
-            "integrity": "sha512-KoB4fyKXTR+wYENkIG3fFF+5G6N4GFvzYx8Jax8BR4vmddtuqSb5oQmYu2Uu067vT/Fod7gxeQYKupm8gAcMSQ==",
+            "integrity": "sha512-h1+yTWeYbRdAyJ/jMiVw0l6fOOm/0D1vNLui9iPuqgRGnXA0u21gAqOyB5iHjlM9MMfNOm9RHCQ7zLIzT0x11Q==",
             "optional": true,
             "os": [
                 "linux"
             ],
-            "resolved": "https://registry.npmjs.org/@rollup/rollup-linux-x64-musl/-/rollup-linux-x64-musl-4.17.1.tgz",
-            "version": "4.17.1"
+            "resolved": "https://registry.npmjs.org/@rollup/rollup-linux-x64-musl/-/rollup-linux-x64-musl-4.17.2.tgz",
+            "version": "4.17.2"
         },
         "node_modules/@sinclair/typebox": {
             "dev": true,
             "integrity": "sha512-+Fj43pSMwJs4KRrH/938Uf+uAELIgVBmQzg/q1YG10djyfA3TnrU8N8XzqCh/okZdszqBQTZf96idMfE5lnwTA==",
             "resolved": "https://registry.npmjs.org/@sinclair/typebox/-/typebox-0.27.8.tgz",
             "version": "0.27.8"
         },
@@ -772,39 +772,39 @@
                 "vue": "^3.2.25"
             },
             "resolved": "https://registry.npmjs.org/@vitejs/plugin-vue/-/plugin-vue-4.6.2.tgz",
             "version": "4.6.2"
         },
         "node_modules/@vitest/expect": {
             "dependencies": {
-                "@vitest/spy": "1.5.2",
-                "@vitest/utils": "1.5.2",
+                "@vitest/spy": "1.5.3",
+                "@vitest/utils": "1.5.3",
                 "chai": "^4.3.10"
             },
             "dev": true,
             "funding": {
                 "url": "https://opencollective.com/vitest"
             },
-            "integrity": "sha512-rf7MTD1WCoDlN3FfYJ9Llfp0PbdtOMZ3FIF0AVkDnKbp3oiMW1c8AmvRZBcqbAhDUAvF52e9zx4WQM1r3oraVA==",
-            "resolved": "https://registry.npmjs.org/@vitest/expect/-/expect-1.5.2.tgz",
-            "version": "1.5.2"
+            "integrity": "sha512-y+waPz31pOFr3rD7vWTbwiLe5+MgsMm40jTZbQE8p8/qXyBX3CQsIXRx9XK12IbY7q/t5a5aM/ckt33b4PxK2g==",
+            "resolved": "https://registry.npmjs.org/@vitest/expect/-/expect-1.5.3.tgz",
+            "version": "1.5.3"
         },
         "node_modules/@vitest/runner": {
             "dependencies": {
-                "@vitest/utils": "1.5.2",
+                "@vitest/utils": "1.5.3",
                 "p-limit": "^5.0.0",
                 "pathe": "^1.1.1"
             },
             "dev": true,
             "funding": {
                 "url": "https://opencollective.com/vitest"
             },
-            "integrity": "sha512-7IJ7sJhMZrqx7HIEpv3WrMYcq8ZNz9L6alo81Y6f8hV5mIE6yVZsFoivLZmr0D777klm1ReqonE9LyChdcmw6g==",
-            "resolved": "https://registry.npmjs.org/@vitest/runner/-/runner-1.5.2.tgz",
-            "version": "1.5.2"
+            "integrity": "sha512-7PlfuReN8692IKQIdCxwir1AOaP5THfNkp0Uc4BKr2na+9lALNit7ub9l3/R7MP8aV61+mHKRGiqEKRIwu6iiQ==",
+            "resolved": "https://registry.npmjs.org/@vitest/runner/-/runner-1.5.3.tgz",
+            "version": "1.5.3"
         },
         "node_modules/@vitest/runner/node_modules/p-limit": {
             "dependencies": {
                 "yocto-queue": "^1.0.0"
             },
             "dev": true,
             "engines": {
@@ -835,44 +835,44 @@
                 "pathe": "^1.1.1",
                 "pretty-format": "^29.7.0"
             },
             "dev": true,
             "funding": {
                 "url": "https://opencollective.com/vitest"
             },
-            "integrity": "sha512-CTEp/lTYos8fuCc9+Z55Ga5NVPKUgExritjF5VY7heRFUfheoAqBneUlvXSUJHUZPjnPmyZA96yLRJDP1QATFQ==",
-            "resolved": "https://registry.npmjs.org/@vitest/snapshot/-/snapshot-1.5.2.tgz",
-            "version": "1.5.2"
+            "integrity": "sha512-K3mvIsjyKYBhNIDujMD2gfQEzddLe51nNOAf45yKRt/QFJcUIeTQd2trRvv6M6oCBHNVnZwFWbQ4yj96ibiDsA==",
+            "resolved": "https://registry.npmjs.org/@vitest/snapshot/-/snapshot-1.5.3.tgz",
+            "version": "1.5.3"
         },
         "node_modules/@vitest/spy": {
             "dependencies": {
                 "tinyspy": "^2.2.0"
             },
             "dev": true,
             "funding": {
                 "url": "https://opencollective.com/vitest"
             },
-            "integrity": "sha512-xCcPvI8JpCtgikT9nLpHPL1/81AYqZy1GCy4+MCHBE7xi8jgsYkULpW5hrx5PGLgOQjUpb6fd15lqcriJ40tfQ==",
-            "resolved": "https://registry.npmjs.org/@vitest/spy/-/spy-1.5.2.tgz",
-            "version": "1.5.2"
+            "integrity": "sha512-Llj7Jgs6lbnL55WoshJUUacdJfjU2honvGcAJBxhra5TPEzTJH8ZuhI3p/JwqqfnTr4PmP7nDmOXP53MS7GJlg==",
+            "resolved": "https://registry.npmjs.org/@vitest/spy/-/spy-1.5.3.tgz",
+            "version": "1.5.3"
         },
         "node_modules/@vitest/utils": {
             "dependencies": {
                 "diff-sequences": "^29.6.3",
                 "estree-walker": "^3.0.3",
                 "loupe": "^2.3.7",
                 "pretty-format": "^29.7.0"
             },
             "dev": true,
             "funding": {
                 "url": "https://opencollective.com/vitest"
             },
-            "integrity": "sha512-sWOmyofuXLJ85VvXNsroZur7mOJGiQeM0JN3/0D1uU8U9bGFM69X1iqHaRXl6R8BwaLY6yPCogP257zxTzkUdA==",
-            "resolved": "https://registry.npmjs.org/@vitest/utils/-/utils-1.5.2.tgz",
-            "version": "1.5.2"
+            "integrity": "sha512-rE9DTN1BRhzkzqNQO+kw8ZgfeEBCLXiHJwetk668shmNBpSagQxneT5eSqEBLP+cqSiAeecvQmbpFfdMyLcIQA==",
+            "resolved": "https://registry.npmjs.org/@vitest/utils/-/utils-1.5.3.tgz",
+            "version": "1.5.3"
         },
         "node_modules/@vitest/utils/node_modules/estree-walker": {
             "dependencies": {
                 "@types/estree": "^1.0.0"
             },
             "dev": true,
             "integrity": "sha512-7RUKfXgSMMkzt6ZuXmqapOurLGPPfgj6l9uRZ7lRGolvk0y2yocc35LdcxKC5PQZdn2DMqioAQ2NoWcrTKmm6g==",
@@ -1794,17 +1794,17 @@
             "dev": true,
             "integrity": "sha512-I88TYZWc9XiYHRQ4/3c5rjjfgkjhLyW2luGIheGERbNQ6OY7yTybanSpDXZa8y7VUP9YmDcYa+eyq4ca7iLqWA==",
             "resolved": "https://registry.npmjs.org/eastasianwidth/-/eastasianwidth-0.2.0.tgz",
             "version": "0.2.0"
         },
         "node_modules/electron-to-chromium": {
             "dev": true,
-            "integrity": "sha512-9ItEpeu15hW5m8jKdriL+BQrgwDTXEL9pn4SkillWFu73ZNNNQ2BKKLS+ZHv2vC9UkNhosAeyfxOf/5OSeTCPA==",
-            "resolved": "https://registry.npmjs.org/electron-to-chromium/-/electron-to-chromium-1.4.750.tgz",
-            "version": "1.4.750"
+            "integrity": "sha512-7Kr5jUdns5rL/M9wFFmMZAgFDuL2YOnanFH4OI4iFzUqyh3XOL7nAGbSlSMZdzKMIyyTpNSbqZsWG9odwLeKvA==",
+            "resolved": "https://registry.npmjs.org/electron-to-chromium/-/electron-to-chromium-1.4.754.tgz",
+            "version": "1.4.754"
         },
         "node_modules/emoji-regex": {
             "dev": true,
             "integrity": "sha512-L18DaJsXSUk2+42pv8mLs5jJT2hqFkFE4j21wOmgbUqsZ2hL72NsUU785g9RXgo3s0ZNgVl42TiHp3ZtOv/Vyg==",
             "resolved": "https://registry.npmjs.org/emoji-regex/-/emoji-regex-9.2.2.tgz",
             "version": "9.2.2"
         },
@@ -2577,25 +2577,26 @@
             },
             "integrity": "sha512-AhO5QUcj8llrbG09iWhPU2B204J1xnPeL8kQmVorSsy+Sjj1sk8gIyh6cUocGmH4L0UuhAJy+hJMRA4mgA4mFQ==",
             "resolved": "https://registry.npmjs.org/globals/-/globals-13.24.0.tgz",
             "version": "13.24.0"
         },
         "node_modules/globalthis": {
             "dependencies": {
-                "define-properties": "^1.1.3"
+                "define-properties": "^1.2.1",
+                "gopd": "^1.0.1"
             },
             "engines": {
                 "node": ">= 0.4"
             },
             "funding": {
                 "url": "https://github.com/sponsors/ljharb"
             },
-            "integrity": "sha512-sFdI5LyBiNTHjRd7cGPWapiHWMOXKyuBNX/cWJ3NfzrZQVa8GI/8cofCl74AOVqq9W5kNmguTIzJ/1s2gyI9wA==",
-            "resolved": "https://registry.npmjs.org/globalthis/-/globalthis-1.0.3.tgz",
-            "version": "1.0.3"
+            "integrity": "sha512-DpLKbNU4WylpxJykQujfCcwYWiV/Jhm50Goo0wrVILAv5jOr9d+H+UR3PhSCD2rCCEIg0uc+G+muBTwD54JhDQ==",
+            "resolved": "https://registry.npmjs.org/globalthis/-/globalthis-1.0.4.tgz",
+            "version": "1.0.4"
         },
         "node_modules/gopd": {
             "dependencies": {
                 "get-intrinsic": "^1.1.3"
             },
             "funding": {
                 "url": "https://github.com/sponsors/ljharb"
@@ -3409,21 +3410,21 @@
             "resolved": "https://registry.npmjs.org/minipass/-/minipass-7.0.4.tgz",
             "version": "7.0.4"
         },
         "node_modules/mlly": {
             "dependencies": {
                 "acorn": "^8.11.3",
                 "pathe": "^1.1.2",
-                "pkg-types": "^1.0.3",
-                "ufo": "^1.3.2"
+                "pkg-types": "^1.1.0",
+                "ufo": "^1.5.3"
             },
             "dev": true,
-            "integrity": "sha512-vLgaHvaeunuOXHSmEbZ9izxPx3USsk8KCQ8iC+aTlp5sKRSoZvwhHh5L9VbKSaVC6sJDqbyohIS76E2VmHIPAA==",
-            "resolved": "https://registry.npmjs.org/mlly/-/mlly-1.6.1.tgz",
-            "version": "1.6.1"
+            "integrity": "sha512-U9SDaXGEREBYQgfejV97coK0UL1r+qnF2SyO9A3qcI8MzKnsIFKHNVEkrDyNncQTKQQumsasmeq84eNMdBfsNQ==",
+            "resolved": "https://registry.npmjs.org/mlly/-/mlly-1.7.0.tgz",
+            "version": "1.7.0"
         },
         "node_modules/mock-property": {
             "dependencies": {
                 "define-data-property": "^1.1.1",
                 "functions-have-names": "^1.2.3",
                 "gopd": "^1.0.1",
                 "has-property-descriptors": "^1.0.0",
@@ -4385,17 +4386,17 @@
                 "chokidar": ">=3.0.0 <4.0.0",
                 "immutable": "^4.0.0",
                 "source-map-js": ">=0.6.2 <2.0.0"
             },
             "engines": {
                 "node": ">=14.0.0"
             },
-            "integrity": "sha512-ShMYi3WkrDWxExyxSZPst4/okE9ts46xZmJDSawJQrnte7M1V9fScVB+uNXOVKRBt0PggHOwoZcn8mYX4trnBw==",
-            "resolved": "https://registry.npmjs.org/sass/-/sass-1.75.0.tgz",
-            "version": "1.75.0"
+            "integrity": "sha512-nc3LeqvF2FNW5xGF1zxZifdW3ffIz5aBb7I7tSvOoNu7z1RQ6pFt9MBuiPtjgaI62YWrM/txjWlOCFiGtf2xpw==",
+            "resolved": "https://registry.npmjs.org/sass/-/sass-1.76.0.tgz",
+            "version": "1.76.0"
         },
         "node_modules/scule": {
             "dev": true,
             "integrity": "sha512-6FtHJEvt+pVMIB9IBY+IcCJ6Z5f1iQnytgyfKMhDKgmzYG+TeH/wx1y3l27rshSbLiSanrR9ffZDrEsmjlQF2g==",
             "resolved": "https://registry.npmjs.org/scule/-/scule-1.3.0.tgz",
             "version": "1.3.0"
         },
@@ -4899,17 +4900,17 @@
                 "acorn": "^8.8.2",
                 "commander": "^2.20.0",
                 "source-map-support": "~0.5.20"
             },
             "engines": {
                 "node": ">=10"
             },
-            "integrity": "sha512-xRdd0v64a8mFK9bnsKVdoNP9GQIKUAaJPTaqEQDL4w/J8WaW4sWXXoMZ+6SimPkfT5bElreXf8m9HnmPc3E1BQ==",
-            "resolved": "https://registry.npmjs.org/terser/-/terser-5.30.4.tgz",
-            "version": "5.30.4"
+            "integrity": "sha512-Q1JFAoUKE5IMfI4Z/lkE/E6+SwgzO+x4tq4v1AyBLRj8VSYvRO6A/rQrPg1yud4g0En9EKI1TvFRF2tQFcoUkg==",
+            "resolved": "https://registry.npmjs.org/terser/-/terser-5.31.0.tgz",
+            "version": "5.31.0"
         },
         "node_modules/terser/node_modules/commander": {
             "integrity": "sha512-GpVkmM8vF2vQUkj2LvZmD35JxeJOLCwJ9cUkugyk2nuhbv3+mJvpLYYt+0+USMxE+oj+ey/lJEnhZw75x/OMcQ==",
             "resolved": "https://registry.npmjs.org/commander/-/commander-2.20.3.tgz",
             "version": "2.20.3"
         },
         "node_modules/terser/node_modules/source-map": {
@@ -5356,15 +5357,15 @@
             "version": "7.4.6"
         },
         "node_modules/update-browserslist-db": {
             "bin": {
                 "update-browserslist-db": "cli.js"
             },
             "dependencies": {
-                "escalade": "^3.1.1",
+                "escalade": "^3.1.2",
                 "picocolors": "^1.0.0"
             },
             "dev": true,
             "funding": [
                 {
                     "type": "opencollective",
                     "url": "https://opencollective.com/browserslist"
@@ -5374,20 +5375,20 @@
                     "url": "https://tidelift.com/funding/github/npm/browserslist"
                 },
                 {
                     "type": "github",
                     "url": "https://github.com/sponsors/ai"
                 }
             ],
-            "integrity": "sha512-xebP81SNcPuNpPP3uzeW1NYXxI3rxyJzF3pD6sH4jE7o/IX+WtSpwnVU+qIsDPyk0d3hmFQ7mjqc6AtV604hbg==",
+            "integrity": "sha512-JixKH8GR2pWYshIPUg/NujK3JO7JiqEEUiNArE86NQyrgUuZeTlZQN3xuS/yiV5Kb48ev9K6RqNkaJjXsdg7Jw==",
             "peerDependencies": {
                 "browserslist": ">= 4.21.0"
             },
-            "resolved": "https://registry.npmjs.org/update-browserslist-db/-/update-browserslist-db-1.0.13.tgz",
-            "version": "1.0.13"
+            "resolved": "https://registry.npmjs.org/update-browserslist-db/-/update-browserslist-db-1.0.14.tgz",
+            "version": "1.0.14"
         },
         "node_modules/uri-js": {
             "dependencies": {
                 "punycode": "^2.1.0"
             },
             "dev": true,
             "integrity": "sha512-7rKUyy33Q1yc98pQ1DAmLtwX109F7TIfWlW1Ydo8Wl1ii1SeHieeh0HHfPeL2fMXK6z0s8ecKs9frCuLJvndBg==",
@@ -5469,17 +5470,17 @@
             "dev": true,
             "engines": {
                 "node": "^18.0.0 || >=20.0.0"
             },
             "funding": {
                 "url": "https://opencollective.com/vitest"
             },
-            "integrity": "sha512-Y8p91kz9zU+bWtF7HGt6DVw2JbhyuB2RlZix3FPYAYmUyZ3n7iTp8eSyLyY6sxtPegvxQtmlTMhfPhUfCUF93A==",
-            "resolved": "https://registry.npmjs.org/vite-node/-/vite-node-1.5.2.tgz",
-            "version": "1.5.2"
+            "integrity": "sha512-axFo00qiCpU/JLd8N1gu9iEYL3xTbMbMrbe5nDp9GL0nb6gurIdZLkkFogZXWnE8Oyy5kfSLwNVIcVsnhE7lgQ==",
+            "resolved": "https://registry.npmjs.org/vite-node/-/vite-node-1.5.3.tgz",
+            "version": "1.5.3"
         },
         "node_modules/vite-plugin-json5": {
             "dependencies": {
                 "json5": "^2.2.3"
             },
             "dev": true,
             "integrity": "sha512-V0EowrUhYRXAYPy62L9KLgPqd1L7lfVZcjvLh1fj+DIo5X2t6DT2/HOoiAV9FE4YEljdgFJByA+XwKxZ78uQww==",
@@ -5498,76 +5499,76 @@
                 "@types/estree": "1.0.5"
             },
             "dev": true,
             "engines": {
                 "node": ">=18.0.0",
                 "npm": ">=8.0.0"
             },
-            "integrity": "sha512-0gG94inrUtg25sB2V/pApwiv1lUb0bQ25FPNuzO89Baa+B+c0ccaaBKM5zkZV/12pUUdH+lWCSm9wmHqyocuVQ==",
+            "integrity": "sha512-/9ClTJPByC0U4zNLowV1tMBe8yMEAxewtR3cUNX5BoEpGH3dQEWpJLr6CLp0fPdYRF/fzVOgvDb1zXuakwF5kQ==",
             "optionalDependencies": {
-                "@rollup/rollup-android-arm-eabi": "4.17.1",
-                "@rollup/rollup-android-arm64": "4.17.1",
-                "@rollup/rollup-darwin-arm64": "4.17.1",
-                "@rollup/rollup-darwin-x64": "4.17.1",
-                "@rollup/rollup-linux-arm-gnueabihf": "4.17.1",
-                "@rollup/rollup-linux-arm-musleabihf": "4.17.1",
-                "@rollup/rollup-linux-arm64-gnu": "4.17.1",
-                "@rollup/rollup-linux-arm64-musl": "4.17.1",
-                "@rollup/rollup-linux-powerpc64le-gnu": "4.17.1",
-                "@rollup/rollup-linux-riscv64-gnu": "4.17.1",
-                "@rollup/rollup-linux-s390x-gnu": "4.17.1",
-                "@rollup/rollup-linux-x64-gnu": "4.17.1",
-                "@rollup/rollup-linux-x64-musl": "4.17.1",
-                "@rollup/rollup-win32-arm64-msvc": "4.17.1",
-                "@rollup/rollup-win32-ia32-msvc": "4.17.1",
-                "@rollup/rollup-win32-x64-msvc": "4.17.1",
+                "@rollup/rollup-android-arm-eabi": "4.17.2",
+                "@rollup/rollup-android-arm64": "4.17.2",
+                "@rollup/rollup-darwin-arm64": "4.17.2",
+                "@rollup/rollup-darwin-x64": "4.17.2",
+                "@rollup/rollup-linux-arm-gnueabihf": "4.17.2",
+                "@rollup/rollup-linux-arm-musleabihf": "4.17.2",
+                "@rollup/rollup-linux-arm64-gnu": "4.17.2",
+                "@rollup/rollup-linux-arm64-musl": "4.17.2",
+                "@rollup/rollup-linux-powerpc64le-gnu": "4.17.2",
+                "@rollup/rollup-linux-riscv64-gnu": "4.17.2",
+                "@rollup/rollup-linux-s390x-gnu": "4.17.2",
+                "@rollup/rollup-linux-x64-gnu": "4.17.2",
+                "@rollup/rollup-linux-x64-musl": "4.17.2",
+                "@rollup/rollup-win32-arm64-msvc": "4.17.2",
+                "@rollup/rollup-win32-ia32-msvc": "4.17.2",
+                "@rollup/rollup-win32-x64-msvc": "4.17.2",
                 "fsevents": "~2.3.2"
             },
-            "resolved": "https://registry.npmjs.org/rollup/-/rollup-4.17.1.tgz",
-            "version": "4.17.1"
+            "resolved": "https://registry.npmjs.org/rollup/-/rollup-4.17.2.tgz",
+            "version": "4.17.2"
         },
         "node_modules/vitest": {
             "bin": {
                 "vitest": "vitest.mjs"
             },
             "dependencies": {
-                "@vitest/expect": "1.5.2",
-                "@vitest/runner": "1.5.2",
-                "@vitest/snapshot": "1.5.2",
-                "@vitest/spy": "1.5.2",
-                "@vitest/utils": "1.5.2",
+                "@vitest/expect": "1.5.3",
+                "@vitest/runner": "1.5.3",
+                "@vitest/snapshot": "1.5.3",
+                "@vitest/spy": "1.5.3",
+                "@vitest/utils": "1.5.3",
                 "acorn-walk": "^8.3.2",
                 "chai": "^4.3.10",
                 "debug": "^4.3.4",
                 "execa": "^8.0.1",
                 "local-pkg": "^0.5.0",
                 "magic-string": "^0.30.5",
                 "pathe": "^1.1.1",
                 "picocolors": "^1.0.0",
                 "std-env": "^3.5.0",
                 "strip-literal": "^2.0.0",
                 "tinybench": "^2.5.1",
                 "tinypool": "^0.8.3",
                 "vite": "^5.0.0",
-                "vite-node": "1.5.2",
+                "vite-node": "1.5.3",
                 "why-is-node-running": "^2.2.2"
             },
             "dev": true,
             "engines": {
                 "node": "^18.0.0 || >=20.0.0"
             },
             "funding": {
                 "url": "https://opencollective.com/vitest"
             },
-            "integrity": "sha512-l9gwIkq16ug3xY7BxHwcBQovLZG75zZL0PlsiYQbf76Rz6QGs54416UWMtC0jXeihvHvcHrf2ROEjkQRVpoZYw==",
+            "integrity": "sha512-2oM7nLXylw3mQlW6GXnRriw+7YvZFk/YNV8AxIC3Z3MfFbuziLGWP9GPxxu/7nRlXhqyxBikpamr+lEEj1sUEw==",
             "peerDependencies": {
                 "@edge-runtime/vm": "*",
                 "@types/node": "^18.0.0 || >=20.0.0",
-                "@vitest/browser": "1.5.2",
-                "@vitest/ui": "1.5.2",
+                "@vitest/browser": "1.5.3",
+                "@vitest/ui": "1.5.3",
                 "happy-dom": "*",
                 "jsdom": "*"
             },
             "peerDependenciesMeta": {
                 "@edge-runtime/vm": {
                     "optional": true
                 },
@@ -5583,16 +5584,16 @@
                 "happy-dom": {
                     "optional": true
                 },
                 "jsdom": {
                     "optional": true
                 }
             },
-            "resolved": "https://registry.npmjs.org/vitest/-/vitest-1.5.2.tgz",
-            "version": "1.5.2"
+            "resolved": "https://registry.npmjs.org/vitest/-/vitest-1.5.3.tgz",
+            "version": "1.5.3"
         },
         "node_modules/vitest/node_modules/local-pkg": {
             "dependencies": {
                 "mlly": "^1.4.2",
                 "pkg-types": "^1.0.3"
             },
             "dev": true,
```

### Comparing `swanlab-0.3.0/node_modules/@alloc/quick-lru/package.json` & `swanlab-0.3.1/node_modules/@alloc/quick-lru/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@antfu/utils/package.json` & `swanlab-0.3.1/node_modules/@antfu/utils/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@antv/adjust/package.json` & `swanlab-0.3.1/node_modules/@antv/adjust/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@antv/adjust/node_modules/tslib/package.json` & `swanlab-0.3.1/node_modules/@antv/adjust/node_modules/tslib/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@antv/attr/package.json` & `swanlab-0.3.1/node_modules/@antv/attr/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@antv/color-util/package.json` & `swanlab-0.3.1/node_modules/@antv/color-util/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@antv/component/package.json` & `swanlab-0.3.1/node_modules/@antv/component/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@antv/component/node_modules/@antv/path-util/package.json` & `swanlab-0.3.1/node_modules/@antv/component/node_modules/@antv/path-util/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@antv/component/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json` & `swanlab-0.3.1/node_modules/@antv/component/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@antv/coord/package.json` & `swanlab-0.3.1/node_modules/@antv/coord/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@antv/dom-util/package.json` & `swanlab-0.3.1/node_modules/@antv/dom-util/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@antv/event-emitter/package.json` & `swanlab-0.3.1/node_modules/@antv/event-emitter/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@antv/g-base/package.json` & `swanlab-0.3.1/node_modules/@antv/g-base/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@antv/g-base/node_modules/@antv/path-util/package.json` & `swanlab-0.3.1/node_modules/@antv/g-base/node_modules/@antv/path-util/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@antv/g-base/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json` & `swanlab-0.3.1/node_modules/@antv/g-base/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@antv/g-canvas/package.json` & `swanlab-0.3.1/node_modules/@antv/g-canvas/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@antv/g-canvas/node_modules/@antv/path-util/package.json` & `swanlab-0.3.1/node_modules/@antv/g-canvas/node_modules/@antv/path-util/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@antv/g-canvas/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json` & `swanlab-0.3.1/node_modules/@antv/g-canvas/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@antv/g-math/package.json` & `swanlab-0.3.1/node_modules/@antv/g-math/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@antv/g-svg/package.json` & `swanlab-0.3.1/node_modules/@antv/g-svg/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@antv/g2/package.json` & `swanlab-0.3.1/node_modules/@antv/g2/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@antv/g2/node_modules/@antv/path-util/package.json` & `swanlab-0.3.1/node_modules/@antv/g2/node_modules/@antv/path-util/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@antv/g2/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json` & `swanlab-0.3.1/node_modules/@antv/g2/node_modules/@antv/path-util/node_modules/@antv/matrix-util/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@antv/g2plot/package.json` & `swanlab-0.3.1/node_modules/@antv/g2plot/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@antv/matrix-util/package.json` & `swanlab-0.3.1/node_modules/@antv/matrix-util/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@antv/path-util/package.json` & `swanlab-0.3.1/node_modules/@antv/path-util/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@antv/scale/package.json` & `swanlab-0.3.1/node_modules/@antv/scale/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@antv/util/package.json` & `swanlab-0.3.1/node_modules/@antv/util/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@babel/parser/package.json` & `swanlab-0.3.1/node_modules/@babel/parser/package.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9681372549019609%*

 * *Differences: {"'devDependencies'": "{'@babel/helper-validator-identifier': '^7.24.5'}", "'version'": "'7.24.5'"}*

```diff
@@ -4,15 +4,15 @@
     "bugs": "https://github.com/babel/babel/issues?utf8=%E2%9C%93&q=is%3Aissue+label%3A%22pkg%3A+parser+%28babylon%29%22+is%3Aopen",
     "description": "A JavaScript parser",
     "devDependencies": {
         "@babel/code-frame": "^7.24.2",
         "@babel/helper-check-duplicate-nodes": "^7.22.5",
         "@babel/helper-fixtures": "^7.24.4",
         "@babel/helper-string-parser": "^7.24.1",
-        "@babel/helper-validator-identifier": "^7.22.20",
+        "@babel/helper-validator-identifier": "^7.24.5",
         "charcodes": "^0.2.0"
     },
     "engines": {
         "node": ">=6.0.0"
     },
     "files": [
         "bin",
@@ -38,9 +38,9 @@
     "repository": {
         "directory": "packages/babel-parser",
         "type": "git",
         "url": "https://github.com/babel/babel.git"
     },
     "type": "commonjs",
     "types": "./typings/babel-parser.d.ts",
-    "version": "7.24.4"
+    "version": "7.24.5"
 }
```

### Comparing `swanlab-0.3.0/node_modules/@eslint/eslintrc/package.json` & `swanlab-0.3.1/node_modules/@eslint/eslintrc/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@eslint/js/package.json` & `swanlab-0.3.1/node_modules/@eslint/js/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@eslint-community/eslint-utils/package.json` & `swanlab-0.3.1/node_modules/@eslint-community/eslint-utils/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@eslint-community/regexpp/package.json` & `swanlab-0.3.1/node_modules/@eslint-community/regexpp/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@headlessui/vue/package.json` & `swanlab-0.3.1/node_modules/@headlessui/vue/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@humanwhocodes/config-array/package.json` & `swanlab-0.3.1/node_modules/@humanwhocodes/config-array/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@humanwhocodes/module-importer/package.json` & `swanlab-0.3.1/node_modules/@humanwhocodes/module-importer/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@humanwhocodes/object-schema/package.json` & `swanlab-0.3.1/node_modules/@humanwhocodes/object-schema/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@intlify/core-base/package.json` & `swanlab-0.3.1/node_modules/@intlify/core-base/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@intlify/message-compiler/package.json` & `swanlab-0.3.1/node_modules/@intlify/message-compiler/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@intlify/shared/package.json` & `swanlab-0.3.1/node_modules/@intlify/shared/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@isaacs/cliui/package.json` & `swanlab-0.3.1/node_modules/@isaacs/cliui/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@isaacs/cliui/node_modules/ansi-regex/package.json` & `swanlab-0.3.1/node_modules/@isaacs/cliui/node_modules/ansi-regex/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@isaacs/cliui/node_modules/strip-ansi/package.json` & `swanlab-0.3.1/node_modules/@isaacs/cliui/node_modules/strip-ansi/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@jest/schemas/package.json` & `swanlab-0.3.1/node_modules/@jest/schemas/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@jridgewell/gen-mapping/package.json` & `swanlab-0.3.1/node_modules/@jridgewell/gen-mapping/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@jridgewell/resolve-uri/package.json` & `swanlab-0.3.1/node_modules/@jridgewell/resolve-uri/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@jridgewell/set-array/package.json` & `swanlab-0.3.1/node_modules/@jridgewell/set-array/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@jridgewell/source-map/package.json` & `swanlab-0.3.1/node_modules/@jridgewell/source-map/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@jridgewell/sourcemap-codec/package.json` & `swanlab-0.3.1/node_modules/@jridgewell/sourcemap-codec/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@jridgewell/trace-mapping/package.json` & `swanlab-0.3.1/node_modules/@jridgewell/trace-mapping/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@ljharb/resumer/package.json` & `swanlab-0.3.1/node_modules/@ljharb/resumer/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@ljharb/through/package.json` & `swanlab-0.3.1/node_modules/@ljharb/through/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@nodelib/fs.scandir/package.json` & `swanlab-0.3.1/node_modules/@nodelib/fs.scandir/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@nodelib/fs.stat/package.json` & `swanlab-0.3.1/node_modules/@nodelib/fs.stat/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@nodelib/fs.walk/package.json` & `swanlab-0.3.1/node_modules/@nodelib/fs.walk/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@pkgjs/parseargs/package.json` & `swanlab-0.3.1/node_modules/@pkgjs/parseargs/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@popperjs/core/package.json` & `swanlab-0.3.1/node_modules/@popperjs/core/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@rollup/pluginutils/package.json` & `swanlab-0.3.1/node_modules/@rollup/pluginutils/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@sinclair/typebox/package.json` & `swanlab-0.3.1/node_modules/@sinclair/typebox/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@tanstack/virtual-core/package.json` & `swanlab-0.3.1/node_modules/@tanstack/virtual-core/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@tanstack/vue-virtual/package.json` & `swanlab-0.3.1/node_modules/@tanstack/vue-virtual/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@types/d3-timer/package.json` & `swanlab-0.3.1/node_modules/@types/d3-timer/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@types/estree/package.json` & `swanlab-0.3.1/node_modules/@types/estree/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@ungap/structured-clone/package.json` & `swanlab-0.3.1/node_modules/@ungap/structured-clone/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@vitejs/plugin-vue/package.json` & `swanlab-0.3.1/node_modules/@vitejs/plugin-vue/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@vitest/expect/package.json` & `swanlab-0.3.1/node_modules/@vitest/expect/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9594907407407409%*

 * *Differences: {"'dependencies'": "{'@vitest/spy': '1.5.3', '@vitest/utils': '1.5.3'}",*

 * * "'devDependencies'": "{'@vitest/runner': '1.5.3'}",*

 * * "'version'": "'1.5.3'"}*

```diff
@@ -1,20 +1,20 @@
 {
     "bugs": {
         "url": "https://github.com/vitest-dev/vitest/issues"
     },
     "dependencies": {
-        "@vitest/spy": "1.5.2",
-        "@vitest/utils": "1.5.2",
+        "@vitest/spy": "1.5.3",
+        "@vitest/utils": "1.5.3",
         "chai": "^4.3.10"
     },
     "description": "Jest's expect matchers as a Chai plugin",
     "devDependencies": {
         "@types/chai": "4.3.6",
-        "@vitest/runner": "1.5.2",
+        "@vitest/runner": "1.5.3",
         "picocolors": "^1.0.0",
         "rollup-plugin-copy": "^3.5.0"
     },
     "exports": {
         ".": {
             "default": "./dist/index.js",
             "types": "./index.d.ts"
@@ -39,9 +39,9 @@
     "scripts": {
         "build": "rimraf dist && rollup -c",
         "dev": "rollup -c --watch"
     },
     "sideEffects": false,
     "type": "module",
     "types": "./index.d.ts",
-    "version": "1.5.2"
+    "version": "1.5.3"
 }
```

### Comparing `swanlab-0.3.0/node_modules/@vitest/runner/package.json` & `swanlab-0.3.1/node_modules/@vitest/runner/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9656862745098038%*

 * *Differences: {"'dependencies'": "{'@vitest/utils': '1.5.3'}", "'version'": "'1.5.3'"}*

```diff
@@ -1,13 +1,13 @@
 {
     "bugs": {
         "url": "https://github.com/vitest-dev/vitest/issues"
     },
     "dependencies": {
-        "@vitest/utils": "1.5.2",
+        "@vitest/utils": "1.5.3",
         "p-limit": "^5.0.0",
         "pathe": "^1.1.1"
     },
     "description": "Vitest test runner",
     "exports": {
         ".": {
             "default": "./dist/index.js",
@@ -41,9 +41,9 @@
     "scripts": {
         "build": "rimraf dist && rollup -c",
         "dev": "rollup -c --watch"
     },
     "sideEffects": true,
     "type": "module",
     "types": "./dist/index.d.ts",
-    "version": "1.5.2"
+    "version": "1.5.3"
 }
```

### Comparing `swanlab-0.3.0/node_modules/@vitest/runner/node_modules/p-limit/package.json` & `swanlab-0.3.1/node_modules/@vitest/runner/node_modules/p-limit/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@vitest/runner/node_modules/yocto-queue/package.json` & `swanlab-0.3.1/node_modules/@vitest/runner/node_modules/yocto-queue/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@vitest/snapshot/package.json` & `swanlab-0.3.1/node_modules/@vitest/snapshot/package.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9675925925925927%*

 * *Differences: {"'devDependencies'": "{'@vitest/utils': '1.5.3'}", "'version'": "'1.5.3'"}*

```diff
@@ -6,15 +6,15 @@
         "magic-string": "^0.30.5",
         "pathe": "^1.1.1",
         "pretty-format": "^29.7.0"
     },
     "description": "Vitest snapshot manager",
     "devDependencies": {
         "@types/natural-compare": "^1.4.3",
-        "@vitest/utils": "1.5.2",
+        "@vitest/utils": "1.5.3",
         "natural-compare": "^1.4.0"
     },
     "exports": {
         ".": {
             "default": "./dist/index.js",
             "types": "./dist/index.d.ts"
         },
@@ -46,9 +46,9 @@
     "scripts": {
         "build": "rimraf dist && rollup -c",
         "dev": "rollup -c --watch"
     },
     "sideEffects": false,
     "type": "module",
     "types": "./dist/index.d.ts",
-    "version": "1.5.2"
+    "version": "1.5.3"
 }
```

### Comparing `swanlab-0.3.0/node_modules/@vitest/spy/package.json` & `swanlab-0.3.1/node_modules/@vitest/spy/package.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9705882352941176%*

 * *Differences: {"'version'": "'1.5.3'"}*

```diff
@@ -30,9 +30,9 @@
     "scripts": {
         "build": "rimraf dist && rollup -c",
         "dev": "rollup -c --watch"
     },
     "sideEffects": false,
     "type": "module",
     "types": "./dist/index.d.ts",
-    "version": "1.5.2"
+    "version": "1.5.3"
 }
```

### Comparing `swanlab-0.3.0/node_modules/@vitest/utils/package.json` & `swanlab-0.3.1/node_modules/@vitest/utils/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9736842105263158%*

 * *Differences: {"'version'": "'1.5.3'"}*

```diff
@@ -66,9 +66,9 @@
     "typesVersions": {
         "*": {
             "source-map": [
                 "dist/source-map.d.ts"
             ]
         }
     },
-    "version": "1.5.2"
+    "version": "1.5.3"
 }
```

### Comparing `swanlab-0.3.0/node_modules/@vitest/utils/node_modules/estree-walker/package.json` & `swanlab-0.3.1/node_modules/@vitest/utils/node_modules/estree-walker/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@vue/compiler-core/package.json` & `swanlab-0.3.1/node_modules/@vue/compiler-core/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@vue/compiler-dom/package.json` & `swanlab-0.3.1/node_modules/@vue/compiler-dom/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@vue/compiler-sfc/package.json` & `swanlab-0.3.1/node_modules/@vue/compiler-sfc/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@vue/compiler-ssr/package.json` & `swanlab-0.3.1/node_modules/@vue/compiler-ssr/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@vue/devtools-api/package.json` & `swanlab-0.3.1/node_modules/@vue/devtools-api/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@vue/reactivity/package.json` & `swanlab-0.3.1/node_modules/@vue/reactivity/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@vue/runtime-core/package.json` & `swanlab-0.3.1/node_modules/@vue/runtime-core/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@vue/runtime-dom/package.json` & `swanlab-0.3.1/node_modules/@vue/runtime-dom/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@vue/server-renderer/package.json` & `swanlab-0.3.1/node_modules/@vue/server-renderer/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/@vue/shared/package.json` & `swanlab-0.3.1/node_modules/@vue/shared/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/acorn/package.json` & `swanlab-0.3.1/node_modules/acorn/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/acorn-jsx/package.json` & `swanlab-0.3.1/node_modules/acorn-jsx/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/acorn-walk/package.json` & `swanlab-0.3.1/node_modules/acorn-walk/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/ajv/package.json` & `swanlab-0.3.1/node_modules/ajv/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/ajv/lib/refs/data.json` & `swanlab-0.3.1/node_modules/ajv/lib/refs/data.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/ajv/lib/refs/json-schema-draft-04.json` & `swanlab-0.3.1/node_modules/ajv/lib/refs/json-schema-draft-04.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/ajv/lib/refs/json-schema-draft-06.json` & `swanlab-0.3.1/node_modules/ajv/lib/refs/json-schema-draft-06.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/ajv/lib/refs/json-schema-draft-07.json` & `swanlab-0.3.1/node_modules/ajv/lib/refs/json-schema-draft-07.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/ajv/lib/refs/json-schema-secure.json` & `swanlab-0.3.1/node_modules/ajv/lib/refs/json-schema-secure.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/align-text/package.json` & `swanlab-0.3.1/node_modules/align-text/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/ansi-regex/package.json` & `swanlab-0.3.1/node_modules/ansi-regex/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/ansi-styles/package.json` & `swanlab-0.3.1/node_modules/ansi-styles/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/any-promise/package.json` & `swanlab-0.3.1/node_modules/any-promise/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/anymatch/package.json` & `swanlab-0.3.1/node_modules/anymatch/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/arg/package.json` & `swanlab-0.3.1/node_modules/arg/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/argparse/package.json` & `swanlab-0.3.1/node_modules/argparse/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/array-buffer-byte-length/package.json` & `swanlab-0.3.1/node_modules/array-buffer-byte-length/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/array-buffer-byte-length/tsconfig.json` & `swanlab-0.3.1/node_modules/array-buffer-byte-length/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/arraybuffer.prototype.slice/package.json` & `swanlab-0.3.1/node_modules/arraybuffer.prototype.slice/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/assertion-error/package.json` & `swanlab-0.3.1/node_modules/assertion-error/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/asynckit/package.json` & `swanlab-0.3.1/node_modules/asynckit/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/autoprefixer/package.json` & `swanlab-0.3.1/node_modules/autoprefixer/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/available-typed-arrays/package.json` & `swanlab-0.3.1/node_modules/available-typed-arrays/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/available-typed-arrays/tsconfig.json` & `swanlab-0.3.1/node_modules/available-typed-arrays/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/axios/package.json` & `swanlab-0.3.1/node_modules/axios/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/balanced-match/package.json` & `swanlab-0.3.1/node_modules/balanced-match/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/binary-extensions/binary-extensions.json` & `swanlab-0.3.1/node_modules/binary-extensions/binary-extensions.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/binary-extensions/package.json` & `swanlab-0.3.1/node_modules/binary-extensions/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/boolbase/package.json` & `swanlab-0.3.1/node_modules/boolbase/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/brace-expansion/package.json` & `swanlab-0.3.1/node_modules/brace-expansion/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/braces/package.json` & `swanlab-0.3.1/node_modules/braces/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/browserslist/package.json` & `swanlab-0.3.1/node_modules/browserslist/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/cac/package.json` & `swanlab-0.3.1/node_modules/cac/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/call-bind/package.json` & `swanlab-0.3.1/node_modules/call-bind/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/callsites/package.json` & `swanlab-0.3.1/node_modules/callsites/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/camelcase/package.json` & `swanlab-0.3.1/node_modules/camelcase/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/camelcase-css/package.json` & `swanlab-0.3.1/node_modules/camelcase-css/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/caniuse-lite/package.json` & `swanlab-0.3.1/node_modules/caniuse-lite/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/center-align/package.json` & `swanlab-0.3.1/node_modules/center-align/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/chai/package.json` & `swanlab-0.3.1/node_modules/chai/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/chalk/package.json` & `swanlab-0.3.1/node_modules/chalk/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/check-error/package.json` & `swanlab-0.3.1/node_modules/check-error/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/chokidar/package.json` & `swanlab-0.3.1/node_modules/chokidar/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/chokidar/node_modules/glob-parent/package.json` & `swanlab-0.3.1/node_modules/chokidar/node_modules/glob-parent/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/cliui/package.json` & `swanlab-0.3.1/node_modules/cliui/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/color-convert/package.json` & `swanlab-0.3.1/node_modules/color-convert/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/color-name/package.json` & `swanlab-0.3.1/node_modules/color-name/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/combined-stream/package.json` & `swanlab-0.3.1/node_modules/combined-stream/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/commander/package.json` & `swanlab-0.3.1/node_modules/commander/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/concat-map/package.json` & `swanlab-0.3.1/node_modules/concat-map/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/confbox/package.json` & `swanlab-0.3.1/node_modules/confbox/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/contour_plot/package.json` & `swanlab-0.3.1/node_modules/contour_plot/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/cross-spawn/package.json` & `swanlab-0.3.1/node_modules/cross-spawn/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/cssesc/package.json` & `swanlab-0.3.1/node_modules/cssesc/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/csstype/package.json` & `swanlab-0.3.1/node_modules/csstype/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/d3-color/package.json` & `swanlab-0.3.1/node_modules/d3-color/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/d3-ease/package.json` & `swanlab-0.3.1/node_modules/d3-ease/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/d3-hierarchy/package.json` & `swanlab-0.3.1/node_modules/d3-hierarchy/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/d3-interpolate/package.json` & `swanlab-0.3.1/node_modules/d3-interpolate/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/d3-regression/package.json` & `swanlab-0.3.1/node_modules/d3-regression/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/d3-timer/package.json` & `swanlab-0.3.1/node_modules/d3-timer/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/data-view-buffer/package.json` & `swanlab-0.3.1/node_modules/data-view-buffer/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/data-view-buffer/tsconfig.json` & `swanlab-0.3.1/node_modules/data-view-buffer/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/data-view-byte-length/package.json` & `swanlab-0.3.1/node_modules/data-view-byte-length/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/data-view-byte-offset/package.json` & `swanlab-0.3.1/node_modules/data-view-byte-offset/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/data-view-byte-offset/tsconfig.json` & `swanlab-0.3.1/node_modules/data-view-byte-offset/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/debug/package.json` & `swanlab-0.3.1/node_modules/debug/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/decamelize/package.json` & `swanlab-0.3.1/node_modules/decamelize/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/deep-eql/package.json` & `swanlab-0.3.1/node_modules/deep-eql/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/deep-equal/package.json` & `swanlab-0.3.1/node_modules/deep-equal/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/deep-is/package.json` & `swanlab-0.3.1/node_modules/deep-is/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/define-data-property/package.json` & `swanlab-0.3.1/node_modules/define-data-property/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/define-data-property/tsconfig.json` & `swanlab-0.3.1/node_modules/define-data-property/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/define-properties/package.json` & `swanlab-0.3.1/node_modules/define-properties/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/defined/package.json` & `swanlab-0.3.1/node_modules/defined/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/delayed-stream/package.json` & `swanlab-0.3.1/node_modules/delayed-stream/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/detect-browser/package.json` & `swanlab-0.3.1/node_modules/detect-browser/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/didyoumean/package.json` & `swanlab-0.3.1/node_modules/didyoumean/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/diff-sequences/package.json` & `swanlab-0.3.1/node_modules/diff-sequences/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/dlv/package.json` & `swanlab-0.3.1/node_modules/dlv/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/doctrine/package.json` & `swanlab-0.3.1/node_modules/doctrine/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/dotignore/package.json` & `swanlab-0.3.1/node_modules/dotignore/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/electron-to-chromium/chromium-versions.json` & `swanlab-0.3.1/node_modules/electron-to-chromium/chromium-versions.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/electron-to-chromium/full-chromium-versions.json` & `swanlab-0.3.1/node_modules/electron-to-chromium/full-chromium-versions.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9974012474012475%*

 * *Differences: {"'124.0.6367.91'": "['30.0.2']",*

 * * "'125.0.6412.0'": "{insert: [(2, '31.0.0-alpha.3'), (10, '32.0.0-nightly.20240429'), (11, "*

 * *                   "'32.0.0-nightly.20240430'), (12, '32.0.0-nightly.20240501')]}"}*

```diff
@@ -1364,24 +1364,31 @@
         "30.0.1"
     ],
     "124.0.6367.9": [
         "30.0.0-beta.3",
         "30.0.0-beta.4",
         "30.0.0-beta.5"
     ],
+    "124.0.6367.91": [
+        "30.0.2"
+    ],
     "125.0.6412.0": [
         "31.0.0-alpha.1",
         "31.0.0-alpha.2",
+        "31.0.0-alpha.3",
         "32.0.0-nightly.20240418",
         "32.0.0-nightly.20240419",
         "32.0.0-nightly.20240422",
         "32.0.0-nightly.20240423",
         "32.0.0-nightly.20240424",
         "32.0.0-nightly.20240425",
-        "32.0.0-nightly.20240426"
+        "32.0.0-nightly.20240426",
+        "32.0.0-nightly.20240429",
+        "32.0.0-nightly.20240430",
+        "32.0.0-nightly.20240501"
     ],
     "39.0.2171.65": [
         "0.20.0",
         "0.20.1",
         "0.20.2",
         "0.20.3",
         "0.20.4",
```

### Comparing `swanlab-0.3.0/node_modules/electron-to-chromium/full-versions.json` & `swanlab-0.3.1/node_modules/electron-to-chromium/full-versions.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9978768577494692%*

 * *Differences: {"'30.0.2'": "'124.0.6367.91'",*

 * * "'31.0.0-alpha.3'": "'125.0.6412.0'",*

 * * "'32.0.0-nightly.20240429'": "'125.0.6412.0'",*

 * * "'32.0.0-nightly.20240430'": "'125.0.6412.0'",*

 * * "'32.0.0-nightly.20240501'": "'125.0.6412.0'"}*

```diff
@@ -1938,16 +1938,18 @@
     "30.0.0-nightly.20240214": "123.0.6272.0",
     "30.0.0-nightly.20240215": "123.0.6296.0",
     "30.0.0-nightly.20240216": "123.0.6296.0",
     "30.0.0-nightly.20240219": "123.0.6296.0",
     "30.0.0-nightly.20240220": "123.0.6296.0",
     "30.0.0-nightly.20240221": "123.0.6296.0",
     "30.0.1": "124.0.6367.60",
+    "30.0.2": "124.0.6367.91",
     "31.0.0-alpha.1": "125.0.6412.0",
     "31.0.0-alpha.2": "125.0.6412.0",
+    "31.0.0-alpha.3": "125.0.6412.0",
     "31.0.0-nightly.20240222": "123.0.6312.5",
     "31.0.0-nightly.20240223": "123.0.6312.5",
     "31.0.0-nightly.20240226": "123.0.6312.5",
     "31.0.0-nightly.20240227": "123.0.6312.5",
     "31.0.0-nightly.20240228": "123.0.6312.5",
     "31.0.0-nightly.20240229": "124.0.6323.0",
     "31.0.0-nightly.20240301": "124.0.6323.0",
@@ -1981,14 +1983,17 @@
     "32.0.0-nightly.20240418": "125.0.6412.0",
     "32.0.0-nightly.20240419": "125.0.6412.0",
     "32.0.0-nightly.20240422": "125.0.6412.0",
     "32.0.0-nightly.20240423": "125.0.6412.0",
     "32.0.0-nightly.20240424": "125.0.6412.0",
     "32.0.0-nightly.20240425": "125.0.6412.0",
     "32.0.0-nightly.20240426": "125.0.6412.0",
+    "32.0.0-nightly.20240429": "125.0.6412.0",
+    "32.0.0-nightly.20240430": "125.0.6412.0",
+    "32.0.0-nightly.20240501": "125.0.6412.0",
     "4.0.0": "69.0.3497.106",
     "4.0.0-beta.1": "69.0.3497.106",
     "4.0.0-beta.10": "69.0.3497.106",
     "4.0.0-beta.11": "69.0.3497.106",
     "4.0.0-beta.2": "69.0.3497.106",
     "4.0.0-beta.3": "69.0.3497.106",
     "4.0.0-beta.4": "69.0.3497.106",
```

### Comparing `swanlab-0.3.0/node_modules/electron-to-chromium/package.json` & `swanlab-0.3.1/node_modules/electron-to-chromium/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9545454545454546%*

 * *Differences: {"'version'": "'1.4.754'"}*

```diff
@@ -36,9 +36,9 @@
     },
     "scripts": {
         "build": "node build.mjs",
         "report": "nyc report --reporter=text-lcov > coverage.lcov && codecov",
         "test": "nyc ava --verbose",
         "update": "node automated-update.js"
     },
-    "version": "1.4.750"
+    "version": "1.4.754"
 }
```

### Comparing `swanlab-0.3.0/node_modules/electron-to-chromium/versions.json` & `swanlab-0.3.1/node_modules/electron-to-chromium/versions.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/emoji-regex/package.json` & `swanlab-0.3.1/node_modules/emoji-regex/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/entities/package.json` & `swanlab-0.3.1/node_modules/entities/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/es-abstract/package.json` & `swanlab-0.3.1/node_modules/es-abstract/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/es-abstract/helpers/caseFolding.json` & `swanlab-0.3.1/node_modules/es-abstract/helpers/caseFolding.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/es-abstract/node_modules/object-inspect/package.json` & `swanlab-0.3.1/node_modules/es-abstract/node_modules/object-inspect/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/es-define-property/package.json` & `swanlab-0.3.1/node_modules/es-define-property/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/es-define-property/tsconfig.json` & `swanlab-0.3.1/node_modules/es-define-property/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/es-errors/package.json` & `swanlab-0.3.1/node_modules/es-errors/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/es-errors/tsconfig.json` & `swanlab-0.3.1/node_modules/es-errors/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/es-object-atoms/package.json` & `swanlab-0.3.1/node_modules/es-object-atoms/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/es-set-tostringtag/package.json` & `swanlab-0.3.1/node_modules/es-set-tostringtag/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/es-set-tostringtag/tsconfig.json` & `swanlab-0.3.1/node_modules/es-set-tostringtag/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/es-to-primitive/package.json` & `swanlab-0.3.1/node_modules/es-to-primitive/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/esbuild/package.json` & `swanlab-0.3.1/node_modules/esbuild/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/escalade/package.json` & `swanlab-0.3.1/node_modules/escalade/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/escape-string-regexp/package.json` & `swanlab-0.3.1/node_modules/escape-string-regexp/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/eslint/package.json` & `swanlab-0.3.1/node_modules/eslint/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/eslint/conf/replacements.json` & `swanlab-0.3.1/node_modules/eslint/conf/replacements.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/eslint/conf/rule-type-list.json` & `swanlab-0.3.1/node_modules/eslint/conf/rule-type-list.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/eslint/lib/cli-engine/formatters/formatters-meta.json` & `swanlab-0.3.1/node_modules/eslint/lib/cli-engine/formatters/formatters-meta.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/eslint-plugin-prettier/package.json` & `swanlab-0.3.1/node_modules/eslint-plugin-prettier/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/eslint-plugin-vue/package.json` & `swanlab-0.3.1/node_modules/eslint-plugin-vue/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/eslint-plugin-vue/lib/utils/html-elements.json` & `swanlab-0.3.1/node_modules/eslint-plugin-vue/lib/utils/html-elements.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/eslint-plugin-vue/lib/utils/js-reserved.json` & `swanlab-0.3.1/node_modules/eslint-plugin-vue/lib/utils/js-reserved.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/eslint-plugin-vue/lib/utils/key-aliases.json` & `swanlab-0.3.1/node_modules/eslint-plugin-vue/lib/utils/key-aliases.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/eslint-plugin-vue/lib/utils/svg-attributes-weird-case.json` & `swanlab-0.3.1/node_modules/eslint-plugin-vue/lib/utils/svg-attributes-weird-case.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/eslint-plugin-vue/lib/utils/svg-elements.json` & `swanlab-0.3.1/node_modules/eslint-plugin-vue/lib/utils/svg-elements.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/eslint-plugin-vue/lib/utils/vue-component-options.json` & `swanlab-0.3.1/node_modules/eslint-plugin-vue/lib/utils/vue-component-options.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/eslint-plugin-vue/lib/utils/vue3-export-names.json` & `swanlab-0.3.1/node_modules/eslint-plugin-vue/lib/utils/vue3-export-names.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/eslint-scope/package.json` & `swanlab-0.3.1/node_modules/eslint-scope/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/eslint-visitor-keys/package.json` & `swanlab-0.3.1/node_modules/eslint-visitor-keys/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/espree/package.json` & `swanlab-0.3.1/node_modules/espree/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/esquery/package.json` & `swanlab-0.3.1/node_modules/esquery/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/esrecurse/package.json` & `swanlab-0.3.1/node_modules/esrecurse/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/estraverse/package.json` & `swanlab-0.3.1/node_modules/estraverse/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/estree-walker/package.json` & `swanlab-0.3.1/node_modules/estree-walker/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/esutils/package.json` & `swanlab-0.3.1/node_modules/esutils/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/execa/package.json` & `swanlab-0.3.1/node_modules/execa/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/fast-deep-equal/package.json` & `swanlab-0.3.1/node_modules/fast-deep-equal/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/fast-diff/package.json` & `swanlab-0.3.1/node_modules/fast-diff/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/fast-glob/package.json` & `swanlab-0.3.1/node_modules/fast-glob/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/fast-glob/node_modules/glob-parent/package.json` & `swanlab-0.3.1/node_modules/fast-glob/node_modules/glob-parent/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/fast-json-stable-stringify/package.json` & `swanlab-0.3.1/node_modules/fast-json-stable-stringify/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/fast-json-stable-stringify/benchmark/test.json` & `swanlab-0.3.1/node_modules/fast-json-stable-stringify/benchmark/test.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/fast-levenshtein/package.json` & `swanlab-0.3.1/node_modules/fast-levenshtein/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/fastq/package.json` & `swanlab-0.3.1/node_modules/fastq/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/fecha/package.json` & `swanlab-0.3.1/node_modules/fecha/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/file-entry-cache/package.json` & `swanlab-0.3.1/node_modules/file-entry-cache/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/fill-range/package.json` & `swanlab-0.3.1/node_modules/fill-range/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/find-up/package.json` & `swanlab-0.3.1/node_modules/find-up/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/flat-cache/package.json` & `swanlab-0.3.1/node_modules/flat-cache/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/flatted/package.json` & `swanlab-0.3.1/node_modules/flatted/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/fmin/package.json` & `swanlab-0.3.1/node_modules/fmin/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/follow-redirects/package.json` & `swanlab-0.3.1/node_modules/follow-redirects/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/for-each/package.json` & `swanlab-0.3.1/node_modules/for-each/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/foreground-child/package.json` & `swanlab-0.3.1/node_modules/foreground-child/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/form-data/package.json` & `swanlab-0.3.1/node_modules/form-data/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/fraction.js/package.json` & `swanlab-0.3.1/node_modules/fraction.js/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/fs.realpath/package.json` & `swanlab-0.3.1/node_modules/fs.realpath/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/function-bind/package.json` & `swanlab-0.3.1/node_modules/function-bind/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/function.prototype.name/package.json` & `swanlab-0.3.1/node_modules/function.prototype.name/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/functions-have-names/package.json` & `swanlab-0.3.1/node_modules/functions-have-names/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/get-func-name/package.json` & `swanlab-0.3.1/node_modules/get-func-name/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/get-intrinsic/package.json` & `swanlab-0.3.1/node_modules/get-intrinsic/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/get-stream/package.json` & `swanlab-0.3.1/node_modules/get-stream/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/get-symbol-description/package.json` & `swanlab-0.3.1/node_modules/get-symbol-description/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/gl-matrix/package.json` & `swanlab-0.3.1/node_modules/gl-matrix/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/glob/package.json` & `swanlab-0.3.1/node_modules/glob/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/glob-parent/package.json` & `swanlab-0.3.1/node_modules/glob-parent/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/globals/globals.json` & `swanlab-0.3.1/node_modules/globals/globals.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/globals/package.json` & `swanlab-0.3.1/node_modules/globals/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/globalthis/package.json` & `swanlab-0.3.1/node_modules/globalthis/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9417420814479639%*

 * *Differences: {"'dependencies'": "{'define-properties': '^1.2.1', 'gopd': '^1.0.1'}",*

 * * "'devDependencies'": "{'@es-shims/api': '^2.5.0', '@ljharb/eslint-config': '^21.1.0', 'aud': "*

 * *                      "'^2.0.4', 'tape': '^5.7.5', 'npmignore': '^0.3.1'}",*

 * * "'version'": "'1.0.4'"}*

```diff
@@ -8,30 +8,32 @@
         "template": "keepachangelog",
         "unreleased": false
     },
     "browser": {
         "./implementation": "./implementation.browser.js"
     },
     "dependencies": {
-        "define-properties": "^1.1.3"
+        "define-properties": "^1.2.1",
+        "gopd": "^1.0.1"
     },
     "description": "ECMAScript spec-compliant polyfill/shim for `globalThis`",
     "devDependencies": {
-        "@es-shims/api": "^2.2.3",
-        "@ljharb/eslint-config": "^21.0.0",
-        "aud": "^2.0.0",
+        "@es-shims/api": "^2.5.0",
+        "@ljharb/eslint-config": "^21.1.0",
+        "aud": "^2.0.4",
         "auto-changelog": "^2.4.0",
         "browserify": "^16.5.2",
         "eslint": "=8.8.0",
         "for-each": "^0.3.3",
         "in-publish": "^2.0.1",
         "is": "^3.3.0",
+        "npmignore": "^0.3.1",
         "nyc": "^10.3.2",
         "safe-publish-latest": "^2.0.0",
-        "tape": "^5.5.3"
+        "tape": "^5.7.5"
     },
     "engines": {
         "node": ">= 0.4"
     },
     "funding": {
         "url": "https://github.com/sponsors/ljharb"
     },
@@ -89,9 +91,9 @@
             "safari/4.0..latest",
             "ipad/6.0..latest",
             "iphone/6.0..latest",
             "android-browser/4.2"
         ],
         "files": "test/index.js"
     },
-    "version": "1.0.3"
+    "version": "1.0.4"
 }
```

### Comparing `swanlab-0.3.0/node_modules/gopd/package.json` & `swanlab-0.3.1/node_modules/gopd/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/graphemer/package.json` & `swanlab-0.3.1/node_modules/graphemer/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/has/package.json` & `swanlab-0.3.1/node_modules/has/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/has-ansi/package.json` & `swanlab-0.3.1/node_modules/has-ansi/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/has-ansi/node_modules/ansi-regex/package.json` & `swanlab-0.3.1/node_modules/has-ansi/node_modules/ansi-regex/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/has-bigints/package.json` & `swanlab-0.3.1/node_modules/has-bigints/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/has-flag/package.json` & `swanlab-0.3.1/node_modules/has-flag/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/has-property-descriptors/package.json` & `swanlab-0.3.1/node_modules/has-property-descriptors/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/has-proto/package.json` & `swanlab-0.3.1/node_modules/has-proto/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/has-proto/tsconfig.json` & `swanlab-0.3.1/node_modules/has-proto/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/has-symbols/package.json` & `swanlab-0.3.1/node_modules/has-symbols/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/has-tostringtag/package.json` & `swanlab-0.3.1/node_modules/has-tostringtag/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/has-tostringtag/tsconfig.json` & `swanlab-0.3.1/node_modules/has-tostringtag/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/hasown/package.json` & `swanlab-0.3.1/node_modules/hasown/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/human-signals/package.json` & `swanlab-0.3.1/node_modules/human-signals/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/husky/package.json` & `swanlab-0.3.1/node_modules/husky/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/ignore/package.json` & `swanlab-0.3.1/node_modules/ignore/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/immutable/package.json` & `swanlab-0.3.1/node_modules/immutable/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/import-fresh/package.json` & `swanlab-0.3.1/node_modules/import-fresh/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/imurmurhash/package.json` & `swanlab-0.3.1/node_modules/imurmurhash/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/inflight/package.json` & `swanlab-0.3.1/node_modules/inflight/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/inherits/package.json` & `swanlab-0.3.1/node_modules/inherits/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/internal-slot/package.json` & `swanlab-0.3.1/node_modules/internal-slot/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/is-arguments/package.json` & `swanlab-0.3.1/node_modules/is-arguments/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/is-array-buffer/package.json` & `swanlab-0.3.1/node_modules/is-array-buffer/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/is-array-buffer/tsconfig.json` & `swanlab-0.3.1/node_modules/is-array-buffer/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/is-bigint/package.json` & `swanlab-0.3.1/node_modules/is-bigint/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/is-binary-path/package.json` & `swanlab-0.3.1/node_modules/is-binary-path/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/is-boolean-object/package.json` & `swanlab-0.3.1/node_modules/is-boolean-object/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/is-buffer/package.json` & `swanlab-0.3.1/node_modules/is-buffer/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/is-callable/package.json` & `swanlab-0.3.1/node_modules/is-callable/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/is-core-module/core.json` & `swanlab-0.3.1/node_modules/is-core-module/core.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/is-core-module/package.json` & `swanlab-0.3.1/node_modules/is-core-module/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/is-data-view/package.json` & `swanlab-0.3.1/node_modules/is-data-view/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/is-data-view/tsconfig.json` & `swanlab-0.3.1/node_modules/is-data-view/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/is-date-object/package.json` & `swanlab-0.3.1/node_modules/is-date-object/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/is-extglob/package.json` & `swanlab-0.3.1/node_modules/is-extglob/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/is-fullwidth-code-point/package.json` & `swanlab-0.3.1/node_modules/is-fullwidth-code-point/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/is-glob/package.json` & `swanlab-0.3.1/node_modules/is-glob/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/is-negative-zero/package.json` & `swanlab-0.3.1/node_modules/is-negative-zero/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/is-negative-zero/tsconfig.json` & `swanlab-0.3.1/node_modules/is-negative-zero/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/is-number/package.json` & `swanlab-0.3.1/node_modules/is-number/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/is-number-object/package.json` & `swanlab-0.3.1/node_modules/is-number-object/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/is-path-inside/package.json` & `swanlab-0.3.1/node_modules/is-path-inside/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/is-regex/package.json` & `swanlab-0.3.1/node_modules/is-regex/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/is-shared-array-buffer/package.json` & `swanlab-0.3.1/node_modules/is-shared-array-buffer/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/is-shared-array-buffer/tsconfig.json` & `swanlab-0.3.1/node_modules/is-shared-array-buffer/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/is-stream/package.json` & `swanlab-0.3.1/node_modules/is-stream/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/is-string/package.json` & `swanlab-0.3.1/node_modules/is-string/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/is-symbol/package.json` & `swanlab-0.3.1/node_modules/is-symbol/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/is-typed-array/package.json` & `swanlab-0.3.1/node_modules/is-typed-array/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/is-typed-array/tsconfig.json` & `swanlab-0.3.1/node_modules/is-typed-array/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/is-weakref/package.json` & `swanlab-0.3.1/node_modules/is-weakref/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/isarray/package.json` & `swanlab-0.3.1/node_modules/isarray/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/isexe/package.json` & `swanlab-0.3.1/node_modules/isexe/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/jackspeak/package.json` & `swanlab-0.3.1/node_modules/jackspeak/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/jiti/package.json` & `swanlab-0.3.1/node_modules/jiti/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/js-yaml/package.json` & `swanlab-0.3.1/node_modules/js-yaml/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/json-buffer/package.json` & `swanlab-0.3.1/node_modules/json-buffer/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/json-schema-traverse/package.json` & `swanlab-0.3.1/node_modules/json-schema-traverse/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/json-stable-stringify-without-jsonify/package.json` & `swanlab-0.3.1/node_modules/json-stable-stringify-without-jsonify/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/json2module/package.json` & `swanlab-0.3.1/node_modules/json2module/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/json5/package.json` & `swanlab-0.3.1/node_modules/json5/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/keyv/package.json` & `swanlab-0.3.1/node_modules/keyv/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/kind-of/package.json` & `swanlab-0.3.1/node_modules/kind-of/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/lazy-cache/package.json` & `swanlab-0.3.1/node_modules/lazy-cache/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/levn/package.json` & `swanlab-0.3.1/node_modules/levn/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/lilconfig/package.json` & `swanlab-0.3.1/node_modules/lilconfig/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/lines-and-columns/package.json` & `swanlab-0.3.1/node_modules/lines-and-columns/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/local-pkg/package.json` & `swanlab-0.3.1/node_modules/local-pkg/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/locate-path/package.json` & `swanlab-0.3.1/node_modules/locate-path/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/lodash/package.json` & `swanlab-0.3.1/node_modules/lodash/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/lodash-es/package.json` & `swanlab-0.3.1/node_modules/lodash-es/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/lodash.merge/package.json` & `swanlab-0.3.1/node_modules/lodash.merge/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/longest/package.json` & `swanlab-0.3.1/node_modules/longest/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/loupe/package.json` & `swanlab-0.3.1/node_modules/loupe/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/lru-cache/package.json` & `swanlab-0.3.1/node_modules/lru-cache/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/magic-string/package.json` & `swanlab-0.3.1/node_modules/magic-string/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/merge2/package.json` & `swanlab-0.3.1/node_modules/merge2/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/micromatch/package.json` & `swanlab-0.3.1/node_modules/micromatch/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/mime-db/db.json` & `swanlab-0.3.1/node_modules/mime-db/db.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/mime-db/package.json` & `swanlab-0.3.1/node_modules/mime-db/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/mime-types/package.json` & `swanlab-0.3.1/node_modules/mime-types/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/mimic-fn/package.json` & `swanlab-0.3.1/node_modules/mimic-fn/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/minimatch/package.json` & `swanlab-0.3.1/node_modules/minimatch/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/minimist/package.json` & `swanlab-0.3.1/node_modules/minimist/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/minipass/package.json` & `swanlab-0.3.1/node_modules/minipass/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/mlly/package.json` & `swanlab-0.3.1/node_modules/mlly/package.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9148065476190477%*

 * *Differences: {"'dependencies'": "{'pkg-types': '^1.1.0', 'ufo': '^1.5.3'}",*

 * * "'devDependencies'": "{'@types/node': '^20.12.7', '@vitest/coverage-v8': '^1.5.3', 'eslint': "*

 * *                      "'^9.1.1', 'eslint-config-unjs': '0.3.0-rc.7', 'import-meta-resolve': "*

 * *                      "'^4.1.0', 'prettier': '^3.2.5', 'typescript': '^5.4.5', 'vitest': '^1.5.3'}",*

 * * "'packageManager'": "'pnpm@9.0.6'",*

 * * "'scripts'": "{'lint': 'eslint src test && prettier -c src test', 'lint:fix': 'eslint src test "*

 * *              "--fix && […]*

```diff
@@ -1,50 +1,50 @@
 {
     "dependencies": {
         "acorn": "^8.11.3",
         "pathe": "^1.1.2",
-        "pkg-types": "^1.0.3",
-        "ufo": "^1.3.2"
+        "pkg-types": "^1.1.0",
+        "ufo": "^1.5.3"
     },
     "description": "Missing ECMAScript module utils for Node.js",
     "devDependencies": {
-        "@types/node": "^20.11.16",
-        "@vitest/coverage-v8": "^1.2.2",
+        "@types/node": "^20.12.7",
+        "@vitest/coverage-v8": "^1.5.3",
         "changelogen": "^0.5.5",
-        "eslint": "^8.56.0",
-        "eslint-config-unjs": "^0.2.1",
-        "import-meta-resolve": "^4.0.0",
+        "eslint": "^9.1.1",
+        "eslint-config-unjs": "0.3.0-rc.7",
+        "import-meta-resolve": "^4.1.0",
         "jiti": "^1.21.0",
-        "prettier": "^3.2.4",
+        "prettier": "^3.2.5",
         "std-env": "^3.7.0",
-        "typescript": "^5.3.3",
+        "typescript": "^5.4.5",
         "unbuild": "^2.0.0",
-        "vitest": "^1.2.2"
+        "vitest": "^1.5.3"
     },
     "exports": {
         "import": "./dist/index.mjs",
         "require": "./dist/index.cjs",
         "types": "./dist/index.d.ts"
     },
     "files": [
         "dist"
     ],
     "license": "MIT",
     "main": "./dist/index.cjs",
     "module": "./dist/index.mjs",
     "name": "mlly",
-    "packageManager": "pnpm@8.15.1",
+    "packageManager": "pnpm@9.0.6",
     "repository": "unjs/mlly",
     "scripts": {
         "build": "unbuild",
         "dev": "vitest",
-        "lint": "eslint --ext .ts,.js src test && prettier -c src test",
-        "lint:fix": "eslint --ext .ts,.js src test --fix && prettier -w src test",
+        "lint": "eslint src test && prettier -c src test",
+        "lint:fix": "eslint src test --fix && prettier -w src test",
         "release": "pnpm test && pnpm build && changelogen --release && npm publish && git push --follow-tags",
         "test": "pnpm lint && pnpm test:types && vitest run",
         "test:types": "tsc --noEmit"
     },
     "sideEffects": false,
     "type": "module",
     "types": "./dist/index.d.ts",
-    "version": "1.6.1"
+    "version": "1.7.0"
 }
```

### Comparing `swanlab-0.3.0/node_modules/mock-property/package.json` & `swanlab-0.3.1/node_modules/mock-property/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/mockjs/package.json` & `swanlab-0.3.1/node_modules/mockjs/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/moment/package.json` & `swanlab-0.3.1/node_modules/moment/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/ms/package.json` & `swanlab-0.3.1/node_modules/ms/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/mz/package.json` & `swanlab-0.3.1/node_modules/mz/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/nanoid/package.json` & `swanlab-0.3.1/node_modules/nanoid/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/natural-compare/package.json` & `swanlab-0.3.1/node_modules/natural-compare/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/node-releases/data/processed/envs.json` & `swanlab-0.3.1/node_modules/node-releases/data/processed/envs.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/node-releases/data/release-schedule/release-schedule.json` & `swanlab-0.3.1/node_modules/node-releases/data/release-schedule/release-schedule.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/normalize-path/package.json` & `swanlab-0.3.1/node_modules/normalize-path/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/normalize-range/package.json` & `swanlab-0.3.1/node_modules/normalize-range/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/npm-run-path/package.json` & `swanlab-0.3.1/node_modules/npm-run-path/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/npm-run-path/node_modules/path-key/package.json` & `swanlab-0.3.1/node_modules/npm-run-path/node_modules/path-key/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/nth-check/package.json` & `swanlab-0.3.1/node_modules/nth-check/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/object-assign/package.json` & `swanlab-0.3.1/node_modules/object-assign/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/object-hash/package.json` & `swanlab-0.3.1/node_modules/object-hash/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/object-inspect/package.json` & `swanlab-0.3.1/node_modules/object-inspect/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/object-is/package.json` & `swanlab-0.3.1/node_modules/object-is/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/object-keys/package.json` & `swanlab-0.3.1/node_modules/object-keys/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/object.assign/package.json` & `swanlab-0.3.1/node_modules/object.assign/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/once/package.json` & `swanlab-0.3.1/node_modules/once/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/onetime/package.json` & `swanlab-0.3.1/node_modules/onetime/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/optionator/package.json` & `swanlab-0.3.1/node_modules/optionator/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/p-limit/package.json` & `swanlab-0.3.1/node_modules/p-limit/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/p-locate/package.json` & `swanlab-0.3.1/node_modules/p-locate/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/parent-module/package.json` & `swanlab-0.3.1/node_modules/parent-module/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/path-exists/package.json` & `swanlab-0.3.1/node_modules/path-exists/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/path-is-absolute/package.json` & `swanlab-0.3.1/node_modules/path-is-absolute/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/path-key/package.json` & `swanlab-0.3.1/node_modules/path-key/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/path-parse/package.json` & `swanlab-0.3.1/node_modules/path-parse/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/path-scurry/package.json` & `swanlab-0.3.1/node_modules/path-scurry/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/path-scurry/node_modules/lru-cache/package.json` & `swanlab-0.3.1/node_modules/path-scurry/node_modules/lru-cache/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/pathe/package.json` & `swanlab-0.3.1/node_modules/pathe/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/pathval/package.json` & `swanlab-0.3.1/node_modules/pathval/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/pdfast/package.json` & `swanlab-0.3.1/node_modules/pdfast/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/picocolors/package.json` & `swanlab-0.3.1/node_modules/picocolors/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/picomatch/package.json` & `swanlab-0.3.1/node_modules/picomatch/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/pify/package.json` & `swanlab-0.3.1/node_modules/pify/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/pinia/package.json` & `swanlab-0.3.1/node_modules/pinia/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/pinia/node_modules/vue-demi/package.json` & `swanlab-0.3.1/node_modules/pinia/node_modules/vue-demi/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/pirates/package.json` & `swanlab-0.3.1/node_modules/pirates/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/pkg-types/package.json` & `swanlab-0.3.1/node_modules/pkg-types/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/possible-typed-array-names/package.json` & `swanlab-0.3.1/node_modules/possible-typed-array-names/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/possible-typed-array-names/tsconfig.json` & `swanlab-0.3.1/node_modules/possible-typed-array-names/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/postcss/package.json` & `swanlab-0.3.1/node_modules/postcss/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/postcss-import/package.json` & `swanlab-0.3.1/node_modules/postcss-import/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/postcss-js/package.json` & `swanlab-0.3.1/node_modules/postcss-js/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/postcss-load-config/package.json` & `swanlab-0.3.1/node_modules/postcss-load-config/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/postcss-load-config/node_modules/lilconfig/package.json` & `swanlab-0.3.1/node_modules/postcss-load-config/node_modules/lilconfig/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/postcss-nested/package.json` & `swanlab-0.3.1/node_modules/postcss-nested/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/postcss-selector-parser/package.json` & `swanlab-0.3.1/node_modules/postcss-selector-parser/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/postcss-value-parser/package.json` & `swanlab-0.3.1/node_modules/postcss-value-parser/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/prelude-ls/package.json` & `swanlab-0.3.1/node_modules/prelude-ls/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/prettier-linter-helpers/package.json` & `swanlab-0.3.1/node_modules/prettier-linter-helpers/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/pretty-format/package.json` & `swanlab-0.3.1/node_modules/pretty-format/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/pretty-format/node_modules/ansi-styles/package.json` & `swanlab-0.3.1/node_modules/pretty-format/node_modules/ansi-styles/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/proxy-from-env/package.json` & `swanlab-0.3.1/node_modules/proxy-from-env/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/punycode/package.json` & `swanlab-0.3.1/node_modules/punycode/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/queue-microtask/package.json` & `swanlab-0.3.1/node_modules/queue-microtask/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/read-cache/package.json` & `swanlab-0.3.1/node_modules/read-cache/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/readdirp/package.json` & `swanlab-0.3.1/node_modules/readdirp/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/regexp.prototype.flags/package.json` & `swanlab-0.3.1/node_modules/regexp.prototype.flags/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/repeat-string/package.json` & `swanlab-0.3.1/node_modules/repeat-string/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/resolve/package.json` & `swanlab-0.3.1/node_modules/resolve/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/resolve/lib/core.json` & `swanlab-0.3.1/node_modules/resolve/lib/core.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/resolve-from/package.json` & `swanlab-0.3.1/node_modules/resolve-from/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/reusify/package.json` & `swanlab-0.3.1/node_modules/reusify/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/right-align/package.json` & `swanlab-0.3.1/node_modules/right-align/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/rimraf/package.json` & `swanlab-0.3.1/node_modules/rimraf/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/rollup/package.json` & `swanlab-0.3.1/node_modules/rollup/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/rollup/node_modules/ansi-regex/package.json` & `swanlab-0.3.1/node_modules/rollup/node_modules/ansi-regex/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/rollup/node_modules/ansi-styles/package.json` & `swanlab-0.3.1/node_modules/rollup/node_modules/ansi-styles/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/rollup/node_modules/chalk/package.json` & `swanlab-0.3.1/node_modules/rollup/node_modules/chalk/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/rollup/node_modules/escape-string-regexp/package.json` & `swanlab-0.3.1/node_modules/rollup/node_modules/escape-string-regexp/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/rollup/node_modules/strip-ansi/package.json` & `swanlab-0.3.1/node_modules/rollup/node_modules/strip-ansi/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/rollup/node_modules/supports-color/package.json` & `swanlab-0.3.1/node_modules/rollup/node_modules/supports-color/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/run-parallel/package.json` & `swanlab-0.3.1/node_modules/run-parallel/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/rw/package.json` & `swanlab-0.3.1/node_modules/rw/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/safe-array-concat/package.json` & `swanlab-0.3.1/node_modules/safe-array-concat/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/safe-regex-test/package.json` & `swanlab-0.3.1/node_modules/safe-regex-test/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/sass/package.json` & `swanlab-0.3.1/node_modules/sass/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'version'": "'1.76.0'"}*

```diff
@@ -40,9 +40,9 @@
     "main": "sass.node.js",
     "name": "sass",
     "repository": {
         "type": "git",
         "url": "https://github.com/sass/dart-sass"
     },
     "types": "types/index.d.ts",
-    "version": "1.75.0"
+    "version": "1.76.0"
 }
```

### Comparing `swanlab-0.3.0/node_modules/scule/package.json` & `swanlab-0.3.1/node_modules/scule/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/semver/package.json` & `swanlab-0.3.1/node_modules/semver/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/set-function-length/package.json` & `swanlab-0.3.1/node_modules/set-function-length/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/set-function-name/package.json` & `swanlab-0.3.1/node_modules/set-function-name/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/set-function-name/tsconfig.json` & `swanlab-0.3.1/node_modules/set-function-name/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/shebang-command/package.json` & `swanlab-0.3.1/node_modules/shebang-command/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/shebang-regex/package.json` & `swanlab-0.3.1/node_modules/shebang-regex/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/side-channel/package.json` & `swanlab-0.3.1/node_modules/side-channel/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/side-channel/tsconfig.json` & `swanlab-0.3.1/node_modules/side-channel/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/side-channel/node_modules/object-inspect/package.json` & `swanlab-0.3.1/node_modules/side-channel/node_modules/object-inspect/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/siginfo/package.json` & `swanlab-0.3.1/node_modules/siginfo/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/signal-exit/package.json` & `swanlab-0.3.1/node_modules/signal-exit/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/size-sensor/package.json` & `swanlab-0.3.1/node_modules/size-sensor/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/source-map/package.json` & `swanlab-0.3.1/node_modules/source-map/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/source-map-js/package.json` & `swanlab-0.3.1/node_modules/source-map-js/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/source-map-support/package.json` & `swanlab-0.3.1/node_modules/source-map-support/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/std-env/package.json` & `swanlab-0.3.1/node_modules/std-env/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/string-width/package.json` & `swanlab-0.3.1/node_modules/string-width/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/string-width/node_modules/ansi-regex/package.json` & `swanlab-0.3.1/node_modules/string-width/node_modules/ansi-regex/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/string-width/node_modules/strip-ansi/package.json` & `swanlab-0.3.1/node_modules/string-width/node_modules/strip-ansi/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/string-width-cjs/package.json` & `swanlab-0.3.1/node_modules/string-width-cjs/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/string-width-cjs/node_modules/emoji-regex/package.json` & `swanlab-0.3.1/node_modules/string-width-cjs/node_modules/emoji-regex/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/string.prototype.trim/package.json` & `swanlab-0.3.1/node_modules/string.prototype.trim/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/string.prototype.trimend/package.json` & `swanlab-0.3.1/node_modules/string.prototype.trimend/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/string.prototype.trimstart/package.json` & `swanlab-0.3.1/node_modules/string.prototype.trimstart/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/strip-ansi/package.json` & `swanlab-0.3.1/node_modules/strip-ansi/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/strip-ansi-cjs/package.json` & `swanlab-0.3.1/node_modules/strip-ansi-cjs/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/strip-final-newline/package.json` & `swanlab-0.3.1/node_modules/strip-final-newline/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/strip-json-comments/package.json` & `swanlab-0.3.1/node_modules/strip-json-comments/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/strip-literal/package.json` & `swanlab-0.3.1/node_modules/strip-literal/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/sucrase/package.json` & `swanlab-0.3.1/node_modules/sucrase/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/sucrase/node_modules/brace-expansion/package.json` & `swanlab-0.3.1/node_modules/sucrase/node_modules/brace-expansion/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/sucrase/node_modules/commander/package.json` & `swanlab-0.3.1/node_modules/sucrase/node_modules/commander/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/sucrase/node_modules/glob/package.json` & `swanlab-0.3.1/node_modules/sucrase/node_modules/glob/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/sucrase/node_modules/minimatch/package.json` & `swanlab-0.3.1/node_modules/sucrase/node_modules/minimatch/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/supports-color/package.json` & `swanlab-0.3.1/node_modules/supports-color/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/supports-preserve-symlinks-flag/package.json` & `swanlab-0.3.1/node_modules/supports-preserve-symlinks-flag/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/tailwindcss/package.json` & `swanlab-0.3.1/node_modules/tailwindcss/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/tape/package.json` & `swanlab-0.3.1/node_modules/tape/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/terser/package.json` & `swanlab-0.3.1/node_modules/terser/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9772727272727273%*

 * *Differences: {"'version'": "'5.31.0'"}*

```diff
@@ -145,9 +145,9 @@
         "prepare": "npm run build",
         "test": "node test/compress.js && mocha test/mocha",
         "test:compress": "node test/compress.js",
         "test:mocha": "mocha test/mocha"
     },
     "type": "module",
     "types": "tools/terser.d.ts",
-    "version": "5.30.4"
+    "version": "5.31.0"
 }
```

### Comparing `swanlab-0.3.0/node_modules/terser/node_modules/commander/package.json` & `swanlab-0.3.1/node_modules/terser/node_modules/commander/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/terser/node_modules/source-map/package.json` & `swanlab-0.3.1/node_modules/terser/node_modules/source-map/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/terser/node_modules/source-map-support/package.json` & `swanlab-0.3.1/node_modules/terser/node_modules/source-map-support/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/text-table/package.json` & `swanlab-0.3.1/node_modules/text-table/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/thenify/package.json` & `swanlab-0.3.1/node_modules/thenify/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/thenify-all/package.json` & `swanlab-0.3.1/node_modules/thenify-all/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/tinybench/package.json` & `swanlab-0.3.1/node_modules/tinybench/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/tinypool/package.json` & `swanlab-0.3.1/node_modules/tinypool/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/tinyspy/package.json` & `swanlab-0.3.1/node_modules/tinyspy/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/tippy.js/package.json` & `swanlab-0.3.1/node_modules/tippy.js/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/to-regex-range/package.json` & `swanlab-0.3.1/node_modules/to-regex-range/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/ts-interface-checker/package.json` & `swanlab-0.3.1/node_modules/ts-interface-checker/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/tslib/package.json` & `swanlab-0.3.1/node_modules/tslib/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/type-check/package.json` & `swanlab-0.3.1/node_modules/type-check/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/type-detect/package.json` & `swanlab-0.3.1/node_modules/type-detect/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/type-fest/package.json` & `swanlab-0.3.1/node_modules/type-fest/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/typed-array-buffer/package.json` & `swanlab-0.3.1/node_modules/typed-array-buffer/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/typed-array-buffer/tsconfig.json` & `swanlab-0.3.1/node_modules/typed-array-buffer/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/typed-array-byte-length/package.json` & `swanlab-0.3.1/node_modules/typed-array-byte-length/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/typed-array-byte-length/tsconfig.json` & `swanlab-0.3.1/node_modules/typed-array-byte-length/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/typed-array-byte-offset/package.json` & `swanlab-0.3.1/node_modules/typed-array-byte-offset/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/typed-array-byte-offset/tsconfig.json` & `swanlab-0.3.1/node_modules/typed-array-byte-offset/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/typed-array-length/package.json` & `swanlab-0.3.1/node_modules/typed-array-length/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/ufo/package.json` & `swanlab-0.3.1/node_modules/ufo/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/uglify-js/package.json` & `swanlab-0.3.1/node_modules/uglify-js/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/uglify-js/node_modules/source-map/package.json` & `swanlab-0.3.1/node_modules/uglify-js/node_modules/source-map/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/uglify-js/tools/domprops.json` & `swanlab-0.3.1/node_modules/uglify-js/tools/domprops.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/unbox-primitive/package.json` & `swanlab-0.3.1/node_modules/unbox-primitive/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/unimport/package.json` & `swanlab-0.3.1/node_modules/unimport/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/unimport/node_modules/escape-string-regexp/package.json` & `swanlab-0.3.1/node_modules/unimport/node_modules/escape-string-regexp/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/unimport/node_modules/estree-walker/package.json` & `swanlab-0.3.1/node_modules/unimport/node_modules/estree-walker/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/unimport/node_modules/local-pkg/package.json` & `swanlab-0.3.1/node_modules/unimport/node_modules/local-pkg/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/unplugin/package.json` & `swanlab-0.3.1/node_modules/unplugin/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/unplugin-auto-import/package.json` & `swanlab-0.3.1/node_modules/unplugin-auto-import/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/unplugin-auto-import/node_modules/brace-expansion/package.json` & `swanlab-0.3.1/node_modules/unplugin-auto-import/node_modules/brace-expansion/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/unplugin-auto-import/node_modules/minimatch/package.json` & `swanlab-0.3.1/node_modules/unplugin-auto-import/node_modules/minimatch/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/unplugin-vue-components/package.json` & `swanlab-0.3.1/node_modules/unplugin-vue-components/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/unplugin-vue-components/node_modules/brace-expansion/package.json` & `swanlab-0.3.1/node_modules/unplugin-vue-components/node_modules/brace-expansion/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/unplugin-vue-components/node_modules/minimatch/package.json` & `swanlab-0.3.1/node_modules/unplugin-vue-components/node_modules/minimatch/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/update-browserslist-db/package.json` & `swanlab-0.3.1/node_modules/update-browserslist-db/package.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9519230769230769%*

 * *Differences: {"'dependencies'": "{'escalade': '^3.1.2'}", "'version'": "'1.0.14'"}*

```diff
@@ -1,12 +1,12 @@
 {
     "author": "Andrey Sitnik <andrey@sitnik.ru>",
     "bin": "cli.js",
     "dependencies": {
-        "escalade": "^3.1.1",
+        "escalade": "^3.1.2",
         "picocolors": "^1.0.0"
     },
     "description": "CLI tool to update caniuse-lite to refresh target browsers from Browserslist config",
     "exports": {
         ".": "./index.js",
         "./package.json": "./package.json"
     },
@@ -32,9 +32,9 @@
     "license": "MIT",
     "name": "update-browserslist-db",
     "peerDependencies": {
         "browserslist": ">= 4.21.0"
     },
     "repository": "browserslist/update-db",
     "types": "./index.d.ts",
-    "version": "1.0.13"
+    "version": "1.0.14"
 }
```

### Comparing `swanlab-0.3.0/node_modules/uri-js/package.json` & `swanlab-0.3.1/node_modules/uri-js/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/util-deprecate/package.json` & `swanlab-0.3.1/node_modules/util-deprecate/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/vite/package.json` & `swanlab-0.3.1/node_modules/vite/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/vite/node_modules/rollup/package.json` & `swanlab-0.3.1/node_modules/vite/node_modules/rollup/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9674036002360811%*

 * *Differences: {"'optionalDependencies'": "{'@rollup/rollup-darwin-arm64': '4.17.2', "*

 * *                           "'@rollup/rollup-android-arm64': '4.17.2', "*

 * *                           "'@rollup/rollup-win32-arm64-msvc': '4.17.2', "*

 * *                           "'@rollup/rollup-linux-arm64-gnu': '4.17.2', "*

 * *                           "'@rollup/rollup-linux-arm64-musl': '4.17.2', "*

 * *                           "'@rollup/rollup-android-arm-eabi': '4.17.2', "*

 * *                           "'@rollup/rollup-linux-arm-gnueabihf': '4. […]*

```diff
@@ -167,41 +167,42 @@
                 "x86_64-unknown-linux-gnu",
                 "x86_64-unknown-linux-musl"
             ],
             "defaults": false
         }
     },
     "optionalDependencies": {
-        "@rollup/rollup-android-arm-eabi": "4.17.1",
-        "@rollup/rollup-android-arm64": "4.17.1",
-        "@rollup/rollup-darwin-arm64": "4.17.1",
-        "@rollup/rollup-darwin-x64": "4.17.1",
-        "@rollup/rollup-linux-arm-gnueabihf": "4.17.1",
-        "@rollup/rollup-linux-arm-musleabihf": "4.17.1",
-        "@rollup/rollup-linux-arm64-gnu": "4.17.1",
-        "@rollup/rollup-linux-arm64-musl": "4.17.1",
-        "@rollup/rollup-linux-powerpc64le-gnu": "4.17.1",
-        "@rollup/rollup-linux-riscv64-gnu": "4.17.1",
-        "@rollup/rollup-linux-s390x-gnu": "4.17.1",
-        "@rollup/rollup-linux-x64-gnu": "4.17.1",
-        "@rollup/rollup-linux-x64-musl": "4.17.1",
-        "@rollup/rollup-win32-arm64-msvc": "4.17.1",
-        "@rollup/rollup-win32-ia32-msvc": "4.17.1",
-        "@rollup/rollup-win32-x64-msvc": "4.17.1",
+        "@rollup/rollup-android-arm-eabi": "4.17.2",
+        "@rollup/rollup-android-arm64": "4.17.2",
+        "@rollup/rollup-darwin-arm64": "4.17.2",
+        "@rollup/rollup-darwin-x64": "4.17.2",
+        "@rollup/rollup-linux-arm-gnueabihf": "4.17.2",
+        "@rollup/rollup-linux-arm-musleabihf": "4.17.2",
+        "@rollup/rollup-linux-arm64-gnu": "4.17.2",
+        "@rollup/rollup-linux-arm64-musl": "4.17.2",
+        "@rollup/rollup-linux-powerpc64le-gnu": "4.17.2",
+        "@rollup/rollup-linux-riscv64-gnu": "4.17.2",
+        "@rollup/rollup-linux-s390x-gnu": "4.17.2",
+        "@rollup/rollup-linux-x64-gnu": "4.17.2",
+        "@rollup/rollup-linux-x64-musl": "4.17.2",
+        "@rollup/rollup-win32-arm64-msvc": "4.17.2",
+        "@rollup/rollup-win32-ia32-msvc": "4.17.2",
+        "@rollup/rollup-win32-x64-msvc": "4.17.2",
         "fsevents": "~2.3.2"
     },
     "overrides": {
         "axios": "^1.6.8",
         "semver": "^7.6.0"
     },
     "repository": "rollup/rollup",
     "scripts": {
         "build": "concurrently -c green,blue \"npm run build:wasm\" \"npm:build:ast-converters\" && concurrently -c green,blue \"npm run build:napi -- --release\" \"npm:build:js\" && npm run build:copy-native",
         "build:ast-converters": "node scripts/generate-ast-converters.js",
         "build:bootstrap": "shx mv dist dist-build && node dist-build/bin/rollup --config rollup.config.ts --configPlugin typescript --forceExit && shx rm -rf dist-build",
+        "build:bootstrap:cjs": "shx mv dist dist-build && node dist-build/bin/rollup --config rollup.config.ts --configPlugin typescript --configTest --forceExit && shx rm -rf dist-build",
         "build:cjs": "rollup --config rollup.config.ts --configPlugin typescript --configTest --forceExit",
         "build:copy-native": "shx mkdir -p dist && shx cp rollup.*.node dist/",
         "build:docs": "vitepress build docs",
         "build:js": "rollup --config rollup.config.ts --configPlugin typescript --forceExit",
         "build:js:node": "rollup --config rollup.config.ts --configPlugin typescript --configIsBuildNode --forceExit",
         "build:napi": "napi build --platform --dts native.d.ts --js false --cargo-cwd rust -p bindings_napi --cargo-name bindings_napi",
         "build:prepare": "concurrently -c green,blue \"npm run build:napi -- --release\" \"npm:build:js:node\" && npm run build:copy-native",
@@ -218,15 +219,15 @@
         "lint:js": "eslint . --fix --cache",
         "lint:js:nofix": "eslint . --cache",
         "lint:markdown": "prettier --write \"**/*.md\"",
         "lint:markdown:nofix": "prettier --check \"**/*.md\"",
         "lint:native-js": "node scripts/lint-native-js.js",
         "lint:rust": "cd rust && cargo fmt && cargo clippy --fix --allow-dirty",
         "lint:rust:nofix": "cd rust && cargo fmt --check && cargo clippy",
-        "perf": "npm run build && node --expose-gc scripts/perf-report/index.js",
+        "perf": "npm run build:bootstrap:cjs && node --expose-gc scripts/perf-report/index.js",
         "postpublish": "node scripts/postpublish.js",
         "prepare": "husky && node scripts/check-release.js || npm run build:prepare",
         "prepublish:napi": "napi prepublish --skip-gh-release",
         "prepublishOnly": "node scripts/check-release.js && node scripts/prepublish.js",
         "preview:docs": "vitepress preview docs",
         "release": "node scripts/prepare-release.js",
         "release:docs": "git fetch --update-head-ok origin master:master && git branch --force documentation-published master && git push origin documentation-published",
@@ -244,9 +245,9 @@
         "test:typescript": "shx rm -rf test/typescript/dist && shx cp -r dist test/typescript/ && tsc --noEmit -p test/typescript && tsc --noEmit && tsc --noEmit -p scripts",
         "test:update-snapshots": "node scripts/update-snapshots.js",
         "update:js": "npm run build:js && npm run build:copy-native",
         "update:napi": "npm run build:napi && npm run build:copy-native",
         "watch": "rollup --config rollup.config.ts --configPlugin typescript --watch"
     },
     "types": "dist/rollup.d.ts",
-    "version": "4.17.1"
+    "version": "4.17.2"
 }
```

### Comparing `swanlab-0.3.0/node_modules/vite-node/package.json` & `swanlab-0.3.1/node_modules/vite-node/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9772727272727273%*

 * *Differences: {"'version'": "'1.5.3'"}*

```diff
@@ -87,9 +87,9 @@
         "*": {
             "*": [
                 "./dist/*",
                 "./dist/index.d.ts"
             ]
         }
     },
-    "version": "1.5.2"
+    "version": "1.5.3"
 }
```

### Comparing `swanlab-0.3.0/node_modules/vite-plugin-json5/package.json` & `swanlab-0.3.1/node_modules/vite-plugin-json5/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/vitest/package.json` & `swanlab-0.3.1/node_modules/vitest/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9725694444444445%*

 * *Differences: {"'dependencies'": "{'@vitest/expect': '1.5.3', '@vitest/runner': '1.5.3', '@vitest/spy': '1.5.3', "*

 * *                   "'@vitest/utils': '1.5.3', 'vite-node': '1.5.3', '@vitest/snapshot': '1.5.3'}",*

 * * "'peerDependencies'": "{'@vitest/browser': '1.5.3', '@vitest/ui': '1.5.3'}",*

 * * "'version'": "'1.5.3'"}*

```diff
@@ -3,33 +3,33 @@
     "bin": {
         "vitest": "./vitest.mjs"
     },
     "bugs": {
         "url": "https://github.com/vitest-dev/vitest/issues"
     },
     "dependencies": {
-        "@vitest/expect": "1.5.2",
-        "@vitest/runner": "1.5.2",
-        "@vitest/snapshot": "1.5.2",
-        "@vitest/spy": "1.5.2",
-        "@vitest/utils": "1.5.2",
+        "@vitest/expect": "1.5.3",
+        "@vitest/runner": "1.5.3",
+        "@vitest/snapshot": "1.5.3",
+        "@vitest/spy": "1.5.3",
+        "@vitest/utils": "1.5.3",
         "acorn-walk": "^8.3.2",
         "chai": "^4.3.10",
         "debug": "^4.3.4",
         "execa": "^8.0.1",
         "local-pkg": "^0.5.0",
         "magic-string": "^0.30.5",
         "pathe": "^1.1.1",
         "picocolors": "^1.0.0",
         "std-env": "^3.5.0",
         "strip-literal": "^2.0.0",
         "tinybench": "^2.5.1",
         "tinypool": "^0.8.3",
         "vite": "^5.0.0",
-        "vite-node": "1.5.2",
+        "vite-node": "1.5.3",
         "why-is-node-running": "^2.2.2"
     },
     "description": "Next generation testing framework powered by Vite",
     "devDependencies": {
         "@ampproject/remapping": "^2.2.1",
         "@antfu/install-pkg": "^0.3.1",
         "@edge-runtime/vm": "^3.1.8",
@@ -154,16 +154,16 @@
     "license": "MIT",
     "main": "./dist/index.js",
     "module": "./dist/index.js",
     "name": "vitest",
     "peerDependencies": {
         "@edge-runtime/vm": "*",
         "@types/node": "^18.0.0 || >=20.0.0",
-        "@vitest/browser": "1.5.2",
-        "@vitest/ui": "1.5.2",
+        "@vitest/browser": "1.5.3",
+        "@vitest/ui": "1.5.3",
         "happy-dom": "*",
         "jsdom": "*"
     },
     "peerDependenciesMeta": {
         "@edge-runtime/vm": {
             "optional": true
         },
@@ -191,9 +191,9 @@
     "scripts": {
         "build": "rimraf dist && rollup -c",
         "dev": "NODE_OPTIONS=\"--max-old-space-size=8192\" rollup -c --watch -m inline"
     },
     "sideEffects": false,
     "type": "module",
     "types": "./dist/index.d.ts",
-    "version": "1.5.2"
+    "version": "1.5.3"
 }
```

### Comparing `swanlab-0.3.0/node_modules/vitest/node_modules/local-pkg/package.json` & `swanlab-0.3.1/node_modules/vitest/node_modules/local-pkg/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/vitest/node_modules/strip-literal/package.json` & `swanlab-0.3.1/node_modules/vitest/node_modules/strip-literal/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/vue/package.json` & `swanlab-0.3.1/node_modules/vue/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/vue-eslint-parser/package.json` & `swanlab-0.3.1/node_modules/vue-eslint-parser/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/vue-i18n/package.json` & `swanlab-0.3.1/node_modules/vue-i18n/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/vue-i18n/vetur/attributes.json` & `swanlab-0.3.1/node_modules/vue-i18n/vetur/attributes.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/vue-i18n/vetur/tags.json` & `swanlab-0.3.1/node_modules/vue-i18n/vetur/tags.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/vue-router/package.json` & `swanlab-0.3.1/node_modules/vue-router/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/vue-router/vetur/attributes.json` & `swanlab-0.3.1/node_modules/vue-router/vetur/attributes.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/vue-router/vetur/tags.json` & `swanlab-0.3.1/node_modules/vue-router/vetur/tags.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/vue-tippy/package.json` & `swanlab-0.3.1/node_modules/vue-tippy/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/vue-tippy/tsconfig.json` & `swanlab-0.3.1/node_modules/vue-tippy/tsconfig.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/vue-tippy/vetur/attributes.json` & `swanlab-0.3.1/node_modules/vue-tippy/vetur/attributes.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/vue-tippy/vetur/tags.json` & `swanlab-0.3.1/node_modules/vue-tippy/vetur/tags.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/webpack-sources/package.json` & `swanlab-0.3.1/node_modules/webpack-sources/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/webpack-virtual-modules/package.json` & `swanlab-0.3.1/node_modules/webpack-virtual-modules/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/which/package.json` & `swanlab-0.3.1/node_modules/which/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/which-boxed-primitive/package.json` & `swanlab-0.3.1/node_modules/which-boxed-primitive/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/which-typed-array/package.json` & `swanlab-0.3.1/node_modules/which-typed-array/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/why-is-node-running/package.json` & `swanlab-0.3.1/node_modules/why-is-node-running/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/window-size/package.json` & `swanlab-0.3.1/node_modules/window-size/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/word-wrap/package.json` & `swanlab-0.3.1/node_modules/word-wrap/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/wordwrap/package.json` & `swanlab-0.3.1/node_modules/wordwrap/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/wrap-ansi/package.json` & `swanlab-0.3.1/node_modules/wrap-ansi/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/wrap-ansi/node_modules/ansi-regex/package.json` & `swanlab-0.3.1/node_modules/wrap-ansi/node_modules/ansi-regex/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/wrap-ansi/node_modules/ansi-styles/package.json` & `swanlab-0.3.1/node_modules/wrap-ansi/node_modules/ansi-styles/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/wrap-ansi/node_modules/strip-ansi/package.json` & `swanlab-0.3.1/node_modules/wrap-ansi/node_modules/strip-ansi/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/wrap-ansi-cjs/package.json` & `swanlab-0.3.1/node_modules/wrap-ansi-cjs/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/wrap-ansi-cjs/node_modules/emoji-regex/package.json` & `swanlab-0.3.1/node_modules/wrap-ansi-cjs/node_modules/emoji-regex/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/wrap-ansi-cjs/node_modules/string-width/package.json` & `swanlab-0.3.1/node_modules/wrap-ansi-cjs/node_modules/string-width/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/wrappy/package.json` & `swanlab-0.3.1/node_modules/wrappy/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/xml-name-validator/package.json` & `swanlab-0.3.1/node_modules/xml-name-validator/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/yallist/package.json` & `swanlab-0.3.1/node_modules/yallist/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/yaml/package.json` & `swanlab-0.3.1/node_modules/yaml/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/yargs/package.json` & `swanlab-0.3.1/node_modules/yargs/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/node_modules/yocto-queue/package.json` & `swanlab-0.3.1/node_modules/yocto-queue/package.json`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/env.py` & `swanlab-0.3.1/swanlab/env.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/error.py` & `swanlab-0.3.1/swanlab/error.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/package.py` & `swanlab-0.3.1/swanlab/package.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/api/cos.py` & `swanlab-0.3.1/swanlab/api/cos.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/api/http.py` & `swanlab-0.3.1/swanlab/api/http.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/api/info.py` & `swanlab-0.3.1/swanlab/api/info.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/api/auth/login.py` & `swanlab-0.3.1/swanlab/api/auth/login.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/api/upload/__init__.py` & `swanlab-0.3.1/swanlab/api/upload/__init__.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/api/upload/model.py` & `swanlab-0.3.1/swanlab/api/upload/model.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/cli/main.py` & `swanlab-0.3.1/swanlab/cli/main.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/cli/utils.py` & `swanlab-0.3.1/swanlab/cli/utils.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/cloud/_log_collector.py` & `swanlab-0.3.1/swanlab/cloud/_log_collector.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/cloud/start_thread.py` & `swanlab-0.3.1/swanlab/cloud/start_thread.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/cloud/task_types.py` & `swanlab-0.3.1/swanlab/cloud/task_types.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/cloud/utils.py` & `swanlab-0.3.1/swanlab/cloud/utils.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/cloud/dog/log_sniffer.py` & `swanlab-0.3.1/swanlab/cloud/dog/log_sniffer.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/cloud/dog/metadata_handle.py` & `swanlab-0.3.1/swanlab/cloud/dog/metadata_handle.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/cloud/dog/sniffer_queue.py` & `swanlab-0.3.1/swanlab/cloud/dog/sniffer_queue.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/compat/server/controller/experiment.py` & `swanlab-0.3.1/swanlab/compat/server/controller/experiment.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/data/__init__.py` & `swanlab-0.3.1/swanlab/data/__init__.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/data/config.py` & `swanlab-0.3.1/swanlab/data/config.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/data/sdk.py` & `swanlab-0.3.1/swanlab/data/sdk.py`

 * *Files 0% similar despite different names*

```diff
@@ -389,23 +389,28 @@
         logdir = os.path.abspath("swanlog")
         try:
             os.makedirs(logdir, exist_ok=True)
             if not os.access(logdir, os.W_OK):
                 raise IOError
         except IOError:
             raise IOError("logdir must have Write permission.")
+    # 如果logdir是空的，创建.gitignore文件，写入*
+    if not os.listdir(logdir):
+        with open(os.path.join(logdir, ".gitignore"), "w") as f:
+            f.write("*")
     return logdir
 
 
 def _init_config(config: Union[dict, str]):
     """初始化传入的config参数"""
-    if isinstance(config, dict) or config is None:
-        return config
-    swanlog.info("The parameter config is loaded from the configuration file: {}".format(config))
-    return check_load_json_yaml(config, "config")
+    if isinstance(config, str):
+        swanlog.info("The parameter config is loaded from the configuration file: {}".format(config))
+        return check_load_json_yaml(config, "config")
+
+    return config
 
 
 def _load_data(load_data: dict, key: str, value):
     """从load_data中加载数据，如果value不是None"""
     if value is not None:
         # tip = "The parameter {} is loaded from the configuration file: {}".format(FONT.bold(key), value)
         # print(FONT.swanlab(tip))
```

### Comparing `swanlab-0.3.0/swanlab/data/settings.py` & `swanlab-0.3.1/swanlab/data/settings.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/data/modules/audio.py` & `swanlab-0.3.1/swanlab/data/modules/audio.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/data/modules/base.py` & `swanlab-0.3.1/swanlab/data/modules/base.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/data/modules/chart.py` & `swanlab-0.3.1/swanlab/data/modules/chart.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/data/modules/image.py` & `swanlab-0.3.1/swanlab/data/modules/image.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/data/modules/object_3d.py` & `swanlab-0.3.1/swanlab/data/modules/object_3d.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/data/modules/text.py` & `swanlab-0.3.1/swanlab/data/modules/text.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/data/modules/video.py` & `swanlab-0.3.1/swanlab/data/modules/video.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/data/modules/utils_modules/bounding_boxes.py` & `swanlab-0.3.1/swanlab/data/modules/utils_modules/bounding_boxes.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/data/modules/utils_modules/image_mask.py` & `swanlab-0.3.1/swanlab/data/modules/utils_modules/image_mask.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/data/run/exp.py` & `swanlab-0.3.1/swanlab/data/run/exp.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/data/run/main.py` & `swanlab-0.3.1/swanlab/data/run/main.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/data/system/info.py` & `swanlab-0.3.1/swanlab/data/system/info.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/data/system/monitor.py` & `swanlab-0.3.1/swanlab/data/system/monitor.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/data/system/bin/apple_gpu_stats` & `swanlab-0.3.1/swanlab/data/system/bin/apple_gpu_stats`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/data/utils/file.py` & `swanlab-0.3.1/swanlab/data/utils/file.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/data/utils/model.py` & `swanlab-0.3.1/swanlab/data/utils/model.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/db/__init__.py` & `swanlab-0.3.1/swanlab/db/__init__.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/db/db_connect.py` & `swanlab-0.3.1/swanlab/db/db_connect.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/db/error.py` & `swanlab-0.3.1/swanlab/db/error.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/db/model.py` & `swanlab-0.3.1/swanlab/db/model.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/db/docs/Errors.md` & `swanlab-0.3.1/swanlab/db/docs/Errors.md`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/db/docs/README.md` & `swanlab-0.3.1/swanlab/db/docs/README.md`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/db/migrate/chart.py` & `swanlab-0.3.1/swanlab/db/migrate/chart.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/db/migrate/experiment.py` & `swanlab-0.3.1/swanlab/db/migrate/experiment.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/db/migrate/namespace.py` & `swanlab-0.3.1/swanlab/db/migrate/namespace.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/db/migrate/project.py` & `swanlab-0.3.1/swanlab/db/migrate/project.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/db/models/charts.py` & `swanlab-0.3.1/swanlab/db/models/charts.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/db/models/displays.py` & `swanlab-0.3.1/swanlab/db/models/displays.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/db/models/experiments.py` & `swanlab-0.3.1/swanlab/db/models/experiments.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/db/models/namespaces.py` & `swanlab-0.3.1/swanlab/db/models/namespaces.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/db/models/projects.py` & `swanlab-0.3.1/swanlab/db/models/projects.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/db/models/sources.py` & `swanlab-0.3.1/swanlab/db/models/sources.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/db/models/tags.py` & `swanlab-0.3.1/swanlab/db/models/tags.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/db/utils/chart.py` & `swanlab-0.3.1/swanlab/db/utils/chart.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/integration/huggingface.py` & `swanlab-0.3.1/swanlab/integration/huggingface.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/integration/mmengine.py` & `swanlab-0.3.1/swanlab/integration/mmengine.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/integration/pytorch_lightning.py` & `swanlab-0.3.1/swanlab/integration/pytorch_lightning.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/integration/integration_utils/autologging.py` & `swanlab-0.3.1/swanlab/integration/integration_utils/autologging.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/integration/integration_utils/get_modules.py` & `swanlab-0.3.1/swanlab/integration/integration_utils/get_modules.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/integration/integration_utils/timer.py` & `swanlab-0.3.1/swanlab/integration/integration_utils/timer.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/integration/openai/openai.py` & `swanlab-0.3.1/swanlab/integration/openai/openai.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/integration/openai/resolver.py` & `swanlab-0.3.1/swanlab/integration/openai/resolver.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/integration/zhipuai/resolver.py` & `swanlab-0.3.1/swanlab/integration/zhipuai/resolver.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/integration/zhipuai/zhipuai.py` & `swanlab-0.3.1/swanlab/integration/zhipuai/zhipuai.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/log/console.py` & `swanlab-0.3.1/swanlab/log/console.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/log/log.py` & `swanlab-0.3.1/swanlab/log/log.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/server/app.py` & `swanlab-0.3.1/swanlab/server/app.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/server/settings.py` & `swanlab-0.3.1/swanlab/server/settings.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/server/controller/chart.py` & `swanlab-0.3.1/swanlab/server/controller/chart.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/server/controller/experiment.py` & `swanlab-0.3.1/swanlab/server/controller/experiment.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/server/controller/namespace.py` & `swanlab-0.3.1/swanlab/server/controller/namespace.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/server/controller/project.py` & `swanlab-0.3.1/swanlab/server/controller/project.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/server/controller/utils/__init__.py` & `swanlab-0.3.1/swanlab/server/controller/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/server/controller/utils/charts.py` & `swanlab-0.3.1/swanlab/server/controller/utils/charts.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/server/controller/utils/tag.py` & `swanlab-0.3.1/swanlab/server/controller/utils/tag.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/server/middleware/common.py` & `swanlab-0.3.1/swanlab/server/middleware/common.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/server/module/resp.py` & `swanlab-0.3.1/swanlab/server/module/resp.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/server/router/chart.py` & `swanlab-0.3.1/swanlab/server/router/chart.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/server/router/experiment.py` & `swanlab-0.3.1/swanlab/server/router/experiment.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/server/router/media.py` & `swanlab-0.3.1/swanlab/server/router/media.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/server/router/namespace.py` & `swanlab-0.3.1/swanlab/server/router/namespace.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/server/router/project.py` & `swanlab-0.3.1/swanlab/server/router/project.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/template/assets/ChartPage-CR1Gy4nD.js` & `swanlab-0.3.1/swanlab/template/assets/ChartPage-CR1Gy4nD.js`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/template/assets/ChartsView-Cp_w0mYy.js` & `swanlab-0.3.1/swanlab/template/assets/ChartsView-Cp_w0mYy.js`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/template/assets/EnvHardware-UlpkNHre.js` & `swanlab-0.3.1/swanlab/template/assets/EnvHardware-UlpkNHre.js`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/template/assets/EnvIndex-QRnlb5o-.js` & `swanlab-0.3.1/swanlab/template/assets/EnvIndex-QRnlb5o-.js`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/template/assets/EnvItems-BByd5_l_.js` & `swanlab-0.3.1/swanlab/template/assets/EnvItems-BByd5_l_.js`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/template/assets/EnvItems-BfjcRO-X.css` & `swanlab-0.3.1/swanlab/template/assets/EnvItems-BfjcRO-X.css`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/template/assets/EnvRequirements-C_C5xDM7.js` & `swanlab-0.3.1/swanlab/template/assets/EnvRequirements-C_C5xDM7.js`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/template/assets/EnvironmentPage-DWu4jgoh.js` & `swanlab-0.3.1/swanlab/template/assets/EnvironmentPage-DWu4jgoh.js`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/template/assets/ExperimentView-BwOYqQ05.js` & `swanlab-0.3.1/swanlab/template/assets/ExperimentView-BwOYqQ05.js`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/template/assets/ExperimentView-CCDMXo4h.css` & `swanlab-0.3.1/swanlab/template/assets/ExperimentView-CCDMXo4h.css`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/template/assets/FuncBar-BsXaYgxx.js` & `swanlab-0.3.1/swanlab/template/assets/FuncBar-BsXaYgxx.js`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/template/assets/HomeView-BIJzBfvA.css` & `swanlab-0.3.1/swanlab/template/assets/HomeView-BIJzBfvA.css`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/template/assets/HomeView-BM5pU9yO.js` & `swanlab-0.3.1/swanlab/template/assets/HomeView-BM5pU9yO.js`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/template/assets/IndexPage-C5dvtib2.css` & `swanlab-0.3.1/swanlab/template/assets/IndexPage-C5dvtib2.css`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/template/assets/IndexPage-DNYsYgRx.js` & `swanlab-0.3.1/swanlab/template/assets/IndexPage-DNYsYgRx.js`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/template/assets/JetBrainsMono-Regular-Dh36KTnx.ttf` & `swanlab-0.3.1/swanlab/template/assets/JetBrainsMono-Regular-Dh36KTnx.ttf`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/template/assets/LogPage-DBzoauOW.css` & `swanlab-0.3.1/swanlab/template/assets/LogPage-DBzoauOW.css`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/template/assets/LogPage-fDtMFLcB.js` & `swanlab-0.3.1/swanlab/template/assets/LogPage-fDtMFLcB.js`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/template/assets/NotFound--wQ84Mpr.js` & `swanlab-0.3.1/swanlab/template/assets/NotFound--wQ84Mpr.js`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/template/assets/SLLoading-wlC0Kmfx.js` & `swanlab-0.3.1/swanlab/template/assets/SLLoading-wlC0Kmfx.js`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/template/assets/SLStatusLabel-1A8U87-U.js` & `swanlab-0.3.1/swanlab/template/assets/SLStatusLabel-1A8U87-U.js`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/template/assets/SLStatusLabel-BRacn5XK.css` & `swanlab-0.3.1/swanlab/template/assets/SLStatusLabel-BRacn5XK.css`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/template/assets/SourceSansPro-Regular-J3NOkSfZ.ttf` & `swanlab-0.3.1/swanlab/template/assets/SourceSansPro-Regular-J3NOkSfZ.ttf`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/template/assets/chart-B0yY4W3r.js` & `swanlab-0.3.1/swanlab/template/assets/chart-B0yY4W3r.js`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/template/assets/chart-DXdkqIcq.css` & `swanlab-0.3.1/swanlab/template/assets/chart-DXdkqIcq.css`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/template/assets/index-BH23qgZj.js` & `swanlab-0.3.1/swanlab/template/assets/index-BH23qgZj.js`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/template/assets/index-DUgbEQPz.css` & `swanlab-0.3.1/swanlab/template/assets/index-DUgbEQPz.css`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/template/assets/logo-ChHf2ozk.ico` & `swanlab-0.3.1/swanlab/template/assets/logo-ChHf2ozk.ico`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/utils/file.py` & `swanlab-0.3.1/swanlab/utils/file.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/utils/font.py` & `swanlab-0.3.1/swanlab/utils/font.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/utils/judgment.py` & `swanlab-0.3.1/swanlab/utils/judgment.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/swanlab/utils/key.py` & `swanlab-0.3.1/swanlab/utils/key.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/test/create_experiment.py` & `swanlab-0.3.1/test/create_experiment.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/test/start_server.py` & `swanlab-0.3.1/test/start_server.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/test/unit/pytest_example.py` & `swanlab-0.3.1/test/unit/pytest_example.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/test/unit/auth/pytest_login.py` & `swanlab-0.3.1/test/unit/auth/pytest_login.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/test/unit/data/run/pytest_main.py` & `swanlab-0.3.1/test/unit/data/run/pytest_main.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/test/unit/log/pytest_log.py` & `swanlab-0.3.1/test/unit/log/pytest_log.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/test/unit/server/controller/utils/utils.py` & `swanlab-0.3.1/test/unit/server/controller/utils/utils.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/test/unit/utils/pytest_file.py` & `swanlab-0.3.1/test/unit/utils/pytest_file.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/test/unit/utils/pytest_key.py` & `swanlab-0.3.1/test/unit/utils/pytest_key.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/test/unit/utils/pytest_package.py` & `swanlab-0.3.1/test/unit/utils/pytest_package.py`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/LICENSE` & `swanlab-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/pyproject.toml` & `swanlab-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `swanlab-0.3.0/PKG-INFO` & `swanlab-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: swanlab
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python library for streamlined tracking and management of AI training processes.
 Project-URL: Homepage, https://swanhub.co
 Project-URL: Source, https://github.com/SwanHubX/SwanLab
 Project-URL: Bug Reports, https://github.com/SwanHubX/SwanLab/issues
 Project-URL: Documentation, https://geektechstudio.feishu.cn/wiki/space/7310593325374013444?ccm_open_type=lark_wiki_spaceLink&open_tab_from=wiki_home
 Author-email: Cunyue <team@swanhub.co>, Feudalman <team@swanhub.co>, ZeYi Lin <team@swanhub.co>, KashiwaByte <team@swanhub.co>
 License-Expression: Apache-2.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: swanlab Version: 0.3.0 Summary: Python library for
+Metadata-Version: 2.3 Name: swanlab Version: 0.3.1 Summary: Python library for
 streamlined tracking and management of AI training processes. Project-URL:
 Homepage, https://swanhub.co Project-URL: Source, https://github.com/SwanHubX/
 SwanLab Project-URL: Bug Reports, https://github.com/SwanHubX/SwanLab/issues
 Project-URL: Documentation, https://geektechstudio.feishu.cn/wiki/space/
 7310593325374013444?ccm_open_type=lark_wiki_spaceLink&open_tab_from=wiki_home
 Author-email: Cunyue
 swanhub.co>, Feudalman
```

