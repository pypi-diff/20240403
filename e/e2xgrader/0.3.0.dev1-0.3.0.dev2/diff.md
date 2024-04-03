# Comparing `tmp/e2xgrader-0.3.0.dev1.tar.gz` & `tmp/e2xgrader-0.3.0.dev2.tar.gz`

## Comparing `e2xgrader-0.3.0.dev1.tar` & `e2xgrader-0.3.0.dev2.tar`

### file list

```diff
@@ -1,339 +1,339 @@
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/.babelrc
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/.coveragerc
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/.readthedocs.yaml
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/MANIFEST.in
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/lerna.json
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/nbgrader_config.py
--rw-r--r--   0        0        0   964703 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/package-lock.json
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/package.json
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/sonar-project.properties
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/.github/workflows/black.yml
--rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/.github/workflows/dispatch.yml
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/.github/workflows/python-package.yml
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/.github/workflows/ruff.yml
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/.github/workflows/sonar-scan.yml
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/.gitignore
--rw-r--r--   0        0        0    21865 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/coverage_html.js
--rw-r--r--   0        0        0    18396 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_0a574a50e34851d4___init___py.html
--rw-r--r--   0        0        0     7936 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_0ff1fe3f8b795b70___init___py.html
--rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_0ff1fe3f8b795b70_activatemodeapp_py.html
--rw-r--r--   0        0        0    13279 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_0ff1fe3f8b795b70_baseapp_py.html
--rw-r--r--   0        0        0     8241 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_0ff1fe3f8b795b70_deactivatemodeapp_py.html
--rw-r--r--   0        0        0    15010 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_0ff1fe3f8b795b70_e2xgraderapp_py.html
--rw-r--r--   0        0        0     6682 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_0ff1fe3f8b795b70_showmodeapp_py.html
--rw-r--r--   0        0        0    20948 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_0ff1fe3f8b795b70_togglemodeapp_py.html
--rw-r--r--   0        0        0     5286 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_2448a76917b6613d___init___py.html
--rw-r--r--   0        0        0     8558 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_2448a76917b6613d_assignmentlist_py.html
--rw-r--r--   0        0        0    36265 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_2448a76917b6613d_handlers_py.html
--rw-r--r--   0        0        0     6152 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_294994a5caef5622___init___py.html
--rw-r--r--   0        0        0    10207 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_294994a5caef5622_student_py.html
--rw-r--r--   0        0        0    11420 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_2d23d5c010468094___init___py.html
--rw-r--r--   0        0        0    10074 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_2d23d5c010468094_clearhiddentests_py.html
--rw-r--r--   0        0        0    11422 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_2d23d5c010468094_clearsolutions_py.html
--rw-r--r--   0        0        0    35385 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_2d23d5c010468094_extractattachments_py.html
--rw-r--r--   0        0        0    10587 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_2d23d5c010468094_filtercellsbyid_py.html
--rw-r--r--   0        0        0    11853 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_2d23d5c010468094_filtertests_py.html
--rw-r--r--   0        0        0    14907 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_2d23d5c010468094_overwritecells_py.html
--rw-r--r--   0        0        0    19006 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_2d23d5c010468094_permutetasks_py.html
--rw-r--r--   0        0        0    38276 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_2d23d5c010468094_saveautogrades_py.html
--rw-r--r--   0        0        0    15444 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_2d23d5c010468094_savecells_py.html
--rw-r--r--   0        0        0    80079 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_2d23d5c010468094_scramble_py.html
--rw-r--r--   0        0        0    18451 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_2d23d5c010468094_unpermutetasks_py.html
--rw-r--r--   0        0        0    12358 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_2d23d5c010468094_unscramble_py.html
--rw-r--r--   0        0        0    15721 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_2d23d5c010468094_validateextracells_py.html
--rw-r--r--   0        0        0     6257 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_37d73105d5cffd7e___init___py.html
--rw-r--r--   0        0        0    10842 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_37d73105d5cffd7e_base_py.html
--rw-r--r--   0        0        0    21835 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_37d73105d5cffd7e_code_py.html
--rw-r--r--   0        0        0    13300 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_37d73105d5cffd7e_multiplechoice_py.html
--rw-r--r--   0        0        0    11679 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_37d73105d5cffd7e_singlechoice_py.html
--rw-r--r--   0        0        0     4512 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_5beb92c0ecba1ed4___init___py.html
--rw-r--r--   0        0        0     4530 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_5ef362e6f46f83e2___init___py.html
--rw-r--r--   0        0        0     5540 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_710bf0b8e9508f41___init___py.html
--rw-r--r--   0        0        0    11645 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_710bf0b8e9508f41_highlight_py.html
--rw-r--r--   0        0        0     4514 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_7805cff25cc2d712___init___py.html
--rw-r--r--   0        0        0    22670 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_7805cff25cc2d712_extra_cells_py.html
--rw-r--r--   0        0        0    40157 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_7805cff25cc2d712_mode_py.html
--rw-r--r--   0        0        0     5536 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_78932b1391e2ad05___init___py.html
--rw-r--r--   0        0        0    20256 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_78932b1391e2ad05_nbgraderapi_py.html
--rw-r--r--   0        0        0     4550 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_83df762bc77ead36___init___py.html
--rw-r--r--   0        0        0     6158 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_866c9e7ae337468e___init___py.html
--rw-r--r--   0        0        0    13167 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_866c9e7ae337468e_teacher_py.html
--rw-r--r--   0        0        0     4524 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_8fe6e31f42e6838f___init___py.html
--rw-r--r--   0        0        0     5228 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_94f16e40fada4634___init___py.html
--rw-r--r--   0        0        0    21878 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_94f16e40fada4634_apihandlers_py.html
--rw-r--r--   0        0        0    18164 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_94f16e40fada4634_help_py.html
--rw-r--r--   0        0        0     5233 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_98391cc2871b8725___init___py.html
--rw-r--r--   0        0        0    10298 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_98391cc2871b8725_base_py.html
--rw-r--r--   0        0        0    14037 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_98391cc2871b8725_manager_py.html
--rw-r--r--   0        0        0    30248 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_98391cc2871b8725_nbextensions_py.html
--rw-r--r--   0        0        0    21891 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_98391cc2871b8725_serverextensions_py.html
--rw-r--r--   0        0        0    21214 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_98391cc2871b8725_utils_py.html
--rw-r--r--   0        0        0     5559 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_9b0ce7ff0ae20648___init___py.html
--rw-r--r--   0        0        0    51443 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_9b0ce7ff0ae20648_apihandlers_py.html
--rw-r--r--   0        0        0    10048 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_9b0ce7ff0ae20648_e2xgraderapi_py.html
--rw-r--r--   0        0        0     4530 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_c74475b6151f7a7b___init___py.html
--rw-r--r--   0        0        0    50468 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_c74475b6151f7a7b_cells_py.html
--rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_d878b7d22c4c16e4___init___py.html
--rw-r--r--   0        0        0    19960 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_d878b7d22c4c16e4_diagrameditor_py.html
--rw-r--r--   0        0        0     4558 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_dbfe9cfbceae7526___init___py.html
--rw-r--r--   0        0        0     6173 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_e43806ab68cc7f97___init___py.html
--rw-r--r--   0        0        0     7158 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_e43806ab68cc7f97_student_exam_py.html
--rw-r--r--   0        0        0     5925 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_e533b0b56079eb7c___init___py.html
--rw-r--r--   0        0        0    46599 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_e533b0b56079eb7c_exporter_py.html
--rw-r--r--   0        0        0    46736 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_e533b0b56079eb7c_gradeexporter_py.html
--rw-r--r--   0        0        0    21518 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_e533b0b56079eb7c_submissionexporter_py.html
--rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_e7343efe92bf6800___init___py.html
--rw-r--r--   0        0        0    20756 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_e7343efe92bf6800_formgrader_py.html
--rw-r--r--   0        0        0    79326 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_e7343efe92bf6800_handlers_py.html
--rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_f7a0650fde384913___init___py.html
--rw-r--r--   0        0        0     9032 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_fddc8d031c76e3e4___init___py.html
--rw-r--r--   0        0        0    40230 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_fddc8d031c76e3e4_collect_py.html
--rw-r--r--   0        0        0    20286 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_fddc8d031c76e3e4_exchange_py.html
--rw-r--r--   0        0        0    32227 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_fddc8d031c76e3e4_fetch_assignment_py.html
--rw-r--r--   0        0        0    49728 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_fddc8d031c76e3e4_fetch_feedback_py.html
--rw-r--r--   0        0        0    40050 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_fddc8d031c76e3e4_hash_utils_py.html
--rw-r--r--   0        0        0    88239 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_fddc8d031c76e3e4_list_py.html
--rw-r--r--   0        0        0    49978 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_fddc8d031c76e3e4_release_assignment_py.html
--rw-r--r--   0        0        0    51098 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_fddc8d031c76e3e4_release_feedback_py.html
--rw-r--r--   0        0        0    85210 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_fddc8d031c76e3e4_submit_py.html
--rw-r--r--   0        0        0    17748 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_fddc8d031c76e3e4_utils_py.html
--rw-r--r--   0        0        0     5300 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_ff9ed41ff67ae67c___init___py.html
--rw-r--r--   0        0        0    27556 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_ff9ed41ff67ae67c_handlers_py.html
--rw-r--r--   0        0        0     6850 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_ff9ed41ff67ae67c_validateassignment_py.html
--rw-r--r--   0        0        0    21812 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_ff9ed41ff67ae67c_validator_py.html
--rw-r--r--   0        0        0     5239 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_ffb521de3e56ad10___init___py.html
--rw-r--r--   0        0        0    17468 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_ffb521de3e56ad10_extension_py.html
--rw-r--r--   0        0        0     4542 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/d_ffe7516a0565d1ec___init___py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/favicon_32.png
--rw-r--r--   0        0        0    33168 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/keybd_open.png
--rw-r--r--   0        0        0    21422 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/status.json
--rw-r--r--   0        0        0    12406 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/coverage_report/style.css
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/docs/make.bat
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/docs/requirements.txt
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/docs/source/conf.py
--rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/docs/source/index.rst
--rw-r--r--   0        0        0    10337 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/docs/source/extensions/apps.rst
--rw-r--r--   0        0        0     3471 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/docs/source/extensions/autograders.rst
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/docs/source/extensions/index.rst
--rw-r--r--   0        0        0    37523 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/docs/source/extensions/img/convert_grades.png
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/docs/source/getting_started/configuration.rst
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/docs/source/getting_started/index.rst
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/docs/source/getting_started/installation.rst
--rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/docs/source/getting_started/modes.rst
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/docs/source/user_docs/authoring.rst
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/docs/source/user_docs/grade_export.rst
--rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/docs/source/user_docs/grading.rst
--rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/docs/source/user_docs/help_extension.rst
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/docs/source/user_docs/index.rst
--rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/docs/source/user_docs/modes.rst
--rw-r--r--   0        0        0     4946 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/docs/source/user_docs/cells/cells.rst
--rw-r--r--   0        0        0    30552 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/docs/source/user_docs/cells/img/attachment_editor.png
--rw-r--r--   0        0        0    80690 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/docs/source/user_docs/cells/img/diagram_editor.png
--rw-r--r--   0        0        0    17552 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/docs/source/user_docs/cells/img/diagram_empty.png
--rw-r--r--   0        0        0    21305 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/docs/source/user_docs/cells/img/diagram_filled.png
--rw-r--r--   0        0        0    16291 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/docs/source/user_docs/cells/img/mc_edit.png
--rw-r--r--   0        0        0    17990 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/docs/source/user_docs/cells/img/mc_render.png
--rw-r--r--   0        0        0    12007 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/docs/source/user_docs/cells/img/sc_edit.png
--rw-r--r--   0        0        0    14139 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/docs/source/user_docs/cells/img/sc_render.png
--rw-r--r--   0        0        0    23745 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/docs/source/user_docs/cells/img/upload_question_rendered.png
--rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/docs/source/user_docs/exchange/base_exchange.rst
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/docs/source/user_docs/exchange/index.rst
--rw-r--r--   0        0        0     3075 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/docs/source/user_docs/exchange/submit.rst
--rw-r--r--   0        0        0    50924 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/docs/source/user_docs/exchange/img/submitted_html.png
--rw-r--r--   0        0        0    46425 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/docs/source/user_docs/exchange/img/submitted_html_de.png
--rw-r--r--   0        0        0    75660 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/docs/source/user_docs/img/annotate_answer.png
--rw-r--r--   0        0        0    36170 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/docs/source/user_docs/img/assignment_toolbar_code.png
--rw-r--r--   0        0        0    34390 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/docs/source/user_docs/img/assignment_toolbar_md.png
--rw-r--r--   0        0        0    12214 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/docs/source/user_docs/img/cell_type_change_alert.png
--rw-r--r--   0        0        0    36165 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/docs/source/user_docs/img/exam_toolbar.png
--rw-r--r--   0        0        0    77628 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/docs/source/user_docs/img/export_grades_dialog.png
--rw-r--r--   0        0        0     7735 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/docs/source/user_docs/img/exported_grades.png
--rw-r--r--   0        0        0     8706 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/docs/source/user_docs/img/exported_grades_max_score.png
--rw-r--r--   0        0        0     7862 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/docs/source/user_docs/img/exported_grades_normalized.png
--rw-r--r--   0        0        0    19045 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/docs/source/user_docs/img/help_tab.png
--rw-r--r--   0        0        0    12085 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/docs/source/user_docs/img/move_cell_alert.png
--rw-r--r--   0        0        0    45645 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/docs/source/user_docs/img/submit.png
--rw-r--r--   0        0        0    79144 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/docs/source/user_docs/img/task_view.png
--rw-r--r--   0        0        0    82489 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/docs/source/user_docs/img/task_view_task.png
--rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/__init__.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/__main__.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/__version__.py
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/apps/__init__.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/apps/activatemodeapp.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/apps/baseapp.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/apps/deactivatemodeapp.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/apps/e2xgraderapp.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/apps/showmodeapp.py
--rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/apps/togglemodeapp.py
--rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/config/__init__.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/exchange/__init__.py
--rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/exchange/collect.py
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/exchange/exchange.py
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/exchange/fetch_assignment.py
--rw-r--r--   0        0        0     6604 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/exchange/fetch_feedback.py
--rw-r--r--   0        0        0     4795 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/exchange/hash_utils.py
--rw-r--r--   0        0        0    11216 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/exchange/list.py
--rw-r--r--   0        0        0     5819 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/exchange/release_assignment.py
--rw-r--r--   0        0        0     5879 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/exchange/release_feedback.py
--rw-r--r--   0        0        0     9801 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/exchange/submit.py
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/exchange/utils.py
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/exporters/__init__.py
--rw-r--r--   0        0        0     4811 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/exporters/exporter.py
--rw-r--r--   0        0        0     5052 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/exporters/gradeexporter.py
--rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/exporters/submissionexporter.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/exporters/filters/__init__.py
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/exporters/filters/highlight.py
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/exporters/templates/hashcode_cell.html
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/extensions/__init__.py
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/extensions/base.py
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/extensions/manager.py
--rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/extensions/nbextensions.py
--rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/extensions/serverextensions.py
--rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/extensions/utils.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/graders/__init__.py
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/graders/base.py
--rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/graders/code.py
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/graders/multiplechoice.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/graders/singlechoice.py
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/preprocessors/__init__.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/preprocessors/clearhiddentests.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/preprocessors/clearsolutions.py
--rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/preprocessors/extractattachments.py
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/preprocessors/filtercellsbyid.py
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/preprocessors/filtertests.py
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/preprocessors/overwritecells.py
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/preprocessors/permutetasks.py
--rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/preprocessors/saveautogrades.py
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/preprocessors/savecells.py
--rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/preprocessors/scramble.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/preprocessors/unpermutetasks.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/preprocessors/unscramble.py
--rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/preprocessors/validateextracells.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/__init__.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/assignment_list/__init__.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/assignment_list/assignmentlist.py
--rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/assignment_list/handlers.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/diagram_editor/__init__.py
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/diagram_editor/diagrameditor.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/e2xgraderapi/__init__.py
--rw-r--r--   0        0        0     5382 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/e2xgraderapi/apihandlers.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/e2xgraderapi/e2xgraderapi.py
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/e2xgraderapi/presets/questions/Code (Autograded).ipynb
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/e2xgraderapi/presets/questions/Code (Manual).ipynb
--rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/e2xgraderapi/presets/questions/Diagram.ipynb
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/e2xgraderapi/presets/questions/Freetext.ipynb
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/e2xgraderapi/presets/questions/Multiple Choice.ipynb
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/e2xgraderapi/presets/questions/Single Choice.ipynb
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/e2xgraderapi/presets/questions/Upload Files.ipynb
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/e2xgraderapi/presets/template/Footer.ipynb
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/e2xgraderapi/presets/template/Group Info.ipynb
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/e2xgraderapi/presets/template/Header.ipynb
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/e2xgraderapi/presets/template/Student Info.ipynb
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/e2xgraderapi/templates/feedback/conf.json
--rw-r--r--   0        0        0     8033 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/e2xgraderapi/templates/feedback/index.html.j2
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/e2xgraderapi/templates/form/conf.json
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/e2xgraderapi/templates/form/index.html.j2
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/formgrader/__init__.py
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/formgrader/formgrader.py
--rw-r--r--   0        0        0     9023 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/formgrader/handlers.py
--rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/formgrader/static/css/eraser-solid.svg
--rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/formgrader/static/css/pencil-solid.svg
--rw-r--r--   0        0        0    10212 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/formgrader/static/js/formgrade.js
--rw-r--r--   0        0        0    10309 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/formgrader/static/js/formgrade_models.js
--rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/formgrader/static/js/gradebook_assignments.js
--rw-r--r--   0        0        0     7144 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/formgrader/static/js/gradebook_notebook_submissions.js
--rw-r--r--   0        0        0     4460 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/formgrader/static/js/gradebook_notebooks.js
--rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/formgrader/static/js/gradebook_tasks.js
--rw-r--r--   0        0        0    20909 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/formgrader/static/js/manage_assignments.js
--rw-r--r--   0        0        0    11457 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/formgrader/static/js/manage_submissions.js
--rw-r--r--   0        0        0     6587 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/formgrader/templates/base.tpl
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/formgrader/templates/export_grades.tpl
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/formgrader/templates/gradebook_base.tpl
--rw-r--r--   0        0        0     4476 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/formgrader/templates/manage_assignments.tpl
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/formgrader/templates/manage_students_base.tpl
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/formgrader/templates/manage_submissions.tpl
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/formgrader/templates/formgrade/conf.json
--rw-r--r--   0        0        0     5542 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/formgrader/templates/formgrade/formgrade_macros.html.j2
--rw-r--r--   0        0        0    12093 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/formgrader/templates/formgrade/index.html.j2
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/formgrader/templates/task_view/gradebook_assignments.tpl
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/formgrader/templates/task_view/gradebook_base.tpl
--rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/formgrader/templates/task_view/gradebook_notebook_submissions.tpl
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/formgrader/templates/task_view/gradebook_notebooks.tpl
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/formgrader/templates/task_view/gradebook_tasks.tpl
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/help/__init__.py
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/help/apihandlers.py
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/help/help.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/nbgraderapi/__init__.py
--rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/nbgraderapi/nbgraderapi.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/validate_assignment/__init__.py
--rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/validate_assignment/handlers.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/validate_assignment/validateassignment.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/validate_assignment/validator.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/base/__init__.py
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/base/extension.py
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/student/__init__.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/student/student.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/student_exam/__init__.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/student_exam/student_exam.py
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/teacher/__init__.py
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/teacher/teacher.py
--rw-r--r--   0        0        0   136740 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/static/nbextensions/notebook/student/main.js
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/static/nbextensions/notebook/student/main.js.LICENSE.txt
--rw-r--r--   0        0        0   167170 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/static/nbextensions/notebook/student_exam/main.js
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/static/nbextensions/notebook/student_exam/main.js.LICENSE.txt
--rw-r--r--   0        0        0   168862 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/static/nbextensions/notebook/teacher/main.js
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/static/nbextensions/notebook/teacher/main.js.LICENSE.txt
--rw-r--r--   0        0        0     3675 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/static/nbextensions/tree/student/main.js
--rw-r--r--   0        0        0    13207 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/static/nbextensions/tree/student_exam/main.js
--rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/static/nbextensions/tree/teacher/main.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/tests/apps/__init__.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/tests/apps/test_activatemodeapp.py
--rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/tests/apps/test_baseapp.py
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/tests/apps/test_deactivatemodeapp.py
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/tests/apps/test_e2xgraderapp.py
--rw-r--r--   0        0        0     6964 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/tests/apps/test_e2xmanager.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/tests/apps/test_showmodeapp.py
--rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/tests/apps/test_togglemodeapp.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/tests/exchange/__init__.py
--rw-r--r--   0        0        0     5363 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/tests/exchange/test_hash_utils.py
--rw-r--r--   0        0        0    13121 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/tests/exchange/test_submit.py
--rw-r--r--   0        0        0     3041 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/tests/exchange/test_utils.py
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/tests/exchange/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/tests/exporters/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/tests/exporters/filters/__init__.py
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/tests/exporters/filters/test_highlight.py
--rw-r--r--   0        0        0     4251 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/tests/extensions/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/tests/graders/__init__.py
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/tests/graders/test_base.py
--rw-r--r--   0        0        0     3159 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/tests/graders/test_code.py
--rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/tests/graders/test_multiplechoice.py
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/tests/graders/test_singlechoice.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/tests/preprocessors/__init__.py
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/tests/preprocessors/test_clearhiddentests.py
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/tests/preprocessors/test_clearsolutions.py
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/tests/preprocessors/test_extractattachments.py
--rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/tests/preprocessors/test_filtercellsbyid.py
--rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/tests/preprocessors/test_filtertests.py
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/tests/preprocessors/test_unscramble.py
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/tests/preprocessors/test_validateextracells.py
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/tests/server_extensions/apps/diagram_editor/test_diagrameditor.py
--rw-r--r--   0        0        0     3267 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/tests/server_extensions/apps/validate_assignment/test_validator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/tests/test_utils/__init__.py
--rw-r--r--   0        0        0     4757 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/tests/test_utils/cells.py
--rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/tests/test_utils/test_utils.py
--rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/tests/utils/test_mode.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/utils/__init__.py
--rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/utils/extra_cells.py
--rw-r--r--   0        0        0     4591 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/utils/mode.py
--rw-r--r--   0        0        0     3295 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/e2xgrader/utils/nbgrader_cells.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/etc/jupyter/jupyter_server_config.d/e2xgrader.json
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/LICENSE
--rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/README.md
--rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/pyproject.toml
--rw-r--r--   0        0        0     3795 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev1/PKG-INFO
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/.babelrc
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/.coveragerc
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/.readthedocs.yaml
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/MANIFEST.in
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/lerna.json
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/nbgrader_config.py
+-rw-r--r--   0        0        0   964703 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/package-lock.json
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/package.json
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/sonar-project.properties
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/.github/workflows/black.yml
+-rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/.github/workflows/dispatch.yml
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/.github/workflows/ruff.yml
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/.github/workflows/sonar-scan.yml
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/.gitignore
+-rw-r--r--   0        0        0    21865 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/coverage_html.js
+-rw-r--r--   0        0        0    18396 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_0a574a50e34851d4___init___py.html
+-rw-r--r--   0        0        0     7936 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_0ff1fe3f8b795b70___init___py.html
+-rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_0ff1fe3f8b795b70_activatemodeapp_py.html
+-rw-r--r--   0        0        0    13279 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_0ff1fe3f8b795b70_baseapp_py.html
+-rw-r--r--   0        0        0     8241 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_0ff1fe3f8b795b70_deactivatemodeapp_py.html
+-rw-r--r--   0        0        0    15010 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_0ff1fe3f8b795b70_e2xgraderapp_py.html
+-rw-r--r--   0        0        0     6682 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_0ff1fe3f8b795b70_showmodeapp_py.html
+-rw-r--r--   0        0        0    20948 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_0ff1fe3f8b795b70_togglemodeapp_py.html
+-rw-r--r--   0        0        0     5286 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_2448a76917b6613d___init___py.html
+-rw-r--r--   0        0        0     8558 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_2448a76917b6613d_assignmentlist_py.html
+-rw-r--r--   0        0        0    36265 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_2448a76917b6613d_handlers_py.html
+-rw-r--r--   0        0        0     6152 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_294994a5caef5622___init___py.html
+-rw-r--r--   0        0        0    10207 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_294994a5caef5622_student_py.html
+-rw-r--r--   0        0        0    11420 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_2d23d5c010468094___init___py.html
+-rw-r--r--   0        0        0    10074 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_2d23d5c010468094_clearhiddentests_py.html
+-rw-r--r--   0        0        0    11422 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_2d23d5c010468094_clearsolutions_py.html
+-rw-r--r--   0        0        0    35385 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_2d23d5c010468094_extractattachments_py.html
+-rw-r--r--   0        0        0    10587 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_2d23d5c010468094_filtercellsbyid_py.html
+-rw-r--r--   0        0        0    11853 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_2d23d5c010468094_filtertests_py.html
+-rw-r--r--   0        0        0    14907 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_2d23d5c010468094_overwritecells_py.html
+-rw-r--r--   0        0        0    19006 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_2d23d5c010468094_permutetasks_py.html
+-rw-r--r--   0        0        0    38276 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_2d23d5c010468094_saveautogrades_py.html
+-rw-r--r--   0        0        0    15444 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_2d23d5c010468094_savecells_py.html
+-rw-r--r--   0        0        0    80079 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_2d23d5c010468094_scramble_py.html
+-rw-r--r--   0        0        0    18451 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_2d23d5c010468094_unpermutetasks_py.html
+-rw-r--r--   0        0        0    12358 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_2d23d5c010468094_unscramble_py.html
+-rw-r--r--   0        0        0    15721 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_2d23d5c010468094_validateextracells_py.html
+-rw-r--r--   0        0        0     6257 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_37d73105d5cffd7e___init___py.html
+-rw-r--r--   0        0        0    10842 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_37d73105d5cffd7e_base_py.html
+-rw-r--r--   0        0        0    21835 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_37d73105d5cffd7e_code_py.html
+-rw-r--r--   0        0        0    13300 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_37d73105d5cffd7e_multiplechoice_py.html
+-rw-r--r--   0        0        0    11679 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_37d73105d5cffd7e_singlechoice_py.html
+-rw-r--r--   0        0        0     4512 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_5beb92c0ecba1ed4___init___py.html
+-rw-r--r--   0        0        0     4530 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_5ef362e6f46f83e2___init___py.html
+-rw-r--r--   0        0        0     5540 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_710bf0b8e9508f41___init___py.html
+-rw-r--r--   0        0        0    11645 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_710bf0b8e9508f41_highlight_py.html
+-rw-r--r--   0        0        0     4514 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_7805cff25cc2d712___init___py.html
+-rw-r--r--   0        0        0    22670 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_7805cff25cc2d712_extra_cells_py.html
+-rw-r--r--   0        0        0    40157 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_7805cff25cc2d712_mode_py.html
+-rw-r--r--   0        0        0     5536 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_78932b1391e2ad05___init___py.html
+-rw-r--r--   0        0        0    20256 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_78932b1391e2ad05_nbgraderapi_py.html
+-rw-r--r--   0        0        0     4550 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_83df762bc77ead36___init___py.html
+-rw-r--r--   0        0        0     6158 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_866c9e7ae337468e___init___py.html
+-rw-r--r--   0        0        0    13167 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_866c9e7ae337468e_teacher_py.html
+-rw-r--r--   0        0        0     4524 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_8fe6e31f42e6838f___init___py.html
+-rw-r--r--   0        0        0     5228 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_94f16e40fada4634___init___py.html
+-rw-r--r--   0        0        0    21878 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_94f16e40fada4634_apihandlers_py.html
+-rw-r--r--   0        0        0    18164 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_94f16e40fada4634_help_py.html
+-rw-r--r--   0        0        0     5233 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_98391cc2871b8725___init___py.html
+-rw-r--r--   0        0        0    10298 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_98391cc2871b8725_base_py.html
+-rw-r--r--   0        0        0    14037 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_98391cc2871b8725_manager_py.html
+-rw-r--r--   0        0        0    30248 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_98391cc2871b8725_nbextensions_py.html
+-rw-r--r--   0        0        0    21891 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_98391cc2871b8725_serverextensions_py.html
+-rw-r--r--   0        0        0    21214 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_98391cc2871b8725_utils_py.html
+-rw-r--r--   0        0        0     5559 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_9b0ce7ff0ae20648___init___py.html
+-rw-r--r--   0        0        0    51443 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_9b0ce7ff0ae20648_apihandlers_py.html
+-rw-r--r--   0        0        0    10048 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_9b0ce7ff0ae20648_e2xgraderapi_py.html
+-rw-r--r--   0        0        0     4530 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_c74475b6151f7a7b___init___py.html
+-rw-r--r--   0        0        0    50468 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_c74475b6151f7a7b_cells_py.html
+-rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_d878b7d22c4c16e4___init___py.html
+-rw-r--r--   0        0        0    19960 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_d878b7d22c4c16e4_diagrameditor_py.html
+-rw-r--r--   0        0        0     4558 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_dbfe9cfbceae7526___init___py.html
+-rw-r--r--   0        0        0     6173 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_e43806ab68cc7f97___init___py.html
+-rw-r--r--   0        0        0     7158 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_e43806ab68cc7f97_student_exam_py.html
+-rw-r--r--   0        0        0     5925 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_e533b0b56079eb7c___init___py.html
+-rw-r--r--   0        0        0    46599 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_e533b0b56079eb7c_exporter_py.html
+-rw-r--r--   0        0        0    46736 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_e533b0b56079eb7c_gradeexporter_py.html
+-rw-r--r--   0        0        0    21518 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_e533b0b56079eb7c_submissionexporter_py.html
+-rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_e7343efe92bf6800___init___py.html
+-rw-r--r--   0        0        0    20756 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_e7343efe92bf6800_formgrader_py.html
+-rw-r--r--   0        0        0    79326 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_e7343efe92bf6800_handlers_py.html
+-rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_f7a0650fde384913___init___py.html
+-rw-r--r--   0        0        0     9032 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_fddc8d031c76e3e4___init___py.html
+-rw-r--r--   0        0        0    40230 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_fddc8d031c76e3e4_collect_py.html
+-rw-r--r--   0        0        0    20286 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_fddc8d031c76e3e4_exchange_py.html
+-rw-r--r--   0        0        0    32227 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_fddc8d031c76e3e4_fetch_assignment_py.html
+-rw-r--r--   0        0        0    49728 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_fddc8d031c76e3e4_fetch_feedback_py.html
+-rw-r--r--   0        0        0    40050 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_fddc8d031c76e3e4_hash_utils_py.html
+-rw-r--r--   0        0        0    88239 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_fddc8d031c76e3e4_list_py.html
+-rw-r--r--   0        0        0    49978 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_fddc8d031c76e3e4_release_assignment_py.html
+-rw-r--r--   0        0        0    51098 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_fddc8d031c76e3e4_release_feedback_py.html
+-rw-r--r--   0        0        0    85210 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_fddc8d031c76e3e4_submit_py.html
+-rw-r--r--   0        0        0    17748 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_fddc8d031c76e3e4_utils_py.html
+-rw-r--r--   0        0        0     5300 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_ff9ed41ff67ae67c___init___py.html
+-rw-r--r--   0        0        0    27556 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_ff9ed41ff67ae67c_handlers_py.html
+-rw-r--r--   0        0        0     6850 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_ff9ed41ff67ae67c_validateassignment_py.html
+-rw-r--r--   0        0        0    21812 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_ff9ed41ff67ae67c_validator_py.html
+-rw-r--r--   0        0        0     5239 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_ffb521de3e56ad10___init___py.html
+-rw-r--r--   0        0        0    17468 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_ffb521de3e56ad10_extension_py.html
+-rw-r--r--   0        0        0     4542 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/d_ffe7516a0565d1ec___init___py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/favicon_32.png
+-rw-r--r--   0        0        0    33168 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/keybd_open.png
+-rw-r--r--   0        0        0    21422 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/status.json
+-rw-r--r--   0        0        0    12406 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/coverage_report/style.css
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/docs/make.bat
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/docs/requirements.txt
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/docs/source/conf.py
+-rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/docs/source/index.rst
+-rw-r--r--   0        0        0    10337 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/docs/source/extensions/apps.rst
+-rw-r--r--   0        0        0     3471 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/docs/source/extensions/autograders.rst
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/docs/source/extensions/index.rst
+-rw-r--r--   0        0        0    37523 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/docs/source/extensions/img/convert_grades.png
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/docs/source/getting_started/configuration.rst
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/docs/source/getting_started/index.rst
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/docs/source/getting_started/installation.rst
+-rw-r--r--   0        0        0     1981 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/docs/source/getting_started/modes.rst
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/docs/source/user_docs/authoring.rst
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/docs/source/user_docs/grade_export.rst
+-rw-r--r--   0        0        0     1566 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/docs/source/user_docs/grading.rst
+-rw-r--r--   0        0        0     1194 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/docs/source/user_docs/help_extension.rst
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/docs/source/user_docs/index.rst
+-rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/docs/source/user_docs/modes.rst
+-rw-r--r--   0        0        0     4946 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/docs/source/user_docs/cells/cells.rst
+-rw-r--r--   0        0        0    30552 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/docs/source/user_docs/cells/img/attachment_editor.png
+-rw-r--r--   0        0        0    80690 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/docs/source/user_docs/cells/img/diagram_editor.png
+-rw-r--r--   0        0        0    17552 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/docs/source/user_docs/cells/img/diagram_empty.png
+-rw-r--r--   0        0        0    21305 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/docs/source/user_docs/cells/img/diagram_filled.png
+-rw-r--r--   0        0        0    16291 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/docs/source/user_docs/cells/img/mc_edit.png
+-rw-r--r--   0        0        0    17990 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/docs/source/user_docs/cells/img/mc_render.png
+-rw-r--r--   0        0        0    12007 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/docs/source/user_docs/cells/img/sc_edit.png
+-rw-r--r--   0        0        0    14139 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/docs/source/user_docs/cells/img/sc_render.png
+-rw-r--r--   0        0        0    23745 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/docs/source/user_docs/cells/img/upload_question_rendered.png
+-rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/docs/source/user_docs/exchange/base_exchange.rst
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/docs/source/user_docs/exchange/index.rst
+-rw-r--r--   0        0        0     3075 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/docs/source/user_docs/exchange/submit.rst
+-rw-r--r--   0        0        0    50924 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/docs/source/user_docs/exchange/img/submitted_html.png
+-rw-r--r--   0        0        0    46425 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/docs/source/user_docs/exchange/img/submitted_html_de.png
+-rw-r--r--   0        0        0    75660 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/docs/source/user_docs/img/annotate_answer.png
+-rw-r--r--   0        0        0    36170 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/docs/source/user_docs/img/assignment_toolbar_code.png
+-rw-r--r--   0        0        0    34390 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/docs/source/user_docs/img/assignment_toolbar_md.png
+-rw-r--r--   0        0        0    12214 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/docs/source/user_docs/img/cell_type_change_alert.png
+-rw-r--r--   0        0        0    36165 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/docs/source/user_docs/img/exam_toolbar.png
+-rw-r--r--   0        0        0    77628 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/docs/source/user_docs/img/export_grades_dialog.png
+-rw-r--r--   0        0        0     7735 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/docs/source/user_docs/img/exported_grades.png
+-rw-r--r--   0        0        0     8706 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/docs/source/user_docs/img/exported_grades_max_score.png
+-rw-r--r--   0        0        0     7862 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/docs/source/user_docs/img/exported_grades_normalized.png
+-rw-r--r--   0        0        0    19045 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/docs/source/user_docs/img/help_tab.png
+-rw-r--r--   0        0        0    12085 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/docs/source/user_docs/img/move_cell_alert.png
+-rw-r--r--   0        0        0    45645 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/docs/source/user_docs/img/submit.png
+-rw-r--r--   0        0        0    79144 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/docs/source/user_docs/img/task_view.png
+-rw-r--r--   0        0        0    82489 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/docs/source/user_docs/img/task_view_task.png
+-rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/__init__.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/__main__.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/__version__.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/apps/__init__.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/apps/activatemodeapp.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/apps/baseapp.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/apps/deactivatemodeapp.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/apps/e2xgraderapp.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/apps/showmodeapp.py
+-rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/apps/togglemodeapp.py
+-rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/config/__init__.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/exchange/__init__.py
+-rw-r--r--   0        0        0     4698 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/exchange/collect.py
+-rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/exchange/exchange.py
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/exchange/fetch_assignment.py
+-rw-r--r--   0        0        0     6604 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/exchange/fetch_feedback.py
+-rw-r--r--   0        0        0     4795 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/exchange/hash_utils.py
+-rw-r--r--   0        0        0    11216 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/exchange/list.py
+-rw-r--r--   0        0        0     5819 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/exchange/release_assignment.py
+-rw-r--r--   0        0        0     5879 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/exchange/release_feedback.py
+-rw-r--r--   0        0        0     9801 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/exchange/submit.py
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/exchange/utils.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/exporters/__init__.py
+-rw-r--r--   0        0        0     4811 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/exporters/exporter.py
+-rw-r--r--   0        0        0     5052 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/exporters/gradeexporter.py
+-rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/exporters/submissionexporter.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/exporters/filters/__init__.py
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/exporters/filters/highlight.py
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/exporters/templates/hashcode_cell.html
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/extensions/__init__.py
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/extensions/base.py
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/extensions/manager.py
+-rw-r--r--   0        0        0     3070 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/extensions/nbextensions.py
+-rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/extensions/serverextensions.py
+-rw-r--r--   0        0        0     2023 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/extensions/utils.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/graders/__init__.py
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/graders/base.py
+-rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/graders/code.py
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/graders/multiplechoice.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/graders/singlechoice.py
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/preprocessors/__init__.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/preprocessors/clearhiddentests.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/preprocessors/clearsolutions.py
+-rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/preprocessors/extractattachments.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/preprocessors/filtercellsbyid.py
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/preprocessors/filtertests.py
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/preprocessors/overwritecells.py
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/preprocessors/permutetasks.py
+-rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/preprocessors/saveautogrades.py
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/preprocessors/savecells.py
+-rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/preprocessors/scramble.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/preprocessors/unpermutetasks.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/preprocessors/unscramble.py
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/preprocessors/validateextracells.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/__init__.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/assignment_list/__init__.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/assignment_list/assignmentlist.py
+-rw-r--r--   0        0        0     3886 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/assignment_list/handlers.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/diagram_editor/__init__.py
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/diagram_editor/diagrameditor.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/e2xgraderapi/__init__.py
+-rw-r--r--   0        0        0     5382 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/e2xgraderapi/apihandlers.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/e2xgraderapi/e2xgraderapi.py
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/e2xgraderapi/presets/questions/Code (Autograded).ipynb
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/e2xgraderapi/presets/questions/Code (Manual).ipynb
+-rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/e2xgraderapi/presets/questions/Diagram.ipynb
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/e2xgraderapi/presets/questions/Freetext.ipynb
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/e2xgraderapi/presets/questions/Multiple Choice.ipynb
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/e2xgraderapi/presets/questions/Single Choice.ipynb
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/e2xgraderapi/presets/questions/Upload Files.ipynb
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/e2xgraderapi/presets/template/Footer.ipynb
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/e2xgraderapi/presets/template/Group Info.ipynb
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/e2xgraderapi/presets/template/Header.ipynb
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/e2xgraderapi/presets/template/Student Info.ipynb
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/e2xgraderapi/templates/feedback/conf.json
+-rw-r--r--   0        0        0     8033 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/e2xgraderapi/templates/feedback/index.html.j2
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/e2xgraderapi/templates/form/conf.json
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/e2xgraderapi/templates/form/index.html.j2
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/formgrader/__init__.py
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/formgrader/formgrader.py
+-rw-r--r--   0        0        0     9023 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/formgrader/handlers.py
+-rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/formgrader/static/css/eraser-solid.svg
+-rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/formgrader/static/css/pencil-solid.svg
+-rw-r--r--   0        0        0    10212 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/formgrader/static/js/formgrade.js
+-rw-r--r--   0        0        0    10309 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/formgrader/static/js/formgrade_models.js
+-rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/formgrader/static/js/gradebook_assignments.js
+-rw-r--r--   0        0        0     7144 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/formgrader/static/js/gradebook_notebook_submissions.js
+-rw-r--r--   0        0        0     4460 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/formgrader/static/js/gradebook_notebooks.js
+-rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/formgrader/static/js/gradebook_tasks.js
+-rw-r--r--   0        0        0    20909 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/formgrader/static/js/manage_assignments.js
+-rw-r--r--   0        0        0    11457 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/formgrader/static/js/manage_submissions.js
+-rw-r--r--   0        0        0     6587 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/formgrader/templates/base.tpl
+-rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/formgrader/templates/export_grades.tpl
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/formgrader/templates/gradebook_base.tpl
+-rw-r--r--   0        0        0     4476 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/formgrader/templates/manage_assignments.tpl
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/formgrader/templates/manage_students_base.tpl
+-rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/formgrader/templates/manage_submissions.tpl
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/formgrader/templates/formgrade/conf.json
+-rw-r--r--   0        0        0     5542 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/formgrader/templates/formgrade/formgrade_macros.html.j2
+-rw-r--r--   0        0        0    12093 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/formgrader/templates/formgrade/index.html.j2
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/formgrader/templates/task_view/gradebook_assignments.tpl
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/formgrader/templates/task_view/gradebook_base.tpl
+-rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/formgrader/templates/task_view/gradebook_notebook_submissions.tpl
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/formgrader/templates/task_view/gradebook_notebooks.tpl
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/formgrader/templates/task_view/gradebook_tasks.tpl
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/help/__init__.py
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/help/apihandlers.py
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/help/help.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/nbgraderapi/__init__.py
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/nbgraderapi/nbgraderapi.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/validate_assignment/__init__.py
+-rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/validate_assignment/handlers.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/validate_assignment/validateassignment.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/validate_assignment/validator.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/base/__init__.py
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/base/extension.py
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/student/__init__.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/student/student.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/student_exam/__init__.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/student_exam/student_exam.py
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/teacher/__init__.py
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/teacher/teacher.py
+-rw-r--r--   0        0        0   136895 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/static/nbextensions/notebook/student/main.js
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/static/nbextensions/notebook/student/main.js.LICENSE.txt
+-rw-r--r--   0        0        0   167463 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/static/nbextensions/notebook/student_exam/main.js
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/static/nbextensions/notebook/student_exam/main.js.LICENSE.txt
+-rw-r--r--   0        0        0   169081 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/static/nbextensions/notebook/teacher/main.js
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/static/nbextensions/notebook/teacher/main.js.LICENSE.txt
+-rw-r--r--   0        0        0     3675 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/static/nbextensions/tree/student/main.js
+-rw-r--r--   0        0        0    13280 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/static/nbextensions/tree/student_exam/main.js
+-rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/static/nbextensions/tree/teacher/main.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/tests/apps/__init__.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/tests/apps/test_activatemodeapp.py
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/tests/apps/test_baseapp.py
+-rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/tests/apps/test_deactivatemodeapp.py
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/tests/apps/test_e2xgraderapp.py
+-rw-r--r--   0        0        0     6964 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/tests/apps/test_e2xmanager.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/tests/apps/test_showmodeapp.py
+-rw-r--r--   0        0        0     2359 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/tests/apps/test_togglemodeapp.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/tests/exchange/__init__.py
+-rw-r--r--   0        0        0     5363 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/tests/exchange/test_hash_utils.py
+-rw-r--r--   0        0        0    13121 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/tests/exchange/test_submit.py
+-rw-r--r--   0        0        0     3041 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/tests/exchange/test_utils.py
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/tests/exchange/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/tests/exporters/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/tests/exporters/filters/__init__.py
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/tests/exporters/filters/test_highlight.py
+-rw-r--r--   0        0        0     4251 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/tests/extensions/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/tests/graders/__init__.py
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/tests/graders/test_base.py
+-rw-r--r--   0        0        0     3159 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/tests/graders/test_code.py
+-rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/tests/graders/test_multiplechoice.py
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/tests/graders/test_singlechoice.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/tests/preprocessors/__init__.py
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/tests/preprocessors/test_clearhiddentests.py
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/tests/preprocessors/test_clearsolutions.py
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/tests/preprocessors/test_extractattachments.py
+-rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/tests/preprocessors/test_filtercellsbyid.py
+-rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/tests/preprocessors/test_filtertests.py
+-rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/tests/preprocessors/test_unscramble.py
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/tests/preprocessors/test_validateextracells.py
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/tests/server_extensions/apps/diagram_editor/test_diagrameditor.py
+-rw-r--r--   0        0        0     3267 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/tests/server_extensions/apps/validate_assignment/test_validator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/tests/test_utils/__init__.py
+-rw-r--r--   0        0        0     4757 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/tests/test_utils/cells.py
+-rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/tests/test_utils/test_utils.py
+-rw-r--r--   0        0        0     5123 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/tests/utils/test_mode.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/utils/__init__.py
+-rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/utils/extra_cells.py
+-rw-r--r--   0        0        0     4591 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/utils/mode.py
+-rw-r--r--   0        0        0     3295 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/e2xgrader/utils/nbgrader_cells.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/etc/jupyter/jupyter_server_config.d/e2xgrader.json
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/LICENSE
+-rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/README.md
+-rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/pyproject.toml
+-rw-r--r--   0        0        0     3795 2020-02-02 00:00:00.000000 e2xgrader-0.3.0.dev2/PKG-INFO
```

