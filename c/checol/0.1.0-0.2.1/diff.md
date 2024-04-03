# Comparing `tmp/checol-0.1.0.tar.gz` & `tmp/checol-0.2.1.tar.gz`

## Comparing `checol-0.1.0.tar` & `checol-0.2.1.tar`

### file list

```diff
@@ -1,237 +1,237 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 checol-0.1.0/.python-version
--rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 checol-0.1.0/checol-0.1.0-py3-none-any.whl
--rw-r--r--   0        0        0     6035 2020-02-02 00:00:00.000000 checol-0.1.0/package-lock.json
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 checol-0.1.0/package.json
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 checol-0.1.0/requirements-dev.lock
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 checol-0.1.0/requirements.lock
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 checol-0.1.0/.github/workflows/rye-lint.yml
--rw-r--r--   0        0        0     5947 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/.package-lock.json
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/.bin/nanoid -> ../nanoid/bin/nanoid.cjs
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/.bin/parser -> ../@babel/parser/bin/babel-parser.js
--rw-r--r--   0        0        0    38238 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/@babel/parser/CHANGELOG.md
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/@babel/parser/LICENSE
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/@babel/parser/README.md
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/@babel/parser/index.cjs
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/@babel/parser/package.json
--rwxr-xr-x   0        0        0      328 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/@babel/parser/bin/babel-parser.js
--rw-r--r--   0        0        0   484739 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/@babel/parser/lib/index.js
--rw-r--r--   0        0        0  1349600 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/@babel/parser/lib/index.js.map
--rw-r--r--   0        0        0     7547 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/@babel/parser/typings/babel-parser.d.ts
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/@jridgewell/sourcemap-codec/LICENSE
--rw-r--r--   0        0        0     6893 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/@jridgewell/sourcemap-codec/README.md
--rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/@jridgewell/sourcemap-codec/package.json
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/@vue/compiler-core/LICENSE
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/@vue/compiler-core/README.md
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/@vue/compiler-core/index.js
--rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/@vue/compiler-core/package.json
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/@vue/compiler-dom/LICENSE
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/@vue/compiler-dom/README.md
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/@vue/compiler-dom/index.js
--rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/@vue/compiler-dom/package.json
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/@vue/compiler-sfc/LICENSE
--rw-r--r--   0        0        0     4444 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/@vue/compiler-sfc/README.md
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/@vue/compiler-sfc/package.json
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/@vue/compiler-ssr/LICENSE
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/@vue/compiler-ssr/README.md
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/@vue/compiler-ssr/package.json
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/@vue/shared/LICENSE
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/@vue/shared/README.md
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/@vue/shared/index.js
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/@vue/shared/package.json
--rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/LICENSE
--rw-r--r--   0        0        0     2883 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/package.json
--rw-r--r--   0        0        0     5074 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/readme.md
--rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/decode.d.ts
--rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/decode.d.ts.map
--rw-r--r--   0        0        0    22611 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/decode.js
--rw-r--r--   0        0        0    11591 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/decode.js.map
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/decode_codepoint.d.ts
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/decode_codepoint.d.ts.map
--rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/decode_codepoint.js
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/decode_codepoint.js.map
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/encode.d.ts
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/encode.d.ts.map
--rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/encode.js
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/encode.js.map
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/escape.d.ts
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/escape.d.ts.map
--rw-r--r--   0        0        0     4311 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/escape.js
--rw-r--r--   0        0        0     2874 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/escape.js.map
--rw-r--r--   0        0        0     3332 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/index.d.ts
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/index.d.ts.map
--rw-r--r--   0        0        0     7144 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/index.js
--rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/index.js.map
--rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/esm/decode.d.ts
--rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/esm/decode.d.ts.map
--rw-r--r--   0        0        0    19810 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/esm/decode.js
--rw-r--r--   0        0        0    11475 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/esm/decode.js.map
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/esm/decode_codepoint.d.ts
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/esm/decode_codepoint.d.ts.map
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/esm/decode_codepoint.js
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/esm/decode_codepoint.js.map
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/esm/encode.d.ts
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/esm/encode.d.ts.map
--rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/esm/encode.js
--rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/esm/encode.js.map
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/esm/escape.d.ts
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/esm/escape.d.ts.map
--rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/esm/escape.js
--rw-r--r--   0        0        0     2897 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/esm/escape.js.map
--rw-r--r--   0        0        0     3332 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/esm/index.d.ts
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/esm/index.d.ts.map
--rw-r--r--   0        0        0     4057 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/esm/index.js
--rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/esm/index.js.map
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/esm/package.json
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/esm/generated/decode-data-html.d.ts
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/esm/generated/decode-data-html.d.ts.map
--rw-r--r--   0        0        0    47724 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/esm/generated/decode-data-html.js
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/esm/generated/decode-data-html.js.map
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/esm/generated/decode-data-xml.d.ts
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/esm/generated/decode-data-xml.d.ts.map
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/esm/generated/decode-data-xml.js
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/esm/generated/decode-data-xml.js.map
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/esm/generated/encode-html.d.ts
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/esm/generated/encode-html.d.ts.map
--rw-r--r--   0        0        0    27039 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/esm/generated/encode-html.js
--rw-r--r--   0        0        0    48225 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/esm/generated/encode-html.js.map
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/generated/decode-data-html.d.ts
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/generated/decode-data-html.d.ts.map
--rw-r--r--   0        0        0    47822 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/generated/decode-data-html.js
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/generated/decode-data-html.js.map
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/generated/decode-data-xml.d.ts
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/generated/decode-data-xml.d.ts.map
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/generated/decode-data-xml.js
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/generated/decode-data-xml.js.map
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/generated/encode-html.d.ts
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/generated/encode-html.d.ts.map
--rw-r--r--   0        0        0    27119 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/generated/encode-html.js
--rw-r--r--   0        0        0    48228 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/entities/lib/generated/encode-html.js.map
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/estree-walker/CHANGELOG.md
--rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/estree-walker/LICENSE
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/estree-walker/README.md
--rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/estree-walker/package.json
--rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/estree-walker/src/async.js
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/estree-walker/src/index.js
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/estree-walker/src/package.json
--rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/estree-walker/src/sync.js
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/estree-walker/src/walker.js
--rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/estree-walker/types/async.d.ts
--rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/estree-walker/types/index.d.ts
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/estree-walker/types/sync.d.ts
--rw-r--r--   0        0        0    15666 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/estree-walker/types/tsconfig.tsbuildinfo
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/estree-walker/types/walker.d.ts
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/magic-string/LICENSE
--rw-r--r--   0        0        0    12117 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/magic-string/README.md
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/magic-string/package.json
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/nanoid/LICENSE
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/nanoid/README.md
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/nanoid/index.browser.cjs
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/nanoid/index.browser.js
--rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/nanoid/index.cjs
--rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/nanoid/index.d.cts
--rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/nanoid/index.d.ts
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/nanoid/index.js
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/nanoid/nanoid.js
--rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/nanoid/package.json
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/nanoid/async/index.browser.cjs
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/nanoid/async/index.browser.js
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/nanoid/async/index.cjs
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/nanoid/async/index.d.ts
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/nanoid/async/index.js
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/nanoid/async/index.native.js
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/nanoid/async/package.json
--rwxr-xr-x   0        0        0     1129 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/nanoid/bin/nanoid.cjs
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/nanoid/non-secure/index.cjs
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/nanoid/non-secure/index.d.ts
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/nanoid/non-secure/index.js
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/nanoid/non-secure/package.json
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/nanoid/url-alphabet/index.cjs
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/nanoid/url-alphabet/index.js
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/nanoid/url-alphabet/package.json
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/picocolors/LICENSE
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/picocolors/README.md
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/picocolors/package.json
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/picocolors/picocolors.browser.js
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/picocolors/picocolors.d.ts
--rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/picocolors/picocolors.js
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/picocolors/types.ts
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/postcss/LICENSE
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/postcss/README.md
--rwxr-xr-x   0        0        0     2496 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/postcss/package.json
--rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/postcss/lib/at-rule.d.ts
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/postcss/lib/at-rule.js
--rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/postcss/lib/comment.d.ts
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/postcss/lib/comment.js
--rw-r--r--   0        0        0    13538 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/postcss/lib/container.d.ts
--rw-r--r--   0        0        0    10566 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/postcss/lib/container.js
--rw-r--r--   0        0        0     6503 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/postcss/lib/css-syntax-error.d.ts
--rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/postcss/lib/css-syntax-error.js
--rw-r--r--   0        0        0     3815 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/postcss/lib/declaration.d.ts
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/postcss/lib/declaration.js
--rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/postcss/lib/document.d.ts
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/postcss/lib/document.js
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/postcss/lib/fromJSON.d.ts
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/postcss/lib/fromJSON.js
--rw-r--r--   0        0        0     4424 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/postcss/lib/input.d.ts
--rw-r--r--   0        0        0     6190 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/postcss/lib/input.js
--rw-r--r--   0        0        0     5007 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/postcss/lib/lazy-result.d.ts
--rw-r--r--   0        0        0    13562 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/postcss/lib/lazy-result.js
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/postcss/lib/list.d.ts
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/postcss/lib/list.js
--rw-r--r--   0        0        0     9725 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/postcss/lib/map-generator.js
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/postcss/lib/no-work-result.d.ts
--rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/postcss/lib/no-work-result.js
--rw-r--r--   0        0        0    13874 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/postcss/lib/node.d.ts
--rw-r--r--   0        0        0     8753 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/postcss/lib/node.js
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/postcss/lib/parse.d.ts
--rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/postcss/lib/parse.js
--rw-r--r--   0        0        0    14725 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/postcss/lib/parser.js
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/postcss/lib/postcss.d.mts
--rw-r--r--   0        0        0    11255 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/postcss/lib/postcss.d.ts
--rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/postcss/lib/postcss.js
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/postcss/lib/postcss.mjs
--rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/postcss/lib/previous-map.d.ts
--rw-r--r--   0        0        0     3923 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/postcss/lib/previous-map.js
--rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/postcss/lib/processor.d.ts
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/postcss/lib/processor.js
--rw-r--r--   0        0        0     4417 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/postcss/lib/result.d.ts
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/postcss/lib/result.js
--rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/postcss/lib/root.d.ts
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/postcss/lib/root.js
--rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/postcss/lib/rule.d.ts
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/postcss/lib/rule.js
--rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/postcss/lib/stringifier.d.ts
--rw-r--r--   0        0        0     8220 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/postcss/lib/stringifier.js
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/postcss/lib/stringify.d.ts
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/postcss/lib/stringify.js
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/postcss/lib/symbols.js
--rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/postcss/lib/terminal-highlight.js
--rw-r--r--   0        0        0     6538 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/postcss/lib/tokenize.js
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/postcss/lib/warn-once.js
--rw-r--r--   0        0        0     2994 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/postcss/lib/warning.d.ts
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/postcss/lib/warning.js
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/source-map-js/LICENSE
--rw-r--r--   0        0        0    26040 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/source-map-js/README.md
--rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/source-map-js/package.json
--rw-r--r--   0        0        0     3854 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/source-map-js/source-map.d.ts
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/source-map-js/source-map.js
--rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/source-map-js/lib/array-set.js
--rw-r--r--   0        0        0     4714 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/source-map-js/lib/base64-vlq.js
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/source-map-js/lib/base64.js
--rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/source-map-js/lib/binary-search.js
--rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/source-map-js/lib/mapping-list.js
--rw-r--r--   0        0        0     4068 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/source-map-js/lib/quick-sort.js
--rw-r--r--   0        0        0    41500 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/source-map-js/lib/source-map-consumer.js
--rw-r--r--   0        0        0    14933 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/source-map-js/lib/source-map-generator.js
--rw-r--r--   0        0        0    13808 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/source-map-js/lib/source-node.js
--rw-r--r--   0        0        0    15403 2020-02-02 00:00:00.000000 checol-0.1.0/node_modules/source-map-js/lib/util.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 checol-0.1.0/src/checol/__init__.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 checol-0.1.0/src/checol/__main__.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 checol-0.1.0/src/checol/gpt.py
--rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 checol-0.1.0/src/checol/main.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 checol-0.1.0/src/checol/vcs.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 checol-0.1.0/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 checol-0.1.0/LICENSE
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 checol-0.1.0/README.md
--rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 checol-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 checol-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 checol-0.2.1/.python-version
+-rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 checol-0.2.1/checol-0.1.0-py3-none-any.whl
+-rw-r--r--   0        0        0     6035 2020-02-02 00:00:00.000000 checol-0.2.1/package-lock.json
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 checol-0.2.1/package.json
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 checol-0.2.1/requirements-dev.lock
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 checol-0.2.1/requirements.lock
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 checol-0.2.1/.github/workflows/rye-lint.yml
+-rw-r--r--   0        0        0     5947 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/.package-lock.json
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/.bin/nanoid -> ../nanoid/bin/nanoid.cjs
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/.bin/parser -> ../@babel/parser/bin/babel-parser.js
+-rw-r--r--   0        0        0    38238 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/@babel/parser/CHANGELOG.md
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/@babel/parser/LICENSE
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/@babel/parser/README.md
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/@babel/parser/index.cjs
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/@babel/parser/package.json
+-rwxr-xr-x   0        0        0      328 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/@babel/parser/bin/babel-parser.js
+-rw-r--r--   0        0        0   484739 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/@babel/parser/lib/index.js
+-rw-r--r--   0        0        0  1349600 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/@babel/parser/lib/index.js.map
+-rw-r--r--   0        0        0     7547 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/@babel/parser/typings/babel-parser.d.ts
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/@jridgewell/sourcemap-codec/LICENSE
+-rw-r--r--   0        0        0     6893 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/@jridgewell/sourcemap-codec/README.md
+-rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/@jridgewell/sourcemap-codec/package.json
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/@vue/compiler-core/LICENSE
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/@vue/compiler-core/README.md
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/@vue/compiler-core/index.js
+-rw-r--r--   0        0        0     1386 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/@vue/compiler-core/package.json
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/@vue/compiler-dom/LICENSE
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/@vue/compiler-dom/README.md
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/@vue/compiler-dom/index.js
+-rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/@vue/compiler-dom/package.json
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/@vue/compiler-sfc/LICENSE
+-rw-r--r--   0        0        0     4444 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/@vue/compiler-sfc/README.md
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/@vue/compiler-sfc/package.json
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/@vue/compiler-ssr/LICENSE
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/@vue/compiler-ssr/README.md
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/@vue/compiler-ssr/package.json
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/@vue/shared/LICENSE
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/@vue/shared/README.md
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/@vue/shared/index.js
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/@vue/shared/package.json
+-rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/LICENSE
+-rw-r--r--   0        0        0     2883 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/package.json
+-rw-r--r--   0        0        0     5074 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/readme.md
+-rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/decode.d.ts
+-rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/decode.d.ts.map
+-rw-r--r--   0        0        0    22611 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/decode.js
+-rw-r--r--   0        0        0    11591 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/decode.js.map
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/decode_codepoint.d.ts
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/decode_codepoint.d.ts.map
+-rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/decode_codepoint.js
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/decode_codepoint.js.map
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/encode.d.ts
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/encode.d.ts.map
+-rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/encode.js
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/encode.js.map
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/escape.d.ts
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/escape.d.ts.map
+-rw-r--r--   0        0        0     4311 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/escape.js
+-rw-r--r--   0        0        0     2874 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/escape.js.map
+-rw-r--r--   0        0        0     3332 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/index.d.ts
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/index.d.ts.map
+-rw-r--r--   0        0        0     7144 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/index.js
+-rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/index.js.map
+-rw-r--r--   0        0        0     8102 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/esm/decode.d.ts
+-rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/esm/decode.d.ts.map
+-rw-r--r--   0        0        0    19810 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/esm/decode.js
+-rw-r--r--   0        0        0    11475 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/esm/decode.js.map
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/esm/decode_codepoint.d.ts
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/esm/decode_codepoint.d.ts.map
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/esm/decode_codepoint.js
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/esm/decode_codepoint.js.map
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/esm/encode.d.ts
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/esm/encode.d.ts.map
+-rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/esm/encode.js
+-rw-r--r--   0        0        0     1865 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/esm/encode.js.map
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/esm/escape.d.ts
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/esm/escape.d.ts.map
+-rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/esm/escape.js
+-rw-r--r--   0        0        0     2897 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/esm/escape.js.map
+-rw-r--r--   0        0        0     3332 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/esm/index.d.ts
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/esm/index.d.ts.map
+-rw-r--r--   0        0        0     4057 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/esm/index.js
+-rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/esm/index.js.map
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/esm/package.json
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/esm/generated/decode-data-html.d.ts
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/esm/generated/decode-data-html.d.ts.map
+-rw-r--r--   0        0        0    47724 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/esm/generated/decode-data-html.js
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/esm/generated/decode-data-html.js.map
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/esm/generated/decode-data-xml.d.ts
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/esm/generated/decode-data-xml.d.ts.map
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/esm/generated/decode-data-xml.js
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/esm/generated/decode-data-xml.js.map
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/esm/generated/encode-html.d.ts
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/esm/generated/encode-html.d.ts.map
+-rw-r--r--   0        0        0    27039 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/esm/generated/encode-html.js
+-rw-r--r--   0        0        0    48225 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/esm/generated/encode-html.js.map
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/generated/decode-data-html.d.ts
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/generated/decode-data-html.d.ts.map
+-rw-r--r--   0        0        0    47822 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/generated/decode-data-html.js
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/generated/decode-data-html.js.map
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/generated/decode-data-xml.d.ts
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/generated/decode-data-xml.d.ts.map
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/generated/decode-data-xml.js
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/generated/decode-data-xml.js.map
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/generated/encode-html.d.ts
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/generated/encode-html.d.ts.map
+-rw-r--r--   0        0        0    27119 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/generated/encode-html.js
+-rw-r--r--   0        0        0    48228 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/entities/lib/generated/encode-html.js.map
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/estree-walker/CHANGELOG.md
+-rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/estree-walker/LICENSE
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/estree-walker/README.md
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/estree-walker/package.json
+-rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/estree-walker/src/async.js
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/estree-walker/src/index.js
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/estree-walker/src/package.json
+-rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/estree-walker/src/sync.js
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/estree-walker/src/walker.js
+-rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/estree-walker/types/async.d.ts
+-rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/estree-walker/types/index.d.ts
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/estree-walker/types/sync.d.ts
+-rw-r--r--   0        0        0    15666 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/estree-walker/types/tsconfig.tsbuildinfo
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/estree-walker/types/walker.d.ts
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/magic-string/LICENSE
+-rw-r--r--   0        0        0    12117 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/magic-string/README.md
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/magic-string/package.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/nanoid/LICENSE
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/nanoid/README.md
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/nanoid/index.browser.cjs
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/nanoid/index.browser.js
+-rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/nanoid/index.cjs
+-rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/nanoid/index.d.cts
+-rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/nanoid/index.d.ts
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/nanoid/index.js
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/nanoid/nanoid.js
+-rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/nanoid/package.json
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/nanoid/async/index.browser.cjs
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/nanoid/async/index.browser.js
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/nanoid/async/index.cjs
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/nanoid/async/index.d.ts
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/nanoid/async/index.js
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/nanoid/async/index.native.js
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/nanoid/async/package.json
+-rwxr-xr-x   0        0        0     1129 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/nanoid/bin/nanoid.cjs
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/nanoid/non-secure/index.cjs
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/nanoid/non-secure/index.d.ts
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/nanoid/non-secure/index.js
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/nanoid/non-secure/package.json
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/nanoid/url-alphabet/index.cjs
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/nanoid/url-alphabet/index.js
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/nanoid/url-alphabet/package.json
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/picocolors/LICENSE
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/picocolors/README.md
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/picocolors/package.json
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/picocolors/picocolors.browser.js
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/picocolors/picocolors.d.ts
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/picocolors/picocolors.js
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/picocolors/types.ts
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/postcss/LICENSE
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/postcss/README.md
+-rwxr-xr-x   0        0        0     2496 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/postcss/package.json
+-rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/postcss/lib/at-rule.d.ts
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/postcss/lib/at-rule.js
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/postcss/lib/comment.d.ts
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/postcss/lib/comment.js
+-rw-r--r--   0        0        0    13538 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/postcss/lib/container.d.ts
+-rw-r--r--   0        0        0    10566 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/postcss/lib/container.js
+-rw-r--r--   0        0        0     6503 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/postcss/lib/css-syntax-error.d.ts
+-rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/postcss/lib/css-syntax-error.js
+-rw-r--r--   0        0        0     3815 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/postcss/lib/declaration.d.ts
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/postcss/lib/declaration.js
+-rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/postcss/lib/document.d.ts
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/postcss/lib/document.js
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/postcss/lib/fromJSON.d.ts
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/postcss/lib/fromJSON.js
+-rw-r--r--   0        0        0     4424 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/postcss/lib/input.d.ts
+-rw-r--r--   0        0        0     6190 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/postcss/lib/input.js
+-rw-r--r--   0        0        0     5007 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/postcss/lib/lazy-result.d.ts
+-rw-r--r--   0        0        0    13562 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/postcss/lib/lazy-result.js
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/postcss/lib/list.d.ts
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/postcss/lib/list.js
+-rw-r--r--   0        0        0     9725 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/postcss/lib/map-generator.js
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/postcss/lib/no-work-result.d.ts
+-rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/postcss/lib/no-work-result.js
+-rw-r--r--   0        0        0    13874 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/postcss/lib/node.d.ts
+-rw-r--r--   0        0        0     8753 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/postcss/lib/node.js
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/postcss/lib/parse.d.ts
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/postcss/lib/parse.js
+-rw-r--r--   0        0        0    14725 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/postcss/lib/parser.js
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/postcss/lib/postcss.d.mts
+-rw-r--r--   0        0        0    11255 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/postcss/lib/postcss.d.ts
+-rw-r--r--   0        0        0     2898 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/postcss/lib/postcss.js
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/postcss/lib/postcss.mjs
+-rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/postcss/lib/previous-map.d.ts
+-rw-r--r--   0        0        0     3923 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/postcss/lib/previous-map.js
+-rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/postcss/lib/processor.d.ts
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/postcss/lib/processor.js
+-rw-r--r--   0        0        0     4417 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/postcss/lib/result.d.ts
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/postcss/lib/result.js
+-rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/postcss/lib/root.d.ts
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/postcss/lib/root.js
+-rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/postcss/lib/rule.d.ts
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/postcss/lib/rule.js
+-rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/postcss/lib/stringifier.d.ts
+-rw-r--r--   0        0        0     8220 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/postcss/lib/stringifier.js
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/postcss/lib/stringify.d.ts
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/postcss/lib/stringify.js
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/postcss/lib/symbols.js
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/postcss/lib/terminal-highlight.js
+-rw-r--r--   0        0        0     6538 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/postcss/lib/tokenize.js
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/postcss/lib/warn-once.js
+-rw-r--r--   0        0        0     2994 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/postcss/lib/warning.d.ts
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/postcss/lib/warning.js
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/source-map-js/LICENSE
+-rw-r--r--   0        0        0    26040 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/source-map-js/README.md
+-rw-r--r--   0        0        0     2548 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/source-map-js/package.json
+-rw-r--r--   0        0        0     3854 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/source-map-js/source-map.d.ts
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/source-map-js/source-map.js
+-rw-r--r--   0        0        0     3197 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/source-map-js/lib/array-set.js
+-rw-r--r--   0        0        0     4714 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/source-map-js/lib/base64-vlq.js
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/source-map-js/lib/base64.js
+-rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/source-map-js/lib/binary-search.js
+-rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/source-map-js/lib/mapping-list.js
+-rw-r--r--   0        0        0     4068 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/source-map-js/lib/quick-sort.js
+-rw-r--r--   0        0        0    41500 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/source-map-js/lib/source-map-consumer.js
+-rw-r--r--   0        0        0    14933 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/source-map-js/lib/source-map-generator.js
+-rw-r--r--   0        0        0    13808 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/source-map-js/lib/source-node.js
+-rw-r--r--   0        0        0    15403 2020-02-02 00:00:00.000000 checol-0.2.1/node_modules/source-map-js/lib/util.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 checol-0.2.1/src/checol/__init__.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 checol-0.2.1/src/checol/__main__.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 checol-0.2.1/src/checol/gpt.py
+-rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 checol-0.2.1/src/checol/main.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 checol-0.2.1/src/checol/vcs.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 checol-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 checol-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 checol-0.2.1/README.md
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 checol-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 checol-0.2.1/PKG-INFO
```

