# Comparing `tmp/glyphsets-0.6.8.tar.gz` & `tmp/glyphsets-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glyphsets-0.6.8.tar", last modified: Wed Dec 13 15:18:48 2023, max compression
+gzip compressed data, was "glyphsets-0.6.9.tar", last modified: Fri Dec 15 14:17:58 2023, max compression
```

## Comparing `glyphsets-0.6.8.tar` & `glyphsets-0.6.9.tar`

### file list

```diff
@@ -1,529 +1,530 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.648574 glyphsets-0.6.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.536573 glyphsets-0.6.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.548573 glyphsets-0.6.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2023-12-13 15:18:37.000000 glyphsets-0.6.8/.github/workflows/publish-release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      695 2023-12-13 15:18:37.000000 glyphsets-0.6.8/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)       43 2023-12-13 15:18:37.000000 glyphsets-0.6.8/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.548573 glyphsets-0.6.8/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2023-12-13 15:18:37.000000 glyphsets-0.6.8/.vscode/settings.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.536573 glyphsets-0.6.8/Archive/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.548573 glyphsets-0.6.8/Archive/GF Glyph Sets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.548573 glyphsets-0.6.8/Archive/GF Glyph Sets/Arabic/
--rw-r--r--   0 runner    (1001) docker     (127)     4544 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/Arabic/GF-arabic-core.nam
--rw-r--r--   0 runner    (1001) docker     (127)     6134 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/Arabic/GF-arabic-plus.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/Arabic/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.548573 glyphsets-0.6.8/Archive/GF Glyph Sets/Cyrillic/
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-historical_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-plus-locl_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    10080 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-plus_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-pro_unique-glyphs.nam
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.536573 glyphsets-0.6.8/Archive/GF Glyph Sets/Cyrillic/filter lists/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.552573 glyphsets-0.6.8/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/
--rw-r--r--   0 runner    (1001) docker     (127)      473 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/historical_unique-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      668 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus-locl_unique-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      485 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus-locl_unique-glyphs_italic.txt
--rw-r--r--   0 runner    (1001) docker     (127)      596 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus-locl_unique-glyphs_roman.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus_unique-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      712 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus_unique-glyphs_core.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus_unique-glyphs_smallcaps.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/pro_unique-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      461 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/pro_unique-glyphs_smallcaps.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.552573 glyphsets-0.6.8/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/historical_unique-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      640 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus-locl_unique-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      463 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus-locl_unique-glyphs_italic.txt
--rw-r--r--   0 runner    (1001) docker     (127)      559 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus-locl_unique-glyphs_roman.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus_unique-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      791 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus_unique-glyphs_core.txt
--rw-r--r--   0 runner    (1001) docker     (127)      990 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus_unique-glyphs_smallcaps.txt
--rw-r--r--   0 runner    (1001) docker     (127)      734 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/pro_unique-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      297 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/pro_unique-glyphs_smallcaps.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6864 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/GF-latin-core_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     6148 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/GF-latin-expert_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    18371 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/GF-latin-global_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      683 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/GF-latin-plus_optional-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    16079 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/GF-latin-plus_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      795 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/GF-latin-pro_optional-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     5442 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/GF-latin-pro_unique-glyphs.nam
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.556573 glyphsets-0.6.8/Archive/GF Glyph Sets/Greek/
--rw-r--r--   0 runner    (1001) docker     (127)    16666 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/Greek/GF-greek-ancient-musical-symbols.nam
--rw-r--r--   0 runner    (1001) docker     (127)     5589 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/Greek/GF-greek-archaic.nam
--rw-r--r--   0 runner    (1001) docker     (127)     5663 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/Greek/GF-greek-coptic.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/Greek/GF-greek-core.nam
--rw-r--r--   0 runner    (1001) docker     (127)     8571 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/Greek/GF-greek-expert.nam
--rw-r--r--   0 runner    (1001) docker     (127)    14827 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/Greek/GF-greek-plus.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2776 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/Greek/GF-greek-pro.nam
--rw-r--r--   0 runner    (1001) docker     (127)     7194 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/Greek/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.536573 glyphsets-0.6.8/Archive/GF Glyph Sets/Greek/filter lists/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.556573 glyphsets-0.6.8/Archive/GF Glyph Sets/Greek/filter lists/nice names/
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/Greek/filter lists/nice names/ancient-musical-symbols.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/Greek/filter lists/nice names/archaic.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/Greek/filter lists/nice names/coptic.txt
--rw-r--r--   0 runner    (1001) docker     (127)      613 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/Greek/filter lists/nice names/core.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5907 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/Greek/filter lists/nice names/expert.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5156 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/Greek/filter lists/nice names/plus.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/Greek/filter lists/nice names/pro.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.556573 glyphsets-0.6.8/Archive/GF Glyph Sets/Greek/filter lists/uni names/
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/Greek/filter lists/uni names/ancient-musical-symbols.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/Greek/filter lists/uni names/archaic.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/Greek/filter lists/uni names/coptic.txt
--rw-r--r--   0 runner    (1001) docker     (127)      592 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/Greek/filter lists/uni names/core.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3395 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/Greek/filter lists/uni names/expert.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/Greek/filter lists/uni names/plus.txt
--rw-r--r--   0 runner    (1001) docker     (127)      665 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/Greek/filter lists/uni names/pro.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12967 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3667 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/RECOMMENDED.md
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/TROUBLESHOOTING.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.556573 glyphsets-0.6.8/Archive/GF Glyph Sets/Vietnamese/
--rw-r--r--   0 runner    (1001) docker     (127)     4482 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/Vietnamese/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.556573 glyphsets-0.6.8/Archive/GF Glyph Sets/Vietnamese/img/
--rw-r--r--   0 runner    (1001) docker     (127)    16279 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/Vietnamese/img/VIT_accents.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    75853 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/Vietnamese/img/VIT_glyphs.jpg
--rw-r--r--   0 runner    (1001) docker     (127)   104148 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/Vietnamese/img/locl.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.560573 glyphsets-0.6.8/Archive/GF Glyph Sets/filter lists/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/filter lists/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.560573 glyphsets-0.6.8/Archive/GF Glyph Sets/filter lists/nice names/
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/filter lists/nice names/core_unique-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3414 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/filter lists/nice names/expert_unique-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      458 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/filter lists/nice names/plus_optional-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4023 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/filter lists/nice names/plus_unique-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      462 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/filter lists/nice names/pro_optional-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/filter lists/nice names/pro_unique-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      465 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/filter lists/plus_optional-glyphs_case-accents.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/filter lists/plus_unique-glyphs_vietnamese-all.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/filter lists/plus_unique-glyphs_vietnamese-unique.txt
--rw-r--r--   0 runner    (1001) docker     (127)      461 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/filter lists/pro_optional-glyphs_case-punctuation.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.560573 glyphsets-0.6.8/Archive/GF Glyph Sets/filter lists/uni names/
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/filter lists/uni names/core_unique-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/filter lists/uni names/expert_unique-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      354 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/filter lists/uni names/plus_optional-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3123 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/filter lists/uni names/plus_unique-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      462 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/filter lists/uni names/pro_optional-glyphs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/filter lists/uni names/pro_unique-glyphs.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.564573 glyphsets-0.6.8/Archive/GF Glyph Sets/glyphTypeSorting/
--rw-r--r--   0 runner    (1001) docker     (127)     4917 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/glyphTypeSorting/EXPERT_composites_207.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/glyphTypeSorting/EXPERT_drawn_62.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/glyphTypeSorting/EXPERT_either_4.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7831 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/glyphTypeSorting/PLUS_composites_360.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4010 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/glyphTypeSorting/PLUS_drawn_215.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4057 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/glyphTypeSorting/PLUS_drawn_216.txt
--rw-r--r--   0 runner    (1001) docker     (127)      330 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/glyphTypeSorting/PLUS_either_19.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/glyphTypeSorting/PRO_composites_116.txt
--rw-r--r--   0 runner    (1001) docker     (127)      585 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/glyphTypeSorting/PRO_drawn_26.txt
--rw-r--r--   0 runner    (1001) docker     (127)      100 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/glyphTypeSorting/PRO_either_4.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.564573 glyphsets-0.6.8/Archive/GF Glyph Sets/tutorials/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.564573 glyphsets-0.6.8/Archive/GF Glyph Sets/tutorials/Glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)    43666 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/tutorials/Glyphs/CustomFilter.plist
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.564573 glyphsets-0.6.8/Archive/GF Glyph Sets/tutorials/Glyphs/Info/
--rw-r--r--   0 runner    (1001) docker     (127)    89964 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/tutorials/Glyphs/Info/GlyphData.xml
--rw-r--r--   0 runner    (1001) docker     (127)     9153 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/tutorials/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.568573 glyphsets-0.6.8/Archive/GF Glyph Sets/tutorials/img/
--rw-r--r--   0 runner    (1001) docker     (127)    35092 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/tutorials/img/Directory.png
--rw-r--r--   0 runner    (1001) docker     (127)    98535 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/tutorials/img/ListFilters.png
--rw-r--r--   0 runner    (1001) docker     (127)    84092 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/tutorials/img/PoiretOne-locl.png
--rw-r--r--   0 runner    (1001) docker     (127)    24052 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/tutorials/img/ecircumflexacute.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    71431 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/tutorials/img/fix-1.png
--rw-r--r--   0 runner    (1001) docker     (127)    33541 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/tutorials/img/fix-2.png
--rw-r--r--   0 runner    (1001) docker     (127)    45217 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/tutorials/img/fix-3.png
--rw-r--r--   0 runner    (1001) docker     (127)    53065 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/tutorials/img/list-filter-1.png
--rw-r--r--   0 runner    (1001) docker     (127)     7677 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Archive/GF Glyph Sets/tutorials/img/list-filter.png
--rw-r--r--   0 runner    (1001) docker     (127)     4835 2023-12-13 15:18:37.000000 glyphsets-0.6.8/CHANGELOG.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.568573 glyphsets-0.6.8/GF_glyphsets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.568573 glyphsets-0.6.8/GF_glyphsets/Arabic/
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Arabic/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.568573 glyphsets-0.6.8/GF_glyphsets/Arabic/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)    15527 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Arabic/glyphs/CustomFilter_GF_Arabic.plist
--rw-r--r--   0 runner    (1001) docker     (127)    15494 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Arabic/glyphs/GF_Arabic_Core.glyphs
--rw-r--r--   0 runner    (1001) docker     (127)     6459 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Arabic/glyphs/GF_Arabic_Plus.glyphs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.568573 glyphsets-0.6.8/GF_glyphsets/Arabic/nam/
--rw-r--r--   0 runner    (1001) docker     (127)     4037 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Arabic/nam/GF_Arabic_Core.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Arabic/nam/GF_Arabic_Plus.nam
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.540573 glyphsets-0.6.8/GF_glyphsets/Arabic/txt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.568573 glyphsets-0.6.8/GF_glyphsets/Arabic/txt/nice-names/
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Arabic/txt/nice-names/GF_Arabic_Core.txt
--rw-r--r--   0 runner    (1001) docker     (127)      540 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Arabic/txt/nice-names/GF_Arabic_Plus.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.568573 glyphsets-0.6.8/GF_glyphsets/Arabic/txt/prod-names/
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Arabic/txt/prod-names/GF_Arabic_Core.txt
--rw-r--r--   0 runner    (1001) docker     (127)      343 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Arabic/txt/prod-names/GF_Arabic_Plus.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.568573 glyphsets-0.6.8/GF_glyphsets/Cyrillic/
--rw-r--r--   0 runner    (1001) docker     (127)     4089 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Cyrillic/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.572573 glyphsets-0.6.8/GF_glyphsets/Cyrillic/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)    21454 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Cyrillic/glyphs/CustomFilter_GF_Cyrillic.plist
--rw-r--r--   0 runner    (1001) docker     (127)    11221 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_Core.glyphs
--rw-r--r--   0 runner    (1001) docker     (127)     5815 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_Historical.glyphs
--rw-r--r--   0 runner    (1001) docker     (127)    11251 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_Plus.glyphs
--rw-r--r--   0 runner    (1001) docker     (127)     4804 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_PlusLoclItalic.glyphs
--rw-r--r--   0 runner    (1001) docker     (127)     5310 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_PlusLoclRoman.glyphs
--rw-r--r--   0 runner    (1001) docker     (127)     7759 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_Pro.glyphs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.572573 glyphsets-0.6.8/GF_glyphsets/Cyrillic/nam/
--rw-r--r--   0 runner    (1001) docker     (127)     3462 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_Core.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_Historical.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3956 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_Plus.nam
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_PlusLoclItalic.nam
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_PlusLoclRoman.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_Pro.nam
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.540573 glyphsets-0.6.8/GF_glyphsets/Cyrillic/txt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.572573 glyphsets-0.6.8/GF_glyphsets/Cyrillic/txt/nice-names/
--rw-r--r--   0 runner    (1001) docker     (127)      710 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_Core.txt
--rw-r--r--   0 runner    (1001) docker     (127)      472 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_Historical.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_Plus.txt
--rw-r--r--   0 runner    (1001) docker     (127)      483 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_PlusLoclItalic.txt
--rw-r--r--   0 runner    (1001) docker     (127)      594 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_PlusLoclRoman.txt
--rw-r--r--   0 runner    (1001) docker     (127)      773 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_Pro.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.572573 glyphsets-0.6.8/GF_glyphsets/Cyrillic/txt/prod-names/
--rw-r--r--   0 runner    (1001) docker     (127)      785 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Cyrillic/txt/prod-names/GF_Cyrillic_Core.txt
--rw-r--r--   0 runner    (1001) docker     (127)      287 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Cyrillic/txt/prod-names/GF_Cyrillic_Historical.txt
--rw-r--r--   0 runner    (1001) docker     (127)      777 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Cyrillic/txt/prod-names/GF_Cyrillic_Plus.txt
--rw-r--r--   0 runner    (1001) docker     (127)      466 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Cyrillic/txt/prod-names/GF_Cyrillic_PlusLoclItalic.txt
--rw-r--r--   0 runner    (1001) docker     (127)      562 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Cyrillic/txt/prod-names/GF_Cyrillic_PlusLoclRoman.txt
--rw-r--r--   0 runner    (1001) docker     (127)      461 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Cyrillic/txt/prod-names/GF_Cyrillic_Pro.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.572573 glyphsets-0.6.8/GF_glyphsets/Greek/
--rw-r--r--   0 runner    (1001) docker     (127)     7194 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Greek/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.576573 glyphsets-0.6.8/GF_glyphsets/Greek/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)    56423 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Greek/glyphs/CustomFilter_GF_Greek.plist
--rw-r--r--   0 runner    (1001) docker     (127)    30534 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Greek/glyphs/GF_Greek_AncientMusicalSymbols.glyphs
--rw-r--r--   0 runner    (1001) docker     (127)    16742 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Greek/glyphs/GF_Greek_Archaic.glyphs
--rw-r--r--   0 runner    (1001) docker     (127)    15594 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Greek/glyphs/GF_Greek_Coptic.glyphs
--rw-r--r--   0 runner    (1001) docker     (127)     9091 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Greek/glyphs/GF_Greek_Core.glyphs
--rw-r--r--   0 runner    (1001) docker     (127)    26352 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Greek/glyphs/GF_Greek_Expert.glyphs
--rw-r--r--   0 runner    (1001) docker     (127)    28310 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Greek/glyphs/GF_Greek_Plus.glyphs
--rw-r--r--   0 runner    (1001) docker     (127)    10390 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Greek/glyphs/GF_Greek_Pro.glyphs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.576573 glyphsets-0.6.8/GF_glyphsets/Greek/nam/
--rw-r--r--   0 runner    (1001) docker     (127)    15006 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Greek/nam/GF_Greek_AncientMusicalSymbols.nam
--rw-r--r--   0 runner    (1001) docker     (127)     4912 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Greek/nam/GF_Greek_Archaic.nam
--rw-r--r--   0 runner    (1001) docker     (127)     4550 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Greek/nam/GF_Greek_Coptic.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Greek/nam/GF_Greek_Core.nam
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Greek/nam/GF_Greek_Expert.nam
--rw-r--r--   0 runner    (1001) docker     (127)    12597 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Greek/nam/GF_Greek_Plus.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Greek/nam/GF_Greek_Pro.nam
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.540573 glyphsets-0.6.8/GF_glyphsets/Greek/txt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.580573 glyphsets-0.6.8/GF_glyphsets/Greek/txt/nice-names/
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Greek/txt/nice-names/GF_Greek_AncientMusicalSymbols.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Archaic.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Coptic.txt
--rw-r--r--   0 runner    (1001) docker     (127)      612 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Core.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5906 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Expert.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5155 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Plus.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Pro.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.580573 glyphsets-0.6.8/GF_glyphsets/Greek/txt/prod-names/
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Greek/txt/prod-names/GF_Greek_AncientMusicalSymbols.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Archaic.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Coptic.txt
--rw-r--r--   0 runner    (1001) docker     (127)      591 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Core.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3394 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Expert.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Plus.txt
--rw-r--r--   0 runner    (1001) docker     (127)      664 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Pro.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.580573 glyphsets-0.6.8/GF_glyphsets/Latin/
--rw-r--r--   0 runner    (1001) docker     (127)     8429 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Latin/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.580573 glyphsets-0.6.8/GF_glyphsets/Latin/definitions/
--rw-r--r--   0 runner    (1001) docker     (127)     3017 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Latin/definitions/GF_Latin_Core.stub.glyphs
--rw-r--r--   0 runner    (1001) docker     (127)     2016 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Latin/definitions/GF_Latin_Core.stub.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2821 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Latin/definitions/GF_Latin_Kernel.stub.nam
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.580573 glyphsets-0.6.8/GF_glyphsets/Latin/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)    37841 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Latin/glyphs/CustomFilter_GF_Latin.plist
--rw-r--r--   0 runner    (1001) docker     (127)    62282 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Latin/glyphs/GF_Latin_African.glyphs
--rw-r--r--   0 runner    (1001) docker     (127)    19144 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Latin/glyphs/GF_Latin_Beyond.glyphs
--rw-r--r--   0 runner    (1001) docker     (127)    16087 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Latin/glyphs/GF_Latin_Core.glyphs
--rw-r--r--   0 runner    (1001) docker     (127)     5086 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Latin/glyphs/GF_Latin_Kernel.glyphs
--rw-r--r--   0 runner    (1001) docker     (127)    18721 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Latin/glyphs/GF_Latin_Plus.glyphs
--rw-r--r--   0 runner    (1001) docker     (127)    15064 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Latin/glyphs/GF_Latin_Vietnamese.glyphs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.584573 glyphsets-0.6.8/GF_glyphsets/Latin/nam/
--rw-r--r--   0 runner    (1001) docker     (127)    17738 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Latin/nam/GF_Latin_African.nam
--rw-r--r--   0 runner    (1001) docker     (127)     5398 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Latin/nam/GF_Latin_Beyond.nam
--rw-r--r--   0 runner    (1001) docker     (127)    10747 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Latin/nam/GF_Latin_Core.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2897 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Latin/nam/GF_Latin_Kernel.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Latin/nam/GF_Latin_Plus.nam
--rw-r--r--   0 runner    (1001) docker     (127)     4858 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Latin/nam/GF_Latin_Vietnamese.nam
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.540573 glyphsets-0.6.8/GF_glyphsets/Latin/txt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.584573 glyphsets-0.6.8/GF_glyphsets/Latin/txt/nice-names/
--rw-r--r--   0 runner    (1001) docker     (127)     4637 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Latin/txt/nice-names/GF_Latin_African.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Beyond.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Core.txt
--rw-r--r--   0 runner    (1001) docker     (127)      692 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Kernel.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Plus.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Vietnamese.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.584573 glyphsets-0.6.8/GF_glyphsets/Latin/txt/prod-names/
--rw-r--r--   0 runner    (1001) docker     (127)     3438 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Latin/txt/prod-names/GF_Latin_African.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Beyond.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Core.txt
--rw-r--r--   0 runner    (1001) docker     (127)      692 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Kernel.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Plus.txt
--rw-r--r--   0 runner    (1001) docker     (127)      886 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Vietnamese.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.584573 glyphsets-0.6.8/GF_glyphsets/Phonetics/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Phonetics/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.588573 glyphsets-0.6.8/GF_glyphsets/Phonetics/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)    19280 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Phonetics/glyphs/CustomFilter_GF_Phonetics.plist
--rw-r--r--   0 runner    (1001) docker     (127)     4478 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_APA.glyphs
--rw-r--r--   0 runner    (1001) docker     (127)     8928 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_DisorderedSpeech.glyphs
--rw-r--r--   0 runner    (1001) docker     (127)     3524 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_IPAHistorical.glyphs
--rw-r--r--   0 runner    (1001) docker     (127)    17764 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_IPAStandard.glyphs
--rw-r--r--   0 runner    (1001) docker     (127)     3395 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_SinoExt.glyphs
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_UPA.glyphs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.588573 glyphsets-0.6.8/GF_glyphsets/Phonetics/nam/
--rw-r--r--   0 runner    (1001) docker     (127)      877 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Phonetics/nam/GF_Phonetics_APA.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2542 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Phonetics/nam/GF_Phonetics_DisorderedSpeech.nam
--rw-r--r--   0 runner    (1001) docker     (127)      508 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Phonetics/nam/GF_Phonetics_IPAHistorical.nam
--rw-r--r--   0 runner    (1001) docker     (127)     6119 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Phonetics/nam/GF_Phonetics_IPAStandard.nam
--rw-r--r--   0 runner    (1001) docker     (127)      466 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Phonetics/nam/GF_Phonetics_SinoExt.nam
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Phonetics/nam/GF_Phonetics_UPA.nam
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.544573 glyphsets-0.6.8/GF_glyphsets/Phonetics/txt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.588573 glyphsets-0.6.8/GF_glyphsets/Phonetics/txt/nice-names/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Phonetics/txt/nice-names/GF_Phonetics_APA.txt
--rw-r--r--   0 runner    (1001) docker     (127)      855 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Phonetics/txt/nice-names/GF_Phonetics_DisorderedSpeech.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Phonetics/txt/nice-names/GF_Phonetics_IPAHistorical.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Phonetics/txt/nice-names/GF_Phonetics_IPAStandard.txt
--rw-r--r--   0 runner    (1001) docker     (127)      122 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Phonetics/txt/nice-names/GF_Phonetics_SinoExt.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Phonetics/txt/nice-names/GF_Phonetics_UPA.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.592574 glyphsets-0.6.8/GF_glyphsets/Phonetics/txt/prod-names/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Phonetics/txt/prod-names/GF_Phonetics_APA.txt
--rw-r--r--   0 runner    (1001) docker     (127)      568 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Phonetics/txt/prod-names/GF_Phonetics_DisorderedSpeech.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Phonetics/txt/prod-names/GF_Phonetics_IPAHistorical.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Phonetics/txt/prod-names/GF_Phonetics_IPAStandard.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Phonetics/txt/prod-names/GF_Phonetics_SinoExt.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/Phonetics/txt/prod-names/GF_Phonetics_UPA.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.592574 glyphsets-0.6.8/GF_glyphsets/TransLatin/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/TransLatin/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.592574 glyphsets-0.6.8/GF_glyphsets/TransLatin/glyphs/
--rw-r--r--   0 runner    (1001) docker     (127)     7427 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/TransLatin/glyphs/CustomFilter_GF_TransLatin.plist
--rw-r--r--   0 runner    (1001) docker     (127)     6786 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/TransLatin/glyphs/GF_TransLatin_Arabic.glyphs
--rw-r--r--   0 runner    (1001) docker     (127)    14581 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/TransLatin/glyphs/GF_TransLatin_Pinyin.glyphs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.592574 glyphsets-0.6.8/GF_glyphsets/TransLatin/nam/
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/TransLatin/nam/GF_TransLatin_Arabic.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3635 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/TransLatin/nam/GF_TransLatin_Pinyin.nam
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.544573 glyphsets-0.6.8/GF_glyphsets/TransLatin/txt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.592574 glyphsets-0.6.8/GF_glyphsets/TransLatin/txt/nice-names/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/TransLatin/txt/nice-names/GF_TransLatin_Arabic.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/TransLatin/txt/nice-names/GF_TransLatin_Pinyin.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.592574 glyphsets-0.6.8/GF_glyphsets/TransLatin/txt/prod-names/
--rw-r--r--   0 runner    (1001) docker     (127)      301 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/TransLatin/txt/prod-names/GF_TransLatin_Arabic.txt
--rw-r--r--   0 runner    (1001) docker     (127)      799 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/TransLatin/txt/prod-names/GF_TransLatin_Pinyin.txt
--rw-r--r--   0 runner    (1001) docker     (127)      550 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/empty_font.glyphs
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2023-12-13 15:18:37.000000 glyphsets-0.6.8/GF_glyphsets/update-gs.sh
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-12-13 15:18:37.000000 glyphsets-0.6.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.544573 glyphsets-0.6.8/Lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.596573 glyphsets-0.6.8/Lib/glyphsets/
--rw-r--r--   0 runner    (1001) docker     (127)     9723 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3372 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2023-12-13 15:18:48.000000 glyphsets-0.6.8/Lib/glyphsets/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    16554 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/codepoints.py
--rw-r--r--   0 runner    (1001) docker     (127)   587834 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/data.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.596573 glyphsets-0.6.8/Lib/glyphsets/definitions/
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/definitions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.596573 glyphsets-0.6.8/Lib/glyphsets/definitions/nam/
--rw-r--r--   0 runner    (1001) docker     (127)    10747 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/definitions/nam/GF_Latin_Core.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2897 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/definitions/nam/GF_Latin_Kernel.nam
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.632574 glyphsets-0.6.8/Lib/glyphsets/encodings/
--rw-r--r--   0 runner    (1001) docker     (127)     7232 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4230 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/adlam_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/ahom_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    20007 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/anatolian-hieroglyphs_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    57487 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/arabic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3688 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/armenian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/avestan_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     4358 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/balinese_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    22272 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/bamum_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/bassa-vah_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/batak_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3395 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/bengali_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3012 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/bhaiksuki_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3204 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/brahmi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     9037 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/braille_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      984 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/buginese_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      688 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/buhid_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    25715 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/canadian-aboriginal_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/carian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2799 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/caucasian-albanian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2534 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/chakma_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/cham_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     5389 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/cherokee_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)   284694 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/chinese-hongkong_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)   298348 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/chinese-simplified_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)   241902 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/chinese-traditional_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/chorasmian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     6988 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/coptic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    46227 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/cuneiform_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/cypriot_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3518 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/cypro-minoan_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     5503 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/cyrillic-ext_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/cyrillic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/deseret_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     7837 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/devanagari_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/dives-akuru_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/dogra_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     4776 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/duployan_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    41018 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/egyptian-hieroglyphs_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/elbasan_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      689 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/elymaic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    33746 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/emoji_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    16949 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/ethiopic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     7001 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/georgian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     5502 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/glagolitic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      923 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/gothic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3473 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/grantha_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    13891 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/greek-ext_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     5381 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/greek_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3677 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/gujarati_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/gunjala-gondi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/gurmukhi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/hanifi-rohingya_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      757 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/hanunoo_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      794 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/hatran_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3793 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/hebrew_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/imperial-aramaic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3378 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/indic-siyaq-numbers_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/inscriptional-pahlavi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/inscriptional-parthian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    91251 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/japanese_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2861 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/javanese_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/kaithi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3112 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/kannada_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/kawi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/kayah-li_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/kharoshthi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    21734 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/khitan-small-script_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     7970 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/khmer_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2439 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/khojki_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/khudawadi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    80178 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/korean_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/lao_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    37362 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/latin-ext_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     7898 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/latin_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/lepcha_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/limbu_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     9503 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/linear-a_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     9214 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/linear-b_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/lisu_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      755 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/lycian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      712 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/lydian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/mahajani_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      792 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/makasar_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     4477 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/malayalam_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      917 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/mandaic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/manichaean_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2179 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/marchen_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/masaram-gondi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)   190939 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/math.nam
--rw-r--r--   0 runner    (1001) docker     (127)    95179 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/math_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      621 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/mayan-numerals_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3293 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/medefaidrin_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/meetei-mayek_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     8592 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/mende-kikakui_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/meroitic-cursive_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/meroitic-hieroglyphs_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     5231 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/meroitic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     4051 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/miao_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/modi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     7491 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/mongolian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/mro_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/multani_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    24495 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/music_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     7463 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/myanmar_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/nabataean_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/nag-mundari_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2998 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/nandinagari_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/new-tai-lue_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/newa_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/nko_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    13878 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/nushu_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/nyiakeng-puachue-hmong_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      811 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/ogham_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/ol-chiki_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     4526 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/old-hungarian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/old-italic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/old-north-arabian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/old-permic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/old-persian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/old-sogdian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/old-south-arabian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2766 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/old-turkic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/old-uyghur_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2687 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/oriya_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2472 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/osage_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/osmanya_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2627 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/ottoman-siyaq-numbers_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     4508 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/pahawh-hmong_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/palmyrene_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/pau-cin-hau_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/phags-pa_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      943 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/phoenician_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/psalter-pahlavi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/rejang_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/runic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/samaritan_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/saurashtra_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/sharada_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/shavian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/siddham_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    35208 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/signwriting_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     4834 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/sinhala_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/sogdian_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/sora-sompeng_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2666 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/soyombo_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/sundanese_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/syloti-nagri_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)   118220 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/symbols_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     4168 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/syriac_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      817 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/tagalog_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      696 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/tagbanwa_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/tai-le_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/tai-tham_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/tai-viet_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/takri_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/tamil-supplement_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2306 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/tamil_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2941 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/tangsa_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)   212192 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/tangut_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3171 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/telugu_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/thaana_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/thai_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     7175 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/tibetan_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/tifinagh_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3115 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/tirhuta_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      990 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/toto_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)      935 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/ugaritic_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     7189 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/vai_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     5794 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/vietnamese_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/vithkuqi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/wancho_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/warang-citi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     5193 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/wgl-latin.enc
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/yezidi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)    30939 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/yi_unique-glyphs.nam
--rw-r--r--   0 runner    (1001) docker     (127)     2874 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/encodings/zanabazar-square_unique-glyphs.nam
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.640574 glyphsets-0.6.8/Lib/glyphsets/slices/
--rw-r--r--   0 runner    (1001) docker     (127)      782 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/slices/README.md
--rw-r--r--   0 runner    (1001) docker     (127)  1087488 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/slices/hongkong-chinese_default.txt
--rw-r--r--   0 runner    (1001) docker     (127)   893039 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/slices/japanese_default.txt
--rw-r--r--   0 runner    (1001) docker     (127)   876086 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/slices/korean_default.txt
--rw-r--r--   0 runner    (1001) docker     (127)   889189 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/slices/simplified-chinese_default.txt
--rw-r--r--   0 runner    (1001) docker     (127)   904276 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/slices/traditional-chinese_default.txt
--rw-r--r--   0 runner    (1001) docker     (127)      938 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/subsets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3017 2023-12-13 15:18:37.000000 glyphsets-0.6.8/Lib/glyphsets/test_strings.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.644574 glyphsets-0.6.8/Lib/glyphsets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7948 2023-12-13 15:18:48.000000 glyphsets-0.6.8/Lib/glyphsets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    23856 2023-12-13 15:18:48.000000 glyphsets-0.6.8/Lib/glyphsets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 15:18:48.000000 glyphsets-0.6.8/Lib/glyphsets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2023-12-13 15:18:48.000000 glyphsets-0.6.8/Lib/glyphsets.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 15:18:48.000000 glyphsets-0.6.8/Lib/glyphsets.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       56 2023-12-13 15:18:48.000000 glyphsets-0.6.8/Lib/glyphsets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-12-13 15:18:48.000000 glyphsets-0.6.8/Lib/glyphsets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7948 2023-12-13 15:18:48.648574 glyphsets-0.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7169 2023-12-13 15:18:37.000000 glyphsets-0.6.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       68 2023-12-13 15:18:37.000000 glyphsets-0.6.8/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.644574 glyphsets-0.6.8/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     7064 2023-12-13 15:18:37.000000 glyphsets-0.6.8/scripts/assemble_charactersets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2023-12-13 15:18:37.000000 glyphsets-0.6.8/scripts/assemble_languages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2023-12-13 15:18:37.000000 glyphsets-0.6.8/scripts/create-glyphset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2023-12-13 15:18:37.000000 glyphsets-0.6.8/scripts/find_language_for_character.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 15:18:48.648574 glyphsets-0.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2023-12-13 15:18:37.000000 glyphsets-0.6.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.644574 glyphsets-0.6.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2023-12-13 15:18:37.000000 glyphsets-0.6.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:18:48.644574 glyphsets-0.6.8/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)    90712 2023-12-13 15:18:37.000000 glyphsets-0.6.8/tests/data/MavenPro[wght].ttf
--rw-r--r--   0 runner    (1001) docker     (127)     4264 2023-12-13 15:18:37.000000 glyphsets-0.6.8/tests/test_glyphdata.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2023-12-13 15:18:37.000000 glyphsets-0.6.8/tests/test_glyphsets.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2023-12-13 15:18:37.000000 glyphsets-0.6.8/tests/test_teststrings.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2023-12-13 15:18:37.000000 glyphsets-0.6.8/tests/test_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4132 2023-12-13 15:18:37.000000 glyphsets-0.6.8/tests/testcoverage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.826099 glyphsets-0.6.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.722099 glyphsets-0.6.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.730099 glyphsets-0.6.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2023-12-15 14:17:45.000000 glyphsets-0.6.9/.github/workflows/publish-release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2023-12-15 14:17:45.000000 glyphsets-0.6.9/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2023-12-15 14:17:45.000000 glyphsets-0.6.9/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.730099 glyphsets-0.6.9/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2023-12-15 14:17:45.000000 glyphsets-0.6.9/.vscode/settings.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.722099 glyphsets-0.6.9/Archive/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.734099 glyphsets-0.6.9/Archive/GF Glyph Sets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.734099 glyphsets-0.6.9/Archive/GF Glyph Sets/Arabic/
+-rw-r--r--   0 runner    (1001) docker     (127)     4544 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Arabic/GF-arabic-core.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     6134 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Arabic/GF-arabic-plus.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Arabic/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.734099 glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-historical_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-plus-locl_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)    10080 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-plus_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-pro_unique-glyphs.nam
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.722099 glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.734099 glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/historical_unique-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus-locl_unique-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus-locl_unique-glyphs_italic.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus-locl_unique-glyphs_roman.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus_unique-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus_unique-glyphs_core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus_unique-glyphs_smallcaps.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/pro_unique-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/pro_unique-glyphs_smallcaps.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.738099 glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/historical_unique-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus-locl_unique-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus-locl_unique-glyphs_italic.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus-locl_unique-glyphs_roman.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus_unique-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus_unique-glyphs_core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus_unique-glyphs_smallcaps.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/pro_unique-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/pro_unique-glyphs_smallcaps.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6864 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/GF-latin-core_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     6148 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/GF-latin-expert_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)    18371 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/GF-latin-global_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/GF-latin-plus_optional-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)    16079 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/GF-latin-plus_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/GF-latin-pro_optional-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     5442 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/GF-latin-pro_unique-glyphs.nam
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.738099 glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/
+-rw-r--r--   0 runner    (1001) docker     (127)    16666 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/GF-greek-ancient-musical-symbols.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     5589 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/GF-greek-archaic.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     5663 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/GF-greek-coptic.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/GF-greek-core.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     8571 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/GF-greek-expert.nam
+-rw-r--r--   0 runner    (1001) docker     (127)    14827 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/GF-greek-plus.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2776 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/GF-greek-pro.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     7194 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.722099 glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/filter lists/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.742099 glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/filter lists/nice names/
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/filter lists/nice names/ancient-musical-symbols.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/filter lists/nice names/archaic.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/filter lists/nice names/coptic.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/filter lists/nice names/core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5907 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/filter lists/nice names/expert.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5156 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/filter lists/nice names/plus.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/filter lists/nice names/pro.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.742099 glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/filter lists/uni names/
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/filter lists/uni names/ancient-musical-symbols.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/filter lists/uni names/archaic.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/filter lists/uni names/coptic.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/filter lists/uni names/core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3395 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/filter lists/uni names/expert.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/filter lists/uni names/plus.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/filter lists/uni names/pro.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12967 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3667 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/RECOMMENDED.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/TROUBLESHOOTING.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.742099 glyphsets-0.6.9/Archive/GF Glyph Sets/Vietnamese/
+-rw-r--r--   0 runner    (1001) docker     (127)     4482 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Vietnamese/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.742099 glyphsets-0.6.9/Archive/GF Glyph Sets/Vietnamese/img/
+-rw-r--r--   0 runner    (1001) docker     (127)    16279 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Vietnamese/img/VIT_accents.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    75853 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Vietnamese/img/VIT_glyphs.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)   104148 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/Vietnamese/img/locl.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.742099 glyphsets-0.6.9/Archive/GF Glyph Sets/filter lists/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/filter lists/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.746099 glyphsets-0.6.9/Archive/GF Glyph Sets/filter lists/nice names/
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/filter lists/nice names/core_unique-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3414 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/filter lists/nice names/expert_unique-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/filter lists/nice names/plus_optional-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4023 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/filter lists/nice names/plus_unique-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/filter lists/nice names/pro_optional-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/filter lists/nice names/pro_unique-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/filter lists/plus_optional-glyphs_case-accents.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/filter lists/plus_unique-glyphs_vietnamese-all.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/filter lists/plus_unique-glyphs_vietnamese-unique.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/filter lists/pro_optional-glyphs_case-punctuation.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.746099 glyphsets-0.6.9/Archive/GF Glyph Sets/filter lists/uni names/
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/filter lists/uni names/core_unique-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/filter lists/uni names/expert_unique-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/filter lists/uni names/plus_optional-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3123 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/filter lists/uni names/plus_unique-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/filter lists/uni names/pro_optional-glyphs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/filter lists/uni names/pro_unique-glyphs.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.746099 glyphsets-0.6.9/Archive/GF Glyph Sets/glyphTypeSorting/
+-rw-r--r--   0 runner    (1001) docker     (127)     4917 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/glyphTypeSorting/EXPERT_composites_207.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/glyphTypeSorting/EXPERT_drawn_62.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/glyphTypeSorting/EXPERT_either_4.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7831 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/glyphTypeSorting/PLUS_composites_360.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4010 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/glyphTypeSorting/PLUS_drawn_215.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4057 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/glyphTypeSorting/PLUS_drawn_216.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/glyphTypeSorting/PLUS_either_19.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/glyphTypeSorting/PRO_composites_116.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/glyphTypeSorting/PRO_drawn_26.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/glyphTypeSorting/PRO_either_4.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.746099 glyphsets-0.6.9/Archive/GF Glyph Sets/tutorials/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.746099 glyphsets-0.6.9/Archive/GF Glyph Sets/tutorials/Glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)    43666 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/tutorials/Glyphs/CustomFilter.plist
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.746099 glyphsets-0.6.9/Archive/GF Glyph Sets/tutorials/Glyphs/Info/
+-rw-r--r--   0 runner    (1001) docker     (127)    89964 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/tutorials/Glyphs/Info/GlyphData.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     9153 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/tutorials/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.750099 glyphsets-0.6.9/Archive/GF Glyph Sets/tutorials/img/
+-rw-r--r--   0 runner    (1001) docker     (127)    35092 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/tutorials/img/Directory.png
+-rw-r--r--   0 runner    (1001) docker     (127)    98535 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/tutorials/img/ListFilters.png
+-rw-r--r--   0 runner    (1001) docker     (127)    84092 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/tutorials/img/PoiretOne-locl.png
+-rw-r--r--   0 runner    (1001) docker     (127)    24052 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/tutorials/img/ecircumflexacute.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    71431 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/tutorials/img/fix-1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    33541 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/tutorials/img/fix-2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    45217 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/tutorials/img/fix-3.png
+-rw-r--r--   0 runner    (1001) docker     (127)    53065 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/tutorials/img/list-filter-1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7677 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Archive/GF Glyph Sets/tutorials/img/list-filter.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4835 2023-12-15 14:17:45.000000 glyphsets-0.6.9/CHANGELOG.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.750099 glyphsets-0.6.9/GF_glyphsets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.750099 glyphsets-0.6.9/GF_glyphsets/Arabic/
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Arabic/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.750099 glyphsets-0.6.9/GF_glyphsets/Arabic/definitions/
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Arabic/definitions/GF_Arabic_Core.stub.nam
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.750099 glyphsets-0.6.9/GF_glyphsets/Arabic/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)    17968 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Arabic/glyphs/CustomFilter_GF_Arabic.plist
+-rw-r--r--   0 runner    (1001) docker     (127)     6753 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Arabic/glyphs/GF_Arabic_Core.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)     6085 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Arabic/glyphs/GF_Arabic_Plus.glyphs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.750099 glyphsets-0.6.9/GF_glyphsets/Arabic/nam/
+-rw-r--r--   0 runner    (1001) docker     (127)     4056 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Arabic/nam/GF_Arabic_Core.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     3727 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Arabic/nam/GF_Arabic_Plus.nam
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.726099 glyphsets-0.6.9/GF_glyphsets/Arabic/txt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.754099 glyphsets-0.6.9/GF_glyphsets/Arabic/txt/nice-names/
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Arabic/txt/nice-names/GF_Arabic_Core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Arabic/txt/nice-names/GF_Arabic_Plus.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.754099 glyphsets-0.6.9/GF_glyphsets/Arabic/txt/prod-names/
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Arabic/txt/prod-names/GF_Arabic_Core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Arabic/txt/prod-names/GF_Arabic_Plus.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.754099 glyphsets-0.6.9/GF_glyphsets/Cyrillic/
+-rw-r--r--   0 runner    (1001) docker     (127)     4089 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Cyrillic/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.754099 glyphsets-0.6.9/GF_glyphsets/Cyrillic/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)    21454 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Cyrillic/glyphs/CustomFilter_GF_Cyrillic.plist
+-rw-r--r--   0 runner    (1001) docker     (127)    11221 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_Core.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)     5815 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_Historical.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)    11251 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_Plus.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)     4804 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_PlusLoclItalic.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)     5310 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_PlusLoclRoman.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)     7759 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_Pro.glyphs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.754099 glyphsets-0.6.9/GF_glyphsets/Cyrillic/nam/
+-rw-r--r--   0 runner    (1001) docker     (127)     3462 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_Core.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_Historical.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     3956 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_Plus.nam
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_PlusLoclItalic.nam
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_PlusLoclRoman.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_Pro.nam
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.726099 glyphsets-0.6.9/GF_glyphsets/Cyrillic/txt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.758099 glyphsets-0.6.9/GF_glyphsets/Cyrillic/txt/nice-names/
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_Core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_Historical.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_Plus.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_PlusLoclItalic.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_PlusLoclRoman.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_Pro.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.758099 glyphsets-0.6.9/GF_glyphsets/Cyrillic/txt/prod-names/
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Cyrillic/txt/prod-names/GF_Cyrillic_Core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Cyrillic/txt/prod-names/GF_Cyrillic_Historical.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Cyrillic/txt/prod-names/GF_Cyrillic_Plus.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Cyrillic/txt/prod-names/GF_Cyrillic_PlusLoclItalic.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Cyrillic/txt/prod-names/GF_Cyrillic_PlusLoclRoman.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Cyrillic/txt/prod-names/GF_Cyrillic_Pro.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.758099 glyphsets-0.6.9/GF_glyphsets/Greek/
+-rw-r--r--   0 runner    (1001) docker     (127)     7194 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Greek/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.758099 glyphsets-0.6.9/GF_glyphsets/Greek/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)    56423 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Greek/glyphs/CustomFilter_GF_Greek.plist
+-rw-r--r--   0 runner    (1001) docker     (127)    30534 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Greek/glyphs/GF_Greek_AncientMusicalSymbols.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)    16742 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Greek/glyphs/GF_Greek_Archaic.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)    15594 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Greek/glyphs/GF_Greek_Coptic.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)     9091 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Greek/glyphs/GF_Greek_Core.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)    26352 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Greek/glyphs/GF_Greek_Expert.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)    28310 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Greek/glyphs/GF_Greek_Plus.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)    10390 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Greek/glyphs/GF_Greek_Pro.glyphs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.762099 glyphsets-0.6.9/GF_glyphsets/Greek/nam/
+-rw-r--r--   0 runner    (1001) docker     (127)    15006 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Greek/nam/GF_Greek_AncientMusicalSymbols.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     4912 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Greek/nam/GF_Greek_Archaic.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     4550 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Greek/nam/GF_Greek_Coptic.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Greek/nam/GF_Greek_Core.nam
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Greek/nam/GF_Greek_Expert.nam
+-rw-r--r--   0 runner    (1001) docker     (127)    12597 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Greek/nam/GF_Greek_Plus.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Greek/nam/GF_Greek_Pro.nam
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.726099 glyphsets-0.6.9/GF_glyphsets/Greek/txt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.762099 glyphsets-0.6.9/GF_glyphsets/Greek/txt/nice-names/
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Greek/txt/nice-names/GF_Greek_AncientMusicalSymbols.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Archaic.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Coptic.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5906 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Expert.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5155 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Plus.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Pro.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.762099 glyphsets-0.6.9/GF_glyphsets/Greek/txt/prod-names/
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Greek/txt/prod-names/GF_Greek_AncientMusicalSymbols.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Archaic.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Coptic.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3394 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Expert.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Plus.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Pro.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.762099 glyphsets-0.6.9/GF_glyphsets/Latin/
+-rw-r--r--   0 runner    (1001) docker     (127)     8429 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Latin/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.762099 glyphsets-0.6.9/GF_glyphsets/Latin/definitions/
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Latin/definitions/GF_Latin_Core.stub.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Latin/definitions/GF_Latin_Core.stub.nam
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.766099 glyphsets-0.6.9/GF_glyphsets/Latin/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)    38119 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Latin/glyphs/CustomFilter_GF_Latin.plist
+-rw-r--r--   0 runner    (1001) docker     (127)    62282 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Latin/glyphs/GF_Latin_African.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)    19144 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Latin/glyphs/GF_Latin_Beyond.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)    16357 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Latin/glyphs/GF_Latin_Core.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)    16570 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Latin/glyphs/GF_Latin_Kernel.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)    18721 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Latin/glyphs/GF_Latin_Plus.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)    15064 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Latin/glyphs/GF_Latin_Vietnamese.glyphs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.766099 glyphsets-0.6.9/GF_glyphsets/Latin/nam/
+-rw-r--r--   0 runner    (1001) docker     (127)    17738 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Latin/nam/GF_Latin_African.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     5398 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Latin/nam/GF_Latin_Beyond.nam
+-rw-r--r--   0 runner    (1001) docker     (127)    11101 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Latin/nam/GF_Latin_Core.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Latin/nam/GF_Latin_Kernel.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Latin/nam/GF_Latin_Plus.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     4858 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Latin/nam/GF_Latin_Vietnamese.nam
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.726099 glyphsets-0.6.9/GF_glyphsets/Latin/txt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.766099 glyphsets-0.6.9/GF_glyphsets/Latin/txt/nice-names/
+-rw-r--r--   0 runner    (1001) docker     (127)     4637 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Latin/txt/nice-names/GF_Latin_African.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Beyond.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Kernel.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Plus.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Vietnamese.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.770099 glyphsets-0.6.9/GF_glyphsets/Latin/txt/prod-names/
+-rw-r--r--   0 runner    (1001) docker     (127)     3438 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Latin/txt/prod-names/GF_Latin_African.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Beyond.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2549 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Kernel.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Plus.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Vietnamese.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.770099 glyphsets-0.6.9/GF_glyphsets/Phonetics/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Phonetics/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.770099 glyphsets-0.6.9/GF_glyphsets/Phonetics/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)    19280 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Phonetics/glyphs/CustomFilter_GF_Phonetics.plist
+-rw-r--r--   0 runner    (1001) docker     (127)     4478 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_APA.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)     8928 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_DisorderedSpeech.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_IPAHistorical.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)    17764 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_IPAStandard.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)     3395 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_SinoExt.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_UPA.glyphs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.770099 glyphsets-0.6.9/GF_glyphsets/Phonetics/nam/
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Phonetics/nam/GF_Phonetics_APA.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2542 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Phonetics/nam/GF_Phonetics_DisorderedSpeech.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Phonetics/nam/GF_Phonetics_IPAHistorical.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     6119 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Phonetics/nam/GF_Phonetics_IPAStandard.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Phonetics/nam/GF_Phonetics_SinoExt.nam
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Phonetics/nam/GF_Phonetics_UPA.nam
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.726099 glyphsets-0.6.9/GF_glyphsets/Phonetics/txt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.774099 glyphsets-0.6.9/GF_glyphsets/Phonetics/txt/nice-names/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Phonetics/txt/nice-names/GF_Phonetics_APA.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Phonetics/txt/nice-names/GF_Phonetics_DisorderedSpeech.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Phonetics/txt/nice-names/GF_Phonetics_IPAHistorical.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Phonetics/txt/nice-names/GF_Phonetics_IPAStandard.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Phonetics/txt/nice-names/GF_Phonetics_SinoExt.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Phonetics/txt/nice-names/GF_Phonetics_UPA.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.774099 glyphsets-0.6.9/GF_glyphsets/Phonetics/txt/prod-names/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Phonetics/txt/prod-names/GF_Phonetics_APA.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Phonetics/txt/prod-names/GF_Phonetics_DisorderedSpeech.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Phonetics/txt/prod-names/GF_Phonetics_IPAHistorical.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Phonetics/txt/prod-names/GF_Phonetics_IPAStandard.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Phonetics/txt/prod-names/GF_Phonetics_SinoExt.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/Phonetics/txt/prod-names/GF_Phonetics_UPA.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.774099 glyphsets-0.6.9/GF_glyphsets/TransLatin/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/TransLatin/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.774099 glyphsets-0.6.9/GF_glyphsets/TransLatin/glyphs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7427 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/TransLatin/glyphs/CustomFilter_GF_TransLatin.plist
+-rw-r--r--   0 runner    (1001) docker     (127)     6786 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/TransLatin/glyphs/GF_TransLatin_Arabic.glyphs
+-rw-r--r--   0 runner    (1001) docker     (127)    14581 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/TransLatin/glyphs/GF_TransLatin_Pinyin.glyphs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.774099 glyphsets-0.6.9/GF_glyphsets/TransLatin/nam/
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/TransLatin/nam/GF_TransLatin_Arabic.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/TransLatin/nam/GF_TransLatin_Pinyin.nam
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.730099 glyphsets-0.6.9/GF_glyphsets/TransLatin/txt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.774099 glyphsets-0.6.9/GF_glyphsets/TransLatin/txt/nice-names/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/TransLatin/txt/nice-names/GF_TransLatin_Arabic.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/TransLatin/txt/nice-names/GF_TransLatin_Pinyin.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.774099 glyphsets-0.6.9/GF_glyphsets/TransLatin/txt/prod-names/
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/TransLatin/txt/prod-names/GF_TransLatin_Arabic.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/TransLatin/txt/prod-names/GF_TransLatin_Pinyin.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2023-12-15 14:17:45.000000 glyphsets-0.6.9/GF_glyphsets/update-gs.sh
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-12-15 14:17:45.000000 glyphsets-0.6.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.730099 glyphsets-0.6.9/Lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.778099 glyphsets-0.6.9/Lib/glyphsets/
+-rw-r--r--   0 runner    (1001) docker     (127)     9723 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3372 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2023-12-15 14:17:58.000000 glyphsets-0.6.9/Lib/glyphsets/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16554 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/codepoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)   587834 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/data.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.778099 glyphsets-0.6.9/Lib/glyphsets/definitions/
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/definitions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.778099 glyphsets-0.6.9/Lib/glyphsets/definitions/nam/
+-rw-r--r--   0 runner    (1001) docker     (127)     4056 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/definitions/nam/GF_Arabic_Core.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     3727 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/definitions/nam/GF_Arabic_Plus.nam
+-rw-r--r--   0 runner    (1001) docker     (127)    11101 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/definitions/nam/GF_Latin_Core.nam
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.814099 glyphsets-0.6.9/Lib/glyphsets/encodings/
+-rw-r--r--   0 runner    (1001) docker     (127)     7232 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4230 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/adlam_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/ahom_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)    20007 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/anatolian-hieroglyphs_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)    57487 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/arabic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     3688 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/armenian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/avestan_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     4358 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/balinese_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)    22272 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/bamum_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/bassa-vah_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/batak_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     3395 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/bengali_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     3012 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/bhaiksuki_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     3204 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/brahmi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     9037 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/braille_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/buginese_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/buhid_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)    25715 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/canadian-aboriginal_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/carian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/caucasian-albanian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2534 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/chakma_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/cham_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     5389 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/cherokee_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)   284694 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/chinese-hongkong_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)   298348 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/chinese-simplified_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)   241902 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/chinese-traditional_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/chorasmian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     6988 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/coptic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)    46227 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/cuneiform_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/cypriot_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     3518 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/cypro-minoan_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     5503 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/cyrillic-ext_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/cyrillic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/deseret_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     7837 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/devanagari_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/dives-akuru_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/dogra_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     4776 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/duployan_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)    41018 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/egyptian-hieroglyphs_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/elbasan_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/elymaic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)    33746 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/emoji_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)    16949 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/ethiopic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     7001 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/georgian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     5502 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/glagolitic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/gothic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     3473 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/grantha_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)    13891 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/greek-ext_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     5381 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/greek_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     3677 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/gujarati_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/gunjala-gondi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/gurmukhi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/hanifi-rohingya_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/hanunoo_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/hatran_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     3793 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/hebrew_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/imperial-aramaic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/indic-siyaq-numbers_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/inscriptional-pahlavi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/inscriptional-parthian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)    91251 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/japanese_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2861 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/javanese_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2662 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/kaithi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     3112 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/kannada_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/kawi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/kayah-li_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/kharoshthi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)    21734 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/khitan-small-script_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     7970 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/khmer_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/khojki_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/khudawadi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)    80178 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/korean_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/lao_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)    37362 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/latin-ext_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     7898 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/latin_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/lepcha_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/limbu_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     9503 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/linear-a_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     9214 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/linear-b_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/lisu_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/lycian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/lydian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/mahajani_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/makasar_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     4477 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/malayalam_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/mandaic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/manichaean_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/marchen_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/masaram-gondi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)   190939 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/math.nam
+-rw-r--r--   0 runner    (1001) docker     (127)    95179 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/math_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/mayan-numerals_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     3293 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/medefaidrin_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/meetei-mayek_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     8592 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/mende-kikakui_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/meroitic-cursive_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/meroitic-hieroglyphs_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     5231 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/meroitic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     4051 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/miao_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2508 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/modi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     7491 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/mongolian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/mro_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/multani_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)    24495 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/music_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     7463 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/myanmar_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/nabataean_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/nag-mundari_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2998 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/nandinagari_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/new-tai-lue_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/newa_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/nko_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)    13878 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/nushu_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/nyiakeng-puachue-hmong_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/ogham_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/ol-chiki_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     4526 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/old-hungarian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/old-italic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/old-north-arabian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/old-permic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/old-persian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/old-sogdian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/old-south-arabian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2766 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/old-turkic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/old-uyghur_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2687 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/oriya_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/osage_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/osmanya_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/ottoman-siyaq-numbers_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     4508 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/pahawh-hmong_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/palmyrene_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/pau-cin-hau_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/phags-pa_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/phoenician_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/psalter-pahlavi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/rejang_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/runic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/samaritan_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/saurashtra_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/sharada_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/shavian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/siddham_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)    35208 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/signwriting_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     4834 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/sinhala_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/sogdian_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/sora-sompeng_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2666 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/soyombo_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/sundanese_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/syloti-nagri_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)   118220 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/symbols_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     4168 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/syriac_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/tagalog_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/tagbanwa_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/tai-le_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/tai-tham_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/tai-viet_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/takri_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/tamil-supplement_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/tamil_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2941 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/tangsa_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)   212192 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/tangut_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     3171 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/telugu_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/thaana_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/thai_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     7175 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/tibetan_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/tifinagh_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     3115 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/tirhuta_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/toto_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/ugaritic_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     7189 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/vai_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     5794 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/vietnamese_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/vithkuqi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/wancho_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/warang-citi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     5193 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/wgl-latin.enc
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/yezidi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)    30939 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/yi_unique-glyphs.nam
+-rw-r--r--   0 runner    (1001) docker     (127)     2874 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/encodings/zanabazar-square_unique-glyphs.nam
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.822099 glyphsets-0.6.9/Lib/glyphsets/slices/
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/slices/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)  1087488 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/slices/hongkong-chinese_default.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   893039 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/slices/japanese_default.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   876086 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/slices/korean_default.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   889189 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/slices/simplified-chinese_default.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   904276 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/slices/traditional-chinese_default.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/subsets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2023-12-15 14:17:45.000000 glyphsets-0.6.9/Lib/glyphsets/test_strings.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.826099 glyphsets-0.6.9/Lib/glyphsets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7948 2023-12-15 14:17:58.000000 glyphsets-0.6.9/Lib/glyphsets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    23873 2023-12-15 14:17:58.000000 glyphsets-0.6.9/Lib/glyphsets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-15 14:17:58.000000 glyphsets-0.6.9/Lib/glyphsets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2023-12-15 14:17:58.000000 glyphsets-0.6.9/Lib/glyphsets.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-15 14:17:58.000000 glyphsets-0.6.9/Lib/glyphsets.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2023-12-15 14:17:58.000000 glyphsets-0.6.9/Lib/glyphsets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2023-12-15 14:17:58.000000 glyphsets-0.6.9/Lib/glyphsets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7948 2023-12-15 14:17:58.826099 glyphsets-0.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7169 2023-12-15 14:17:45.000000 glyphsets-0.6.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2023-12-15 14:17:45.000000 glyphsets-0.6.9/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.822099 glyphsets-0.6.9/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     7077 2023-12-15 14:17:45.000000 glyphsets-0.6.9/scripts/assemble_charactersets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2023-12-15 14:17:45.000000 glyphsets-0.6.9/scripts/assemble_languages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2023-12-15 14:17:45.000000 glyphsets-0.6.9/scripts/create-glyphset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2023-12-15 14:17:45.000000 glyphsets-0.6.9/scripts/find_language_for_character.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-15 14:17:58.826099 glyphsets-0.6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2023-12-15 14:17:45.000000 glyphsets-0.6.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.826099 glyphsets-0.6.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1501 2023-12-15 14:17:45.000000 glyphsets-0.6.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 14:17:58.826099 glyphsets-0.6.9/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    90712 2023-12-15 14:17:45.000000 glyphsets-0.6.9/tests/data/MavenPro[wght].ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     4264 2023-12-15 14:17:45.000000 glyphsets-0.6.9/tests/test_glyphdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2023-12-15 14:17:45.000000 glyphsets-0.6.9/tests/test_glyphsets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2023-12-15 14:17:45.000000 glyphsets-0.6.9/tests/test_teststrings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2023-12-15 14:17:45.000000 glyphsets-0.6.9/tests/test_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4132 2023-12-15 14:17:45.000000 glyphsets-0.6.9/tests/testcoverage.py
```

### Comparing `glyphsets-0.6.8/.github/workflows/publish-release.yml` & `glyphsets-0.6.9/.github/workflows/publish-release.yml`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/.github/workflows/test.yml` & `glyphsets-0.6.9/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/Arabic/GF-arabic-core.nam` & `glyphsets-0.6.9/Archive/GF Glyph Sets/Arabic/GF-arabic-core.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/Arabic/GF-arabic-plus.nam` & `glyphsets-0.6.9/Archive/GF Glyph Sets/Arabic/GF-arabic-plus.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/Arabic/README.md` & `glyphsets-0.6.9/Archive/GF Glyph Sets/Arabic/README.md`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-historical_unique-glyphs.nam` & `glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-historical_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-plus-locl_unique-glyphs.nam` & `glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-plus-locl_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-plus_unique-glyphs.nam` & `glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-plus_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-pro_unique-glyphs.nam` & `glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/GF-cyrillic-pro_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus-locl_unique-glyphs.txt` & `glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus-locl_unique-glyphs.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus-locl_unique-glyphs_roman.txt` & `glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus-locl_unique-glyphs_roman.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus_unique-glyphs.txt` & `glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus_unique-glyphs.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus_unique-glyphs_core.txt` & `glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus_unique-glyphs_core.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus_unique-glyphs_smallcaps.txt` & `glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/plus_unique-glyphs_smallcaps.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/pro_unique-glyphs.txt` & `glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/nice names/pro_unique-glyphs.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus-locl_unique-glyphs.txt` & `glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus-locl_unique-glyphs.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus-locl_unique-glyphs_roman.txt` & `glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus-locl_unique-glyphs_roman.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus_unique-glyphs.txt` & `glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus_unique-glyphs.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus_unique-glyphs_core.txt` & `glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus_unique-glyphs_core.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus_unique-glyphs_smallcaps.txt` & `glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/plus_unique-glyphs_smallcaps.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/pro_unique-glyphs.txt` & `glyphsets-0.6.9/Archive/GF Glyph Sets/Cyrillic/filter lists/uni names/pro_unique-glyphs.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/GF-latin-core_unique-glyphs.nam` & `glyphsets-0.6.9/Archive/GF Glyph Sets/GF-latin-core_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/GF-latin-expert_unique-glyphs.nam` & `glyphsets-0.6.9/Archive/GF Glyph Sets/GF-latin-expert_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/GF-latin-global_unique-glyphs.nam` & `glyphsets-0.6.9/Archive/GF Glyph Sets/GF-latin-global_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/GF-latin-plus_optional-glyphs.nam` & `glyphsets-0.6.9/Archive/GF Glyph Sets/GF-latin-plus_optional-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/GF-latin-plus_unique-glyphs.nam` & `glyphsets-0.6.9/Archive/GF Glyph Sets/GF-latin-plus_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/GF-latin-pro_optional-glyphs.nam` & `glyphsets-0.6.9/Archive/GF Glyph Sets/GF-latin-pro_optional-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/GF-latin-pro_unique-glyphs.nam` & `glyphsets-0.6.9/Archive/GF Glyph Sets/GF-latin-pro_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/Greek/GF-greek-ancient-musical-symbols.nam` & `glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/GF-greek-ancient-musical-symbols.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/Greek/GF-greek-archaic.nam` & `glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/GF-greek-archaic.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/Greek/GF-greek-coptic.nam` & `glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/GF-greek-coptic.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/Greek/GF-greek-core.nam` & `glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/GF-greek-core.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/Greek/GF-greek-expert.nam` & `glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/GF-greek-expert.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/Greek/GF-greek-plus.nam` & `glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/GF-greek-plus.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/Greek/GF-greek-pro.nam` & `glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/GF-greek-pro.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/Greek/README.md` & `glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/README.md`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/Greek/filter lists/nice names/ancient-musical-symbols.txt` & `glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/filter lists/nice names/ancient-musical-symbols.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/Greek/filter lists/nice names/archaic.txt` & `glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/filter lists/nice names/archaic.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/Greek/filter lists/nice names/coptic.txt` & `glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/filter lists/nice names/coptic.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/Greek/filter lists/nice names/core.txt` & `glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/filter lists/nice names/core.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/Greek/filter lists/nice names/expert.txt` & `glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/filter lists/nice names/expert.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/Greek/filter lists/nice names/plus.txt` & `glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/filter lists/nice names/plus.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/Greek/filter lists/nice names/pro.txt` & `glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/filter lists/nice names/pro.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/Greek/filter lists/uni names/ancient-musical-symbols.txt` & `glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/filter lists/uni names/ancient-musical-symbols.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/Greek/filter lists/uni names/archaic.txt` & `glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/filter lists/uni names/archaic.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/Greek/filter lists/uni names/coptic.txt` & `glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/filter lists/uni names/coptic.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/Greek/filter lists/uni names/core.txt` & `glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/filter lists/uni names/core.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/Greek/filter lists/uni names/expert.txt` & `glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/filter lists/uni names/expert.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/Greek/filter lists/uni names/plus.txt` & `glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/filter lists/uni names/plus.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/Greek/filter lists/uni names/pro.txt` & `glyphsets-0.6.9/Archive/GF Glyph Sets/Greek/filter lists/uni names/pro.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/README.md` & `glyphsets-0.6.9/Archive/GF Glyph Sets/README.md`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/RECOMMENDED.md` & `glyphsets-0.6.9/Archive/GF Glyph Sets/RECOMMENDED.md`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/TROUBLESHOOTING.md` & `glyphsets-0.6.9/Archive/GF Glyph Sets/TROUBLESHOOTING.md`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/Vietnamese/README.md` & `glyphsets-0.6.9/Archive/GF Glyph Sets/Vietnamese/README.md`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/Vietnamese/img/VIT_accents.jpg` & `glyphsets-0.6.9/Archive/GF Glyph Sets/Vietnamese/img/VIT_accents.jpg`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/Vietnamese/img/VIT_glyphs.jpg` & `glyphsets-0.6.9/Archive/GF Glyph Sets/Vietnamese/img/VIT_glyphs.jpg`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/Vietnamese/img/locl.png` & `glyphsets-0.6.9/Archive/GF Glyph Sets/Vietnamese/img/locl.png`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/filter lists/nice names/core_unique-glyphs.txt` & `glyphsets-0.6.9/Archive/GF Glyph Sets/filter lists/nice names/core_unique-glyphs.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/filter lists/nice names/expert_unique-glyphs.txt` & `glyphsets-0.6.9/Archive/GF Glyph Sets/filter lists/nice names/expert_unique-glyphs.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/filter lists/nice names/plus_unique-glyphs.txt` & `glyphsets-0.6.9/Archive/GF Glyph Sets/filter lists/nice names/plus_unique-glyphs.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/filter lists/nice names/pro_unique-glyphs.txt` & `glyphsets-0.6.9/Archive/GF Glyph Sets/filter lists/nice names/pro_unique-glyphs.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/filter lists/plus_unique-glyphs_vietnamese-all.txt` & `glyphsets-0.6.9/Archive/GF Glyph Sets/filter lists/plus_unique-glyphs_vietnamese-all.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/filter lists/plus_unique-glyphs_vietnamese-unique.txt` & `glyphsets-0.6.9/Archive/GF Glyph Sets/filter lists/plus_unique-glyphs_vietnamese-unique.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/filter lists/uni names/core_unique-glyphs.txt` & `glyphsets-0.6.9/Archive/GF Glyph Sets/filter lists/uni names/core_unique-glyphs.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/filter lists/uni names/expert_unique-glyphs.txt` & `glyphsets-0.6.9/Archive/GF Glyph Sets/filter lists/uni names/expert_unique-glyphs.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/filter lists/uni names/plus_unique-glyphs.txt` & `glyphsets-0.6.9/Archive/GF Glyph Sets/filter lists/uni names/plus_unique-glyphs.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/filter lists/uni names/pro_unique-glyphs.txt` & `glyphsets-0.6.9/Archive/GF Glyph Sets/filter lists/uni names/pro_unique-glyphs.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/glyphTypeSorting/EXPERT_composites_207.txt` & `glyphsets-0.6.9/Archive/GF Glyph Sets/glyphTypeSorting/EXPERT_composites_207.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/glyphTypeSorting/EXPERT_drawn_62.txt` & `glyphsets-0.6.9/Archive/GF Glyph Sets/glyphTypeSorting/EXPERT_drawn_62.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/glyphTypeSorting/PLUS_composites_360.txt` & `glyphsets-0.6.9/Archive/GF Glyph Sets/glyphTypeSorting/PLUS_composites_360.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/glyphTypeSorting/PLUS_drawn_215.txt` & `glyphsets-0.6.9/Archive/GF Glyph Sets/glyphTypeSorting/PLUS_drawn_215.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/glyphTypeSorting/PLUS_drawn_216.txt` & `glyphsets-0.6.9/Archive/GF Glyph Sets/glyphTypeSorting/PLUS_drawn_216.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/glyphTypeSorting/PRO_composites_116.txt` & `glyphsets-0.6.9/Archive/GF Glyph Sets/glyphTypeSorting/PRO_composites_116.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/glyphTypeSorting/PRO_drawn_26.txt` & `glyphsets-0.6.9/Archive/GF Glyph Sets/glyphTypeSorting/PRO_drawn_26.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/tutorials/Glyphs/CustomFilter.plist` & `glyphsets-0.6.9/Archive/GF Glyph Sets/tutorials/Glyphs/CustomFilter.plist`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/tutorials/Glyphs/Info/GlyphData.xml` & `glyphsets-0.6.9/Archive/GF Glyph Sets/tutorials/Glyphs/Info/GlyphData.xml`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/tutorials/README.md` & `glyphsets-0.6.9/Archive/GF Glyph Sets/tutorials/README.md`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/tutorials/img/Directory.png` & `glyphsets-0.6.9/Archive/GF Glyph Sets/tutorials/img/Directory.png`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/tutorials/img/ListFilters.png` & `glyphsets-0.6.9/Archive/GF Glyph Sets/tutorials/img/ListFilters.png`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/tutorials/img/PoiretOne-locl.png` & `glyphsets-0.6.9/Archive/GF Glyph Sets/tutorials/img/PoiretOne-locl.png`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/tutorials/img/ecircumflexacute.jpg` & `glyphsets-0.6.9/Archive/GF Glyph Sets/tutorials/img/ecircumflexacute.jpg`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/tutorials/img/fix-1.png` & `glyphsets-0.6.9/Archive/GF Glyph Sets/tutorials/img/fix-1.png`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/tutorials/img/fix-2.png` & `glyphsets-0.6.9/Archive/GF Glyph Sets/tutorials/img/fix-2.png`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/tutorials/img/fix-3.png` & `glyphsets-0.6.9/Archive/GF Glyph Sets/tutorials/img/fix-3.png`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/tutorials/img/list-filter-1.png` & `glyphsets-0.6.9/Archive/GF Glyph Sets/tutorials/img/list-filter-1.png`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Archive/GF Glyph Sets/tutorials/img/list-filter.png` & `glyphsets-0.6.9/Archive/GF Glyph Sets/tutorials/img/list-filter.png`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/CHANGELOG.md` & `glyphsets-0.6.9/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Arabic/README.md` & `glyphsets-0.6.9/GF_glyphsets/Arabic/README.md`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Arabic/glyphs/CustomFilter_GF_Arabic.plist` & `glyphsets-0.6.9/GF_glyphsets/Arabic/glyphs/CustomFilter_GF_Arabic.plist`

 * *Files 9% similar despite different names*

