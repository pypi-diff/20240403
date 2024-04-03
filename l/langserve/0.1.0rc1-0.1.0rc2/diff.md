# Comparing `tmp/langserve-0.1.0rc1.tar.gz` & `tmp/langserve-0.1.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langserve-0.1.0rc1.tar", max compression
+gzip compressed data, was "langserve-0.1.0rc2.tar", max compression
```

## Comparing `langserve-0.1.0rc1.tar` & `langserve-0.1.0rc2.tar`

### file list

```diff
@@ -1,145 +1,145 @@
--rw-r--r--   0        0        0     3757 2024-04-01 19:51:36.072289 langserve-0.1.0rc1/LICENSE
--rw-r--r--   0        0        0    42394 2024-04-01 19:51:36.072289 langserve-0.1.0rc1/README.md
--rw-r--r--   0        0        0      505 2024-04-01 19:51:36.080289 langserve-0.1.0rc1/langserve/__init__.py
--rw-r--r--   0        0        0    63222 2024-04-01 19:51:36.080289 langserve-0.1.0rc1/langserve/api_handler.py
--rw-r--r--   0        0        0    14240 2024-04-01 19:51:36.080289 langserve-0.1.0rc1/langserve/callbacks.py
--rw-r--r--   0        0        0      436 2024-04-01 19:51:36.080289 langserve-0.1.0rc1/langserve/chat_playground/.eslintrc.cjs
--rw-r--r--   0        0        0      266 2024-04-01 19:51:36.080289 langserve-0.1.0rc1/langserve/chat_playground/.gitignore
--rw-r--r--   0        0        0     1263 2024-04-01 19:51:36.080289 langserve-0.1.0rc1/langserve/chat_playground/README.md
--rw-r--r--   0        0        0    23810 2024-04-01 19:51:36.080289 langserve-0.1.0rc1/langserve/chat_playground/dist/assets/index-434ff580.css
--rw-r--r--   0        0        0   494586 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/dist/assets/index-86d4d9c0.js
--rw-r--r--   0        0        0    40410 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/dist/favicon.ico
--rw-r--r--   0        0        0     1141 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/dist/index.html
--rw-r--r--   0        0        0      981 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/index.html
--rw-r--r--   0        0        0     1526 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/package.json
--rw-r--r--   0        0        0       81 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/postcss.config.js
--rw-r--r--   0        0        0    40410 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/public/favicon.ico
--rw-r--r--   0        0        0     2554 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/src/App.css
--rw-r--r--   0        0        0     2989 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/src/App.tsx
--rw-r--r--   0        0        0      310 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/src/assets/ArrowUp.svg
--rw-r--r--   0        0        0     2626 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/src/assets/ChatIcon.svg
--rw-r--r--   0        0        0      789 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/src/assets/CheckCircleIcon.svg
--rw-r--r--   0        0        0      328 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/src/assets/CheckCircleIcon2.svg
--rw-r--r--   0        0        0      505 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/src/assets/ChevronRight.svg
--rw-r--r--   0        0        0     1153 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/src/assets/CircleSpinIcon.svg
--rw-r--r--   0        0        0      823 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/src/assets/CodeIcon.svg
--rw-r--r--   0        0        0     1328 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/src/assets/CopyIcon.svg
--rw-r--r--   0        0        0     1744 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/src/assets/EmptyState.svg
--rw-r--r--   0        0        0    11000 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/src/assets/LangServeLogo.svg
--rw-r--r--   0        0        0     2350 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/src/assets/PadlockIcon.svg
--rw-r--r--   0        0        0      670 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/src/assets/PlusIcon.svg
--rw-r--r--   0        0        0      400 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/src/assets/RefreshCW.svg
--rw-r--r--   0        0        0     1260 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/src/assets/SendIcon.svg
--rw-r--r--   0        0        0     1831 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/src/assets/ShareIcon.svg
--rw-r--r--   0        0        0      374 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/src/assets/ThumbsDownIcon.svg
--rw-r--r--   0        0        0      354 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/src/assets/ThumbsUpIcon.svg
--rw-r--r--   0        0        0     1509 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/src/assets/TrashIcon.svg
--rw-r--r--   0        0        0      346 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/src/assets/XCircle.svg
--rw-r--r--   0        0        0     1578 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/src/components/AutosizeTextarea.tsx
--rw-r--r--   0        0        0     4288 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/src/components/ChatMessage.tsx
--rw-r--r--   0        0        0     7735 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/src/components/ChatWindow.tsx
--rw-r--r--   0        0        0     5116 2024-04-01 19:51:36.084289 langserve-0.1.0rc1/langserve/chat_playground/src/components/ShareDialog.tsx
--rw-r--r--   0        0        0     3463 2024-04-01 19:51:36.088289 langserve-0.1.0rc1/langserve/chat_playground/src/components/feedback/CorrectnessFeedback.tsx
--rw-r--r--   0        0        0      308 2024-04-01 19:51:36.088289 langserve-0.1.0rc1/langserve/chat_playground/src/main.tsx
--rw-r--r--   0        0        0      368 2024-04-01 19:51:36.088289 langserve-0.1.0rc1/langserve/chat_playground/src/types.tsx
--rw-r--r--   0        0        0     3924 2024-04-01 19:51:36.088289 langserve-0.1.0rc1/langserve/chat_playground/src/useSchemas.tsx
--rw-r--r--   0        0        0     2345 2024-04-01 19:51:36.088289 langserve-0.1.0rc1/langserve/chat_playground/src/useStreamCallback.tsx
--rw-r--r--   0        0        0     3406 2024-04-01 19:51:36.088289 langserve-0.1.0rc1/langserve/chat_playground/src/useStreamLog.tsx
--rw-r--r--   0        0        0      183 2024-04-01 19:51:36.088289 langserve-0.1.0rc1/langserve/chat_playground/src/utils/cn.ts
--rw-r--r--   0        0        0     5344 2024-04-01 19:51:36.088289 langserve-0.1.0rc1/langserve/chat_playground/src/utils/defaults.ts
--rw-r--r--   0        0        0      140 2024-04-01 19:51:36.088289 langserve-0.1.0rc1/langserve/chat_playground/src/utils/json-refs.d.ts
--rw-r--r--   0        0        0   367401 2024-04-01 19:51:36.088289 langserve-0.1.0rc1/langserve/chat_playground/src/utils/json-refs.js
--rw-r--r--   0        0        0      227 2024-04-01 19:51:36.088289 langserve-0.1.0rc1/langserve/chat_playground/src/utils/messages.ts
--rw-r--r--   0        0        0      726 2024-04-01 19:51:36.088289 langserve-0.1.0rc1/langserve/chat_playground/src/utils/path.ts
--rw-r--r--   0        0        0      548 2024-04-01 19:51:36.088289 langserve-0.1.0rc1/langserve/chat_playground/src/utils/schema.ts
--rw-r--r--   0        0        0      330 2024-04-01 19:51:36.088289 langserve-0.1.0rc1/langserve/chat_playground/src/utils/simplifySchema.ts
--rw-r--r--   0        0        0      147 2024-04-01 19:51:36.088289 langserve-0.1.0rc1/langserve/chat_playground/src/utils/str.ts
--rw-r--r--   0        0        0      958 2024-04-01 19:51:36.088289 langserve-0.1.0rc1/langserve/chat_playground/src/utils/url.ts
--rw-r--r--   0        0        0       87 2024-04-01 19:51:36.088289 langserve-0.1.0rc1/langserve/chat_playground/src/vite-env.d.ts
--rw-r--r--   0        0        0      950 2024-04-01 19:51:36.088289 langserve-0.1.0rc1/langserve/chat_playground/tailwind.config.js
--rw-r--r--   0        0        0      605 2024-04-01 19:51:36.088289 langserve-0.1.0rc1/langserve/chat_playground/tsconfig.json
--rw-r--r--   0        0        0      213 2024-04-01 19:51:36.088289 langserve-0.1.0rc1/langserve/chat_playground/tsconfig.node.json
--rw-r--r--   0        0        0      571 2024-04-01 19:51:36.088289 langserve-0.1.0rc1/langserve/chat_playground/vite.config.ts
--rw-r--r--   0        0        0   134098 2024-04-01 19:51:36.092289 langserve-0.1.0rc1/langserve/chat_playground/yarn.lock
--rw-r--r--   0        0        0    31643 2024-04-01 19:51:36.092289 langserve-0.1.0rc1/langserve/client.py
--rw-r--r--   0        0        0    14983 2024-04-01 19:51:36.092289 langserve-0.1.0rc1/langserve/lzstring.py
--rw-r--r--   0        0        0      436 2024-04-01 19:51:36.092289 langserve-0.1.0rc1/langserve/playground/.eslintrc.cjs
--rw-r--r--   0        0        0      266 2024-04-01 19:51:36.092289 langserve-0.1.0rc1/langserve/playground/.gitignore
--rw-r--r--   0        0        0     1263 2024-04-01 19:51:36.092289 langserve-0.1.0rc1/langserve/playground/README.md
--rw-r--r--   0        0        0    16476 2024-04-01 19:51:36.092289 langserve-0.1.0rc1/langserve/playground/dist/assets/index-52e8ab2f.css
--rw-r--r--   0        0        0  1332675 2024-04-01 19:51:36.100289 langserve-0.1.0rc1/langserve/playground/dist/assets/index-dbc96538.js
--rw-r--r--   0        0        0    40410 2024-04-01 19:51:36.100289 langserve-0.1.0rc1/langserve/playground/dist/favicon.ico
--rw-r--r--   0        0        0      916 2024-04-01 19:51:36.100289 langserve-0.1.0rc1/langserve/playground/dist/index.html
--rw-r--r--   0        0        0      756 2024-04-01 19:51:36.100289 langserve-0.1.0rc1/langserve/playground/index.html
--rw-r--r--   0        0        0     1616 2024-04-01 19:51:36.100289 langserve-0.1.0rc1/langserve/playground/package.json
--rw-r--r--   0        0        0       81 2024-04-01 19:51:36.100289 langserve-0.1.0rc1/langserve/playground/postcss.config.js
--rw-r--r--   0        0        0    40410 2024-04-01 19:51:36.100289 langserve-0.1.0rc1/langserve/playground/public/favicon.ico
--rw-r--r--   0        0        0     2081 2024-04-01 19:51:36.100289 langserve-0.1.0rc1/langserve/playground/src/App.css
--rw-r--r--   0        0        0     7176 2024-04-01 19:51:36.100289 langserve-0.1.0rc1/langserve/playground/src/App.tsx
--rw-r--r--   0        0        0     2626 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/assets/ChatIcon.svg
--rw-r--r--   0        0        0      792 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/assets/CheckCircleIcon.svg
--rw-r--r--   0        0        0      505 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/assets/ChevronRight.svg
--rw-r--r--   0        0        0     1153 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/assets/CircleSpinIcon.svg
--rw-r--r--   0        0        0      823 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/assets/CodeIcon.svg
--rw-r--r--   0        0        0     1328 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/assets/CopyIcon.svg
--rw-r--r--   0        0        0     2350 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/assets/PadlockIcon.svg
--rw-r--r--   0        0        0      670 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/assets/PlusIcon.svg
--rw-r--r--   0        0        0     1260 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/assets/SendIcon.svg
--rw-r--r--   0        0        0     1831 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/assets/ShareIcon.svg
--rw-r--r--   0        0        0     1089 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/assets/ThumbsDownIcon.svg
--rw-r--r--   0        0        0      549 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/assets/ThumbsUpIcon.svg
--rw-r--r--   0        0        0     1509 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/assets/TrashIcon.svg
--rw-r--r--   0        0        0     1424 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/components/AutosizeTextarea.tsx
--rw-r--r--   0        0        0     5541 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/components/ChatMessageInput.tsx
--rw-r--r--   0        0        0     5595 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/components/ChatMessageTuplesControlRenderer.tsx
--rw-r--r--   0        0        0     5168 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/components/ChatMessagesControlRenderer.tsx
--rw-r--r--   0        0        0     1076 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/components/CustomAnyOfRenderer.tsx
--rw-r--r--   0        0        0     2519 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/components/CustomArrayControlRenderer/DeleteDialog.tsx
--rw-r--r--   0        0        0    13357 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/components/CustomArrayControlRenderer/MaterialTableControl.tsx
--rw-r--r--   0        0        0     1562 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/components/CustomArrayControlRenderer/NoBorderTableCell.tsx
--rw-r--r--   0        0        0     3182 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/components/CustomArrayControlRenderer/TableToolbar.tsx
--rw-r--r--   0        0        0     1819 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/components/CustomArrayControlRenderer/ValidationIcon.tsx
--rw-r--r--   0        0        0     3680 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/components/CustomArrayControlRenderer.tsx
--rw-r--r--   0        0        0     2617 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/components/CustomTextAreaCell.tsx
--rw-r--r--   0        0        0     1256 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/components/FileBase64Tester.tsx
--rw-r--r--   0        0        0     2468 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/components/IntermediateSteps.tsx
--rw-r--r--   0        0        0     2941 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/components/JsonTextAreaCell.tsx
--rw-r--r--   0        0        0     5189 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/components/ShareDialog.tsx
--rw-r--r--   0        0        0     3320 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/components/StreamOutput.tsx
--rw-r--r--   0        0        0     2347 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/components/SubmitButton.tsx
--rw-r--r--   0        0        0     2910 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/components/feedback/CorrectnessFeedback.tsx
--rw-r--r--   0        0        0      308 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/main.tsx
--rw-r--r--   0        0        0     3372 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/renderers.tsx
--rw-r--r--   0        0        0     1580 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/sections/SectionConfigure.tsx
--rw-r--r--   0        0        0     2125 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/sections/SectionInputs.tsx
--rw-r--r--   0        0        0      358 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/types.tsx
--rw-r--r--   0        0        0     2633 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/useSchemas.tsx
--rw-r--r--   0        0        0     2345 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/useStreamCallback.tsx
--rw-r--r--   0        0        0     3401 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/useStreamLog.tsx
--rw-r--r--   0        0        0      183 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/utils/cn.ts
--rw-r--r--   0        0        0     5344 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/utils/defaults.ts
--rw-r--r--   0        0        0      140 2024-04-01 19:51:36.104289 langserve-0.1.0rc1/langserve/playground/src/utils/json-refs.d.ts
--rw-r--r--   0        0        0   367401 2024-04-01 19:51:36.108289 langserve-0.1.0rc1/langserve/playground/src/utils/json-refs.js
--rw-r--r--   0        0        0      227 2024-04-01 19:51:36.108289 langserve-0.1.0rc1/langserve/playground/src/utils/messages.ts
--rw-r--r--   0        0        0      726 2024-04-01 19:51:36.108289 langserve-0.1.0rc1/langserve/playground/src/utils/path.ts
--rw-r--r--   0        0        0      548 2024-04-01 19:51:36.108289 langserve-0.1.0rc1/langserve/playground/src/utils/schema.ts
--rw-r--r--   0        0        0      330 2024-04-01 19:51:36.108289 langserve-0.1.0rc1/langserve/playground/src/utils/simplifySchema.ts
--rw-r--r--   0        0        0      147 2024-04-01 19:51:36.108289 langserve-0.1.0rc1/langserve/playground/src/utils/str.ts
--rw-r--r--   0        0        0      958 2024-04-01 19:51:36.108289 langserve-0.1.0rc1/langserve/playground/src/utils/url.ts
--rw-r--r--   0        0        0       87 2024-04-01 19:51:36.108289 langserve-0.1.0rc1/langserve/playground/src/vite-env.d.ts
--rw-r--r--   0        0        0      781 2024-04-01 19:51:36.108289 langserve-0.1.0rc1/langserve/playground/tailwind.config.js
--rw-r--r--   0        0        0      605 2024-04-01 19:51:36.108289 langserve-0.1.0rc1/langserve/playground/tsconfig.json
--rw-r--r--   0        0        0      213 2024-04-01 19:51:36.108289 langserve-0.1.0rc1/langserve/playground/tsconfig.node.json
--rw-r--r--   0        0        0      539 2024-04-01 19:51:36.108289 langserve-0.1.0rc1/langserve/playground/vite.config.ts
--rw-r--r--   0        0        0   135134 2024-04-01 19:51:36.108289 langserve-0.1.0rc1/langserve/playground/yarn.lock
--rw-r--r--   0        0        0     3543 2024-04-01 19:51:36.092289 langserve-0.1.0rc1/langserve/playground.py
--rw-r--r--   0        0        0        0 2024-04-01 19:51:36.108289 langserve-0.1.0rc1/langserve/py.typed
--rw-r--r--   0        0        0     1187 2024-04-01 19:51:36.108289 langserve-0.1.0rc1/langserve/pydantic_v1.py
--rw-r--r--   0        0        0     5337 2024-04-01 19:51:36.108289 langserve-0.1.0rc1/langserve/schema.py
--rw-r--r--   0        0        0     7004 2024-04-01 19:51:36.108289 langserve-0.1.0rc1/langserve/serialization.py
--rw-r--r--   0        0        0    46956 2024-04-01 19:51:36.108289 langserve-0.1.0rc1/langserve/server.py
--rw-r--r--   0        0        0     4089 2024-04-01 19:51:36.108289 langserve-0.1.0rc1/langserve/server_sent_events.py
--rw-r--r--   0        0        0    17233 2024-04-01 19:51:36.108289 langserve-0.1.0rc1/langserve/validation.py
--rw-r--r--   0        0        0      307 2024-04-01 19:51:36.108289 langserve-0.1.0rc1/langserve/version.py
--rw-r--r--   0        0        0     2539 2024-04-01 19:51:36.112289 langserve-0.1.0rc1/pyproject.toml
--rw-r--r--   0        0        0    43302 1970-01-01 00:00:00.000000 langserve-0.1.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     3757 2024-04-03 20:20:49.634701 langserve-0.1.0rc2/LICENSE
+-rw-r--r--   0        0        0    42394 2024-04-03 20:20:49.634701 langserve-0.1.0rc2/README.md
+-rw-r--r--   0        0        0      505 2024-04-03 20:20:49.638701 langserve-0.1.0rc2/langserve/__init__.py
+-rw-r--r--   0        0        0    64390 2024-04-03 20:20:49.638701 langserve-0.1.0rc2/langserve/api_handler.py
+-rw-r--r--   0        0        0    14240 2024-04-03 20:20:49.638701 langserve-0.1.0rc2/langserve/callbacks.py
+-rw-r--r--   0        0        0      436 2024-04-03 20:20:49.638701 langserve-0.1.0rc2/langserve/chat_playground/.eslintrc.cjs
+-rw-r--r--   0        0        0      266 2024-04-03 20:20:49.638701 langserve-0.1.0rc2/langserve/chat_playground/.gitignore
+-rw-r--r--   0        0        0     1263 2024-04-03 20:20:49.638701 langserve-0.1.0rc2/langserve/chat_playground/README.md
+-rw-r--r--   0        0        0    23810 2024-04-03 20:20:49.638701 langserve-0.1.0rc2/langserve/chat_playground/dist/assets/index-434ff580.css
+-rw-r--r--   0        0        0   494586 2024-04-03 20:20:49.642701 langserve-0.1.0rc2/langserve/chat_playground/dist/assets/index-86d4d9c0.js
+-rw-r--r--   0        0        0    40410 2024-04-03 20:20:49.642701 langserve-0.1.0rc2/langserve/chat_playground/dist/favicon.ico
+-rw-r--r--   0        0        0     1141 2024-04-03 20:20:49.642701 langserve-0.1.0rc2/langserve/chat_playground/dist/index.html
+-rw-r--r--   0        0        0      981 2024-04-03 20:20:49.642701 langserve-0.1.0rc2/langserve/chat_playground/index.html
+-rw-r--r--   0        0        0     1526 2024-04-03 20:20:49.642701 langserve-0.1.0rc2/langserve/chat_playground/package.json
+-rw-r--r--   0        0        0       81 2024-04-03 20:20:49.642701 langserve-0.1.0rc2/langserve/chat_playground/postcss.config.js
+-rw-r--r--   0        0        0    40410 2024-04-03 20:20:49.642701 langserve-0.1.0rc2/langserve/chat_playground/public/favicon.ico
+-rw-r--r--   0        0        0     2554 2024-04-03 20:20:49.642701 langserve-0.1.0rc2/langserve/chat_playground/src/App.css
+-rw-r--r--   0        0        0     2989 2024-04-03 20:20:49.642701 langserve-0.1.0rc2/langserve/chat_playground/src/App.tsx
+-rw-r--r--   0        0        0      310 2024-04-03 20:20:49.642701 langserve-0.1.0rc2/langserve/chat_playground/src/assets/ArrowUp.svg
+-rw-r--r--   0        0        0     2626 2024-04-03 20:20:49.642701 langserve-0.1.0rc2/langserve/chat_playground/src/assets/ChatIcon.svg
+-rw-r--r--   0        0        0      789 2024-04-03 20:20:49.642701 langserve-0.1.0rc2/langserve/chat_playground/src/assets/CheckCircleIcon.svg
+-rw-r--r--   0        0        0      328 2024-04-03 20:20:49.642701 langserve-0.1.0rc2/langserve/chat_playground/src/assets/CheckCircleIcon2.svg
+-rw-r--r--   0        0        0      505 2024-04-03 20:20:49.642701 langserve-0.1.0rc2/langserve/chat_playground/src/assets/ChevronRight.svg
+-rw-r--r--   0        0        0     1153 2024-04-03 20:20:49.642701 langserve-0.1.0rc2/langserve/chat_playground/src/assets/CircleSpinIcon.svg
+-rw-r--r--   0        0        0      823 2024-04-03 20:20:49.642701 langserve-0.1.0rc2/langserve/chat_playground/src/assets/CodeIcon.svg
+-rw-r--r--   0        0        0     1328 2024-04-03 20:20:49.642701 langserve-0.1.0rc2/langserve/chat_playground/src/assets/CopyIcon.svg
+-rw-r--r--   0        0        0     1744 2024-04-03 20:20:49.642701 langserve-0.1.0rc2/langserve/chat_playground/src/assets/EmptyState.svg
+-rw-r--r--   0        0        0    11000 2024-04-03 20:20:49.642701 langserve-0.1.0rc2/langserve/chat_playground/src/assets/LangServeLogo.svg
+-rw-r--r--   0        0        0     2350 2024-04-03 20:20:49.642701 langserve-0.1.0rc2/langserve/chat_playground/src/assets/PadlockIcon.svg
+-rw-r--r--   0        0        0      670 2024-04-03 20:20:49.642701 langserve-0.1.0rc2/langserve/chat_playground/src/assets/PlusIcon.svg
+-rw-r--r--   0        0        0      400 2024-04-03 20:20:49.642701 langserve-0.1.0rc2/langserve/chat_playground/src/assets/RefreshCW.svg
+-rw-r--r--   0        0        0     1260 2024-04-03 20:20:49.642701 langserve-0.1.0rc2/langserve/chat_playground/src/assets/SendIcon.svg
+-rw-r--r--   0        0        0     1831 2024-04-03 20:20:49.642701 langserve-0.1.0rc2/langserve/chat_playground/src/assets/ShareIcon.svg
+-rw-r--r--   0        0        0      374 2024-04-03 20:20:49.642701 langserve-0.1.0rc2/langserve/chat_playground/src/assets/ThumbsDownIcon.svg
+-rw-r--r--   0        0        0      354 2024-04-03 20:20:49.642701 langserve-0.1.0rc2/langserve/chat_playground/src/assets/ThumbsUpIcon.svg
+-rw-r--r--   0        0        0     1509 2024-04-03 20:20:49.642701 langserve-0.1.0rc2/langserve/chat_playground/src/assets/TrashIcon.svg
+-rw-r--r--   0        0        0      346 2024-04-03 20:20:49.642701 langserve-0.1.0rc2/langserve/chat_playground/src/assets/XCircle.svg
+-rw-r--r--   0        0        0     1578 2024-04-03 20:20:49.642701 langserve-0.1.0rc2/langserve/chat_playground/src/components/AutosizeTextarea.tsx
+-rw-r--r--   0        0        0     4288 2024-04-03 20:20:49.642701 langserve-0.1.0rc2/langserve/chat_playground/src/components/ChatMessage.tsx
+-rw-r--r--   0        0        0     7735 2024-04-03 20:20:49.642701 langserve-0.1.0rc2/langserve/chat_playground/src/components/ChatWindow.tsx
+-rw-r--r--   0        0        0     5116 2024-04-03 20:20:49.642701 langserve-0.1.0rc2/langserve/chat_playground/src/components/ShareDialog.tsx
+-rw-r--r--   0        0        0     3463 2024-04-03 20:20:49.642701 langserve-0.1.0rc2/langserve/chat_playground/src/components/feedback/CorrectnessFeedback.tsx
+-rw-r--r--   0        0        0      308 2024-04-03 20:20:49.642701 langserve-0.1.0rc2/langserve/chat_playground/src/main.tsx
+-rw-r--r--   0        0        0      368 2024-04-03 20:20:49.642701 langserve-0.1.0rc2/langserve/chat_playground/src/types.tsx
+-rw-r--r--   0        0        0     3924 2024-04-03 20:20:49.642701 langserve-0.1.0rc2/langserve/chat_playground/src/useSchemas.tsx
+-rw-r--r--   0        0        0     2345 2024-04-03 20:20:49.646701 langserve-0.1.0rc2/langserve/chat_playground/src/useStreamCallback.tsx
+-rw-r--r--   0        0        0     3406 2024-04-03 20:20:49.646701 langserve-0.1.0rc2/langserve/chat_playground/src/useStreamLog.tsx
+-rw-r--r--   0        0        0      183 2024-04-03 20:20:49.646701 langserve-0.1.0rc2/langserve/chat_playground/src/utils/cn.ts
+-rw-r--r--   0        0        0     5344 2024-04-03 20:20:49.646701 langserve-0.1.0rc2/langserve/chat_playground/src/utils/defaults.ts
+-rw-r--r--   0        0        0      140 2024-04-03 20:20:49.646701 langserve-0.1.0rc2/langserve/chat_playground/src/utils/json-refs.d.ts
+-rw-r--r--   0        0        0   367401 2024-04-03 20:20:49.646701 langserve-0.1.0rc2/langserve/chat_playground/src/utils/json-refs.js
+-rw-r--r--   0        0        0      227 2024-04-03 20:20:49.646701 langserve-0.1.0rc2/langserve/chat_playground/src/utils/messages.ts
+-rw-r--r--   0        0        0      726 2024-04-03 20:20:49.646701 langserve-0.1.0rc2/langserve/chat_playground/src/utils/path.ts
+-rw-r--r--   0        0        0      548 2024-04-03 20:20:49.646701 langserve-0.1.0rc2/langserve/chat_playground/src/utils/schema.ts
+-rw-r--r--   0        0        0      330 2024-04-03 20:20:49.646701 langserve-0.1.0rc2/langserve/chat_playground/src/utils/simplifySchema.ts
+-rw-r--r--   0        0        0      147 2024-04-03 20:20:49.646701 langserve-0.1.0rc2/langserve/chat_playground/src/utils/str.ts
+-rw-r--r--   0        0        0      958 2024-04-03 20:20:49.646701 langserve-0.1.0rc2/langserve/chat_playground/src/utils/url.ts
+-rw-r--r--   0        0        0       87 2024-04-03 20:20:49.646701 langserve-0.1.0rc2/langserve/chat_playground/src/vite-env.d.ts
+-rw-r--r--   0        0        0      950 2024-04-03 20:20:49.646701 langserve-0.1.0rc2/langserve/chat_playground/tailwind.config.js
+-rw-r--r--   0        0        0      605 2024-04-03 20:20:49.646701 langserve-0.1.0rc2/langserve/chat_playground/tsconfig.json
+-rw-r--r--   0        0        0      213 2024-04-03 20:20:49.646701 langserve-0.1.0rc2/langserve/chat_playground/tsconfig.node.json
+-rw-r--r--   0        0        0      571 2024-04-03 20:20:49.646701 langserve-0.1.0rc2/langserve/chat_playground/vite.config.ts
+-rw-r--r--   0        0        0   134098 2024-04-03 20:20:49.646701 langserve-0.1.0rc2/langserve/chat_playground/yarn.lock
+-rw-r--r--   0        0        0    31643 2024-04-03 20:20:49.646701 langserve-0.1.0rc2/langserve/client.py
+-rw-r--r--   0        0        0    14983 2024-04-03 20:20:49.646701 langserve-0.1.0rc2/langserve/lzstring.py
+-rw-r--r--   0        0        0      436 2024-04-03 20:20:49.646701 langserve-0.1.0rc2/langserve/playground/.eslintrc.cjs
+-rw-r--r--   0        0        0      266 2024-04-03 20:20:49.646701 langserve-0.1.0rc2/langserve/playground/.gitignore
+-rw-r--r--   0        0        0     1263 2024-04-03 20:20:49.646701 langserve-0.1.0rc2/langserve/playground/README.md
+-rw-r--r--   0        0        0    16476 2024-04-03 20:20:49.646701 langserve-0.1.0rc2/langserve/playground/dist/assets/index-52e8ab2f.css
+-rw-r--r--   0        0        0  1332675 2024-04-03 20:20:49.654702 langserve-0.1.0rc2/langserve/playground/dist/assets/index-dbc96538.js
+-rw-r--r--   0        0        0    40410 2024-04-03 20:20:49.654702 langserve-0.1.0rc2/langserve/playground/dist/favicon.ico
+-rw-r--r--   0        0        0      916 2024-04-03 20:20:49.654702 langserve-0.1.0rc2/langserve/playground/dist/index.html
+-rw-r--r--   0        0        0      756 2024-04-03 20:20:49.654702 langserve-0.1.0rc2/langserve/playground/index.html
+-rw-r--r--   0        0        0     1616 2024-04-03 20:20:49.654702 langserve-0.1.0rc2/langserve/playground/package.json
+-rw-r--r--   0        0        0       81 2024-04-03 20:20:49.654702 langserve-0.1.0rc2/langserve/playground/postcss.config.js
+-rw-r--r--   0        0        0    40410 2024-04-03 20:20:49.654702 langserve-0.1.0rc2/langserve/playground/public/favicon.ico
+-rw-r--r--   0        0        0     2081 2024-04-03 20:20:49.654702 langserve-0.1.0rc2/langserve/playground/src/App.css
+-rw-r--r--   0        0        0     7176 2024-04-03 20:20:49.654702 langserve-0.1.0rc2/langserve/playground/src/App.tsx
+-rw-r--r--   0        0        0     2626 2024-04-03 20:20:49.654702 langserve-0.1.0rc2/langserve/playground/src/assets/ChatIcon.svg
+-rw-r--r--   0        0        0      792 2024-04-03 20:20:49.654702 langserve-0.1.0rc2/langserve/playground/src/assets/CheckCircleIcon.svg
+-rw-r--r--   0        0        0      505 2024-04-03 20:20:49.654702 langserve-0.1.0rc2/langserve/playground/src/assets/ChevronRight.svg
+-rw-r--r--   0        0        0     1153 2024-04-03 20:20:49.654702 langserve-0.1.0rc2/langserve/playground/src/assets/CircleSpinIcon.svg
+-rw-r--r--   0        0        0      823 2024-04-03 20:20:49.654702 langserve-0.1.0rc2/langserve/playground/src/assets/CodeIcon.svg
+-rw-r--r--   0        0        0     1328 2024-04-03 20:20:49.654702 langserve-0.1.0rc2/langserve/playground/src/assets/CopyIcon.svg
+-rw-r--r--   0        0        0     2350 2024-04-03 20:20:49.654702 langserve-0.1.0rc2/langserve/playground/src/assets/PadlockIcon.svg
+-rw-r--r--   0        0        0      670 2024-04-03 20:20:49.654702 langserve-0.1.0rc2/langserve/playground/src/assets/PlusIcon.svg
+-rw-r--r--   0        0        0     1260 2024-04-03 20:20:49.654702 langserve-0.1.0rc2/langserve/playground/src/assets/SendIcon.svg
+-rw-r--r--   0        0        0     1831 2024-04-03 20:20:49.654702 langserve-0.1.0rc2/langserve/playground/src/assets/ShareIcon.svg
+-rw-r--r--   0        0        0     1089 2024-04-03 20:20:49.654702 langserve-0.1.0rc2/langserve/playground/src/assets/ThumbsDownIcon.svg
+-rw-r--r--   0        0        0      549 2024-04-03 20:20:49.654702 langserve-0.1.0rc2/langserve/playground/src/assets/ThumbsUpIcon.svg
+-rw-r--r--   0        0        0     1509 2024-04-03 20:20:49.654702 langserve-0.1.0rc2/langserve/playground/src/assets/TrashIcon.svg
+-rw-r--r--   0        0        0     1424 2024-04-03 20:20:49.654702 langserve-0.1.0rc2/langserve/playground/src/components/AutosizeTextarea.tsx
+-rw-r--r--   0        0        0     5541 2024-04-03 20:20:49.654702 langserve-0.1.0rc2/langserve/playground/src/components/ChatMessageInput.tsx
+-rw-r--r--   0        0        0     5595 2024-04-03 20:20:49.654702 langserve-0.1.0rc2/langserve/playground/src/components/ChatMessageTuplesControlRenderer.tsx
+-rw-r--r--   0        0        0     5168 2024-04-03 20:20:49.654702 langserve-0.1.0rc2/langserve/playground/src/components/ChatMessagesControlRenderer.tsx
+-rw-r--r--   0        0        0     1076 2024-04-03 20:20:49.654702 langserve-0.1.0rc2/langserve/playground/src/components/CustomAnyOfRenderer.tsx
+-rw-r--r--   0        0        0     2519 2024-04-03 20:20:49.654702 langserve-0.1.0rc2/langserve/playground/src/components/CustomArrayControlRenderer/DeleteDialog.tsx
+-rw-r--r--   0        0        0    13357 2024-04-03 20:20:49.654702 langserve-0.1.0rc2/langserve/playground/src/components/CustomArrayControlRenderer/MaterialTableControl.tsx
+-rw-r--r--   0        0        0     1562 2024-04-03 20:20:49.654702 langserve-0.1.0rc2/langserve/playground/src/components/CustomArrayControlRenderer/NoBorderTableCell.tsx
+-rw-r--r--   0        0        0     3182 2024-04-03 20:20:49.654702 langserve-0.1.0rc2/langserve/playground/src/components/CustomArrayControlRenderer/TableToolbar.tsx
+-rw-r--r--   0        0        0     1819 2024-04-03 20:20:49.654702 langserve-0.1.0rc2/langserve/playground/src/components/CustomArrayControlRenderer/ValidationIcon.tsx
+-rw-r--r--   0        0        0     3680 2024-04-03 20:20:49.654702 langserve-0.1.0rc2/langserve/playground/src/components/CustomArrayControlRenderer.tsx
+-rw-r--r--   0        0        0     2617 2024-04-03 20:20:49.654702 langserve-0.1.0rc2/langserve/playground/src/components/CustomTextAreaCell.tsx
+-rw-r--r--   0        0        0     1256 2024-04-03 20:20:49.654702 langserve-0.1.0rc2/langserve/playground/src/components/FileBase64Tester.tsx
+-rw-r--r--   0        0        0     2468 2024-04-03 20:20:49.654702 langserve-0.1.0rc2/langserve/playground/src/components/IntermediateSteps.tsx
+-rw-r--r--   0        0        0     2941 2024-04-03 20:20:49.654702 langserve-0.1.0rc2/langserve/playground/src/components/JsonTextAreaCell.tsx
+-rw-r--r--   0        0        0     5189 2024-04-03 20:20:49.654702 langserve-0.1.0rc2/langserve/playground/src/components/ShareDialog.tsx
+-rw-r--r--   0        0        0     3320 2024-04-03 20:20:49.654702 langserve-0.1.0rc2/langserve/playground/src/components/StreamOutput.tsx
+-rw-r--r--   0        0        0     2347 2024-04-03 20:20:49.654702 langserve-0.1.0rc2/langserve/playground/src/components/SubmitButton.tsx
+-rw-r--r--   0        0        0     2910 2024-04-03 20:20:49.654702 langserve-0.1.0rc2/langserve/playground/src/components/feedback/CorrectnessFeedback.tsx
+-rw-r--r--   0        0        0      308 2024-04-03 20:20:49.654702 langserve-0.1.0rc2/langserve/playground/src/main.tsx
+-rw-r--r--   0        0        0     3372 2024-04-03 20:20:49.658702 langserve-0.1.0rc2/langserve/playground/src/renderers.tsx
+-rw-r--r--   0        0        0     1580 2024-04-03 20:20:49.658702 langserve-0.1.0rc2/langserve/playground/src/sections/SectionConfigure.tsx
+-rw-r--r--   0        0        0     2125 2024-04-03 20:20:49.658702 langserve-0.1.0rc2/langserve/playground/src/sections/SectionInputs.tsx
+-rw-r--r--   0        0        0      358 2024-04-03 20:20:49.658702 langserve-0.1.0rc2/langserve/playground/src/types.tsx
+-rw-r--r--   0        0        0     2633 2024-04-03 20:20:49.658702 langserve-0.1.0rc2/langserve/playground/src/useSchemas.tsx
+-rw-r--r--   0        0        0     2345 2024-04-03 20:20:49.658702 langserve-0.1.0rc2/langserve/playground/src/useStreamCallback.tsx
+-rw-r--r--   0        0        0     3401 2024-04-03 20:20:49.658702 langserve-0.1.0rc2/langserve/playground/src/useStreamLog.tsx
+-rw-r--r--   0        0        0      183 2024-04-03 20:20:49.658702 langserve-0.1.0rc2/langserve/playground/src/utils/cn.ts
+-rw-r--r--   0        0        0     5344 2024-04-03 20:20:49.658702 langserve-0.1.0rc2/langserve/playground/src/utils/defaults.ts
+-rw-r--r--   0        0        0      140 2024-04-03 20:20:49.658702 langserve-0.1.0rc2/langserve/playground/src/utils/json-refs.d.ts
+-rw-r--r--   0        0        0   367401 2024-04-03 20:20:49.658702 langserve-0.1.0rc2/langserve/playground/src/utils/json-refs.js
+-rw-r--r--   0        0        0      227 2024-04-03 20:20:49.658702 langserve-0.1.0rc2/langserve/playground/src/utils/messages.ts
+-rw-r--r--   0        0        0      726 2024-04-03 20:20:49.658702 langserve-0.1.0rc2/langserve/playground/src/utils/path.ts
+-rw-r--r--   0        0        0      548 2024-04-03 20:20:49.658702 langserve-0.1.0rc2/langserve/playground/src/utils/schema.ts
+-rw-r--r--   0        0        0      330 2024-04-03 20:20:49.658702 langserve-0.1.0rc2/langserve/playground/src/utils/simplifySchema.ts
+-rw-r--r--   0        0        0      147 2024-04-03 20:20:49.658702 langserve-0.1.0rc2/langserve/playground/src/utils/str.ts
+-rw-r--r--   0        0        0      958 2024-04-03 20:20:49.658702 langserve-0.1.0rc2/langserve/playground/src/utils/url.ts
+-rw-r--r--   0        0        0       87 2024-04-03 20:20:49.658702 langserve-0.1.0rc2/langserve/playground/src/vite-env.d.ts
+-rw-r--r--   0        0        0      781 2024-04-03 20:20:49.658702 langserve-0.1.0rc2/langserve/playground/tailwind.config.js
+-rw-r--r--   0        0        0      605 2024-04-03 20:20:49.658702 langserve-0.1.0rc2/langserve/playground/tsconfig.json
+-rw-r--r--   0        0        0      213 2024-04-03 20:20:49.658702 langserve-0.1.0rc2/langserve/playground/tsconfig.node.json
+-rw-r--r--   0        0        0      539 2024-04-03 20:20:49.658702 langserve-0.1.0rc2/langserve/playground/vite.config.ts
+-rw-r--r--   0        0        0   135134 2024-04-03 20:20:49.658702 langserve-0.1.0rc2/langserve/playground/yarn.lock
+-rw-r--r--   0        0        0     3543 2024-04-03 20:20:49.646701 langserve-0.1.0rc2/langserve/playground.py
+-rw-r--r--   0        0        0        0 2024-04-03 20:20:49.658702 langserve-0.1.0rc2/langserve/py.typed
+-rw-r--r--   0        0        0     1187 2024-04-03 20:20:49.658702 langserve-0.1.0rc2/langserve/pydantic_v1.py
+-rw-r--r--   0        0        0     5349 2024-04-03 20:20:49.658702 langserve-0.1.0rc2/langserve/schema.py
+-rw-r--r--   0        0        0     7004 2024-04-03 20:20:49.658702 langserve-0.1.0rc2/langserve/serialization.py
+-rw-r--r--   0        0        0    46956 2024-04-03 20:20:49.658702 langserve-0.1.0rc2/langserve/server.py
+-rw-r--r--   0        0        0     4089 2024-04-03 20:20:49.658702 langserve-0.1.0rc2/langserve/server_sent_events.py
+-rw-r--r--   0        0        0    17233 2024-04-03 20:20:49.658702 langserve-0.1.0rc2/langserve/validation.py
+-rw-r--r--   0        0        0      307 2024-04-03 20:20:49.658702 langserve-0.1.0rc2/langserve/version.py
+-rw-r--r--   0        0        0     2539 2024-04-03 20:20:49.662702 langserve-0.1.0rc2/pyproject.toml
+-rw-r--r--   0        0        0    43302 1970-01-01 00:00:00.000000 langserve-0.1.0rc2/PKG-INFO
```

### Comparing `langserve-0.1.0rc1/LICENSE` & `langserve-0.1.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/README.md` & `langserve-0.1.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/api_handler.py` & `langserve-0.1.0rc2/langserve/api_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -473,19 +473,14 @@
     config["callbacks"].extend(callbacks)
 
 
 _MODEL_REGISTRY = {}
 _SEEN_NAMES = set()
 
 