### Comparing `e2xgrader-0.3.0.dev1/.pre-commit-config.yaml` & `e2xgrader-0.3.0.dev2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/.readthedocs.yaml` & `e2xgrader-0.3.0.dev2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/nbgrader_config.py` & `e2xgrader-0.3.0.dev2/nbgrader_config.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/package-lock.json` & `e2xgrader-0.3.0.dev2/package-lock.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9165651487152658%*

 * *Differences: {"'dependencies'": "{'@e2xgrader/assignment-view-celltoolbar': {'requires': {'@e2xgrader/cells': "*

 * *                   "'0.3.0-dev2', '@e2xgrader/utils': '0.3.0-dev2'}}, "*

 * *                   "'@e2xgrader/authoring-menubar': {'requires': {'@e2xgrader/api': '0.3.0-dev2', "*

 * *                   "'@e2xgrader/menubar': '0.3.0-dev2', '@e2xgrader/utils': '0.3.0-dev2'}}, "*

 * *                   "'@e2xgrader/cell-extension': {'requires': {'@e2xgrader/cells': '0.3.0-dev2'}}, "*

 * *                   "'@e2xgrader/cells': {'requ […]*

```diff
@@ -1258,80 +1258,80 @@
                 "webpack-cli": "^4.9.2"
             },
             "version": "file:packages/api"
         },
         "@e2xgrader/assignment-view-celltoolbar": {
             "requires": {
                 "@babel/preset-env": "^7.16.11",
-                "@e2xgrader/cells": "0.3.0-dev1",
-                "@e2xgrader/utils": "0.3.0-dev1",
+                "@e2xgrader/cells": "0.3.0-dev2",
+                "@e2xgrader/utils": "0.3.0-dev2",
                 "css-loader": "^6.6.0",
                 "style-loader": "^3.3.1",
                 "webpack": "^5.70.0",
                 "webpack-cli": "^4.9.2"
             },
             "version": "file:packages/assignment-view-celltoolbar"
         },
         "@e2xgrader/authoring-menubar": {
             "requires": {
-                "@e2xgrader/api": "0.3.0-dev1",
-                "@e2xgrader/menubar": "0.3.0-dev1",
-                "@e2xgrader/utils": "0.3.0-dev1",
+                "@e2xgrader/api": "0.3.0-dev2",
+                "@e2xgrader/menubar": "0.3.0-dev2",
+                "@e2xgrader/utils": "0.3.0-dev2",
                 "webpack": "^5.73.0",
                 "webpack-cli": "^4.9.2"
             },
             "version": "file:packages/authoring-menubar"
         },
         "@e2xgrader/cell-extension": {
             "requires": {
                 "@babel/preset-env": "^7.16.11",
-                "@e2xgrader/cells": "0.3.0-dev1",
+                "@e2xgrader/cells": "0.3.0-dev2",
                 "css-loader": "^6.6.0",
                 "style-loader": "^3.3.1",
                 "webpack": "^5.70.0",
                 "webpack-cli": "^4.9.2"
             },
             "version": "file:packages/cell-extension"
         },
         "@e2xgrader/cells": {
             "requires": {
                 "@babel/preset-env": "^7.16.11",
-                "@e2xgrader/api": "0.3.0-dev1",
+                "@e2xgrader/api": "0.3.0-dev2",
                 "css-loader": "^6.6.0",
                 "style-loader": "^3.3.1",
                 "webpack": "^5.70.0",
                 "webpack-cli": "^4.9.2"
             },
             "version": "file:packages/cells"
         },
         "@e2xgrader/create-assignment-celltoolbar": {
             "requires": {
                 "@babel/preset-env": "^7.16.11",
-                "@e2xgrader/cells": "0.3.0-dev1",
-                "@e2xgrader/utils": "0.3.0-dev1",
+                "@e2xgrader/cells": "0.3.0-dev2",
+                "@e2xgrader/utils": "0.3.0-dev2",
                 "css-loader": "^6.6.0",
                 "style-loader": "^3.3.1",
                 "webpack": "^5.70.0",
                 "webpack-cli": "^4.9.2"
             },
             "version": "file:packages/create-assignment-celltoolbar"
         },
         "@e2xgrader/exam-menubar": {
             "requires": {
-                "@e2xgrader/api": "0.3.0-dev1",
-                "@e2xgrader/menubar": "0.3.0-dev1",
+                "@e2xgrader/api": "0.3.0-dev2",
+                "@e2xgrader/menubar": "0.3.0-dev2",
                 "webpack": "^5.73.0",
                 "webpack-cli": "^4.9.2"
             },
             "version": "file:packages/exam-menubar"
         },
         "@e2xgrader/help-tab": {
             "requires": {
                 "@babel/preset-env": "^7.16.11",
-                "@e2xgrader/api": "0.3.0-dev1",
+                "@e2xgrader/api": "0.3.0-dev2",
                 "css-loader": "^6.6.0",
                 "style-loader": "^3.3.1",
                 "webpack": "^5.70.0",
                 "webpack-cli": "^4.9.2"
             },
             "version": "file:packages/help-tab"
         },
@@ -1341,59 +1341,59 @@
                 "webpack-cli": "^4.9.2"
             },
             "version": "file:packages/menubar"
         },
         "@e2xgrader/notebook-extensions": {
             "requires": {
                 "@babel/preset-env": "^7.16.11",
-                "@e2xgrader/assignment-view-celltoolbar": "0.3.0-dev1",
-                "@e2xgrader/authoring-menubar": "0.3.0-dev1",
-                "@e2xgrader/cell-extension": "0.3.0-dev1",
-                "@e2xgrader/create-assignment-celltoolbar": "0.3.0-dev1",
-                "@e2xgrader/exam-menubar": "0.3.0-dev1",
-                "@e2xgrader/restricted-assignment-notebook": "0.3.0-dev1",
-                "@e2xgrader/restricted-exam-notebook": "0.3.0-dev1",
-                "@e2xgrader/utils": "0.3.0-dev1",
+                "@e2xgrader/assignment-view-celltoolbar": "0.3.0-dev2",
+                "@e2xgrader/authoring-menubar": "0.3.0-dev2",
+                "@e2xgrader/cell-extension": "0.3.0-dev2",
+                "@e2xgrader/create-assignment-celltoolbar": "0.3.0-dev2",
+                "@e2xgrader/exam-menubar": "0.3.0-dev2",
+                "@e2xgrader/restricted-assignment-notebook": "0.3.0-dev2",
+                "@e2xgrader/restricted-exam-notebook": "0.3.0-dev2",
+                "@e2xgrader/utils": "0.3.0-dev2",
                 "css-loader": "^6.6.0",
                 "style-loader": "^3.3.1",
                 "webpack": "^5.70.0",
                 "webpack-cli": "^4.9.2"
             },
             "version": "file:packages/notebook-extensions"
         },
         "@e2xgrader/restricted-assignment-notebook": {
             "requires": {
-                "@e2xgrader/utils": "0.3.0-dev1",
+                "@e2xgrader/utils": "0.3.0-dev2",
                 "webpack": "^5.73.0",
                 "webpack-cli": "^4.9.2"
             },
             "version": "file:packages/restricted-assignment-notebook"
         },
         "@e2xgrader/restricted-exam-notebook": {
             "requires": {
-                "@e2xgrader/utils": "0.3.0-dev1",
+                "@e2xgrader/utils": "0.3.0-dev2",
                 "webpack": "^5.73.0",
                 "webpack-cli": "^4.9.2"
             },
             "version": "file:packages/restricted-exam-notebook"
         },
         "@e2xgrader/tree-extensions": {
             "requires": {
                 "@babel/preset-env": "^7.16.11",
-                "@e2xgrader/help-tab": "0.3.0-dev1",
+                "@e2xgrader/help-tab": "0.3.0-dev2",
                 "css-loader": "^6.6.0",
                 "style-loader": "^3.3.1",
                 "webpack": "^5.70.0",
                 "webpack-cli": "^4.9.2"
             },
             "version": "file:packages/tree-extensions"
         },
         "@e2xgrader/utils": {
             "requires": {
-                "@e2xgrader/api": "0.3.0-dev1",
+                "@e2xgrader/api": "0.3.0-dev2",
                 "webpack": "^5.73.0",
                 "webpack-cli": "^4.9.2"
             },
             "version": "file:packages/utils"
         },
         "@gar/promisify": {
             "dev": true,
@@ -10791,15 +10791,15 @@
                 "babel-preset-env": "^1.7.0",
                 "lerna": "^5.3.0",
                 "prettier": "^2.7.1"
             },
             "hasInstallScript": true,
             "license": "MIT",
             "name": "e2xgrader",
-            "version": "0.3.0-dev1",
+            "version": "0.3.0-dev2",
             "workspaces": [
                 "packages/*"
             ]
         },
         "node_modules/@ampproject/remapping": {
             "dependencies": {
                 "@jridgewell/gen-mapping": "^0.1.0",
@@ -24464,31 +24464,31 @@
         "packages/api": {
             "devDependencies": {
                 "webpack": "^5.73.0",
                 "webpack-cli": "^4.9.2"
             },
             "license": "MIT",
             "name": "@e2xgrader/api",
-            "version": "0.3.0-dev1"
+            "version": "0.3.0-dev2"
         },
         "packages/assignment-view-celltoolbar": {
             "dependencies": {
-                "@e2xgrader/cells": "0.3.0-dev1",
-                "@e2xgrader/utils": "0.3.0-dev1"
+                "@e2xgrader/cells": "0.3.0-dev2",
+                "@e2xgrader/utils": "0.3.0-dev2"
             },
             "devDependencies": {
                 "@babel/preset-env": "^7.16.11",
                 "css-loader": "^6.6.0",
                 "style-loader": "^3.3.1",
                 "webpack": "^5.70.0",
                 "webpack-cli": "^4.9.2"
             },
             "license": "ISC",
             "name": "@e2xgrader/assignment-view-celltoolbar",
-            "version": "0.3.0-dev1"
+            "version": "0.3.0-dev2"
         },
         "packages/authoring": {
             "dependencies": {
                 "@e2xgrader/api": "*",
                 "@emotion/react": "^11.9.3",
                 "@emotion/styled": "^11.9.3",
                 "@fontsource/roboto": "^4.5.7",
@@ -24505,71 +24505,71 @@
             },
             "extraneous": true,
             "name": "@e2xgrader/authoring",
             "version": "0.1.0"
         },
         "packages/authoring-menubar": {
             "dependencies": {
-                "@e2xgrader/api": "0.3.0-dev1",
-                "@e2xgrader/menubar": "0.3.0-dev1",
-                "@e2xgrader/utils": "0.3.0-dev1"
+                "@e2xgrader/api": "0.3.0-dev2",
+                "@e2xgrader/menubar": "0.3.0-dev2",
+                "@e2xgrader/utils": "0.3.0-dev2"
             },
             "devDependencies": {
                 "webpack": "^5.73.0",
                 "webpack-cli": "^4.9.2"
             },
             "license": "MIT",
             "name": "@e2xgrader/authoring-menubar",
-            "version": "0.3.0-dev1"
+            "version": "0.3.0-dev2"
         },
         "packages/cell-extension": {
             "dependencies": {
-                "@e2xgrader/cells": "0.3.0-dev1"
+                "@e2xgrader/cells": "0.3.0-dev2"
             },
             "devDependencies": {
                 "@babel/preset-env": "^7.16.11",
                 "css-loader": "^6.6.0",
                 "style-loader": "^3.3.1",
                 "webpack": "^5.70.0",
                 "webpack-cli": "^4.9.2"
             },
             "license": "ISC",
             "name": "@e2xgrader/cell-extension",
-            "version": "0.3.0-dev1"
+            "version": "0.3.0-dev2"
         },
         "packages/cells": {
             "dependencies": {
-                "@e2xgrader/api": "0.3.0-dev1"
+                "@e2xgrader/api": "0.3.0-dev2"
             },
             "devDependencies": {
                 "@babel/preset-env": "^7.16.11",
                 "css-loader": "^6.6.0",
                 "style-loader": "^3.3.1",
                 "webpack": "^5.70.0",
                 "webpack-cli": "^4.9.2"
             },
             "license": "ISC",
             "name": "@e2xgrader/cells",
-            "version": "0.3.0-dev1"
+            "version": "0.3.0-dev2"
         },
         "packages/create-assignment-celltoolbar": {
             "dependencies": {
-                "@e2xgrader/cells": "0.3.0-dev1",
-                "@e2xgrader/utils": "0.3.0-dev1"
+                "@e2xgrader/cells": "0.3.0-dev2",
+                "@e2xgrader/utils": "0.3.0-dev2"
             },
             "devDependencies": {
                 "@babel/preset-env": "^7.16.11",
                 "css-loader": "^6.6.0",
                 "style-loader": "^3.3.1",
                 "webpack": "^5.70.0",
                 "webpack-cli": "^4.9.2"
             },
             "license": "ISC",
             "name": "@e2xgrader/create-assignment-celltoolbar",
-            "version": "0.3.0-dev1"
+            "version": "0.3.0-dev2"
         },
         "packages/create-assignment-extension": {
             "devDependencies": {
                 "@babel/preset-env": "^7.16.11",
                 "@e2xgrader/cells": "*",
                 "css-loader": "^6.6.0",
                 "style-loader": "^3.3.1",
@@ -24579,48 +24579,48 @@
             "extraneous": true,
             "license": "ISC",
             "name": "@e2xgrader/create-assignment-extension",
             "version": "0.1.0.dev0"
         },
         "packages/exam-menubar": {
             "dependencies": {
-                "@e2xgrader/api": "0.3.0-dev1",
-                "@e2xgrader/menubar": "0.3.0-dev1"
+                "@e2xgrader/api": "0.3.0-dev2",
+                "@e2xgrader/menubar": "0.3.0-dev2"
             },
             "devDependencies": {
                 "webpack": "^5.73.0",
                 "webpack-cli": "^4.9.2"
             },
             "license": "MIT",
             "name": "@e2xgrader/exam-menubar",
-            "version": "0.3.0-dev1"
+            "version": "0.3.0-dev2"
         },
         "packages/help-tab": {
             "dependencies": {
-                "@e2xgrader/api": "0.3.0-dev1"
+                "@e2xgrader/api": "0.3.0-dev2"
             },
             "devDependencies": {
                 "@babel/preset-env": "^7.16.11",
                 "css-loader": "^6.6.0",
                 "style-loader": "^3.3.1",
                 "webpack": "^5.70.0",
                 "webpack-cli": "^4.9.2"
             },
             "license": "ISC",
             "name": "@e2xgrader/help-tab",
-            "version": "0.3.0-dev1"
+            "version": "0.3.0-dev2"
         },
         "packages/menubar": {
             "devDependencies": {
                 "webpack": "^5.73.0",
                 "webpack-cli": "^4.9.2"
             },
             "license": "MIT",
             "name": "@e2xgrader/menubar",
-            "version": "0.3.0-dev1"
+            "version": "0.3.0-dev2"
         },
         "packages/nbextensions": {
             "devDependencies": {
                 "babel-cli": "^6.26.0",
                 "babel-core": "^6.26.3",
                 "babel-plugin-transform-class-properties": "^6.24.1",
                 "babel-preset-env": "^1.7.0"
@@ -24638,82 +24638,82 @@
             "extraneous": true,
             "license": "MIT",
             "name": "@e2xgrader/nbgrader-utils",
             "version": "0.1.0.dev0"
         },
         "packages/notebook-extensions": {
             "dependencies": {
-                "@e2xgrader/assignment-view-celltoolbar": "0.3.0-dev1",
-                "@e2xgrader/authoring-menubar": "0.3.0-dev1",
-                "@e2xgrader/cell-extension": "0.3.0-dev1",
-                "@e2xgrader/create-assignment-celltoolbar": "0.3.0-dev1",
-                "@e2xgrader/exam-menubar": "0.3.0-dev1",
-                "@e2xgrader/restricted-assignment-notebook": "0.3.0-dev1",
-                "@e2xgrader/restricted-exam-notebook": "0.3.0-dev1",
-                "@e2xgrader/utils": "0.3.0-dev1"
+                "@e2xgrader/assignment-view-celltoolbar": "0.3.0-dev2",
+                "@e2xgrader/authoring-menubar": "0.3.0-dev2",
+                "@e2xgrader/cell-extension": "0.3.0-dev2",
+                "@e2xgrader/create-assignment-celltoolbar": "0.3.0-dev2",
+                "@e2xgrader/exam-menubar": "0.3.0-dev2",
+                "@e2xgrader/restricted-assignment-notebook": "0.3.0-dev2",
+                "@e2xgrader/restricted-exam-notebook": "0.3.0-dev2",
+                "@e2xgrader/utils": "0.3.0-dev2"
             },
             "devDependencies": {
                 "@babel/preset-env": "^7.16.11",
                 "css-loader": "^6.6.0",
                 "style-loader": "^3.3.1",
                 "webpack": "^5.70.0",
                 "webpack-cli": "^4.9.2"
             },
             "license": "ISC",
             "name": "@e2xgrader/notebook-extensions",
-            "version": "0.3.0-dev1"
+            "version": "0.3.0-dev2"
         },
         "packages/restricted-assignment-notebook": {
             "dependencies": {
-                "@e2xgrader/utils": "0.3.0-dev1"
+                "@e2xgrader/utils": "0.3.0-dev2"
             },
             "devDependencies": {
                 "webpack": "^5.73.0",
                 "webpack-cli": "^4.9.2"
             },
             "license": "MIT",
             "name": "@e2xgrader/restricted-assignment-notebook",
-            "version": "0.3.0-dev1"
+            "version": "0.3.0-dev2"
         },
         "packages/restricted-exam-notebook": {
             "dependencies": {
-                "@e2xgrader/utils": "0.3.0-dev1"
+                "@e2xgrader/utils": "0.3.0-dev2"
             },
             "devDependencies": {
                 "webpack": "^5.73.0",
                 "webpack-cli": "^4.9.2"
             },
             "license": "MIT",
             "name": "@e2xgrader/restricted-exam-notebook",
-            "version": "0.3.0-dev1"
+            "version": "0.3.0-dev2"
         },
         "packages/tree-extensions": {
             "dependencies": {
-                "@e2xgrader/help-tab": "0.3.0-dev1"
+                "@e2xgrader/help-tab": "0.3.0-dev2"
             },
             "devDependencies": {
                 "@babel/preset-env": "^7.16.11",
                 "css-loader": "^6.6.0",
                 "style-loader": "^3.3.1",
                 "webpack": "^5.70.0",
                 "webpack-cli": "^4.9.2"
             },
             "license": "ISC",
             "name": "@e2xgrader/tree-extensions",
-            "version": "0.3.0-dev1"
+            "version": "0.3.0-dev2"
         },
         "packages/utils": {
             "dependencies": {
-                "@e2xgrader/api": "0.3.0-dev1"
+                "@e2xgrader/api": "0.3.0-dev2"
             },
             "devDependencies": {
                 "webpack": "^5.73.0",
                 "webpack-cli": "^4.9.2"
             },
             "license": "MIT",
             "name": "@e2xgrader/utils",
-            "version": "0.3.0-dev1"
+            "version": "0.3.0-dev2"
         }
     },
     "requires": true,
-    "version": "0.3.0-dev1"
+    "version": "0.3.0-dev2"
 }
```

### Comparing `e2xgrader-0.3.0.dev1/package.json` & `e2xgrader-0.3.0.dev2/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'0.3.0-dev2'"}*

```diff
@@ -30,12 +30,12 @@
     },
     "scripts": {
         "build": "lerna run build",
         "install": "lerna run bootstrap",
         "prettier": "prettier --write \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\"",
         "prettier:files": "prettier --write"
     },
-    "version": "0.3.0-dev1",
+    "version": "0.3.0-dev2",
     "workspaces": [
         "packages/*"
     ]
 }
```

### Comparing `e2xgrader-0.3.0.dev1/.github/workflows/dispatch.yml` & `e2xgrader-0.3.0.dev2/.github/workflows/dispatch.yml`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/.github/workflows/python-package.yml` & `e2xgrader-0.3.0.dev2/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/.github/workflows/sonar-scan.yml` & `e2xgrader-0.3.0.dev2/.github/workflows/sonar-scan.yml`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/coverage_html.js` & `e2xgrader-0.3.0.dev2/coverage_report/coverage_html.js`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_0a574a50e34851d4___init___py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_0a574a50e34851d4___init___py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_0ff1fe3f8b795b70___init___py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_0ff1fe3f8b795b70___init___py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_0ff1fe3f8b795b70_activatemodeapp_py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_0ff1fe3f8b795b70_activatemodeapp_py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_0ff1fe3f8b795b70_baseapp_py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_0ff1fe3f8b795b70_baseapp_py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_0ff1fe3f8b795b70_deactivatemodeapp_py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_0ff1fe3f8b795b70_deactivatemodeapp_py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_0ff1fe3f8b795b70_e2xgraderapp_py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_0ff1fe3f8b795b70_e2xgraderapp_py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_0ff1fe3f8b795b70_showmodeapp_py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_0ff1fe3f8b795b70_showmodeapp_py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_0ff1fe3f8b795b70_togglemodeapp_py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_0ff1fe3f8b795b70_togglemodeapp_py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_2448a76917b6613d___init___py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_2448a76917b6613d___init___py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_2448a76917b6613d_assignmentlist_py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_2448a76917b6613d_assignmentlist_py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_2448a76917b6613d_handlers_py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_2448a76917b6613d_handlers_py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_294994a5caef5622___init___py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_294994a5caef5622___init___py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_294994a5caef5622_student_py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_294994a5caef5622_student_py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_2d23d5c010468094___init___py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_2d23d5c010468094___init___py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_2d23d5c010468094_clearhiddentests_py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_2d23d5c010468094_clearhiddentests_py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_2d23d5c010468094_clearsolutions_py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_2d23d5c010468094_clearsolutions_py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_2d23d5c010468094_extractattachments_py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_2d23d5c010468094_extractattachments_py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_2d23d5c010468094_filtercellsbyid_py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_2d23d5c010468094_filtercellsbyid_py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_2d23d5c010468094_filtertests_py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_2d23d5c010468094_filtertests_py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_2d23d5c010468094_overwritecells_py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_2d23d5c010468094_overwritecells_py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_2d23d5c010468094_permutetasks_py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_2d23d5c010468094_permutetasks_py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_2d23d5c010468094_saveautogrades_py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_2d23d5c010468094_saveautogrades_py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_2d23d5c010468094_savecells_py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_2d23d5c010468094_savecells_py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_2d23d5c010468094_scramble_py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_2d23d5c010468094_scramble_py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_2d23d5c010468094_unpermutetasks_py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_2d23d5c010468094_unpermutetasks_py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_2d23d5c010468094_unscramble_py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_2d23d5c010468094_unscramble_py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_2d23d5c010468094_validateextracells_py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_2d23d5c010468094_validateextracells_py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_37d73105d5cffd7e___init___py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_37d73105d5cffd7e___init___py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_37d73105d5cffd7e_base_py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_37d73105d5cffd7e_base_py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_37d73105d5cffd7e_code_py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_37d73105d5cffd7e_code_py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_37d73105d5cffd7e_multiplechoice_py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_37d73105d5cffd7e_multiplechoice_py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_37d73105d5cffd7e_singlechoice_py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_37d73105d5cffd7e_singlechoice_py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_5beb92c0ecba1ed4___init___py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_5beb92c0ecba1ed4___init___py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_5ef362e6f46f83e2___init___py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_5ef362e6f46f83e2___init___py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_710bf0b8e9508f41___init___py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_710bf0b8e9508f41___init___py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_710bf0b8e9508f41_highlight_py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_710bf0b8e9508f41_highlight_py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_7805cff25cc2d712___init___py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_7805cff25cc2d712___init___py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_7805cff25cc2d712_extra_cells_py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_7805cff25cc2d712_extra_cells_py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_7805cff25cc2d712_mode_py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_7805cff25cc2d712_mode_py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_78932b1391e2ad05___init___py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_78932b1391e2ad05___init___py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_78932b1391e2ad05_nbgraderapi_py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_78932b1391e2ad05_nbgraderapi_py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_83df762bc77ead36___init___py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_83df762bc77ead36___init___py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_866c9e7ae337468e___init___py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_866c9e7ae337468e___init___py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_866c9e7ae337468e_teacher_py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_866c9e7ae337468e_teacher_py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_8fe6e31f42e6838f___init___py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_8fe6e31f42e6838f___init___py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_94f16e40fada4634___init___py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_94f16e40fada4634___init___py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_94f16e40fada4634_apihandlers_py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_94f16e40fada4634_apihandlers_py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_94f16e40fada4634_help_py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_94f16e40fada4634_help_py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_98391cc2871b8725___init___py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_98391cc2871b8725___init___py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_98391cc2871b8725_base_py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_98391cc2871b8725_base_py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_98391cc2871b8725_manager_py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_98391cc2871b8725_manager_py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_98391cc2871b8725_nbextensions_py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_98391cc2871b8725_nbextensions_py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_98391cc2871b8725_serverextensions_py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_98391cc2871b8725_serverextensions_py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_98391cc2871b8725_utils_py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_98391cc2871b8725_utils_py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_9b0ce7ff0ae20648___init___py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_9b0ce7ff0ae20648___init___py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_9b0ce7ff0ae20648_apihandlers_py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_9b0ce7ff0ae20648_apihandlers_py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_9b0ce7ff0ae20648_e2xgraderapi_py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_9b0ce7ff0ae20648_e2xgraderapi_py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_c74475b6151f7a7b___init___py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_c74475b6151f7a7b___init___py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_c74475b6151f7a7b_cells_py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_c74475b6151f7a7b_cells_py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_d878b7d22c4c16e4___init___py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_d878b7d22c4c16e4___init___py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_d878b7d22c4c16e4_diagrameditor_py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_d878b7d22c4c16e4_diagrameditor_py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_dbfe9cfbceae7526___init___py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_dbfe9cfbceae7526___init___py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_e43806ab68cc7f97___init___py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_e43806ab68cc7f97___init___py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_e43806ab68cc7f97_student_exam_py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_e43806ab68cc7f97_student_exam_py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_e533b0b56079eb7c___init___py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_e533b0b56079eb7c___init___py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_e533b0b56079eb7c_exporter_py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_e533b0b56079eb7c_exporter_py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_e533b0b56079eb7c_gradeexporter_py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_e533b0b56079eb7c_gradeexporter_py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_e533b0b56079eb7c_submissionexporter_py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_e533b0b56079eb7c_submissionexporter_py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_e7343efe92bf6800___init___py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_e7343efe92bf6800___init___py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_e7343efe92bf6800_formgrader_py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_e7343efe92bf6800_formgrader_py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_e7343efe92bf6800_handlers_py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_e7343efe92bf6800_handlers_py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_f7a0650fde384913___init___py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_f7a0650fde384913___init___py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_fddc8d031c76e3e4___init___py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_fddc8d031c76e3e4___init___py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_fddc8d031c76e3e4_collect_py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_fddc8d031c76e3e4_collect_py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_fddc8d031c76e3e4_exchange_py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_fddc8d031c76e3e4_exchange_py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_fddc8d031c76e3e4_fetch_assignment_py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_fddc8d031c76e3e4_fetch_assignment_py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_fddc8d031c76e3e4_fetch_feedback_py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_fddc8d031c76e3e4_fetch_feedback_py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_fddc8d031c76e3e4_hash_utils_py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_fddc8d031c76e3e4_hash_utils_py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_fddc8d031c76e3e4_list_py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_fddc8d031c76e3e4_list_py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_fddc8d031c76e3e4_release_assignment_py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_fddc8d031c76e3e4_release_assignment_py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_fddc8d031c76e3e4_release_feedback_py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_fddc8d031c76e3e4_release_feedback_py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_fddc8d031c76e3e4_submit_py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_fddc8d031c76e3e4_submit_py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_fddc8d031c76e3e4_utils_py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_fddc8d031c76e3e4_utils_py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_ff9ed41ff67ae67c___init___py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_ff9ed41ff67ae67c___init___py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_ff9ed41ff67ae67c_handlers_py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_ff9ed41ff67ae67c_handlers_py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_ff9ed41ff67ae67c_validateassignment_py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_ff9ed41ff67ae67c_validateassignment_py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_ff9ed41ff67ae67c_validator_py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_ff9ed41ff67ae67c_validator_py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_ffb521de3e56ad10___init___py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_ffb521de3e56ad10___init___py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_ffb521de3e56ad10_extension_py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_ffb521de3e56ad10_extension_py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/d_ffe7516a0565d1ec___init___py.html` & `e2xgrader-0.3.0.dev2/coverage_report/d_ffe7516a0565d1ec___init___py.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/favicon_32.png` & `e2xgrader-0.3.0.dev2/coverage_report/favicon_32.png`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/index.html` & `e2xgrader-0.3.0.dev2/coverage_report/index.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/keybd_closed.png` & `e2xgrader-0.3.0.dev2/coverage_report/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/keybd_open.png` & `e2xgrader-0.3.0.dev2/coverage_report/keybd_open.png`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/status.json` & `e2xgrader-0.3.0.dev2/coverage_report/status.json`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/coverage_report/style.css` & `e2xgrader-0.3.0.dev2/coverage_report/style.css`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/docs/Makefile` & `e2xgrader-0.3.0.dev2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/docs/make.bat` & `e2xgrader-0.3.0.dev2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/docs/source/conf.py` & `e2xgrader-0.3.0.dev2/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = "e2xgrader"
 copyright = "2023, Tim Metzler"
 author = "Tim Metzler"
-release = "0.3.0-dev1"
+release = "0.3.0-dev2"
 github_project_url = "https://github.com/Digiklausur/e2xgrader"
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = []
```

### Comparing `e2xgrader-0.3.0.dev1/docs/source/index.rst` & `e2xgrader-0.3.0.dev2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/docs/source/extensions/apps.rst` & `e2xgrader-0.3.0.dev2/docs/source/extensions/apps.rst`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/docs/source/extensions/autograders.rst` & `e2xgrader-0.3.0.dev2/docs/source/extensions/autograders.rst`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/docs/source/extensions/img/convert_grades.png` & `e2xgrader-0.3.0.dev2/docs/source/extensions/img/convert_grades.png`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/docs/source/getting_started/configuration.rst` & `e2xgrader-0.3.0.dev2/docs/source/getting_started/configuration.rst`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/docs/source/getting_started/modes.rst` & `e2xgrader-0.3.0.dev2/docs/source/getting_started/modes.rst`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/docs/source/user_docs/grade_export.rst` & `e2xgrader-0.3.0.dev2/docs/source/user_docs/grade_export.rst`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/docs/source/user_docs/grading.rst` & `e2xgrader-0.3.0.dev2/docs/source/user_docs/grading.rst`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/docs/source/user_docs/help_extension.rst` & `e2xgrader-0.3.0.dev2/docs/source/user_docs/help_extension.rst`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/docs/source/user_docs/modes.rst` & `e2xgrader-0.3.0.dev2/docs/source/user_docs/modes.rst`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/docs/source/user_docs/cells/cells.rst` & `e2xgrader-0.3.0.dev2/docs/source/user_docs/cells/cells.rst`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/docs/source/user_docs/cells/img/attachment_editor.png` & `e2xgrader-0.3.0.dev2/docs/source/user_docs/cells/img/attachment_editor.png`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/docs/source/user_docs/cells/img/diagram_editor.png` & `e2xgrader-0.3.0.dev2/docs/source/user_docs/cells/img/diagram_editor.png`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/docs/source/user_docs/cells/img/diagram_empty.png` & `e2xgrader-0.3.0.dev2/docs/source/user_docs/cells/img/diagram_empty.png`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/docs/source/user_docs/cells/img/diagram_filled.png` & `e2xgrader-0.3.0.dev2/docs/source/user_docs/cells/img/diagram_filled.png`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/docs/source/user_docs/cells/img/mc_edit.png` & `e2xgrader-0.3.0.dev2/docs/source/user_docs/cells/img/mc_edit.png`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/docs/source/user_docs/cells/img/mc_render.png` & `e2xgrader-0.3.0.dev2/docs/source/user_docs/cells/img/mc_render.png`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/docs/source/user_docs/cells/img/sc_edit.png` & `e2xgrader-0.3.0.dev2/docs/source/user_docs/cells/img/sc_edit.png`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/docs/source/user_docs/cells/img/sc_render.png` & `e2xgrader-0.3.0.dev2/docs/source/user_docs/cells/img/sc_render.png`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/docs/source/user_docs/cells/img/upload_question_rendered.png` & `e2xgrader-0.3.0.dev2/docs/source/user_docs/cells/img/upload_question_rendered.png`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/docs/source/user_docs/exchange/base_exchange.rst` & `e2xgrader-0.3.0.dev2/docs/source/user_docs/exchange/base_exchange.rst`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/docs/source/user_docs/exchange/submit.rst` & `e2xgrader-0.3.0.dev2/docs/source/user_docs/exchange/submit.rst`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/docs/source/user_docs/exchange/img/submitted_html.png` & `e2xgrader-0.3.0.dev2/docs/source/user_docs/exchange/img/submitted_html.png`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/docs/source/user_docs/exchange/img/submitted_html_de.png` & `e2xgrader-0.3.0.dev2/docs/source/user_docs/exchange/img/submitted_html_de.png`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/docs/source/user_docs/img/annotate_answer.png` & `e2xgrader-0.3.0.dev2/docs/source/user_docs/img/annotate_answer.png`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/docs/source/user_docs/img/assignment_toolbar_code.png` & `e2xgrader-0.3.0.dev2/docs/source/user_docs/img/assignment_toolbar_code.png`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/docs/source/user_docs/img/assignment_toolbar_md.png` & `e2xgrader-0.3.0.dev2/docs/source/user_docs/img/assignment_toolbar_md.png`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/docs/source/user_docs/img/cell_type_change_alert.png` & `e2xgrader-0.3.0.dev2/docs/source/user_docs/img/cell_type_change_alert.png`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/docs/source/user_docs/img/exam_toolbar.png` & `e2xgrader-0.3.0.dev2/docs/source/user_docs/img/exam_toolbar.png`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/docs/source/user_docs/img/export_grades_dialog.png` & `e2xgrader-0.3.0.dev2/docs/source/user_docs/img/export_grades_dialog.png`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/docs/source/user_docs/img/exported_grades.png` & `e2xgrader-0.3.0.dev2/docs/source/user_docs/img/exported_grades.png`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/docs/source/user_docs/img/exported_grades_max_score.png` & `e2xgrader-0.3.0.dev2/docs/source/user_docs/img/exported_grades_max_score.png`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/docs/source/user_docs/img/exported_grades_normalized.png` & `e2xgrader-0.3.0.dev2/docs/source/user_docs/img/exported_grades_normalized.png`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/docs/source/user_docs/img/help_tab.png` & `e2xgrader-0.3.0.dev2/docs/source/user_docs/img/help_tab.png`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/docs/source/user_docs/img/move_cell_alert.png` & `e2xgrader-0.3.0.dev2/docs/source/user_docs/img/move_cell_alert.png`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/docs/source/user_docs/img/submit.png` & `e2xgrader-0.3.0.dev2/docs/source/user_docs/img/submit.png`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/docs/source/user_docs/img/task_view.png` & `e2xgrader-0.3.0.dev2/docs/source/user_docs/img/task_view.png`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/docs/source/user_docs/img/task_view_task.png` & `e2xgrader-0.3.0.dev2/docs/source/user_docs/img/task_view_task.png`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/__init__.py` & `e2xgrader-0.3.0.dev2/e2xgrader/__init__.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/apps/activatemodeapp.py` & `e2xgrader-0.3.0.dev2/e2xgrader/apps/activatemodeapp.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/apps/baseapp.py` & `e2xgrader-0.3.0.dev2/e2xgrader/apps/baseapp.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/apps/e2xgraderapp.py` & `e2xgrader-0.3.0.dev2/e2xgrader/apps/e2xgraderapp.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/apps/togglemodeapp.py` & `e2xgrader-0.3.0.dev2/e2xgrader/apps/togglemodeapp.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/config/__init__.py` & `e2xgrader-0.3.0.dev2/e2xgrader/config/__init__.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/exchange/__init__.py` & `e2xgrader-0.3.0.dev2/e2xgrader/exchange/__init__.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/exchange/collect.py` & `e2xgrader-0.3.0.dev2/e2xgrader/exchange/collect.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/exchange/exchange.py` & `e2xgrader-0.3.0.dev2/e2xgrader/exchange/exchange.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/exchange/fetch_assignment.py` & `e2xgrader-0.3.0.dev2/e2xgrader/exchange/fetch_assignment.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/exchange/fetch_feedback.py` & `e2xgrader-0.3.0.dev2/e2xgrader/exchange/fetch_feedback.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/exchange/hash_utils.py` & `e2xgrader-0.3.0.dev2/e2xgrader/exchange/hash_utils.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/exchange/list.py` & `e2xgrader-0.3.0.dev2/e2xgrader/exchange/list.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/exchange/release_assignment.py` & `e2xgrader-0.3.0.dev2/e2xgrader/exchange/release_assignment.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/exchange/release_feedback.py` & `e2xgrader-0.3.0.dev2/e2xgrader/exchange/release_feedback.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/exchange/submit.py` & `e2xgrader-0.3.0.dev2/e2xgrader/exchange/submit.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/exchange/utils.py` & `e2xgrader-0.3.0.dev2/e2xgrader/exchange/utils.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/exporters/exporter.py` & `e2xgrader-0.3.0.dev2/e2xgrader/exporters/exporter.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/exporters/gradeexporter.py` & `e2xgrader-0.3.0.dev2/e2xgrader/exporters/gradeexporter.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/exporters/submissionexporter.py` & `e2xgrader-0.3.0.dev2/e2xgrader/exporters/submissionexporter.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/exporters/filters/highlight.py` & `e2xgrader-0.3.0.dev2/e2xgrader/exporters/filters/highlight.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/exporters/templates/hashcode_cell.html` & `e2xgrader-0.3.0.dev2/e2xgrader/exporters/templates/hashcode_cell.html`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/extensions/base.py` & `e2xgrader-0.3.0.dev2/e2xgrader/extensions/base.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/extensions/manager.py` & `e2xgrader-0.3.0.dev2/e2xgrader/extensions/manager.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/extensions/nbextensions.py` & `e2xgrader-0.3.0.dev2/e2xgrader/extensions/nbextensions.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/extensions/serverextensions.py` & `e2xgrader-0.3.0.dev2/e2xgrader/extensions/serverextensions.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/extensions/utils.py` & `e2xgrader-0.3.0.dev2/e2xgrader/extensions/utils.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/graders/base.py` & `e2xgrader-0.3.0.dev2/e2xgrader/graders/base.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/graders/code.py` & `e2xgrader-0.3.0.dev2/e2xgrader/graders/code.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/graders/multiplechoice.py` & `e2xgrader-0.3.0.dev2/e2xgrader/graders/multiplechoice.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/graders/singlechoice.py` & `e2xgrader-0.3.0.dev2/e2xgrader/graders/singlechoice.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/preprocessors/__init__.py` & `e2xgrader-0.3.0.dev2/e2xgrader/preprocessors/__init__.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/preprocessors/clearhiddentests.py` & `e2xgrader-0.3.0.dev2/e2xgrader/preprocessors/clearhiddentests.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/preprocessors/clearsolutions.py` & `e2xgrader-0.3.0.dev2/e2xgrader/preprocessors/clearsolutions.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/preprocessors/extractattachments.py` & `e2xgrader-0.3.0.dev2/e2xgrader/preprocessors/extractattachments.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/preprocessors/filtercellsbyid.py` & `e2xgrader-0.3.0.dev2/e2xgrader/preprocessors/filtercellsbyid.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/preprocessors/filtertests.py` & `e2xgrader-0.3.0.dev2/e2xgrader/preprocessors/filtertests.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/preprocessors/overwritecells.py` & `e2xgrader-0.3.0.dev2/e2xgrader/preprocessors/overwritecells.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/preprocessors/permutetasks.py` & `e2xgrader-0.3.0.dev2/e2xgrader/preprocessors/permutetasks.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/preprocessors/saveautogrades.py` & `e2xgrader-0.3.0.dev2/e2xgrader/preprocessors/saveautogrades.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/preprocessors/savecells.py` & `e2xgrader-0.3.0.dev2/e2xgrader/preprocessors/savecells.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/preprocessors/scramble.py` & `e2xgrader-0.3.0.dev2/e2xgrader/preprocessors/scramble.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/preprocessors/unpermutetasks.py` & `e2xgrader-0.3.0.dev2/e2xgrader/preprocessors/unpermutetasks.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/preprocessors/unscramble.py` & `e2xgrader-0.3.0.dev2/e2xgrader/preprocessors/unscramble.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/preprocessors/validateextracells.py` & `e2xgrader-0.3.0.dev2/e2xgrader/preprocessors/validateextracells.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/assignment_list/handlers.py` & `e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/assignment_list/handlers.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/diagram_editor/diagrameditor.py` & `e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/diagram_editor/diagrameditor.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/e2xgraderapi/apihandlers.py` & `e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/e2xgraderapi/apihandlers.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/e2xgraderapi/e2xgraderapi.py` & `e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/e2xgraderapi/e2xgraderapi.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/e2xgraderapi/presets/questions/Code (Autograded).ipynb` & `e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/e2xgraderapi/presets/questions/Code (Autograded).ipynb`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/e2xgraderapi/presets/questions/Code (Manual).ipynb` & `e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/e2xgraderapi/presets/questions/Code (Manual).ipynb`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/e2xgraderapi/presets/questions/Diagram.ipynb` & `e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/e2xgraderapi/presets/questions/Diagram.ipynb`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/e2xgraderapi/presets/questions/Freetext.ipynb` & `e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/e2xgraderapi/presets/questions/Freetext.ipynb`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/e2xgraderapi/presets/questions/Multiple Choice.ipynb` & `e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/e2xgraderapi/presets/questions/Multiple Choice.ipynb`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/e2xgraderapi/presets/questions/Single Choice.ipynb` & `e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/e2xgraderapi/presets/questions/Single Choice.ipynb`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/e2xgraderapi/presets/questions/Upload Files.ipynb` & `e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/e2xgraderapi/presets/questions/Upload Files.ipynb`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/e2xgraderapi/presets/template/Footer.ipynb` & `e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/e2xgraderapi/presets/template/Footer.ipynb`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/e2xgraderapi/presets/template/Group Info.ipynb` & `e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/e2xgraderapi/presets/template/Group Info.ipynb`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/e2xgraderapi/presets/template/Header.ipynb` & `e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/e2xgraderapi/presets/template/Header.ipynb`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/e2xgraderapi/presets/template/Student Info.ipynb` & `e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/e2xgraderapi/presets/template/Student Info.ipynb`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/e2xgraderapi/templates/feedback/index.html.j2` & `e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/e2xgraderapi/templates/feedback/index.html.j2`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/formgrader/formgrader.py` & `e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/formgrader/formgrader.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/formgrader/handlers.py` & `e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/formgrader/handlers.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/formgrader/static/css/eraser-solid.svg` & `e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/formgrader/static/css/eraser-solid.svg`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/formgrader/static/css/pencil-solid.svg` & `e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/formgrader/static/css/pencil-solid.svg`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/formgrader/static/js/formgrade.js` & `e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/formgrader/static/js/formgrade.js`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/formgrader/static/js/formgrade_models.js` & `e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/formgrader/static/js/formgrade_models.js`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/formgrader/static/js/gradebook_assignments.js` & `e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/formgrader/static/js/gradebook_assignments.js`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/formgrader/static/js/gradebook_notebook_submissions.js` & `e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/formgrader/static/js/gradebook_notebook_submissions.js`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/formgrader/static/js/gradebook_notebooks.js` & `e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/formgrader/static/js/gradebook_notebooks.js`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/formgrader/static/js/gradebook_tasks.js` & `e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/formgrader/static/js/gradebook_tasks.js`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/formgrader/static/js/manage_assignments.js` & `e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/formgrader/static/js/manage_assignments.js`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/formgrader/static/js/manage_submissions.js` & `e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/formgrader/static/js/manage_submissions.js`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/formgrader/templates/base.tpl` & `e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/formgrader/templates/base.tpl`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/formgrader/templates/export_grades.tpl` & `e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/formgrader/templates/export_grades.tpl`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/formgrader/templates/manage_assignments.tpl` & `e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/formgrader/templates/manage_assignments.tpl`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/formgrader/templates/manage_submissions.tpl` & `e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/formgrader/templates/manage_submissions.tpl`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/formgrader/templates/formgrade/formgrade_macros.html.j2` & `e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/formgrader/templates/formgrade/formgrade_macros.html.j2`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/formgrader/templates/formgrade/index.html.j2` & `e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/formgrader/templates/formgrade/index.html.j2`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/formgrader/templates/task_view/gradebook_assignments.tpl` & `e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/formgrader/templates/task_view/gradebook_assignments.tpl`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/formgrader/templates/task_view/gradebook_notebook_submissions.tpl` & `e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/formgrader/templates/task_view/gradebook_notebook_submissions.tpl`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/formgrader/templates/task_view/gradebook_notebooks.tpl` & `e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/formgrader/templates/task_view/gradebook_notebooks.tpl`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/formgrader/templates/task_view/gradebook_tasks.tpl` & `e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/formgrader/templates/task_view/gradebook_tasks.tpl`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/help/apihandlers.py` & `e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/help/apihandlers.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/help/help.py` & `e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/help/help.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/nbgraderapi/nbgraderapi.py` & `e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/nbgraderapi/nbgraderapi.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/validate_assignment/handlers.py` & `e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/validate_assignment/handlers.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/apps/validate_assignment/validator.py` & `e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/apps/validate_assignment/validator.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/base/extension.py` & `e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/base/extension.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/student/student.py` & `e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/student/student.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/server_extensions/teacher/teacher.py` & `e2xgrader-0.3.0.dev2/e2xgrader/server_extensions/teacher/teacher.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/static/nbextensions/notebook/student/main.js` & `e2xgrader-0.3.0.dev2/e2xgrader/static/nbextensions/notebook/student/main.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -2668,15 +2668,17 @@
                                             throw new Error("Mode needs to be either 'command' or 'edit'")
                                         }
 
                                         function Y(t, ...e) {
                                             const n = W(t);
                                             for (const r of e) try {
                                                 n.remove_shortcut(r)
-                                            } catch (t) {}
+                                            } catch (e) {
+                                                console.log("Error removing shortcut", r, "from", t, "mode:", e.message)
+                                            }
                                         }
 
                                         function I(t, e, n, r, o = "zz") {
                                             W(t).add_shortcut(e, {
                                                 help: r,
                                                 help_index: o,
                                                 handler: n
@@ -2690,15 +2692,15 @@
                                                 else {
                                                     let e = this.get_selected_cell();
                                                     t = this.find_cell_index(e), e.execute()
                                                 }
                                                 t = Math.min(t + 1, this.ncells() - 1), this.select(t), this.focus_cell()
                                             };
                                             const t = ["alt-enter", "shift-enter"];
-                                            Y("edit", t), Y("command", t);
+                                            Y("edit", ...t), Y("command", ...t);
                                             const e = "run cell",
                                                 n = function(t) {
                                                     return L().notebook.execute_cell_and_select_below_without_insert(), !1
                                                 };
                                             for (const r of t) I("edit", r, n, e), I("command", r, n, e)
                                         }
                                         var R = o(804);
@@ -2907,35 +2909,37 @@
                                 value: function(t, e, n) {
                                     var r = a()("<button/>").attr("type", "button").attr("id", e).addClass("exam_btn").text(t);
                                     return r.on("click", n), r
                                 }
                             }, {
                                 key: "create_header",
                                 value: function(t, e, n) {
-                                    if (null === e.cell_type) setTimeout((function() {
-                                        this.create_header(t, e, n)
-                                    }), 100);
-                                    else {
+                                    if (null === e.cell_type) {
+                                        var r = this;
+                                        setTimeout((function() {
+                                            r.create_header(t, e, n)
+                                        }), 100)
+                                    } else {
                                         if (!d.utils.is_solution(e)) return this.remove_classes(e), void this.add_hidden(e);
                                         if (this.add_highlight(e), h.utils.is_e2x(e)) return;
                                         if ("code" === e.cell_type) {
-                                            var r = this.create_button("Run", "run", (function() {
+                                            var o = this.create_button("Run", "run", (function() {
                                                 e.execute()
                                             }));
-                                            a()(t).append(a()("<span/>").append(r).addClass("cell_control"))
+                                            a()(t).append(a()("<span/>").append(o).addClass("cell_control"))
                                         } else if ("markdown" === e.cell_type) {
-                                            var o = this.create_button("Edit", "edit", (function() {
+                                            var i = this.create_button("Edit", "edit", (function() {
                                                     e.events.trigger("select.Cell", {
                                                         cell: e
                                                     }), s().notebook.edit_mode(), n.rebuild()
                                                 })),
-                                                i = this.create_button("Preview", "preview", (function() {
+                                                c = this.create_button("Preview", "preview", (function() {
                                                     e.execute(), n.rebuild()
                                                 }));
-                                            a()(t).append(a()("<span/>").append(o).append(i).addClass("cell_control"))
+                                            a()(t).append(a()("<span/>").append(i).append(c).addClass("cell_control"))
                                         }
                                     }
                                 }
                             }]) && function(t, e) {
                                 for (var n = 0; n < e.length; n++) {
                                     var r = e[n];
                                     r.enumerable = r.enumerable || !1, r.configurable = !0, "value" in r && (r.writable = !0), Object.defineProperty(t, r.key, r)
@@ -5764,15 +5768,17 @@
                                             throw new Error("Mode needs to be either 'command' or 'edit'")
                                         }
 
                                         function Y(t, ...e) {
                                             const n = W(t);
                                             for (const r of e) try {
                                                 n.remove_shortcut(r)
-                                            } catch (t) {}
+                                            } catch (e) {
+                                                console.log("Error removing shortcut", r, "from", t, "mode:", e.message)
+                                            }
                                         }
 
                                         function I(t, e, n, r, o = "zz") {
                                             W(t).add_shortcut(e, {
                                                 help: r,
                                                 help_index: o,
                                                 handler: n
@@ -5786,15 +5792,15 @@
                                                 else {
                                                     let e = this.get_selected_cell();
                                                     t = this.find_cell_index(e), e.execute()
                                                 }
                                                 t = Math.min(t + 1, this.ncells() - 1), this.select(t), this.focus_cell()
                                             };
                                             const t = ["alt-enter", "shift-enter"];
-                                            Y("edit", t), Y("command", t);
+                                            Y("edit", ...t), Y("command", ...t);
                                             const e = "run cell",
                                                 n = function(t) {
                                                     return L().notebook.execute_cell_and_select_below_without_insert(), !1
                                                 };
                                             for (const r of t) I("edit", r, n, e), I("command", r, n, e)
                                         }
                                         var R = o(804);
```

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/static/nbextensions/notebook/student_exam/main.js` & `e2xgrader-0.3.0.dev2/e2xgrader/static/nbextensions/notebook/student_exam/main.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,24 +1,24 @@
 /*! For license information please see main.js.LICENSE.txt */
-define(["base/js/namespace", "base/js/events", "base/js/dialog", "jquery", "notebook/js/textcell", "base/js/markdown", "notebook/js/notebook", "underscore", "notebook/js/celltoolbar", "notebook/js/cell", "base/js/utils"], ((e, t, n, r, o, i, a, c, s, l, u) => (() => {
+define(["base/js/namespace", "base/js/events", "base/js/dialog", "jquery", "notebook/js/textcell", "base/js/markdown", "notebook/js/notebook", "underscore", "notebook/js/celltoolbar", "notebook/js/cell", "base/js/utils"], ((e, t, n, r, o, i, a, s, c, l, u) => (() => {
     var d = {
             322: (e, t, n) => {
                 (() => {
                     var t = {
                             492: (e, t, n) => {
                                 "use strict";
                                 n.d(t, {
-                                    Z: () => c
+                                    Z: () => s
                                 });
                                 var r = n(601),
                                     o = n.n(r),
                                     i = n(609),
                                     a = n.n(i)()(o());
                                 a.push([e.id, ".celltoolbar {\n  /* safari fix, we cannot use -webkit-flex on hbox\n    and vbox either or all css get borked\n    cf https://github.com/jupyter/nbgrader/issues/394.\n    manual workaround while #370 is not released. */\n  display: -webkit-flex;\n}\n\n.highlight {\n  background-color: #009ee0;\n  height: 2.5em;\n  display: inline-block;\n}\n\n.minimized {\n  height: 0.5em;\n}\n\n.exam_btn {\n  display: inline-block;\n  height: 95%;\n  margin-top: -1px;\n  /*vertical-align: middle;*/\n  text-align: center;\n  border: none;\n  margin-left: 2px;\n}\n\n.exam_btn:hover {\n  background-color: #fff;\n}\n\n#run.exam_btn {\n  border: none;\n}\n\n#preview.exam_btn {\n  border: none;\n}\n\n.cell_id {\n  padding-left: 1em;\n  color: white;\n  font-weight: bold;\n  font-size: 1.5em;\n}\n\n.cell_control {\n  float: right;\n}\n\n#submitting {\n  position: fixed;\n  top: 0;\n  left: 0;\n  background-color: rgba(1, 1, 1, 0.1);\n  width: 100%;\n  height: 100%;\n}\n\n#submit_spinner {\n  margin-left: 48%;\n  font-size: 3em;\n  margin-top: 15%;\n}\n", ""]);
-                                const c = a
+                                const s = a
                             },
                             609: e => {
                                 "use strict";
                                 e.exports = function(e) {
                                     var t = [];
                                     return t.toString = function() {
                                         return this.map((function(t) {
@@ -28,17 +28,17 @@
                                         })).join("")
                                     }, t.i = function(e, n, r, o, i) {
                                         "string" == typeof e && (e = [
                                             [null, e, void 0]
                                         ]);
                                         var a = {};
                                         if (r)
-                                            for (var c = 0; c < this.length; c++) {
-                                                var s = this[c][0];
-                                                null != s && (a[s] = !0)
+                                            for (var s = 0; s < this.length; s++) {
+                                                var c = this[s][0];
+                                                null != c && (a[c] = !0)
                                             }
                                         for (var l = 0; l < e.length; l++) {
                                             var u = [].concat(e[l]);
                                             r && a[u[0]] || (void 0 !== i && (void 0 === u[5] || (u[1] = "@layer".concat(u[5].length > 0 ? " ".concat(u[5]) : "", " {").concat(u[1], "}")), u[5] = i), n && (u[2] ? (u[1] = "@media ".concat(u[2], " {").concat(u[1], "}"), u[2] = n) : u[2] = n), o && (u[4] ? (u[1] = "@supports (".concat(u[4], ") {").concat(u[1], "}"), u[4] = o) : u[4] = "".concat(o)), t.push(u))
                                         }
                                     }, t
                                 }
@@ -58,34 +58,34 @@
                                         if (t[r].identifier === e) {
                                             n = r;
                                             break
                                         } return n
                                 }
 
                                 function r(e, r) {
-                                    for (var i = {}, a = [], c = 0; c < e.length; c++) {
-                                        var s = e[c],
-                                            l = r.base ? s[0] + r.base : s[0],
+                                    for (var i = {}, a = [], s = 0; s < e.length; s++) {
+                                        var c = e[s],
+                                            l = r.base ? c[0] + r.base : c[0],
                                             u = i[l] || 0,
                                             d = "".concat(l, " ").concat(u);
                                         i[l] = u + 1;
                                         var f = n(d),
-                                            p = {
-                                                css: s[1],
-                                                media: s[2],
-                                                sourceMap: s[3],
-                                                supports: s[4],
-                                                layer: s[5]
+                                            h = {
+                                                css: c[1],
+                                                media: c[2],
+                                                sourceMap: c[3],
+                                                supports: c[4],
+                                                layer: c[5]
                                             };
-                                        if (-1 !== f) t[f].references++, t[f].updater(p);
+                                        if (-1 !== f) t[f].references++, t[f].updater(h);
                                         else {
-                                            var h = o(p, r);
-                                            r.byIndex = c, t.splice(c, 0, {
+                                            var p = o(h, r);
+                                            r.byIndex = s, t.splice(s, 0, {
                                                 identifier: d,
-                                                updater: h,
+                                                updater: p,
                                                 references: 1
                                             })
                                         }
                                         a.push(d)
                                     }
                                     return a
                                 }
@@ -101,22 +101,22 @@
                                         }
                                 }
                                 e.exports = function(e, o) {
                                     var i = r(e = e || [], o = o || {});
                                     return function(e) {
                                         e = e || [];
                                         for (var a = 0; a < i.length; a++) {
-                                            var c = n(i[a]);
-                                            t[c].references--
+                                            var s = n(i[a]);
+                                            t[s].references--
                                         }
-                                        for (var s = r(e, o), l = 0; l < i.length; l++) {
+                                        for (var c = r(e, o), l = 0; l < i.length; l++) {
                                             var u = n(i[l]);
                                             0 === t[u].references && (t[u].updater(), t.splice(u, 1))
                                         }
-                                        i = s
+                                        i = c
                                     }
                                 }
                             },
                             793: e => {
                                 "use strict";
                                 var t = {};
                                 e.exports = function(e, n) {
@@ -297,54 +297,54 @@
                                             cells: () => Ne,
                                             utils: () => e
                                         });
                                         var e = {};
                                         o.r(e), o.d(e, {
                                             create_e2x_metadata: () => u,
                                             get_e2x_cell_type: () => f,
-                                            get_e2x_field: () => p,
+                                            get_e2x_field: () => h,
                                             get_e2x_metadata: () => d,
-                                            is_e2x: () => s,
+                                            is_e2x: () => c,
                                             remove_e2x_metadata: () => l,
-                                            set_e2x_field: () => h
+                                            set_e2x_field: () => p
                                         });
                                         const t = n(86);
                                         var r = o.n(t);
                                         const a = n(761);
-                                        var c = o.n(a);
+                                        var s = o.n(a);
 
-                                        function s(e) {
+                                        function c(e) {
                                             return e.hasOwnProperty("metadata") && e.metadata.hasOwnProperty("extended_cell")
                                         }
 
                                         function l(e) {
-                                            s(e) && (delete e.metadata.extended_cell, e.rendered && (e.unrender(), e.render()))
+                                            c(e) && (delete e.metadata.extended_cell, e.rendered && (e.unrender(), e.render()))
                                         }
 
                                         function u(e, t) {
-                                            s(e) || (e.metadata.extended_cell = {
+                                            c(e) || (e.metadata.extended_cell = {
                                                 type: t
                                             })
                                         }
 
                                         function d(e) {
-                                            return s(e) ? e.metadata.extended_cell : {}
+                                            return c(e) ? e.metadata.extended_cell : {}
                                         }
 
                                         function f(e) {
-                                            return p(e, "type", "")
+                                            return h(e, "type", "")
                                         }
 
-                                        function p(e, t) {
+                                        function h(e, t) {
                                             var n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : {};
-                                            return s(e) && e.metadata.extended_cell[t] || n
+                                            return c(e) && e.metadata.extended_cell[t] || n
                                         }
 
-                                        function h(e, t, n) {
-                                            s(e) && (e.metadata.extended_cell[t] = n)
+                                        function p(e, t, n) {
+                                            c(e) && (e.metadata.extended_cell[t] = n)
                                         }
 
                                         function m(e, t) {
                                             (null == t || t > e.length) && (t = e.length);
                                             for (var n = 0, r = new Array(t); n < t; n++) r[n] = e[n];
                                             return r
                                         }
@@ -355,81 +355,81 @@
                                                 }(this, e), this.cell = t, this.options = n, this.initialize_options()
                                             }
                                             var t, n;
                                             return t = e, (n = [{
                                                 key: "initialize_options",
                                                 value: function() {
                                                     var e = this,
-                                                        t = p(this.cell, "options"),
+                                                        t = h(this.cell, "options"),
                                                         n = [];
                                                     Object.keys(t).forEach((function(t) {
                                                         e.options.hasOwnProperty(t) || n.push(t)
                                                     })), n.forEach((function(e) {
                                                         return delete t[e]
                                                     })), Object.keys(this.options).forEach((function(n) {
                                                         t.hasOwnProperty(n) || (t[n] = e.options[n])
-                                                    })), h(this.cell, "options", t)
+                                                    })), p(this.cell, "options", t)
                                                 }
                                             }, {
                                                 key: "get_option",
                                                 value: function(e) {
-                                                    var t = p(this.cell, "options");
+                                                    var t = h(this.cell, "options");
                                                     return t.hasOwnProperty(e) ? t[e] : this.options[e].value
                                                 }
                                             }, {
                                                 key: "set_option",
                                                 value: function(e, t) {
                                                     console.log("Setting options", e, t);
-                                                    var n = p(this.cell, "options");
-                                                    n[e].value = t, h(this.cell, "options", n)
+                                                    var n = h(this.cell, "options");
+                                                    n[e].value = t, p(this.cell, "options", n)
                                                 }
                                             }, {
                                                 key: "render",
                                                 value: function() {
-                                                    for (var e = this, t = c()("<div/>").addClass("e2x_options"), n = function() {
+                                                    for (var e = this, t = s()("<div/>").addClass("e2x_options"), n = function() {
                                                             var n, i = function(e) {
                                                                     if (Array.isArray(e)) return e
                                                                 }(n = o[r]) || function(e, t) {
                                                                     var n = null == e ? null : "undefined" != typeof Symbol && e[Symbol.iterator] || e["@@iterator"];
                                                                     if (null != n) {
                                                                         var r, o, i = [],
                                                                             a = !0,
-                                                                            c = !1;
+                                                                            s = !1;
                                                                         try {
                                                                             for (n = n.call(e); !(a = (r = n.next()).done) && (i.push(r.value), 2 !== i.length); a = !0);
                                                                         } catch (e) {
-                                                                            c = !0, o = e
+                                                                            s = !0, o = e
                                                                         } finally {
                                                                             try {
                                                                                 a || null == n.return || n.return()
                                                                             } finally {
-                                                                                if (c) throw o
+                                                                                if (s) throw o
                                                                             }
                                                                         }
                                                                         return i
                                                                     }
                                                                 }(n) || function(e, t) {
                                                                     if (e) {
                                                                         if ("string" == typeof e) return m(e, 2);
                                                                         var n = Object.prototype.toString.call(e).slice(8, -1);
                                                                         return "Object" === n && e.constructor && (n = e.constructor.name), "Map" === n || "Set" === n ? Array.from(e) : "Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n) ? m(e, 2) : void 0
                                                                     }
                                                                 }(n) || function() {
                                                                     throw new TypeError("Invalid attempt to destructure non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
                                                                 }(),
                                                                 a = i[0],
-                                                                s = i[1];
-                                                            if ("checkbox" == s.type) {
-                                                                var l = c()("<div/>"),
-                                                                    u = c()("<input/>").attr("type", s.type);
-                                                                l.append(u), l.append(c()("<span/>").text(s.text)), s.value && u.attr("checked", "checked"), u.on("change", (function() {
+                                                                c = i[1];
+                                                            if ("checkbox" == c.type) {
+                                                                var l = s()("<div/>"),
+                                                                    u = s()("<input/>").attr("type", c.type);
+                                                                l.append(u), l.append(s()("<span/>").text(c.text)), c.value && u.attr("checked", "checked"), u.on("change", (function() {
                                                                     e.set_option(a, !!this.checked)
                                                                 })), t.append(l)
                                                             }
-                                                        }, r = 0, o = Object.entries(p(this.cell, "options")); r < o.length; r++) n();
+                                                        }, r = 0, o = Object.entries(h(this.cell, "options")); r < o.length; r++) n();
                                                     return t
                                                 }
                                             }]) && function(e, t) {
                                                 for (var n = 0; n < t.length; n++) {
                                                     var r = t[n];
                                                     r.enumerable = r.enumerable || !1, r.configurable = !0, "value" in r && (r.writable = !0), Object.defineProperty(e, r.key, r)
                                                 }
@@ -458,18 +458,18 @@
                                                     this.cell.render()
                                                 }
                                             }, {
                                                 key: "render_grader_settings",
                                                 value: function() {
                                                     if (this.edit_mode) {
                                                         var e = this,
-                                                            t = c()(this.cell.element).find(".rendered_html");
+                                                            t = s()(this.cell.element).find(".rendered_html");
                                                         t.find(".e2x_grader_options").remove();
-                                                        var n = c()("<div/>").addClass("e2x_grader_options");
-                                                        n.append(c()("<hr/>")), n.append(this.option_dict.render()), n.append(c()("<button/>").attr("type", "button").addClass("e2x_unrender").on("click", (function() {
+                                                        var n = s()("<div/>").addClass("e2x_grader_options");
+                                                        n.append(s()("<hr/>")), n.append(this.option_dict.render()), n.append(s()("<button/>").attr("type", "button").addClass("e2x_unrender").on("click", (function() {
                                                             e.cell.unrender_force(), e.cell.keyboard_manager.enable()
                                                         })).append("Edit cell")), t.append(n)
                                                     }
                                                 }
                                             }]) && function(e, t) {
                                                 for (var n = 0; n < t.length; n++) {
                                                     var r = t[n];
@@ -566,20 +566,20 @@
                                                 function n(e, r) {
                                                     var o;
                                                     return _(this, n), (o = t.call(this, e, r)).choice_field = "choice", o
                                                 }
                                                 return k(n, [{
                                                     key: "set_choice",
                                                     value: function(e) {
-                                                        h(this.cell, this.choice_field, e)
+                                                        p(this.cell, this.choice_field, e)
                                                     }
                                                 }, {
                                                     key: "get_choices",
                                                     value: function() {
-                                                        return p(this.cell, this.choice_field, [])
+                                                        return h(this.cell, this.choice_field, [])
                                                     }
                                                 }]), n
                                             }(g),
                                             A = function(e) {
                                                 x(n, e);
                                                 var t = E(n);
 
@@ -600,19 +600,19 @@
                                                             t = this.get_choices(),
                                                             n = this;
                                                         if (e.length > 0) {
                                                             var o = e[0],
                                                                 i = $("<form>").addClass("hbrs_radio"),
                                                                 a = $(o).find("li");
                                                             t.length > 0 && t[0] >= a.length && (this.get_metadata()[this.choice_field] = [], t = this.get_choices());
-                                                            for (var c = 0; c < a.length; c++) {
-                                                                var s = this.create_radio_button("my_radio", c, t.indexOf(c.toString()) >= 0, (function() {
+                                                            for (var s = 0; s < a.length; s++) {
+                                                                var c = this.create_radio_button("my_radio", s, t.indexOf(s.toString()) >= 0, (function() {
                                                                     n.set_choice(this.value)
                                                                 }));
-                                                                r().keyboard_manager.register_events(s), i.append($("<div>").append(s).append("&nbsp;&nbsp;").append(a[c].childNodes))
+                                                                r().keyboard_manager.register_events(c), i.append($("<div>").append(c).append("&nbsp;&nbsp;").append(a[s].childNodes))
                                                             }
                                                             $(o).replaceWith(i)
                                                         }
                                                         this.render_grader_settings()
                                                     }
                                                 }]), n
                                             }(C),
@@ -623,20 +623,20 @@
                                                 function n(e) {
                                                     var r;
                                                     return _(this, n), (r = t.call(this, e, "multiplechoice")).choice_count_field = "num_of_choices", r
                                                 }
                                                 return k(n, [{
                                                     key: "get_number_of_choices",
                                                     value: function() {
-                                                        return p(this.cell, this.choice_count_field, [])
+                                                        return h(this.cell, this.choice_count_field, [])
                                                     }
                                                 }, {
                                                     key: "set_number_of_choices",
                                                     value: function(e) {
-                                                        h(this.cell, this.choice_count_field, e)
+                                                        p(this.cell, this.choice_count_field, e)
                                                     }
                                                 }, {
                                                     key: "add_choice",
                                                     value: function(e) {
                                                         var t = this.get_choices();
                                                         t.indexOf(e) > -1 || (t.push(e), this.set_choice(t))
                                                     }
@@ -663,18 +663,18 @@
                                                         var e = $(this.cell.element).find(".rendered_html").find("ul");
                                                         if (e.length > 0) {
                                                             var t = e[0],
                                                                 n = $("<form>").addClass("hbrs_checkbox"),
                                                                 o = $(t).find("li");
                                                             this.get_number_of_choices() != o.length && (this.set_number_of_choices(o.length), this.get_metadata()[this.choice_field] = []);
                                                             for (var i = this.get_choices(), a = 0; a < o.length; a++) {
-                                                                var c = this.create_checkbox("my_checkbox", a, i.indexOf(a.toString()) >= 0);
-                                                                r().keyboard_manager.register_events(c);
-                                                                var s = $("<div>").append(c).append("&nbsp;&nbsp;").append(o[a].childNodes);
-                                                                n.append(s)
+                                                                var s = this.create_checkbox("my_checkbox", a, i.indexOf(a.toString()) >= 0);
+                                                                r().keyboard_manager.register_events(s);
+                                                                var c = $("<div>").append(s).append("&nbsp;&nbsp;").append(o[a].childNodes);
+                                                                n.append(c)
                                                             }
                                                             $(t).replaceWith(n)
                                                         }
                                                         this.render_grader_settings()
                                                     }
                                                 }]), n
                                             }(C);
@@ -936,31 +936,31 @@
                                                 t = Object.prototype,
                                                 n = t.hasOwnProperty,
                                                 r = "function" == typeof Symbol ? Symbol : {},
                                                 o = r.iterator || "@@iterator",
                                                 i = r.asyncIterator || "@@asyncIterator",
                                                 a = r.toStringTag || "@@toStringTag";
 
-                                            function c(e, t, n) {
+                                            function s(e, t, n) {
                                                 return Object.defineProperty(e, t, {
                                                     value: n,
                                                     enumerable: !0,
                                                     configurable: !0,
                                                     writable: !0
                                                 }), e[t]
                                             }
                                             try {
-                                                c({}, "")
+                                                s({}, "")
                                             } catch (e) {
-                                                c = function(e, t, n) {
+                                                s = function(e, t, n) {
                                                     return e[t] = n
                                                 }
                                             }
 
-                                            function s(e, t, n, r) {
+                                            function c(e, t, n, r) {
                                                 var o = t && t.prototype instanceof d ? t : d,
                                                     i = Object.create(o.prototype),
                                                     a = new x(r || []);
                                                 return i._invoke = function(e, t, n) {
                                                     var r = "suspendedStart";
                                                     return function(o, i) {
                                                         if ("executing" === r) throw new Error("Generator is already running");
@@ -970,35 +970,35 @@
                                                                 value: void 0,
                                                                 done: !0
                                                             }
                                                         }
                                                         for (n.method = o, n.arg = i;;) {
                                                             var a = n.delegate;
                                                             if (a) {
-                                                                var c = _(a, n);
-                                                                if (c) {
-                                                                    if (c === u) continue;
-                                                                    return c
+                                                                var s = _(a, n);
+                                                                if (s) {
+                                                                    if (s === u) continue;
+                                                                    return s
                                                                 }
                                                             }
                                                             if ("next" === n.method) n.sent = n._sent = n.arg;
                                                             else if ("throw" === n.method) {
                                                                 if ("suspendedStart" === r) throw r = "completed", n.arg;
                                                                 n.dispatchException(n.arg)
                                                             } else "return" === n.method && n.abrupt("return", n.arg);
                                                             r = "executing";
-                                                            var s = l(e, t, n);
-                                                            if ("normal" === s.type) {
-                                                                if (r = n.done ? "completed" : "suspendedYield", s.arg === u) continue;
+                                                            var c = l(e, t, n);
+                                                            if ("normal" === c.type) {
+                                                                if (r = n.done ? "completed" : "suspendedYield", c.arg === u) continue;
                                                                 return {
-                                                                    value: s.arg,
+                                                                    value: c.arg,
                                                                     done: n.done
                                                                 }
                                                             }
-                                                            "throw" === s.type && (r = "completed", n.method = "throw", n.arg = s.arg)
+                                                            "throw" === c.type && (r = "completed", n.method = "throw", n.arg = c.arg)
                                                         }
                                                     }
                                                 }(e, n, a), i
                                             }
 
                                             function l(e, t, n) {
                                                 try {
@@ -1009,56 +1009,56 @@
                                                 } catch (e) {
                                                     return {
                                                         type: "throw",
                                                         arg: e
                                                     }
                                                 }
                                             }
-                                            e.wrap = s;
+                                            e.wrap = c;
                                             var u = {};
 
                                             function d() {}
 
                                             function f() {}
 
-                                            function p() {}
-                                            var h = {};
-                                            c(h, o, (function() {
+                                            function h() {}
+                                            var p = {};
+                                            s(p, o, (function() {
                                                 return this
                                             }));
                                             var m = Object.getPrototypeOf,
                                                 y = m && m(m(O([])));
-                                            y && y !== t && n.call(y, o) && (h = y);
-                                            var v = p.prototype = d.prototype = Object.create(h);
+                                            y && y !== t && n.call(y, o) && (p = y);
+                                            var v = h.prototype = d.prototype = Object.create(p);
 
                                             function g(e) {
                                                 ["next", "throw", "return"].forEach((function(t) {
-                                                    c(e, t, (function(e) {
+                                                    s(e, t, (function(e) {
                                                         return this._invoke(t, e)
                                                     }))
                                                 }))
                                             }
 
                                             function b(e, t) {
-                                                function r(o, i, a, c) {
-                                                    var s = l(e[o], e, i);
-                                                    if ("throw" !== s.type) {
-                                                        var u = s.arg,
+                                                function r(o, i, a, s) {
+                                                    var c = l(e[o], e, i);
+                                                    if ("throw" !== c.type) {
+                                                        var u = c.arg,
                                                             d = u.value;
                                                         return d && "object" == U(d) && n.call(d, "__await") ? t.resolve(d.__await).then((function(e) {
-                                                            r("next", e, a, c)
+                                                            r("next", e, a, s)
                                                         }), (function(e) {
-                                                            r("throw", e, a, c)
+                                                            r("throw", e, a, s)
                                                         })) : t.resolve(d).then((function(e) {
                                                             u.value = e, a(u)
                                                         }), (function(e) {
-                                                            return r("throw", e, a, c)
+                                                            return r("throw", e, a, s)
                                                         }))
                                                     }
-                                                    c(s.arg)
+                                                    s(c.arg)
                                                 }
                                                 var o;
                                                 this._invoke = function(e, n) {
                                                     function i() {
                                                         return new t((function(t, o) {
                                                             r(e, n, t, o)
                                                         }))
@@ -1122,34 +1122,34 @@
 
                                             function E() {
                                                 return {
                                                     value: void 0,
                                                     done: !0
                                                 }
                                             }
-                                            return f.prototype = p, c(v, "constructor", p), c(p, "constructor", f), f.displayName = c(p, a, "GeneratorFunction"), e.isGeneratorFunction = function(e) {
+                                            return f.prototype = h, s(v, "constructor", h), s(h, "constructor", f), f.displayName = s(h, a, "GeneratorFunction"), e.isGeneratorFunction = function(e) {
                                                 var t = "function" == typeof e && e.constructor;
                                                 return !!t && (t === f || "GeneratorFunction" === (t.displayName || t.name))
                                             }, e.mark = function(e) {
-                                                return Object.setPrototypeOf ? Object.setPrototypeOf(e, p) : (e.__proto__ = p, c(e, a, "GeneratorFunction")), e.prototype = Object.create(v), e
+                                                return Object.setPrototypeOf ? Object.setPrototypeOf(e, h) : (e.__proto__ = h, s(e, a, "GeneratorFunction")), e.prototype = Object.create(v), e
                                             }, e.awrap = function(e) {
                                                 return {
                                                     __await: e
                                                 }
-                                            }, g(b.prototype), c(b.prototype, i, (function() {
+                                            }, g(b.prototype), s(b.prototype, i, (function() {
                                                 return this
                                             })), e.AsyncIterator = b, e.async = function(t, n, r, o, i) {
                                                 void 0 === i && (i = Promise);
-                                                var a = new b(s(t, n, r, o), i);
+                                                var a = new b(c(t, n, r, o), i);
                                                 return e.isGeneratorFunction(n) ? a : a.next().then((function(e) {
                                                     return e.done ? e.value : a.next()
                                                 }))
-                                            }, g(v), c(v, a, "Generator"), c(v, o, (function() {
+                                            }, g(v), s(v, a, "Generator"), s(v, o, (function() {
                                                 return this
-                                            })), c(v, "toString", (function() {
+                                            })), s(v, "toString", (function() {
                                                 return "[object Generator]"
                                             })), e.keys = function(e) {
                                                 var t = [];
                                                 for (var n in e) t.push(n);
                                                 return t.reverse(),
                                                     function n() {
                                                         for (; t.length;) {
@@ -1178,23 +1178,23 @@
                                                         return a.type = "throw", a.arg = e, t.next = n, r && (t.method = "next", t.arg = void 0), !!r
                                                     }
                                                     for (var o = this.tryEntries.length - 1; o >= 0; --o) {
                                                         var i = this.tryEntries[o],
                                                             a = i.completion;
                                                         if ("root" === i.tryLoc) return r("end");
                                                         if (i.tryLoc <= this.prev) {
-                                                            var c = n.call(i, "catchLoc"),
-                                                                s = n.call(i, "finallyLoc");
-                                                            if (c && s) {
+                                                            var s = n.call(i, "catchLoc"),
+                                                                c = n.call(i, "finallyLoc");
+                                                            if (s && c) {
                                                                 if (this.prev < i.catchLoc) return r(i.catchLoc, !0);
                                                                 if (this.prev < i.finallyLoc) return r(i.finallyLoc)
-                                                            } else if (c) {
+                                                            } else if (s) {
                                                                 if (this.prev < i.catchLoc) return r(i.catchLoc, !0)
                                                             } else {
-                                                                if (!s) throw new Error("try statement without catch or finally");
+                                                                if (!c) throw new Error("try statement without catch or finally");
                                                                 if (this.prev < i.finallyLoc) return r(i.finallyLoc)
                                                             }
                                                         }
                                                     }
                                                 },
                                                 abrupt: function(e, t) {
                                                     for (var r = this.tryEntries.length - 1; r >= 0; --r) {
@@ -1283,35 +1283,35 @@
                                                 var r = t[n];
                                                 r.enumerable = r.enumerable || !1, r.configurable = !0, "value" in r && (r.writable = !0), Object.defineProperty(e, r.key, r)
                                             }
                                         }
 
                                         function X(e, t, n, r, o, i, a) {
                                             try {
-                                                var c = e[i](a),
-                                                    s = c.value
+                                                var s = e[i](a),
+                                                    c = s.value
                                             } catch (e) {
                                                 return void n(e)
                                             }
-                                            c.done ? t(s) : Promise.resolve(s).then(r, o)
+                                            s.done ? t(c) : Promise.resolve(c).then(r, o)
                                         }
 
                                         function ee(e) {
                                             return function() {
                                                 var t = this,
                                                     n = arguments;
                                                 return new Promise((function(r, o) {
                                                     var i = e.apply(t, n);
 
                                                     function a(e) {
-                                                        X(i, r, o, a, c, "next", e)
+                                                        X(i, r, o, a, s, "next", e)
                                                     }
 
-                                                    function c(e) {
-                                                        X(i, r, o, a, c, "throw", e)
+                                                    function s(e) {
+                                                        X(i, r, o, a, s, "throw", e)
                                                     }
                                                     a(void 0)
                                                 }))
                                             }
                                         }
                                         var te = !1,
                                             ne = {};
@@ -1342,18 +1342,18 @@
                                                 }), e, null, [
                                                     [1, 8]
                                                 ])
                                             })))).apply(this, arguments)
                                         }
                                         const ie = function() {
                                             function e(t, n, r, o, i, a) {
-                                                var c = arguments.length > 6 && void 0 !== arguments[6] ? arguments[6] : {};
+                                                var s = arguments.length > 6 && void 0 !== arguments[6] ? arguments[6] : {};
                                                 K(this, e), this.config = null, this.ui = "min", this.xml = null, this.format = "xml", this.libraries = !0, this.frameStyle = "position:absolute;bottom:0;border:0;width:100%;height:100%;";
-                                                var s = H(H({}, ne), c);
-                                                this.config = t || this.config, this.ui = n || this.ui, this.done = r || function() {}, this.initialized = o || function() {}, this.urlParams = i, this.cell = a, this.handleMessageEvent = this.handleMessageEvent.bind(this), this.frame = null, this.startElement = null, this.format = "xml", this.xml = null, this.drawDomain = s.drawDomain || "https://embed.diagrams.net/", this.origin = s.drawOrigin || "https://embed.diagrams.net/", this.frameStyle = "position:absolute;bottom:0;border:0;width:100%;height:100%;", this.libs = s.libs || []
+                                                var c = H(H({}, ne), s);
+                                                this.config = t || this.config, this.ui = n || this.ui, this.done = r || function() {}, this.initialized = o || function() {}, this.urlParams = i, this.cell = a, this.handleMessageEvent = this.handleMessageEvent.bind(this), this.frame = null, this.startElement = null, this.format = "xml", this.xml = null, this.drawDomain = c.drawDomain || "https://embed.diagrams.net/", this.origin = c.drawOrigin || "https://embed.diagrams.net/", this.frameStyle = "position:absolute;bottom:0;border:0;width:100%;height:100%;", this.libs = c.libs || []
                                             }
                                             var t, n, r, o;
                                             return t = e, n = [{
                                                 key: "handleMessageEvent",
                                                 value: function(e) {
                                                     var t = new URL(this.origin),
                                                         n = new URL(e.origin);
@@ -1491,29 +1491,29 @@
                                                 key: "save",
                                                 value: function(e, t, n) {
                                                     this.done(e, t, n)
                                                 }
                                             }], r = [{
                                                 key: "editElement",
                                                 value: function(t, n, r, o, i, a) {
-                                                    var c = arguments.length > 6 && void 0 !== arguments[6] ? arguments[6] : {};
+                                                    var s = arguments.length > 6 && void 0 !== arguments[6] ? arguments[6] : {};
                                                     if (!n.diagramEditorStarting) return n.diagramEditorStarting = !0, new e(r, o, i, (function() {
                                                         delete n.diagramEditorStarting
-                                                    }), a, t, c).editElement(n)
+                                                    }), a, t, s).editElement(n)
                                                 }
                                             }, {
                                                 key: "editDiagram",
                                                 value: (o = ee(F().mark((function e(t, n, r, o, i, a) {
-                                                    var c, s = this,
+                                                    var s, c = this,
                                                         l = arguments;
                                                     return F().wrap((function(e) {
                                                         for (;;) switch (e.prev = e.next) {
                                                             case 0:
-                                                                c = l.length > 6 && void 0 !== l[6] ? l[6] : {}, re().then((function() {
-                                                                    return s.editElement(t, n, r, o, i, a, c)
+                                                                s = l.length > 6 && void 0 !== l[6] ? l[6] : {}, re().then((function() {
+                                                                    return c.editElement(t, n, r, o, i, a, s)
                                                                 }));
                                                             case 2:
                                                             case "end":
                                                                 return e.stop()
                                                         }
                                                     }), e)
                                                 }))), function(e, t, n, r, i, a) {
@@ -1528,43 +1528,43 @@
                                             return ae = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
                                                 return typeof e
                                             } : function(e) {
                                                 return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
                                             }, ae(e)
                                         }
 
-                                        function ce() {
-                                            ce = function() {
+                                        function se() {
+                                            se = function() {
                                                 return e
                                             };
                                             var e = {},
                                                 t = Object.prototype,
                                                 n = t.hasOwnProperty,
                                                 r = "function" == typeof Symbol ? Symbol : {},
                                                 o = r.iterator || "@@iterator",
                                                 i = r.asyncIterator || "@@asyncIterator",
                                                 a = r.toStringTag || "@@toStringTag";
 
-                                            function c(e, t, n) {
+                                            function s(e, t, n) {
                                                 return Object.defineProperty(e, t, {
                                                     value: n,
                                                     enumerable: !0,
                                                     configurable: !0,
                                                     writable: !0
                                                 }), e[t]
                                             }
                                             try {
-                                                c({}, "")
+                                                s({}, "")
                                             } catch (e) {
-                                                c = function(e, t, n) {
+                                                s = function(e, t, n) {
                                                     return e[t] = n
                                                 }
                                             }
 
-                                            function s(e, t, n, r) {
+                                            function c(e, t, n, r) {
                                                 var o = t && t.prototype instanceof d ? t : d,
                                                     i = Object.create(o.prototype),
                                                     a = new x(r || []);
                                                 return i._invoke = function(e, t, n) {
                                                     var r = "suspendedStart";
                                                     return function(o, i) {
                                                         if ("executing" === r) throw new Error("Generator is already running");
@@ -1574,35 +1574,35 @@
                                                                 value: void 0,
                                                                 done: !0
                                                             }
                                                         }
                                                         for (n.method = o, n.arg = i;;) {
                                                             var a = n.delegate;
                                                             if (a) {
-                                                                var c = _(a, n);
-                                                                if (c) {
-                                                                    if (c === u) continue;
-                                                                    return c
+                                                                var s = _(a, n);
+                                                                if (s) {
+                                                                    if (s === u) continue;
+                                                                    return s
                                                                 }
                                                             }
                                                             if ("next" === n.method) n.sent = n._sent = n.arg;
                                                             else if ("throw" === n.method) {
                                                                 if ("suspendedStart" === r) throw r = "completed", n.arg;
                                                                 n.dispatchException(n.arg)
                                                             } else "return" === n.method && n.abrupt("return", n.arg);
                                                             r = "executing";
-                                                            var s = l(e, t, n);
-                                                            if ("normal" === s.type) {
-                                                                if (r = n.done ? "completed" : "suspendedYield", s.arg === u) continue;
+                                                            var c = l(e, t, n);
+                                                            if ("normal" === c.type) {
+                                                                if (r = n.done ? "completed" : "suspendedYield", c.arg === u) continue;
                                                                 return {
-                                                                    value: s.arg,
+                                                                    value: c.arg,
                                                                     done: n.done
                                                                 }
                                                             }
-                                                            "throw" === s.type && (r = "completed", n.method = "throw", n.arg = s.arg)
+                                                            "throw" === c.type && (r = "completed", n.method = "throw", n.arg = c.arg)
                                                         }
                                                     }
                                                 }(e, n, a), i
                                             }
 
                                             function l(e, t, n) {
                                                 try {
@@ -1613,56 +1613,56 @@
                                                 } catch (e) {
                                                     return {
                                                         type: "throw",
                                                         arg: e
                                                     }
                                                 }
                                             }
-                                            e.wrap = s;
+                                            e.wrap = c;
                                             var u = {};
 
                                             function d() {}
 
                                             function f() {}
 
-                                            function p() {}
-                                            var h = {};
-                                            c(h, o, (function() {
+                                            function h() {}
+                                            var p = {};
+                                            s(p, o, (function() {
                                                 return this
                                             }));
                                             var m = Object.getPrototypeOf,
                                                 y = m && m(m(O([])));
-                                            y && y !== t && n.call(y, o) && (h = y);
-                                            var v = p.prototype = d.prototype = Object.create(h);
+                                            y && y !== t && n.call(y, o) && (p = y);
+                                            var v = h.prototype = d.prototype = Object.create(p);
 
                                             function g(e) {
                                                 ["next", "throw", "return"].forEach((function(t) {
-                                                    c(e, t, (function(e) {
+                                                    s(e, t, (function(e) {
                                                         return this._invoke(t, e)
                                                     }))
                                                 }))
                                             }
 
                                             function b(e, t) {
-                                                function r(o, i, a, c) {
-                                                    var s = l(e[o], e, i);
-                                                    if ("throw" !== s.type) {
-                                                        var u = s.arg,
+                                                function r(o, i, a, s) {
+                                                    var c = l(e[o], e, i);
+                                                    if ("throw" !== c.type) {
+                                                        var u = c.arg,
                                                             d = u.value;
                                                         return d && "object" == ae(d) && n.call(d, "__await") ? t.resolve(d.__await).then((function(e) {
-                                                            r("next", e, a, c)
+                                                            r("next", e, a, s)
                                                         }), (function(e) {
-                                                            r("throw", e, a, c)
+                                                            r("throw", e, a, s)
                                                         })) : t.resolve(d).then((function(e) {
                                                             u.value = e, a(u)
                                                         }), (function(e) {
-                                                            return r("throw", e, a, c)
+                                                            return r("throw", e, a, s)
                                                         }))
                                                     }
-                                                    c(s.arg)
+                                                    s(c.arg)
                                                 }
                                                 var o;
                                                 this._invoke = function(e, n) {
                                                     function i() {
                                                         return new t((function(t, o) {
                                                             r(e, n, t, o)
                                                         }))
@@ -1726,34 +1726,34 @@
 
                                             function E() {
                                                 return {
                                                     value: void 0,
                                                     done: !0
                                                 }
                                             }
-                                            return f.prototype = p, c(v, "constructor", p), c(p, "constructor", f), f.displayName = c(p, a, "GeneratorFunction"), e.isGeneratorFunction = function(e) {
+                                            return f.prototype = h, s(v, "constructor", h), s(h, "constructor", f), f.displayName = s(h, a, "GeneratorFunction"), e.isGeneratorFunction = function(e) {
                                                 var t = "function" == typeof e && e.constructor;
                                                 return !!t && (t === f || "GeneratorFunction" === (t.displayName || t.name))
                                             }, e.mark = function(e) {
-                                                return Object.setPrototypeOf ? Object.setPrototypeOf(e, p) : (e.__proto__ = p, c(e, a, "GeneratorFunction")), e.prototype = Object.create(v), e
+                                                return Object.setPrototypeOf ? Object.setPrototypeOf(e, h) : (e.__proto__ = h, s(e, a, "GeneratorFunction")), e.prototype = Object.create(v), e
                                             }, e.awrap = function(e) {
                                                 return {
                                                     __await: e
                                                 }
-                                            }, g(b.prototype), c(b.prototype, i, (function() {
+                                            }, g(b.prototype), s(b.prototype, i, (function() {
                                                 return this
                                             })), e.AsyncIterator = b, e.async = function(t, n, r, o, i) {
                                                 void 0 === i && (i = Promise);
-                                                var a = new b(s(t, n, r, o), i);
+                                                var a = new b(c(t, n, r, o), i);
                                                 return e.isGeneratorFunction(n) ? a : a.next().then((function(e) {
                                                     return e.done ? e.value : a.next()
                                                 }))
-                                            }, g(v), c(v, a, "Generator"), c(v, o, (function() {
+                                            }, g(v), s(v, a, "Generator"), s(v, o, (function() {
                                                 return this
-                                            })), c(v, "toString", (function() {
+                                            })), s(v, "toString", (function() {
                                                 return "[object Generator]"
                                             })), e.keys = function(e) {
                                                 var t = [];
                                                 for (var n in e) t.push(n);
                                                 return t.reverse(),
                                                     function n() {
                                                         for (; t.length;) {
@@ -1782,23 +1782,23 @@
                                                         return a.type = "throw", a.arg = e, t.next = n, r && (t.method = "next", t.arg = void 0), !!r
                                                     }
                                                     for (var o = this.tryEntries.length - 1; o >= 0; --o) {
                                                         var i = this.tryEntries[o],
                                                             a = i.completion;
                                                         if ("root" === i.tryLoc) return r("end");
                                                         if (i.tryLoc <= this.prev) {
-                                                            var c = n.call(i, "catchLoc"),
-                                                                s = n.call(i, "finallyLoc");
-                                                            if (c && s) {
+                                                            var s = n.call(i, "catchLoc"),
+                                                                c = n.call(i, "finallyLoc");
+                                                            if (s && c) {
                                                                 if (this.prev < i.catchLoc) return r(i.catchLoc, !0);
                                                                 if (this.prev < i.finallyLoc) return r(i.finallyLoc)
-                                                            } else if (c) {
+                                                            } else if (s) {
                                                                 if (this.prev < i.catchLoc) return r(i.catchLoc, !0)
                                                             } else {
-                                                                if (!s) throw new Error("try statement without catch or finally");
+                                                                if (!c) throw new Error("try statement without catch or finally");
                                                                 if (this.prev < i.finallyLoc) return r(i.finallyLoc)
                                                             }
                                                         }
                                                     }
                                                 },
                                                 abrupt: function(e, t) {
                                                     for (var r = this.tryEntries.length - 1; r >= 0; --r) {
@@ -1842,22 +1842,22 @@
                                                         resultName: t,
                                                         nextLoc: n
                                                     }, "next" === this.method && (this.arg = void 0), u
                                                 }
                                             }, e
                                         }
 
-                                        function se(e, t, n, r, o, i, a) {
+                                        function ce(e, t, n, r, o, i, a) {
                                             try {
-                                                var c = e[i](a),
-                                                    s = c.value
+                                                var s = e[i](a),
+                                                    c = s.value
                                             } catch (e) {
                                                 return void n(e)
                                             }
-                                            c.done ? t(s) : Promise.resolve(s).then(r, o)
+                                            s.done ? t(c) : Promise.resolve(c).then(r, o)
                                         }
 
                                         function le(e, t) {
                                             if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
                                         }
 
                                         function ue(e, t) {
@@ -1879,24 +1879,24 @@
                                                 constructor: {
                                                     value: e,
                                                     writable: !0,
                                                     configurable: !0
                                                 }
                                             }), Object.defineProperty(e, "prototype", {
                                                 writable: !1
-                                            }), t && pe(e, t)
+                                            }), t && he(e, t)
                                         }
 
-                                        function pe(e, t) {
-                                            return pe = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(e, t) {
+                                        function he(e, t) {
+                                            return he = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(e, t) {
                                                 return e.__proto__ = t, e
-                                            }, pe(e, t)
+                                            }, he(e, t)
                                         }
 
-                                        function he(e) {
+                                        function pe(e) {
                                             var t = function() {
                                                 if ("undefined" == typeof Reflect || !Reflect.construct) return !1;
                                                 if (Reflect.construct.sham) return !1;
                                                 if ("function" == typeof Proxy) return !0;
                                                 try {
                                                     return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], (function() {}))), !0
                                                 } catch (e) {
@@ -1925,29 +1925,29 @@
                                         function ye(e) {
                                             return ye = Object.setPrototypeOf ? Object.getPrototypeOf.bind() : function(e) {
                                                 return e.__proto__ || Object.getPrototypeOf(e)
                                             }, ye(e)
                                         }
                                         var ve = function(e) {
                                                 fe(n, e);
-                                                var t = he(n);
+                                                var t = pe(n);
 
                                                 function n() {
                                                     return le(this, n), t.apply(this, arguments)
                                                 }
                                                 return de(n, [{
                                                     key: "postSaveHook",
                                                     value: function() {
                                                         this.cell.unrender_force(), this.cell.render()
                                                     }
                                                 }]), n
                                             }(R),
                                             ge = function(e) {
                                                 fe(n, e);
-                                                var t = he(n);
+                                                var t = pe(n);
 
                                                 function n(e) {
                                                     var r;
                                                     return le(this, n), (r = t.call(this, e, "diagram", {
                                                         replace_diagram: {
                                                             type: "checkbox",
                                                             text: "Replace this diagram with an empty diagram in the student version",
@@ -1973,25 +1973,25 @@
                                                             return function() {
                                                                 var t = this,
                                                                     n = arguments;
                                                                 return new Promise((function(r, o) {
                                                                     var i = e.apply(t, n);
 
                                                                     function a(e) {
-                                                                        se(i, r, o, a, c, "next", e)
+                                                                        ce(i, r, o, a, s, "next", e)
                                                                     }
 
-                                                                    function c(e) {
-                                                                        se(i, r, o, a, c, "throw", e)
+                                                                    function s(e) {
+                                                                        ce(i, r, o, a, s, "throw", e)
                                                                     }
                                                                     a(void 0)
                                                                 }))
                                                             }
-                                                        }(ce().mark((function t() {
-                                                            return ce().wrap((function(t) {
+                                                        }(se().mark((function t() {
+                                                            return se().wrap((function(t) {
                                                                 for (;;) switch (t.prev = t.next) {
                                                                     case 0:
                                                                         return t.prev = 0, t.next = 3, ie.editDiagram(e, r[0]);
                                                                     case 3:
                                                                         t.next = 8;
                                                                         break;
                                                                     case 5:
@@ -2082,34 +2082,34 @@
                                                             alert("Could not access webcam!\n" + e)
                                                         }))
                                                     }
                                                 }, {
                                                     key: "openDialog",
                                                     value: function() {
                                                         var e = this,
-                                                            t = c()("<div/>").attr("id", "webcamDiv"),
-                                                            n = c()("<video/>");
+                                                            t = s()("<div/>").attr("id", "webcamDiv"),
+                                                            n = s()("<video/>");
                                                         t.append(n);
-                                                        var r = c()("<div/>").attr("id", "videoControls");
-                                                        r.append(c()("<button/>").attr("id", "takePhoto").on("click", (function() {
-                                                            n[0].paused ? (n[0].play(), c()("#saveImage").attr("disabled", !0), c()("#takePhoto span").text("Take Photo")) : (n[0].pause(), c()("#saveImage").removeAttr("disabled"), c()("#takePhoto span").text("Retry"))
-                                                        })).append(c()("<span/>").text("Take Photo"))), t.append(r), _e().modal({
+                                                        var r = s()("<div/>").attr("id", "videoControls");
+                                                        r.append(s()("<button/>").attr("id", "takePhoto").on("click", (function() {
+                                                            n[0].paused ? (n[0].play(), s()("#saveImage").attr("disabled", !0), s()("#takePhoto span").text("Take Photo")) : (n[0].pause(), s()("#saveImage").removeAttr("disabled"), s()("#takePhoto span").text("Retry"))
+                                                        })).append(s()("<span/>").text("Take Photo"))), t.append(r), _e().modal({
                                                             keyboard_manager: Jupyter.keyboard_manager,
                                                             title: "Take Photo",
                                                             open: function() {
-                                                                c()("#webcamDiv").bind("destroyed", (function() {
+                                                                s()("#webcamDiv").bind("destroyed", (function() {
                                                                     e.close()
                                                                 }))
                                                             },
                                                             body: t,
                                                             buttons: {
                                                                 "Save Image": {
                                                                     id: "saveImage",
                                                                     click: function() {
-                                                                        var t = c()("<canvas/>").attr("width", n[0].videoWidth).attr("height", n[0].videoHeight);
+                                                                        var t = s()("<canvas/>").attr("width", n[0].videoWidth).attr("height", n[0].videoHeight);
                                                                         t[0].getContext("2d").drawImage(n[0], 0, 0, n[0].videoWidth, n[0].videoHeight);
                                                                         var r = t[0].toDataURL("image/png"),
                                                                             o = e.model.getName("webcam", "png");
                                                                         e.model.setAttachment(o, r)
                                                                     }
                                                                 },
                                                                 Cancel: {}
@@ -2154,96 +2154,96 @@
                                                         e = Reflect.construct(r, arguments, o)
                                                     } else e = r.apply(this, arguments);
                                                     return xe(this, e)
                                                 });
 
                                                 function o(e, t) {
                                                     var n;
-                                                    return Se(this, o), (n = r.call(this)).cell = e, n.model = t, n.element = c()("<div/>").addClass("gallery-view"), t.registerObserver(Oe(n)), n
+                                                    return Se(this, o), (n = r.call(this)).cell = e, n.model = t, n.element = s()("<div/>").addClass("gallery-view"), t.registerObserver(Oe(n)), n
                                                 }
                                                 return Ce(o, [{
                                                     key: "notify",
                                                     value: function(e) {
-                                                        "delete" == e.type ? this.element.find(c()("#" + e.id)).remove() : "add" == e.type && this.addThumbnail(this.model.getAttachment(e.key))
+                                                        "delete" == e.type ? this.element.find(s()("#" + e.id)).remove() : "add" == e.type && this.addThumbnail(this.model.getAttachment(e.key))
                                                     }
                                                 }, {
                                                     key: "addThumbnail",
                                                     value: function(e) {
                                                         var t = this,
-                                                            n = c()("<div/>").addClass("gallery-item").attr("id", e.id),
-                                                            r = c()("<div/>").addClass("remove-file-modal").append(c()("<p/>").append("Are you sure you want to delete the file " + e.name + " ?")),
-                                                            o = c()("<i/>").addClass("fa fa-trash");
+                                                            n = s()("<div/>").addClass("gallery-item").attr("id", e.id),
+                                                            r = s()("<div/>").addClass("remove-file-modal").append(s()("<p/>").append("Are you sure you want to delete the file " + e.name + " ?")),
+                                                            o = s()("<i/>").addClass("fa fa-trash");
                                                         o.on("click", (function() {
                                                             _e().modal({
                                                                 body: r,
                                                                 buttons: {
                                                                     Delete: {
                                                                         class: "button-delete",
                                                                         click: function() {
                                                                             return t.model.removeAttachment(e.name)
                                                                         }
                                                                     },
                                                                     Cancel: {}
                                                                 }
                                                             })
                                                         })), n.append(o);
-                                                        var i = c()("<i/>").addClass("fa fa-search-plus").on("click", (function() {
+                                                        var i = s()("<i/>").addClass("fa fa-search-plus").on("click", (function() {
                                                             var t = document.createElement("a");
                                                             t.href = "data:" + e.type + ";base64," + e.data, t.target = "_blank", t.download = e.name, document.body.appendChild(t), t.click(), document.body.removeChild(t)
                                                         }));
                                                         n.append(i);
-                                                        var a = c()("<div/>").addClass("thumbnail"),
-                                                            s = c()("<div/>").addClass("caption");
-                                                        if (s.append(c()("<span/>").text(e.name)), e.type.startsWith("image")) {
+                                                        var a = s()("<div/>").addClass("thumbnail"),
+                                                            c = s()("<div/>").addClass("caption");
+                                                        if (c.append(s()("<span/>").text(e.name)), e.type.startsWith("image")) {
                                                             var l = new Image;
                                                             l.src = "data:" + e.type + ";base64," + e.data, a.append(l)
                                                         }
-                                                        n.append(a).append(s), this.element.append(n)
+                                                        n.append(a).append(c), this.element.append(n)
                                                     }
                                                 }, {
                                                     key: "getControls",
                                                     value: function() {
                                                         var e = this,
-                                                            t = c()("<div/>").addClass("attachment-controls");
-                                                        t.append(c()("<button/>").addClass("btn-e2x").append(c()("<i/>").addClass("fa fa-camera")).append("Webcam").on("click", (function() {
+                                                            t = s()("<div/>").addClass("attachment-controls");
+                                                        t.append(s()("<button/>").addClass("btn-e2x").append(s()("<i/>").addClass("fa fa-camera")).append("Webcam").on("click", (function() {
                                                             return new Pe(e.model).open()
                                                         })));
-                                                        var n = c()("<button/>").addClass("btn-e2x").addClass("upload-btn").append(c()("<i/>").addClass("fa fa-upload")).append("Upload").on("click", (function() {
-                                                            return c()("#upload-attachments")[0].click()
+                                                        var n = s()("<button/>").addClass("btn-e2x").addClass("upload-btn").append(s()("<i/>").addClass("fa fa-upload")).append("Upload").on("click", (function() {
+                                                            return s()("#upload-attachments")[0].click()
                                                         }));
-                                                        return n.append(c()("<input/>").attr("id", "upload-attachments").attr("type", "file").attr("accept", "application/pdf,image/*").attr("multiple", "multiple").on("change", (function() {
+                                                        return n.append(s()("<input/>").attr("id", "upload-attachments").attr("type", "file").attr("accept", "application/pdf,image/*").attr("multiple", "multiple").on("change", (function() {
                                                             return e.uploadFiles()
                                                         }))), t.append(n), t
                                                     }
                                                 }, {
                                                     key: "uploadFiles",
                                                     value: function() {
-                                                        var e = c()("#upload-attachments")[0],
+                                                        var e = s()("#upload-attachments")[0],
                                                             t = this;
                                                         Array.prototype.forEach.call(e.files, (function(e) {
                                                             var n = new FileReader;
                                                             n.readAsDataURL(e), n.onload = function() {
                                                                 var r = n.result,
                                                                     o = e.name;
                                                                 if (t.model.hasAttachment(o)) {
                                                                     var i = o.split(".")[0],
                                                                         a = o.replace(i + ".", ""),
-                                                                        c = t.model.getName(i, a);
-                                                                    confirm("A file with the name " + o + " already exists!\nDo you want to rename it to " + c + "?") && t.model.setAttachment(c, r)
+                                                                        s = t.model.getName(i, a);
+                                                                    confirm("A file with the name " + o + " already exists!\nDo you want to rename it to " + s + "?") && t.model.setAttachment(s, r)
                                                                 } else t.model.setAttachment(o, r)
                                                             }, n.onerror = function() {
                                                                 console.log(n.error)
                                                             }
                                                         }))
                                                     }
                                                 }, {
                                                     key: "open",
                                                     value: function() {
-                                                        var e = c()("<div/>").addClass("attachment-editor");
-                                                        this.element = c()("<div/>").addClass("gallery-view"), e.append(this.element), e.append(this.getControls());
+                                                        var e = s()("<div/>").addClass("attachment-editor");
+                                                        this.element = s()("<div/>").addClass("gallery-view"), e.append(this.element), e.append(this.getControls());
                                                         var t = this;
                                                         this.model.getAttachments().forEach((function(e) {
                                                             return t.addThumbnail(e)
                                                         })), _e().modal({
                                                             keyboard_manager: Jupyter.keyboard_manager,
                                                             title: "Attachment Editor",
                                                             body: e
@@ -2364,23 +2364,23 @@
                                                         var r;
                                                         return Ge(this, n), (r = t.call(this, e, "attachments")).model = new Ye(e), r.view = new Be(e, r.model), r
                                                     }
                                                     return Ze(n, [{
                                                         key: "get_attachment_button",
                                                         value: function() {
                                                             var e = this;
-                                                            return c()("<button>").attr("type", "button").addClass("edit_attachments btn-e2x").on("click", (function() {
+                                                            return s()("<button>").attr("type", "button").addClass("edit_attachments btn-e2x").on("click", (function() {
                                                                 e.view.open()
                                                             })).append("Add Files / Images")
                                                         }
                                                     }, {
                                                         key: "render",
                                                         value: function() {
                                                             this.cell.render_force();
-                                                            var e = c()(this.cell.element).find(".rendered_html");
+                                                            var e = s()(this.cell.element).find(".rendered_html");
                                                             e.find(".edit_attachments").length < 1 && e.append(this.get_attachment_button()), this.render_grader_settings()
                                                         }
                                                     }]), n
                                                 }(g),
                                                 diagram: ge
                                             }
                                     })(), e.exports = i
@@ -2513,49 +2513,49 @@
                                             is_invalid: () => G,
                                             is_locked: () => x,
                                             is_nbgrader: () => l,
                                             is_solution: () => v,
                                             is_task: () => w,
                                             is_test: () => A,
                                             nbgrader_schema_version: () => a,
-                                            randomString: () => c,
-                                            remove_nbgrader_field: () => h,
+                                            randomString: () => s,
+                                            remove_nbgrader_field: () => p,
                                             remove_nbgrader_metadata: () => u,
                                             set_grade: () => _,
                                             set_grade_id: () => C,
                                             set_locked: () => O,
-                                            set_nbgrader_field: () => p,
+                                            set_nbgrader_field: () => h,
                                             set_points: () => S,
                                             set_schema_version: () => y,
                                             set_solution: () => g,
                                             set_task: () => k,
                                             to_description: () => T,
-                                            to_float: () => s,
+                                            to_float: () => c,
                                             to_test: () => P
                                         });
                                         var t = {};
                                         o.r(t), o.d(t, {
                                             add_shortcut: () => W,
                                             disable_add_cell_on_execute: () => Y,
                                             remove_shortcuts: () => I
                                         });
                                         var r = {};
                                         o.r(r), o.d(r, {
                                             add_username: () => R
                                         });
                                         const a = 3;
 
-                                        function c(e) {
+                                        function s(e) {
                                             let t, n = "",
                                                 r = "abcdef0123456789";
                                             for (t = 0; t < e; t++) n += r[Math.floor(Math.random() * r.length)];
                                             return n
                                         }
 
-                                        function s(e) {
+                                        function c(e) {
                                             return void 0 === e || "" === e ? 0 : parseFloat(e)
                                         }
 
                                         function l(e) {
                                             return e.metadata.hasOwnProperty("nbgrader")
                                         }
 
@@ -2567,76 +2567,76 @@
                                             l(e) || (e.metadata.nbgrader = {})
                                         }
 
                                         function f(e, t, n = {}) {
                                             return l(e) && e.metadata.nbgrader[t] || n
                                         }
 
-                                        function p(e, t, n) {
+                                        function h(e, t, n) {
                                             l(e) || (e.metadata.nbgrader = {}), e.metadata.nbgrader[t] = n
                                         }
 
-                                        function h(e, t) {
+                                        function p(e, t) {
                                             l(e) && e.metadata.nbgrader.hasOwnProperty(t) && delete e.metadata.nbgrader[t]
                                         }
 
                                         function m(e) {
                                             if (l(e)) return void 0 === f(e, "schema_version") ? 0 : f(e, "schema_version")
                                         }
 
                                         function y(e) {
-                                            l(e) || d(e), p(e, "schema_version", a)
+                                            l(e) || d(e), h(e, "schema_version", a)
                                         }
 
                                         function v(e) {
                                             return f(e, "solution", !1)
                                         }
 
                                         function g(e, t) {
-                                            p(e, "solution", t)
+                                            h(e, "solution", t)
                                         }
 
                                         function b(e) {
                                             return f(e, "grade", !1)
                                         }
 
                                         function _(e, t) {
-                                            p(e, "grade", t)
+                                            h(e, "grade", t)
                                         }
 
                                         function w(e) {
                                             return f(e, "task", !1)
                                         }
 
                                         function k(e, t) {
-                                            p(e, "task", t)
+                                            h(e, "task", t)
                                         }
 
                                         function x(e) {
                                             return f(e, "locked", !1)
                                         }
 
                                         function O(e, t) {
-                                            p(e, "locked", t)
+                                            h(e, "locked", t)
                                         }
 
                                         function E(e) {
-                                            return s(f(e, "points", 0))
+                                            return c(f(e, "points", 0))
                                         }
 
                                         function S(e, t) {
-                                            p(e, "points", Math.max(0, s(t)))
+                                            h(e, "points", Math.max(0, c(t)))
                                         }
 
                                         function j(e) {
-                                            return f(e, "grade_id", "cell-" + c(16))
+                                            return f(e, "grade_id", "cell-" + s(16))
                                         }
 
                                         function C(e, t) {
-                                            p(e, "grade_id", t)
+                                            h(e, "grade_id", t)
                                         }
 
                                         function A(e) {
                                             return b(e) && x(e) && !v(e)
                                         }
 
                                         function P(e) {
@@ -2668,15 +2668,17 @@
                                             throw new Error("Mode needs to be either 'command' or 'edit'")
                                         }
 
                                         function I(e, ...t) {
                                             const n = M(e);
                                             for (const r of t) try {
                                                 n.remove_shortcut(r)
-                                            } catch (e) {}
+                                            } catch (t) {
+                                                console.log("Error removing shortcut", r, "from", e, "mode:", t.message)
+                                            }
                                         }
 
                                         function W(e, t, n, r, o = "zz") {
                                             M(e).add_shortcut(t, {
                                                 help: r,
                                                 help_index: o,
                                                 handler: n
@@ -2690,15 +2692,15 @@
                                                 else {
                                                     let t = this.get_selected_cell();
                                                     e = this.find_cell_index(t), t.execute()
                                                 }
                                                 e = Math.min(e + 1, this.ncells() - 1), this.select(e), this.focus_cell()
                                             };
                                             const e = ["alt-enter", "shift-enter"];
-                                            I("edit", e), I("command", e);
+                                            I("edit", ...e), I("command", ...e);
                                             const t = "run cell",
                                                 n = function(e) {
                                                     return J().notebook.execute_cell_and_select_below_without_insert(), !1
                                                 };
                                             for (const r of e) W("edit", r, n, t), W("command", r, n, t)
                                         }
                                         var N = o(804);
@@ -2766,23 +2768,23 @@
                         o.r(i), o.d(i, {
                             AssignmentViewToolbar: () => A
                         });
                         const e = n(75);
                         var t = o.n(e),
                             r = o(761),
                             a = o.n(r),
-                            c = o(86),
-                            s = o.n(c);
+                            s = o(86),
+                            c = o.n(s);
                         const l = n(290);
                         var u = o.n(l);
                         const d = n(600);
                         var f = o(426),
-                            p = o(355),
-                            h = o(62),
-                            m = o.n(h),
+                            h = o(355),
+                            p = o(62),
+                            m = o.n(p),
                             y = o(36),
                             v = o.n(y),
                             g = o(793),
                             b = o.n(g),
                             _ = o(892),
                             w = o.n(_),
                             k = o(173),
@@ -2804,20 +2806,20 @@
                                     if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
                                 }(this, e), this.highlight = "highlight", this.minimized = "minimized", this.preset_name = "Assignment View", this.initialize_events(), this.register()
                             }
                             var n, r;
                             return n = e, (r = [{
                                 key: "register",
                                 value: function() {
-                                    d.CellToolbar._presets.hasOwnProperty(this.preset_name) || (d.CellToolbar.register_callback("assignment_view.create_header", t().bind(this.create_header, this)), d.CellToolbar.register_preset(this.preset_name, ["assignment_view.create_header"], s().notebook))
+                                    d.CellToolbar._presets.hasOwnProperty(this.preset_name) || (d.CellToolbar.register_callback("assignment_view.create_header", t().bind(this.create_header, this)), d.CellToolbar.register_preset(this.preset_name, ["assignment_view.create_header"], c().notebook))
                                 }
                             }, {
                                 key: "activate",
                                 value: function() {
-                                    d.CellToolbar.activate_preset(this.preset_name), s().CellToolbar.global_show()
+                                    d.CellToolbar.activate_preset(this.preset_name), c().CellToolbar.global_show()
                                 }
                             }, {
                                 key: "initialize_events",
                                 value: function() {
                                     var e = this;
                                     u().on("preset_activated.CellToolbar", (function(t, n) {
                                         if (n.name != e.preset_name) {
@@ -2849,35 +2851,35 @@
                                                             },
                                                             f: o
                                                         }
                                                     }
                                                     throw new TypeError("Invalid attempt to iterate non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
                                                 }
                                                 var i, a = !0,
-                                                    c = !1;
+                                                    s = !1;
                                                 return {
                                                     s: function() {
                                                         n = n.call(e)
                                                     },
                                                     n: function() {
                                                         var e = n.next();
                                                         return a = e.done, e
                                                     },
                                                     e: function(e) {
-                                                        c = !0, i = e
+                                                        s = !0, i = e
                                                     },
                                                     f: function() {
                                                         try {
                                                             a || null == n.return || n.return()
                                                         } finally {
-                                                            if (c) throw i
+                                                            if (s) throw i
                                                         }
                                                     }
                                                 }
-                                            }(s().notebook.get_cells());
+                                            }(c().notebook.get_cells());
                                             try {
                                                 for (o.s(); !(r = o.n()).done;) {
                                                     var i = r.value;
                                                     e.remove_classes(i)
                                                 }
                                             } catch (e) {
                                                 o.e(e)
@@ -2907,35 +2909,37 @@
                                 value: function(e, t, n) {
                                     var r = a()("<button/>").attr("type", "button").attr("id", t).addClass("exam_btn").text(e);
                                     return r.on("click", n), r
                                 }
                             }, {
                                 key: "create_header",
                                 value: function(e, t, n) {
-                                    if (null === t.cell_type) setTimeout((function() {
-                                        this.create_header(e, t, n)
-                                    }), 100);
-                                    else {
+                                    if (null === t.cell_type) {
+                                        var r = this;
+                                        setTimeout((function() {
+                                            r.create_header(e, t, n)
+                                        }), 100)
+                                    } else {
                                         if (!f.utils.is_solution(t)) return this.remove_classes(t), void this.add_hidden(t);
-                                        if (this.add_highlight(t), p.utils.is_e2x(t)) return;
+                                        if (this.add_highlight(t), h.utils.is_e2x(t)) return;
                                         if ("code" === t.cell_type) {
-                                            var r = this.create_button("Run", "run", (function() {
+                                            var o = this.create_button("Run", "run", (function() {
                                                 t.execute()
                                             }));
-                                            a()(e).append(a()("<span/>").append(r).addClass("cell_control"))
+                                            a()(e).append(a()("<span/>").append(o).addClass("cell_control"))
                                         } else if ("markdown" === t.cell_type) {
-                                            var o = this.create_button("Edit", "edit", (function() {
+                                            var i = this.create_button("Edit", "edit", (function() {
                                                     t.events.trigger("select.Cell", {
                                                         cell: t
-                                                    }), s().notebook.edit_mode(), n.rebuild()
+                                                    }), c().notebook.edit_mode(), n.rebuild()
                                                 })),
-                                                i = this.create_button("Preview", "preview", (function() {
+                                                s = this.create_button("Preview", "preview", (function() {
                                                     t.execute(), n.rebuild()
                                                 }));
-                                            a()(e).append(a()("<span/>").append(o).append(i).addClass("cell_control"))
+                                            a()(e).append(a()("<span/>").append(i).append(s).addClass("cell_control"))
                                         }
                                     }
                                 }
                             }]) && function(e, t) {
                                 for (var n = 0; n < t.length; n++) {
                                     var r = t[n];
                                     r.enumerable = r.enumerable || !1, r.configurable = !0, "value" in r && (r.writable = !0), Object.defineProperty(e, r.key, r)
@@ -2949,22 +2953,22 @@
             },
             761: (e, t, n) => {
                 (() => {
                     var t = {
                             164: (e, t, n) => {
                                 "use strict";
                                 n.d(t, {
-                                    Z: () => c
+                                    Z: () => s
                                 });
                                 var r = n(601),
                                     o = n.n(r),
                                     i = n(609),
                                     a = n.n(i)()(o());
                                 a.push([e.id, ".hbrs_radio {\n  padding-top: 2em;\n  padding-left: 0.5em;\n}\n\n.hbrs_checkbox {\n  padding-top: 2em;\n  padding-left: 0.5em;\n}\n\n.hbrs_points {\n  width: 5em;\n  margin-left: 1em;\n  margin-right: 0.5em;\n}\n\n.hbrs_unrender {\n  margin-top: 1em;\n  margin-left: 0.5em;\n}\n\n.gallery-view {\n  min-height: 15em;\n  min-width: 100%;\n  overflow-y: scroll;\n  display: grid;\n  grid-template-columns: repeat(auto-fill, minmax(10em, 1fr));\n  grid-gap: 1em;\n  padding-right: 0.5em;\n}\n\n#upload-attachments {\n  display: none;\n}\n\n.gallery-item {\n  position: relative;\n  background-color: #eee;\n  border: 1px solid black;\n  height: 14em;\n  text-align: center;\n}\n\n.caption {\n  position: absolute;\n  padding-top: 1em;\n  top: 10em;\n  min-height: 4em;\n  width: 100%;\n  background-color: #bbb;\n  word-wrap: break-word;\n}\n\n.thumbnail {\n  height: 10em;\n  display: flex;\n  justify-content: center;\n  align-items: center;\n}\n\n.rendered_html > .edit_attachments {\n  margin-top: 2em;\n}\n\n.thumbnail img {\n  max-height: 10em;\n  max-width: 100%;\n}\n\n.gallery-item .fa-trash {\n  position: absolute;\n  right: 0.5em;\n  top: 0.5em;\n  color: #a00;\n}\n\n.gallery-item .fa-search-plus {\n  position: absolute;\n  right: 2em;\n  top: 0.5em;\n  color: #555;\n}\n\n.button-delete {\n  background: #a00;\n  color: #ddd;\n}\n\n.attachment-controls > button > i {\n  padding-right: 1em;\n}\n\niframe {\n  z-index: 5000;\n}\n", ""]);
-                                const c = a
+                                const s = a
                             },
                             609: e => {
                                 "use strict";
                                 e.exports = function(e) {
                                     var t = [];
                                     return t.toString = function() {
                                         return this.map((function(t) {
@@ -2974,17 +2978,17 @@
                                         })).join("")
                                     }, t.i = function(e, n, r, o, i) {
                                         "string" == typeof e && (e = [
                                             [null, e, void 0]
                                         ]);
                                         var a = {};
                                         if (r)
-                                            for (var c = 0; c < this.length; c++) {
-                                                var s = this[c][0];
-                                                null != s && (a[s] = !0)
+                                            for (var s = 0; s < this.length; s++) {
+                                                var c = this[s][0];
+                                                null != c && (a[c] = !0)
                                             }
                                         for (var l = 0; l < e.length; l++) {
                                             var u = [].concat(e[l]);
                                             r && a[u[0]] || (void 0 !== i && (void 0 === u[5] || (u[1] = "@layer".concat(u[5].length > 0 ? " ".concat(u[5]) : "", " {").concat(u[1], "}")), u[5] = i), n && (u[2] ? (u[1] = "@media ".concat(u[2], " {").concat(u[1], "}"), u[2] = n) : u[2] = n), o && (u[4] ? (u[1] = "@supports (".concat(u[4], ") {").concat(u[1], "}"), u[4] = o) : u[4] = "".concat(o)), t.push(u))
                                         }
                                     }, t
                                 }
@@ -3004,34 +3008,34 @@
                                         if (t[r].identifier === e) {
                                             n = r;
                                             break
                                         } return n
                                 }
 
                                 function r(e, r) {
-                                    for (var i = {}, a = [], c = 0; c < e.length; c++) {
-                                        var s = e[c],
-                                            l = r.base ? s[0] + r.base : s[0],
+                                    for (var i = {}, a = [], s = 0; s < e.length; s++) {
+                                        var c = e[s],
+                                            l = r.base ? c[0] + r.base : c[0],
                                             u = i[l] || 0,
                                             d = "".concat(l, " ").concat(u);
                                         i[l] = u + 1;
                                         var f = n(d),
-                                            p = {
-                                                css: s[1],
-                                                media: s[2],
-                                                sourceMap: s[3],
-                                                supports: s[4],
-                                                layer: s[5]
+                                            h = {
+                                                css: c[1],
+                                                media: c[2],
+                                                sourceMap: c[3],
+                                                supports: c[4],
+                                                layer: c[5]
                                             };
-                                        if (-1 !== f) t[f].references++, t[f].updater(p);
+                                        if (-1 !== f) t[f].references++, t[f].updater(h);
                                         else {
-                                            var h = o(p, r);
-                                            r.byIndex = c, t.splice(c, 0, {
+                                            var p = o(h, r);
+                                            r.byIndex = s, t.splice(s, 0, {
                                                 identifier: d,
-                                                updater: h,
+                                                updater: p,
                                                 references: 1
                                             })
                                         }
                                         a.push(d)
                                     }
                                     return a
                                 }
@@ -3047,22 +3051,22 @@
                                         }
                                 }
                                 e.exports = function(e, o) {
                                     var i = r(e = e || [], o = o || {});
                                     return function(e) {
                                         e = e || [];
                                         for (var a = 0; a < i.length; a++) {
-                                            var c = n(i[a]);
-                                            t[c].references--
+                                            var s = n(i[a]);
+                                            t[s].references--
                                         }
-                                        for (var s = r(e, o), l = 0; l < i.length; l++) {
+                                        for (var c = r(e, o), l = 0; l < i.length; l++) {
                                             var u = n(i[l]);
                                             0 === t[u].references && (t[u].updater(), t.splice(u, 1))
                                         }
-                                        i = s
+                                        i = c
                                     }
                                 }
                             },
                             793: e => {
                                 "use strict";
                                 var t = {};
                                 e.exports = function(e, n) {
@@ -3243,54 +3247,54 @@
                                             cells: () => Ne,
                                             utils: () => e
                                         });
                                         var e = {};
                                         o.r(e), o.d(e, {
                                             create_e2x_metadata: () => u,
                                             get_e2x_cell_type: () => f,
-                                            get_e2x_field: () => p,
+                                            get_e2x_field: () => h,
                                             get_e2x_metadata: () => d,
-                                            is_e2x: () => s,
+                                            is_e2x: () => c,
                                             remove_e2x_metadata: () => l,
-                                            set_e2x_field: () => h
+                                            set_e2x_field: () => p
                                         });
                                         const t = n(86);
                                         var r = o.n(t);
                                         const a = n(761);
-                                        var c = o.n(a);
+                                        var s = o.n(a);
 
-                                        function s(e) {
+                                        function c(e) {
                                             return e.hasOwnProperty("metadata") && e.metadata.hasOwnProperty("extended_cell")
                                         }
 
                                         function l(e) {
-                                            s(e) && (delete e.metadata.extended_cell, e.rendered && (e.unrender(), e.render()))
+                                            c(e) && (delete e.metadata.extended_cell, e.rendered && (e.unrender(), e.render()))
                                         }
 
                                         function u(e, t) {
-                                            s(e) || (e.metadata.extended_cell = {
+                                            c(e) || (e.metadata.extended_cell = {
                                                 type: t
                                             })
                                         }
 
                                         function d(e) {
-                                            return s(e) ? e.metadata.extended_cell : {}
+                                            return c(e) ? e.metadata.extended_cell : {}
                                         }
 
                                         function f(e) {
-                                            return p(e, "type", "")
+                                            return h(e, "type", "")
                                         }
 
-                                        function p(e, t) {
+                                        function h(e, t) {
                                             var n = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : {};
-                                            return s(e) && e.metadata.extended_cell[t] || n
+                                            return c(e) && e.metadata.extended_cell[t] || n
                                         }
 
-                                        function h(e, t, n) {
-                                            s(e) && (e.metadata.extended_cell[t] = n)
+                                        function p(e, t, n) {
+                                            c(e) && (e.metadata.extended_cell[t] = n)
                                         }
 
                                         function m(e, t) {
                                             (null == t || t > e.length) && (t = e.length);
                                             for (var n = 0, r = new Array(t); n < t; n++) r[n] = e[n];
                                             return r
                                         }
@@ -3301,81 +3305,81 @@
                                                 }(this, e), this.cell = t, this.options = n, this.initialize_options()
                                             }
                                             var t, n;
                                             return t = e, (n = [{
                                                 key: "initialize_options",
                                                 value: function() {
                                                     var e = this,
-                                                        t = p(this.cell, "options"),
+                                                        t = h(this.cell, "options"),
                                                         n = [];
                                                     Object.keys(t).forEach((function(t) {
                                                         e.options.hasOwnProperty(t) || n.push(t)
                                                     })), n.forEach((function(e) {
                                                         return delete t[e]
                                                     })), Object.keys(this.options).forEach((function(n) {
                                                         t.hasOwnProperty(n) || (t[n] = e.options[n])
-                                                    })), h(this.cell, "options", t)
+                                                    })), p(this.cell, "options", t)
                                                 }
                                             }, {
                                                 key: "get_option",
                                                 value: function(e) {
-                                                    var t = p(this.cell, "options");
+                                                    var t = h(this.cell, "options");
                                                     return t.hasOwnProperty(e) ? t[e] : this.options[e].value
                                                 }
                                             }, {
                                                 key: "set_option",
                                                 value: function(e, t) {
                                                     console.log("Setting options", e, t);
-                                                    var n = p(this.cell, "options");
-                                                    n[e].value = t, h(this.cell, "options", n)
+                                                    var n = h(this.cell, "options");
+                                                    n[e].value = t, p(this.cell, "options", n)
                                                 }
                                             }, {
                                                 key: "render",
                                                 value: function() {
-                                                    for (var e = this, t = c()("<div/>").addClass("e2x_options"), n = function() {
+                                                    for (var e = this, t = s()("<div/>").addClass("e2x_options"), n = function() {
                                                             var n, i = function(e) {
                                                                     if (Array.isArray(e)) return e
                                                                 }(n = o[r]) || function(e, t) {
                                                                     var n = null == e ? null : "undefined" != typeof Symbol && e[Symbol.iterator] || e["@@iterator"];
                                                                     if (null != n) {
                                                                         var r, o, i = [],
                                                                             a = !0,
-                                                                            c = !1;
+                                                                            s = !1;
                                                                         try {
                                                                             for (n = n.call(e); !(a = (r = n.next()).done) && (i.push(r.value), 2 !== i.length); a = !0);
                                                                         } catch (e) {
-                                                                            c = !0, o = e
+                                                                            s = !0, o = e
                                                                         } finally {
                                                                             try {
                                                                                 a || null == n.return || n.return()
                                                                             } finally {
-                                                                                if (c) throw o
+                                                                                if (s) throw o
                                                                             }
                                                                         }
                                                                         return i
                                                                     }
                                                                 }(n) || function(e, t) {
                                                                     if (e) {
                                                                         if ("string" == typeof e) return m(e, 2);
                                                                         var n = Object.prototype.toString.call(e).slice(8, -1);
                                                                         return "Object" === n && e.constructor && (n = e.constructor.name), "Map" === n || "Set" === n ? Array.from(e) : "Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n) ? m(e, 2) : void 0
                                                                     }
                                                                 }(n) || function() {
                                                                     throw new TypeError("Invalid attempt to destructure non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
                                                                 }(),
                                                                 a = i[0],
-                                                                s = i[1];
-                                                            if ("checkbox" == s.type) {
-                                                                var l = c()("<div/>"),
-                                                                    u = c()("<input/>").attr("type", s.type);
-                                                                l.append(u), l.append(c()("<span/>").text(s.text)), s.value && u.attr("checked", "checked"), u.on("change", (function() {
+                                                                c = i[1];
+                                                            if ("checkbox" == c.type) {
+                                                                var l = s()("<div/>"),
+                                                                    u = s()("<input/>").attr("type", c.type);
+                                                                l.append(u), l.append(s()("<span/>").text(c.text)), c.value && u.attr("checked", "checked"), u.on("change", (function() {
                                                                     e.set_option(a, !!this.checked)
                                                                 })), t.append(l)
                                                             }
-                                                        }, r = 0, o = Object.entries(p(this.cell, "options")); r < o.length; r++) n();
+                                                        }, r = 0, o = Object.entries(h(this.cell, "options")); r < o.length; r++) n();
                                                     return t
                                                 }
                                             }]) && function(e, t) {
                                                 for (var n = 0; n < t.length; n++) {
                                                     var r = t[n];
                                                     r.enumerable = r.enumerable || !1, r.configurable = !0, "value" in r && (r.writable = !0), Object.defineProperty(e, r.key, r)
                                                 }
@@ -3404,18 +3408,18 @@
                                                     this.cell.render()
                                                 }
                                             }, {
                                                 key: "render_grader_settings",
                                                 value: function() {
                                                     if (this.edit_mode) {
                                                         var e = this,
-                                                            t = c()(this.cell.element).find(".rendered_html");
+                                                            t = s()(this.cell.element).find(".rendered_html");
                                                         t.find(".e2x_grader_options").remove();
-                                                        var n = c()("<div/>").addClass("e2x_grader_options");
-                                                        n.append(c()("<hr/>")), n.append(this.option_dict.render()), n.append(c()("<button/>").attr("type", "button").addClass("e2x_unrender").on("click", (function() {
+                                                        var n = s()("<div/>").addClass("e2x_grader_options");
+                                                        n.append(s()("<hr/>")), n.append(this.option_dict.render()), n.append(s()("<button/>").attr("type", "button").addClass("e2x_unrender").on("click", (function() {
                                                             e.cell.unrender_force(), e.cell.keyboard_manager.enable()
                                                         })).append("Edit cell")), t.append(n)
                                                     }
                                                 }
                                             }]) && function(e, t) {
                                                 for (var n = 0; n < t.length; n++) {
                                                     var r = t[n];
@@ -3512,20 +3516,20 @@
                                                 function n(e, r) {
                                                     var o;
                                                     return _(this, n), (o = t.call(this, e, r)).choice_field = "choice", o
                                                 }
                                                 return k(n, [{
                                                     key: "set_choice",
                                                     value: function(e) {
-                                                        h(this.cell, this.choice_field, e)
+                                                        p(this.cell, this.choice_field, e)
                                                     }
                                                 }, {
                                                     key: "get_choices",
                                                     value: function() {
-                                                        return p(this.cell, this.choice_field, [])
+                                                        return h(this.cell, this.choice_field, [])
                                                     }
                                                 }]), n
                                             }(g),
                                             A = function(e) {
                                                 x(n, e);
                                                 var t = E(n);
 
@@ -3546,19 +3550,19 @@
                                                             t = this.get_choices(),
                                                             n = this;
                                                         if (e.length > 0) {
                                                             var o = e[0],
                                                                 i = $("<form>").addClass("hbrs_radio"),
                                                                 a = $(o).find("li");
                                                             t.length > 0 && t[0] >= a.length && (this.get_metadata()[this.choice_field] = [], t = this.get_choices());
-                                                            for (var c = 0; c < a.length; c++) {
-                                                                var s = this.create_radio_button("my_radio", c, t.indexOf(c.toString()) >= 0, (function() {
+                                                            for (var s = 0; s < a.length; s++) {
+                                                                var c = this.create_radio_button("my_radio", s, t.indexOf(s.toString()) >= 0, (function() {
                                                                     n.set_choice(this.value)
                                                                 }));
-                                                                r().keyboard_manager.register_events(s), i.append($("<div>").append(s).append("&nbsp;&nbsp;").append(a[c].childNodes))
+                                                                r().keyboard_manager.register_events(c), i.append($("<div>").append(c).append("&nbsp;&nbsp;").append(a[s].childNodes))
                                                             }
                                                             $(o).replaceWith(i)
                                                         }
                                                         this.render_grader_settings()
                                                     }
                                                 }]), n
                                             }(C),
@@ -3569,20 +3573,20 @@
                                                 function n(e) {
                                                     var r;
                                                     return _(this, n), (r = t.call(this, e, "multiplechoice")).choice_count_field = "num_of_choices", r
                                                 }
                                                 return k(n, [{
                                                     key: "get_number_of_choices",
                                                     value: function() {
-                                                        return p(this.cell, this.choice_count_field, [])
+                                                        return h(this.cell, this.choice_count_field, [])
                                                     }
                                                 }, {
                                                     key: "set_number_of_choices",
                                                     value: function(e) {
-                                                        h(this.cell, this.choice_count_field, e)
+                                                        p(this.cell, this.choice_count_field, e)
                                                     }
                                                 }, {
                                                     key: "add_choice",
                                                     value: function(e) {
                                                         var t = this.get_choices();
                                                         t.indexOf(e) > -1 || (t.push(e), this.set_choice(t))
                                                     }
@@ -3609,18 +3613,18 @@
                                                         var e = $(this.cell.element).find(".rendered_html").find("ul");
                                                         if (e.length > 0) {
                                                             var t = e[0],
                                                                 n = $("<form>").addClass("hbrs_checkbox"),
                                                                 o = $(t).find("li");
                                                             this.get_number_of_choices() != o.length && (this.set_number_of_choices(o.length), this.get_metadata()[this.choice_field] = []);
                                                             for (var i = this.get_choices(), a = 0; a < o.length; a++) {
-                                                                var c = this.create_checkbox("my_checkbox", a, i.indexOf(a.toString()) >= 0);
-                                                                r().keyboard_manager.register_events(c);
-                                                                var s = $("<div>").append(c).append("&nbsp;&nbsp;").append(o[a].childNodes);
-                                                                n.append(s)
+                                                                var s = this.create_checkbox("my_checkbox", a, i.indexOf(a.toString()) >= 0);
+                                                                r().keyboard_manager.register_events(s);
+                                                                var c = $("<div>").append(s).append("&nbsp;&nbsp;").append(o[a].childNodes);
+                                                                n.append(c)
                                                             }
                                                             $(t).replaceWith(n)
                                                         }
                                                         this.render_grader_settings()
                                                     }
                                                 }]), n
                                             }(C);
@@ -3882,31 +3886,31 @@
                                                 t = Object.prototype,
                                                 n = t.hasOwnProperty,
                                                 r = "function" == typeof Symbol ? Symbol : {},
                                                 o = r.iterator || "@@iterator",
                                                 i = r.asyncIterator || "@@asyncIterator",
                                                 a = r.toStringTag || "@@toStringTag";
 
-                                            function c(e, t, n) {
+                                            function s(e, t, n) {
                                                 return Object.defineProperty(e, t, {
                                                     value: n,
                                                     enumerable: !0,
                                                     configurable: !0,
                                                     writable: !0
                                                 }), e[t]
                                             }
                                             try {
-                                                c({}, "")
+                                                s({}, "")
                                             } catch (e) {
-                                                c = function(e, t, n) {
+                                                s = function(e, t, n) {
                                                     return e[t] = n
                                                 }
                                             }
 
-                                            function s(e, t, n, r) {
+                                            function c(e, t, n, r) {
                                                 var o = t && t.prototype instanceof d ? t : d,
                                                     i = Object.create(o.prototype),
                                                     a = new x(r || []);
                                                 return i._invoke = function(e, t, n) {
                                                     var r = "suspendedStart";
                                                     return function(o, i) {
                                                         if ("executing" === r) throw new Error("Generator is already running");
@@ -3916,35 +3920,35 @@
                                                                 value: void 0,
                                                                 done: !0
                                                             }
                                                         }
                                                         for (n.method = o, n.arg = i;;) {
                                                             var a = n.delegate;
                                                             if (a) {
-                                                                var c = _(a, n);
-                                                                if (c) {
-                                                                    if (c === u) continue;
-                                                                    return c
+                                                                var s = _(a, n);
+                                                                if (s) {
+                                                                    if (s === u) continue;
+                                                                    return s
                                                                 }
                                                             }
                                                             if ("next" === n.method) n.sent = n._sent = n.arg;
                                                             else if ("throw" === n.method) {
                                                                 if ("suspendedStart" === r) throw r = "completed", n.arg;
                                                                 n.dispatchException(n.arg)
                                                             } else "return" === n.method && n.abrupt("return", n.arg);
                                                             r = "executing";
-                                                            var s = l(e, t, n);
-                                                            if ("normal" === s.type) {
-                                                                if (r = n.done ? "completed" : "suspendedYield", s.arg === u) continue;
+                                                            var c = l(e, t, n);
+                                                            if ("normal" === c.type) {
+                                                                if (r = n.done ? "completed" : "suspendedYield", c.arg === u) continue;
                                                                 return {
-                                                                    value: s.arg,
+                                                                    value: c.arg,
                                                                     done: n.done
                                                                 }
                                                             }
-                                                            "throw" === s.type && (r = "completed", n.method = "throw", n.arg = s.arg)
+                                                            "throw" === c.type && (r = "completed", n.method = "throw", n.arg = c.arg)
                                                         }
                                                     }
                                                 }(e, n, a), i
                                             }
 
                                             function l(e, t, n) {
                                                 try {
@@ -3955,56 +3959,56 @@
                                                 } catch (e) {
                                                     return {
                                                         type: "throw",
                                                         arg: e
                                                     }
                                                 }
                                             }
-                                            e.wrap = s;
+                                            e.wrap = c;
                                             var u = {};
 
                                             function d() {}
 
                                             function f() {}
 
-                                            function p() {}
-                                            var h = {};
-                                            c(h, o, (function() {
+                                            function h() {}
+                                            var p = {};
+                                            s(p, o, (function() {
                                                 return this
                                             }));
                                             var m = Object.getPrototypeOf,
                                                 y = m && m(m(O([])));
-                                            y && y !== t && n.call(y, o) && (h = y);
-                                            var v = p.prototype = d.prototype = Object.create(h);
+                                            y && y !== t && n.call(y, o) && (p = y);
+                                            var v = h.prototype = d.prototype = Object.create(p);
 
                                             function g(e) {
                                                 ["next", "throw", "return"].forEach((function(t) {
-                                                    c(e, t, (function(e) {
+                                                    s(e, t, (function(e) {
                                                         return this._invoke(t, e)
                                                     }))
                                                 }))
                                             }
 
                                             function b(e, t) {
-                                                function r(o, i, a, c) {
-                                                    var s = l(e[o], e, i);
-                                                    if ("throw" !== s.type) {
-                                                        var u = s.arg,
+                                                function r(o, i, a, s) {
+                                                    var c = l(e[o], e, i);
+                                                    if ("throw" !== c.type) {
+                                                        var u = c.arg,
                                                             d = u.value;
                                                         return d && "object" == U(d) && n.call(d, "__await") ? t.resolve(d.__await).then((function(e) {
-                                                            r("next", e, a, c)
+                                                            r("next", e, a, s)
                                                         }), (function(e) {
-                                                            r("throw", e, a, c)
+                                                            r("throw", e, a, s)
                                                         })) : t.resolve(d).then((function(e) {
                                                             u.value = e, a(u)
                                                         }), (function(e) {
-                                                            return r("throw", e, a, c)
+                                                            return r("throw", e, a, s)
                                                         }))
                                                     }
-                                                    c(s.arg)
+                                                    s(c.arg)
                                                 }
                                                 var o;
                                                 this._invoke = function(e, n) {
                                                     function i() {
                                                         return new t((function(t, o) {
                                                             r(e, n, t, o)
                                                         }))
@@ -4068,34 +4072,34 @@
 
                                             function E() {
                                                 return {
                                                     value: void 0,
                                                     done: !0
                                                 }
                                             }
-                                            return f.prototype = p, c(v, "constructor", p), c(p, "constructor", f), f.displayName = c(p, a, "GeneratorFunction"), e.isGeneratorFunction = function(e) {
+                                            return f.prototype = h, s(v, "constructor", h), s(h, "constructor", f), f.displayName = s(h, a, "GeneratorFunction"), e.isGeneratorFunction = function(e) {
                                                 var t = "function" == typeof e && e.constructor;
                                                 return !!t && (t === f || "GeneratorFunction" === (t.displayName || t.name))
                                             }, e.mark = function(e) {
-                                                return Object.setPrototypeOf ? Object.setPrototypeOf(e, p) : (e.__proto__ = p, c(e, a, "GeneratorFunction")), e.prototype = Object.create(v), e
+                                                return Object.setPrototypeOf ? Object.setPrototypeOf(e, h) : (e.__proto__ = h, s(e, a, "GeneratorFunction")), e.prototype = Object.create(v), e
                                             }, e.awrap = function(e) {
                                                 return {
                                                     __await: e
                                                 }
-                                            }, g(b.prototype), c(b.prototype, i, (function() {
+                                            }, g(b.prototype), s(b.prototype, i, (function() {
                                                 return this
                                             })), e.AsyncIterator = b, e.async = function(t, n, r, o, i) {
                                                 void 0 === i && (i = Promise);
-                                                var a = new b(s(t, n, r, o), i);
+                                                var a = new b(c(t, n, r, o), i);
                                                 return e.isGeneratorFunction(n) ? a : a.next().then((function(e) {
                                                     return e.done ? e.value : a.next()
                                                 }))
-                                            }, g(v), c(v, a, "Generator"), c(v, o, (function() {
+                                            }, g(v), s(v, a, "Generator"), s(v, o, (function() {
                                                 return this
-                                            })), c(v, "toString", (function() {
+                                            })), s(v, "toString", (function() {
                                                 return "[object Generator]"
                                             })), e.keys = function(e) {
                                                 var t = [];
                                                 for (var n in e) t.push(n);
                                                 return t.reverse(),
                                                     function n() {
                                                         for (; t.length;) {
@@ -4124,23 +4128,23 @@
                                                         return a.type = "throw", a.arg = e, t.next = n, r && (t.method = "next", t.arg = void 0), !!r
                                                     }
                                                     for (var o = this.tryEntries.length - 1; o >= 0; --o) {
                                                         var i = this.tryEntries[o],
                                                             a = i.completion;
                                                         if ("root" === i.tryLoc) return r("end");
                                                         if (i.tryLoc <= this.prev) {
-                                                            var c = n.call(i, "catchLoc"),
-                                                                s = n.call(i, "finallyLoc");
-                                                            if (c && s) {
+                                                            var s = n.call(i, "catchLoc"),
+                                                                c = n.call(i, "finallyLoc");
+                                                            if (s && c) {
                                                                 if (this.prev < i.catchLoc) return r(i.catchLoc, !0);
                                                                 if (this.prev < i.finallyLoc) return r(i.finallyLoc)
-                                                            } else if (c) {
+                                                            } else if (s) {
                                                                 if (this.prev < i.catchLoc) return r(i.catchLoc, !0)
                                                             } else {
-                                                                if (!s) throw new Error("try statement without catch or finally");
+                                                                if (!c) throw new Error("try statement without catch or finally");
                                                                 if (this.prev < i.finallyLoc) return r(i.finallyLoc)
                                                             }
                                                         }
                                                     }
                                                 },
                                                 abrupt: function(e, t) {
                                                     for (var r = this.tryEntries.length - 1; r >= 0; --r) {
@@ -4229,35 +4233,35 @@
                                                 var r = t[n];
                                                 r.enumerable = r.enumerable || !1, r.configurable = !0, "value" in r && (r.writable = !0), Object.defineProperty(e, r.key, r)
                                             }
                                         }
 
                                         function X(e, t, n, r, o, i, a) {
                                             try {
-                                                var c = e[i](a),
-                                                    s = c.value
+                                                var s = e[i](a),
+                                                    c = s.value
                                             } catch (e) {
                                                 return void n(e)
                                             }
-                                            c.done ? t(s) : Promise.resolve(s).then(r, o)
+                                            s.done ? t(c) : Promise.resolve(c).then(r, o)
                                         }
 
                                         function ee(e) {
                                             return function() {
                                                 var t = this,
                                                     n = arguments;
                                                 return new Promise((function(r, o) {
                                                     var i = e.apply(t, n);
 
                                                     function a(e) {
-                                                        X(i, r, o, a, c, "next", e)
+                                                        X(i, r, o, a, s, "next", e)
                                                     }
 
-                                                    function c(e) {
-                                                        X(i, r, o, a, c, "throw", e)
+                                                    function s(e) {
+                                                        X(i, r, o, a, s, "throw", e)
                                                     }
                                                     a(void 0)
                                                 }))
                                             }
                                         }
                                         var te = !1,
                                             ne = {};
@@ -4288,18 +4292,18 @@
                                                 }), e, null, [
                                                     [1, 8]
                                                 ])
                                             })))).apply(this, arguments)
                                         }
                                         const ie = function() {
                                             function e(t, n, r, o, i, a) {
-                                                var c = arguments.length > 6 && void 0 !== arguments[6] ? arguments[6] : {};
+                                                var s = arguments.length > 6 && void 0 !== arguments[6] ? arguments[6] : {};
                                                 K(this, e), this.config = null, this.ui = "min", this.xml = null, this.format = "xml", this.libraries = !0, this.frameStyle = "position:absolute;bottom:0;border:0;width:100%;height:100%;";
-                                                var s = H(H({}, ne), c);
-                                                this.config = t || this.config, this.ui = n || this.ui, this.done = r || function() {}, this.initialized = o || function() {}, this.urlParams = i, this.cell = a, this.handleMessageEvent = this.handleMessageEvent.bind(this), this.frame = null, this.startElement = null, this.format = "xml", this.xml = null, this.drawDomain = s.drawDomain || "https://embed.diagrams.net/", this.origin = s.drawOrigin || "https://embed.diagrams.net/", this.frameStyle = "position:absolute;bottom:0;border:0;width:100%;height:100%;", this.libs = s.libs || []
+                                                var c = H(H({}, ne), s);
+                                                this.config = t || this.config, this.ui = n || this.ui, this.done = r || function() {}, this.initialized = o || function() {}, this.urlParams = i, this.cell = a, this.handleMessageEvent = this.handleMessageEvent.bind(this), this.frame = null, this.startElement = null, this.format = "xml", this.xml = null, this.drawDomain = c.drawDomain || "https://embed.diagrams.net/", this.origin = c.drawOrigin || "https://embed.diagrams.net/", this.frameStyle = "position:absolute;bottom:0;border:0;width:100%;height:100%;", this.libs = c.libs || []
                                             }
                                             var t, n, r, o;
                                             return t = e, n = [{
                                                 key: "handleMessageEvent",
                                                 value: function(e) {
                                                     var t = new URL(this.origin),
                                                         n = new URL(e.origin);
@@ -4437,29 +4441,29 @@
                                                 key: "save",
                                                 value: function(e, t, n) {
                                                     this.done(e, t, n)
                                                 }
                                             }], r = [{
                                                 key: "editElement",
                                                 value: function(t, n, r, o, i, a) {
-                                                    var c = arguments.length > 6 && void 0 !== arguments[6] ? arguments[6] : {};
+                                                    var s = arguments.length > 6 && void 0 !== arguments[6] ? arguments[6] : {};
                                                     if (!n.diagramEditorStarting) return n.diagramEditorStarting = !0, new e(r, o, i, (function() {
                                                         delete n.diagramEditorStarting
-                                                    }), a, t, c).editElement(n)
+                                                    }), a, t, s).editElement(n)
                                                 }
                                             }, {
                                                 key: "editDiagram",
                                                 value: (o = ee(F().mark((function e(t, n, r, o, i, a) {
-                                                    var c, s = this,
+                                                    var s, c = this,
                                                         l = arguments;
                                                     return F().wrap((function(e) {
                                                         for (;;) switch (e.prev = e.next) {
                                                             case 0:
-                                                                c = l.length > 6 && void 0 !== l[6] ? l[6] : {}, re().then((function() {
-                                                                    return s.editElement(t, n, r, o, i, a, c)
+                                                                s = l.length > 6 && void 0 !== l[6] ? l[6] : {}, re().then((function() {
+                                                                    return c.editElement(t, n, r, o, i, a, s)
                                                                 }));
                                                             case 2:
                                                             case "end":
                                                                 return e.stop()
                                                         }
                                                     }), e)
                                                 }))), function(e, t, n, r, i, a) {
@@ -4474,43 +4478,43 @@
                                             return ae = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
                                                 return typeof e
                                             } : function(e) {
                                                 return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
                                             }, ae(e)
                                         }
 
-                                        function ce() {
-                                            ce = function() {
+                                        function se() {
+                                            se = function() {
                                                 return e
                                             };
                                             var e = {},
                                                 t = Object.prototype,
                                                 n = t.hasOwnProperty,
                                                 r = "function" == typeof Symbol ? Symbol : {},
                                                 o = r.iterator || "@@iterator",
                                                 i = r.asyncIterator || "@@asyncIterator",
                                                 a = r.toStringTag || "@@toStringTag";
 
-                                            function c(e, t, n) {
+                                            function s(e, t, n) {
                                                 return Object.defineProperty(e, t, {
                                                     value: n,
                                                     enumerable: !0,
                                                     configurable: !0,
                                                     writable: !0
                                                 }), e[t]
                                             }
                                             try {
-                                                c({}, "")
+                                                s({}, "")
                                             } catch (e) {
-                                                c = function(e, t, n) {
+                                                s = function(e, t, n) {
                                                     return e[t] = n
                                                 }
                                             }
 
-                                            function s(e, t, n, r) {
+                                            function c(e, t, n, r) {
                                                 var o = t && t.prototype instanceof d ? t : d,
                                                     i = Object.create(o.prototype),
                                                     a = new x(r || []);
                                                 return i._invoke = function(e, t, n) {
                                                     var r = "suspendedStart";
                                                     return function(o, i) {
                                                         if ("executing" === r) throw new Error("Generator is already running");
@@ -4520,35 +4524,35 @@
                                                                 value: void 0,
                                                                 done: !0
                                                             }
                                                         }
                                                         for (n.method = o, n.arg = i;;) {
                                                             var a = n.delegate;
                                                             if (a) {
-                                                                var c = _(a, n);
-                                                                if (c) {
-                                                                    if (c === u) continue;
-                                                                    return c
+                                                                var s = _(a, n);
+                                                                if (s) {
+                                                                    if (s === u) continue;
+                                                                    return s
                                                                 }
                                                             }
                                                             if ("next" === n.method) n.sent = n._sent = n.arg;
                                                             else if ("throw" === n.method) {
                                                                 if ("suspendedStart" === r) throw r = "completed", n.arg;
                                                                 n.dispatchException(n.arg)
                                                             } else "return" === n.method && n.abrupt("return", n.arg);
                                                             r = "executing";
-                                                            var s = l(e, t, n);
-                                                            if ("normal" === s.type) {
-                                                                if (r = n.done ? "completed" : "suspendedYield", s.arg === u) continue;
+                                                            var c = l(e, t, n);
+                                                            if ("normal" === c.type) {
+                                                                if (r = n.done ? "completed" : "suspendedYield", c.arg === u) continue;
                                                                 return {
-                                                                    value: s.arg,
+                                                                    value: c.arg,
                                                                     done: n.done
                                                                 }
                                                             }
-                                                            "throw" === s.type && (r = "completed", n.method = "throw", n.arg = s.arg)
+                                                            "throw" === c.type && (r = "completed", n.method = "throw", n.arg = c.arg)
                                                         }
                                                     }
                                                 }(e, n, a), i
                                             }
 
                                             function l(e, t, n) {
                                                 try {
@@ -4559,56 +4563,56 @@
                                                 } catch (e) {
                                                     return {
                                                         type: "throw",
                                                         arg: e
                                                     }
                                                 }
                                             }
-                                            e.wrap = s;
+                                            e.wrap = c;
                                             var u = {};
 
                                             function d() {}
 
                                             function f() {}
 
-                                            function p() {}
-                                            var h = {};
-                                            c(h, o, (function() {
+                                            function h() {}
+                                            var p = {};
+                                            s(p, o, (function() {
                                                 return this
                                             }));
                                             var m = Object.getPrototypeOf,
                                                 y = m && m(m(O([])));
-                                            y && y !== t && n.call(y, o) && (h = y);
-                                            var v = p.prototype = d.prototype = Object.create(h);
+                                            y && y !== t && n.call(y, o) && (p = y);
+                                            var v = h.prototype = d.prototype = Object.create(p);
 
                                             function g(e) {
                                                 ["next", "throw", "return"].forEach((function(t) {
-                                                    c(e, t, (function(e) {
+                                                    s(e, t, (function(e) {
                                                         return this._invoke(t, e)
                                                     }))
                                                 }))
                                             }
 
                                             function b(e, t) {
-                                                function r(o, i, a, c) {
-                                                    var s = l(e[o], e, i);
-                                                    if ("throw" !== s.type) {
-                                                        var u = s.arg,
+                                                function r(o, i, a, s) {
+                                                    var c = l(e[o], e, i);
+                                                    if ("throw" !== c.type) {
+                                                        var u = c.arg,
                                                             d = u.value;
                                                         return d && "object" == ae(d) && n.call(d, "__await") ? t.resolve(d.__await).then((function(e) {
-                                                            r("next", e, a, c)
+                                                            r("next", e, a, s)
                                                         }), (function(e) {
-                                                            r("throw", e, a, c)
+                                                            r("throw", e, a, s)
                                                         })) : t.resolve(d).then((function(e) {
                                                             u.value = e, a(u)
                                                         }), (function(e) {
-                                                            return r("throw", e, a, c)
+                                                            return r("throw", e, a, s)
                                                         }))
                                                     }
-                                                    c(s.arg)
+                                                    s(c.arg)
                                                 }
                                                 var o;
                                                 this._invoke = function(e, n) {
                                                     function i() {
                                                         return new t((function(t, o) {
                                                             r(e, n, t, o)
                                                         }))
@@ -4672,34 +4676,34 @@
 
                                             function E() {
                                                 return {
                                                     value: void 0,
                                                     done: !0
                                                 }
                                             }
-                                            return f.prototype = p, c(v, "constructor", p), c(p, "constructor", f), f.displayName = c(p, a, "GeneratorFunction"), e.isGeneratorFunction = function(e) {
+                                            return f.prototype = h, s(v, "constructor", h), s(h, "constructor", f), f.displayName = s(h, a, "GeneratorFunction"), e.isGeneratorFunction = function(e) {
                                                 var t = "function" == typeof e && e.constructor;
                                                 return !!t && (t === f || "GeneratorFunction" === (t.displayName || t.name))
                                             }, e.mark = function(e) {
-                                                return Object.setPrototypeOf ? Object.setPrototypeOf(e, p) : (e.__proto__ = p, c(e, a, "GeneratorFunction")), e.prototype = Object.create(v), e
+                                                return Object.setPrototypeOf ? Object.setPrototypeOf(e, h) : (e.__proto__ = h, s(e, a, "GeneratorFunction")), e.prototype = Object.create(v), e
                                             }, e.awrap = function(e) {
                                                 return {
                                                     __await: e
                                                 }
-                                            }, g(b.prototype), c(b.prototype, i, (function() {
+                                            }, g(b.prototype), s(b.prototype, i, (function() {
                                                 return this
                                             })), e.AsyncIterator = b, e.async = function(t, n, r, o, i) {
                                                 void 0 === i && (i = Promise);
-                                                var a = new b(s(t, n, r, o), i);
+                                                var a = new b(c(t, n, r, o), i);
                                                 return e.isGeneratorFunction(n) ? a : a.next().then((function(e) {
                                                     return e.done ? e.value : a.next()
                                                 }))
-                                            }, g(v), c(v, a, "Generator"), c(v, o, (function() {
+                                            }, g(v), s(v, a, "Generator"), s(v, o, (function() {
                                                 return this
-                                            })), c(v, "toString", (function() {
+                                            })), s(v, "toString", (function() {
                                                 return "[object Generator]"
                                             })), e.keys = function(e) {
                                                 var t = [];
                                                 for (var n in e) t.push(n);
                                                 return t.reverse(),
                                                     function n() {
                                                         for (; t.length;) {
@@ -4728,23 +4732,23 @@
                                                         return a.type = "throw", a.arg = e, t.next = n, r && (t.method = "next", t.arg = void 0), !!r
                                                     }
                                                     for (var o = this.tryEntries.length - 1; o >= 0; --o) {
                                                         var i = this.tryEntries[o],
                                                             a = i.completion;
                                                         if ("root" === i.tryLoc) return r("end");
                                                         if (i.tryLoc <= this.prev) {
-                                                            var c = n.call(i, "catchLoc"),
-                                                                s = n.call(i, "finallyLoc");
-                                                            if (c && s) {
+                                                            var s = n.call(i, "catchLoc"),
+                                                                c = n.call(i, "finallyLoc");
+                                                            if (s && c) {
                                                                 if (this.prev < i.catchLoc) return r(i.catchLoc, !0);
                                                                 if (this.prev < i.finallyLoc) return r(i.finallyLoc)
-                                                            } else if (c) {
+                                                            } else if (s) {
                                                                 if (this.prev < i.catchLoc) return r(i.catchLoc, !0)
                                                             } else {
-                                                                if (!s) throw new Error("try statement without catch or finally");
+                                                                if (!c) throw new Error("try statement without catch or finally");
                                                                 if (this.prev < i.finallyLoc) return r(i.finallyLoc)
                                                             }
                                                         }
                                                     }
                                                 },
                                                 abrupt: function(e, t) {
                                                     for (var r = this.tryEntries.length - 1; r >= 0; --r) {
@@ -4788,22 +4792,22 @@
                                                         resultName: t,
                                                         nextLoc: n
                                                     }, "next" === this.method && (this.arg = void 0), u
                                                 }
                                             }, e
                                         }
 
-                                        function se(e, t, n, r, o, i, a) {
+                                        function ce(e, t, n, r, o, i, a) {
                                             try {
-                                                var c = e[i](a),
-                                                    s = c.value
+                                                var s = e[i](a),
+                                                    c = s.value
                                             } catch (e) {
                                                 return void n(e)
                                             }
-                                            c.done ? t(s) : Promise.resolve(s).then(r, o)
+                                            s.done ? t(c) : Promise.resolve(c).then(r, o)
                                         }
 
                                         function le(e, t) {
                                             if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
                                         }
 
                                         function ue(e, t) {
@@ -4825,24 +4829,24 @@
                                                 constructor: {
                                                     value: e,
                                                     writable: !0,
                                                     configurable: !0
                                                 }
                                             }), Object.defineProperty(e, "prototype", {
                                                 writable: !1
-                                            }), t && pe(e, t)
+                                            }), t && he(e, t)
                                         }
 
-                                        function pe(e, t) {
-                                            return pe = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(e, t) {
+                                        function he(e, t) {
+                                            return he = Object.setPrototypeOf ? Object.setPrototypeOf.bind() : function(e, t) {
                                                 return e.__proto__ = t, e
-                                            }, pe(e, t)
+                                            }, he(e, t)
                                         }
 
-                                        function he(e) {
+                                        function pe(e) {
                                             var t = function() {
                                                 if ("undefined" == typeof Reflect || !Reflect.construct) return !1;
                                                 if (Reflect.construct.sham) return !1;
                                                 if ("function" == typeof Proxy) return !0;
                                                 try {
                                                     return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], (function() {}))), !0
                                                 } catch (e) {
@@ -4871,29 +4875,29 @@
                                         function ye(e) {
                                             return ye = Object.setPrototypeOf ? Object.getPrototypeOf.bind() : function(e) {
                                                 return e.__proto__ || Object.getPrototypeOf(e)
                                             }, ye(e)
                                         }
                                         var ve = function(e) {
                                                 fe(n, e);
-                                                var t = he(n);
+                                                var t = pe(n);
 
                                                 function n() {
                                                     return le(this, n), t.apply(this, arguments)
                                                 }
                                                 return de(n, [{
                                                     key: "postSaveHook",
                                                     value: function() {
                                                         this.cell.unrender_force(), this.cell.render()
                                                     }
                                                 }]), n
                                             }(R),
                                             ge = function(e) {
                                                 fe(n, e);
-                                                var t = he(n);
+                                                var t = pe(n);
 
                                                 function n(e) {
                                                     var r;
                                                     return le(this, n), (r = t.call(this, e, "diagram", {
                                                         replace_diagram: {
                                                             type: "checkbox",
                                                             text: "Replace this diagram with an empty diagram in the student version",
@@ -4919,25 +4923,25 @@
                                                             return function() {
                                                                 var t = this,
                                                                     n = arguments;
                                                                 return new Promise((function(r, o) {
                                                                     var i = e.apply(t, n);
 
                                                                     function a(e) {
-                                                                        se(i, r, o, a, c, "next", e)
+                                                                        ce(i, r, o, a, s, "next", e)
                                                                     }
 
-                                                                    function c(e) {
-                                                                        se(i, r, o, a, c, "throw", e)
+                                                                    function s(e) {
+                                                                        ce(i, r, o, a, s, "throw", e)
                                                                     }
                                                                     a(void 0)
                                                                 }))
                                                             }
-                                                        }(ce().mark((function t() {
-                                                            return ce().wrap((function(t) {
+                                                        }(se().mark((function t() {
+                                                            return se().wrap((function(t) {
                                                                 for (;;) switch (t.prev = t.next) {
                                                                     case 0:
                                                                         return t.prev = 0, t.next = 3, ie.editDiagram(e, r[0]);
                                                                     case 3:
                                                                         t.next = 8;
                                                                         break;
                                                                     case 5:
@@ -5028,34 +5032,34 @@
                                                             alert("Could not access webcam!\n" + e)
                                                         }))
                                                     }
                                                 }, {
                                                     key: "openDialog",
                                                     value: function() {
                                                         var e = this,
-                                                            t = c()("<div/>").attr("id", "webcamDiv"),
-                                                            n = c()("<video/>");
+                                                            t = s()("<div/>").attr("id", "webcamDiv"),
+                                                            n = s()("<video/>");
                                                         t.append(n);
-                                                        var r = c()("<div/>").attr("id", "videoControls");
-                                                        r.append(c()("<button/>").attr("id", "takePhoto").on("click", (function() {
-                                                            n[0].paused ? (n[0].play(), c()("#saveImage").attr("disabled", !0), c()("#takePhoto span").text("Take Photo")) : (n[0].pause(), c()("#saveImage").removeAttr("disabled"), c()("#takePhoto span").text("Retry"))
-                                                        })).append(c()("<span/>").text("Take Photo"))), t.append(r), _e().modal({
+                                                        var r = s()("<div/>").attr("id", "videoControls");
+                                                        r.append(s()("<button/>").attr("id", "takePhoto").on("click", (function() {
+                                                            n[0].paused ? (n[0].play(), s()("#saveImage").attr("disabled", !0), s()("#takePhoto span").text("Take Photo")) : (n[0].pause(), s()("#saveImage").removeAttr("disabled"), s()("#takePhoto span").text("Retry"))
+                                                        })).append(s()("<span/>").text("Take Photo"))), t.append(r), _e().modal({
                                                             keyboard_manager: Jupyter.keyboard_manager,
                                                             title: "Take Photo",
                                                             open: function() {
-                                                                c()("#webcamDiv").bind("destroyed", (function() {
+                                                                s()("#webcamDiv").bind("destroyed", (function() {
                                                                     e.close()
                                                                 }))
                                                             },
                                                             body: t,
                                                             buttons: {
                                                                 "Save Image": {
                                                                     id: "saveImage",
                                                                     click: function() {
-                                                                        var t = c()("<canvas/>").attr("width", n[0].videoWidth).attr("height", n[0].videoHeight);
+                                                                        var t = s()("<canvas/>").attr("width", n[0].videoWidth).attr("height", n[0].videoHeight);
                                                                         t[0].getContext("2d").drawImage(n[0], 0, 0, n[0].videoWidth, n[0].videoHeight);
                                                                         var r = t[0].toDataURL("image/png"),
                                                                             o = e.model.getName("webcam", "png");
                                                                         e.model.setAttachment(o, r)
                                                                     }
                                                                 },
                                                                 Cancel: {}
@@ -5100,96 +5104,96 @@
                                                         e = Reflect.construct(r, arguments, o)
                                                     } else e = r.apply(this, arguments);
                                                     return xe(this, e)
                                                 });
 
                                                 function o(e, t) {
                                                     var n;
-                                                    return Se(this, o), (n = r.call(this)).cell = e, n.model = t, n.element = c()("<div/>").addClass("gallery-view"), t.registerObserver(Oe(n)), n
+                                                    return Se(this, o), (n = r.call(this)).cell = e, n.model = t, n.element = s()("<div/>").addClass("gallery-view"), t.registerObserver(Oe(n)), n
                                                 }
                                                 return Ce(o, [{
                                                     key: "notify",
                                                     value: function(e) {
-                                                        "delete" == e.type ? this.element.find(c()("#" + e.id)).remove() : "add" == e.type && this.addThumbnail(this.model.getAttachment(e.key))
+                                                        "delete" == e.type ? this.element.find(s()("#" + e.id)).remove() : "add" == e.type && this.addThumbnail(this.model.getAttachment(e.key))
                                                     }
                                                 }, {
                                                     key: "addThumbnail",
                                                     value: function(e) {
                                                         var t = this,
-                                                            n = c()("<div/>").addClass("gallery-item").attr("id", e.id),
-                                                            r = c()("<div/>").addClass("remove-file-modal").append(c()("<p/>").append("Are you sure you want to delete the file " + e.name + " ?")),
-                                                            o = c()("<i/>").addClass("fa fa-trash");
+                                                            n = s()("<div/>").addClass("gallery-item").attr("id", e.id),
+                                                            r = s()("<div/>").addClass("remove-file-modal").append(s()("<p/>").append("Are you sure you want to delete the file " + e.name + " ?")),
+                                                            o = s()("<i/>").addClass("fa fa-trash");
                                                         o.on("click", (function() {
                                                             _e().modal({
                                                                 body: r,
                                                                 buttons: {
                                                                     Delete: {
                                                                         class: "button-delete",
                                                                         click: function() {
                                                                             return t.model.removeAttachment(e.name)
                                                                         }
                                                                     },
                                                                     Cancel: {}
                                                                 }
                                                             })
                                                         })), n.append(o);
-                                                        var i = c()("<i/>").addClass("fa fa-search-plus").on("click", (function() {
+                                                        var i = s()("<i/>").addClass("fa fa-search-plus").on("click", (function() {
                                                             var t = document.createElement("a");
                                                             t.href = "data:" + e.type + ";base64," + e.data, t.target = "_blank", t.download = e.name, document.body.appendChild(t), t.click(), document.body.removeChild(t)
                                                         }));
                                                         n.append(i);
-                                                        var a = c()("<div/>").addClass("thumbnail"),
-                                                            s = c()("<div/>").addClass("caption");
-                                                        if (s.append(c()("<span/>").text(e.name)), e.type.startsWith("image")) {
+                                                        var a = s()("<div/>").addClass("thumbnail"),
+                                                            c = s()("<div/>").addClass("caption");
+                                                        if (c.append(s()("<span/>").text(e.name)), e.type.startsWith("image")) {
                                                             var l = new Image;
                                                             l.src = "data:" + e.type + ";base64," + e.data, a.append(l)
                                                         }
-                                                        n.append(a).append(s), this.element.append(n)
+                                                        n.append(a).append(c), this.element.append(n)
                                                     }
                                                 }, {
                                                     key: "getControls",
                                                     value: function() {
                                                         var e = this,
-                                                            t = c()("<div/>").addClass("attachment-controls");
-                                                        t.append(c()("<button/>").addClass("btn-e2x").append(c()("<i/>").addClass("fa fa-camera")).append("Webcam").on("click", (function() {
+                                                            t = s()("<div/>").addClass("attachment-controls");
+                                                        t.append(s()("<button/>").addClass("btn-e2x").append(s()("<i/>").addClass("fa fa-camera")).append("Webcam").on("click", (function() {
                                                             return new Pe(e.model).open()
                                                         })));
-                                                        var n = c()("<button/>").addClass("btn-e2x").addClass("upload-btn").append(c()("<i/>").addClass("fa fa-upload")).append("Upload").on("click", (function() {
-                                                            return c()("#upload-attachments")[0].click()
+                                                        var n = s()("<button/>").addClass("btn-e2x").addClass("upload-btn").append(s()("<i/>").addClass("fa fa-upload")).append("Upload").on("click", (function() {
+                                                            return s()("#upload-attachments")[0].click()
                                                         }));
-                                                        return n.append(c()("<input/>").attr("id", "upload-attachments").attr("type", "file").attr("accept", "application/pdf,image/*").attr("multiple", "multiple").on("change", (function() {
+                                                        return n.append(s()("<input/>").attr("id", "upload-attachments").attr("type", "file").attr("accept", "application/pdf,image/*").attr("multiple", "multiple").on("change", (function() {
                                                             return e.uploadFiles()
                                                         }))), t.append(n), t
                                                     }
                                                 }, {
                                                     key: "uploadFiles",
                                                     value: function() {
-                                                        var e = c()("#upload-attachments")[0],
+                                                        var e = s()("#upload-attachments")[0],
                                                             t = this;
                                                         Array.prototype.forEach.call(e.files, (function(e) {
                                                             var n = new FileReader;
                                                             n.readAsDataURL(e), n.onload = function() {
                                                                 var r = n.result,
                                                                     o = e.name;
                                                                 if (t.model.hasAttachment(o)) {
                                                                     var i = o.split(".")[0],
                                                                         a = o.replace(i + ".", ""),
-                                                                        c = t.model.getName(i, a);
-                                                                    confirm("A file with the name " + o + " already exists!\nDo you want to rename it to " + c + "?") && t.model.setAttachment(c, r)
+                                                                        s = t.model.getName(i, a);
+                                                                    confirm("A file with the name " + o + " already exists!\nDo you want to rename it to " + s + "?") && t.model.setAttachment(s, r)
                                                                 } else t.model.setAttachment(o, r)
                                                             }, n.onerror = function() {
                                                                 console.log(n.error)
                                                             }
                                                         }))
                                                     }
                                                 }, {
                                                     key: "open",
                                                     value: function() {
-                                                        var e = c()("<div/>").addClass("attachment-editor");
-                                                        this.element = c()("<div/>").addClass("gallery-view"), e.append(this.element), e.append(this.getControls());
+                                                        var e = s()("<div/>").addClass("attachment-editor");
+                                                        this.element = s()("<div/>").addClass("gallery-view"), e.append(this.element), e.append(this.getControls());
                                                         var t = this;
                                                         this.model.getAttachments().forEach((function(e) {
                                                             return t.addThumbnail(e)
                                                         })), _e().modal({
                                                             keyboard_manager: Jupyter.keyboard_manager,
                                                             title: "Attachment Editor",
                                                             body: e
@@ -5310,23 +5314,23 @@
                                                         var r;
                                                         return Ge(this, n), (r = t.call(this, e, "attachments")).model = new Ye(e), r.view = new Be(e, r.model), r
                                                     }
                                                     return Ze(n, [{
                                                         key: "get_attachment_button",
                                                         value: function() {
                                                             var e = this;
-                                                            return c()("<button>").attr("type", "button").addClass("edit_attachments btn-e2x").on("click", (function() {
+                                                            return s()("<button>").attr("type", "button").addClass("edit_attachments btn-e2x").on("click", (function() {
                                                                 e.view.open()
                                                             })).append("Add Files / Images")
                                                         }
                                                     }, {
                                                         key: "render",
                                                         value: function() {
                                                             this.cell.render_force();
-                                                            var e = c()(this.cell.element).find(".rendered_html");
+                                                            var e = s()(this.cell.element).find(".rendered_html");
                                                             e.find(".edit_attachments").length < 1 && e.append(this.get_attachment_button()), this.render_grader_settings()
                                                         }
                                                     }]), n
                                                 }(g),
                                                 diagram: ge
                                             }
                                     })(), e.exports = i
@@ -5379,25 +5383,25 @@
                         o.r(i), o.d(i, {
                             initialize_cell_extension: () => Q
                         });
                         var e = o(761),
                             t = o.n(e);
                         const r = n(315);
                         var a = o(355);
-                        const c = n(767);
-                        var s = o.n(c);
+                        const s = n(767);
+                        var c = o.n(s);
                         r.MarkdownCell.prototype.render, r.MarkdownCell.prototype.unrender;
                         var l = o(86),
                             u = o.n(l);
                         const d = n(290);
                         var f = o.n(d);
-                        const p = n(140);
-                        var h = !1,
+                        const h = n(140);
+                        var p = !1,
                             m = r.MarkdownCell.prototype.render,
-                            y = p.Notebook.prototype.to_markdown,
+                            y = h.Notebook.prototype.to_markdown,
                             v = r.TextCell.prototype.toJSON,
                             g = r.MarkdownCell.prototype.unrender;
 
                         function b() {
                             var e = u().notebook.get_cells();
                             for (var t in e) {
                                 var n = e[t];
@@ -5426,15 +5430,15 @@
                                 }
                             }, r.MarkdownCell.prototype.unsafe_render = function() {
                                 this.drag_counter = 0, this.inner_cell.removeClass("dropzone");
                                 var e = r.TextCell.prototype.render.apply(this);
                                 if (e) {
                                     var t = this,
                                         n = this.get_text();
-                                    "" === n && (n = this.placeholder), s().render(n, {
+                                    "" === n && (n = this.placeholder), c().render(n, {
                                         with_math: !0,
                                         clean_tables: !0,
                                         sanitize: !1
                                     }, (function(e, n) {
                                         (n = $(n)).find(":header").addBack(":header").each((function(e, n) {
                                             var r = (n = $(n)).text().replace(/ /g, "-");
                                             n.attr("id", r), n.append($("<a/>").addClass("anchor-link").attr("href", "#" + r).text("¶").on("click", (function() {
@@ -5453,50 +5457,50 @@
                                             cell: t
                                         })
                                     }))
                                 }
                                 return e
                             }, r.TextCell.prototype.toJSON = function() {
                                 return "attachments" == a.utils.get_e2x_cell_type(this) ? (arguments[0] = !1, v.apply(this, arguments)) : v.apply(this, arguments)
-                            }, p.Notebook.prototype.to_markdown = function() {
+                            }, h.Notebook.prototype.to_markdown = function() {
                                 y.apply(this, arguments);
                                 var e = this.get_cell(arguments[0]);
                                 e.unrender_force(), e.render()
                             }, r.MarkdownCell.prototype.unrender_force = g, r.MarkdownCell.prototype.unrender = function() {
                                 a.utils.is_e2x(this) || g.apply(this, arguments)
                             }, r.MarkdownCell.prototype.render_force = m, r.MarkdownCell.prototype.render = function() {
                                 var e = a.utils.get_e2x_cell_type(this);
                                 if (a.cells.hasOwnProperty(e)) {
                                     var t = new a.cells[e](this);
-                                    t.edit_mode = h, t.render()
+                                    t.edit_mode = p, t.render()
                                 } else m.apply(this, arguments)
-                            }, u().notebook.metadata.hasOwnProperty("celltoolbar") && "Create Assignment" === u().notebook.metadata.celltoolbar && (h = !0), f().on("preset_activated.CellToolbar", (function(e, t) {
-                                h = "Create Assignment" == t.name, b()
+                            }, u().notebook.metadata.hasOwnProperty("celltoolbar") && "Create Assignment" === u().notebook.metadata.celltoolbar && (p = !0), f().on("preset_activated.CellToolbar", (function(e, t) {
+                                p = "Create Assignment" == t.name, b()
                             })), f().on("global_hide.CellToolbar", (function(e, t) {
-                                h = !1, b()
+                                p = !1, b()
                             })), b()
                         }
                         G.styleTagTransform = B(), G.setAttributes = j(), G.insert = E().bind(null, "head"), G.domAPI = x(), G.insertStyleElement = A(), w()(T.Z, G), T.Z && T.Z.locals && T.Z.locals
                     })(), e.exports = i
                 })()
             },
             703: (e, t, n) => {
                 (() => {
                     var t = {
                             19: (e, t, n) => {
                                 "use strict";
                                 n.d(t, {
-                                    Z: () => c
+                                    Z: () => s
                                 });
                                 var r = n(601),
                                     o = n.n(r),
                                     i = n(609),
                                     a = n.n(i)()(o());
                                 a.push([e.id, "#e2x-menubar .e2x-submit {\n  background-color: var(--orange);\n  border: 2px solid var(--orange-border);\n}\n\n#e2x-menubar .e2x-submit i {\n  padding-left: 0.5em;\n}\n\n#submitting {\n  position: fixed;\n  top: 0;\n  left: 0;\n  width: 100%;\n  height: 100%;\n  background-color: rgba(0, 0, 0, 0.5); /* Transparent black */\n  display: flex;\n  justify-content: center;\n  align-items: center;\n  z-index: 9999;\n}\n\n#submitting_box {\n  background-color: white;\n  padding: 20px;\n  border-radius: 10px;\n  text-align: center;\n  box-shadow: 0 0 10px rgba(0, 0, 0, 0.5); /* Shadow effect */\n}\n\n#submit_spinner {\n  margin: auto;\n}\n\n#submitting p {\n  margin-top: 2em;\n  color: black;\n  text-align: center;\n  font-weight: bold;\n  font-size: 1.5em;\n}\n\n#hashcode_label {\n  font-weight: bold;\n  color: darkgreen;\n}\n", ""]);
-                                const c = a
+                                const s = a
                             },
                             609: e => {
                                 "use strict";
                                 e.exports = function(e) {
                                     var t = [];
                                     return t.toString = function() {
                                         return this.map((function(t) {
@@ -5506,17 +5510,17 @@
                                         })).join("")
                                     }, t.i = function(e, n, r, o, i) {
                                         "string" == typeof e && (e = [
                                             [null, e, void 0]
                                         ]);
                                         var a = {};
                                         if (r)
-                                            for (var c = 0; c < this.length; c++) {
-                                                var s = this[c][0];
-                                                null != s && (a[s] = !0)
+                                            for (var s = 0; s < this.length; s++) {
+                                                var c = this[s][0];
+                                                null != c && (a[c] = !0)
                                             }
                                         for (var l = 0; l < e.length; l++) {
                                             var u = [].concat(e[l]);
                                             r && a[u[0]] || (void 0 !== i && (void 0 === u[5] || (u[1] = "@layer".concat(u[5].length > 0 ? " ".concat(u[5]) : "", " {").concat(u[1], "}")), u[5] = i), n && (u[2] ? (u[1] = "@media ".concat(u[2], " {").concat(u[1], "}"), u[2] = n) : u[2] = n), o && (u[4] ? (u[1] = "@supports (".concat(u[4], ") {").concat(u[1], "}"), u[4] = o) : u[4] = "".concat(o)), t.push(u))
                                         }
                                     }, t
                                 }
@@ -5536,34 +5540,34 @@
                                         if (t[r].identifier === e) {
                                             n = r;
                                             break
                                         } return n
                                 }
 
                                 function r(e, r) {
-                                    for (var i = {}, a = [], c = 0; c < e.length; c++) {
-                                        var s = e[c],
-                                            l = r.base ? s[0] + r.base : s[0],
+                                    for (var i = {}, a = [], s = 0; s < e.length; s++) {
+                                        var c = e[s],
+                                            l = r.base ? c[0] + r.base : c[0],
                                             u = i[l] || 0,
                                             d = "".concat(l, " ").concat(u);
                                         i[l] = u + 1;
                                         var f = n(d),
-                                            p = {
-                                                css: s[1],
-                                                media: s[2],
-                                                sourceMap: s[3],
-                                                supports: s[4],
-                                                layer: s[5]
+                                            h = {
+                                                css: c[1],
+                                                media: c[2],
+                                                sourceMap: c[3],
+                                                supports: c[4],
+                                                layer: c[5]
                                             };
-                                        if (-1 !== f) t[f].references++, t[f].updater(p);
+                                        if (-1 !== f) t[f].references++, t[f].updater(h);
                                         else {
-                                            var h = o(p, r);
-                                            r.byIndex = c, t.splice(c, 0, {
+                                            var p = o(h, r);
+                                            r.byIndex = s, t.splice(s, 0, {
                                                 identifier: d,
-                                                updater: h,
+                                                updater: p,
                                                 references: 1
                                             })
                                         }
                                         a.push(d)
                                     }
                                     return a
                                 }
@@ -5579,22 +5583,22 @@
                                         }
                                 }
                                 e.exports = function(e, o) {
                                     var i = r(e = e || [], o = o || {});
                                     return function(e) {
                                         e = e || [];
                                         for (var a = 0; a < i.length; a++) {
-                                            var c = n(i[a]);
-                                            t[c].references--
+                                            var s = n(i[a]);
+                                            t[s].references--
                                         }
-                                        for (var s = r(e, o), l = 0; l < i.length; l++) {
+                                        for (var c = r(e, o), l = 0; l < i.length; l++) {
                                             var u = n(i[l]);
                                             0 === t[u].references && (t[u].updater(), t.splice(u, 1))
                                         }
-                                        i = s
+                                        i = c
                                     }
                                 }
                             },
                             793: e => {
                                 "use strict";
                                 var t = {};
                                 e.exports = function(e, n) {
@@ -5739,22 +5743,22 @@
                             },
                             237: (e, t, n) => {
                                 (() => {
                                     "use strict";
                                     var t = {
                                             616: (e, t, n) => {
                                                 n.d(t, {
-                                                    Z: () => c
+                                                    Z: () => s
                                                 });
                                                 var r = n(601),
                                                     o = n.n(r),
                                                     i = n(609),
                                                     a = n.n(i)()(o());
                                                 a.push([e.id, ":root {\n  --blue: #eaf4f7;\n  --blue-border: #dae4e7;\n  --blue-hover: #c4dde6;\n  --light-blue: #f8fbfc;\n  --orange: #f37726;\n  --orange-border: #f3631d;\n}\n\n#e2x-menubar {\n  display: flex;\n  background-color: var(--blue);\n  line-height: 3em;\n  border: 1px solid var(--blue-border);\n}\n\n#e2x-menubar a {\n  text-decoration: none;\n  color: black;\n}\n\n.e2x-badge {\n  display: inline-block;\n  padding: 0 1em 0 1em;\n  border-right: 1px solid var(--blue-border);\n}\n\n.e2x-divider {\n  display: inline-block;\n  height: 3em;\n  width: 0px;\n  border-right: 1px solid var(--blue-border);\n}\n\n.e2x-spacer {\n  flex-grow: 1;\n}\n\n#e2x-menubar button,\n.e2x-button {\n  display: inline-block;\n  padding: 0 1em 0 1em;\n  height: 3em;\n  border: none;\n  background-color: var(--blue);\n  cursor: pointer;\n}\n\n#e2x-menubar button:hover,\n.e2x-button:hover {\n  color: black;\n  background-color: var(--blue-hover);\n}\n\n.e2x-dropdown {\n  position: relative;\n  display: inline-block;\n}\n\n.e2x-dropdown-content {\n  position: absolute;\n  display: none;\n  list-style-type: none;\n  background-color: var(--light-blue);\n  text-decoration: none;\n  box-shadow: 0 6px 12px rgba(0, 0, 0, 0.15);\n  padding: 0.5em 0 0.5em 0;\n  min-width: 9em;\n  border: 1px solid rgba(0, 0, 0, 0.15);\n}\n\n.e2x-dropdown:hover .e2x-dropdown-content {\n  display: block;\n}\n\n.e2x-dropdown:hover .e2x-button {\n  background-color: var(--blue-hover);\n}\n\n.e2x-dropdown-item:hover {\n  background-color: var(--blue);\n}\n\n.e2x-dropdown-item {\n  line-height: 2em;\n  padding: 0 0.5em 0 0.5em;\n  white-space: nowrap;\n  cursor: pointer;\n}\n\n#save-notbook i {\n  scale: 1.5;\n}\n", ""]);
-                                                const c = a
+                                                const s = a
                                             },
                                             609: e => {
                                                 e.exports = function(e) {
                                                     var t = [];
                                                     return t.toString = function() {
                                                         return this.map((function(t) {
                                                             var n = "",
@@ -5763,17 +5767,17 @@
                                                         })).join("")
                                                     }, t.i = function(e, n, r, o, i) {
                                                         "string" == typeof e && (e = [
                                                             [null, e, void 0]
                                                         ]);
                                                         var a = {};
                                                         if (r)
-                                                            for (var c = 0; c < this.length; c++) {
-                                                                var s = this[c][0];
-                                                                null != s && (a[s] = !0)
+                                                            for (var s = 0; s < this.length; s++) {
+                                                                var c = this[s][0];
+                                                                null != c && (a[c] = !0)
                                                             }
                                                         for (var l = 0; l < e.length; l++) {
                                                             var u = [].concat(e[l]);
                                                             r && a[u[0]] || (void 0 !== i && (void 0 === u[5] || (u[1] = "@layer".concat(u[5].length > 0 ? " ".concat(u[5]) : "", " {").concat(u[1], "}")), u[5] = i), n && (u[2] ? (u[1] = "@media ".concat(u[2], " {").concat(u[1], "}"), u[2] = n) : u[2] = n), o && (u[4] ? (u[1] = "@supports (".concat(u[4], ") {").concat(u[1], "}"), u[4] = o) : u[4] = "".concat(o)), t.push(u))
                                                         }
                                                     }, t
                                                 }
@@ -5791,34 +5795,34 @@
                                                         if (t[r].identifier === e) {
                                                             n = r;
                                                             break
                                                         } return n
                                                 }
 
                                                 function r(e, r) {
-                                                    for (var i = {}, a = [], c = 0; c < e.length; c++) {
-                                                        var s = e[c],
-                                                            l = r.base ? s[0] + r.base : s[0],
+                                                    for (var i = {}, a = [], s = 0; s < e.length; s++) {
+                                                        var c = e[s],
+                                                            l = r.base ? c[0] + r.base : c[0],
                                                             u = i[l] || 0,
                                                             d = "".concat(l, " ").concat(u);
                                                         i[l] = u + 1;
                                                         var f = n(d),
-                                                            p = {
-                                                                css: s[1],
-                                                                media: s[2],
-                                                                sourceMap: s[3],
-                                                                supports: s[4],
-                                                                layer: s[5]
+                                                            h = {
+                                                                css: c[1],
+                                                                media: c[2],
+                                                                sourceMap: c[3],
+                                                                supports: c[4],
+                                                                layer: c[5]
                                                             };
-                                                        if (-1 !== f) t[f].references++, t[f].updater(p);
+                                                        if (-1 !== f) t[f].references++, t[f].updater(h);
                                                         else {
-                                                            var h = o(p, r);
-                                                            r.byIndex = c, t.splice(c, 0, {
+                                                            var p = o(h, r);
+                                                            r.byIndex = s, t.splice(s, 0, {
                                                                 identifier: d,
-                                                                updater: h,
+                                                                updater: p,
                                                                 references: 1
                                                             })
                                                         }
                                                         a.push(d)
                                                     }
                                                     return a
                                                 }
@@ -5834,22 +5838,22 @@
                                                         }
                                                 }
                                                 e.exports = function(e, o) {
                                                     var i = r(e = e || [], o = o || {});
                                                     return function(e) {
                                                         e = e || [];
                                                         for (var a = 0; a < i.length; a++) {
-                                                            var c = n(i[a]);
-                                                            t[c].references--
+                                                            var s = n(i[a]);
+                                                            t[s].references--
                                                         }
-                                                        for (var s = r(e, o), l = 0; l < i.length; l++) {
+                                                        for (var c = r(e, o), l = 0; l < i.length; l++) {
                                                             var u = n(i[l]);
                                                             0 === t[u].references && (t[u].updater(), t.splice(u, 1))
                                                         }
-                                                        i = s
+                                                        i = c
                                                     }
                                                 }
                                             },
                                             793: e => {
                                                 var t = {};
                                                 e.exports = function(e, n) {
                                                     var r = function(e) {
@@ -5946,27 +5950,27 @@
                                         o.r(i), o.d(i, {
                                             Menubar: () => b
                                         });
                                         const e = n(761);
                                         var t = o.n(e),
                                             r = o(62),
                                             a = o.n(r),
-                                            c = o(36),
-                                            s = o.n(c),
+                                            s = o(36),
+                                            c = o.n(s),
                                             l = o(793),
                                             u = o.n(l),
                                             d = o(892),
                                             f = o.n(d),
-                                            p = o(173),
-                                            h = o.n(p),
+                                            h = o(173),
+                                            p = o.n(h),
                                             m = o(464),
                                             y = o.n(m),
                                             v = o(616),
                                             g = {};
-                                        g.styleTagTransform = y(), g.setAttributes = f(), g.insert = u().bind(null, "head"), g.domAPI = s(), g.insertStyleElement = h(), a()(v.Z, g), v.Z && v.Z.locals && v.Z.locals;
+                                        g.styleTagTransform = y(), g.setAttributes = f(), g.insert = u().bind(null, "head"), g.domAPI = c(), g.insertStyleElement = p(), a()(v.Z, g), v.Z && v.Z.locals && v.Z.locals;
                                         class b {
                                             constructor() {
                                                 this.element = t()("<div/>").attr("id", "e2x-menubar").append(t()("<span/>").text("e²x").addClass("e2x-badge"))
                                             }
                                             hide_maintoolbar() {
                                                 t()("#maintoolbar-container").hide()
                                             }
@@ -6044,21 +6048,21 @@
                         o.r(i), o.d(i, {
                             ExamMenubar: () => C
                         });
                         var e = o(761),
                             t = o.n(e);
                         const r = n(527);
                         var a = o.n(r),
-                            c = o(237),
-                            s = o(804);
+                            s = o(237),
+                            c = o(804);
                         const l = n(30);
                         var u = o.n(l);
                         const d = n(566);
                         var f = o.n(d);
-                        class p {
+                        class h {
                             constructor() {
                                 this.courses = [], this.assignment = void 0, this.base_url = a().notebook.base_url, this.name = a().notebook.notebook_name.split(".ipynb")[0];
                                 let e = window.location.href.split("/");
                                 this.assignment_id = e[e.length - 2], this.get_courses()
                             }
                             get_courses() {
                                 let e = this,
@@ -6169,45 +6173,45 @@
                                             },
                                             class: "btn-success"
                                         }
                                     }
                                 })
                             }
                         }
-                        var h = o(62),
-                            m = o.n(h),
+                        var p = o(62),
+                            m = o.n(p),
                             y = o(36),
                             v = o.n(y),
                             g = o(793),
                             b = o.n(g),
                             _ = o(892),
                             w = o.n(_),
                             k = o(173),
                             x = o.n(k),
                             O = o(464),
                             E = o.n(O),
                             S = o(19),
                             j = {};
                         j.styleTagTransform = E(), j.setAttributes = w(), j.insert = b().bind(null, "head"), j.domAPI = v(), j.insertStyleElement = x(), m()(S.Z, j), S.Z && S.Z.locals && S.Z.locals;
-                        class C extends c.Menubar {
+                        class C extends s.Menubar {
                             constructor() {
-                                super(), this.submit = new p
+                                super(), this.submit = new h
                             }
                             add_kernel_indiciator() {
                                 this.element.append(t()("<span/>").css("padding", "0 1em 0 1em").append(t()(".kernel_indicator_name").css("padding-left", ".5em")).append(t()("#kernel_indicator_icon").css("padding-left", ".5em")))
                             }
                             add_help() {
                                 let e = this,
                                     n = [];
-                                s.requests.get((0, s.urlJoin)(a().notebook.base_url, "e2x/help/api/files")).then((e => {
+                                c.requests.get((0, c.urlJoin)(a().notebook.base_url, "e2x/help/api/files")).then((e => {
                                     e.forEach((function(e) {
                                         n.push({
                                             label: e[0],
                                             callback: function() {
-                                                window.open((0, s.urlJoin)(a().notebook.base_url, "e2x/help/static/", e[1]), "_blank")
+                                                window.open((0, c.urlJoin)(a().notebook.base_url, "e2x/help/static/", e[1]), "_blank")
                                             }
                                         })
                                     }))
                                 })).finally((() => {
                                     n.length > 0 && e.add_dropdown("help", "Additional Resources", n), e.element.append(t()("<div/>").addClass("e2x-button e2x-submit").on("click", (function() {
                                         e.submit.prepare_submit()
                                     })).append("Submit").append(t()("<i/>").addClass("fa fa-paper-plane")))
@@ -6355,49 +6359,49 @@
                                             is_invalid: () => G,
                                             is_locked: () => x,
                                             is_nbgrader: () => l,
                                             is_solution: () => v,
                                             is_task: () => w,
                                             is_test: () => A,
                                             nbgrader_schema_version: () => a,
-                                            randomString: () => c,
-                                            remove_nbgrader_field: () => h,
+                                            randomString: () => s,
+                                            remove_nbgrader_field: () => p,
                                             remove_nbgrader_metadata: () => u,
                                             set_grade: () => _,
                                             set_grade_id: () => C,
                                             set_locked: () => O,
-                                            set_nbgrader_field: () => p,
+                                            set_nbgrader_field: () => h,
                                             set_points: () => S,
                                             set_schema_version: () => y,
                                             set_solution: () => g,
                                             set_task: () => k,
                                             to_description: () => T,
-                                            to_float: () => s,
+                                            to_float: () => c,
                                             to_test: () => P
                                         });
                                         var t = {};
                                         o.r(t), o.d(t, {
                                             add_shortcut: () => W,
                                             disable_add_cell_on_execute: () => Y,
                                             remove_shortcuts: () => I
                                         });
                                         var r = {};
                                         o.r(r), o.d(r, {
                                             add_username: () => R
                                         });
                                         const a = 3;
 
-                                        function c(e) {
+                                        function s(e) {
                                             let t, n = "",
                                                 r = "abcdef0123456789";
                                             for (t = 0; t < e; t++) n += r[Math.floor(Math.random() * r.length)];
                                             return n
                                         }
 
-                                        function s(e) {
+                                        function c(e) {
                                             return void 0 === e || "" === e ? 0 : parseFloat(e)
                                         }
 
                                         function l(e) {
                                             return e.metadata.hasOwnProperty("nbgrader")
                                         }
 
@@ -6409,76 +6413,76 @@
                                             l(e) || (e.metadata.nbgrader = {})
                                         }
 
                                         function f(e, t, n = {}) {
                                             return l(e) && e.metadata.nbgrader[t] || n
                                         }
 
-                                        function p(e, t, n) {
+                                        function h(e, t, n) {
                                             l(e) || (e.metadata.nbgrader = {}), e.metadata.nbgrader[t] = n
                                         }
 
-                                        function h(e, t) {
+                                        function p(e, t) {
                                             l(e) && e.metadata.nbgrader.hasOwnProperty(t) && delete e.metadata.nbgrader[t]
                                         }
 
                                         function m(e) {
                                             if (l(e)) return void 0 === f(e, "schema_version") ? 0 : f(e, "schema_version")
                                         }
 
                                         function y(e) {
-                                            l(e) || d(e), p(e, "schema_version", a)
+                                            l(e) || d(e), h(e, "schema_version", a)
                                         }
 
                                         function v(e) {
                                             return f(e, "solution", !1)
                                         }
 
                                         function g(e, t) {
-                                            p(e, "solution", t)
+                                            h(e, "solution", t)
                                         }
 
                                         function b(e) {
                                             return f(e, "grade", !1)
                                         }
 
                                         function _(e, t) {
-                                            p(e, "grade", t)
+                                            h(e, "grade", t)
                                         }
 
                                         function w(e) {
                                             return f(e, "task", !1)
                                         }
 
                                         function k(e, t) {
-                                            p(e, "task", t)
+                                            h(e, "task", t)
                                         }
 
                                         function x(e) {
                                             return f(e, "locked", !1)
                                         }
 
                                         function O(e, t) {
-                                            p(e, "locked", t)
+                                            h(e, "locked", t)
                                         }
 
                                         function E(e) {
-                                            return s(f(e, "points", 0))
+                                            return c(f(e, "points", 0))
                                         }
 
                                         function S(e, t) {
-                                            p(e, "points", Math.max(0, s(t)))
+                                            h(e, "points", Math.max(0, c(t)))
                                         }
 
                                         function j(e) {
-                                            return f(e, "grade_id", "cell-" + c(16))
+                                            return f(e, "grade_id", "cell-" + s(16))
                                         }
 
                                         function C(e, t) {
-                                            p(e, "grade_id", t)
+                                            h(e, "grade_id", t)
                                         }
 
                                         function A(e) {
                                             return b(e) && x(e) && !v(e)
                                         }
 
                                         function P(e) {
@@ -6510,15 +6514,17 @@
                                             throw new Error("Mode needs to be either 'command' or 'edit'")
                                         }
 
                                         function I(e, ...t) {
                                             const n = M(e);
                                             for (const r of t) try {
                                                 n.remove_shortcut(r)
-                                            } catch (e) {}
+                                            } catch (t) {
+                                                console.log("Error removing shortcut", r, "from", e, "mode:", t.message)
+                                            }
                                         }
 
                                         function W(e, t, n, r, o = "zz") {
                                             M(e).add_shortcut(t, {
                                                 help: r,
                                                 help_index: o,
                                                 handler: n
@@ -6532,15 +6538,15 @@
                                                 else {
                                                     let t = this.get_selected_cell();
                                                     e = this.find_cell_index(t), t.execute()
                                                 }
                                                 e = Math.min(e + 1, this.ncells() - 1), this.select(e), this.focus_cell()
                                             };
                                             const e = ["alt-enter", "shift-enter"];
-                                            I("edit", e), I("command", e);
+                                            I("edit", ...e), I("command", ...e);
                                             const t = "run cell",
                                                 n = function(e) {
                                                     return J().notebook.execute_cell_and_select_below_without_insert(), !1
                                                 };
                                             for (const r of e) W("edit", r, n, t), W("command", r, n, t)
                                         }
                                         var N = o(804);
@@ -6599,33 +6605,33 @@
                         o.r(i), o.d(i, {
                             patch_assignment_notebook: () => Z
                         });
                         const e = n(404);
                         var t = o.n(e),
                             r = o(86),
                             a = o.n(r);
-                        const c = n(566);
-                        var s = o.n(c),
+                        const s = n(566);
+                        var c = o.n(s),
                             l = o(426),
                             u = o(851);
                         const d = n(425),
                             f = u.Notebook.prototype.to_code,
-                            p = u.Notebook.prototype.to_markdown,
-                            h = u.Notebook.prototype.to_raw,
+                            h = u.Notebook.prototype.to_markdown,
+                            p = u.Notebook.prototype.to_raw,
                             m = u.Notebook.prototype.move_cell_down,
                             y = u.Notebook.prototype.move_selection_down,
                             v = u.Notebook.prototype.move_cell_up,
                             g = u.Notebook.prototype.move_selection_up,
                             b = u.Notebook.prototype.paste_cell_replace,
                             _ = u.Notebook.prototype.paste_cell_above,
                             w = u.Notebook.prototype.paste_cell_below;
 
                         function k() {
                             let e = t()("<div/>").append(t()("<span/>").text("You can not change the type of a cell that belongs to the assignment!"));
-                            s().modal({
+                            c().modal({
                                 keyboard_manager: a().keyboard_manager,
                                 title: "Can not change cell type",
                                 body: e,
                                 buttons: {
                                     OK: {}
                                 }
                             })
@@ -6640,15 +6646,15 @@
                         }
 
                         function O(e) {
                             let n = !1;
                             return e.some((function(e) {
                                 return l.utils.is_nbgrader(e) && (n = !0, function() {
                                     let e = t()("<div/>").append(t()("<span/>").text("At least one of the selected cells belongs to the assignment and can not be moved!"));
-                                    s().modal({
+                                    c().modal({
                                         keyboard_manager: a().keyboard_manager,
                                         title: "Can not move cells",
                                         body: e,
                                         buttons: {
                                             OK: {}
                                         }
                                     })
@@ -6657,19 +6663,19 @@
                         }
 
                         function E() {
                             l.utils.is_nbgrader(a().notebook.get_cell(arguments[0])) ? k() : f.apply(this, arguments)
                         }
 
                         function S() {
-                            l.utils.is_nbgrader(a().notebook.get_cell(arguments[0])) ? k() : p.apply(this, arguments)
+                            l.utils.is_nbgrader(a().notebook.get_cell(arguments[0])) ? k() : h.apply(this, arguments)
                         }
 
                         function j() {
-                            l.utils.is_nbgrader(a().notebook.get_cell(arguments[0])) ? k() : h.apply(this, arguments)
+                            l.utils.is_nbgrader(a().notebook.get_cell(arguments[0])) ? k() : p.apply(this, arguments)
                         }
 
                         function C() {
                             let e = arguments[0];
                             void 0 === e ? a().notebook.move_selection_down() : O([a().notebook.get_cell(e)]) && m.apply(this, arguments)
                         }
 
@@ -6836,49 +6842,49 @@
                                             is_invalid: () => G,
                                             is_locked: () => x,
                                             is_nbgrader: () => l,
                                             is_solution: () => v,
                                             is_task: () => w,
                                             is_test: () => A,
                                             nbgrader_schema_version: () => a,
-                                            randomString: () => c,
-                                            remove_nbgrader_field: () => h,
+                                            randomString: () => s,
+                                            remove_nbgrader_field: () => p,
                                             remove_nbgrader_metadata: () => u,
                                             set_grade: () => _,
                                             set_grade_id: () => C,
                                             set_locked: () => O,
-                                            set_nbgrader_field: () => p,
+                                            set_nbgrader_field: () => h,
                                             set_points: () => S,
                                             set_schema_version: () => y,
                                             set_solution: () => g,
                                             set_task: () => k,
                                             to_description: () => T,
-                                            to_float: () => s,
+                                            to_float: () => c,
                                             to_test: () => P
                                         });
                                         var t = {};
                                         o.r(t), o.d(t, {
                                             add_shortcut: () => W,
                                             disable_add_cell_on_execute: () => Y,
                                             remove_shortcuts: () => I
                                         });
                                         var r = {};
                                         o.r(r), o.d(r, {
                                             add_username: () => R
                                         });
                                         const a = 3;
 
-                                        function c(e) {
+                                        function s(e) {
                                             let t, n = "",
                                                 r = "abcdef0123456789";
                                             for (t = 0; t < e; t++) n += r[Math.floor(Math.random() * r.length)];
                                             return n
                                         }
 
-                                        function s(e) {
+                                        function c(e) {
                                             return void 0 === e || "" === e ? 0 : parseFloat(e)
                                         }
 
                                         function l(e) {
                                             return e.metadata.hasOwnProperty("nbgrader")
                                         }
 
@@ -6890,76 +6896,76 @@
                                             l(e) || (e.metadata.nbgrader = {})
                                         }
 
                                         function f(e, t, n = {}) {
                                             return l(e) && e.metadata.nbgrader[t] || n
                                         }
 
-                                        function p(e, t, n) {
+                                        function h(e, t, n) {
                                             l(e) || (e.metadata.nbgrader = {}), e.metadata.nbgrader[t] = n
                                         }
 
-                                        function h(e, t) {
+                                        function p(e, t) {
                                             l(e) && e.metadata.nbgrader.hasOwnProperty(t) && delete e.metadata.nbgrader[t]
                                         }
 
                                         function m(e) {
                                             if (l(e)) return void 0 === f(e, "schema_version") ? 0 : f(e, "schema_version")
                                         }
 
                                         function y(e) {
-                                            l(e) || d(e), p(e, "schema_version", a)
+                                            l(e) || d(e), h(e, "schema_version", a)
                                         }
 
                                         function v(e) {
                                             return f(e, "solution", !1)
                                         }
 
                                         function g(e, t) {
-                                            p(e, "solution", t)
+                                            h(e, "solution", t)
                                         }
 
                                         function b(e) {
                                             return f(e, "grade", !1)
                                         }
 
                                         function _(e, t) {
-                                            p(e, "grade", t)
+                                            h(e, "grade", t)
                                         }
 
                                         function w(e) {
                                             return f(e, "task", !1)
                                         }
 
                                         function k(e, t) {
-                                            p(e, "task", t)
+                                            h(e, "task", t)
                                         }
 
                                         function x(e) {
                                             return f(e, "locked", !1)
                                         }
 
                                         function O(e, t) {
-                                            p(e, "locked", t)
+                                            h(e, "locked", t)
                                         }
 
                                         function E(e) {
-                                            return s(f(e, "points", 0))
+                                            return c(f(e, "points", 0))
                                         }
 
                                         function S(e, t) {
-                                            p(e, "points", Math.max(0, s(t)))
+                                            h(e, "points", Math.max(0, c(t)))
                                         }
 
                                         function j(e) {
-                                            return f(e, "grade_id", "cell-" + c(16))
+                                            return f(e, "grade_id", "cell-" + s(16))
                                         }
 
                                         function C(e, t) {
-                                            p(e, "grade_id", t)
+                                            h(e, "grade_id", t)
                                         }
 
                                         function A(e) {
                                             return b(e) && x(e) && !v(e)
                                         }
 
                                         function P(e) {
@@ -6989,17 +6995,19 @@
                                             if ("command" === e) return J().keyboard_manager.command_shortcuts;
                                             if ("edit" === e) return J().keyboard_manager.edit_shortcuts;
                                             throw new Error("Mode needs to be either 'command' or 'edit'")
                                         }
 
                                         function I(e, ...t) {
                                             const n = M(e);
-                                            for (const e of t) try {
-                                                n.remove_shortcut(e)
-                                            } catch (e) {}
+                                            for (const r of t) try {
+                                                n.remove_shortcut(r)
+                                            } catch (t) {
+                                                console.log("Error removing shortcut", r, "from", e, "mode:", t.message)
+                                            }
                                         }
 
                                         function W(e, t, n, r, o = "zz") {
                                             M(e).add_shortcut(t, {
                                                 help: r,
                                                 help_index: o,
                                                 handler: n
@@ -7013,15 +7021,15 @@
                                                 else {
                                                     let t = this.get_selected_cell();
                                                     e = this.find_cell_index(t), t.execute()
                                                 }
                                                 e = Math.min(e + 1, this.ncells() - 1), this.select(e), this.focus_cell()
                                             };
                                             const e = ["alt-enter", "shift-enter"];
-                                            I("edit", e), I("command", e);
+                                            I("edit", ...e), I("command", ...e);
                                             const t = "run cell",
                                                 n = function(e) {
                                                     return J().notebook.execute_cell_and_select_below_without_insert(), !1
                                                 };
                                             for (const r of e) W("edit", r, n, t), W("command", r, n, t)
                                         }
                                         var N = o(804);
@@ -7074,16 +7082,18 @@
                         "use strict";
                         o.r(i), o.d(i, {
                             disable_shortcuts: () => t
                         });
                         var e = o(426);
 
                         function t() {
-                            const t = ["x", "c", "v", "a", "b", "shift-v", "shift-m", "y", "m", "r", "ctrl-shift-f", "ctrl-shift-p", "p", "d,d"];
-                            e.shortcuts.remove_shortcuts("command", t), e.shortcuts.remove_shortcuts("edit", t), e.shortcuts.remove_shortcuts("command", "crtl-v"), e.shortcuts.disable_add_cell_on_execute(), e.shortcuts.add_shortcut("command", "ctrl-v", (function(e) {
+                            const t = ["x", "c", "v", "a", "b", "shift-v", "shift-m", "y", "m", "r", "ctrl-shift-f", "ctrl-shift-p", "p", "d,d"],
+                                n = ["command", "edit"];
+                            for (let r of n) e.shortcuts.remove_shortcuts(r, ...t);
+                            e.shortcuts.remove_shortcuts("command", "crtl-v"), e.shortcuts.disable_add_cell_on_execute(), e.shortcuts.add_shortcut("command", "ctrl-v", (function(e) {
                                 return !1
                             }), "no action")
                         }
                     })(), e.exports = i
                 })()
             },
             426: (e, t, n) => {
@@ -7213,49 +7223,49 @@
                             is_invalid: () => G,
                             is_locked: () => x,
                             is_nbgrader: () => l,
                             is_solution: () => v,
                             is_task: () => w,
                             is_test: () => A,
                             nbgrader_schema_version: () => a,
-                            randomString: () => c,
-                            remove_nbgrader_field: () => h,
+                            randomString: () => s,
+                            remove_nbgrader_field: () => p,
                             remove_nbgrader_metadata: () => u,
                             set_grade: () => _,
                             set_grade_id: () => C,
                             set_locked: () => O,
-                            set_nbgrader_field: () => p,
+                            set_nbgrader_field: () => h,
                             set_points: () => S,
                             set_schema_version: () => y,
                             set_solution: () => g,
                             set_task: () => k,
                             to_description: () => T,
-                            to_float: () => s,
+                            to_float: () => c,
                             to_test: () => P
                         });
                         var t = {};
                         o.r(t), o.d(t, {
                             add_shortcut: () => W,
                             disable_add_cell_on_execute: () => Y,
                             remove_shortcuts: () => I
                         });
                         var r = {};
                         o.r(r), o.d(r, {
                             add_username: () => R
                         });
                         const a = 3;
 
-                        function c(e) {
+                        function s(e) {
                             let t, n = "",
                                 r = "abcdef0123456789";
                             for (t = 0; t < e; t++) n += r[Math.floor(Math.random() * r.length)];
                             return n
                         }
 
-                        function s(e) {
+                        function c(e) {
                             return void 0 === e || "" === e ? 0 : parseFloat(e)
                         }
 
                         function l(e) {
                             return e.metadata.hasOwnProperty("nbgrader")
                         }
 
@@ -7267,76 +7277,76 @@
                             l(e) || (e.metadata.nbgrader = {})
                         }
 
                         function f(e, t, n = {}) {
                             return l(e) && e.metadata.nbgrader[t] || n
                         }
 
-                        function p(e, t, n) {
+                        function h(e, t, n) {
                             l(e) || (e.metadata.nbgrader = {}), e.metadata.nbgrader[t] = n
                         }
 
-                        function h(e, t) {
+                        function p(e, t) {
                             l(e) && e.metadata.nbgrader.hasOwnProperty(t) && delete e.metadata.nbgrader[t]
                         }
 
                         function m(e) {
                             if (l(e)) return void 0 === f(e, "schema_version") ? 0 : f(e, "schema_version")
                         }
 
                         function y(e) {
-                            l(e) || d(e), p(e, "schema_version", a)
+                            l(e) || d(e), h(e, "schema_version", a)
                         }
 
                         function v(e) {
                             return f(e, "solution", !1)
                         }
 
                         function g(e, t) {
-                            p(e, "solution", t)
+                            h(e, "solution", t)
                         }
 
                         function b(e) {
                             return f(e, "grade", !1)
                         }
 
                         function _(e, t) {
-                            p(e, "grade", t)
+                            h(e, "grade", t)
                         }
 
                         function w(e) {
                             return f(e, "task", !1)
                         }
 
                         function k(e, t) {
-                            p(e, "task", t)
+                            h(e, "task", t)
                         }
 
                         function x(e) {
                             return f(e, "locked", !1)
                         }
 
                         function O(e, t) {
-                            p(e, "locked", t)
+                            h(e, "locked", t)
                         }
 
                         function E(e) {
-                            return s(f(e, "points", 0))
+                            return c(f(e, "points", 0))
                         }
 
                         function S(e, t) {
-                            p(e, "points", Math.max(0, s(t)))
+                            h(e, "points", Math.max(0, c(t)))
                         }
 
                         function j(e) {
-                            return f(e, "grade_id", "cell-" + c(16))
+                            return f(e, "grade_id", "cell-" + s(16))
                         }
 
                         function C(e, t) {
-                            p(e, "grade_id", t)
+                            h(e, "grade_id", t)
                         }
 
                         function A(e) {
                             return b(e) && x(e) && !v(e)
                         }
 
                         function P(e) {
@@ -7366,17 +7376,19 @@
                             if ("command" === e) return J().keyboard_manager.command_shortcuts;
                             if ("edit" === e) return J().keyboard_manager.edit_shortcuts;
                             throw new Error("Mode needs to be either 'command' or 'edit'")
                         }
 
                         function I(e, ...t) {
                             const n = M(e);
-                            for (const e of t) try {
-                                n.remove_shortcut(e)
-                            } catch (e) {}
+                            for (const r of t) try {
+                                n.remove_shortcut(r)
+                            } catch (t) {
+                                console.log("Error removing shortcut", r, "from", e, "mode:", t.message)
+                            }
                         }
 
                         function W(e, t, n, r, o = "zz") {
                             M(e).add_shortcut(t, {
                                 help: r,
                                 help_index: o,
                                 handler: n
@@ -7390,15 +7402,15 @@
                                 else {
                                     let t = this.get_selected_cell();
                                     e = this.find_cell_index(t), t.execute()
                                 }
                                 e = Math.min(e + 1, this.ncells() - 1), this.select(e), this.focus_cell()
                             };
                             const e = ["alt-enter", "shift-enter"];
-                            I("edit", e), I("command", e);
+                            I("edit", ...e), I("command", ...e);
                             const t = "run cell",
                                 n = function(e) {
                                     return J().notebook.execute_cell_and_select_below_without_insert(), !1
                                 };
                             for (const r of e) W("edit", r, n, t), W("command", r, n, t)
                         }
                         var N = o(804);
@@ -7441,76 +7453,76 @@
             },
             425: e => {
                 "use strict";
                 e.exports = l
             },
             600: e => {
                 "use strict";
-                e.exports = s
+                e.exports = c
             },
             140: e => {
                 "use strict";
                 e.exports = a
             },
             315: e => {
                 "use strict";
                 e.exports = o
             },
             75: e => {
                 "use strict";
-                e.exports = c
+                e.exports = s
             }
         },
         f = {};
 
-    function p(e) {
+    function h(e) {
         var t = f[e];
         if (void 0 !== t) return t.exports;
         var n = f[e] = {
             exports: {}
         };
-        return d[e](n, n.exports, p), n.exports
+        return d[e](n, n.exports, h), n.exports
     }
-    p.n = e => {
+    h.n = e => {
         var t = e && e.__esModule ? () => e.default : () => e;
-        return p.d(t, {
+        return h.d(t, {
             a: t
         }), t
-    }, p.d = (e, t) => {
-        for (var n in t) p.o(t, n) && !p.o(e, n) && Object.defineProperty(e, n, {
+    }, h.d = (e, t) => {
+        for (var n in t) h.o(t, n) && !h.o(e, n) && Object.defineProperty(e, n, {
             enumerable: !0,
             get: t[n]
         })
-    }, p.o = (e, t) => Object.prototype.hasOwnProperty.call(e, t), p.r = e => {
+    }, h.o = (e, t) => Object.prototype.hasOwnProperty.call(e, t), h.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
     };
-    var h = {};
+    var p = {};
     return (() => {
         "use strict";
-        p.r(h), p.d(h, {
+        h.r(p), h.d(p, {
             load_ipython_extension: () => d
         });
-        var e = p(527),
-            t = p.n(e),
-            n = p(290),
-            r = p.n(n),
-            o = p(761),
-            i = p(322),
-            a = p(654),
-            c = p(532),
-            s = p(703),
-            l = p(426);
+        var e = h(527),
+            t = h.n(e),
+            n = h(290),
+            r = h.n(n),
+            o = h(761),
+            i = h(322),
+            a = h(654),
+            s = h(532),
+            c = h(703),
+            l = h(426);
 
         function u() {
-            (0, o.initialize_cell_extension)(), (0, a.patch_assignment_notebook)(), (new s.ExamMenubar).activate(), (new i.AssignmentViewToolbar).activate(), (0, c.disable_shortcuts)(), l.username.add_username()
+            (0, o.initialize_cell_extension)(), (0, a.patch_assignment_notebook)(), (new c.ExamMenubar).activate(), (new i.AssignmentViewToolbar).activate(), (0, s.disable_shortcuts)(), l.username.add_username()
         }
 
         function d() {
             var e;
             null !== (e = t().notebook) && void 0 !== e && e._fully_loaded ? u() : r().on("notebook_loaded.Notebook", u)
         }
-    })(), h
+    })(), p
 })()));
```

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/static/nbextensions/notebook/teacher/main.js` & `e2xgrader-0.3.0.dev2/e2xgrader/static/nbextensions/notebook/teacher/main.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -476,19 +476,19 @@
                                             c = o.n(s),
                                             l = o(793),
                                             u = o.n(l),
                                             d = o(892),
                                             f = o.n(d),
                                             p = o(173),
                                             h = o.n(p),
-                                            y = o(464),
-                                            m = o.n(y),
+                                            m = o(464),
+                                            y = o.n(m),
                                             v = o(616),
                                             g = {};
-                                        g.styleTagTransform = m(), g.setAttributes = f(), g.insert = u().bind(null, "head"), g.domAPI = c(), g.insertStyleElement = h(), a()(v.Z, g), v.Z && v.Z.locals && v.Z.locals;
+                                        g.styleTagTransform = y(), g.setAttributes = f(), g.insert = u().bind(null, "head"), g.domAPI = c(), g.insertStyleElement = h(), a()(v.Z, g), v.Z && v.Z.locals && v.Z.locals;
                                         class b {
                                             constructor() {
                                                 this.element = e()("<div/>").attr("id", "e2x-menubar").append(e()("<span/>").text("e²x").addClass("e2x-badge"))
                                             }
                                             hide_maintoolbar() {
                                                 e()("#maintoolbar-container").hide()
                                             }
@@ -643,15 +643,15 @@
                                         });
                                         var t = {};
                                         o.r(t), o.d(t, {
                                             create_nbgrader_metadata: () => d,
                                             get_grade_id: () => S,
                                             get_nbgrader_field: () => f,
                                             get_points: () => E,
-                                            get_schema_version: () => y,
+                                            get_schema_version: () => m,
                                             is_description: () => B,
                                             is_empty: () => G,
                                             is_grade: () => b,
                                             is_invalid: () => Q,
                                             is_locked: () => x,
                                             is_nbgrader: () => l,
                                             is_solution: () => v,
@@ -662,15 +662,15 @@
                                             remove_nbgrader_field: () => h,
                                             remove_nbgrader_metadata: () => u,
                                             set_grade: () => _,
                                             set_grade_id: () => j,
                                             set_locked: () => O,
                                             set_nbgrader_field: () => p,
                                             set_points: () => C,
-                                            set_schema_version: () => m,
+                                            set_schema_version: () => y,
                                             set_solution: () => g,
                                             set_task: () => k,
                                             to_description: () => T,
                                             to_float: () => c,
                                             to_test: () => P
                                         });
                                         var e = {};
@@ -716,19 +716,19 @@
                                             l(t) || (t.metadata.nbgrader = {}), t.metadata.nbgrader[e] = n
                                         }
 
                                         function h(t, e) {
                                             l(t) && t.metadata.nbgrader.hasOwnProperty(e) && delete t.metadata.nbgrader[e]
                                         }
 
-                                        function y(t) {
+                                        function m(t) {
                                             if (l(t)) return void 0 === f(t, "schema_version") ? 0 : f(t, "schema_version")
                                         }
 
-                                        function m(t) {
+                                        function y(t) {
                                             l(t) || d(t), p(t, "schema_version", a)
                                         }
 
                                         function v(t) {
                                             return f(t, "solution", !1)
                                         }
 
@@ -777,23 +777,23 @@
                                         }
 
                                         function A(t) {
                                             return b(t) && x(t) && !v(t)
                                         }
 
                                         function P(t) {
-                                            remove_metadata(t), m(t), g(t, !1), _(t, !0), O(t, !0)
+                                            remove_metadata(t), y(t), g(t, !1), _(t, !0), O(t, !0)
                                         }
 
                                         function B(t) {
                                             return x(t) && !b(t) && !v(t)
                                         }
 
                                         function T(t) {
-                                            remove_metadata(t), m(t), g(t, !1), _(t, !1), O(t, !0)
+                                            remove_metadata(t), y(t), g(t, !1), _(t, !1), O(t, !0)
                                         }
 
                                         function Q(t) {
                                             return !(w(t) || v(t) && b(t) || (!v(t) || "code" === t.cell_type) && (!b(t) || "code" === t.cell_type))
                                         }
 
                                         function G(t) {
@@ -807,17 +807,19 @@
                                             if ("command" === t) return I().keyboard_manager.command_shortcuts;
                                             if ("edit" === t) return I().keyboard_manager.edit_shortcuts;
                                             throw new Error("Mode needs to be either 'command' or 'edit'")
                                         }
 
                                         function M(t, ...e) {
                                             const n = J(t);
-                                            for (const t of e) try {
-                                                n.remove_shortcut(t)
-                                            } catch (t) {}
+                                            for (const r of e) try {
+                                                n.remove_shortcut(r)
+                                            } catch (e) {
+                                                console.log("Error removing shortcut", r, "from", t, "mode:", e.message)
+                                            }
                                         }
 
                                         function W(t, e, n, r, o = "zz") {
                                             J(t).add_shortcut(e, {
                                                 help: r,
                                                 help_index: o,
                                                 handler: n
@@ -831,15 +833,15 @@
                                                 else {
                                                     let e = this.get_selected_cell();
                                                     t = this.find_cell_index(e), e.execute()
                                                 }
                                                 t = Math.min(t + 1, this.ncells() - 1), this.select(t), this.focus_cell()
                                             };
                                             const t = ["alt-enter", "shift-enter"];
-                                            M("edit", t), M("command", t);
+                                            M("edit", ...t), M("command", ...t);
                                             const e = "run cell",
                                                 n = function(t) {
                                                     return I().notebook.execute_cell_and_select_below_without_insert(), !1
                                                 };
                                             for (const r of t) W("edit", r, n, e), W("command", r, n, e)
                                         }
                                         var R = o(804);
@@ -912,17 +914,17 @@
                             c = o.n(s),
                             l = o(892),
                             u = o.n(l),
                             d = o(173),
                             f = o.n(d),
                             p = o(464),
                             h = o.n(p),
-                            y = o(262),
-                            m = {};
-                        m.styleTagTransform = h(), m.setAttributes = u(), m.insert = c().bind(null, "head"), m.domAPI = a(), m.insertStyleElement = f(), e()(y.Z, m), y.Z && y.Z.locals && y.Z.locals;
+                            m = o(262),
+                            y = {};
+                        y.styleTagTransform = h(), y.setAttributes = u(), y.insert = c().bind(null, "head"), y.domAPI = a(), y.insertStyleElement = f(), e()(m.Z, y), m.Z && m.Z.locals && m.Z.locals;
                         var v = o(237),
                             g = o(761),
                             b = o.n(g),
                             _ = o(86),
                             w = o.n(_);
                         const k = n(566);
                         var x = o.n(k),
@@ -1435,20 +1437,20 @@
                                             return c(t) && t.metadata.extended_cell[e] || n
                                         }
 
                                         function h(t, e, n) {
                                             c(t) && (t.metadata.extended_cell[e] = n)
                                         }
 
-                                        function y(t, e) {
+                                        function m(t, e) {
                                             (null == e || e > t.length) && (e = t.length);
                                             for (var n = 0, r = new Array(e); n < e; n++) r[n] = t[n];
                                             return r
                                         }
-                                        var m = function() {
+                                        var y = function() {
                                             function t(e, n) {
                                                 ! function(t, e) {
                                                     if (!(t instanceof e)) throw new TypeError("Cannot call a class as a function")
                                                 }(this, t), this.cell = e, this.options = n, this.initialize_options()
                                             }
                                             var e, n;
                                             return e = t, (n = [{
@@ -1501,17 +1503,17 @@
                                                                                 if (s) throw o
                                                                             }
                                                                         }
                                                                         return i
                                                                     }
                                                                 }(n) || function(t, e) {
                                                                     if (t) {
-                                                                        if ("string" == typeof t) return y(t, 2);
+                                                                        if ("string" == typeof t) return m(t, 2);
                                                                         var n = Object.prototype.toString.call(t).slice(8, -1);
-                                                                        return "Object" === n && t.constructor && (n = t.constructor.name), "Map" === n || "Set" === n ? Array.from(t) : "Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n) ? y(t, 2) : void 0
+                                                                        return "Object" === n && t.constructor && (n = t.constructor.name), "Map" === n || "Set" === n ? Array.from(t) : "Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n) ? m(t, 2) : void 0
                                                                     }
                                                                 }(n) || function() {
                                                                     throw new TypeError("Invalid attempt to destructure non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
                                                                 }(),
                                                                 a = i[0],
                                                                 c = i[1];
                                                             if ("checkbox" == c.type) {
@@ -1536,15 +1538,15 @@
 
                                         function v(t, e) {
                                             if (!(t instanceof e)) throw new TypeError("Cannot call a class as a function")
                                         }
                                         var g = function() {
                                             function t(e, n) {
                                                 var r = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : {};
-                                                v(this, t), this.type = n, this.cell = e, u(this.cell, this.type), this.option_dict = new m(this.cell, r)
+                                                v(this, t), this.type = n, this.cell = e, u(this.cell, this.type), this.option_dict = new y(this.cell, r)
                                             }
                                             var e, n;
                                             return e = t, (n = [{
                                                 key: "get_metadata",
                                                 value: function() {
                                                     return d(this.cell)
                                                 }
@@ -2117,17 +2119,17 @@
                                             function f() {}
 
                                             function p() {}
                                             var h = {};
                                             s(h, o, (function() {
                                                 return this
                                             }));
-                                            var y = Object.getPrototypeOf,
-                                                m = y && y(y(O([])));
-                                            m && m !== e && n.call(m, o) && (h = m);
+                                            var m = Object.getPrototypeOf,
+                                                y = m && m(m(O([])));
+                                            y && y !== e && n.call(y, o) && (h = y);
                                             var v = p.prototype = d.prototype = Object.create(h);
 
                                             function g(t) {
                                                 ["next", "throw", "return"].forEach((function(e) {
                                                     s(t, e, (function(t) {
                                                         return this._invoke(e, t)
                                                     }))
@@ -2721,17 +2723,17 @@
                                             function f() {}
 
                                             function p() {}
                                             var h = {};
                                             s(h, o, (function() {
                                                 return this
                                             }));
-                                            var y = Object.getPrototypeOf,
-                                                m = y && y(y(O([])));
-                                            m && m !== e && n.call(m, o) && (h = m);
+                                            var m = Object.getPrototypeOf,
+                                                y = m && m(m(O([])));
+                                            y && y !== e && n.call(y, o) && (h = y);
                                             var v = p.prototype = d.prototype = Object.create(h);
 
                                             function g(t) {
                                                 ["next", "throw", "return"].forEach((function(e) {
                                                     s(t, e, (function(t) {
                                                         return this._invoke(e, t)
                                                     }))
@@ -2996,36 +2998,36 @@
                                                 try {
                                                     return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], (function() {}))), !0
                                                 } catch (t) {
                                                     return !1
                                                 }
                                             }();
                                             return function() {
-                                                var n, r = mt(t);
+                                                var n, r = yt(t);
                                                 if (e) {
-                                                    var o = mt(this).constructor;
+                                                    var o = yt(this).constructor;
                                                     n = Reflect.construct(r, arguments, o)
                                                 } else n = r.apply(this, arguments);
-                                                return yt(this, n)
+                                                return mt(this, n)
                                             }
                                         }
 
-                                        function yt(t, e) {
+                                        function mt(t, e) {
                                             if (e && ("object" === at(e) || "function" == typeof e)) return e;
                                             if (void 0 !== e) throw new TypeError("Derived constructors may only return object or undefined");
                                             return function(t) {
                                                 if (void 0 === t) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
                                                 return t
                                             }(t)
                                         }
 
-                                        function mt(t) {
-                                            return mt = Object.setPrototypeOf ? Object.getPrototypeOf.bind() : function(t) {
+                                        function yt(t) {
+                                            return yt = Object.setPrototypeOf ? Object.getPrototypeOf.bind() : function(t) {
                                                 return t.__proto__ || Object.getPrototypeOf(t)
-                                            }, mt(t)
+                                            }, yt(t)
                                         }
                                         var vt = function(t) {
                                                 ft(n, t);
                                                 var e = ht(n);
 
                                                 function n() {
                                                     return lt(this, n), e.apply(this, arguments)
@@ -3538,16 +3540,16 @@
                         r.MarkdownCell.prototype.render, r.MarkdownCell.prototype.unrender;
                         var l = o(86),
                             u = o.n(l);
                         const d = n(290);
                         var f = o.n(d);
                         const p = n(140);
                         var h = !1,
-                            y = r.MarkdownCell.prototype.render,
-                            m = p.Notebook.prototype.to_markdown,
+                            m = r.MarkdownCell.prototype.render,
+                            y = p.Notebook.prototype.to_markdown,
                             v = r.TextCell.prototype.toJSON,
                             g = r.MarkdownCell.prototype.unrender;
 
                         function b() {
                             var t = u().notebook.get_cells();
                             for (var e in t) {
                                 var n = t[e];
@@ -3604,25 +3606,25 @@
                                         })
                                     }))
                                 }
                                 return t
                             }, r.TextCell.prototype.toJSON = function() {
                                 return "attachments" == a.utils.get_e2x_cell_type(this) ? (arguments[0] = !1, v.apply(this, arguments)) : v.apply(this, arguments)
                             }, p.Notebook.prototype.to_markdown = function() {
-                                m.apply(this, arguments);
+                                y.apply(this, arguments);
                                 var t = this.get_cell(arguments[0]);
                                 t.unrender_force(), t.render()
                             }, r.MarkdownCell.prototype.unrender_force = g, r.MarkdownCell.prototype.unrender = function() {
                                 a.utils.is_e2x(this) || g.apply(this, arguments)
-                            }, r.MarkdownCell.prototype.render_force = y, r.MarkdownCell.prototype.render = function() {
+                            }, r.MarkdownCell.prototype.render_force = m, r.MarkdownCell.prototype.render = function() {
                                 var t = a.utils.get_e2x_cell_type(this);
                                 if (a.cells.hasOwnProperty(t)) {
                                     var e = new a.cells[t](this);
                                     e.edit_mode = h, e.render()
-                                } else y.apply(this, arguments)
+                                } else m.apply(this, arguments)
                             }, u().notebook.metadata.hasOwnProperty("celltoolbar") && "Create Assignment" === u().notebook.metadata.celltoolbar && (h = !0), f().on("preset_activated.CellToolbar", (function(t, e) {
                                 h = "Create Assignment" == e.name, b()
                             })), f().on("global_hide.CellToolbar", (function(t, e) {
                                 h = !1, b()
                             })), b()
                         }
                         Q.styleTagTransform = B(), Q.setAttributes = S(), Q.insert = E().bind(null, "head"), Q.domAPI = x(), Q.insertStyleElement = A(), w()(T.Z, Q), T.Z && T.Z.locals && T.Z.locals
@@ -3967,20 +3969,20 @@
                                             return c(t) && t.metadata.extended_cell[e] || n
                                         }
 
                                         function h(t, e, n) {
                                             c(t) && (t.metadata.extended_cell[e] = n)
                                         }
 
-                                        function y(t, e) {
+                                        function m(t, e) {
                                             (null == e || e > t.length) && (e = t.length);
                                             for (var n = 0, r = new Array(e); n < e; n++) r[n] = t[n];
                                             return r
                                         }
-                                        var m = function() {
+                                        var y = function() {
                                             function t(e, n) {
                                                 ! function(t, e) {
                                                     if (!(t instanceof e)) throw new TypeError("Cannot call a class as a function")
                                                 }(this, t), this.cell = e, this.options = n, this.initialize_options()
                                             }
                                             var e, n;
                                             return e = t, (n = [{
@@ -4033,17 +4035,17 @@
                                                                                 if (s) throw o
                                                                             }
                                                                         }
                                                                         return i
                                                                     }
                                                                 }(n) || function(t, e) {
                                                                     if (t) {
-                                                                        if ("string" == typeof t) return y(t, 2);
+                                                                        if ("string" == typeof t) return m(t, 2);
                                                                         var n = Object.prototype.toString.call(t).slice(8, -1);
-                                                                        return "Object" === n && t.constructor && (n = t.constructor.name), "Map" === n || "Set" === n ? Array.from(t) : "Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n) ? y(t, 2) : void 0
+                                                                        return "Object" === n && t.constructor && (n = t.constructor.name), "Map" === n || "Set" === n ? Array.from(t) : "Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n) ? m(t, 2) : void 0
                                                                     }
                                                                 }(n) || function() {
                                                                     throw new TypeError("Invalid attempt to destructure non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
                                                                 }(),
                                                                 a = i[0],
                                                                 c = i[1];
                                                             if ("checkbox" == c.type) {
@@ -4068,15 +4070,15 @@
 
                                         function v(t, e) {
                                             if (!(t instanceof e)) throw new TypeError("Cannot call a class as a function")
                                         }
                                         var g = function() {
                                             function t(e, n) {
                                                 var r = arguments.length > 2 && void 0 !== arguments[2] ? arguments[2] : {};
-                                                v(this, t), this.type = n, this.cell = e, u(this.cell, this.type), this.option_dict = new m(this.cell, r)
+                                                v(this, t), this.type = n, this.cell = e, u(this.cell, this.type), this.option_dict = new y(this.cell, r)
                                             }
                                             var e, n;
                                             return e = t, (n = [{
                                                 key: "get_metadata",
                                                 value: function() {
                                                     return d(this.cell)
                                                 }
@@ -4649,17 +4651,17 @@
                                             function f() {}
 
                                             function p() {}
                                             var h = {};
                                             s(h, o, (function() {
                                                 return this
                                             }));
-                                            var y = Object.getPrototypeOf,
-                                                m = y && y(y(O([])));
-                                            m && m !== e && n.call(m, o) && (h = m);
+                                            var m = Object.getPrototypeOf,
+                                                y = m && m(m(O([])));
+                                            y && y !== e && n.call(y, o) && (h = y);
                                             var v = p.prototype = d.prototype = Object.create(h);
 
                                             function g(t) {
                                                 ["next", "throw", "return"].forEach((function(e) {
                                                     s(t, e, (function(t) {
                                                         return this._invoke(e, t)
                                                     }))
@@ -5253,17 +5255,17 @@
                                             function f() {}
 
                                             function p() {}
                                             var h = {};
                                             s(h, o, (function() {
                                                 return this
                                             }));
-                                            var y = Object.getPrototypeOf,
-                                                m = y && y(y(O([])));
-                                            m && m !== e && n.call(m, o) && (h = m);
+                                            var m = Object.getPrototypeOf,
+                                                y = m && m(m(O([])));
+                                            y && y !== e && n.call(y, o) && (h = y);
                                             var v = p.prototype = d.prototype = Object.create(h);
 
                                             function g(t) {
                                                 ["next", "throw", "return"].forEach((function(e) {
                                                     s(t, e, (function(t) {
                                                         return this._invoke(e, t)
                                                     }))
@@ -5528,36 +5530,36 @@
                                                 try {
                                                     return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], (function() {}))), !0
                                                 } catch (t) {
                                                     return !1
                                                 }
                                             }();
                                             return function() {
-                                                var n, r = mt(t);
+                                                var n, r = yt(t);
                                                 if (e) {
-                                                    var o = mt(this).constructor;
+                                                    var o = yt(this).constructor;
                                                     n = Reflect.construct(r, arguments, o)
                                                 } else n = r.apply(this, arguments);
-                                                return yt(this, n)
+                                                return mt(this, n)
                                             }
                                         }
 
-                                        function yt(t, e) {
+                                        function mt(t, e) {
                                             if (e && ("object" === at(e) || "function" == typeof e)) return e;
                                             if (void 0 !== e) throw new TypeError("Derived constructors may only return object or undefined");
                                             return function(t) {
                                                 if (void 0 === t) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
                                                 return t
                                             }(t)
                                         }
 
-                                        function mt(t) {
-                                            return mt = Object.setPrototypeOf ? Object.getPrototypeOf.bind() : function(t) {
+                                        function yt(t) {
+                                            return yt = Object.setPrototypeOf ? Object.getPrototypeOf.bind() : function(t) {
                                                 return t.__proto__ || Object.getPrototypeOf(t)
-                                            }, mt(t)
+                                            }, yt(t)
                                         }
                                         var vt = function(t) {
                                                 ft(n, t);
                                                 var e = ht(n);
 
                                                 function n() {
                                                     return lt(this, n), e.apply(this, arguments)
@@ -6130,15 +6132,15 @@
                                         });
                                         var t = {};
                                         o.r(t), o.d(t, {
                                             create_nbgrader_metadata: () => d,
                                             get_grade_id: () => S,
                                             get_nbgrader_field: () => f,
                                             get_points: () => E,
-                                            get_schema_version: () => y,
+                                            get_schema_version: () => m,
                                             is_description: () => B,
                                             is_empty: () => G,
                                             is_grade: () => b,
                                             is_invalid: () => Q,
                                             is_locked: () => x,
                                             is_nbgrader: () => l,
                                             is_solution: () => v,
@@ -6149,15 +6151,15 @@
                                             remove_nbgrader_field: () => h,
                                             remove_nbgrader_metadata: () => u,
                                             set_grade: () => _,
                                             set_grade_id: () => j,
                                             set_locked: () => O,
                                             set_nbgrader_field: () => p,
                                             set_points: () => C,
-                                            set_schema_version: () => m,
+                                            set_schema_version: () => y,
                                             set_solution: () => g,
                                             set_task: () => k,
                                             to_description: () => T,
                                             to_float: () => c,
                                             to_test: () => P
                                         });
                                         var e = {};
@@ -6203,19 +6205,19 @@
                                             l(t) || (t.metadata.nbgrader = {}), t.metadata.nbgrader[e] = n
                                         }
 
                                         function h(t, e) {
                                             l(t) && t.metadata.nbgrader.hasOwnProperty(e) && delete t.metadata.nbgrader[e]
                                         }
 
-                                        function y(t) {
+                                        function m(t) {
                                             if (l(t)) return void 0 === f(t, "schema_version") ? 0 : f(t, "schema_version")
                                         }
 
-                                        function m(t) {
+                                        function y(t) {
                                             l(t) || d(t), p(t, "schema_version", a)
                                         }
 
                                         function v(t) {
                                             return f(t, "solution", !1)
                                         }
 
@@ -6264,23 +6266,23 @@
                                         }
 
                                         function A(t) {
                                             return b(t) && x(t) && !v(t)
                                         }
 
                                         function P(t) {
-                                            remove_metadata(t), m(t), g(t, !1), _(t, !0), O(t, !0)
+                                            remove_metadata(t), y(t), g(t, !1), _(t, !0), O(t, !0)
                                         }
 
                                         function B(t) {
                                             return x(t) && !b(t) && !v(t)
                                         }
 
                                         function T(t) {
-                                            remove_metadata(t), m(t), g(t, !1), _(t, !1), O(t, !0)
+                                            remove_metadata(t), y(t), g(t, !1), _(t, !1), O(t, !0)
                                         }
 
                                         function Q(t) {
                                             return !(w(t) || v(t) && b(t) || (!v(t) || "code" === t.cell_type) && (!b(t) || "code" === t.cell_type))
                                         }
 
                                         function G(t) {
@@ -6296,15 +6298,17 @@
                                             throw new Error("Mode needs to be either 'command' or 'edit'")
                                         }
 
                                         function M(t, ...e) {
                                             const n = J(t);
                                             for (const r of e) try {
                                                 n.remove_shortcut(r)
-                                            } catch (t) {}
+                                            } catch (e) {
+                                                console.log("Error removing shortcut", r, "from", t, "mode:", e.message)
+                                            }
                                         }
 
                                         function W(t, e, n, r, o = "zz") {
                                             J(t).add_shortcut(e, {
                                                 help: r,
                                                 help_index: o,
                                                 handler: n
@@ -6318,15 +6322,15 @@
                                                 else {
                                                     let e = this.get_selected_cell();
                                                     t = this.find_cell_index(e), e.execute()
                                                 }
                                                 t = Math.min(t + 1, this.ncells() - 1), this.select(t), this.focus_cell()
                                             };
                                             const t = ["alt-enter", "shift-enter"];
-                                            M("edit", t), M("command", t);
+                                            M("edit", ...t), M("command", ...t);
                                             const e = "run cell",
                                                 n = function(t) {
                                                     return I().notebook.execute_cell_and_select_below_without_insert(), !1
                                                 };
                                             for (const r of t) W("edit", r, n, e), W("command", r, n, e)
                                         }
                                         var R = o(804);
@@ -6403,22 +6407,22 @@
                         const l = n(290);
                         var u = o.n(l);
                         const d = n(600);
                         var f = o(856),
                             p = o.n(f),
                             h = o(426);
 
-                        function y(t, e) {
+                        function m(t, e) {
                             var n = "undefined" != typeof Symbol && t[Symbol.iterator] || t["@@iterator"];
                             if (!n) {
                                 if (Array.isArray(t) || (n = function(t, e) {
                                         if (t) {
-                                            if ("string" == typeof t) return m(t, e);
+                                            if ("string" == typeof t) return y(t, e);
                                             var n = Object.prototype.toString.call(t).slice(8, -1);
-                                            return "Object" === n && t.constructor && (n = t.constructor.name), "Map" === n || "Set" === n ? Array.from(t) : "Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n) ? m(t, e) : void 0
+                                            return "Object" === n && t.constructor && (n = t.constructor.name), "Map" === n || "Set" === n ? Array.from(t) : "Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n) ? y(t, e) : void 0
                                         }
                                     }(t)) || e && t && "number" == typeof t.length) {
                                     n && (t = n);
                                     var r = 0,
                                         o = function() {};
                                     return {
                                         s: o,
@@ -6457,15 +6461,15 @@
                                     } finally {
                                         if (s) throw i
                                     }
                                 }
                             }
                         }
 
-                        function m(t, e) {
+                        function y(t, e) {
                             (null == e || e > t.length) && (e = t.length);
                             for (var n = 0, r = new Array(e); n < e; n++) r[n] = t[n];
                             return r
                         }
                         var v = function() {
                                 function t() {
                                     ! function(t, e) {
@@ -6493,15 +6497,15 @@
                                 }, {
                                     key: "validate_ids",
                                     value: function() {
                                         if (void 0 === this.warning) {
                                             var t, e = this.get_modal_opts(),
                                                 n = $(".nbgrader-id-input"),
                                                 r = new Object,
-                                                o = y(n);
+                                                o = m(n);
                                             try {
                                                 for (o.s(); !(t = o.n()).done;) {
                                                     var i = t.value,
                                                         a = $(i).val();
                                                     if (!this.grade_id_regex.test(a)) {
                                                         e.title = "Invalid nbgrader cell ID", e.body = "At least one cell has an invalid nbgrader ID. Cell IDs must contain at least one character, and may only contain letters, numbers, hyphens, and/or underscores.", this.warning = p().modal(e);
                                                         break
@@ -6521,15 +6525,15 @@
                                     }
                                 }, {
                                     key: "validate_schema_version",
                                     value: function() {
                                         if (void 0 === this.warning) {
                                             var t, e = c().notebook.get_cells(),
                                                 n = this.get_modal_opts(),
-                                                r = y(e);
+                                                r = m(e);
                                             try {
                                                 for (r.s(); !(t = r.n()).done;) {
                                                     var o = t.value,
                                                         i = h.utils.get_schema_version(o);
                                                     if (void 0 !== i && i < h.utils.nbgrader_schema_version) {
                                                         n.title = "Outdated schema version", n.body = $("<p/>").html("At least one cell has an old version (" + i + ") of the nbgrader metadata. Please back up this notebook and then update the metadata on the command line using the following command: <code>nbgrader update " + c().notebook.notebook_path + "</code>"), this.warning = p().modal(n);
                                                         break
@@ -6995,15 +6999,15 @@
                         });
                         var t = {};
                         o.r(t), o.d(t, {
                             create_nbgrader_metadata: () => d,
                             get_grade_id: () => S,
                             get_nbgrader_field: () => f,
                             get_points: () => E,
-                            get_schema_version: () => y,
+                            get_schema_version: () => m,
                             is_description: () => B,
                             is_empty: () => G,
                             is_grade: () => b,
                             is_invalid: () => Q,
                             is_locked: () => x,
                             is_nbgrader: () => l,
                             is_solution: () => v,
@@ -7014,15 +7018,15 @@
                             remove_nbgrader_field: () => h,
                             remove_nbgrader_metadata: () => u,
                             set_grade: () => _,
                             set_grade_id: () => j,
                             set_locked: () => O,
                             set_nbgrader_field: () => p,
                             set_points: () => C,
-                            set_schema_version: () => m,
+                            set_schema_version: () => y,
                             set_solution: () => g,
                             set_task: () => k,
                             to_description: () => T,
                             to_float: () => c,
                             to_test: () => P
                         });
                         var e = {};
@@ -7068,19 +7072,19 @@
                             l(t) || (t.metadata.nbgrader = {}), t.metadata.nbgrader[e] = n
                         }
 
                         function h(t, e) {
                             l(t) && t.metadata.nbgrader.hasOwnProperty(e) && delete t.metadata.nbgrader[e]
                         }
 
-                        function y(t) {
+                        function m(t) {
                             if (l(t)) return void 0 === f(t, "schema_version") ? 0 : f(t, "schema_version")
                         }
 
-                        function m(t) {
+                        function y(t) {
                             l(t) || d(t), p(t, "schema_version", a)
                         }
 
                         function v(t) {
                             return f(t, "solution", !1)
                         }
 
@@ -7129,23 +7133,23 @@
                         }
 
                         function A(t) {
                             return b(t) && x(t) && !v(t)
                         }
 
                         function P(t) {
-                            remove_metadata(t), m(t), g(t, !1), _(t, !0), O(t, !0)
+                            remove_metadata(t), y(t), g(t, !1), _(t, !0), O(t, !0)
                         }
 
                         function B(t) {
                             return x(t) && !b(t) && !v(t)
                         }
 
                         function T(t) {
-                            remove_metadata(t), m(t), g(t, !1), _(t, !1), O(t, !0)
+                            remove_metadata(t), y(t), g(t, !1), _(t, !1), O(t, !0)
                         }
 
                         function Q(t) {
                             return !(w(t) || v(t) && b(t) || (!v(t) || "code" === t.cell_type) && (!b(t) || "code" === t.cell_type))
                         }
 
                         function G(t) {
@@ -7159,17 +7163,19 @@
                             if ("command" === t) return I().keyboard_manager.command_shortcuts;
                             if ("edit" === t) return I().keyboard_manager.edit_shortcuts;
                             throw new Error("Mode needs to be either 'command' or 'edit'")
                         }
 
                         function M(t, ...e) {
                             const n = J(t);
-                            for (const t of e) try {
-                                n.remove_shortcut(t)
-                            } catch (t) {}
+                            for (const r of e) try {
+                                n.remove_shortcut(r)
+                            } catch (e) {
+                                console.log("Error removing shortcut", r, "from", t, "mode:", e.message)
+                            }
                         }
 
                         function W(t, e, n, r, o = "zz") {
                             J(t).add_shortcut(e, {
                                 help: r,
                                 help_index: o,
                                 handler: n
@@ -7183,15 +7189,15 @@
                                 else {
                                     let e = this.get_selected_cell();
                                     t = this.find_cell_index(e), e.execute()
                                 }
                                 t = Math.min(t + 1, this.ncells() - 1), this.select(t), this.focus_cell()
                             };
                             const t = ["alt-enter", "shift-enter"];
-                            M("edit", t), M("command", t);
+                            M("edit", ...t), M("command", ...t);
                             const e = "run cell",
                                 n = function(t) {
                                     return I().notebook.execute_cell_and_select_below_without_insert(), !1
                                 };
                             for (const r of t) W("edit", r, n, e), W("command", r, n, e)
                         }
                         var R = o(804);
@@ -7272,15 +7278,15 @@
             value: !0
         })
     };
     var f = {};
     return (() => {
         "use strict";
         d.r(f), d.d(f, {
-            load_ipython_extension: () => y,
+            load_ipython_extension: () => m,
             remove_empty_cells: () => u
         });
         var t = d(527),
             e = d.n(t),
             n = d(290),
             r = d.n(n),
             o = d(761),
@@ -7396,12 +7402,12 @@
 
         function h() {
             (0, o.initialize_cell_extension)();
             var t, n = new i.CreateAssignmentToolbar;
             n.register(), console.log("Are we a taskbook?"), console.log(e().notebook.metadata), console.log(p()), p() ? (n.activate(), (new a.TaskMenubar).activate(), s.shortcuts.disable_add_cell_on_execute(), r().on("before_save.Notebook", u)) : (t = e().notebook.metadata).hasOwnProperty("nbassignment") && t.nbassignment.hasOwnProperty("type") && "template" === t.nbassignment.type && (n.activate(), (new a.TemplateMenubar).activate(), s.shortcuts.disable_add_cell_on_execute(), r().on("before_save.Notebook", u))
         }
 
-        function y() {
+        function m() {
             null !== e() && void 0 !== e() && e().notebook._fully_loaded ? h() : r().on("notebook_loaded.Notebook", h)
         }
     })(), f
 })()));
```

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/static/nbextensions/tree/student/main.js` & `e2xgrader-0.3.0.dev2/e2xgrader/static/nbextensions/tree/student/main.js`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/static/nbextensions/tree/student_exam/main.js` & `e2xgrader-0.3.0.dev2/e2xgrader/static/nbextensions/tree/student_exam/main.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,20 +1,20 @@
 define(["jquery", "base/js/namespace", "notebook/js/notebook"], ((e, t, n) => (() => {
     var r = {
             526: (e, t, n) => {
                 "use strict";
                 n.d(t, {
-                    Z: () => s
+                    Z: () => i
                 });
                 var r = n(601),
                     o = n.n(r),
                     a = n(609),
-                    i = n.n(a)()(o());
-                i.push([e.id, "#notebook_toolbar {\n  display: none !important;\n}\n\n.clusters_tab_link {\n  display: none !important;\n}\n\n#shutdown_widget {\n  display: none !important;\n}\n", ""]);
-                const s = i
+                    s = n.n(a)()(o());
+                s.push([e.id, "#notebook_toolbar {\n  display: none !important;\n}\n\n.clusters_tab_link {\n  display: none !important;\n}\n\n#shutdown_widget {\n  display: none !important;\n}\n", ""]);
+                const i = s
             },
             609: e => {
                 "use strict";
                 e.exports = function(e) {
                     var t = [];
                     return t.toString = function() {
                         return this.map((function(t) {
@@ -22,23 +22,23 @@
                                 r = void 0 !== t[5];
                             return t[4] && (n += "@supports (".concat(t[4], ") {")), t[2] && (n += "@media ".concat(t[2], " {")), r && (n += "@layer".concat(t[5].length > 0 ? " ".concat(t[5]) : "", " {")), n += e(t), r && (n += "}"), t[2] && (n += "}"), t[4] && (n += "}"), n
                         })).join("")
                     }, t.i = function(e, n, r, o, a) {
                         "string" == typeof e && (e = [
                             [null, e, void 0]
                         ]);
-                        var i = {};
+                        var s = {};
                         if (r)
-                            for (var s = 0; s < this.length; s++) {
-                                var c = this[s][0];
-                                null != c && (i[c] = !0)
+                            for (var i = 0; i < this.length; i++) {
+                                var c = this[i][0];
+                                null != c && (s[c] = !0)
                             }
                         for (var d = 0; d < e.length; d++) {
                             var u = [].concat(e[d]);
-                            r && i[u[0]] || (void 0 !== a && (void 0 === u[5] || (u[1] = "@layer".concat(u[5].length > 0 ? " ".concat(u[5]) : "", " {").concat(u[1], "}")), u[5] = a), n && (u[2] ? (u[1] = "@media ".concat(u[2], " {").concat(u[1], "}"), u[2] = n) : u[2] = n), o && (u[4] ? (u[1] = "@supports (".concat(u[4], ") {").concat(u[1], "}"), u[4] = o) : u[4] = "".concat(o)), t.push(u))
+                            r && s[u[0]] || (void 0 !== a && (void 0 === u[5] || (u[1] = "@layer".concat(u[5].length > 0 ? " ".concat(u[5]) : "", " {").concat(u[1], "}")), u[5] = a), n && (u[2] ? (u[1] = "@media ".concat(u[2], " {").concat(u[1], "}"), u[2] = n) : u[2] = n), o && (u[4] ? (u[1] = "@supports (".concat(u[4], ") {").concat(u[1], "}"), u[4] = o) : u[4] = "".concat(o)), t.push(u))
                         }
                     }, t
                 }
             },
             601: e => {
                 "use strict";
                 e.exports = function(e) {
@@ -54,16 +54,16 @@
                         if (t[r].identifier === e) {
                             n = r;
                             break
                         } return n
                 }
 
                 function r(e, r) {
-                    for (var a = {}, i = [], s = 0; s < e.length; s++) {
-                        var c = e[s],
+                    for (var a = {}, s = [], i = 0; i < e.length; i++) {
+                        var c = e[i],
                             d = r.base ? c[0] + r.base : c[0],
                             u = a[d] || 0,
                             l = "".concat(d, " ").concat(u);
                         a[d] = u + 1;
                         var p = n(l),
                             f = {
                                 css: c[1],
@@ -71,23 +71,23 @@
                                 sourceMap: c[3],
                                 supports: c[4],
                                 layer: c[5]
                             };
                         if (-1 !== p) t[p].references++, t[p].updater(f);
                         else {
                             var m = o(f, r);
-                            r.byIndex = s, t.splice(s, 0, {
+                            r.byIndex = i, t.splice(i, 0, {
                                 identifier: l,
                                 updater: m,
                                 references: 1
                             })
                         }
-                        i.push(l)
+                        s.push(l)
                     }
-                    return i
+                    return s
                 }
 
                 function o(e, t) {
                     var n = t.domAPI(t);
                     return n.update(e),
                         function(t) {
                             if (t) {
@@ -96,17 +96,17 @@
                             } else n.remove()
                         }
                 }
                 e.exports = function(e, o) {
                     var a = r(e = e || [], o = o || {});
                     return function(e) {
                         e = e || [];
-                        for (var i = 0; i < a.length; i++) {
-                            var s = n(a[i]);
-                            t[s].references--
+                        for (var s = 0; s < a.length; s++) {
+                            var i = n(a[s]);
+                            t[i].references--
                         }
                         for (var c = r(e, o), d = 0; d < a.length; d++) {
                             var u = n(a[d]);
                             0 === t[u].references && (t[u].updater(), t.splice(u, 1))
                         }
                         a = c
                     }
@@ -291,30 +291,30 @@
                         "use strict";
                         o.r(a), o.d(a, {
                             load_help_tab: () => c
                         });
                         const e = n(404);
                         var t = o.n(e);
                         const r = n(527);
-                        var i = o.n(r),
-                            s = o(804);
+                        var s = o.n(r),
+                            i = o(804);
 
                         function c() {
-                            i().notebook_list && (t()(".tab-content").append(function() {
+                            s().notebook_list && (t()(".tab-content").append(function() {
                                 const e = t()("<div/>").attr("id", "e2xhelp").addClass("tab-pane"),
                                     n = t()("<div/>").attr("id", "resources");
                                 return n.append(t()("<h4/>").append("Resources")), n.append(t()("<div/>").attr("id", "additional-links")), e.append(n), e
                             }()), t()("#tabs").append(t()("<li/>").append(t()("<a/>").attr("href", "#e2xhelp").attr("data-toggle", "tab").text("Help").on("click", (function(e) {
-                                window.history.pushState(null, null, "#e2xhelp"), s.requests.get((0, s.urlJoin)(i().notebook_list.base_url, "e2x/help/api/files")).then((e => {
+                                window.history.pushState(null, null, "#e2xhelp"), i.requests.get((0, i.urlJoin)(s().notebook_list.base_url, "e2x/help/api/files")).then((e => {
                                     let n = t()("#additional-links");
                                     n.empty();
                                     let r = t()("<ul/>");
                                     e.forEach((function(e) {
                                         var n, o;
-                                        r.append((n = (0, s.urlJoin)(i().notebook_list.base_url, "e2x/help/static/", e[1]), o = e[0], t()("<li/>").append(function(e, n, r = "_blank") {
+                                        r.append((n = (0, i.urlJoin)(s().notebook_list.base_url, "e2x/help/static/", e[1]), o = e[0], t()("<li/>").append(function(e, n, r = "_blank") {
                                             return t()("<a/>").attr("href", e).attr("target", r).text(n)
                                         }(n, o))))
                                     })), e.length > 0 ? n.append(r) : n.append("There are no additional resources!")
                                 }))
                             })))))
                         }
                     })(), e.exports = a
@@ -439,32 +439,32 @@
                             create_nbgrader_metadata: () => l,
                             get_grade_id: () => P,
                             get_nbgrader_field: () => p,
                             get_points: () => O,
                             get_schema_version: () => _,
                             is_description: () => C,
                             is_empty: () => I,
-                            is_grade: () => y,
+                            is_grade: () => v,
                             is_invalid: () => N,
                             is_locked: () => w,
                             is_nbgrader: () => d,
                             is_solution: () => b,
                             is_task: () => x,
                             is_test: () => M,
-                            nbgrader_schema_version: () => i,
-                            randomString: () => s,
+                            nbgrader_schema_version: () => s,
+                            randomString: () => i,
                             remove_nbgrader_field: () => m,
                             remove_nbgrader_metadata: () => u,
-                            set_grade: () => g,
+                            set_grade: () => y,
                             set_grade_id: () => T,
                             set_locked: () => k,
                             set_nbgrader_field: () => f,
                             set_points: () => j,
                             set_schema_version: () => h,
-                            set_solution: () => v,
+                            set_solution: () => g,
                             set_task: () => S,
                             to_description: () => J,
                             to_float: () => c,
                             to_test: () => E
                         });
                         var t = {};
                         o.r(t), o.d(t, {
@@ -472,17 +472,17 @@
                             disable_add_cell_on_execute: () => Z,
                             remove_shortcuts: () => A
                         });
                         var r = {};
                         o.r(r), o.d(r, {
                             add_username: () => D
                         });
-                        const i = 3;
+                        const s = 3;
 
-                        function s(e) {
+                        function i(e) {
                             let t, n = "",
                                 r = "abcdef0123456789";
                             for (t = 0; t < e; t++) n += r[Math.floor(Math.random() * r.length)];
                             return n
                         }
 
                         function c(e) {
@@ -514,30 +514,30 @@
                         }
 
                         function _(e) {
                             if (d(e)) return void 0 === p(e, "schema_version") ? 0 : p(e, "schema_version")
                         }
 
                         function h(e) {
-                            d(e) || l(e), f(e, "schema_version", i)
+                            d(e) || l(e), f(e, "schema_version", s)
                         }
 
                         function b(e) {
                             return p(e, "solution", !1)
                         }
 
-                        function v(e, t) {
+                        function g(e, t) {
                             f(e, "solution", t)
                         }
 
-                        function y(e) {
+                        function v(e) {
                             return p(e, "grade", !1)
                         }
 
-                        function g(e, t) {
+                        function y(e, t) {
                             f(e, "grade", t)
                         }
 
                         function x(e) {
                             return p(e, "task", !1)
                         }
 
@@ -558,39 +558,39 @@
                         }
 
                         function j(e, t) {
                             f(e, "points", Math.max(0, c(t)))
                         }
 
                         function P(e) {
-                            return p(e, "grade_id", "cell-" + s(16))
+                            return p(e, "grade_id", "cell-" + i(16))
                         }
 
                         function T(e, t) {
                             f(e, "grade_id", t)
                         }
 
                         function M(e) {
-                            return y(e) && w(e) && !b(e)
+                            return v(e) && w(e) && !b(e)
                         }
 
                         function E(e) {
-                            remove_metadata(e), h(e), v(e, !1), g(e, !0), k(e, !0)
+                            remove_metadata(e), h(e), g(e, !1), y(e, !0), k(e, !0)
                         }
 
                         function C(e) {
-                            return w(e) && !y(e) && !b(e)
+                            return w(e) && !v(e) && !b(e)
                         }
 
                         function J(e) {
-                            remove_metadata(e), h(e), v(e, !1), g(e, !1), k(e, !0)
+                            remove_metadata(e), h(e), g(e, !1), y(e, !1), k(e, !0)
                         }
 
                         function N(e) {
-                            return !(x(e) || b(e) && y(e) || (!b(e) || "code" === e.cell_type) && (!y(e) || "code" === e.cell_type))
+                            return !(x(e) || b(e) && v(e) || (!b(e) || "code" === e.cell_type) && (!v(e) || "code" === e.cell_type))
                         }
 
                         function I(e) {
                             return 0 == e.get_text().length
                         }
                         const R = n(527);
                         var U = o.n(R);
@@ -600,17 +600,19 @@
                             if ("command" === e) return U().keyboard_manager.command_shortcuts;
                             if ("edit" === e) return U().keyboard_manager.edit_shortcuts;
                             throw new Error("Mode needs to be either 'command' or 'edit'")
                         }
 
                         function A(e, ...t) {
                             const n = q(e);
-                            for (const e of t) try {
-                                n.remove_shortcut(e)
-                            } catch (e) {}
+                            for (const r of t) try {
+                                n.remove_shortcut(r)
+                            } catch (t) {
+                                console.log("Error removing shortcut", r, "from", e, "mode:", t.message)
+                            }
                         }
 
                         function F(e, t, n, r, o = "zz") {
                             q(e).add_shortcut(t, {
                                 help: r,
                                 help_index: o,
                                 handler: n
@@ -624,15 +626,15 @@
                                 else {
                                     let t = this.get_selected_cell();
                                     e = this.find_cell_index(t), t.execute()
                                 }
                                 e = Math.min(e + 1, this.ncells() - 1), this.select(e), this.focus_cell()
                             };
                             const e = ["alt-enter", "shift-enter"];
-                            A("edit", e), A("command", e);
+                            A("edit", ...e), A("command", ...e);
                             const t = "run cell",
                                 n = function(e) {
                                     return U().notebook.execute_cell_and_select_below_without_insert(), !1
                                 };
                             for (const r of e) F("edit", r, n, t), F("command", r, n, t)
                         }
                         var z = o(804);
@@ -686,36 +688,36 @@
     }, a.o = (e, t) => Object.prototype.hasOwnProperty.call(e, t), a.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
     }, a.nc = void 0;
-    var i = {};
+    var s = {};
     return (() => {
         "use strict";
-        a.r(i), a.d(i, {
-            load_ipython_extension: () => v
+        a.r(s), a.d(s, {
+            load_ipython_extension: () => g
         });
         var e = a(62),
             t = a.n(e),
             n = a(36),
             r = a.n(n),
             o = a(793),
-            s = a.n(o),
+            i = a.n(o),
             c = a(892),
             d = a.n(c),
             u = a(173),
             l = a.n(u),
             p = a(464),
             f = a.n(p),
             m = a(526),
             _ = {};
-        _.styleTagTransform = f(), _.setAttributes = d(), _.insert = s().bind(null, "head"), _.domAPI = r(), _.insertStyleElement = l(), t()(m.Z, _), m.Z && m.Z.locals && m.Z.locals;
+        _.styleTagTransform = f(), _.setAttributes = d(), _.insert = i().bind(null, "head"), _.domAPI = r(), _.insertStyleElement = l(), t()(m.Z, _), m.Z && m.Z.locals && m.Z.locals;
         var h = a(414),
             b = a(426);
 
-        function v() {
+        function g() {
             (0, h.load_help_tab)(), b.username.add_username()
         }
-    })(), i
+    })(), s
 })()));
```

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/static/nbextensions/tree/teacher/main.js` & `e2xgrader-0.3.0.dev2/e2xgrader/static/nbextensions/tree/teacher/main.js`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/tests/apps/test_activatemodeapp.py` & `e2xgrader-0.3.0.dev2/e2xgrader/tests/apps/test_activatemodeapp.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/tests/apps/test_baseapp.py` & `e2xgrader-0.3.0.dev2/e2xgrader/tests/apps/test_baseapp.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/tests/apps/test_deactivatemodeapp.py` & `e2xgrader-0.3.0.dev2/e2xgrader/tests/apps/test_deactivatemodeapp.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/tests/apps/test_e2xgraderapp.py` & `e2xgrader-0.3.0.dev2/e2xgrader/tests/apps/test_e2xgraderapp.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/tests/apps/test_e2xmanager.py` & `e2xgrader-0.3.0.dev2/e2xgrader/tests/apps/test_e2xmanager.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/tests/apps/test_showmodeapp.py` & `e2xgrader-0.3.0.dev2/e2xgrader/tests/apps/test_showmodeapp.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/tests/apps/test_togglemodeapp.py` & `e2xgrader-0.3.0.dev2/e2xgrader/tests/apps/test_togglemodeapp.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/tests/exchange/test_hash_utils.py` & `e2xgrader-0.3.0.dev2/e2xgrader/tests/exchange/test_hash_utils.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/tests/exchange/test_submit.py` & `e2xgrader-0.3.0.dev2/e2xgrader/tests/exchange/test_submit.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/tests/exchange/test_utils.py` & `e2xgrader-0.3.0.dev2/e2xgrader/tests/exchange/test_utils.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/tests/exchange/utils.py` & `e2xgrader-0.3.0.dev2/e2xgrader/tests/exchange/utils.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/tests/exporters/filters/test_highlight.py` & `e2xgrader-0.3.0.dev2/e2xgrader/tests/exporters/filters/test_highlight.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/tests/extensions/test_utils.py` & `e2xgrader-0.3.0.dev2/e2xgrader/tests/extensions/test_utils.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/tests/graders/test_base.py` & `e2xgrader-0.3.0.dev2/e2xgrader/tests/graders/test_base.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/tests/graders/test_code.py` & `e2xgrader-0.3.0.dev2/e2xgrader/tests/graders/test_code.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/tests/graders/test_multiplechoice.py` & `e2xgrader-0.3.0.dev2/e2xgrader/tests/graders/test_multiplechoice.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/tests/graders/test_singlechoice.py` & `e2xgrader-0.3.0.dev2/e2xgrader/tests/graders/test_singlechoice.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/tests/preprocessors/test_clearhiddentests.py` & `e2xgrader-0.3.0.dev2/e2xgrader/tests/preprocessors/test_clearhiddentests.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/tests/preprocessors/test_clearsolutions.py` & `e2xgrader-0.3.0.dev2/e2xgrader/tests/preprocessors/test_clearsolutions.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/tests/preprocessors/test_extractattachments.py` & `e2xgrader-0.3.0.dev2/e2xgrader/tests/preprocessors/test_extractattachments.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/tests/preprocessors/test_filtercellsbyid.py` & `e2xgrader-0.3.0.dev2/e2xgrader/tests/preprocessors/test_filtercellsbyid.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/tests/preprocessors/test_filtertests.py` & `e2xgrader-0.3.0.dev2/e2xgrader/tests/preprocessors/test_filtertests.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/tests/preprocessors/test_unscramble.py` & `e2xgrader-0.3.0.dev2/e2xgrader/tests/preprocessors/test_unscramble.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/tests/preprocessors/test_validateextracells.py` & `e2xgrader-0.3.0.dev2/e2xgrader/tests/preprocessors/test_validateextracells.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/tests/server_extensions/apps/diagram_editor/test_diagrameditor.py` & `e2xgrader-0.3.0.dev2/e2xgrader/tests/server_extensions/apps/diagram_editor/test_diagrameditor.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/tests/server_extensions/apps/validate_assignment/test_validator.py` & `e2xgrader-0.3.0.dev2/e2xgrader/tests/server_extensions/apps/validate_assignment/test_validator.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/tests/test_utils/cells.py` & `e2xgrader-0.3.0.dev2/e2xgrader/tests/test_utils/cells.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/tests/test_utils/test_utils.py` & `e2xgrader-0.3.0.dev2/e2xgrader/tests/test_utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/tests/utils/test_mode.py` & `e2xgrader-0.3.0.dev2/e2xgrader/tests/utils/test_mode.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/utils/extra_cells.py` & `e2xgrader-0.3.0.dev2/e2xgrader/utils/extra_cells.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/utils/mode.py` & `e2xgrader-0.3.0.dev2/e2xgrader/utils/mode.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/e2xgrader/utils/nbgrader_cells.py` & `e2xgrader-0.3.0.dev2/e2xgrader/utils/nbgrader_cells.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/.gitignore` & `e2xgrader-0.3.0.dev2/.gitignore`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/LICENSE` & `e2xgrader-0.3.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/README.md` & `e2xgrader-0.3.0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.3.0.dev1/pyproject.toml` & `e2xgrader-0.3.0.dev2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     "e2xgrader/static"
 ]
 
 [tool.tbump]
 github_url = "https://github.com/Digiklausur/e2xgrader/"
 
 [tool.tbump.version]
-current = "0.3.0-dev1"
+current = "0.3.0-dev2"
 
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
```

### Comparing `e2xgrader-0.3.0.dev1/PKG-INFO` & `e2xgrader-0.3.0.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e2xgrader
-Version: 0.3.0.dev1
+Version: 0.3.0.dev2
 Summary: An addon for nbgrader
 Project-URL: Source, https://github.com/Digiklausur/e2xgrader
 Project-URL: Documentation, https://e2xgrader.readthedocs.io/en/latest/
 Project-URL: Issues, https://github.com/Digiklausur/e2xgrader/issues
 Project-URL: Pypi, https://pypi.org/project/e2xgrader/
 Author-email: Tim Metzler <tim.metzler@h-brs.de>
 License-Expression: MIT
```