#### Comparing `glyphsets-0.6.8/GF_glyphsets/Arabic/glyphs/CustomFilter_GF_Arabic.plist` & `glyphsets-0.6.9/GF_glyphsets/Arabic/glyphs/CustomFilter_GF_Arabic.plist`

```diff
@@ -343,207 +343,294 @@
       </array>
       <key>name</key>
       <string>GF_Latin_Core</string>
     </dict>
     <dict>
       <key>list</key>
       <array>
+        <string>space</string>
+        <string>exclam</string>
+        <string>quotedbl</string>
+        <string>numbersign</string>
+        <string>percent</string>
+        <string>quotesingle</string>
+        <string>parenleft</string>
+        <string>parenright</string>
+        <string>asterisk</string>
+        <string>plus</string>
+        <string>comma</string>
+        <string>hyphen</string>
+        <string>period</string>
+        <string>slash</string>
+        <string>zero</string>
+        <string>one</string>
+        <string>two</string>
+        <string>three</string>
+        <string>four</string>
+        <string>five</string>
+        <string>six</string>
+        <string>seven</string>
+        <string>eight</string>
+        <string>nine</string>
+        <string>colon</string>
+        <string>less</string>
+        <string>equal</string>
+        <string>greater</string>
+        <string>bracketleft</string>
+        <string>backslash</string>
+        <string>bracketright</string>
+        <string>braceleft</string>
+        <string>bar</string>
+        <string>braceright</string>
+        <string>nbspace</string>
+        <string>guillemetleft</string>
+        <string>guillemetright</string>
+        <string>multiply</string>
+        <string>divide</string>
+        <string>perthousand-ar</string>
+        <string>comma-ar</string>
+        <string>dateseparator-ar</string>
+        <string>semicolon-ar</string>
+        <string>mark-ar</string>
+        <string>question-ar</string>
         <string>hamza-ar</string>
-        <string>alef-ar</string>
+        <string>alefMadda-ar</string>
         <string>alefHamzaabove-ar</string>
+        <string>wawHamzaabove-ar</string>
         <string>alefHamzabelow-ar</string>
-        <string>alefMadda-ar</string>
+        <string>yehHamzaabove-ar</string>
+        <string>alef-ar</string>
         <string>beh-ar</string>
-        <string>peh-ar</string>
+        <string>tehMarbuta-ar</string>
         <string>teh-ar</string>
         <string>theh-ar</string>
-        <string>tteh-ar</string>
         <string>jeem-ar</string>
-        <string>tcheh-ar</string>
         <string>hah-ar</string>
         <string>khah-ar</string>
         <string>dal-ar</string>
         <string>thal-ar</string>
-        <string>ddal-ar</string>
         <string>reh-ar</string>
         <string>zain-ar</string>
-        <string>rreh-ar</string>
         <string>seen-ar</string>
         <string>sheen-ar</string>
         <string>sad-ar</string>
         <string>dad-ar</string>
         <string>tah-ar</string>
         <string>zah-ar</string>
         <string>ain-ar</string>
         <string>ghain-ar</string>
+        <string>kashida-ar</string>
         <string>feh-ar</string>
-        <string>veh-ar</string>
-        <string>fehDotmovedbelow-ar</string>
-        <string>fehThreedotsbelow-ar</string>
         <string>qaf-ar</string>
-        <string>qafDotabove-ar</string>
-        <string>qafThreedotsabove-ar</string>
         <string>kaf-ar</string>
-        <string>keheh-ar</string>
-        <string>kehehThreedotsabove-ar</string>
-        <string>gaf-ar</string>
-        <string>ng-ar</string>
         <string>lam-ar</string>
         <string>meem-ar</string>
         <string>noon-ar</string>
-        <string>noonghunna-ar</string>
         <string>heh-ar</string>
-        <string>hehHamzaabove-ar</string>
-        <string>hehgoal-ar</string>
-        <string>hehgoalHamzaabove-ar</string>
-        <string>hehDoachashmee-ar</string>
-        <string>tehMarbuta-ar</string>
-        <string>tehMarbutagoal-ar</string>
         <string>waw-ar</string>
-        <string>wawHamzaabove-ar</string>
         <string>alefMaksura-ar</string>
         <string>yeh-ar</string>
-        <string>yehHamzaabove-ar</string>
-        <string>yehFarsi-ar</string>
-        <string>yehbarree-ar</string>
-        <string>yehbarreeHamzaabove-ar</string>
-        <string>ae-ar</string>
-        <string>kashida-ar</string>
-        <string>decimalseparator-ar</string>
-        <string>thousandseparator-ar</string>
+        <string>fathatan-ar</string>
+        <string>dammatan-ar</string>
+        <string>kasratan-ar</string>
+        <string>fatha-ar</string>
+        <string>damma-ar</string>
+        <string>kasra-ar</string>
+        <string>shadda-ar</string>
+        <string>sukun-ar</string>
+        <string>madda-ar</string>
+        <string>hamzaabove-ar</string>
+        <string>hamzabelow-ar</string>
         <string>zero-ar</string>
         <string>one-ar</string>
         <string>two-ar</string>
         <string>three-ar</string>
         <string>four-ar</string>
         <string>five-ar</string>
         <string>six-ar</string>
         <string>seven-ar</string>
         <string>eight-ar</string>
         <string>nine-ar</string>
-        <string>zeroFarsi-ar</string>
-        <string>oneFarsi-ar</string>
-        <string>twoFarsi-ar</string>
-        <string>threeFarsi-ar</string>
-        <string>fourFarsi-ar</string>
-        <string>fiveFarsi-ar</string>
-        <string>sixFarsi-ar</string>
-        <string>sevenFarsi-ar</string>
-        <string>eightFarsi-ar</string>
-        <string>nineFarsi-ar</string>
+        <string>percent-ar</string>
+        <string>decimalseparator-ar</string>
+        <string>thousandseparator-ar</string>
+        <string>asterisk-ar</string>
+        <string>alefabove-ar</string>
+        <string>tteh-ar</string>
+        <string>peh-ar</string>
+        <string>tcheh-ar</string>
+        <string>ddal-ar</string>
+        <string>rreh-ar</string>
+        <string>jeh-ar</string>
+        <string>keheh-ar</string>
+        <string>gaf-ar</string>
+        <string>hehDoachashmee-ar</string>
+        <string>hehgoal-ar</string>
+        <string>yeh-farsi</string>
+        <string>yehbarree-ar</string>
+        <string>fullstop-ar</string>
+        <string>zero-persian</string>
+        <string>one-persian</string>
+        <string>two-persian</string>
+        <string>three-persian</string>
+        <string>four-persian</string>
+        <string>five-persian</string>
+        <string>six-persian</string>
+        <string>seven-persian</string>
+        <string>eight-persian</string>
+        <string>nine-persian</string>
+        <string>kehehThreedotsabove-ar</string>
+        <string>lefttorightmark</string>
+        <string>endash</string>
+        <string>emdash</string>
+        <string>quoteleft</string>
+        <string>quoteright</string>
+        <string>quotedblleft</string>
+        <string>quotedblright</string>
+        <string>ellipsis</string>
+        <string>guilsinglleft</string>
+        <string>guilsinglright</string>
+        <string>minus</string>
+        <string>parenleft-ar</string>
+        <string>parenright-ar</string>
+      </array>
+      <key>name</key>
+      <string>GF_Arabic_Core</string>
+    </dict>
+    <dict>
+      <key>list</key>
+      <array>
+        <string>exclam</string>
+        <string>percent</string>
+        <string>quotesingle</string>
+        <string>parenleft</string>
+        <string>parenright</string>
+        <string>plus</string>
+        <string>comma</string>
+        <string>hyphen</string>
+        <string>period</string>
+        <string>slash</string>
         <string>zero</string>
         <string>one</string>
         <string>two</string>
         <string>three</string>
         <string>four</string>
         <string>five</string>
         <string>six</string>
         <string>seven</string>
         <string>eight</string>
         <string>nine</string>
-        <string>space</string>
-        <string>nbspace</string>
-        <string>fullstop-ar</string>
-        <string>comma-ar</string>
-        <string>semicolon-ar</string>
-        <string>question-ar</string>
-        <string>asterisk-ar</string>
-        <string>period</string>
         <string>colon</string>
-        <string>ellipsis</string>
-        <string>exclam</string>
-        <string>asterisk</string>
-        <string>numbersign</string>
-        <string>slash</string>
-        <string>backslash</string>
-        <string>hyphen</string>
-        <string>parenleft</string>
-        <string>parenright</string>
-        <string>braceleft</string>
-        <string>braceright</string>
+        <string>semicolon</string>
         <string>bracketleft</string>
         <string>bracketright</string>
-        <string>quotedblleft</string>
-        <string>quotedblright</string>
-        <string>quoteleft</string>
-        <string>quoteright</string>
-        <string>guillemetleft</string>
-        <string>guillemetright</string>
-        <string>quotedbl</string>
-        <string>quotesingle</string>
-        <string>percent-ar</string>
-        <string>bar</string>
-        <string>plus</string>
-        <string>multiply</string>
-        <string>divide</string>
-        <string>equal</string>
-        <string>greater</string>
-        <string>less</string>
-        <string>percent</string>
-        <string>hamzaabove-ar</string>
-        <string>hamzabelow-ar</string>
+        <string>perthousand-ar</string>
+        <string>comma-ar</string>
+        <string>hamza-ar</string>
+        <string>alefMadda-ar</string>
+        <string>alefHamzaabove-ar</string>
+        <string>wawHamzaabove-ar</string>
+        <string>yehHamzaabove-ar</string>
+        <string>alef-ar</string>
+        <string>beh-ar</string>
+        <string>tehMarbuta-ar</string>
+        <string>teh-ar</string>
+        <string>theh-ar</string>
+        <string>jeem-ar</string>
+        <string>hah-ar</string>
+        <string>khah-ar</string>
+        <string>dal-ar</string>
+        <string>thal-ar</string>
+        <string>reh-ar</string>
+        <string>zain-ar</string>
+        <string>seen-ar</string>
+        <string>sheen-ar</string>
+        <string>sad-ar</string>
+        <string>dad-ar</string>
+        <string>tah-ar</string>
+        <string>zah-ar</string>
+        <string>ain-ar</string>
+        <string>ghain-ar</string>
+        <string>feh-ar</string>
+        <string>qaf-ar</string>
+        <string>kaf-ar</string>
+        <string>lam-ar</string>
+        <string>meem-ar</string>
+        <string>noon-ar</string>
+        <string>heh-ar</string>
+        <string>waw-ar</string>
+        <string>alefMaksura-ar</string>
+        <string>yeh-ar</string>
         <string>fathatan-ar</string>
         <string>dammatan-ar</string>
         <string>kasratan-ar</string>
         <string>fatha-ar</string>
         <string>damma-ar</string>
         <string>kasra-ar</string>
         <string>shadda-ar</string>
         <string>sukun-ar</string>
-        <string>madda-ar</string>
-        <string>uni069COVE</string>
-      </array>
-      <key>name</key>
-      <string>GF_Arabic_Core</string>
-    </dict>
-    <dict>
-      <key>list</key>
-      <array>
-        <string>highhamza-ar</string>
-        <string>beeh-ar</string>
-        <string>beheh-ar</string>
+        <string>hamzaabove-ar</string>
+        <string>zero-ar</string>
+        <string>one-ar</string>
+        <string>two-ar</string>
+        <string>three-ar</string>
+        <string>four-ar</string>
+        <string>five-ar</string>
+        <string>six-ar</string>
+        <string>seven-ar</string>
+        <string>eight-ar</string>
+        <string>nine-ar</string>
+        <string>percent-ar</string>
+        <string>decimalseparator-ar</string>
+        <string>thousandseparator-ar</string>
+        <string>alefabove-ar</string>
         <string>tehRing-ar</string>
-        <string>tehThreedotsdown-ar</string>
-        <string>tteheh-ar</string>
-        <string>teheh-ar</string>
-        <string>tcheheh-ar</string>
-        <string>nyeh-ar</string>
-        <string>dyeh-ar</string>
+        <string>peh-ar</string>
         <string>hahHamzaabove-ar</string>
         <string>hahThreedotsabove-ar</string>
-        <string>dahal-ar</string>
-        <string>ddahal-ar</string>
+        <string>tcheh-ar</string>
         <string>dalRing-ar</string>
-        <string>dalDotbelow-ar</string>
-        <string>dalThreedotsdown-ar</string>
         <string>rehRing-ar</string>
         <string>rehVbelow-ar</string>
         <string>rehDotbelowdotabove-ar</string>
-        <string>rehFourdots-ar</string>
+        <string>jeh-ar</string>
         <string>seenDotbelowDotabove-ar</string>
-        <string>sheenThreedotsbelow-ar</string>
-        <string>ainThreedots-ar</string>
-        <string>peheh-ar</string>
-        <string>kehehDotabove-ar</string>
-        <string>kafswash-ar</string>
+        <string>veh-ar</string>
+        <string>keheh-ar</string>
         <string>kafRing-ar</string>
-        <string>ngoeh-ar</string>
-        <string>gueh-ar</string>
+        <string>ng-ar</string>
+        <string>gaf-ar</string>
         <string>lamVabove-ar</string>
-        <string>rnoon-ar</string>
         <string>noonRing-ar</string>
-        <string>noonThreedotsabove-ar</string>
-        <string>wawDotabove-ar</string>
+        <string>hehDoachashmee-ar</string>
         <string>oe-ar</string>
         <string>u-ar</string>
         <string>yu-ar</string>
         <string>ve-ar</string>
-        <string>yehVabove-ar</string>
+        <string>yeh-farsi</string>
         <string>yehTail-ar</string>
+        <string>yehVabove-ar</string>
         <string>e-ar</string>
-        <string>fathaHorizont-ar</string>
+        <string>fullstop-ar</string>
+        <string>ae-ar</string>
+        <string>zero-persian</string>
+        <string>one-persian</string>
+        <string>two-persian</string>
+        <string>three-persian</string>
+        <string>four-persian</string>
+        <string>five-persian</string>
+        <string>six-persian</string>
+        <string>seven-persian</string>
+        <string>eight-persian</string>
+        <string>nine-persian</string>
+        <string>sindhiampersand-ar</string>
+        <string>sindhipostpositionmen-ar</string>
+        <string>lefttorightmark</string>
+        <string>righttoleftmark</string>
+        <string>quoteleft</string>
+        <string>minus</string>
       </array>
       <key>name</key>
       <string>GF_Arabic_Plus</string>
     </dict>
   </array>
 </plist>
```