-def _is_scoped_feedback_enabled() -> bool:
-    """Temporary hard-coded as False. Used only to enable during unit tests."""
-    return False
-
-
 class PerKeyFeedbackConfig(TypedDict):
     """Per feedback configuration.
 
     Use to configure the feedback token.
     """
 
     key: str
@@ -646,15 +641,16 @@
         self._token_feedback_config = token_feedback_config
         self._token_feedback_enabled = token_feedback_config is not None
 
         # Client is patched using mock.patch, if changing the names
         # remember to make relevant updates in the unit tests.
         self._langsmith_client = (
             ls_client.Client()
-            if tracing_is_enabled() and enable_feedback_endpoint
+            if tracing_is_enabled()
+            and (enable_feedback_endpoint or self._token_feedback_enabled)
             else None
         )
 
         with_types = {}
 
         if input_type != "auto":
             with_types["input_type"] = input_type
@@ -1177,29 +1173,47 @@
         try:
             config, input_ = await self._get_config_and_input(
                 request,
                 config_hash,
                 endpoint="stream_log",
                 server_config=server_config,
             )
+            run_id = config["run_id"]
         except BaseException:
             # Exceptions will be properly translated by default FastAPI middleware
             # to either 422 (on input validation) or 500 internal server errors.
             raise
         try:
             body = await request.json()
             with _with_validation_error_translation():
                 stream_log_request = StreamLogParameters(**body)
         except json.JSONDecodeError:
             raise RequestValidationError(errors=["Invalid JSON body"])
         except RequestValidationError:
             raise
 