### Comparing `checol-0.1.0/checol-0.1.0-py3-none-any.whl` & `checol-0.2.1/checol-0.1.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/package-lock.json` & `checol-0.2.1/package-lock.json`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/requirements-dev.lock` & `checol-0.2.1/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/requirements.lock` & `checol-0.2.1/requirements.lock`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/.package-lock.json` & `checol-0.2.1/node_modules/.package-lock.json`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/@babel/parser/CHANGELOG.md` & `checol-0.2.1/node_modules/@babel/parser/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/@babel/parser/LICENSE` & `checol-0.2.1/node_modules/@babel/parser/LICENSE`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/@babel/parser/package.json` & `checol-0.2.1/node_modules/@babel/parser/package.json`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/@babel/parser/lib/index.js` & `checol-0.2.1/node_modules/@babel/parser/lib/index.js`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/@babel/parser/lib/index.js.map` & `checol-0.2.1/node_modules/@babel/parser/lib/index.js.map`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/@babel/parser/typings/babel-parser.d.ts` & `checol-0.2.1/node_modules/@babel/parser/typings/babel-parser.d.ts`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/@jridgewell/sourcemap-codec/LICENSE` & `checol-0.2.1/node_modules/@jridgewell/sourcemap-codec/LICENSE`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/@jridgewell/sourcemap-codec/README.md` & `checol-0.2.1/node_modules/@jridgewell/sourcemap-codec/README.md`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/@jridgewell/sourcemap-codec/package.json` & `checol-0.2.1/node_modules/@jridgewell/sourcemap-codec/package.json`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/@vue/compiler-core/LICENSE` & `checol-0.2.1/node_modules/@vue/compiler-core/LICENSE`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/@vue/compiler-core/package.json` & `checol-0.2.1/node_modules/@vue/compiler-core/package.json`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/@vue/compiler-dom/LICENSE` & `checol-0.2.1/node_modules/@vue/compiler-dom/LICENSE`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/@vue/compiler-dom/package.json` & `checol-0.2.1/node_modules/@vue/compiler-dom/package.json`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/@vue/compiler-sfc/LICENSE` & `checol-0.2.1/node_modules/@vue/compiler-sfc/LICENSE`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/@vue/compiler-sfc/README.md` & `checol-0.2.1/node_modules/@vue/compiler-sfc/README.md`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/@vue/compiler-sfc/package.json` & `checol-0.2.1/node_modules/@vue/compiler-sfc/package.json`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/@vue/compiler-ssr/LICENSE` & `checol-0.2.1/node_modules/@vue/compiler-ssr/LICENSE`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/@vue/compiler-ssr/package.json` & `checol-0.2.1/node_modules/@vue/compiler-ssr/package.json`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/@vue/shared/LICENSE` & `checol-0.2.1/node_modules/@vue/shared/LICENSE`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/@vue/shared/package.json` & `checol-0.2.1/node_modules/@vue/shared/package.json`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/entities/LICENSE` & `checol-0.2.1/node_modules/entities/LICENSE`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/entities/package.json` & `checol-0.2.1/node_modules/entities/package.json`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/entities/readme.md` & `checol-0.2.1/node_modules/entities/readme.md`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/entities/lib/decode.d.ts` & `checol-0.2.1/node_modules/entities/lib/decode.d.ts`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/entities/lib/decode.d.ts.map` & `checol-0.2.1/node_modules/entities/lib/decode.d.ts.map`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/entities/lib/decode.js` & `checol-0.2.1/node_modules/entities/lib/decode.js`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/entities/lib/decode.js.map` & `checol-0.2.1/node_modules/entities/lib/decode.js.map`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/entities/lib/decode_codepoint.d.ts` & `checol-0.2.1/node_modules/entities/lib/decode_codepoint.d.ts`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/entities/lib/decode_codepoint.js` & `checol-0.2.1/node_modules/entities/lib/decode_codepoint.js`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/entities/lib/decode_codepoint.js.map` & `checol-0.2.1/node_modules/entities/lib/decode_codepoint.js.map`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/entities/lib/encode.d.ts` & `checol-0.2.1/node_modules/entities/lib/encode.d.ts`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/entities/lib/encode.js` & `checol-0.2.1/node_modules/entities/lib/encode.js`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/entities/lib/encode.js.map` & `checol-0.2.1/node_modules/entities/lib/encode.js.map`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/entities/lib/escape.d.ts` & `checol-0.2.1/node_modules/entities/lib/escape.d.ts`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/entities/lib/escape.d.ts.map` & `checol-0.2.1/node_modules/entities/lib/escape.d.ts.map`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/entities/lib/escape.js` & `checol-0.2.1/node_modules/entities/lib/escape.js`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/entities/lib/escape.js.map` & `checol-0.2.1/node_modules/entities/lib/escape.js.map`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/entities/lib/index.d.ts` & `checol-0.2.1/node_modules/entities/lib/index.d.ts`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/entities/lib/index.d.ts.map` & `checol-0.2.1/node_modules/entities/lib/index.d.ts.map`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/entities/lib/index.js` & `checol-0.2.1/node_modules/entities/lib/index.js`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/entities/lib/index.js.map` & `checol-0.2.1/node_modules/entities/lib/index.js.map`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/entities/lib/esm/decode.d.ts` & `checol-0.2.1/node_modules/entities/lib/esm/decode.d.ts`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/entities/lib/esm/decode.d.ts.map` & `checol-0.2.1/node_modules/entities/lib/esm/decode.d.ts.map`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/entities/lib/esm/decode.js` & `checol-0.2.1/node_modules/entities/lib/esm/decode.js`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/entities/lib/esm/decode.js.map` & `checol-0.2.1/node_modules/entities/lib/esm/decode.js.map`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/entities/lib/esm/decode_codepoint.d.ts` & `checol-0.2.1/node_modules/entities/lib/esm/decode_codepoint.d.ts`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/entities/lib/esm/decode_codepoint.js` & `checol-0.2.1/node_modules/entities/lib/esm/decode_codepoint.js`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/entities/lib/esm/decode_codepoint.js.map` & `checol-0.2.1/node_modules/entities/lib/esm/decode_codepoint.js.map`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/entities/lib/esm/encode.d.ts` & `checol-0.2.1/node_modules/entities/lib/esm/encode.d.ts`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/entities/lib/esm/encode.js` & `checol-0.2.1/node_modules/entities/lib/esm/encode.js`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/entities/lib/esm/encode.js.map` & `checol-0.2.1/node_modules/entities/lib/esm/encode.js.map`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/entities/lib/esm/escape.d.ts` & `checol-0.2.1/node_modules/entities/lib/esm/escape.d.ts`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/entities/lib/esm/escape.d.ts.map` & `checol-0.2.1/node_modules/entities/lib/esm/escape.d.ts.map`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/entities/lib/esm/escape.js` & `checol-0.2.1/node_modules/entities/lib/esm/escape.js`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/entities/lib/esm/escape.js.map` & `checol-0.2.1/node_modules/entities/lib/esm/escape.js.map`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/entities/lib/esm/index.d.ts` & `checol-0.2.1/node_modules/entities/lib/esm/index.d.ts`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/entities/lib/esm/index.d.ts.map` & `checol-0.2.1/node_modules/entities/lib/esm/index.d.ts.map`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/entities/lib/esm/index.js` & `checol-0.2.1/node_modules/entities/lib/esm/index.js`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/entities/lib/esm/index.js.map` & `checol-0.2.1/node_modules/entities/lib/esm/index.js.map`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/entities/lib/esm/generated/decode-data-html.js` & `checol-0.2.1/node_modules/entities/lib/esm/generated/decode-data-html.js`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/entities/lib/esm/generated/encode-html.js` & `checol-0.2.1/node_modules/entities/lib/esm/generated/encode-html.js`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/entities/lib/esm/generated/encode-html.js.map` & `checol-0.2.1/node_modules/entities/lib/esm/generated/encode-html.js.map`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/entities/lib/generated/decode-data-html.js` & `checol-0.2.1/node_modules/entities/lib/generated/decode-data-html.js`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/entities/lib/generated/encode-html.js` & `checol-0.2.1/node_modules/entities/lib/generated/encode-html.js`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/entities/lib/generated/encode-html.js.map` & `checol-0.2.1/node_modules/entities/lib/generated/encode-html.js.map`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/estree-walker/CHANGELOG.md` & `checol-0.2.1/node_modules/estree-walker/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/estree-walker/LICENSE` & `checol-0.2.1/node_modules/estree-walker/LICENSE`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/estree-walker/README.md` & `checol-0.2.1/node_modules/estree-walker/README.md`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/estree-walker/package.json` & `checol-0.2.1/node_modules/estree-walker/package.json`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/estree-walker/src/async.js` & `checol-0.2.1/node_modules/estree-walker/src/async.js`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/estree-walker/src/index.js` & `checol-0.2.1/node_modules/estree-walker/src/index.js`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/estree-walker/src/sync.js` & `checol-0.2.1/node_modules/estree-walker/src/sync.js`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/estree-walker/src/walker.js` & `checol-0.2.1/node_modules/estree-walker/src/walker.js`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/estree-walker/types/async.d.ts` & `checol-0.2.1/node_modules/estree-walker/types/async.d.ts`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/estree-walker/types/index.d.ts` & `checol-0.2.1/node_modules/estree-walker/types/index.d.ts`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/estree-walker/types/sync.d.ts` & `checol-0.2.1/node_modules/estree-walker/types/sync.d.ts`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/estree-walker/types/tsconfig.tsbuildinfo` & `checol-0.2.1/node_modules/estree-walker/types/tsconfig.tsbuildinfo`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/estree-walker/types/walker.d.ts` & `checol-0.2.1/node_modules/estree-walker/types/walker.d.ts`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/magic-string/LICENSE` & `checol-0.2.1/node_modules/magic-string/LICENSE`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/magic-string/README.md` & `checol-0.2.1/node_modules/magic-string/README.md`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/magic-string/package.json` & `checol-0.2.1/node_modules/magic-string/package.json`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/nanoid/LICENSE` & `checol-0.2.1/node_modules/nanoid/LICENSE`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/nanoid/README.md` & `checol-0.2.1/node_modules/nanoid/README.md`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/nanoid/index.browser.cjs` & `checol-0.2.1/node_modules/nanoid/index.browser.cjs`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/nanoid/index.browser.js` & `checol-0.2.1/node_modules/nanoid/index.browser.js`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/nanoid/index.cjs` & `checol-0.2.1/node_modules/nanoid/index.cjs`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/nanoid/index.d.cts` & `checol-0.2.1/node_modules/nanoid/index.d.cts`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/nanoid/index.d.ts` & `checol-0.2.1/node_modules/nanoid/index.d.ts`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/nanoid/index.js` & `checol-0.2.1/node_modules/nanoid/index.js`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/nanoid/package.json` & `checol-0.2.1/node_modules/nanoid/package.json`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/nanoid/async/index.browser.cjs` & `checol-0.2.1/node_modules/nanoid/async/index.browser.cjs`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/nanoid/async/index.browser.js` & `checol-0.2.1/node_modules/nanoid/async/index.browser.js`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/nanoid/async/index.cjs` & `checol-0.2.1/node_modules/nanoid/async/index.cjs`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/nanoid/async/index.d.ts` & `checol-0.2.1/node_modules/nanoid/async/index.d.ts`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/nanoid/async/index.js` & `checol-0.2.1/node_modules/nanoid/async/index.js`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/nanoid/async/index.native.js` & `checol-0.2.1/node_modules/nanoid/async/index.native.js`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/nanoid/bin/nanoid.cjs` & `checol-0.2.1/node_modules/nanoid/bin/nanoid.cjs`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/nanoid/non-secure/index.d.ts` & `checol-0.2.1/node_modules/nanoid/non-secure/index.d.ts`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/picocolors/LICENSE` & `checol-0.2.1/node_modules/picocolors/LICENSE`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/picocolors/README.md` & `checol-0.2.1/node_modules/picocolors/README.md`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/picocolors/package.json` & `checol-0.2.1/node_modules/picocolors/package.json`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/picocolors/picocolors.js` & `checol-0.2.1/node_modules/picocolors/picocolors.js`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/picocolors/types.ts` & `checol-0.2.1/node_modules/picocolors/types.ts`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/postcss/LICENSE` & `checol-0.2.1/node_modules/postcss/LICENSE`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/postcss/README.md` & `checol-0.2.1/node_modules/postcss/README.md`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/postcss/package.json` & `checol-0.2.1/node_modules/postcss/package.json`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/postcss/lib/at-rule.d.ts` & `checol-0.2.1/node_modules/postcss/lib/at-rule.d.ts`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/postcss/lib/comment.d.ts` & `checol-0.2.1/node_modules/postcss/lib/comment.d.ts`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/postcss/lib/container.d.ts` & `checol-0.2.1/node_modules/postcss/lib/container.d.ts`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/postcss/lib/container.js` & `checol-0.2.1/node_modules/postcss/lib/container.js`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/postcss/lib/css-syntax-error.d.ts` & `checol-0.2.1/node_modules/postcss/lib/css-syntax-error.d.ts`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/postcss/lib/css-syntax-error.js` & `checol-0.2.1/node_modules/postcss/lib/css-syntax-error.js`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/postcss/lib/declaration.d.ts` & `checol-0.2.1/node_modules/postcss/lib/declaration.d.ts`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/postcss/lib/document.d.ts` & `checol-0.2.1/node_modules/postcss/lib/document.d.ts`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/postcss/lib/document.js` & `checol-0.2.1/node_modules/postcss/lib/document.js`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/postcss/lib/fromJSON.js` & `checol-0.2.1/node_modules/postcss/lib/fromJSON.js`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/postcss/lib/input.d.ts` & `checol-0.2.1/node_modules/postcss/lib/input.d.ts`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/postcss/lib/input.js` & `checol-0.2.1/node_modules/postcss/lib/input.js`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/postcss/lib/lazy-result.d.ts` & `checol-0.2.1/node_modules/postcss/lib/lazy-result.d.ts`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/postcss/lib/lazy-result.js` & `checol-0.2.1/node_modules/postcss/lib/lazy-result.js`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/postcss/lib/list.d.ts` & `checol-0.2.1/node_modules/postcss/lib/list.d.ts`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/postcss/lib/list.js` & `checol-0.2.1/node_modules/postcss/lib/list.js`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/postcss/lib/map-generator.js` & `checol-0.2.1/node_modules/postcss/lib/map-generator.js`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/postcss/lib/no-work-result.d.ts` & `checol-0.2.1/node_modules/postcss/lib/no-work-result.d.ts`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/postcss/lib/no-work-result.js` & `checol-0.2.1/node_modules/postcss/lib/no-work-result.js`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/postcss/lib/node.d.ts` & `checol-0.2.1/node_modules/postcss/lib/node.d.ts`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/postcss/lib/node.js` & `checol-0.2.1/node_modules/postcss/lib/node.js`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/postcss/lib/parse.js` & `checol-0.2.1/node_modules/postcss/lib/parse.js`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/postcss/lib/parser.js` & `checol-0.2.1/node_modules/postcss/lib/parser.js`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/postcss/lib/postcss.d.mts` & `checol-0.2.1/node_modules/postcss/lib/postcss.d.mts`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/postcss/lib/postcss.d.ts` & `checol-0.2.1/node_modules/postcss/lib/postcss.d.ts`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/postcss/lib/postcss.js` & `checol-0.2.1/node_modules/postcss/lib/postcss.js`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/postcss/lib/postcss.mjs` & `checol-0.2.1/node_modules/postcss/lib/postcss.mjs`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/postcss/lib/previous-map.d.ts` & `checol-0.2.1/node_modules/postcss/lib/previous-map.d.ts`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/postcss/lib/previous-map.js` & `checol-0.2.1/node_modules/postcss/lib/previous-map.js`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/postcss/lib/processor.d.ts` & `checol-0.2.1/node_modules/postcss/lib/processor.d.ts`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/postcss/lib/processor.js` & `checol-0.2.1/node_modules/postcss/lib/processor.js`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/postcss/lib/result.d.ts` & `checol-0.2.1/node_modules/postcss/lib/result.d.ts`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/postcss/lib/result.js` & `checol-0.2.1/node_modules/postcss/lib/result.js`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/postcss/lib/root.d.ts` & `checol-0.2.1/node_modules/postcss/lib/root.d.ts`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/postcss/lib/root.js` & `checol-0.2.1/node_modules/postcss/lib/root.js`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/postcss/lib/rule.d.ts` & `checol-0.2.1/node_modules/postcss/lib/rule.d.ts`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/postcss/lib/rule.js` & `checol-0.2.1/node_modules/postcss/lib/rule.js`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/postcss/lib/stringifier.d.ts` & `checol-0.2.1/node_modules/postcss/lib/stringifier.d.ts`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/postcss/lib/stringifier.js` & `checol-0.2.1/node_modules/postcss/lib/stringifier.js`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/postcss/lib/terminal-highlight.js` & `checol-0.2.1/node_modules/postcss/lib/terminal-highlight.js`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/postcss/lib/tokenize.js` & `checol-0.2.1/node_modules/postcss/lib/tokenize.js`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/postcss/lib/warning.d.ts` & `checol-0.2.1/node_modules/postcss/lib/warning.d.ts`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/postcss/lib/warning.js` & `checol-0.2.1/node_modules/postcss/lib/warning.js`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/source-map-js/LICENSE` & `checol-0.2.1/node_modules/source-map-js/LICENSE`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/source-map-js/README.md` & `checol-0.2.1/node_modules/source-map-js/README.md`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/source-map-js/package.json` & `checol-0.2.1/node_modules/source-map-js/package.json`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/source-map-js/source-map.d.ts` & `checol-0.2.1/node_modules/source-map-js/source-map.d.ts`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/source-map-js/lib/array-set.js` & `checol-0.2.1/node_modules/source-map-js/lib/array-set.js`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/source-map-js/lib/base64-vlq.js` & `checol-0.2.1/node_modules/source-map-js/lib/base64-vlq.js`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/source-map-js/lib/base64.js` & `checol-0.2.1/node_modules/source-map-js/lib/base64.js`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/source-map-js/lib/binary-search.js` & `checol-0.2.1/node_modules/source-map-js/lib/binary-search.js`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/source-map-js/lib/mapping-list.js` & `checol-0.2.1/node_modules/source-map-js/lib/mapping-list.js`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/source-map-js/lib/quick-sort.js` & `checol-0.2.1/node_modules/source-map-js/lib/quick-sort.js`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/source-map-js/lib/source-map-consumer.js` & `checol-0.2.1/node_modules/source-map-js/lib/source-map-consumer.js`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/source-map-js/lib/source-map-generator.js` & `checol-0.2.1/node_modules/source-map-js/lib/source-map-generator.js`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/source-map-js/lib/source-node.js` & `checol-0.2.1/node_modules/source-map-js/lib/source-node.js`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/node_modules/source-map-js/lib/util.js` & `checol-0.2.1/node_modules/source-map-js/lib/util.js`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/src/checol/gpt.py` & `checol-0.2.1/src/checol/gpt.py`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/src/checol/main.py` & `checol-0.2.1/src/checol/main.py`

 * *Files identical despite different names*

### Comparing `checol-0.1.0/LICENSE` & `checol-0.2.1/LICENSE`

 * *Files identical despite different names*