### Comparing `glyphsets-0.6.8/GF_glyphsets/Arabic/glyphs/GF_Arabic_Core.glyphs` & `glyphsets-0.6.9/GF_glyphsets/Greek/glyphs/GF_Greek_Archaic.glyphs`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {
 .appVersion = "3124";
 .formatVersion = 3;
 date = "2021-10-28 12:22:31 +0000";
-familyName = "GF Arabic Core";
+familyName = "GF Greek Archaic";
 featurePrefixes = (
 {
 automatic = 1;
 code = "languagesystem DFLT dflt;
 
 languagesystem latn dflt;
 languagesystem latn AZE;
@@ -118,1451 +118,1442 @@
 }
 );
 name = Regular;
 }
 );
 glyphs = (
 {
-glyphname = "hamza-ar";
+glyphname = Heta;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1569;
+unicode = 880;
 },
 {
-glyphname = "alef-ar";
+glyphname = Archaicsampi;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1575;
+unicode = 882;
 },
 {
-glyphname = "alefHamzaabove-ar";
+glyphname = Pamphyliandigamma;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1571;
+unicode = 886;
 },
 {
-glyphname = "alefHamzabelow-ar";
+glyphname = KoppaArchaic;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1573;
+unicode = 984;
 },
 {
-glyphname = "alefMadda-ar";
+glyphname = UpsilonhookSymbol;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1570;
+unicode = 978;
 },
 {
-glyphname = "beh-ar";
+glyphname = UpsilonacutehookSymbol;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1576;
+unicode = 979;
 },
 {
-glyphname = "peh-ar";
+glyphname = UpsilondieresishookSymbol;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1662;
+unicode = 980;
 },
 {
-glyphname = "teh-ar";
+glyphname = ThetaSymbol;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1578;
+unicode = 1012;
 },
 {
-glyphname = "theh-ar";
+glyphname = Sho;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1579;
+unicode = 1015;
 },
 {
-glyphname = "tteh-ar";
+glyphname = SigmaLunateSymbol;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1657;
+unicode = 1017;
 },
 {
-glyphname = "jeem-ar";
+glyphname = San;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1580;
+unicode = 1018;
 },
 {
-glyphname = "tcheh-ar";
+glyphname = SigmaLunateReversedSymbol;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1670;
+unicode = 1021;
 },
 {
-glyphname = "hah-ar";
+glyphname = SigmaLunateDottedSymbol;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1581;
+unicode = 1022;
 },
 {
-glyphname = "khah-ar";
+glyphname = SigmaLunateDottedReversedSymbol;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1582;
+unicode = 1023;
 },
 {
-glyphname = "dal-ar";
+glyphname = heta;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1583;
+unicode = 881;
 },
 {
-glyphname = "thal-ar";
+glyphname = archaicsampi;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1584;
+unicode = 883;
 },
 {
-glyphname = "ddal-ar";
+glyphname = pamphyliandigamma;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1672;
+unicode = 887;
 },
 {
-glyphname = "reh-ar";
+glyphname = sigmaLunateReversedSymbol;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1585;
+unicode = 891;
 },
 {
-glyphname = "zain-ar";
+glyphname = sigmaLunateDottedSymbol;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1586;
+unicode = 892;
 },
 {
-glyphname = "rreh-ar";
+glyphname = sigmaLunateDottedReversedSymbol;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1681;
+unicode = 893;
 },
 {
-glyphname = "seen-ar";
+glyphname = koppaArchaic;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1587;
+unicode = 985;
 },
 {
-glyphname = "sheen-ar";
+glyphname = betaSymbol;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1588;
+unicode = 976;
 },
 {
-glyphname = "sad-ar";
+glyphname = thetaSymbol;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1589;
+unicode = 977;
 },
 {
-glyphname = "dad-ar";
+glyphname = phiSymbol;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1590;
+unicode = 981;
 },
 {
-glyphname = "tah-ar";
+glyphname = piSymbol;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1591;
+unicode = 982;
 },
 {
-glyphname = "zah-ar";
+glyphname = kappaSymbol;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1592;
+unicode = 1008;
 },
 {
-glyphname = "ain-ar";
+glyphname = rhoSymbol;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1593;
+unicode = 1009;
 },
 {
-glyphname = "ghain-ar";
+glyphname = sigmaLunateSymbol;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1594;
+unicode = 1010;
 },
 {
-glyphname = "feh-ar";
+glyphname = yot;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1601;
+unicode = 1011;
 },
 {
-glyphname = "veh-ar";
+glyphname = epsilonLunateSymbol;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1700;
+unicode = 1013;
 },
 {
-glyphname = "fehDotmovedbelow-ar";
+glyphname = sho;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1698;
+unicode = 1016;
 },
 {
-glyphname = "fehThreedotsbelow-ar";
+glyphname = san;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1701;
+unicode = 1019;
 },
 {
-glyphname = "qaf-ar";
+glyphname = rhoStrokeSymbol;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1602;
+unicode = 1020;
 },
 {
-glyphname = "qafDotabove-ar";
+glyphname = "onequarter-atticGreek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1703;
+unicode = 65856;
 },
 {
-glyphname = "qafThreedotsabove-ar";
+glyphname = "onehalf-atticGreek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1704;
+unicode = 65857;
 },
 {
-glyphname = "kaf-ar";
+glyphname = "onedrachma-atticGreek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1603;
+unicode = 65858;
 },
 {
-glyphname = "keheh-ar";
+glyphname = "five-atticGreek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1705;
+unicode = 65859;
 },
 {
-glyphname = "kehehThreedotsabove-ar";
+glyphname = "fifty-atticGreek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1891;
+unicode = 65860;
 },
 {
-glyphname = "gaf-ar";
+glyphname = "fivehundred-atticGreek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1711;
+unicode = 65861;
 },
 {
-glyphname = "ng-ar";
+glyphname = "fivethousand-atticGreek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1709;
+unicode = 65862;
 },
 {
-glyphname = "lam-ar";
+glyphname = "fiftythousand-atticGreek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1604;
+unicode = 65863;
 },
 {
-glyphname = "meem-ar";
+glyphname = "fivetalents-atticGreek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1605;
+unicode = 65864;
 },
 {
-glyphname = "noon-ar";
+glyphname = "tentalents-atticGreek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1606;
+unicode = 65865;
 },
 {
-glyphname = "noonghunna-ar";
+glyphname = "fiftytalents-atticGreek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1722;
+unicode = 65866;
 },
 {
-glyphname = "heh-ar";
+glyphname = "onehundredtalents-atticGreek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1607;
+unicode = 65867;
 },
 {
-glyphname = "hehHamzaabove-ar";
+glyphname = "fivehundredtalents-atticGreek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1728;
+unicode = 65868;
 },
 {
-glyphname = "hehgoal-ar";
+glyphname = "onethousandtalents-atticGreek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1729;
+unicode = 65869;
 },
 {
-glyphname = "hehgoalHamzaabove-ar";
+glyphname = "fivethousandtalents-atticGreek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1730;
+unicode = 65870;
 },
 {
-glyphname = "hehDoachashmee-ar";
+glyphname = "fivestaters-atticGreek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1726;
+unicode = 65871;
 },
 {
-glyphname = "tehMarbuta-ar";
+glyphname = "tenstaters-atticGreek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1577;
+unicode = 65872;
 },
 {
-glyphname = "tehMarbutagoal-ar";
+glyphname = "fiftystaters-atticGreek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1731;
+unicode = 65873;
 },
 {
-glyphname = "waw-ar";
+glyphname = "onehundredstaters-atticGreek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1608;
+unicode = 65874;
 },
 {
-glyphname = "wawHamzaabove-ar";
+glyphname = "fivehundredstaters-atticGreek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1572;
+unicode = 65875;
 },
 {
-glyphname = "alefMaksura-ar";
+glyphname = "onethousandstaters-atticGreek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1609;
+unicode = 65876;
 },
 {
-glyphname = "yeh-ar";
+glyphname = "tenthousandstaters-atticGreek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1610;
+unicode = 65877;
 },
 {
-glyphname = "yehHamzaabove-ar";
+glyphname = "fiftythousandstaters-atticGreek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1574;
+unicode = 65878;
 },
 {
-glyphname = "yehFarsi-ar";
+glyphname = "tenmnas-atticGreek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1740;
+unicode = 65879;
 },
 {
-glyphname = "yehbarree-ar";
+glyphname = "heraeumoneplethron-ancientGreek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1746;
+unicode = 65880;
 },
 {
-glyphname = "yehbarreeHamzaabove-ar";
+glyphname = "thespianone-ancientGreek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1747;
+unicode = 65881;
 },
 {
-glyphname = "ae-ar";
+glyphname = "hermionianone-ancientGreek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1749;
+unicode = 65882;
 },
 {
-glyphname = "kashida-ar";
+glyphname = "epidaureantwo-ancientGreek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1600;
+unicode = 65883;
 },
 {
-glyphname = "decimalseparator-ar";
+glyphname = "thespiantwo-ancientGreek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1643;
+unicode = 65884;
 },
 {
-glyphname = "thousandseparator-ar";
+glyphname = "cyrenaictwodrachmas-ancientGreek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1644;
+unicode = 65885;
 },
 {
-glyphname = "zero-ar";
+glyphname = "epidaureantwodrachmas-ancientGreek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1632;
+unicode = 65886;
 },
 {
-glyphname = "one-ar";
+glyphname = "troezenianfive-ancientGreek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1633;
+unicode = 65887;
 },
 {
-glyphname = "two-ar";
+glyphname = "troezenianten-ancientGreek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1634;
+unicode = 65888;
 },
 {
-glyphname = "three-ar";
+glyphname = "troezeniantenalternateform-ancientGreek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1635;
+unicode = 65889;
 },
 {
-glyphname = "four-ar";
+glyphname = "hermionianten-ancientGreek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1636;
+unicode = 65890;
 },
 {
-glyphname = "five-ar";
+glyphname = "messenianten-ancientGreek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1637;
+unicode = 65891;
 },
 {
-glyphname = "six-ar";
+glyphname = "thespianten-ancientGreek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1638;
+unicode = 65892;
 },
 {
-glyphname = "seven-ar";
+glyphname = "thespianthirty-ancientGreek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1639;
+unicode = 65893;
 },
 {
-glyphname = "eight-ar";
+glyphname = "troezenianfifty-ancientGreek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1640;
+unicode = 65894;
 },
 {
-glyphname = "nine-ar";
+glyphname = "troezenianfiftyalternateform-ancientGreek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1641;
+unicode = 65895;
 },
 {
-glyphname = "zeroFarsi-ar";
+glyphname = "hermionianfifty-ancientGreek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1776;
+unicode = 65896;
 },
 {
-glyphname = "oneFarsi-ar";
+glyphname = "thespianfifty-ancientGreek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1777;
+unicode = 65897;
 },
 {
-glyphname = "twoFarsi-ar";
+glyphname = "thespianonehundred-ancientGreek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1778;
+unicode = 65898;
 },
 {
-glyphname = "threeFarsi-ar";
+glyphname = "thespianthreehundred-ancientGreek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1779;
+unicode = 65899;
 },
 {
-glyphname = "fourFarsi-ar";
+glyphname = "epidaureanfivehundred-ancientGreek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1780;
+unicode = 65900;
 },
 {
-glyphname = "fiveFarsi-ar";
+glyphname = "troezenianfivehundred-ancientGreek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1781;
+unicode = 65901;
 },
 {
-glyphname = "sixFarsi-ar";
+glyphname = "thespianfivehundred-ancientGreek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1782;
+unicode = 65902;
 },
 {
-glyphname = "sevenFarsi-ar";
+glyphname = "carystianfivehundred-ancientGreek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1783;
+unicode = 65903;
 },
 {
-glyphname = "eightFarsi-ar";
+glyphname = "naxianfivehundred-ancientGreek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1784;
+unicode = 65904;
 },
 {
-glyphname = "nineFarsi-ar";
+glyphname = "thespianonethousand-ancientGreek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1785;
+unicode = 65905;
 },
 {
-glyphname = zero;
+glyphname = "thespianfivethousand-ancientGreek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 48;
+unicode = 65906;
 },
 {
-glyphname = one;
+glyphname = "delphicfivemnas-ancientGreek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 49;
+unicode = 65907;
 },
 {
-glyphname = two;
+glyphname = "stratianfiftymnas-ancientGreek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 50;
+unicode = 65908;
 },
 {
-glyphname = three;
+glyphname = "onehalf-greek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 51;
+unicode = 65909;
 },
 {
-glyphname = four;
+glyphname = "onehalfAlternate-greek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 52;
+unicode = 65910;
 },
 {
-glyphname = five;
+glyphname = "twothirds-greek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 53;
+unicode = 65911;
 },
 {
-glyphname = six;
+glyphname = "threequarters-greek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 54;
+unicode = 65912;
 },
 {
-glyphname = seven;
+glyphname = "zero-greek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 55;
+unicode = 65930;
 },
 {
-glyphname = eight;
+glyphname = "year-greek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 56;
+unicode = 65913;
 },
 {
-glyphname = nine;
+glyphname = "talent-greek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 57;
+unicode = 65914;
 },
 {
-glyphname = space;
-layers = (
-{
-layerId = m01;
-width = 200;
-}
-);
-unicode = 32;
-},
-{
-glyphname = nbspace;
+glyphname = "drachma-greek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 160;
+unicode = 65915;
 },
 {
-glyphname = "fullstop-ar";
+glyphname = "obol-greek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1748;
+unicode = 65916;
 },
 {
-glyphname = "comma-ar";
+glyphname = "twoObols-greek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1548;
+unicode = 65917;
 },
 {
-glyphname = "semicolon-ar";
+glyphname = "threeObols-greek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1563;
+unicode = 65918;
 },
 {
-glyphname = "question-ar";
+glyphname = "fourObols-greek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1567;
+unicode = 65919;
 },
 {
-glyphname = "asterisk-ar";
+glyphname = "fiveObols-greek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1645;
+unicode = 65920;
 },
 {
-glyphname = period;
+glyphname = "metretes-greek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 46;
+unicode = 65921;
 },
 {
-glyphname = colon;
+glyphname = "kyathosBase-greek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 58;
+unicode = 65922;
 },
 {
-glyphname = ellipsis;
+glyphname = "litra-greek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 8230;
+unicode = 65923;
 },
 {
-glyphname = exclam;
+glyphname = "ounkia-greek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 33;
+unicode = 65924;
 },
 {
-glyphname = asterisk;
+glyphname = "xestes-greek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 42;
+unicode = 65925;
 },
 {
-glyphname = numbersign;
+glyphname = "artabe-greek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 35;
+unicode = 65926;
 },
 {
-glyphname = slash;
+glyphname = "aroura-greek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 47;
+unicode = 65927;
 },
 {
-glyphname = backslash;
+glyphname = "gramma-greek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 92;
+unicode = 65928;
 },
 {
-glyphname = hyphen;
+glyphname = "tryblionBase-greek";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 45;
+unicode = 65929;
 },
 {
-glyphname = parenleft;
+glyphname = epsilonLunateReversedSymbol;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 40;
+unicode = 1014;
 },
 {
-glyphname = parenright;
+glyphname = sunSymbol;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 41;
+unicode = 9737;
 },
 {
-glyphname = braceleft;
+glyphname = blackstar;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 123;
+unicode = 9733;
 },
 {
-glyphname = braceright;
+glyphname = ascendingNode;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 125;
+unicode = 9738;
 },
 {
-glyphname = bracketleft;
+glyphname = descendingNode;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 91;
+unicode = 9739;
 },
 {
-glyphname = bracketright;
+glyphname = conjunction;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 93;
+unicode = 9740;
 },
 {
-glyphname = quotedblleft;
+glyphname = opposition;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 8220;
+unicode = 9741;
 },
 {
-glyphname = quotedblright;
+glyphname = constantineCross;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 8221;
+unicode = 9767;
 },
 {
-glyphname = quoteleft;
+glyphname = jerusalemCross;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 8216;
+unicode = 9769;
 },
 {
-glyphname = quoteright;
+glyphname = firstQuarterMoon;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 8217;
+unicode = 9789;
 },
 {
-glyphname = guillemetleft;
+glyphname = lastQuarterMoon;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 171;
+unicode = 9790;
 },
 {
-glyphname = guillemetright;
+glyphname = mercury;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 187;
+unicode = 9791;
 },
 {
-glyphname = quotedbl;
+glyphname = venus;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 34;
+unicode = 9792;
 },
 {
-glyphname = quotesingle;
+glyphname = earth;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 39;
+unicode = 9793;
 },
 {
-glyphname = "percent-ar";
+glyphname = mars;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1642;
+unicode = 9794;
 },
 {
-glyphname = bar;
+glyphname = jupiter;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 124;
+unicode = 9795;
 },
 {
-glyphname = plus;
+glyphname = saturn;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 43;
+unicode = 9796;
 },
 {
-glyphname = multiply;
+glyphname = uranus;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 215;
+unicode = 9797;
 },
 {
-glyphname = divide;
+glyphname = neptune;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 247;
+unicode = 9798;
 },
 {
-glyphname = equal;
+glyphname = pluto;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 61;
+unicode = 9799;
 },
 {
-glyphname = greater;
+glyphname = aries;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 62;
+unicode = 9800;
 },
 {
-glyphname = less;
+glyphname = taurus;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 60;
+unicode = 9801;
 },
 {
-glyphname = percent;
+glyphname = gemini;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 37;
+unicode = 9802;
 },
 {
-glyphname = "hamzaabove-ar";
+glyphname = cancer;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1620;
+unicode = 9803;
 },
 {
-glyphname = "hamzabelow-ar";
+glyphname = leo;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1621;
+unicode = 9804;
 },
 {
-glyphname = "fathatan-ar";
+glyphname = virgo;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1611;
+unicode = 9805;
 },
 {
-glyphname = "dammatan-ar";
+glyphname = libra;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1612;
+unicode = 9806;
 },
 {
-glyphname = "kasratan-ar";
+glyphname = scorpius;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1613;
+unicode = 9807;
 },
 {
-glyphname = "fatha-ar";
+glyphname = sagittarius;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1614;
+unicode = 9808;
 },
 {
-glyphname = "damma-ar";
+glyphname = capricorn;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1615;
+unicode = 9809;
 },
 {
-glyphname = "kasra-ar";
+glyphname = aquarius;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1616;
+unicode = 9810;
 },
 {
-glyphname = "shadda-ar";
+glyphname = pisces;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1617;
+unicode = 9811;
 },
 {
-glyphname = "sukun-ar";
+glyphname = threeDimensionalAngle;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1618;
+unicode = 10176;
 },
 {
-glyphname = "madda-ar";
+glyphname = whitetrianglecontainingwhitetriangle;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1619;
+unicode = 10177;
 },
 {
-glyphname = uni069COVE;
+glyphname = whiteSquare;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
+unicode = 9633;
 }
 );
 metrics = (
 {
 type = ascender;
 },
 {
```

### Comparing `glyphsets-0.6.8/GF_glyphsets/Arabic/glyphs/GF_Arabic_Plus.glyphs` & `glyphsets-0.6.9/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_Historical.glyphs`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {
 .appVersion = "3124";
 .formatVersion = 3;
 date = "2021-10-28 12:22:31 +0000";
-familyName = "GF Arabic Plus";
+familyName = "GF Cyrillic Historical";
 featurePrefixes = (
 {
 automatic = 1;
 code = "languagesystem DFLT dflt;
 
 languagesystem latn dflt;
 languagesystem latn AZE;
@@ -118,442 +118,372 @@
 }
 );
 name = Regular;
 }
 );
 glyphs = (
 {
-glyphname = "highhamza-ar";
+glyphname = "OmegaBroad-cy";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1652;
+unicode = 42572;
 },
 {
-glyphname = "beeh-ar";
+glyphname = "Omega-cy";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1659;
+unicode = 1120;
 },
 {
-glyphname = "beheh-ar";
+glyphname = "Eiotified-cy";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1664;
+unicode = 1124;
 },
 {
-glyphname = "tehRing-ar";
+glyphname = "Yuslittle-cy";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1660;
+unicode = 1126;
 },
 {
-glyphname = "tehThreedotsdown-ar";
+glyphname = "Yuslittleiotified-cy";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1661;
+unicode = 1128;
 },
 {
-glyphname = "tteheh-ar";
+glyphname = "Yusbigiotified-cy";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1658;
+unicode = 1132;
 },
 {
-glyphname = "teheh-ar";
+glyphname = "Ksi-cy";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1663;
+unicode = 1134;
 },
 {
-glyphname = "tcheheh-ar";
+glyphname = "Psi-cy";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1671;
+unicode = 1136;
 },
 {
-glyphname = "nyeh-ar";
+glyphname = "Izhitsadblgrave-cy";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1667;
+unicode = 1142;
 },
 {
-glyphname = "dyeh-ar";
+glyphname = "Uk-cy";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1668;
+unicode = 1144;
 },
 {
-glyphname = "hahHamzaabove-ar";
+glyphname = "Koppa-cy";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1665;
+unicode = 1152;
 },
 {
-glyphname = "hahThreedotsabove-ar";
+glyphname = "omega-cy";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1669;
+unicode = 1121;
 },
 {
-glyphname = "dahal-ar";
+glyphname = "eiotified-cy";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1676;
+unicode = 1125;
 },
 {
-glyphname = "ddahal-ar";
+glyphname = "yuslittle-cy";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1677;
+unicode = 1127;
 },
 {
-glyphname = "dalRing-ar";
+glyphname = "yuslittleiotified-cy";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1673;
+unicode = 1129;
 },
 {
-glyphname = "dalDotbelow-ar";
+glyphname = "yusbigiotified-cy";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1674;
+unicode = 1133;
 },
 {
-glyphname = "dalThreedotsdown-ar";
+glyphname = "ksi-cy";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1679;
+unicode = 1135;
 },
 {
-glyphname = "rehRing-ar";
+glyphname = "psi-cy";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1683;
+unicode = 1137;
 },
 {
-glyphname = "rehVbelow-ar";
+glyphname = "izhitsadblgrave-cy";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1685;
+unicode = 1143;
 },
 {
-glyphname = "rehDotbelowdotabove-ar";
+glyphname = "uk-cy";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1686;
+unicode = 1145;
 },
 {
-glyphname = "rehFourdots-ar";
+glyphname = "koppa-cy";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1689;
+unicode = 1153;
 },
 {
-glyphname = "seenDotbelowDotabove-ar";
+glyphname = "omegaBroad-cy";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1690;
+unicode = 42573;
 },
 {
-glyphname = "sheenThreedotsbelow-ar";
+glyphname = "thousand-cy";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1692;
+unicode = 1154;
 },
 {
-glyphname = "ainThreedots-ar";
+glyphname = "hundredthousandssigncomb-cy";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1696;
+unicode = 1160;
 },
 {
-glyphname = "peheh-ar";
+glyphname = "millionssigncomb-cy";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1702;
+unicode = 1161;
 },
 {
-glyphname = "kehehDotabove-ar";
+glyphname = "titlocomb-cy";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1890;
+unicode = 1155;
 },
 {
-glyphname = "kafswash-ar";
+glyphname = "palatalizationcomb-cy";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1706;
+unicode = 1156;
 },
 {
-glyphname = "kafRing-ar";
+glyphname = "dasiapneumatacomb-cy";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1707;
+unicode = 1157;
 },
 {
-glyphname = "ngoeh-ar";
+glyphname = "psilipneumatacomb-cy";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1713;
+unicode = 1158;
 },
 {
-glyphname = "gueh-ar";
+glyphname = "pokrytiecomb-cy";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1715;
+unicode = 1159;
 },
 {
-glyphname = "lamVabove-ar";
+glyphname = uni047A;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1717;
+unicode = 1146;
 },
 {
-glyphname = "rnoon-ar";
+glyphname = uni047B;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1723;
+unicode = 1147;
 },
 {
-glyphname = "noonRing-ar";
+glyphname = uni047C;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1724;
+unicode = 1148;
 },
 {
-glyphname = "noonThreedotsabove-ar";
+glyphname = uni047D;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1725;
+unicode = 1149;
 },
 {
-glyphname = "wawDotabove-ar";
+glyphname = uni047E;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1743;
+unicode = 1150;
 },
 {
-glyphname = "oe-ar";
+glyphname = uni047F;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1734;
-},
-{
-glyphname = "u-ar";
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-unicode = 1735;
-},
-{
-glyphname = "yu-ar";
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-unicode = 1736;
-},
-{
-glyphname = "ve-ar";
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-unicode = 1739;
-},
-{
-glyphname = "yehVabove-ar";
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-unicode = 1742;
-},
-{
-glyphname = "yehTail-ar";
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-unicode = 1741;
-},
-{
-glyphname = "e-ar";
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-unicode = 1744;
-},
-{
-glyphname = "fathaHorizont-ar";
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-unicode = 1625;
+unicode = 1151;
 }
 );
 metrics = (
 {
 type = ascender;
 },
 {
```

### Comparing `glyphsets-0.6.8/GF_glyphsets/Arabic/nam/GF_Arabic_Core.nam` & `glyphsets-0.6.9/GF_glyphsets/Arabic/nam/GF_Arabic_Core.nam`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+# This file is auto-generated; do not edit. See /README.md for instructions.
 0x0020 SPACE
 0x0021 EXCLAMATION MARK
 0x0022 QUOTATION MARK
 0x0023 NUMBER SIGN
 0x0025 PERCENT SIGN
 0x0027 APOSTROPHE
 0x0028 LEFT PARENTHESIS
 0x0029 RIGHT PARENTHESIS
 0x002A ASTERISK
 0x002B PLUS SIGN
+0x002C COMMA
 0x002D HYPHEN-MINUS
 0x002E FULL STOP
 0x002F SOLIDUS
 0x0030 DIGIT ZERO
 0x0031 DIGIT ONE
 0x0032 DIGIT TWO
 0x0033 DIGIT THREE
@@ -32,16 +34,19 @@
 0x007C VERTICAL LINE
 0x007D RIGHT CURLY BRACKET
 0x00A0 NO-BREAK SPACE
 0x00AB LEFT-POINTING DOUBLE ANGLE QUOTATION MARK
 0x00BB RIGHT-POINTING DOUBLE ANGLE QUOTATION MARK
 0x00D7 MULTIPLICATION SIGN
 0x00F7 DIVISION SIGN
+0x0609 ARABIC-INDIC PER MILLE SIGN
 0x060C ARABIC COMMA
+0x060D ARABIC DATE SEPARATOR
 0x061B ARABIC SEMICOLON
+0x061C ARABIC LETTER MARK
 0x061F ARABIC QUESTION MARK
 0x0621 ARABIC LETTER HAMZA
 0x0622 ARABIC LETTER ALEF WITH MADDA ABOVE
 0x0623 ARABIC LETTER ALEF WITH HAMZA ABOVE
 0x0624 ARABIC LETTER WAW WITH HAMZA ABOVE
 0x0625 ARABIC LETTER ALEF WITH HAMZA BELOW
 0x0626 ARABIC LETTER YEH WITH HAMZA ABOVE
@@ -97,47 +102,45 @@
 0x0667 ARABIC-INDIC DIGIT SEVEN
 0x0668 ARABIC-INDIC DIGIT EIGHT
 0x0669 ARABIC-INDIC DIGIT NINE
 0x066A ARABIC PERCENT SIGN
 0x066B ARABIC DECIMAL SEPARATOR
 0x066C ARABIC THOUSANDS SEPARATOR
 0x066D ARABIC FIVE POINTED STAR
+0x0670 ARABIC LETTER SUPERSCRIPT ALEF
 0x0679 ARABIC LETTER TTEH
 0x067E ARABIC LETTER PEH
 0x0686 ARABIC LETTER TCHEH
 0x0688 ARABIC LETTER DDAL
 0x0691 ARABIC LETTER RREH
-0x06A2 ARABIC LETTER FEH WITH DOT MOVED BELOW
-0x06A4 ARABIC LETTER VEH
-0x06A5 ARABIC LETTER FEH WITH THREE DOTS BELOW
-0x06A7 ARABIC LETTER QAF WITH DOT ABOVE
-0x06A8 ARABIC LETTER QAF WITH THREE DOTS ABOVE
+0x0698 ARABIC LETTER JEH
 0x06A9 ARABIC LETTER KEHEH
-0x06AD ARABIC LETTER NG
 0x06AF ARABIC LETTER GAF
-0x06BA ARABIC LETTER NOON GHUNNA
 0x06BE ARABIC LETTER HEH DOACHASHMEE
-0x06C0 ARABIC LETTER HEH WITH YEH ABOVE
 0x06C1 ARABIC LETTER HEH GOAL
-0x06C2 ARABIC LETTER HEH GOAL WITH HAMZA ABOVE
-0x06C3 ARABIC LETTER TEH MARBUTA GOAL
 0x06CC ARABIC LETTER FARSI YEH
 0x06D2 ARABIC LETTER YEH BARREE
-0x06D3 ARABIC LETTER YEH BARREE WITH HAMZA ABOVE
 0x06D4 ARABIC FULL STOP
-0x06D5 ARABIC LETTER AE
 0x06F0 EXTENDED ARABIC-INDIC DIGIT ZERO
 0x06F1 EXTENDED ARABIC-INDIC DIGIT ONE
 0x06F2 EXTENDED ARABIC-INDIC DIGIT TWO
 0x06F3 EXTENDED ARABIC-INDIC DIGIT THREE
 0x06F4 EXTENDED ARABIC-INDIC DIGIT FOUR
 0x06F5 EXTENDED ARABIC-INDIC DIGIT FIVE
 0x06F6 EXTENDED ARABIC-INDIC DIGIT SIX
 0x06F7 EXTENDED ARABIC-INDIC DIGIT SEVEN
 0x06F8 EXTENDED ARABIC-INDIC DIGIT EIGHT
 0x06F9 EXTENDED ARABIC-INDIC DIGIT NINE
 0x0763 ARABIC LETTER KEHEH WITH THREE DOTS ABOVE
+0x200E LEFT-TO-RIGHT MARK
+0x2013 EN DASH
+0x2014 EM DASH
 0x2018 LEFT SINGLE QUOTATION MARK
 0x2019 RIGHT SINGLE QUOTATION MARK
 0x201C LEFT DOUBLE QUOTATION MARK
 0x201D RIGHT DOUBLE QUOTATION MARK
-0x2026 HORIZONTAL ELLIPSIS
+0x2026 HORIZONTAL ELLIPSIS
+0x2039 SINGLE LEFT-POINTING ANGLE QUOTATION MARK
+0x203A SINGLE RIGHT-POINTING ANGLE QUOTATION MARK
+0x2212 MINUS SIGN
+0xFD3E ORNATE LEFT PARENTHESIS
+0xFD3F ORNATE RIGHT PARENTHESIS
```

### Comparing `glyphsets-0.6.8/GF_glyphsets/Arabic/txt/nice-names/GF_Arabic_Core.txt` & `glyphsets-0.6.9/GF_glyphsets/Arabic/txt/nice-names/GF_Arabic_Plus.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,144 +1,130 @@
+# This file is auto-generated; do not edit. See /README.md for instructions.
+exclam
+percent
+quotesingle
+parenleft
+parenright
+plus
+comma
+hyphen
+period
+slash
+zero
+one
+two
+three
+four
+five
+six
+seven
+eight
+nine
+colon
+semicolon
+bracketleft
+bracketright
+perthousand-ar
+comma-ar
 hamza-ar
-alef-ar
-alefHamzaabove-ar
-alefHamzabelow-ar
 alefMadda-ar
+alefHamzaabove-ar
+wawHamzaabove-ar
+yehHamzaabove-ar
+alef-ar
 beh-ar
-peh-ar
+tehMarbuta-ar
 teh-ar
 theh-ar
-tteh-ar
 jeem-ar
-tcheh-ar
 hah-ar
 khah-ar
 dal-ar
 thal-ar
-ddal-ar
 reh-ar
 zain-ar
-rreh-ar
 seen-ar
 sheen-ar
 sad-ar
 dad-ar
 tah-ar
 zah-ar
 ain-ar
 ghain-ar
 feh-ar
-veh-ar
-fehDotmovedbelow-ar
-fehThreedotsbelow-ar
 qaf-ar
-qafDotabove-ar
-qafThreedotsabove-ar
 kaf-ar
-keheh-ar
-kehehThreedotsabove-ar
-gaf-ar
-ng-ar
 lam-ar
 meem-ar
 noon-ar
-noonghunna-ar
 heh-ar
-hehHamzaabove-ar
-hehgoal-ar
-hehgoalHamzaabove-ar
-hehDoachashmee-ar
-tehMarbuta-ar
-tehMarbutagoal-ar
 waw-ar
-wawHamzaabove-ar
 alefMaksura-ar
 yeh-ar
-yehHamzaabove-ar
-yehFarsi-ar
-yehbarree-ar
-yehbarreeHamzaabove-ar
-ae-ar
-kashida-ar
-decimalseparator-ar
-thousandseparator-ar
+fathatan-ar
+dammatan-ar
+kasratan-ar
+fatha-ar
+damma-ar
+kasra-ar
+shadda-ar
+sukun-ar
+hamzaabove-ar
 zero-ar
 one-ar
 two-ar
 three-ar
 four-ar
 five-ar
 six-ar
 seven-ar
 eight-ar
 nine-ar
-zeroFarsi-ar
-oneFarsi-ar
-twoFarsi-ar
-threeFarsi-ar
-fourFarsi-ar
-fiveFarsi-ar
-sixFarsi-ar
-sevenFarsi-ar
-eightFarsi-ar
-nineFarsi-ar
-zero
-one
-two
-three
-four
-five
-six
-seven
-eight
-nine
-space
-nbspace
+percent-ar
+decimalseparator-ar
+thousandseparator-ar
+alefabove-ar
+tehRing-ar
+peh-ar
+hahHamzaabove-ar
+hahThreedotsabove-ar
+tcheh-ar
+dalRing-ar
+rehRing-ar
+rehVbelow-ar
+rehDotbelowdotabove-ar
+jeh-ar
+seenDotbelowDotabove-ar
+veh-ar
+keheh-ar
+kafRing-ar
+ng-ar
+gaf-ar
+lamVabove-ar
+noonRing-ar
+hehDoachashmee-ar
+oe-ar
+u-ar
+yu-ar
+ve-ar
+yeh-farsi
+yehTail-ar
+yehVabove-ar
+e-ar
 fullstop-ar
-comma-ar
-semicolon-ar
-question-ar
-asterisk-ar
-period
-colon
-ellipsis
-exclam
-asterisk
-numbersign
-slash
-backslash
-hyphen
-parenleft
-parenright
-braceleft
-braceright
-bracketleft
-bracketright
-quotedblleft
-quotedblright
+ae-ar
+zero-persian
+one-persian
+two-persian
+three-persian
+four-persian
+five-persian
+six-persian
+seven-persian
+eight-persian
+nine-persian
+sindhiampersand-ar
+sindhipostpositionmen-ar
+lefttorightmark
+righttoleftmark
 quoteleft
-quoteright
-guillemetleft
-guillemetright
-quotedbl
-quotesingle
-percent-ar
-bar
-plus
-multiply
-divide
-equal
-greater
-less
-percent
-hamzaabove-ar
-hamzabelow-ar
-fathatan-ar
-dammatan-ar
-kasratan-ar
-fatha-ar
-damma-ar
-kasra-ar
-shadda-ar
-sukun-ar
-madda-ar
-uni069COVE
+minus
```

### Comparing `glyphsets-0.6.8/GF_glyphsets/Arabic/txt/prod-names/GF_Arabic_Core.txt` & `glyphsets-0.6.9/GF_glyphsets/Arabic/txt/prod-names/GF_Arabic_Core.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,144 +1,146 @@
+# This file is auto-generated; do not edit. See /README.md for instructions.
+space
+exclam
+quotedbl
+numbersign
+percent
+quotesingle
+parenleft
+parenright
+asterisk
+plus
+comma
+hyphen
+period
+slash
+zero
+one
+two
+three
+four
+five
+six
+seven
+eight
+nine
+colon
+less
+equal
+greater
+bracketleft
+backslash
+bracketright
+braceleft
+bar
+braceright
+uni00A0
+guillemotleft
+guillemotright
+multiply
+divide
+uni0609
+uni060C
+uni060D
+uni061B
+uni061C
+uni061F
 uni0621
-uni0627
+uni0622
 uni0623
+uni0624
 uni0625
-uni0622
+uni0626
+uni0627
 uni0628
-uni067E
+uni0629
 uni062A
 uni062B
-uni0679
 uni062C
-uni0686
 uni062D
 uni062E
 uni062F
 uni0630
-uni0688
 uni0631
 uni0632
-uni0691
 uni0633
 uni0634
 uni0635
 uni0636
 uni0637
 uni0638
 uni0639
 uni063A
+uni0640
 uni0641
-uni06A4
-uni06A2
-uni06A5
 uni0642
-uni06A7
-uni06A8
 uni0643
-uni06A9
-uni0763
-uni06AF
-uni06AD
 uni0644
 uni0645
 uni0646
-uni06BA
 uni0647
-uni06C0
-uni06C1
-uni06C2
-uni06BE
-uni0629
-uni06C3
 uni0648
-uni0624
 uni0649
 uni064A
-uni0626
-yehFarsiar
-uni06D2
-uni06D3
-uni06D5
-uni0640
-uni066B
-uni066C
+uni064B
+uni064C
+uni064D
+uni064E
+uni064F
+uni0650
+uni0651
+uni0652
+uni0653
+uni0654
+uni0655
 uni0660
 uni0661
 uni0662
 uni0663
 uni0664
 uni0665
 uni0666
 uni0667
 uni0668
 uni0669
-zeroFarsiar
-oneFarsiar
-twoFarsiar
-threeFarsiar
-fourFarsiar
-fiveFarsiar
-sixFarsiar
-sevenFarsiar
-eightFarsiar
-nineFarsiar
-zero
-one
-two
-three
-four
-five
-six
-seven
-eight
-nine
-space
-uni00A0
-uni06D4
-uni060C
-uni061B
-uni061F
+uni066A
+uni066B
+uni066C
 uni066D
-period
-colon
-ellipsis
-exclam
-asterisk
-numbersign
-slash
-backslash
-hyphen
-parenleft
-parenright
-braceleft
-braceright
-bracketleft
-bracketright
-quotedblleft
-quotedblright
+uni0670
+uni0679
+uni067E
+uni0686
+uni0688
+uni0691
+uni0698
+uni06A9
+uni06AF
+uni06BE
+uni06C1
+uni06CC
+uni06D2
+uni06D4
+uni06F0
+uni06F1
+uni06F2
+uni06F3
+uni06F4
+uni06F5
+uni06F6
+uni06F7
+uni06F8
+uni06F9
+uni0763
+uni200E
+endash
+emdash
 quoteleft
 quoteright
-guillemotleft
-guillemotright
-quotedbl
-quotesingle
-uni066A
-bar
-plus
-multiply
-divide
-equal
-greater
-less
-percent
-uni0654
-uni0655
-uni064B
-uni064C
-uni064D
-uni064E
-uni064F
-uni0650
-uni0651
-uni0652
-uni0653
-uni069COVE
+quotedblleft
+quotedblright
+ellipsis
+guilsinglleft
+guilsinglright
+minus
+uniFD3E
+uniFD3F
```

### Comparing `glyphsets-0.6.8/GF_glyphsets/Cyrillic/README.md` & `glyphsets-0.6.9/GF_glyphsets/Cyrillic/README.md`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Cyrillic/glyphs/CustomFilter_GF_Cyrillic.plist` & `glyphsets-0.6.9/GF_glyphsets/Cyrillic/glyphs/CustomFilter_GF_Cyrillic.plist`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_Core.glyphs` & `glyphsets-0.6.9/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_Core.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_Historical.glyphs` & `glyphsets-0.6.9/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_PlusLoclRoman.glyphs`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {
 .appVersion = "3124";
 .formatVersion = 3;
 date = "2021-10-28 12:22:31 +0000";
-familyName = "GF Cyrillic Historical";
+familyName = "GF Cyrillic Plus Locl Roman";
 featurePrefixes = (
 {
 automatic = 1;
 code = "languagesystem DFLT dflt;
 
 languagesystem latn dflt;
 languagesystem latn AZE;
@@ -118,372 +118,327 @@
 }
 );
 name = Regular;
 }
 );
 glyphs = (
 {
-glyphname = "OmegaBroad-cy";
+glyphname = "De-cy.loclBGR";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 42572;
 },
 {
-glyphname = "Omega-cy";
+glyphname = "Ii-cy.loclBGR";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1120;
 },
 {
-glyphname = "Eiotified-cy";
+glyphname = "Iishort-cy.loclBGR";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1124;
 },
 {
-glyphname = "Yuslittle-cy";
+glyphname = "Iigrave-cy.loclBGR";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1126;
 },
 {
-glyphname = "Yuslittleiotified-cy";
+glyphname = "El-cy.loclBGR";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1128;
 },
 {
-glyphname = "Yusbigiotified-cy";
+glyphname = "Ef-cy.loclBGR";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1132;
 },
 {
-glyphname = "Ksi-cy";
+glyphname = "Gestroke-cy.loclBSH";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1134;
 },
 {
-glyphname = "Psi-cy";
+glyphname = "Zedescender-cy.loclBSH";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1136;
 },
 {
-glyphname = "Izhitsadblgrave-cy";
+glyphname = "Esdescender-cy.loclBSH";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1142;
 },
 {
-glyphname = "Uk-cy";
+glyphname = "Esdescender-cy.loclCHU";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1144;
 },
 {
-glyphname = "Koppa-cy";
+glyphname = "ve-cy.loclBGR";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1152;
 },
 {
-glyphname = "omega-cy";
+glyphname = "ge-cy.loclBGR";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1121;
 },
 {
-glyphname = "eiotified-cy";
+glyphname = "de-cy.loclBGR";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1125;
 },
 {
-glyphname = "yuslittle-cy";
+glyphname = "zhe-cy.loclBGR";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1127;
 },
 {
-glyphname = "yuslittleiotified-cy";
+glyphname = "ze-cy.loclBGR";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1129;
 },
 {
-glyphname = "yusbigiotified-cy";
+glyphname = "ii-cy.loclBGR";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1133;
 },
 {
-glyphname = "ksi-cy";
+glyphname = "iishort-cy.loclBGR";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1135;
 },
 {
-glyphname = "psi-cy";
+glyphname = "iigrave-cy.loclBGR";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1137;
 },
 {
-glyphname = "izhitsadblgrave-cy";
+glyphname = "ka-cy.loclBGR";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1143;
 },
 {
-glyphname = "uk-cy";
+glyphname = "el-cy.loclBGR";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1145;
 },
 {
-glyphname = "koppa-cy";
+glyphname = "en-cy.loclBGR";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1153;
 },
 {
-glyphname = "omegaBroad-cy";
+glyphname = "pe-cy.loclBGR";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 42573;
 },
 {
-glyphname = "thousand-cy";
+glyphname = "te-cy.loclBGR";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1154;
 },
 {
-glyphname = "hundredthousandssigncomb-cy";
+glyphname = "che-cy.loclBGR";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1160;
 },
 {
-glyphname = "millionssigncomb-cy";
+glyphname = "tse-cy.loclBGR";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1161;
 },
 {
-glyphname = "titlocomb-cy";
+glyphname = "sha-cy.loclBGR";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1155;
 },
 {
-glyphname = "palatalizationcomb-cy";
+glyphname = "shcha-cy.loclBGR";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1156;
 },
 {
-glyphname = "dasiapneumatacomb-cy";
+glyphname = "softsign-cy.loclBGR";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1157;
 },
 {
-glyphname = "psilipneumatacomb-cy";
+glyphname = "hardsign-cy.loclBGR";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1158;
 },
 {
-glyphname = "pokrytiecomb-cy";
+glyphname = "yu-cy.loclBGR";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1159;
 },
 {
-glyphname = uni047A;
+glyphname = "gestroke-cy.loclBSH";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1146;
 },
 {
-glyphname = uni047B;
+glyphname = "zedescender-cy.loclBSH";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1147;
 },
 {
-glyphname = uni047C;
+glyphname = "esdescender-cy.loclBSH";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1148;
 },
 {
-glyphname = uni047D;
+glyphname = "esdescender-cy.loclCHU";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1149;
 },
 {
-glyphname = uni047E;
+glyphname = "be-cy.loclSRB";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1150;
-},
-{
-glyphname = uni047F;
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-unicode = 1151;
 }
 );
 metrics = (
 {
 type = ascender;
 },
 {
```

### Comparing `glyphsets-0.6.8/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_Plus.glyphs` & `glyphsets-0.6.9/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_Plus.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_PlusLoclItalic.glyphs` & `glyphsets-0.6.9/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_PlusLoclItalic.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_Pro.glyphs` & `glyphsets-0.6.9/GF_glyphsets/Cyrillic/glyphs/GF_Cyrillic_Pro.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_Core.nam` & `glyphsets-0.6.9/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_Core.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_Historical.nam` & `glyphsets-0.6.9/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_Historical.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_Plus.nam` & `glyphsets-0.6.9/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_Plus.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_Pro.nam` & `glyphsets-0.6.9/GF_glyphsets/Cyrillic/nam/GF_Cyrillic_Pro.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_Core.txt` & `glyphsets-0.6.9/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_Core.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_Plus.txt` & `glyphsets-0.6.9/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_Plus.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_PlusLoclRoman.txt` & `glyphsets-0.6.9/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_PlusLoclRoman.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_Pro.txt` & `glyphsets-0.6.9/GF_glyphsets/Cyrillic/txt/nice-names/GF_Cyrillic_Pro.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Cyrillic/txt/prod-names/GF_Cyrillic_Core.txt` & `glyphsets-0.6.9/GF_glyphsets/Cyrillic/txt/prod-names/GF_Cyrillic_Core.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Cyrillic/txt/prod-names/GF_Cyrillic_Plus.txt` & `glyphsets-0.6.9/GF_glyphsets/Cyrillic/txt/prod-names/GF_Cyrillic_Plus.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Cyrillic/txt/prod-names/GF_Cyrillic_PlusLoclRoman.txt` & `glyphsets-0.6.9/GF_glyphsets/Cyrillic/txt/prod-names/GF_Cyrillic_PlusLoclRoman.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Greek/README.md` & `glyphsets-0.6.9/GF_glyphsets/Greek/README.md`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Greek/glyphs/CustomFilter_GF_Greek.plist` & `glyphsets-0.6.9/GF_glyphsets/Greek/glyphs/CustomFilter_GF_Greek.plist`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Greek/glyphs/GF_Greek_AncientMusicalSymbols.glyphs` & `glyphsets-0.6.9/GF_glyphsets/Greek/glyphs/GF_Greek_AncientMusicalSymbols.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Greek/glyphs/GF_Greek_Archaic.glyphs` & `glyphsets-0.6.9/GF_glyphsets/TransLatin/glyphs/GF_TransLatin_Pinyin.glyphs`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {
 .appVersion = "3124";
 .formatVersion = 3;
 date = "2021-10-28 12:22:31 +0000";
-familyName = "GF Greek Archaic";
+familyName = "GF TransLatin Pinyin";
 featurePrefixes = (
 {
 automatic = 1;
 code = "languagesystem DFLT dflt;
 
 languagesystem latn dflt;
 languagesystem latn AZE;
@@ -118,1442 +118,1118 @@
 }
 );
 name = Regular;
 }
 );
 glyphs = (
 {
-glyphname = Heta;
+color = 3;
+glyphname = Aacute;
+lastChange = "2022-04-29 09:57:47 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 880;
+unicode = 193;
 },
 {
-glyphname = Archaicsampi;
+color = 3;
+glyphname = Abreve;
+lastChange = "2022-04-29 09:57:47 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 882;
+unicode = 258;
 },
 {
-glyphname = Pamphyliandigamma;
+glyphname = Acaron;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 886;
+unicode = 461;
 },
 {
-glyphname = KoppaArchaic;
+color = 3;
+glyphname = Acircumflex;
+lastChange = "2022-04-29 09:57:47 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 984;
+unicode = 194;
 },
 {
-glyphname = UpsilonhookSymbol;
+color = 3;
+glyphname = Acircumflex;
+lastChange = "2022-04-29 09:57:47 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 978;
+unicode = 194;
 },
 {
-glyphname = UpsilonacutehookSymbol;
+color = 3;
+glyphname = Agrave;
+lastChange = "2022-04-29 09:57:47 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 979;
+unicode = 192;
 },
 {
-glyphname = UpsilondieresishookSymbol;
+glyphname = Amacron;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 980;
+unicode = 256;
 },
 {
-glyphname = ThetaSymbol;
+color = 3;
+glyphname = Eacute;
+lastChange = "2022-04-29 09:57:47 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1012;
+unicode = 201;
 },
 {
-glyphname = Sho;
+color = 3;
+glyphname = Ebreve;
+lastChange = "2022-04-29 09:57:47 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1015;
+unicode = 276;
 },
 {
-glyphname = SigmaLunateSymbol;
+glyphname = Ecaron;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1017;
+unicode = 282;
 },
 {
-glyphname = San;
+color = 3;
+glyphname = Ecircumflex;
+lastChange = "2022-04-29 09:57:47 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1018;
+unicode = 202;
 },
 {
-glyphname = SigmaLunateReversedSymbol;
+color = 3;
+glyphname = Egrave;
+lastChange = "2022-04-29 09:57:47 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1021;
+unicode = 200;
 },
 {
-glyphname = SigmaLunateDottedSymbol;
+color = 3;
+glyphname = Emacron;
+lastChange = "2022-04-29 09:57:47 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1022;
+unicode = 274;
 },
 {
-glyphname = SigmaLunateDottedReversedSymbol;
+color = 3;
+glyphname = Iacute;
+lastChange = "2022-04-29 09:57:47 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1023;
+unicode = 205;
 },
 {
-glyphname = heta;
+color = 3;
+glyphname = Ibreve;
+lastChange = "2022-04-29 09:45:08 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 881;
+unicode = 300;
 },
 {
-glyphname = archaicsampi;
+glyphname = Icaron;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 883;
+unicode = 463;
 },
 {
-glyphname = pamphyliandigamma;
+color = 3;
+glyphname = Icircumflex;
+lastChange = "2022-04-29 09:57:47 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 887;
+unicode = 206;
 },
 {
-glyphname = sigmaLunateReversedSymbol;
+color = 3;
+glyphname = Idieresis;
+lastChange = "2022-04-29 09:57:47 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 891;
+unicode = 207;
 },
 {
-glyphname = sigmaLunateDottedSymbol;
+color = 3;
+glyphname = Igrave;
+lastChange = "2022-04-29 09:57:47 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 892;
+unicode = 204;
 },
 {
-glyphname = sigmaLunateDottedReversedSymbol;
+glyphname = Imacron;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 893;
+unicode = 298;
 },
 {
-glyphname = koppaArchaic;
+color = 3;
+glyphname = Macute;
+lastChange = "2022-04-29 09:57:47 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 985;
+unicode = 7742;
 },
 {
-glyphname = betaSymbol;
+color = 3;
+glyphname = Nacute;
+lastChange = "2022-04-29 09:57:47 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 976;
+unicode = 323;
 },
 {
-glyphname = thetaSymbol;
+color = 3;
+glyphname = Ngrave;
+lastChange = "2022-04-29 09:57:47 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 977;
+unicode = 504;
 },
 {
-glyphname = phiSymbol;
+color = 3;
+glyphname = Oacute;
+lastChange = "2022-04-29 09:57:47 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 981;
+unicode = 211;
 },
 {
-glyphname = piSymbol;
+color = 3;
+glyphname = Obreve;
+lastChange = "2022-04-29 09:57:47 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 982;
+unicode = 334;
 },
 {
-glyphname = kappaSymbol;
+glyphname = Ocaron;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1008;
+unicode = 465;
 },
 {
-glyphname = rhoSymbol;
+color = 3;
+glyphname = Ocircumflex;
+lastChange = "2022-04-29 09:57:47 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1009;
+unicode = 212;
 },
 {
-glyphname = sigmaLunateSymbol;
+color = 3;
+glyphname = Ograve;
+lastChange = "2022-04-29 09:57:47 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1010;
+unicode = 210;
 },
 {
-glyphname = yot;
+color = 3;
+glyphname = Omacron;
+lastChange = "2022-04-29 09:57:47 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1011;
+unicode = 332;
 },
 {
-glyphname = epsilonLunateSymbol;
+color = 3;
+glyphname = Uacute;
+lastChange = "2022-04-29 09:57:47 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1013;
+unicode = 218;
 },
 {
-glyphname = sho;
+color = 3;
+glyphname = Ubreve;
+lastChange = "2022-04-29 09:57:47 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1016;
+unicode = 364;
 },
 {
-glyphname = san;
+glyphname = Ucaron;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1019;
+unicode = 467;
 },
 {
-glyphname = rhoStrokeSymbol;
+color = 3;
+glyphname = Ucircumflex;
+lastChange = "2022-04-29 09:57:47 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 1020;
+unicode = 219;
 },
 {
-glyphname = "onequarter-atticGreek";
+glyphname = Udieresis;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65856;
+unicode = 220;
 },
 {
-glyphname = "onehalf-atticGreek";
+glyphname = Udieresisacute;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65857;
+unicode = 471;
 },
 {
-glyphname = "onedrachma-atticGreek";
+glyphname = Udieresiscaron;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65858;
+unicode = 473;
 },
 {
-glyphname = "five-atticGreek";
+glyphname = Udieresisgrave;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65859;
+unicode = 475;
 },
 {
-glyphname = "fifty-atticGreek";
+glyphname = Udieresismacron;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65860;
+unicode = 469;
 },
 {
-glyphname = "fivehundred-atticGreek";
+color = 3;
+glyphname = Ugrave;
+lastChange = "2022-04-29 09:57:47 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65861;
+unicode = 217;
 },
 {
-glyphname = "fivethousand-atticGreek";
+glyphname = Umacron;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65862;
+unicode = 362;
 },
 {
-glyphname = "fiftythousand-atticGreek";
+color = 3;
+glyphname = aacute;
+lastChange = "2022-04-29 09:57:47 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65863;
+unicode = 225;
 },
 {
-glyphname = "fivetalents-atticGreek";
+color = 3;
+glyphname = abreve;
+lastChange = "2022-04-29 09:57:47 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65864;
+unicode = 259;
 },
 {
-glyphname = "tentalents-atticGreek";
+glyphname = acaron;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65865;
+unicode = 462;
 },
 {
-glyphname = "fiftytalents-atticGreek";
+color = 3;
+glyphname = acircumflex;
+lastChange = "2022-04-29 09:57:47 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65866;
+unicode = 226;
 },
 {
-glyphname = "onehundredtalents-atticGreek";
+color = 3;
+glyphname = agrave;
+lastChange = "2022-04-29 09:57:47 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65867;
+unicode = 224;
 },
 {
-glyphname = "fivehundredtalents-atticGreek";
+color = 3;
+glyphname = agrave;
+lastChange = "2022-04-29 09:57:47 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65868;
+unicode = 224;
 },
 {
-glyphname = "onethousandtalents-atticGreek";
+glyphname = amacron;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65869;
+unicode = 257;
 },
 {
-glyphname = "fivethousandtalents-atticGreek";
+glyphname = eacute;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65870;
+unicode = 233;
 },
 {
-glyphname = "fivestaters-atticGreek";
+color = 3;
+glyphname = ebreve;
+lastChange = "2022-04-29 09:57:47 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65871;
+unicode = 277;
 },
 {
-glyphname = "tenstaters-atticGreek";
+glyphname = ecaron;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65872;
+unicode = 283;
 },
 {
-glyphname = "fiftystaters-atticGreek";
+color = 3;
+glyphname = ecircumflex;
+lastChange = "2022-04-29 09:57:47 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65873;
+unicode = 234;
 },
 {
-glyphname = "onehundredstaters-atticGreek";
+color = 3;
+glyphname = egrave;
+lastChange = "2022-04-29 09:57:47 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65874;
+unicode = 232;
 },
 {
-glyphname = "fivehundredstaters-atticGreek";
+color = 3;
+glyphname = emacron;
+lastChange = "2022-04-29 09:57:47 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65875;
+unicode = 275;
 },
 {
-glyphname = "onethousandstaters-atticGreek";
+glyphname = iacute;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65876;
+unicode = 237;
 },
 {
-glyphname = "tenthousandstaters-atticGreek";
+color = 3;
+glyphname = ibreve;
+lastChange = "2022-04-29 09:57:47 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65877;
+unicode = 301;
 },
 {
-glyphname = "fiftythousandstaters-atticGreek";
+glyphname = icaron;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65878;
+unicode = 464;
 },
 {
-glyphname = "tenmnas-atticGreek";
+color = 3;
+glyphname = icircumflex;
+lastChange = "2022-04-29 09:57:47 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65879;
+unicode = 238;
 },
 {
-glyphname = "heraeumoneplethron-ancientGreek";
+color = 3;
+glyphname = igrave;
+lastChange = "2022-04-29 09:57:47 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65880;
+unicode = 236;
 },
 {
-glyphname = "thespianone-ancientGreek";
+color = 3;
+glyphname = igrave;
+lastChange = "2022-04-29 09:57:47 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65881;
+unicode = 236;
 },
 {
-glyphname = "hermionianone-ancientGreek";
+color = 3;
+glyphname = imacron;
+lastChange = "2022-04-29 09:57:47 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65882;
+unicode = 299;
 },
 {
-glyphname = "epidaureantwo-ancientGreek";
+color = 3;
+glyphname = macute;
+lastChange = "2022-04-29 09:57:47 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65883;
+unicode = 7743;
 },
 {
-glyphname = "thespiantwo-ancientGreek";
+color = 3;
+glyphname = ngrave;
+lastChange = "2022-04-29 09:57:47 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65884;
+unicode = 505;
 },
 {
-glyphname = "cyrenaictwodrachmas-ancientGreek";
+color = 3;
+glyphname = ntilde;
+lastChange = "2022-04-29 09:57:47 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65885;
+unicode = 241;
 },
 {
-glyphname = "epidaureantwodrachmas-ancientGreek";
+color = 3;
+glyphname = oacute;
+lastChange = "2022-04-29 09:57:47 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65886;
+unicode = 243;
 },
 {
-glyphname = "troezenianfive-ancientGreek";
+color = 3;
+glyphname = obreve;
+lastChange = "2022-04-29 09:57:47 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65887;
+unicode = 335;
 },
 {
-glyphname = "troezenianten-ancientGreek";
+glyphname = ocaron;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65888;
+unicode = 466;
 },
 {
-glyphname = "troezeniantenalternateform-ancientGreek";
+color = 3;
+glyphname = ocircumflex;
+lastChange = "2022-04-29 09:57:47 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65889;
+unicode = 244;
 },
 {
-glyphname = "hermionianten-ancientGreek";
+color = 3;
+glyphname = ograve;
+lastChange = "2022-04-29 09:57:47 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65890;
+unicode = 242;
 },
 {
-glyphname = "messenianten-ancientGreek";
+color = 3;
+glyphname = omacron;
+lastChange = "2022-04-29 09:57:47 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65891;
+unicode = 333;
 },
 {
-glyphname = "thespianten-ancientGreek";
+color = 3;
+glyphname = uacute;
+lastChange = "2022-04-29 09:57:47 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65892;
+unicode = 250;
 },
 {
-glyphname = "thespianthirty-ancientGreek";
+color = 3;
+glyphname = ubreve;
+lastChange = "2022-04-29 09:57:47 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65893;
+unicode = 365;
 },
 {
-glyphname = "troezenianfifty-ancientGreek";
+glyphname = ucaron;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65894;
+unicode = 468;
 },
 {
-glyphname = "troezenianfiftyalternateform-ancientGreek";
+color = 3;
+glyphname = ucircumflex;
+lastChange = "2022-04-29 09:57:47 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65895;
+unicode = 251;
 },
 {
-glyphname = "hermionianfifty-ancientGreek";
+glyphname = udieresis;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65896;
+unicode = 252;
 },
 {
-glyphname = "thespianfifty-ancientGreek";
+glyphname = udieresisacute;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65897;
+unicode = 472;
 },
 {
-glyphname = "thespianonehundred-ancientGreek";
+glyphname = udieresiscaron;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65898;
+unicode = 474;
 },
 {
-glyphname = "thespianthreehundred-ancientGreek";
+glyphname = udieresisgrave;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65899;
+unicode = 476;
 },
 {
-glyphname = "epidaureanfivehundred-ancientGreek";
+glyphname = udieresismacron;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65900;
+unicode = 470;
 },
 {
-glyphname = "troezenianfivehundred-ancientGreek";
+color = 3;
+glyphname = ugrave;
+lastChange = "2022-04-29 09:57:47 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65901;
+unicode = 249;
 },
 {
-glyphname = "thespianfivehundred-ancientGreek";
+color = 3;
+glyphname = umacron;
+lastChange = "2022-04-29 09:57:47 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65902;
+unicode = 363;
 },
 {
-glyphname = "carystianfivehundred-ancientGreek";
+color = 3;
+glyphname = nmod;
+lastChange = "2022-04-29 09:49:06 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65903;
+unicode = 8319;
 },
 {
-glyphname = "naxianfivehundred-ancientGreek";
+color = 3;
+glyphname = Nmod;
+lastChange = "2022-04-29 09:47:49 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65904;
+unicode = 7482;
 },
 {
-glyphname = "thespianonethousand-ancientGreek";
+glyphname = dieresiscomb;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65905;
+unicode = 776;
 },
 {
-glyphname = "thespianfivethousand-ancientGreek";
+glyphname = gravecomb;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65906;
+unicode = 768;
 },
 {
-glyphname = "delphicfivemnas-ancientGreek";
+color = 3;
+glyphname = gravecomb_dotaboverightcomb;
+lastChange = "2022-04-29 09:38:36 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65907;
 },
 {
-glyphname = "stratianfiftymnas-ancientGreek";
+glyphname = acutecomb;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65908;
+unicode = 769;
 },
 {
-glyphname = "onehalf-greek";
+color = 3;
+glyphname = acutecomb_dotaboverightcomb;
+lastChange = "2022-04-29 09:38:36 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65909;
 },
 {
-glyphname = "onehalfAlternate-greek";
+glyphname = circumflexcomb;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65910;
+unicode = 770;
 },
 {
-glyphname = "twothirds-greek";
+color = 3;
+glyphname = circumflexcomb_dotaboverightcomb;
+lastChange = "2022-04-29 09:38:36 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65911;
 },
 {
-glyphname = "threequarters-greek";
+glyphname = caroncomb;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65912;
+unicode = 780;
 },
 {
-glyphname = "zero-greek";
+color = 3;
+glyphname = brevecomb;
+lastChange = "2022-04-29 09:54:41 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65930;
+unicode = 774;
 },
 {
-glyphname = "year-greek";
+color = 3;
+glyphname = brevecomb_dotaboverightcomb;
+lastChange = "2022-04-29 09:39:46 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65913;
 },
 {
-glyphname = "talent-greek";
+glyphname = macroncomb;
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65914;
+unicode = 772;
 },
 {
-glyphname = "drachma-greek";
+color = 3;
+glyphname = macroncomb_dotaboverightcomb;
+lastChange = "2022-04-29 09:38:54 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65915;
 },
 {
-glyphname = "obol-greek";
+color = 3;
+glyphname = verticallineabovecomb;
+lastChange = "2022-04-29 09:35:43 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65916;
+unicode = 781;
 },
 {
-glyphname = "twoObols-greek";
+color = 3;
+glyphname = verticallineabovecomb_dotaboverightcomb;
+lastChange = "2022-04-29 09:39:27 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65917;
 },
 {
-glyphname = "threeObols-greek";
+color = 3;
+glyphname = dotaboverightcomb;
+lastChange = "2022-04-29 09:38:36 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65918;
+unicode = 856;
 },
 {
-glyphname = "fourObols-greek";
+color = 3;
+glyphname = apostrophemod;
+lastChange = "2022-04-29 09:38:36 +0000";
 layers = (
 {
 layerId = m01;
 width = 600;
 }
 );
-unicode = 65919;
-},
-{
-glyphname = "fiveObols-greek";
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-unicode = 65920;
-},
-{
-glyphname = "metretes-greek";
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-unicode = 65921;
-},
-{
-glyphname = "kyathosBase-greek";
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-unicode = 65922;
-},
-{
-glyphname = "litra-greek";
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-unicode = 65923;
-},
-{
-glyphname = "ounkia-greek";
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-unicode = 65924;
-},
-{
-glyphname = "xestes-greek";
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-unicode = 65925;
-},
-{
-glyphname = "artabe-greek";
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-unicode = 65926;
-},
-{
-glyphname = "aroura-greek";
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-unicode = 65927;
-},
-{
-glyphname = "gramma-greek";
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-unicode = 65928;
-},
-{
-glyphname = "tryblionBase-greek";
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-unicode = 65929;
-},
-{
-glyphname = epsilonLunateReversedSymbol;
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-unicode = 1014;
-},
-{
-glyphname = sunSymbol;
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-unicode = 9737;
-},
-{
-glyphname = blackstar;
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-unicode = 9733;
-},
-{
-glyphname = ascendingNode;
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-unicode = 9738;
-},
-{
-glyphname = descendingNode;
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-unicode = 9739;
-},
-{
-glyphname = conjunction;
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-unicode = 9740;
-},
-{
-glyphname = opposition;
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-unicode = 9741;
-},
-{
-glyphname = constantineCross;
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-unicode = 9767;
-},
-{
-glyphname = jerusalemCross;
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-unicode = 9769;
-},
-{
-glyphname = firstQuarterMoon;
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-unicode = 9789;
-},
-{
-glyphname = lastQuarterMoon;
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-unicode = 9790;
-},
-{
-glyphname = mercury;
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-unicode = 9791;
-},
-{
-glyphname = venus;
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-unicode = 9792;
-},
-{
-glyphname = earth;
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-unicode = 9793;
-},
-{
-glyphname = mars;
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-unicode = 9794;
-},
-{
-glyphname = jupiter;
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-unicode = 9795;
-},
-{
-glyphname = saturn;
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-unicode = 9796;
-},
-{
-glyphname = uranus;
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-unicode = 9797;
-},
-{
-glyphname = neptune;
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-unicode = 9798;
-},
-{
-glyphname = pluto;
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-unicode = 9799;
-},
-{
-glyphname = aries;
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-unicode = 9800;
-},
-{
-glyphname = taurus;
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-unicode = 9801;
-},
-{
-glyphname = gemini;
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-unicode = 9802;
-},
-{
-glyphname = cancer;
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-unicode = 9803;
-},
-{
-glyphname = leo;
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-unicode = 9804;
-},
-{
-glyphname = virgo;
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-unicode = 9805;
-},
-{
-glyphname = libra;
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-unicode = 9806;
-},
-{
-glyphname = scorpius;
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-unicode = 9807;
-},
-{
-glyphname = sagittarius;
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-unicode = 9808;
-},
-{
-glyphname = capricorn;
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-unicode = 9809;
-},
-{
-glyphname = aquarius;
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-unicode = 9810;
-},
-{
-glyphname = pisces;
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-unicode = 9811;
-},
-{
-glyphname = threeDimensionalAngle;
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-unicode = 10176;
-},
-{
-glyphname = whitetrianglecontainingwhitetriangle;
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-unicode = 10177;
-},
-{
-glyphname = whiteSquare;
-layers = (
-{
-layerId = m01;
-width = 600;
-}
-);
-unicode = 9633;
+unicode = 700;
 }
 );
 metrics = (
 {
 type = ascender;
 },
 {
```

### Comparing `glyphsets-0.6.8/GF_glyphsets/Greek/glyphs/GF_Greek_Coptic.glyphs` & `glyphsets-0.6.9/GF_glyphsets/Greek/glyphs/GF_Greek_Coptic.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Greek/glyphs/GF_Greek_Core.glyphs` & `glyphsets-0.6.9/GF_glyphsets/Greek/glyphs/GF_Greek_Core.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Greek/glyphs/GF_Greek_Expert.glyphs` & `glyphsets-0.6.9/GF_glyphsets/Greek/glyphs/GF_Greek_Expert.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Greek/glyphs/GF_Greek_Plus.glyphs` & `glyphsets-0.6.9/GF_glyphsets/Greek/glyphs/GF_Greek_Plus.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Greek/glyphs/GF_Greek_Pro.glyphs` & `glyphsets-0.6.9/GF_glyphsets/Greek/glyphs/GF_Greek_Pro.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Greek/nam/GF_Greek_AncientMusicalSymbols.nam` & `glyphsets-0.6.9/GF_glyphsets/Greek/nam/GF_Greek_AncientMusicalSymbols.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Greek/nam/GF_Greek_Archaic.nam` & `glyphsets-0.6.9/GF_glyphsets/Greek/nam/GF_Greek_Archaic.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Greek/nam/GF_Greek_Coptic.nam` & `glyphsets-0.6.9/GF_glyphsets/Greek/nam/GF_Greek_Coptic.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Greek/nam/GF_Greek_Core.nam` & `glyphsets-0.6.9/GF_glyphsets/Greek/nam/GF_Greek_Core.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Greek/nam/GF_Greek_Plus.nam` & `glyphsets-0.6.9/GF_glyphsets/Greek/nam/GF_Greek_Plus.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Greek/nam/GF_Greek_Pro.nam` & `glyphsets-0.6.9/GF_glyphsets/Greek/nam/GF_Greek_Pro.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Greek/txt/nice-names/GF_Greek_AncientMusicalSymbols.txt` & `glyphsets-0.6.9/GF_glyphsets/Greek/txt/nice-names/GF_Greek_AncientMusicalSymbols.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Archaic.txt` & `glyphsets-0.6.9/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Archaic.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Coptic.txt` & `glyphsets-0.6.9/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Coptic.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Core.txt` & `glyphsets-0.6.9/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Core.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Expert.txt` & `glyphsets-0.6.9/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Expert.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Plus.txt` & `glyphsets-0.6.9/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Plus.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Pro.txt` & `glyphsets-0.6.9/GF_glyphsets/Greek/txt/nice-names/GF_Greek_Pro.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Greek/txt/prod-names/GF_Greek_AncientMusicalSymbols.txt` & `glyphsets-0.6.9/GF_glyphsets/Greek/txt/prod-names/GF_Greek_AncientMusicalSymbols.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Archaic.txt` & `glyphsets-0.6.9/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Archaic.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Coptic.txt` & `glyphsets-0.6.9/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Coptic.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Core.txt` & `glyphsets-0.6.9/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Core.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Expert.txt` & `glyphsets-0.6.9/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Expert.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Plus.txt` & `glyphsets-0.6.9/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Plus.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Pro.txt` & `glyphsets-0.6.9/GF_glyphsets/Greek/txt/prod-names/GF_Greek_Pro.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Latin/README.md` & `glyphsets-0.6.9/GF_glyphsets/Latin/README.md`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Latin/definitions/GF_Latin_Core.stub.glyphs` & `glyphsets-0.6.9/GF_glyphsets/Latin/definitions/GF_Latin_Core.stub.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Latin/definitions/GF_Latin_Core.stub.nam` & `glyphsets-0.6.9/GF_glyphsets/Latin/definitions/GF_Latin_Core.stub.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Latin/definitions/GF_Latin_Kernel.stub.nam` & `glyphsets-0.6.9/GF_glyphsets/Latin/nam/GF_Latin_Kernel.nam`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -109,8 +109,8 @@
 0x2019 RIGHT SINGLE QUOTATION MARK
 0x201C LEFT DOUBLE QUOTATION MARK
 0x201D RIGHT DOUBLE QUOTATION MARK
 0x2022 BULLET
 0x2026 HORIZONTAL ELLIPSIS
 0x20AC EURO SIGN
 0x2122 TRADE MARK SIGN
-0x2212 MINUS SIGN
+0x2212 MINUS SIGN
```

### Comparing `glyphsets-0.6.8/GF_glyphsets/Latin/glyphs/CustomFilter_GF_Latin.plist` & `glyphsets-0.6.9/GF_glyphsets/Latin/glyphs/CustomFilter_GF_Latin.plist`

 * *Files 0% similar despite different names*

#### Comparing `glyphsets-0.6.8/GF_glyphsets/Latin/glyphs/CustomFilter_GF_Latin.plist` & `glyphsets-0.6.9/GF_glyphsets/Latin/glyphs/CustomFilter_GF_Latin.plist`

```diff
@@ -780,14 +780,16 @@
         <string>gbreve</string>
         <string>Gdotaccent</string>
         <string>gdotaccent</string>
         <string>Gcommaaccent</string>
         <string>gcommaaccent</string>
         <string>Hbar</string>
         <string>hbar</string>
+        <string>Itilde</string>
+        <string>itilde</string>
         <string>Imacron</string>
         <string>imacron</string>
         <string>Iogonek</string>
         <string>iogonek</string>
         <string>Idotaccent</string>
         <string>idotless</string>
         <string>Kcommaaccent</string>
@@ -818,14 +820,16 @@
         <string>sacute</string>
         <string>Scedilla</string>
         <string>scedilla</string>
         <string>Scaron</string>
         <string>scaron</string>
         <string>Tcaron</string>
         <string>tcaron</string>
+        <string>Utilde</string>
+        <string>utilde</string>
         <string>Umacron</string>
         <string>umacron</string>
         <string>Uring</string>
         <string>uring</string>
         <string>Uhungarumlaut</string>
         <string>uhungarumlaut</string>
         <string>Uogonek</string>
@@ -842,14 +846,15 @@
         <string>Zcaron</string>
         <string>zcaron</string>
         <string>Scommaaccent</string>
         <string>scommaaccent</string>
         <string>Tcommaaccent</string>
         <string>tcommaaccent</string>
         <string>jdotless</string>
+        <string>apostrophemod</string>
         <string>circumflex</string>
         <string>caron</string>
         <string>breve</string>
         <string>dotaccent</string>
         <string>ring</string>
         <string>ogonek</string>
         <string>tilde</string>
@@ -871,16 +876,20 @@
         <string>Wgrave</string>
         <string>wgrave</string>
         <string>Wacute</string>
         <string>wacute</string>
         <string>Wdieresis</string>
         <string>wdieresis</string>
         <string>Germandbls</string>
+        <string>Etilde</string>
+        <string>etilde</string>
         <string>Ygrave</string>
         <string>ygrave</string>
+        <string>Ytilde</string>
+        <string>ytilde</string>
         <string>endash</string>
         <string>emdash</string>
         <string>quoteleft</string>
         <string>quoteright</string>
         <string>quotesinglbase</string>
         <string>quotedblleft</string>
         <string>quotedblright</string>
@@ -900,47 +909,56 @@
       </array>
       <key>name</key>
       <string>GF_Latin_Core</string>
     </dict>
     <dict>
       <key>list</key>
       <array>
-        <string>space</string>
-        <string>exclam</string>
-        <string>quotedbl</string>
-        <string>numbersign</string>
-        <string>dollar</string>
-        <string>percent</string>
-        <string>ampersand</string>
-        <string>quotesingle</string>
-        <string>parenleft</string>
-        <string>parenright</string>
-        <string>asterisk</string>
-        <string>plus</string>
-        <string>comma</string>
-        <string>hyphen</string>
-        <string>period</string>
-        <string>slash</string>
         <string>zero</string>
         <string>one</string>
         <string>two</string>
         <string>three</string>
         <string>four</string>
         <string>five</string>
         <string>six</string>
         <string>seven</string>
         <string>eight</string>
         <string>nine</string>
+        <string>space</string>
+        <string>nbspace</string>
+        <string>period</string>
         <string>colon</string>
-        <string>semicolon</string>
-        <string>less</string>
+        <string>ellipsis</string>
+        <string>exclam</string>
+        <string>asterisk</string>
+        <string>numbersign</string>
+        <string>slash</string>
+        <string>backslash</string>
+        <string>hyphen</string>
+        <string>parenleft</string>
+        <string>parenright</string>
+        <string>braceleft</string>
+        <string>braceright</string>
+        <string>bracketleft</string>
+        <string>bracketright</string>
+        <string>quotedblleft</string>
+        <string>quotedblright</string>
+        <string>quoteleft</string>
+        <string>quoteright</string>
+        <string>quotedbl</string>
+        <string>quotesingle</string>
+        <string>bar</string>
+        <string>plus</string>
+        <string>multiply</string>
+        <string>divide</string>
         <string>equal</string>
         <string>greater</string>
-        <string>question</string>
-        <string>at</string>
+        <string>less</string>
+        <string>percent</string>
+        <string>degree</string>
         <string>A</string>
         <string>B</string>
         <string>C</string>
         <string>D</string>
         <string>E</string>
         <string>F</string>
         <string>G</string>
@@ -959,20 +977,14 @@
         <string>T</string>
         <string>U</string>
         <string>V</string>
         <string>W</string>
         <string>X</string>
         <string>Y</string>
         <string>Z</string>
-        <string>bracketleft</string>
-        <string>backslash</string>
-        <string>bracketright</string>
-        <string>asciicircum</string>
-        <string>underscore</string>
-        <string>grave</string>
         <string>a</string>
         <string>b</string>
         <string>c</string>
         <string>d</string>
         <string>e</string>
         <string>f</string>
         <string>g</string>
@@ -991,39 +1003,37 @@
         <string>t</string>
         <string>u</string>
         <string>v</string>
         <string>w</string>
         <string>x</string>
         <string>y</string>
         <string>z</string>
-        <string>braceleft</string>
-        <string>bar</string>
-        <string>braceright</string>
-        <string>asciitilde</string>
-        <string>nbspace</string>
-        <string>cent</string>
-        <string>sterling</string>
-        <string>yen</string>
-        <string>copyright</string>
-        <string>registered</string>
-        <string>degree</string>
+        <string>.notdef</string>
+        <string>comma</string>
+        <string>semicolon</string>
+        <string>question</string>
         <string>periodcentered</string>
-        <string>multiply</string>
-        <string>divide</string>
+        <string>bullet</string>
         <string>endash</string>
         <string>emdash</string>
-        <string>quoteleft</string>
-        <string>quoteright</string>
-        <string>quotedblleft</string>
-        <string>quotedblright</string>
-        <string>bullet</string>
-        <string>ellipsis</string>
-        <string>euro</string>
+        <string>underscore</string>
+        <string>at</string>
+        <string>ampersand</string>
+        <string>copyright</string>
+        <string>registered</string>
         <string>trademark</string>
+        <string>cent</string>
+        <string>dollar</string>
+        <string>euro</string>
+        <string>sterling</string>
+        <string>yen</string>
         <string>minus</string>
+        <string>asciitilde</string>
+        <string>asciicircum</string>
+        <string>grave</string>
       </array>
       <key>name</key>
       <string>GF_Latin_Kernel</string>
     </dict>
     <dict>
       <key>list</key>
       <array>
```

### Comparing `glyphsets-0.6.8/GF_glyphsets/Latin/glyphs/GF_Latin_African.glyphs` & `glyphsets-0.6.9/GF_glyphsets/Latin/glyphs/GF_Latin_African.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Latin/glyphs/GF_Latin_Beyond.glyphs` & `glyphsets-0.6.9/GF_glyphsets/Latin/glyphs/GF_Latin_Beyond.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Latin/glyphs/GF_Latin_Core.glyphs` & `glyphsets-0.6.9/GF_glyphsets/Latin/glyphs/GF_Latin_Core.glyphs`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,10 @@
 {
 .appVersion = "3151";
 .formatVersion = 3;
-axes = (
-{
-name = Weight;
-tag = wght;
-},
-{
-name = Width;
-tag = wdth;
-}
-);
 date = "2021-10-28 12:22:31 +0000";
 familyName = "GF Latin Core";
 featurePrefixes = (
 {
 automatic = 1;
 code = "languagesystem DFLT dflt;
 
@@ -98,18 +88,14 @@
 code = "sub periodcentered.loclCAT by periodcentered.loclCAT.case;
 ";
 tag = case;
 }
 );
 fontMaster = (
 {
-axesValues = (
-100,
-100
-);
 id = m01;
 metricValues = (
 {
 over = 16;
 pos = 800;
 },
 {
@@ -485,14 +471,18 @@
 unicode = 180;
 },
 {
 glyphname = cedilla;
 unicode = 184;
 },
 {
+glyphname = apostrophemod;
+unicode = 700;
+},
+{
 glyphname = circumflex;
 unicode = 710;
 },
 {
 glyphname = caron;
 unicode = 711;
 },
@@ -1175,14 +1165,22 @@
 unicode = 294;
 },
 {
 glyphname = hbar;
 unicode = 295;
 },
 {
+glyphname = Itilde;
+unicode = 296;
+},
+{
+glyphname = itilde;
+unicode = 297;
+},
+{
 glyphname = Imacron;
 unicode = 298;
 },
 {
 glyphname = imacron;
 unicode = 299;
 },
@@ -1327,14 +1325,22 @@
 unicode = 356;
 },
 {
 glyphname = tcaron;
 unicode = 357;
 },
 {
+glyphname = Utilde;
+unicode = 360;
+},
+{
+glyphname = utilde;
+unicode = 361;
+},
+{
 glyphname = Umacron;
 unicode = 362;
 },
 {
 glyphname = umacron;
 unicode = 363;
 },
@@ -1451,20 +1457,36 @@
 unicode = 7813;
 },
 {
 glyphname = Germandbls;
 unicode = 7838;
 },
 {
+glyphname = Etilde;
+unicode = 7868;
+},
+{
+glyphname = etilde;
+unicode = 7869;
+},
+{
 glyphname = Ygrave;
 unicode = 7922;
 },
 {
 glyphname = ygrave;
 unicode = 7923;
+},
+{
+glyphname = Ytilde;
+unicode = 7928;
+},
+{
+glyphname = ytilde;
+unicode = 7929;
 }
 );
 instances = (
 );
 kerningLTR = {
 };
 metrics = (
```

### Comparing `glyphsets-0.6.8/GF_glyphsets/Latin/glyphs/GF_Latin_Kernel.glyphs` & `glyphsets-0.6.9/GF_glyphsets/Arabic/glyphs/GF_Arabic_Plus.glyphs`

 * *Files 22% similar despite different names*

```diff
@@ -1,545 +1,536 @@
 {
-.appVersion = "3151";
-.formatVersion = 3;
-axes = (
+.appVersion = "895";
+customParameters = (
 {
-name = Weight;
-tag = wght;
-},
-{
-name = Width;
-tag = wdth;
+name = Axes;
+value = (
+);
 }
 );
-date = "2023-12-13 14:28:10 +0000";
-familyName = GF_Latin_Kernel;
+familyName = GF_Arabic_Plus;
 fontMaster = (
-{
-axesValues = (
-100,
-100
 );
-id = m01;
-metricValues = (
+glyphs = (
 {
-over = 16;
-pos = 800;
+glyphname = percent;
+unicode = 0025;
 },
 {
-over = 16;
-pos = 700;
+glyphname = plus;
+unicode = 002B;
 },
 {
-over = 16;
-pos = 500;
+glyphname = "perthousand-ar";
+unicode = 0609;
 },
 {
-over = -16;
+glyphname = "percent-ar";
+unicode = 066A;
 },
 {
-over = -16;
-pos = -200;
+glyphname = "sindhipostpositionmen-ar";
+unicode = 06FE;
 },
 {
-over = -16;
-}
-);
-name = Regular;
-}
-);
-glyphs = (
+glyphname = minus;
+unicode = 2212;
+},
 {
-glyphname = dollar;
-unicode = 36;
+glyphname = lefttorightmark;
+unicode = 200E;
 },
 {
-glyphname = percent;
-unicode = 37;
+glyphname = righttoleftmark;
+unicode = 200F;
 },
 {
-glyphname = ampersand;
-unicode = 38;
+glyphname = exclam;
+unicode = 0021;
 },
 {
-glyphname = plus;
-unicode = 43;
+glyphname = quotesingle;
+unicode = 0027;
 },
 {
-glyphname = less;
-unicode = 60;
+glyphname = parenleft;
+unicode = 0028;
 },
 {
-glyphname = equal;
-unicode = 61;
+glyphname = parenright;
+unicode = 0029;
 },
 {
-glyphname = greater;
-unicode = 62;
+glyphname = comma;
+unicode = 002C;
 },
 {
-glyphname = at;
-unicode = 64;
+glyphname = hyphen;
+unicode = 002D;
 },
 {
-glyphname = asciicircum;
-unicode = 94;
+glyphname = period;
+unicode = 002E;
 },
 {
-glyphname = bar;
-unicode = 124;
+glyphname = slash;
+unicode = 002F;
 },
 {
-glyphname = asciitilde;
-unicode = 126;
+glyphname = colon;
+unicode = 003A;
 },
 {
-glyphname = cent;
-unicode = 162;
+glyphname = semicolon;
+unicode = 003B;
 },
 {
-glyphname = sterling;
-unicode = 163;
+glyphname = bracketleft;
+unicode = 005B;
 },
 {
-glyphname = yen;
-unicode = 165;
+glyphname = bracketright;
+unicode = 005D;
 },
 {
-glyphname = copyright;
-unicode = 169;
+glyphname = "comma-ar";
+unicode = 060C;
 },
 {
-glyphname = registered;
-unicode = 174;
+glyphname = "fullstop-ar";
+unicode = 06D4;
 },
 {
-glyphname = degree;
-unicode = 176;
+glyphname = "sindhiampersand-ar";
+unicode = 06FD;
 },
 {
-glyphname = multiply;
-unicode = 215;
+glyphname = quoteleft;
+unicode = 2018;
 },
 {
-glyphname = divide;
-unicode = 247;
+glyphname = zero;
+unicode = 0030;
 },
 {
-glyphname = euro;
-unicode = 8364;
+glyphname = one;
+unicode = 0031;
 },
 {
-glyphname = trademark;
-unicode = 8482;
+glyphname = two;
+unicode = 0032;
 },
 {
-glyphname = minus;
-unicode = 8722;
+glyphname = three;
+unicode = 0033;
 },
 {
-glyphname = space;
-unicode = 32;
+glyphname = four;
+unicode = 0034;
 },
 {
-glyphname = nbspace;
-unicode = 160;
+glyphname = five;
+unicode = 0035;
 },
 {
-glyphname = exclam;
-unicode = 33;
+glyphname = six;
+unicode = 0036;
 },
 {
-glyphname = quotedbl;
-unicode = 34;
+glyphname = seven;
+unicode = 0037;
 },
 {
-glyphname = numbersign;
-unicode = 35;
+glyphname = eight;
+unicode = 0038;
 },
 {
-glyphname = quotesingle;
-unicode = 39;
+glyphname = nine;
+unicode = 0039;
 },
 {
-glyphname = parenleft;
-unicode = 40;
+glyphname = "zero-ar";
+unicode = 0660;
 },
 {
-glyphname = parenright;
-unicode = 41;
+glyphname = "one-ar";
+unicode = 0661;
 },
 {
-glyphname = asterisk;
-unicode = 42;
+glyphname = "two-ar";
+unicode = 0662;
 },
 {
-glyphname = comma;
-unicode = 44;
+glyphname = "three-ar";
+unicode = 0663;
 },
 {
-glyphname = hyphen;
-unicode = 45;
+glyphname = "four-ar";
+unicode = 0664;
 },
 {
-glyphname = period;
-unicode = 46;
+glyphname = "five-ar";
+unicode = 0665;
 },
 {
-glyphname = slash;
-unicode = 47;
+glyphname = "six-ar";
+unicode = 0666;
 },
 {
-glyphname = colon;
-unicode = 58;
+glyphname = "seven-ar";
+unicode = 0667;
 },
 {
-glyphname = semicolon;
-unicode = 59;
+glyphname = "eight-ar";
+unicode = 0668;
 },
 {
-glyphname = question;
-unicode = 63;
+glyphname = "nine-ar";
+unicode = 0669;
 },
 {
-glyphname = bracketleft;
-unicode = 91;
+glyphname = "decimalseparator-ar";
+unicode = 066B;
 },
 {
-glyphname = backslash;
-unicode = 92;
+glyphname = "thousandseparator-ar";
+unicode = 066C;
 },
 {
-glyphname = bracketright;
-unicode = 93;
+glyphname = "zero-persian";
+unicode = 06F0;
 },
 {
-glyphname = underscore;
-unicode = 95;
+glyphname = "one-persian";
+unicode = 06F1;
 },
 {
-glyphname = braceleft;
-unicode = 123;
+glyphname = "two-persian";
+unicode = 06F2;
 },
 {
-glyphname = braceright;
-unicode = 125;
+glyphname = "three-persian";
+unicode = 06F3;
 },
 {
-glyphname = periodcentered;
-unicode = 183;
+glyphname = "four-persian";
+unicode = 06F4;
 },
 {
-glyphname = endash;
-unicode = 8211;
+glyphname = "five-persian";
+unicode = 06F5;
 },
 {
-glyphname = emdash;
-unicode = 8212;
+glyphname = "six-persian";
+unicode = 06F6;
 },
 {
-glyphname = quoteleft;
-unicode = 8216;
+glyphname = "seven-persian";
+unicode = 06F7;
 },
 {
-glyphname = quoteright;
-unicode = 8217;
+glyphname = "eight-persian";
+unicode = 06F8;
 },
 {
-glyphname = quotedblleft;
-unicode = 8220;
+glyphname = "nine-persian";
+unicode = 06F9;
 },
 {
-glyphname = quotedblright;
-unicode = 8221;
+glyphname = "fathatan-ar";
+unicode = 064B;
 },
 {
-glyphname = bullet;
-unicode = 8226;
+glyphname = "dammatan-ar";
+unicode = 064C;
 },
 {
-glyphname = ellipsis;
-unicode = 8230;
+glyphname = "kasratan-ar";
+unicode = 064D;
 },
 {
-glyphname = zero;
-unicode = 48;
+glyphname = "fatha-ar";
+unicode = 064E;
 },
 {
-glyphname = one;
-unicode = 49;
+glyphname = "damma-ar";
+unicode = 064F;
 },
 {
-glyphname = two;
-unicode = 50;
+glyphname = "kasra-ar";
+unicode = 0650;
 },
 {
-glyphname = three;
-unicode = 51;
+glyphname = "shadda-ar";
+unicode = 0651;
 },
 {
-glyphname = four;
-unicode = 52;
+glyphname = "sukun-ar";
+unicode = 0652;
 },
 {
-glyphname = five;
-unicode = 53;
+glyphname = "hamzaabove-ar";
+unicode = 0654;
 },
 {
-glyphname = six;
-unicode = 54;
+glyphname = "alefabove-ar";
+unicode = 0670;
 },
 {
-glyphname = seven;
-unicode = 55;
+glyphname = "hamza-ar";
+unicode = 0621;
 },
 {
-glyphname = eight;
-unicode = 56;
+glyphname = "alefMadda-ar";
+unicode = 0622;
 },
 {
-glyphname = nine;
-unicode = 57;
+glyphname = "alefHamzaabove-ar";
+unicode = 0623;
 },
 {
-glyphname = grave;
-unicode = 96;
+glyphname = "wawHamzaabove-ar";
+unicode = 0624;
 },
 {
-glyphname = A;
-unicode = 65;
+glyphname = "yehHamzaabove-ar";
+unicode = 0626;
 },
 {
-glyphname = B;
-unicode = 66;
+glyphname = "alef-ar";
+unicode = 0627;
 },
 {
-glyphname = C;
-unicode = 67;
+glyphname = "beh-ar";
+unicode = 0628;
 },
 {
-glyphname = D;
-unicode = 68;
+glyphname = "tehMarbuta-ar";
+unicode = 0629;
 },
 {
-glyphname = E;
-unicode = 69;
+glyphname = "teh-ar";
+unicode = 062A;
 },
 {
-glyphname = F;
-unicode = 70;
+glyphname = "theh-ar";
+unicode = 062B;
 },
 {
-glyphname = G;
-unicode = 71;
+glyphname = "jeem-ar";
+unicode = 062C;
 },
 {
-glyphname = H;
-unicode = 72;
+glyphname = "hah-ar";
+unicode = 062D;
 },
 {
-glyphname = I;
-unicode = 73;
+glyphname = "khah-ar";
+unicode = 062E;
 },
 {
-glyphname = J;
-unicode = 74;
+glyphname = "dal-ar";
+unicode = 062F;
 },
 {
-glyphname = K;
-unicode = 75;
+glyphname = "thal-ar";
+unicode = 0630;
 },
 {
-glyphname = L;
-unicode = 76;
+glyphname = "reh-ar";
+unicode = 0631;
 },
 {
-glyphname = M;
-unicode = 77;
+glyphname = "zain-ar";
+unicode = 0632;
 },
 {
-glyphname = N;
-unicode = 78;
+glyphname = "seen-ar";
+unicode = 0633;
 },
 {
-glyphname = O;
-unicode = 79;
+glyphname = "sheen-ar";
+unicode = 0634;
 },
 {
-glyphname = P;
-unicode = 80;
+glyphname = "sad-ar";
+unicode = 0635;
 },
 {
-glyphname = Q;
-unicode = 81;
+glyphname = "dad-ar";
+unicode = 0636;
 },
 {
-glyphname = R;
-unicode = 82;
+glyphname = "tah-ar";
+unicode = 0637;
 },
 {
-glyphname = S;
-unicode = 83;
+glyphname = "zah-ar";
+unicode = 0638;
 },
 {
-glyphname = T;
-unicode = 84;
+glyphname = "ain-ar";
+unicode = 0639;
 },
 {
-glyphname = U;
-unicode = 85;
+glyphname = "ghain-ar";
+unicode = 063A;
 },
 {
-glyphname = V;
-unicode = 86;
+glyphname = "feh-ar";
+unicode = 0641;
 },
 {
-glyphname = W;
-unicode = 87;
+glyphname = "qaf-ar";
+unicode = 0642;
 },
 {
-glyphname = X;
-unicode = 88;
+glyphname = "kaf-ar";
+unicode = 0643;
 },
 {
-glyphname = Y;
-unicode = 89;
+glyphname = "lam-ar";
+unicode = 0644;
 },
 {
-glyphname = Z;
-unicode = 90;
+glyphname = "meem-ar";
+unicode = 0645;
 },
 {
-glyphname = a;
-unicode = 97;
+glyphname = "noon-ar";
+unicode = 0646;
 },
 {
-glyphname = b;
-unicode = 98;
+glyphname = "heh-ar";
+unicode = 0647;
 },
 {
-glyphname = c;
-unicode = 99;
+glyphname = "waw-ar";
+unicode = 0648;
 },
 {
-glyphname = d;
-unicode = 100;
+glyphname = "alefMaksura-ar";
+unicode = 0649;
 },
 {
-glyphname = e;
-unicode = 101;
+glyphname = "yeh-ar";
+unicode = 064A;
 },
 {
-glyphname = f;
-unicode = 102;
+glyphname = "tehRing-ar";
+unicode = 067C;
 },
 {
-glyphname = g;
-unicode = 103;
+glyphname = "peh-ar";
+unicode = 067E;
 },
 {
-glyphname = h;
-unicode = 104;
+glyphname = "hahHamzaabove-ar";
+unicode = 0681;
 },
 {
-glyphname = i;
-unicode = 105;
+glyphname = "hahThreedotsabove-ar";
+unicode = 0685;
 },
 {
-glyphname = j;
-unicode = 106;
+glyphname = "tcheh-ar";
+unicode = 0686;
 },
 {
-glyphname = k;
-unicode = 107;
+glyphname = "dalRing-ar";
+unicode = 0689;
 },
 {
-glyphname = l;
-unicode = 108;
+glyphname = "rehRing-ar";
+unicode = 0693;
 },
 {
-glyphname = m;
-unicode = 109;
+glyphname = "rehVbelow-ar";
+unicode = 0695;
 },
 {
-glyphname = n;
-unicode = 110;
+glyphname = "rehDotbelowdotabove-ar";
+unicode = 0696;
 },
 {
-glyphname = o;
-unicode = 111;
+glyphname = "jeh-ar";
+unicode = 0698;
 },
 {
-glyphname = p;
-unicode = 112;
+glyphname = "seenDotbelowDotabove-ar";
+unicode = 069A;
 },
 {
-glyphname = q;
-unicode = 113;
+glyphname = "veh-ar";
+unicode = 06A4;
 },
 {
-glyphname = r;
-unicode = 114;
+glyphname = "keheh-ar";
+unicode = 06A9;
 },
 {
-glyphname = s;
-unicode = 115;
+glyphname = "kafRing-ar";
+unicode = 06AB;
 },
 {
-glyphname = t;
-unicode = 116;
+glyphname = "ng-ar";
+unicode = 06AD;
 },
 {
-glyphname = u;
-unicode = 117;
+glyphname = "gaf-ar";
+unicode = 06AF;
 },
 {
-glyphname = v;
-unicode = 118;
+glyphname = "lamVabove-ar";
+unicode = 06B5;
 },
 {
-glyphname = w;
-unicode = 119;
+glyphname = "noonRing-ar";
+unicode = 06BC;
 },
 {
-glyphname = x;
-unicode = 120;
+glyphname = "hehDoachashmee-ar";
+unicode = 06BE;
 },
 {
-glyphname = y;
-unicode = 121;
+glyphname = "oe-ar";
+unicode = 06C6;
 },
 {
-glyphname = z;
-unicode = 122;
-}
-);
-instances = (
-);
-kerningLTR = {
-};
-metrics = (
+glyphname = "u-ar";
+unicode = 06C7;
+},
+{
+glyphname = "yu-ar";
+unicode = 06C8;
+},
 {
-type = ascender;
+glyphname = "ve-ar";
+unicode = 06CB;
 },
 {
-type = "cap height";
+glyphname = "yeh-farsi";
+unicode = 06CC;
 },
 {
-type = "x-height";
+glyphname = "yehTail-ar";
+unicode = 06CD;
 },
 {
-type = baseline;
+glyphname = "yehVabove-ar";
+unicode = 06CE;
 },
 {
-type = descender;
+glyphname = "e-ar";
+unicode = 06D0;
 },
 {
-type = "italic angle";
+glyphname = "ae-ar";
+unicode = 06D5;
 }
 );
-stems = (
+instances = (
 );
 unitsPerEm = 1000;
 versionMajor = 1;
 versionMinor = 0;
 }
```

### Comparing `glyphsets-0.6.8/GF_glyphsets/Latin/glyphs/GF_Latin_Plus.glyphs` & `glyphsets-0.6.9/GF_glyphsets/Latin/glyphs/GF_Latin_Plus.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Latin/glyphs/GF_Latin_Vietnamese.glyphs` & `glyphsets-0.6.9/GF_glyphsets/Latin/glyphs/GF_Latin_Vietnamese.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Latin/nam/GF_Latin_African.nam` & `glyphsets-0.6.9/GF_glyphsets/Latin/nam/GF_Latin_African.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Latin/nam/GF_Latin_Beyond.nam` & `glyphsets-0.6.9/GF_glyphsets/Latin/nam/GF_Latin_Beyond.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Latin/nam/GF_Latin_Core.nam` & `glyphsets-0.6.9/GF_glyphsets/Latin/nam/GF_Latin_Core.nam`

 * *Files 2% similar despite different names*

```diff
@@ -206,14 +206,16 @@
 0x011F LATIN SMALL LETTER G WITH BREVE
 0x0120 LATIN CAPITAL LETTER G WITH DOT ABOVE
 0x0121 LATIN SMALL LETTER G WITH DOT ABOVE
 0x0122 LATIN CAPITAL LETTER G WITH CEDILLA
 0x0123 LATIN SMALL LETTER G WITH CEDILLA
 0x0126 LATIN CAPITAL LETTER H WITH STROKE
 0x0127 LATIN SMALL LETTER H WITH STROKE
+0x0128 LATIN CAPITAL LETTER I WITH TILDE
+0x0129 LATIN SMALL LETTER I WITH TILDE
 0x012A LATIN CAPITAL LETTER I WITH MACRON
 0x012B LATIN SMALL LETTER I WITH MACRON
 0x012E LATIN CAPITAL LETTER I WITH OGONEK
 0x012F LATIN SMALL LETTER I WITH OGONEK
 0x0130 LATIN CAPITAL LETTER I WITH DOT ABOVE
 0x0131 LATIN SMALL LETTER DOTLESS I
 0x0136 LATIN CAPITAL LETTER K WITH CEDILLA
@@ -244,14 +246,16 @@
 0x015B LATIN SMALL LETTER S WITH ACUTE
 0x015E LATIN CAPITAL LETTER S WITH CEDILLA
 0x015F LATIN SMALL LETTER S WITH CEDILLA
 0x0160 LATIN CAPITAL LETTER S WITH CARON
 0x0161 LATIN SMALL LETTER S WITH CARON
 0x0164 LATIN CAPITAL LETTER T WITH CARON
 0x0165 LATIN SMALL LETTER T WITH CARON
+0x0168 LATIN CAPITAL LETTER U WITH TILDE
+0x0169 LATIN SMALL LETTER U WITH TILDE
 0x016A LATIN CAPITAL LETTER U WITH MACRON
 0x016B LATIN SMALL LETTER U WITH MACRON
 0x016E LATIN CAPITAL LETTER U WITH RING ABOVE
 0x016F LATIN SMALL LETTER U WITH RING ABOVE
 0x0170 LATIN CAPITAL LETTER U WITH DOUBLE ACUTE
 0x0171 LATIN SMALL LETTER U WITH DOUBLE ACUTE
 0x0172 LATIN CAPITAL LETTER U WITH OGONEK
@@ -268,14 +272,15 @@
 0x017D LATIN CAPITAL LETTER Z WITH CARON
 0x017E LATIN SMALL LETTER Z WITH CARON
 0x0218 LATIN CAPITAL LETTER S WITH COMMA BELOW
 0x0219 LATIN SMALL LETTER S WITH COMMA BELOW
 0x021A LATIN CAPITAL LETTER T WITH COMMA BELOW
 0x021B LATIN SMALL LETTER T WITH COMMA BELOW
 0x0237 LATIN SMALL LETTER DOTLESS J
+0x02BC MODIFIER LETTER APOSTROPHE
 0x02C6 MODIFIER LETTER CIRCUMFLEX ACCENT
 0x02C7 CARON
 0x02D8 BREVE
 0x02D9 DOT ABOVE
 0x02DA RING ABOVE
 0x02DB OGONEK
 0x02DC SMALL TILDE
@@ -297,16 +302,20 @@
 0x1E80 LATIN CAPITAL LETTER W WITH GRAVE
 0x1E81 LATIN SMALL LETTER W WITH GRAVE
 0x1E82 LATIN CAPITAL LETTER W WITH ACUTE
 0x1E83 LATIN SMALL LETTER W WITH ACUTE
 0x1E84 LATIN CAPITAL LETTER W WITH DIAERESIS
 0x1E85 LATIN SMALL LETTER W WITH DIAERESIS
 0x1E9E LATIN CAPITAL LETTER SHARP S
+0x1EBC LATIN CAPITAL LETTER E WITH TILDE
+0x1EBD LATIN SMALL LETTER E WITH TILDE
 0x1EF2 LATIN CAPITAL LETTER Y WITH GRAVE
 0x1EF3 LATIN SMALL LETTER Y WITH GRAVE
+0x1EF8 LATIN CAPITAL LETTER Y WITH TILDE
+0x1EF9 LATIN SMALL LETTER Y WITH TILDE
 0x2013 EN DASH
 0x2014 EM DASH
 0x2018 LEFT SINGLE QUOTATION MARK
 0x2019 RIGHT SINGLE QUOTATION MARK
 0x201A SINGLE LOW-9 QUOTATION MARK
 0x201C LEFT DOUBLE QUOTATION MARK
 0x201D RIGHT DOUBLE QUOTATION MARK
```

### Comparing `glyphsets-0.6.8/GF_glyphsets/Latin/nam/GF_Latin_Plus.nam` & `glyphsets-0.6.9/GF_glyphsets/Latin/nam/GF_Latin_Plus.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Latin/nam/GF_Latin_Vietnamese.nam` & `glyphsets-0.6.9/GF_glyphsets/Latin/nam/GF_Latin_Vietnamese.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Latin/txt/nice-names/GF_Latin_African.txt` & `glyphsets-0.6.9/GF_glyphsets/Latin/txt/nice-names/GF_Latin_African.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Beyond.txt` & `glyphsets-0.6.9/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Beyond.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Core.txt` & `glyphsets-0.6.9/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Core.txt`

 * *Files 4% similar despite different names*

```diff
@@ -206,14 +206,16 @@
 gbreve
 Gdotaccent
 gdotaccent
 Gcommaaccent
 gcommaaccent
 Hbar
 hbar
+Itilde
+itilde
 Imacron
 imacron
 Iogonek
 iogonek
 Idotaccent
 idotless
 Kcommaaccent
@@ -244,14 +246,16 @@
 sacute
 Scedilla
 scedilla
 Scaron
 scaron
 Tcaron
 tcaron
+Utilde
+utilde
 Umacron
 umacron
 Uring
 uring
 Uhungarumlaut
 uhungarumlaut
 Uogonek
@@ -268,14 +272,15 @@
 Zcaron
 zcaron
 Scommaaccent
 scommaaccent
 Tcommaaccent
 tcommaaccent
 jdotless
+apostrophemod
 circumflex
 caron
 breve
 dotaccent
 ring
 ogonek
 tilde
@@ -297,16 +302,20 @@
 Wgrave
 wgrave
 Wacute
 wacute
 Wdieresis
 wdieresis
 Germandbls
+Etilde
+etilde
 Ygrave
 ygrave
+Ytilde
+ytilde
 endash
 emdash
 quoteleft
 quoteright
 quotesinglbase
 quotedblleft
 quotedblright
```

### Comparing `glyphsets-0.6.8/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Plus.txt` & `glyphsets-0.6.9/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Plus.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Vietnamese.txt` & `glyphsets-0.6.9/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Vietnamese.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Latin/txt/prod-names/GF_Latin_African.txt` & `glyphsets-0.6.9/GF_glyphsets/Latin/txt/prod-names/GF_Latin_African.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Beyond.txt` & `glyphsets-0.6.9/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Beyond.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Core.txt` & `glyphsets-0.6.9/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Core.txt`

 * *Files 6% similar despite different names*

```diff
@@ -206,14 +206,16 @@
 gbreve
 Gdotaccent
 gdotaccent
 uni0122
 uni0123
 Hbar
 hbar
+Itilde
+itilde
 Imacron
 imacron
 Iogonek
 iogonek
 Idotaccent
 dotlessi
 uni0136
@@ -244,14 +246,16 @@
 sacute
 Scedilla
 scedilla
 Scaron
 scaron
 Tcaron
 tcaron
+Utilde
+utilde
 Umacron
 umacron
 Uring
 uring
 Uhungarumlaut
 uhungarumlaut
 Uogonek
@@ -268,14 +272,15 @@
 Zcaron
 zcaron
 uni0218
 uni0219
 uni021A
 uni021B
 uni0237
+uni02BC
 circumflex
 caron
 breve
 dotaccent
 ring
 ogonek
 tilde
@@ -297,16 +302,20 @@
 Wgrave
 wgrave
 Wacute
 wacute
 Wdieresis
 wdieresis
 uni1E9E
+uni1EBC
+uni1EBD
 Ygrave
 ygrave
+uni1EF8
+uni1EF9
 endash
 emdash
 quoteleft
 quoteright
 quotesinglbase
 quotedblleft
 quotedblright
```

### Comparing `glyphsets-0.6.8/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Kernel.txt` & `glyphsets-0.6.9/GF_glyphsets/Latin/txt/nice-names/GF_Latin_Kernel.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,41 +1,49 @@
-# This file is auto-generated; do not edit. See /README.md for instructions.
-space
-exclam
-quotedbl
-numbersign
-dollar
-percent
-ampersand
-quotesingle
-parenleft
-parenright
-asterisk
-plus
-comma
-hyphen
-period
-slash
 zero
 one
 two
 three
 four
 five
 six
 seven
 eight
 nine
+space
+nbspace
+period
 colon
-semicolon
-less
+ellipsis
+exclam
+asterisk
+numbersign
+slash
+backslash
+hyphen
+parenleft
+parenright
+braceleft
+braceright
+bracketleft
+bracketright
+quotedblleft
+quotedblright
+quoteleft
+quoteright
+quotedbl
+quotesingle
+bar
+plus
+multiply
+divide
 equal
 greater
-question
-at
+less
+percent
+degree
 A
 B
 C
 D
 E
 F
 G
@@ -54,20 +62,14 @@
 T
 U
 V
 W
 X
 Y
 Z
-bracketleft
-backslash
-bracketright
-asciicircum
-underscore
-grave
 a
 b
 c
 d
 e
 f
 g
@@ -86,32 +88,30 @@
 t
 u
 v
 w
 x
 y
 z
-braceleft
-bar
-braceright
-asciitilde
-uni00A0
-cent
-sterling
-yen
-copyright
-registered
-degree
+.notdef
+comma
+semicolon
+question
 periodcentered
-multiply
-divide
+bullet
 endash
 emdash
-quoteleft
-quoteright
-quotedblleft
-quotedblright
-bullet
-ellipsis
-Euro
+underscore
+at
+ampersand
+copyright
+registered
 trademark
-minus
+cent
+dollar
+euro
+sterling
+yen
+minus
+asciitilde
+asciicircum
+grave
```

### Comparing `glyphsets-0.6.8/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Plus.txt` & `glyphsets-0.6.9/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Plus.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Vietnamese.txt` & `glyphsets-0.6.9/GF_glyphsets/Latin/txt/prod-names/GF_Latin_Vietnamese.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Phonetics/glyphs/CustomFilter_GF_Phonetics.plist` & `glyphsets-0.6.9/GF_glyphsets/Phonetics/glyphs/CustomFilter_GF_Phonetics.plist`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_APA.glyphs` & `glyphsets-0.6.9/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_APA.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_DisorderedSpeech.glyphs` & `glyphsets-0.6.9/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_DisorderedSpeech.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_IPAHistorical.glyphs` & `glyphsets-0.6.9/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_IPAHistorical.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_IPAStandard.glyphs` & `glyphsets-0.6.9/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_IPAStandard.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_SinoExt.glyphs` & `glyphsets-0.6.9/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_SinoExt.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_UPA.glyphs` & `glyphsets-0.6.9/GF_glyphsets/Phonetics/glyphs/GF_Phonetics_UPA.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Phonetics/nam/GF_Phonetics_APA.nam` & `glyphsets-0.6.9/GF_glyphsets/Phonetics/nam/GF_Phonetics_APA.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Phonetics/nam/GF_Phonetics_DisorderedSpeech.nam` & `glyphsets-0.6.9/GF_glyphsets/Phonetics/nam/GF_Phonetics_DisorderedSpeech.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Phonetics/nam/GF_Phonetics_IPAStandard.nam` & `glyphsets-0.6.9/GF_glyphsets/Phonetics/nam/GF_Phonetics_IPAStandard.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Phonetics/txt/nice-names/GF_Phonetics_DisorderedSpeech.txt` & `glyphsets-0.6.9/GF_glyphsets/Phonetics/txt/nice-names/GF_Phonetics_DisorderedSpeech.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Phonetics/txt/nice-names/GF_Phonetics_IPAStandard.txt` & `glyphsets-0.6.9/GF_glyphsets/Phonetics/txt/nice-names/GF_Phonetics_IPAStandard.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Phonetics/txt/prod-names/GF_Phonetics_DisorderedSpeech.txt` & `glyphsets-0.6.9/GF_glyphsets/Phonetics/txt/prod-names/GF_Phonetics_DisorderedSpeech.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/Phonetics/txt/prod-names/GF_Phonetics_IPAStandard.txt` & `glyphsets-0.6.9/GF_glyphsets/Phonetics/txt/prod-names/GF_Phonetics_IPAStandard.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/README.md` & `glyphsets-0.6.9/GF_glyphsets/README.md`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/TransLatin/glyphs/CustomFilter_GF_TransLatin.plist` & `glyphsets-0.6.9/GF_glyphsets/TransLatin/glyphs/CustomFilter_GF_TransLatin.plist`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/TransLatin/glyphs/GF_TransLatin_Arabic.glyphs` & `glyphsets-0.6.9/GF_glyphsets/TransLatin/glyphs/GF_TransLatin_Arabic.glyphs`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/TransLatin/nam/GF_TransLatin_Arabic.nam` & `glyphsets-0.6.9/GF_glyphsets/TransLatin/nam/GF_TransLatin_Arabic.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/TransLatin/nam/GF_TransLatin_Pinyin.nam` & `glyphsets-0.6.9/GF_glyphsets/TransLatin/nam/GF_TransLatin_Pinyin.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/TransLatin/txt/nice-names/GF_TransLatin_Pinyin.txt` & `glyphsets-0.6.9/GF_glyphsets/TransLatin/txt/nice-names/GF_TransLatin_Pinyin.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/TransLatin/txt/prod-names/GF_TransLatin_Pinyin.txt` & `glyphsets-0.6.9/GF_glyphsets/TransLatin/txt/prod-names/GF_TransLatin_Pinyin.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/GF_glyphsets/update-gs.sh` & `glyphsets-0.6.9/GF_glyphsets/update-gs.sh`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/LICENSE` & `glyphsets-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/__init__.py` & `glyphsets-0.6.9/Lib/glyphsets/__init__.py`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/__main__.py` & `glyphsets-0.6.9/Lib/glyphsets/__main__.py`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/codepoints.py` & `glyphsets-0.6.9/Lib/glyphsets/codepoints.py`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/data.json` & `glyphsets-0.6.9/Lib/glyphsets/data.json`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/definitions/__init__.py` & `glyphsets-0.6.9/Lib/glyphsets/definitions/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,46 +1,65 @@
 # Google Fonts glyphset definitions to be consumed by other tools.
 # The "script" value needs to correspond to the folder name
 # in /GF_Glyphsets of this repo in order to find the other definition files.
 
 import os
 
 glyphset_definitions = {
-    "GF_Latin_Kernel": {"script": "Latin", "language_codes": []},
     "GF_Latin_Core": {
         "script": "Latin",
         "language_codes": [
             "ca_Latn",  # Catalan
             "cs_Latn",  # Czech
             "cy_Latn",  # Welsh
             "da_Latn",  # Danish
             "de_Latn",  # German
             "en_Latn",  # English
             "es_Latn",  # Spanish
             "fi_Latn",  # Finnish
             "fr_Latn",  # French
+            "gn_Latn",  # Guarani
             "hr_Latn",  # Croatian
             "hu_Latn",  # Hungarian
             "is_Latn",  # Icelandic
             "it_Latn",  # Italian
             "lt_Latn",  # Lithuanian
             "lv_Latn",  # Latvian
             "mt_Latn",  # Maltese
             "nb_Latn",  # Norwegian Bokmål
             "nl_Latn",  # Dutch
             "pl_Latn",  # Polish
             "pt_Latn",  # Portuguese
+            "qu_Latn",  # Quechua
             "ro_Latn",  # Romanian
             "sk_Latn",  # Slovak
             "sq_Latn",  # Albanian
             "sr_Latn",  # Serbian (Latin)
             "sv_Latn",  # Swedish
             "tr_Latn",  # Turkish
         ],
     },
+    "GF_Arabic_Core": {
+        "script": "Arabic",
+        "language_codes": [
+            "ar_Arab",  # Arabic
+            "fa_Arab",  # Persian
+            "ur_Arab",  # Urdu
+        ],
+    },
+    "GF_Arabic_Plus": {
+        "script": "Arabic",
+        "language_codes": [
+            "ckb_Arab",  # Kurdish
+            "ms_Arab",  # Malay
+            "ps_Arab",  # Pashto
+            "ps_Arab",  # Sindhi
+            "ug_Arab",  # Uyghur
+        ],
+    },
 }
 
 
 def unicodes_per_glyphset(glyphset_name):
     character_set = set()
     # Read .nam file
     nam_path = os.path.join(os.path.dirname(__file__), "nam", f"{glyphset_name}.nam")
```

### Comparing `glyphsets-0.6.8/Lib/glyphsets/definitions/nam/GF_Latin_Core.nam` & `glyphsets-0.6.9/Lib/glyphsets/definitions/nam/GF_Latin_Core.nam`

 * *Files 2% similar despite different names*

```diff
@@ -206,14 +206,16 @@
 0x011F LATIN SMALL LETTER G WITH BREVE
 0x0120 LATIN CAPITAL LETTER G WITH DOT ABOVE
 0x0121 LATIN SMALL LETTER G WITH DOT ABOVE
 0x0122 LATIN CAPITAL LETTER G WITH CEDILLA
 0x0123 LATIN SMALL LETTER G WITH CEDILLA
 0x0126 LATIN CAPITAL LETTER H WITH STROKE
 0x0127 LATIN SMALL LETTER H WITH STROKE
+0x0128 LATIN CAPITAL LETTER I WITH TILDE
+0x0129 LATIN SMALL LETTER I WITH TILDE
 0x012A LATIN CAPITAL LETTER I WITH MACRON
 0x012B LATIN SMALL LETTER I WITH MACRON
 0x012E LATIN CAPITAL LETTER I WITH OGONEK
 0x012F LATIN SMALL LETTER I WITH OGONEK
 0x0130 LATIN CAPITAL LETTER I WITH DOT ABOVE
 0x0131 LATIN SMALL LETTER DOTLESS I
 0x0136 LATIN CAPITAL LETTER K WITH CEDILLA
@@ -244,14 +246,16 @@
 0x015B LATIN SMALL LETTER S WITH ACUTE
 0x015E LATIN CAPITAL LETTER S WITH CEDILLA
 0x015F LATIN SMALL LETTER S WITH CEDILLA
 0x0160 LATIN CAPITAL LETTER S WITH CARON
 0x0161 LATIN SMALL LETTER S WITH CARON
 0x0164 LATIN CAPITAL LETTER T WITH CARON
 0x0165 LATIN SMALL LETTER T WITH CARON
+0x0168 LATIN CAPITAL LETTER U WITH TILDE
+0x0169 LATIN SMALL LETTER U WITH TILDE
 0x016A LATIN CAPITAL LETTER U WITH MACRON
 0x016B LATIN SMALL LETTER U WITH MACRON
 0x016E LATIN CAPITAL LETTER U WITH RING ABOVE
 0x016F LATIN SMALL LETTER U WITH RING ABOVE
 0x0170 LATIN CAPITAL LETTER U WITH DOUBLE ACUTE
 0x0171 LATIN SMALL LETTER U WITH DOUBLE ACUTE
 0x0172 LATIN CAPITAL LETTER U WITH OGONEK
@@ -268,14 +272,15 @@
 0x017D LATIN CAPITAL LETTER Z WITH CARON
 0x017E LATIN SMALL LETTER Z WITH CARON
 0x0218 LATIN CAPITAL LETTER S WITH COMMA BELOW
 0x0219 LATIN SMALL LETTER S WITH COMMA BELOW
 0x021A LATIN CAPITAL LETTER T WITH COMMA BELOW
 0x021B LATIN SMALL LETTER T WITH COMMA BELOW
 0x0237 LATIN SMALL LETTER DOTLESS J
+0x02BC MODIFIER LETTER APOSTROPHE
 0x02C6 MODIFIER LETTER CIRCUMFLEX ACCENT
 0x02C7 CARON
 0x02D8 BREVE
 0x02D9 DOT ABOVE
 0x02DA RING ABOVE
 0x02DB OGONEK
 0x02DC SMALL TILDE
@@ -297,16 +302,20 @@
 0x1E80 LATIN CAPITAL LETTER W WITH GRAVE
 0x1E81 LATIN SMALL LETTER W WITH GRAVE
 0x1E82 LATIN CAPITAL LETTER W WITH ACUTE
 0x1E83 LATIN SMALL LETTER W WITH ACUTE
 0x1E84 LATIN CAPITAL LETTER W WITH DIAERESIS
 0x1E85 LATIN SMALL LETTER W WITH DIAERESIS
 0x1E9E LATIN CAPITAL LETTER SHARP S
+0x1EBC LATIN CAPITAL LETTER E WITH TILDE
+0x1EBD LATIN SMALL LETTER E WITH TILDE
 0x1EF2 LATIN CAPITAL LETTER Y WITH GRAVE
 0x1EF3 LATIN SMALL LETTER Y WITH GRAVE
+0x1EF8 LATIN CAPITAL LETTER Y WITH TILDE
+0x1EF9 LATIN SMALL LETTER Y WITH TILDE
 0x2013 EN DASH
 0x2014 EM DASH
 0x2018 LEFT SINGLE QUOTATION MARK
 0x2019 RIGHT SINGLE QUOTATION MARK
 0x201A SINGLE LOW-9 QUOTATION MARK
 0x201C LEFT DOUBLE QUOTATION MARK
 0x201D RIGHT DOUBLE QUOTATION MARK
```

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/README.md` & `glyphsets-0.6.9/Lib/glyphsets/encodings/README.md`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/adlam_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/adlam_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/ahom_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/ahom_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/anatolian-hieroglyphs_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/anatolian-hieroglyphs_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/arabic_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/arabic_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/armenian_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/armenian_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/avestan_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/avestan_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/balinese_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/balinese_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/bamum_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/bamum_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/bassa-vah_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/bassa-vah_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/batak_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/batak_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/bengali_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/bengali_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/bhaiksuki_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/bhaiksuki_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/brahmi_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/brahmi_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/braille_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/braille_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/buginese_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/buginese_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/buhid_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/buhid_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/canadian-aboriginal_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/canadian-aboriginal_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/carian_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/carian_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/caucasian-albanian_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/caucasian-albanian_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/chakma_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/chakma_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/cham_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/cham_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/cherokee_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/cherokee_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/chinese-hongkong_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/chinese-hongkong_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/chinese-simplified_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/chinese-simplified_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/chinese-traditional_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/chinese-traditional_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/chorasmian_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/chorasmian_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/coptic_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/coptic_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/cuneiform_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/cuneiform_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/cypriot_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/cypriot_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/cypro-minoan_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/cypro-minoan_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/cyrillic-ext_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/cyrillic-ext_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/cyrillic_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/cyrillic_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/deseret_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/deseret_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/devanagari_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/devanagari_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/dives-akuru_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/dives-akuru_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/dogra_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/dogra_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/duployan_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/duployan_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/egyptian-hieroglyphs_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/egyptian-hieroglyphs_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/elbasan_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/elbasan_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/elymaic_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/elymaic_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/emoji_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/emoji_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/ethiopic_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/ethiopic_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/georgian_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/georgian_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/glagolitic_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/glagolitic_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/gothic_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/gothic_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/grantha_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/grantha_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/greek-ext_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/greek-ext_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/greek_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/greek_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/gujarati_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/gujarati_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/gunjala-gondi_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/gunjala-gondi_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/gurmukhi_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/gurmukhi_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/hanifi-rohingya_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/hanifi-rohingya_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/hanunoo_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/hanunoo_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/hatran_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/hatran_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/hebrew_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/hebrew_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/imperial-aramaic_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/imperial-aramaic_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/indic-siyaq-numbers_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/indic-siyaq-numbers_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/inscriptional-pahlavi_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/inscriptional-pahlavi_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/inscriptional-parthian_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/inscriptional-parthian_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/japanese_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/japanese_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/javanese_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/javanese_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/kaithi_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/kaithi_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/kannada_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/kannada_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/kawi_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/kawi_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/kayah-li_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/kayah-li_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/kharoshthi_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/kharoshthi_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/khitan-small-script_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/khitan-small-script_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/khmer_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/khmer_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/khojki_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/khojki_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/khudawadi_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/khudawadi_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/korean_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/korean_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/lao_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/lao_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/latin-ext_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/latin-ext_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/latin_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/latin_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/lepcha_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/lepcha_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/limbu_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/limbu_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/linear-a_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/linear-a_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/linear-b_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/linear-b_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/lisu_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/lisu_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/lycian_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/lycian_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/lydian_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/lydian_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/mahajani_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/mahajani_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/makasar_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/makasar_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/malayalam_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/malayalam_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/mandaic_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/mandaic_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/manichaean_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/manichaean_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/marchen_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/marchen_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/masaram-gondi_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/masaram-gondi_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/math.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/math.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/math_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/math_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/mayan-numerals_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/mayan-numerals_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/medefaidrin_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/medefaidrin_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/meetei-mayek_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/meetei-mayek_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/mende-kikakui_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/mende-kikakui_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/meroitic-cursive_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/meroitic-cursive_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/meroitic-hieroglyphs_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/meroitic-hieroglyphs_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/meroitic_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/meroitic_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/miao_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/miao_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/modi_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/modi_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/mongolian_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/mongolian_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/mro_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/mro_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/multani_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/multani_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/music_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/music_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/myanmar_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/myanmar_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/nabataean_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/nabataean_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/nag-mundari_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/nag-mundari_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/nandinagari_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/nandinagari_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/new-tai-lue_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/new-tai-lue_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/newa_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/newa_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/nko_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/nko_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/nushu_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/nushu_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/nyiakeng-puachue-hmong_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/nyiakeng-puachue-hmong_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/ogham_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/ogham_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/ol-chiki_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/ol-chiki_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/old-hungarian_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/old-hungarian_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/old-italic_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/old-italic_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/old-north-arabian_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/old-north-arabian_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/old-permic_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/old-permic_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/old-persian_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/old-persian_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/old-sogdian_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/old-sogdian_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/old-south-arabian_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/old-south-arabian_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/old-turkic_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/old-turkic_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/old-uyghur_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/old-uyghur_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/oriya_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/oriya_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/osage_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/osage_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/osmanya_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/osmanya_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/ottoman-siyaq-numbers_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/ottoman-siyaq-numbers_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/pahawh-hmong_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/pahawh-hmong_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/palmyrene_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/palmyrene_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/pau-cin-hau_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/pau-cin-hau_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/phags-pa_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/phags-pa_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/phoenician_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/phoenician_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/psalter-pahlavi_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/psalter-pahlavi_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/rejang_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/rejang_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/runic_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/runic_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/samaritan_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/samaritan_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/saurashtra_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/saurashtra_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/sharada_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/sharada_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/shavian_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/shavian_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/siddham_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/siddham_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/signwriting_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/signwriting_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/sinhala_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/sinhala_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/sogdian_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/sogdian_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/sora-sompeng_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/sora-sompeng_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/soyombo_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/soyombo_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/sundanese_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/sundanese_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/syloti-nagri_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/syloti-nagri_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/symbols_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/symbols_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/syriac_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/syriac_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/tagalog_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/tagalog_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/tagbanwa_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/tagbanwa_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/tai-le_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/tai-le_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/tai-tham_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/tai-tham_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/tai-viet_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/tai-viet_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/takri_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/takri_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/tamil-supplement_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/tamil-supplement_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/tamil_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/tamil_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/tangsa_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/tangsa_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/tangut_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/tangut_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/telugu_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/telugu_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/thaana_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/thaana_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/thai_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/thai_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/tibetan_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/tibetan_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/tifinagh_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/tifinagh_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/tirhuta_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/tirhuta_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/toto_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/toto_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/ugaritic_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/ugaritic_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/vai_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/vai_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/vietnamese_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/vietnamese_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/vithkuqi_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/vithkuqi_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/wancho_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/wancho_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/warang-citi_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/warang-citi_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/wgl-latin.enc` & `glyphsets-0.6.9/Lib/glyphsets/encodings/wgl-latin.enc`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/yezidi_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/yezidi_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/yi_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/yi_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/encodings/zanabazar-square_unique-glyphs.nam` & `glyphsets-0.6.9/Lib/glyphsets/encodings/zanabazar-square_unique-glyphs.nam`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/slices/README.md` & `glyphsets-0.6.9/Lib/glyphsets/slices/README.md`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/slices/hongkong-chinese_default.txt` & `glyphsets-0.6.9/Lib/glyphsets/slices/hongkong-chinese_default.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/slices/japanese_default.txt` & `glyphsets-0.6.9/Lib/glyphsets/slices/japanese_default.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/slices/korean_default.txt` & `glyphsets-0.6.9/Lib/glyphsets/slices/korean_default.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/slices/simplified-chinese_default.txt` & `glyphsets-0.6.9/Lib/glyphsets/slices/simplified-chinese_default.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/slices/traditional-chinese_default.txt` & `glyphsets-0.6.9/Lib/glyphsets/slices/traditional-chinese_default.txt`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/subsets.py` & `glyphsets-0.6.9/Lib/glyphsets/subsets.py`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets/test_strings.json` & `glyphsets-0.6.9/Lib/glyphsets/test_strings.json`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/Lib/glyphsets.egg-info/PKG-INFO` & `glyphsets-0.6.9/Lib/glyphsets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glyphsets
-Version: 0.6.8
+Version: 0.6.9
 Summary: A python API for evaluating coverage of glyph sets in font projects.
 Home-page: https://github.com/googlefonts/glyphsets/
 Author: Dave Crossland, Eli Heuer, Felipe Sanches, Lasse Fister, Marc Foley, Yanone, Roderick Sheeter
 Author-email: dave@lab6.com
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Text Processing :: Fonts
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `glyphsets-0.6.8/Lib/glyphsets.egg-info/SOURCES.txt` & `glyphsets-0.6.9/Lib/glyphsets.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -104,17 +104,17 @@
 Archive/GF Glyph Sets/tutorials/img/ecircumflexacute.jpg
 Archive/GF Glyph Sets/tutorials/img/fix-1.png
 Archive/GF Glyph Sets/tutorials/img/fix-2.png
 Archive/GF Glyph Sets/tutorials/img/fix-3.png
 Archive/GF Glyph Sets/tutorials/img/list-filter-1.png
 Archive/GF Glyph Sets/tutorials/img/list-filter.png
 GF_glyphsets/README.md
-GF_glyphsets/empty_font.glyphs
 GF_glyphsets/update-gs.sh
 GF_glyphsets/Arabic/README.md
+GF_glyphsets/Arabic/definitions/GF_Arabic_Core.stub.nam
 GF_glyphsets/Arabic/glyphs/CustomFilter_GF_Arabic.plist
 GF_glyphsets/Arabic/glyphs/GF_Arabic_Core.glyphs
 GF_glyphsets/Arabic/glyphs/GF_Arabic_Plus.glyphs
 GF_glyphsets/Arabic/nam/GF_Arabic_Core.nam
 GF_glyphsets/Arabic/nam/GF_Arabic_Plus.nam
 GF_glyphsets/Arabic/txt/nice-names/GF_Arabic_Core.txt
 GF_glyphsets/Arabic/txt/nice-names/GF_Arabic_Plus.txt
@@ -175,15 +175,14 @@
 GF_glyphsets/Greek/txt/prod-names/GF_Greek_Core.txt
 GF_glyphsets/Greek/txt/prod-names/GF_Greek_Expert.txt
 GF_glyphsets/Greek/txt/prod-names/GF_Greek_Plus.txt
 GF_glyphsets/Greek/txt/prod-names/GF_Greek_Pro.txt
 GF_glyphsets/Latin/README.md
 GF_glyphsets/Latin/definitions/GF_Latin_Core.stub.glyphs
 GF_glyphsets/Latin/definitions/GF_Latin_Core.stub.nam
-GF_glyphsets/Latin/definitions/GF_Latin_Kernel.stub.nam
 GF_glyphsets/Latin/glyphs/CustomFilter_GF_Latin.plist
 GF_glyphsets/Latin/glyphs/GF_Latin_African.glyphs
 GF_glyphsets/Latin/glyphs/GF_Latin_Beyond.glyphs
 GF_glyphsets/Latin/glyphs/GF_Latin_Core.glyphs
 GF_glyphsets/Latin/glyphs/GF_Latin_Kernel.glyphs
 GF_glyphsets/Latin/glyphs/GF_Latin_Plus.glyphs
 GF_glyphsets/Latin/glyphs/GF_Latin_Vietnamese.glyphs
@@ -252,16 +251,17 @@
 Lib/glyphsets.egg-info/SOURCES.txt
 Lib/glyphsets.egg-info/dependency_links.txt
 Lib/glyphsets.egg-info/entry_points.txt
 Lib/glyphsets.egg-info/not-zip-safe
 Lib/glyphsets.egg-info/requires.txt
 Lib/glyphsets.egg-info/top_level.txt
 Lib/glyphsets/definitions/__init__.py
+Lib/glyphsets/definitions/nam/GF_Arabic_Core.nam
+Lib/glyphsets/definitions/nam/GF_Arabic_Plus.nam
 Lib/glyphsets/definitions/nam/GF_Latin_Core.nam
-Lib/glyphsets/definitions/nam/GF_Latin_Kernel.nam
 Lib/glyphsets/encodings/README.md
 Lib/glyphsets/encodings/adlam_unique-glyphs.nam
 Lib/glyphsets/encodings/ahom_unique-glyphs.nam
 Lib/glyphsets/encodings/anatolian-hieroglyphs_unique-glyphs.nam
 Lib/glyphsets/encodings/arabic_unique-glyphs.nam
 Lib/glyphsets/encodings/armenian_unique-glyphs.nam
 Lib/glyphsets/encodings/avestan_unique-glyphs.nam
```

### Comparing `glyphsets-0.6.8/PKG-INFO` & `glyphsets-0.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glyphsets
-Version: 0.6.8
+Version: 0.6.9
 Summary: A python API for evaluating coverage of glyph sets in font projects.
 Home-page: https://github.com/googlefonts/glyphsets/
 Author: Dave Crossland, Eli Heuer, Felipe Sanches, Lasse Fister, Marc Foley, Yanone, Roderick Sheeter
 Author-email: dave@lab6.com
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Text Processing :: Fonts
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `glyphsets-0.6.8/README.md` & `glyphsets-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/scripts/assemble_charactersets.py` & `glyphsets-0.6.9/scripts/assemble_charactersets.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,14 @@
             f"{glyphset_name}.nam",
         )
     )
     glyphs_stub_path = os.path.join(
         root_folder, script, "definitions", f"{glyphset_name}.stub.glyphs"
     )
     glyphs_path = os.path.join(root_folder, script, "glyphs", f"{glyphset_name}.glyphs")
-    glyphs_empty_path = os.path.join(root_folder, f"empty_font.glyphs")
     txt_nicenames_path = os.path.join(
         root_folder, script, "txt", "nice-names", f"{glyphset_name}.txt"
     )
     txt_prodnames_path = os.path.join(
         root_folder, script, "txt", "prod-names", f"{glyphset_name}.txt"
     )
     plist_path = os.path.join(
@@ -116,15 +115,15 @@
 
     assert type(GLYPHDATA) is glyphsLib.glyphdata.GlyphData
 
     # Create glyphs file and add characters
     if os.path.exists(glyphs_stub_path):
         font = glyphsLib.load(glyphs_stub_path)
     else:
-        font = glyphsLib.load(glyphs_empty_path)
+        font = glyphsLib.GSFont()
         font.familyName = glyphset_name
     for _i, unicode in enumerate(sorted(list(character_set))):
         unicode = f"{unicode:#0{6}X}".replace("0X", "")
         glyph_info = _lookup_attributes_by_unicode(unicode, GLYPHDATA)
         glyph = glyphsLib.GSGlyph(glyph_info["name"])
         glyph.unicode = unicode
         font.glyphs.append(glyph)
@@ -134,14 +133,18 @@
     unicode_sorted_glyphs = sorted(font.glyphs, key=functools.cmp_to_key(sort_unicodes))
     glyph_names = [glyph.name for glyph in unicode_sorted_glyphs]
     production_glyph_names = [
         get_glyph(glyph.name).production_name for glyph in unicode_sorted_glyphs
     ]
 
     # Save glyphs file
+    font.axes = []
+    for master in font.masters:
+        master.axes = []
+    font.instances = []
     font.save(glyphs_path)
 
     # Output sorted character set to .nam file
     with open(nam_path, "w") as f:
         f.write(
             "# This file is auto-generated; do not edit. See /README.md for instructions.\n"
         )
```

### Comparing `glyphsets-0.6.8/scripts/assemble_languages.py` & `glyphsets-0.6.9/scripts/assemble_languages.py`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/scripts/create-glyphset.py` & `glyphsets-0.6.9/scripts/create-glyphset.py`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/scripts/find_language_for_character.py` & `glyphsets-0.6.9/scripts/find_language_for_character.py`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/setup.py` & `glyphsets-0.6.9/setup.py`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/tests/__init__.py` & `glyphsets-0.6.9/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/tests/data/MavenPro[wght].ttf` & `glyphsets-0.6.9/tests/data/MavenPro[wght].ttf`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/tests/test_glyphdata.py` & `glyphsets-0.6.9/tests/test_glyphdata.py`

 * *Files identical despite different names*

### Comparing `glyphsets-0.6.8/tests/testcoverage.py` & `glyphsets-0.6.9/tests/testcoverage.py`

 * *Files identical despite different names*