+        feedback_key: Optional[str]
+
+        if self._token_feedback_enabled:
+            # Create task to create a presigned feedback token
+            feedback_key: str = self._token_feedback_config["key_configs"][0]["key"]
+            feedback_coro = run_in_executor(
+                None,
+                self._langsmith_client.create_presigned_feedback_token,
+                run_id,
+                feedback_key,
+            )
+            task: Optional[asyncio.Task] = asyncio.create_task(feedback_coro)
+        else:
+            feedback_key = None
+            task = None
+
         async def _stream_log() -> AsyncIterator[dict]:
             """Stream the output of the runnable."""
+            has_sent_metadata = False
             try:
                 async for chunk in self._runnable.astream_log(
                     input_,
                     config=config,
                     diff=True,
                     include_names=stream_log_request.include_names,
                     include_types=stream_log_request.include_types,
@@ -1225,14 +1239,26 @@
                         yield {
                             # EventSourceResponse expects a string for data
                             # so after serializing into bytes, we decode into utf-8
                             # to get a string.
                             "data": self._serializer.dumps(data).decode("utf-8"),
                             "event": "data",
                         }
+
+                    # Send a metadata event as soon as possible
+                    if not has_sent_metadata and self._enable_feedback_endpoint:
+                        if task is None:
+                            raise AssertionError("Feedback token task was not created.")
+                        if not task.done():
+                            continue
+                        feedback_token = task.result()
+                        yield _create_metadata_event(
+                            run_id, feedback_key, feedback_token
+                        )
+                        has_sent_metadata = True
                 yield {"event": "end"}
             except BaseException:
                 yield {
                     "event": "error",
                     # Do not expose the error message to the client since
                     # the message may contain sensitive information.
                     # We'll add client side errors for validation as well.
```

### Comparing `langserve-0.1.0rc1/langserve/callbacks.py` & `langserve-0.1.0rc2/langserve/callbacks.py`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/chat_playground/README.md` & `langserve-0.1.0rc2/langserve/chat_playground/README.md`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/chat_playground/dist/assets/index-434ff580.css` & `langserve-0.1.0rc2/langserve/chat_playground/dist/assets/index-434ff580.css`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/chat_playground/dist/assets/index-86d4d9c0.js` & `langserve-0.1.0rc2/langserve/chat_playground/dist/assets/index-86d4d9c0.js`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/chat_playground/dist/favicon.ico` & `langserve-0.1.0rc2/langserve/chat_playground/dist/favicon.ico`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/chat_playground/dist/index.html` & `langserve-0.1.0rc2/langserve/chat_playground/dist/index.html`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/chat_playground/index.html` & `langserve-0.1.0rc2/langserve/chat_playground/index.html`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/chat_playground/package.json` & `langserve-0.1.0rc2/langserve/chat_playground/package.json`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/chat_playground/public/favicon.ico` & `langserve-0.1.0rc2/langserve/chat_playground/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/chat_playground/src/App.css` & `langserve-0.1.0rc2/langserve/chat_playground/src/App.css`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/chat_playground/src/App.tsx` & `langserve-0.1.0rc2/langserve/chat_playground/src/App.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/chat_playground/src/assets/ChatIcon.svg` & `langserve-0.1.0rc2/langserve/chat_playground/src/assets/ChatIcon.svg`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/chat_playground/src/assets/CheckCircleIcon.svg` & `langserve-0.1.0rc2/langserve/chat_playground/src/assets/CheckCircleIcon.svg`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/chat_playground/src/assets/CircleSpinIcon.svg` & `langserve-0.1.0rc2/langserve/chat_playground/src/assets/CircleSpinIcon.svg`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/chat_playground/src/assets/CodeIcon.svg` & `langserve-0.1.0rc2/langserve/chat_playground/src/assets/CodeIcon.svg`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/chat_playground/src/assets/CopyIcon.svg` & `langserve-0.1.0rc2/langserve/chat_playground/src/assets/CopyIcon.svg`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/chat_playground/src/assets/EmptyState.svg` & `langserve-0.1.0rc2/langserve/chat_playground/src/assets/EmptyState.svg`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/chat_playground/src/assets/LangServeLogo.svg` & `langserve-0.1.0rc2/langserve/chat_playground/src/assets/LangServeLogo.svg`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/chat_playground/src/assets/PadlockIcon.svg` & `langserve-0.1.0rc2/langserve/chat_playground/src/assets/PadlockIcon.svg`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/chat_playground/src/assets/PlusIcon.svg` & `langserve-0.1.0rc2/langserve/chat_playground/src/assets/PlusIcon.svg`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/chat_playground/src/assets/SendIcon.svg` & `langserve-0.1.0rc2/langserve/chat_playground/src/assets/SendIcon.svg`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/chat_playground/src/assets/ShareIcon.svg` & `langserve-0.1.0rc2/langserve/chat_playground/src/assets/ShareIcon.svg`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/chat_playground/src/assets/TrashIcon.svg` & `langserve-0.1.0rc2/langserve/chat_playground/src/assets/TrashIcon.svg`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/chat_playground/src/components/AutosizeTextarea.tsx` & `langserve-0.1.0rc2/langserve/chat_playground/src/components/AutosizeTextarea.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/chat_playground/src/components/ChatMessage.tsx` & `langserve-0.1.0rc2/langserve/chat_playground/src/components/ChatMessage.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/chat_playground/src/components/ChatWindow.tsx` & `langserve-0.1.0rc2/langserve/chat_playground/src/components/ChatWindow.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/chat_playground/src/components/ShareDialog.tsx` & `langserve-0.1.0rc2/langserve/chat_playground/src/components/ShareDialog.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/chat_playground/src/components/feedback/CorrectnessFeedback.tsx` & `langserve-0.1.0rc2/langserve/chat_playground/src/components/feedback/CorrectnessFeedback.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/chat_playground/src/useSchemas.tsx` & `langserve-0.1.0rc2/langserve/chat_playground/src/useSchemas.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/chat_playground/src/useStreamCallback.tsx` & `langserve-0.1.0rc2/langserve/chat_playground/src/useStreamCallback.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/chat_playground/src/useStreamLog.tsx` & `langserve-0.1.0rc2/langserve/chat_playground/src/useStreamLog.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/chat_playground/src/utils/defaults.ts` & `langserve-0.1.0rc2/langserve/chat_playground/src/utils/defaults.ts`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/chat_playground/src/utils/json-refs.js` & `langserve-0.1.0rc2/langserve/chat_playground/src/utils/json-refs.js`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/chat_playground/src/utils/path.ts` & `langserve-0.1.0rc2/langserve/chat_playground/src/utils/path.ts`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/chat_playground/src/utils/schema.ts` & `langserve-0.1.0rc2/langserve/chat_playground/src/utils/schema.ts`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/chat_playground/src/utils/url.ts` & `langserve-0.1.0rc2/langserve/chat_playground/src/utils/url.ts`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/chat_playground/tailwind.config.js` & `langserve-0.1.0rc2/langserve/chat_playground/tailwind.config.js`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/chat_playground/tsconfig.json` & `langserve-0.1.0rc2/langserve/chat_playground/tsconfig.json`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/chat_playground/vite.config.ts` & `langserve-0.1.0rc2/langserve/chat_playground/vite.config.ts`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/chat_playground/yarn.lock` & `langserve-0.1.0rc2/langserve/chat_playground/yarn.lock`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/client.py` & `langserve-0.1.0rc2/langserve/client.py`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/lzstring.py` & `langserve-0.1.0rc2/langserve/lzstring.py`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/playground/README.md` & `langserve-0.1.0rc2/langserve/playground/README.md`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/playground/dist/assets/index-52e8ab2f.css` & `langserve-0.1.0rc2/langserve/playground/dist/assets/index-52e8ab2f.css`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/playground/dist/assets/index-dbc96538.js` & `langserve-0.1.0rc2/langserve/playground/dist/assets/index-dbc96538.js`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/playground/dist/favicon.ico` & `langserve-0.1.0rc2/langserve/playground/dist/favicon.ico`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/playground/dist/index.html` & `langserve-0.1.0rc2/langserve/playground/dist/index.html`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/playground/index.html` & `langserve-0.1.0rc2/langserve/playground/index.html`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/playground/package.json` & `langserve-0.1.0rc2/langserve/playground/package.json`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/playground/public/favicon.ico` & `langserve-0.1.0rc2/langserve/playground/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/playground/src/App.css` & `langserve-0.1.0rc2/langserve/playground/src/App.css`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/playground/src/App.tsx` & `langserve-0.1.0rc2/langserve/playground/src/App.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/playground/src/assets/ChatIcon.svg` & `langserve-0.1.0rc2/langserve/playground/src/assets/ChatIcon.svg`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/playground/src/assets/CheckCircleIcon.svg` & `langserve-0.1.0rc2/langserve/playground/src/assets/CheckCircleIcon.svg`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/playground/src/assets/CircleSpinIcon.svg` & `langserve-0.1.0rc2/langserve/playground/src/assets/CircleSpinIcon.svg`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/playground/src/assets/CodeIcon.svg` & `langserve-0.1.0rc2/langserve/playground/src/assets/CodeIcon.svg`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/playground/src/assets/CopyIcon.svg` & `langserve-0.1.0rc2/langserve/playground/src/assets/CopyIcon.svg`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/playground/src/assets/PadlockIcon.svg` & `langserve-0.1.0rc2/langserve/playground/src/assets/PadlockIcon.svg`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/playground/src/assets/PlusIcon.svg` & `langserve-0.1.0rc2/langserve/playground/src/assets/PlusIcon.svg`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/playground/src/assets/SendIcon.svg` & `langserve-0.1.0rc2/langserve/playground/src/assets/SendIcon.svg`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/playground/src/assets/ShareIcon.svg` & `langserve-0.1.0rc2/langserve/playground/src/assets/ShareIcon.svg`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/playground/src/assets/ThumbsDownIcon.svg` & `langserve-0.1.0rc2/langserve/playground/src/assets/ThumbsDownIcon.svg`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/playground/src/assets/ThumbsUpIcon.svg` & `langserve-0.1.0rc2/langserve/playground/src/assets/ThumbsUpIcon.svg`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/playground/src/assets/TrashIcon.svg` & `langserve-0.1.0rc2/langserve/playground/src/assets/TrashIcon.svg`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/playground/src/components/AutosizeTextarea.tsx` & `langserve-0.1.0rc2/langserve/playground/src/components/AutosizeTextarea.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/playground/src/components/ChatMessageInput.tsx` & `langserve-0.1.0rc2/langserve/playground/src/components/ChatMessageInput.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/playground/src/components/ChatMessageTuplesControlRenderer.tsx` & `langserve-0.1.0rc2/langserve/playground/src/components/ChatMessageTuplesControlRenderer.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/playground/src/components/ChatMessagesControlRenderer.tsx` & `langserve-0.1.0rc2/langserve/playground/src/components/ChatMessagesControlRenderer.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/playground/src/components/CustomAnyOfRenderer.tsx` & `langserve-0.1.0rc2/langserve/playground/src/components/CustomAnyOfRenderer.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/playground/src/components/CustomArrayControlRenderer/DeleteDialog.tsx` & `langserve-0.1.0rc2/langserve/playground/src/components/CustomArrayControlRenderer/DeleteDialog.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/playground/src/components/CustomArrayControlRenderer/MaterialTableControl.tsx` & `langserve-0.1.0rc2/langserve/playground/src/components/CustomArrayControlRenderer/MaterialTableControl.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/playground/src/components/CustomArrayControlRenderer/NoBorderTableCell.tsx` & `langserve-0.1.0rc2/langserve/playground/src/components/CustomArrayControlRenderer/NoBorderTableCell.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/playground/src/components/CustomArrayControlRenderer/TableToolbar.tsx` & `langserve-0.1.0rc2/langserve/playground/src/components/CustomArrayControlRenderer/TableToolbar.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/playground/src/components/CustomArrayControlRenderer/ValidationIcon.tsx` & `langserve-0.1.0rc2/langserve/playground/src/components/CustomArrayControlRenderer/ValidationIcon.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/playground/src/components/CustomArrayControlRenderer.tsx` & `langserve-0.1.0rc2/langserve/playground/src/components/CustomArrayControlRenderer.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/playground/src/components/CustomTextAreaCell.tsx` & `langserve-0.1.0rc2/langserve/playground/src/components/CustomTextAreaCell.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/playground/src/components/FileBase64Tester.tsx` & `langserve-0.1.0rc2/langserve/playground/src/components/FileBase64Tester.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/playground/src/components/IntermediateSteps.tsx` & `langserve-0.1.0rc2/langserve/playground/src/components/IntermediateSteps.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/playground/src/components/JsonTextAreaCell.tsx` & `langserve-0.1.0rc2/langserve/playground/src/components/JsonTextAreaCell.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/playground/src/components/ShareDialog.tsx` & `langserve-0.1.0rc2/langserve/playground/src/components/ShareDialog.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/playground/src/components/StreamOutput.tsx` & `langserve-0.1.0rc2/langserve/playground/src/components/StreamOutput.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/playground/src/components/SubmitButton.tsx` & `langserve-0.1.0rc2/langserve/playground/src/components/SubmitButton.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/playground/src/components/feedback/CorrectnessFeedback.tsx` & `langserve-0.1.0rc2/langserve/playground/src/components/feedback/CorrectnessFeedback.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/playground/src/renderers.tsx` & `langserve-0.1.0rc2/langserve/playground/src/renderers.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/playground/src/sections/SectionConfigure.tsx` & `langserve-0.1.0rc2/langserve/playground/src/sections/SectionConfigure.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/playground/src/sections/SectionInputs.tsx` & `langserve-0.1.0rc2/langserve/playground/src/sections/SectionInputs.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/playground/src/useSchemas.tsx` & `langserve-0.1.0rc2/langserve/playground/src/useSchemas.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/playground/src/useStreamCallback.tsx` & `langserve-0.1.0rc2/langserve/playground/src/useStreamCallback.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/playground/src/useStreamLog.tsx` & `langserve-0.1.0rc2/langserve/playground/src/useStreamLog.tsx`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/playground/src/utils/defaults.ts` & `langserve-0.1.0rc2/langserve/playground/src/utils/defaults.ts`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/playground/src/utils/json-refs.js` & `langserve-0.1.0rc2/langserve/playground/src/utils/json-refs.js`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/playground/src/utils/path.ts` & `langserve-0.1.0rc2/langserve/playground/src/utils/path.ts`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/playground/src/utils/schema.ts` & `langserve-0.1.0rc2/langserve/playground/src/utils/schema.ts`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/playground/src/utils/url.ts` & `langserve-0.1.0rc2/langserve/playground/src/utils/url.ts`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/playground/tailwind.config.js` & `langserve-0.1.0rc2/langserve/playground/tailwind.config.js`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/playground/tsconfig.json` & `langserve-0.1.0rc2/langserve/playground/tsconfig.json`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/playground/vite.config.ts` & `langserve-0.1.0rc2/langserve/playground/vite.config.ts`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/playground/yarn.lock` & `langserve-0.1.0rc2/langserve/playground/yarn.lock`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/playground.py` & `langserve-0.1.0rc2/langserve/playground.py`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/pydantic_v1.py` & `langserve-0.1.0rc2/langserve/pydantic_v1.py`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/schema.py` & `langserve-0.1.0rc2/langserve/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,15 +112,15 @@
     comment: Optional[str] = None
     """Comment or explanation for the feedback."""
 
 
 class FeedbackCreateRequestTokenBased(BaseModel):
     """Shared information between create requests of feedback and feedback objects."""
 
-    token_or_url: UUID
+    token_or_url: Union[UUID, str]
     """The associated run ID this feedback is logged for."""
 
     score: Optional[Union[float, int, bool]] = None
     """Value or score to assign the run."""
 
     value: Optional[Union[float, int, bool, str, Dict]] = None
     """The display value for the feedback if not a metric."""
```

### Comparing `langserve-0.1.0rc1/langserve/serialization.py` & `langserve-0.1.0rc2/langserve/serialization.py`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/server.py` & `langserve-0.1.0rc2/langserve/server.py`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/server_sent_events.py` & `langserve-0.1.0rc2/langserve/server_sent_events.py`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/langserve/validation.py` & `langserve-0.1.0rc2/langserve/validation.py`

 * *Files identical despite different names*

### Comparing `langserve-0.1.0rc1/pyproject.toml` & `langserve-0.1.0rc2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langserve"
-version = "0.1.0rc1"
+version = "0.1.0rc2"
 description = ""
 readme = "README.md"
 authors = ["LangChain"]
 license = "LangServe"
 repository = "https://github.com/langchain-ai/langserve"
 exclude = ["langserve/playground,langserve/chat_playground"]
 include = ["langserve/playground/dist/**/*", "langserve/chat_playground/dist/**/*"]
```

### Comparing `langserve-0.1.0rc1/PKG-INFO` & `langserve-0.1.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langserve
-Version: 0.1.0rc1
+Version: 0.1.0rc2
 Summary: 
 Home-page: https://github.com/langchain-ai/langserve
 License: LangServe
 Author: LangChain
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

